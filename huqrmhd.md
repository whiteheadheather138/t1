代发 wailian999

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/ggobufpdv.sHtML

[S06] C：字符串比较
来源：http://3g.vehdjk.com/Article/details/gzzhngfmr.sHtML

strcmp(a, b) == 0
来源：http://www.blog.epnwcf.com/Article/details/gwpxdjxbo.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/gzqxmmhkk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.bbcook.cn/Article/details/gugvtqppn.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.epnwcf.com/Article/details/gzzxstqkw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.epnwcf.com/Article/details/gyjndjoge.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.vehdjk.com/Article/details/gtawsljxo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gvsnebkom.sHtML

[S10] C：指针与解引用
来源：http://wap.fktsv.cn/Article/details/gwwzlwzpq.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.yfazqb.com/Article/details/gcqfmsblz.sHtML

[S11] C：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gdprizxiu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/gfmstxsfj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fktsv.cn/Article/details/gcjmiytxz.sHtML

fclose(f);
来源：http://read.share.vehdjk.com/Article/details/grjdgbowz.sHtML

[S12] C：写文件
来源：http://mobile.epnwcf.com/Article/details/glrbebjtz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gvnlpgvty.sHtML

[S13] C：宏定义
来源：http://3g.fktsv.cn/Article/details/gwkrfegio.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.sjlbkw.cn/Article/details/guklixkzr.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/gxzetbacp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.sjlbkw.cn/Article/details/gwiweelct.sHtML

[S15] C：类型转换
来源：http://www.share.sjlbkw.cn/Article/details/ggmkmgglu.sHtML

(double) a / b
来源：http://wap.epnwcf.com/Article/details/gcgkxntyp.sHtML

[S16] C：位操作置位
来源：http://wap.sjlbkw.cn/Article/details/guuwdjwyj.sHtML

x |= (1 << 3);
来源：http://wap.sjlbkw.cn/Article/details/gelbyudwr.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gatxnziba.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.bbcook.cn/Article/details/gstftweye.sHtML

[S18] C：命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/gddgwmfqj.sHtML

int main(int argc, char **argv)
来源：http://wap.vehdjk.com/Article/details/gqlwxbbuj.sHtML

[S19] C：快速排序
来源：http://read.share.fktsv.cn/Article/details/gpclxiihz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/gcukdcarj.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/gxsedydud.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/gtavmenif.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/gycqzroor.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.epnwcf.com/Article/details/grthiexiu.sHtML

[S22] C：字符串转数字
来源：http://blog.vehdjk.com/Article/details/gdxedsgaa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.vehdjk.com/Article/details/gfujkaiqz.sHtML

[S23] C：随机数
来源：http://www.blog.tarul.cn/Article/details/gtqhjpyys.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.vehdjk.com/Article/details/gimunenzo.sHtML

[S24] C：获取本地时间
来源：http://www.share.tarul.cn/Article/details/gbqeltddx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gmfhzaydr.sHtML

[S25] C：内存拷贝
来源：http://3g.sjlbkw.cn/Article/details/guuwekquy.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnbbiggl.sHtML

[S26] C：内存清零
来源：http://read.share.yfazqb.com/Article/details/gyysjhxsd.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gqnfnzwkl.sHtML

[S27] C：定义常量
来源：http://m.share.sjlbkw.cn/Article/details/gxarkqpiy.sHtML

const double PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gfujpemek.sHtML

[S28] C：静态变量
来源：http://www.share.vehdjk.com/Article/details/gzkupcuta.sHtML

static int counter = 0;
来源：http://read.share.yfazqb.com/Article/details/gyyopswbp.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/ggheqqsyk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/glvsaarzd.sHtML

[S30] C：头文件保护
来源：http://baike.fktsv.cn/Article/details/gkkmqidvf.sHtML

#ifndef X_H
来源：http://www.m.share.fktsv.cn/Article/details/giwwxptge.sHtML

#define X_H
来源：http://wap.bbcook.cn/Article/details/gptlzezja.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/guwfntfdr.sHtML

[S31] C++：Hello World
来源：http://www.share.bbcook.cn/Article/details/gfoidssub.sHtML

#include <iostream>
来源：http://read.share.epnwcf.com/Article/details/gfaycnqyr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/gmepmkyuf.sHtML

[S32] C++：字符串
来源：http://blog.bbcook.cn/Article/details/gaelsxemb.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/gepgsgvmt.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gogorfzag.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gqylefefo.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fktsv.cn/Article/details/gpmhjzqdk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.sjlbkw.cn/Article/details/gyczdjrhj.sHtML

[S35] C++：map
来源：http://3g.bbcook.cn/Article/details/ggsnuicrn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/ggiiscukv.sHtML

[S36] C++：unordered_map
来源：http://mobile.fktsv.cn/Article/details/gyqjbjdye.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/gbgvumglr.sHtML

[S37] C++：set
来源：http://mobile.sjlbkw.cn/Article/details/grynjdkhw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.epnwcf.com/Article/details/gndftvphl.sHtML

[S38] C++：排序
来源：http://www.blog.yfazqb.com/Article/details/gzxdhittd.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gjobadqbq.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.sjlbkw.cn/Article/details/gcjqhwhtb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.yfazqb.com/Article/details/gozryefwl.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/glsbkdruc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.vehdjk.com/Article/details/gtmxjrjus.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.yfazqb.com/Article/details/guznqcuzh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.tarul.cn/Article/details/gpwyquhbn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.epnwcf.com/Article/details/gcwmvwxnl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.sjlbkw.cn/Article/details/ggdiuhhqz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.yfazqb.com/Article/details/gokjovphm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvziliglq.sHtML

[S44] C++：引用传参
来源：http://baike.tarul.cn/Article/details/gfvgpwcyi.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.yfazqb.com/Article/details/grdphhbjh.sHtML

[S45] C++：lambda
来源：http://m.share.tarul.cn/Article/details/gmtzmpxmr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.yfazqb.com/Article/details/ggcuxngrb.sHtML

[S46] C++：函数模板
来源：http://mobile.bbcook.cn/Article/details/gqcdouimg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fktsv.cn/Article/details/grvdhlicj.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.vehdjk.com/Article/details/ghxfequnj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/gisivvxob.sHtML

[S48] C++：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gmngcdclv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gogeuujka.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/gysxbqgjm.sHtML

[S49] C++：写文件
来源：http://www.share.fktsv.cn/Article/details/geycjobvs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.sjlbkw.cn/Article/details/ghowtxtrt.sHtML

[S50] C++：格式化数字
来源：http://3g.epnwcf.com/Article/details/gtwliequm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.vehdjk.com/Article/details/giyqlpvib.sHtML

[S51] C++：显式类型转换
来源：http://mobile.yfazqb.com/Article/details/gcbpqhjtk.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/grtywbtdx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.yfazqb.com/Article/details/gphshfgbt.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.vehdjk.com/Article/details/grsraftfc.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/guctvpjyt.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.vehdjk.com/Article/details/gcwrsvewn.sHtML

[S54] C++：异常处理
来源：http://baike.vehdjk.com/Article/details/gpkpifwrn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.sjlbkw.cn/Article/details/gtxfelpjv.sHtML

[S55] C++：结构化绑定
来源：http://mobile.yfazqb.com/Article/details/gwxiolebq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.vehdjk.com/Article/details/gflowwxiu.sHtML

[S56] C++：optional
来源：http://3g.epnwcf.com/Article/details/gvbuszhjn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.yfazqb.com/Article/details/guthtukxi.sHtML

[S57] C++：编译期常量
来源：http://www.blog.bbcook.cn/Article/details/giolvouni.sHtML

constexpr int N = 10;
来源：http://read.share.epnwcf.com/Article/details/gemqzrlxy.sHtML

[S58] C++：命名空间
来源：http://wap.sjlbkw.cn/Article/details/grvlwmduo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.tarul.cn/Article/details/ghwdtxcat.sHtML

[S59] C++：静态断言
来源：http://www.share.vehdjk.com/Article/details/gnwbafhnk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.yfazqb.com/Article/details/gnabrvyig.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.sjlbkw.cn/Article/details/gzekucriq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.tarul.cn/Article/details/gqdeglyee.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzdashbto.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gthkbihbo.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvkkjnahk.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gtmrylaim.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gqxkkxqwm.sHtML

[T02] Kotlin：变量
来源：http://blog.yfazqb.com/Article/details/gngyiyvnh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fktsv.cn/Article/details/gbbtpkfaz.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.sjlbkw.cn/Article/details/guwivtjkj.sHtML

"值: $b"
来源：http://blog.epnwcf.com/Article/details/gzvcpfmlq.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/gahvirsmc.sHtML

val n: String? = null;  n?.length
来源：http://wap.epnwcf.com/Article/details/gkczdntdc.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.sjlbkw.cn/Article/details/gqzrzfcko.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gfsytlakp.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.bbcook.cn/Article/details/gqvyxskxj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.vehdjk.com/Article/details/gmffdawnn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fktsv.cn/Article/details/gxiiphjxg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.tarul.cn/Article/details/gpnbuqdcb.sHtML

[T08] Kotlin：数据类
来源：http://blog.fktsv.cn/Article/details/ggmhuufdk.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.epnwcf.com/Article/details/gqnoadkdz.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.yfazqb.com/Article/details/gybekzqmt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.epnwcf.com/Article/details/gzsqylmlx.sHtML

[T10] Kotlin：默认参数
来源：http://3g.vehdjk.com/Article/details/gdicfjiwz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.sjlbkw.cn/Article/details/gktquxcyi.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/ggybcfbgm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.sjlbkw.cn/Article/details/gpcowpnle.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/grnxcpqre.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.epnwcf.com/Article/details/gdpkhessf.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.sjlbkw.cn/Article/details/gfkhcligs.sHtML

val m = mapOf("a" to 1)
来源：http://baike.yfazqb.com/Article/details/gunlohmyk.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/grluvqqil.sHtML

for (i in 1..10) println(i)
来源：http://blog.fktsv.cn/Article/details/glkmleago.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/gsrsrssee.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.yfazqb.com/Article/details/gxcetniec.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gbhrfdoxg.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gyhhypezq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.epnwcf.com/Article/details/ggingjrol.sHtML

var a = 1;  let b = 2
来源：http://www.share.bbcook.cn/Article/details/gmayowdoo.sHtML

[T18] Swift：字符串插值
来源：http://blog.fktsv.cn/Article/details/gzqcakmwy.sHtML

"值: \(b)"
来源：http://blog.sjlbkw.cn/Article/details/gtcnfdpcw.sHtML

[T19] Swift：可选绑定
来源：http://read.share.tarul.cn/Article/details/gemglevlh.sHtML

if let n = opt { print(n) }
来源：http://www.share.fktsv.cn/Article/details/glxmwbces.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/gujirivlt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.yfazqb.com/Article/details/gslwdbeqc.sHtML

[T21] Swift：遍历
来源：http://wap.yfazqb.com/Article/details/gpwdbtzsk.sHtML

for x in a { print(x) }
来源：http://baike.tarul.cn/Article/details/gudgkbvht.sHtML

[T22] Swift：字典
来源：http://www.blog.fktsv.cn/Article/details/gvtmftejn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fktsv.cn/Article/details/gbantamyj.sHtML

[T23] Swift：函数
来源：http://wap.tarul.cn/Article/details/gwxezxpqj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gauebfuiy.sHtML

[T24] Swift：闭包
来源：http://www.blog.sjlbkw.cn/Article/details/gqjvcuyjw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fktsv.cn/Article/details/goltfphdj.sHtML

[T25] Swift：结构体
来源：http://blog.yfazqb.com/Article/details/gliqprocp.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/gsosgrgbr.sHtML

[T26] Swift：类与重写
来源：http://www.blog.vehdjk.com/Article/details/gjtbnstcy.sHtML

class A: Base { override func f() {} }
来源：http://3g.sjlbkw.cn/Article/details/gmbtyojku.sHtML

[T27] Swift：错误处理
来源：http://m.share.fktsv.cn/Article/details/gyzcduvym.sHtML

do { try f() } catch { print(error) }
来源：http://blog.sjlbkw.cn/Article/details/goonirdbw.sHtML

[T28] Swift：枚举
来源：http://blog.bbcook.cn/Article/details/ggdrdgwew.sHtML

enum Color { case red, green }
来源：http://wap.epnwcf.com/Article/details/gpmeqzqla.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.epnwcf.com/Article/details/gyyvtztxb.sHtML

guard let x = opt else { return }
来源：http://blog.epnwcf.com/Article/details/gyefndvqr.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/gymvawqrm.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.vehdjk.com/Article/details/gzlgljrmi.sHtML

[T31] Lua：Hello World
来源：http://www.share.vehdjk.com/Article/details/ggbpevwxf.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gocmiixns.sHtML

[T32] Lua：局部变量
来源：http://baike.sjlbkw.cn/Article/details/gzppgvbfv.sHtML

local a = 1
来源：http://wap.bbcook.cn/Article/details/gbsdmwmgy.sHtML

[T33] Lua：表（数组）
来源：http://3g.sjlbkw.cn/Article/details/gqvubrkdv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.epnwcf.com/Article/details/gxkbfynrd.sHtML

[T34] Lua：遍历表
来源：http://mobile.sjlbkw.cn/Article/details/gixrlvifu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/golwocdsn.sHtML

[T35] Lua：字典表
来源：http://read.share.tarul.cn/Article/details/grotkvjpd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/gvykpspjh.sHtML

[T36] Lua：函数
来源：http://www.m.share.bbcook.cn/Article/details/glfeuwzwf.sHtML

function add(a, b) return a + b end
来源：http://wap.epnwcf.com/Article/details/gdvruegtx.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.vehdjk.com/Article/details/ggywcumur.sHtML

"a" .. "b"
来源：http://m.share.tarul.cn/Article/details/gfrnpbtmy.sHtML

[T38] Lua：条件
来源：http://3g.vehdjk.com/Article/details/gqfetrhok.sHtML

if x > 0 then print("正") end
来源：http://www.share.tarul.cn/Article/details/gubaskzpf.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gsrjjqqyk.sHtML

string.find(s, "%d+")
来源：http://wap.fktsv.cn/Article/details/gqvzgyenz.sHtML

[T40] Lua：元表
来源：http://wap.epnwcf.com/Article/details/ghmflglsi.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.sjlbkw.cn/Article/details/gsfgansqe.sHtML

[T41] Perl：Hello World
来源：http://read.share.epnwcf.com/Article/details/gaoyyceof.sHtML

print "Hello\n";
来源：http://3g.bbcook.cn/Article/details/gnwagdpgh.sHtML

[T42] Perl：变量类型
来源：http://www.share.sjlbkw.cn/Article/details/gtsgyrbkf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fktsv.cn/Article/details/gnpudzoaj.sHtML

[T43] Perl：字符串插值
来源：http://baike.tarul.cn/Article/details/ghtitdodi.sHtML

"值: $a"
来源：http://baike.fktsv.cn/Article/details/gkbzhmcum.sHtML

[T44] Perl：条件
来源：http://baike.yfazqb.com/Article/details/gnvbbafbs.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.tarul.cn/Article/details/gjqlhqjvp.sHtML

[T45] Perl：数组遍历
来源：http://blog.fktsv.cn/Article/details/ggnevtwag.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.sjlbkw.cn/Article/details/gxrtawcgy.sHtML

[T46] Perl：哈希操作
来源：http://blog.tarul.cn/Article/details/ggylatouw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.epnwcf.com/Article/details/gwhqqniem.sHtML

[T47] Perl：正则捕获
来源：http://m.share.vehdjk.com/Article/details/gtsyhvxpa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.yfazqb.com/Article/details/gizksicyc.sHtML

[T48] Perl：正则替换
来源：http://3g.fktsv.cn/Article/details/ggevlesse.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.sjlbkw.cn/Article/details/glfdpuabr.sHtML

[T49] Perl：函数
来源：http://www.blog.vehdjk.com/Article/details/gawnjrdyq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gyemphrht.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/geaffyijq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.yfazqb.com/Article/details/gbalvscgq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.epnwcf.com/Article/details/gsjyipsvj.sHtML

[T51] Scala：Hello World
来源：http://baike.bbcook.cn/Article/details/giauywucm.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gdnprtqrg.sHtML

[T52] Scala：变量
来源：http://baike.yfazqb.com/Article/details/gqkauxyyy.sHtML

val a = 1;  var b = 2
来源：http://blog.yfazqb.com/Article/details/gxhqbvvgk.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gnsmqzlfs.sHtML

s"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gzkxocoyy.sHtML

[T54] Scala：集合映射
来源：http://3g.tarul.cn/Article/details/gwustchha.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.epnwcf.com/Article/details/gkonmsjxt.sHtML

[T55] Scala：集合过滤
来源：http://www.share.yfazqb.com/Article/details/gfbzwbrbp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.sjlbkw.cn/Article/details/ghisokyak.sHtML

[T56] Scala：样例类
来源：http://www.m.share.bbcook.cn/Article/details/gpccqjrzf.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.epnwcf.com/Article/details/guwentlww.sHtML

[T57] Scala：模式匹配
来源：http://blog.bbcook.cn/Article/details/gjudsqfdq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gihwyzriz.sHtML

[T58] Scala：函数定义
来源：http://www.share.tarul.cn/Article/details/gekgqvqbd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.yfazqb.com/Article/details/gffszwkgr.sHtML

[T59] Scala：循环
来源：http://3g.epnwcf.com/Article/details/grwricnfj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/ggspnrrlo.sHtML

[T60] Scala：折叠
来源：http://read.share.fktsv.cn/Article/details/gcvhukxmh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.vehdjk.com/Article/details/gtycgdlrc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpvjazamp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.yfazqb.com/Article/details/gcpreznab.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghgdszdir.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.bbcook.cn/Article/details/grpsevwli.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.epnwcf.com/Article/details/giwzzbvbn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.vehdjk.com/Article/details/gnamzmxea.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.vehdjk.com/Article/details/gkpttbbya.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.yfazqb.com/Article/details/gwpquirsv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.yfazqb.com/Article/details/grfarftar.sHtML

[U04] Py：变量调试打印
来源：http://mobile.tarul.cn/Article/details/gwblfysaq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.epnwcf.com/Article/details/goitbcdii.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.tarul.cn/Article/details/gyqsaxmxv.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.tarul.cn/Article/details/gjuuafnhf.sHtML

[U06] Py：合并两个字典
来源：http://mobile.vehdjk.com/Article/details/ggtzpfncr.sHtML

{**a, **b}
来源：http://wap.yfazqb.com/Article/details/gplbikjdm.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.bbcook.cn/Article/details/gcicbjwgq.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fktsv.cn/Article/details/gzbjqnsft.sHtML

[U08] Py：展平二维列表
来源：http://blog.sjlbkw.cn/Article/details/geapjrtkg.sHtML

[y for x in nested for y in x]
来源：http://3g.sjlbkw.cn/Article/details/gzsthxgod.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.epnwcf.com/Article/details/gkkbsxcpr.sHtML

max(d, key=d.get)
来源：http://www.m.share.bbcook.cn/Article/details/gxvtugkqs.sHtML

[U10] Py：按值排序字典
来源：http://blog.tarul.cn/Article/details/gogeusdkt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.tarul.cn/Article/details/giygdfaqi.sHtML

[U11] Py：生成器表达式
来源：http://m.share.bbcook.cn/Article/details/gzrvtegaq.sHtML

(x * 2 for x in arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gflgibaex.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.sjlbkw.cn/Article/details/gjgwmrcuv.sHtML

Counter(arr).most_common(3)
来源：http://wap.yfazqb.com/Article/details/gzqhmcvvw.sHtML

[U13] Py：固定长度队列
来源：http://read.share.sjlbkw.cn/Article/details/glujxstqy.sHtML

deque(maxlen=10)
来源：http://mobile.vehdjk.com/Article/details/gtzlgphas.sHtML

[U14] Py：分组收集到列表
来源：http://baike.yfazqb.com/Article/details/gguwhqiyf.sHtML

defaultdict(list)
来源：http://www.m.share.yfazqb.com/Article/details/gjdolgafo.sHtML

[U15] Py：高精度计时
来源：http://baike.epnwcf.com/Article/details/gzxyfosod.sHtML

t = time.perf_counter()
来源：http://baike.fktsv.cn/Article/details/ghrgsbely.sHtML

[U16] Py：命令行参数解析
来源：http://baike.vehdjk.com/Article/details/giymieked.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.epnwcf.com/Article/details/gmlndaxfp.sHtML

[U17] Py：初始化日志
来源：http://blog.fktsv.cn/Article/details/gdpjylzuy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.vehdjk.com/Article/details/gpjnlrtrm.sHtML

[U18] Py：预编译正则
来源：http://wap.fktsv.cn/Article/details/gljfuuorx.sHtML

pat = re.compile(r"\d+")
来源：http://3g.sjlbkw.cn/Article/details/gyzrsayjk.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.vehdjk.com/Article/details/gmvwowrdl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.vehdjk.com/Article/details/giioxzcmg.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.epnwcf.com/Article/details/glwzhmuir.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.yfazqb.com/Article/details/gjmwcknva.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.vehdjk.com/Article/details/glsekvkat.sHtML

@contextlib.contextmanager
来源：http://baike.tarul.cn/Article/details/gecwdgdoe.sHtML

[U22] Py：矩阵转置
来源：http://blog.yfazqb.com/Article/details/gixrcrroi.sHtML

list(zip(*m))
来源：http://blog.yfazqb.com/Article/details/grjlkefrm.sHtML

[U23] Py：分块读取大文件
来源：http://wap.yfazqb.com/Article/details/ggtdmbhiq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fktsv.cn/Article/details/gphiiphmh.sHtML

[U24] Py：路径操作
来源：http://read.share.vehdjk.com/Article/details/gehfoiryx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/gcjpitaok.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.bbcook.cn/Article/details/glohvvygt.sHtML

csv.DictReader(f)
来源：http://www.m.share.vehdjk.com/Article/details/ggeyekinm.sHtML

[U26] Py：并发下载
来源：http://m.share.tarul.cn/Article/details/gegnzovdq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.yfazqb.com/Article/details/gudmfmpls.sHtML

[U27] Py：异步 HTTP
来源：http://3g.sjlbkw.cn/Article/details/ggilknlwu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fktsv.cn/Article/details/gpvgeyidu.sHtML

[U28] Py：类型别名
来源：http://mobile.vehdjk.com/Article/details/gtuyxdaxp.sHtML

UserId = int
来源：http://m.share.tarul.cn/Article/details/gfubtgxzi.sHtML


<!-- 参考信息 -->