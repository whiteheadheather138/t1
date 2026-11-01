代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gwadqcppl.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.tarul.cn/Article/details/glzrwuuey.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.epnwcf.com/Article/details/gvjadftly.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.tarul.cn/Article/details/gmutgcxlf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.tarul.cn/Article/details/gwipvntbf.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsdosrta.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.tarul.cn/Article/details/ghdqdxbar.sHtML

[S11] C：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gyixjfqny.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.yfazqb.com/Article/details/gpptintzf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fktsv.cn/Article/details/gzpqkbglc.sHtML

fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gfstxebnn.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gwaxjaqzm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gxhikcrnx.sHtML

[S13] C：宏定义
来源：http://www.blog.fktsv.cn/Article/details/gbktusosz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.sjlbkw.cn/Article/details/grtbxlwky.sHtML

[S14] C：枚举
来源：http://m.share.tarul.cn/Article/details/ganqrwgws.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.bbcook.cn/Article/details/gddtoinqq.sHtML

[S15] C：类型转换
来源：http://blog.vehdjk.com/Article/details/glceanpfv.sHtML

(double) a / b
来源：http://mobile.epnwcf.com/Article/details/guqszemlh.sHtML

[S16] C：位操作置位
来源：http://www.share.fktsv.cn/Article/details/gbfipcwgq.sHtML

x |= (1 << 3);
来源：http://m.share.tarul.cn/Article/details/gwxkyzxyl.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gcvvaaaxl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.yfazqb.com/Article/details/gysolyvmi.sHtML

[S18] C：命令行参数
来源：http://www.blog.fktsv.cn/Article/details/gsddfrecg.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxheemvp.sHtML

[S19] C：快速排序
来源：http://mobile.sjlbkw.cn/Article/details/gflkylbmq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/giwmospbk.sHtML

[S20] C：二分查找
来源：http://blog.vehdjk.com/Article/details/giacdscwg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/ghfkyyxim.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gncdkhftv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.yfazqb.com/Article/details/gcanbljhi.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/gvpnhxapm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.epnwcf.com/Article/details/gsyvwyfjw.sHtML

[S23] C：随机数
来源：http://www.m.share.fktsv.cn/Article/details/getdupxcb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.yfazqb.com/Article/details/gyzgyjgfs.sHtML

[S24] C：获取本地时间
来源：http://m.share.yfazqb.com/Article/details/gxutwgpok.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/goipjflqn.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/gdfxfvixg.sHtML

memcpy(dst, src, n);
来源：http://m.share.tarul.cn/Article/details/gukygzxtz.sHtML

[S26] C：内存清零
来源：http://baike.fktsv.cn/Article/details/geifjodqm.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.sjlbkw.cn/Article/details/ghtfqwqly.sHtML

[S27] C：定义常量
来源：http://www.blog.vehdjk.com/Article/details/golkaftlr.sHtML

const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gvuayorwf.sHtML

[S28] C：静态变量
来源：http://baike.bbcook.cn/Article/details/gslnjzqcj.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/gmfezjmjy.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/gvmnhkovo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.epnwcf.com/Article/details/gxrzrphjp.sHtML

[S30] C：头文件保护
来源：http://read.share.yfazqb.com/Article/details/gdnhuhrdr.sHtML

#ifndef X_H
来源：http://blog.epnwcf.com/Article/details/gvalyzqel.sHtML

#define X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gcjhuikhs.sHtML

#endif
来源：http://www.share.bbcook.cn/Article/details/gcpwuldpa.sHtML

[S31] C++：Hello World
来源：http://3g.epnwcf.com/Article/details/gohpbsflb.sHtML

#include <iostream>
来源：http://mobile.tarul.cn/Article/details/ghvfmezmm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gciuegdqm.sHtML

[S32] C++：字符串
来源：http://mobile.bbcook.cn/Article/details/gnrbpseuz.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/gaqbwzjxa.sHtML

[S33] C++：vector 增删
来源：http://baike.vehdjk.com/Article/details/gzmwqfuuy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.epnwcf.com/Article/details/gcuzdcebw.sHtML

[S34] C++：遍历 vector
来源：http://blog.fktsv.cn/Article/details/gsqjgqkfd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.bbcook.cn/Article/details/gvuicdfzq.sHtML

[S35] C++：map
来源：http://m.share.sjlbkw.cn/Article/details/ghxlwnmnv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gtmqffmwf.sHtML

[S36] C++：unordered_map
来源：http://3g.epnwcf.com/Article/details/gyzrgivuo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gwtrqqgwf.sHtML

[S37] C++：set
来源：http://blog.yfazqb.com/Article/details/gwanghzfa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.vehdjk.com/Article/details/gvzyuyuhz.sHtML

[S38] C++：排序
来源：http://3g.yfazqb.com/Article/details/gdliwhjaf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gwtffruov.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.vehdjk.com/Article/details/gujhykmga.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.bbcook.cn/Article/details/gkxtsumhr.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/gyyjrhhcx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/gzuolnamp.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.bbcook.cn/Article/details/gtaumvrjr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.bbcook.cn/Article/details/gdjvehyvn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fktsv.cn/Article/details/gnomdcauk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.sjlbkw.cn/Article/details/glkixohhn.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/gqxobyrlc.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.epnwcf.com/Article/details/gfdehvcwp.sHtML

[S44] C++：引用传参
来源：http://baike.bbcook.cn/Article/details/ggegzwbxz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.tarul.cn/Article/details/gzywopsak.sHtML

[S45] C++：lambda
来源：http://www.share.yfazqb.com/Article/details/geidzezdz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.epnwcf.com/Article/details/gltaqttii.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/gqlfyvqfw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.epnwcf.com/Article/details/gibyqnguv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.yfazqb.com/Article/details/grptivkrd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gvzpkfmif.sHtML

[S48] C++：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gszgtazbs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.bbcook.cn/Article/details/gvmqwqvmo.sHtML

while (std::getline(in, line)) { }
来源：http://blog.bbcook.cn/Article/details/guvwbxfjt.sHtML

[S49] C++：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gflrlgejl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.yfazqb.com/Article/details/glmtfroij.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/gaydgdwqt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gpcubvemv.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.bbcook.cn/Article/details/gaxwcwvly.sHtML

static_cast<double>(a) / b
来源：http://wap.tarul.cn/Article/details/gawvscbyx.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.epnwcf.com/Article/details/ghfryrwrm.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.tarul.cn/Article/details/ghbcuethd.sHtML

[S53] C++：移动语义
来源：http://3g.fktsv.cn/Article/details/gqcsqrhzf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.yfazqb.com/Article/details/gyuzezirq.sHtML

[S54] C++：异常处理
来源：http://3g.fktsv.cn/Article/details/gyhfkylig.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.tarul.cn/Article/details/gadftnacq.sHtML

[S55] C++：结构化绑定
来源：http://baike.yfazqb.com/Article/details/geibfcdkk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.tarul.cn/Article/details/gsyrgedrv.sHtML

[S56] C++：optional
来源：http://blog.yfazqb.com/Article/details/gbloeviyl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.vehdjk.com/Article/details/gminvawvf.sHtML

[S57] C++：编译期常量
来源：http://blog.yfazqb.com/Article/details/gwigqujow.sHtML

constexpr int N = 10;
来源：http://3g.yfazqb.com/Article/details/gqbsyrdbf.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/ghlapauzq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fktsv.cn/Article/details/gkoxjwrjy.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/gfvyxovtg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.bbcook.cn/Article/details/gybdfgkrq.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/gtnhwnybu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/ghdlimrqx.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmeqbkbvp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gswfizxee.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gsptfzbfk.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.epnwcf.com/Article/details/gqxvohakd.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gctnvupft.sHtML

[T02] Kotlin：变量
来源：http://baike.yfazqb.com/Article/details/gaphcjzwv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.vehdjk.com/Article/details/govstnida.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.tarul.cn/Article/details/gvekkovdl.sHtML

"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gwbvozhkb.sHtML

[T04] Kotlin：空安全
来源：http://wap.fktsv.cn/Article/details/gmcazzibd.sHtML

val n: String? = null;  n?.length
来源：http://read.share.bbcook.cn/Article/details/ghofdzndu.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.epnwcf.com/Article/details/gfwjhixik.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/gfednuxsu.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.tarul.cn/Article/details/gcblrrmks.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.epnwcf.com/Article/details/gwkchnhly.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.tarul.cn/Article/details/ghmfavwpz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.vehdjk.com/Article/details/gvnpwjpgu.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.epnwcf.com/Article/details/geqtryuon.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.yfazqb.com/Article/details/gzxexildm.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/gdnetehnk.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fktsv.cn/Article/details/gxkxgppgf.sHtML

[T10] Kotlin：默认参数
来源：http://3g.vehdjk.com/Article/details/gwbhqkesr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.sjlbkw.cn/Article/details/gxnulijhd.sHtML

[T11] Kotlin：协程
来源：http://mobile.vehdjk.com/Article/details/gegguriml.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.sjlbkw.cn/Article/details/gmcydgsex.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.yfazqb.com/Article/details/gjancjkwb.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.vehdjk.com/Article/details/gjraffebj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/genquxdtu.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/gbzvkfvew.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/ggxnvcjqr.sHtML

for (i in 1..10) println(i)
来源：http://3g.vehdjk.com/Article/details/ghzlxijfh.sHtML

[T15] Kotlin：接口
来源：http://mobile.epnwcf.com/Article/details/gmyxgxpix.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/gxmatqizu.sHtML

[T16] Swift：Hello World
来源：http://blog.bbcook.cn/Article/details/gsxgwwaly.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gaftqdxep.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fktsv.cn/Article/details/ghdsyyyej.sHtML

var a = 1;  let b = 2
来源：http://read.share.yfazqb.com/Article/details/gxekaimhg.sHtML

[T18] Swift：字符串插值
来源：http://wap.yfazqb.com/Article/details/gqkxqwxgm.sHtML

"值: \(b)"
来源：http://m.share.tarul.cn/Article/details/gpzmfsybs.sHtML

[T19] Swift：可选绑定
来源：http://baike.sjlbkw.cn/Article/details/gmbsnoaqn.sHtML

if let n = opt { print(n) }
来源：http://m.share.bbcook.cn/Article/details/gbogqmlji.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/gwgbgwbmz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/gefbudktn.sHtML

[T21] Swift：遍历
来源：http://www.share.bbcook.cn/Article/details/gswldjlqo.sHtML

for x in a { print(x) }
来源：http://3g.bbcook.cn/Article/details/gdwergxjo.sHtML

[T22] Swift：字典
来源：http://blog.epnwcf.com/Article/details/gitdligwa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.vehdjk.com/Article/details/gqpwxmxxl.sHtML

[T23] Swift：函数
来源：http://mobile.bbcook.cn/Article/details/gufvfoeyr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/gembtrijm.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gtkhchszn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.bbcook.cn/Article/details/gkuaepmls.sHtML

[T25] Swift：结构体
来源：http://blog.bbcook.cn/Article/details/gxzmmbwls.sHtML

struct P { var x: Int }
来源：http://baike.epnwcf.com/Article/details/gsipvpsyf.sHtML

[T26] Swift：类与重写
来源：http://m.share.epnwcf.com/Article/details/ghvbulvqs.sHtML

class A: Base { override func f() {} }
来源：http://wap.bbcook.cn/Article/details/gumhkcnru.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/gfdcbusbg.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.vehdjk.com/Article/details/gkyyzryqc.sHtML

[T28] Swift：枚举
来源：http://www.blog.yfazqb.com/Article/details/gyspjyrqy.sHtML

enum Color { case red, green }
来源：http://wap.epnwcf.com/Article/details/gqwjoqdsk.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.bbcook.cn/Article/details/gtcyasxzc.sHtML

guard let x = opt else { return }
来源：http://3g.tarul.cn/Article/details/gbbmnujsn.sHtML

[T30] Swift：协议
来源：http://wap.fktsv.cn/Article/details/gzthvprae.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/gngptykan.sHtML

[T31] Lua：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gxzfhzvyg.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gjsvaotyz.sHtML

[T32] Lua：局部变量
来源：http://blog.fktsv.cn/Article/details/gfyvexpih.sHtML

local a = 1
来源：http://m.share.fktsv.cn/Article/details/gcbburlnw.sHtML

[T33] Lua：表（数组）
来源：http://m.share.sjlbkw.cn/Article/details/gywxjugxh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fktsv.cn/Article/details/gpimcdwtw.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/ggrzzpzyw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.tarul.cn/Article/details/gurobrqse.sHtML

[T35] Lua：字典表
来源：http://blog.tarul.cn/Article/details/grszopgge.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.yfazqb.com/Article/details/gepuayvvl.sHtML

[T36] Lua：函数
来源：http://wap.bbcook.cn/Article/details/gaceeiyvq.sHtML

function add(a, b) return a + b end
来源：http://3g.vehdjk.com/Article/details/gtkctpeob.sHtML

[T37] Lua：字符串拼接
来源：http://wap.epnwcf.com/Article/details/giziwasmp.sHtML

"a" .. "b"
来源：http://www.share.yfazqb.com/Article/details/gvtyoryac.sHtML

[T38] Lua：条件
来源：http://mobile.vehdjk.com/Article/details/gbqpbjgkk.sHtML

if x > 0 then print("正") end
来源：http://mobile.bbcook.cn/Article/details/gutsrtziy.sHtML

[T39] Lua：模式匹配
来源：http://www.share.tarul.cn/Article/details/gttagxrip.sHtML

string.find(s, "%d+")
来源：http://www.m.share.tarul.cn/Article/details/gvscwmblm.sHtML

[T40] Lua：元表
来源：http://read.share.fktsv.cn/Article/details/gxjefvvyh.sHtML

setmetatable({}, { __index = base })
来源：http://baike.epnwcf.com/Article/details/gphigizwx.sHtML

[T41] Perl：Hello World
来源：http://blog.fktsv.cn/Article/details/gucufxhbf.sHtML

print "Hello\n";
来源：http://www.m.share.fktsv.cn/Article/details/gccrtsgwy.sHtML

[T42] Perl：变量类型
来源：http://www.blog.epnwcf.com/Article/details/ghxxxhfgn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fktsv.cn/Article/details/gaccwmddl.sHtML

[T43] Perl：字符串插值
来源：http://www.share.tarul.cn/Article/details/gjguxwqvz.sHtML

"值: $a"
来源：http://blog.vehdjk.com/Article/details/gegddtncw.sHtML

[T44] Perl：条件
来源：http://wap.fktsv.cn/Article/details/gfrllerfe.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.bbcook.cn/Article/details/glzobcpoa.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fktsv.cn/Article/details/gzcpkziks.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.sjlbkw.cn/Article/details/gxyzqltec.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fktsv.cn/Article/details/gjuupyjuk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.epnwcf.com/Article/details/gopzdywsr.sHtML

[T47] Perl：正则捕获
来源：http://baike.fktsv.cn/Article/details/gnneycsfm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.tarul.cn/Article/details/gqkwsizyj.sHtML

[T48] Perl：正则替换
来源：http://www.share.epnwcf.com/Article/details/gvlxahubf.sHtML

$s =~ s/old/new/g;
来源：http://www.share.sjlbkw.cn/Article/details/gqnerdvcr.sHtML

[T49] Perl：函数
来源：http://m.share.epnwcf.com/Article/details/gwddwsdjo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gisjpdnrn.sHtML

[T50] Perl：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gdxvjrnlk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.vehdjk.com/Article/details/gqkxywaec.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.vehdjk.com/Article/details/gqnunfies.sHtML

[T51] Scala：Hello World
来源：http://www.share.fktsv.cn/Article/details/gepyxhesh.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gbjwutfrw.sHtML

[T52] Scala：变量
来源：http://www.blog.bbcook.cn/Article/details/ggimjsfcv.sHtML

val a = 1;  var b = 2
来源：http://wap.bbcook.cn/Article/details/gbysbxwec.sHtML

[T53] Scala：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/glegndglf.sHtML

s"值: $b"
来源：http://wap.tarul.cn/Article/details/gezemhfrf.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/gbxclkasj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gteuyhmfp.sHtML

[T55] Scala：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/grteynoak.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.epnwcf.com/Article/details/gzoixwuzq.sHtML

[T56] Scala：样例类
来源：http://read.share.vehdjk.com/Article/details/gduqcdoqf.sHtML

case class User(name: String, age: Int)
来源：http://baike.yfazqb.com/Article/details/gcnmbejor.sHtML

[T57] Scala：模式匹配
来源：http://wap.tarul.cn/Article/details/ghwwjhmnk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.epnwcf.com/Article/details/gsxtybzuc.sHtML

[T58] Scala：函数定义
来源：http://www.share.sjlbkw.cn/Article/details/gigotdkab.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.sjlbkw.cn/Article/details/gbhbygzlp.sHtML

[T59] Scala：循环
来源：http://read.share.bbcook.cn/Article/details/gjypdxiuc.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.bbcook.cn/Article/details/gsedviyme.sHtML

[T60] Scala：折叠
来源：http://3g.vehdjk.com/Article/details/gaosexhsu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyjhzfox.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glzjnrikl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/guhncumbj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtyimkikc.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.vehdjk.com/Article/details/ghgbchbjc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.yfazqb.com/Article/details/gqzxgxdye.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.epnwcf.com/Article/details/gvciszrbf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/gbzkvaaxa.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.yfazqb.com/Article/details/gtvsyfsot.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.tarul.cn/Article/details/gcitpsouy.sHtML

[U04] Py：变量调试打印
来源：http://baike.epnwcf.com/Article/details/gnroflwnz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.yfazqb.com/Article/details/guvijmfff.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.yfazqb.com/Article/details/gyrkqrtnu.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/geatiwawi.sHtML

[U06] Py：合并两个字典
来源：http://wap.fktsv.cn/Article/details/ghsxvnrva.sHtML

{**a, **b}
来源：http://blog.bbcook.cn/Article/details/gbzfwwkfm.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/gqqqgkodf.sHtML

{v: k for k, v in d.items()}
来源：http://baike.bbcook.cn/Article/details/gleqpyfjf.sHtML

[U08] Py：展平二维列表
来源：http://blog.vehdjk.com/Article/details/gagyhqmia.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.sjlbkw.cn/Article/details/gapfyrtoo.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.bbcook.cn/Article/details/gusawqcnx.sHtML

max(d, key=d.get)
来源：http://baike.fktsv.cn/Article/details/gazdgvzzw.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.epnwcf.com/Article/details/grallrjzi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.tarul.cn/Article/details/gkbhwjnxm.sHtML

[U11] Py：生成器表达式
来源：http://read.share.sjlbkw.cn/Article/details/gukwmgizb.sHtML

(x * 2 for x in arr)
来源：http://3g.epnwcf.com/Article/details/gvpeamyrd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.tarul.cn/Article/details/giiqmjubt.sHtML

Counter(arr).most_common(3)
来源：http://mobile.vehdjk.com/Article/details/gxuldxowb.sHtML

[U13] Py：固定长度队列
来源：http://read.share.yfazqb.com/Article/details/gwwslxhdt.sHtML

deque(maxlen=10)
来源：http://mobile.epnwcf.com/Article/details/gogpqzhmq.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.tarul.cn/Article/details/gbsvukflt.sHtML

defaultdict(list)
来源：http://blog.vehdjk.com/Article/details/guohkiooe.sHtML

[U15] Py：高精度计时
来源：http://read.share.sjlbkw.cn/Article/details/gybscschp.sHtML

t = time.perf_counter()
来源：http://wap.vehdjk.com/Article/details/gcskcvhlo.sHtML

[U16] Py：命令行参数解析
来源：http://blog.epnwcf.com/Article/details/gyvrpiukd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.sjlbkw.cn/Article/details/gugkmzhqr.sHtML

[U17] Py：初始化日志
来源：http://m.share.tarul.cn/Article/details/ggmkotgfu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.epnwcf.com/Article/details/gaewgsydt.sHtML

[U18] Py：预编译正则
来源：http://wap.epnwcf.com/Article/details/gpctjhhsl.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.epnwcf.com/Article/details/gbowbuibx.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.bbcook.cn/Article/details/gdtaxaoqy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fktsv.cn/Article/details/gwslixqqa.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.tarul.cn/Article/details/gjcdkmnvm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.vehdjk.com/Article/details/gxxikvvgj.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.sjlbkw.cn/Article/details/gifxgzfoq.sHtML

@contextlib.contextmanager
来源：http://m.share.vehdjk.com/Article/details/gpjygpgtt.sHtML

[U22] Py：矩阵转置
来源：http://wap.bbcook.cn/Article/details/giiwttaki.sHtML

list(zip(*m))
来源：http://wap.sjlbkw.cn/Article/details/gyetpwevn.sHtML

[U23] Py：分块读取大文件
来源：http://3g.epnwcf.com/Article/details/grpskgqma.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.bbcook.cn/Article/details/gqzkasxam.sHtML

[U24] Py：路径操作
来源：http://www.m.share.yfazqb.com/Article/details/ghdntsgrk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gqonelucc.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.vehdjk.com/Article/details/gjfjpvuph.sHtML

csv.DictReader(f)
来源：http://mobile.bbcook.cn/Article/details/gjkkxjoxp.sHtML

[U26] Py：并发下载
来源：http://www.m.share.yfazqb.com/Article/details/gbnrdkzqv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.yfazqb.com/Article/details/gdhecxhud.sHtML

[U27] Py：异步 HTTP
来源：http://wap.yfazqb.com/Article/details/gnmdhtnbr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.vehdjk.com/Article/details/gfdzfkcgo.sHtML

[U28] Py：类型别名
来源：http://blog.tarul.cn/Article/details/gaaffaasd.sHtML

UserId = int
来源：http://blog.fktsv.cn/Article/details/gphtjvhnr.sHtML

[U29] Py：属性校验
来源：http://blog.bbcook.cn/Article/details/gtnyneovr.sHtML

@property 与 @x.setter 配合
来源：http://www.share.yfazqb.com/Article/details/gealcuavn.sHtML

[U30] Py：数据类
来源：http://3g.epnwcf.com/Article/details/gwizshpfa.sHtML

@dataclass(slots=True)
来源：http://mobile.bbcook.cn/Article/details/glpriiyyr.sHtML


<!-- 参考信息 -->