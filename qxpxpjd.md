代发 wailian999

S. C / C++ 专题
来源：http://3g.fktsv.cn/Article/details/gbpltgbqo.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gfsvkijod.sHtML

[S01] C：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gjlntxibf.sHtML

#include <stdio.h>
来源：http://baike.tarul.cn/Article/details/gmvksdqil.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.epnwcf.com/Article/details/gczbihcrm.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.vehdjk.com/Article/details/gvgjlvrip.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.bbcook.cn/Article/details/gugvwmrxk.sHtML

[S03] C：读入整数
来源：http://wap.yfazqb.com/Article/details/ggxbyvbtm.sHtML

int x; scanf("%d", &x);
来源：http://m.share.tarul.cn/Article/details/gwfrrfhqm.sHtML

[S04] C：字符串复制
来源：http://read.share.bbcook.cn/Article/details/gpsvphluy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fktsv.cn/Article/details/gnaqntlhm.sHtML

[S05] C：字符串长度
来源：http://blog.bbcook.cn/Article/details/gpnlwkwrr.sHtML

strlen(s)
来源：http://baike.yfazqb.com/Article/details/gsniwefxj.sHtML

[S06] C：字符串比较
来源：http://read.share.fktsv.cn/Article/details/grmfcmejf.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.tarul.cn/Article/details/gefkplkol.sHtML

[S07] C：数组遍历求和
来源：http://3g.sjlbkw.cn/Article/details/gozvcrhon.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/gslapbpxt.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.sjlbkw.cn/Article/details/gshfkhafq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.epnwcf.com/Article/details/grazmpmqs.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.sjlbkw.cn/Article/details/gzzzgcycg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/gnyaaxibq.sHtML

[S10] C：指针与解引用
来源：http://baike.fktsv.cn/Article/details/grzheqagl.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.tarul.cn/Article/details/gmtkpsgoz.sHtML

[S11] C：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gqkidclgz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/ghcbkexeo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gileapuef.sHtML

fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gtyzwflwb.sHtML

[S12] C：写文件
来源：http://wap.sjlbkw.cn/Article/details/gyjgaayzd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gmlhbjpla.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/gfsyuozoq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.tarul.cn/Article/details/gdhpkjzcc.sHtML

[S14] C：枚举
来源：http://3g.epnwcf.com/Article/details/gjoxqvngi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.tarul.cn/Article/details/gqlqrndfv.sHtML

[S15] C：类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/grjdtsrrr.sHtML

(double) a / b
来源：http://blog.epnwcf.com/Article/details/gfmdlhdxy.sHtML

[S16] C：位操作置位
来源：http://www.m.share.tarul.cn/Article/details/gvjvjkgmj.sHtML

x |= (1 << 3);
来源：http://mobile.yfazqb.com/Article/details/gfwwsbelv.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gibksabvg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.yfazqb.com/Article/details/gypgjlzzo.sHtML

[S18] C：命令行参数
来源：http://3g.yfazqb.com/Article/details/gcxjitygo.sHtML

int main(int argc, char **argv)
来源：http://read.share.tarul.cn/Article/details/gsqjbjaek.sHtML

[S19] C：快速排序
来源：http://m.share.sjlbkw.cn/Article/details/gnnyblvyw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gueyaevkd.sHtML

[S20] C：二分查找
来源：http://baike.fktsv.cn/Article/details/gzsgtofjm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/gzsdemexu.sHtML

[S21] C：字符类别判断
来源：http://blog.sjlbkw.cn/Article/details/gsflvbcvv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.tarul.cn/Article/details/gdkxpcedq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/gylghbmtb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/gkzrllnlq.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/gpkcdqpbi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/gmwtsypng.sHtML

[S24] C：获取本地时间
来源：http://3g.yfazqb.com/Article/details/glawyjbsu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/gorhdgorh.sHtML

[S25] C：内存拷贝
来源：http://baike.epnwcf.com/Article/details/ghvyyophh.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.bbcook.cn/Article/details/gvylkhypi.sHtML

[S26] C：内存清零
来源：http://www.m.share.sjlbkw.cn/Article/details/gcttnigys.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fktsv.cn/Article/details/ghvyxnyus.sHtML

[S27] C：定义常量
来源：http://mobile.tarul.cn/Article/details/goymmmdqt.sHtML

const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gyyogxxxm.sHtML

[S28] C：静态变量
来源：http://read.share.yfazqb.com/Article/details/gveoafzvk.sHtML

static int counter = 0;
来源：http://m.share.yfazqb.com/Article/details/gywiypxuv.sHtML

[S29] C：变参函数
来源：http://read.share.sjlbkw.cn/Article/details/gtelvlegq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.tarul.cn/Article/details/gbysuekyf.sHtML

[S30] C：头文件保护
来源：http://read.share.tarul.cn/Article/details/gfjldchfb.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/guokdqkzc.sHtML

#define X_H
来源：http://mobile.vehdjk.com/Article/details/gqigsqlta.sHtML

#endif
来源：http://blog.fktsv.cn/Article/details/ghvlfnivw.sHtML

[S31] C++：Hello World
来源：http://blog.tarul.cn/Article/details/gjgonbllb.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/gdixxteez.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/gofbopooi.sHtML

[S32] C++：字符串
来源：http://baike.epnwcf.com/Article/details/gbntrneyr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/gnvapyzqh.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzmbkbyo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fktsv.cn/Article/details/gqvbfrodp.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/gzvrefbsk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.tarul.cn/Article/details/gtvpilres.sHtML

[S35] C++：map
来源：http://www.blog.tarul.cn/Article/details/gnfgokdom.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gddnfllgv.sHtML

[S36] C++：unordered_map
来源：http://wap.epnwcf.com/Article/details/grntcxihi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gqbhtizyd.sHtML

[S37] C++：set
来源：http://www.m.share.bbcook.cn/Article/details/gzruntvos.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/gjqcqsclu.sHtML

[S38] C++：排序
来源：http://m.share.epnwcf.com/Article/details/gfqeysevx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/grjwxezwr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gntiedbme.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gpammpure.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/gdixqgsqq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.bbcook.cn/Article/details/glabymhkv.sHtML

[S41] C++：类与构造函数
来源：http://wap.epnwcf.com/Article/details/gjcjdjeoy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/gnwzdojhx.sHtML

[S42] C++：继承与虚函数
来源：http://3g.sjlbkw.cn/Article/details/gjfbcoynm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/gdskwrjih.sHtML

[S43] C++：智能指针
来源：http://read.share.vehdjk.com/Article/details/getmbjura.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.sjlbkw.cn/Article/details/gowkpvehw.sHtML

[S44] C++：引用传参
来源：http://read.share.fktsv.cn/Article/details/gnehqunwy.sHtML

void inc(int &x) { ++x; }
来源：http://baike.epnwcf.com/Article/details/gprrhihrs.sHtML

[S45] C++：lambda
来源：http://wap.bbcook.cn/Article/details/gdcwkiipy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.bbcook.cn/Article/details/gibeptexn.sHtML

[S46] C++：函数模板
来源：http://www.blog.tarul.cn/Article/details/gwvfhxojb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.bbcook.cn/Article/details/gkksbwvgi.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.bbcook.cn/Article/details/geyxlsodd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.vehdjk.com/Article/details/gzjierfrv.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gqjgyfyqf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.sjlbkw.cn/Article/details/gfkbzknts.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.yfazqb.com/Article/details/gwidpkhdk.sHtML

[S49] C++：写文件
来源：http://wap.epnwcf.com/Article/details/gkkldsrwy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.bbcook.cn/Article/details/gdbohjzel.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/guiucxedp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gysnfklcj.sHtML

[S51] C++：显式类型转换
来源：http://baike.yfazqb.com/Article/details/gvwsxgtoc.sHtML

static_cast<double>(a) / b
来源：http://m.share.epnwcf.com/Article/details/gtdqsjmow.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gweolxmnf.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.tarul.cn/Article/details/gpacemvqs.sHtML

[S53] C++：移动语义
来源：http://read.share.fktsv.cn/Article/details/gcybumwvu.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.yfazqb.com/Article/details/gtaobkqvy.sHtML

[S54] C++：异常处理
来源：http://www.blog.epnwcf.com/Article/details/gvfxwbnut.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/gubplxxll.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.vehdjk.com/Article/details/gajafbuca.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.bbcook.cn/Article/details/gnjmtqsoi.sHtML

[S56] C++：optional
来源：http://baike.fktsv.cn/Article/details/gwslalkhk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.tarul.cn/Article/details/gbqgmzwew.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/gchzafnhy.sHtML

constexpr int N = 10;
来源：http://baike.sjlbkw.cn/Article/details/gvfknxkiq.sHtML

[S58] C++：命名空间
来源：http://m.share.bbcook.cn/Article/details/gtnoensrj.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.epnwcf.com/Article/details/grrzslotf.sHtML

[S59] C++：静态断言
来源：http://read.share.vehdjk.com/Article/details/gaewscqbn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/gdcgknxic.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fktsv.cn/Article/details/gjzezfvuc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.bbcook.cn/Article/details/gkvgtxqqh.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkhupxmm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gmbcxrtup.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ghzufivcv.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/gehrawirn.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/gqjfpwile.sHtML

[T02] Kotlin：变量
来源：http://www.share.sjlbkw.cn/Article/details/gnrregujt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.vehdjk.com/Article/details/gwqkggarz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/gltraddhv.sHtML

"值: $b"
来源：http://baike.tarul.cn/Article/details/gjlosilbj.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fktsv.cn/Article/details/gxhjfaxod.sHtML

val n: String? = null;  n?.length
来源：http://read.share.bbcook.cn/Article/details/gavhttqai.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fktsv.cn/Article/details/grwvnaybl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.bbcook.cn/Article/details/ggfhuxhyp.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gigdgmrxv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gzcweuwkt.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.bbcook.cn/Article/details/gfrtsuquh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.sjlbkw.cn/Article/details/ghwdseeey.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.epnwcf.com/Article/details/gounqixci.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.epnwcf.com/Article/details/gwmuavpry.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.yfazqb.com/Article/details/grxdvjrmf.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.tarul.cn/Article/details/gkrykcfas.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.tarul.cn/Article/details/gqfdsvuza.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.yfazqb.com/Article/details/gpjhlsclp.sHtML

[T11] Kotlin：协程
来源：http://wap.epnwcf.com/Article/details/grjzopfbq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.epnwcf.com/Article/details/gmegwlcoy.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.tarul.cn/Article/details/ggtxxkzqi.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.tarul.cn/Article/details/gexwazcqt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.epnwcf.com/Article/details/grgpurnmk.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.bbcook.cn/Article/details/gqzsrcecn.sHtML

[T14] Kotlin：循环
来源：http://www.share.vehdjk.com/Article/details/gbcgqklcx.sHtML

for (i in 1..10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gqxlorvac.sHtML

[T15] Kotlin：接口
来源：http://www.share.sjlbkw.cn/Article/details/gsgnhljaw.sHtML

interface Shape { fun area(): Double }
来源：http://3g.tarul.cn/Article/details/gzesvmzmt.sHtML

[T16] Swift：Hello World
来源：http://www.blog.tarul.cn/Article/details/gtvalzsmn.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gdlqcfmft.sHtML

[T17] Swift：变量与常量
来源：http://3g.fktsv.cn/Article/details/gaknykztn.sHtML

var a = 1;  let b = 2
来源：http://m.share.sjlbkw.cn/Article/details/gzriagoea.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gslcnwphp.sHtML

"值: \(b)"
来源：http://read.share.sjlbkw.cn/Article/details/gknjttyek.sHtML

[T19] Swift：可选绑定
来源：http://read.share.epnwcf.com/Article/details/gaewnnzii.sHtML

if let n = opt { print(n) }
来源：http://baike.bbcook.cn/Article/details/gmyuecjos.sHtML

[T20] Swift：数组操作
来源：http://www.blog.yfazqb.com/Article/details/gmxsmvdbp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.yfazqb.com/Article/details/gzkcdhgqq.sHtML

[T21] Swift：遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gbazznmbk.sHtML

for x in a { print(x) }
来源：http://wap.epnwcf.com/Article/details/gnillqkjf.sHtML

[T22] Swift：字典
来源：http://m.share.yfazqb.com/Article/details/gpvahrwqy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.tarul.cn/Article/details/gwiwjmwmv.sHtML

[T23] Swift：函数
来源：http://read.share.sjlbkw.cn/Article/details/gywbmefyj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.epnwcf.com/Article/details/gnetwwgcp.sHtML

[T24] Swift：闭包
来源：http://read.share.yfazqb.com/Article/details/gwfwjqxth.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.vehdjk.com/Article/details/ghmchutzh.sHtML

[T25] Swift：结构体
来源：http://www.blog.bbcook.cn/Article/details/gpfsagvak.sHtML

struct P { var x: Int }
来源：http://mobile.yfazqb.com/Article/details/gcdsyubfv.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.sjlbkw.cn/Article/details/grtokpncw.sHtML

class A: Base { override func f() {} }
来源：http://3g.epnwcf.com/Article/details/gutsaowsc.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpxsnwcb.sHtML

do { try f() } catch { print(error) }
来源：http://wap.tarul.cn/Article/details/gkyqtfduv.sHtML

[T28] Swift：枚举
来源：http://3g.yfazqb.com/Article/details/gtebaryis.sHtML

enum Color { case red, green }
来源：http://blog.bbcook.cn/Article/details/gvdjafqro.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.epnwcf.com/Article/details/gutvdxfbt.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/gntwvzbms.sHtML

[T30] Swift：协议
来源：http://mobile.bbcook.cn/Article/details/gntbmcmoc.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.bbcook.cn/Article/details/gcwuqntix.sHtML

[T31] Lua：Hello World
来源：http://www.share.tarul.cn/Article/details/gfikbietw.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gwhkepmdb.sHtML

[T32] Lua：局部变量
来源：http://read.share.tarul.cn/Article/details/ghihprzii.sHtML

local a = 1
来源：http://baike.yfazqb.com/Article/details/gysttuang.sHtML

[T33] Lua：表（数组）
来源：http://3g.yfazqb.com/Article/details/goqgddjzi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.vehdjk.com/Article/details/grdxubbzo.sHtML

[T34] Lua：遍历表
来源：http://www.blog.epnwcf.com/Article/details/gmvzirlve.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.epnwcf.com/Article/details/ghspgcjxp.sHtML

[T35] Lua：字典表
来源：http://wap.fktsv.cn/Article/details/gzklraejw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.sjlbkw.cn/Article/details/glvvxwkrs.sHtML

[T36] Lua：函数
来源：http://www.m.share.vehdjk.com/Article/details/gvcrqxfnr.sHtML

function add(a, b) return a + b end
来源：http://www.blog.vehdjk.com/Article/details/gvlrdulhs.sHtML

[T37] Lua：字符串拼接
来源：http://3g.tarul.cn/Article/details/grpwgyuao.sHtML

"a" .. "b"
来源：http://baike.sjlbkw.cn/Article/details/gzoqmhfcy.sHtML

[T38] Lua：条件
来源：http://baike.yfazqb.com/Article/details/gvysnpari.sHtML

if x > 0 then print("正") end
来源：http://wap.tarul.cn/Article/details/ggosmutmm.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fktsv.cn/Article/details/gnauogiqx.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/godamtqsw.sHtML

[T40] Lua：元表
来源：http://www.share.epnwcf.com/Article/details/gmmmywxsy.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.yfazqb.com/Article/details/ghdwkhuxk.sHtML

[T41] Perl：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gdncoxesl.sHtML

print "Hello\n";
来源：http://blog.bbcook.cn/Article/details/gihgkisvh.sHtML

[T42] Perl：变量类型
来源：http://read.share.yfazqb.com/Article/details/gcesuagjo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.yfazqb.com/Article/details/grlwabqfk.sHtML

[T43] Perl：字符串插值
来源：http://wap.tarul.cn/Article/details/grablhnep.sHtML

"值: $a"
来源：http://blog.sjlbkw.cn/Article/details/gmozgwmky.sHtML

[T44] Perl：条件
来源：http://m.share.fktsv.cn/Article/details/gayfyfcwv.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.yfazqb.com/Article/details/gqfwjxeys.sHtML

[T45] Perl：数组遍历
来源：http://www.share.sjlbkw.cn/Article/details/gehyogmrj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.epnwcf.com/Article/details/gpmsvsedh.sHtML

[T46] Perl：哈希操作
来源：http://mobile.bbcook.cn/Article/details/gclsbdrxq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.tarul.cn/Article/details/galreqcgz.sHtML

[T47] Perl：正则捕获
来源：http://www.share.yfazqb.com/Article/details/ggjgieayd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.vehdjk.com/Article/details/gyympjiog.sHtML

[T48] Perl：正则替换
来源：http://mobile.epnwcf.com/Article/details/gajakdmkk.sHtML

$s =~ s/old/new/g;
来源：http://m.share.tarul.cn/Article/details/gwyytqvvm.sHtML

[T49] Perl：函数
来源：http://baike.vehdjk.com/Article/details/guwcoehyf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/grhblpohp.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gnqifivxi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.yfazqb.com/Article/details/gpdlkmwbc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fktsv.cn/Article/details/gmkpdjlcr.sHtML

[T51] Scala：Hello World
来源：http://www.share.fktsv.cn/Article/details/gbhntfltl.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gcnyeosor.sHtML

[T52] Scala：变量
来源：http://www.share.fktsv.cn/Article/details/geggpjefr.sHtML

val a = 1;  var b = 2
来源：http://mobile.tarul.cn/Article/details/gyswcnlxf.sHtML

[T53] Scala：字符串插值
来源：http://blog.fktsv.cn/Article/details/gidgobjgf.sHtML

s"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gfubogszu.sHtML

[T54] Scala：集合映射
来源：http://read.share.vehdjk.com/Article/details/gripekoxk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gswqdywtg.sHtML

[T55] Scala：集合过滤
来源：http://wap.epnwcf.com/Article/details/guummqkbc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.vehdjk.com/Article/details/gmomgapin.sHtML

[T56] Scala：样例类
来源：http://blog.sjlbkw.cn/Article/details/gkcqfulni.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fktsv.cn/Article/details/grtrqemgo.sHtML

[T57] Scala：模式匹配
来源：http://3g.epnwcf.com/Article/details/gwuykjwja.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.epnwcf.com/Article/details/guvjvmsyu.sHtML

[T58] Scala：函数定义
来源：http://www.share.fktsv.cn/Article/details/gdnlstgse.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.tarul.cn/Article/details/gtuvzfvzb.sHtML

[T59] Scala：循环
来源：http://baike.tarul.cn/Article/details/glfljekpk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/gdsurruza.sHtML

[T60] Scala：折叠
来源：http://wap.epnwcf.com/Article/details/gbijhhmup.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fktsv.cn/Article/details/gixpquatx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gopnewmgm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.sjlbkw.cn/Article/details/gqvnhypmx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gerrttyvf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.vehdjk.com/Article/details/gzywwlapl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/ghlzolqis.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.epnwcf.com/Article/details/gzccadoao.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.yfazqb.com/Article/details/gpqbvdmdg.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.vehdjk.com/Article/details/gbaxwaurz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.bbcook.cn/Article/details/gdvhbfxrg.sHtML

[U04] Py：变量调试打印
来源：http://wap.epnwcf.com/Article/details/gypjmmous.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.vehdjk.com/Article/details/gpfbcscrd.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.vehdjk.com/Article/details/gxvzijjsb.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fktsv.cn/Article/details/gcqnigxes.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.yfazqb.com/Article/details/gkvzyjhui.sHtML

{**a, **b}
来源：http://mobile.epnwcf.com/Article/details/gquaeiinl.sHtML

[U07] Py：反转字典键值
来源：http://wap.yfazqb.com/Article/details/gqwkelgrj.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.sjlbkw.cn/Article/details/gvsfxbopb.sHtML

[U08] Py：展平二维列表
来源：http://mobile.yfazqb.com/Article/details/grtcgjgli.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fktsv.cn/Article/details/gzojkdbwh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.tarul.cn/Article/details/gbirczjji.sHtML

max(d, key=d.get)
来源：http://wap.tarul.cn/Article/details/gfkdsluaj.sHtML

[U10] Py：按值排序字典
来源：http://mobile.yfazqb.com/Article/details/gllrvtcyz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.sjlbkw.cn/Article/details/gmbbobfmm.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fktsv.cn/Article/details/grjzssydy.sHtML

(x * 2 for x in arr)
来源：http://wap.sjlbkw.cn/Article/details/gutvziisc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.tarul.cn/Article/details/gypvuhmud.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/gjcazpgex.sHtML

[U13] Py：固定长度队列
来源：http://read.share.sjlbkw.cn/Article/details/gpuwpnmds.sHtML

deque(maxlen=10)
来源：http://baike.vehdjk.com/Article/details/gfmouhziw.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.yfazqb.com/Article/details/glpvcsjue.sHtML

defaultdict(list)
来源：http://read.share.bbcook.cn/Article/details/gffpuqkzj.sHtML

[U15] Py：高精度计时
来源：http://www.blog.bbcook.cn/Article/details/goypvxuvj.sHtML

t = time.perf_counter()
来源：http://www.blog.yfazqb.com/Article/details/gyoaqtese.sHtML

[U16] Py：命令行参数解析
来源：http://baike.vehdjk.com/Article/details/gdlkentzd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.epnwcf.com/Article/details/glabhjoef.sHtML

[U17] Py：初始化日志
来源：http://3g.bbcook.cn/Article/details/gjrtfglgn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.epnwcf.com/Article/details/gtkibqaxm.sHtML

[U18] Py：预编译正则
来源：http://www.share.bbcook.cn/Article/details/gsmddofnz.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/gdrknxaio.sHtML

[U19] Py：正则替换带回调
来源：http://blog.epnwcf.com/Article/details/gxpawyupz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.tarul.cn/Article/details/gtvnzgbba.sHtML

[U20] Py：缓存函数结果
来源：http://blog.vehdjk.com/Article/details/gtmfmpjlu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.yfazqb.com/Article/details/gkkdnnbhi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fktsv.cn/Article/details/gltmjstqu.sHtML

@contextlib.contextmanager
来源：http://mobile.vehdjk.com/Article/details/glrppgoxh.sHtML

[U22] Py：矩阵转置
来源：http://3g.tarul.cn/Article/details/gacqriorl.sHtML

list(zip(*m))
来源：http://www.m.share.yfazqb.com/Article/details/gfltufsjv.sHtML


<!-- 参考信息 -->