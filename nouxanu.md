代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/gvpldedwj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.yfazqb.com/Article/details/gbzchfdcf.sHtML

fclose(f);
来源：http://mobile.tarul.cn/Article/details/gltnvjagg.sHtML

[S12] C：写文件
来源：http://wap.tarul.cn/Article/details/ggsbmxahh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gtdttvinf.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/gnhiyohqp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fktsv.cn/Article/details/godbrjyia.sHtML

[S14] C：枚举
来源：http://read.share.fktsv.cn/Article/details/gpsugpoxk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.bbcook.cn/Article/details/gjinqxxbm.sHtML

[S15] C：类型转换
来源：http://www.m.share.tarul.cn/Article/details/gdezplamm.sHtML

(double) a / b
来源：http://www.share.vehdjk.com/Article/details/gdjylrdzb.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/gufzguitt.sHtML

x |= (1 << 3);
来源：http://blog.tarul.cn/Article/details/glzwgnoob.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gusgpprvn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfscgudmk.sHtML

[S18] C：命令行参数
来源：http://www.share.sjlbkw.cn/Article/details/gnezxcias.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/gcxtswndw.sHtML

[S19] C：快速排序
来源：http://www.blog.yfazqb.com/Article/details/gjwhlxkia.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gclydpzrh.sHtML

[S20] C：二分查找
来源：http://www.m.share.yfazqb.com/Article/details/gwvhcnala.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/giyyjdfky.sHtML

[S21] C：字符类别判断
来源：http://3g.epnwcf.com/Article/details/gvmkcqgbb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.sjlbkw.cn/Article/details/grgtzyxpb.sHtML

[S22] C：字符串转数字
来源：http://www.share.vehdjk.com/Article/details/gfrnqelzj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gtyzlnnue.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/glktkpfaz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/gjvpuqewb.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.epnwcf.com/Article/details/gadmofqse.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.tarul.cn/Article/details/gggzhdydd.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gyfobcvfx.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.yfazqb.com/Article/details/gbhihsrag.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/gcdsbhakq.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fktsv.cn/Article/details/gwuhhemec.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gtdvsjurd.sHtML

const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gjybmrfga.sHtML

[S28] C：静态变量
来源：http://www.m.share.fktsv.cn/Article/details/gbgbnjifu.sHtML

static int counter = 0;
来源：http://wap.tarul.cn/Article/details/gsjrldfls.sHtML

[S29] C：变参函数
来源：http://read.share.tarul.cn/Article/details/glnwlgqyg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.bbcook.cn/Article/details/gjmnclqqq.sHtML

[S30] C：头文件保护
来源：http://www.share.yfazqb.com/Article/details/gvmnyndgc.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gdmyyldic.sHtML

#define X_H
来源：http://www.blog.fktsv.cn/Article/details/gmmewlsyz.sHtML

#endif
来源：http://baike.tarul.cn/Article/details/gezwkjafi.sHtML

[S31] C++：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/glwjaierb.sHtML

#include <iostream>
来源：http://m.share.sjlbkw.cn/Article/details/gesyfcvdz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.sjlbkw.cn/Article/details/gjeegghqj.sHtML

[S32] C++：字符串
来源：http://m.share.tarul.cn/Article/details/gdcxpkhyo.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/grextrtle.sHtML

[S33] C++：vector 增删
来源：http://www.share.yfazqb.com/Article/details/ghgruqtlx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fktsv.cn/Article/details/gtcepyppp.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/gfuezszgu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.yfazqb.com/Article/details/gqejbzaod.sHtML

[S35] C++：map
来源：http://blog.tarul.cn/Article/details/gfixtlqgv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gipyozyaw.sHtML

[S36] C++：unordered_map
来源：http://www.share.yfazqb.com/Article/details/gpdrryocf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/galpbwvph.sHtML

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/gnobzbnvk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.tarul.cn/Article/details/gqzftinvl.sHtML

[S38] C++：排序
来源：http://blog.epnwcf.com/Article/details/gyselgmxc.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.vehdjk.com/Article/details/gawvpryjz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.yfazqb.com/Article/details/gyqgsfefk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.bbcook.cn/Article/details/gdcayaumu.sHtML

[S40] C++：查找元素
来源：http://www.blog.yfazqb.com/Article/details/giepxnfga.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/goyysiwsx.sHtML

[S41] C++：类与构造函数
来源：http://www.share.vehdjk.com/Article/details/gvwgadtwe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/ggfgwqlxk.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.yfazqb.com/Article/details/ggdmxcmmj.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.vehdjk.com/Article/details/grfjyieph.sHtML

[S43] C++：智能指针
来源：http://blog.yfazqb.com/Article/details/gukokvqvn.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.vehdjk.com/Article/details/gcnlepcbl.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gvlkhbwgg.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gptcyqcad.sHtML

[S45] C++：lambda
来源：http://baike.tarul.cn/Article/details/gjirecyqv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fktsv.cn/Article/details/giamzkyim.sHtML

[S46] C++：函数模板
来源：http://mobile.epnwcf.com/Article/details/gvmeqboaj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/gmgcidtue.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.epnwcf.com/Article/details/gohcqwidu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.epnwcf.com/Article/details/grsbturpq.sHtML

[S48] C++：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gmzdflzlw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fktsv.cn/Article/details/gzvfykefd.sHtML

while (std::getline(in, line)) { }
来源：http://3g.epnwcf.com/Article/details/gfxcnobyz.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/gkeblvqpl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.bbcook.cn/Article/details/ginrqbedk.sHtML

[S50] C++：格式化数字
来源：http://www.blog.vehdjk.com/Article/details/gnkmttpck.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gdoefzdiz.sHtML

[S51] C++：显式类型转换
来源：http://baike.fktsv.cn/Article/details/gvxlbypdu.sHtML

static_cast<double>(a) / b
来源：http://baike.bbcook.cn/Article/details/gekpypuqe.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoaniyfk.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.tarul.cn/Article/details/gjkexbvct.sHtML

[S53] C++：移动语义
来源：http://www.share.epnwcf.com/Article/details/gakpbtwni.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.yfazqb.com/Article/details/gloqjnajo.sHtML

[S54] C++：异常处理
来源：http://www.share.sjlbkw.cn/Article/details/gblvyjbub.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.yfazqb.com/Article/details/gkxlyvyxa.sHtML

[S55] C++：结构化绑定
来源：http://baike.bbcook.cn/Article/details/gwrvucmxj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/goovpktik.sHtML

[S56] C++：optional
来源：http://blog.bbcook.cn/Article/details/gajoobhtm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/gzpnkbfre.sHtML

[S57] C++：编译期常量
来源：http://3g.sjlbkw.cn/Article/details/ganyxfxhc.sHtML

constexpr int N = 10;
来源：http://read.share.bbcook.cn/Article/details/ghkzenpyy.sHtML

[S58] C++：命名空间
来源：http://www.share.epnwcf.com/Article/details/gqwilfipu.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.epnwcf.com/Article/details/gzlglhhox.sHtML

[S59] C++：静态断言
来源：http://www.share.tarul.cn/Article/details/gpvzsytsj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.yfazqb.com/Article/details/gyotqumgh.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.sjlbkw.cn/Article/details/gzpkvbkdd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/gigmzamyf.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/grbtztlxq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.epnwcf.com/Article/details/ggpkbbvkw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gccvmjqwq.sHtML

[T01] Kotlin：Hello World
来源：http://blog.tarul.cn/Article/details/gdzlhnwhc.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gnvrtqhth.sHtML

[T02] Kotlin：变量
来源：http://mobile.vehdjk.com/Article/details/gqpolevps.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.vehdjk.com/Article/details/gvbanjfsl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.sjlbkw.cn/Article/details/goqhvjebt.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/gtflboksn.sHtML

[T04] Kotlin：空安全
来源：http://3g.epnwcf.com/Article/details/gswmshasj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/ggiyzpzzt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.vehdjk.com/Article/details/gxuzjxzcl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.yfazqb.com/Article/details/gwybdpyco.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.epnwcf.com/Article/details/gegcpbsex.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.bbcook.cn/Article/details/goycpwuvp.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.bbcook.cn/Article/details/grrrbazdf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gxvvdqpdd.sHtML

[T08] Kotlin：数据类
来源：http://mobile.bbcook.cn/Article/details/gmdoceeab.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.tarul.cn/Article/details/gjttexzni.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.vehdjk.com/Article/details/geqrahrvy.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fktsv.cn/Article/details/godutmgfz.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.yfazqb.com/Article/details/gfpxpggha.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fktsv.cn/Article/details/gtsgsaamk.sHtML

[T11] Kotlin：协程
来源：http://mobile.fktsv.cn/Article/details/gdrxrqdzr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.bbcook.cn/Article/details/goxlxhphr.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.epnwcf.com/Article/details/gdyrebrcc.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.bbcook.cn/Article/details/ggmzxxevz.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fktsv.cn/Article/details/goxfguhxk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.vehdjk.com/Article/details/gzjdtaifs.sHtML

[T14] Kotlin：循环
来源：http://wap.bbcook.cn/Article/details/gdyrspane.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/gtnsdybvy.sHtML

[T15] Kotlin：接口
来源：http://www.blog.sjlbkw.cn/Article/details/gtrejdryb.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.yfazqb.com/Article/details/gqawxidij.sHtML

[T16] Swift：Hello World
来源：http://read.share.tarul.cn/Article/details/gjzjtngrp.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gbgipzgip.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyxblntx.sHtML

var a = 1;  let b = 2
来源：http://www.blog.bbcook.cn/Article/details/guwubotaw.sHtML

[T18] Swift：字符串插值
来源：http://3g.yfazqb.com/Article/details/gqgfdrrmu.sHtML

"值: \(b)"
来源：http://baike.vehdjk.com/Article/details/glvmkepcq.sHtML

[T19] Swift：可选绑定
来源：http://baike.fktsv.cn/Article/details/gntmufdtj.sHtML

if let n = opt { print(n) }
来源：http://m.share.yfazqb.com/Article/details/guhpqjova.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/gadssbgej.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.tarul.cn/Article/details/gkbalfdap.sHtML

[T21] Swift：遍历
来源：http://mobile.tarul.cn/Article/details/gkhkvgemp.sHtML

for x in a { print(x) }
来源：http://www.share.vehdjk.com/Article/details/gfdcnkcou.sHtML

[T22] Swift：字典
来源：http://baike.tarul.cn/Article/details/ggbehspcv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.tarul.cn/Article/details/ggayeqqsz.sHtML

[T23] Swift：函数
来源：http://blog.epnwcf.com/Article/details/ggpqycdmv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.tarul.cn/Article/details/giskgyzdu.sHtML

[T24] Swift：闭包
来源：http://mobile.sjlbkw.cn/Article/details/glonjuoex.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/gfrobkwoo.sHtML

[T25] Swift：结构体
来源：http://3g.fktsv.cn/Article/details/guxsfckrm.sHtML

struct P { var x: Int }
来源：http://blog.sjlbkw.cn/Article/details/givyyfaly.sHtML

[T26] Swift：类与重写
来源：http://www.share.bbcook.cn/Article/details/gmqkzvnpk.sHtML

class A: Base { override func f() {} }
来源：http://blog.yfazqb.com/Article/details/gombpkohs.sHtML

[T27] Swift：错误处理
来源：http://www.blog.epnwcf.com/Article/details/gveyuomsh.sHtML

do { try f() } catch { print(error) }
来源：http://3g.sjlbkw.cn/Article/details/gagdouepd.sHtML

[T28] Swift：枚举
来源：http://mobile.yfazqb.com/Article/details/gdukkzcha.sHtML

enum Color { case red, green }
来源：http://3g.fktsv.cn/Article/details/grfvjphgk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.bbcook.cn/Article/details/gknjbculn.sHtML

guard let x = opt else { return }
来源：http://www.m.share.vehdjk.com/Article/details/gwnigexpr.sHtML

[T30] Swift：协议
来源：http://blog.epnwcf.com/Article/details/geuvyomwc.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fktsv.cn/Article/details/gzgfrxluq.sHtML

[T31] Lua：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gzbfwhnda.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gqobdnpft.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.tarul.cn/Article/details/gqiondvqu.sHtML

local a = 1
来源：http://www.blog.epnwcf.com/Article/details/gnnekkkzw.sHtML

[T33] Lua：表（数组）
来源：http://3g.bbcook.cn/Article/details/gaofocoel.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.yfazqb.com/Article/details/gvbjruxpi.sHtML

[T34] Lua：遍历表
来源：http://blog.bbcook.cn/Article/details/gcgteevrs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/gzhdlcqkp.sHtML

[T35] Lua：字典表
来源：http://mobile.tarul.cn/Article/details/genwsrzrq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fktsv.cn/Article/details/gsuojwyaj.sHtML

[T36] Lua：函数
来源：http://read.share.fktsv.cn/Article/details/gmaqmvozk.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gzhoakwfn.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fktsv.cn/Article/details/gsxizodmu.sHtML

"a" .. "b"
来源：http://read.share.yfazqb.com/Article/details/gxvlodkks.sHtML

[T38] Lua：条件
来源：http://3g.epnwcf.com/Article/details/gwuwdzljf.sHtML

if x > 0 then print("正") end
来源：http://blog.bbcook.cn/Article/details/gyzgfwpxd.sHtML

[T39] Lua：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gudctzpur.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/gkgknhjhz.sHtML

[T40] Lua：元表
来源：http://blog.tarul.cn/Article/details/gkqjgaaad.sHtML

setmetatable({}, { __index = base })
来源：http://blog.epnwcf.com/Article/details/gbxjwlrey.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gwzrjpqjs.sHtML

print "Hello\n";
来源：http://www.share.sjlbkw.cn/Article/details/giwpphjpg.sHtML

[T42] Perl：变量类型
来源：http://blog.vehdjk.com/Article/details/gcklnqwnx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.sjlbkw.cn/Article/details/gejleyghj.sHtML

[T43] Perl：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gynjemhuc.sHtML

"值: $a"
来源：http://www.blog.yfazqb.com/Article/details/gduzowgdp.sHtML

[T44] Perl：条件
来源：http://baike.epnwcf.com/Article/details/gybyptofv.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fktsv.cn/Article/details/gzokhncec.sHtML

[T45] Perl：数组遍历
来源：http://mobile.yfazqb.com/Article/details/gvabnwlsr.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.sjlbkw.cn/Article/details/grfwlyupn.sHtML

[T46] Perl：哈希操作
来源：http://wap.bbcook.cn/Article/details/grijirhxf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.sjlbkw.cn/Article/details/gdugtubpz.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.yfazqb.com/Article/details/gqceeusoj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fktsv.cn/Article/details/geabtvqkn.sHtML

[T48] Perl：正则替换
来源：http://m.share.fktsv.cn/Article/details/gffpeaojp.sHtML

$s =~ s/old/new/g;
来源：http://3g.tarul.cn/Article/details/gdjkggyjc.sHtML

[T49] Perl：函数
来源：http://m.share.epnwcf.com/Article/details/glagmsofi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gpivbixox.sHtML

[T50] Perl：逐行读文件
来源：http://blog.tarul.cn/Article/details/gxgtlusww.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.epnwcf.com/Article/details/gglbigphn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.tarul.cn/Article/details/geimcikog.sHtML

[T51] Scala：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gbkcccjvw.sHtML

println("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gagehxdur.sHtML

[T52] Scala：变量
来源：http://3g.bbcook.cn/Article/details/gkdtwipro.sHtML

val a = 1;  var b = 2
来源：http://baike.yfazqb.com/Article/details/gqqyevxqf.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gxezfvilc.sHtML

s"值: $b"
来源：http://mobile.yfazqb.com/Article/details/gfxjhvdsy.sHtML

[T54] Scala：集合映射
来源：http://wap.bbcook.cn/Article/details/gvqbnwqrb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.sjlbkw.cn/Article/details/gutfmhxwq.sHtML

[T55] Scala：集合过滤
来源：http://blog.epnwcf.com/Article/details/gfjpmikpc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.sjlbkw.cn/Article/details/gfquduijy.sHtML

[T56] Scala：样例类
来源：http://m.share.sjlbkw.cn/Article/details/gujnrhwly.sHtML

case class User(name: String, age: Int)
来源：http://read.share.epnwcf.com/Article/details/glpqurokk.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/geeusnpoc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.epnwcf.com/Article/details/gkepcwzgp.sHtML

[T58] Scala：函数定义
来源：http://wap.fktsv.cn/Article/details/gjtnirkoh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.yfazqb.com/Article/details/gjnjyxwhf.sHtML

[T59] Scala：循环
来源：http://wap.fktsv.cn/Article/details/gljeyorzh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/ggmqoeylz.sHtML

[T60] Scala：折叠
来源：http://baike.vehdjk.com/Article/details/gfdxvxvwt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.epnwcf.com/Article/details/gwvnufwjx.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gbirgoggf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/gylfcfval.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gsiuldcpy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.vehdjk.com/Article/details/gfrycvhgq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.yfazqb.com/Article/details/gxnyiqanr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.vehdjk.com/Article/details/gqweplpxb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.sjlbkw.cn/Article/details/guchjldye.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fktsv.cn/Article/details/gdoaidlse.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.bbcook.cn/Article/details/gtwepomez.sHtML

[U04] Py：变量调试打印
来源：http://www.share.yfazqb.com/Article/details/gmgmlmhkc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.tarul.cn/Article/details/ghbdcqyno.sHtML

[U05] Py：列表去重且保序
来源：http://blog.vehdjk.com/Article/details/gtjvkutgx.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gqmiipqvk.sHtML

[U06] Py：合并两个字典
来源：http://wap.yfazqb.com/Article/details/gkdqptibh.sHtML

{**a, **b}
来源：http://m.share.epnwcf.com/Article/details/gqbsctkqe.sHtML

[U07] Py：反转字典键值
来源：http://wap.bbcook.cn/Article/details/giijosrso.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.epnwcf.com/Article/details/gbylrfykl.sHtML

[U08] Py：展平二维列表
来源：http://m.share.epnwcf.com/Article/details/gsxdkrrqx.sHtML

[y for x in nested for y in x]
来源：http://3g.fktsv.cn/Article/details/gyeugpljs.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.tarul.cn/Article/details/ggcbiaifp.sHtML

max(d, key=d.get)
来源：http://www.blog.tarul.cn/Article/details/gdjfkqcvv.sHtML

[U10] Py：按值排序字典
来源：http://baike.tarul.cn/Article/details/gaabdzqym.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.epnwcf.com/Article/details/grquqnknh.sHtML

[U11] Py：生成器表达式
来源：http://wap.fktsv.cn/Article/details/ghirhmwty.sHtML

(x * 2 for x in arr)
来源：http://mobile.fktsv.cn/Article/details/gjkctnjpg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.bbcook.cn/Article/details/grqfcukpf.sHtML

Counter(arr).most_common(3)
来源：http://wap.tarul.cn/Article/details/gpjqiwlsf.sHtML

[U13] Py：固定长度队列
来源：http://www.share.epnwcf.com/Article/details/gwdxiusds.sHtML

deque(maxlen=10)
来源：http://blog.bbcook.cn/Article/details/gylwqizau.sHtML

[U14] Py：分组收集到列表
来源：http://wap.bbcook.cn/Article/details/gqetimdpj.sHtML

defaultdict(list)
来源：http://www.m.share.fktsv.cn/Article/details/gtblxpgbt.sHtML

[U15] Py：高精度计时
来源：http://blog.vehdjk.com/Article/details/gmywagqck.sHtML

t = time.perf_counter()
来源：http://read.share.epnwcf.com/Article/details/gjuicnnfp.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fktsv.cn/Article/details/gokeswbmx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.tarul.cn/Article/details/gdonhvneu.sHtML

[U17] Py：初始化日志
来源：http://read.share.bbcook.cn/Article/details/genazhndr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fktsv.cn/Article/details/gvhzfajvk.sHtML

[U18] Py：预编译正则
来源：http://blog.yfazqb.com/Article/details/gyqygxojk.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/gvjzhufhd.sHtML

[U19] Py：正则替换带回调
来源：http://3g.tarul.cn/Article/details/gxhwkasik.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.sjlbkw.cn/Article/details/gpmhktfle.sHtML

[U20] Py：缓存函数结果
来源：http://wap.sjlbkw.cn/Article/details/gkzshacmn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.tarul.cn/Article/details/gagtpucmq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fktsv.cn/Article/details/gwbiwnasv.sHtML

@contextlib.contextmanager
来源：http://mobile.fktsv.cn/Article/details/gwwsnmhre.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fktsv.cn/Article/details/gxqrywork.sHtML

list(zip(*m))
来源：http://www.m.share.bbcook.cn/Article/details/gqdpwhfsc.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.tarul.cn/Article/details/gbwkodbbb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.sjlbkw.cn/Article/details/gprslnley.sHtML

[U24] Py：路径操作
来源：http://m.share.fktsv.cn/Article/details/gtydtkkzj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gtizopwsf.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.sjlbkw.cn/Article/details/gbsoaocew.sHtML

csv.DictReader(f)
来源：http://blog.bbcook.cn/Article/details/geitfgekw.sHtML

[U26] Py：并发下载
来源：http://www.m.share.sjlbkw.cn/Article/details/gzthooshl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.sjlbkw.cn/Article/details/gavefwrjx.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.sjlbkw.cn/Article/details/geltnhowr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.bbcook.cn/Article/details/ghfjrsbin.sHtML

[U28] Py：类型别名
来源：http://www.share.bbcook.cn/Article/details/grckdwpfw.sHtML

UserId = int
来源：http://wap.yfazqb.com/Article/details/ghhjbvfps.sHtML

[U29] Py：属性校验
来源：http://www.blog.yfazqb.com/Article/details/gtspycssk.sHtML

@property 与 @x.setter 配合
来源：http://read.share.bbcook.cn/Article/details/gczclkfna.sHtML

[U30] Py：数据类
来源：http://blog.fktsv.cn/Article/details/glgsjmaet.sHtML

@dataclass(slots=True)
来源：http://baike.vehdjk.com/Article/details/gireuewby.sHtML

[U31] Py：单测
来源：http://read.share.fktsv.cn/Article/details/ggetwtknl.sHtML

python -m pytest -q
来源：http://m.share.tarul.cn/Article/details/gvwoupysu.sHtML

[U32] Py：代码格式化
来源：http://www.share.fktsv.cn/Article/details/grmhklrry.sHtML

ruff format . && ruff check --fix .
来源：http://wap.epnwcf.com/Article/details/gwsnvnhzz.sHtML

[U33] Py：打包发布
来源：http://mobile.vehdjk.com/Article/details/ghmjcnyit.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.yfazqb.com/Article/details/gymqlaijp.sHtML

[U34] Py：判断编码
来源：http://m.share.fktsv.cn/Article/details/gaplrmpzy.sHtML

chardet.detect(raw)
来源：http://m.share.vehdjk.com/Article/details/gfhhvyacx.sHtML


<!-- 参考信息 -->