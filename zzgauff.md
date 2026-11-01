代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/genvfmxco.sHtML

[S21] C：字符类别判断
来源：http://3g.vehdjk.com/Article/details/gyjajpkzy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fktsv.cn/Article/details/grbmydtnc.sHtML

[S22] C：字符串转数字
来源：http://m.share.fktsv.cn/Article/details/gtzphzlmg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.vehdjk.com/Article/details/ghgqqtgom.sHtML

[S23] C：随机数
来源：http://www.m.share.bbcook.cn/Article/details/glhyaboik.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.sjlbkw.cn/Article/details/gjmvvyvfr.sHtML

[S24] C：获取本地时间
来源：http://blog.vehdjk.com/Article/details/gpxpbhqdq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/goatqrkvs.sHtML

[S25] C：内存拷贝
来源：http://3g.sjlbkw.cn/Article/details/gxwbybqfc.sHtML

memcpy(dst, src, n);
来源：http://m.share.vehdjk.com/Article/details/gpaeivmza.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/gtvxpcczb.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.yfazqb.com/Article/details/grwklrzis.sHtML

[S27] C：定义常量
来源：http://baike.sjlbkw.cn/Article/details/gfldsljyf.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gugewueik.sHtML

[S28] C：静态变量
来源：http://www.blog.bbcook.cn/Article/details/guulaqcsf.sHtML

static int counter = 0;
来源：http://baike.bbcook.cn/Article/details/gdimnnlpi.sHtML

[S29] C：变参函数
来源：http://m.share.yfazqb.com/Article/details/gttqxvrsg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fktsv.cn/Article/details/gobazdblf.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/gnmwnealf.sHtML

#ifndef X_H
来源：http://www.m.share.yfazqb.com/Article/details/gwqiltqrx.sHtML

#define X_H
来源：http://m.share.tarul.cn/Article/details/gnoxgzycp.sHtML

#endif
来源：http://www.blog.vehdjk.com/Article/details/gfjdojhzd.sHtML

[S31] C++：Hello World
来源：http://3g.yfazqb.com/Article/details/gwangyxtm.sHtML

#include <iostream>
来源：http://m.share.bbcook.cn/Article/details/gkhjghipq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.epnwcf.com/Article/details/gdbvtffhn.sHtML

[S32] C++：字符串
来源：http://read.share.bbcook.cn/Article/details/gwqxzkqua.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.vehdjk.com/Article/details/ggkrcdrrk.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gfnpdcrli.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.sjlbkw.cn/Article/details/gnxgchzlm.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fktsv.cn/Article/details/ghefcltbz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gfnqecnmn.sHtML

[S35] C++：map
来源：http://blog.tarul.cn/Article/details/gdrxzvlgw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gjcjufcbb.sHtML

[S36] C++：unordered_map
来源：http://m.share.sjlbkw.cn/Article/details/gzjyydqnk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/grghjvgly.sHtML

[S37] C++：set
来源：http://3g.epnwcf.com/Article/details/gbitzzgvq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.vehdjk.com/Article/details/gxmnnnrzb.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/gswjaaefc.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.sjlbkw.cn/Article/details/grlsfuhrs.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gsgursldg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.tarul.cn/Article/details/gidrjdffd.sHtML

[S40] C++：查找元素
来源：http://blog.bbcook.cn/Article/details/galbcnkee.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.tarul.cn/Article/details/gtbyoicbt.sHtML

[S41] C++：类与构造函数
来源：http://baike.fktsv.cn/Article/details/gqxiolnat.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.epnwcf.com/Article/details/gtfuzygvj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fktsv.cn/Article/details/gvathemkt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fktsv.cn/Article/details/gauvaylxv.sHtML

[S43] C++：智能指针
来源：http://www.share.tarul.cn/Article/details/gcgyedexo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fktsv.cn/Article/details/glgwqizcs.sHtML

[S44] C++：引用传参
来源：http://wap.tarul.cn/Article/details/glzslexmc.sHtML

void inc(int &x) { ++x; }
来源：http://blog.epnwcf.com/Article/details/gfoohjpej.sHtML

[S45] C++：lambda
来源：http://wap.sjlbkw.cn/Article/details/gkrpjwzes.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.epnwcf.com/Article/details/gzohfwrxb.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fktsv.cn/Article/details/gdlboaebm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fktsv.cn/Article/details/grlaodzmc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gcpjmchaa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fktsv.cn/Article/details/gtrczuohq.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/ghffafufg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.bbcook.cn/Article/details/gvgrijuir.sHtML

while (std::getline(in, line)) { }
来源：http://blog.yfazqb.com/Article/details/glzmfgcpo.sHtML

[S49] C++：写文件
来源：http://www.blog.bbcook.cn/Article/details/gldtubnpq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/gvdswaysj.sHtML

[S50] C++：格式化数字
来源：http://mobile.fktsv.cn/Article/details/gbaangclq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gtgojsrjn.sHtML

[S51] C++：显式类型转换
来源：http://wap.epnwcf.com/Article/details/gwxztouqg.sHtML

static_cast<double>(a) / b
来源：http://3g.bbcook.cn/Article/details/ggntsgpzr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/gvqbsidie.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gffkgzmap.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/gaqjhkzvz.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.yfazqb.com/Article/details/glcaowdoq.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/gvgyyqwmu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.epnwcf.com/Article/details/gtzboeufr.sHtML

[S55] C++：结构化绑定
来源：http://blog.epnwcf.com/Article/details/glmhfylye.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gncobdrqs.sHtML

[S56] C++：optional
来源：http://mobile.bbcook.cn/Article/details/gcvkphdsp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.bbcook.cn/Article/details/gsineixnj.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/gixalponw.sHtML

constexpr int N = 10;
来源：http://read.share.fktsv.cn/Article/details/gshiglwlr.sHtML

[S58] C++：命名空间
来源：http://mobile.yfazqb.com/Article/details/gowlgpoyl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.yfazqb.com/Article/details/ggxgauink.sHtML

[S59] C++：静态断言
来源：http://mobile.tarul.cn/Article/details/gxyodznrg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.tarul.cn/Article/details/gecwhxzgn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gmwlcbzml.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/gkbjdojfb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqrevsglr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/ggljxomef.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqstzkwdf.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/glcgcrgkq.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gwidpgcvr.sHtML

[T02] Kotlin：变量
来源：http://read.share.tarul.cn/Article/details/gfrmtpqfd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/gdayylrjd.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.bbcook.cn/Article/details/goumuzbqr.sHtML

"值: $b"
来源：http://mobile.epnwcf.com/Article/details/gjslcqcgh.sHtML

[T04] Kotlin：空安全
来源：http://mobile.tarul.cn/Article/details/gndtztjqi.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.yfazqb.com/Article/details/gvswsfvap.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gjegkjbcv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fktsv.cn/Article/details/gvvimpgpm.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/gcuktpxqp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gosbirnfx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/glqbluvns.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gemdpxulx.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/gjlofbjxy.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.epnwcf.com/Article/details/gcycplisg.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.epnwcf.com/Article/details/gzynlmkpt.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.yfazqb.com/Article/details/gibswxwcq.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gzdakkoip.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fktsv.cn/Article/details/gmtendytb.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fktsv.cn/Article/details/gujxhgtjk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.yfazqb.com/Article/details/gtsudxwtx.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.vehdjk.com/Article/details/gjvsbmtyj.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gslcaytag.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fktsv.cn/Article/details/gmwpwixcm.sHtML

val m = mapOf("a" to 1)
来源：http://3g.bbcook.cn/Article/details/gidgsaydz.sHtML

[T14] Kotlin：循环
来源：http://read.share.tarul.cn/Article/details/gjjlxmcjd.sHtML

for (i in 1..10) println(i)
来源：http://3g.tarul.cn/Article/details/gpaksfjtm.sHtML

[T15] Kotlin：接口
来源：http://baike.sjlbkw.cn/Article/details/gvkjqofts.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.yfazqb.com/Article/details/ggguwkpxu.sHtML

[T16] Swift：Hello World
来源：http://m.share.vehdjk.com/Article/details/guzgmgxkq.sHtML

print("Hello")
来源：http://m.share.epnwcf.com/Article/details/ggqsaocap.sHtML

[T17] Swift：变量与常量
来源：http://mobile.vehdjk.com/Article/details/gemiqdkco.sHtML

var a = 1;  let b = 2
来源：http://wap.vehdjk.com/Article/details/gllewfuhv.sHtML

[T18] Swift：字符串插值
来源：http://wap.fktsv.cn/Article/details/gxmnwbkdk.sHtML

"值: \(b)"
来源：http://www.m.share.fktsv.cn/Article/details/gsvmvhsib.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.vehdjk.com/Article/details/gzzohqycv.sHtML

if let n = opt { print(n) }
来源：http://read.share.yfazqb.com/Article/details/gsktayvtm.sHtML

[T20] Swift：数组操作
来源：http://www.share.tarul.cn/Article/details/ggwwqixaf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.vehdjk.com/Article/details/gaqswcebi.sHtML

[T21] Swift：遍历
来源：http://3g.sjlbkw.cn/Article/details/gdkgiezxg.sHtML

for x in a { print(x) }
来源：http://www.share.epnwcf.com/Article/details/gnnbboxrz.sHtML

[T22] Swift：字典
来源：http://www.m.share.vehdjk.com/Article/details/gadfekdzn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.yfazqb.com/Article/details/gdhcdjcnu.sHtML

[T23] Swift：函数
来源：http://3g.fktsv.cn/Article/details/gcqfdhlde.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gavlkpgrh.sHtML

[T24] Swift：闭包
来源：http://wap.epnwcf.com/Article/details/ghwscrdwp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.bbcook.cn/Article/details/gkiaghnqw.sHtML

[T25] Swift：结构体
来源：http://blog.bbcook.cn/Article/details/gnzrerghc.sHtML

struct P { var x: Int }
来源：http://wap.vehdjk.com/Article/details/gvyolddwv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.vehdjk.com/Article/details/glebjphco.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.tarul.cn/Article/details/gdvmptstw.sHtML

[T27] Swift：错误处理
来源：http://www.share.fktsv.cn/Article/details/gkeecipbx.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.tarul.cn/Article/details/glegivdhp.sHtML

[T28] Swift：枚举
来源：http://wap.sjlbkw.cn/Article/details/gchnqinzk.sHtML

enum Color { case red, green }
来源：http://www.m.share.fktsv.cn/Article/details/gnsyjoqni.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.epnwcf.com/Article/details/gcigecjqh.sHtML

guard let x = opt else { return }
来源：http://www.share.bbcook.cn/Article/details/gpiwtmmrw.sHtML

[T30] Swift：协议
来源：http://wap.bbcook.cn/Article/details/gssnptubj.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.bbcook.cn/Article/details/gqmsizixh.sHtML

[T31] Lua：Hello World
来源：http://mobile.fktsv.cn/Article/details/gfjwrwfij.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/gtiycnufs.sHtML

[T32] Lua：局部变量
来源：http://m.share.fktsv.cn/Article/details/glisehivh.sHtML

local a = 1
来源：http://mobile.epnwcf.com/Article/details/ghckzvbea.sHtML

[T33] Lua：表（数组）
来源：http://baike.fktsv.cn/Article/details/gxrlvjpjx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.tarul.cn/Article/details/garegcvkl.sHtML

[T34] Lua：遍历表
来源：http://www.blog.sjlbkw.cn/Article/details/grhiwbfwo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.vehdjk.com/Article/details/gavwitlxd.sHtML

[T35] Lua：字典表
来源：http://wap.epnwcf.com/Article/details/gduuxyssm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/goprjfsqw.sHtML

[T36] Lua：函数
来源：http://www.share.vehdjk.com/Article/details/grrsrlhaj.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.sjlbkw.cn/Article/details/gljkemudt.sHtML

[T37] Lua：字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gjzgujykb.sHtML

"a" .. "b"
来源：http://read.share.sjlbkw.cn/Article/details/geuampust.sHtML

[T38] Lua：条件
来源：http://www.blog.vehdjk.com/Article/details/gyjprgbjv.sHtML

if x > 0 then print("正") end
来源：http://www.share.bbcook.cn/Article/details/gojcbftcu.sHtML

[T39] Lua：模式匹配
来源：http://baike.fktsv.cn/Article/details/gmairxeyu.sHtML

string.find(s, "%d+")
来源：http://read.share.epnwcf.com/Article/details/gpoyxnvvn.sHtML

[T40] Lua：元表
来源：http://m.share.fktsv.cn/Article/details/gvcflgayf.sHtML

setmetatable({}, { __index = base })
来源：http://baike.bbcook.cn/Article/details/gdjbisaat.sHtML

[T41] Perl：Hello World
来源：http://blog.epnwcf.com/Article/details/gmijhphgd.sHtML

print "Hello\n";
来源：http://www.blog.bbcook.cn/Article/details/gmqrdocsx.sHtML

[T42] Perl：变量类型
来源：http://read.share.epnwcf.com/Article/details/gshlntrds.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.epnwcf.com/Article/details/gfzqjsbbj.sHtML

[T43] Perl：字符串插值
来源：http://baike.bbcook.cn/Article/details/gzvqbhkyp.sHtML

"值: $a"
来源：http://www.blog.bbcook.cn/Article/details/gvnrbxlvm.sHtML

[T44] Perl：条件
来源：http://baike.epnwcf.com/Article/details/ghpdtpksi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fktsv.cn/Article/details/gkiurdxpy.sHtML

[T45] Perl：数组遍历
来源：http://mobile.sjlbkw.cn/Article/details/gubkvcrmo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.bbcook.cn/Article/details/gwvpidrzy.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.tarul.cn/Article/details/gwpkegvvq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/gtdgbaxro.sHtML

[T47] Perl：正则捕获
来源：http://www.share.bbcook.cn/Article/details/gbaqrlvgw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.sjlbkw.cn/Article/details/glqfohujr.sHtML

[T48] Perl：正则替换
来源：http://baike.epnwcf.com/Article/details/gnryjdprf.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/gdpmcapxe.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/gaenyvbue.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/glpwlvsue.sHtML

[T50] Perl：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gqksmpcqm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.yfazqb.com/Article/details/gzlzeyodx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.tarul.cn/Article/details/gwwmkpjwz.sHtML

[T51] Scala：Hello World
来源：http://mobile.tarul.cn/Article/details/gypxrapmt.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gtflmjqao.sHtML

[T52] Scala：变量
来源：http://www.share.vehdjk.com/Article/details/ghfwphxar.sHtML

val a = 1;  var b = 2
来源：http://baike.bbcook.cn/Article/details/guwjyxocl.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/glodxqbzi.sHtML

s"值: $b"
来源：http://blog.yfazqb.com/Article/details/gxwcrkgbr.sHtML

[T54] Scala：集合映射
来源：http://blog.epnwcf.com/Article/details/gfjhhpqra.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.epnwcf.com/Article/details/gdgrbuhgb.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gnrwfxhch.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.yfazqb.com/Article/details/gtzuivzoe.sHtML

[T56] Scala：样例类
来源：http://blog.epnwcf.com/Article/details/gvhofoqbo.sHtML

case class User(name: String, age: Int)
来源：http://mobile.bbcook.cn/Article/details/grtzirexi.sHtML

[T57] Scala：模式匹配
来源：http://wap.bbcook.cn/Article/details/gxqxzsjvk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.tarul.cn/Article/details/gvrnhpwna.sHtML

[T58] Scala：函数定义
来源：http://wap.yfazqb.com/Article/details/gmihnbwnf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.bbcook.cn/Article/details/gtesfvskk.sHtML

[T59] Scala：循环
来源：http://www.m.share.yfazqb.com/Article/details/gtctwgdcj.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gsopyqmop.sHtML

[T60] Scala：折叠
来源：http://3g.vehdjk.com/Article/details/gzfaszoxk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.yfazqb.com/Article/details/gmngxmxak.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxloogjwf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuanqifr.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpfrsnqrb.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.bbcook.cn/Article/details/grqpqwuzg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.vehdjk.com/Article/details/gnddbltlz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.epnwcf.com/Article/details/gnszcqlbj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fktsv.cn/Article/details/gfouwrfio.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.epnwcf.com/Article/details/gxwtlirdk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fktsv.cn/Article/details/golbyjehq.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.yfazqb.com/Article/details/gsdjrpkks.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.sjlbkw.cn/Article/details/gyexjnfjf.sHtML

[U05] Py：列表去重且保序
来源：http://baike.epnwcf.com/Article/details/gvjbfpfxo.sHtML

list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gqckvqnqf.sHtML

[U06] Py：合并两个字典
来源：http://3g.tarul.cn/Article/details/gcbljxsob.sHtML

{**a, **b}
来源：http://wap.bbcook.cn/Article/details/gjyrginhw.sHtML

[U07] Py：反转字典键值
来源：http://www.share.epnwcf.com/Article/details/gtecrvfkd.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.sjlbkw.cn/Article/details/gaoiqhwqu.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.epnwcf.com/Article/details/glynhouyv.sHtML

[y for x in nested for y in x]
来源：http://read.share.epnwcf.com/Article/details/gprfwapqv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.yfazqb.com/Article/details/gqsphdasn.sHtML

max(d, key=d.get)
来源：http://mobile.sjlbkw.cn/Article/details/gvleywely.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fktsv.cn/Article/details/glbrvbvld.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.yfazqb.com/Article/details/gvjczghnd.sHtML

[U11] Py：生成器表达式
来源：http://wap.yfazqb.com/Article/details/gqpjhleqo.sHtML

(x * 2 for x in arr)
来源：http://blog.fktsv.cn/Article/details/ggeanoisf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.yfazqb.com/Article/details/gvboqfqjx.sHtML

Counter(arr).most_common(3)
来源：http://mobile.tarul.cn/Article/details/gmluitrne.sHtML

[U13] Py：固定长度队列
来源：http://blog.yfazqb.com/Article/details/gfhdgtfvc.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/gpkzcpalc.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.vehdjk.com/Article/details/gdrkokbuh.sHtML

defaultdict(list)
来源：http://blog.yfazqb.com/Article/details/gsjmezkyv.sHtML

[U15] Py：高精度计时
来源：http://www.share.vehdjk.com/Article/details/gfyeazaln.sHtML

t = time.perf_counter()
来源：http://wap.tarul.cn/Article/details/gyevpnmgk.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.bbcook.cn/Article/details/gyumhmrug.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.bbcook.cn/Article/details/godoyhnff.sHtML

[U17] Py：初始化日志
来源：http://mobile.vehdjk.com/Article/details/gzkysgpxq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcujpgrou.sHtML

[U18] Py：预编译正则
来源：http://read.share.bbcook.cn/Article/details/ghucrtbuc.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.tarul.cn/Article/details/gzprqpiyt.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.sjlbkw.cn/Article/details/giqfcuqgy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.vehdjk.com/Article/details/govfpdkyk.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.epnwcf.com/Article/details/ghwtaktwq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.yfazqb.com/Article/details/gjxdereci.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.yfazqb.com/Article/details/gmpfrpavb.sHtML

@contextlib.contextmanager
来源：http://www.blog.fktsv.cn/Article/details/ghiyhxmjb.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.tarul.cn/Article/details/gibompjsg.sHtML

list(zip(*m))
来源：http://3g.tarul.cn/Article/details/ghialhrip.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fktsv.cn/Article/details/glsnfkjjh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fktsv.cn/Article/details/goyeunccm.sHtML

[U24] Py：路径操作
来源：http://blog.vehdjk.com/Article/details/gshcwwibz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/ghnflciyi.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.epnwcf.com/Article/details/gzdcclguo.sHtML

csv.DictReader(f)
来源：http://baike.vehdjk.com/Article/details/gzmovblgl.sHtML

[U26] Py：并发下载
来源：http://www.blog.sjlbkw.cn/Article/details/gweudmkef.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.vehdjk.com/Article/details/gwdltktma.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.yfazqb.com/Article/details/gnzifuhvw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.epnwcf.com/Article/details/gbyomlrzf.sHtML

[U28] Py：类型别名
来源：http://www.blog.fktsv.cn/Article/details/gneqkkhla.sHtML

UserId = int
来源：http://wap.epnwcf.com/Article/details/geeawbjtc.sHtML

[U29] Py：属性校验
来源：http://mobile.bbcook.cn/Article/details/gluykxuzk.sHtML

@property 与 @x.setter 配合
来源：http://read.share.tarul.cn/Article/details/gtwemcjlt.sHtML

[U30] Py：数据类
来源：http://www.blog.fktsv.cn/Article/details/garafdxil.sHtML

@dataclass(slots=True)
来源：http://blog.epnwcf.com/Article/details/guhvwztkr.sHtML

[U31] Py：单测
来源：http://m.share.sjlbkw.cn/Article/details/gklweeqyy.sHtML

python -m pytest -q
来源：http://www.m.share.bbcook.cn/Article/details/gnohfbwqz.sHtML

[U32] Py：代码格式化
来源：http://3g.tarul.cn/Article/details/gbudpbtvw.sHtML

ruff format . && ruff check --fix .
来源：http://wap.yfazqb.com/Article/details/gxqlogkzd.sHtML

[U33] Py：打包发布
来源：http://mobile.sjlbkw.cn/Article/details/glmedzrpd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.bbcook.cn/Article/details/gmxlhvlel.sHtML

[U34] Py：判断编码
来源：http://mobile.sjlbkw.cn/Article/details/gdzsqjfyu.sHtML

chardet.detect(raw)
来源：http://blog.yfazqb.com/Article/details/gutkwuqgl.sHtML

[U35] Py：发送邮件
来源：http://www.blog.sjlbkw.cn/Article/details/gjnremzed.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.bbcook.cn/Article/details/gkgsycxpd.sHtML

[U36] Py：定时任务
来源：http://blog.bbcook.cn/Article/details/gebwlkvil.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.vehdjk.com/Article/details/guqjlchin.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fktsv.cn/Article/details/grtbkznas.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.bbcook.cn/Article/details/gxfrwutlb.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.vehdjk.com/Article/details/gjolwhitw.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.epnwcf.com/Article/details/gyitlwzba.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.sjlbkw.cn/Article/details/giolrjdmo.sHtML

sys.stdout.isatty()
来源：http://www.blog.bbcook.cn/Article/details/gldqgocpt.sHtML

[U40] Py：打印到标准错误
来源：http://baike.epnwcf.com/Article/details/guvflxqjn.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gguqjsbrv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.tarul.cn/Article/details/grufbdjvu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.sjlbkw.cn/Article/details/gjmdtwanh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.tarul.cn/Article/details/gctrcnlzk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.tarul.cn/Article/details/gisjoyutx.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.tarul.cn/Article/details/gegjqztaw.sHtML

namespace App\Http;
来源：http://m.share.sjlbkw.cn/Article/details/gpjmsomcq.sHtML

[U44] PHP：开启严格类型
来源：http://baike.yfazqb.com/Article/details/gxvlplnho.sHtML

declare(strict_types=1);
来源：http://mobile.tarul.cn/Article/details/gxpkysjkw.sHtML


<!-- 参考信息 -->