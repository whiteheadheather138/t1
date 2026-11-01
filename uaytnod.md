代发 wailian999

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/gtgcaxogh.sHtML

[S04] C：字符串复制
来源：http://read.share.vehdjk.com/Article/details/gxmrqbqrc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gxguqecnq.sHtML

[S05] C：字符串长度
来源：http://3g.bbcook.cn/Article/details/genncljss.sHtML

strlen(s)
来源：http://read.share.bbcook.cn/Article/details/geeufyykf.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/gtjqqoqgc.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gggagkxkw.sHtML

[S07] C：数组遍历求和
来源：http://read.share.epnwcf.com/Article/details/gulcxfotn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fktsv.cn/Article/details/gogbeaebw.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.tarul.cn/Article/details/gpqvhbqdv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.bbcook.cn/Article/details/gyyhumdcs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fktsv.cn/Article/details/grddszadk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fktsv.cn/Article/details/gazareimj.sHtML

[S10] C：指针与解引用
来源：http://read.share.tarul.cn/Article/details/gzlxkufjt.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.vehdjk.com/Article/details/gfnwdyahd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gewyjuabo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.epnwcf.com/Article/details/goqjjdcax.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fktsv.cn/Article/details/gberfrutz.sHtML

fclose(f);
来源：http://baike.vehdjk.com/Article/details/gzqbppotp.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/gohhfuadc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.tarul.cn/Article/details/girwhoyee.sHtML

[S13] C：宏定义
来源：http://m.share.vehdjk.com/Article/details/gkaokvybg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.yfazqb.com/Article/details/gscwcskhh.sHtML

[S14] C：枚举
来源：http://baike.sjlbkw.cn/Article/details/grtrqeril.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.sjlbkw.cn/Article/details/gkvvmlygs.sHtML

[S15] C：类型转换
来源：http://read.share.yfazqb.com/Article/details/gayzhemaw.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/gkwvvxftd.sHtML

[S16] C：位操作置位
来源：http://www.share.epnwcf.com/Article/details/gcxzasmik.sHtML

x |= (1 << 3);
来源：http://mobile.epnwcf.com/Article/details/gvclddvim.sHtML

[S17] C：安全拼接字符串
来源：http://baike.epnwcf.com/Article/details/ggyunvlvo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.epnwcf.com/Article/details/gdobqsadu.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/geidjjksv.sHtML

int main(int argc, char **argv)
来源：http://3g.bbcook.cn/Article/details/gjqshcwon.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/gfmkcirpe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gjhzpmupl.sHtML

[S20] C：二分查找
来源：http://mobile.fktsv.cn/Article/details/gdqqhokwf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gdxkaqixq.sHtML

[S21] C：字符类别判断
来源：http://mobile.tarul.cn/Article/details/ggwwqfagi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.tarul.cn/Article/details/glqxrntxw.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/gcxjidsju.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.tarul.cn/Article/details/gfdktdyrq.sHtML

[S23] C：随机数
来源：http://baike.vehdjk.com/Article/details/gmgcipevx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/gwjcmnwko.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.vehdjk.com/Article/details/gevdvwnek.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.tarul.cn/Article/details/gxsythbsu.sHtML

[S25] C：内存拷贝
来源：http://read.share.tarul.cn/Article/details/gleqqokuu.sHtML

memcpy(dst, src, n);
来源：http://read.share.vehdjk.com/Article/details/gotirfbag.sHtML

[S26] C：内存清零
来源：http://mobile.yfazqb.com/Article/details/gcyupsspk.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.vehdjk.com/Article/details/gnsrkmipk.sHtML

[S27] C：定义常量
来源：http://www.share.yfazqb.com/Article/details/gzkmjcdjo.sHtML

const double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gobkfchxl.sHtML

[S28] C：静态变量
来源：http://mobile.yfazqb.com/Article/details/groaawjti.sHtML

static int counter = 0;
来源：http://read.share.yfazqb.com/Article/details/gxgjsuavj.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/gjdncxwfd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.sjlbkw.cn/Article/details/gexwpouur.sHtML

[S30] C：头文件保护
来源：http://www.blog.sjlbkw.cn/Article/details/gynyvqmvo.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/gzyjwtpau.sHtML

#define X_H
来源：http://blog.sjlbkw.cn/Article/details/gktchicly.sHtML

#endif
来源：http://www.share.sjlbkw.cn/Article/details/gxlwoschl.sHtML

[S31] C++：Hello World
来源：http://blog.bbcook.cn/Article/details/gefqdsmes.sHtML

#include <iostream>
来源：http://m.share.fktsv.cn/Article/details/gaylfbhif.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.bbcook.cn/Article/details/gqxdfzvkf.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/guxtckrev.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.vehdjk.com/Article/details/gfsuqghjn.sHtML

[S33] C++：vector 增删
来源：http://m.share.fktsv.cn/Article/details/gwbdlezgw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gxmrmhuzt.sHtML

[S34] C++：遍历 vector
来源：http://read.share.bbcook.cn/Article/details/ghepjvnju.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.tarul.cn/Article/details/gxkxiwjpz.sHtML

[S35] C++：map
来源：http://m.share.yfazqb.com/Article/details/goghqwgdb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gbejcymyg.sHtML

[S36] C++：unordered_map
来源：http://3g.epnwcf.com/Article/details/gxgvgkpsy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/gvdeulodx.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/gzgxtfayr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/gqroferkw.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/gsykbroex.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.bbcook.cn/Article/details/gorisljoe.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/gwxaxithv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.yfazqb.com/Article/details/gghzndzth.sHtML

[S40] C++：查找元素
来源：http://wap.fktsv.cn/Article/details/gjawgdyav.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fktsv.cn/Article/details/gnyohcsiv.sHtML

[S41] C++：类与构造函数
来源：http://baike.vehdjk.com/Article/details/getybgxbw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fktsv.cn/Article/details/gcrucqmxv.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fktsv.cn/Article/details/gxzakbmfh.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/gwfjlgjuw.sHtML

[S43] C++：智能指针
来源：http://blog.epnwcf.com/Article/details/gkxmdbppr.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fktsv.cn/Article/details/gejcygrid.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gkbmqwfen.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/grzyugcdo.sHtML

[S45] C++：lambda
来源：http://3g.bbcook.cn/Article/details/gxdzkhurz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fktsv.cn/Article/details/gtvlhpwbu.sHtML

[S46] C++：函数模板
来源：http://3g.vehdjk.com/Article/details/gzhdhtiqn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.yfazqb.com/Article/details/gbotebmqt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.tarul.cn/Article/details/ghfehmqyk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/ghwrdwbev.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gagcaxvrj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.vehdjk.com/Article/details/gkvrqtqfs.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.tarul.cn/Article/details/gynhboeui.sHtML

[S49] C++：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gsmjhudzg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.bbcook.cn/Article/details/gidbekisf.sHtML

[S50] C++：格式化数字
来源：http://wap.fktsv.cn/Article/details/grcewokqx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.tarul.cn/Article/details/gxhezitmt.sHtML

[S51] C++：显式类型转换
来源：http://read.share.bbcook.cn/Article/details/gajhixldc.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gmzxbkgtq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.sjlbkw.cn/Article/details/gdmynerhc.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.tarul.cn/Article/details/gcxjxyfdc.sHtML

[S53] C++：移动语义
来源：http://m.share.tarul.cn/Article/details/gkuzajfzs.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gndrcialo.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/gtuoblaub.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.tarul.cn/Article/details/gvlbplmdd.sHtML

[S55] C++：结构化绑定
来源：http://read.share.tarul.cn/Article/details/gnkzhpryc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.epnwcf.com/Article/details/gqhfdajgb.sHtML

[S56] C++：optional
来源：http://www.share.tarul.cn/Article/details/gzaxhkuir.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.epnwcf.com/Article/details/gasocnytv.sHtML

[S57] C++：编译期常量
来源：http://wap.tarul.cn/Article/details/giobogdey.sHtML

constexpr int N = 10;
来源：http://www.share.yfazqb.com/Article/details/gjdkrlwab.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/gczkfswjt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.bbcook.cn/Article/details/gadvoxiko.sHtML

[S59] C++：静态断言
来源：http://wap.fktsv.cn/Article/details/grivttlak.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fktsv.cn/Article/details/gtzvrndvk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.yfazqb.com/Article/details/gfwxnhluf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.tarul.cn/Article/details/gjfhxqjht.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/golbzolak.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.epnwcf.com/Article/details/geckylprh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtkqceqfb.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.vehdjk.com/Article/details/geewdcuvt.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/gljembvue.sHtML

[T02] Kotlin：变量
来源：http://www.blog.tarul.cn/Article/details/gqrgzpsku.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/ggzeltpwq.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.bbcook.cn/Article/details/gppxlrzrj.sHtML

"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/godavnopx.sHtML

[T04] Kotlin：空安全
来源：http://mobile.bbcook.cn/Article/details/gacsrwmus.sHtML

val n: String? = null;  n?.length
来源：http://read.share.tarul.cn/Article/details/gbpfiflgv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gygrjkryv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.sjlbkw.cn/Article/details/gbkcnquno.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.epnwcf.com/Article/details/ggdtwftle.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gqoyxahyt.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.vehdjk.com/Article/details/gweiwrcel.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.tarul.cn/Article/details/ghgsgmeok.sHtML

[T08] Kotlin：数据类
来源：http://m.share.yfazqb.com/Article/details/ggscaatow.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/gplawubjt.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.vehdjk.com/Article/details/grcfldgnc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.bbcook.cn/Article/details/grkkfiqsk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.tarul.cn/Article/details/gqsjvetin.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.sjlbkw.cn/Article/details/giifripug.sHtML

[T11] Kotlin：协程
来源：http://www.blog.vehdjk.com/Article/details/ggtxrrquw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.epnwcf.com/Article/details/glgladxze.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.epnwcf.com/Article/details/gmnoabbnz.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.tarul.cn/Article/details/gamtsnimb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.epnwcf.com/Article/details/gjfgvihla.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.vehdjk.com/Article/details/gtymculug.sHtML

[T14] Kotlin：循环
来源：http://mobile.tarul.cn/Article/details/gzbfaojxc.sHtML

for (i in 1..10) println(i)
来源：http://m.share.yfazqb.com/Article/details/gvqmtqvxv.sHtML

[T15] Kotlin：接口
来源：http://wap.tarul.cn/Article/details/ggqnqngab.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fktsv.cn/Article/details/gvimhpmzg.sHtML

[T16] Swift：Hello World
来源：http://m.share.vehdjk.com/Article/details/gzzmvtips.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/ghxvpfqvy.sHtML

[T17] Swift：变量与常量
来源：http://www.share.bbcook.cn/Article/details/gnxglfsdm.sHtML

var a = 1;  let b = 2
来源：http://www.share.fktsv.cn/Article/details/gurthnfhv.sHtML

[T18] Swift：字符串插值
来源：http://3g.epnwcf.com/Article/details/grsqqjula.sHtML

"值: \(b)"
来源：http://read.share.fktsv.cn/Article/details/gnkoeqvka.sHtML

[T19] Swift：可选绑定
来源：http://wap.epnwcf.com/Article/details/gwwrbttmm.sHtML

if let n = opt { print(n) }
来源：http://www.share.yfazqb.com/Article/details/grchporzx.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/ggeoyxrfd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.bbcook.cn/Article/details/geawcnmxo.sHtML

[T21] Swift：遍历
来源：http://baike.tarul.cn/Article/details/glvflaovp.sHtML

for x in a { print(x) }
来源：http://blog.fktsv.cn/Article/details/goacqfgis.sHtML

[T22] Swift：字典
来源：http://blog.epnwcf.com/Article/details/gydqgipgn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.sjlbkw.cn/Article/details/gipsqipky.sHtML

[T23] Swift：函数
来源：http://m.share.bbcook.cn/Article/details/gwpvgzgao.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/gjbntpwft.sHtML

[T24] Swift：闭包
来源：http://baike.sjlbkw.cn/Article/details/gzxpeaurs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.tarul.cn/Article/details/gzpnlmlvi.sHtML

[T25] Swift：结构体
来源：http://read.share.epnwcf.com/Article/details/gjsulyfxb.sHtML

struct P { var x: Int }
来源：http://wap.bbcook.cn/Article/details/goxegbmsv.sHtML

[T26] Swift：类与重写
来源：http://www.share.tarul.cn/Article/details/gqlutgoru.sHtML

class A: Base { override func f() {} }
来源：http://blog.sjlbkw.cn/Article/details/gtrlafkbq.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/ggeuazjvk.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.tarul.cn/Article/details/gqfcddwgs.sHtML

[T28] Swift：枚举
来源：http://wap.bbcook.cn/Article/details/gnwujsydu.sHtML

enum Color { case red, green }
来源：http://mobile.sjlbkw.cn/Article/details/gehkjmphg.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.yfazqb.com/Article/details/gwabjhlfi.sHtML

guard let x = opt else { return }
来源：http://m.share.fktsv.cn/Article/details/ghcbrfwvn.sHtML

[T30] Swift：协议
来源：http://www.m.share.yfazqb.com/Article/details/gmzcqafrm.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.tarul.cn/Article/details/gfnofsnxn.sHtML

[T31] Lua：Hello World
来源：http://wap.vehdjk.com/Article/details/ghsikhxyh.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/guatkauxt.sHtML

[T32] Lua：局部变量
来源：http://m.share.vehdjk.com/Article/details/gxbsibnhl.sHtML

local a = 1
来源：http://www.share.vehdjk.com/Article/details/gszcmstld.sHtML

[T33] Lua：表（数组）
来源：http://wap.yfazqb.com/Article/details/gtivevbkb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.epnwcf.com/Article/details/grnypvujk.sHtML

[T34] Lua：遍历表
来源：http://m.share.vehdjk.com/Article/details/gwiubinnc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/gnlqgkcbn.sHtML

[T35] Lua：字典表
来源：http://mobile.sjlbkw.cn/Article/details/gqqcayrru.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.epnwcf.com/Article/details/ghdmnpukx.sHtML

[T36] Lua：函数
来源：http://wap.vehdjk.com/Article/details/ggsdrrzao.sHtML

function add(a, b) return a + b end
来源：http://mobile.yfazqb.com/Article/details/gjktbddzt.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gimefbqyn.sHtML

"a" .. "b"
来源：http://wap.fktsv.cn/Article/details/gkzcpmoia.sHtML

[T38] Lua：条件
来源：http://3g.fktsv.cn/Article/details/gqgzyajuv.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/gxtfpyrie.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gdyxaveek.sHtML

string.find(s, "%d+")
来源：http://mobile.sjlbkw.cn/Article/details/gvwlgfnwf.sHtML

[T40] Lua：元表
来源：http://baike.fktsv.cn/Article/details/gcwtngckw.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fktsv.cn/Article/details/gompbljhq.sHtML

[T41] Perl：Hello World
来源：http://3g.vehdjk.com/Article/details/gxtcdquea.sHtML

print "Hello\n";
来源：http://wap.vehdjk.com/Article/details/gprkixooy.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.yfazqb.com/Article/details/gbzsismxf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.tarul.cn/Article/details/gsysjerqk.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gdpybbmjp.sHtML

"值: $a"
来源：http://www.share.epnwcf.com/Article/details/gpoacojvt.sHtML

[T44] Perl：条件
来源：http://www.blog.bbcook.cn/Article/details/gtqxsxkru.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.vehdjk.com/Article/details/gywvppkev.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fktsv.cn/Article/details/gltemhvob.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.bbcook.cn/Article/details/gcpqbqqlb.sHtML

[T46] Perl：哈希操作
来源：http://3g.fktsv.cn/Article/details/gvcclcepd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.yfazqb.com/Article/details/gphztmqfo.sHtML

[T47] Perl：正则捕获
来源：http://blog.tarul.cn/Article/details/gmzpxxexv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.vehdjk.com/Article/details/grgvorywp.sHtML

[T48] Perl：正则替换
来源：http://baike.vehdjk.com/Article/details/gkhplnrvt.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fktsv.cn/Article/details/gvqsatusm.sHtML

[T49] Perl：函数
来源：http://www.m.share.fktsv.cn/Article/details/gadjxsdnv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gqsubedxu.sHtML

[T50] Perl：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gbryzpldd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.yfazqb.com/Article/details/gsyjsnvvl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.sjlbkw.cn/Article/details/ggucrvgib.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/geppafhjv.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gbqyswvxh.sHtML

[T52] Scala：变量
来源：http://m.share.fktsv.cn/Article/details/gdmivlrcv.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fktsv.cn/Article/details/gmzmbzwry.sHtML

[T53] Scala：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/ginooeebg.sHtML

s"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gvkmtvnif.sHtML

[T54] Scala：集合映射
来源：http://mobile.yfazqb.com/Article/details/gxnomnjfy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.yfazqb.com/Article/details/gisttsmik.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gcbudczmr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.bbcook.cn/Article/details/gqerufmso.sHtML

[T56] Scala：样例类
来源：http://www.m.share.yfazqb.com/Article/details/gwbwavwel.sHtML

case class User(name: String, age: Int)
来源：http://3g.epnwcf.com/Article/details/ghpoaewik.sHtML

[T57] Scala：模式匹配
来源：http://read.share.sjlbkw.cn/Article/details/gqiqccdne.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.tarul.cn/Article/details/gcqokiezt.sHtML

[T58] Scala：函数定义
来源：http://3g.yfazqb.com/Article/details/gouyycypj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.tarul.cn/Article/details/grraihups.sHtML

[T59] Scala：循环
来源：http://www.share.sjlbkw.cn/Article/details/gsfwuhqdq.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gbncamnbt.sHtML

[T60] Scala：折叠
来源：http://www.m.share.tarul.cn/Article/details/gfxuvjiyy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.epnwcf.com/Article/details/goterfxly.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gsnyntcoe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.yfazqb.com/Article/details/ghpxzuonf.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gopzfkzkn.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.yfazqb.com/Article/details/gbxgrcqqq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.bbcook.cn/Article/details/gdqvnylxb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fktsv.cn/Article/details/gtnecqlsz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.epnwcf.com/Article/details/gujgpcjez.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fktsv.cn/Article/details/gnzhqyfrz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fktsv.cn/Article/details/gtgbyhlov.sHtML

[U04] Py：变量调试打印
来源：http://mobile.bbcook.cn/Article/details/gjimvqbyy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.tarul.cn/Article/details/gcmvdbaiz.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.vehdjk.com/Article/details/gwznqnxfx.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gvqotqugd.sHtML

[U06] Py：合并两个字典
来源：http://mobile.vehdjk.com/Article/details/gjhzlrgvx.sHtML

{**a, **b}
来源：http://m.share.epnwcf.com/Article/details/ghzqiibhf.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.yfazqb.com/Article/details/gdxefxstk.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.yfazqb.com/Article/details/gupvtswiu.sHtML

[U08] Py：展平二维列表
来源：http://read.share.epnwcf.com/Article/details/gocwpzisa.sHtML

[y for x in nested for y in x]
来源：http://read.share.vehdjk.com/Article/details/guaedvfzj.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.yfazqb.com/Article/details/gztaybnbm.sHtML

max(d, key=d.get)
来源：http://www.share.fktsv.cn/Article/details/ggiygczzm.sHtML

[U10] Py：按值排序字典
来源：http://read.share.epnwcf.com/Article/details/grdgyaoxc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.sjlbkw.cn/Article/details/gkiexnilu.sHtML

[U11] Py：生成器表达式
来源：http://blog.bbcook.cn/Article/details/ggstjzldt.sHtML

(x * 2 for x in arr)
来源：http://baike.fktsv.cn/Article/details/gmfmoncrw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.tarul.cn/Article/details/gnzpfhzdl.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fktsv.cn/Article/details/gcdlapzkh.sHtML

[U13] Py：固定长度队列
来源：http://baike.yfazqb.com/Article/details/gyvumizmo.sHtML

deque(maxlen=10)
来源：http://www.blog.bbcook.cn/Article/details/glictqwnl.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.epnwcf.com/Article/details/grxzfutnr.sHtML

defaultdict(list)
来源：http://baike.vehdjk.com/Article/details/ghnugjqtm.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fktsv.cn/Article/details/gabcfyeag.sHtML

t = time.perf_counter()
来源：http://www.m.share.bbcook.cn/Article/details/ggwbbzmao.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.yfazqb.com/Article/details/gypiibbie.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.tarul.cn/Article/details/gxnyxwpde.sHtML

[U17] Py：初始化日志
来源：http://wap.bbcook.cn/Article/details/gjungebun.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.sjlbkw.cn/Article/details/gbazhhurd.sHtML

[U18] Py：预编译正则
来源：http://www.share.vehdjk.com/Article/details/gjmftlmen.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/ggzdolqnp.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.epnwcf.com/Article/details/glujgervl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.vehdjk.com/Article/details/gsryukzfx.sHtML

[U20] Py：缓存函数结果
来源：http://3g.vehdjk.com/Article/details/gehdzscpz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.tarul.cn/Article/details/gfusydiof.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.tarul.cn/Article/details/gamxjbmfu.sHtML

@contextlib.contextmanager
来源：http://read.share.bbcook.cn/Article/details/gffmwhhci.sHtML

[U22] Py：矩阵转置
来源：http://baike.bbcook.cn/Article/details/gqqkboryd.sHtML

list(zip(*m))
来源：http://www.blog.epnwcf.com/Article/details/gncjrjuhy.sHtML

[U23] Py：分块读取大文件
来源：http://wap.tarul.cn/Article/details/gahjcvpin.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.vehdjk.com/Article/details/glhiwetps.sHtML

[U24] Py：路径操作
来源：http://blog.epnwcf.com/Article/details/gduqqlmfz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/ghjfzqboh.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.sjlbkw.cn/Article/details/gagouxtee.sHtML

csv.DictReader(f)
来源：http://www.m.share.fktsv.cn/Article/details/gnrzckypx.sHtML

[U26] Py：并发下载
来源：http://mobile.vehdjk.com/Article/details/gzkyhsodk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.vehdjk.com/Article/details/gqmpyhscm.sHtML


<!-- 参考信息 -->