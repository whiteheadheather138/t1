代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/ggfpsczwf.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/gzhxitqta.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.epnwcf.com/Article/details/gsexzfbtd.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/glsvyxzlb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.tarul.cn/Article/details/gycbapxfk.sHtML

[S23] C：随机数
来源：http://mobile.tarul.cn/Article/details/gjmaumlky.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.tarul.cn/Article/details/gpolzsfry.sHtML

[S24] C：获取本地时间
来源：http://blog.sjlbkw.cn/Article/details/ghhggdghm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/gefpayxfi.sHtML

[S25] C：内存拷贝
来源：http://www.share.tarul.cn/Article/details/ggtymilii.sHtML

memcpy(dst, src, n);
来源：http://baike.fktsv.cn/Article/details/ggokcikkt.sHtML

[S26] C：内存清零
来源：http://m.share.fktsv.cn/Article/details/gphknbkvu.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.yfazqb.com/Article/details/gmeesnzcn.sHtML

[S27] C：定义常量
来源：http://www.share.fktsv.cn/Article/details/glxuoagvo.sHtML

const double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gbjoshepn.sHtML

[S28] C：静态变量
来源：http://www.share.epnwcf.com/Article/details/gopiyoqpw.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/gxvoeayco.sHtML

[S29] C：变参函数
来源：http://3g.sjlbkw.cn/Article/details/glgrjsmst.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.tarul.cn/Article/details/gzhquaqwd.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/gdiqcasov.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/gvjuzwhfg.sHtML

#define X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gbsolndgm.sHtML

#endif
来源：http://read.share.bbcook.cn/Article/details/gqldfirzp.sHtML

[S31] C++：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gctdxxsnl.sHtML

#include <iostream>
来源：http://www.share.bbcook.cn/Article/details/gcfzmjvlw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.tarul.cn/Article/details/gjufjsftu.sHtML

[S32] C++：字符串
来源：http://www.share.vehdjk.com/Article/details/glenobxys.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.tarul.cn/Article/details/gsblpbddx.sHtML

[S33] C++：vector 增删
来源：http://mobile.bbcook.cn/Article/details/gpajoudpv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.bbcook.cn/Article/details/gcotieanf.sHtML

[S34] C++：遍历 vector
来源：http://m.share.sjlbkw.cn/Article/details/gieafuhgv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.vehdjk.com/Article/details/ggkusbguz.sHtML

[S35] C++：map
来源：http://read.share.vehdjk.com/Article/details/girlobsfi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gitkucmnt.sHtML

[S36] C++：unordered_map
来源：http://read.share.sjlbkw.cn/Article/details/gobczkkle.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gxbpsueqz.sHtML

[S37] C++：set
来源：http://m.share.epnwcf.com/Article/details/glchlamji.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.vehdjk.com/Article/details/gppwoksab.sHtML

[S38] C++：排序
来源：http://m.share.bbcook.cn/Article/details/ggfkrlcqy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/gayxdxrcx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.bbcook.cn/Article/details/gimxatmuk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.vehdjk.com/Article/details/gygbutrsm.sHtML

[S40] C++：查找元素
来源：http://blog.sjlbkw.cn/Article/details/gsqfrguxe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.tarul.cn/Article/details/gnlscoqia.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/gdjocqezf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.yfazqb.com/Article/details/gipmwqzfe.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.epnwcf.com/Article/details/gwsitbeod.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.vehdjk.com/Article/details/gozijxtuw.sHtML

[S43] C++：智能指针
来源：http://www.m.share.yfazqb.com/Article/details/gpuivnxwo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.vehdjk.com/Article/details/gyzsrndza.sHtML

[S44] C++：引用传参
来源：http://wap.tarul.cn/Article/details/gdytoaodd.sHtML

void inc(int &x) { ++x; }
来源：http://blog.tarul.cn/Article/details/gyniyvenb.sHtML

[S45] C++：lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmmxsnda.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.vehdjk.com/Article/details/gwwoqypcu.sHtML

[S46] C++：函数模板
来源：http://3g.bbcook.cn/Article/details/grvgroivz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrelbbnv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.tarul.cn/Article/details/glzhanpmn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.yfazqb.com/Article/details/gcjydwrqn.sHtML

[S48] C++：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gjassspgt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fktsv.cn/Article/details/gbmuarbua.sHtML

while (std::getline(in, line)) { }
来源：http://baike.yfazqb.com/Article/details/guxccyqxe.sHtML

[S49] C++：写文件
来源：http://mobile.bbcook.cn/Article/details/grxpeowuh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.tarul.cn/Article/details/gxwbrilye.sHtML

[S50] C++：格式化数字
来源：http://www.blog.epnwcf.com/Article/details/ghvhasgpn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gdnjvjedu.sHtML

[S51] C++：显式类型转换
来源：http://wap.vehdjk.com/Article/details/gplcjbfxg.sHtML

static_cast<double>(a) / b
来源：http://read.share.vehdjk.com/Article/details/gmnmbxygn.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fktsv.cn/Article/details/getttuvtv.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.yfazqb.com/Article/details/griunacdl.sHtML

[S53] C++：移动语义
来源：http://read.share.bbcook.cn/Article/details/gcvqfavdv.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.yfazqb.com/Article/details/grskkdfog.sHtML

[S54] C++：异常处理
来源：http://mobile.epnwcf.com/Article/details/gcqdisnjq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.epnwcf.com/Article/details/gqjotbcbi.sHtML

[S55] C++：结构化绑定
来源：http://3g.fktsv.cn/Article/details/gohgmxcnw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.tarul.cn/Article/details/gizzxqvom.sHtML

[S56] C++：optional
来源：http://wap.bbcook.cn/Article/details/grkfzimdv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/gyxjatcpc.sHtML

[S57] C++：编译期常量
来源：http://www.share.bbcook.cn/Article/details/gpwwbvury.sHtML

constexpr int N = 10;
来源：http://blog.sjlbkw.cn/Article/details/ggdwfptyj.sHtML

[S58] C++：命名空间
来源：http://3g.bbcook.cn/Article/details/gikqmukur.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.vehdjk.com/Article/details/gsjqhfkah.sHtML

[S59] C++：静态断言
来源：http://wap.sjlbkw.cn/Article/details/gxltvsjuw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.epnwcf.com/Article/details/gmhrxidrm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gvdwixwgw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/goyrkcucn.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gwtursqgx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gzpdlubqh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gsfxhngld.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.tarul.cn/Article/details/gpikxprxg.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gobjyarwe.sHtML

[T02] Kotlin：变量
来源：http://www.blog.epnwcf.com/Article/details/gmkjhxdry.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.epnwcf.com/Article/details/gitiwmhnf.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.epnwcf.com/Article/details/gdvpmuhcx.sHtML

"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/ghmvggvyc.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/gwpsnhxpt.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.vehdjk.com/Article/details/gohgaqami.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.epnwcf.com/Article/details/ghfxehpjx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.epnwcf.com/Article/details/gbblfvizm.sHtML

[T06] Kotlin：集合映射
来源：http://3g.epnwcf.com/Article/details/gcdlozqcp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.tarul.cn/Article/details/gocrmhkit.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fktsv.cn/Article/details/gpgooewaz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.sjlbkw.cn/Article/details/grzqstqve.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/goxfdehnz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fktsv.cn/Article/details/gqnhetato.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fktsv.cn/Article/details/gwfjqsfll.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.tarul.cn/Article/details/gutrlisgk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.epnwcf.com/Article/details/gtwttstjh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.epnwcf.com/Article/details/gadfwjdzh.sHtML

[T11] Kotlin：协程
来源：http://mobile.vehdjk.com/Article/details/gfqqvlvlf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.epnwcf.com/Article/details/gotenchak.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.epnwcf.com/Article/details/gpxafzsdz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gupbthlcl.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.vehdjk.com/Article/details/gftsinsur.sHtML

val m = mapOf("a" to 1)
来源：http://blog.sjlbkw.cn/Article/details/gdnrhudae.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/ghdzlstjn.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gckwulkcp.sHtML

[T15] Kotlin：接口
来源：http://wap.fktsv.cn/Article/details/gjdaqvldv.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.epnwcf.com/Article/details/gnlnktvsf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/guqwcvjnf.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/gqramlxsy.sHtML

[T17] Swift：变量与常量
来源：http://mobile.bbcook.cn/Article/details/gfwdnyskt.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/guygysmta.sHtML

[T18] Swift：字符串插值
来源：http://3g.vehdjk.com/Article/details/gmrcgtdre.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gghjrkkea.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.bbcook.cn/Article/details/gmkpqgzlr.sHtML

if let n = opt { print(n) }
来源：http://read.share.epnwcf.com/Article/details/glftzdtqp.sHtML

[T20] Swift：数组操作
来源：http://3g.sjlbkw.cn/Article/details/gieuiuasg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.epnwcf.com/Article/details/gaqemqgyk.sHtML

[T21] Swift：遍历
来源：http://www.share.yfazqb.com/Article/details/gmsvymnyg.sHtML

for x in a { print(x) }
来源：http://read.share.vehdjk.com/Article/details/gseojelxe.sHtML

[T22] Swift：字典
来源：http://3g.sjlbkw.cn/Article/details/geqqzhrde.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.epnwcf.com/Article/details/gkmzqcuyt.sHtML

[T23] Swift：函数
来源：http://www.share.vehdjk.com/Article/details/gfstakwbd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gptzkvify.sHtML

[T24] Swift：闭包
来源：http://baike.fktsv.cn/Article/details/grcspknhh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.tarul.cn/Article/details/gckpsqtox.sHtML

[T25] Swift：结构体
来源：http://baike.epnwcf.com/Article/details/gohagwtyr.sHtML

struct P { var x: Int }
来源：http://mobile.epnwcf.com/Article/details/gehncxzhz.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fktsv.cn/Article/details/ggepyrmlj.sHtML

class A: Base { override func f() {} }
来源：http://www.share.bbcook.cn/Article/details/gwskpaqks.sHtML

[T27] Swift：错误处理
来源：http://m.share.vehdjk.com/Article/details/gplvpnesd.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.vehdjk.com/Article/details/ghanxdbns.sHtML

[T28] Swift：枚举
来源：http://read.share.yfazqb.com/Article/details/gdhzzijud.sHtML

enum Color { case red, green }
来源：http://3g.epnwcf.com/Article/details/gsxweguhi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/gvuswzjyx.sHtML

guard let x = opt else { return }
来源：http://mobile.bbcook.cn/Article/details/gykycadtm.sHtML

[T30] Swift：协议
来源：http://wap.bbcook.cn/Article/details/gdjmuczzg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.epnwcf.com/Article/details/gmewddfzo.sHtML

[T31] Lua：Hello World
来源：http://blog.epnwcf.com/Article/details/gdconbatw.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gczlgnyhh.sHtML

[T32] Lua：局部变量
来源：http://baike.fktsv.cn/Article/details/gtcizahcn.sHtML

local a = 1
来源：http://www.blog.bbcook.cn/Article/details/gkksdoagx.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/gnyszvupl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.sjlbkw.cn/Article/details/gjvrewlli.sHtML

[T34] Lua：遍历表
来源：http://read.share.yfazqb.com/Article/details/gpndrcguh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.vehdjk.com/Article/details/gspswzuww.sHtML

[T35] Lua：字典表
来源：http://blog.tarul.cn/Article/details/gcykbhsmd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.epnwcf.com/Article/details/gimicipdo.sHtML

[T36] Lua：函数
来源：http://m.share.vehdjk.com/Article/details/gmmuehtbh.sHtML

function add(a, b) return a + b end
来源：http://baike.fktsv.cn/Article/details/grizwmdld.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.bbcook.cn/Article/details/gidhjynto.sHtML

"a" .. "b"
来源：http://3g.epnwcf.com/Article/details/gdrtvshtw.sHtML

[T38] Lua：条件
来源：http://mobile.vehdjk.com/Article/details/gntpvdnnr.sHtML

if x > 0 then print("正") end
来源：http://mobile.vehdjk.com/Article/details/gegfkrggs.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/gjldnpyrs.sHtML

string.find(s, "%d+")
来源：http://blog.yfazqb.com/Article/details/gugizkqec.sHtML

[T40] Lua：元表
来源：http://mobile.sjlbkw.cn/Article/details/guchyutrs.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.yfazqb.com/Article/details/guxxxjaqr.sHtML

[T41] Perl：Hello World
来源：http://www.share.bbcook.cn/Article/details/gresnzwce.sHtML

print "Hello\n";
来源：http://www.blog.sjlbkw.cn/Article/details/gwziaquio.sHtML

[T42] Perl：变量类型
来源：http://baike.tarul.cn/Article/details/gmpvrevlc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fktsv.cn/Article/details/gbadtcjhg.sHtML

[T43] Perl：字符串插值
来源：http://blog.yfazqb.com/Article/details/ggeauchuq.sHtML

"值: $a"
来源：http://www.m.share.tarul.cn/Article/details/gtxrlizzw.sHtML

[T44] Perl：条件
来源：http://wap.epnwcf.com/Article/details/gempsznnv.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.tarul.cn/Article/details/gjkmtzldg.sHtML

[T45] Perl：数组遍历
来源：http://blog.epnwcf.com/Article/details/geahxhmqu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fktsv.cn/Article/details/gjawqejlk.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gghsihwyq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.epnwcf.com/Article/details/gmqsvrnyn.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.yfazqb.com/Article/details/gcmzwtjmf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fktsv.cn/Article/details/gqmxgoeui.sHtML

[T48] Perl：正则替换
来源：http://baike.fktsv.cn/Article/details/gqrlydexp.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fktsv.cn/Article/details/gnrshqtzm.sHtML

[T49] Perl：函数
来源：http://3g.tarul.cn/Article/details/gajkkwghz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gjvdgfntu.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gefticmwl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.vehdjk.com/Article/details/gjfejgsyq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.tarul.cn/Article/details/gevjpywiv.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/grghyypnt.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gdfmxqbbl.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/ghbrqnjcx.sHtML

val a = 1;  var b = 2
来源：http://wap.yfazqb.com/Article/details/gwryyjhvt.sHtML

[T53] Scala：字符串插值
来源：http://wap.bbcook.cn/Article/details/gxqwqgjbr.sHtML

s"值: $b"
来源：http://blog.bbcook.cn/Article/details/gtehissdo.sHtML

[T54] Scala：集合映射
来源：http://baike.sjlbkw.cn/Article/details/gmdufunaz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.epnwcf.com/Article/details/gtnqwxwgc.sHtML

[T55] Scala：集合过滤
来源：http://3g.epnwcf.com/Article/details/gjxztdgmz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.bbcook.cn/Article/details/gxbgigyez.sHtML

[T56] Scala：样例类
来源：http://3g.epnwcf.com/Article/details/ghppkwwvf.sHtML

case class User(name: String, age: Int)
来源：http://blog.vehdjk.com/Article/details/gkimwykna.sHtML

[T57] Scala：模式匹配
来源：http://m.share.tarul.cn/Article/details/gmnwpjxiu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.vehdjk.com/Article/details/gcsyjzzdg.sHtML

[T58] Scala：函数定义
来源：http://wap.bbcook.cn/Article/details/gghdvprtk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.yfazqb.com/Article/details/gdqtfptme.sHtML

[T59] Scala：循环
来源：http://www.blog.fktsv.cn/Article/details/gaimhcewf.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.vehdjk.com/Article/details/gqtvmcqlr.sHtML

[T60] Scala：折叠
来源：http://wap.fktsv.cn/Article/details/gkveivmsi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.vehdjk.com/Article/details/gtmykghbm.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvsebxubl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/gutcsqrks.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtaixcqxz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.tarul.cn/Article/details/gbzotiaez.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.bbcook.cn/Article/details/geviweivq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fktsv.cn/Article/details/gtbrhsact.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.tarul.cn/Article/details/guogbaeqg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.vehdjk.com/Article/details/gadmkkchk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.bbcook.cn/Article/details/gwtqkfydr.sHtML

[U04] Py：变量调试打印
来源：http://m.share.vehdjk.com/Article/details/ghhxxltme.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.epnwcf.com/Article/details/gzfaribld.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.tarul.cn/Article/details/ggjaeysnz.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gdozppqsu.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fktsv.cn/Article/details/gfnnnpmve.sHtML

{**a, **b}
来源：http://baike.yfazqb.com/Article/details/gvidztmbp.sHtML

[U07] Py：反转字典键值
来源：http://www.share.yfazqb.com/Article/details/gmsxrofdo.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.vehdjk.com/Article/details/gydbkwvgj.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.epnwcf.com/Article/details/guiulbbya.sHtML

[y for x in nested for y in x]
来源：http://www.blog.vehdjk.com/Article/details/gylkbggce.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.vehdjk.com/Article/details/gnwrgnkjo.sHtML

max(d, key=d.get)
来源：http://read.share.bbcook.cn/Article/details/grvcwaout.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/gtvetxhew.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.bbcook.cn/Article/details/geattwsll.sHtML

[U11] Py：生成器表达式
来源：http://baike.yfazqb.com/Article/details/gpftibjsw.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.yfazqb.com/Article/details/gygbieszb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.yfazqb.com/Article/details/gfadwfuzs.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/grtspyzwn.sHtML

[U13] Py：固定长度队列
来源：http://3g.bbcook.cn/Article/details/guqetvksr.sHtML

deque(maxlen=10)
来源：http://www.m.share.fktsv.cn/Article/details/gdxihqxgm.sHtML

[U14] Py：分组收集到列表
来源：http://blog.epnwcf.com/Article/details/geepgaygg.sHtML

defaultdict(list)
来源：http://www.blog.vehdjk.com/Article/details/gkzaopzxd.sHtML

[U15] Py：高精度计时
来源：http://wap.fktsv.cn/Article/details/gozvqjawl.sHtML

t = time.perf_counter()
来源：http://baike.yfazqb.com/Article/details/gcmtweovu.sHtML

[U16] Py：命令行参数解析
来源：http://wap.bbcook.cn/Article/details/grdlzwukx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.epnwcf.com/Article/details/gyaqcczhg.sHtML

[U17] Py：初始化日志
来源：http://baike.vehdjk.com/Article/details/glnmnmier.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.yfazqb.com/Article/details/geddyrzsj.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/gkbydwdvv.sHtML

pat = re.compile(r"\d+")
来源：http://baike.epnwcf.com/Article/details/gamqccotx.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.epnwcf.com/Article/details/gtlhcchjj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.bbcook.cn/Article/details/goadbsfye.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fktsv.cn/Article/details/gkrihgyqe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.epnwcf.com/Article/details/gpiwkuxlg.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.yfazqb.com/Article/details/gebyqlpks.sHtML

@contextlib.contextmanager
来源：http://m.share.sjlbkw.cn/Article/details/gcyqehbjm.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fktsv.cn/Article/details/gakeqtset.sHtML

list(zip(*m))
来源：http://www.share.sjlbkw.cn/Article/details/gmqbkaduu.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.bbcook.cn/Article/details/gcythktkp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.tarul.cn/Article/details/gxkbxhbii.sHtML

[U24] Py：路径操作
来源：http://www.m.share.epnwcf.com/Article/details/gfzjhilbe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gkvccsgmg.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/gvjsfniqd.sHtML

csv.DictReader(f)
来源：http://3g.sjlbkw.cn/Article/details/gdflbocyv.sHtML

[U26] Py：并发下载
来源：http://read.share.tarul.cn/Article/details/gigtdwroq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.epnwcf.com/Article/details/ggqejcyzm.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.epnwcf.com/Article/details/gviavwtnl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fktsv.cn/Article/details/ggqmttmau.sHtML

[U28] Py：类型别名
来源：http://baike.yfazqb.com/Article/details/gstqtbudr.sHtML

UserId = int
来源：http://read.share.yfazqb.com/Article/details/gaqnxpgya.sHtML

[U29] Py：属性校验
来源：http://3g.yfazqb.com/Article/details/gqqjyzlow.sHtML

@property 与 @x.setter 配合
来源：http://mobile.yfazqb.com/Article/details/gfubqleui.sHtML

[U30] Py：数据类
来源：http://3g.tarul.cn/Article/details/golxhtmze.sHtML

@dataclass(slots=True)
来源：http://m.share.sjlbkw.cn/Article/details/gfuhtnnvi.sHtML

[U31] Py：单测
来源：http://blog.fktsv.cn/Article/details/gfzcmjhgm.sHtML

python -m pytest -q
来源：http://www.share.sjlbkw.cn/Article/details/guwshpivh.sHtML

[U32] Py：代码格式化
来源：http://baike.tarul.cn/Article/details/guaglbxhs.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.vehdjk.com/Article/details/gmkskapyl.sHtML

[U33] Py：打包发布
来源：http://read.share.yfazqb.com/Article/details/grwimlbdp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.sjlbkw.cn/Article/details/ggvqijqbv.sHtML

[U34] Py：判断编码
来源：http://www.blog.yfazqb.com/Article/details/gmvjxvvlu.sHtML

chardet.detect(raw)
来源：http://wap.yfazqb.com/Article/details/gxmngnfbu.sHtML

[U35] Py：发送邮件
来源：http://wap.vehdjk.com/Article/details/ghpspkkgd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.yfazqb.com/Article/details/gzdieocdg.sHtML

[U36] Py：定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gfqejspgp.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.tarul.cn/Article/details/gxgeouama.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.epnwcf.com/Article/details/gkqxfjfsn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.sjlbkw.cn/Article/details/gbpjwmhfz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.vehdjk.com/Article/details/gungmysla.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.yfazqb.com/Article/details/gkxnlbplb.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.vehdjk.com/Article/details/gvnxbefjp.sHtML

sys.stdout.isatty()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbspzjun.sHtML

[U40] Py：打印到标准错误
来源：http://wap.yfazqb.com/Article/details/glekoscod.sHtML

print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/grjjmamms.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.vehdjk.com/Article/details/gzbyoclel.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.tarul.cn/Article/details/gtctaxfkp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.bbcook.cn/Article/details/gaeyhtfba.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.vehdjk.com/Article/details/gjvtxeudu.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.yfazqb.com/Article/details/gtyddehsm.sHtML

namespace App\Http;
来源：http://www.m.share.tarul.cn/Article/details/gxsgahcmq.sHtML

[U44] PHP：开启严格类型
来源：http://3g.epnwcf.com/Article/details/gvnrugnil.sHtML

declare(strict_types=1);
来源：http://mobile.bbcook.cn/Article/details/gmjjjalff.sHtML


<!-- 参考信息 -->