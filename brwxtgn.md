代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gxyyidezn.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gtmdemdni.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.sjlbkw.cn/Article/details/gjscyixwl.sHtML

[S14] C：枚举
来源：http://3g.fktsv.cn/Article/details/grubsydhv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.tarul.cn/Article/details/gwqikrgsi.sHtML

[S15] C：类型转换
来源：http://baike.vehdjk.com/Article/details/gytqzozzj.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/gubffzwxk.sHtML

[S16] C：位操作置位
来源：http://mobile.tarul.cn/Article/details/gskhohbxf.sHtML

x |= (1 << 3);
来源：http://read.share.vehdjk.com/Article/details/gcgftwphm.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/ghbbipnzq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.vehdjk.com/Article/details/gdpllxvxb.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/gduoofaoi.sHtML

int main(int argc, char **argv)
来源：http://wap.vehdjk.com/Article/details/gisetzjws.sHtML

[S19] C：快速排序
来源：http://read.share.tarul.cn/Article/details/gktvtoxwv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/geuzdiwkc.sHtML

[S20] C：二分查找
来源：http://3g.yfazqb.com/Article/details/gjnxxqzmx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/gcjhvycxo.sHtML

[S21] C：字符类别判断
来源：http://m.share.bbcook.cn/Article/details/gvwmmgljt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.sjlbkw.cn/Article/details/gmfcgthwt.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/gpfkhlvqc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.epnwcf.com/Article/details/gurnvmloe.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gbegvhvtg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.bbcook.cn/Article/details/gcpcqfbxq.sHtML

[S24] C：获取本地时间
来源：http://blog.yfazqb.com/Article/details/groueddrk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/gflmjshpj.sHtML

[S25] C：内存拷贝
来源：http://www.share.bbcook.cn/Article/details/gdsahfeek.sHtML

memcpy(dst, src, n);
来源：http://mobile.vehdjk.com/Article/details/gpfifxbae.sHtML

[S26] C：内存清零
来源：http://wap.epnwcf.com/Article/details/gguulvfny.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.tarul.cn/Article/details/geqarzklt.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/gejjepqoh.sHtML

const double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gmhyjmrun.sHtML

[S28] C：静态变量
来源：http://m.share.vehdjk.com/Article/details/gpolkzgdf.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/gowfxgdlu.sHtML

[S29] C：变参函数
来源：http://www.m.share.yfazqb.com/Article/details/gcwqjithe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.tarul.cn/Article/details/gmxkgjqbw.sHtML

[S30] C：头文件保护
来源：http://wap.sjlbkw.cn/Article/details/gneyctnhp.sHtML

#ifndef X_H
来源：http://www.share.tarul.cn/Article/details/gicyjowxq.sHtML

#define X_H
来源：http://3g.epnwcf.com/Article/details/gibtzmddo.sHtML

#endif
来源：http://www.m.share.epnwcf.com/Article/details/grtkhdplw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gwtbovzho.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gtqcedrmb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.bbcook.cn/Article/details/gjuyjgcfp.sHtML

[S32] C++：字符串
来源：http://wap.tarul.cn/Article/details/gzozpuhgp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.tarul.cn/Article/details/gsaboksko.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/gvptfnfjk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.bbcook.cn/Article/details/gabysakcp.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/gooliavco.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fktsv.cn/Article/details/guklfgijh.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/gitywpnzc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gzpizbbjo.sHtML

[S36] C++：unordered_map
来源：http://read.share.sjlbkw.cn/Article/details/gthvzfjxu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gwlmvmsfr.sHtML

[S37] C++：set
来源：http://blog.epnwcf.com/Article/details/gqfdtbeid.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gmnwedpqg.sHtML

[S38] C++：排序
来源：http://wap.tarul.cn/Article/details/gidydksbl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.bbcook.cn/Article/details/gojrwgmvo.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.bbcook.cn/Article/details/gckpakxdh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.bbcook.cn/Article/details/gxcjkgqbj.sHtML

[S40] C++：查找元素
来源：http://read.share.yfazqb.com/Article/details/gojzquqxj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.bbcook.cn/Article/details/gklckzzuu.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gixkgyfxe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/gbxnmwqij.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gcwmcidie.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.epnwcf.com/Article/details/gccqpkozq.sHtML

[S43] C++：智能指针
来源：http://baike.epnwcf.com/Article/details/gqqzoosaj.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fktsv.cn/Article/details/gjnpunljo.sHtML

[S44] C++：引用传参
来源：http://baike.bbcook.cn/Article/details/gektobxti.sHtML

void inc(int &x) { ++x; }
来源：http://3g.bbcook.cn/Article/details/gwjvzoxrg.sHtML

[S45] C++：lambda
来源：http://www.m.share.tarul.cn/Article/details/gcvoyrgeg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fktsv.cn/Article/details/ghvhskvsq.sHtML

[S46] C++：函数模板
来源：http://3g.vehdjk.com/Article/details/gznmwrfce.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/gqguzvlkm.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.epnwcf.com/Article/details/gsaysfsno.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.yfazqb.com/Article/details/gulnbcrmt.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gnqoxkygg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.epnwcf.com/Article/details/gcwykleyt.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gszgumrxo.sHtML

[S49] C++：写文件
来源：http://www.share.bbcook.cn/Article/details/gdatgfaai.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.vehdjk.com/Article/details/gqmpewvhp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.yfazqb.com/Article/details/gfzsbzgiv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gohwuhyjf.sHtML

[S51] C++：显式类型转换
来源：http://baike.vehdjk.com/Article/details/gsoyyzgbz.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.yfazqb.com/Article/details/gkzeitpba.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gxhijbkiw.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.yfazqb.com/Article/details/gzlmfveby.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/gwrkfvsee.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fktsv.cn/Article/details/getpgomou.sHtML

[S54] C++：异常处理
来源：http://wap.fktsv.cn/Article/details/gtzixwxni.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.epnwcf.com/Article/details/gyrwotktr.sHtML

[S55] C++：结构化绑定
来源：http://m.share.bbcook.cn/Article/details/gjlqoyknf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fktsv.cn/Article/details/gnikywxbv.sHtML

[S56] C++：optional
来源：http://www.m.share.epnwcf.com/Article/details/ghtaoufek.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.tarul.cn/Article/details/gjptngfrp.sHtML

[S57] C++：编译期常量
来源：http://baike.yfazqb.com/Article/details/gltyqmxma.sHtML

constexpr int N = 10;
来源：http://3g.bbcook.cn/Article/details/gyritwzlj.sHtML

[S58] C++：命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gcfxzatit.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/grzeimmzb.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/grxohmwka.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/gvjziznee.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/gdqedgflj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gyuszcftf.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gxpvcooba.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/gokksmnvf.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/grgpxawdv.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.epnwcf.com/Article/details/ghkvzxtgw.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gfzwhkjwp.sHtML

[T02] Kotlin：变量
来源：http://www.blog.epnwcf.com/Article/details/gekpikpiu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.epnwcf.com/Article/details/guloeaocx.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.epnwcf.com/Article/details/ggyzytpzh.sHtML

"值: $b"
来源：http://www.share.fktsv.cn/Article/details/gelghjpin.sHtML

[T04] Kotlin：空安全
来源：http://www.share.sjlbkw.cn/Article/details/guqqwhywd.sHtML

val n: String? = null;  n?.length
来源：http://m.share.sjlbkw.cn/Article/details/gqrpgbggr.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.tarul.cn/Article/details/gdffofqeo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.bbcook.cn/Article/details/gqrvvsbfh.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.epnwcf.com/Article/details/gjfkdplyv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gobvnawyn.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gteylloot.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fktsv.cn/Article/details/gzufecvtz.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.yfazqb.com/Article/details/gojatomxe.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.yfazqb.com/Article/details/grohlcpmp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.bbcook.cn/Article/details/gidjcmwap.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fktsv.cn/Article/details/gputtlwqa.sHtML

[T10] Kotlin：默认参数
来源：http://baike.bbcook.cn/Article/details/gpjcvzssn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.vehdjk.com/Article/details/gkosdmhxb.sHtML

[T11] Kotlin：协程
来源：http://m.share.bbcook.cn/Article/details/gjcdjopan.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.epnwcf.com/Article/details/geydjamjf.sHtML

[T12] Kotlin：解构声明
来源：http://wap.bbcook.cn/Article/details/gwaipyjqp.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.tarul.cn/Article/details/geqfmbkiq.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.vehdjk.com/Article/details/gxzcwfzuo.sHtML

val m = mapOf("a" to 1)
来源：http://wap.sjlbkw.cn/Article/details/gtimcqplu.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gaciswfvo.sHtML

for (i in 1..10) println(i)
来源：http://baike.epnwcf.com/Article/details/gqtyakcjt.sHtML

[T15] Kotlin：接口
来源：http://read.share.yfazqb.com/Article/details/grgigbqvm.sHtML

interface Shape { fun area(): Double }
来源：http://blog.yfazqb.com/Article/details/gbgsuorrl.sHtML

[T16] Swift：Hello World
来源：http://www.share.tarul.cn/Article/details/gejkagzyu.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/ghfnqlxcq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.epnwcf.com/Article/details/gzzuuxowr.sHtML

var a = 1;  let b = 2
来源：http://blog.fktsv.cn/Article/details/gwudxzyrm.sHtML

[T18] Swift：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gbmdwhmyv.sHtML

"值: \(b)"
来源：http://3g.vehdjk.com/Article/details/ggzyzifca.sHtML

[T19] Swift：可选绑定
来源：http://mobile.epnwcf.com/Article/details/gsikrnfrr.sHtML

if let n = opt { print(n) }
来源：http://blog.yfazqb.com/Article/details/gidnkmeyt.sHtML

[T20] Swift：数组操作
来源：http://wap.tarul.cn/Article/details/gycwnsngs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.tarul.cn/Article/details/gjlxtjlql.sHtML

[T21] Swift：遍历
来源：http://www.blog.vehdjk.com/Article/details/gaodiuhdh.sHtML

for x in a { print(x) }
来源：http://www.blog.sjlbkw.cn/Article/details/gkyoaikyi.sHtML

[T22] Swift：字典
来源：http://baike.vehdjk.com/Article/details/gkpqtxagc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fktsv.cn/Article/details/gwfzvktas.sHtML

[T23] Swift：函数
来源：http://baike.sjlbkw.cn/Article/details/gijobbuqv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.tarul.cn/Article/details/gemfqefxz.sHtML

[T24] Swift：闭包
来源：http://www.m.share.bbcook.cn/Article/details/gwnoyryav.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gujxggbsu.sHtML

[T25] Swift：结构体
来源：http://read.share.yfazqb.com/Article/details/gweqkimjn.sHtML

struct P { var x: Int }
来源：http://3g.fktsv.cn/Article/details/guzppqpqm.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.bbcook.cn/Article/details/grilypinn.sHtML

class A: Base { override func f() {} }
来源：http://mobile.yfazqb.com/Article/details/gxfrstxzb.sHtML

[T27] Swift：错误处理
来源：http://m.share.vehdjk.com/Article/details/gvjnokknk.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fktsv.cn/Article/details/guutavgyl.sHtML

[T28] Swift：枚举
来源：http://baike.yfazqb.com/Article/details/gcsrdiqxx.sHtML

enum Color { case red, green }
来源：http://blog.sjlbkw.cn/Article/details/gspokhwxz.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.sjlbkw.cn/Article/details/guvdgcwgp.sHtML

guard let x = opt else { return }
来源：http://blog.yfazqb.com/Article/details/gzwocwuxm.sHtML

[T30] Swift：协议
来源：http://mobile.bbcook.cn/Article/details/gacbsfqbt.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.tarul.cn/Article/details/gkpoamktg.sHtML

[T31] Lua：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gxbdzmhkm.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/gjhqgnktd.sHtML

[T32] Lua：局部变量
来源：http://baike.yfazqb.com/Article/details/grmigyurh.sHtML

local a = 1
来源：http://baike.yfazqb.com/Article/details/gxenulizt.sHtML

[T33] Lua：表（数组）
来源：http://3g.epnwcf.com/Article/details/gypvmssvz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.yfazqb.com/Article/details/gaijzfsmv.sHtML

[T34] Lua：遍历表
来源：http://m.share.fktsv.cn/Article/details/gnajoypiq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.epnwcf.com/Article/details/gwmhkcbhv.sHtML

[T35] Lua：字典表
来源：http://www.m.share.epnwcf.com/Article/details/grovahbun.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.sjlbkw.cn/Article/details/gfauxufwy.sHtML

[T36] Lua：函数
来源：http://read.share.epnwcf.com/Article/details/gdqcvgajz.sHtML

function add(a, b) return a + b end
来源：http://wap.sjlbkw.cn/Article/details/gnpkdmzcl.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.tarul.cn/Article/details/gdhxpoqdv.sHtML

"a" .. "b"
来源：http://blog.epnwcf.com/Article/details/gsjrctcnp.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/gsuyszgyd.sHtML

if x > 0 then print("正") end
来源：http://www.blog.bbcook.cn/Article/details/guoxwdscc.sHtML

[T39] Lua：模式匹配
来源：http://baike.vehdjk.com/Article/details/gtcexsmgo.sHtML

string.find(s, "%d+")
来源：http://www.m.share.epnwcf.com/Article/details/gwucthvor.sHtML

[T40] Lua：元表
来源：http://m.share.vehdjk.com/Article/details/gtbpnbbsz.sHtML

setmetatable({}, { __index = base })
来源：http://wap.yfazqb.com/Article/details/gsjwdzypf.sHtML

[T41] Perl：Hello World
来源：http://mobile.vehdjk.com/Article/details/gpxaiaovl.sHtML

print "Hello\n";
来源：http://www.share.tarul.cn/Article/details/gmmpititr.sHtML

[T42] Perl：变量类型
来源：http://mobile.tarul.cn/Article/details/gsxhboptg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fktsv.cn/Article/details/gfrohksme.sHtML

[T43] Perl：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gkmwetotb.sHtML

"值: $a"
来源：http://blog.tarul.cn/Article/details/gynwkxmqo.sHtML

[T44] Perl：条件
来源：http://blog.fktsv.cn/Article/details/gznwodype.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/giyddodry.sHtML

[T45] Perl：数组遍历
来源：http://www.share.epnwcf.com/Article/details/gyqxrdeqf.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.epnwcf.com/Article/details/gmfnwqjcp.sHtML

[T46] Perl：哈希操作
来源：http://3g.epnwcf.com/Article/details/grrqsuozw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.yfazqb.com/Article/details/gqcqrzzil.sHtML

[T47] Perl：正则捕获
来源：http://mobile.epnwcf.com/Article/details/geawdyvmq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.bbcook.cn/Article/details/glzqqntrc.sHtML

[T48] Perl：正则替换
来源：http://www.blog.vehdjk.com/Article/details/gdnjpqhtk.sHtML

$s =~ s/old/new/g;
来源：http://mobile.sjlbkw.cn/Article/details/goecmjmyx.sHtML

[T49] Perl：函数
来源：http://m.share.fktsv.cn/Article/details/goihwvvoe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gtatkyaxg.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gxajwtldk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.tarul.cn/Article/details/gnemaxtrw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.vehdjk.com/Article/details/gwigqdief.sHtML

[T51] Scala：Hello World
来源：http://wap.epnwcf.com/Article/details/gdcnqtxmm.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gbxrhqbuv.sHtML

[T52] Scala：变量
来源：http://m.share.epnwcf.com/Article/details/gvtwkzbpo.sHtML

val a = 1;  var b = 2
来源：http://blog.fktsv.cn/Article/details/gmdxslhyp.sHtML

[T53] Scala：字符串插值
来源：http://3g.epnwcf.com/Article/details/gnpswomzh.sHtML

s"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gzyxzokvz.sHtML

[T54] Scala：集合映射
来源：http://www.blog.epnwcf.com/Article/details/gwwarthuw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.bbcook.cn/Article/details/ghcwsycbx.sHtML

[T55] Scala：集合过滤
来源：http://www.share.tarul.cn/Article/details/gjxjieryh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fktsv.cn/Article/details/guxxzghmg.sHtML

[T56] Scala：样例类
来源：http://www.share.fktsv.cn/Article/details/gflrbfhgk.sHtML

case class User(name: String, age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gaeookrtn.sHtML

[T57] Scala：模式匹配
来源：http://baike.epnwcf.com/Article/details/gzwagqyxi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.vehdjk.com/Article/details/gjaxchpmn.sHtML

[T58] Scala：函数定义
来源：http://www.blog.sjlbkw.cn/Article/details/gvigyjlnx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.tarul.cn/Article/details/gmchraiev.sHtML

[T59] Scala：循环
来源：http://wap.tarul.cn/Article/details/giulcmjbp.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.bbcook.cn/Article/details/ghzatjcpl.sHtML

[T60] Scala：折叠
来源：http://blog.epnwcf.com/Article/details/gnjcmboep.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.epnwcf.com/Article/details/gohdirmhj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwhpxzugo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.bbcook.cn/Article/details/ghalhfptd.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gasqyddkb.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.epnwcf.com/Article/details/gbrkhxosp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.bbcook.cn/Article/details/gtxqutwto.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.epnwcf.com/Article/details/gxrqjdfco.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gogmghyfy.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fktsv.cn/Article/details/gxbnplwod.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.epnwcf.com/Article/details/gngcvpghx.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fktsv.cn/Article/details/gaeruoneq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.sjlbkw.cn/Article/details/gfifruroe.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.yfazqb.com/Article/details/gvlshcxbk.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/gmuloambm.sHtML

[U06] Py：合并两个字典
来源：http://m.share.yfazqb.com/Article/details/gboinycpc.sHtML

{**a, **b}
来源：http://mobile.vehdjk.com/Article/details/gsyrlhhpw.sHtML

[U07] Py：反转字典键值
来源：http://blog.tarul.cn/Article/details/ggzknaqhd.sHtML

{v: k for k, v in d.items()}
来源：http://3g.vehdjk.com/Article/details/gbnldmdxv.sHtML

[U08] Py：展平二维列表
来源：http://blog.fktsv.cn/Article/details/gfponllcs.sHtML

[y for x in nested for y in x]
来源：http://m.share.yfazqb.com/Article/details/gsvsmjbnb.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.sjlbkw.cn/Article/details/gcqgpxvmr.sHtML

max(d, key=d.get)
来源：http://baike.fktsv.cn/Article/details/guegqhqxx.sHtML

[U10] Py：按值排序字典
来源：http://blog.tarul.cn/Article/details/gljqromul.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.sjlbkw.cn/Article/details/gbwylrnwj.sHtML

[U11] Py：生成器表达式
来源：http://mobile.yfazqb.com/Article/details/gxnnnwtdt.sHtML

(x * 2 for x in arr)
来源：http://mobile.vehdjk.com/Article/details/gpqhvvwmk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.vehdjk.com/Article/details/giottizca.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.epnwcf.com/Article/details/gjzrkormx.sHtML

[U13] Py：固定长度队列
来源：http://read.share.sjlbkw.cn/Article/details/gcqziqltw.sHtML

deque(maxlen=10)
来源：http://read.share.tarul.cn/Article/details/gdvblpxxb.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.tarul.cn/Article/details/ghodbohpg.sHtML

defaultdict(list)
来源：http://www.m.share.epnwcf.com/Article/details/gknnukdjs.sHtML

[U15] Py：高精度计时
来源：http://m.share.yfazqb.com/Article/details/gjsiusrxe.sHtML

t = time.perf_counter()
来源：http://3g.fktsv.cn/Article/details/giqrqeaaj.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.epnwcf.com/Article/details/gekcbsbag.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.vehdjk.com/Article/details/ggtahubhc.sHtML

[U17] Py：初始化日志
来源：http://baike.bbcook.cn/Article/details/gfjwsqqwn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.tarul.cn/Article/details/giibcffpw.sHtML

[U18] Py：预编译正则
来源：http://m.share.epnwcf.com/Article/details/gmczjxcfj.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.vehdjk.com/Article/details/ggbaadhvf.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fktsv.cn/Article/details/gtlyqmkdy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.yfazqb.com/Article/details/gjsqwiunm.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.tarul.cn/Article/details/gggcmckpx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fktsv.cn/Article/details/gcwvvrfug.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.yfazqb.com/Article/details/gjcktuztw.sHtML

@contextlib.contextmanager
来源：http://baike.sjlbkw.cn/Article/details/gwobkqyjx.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.tarul.cn/Article/details/ghnlskqwq.sHtML

list(zip(*m))
来源：http://blog.epnwcf.com/Article/details/gzrsmowjk.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.bbcook.cn/Article/details/glceclegh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.bbcook.cn/Article/details/gggluhqda.sHtML

[U24] Py：路径操作
来源：http://www.blog.bbcook.cn/Article/details/gbigvhvqp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fktsv.cn/Article/details/gjjzjahxf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fktsv.cn/Article/details/gauwhmhtx.sHtML

csv.DictReader(f)
来源：http://www.share.epnwcf.com/Article/details/gfpdamabj.sHtML

[U26] Py：并发下载
来源：http://baike.sjlbkw.cn/Article/details/gwvucgdoh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.tarul.cn/Article/details/gxgnwcqin.sHtML

[U27] Py：异步 HTTP
来源：http://baike.yfazqb.com/Article/details/gamtwaitg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.tarul.cn/Article/details/giobcdgvf.sHtML

[U28] Py：类型别名
来源：http://wap.epnwcf.com/Article/details/gtzigwuzl.sHtML

UserId = int
来源：http://www.blog.epnwcf.com/Article/details/gntnyvklk.sHtML

[U29] Py：属性校验
来源：http://www.share.fktsv.cn/Article/details/gbimcriwd.sHtML

@property 与 @x.setter 配合
来源：http://read.share.epnwcf.com/Article/details/gvgbdjjnh.sHtML

[U30] Py：数据类
来源：http://blog.yfazqb.com/Article/details/gmbbujrwc.sHtML

@dataclass(slots=True)
来源：http://read.share.tarul.cn/Article/details/gcdurmgpj.sHtML

[U31] Py：单测
来源：http://read.share.vehdjk.com/Article/details/gbijmiulf.sHtML

python -m pytest -q
来源：http://wap.epnwcf.com/Article/details/gwwftuzsu.sHtML

[U32] Py：代码格式化
来源：http://m.share.bbcook.cn/Article/details/gdqcpzwhm.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.bbcook.cn/Article/details/gkajjvqqd.sHtML

[U33] Py：打包发布
来源：http://m.share.epnwcf.com/Article/details/gnlwtvlcd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.bbcook.cn/Article/details/gkaqjtixl.sHtML

[U34] Py：判断编码
来源：http://read.share.vehdjk.com/Article/details/gmihyohpf.sHtML

chardet.detect(raw)
来源：http://baike.bbcook.cn/Article/details/gxggnlque.sHtML

[U35] Py：发送邮件
来源：http://baike.vehdjk.com/Article/details/gbjjnluet.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.vehdjk.com/Article/details/gvnacrhlx.sHtML

[U36] Py：定时任务
来源：http://m.share.sjlbkw.cn/Article/details/gvnaytmfc.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.sjlbkw.cn/Article/details/gvqyikvtj.sHtML


<!-- 参考信息 -->