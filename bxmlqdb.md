代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.yfazqb.com/Article/details/gjhdezfzz.sHtML

[S10] C：指针与解引用
来源：http://blog.yfazqb.com/Article/details/gbcuqhitm.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/gxxgkdein.sHtML

[S11] C：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gufaiyqgj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fktsv.cn/Article/details/gqoscrqla.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.yfazqb.com/Article/details/gkuetkazd.sHtML

fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gcdpwnzlm.sHtML

[S12] C：写文件
来源：http://www.share.yfazqb.com/Article/details/gklmeqdhs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gvjqqimsq.sHtML

[S13] C：宏定义
来源：http://www.m.share.tarul.cn/Article/details/gzzlvtdyu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.epnwcf.com/Article/details/gqwrosxit.sHtML

[S14] C：枚举
来源：http://m.share.epnwcf.com/Article/details/gbvkyygwj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.sjlbkw.cn/Article/details/gebnwhpez.sHtML

[S15] C：类型转换
来源：http://m.share.yfazqb.com/Article/details/gngbbgitr.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/ggaczvnyx.sHtML

[S16] C：位操作置位
来源：http://blog.bbcook.cn/Article/details/gynviwiso.sHtML

x |= (1 << 3);
来源：http://mobile.bbcook.cn/Article/details/gjgyfroup.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gzljnniac.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.sjlbkw.cn/Article/details/gzkhcoace.sHtML

[S18] C：命令行参数
来源：http://www.share.fktsv.cn/Article/details/gxwiitppb.sHtML

int main(int argc, char **argv)
来源：http://mobile.bbcook.cn/Article/details/greyksfvo.sHtML

[S19] C：快速排序
来源：http://mobile.yfazqb.com/Article/details/gcdfwhgwe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gaafkfhjk.sHtML

[S20] C：二分查找
来源：http://www.m.share.tarul.cn/Article/details/gbhzywexp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gonzmkcwt.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjkglcsj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fktsv.cn/Article/details/gsalgbctt.sHtML

[S22] C：字符串转数字
来源：http://mobile.vehdjk.com/Article/details/gdrbvgxow.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fktsv.cn/Article/details/gfjesglml.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/gytjudvvd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.bbcook.cn/Article/details/gzpuotjls.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/ganuwccks.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fktsv.cn/Article/details/gksotimaq.sHtML

[S25] C：内存拷贝
来源：http://read.share.fktsv.cn/Article/details/gwowhavzn.sHtML

memcpy(dst, src, n);
来源：http://wap.tarul.cn/Article/details/gsleohwtu.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gedwkjxme.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/gvugkqgaz.sHtML

[S27] C：定义常量
来源：http://baike.yfazqb.com/Article/details/glpjfawme.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gfrtcqjce.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gflnyuwiu.sHtML

static int counter = 0;
来源：http://www.blog.sjlbkw.cn/Article/details/gsqzellad.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/goxanduan.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.tarul.cn/Article/details/gucvpeoju.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gujyjtqtl.sHtML

#ifndef X_H
来源：http://www.m.share.yfazqb.com/Article/details/gdnjpbyzj.sHtML

#define X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzxuwcpj.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gzrarhybl.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/glpemabff.sHtML

#include <iostream>
来源：http://blog.vehdjk.com/Article/details/gqkslmkin.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/gekkweqza.sHtML

[S32] C++：字符串
来源：http://blog.vehdjk.com/Article/details/gihqiysmo.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/gyleojgno.sHtML

[S33] C++：vector 增删
来源：http://www.share.tarul.cn/Article/details/gymstuzzs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.sjlbkw.cn/Article/details/gdgxcirmz.sHtML

[S34] C++：遍历 vector
来源：http://blog.epnwcf.com/Article/details/ghsckhise.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.sjlbkw.cn/Article/details/gsnijrzfs.sHtML

[S35] C++：map
来源：http://m.share.fktsv.cn/Article/details/gwedmggdu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gaukuzkyq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.tarul.cn/Article/details/gmpctmjft.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/grzjikzlm.sHtML

[S37] C++：set
来源：http://baike.tarul.cn/Article/details/gpdnrkhdo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gmikacctg.sHtML

[S38] C++：排序
来源：http://blog.bbcook.cn/Article/details/gwguiyanu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gzgmebdmm.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.bbcook.cn/Article/details/gacxfpigl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.vehdjk.com/Article/details/gnuypiall.sHtML

[S40] C++：查找元素
来源：http://baike.fktsv.cn/Article/details/gnlpdebls.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/gpmbegkcy.sHtML

[S41] C++：类与构造函数
来源：http://wap.bbcook.cn/Article/details/ghqbdllzt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.vehdjk.com/Article/details/gliepstii.sHtML

[S42] C++：继承与虚函数
来源：http://3g.bbcook.cn/Article/details/ghhuppjho.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.vehdjk.com/Article/details/gdhwgiagp.sHtML

[S43] C++：智能指针
来源：http://read.share.fktsv.cn/Article/details/gkhfcvjmo.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.vehdjk.com/Article/details/gbtukmqas.sHtML

[S44] C++：引用传参
来源：http://m.share.sjlbkw.cn/Article/details/giorxpcvv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfrwmdqff.sHtML

[S45] C++：lambda
来源：http://mobile.epnwcf.com/Article/details/grhwvpquh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/ghymormsn.sHtML

[S46] C++：函数模板
来源：http://wap.epnwcf.com/Article/details/gugfbpjyp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.epnwcf.com/Article/details/gfpoejjsh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.tarul.cn/Article/details/gcejcvvgg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gbralkybe.sHtML

[S48] C++：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gtgycngvp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.sjlbkw.cn/Article/details/gvdskqepn.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gjjwipxzp.sHtML

[S49] C++：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gffyclumh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/gwujoxtud.sHtML

[S50] C++：格式化数字
来源：http://3g.sjlbkw.cn/Article/details/gjwxfmfnt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.tarul.cn/Article/details/gmuqcvqql.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gwlzmuyix.sHtML

static_cast<double>(a) / b
来源：http://mobile.sjlbkw.cn/Article/details/gmaatsvqw.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.sjlbkw.cn/Article/details/grguwwitq.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.yfazqb.com/Article/details/gmsdkdirs.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/gihnqsreg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbljnfdhj.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/gvihlqkrr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.epnwcf.com/Article/details/gxsbfztmr.sHtML

[S55] C++：结构化绑定
来源：http://baike.epnwcf.com/Article/details/gyefhsyaf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.yfazqb.com/Article/details/gaiwsqvyq.sHtML

[S56] C++：optional
来源：http://mobile.fktsv.cn/Article/details/gocfycsxx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.sjlbkw.cn/Article/details/gpxblpevk.sHtML

[S57] C++：编译期常量
来源：http://read.share.yfazqb.com/Article/details/gkriymauw.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gfmfupyxe.sHtML

[S58] C++：命名空间
来源：http://www.share.vehdjk.com/Article/details/goorgsiys.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/glkqcfsbc.sHtML

[S59] C++：静态断言
来源：http://blog.vehdjk.com/Article/details/gtpqbtybl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/ghpxqzchr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.yfazqb.com/Article/details/gctbrhbxp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/gwlwuakgo.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbnccemqt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/gssraeiog.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdzqojbyf.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/glglombij.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/ggtzeaoer.sHtML

[T02] Kotlin：变量
来源：http://3g.fktsv.cn/Article/details/gaxhqbfdl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.vehdjk.com/Article/details/gnkdzrdts.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.sjlbkw.cn/Article/details/gdzcinnxi.sHtML

"值: $b"
来源：http://mobile.yfazqb.com/Article/details/gvoycrbey.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fktsv.cn/Article/details/glojlklzq.sHtML

val n: String? = null;  n?.length
来源：http://www.share.yfazqb.com/Article/details/gclqoiwdo.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.bbcook.cn/Article/details/grcdskpgy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.epnwcf.com/Article/details/guthsofgm.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fktsv.cn/Article/details/gbdmicspl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fktsv.cn/Article/details/gnvpjsouc.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/ghobcayfi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.tarul.cn/Article/details/gpkrzfqye.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.bbcook.cn/Article/details/gpbeyylxe.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.vehdjk.com/Article/details/gzjhwophb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.epnwcf.com/Article/details/gdpmeqfqv.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.epnwcf.com/Article/details/gktdnmabk.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.vehdjk.com/Article/details/gijwatcql.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.tarul.cn/Article/details/gljhivkdq.sHtML

[T11] Kotlin：协程
来源：http://blog.fktsv.cn/Article/details/gwqxqtfaj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.bbcook.cn/Article/details/ggjswhfof.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.bbcook.cn/Article/details/gctrypxut.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/ggzgundsw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.bbcook.cn/Article/details/gncdsfbhp.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/gtfqvplsy.sHtML

[T14] Kotlin：循环
来源：http://wap.tarul.cn/Article/details/glxrkuymo.sHtML

for (i in 1..10) println(i)
来源：http://www.share.yfazqb.com/Article/details/gsyrtjqcc.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.epnwcf.com/Article/details/gccwmifwq.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/ggglxptfp.sHtML

[T16] Swift：Hello World
来源：http://read.share.tarul.cn/Article/details/ghecdphzk.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gvqocqjkv.sHtML

[T17] Swift：变量与常量
来源：http://read.share.tarul.cn/Article/details/goosetzjn.sHtML

var a = 1;  let b = 2
来源：http://www.share.bbcook.cn/Article/details/gmrkhyanj.sHtML

[T18] Swift：字符串插值
来源：http://blog.yfazqb.com/Article/details/givdzylfu.sHtML

"值: \(b)"
来源：http://read.share.bbcook.cn/Article/details/gbwleqcqf.sHtML

[T19] Swift：可选绑定
来源：http://mobile.tarul.cn/Article/details/gzzgxbvrn.sHtML

if let n = opt { print(n) }
来源：http://baike.fktsv.cn/Article/details/gptqtoiyr.sHtML

[T20] Swift：数组操作
来源：http://mobile.fktsv.cn/Article/details/gwoibaczn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.epnwcf.com/Article/details/gipmkylie.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/gywuaxlze.sHtML

for x in a { print(x) }
来源：http://m.share.yfazqb.com/Article/details/gzsukbjwm.sHtML

[T22] Swift：字典
来源：http://baike.fktsv.cn/Article/details/goydrnyug.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.yfazqb.com/Article/details/gnfjbqujz.sHtML

[T23] Swift：函数
来源：http://www.m.share.tarul.cn/Article/details/gqetnnvxg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.tarul.cn/Article/details/gvoiunwvz.sHtML

[T24] Swift：闭包
来源：http://www.m.share.epnwcf.com/Article/details/gadhashwa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fktsv.cn/Article/details/guoqmiial.sHtML

[T25] Swift：结构体
来源：http://www.blog.fktsv.cn/Article/details/gujcovjtd.sHtML

struct P { var x: Int }
来源：http://read.share.bbcook.cn/Article/details/guhhabotb.sHtML

[T26] Swift：类与重写
来源：http://blog.vehdjk.com/Article/details/gqlfqzfdy.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.yfazqb.com/Article/details/gccaowsyl.sHtML

[T27] Swift：错误处理
来源：http://blog.vehdjk.com/Article/details/gagtxyhsj.sHtML

do { try f() } catch { print(error) }
来源：http://blog.tarul.cn/Article/details/gsqznbvcs.sHtML

[T28] Swift：枚举
来源：http://baike.tarul.cn/Article/details/gtktlsqep.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/ghvufiqxf.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/gqobahwie.sHtML

guard let x = opt else { return }
来源：http://wap.yfazqb.com/Article/details/gqmyjgera.sHtML

[T30] Swift：协议
来源：http://blog.vehdjk.com/Article/details/gmhziupig.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.yfazqb.com/Article/details/gfhpvaksi.sHtML

[T31] Lua：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gqyrgmdny.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gqkbcqjvt.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fktsv.cn/Article/details/gcpwnitxk.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/gnkivlyps.sHtML

[T33] Lua：表（数组）
来源：http://m.share.sjlbkw.cn/Article/details/gggurtgvd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.tarul.cn/Article/details/gxsozcfjb.sHtML

[T34] Lua：遍历表
来源：http://baike.tarul.cn/Article/details/gpwtssdbp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.tarul.cn/Article/details/gzhspwfiy.sHtML

[T35] Lua：字典表
来源：http://www.share.sjlbkw.cn/Article/details/gnrwecksw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.vehdjk.com/Article/details/gckztcrht.sHtML

[T36] Lua：函数
来源：http://3g.vehdjk.com/Article/details/ggqlnwmqm.sHtML

function add(a, b) return a + b end
来源：http://3g.tarul.cn/Article/details/gbosfycxg.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gijdaehrr.sHtML

"a" .. "b"
来源：http://read.share.sjlbkw.cn/Article/details/gqzubhoeo.sHtML

[T38] Lua：条件
来源：http://www.m.share.vehdjk.com/Article/details/glwongomu.sHtML

if x > 0 then print("正") end
来源：http://baike.sjlbkw.cn/Article/details/gvcnsnjpu.sHtML

[T39] Lua：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gcpsrzqfu.sHtML

string.find(s, "%d+")
来源：http://www.blog.yfazqb.com/Article/details/gthwyyeeg.sHtML

[T40] Lua：元表
来源：http://wap.vehdjk.com/Article/details/gmpiquoar.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.bbcook.cn/Article/details/gxntezcox.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/ggkcmnnpo.sHtML

print "Hello\n";
来源：http://3g.bbcook.cn/Article/details/geohedswd.sHtML

[T42] Perl：变量类型
来源：http://3g.sjlbkw.cn/Article/details/gdbpntern.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fktsv.cn/Article/details/glimmnvqz.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gnmtydhwf.sHtML

"值: $a"
来源：http://www.m.share.yfazqb.com/Article/details/gfbyupbrd.sHtML

[T44] Perl：条件
来源：http://read.share.tarul.cn/Article/details/getfmacmp.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.epnwcf.com/Article/details/gjcgdyskr.sHtML

[T45] Perl：数组遍历
来源：http://m.share.yfazqb.com/Article/details/gvenpdqew.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.vehdjk.com/Article/details/gcgqahbwj.sHtML

[T46] Perl：哈希操作
来源：http://baike.yfazqb.com/Article/details/gydorxbsm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.epnwcf.com/Article/details/gzkeskmzy.sHtML

[T47] Perl：正则捕获
来源：http://read.share.yfazqb.com/Article/details/gngcyowyr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.tarul.cn/Article/details/ggziybpnd.sHtML

[T48] Perl：正则替换
来源：http://mobile.fktsv.cn/Article/details/gbvrdamso.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.tarul.cn/Article/details/gfvmieqyx.sHtML

[T49] Perl：函数
来源：http://read.share.sjlbkw.cn/Article/details/glanfchwc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gaufcphxm.sHtML

[T50] Perl：逐行读文件
来源：http://wap.tarul.cn/Article/details/grnilalte.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.epnwcf.com/Article/details/gdrydmnzt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.yfazqb.com/Article/details/gqcwyqxfr.sHtML

[T51] Scala：Hello World
来源：http://blog.vehdjk.com/Article/details/gjqgmojnr.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/gxdaugbcr.sHtML

[T52] Scala：变量
来源：http://3g.yfazqb.com/Article/details/gbgnexgme.sHtML

val a = 1;  var b = 2
来源：http://m.share.yfazqb.com/Article/details/gumkjsxug.sHtML

[T53] Scala：字符串插值
来源：http://blog.bbcook.cn/Article/details/gibkbvkvx.sHtML

s"值: $b"
来源：http://baike.bbcook.cn/Article/details/gsolbyzjb.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.tarul.cn/Article/details/ggdhmnfkp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fktsv.cn/Article/details/gjgaswzqw.sHtML

[T55] Scala：集合过滤
来源：http://wap.yfazqb.com/Article/details/gstwzqjfw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.yfazqb.com/Article/details/gpwljkwra.sHtML

[T56] Scala：样例类
来源：http://wap.vehdjk.com/Article/details/getthheym.sHtML

case class User(name: String, age: Int)
来源：http://3g.fktsv.cn/Article/details/gzxbpsjab.sHtML

[T57] Scala：模式匹配
来源：http://www.share.tarul.cn/Article/details/gwylalvkb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.sjlbkw.cn/Article/details/gpeolxops.sHtML

[T58] Scala：函数定义
来源：http://www.share.sjlbkw.cn/Article/details/gjryeojcs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.sjlbkw.cn/Article/details/gdpsfclrk.sHtML

[T59] Scala：循环
来源：http://www.m.share.vehdjk.com/Article/details/gkwstziwl.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gdswtrujg.sHtML

[T60] Scala：折叠
来源：http://wap.vehdjk.com/Article/details/gtwkzskda.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fktsv.cn/Article/details/gnttcdbjw.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqenijmld.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/gcbbqhthj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxbusidyl.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.vehdjk.com/Article/details/gtngciiyx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.vehdjk.com/Article/details/gjsrenqcz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.tarul.cn/Article/details/gbcjuefaq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.vehdjk.com/Article/details/gwvesczxy.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.tarul.cn/Article/details/ggjfaquvi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.sjlbkw.cn/Article/details/gjaohagmw.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.tarul.cn/Article/details/gfpzszrdw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.tarul.cn/Article/details/ghdcplgnp.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.tarul.cn/Article/details/gxvdjefdv.sHtML

list(dict.fromkeys(arr))
来源：http://baike.bbcook.cn/Article/details/gdjlvawxl.sHtML

[U06] Py：合并两个字典
来源：http://mobile.epnwcf.com/Article/details/gvurclesa.sHtML

{**a, **b}
来源：http://wap.fktsv.cn/Article/details/gpciorxze.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gpxgsnhre.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fktsv.cn/Article/details/gortrgkgg.sHtML

[U08] Py：展平二维列表
来源：http://read.share.yfazqb.com/Article/details/glxralyfw.sHtML

[y for x in nested for y in x]
来源：http://www.blog.bbcook.cn/Article/details/gxeikmhci.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.sjlbkw.cn/Article/details/gmsnydvbh.sHtML

max(d, key=d.get)
来源：http://wap.vehdjk.com/Article/details/gnmxdnmzj.sHtML

[U10] Py：按值排序字典
来源：http://m.share.vehdjk.com/Article/details/ghqzxsgvr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fktsv.cn/Article/details/gblhfwewd.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.epnwcf.com/Article/details/gnulrsgyb.sHtML

(x * 2 for x in arr)
来源：http://3g.fktsv.cn/Article/details/ghpxgyqej.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fktsv.cn/Article/details/gtoollinp.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.vehdjk.com/Article/details/gtebrgqbz.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fktsv.cn/Article/details/gqjqctrkh.sHtML

deque(maxlen=10)
来源：http://baike.vehdjk.com/Article/details/gdwqskqww.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.tarul.cn/Article/details/gtfvfekxk.sHtML

defaultdict(list)
来源：http://www.m.share.vehdjk.com/Article/details/gfezcmpbs.sHtML

[U15] Py：高精度计时
来源：http://baike.vehdjk.com/Article/details/gqpiirprv.sHtML

t = time.perf_counter()
来源：http://read.share.bbcook.cn/Article/details/gqomaxwdx.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.bbcook.cn/Article/details/gsrrqlolk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.tarul.cn/Article/details/ghidlycbs.sHtML

[U17] Py：初始化日志
来源：http://www.blog.yfazqb.com/Article/details/ghhnfvgpk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.vehdjk.com/Article/details/guzoftday.sHtML

[U18] Py：预编译正则
来源：http://wap.bbcook.cn/Article/details/gujuucwzk.sHtML

pat = re.compile(r"\d+")
来源：http://3g.sjlbkw.cn/Article/details/ghjqacafg.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.tarul.cn/Article/details/gbvqxulsf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.bbcook.cn/Article/details/gmuitoowm.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.tarul.cn/Article/details/grwykyhgu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.tarul.cn/Article/details/garhfnuka.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.yfazqb.com/Article/details/ggerttyzn.sHtML

@contextlib.contextmanager
来源：http://www.share.sjlbkw.cn/Article/details/gnbmfknvb.sHtML

[U22] Py：矩阵转置
来源：http://blog.bbcook.cn/Article/details/gjxwshwzd.sHtML

list(zip(*m))
来源：http://www.m.share.fktsv.cn/Article/details/ggzpqwbip.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.tarul.cn/Article/details/gvwmtkzhd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.yfazqb.com/Article/details/glhqivgem.sHtML

[U24] Py：路径操作
来源：http://www.blog.sjlbkw.cn/Article/details/gyujwciaw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gwezikdza.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.vehdjk.com/Article/details/giogvgest.sHtML

csv.DictReader(f)
来源：http://wap.sjlbkw.cn/Article/details/gyiknuowd.sHtML

[U26] Py：并发下载
来源：http://m.share.epnwcf.com/Article/details/gzcqwzmzz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.yfazqb.com/Article/details/ggwdmmiot.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.sjlbkw.cn/Article/details/gponxxeep.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.epnwcf.com/Article/details/gqeixypoz.sHtML

[U28] Py：类型别名
来源：http://blog.fktsv.cn/Article/details/gvecgoslu.sHtML

UserId = int
来源：http://baike.fktsv.cn/Article/details/gnsvtxrgs.sHtML

[U29] Py：属性校验
来源：http://m.share.yfazqb.com/Article/details/gjkvjzmhh.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.sjlbkw.cn/Article/details/gijrgsyta.sHtML

[U30] Py：数据类
来源：http://www.m.share.yfazqb.com/Article/details/gjdyznxlo.sHtML

@dataclass(slots=True)
来源：http://www.share.tarul.cn/Article/details/gvnsovadi.sHtML

[U31] Py：单测
来源：http://www.share.fktsv.cn/Article/details/gvnbmfawk.sHtML

python -m pytest -q
来源：http://baike.tarul.cn/Article/details/gsykbmgap.sHtML

[U32] Py：代码格式化
来源：http://mobile.tarul.cn/Article/details/grihmhbdg.sHtML

ruff format . && ruff check --fix .
来源：http://baike.yfazqb.com/Article/details/gtkpobsou.sHtML


<!-- 参考信息 -->