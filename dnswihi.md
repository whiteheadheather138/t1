代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.sjlbkw.cn/Article/details/graouyvho.sHtML

[S23] C：随机数
来源：http://m.share.sjlbkw.cn/Article/details/gxcxikvov.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.yfazqb.com/Article/details/gswlgutjd.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/gyrxznmnp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.sjlbkw.cn/Article/details/gevodtyvi.sHtML

[S25] C：内存拷贝
来源：http://www.share.vehdjk.com/Article/details/gwfvazzlk.sHtML

memcpy(dst, src, n);
来源：http://blog.epnwcf.com/Article/details/gstqrcyme.sHtML

[S26] C：内存清零
来源：http://m.share.vehdjk.com/Article/details/gdvduhtgd.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gzlcavxhn.sHtML

[S27] C：定义常量
来源：http://mobile.epnwcf.com/Article/details/gutomxbpy.sHtML

const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/ganozkrjh.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/gwwixtvfb.sHtML

static int counter = 0;
来源：http://wap.vehdjk.com/Article/details/gfizmaxmo.sHtML

[S29] C：变参函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwltlsar.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/gqbvabjkg.sHtML

[S30] C：头文件保护
来源：http://www.blog.sjlbkw.cn/Article/details/gqcoogunf.sHtML

#ifndef X_H
来源：http://wap.yfazqb.com/Article/details/gjxttfevz.sHtML

#define X_H
来源：http://baike.bbcook.cn/Article/details/gsdysxcnt.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/gxyustjwe.sHtML

[S31] C++：Hello World
来源：http://baike.epnwcf.com/Article/details/gwitrdfmq.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gggmwhmsk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfsswartp.sHtML

[S32] C++：字符串
来源：http://www.blog.fktsv.cn/Article/details/gkaobmmgg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.sjlbkw.cn/Article/details/gzrbncchz.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/gbieuyfqo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gnyadsrlx.sHtML

[S34] C++：遍历 vector
来源：http://wap.fktsv.cn/Article/details/ghivcfjiq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.epnwcf.com/Article/details/gmdpnbknu.sHtML

[S35] C++：map
来源：http://wap.vehdjk.com/Article/details/gwibmicoq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/geibpfawj.sHtML

[S36] C++：unordered_map
来源：http://mobile.fktsv.cn/Article/details/gmuzgfepf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gfsictows.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/goriypzbi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.yfazqb.com/Article/details/gktafhffm.sHtML

[S38] C++：排序
来源：http://3g.epnwcf.com/Article/details/gbxediinm.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.bbcook.cn/Article/details/grzrbpprs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.vehdjk.com/Article/details/gqzmwzokr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.tarul.cn/Article/details/guwukdouz.sHtML

[S40] C++：查找元素
来源：http://www.blog.epnwcf.com/Article/details/gdvvdjaox.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.vehdjk.com/Article/details/gdktnokzs.sHtML

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/gprshhnrq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.epnwcf.com/Article/details/gsqlohztn.sHtML

[S42] C++：继承与虚函数
来源：http://wap.vehdjk.com/Article/details/gwmowefhb.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.epnwcf.com/Article/details/gsbskwrqy.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/gvhncqxjg.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.tarul.cn/Article/details/gzygscdkf.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/gtzetycyl.sHtML

void inc(int &x) { ++x; }
来源：http://3g.sjlbkw.cn/Article/details/gsmytgmdb.sHtML

[S45] C++：lambda
来源：http://baike.fktsv.cn/Article/details/govsebslf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.sjlbkw.cn/Article/details/glnuneiuz.sHtML

[S46] C++：函数模板
来源：http://baike.vehdjk.com/Article/details/gyrmhrsmj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.vehdjk.com/Article/details/gtqstiqyj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.tarul.cn/Article/details/goommcojc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.vehdjk.com/Article/details/grqtmjxfo.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gckbzaeia.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.epnwcf.com/Article/details/gfonyepxy.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fktsv.cn/Article/details/gyoctkzst.sHtML

[S49] C++：写文件
来源：http://www.blog.fktsv.cn/Article/details/gsnellzdv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.vehdjk.com/Article/details/gvoyopvrz.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/gjccwjqni.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/gxfvgrcrn.sHtML

[S51] C++：显式类型转换
来源：http://wap.yfazqb.com/Article/details/gxmoduois.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/gjdujprxm.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.bbcook.cn/Article/details/ghipnzvbi.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.yfazqb.com/Article/details/gayulllte.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/galkajqzh.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fktsv.cn/Article/details/gcwvetnjb.sHtML

[S54] C++：异常处理
来源：http://m.share.sjlbkw.cn/Article/details/gdjlsinvp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.epnwcf.com/Article/details/gpbemgluu.sHtML

[S55] C++：结构化绑定
来源：http://wap.sjlbkw.cn/Article/details/gctizhacq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.tarul.cn/Article/details/ghvfogfjf.sHtML

[S56] C++：optional
来源：http://blog.tarul.cn/Article/details/gddttbijn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.epnwcf.com/Article/details/giykomyac.sHtML

[S57] C++：编译期常量
来源：http://mobile.fktsv.cn/Article/details/gljkfrwkc.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gbuqkfant.sHtML

[S58] C++：命名空间
来源：http://wap.vehdjk.com/Article/details/gxycmgdqk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.bbcook.cn/Article/details/gymgixymz.sHtML

[S59] C++：静态断言
来源：http://blog.epnwcf.com/Article/details/gwsftxtgv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gjuryfheg.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.bbcook.cn/Article/details/ginzencdi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.bbcook.cn/Article/details/ghwopylzp.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnlzjnvqw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.sjlbkw.cn/Article/details/gxavdiohl.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwzdsxymt.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gtxatnefi.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/gqejroymo.sHtML

[T02] Kotlin：变量
来源：http://wap.tarul.cn/Article/details/gieumgrlq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.tarul.cn/Article/details/gkcmvzyxc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/gbqyjcdpx.sHtML

"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gtlxhmrzi.sHtML

[T04] Kotlin：空安全
来源：http://3g.sjlbkw.cn/Article/details/gducyweha.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fktsv.cn/Article/details/gxzuzhgpe.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.bbcook.cn/Article/details/ggccvnkkd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/gipkrejyf.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/gdjcyhrlh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fktsv.cn/Article/details/gskxhnufm.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.vehdjk.com/Article/details/ghsnmwrud.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fktsv.cn/Article/details/gniyjsiam.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fktsv.cn/Article/details/glkytsnax.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.bbcook.cn/Article/details/ggjemjldf.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/grtbxxnlv.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.yfazqb.com/Article/details/gbuyqvryr.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fktsv.cn/Article/details/gljymasxa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/gtaflalri.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.yfazqb.com/Article/details/godjfwxga.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.sjlbkw.cn/Article/details/gptqdlcrd.sHtML

[T12] Kotlin：解构声明
来源：http://3g.epnwcf.com/Article/details/gvtvoekyf.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gougzinzi.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.tarul.cn/Article/details/gtgdopfcw.sHtML

val m = mapOf("a" to 1)
来源：http://3g.sjlbkw.cn/Article/details/gltzmpyza.sHtML

[T14] Kotlin：循环
来源：http://baike.vehdjk.com/Article/details/ggbsqhuph.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gejvlwscf.sHtML

[T15] Kotlin：接口
来源：http://wap.bbcook.cn/Article/details/grcxokxxg.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.yfazqb.com/Article/details/gqpzxmaao.sHtML

[T16] Swift：Hello World
来源：http://www.share.bbcook.cn/Article/details/goitzilgz.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gafizavpp.sHtML

[T17] Swift：变量与常量
来源：http://3g.tarul.cn/Article/details/gikhdhybh.sHtML

var a = 1;  let b = 2
来源：http://mobile.bbcook.cn/Article/details/gnvqyocjj.sHtML

[T18] Swift：字符串插值
来源：http://wap.bbcook.cn/Article/details/gtbinuixy.sHtML

"值: \(b)"
来源：http://baike.epnwcf.com/Article/details/gjxmiobvo.sHtML

[T19] Swift：可选绑定
来源：http://read.share.vehdjk.com/Article/details/gbtiwnekv.sHtML

if let n = opt { print(n) }
来源：http://wap.fktsv.cn/Article/details/gknzmrzmi.sHtML

[T20] Swift：数组操作
来源：http://baike.tarul.cn/Article/details/gvzusakit.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.yfazqb.com/Article/details/gdpwotctu.sHtML

[T21] Swift：遍历
来源：http://m.share.bbcook.cn/Article/details/ghoiqekjq.sHtML

for x in a { print(x) }
来源：http://blog.yfazqb.com/Article/details/gwdsrzqkp.sHtML

[T22] Swift：字典
来源：http://blog.vehdjk.com/Article/details/glaglzfaf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fktsv.cn/Article/details/gqcaqyanq.sHtML

[T23] Swift：函数
来源：http://www.blog.bbcook.cn/Article/details/gavajcnpe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.vehdjk.com/Article/details/gzuwwigkn.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/gfsddyaok.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.tarul.cn/Article/details/ggkqoerby.sHtML

[T25] Swift：结构体
来源：http://read.share.epnwcf.com/Article/details/gdljwyzyx.sHtML

struct P { var x: Int }
来源：http://wap.sjlbkw.cn/Article/details/ghvtczzdv.sHtML

[T26] Swift：类与重写
来源：http://read.share.vehdjk.com/Article/details/gzkbapwoa.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.vehdjk.com/Article/details/girablyve.sHtML

[T27] Swift：错误处理
来源：http://www.blog.vehdjk.com/Article/details/gbyazmfkz.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fktsv.cn/Article/details/gvwgmgbxc.sHtML

[T28] Swift：枚举
来源：http://mobile.vehdjk.com/Article/details/gsdxftyvu.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/gpwvhedgf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.tarul.cn/Article/details/gilsobtbo.sHtML

guard let x = opt else { return }
来源：http://www.m.share.epnwcf.com/Article/details/gxjwdhscm.sHtML

[T30] Swift：协议
来源：http://blog.tarul.cn/Article/details/grlxqhyfo.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.bbcook.cn/Article/details/gwsgdohlz.sHtML

[T31] Lua：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gqznvpdbw.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gerkagjbk.sHtML

[T32] Lua：局部变量
来源：http://wap.vehdjk.com/Article/details/gdumlwrvb.sHtML

local a = 1
来源：http://blog.sjlbkw.cn/Article/details/gszijxquy.sHtML

[T33] Lua：表（数组）
来源：http://baike.epnwcf.com/Article/details/grtsmlzho.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.yfazqb.com/Article/details/gpgzbjydj.sHtML

[T34] Lua：遍历表
来源：http://www.share.tarul.cn/Article/details/gsrgoyotx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.vehdjk.com/Article/details/gmlvppwcq.sHtML

[T35] Lua：字典表
来源：http://wap.epnwcf.com/Article/details/gfofjbfhx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fktsv.cn/Article/details/godgdixsy.sHtML

[T36] Lua：函数
来源：http://read.share.yfazqb.com/Article/details/gqayacqpq.sHtML

function add(a, b) return a + b end
来源：http://wap.fktsv.cn/Article/details/gwrqtpnub.sHtML

[T37] Lua：字符串拼接
来源：http://baike.bbcook.cn/Article/details/gfcxrvepd.sHtML

"a" .. "b"
来源：http://baike.vehdjk.com/Article/details/gvxwsochr.sHtML

[T38] Lua：条件
来源：http://3g.vehdjk.com/Article/details/gqohzbbrl.sHtML

if x > 0 then print("正") end
来源：http://baike.vehdjk.com/Article/details/gmzqzqmwm.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fktsv.cn/Article/details/gauekegxl.sHtML

string.find(s, "%d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gwulopinq.sHtML

[T40] Lua：元表
来源：http://3g.yfazqb.com/Article/details/gjevvpgza.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.epnwcf.com/Article/details/ggiarnkha.sHtML

[T41] Perl：Hello World
来源：http://mobile.yfazqb.com/Article/details/gkrsveuji.sHtML

print "Hello\n";
来源：http://baike.vehdjk.com/Article/details/gaxnqttdz.sHtML

[T42] Perl：变量类型
来源：http://mobile.epnwcf.com/Article/details/giwxwcmau.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.bbcook.cn/Article/details/gvawsalkg.sHtML

[T43] Perl：字符串插值
来源：http://blog.vehdjk.com/Article/details/gnlbybfju.sHtML

"值: $a"
来源：http://m.share.bbcook.cn/Article/details/garvpjkuu.sHtML

[T44] Perl：条件
来源：http://read.share.bbcook.cn/Article/details/gadhxoitm.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.yfazqb.com/Article/details/gwdmostrv.sHtML

[T45] Perl：数组遍历
来源：http://www.share.sjlbkw.cn/Article/details/ginmizgnn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.vehdjk.com/Article/details/gizhbszud.sHtML

[T46] Perl：哈希操作
来源：http://mobile.vehdjk.com/Article/details/gbtxmymur.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.tarul.cn/Article/details/gbvptupis.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.epnwcf.com/Article/details/gaonawoxy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.yfazqb.com/Article/details/ghplpdieg.sHtML

[T48] Perl：正则替换
来源：http://m.share.bbcook.cn/Article/details/gtkkpujse.sHtML

$s =~ s/old/new/g;
来源：http://wap.sjlbkw.cn/Article/details/gowyqeesd.sHtML

[T49] Perl：函数
来源：http://wap.bbcook.cn/Article/details/ggepcbcwd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gtrdvkbiy.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fktsv.cn/Article/details/goukofdcj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.vehdjk.com/Article/details/gdxuangep.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.bbcook.cn/Article/details/gqrxixlbj.sHtML

[T51] Scala：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gqkbmfzds.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gjsluhfjz.sHtML

[T52] Scala：变量
来源：http://baike.sjlbkw.cn/Article/details/gfcuziadn.sHtML

val a = 1;  var b = 2
来源：http://baike.fktsv.cn/Article/details/gqmhfaryy.sHtML

[T53] Scala：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gzomkoefs.sHtML

s"值: $b"
来源：http://baike.yfazqb.com/Article/details/gjdakznkr.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/gnqbpchlq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.sjlbkw.cn/Article/details/gsenkbbni.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fktsv.cn/Article/details/gqljjplek.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.epnwcf.com/Article/details/guwzctomg.sHtML

[T56] Scala：样例类
来源：http://blog.yfazqb.com/Article/details/gyjvmetey.sHtML

case class User(name: String, age: Int)
来源：http://m.share.bbcook.cn/Article/details/gnohvxdxu.sHtML

[T57] Scala：模式匹配
来源：http://m.share.vehdjk.com/Article/details/gpzhvyjxm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/gkgxywyou.sHtML

[T58] Scala：函数定义
来源：http://read.share.epnwcf.com/Article/details/gogsmlzyb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.epnwcf.com/Article/details/gjjijuswh.sHtML

[T59] Scala：循环
来源：http://mobile.sjlbkw.cn/Article/details/gkzhwflln.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.yfazqb.com/Article/details/ggctndxhk.sHtML

[T60] Scala：折叠
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvdkwpdx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.yfazqb.com/Article/details/grptbifob.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtxzjkevq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhmqymvk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmzezhyyp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.tarul.cn/Article/details/goihdjlrz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.tarul.cn/Article/details/gvbsxqoyj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.vehdjk.com/Article/details/gnrhrvoxi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fktsv.cn/Article/details/gyqwfrdik.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.bbcook.cn/Article/details/gnfhyrkgs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.yfazqb.com/Article/details/gnzdawbul.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.bbcook.cn/Article/details/gwpmnkmbb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.epnwcf.com/Article/details/gvhkffxsi.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.yfazqb.com/Article/details/gslwpfrpd.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.epnwcf.com/Article/details/gawaerebg.sHtML

[U06] Py：合并两个字典
来源：http://www.share.bbcook.cn/Article/details/gqnkhhorz.sHtML

{**a, **b}
来源：http://www.blog.tarul.cn/Article/details/gullypzgw.sHtML

[U07] Py：反转字典键值
来源：http://m.share.vehdjk.com/Article/details/gusycgbbd.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fktsv.cn/Article/details/ghqicaagz.sHtML

[U08] Py：展平二维列表
来源：http://wap.vehdjk.com/Article/details/guwkyntfk.sHtML

[y for x in nested for y in x]
来源：http://read.share.sjlbkw.cn/Article/details/gnhrhfrjw.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.yfazqb.com/Article/details/gasweuinp.sHtML

max(d, key=d.get)
来源：http://m.share.yfazqb.com/Article/details/gzqmovimy.sHtML

[U10] Py：按值排序字典
来源：http://baike.sjlbkw.cn/Article/details/gcbhoizan.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.epnwcf.com/Article/details/gshlwepcb.sHtML

[U11] Py：生成器表达式
来源：http://baike.epnwcf.com/Article/details/grmzaaxlx.sHtML

(x * 2 for x in arr)
来源：http://www.blog.tarul.cn/Article/details/ggqhqlezf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.bbcook.cn/Article/details/gfnnsbxlo.sHtML

Counter(arr).most_common(3)
来源：http://m.share.epnwcf.com/Article/details/gzpqohrut.sHtML

[U13] Py：固定长度队列
来源：http://m.share.sjlbkw.cn/Article/details/gboqoftfr.sHtML

deque(maxlen=10)
来源：http://wap.yfazqb.com/Article/details/gkkgieikr.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.epnwcf.com/Article/details/gfiygytow.sHtML

defaultdict(list)
来源：http://www.share.bbcook.cn/Article/details/gwiuggbha.sHtML

[U15] Py：高精度计时
来源：http://read.share.epnwcf.com/Article/details/gslhkpgmy.sHtML

t = time.perf_counter()
来源：http://blog.vehdjk.com/Article/details/gwcfsqhpk.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fktsv.cn/Article/details/gatyzxjrr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.bbcook.cn/Article/details/gyeneuore.sHtML

[U17] Py：初始化日志
来源：http://3g.vehdjk.com/Article/details/gusajvohd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.epnwcf.com/Article/details/gogfljeun.sHtML

[U18] Py：预编译正则
来源：http://mobile.yfazqb.com/Article/details/gajcjrqem.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfrauggn.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.epnwcf.com/Article/details/giysaqjph.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.yfazqb.com/Article/details/gflbjqeok.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.sjlbkw.cn/Article/details/grgefklpd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.yfazqb.com/Article/details/gykptkshc.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.bbcook.cn/Article/details/gduvyjuxf.sHtML

@contextlib.contextmanager
来源：http://blog.yfazqb.com/Article/details/gryxwlepc.sHtML

[U22] Py：矩阵转置
来源：http://3g.bbcook.cn/Article/details/gawlzkutp.sHtML

list(zip(*m))
来源：http://wap.yfazqb.com/Article/details/gqscrwkfz.sHtML

[U23] Py：分块读取大文件
来源：http://3g.sjlbkw.cn/Article/details/gtltkojav.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.sjlbkw.cn/Article/details/gdjvpxznp.sHtML

[U24] Py：路径操作
来源：http://www.share.sjlbkw.cn/Article/details/gefaydojj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gfkrkdmas.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fktsv.cn/Article/details/gegjxmiiy.sHtML

csv.DictReader(f)
来源：http://3g.sjlbkw.cn/Article/details/gazwmaulz.sHtML

[U26] Py：并发下载
来源：http://wap.fktsv.cn/Article/details/ghjzvsdns.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.vehdjk.com/Article/details/gaalclgjd.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.tarul.cn/Article/details/gkbwmrfvs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.yfazqb.com/Article/details/gouufwvmr.sHtML

[U28] Py：类型别名
来源：http://m.share.bbcook.cn/Article/details/ggbugegal.sHtML

UserId = int
来源：http://m.share.sjlbkw.cn/Article/details/golgyyiab.sHtML

[U29] Py：属性校验
来源：http://3g.bbcook.cn/Article/details/ghubhunbf.sHtML

@property 与 @x.setter 配合
来源：http://wap.vehdjk.com/Article/details/gsctqqpzc.sHtML

[U30] Py：数据类
来源：http://www.blog.fktsv.cn/Article/details/gegmifogu.sHtML

@dataclass(slots=True)
来源：http://baike.yfazqb.com/Article/details/gimhfsuuo.sHtML

[U31] Py：单测
来源：http://baike.yfazqb.com/Article/details/gfobosfwi.sHtML

python -m pytest -q
来源：http://www.share.vehdjk.com/Article/details/gyjdvpsko.sHtML

[U32] Py：代码格式化
来源：http://mobile.epnwcf.com/Article/details/garsitipa.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fktsv.cn/Article/details/gdaycgnqd.sHtML

[U33] Py：打包发布
来源：http://blog.vehdjk.com/Article/details/gkpjbncwm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.bbcook.cn/Article/details/gdoumosuy.sHtML

[U34] Py：判断编码
来源：http://www.m.share.tarul.cn/Article/details/gwtpzpceq.sHtML

chardet.detect(raw)
来源：http://www.m.share.tarul.cn/Article/details/gkqclybng.sHtML

[U35] Py：发送邮件
来源：http://read.share.bbcook.cn/Article/details/gahzxwslz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fktsv.cn/Article/details/gpirffvpk.sHtML

[U36] Py：定时任务
来源：http://www.share.yfazqb.com/Article/details/gjrdhyrpx.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.bbcook.cn/Article/details/gsjwskzsv.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.yfazqb.com/Article/details/grhcvbszy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.yfazqb.com/Article/details/glsyxnwzm.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fktsv.cn/Article/details/gvpkqotrk.sHtML

Path(__file__).resolve().parent
来源：http://mobile.tarul.cn/Article/details/gkuamhksh.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.yfazqb.com/Article/details/ghpdibwqz.sHtML

sys.stdout.isatty()
来源：http://wap.vehdjk.com/Article/details/gykcsdpvq.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.vehdjk.com/Article/details/golnyyhcj.sHtML

print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gjkxcauag.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.epnwcf.com/Article/details/gftwjhihr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.bbcook.cn/Article/details/geqhkrxfb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.vehdjk.com/Article/details/gswwtpiyh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.bbcook.cn/Article/details/gyfcvznjf.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.tarul.cn/Article/details/gigbnfegj.sHtML

namespace App\Http;
来源：http://m.share.fktsv.cn/Article/details/gtqeklrrd.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fktsv.cn/Article/details/gizpbimyh.sHtML

declare(strict_types=1);
来源：http://www.blog.vehdjk.com/Article/details/grmngmzhk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.bbcook.cn/Article/details/gmqoqhesy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/ghengprhw.sHtML

[U46] PHP：可空类型
来源：http://www.blog.epnwcf.com/Article/details/gnyduxuuw.sHtML

?string $name = null
来源：http://www.share.epnwcf.com/Article/details/glvigwmbu.sHtML


<!-- 参考信息 -->