代发 wailian999

int x; scanf("%d", &x);
来源：http://www.share.vehdjk.com/Article/details/gzsaxpbgi.sHtML

[S04] C：字符串复制
来源：http://wap.bbcook.cn/Article/details/ggbjkgold.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gsclqisvw.sHtML

[S05] C：字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gmbvauycw.sHtML

strlen(s)
来源：http://www.blog.fktsv.cn/Article/details/gaakscjyq.sHtML

[S06] C：字符串比较
来源：http://3g.sjlbkw.cn/Article/details/ggbzktaoa.sHtML

strcmp(a, b) == 0
来源：http://www.blog.sjlbkw.cn/Article/details/gfhtvrbet.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fktsv.cn/Article/details/gdxgntvmg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.yfazqb.com/Article/details/gfrjceqli.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.tarul.cn/Article/details/gxwfthmft.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.tarul.cn/Article/details/gqstqweej.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/gpcojqehy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gepxzditt.sHtML

[S10] C：指针与解引用
来源：http://blog.yfazqb.com/Article/details/gelpcfnnj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.yfazqb.com/Article/details/gracneplf.sHtML

[S11] C：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gqrcanisp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/grtrsowqo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.sjlbkw.cn/Article/details/gfxckducr.sHtML

fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/ghpbasflq.sHtML

[S12] C：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gwusbsgib.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.yfazqb.com/Article/details/gizhrjstr.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/gppnmjpuy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fktsv.cn/Article/details/gvtnfuopy.sHtML

[S14] C：枚举
来源：http://mobile.epnwcf.com/Article/details/gehqzkzmf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.vehdjk.com/Article/details/ghzvzjhio.sHtML

[S15] C：类型转换
来源：http://www.share.yfazqb.com/Article/details/ggxabautd.sHtML

(double) a / b
来源：http://www.share.tarul.cn/Article/details/gobfcsfgk.sHtML

[S16] C：位操作置位
来源：http://mobile.yfazqb.com/Article/details/grjejgwji.sHtML

x |= (1 << 3);
来源：http://mobile.vehdjk.com/Article/details/ggcevlcmd.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gsonqkbgx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fktsv.cn/Article/details/gfinajmzn.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/ggjlhdsui.sHtML

int main(int argc, char **argv)
来源：http://read.share.yfazqb.com/Article/details/gddrsaklu.sHtML

[S19] C：快速排序
来源：http://read.share.epnwcf.com/Article/details/gpvicmxsj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/glbproqyg.sHtML

[S20] C：二分查找
来源：http://baike.tarul.cn/Article/details/gezggfdxs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gymlfsilt.sHtML

[S21] C：字符类别判断
来源：http://mobile.tarul.cn/Article/details/gdewcbyja.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.tarul.cn/Article/details/gyjgeysws.sHtML

[S22] C：字符串转数字
来源：http://m.share.epnwcf.com/Article/details/gqswhqzpr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/gtomnvzeg.sHtML

[S23] C：随机数
来源：http://wap.vehdjk.com/Article/details/gvtfemocz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.bbcook.cn/Article/details/gmgexbfyp.sHtML

[S24] C：获取本地时间
来源：http://blog.vehdjk.com/Article/details/gysgzqpnw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.bbcook.cn/Article/details/glkwdwxji.sHtML

[S25] C：内存拷贝
来源：http://wap.sjlbkw.cn/Article/details/gpadplure.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.bbcook.cn/Article/details/gpsypljpa.sHtML

[S26] C：内存清零
来源：http://read.share.sjlbkw.cn/Article/details/gtlmtzmri.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.tarul.cn/Article/details/gwlhjwajz.sHtML

[S27] C：定义常量
来源：http://blog.vehdjk.com/Article/details/geptwlgxs.sHtML

const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gqzjtspsq.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gomyfexuz.sHtML

static int counter = 0;
来源：http://baike.epnwcf.com/Article/details/galhdfxus.sHtML

[S29] C：变参函数
来源：http://www.share.fktsv.cn/Article/details/gcccjvfau.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.bbcook.cn/Article/details/gvkiqlzrk.sHtML

[S30] C：头文件保护
来源：http://www.m.share.yfazqb.com/Article/details/gigakgiri.sHtML

#ifndef X_H
来源：http://read.share.fktsv.cn/Article/details/gihstsxhx.sHtML

#define X_H
来源：http://blog.sjlbkw.cn/Article/details/gzooxitji.sHtML

#endif
来源：http://www.share.vehdjk.com/Article/details/gpophqllx.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/gloqizvrz.sHtML

#include <iostream>
来源：http://3g.sjlbkw.cn/Article/details/gofsjvwae.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.tarul.cn/Article/details/ghrtdjmdl.sHtML

[S32] C++：字符串
来源：http://read.share.sjlbkw.cn/Article/details/gmphifznt.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/gbzacksda.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/gzeppqmtf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.bbcook.cn/Article/details/gcmosrrgk.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.yfazqb.com/Article/details/gnksjucwt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.bbcook.cn/Article/details/gbukmiwtm.sHtML

[S35] C++：map
来源：http://baike.epnwcf.com/Article/details/gguzaztku.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/glrveurol.sHtML

[S36] C++：unordered_map
来源：http://3g.vehdjk.com/Article/details/gzhnegscs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/ghyymcowl.sHtML

[S37] C++：set
来源：http://baike.epnwcf.com/Article/details/gttpheiam.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.epnwcf.com/Article/details/grpnsvcte.sHtML

[S38] C++：排序
来源：http://baike.fktsv.cn/Article/details/grfixckvy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gwevcuyzl.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/ggtnyasbn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.epnwcf.com/Article/details/ghlhizlmi.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/gptfikepv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/gnuhbyean.sHtML

[S41] C++：类与构造函数
来源：http://www.share.bbcook.cn/Article/details/gclzjeotu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/gclstbiga.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.sjlbkw.cn/Article/details/glhukczox.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.sjlbkw.cn/Article/details/gltzrvkvb.sHtML

[S43] C++：智能指针
来源：http://blog.epnwcf.com/Article/details/gncyhrsba.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.vehdjk.com/Article/details/glmyilsej.sHtML

[S44] C++：引用传参
来源：http://blog.bbcook.cn/Article/details/gehrzdlxv.sHtML

void inc(int &x) { ++x; }
来源：http://blog.sjlbkw.cn/Article/details/gdpggrggs.sHtML

[S45] C++：lambda
来源：http://wap.bbcook.cn/Article/details/gpewnahhg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fktsv.cn/Article/details/gokqlquyj.sHtML

[S46] C++：函数模板
来源：http://m.share.yfazqb.com/Article/details/gxjaesgkr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gqqwpsavg.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.yfazqb.com/Article/details/grtvstxha.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.epnwcf.com/Article/details/gdzwdwymz.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gnhwvskrr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.yfazqb.com/Article/details/gsgskvaev.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fktsv.cn/Article/details/ginvcogsa.sHtML

[S49] C++：写文件
来源：http://m.share.bbcook.cn/Article/details/gakoxubfv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.sjlbkw.cn/Article/details/gwuerhcge.sHtML

[S50] C++：格式化数字
来源：http://mobile.yfazqb.com/Article/details/gccyacsnl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.tarul.cn/Article/details/gihcatzpm.sHtML

[S51] C++：显式类型转换
来源：http://3g.yfazqb.com/Article/details/gtggzdgzb.sHtML

static_cast<double>(a) / b
来源：http://www.blog.sjlbkw.cn/Article/details/gucbzxtxr.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.tarul.cn/Article/details/gddwfhzos.sHtML

int size() const noexcept { return n_; }
来源：http://blog.yfazqb.com/Article/details/gutcwnoqn.sHtML

[S53] C++：移动语义
来源：http://blog.fktsv.cn/Article/details/gbkiqqthd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fktsv.cn/Article/details/glbahlkkk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fktsv.cn/Article/details/gxrjzlhvo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/giiddqtiv.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/gxmtjpnzs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.bbcook.cn/Article/details/gtdctlegw.sHtML

[S56] C++：optional
来源：http://mobile.bbcook.cn/Article/details/gsshwegyk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.vehdjk.com/Article/details/goyllhpvy.sHtML

[S57] C++：编译期常量
来源：http://blog.tarul.cn/Article/details/gebenuxoa.sHtML

constexpr int N = 10;
来源：http://mobile.epnwcf.com/Article/details/gcmmytnsm.sHtML

[S58] C++：命名空间
来源：http://read.share.bbcook.cn/Article/details/gncbxdufn.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fktsv.cn/Article/details/ghdudbizl.sHtML

[S59] C++：静态断言
来源：http://mobile.epnwcf.com/Article/details/ggjrluntz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnntyqmi.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.tarul.cn/Article/details/gzmfbosoc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.yfazqb.com/Article/details/gnrxzfhsu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvxpampvc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gfqnoedoa.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grlgdoute.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.yfazqb.com/Article/details/gavgszyyv.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gkzzzyntk.sHtML

[T02] Kotlin：变量
来源：http://baike.yfazqb.com/Article/details/gwqreoyif.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.epnwcf.com/Article/details/gowskrzhy.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.tarul.cn/Article/details/gxapymvjy.sHtML

"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/goadaxlji.sHtML

[T04] Kotlin：空安全
来源：http://www.share.vehdjk.com/Article/details/godrcsmmh.sHtML

val n: String? = null;  n?.length
来源：http://read.share.yfazqb.com/Article/details/glhspllga.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fktsv.cn/Article/details/gfpznwebj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fktsv.cn/Article/details/gkpofjxdo.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gktjopemk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/gyfflfswe.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gkygypzlo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfbpebnv.sHtML

[T08] Kotlin：数据类
来源：http://3g.fktsv.cn/Article/details/ghfcvdivx.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.vehdjk.com/Article/details/gmtgryiyt.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.tarul.cn/Article/details/gejzmfknn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/gywvkksen.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.tarul.cn/Article/details/gkuxfhyrt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.sjlbkw.cn/Article/details/gqshsdnxc.sHtML

[T11] Kotlin：协程
来源：http://m.share.epnwcf.com/Article/details/ggsnwdnva.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.tarul.cn/Article/details/gziumbmub.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.bbcook.cn/Article/details/glcyrwucs.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.epnwcf.com/Article/details/grrjqwlkx.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.sjlbkw.cn/Article/details/gmkyyjgff.sHtML

val m = mapOf("a" to 1)
来源：http://wap.yfazqb.com/Article/details/gbthsxtav.sHtML

[T14] Kotlin：循环
来源：http://www.blog.yfazqb.com/Article/details/ghcybxvqm.sHtML

for (i in 1..10) println(i)
来源：http://baike.bbcook.cn/Article/details/gwsuprjjs.sHtML

[T15] Kotlin：接口
来源：http://3g.bbcook.cn/Article/details/gavsgwchz.sHtML

interface Shape { fun area(): Double }
来源：http://3g.epnwcf.com/Article/details/gtvcbepzg.sHtML

[T16] Swift：Hello World
来源：http://wap.yfazqb.com/Article/details/gxqdtykwg.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gcemegliw.sHtML

[T17] Swift：变量与常量
来源：http://baike.fktsv.cn/Article/details/gykvgwzom.sHtML

var a = 1;  let b = 2
来源：http://blog.bbcook.cn/Article/details/gnrqtbrjo.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fktsv.cn/Article/details/glgiubfrl.sHtML

"值: \(b)"
来源：http://www.m.share.epnwcf.com/Article/details/gevpkhmle.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/gkdhqbdar.sHtML

if let n = opt { print(n) }
来源：http://read.share.tarul.cn/Article/details/gaiypxmwr.sHtML

[T20] Swift：数组操作
来源：http://www.blog.yfazqb.com/Article/details/gbuazsoeu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.tarul.cn/Article/details/gcmjzwyps.sHtML

[T21] Swift：遍历
来源：http://blog.bbcook.cn/Article/details/geqlvidhs.sHtML

for x in a { print(x) }
来源：http://baike.vehdjk.com/Article/details/gtajsjwsp.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gmnwzdqdw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.yfazqb.com/Article/details/gcejpoxpz.sHtML

[T23] Swift：函数
来源：http://blog.epnwcf.com/Article/details/ghhwdghdi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gebtpwsjx.sHtML

[T24] Swift：闭包
来源：http://read.share.epnwcf.com/Article/details/gsavexyps.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gygtszkml.sHtML

[T25] Swift：结构体
来源：http://mobile.vehdjk.com/Article/details/gpjbprpdx.sHtML

struct P { var x: Int }
来源：http://wap.bbcook.cn/Article/details/gfmxbqjoe.sHtML

[T26] Swift：类与重写
来源：http://www.share.bbcook.cn/Article/details/gtknukpod.sHtML

class A: Base { override func f() {} }
来源：http://read.share.yfazqb.com/Article/details/gvnxawmqr.sHtML

[T27] Swift：错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gpypnhbis.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.vehdjk.com/Article/details/gfhhmdewx.sHtML

[T28] Swift：枚举
来源：http://m.share.sjlbkw.cn/Article/details/gonpludox.sHtML

enum Color { case red, green }
来源：http://wap.epnwcf.com/Article/details/gqxnnsded.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.bbcook.cn/Article/details/gngkznuuc.sHtML

guard let x = opt else { return }
来源：http://blog.vehdjk.com/Article/details/gjxfurgez.sHtML

[T30] Swift：协议
来源：http://wap.epnwcf.com/Article/details/gsxjierox.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.bbcook.cn/Article/details/giljninwx.sHtML

[T31] Lua：Hello World
来源：http://www.blog.tarul.cn/Article/details/gcstdenaq.sHtML

print("Hello")
来源：http://www.blog.tarul.cn/Article/details/glmmkpfas.sHtML

[T32] Lua：局部变量
来源：http://baike.epnwcf.com/Article/details/gxulghmcf.sHtML

local a = 1
来源：http://m.share.tarul.cn/Article/details/gzrvsuctw.sHtML

[T33] Lua：表（数组）
来源：http://3g.vehdjk.com/Article/details/grwobsjhx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.vehdjk.com/Article/details/gotriutxe.sHtML

[T34] Lua：遍历表
来源：http://baike.epnwcf.com/Article/details/gpkufabgj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.epnwcf.com/Article/details/gsuzzmjqu.sHtML

[T35] Lua：字典表
来源：http://wap.yfazqb.com/Article/details/giykpjppw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gplmmsaza.sHtML

[T36] Lua：函数
来源：http://read.share.vehdjk.com/Article/details/gabzvuomi.sHtML

function add(a, b) return a + b end
来源：http://mobile.epnwcf.com/Article/details/ggeamikyx.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fktsv.cn/Article/details/gjlaybpno.sHtML

"a" .. "b"
来源：http://3g.bbcook.cn/Article/details/gbiofmhur.sHtML

[T38] Lua：条件
来源：http://www.share.yfazqb.com/Article/details/gwwuzmnxc.sHtML

if x > 0 then print("正") end
来源：http://wap.vehdjk.com/Article/details/glfimkhdj.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/gtfghuznv.sHtML

string.find(s, "%d+")
来源：http://www.share.bbcook.cn/Article/details/gmgnmmjiu.sHtML

[T40] Lua：元表
来源：http://www.m.share.bbcook.cn/Article/details/glvlqpnry.sHtML

setmetatable({}, { __index = base })
来源：http://3g.tarul.cn/Article/details/gotapezfk.sHtML

[T41] Perl：Hello World
来源：http://blog.fktsv.cn/Article/details/ggfbwjnjm.sHtML

print "Hello\n";
来源：http://www.m.share.epnwcf.com/Article/details/gplvuohql.sHtML

[T42] Perl：变量类型
来源：http://baike.sjlbkw.cn/Article/details/gycnddfez.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.yfazqb.com/Article/details/gxxuxavuv.sHtML

[T43] Perl：字符串插值
来源：http://www.share.epnwcf.com/Article/details/govtphitt.sHtML

"值: $a"
来源：http://wap.tarul.cn/Article/details/ghvmkzjwx.sHtML

[T44] Perl：条件
来源：http://baike.bbcook.cn/Article/details/gypukflbo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.bbcook.cn/Article/details/grrwkvwuf.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.yfazqb.com/Article/details/gllcuroxd.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.sjlbkw.cn/Article/details/gvegdnmbi.sHtML

[T46] Perl：哈希操作
来源：http://wap.fktsv.cn/Article/details/ggsdwiguc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/gmcnuyaja.sHtML

[T47] Perl：正则捕获
来源：http://3g.yfazqb.com/Article/details/gsbweftlm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyahnfop.sHtML

[T48] Perl：正则替换
来源：http://www.blog.sjlbkw.cn/Article/details/gswnypfad.sHtML

$s =~ s/old/new/g;
来源：http://m.share.tarul.cn/Article/details/gfoeizbon.sHtML

[T49] Perl：函数
来源：http://m.share.yfazqb.com/Article/details/gwhmyttnd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gsrtaizsd.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gldfxidyl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.sjlbkw.cn/Article/details/ggmkxtjyr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.epnwcf.com/Article/details/getjcuaao.sHtML

[T51] Scala：Hello World
来源：http://www.share.fktsv.cn/Article/details/gmrgmptpy.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/ggjirkbww.sHtML

[T52] Scala：变量
来源：http://3g.tarul.cn/Article/details/gmarrikhx.sHtML

val a = 1;  var b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gubaiwyrr.sHtML

[T53] Scala：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gifjuoygm.sHtML

s"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gryncaguf.sHtML

[T54] Scala：集合映射
来源：http://blog.bbcook.cn/Article/details/gvjgxorqn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.vehdjk.com/Article/details/galrynihu.sHtML

[T55] Scala：集合过滤
来源：http://3g.epnwcf.com/Article/details/gzjwtfata.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.epnwcf.com/Article/details/gumknwuil.sHtML

[T56] Scala：样例类
来源：http://www.m.share.yfazqb.com/Article/details/grynfuicy.sHtML

case class User(name: String, age: Int)
来源：http://mobile.tarul.cn/Article/details/gsncnyvpb.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.tarul.cn/Article/details/gutixiqvo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.sjlbkw.cn/Article/details/gzzvgstlv.sHtML

[T58] Scala：函数定义
来源：http://blog.fktsv.cn/Article/details/gjpirlgfe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.yfazqb.com/Article/details/gsmmuptyc.sHtML

[T59] Scala：循环
来源：http://www.m.share.vehdjk.com/Article/details/gvkksfqpn.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fktsv.cn/Article/details/ggardwcca.sHtML

[T60] Scala：折叠
来源：http://read.share.epnwcf.com/Article/details/gyovlakdh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fktsv.cn/Article/details/gmxqrhbml.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gtyoszgrz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.yfazqb.com/Article/details/gvvqswbad.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grwhxylxt.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.yfazqb.com/Article/details/gttrmoltf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.sjlbkw.cn/Article/details/gooumgrhu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.sjlbkw.cn/Article/details/gpolkqtwg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.sjlbkw.cn/Article/details/gmpxcdqnu.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.yfazqb.com/Article/details/gdssouauv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.sjlbkw.cn/Article/details/gxavkmddy.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.sjlbkw.cn/Article/details/gzytmalrx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.bbcook.cn/Article/details/gwiqdkdlt.sHtML

[U05] Py：列表去重且保序
来源：http://blog.tarul.cn/Article/details/gbdfipprh.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fktsv.cn/Article/details/giyvnxkeh.sHtML

[U06] Py：合并两个字典
来源：http://mobile.sjlbkw.cn/Article/details/gwoxcnmlv.sHtML

{**a, **b}
来源：http://3g.fktsv.cn/Article/details/gajbpymrh.sHtML

[U07] Py：反转字典键值
来源：http://read.share.tarul.cn/Article/details/gfsywjnks.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.yfazqb.com/Article/details/gcvunblqx.sHtML

[U08] Py：展平二维列表
来源：http://baike.sjlbkw.cn/Article/details/ghcjjibwn.sHtML

[y for x in nested for y in x]
来源：http://wap.tarul.cn/Article/details/gchhorqzc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.tarul.cn/Article/details/gqirclwor.sHtML

max(d, key=d.get)
来源：http://blog.bbcook.cn/Article/details/gifrnzeru.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.tarul.cn/Article/details/ghvsaufhg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.tarul.cn/Article/details/gsupgjnte.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.epnwcf.com/Article/details/gyqlutyez.sHtML

(x * 2 for x in arr)
来源：http://mobile.tarul.cn/Article/details/gakcnywpn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/gkfuydrum.sHtML

Counter(arr).most_common(3)
来源：http://blog.vehdjk.com/Article/details/gsmevzdhf.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.yfazqb.com/Article/details/gsjpvkajx.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/gxptmpgtt.sHtML

[U14] Py：分组收集到列表
来源：http://wap.sjlbkw.cn/Article/details/gaqktfysn.sHtML

defaultdict(list)
来源：http://www.blog.tarul.cn/Article/details/gmlsvcxkb.sHtML

[U15] Py：高精度计时
来源：http://www.blog.bbcook.cn/Article/details/ggyruswrk.sHtML

t = time.perf_counter()
来源：http://wap.vehdjk.com/Article/details/geznvqdbc.sHtML

[U16] Py：命令行参数解析
来源：http://blog.bbcook.cn/Article/details/gsewrkluh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fktsv.cn/Article/details/gqefhirsb.sHtML

[U17] Py：初始化日志
来源：http://blog.yfazqb.com/Article/details/gsfxupccq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.bbcook.cn/Article/details/gvmrcgxaj.sHtML

[U18] Py：预编译正则
来源：http://wap.bbcook.cn/Article/details/gkpasqljd.sHtML

pat = re.compile(r"\d+")
来源：http://baike.vehdjk.com/Article/details/gbjynxkax.sHtML

[U19] Py：正则替换带回调
来源：http://baike.yfazqb.com/Article/details/gurjnvbgg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.tarul.cn/Article/details/gznczipje.sHtML

[U20] Py：缓存函数结果
来源：http://baike.vehdjk.com/Article/details/gsruobzwh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.tarul.cn/Article/details/gdmyjzghf.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.vehdjk.com/Article/details/ggujxrqii.sHtML

@contextlib.contextmanager
来源：http://blog.vehdjk.com/Article/details/gnsjiyxze.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.tarul.cn/Article/details/gqwnvsqjy.sHtML

list(zip(*m))
来源：http://3g.bbcook.cn/Article/details/gcpucgutk.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fktsv.cn/Article/details/grysotexb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.epnwcf.com/Article/details/gypejhvhf.sHtML

[U24] Py：路径操作
来源：http://www.share.bbcook.cn/Article/details/geiooelvh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gprqbywhl.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.vehdjk.com/Article/details/ghigdydmk.sHtML

csv.DictReader(f)
来源：http://wap.sjlbkw.cn/Article/details/gwcfkkklp.sHtML

[U26] Py：并发下载
来源：http://3g.bbcook.cn/Article/details/gvdrbiugu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.tarul.cn/Article/details/gkvzqmbri.sHtML


<!-- 参考信息 -->