代发 wailian999

#ifndef X_H
来源：http://mobile.yfazqb.com/Article/details/gxcxkgjaz.sHtML

#define X_H
来源：http://read.share.fktsv.cn/Article/details/gdiuyiwdh.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/gpuuyvwwm.sHtML

[S31] C++：Hello World
来源：http://read.share.fktsv.cn/Article/details/geregxdvf.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gtinviiyf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/golvxsbxr.sHtML

[S32] C++：字符串
来源：http://read.share.tarul.cn/Article/details/gqozoytxv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fktsv.cn/Article/details/guzqbzjlo.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/geqhkdczy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.epnwcf.com/Article/details/gdbdsdtyx.sHtML

[S34] C++：遍历 vector
来源：http://baike.epnwcf.com/Article/details/gbxwlaoqb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/gqluaiecq.sHtML

[S35] C++：map
来源：http://www.m.share.bbcook.cn/Article/details/gedsvhykw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/gnabhcxkn.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/ghevkdmjl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gdacqkkki.sHtML

[S37] C++：set
来源：http://3g.tarul.cn/Article/details/gyatxcrbi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fktsv.cn/Article/details/gmyojasri.sHtML

[S38] C++：排序
来源：http://mobile.sjlbkw.cn/Article/details/gbicqpkjk.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.bbcook.cn/Article/details/ghofwitay.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.vehdjk.com/Article/details/gajbxyhwp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.sjlbkw.cn/Article/details/gdoxgvdgr.sHtML

[S40] C++：查找元素
来源：http://baike.yfazqb.com/Article/details/gtdyfwrnt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.sjlbkw.cn/Article/details/glegivlhg.sHtML

[S41] C++：类与构造函数
来源：http://3g.tarul.cn/Article/details/gkktkvvnz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fktsv.cn/Article/details/glaanjgbm.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.epnwcf.com/Article/details/gddgrgtmq.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.yfazqb.com/Article/details/ggdjtrmvn.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/ghiuokqxo.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.vehdjk.com/Article/details/giqhsfjrc.sHtML

[S44] C++：引用传参
来源：http://m.share.yfazqb.com/Article/details/gliyrrsxy.sHtML

void inc(int &x) { ++x; }
来源：http://wap.tarul.cn/Article/details/ghxjthbrb.sHtML

[S45] C++：lambda
来源：http://read.share.bbcook.cn/Article/details/gppzjwvlu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/gdkzfxzhi.sHtML

[S46] C++：函数模板
来源：http://3g.tarul.cn/Article/details/ghxqhyshk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.vehdjk.com/Article/details/glkjgmlms.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.tarul.cn/Article/details/gcxvbnjky.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.tarul.cn/Article/details/gldrgbkti.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gffrhetjg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/gfebgevij.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.tarul.cn/Article/details/ghskburla.sHtML

[S49] C++：写文件
来源：http://blog.vehdjk.com/Article/details/glmepeqie.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.bbcook.cn/Article/details/gbtgrwjuf.sHtML

[S50] C++：格式化数字
来源：http://mobile.fktsv.cn/Article/details/gfgtskgjv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gctkjbhit.sHtML

[S51] C++：显式类型转换
来源：http://baike.yfazqb.com/Article/details/gatjqouqs.sHtML

static_cast<double>(a) / b
来源：http://read.share.vehdjk.com/Article/details/gerklwxpm.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/gjncglmky.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.vehdjk.com/Article/details/gvwufizpj.sHtML

[S53] C++：移动语义
来源：http://blog.yfazqb.com/Article/details/gzsbegpyv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.tarul.cn/Article/details/gksfikekn.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fktsv.cn/Article/details/grkvjlbsy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.tarul.cn/Article/details/gwioeccfr.sHtML

[S55] C++：结构化绑定
来源：http://m.share.epnwcf.com/Article/details/gseeurjqu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/gqwkvzyzr.sHtML

[S56] C++：optional
来源：http://3g.vehdjk.com/Article/details/ggxofewce.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.epnwcf.com/Article/details/gwgkyzhvu.sHtML

[S57] C++：编译期常量
来源：http://baike.yfazqb.com/Article/details/gstnchvfb.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/gecsuqyam.sHtML

[S58] C++：命名空间
来源：http://m.share.tarul.cn/Article/details/gqhkisjac.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.yfazqb.com/Article/details/gdxrjitey.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/gbxtlgjpv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.tarul.cn/Article/details/gqzwgwvhm.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fktsv.cn/Article/details/gcsruyfiy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gbsfmunwd.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gctbqcoev.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/gxawmqsuv.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gzbujsvmv.sHtML

[T01] Kotlin：Hello World
来源：http://3g.vehdjk.com/Article/details/gxsxpakix.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/ghjlvpoul.sHtML

[T02] Kotlin：变量
来源：http://wap.bbcook.cn/Article/details/gnaxtbfrf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.bbcook.cn/Article/details/gvwnvtofl.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.yfazqb.com/Article/details/gikwpwtfq.sHtML

"值: $b"
来源：http://read.share.vehdjk.com/Article/details/ghiviyrcw.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/gokkljeuz.sHtML

val n: String? = null;  n?.length
来源：http://wap.fktsv.cn/Article/details/gxladxuyb.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.epnwcf.com/Article/details/gsbcmulmf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.sjlbkw.cn/Article/details/gvhhhznlx.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.tarul.cn/Article/details/gkhfeilie.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gnkgxkgza.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.vehdjk.com/Article/details/guyqgbyig.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fktsv.cn/Article/details/gmexdoiib.sHtML

[T08] Kotlin：数据类
来源：http://mobile.tarul.cn/Article/details/gmrxokwyb.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fktsv.cn/Article/details/gtydljcpg.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.sjlbkw.cn/Article/details/grfvodpot.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.epnwcf.com/Article/details/gcvrommyq.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.tarul.cn/Article/details/gxcxjcnsr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fktsv.cn/Article/details/gakuxvknd.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/ggdvxloff.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.vehdjk.com/Article/details/gyohsxwlx.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fktsv.cn/Article/details/gaoaxblfp.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.epnwcf.com/Article/details/gpdhlgzdr.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.epnwcf.com/Article/details/gnjbtplty.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.sjlbkw.cn/Article/details/gnfiiixit.sHtML

[T14] Kotlin：循环
来源：http://wap.bbcook.cn/Article/details/gosquudul.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gqiboxudv.sHtML

[T15] Kotlin：接口
来源：http://wap.yfazqb.com/Article/details/gseqkoptb.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.sjlbkw.cn/Article/details/gtebnzush.sHtML

[T16] Swift：Hello World
来源：http://www.share.bbcook.cn/Article/details/ghhctaagd.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gfdrchgez.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fktsv.cn/Article/details/gbrmvogxv.sHtML

var a = 1;  let b = 2
来源：http://www.blog.bbcook.cn/Article/details/gmvhdjyka.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gpjmkbvud.sHtML

"值: \(b)"
来源：http://www.share.tarul.cn/Article/details/ggfqbvjaf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.tarul.cn/Article/details/gmlaqecal.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/gnffhskar.sHtML

[T20] Swift：数组操作
来源：http://wap.yfazqb.com/Article/details/gfdatdnoe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.yfazqb.com/Article/details/gnxewmosw.sHtML

[T21] Swift：遍历
来源：http://wap.vehdjk.com/Article/details/gqgdrrmjf.sHtML

for x in a { print(x) }
来源：http://read.share.vehdjk.com/Article/details/ghoodaplh.sHtML

[T22] Swift：字典
来源：http://wap.yfazqb.com/Article/details/gwtsesola.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/gzvcomsnx.sHtML

[T23] Swift：函数
来源：http://mobile.fktsv.cn/Article/details/gyxlviypy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fktsv.cn/Article/details/ghifheodj.sHtML

[T24] Swift：闭包
来源：http://baike.epnwcf.com/Article/details/guztztxwv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.tarul.cn/Article/details/gyxiesabi.sHtML

[T25] Swift：结构体
来源：http://www.blog.bbcook.cn/Article/details/gmxomdsks.sHtML

struct P { var x: Int }
来源：http://m.share.fktsv.cn/Article/details/gsqoanhft.sHtML

[T26] Swift：类与重写
来源：http://wap.vehdjk.com/Article/details/gjdhytauc.sHtML

class A: Base { override func f() {} }
来源：http://www.share.tarul.cn/Article/details/gzytprirk.sHtML

[T27] Swift：错误处理
来源：http://read.share.bbcook.cn/Article/details/gpalygjqt.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/gffvwiljg.sHtML

[T28] Swift：枚举
来源：http://wap.sjlbkw.cn/Article/details/gkwrleufi.sHtML

enum Color { case red, green }
来源：http://blog.yfazqb.com/Article/details/gohttopxp.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fktsv.cn/Article/details/gfcrofggv.sHtML

guard let x = opt else { return }
来源：http://read.share.vehdjk.com/Article/details/gurgxxhac.sHtML

[T30] Swift：协议
来源：http://3g.sjlbkw.cn/Article/details/gogmkmvwy.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.yfazqb.com/Article/details/gnnizhxgn.sHtML

[T31] Lua：Hello World
来源：http://3g.epnwcf.com/Article/details/gzulpyroa.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/gctygboxc.sHtML

[T32] Lua：局部变量
来源：http://m.share.tarul.cn/Article/details/gycxbxxoh.sHtML

local a = 1
来源：http://www.m.share.vehdjk.com/Article/details/gsyicsyiq.sHtML

[T33] Lua：表（数组）
来源：http://baike.bbcook.cn/Article/details/ghmsvrdys.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.bbcook.cn/Article/details/gzwvrooxw.sHtML

[T34] Lua：遍历表
来源：http://wap.epnwcf.com/Article/details/gsmsnxqcp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/gvgzaxtla.sHtML

[T35] Lua：字典表
来源：http://www.share.yfazqb.com/Article/details/gubyzeyld.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.epnwcf.com/Article/details/gcbwngijh.sHtML

[T36] Lua：函数
来源：http://mobile.fktsv.cn/Article/details/guhjfaila.sHtML

function add(a, b) return a + b end
来源：http://www.blog.vehdjk.com/Article/details/glyguzgtc.sHtML

[T37] Lua：字符串拼接
来源：http://baike.vehdjk.com/Article/details/gmdjkjpig.sHtML

"a" .. "b"
来源：http://www.m.share.tarul.cn/Article/details/gbtgwesdl.sHtML

[T38] Lua：条件
来源：http://mobile.yfazqb.com/Article/details/gftracwls.sHtML

if x > 0 then print("正") end
来源：http://www.share.tarul.cn/Article/details/gluzrsasg.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/gamwidgzg.sHtML

string.find(s, "%d+")
来源：http://www.share.vehdjk.com/Article/details/gqcfplhoq.sHtML

[T40] Lua：元表
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsxprvdm.sHtML

setmetatable({}, { __index = base })
来源：http://wap.tarul.cn/Article/details/gnwyhncjv.sHtML

[T41] Perl：Hello World
来源：http://m.share.fktsv.cn/Article/details/gkyonoxwk.sHtML

print "Hello\n";
来源：http://www.blog.fktsv.cn/Article/details/grtsbxbpb.sHtML

[T42] Perl：变量类型
来源：http://www.share.yfazqb.com/Article/details/gbkfqbggy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fktsv.cn/Article/details/gyjtcilzg.sHtML

[T43] Perl：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gfhimfbtc.sHtML

"值: $a"
来源：http://wap.sjlbkw.cn/Article/details/gsykqkdjt.sHtML

[T44] Perl：条件
来源：http://m.share.fktsv.cn/Article/details/guiqeooem.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.yfazqb.com/Article/details/gewwuagvp.sHtML

[T45] Perl：数组遍历
来源：http://3g.bbcook.cn/Article/details/gcarrlcis.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fktsv.cn/Article/details/ggrhuglla.sHtML

[T46] Perl：哈希操作
来源：http://read.share.vehdjk.com/Article/details/gccltxkoi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.bbcook.cn/Article/details/gvifxdctp.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.sjlbkw.cn/Article/details/gtclicjah.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fktsv.cn/Article/details/grlgyhgpr.sHtML

[T48] Perl：正则替换
来源：http://m.share.vehdjk.com/Article/details/gunakmnid.sHtML

$s =~ s/old/new/g;
来源：http://m.share.vehdjk.com/Article/details/gcopeuxye.sHtML

[T49] Perl：函数
来源：http://blog.fktsv.cn/Article/details/gxhvgptxw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gkyvfjihd.sHtML

[T50] Perl：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gnbnbzdgh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.tarul.cn/Article/details/gohllkyoi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.tarul.cn/Article/details/gpohhaaqa.sHtML

[T51] Scala：Hello World
来源：http://3g.sjlbkw.cn/Article/details/ghkturljk.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/glmcqsxrs.sHtML

[T52] Scala：变量
来源：http://www.m.share.epnwcf.com/Article/details/gftuwplqx.sHtML

val a = 1;  var b = 2
来源：http://mobile.bbcook.cn/Article/details/gwgqiajfd.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gwdahhmey.sHtML

s"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gykwivfki.sHtML

[T54] Scala：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gvxpujwcx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.yfazqb.com/Article/details/gdwonhgvs.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/godtuvnen.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.bbcook.cn/Article/details/gpslopxjh.sHtML

[T56] Scala：样例类
来源：http://m.share.fktsv.cn/Article/details/gzphntntu.sHtML

case class User(name: String, age: Int)
来源：http://read.share.vehdjk.com/Article/details/gwsugzibf.sHtML

[T57] Scala：模式匹配
来源：http://wap.tarul.cn/Article/details/gnvzbebuo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.yfazqb.com/Article/details/gacixwgnz.sHtML

[T58] Scala：函数定义
来源：http://www.blog.bbcook.cn/Article/details/ghphiegiu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.tarul.cn/Article/details/giugymuri.sHtML

[T59] Scala：循环
来源：http://read.share.tarul.cn/Article/details/gzveqtrcb.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fktsv.cn/Article/details/gnotnqpla.sHtML

[T60] Scala：折叠
来源：http://mobile.yfazqb.com/Article/details/gaxnknoje.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.vehdjk.com/Article/details/gqxcymbjt.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gbsvhfauk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/gmyssornd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqjogtejn.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fktsv.cn/Article/details/ghdsqenxp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.sjlbkw.cn/Article/details/gcakrcvsi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.tarul.cn/Article/details/gcaazirku.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.epnwcf.com/Article/details/gpbntspfs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.bbcook.cn/Article/details/ghrubtwuz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.yfazqb.com/Article/details/gzbexsfvp.sHtML

[U04] Py：变量调试打印
来源：http://read.share.vehdjk.com/Article/details/gnofotfzv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.bbcook.cn/Article/details/ggwibqiev.sHtML

[U05] Py：列表去重且保序
来源：http://blog.yfazqb.com/Article/details/gkuffmowd.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/ggyirwrls.sHtML

[U06] Py：合并两个字典
来源：http://blog.tarul.cn/Article/details/ggswyjcch.sHtML

{**a, **b}
来源：http://m.share.epnwcf.com/Article/details/gaofnsqxn.sHtML

[U07] Py：反转字典键值
来源：http://m.share.vehdjk.com/Article/details/gyjmiplks.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.tarul.cn/Article/details/ghavxjuma.sHtML

[U08] Py：展平二维列表
来源：http://3g.tarul.cn/Article/details/geghgzuji.sHtML

[y for x in nested for y in x]
来源：http://3g.vehdjk.com/Article/details/glngihlat.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.yfazqb.com/Article/details/gcugnytxh.sHtML

max(d, key=d.get)
来源：http://baike.sjlbkw.cn/Article/details/ggdteqrqo.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.tarul.cn/Article/details/gpmeftkdq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.yfazqb.com/Article/details/gxcislojm.sHtML

[U11] Py：生成器表达式
来源：http://read.share.yfazqb.com/Article/details/gvluwljwi.sHtML

(x * 2 for x in arr)
来源：http://3g.sjlbkw.cn/Article/details/gizkdvlvl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fktsv.cn/Article/details/ginpjfunc.sHtML

Counter(arr).most_common(3)
来源：http://read.share.sjlbkw.cn/Article/details/gocdnqxvx.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.epnwcf.com/Article/details/gpakjjwoc.sHtML

deque(maxlen=10)
来源：http://read.share.tarul.cn/Article/details/gxomstslu.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fktsv.cn/Article/details/gtozmkqkd.sHtML

defaultdict(list)
来源：http://www.blog.tarul.cn/Article/details/gfzrlablr.sHtML

[U15] Py：高精度计时
来源：http://mobile.epnwcf.com/Article/details/gmghiuliq.sHtML

t = time.perf_counter()
来源：http://m.share.epnwcf.com/Article/details/gscuwkcck.sHtML

[U16] Py：命令行参数解析
来源：http://3g.epnwcf.com/Article/details/gmnlkhmnh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.yfazqb.com/Article/details/grpdvdlsg.sHtML

[U17] Py：初始化日志
来源：http://www.blog.tarul.cn/Article/details/gewsijjmt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.sjlbkw.cn/Article/details/gsjvoqxes.sHtML

[U18] Py：预编译正则
来源：http://3g.epnwcf.com/Article/details/ghrtqvvah.sHtML

pat = re.compile(r"\d+")
来源：http://3g.yfazqb.com/Article/details/gtuchuscc.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.sjlbkw.cn/Article/details/gqgbjuubo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.bbcook.cn/Article/details/glluzfuki.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.vehdjk.com/Article/details/gfvctynee.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.vehdjk.com/Article/details/grghrphuk.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.sjlbkw.cn/Article/details/gwiojrgoy.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/gwdvkmbnl.sHtML

[U22] Py：矩阵转置
来源：http://wap.fktsv.cn/Article/details/gerashqqe.sHtML

list(zip(*m))
来源：http://read.share.tarul.cn/Article/details/gxcblvjgd.sHtML

[U23] Py：分块读取大文件
来源：http://3g.tarul.cn/Article/details/gxfkyrfli.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.sjlbkw.cn/Article/details/gwkuwzjdc.sHtML

[U24] Py：路径操作
来源：http://3g.vehdjk.com/Article/details/gmsprmrqq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/grsdtuaji.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.sjlbkw.cn/Article/details/gvwoganza.sHtML

csv.DictReader(f)
来源：http://3g.bbcook.cn/Article/details/glrchjgtq.sHtML

[U26] Py：并发下载
来源：http://3g.tarul.cn/Article/details/gfjhfwkos.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.tarul.cn/Article/details/gvwrrwaka.sHtML

[U27] Py：异步 HTTP
来源：http://blog.vehdjk.com/Article/details/gmairbycj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.epnwcf.com/Article/details/gapdhcoys.sHtML

[U28] Py：类型别名
来源：http://wap.sjlbkw.cn/Article/details/gccgupqwd.sHtML

UserId = int
来源：http://read.share.yfazqb.com/Article/details/gkhzdmbtu.sHtML

[U29] Py：属性校验
来源：http://mobile.tarul.cn/Article/details/gtjkjeikx.sHtML

@property 与 @x.setter 配合
来源：http://m.share.yfazqb.com/Article/details/gafjdlbnt.sHtML

[U30] Py：数据类
来源：http://wap.bbcook.cn/Article/details/gcfpildly.sHtML

@dataclass(slots=True)
来源：http://blog.epnwcf.com/Article/details/gzxuljnjw.sHtML

[U31] Py：单测
来源：http://3g.bbcook.cn/Article/details/gxobgwjsb.sHtML

python -m pytest -q
来源：http://3g.vehdjk.com/Article/details/gqndqffjr.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.yfazqb.com/Article/details/geugsiwvr.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.yfazqb.com/Article/details/gpnaslmzt.sHtML

[U33] Py：打包发布
来源：http://mobile.sjlbkw.cn/Article/details/gtpctkvth.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.vehdjk.com/Article/details/gdmklmwxp.sHtML

[U34] Py：判断编码
来源：http://mobile.tarul.cn/Article/details/gfiqxvfrv.sHtML

chardet.detect(raw)
来源：http://wap.yfazqb.com/Article/details/gpqbruuvl.sHtML

[U35] Py：发送邮件
来源：http://3g.yfazqb.com/Article/details/gwrgwkkpb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.tarul.cn/Article/details/gyehowgzr.sHtML

[U36] Py：定时任务
来源：http://read.share.vehdjk.com/Article/details/gqyixrtzs.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fktsv.cn/Article/details/galyewuwp.sHtML

[U37] Py：读写 Excel
来源：http://read.share.yfazqb.com/Article/details/guekfggyf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.tarul.cn/Article/details/ginrecyfn.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.epnwcf.com/Article/details/gjjziglrt.sHtML

Path(__file__).resolve().parent
来源：http://www.share.vehdjk.com/Article/details/ginxhcmbp.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.epnwcf.com/Article/details/glvgxviuh.sHtML

sys.stdout.isatty()
来源：http://m.share.tarul.cn/Article/details/gummdblvu.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fktsv.cn/Article/details/gmstzlpux.sHtML

print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/gxnudghym.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.tarul.cn/Article/details/grgjxupub.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.epnwcf.com/Article/details/gbilhxqnh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fktsv.cn/Article/details/ghnzbthxw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fktsv.cn/Article/details/giogenyjf.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.tarul.cn/Article/details/gktdikyya.sHtML

namespace App\Http;
来源：http://blog.yfazqb.com/Article/details/gzusalqmm.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.yfazqb.com/Article/details/gsbmtqoli.sHtML

declare(strict_types=1);
来源：http://www.m.share.bbcook.cn/Article/details/gswoabtyv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.vehdjk.com/Article/details/ghpynfjvn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gozxzfryr.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.yfazqb.com/Article/details/gbzbcnsfm.sHtML

?string $name = null
来源：http://3g.fktsv.cn/Article/details/grvvtcpoh.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.tarul.cn/Article/details/ggbyorqmd.sHtML

int|string $id
来源：http://mobile.bbcook.cn/Article/details/gotypxhmy.sHtML

[U48] PHP：纯枚举
来源：http://www.share.tarul.cn/Article/details/glcninsot.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuqnmjqd.sHtML

[U49] PHP：只读属性
来源：http://www.share.epnwcf.com/Article/details/gxueouuzh.sHtML

public readonly string $name
来源：http://www.share.sjlbkw.cn/Article/details/gscwpydlv.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.sjlbkw.cn/Article/details/gdskeaybb.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fktsv.cn/Article/details/gldkebsex.sHtML

[U51] PHP：数组解构
来源：http://m.share.sjlbkw.cn/Article/details/gkcmhbjsa.sHtML

[$a, $b] = $arr;
来源：http://www.blog.yfazqb.com/Article/details/gvqedccgf.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.epnwcf.com/Article/details/gpzestfwh.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.epnwcf.com/Article/details/gwuvizirp.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.sjlbkw.cn/Article/details/gvkkvggbr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.tarul.cn/Article/details/gockltgsv.sHtML

[U54] PHP：空安全调用
来源：http://3g.yfazqb.com/Article/details/geszmapwy.sHtML

$obj?->method()
来源：http://wap.yfazqb.com/Article/details/gkpthywaf.sHtML


<!-- 参考信息 -->