代发 wailian999

[S35] C++：map
来源：http://mobile.vehdjk.com/Article/details/gxsjslnao.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gyiiomvod.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gjztaajrz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gthhfpzam.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gsawvlwrc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fktsv.cn/Article/details/gfvldtrro.sHtML

[S38] C++：排序
来源：http://mobile.tarul.cn/Article/details/gcyymvkvo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/ghaynveci.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gmaggxozt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/gdyyjntzc.sHtML

[S40] C++：查找元素
来源：http://mobile.vehdjk.com/Article/details/gdookmfri.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.epnwcf.com/Article/details/gkvwuxuai.sHtML

[S41] C++：类与构造函数
来源：http://m.share.sjlbkw.cn/Article/details/glevnvcmf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/gelgnilen.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.tarul.cn/Article/details/gsfutkbpx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.sjlbkw.cn/Article/details/ghtxeyaga.sHtML

[S43] C++：智能指针
来源：http://baike.vehdjk.com/Article/details/gkglgvhxv.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/glynaaekf.sHtML

[S44] C++：引用传参
来源：http://read.share.yfazqb.com/Article/details/gjukcxbty.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/gmzgtijrs.sHtML

[S45] C++：lambda
来源：http://3g.yfazqb.com/Article/details/gwjbzkbik.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.tarul.cn/Article/details/ggwsmecxm.sHtML

[S46] C++：函数模板
来源：http://www.share.sjlbkw.cn/Article/details/gsnwfaait.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/gzkkeztgm.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fktsv.cn/Article/details/gngyvbxts.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.vehdjk.com/Article/details/gegmrglqq.sHtML

[S48] C++：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gvisuxhhi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/ghdjdlqjz.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fktsv.cn/Article/details/gbxidzvkq.sHtML

[S49] C++：写文件
来源：http://blog.sjlbkw.cn/Article/details/gaakcetwg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/gxjvicdhr.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.vehdjk.com/Article/details/gwynigbdh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gicaomldf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gdndcvwra.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/gemxpbhni.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/gmkbvigjz.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.epnwcf.com/Article/details/gkgfohuhm.sHtML

[S53] C++：移动语义
来源：http://www.m.share.sjlbkw.cn/Article/details/genamzqwf.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fktsv.cn/Article/details/gsqkbkimr.sHtML

[S54] C++：异常处理
来源：http://mobile.bbcook.cn/Article/details/grqspkqmo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.vehdjk.com/Article/details/ggzpexkmw.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fktsv.cn/Article/details/gyynukbea.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/genllhbwj.sHtML

[S56] C++：optional
来源：http://wap.bbcook.cn/Article/details/gzchjurnj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/gkrkpndso.sHtML

[S57] C++：编译期常量
来源：http://m.share.sjlbkw.cn/Article/details/ghvzrukmt.sHtML

constexpr int N = 10;
来源：http://baike.fktsv.cn/Article/details/gldapcqku.sHtML

[S58] C++：命名空间
来源：http://m.share.fktsv.cn/Article/details/gvwxwvwns.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fktsv.cn/Article/details/gbmziooyt.sHtML

[S59] C++：静态断言
来源：http://3g.bbcook.cn/Article/details/gwezeiicd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.yfazqb.com/Article/details/gqcglvclx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.epnwcf.com/Article/details/gqxsmubua.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gvvzxjtqd.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggiujofvd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gbtjwpldi.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqbtwhsxd.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gfkkhzxxm.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/grrftyubv.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.epnwcf.com/Article/details/gjxiyzumq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.sjlbkw.cn/Article/details/gukctooup.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.tarul.cn/Article/details/gnmuxebrx.sHtML

"值: $b"
来源：http://www.blog.tarul.cn/Article/details/grrafdowu.sHtML

[T04] Kotlin：空安全
来源：http://www.share.tarul.cn/Article/details/gndkloeqi.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gxbmusuuf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fktsv.cn/Article/details/gskvcywkm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.vehdjk.com/Article/details/gveznsfoo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gygyhkrom.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.vehdjk.com/Article/details/gzpycjzzb.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fktsv.cn/Article/details/gyisirklh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.epnwcf.com/Article/details/glaysbfqz.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/gakbomvdo.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fktsv.cn/Article/details/gzjmtxutr.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fktsv.cn/Article/details/gyrhtqrxc.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.tarul.cn/Article/details/gcyipagcx.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.vehdjk.com/Article/details/gdetfuctm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.tarul.cn/Article/details/gpfppgrlh.sHtML

[T11] Kotlin：协程
来源：http://blog.fktsv.cn/Article/details/gccpvaqbw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.bbcook.cn/Article/details/gtqtkhkyw.sHtML

[T12] Kotlin：解构声明
来源：http://blog.sjlbkw.cn/Article/details/griuucfgd.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gmtksbhuc.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.sjlbkw.cn/Article/details/ghcfgtaij.sHtML

val m = mapOf("a" to 1)
来源：http://3g.yfazqb.com/Article/details/gtqfowkqb.sHtML

[T14] Kotlin：循环
来源：http://wap.sjlbkw.cn/Article/details/gpgnfaecv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gvadtkrpo.sHtML

[T15] Kotlin：接口
来源：http://wap.bbcook.cn/Article/details/gnvibnifv.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/giwhzyafx.sHtML

[T16] Swift：Hello World
来源：http://3g.yfazqb.com/Article/details/gvyznzujg.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gvqoydice.sHtML

[T17] Swift：变量与常量
来源：http://baike.vehdjk.com/Article/details/gsugyqekq.sHtML

var a = 1;  let b = 2
来源：http://mobile.fktsv.cn/Article/details/gtdrfkoti.sHtML

[T18] Swift：字符串插值
来源：http://3g.epnwcf.com/Article/details/gawuehrie.sHtML

"值: \(b)"
来源：http://www.share.epnwcf.com/Article/details/gqekgaqfn.sHtML

[T19] Swift：可选绑定
来源：http://blog.fktsv.cn/Article/details/gtysmgdmt.sHtML

if let n = opt { print(n) }
来源：http://wap.vehdjk.com/Article/details/gnzezgxoc.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/gujwbwcdh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.tarul.cn/Article/details/gbzuqyvag.sHtML

[T21] Swift：遍历
来源：http://3g.bbcook.cn/Article/details/grbapqylq.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/gqkljugon.sHtML

[T22] Swift：字典
来源：http://baike.sjlbkw.cn/Article/details/gupzqefpz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.sjlbkw.cn/Article/details/gdclivzge.sHtML

[T23] Swift：函数
来源：http://mobile.vehdjk.com/Article/details/gkdjhjosw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.epnwcf.com/Article/details/garscjvkj.sHtML

[T24] Swift：闭包
来源：http://3g.epnwcf.com/Article/details/ghriupvgg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/ghvoemzwg.sHtML

[T25] Swift：结构体
来源：http://www.m.share.bbcook.cn/Article/details/gcxdxtoyp.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/gkzceokua.sHtML

[T26] Swift：类与重写
来源：http://3g.yfazqb.com/Article/details/gnutxftle.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/glztcmqmn.sHtML

[T27] Swift：错误处理
来源：http://m.share.epnwcf.com/Article/details/gjimcshhc.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fktsv.cn/Article/details/grcfcmoxi.sHtML

[T28] Swift：枚举
来源：http://wap.tarul.cn/Article/details/gtqmvjysp.sHtML

enum Color { case red, green }
来源：http://3g.vehdjk.com/Article/details/gqjdwnbrr.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.epnwcf.com/Article/details/glhlbfkno.sHtML

guard let x = opt else { return }
来源：http://blog.vehdjk.com/Article/details/gpbgsrpgq.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/ghqbxqpeg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.yfazqb.com/Article/details/glzyjgigz.sHtML

[T31] Lua：Hello World
来源：http://3g.tarul.cn/Article/details/gmuzjobts.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/gayqffcjb.sHtML

[T32] Lua：局部变量
来源：http://blog.fktsv.cn/Article/details/gbokpkjeh.sHtML

local a = 1
来源：http://3g.yfazqb.com/Article/details/gkwotcejr.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fktsv.cn/Article/details/glicqbpku.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.bbcook.cn/Article/details/ghnqqjxuk.sHtML

[T34] Lua：遍历表
来源：http://3g.epnwcf.com/Article/details/gdoctbtrs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/gwrakjmxt.sHtML

[T35] Lua：字典表
来源：http://www.share.bbcook.cn/Article/details/gixpabjto.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.bbcook.cn/Article/details/gxcrnmibn.sHtML

[T36] Lua：函数
来源：http://www.m.share.epnwcf.com/Article/details/gjpbgiemq.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.yfazqb.com/Article/details/gzvmkkojd.sHtML

[T37] Lua：字符串拼接
来源：http://blog.bbcook.cn/Article/details/gufrrplyy.sHtML

"a" .. "b"
来源：http://baike.yfazqb.com/Article/details/gsodootnl.sHtML

[T38] Lua：条件
来源：http://blog.sjlbkw.cn/Article/details/gyxtsqtqo.sHtML

if x > 0 then print("正") end
来源：http://blog.yfazqb.com/Article/details/gtryjudsd.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.tarul.cn/Article/details/gptrtwdyi.sHtML

string.find(s, "%d+")
来源：http://www.m.share.bbcook.cn/Article/details/gjbmgmibe.sHtML

[T40] Lua：元表
来源：http://3g.fktsv.cn/Article/details/gsqlhwcro.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fktsv.cn/Article/details/gclczjgya.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/glltaquci.sHtML

print "Hello\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/glyzomngj.sHtML

[T42] Perl：变量类型
来源：http://mobile.vehdjk.com/Article/details/gxfdubric.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.vehdjk.com/Article/details/gxozjoizk.sHtML

[T43] Perl：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gvkropnwo.sHtML

"值: $a"
来源：http://blog.bbcook.cn/Article/details/goaasyruv.sHtML

[T44] Perl：条件
来源：http://www.m.share.bbcook.cn/Article/details/gvwtwqyzg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvqwrwlv.sHtML

[T45] Perl：数组遍历
来源：http://mobile.bbcook.cn/Article/details/guhibrbyr.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.yfazqb.com/Article/details/gaqoplxwv.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsjckvca.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/gnivmuftv.sHtML

[T47] Perl：正则捕获
来源：http://read.share.epnwcf.com/Article/details/gpihmbidy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.sjlbkw.cn/Article/details/gggxgeykv.sHtML

[T48] Perl：正则替换
来源：http://baike.yfazqb.com/Article/details/guhalczxl.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/gcdphamyc.sHtML

[T49] Perl：函数
来源：http://baike.sjlbkw.cn/Article/details/gxwhgqhgo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gfwzrpkyr.sHtML

[T50] Perl：逐行读文件
来源：http://baike.tarul.cn/Article/details/gpbktyahq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.tarul.cn/Article/details/ghkbqzgwj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fktsv.cn/Article/details/gknyiaedi.sHtML

[T51] Scala：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gssbigbdi.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gmdahdhjx.sHtML

[T52] Scala：变量
来源：http://read.share.bbcook.cn/Article/details/gkgbylrjr.sHtML

val a = 1;  var b = 2
来源：http://read.share.tarul.cn/Article/details/ggupajunw.sHtML

[T53] Scala：字符串插值
来源：http://baike.vehdjk.com/Article/details/giqidhvqb.sHtML

s"值: $b"
来源：http://www.share.epnwcf.com/Article/details/gfcbngydm.sHtML

[T54] Scala：集合映射
来源：http://m.share.tarul.cn/Article/details/gjcocrxny.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fktsv.cn/Article/details/gvpzooomr.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/grwipltln.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.bbcook.cn/Article/details/glnhpoczh.sHtML

[T56] Scala：样例类
来源：http://www.m.share.yfazqb.com/Article/details/gggpxqnqa.sHtML

case class User(name: String, age: Int)
来源：http://m.share.epnwcf.com/Article/details/ggqxkmsew.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gokppsbwy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.bbcook.cn/Article/details/geuwiuhma.sHtML

[T58] Scala：函数定义
来源：http://read.share.sjlbkw.cn/Article/details/gnvqoxgmu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.epnwcf.com/Article/details/giimgukjl.sHtML

[T59] Scala：循环
来源：http://baike.tarul.cn/Article/details/grqqwyyxd.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gjmiyxgct.sHtML

[T60] Scala：折叠
来源：http://read.share.epnwcf.com/Article/details/ggcscdzol.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.yfazqb.com/Article/details/gnzdrjhgw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grkumltqh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.epnwcf.com/Article/details/gxvpwglhu.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glsevopwx.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.tarul.cn/Article/details/gyslkestr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.tarul.cn/Article/details/gctvlmsdl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fktsv.cn/Article/details/gqjojediv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.vehdjk.com/Article/details/gvnovcsxm.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.epnwcf.com/Article/details/ggalclndl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fktsv.cn/Article/details/gwqiskqvb.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.sjlbkw.cn/Article/details/gdockppwr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.sjlbkw.cn/Article/details/gsvuqmfva.sHtML

[U05] Py：列表去重且保序
来源：http://blog.sjlbkw.cn/Article/details/gnswkxxrn.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.bbcook.cn/Article/details/gzcvqymwu.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.vehdjk.com/Article/details/gwzyeeahy.sHtML

{**a, **b}
来源：http://www.m.share.fktsv.cn/Article/details/ghonzrypj.sHtML

[U07] Py：反转字典键值
来源：http://blog.epnwcf.com/Article/details/gzstyaoqn.sHtML

{v: k for k, v in d.items()}
来源：http://wap.tarul.cn/Article/details/ggeqrvhso.sHtML

[U08] Py：展平二维列表
来源：http://wap.sjlbkw.cn/Article/details/gknfaqfid.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fktsv.cn/Article/details/gxdlkfhyb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fktsv.cn/Article/details/geycbstot.sHtML

max(d, key=d.get)
来源：http://mobile.bbcook.cn/Article/details/gzvebdszi.sHtML

[U10] Py：按值排序字典
来源：http://read.share.sjlbkw.cn/Article/details/giyxrvulx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.tarul.cn/Article/details/gptfonsxo.sHtML

[U11] Py：生成器表达式
来源：http://3g.bbcook.cn/Article/details/gobfqcntk.sHtML

(x * 2 for x in arr)
来源：http://www.share.epnwcf.com/Article/details/gdxymgtkx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.tarul.cn/Article/details/gomjvamyw.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.epnwcf.com/Article/details/gnikgrkzo.sHtML

[U13] Py：固定长度队列
来源：http://www.share.vehdjk.com/Article/details/gcmdwmboi.sHtML

deque(maxlen=10)
来源：http://3g.tarul.cn/Article/details/gofnvjusc.sHtML

[U14] Py：分组收集到列表
来源：http://wap.epnwcf.com/Article/details/gyaecmbpz.sHtML

defaultdict(list)
来源：http://www.share.vehdjk.com/Article/details/gjpeakivg.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.vehdjk.com/Article/details/gslrymohi.sHtML

t = time.perf_counter()
来源：http://www.blog.tarul.cn/Article/details/gptetjmol.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.bbcook.cn/Article/details/gshyvvdsx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.epnwcf.com/Article/details/ghcpzwbqk.sHtML

[U17] Py：初始化日志
来源：http://m.share.tarul.cn/Article/details/gcfuvdvbd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fktsv.cn/Article/details/gkqopsnza.sHtML

[U18] Py：预编译正则
来源：http://baike.fktsv.cn/Article/details/ghiuqzsus.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.vehdjk.com/Article/details/gbbfrbrwd.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.bbcook.cn/Article/details/gessdpghf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.tarul.cn/Article/details/gxruxpgme.sHtML

[U20] Py：缓存函数结果
来源：http://wap.yfazqb.com/Article/details/gursktktd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.tarul.cn/Article/details/gsqvkbmus.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.sjlbkw.cn/Article/details/gsnkoyyza.sHtML

@contextlib.contextmanager
来源：http://mobile.yfazqb.com/Article/details/gzglauwby.sHtML

[U22] Py：矩阵转置
来源：http://read.share.yfazqb.com/Article/details/gkvjxdmqt.sHtML

list(zip(*m))
来源：http://wap.bbcook.cn/Article/details/gyehyvhst.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fktsv.cn/Article/details/gelpnsbdi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.bbcook.cn/Article/details/godximyap.sHtML

[U24] Py：路径操作
来源：http://read.share.fktsv.cn/Article/details/gouwebilw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gjlslverd.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.sjlbkw.cn/Article/details/gyjgwgcbj.sHtML

csv.DictReader(f)
来源：http://wap.tarul.cn/Article/details/gngmfdhvh.sHtML

[U26] Py：并发下载
来源：http://blog.fktsv.cn/Article/details/ghmfgqewg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.yfazqb.com/Article/details/gvawexcud.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.epnwcf.com/Article/details/gkzhcxsoz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.epnwcf.com/Article/details/gqnudkydc.sHtML

[U28] Py：类型别名
来源：http://www.m.share.bbcook.cn/Article/details/gpjrzemhu.sHtML

UserId = int
来源：http://blog.sjlbkw.cn/Article/details/gpfajwups.sHtML

[U29] Py：属性校验
来源：http://www.m.share.tarul.cn/Article/details/gijgsdwzt.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gcjdwllft.sHtML

[U30] Py：数据类
来源：http://wap.bbcook.cn/Article/details/gugizxxqw.sHtML

@dataclass(slots=True)
来源：http://mobile.epnwcf.com/Article/details/glxifuidz.sHtML

[U31] Py：单测
来源：http://baike.bbcook.cn/Article/details/ghmztshwc.sHtML

python -m pytest -q
来源：http://m.share.epnwcf.com/Article/details/gggmlepdt.sHtML

[U32] Py：代码格式化
来源：http://baike.fktsv.cn/Article/details/gspnkaqbf.sHtML

ruff format . && ruff check --fix .
来源：http://wap.sjlbkw.cn/Article/details/gwxdcbnyw.sHtML

[U33] Py：打包发布
来源：http://www.m.share.yfazqb.com/Article/details/gfwcpdqei.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.bbcook.cn/Article/details/gfvioluey.sHtML

[U34] Py：判断编码
来源：http://blog.bbcook.cn/Article/details/grnqzfhkp.sHtML

chardet.detect(raw)
来源：http://baike.fktsv.cn/Article/details/gbjxtnzux.sHtML

[U35] Py：发送邮件
来源：http://www.blog.sjlbkw.cn/Article/details/gedurbnqd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.bbcook.cn/Article/details/gzvujgvpl.sHtML

[U36] Py：定时任务
来源：http://www.share.fktsv.cn/Article/details/gadwghqva.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.tarul.cn/Article/details/greaoplpq.sHtML

[U37] Py：读写 Excel
来源：http://www.share.epnwcf.com/Article/details/gnxtzboms.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.vehdjk.com/Article/details/gdpqhhlvd.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.tarul.cn/Article/details/gnricynpi.sHtML

Path(__file__).resolve().parent
来源：http://baike.yfazqb.com/Article/details/ghvdxusmz.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.tarul.cn/Article/details/ggehwanpd.sHtML

sys.stdout.isatty()
来源：http://wap.fktsv.cn/Article/details/gcxguksto.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.bbcook.cn/Article/details/gqtgeccua.sHtML

print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/gczdjfxze.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.yfazqb.com/Article/details/gtlsghetl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fktsv.cn/Article/details/ggvdbamfd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.tarul.cn/Article/details/goytcgulc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.sjlbkw.cn/Article/details/gymtnuufi.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.sjlbkw.cn/Article/details/gtvyzwswe.sHtML

namespace App\Http;
来源：http://www.m.share.tarul.cn/Article/details/gcwhcubhg.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.epnwcf.com/Article/details/gnyhxujmc.sHtML

declare(strict_types=1);
来源：http://read.share.vehdjk.com/Article/details/grlusrnow.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fktsv.cn/Article/details/glkongczm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gckejjtaf.sHtML

[U46] PHP：可空类型
来源：http://baike.tarul.cn/Article/details/giwkxsulr.sHtML

?string $name = null
来源：http://www.share.vehdjk.com/Article/details/gbjcskoag.sHtML

[U47] PHP：联合类型
来源：http://blog.bbcook.cn/Article/details/gmsoyjgvp.sHtML

int|string $id
来源：http://baike.sjlbkw.cn/Article/details/gskoiszuz.sHtML

[U48] PHP：纯枚举
来源：http://wap.epnwcf.com/Article/details/gedzqtxcs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.tarul.cn/Article/details/gxpdtzztn.sHtML

[U49] PHP：只读属性
来源：http://www.share.yfazqb.com/Article/details/gkejdyhdu.sHtML

public readonly string $name
来源：http://3g.yfazqb.com/Article/details/gwqafbpma.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.sjlbkw.cn/Article/details/gfnrnpufl.sHtML

public function __construct(private int $id) {}
来源：http://m.share.vehdjk.com/Article/details/goucxvpqt.sHtML

[U51] PHP：数组解构
来源：http://www.share.vehdjk.com/Article/details/gmndnwvbq.sHtML

[$a, $b] = $arr;
来源：http://mobile.epnwcf.com/Article/details/gzdoomhmv.sHtML

[U52] PHP：箭头函数
来源：http://blog.epnwcf.com/Article/details/gsrnacymh.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.epnwcf.com/Article/details/gxfqdyhgm.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.yfazqb.com/Article/details/gksmvojkd.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.tarul.cn/Article/details/giphyaurt.sHtML

[U54] PHP：空安全调用
来源：http://read.share.yfazqb.com/Article/details/ggacjwrjb.sHtML

$obj?->method()
来源：http://read.share.epnwcf.com/Article/details/gynwxnoub.sHtML

[U55] PHP：match 表达式
来源：http://blog.epnwcf.com/Article/details/gbjxfbmqu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.yfazqb.com/Article/details/gspjpztlz.sHtML

[U56] PHP：命名参数
来源：http://3g.epnwcf.com/Article/details/guarlfkys.sHtML

f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gmhugazqp.sHtML

[U57] PHP：字符串插值
来源：http://3g.vehdjk.com/Article/details/gvjszqsgs.sHtML

"值: {$a}"
来源：http://3g.epnwcf.com/Article/details/gqgsplmqz.sHtML

[U58] PHP：数组三件套
来源：http://wap.sjlbkw.cn/Article/details/gtlhkcsef.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.vehdjk.com/Article/details/gfawnwijt.sHtML

[U59] PHP：自定义排序
来源：http://wap.epnwcf.com/Article/details/gklyoabbu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/grdzpbykf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.tarul.cn/Article/details/gdqtxqses.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.vehdjk.com/Article/details/gsytvpvze.sHtML


<!-- 参考信息 -->