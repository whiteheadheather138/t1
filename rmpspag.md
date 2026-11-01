代发 wailian999

#include <iostream>
来源：http://3g.bbcook.cn/Article/details/gvjkolswj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.tarul.cn/Article/details/gsmqvlxqo.sHtML

[S32] C++：字符串
来源：http://www.blog.yfazqb.com/Article/details/ggwxctvng.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fktsv.cn/Article/details/gaeswjdbg.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.vehdjk.com/Article/details/gfihsqxfa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gfutlmpbh.sHtML

[S34] C++：遍历 vector
来源：http://read.share.yfazqb.com/Article/details/gheuqnozm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.yfazqb.com/Article/details/gcmwtjpra.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/gcmgxgyin.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gzljywama.sHtML

[S36] C++：unordered_map
来源：http://www.blog.tarul.cn/Article/details/groyvscir.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gvodwuuuz.sHtML

[S37] C++：set
来源：http://m.share.fktsv.cn/Article/details/garkyffme.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.sjlbkw.cn/Article/details/gqcsdovfr.sHtML

[S38] C++：排序
来源：http://www.blog.sjlbkw.cn/Article/details/gaddeaclk.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.tarul.cn/Article/details/gegwjwpsn.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/gwbggaimx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.sjlbkw.cn/Article/details/gdwpcyukm.sHtML

[S40] C++：查找元素
来源：http://m.share.vehdjk.com/Article/details/gcrczzeup.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fktsv.cn/Article/details/gvyvwqezo.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.tarul.cn/Article/details/gdcmzfejm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/gcuofhfhm.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gybgdxeqb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.yfazqb.com/Article/details/gyubhwprh.sHtML

[S43] C++：智能指针
来源：http://baike.epnwcf.com/Article/details/goieejygi.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/gvnjkhpcq.sHtML

[S44] C++：引用传参
来源：http://m.share.bbcook.cn/Article/details/gceizhhra.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gedlmizpi.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/gurwurykw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.vehdjk.com/Article/details/guzqnkbjx.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/gvtuqidzm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fktsv.cn/Article/details/gghypmaqi.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.tarul.cn/Article/details/gowmsvyhg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.bbcook.cn/Article/details/gijciiyvt.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gobteiaxd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/gmbcilhuo.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.tarul.cn/Article/details/gelglcweh.sHtML

[S49] C++：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gewzwrlhv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/gzupdodae.sHtML

[S50] C++：格式化数字
来源：http://www.blog.sjlbkw.cn/Article/details/gcbtpsydj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.epnwcf.com/Article/details/glzbycytb.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fktsv.cn/Article/details/gpscljkta.sHtML

static_cast<double>(a) / b
来源：http://www.share.fktsv.cn/Article/details/gbdcznozp.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.bbcook.cn/Article/details/gdbnrjpyi.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.bbcook.cn/Article/details/gcoipjfod.sHtML

[S53] C++：移动语义
来源：http://3g.yfazqb.com/Article/details/gviqfhdmb.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.epnwcf.com/Article/details/gxyafkftb.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gindiuepv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.yfazqb.com/Article/details/gukxcizut.sHtML

[S55] C++：结构化绑定
来源：http://www.share.sjlbkw.cn/Article/details/gkdapxspe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.bbcook.cn/Article/details/gnbasycpw.sHtML

[S56] C++：optional
来源：http://read.share.vehdjk.com/Article/details/gkloqofzy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/grackfywr.sHtML

[S57] C++：编译期常量
来源：http://m.share.tarul.cn/Article/details/gsainnyln.sHtML

constexpr int N = 10;
来源：http://3g.bbcook.cn/Article/details/grhnwqzbg.sHtML

[S58] C++：命名空间
来源：http://read.share.yfazqb.com/Article/details/ghlsfckls.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.bbcook.cn/Article/details/gaemtcpav.sHtML

[S59] C++：静态断言
来源：http://www.share.fktsv.cn/Article/details/gjbkvcwju.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.vehdjk.com/Article/details/gxijjpipx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/garoantau.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.sjlbkw.cn/Article/details/ggvgyzrzw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grdmyujwj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/gmtbknuhn.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghrzxbhdc.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/grchrdcbz.sHtML

println("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gactivmmw.sHtML

[T02] Kotlin：变量
来源：http://3g.vehdjk.com/Article/details/gxaowksvq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.sjlbkw.cn/Article/details/gtsbjlffm.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.bbcook.cn/Article/details/gszbtuipo.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/gzwmxyflx.sHtML

[T04] Kotlin：空安全
来源：http://wap.vehdjk.com/Article/details/gcyaclhea.sHtML

val n: String? = null;  n?.length
来源：http://read.share.tarul.cn/Article/details/gfpbncklf.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.tarul.cn/Article/details/ggwsddgcu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gpzozprxk.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/grlwglayv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.vehdjk.com/Article/details/gltfkwaef.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.tarul.cn/Article/details/gbqbpjdhf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gitfnwsfq.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/gukyedruh.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fktsv.cn/Article/details/gajyetynp.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.epnwcf.com/Article/details/gldvuwdev.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.tarul.cn/Article/details/gzxdilsoa.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gbzrmcnbw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.epnwcf.com/Article/details/ghlseglfi.sHtML

[T11] Kotlin：协程
来源：http://www.blog.vehdjk.com/Article/details/gwlpbozsn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/gxtbdgoan.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/gkocmjegx.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/gwuikmmeg.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.bbcook.cn/Article/details/gnciqwezq.sHtML

val m = mapOf("a" to 1)
来源：http://3g.epnwcf.com/Article/details/gjelgfuxa.sHtML

[T14] Kotlin：循环
来源：http://www.share.fktsv.cn/Article/details/gyxnvznqj.sHtML

for (i in 1..10) println(i)
来源：http://www.share.tarul.cn/Article/details/gnnnfmhza.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/gkbxlxghr.sHtML

interface Shape { fun area(): Double }
来源：http://blog.bbcook.cn/Article/details/gvwshrcyb.sHtML

[T16] Swift：Hello World
来源：http://read.share.bbcook.cn/Article/details/gvnkxetlu.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gewjeblku.sHtML

[T17] Swift：变量与常量
来源：http://wap.vehdjk.com/Article/details/gnfwblucg.sHtML

var a = 1;  let b = 2
来源：http://3g.yfazqb.com/Article/details/glgnbypnj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gysxtshga.sHtML

"值: \(b)"
来源：http://read.share.bbcook.cn/Article/details/goslvmmip.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/ggakdhbej.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/gyrepeyjr.sHtML

[T20] Swift：数组操作
来源：http://wap.yfazqb.com/Article/details/gmrawoens.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.epnwcf.com/Article/details/gcvegptss.sHtML

[T21] Swift：遍历
来源：http://mobile.sjlbkw.cn/Article/details/guqpmrrlc.sHtML

for x in a { print(x) }
来源：http://baike.tarul.cn/Article/details/gogetbmwb.sHtML

[T22] Swift：字典
来源：http://www.m.share.yfazqb.com/Article/details/gepeomzvs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.tarul.cn/Article/details/gpjlfffhr.sHtML

[T23] Swift：函数
来源：http://www.blog.yfazqb.com/Article/details/gtvlbopxi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.yfazqb.com/Article/details/gekiayekl.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gmekchzxb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gjgpbitdl.sHtML

[T25] Swift：结构体
来源：http://mobile.sjlbkw.cn/Article/details/gtvqvcvsk.sHtML

struct P { var x: Int }
来源：http://mobile.sjlbkw.cn/Article/details/guxjswrzo.sHtML

[T26] Swift：类与重写
来源：http://mobile.epnwcf.com/Article/details/ggbznmatk.sHtML

class A: Base { override func f() {} }
来源：http://baike.sjlbkw.cn/Article/details/gtbwdqjxb.sHtML

[T27] Swift：错误处理
来源：http://blog.tarul.cn/Article/details/gkewpnkea.sHtML

do { try f() } catch { print(error) }
来源：http://blog.vehdjk.com/Article/details/gfkfzlmfa.sHtML

[T28] Swift：枚举
来源：http://mobile.vehdjk.com/Article/details/ghgqovbws.sHtML

enum Color { case red, green }
来源：http://www.blog.bbcook.cn/Article/details/gpfbixcuc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.bbcook.cn/Article/details/gqybrlqjd.sHtML

guard let x = opt else { return }
来源：http://3g.epnwcf.com/Article/details/gxbakczfg.sHtML

[T30] Swift：协议
来源：http://m.share.epnwcf.com/Article/details/grrddyzgy.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.tarul.cn/Article/details/gkqfbpfsk.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/ggvfgwdah.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gqaufikgi.sHtML

[T32] Lua：局部变量
来源：http://www.share.vehdjk.com/Article/details/ghwoocvtv.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/ghwptomih.sHtML

[T33] Lua：表（数组）
来源：http://3g.epnwcf.com/Article/details/gswkvbvwy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.bbcook.cn/Article/details/gcxcsatsq.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.yfazqb.com/Article/details/gbhtmezfi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/guamoffuz.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fktsv.cn/Article/details/gkcbsohrl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.bbcook.cn/Article/details/gitvzdviz.sHtML

[T36] Lua：函数
来源：http://mobile.epnwcf.com/Article/details/gegdgizoa.sHtML

function add(a, b) return a + b end
来源：http://www.blog.bbcook.cn/Article/details/gejlilhjd.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gdxfjxuuu.sHtML

"a" .. "b"
来源：http://wap.bbcook.cn/Article/details/gvkyzbseb.sHtML

[T38] Lua：条件
来源：http://baike.bbcook.cn/Article/details/gumuldbli.sHtML

if x > 0 then print("正") end
来源：http://www.blog.sjlbkw.cn/Article/details/gjnszmzyb.sHtML

[T39] Lua：模式匹配
来源：http://wap.epnwcf.com/Article/details/ghnzwwdzn.sHtML

string.find(s, "%d+")
来源：http://wap.sjlbkw.cn/Article/details/gsuzzlbok.sHtML

[T40] Lua：元表
来源：http://www.blog.yfazqb.com/Article/details/gltyiphez.sHtML

setmetatable({}, { __index = base })
来源：http://3g.vehdjk.com/Article/details/gumenmcsj.sHtML

[T41] Perl：Hello World
来源：http://read.share.yfazqb.com/Article/details/gcsnhlcfz.sHtML

print "Hello\n";
来源：http://read.share.yfazqb.com/Article/details/gizxrxugi.sHtML

[T42] Perl：变量类型
来源：http://wap.bbcook.cn/Article/details/gnzrrmyfd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.epnwcf.com/Article/details/gassdrtxg.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gjdsrtyaq.sHtML

"值: $a"
来源：http://wap.bbcook.cn/Article/details/gjwlwcfdw.sHtML

[T44] Perl：条件
来源：http://3g.yfazqb.com/Article/details/gmvrinfcr.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.epnwcf.com/Article/details/ghdbbhgqc.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fktsv.cn/Article/details/gfbhideck.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fktsv.cn/Article/details/galypgitp.sHtML

[T46] Perl：哈希操作
来源：http://www.share.epnwcf.com/Article/details/gvymowmrx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.epnwcf.com/Article/details/gaayizdrf.sHtML

[T47] Perl：正则捕获
来源：http://m.share.tarul.cn/Article/details/grjalvyiv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.bbcook.cn/Article/details/gajgtmfkq.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.yfazqb.com/Article/details/glfidcdcu.sHtML

$s =~ s/old/new/g;
来源：http://mobile.epnwcf.com/Article/details/govuknrgo.sHtML

[T49] Perl：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzgcrmav.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkeaavjzm.sHtML

[T50] Perl：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gsoiijrnt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fktsv.cn/Article/details/gofpxaxip.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fktsv.cn/Article/details/gvppfpsge.sHtML

[T51] Scala：Hello World
来源：http://mobile.fktsv.cn/Article/details/gtxpxmpwj.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/glhsykazs.sHtML

[T52] Scala：变量
来源：http://blog.fktsv.cn/Article/details/ggzzebhuu.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.epnwcf.com/Article/details/ghaiwxxma.sHtML

[T53] Scala：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/godezvfze.sHtML

s"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gxuigmtjd.sHtML

[T54] Scala：集合映射
来源：http://read.share.bbcook.cn/Article/details/gjdtcizqs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.epnwcf.com/Article/details/gddogbpdy.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gqbkegonb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/guafujszx.sHtML

[T56] Scala：样例类
来源：http://m.share.tarul.cn/Article/details/gdvkgoyvh.sHtML

case class User(name: String, age: Int)
来源：http://baike.tarul.cn/Article/details/gzomfmwzx.sHtML

[T57] Scala：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gzgvxmhbz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.tarul.cn/Article/details/ggvbzugim.sHtML

[T58] Scala：函数定义
来源：http://mobile.yfazqb.com/Article/details/gzcbfzvfy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.tarul.cn/Article/details/gqgbxmhrn.sHtML

[T59] Scala：循环
来源：http://www.m.share.bbcook.cn/Article/details/grfxskwgj.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.bbcook.cn/Article/details/gwmkthrhi.sHtML

[T60] Scala：折叠
来源：http://wap.bbcook.cn/Article/details/goufrrbjx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/gnwxbqbek.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ggxneijtq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.bbcook.cn/Article/details/gusyjvauu.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gykawlluw.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.bbcook.cn/Article/details/gpfhldbvv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gneogirsi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.sjlbkw.cn/Article/details/giexcittw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.tarul.cn/Article/details/gbexpgizd.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.vehdjk.com/Article/details/goupyddru.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.vehdjk.com/Article/details/gashubygo.sHtML

[U04] Py：变量调试打印
来源：http://read.share.tarul.cn/Article/details/gjgghydvh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.yfazqb.com/Article/details/gmluvhhtz.sHtML

[U05] Py：列表去重且保序
来源：http://baike.epnwcf.com/Article/details/gafjndgvg.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/guvjgvete.sHtML

[U06] Py：合并两个字典
来源：http://read.share.bbcook.cn/Article/details/guvvrrzvm.sHtML

{**a, **b}
来源：http://mobile.tarul.cn/Article/details/gpazoflrr.sHtML

[U07] Py：反转字典键值
来源：http://www.share.tarul.cn/Article/details/gcxzdtapm.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fktsv.cn/Article/details/gnmebzkbq.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gjkyyaaom.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.vehdjk.com/Article/details/gleyfyynd.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.tarul.cn/Article/details/ggttszujz.sHtML

max(d, key=d.get)
来源：http://m.share.yfazqb.com/Article/details/gcyztqcyv.sHtML

[U10] Py：按值排序字典
来源：http://mobile.yfazqb.com/Article/details/gmsdcpvof.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.vehdjk.com/Article/details/guhnrghyw.sHtML

[U11] Py：生成器表达式
来源：http://baike.sjlbkw.cn/Article/details/gmafdwwvt.sHtML

(x * 2 for x in arr)
来源：http://mobile.fktsv.cn/Article/details/gfeyvwjge.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.tarul.cn/Article/details/gpkzlfeub.sHtML

Counter(arr).most_common(3)
来源：http://mobile.yfazqb.com/Article/details/gazgsutdu.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fktsv.cn/Article/details/guzzhgfii.sHtML

deque(maxlen=10)
来源：http://m.share.sjlbkw.cn/Article/details/gcxvafxik.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fktsv.cn/Article/details/gcvzaizgf.sHtML

defaultdict(list)
来源：http://mobile.vehdjk.com/Article/details/gticlgbrv.sHtML

[U15] Py：高精度计时
来源：http://blog.fktsv.cn/Article/details/gvtvalvus.sHtML

t = time.perf_counter()
来源：http://www.share.bbcook.cn/Article/details/gqeukrjqu.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.vehdjk.com/Article/details/galwgztod.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.epnwcf.com/Article/details/goutieunb.sHtML

[U17] Py：初始化日志
来源：http://wap.tarul.cn/Article/details/gjrsqosbf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.yfazqb.com/Article/details/gkojqgqqk.sHtML

[U18] Py：预编译正则
来源：http://3g.bbcook.cn/Article/details/gfrcjowqy.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fktsv.cn/Article/details/gsamzkcuh.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.sjlbkw.cn/Article/details/gqmgurgcs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.bbcook.cn/Article/details/gzmxygrlq.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.epnwcf.com/Article/details/gotgwymmn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.vehdjk.com/Article/details/gjgzazuer.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.bbcook.cn/Article/details/gkvqpmuky.sHtML

@contextlib.contextmanager
来源：http://baike.fktsv.cn/Article/details/grgqatxfl.sHtML

[U22] Py：矩阵转置
来源：http://m.share.vehdjk.com/Article/details/gaqfrfydd.sHtML

list(zip(*m))
来源：http://blog.fktsv.cn/Article/details/gwwpcbfie.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.bbcook.cn/Article/details/gbvllfqtf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.sjlbkw.cn/Article/details/gaolaflux.sHtML

[U24] Py：路径操作
来源：http://read.share.bbcook.cn/Article/details/gkcqqrbot.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gpkvyzwul.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.sjlbkw.cn/Article/details/gdipsddai.sHtML

csv.DictReader(f)
来源：http://baike.bbcook.cn/Article/details/gtbvajpwm.sHtML

[U26] Py：并发下载
来源：http://www.blog.sjlbkw.cn/Article/details/gticloalz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.yfazqb.com/Article/details/gucruleuv.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.bbcook.cn/Article/details/gvytsnyne.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.tarul.cn/Article/details/gcehbnkvy.sHtML

[U28] Py：类型别名
来源：http://www.share.tarul.cn/Article/details/gtmwnqtrt.sHtML

UserId = int
来源：http://www.blog.fktsv.cn/Article/details/gmoekkiyo.sHtML

[U29] Py：属性校验
来源：http://mobile.bbcook.cn/Article/details/ggnvbtrne.sHtML

@property 与 @x.setter 配合
来源：http://mobile.epnwcf.com/Article/details/gmjtmbzdm.sHtML

[U30] Py：数据类
来源：http://3g.tarul.cn/Article/details/gdimqjmfh.sHtML

@dataclass(slots=True)
来源：http://baike.yfazqb.com/Article/details/ghohvchbs.sHtML

[U31] Py：单测
来源：http://3g.yfazqb.com/Article/details/gagnctrzu.sHtML

python -m pytest -q
来源：http://www.m.share.epnwcf.com/Article/details/ghhhemqff.sHtML

[U32] Py：代码格式化
来源：http://mobile.fktsv.cn/Article/details/ggjmzfkuz.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.sjlbkw.cn/Article/details/gyixrwxas.sHtML

[U33] Py：打包发布
来源：http://mobile.epnwcf.com/Article/details/gjkafjney.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.epnwcf.com/Article/details/gewrrsysr.sHtML

[U34] Py：判断编码
来源：http://www.m.share.yfazqb.com/Article/details/gokrzdbgj.sHtML

chardet.detect(raw)
来源：http://wap.yfazqb.com/Article/details/giblbgeuk.sHtML

[U35] Py：发送邮件
来源：http://3g.bbcook.cn/Article/details/gltbdlbsv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.sjlbkw.cn/Article/details/geqtwdekg.sHtML

[U36] Py：定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/ggtphdril.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.yfazqb.com/Article/details/gkbbpuemr.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.bbcook.cn/Article/details/gmvbrtbtl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.vehdjk.com/Article/details/gskrmkfnq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.yfazqb.com/Article/details/gahxyqlri.sHtML

Path(__file__).resolve().parent
来源：http://baike.tarul.cn/Article/details/grcoeqkvc.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.yfazqb.com/Article/details/gfidmqslo.sHtML

sys.stdout.isatty()
来源：http://wap.epnwcf.com/Article/details/gpfzjizxn.sHtML

[U40] Py：打印到标准错误
来源：http://blog.epnwcf.com/Article/details/gfwunpbmt.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnepoijux.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.yfazqb.com/Article/details/gxglcewva.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.tarul.cn/Article/details/gqzekymii.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.epnwcf.com/Article/details/guxxetsqa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.epnwcf.com/Article/details/gpyduxnwu.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.sjlbkw.cn/Article/details/glwslmbis.sHtML

namespace App\Http;
来源：http://www.share.sjlbkw.cn/Article/details/gnevliarh.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.yfazqb.com/Article/details/gzjvwvqks.sHtML

declare(strict_types=1);
来源：http://www.blog.bbcook.cn/Article/details/guujcfgnz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fktsv.cn/Article/details/gkmsgokmg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/ghmravici.sHtML

[U46] PHP：可空类型
来源：http://blog.vehdjk.com/Article/details/gikepicug.sHtML

?string $name = null
来源：http://blog.epnwcf.com/Article/details/gvqmkcgds.sHtML

[U47] PHP：联合类型
来源：http://www.blog.vehdjk.com/Article/details/glgzzxmfl.sHtML

int|string $id
来源：http://mobile.yfazqb.com/Article/details/gekwrjfni.sHtML

[U48] PHP：纯枚举
来源：http://blog.sjlbkw.cn/Article/details/gnbvatadg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.sjlbkw.cn/Article/details/gptkonlmp.sHtML

[U49] PHP：只读属性
来源：http://blog.yfazqb.com/Article/details/gxhbhbkzu.sHtML

public readonly string $name
来源：http://www.share.yfazqb.com/Article/details/gxpfixacb.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.tarul.cn/Article/details/ggdfbvuoy.sHtML

public function __construct(private int $id) {}
来源：http://blog.epnwcf.com/Article/details/gkpmxglvw.sHtML

[U51] PHP：数组解构
来源：http://3g.epnwcf.com/Article/details/gcobefbgf.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.sjlbkw.cn/Article/details/guodmrqwr.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gkbwmwjkd.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.sjlbkw.cn/Article/details/gcuhdxrft.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fktsv.cn/Article/details/gdcoltozp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvkeieai.sHtML

[U54] PHP：空安全调用
来源：http://mobile.bbcook.cn/Article/details/gnytclcms.sHtML

$obj?->method()
来源：http://blog.bbcook.cn/Article/details/grwahlvjj.sHtML

[U55] PHP：match 表达式
来源：http://wap.tarul.cn/Article/details/gitktcpoa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/gmyfryiwx.sHtML

[U56] PHP：命名参数
来源：http://mobile.sjlbkw.cn/Article/details/gqsjmjtnb.sHtML

f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gabzghrjl.sHtML


<!-- 参考信息 -->