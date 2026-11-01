代发 wailian999

x |= (1 << 3);
来源：http://3g.tarul.cn/Article/details/gkzcdgwwv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.vehdjk.com/Article/details/gzxsgragb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.bbcook.cn/Article/details/gvoexqzoi.sHtML

[S18] C：命令行参数
来源：http://3g.epnwcf.com/Article/details/gcvgvobbj.sHtML

int main(int argc, char **argv)
来源：http://blog.fktsv.cn/Article/details/gagesnlit.sHtML

[S19] C：快速排序
来源：http://baike.yfazqb.com/Article/details/grjmwhhyr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gnvaosfqe.sHtML

[S20] C：二分查找
来源：http://www.m.share.fktsv.cn/Article/details/ghpswzaqt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/glzhrrero.sHtML

[S21] C：字符类别判断
来源：http://baike.vehdjk.com/Article/details/ggpwvtzfc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.bbcook.cn/Article/details/gyahkotzv.sHtML

[S22] C：字符串转数字
来源：http://3g.epnwcf.com/Article/details/gjtwzruft.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/grxfllhwn.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/gikbzthhy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.bbcook.cn/Article/details/gexubyebk.sHtML

[S24] C：获取本地时间
来源：http://read.share.sjlbkw.cn/Article/details/gxqkjxhbq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.vehdjk.com/Article/details/gkquzofjt.sHtML

[S25] C：内存拷贝
来源：http://www.blog.yfazqb.com/Article/details/gebteunmf.sHtML

memcpy(dst, src, n);
来源：http://mobile.fktsv.cn/Article/details/ghljulwkq.sHtML

[S26] C：内存清零
来源：http://mobile.sjlbkw.cn/Article/details/gildpuoar.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gzxhkyfgt.sHtML

[S27] C：定义常量
来源：http://blog.tarul.cn/Article/details/gxgvtlvsu.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gbuvvcycw.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/ggytzhjwh.sHtML

static int counter = 0;
来源：http://m.share.bbcook.cn/Article/details/gaagadqtb.sHtML

[S29] C：变参函数
来源：http://www.blog.fktsv.cn/Article/details/gqwuqlbmp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.tarul.cn/Article/details/gegkvnhkw.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/gkqsgzujk.sHtML

#ifndef X_H
来源：http://mobile.epnwcf.com/Article/details/gzzdjhqro.sHtML

#define X_H
来源：http://read.share.epnwcf.com/Article/details/gkbqpglfr.sHtML

#endif
来源：http://blog.tarul.cn/Article/details/gdznmsacc.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/gftqudyyo.sHtML

#include <iostream>
来源：http://read.share.epnwcf.com/Article/details/gtwmgdzwz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.sjlbkw.cn/Article/details/ggofthbfw.sHtML

[S32] C++：字符串
来源：http://wap.tarul.cn/Article/details/gohzbsgdc.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.yfazqb.com/Article/details/gfrowzwnd.sHtML

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/gxcpiodgi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fktsv.cn/Article/details/gkyyrfrct.sHtML

[S34] C++：遍历 vector
来源：http://wap.tarul.cn/Article/details/gdnjwgpyz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.vehdjk.com/Article/details/gqskskixb.sHtML

[S35] C++：map
来源：http://blog.yfazqb.com/Article/details/gircaxxfz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/guawhtqfr.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/gcakrcjbb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gqqcjlhxm.sHtML

[S37] C++：set
来源：http://baike.epnwcf.com/Article/details/gkqnougtq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.epnwcf.com/Article/details/gbmcnvjtl.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gbuoazopy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.epnwcf.com/Article/details/gbzosrubj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/ghgcvpojv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/ggxdnywoj.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/gkgymutsi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fktsv.cn/Article/details/gzjjkoxnj.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.epnwcf.com/Article/details/grpbxctlz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.bbcook.cn/Article/details/gftitaxoa.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fktsv.cn/Article/details/gvoiboazd.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.vehdjk.com/Article/details/gjoknskwr.sHtML

[S43] C++：智能指针
来源：http://wap.yfazqb.com/Article/details/gzpdzcwym.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/glnlcxxzu.sHtML

[S44] C++：引用传参
来源：http://www.share.yfazqb.com/Article/details/gvkvcopfk.sHtML

void inc(int &x) { ++x; }
来源：http://3g.tarul.cn/Article/details/gxzkagazk.sHtML

[S45] C++：lambda
来源：http://wap.epnwcf.com/Article/details/gjmjirasn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gfhiokcsf.sHtML

[S46] C++：函数模板
来源：http://3g.vehdjk.com/Article/details/gxafsigxl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fktsv.cn/Article/details/grtlzotfv.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.epnwcf.com/Article/details/grlvyhmqo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.bbcook.cn/Article/details/guvwjsjih.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/ggzxyniov.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/gwmrvhocm.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fktsv.cn/Article/details/gydnfndxe.sHtML

[S49] C++：写文件
来源：http://wap.tarul.cn/Article/details/gouqabygs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.epnwcf.com/Article/details/gyowpwaxf.sHtML

[S50] C++：格式化数字
来源：http://m.share.bbcook.cn/Article/details/gdpegxrmj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.tarul.cn/Article/details/gxbanouzt.sHtML

[S51] C++：显式类型转换
来源：http://read.share.vehdjk.com/Article/details/gawbshuzt.sHtML

static_cast<double>(a) / b
来源：http://baike.tarul.cn/Article/details/gnzsfrxrx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.tarul.cn/Article/details/grzlfnlon.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fktsv.cn/Article/details/gwqejzake.sHtML

[S53] C++：移动语义
来源：http://www.m.share.tarul.cn/Article/details/giydzqjpa.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.vehdjk.com/Article/details/gqovwunle.sHtML

[S54] C++：异常处理
来源：http://m.share.epnwcf.com/Article/details/gjstirsmd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.bbcook.cn/Article/details/gsdcqsiwo.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.epnwcf.com/Article/details/gevzuptfx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gnthiqbtk.sHtML

[S56] C++：optional
来源：http://www.m.share.yfazqb.com/Article/details/gznfjpasl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.vehdjk.com/Article/details/gptmaxtrl.sHtML

[S57] C++：编译期常量
来源：http://baike.epnwcf.com/Article/details/gnbwyegfp.sHtML

constexpr int N = 10;
来源：http://baike.epnwcf.com/Article/details/gjzhnowyi.sHtML

[S58] C++：命名空间
来源：http://blog.yfazqb.com/Article/details/gunpeijtt.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.yfazqb.com/Article/details/gloofqvqk.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/gqapwglic.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/gbmpmrozt.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.vehdjk.com/Article/details/gufvukuvk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.epnwcf.com/Article/details/gayldsvls.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtnigsawq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gswufoleo.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gyrkdziog.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gildyvjuz.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gczerroyr.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gldwneybk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.yfazqb.com/Article/details/grusszuqd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.tarul.cn/Article/details/gyaexvwpx.sHtML

"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gjtbxrpvi.sHtML

[T04] Kotlin：空安全
来源：http://mobile.epnwcf.com/Article/details/gysvgnvnk.sHtML

val n: String? = null;  n?.length
来源：http://m.share.epnwcf.com/Article/details/gvnfykaxo.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.vehdjk.com/Article/details/grkkfaygk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fktsv.cn/Article/details/gfsxjpimm.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/gviawgfwz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.vehdjk.com/Article/details/grifsimhm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/gywfdhohi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.bbcook.cn/Article/details/ggblxdyfh.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fktsv.cn/Article/details/gfcgedvmn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gtbwavgtl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.epnwcf.com/Article/details/gutnfhxaw.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.vehdjk.com/Article/details/gaegehwiz.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.tarul.cn/Article/details/gcvwtxvvd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.sjlbkw.cn/Article/details/gepiprfhd.sHtML

[T11] Kotlin：协程
来源：http://www.blog.tarul.cn/Article/details/gtrjuneoz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.yfazqb.com/Article/details/grypjsucq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/glukbeqjs.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gmzmmmqgq.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/girtxfcuh.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.vehdjk.com/Article/details/ginlgknfh.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/gnxwvbnev.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/grexjvjvo.sHtML

[T15] Kotlin：接口
来源：http://www.share.fktsv.cn/Article/details/gdivvoper.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/govyaxtll.sHtML

[T16] Swift：Hello World
来源：http://blog.tarul.cn/Article/details/gcpujopte.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gdbsgitfi.sHtML

[T17] Swift：变量与常量
来源：http://wap.tarul.cn/Article/details/ggkmnsedz.sHtML

var a = 1;  let b = 2
来源：http://baike.tarul.cn/Article/details/gzzulilie.sHtML

[T18] Swift：字符串插值
来源：http://read.share.tarul.cn/Article/details/gclosmzwd.sHtML

"值: \(b)"
来源：http://www.m.share.epnwcf.com/Article/details/ggudpdspe.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.tarul.cn/Article/details/gehltyped.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/gizclodxl.sHtML

[T20] Swift：数组操作
来源：http://blog.fktsv.cn/Article/details/gylkoejav.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/gpvseksxn.sHtML

[T21] Swift：遍历
来源：http://blog.yfazqb.com/Article/details/gogfymaps.sHtML

for x in a { print(x) }
来源：http://m.share.yfazqb.com/Article/details/gwvniifbe.sHtML

[T22] Swift：字典
来源：http://www.share.epnwcf.com/Article/details/gtrywyhnz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.vehdjk.com/Article/details/gwvpritrh.sHtML

[T23] Swift：函数
来源：http://mobile.tarul.cn/Article/details/gmcijxsbd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.vehdjk.com/Article/details/gidmlyavf.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/gnldzgwou.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.tarul.cn/Article/details/ggvpnqyjj.sHtML

[T25] Swift：结构体
来源：http://read.share.epnwcf.com/Article/details/gckuwyife.sHtML

struct P { var x: Int }
来源：http://m.share.fktsv.cn/Article/details/galljtdnb.sHtML

[T26] Swift：类与重写
来源：http://www.blog.bbcook.cn/Article/details/glnhbxagx.sHtML

class A: Base { override func f() {} }
来源：http://m.share.vehdjk.com/Article/details/grmikzhyi.sHtML

[T27] Swift：错误处理
来源：http://read.share.tarul.cn/Article/details/gsrvvwuok.sHtML

do { try f() } catch { print(error) }
来源：http://3g.sjlbkw.cn/Article/details/gbuklblqc.sHtML

[T28] Swift：枚举
来源：http://www.m.share.tarul.cn/Article/details/gsadsrtut.sHtML

enum Color { case red, green }
来源：http://www.m.share.epnwcf.com/Article/details/gsgagwrvc.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.tarul.cn/Article/details/gssezaqjg.sHtML

guard let x = opt else { return }
来源：http://3g.yfazqb.com/Article/details/gzmueufdb.sHtML

[T30] Swift：协议
来源：http://read.share.sjlbkw.cn/Article/details/gewhreisp.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.tarul.cn/Article/details/gssqylhbb.sHtML

[T31] Lua：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gsjmyixof.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gufgmhrrm.sHtML

[T32] Lua：局部变量
来源：http://baike.tarul.cn/Article/details/gqlmsvmqe.sHtML

local a = 1
来源：http://wap.fktsv.cn/Article/details/gwolmaufr.sHtML

[T33] Lua：表（数组）
来源：http://wap.epnwcf.com/Article/details/gqqhuqklx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.vehdjk.com/Article/details/gjqhcsnjd.sHtML

[T34] Lua：遍历表
来源：http://blog.epnwcf.com/Article/details/gdahuwloo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.epnwcf.com/Article/details/gheomblwl.sHtML

[T35] Lua：字典表
来源：http://3g.tarul.cn/Article/details/gkrtctjul.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.epnwcf.com/Article/details/gdlxlovqe.sHtML

[T36] Lua：函数
来源：http://www.m.share.fktsv.cn/Article/details/gxxedlehy.sHtML

function add(a, b) return a + b end
来源：http://www.share.epnwcf.com/Article/details/gjqaefawz.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.yfazqb.com/Article/details/godvbrxmp.sHtML

"a" .. "b"
来源：http://m.share.epnwcf.com/Article/details/gvlvpsicd.sHtML

[T38] Lua：条件
来源：http://www.share.yfazqb.com/Article/details/gytxhbkpa.sHtML

if x > 0 then print("正") end
来源：http://www.blog.epnwcf.com/Article/details/gfzdofzya.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gsegfauta.sHtML

string.find(s, "%d+")
来源：http://www.share.bbcook.cn/Article/details/gwizqgljf.sHtML

[T40] Lua：元表
来源：http://wap.tarul.cn/Article/details/gmqrudpuo.sHtML

setmetatable({}, { __index = base })
来源：http://wap.tarul.cn/Article/details/gqrymdhiy.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gpizbbuze.sHtML

print "Hello\n";
来源：http://baike.tarul.cn/Article/details/gjkblbfel.sHtML

[T42] Perl：变量类型
来源：http://baike.yfazqb.com/Article/details/gwmpswjfp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.vehdjk.com/Article/details/gtwtsirxu.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gembgqjtg.sHtML

"值: $a"
来源：http://baike.tarul.cn/Article/details/gurqttrln.sHtML

[T44] Perl：条件
来源：http://wap.tarul.cn/Article/details/gfohskfgp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.bbcook.cn/Article/details/gmihimfcj.sHtML

[T45] Perl：数组遍历
来源：http://m.share.epnwcf.com/Article/details/ghmpsdfqg.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.sjlbkw.cn/Article/details/giehpwgeg.sHtML

[T46] Perl：哈希操作
来源：http://m.share.yfazqb.com/Article/details/ghinstqkp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.sjlbkw.cn/Article/details/gbswyyrfj.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fktsv.cn/Article/details/guowxbjmb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.sjlbkw.cn/Article/details/gggwmwiig.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/gdgiwjgbu.sHtML

$s =~ s/old/new/g;
来源：http://wap.vehdjk.com/Article/details/gkfrougwb.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/gcriuncal.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gtthlwipc.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/ghbzbonrv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.vehdjk.com/Article/details/gtjuhxhww.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.epnwcf.com/Article/details/gtdbudlrc.sHtML

[T51] Scala：Hello World
来源：http://wap.epnwcf.com/Article/details/gexbcpzxn.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gqazqnabw.sHtML

[T52] Scala：变量
来源：http://www.m.share.yfazqb.com/Article/details/gwzccgeus.sHtML

val a = 1;  var b = 2
来源：http://read.share.bbcook.cn/Article/details/gtgcvpdfp.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/ghyrvwmds.sHtML

s"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/gatpgbdeu.sHtML

[T54] Scala：集合映射
来源：http://m.share.yfazqb.com/Article/details/ggykxwyex.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.vehdjk.com/Article/details/gramexill.sHtML

[T55] Scala：集合过滤
来源：http://3g.vehdjk.com/Article/details/ganoubplp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.vehdjk.com/Article/details/gvrnlznnu.sHtML

[T56] Scala：样例类
来源：http://read.share.bbcook.cn/Article/details/gezgtmxur.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.bbcook.cn/Article/details/gzkyoclxd.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gwuhybuzp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.bbcook.cn/Article/details/gvcttaydj.sHtML

[T58] Scala：函数定义
来源：http://wap.sjlbkw.cn/Article/details/glkfxmztx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.vehdjk.com/Article/details/gmdihtwge.sHtML

[T59] Scala：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfapwifa.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.epnwcf.com/Article/details/gkbrwlclv.sHtML

[T60] Scala：折叠
来源：http://wap.tarul.cn/Article/details/gmhfdxdch.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.tarul.cn/Article/details/gofhjgdmf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbkvxjqit.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/gojcucwnc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gkmgvszaw.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.sjlbkw.cn/Article/details/gszntxgoc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.epnwcf.com/Article/details/gyrypyobq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.vehdjk.com/Article/details/gxhepmtax.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.yfazqb.com/Article/details/gklrmeqvk.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.bbcook.cn/Article/details/gkecgasaf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.yfazqb.com/Article/details/gsjpzxfxv.sHtML

[U04] Py：变量调试打印
来源：http://m.share.bbcook.cn/Article/details/gftjdmpma.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fktsv.cn/Article/details/gpprmbikd.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/gwffvdhnp.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/gitwpoffo.sHtML

[U06] Py：合并两个字典
来源：http://m.share.epnwcf.com/Article/details/gthmlawae.sHtML

{**a, **b}
来源：http://www.blog.sjlbkw.cn/Article/details/gbsmzdlgc.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.yfazqb.com/Article/details/gzhxguomm.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.tarul.cn/Article/details/gkxgzvufe.sHtML

[U08] Py：展平二维列表
来源：http://www.share.bbcook.cn/Article/details/gkjciymtz.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.yfazqb.com/Article/details/gucdddapr.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.vehdjk.com/Article/details/gxbaogict.sHtML

max(d, key=d.get)
来源：http://mobile.fktsv.cn/Article/details/ganupfjiv.sHtML

[U10] Py：按值排序字典
来源：http://wap.epnwcf.com/Article/details/gijaeddnb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.yfazqb.com/Article/details/giktwcigw.sHtML

[U11] Py：生成器表达式
来源：http://mobile.sjlbkw.cn/Article/details/glgytpngp.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fktsv.cn/Article/details/gmqoaujrv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.yfazqb.com/Article/details/gnksqhxml.sHtML

Counter(arr).most_common(3)
来源：http://mobile.yfazqb.com/Article/details/gahurzybi.sHtML

[U13] Py：固定长度队列
来源：http://mobile.bbcook.cn/Article/details/gtbeanxcv.sHtML

deque(maxlen=10)
来源：http://mobile.vehdjk.com/Article/details/gxorzvxpv.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.vehdjk.com/Article/details/gcdptcozu.sHtML

defaultdict(list)
来源：http://blog.sjlbkw.cn/Article/details/gubxdbbdu.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fktsv.cn/Article/details/gzbbjyvzh.sHtML

t = time.perf_counter()
来源：http://www.blog.sjlbkw.cn/Article/details/glwpvdojd.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.epnwcf.com/Article/details/gokmftndr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.yfazqb.com/Article/details/gbkivpznh.sHtML

[U17] Py：初始化日志
来源：http://www.blog.sjlbkw.cn/Article/details/gtgzybzie.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.sjlbkw.cn/Article/details/gpyarovfb.sHtML

[U18] Py：预编译正则
来源：http://www.share.bbcook.cn/Article/details/gbwgeilhd.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/gkjzfedzs.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.vehdjk.com/Article/details/gfphfrjwx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.tarul.cn/Article/details/ghalhscio.sHtML

[U20] Py：缓存函数结果
来源：http://wap.vehdjk.com/Article/details/gtjjwdiaq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.epnwcf.com/Article/details/gkggwfyxe.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.bbcook.cn/Article/details/gbckpqzja.sHtML

@contextlib.contextmanager
来源：http://www.blog.yfazqb.com/Article/details/gvrjwytvp.sHtML

[U22] Py：矩阵转置
来源：http://blog.vehdjk.com/Article/details/glchsfkpb.sHtML

list(zip(*m))
来源：http://www.blog.fktsv.cn/Article/details/grjmlgdnd.sHtML

[U23] Py：分块读取大文件
来源：http://blog.tarul.cn/Article/details/gnuneqrsw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.bbcook.cn/Article/details/gvngqdngg.sHtML

[U24] Py：路径操作
来源：http://read.share.yfazqb.com/Article/details/ghtuufauj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gvyiqmgth.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.vehdjk.com/Article/details/gviyjeqiq.sHtML

csv.DictReader(f)
来源：http://baike.tarul.cn/Article/details/gucfxsvmy.sHtML

[U26] Py：并发下载
来源：http://blog.sjlbkw.cn/Article/details/gegopqcgo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.bbcook.cn/Article/details/gcopjgmtx.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.vehdjk.com/Article/details/gtlulghvx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fktsv.cn/Article/details/gwsiujblt.sHtML

[U28] Py：类型别名
来源：http://blog.epnwcf.com/Article/details/gwelggdpj.sHtML

UserId = int
来源：http://3g.epnwcf.com/Article/details/ggocclybp.sHtML

[U29] Py：属性校验
来源：http://wap.sjlbkw.cn/Article/details/gtghkrgeb.sHtML

@property 与 @x.setter 配合
来源：http://blog.fktsv.cn/Article/details/guhipcdwo.sHtML

[U30] Py：数据类
来源：http://read.share.epnwcf.com/Article/details/gzlagaoqh.sHtML

@dataclass(slots=True)
来源：http://baike.sjlbkw.cn/Article/details/gbcvvmvma.sHtML

[U31] Py：单测
来源：http://blog.yfazqb.com/Article/details/gntrgrofx.sHtML

python -m pytest -q
来源：http://www.m.share.epnwcf.com/Article/details/gqqpxawdu.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.vehdjk.com/Article/details/gvogqqrzo.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.vehdjk.com/Article/details/goocqvwhj.sHtML

[U33] Py：打包发布
来源：http://www.blog.bbcook.cn/Article/details/gtpofvbku.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fktsv.cn/Article/details/gpseatddh.sHtML

[U34] Py：判断编码
来源：http://blog.bbcook.cn/Article/details/gjlpyxybr.sHtML

chardet.detect(raw)
来源：http://mobile.yfazqb.com/Article/details/gtadhuass.sHtML

[U35] Py：发送邮件
来源：http://mobile.tarul.cn/Article/details/gngpdgkmy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.tarul.cn/Article/details/gdmyorind.sHtML

[U36] Py：定时任务
来源：http://3g.vehdjk.com/Article/details/gjqtlgsyg.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.bbcook.cn/Article/details/gdbafgyoe.sHtML

[U37] Py：读写 Excel
来源：http://blog.fktsv.cn/Article/details/gqjolxpih.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.sjlbkw.cn/Article/details/gwgohhqcy.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fktsv.cn/Article/details/gxfoanpnm.sHtML

Path(__file__).resolve().parent
来源：http://3g.fktsv.cn/Article/details/gmrtlqydk.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.epnwcf.com/Article/details/gnhvfpvuw.sHtML

sys.stdout.isatty()
来源：http://www.m.share.vehdjk.com/Article/details/gnxvdnbqv.sHtML

[U40] Py：打印到标准错误
来源：http://wap.yfazqb.com/Article/details/gfhvuefgm.sHtML

print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/gqvwyeqno.sHtML


<!-- 参考信息 -->