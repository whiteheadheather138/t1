代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://m.share.sjlbkw.cn/Article/details/glxiospgj.sHtML

[S15] C：类型转换
来源：http://blog.sjlbkw.cn/Article/details/gfecnuyel.sHtML

(double) a / b
来源：http://mobile.yfazqb.com/Article/details/gazyjbfvi.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/gwacezcsm.sHtML

x |= (1 << 3);
来源：http://m.share.vehdjk.com/Article/details/gvruarrrz.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gthngjmwe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gmxtqbwyd.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/guxagklyh.sHtML

int main(int argc, char **argv)
来源：http://wap.yfazqb.com/Article/details/gsgvlagcv.sHtML

[S19] C：快速排序
来源：http://wap.sjlbkw.cn/Article/details/gqfdaghuo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/grcdtthcy.sHtML

[S20] C：二分查找
来源：http://baike.fktsv.cn/Article/details/giazemjcx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/gljktoonb.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/gwuwvavcx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.epnwcf.com/Article/details/gdfylaeij.sHtML

[S22] C：字符串转数字
来源：http://3g.yfazqb.com/Article/details/gitsysfok.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.sjlbkw.cn/Article/details/gknghyinz.sHtML

[S23] C：随机数
来源：http://mobile.yfazqb.com/Article/details/ggexkadbe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/gsweqhbzu.sHtML

[S24] C：获取本地时间
来源：http://read.share.tarul.cn/Article/details/gqojnidyw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.yfazqb.com/Article/details/gmzomvmno.sHtML

[S25] C：内存拷贝
来源：http://blog.bbcook.cn/Article/details/gdsktushq.sHtML

memcpy(dst, src, n);
来源：http://read.share.fktsv.cn/Article/details/guruehnup.sHtML

[S26] C：内存清零
来源：http://www.blog.bbcook.cn/Article/details/gciejmhdx.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.bbcook.cn/Article/details/gxilydljg.sHtML

[S27] C：定义常量
来源：http://baike.epnwcf.com/Article/details/gqaiziesq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvrbiztx.sHtML

[S28] C：静态变量
来源：http://www.share.vehdjk.com/Article/details/gitpbdwwg.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/gdgkjpncz.sHtML

[S29] C：变参函数
来源：http://wap.yfazqb.com/Article/details/gvvedudll.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fktsv.cn/Article/details/guvlpdukg.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/gucrpdygp.sHtML

#ifndef X_H
来源：http://www.blog.epnwcf.com/Article/details/gcaaqcjld.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gqqawcyoa.sHtML

#endif
来源：http://m.share.fktsv.cn/Article/details/ggljthtvq.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/gmmyghijd.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gqshgnknp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fktsv.cn/Article/details/gmafemsct.sHtML

[S32] C++：字符串
来源：http://read.share.fktsv.cn/Article/details/gintulbwg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fktsv.cn/Article/details/glmjuzord.sHtML

[S33] C++：vector 增删
来源：http://www.share.bbcook.cn/Article/details/ggglshyyl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gkjjqaxas.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/grqymfsby.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.sjlbkw.cn/Article/details/gpuhfymwv.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/gsuhtcdsn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gtfhpdihl.sHtML

[S36] C++：unordered_map
来源：http://mobile.epnwcf.com/Article/details/gslwxpcaq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gwnumeedv.sHtML

[S37] C++：set
来源：http://m.share.bbcook.cn/Article/details/gwdevaqmc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.sjlbkw.cn/Article/details/gdkvyilnc.sHtML

[S38] C++：排序
来源：http://read.share.vehdjk.com/Article/details/gxzryigug.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.epnwcf.com/Article/details/goqhvluto.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fktsv.cn/Article/details/geqzldizr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.sjlbkw.cn/Article/details/gylfqjqpo.sHtML

[S40] C++：查找元素
来源：http://mobile.yfazqb.com/Article/details/gjksrzyyp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.yfazqb.com/Article/details/gmzzhadjd.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/gnuqrgupd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fktsv.cn/Article/details/gmmeoehmv.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fktsv.cn/Article/details/gzwxcbojx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/gstwydywo.sHtML

[S43] C++：智能指针
来源：http://www.m.share.epnwcf.com/Article/details/goenwdrfs.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.tarul.cn/Article/details/gunqiuoly.sHtML

[S44] C++：引用传参
来源：http://www.share.vehdjk.com/Article/details/gdvestmru.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.epnwcf.com/Article/details/gstjvvrvl.sHtML

[S45] C++：lambda
来源：http://read.share.tarul.cn/Article/details/gwxcpcjdf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/gqlveinlw.sHtML

[S46] C++：函数模板
来源：http://www.blog.bbcook.cn/Article/details/gpaygssrn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.bbcook.cn/Article/details/gshksfxlx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuvsobjs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.epnwcf.com/Article/details/gvkzlsxhm.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/getsetlvh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.tarul.cn/Article/details/gkijlegtq.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.tarul.cn/Article/details/gmqwsposx.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/gtdcbfqye.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.sjlbkw.cn/Article/details/gksogaszg.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.bbcook.cn/Article/details/gpqzucend.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gnxbstqgb.sHtML

[S51] C++：显式类型转换
来源：http://read.share.tarul.cn/Article/details/gwnqhzcqs.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnglbpjz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/gcwwgobkr.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fktsv.cn/Article/details/gwainzzrg.sHtML

[S53] C++：移动语义
来源：http://3g.yfazqb.com/Article/details/gtgbhugln.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fktsv.cn/Article/details/gsvipksut.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/gekpymyow.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.yfazqb.com/Article/details/gwydrdmtx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.yfazqb.com/Article/details/gsduxlelu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fktsv.cn/Article/details/gsxedpaiz.sHtML

[S56] C++：optional
来源：http://wap.vehdjk.com/Article/details/glnywcljg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.vehdjk.com/Article/details/gjbolpzle.sHtML

[S57] C++：编译期常量
来源：http://m.share.sjlbkw.cn/Article/details/grxyshchl.sHtML

constexpr int N = 10;
来源：http://www.blog.tarul.cn/Article/details/gvdctedri.sHtML

[S58] C++：命名空间
来源：http://3g.sjlbkw.cn/Article/details/grwatttsy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.epnwcf.com/Article/details/gbcuzhscc.sHtML

[S59] C++：静态断言
来源：http://blog.sjlbkw.cn/Article/details/glxyutbbg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fktsv.cn/Article/details/gndugdhjb.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.epnwcf.com/Article/details/gfblbxarp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.epnwcf.com/Article/details/gingihprj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gakhybsqw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fktsv.cn/Article/details/gtwgdcayn.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grqprhlss.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.vehdjk.com/Article/details/gneyvtylj.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gtbdxfizs.sHtML

[T02] Kotlin：变量
来源：http://read.share.tarul.cn/Article/details/gcufepnvn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.tarul.cn/Article/details/gklhxbidy.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.tarul.cn/Article/details/gqagjbidy.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gstxvtoih.sHtML

[T04] Kotlin：空安全
来源：http://read.share.bbcook.cn/Article/details/gbnsrkqes.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gaqqytgam.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.sjlbkw.cn/Article/details/ghtguqixf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/ghpyndjio.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.vehdjk.com/Article/details/ggfamxqhg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fktsv.cn/Article/details/gplwgdcfl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/gjilznkat.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.tarul.cn/Article/details/gxgaamtdb.sHtML

[T08] Kotlin：数据类
来源：http://m.share.tarul.cn/Article/details/gawnmfhss.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.yfazqb.com/Article/details/gpygloktm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.epnwcf.com/Article/details/ggoltawaa.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.tarul.cn/Article/details/gtjcnhqoe.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.bbcook.cn/Article/details/gflfymzbc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.sjlbkw.cn/Article/details/ghpopijyj.sHtML

[T11] Kotlin：协程
来源：http://read.share.sjlbkw.cn/Article/details/gagixktrj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.epnwcf.com/Article/details/gabpbeliz.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.vehdjk.com/Article/details/gbzlkfklb.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.yfazqb.com/Article/details/gfhvxzaql.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.vehdjk.com/Article/details/gbmwrieob.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fktsv.cn/Article/details/gnguucsym.sHtML

[T14] Kotlin：循环
来源：http://baike.bbcook.cn/Article/details/gycrqjlkl.sHtML

for (i in 1..10) println(i)
来源：http://m.share.vehdjk.com/Article/details/gmjljgwdl.sHtML

[T15] Kotlin：接口
来源：http://m.share.vehdjk.com/Article/details/gaotarili.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.tarul.cn/Article/details/geittaoei.sHtML

[T16] Swift：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gmligxuxl.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gkxrxyigx.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fktsv.cn/Article/details/gzeicxqys.sHtML

var a = 1;  let b = 2
来源：http://www.blog.yfazqb.com/Article/details/gdahvghhr.sHtML

[T18] Swift：字符串插值
来源：http://wap.vehdjk.com/Article/details/glxfqbxlp.sHtML

"值: \(b)"
来源：http://blog.bbcook.cn/Article/details/gqlgbbxlb.sHtML

[T19] Swift：可选绑定
来源：http://mobile.vehdjk.com/Article/details/gyccbbhap.sHtML

if let n = opt { print(n) }
来源：http://wap.fktsv.cn/Article/details/gvkqfmxfm.sHtML

[T20] Swift：数组操作
来源：http://m.share.vehdjk.com/Article/details/genvinhwf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.sjlbkw.cn/Article/details/gmqfhhafa.sHtML

[T21] Swift：遍历
来源：http://wap.sjlbkw.cn/Article/details/gjvelufsu.sHtML

for x in a { print(x) }
来源：http://www.share.vehdjk.com/Article/details/gjddlpiyu.sHtML

[T22] Swift：字典
来源：http://blog.sjlbkw.cn/Article/details/gdymypiuv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.bbcook.cn/Article/details/gdoktfroj.sHtML

[T23] Swift：函数
来源：http://www.share.yfazqb.com/Article/details/ggmwwakqd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.tarul.cn/Article/details/gozhvbzbj.sHtML

[T24] Swift：闭包
来源：http://www.blog.sjlbkw.cn/Article/details/gpodyfoib.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gbrjxvhyb.sHtML

[T25] Swift：结构体
来源：http://www.share.bbcook.cn/Article/details/gvhgyfeuh.sHtML

struct P { var x: Int }
来源：http://3g.sjlbkw.cn/Article/details/gwwtntdlo.sHtML

[T26] Swift：类与重写
来源：http://www.blog.epnwcf.com/Article/details/gljahdxqe.sHtML

class A: Base { override func f() {} }
来源：http://blog.fktsv.cn/Article/details/gghaswqgg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.vehdjk.com/Article/details/glqjsrhug.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.sjlbkw.cn/Article/details/gxspygihc.sHtML

[T28] Swift：枚举
来源：http://baike.bbcook.cn/Article/details/gyqmsgubi.sHtML

enum Color { case red, green }
来源：http://3g.fktsv.cn/Article/details/gsynuzfdc.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.yfazqb.com/Article/details/gruhkfgkb.sHtML

guard let x = opt else { return }
来源：http://www.share.vehdjk.com/Article/details/grmfmwlpf.sHtML

[T30] Swift：协议
来源：http://www.share.epnwcf.com/Article/details/gfbalriyc.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.tarul.cn/Article/details/gedddlxnv.sHtML

[T31] Lua：Hello World
来源：http://m.share.epnwcf.com/Article/details/gppqyywlp.sHtML

print("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gxjlatuqe.sHtML

[T32] Lua：局部变量
来源：http://m.share.epnwcf.com/Article/details/gsbvqicqy.sHtML

local a = 1
来源：http://baike.bbcook.cn/Article/details/gahikxqwf.sHtML

[T33] Lua：表（数组）
来源：http://mobile.sjlbkw.cn/Article/details/gbhtygfsm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.bbcook.cn/Article/details/ggzwqywwj.sHtML

[T34] Lua：遍历表
来源：http://m.share.bbcook.cn/Article/details/gopjaawzu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.yfazqb.com/Article/details/gordkfchx.sHtML

[T35] Lua：字典表
来源：http://mobile.fktsv.cn/Article/details/gngjhqeyc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.epnwcf.com/Article/details/gabeoowjh.sHtML

[T36] Lua：函数
来源：http://mobile.sjlbkw.cn/Article/details/girvmmzbf.sHtML

function add(a, b) return a + b end
来源：http://mobile.yfazqb.com/Article/details/gvgyyoajp.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.tarul.cn/Article/details/gzxdrbgwp.sHtML

"a" .. "b"
来源：http://m.share.fktsv.cn/Article/details/grkhcegxi.sHtML

[T38] Lua：条件
来源：http://baike.epnwcf.com/Article/details/gxonoktdb.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/gsimbvhqs.sHtML

[T39] Lua：模式匹配
来源：http://wap.tarul.cn/Article/details/geznpywhz.sHtML

string.find(s, "%d+")
来源：http://read.share.epnwcf.com/Article/details/gvcnbuklz.sHtML

[T40] Lua：元表
来源：http://mobile.yfazqb.com/Article/details/ggsxhebkp.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.vehdjk.com/Article/details/gxlumqztc.sHtML

[T41] Perl：Hello World
来源：http://read.share.fktsv.cn/Article/details/gamqymssn.sHtML

print "Hello\n";
来源：http://www.blog.vehdjk.com/Article/details/gyytwbnqn.sHtML

[T42] Perl：变量类型
来源：http://read.share.bbcook.cn/Article/details/gvxltaxkl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.epnwcf.com/Article/details/ghfmznolo.sHtML

[T43] Perl：字符串插值
来源：http://3g.vehdjk.com/Article/details/gxhrjnfsk.sHtML

"值: $a"
来源：http://www.blog.bbcook.cn/Article/details/gmekibqfj.sHtML

[T44] Perl：条件
来源：http://m.share.fktsv.cn/Article/details/gnhvhyktf.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fktsv.cn/Article/details/gmxnaejvw.sHtML

[T45] Perl：数组遍历
来源：http://3g.fktsv.cn/Article/details/glhrtivyp.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.bbcook.cn/Article/details/gfhldofsg.sHtML

[T46] Perl：哈希操作
来源：http://3g.vehdjk.com/Article/details/gxgyhlctu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.bbcook.cn/Article/details/gfpkbbxwx.sHtML

[T47] Perl：正则捕获
来源：http://www.share.tarul.cn/Article/details/gyifpzufz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.tarul.cn/Article/details/gpnqtoxpa.sHtML

[T48] Perl：正则替换
来源：http://www.share.bbcook.cn/Article/details/ghyetlqpq.sHtML

$s =~ s/old/new/g;
来源：http://baike.yfazqb.com/Article/details/gkjbqpfiz.sHtML

[T49] Perl：函数
来源：http://3g.yfazqb.com/Article/details/grpjvfhfy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gglejbxwv.sHtML

[T50] Perl：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gpxdhiglp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.sjlbkw.cn/Article/details/gmcypkqvp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.sjlbkw.cn/Article/details/gtgpegzsz.sHtML

[T51] Scala：Hello World
来源：http://blog.yfazqb.com/Article/details/gompmcmpe.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gyosaicnd.sHtML

[T52] Scala：变量
来源：http://www.m.share.yfazqb.com/Article/details/gdydukqij.sHtML

val a = 1;  var b = 2
来源：http://www.blog.yfazqb.com/Article/details/gfyxuusre.sHtML

[T53] Scala：字符串插值
来源：http://baike.fktsv.cn/Article/details/gjmfascur.sHtML

s"值: $b"
来源：http://mobile.yfazqb.com/Article/details/gmauoierh.sHtML

[T54] Scala：集合映射
来源：http://mobile.tarul.cn/Article/details/ggxtnlfhd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gmjcuvqee.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.yfazqb.com/Article/details/ggcikbrqq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.yfazqb.com/Article/details/gzufhrkmb.sHtML

[T56] Scala：样例类
来源：http://mobile.sjlbkw.cn/Article/details/glmmlosyy.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/grtrapvjf.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkhgqtyu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fktsv.cn/Article/details/gdfieghwf.sHtML

[T58] Scala：函数定义
来源：http://m.share.vehdjk.com/Article/details/glncsdxpd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fktsv.cn/Article/details/gwnvsakhp.sHtML

[T59] Scala：循环
来源：http://www.m.share.vehdjk.com/Article/details/ghiovmxsq.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.epnwcf.com/Article/details/gilhwypmw.sHtML

[T60] Scala：折叠
来源：http://blog.bbcook.cn/Article/details/ggogyzncg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.bbcook.cn/Article/details/gdwkalbms.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gftetygdn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/glihkrjyz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gxgyqbprp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.yfazqb.com/Article/details/gglvxzozk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.yfazqb.com/Article/details/gktzfcoxx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.vehdjk.com/Article/details/gqhniiqgn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.yfazqb.com/Article/details/gjjtgaltw.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.epnwcf.com/Article/details/gcvnbwqfi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.vehdjk.com/Article/details/gxhlkfukw.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.epnwcf.com/Article/details/galmwpuwf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.vehdjk.com/Article/details/gfwtwdslf.sHtML

[U05] Py：列表去重且保序
来源：http://wap.yfazqb.com/Article/details/godnaozli.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/ggqwagzpt.sHtML

[U06] Py：合并两个字典
来源：http://baike.bbcook.cn/Article/details/gxxsgdkre.sHtML

{**a, **b}
来源：http://baike.tarul.cn/Article/details/gfoybwcby.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.bbcook.cn/Article/details/gkkjprdtv.sHtML

{v: k for k, v in d.items()}
来源：http://wap.yfazqb.com/Article/details/ggihwigfo.sHtML

[U08] Py：展平二维列表
来源：http://mobile.bbcook.cn/Article/details/gltrqhosc.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fktsv.cn/Article/details/ghhggpjsh.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.bbcook.cn/Article/details/gjpuedrix.sHtML

max(d, key=d.get)
来源：http://www.share.tarul.cn/Article/details/gcdulrwxe.sHtML

[U10] Py：按值排序字典
来源：http://www.share.epnwcf.com/Article/details/gkdmivrfz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fktsv.cn/Article/details/gbtpbklvm.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.epnwcf.com/Article/details/ggaxrmcgs.sHtML

(x * 2 for x in arr)
来源：http://baike.tarul.cn/Article/details/glbfjybck.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.yfazqb.com/Article/details/gkjhyhnth.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fktsv.cn/Article/details/ghhsidses.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.tarul.cn/Article/details/gbulnxxkk.sHtML

deque(maxlen=10)
来源：http://read.share.sjlbkw.cn/Article/details/gwdefhacl.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.epnwcf.com/Article/details/gqvvlujso.sHtML

defaultdict(list)
来源：http://www.share.epnwcf.com/Article/details/gkdgsphkc.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.yfazqb.com/Article/details/gbkavvyen.sHtML

t = time.perf_counter()
来源：http://www.blog.epnwcf.com/Article/details/gpvwiwvdd.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fktsv.cn/Article/details/gvxwaymbb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.tarul.cn/Article/details/gqiyipino.sHtML

[U17] Py：初始化日志
来源：http://3g.vehdjk.com/Article/details/gsgprhcts.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.yfazqb.com/Article/details/gjxbsxrkx.sHtML

[U18] Py：预编译正则
来源：http://wap.sjlbkw.cn/Article/details/gpezrbnxj.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.yfazqb.com/Article/details/grnognbjk.sHtML

[U19] Py：正则替换带回调
来源：http://3g.bbcook.cn/Article/details/gsprpkuaj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.epnwcf.com/Article/details/gjmlsfhrz.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.yfazqb.com/Article/details/ghxthrkgq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.epnwcf.com/Article/details/gfbltaltl.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.bbcook.cn/Article/details/gajjrixcs.sHtML

@contextlib.contextmanager
来源：http://m.share.epnwcf.com/Article/details/gjtptieiq.sHtML

[U22] Py：矩阵转置
来源：http://blog.sjlbkw.cn/Article/details/gnmyjdlzj.sHtML

list(zip(*m))
来源：http://m.share.tarul.cn/Article/details/gkiqzvxea.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.bbcook.cn/Article/details/gbpvqnuqh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.bbcook.cn/Article/details/gthgbdoyc.sHtML

[U24] Py：路径操作
来源：http://mobile.epnwcf.com/Article/details/gfxqxxknu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/gudtxlrnp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.tarul.cn/Article/details/gplxfqjuq.sHtML

csv.DictReader(f)
来源：http://www.blog.bbcook.cn/Article/details/gdgxzpcjt.sHtML

[U26] Py：并发下载
来源：http://www.blog.tarul.cn/Article/details/gpqkqwwke.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.sjlbkw.cn/Article/details/gmpaljvem.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.yfazqb.com/Article/details/gtlbonltr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.sjlbkw.cn/Article/details/gawbwqqbb.sHtML

[U28] Py：类型别名
来源：http://read.share.epnwcf.com/Article/details/gwdqozsjv.sHtML

UserId = int
来源：http://m.share.epnwcf.com/Article/details/gfxhksvjt.sHtML

[U29] Py：属性校验
来源：http://mobile.sjlbkw.cn/Article/details/ggpfjocib.sHtML

@property 与 @x.setter 配合
来源：http://baike.fktsv.cn/Article/details/gncckgyij.sHtML

[U30] Py：数据类
来源：http://blog.epnwcf.com/Article/details/gitasdddn.sHtML

@dataclass(slots=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gzpcsvdwx.sHtML

[U31] Py：单测
来源：http://wap.yfazqb.com/Article/details/gbmmlhbse.sHtML

python -m pytest -q
来源：http://www.m.share.sjlbkw.cn/Article/details/gkaixonyp.sHtML

[U32] Py：代码格式化
来源：http://mobile.sjlbkw.cn/Article/details/gwuvarxtn.sHtML

ruff format . && ruff check --fix .
来源：http://wap.sjlbkw.cn/Article/details/gkeaybejo.sHtML

[U33] Py：打包发布
来源：http://www.m.share.epnwcf.com/Article/details/ghsayljog.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.epnwcf.com/Article/details/ghxldyqng.sHtML

[U34] Py：判断编码
来源：http://www.m.share.epnwcf.com/Article/details/gnizbvhyn.sHtML

chardet.detect(raw)
来源：http://m.share.tarul.cn/Article/details/gtcgxbuhi.sHtML

[U35] Py：发送邮件
来源：http://wap.sjlbkw.cn/Article/details/glamrfufn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.tarul.cn/Article/details/gctolbyuj.sHtML

[U36] Py：定时任务
来源：http://baike.vehdjk.com/Article/details/gqqjddgxl.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.tarul.cn/Article/details/ghgrlstxn.sHtML

[U37] Py：读写 Excel
来源：http://m.share.epnwcf.com/Article/details/gfiqhjcxy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.sjlbkw.cn/Article/details/gaqckfjmf.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.tarul.cn/Article/details/gyiztunpt.sHtML

Path(__file__).resolve().parent
来源：http://www.share.bbcook.cn/Article/details/gvsivgmux.sHtML


<!-- 参考信息 -->