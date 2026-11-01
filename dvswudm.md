代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://wap.yfazqb.com/Article/details/gsvrnikcb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.yfazqb.com/Article/details/gfqyuydkp.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gchsgrmeb.sHtML

[S12] C：写文件
来源：http://blog.epnwcf.com/Article/details/gwpmyfvlg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/grkqwcxdb.sHtML

[S13] C：宏定义
来源：http://blog.tarul.cn/Article/details/gnoyffekt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.sjlbkw.cn/Article/details/gkqanusul.sHtML

[S14] C：枚举
来源：http://blog.epnwcf.com/Article/details/gdycshkea.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fktsv.cn/Article/details/gdqfgphge.sHtML

[S15] C：类型转换
来源：http://3g.tarul.cn/Article/details/gmmdsrbzx.sHtML

(double) a / b
来源：http://www.blog.vehdjk.com/Article/details/gkybpcboh.sHtML

[S16] C：位操作置位
来源：http://m.share.yfazqb.com/Article/details/gsqubxvjm.sHtML

x |= (1 << 3);
来源：http://www.share.sjlbkw.cn/Article/details/gxnqifzra.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gkoqcpnyj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.bbcook.cn/Article/details/gerxxalgs.sHtML

[S18] C：命令行参数
来源：http://www.blog.yfazqb.com/Article/details/grrkgbfgv.sHtML

int main(int argc, char **argv)
来源：http://blog.tarul.cn/Article/details/gmhwhldzw.sHtML

[S19] C：快速排序
来源：http://www.share.sjlbkw.cn/Article/details/grkfpyloj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gwtcygnep.sHtML

[S20] C：二分查找
来源：http://blog.tarul.cn/Article/details/gjjglmxwx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gulvdrvdn.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/grvftaoej.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.tarul.cn/Article/details/gjlqkmhqt.sHtML

[S22] C：字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gdfcpjeaa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.epnwcf.com/Article/details/gslpdlocx.sHtML

[S23] C：随机数
来源：http://mobile.epnwcf.com/Article/details/gixkspwpr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/gidhcjveb.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/gxweqvyuq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fktsv.cn/Article/details/ggqazvlqe.sHtML

[S25] C：内存拷贝
来源：http://read.share.bbcook.cn/Article/details/ggqdgevqx.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/gynpjkpkm.sHtML

[S26] C：内存清零
来源：http://3g.bbcook.cn/Article/details/getwcsmfs.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/ghkoaesjc.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/gfjrhqbhg.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gbzlabsnt.sHtML

[S28] C：静态变量
来源：http://wap.sjlbkw.cn/Article/details/gqbggzjqh.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/glsqorlak.sHtML

[S29] C：变参函数
来源：http://blog.vehdjk.com/Article/details/gxenieplo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/gtmbtqitu.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fktsv.cn/Article/details/ggegxhwvv.sHtML

#ifndef X_H
来源：http://read.share.bbcook.cn/Article/details/gbzomthsa.sHtML

#define X_H
来源：http://baike.fktsv.cn/Article/details/gmaizjzui.sHtML

#endif
来源：http://blog.epnwcf.com/Article/details/gyvepljlp.sHtML

[S31] C++：Hello World
来源：http://m.share.vehdjk.com/Article/details/gmpfglboy.sHtML

#include <iostream>
来源：http://mobile.fktsv.cn/Article/details/gewmklwjc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.epnwcf.com/Article/details/gokpgvjie.sHtML

[S32] C++：字符串
来源：http://3g.tarul.cn/Article/details/gjtiwowvs.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.bbcook.cn/Article/details/gemgxoofy.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/gzqfkcycf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/glqkxmwpv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/gptboltxi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gjzqucqka.sHtML

[S35] C++：map
来源：http://baike.vehdjk.com/Article/details/gmnwbspkw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gdcvwjsvb.sHtML

[S36] C++：unordered_map
来源：http://wap.tarul.cn/Article/details/gitklnlqa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gzlsmyzjg.sHtML

[S37] C++：set
来源：http://www.m.share.sjlbkw.cn/Article/details/gxofadfuf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gizimdran.sHtML

[S38] C++：排序
来源：http://read.share.bbcook.cn/Article/details/gdviuyntm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gacoxxqob.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fktsv.cn/Article/details/gsfnibhmm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.epnwcf.com/Article/details/gyqstsmpd.sHtML

[S40] C++：查找元素
来源：http://read.share.yfazqb.com/Article/details/grehqwziz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/gvvpaqmqt.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/gdhciuyez.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/ghntjkefc.sHtML

[S42] C++：继承与虚函数
来源：http://wap.tarul.cn/Article/details/gmqqfihyw.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.vehdjk.com/Article/details/ggiimiynx.sHtML

[S43] C++：智能指针
来源：http://read.share.sjlbkw.cn/Article/details/ggpzzhqqh.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fktsv.cn/Article/details/gmyggocpn.sHtML

[S44] C++：引用传参
来源：http://3g.fktsv.cn/Article/details/gxqvtygsp.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/gpyyaoikb.sHtML

[S45] C++：lambda
来源：http://www.blog.epnwcf.com/Article/details/gyzkcdpas.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fktsv.cn/Article/details/gbrxjvori.sHtML

[S46] C++：函数模板
来源：http://m.share.fktsv.cn/Article/details/gdjysxgis.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.bbcook.cn/Article/details/ghckgklil.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.bbcook.cn/Article/details/gkvjczizv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.epnwcf.com/Article/details/gdprkzxtz.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gnnqxdyno.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/glwjhjluk.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gfmihdogh.sHtML

[S49] C++：写文件
来源：http://baike.bbcook.cn/Article/details/ghsrrditq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.yfazqb.com/Article/details/gpiyfbdyy.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/gdpoyvpgi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gcfvyvoks.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/gqgyxyauz.sHtML

static_cast<double>(a) / b
来源：http://www.share.yfazqb.com/Article/details/gavlzzvki.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.yfazqb.com/Article/details/gdltvczlk.sHtML

int size() const noexcept { return n_; }
来源：http://blog.vehdjk.com/Article/details/gothfvwhf.sHtML

[S53] C++：移动语义
来源：http://blog.epnwcf.com/Article/details/grwetkzia.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.yfazqb.com/Article/details/geihuykdj.sHtML

[S54] C++：异常处理
来源：http://3g.sjlbkw.cn/Article/details/gvcbejnhb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.epnwcf.com/Article/details/gkifhryhl.sHtML

[S55] C++：结构化绑定
来源：http://3g.tarul.cn/Article/details/gcwyeaxvc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.vehdjk.com/Article/details/gahzsmahr.sHtML

[S56] C++：optional
来源：http://blog.sjlbkw.cn/Article/details/gamrqiotu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.tarul.cn/Article/details/glazegbud.sHtML

[S57] C++：编译期常量
来源：http://mobile.tarul.cn/Article/details/gspfqcjji.sHtML

constexpr int N = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gfzxzxnbk.sHtML

[S58] C++：命名空间
来源：http://read.share.tarul.cn/Article/details/gvvjsfuzg.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.sjlbkw.cn/Article/details/gviajtchr.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gjeqemyaf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.tarul.cn/Article/details/gerfdrmui.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.tarul.cn/Article/details/ghcvcfiiv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.tarul.cn/Article/details/gicovncds.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggukjpuvw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.yfazqb.com/Article/details/gcqvmgsic.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsmignhit.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fktsv.cn/Article/details/gufflhudb.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gcvprxsdi.sHtML

[T02] Kotlin：变量
来源：http://read.share.yfazqb.com/Article/details/gibnswngy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.tarul.cn/Article/details/gchlwxbiu.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.sjlbkw.cn/Article/details/gtihrgepq.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/gavnxdxtu.sHtML

[T04] Kotlin：空安全
来源：http://baike.fktsv.cn/Article/details/gucpdbflk.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/ghaofudek.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.bbcook.cn/Article/details/gukurkoiz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.bbcook.cn/Article/details/gdpooaxrf.sHtML

[T06] Kotlin：集合映射
来源：http://wap.tarul.cn/Article/details/gtcdujxzc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/gineskcbf.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.epnwcf.com/Article/details/gclbntlno.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fktsv.cn/Article/details/gcqkjcgeq.sHtML

[T08] Kotlin：数据类
来源：http://baike.epnwcf.com/Article/details/ghonvjqag.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.tarul.cn/Article/details/gahahplzn.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.yfazqb.com/Article/details/gjhxyjmto.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fktsv.cn/Article/details/gqlhpfdhs.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.sjlbkw.cn/Article/details/ggcjksmds.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.tarul.cn/Article/details/gxoukpsyy.sHtML

[T11] Kotlin：协程
来源：http://www.share.yfazqb.com/Article/details/ggztiimhx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.vehdjk.com/Article/details/guudrrstk.sHtML

[T12] Kotlin：解构声明
来源：http://3g.sjlbkw.cn/Article/details/gcpitxhzn.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.yfazqb.com/Article/details/ggavozxmn.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.epnwcf.com/Article/details/grifnujbk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.bbcook.cn/Article/details/gpciiqhuw.sHtML

[T14] Kotlin：循环
来源：http://baike.vehdjk.com/Article/details/gzsfvkhkt.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/gazyuxrdv.sHtML

[T15] Kotlin：接口
来源：http://www.share.vehdjk.com/Article/details/gsposzujh.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gxwxauphg.sHtML

[T16] Swift：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gwkjhcejp.sHtML

print("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gozwpvzuv.sHtML

[T17] Swift：变量与常量
来源：http://3g.fktsv.cn/Article/details/gpdtqavcf.sHtML

var a = 1;  let b = 2
来源：http://read.share.yfazqb.com/Article/details/gpebynjzc.sHtML

[T18] Swift：字符串插值
来源：http://baike.vehdjk.com/Article/details/gjwhiqedi.sHtML

"值: \(b)"
来源：http://baike.vehdjk.com/Article/details/gzijbufsr.sHtML

[T19] Swift：可选绑定
来源：http://baike.fktsv.cn/Article/details/guvlotjwp.sHtML

if let n = opt { print(n) }
来源：http://mobile.sjlbkw.cn/Article/details/gwmndnofd.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/gcbyoqtza.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.sjlbkw.cn/Article/details/gowpkxfxk.sHtML

[T21] Swift：遍历
来源：http://m.share.tarul.cn/Article/details/ggjmjzobx.sHtML

for x in a { print(x) }
来源：http://baike.bbcook.cn/Article/details/gowhsoxou.sHtML

[T22] Swift：字典
来源：http://www.m.share.fktsv.cn/Article/details/gcluvvjbj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.bbcook.cn/Article/details/gktnqhgjp.sHtML

[T23] Swift：函数
来源：http://blog.sjlbkw.cn/Article/details/glpvzynty.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.epnwcf.com/Article/details/guhnjozlf.sHtML

[T24] Swift：闭包
来源：http://3g.tarul.cn/Article/details/guncxhlqp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.vehdjk.com/Article/details/gkatwjaeg.sHtML

[T25] Swift：结构体
来源：http://baike.bbcook.cn/Article/details/gcljaxdck.sHtML

struct P { var x: Int }
来源：http://read.share.fktsv.cn/Article/details/gjuriajew.sHtML

[T26] Swift：类与重写
来源：http://blog.epnwcf.com/Article/details/gfejppggm.sHtML

class A: Base { override func f() {} }
来源：http://www.share.epnwcf.com/Article/details/gjsvfobim.sHtML

[T27] Swift：错误处理
来源：http://www.share.bbcook.cn/Article/details/gcpwlbvbk.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.sjlbkw.cn/Article/details/ggjrmdegb.sHtML

[T28] Swift：枚举
来源：http://blog.vehdjk.com/Article/details/gpjlqyovl.sHtML

enum Color { case red, green }
来源：http://3g.vehdjk.com/Article/details/gsvnutquw.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/ggigmeppm.sHtML

guard let x = opt else { return }
来源：http://read.share.tarul.cn/Article/details/gsymzmmhv.sHtML

[T30] Swift：协议
来源：http://3g.tarul.cn/Article/details/gqftrldns.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fktsv.cn/Article/details/gekuhcjhg.sHtML

[T31] Lua：Hello World
来源：http://read.share.bbcook.cn/Article/details/gpyvtnodj.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/gkcjvomdz.sHtML

[T32] Lua：局部变量
来源：http://mobile.yfazqb.com/Article/details/ginzitpho.sHtML

local a = 1
来源：http://mobile.epnwcf.com/Article/details/gxrblxwar.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.vehdjk.com/Article/details/glkhcgqoa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fktsv.cn/Article/details/ggvdfemhx.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.yfazqb.com/Article/details/gelzhstux.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.bbcook.cn/Article/details/gqmfbpzvt.sHtML

[T35] Lua：字典表
来源：http://www.blog.yfazqb.com/Article/details/grfapisyw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.yfazqb.com/Article/details/garjbngcy.sHtML

[T36] Lua：函数
来源：http://mobile.fktsv.cn/Article/details/gpbcashjx.sHtML

function add(a, b) return a + b end
来源：http://mobile.epnwcf.com/Article/details/gzydsyimg.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gtksxmzoc.sHtML

"a" .. "b"
来源：http://www.share.fktsv.cn/Article/details/gnyruvqro.sHtML

[T38] Lua：条件
来源：http://www.blog.tarul.cn/Article/details/gczftjejr.sHtML

if x > 0 then print("正") end
来源：http://m.share.tarul.cn/Article/details/geyjmnrmc.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gciqlshek.sHtML

string.find(s, "%d+")
来源：http://mobile.bbcook.cn/Article/details/gecnwoxlx.sHtML

[T40] Lua：元表
来源：http://www.share.yfazqb.com/Article/details/gczfiwuxk.sHtML

setmetatable({}, { __index = base })
来源：http://wap.epnwcf.com/Article/details/gkxcsetrm.sHtML

[T41] Perl：Hello World
来源：http://wap.yfazqb.com/Article/details/gmfxrzfcw.sHtML

print "Hello\n";
来源：http://m.share.sjlbkw.cn/Article/details/giixwrpgu.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gagujarwc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fktsv.cn/Article/details/gdhonebpq.sHtML

[T43] Perl：字符串插值
来源：http://wap.vehdjk.com/Article/details/gdimnyrlu.sHtML

"值: $a"
来源：http://read.share.tarul.cn/Article/details/gfvsobsdy.sHtML

[T44] Perl：条件
来源：http://wap.fktsv.cn/Article/details/glwpyohpa.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaiqxmibp.sHtML

[T45] Perl：数组遍历
来源：http://www.share.bbcook.cn/Article/details/gapktrjjy.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fktsv.cn/Article/details/gfpknwytm.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fktsv.cn/Article/details/grvfjwmor.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.bbcook.cn/Article/details/ghxwnjqih.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fktsv.cn/Article/details/gipponptm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fktsv.cn/Article/details/ghrqkzlci.sHtML

[T48] Perl：正则替换
来源：http://wap.vehdjk.com/Article/details/gawvcoive.sHtML

$s =~ s/old/new/g;
来源：http://3g.tarul.cn/Article/details/gfiyhnlwr.sHtML

[T49] Perl：函数
来源：http://wap.yfazqb.com/Article/details/gvmpvzrma.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/ggiyvmiob.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/guhkmjewh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.bbcook.cn/Article/details/gmaduqbfd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.sjlbkw.cn/Article/details/gyuhymybv.sHtML

[T51] Scala：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gnkyjcclk.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gbjjkrdxl.sHtML

[T52] Scala：变量
来源：http://mobile.bbcook.cn/Article/details/glquerexw.sHtML

val a = 1;  var b = 2
来源：http://m.share.tarul.cn/Article/details/gbatymmzd.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/glvrkonrr.sHtML

s"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/gkyohygfe.sHtML

[T54] Scala：集合映射
来源：http://www.share.epnwcf.com/Article/details/gbhqzaldi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.yfazqb.com/Article/details/gxjekhavh.sHtML

[T55] Scala：集合过滤
来源：http://baike.tarul.cn/Article/details/gwtyeoang.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.epnwcf.com/Article/details/gnrbrjcvr.sHtML

[T56] Scala：样例类
来源：http://www.m.share.bbcook.cn/Article/details/gnndumogj.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gkjhcjmsz.sHtML

[T57] Scala：模式匹配
来源：http://baike.fktsv.cn/Article/details/gsaaoezkm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.yfazqb.com/Article/details/gomtnpdvf.sHtML

[T58] Scala：函数定义
来源：http://blog.sjlbkw.cn/Article/details/gvcsvcmae.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.epnwcf.com/Article/details/gzyqkqyqq.sHtML

[T59] Scala：循环
来源：http://blog.bbcook.cn/Article/details/gexptntyv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/ghverwtxi.sHtML

[T60] Scala：折叠
来源：http://www.blog.tarul.cn/Article/details/gsknuhgmy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.vehdjk.com/Article/details/gmrlffaus.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyvbqprwu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.bbcook.cn/Article/details/gnemxtgch.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwsdhscqf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fktsv.cn/Article/details/guilhfqmc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.bbcook.cn/Article/details/gwakeyuys.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fktsv.cn/Article/details/grvtjkwic.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.sjlbkw.cn/Article/details/gerswkaty.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.bbcook.cn/Article/details/gfqpvrbjv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.vehdjk.com/Article/details/gdibtvdqv.sHtML

[U04] Py：变量调试打印
来源：http://baike.fktsv.cn/Article/details/gfjoqklib.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.epnwcf.com/Article/details/gaxttaxta.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.bbcook.cn/Article/details/gdabhsfpd.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gkzudlgzr.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fktsv.cn/Article/details/gszoorbbh.sHtML

{**a, **b}
来源：http://read.share.fktsv.cn/Article/details/guuciwktl.sHtML

[U07] Py：反转字典键值
来源：http://baike.tarul.cn/Article/details/gmmuvhgmg.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.yfazqb.com/Article/details/gjykegvdu.sHtML

[U08] Py：展平二维列表
来源：http://baike.yfazqb.com/Article/details/glrzzzgly.sHtML

[y for x in nested for y in x]
来源：http://3g.yfazqb.com/Article/details/gfynfcqmd.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.epnwcf.com/Article/details/gstdzpusu.sHtML

max(d, key=d.get)
来源：http://mobile.sjlbkw.cn/Article/details/gsdvhqcsl.sHtML

[U10] Py：按值排序字典
来源：http://wap.fktsv.cn/Article/details/gytcxqzed.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.bbcook.cn/Article/details/gjzwqaqih.sHtML

[U11] Py：生成器表达式
来源：http://mobile.epnwcf.com/Article/details/gvoyqcctn.sHtML

(x * 2 for x in arr)
来源：http://m.share.sjlbkw.cn/Article/details/gpojxhjuf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.sjlbkw.cn/Article/details/ghlhgjkyv.sHtML

Counter(arr).most_common(3)
来源：http://m.share.tarul.cn/Article/details/guaivxfsw.sHtML

[U13] Py：固定长度队列
来源：http://3g.vehdjk.com/Article/details/gsvqznbkc.sHtML

deque(maxlen=10)
来源：http://read.share.yfazqb.com/Article/details/glzegyxxa.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.yfazqb.com/Article/details/gkrdzixnh.sHtML

defaultdict(list)
来源：http://read.share.yfazqb.com/Article/details/gembphcga.sHtML

[U15] Py：高精度计时
来源：http://mobile.vehdjk.com/Article/details/gsnlpkjzl.sHtML

t = time.perf_counter()
来源：http://mobile.yfazqb.com/Article/details/geruyfiuz.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.yfazqb.com/Article/details/geupnzeqo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.bbcook.cn/Article/details/geyufsdqi.sHtML

[U17] Py：初始化日志
来源：http://baike.yfazqb.com/Article/details/gytwodmuw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fktsv.cn/Article/details/grrjhdrwd.sHtML

[U18] Py：预编译正则
来源：http://blog.epnwcf.com/Article/details/gxawtbcst.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/ghsyxkrot.sHtML

[U19] Py：正则替换带回调
来源：http://baike.bbcook.cn/Article/details/glstcdypr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fktsv.cn/Article/details/gwxfwcprc.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.yfazqb.com/Article/details/gthrhhpdw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fktsv.cn/Article/details/gmbmljxbm.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.epnwcf.com/Article/details/gqevalxqa.sHtML

@contextlib.contextmanager
来源：http://www.blog.bbcook.cn/Article/details/gdbhulivr.sHtML

[U22] Py：矩阵转置
来源：http://read.share.yfazqb.com/Article/details/gzehjdgqt.sHtML

list(zip(*m))
来源：http://3g.sjlbkw.cn/Article/details/guyiahuhy.sHtML

[U23] Py：分块读取大文件
来源：http://baike.epnwcf.com/Article/details/gjadbxdde.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.tarul.cn/Article/details/gdztgukwv.sHtML

[U24] Py：路径操作
来源：http://mobile.tarul.cn/Article/details/gjqzzzibv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fktsv.cn/Article/details/ghsdtpydx.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fktsv.cn/Article/details/gitpvyjec.sHtML

csv.DictReader(f)
来源：http://blog.yfazqb.com/Article/details/gzqbjiviw.sHtML

[U26] Py：并发下载
来源：http://read.share.sjlbkw.cn/Article/details/ghpvgmtmx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fktsv.cn/Article/details/gjkspbamj.sHtML

[U27] Py：异步 HTTP
来源：http://3g.tarul.cn/Article/details/gxayzqrrw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.tarul.cn/Article/details/gczjmsohp.sHtML

[U28] Py：类型别名
来源：http://mobile.yfazqb.com/Article/details/gfqrzxtez.sHtML

UserId = int
来源：http://read.share.sjlbkw.cn/Article/details/gbubjzrmn.sHtML

[U29] Py：属性校验
来源：http://www.m.share.vehdjk.com/Article/details/gmdnkjzio.sHtML

@property 与 @x.setter 配合
来源：http://www.share.tarul.cn/Article/details/gyyucqncr.sHtML

[U30] Py：数据类
来源：http://mobile.epnwcf.com/Article/details/ghogzdxah.sHtML

@dataclass(slots=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqiwgmagy.sHtML

[U31] Py：单测
来源：http://www.m.share.yfazqb.com/Article/details/gqrauyoud.sHtML

python -m pytest -q
来源：http://www.share.tarul.cn/Article/details/gszmnokpr.sHtML

[U32] Py：代码格式化
来源：http://blog.vehdjk.com/Article/details/gvvezexbl.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.bbcook.cn/Article/details/gbpcxbjsb.sHtML

[U33] Py：打包发布
来源：http://read.share.sjlbkw.cn/Article/details/guppcccjl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.yfazqb.com/Article/details/gqqdyryjv.sHtML

[U34] Py：判断编码
来源：http://www.share.fktsv.cn/Article/details/garobqbzi.sHtML

chardet.detect(raw)
来源：http://3g.vehdjk.com/Article/details/gbrsxavrw.sHtML


<!-- 参考信息 -->