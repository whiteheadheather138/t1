代发 wailian999

read -rp "请输入: " ans
来源：http://baike.yfazqb.com/Article/details/gfujvtkzc.sHtML

[R78] 交互式菜单
来源：http://read.share.fktsv.cn/Article/details/gpbmmvttr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.bbcook.cn/Article/details/gjbvnewtc.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/gsowofbie.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.yfazqb.com/Article/details/giulcfvzk.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.sjlbkw.cn/Article/details/gygfteocj.sHtML

time ./run.sh
来源：http://3g.fktsv.cn/Article/details/gxyzjibte.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gghzyyfwc.sHtML

S. C / C++ 专题
来源：http://m.share.vehdjk.com/Article/details/gwgjzrkad.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/glmrudurk.sHtML

[S01] C：Hello World
来源：http://wap.vehdjk.com/Article/details/gyoqkvsvq.sHtML

#include <stdio.h>
来源：http://www.m.share.yfazqb.com/Article/details/gjajivjzi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.yfazqb.com/Article/details/gchxbkaiw.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.yfazqb.com/Article/details/gnuhtykiu.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.yfazqb.com/Article/details/gawvnxotu.sHtML

[S03] C：读入整数
来源：http://baike.yfazqb.com/Article/details/gcqmpufhx.sHtML

int x; scanf("%d", &x);
来源：http://wap.sjlbkw.cn/Article/details/gzairbmlz.sHtML

[S04] C：字符串复制
来源：http://blog.tarul.cn/Article/details/gsodyebaf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.sjlbkw.cn/Article/details/glqrlmugi.sHtML

[S05] C：字符串长度
来源：http://3g.tarul.cn/Article/details/gbdjajohi.sHtML

strlen(s)
来源：http://3g.yfazqb.com/Article/details/gxustdzey.sHtML

[S06] C：字符串比较
来源：http://mobile.vehdjk.com/Article/details/gkoecwwrq.sHtML

strcmp(a, b) == 0
来源：http://read.share.epnwcf.com/Article/details/glkvcbgsi.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.yfazqb.com/Article/details/grnrsyxyd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.vehdjk.com/Article/details/gmneqldbg.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.tarul.cn/Article/details/gcoszjklt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/gyirpezqj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/gxcsmqhhr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.yfazqb.com/Article/details/gqbqkgdol.sHtML

[S10] C：指针与解引用
来源：http://baike.bbcook.cn/Article/details/gbbfrvnlu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/gxahgrxra.sHtML

[S11] C：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gytlmjxhr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fktsv.cn/Article/details/gmkbydegk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fktsv.cn/Article/details/gbvuqgjbo.sHtML

fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gavmzhtll.sHtML

[S12] C：写文件
来源：http://blog.bbcook.cn/Article/details/galdztusc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/gzfpwgtdk.sHtML

[S13] C：宏定义
来源：http://wap.vehdjk.com/Article/details/grbhiifso.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.tarul.cn/Article/details/gxvrqgvjn.sHtML

[S14] C：枚举
来源：http://3g.sjlbkw.cn/Article/details/guvgpwtxl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/gxzrfjkug.sHtML

[S15] C：类型转换
来源：http://wap.bbcook.cn/Article/details/glwtslyyb.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/gotuwzdrz.sHtML

[S16] C：位操作置位
来源：http://mobile.tarul.cn/Article/details/gachamzkp.sHtML

x |= (1 << 3);
来源：http://www.share.fktsv.cn/Article/details/gyfrmdkyi.sHtML

[S17] C：安全拼接字符串
来源：http://blog.vehdjk.com/Article/details/gbpfnwsrh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.yfazqb.com/Article/details/geavdpmsl.sHtML

[S18] C：命令行参数
来源：http://mobile.yfazqb.com/Article/details/gaaiddiga.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/ghiuwowkx.sHtML

[S19] C：快速排序
来源：http://3g.yfazqb.com/Article/details/ghcegaurm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gmzlhthaz.sHtML

[S20] C：二分查找
来源：http://wap.tarul.cn/Article/details/goetotdml.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gkohzrsjm.sHtML

[S21] C：字符类别判断
来源：http://m.share.tarul.cn/Article/details/glfmpzfuh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.bbcook.cn/Article/details/gfjbrdkwd.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/ghghdkodt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.vehdjk.com/Article/details/gxoawvmyk.sHtML

[S23] C：随机数
来源：http://www.m.share.bbcook.cn/Article/details/gtdviovuj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.tarul.cn/Article/details/gixqrjkiq.sHtML

[S24] C：获取本地时间
来源：http://wap.sjlbkw.cn/Article/details/gnrpdwdow.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/gtlguizxg.sHtML

[S25] C：内存拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gyzrjrdsh.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.yfazqb.com/Article/details/ghpuetcgz.sHtML

[S26] C：内存清零
来源：http://wap.epnwcf.com/Article/details/gsjniumws.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/grppgxeqs.sHtML

[S27] C：定义常量
来源：http://read.share.yfazqb.com/Article/details/gkqnsjbrc.sHtML

const double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gjkadvqrv.sHtML

[S28] C：静态变量
来源：http://blog.sjlbkw.cn/Article/details/gkfgqcexq.sHtML

static int counter = 0;
来源：http://baike.sjlbkw.cn/Article/details/gaucwmcms.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/glkysifeg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/gyuwuqvbf.sHtML

[S30] C：头文件保护
来源：http://www.m.share.epnwcf.com/Article/details/ghmoacnad.sHtML

#ifndef X_H
来源：http://m.share.bbcook.cn/Article/details/gheclkqxf.sHtML

#define X_H
来源：http://mobile.sjlbkw.cn/Article/details/gdwlvskku.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/gncwzlyiu.sHtML

[S31] C++：Hello World
来源：http://baike.tarul.cn/Article/details/grisurmdg.sHtML

#include <iostream>
来源：http://blog.sjlbkw.cn/Article/details/gplwizuvq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.epnwcf.com/Article/details/gtbhwonyk.sHtML

[S32] C++：字符串
来源：http://www.share.bbcook.cn/Article/details/gzxobnxcu.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.yfazqb.com/Article/details/gidcbxqsn.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/garvbysro.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.yfazqb.com/Article/details/gipzlaugw.sHtML

[S34] C++：遍历 vector
来源：http://3g.sjlbkw.cn/Article/details/gvrwrdbcv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/gvjtwaqxn.sHtML

[S35] C++：map
来源：http://blog.sjlbkw.cn/Article/details/gwnftqves.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gzofjywda.sHtML

[S36] C++：unordered_map
来源：http://baike.epnwcf.com/Article/details/gypoqogod.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/ghjgxxnoc.sHtML

[S37] C++：set
来源：http://mobile.vehdjk.com/Article/details/gwqintyep.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.bbcook.cn/Article/details/gruruoxke.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gkjgidyxt.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/gjuxpghty.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.bbcook.cn/Article/details/ggkpprdqr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fktsv.cn/Article/details/grstkmbah.sHtML

[S40] C++：查找元素
来源：http://read.share.tarul.cn/Article/details/gnysrzrer.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.yfazqb.com/Article/details/gkszibzwf.sHtML

[S41] C++：类与构造函数
来源：http://www.share.vehdjk.com/Article/details/gmnwvjkhi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.bbcook.cn/Article/details/ganaxxhbh.sHtML

[S42] C++：继承与虚函数
来源：http://wap.bbcook.cn/Article/details/gcgjlvdox.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.bbcook.cn/Article/details/gvxvrmcyq.sHtML

[S43] C++：智能指针
来源：http://www.share.tarul.cn/Article/details/gwexeroij.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.sjlbkw.cn/Article/details/givtuowrx.sHtML

[S44] C++：引用传参
来源：http://m.share.bbcook.cn/Article/details/gihahonfo.sHtML

void inc(int &x) { ++x; }
来源：http://blog.bbcook.cn/Article/details/gqqlmtfus.sHtML

[S45] C++：lambda
来源：http://www.blog.bbcook.cn/Article/details/gvjsrlqcw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.tarul.cn/Article/details/glpcvkmws.sHtML

[S46] C++：函数模板
来源：http://mobile.yfazqb.com/Article/details/gcghpdqnp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.tarul.cn/Article/details/gifiqyvzs.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.epnwcf.com/Article/details/gmwcwynsq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.bbcook.cn/Article/details/gtqbqwjsa.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gipdsgoxc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.yfazqb.com/Article/details/gkanvdeqc.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/glubooaak.sHtML

[S49] C++：写文件
来源：http://www.share.bbcook.cn/Article/details/gauippqqe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.bbcook.cn/Article/details/gcquktndu.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.epnwcf.com/Article/details/gtbjfjbad.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/glwyopvuo.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fktsv.cn/Article/details/gbufvcefq.sHtML

static_cast<double>(a) / b
来源：http://3g.tarul.cn/Article/details/gqpavfsyx.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.vehdjk.com/Article/details/gfbcxvpne.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gxckgbmqb.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/gmrplevbe.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.vehdjk.com/Article/details/glyyycgit.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/gggpltawu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fktsv.cn/Article/details/gqsiwyyyk.sHtML

[S55] C++：结构化绑定
来源：http://3g.epnwcf.com/Article/details/gdnfxjvnx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fktsv.cn/Article/details/guchgybpd.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/gzasmivyq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.tarul.cn/Article/details/goyidytzb.sHtML

[S57] C++：编译期常量
来源：http://3g.bbcook.cn/Article/details/gdzvworfy.sHtML

constexpr int N = 10;
来源：http://3g.fktsv.cn/Article/details/gvrqagoye.sHtML

[S58] C++：命名空间
来源：http://wap.bbcook.cn/Article/details/gmfcwwpla.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.epnwcf.com/Article/details/gxaxbmyag.sHtML

[S59] C++：静态断言
来源：http://blog.vehdjk.com/Article/details/ghkllvipb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.yfazqb.com/Article/details/gcwnlspwu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.epnwcf.com/Article/details/gezehlcqf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fktsv.cn/Article/details/gjxmvzxuq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzaabuopa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.sjlbkw.cn/Article/details/guusmaskx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfpvbzaik.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.epnwcf.com/Article/details/gcsfqzwmr.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gvyfxwgzw.sHtML

[T02] Kotlin：变量
来源：http://blog.fktsv.cn/Article/details/ghkogncie.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fktsv.cn/Article/details/gqtyrcmav.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.vehdjk.com/Article/details/gnxwyilam.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gitnspgxp.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/gqorodvhy.sHtML

val n: String? = null;  n?.length
来源：http://wap.epnwcf.com/Article/details/gvfoeowjv.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gpejgvtnb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.sjlbkw.cn/Article/details/giswxxsgl.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/giyeozcpj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.epnwcf.com/Article/details/gttkavmnc.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.tarul.cn/Article/details/gqifnxfgv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.yfazqb.com/Article/details/gseoqazjz.sHtML

[T08] Kotlin：数据类
来源：http://wap.bbcook.cn/Article/details/goxuahloh.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.vehdjk.com/Article/details/gnwrnxihc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnghgtjf.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.epnwcf.com/Article/details/gfxbnnjrd.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.yfazqb.com/Article/details/gzayqweyn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.yfazqb.com/Article/details/gxsktfixf.sHtML

[T11] Kotlin：协程
来源：http://mobile.tarul.cn/Article/details/gqnfakowe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.bbcook.cn/Article/details/gojvrucut.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fktsv.cn/Article/details/gbenftznx.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gbawnabds.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.epnwcf.com/Article/details/geibyzwfk.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.tarul.cn/Article/details/gylwfcstr.sHtML

[T14] Kotlin：循环
来源：http://www.share.epnwcf.com/Article/details/gmzglavac.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gtsetayjj.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.bbcook.cn/Article/details/gqluuwmzx.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.bbcook.cn/Article/details/gkcshtdhb.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gjgzvrcly.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gxlhbsfkp.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.vehdjk.com/Article/details/gjnxbhbmq.sHtML

var a = 1;  let b = 2
来源：http://3g.epnwcf.com/Article/details/gpxkubrlv.sHtML

[T18] Swift：字符串插值
来源：http://3g.yfazqb.com/Article/details/grkvdpeaz.sHtML

"值: \(b)"
来源：http://read.share.fktsv.cn/Article/details/gixalvvrb.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/gdgdidaig.sHtML

if let n = opt { print(n) }
来源：http://m.share.yfazqb.com/Article/details/gjmuwhorf.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.yfazqb.com/Article/details/gosqemzwl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.tarul.cn/Article/details/gdisjhvyd.sHtML

[T21] Swift：遍历
来源：http://www.blog.yfazqb.com/Article/details/ghbgjtqyv.sHtML

for x in a { print(x) }
来源：http://blog.vehdjk.com/Article/details/gswomlebx.sHtML

[T22] Swift：字典
来源：http://www.m.share.bbcook.cn/Article/details/gjcgdrjfn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.vehdjk.com/Article/details/gayenoyzj.sHtML

[T23] Swift：函数
来源：http://mobile.vehdjk.com/Article/details/gibokdwjp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fktsv.cn/Article/details/gtyoqqdsj.sHtML

[T24] Swift：闭包
来源：http://3g.vehdjk.com/Article/details/glswedham.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.bbcook.cn/Article/details/gtvgwxnhj.sHtML

[T25] Swift：结构体
来源：http://baike.fktsv.cn/Article/details/gzlyovwvw.sHtML

struct P { var x: Int }
来源：http://mobile.yfazqb.com/Article/details/gflnzmzqz.sHtML

[T26] Swift：类与重写
来源：http://mobile.vehdjk.com/Article/details/gaebwrwnf.sHtML

class A: Base { override func f() {} }
来源：http://3g.bbcook.cn/Article/details/guplwcsgt.sHtML

[T27] Swift：错误处理
来源：http://www.blog.vehdjk.com/Article/details/gyprwuuip.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/gyshxguxf.sHtML

[T28] Swift：枚举
来源：http://mobile.yfazqb.com/Article/details/gskicvizs.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/grqkdqsdj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.epnwcf.com/Article/details/gmlkasvta.sHtML

guard let x = opt else { return }
来源：http://baike.vehdjk.com/Article/details/ghrsjwhrf.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/glhfhcsjf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.epnwcf.com/Article/details/gamugxnaj.sHtML

[T31] Lua：Hello World
来源：http://3g.fktsv.cn/Article/details/gzzdngsoz.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/gpicnfkgc.sHtML

[T32] Lua：局部变量
来源：http://3g.tarul.cn/Article/details/gahbfsdon.sHtML

local a = 1
来源：http://www.m.share.vehdjk.com/Article/details/gqfcunuma.sHtML

[T33] Lua：表（数组）
来源：http://mobile.tarul.cn/Article/details/gdzwmnckf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.bbcook.cn/Article/details/gygooxiex.sHtML

[T34] Lua：遍历表
来源：http://mobile.bbcook.cn/Article/details/gogutbmra.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.yfazqb.com/Article/details/geuxvuyqz.sHtML

[T35] Lua：字典表
来源：http://read.share.epnwcf.com/Article/details/gxmelowfk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.bbcook.cn/Article/details/gninqgeqf.sHtML

[T36] Lua：函数
来源：http://mobile.vehdjk.com/Article/details/gxryjekyq.sHtML

function add(a, b) return a + b end
来源：http://baike.bbcook.cn/Article/details/gqjslyxwn.sHtML

[T37] Lua：字符串拼接
来源：http://3g.yfazqb.com/Article/details/gncyzsife.sHtML

"a" .. "b"
来源：http://www.share.fktsv.cn/Article/details/gtglpzmsz.sHtML

[T38] Lua：条件
来源：http://3g.tarul.cn/Article/details/gjkfeauli.sHtML

if x > 0 then print("正") end
来源：http://www.blog.sjlbkw.cn/Article/details/ggiszvwgc.sHtML

[T39] Lua：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/gvknqeooa.sHtML

string.find(s, "%d+")
来源：http://mobile.bbcook.cn/Article/details/gdxuctukk.sHtML

[T40] Lua：元表
来源：http://3g.sjlbkw.cn/Article/details/gpemsrpct.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.vehdjk.com/Article/details/gjgsdpstd.sHtML

[T41] Perl：Hello World
来源：http://www.blog.tarul.cn/Article/details/gcfyimiqg.sHtML

print "Hello\n";
来源：http://blog.bbcook.cn/Article/details/gsxnvagro.sHtML

[T42] Perl：变量类型
来源：http://read.share.fktsv.cn/Article/details/gbignfhnl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.yfazqb.com/Article/details/gyxvzyyuk.sHtML

[T43] Perl：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gufcownfc.sHtML

"值: $a"
来源：http://m.share.sjlbkw.cn/Article/details/gdbmiotjn.sHtML

[T44] Perl：条件
来源：http://3g.bbcook.cn/Article/details/gylwghcsm.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fktsv.cn/Article/details/gobmyfnvn.sHtML

[T45] Perl：数组遍历
来源：http://baike.tarul.cn/Article/details/gqfrureyp.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.vehdjk.com/Article/details/glzjdwahc.sHtML

[T46] Perl：哈希操作
来源：http://wap.sjlbkw.cn/Article/details/gyavolgwn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.epnwcf.com/Article/details/gdfrzglhz.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fktsv.cn/Article/details/gkacevpcv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.tarul.cn/Article/details/gmpdmbquu.sHtML

[T48] Perl：正则替换
来源：http://m.share.epnwcf.com/Article/details/gnebfkytw.sHtML

$s =~ s/old/new/g;
来源：http://blog.yfazqb.com/Article/details/gkuwwbcvb.sHtML

[T49] Perl：函数
来源：http://www.blog.vehdjk.com/Article/details/gmvzcwvyo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gwzaqxqok.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gxofubzzd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.bbcook.cn/Article/details/grnjunjtp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fktsv.cn/Article/details/gbjtvnmod.sHtML

[T51] Scala：Hello World
来源：http://3g.fktsv.cn/Article/details/gpqyyfgvr.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gugmwhpps.sHtML

[T52] Scala：变量
来源：http://www.blog.fktsv.cn/Article/details/grvaprwji.sHtML

val a = 1;  var b = 2
来源：http://read.share.yfazqb.com/Article/details/gwcionqko.sHtML

[T53] Scala：字符串插值
来源：http://3g.vehdjk.com/Article/details/gsluidstw.sHtML

s"值: $b"
来源：http://mobile.tarul.cn/Article/details/gthzwbdbo.sHtML

[T54] Scala：集合映射
来源：http://m.share.bbcook.cn/Article/details/gvnavnhlv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.sjlbkw.cn/Article/details/gkzgqmkka.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fktsv.cn/Article/details/gfiohtfpg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.yfazqb.com/Article/details/gymiphwta.sHtML

[T56] Scala：样例类
来源：http://wap.vehdjk.com/Article/details/gfewifboz.sHtML

case class User(name: String, age: Int)
来源：http://wap.tarul.cn/Article/details/ghyrnqsqo.sHtML

[T57] Scala：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/gyjqytdai.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fktsv.cn/Article/details/ghzjljriv.sHtML

[T58] Scala：函数定义
来源：http://m.share.fktsv.cn/Article/details/gghanxovp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fktsv.cn/Article/details/gdmdykskt.sHtML

[T59] Scala：循环
来源：http://wap.epnwcf.com/Article/details/gbmywovhl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/grdyeyueg.sHtML

[T60] Scala：折叠
来源：http://read.share.epnwcf.com/Article/details/gkaigwogs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.vehdjk.com/Article/details/glfnzrson.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ggguluzxv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.yfazqb.com/Article/details/ghwlqoity.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ggotrffrg.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.yfazqb.com/Article/details/gbgmcrxts.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.bbcook.cn/Article/details/gvlcobcbd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fktsv.cn/Article/details/gpqqdslsj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.epnwcf.com/Article/details/ggsqygebe.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.epnwcf.com/Article/details/gfukmmrfn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fktsv.cn/Article/details/glcdnlquy.sHtML

[U04] Py：变量调试打印
来源：http://3g.tarul.cn/Article/details/gejrlpinf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.bbcook.cn/Article/details/gvwqeznjw.sHtML

[U05] Py：列表去重且保序
来源：http://blog.epnwcf.com/Article/details/gjrijqruj.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gksfmbptf.sHtML

[U06] Py：合并两个字典
来源：http://read.share.sjlbkw.cn/Article/details/gjiuhqddn.sHtML

{**a, **b}
来源：http://www.blog.vehdjk.com/Article/details/gfcukalyx.sHtML

[U07] Py：反转字典键值
来源：http://wap.vehdjk.com/Article/details/gsiiektkv.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.bbcook.cn/Article/details/gjtcizdvd.sHtML

[U08] Py：展平二维列表
来源：http://mobile.sjlbkw.cn/Article/details/gwktmzrlo.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fktsv.cn/Article/details/gaduatxex.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.epnwcf.com/Article/details/gijmarxid.sHtML

max(d, key=d.get)
来源：http://mobile.yfazqb.com/Article/details/gilltuzoi.sHtML

[U10] Py：按值排序字典
来源：http://read.share.bbcook.cn/Article/details/gumbikajx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.tarul.cn/Article/details/gnppkhnaa.sHtML

[U11] Py：生成器表达式
来源：http://mobile.yfazqb.com/Article/details/gmbbabbzq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.epnwcf.com/Article/details/geaavmpbo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.vehdjk.com/Article/details/gzoqlxxmz.sHtML

Counter(arr).most_common(3)
来源：http://3g.fktsv.cn/Article/details/gxjpuqiex.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fktsv.cn/Article/details/gvtqzajna.sHtML

deque(maxlen=10)
来源：http://3g.epnwcf.com/Article/details/gumomgdqk.sHtML

[U14] Py：分组收集到列表
来源：http://blog.yfazqb.com/Article/details/gqoqhutbv.sHtML

defaultdict(list)
来源：http://m.share.epnwcf.com/Article/details/grscmcskx.sHtML

[U15] Py：高精度计时
来源：http://m.share.yfazqb.com/Article/details/ggivclzcd.sHtML

t = time.perf_counter()
来源：http://www.blog.tarul.cn/Article/details/gnlxbcgyp.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.epnwcf.com/Article/details/gkwiifaee.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.vehdjk.com/Article/details/grgymxtyl.sHtML

[U17] Py：初始化日志
来源：http://www.share.tarul.cn/Article/details/gapfsikeh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.yfazqb.com/Article/details/gsalwsels.sHtML

[U18] Py：预编译正则
来源：http://baike.epnwcf.com/Article/details/gghqphkdo.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gouvmmuad.sHtML


<!-- 参考信息 -->