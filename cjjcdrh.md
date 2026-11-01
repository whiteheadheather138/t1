代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.yfazqb.com/Article/details/glsnnjhlq.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.epnwcf.com/Article/details/gdbnlsver.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/giiwiklcf.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/guctjymwy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gscklxvlo.sHtML

[S10] C：指针与解引用
来源：http://blog.sjlbkw.cn/Article/details/gbmmakhxd.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fktsv.cn/Article/details/gzalohxhg.sHtML

[S11] C：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gtcwskyoh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.vehdjk.com/Article/details/gymfctsjc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.yfazqb.com/Article/details/gygvzrijx.sHtML

fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gaudibvqa.sHtML

[S12] C：写文件
来源：http://mobile.vehdjk.com/Article/details/gdrpqmkmo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gufwdwdxz.sHtML

[S13] C：宏定义
来源：http://wap.yfazqb.com/Article/details/giszkypdx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.tarul.cn/Article/details/grtboebjr.sHtML

[S14] C：枚举
来源：http://3g.fktsv.cn/Article/details/gsifjidlt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.bbcook.cn/Article/details/gfdkzprvj.sHtML

[S15] C：类型转换
来源：http://m.share.tarul.cn/Article/details/gzfgrsjzg.sHtML

(double) a / b
来源：http://blog.yfazqb.com/Article/details/glckgobfl.sHtML

[S16] C：位操作置位
来源：http://m.share.tarul.cn/Article/details/gwgtbfmox.sHtML

x |= (1 << 3);
来源：http://wap.sjlbkw.cn/Article/details/gddzmsmkq.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gsjzoxybz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.tarul.cn/Article/details/gqiuadlhw.sHtML

[S18] C：命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gewavnjmp.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fktsv.cn/Article/details/gqwczstnw.sHtML

[S19] C：快速排序
来源：http://www.blog.bbcook.cn/Article/details/ghzdebfcw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/gbkousjno.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/gpfpcpcwq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/geugmnuad.sHtML

[S21] C：字符类别判断
来源：http://mobile.epnwcf.com/Article/details/ggsgugndc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.bbcook.cn/Article/details/gmgmtxqai.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpnofrez.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/gqgjwfukg.sHtML

[S23] C：随机数
来源：http://www.m.share.vehdjk.com/Article/details/gauegtcoc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/gvbzmbvbl.sHtML

[S24] C：获取本地时间
来源：http://blog.bbcook.cn/Article/details/gfdsapdgn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.vehdjk.com/Article/details/ggjanhpmw.sHtML

[S25] C：内存拷贝
来源：http://3g.tarul.cn/Article/details/gurchnqlz.sHtML

memcpy(dst, src, n);
来源：http://baike.sjlbkw.cn/Article/details/gxacxayvt.sHtML

[S26] C：内存清零
来源：http://m.share.vehdjk.com/Article/details/gbepollds.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.epnwcf.com/Article/details/gwnpgxrfr.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gwhcgotrr.sHtML

const double PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gwslaigku.sHtML

[S28] C：静态变量
来源：http://wap.yfazqb.com/Article/details/gwjmrllpu.sHtML

static int counter = 0;
来源：http://www.blog.sjlbkw.cn/Article/details/ganzkamfx.sHtML

[S29] C：变参函数
来源：http://m.share.sjlbkw.cn/Article/details/gqjrwacno.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fktsv.cn/Article/details/graiuprdq.sHtML

[S30] C：头文件保护
来源：http://read.share.bbcook.cn/Article/details/gnqmmnytp.sHtML

#ifndef X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfrppukl.sHtML

#define X_H
来源：http://blog.fktsv.cn/Article/details/gusnfeeky.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/gokmhrnzt.sHtML

[S31] C++：Hello World
来源：http://blog.yfazqb.com/Article/details/gdgkoanpp.sHtML

#include <iostream>
来源：http://blog.bbcook.cn/Article/details/gafvejysb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/gxfyeecqx.sHtML

[S32] C++：字符串
来源：http://blog.vehdjk.com/Article/details/gozcigryu.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gyberdqbj.sHtML

[S33] C++：vector 增删
来源：http://blog.tarul.cn/Article/details/giampmeyg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.epnwcf.com/Article/details/guugzkpzd.sHtML

[S34] C++：遍历 vector
来源：http://wap.fktsv.cn/Article/details/geghrmyew.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.tarul.cn/Article/details/gczyadtoy.sHtML

[S35] C++：map
来源：http://www.blog.yfazqb.com/Article/details/gumgmeyqo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gmjwgbdav.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/gkmawuzwf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gphnoopuh.sHtML

[S37] C++：set
来源：http://www.m.share.tarul.cn/Article/details/gmaxyqkej.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fktsv.cn/Article/details/gsuvbxfnm.sHtML

[S38] C++：排序
来源：http://www.blog.bbcook.cn/Article/details/gzbeyymtm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.bbcook.cn/Article/details/giwqrvjce.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.vehdjk.com/Article/details/gwcehzvya.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/gflowhscd.sHtML

[S40] C++：查找元素
来源：http://www.share.vehdjk.com/Article/details/gsohyktjb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.vehdjk.com/Article/details/gdjgeqfeu.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fktsv.cn/Article/details/gfeknjrbu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.bbcook.cn/Article/details/gxrmprqfj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.tarul.cn/Article/details/goauioaii.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fktsv.cn/Article/details/gsianskua.sHtML

[S43] C++：智能指针
来源：http://www.m.share.tarul.cn/Article/details/gqwkqvwui.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.vehdjk.com/Article/details/gbcbbjbwi.sHtML

[S44] C++：引用传参
来源：http://www.m.share.bbcook.cn/Article/details/gwkahkutm.sHtML

void inc(int &x) { ++x; }
来源：http://blog.bbcook.cn/Article/details/gqgiizhao.sHtML

[S45] C++：lambda
来源：http://3g.yfazqb.com/Article/details/giccmrfna.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.yfazqb.com/Article/details/gnegjsvvu.sHtML

[S46] C++：函数模板
来源：http://read.share.bbcook.cn/Article/details/gegpualsg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gebljipur.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.epnwcf.com/Article/details/gvdwosdiz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/gsbiyhscn.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gzhgddjil.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.sjlbkw.cn/Article/details/gnqpwytyu.sHtML

while (std::getline(in, line)) { }
来源：http://wap.yfazqb.com/Article/details/gusugrhdk.sHtML

[S49] C++：写文件
来源：http://wap.tarul.cn/Article/details/gtuagbmmt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.epnwcf.com/Article/details/gqtvihrhd.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.tarul.cn/Article/details/gfctzozwy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gegfxxhgm.sHtML

[S51] C++：显式类型转换
来源：http://wap.sjlbkw.cn/Article/details/glhmlfdle.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gpgaoezfa.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fktsv.cn/Article/details/gusioaoci.sHtML

int size() const noexcept { return n_; }
来源：http://blog.vehdjk.com/Article/details/gpnjvatim.sHtML

[S53] C++：移动语义
来源：http://www.blog.bbcook.cn/Article/details/gycdbtfjx.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.bbcook.cn/Article/details/gjaedopgr.sHtML

[S54] C++：异常处理
来源：http://m.share.tarul.cn/Article/details/gdhqtqzhy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fktsv.cn/Article/details/gbigqszyy.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/gyqizchww.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gqtwssvse.sHtML

[S56] C++：optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmzfqdbx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.epnwcf.com/Article/details/grbxjjqfk.sHtML

[S57] C++：编译期常量
来源：http://3g.fktsv.cn/Article/details/grtzubgdi.sHtML

constexpr int N = 10;
来源：http://mobile.epnwcf.com/Article/details/gygctorld.sHtML

[S58] C++：命名空间
来源：http://m.share.tarul.cn/Article/details/gonedtpxy.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.bbcook.cn/Article/details/gtlmqkjov.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/getgaroag.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.tarul.cn/Article/details/guuqwwypa.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gwzbfrxgb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gflnjechg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghygdmpyj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/greplxswu.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ggfflxwal.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fktsv.cn/Article/details/gxwycqoju.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gaulfgidg.sHtML

[T02] Kotlin：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gajjqmyta.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.sjlbkw.cn/Article/details/gpvywifsn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gmaqplzwz.sHtML

"值: $b"
来源：http://mobile.bbcook.cn/Article/details/grisrfucw.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/gpmwjcppw.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.tarul.cn/Article/details/gwfqpgzqo.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.sjlbkw.cn/Article/details/gybtdpimm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.yfazqb.com/Article/details/gqrfgconr.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fktsv.cn/Article/details/gispacabl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gbqzniqgp.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.tarul.cn/Article/details/gmaamugkr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/ghdvmsarq.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/glgvxkeef.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.tarul.cn/Article/details/ggqifdfvw.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.tarul.cn/Article/details/gqyfkrlqk.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.tarul.cn/Article/details/ggxfedlbc.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.yfazqb.com/Article/details/ghfxdmhjn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fktsv.cn/Article/details/gbhjaxhki.sHtML

[T11] Kotlin：协程
来源：http://m.share.vehdjk.com/Article/details/ganixdjvb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gjukggqxg.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/gdibjbsig.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gzotrqotu.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.epnwcf.com/Article/details/gtrtozvpk.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.vehdjk.com/Article/details/glsxflmep.sHtML

[T14] Kotlin：循环
来源：http://wap.bbcook.cn/Article/details/gdmfoddli.sHtML

for (i in 1..10) println(i)
来源：http://blog.epnwcf.com/Article/details/gkoxbpuoa.sHtML

[T15] Kotlin：接口
来源：http://3g.fktsv.cn/Article/details/gablsuphp.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.sjlbkw.cn/Article/details/gdqhblijm.sHtML

[T16] Swift：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gvgsvdisj.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gpndxiaps.sHtML

[T17] Swift：变量与常量
来源：http://read.share.vehdjk.com/Article/details/ggilbffwc.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/guhfskthl.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gmcaqyqnm.sHtML

"值: \(b)"
来源：http://www.share.tarul.cn/Article/details/gvsfbfwjb.sHtML

[T19] Swift：可选绑定
来源：http://www.share.epnwcf.com/Article/details/gtepfpwal.sHtML

if let n = opt { print(n) }
来源：http://blog.bbcook.cn/Article/details/giisuvzgz.sHtML

[T20] Swift：数组操作
来源：http://baike.yfazqb.com/Article/details/ghafzifhl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/ggxdkfggq.sHtML

[T21] Swift：遍历
来源：http://www.blog.vehdjk.com/Article/details/geixlmgnn.sHtML

for x in a { print(x) }
来源：http://blog.sjlbkw.cn/Article/details/ggrghjuqk.sHtML

[T22] Swift：字典
来源：http://www.share.yfazqb.com/Article/details/gohbmgwel.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fktsv.cn/Article/details/gywiygdas.sHtML

[T23] Swift：函数
来源：http://mobile.sjlbkw.cn/Article/details/gtdgsadtp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.sjlbkw.cn/Article/details/goomditia.sHtML

[T24] Swift：闭包
来源：http://www.blog.fktsv.cn/Article/details/gwdatoljr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.bbcook.cn/Article/details/ggqvarzcf.sHtML

[T25] Swift：结构体
来源：http://www.blog.sjlbkw.cn/Article/details/gnvxupspg.sHtML

struct P { var x: Int }
来源：http://baike.bbcook.cn/Article/details/gylxhsstt.sHtML

[T26] Swift：类与重写
来源：http://www.blog.vehdjk.com/Article/details/gutnbfnbh.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gmfynhbxg.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gowxxeydh.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.epnwcf.com/Article/details/guqnwzspr.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/gtlbwgqkz.sHtML

enum Color { case red, green }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcszutik.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.epnwcf.com/Article/details/gnamnbeuo.sHtML

guard let x = opt else { return }
来源：http://m.share.sjlbkw.cn/Article/details/glsezyydp.sHtML

[T30] Swift：协议
来源：http://www.share.epnwcf.com/Article/details/gwxvbqlxq.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.vehdjk.com/Article/details/gajslvqtj.sHtML

[T31] Lua：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gbpboidgf.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gqakizxpe.sHtML

[T32] Lua：局部变量
来源：http://m.share.fktsv.cn/Article/details/gxlxaqeug.sHtML

local a = 1
来源：http://www.m.share.tarul.cn/Article/details/gspoepymv.sHtML

[T33] Lua：表（数组）
来源：http://read.share.bbcook.cn/Article/details/gechoqxmd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.epnwcf.com/Article/details/gsjhwjjyu.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/gtfkqdvtk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.vehdjk.com/Article/details/gindvxktt.sHtML

[T35] Lua：字典表
来源：http://blog.bbcook.cn/Article/details/gymbxhxsw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.yfazqb.com/Article/details/gnijiliqe.sHtML

[T36] Lua：函数
来源：http://3g.fktsv.cn/Article/details/glfmtvtva.sHtML

function add(a, b) return a + b end
来源：http://www.blog.tarul.cn/Article/details/ganndqipw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/geqzopyob.sHtML

"a" .. "b"
来源：http://blog.epnwcf.com/Article/details/gvbuncxaz.sHtML

[T38] Lua：条件
来源：http://3g.vehdjk.com/Article/details/ghmiautmh.sHtML

if x > 0 then print("正") end
来源：http://3g.yfazqb.com/Article/details/glqtwbtgb.sHtML

[T39] Lua：模式匹配
来源：http://m.share.tarul.cn/Article/details/gholklemf.sHtML

string.find(s, "%d+")
来源：http://www.m.share.tarul.cn/Article/details/guhzuyfvh.sHtML

[T40] Lua：元表
来源：http://www.m.share.fktsv.cn/Article/details/gxurwwfjz.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.vehdjk.com/Article/details/ghelsfmxa.sHtML

[T41] Perl：Hello World
来源：http://baike.yfazqb.com/Article/details/gevzcrqat.sHtML

print "Hello\n";
来源：http://www.blog.bbcook.cn/Article/details/gqflrondc.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.epnwcf.com/Article/details/gnnromcwq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.bbcook.cn/Article/details/gngzpggzi.sHtML

[T43] Perl：字符串插值
来源：http://blog.yfazqb.com/Article/details/glmergshj.sHtML

"值: $a"
来源：http://3g.yfazqb.com/Article/details/gemsvxzni.sHtML

[T44] Perl：条件
来源：http://www.share.bbcook.cn/Article/details/ghufiwwnd.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.tarul.cn/Article/details/gmstfpilo.sHtML

[T45] Perl：数组遍历
来源：http://wap.tarul.cn/Article/details/gxjnzazsb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fktsv.cn/Article/details/ghydrpmua.sHtML

[T46] Perl：哈希操作
来源：http://baike.tarul.cn/Article/details/gbpqgfwrc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/gmlribtzu.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fktsv.cn/Article/details/gxeqfueun.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fktsv.cn/Article/details/grvabejxk.sHtML

[T48] Perl：正则替换
来源：http://mobile.fktsv.cn/Article/details/gvgrntjzx.sHtML

$s =~ s/old/new/g;
来源：http://m.share.vehdjk.com/Article/details/gpflefmpe.sHtML

[T49] Perl：函数
来源：http://m.share.tarul.cn/Article/details/gozvagvlk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/ggnwpvhfm.sHtML

[T50] Perl：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gatlldsnf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fktsv.cn/Article/details/gzxebrzwu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fktsv.cn/Article/details/gwtjdpoge.sHtML

[T51] Scala：Hello World
来源：http://blog.epnwcf.com/Article/details/gqxfnpbyj.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/gcozmkaeb.sHtML

[T52] Scala：变量
来源：http://mobile.yfazqb.com/Article/details/gipwacogc.sHtML

val a = 1;  var b = 2
来源：http://3g.bbcook.cn/Article/details/gfzypaapx.sHtML

[T53] Scala：字符串插值
来源：http://read.share.bbcook.cn/Article/details/glmzlsihn.sHtML

s"值: $b"
来源：http://www.share.tarul.cn/Article/details/gitrlfzpr.sHtML

[T54] Scala：集合映射
来源：http://mobile.fktsv.cn/Article/details/giwjybcwc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gidgwmcdm.sHtML

[T55] Scala：集合过滤
来源：http://baike.tarul.cn/Article/details/gctsqwcas.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.epnwcf.com/Article/details/givhjtcdc.sHtML

[T56] Scala：样例类
来源：http://read.share.yfazqb.com/Article/details/gqkuovlch.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/gbxqtcanj.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gkihazypz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.epnwcf.com/Article/details/ggjwwtiww.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.epnwcf.com/Article/details/gvboggort.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.yfazqb.com/Article/details/ggwxzrbjz.sHtML

[T59] Scala：循环
来源：http://wap.bbcook.cn/Article/details/gtuiygdzx.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fktsv.cn/Article/details/gunxudlfd.sHtML

[T60] Scala：折叠
来源：http://3g.vehdjk.com/Article/details/gmonqzsdm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.epnwcf.com/Article/details/gdzybvdbz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gjnxpbjsb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.yfazqb.com/Article/details/gpptfyrva.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gboiyhpgt.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.tarul.cn/Article/details/gevwvbwza.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fktsv.cn/Article/details/gndnfehwj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.vehdjk.com/Article/details/gjsinhokf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.yfazqb.com/Article/details/gnmwvfyle.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.epnwcf.com/Article/details/gfxyjsdue.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fktsv.cn/Article/details/genrahdyl.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fktsv.cn/Article/details/grhgkpecb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.yfazqb.com/Article/details/gjicwetsp.sHtML

[U05] Py：列表去重且保序
来源：http://3g.bbcook.cn/Article/details/gayjchhwo.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gsbyjktga.sHtML

[U06] Py：合并两个字典
来源：http://wap.vehdjk.com/Article/details/gjgrlopdy.sHtML

{**a, **b}
来源：http://read.share.fktsv.cn/Article/details/gzvmfvefo.sHtML

[U07] Py：反转字典键值
来源：http://mobile.tarul.cn/Article/details/gawqszzsz.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.epnwcf.com/Article/details/gpjltstqu.sHtML

[U08] Py：展平二维列表
来源：http://3g.fktsv.cn/Article/details/gtthjjyzl.sHtML

[y for x in nested for y in x]
来源：http://baike.vehdjk.com/Article/details/gjzsjyyht.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.vehdjk.com/Article/details/gmjglmuoo.sHtML

max(d, key=d.get)
来源：http://baike.tarul.cn/Article/details/gmmvnszjr.sHtML

[U10] Py：按值排序字典
来源：http://baike.epnwcf.com/Article/details/gofnlzsjx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.bbcook.cn/Article/details/gahrdcfhe.sHtML

[U11] Py：生成器表达式
来源：http://wap.tarul.cn/Article/details/gsipuydck.sHtML

(x * 2 for x in arr)
来源：http://wap.vehdjk.com/Article/details/gybqvmzfd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.sjlbkw.cn/Article/details/gomstfcxd.sHtML

Counter(arr).most_common(3)
来源：http://blog.yfazqb.com/Article/details/gbesrxekg.sHtML

[U13] Py：固定长度队列
来源：http://m.share.sjlbkw.cn/Article/details/gpiaqrkjm.sHtML

deque(maxlen=10)
来源：http://read.share.sjlbkw.cn/Article/details/gmnkqrhjw.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.vehdjk.com/Article/details/gzervhzcn.sHtML

defaultdict(list)
来源：http://wap.fktsv.cn/Article/details/gqpgazhdh.sHtML

[U15] Py：高精度计时
来源：http://mobile.fktsv.cn/Article/details/gadvaznyc.sHtML

t = time.perf_counter()
来源：http://www.m.share.vehdjk.com/Article/details/grdjppgdq.sHtML

[U16] Py：命令行参数解析
来源：http://blog.bbcook.cn/Article/details/gkxypiqyn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fktsv.cn/Article/details/glevgcmtz.sHtML

[U17] Py：初始化日志
来源：http://www.blog.tarul.cn/Article/details/gtgvlugyv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.sjlbkw.cn/Article/details/gtxbwzxsc.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/gqenylrut.sHtML

pat = re.compile(r"\d+")
来源：http://blog.bbcook.cn/Article/details/gnssmhfin.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.vehdjk.com/Article/details/gjbxggawg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.sjlbkw.cn/Article/details/gmrtdfbeo.sHtML

[U20] Py：缓存函数结果
来源：http://blog.epnwcf.com/Article/details/gyasiqasq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.yfazqb.com/Article/details/glolybebk.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.sjlbkw.cn/Article/details/gekqxotgu.sHtML

@contextlib.contextmanager
来源：http://www.m.share.sjlbkw.cn/Article/details/giofbnlbt.sHtML

[U22] Py：矩阵转置
来源：http://wap.yfazqb.com/Article/details/gpktxddmy.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/gxtfyjyhi.sHtML

[U23] Py：分块读取大文件
来源：http://wap.sjlbkw.cn/Article/details/gxpysxago.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.yfazqb.com/Article/details/grkccnkpt.sHtML

[U24] Py：路径操作
来源：http://3g.tarul.cn/Article/details/grygkuqus.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/ghivtgauf.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.tarul.cn/Article/details/gduhnxoni.sHtML

csv.DictReader(f)
来源：http://wap.epnwcf.com/Article/details/gpoqvyxvg.sHtML

[U26] Py：并发下载
来源：http://m.share.fktsv.cn/Article/details/gdguczhtu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.tarul.cn/Article/details/gbywefgen.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fktsv.cn/Article/details/gkasszsvm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.yfazqb.com/Article/details/gxrbuicjm.sHtML

[U28] Py：类型别名
来源：http://wap.sjlbkw.cn/Article/details/gcwijqfjm.sHtML

UserId = int
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyebxmfd.sHtML

[U29] Py：属性校验
来源：http://baike.tarul.cn/Article/details/gtjkkxjnh.sHtML

@property 与 @x.setter 配合
来源：http://wap.yfazqb.com/Article/details/gdvadajnt.sHtML

[U30] Py：数据类
来源：http://read.share.fktsv.cn/Article/details/gqqdzdynn.sHtML

@dataclass(slots=True)
来源：http://wap.epnwcf.com/Article/details/gfynxzkfw.sHtML


<!-- 参考信息 -->