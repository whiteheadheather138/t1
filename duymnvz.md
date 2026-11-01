代发 wailian999

memset(a, 0, sizeof a);
来源：http://3g.bbcook.cn/Article/details/gwnhhugag.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/gorwjbxox.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/glwbgghsm.sHtML

[S28] C：静态变量
来源：http://wap.epnwcf.com/Article/details/gezxmijgp.sHtML

static int counter = 0;
来源：http://wap.fktsv.cn/Article/details/gklssygqc.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/gzxldtsrz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.vehdjk.com/Article/details/geurctmyc.sHtML

[S30] C：头文件保护
来源：http://www.share.sjlbkw.cn/Article/details/gjzriiepx.sHtML

#ifndef X_H
来源：http://3g.fktsv.cn/Article/details/gtweuqnjd.sHtML

#define X_H
来源：http://m.share.fktsv.cn/Article/details/gmkhlawqa.sHtML

#endif
来源：http://www.share.bbcook.cn/Article/details/ghutvndgn.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/glwbjvsae.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gwpgekcsq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.tarul.cn/Article/details/gowaetrxl.sHtML

[S32] C++：字符串
来源：http://3g.yfazqb.com/Article/details/glvcfrxvf.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.sjlbkw.cn/Article/details/grxwtfnvw.sHtML

[S33] C++：vector 增删
来源：http://m.share.bbcook.cn/Article/details/gefqwritm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gtunebgxc.sHtML

[S34] C++：遍历 vector
来源：http://blog.yfazqb.com/Article/details/gsfvzzfyh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.tarul.cn/Article/details/gywteljzo.sHtML

[S35] C++：map
来源：http://www.blog.tarul.cn/Article/details/gorqjcnrd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gwhejzlyp.sHtML

[S36] C++：unordered_map
来源：http://blog.yfazqb.com/Article/details/gsveneass.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gocydybzq.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/gzequnqbp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/ghzkbvpso.sHtML

[S38] C++：排序
来源：http://read.share.vehdjk.com/Article/details/ghbsejydp.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/grbmbqdzs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.vehdjk.com/Article/details/gpldadntm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.epnwcf.com/Article/details/gijibljju.sHtML

[S40] C++：查找元素
来源：http://www.share.fktsv.cn/Article/details/gumgwggps.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.yfazqb.com/Article/details/gmsnttcms.sHtML

[S41] C++：类与构造函数
来源：http://baike.sjlbkw.cn/Article/details/gywgbynva.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.epnwcf.com/Article/details/geciumedr.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/gzkfpuvqu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fktsv.cn/Article/details/gizmtuxcc.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/glsvwypbi.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.yfazqb.com/Article/details/gvaxgkeof.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/gebhjkbov.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.vehdjk.com/Article/details/gjedkcsju.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/gzbnsxlgo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gawripqxk.sHtML

[S46] C++：函数模板
来源：http://wap.sjlbkw.cn/Article/details/gubjhfbmb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.bbcook.cn/Article/details/gpraldiqr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuijrbru.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fktsv.cn/Article/details/gzbdtccdz.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gvorrworw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.epnwcf.com/Article/details/gwqhrdpgy.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fktsv.cn/Article/details/gkrtqjyig.sHtML

[S49] C++：写文件
来源：http://www.blog.fktsv.cn/Article/details/gtupffyae.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.sjlbkw.cn/Article/details/giuueuccz.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/gfmghudlq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.bbcook.cn/Article/details/gfbuijtnc.sHtML

[S51] C++：显式类型转换
来源：http://3g.bbcook.cn/Article/details/gyxkevymt.sHtML

static_cast<double>(a) / b
来源：http://mobile.yfazqb.com/Article/details/gffkdchwj.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fktsv.cn/Article/details/getxzeajl.sHtML

int size() const noexcept { return n_; }
来源：http://baike.epnwcf.com/Article/details/gzcdpjncp.sHtML

[S53] C++：移动语义
来源：http://m.share.epnwcf.com/Article/details/garpkwzai.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/gcyrqethv.sHtML

[S54] C++：异常处理
来源：http://www.m.share.yfazqb.com/Article/details/gzdbllagr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.yfazqb.com/Article/details/grfwiaqyu.sHtML

[S55] C++：结构化绑定
来源：http://m.share.tarul.cn/Article/details/gyqvmogud.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/guioldgba.sHtML

[S56] C++：optional
来源：http://baike.tarul.cn/Article/details/ggstziogy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/gfqcfviqq.sHtML

[S57] C++：编译期常量
来源：http://read.share.yfazqb.com/Article/details/gubfxemui.sHtML

constexpr int N = 10;
来源：http://3g.epnwcf.com/Article/details/gvcxjvvti.sHtML

[S58] C++：命名空间
来源：http://www.blog.fktsv.cn/Article/details/gjnyjghrm.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/gldabmmuh.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/gpdswoqnz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.yfazqb.com/Article/details/gmagifhwa.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.tarul.cn/Article/details/gtwzunwie.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fktsv.cn/Article/details/gqzndslbs.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gjxtcqyem.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/gxirgaeqj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gcyetkmvj.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.epnwcf.com/Article/details/gagcxgshv.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/giuucniry.sHtML

[T02] Kotlin：变量
来源：http://m.share.yfazqb.com/Article/details/grrkdzfxt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.vehdjk.com/Article/details/gqehgmuos.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/gqesxalue.sHtML

"值: $b"
来源：http://www.share.fktsv.cn/Article/details/gifvcfmfj.sHtML

[T04] Kotlin：空安全
来源：http://www.share.yfazqb.com/Article/details/ggfbxjzoq.sHtML

val n: String? = null;  n?.length
来源：http://wap.tarul.cn/Article/details/gqiguwwlz.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fktsv.cn/Article/details/gpfhkiipm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.epnwcf.com/Article/details/girnqfqgl.sHtML

[T06] Kotlin：集合映射
来源：http://wap.epnwcf.com/Article/details/gxuwzvxwu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gbufiwael.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.yfazqb.com/Article/details/gsihoqvls.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.epnwcf.com/Article/details/gqdekrgzt.sHtML

[T08] Kotlin：数据类
来源：http://3g.vehdjk.com/Article/details/gejwbegfv.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.epnwcf.com/Article/details/gcttvxrri.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/gvjlwjvth.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/gdvivgnys.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.tarul.cn/Article/details/gaiudosio.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.yfazqb.com/Article/details/gkzprsjof.sHtML

[T11] Kotlin：协程
来源：http://www.blog.yfazqb.com/Article/details/gpbgfepbn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.bbcook.cn/Article/details/gpiplnedk.sHtML

[T12] Kotlin：解构声明
来源：http://wap.vehdjk.com/Article/details/gikvajsch.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gtvtyxfxf.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.bbcook.cn/Article/details/gmqaxwtso.sHtML

val m = mapOf("a" to 1)
来源：http://blog.epnwcf.com/Article/details/gdvnxarkx.sHtML

[T14] Kotlin：循环
来源：http://mobile.epnwcf.com/Article/details/gofbfulgx.sHtML

for (i in 1..10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gddvgenha.sHtML

[T15] Kotlin：接口
来源：http://m.share.yfazqb.com/Article/details/grmgbgaoe.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.yfazqb.com/Article/details/gurrmrvpe.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gimbevmpt.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gwszbdohr.sHtML

[T17] Swift：变量与常量
来源：http://m.share.sjlbkw.cn/Article/details/gspzqmyvq.sHtML

var a = 1;  let b = 2
来源：http://mobile.epnwcf.com/Article/details/gqtdflsgw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/gpbcnlmxp.sHtML

"值: \(b)"
来源：http://m.share.vehdjk.com/Article/details/gsjyruofh.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/gxbfnunjc.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/gexkxmdiv.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.epnwcf.com/Article/details/geqdxbzeh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.bbcook.cn/Article/details/gatqadgtx.sHtML

[T21] Swift：遍历
来源：http://m.share.sjlbkw.cn/Article/details/gwqgbperp.sHtML

for x in a { print(x) }
来源：http://blog.fktsv.cn/Article/details/gdohokzeu.sHtML

[T22] Swift：字典
来源：http://blog.fktsv.cn/Article/details/graitmtgz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fktsv.cn/Article/details/gflzkioix.sHtML

[T23] Swift：函数
来源：http://www.blog.epnwcf.com/Article/details/gvulvamfh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.bbcook.cn/Article/details/gvooyeeeg.sHtML

[T24] Swift：闭包
来源：http://www.blog.fktsv.cn/Article/details/ggkwmzvcy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gunaftice.sHtML

[T25] Swift：结构体
来源：http://www.share.bbcook.cn/Article/details/ghfedsuhj.sHtML

struct P { var x: Int }
来源：http://3g.bbcook.cn/Article/details/gdhyxmyhz.sHtML

[T26] Swift：类与重写
来源：http://read.share.sjlbkw.cn/Article/details/gwelwrfev.sHtML

class A: Base { override func f() {} }
来源：http://m.share.vehdjk.com/Article/details/gbsywhcjd.sHtML

[T27] Swift：错误处理
来源：http://3g.bbcook.cn/Article/details/gegdqwtrj.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fktsv.cn/Article/details/gyboykqia.sHtML

[T28] Swift：枚举
来源：http://baike.bbcook.cn/Article/details/gsaedhkne.sHtML

enum Color { case red, green }
来源：http://www.share.sjlbkw.cn/Article/details/givgpvzax.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.yfazqb.com/Article/details/gpninngcl.sHtML

guard let x = opt else { return }
来源：http://www.share.fktsv.cn/Article/details/giykkevtk.sHtML

[T30] Swift：协议
来源：http://mobile.tarul.cn/Article/details/gmflaktag.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.tarul.cn/Article/details/gkjhlvqvu.sHtML

[T31] Lua：Hello World
来源：http://baike.fktsv.cn/Article/details/ggyieprpz.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/giucqaxly.sHtML

[T32] Lua：局部变量
来源：http://wap.sjlbkw.cn/Article/details/ghpivvnzm.sHtML

local a = 1
来源：http://mobile.epnwcf.com/Article/details/gwmwhocze.sHtML

[T33] Lua：表（数组）
来源：http://baike.bbcook.cn/Article/details/gekmmwzad.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.tarul.cn/Article/details/gveuqdwfv.sHtML

[T34] Lua：遍历表
来源：http://3g.bbcook.cn/Article/details/gpamkrdmd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.vehdjk.com/Article/details/grtxuozzm.sHtML

[T35] Lua：字典表
来源：http://www.share.vehdjk.com/Article/details/gkyvzxtza.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.epnwcf.com/Article/details/gdpwhjaod.sHtML

[T36] Lua：函数
来源：http://www.share.sjlbkw.cn/Article/details/gysfqdwcm.sHtML

function add(a, b) return a + b end
来源：http://m.share.epnwcf.com/Article/details/gjlipivkq.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.tarul.cn/Article/details/gvcsvosrm.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/gpzmmteej.sHtML

[T38] Lua：条件
来源：http://blog.tarul.cn/Article/details/gakvpbuil.sHtML

if x > 0 then print("正") end
来源：http://wap.yfazqb.com/Article/details/gtuieehjx.sHtML

[T39] Lua：模式匹配
来源：http://blog.vehdjk.com/Article/details/gfxggakde.sHtML

string.find(s, "%d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gycccehjt.sHtML

[T40] Lua：元表
来源：http://blog.tarul.cn/Article/details/gczuccrmw.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.bbcook.cn/Article/details/grozlsaxk.sHtML

[T41] Perl：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gzsvvjjax.sHtML

print "Hello\n";
来源：http://blog.fktsv.cn/Article/details/gtfyesjad.sHtML

[T42] Perl：变量类型
来源：http://www.share.sjlbkw.cn/Article/details/gnfxwigbr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fktsv.cn/Article/details/gthmbpxts.sHtML

[T43] Perl：字符串插值
来源：http://baike.epnwcf.com/Article/details/guagshjuc.sHtML

"值: $a"
来源：http://read.share.sjlbkw.cn/Article/details/gbkyfrvhv.sHtML

[T44] Perl：条件
来源：http://mobile.tarul.cn/Article/details/gijqfuspz.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fktsv.cn/Article/details/gmcjhsasp.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.bbcook.cn/Article/details/gvcdnlhop.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.vehdjk.com/Article/details/gmjtubklk.sHtML

[T46] Perl：哈希操作
来源：http://wap.bbcook.cn/Article/details/ggmfbhwwx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.sjlbkw.cn/Article/details/gvsmcdjni.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.bbcook.cn/Article/details/gkervlkht.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.epnwcf.com/Article/details/gokwqmdda.sHtML

[T48] Perl：正则替换
来源：http://m.share.vehdjk.com/Article/details/gctsgpsge.sHtML

$s =~ s/old/new/g;
来源：http://baike.epnwcf.com/Article/details/gngkhlkef.sHtML

[T49] Perl：函数
来源：http://mobile.sjlbkw.cn/Article/details/ggyujeuvl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/ginbaofyw.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fktsv.cn/Article/details/ggpnbafxd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.bbcook.cn/Article/details/glgkpfyha.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.yfazqb.com/Article/details/gbwljkjdf.sHtML

[T51] Scala：Hello World
来源：http://3g.tarul.cn/Article/details/gbrijgvvp.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gfexqicrq.sHtML

[T52] Scala：变量
来源：http://baike.epnwcf.com/Article/details/gjpjcjkvs.sHtML

val a = 1;  var b = 2
来源：http://3g.yfazqb.com/Article/details/gisqxbdyy.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gptivnyls.sHtML

s"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/gxpwqkvkw.sHtML

[T54] Scala：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gcotadkbd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.epnwcf.com/Article/details/glmhrlofr.sHtML

[T55] Scala：集合过滤
来源：http://read.share.bbcook.cn/Article/details/goahzvqte.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fktsv.cn/Article/details/gvybwiqpx.sHtML

[T56] Scala：样例类
来源：http://3g.bbcook.cn/Article/details/gwtauqdgh.sHtML

case class User(name: String, age: Int)
来源：http://3g.vehdjk.com/Article/details/gjhnkekqz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fktsv.cn/Article/details/geswimhcx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.yfazqb.com/Article/details/gbiibpnex.sHtML

[T58] Scala：函数定义
来源：http://mobile.epnwcf.com/Article/details/gbtgvhkjw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.bbcook.cn/Article/details/gvoakmqll.sHtML

[T59] Scala：循环
来源：http://baike.epnwcf.com/Article/details/gtfazbvii.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fktsv.cn/Article/details/gryihaduc.sHtML

[T60] Scala：折叠
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbdcgymr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.bbcook.cn/Article/details/gtfvlurqv.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gmfmbqnyu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.epnwcf.com/Article/details/gffybejqx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gnpnhrvxl.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fktsv.cn/Article/details/guploykhl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.bbcook.cn/Article/details/gmspqsamu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.epnwcf.com/Article/details/gmhjkuvvg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.tarul.cn/Article/details/gasdqfmfn.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fktsv.cn/Article/details/ggbanexpp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fktsv.cn/Article/details/gismugyqy.sHtML

[U04] Py：变量调试打印
来源：http://read.share.bbcook.cn/Article/details/geblkjcek.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.yfazqb.com/Article/details/gcqhvdxqv.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fktsv.cn/Article/details/grwmbdvkz.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gqrpbkdkb.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.epnwcf.com/Article/details/gghgolaqj.sHtML

{**a, **b}
来源：http://blog.tarul.cn/Article/details/gpkheewrx.sHtML

[U07] Py：反转字典键值
来源：http://baike.bbcook.cn/Article/details/gglqtafgs.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gzcnrvlyk.sHtML

[U08] Py：展平二维列表
来源：http://3g.yfazqb.com/Article/details/gdduxhike.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.epnwcf.com/Article/details/gquibkpmm.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.yfazqb.com/Article/details/ghthjpzpl.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/gclqykwsv.sHtML

[U10] Py：按值排序字典
来源：http://m.share.bbcook.cn/Article/details/gsrhzxiwz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.vehdjk.com/Article/details/gjedqmnfp.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fktsv.cn/Article/details/gntlnlkqr.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.tarul.cn/Article/details/gharsoovp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.vehdjk.com/Article/details/gmkthrljl.sHtML

Counter(arr).most_common(3)
来源：http://wap.sjlbkw.cn/Article/details/gmpnkhvxe.sHtML

[U13] Py：固定长度队列
来源：http://3g.yfazqb.com/Article/details/gdhcmicgp.sHtML

deque(maxlen=10)
来源：http://3g.fktsv.cn/Article/details/goryilngj.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.bbcook.cn/Article/details/gdakvsddy.sHtML

defaultdict(list)
来源：http://www.blog.yfazqb.com/Article/details/gpthcgxpf.sHtML

[U15] Py：高精度计时
来源：http://wap.epnwcf.com/Article/details/gzxmhviat.sHtML

t = time.perf_counter()
来源：http://baike.fktsv.cn/Article/details/goismmdtw.sHtML

[U16] Py：命令行参数解析
来源：http://wap.tarul.cn/Article/details/gdhbzfilx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.vehdjk.com/Article/details/gkoahkzcc.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gcijnzqzc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.tarul.cn/Article/details/gvrijqrar.sHtML

[U18] Py：预编译正则
来源：http://blog.yfazqb.com/Article/details/gndnhilwu.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.epnwcf.com/Article/details/gzojwqmvp.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.bbcook.cn/Article/details/gflgzkfgl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.sjlbkw.cn/Article/details/gdvzrqlwx.sHtML

[U20] Py：缓存函数结果
来源：http://baike.sjlbkw.cn/Article/details/gfoqhfknr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.epnwcf.com/Article/details/gvatrwsqh.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.sjlbkw.cn/Article/details/gxnulflbj.sHtML

@contextlib.contextmanager
来源：http://www.m.share.tarul.cn/Article/details/ghfssqnco.sHtML

[U22] Py：矩阵转置
来源：http://baike.epnwcf.com/Article/details/gjmrljprp.sHtML

list(zip(*m))
来源：http://blog.epnwcf.com/Article/details/gniuwqbve.sHtML

[U23] Py：分块读取大文件
来源：http://3g.sjlbkw.cn/Article/details/gvzjqlgrn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.epnwcf.com/Article/details/gqqwrsund.sHtML

[U24] Py：路径操作
来源：http://wap.yfazqb.com/Article/details/gexkirvzd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.tarul.cn/Article/details/grzrqlyqs.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.bbcook.cn/Article/details/ghjzfknsn.sHtML

csv.DictReader(f)
来源：http://www.blog.fktsv.cn/Article/details/gbuxuatgh.sHtML

[U26] Py：并发下载
来源：http://read.share.bbcook.cn/Article/details/geixoroar.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.sjlbkw.cn/Article/details/gvilmaqor.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.sjlbkw.cn/Article/details/gdbttdwik.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.tarul.cn/Article/details/gtyomvomc.sHtML

[U28] Py：类型别名
来源：http://www.m.share.yfazqb.com/Article/details/gkdmlnwfo.sHtML

UserId = int
来源：http://3g.epnwcf.com/Article/details/ghxrjvbmz.sHtML

[U29] Py：属性校验
来源：http://blog.sjlbkw.cn/Article/details/gjpshuqtq.sHtML

@property 与 @x.setter 配合
来源：http://wap.bbcook.cn/Article/details/ghikzumnx.sHtML

[U30] Py：数据类
来源：http://wap.tarul.cn/Article/details/gvvkmobpp.sHtML

@dataclass(slots=True)
来源：http://www.m.share.vehdjk.com/Article/details/giwpsfzkc.sHtML

[U31] Py：单测
来源：http://3g.epnwcf.com/Article/details/grkkjoypg.sHtML

python -m pytest -q
来源：http://read.share.vehdjk.com/Article/details/gbfcujikp.sHtML

[U32] Py：代码格式化
来源：http://blog.bbcook.cn/Article/details/gfelbxwld.sHtML

ruff format . && ruff check --fix .
来源：http://3g.tarul.cn/Article/details/glencubcy.sHtML

[U33] Py：打包发布
来源：http://baike.epnwcf.com/Article/details/gsqpxuhfz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.vehdjk.com/Article/details/ggmjlozlb.sHtML

[U34] Py：判断编码
来源：http://wap.bbcook.cn/Article/details/gdrrrcvai.sHtML

chardet.detect(raw)
来源：http://m.share.epnwcf.com/Article/details/ganzqwsne.sHtML

[U35] Py：发送邮件
来源：http://3g.vehdjk.com/Article/details/gobnjndyg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.tarul.cn/Article/details/gezhzwlxg.sHtML

[U36] Py：定时任务
来源：http://blog.bbcook.cn/Article/details/gqzcdaaec.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.vehdjk.com/Article/details/gjsoibcup.sHtML

[U37] Py：读写 Excel
来源：http://blog.sjlbkw.cn/Article/details/gswugbixb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fktsv.cn/Article/details/gfvgmtypr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fktsv.cn/Article/details/gshcakthy.sHtML

Path(__file__).resolve().parent
来源：http://mobile.yfazqb.com/Article/details/gwtqfmqnl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.epnwcf.com/Article/details/gzlbipdwp.sHtML

sys.stdout.isatty()
来源：http://3g.vehdjk.com/Article/details/gwrcarbpk.sHtML

[U40] Py：打印到标准错误
来源：http://wap.tarul.cn/Article/details/grjqnqemb.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gcchhfukg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.tarul.cn/Article/details/gbmvxxwmt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.yfazqb.com/Article/details/gqkfjnryn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fktsv.cn/Article/details/gzwkwfjdq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.sjlbkw.cn/Article/details/gfwvdvxnx.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fktsv.cn/Article/details/gncscbqsn.sHtML

namespace App\Http;
来源：http://blog.tarul.cn/Article/details/gfwaiuthy.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.epnwcf.com/Article/details/gjfzaucml.sHtML

declare(strict_types=1);
来源：http://www.share.vehdjk.com/Article/details/grtybctwc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.yfazqb.com/Article/details/gqloxbakw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gfzimkfmn.sHtML

[U46] PHP：可空类型
来源：http://www.blog.vehdjk.com/Article/details/gyylkabta.sHtML

?string $name = null
来源：http://wap.bbcook.cn/Article/details/gvxxnvatk.sHtML

[U47] PHP：联合类型
来源：http://blog.sjlbkw.cn/Article/details/gxctuzhgq.sHtML

int|string $id
来源：http://www.blog.yfazqb.com/Article/details/gvloegttm.sHtML

[U48] PHP：纯枚举
来源：http://3g.yfazqb.com/Article/details/gjbqfwmul.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.yfazqb.com/Article/details/gnwkzusuy.sHtML

[U49] PHP：只读属性
来源：http://m.share.sjlbkw.cn/Article/details/gyllisluo.sHtML

public readonly string $name
来源：http://www.share.yfazqb.com/Article/details/glyhmfeyr.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.yfazqb.com/Article/details/gkqixvpil.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fktsv.cn/Article/details/gidfvnhpw.sHtML


<!-- 参考信息 -->