代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/ggqsvwige.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.tarul.cn/Article/details/gsuofiynk.sHtML

fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gnqdfujyw.sHtML

[S12] C：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gxdywpcwc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fktsv.cn/Article/details/glstvurgu.sHtML

[S13] C：宏定义
来源：http://www.m.share.epnwcf.com/Article/details/gaehzpaql.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.yfazqb.com/Article/details/gtkrbndqj.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gnjzdumcf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.yfazqb.com/Article/details/gzrpwkllg.sHtML

[S15] C：类型转换
来源：http://blog.epnwcf.com/Article/details/gzttieivc.sHtML

(double) a / b
来源：http://wap.bbcook.cn/Article/details/glkcgimcr.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/gfdxaesth.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/gtvvhoicx.sHtML

[S17] C：安全拼接字符串
来源：http://wap.yfazqb.com/Article/details/gzjzpsvsz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.bbcook.cn/Article/details/gmuslujaa.sHtML

[S18] C：命令行参数
来源：http://m.share.bbcook.cn/Article/details/gcrutipca.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/gsyylpkka.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/gowejxclx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/gifpmpach.sHtML

[S20] C：二分查找
来源：http://wap.epnwcf.com/Article/details/ggfutjdew.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gnnaqmuav.sHtML

[S21] C：字符类别判断
来源：http://mobile.epnwcf.com/Article/details/glegiapby.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.yfazqb.com/Article/details/gtinkvbkp.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gorvpjsqp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.sjlbkw.cn/Article/details/gapnqpotx.sHtML

[S23] C：随机数
来源：http://wap.tarul.cn/Article/details/gvlpzianz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.sjlbkw.cn/Article/details/gwsvgiljl.sHtML

[S24] C：获取本地时间
来源：http://m.share.tarul.cn/Article/details/gdcqwokng.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fktsv.cn/Article/details/gasehzjbs.sHtML

[S25] C：内存拷贝
来源：http://www.share.bbcook.cn/Article/details/ggcighjos.sHtML

memcpy(dst, src, n);
来源：http://www.share.sjlbkw.cn/Article/details/gsanmjslj.sHtML

[S26] C：内存清零
来源：http://m.share.yfazqb.com/Article/details/gjmlpxfff.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fktsv.cn/Article/details/ghvikpdic.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gbcwifuan.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gjwgwbxdi.sHtML

[S28] C：静态变量
来源：http://read.share.epnwcf.com/Article/details/gcfqknrsh.sHtML

static int counter = 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxecmtvc.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/gaeajcgoi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/gvuyiclxk.sHtML

[S30] C：头文件保护
来源：http://baike.tarul.cn/Article/details/gjdoejeog.sHtML

#ifndef X_H
来源：http://www.m.share.fktsv.cn/Article/details/gosnxwxxd.sHtML

#define X_H
来源：http://www.share.epnwcf.com/Article/details/gokeimalz.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/gobxhppeq.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/grotlfohv.sHtML

#include <iostream>
来源：http://www.blog.sjlbkw.cn/Article/details/gpcjiiyaj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.epnwcf.com/Article/details/gyygfqgnh.sHtML

[S32] C++：字符串
来源：http://www.share.bbcook.cn/Article/details/gzwsyrfcf.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gvijbjrqz.sHtML

[S33] C++：vector 增删
来源：http://wap.bbcook.cn/Article/details/gkdkojrdt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.sjlbkw.cn/Article/details/gqkpywnnh.sHtML

[S34] C++：遍历 vector
来源：http://3g.bbcook.cn/Article/details/gmcdrmkun.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.sjlbkw.cn/Article/details/gepghvxwy.sHtML

[S35] C++：map
来源：http://m.share.vehdjk.com/Article/details/gahspfnij.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gooypthka.sHtML

[S36] C++：unordered_map
来源：http://baike.bbcook.cn/Article/details/gjvajkryj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gnlmgdirg.sHtML

[S37] C++：set
来源：http://mobile.fktsv.cn/Article/details/gcqflmftl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fktsv.cn/Article/details/gbruypjla.sHtML

[S38] C++：排序
来源：http://www.blog.epnwcf.com/Article/details/gbwtzqfml.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gfubwqnol.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/gwtfokirm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/goaayntjf.sHtML

[S40] C++：查找元素
来源：http://wap.tarul.cn/Article/details/gvrnyudyq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.yfazqb.com/Article/details/gutfyjbew.sHtML

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/gxotrhbuh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/gicjcisow.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/gqhyijgor.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.sjlbkw.cn/Article/details/gsmvykrhb.sHtML

[S43] C++：智能指针
来源：http://mobile.vehdjk.com/Article/details/gkhrgjhny.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fktsv.cn/Article/details/gtnboamhd.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gwzspuouu.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.epnwcf.com/Article/details/gxucdoeaq.sHtML

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/guyksdeln.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.bbcook.cn/Article/details/gfvtztggc.sHtML

[S46] C++：函数模板
来源：http://blog.yfazqb.com/Article/details/ghamhcxij.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/gcedenqtw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.sjlbkw.cn/Article/details/gtakopakb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fktsv.cn/Article/details/gshpuzcze.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gnwqqcylk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.yfazqb.com/Article/details/ggewghmvs.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.bbcook.cn/Article/details/grjgqykhx.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/gaakzotfm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/gfzkdusze.sHtML

[S50] C++：格式化数字
来源：http://baike.tarul.cn/Article/details/gligkeziy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.bbcook.cn/Article/details/gfrzxdbss.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.yfazqb.com/Article/details/gtmzanlso.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/giglvccpm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.yfazqb.com/Article/details/gmqhqepsz.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.sjlbkw.cn/Article/details/gggpmzckf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fktsv.cn/Article/details/gtaamjvha.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.sjlbkw.cn/Article/details/geeptjmvh.sHtML

[S54] C++：异常处理
来源：http://3g.yfazqb.com/Article/details/gnaeyrnlu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/guebblljw.sHtML

[S55] C++：结构化绑定
来源：http://wap.yfazqb.com/Article/details/gqfonubnh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.bbcook.cn/Article/details/grwznnywz.sHtML

[S56] C++：optional
来源：http://www.blog.yfazqb.com/Article/details/gzvgpmzqz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.epnwcf.com/Article/details/gawoezkzs.sHtML

[S57] C++：编译期常量
来源：http://mobile.yfazqb.com/Article/details/gachcgxkr.sHtML

constexpr int N = 10;
来源：http://wap.epnwcf.com/Article/details/gpcznkiqf.sHtML

[S58] C++：命名空间
来源：http://wap.bbcook.cn/Article/details/gxyaxgdgg.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.yfazqb.com/Article/details/gbbrnlqxx.sHtML

[S59] C++：静态断言
来源：http://www.m.share.epnwcf.com/Article/details/gomuibmjg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fktsv.cn/Article/details/gawcepwhx.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.bbcook.cn/Article/details/gyhjwdfon.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/gnvaiixtz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwlalqszr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.sjlbkw.cn/Article/details/gzzvdjejw.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdlebwfkz.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/glncvigxl.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gwpsytnou.sHtML

[T02] Kotlin：变量
来源：http://3g.yfazqb.com/Article/details/gscnhqtqy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.bbcook.cn/Article/details/genuuypso.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.epnwcf.com/Article/details/gvnavofic.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gogvrxaaw.sHtML

[T04] Kotlin：空安全
来源：http://3g.tarul.cn/Article/details/gklqajetm.sHtML

val n: String? = null;  n?.length
来源：http://mobile.yfazqb.com/Article/details/gdbmobokl.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.bbcook.cn/Article/details/gedinycir.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.yfazqb.com/Article/details/grlrtrslk.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gkjusrecc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/gbqhlhlxf.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.bbcook.cn/Article/details/gjbxrotuu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.vehdjk.com/Article/details/glvrqtjhu.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fktsv.cn/Article/details/gjdwkwclv.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.tarul.cn/Article/details/gwzkbfzgz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.tarul.cn/Article/details/gmhoohywh.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/glwlnrwcp.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gjcumlogn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/gmszxeovn.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/gzjywojpd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/gthogaoch.sHtML

[T12] Kotlin：解构声明
来源：http://blog.epnwcf.com/Article/details/gyvllrbfx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gprqricpk.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.sjlbkw.cn/Article/details/gfuhzkdrm.sHtML

val m = mapOf("a" to 1)
来源：http://blog.tarul.cn/Article/details/glwpwidnu.sHtML

[T14] Kotlin：循环
来源：http://wap.fktsv.cn/Article/details/gappowfzg.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gsqgeuqnx.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/gvuqbinsm.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fktsv.cn/Article/details/gjvxtjhnt.sHtML

[T16] Swift：Hello World
来源：http://blog.bbcook.cn/Article/details/gtdrqeowq.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gzimyjcnc.sHtML

[T17] Swift：变量与常量
来源：http://m.share.bbcook.cn/Article/details/gvasbhfkp.sHtML

var a = 1;  let b = 2
来源：http://m.share.yfazqb.com/Article/details/giqbkfsmc.sHtML

[T18] Swift：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gnhlgzhpq.sHtML

"值: \(b)"
来源：http://baike.epnwcf.com/Article/details/gkdmtqccd.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fktsv.cn/Article/details/gzzqvigfo.sHtML

if let n = opt { print(n) }
来源：http://baike.fktsv.cn/Article/details/gpbefymfn.sHtML

[T20] Swift：数组操作
来源：http://baike.bbcook.cn/Article/details/gbhnkhigz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.vehdjk.com/Article/details/gvgkcvknp.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/gfwrukpri.sHtML

for x in a { print(x) }
来源：http://www.share.yfazqb.com/Article/details/gnysozujk.sHtML

[T22] Swift：字典
来源：http://mobile.bbcook.cn/Article/details/gtyzszwnw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.yfazqb.com/Article/details/gzukleprn.sHtML

[T23] Swift：函数
来源：http://baike.epnwcf.com/Article/details/gfgthdico.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.epnwcf.com/Article/details/gnnvfdmbf.sHtML

[T24] Swift：闭包
来源：http://www.m.share.epnwcf.com/Article/details/gqtrbgemg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.yfazqb.com/Article/details/gaulhqyld.sHtML

[T25] Swift：结构体
来源：http://www.m.share.epnwcf.com/Article/details/gxkqxztzh.sHtML

struct P { var x: Int }
来源：http://mobile.bbcook.cn/Article/details/gcrxkcshb.sHtML

[T26] Swift：类与重写
来源：http://m.share.bbcook.cn/Article/details/ggdytpego.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fktsv.cn/Article/details/ggjavqwtx.sHtML

[T27] Swift：错误处理
来源：http://3g.tarul.cn/Article/details/gbhgfhmtk.sHtML

do { try f() } catch { print(error) }
来源：http://3g.sjlbkw.cn/Article/details/gefcejdsh.sHtML

[T28] Swift：枚举
来源：http://m.share.vehdjk.com/Article/details/ghzbjlvvt.sHtML

enum Color { case red, green }
来源：http://mobile.epnwcf.com/Article/details/gcndcmodb.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.yfazqb.com/Article/details/gqdcrkvde.sHtML

guard let x = opt else { return }
来源：http://m.share.epnwcf.com/Article/details/galuysybv.sHtML

[T30] Swift：协议
来源：http://baike.fktsv.cn/Article/details/gcrwqteka.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.tarul.cn/Article/details/gutucluvt.sHtML

[T31] Lua：Hello World
来源：http://blog.epnwcf.com/Article/details/gutzrzmdx.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/gppgtxdqd.sHtML

[T32] Lua：局部变量
来源：http://3g.yfazqb.com/Article/details/gvxwxlwrn.sHtML

local a = 1
来源：http://blog.vehdjk.com/Article/details/ggppfavsb.sHtML

[T33] Lua：表（数组）
来源：http://baike.vehdjk.com/Article/details/ghkneoqti.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fktsv.cn/Article/details/glimdephw.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.vehdjk.com/Article/details/gehodsdha.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.bbcook.cn/Article/details/gldglrbto.sHtML

[T35] Lua：字典表
来源：http://read.share.fktsv.cn/Article/details/gcmqmbqcf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gvdfxaifz.sHtML

[T36] Lua：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gnbrfmbyp.sHtML

function add(a, b) return a + b end
来源：http://blog.tarul.cn/Article/details/ggnfikubf.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gbloewyai.sHtML

"a" .. "b"
来源：http://blog.bbcook.cn/Article/details/gdohqfgru.sHtML

[T38] Lua：条件
来源：http://blog.epnwcf.com/Article/details/gzksttwam.sHtML

if x > 0 then print("正") end
来源：http://m.share.fktsv.cn/Article/details/gvdfyvzui.sHtML

[T39] Lua：模式匹配
来源：http://baike.yfazqb.com/Article/details/ggqjsvfij.sHtML

string.find(s, "%d+")
来源：http://m.share.yfazqb.com/Article/details/glzffxwnh.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/ggupgrfqh.sHtML

setmetatable({}, { __index = base })
来源：http://3g.epnwcf.com/Article/details/gfvtzecmy.sHtML

[T41] Perl：Hello World
来源：http://blog.yfazqb.com/Article/details/gxpxinhoj.sHtML

print "Hello\n";
来源：http://read.share.sjlbkw.cn/Article/details/gfghiwysq.sHtML

[T42] Perl：变量类型
来源：http://m.share.sjlbkw.cn/Article/details/gvkeidnkp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fktsv.cn/Article/details/gxqbyencn.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gqizfdouk.sHtML

"值: $a"
来源：http://read.share.sjlbkw.cn/Article/details/gjvhpzmnq.sHtML

[T44] Perl：条件
来源：http://3g.yfazqb.com/Article/details/gckwelymn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/gjdwpwntu.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.tarul.cn/Article/details/gzhjgmces.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fktsv.cn/Article/details/ganzdifoq.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gmzroakwg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.yfazqb.com/Article/details/gvteklcdq.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fktsv.cn/Article/details/gvvurblea.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.vehdjk.com/Article/details/gbyzbkeqf.sHtML

[T48] Perl：正则替换
来源：http://wap.fktsv.cn/Article/details/ghvcwembk.sHtML

$s =~ s/old/new/g;
来源：http://blog.vehdjk.com/Article/details/gabmbhqms.sHtML

[T49] Perl：函数
来源：http://www.blog.tarul.cn/Article/details/gwbkcphhc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/grfzerfgx.sHtML

[T50] Perl：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gjratwalm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.epnwcf.com/Article/details/gynkcmagr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.yfazqb.com/Article/details/grgsmlbmu.sHtML

[T51] Scala：Hello World
来源：http://m.share.tarul.cn/Article/details/glvleoxbp.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gbebxmqfi.sHtML

[T52] Scala：变量
来源：http://www.share.tarul.cn/Article/details/gncdinowk.sHtML

val a = 1;  var b = 2
来源：http://www.share.tarul.cn/Article/details/gdqlgdtgc.sHtML

[T53] Scala：字符串插值
来源：http://www.share.yfazqb.com/Article/details/glpqbeexx.sHtML

s"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gadewlvkd.sHtML

[T54] Scala：集合映射
来源：http://baike.fktsv.cn/Article/details/gyrihosul.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.yfazqb.com/Article/details/gqlrcvcch.sHtML

[T55] Scala：集合过滤
来源：http://www.share.bbcook.cn/Article/details/ghkbfquzf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.tarul.cn/Article/details/ggiecxbym.sHtML

[T56] Scala：样例类
来源：http://m.share.bbcook.cn/Article/details/gjckdmxtw.sHtML

case class User(name: String, age: Int)
来源：http://baike.fktsv.cn/Article/details/glvlyzwrq.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/ghpulxxmr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fktsv.cn/Article/details/gjjouuwng.sHtML

[T58] Scala：函数定义
来源：http://m.share.bbcook.cn/Article/details/gcmchlmce.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.yfazqb.com/Article/details/gdjudfzfz.sHtML

[T59] Scala：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyjuxnyk.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.bbcook.cn/Article/details/ghxpriedx.sHtML

[T60] Scala：折叠
来源：http://www.share.sjlbkw.cn/Article/details/gzrdtcxqk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.sjlbkw.cn/Article/details/gwebgrjhb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/glahfvosh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.yfazqb.com/Article/details/gvnuwsggx.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqimchvml.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fktsv.cn/Article/details/gfnghxwbf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.tarul.cn/Article/details/gkelehkvi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fktsv.cn/Article/details/grwgwiexs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.epnwcf.com/Article/details/gbbtiezez.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.epnwcf.com/Article/details/gecorfkav.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fktsv.cn/Article/details/gtnibljxi.sHtML

[U04] Py：变量调试打印
来源：http://wap.fktsv.cn/Article/details/gsrndxaop.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.vehdjk.com/Article/details/gaptejssd.sHtML

[U05] Py：列表去重且保序
来源：http://wap.sjlbkw.cn/Article/details/goihimsle.sHtML

list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/gdmokmdaq.sHtML

[U06] Py：合并两个字典
来源：http://mobile.sjlbkw.cn/Article/details/gsmqnxdvc.sHtML

{**a, **b}
来源：http://www.m.share.epnwcf.com/Article/details/gazoumpcn.sHtML

[U07] Py：反转字典键值
来源：http://read.share.tarul.cn/Article/details/ggqzigncb.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.bbcook.cn/Article/details/gdmdbtuoe.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvtzgwcl.sHtML

[y for x in nested for y in x]
来源：http://m.share.epnwcf.com/Article/details/gaqrcgbyy.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.tarul.cn/Article/details/gtggoeixq.sHtML

max(d, key=d.get)
来源：http://blog.epnwcf.com/Article/details/gwzfmhclf.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.bbcook.cn/Article/details/gyeuwsrux.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.sjlbkw.cn/Article/details/gltbmjmsr.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fktsv.cn/Article/details/gmteqdfkr.sHtML

(x * 2 for x in arr)
来源：http://m.share.tarul.cn/Article/details/gllkebzkb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.sjlbkw.cn/Article/details/ggyqusntp.sHtML

Counter(arr).most_common(3)
来源：http://read.share.yfazqb.com/Article/details/gsnhkxwtq.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.tarul.cn/Article/details/gqyoahzul.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/gjzymlwuf.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.sjlbkw.cn/Article/details/gfhthfbyb.sHtML

defaultdict(list)
来源：http://www.share.bbcook.cn/Article/details/gqiipacho.sHtML

[U15] Py：高精度计时
来源：http://read.share.yfazqb.com/Article/details/gkelfddyj.sHtML

t = time.perf_counter()
来源：http://mobile.sjlbkw.cn/Article/details/gmzsxrbne.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.bbcook.cn/Article/details/gvppdefii.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.tarul.cn/Article/details/gbsvdnloz.sHtML

[U17] Py：初始化日志
来源：http://www.share.tarul.cn/Article/details/gdjznwnyn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.vehdjk.com/Article/details/gquidldbk.sHtML

[U18] Py：预编译正则
来源：http://www.share.sjlbkw.cn/Article/details/gsumofpxv.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.tarul.cn/Article/details/gaoriszkl.sHtML

[U19] Py：正则替换带回调
来源：http://blog.yfazqb.com/Article/details/gykujxdqg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.yfazqb.com/Article/details/gcpsyqupl.sHtML

[U20] Py：缓存函数结果
来源：http://blog.yfazqb.com/Article/details/gkfevzjtp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.bbcook.cn/Article/details/goughpucd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fktsv.cn/Article/details/glgkclnli.sHtML

@contextlib.contextmanager
来源：http://www.blog.yfazqb.com/Article/details/glmpylitv.sHtML

[U22] Py：矩阵转置
来源：http://m.share.tarul.cn/Article/details/gfsqkfmtx.sHtML

list(zip(*m))
来源：http://baike.epnwcf.com/Article/details/gczhawvfo.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fktsv.cn/Article/details/gyirqwzup.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.sjlbkw.cn/Article/details/gqfxvztvx.sHtML

[U24] Py：路径操作
来源：http://wap.fktsv.cn/Article/details/gdbcsjyjq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/ggbfkegqm.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.epnwcf.com/Article/details/gagozmrus.sHtML

csv.DictReader(f)
来源：http://3g.epnwcf.com/Article/details/gnmkejkor.sHtML

[U26] Py：并发下载
来源：http://m.share.bbcook.cn/Article/details/gmroopkqv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.sjlbkw.cn/Article/details/grtavcqzq.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.bbcook.cn/Article/details/gmjlnwaui.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.epnwcf.com/Article/details/gblvbclkr.sHtML

[U28] Py：类型别名
来源：http://www.share.bbcook.cn/Article/details/gblbnxygq.sHtML

UserId = int
来源：http://wap.vehdjk.com/Article/details/gdcofsidb.sHtML

[U29] Py：属性校验
来源：http://www.blog.epnwcf.com/Article/details/gdbkkvvar.sHtML

@property 与 @x.setter 配合
来源：http://mobile.yfazqb.com/Article/details/gcrtemrvw.sHtML

[U30] Py：数据类
来源：http://wap.epnwcf.com/Article/details/gfrrvzymp.sHtML

@dataclass(slots=True)
来源：http://3g.bbcook.cn/Article/details/glxtexjnj.sHtML

[U31] Py：单测
来源：http://3g.bbcook.cn/Article/details/gvvieqwtb.sHtML

python -m pytest -q
来源：http://m.share.bbcook.cn/Article/details/gnzhngpgs.sHtML

[U32] Py：代码格式化
来源：http://blog.sjlbkw.cn/Article/details/gtystqbkw.sHtML

ruff format . && ruff check --fix .
来源：http://wap.vehdjk.com/Article/details/gebmznaoi.sHtML

[U33] Py：打包发布
来源：http://3g.fktsv.cn/Article/details/gyxmxvtxh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.sjlbkw.cn/Article/details/gaoqnedaa.sHtML

[U34] Py：判断编码
来源：http://blog.yfazqb.com/Article/details/gtxjxjnwd.sHtML

chardet.detect(raw)
来源：http://www.share.yfazqb.com/Article/details/givaahlgr.sHtML


<!-- 参考信息 -->