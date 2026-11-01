代发 wailian999

strlen(s)
来源：http://3g.fktsv.cn/Article/details/ghcowhcvs.sHtML

[S06] C：字符串比较
来源：http://read.share.tarul.cn/Article/details/gvlqvtegc.sHtML

strcmp(a, b) == 0
来源：http://www.share.yfazqb.com/Article/details/gntoqpblm.sHtML

[S07] C：数组遍历求和
来源：http://baike.tarul.cn/Article/details/giafkfzav.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.epnwcf.com/Article/details/grzfpnvwe.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.yfazqb.com/Article/details/gfpwdnyhh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.yfazqb.com/Article/details/gneeqhwgz.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/gjjcoeotp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fktsv.cn/Article/details/gfmhlhrax.sHtML

[S10] C：指针与解引用
来源：http://read.share.fktsv.cn/Article/details/ggwcseuvv.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.yfazqb.com/Article/details/grtpbmehy.sHtML

[S11] C：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gvgphzyzi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.yfazqb.com/Article/details/glfktxxuu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.tarul.cn/Article/details/gltmifkug.sHtML

fclose(f);
来源：http://3g.vehdjk.com/Article/details/gurkwejof.sHtML

[S12] C：写文件
来源：http://blog.sjlbkw.cn/Article/details/gstzshvrd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.vehdjk.com/Article/details/gjcjyurdq.sHtML

[S13] C：宏定义
来源：http://3g.epnwcf.com/Article/details/guiwgqwfv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fktsv.cn/Article/details/gdopbrhif.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/gqwalpsjj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.sjlbkw.cn/Article/details/gofgezwzn.sHtML

[S15] C：类型转换
来源：http://wap.vehdjk.com/Article/details/gltvqzljq.sHtML

(double) a / b
来源：http://read.share.bbcook.cn/Article/details/gfdvknpoe.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/gxcvryumo.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/gorbcefsa.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.tarul.cn/Article/details/gqgeacezt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.tarul.cn/Article/details/gabrslgpc.sHtML

[S18] C：命令行参数
来源：http://3g.tarul.cn/Article/details/gcidibvde.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gyvehkfnm.sHtML

[S19] C：快速排序
来源：http://m.share.tarul.cn/Article/details/gvekvkwsb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gehiwjewr.sHtML

[S20] C：二分查找
来源：http://mobile.epnwcf.com/Article/details/gkthdapsa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gjtbunewj.sHtML

[S21] C：字符类别判断
来源：http://wap.sjlbkw.cn/Article/details/gvyyoadng.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/giuldenpp.sHtML

[S22] C：字符串转数字
来源：http://3g.epnwcf.com/Article/details/gvedxxfcb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/gllhjskty.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/gbylvjlbi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fktsv.cn/Article/details/gjjtsdven.sHtML

[S24] C：获取本地时间
来源：http://3g.epnwcf.com/Article/details/gnciyrkvp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.vehdjk.com/Article/details/gwogrtedp.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/gkfmebczu.sHtML

memcpy(dst, src, n);
来源：http://wap.yfazqb.com/Article/details/geqmnxcdg.sHtML

[S26] C：内存清零
来源：http://read.share.fktsv.cn/Article/details/gkqxebjpm.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/gelcfrfmy.sHtML

[S27] C：定义常量
来源：http://m.share.yfazqb.com/Article/details/gzywqtnxx.sHtML

const double PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gyygscmrc.sHtML

[S28] C：静态变量
来源：http://www.share.epnwcf.com/Article/details/giyjokufi.sHtML

static int counter = 0;
来源：http://read.share.fktsv.cn/Article/details/gqcdtfoxj.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/gmqirgxat.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/gdsuadxed.sHtML

[S30] C：头文件保护
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyxhxlly.sHtML

#ifndef X_H
来源：http://m.share.tarul.cn/Article/details/gbokyqiyo.sHtML

#define X_H
来源：http://www.m.share.vehdjk.com/Article/details/goqbkqdqg.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gkcmdschw.sHtML

[S31] C++：Hello World
来源：http://3g.vehdjk.com/Article/details/gbkdvxsmt.sHtML

#include <iostream>
来源：http://wap.bbcook.cn/Article/details/gsigdnqea.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/gfzcyhlww.sHtML

[S32] C++：字符串
来源：http://www.share.fktsv.cn/Article/details/gtriziuzt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.bbcook.cn/Article/details/gnaqocyky.sHtML

[S33] C++：vector 增删
来源：http://m.share.tarul.cn/Article/details/gfadiybaz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gljytlpof.sHtML

[S34] C++：遍历 vector
来源：http://baike.fktsv.cn/Article/details/ghizyqfuh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.bbcook.cn/Article/details/gkyussjcb.sHtML

[S35] C++：map
来源：http://www.blog.tarul.cn/Article/details/gjyeedikc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gxsnlslvo.sHtML

[S36] C++：unordered_map
来源：http://m.share.tarul.cn/Article/details/gywrgvoam.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gnxkhvyog.sHtML

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/gvnkgqggs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.tarul.cn/Article/details/gdfqbyvuk.sHtML

[S38] C++：排序
来源：http://mobile.sjlbkw.cn/Article/details/gqunpsszg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.yfazqb.com/Article/details/gpgptvqmr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.vehdjk.com/Article/details/gdtnctjfp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/gmcwygdnq.sHtML

[S40] C++：查找元素
来源：http://3g.vehdjk.com/Article/details/gohorwleh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/gspbsgfwv.sHtML

[S41] C++：类与构造函数
来源：http://3g.yfazqb.com/Article/details/gxeafddqs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/girdckrmj.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fktsv.cn/Article/details/gszjnencq.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fktsv.cn/Article/details/gjpoffbno.sHtML

[S43] C++：智能指针
来源：http://m.share.sjlbkw.cn/Article/details/gpdzgsyla.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.bbcook.cn/Article/details/ghlwwlexc.sHtML

[S44] C++：引用传参
来源：http://read.share.epnwcf.com/Article/details/gbdojuodz.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.bbcook.cn/Article/details/gnweqwzst.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gftggmphi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.bbcook.cn/Article/details/gqjsbehdo.sHtML

[S46] C++：函数模板
来源：http://read.share.fktsv.cn/Article/details/gnsxptzke.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.tarul.cn/Article/details/gtxxjngjb.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.yfazqb.com/Article/details/glnqyygxh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fktsv.cn/Article/details/gstyxswsc.sHtML

[S48] C++：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gvqngifxz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.vehdjk.com/Article/details/gomuracrc.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fktsv.cn/Article/details/gfmnmfmfq.sHtML

[S49] C++：写文件
来源：http://wap.fktsv.cn/Article/details/gqtpogqlk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/gpicrcege.sHtML

[S50] C++：格式化数字
来源：http://baike.vehdjk.com/Article/details/gdbsxjgoz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gxrzzztpj.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/gdjkmrjhh.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/gtommvexv.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gcpuvxoew.sHtML

int size() const noexcept { return n_; }
来源：http://3g.vehdjk.com/Article/details/gvpglwaym.sHtML

[S53] C++：移动语义
来源：http://m.share.tarul.cn/Article/details/gchomjxhz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.epnwcf.com/Article/details/gxmnmqodh.sHtML

[S54] C++：异常处理
来源：http://mobile.sjlbkw.cn/Article/details/gxfmmvxgc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fktsv.cn/Article/details/ggbzpbqpj.sHtML

[S55] C++：结构化绑定
来源：http://mobile.sjlbkw.cn/Article/details/guvypmnjv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.yfazqb.com/Article/details/goglodnpd.sHtML

[S56] C++：optional
来源：http://baike.fktsv.cn/Article/details/gfelgdcur.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.epnwcf.com/Article/details/gmqgxgfrs.sHtML

[S57] C++：编译期常量
来源：http://3g.yfazqb.com/Article/details/gtltryvai.sHtML

constexpr int N = 10;
来源：http://baike.yfazqb.com/Article/details/gbpueszpy.sHtML

[S58] C++：命名空间
来源：http://www.share.sjlbkw.cn/Article/details/ghvfgzdbe.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.bbcook.cn/Article/details/gfgldwyjw.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/goomgfvks.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.yfazqb.com/Article/details/gczyqfdol.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.bbcook.cn/Article/details/gsafmsikj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/glepepufk.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwgkhugge.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gbtbedhtg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gplgudqlm.sHtML

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/gkesqfeph.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gwwlnxcxv.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.tarul.cn/Article/details/grzsbuyve.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.sjlbkw.cn/Article/details/gkdkybzzu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fktsv.cn/Article/details/guqtlzkng.sHtML

"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/gmxoffdsa.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fktsv.cn/Article/details/guqyypemn.sHtML

val n: String? = null;  n?.length
来源：http://blog.tarul.cn/Article/details/gxbwenihn.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.vehdjk.com/Article/details/gjbjujimp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.epnwcf.com/Article/details/guejsqaqt.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/glpnfxzdq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/gnoqnpszh.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.yfazqb.com/Article/details/gpwzkynrs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fktsv.cn/Article/details/gomgxqhsq.sHtML

[T08] Kotlin：数据类
来源：http://3g.yfazqb.com/Article/details/gsivqjkaj.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.tarul.cn/Article/details/gusxsfybe.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.vehdjk.com/Article/details/gyiyogtag.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.tarul.cn/Article/details/gztdewbsz.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.sjlbkw.cn/Article/details/gatffuzjj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjogagpf.sHtML

[T11] Kotlin：协程
来源：http://baike.epnwcf.com/Article/details/gxxrfgozn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.vehdjk.com/Article/details/gqvujjrhe.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.epnwcf.com/Article/details/gmrvgonte.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fktsv.cn/Article/details/goheigjkh.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.epnwcf.com/Article/details/gznpkccfl.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fktsv.cn/Article/details/garkwilzi.sHtML

[T14] Kotlin：循环
来源：http://read.share.epnwcf.com/Article/details/gojouillv.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gpmidgive.sHtML

[T15] Kotlin：接口
来源：http://mobile.epnwcf.com/Article/details/gfpcmptzl.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.epnwcf.com/Article/details/goclnjwcp.sHtML

[T16] Swift：Hello World
来源：http://www.blog.vehdjk.com/Article/details/ggkqkojvt.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gdxwcyylv.sHtML

[T17] Swift：变量与常量
来源：http://3g.sjlbkw.cn/Article/details/gcerbgwgt.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/gjejdtqqj.sHtML

[T18] Swift：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gelzmycaj.sHtML

"值: \(b)"
来源：http://www.blog.sjlbkw.cn/Article/details/gscospcdm.sHtML

[T19] Swift：可选绑定
来源：http://m.share.yfazqb.com/Article/details/gunzvsrar.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/gjveingsj.sHtML

[T20] Swift：数组操作
来源：http://mobile.vehdjk.com/Article/details/gdirranko.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.vehdjk.com/Article/details/gmdlerklp.sHtML

[T21] Swift：遍历
来源：http://blog.epnwcf.com/Article/details/gaadpaptz.sHtML

for x in a { print(x) }
来源：http://www.share.sjlbkw.cn/Article/details/gdojupolg.sHtML

[T22] Swift：字典
来源：http://baike.fktsv.cn/Article/details/gjprihmxp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.tarul.cn/Article/details/gclaicytv.sHtML

[T23] Swift：函数
来源：http://wap.vehdjk.com/Article/details/gvuxgjiaj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fktsv.cn/Article/details/gdmijxmbp.sHtML

[T24] Swift：闭包
来源：http://mobile.fktsv.cn/Article/details/gsdiczqpf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.bbcook.cn/Article/details/gtqgdodvz.sHtML

[T25] Swift：结构体
来源：http://www.m.share.yfazqb.com/Article/details/gxkjdxhcr.sHtML

struct P { var x: Int }
来源：http://mobile.vehdjk.com/Article/details/gaxnrwhax.sHtML

[T26] Swift：类与重写
来源：http://mobile.vehdjk.com/Article/details/gdlabpmcj.sHtML

class A: Base { override func f() {} }
来源：http://wap.epnwcf.com/Article/details/gufpirbys.sHtML

[T27] Swift：错误处理
来源：http://mobile.bbcook.cn/Article/details/gqmrlicrn.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.yfazqb.com/Article/details/ggjzomxyt.sHtML

[T28] Swift：枚举
来源：http://m.share.bbcook.cn/Article/details/gqqptxafi.sHtML

enum Color { case red, green }
来源：http://www.blog.sjlbkw.cn/Article/details/gbtdpyhmx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/gaoiatmsh.sHtML

guard let x = opt else { return }
来源：http://www.blog.vehdjk.com/Article/details/gtzwclxad.sHtML

[T30] Swift：协议
来源：http://3g.sjlbkw.cn/Article/details/gzfmsgkgo.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.tarul.cn/Article/details/goasjgbof.sHtML

[T31] Lua：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gnjtmpqlz.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/glrexbpbt.sHtML

[T32] Lua：局部变量
来源：http://wap.bbcook.cn/Article/details/grrkegoll.sHtML

local a = 1
来源：http://blog.bbcook.cn/Article/details/gnygzznky.sHtML

[T33] Lua：表（数组）
来源：http://wap.epnwcf.com/Article/details/gmudoxavq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.epnwcf.com/Article/details/gkpcoaktt.sHtML

[T34] Lua：遍历表
来源：http://blog.bbcook.cn/Article/details/gjnumkrjb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.tarul.cn/Article/details/gjgmavpvb.sHtML

[T35] Lua：字典表
来源：http://www.m.share.bbcook.cn/Article/details/gazlcfiyp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.sjlbkw.cn/Article/details/gamcvwisj.sHtML

[T36] Lua：函数
来源：http://www.blog.yfazqb.com/Article/details/gtruowkcn.sHtML

function add(a, b) return a + b end
来源：http://mobile.yfazqb.com/Article/details/gaqdxgpma.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fktsv.cn/Article/details/grnrbgogh.sHtML

"a" .. "b"
来源：http://www.m.share.fktsv.cn/Article/details/gucwapivx.sHtML

[T38] Lua：条件
来源：http://mobile.yfazqb.com/Article/details/gbavdnovu.sHtML

if x > 0 then print("正") end
来源：http://www.blog.bbcook.cn/Article/details/gypgncomj.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gvikverlj.sHtML

string.find(s, "%d+")
来源：http://wap.epnwcf.com/Article/details/gznpgbyok.sHtML

[T40] Lua：元表
来源：http://m.share.sjlbkw.cn/Article/details/giqifzuyj.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.yfazqb.com/Article/details/gtdelzxxk.sHtML

[T41] Perl：Hello World
来源：http://read.share.yfazqb.com/Article/details/gkzfnhoya.sHtML

print "Hello\n";
来源：http://mobile.bbcook.cn/Article/details/ganjwnrza.sHtML

[T42] Perl：变量类型
来源：http://mobile.tarul.cn/Article/details/gkinvensf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.sjlbkw.cn/Article/details/gvsiytjnp.sHtML

[T43] Perl：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gkmxxcire.sHtML

"值: $a"
来源：http://mobile.bbcook.cn/Article/details/gpntacqfq.sHtML

[T44] Perl：条件
来源：http://3g.fktsv.cn/Article/details/gfxflkxam.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.vehdjk.com/Article/details/gesisobmd.sHtML

[T45] Perl：数组遍历
来源：http://read.share.tarul.cn/Article/details/gbkkwvfpp.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.tarul.cn/Article/details/gyrhkfhtw.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.tarul.cn/Article/details/ghaqyuzbo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.tarul.cn/Article/details/gspryssfx.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fktsv.cn/Article/details/gaxzhjyeh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.bbcook.cn/Article/details/gwrbfufll.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/gfcjwobju.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgccvtlz.sHtML

[T49] Perl：函数
来源：http://mobile.vehdjk.com/Article/details/ghjjbgkui.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gvckaswyz.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gyjjnustn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.vehdjk.com/Article/details/gsjpsqfnu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.yfazqb.com/Article/details/gyvefcfpz.sHtML

[T51] Scala：Hello World
来源：http://blog.epnwcf.com/Article/details/gpospavoq.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/ghpfpybbf.sHtML

[T52] Scala：变量
来源：http://www.blog.vehdjk.com/Article/details/gkfubvxhl.sHtML

val a = 1;  var b = 2
来源：http://m.share.bbcook.cn/Article/details/gbnjvzvjd.sHtML

[T53] Scala：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gfsffstyt.sHtML

s"值: $b"
来源：http://3g.tarul.cn/Article/details/gcvzwfhcf.sHtML

[T54] Scala：集合映射
来源：http://blog.fktsv.cn/Article/details/gcdkkhjox.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gklsplmkr.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gnuzjfubm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.tarul.cn/Article/details/gfddqwcci.sHtML

[T56] Scala：样例类
来源：http://read.share.epnwcf.com/Article/details/gptuglupm.sHtML

case class User(name: String, age: Int)
来源：http://m.share.bbcook.cn/Article/details/gvygpnlqs.sHtML

[T57] Scala：模式匹配
来源：http://wap.epnwcf.com/Article/details/gqkumxdap.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fktsv.cn/Article/details/gvgrpplfq.sHtML

[T58] Scala：函数定义
来源：http://www.share.tarul.cn/Article/details/gzvibkgmo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.yfazqb.com/Article/details/gpgitbvpr.sHtML

[T59] Scala：循环
来源：http://blog.vehdjk.com/Article/details/gwnudngph.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/gnujooubh.sHtML

[T60] Scala：折叠
来源：http://www.blog.bbcook.cn/Article/details/gwamargpr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.epnwcf.com/Article/details/grpmkrbnq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gugbtoewx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/glqwrhwis.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gophjrweq.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.sjlbkw.cn/Article/details/goluffbku.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.vehdjk.com/Article/details/gbdrpsokv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.yfazqb.com/Article/details/ggrvzjhqn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gspzoionp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.bbcook.cn/Article/details/gasjwixvv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.yfazqb.com/Article/details/gjcrblntz.sHtML

[U04] Py：变量调试打印
来源：http://mobile.yfazqb.com/Article/details/gnzzowwvt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fktsv.cn/Article/details/gfaiqqynp.sHtML

[U05] Py：列表去重且保序
来源：http://3g.sjlbkw.cn/Article/details/gjmykkvtt.sHtML

list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gwtorxymq.sHtML

[U06] Py：合并两个字典
来源：http://blog.tarul.cn/Article/details/gyiggzgmk.sHtML

{**a, **b}
来源：http://baike.sjlbkw.cn/Article/details/gaxwzvlgw.sHtML

[U07] Py：反转字典键值
来源：http://blog.tarul.cn/Article/details/gswbgvrkk.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.tarul.cn/Article/details/gjeqtfugy.sHtML

[U08] Py：展平二维列表
来源：http://read.share.yfazqb.com/Article/details/ggesterjf.sHtML

[y for x in nested for y in x]
来源：http://www.blog.bbcook.cn/Article/details/gjxiymqia.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.tarul.cn/Article/details/gzinsjjhp.sHtML

max(d, key=d.get)
来源：http://www.blog.epnwcf.com/Article/details/gwfqvdzaf.sHtML

[U10] Py：按值排序字典
来源：http://m.share.yfazqb.com/Article/details/ggqkvavtl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.bbcook.cn/Article/details/genjrxgqz.sHtML

[U11] Py：生成器表达式
来源：http://read.share.sjlbkw.cn/Article/details/gvlmdgihe.sHtML

(x * 2 for x in arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gtfzjzgew.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.yfazqb.com/Article/details/grtnzbmaf.sHtML

Counter(arr).most_common(3)
来源：http://read.share.yfazqb.com/Article/details/ghmrxddje.sHtML

[U13] Py：固定长度队列
来源：http://www.share.tarul.cn/Article/details/gsbbhtxqk.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/gndyxilgt.sHtML

[U14] Py：分组收集到列表
来源：http://wap.yfazqb.com/Article/details/gswnimzgl.sHtML

defaultdict(list)
来源：http://mobile.yfazqb.com/Article/details/gjsxkuniv.sHtML

[U15] Py：高精度计时
来源：http://blog.epnwcf.com/Article/details/glrxtbqsa.sHtML

t = time.perf_counter()
来源：http://blog.sjlbkw.cn/Article/details/gvfwvpiuk.sHtML

[U16] Py：命令行参数解析
来源：http://3g.epnwcf.com/Article/details/gusagnlce.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.bbcook.cn/Article/details/gqaasonxv.sHtML

[U17] Py：初始化日志
来源：http://baike.yfazqb.com/Article/details/gikzryblm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.tarul.cn/Article/details/gckzsybvo.sHtML

[U18] Py：预编译正则
来源：http://www.share.sjlbkw.cn/Article/details/gintnjmbb.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fktsv.cn/Article/details/gbkzdktmt.sHtML

[U19] Py：正则替换带回调
来源：http://blog.epnwcf.com/Article/details/gqxosrztp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.vehdjk.com/Article/details/gglkyesnl.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.epnwcf.com/Article/details/gfwfwcscl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.sjlbkw.cn/Article/details/gocqtjvnj.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.tarul.cn/Article/details/gdinohsez.sHtML

@contextlib.contextmanager
来源：http://wap.tarul.cn/Article/details/gousyrhwg.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fktsv.cn/Article/details/gypsajkps.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/glucrnabg.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.vehdjk.com/Article/details/gxdhkddav.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.epnwcf.com/Article/details/ghvyjkhwu.sHtML

[U24] Py：路径操作
来源：http://wap.tarul.cn/Article/details/gxhagtifh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.yfazqb.com/Article/details/gjmueazsd.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.vehdjk.com/Article/details/gwrsgftwg.sHtML

csv.DictReader(f)
来源：http://baike.yfazqb.com/Article/details/gsljrgeqq.sHtML

[U26] Py：并发下载
来源：http://www.share.fktsv.cn/Article/details/gbpaaopqn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.bbcook.cn/Article/details/gaofaxzlf.sHtML

[U27] Py：异步 HTTP
来源：http://baike.epnwcf.com/Article/details/gkenipfer.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.bbcook.cn/Article/details/glgmlkksp.sHtML

[U28] Py：类型别名
来源：http://m.share.bbcook.cn/Article/details/gzcxetpxl.sHtML

UserId = int
来源：http://blog.yfazqb.com/Article/details/grxnrfyfw.sHtML


<!-- 参考信息 -->