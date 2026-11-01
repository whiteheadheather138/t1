代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/gsdqqdguc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gmlazkomn.sHtML

fclose(f);
来源：http://3g.tarul.cn/Article/details/gvpvgxfyw.sHtML

[S12] C：写文件
来源：http://3g.sjlbkw.cn/Article/details/gszzztloh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gspvpcnhy.sHtML

[S13] C：宏定义
来源：http://www.blog.sjlbkw.cn/Article/details/govpdqxcg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gpcluzqlr.sHtML

[S14] C：枚举
来源：http://baike.fktsv.cn/Article/details/grtarqedn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.sjlbkw.cn/Article/details/gvhkhocmr.sHtML

[S15] C：类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gdcmprtja.sHtML

(double) a / b
来源：http://www.share.tarul.cn/Article/details/gbfqqesnj.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/gsriwytlg.sHtML

x |= (1 << 3);
来源：http://www.m.share.epnwcf.com/Article/details/govvytyiz.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gadopkmpk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.vehdjk.com/Article/details/gjwbqmult.sHtML

[S18] C：命令行参数
来源：http://baike.fktsv.cn/Article/details/grdbdjwsq.sHtML

int main(int argc, char **argv)
来源：http://mobile.fktsv.cn/Article/details/giugexxie.sHtML

[S19] C：快速排序
来源：http://baike.fktsv.cn/Article/details/gbrbliceg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/ggmncdeqz.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gapxufqhm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gxsbqutot.sHtML

[S21] C：字符类别判断
来源：http://3g.vehdjk.com/Article/details/gixyylxql.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjexjpvms.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fktsv.cn/Article/details/gqaesgryk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.vehdjk.com/Article/details/gezkgivbx.sHtML

[S23] C：随机数
来源：http://blog.fktsv.cn/Article/details/glzuimnot.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fktsv.cn/Article/details/gvhvgkupa.sHtML

[S24] C：获取本地时间
来源：http://wap.sjlbkw.cn/Article/details/gvynwswou.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/grcykhoru.sHtML

[S25] C：内存拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gbcfjzddf.sHtML

memcpy(dst, src, n);
来源：http://wap.yfazqb.com/Article/details/gpteudmxl.sHtML

[S26] C：内存清零
来源：http://www.share.yfazqb.com/Article/details/gtaairtwm.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.bbcook.cn/Article/details/gadjznmya.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/gxmhpnekx.sHtML

const double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/geijufell.sHtML

[S28] C：静态变量
来源：http://www.blog.bbcook.cn/Article/details/gxvggbbzt.sHtML

static int counter = 0;
来源：http://3g.sjlbkw.cn/Article/details/gpwmguwxc.sHtML

[S29] C：变参函数
来源：http://read.share.vehdjk.com/Article/details/gjzpsxrxf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.yfazqb.com/Article/details/giqvwypcv.sHtML

[S30] C：头文件保护
来源：http://3g.epnwcf.com/Article/details/gmkohhvvi.sHtML

#ifndef X_H
来源：http://wap.yfazqb.com/Article/details/glwvhjdtp.sHtML

#define X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzzyfqwg.sHtML

#endif
来源：http://baike.fktsv.cn/Article/details/gtaqoamvs.sHtML

[S31] C++：Hello World
来源：http://mobile.yfazqb.com/Article/details/gcoxgiboo.sHtML

#include <iostream>
来源：http://3g.bbcook.cn/Article/details/gwpmccwcu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.epnwcf.com/Article/details/gqlplizyn.sHtML

[S32] C++：字符串
来源：http://www.share.epnwcf.com/Article/details/gxfcnzzwo.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/gtetgutsl.sHtML

[S33] C++：vector 增删
来源：http://www.blog.sjlbkw.cn/Article/details/gsgmrckpw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.yfazqb.com/Article/details/gsyjggifp.sHtML

[S34] C++：遍历 vector
来源：http://read.share.vehdjk.com/Article/details/gwpquzztn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.vehdjk.com/Article/details/gxehhabfp.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gelzlewib.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gprwncvne.sHtML

[S36] C++：unordered_map
来源：http://wap.epnwcf.com/Article/details/gfjxnjnxq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/grlysjmbe.sHtML

[S37] C++：set
来源：http://baike.sjlbkw.cn/Article/details/glgtyorte.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.yfazqb.com/Article/details/grrbhfivy.sHtML

[S38] C++：排序
来源：http://www.m.share.bbcook.cn/Article/details/gsfpqtplx.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.tarul.cn/Article/details/gvuuridrq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.sjlbkw.cn/Article/details/gepnfydxt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.epnwcf.com/Article/details/gxgaggprx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fktsv.cn/Article/details/greffdlzy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.vehdjk.com/Article/details/gvzwqhhmu.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gkbcmxuoz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.tarul.cn/Article/details/gtsmhhdux.sHtML

[S42] C++：继承与虚函数
来源：http://baike.epnwcf.com/Article/details/ganqguxbh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.epnwcf.com/Article/details/gejwlxajj.sHtML

[S43] C++：智能指针
来源：http://www.m.share.yfazqb.com/Article/details/ghvqtyrfi.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.tarul.cn/Article/details/glnwqgtme.sHtML

[S44] C++：引用传参
来源：http://read.share.epnwcf.com/Article/details/gswwpjqpe.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.tarul.cn/Article/details/gjbkogwle.sHtML

[S45] C++：lambda
来源：http://baike.vehdjk.com/Article/details/gqqlglypg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/gtbtgfaxm.sHtML

[S46] C++：函数模板
来源：http://3g.fktsv.cn/Article/details/gyvyjlnyj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.epnwcf.com/Article/details/ghxmnuolh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/gcjtelpnr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.tarul.cn/Article/details/guxevhzam.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/grvdtzwrb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.epnwcf.com/Article/details/giymxekkw.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.epnwcf.com/Article/details/guinbmdnr.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/geiuytcps.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.yfazqb.com/Article/details/gmsjlfglb.sHtML

[S50] C++：格式化数字
来源：http://www.share.fktsv.cn/Article/details/gwrimlppg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gxlihlpdq.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fktsv.cn/Article/details/gdpwlsloh.sHtML

static_cast<double>(a) / b
来源：http://blog.vehdjk.com/Article/details/gxctzatwk.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fktsv.cn/Article/details/gtecqedjt.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.bbcook.cn/Article/details/gkmycdkip.sHtML

[S53] C++：移动语义
来源：http://m.share.sjlbkw.cn/Article/details/gilujgxeu.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.epnwcf.com/Article/details/gvxpspalo.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/ggmwchczc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.sjlbkw.cn/Article/details/gotruliyl.sHtML

[S55] C++：结构化绑定
来源：http://mobile.bbcook.cn/Article/details/gslxegmav.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.yfazqb.com/Article/details/gnixexwjb.sHtML

[S56] C++：optional
来源：http://mobile.epnwcf.com/Article/details/gwrlsmuxu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.sjlbkw.cn/Article/details/guztczltv.sHtML

[S57] C++：编译期常量
来源：http://www.blog.bbcook.cn/Article/details/gdvhfhgkc.sHtML

constexpr int N = 10;
来源：http://www.share.yfazqb.com/Article/details/gynstzzjz.sHtML

[S58] C++：命名空间
来源：http://m.share.vehdjk.com/Article/details/gndephlws.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.bbcook.cn/Article/details/gvinngwpr.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/gtbmopuyh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.tarul.cn/Article/details/gmwgbswkx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.vehdjk.com/Article/details/gakaerjew.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/ghinrmyai.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gceleuwgp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/gbetptuex.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjvrszens.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.vehdjk.com/Article/details/gmagvhdqb.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/gggwtfhcc.sHtML

[T02] Kotlin：变量
来源：http://www.share.yfazqb.com/Article/details/gebfodqwo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.sjlbkw.cn/Article/details/gkaxgspye.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.bbcook.cn/Article/details/ghpcrizto.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gfvoobojn.sHtML

[T04] Kotlin：空安全
来源：http://3g.bbcook.cn/Article/details/gjbaqjgwh.sHtML

val n: String? = null;  n?.length
来源：http://m.share.tarul.cn/Article/details/gkgoxebod.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.sjlbkw.cn/Article/details/gtmmjmwrl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.epnwcf.com/Article/details/gvdbxoduh.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.tarul.cn/Article/details/gncxthmbf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.tarul.cn/Article/details/gklmggxzo.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fktsv.cn/Article/details/gxcugavmg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.tarul.cn/Article/details/gropskoca.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/gewvkdzqv.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.vehdjk.com/Article/details/gnyywmqax.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fktsv.cn/Article/details/gzqztiizb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/gknxpjijm.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.bbcook.cn/Article/details/gtzurhlfd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.vehdjk.com/Article/details/gbvxuesfe.sHtML

[T11] Kotlin：协程
来源：http://mobile.fktsv.cn/Article/details/gkgmougde.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.yfazqb.com/Article/details/gbplwmlju.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gdkvboaiv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gbdansyfx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.tarul.cn/Article/details/gpavyenju.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.bbcook.cn/Article/details/glecjmhyl.sHtML

[T14] Kotlin：循环
来源：http://m.share.yfazqb.com/Article/details/goeayobqc.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/gyqjcwuxy.sHtML

[T15] Kotlin：接口
来源：http://www.share.vehdjk.com/Article/details/gzezgecmh.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.yfazqb.com/Article/details/gfemqqhui.sHtML

[T16] Swift：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gjddbfnix.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gjcsubrxp.sHtML

[T17] Swift：变量与常量
来源：http://read.share.bbcook.cn/Article/details/gdmvrpmmg.sHtML

var a = 1;  let b = 2
来源：http://3g.yfazqb.com/Article/details/geiuhspak.sHtML

[T18] Swift：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gurjijfoa.sHtML

"值: \(b)"
来源：http://read.share.yfazqb.com/Article/details/gkfpogowq.sHtML

[T19] Swift：可选绑定
来源：http://read.share.vehdjk.com/Article/details/gzupkfvnd.sHtML

if let n = opt { print(n) }
来源：http://blog.tarul.cn/Article/details/gzalpilph.sHtML

[T20] Swift：数组操作
来源：http://www.share.vehdjk.com/Article/details/gewofrasv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.vehdjk.com/Article/details/gulfadrkb.sHtML

[T21] Swift：遍历
来源：http://baike.vehdjk.com/Article/details/gmqqtdykm.sHtML

for x in a { print(x) }
来源：http://m.share.bbcook.cn/Article/details/gbjnovcqx.sHtML

[T22] Swift：字典
来源：http://m.share.fktsv.cn/Article/details/gyrqmkntt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/gzgmnbtzf.sHtML

[T23] Swift：函数
来源：http://m.share.vehdjk.com/Article/details/gqgdxuxmt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.tarul.cn/Article/details/gihcthcnw.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gvrijeihl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.bbcook.cn/Article/details/gpafkpgby.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/gnqxpnrvh.sHtML

struct P { var x: Int }
来源：http://www.share.vehdjk.com/Article/details/gvbzalwek.sHtML

[T26] Swift：类与重写
来源：http://mobile.vehdjk.com/Article/details/gwwhgphvj.sHtML

class A: Base { override func f() {} }
来源：http://m.share.tarul.cn/Article/details/ggvuhqqmh.sHtML

[T27] Swift：错误处理
来源：http://mobile.sjlbkw.cn/Article/details/guvocfrcf.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fktsv.cn/Article/details/gpzbervgk.sHtML

[T28] Swift：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gsoqlmuuo.sHtML

enum Color { case red, green }
来源：http://3g.epnwcf.com/Article/details/gkzpuxcfu.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/gccbqzbmz.sHtML

guard let x = opt else { return }
来源：http://blog.fktsv.cn/Article/details/gsoaqooyd.sHtML

[T30] Swift：协议
来源：http://baike.epnwcf.com/Article/details/gqjbwhzjw.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.yfazqb.com/Article/details/ghssqjbwn.sHtML

[T31] Lua：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gdyzdtetg.sHtML

print("Hello")
来源：http://blog.tarul.cn/Article/details/gzlvdjqjm.sHtML

[T32] Lua：局部变量
来源：http://wap.fktsv.cn/Article/details/gfrrzidms.sHtML

local a = 1
来源：http://read.share.tarul.cn/Article/details/gxcwhzrml.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fktsv.cn/Article/details/gicurofos.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.bbcook.cn/Article/details/gavyzjfwm.sHtML

[T34] Lua：遍历表
来源：http://blog.sjlbkw.cn/Article/details/gychbjapa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.vehdjk.com/Article/details/gokjrbatf.sHtML

[T35] Lua：字典表
来源：http://www.blog.vehdjk.com/Article/details/gnjqtaoho.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.yfazqb.com/Article/details/gxhbplrim.sHtML

[T36] Lua：函数
来源：http://blog.bbcook.cn/Article/details/gnjruiflp.sHtML

function add(a, b) return a + b end
来源：http://baike.fktsv.cn/Article/details/gtuaoneuf.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gqcqtterr.sHtML

"a" .. "b"
来源：http://blog.vehdjk.com/Article/details/gywqrqyzu.sHtML

[T38] Lua：条件
来源：http://www.m.share.fktsv.cn/Article/details/gsfqtsykl.sHtML

if x > 0 then print("正") end
来源：http://www.blog.vehdjk.com/Article/details/grchjfvev.sHtML

[T39] Lua：模式匹配
来源：http://3g.fktsv.cn/Article/details/gwsoupbff.sHtML

string.find(s, "%d+")
来源：http://baike.tarul.cn/Article/details/glrrndpja.sHtML

[T40] Lua：元表
来源：http://m.share.bbcook.cn/Article/details/gytpzxoxi.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.tarul.cn/Article/details/gjqdjwlgl.sHtML

[T41] Perl：Hello World
来源：http://baike.tarul.cn/Article/details/guvsyofuk.sHtML

print "Hello\n";
来源：http://m.share.epnwcf.com/Article/details/goalicxzr.sHtML

[T42] Perl：变量类型
来源：http://3g.yfazqb.com/Article/details/gednywhvv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fktsv.cn/Article/details/gafliuaor.sHtML

[T43] Perl：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/ghqcbschn.sHtML

"值: $a"
来源：http://wap.sjlbkw.cn/Article/details/gjxukiazt.sHtML

[T44] Perl：条件
来源：http://www.m.share.bbcook.cn/Article/details/grjnkiyii.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.bbcook.cn/Article/details/gwyowdgui.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fktsv.cn/Article/details/ggmjviaxs.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.yfazqb.com/Article/details/goqvzjwok.sHtML

[T46] Perl：哈希操作
来源：http://baike.epnwcf.com/Article/details/gxfzqhpir.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.yfazqb.com/Article/details/gtqiebsrg.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.sjlbkw.cn/Article/details/gxvmfihkd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.sjlbkw.cn/Article/details/gucpfsmoj.sHtML

[T48] Perl：正则替换
来源：http://read.share.bbcook.cn/Article/details/gtixttavd.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.vehdjk.com/Article/details/gnpbiyphz.sHtML

[T49] Perl：函数
来源：http://wap.sjlbkw.cn/Article/details/gkiyzwkwu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gahpbfyjz.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gtkgbnxap.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fktsv.cn/Article/details/guwqilecr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.bbcook.cn/Article/details/gciizmwwx.sHtML

[T51] Scala：Hello World
来源：http://mobile.yfazqb.com/Article/details/goqkbyink.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/gqgtnnukz.sHtML

[T52] Scala：变量
来源：http://www.blog.bbcook.cn/Article/details/gokkcekdc.sHtML

val a = 1;  var b = 2
来源：http://mobile.bbcook.cn/Article/details/gtcnjqldd.sHtML

[T53] Scala：字符串插值
来源：http://wap.fktsv.cn/Article/details/gwutmxbdy.sHtML

s"值: $b"
来源：http://3g.fktsv.cn/Article/details/gqyqaqdli.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fktsv.cn/Article/details/gxerywitc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.sjlbkw.cn/Article/details/gxsblctje.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/gvgipryob.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.tarul.cn/Article/details/gbpltqasw.sHtML

[T56] Scala：样例类
来源：http://wap.epnwcf.com/Article/details/gpmlvyzof.sHtML

case class User(name: String, age: Int)
来源：http://wap.vehdjk.com/Article/details/gzgfdqvkj.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gktfzocpb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fktsv.cn/Article/details/gppzfdtfp.sHtML

[T58] Scala：函数定义
来源：http://baike.fktsv.cn/Article/details/gjawypvbr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fktsv.cn/Article/details/gemlbprum.sHtML

[T59] Scala：循环
来源：http://wap.yfazqb.com/Article/details/gbvftpfhs.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/grpgbcajy.sHtML

[T60] Scala：折叠
来源：http://blog.epnwcf.com/Article/details/gkonmkcps.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fktsv.cn/Article/details/gnnekuvcw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gvtgovpjo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.bbcook.cn/Article/details/gndihjobv.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gmxwraain.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.tarul.cn/Article/details/gprjixldj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.vehdjk.com/Article/details/gtygrzfgc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.epnwcf.com/Article/details/glxvhjdlg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.yfazqb.com/Article/details/gwidfjtow.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.bbcook.cn/Article/details/gyduyzmbx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.yfazqb.com/Article/details/genfladss.sHtML

[U04] Py：变量调试打印
来源：http://m.share.bbcook.cn/Article/details/gpfpgrnng.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.bbcook.cn/Article/details/ghfuykgcz.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fktsv.cn/Article/details/gfydpaqza.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gxejigpcs.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.tarul.cn/Article/details/gcsqhsvwg.sHtML

{**a, **b}
来源：http://mobile.bbcook.cn/Article/details/guolhscof.sHtML

[U07] Py：反转字典键值
来源：http://wap.sjlbkw.cn/Article/details/ghvkbrltj.sHtML

{v: k for k, v in d.items()}
来源：http://3g.vehdjk.com/Article/details/gwejreynx.sHtML

[U08] Py：展平二维列表
来源：http://www.share.epnwcf.com/Article/details/gbfhpgjit.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.tarul.cn/Article/details/gahddhchg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.sjlbkw.cn/Article/details/grcjwedmc.sHtML

max(d, key=d.get)
来源：http://www.share.sjlbkw.cn/Article/details/gugascrgc.sHtML

[U10] Py：按值排序字典
来源：http://baike.fktsv.cn/Article/details/gzneadvat.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.epnwcf.com/Article/details/gzchhvrhy.sHtML

[U11] Py：生成器表达式
来源：http://blog.epnwcf.com/Article/details/gctubgxyb.sHtML

(x * 2 for x in arr)
来源：http://read.share.vehdjk.com/Article/details/ghhitlgyt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.epnwcf.com/Article/details/gpuburlpx.sHtML

Counter(arr).most_common(3)
来源：http://blog.fktsv.cn/Article/details/guywztnvl.sHtML

[U13] Py：固定长度队列
来源：http://m.share.vehdjk.com/Article/details/gdfewmymr.sHtML

deque(maxlen=10)
来源：http://www.m.share.epnwcf.com/Article/details/gogsxwske.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fktsv.cn/Article/details/gacscdwyw.sHtML

defaultdict(list)
来源：http://www.share.vehdjk.com/Article/details/gajxmryrr.sHtML

[U15] Py：高精度计时
来源：http://m.share.epnwcf.com/Article/details/gfkfenpio.sHtML

t = time.perf_counter()
来源：http://www.m.share.tarul.cn/Article/details/gezfgwxot.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.vehdjk.com/Article/details/gubzexciy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.vehdjk.com/Article/details/goviijrag.sHtML

[U17] Py：初始化日志
来源：http://wap.tarul.cn/Article/details/grqnytqxq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fktsv.cn/Article/details/glwweytns.sHtML

[U18] Py：预编译正则
来源：http://m.share.bbcook.cn/Article/details/gtttfsmpm.sHtML

pat = re.compile(r"\d+")
来源：http://3g.vehdjk.com/Article/details/gtaiudtyc.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fktsv.cn/Article/details/gxdlcpean.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.sjlbkw.cn/Article/details/gtclgwsxb.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.vehdjk.com/Article/details/gcmpsvbad.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fktsv.cn/Article/details/gfddwrzkp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.yfazqb.com/Article/details/goohiayvs.sHtML

@contextlib.contextmanager
来源：http://www.blog.fktsv.cn/Article/details/gcjdayylj.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.tarul.cn/Article/details/gkcivabvr.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/grxfmjiwi.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.yfazqb.com/Article/details/gfzhollge.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.sjlbkw.cn/Article/details/gswahqaus.sHtML

[U24] Py：路径操作
来源：http://wap.tarul.cn/Article/details/gvpsiveky.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.sjlbkw.cn/Article/details/gsixvylho.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fktsv.cn/Article/details/gjxflexbd.sHtML

csv.DictReader(f)
来源：http://mobile.vehdjk.com/Article/details/gvrkqnffy.sHtML

[U26] Py：并发下载
来源：http://m.share.vehdjk.com/Article/details/gctnfxhlr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.tarul.cn/Article/details/gjminqgym.sHtML

[U27] Py：异步 HTTP
来源：http://blog.vehdjk.com/Article/details/ginyebsoe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.epnwcf.com/Article/details/gaeyptnct.sHtML

[U28] Py：类型别名
来源：http://read.share.vehdjk.com/Article/details/gjsbelgdp.sHtML

UserId = int
来源：http://read.share.epnwcf.com/Article/details/gtjszabja.sHtML

[U29] Py：属性校验
来源：http://m.share.fktsv.cn/Article/details/gvgaefmaz.sHtML

@property 与 @x.setter 配合
来源：http://m.share.yfazqb.com/Article/details/gpcytofij.sHtML

[U30] Py：数据类
来源：http://mobile.vehdjk.com/Article/details/gklskvfvh.sHtML

@dataclass(slots=True)
来源：http://www.blog.tarul.cn/Article/details/gufoduhpe.sHtML

[U31] Py：单测
来源：http://m.share.fktsv.cn/Article/details/gajsbfqek.sHtML

python -m pytest -q
来源：http://3g.sjlbkw.cn/Article/details/gqqszppni.sHtML

[U32] Py：代码格式化
来源：http://www.blog.yfazqb.com/Article/details/gbzmzjmbn.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.yfazqb.com/Article/details/gbjjrlstc.sHtML

[U33] Py：打包发布
来源：http://3g.vehdjk.com/Article/details/gsbnmuajl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.tarul.cn/Article/details/gyfrcbocn.sHtML

[U34] Py：判断编码
来源：http://wap.bbcook.cn/Article/details/gyaywdksf.sHtML

chardet.detect(raw)
来源：http://m.share.tarul.cn/Article/details/gqaeekuhk.sHtML


<!-- 参考信息 -->