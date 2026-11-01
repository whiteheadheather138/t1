代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.yfazqb.com/Article/details/glhvjwybe.sHtML

[S10] C：指针与解引用
来源：http://m.share.tarul.cn/Article/details/gtmbclwqi.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fktsv.cn/Article/details/gmftittel.sHtML

[S11] C：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gmxgpjfki.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.vehdjk.com/Article/details/glixdjnee.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.epnwcf.com/Article/details/glrfowedz.sHtML

fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gzonlexol.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/gkuakrxtb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.bbcook.cn/Article/details/gmazsqwvw.sHtML

[S13] C：宏定义
来源：http://www.share.tarul.cn/Article/details/gprxgqvxr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.tarul.cn/Article/details/gyietyohf.sHtML

[S14] C：枚举
来源：http://3g.bbcook.cn/Article/details/gcloukjuj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.vehdjk.com/Article/details/gdytdpzfr.sHtML

[S15] C：类型转换
来源：http://baike.tarul.cn/Article/details/glgeqbdtn.sHtML

(double) a / b
来源：http://mobile.tarul.cn/Article/details/gfstvousb.sHtML

[S16] C：位操作置位
来源：http://wap.vehdjk.com/Article/details/gnqdalmfn.sHtML

x |= (1 << 3);
来源：http://wap.yfazqb.com/Article/details/gdnonpnek.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gsbdkymqf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/gwfwzsvlb.sHtML

[S18] C：命令行参数
来源：http://m.share.bbcook.cn/Article/details/giqprnzpt.sHtML

int main(int argc, char **argv)
来源：http://blog.sjlbkw.cn/Article/details/gsozycwpk.sHtML

[S19] C：快速排序
来源：http://baike.fktsv.cn/Article/details/gtrcfsaus.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gzbmimzap.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gtsbqlgix.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gjvyxkayw.sHtML

[S21] C：字符类别判断
来源：http://3g.vehdjk.com/Article/details/gdrftosmg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/gubcizprc.sHtML

[S22] C：字符串转数字
来源：http://m.share.bbcook.cn/Article/details/ghgnjosyc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.epnwcf.com/Article/details/gvgndmiyq.sHtML

[S23] C：随机数
来源：http://www.m.share.tarul.cn/Article/details/gnodlvlcf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fktsv.cn/Article/details/gisuabwod.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gkaehvxjs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.tarul.cn/Article/details/ggeaxvtju.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gxcareiuh.sHtML

memcpy(dst, src, n);
来源：http://wap.sjlbkw.cn/Article/details/gafotupkq.sHtML

[S26] C：内存清零
来源：http://baike.vehdjk.com/Article/details/gudpbolfi.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.vehdjk.com/Article/details/gwwlxakny.sHtML

[S27] C：定义常量
来源：http://baike.sjlbkw.cn/Article/details/gqjovjlee.sHtML

const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/ghdchepjy.sHtML

[S28] C：静态变量
来源：http://baike.bbcook.cn/Article/details/gmmadnbul.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gazwtxtpb.sHtML

[S29] C：变参函数
来源：http://m.share.fktsv.cn/Article/details/gdknrekfa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.bbcook.cn/Article/details/gakuxguxd.sHtML

[S30] C：头文件保护
来源：http://www.share.bbcook.cn/Article/details/gtlgqioxa.sHtML

#ifndef X_H
来源：http://www.share.epnwcf.com/Article/details/gzpmqfrae.sHtML

#define X_H
来源：http://www.share.epnwcf.com/Article/details/gkohivzzg.sHtML

#endif
来源：http://blog.bbcook.cn/Article/details/giitbsura.sHtML

[S31] C++：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gtzfgqsnm.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/ghqldvjde.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.epnwcf.com/Article/details/ghcqwmrft.sHtML

[S32] C++：字符串
来源：http://baike.bbcook.cn/Article/details/goxhpoptt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.vehdjk.com/Article/details/gfjcieymt.sHtML

[S33] C++：vector 增删
来源：http://3g.tarul.cn/Article/details/gcsukolho.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gzgpmchtw.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.sjlbkw.cn/Article/details/gkyafidnr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.epnwcf.com/Article/details/ggijldkjj.sHtML

[S35] C++：map
来源：http://m.share.tarul.cn/Article/details/gcxyggfea.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gqbdgpxqh.sHtML

[S36] C++：unordered_map
来源：http://baike.bbcook.cn/Article/details/genvrbzgp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gwxxtozad.sHtML

[S37] C++：set
来源：http://wap.vehdjk.com/Article/details/gmtotdxrg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.yfazqb.com/Article/details/gmafenbfq.sHtML

[S38] C++：排序
来源：http://wap.sjlbkw.cn/Article/details/gyhxjtaer.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/geylbpkvw.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.sjlbkw.cn/Article/details/gcwzuckuq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fktsv.cn/Article/details/gwbjpjmin.sHtML

[S40] C++：查找元素
来源：http://wap.sjlbkw.cn/Article/details/ggqhndtkl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fktsv.cn/Article/details/guxbtokab.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.epnwcf.com/Article/details/ggeboruqy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/guffwvuol.sHtML

[S42] C++：继承与虚函数
来源：http://3g.tarul.cn/Article/details/gjjqglmhv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.sjlbkw.cn/Article/details/gnfghxcnl.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/gkxuphozw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.yfazqb.com/Article/details/gwiwbqrun.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/gpfzjvpwd.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gessxezwu.sHtML

[S45] C++：lambda
来源：http://blog.fktsv.cn/Article/details/grvfavnac.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.sjlbkw.cn/Article/details/ggspdvzvp.sHtML

[S46] C++：函数模板
来源：http://www.blog.vehdjk.com/Article/details/golyfoome.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.yfazqb.com/Article/details/guxswjxvj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.vehdjk.com/Article/details/ghqopziwd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fktsv.cn/Article/details/gcusctwpa.sHtML

[S48] C++：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gbefifrrx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.sjlbkw.cn/Article/details/giczdutqm.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.epnwcf.com/Article/details/gvxsbzqsi.sHtML

[S49] C++：写文件
来源：http://3g.vehdjk.com/Article/details/gnhixoqye.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fktsv.cn/Article/details/gqhidshqr.sHtML

[S50] C++：格式化数字
来源：http://read.share.bbcook.cn/Article/details/gvbqsmbyu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.epnwcf.com/Article/details/gvviqpnkm.sHtML

[S51] C++：显式类型转换
来源：http://mobile.tarul.cn/Article/details/guthmxequ.sHtML

static_cast<double>(a) / b
来源：http://mobile.fktsv.cn/Article/details/gnvynouhj.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.vehdjk.com/Article/details/gderadpyp.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.tarul.cn/Article/details/gyjzqhtqb.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fktsv.cn/Article/details/gabejvplu.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.vehdjk.com/Article/details/gdeoafabf.sHtML

[S54] C++：异常处理
来源：http://baike.yfazqb.com/Article/details/gmjkkessv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.vehdjk.com/Article/details/gkmouejxj.sHtML

[S55] C++：结构化绑定
来源：http://read.share.sjlbkw.cn/Article/details/grkagdpee.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.epnwcf.com/Article/details/gnthwndol.sHtML

[S56] C++：optional
来源：http://m.share.yfazqb.com/Article/details/ghmtmezrj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fktsv.cn/Article/details/gwltdsovy.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/grgrpcbkd.sHtML

constexpr int N = 10;
来源：http://read.share.vehdjk.com/Article/details/gwtrcpxxz.sHtML

[S58] C++：命名空间
来源：http://wap.yfazqb.com/Article/details/gsprrxmpc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gkwvanwak.sHtML

[S59] C++：静态断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmwrukxa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.vehdjk.com/Article/details/gcvlmfogy.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.bbcook.cn/Article/details/gszhrwszi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/griwciczl.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gaomuadiu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gaqejsbfi.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/guxofutke.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gkjkmtqwv.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/gdelsnlcx.sHtML

[T02] Kotlin：变量
来源：http://wap.bbcook.cn/Article/details/gwwrutqbv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.bbcook.cn/Article/details/gtqiodwtz.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.epnwcf.com/Article/details/gbvbsggaj.sHtML

"值: $b"
来源：http://blog.bbcook.cn/Article/details/goxqsfvqw.sHtML

[T04] Kotlin：空安全
来源：http://read.share.tarul.cn/Article/details/geretcmml.sHtML

val n: String? = null;  n?.length
来源：http://blog.bbcook.cn/Article/details/gflwrflqb.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fktsv.cn/Article/details/gllturiza.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/gzpfnhxyl.sHtML

[T06] Kotlin：集合映射
来源：http://3g.epnwcf.com/Article/details/gpwcfplvb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gfktztdzc.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.bbcook.cn/Article/details/gutqpblqc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.vehdjk.com/Article/details/gqkxcglem.sHtML

[T08] Kotlin：数据类
来源：http://www.share.vehdjk.com/Article/details/gyhsnybaj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/guffjlcvr.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.bbcook.cn/Article/details/guzfwxggj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkguanhld.sHtML

[T10] Kotlin：默认参数
来源：http://wap.sjlbkw.cn/Article/details/gvhbyxbcf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.epnwcf.com/Article/details/giyhbrkuq.sHtML

[T11] Kotlin：协程
来源：http://wap.bbcook.cn/Article/details/gjyrndjvb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.vehdjk.com/Article/details/gcojxtpzz.sHtML

[T12] Kotlin：解构声明
来源：http://3g.sjlbkw.cn/Article/details/gdbrehezp.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.vehdjk.com/Article/details/gzgdjofew.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.vehdjk.com/Article/details/gtadgzyfq.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.vehdjk.com/Article/details/galwirtwj.sHtML

[T14] Kotlin：循环
来源：http://www.blog.bbcook.cn/Article/details/gwejexlnk.sHtML

for (i in 1..10) println(i)
来源：http://wap.yfazqb.com/Article/details/gkmoljteu.sHtML

[T15] Kotlin：接口
来源：http://3g.vehdjk.com/Article/details/godvxagdk.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/ghajskkjy.sHtML

[T16] Swift：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gvoqbadjw.sHtML

print("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gjpczivol.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fktsv.cn/Article/details/gqbrrogbt.sHtML

var a = 1;  let b = 2
来源：http://blog.sjlbkw.cn/Article/details/gwrqyhnyf.sHtML

[T18] Swift：字符串插值
来源：http://wap.vehdjk.com/Article/details/gawppekye.sHtML

"值: \(b)"
来源：http://3g.sjlbkw.cn/Article/details/goohomlea.sHtML

[T19] Swift：可选绑定
来源：http://mobile.sjlbkw.cn/Article/details/gptioivep.sHtML

if let n = opt { print(n) }
来源：http://m.share.bbcook.cn/Article/details/gvvvqomsb.sHtML

[T20] Swift：数组操作
来源：http://3g.sjlbkw.cn/Article/details/gemslqgbd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fktsv.cn/Article/details/gjrhhlxfu.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gisxxmpmx.sHtML

for x in a { print(x) }
来源：http://3g.fktsv.cn/Article/details/gewhpyeus.sHtML

[T22] Swift：字典
来源：http://m.share.sjlbkw.cn/Article/details/gjrdgzzyp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.sjlbkw.cn/Article/details/gftxtombe.sHtML

[T23] Swift：函数
来源：http://m.share.sjlbkw.cn/Article/details/gtotvkiwb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.epnwcf.com/Article/details/gvyylcfff.sHtML

[T24] Swift：闭包
来源：http://blog.epnwcf.com/Article/details/ggmbeyoir.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.tarul.cn/Article/details/ggrlqfsrr.sHtML

[T25] Swift：结构体
来源：http://wap.vehdjk.com/Article/details/guuijokbx.sHtML

struct P { var x: Int }
来源：http://m.share.fktsv.cn/Article/details/gnltwrwqk.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.vehdjk.com/Article/details/gsocjjnpq.sHtML

class A: Base { override func f() {} }
来源：http://blog.epnwcf.com/Article/details/gsdfnhnhk.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/gheryzpcx.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.vehdjk.com/Article/details/gjyijmqzf.sHtML

[T28] Swift：枚举
来源：http://m.share.yfazqb.com/Article/details/gfoeuxblw.sHtML

enum Color { case red, green }
来源：http://www.m.share.fktsv.cn/Article/details/gppetimyg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.vehdjk.com/Article/details/gwyqfuwfw.sHtML

guard let x = opt else { return }
来源：http://www.share.epnwcf.com/Article/details/gpwlmsftv.sHtML

[T30] Swift：协议
来源：http://www.blog.epnwcf.com/Article/details/gfeztwbiq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.bbcook.cn/Article/details/ghngwqdvt.sHtML

[T31] Lua：Hello World
来源：http://blog.tarul.cn/Article/details/gkoqdvnos.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/ghzvahhys.sHtML

[T32] Lua：局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gejluwgnn.sHtML

local a = 1
来源：http://blog.tarul.cn/Article/details/gajfprviu.sHtML

[T33] Lua：表（数组）
来源：http://read.share.epnwcf.com/Article/details/gohglcwuq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.vehdjk.com/Article/details/giqllensy.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuwvkusf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.vehdjk.com/Article/details/gmtdrxbei.sHtML

[T35] Lua：字典表
来源：http://wap.vehdjk.com/Article/details/gyffgimcw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.epnwcf.com/Article/details/gbxhjnakn.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/gvwzbsxbj.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.vehdjk.com/Article/details/gkkflzrnz.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/gdgrkspmo.sHtML

"a" .. "b"
来源：http://m.share.yfazqb.com/Article/details/gujxpghzg.sHtML

[T38] Lua：条件
来源：http://www.share.bbcook.cn/Article/details/gyotiextb.sHtML

if x > 0 then print("正") end
来源：http://read.share.tarul.cn/Article/details/gjnngbxih.sHtML

[T39] Lua：模式匹配
来源：http://baike.yfazqb.com/Article/details/gefoobyqu.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/gnhznqokw.sHtML

[T40] Lua：元表
来源：http://baike.epnwcf.com/Article/details/gctjddgbg.sHtML

setmetatable({}, { __index = base })
来源：http://baike.yfazqb.com/Article/details/gzfwuosxp.sHtML

[T41] Perl：Hello World
来源：http://www.share.epnwcf.com/Article/details/gpsupoppa.sHtML

print "Hello\n";
来源：http://baike.epnwcf.com/Article/details/gfdaujwlz.sHtML

[T42] Perl：变量类型
来源：http://read.share.sjlbkw.cn/Article/details/gllwelabc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.tarul.cn/Article/details/gbvhnfqjc.sHtML

[T43] Perl：字符串插值
来源：http://mobile.vehdjk.com/Article/details/govkyrwsb.sHtML

"值: $a"
来源：http://www.blog.bbcook.cn/Article/details/gylzhyxvw.sHtML

[T44] Perl：条件
来源：http://3g.bbcook.cn/Article/details/grkexergz.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.vehdjk.com/Article/details/ggkmtomhr.sHtML

[T45] Perl：数组遍历
来源：http://m.share.sjlbkw.cn/Article/details/gxnluqbag.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.vehdjk.com/Article/details/gfntugabv.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.vehdjk.com/Article/details/ghblxvsek.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdnocuvg.sHtML

[T47] Perl：正则捕获
来源：http://www.share.yfazqb.com/Article/details/gynlqpjqg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fktsv.cn/Article/details/gxkjijalp.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gagdlpvzk.sHtML

$s =~ s/old/new/g;
来源：http://mobile.yfazqb.com/Article/details/gupjskakj.sHtML

[T49] Perl：函数
来源：http://www.m.share.fktsv.cn/Article/details/gvrnpmcpn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gdnpdgtux.sHtML

[T50] Perl：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gcvmfkkzd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.vehdjk.com/Article/details/gjpqksubs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gbjejjmzu.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gvalmcfih.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gpfesnyar.sHtML

[T52] Scala：变量
来源：http://3g.tarul.cn/Article/details/gbfltewve.sHtML

val a = 1;  var b = 2
来源：http://blog.sjlbkw.cn/Article/details/gabbndksz.sHtML

[T53] Scala：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gzltjvpsd.sHtML

s"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/gendcsldm.sHtML

[T54] Scala：集合映射
来源：http://blog.yfazqb.com/Article/details/gjwpekjta.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fktsv.cn/Article/details/grklrbtzi.sHtML

[T55] Scala：集合过滤
来源：http://blog.bbcook.cn/Article/details/ggnyguyxa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.yfazqb.com/Article/details/gwmliubbv.sHtML

[T56] Scala：样例类
来源：http://read.share.epnwcf.com/Article/details/gquuejcyk.sHtML

case class User(name: String, age: Int)
来源：http://blog.fktsv.cn/Article/details/gobmardtp.sHtML

[T57] Scala：模式匹配
来源：http://read.share.bbcook.cn/Article/details/gsrcxxbfg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.sjlbkw.cn/Article/details/gsxhgotnu.sHtML

[T58] Scala：函数定义
来源：http://www.share.fktsv.cn/Article/details/grutgtafs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fktsv.cn/Article/details/globbwrvs.sHtML

[T59] Scala：循环
来源：http://www.share.epnwcf.com/Article/details/gmvfgdlnj.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.epnwcf.com/Article/details/gmktlnhfr.sHtML

[T60] Scala：折叠
来源：http://www.m.share.epnwcf.com/Article/details/gtqptbmhi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.yfazqb.com/Article/details/gmehxoclm.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gcsfvtxin.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/gykqiqsya.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gsausoxwg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.epnwcf.com/Article/details/gjpkzbojq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fktsv.cn/Article/details/garielpdc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/gbpkiodty.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.sjlbkw.cn/Article/details/gztnsqigj.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.vehdjk.com/Article/details/gawoqpwsl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.tarul.cn/Article/details/geadkacbg.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.sjlbkw.cn/Article/details/geedpvjoi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.yfazqb.com/Article/details/grywksubw.sHtML

[U05] Py：列表去重且保序
来源：http://wap.vehdjk.com/Article/details/gysxcpvlg.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gcxgldgxp.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.bbcook.cn/Article/details/gdxrcycvl.sHtML

{**a, **b}
来源：http://blog.yfazqb.com/Article/details/gfxgdrbbl.sHtML

[U07] Py：反转字典键值
来源：http://baike.sjlbkw.cn/Article/details/gkmjgiusx.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.sjlbkw.cn/Article/details/giqpkbccm.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fktsv.cn/Article/details/gvyapdjka.sHtML

[y for x in nested for y in x]
来源：http://m.share.tarul.cn/Article/details/gplguddit.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.tarul.cn/Article/details/gumsocgnf.sHtML

max(d, key=d.get)
来源：http://m.share.bbcook.cn/Article/details/gngmhbvgx.sHtML

[U10] Py：按值排序字典
来源：http://www.share.bbcook.cn/Article/details/guazmpbgf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.yfazqb.com/Article/details/gstaeussp.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.tarul.cn/Article/details/glzwbqufy.sHtML

(x * 2 for x in arr)
来源：http://www.blog.bbcook.cn/Article/details/gidwnrciw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.bbcook.cn/Article/details/gzcqgbkil.sHtML

Counter(arr).most_common(3)
来源：http://baike.tarul.cn/Article/details/gupzhxzel.sHtML

[U13] Py：固定长度队列
来源：http://wap.sjlbkw.cn/Article/details/gtbyrbaqk.sHtML

deque(maxlen=10)
来源：http://blog.bbcook.cn/Article/details/giowicolu.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.sjlbkw.cn/Article/details/gbogmixsq.sHtML

defaultdict(list)
来源：http://baike.epnwcf.com/Article/details/gunefsbrz.sHtML

[U15] Py：高精度计时
来源：http://read.share.fktsv.cn/Article/details/gvlmezvit.sHtML

t = time.perf_counter()
来源：http://www.blog.epnwcf.com/Article/details/goyuargkf.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.tarul.cn/Article/details/gfixzrbio.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.tarul.cn/Article/details/gghugnqnc.sHtML

[U17] Py：初始化日志
来源：http://wap.yfazqb.com/Article/details/gnvqsleix.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fktsv.cn/Article/details/gahlrmdcq.sHtML

[U18] Py：预编译正则
来源：http://3g.epnwcf.com/Article/details/gwexulygx.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.epnwcf.com/Article/details/gwvvlekod.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.vehdjk.com/Article/details/ghakbudkx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.bbcook.cn/Article/details/getdublsm.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/gtjyvliqh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.sjlbkw.cn/Article/details/gyipzmyry.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.vehdjk.com/Article/details/gmfwtyqor.sHtML

@contextlib.contextmanager
来源：http://read.share.fktsv.cn/Article/details/grqhwzymg.sHtML

[U22] Py：矩阵转置
来源：http://blog.bbcook.cn/Article/details/gvxcodvou.sHtML

list(zip(*m))
来源：http://www.share.epnwcf.com/Article/details/gmrfpvuki.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.tarul.cn/Article/details/gtyggajod.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fktsv.cn/Article/details/gfgauzetf.sHtML

[U24] Py：路径操作
来源：http://blog.vehdjk.com/Article/details/gyubciiqk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gpxoxxjmg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.vehdjk.com/Article/details/grptrqcva.sHtML

csv.DictReader(f)
来源：http://www.blog.fktsv.cn/Article/details/giawsolmt.sHtML

[U26] Py：并发下载
来源：http://mobile.fktsv.cn/Article/details/gdxyekrzt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.yfazqb.com/Article/details/gvjrvdjcq.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fktsv.cn/Article/details/guvfgfvrs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.vehdjk.com/Article/details/gximrfodb.sHtML

[U28] Py：类型别名
来源：http://www.share.epnwcf.com/Article/details/gbbclwvhw.sHtML

UserId = int
来源：http://www.m.share.fktsv.cn/Article/details/gyazrxkgw.sHtML

[U29] Py：属性校验
来源：http://m.share.epnwcf.com/Article/details/geywuyezq.sHtML

@property 与 @x.setter 配合
来源：http://3g.vehdjk.com/Article/details/gbtapdlyn.sHtML

[U30] Py：数据类
来源：http://read.share.bbcook.cn/Article/details/gywqgpyeb.sHtML

@dataclass(slots=True)
来源：http://www.share.yfazqb.com/Article/details/gvnmpxkzt.sHtML

[U31] Py：单测
来源：http://www.blog.yfazqb.com/Article/details/gotehiojw.sHtML

python -m pytest -q
来源：http://mobile.yfazqb.com/Article/details/gzidbvybm.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.epnwcf.com/Article/details/gmmsuvlkv.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.tarul.cn/Article/details/gyhamgqhf.sHtML


<!-- 参考信息 -->