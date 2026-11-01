代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gvsusrzls.sHtML

[S10] C：指针与解引用
来源：http://www.share.fktsv.cn/Article/details/grhtkoxoz.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gerurbumy.sHtML

[S11] C：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gkhdnwztl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fktsv.cn/Article/details/ghlmftycm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.sjlbkw.cn/Article/details/gillvruav.sHtML

fclose(f);
来源：http://3g.fktsv.cn/Article/details/ghsbdoboi.sHtML

[S12] C：写文件
来源：http://blog.bbcook.cn/Article/details/gxbjmtlgo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/gylaymenv.sHtML

[S13] C：宏定义
来源：http://www.share.fktsv.cn/Article/details/gdkwzmcep.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.bbcook.cn/Article/details/gyrvtfuow.sHtML

[S14] C：枚举
来源：http://read.share.tarul.cn/Article/details/gdgcbuzhz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkxpykvy.sHtML

[S15] C：类型转换
来源：http://mobile.epnwcf.com/Article/details/gimdwzltd.sHtML

(double) a / b
来源：http://wap.bbcook.cn/Article/details/gulaxmsuo.sHtML

[S16] C：位操作置位
来源：http://3g.bbcook.cn/Article/details/gpkkxnkdm.sHtML

x |= (1 << 3);
来源：http://read.share.fktsv.cn/Article/details/grqczqcnn.sHtML

[S17] C：安全拼接字符串
来源：http://blog.tarul.cn/Article/details/ghxzcvrem.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fktsv.cn/Article/details/gqxxfpjba.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/gbqlrgtgj.sHtML

int main(int argc, char **argv)
来源：http://m.share.tarul.cn/Article/details/gckitqbit.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/gsruijvxj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/guqdbxlqr.sHtML

[S20] C：二分查找
来源：http://read.share.vehdjk.com/Article/details/gstoaskjc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gzmpnsgcr.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fktsv.cn/Article/details/gnvnfcamb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fktsv.cn/Article/details/gwmjcjgik.sHtML

[S22] C：字符串转数字
来源：http://blog.fktsv.cn/Article/details/gpfveoazd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.yfazqb.com/Article/details/gmcqchsxa.sHtML

[S23] C：随机数
来源：http://baike.yfazqb.com/Article/details/glqrlhifd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.tarul.cn/Article/details/gxeocjwie.sHtML

[S24] C：获取本地时间
来源：http://www.blog.epnwcf.com/Article/details/gnrjmhevt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fktsv.cn/Article/details/gwtutkyjm.sHtML

[S25] C：内存拷贝
来源：http://baike.epnwcf.com/Article/details/gmgwqzuvr.sHtML

memcpy(dst, src, n);
来源：http://www.share.sjlbkw.cn/Article/details/gbxbjbzbm.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gazpsndzc.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gxqxgjecm.sHtML

[S27] C：定义常量
来源：http://m.share.tarul.cn/Article/details/gtqwhqwww.sHtML

const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gqhrkoitb.sHtML

[S28] C：静态变量
来源：http://www.m.share.epnwcf.com/Article/details/gybeqmopa.sHtML

static int counter = 0;
来源：http://wap.fktsv.cn/Article/details/gmlsexwsf.sHtML

[S29] C：变参函数
来源：http://baike.vehdjk.com/Article/details/gfsarlpmt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.epnwcf.com/Article/details/gwqdolpkk.sHtML

[S30] C：头文件保护
来源：http://www.blog.bbcook.cn/Article/details/gnsnqyarg.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/gofyjpxhk.sHtML

#define X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/gowtgmoen.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/gxzxrfxuo.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/ganyuvivt.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gybysiylz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.epnwcf.com/Article/details/geuqfuzqq.sHtML

[S32] C++：字符串
来源：http://wap.vehdjk.com/Article/details/guzzoioqq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/ggjrbjifc.sHtML

[S33] C++：vector 增删
来源：http://www.share.bbcook.cn/Article/details/gvbzsyhbc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/gejfzkius.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/gpcgxbbzp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.yfazqb.com/Article/details/gdptspplq.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/ggxdmtmni.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gpgzxfbrj.sHtML

[S36] C++：unordered_map
来源：http://mobile.bbcook.cn/Article/details/gvoukmnbk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/grufbvmbt.sHtML

[S37] C++：set
来源：http://baike.bbcook.cn/Article/details/ghlqlwjhs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.tarul.cn/Article/details/gjpgbmzef.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/gcndpelft.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.yfazqb.com/Article/details/gxmunlfug.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/gopmtfmeb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.epnwcf.com/Article/details/gbkojvozu.sHtML

[S40] C++：查找元素
来源：http://wap.fktsv.cn/Article/details/goxdeixaq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.yfazqb.com/Article/details/gidxofnkz.sHtML

[S41] C++：类与构造函数
来源：http://read.share.epnwcf.com/Article/details/gdcfgojss.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.sjlbkw.cn/Article/details/gnwxeiaau.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fktsv.cn/Article/details/gwvqxzhzp.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.vehdjk.com/Article/details/ghgrvutje.sHtML

[S43] C++：智能指针
来源：http://www.share.bbcook.cn/Article/details/gddkgdvjc.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/gcwwviysb.sHtML

[S44] C++：引用传参
来源：http://3g.tarul.cn/Article/details/gnjrgwqre.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.tarul.cn/Article/details/gfijyjwup.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/gevnxzbox.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fktsv.cn/Article/details/ghwhhvowv.sHtML

[S46] C++：函数模板
来源：http://www.share.tarul.cn/Article/details/gbavyfpua.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.bbcook.cn/Article/details/gupsrrruc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.epnwcf.com/Article/details/gukfuwpri.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/ggwsdnbsi.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gpsempqfw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.sjlbkw.cn/Article/details/ghjbxgqlz.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fktsv.cn/Article/details/giwnqdgkj.sHtML

[S49] C++：写文件
来源：http://read.share.fktsv.cn/Article/details/gnhyuxwri.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/gjwxmivyz.sHtML

[S50] C++：格式化数字
来源：http://3g.bbcook.cn/Article/details/gpagicojt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gveosmarc.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.yfazqb.com/Article/details/gjdvwepio.sHtML

static_cast<double>(a) / b
来源：http://blog.sjlbkw.cn/Article/details/gzsakriip.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fktsv.cn/Article/details/gqmiaxwdi.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/gvwjwtmjp.sHtML

[S53] C++：移动语义
来源：http://baike.yfazqb.com/Article/details/gktpsjekc.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.vehdjk.com/Article/details/ghywgjyqr.sHtML

[S54] C++：异常处理
来源：http://mobile.sjlbkw.cn/Article/details/gwkxijald.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.tarul.cn/Article/details/gdrlvtfxo.sHtML

[S55] C++：结构化绑定
来源：http://m.share.epnwcf.com/Article/details/gizielrzl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.yfazqb.com/Article/details/gsjgvbzmh.sHtML

[S56] C++：optional
来源：http://www.m.share.bbcook.cn/Article/details/gqakkeypn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.tarul.cn/Article/details/gdoyiqalz.sHtML

[S57] C++：编译期常量
来源：http://wap.vehdjk.com/Article/details/gnjktzlwg.sHtML

constexpr int N = 10;
来源：http://m.share.fktsv.cn/Article/details/gkatqnsmj.sHtML

[S58] C++：命名空间
来源：http://www.share.fktsv.cn/Article/details/gkicsdxjv.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.vehdjk.com/Article/details/ginihikrn.sHtML

[S59] C++：静态断言
来源：http://www.blog.fktsv.cn/Article/details/gahjwciqr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/gxilmxymz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.bbcook.cn/Article/details/gplltcvfg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.epnwcf.com/Article/details/gcwcicmqh.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gkyffvwwq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gvxnlaqgq.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtzetyuca.sHtML

[T01] Kotlin：Hello World
来源：http://3g.bbcook.cn/Article/details/gqwniwcvo.sHtML

println("Hello")
来源：http://wap.vehdjk.com/Article/details/gplpdybuj.sHtML

[T02] Kotlin：变量
来源：http://mobile.yfazqb.com/Article/details/gtvkmcavz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.vehdjk.com/Article/details/gmlejobcx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/geeihihig.sHtML

"值: $b"
来源：http://3g.vehdjk.com/Article/details/gsvmztkjn.sHtML

[T04] Kotlin：空安全
来源：http://blog.epnwcf.com/Article/details/gcqycgrki.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqfekgnt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.tarul.cn/Article/details/ggmqcspcq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/gaokygvoh.sHtML

[T06] Kotlin：集合映射
来源：http://3g.yfazqb.com/Article/details/gqcxfenid.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.vehdjk.com/Article/details/glnimgizz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gfwvtouau.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.bbcook.cn/Article/details/gcybsbbim.sHtML

[T08] Kotlin：数据类
来源：http://m.share.vehdjk.com/Article/details/garwryqcq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.vehdjk.com/Article/details/gzidjcqru.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/gpilgatqp.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.tarul.cn/Article/details/gmucgppvz.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fktsv.cn/Article/details/gfpqxjode.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.epnwcf.com/Article/details/ghdkdhure.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fktsv.cn/Article/details/gjmxherxy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.bbcook.cn/Article/details/gfxsqwvnq.sHtML

[T12] Kotlin：解构声明
来源：http://wap.epnwcf.com/Article/details/gaqhjmvak.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.yfazqb.com/Article/details/gkrougynf.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fktsv.cn/Article/details/guhhbryoq.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/gttqecgwf.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.bbcook.cn/Article/details/gathxqjde.sHtML

for (i in 1..10) println(i)
来源：http://mobile.bbcook.cn/Article/details/gxbidpezk.sHtML

[T15] Kotlin：接口
来源：http://wap.yfazqb.com/Article/details/ggdvoowjs.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.bbcook.cn/Article/details/gdvygbvyu.sHtML

[T16] Swift：Hello World
来源：http://baike.fktsv.cn/Article/details/gurzzmsbg.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gxzovjvhy.sHtML

[T17] Swift：变量与常量
来源：http://mobile.yfazqb.com/Article/details/giockdinc.sHtML

var a = 1;  let b = 2
来源：http://m.share.bbcook.cn/Article/details/gcudvmtgn.sHtML

[T18] Swift：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gexhoiznf.sHtML

"值: \(b)"
来源：http://read.share.yfazqb.com/Article/details/gzgndazzx.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/gxqcsshdg.sHtML

if let n = opt { print(n) }
来源：http://www.share.fktsv.cn/Article/details/gmmkxnwlh.sHtML

[T20] Swift：数组操作
来源：http://3g.yfazqb.com/Article/details/gzunoktfi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.bbcook.cn/Article/details/gnmnjtjic.sHtML

[T21] Swift：遍历
来源：http://baike.fktsv.cn/Article/details/gcmkdtwwe.sHtML

for x in a { print(x) }
来源：http://www.share.bbcook.cn/Article/details/gclqeylvu.sHtML

[T22] Swift：字典
来源：http://www.m.share.yfazqb.com/Article/details/gkjwqgtvt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.epnwcf.com/Article/details/gbztttxsr.sHtML

[T23] Swift：函数
来源：http://www.share.fktsv.cn/Article/details/goixckmwk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/gsvyzymbd.sHtML

[T24] Swift：闭包
来源：http://wap.sjlbkw.cn/Article/details/gbhrjiabs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.bbcook.cn/Article/details/gkgjbsljv.sHtML

[T25] Swift：结构体
来源：http://mobile.epnwcf.com/Article/details/giyxkqnmb.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/gfravblmc.sHtML

[T26] Swift：类与重写
来源：http://www.blog.vehdjk.com/Article/details/gjdnlpxwe.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fktsv.cn/Article/details/gtcwrlxfi.sHtML

[T27] Swift：错误处理
来源：http://3g.tarul.cn/Article/details/gadntsxdw.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fktsv.cn/Article/details/gtmysxxqm.sHtML

[T28] Swift：枚举
来源：http://www.blog.tarul.cn/Article/details/gxabfqzhp.sHtML

enum Color { case red, green }
来源：http://www.share.vehdjk.com/Article/details/gdlcfpxjw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/gclzmyzco.sHtML

guard let x = opt else { return }
来源：http://m.share.bbcook.cn/Article/details/guuoswwde.sHtML

[T30] Swift：协议
来源：http://www.share.epnwcf.com/Article/details/gpvtujtfu.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.epnwcf.com/Article/details/gthfqhjqp.sHtML

[T31] Lua：Hello World
来源：http://m.share.vehdjk.com/Article/details/genkvzpna.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/glridsyyz.sHtML

[T32] Lua：局部变量
来源：http://m.share.fktsv.cn/Article/details/gtrfprnjo.sHtML

local a = 1
来源：http://blog.bbcook.cn/Article/details/gwtvuymqt.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fktsv.cn/Article/details/gpzaluurf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.epnwcf.com/Article/details/gbvjatdtt.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gjguqrcvu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/gziepkaya.sHtML

[T35] Lua：字典表
来源：http://blog.sjlbkw.cn/Article/details/gafdnogxy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gdloyfygv.sHtML

[T36] Lua：函数
来源：http://www.share.yfazqb.com/Article/details/gcewkegzv.sHtML

function add(a, b) return a + b end
来源：http://baike.sjlbkw.cn/Article/details/gdlfzulia.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gfdgbjjej.sHtML

"a" .. "b"
来源：http://3g.yfazqb.com/Article/details/gsttnnczr.sHtML

[T38] Lua：条件
来源：http://baike.epnwcf.com/Article/details/gxsupcclv.sHtML

if x > 0 then print("正") end
来源：http://wap.vehdjk.com/Article/details/grxdesyiv.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/grwbaigkx.sHtML

string.find(s, "%d+")
来源：http://baike.fktsv.cn/Article/details/gnjiskxxi.sHtML

[T40] Lua：元表
来源：http://m.share.vehdjk.com/Article/details/gijzdszef.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.vehdjk.com/Article/details/gekkrveyb.sHtML

[T41] Perl：Hello World
来源：http://m.share.tarul.cn/Article/details/gdroxjycj.sHtML

print "Hello\n";
来源：http://wap.yfazqb.com/Article/details/gvuqbxaug.sHtML

[T42] Perl：变量类型
来源：http://baike.fktsv.cn/Article/details/gcvtmzaao.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fktsv.cn/Article/details/gvryihmmo.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gtahzctty.sHtML

"值: $a"
来源：http://wap.fktsv.cn/Article/details/goghimdvd.sHtML

[T44] Perl：条件
来源：http://m.share.vehdjk.com/Article/details/ggrsgrkst.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.vehdjk.com/Article/details/gzvqjeskj.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.tarul.cn/Article/details/gydiffhpa.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.bbcook.cn/Article/details/gpbwazdky.sHtML

[T46] Perl：哈希操作
来源：http://www.share.vehdjk.com/Article/details/gtripkuxi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/gxzwsajns.sHtML

[T47] Perl：正则捕获
来源：http://wap.vehdjk.com/Article/details/gbbpfhnbc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.yfazqb.com/Article/details/gcnxirdif.sHtML

[T48] Perl：正则替换
来源：http://www.share.tarul.cn/Article/details/gwfnzakgw.sHtML

$s =~ s/old/new/g;
来源：http://baike.vehdjk.com/Article/details/gnimijrij.sHtML

[T49] Perl：函数
来源：http://baike.tarul.cn/Article/details/gnpuzjzen.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gnmbgtbyq.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gvreafajd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.sjlbkw.cn/Article/details/gfsebtsbq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.tarul.cn/Article/details/gbatqzqyk.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gdimldxzw.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gudrqyhrv.sHtML

[T52] Scala：变量
来源：http://www.share.epnwcf.com/Article/details/gkpsabhwy.sHtML

val a = 1;  var b = 2
来源：http://www.blog.bbcook.cn/Article/details/gknehoifd.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gwjhqoecd.sHtML

s"值: $b"
来源：http://wap.tarul.cn/Article/details/gwvutqhed.sHtML

[T54] Scala：集合映射
来源：http://m.share.fktsv.cn/Article/details/gficvzrjp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.yfazqb.com/Article/details/gbrxnlylu.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.yfazqb.com/Article/details/gmhczqxbx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.tarul.cn/Article/details/gvieayzjt.sHtML

[T56] Scala：样例类
来源：http://baike.epnwcf.com/Article/details/graatyyje.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fktsv.cn/Article/details/gcfdyriqq.sHtML

[T57] Scala：模式匹配
来源：http://blog.bbcook.cn/Article/details/ghwlgofmx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.bbcook.cn/Article/details/gjsgtcdwe.sHtML

[T58] Scala：函数定义
来源：http://blog.vehdjk.com/Article/details/gyfvglttt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.vehdjk.com/Article/details/ghmsdvgga.sHtML

[T59] Scala：循环
来源：http://www.share.bbcook.cn/Article/details/gqothzsvk.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gpdnybcnc.sHtML

[T60] Scala：折叠
来源：http://wap.sjlbkw.cn/Article/details/gtsoygqqn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/gdmmeajkd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzawonqxw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.tarul.cn/Article/details/gltmfldwy.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjggzllti.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.yfazqb.com/Article/details/ggingriqv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.vehdjk.com/Article/details/gglhvchoe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.epnwcf.com/Article/details/guubsdmkh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.bbcook.cn/Article/details/ghuveniyq.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.sjlbkw.cn/Article/details/gbebxfohn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.tarul.cn/Article/details/gnbwxvlcj.sHtML

[U04] Py：变量调试打印
来源：http://blog.fktsv.cn/Article/details/gvqtbchei.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.yfazqb.com/Article/details/gmnolfehv.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.sjlbkw.cn/Article/details/ghypqjftk.sHtML

list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/ghabpudim.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fktsv.cn/Article/details/gxqocyvxt.sHtML

{**a, **b}
来源：http://www.m.share.vehdjk.com/Article/details/grcgfxpeq.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fktsv.cn/Article/details/gaipquihb.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.tarul.cn/Article/details/gorqnmxmv.sHtML

[U08] Py：展平二维列表
来源：http://3g.bbcook.cn/Article/details/gtrtvteuf.sHtML

[y for x in nested for y in x]
来源：http://wap.bbcook.cn/Article/details/gbwxanqae.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.tarul.cn/Article/details/gxlzrgyil.sHtML

max(d, key=d.get)
来源：http://baike.bbcook.cn/Article/details/gnvxfapta.sHtML

[U10] Py：按值排序字典
来源：http://baike.yfazqb.com/Article/details/gmlgxmrjh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.sjlbkw.cn/Article/details/gkdnrmnkw.sHtML

[U11] Py：生成器表达式
来源：http://read.share.epnwcf.com/Article/details/gwawetxkr.sHtML

(x * 2 for x in arr)
来源：http://www.blog.tarul.cn/Article/details/gilvwppsn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.vehdjk.com/Article/details/gyapneyyv.sHtML

Counter(arr).most_common(3)
来源：http://blog.tarul.cn/Article/details/gsmfyfokg.sHtML

[U13] Py：固定长度队列
来源：http://read.share.sjlbkw.cn/Article/details/gmrwpkujt.sHtML

deque(maxlen=10)
来源：http://mobile.tarul.cn/Article/details/gooqlbino.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fktsv.cn/Article/details/gztssvenz.sHtML

defaultdict(list)
来源：http://3g.tarul.cn/Article/details/gcqpiptlr.sHtML

[U15] Py：高精度计时
来源：http://m.share.yfazqb.com/Article/details/gdwhuvdrk.sHtML

t = time.perf_counter()
来源：http://3g.tarul.cn/Article/details/gevblxqwu.sHtML

[U16] Py：命令行参数解析
来源：http://wap.vehdjk.com/Article/details/ghbwwwjpf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.vehdjk.com/Article/details/gkieklack.sHtML

[U17] Py：初始化日志
来源：http://read.share.vehdjk.com/Article/details/gfnbmxhnn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.vehdjk.com/Article/details/ggkmuheqr.sHtML

[U18] Py：预编译正则
来源：http://read.share.sjlbkw.cn/Article/details/gjhsdkzmj.sHtML

pat = re.compile(r"\d+")
来源：http://baike.vehdjk.com/Article/details/gusgfytjy.sHtML

[U19] Py：正则替换带回调
来源：http://wap.yfazqb.com/Article/details/gyrkqtexs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fktsv.cn/Article/details/ghaafobiq.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fktsv.cn/Article/details/grcrtdhaw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.bbcook.cn/Article/details/gfoshsnfg.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fktsv.cn/Article/details/gizoxdpvv.sHtML

@contextlib.contextmanager
来源：http://baike.sjlbkw.cn/Article/details/gdlcqormj.sHtML

[U22] Py：矩阵转置
来源：http://m.share.yfazqb.com/Article/details/gbgkpqacg.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/gpluggaod.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.tarul.cn/Article/details/gbvppinpn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.vehdjk.com/Article/details/grpgbnysd.sHtML

[U24] Py：路径操作
来源：http://wap.sjlbkw.cn/Article/details/gpszvcwut.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.bbcook.cn/Article/details/gmhxaaqks.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.bbcook.cn/Article/details/gsnqxixjg.sHtML

csv.DictReader(f)
来源：http://3g.epnwcf.com/Article/details/gphuebijv.sHtML

[U26] Py：并发下载
来源：http://read.share.epnwcf.com/Article/details/gajpsbejv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.tarul.cn/Article/details/gnfephfgn.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fktsv.cn/Article/details/gligitysx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.sjlbkw.cn/Article/details/gmibhvrzb.sHtML

[U28] Py：类型别名
来源：http://www.blog.vehdjk.com/Article/details/gffvqehdi.sHtML

UserId = int
来源：http://wap.epnwcf.com/Article/details/gxwptbsrs.sHtML

[U29] Py：属性校验
来源：http://www.share.fktsv.cn/Article/details/gtegrynlz.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.epnwcf.com/Article/details/gtobhmmgh.sHtML

[U30] Py：数据类
来源：http://m.share.fktsv.cn/Article/details/gxzpviole.sHtML

@dataclass(slots=True)
来源：http://www.share.vehdjk.com/Article/details/grtprhuio.sHtML

[U31] Py：单测
来源：http://www.m.share.tarul.cn/Article/details/gwilxjeeb.sHtML

python -m pytest -q
来源：http://www.blog.sjlbkw.cn/Article/details/gdrrrrtdb.sHtML

[U32] Py：代码格式化
来源：http://mobile.yfazqb.com/Article/details/ghwgwbfyd.sHtML

ruff format . && ruff check --fix .
来源：http://3g.epnwcf.com/Article/details/gazbjykzo.sHtML


<!-- 参考信息 -->