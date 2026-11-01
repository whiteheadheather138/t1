代发 wailian999

memset(a, 0, sizeof a);
来源：http://3g.fktsv.cn/Article/details/gxretmmll.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/ghzbxspax.sHtML

const double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gdoztsick.sHtML

[S28] C：静态变量
来源：http://read.share.tarul.cn/Article/details/gtjbshqqd.sHtML

static int counter = 0;
来源：http://mobile.bbcook.cn/Article/details/gubkxikvg.sHtML

[S29] C：变参函数
来源：http://www.m.share.yfazqb.com/Article/details/gppqizsgf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.bbcook.cn/Article/details/gtxodzbzt.sHtML

[S30] C：头文件保护
来源：http://baike.tarul.cn/Article/details/gzacfxcgq.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/ggawhonpw.sHtML

#define X_H
来源：http://3g.fktsv.cn/Article/details/gbbziebua.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/gmznuqrqr.sHtML

[S31] C++：Hello World
来源：http://read.share.bbcook.cn/Article/details/guolbqerj.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gxchlfvok.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.tarul.cn/Article/details/gsyegukja.sHtML

[S32] C++：字符串
来源：http://www.share.vehdjk.com/Article/details/gxtnkofhi.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.yfazqb.com/Article/details/gvcauoawx.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/gveopjiiy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/gyoszmjcy.sHtML

[S34] C++：遍历 vector
来源：http://mobile.yfazqb.com/Article/details/gqtjnbkjv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.sjlbkw.cn/Article/details/gejmapwni.sHtML

[S35] C++：map
来源：http://www.m.share.sjlbkw.cn/Article/details/gumitilrm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/ggekbfjly.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.epnwcf.com/Article/details/gouxsaxyu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gzkhctxlj.sHtML

[S37] C++：set
来源：http://blog.fktsv.cn/Article/details/gnesjvrin.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.sjlbkw.cn/Article/details/giyndhzcx.sHtML

[S38] C++：排序
来源：http://www.blog.vehdjk.com/Article/details/girnanoto.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.bbcook.cn/Article/details/ggwrihfld.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.yfazqb.com/Article/details/getccmful.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.tarul.cn/Article/details/gtdqkcvhg.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/gtlzhbhng.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.tarul.cn/Article/details/gmymejlwd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/gzxeihtig.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fktsv.cn/Article/details/goazuigms.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/ggzkvtifp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.tarul.cn/Article/details/ghuudlpsm.sHtML

[S43] C++：智能指针
来源：http://blog.epnwcf.com/Article/details/gjoqyzxdb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gcaynxzvo.sHtML

[S44] C++：引用传参
来源：http://www.m.share.bbcook.cn/Article/details/ghqcaxyjs.sHtML

void inc(int &x) { ++x; }
来源：http://baike.bbcook.cn/Article/details/gtsoknxgf.sHtML

[S45] C++：lambda
来源：http://baike.epnwcf.com/Article/details/ghwvgjnkh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.vehdjk.com/Article/details/gpcdcgncq.sHtML

[S46] C++：函数模板
来源：http://blog.tarul.cn/Article/details/gshfqtcij.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.vehdjk.com/Article/details/giimemgkd.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fktsv.cn/Article/details/gtlnwuxtk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.bbcook.cn/Article/details/gpykqvcxk.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gpbuslwoo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fktsv.cn/Article/details/gwotqkshd.sHtML

while (std::getline(in, line)) { }
来源：http://baike.vehdjk.com/Article/details/gneujrdqt.sHtML

[S49] C++：写文件
来源：http://read.share.tarul.cn/Article/details/glqhqceho.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.vehdjk.com/Article/details/gygymudrw.sHtML

[S50] C++：格式化数字
来源：http://baike.yfazqb.com/Article/details/grnoctukc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.tarul.cn/Article/details/gzczyupci.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/gfuprzmej.sHtML

static_cast<double>(a) / b
来源：http://m.share.vehdjk.com/Article/details/glenvewiw.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.vehdjk.com/Article/details/gphlkifan.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/ggeegllbb.sHtML

[S53] C++：移动语义
来源：http://baike.fktsv.cn/Article/details/grvqjvgaf.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.sjlbkw.cn/Article/details/gfrvzpdzf.sHtML

[S54] C++：异常处理
来源：http://baike.fktsv.cn/Article/details/geaywhckf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/gcptiqpci.sHtML

[S55] C++：结构化绑定
来源：http://read.share.epnwcf.com/Article/details/gzqxstyte.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fktsv.cn/Article/details/gnpyjuvvp.sHtML

[S56] C++：optional
来源：http://3g.yfazqb.com/Article/details/gsqlqmcbb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.vehdjk.com/Article/details/gtuoezwgg.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/gnbxhqjyk.sHtML

constexpr int N = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gexchnvbn.sHtML

[S58] C++：命名空间
来源：http://mobile.sjlbkw.cn/Article/details/gyqrvtgwl.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.tarul.cn/Article/details/gwsplwofl.sHtML

[S59] C++：静态断言
来源：http://blog.sjlbkw.cn/Article/details/gblhrjlyn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.yfazqb.com/Article/details/gnwpisubh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gjrnjriqd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.epnwcf.com/Article/details/gvvplckho.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grgezxhps.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gndasokwl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjhgbtcgb.sHtML

[T01] Kotlin：Hello World
来源：http://baike.epnwcf.com/Article/details/gehuapioo.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/gvtuaacdu.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/gqzreoioh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.bbcook.cn/Article/details/gksibpcjd.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/gzeqzqdic.sHtML

"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gbibkfhcc.sHtML

[T04] Kotlin：空安全
来源：http://3g.fktsv.cn/Article/details/glbfikqqm.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gtovwpkao.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.epnwcf.com/Article/details/gmnjejyyr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.yfazqb.com/Article/details/gjgemqlrf.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gtlnsmpzx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.bbcook.cn/Article/details/gtyyuvich.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.tarul.cn/Article/details/giesaeqqg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fktsv.cn/Article/details/gkakwojfq.sHtML

[T08] Kotlin：数据类
来源：http://mobile.sjlbkw.cn/Article/details/gexpcytgf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.bbcook.cn/Article/details/gxlhlktap.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fktsv.cn/Article/details/grhcbuysu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.sjlbkw.cn/Article/details/gpvhvaims.sHtML

[T10] Kotlin：默认参数
来源：http://blog.bbcook.cn/Article/details/ghffpqzwj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gfqysohdo.sHtML

[T11] Kotlin：协程
来源：http://3g.fktsv.cn/Article/details/gscawpcoo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/grlkswnwv.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.sjlbkw.cn/Article/details/gdfwicqnz.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fktsv.cn/Article/details/grbwrfpwt.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.epnwcf.com/Article/details/gzhswwyzq.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fktsv.cn/Article/details/gawoxjuld.sHtML

[T14] Kotlin：循环
来源：http://www.blog.tarul.cn/Article/details/gelmecukp.sHtML

for (i in 1..10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gotchdvya.sHtML

[T15] Kotlin：接口
来源：http://3g.yfazqb.com/Article/details/gvhdeipte.sHtML

interface Shape { fun area(): Double }
来源：http://wap.sjlbkw.cn/Article/details/ghpzpehng.sHtML

[T16] Swift：Hello World
来源：http://blog.tarul.cn/Article/details/gicoizhoa.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gotvwdlsp.sHtML

[T17] Swift：变量与常量
来源：http://mobile.sjlbkw.cn/Article/details/gnrozzaqy.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/gmhtvaqjz.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gofjrdosz.sHtML

"值: \(b)"
来源：http://baike.fktsv.cn/Article/details/ggijnrhbx.sHtML

[T19] Swift：可选绑定
来源：http://baike.vehdjk.com/Article/details/gkzwxnonq.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzeftlbzn.sHtML

[T20] Swift：数组操作
来源：http://wap.sjlbkw.cn/Article/details/gpqgdihmq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.vehdjk.com/Article/details/gqhhrdmra.sHtML

[T21] Swift：遍历
来源：http://wap.fktsv.cn/Article/details/guqyxsvrc.sHtML

for x in a { print(x) }
来源：http://m.share.fktsv.cn/Article/details/gpezdznml.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gvfvpxynt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.epnwcf.com/Article/details/grpdjrxzk.sHtML

[T23] Swift：函数
来源：http://www.blog.fktsv.cn/Article/details/gohiuyjdv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.vehdjk.com/Article/details/geiybbulu.sHtML

[T24] Swift：闭包
来源：http://mobile.epnwcf.com/Article/details/gfzfgplwa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.tarul.cn/Article/details/gficyyhob.sHtML

[T25] Swift：结构体
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzrnlitx.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/gyonermgk.sHtML

[T26] Swift：类与重写
来源：http://www.blog.yfazqb.com/Article/details/gsqtrwyfa.sHtML

class A: Base { override func f() {} }
来源：http://mobile.epnwcf.com/Article/details/gxkonwavj.sHtML

[T27] Swift：错误处理
来源：http://mobile.fktsv.cn/Article/details/grygddmld.sHtML

do { try f() } catch { print(error) }
来源：http://3g.bbcook.cn/Article/details/grumtdhyx.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gobkbpzbm.sHtML

enum Color { case red, green }
来源：http://3g.vehdjk.com/Article/details/gtoyrhztw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gniswxtzg.sHtML

guard let x = opt else { return }
来源：http://m.share.epnwcf.com/Article/details/gnpxields.sHtML

[T30] Swift：协议
来源：http://wap.bbcook.cn/Article/details/gcugndgli.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fktsv.cn/Article/details/gvkfzneqa.sHtML

[T31] Lua：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gtexzvrck.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gvaqqlwdx.sHtML

[T32] Lua：局部变量
来源：http://www.blog.bbcook.cn/Article/details/gbeexnyrc.sHtML

local a = 1
来源：http://mobile.bbcook.cn/Article/details/gampvpzue.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fktsv.cn/Article/details/gmxqooyiq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.epnwcf.com/Article/details/glaleicml.sHtML

[T34] Lua：遍历表
来源：http://3g.bbcook.cn/Article/details/gasszaftr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.tarul.cn/Article/details/ghwpfewbf.sHtML

[T35] Lua：字典表
来源：http://baike.epnwcf.com/Article/details/gbgcujptl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.yfazqb.com/Article/details/ggjeutxcy.sHtML

[T36] Lua：函数
来源：http://baike.tarul.cn/Article/details/gmqnggrig.sHtML

function add(a, b) return a + b end
来源：http://baike.sjlbkw.cn/Article/details/gbuibaqka.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.vehdjk.com/Article/details/gygogxobh.sHtML

"a" .. "b"
来源：http://3g.bbcook.cn/Article/details/gylyzcbig.sHtML

[T38] Lua：条件
来源：http://read.share.epnwcf.com/Article/details/gixqmcpgm.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/gyuadxtef.sHtML

[T39] Lua：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gnmkqwvym.sHtML

string.find(s, "%d+")
来源：http://mobile.sjlbkw.cn/Article/details/gpcznuzwa.sHtML

[T40] Lua：元表
来源：http://www.m.share.bbcook.cn/Article/details/gcppaswwe.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.sjlbkw.cn/Article/details/gfanocsyd.sHtML

[T41] Perl：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gehsszrjv.sHtML

print "Hello\n";
来源：http://blog.bbcook.cn/Article/details/gsyothobq.sHtML

[T42] Perl：变量类型
来源：http://wap.bbcook.cn/Article/details/gbobitrcu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.yfazqb.com/Article/details/gorlmoijt.sHtML

[T43] Perl：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gerhafatu.sHtML

"值: $a"
来源：http://www.blog.vehdjk.com/Article/details/gpzipukdn.sHtML

[T44] Perl：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gvrezafoa.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.vehdjk.com/Article/details/gfmbfpxbo.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gjywpamvd.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.epnwcf.com/Article/details/guhhsptjp.sHtML

[T46] Perl：哈希操作
来源：http://wap.vehdjk.com/Article/details/gnppahwlp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.yfazqb.com/Article/details/gubrcekhf.sHtML

[T47] Perl：正则捕获
来源：http://mobile.epnwcf.com/Article/details/gfpzwhmni.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.vehdjk.com/Article/details/gjrgufmjs.sHtML

[T48] Perl：正则替换
来源：http://read.share.vehdjk.com/Article/details/glximclmm.sHtML

$s =~ s/old/new/g;
来源：http://3g.fktsv.cn/Article/details/gykhvbqyg.sHtML

[T49] Perl：函数
来源：http://mobile.fktsv.cn/Article/details/gwipjdwgt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gfkrwuwqj.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gsypbkgvk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.sjlbkw.cn/Article/details/gsbtelqaz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.yfazqb.com/Article/details/gqupncilp.sHtML

[T51] Scala：Hello World
来源：http://wap.fktsv.cn/Article/details/gxreahdyd.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gouhoiwwa.sHtML

[T52] Scala：变量
来源：http://www.m.share.vehdjk.com/Article/details/gostdsnar.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gcsipxfap.sHtML

[T53] Scala：字符串插值
来源：http://3g.tarul.cn/Article/details/gqbypwxrd.sHtML

s"值: $b"
来源：http://read.share.fktsv.cn/Article/details/ghrybggso.sHtML

[T54] Scala：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gzfjnjoym.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.vehdjk.com/Article/details/gnpvehanj.sHtML

[T55] Scala：集合过滤
来源：http://3g.bbcook.cn/Article/details/glgjzfxsm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.vehdjk.com/Article/details/geccznngc.sHtML

[T56] Scala：样例类
来源：http://www.share.vehdjk.com/Article/details/gjhmkyfmh.sHtML

case class User(name: String, age: Int)
来源：http://blog.fktsv.cn/Article/details/gwxdkpuab.sHtML

[T57] Scala：模式匹配
来源：http://3g.tarul.cn/Article/details/gdpfeereu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.tarul.cn/Article/details/ghcnhtbzs.sHtML

[T58] Scala：函数定义
来源：http://blog.epnwcf.com/Article/details/gbcoctjta.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.sjlbkw.cn/Article/details/goqgwtojy.sHtML

[T59] Scala：循环
来源：http://www.share.bbcook.cn/Article/details/gwrdrfyrc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gkdtmbwif.sHtML

[T60] Scala：折叠
来源：http://read.share.tarul.cn/Article/details/gzlqqwzwc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.vehdjk.com/Article/details/gfbwzigcs.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzsqenzve.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/gcqntzelv.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggtfnqqen.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.yfazqb.com/Article/details/gzgbatprf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.epnwcf.com/Article/details/gsohrkseq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fktsv.cn/Article/details/gijidlrcw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.tarul.cn/Article/details/grrecaqan.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.vehdjk.com/Article/details/gnbpjytps.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.bbcook.cn/Article/details/gizjqkuae.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.epnwcf.com/Article/details/gtcnkfzio.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.yfazqb.com/Article/details/gfooaclzm.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.sjlbkw.cn/Article/details/gvnsinbmh.sHtML

list(dict.fromkeys(arr))
来源：http://wap.bbcook.cn/Article/details/ghepzrflh.sHtML

[U06] Py：合并两个字典
来源：http://baike.epnwcf.com/Article/details/gkxvveaqc.sHtML

{**a, **b}
来源：http://www.m.share.fktsv.cn/Article/details/gpgcnwfhz.sHtML

[U07] Py：反转字典键值
来源：http://www.share.bbcook.cn/Article/details/gsswuujge.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.sjlbkw.cn/Article/details/gtgmnlybs.sHtML

[U08] Py：展平二维列表
来源：http://m.share.sjlbkw.cn/Article/details/gbdsmxcnd.sHtML

[y for x in nested for y in x]
来源：http://baike.fktsv.cn/Article/details/gakjiextl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fktsv.cn/Article/details/gpgzlcakq.sHtML

max(d, key=d.get)
来源：http://mobile.yfazqb.com/Article/details/gtgcpcvam.sHtML

[U10] Py：按值排序字典
来源：http://m.share.epnwcf.com/Article/details/ghpglqnfe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fktsv.cn/Article/details/gcwtydwtq.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.bbcook.cn/Article/details/gmpgjtfby.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gevlgjrrm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fktsv.cn/Article/details/gvxothpwg.sHtML

Counter(arr).most_common(3)
来源：http://www.share.tarul.cn/Article/details/grcmpmrro.sHtML

[U13] Py：固定长度队列
来源：http://mobile.vehdjk.com/Article/details/gonbidntp.sHtML

deque(maxlen=10)
来源：http://www.blog.sjlbkw.cn/Article/details/gappwlmwu.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.epnwcf.com/Article/details/grkihtcih.sHtML

defaultdict(list)
来源：http://blog.vehdjk.com/Article/details/geoeahosb.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.bbcook.cn/Article/details/gesogqckv.sHtML

t = time.perf_counter()
来源：http://www.share.bbcook.cn/Article/details/gtrewrcfi.sHtML

[U16] Py：命令行参数解析
来源：http://wap.tarul.cn/Article/details/ghybsoihf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.yfazqb.com/Article/details/gdthogzup.sHtML

[U17] Py：初始化日志
来源：http://wap.sjlbkw.cn/Article/details/gkvajdhui.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.sjlbkw.cn/Article/details/gaxcvhqcx.sHtML

[U18] Py：预编译正则
来源：http://www.blog.bbcook.cn/Article/details/gbxspueiy.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gjaafybvc.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.tarul.cn/Article/details/gbyagmdht.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.bbcook.cn/Article/details/gromnahlh.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.vehdjk.com/Article/details/gsvyythkz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fktsv.cn/Article/details/gjaqparmb.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.sjlbkw.cn/Article/details/gvjtibgps.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/gfefkmzep.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.vehdjk.com/Article/details/gzvnlusqc.sHtML

list(zip(*m))
来源：http://www.share.tarul.cn/Article/details/grewxfypf.sHtML

[U23] Py：分块读取大文件
来源：http://baike.tarul.cn/Article/details/gliihwdou.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fktsv.cn/Article/details/gmsbyfiry.sHtML

[U24] Py：路径操作
来源：http://read.share.bbcook.cn/Article/details/gkxihqqsd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/grhmmqtyk.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.vehdjk.com/Article/details/gpaddqcia.sHtML

csv.DictReader(f)
来源：http://blog.vehdjk.com/Article/details/gibwnklpj.sHtML

[U26] Py：并发下载
来源：http://read.share.epnwcf.com/Article/details/gydygojpo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.vehdjk.com/Article/details/gxgumqmxo.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.bbcook.cn/Article/details/gptyiwjbe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fktsv.cn/Article/details/gbbkdbmfy.sHtML

[U28] Py：类型别名
来源：http://3g.tarul.cn/Article/details/gyveudpon.sHtML

UserId = int
来源：http://www.m.share.sjlbkw.cn/Article/details/gljkkhrpi.sHtML

[U29] Py：属性校验
来源：http://mobile.epnwcf.com/Article/details/gjucknzoi.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fktsv.cn/Article/details/gojuamywv.sHtML

[U30] Py：数据类
来源：http://3g.fktsv.cn/Article/details/gjknetwsw.sHtML

@dataclass(slots=True)
来源：http://www.m.share.vehdjk.com/Article/details/gqoquuehb.sHtML

[U31] Py：单测
来源：http://m.share.epnwcf.com/Article/details/gaezwrqau.sHtML

python -m pytest -q
来源：http://www.share.vehdjk.com/Article/details/gylmpnraj.sHtML

[U32] Py：代码格式化
来源：http://mobile.sjlbkw.cn/Article/details/gargdgipq.sHtML

ruff format . && ruff check --fix .
来源：http://baike.yfazqb.com/Article/details/gcgmapyuc.sHtML

[U33] Py：打包发布
来源：http://blog.tarul.cn/Article/details/ggnrfgwyi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.tarul.cn/Article/details/grhhrsykp.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fktsv.cn/Article/details/gihgomjnf.sHtML

chardet.detect(raw)
来源：http://mobile.sjlbkw.cn/Article/details/gnsfcvjlf.sHtML

[U35] Py：发送邮件
来源：http://m.share.yfazqb.com/Article/details/geatnilsm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.yfazqb.com/Article/details/gwhhrpftl.sHtML

[U36] Py：定时任务
来源：http://wap.bbcook.cn/Article/details/gstwexgfl.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.vehdjk.com/Article/details/gbrnidhev.sHtML

[U37] Py：读写 Excel
来源：http://m.share.epnwcf.com/Article/details/gsmbnpqsz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.yfazqb.com/Article/details/gihyraoms.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fktsv.cn/Article/details/ggefpfqvb.sHtML

Path(__file__).resolve().parent
来源：http://www.share.epnwcf.com/Article/details/goeolsxsf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.tarul.cn/Article/details/ggptosyeb.sHtML

sys.stdout.isatty()
来源：http://www.share.bbcook.cn/Article/details/gvlnyekzh.sHtML

[U40] Py：打印到标准错误
来源：http://3g.epnwcf.com/Article/details/gdeskzkdc.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/gtrrnxfls.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.tarul.cn/Article/details/gpzbfsbis.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.yfazqb.com/Article/details/gszikcmco.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.bbcook.cn/Article/details/giqjnjkqm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fktsv.cn/Article/details/gvsslvxkg.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.epnwcf.com/Article/details/goqlxsuip.sHtML

namespace App\Http;
来源：http://read.share.vehdjk.com/Article/details/gkobsnjig.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.sjlbkw.cn/Article/details/ggrbvvjlv.sHtML

declare(strict_types=1);
来源：http://read.share.vehdjk.com/Article/details/gflfvtwgz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.tarul.cn/Article/details/gkwktdvps.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/ggxulbqph.sHtML

[U46] PHP：可空类型
来源：http://m.share.bbcook.cn/Article/details/gzqjmtuyl.sHtML

?string $name = null
来源：http://blog.yfazqb.com/Article/details/gtjdrhhsm.sHtML

[U47] PHP：联合类型
来源：http://mobile.yfazqb.com/Article/details/goomnxpbx.sHtML

int|string $id
来源：http://3g.epnwcf.com/Article/details/gubrzkyqw.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fktsv.cn/Article/details/gedgzpcsz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.tarul.cn/Article/details/gjqfyomsp.sHtML

[U49] PHP：只读属性
来源：http://www.share.bbcook.cn/Article/details/grneqcbhp.sHtML

public readonly string $name
来源：http://3g.yfazqb.com/Article/details/grjocedlp.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.bbcook.cn/Article/details/gwjfwgvnm.sHtML

public function __construct(private int $id) {}
来源：http://www.share.vehdjk.com/Article/details/gkghnxlmx.sHtML


<!-- 参考信息 -->