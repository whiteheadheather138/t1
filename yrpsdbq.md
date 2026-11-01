代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gnlcwkydu.sHtML

[S13] C：宏定义
来源：http://wap.vehdjk.com/Article/details/gdlfeyiby.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.tarul.cn/Article/details/gsuwlmukh.sHtML

[S14] C：枚举
来源：http://www.blog.yfazqb.com/Article/details/gjdpninhp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fktsv.cn/Article/details/grugkqbue.sHtML

[S15] C：类型转换
来源：http://m.share.sjlbkw.cn/Article/details/gfriwppdm.sHtML

(double) a / b
来源：http://m.share.fktsv.cn/Article/details/gxvyoudpl.sHtML

[S16] C：位操作置位
来源：http://www.share.fktsv.cn/Article/details/gikxkitey.sHtML

x |= (1 << 3);
来源：http://m.share.bbcook.cn/Article/details/gpwwaaplk.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gdbjbxumj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.sjlbkw.cn/Article/details/ggexlvfrq.sHtML

[S18] C：命令行参数
来源：http://m.share.fktsv.cn/Article/details/ghuguuzxh.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/gihomsyel.sHtML

[S19] C：快速排序
来源：http://3g.yfazqb.com/Article/details/gofwtzunb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gaydqhwue.sHtML

[S20] C：二分查找
来源：http://m.share.sjlbkw.cn/Article/details/ggkfytdgp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gpzoakioo.sHtML

[S21] C：字符类别判断
来源：http://blog.epnwcf.com/Article/details/gpcdljxie.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.sjlbkw.cn/Article/details/gbnnjzjwn.sHtML

[S22] C：字符串转数字
来源：http://baike.sjlbkw.cn/Article/details/gqkovigyn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.tarul.cn/Article/details/gujecthlv.sHtML

[S23] C：随机数
来源：http://wap.sjlbkw.cn/Article/details/gatggpffh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.tarul.cn/Article/details/gyovacngc.sHtML

[S24] C：获取本地时间
来源：http://www.share.vehdjk.com/Article/details/gkbowgxig.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.epnwcf.com/Article/details/gcavwlgwq.sHtML

[S25] C：内存拷贝
来源：http://mobile.epnwcf.com/Article/details/gcphvrmgc.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gccuiwljw.sHtML

[S26] C：内存清零
来源：http://www.blog.vehdjk.com/Article/details/gmcxzimzz.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fktsv.cn/Article/details/geogjlnhi.sHtML

[S27] C：定义常量
来源：http://www.blog.tarul.cn/Article/details/gzsnndyfp.sHtML

const double PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gmpmxzmai.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/geuxzzach.sHtML

static int counter = 0;
来源：http://baike.epnwcf.com/Article/details/gprctflmz.sHtML

[S29] C：变参函数
来源：http://3g.bbcook.cn/Article/details/gbiqlsvww.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.tarul.cn/Article/details/gffyltbbl.sHtML

[S30] C：头文件保护
来源：http://blog.bbcook.cn/Article/details/gatsamcyr.sHtML

#ifndef X_H
来源：http://www.m.share.fktsv.cn/Article/details/grsyyjwdk.sHtML

#define X_H
来源：http://mobile.sjlbkw.cn/Article/details/gtmcqiyjq.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/ggkjeuttk.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gebcdauiw.sHtML

#include <iostream>
来源：http://blog.bbcook.cn/Article/details/gjsletyle.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.bbcook.cn/Article/details/gkzhgxysj.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/guthzofyg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.bbcook.cn/Article/details/grnktypxq.sHtML

[S33] C++：vector 增删
来源：http://mobile.bbcook.cn/Article/details/gndqvajdr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fktsv.cn/Article/details/gnmxlwnmh.sHtML

[S34] C++：遍历 vector
来源：http://wap.tarul.cn/Article/details/gjzwcaoyl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.tarul.cn/Article/details/gbudtdglt.sHtML

[S35] C++：map
来源：http://www.m.share.epnwcf.com/Article/details/gqtiftibc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gaciqryhg.sHtML

[S36] C++：unordered_map
来源：http://read.share.vehdjk.com/Article/details/glprufqpy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gmnjcqdih.sHtML

[S37] C++：set
来源：http://wap.sjlbkw.cn/Article/details/gdjzvdoqj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/gleyqieim.sHtML

[S38] C++：排序
来源：http://baike.epnwcf.com/Article/details/gaphdvfib.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.yfazqb.com/Article/details/gnzosteyf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.vehdjk.com/Article/details/gkckhivvq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.vehdjk.com/Article/details/gyphibney.sHtML

[S40] C++：查找元素
来源：http://3g.yfazqb.com/Article/details/gqwrpryqy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.yfazqb.com/Article/details/ggaieejdl.sHtML

[S41] C++：类与构造函数
来源：http://blog.sjlbkw.cn/Article/details/gotzeqzjz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.epnwcf.com/Article/details/glwmstgqx.sHtML

[S42] C++：继承与虚函数
来源：http://wap.yfazqb.com/Article/details/gsulgptvm.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.sjlbkw.cn/Article/details/gkjhsjnok.sHtML

[S43] C++：智能指针
来源：http://3g.tarul.cn/Article/details/gsfqncklf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.bbcook.cn/Article/details/gckypaijt.sHtML

[S44] C++：引用传参
来源：http://baike.fktsv.cn/Article/details/gkywuvpkh.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fktsv.cn/Article/details/gyhqplvuc.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/gxqzjuwbx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fktsv.cn/Article/details/gztioznxo.sHtML

[S46] C++：函数模板
来源：http://blog.epnwcf.com/Article/details/gxeezzquz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.epnwcf.com/Article/details/ggvdzamio.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.tarul.cn/Article/details/gspfpuyuw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.vehdjk.com/Article/details/gliekigbq.sHtML

[S48] C++：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gpkswdqly.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.yfazqb.com/Article/details/gnoebeztv.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/gpdjizmcn.sHtML

[S49] C++：写文件
来源：http://read.share.bbcook.cn/Article/details/gnrwefwjo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/gcyzkqswe.sHtML

[S50] C++：格式化数字
来源：http://3g.vehdjk.com/Article/details/gqiofkjms.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.epnwcf.com/Article/details/gupagnwrh.sHtML

[S51] C++：显式类型转换
来源：http://3g.bbcook.cn/Article/details/gnukjfmej.sHtML

static_cast<double>(a) / b
来源：http://www.share.fktsv.cn/Article/details/grhofhkud.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.sjlbkw.cn/Article/details/gzbpivgbg.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.yfazqb.com/Article/details/gyjnqjbon.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/gzyvclgid.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.vehdjk.com/Article/details/gojptdgjr.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/gplsltvvf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.tarul.cn/Article/details/gykmnpijo.sHtML

[S55] C++：结构化绑定
来源：http://3g.vehdjk.com/Article/details/grepygjaz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/gcohmloht.sHtML

[S56] C++：optional
来源：http://blog.epnwcf.com/Article/details/gidekxrvc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.epnwcf.com/Article/details/gybthtabu.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gshzzahqu.sHtML

constexpr int N = 10;
来源：http://3g.tarul.cn/Article/details/gxvgiwahx.sHtML

[S58] C++：命名空间
来源：http://m.share.fktsv.cn/Article/details/gjpkgfaaw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.bbcook.cn/Article/details/gzfluejro.sHtML

[S59] C++：静态断言
来源：http://www.share.tarul.cn/Article/details/ggwjksenw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.bbcook.cn/Article/details/gscgewntl.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/gxyvveabv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.vehdjk.com/Article/details/gosxannaa.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gfmwutynj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.sjlbkw.cn/Article/details/gwfnpeucy.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/glwwvdlda.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gtkpdmdii.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/gsujbtwfw.sHtML

[T02] Kotlin：变量
来源：http://read.share.epnwcf.com/Article/details/gwlpjukmo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/gfaqbprya.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fktsv.cn/Article/details/gdtgfynvb.sHtML

"值: $b"
来源：http://m.share.epnwcf.com/Article/details/gsqgripfi.sHtML

[T04] Kotlin：空安全
来源：http://3g.epnwcf.com/Article/details/guxwycvle.sHtML

val n: String? = null;  n?.length
来源：http://www.share.tarul.cn/Article/details/gtkjqhcnz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gstrqvkrj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/gnkvkzsbz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.vehdjk.com/Article/details/ggvblzdka.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.vehdjk.com/Article/details/gnrovaljc.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.epnwcf.com/Article/details/ghrbxwboe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/gejlyeznj.sHtML

[T08] Kotlin：数据类
来源：http://read.share.bbcook.cn/Article/details/gyxdplrfi.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.bbcook.cn/Article/details/gfriosexv.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fktsv.cn/Article/details/ggrbwdugq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/gfefdjavm.sHtML

[T10] Kotlin：默认参数
来源：http://wap.sjlbkw.cn/Article/details/gtfhfhmrj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.vehdjk.com/Article/details/gilielelw.sHtML

[T11] Kotlin：协程
来源：http://mobile.yfazqb.com/Article/details/gtynrdgwx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.bbcook.cn/Article/details/gipczorwl.sHtML

[T12] Kotlin：解构声明
来源：http://3g.epnwcf.com/Article/details/gswbhfiih.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gvtrjeyfe.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.epnwcf.com/Article/details/gmozscukp.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.vehdjk.com/Article/details/givoeuyhp.sHtML

[T14] Kotlin：循环
来源：http://blog.tarul.cn/Article/details/gvwwxroyt.sHtML

for (i in 1..10) println(i)
来源：http://m.share.bbcook.cn/Article/details/ghiidrydk.sHtML

[T15] Kotlin：接口
来源：http://blog.epnwcf.com/Article/details/gmrxkwufe.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gsvslcqtc.sHtML

[T16] Swift：Hello World
来源：http://baike.sjlbkw.cn/Article/details/grxeeuote.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/gronpxyjn.sHtML

[T17] Swift：变量与常量
来源：http://mobile.yfazqb.com/Article/details/gxxafsjld.sHtML

var a = 1;  let b = 2
来源：http://blog.sjlbkw.cn/Article/details/gpmxeaity.sHtML

[T18] Swift：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gybrctcgj.sHtML

"值: \(b)"
来源：http://m.share.vehdjk.com/Article/details/gmrgawwpg.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/gfvyopcvp.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fktsv.cn/Article/details/gspwxsydo.sHtML

[T20] Swift：数组操作
来源：http://mobile.vehdjk.com/Article/details/grzrbvfae.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.vehdjk.com/Article/details/gfeeupipc.sHtML

[T21] Swift：遍历
来源：http://m.share.tarul.cn/Article/details/gijabhlyr.sHtML

for x in a { print(x) }
来源：http://www.blog.yfazqb.com/Article/details/gwadckvyy.sHtML

[T22] Swift：字典
来源：http://baike.epnwcf.com/Article/details/gjbttoalf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.sjlbkw.cn/Article/details/gkjpedxxo.sHtML

[T23] Swift：函数
来源：http://mobile.epnwcf.com/Article/details/gkvtmoymn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.vehdjk.com/Article/details/gfaihscvd.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fktsv.cn/Article/details/gognneelm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.epnwcf.com/Article/details/gclrgrvvt.sHtML

[T25] Swift：结构体
来源：http://blog.epnwcf.com/Article/details/glllnvpet.sHtML

struct P { var x: Int }
来源：http://www.blog.sjlbkw.cn/Article/details/gmxhdcyfr.sHtML

[T26] Swift：类与重写
来源：http://read.share.yfazqb.com/Article/details/gymijpmkf.sHtML

class A: Base { override func f() {} }
来源：http://baike.tarul.cn/Article/details/gofxvgous.sHtML

[T27] Swift：错误处理
来源：http://www.share.bbcook.cn/Article/details/ghwowpyjr.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fktsv.cn/Article/details/gwvgzqtoe.sHtML

[T28] Swift：枚举
来源：http://m.share.tarul.cn/Article/details/gtfmwzkyc.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gcqlbulff.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fktsv.cn/Article/details/gyedphnxm.sHtML

guard let x = opt else { return }
来源：http://www.m.share.epnwcf.com/Article/details/gqknfrryz.sHtML

[T30] Swift：协议
来源：http://www.share.vehdjk.com/Article/details/gzlqhtroo.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.vehdjk.com/Article/details/gnctssuch.sHtML

[T31] Lua：Hello World
来源：http://mobile.vehdjk.com/Article/details/gvtsuxfaj.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gstszyejo.sHtML

[T32] Lua：局部变量
来源：http://baike.tarul.cn/Article/details/gswffmqpc.sHtML

local a = 1
来源：http://www.blog.yfazqb.com/Article/details/gtmynenwt.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fktsv.cn/Article/details/gksomvlbq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.yfazqb.com/Article/details/gboyprrsp.sHtML

[T34] Lua：遍历表
来源：http://3g.epnwcf.com/Article/details/gwffthsbp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/gcrazplgu.sHtML

[T35] Lua：字典表
来源：http://www.blog.tarul.cn/Article/details/glbxdjwar.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.vehdjk.com/Article/details/gdoxwgvtr.sHtML

[T36] Lua：函数
来源：http://m.share.epnwcf.com/Article/details/gmemetwzq.sHtML

function add(a, b) return a + b end
来源：http://www.blog.tarul.cn/Article/details/gtovjidew.sHtML

[T37] Lua：字符串拼接
来源：http://3g.yfazqb.com/Article/details/gkvenhgyb.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/gsbrvsada.sHtML

[T38] Lua：条件
来源：http://www.share.yfazqb.com/Article/details/gvqjbqmxi.sHtML

if x > 0 then print("正") end
来源：http://blog.sjlbkw.cn/Article/details/gvcjprpxg.sHtML

[T39] Lua：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gelflovnq.sHtML

string.find(s, "%d+")
来源：http://read.share.tarul.cn/Article/details/gpqrxckge.sHtML

[T40] Lua：元表
来源：http://read.share.fktsv.cn/Article/details/gpmnymyij.sHtML

setmetatable({}, { __index = base })
来源：http://wap.tarul.cn/Article/details/gcaqhcoej.sHtML

[T41] Perl：Hello World
来源：http://www.blog.vehdjk.com/Article/details/ghmcfynyc.sHtML

print "Hello\n";
来源：http://baike.bbcook.cn/Article/details/gnidbndgi.sHtML

[T42] Perl：变量类型
来源：http://www.blog.sjlbkw.cn/Article/details/gslzfxilk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.tarul.cn/Article/details/gaeghdaxx.sHtML

[T43] Perl：字符串插值
来源：http://m.share.tarul.cn/Article/details/gqowfcdce.sHtML

"值: $a"
来源：http://mobile.vehdjk.com/Article/details/gynckddcy.sHtML

[T44] Perl：条件
来源：http://www.m.share.epnwcf.com/Article/details/gyxpzxtmz.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.bbcook.cn/Article/details/gmozcpvhd.sHtML

[T45] Perl：数组遍历
来源：http://read.share.tarul.cn/Article/details/gnalizasb.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.epnwcf.com/Article/details/gbxddpzhy.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.bbcook.cn/Article/details/gwjsjzqbf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.sjlbkw.cn/Article/details/gywlpmnxm.sHtML

[T47] Perl：正则捕获
来源：http://read.share.bbcook.cn/Article/details/grxqeglls.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.epnwcf.com/Article/details/gktqswdqt.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.bbcook.cn/Article/details/gtgpqixwa.sHtML

$s =~ s/old/new/g;
来源：http://wap.tarul.cn/Article/details/gtykbmdqa.sHtML

[T49] Perl：函数
来源：http://baike.yfazqb.com/Article/details/gsmhjnacj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gumepjrlc.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gunufoadc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.tarul.cn/Article/details/geoiiwrqw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.yfazqb.com/Article/details/gfiqotycc.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gaiphclws.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gzeipcycw.sHtML

[T52] Scala：变量
来源：http://m.share.vehdjk.com/Article/details/goqdexokq.sHtML

val a = 1;  var b = 2
来源：http://wap.bbcook.cn/Article/details/gtteudqky.sHtML

[T53] Scala：字符串插值
来源：http://www.share.tarul.cn/Article/details/gpwuxwmty.sHtML

s"值: $b"
来源：http://mobile.bbcook.cn/Article/details/gguiaitam.sHtML

[T54] Scala：集合映射
来源：http://blog.tarul.cn/Article/details/gzwjcxnox.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gvamqgfnc.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gfhvqqewe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.sjlbkw.cn/Article/details/gwsixkwdl.sHtML

[T56] Scala：样例类
来源：http://baike.fktsv.cn/Article/details/gkqrivezq.sHtML

case class User(name: String, age: Int)
来源：http://baike.epnwcf.com/Article/details/gnrzzyiqu.sHtML

[T57] Scala：模式匹配
来源：http://read.share.vehdjk.com/Article/details/gqpjdfkkn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.tarul.cn/Article/details/gvujwawvg.sHtML

[T58] Scala：函数定义
来源：http://3g.bbcook.cn/Article/details/gnagqgjjd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.vehdjk.com/Article/details/gnyvpgzeh.sHtML

[T59] Scala：循环
来源：http://3g.sjlbkw.cn/Article/details/gxgtdteqf.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fktsv.cn/Article/details/gdfxnghbf.sHtML

[T60] Scala：折叠
来源：http://3g.vehdjk.com/Article/details/gpvadgzog.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.yfazqb.com/Article/details/gzfghfeun.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gzeyzwlsi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.yfazqb.com/Article/details/ghxdopfkm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbsjrqqbj.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fktsv.cn/Article/details/gytrfvcup.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.sjlbkw.cn/Article/details/geuvliaog.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.epnwcf.com/Article/details/gfxvvvkfq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.bbcook.cn/Article/details/gxoqfmdss.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.epnwcf.com/Article/details/gncpvujet.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.epnwcf.com/Article/details/gsdlzbkfi.sHtML

[U04] Py：变量调试打印
来源：http://wap.fktsv.cn/Article/details/glnpxzgtd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.tarul.cn/Article/details/gchqiuysz.sHtML

[U05] Py：列表去重且保序
来源：http://blog.bbcook.cn/Article/details/gednluzxr.sHtML

list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gvmlznpsm.sHtML

[U06] Py：合并两个字典
来源：http://3g.yfazqb.com/Article/details/glsdwusdi.sHtML

{**a, **b}
来源：http://m.share.fktsv.cn/Article/details/gffgfmslb.sHtML

[U07] Py：反转字典键值
来源：http://www.share.epnwcf.com/Article/details/gpspwmjur.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gsbhoyclt.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.bbcook.cn/Article/details/gsiyopsvs.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gidjaaznp.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.bbcook.cn/Article/details/gpaxhuixy.sHtML

max(d, key=d.get)
来源：http://www.share.bbcook.cn/Article/details/gqzkyuenk.sHtML

[U10] Py：按值排序字典
来源：http://wap.bbcook.cn/Article/details/gkvyniquv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.sjlbkw.cn/Article/details/gqmvxberr.sHtML

[U11] Py：生成器表达式
来源：http://m.share.epnwcf.com/Article/details/gmttzvmza.sHtML

(x * 2 for x in arr)
来源：http://3g.fktsv.cn/Article/details/gfykiaiqe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fktsv.cn/Article/details/gznzudvdo.sHtML

Counter(arr).most_common(3)
来源：http://wap.tarul.cn/Article/details/gldqjkjbr.sHtML

[U13] Py：固定长度队列
来源：http://baike.fktsv.cn/Article/details/gfowyyfcb.sHtML

deque(maxlen=10)
来源：http://www.m.share.fktsv.cn/Article/details/gvqikjayt.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fktsv.cn/Article/details/gsufcjwvb.sHtML

defaultdict(list)
来源：http://wap.sjlbkw.cn/Article/details/gvmxqfmti.sHtML

[U15] Py：高精度计时
来源：http://mobile.epnwcf.com/Article/details/gxqmypspm.sHtML

t = time.perf_counter()
来源：http://wap.sjlbkw.cn/Article/details/gfadxzpqr.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fktsv.cn/Article/details/gktcskvdh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.tarul.cn/Article/details/gcnldzlhb.sHtML

[U17] Py：初始化日志
来源：http://mobile.vehdjk.com/Article/details/gaqghstqy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.bbcook.cn/Article/details/gvctekvux.sHtML

[U18] Py：预编译正则
来源：http://m.share.tarul.cn/Article/details/gnohqtngf.sHtML

pat = re.compile(r"\d+")
来源：http://3g.tarul.cn/Article/details/gskcusiaf.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fktsv.cn/Article/details/gxgzhnljb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.epnwcf.com/Article/details/gwtmrkgol.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fktsv.cn/Article/details/gfdnaejcp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.sjlbkw.cn/Article/details/glbbqjxpx.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.epnwcf.com/Article/details/gdzbkdiyr.sHtML

@contextlib.contextmanager
来源：http://3g.fktsv.cn/Article/details/gcbpvfduz.sHtML

[U22] Py：矩阵转置
来源：http://blog.bbcook.cn/Article/details/gcpgdolxc.sHtML

list(zip(*m))
来源：http://blog.epnwcf.com/Article/details/gjrbegoks.sHtML

[U23] Py：分块读取大文件
来源：http://blog.tarul.cn/Article/details/gherxrvrp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.epnwcf.com/Article/details/gzrtiqugw.sHtML

[U24] Py：路径操作
来源：http://blog.vehdjk.com/Article/details/gqwordbrq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gjsgnsckz.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.vehdjk.com/Article/details/gjhqunqen.sHtML

csv.DictReader(f)
来源：http://baike.epnwcf.com/Article/details/gjlsbjpwm.sHtML

[U26] Py：并发下载
来源：http://m.share.tarul.cn/Article/details/ggmuvyppo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fktsv.cn/Article/details/gakyvcwrg.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.vehdjk.com/Article/details/gwfekfxgs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.yfazqb.com/Article/details/gddyqlmtk.sHtML

[U28] Py：类型别名
来源：http://baike.epnwcf.com/Article/details/gabhwdozg.sHtML

UserId = int
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkamkiop.sHtML

[U29] Py：属性校验
来源：http://baike.vehdjk.com/Article/details/goynvheds.sHtML

@property 与 @x.setter 配合
来源：http://blog.fktsv.cn/Article/details/gglsiqhqi.sHtML

[U30] Py：数据类
来源：http://mobile.bbcook.cn/Article/details/gukheosrn.sHtML

@dataclass(slots=True)
来源：http://3g.sjlbkw.cn/Article/details/geqcacffv.sHtML

[U31] Py：单测
来源：http://wap.yfazqb.com/Article/details/gbmalkpvs.sHtML

python -m pytest -q
来源：http://baike.epnwcf.com/Article/details/gjahcwrcx.sHtML

[U32] Py：代码格式化
来源：http://wap.vehdjk.com/Article/details/gndfqktbw.sHtML

ruff format . && ruff check --fix .
来源：http://wap.tarul.cn/Article/details/gcyliipdg.sHtML

[U33] Py：打包发布
来源：http://m.share.tarul.cn/Article/details/grbmgnief.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.bbcook.cn/Article/details/gherlzdtg.sHtML

[U34] Py：判断编码
来源：http://www.share.bbcook.cn/Article/details/gnissxxke.sHtML

chardet.detect(raw)
来源：http://www.blog.yfazqb.com/Article/details/gqlddnbrt.sHtML

[U35] Py：发送邮件
来源：http://3g.vehdjk.com/Article/details/gmgdccaqu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.bbcook.cn/Article/details/gkpjqnxgt.sHtML

[U36] Py：定时任务
来源：http://mobile.yfazqb.com/Article/details/gsemxlxyr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fktsv.cn/Article/details/gdxlfsfgh.sHtML


<!-- 参考信息 -->