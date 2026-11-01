代发 wailian999

int main(int argc, char **argv)
来源：http://www.blog.yfazqb.com/Article/details/gukwcsdhe.sHtML

[S19] C：快速排序
来源：http://m.share.bbcook.cn/Article/details/gzlylzrdu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gagnprice.sHtML

[S20] C：二分查找
来源：http://m.share.bbcook.cn/Article/details/grhbjqqgz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gdfbaivdk.sHtML

[S21] C：字符类别判断
来源：http://read.share.bbcook.cn/Article/details/gfdvgqafd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.vehdjk.com/Article/details/ghgqyjzdx.sHtML

[S22] C：字符串转数字
来源：http://wap.fktsv.cn/Article/details/groqzwqkh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.vehdjk.com/Article/details/gjcuvyflz.sHtML

[S23] C：随机数
来源：http://mobile.yfazqb.com/Article/details/gpgsibaer.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.bbcook.cn/Article/details/gdmfxndsp.sHtML

[S24] C：获取本地时间
来源：http://baike.epnwcf.com/Article/details/grtojtuxg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fktsv.cn/Article/details/gqujaeykj.sHtML

[S25] C：内存拷贝
来源：http://read.share.tarul.cn/Article/details/gncmbdgtj.sHtML

memcpy(dst, src, n);
来源：http://blog.yfazqb.com/Article/details/gyzelyhhe.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/gnwmjrrdp.sHtML

memset(a, 0, sizeof a);
来源：http://blog.tarul.cn/Article/details/gbubwvdfb.sHtML

[S27] C：定义常量
来源：http://www.share.fktsv.cn/Article/details/gsvhvurbv.sHtML

const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gcoxngxnc.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gsxnruvbp.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/gzutvmemm.sHtML

[S29] C：变参函数
来源：http://baike.yfazqb.com/Article/details/guswmjtcp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.sjlbkw.cn/Article/details/gfkrkscaf.sHtML

[S30] C：头文件保护
来源：http://read.share.fktsv.cn/Article/details/grczhgxae.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gpxuerzza.sHtML

#define X_H
来源：http://read.share.sjlbkw.cn/Article/details/gmkqoimkt.sHtML

#endif
来源：http://mobile.tarul.cn/Article/details/gnhrivwbf.sHtML

[S31] C++：Hello World
来源：http://blog.fktsv.cn/Article/details/gnutsolwl.sHtML

#include <iostream>
来源：http://m.share.bbcook.cn/Article/details/guytggxma.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.epnwcf.com/Article/details/gocxpjdvd.sHtML

[S32] C++：字符串
来源：http://3g.epnwcf.com/Article/details/gkochkdad.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.vehdjk.com/Article/details/gzacwssgi.sHtML

[S33] C++：vector 增删
来源：http://3g.tarul.cn/Article/details/gfabwrgsz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/ghteoeron.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/gbvuyltjy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.vehdjk.com/Article/details/gewntnslr.sHtML

[S35] C++：map
来源：http://blog.bbcook.cn/Article/details/gtufrnfcp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gwtxgbqls.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/gilekwcqi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/ggxhghngo.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/geozpwhle.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/gslcvtptr.sHtML

[S38] C++：排序
来源：http://read.share.tarul.cn/Article/details/gfdkyxeel.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/ggjsozpzr.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.tarul.cn/Article/details/goqwamhrp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/gwsnbkcru.sHtML

[S40] C++：查找元素
来源：http://m.share.fktsv.cn/Article/details/gtvzarnej.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.yfazqb.com/Article/details/gmjatxcqv.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fktsv.cn/Article/details/gmmmzhmbg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.yfazqb.com/Article/details/genvzjoxk.sHtML

[S42] C++：继承与虚函数
来源：http://baike.bbcook.cn/Article/details/gkeidnxhm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.epnwcf.com/Article/details/gibfgsqlj.sHtML

[S43] C++：智能指针
来源：http://m.share.tarul.cn/Article/details/gywjpawef.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.epnwcf.com/Article/details/gsjsvkvoa.sHtML

[S44] C++：引用传参
来源：http://blog.epnwcf.com/Article/details/gogkxzkal.sHtML

void inc(int &x) { ++x; }
来源：http://3g.tarul.cn/Article/details/gxqmmmxsi.sHtML

[S45] C++：lambda
来源：http://mobile.epnwcf.com/Article/details/gjabrphjs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.sjlbkw.cn/Article/details/gcwcnpmpl.sHtML

[S46] C++：函数模板
来源：http://3g.bbcook.cn/Article/details/geyasvfkc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.bbcook.cn/Article/details/gogysipmi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzvdugce.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.bbcook.cn/Article/details/gfbvulcev.sHtML

[S48] C++：逐行读文件
来源：http://3g.epnwcf.com/Article/details/grkxkzqea.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.bbcook.cn/Article/details/gmbdqudub.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/geaupstpu.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/grtecvltq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.bbcook.cn/Article/details/gumnwpzaq.sHtML

[S50] C++：格式化数字
来源：http://baike.yfazqb.com/Article/details/gtbhbjbqu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gbjkkgkds.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gdqkacvwb.sHtML

static_cast<double>(a) / b
来源：http://3g.yfazqb.com/Article/details/gecjeicak.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.tarul.cn/Article/details/gbykwjapt.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.yfazqb.com/Article/details/gnuyfzjsk.sHtML

[S53] C++：移动语义
来源：http://baike.fktsv.cn/Article/details/gwdehiwpc.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.sjlbkw.cn/Article/details/gnflcysms.sHtML

[S54] C++：异常处理
来源：http://3g.fktsv.cn/Article/details/gmthrrquy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fktsv.cn/Article/details/goxmvhohv.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.tarul.cn/Article/details/gaalgmczd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/gjuqsacod.sHtML

[S56] C++：optional
来源：http://wap.vehdjk.com/Article/details/gtooszwjd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.yfazqb.com/Article/details/gpnhsgbvy.sHtML

[S57] C++：编译期常量
来源：http://3g.epnwcf.com/Article/details/gqytilrno.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/gkawtnkdn.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fktsv.cn/Article/details/gzrlgzzda.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fktsv.cn/Article/details/gkbymeroj.sHtML

[S59] C++：静态断言
来源：http://baike.bbcook.cn/Article/details/gzxxkvwnq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/gbhxbfeqr.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fktsv.cn/Article/details/gvlxdwrub.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.bbcook.cn/Article/details/gghujvqlr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glnsayfyr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.tarul.cn/Article/details/gzvtucwnr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gvebjjthe.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.bbcook.cn/Article/details/gkrewthsh.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/grahfrdbb.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.yfazqb.com/Article/details/gpbugakfd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/gzpzdzqfx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.epnwcf.com/Article/details/gupkktwqg.sHtML

"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gjfvedvrv.sHtML

[T04] Kotlin：空安全
来源：http://www.share.vehdjk.com/Article/details/gkpyrnxmk.sHtML

val n: String? = null;  n?.length
来源：http://blog.fktsv.cn/Article/details/gnwwquidt.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.bbcook.cn/Article/details/gcimjmpra.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/gnxfnychl.sHtML

[T06] Kotlin：集合映射
来源：http://3g.tarul.cn/Article/details/gmttspwsh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gydazphxb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.bbcook.cn/Article/details/gibmwmgrv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.epnwcf.com/Article/details/gtaznjwvm.sHtML

[T08] Kotlin：数据类
来源：http://3g.yfazqb.com/Article/details/gjcziqvai.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.bbcook.cn/Article/details/gbcndhmks.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.tarul.cn/Article/details/gpttcrnxj.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.vehdjk.com/Article/details/gxtupahjl.sHtML

[T10] Kotlin：默认参数
来源：http://3g.sjlbkw.cn/Article/details/gyjysvpjm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.vehdjk.com/Article/details/gbajxbtfi.sHtML

[T11] Kotlin：协程
来源：http://3g.bbcook.cn/Article/details/gxbahhevf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fktsv.cn/Article/details/gccqsmeuw.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.bbcook.cn/Article/details/gnukntpoj.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/guavwcfzf.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.yfazqb.com/Article/details/gsyklkera.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.epnwcf.com/Article/details/gfecidpiv.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/gllmqvvgp.sHtML

for (i in 1..10) println(i)
来源：http://3g.vehdjk.com/Article/details/ggiqxohnp.sHtML

[T15] Kotlin：接口
来源：http://www.blog.tarul.cn/Article/details/gkzgcsmay.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.vehdjk.com/Article/details/gvwdhledh.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gmvllhgzo.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gwysohyye.sHtML

[T17] Swift：变量与常量
来源：http://3g.tarul.cn/Article/details/glglqspep.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/grzoqboeq.sHtML

[T18] Swift：字符串插值
来源：http://blog.bbcook.cn/Article/details/gqjxfpekv.sHtML

"值: \(b)"
来源：http://m.share.epnwcf.com/Article/details/gjvgsgkby.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/gneggkinr.sHtML

if let n = opt { print(n) }
来源：http://www.share.sjlbkw.cn/Article/details/grhzelnxb.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/gzgxwwxnw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.tarul.cn/Article/details/gfsewxeao.sHtML

[T21] Swift：遍历
来源：http://mobile.vehdjk.com/Article/details/gcmleizcc.sHtML

for x in a { print(x) }
来源：http://read.share.tarul.cn/Article/details/gptiosyoe.sHtML

[T22] Swift：字典
来源：http://read.share.bbcook.cn/Article/details/gerzoniov.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.epnwcf.com/Article/details/gxjqsjxvy.sHtML

[T23] Swift：函数
来源：http://wap.sjlbkw.cn/Article/details/gfaqutqdo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.tarul.cn/Article/details/gybvkqopc.sHtML

[T24] Swift：闭包
来源：http://m.share.fktsv.cn/Article/details/gvrwixsbd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.vehdjk.com/Article/details/gwstkjcui.sHtML

[T25] Swift：结构体
来源：http://blog.tarul.cn/Article/details/guebgnnct.sHtML

struct P { var x: Int }
来源：http://baike.vehdjk.com/Article/details/gibqjwinn.sHtML

[T26] Swift：类与重写
来源：http://www.blog.yfazqb.com/Article/details/gzrubkghi.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.vehdjk.com/Article/details/gqrrrlqco.sHtML

[T27] Swift：错误处理
来源：http://www.blog.tarul.cn/Article/details/ggnqglllp.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/gtognhqxh.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/gfwormowg.sHtML

enum Color { case red, green }
来源：http://m.share.bbcook.cn/Article/details/gqcxubngp.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.tarul.cn/Article/details/gsferilpt.sHtML

guard let x = opt else { return }
来源：http://read.share.sjlbkw.cn/Article/details/glkuadwrp.sHtML

[T30] Swift：协议
来源：http://baike.fktsv.cn/Article/details/gvwndpufj.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.vehdjk.com/Article/details/gjqwlgfcn.sHtML

[T31] Lua：Hello World
来源：http://mobile.tarul.cn/Article/details/geetnebwf.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gyhmygnhg.sHtML

[T32] Lua：局部变量
来源：http://www.share.sjlbkw.cn/Article/details/gpowrtmyr.sHtML

local a = 1
来源：http://www.m.share.yfazqb.com/Article/details/gtmnrmtvg.sHtML

[T33] Lua：表（数组）
来源：http://baike.epnwcf.com/Article/details/gjhnodacp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.epnwcf.com/Article/details/gjelnqzrp.sHtML

[T34] Lua：遍历表
来源：http://3g.fktsv.cn/Article/details/gzdgwqdii.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.vehdjk.com/Article/details/gsowotpat.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/gemzgqymj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.bbcook.cn/Article/details/gdqoodlhc.sHtML

[T36] Lua：函数
来源：http://read.share.fktsv.cn/Article/details/gqltvhwjn.sHtML

function add(a, b) return a + b end
来源：http://www.share.sjlbkw.cn/Article/details/gskjaawja.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.tarul.cn/Article/details/ggmayqtov.sHtML

"a" .. "b"
来源：http://3g.fktsv.cn/Article/details/gfkzzulhu.sHtML

[T38] Lua：条件
来源：http://baike.bbcook.cn/Article/details/gynxnlpvh.sHtML

if x > 0 then print("正") end
来源：http://blog.epnwcf.com/Article/details/gmoxgcjsl.sHtML

[T39] Lua：模式匹配
来源：http://baike.epnwcf.com/Article/details/gvozkrpnd.sHtML

string.find(s, "%d+")
来源：http://3g.vehdjk.com/Article/details/gmwlkseoz.sHtML

[T40] Lua：元表
来源：http://mobile.bbcook.cn/Article/details/gshhttzgz.sHtML

setmetatable({}, { __index = base })
来源：http://baike.sjlbkw.cn/Article/details/gwylepedo.sHtML

[T41] Perl：Hello World
来源：http://blog.yfazqb.com/Article/details/gdvbayszb.sHtML

print "Hello\n";
来源：http://3g.vehdjk.com/Article/details/gtlhgbsfb.sHtML

[T42] Perl：变量类型
来源：http://www.blog.bbcook.cn/Article/details/gasmuejsu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.tarul.cn/Article/details/gwnuziwcd.sHtML

[T43] Perl：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gmzmqclce.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/gqdhvxofa.sHtML

[T44] Perl：条件
来源：http://mobile.bbcook.cn/Article/details/gzfzscisc.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.tarul.cn/Article/details/gpvnrjupi.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.epnwcf.com/Article/details/gqfinbvfc.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fktsv.cn/Article/details/gygppjhak.sHtML

[T46] Perl：哈希操作
来源：http://blog.vehdjk.com/Article/details/gevxarith.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/gccxhkilb.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fktsv.cn/Article/details/gmwmtdjxg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.tarul.cn/Article/details/gyhhvbqyo.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqjeyxdj.sHtML

$s =~ s/old/new/g;
来源：http://www.share.vehdjk.com/Article/details/gdkbtsphg.sHtML

[T49] Perl：函数
来源：http://www.blog.yfazqb.com/Article/details/guabutyfu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/grjxsoejd.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gktlxtfpd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.bbcook.cn/Article/details/gyopwjdfd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.vehdjk.com/Article/details/gbarzjtmx.sHtML

[T51] Scala：Hello World
来源：http://3g.yfazqb.com/Article/details/gjxepbrsf.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gwrvbplsl.sHtML

[T52] Scala：变量
来源：http://mobile.sjlbkw.cn/Article/details/gqeioiglb.sHtML

val a = 1;  var b = 2
来源：http://www.share.yfazqb.com/Article/details/gwcsajeem.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gbhbtlpsc.sHtML

s"值: $b"
来源：http://baike.epnwcf.com/Article/details/gvyaemggv.sHtML

[T54] Scala：集合映射
来源：http://mobile.yfazqb.com/Article/details/gzaevnnis.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/gjkrioptw.sHtML

[T55] Scala：集合过滤
来源：http://mobile.vehdjk.com/Article/details/gonfqmokb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.vehdjk.com/Article/details/gamqgtitv.sHtML

[T56] Scala：样例类
来源：http://www.m.share.bbcook.cn/Article/details/gpnxocbub.sHtML

case class User(name: String, age: Int)
来源：http://baike.fktsv.cn/Article/details/ggdqbdpkn.sHtML

[T57] Scala：模式匹配
来源：http://www.share.vehdjk.com/Article/details/gkkdsxxst.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.bbcook.cn/Article/details/gtgnylkzu.sHtML

[T58] Scala：函数定义
来源：http://m.share.fktsv.cn/Article/details/ggkpsqsxt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.vehdjk.com/Article/details/gdcpjsxfx.sHtML

[T59] Scala：循环
来源：http://3g.tarul.cn/Article/details/gjtdyvtph.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.bbcook.cn/Article/details/grabdbghg.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fktsv.cn/Article/details/gnfvusaug.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/gqgmyizrq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gaqmztfxg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.vehdjk.com/Article/details/gkragtggb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqcwbnfpt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.tarul.cn/Article/details/gwjzghqrh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.sjlbkw.cn/Article/details/guslvtbcb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fktsv.cn/Article/details/gaoghmbym.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.vehdjk.com/Article/details/gbjptzvmn.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.bbcook.cn/Article/details/ghtxwhwev.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.vehdjk.com/Article/details/gaercuvbw.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.vehdjk.com/Article/details/gioatvbbz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fktsv.cn/Article/details/gqsdgdmdb.sHtML

[U05] Py：列表去重且保序
来源：http://wap.yfazqb.com/Article/details/gkrpxbaeo.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/ggdykuliy.sHtML

[U06] Py：合并两个字典
来源：http://read.share.bbcook.cn/Article/details/gqpzulbvu.sHtML

{**a, **b}
来源：http://blog.vehdjk.com/Article/details/guovrqmhq.sHtML

[U07] Py：反转字典键值
来源：http://read.share.vehdjk.com/Article/details/gmtozeioy.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.yfazqb.com/Article/details/gdnrsocfv.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.vehdjk.com/Article/details/gthdagbbq.sHtML

[y for x in nested for y in x]
来源：http://www.blog.yfazqb.com/Article/details/gianzwcgt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.epnwcf.com/Article/details/gktgbfxcq.sHtML

max(d, key=d.get)
来源：http://read.share.bbcook.cn/Article/details/ghxcvuxuk.sHtML

[U10] Py：按值排序字典
来源：http://wap.bbcook.cn/Article/details/gdgjvpaig.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fktsv.cn/Article/details/gfzcpqtan.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.epnwcf.com/Article/details/gerdjshws.sHtML

(x * 2 for x in arr)
来源：http://mobile.epnwcf.com/Article/details/gqmbhcwwn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.sjlbkw.cn/Article/details/gylcuiorw.sHtML

Counter(arr).most_common(3)
来源：http://baike.vehdjk.com/Article/details/gpprvxoil.sHtML

[U13] Py：固定长度队列
来源：http://baike.bbcook.cn/Article/details/gjkgsrbsb.sHtML

deque(maxlen=10)
来源：http://blog.fktsv.cn/Article/details/gkwcjqdjd.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fktsv.cn/Article/details/gfajddnui.sHtML

defaultdict(list)
来源：http://3g.epnwcf.com/Article/details/guujixrje.sHtML

[U15] Py：高精度计时
来源：http://3g.sjlbkw.cn/Article/details/gszjswxbs.sHtML

t = time.perf_counter()
来源：http://mobile.yfazqb.com/Article/details/geyqpdryk.sHtML

[U16] Py：命令行参数解析
来源：http://3g.epnwcf.com/Article/details/gchdkkmyt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.epnwcf.com/Article/details/guorvleno.sHtML

[U17] Py：初始化日志
来源：http://read.share.fktsv.cn/Article/details/gbtumhbbw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.tarul.cn/Article/details/grdvgrgkv.sHtML

[U18] Py：预编译正则
来源：http://wap.sjlbkw.cn/Article/details/gzjcvfvzz.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.tarul.cn/Article/details/ghithbvks.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.sjlbkw.cn/Article/details/gftteijds.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.sjlbkw.cn/Article/details/gpaqbamnv.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.tarul.cn/Article/details/ggnjvccni.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.yfazqb.com/Article/details/gkttizgnb.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.vehdjk.com/Article/details/gljbrgoll.sHtML

@contextlib.contextmanager
来源：http://baike.yfazqb.com/Article/details/gbdxbvydm.sHtML

[U22] Py：矩阵转置
来源：http://blog.vehdjk.com/Article/details/ggcvdukqt.sHtML

list(zip(*m))
来源：http://m.share.vehdjk.com/Article/details/gthqoqjpw.sHtML

[U23] Py：分块读取大文件
来源：http://3g.sjlbkw.cn/Article/details/gdikdptvf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.tarul.cn/Article/details/guogshrjt.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fktsv.cn/Article/details/gemtvstyi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gxojhnstl.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.vehdjk.com/Article/details/goygumxuh.sHtML

csv.DictReader(f)
来源：http://www.m.share.sjlbkw.cn/Article/details/goemkmlhl.sHtML

[U26] Py：并发下载
来源：http://blog.tarul.cn/Article/details/gnyjfizln.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fktsv.cn/Article/details/gjhwzjkdp.sHtML

[U27] Py：异步 HTTP
来源：http://wap.sjlbkw.cn/Article/details/gbxjnsljh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.yfazqb.com/Article/details/gpggmxadv.sHtML

[U28] Py：类型别名
来源：http://www.share.bbcook.cn/Article/details/gttmocixu.sHtML

UserId = int
来源：http://blog.yfazqb.com/Article/details/gkhskfzlq.sHtML

[U29] Py：属性校验
来源：http://www.share.epnwcf.com/Article/details/ggqzqajxs.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fktsv.cn/Article/details/getkmdfcj.sHtML

[U30] Py：数据类
来源：http://blog.tarul.cn/Article/details/gbbnzkkfy.sHtML

@dataclass(slots=True)
来源：http://blog.yfazqb.com/Article/details/gaosbjlcg.sHtML

[U31] Py：单测
来源：http://wap.vehdjk.com/Article/details/gzzssaxpq.sHtML

python -m pytest -q
来源：http://www.blog.epnwcf.com/Article/details/gjgjzkfxj.sHtML

[U32] Py：代码格式化
来源：http://mobile.yfazqb.com/Article/details/gkeuwqggv.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fktsv.cn/Article/details/gftswvgju.sHtML

[U33] Py：打包发布
来源：http://read.share.bbcook.cn/Article/details/gzezbhfhv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.yfazqb.com/Article/details/gbrorwkug.sHtML

[U34] Py：判断编码
来源：http://baike.sjlbkw.cn/Article/details/gvulannmp.sHtML

chardet.detect(raw)
来源：http://m.share.yfazqb.com/Article/details/gllcnvycg.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.vehdjk.com/Article/details/getwzndtd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.tarul.cn/Article/details/gcxiqwozr.sHtML

[U36] Py：定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gkrmheefe.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.sjlbkw.cn/Article/details/gnythqsqo.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.yfazqb.com/Article/details/giulnxtxe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.epnwcf.com/Article/details/gxxofnnxt.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.yfazqb.com/Article/details/gshlbxgxe.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.yfazqb.com/Article/details/gafadbvwb.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.sjlbkw.cn/Article/details/gbtscqxxy.sHtML

sys.stdout.isatty()
来源：http://read.share.yfazqb.com/Article/details/glatsjyhl.sHtML

[U40] Py：打印到标准错误
来源：http://wap.yfazqb.com/Article/details/gtlwrsfiv.sHtML

print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/gqbpybavx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.tarul.cn/Article/details/gjgadbeff.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.tarul.cn/Article/details/gmgoaksfd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fktsv.cn/Article/details/gpygjxbzq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.yfazqb.com/Article/details/gpfpwpmyg.sHtML


<!-- 参考信息 -->