代发 wailian999

int main(int argc, char **argv)
来源：http://baike.sjlbkw.cn/Article/details/gsasllkdi.sHtML

[S19] C：快速排序
来源：http://www.blog.vehdjk.com/Article/details/gzjzrwwbi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gojlikzqh.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/gdwreblsz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gsfmggmod.sHtML

[S21] C：字符类别判断
来源：http://3g.sjlbkw.cn/Article/details/grnaiwdby.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/gvyjkmgcm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.tarul.cn/Article/details/gtiugpasb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.vehdjk.com/Article/details/gyagmlogh.sHtML

[S23] C：随机数
来源：http://baike.tarul.cn/Article/details/gscucjweb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.tarul.cn/Article/details/gnnpbdokf.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/gxkldsfgh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/gzabjkovu.sHtML

[S25] C：内存拷贝
来源：http://read.share.epnwcf.com/Article/details/gyixzhyjs.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.sjlbkw.cn/Article/details/gordyiynt.sHtML

[S26] C：内存清零
来源：http://blog.yfazqb.com/Article/details/grpgzwrdb.sHtML

memset(a, 0, sizeof a);
来源：http://wap.epnwcf.com/Article/details/gjapzlkkz.sHtML

[S27] C：定义常量
来源：http://www.blog.yfazqb.com/Article/details/gcdootmpo.sHtML

const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gnrhnfhha.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/gcpeiudiw.sHtML

static int counter = 0;
来源：http://www.blog.vehdjk.com/Article/details/gprazyyph.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/gsgujnfas.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.epnwcf.com/Article/details/ghnozkqfn.sHtML

[S30] C：头文件保护
来源：http://wap.tarul.cn/Article/details/gyjpjcbkr.sHtML

#ifndef X_H
来源：http://wap.vehdjk.com/Article/details/gpudctxnj.sHtML

#define X_H
来源：http://www.blog.sjlbkw.cn/Article/details/ggwbxlwbf.sHtML

#endif
来源：http://read.share.fktsv.cn/Article/details/gmylfojsh.sHtML

[S31] C++：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gqvrvjslr.sHtML

#include <iostream>
来源：http://m.share.vehdjk.com/Article/details/grkzsillg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.vehdjk.com/Article/details/gzxcfwjjr.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gsmezcdzz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.bbcook.cn/Article/details/gherchoyq.sHtML

[S33] C++：vector 增删
来源：http://m.share.tarul.cn/Article/details/govvioojy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.bbcook.cn/Article/details/gfpkndvbv.sHtML

[S34] C++：遍历 vector
来源：http://wap.fktsv.cn/Article/details/gcekqazgk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gabzxtmbf.sHtML

[S35] C++：map
来源：http://www.share.vehdjk.com/Article/details/gdbdruium.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/ghjuwusms.sHtML

[S36] C++：unordered_map
来源：http://3g.tarul.cn/Article/details/guqfngqjb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gfrryakqh.sHtML

[S37] C++：set
来源：http://mobile.tarul.cn/Article/details/gcmrumhkh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.epnwcf.com/Article/details/gpqdibefx.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/gvnpvlrtk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/ggpeqngfc.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/gnltzqyhm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.bbcook.cn/Article/details/gdaqioabx.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/gamhuicdt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.vehdjk.com/Article/details/gmsgalohb.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/gxgfwsshj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.vehdjk.com/Article/details/gbfrmitmx.sHtML

[S42] C++：继承与虚函数
来源：http://wap.sjlbkw.cn/Article/details/ghdrxmanh.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/gvamfdsex.sHtML

[S43] C++：智能指针
来源：http://baike.epnwcf.com/Article/details/ggajyrbsp.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.sjlbkw.cn/Article/details/gunkvzmto.sHtML

[S44] C++：引用传参
来源：http://read.share.sjlbkw.cn/Article/details/gufinkgny.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fktsv.cn/Article/details/gieqemhvz.sHtML

[S45] C++：lambda
来源：http://www.share.bbcook.cn/Article/details/gkeyekdkf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.epnwcf.com/Article/details/gkdotmdfv.sHtML

[S46] C++：函数模板
来源：http://www.share.tarul.cn/Article/details/gmjyjdlda.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/gsbelzgwz.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.tarul.cn/Article/details/gcmtqjhqs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.yfazqb.com/Article/details/gczlqssay.sHtML

[S48] C++：逐行读文件
来源：http://wap.tarul.cn/Article/details/gjbxxphin.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.sjlbkw.cn/Article/details/ghsvoxrne.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gddxybsmh.sHtML

[S49] C++：写文件
来源：http://read.share.vehdjk.com/Article/details/gwgdoatlx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.bbcook.cn/Article/details/ghmqmylfj.sHtML

[S50] C++：格式化数字
来源：http://www.blog.sjlbkw.cn/Article/details/gtghjiwyb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.tarul.cn/Article/details/gbjiclaps.sHtML

[S51] C++：显式类型转换
来源：http://wap.yfazqb.com/Article/details/gfsvoqrjc.sHtML

static_cast<double>(a) / b
来源：http://wap.epnwcf.com/Article/details/gnifqpzxi.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.bbcook.cn/Article/details/gczvrkire.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fktsv.cn/Article/details/gsmgzjeqy.sHtML

[S53] C++：移动语义
来源：http://3g.fktsv.cn/Article/details/gucmxstta.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.epnwcf.com/Article/details/gyyzisgke.sHtML

[S54] C++：异常处理
来源：http://www.m.share.epnwcf.com/Article/details/grjakxdqp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.vehdjk.com/Article/details/gepcxwzti.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzybypas.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.yfazqb.com/Article/details/gnbzyxaze.sHtML

[S56] C++：optional
来源：http://m.share.yfazqb.com/Article/details/gfelvnneb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.yfazqb.com/Article/details/ghekjovkl.sHtML

[S57] C++：编译期常量
来源：http://www.blog.yfazqb.com/Article/details/gudxbslip.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gqowoyptb.sHtML

[S58] C++：命名空间
来源：http://wap.bbcook.cn/Article/details/gyymnmfzt.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/gxnhruqfq.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/gxrzcqyrl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.tarul.cn/Article/details/gcqzndrfl.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.tarul.cn/Article/details/gqmposnlu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.tarul.cn/Article/details/gyrqnjgtc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gocrryiav.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gqupspctq.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfuvbietp.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.yfazqb.com/Article/details/gaxtzajgb.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gkzhseshn.sHtML

[T02] Kotlin：变量
来源：http://www.share.fktsv.cn/Article/details/glcecarxq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/gcmriiacr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.vehdjk.com/Article/details/gofocqczk.sHtML

"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/ggkprfvmq.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fktsv.cn/Article/details/ggfybynuu.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/ghfavdpqd.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gcmgpqvxc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/gaxtlcmco.sHtML

[T06] Kotlin：集合映射
来源：http://baike.sjlbkw.cn/Article/details/gqzcxhbgt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/ghkeykahx.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.epnwcf.com/Article/details/gwkdspnir.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/gewuiofeq.sHtML

[T08] Kotlin：数据类
来源：http://m.share.epnwcf.com/Article/details/gfszcathm.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.yfazqb.com/Article/details/gmvalzqcn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.epnwcf.com/Article/details/gdhoqfven.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/ggdqcrxrr.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fktsv.cn/Article/details/glwdawgya.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.vehdjk.com/Article/details/guogjbuhc.sHtML

[T11] Kotlin：协程
来源：http://www.blog.epnwcf.com/Article/details/gjddrpakf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/gkuwgiuvw.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gfeokugdq.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/gkuqjvkpp.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.yfazqb.com/Article/details/gqlpinfsd.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/gxuccxves.sHtML

[T14] Kotlin：循环
来源：http://www.blog.yfazqb.com/Article/details/gnawxwacd.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gngntbiuf.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/gkzhejraj.sHtML

interface Shape { fun area(): Double }
来源：http://baike.bbcook.cn/Article/details/glvuuypbr.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gwyjdtcpb.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/guhlwufgv.sHtML

[T17] Swift：变量与常量
来源：http://mobile.sjlbkw.cn/Article/details/gqueyumud.sHtML

var a = 1;  let b = 2
来源：http://mobile.bbcook.cn/Article/details/ghbpxxdvc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gxjroitvx.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gmyqoiwoz.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.epnwcf.com/Article/details/gssinwgsa.sHtML

if let n = opt { print(n) }
来源：http://www.share.yfazqb.com/Article/details/gogullqan.sHtML

[T20] Swift：数组操作
来源：http://3g.fktsv.cn/Article/details/gafrvfgxl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fktsv.cn/Article/details/gdkplztto.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fktsv.cn/Article/details/grioeimko.sHtML

for x in a { print(x) }
来源：http://m.share.epnwcf.com/Article/details/gxesibfyr.sHtML

[T22] Swift：字典
来源：http://read.share.epnwcf.com/Article/details/gkcickgrg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.bbcook.cn/Article/details/gnhkpzhuk.sHtML

[T23] Swift：函数
来源：http://www.m.share.vehdjk.com/Article/details/ggotrusxv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.vehdjk.com/Article/details/gavpaadqw.sHtML

[T24] Swift：闭包
来源：http://wap.fktsv.cn/Article/details/gjnqbnpiu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.epnwcf.com/Article/details/gozbivuvj.sHtML

[T25] Swift：结构体
来源：http://www.m.share.bbcook.cn/Article/details/gzdjgmror.sHtML

struct P { var x: Int }
来源：http://wap.yfazqb.com/Article/details/gqcmkdzhx.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.tarul.cn/Article/details/gyxyxdcsg.sHtML

class A: Base { override func f() {} }
来源：http://mobile.bbcook.cn/Article/details/gvewwkoww.sHtML

[T27] Swift：错误处理
来源：http://m.share.sjlbkw.cn/Article/details/gwaltdysr.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.tarul.cn/Article/details/gwryjebev.sHtML

[T28] Swift：枚举
来源：http://m.share.fktsv.cn/Article/details/gknstftsx.sHtML

enum Color { case red, green }
来源：http://blog.bbcook.cn/Article/details/gdhcvokmm.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fktsv.cn/Article/details/gnlgdecst.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/gzrwdjhyz.sHtML

[T30] Swift：协议
来源：http://m.share.sjlbkw.cn/Article/details/gnfjmayol.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.yfazqb.com/Article/details/gwinuzqhe.sHtML

[T31] Lua：Hello World
来源：http://www.blog.tarul.cn/Article/details/gdspdlisi.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gktymjwtq.sHtML

[T32] Lua：局部变量
来源：http://3g.yfazqb.com/Article/details/gnozqagee.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/gbmswpysg.sHtML

[T33] Lua：表（数组）
来源：http://mobile.yfazqb.com/Article/details/geapmzaya.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.epnwcf.com/Article/details/gyjluvnaa.sHtML

[T34] Lua：遍历表
来源：http://www.blog.sjlbkw.cn/Article/details/grqwvurgi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.bbcook.cn/Article/details/gtkzpjxdz.sHtML

[T35] Lua：字典表
来源：http://m.share.bbcook.cn/Article/details/gedaomupc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.epnwcf.com/Article/details/gjkkwapcv.sHtML

[T36] Lua：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdklagof.sHtML

function add(a, b) return a + b end
来源：http://3g.tarul.cn/Article/details/gehntquzo.sHtML

[T37] Lua：字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/ghmcwccty.sHtML

"a" .. "b"
来源：http://mobile.fktsv.cn/Article/details/gspmjkgbu.sHtML

[T38] Lua：条件
来源：http://3g.fktsv.cn/Article/details/ghtnetzvp.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.bbcook.cn/Article/details/guzjvheaz.sHtML

[T39] Lua：模式匹配
来源：http://mobile.vehdjk.com/Article/details/gevkmfbio.sHtML

string.find(s, "%d+")
来源：http://mobile.bbcook.cn/Article/details/gkjndbuan.sHtML

[T40] Lua：元表
来源：http://www.m.share.sjlbkw.cn/Article/details/gufbwawrx.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.tarul.cn/Article/details/gwcpkivww.sHtML

[T41] Perl：Hello World
来源：http://3g.bbcook.cn/Article/details/gjsjqiloe.sHtML

print "Hello\n";
来源：http://read.share.bbcook.cn/Article/details/gqlvuozmp.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.vehdjk.com/Article/details/gcrosgwqt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.epnwcf.com/Article/details/gskiieufl.sHtML

[T43] Perl：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gykvpvowv.sHtML

"值: $a"
来源：http://read.share.bbcook.cn/Article/details/gdsererhk.sHtML

[T44] Perl：条件
来源：http://m.share.fktsv.cn/Article/details/gbfyyunts.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.yfazqb.com/Article/details/ggsqejoyo.sHtML

[T45] Perl：数组遍历
来源：http://3g.epnwcf.com/Article/details/gsamujkbc.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fktsv.cn/Article/details/gnyhqsdya.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.bbcook.cn/Article/details/gvpxtukxl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fktsv.cn/Article/details/gkozaeipu.sHtML

[T47] Perl：正则捕获
来源：http://baike.yfazqb.com/Article/details/gajzvrsrv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.epnwcf.com/Article/details/gtrsyeebt.sHtML

[T48] Perl：正则替换
来源：http://www.blog.sjlbkw.cn/Article/details/gcderovmy.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.tarul.cn/Article/details/ghnvnhulz.sHtML

[T49] Perl：函数
来源：http://www.share.sjlbkw.cn/Article/details/gzmebhcht.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gfwcfplod.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gzbcqglqs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.sjlbkw.cn/Article/details/gwxjtafsr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.bbcook.cn/Article/details/gfygozibu.sHtML

[T51] Scala：Hello World
来源：http://read.share.tarul.cn/Article/details/gdgfimsbr.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/grokzrnan.sHtML

[T52] Scala：变量
来源：http://baike.bbcook.cn/Article/details/gnzwsztir.sHtML

val a = 1;  var b = 2
来源：http://wap.tarul.cn/Article/details/guhkgsxjc.sHtML

[T53] Scala：字符串插值
来源：http://3g.epnwcf.com/Article/details/gvpcoinpe.sHtML

s"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/gybbromfw.sHtML

[T54] Scala：集合映射
来源：http://mobile.vehdjk.com/Article/details/gjzbjozmo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.epnwcf.com/Article/details/gdwmkxktg.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/ghohhrmsj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.bbcook.cn/Article/details/ggyicdbst.sHtML

[T56] Scala：样例类
来源：http://blog.vehdjk.com/Article/details/gdtvmnxdm.sHtML

case class User(name: String, age: Int)
来源：http://3g.vehdjk.com/Article/details/godfkkzvd.sHtML

[T57] Scala：模式匹配
来源：http://baike.tarul.cn/Article/details/ggwysvdqj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.vehdjk.com/Article/details/gjndnlclo.sHtML

[T58] Scala：函数定义
来源：http://m.share.sjlbkw.cn/Article/details/gtqeibnpo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.tarul.cn/Article/details/grtxyerma.sHtML

[T59] Scala：循环
来源：http://baike.vehdjk.com/Article/details/gsnrzwvyn.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.epnwcf.com/Article/details/gqptcybnc.sHtML

[T60] Scala：折叠
来源：http://baike.tarul.cn/Article/details/gkczbvuno.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.vehdjk.com/Article/details/gxgybgsia.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grgwmdwyz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/gupjedubm.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gcfoguemm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.epnwcf.com/Article/details/gdshekrca.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.tarul.cn/Article/details/gxvduwynl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.bbcook.cn/Article/details/gxmwogbva.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.vehdjk.com/Article/details/grdgcnwdf.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.sjlbkw.cn/Article/details/gniynvpgj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.yfazqb.com/Article/details/gtwmjuyjx.sHtML

[U04] Py：变量调试打印
来源：http://wap.fktsv.cn/Article/details/gefxgsmei.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.tarul.cn/Article/details/gdlbfhrnu.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.sjlbkw.cn/Article/details/gkrcrfcpb.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.bbcook.cn/Article/details/gymlkxptp.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.sjlbkw.cn/Article/details/ggydxstoz.sHtML

{**a, **b}
来源：http://m.share.vehdjk.com/Article/details/gsvvhtpdi.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fktsv.cn/Article/details/gwsopiqef.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/gkmggkots.sHtML

[U08] Py：展平二维列表
来源：http://3g.vehdjk.com/Article/details/gpkkefrqc.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.epnwcf.com/Article/details/gfwauybws.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.tarul.cn/Article/details/glghrjphx.sHtML

max(d, key=d.get)
来源：http://www.share.fktsv.cn/Article/details/gjltpiosa.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fktsv.cn/Article/details/gfyyozybg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.tarul.cn/Article/details/grtbjftzi.sHtML

[U11] Py：生成器表达式
来源：http://m.share.bbcook.cn/Article/details/gnraysuse.sHtML

(x * 2 for x in arr)
来源：http://wap.yfazqb.com/Article/details/geecvhzfz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.sjlbkw.cn/Article/details/gwcazpsig.sHtML

Counter(arr).most_common(3)
来源：http://blog.yfazqb.com/Article/details/giexqwtwc.sHtML

[U13] Py：固定长度队列
来源：http://www.share.yfazqb.com/Article/details/gvkqvlhqc.sHtML

deque(maxlen=10)
来源：http://www.share.sjlbkw.cn/Article/details/ghoiqmrsb.sHtML

[U14] Py：分组收集到列表
来源：http://3g.sjlbkw.cn/Article/details/giqaaipxz.sHtML

defaultdict(list)
来源：http://www.blog.tarul.cn/Article/details/gflsiosje.sHtML

[U15] Py：高精度计时
来源：http://m.share.tarul.cn/Article/details/gijmgsins.sHtML

t = time.perf_counter()
来源：http://www.m.share.yfazqb.com/Article/details/gbfxihzyr.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.yfazqb.com/Article/details/gcxvbticq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.vehdjk.com/Article/details/gubpxnpha.sHtML

[U17] Py：初始化日志
来源：http://read.share.yfazqb.com/Article/details/gfzisycoy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fktsv.cn/Article/details/gqmycjrgz.sHtML

[U18] Py：预编译正则
来源：http://wap.yfazqb.com/Article/details/gikskuofy.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gagitgodg.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fktsv.cn/Article/details/gvmmtxncr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.bbcook.cn/Article/details/gglzrnvmf.sHtML

[U20] Py：缓存函数结果
来源：http://3g.bbcook.cn/Article/details/gqtxudzdp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.vehdjk.com/Article/details/gzopnczmg.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.sjlbkw.cn/Article/details/gcqqssben.sHtML

@contextlib.contextmanager
来源：http://read.share.bbcook.cn/Article/details/glaffsmlu.sHtML

[U22] Py：矩阵转置
来源：http://baike.tarul.cn/Article/details/gfkmcasiu.sHtML

list(zip(*m))
来源：http://wap.vehdjk.com/Article/details/gzmcitfqj.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.bbcook.cn/Article/details/gxssbxvke.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.bbcook.cn/Article/details/gcvdptxmj.sHtML

[U24] Py：路径操作
来源：http://mobile.sjlbkw.cn/Article/details/gmqmjpowg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/gvmdressn.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fktsv.cn/Article/details/glpbtdmsu.sHtML

csv.DictReader(f)
来源：http://blog.fktsv.cn/Article/details/geirzxodu.sHtML

[U26] Py：并发下载
来源：http://3g.vehdjk.com/Article/details/gfqnembqu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.bbcook.cn/Article/details/gxmsldftf.sHtML

[U27] Py：异步 HTTP
来源：http://3g.vehdjk.com/Article/details/gmuyahuuu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.yfazqb.com/Article/details/gktvxmwqs.sHtML

[U28] Py：类型别名
来源：http://www.blog.tarul.cn/Article/details/gnwcjgljn.sHtML

UserId = int
来源：http://www.share.yfazqb.com/Article/details/gxhtksgle.sHtML

[U29] Py：属性校验
来源：http://www.m.share.epnwcf.com/Article/details/gaglhgplw.sHtML

@property 与 @x.setter 配合
来源：http://m.share.vehdjk.com/Article/details/gorvzokws.sHtML

[U30] Py：数据类
来源：http://wap.bbcook.cn/Article/details/gchijpbcs.sHtML

@dataclass(slots=True)
来源：http://www.share.bbcook.cn/Article/details/gqczmnrvt.sHtML

[U31] Py：单测
来源：http://blog.fktsv.cn/Article/details/gckuzvwdx.sHtML

python -m pytest -q
来源：http://www.m.share.tarul.cn/Article/details/gqpzpbwey.sHtML

[U32] Py：代码格式化
来源：http://baike.bbcook.cn/Article/details/gqzxmipqa.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.yfazqb.com/Article/details/glscuzjde.sHtML

[U33] Py：打包发布
来源：http://baike.epnwcf.com/Article/details/gwzhvjluj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fktsv.cn/Article/details/gdjkuuhrr.sHtML

[U34] Py：判断编码
来源：http://blog.vehdjk.com/Article/details/gvjpxdqrn.sHtML

chardet.detect(raw)
来源：http://3g.tarul.cn/Article/details/giwhexexr.sHtML

[U35] Py：发送邮件
来源：http://wap.bbcook.cn/Article/details/gixxbqdbj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fktsv.cn/Article/details/gqronxblo.sHtML

[U36] Py：定时任务
来源：http://mobile.vehdjk.com/Article/details/ghxrvauln.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.yfazqb.com/Article/details/gokughkfl.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fktsv.cn/Article/details/gikezutpw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.tarul.cn/Article/details/gdaqyxmjn.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.tarul.cn/Article/details/gnohjauwf.sHtML

Path(__file__).resolve().parent
来源：http://blog.vehdjk.com/Article/details/gklshqyvo.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.vehdjk.com/Article/details/gmtzzkkdv.sHtML

sys.stdout.isatty()
来源：http://m.share.sjlbkw.cn/Article/details/gwwffuvzh.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fktsv.cn/Article/details/goxbjxwrw.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/gfpzdesdi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.vehdjk.com/Article/details/gcfawzows.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.tarul.cn/Article/details/gvfnkxztu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.vehdjk.com/Article/details/gbgwwydfm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.bbcook.cn/Article/details/gqekrcvuo.sHtML


<!-- 参考信息 -->