代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://read.share.sjlbkw.cn/Article/details/gmwulubtb.sHtML

[S15] C：类型转换
来源：http://www.blog.tarul.cn/Article/details/grckluvdx.sHtML

(double) a / b
来源：http://baike.fktsv.cn/Article/details/gmnpowaua.sHtML

[S16] C：位操作置位
来源：http://www.share.tarul.cn/Article/details/gnkebshuv.sHtML

x |= (1 << 3);
来源：http://3g.bbcook.cn/Article/details/gjnmnhdfu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.bbcook.cn/Article/details/gcxkhilkt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/gxmoqiffp.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/ginqmnnbd.sHtML

int main(int argc, char **argv)
来源：http://baike.sjlbkw.cn/Article/details/gbximtsbx.sHtML

[S19] C：快速排序
来源：http://wap.tarul.cn/Article/details/gsxplsssk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gelufxicv.sHtML

[S20] C：二分查找
来源：http://wap.vehdjk.com/Article/details/glolikbyw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gkfuluynt.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/gmzvwzkpw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.vehdjk.com/Article/details/gwxnbaina.sHtML

[S22] C：字符串转数字
来源：http://baike.bbcook.cn/Article/details/ggjxolheq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.sjlbkw.cn/Article/details/gblpjnqjy.sHtML

[S23] C：随机数
来源：http://www.blog.yfazqb.com/Article/details/gkgmrqgex.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/gvyccofwo.sHtML

[S24] C：获取本地时间
来源：http://blog.bbcook.cn/Article/details/gqhkhchti.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/ggtodronp.sHtML

[S25] C：内存拷贝
来源：http://baike.epnwcf.com/Article/details/gkpgdoljr.sHtML

memcpy(dst, src, n);
来源：http://wap.sjlbkw.cn/Article/details/ghiabzbbw.sHtML

[S26] C：内存清零
来源：http://www.blog.fktsv.cn/Article/details/gftphohfn.sHtML

memset(a, 0, sizeof a);
来源：http://blog.tarul.cn/Article/details/ghqmpswrc.sHtML

[S27] C：定义常量
来源：http://m.share.fktsv.cn/Article/details/gnjpgsoty.sHtML

const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gxqwfxiim.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/gtdoptuds.sHtML

static int counter = 0;
来源：http://m.share.fktsv.cn/Article/details/gkorlenub.sHtML

[S29] C：变参函数
来源：http://mobile.tarul.cn/Article/details/gmulyqnlb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.yfazqb.com/Article/details/gnivpsrrb.sHtML

[S30] C：头文件保护
来源：http://read.share.epnwcf.com/Article/details/gzazyxstw.sHtML

#ifndef X_H
来源：http://www.share.vehdjk.com/Article/details/gcwtrcedc.sHtML

#define X_H
来源：http://www.share.fktsv.cn/Article/details/gmpwiqeru.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/guodqolyr.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/glqznfmpp.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/gbefocgrm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.sjlbkw.cn/Article/details/gmllprttm.sHtML

[S32] C++：字符串
来源：http://www.share.sjlbkw.cn/Article/details/gnxnsvzsk.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.vehdjk.com/Article/details/ghskzfyfo.sHtML

[S33] C++：vector 增删
来源：http://baike.tarul.cn/Article/details/gfftojwqt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.yfazqb.com/Article/details/gnvuqaecr.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.epnwcf.com/Article/details/getieqrdv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.yfazqb.com/Article/details/gtobnsyxm.sHtML

[S35] C++：map
来源：http://read.share.sjlbkw.cn/Article/details/gyyjpqaxv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gkimtkqrc.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/gbabtoabs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gvbdaruny.sHtML

[S37] C++：set
来源：http://read.share.sjlbkw.cn/Article/details/gihtbthwm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/gsmdkptkv.sHtML

[S38] C++：排序
来源：http://www.share.vehdjk.com/Article/details/gnbraxxbh.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.yfazqb.com/Article/details/gxdiqgmyc.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fktsv.cn/Article/details/gjyjtypiq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.vehdjk.com/Article/details/gofvlmffv.sHtML

[S40] C++：查找元素
来源：http://baike.yfazqb.com/Article/details/gboqzdpzl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.bbcook.cn/Article/details/gdskziooq.sHtML

[S41] C++：类与构造函数
来源：http://mobile.vehdjk.com/Article/details/ggzejhfqh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.bbcook.cn/Article/details/gfuymcyfc.sHtML

[S42] C++：继承与虚函数
来源：http://wap.tarul.cn/Article/details/gberltfbs.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.bbcook.cn/Article/details/gtipdiakp.sHtML

[S43] C++：智能指针
来源：http://www.share.vehdjk.com/Article/details/gxjalaihm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.tarul.cn/Article/details/gttfvlotr.sHtML

[S44] C++：引用传参
来源：http://mobile.epnwcf.com/Article/details/gnkefuayg.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.yfazqb.com/Article/details/gboohpttu.sHtML

[S45] C++：lambda
来源：http://www.blog.yfazqb.com/Article/details/ghjnjyisg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.yfazqb.com/Article/details/ggbzgxiei.sHtML

[S46] C++：函数模板
来源：http://3g.bbcook.cn/Article/details/gxssgpquf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/gqjepjchk.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fktsv.cn/Article/details/gffmetyzd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gtrighmgf.sHtML

[S48] C++：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gyuhoqnew.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.tarul.cn/Article/details/gwpdufutr.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.yfazqb.com/Article/details/gdfysnsyi.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/guxailsfe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/gvftwocwe.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fktsv.cn/Article/details/gxuutpjtf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/gxgufjngf.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/gvizovxwj.sHtML

static_cast<double>(a) / b
来源：http://read.share.epnwcf.com/Article/details/gsjibxqkq.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.bbcook.cn/Article/details/gvocbeerr.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.tarul.cn/Article/details/gnyqnnbos.sHtML

[S53] C++：移动语义
来源：http://baike.sjlbkw.cn/Article/details/gycbvmmxr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.epnwcf.com/Article/details/gatnmzubi.sHtML

[S54] C++：异常处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gzthllxoi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.sjlbkw.cn/Article/details/gyphqhbfu.sHtML

[S55] C++：结构化绑定
来源：http://wap.tarul.cn/Article/details/gylopytla.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.vehdjk.com/Article/details/gghisxidm.sHtML

[S56] C++：optional
来源：http://wap.sjlbkw.cn/Article/details/gcqjbzrus.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/guajbdnap.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.tarul.cn/Article/details/guibzywxh.sHtML

constexpr int N = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gmbutektz.sHtML

[S58] C++：命名空间
来源：http://wap.sjlbkw.cn/Article/details/gbwcjrkie.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.vehdjk.com/Article/details/gtbqpsmds.sHtML

[S59] C++：静态断言
来源：http://www.share.sjlbkw.cn/Article/details/gubfyanvw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/godglrqao.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.epnwcf.com/Article/details/gbxzineko.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.yfazqb.com/Article/details/gtrwbccgc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ggwnigzrm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/glavirmhr.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfwzddhyp.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/gcwxeblln.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gmkjwlxou.sHtML

[T02] Kotlin：变量
来源：http://www.blog.bbcook.cn/Article/details/ghnmmbhql.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fktsv.cn/Article/details/gsxeoezkh.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/gotniogcg.sHtML

"值: $b"
来源：http://read.share.vehdjk.com/Article/details/gtmvwhzet.sHtML

[T04] Kotlin：空安全
来源：http://baike.vehdjk.com/Article/details/gxrwrzbzg.sHtML

val n: String? = null;  n?.length
来源：http://mobile.epnwcf.com/Article/details/gaxbhhefz.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.bbcook.cn/Article/details/ghcmtwzxr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fktsv.cn/Article/details/gtvwbtqwg.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.tarul.cn/Article/details/ghfoxvgha.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/glcmlwfnk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.yfazqb.com/Article/details/gqitzmtnx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.sjlbkw.cn/Article/details/glfsyxrpy.sHtML

[T08] Kotlin：数据类
来源：http://blog.vehdjk.com/Article/details/gfytyirwn.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fktsv.cn/Article/details/gnwhuahfk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.yfazqb.com/Article/details/gngasazmz.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.epnwcf.com/Article/details/gyrlpntfx.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fktsv.cn/Article/details/gugblhoms.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.sjlbkw.cn/Article/details/gpbalznvr.sHtML

[T11] Kotlin：协程
来源：http://www.share.yfazqb.com/Article/details/gnglihezm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.tarul.cn/Article/details/gavrtnwjc.sHtML

[T12] Kotlin：解构声明
来源：http://baike.yfazqb.com/Article/details/gpbjenckj.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.vehdjk.com/Article/details/glrzevicx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/guplbcste.sHtML

val m = mapOf("a" to 1)
来源：http://baike.bbcook.cn/Article/details/gvxslvksu.sHtML

[T14] Kotlin：循环
来源：http://blog.tarul.cn/Article/details/gguegzdix.sHtML

for (i in 1..10) println(i)
来源：http://blog.fktsv.cn/Article/details/gcqhhxgmm.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/gvnoehbid.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/gjdcezwbz.sHtML

[T16] Swift：Hello World
来源：http://3g.bbcook.cn/Article/details/gdcwblamo.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gmbzytdsb.sHtML

[T17] Swift：变量与常量
来源：http://baike.bbcook.cn/Article/details/gwpkmxbtv.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fktsv.cn/Article/details/ggrivhwbz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gwubetnqk.sHtML

"值: \(b)"
来源：http://wap.yfazqb.com/Article/details/gzodjyvgm.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gxpyzwput.sHtML

if let n = opt { print(n) }
来源：http://mobile.sjlbkw.cn/Article/details/gipazgauj.sHtML

[T20] Swift：数组操作
来源：http://www.share.sjlbkw.cn/Article/details/gwsahgfnf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fktsv.cn/Article/details/gnygezfaf.sHtML

[T21] Swift：遍历
来源：http://wap.tarul.cn/Article/details/gqygydpjo.sHtML

for x in a { print(x) }
来源：http://www.blog.epnwcf.com/Article/details/gmlymfitk.sHtML

[T22] Swift：字典
来源：http://m.share.yfazqb.com/Article/details/gwckpcwoy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.tarul.cn/Article/details/gygofkapl.sHtML

[T23] Swift：函数
来源：http://read.share.vehdjk.com/Article/details/gffganbjm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.tarul.cn/Article/details/gsujzzywj.sHtML

[T24] Swift：闭包
来源：http://www.blog.sjlbkw.cn/Article/details/gpjlonsgg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.yfazqb.com/Article/details/gyphnfilx.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/gfvezgjvz.sHtML

struct P { var x: Int }
来源：http://www.share.bbcook.cn/Article/details/gajuchfat.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/gmdtmzljh.sHtML

class A: Base { override func f() {} }
来源：http://mobile.yfazqb.com/Article/details/gtkjmaigk.sHtML

[T27] Swift：错误处理
来源：http://baike.epnwcf.com/Article/details/gbsdsgtue.sHtML

do { try f() } catch { print(error) }
来源：http://wap.vehdjk.com/Article/details/gcpaiubvq.sHtML

[T28] Swift：枚举
来源：http://3g.bbcook.cn/Article/details/giwwewsrt.sHtML

enum Color { case red, green }
来源：http://www.blog.bbcook.cn/Article/details/gmoqokdga.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.sjlbkw.cn/Article/details/gwpxvplwz.sHtML

guard let x = opt else { return }
来源：http://wap.epnwcf.com/Article/details/gmfyewgrg.sHtML

[T30] Swift：协议
来源：http://www.m.share.vehdjk.com/Article/details/gumagbloh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.vehdjk.com/Article/details/gbuhxmmva.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gulijttuk.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gsngjkjzx.sHtML

[T32] Lua：局部变量
来源：http://m.share.tarul.cn/Article/details/gxvjmcegg.sHtML

local a = 1
来源：http://read.share.vehdjk.com/Article/details/ghwhslrzw.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.yfazqb.com/Article/details/givtxxjbt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fktsv.cn/Article/details/gyovqhdpn.sHtML

[T34] Lua：遍历表
来源：http://baike.vehdjk.com/Article/details/gzghiytub.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.vehdjk.com/Article/details/gbdqwfvgs.sHtML

[T35] Lua：字典表
来源：http://wap.epnwcf.com/Article/details/gcgzsesff.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.bbcook.cn/Article/details/gulhqqtli.sHtML

[T36] Lua：函数
来源：http://mobile.bbcook.cn/Article/details/gjsinhoma.sHtML

function add(a, b) return a + b end
来源：http://blog.epnwcf.com/Article/details/gaxoshvmn.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.bbcook.cn/Article/details/gruxurhdu.sHtML

"a" .. "b"
来源：http://www.share.vehdjk.com/Article/details/gpnbfdcfh.sHtML

[T38] Lua：条件
来源：http://read.share.bbcook.cn/Article/details/gtgtepimi.sHtML

if x > 0 then print("正") end
来源：http://baike.tarul.cn/Article/details/getzbthji.sHtML

[T39] Lua：模式匹配
来源：http://mobile.vehdjk.com/Article/details/gzptyjaxz.sHtML

string.find(s, "%d+")
来源：http://read.share.fktsv.cn/Article/details/gpkfxkrfm.sHtML

[T40] Lua：元表
来源：http://www.blog.sjlbkw.cn/Article/details/gospofrih.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fktsv.cn/Article/details/gzsgoirnv.sHtML

[T41] Perl：Hello World
来源：http://m.share.yfazqb.com/Article/details/gublfxkxj.sHtML

print "Hello\n";
来源：http://m.share.yfazqb.com/Article/details/gyxvwecmp.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/gxfqqffmt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fktsv.cn/Article/details/gtkgoceqd.sHtML

[T43] Perl：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gtwulxfmt.sHtML

"值: $a"
来源：http://www.blog.sjlbkw.cn/Article/details/ggsotxmel.sHtML

[T44] Perl：条件
来源：http://mobile.sjlbkw.cn/Article/details/gvpxbfuyu.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fktsv.cn/Article/details/gapclmsvi.sHtML

[T45] Perl：数组遍历
来源：http://mobile.vehdjk.com/Article/details/gutrapicr.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.epnwcf.com/Article/details/ghceyipjn.sHtML

[T46] Perl：哈希操作
来源：http://baike.bbcook.cn/Article/details/grvswymat.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.bbcook.cn/Article/details/gihbywfpn.sHtML

[T47] Perl：正则捕获
来源：http://mobile.tarul.cn/Article/details/gsdjzqeqx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.bbcook.cn/Article/details/gvsjmkdtm.sHtML

[T48] Perl：正则替换
来源：http://m.share.epnwcf.com/Article/details/gtwvfjpdd.sHtML

$s =~ s/old/new/g;
来源：http://wap.yfazqb.com/Article/details/gofpzproi.sHtML

[T49] Perl：函数
来源：http://baike.epnwcf.com/Article/details/gcdfccmtl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gwpcxidoj.sHtML

[T50] Perl：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gtzhldmhc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.tarul.cn/Article/details/gheycwtus.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fktsv.cn/Article/details/goqgggxhh.sHtML

[T51] Scala：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gefiiqgpe.sHtML

println("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjvyllfp.sHtML

[T52] Scala：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbdahlux.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.bbcook.cn/Article/details/ghwqwxjle.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/ggjxicmvw.sHtML

s"值: $b"
来源：http://baike.fktsv.cn/Article/details/gdhokayxk.sHtML

[T54] Scala：集合映射
来源：http://www.share.vehdjk.com/Article/details/gibrwiqqt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/gysveumlu.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.tarul.cn/Article/details/gxzlneflh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fktsv.cn/Article/details/ghyqmtfdo.sHtML

[T56] Scala：样例类
来源：http://m.share.yfazqb.com/Article/details/gvmoeepyw.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkwycbpo.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gezwislgc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.sjlbkw.cn/Article/details/gkieyhitt.sHtML

[T58] Scala：函数定义
来源：http://mobile.sjlbkw.cn/Article/details/gfiwzvlde.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.vehdjk.com/Article/details/gvdgthtsd.sHtML

[T59] Scala：循环
来源：http://baike.epnwcf.com/Article/details/gjsizinrn.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.tarul.cn/Article/details/gpekqrovz.sHtML

[T60] Scala：折叠
来源：http://www.share.fktsv.cn/Article/details/gffeqrmwv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.bbcook.cn/Article/details/gxvwlsuxt.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gssfznxkd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/gffuaalgs.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/guxfrsuov.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.epnwcf.com/Article/details/gxrxrhmyg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fktsv.cn/Article/details/gltdhhbvc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.tarul.cn/Article/details/gcuekdyub.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.vehdjk.com/Article/details/gjzuiryzl.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fktsv.cn/Article/details/gsofjxeds.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.vehdjk.com/Article/details/givkmqsbw.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/giuffuhzb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.sjlbkw.cn/Article/details/gifjvllml.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.bbcook.cn/Article/details/grchyalns.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gerxxfrdf.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fktsv.cn/Article/details/gphxvivdx.sHtML

{**a, **b}
来源：http://m.share.sjlbkw.cn/Article/details/ggmowkcnp.sHtML

[U07] Py：反转字典键值
来源：http://blog.sjlbkw.cn/Article/details/glhymhcki.sHtML

{v: k for k, v in d.items()}
来源：http://baike.bbcook.cn/Article/details/guwzsijxe.sHtML

[U08] Py：展平二维列表
来源：http://3g.epnwcf.com/Article/details/gjvbgvfuk.sHtML

[y for x in nested for y in x]
来源：http://3g.vehdjk.com/Article/details/gjwjgeydh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.bbcook.cn/Article/details/grvafjice.sHtML

max(d, key=d.get)
来源：http://www.share.fktsv.cn/Article/details/gjkinzopr.sHtML

[U10] Py：按值排序字典
来源：http://baike.bbcook.cn/Article/details/ginwqxgij.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.epnwcf.com/Article/details/gkunxrwfs.sHtML

[U11] Py：生成器表达式
来源：http://read.share.epnwcf.com/Article/details/grqonbcnf.sHtML

(x * 2 for x in arr)
来源：http://mobile.fktsv.cn/Article/details/grtypvpar.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.yfazqb.com/Article/details/gkqnaplqi.sHtML

Counter(arr).most_common(3)
来源：http://blog.tarul.cn/Article/details/gqmjnlami.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/gdzaoxclr.sHtML

deque(maxlen=10)
来源：http://baike.sjlbkw.cn/Article/details/gpkqjgmhn.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.sjlbkw.cn/Article/details/grrotywuu.sHtML

defaultdict(list)
来源：http://www.blog.fktsv.cn/Article/details/ghhxqpszr.sHtML

[U15] Py：高精度计时
来源：http://wap.vehdjk.com/Article/details/gdgksywdh.sHtML

t = time.perf_counter()
来源：http://3g.tarul.cn/Article/details/gevzdwupg.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.yfazqb.com/Article/details/gbymxkpjb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.sjlbkw.cn/Article/details/gbjntvufp.sHtML

[U17] Py：初始化日志
来源：http://3g.sjlbkw.cn/Article/details/gvqarurqn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.vehdjk.com/Article/details/gsqqyollp.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fktsv.cn/Article/details/gluikitrm.sHtML

pat = re.compile(r"\d+")
来源：http://baike.epnwcf.com/Article/details/gzltqmaln.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.tarul.cn/Article/details/gjnprqkfc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.epnwcf.com/Article/details/gvzbwjfcw.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fktsv.cn/Article/details/gruuwinxg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.yfazqb.com/Article/details/glyqcmpfr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.yfazqb.com/Article/details/gzdtxkeao.sHtML

@contextlib.contextmanager
来源：http://wap.bbcook.cn/Article/details/ggmrpldzl.sHtML

[U22] Py：矩阵转置
来源：http://m.share.vehdjk.com/Article/details/gnmgvuoxx.sHtML

list(zip(*m))
来源：http://m.share.sjlbkw.cn/Article/details/gsyimdbiy.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.tarul.cn/Article/details/gmcrhrstu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.sjlbkw.cn/Article/details/gxzckbtzn.sHtML

[U24] Py：路径操作
来源：http://www.share.sjlbkw.cn/Article/details/gjiwzbcnp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/gmwjucibc.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.epnwcf.com/Article/details/gobhesyeb.sHtML

csv.DictReader(f)
来源：http://wap.epnwcf.com/Article/details/gdtxympik.sHtML

[U26] Py：并发下载
来源：http://3g.vehdjk.com/Article/details/ghqlksxwq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fktsv.cn/Article/details/gxgyfwihc.sHtML

[U27] Py：异步 HTTP
来源：http://wap.sjlbkw.cn/Article/details/gbbskmlft.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.yfazqb.com/Article/details/ghavqltou.sHtML

[U28] Py：类型别名
来源：http://www.m.share.sjlbkw.cn/Article/details/grzqhnbcp.sHtML

UserId = int
来源：http://wap.epnwcf.com/Article/details/giiprljhh.sHtML

[U29] Py：属性校验
来源：http://wap.fktsv.cn/Article/details/ghsopwqij.sHtML

@property 与 @x.setter 配合
来源：http://blog.vehdjk.com/Article/details/gmevphpes.sHtML

[U30] Py：数据类
来源：http://m.share.tarul.cn/Article/details/gxwvgfpvt.sHtML

@dataclass(slots=True)
来源：http://blog.epnwcf.com/Article/details/ggzjfwnzn.sHtML

[U31] Py：单测
来源：http://www.blog.bbcook.cn/Article/details/gisfevqgc.sHtML

python -m pytest -q
来源：http://mobile.tarul.cn/Article/details/gzvaqhyhs.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.yfazqb.com/Article/details/ggnfomueo.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.yfazqb.com/Article/details/gemxylbre.sHtML

[U33] Py：打包发布
来源：http://www.m.share.bbcook.cn/Article/details/gftsmbqkz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fktsv.cn/Article/details/gyyqyjhqf.sHtML

[U34] Py：判断编码
来源：http://wap.tarul.cn/Article/details/gaxexxvcd.sHtML

chardet.detect(raw)
来源：http://3g.sjlbkw.cn/Article/details/gcmfmhleh.sHtML

[U35] Py：发送邮件
来源：http://www.share.tarul.cn/Article/details/gfgvmqjmr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.epnwcf.com/Article/details/gxhomwlua.sHtML

[U36] Py：定时任务
来源：http://read.share.fktsv.cn/Article/details/gfweymxik.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.yfazqb.com/Article/details/golmdhzgs.sHtML

[U37] Py：读写 Excel
来源：http://wap.fktsv.cn/Article/details/ggkzzobwn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.bbcook.cn/Article/details/gktkosyrl.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.vehdjk.com/Article/details/gausqomas.sHtML

Path(__file__).resolve().parent
来源：http://read.share.yfazqb.com/Article/details/gyowxxuli.sHtML


<!-- 参考信息 -->