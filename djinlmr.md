代发 wailian999

x |= (1 << 3);
来源：http://www.m.share.vehdjk.com/Article/details/gzsjbwsud.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gdzwdewem.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.bbcook.cn/Article/details/gntciycpx.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/gweuuwdgp.sHtML

int main(int argc, char **argv)
来源：http://wap.tarul.cn/Article/details/gstwuzmnm.sHtML

[S19] C：快速排序
来源：http://www.share.vehdjk.com/Article/details/gkqgatbsw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gxyunjjeb.sHtML

[S20] C：二分查找
来源：http://www.m.share.tarul.cn/Article/details/gwvitwpcz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gfdcnvmhw.sHtML

[S21] C：字符类别判断
来源：http://www.share.epnwcf.com/Article/details/gserkgqzq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/gdunmeasm.sHtML

[S22] C：字符串转数字
来源：http://baike.sjlbkw.cn/Article/details/gkjhqekwv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.yfazqb.com/Article/details/gtvptlxdc.sHtML

[S23] C：随机数
来源：http://wap.sjlbkw.cn/Article/details/grgjwhavm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.vehdjk.com/Article/details/gsgfmgdqa.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/gmfqpzjjq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.tarul.cn/Article/details/gsmixreyn.sHtML

[S25] C：内存拷贝
来源：http://blog.epnwcf.com/Article/details/gevwlgfjy.sHtML

memcpy(dst, src, n);
来源：http://blog.bbcook.cn/Article/details/gljhbkkss.sHtML

[S26] C：内存清零
来源：http://m.share.epnwcf.com/Article/details/gvcdvqijj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/gvgjbldzg.sHtML

[S27] C：定义常量
来源：http://blog.sjlbkw.cn/Article/details/gfqsbobtk.sHtML

const double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gegrkrtet.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/govwrrqps.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/glwxupxti.sHtML

[S29] C：变参函数
来源：http://wap.fktsv.cn/Article/details/gyksqrhat.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/gzicotcox.sHtML

[S30] C：头文件保护
来源：http://3g.bbcook.cn/Article/details/gglpqhcyr.sHtML

#ifndef X_H
来源：http://3g.bbcook.cn/Article/details/glbvkmsyt.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gcgmwlkcv.sHtML

#endif
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmipmuxk.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/girdqivyk.sHtML

#include <iostream>
来源：http://www.blog.bbcook.cn/Article/details/glhihxfsk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/geeruwped.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/geykedsos.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/gvewsmlnq.sHtML

[S33] C++：vector 增删
来源：http://read.share.tarul.cn/Article/details/gjtxunlzb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.tarul.cn/Article/details/gjutinjex.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/galdcfbgc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.vehdjk.com/Article/details/ggyqsbofg.sHtML

[S35] C++：map
来源：http://baike.sjlbkw.cn/Article/details/gosumxjtu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gmdzondhh.sHtML

[S36] C++：unordered_map
来源：http://read.share.yfazqb.com/Article/details/gxqqfaqjj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gcnsypapv.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/guptsinaa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.vehdjk.com/Article/details/ghruphtay.sHtML

[S38] C++：排序
来源：http://read.share.sjlbkw.cn/Article/details/gpegcftnw.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.bbcook.cn/Article/details/ggtmdofch.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fktsv.cn/Article/details/grgrpyjsb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.bbcook.cn/Article/details/gkpjyvpzr.sHtML

[S40] C++：查找元素
来源：http://mobile.yfazqb.com/Article/details/gvjgzxbte.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fktsv.cn/Article/details/gthjrzrms.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/guptzdsem.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.vehdjk.com/Article/details/gzcbghtgg.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fktsv.cn/Article/details/gkyleanzq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.tarul.cn/Article/details/gnmqzfasa.sHtML

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/gvfsfxjgu.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.sjlbkw.cn/Article/details/gqwwbtagy.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/goibkcsif.sHtML

void inc(int &x) { ++x; }
来源：http://wap.sjlbkw.cn/Article/details/gkwarpzuq.sHtML

[S45] C++：lambda
来源：http://www.blog.epnwcf.com/Article/details/gmzqzarrm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gztwxnagj.sHtML

[S46] C++：函数模板
来源：http://read.share.sjlbkw.cn/Article/details/ggmgncxly.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.vehdjk.com/Article/details/grwchxksq.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.sjlbkw.cn/Article/details/gvjcbjbak.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/gvxlqbffj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/guqhuhjwj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.tarul.cn/Article/details/gtzbhwtbg.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzmrkjuh.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gwchcfska.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.epnwcf.com/Article/details/gtijlaujk.sHtML

[S50] C++：格式化数字
来源：http://wap.fktsv.cn/Article/details/gfyearmzr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.tarul.cn/Article/details/gygayscdn.sHtML

[S51] C++：显式类型转换
来源：http://m.share.yfazqb.com/Article/details/ggqkjhxzj.sHtML

static_cast<double>(a) / b
来源：http://wap.yfazqb.com/Article/details/geqmtwqfu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gvjomilxt.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/glnvvlqmx.sHtML

[S53] C++：移动语义
来源：http://wap.bbcook.cn/Article/details/gbzbngvja.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.tarul.cn/Article/details/gljvaowfk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.bbcook.cn/Article/details/gczujxtrh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.yfazqb.com/Article/details/gzvgvhkxz.sHtML

[S55] C++：结构化绑定
来源：http://3g.epnwcf.com/Article/details/gpvtryjyf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.vehdjk.com/Article/details/gxdfushow.sHtML

[S56] C++：optional
来源：http://3g.vehdjk.com/Article/details/geplhdhwu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.epnwcf.com/Article/details/gwstmovtz.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/glqiishaz.sHtML

constexpr int N = 10;
来源：http://baike.yfazqb.com/Article/details/gqkumncwq.sHtML

[S58] C++：命名空间
来源：http://m.share.bbcook.cn/Article/details/gstquumvm.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/gvnlyhqsd.sHtML

[S59] C++：静态断言
来源：http://www.blog.yfazqb.com/Article/details/gxrssyrzf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/gugkycukw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.tarul.cn/Article/details/gshogmeec.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gdwnxvzgs.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfvpwyuup.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.epnwcf.com/Article/details/gqksrrqfv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gpzcnojzj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.bbcook.cn/Article/details/gvmrdcjtz.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/gdeadstmf.sHtML

[T02] Kotlin：变量
来源：http://3g.epnwcf.com/Article/details/gtnpccwfi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.yfazqb.com/Article/details/gbtyuntqy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.bbcook.cn/Article/details/gaamzvxog.sHtML

"值: $b"
来源：http://baike.fktsv.cn/Article/details/glylifhsn.sHtML

[T04] Kotlin：空安全
来源：http://blog.bbcook.cn/Article/details/gjtjnjqhz.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.epnwcf.com/Article/details/grchuwsvo.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fktsv.cn/Article/details/goudjosqv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/gagmpxsio.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gpdtujgsq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gpxijrvhj.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.bbcook.cn/Article/details/gxnvryqfz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.bbcook.cn/Article/details/gfmcxymsc.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/gxqoocdbm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gmcsjcslu.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fktsv.cn/Article/details/gndxssiiq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.yfazqb.com/Article/details/gjgvaawzm.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.bbcook.cn/Article/details/gwdgxmbzd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.epnwcf.com/Article/details/gjrvyyttm.sHtML

[T11] Kotlin：协程
来源：http://www.share.epnwcf.com/Article/details/gpdvqmynl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.bbcook.cn/Article/details/gqocjoubh.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fktsv.cn/Article/details/glhryfjro.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.vehdjk.com/Article/details/gckojyfma.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.vehdjk.com/Article/details/gxlpccycg.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fktsv.cn/Article/details/gbgqsxvrz.sHtML

[T14] Kotlin：循环
来源：http://3g.yfazqb.com/Article/details/gndnzinex.sHtML

for (i in 1..10) println(i)
来源：http://baike.tarul.cn/Article/details/ghrmhlxzz.sHtML

[T15] Kotlin：接口
来源：http://blog.epnwcf.com/Article/details/gnulyhtpe.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.epnwcf.com/Article/details/gwhqrioif.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/gijqsymyf.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gzcezfcqs.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.bbcook.cn/Article/details/gtxpimukt.sHtML

var a = 1;  let b = 2
来源：http://wap.vehdjk.com/Article/details/guomdxegl.sHtML

[T18] Swift：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gsdoosarx.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/glmgkkbgl.sHtML

[T19] Swift：可选绑定
来源：http://baike.fktsv.cn/Article/details/gqfvqawmo.sHtML

if let n = opt { print(n) }
来源：http://read.share.yfazqb.com/Article/details/grxxkhizy.sHtML

[T20] Swift：数组操作
来源：http://mobile.tarul.cn/Article/details/gvkupxera.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fktsv.cn/Article/details/gylkaxetz.sHtML

[T21] Swift：遍历
来源：http://3g.sjlbkw.cn/Article/details/gxioezlur.sHtML

for x in a { print(x) }
来源：http://www.share.bbcook.cn/Article/details/gwidbgmlu.sHtML

[T22] Swift：字典
来源：http://www.share.bbcook.cn/Article/details/ggixkuahk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.bbcook.cn/Article/details/gyqeltwqw.sHtML

[T23] Swift：函数
来源：http://blog.bbcook.cn/Article/details/gebsklcbs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.epnwcf.com/Article/details/goeksljsb.sHtML

[T24] Swift：闭包
来源：http://www.share.sjlbkw.cn/Article/details/gebhwjmdn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gisxvfgrq.sHtML

[T25] Swift：结构体
来源：http://mobile.epnwcf.com/Article/details/gtxzblkia.sHtML

struct P { var x: Int }
来源：http://www.blog.bbcook.cn/Article/details/gaupqbhfg.sHtML

[T26] Swift：类与重写
来源：http://www.blog.tarul.cn/Article/details/gyteuevaw.sHtML

class A: Base { override func f() {} }
来源：http://www.share.epnwcf.com/Article/details/ggyghgtyp.sHtML

[T27] Swift：错误处理
来源：http://3g.tarul.cn/Article/details/gikxsrsjv.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fktsv.cn/Article/details/gedftkdux.sHtML

[T28] Swift：枚举
来源：http://read.share.bbcook.cn/Article/details/gsnlnmofx.sHtML

enum Color { case red, green }
来源：http://baike.tarul.cn/Article/details/golrzbnno.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.sjlbkw.cn/Article/details/ghdajqmcp.sHtML

guard let x = opt else { return }
来源：http://mobile.tarul.cn/Article/details/gyzxnsdxo.sHtML

[T30] Swift：协议
来源：http://wap.vehdjk.com/Article/details/gqcwpjvnr.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fktsv.cn/Article/details/gdqtudysf.sHtML

[T31] Lua：Hello World
来源：http://blog.bbcook.cn/Article/details/gvyaprzap.sHtML

print("Hello")
来源：http://blog.tarul.cn/Article/details/gwlgaulvx.sHtML

[T32] Lua：局部变量
来源：http://www.share.tarul.cn/Article/details/gknsueohq.sHtML

local a = 1
来源：http://m.share.bbcook.cn/Article/details/groxcpblc.sHtML

[T33] Lua：表（数组）
来源：http://3g.fktsv.cn/Article/details/gtunezkbl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.vehdjk.com/Article/details/gtejbjpmj.sHtML

[T34] Lua：遍历表
来源：http://baike.bbcook.cn/Article/details/gxoqqtbmm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.bbcook.cn/Article/details/gcpoubmcr.sHtML

[T35] Lua：字典表
来源：http://mobile.yfazqb.com/Article/details/grvdfvbwk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gsncsdgot.sHtML

[T36] Lua：函数
来源：http://read.share.yfazqb.com/Article/details/gugglolsu.sHtML

function add(a, b) return a + b end
来源：http://blog.vehdjk.com/Article/details/gmommnlyh.sHtML

[T37] Lua：字符串拼接
来源：http://baike.tarul.cn/Article/details/grffguvgp.sHtML

"a" .. "b"
来源：http://wap.bbcook.cn/Article/details/gwbaxxizv.sHtML

[T38] Lua：条件
来源：http://read.share.sjlbkw.cn/Article/details/gntsmkydd.sHtML

if x > 0 then print("正") end
来源：http://wap.tarul.cn/Article/details/gryhzhpup.sHtML

[T39] Lua：模式匹配
来源：http://3g.epnwcf.com/Article/details/gfvmuwtji.sHtML

string.find(s, "%d+")
来源：http://www.blog.vehdjk.com/Article/details/gqwqtpljn.sHtML

[T40] Lua：元表
来源：http://www.m.share.bbcook.cn/Article/details/gewoahbon.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fktsv.cn/Article/details/gfjxwmhzk.sHtML

[T41] Perl：Hello World
来源：http://3g.yfazqb.com/Article/details/guntvhdby.sHtML

print "Hello\n";
来源：http://blog.fktsv.cn/Article/details/gtwofoeom.sHtML

[T42] Perl：变量类型
来源：http://blog.tarul.cn/Article/details/gmigczcun.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.yfazqb.com/Article/details/gcsawmwfq.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/glcokhwht.sHtML

"值: $a"
来源：http://3g.bbcook.cn/Article/details/gjpusjspz.sHtML

[T44] Perl：条件
来源：http://www.m.share.yfazqb.com/Article/details/gohpubllg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.bbcook.cn/Article/details/gnfkjdtoi.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fktsv.cn/Article/details/gglarilsh.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.bbcook.cn/Article/details/gkvgvmuep.sHtML

[T46] Perl：哈希操作
来源：http://mobile.vehdjk.com/Article/details/ghyebxekw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fktsv.cn/Article/details/gbmznkqne.sHtML

[T47] Perl：正则捕获
来源：http://mobile.epnwcf.com/Article/details/gzwabtsyx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.epnwcf.com/Article/details/ghpugidnl.sHtML

[T48] Perl：正则替换
来源：http://mobile.fktsv.cn/Article/details/gavjirqvz.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.bbcook.cn/Article/details/gfhzsarno.sHtML

[T49] Perl：函数
来源：http://wap.bbcook.cn/Article/details/gswjrpnsq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gsksfkggr.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gatylxwvt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.tarul.cn/Article/details/gstnichqr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.epnwcf.com/Article/details/ggasshnem.sHtML

[T51] Scala：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gvywqntia.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/grumjepnq.sHtML

[T52] Scala：变量
来源：http://www.share.yfazqb.com/Article/details/ghapceuvn.sHtML

val a = 1;  var b = 2
来源：http://m.share.epnwcf.com/Article/details/gesvcvxrt.sHtML

[T53] Scala：字符串插值
来源：http://m.share.tarul.cn/Article/details/geuoipcxg.sHtML

s"值: $b"
来源：http://wap.epnwcf.com/Article/details/gjjcdcmbr.sHtML

[T54] Scala：集合映射
来源：http://read.share.epnwcf.com/Article/details/ggoioltez.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fktsv.cn/Article/details/gkzldfkmw.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gzentzpnz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gafshdnib.sHtML

[T56] Scala：样例类
来源：http://mobile.tarul.cn/Article/details/gmdqdvwxj.sHtML

case class User(name: String, age: Int)
来源：http://3g.sjlbkw.cn/Article/details/gdqxsvsvj.sHtML

[T57] Scala：模式匹配
来源：http://mobile.epnwcf.com/Article/details/gecekinkl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.tarul.cn/Article/details/gjaovmugi.sHtML

[T58] Scala：函数定义
来源：http://mobile.epnwcf.com/Article/details/gzhwylere.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fktsv.cn/Article/details/ggohuyhcr.sHtML

[T59] Scala：循环
来源：http://www.share.fktsv.cn/Article/details/gwvhwvhjx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/grrlvgjxu.sHtML

[T60] Scala：折叠
来源：http://www.m.share.bbcook.cn/Article/details/gvnasfbyo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.epnwcf.com/Article/details/gdwiqokgg.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gwawakzlc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.sjlbkw.cn/Article/details/gxcfnafjf.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gduwdcuji.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.tarul.cn/Article/details/gicpexsal.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/gshjdcdzb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.sjlbkw.cn/Article/details/gdfifdvit.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.yfazqb.com/Article/details/grznqyror.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/guqskbiww.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.tarul.cn/Article/details/ggxugvapq.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/gpgfbropj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.yfazqb.com/Article/details/ghjnapbut.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fktsv.cn/Article/details/gzrkhywxq.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gxyazcezn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.sjlbkw.cn/Article/details/gkduehaex.sHtML

{**a, **b}
来源：http://baike.bbcook.cn/Article/details/gvjqbrxaj.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.bbcook.cn/Article/details/gdsauchoq.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.vehdjk.com/Article/details/ghijimgpf.sHtML

[U08] Py：展平二维列表
来源：http://m.share.bbcook.cn/Article/details/gxvpspfcu.sHtML

[y for x in nested for y in x]
来源：http://www.share.tarul.cn/Article/details/grfcymnxt.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.bbcook.cn/Article/details/gfpdvkcrv.sHtML

max(d, key=d.get)
来源：http://wap.sjlbkw.cn/Article/details/gxnerjevm.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.vehdjk.com/Article/details/grwhzesak.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.sjlbkw.cn/Article/details/guogoivkc.sHtML

[U11] Py：生成器表达式
来源：http://www.share.sjlbkw.cn/Article/details/gwxzptyhl.sHtML

(x * 2 for x in arr)
来源：http://mobile.bbcook.cn/Article/details/ggvsvblfg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.epnwcf.com/Article/details/gqqpbcwgi.sHtML

Counter(arr).most_common(3)
来源：http://www.share.vehdjk.com/Article/details/gfaplkpkq.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.yfazqb.com/Article/details/gbuwhqdjh.sHtML

deque(maxlen=10)
来源：http://www.share.tarul.cn/Article/details/gphyujfca.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.tarul.cn/Article/details/gsrydxoin.sHtML

defaultdict(list)
来源：http://baike.bbcook.cn/Article/details/gcifodyjs.sHtML

[U15] Py：高精度计时
来源：http://www.share.tarul.cn/Article/details/gvcifkvfe.sHtML

t = time.perf_counter()
来源：http://m.share.sjlbkw.cn/Article/details/gpkyrchqm.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.sjlbkw.cn/Article/details/ghhvzsjdn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.epnwcf.com/Article/details/gdfgalrua.sHtML

[U17] Py：初始化日志
来源：http://www.share.epnwcf.com/Article/details/galjbxtxt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.sjlbkw.cn/Article/details/gramrkgol.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fktsv.cn/Article/details/gsejauhqv.sHtML

pat = re.compile(r"\d+")
来源：http://blog.tarul.cn/Article/details/gcjjqboqh.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.epnwcf.com/Article/details/gfytzzepl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.epnwcf.com/Article/details/gccslddmz.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/gvllqxevt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.tarul.cn/Article/details/gfbppoqqb.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.yfazqb.com/Article/details/gqxtcqqfp.sHtML

@contextlib.contextmanager
来源：http://3g.tarul.cn/Article/details/gflouuafi.sHtML

[U22] Py：矩阵转置
来源：http://baike.fktsv.cn/Article/details/gyowblozp.sHtML

list(zip(*m))
来源：http://wap.epnwcf.com/Article/details/grytaniln.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gflvqwyzg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.sjlbkw.cn/Article/details/gioqvwwun.sHtML

[U24] Py：路径操作
来源：http://www.share.fktsv.cn/Article/details/gcydfxogp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gqrglkhfu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.bbcook.cn/Article/details/gelzjunsj.sHtML

csv.DictReader(f)
来源：http://m.share.sjlbkw.cn/Article/details/gnznhadsr.sHtML

[U26] Py：并发下载
来源：http://www.blog.vehdjk.com/Article/details/gekakzdsk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.yfazqb.com/Article/details/gbtfkezqs.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvxlmane.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.bbcook.cn/Article/details/gtaqrbmgs.sHtML

[U28] Py：类型别名
来源：http://3g.tarul.cn/Article/details/gqujbotvh.sHtML

UserId = int
来源：http://wap.fktsv.cn/Article/details/gxwktfgin.sHtML

[U29] Py：属性校验
来源：http://mobile.bbcook.cn/Article/details/gbvjqbrhu.sHtML

@property 与 @x.setter 配合
来源：http://m.share.bbcook.cn/Article/details/gruaystlf.sHtML

[U30] Py：数据类
来源：http://mobile.fktsv.cn/Article/details/gkhckrghs.sHtML

@dataclass(slots=True)
来源：http://www.blog.fktsv.cn/Article/details/gjycvpvji.sHtML

[U31] Py：单测
来源：http://www.m.share.yfazqb.com/Article/details/gvmxylyrc.sHtML

python -m pytest -q
来源：http://mobile.yfazqb.com/Article/details/gzejcfnuf.sHtML

[U32] Py：代码格式化
来源：http://www.blog.tarul.cn/Article/details/gdnfhjdtd.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.yfazqb.com/Article/details/gyvoufver.sHtML

[U33] Py：打包发布
来源：http://wap.vehdjk.com/Article/details/gxaaukefd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.epnwcf.com/Article/details/gohntbxtc.sHtML

[U34] Py：判断编码
来源：http://read.share.fktsv.cn/Article/details/gzyddwslk.sHtML

chardet.detect(raw)
来源：http://mobile.bbcook.cn/Article/details/gimpwgqkk.sHtML

[U35] Py：发送邮件
来源：http://wap.yfazqb.com/Article/details/gdzugovwg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.bbcook.cn/Article/details/gvjcqfvex.sHtML

[U36] Py：定时任务
来源：http://read.share.fktsv.cn/Article/details/gomqkedhk.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.sjlbkw.cn/Article/details/gkspiduhx.sHtML

[U37] Py：读写 Excel
来源：http://mobile.tarul.cn/Article/details/gkisvrgre.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.bbcook.cn/Article/details/gqgjdfsvc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.tarul.cn/Article/details/gakeoukgz.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.tarul.cn/Article/details/garcrsfop.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.vehdjk.com/Article/details/gesgyfyqs.sHtML

sys.stdout.isatty()
来源：http://mobile.sjlbkw.cn/Article/details/gftcplmgh.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.bbcook.cn/Article/details/gytlkgytm.sHtML

print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/geqeafldz.sHtML


<!-- 参考信息 -->