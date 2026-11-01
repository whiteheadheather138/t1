代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gfoljpyhn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/gfvswymjg.sHtML

time ./run.sh
来源：http://mobile.vehdjk.com/Article/details/gqykczvdb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gzzpxnjkv.sHtML

S. C / C++ 专题
来源：http://baike.bbcook.cn/Article/details/gzothviia.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gzpdkwwig.sHtML

[S01] C：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gydipblvf.sHtML

#include <stdio.h>
来源：http://3g.bbcook.cn/Article/details/gnztqfuev.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.bbcook.cn/Article/details/gcqrdnaxx.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.bbcook.cn/Article/details/gkomxpwhw.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.bbcook.cn/Article/details/gagmofrvr.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gcllggfkh.sHtML

int x; scanf("%d", &x);
来源：http://baike.fktsv.cn/Article/details/gmsczwoav.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/gilomspaf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/gbovxreev.sHtML

[S05] C：字符串长度
来源：http://baike.vehdjk.com/Article/details/gqgkedpxb.sHtML

strlen(s)
来源：http://read.share.sjlbkw.cn/Article/details/gyfcklgaz.sHtML

[S06] C：字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gwubsdxfr.sHtML

strcmp(a, b) == 0
来源：http://read.share.vehdjk.com/Article/details/gouqgsufi.sHtML

[S07] C：数组遍历求和
来源：http://read.share.vehdjk.com/Article/details/gdvjbtnaq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.epnwcf.com/Article/details/gjdulkpip.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/gqqesgegg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.sjlbkw.cn/Article/details/gejnoetkp.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.vehdjk.com/Article/details/gpyerdnyp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.yfazqb.com/Article/details/gzgvqrxnd.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/gtncqwgsx.sHtML

int *p = &a;  *p = 5;
来源：http://3g.sjlbkw.cn/Article/details/gcujogvqz.sHtML

[S11] C：逐行读文件
来源：http://wap.vehdjk.com/Article/details/glwxtxjdm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/ghekjkatq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.sjlbkw.cn/Article/details/gpisybsny.sHtML

fclose(f);
来源：http://blog.yfazqb.com/Article/details/gbkmutjnn.sHtML

[S12] C：写文件
来源：http://baike.vehdjk.com/Article/details/gkmxtrwky.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/ggymoiinu.sHtML

[S13] C：宏定义
来源：http://baike.vehdjk.com/Article/details/gvbjnvrdk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gqeccgokb.sHtML

[S14] C：枚举
来源：http://m.share.vehdjk.com/Article/details/gcghtcvlo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.sjlbkw.cn/Article/details/gywiiudex.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/grwexkeks.sHtML

(double) a / b
来源：http://blog.tarul.cn/Article/details/gxwkaxurh.sHtML

[S16] C：位操作置位
来源：http://wap.sjlbkw.cn/Article/details/gdocvgahe.sHtML

x |= (1 << 3);
来源：http://read.share.yfazqb.com/Article/details/gxgystajc.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/gbhsyvugl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.bbcook.cn/Article/details/gajhhjxpy.sHtML

[S18] C：命令行参数
来源：http://baike.epnwcf.com/Article/details/gqevjzowi.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/gdnrrxnix.sHtML

[S19] C：快速排序
来源：http://read.share.tarul.cn/Article/details/gvnfftxxf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gaxaeeyzp.sHtML

[S20] C：二分查找
来源：http://read.share.epnwcf.com/Article/details/gxfwtnpbs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gspwidrzv.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/gftuuawak.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/gcvbibvzz.sHtML

[S22] C：字符串转数字
来源：http://baike.bbcook.cn/Article/details/gueoqmkhu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.sjlbkw.cn/Article/details/geunljrxi.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/giwufeorn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.bbcook.cn/Article/details/gtbkforxt.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.yfazqb.com/Article/details/grfvlszvh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/gkqscnoji.sHtML

[S25] C：内存拷贝
来源：http://www.blog.tarul.cn/Article/details/ggwcfkutd.sHtML

memcpy(dst, src, n);
来源：http://3g.sjlbkw.cn/Article/details/ghnkeiiby.sHtML

[S26] C：内存清零
来源：http://3g.vehdjk.com/Article/details/gyptqcmka.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.bbcook.cn/Article/details/gwpetljbg.sHtML

[S27] C：定义常量
来源：http://m.share.fktsv.cn/Article/details/gaoacuyrc.sHtML

const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gpyfvvzzd.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gkfnvpnzq.sHtML

static int counter = 0;
来源：http://mobile.sjlbkw.cn/Article/details/gdkewthbm.sHtML

[S29] C：变参函数
来源：http://m.share.vehdjk.com/Article/details/gtnbdytvu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.tarul.cn/Article/details/gllrwjklm.sHtML

[S30] C：头文件保护
来源：http://www.blog.bbcook.cn/Article/details/gsrcttbyt.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gvqrssowg.sHtML

#define X_H
来源：http://3g.sjlbkw.cn/Article/details/ggqfnntwg.sHtML

#endif
来源：http://www.share.epnwcf.com/Article/details/gpqfzgkqe.sHtML

[S31] C++：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gjbqqysed.sHtML

#include <iostream>
来源：http://blog.epnwcf.com/Article/details/glahouyuu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.epnwcf.com/Article/details/gsvykcyrr.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/gghwivndq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/grdvsrjgp.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/gkyitezfy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.tarul.cn/Article/details/gqieeuhzp.sHtML

[S34] C++：遍历 vector
来源：http://baike.vehdjk.com/Article/details/gtwckyvsj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.bbcook.cn/Article/details/geigelxcr.sHtML

[S35] C++：map
来源：http://3g.bbcook.cn/Article/details/gqclcmbhe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gmszbernu.sHtML

[S36] C++：unordered_map
来源：http://baike.vehdjk.com/Article/details/gsckmnwsf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gkyzebynj.sHtML

[S37] C++：set
来源：http://www.blog.vehdjk.com/Article/details/gfocjllft.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.sjlbkw.cn/Article/details/gsdpaphqm.sHtML

[S38] C++：排序
来源：http://www.blog.bbcook.cn/Article/details/glfmyurby.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.yfazqb.com/Article/details/gdvdxotkg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.bbcook.cn/Article/details/gtbffiyon.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.yfazqb.com/Article/details/gxntubsdy.sHtML

[S40] C++：查找元素
来源：http://www.blog.epnwcf.com/Article/details/ghzfswmys.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.sjlbkw.cn/Article/details/gvhsnklfo.sHtML

[S41] C++：类与构造函数
来源：http://read.share.epnwcf.com/Article/details/gdfaobyzd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.sjlbkw.cn/Article/details/glfwygybp.sHtML

[S42] C++：继承与虚函数
来源：http://baike.tarul.cn/Article/details/gjoaxpjxu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.bbcook.cn/Article/details/gedkmmhog.sHtML

[S43] C++：智能指针
来源：http://3g.yfazqb.com/Article/details/ghssswwvn.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.sjlbkw.cn/Article/details/glqcamsuo.sHtML

[S44] C++：引用传参
来源：http://blog.sjlbkw.cn/Article/details/gqydoozxr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.sjlbkw.cn/Article/details/guukhjasi.sHtML

[S45] C++：lambda
来源：http://mobile.vehdjk.com/Article/details/gircaxqdl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.vehdjk.com/Article/details/gyiezpezy.sHtML

[S46] C++：函数模板
来源：http://baike.tarul.cn/Article/details/gjvocfbuy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/gndqulqgk.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.sjlbkw.cn/Article/details/gftbhgunn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.bbcook.cn/Article/details/gbroyyosj.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gislmbozv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.sjlbkw.cn/Article/details/grgzaqien.sHtML

while (std::getline(in, line)) { }
来源：http://baike.yfazqb.com/Article/details/gfwluxmou.sHtML

[S49] C++：写文件
来源：http://baike.yfazqb.com/Article/details/gbvtletqa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.epnwcf.com/Article/details/giczxirqp.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/gmwiwonds.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gdyudnydi.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gevrpacyk.sHtML

static_cast<double>(a) / b
来源：http://wap.sjlbkw.cn/Article/details/gifpwmcmr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fktsv.cn/Article/details/gaygqxiyv.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fktsv.cn/Article/details/gyxfzchuq.sHtML

[S53] C++：移动语义
来源：http://blog.yfazqb.com/Article/details/gwpumvfcw.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fktsv.cn/Article/details/gnjdjixmq.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/ggjdtghza.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.vehdjk.com/Article/details/goollhlrj.sHtML

[S55] C++：结构化绑定
来源：http://mobile.yfazqb.com/Article/details/gbexqklsr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.vehdjk.com/Article/details/gwosgywxd.sHtML

[S56] C++：optional
来源：http://baike.vehdjk.com/Article/details/gnqbxdydm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.tarul.cn/Article/details/gwjthyzau.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gvanorlws.sHtML

constexpr int N = 10;
来源：http://wap.vehdjk.com/Article/details/gnzxdxfwu.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/gsncmlhdf.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.sjlbkw.cn/Article/details/ggrrfofsy.sHtML

[S59] C++：静态断言
来源：http://mobile.epnwcf.com/Article/details/gejfetfyf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.epnwcf.com/Article/details/gwkrijmqc.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.yfazqb.com/Article/details/gcubivwol.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.tarul.cn/Article/details/guwfnzxfe.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gylwpwiex.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/gfzqdnqzx.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghflfsgwl.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.tarul.cn/Article/details/gdehdtsjx.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gxxlcetma.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.epnwcf.com/Article/details/gojaoojsm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.tarul.cn/Article/details/giwrzyfut.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/gtwvusabq.sHtML

"值: $b"
来源：http://www.share.fktsv.cn/Article/details/gktmoawky.sHtML

[T04] Kotlin：空安全
来源：http://wap.tarul.cn/Article/details/gtraltmqw.sHtML

val n: String? = null;  n?.length
来源：http://blog.sjlbkw.cn/Article/details/gqnxzfocp.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.vehdjk.com/Article/details/gwgvhtlui.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.yfazqb.com/Article/details/glpomvish.sHtML

[T06] Kotlin：集合映射
来源：http://blog.bbcook.cn/Article/details/goeywogtx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/gsdpdesam.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/getchwxxz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fktsv.cn/Article/details/gxdwasvea.sHtML

[T08] Kotlin：数据类
来源：http://www.share.vehdjk.com/Article/details/gfscofxao.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.epnwcf.com/Article/details/galokpyel.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.tarul.cn/Article/details/gowuvzwqh.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.tarul.cn/Article/details/gnpbjaian.sHtML

[T10] Kotlin：默认参数
来源：http://blog.vehdjk.com/Article/details/gkdgdfump.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.tarul.cn/Article/details/gurwxgiry.sHtML

[T11] Kotlin：协程
来源：http://baike.fktsv.cn/Article/details/ghsnngjjt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.epnwcf.com/Article/details/gskwpfmat.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.sjlbkw.cn/Article/details/glvcjreii.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.yfazqb.com/Article/details/gkhdevcqg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fktsv.cn/Article/details/gjipssxjs.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fktsv.cn/Article/details/gitvgupmd.sHtML

[T14] Kotlin：循环
来源：http://mobile.yfazqb.com/Article/details/gzpyhjytw.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.vehdjk.com/Article/details/gvsmpolyv.sHtML

[T15] Kotlin：接口
来源：http://wap.vehdjk.com/Article/details/gkofbupge.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.yfazqb.com/Article/details/gsiouwubs.sHtML

[T16] Swift：Hello World
来源：http://blog.vehdjk.com/Article/details/gxyhocxww.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/ggaqzoyxc.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.bbcook.cn/Article/details/gcrfvzczk.sHtML

var a = 1;  let b = 2
来源：http://www.share.sjlbkw.cn/Article/details/grhsufoth.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/ggqawsuuz.sHtML

"值: \(b)"
来源：http://wap.bbcook.cn/Article/details/gmzehpwsp.sHtML

[T19] Swift：可选绑定
来源：http://baike.bbcook.cn/Article/details/gbzryiorb.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/gbarzqlkg.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/graklfqst.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.tarul.cn/Article/details/gccvfvqpa.sHtML

[T21] Swift：遍历
来源：http://baike.fktsv.cn/Article/details/goyxlzliu.sHtML

for x in a { print(x) }
来源：http://m.share.tarul.cn/Article/details/giaxivotz.sHtML

[T22] Swift：字典
来源：http://wap.fktsv.cn/Article/details/ghkkxgquz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.vehdjk.com/Article/details/gunttrevw.sHtML

[T23] Swift：函数
来源：http://m.share.epnwcf.com/Article/details/gabctinjn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.sjlbkw.cn/Article/details/gkbnxwbym.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gujgriawd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gywucpqqc.sHtML

[T25] Swift：结构体
来源：http://read.share.vehdjk.com/Article/details/guxiuhywo.sHtML

struct P { var x: Int }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsqfoqfw.sHtML

[T26] Swift：类与重写
来源：http://www.blog.epnwcf.com/Article/details/grncgzplv.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.epnwcf.com/Article/details/gyzdxffrf.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/gcepquyte.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.yfazqb.com/Article/details/gourxnmhy.sHtML

[T28] Swift：枚举
来源：http://wap.sjlbkw.cn/Article/details/gipzlirkf.sHtML

enum Color { case red, green }
来源：http://3g.sjlbkw.cn/Article/details/gbzawclwh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gbcdqpgip.sHtML

guard let x = opt else { return }
来源：http://wap.tarul.cn/Article/details/glesgdjei.sHtML

[T30] Swift：协议
来源：http://3g.yfazqb.com/Article/details/grnuhsiik.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.tarul.cn/Article/details/goznuuncy.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gtucebfji.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/goofavwrs.sHtML

[T32] Lua：局部变量
来源：http://www.blog.yfazqb.com/Article/details/gqysooxog.sHtML

local a = 1
来源：http://m.share.epnwcf.com/Article/details/gdprwdxuq.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/gitjyuoip.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fktsv.cn/Article/details/gobbcpqpg.sHtML

[T34] Lua：遍历表
来源：http://mobile.fktsv.cn/Article/details/glxraxaji.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/gxvdvwscf.sHtML

[T35] Lua：字典表
来源：http://mobile.bbcook.cn/Article/details/gssvsbpbv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.tarul.cn/Article/details/gppgdjoql.sHtML

[T36] Lua：函数
来源：http://wap.vehdjk.com/Article/details/ggwqtwqae.sHtML

function add(a, b) return a + b end
来源：http://mobile.bbcook.cn/Article/details/glipitgvm.sHtML

[T37] Lua：字符串拼接
来源：http://3g.tarul.cn/Article/details/gnqopvuiv.sHtML

"a" .. "b"
来源：http://www.m.share.fktsv.cn/Article/details/gplbsasnk.sHtML

[T38] Lua：条件
来源：http://wap.vehdjk.com/Article/details/gygoemlxb.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.yfazqb.com/Article/details/gomgitraa.sHtML

[T39] Lua：模式匹配
来源：http://read.share.vehdjk.com/Article/details/gdekkyqdr.sHtML

string.find(s, "%d+")
来源：http://baike.tarul.cn/Article/details/gtodfbdqs.sHtML

[T40] Lua：元表
来源：http://m.share.vehdjk.com/Article/details/gwwffuaac.sHtML

setmetatable({}, { __index = base })
来源：http://3g.yfazqb.com/Article/details/gnpjstukn.sHtML

[T41] Perl：Hello World
来源：http://www.share.yfazqb.com/Article/details/gfpjvpixo.sHtML

print "Hello\n";
来源：http://3g.yfazqb.com/Article/details/gbtdbefth.sHtML

[T42] Perl：变量类型
来源：http://3g.tarul.cn/Article/details/gzbctngma.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fktsv.cn/Article/details/gavfeuvnh.sHtML

[T43] Perl：字符串插值
来源：http://wap.vehdjk.com/Article/details/gsjtfawop.sHtML

"值: $a"
来源：http://mobile.epnwcf.com/Article/details/gzzlbyluh.sHtML

[T44] Perl：条件
来源：http://blog.sjlbkw.cn/Article/details/gthlinbpw.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/gjaklpeyl.sHtML

[T45] Perl：数组遍历
来源：http://baike.tarul.cn/Article/details/gpxlkpvbl.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.bbcook.cn/Article/details/ghvhtgfip.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gbhtbzrhd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/gggzlbuex.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.epnwcf.com/Article/details/gotokyuvu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guhekqxnh.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gaxbpseya.sHtML

$s =~ s/old/new/g;
来源：http://blog.yfazqb.com/Article/details/gbskjglmk.sHtML

[T49] Perl：函数
来源：http://blog.epnwcf.com/Article/details/guvgiucuh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gvjfilvef.sHtML

[T50] Perl：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gzebjflym.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.bbcook.cn/Article/details/ghvjqkcfp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.bbcook.cn/Article/details/gnmjvsxxs.sHtML

[T51] Scala：Hello World
来源：http://3g.vehdjk.com/Article/details/gltlbnysl.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gpzajtxpz.sHtML

[T52] Scala：变量
来源：http://baike.sjlbkw.cn/Article/details/goqnrezea.sHtML

val a = 1;  var b = 2
来源：http://blog.yfazqb.com/Article/details/gpgygmlpi.sHtML

[T53] Scala：字符串插值
来源：http://mobile.bbcook.cn/Article/details/glpgesmsl.sHtML

s"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gpgtezemm.sHtML

[T54] Scala：集合映射
来源：http://3g.epnwcf.com/Article/details/gvmskcfkl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.sjlbkw.cn/Article/details/ggwpsilui.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gxsenzfqc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.sjlbkw.cn/Article/details/gevjhotfz.sHtML

[T56] Scala：样例类
来源：http://www.blog.epnwcf.com/Article/details/gwubvrmbe.sHtML

case class User(name: String, age: Int)
来源：http://read.share.tarul.cn/Article/details/ganpdutof.sHtML

[T57] Scala：模式匹配
来源：http://www.share.tarul.cn/Article/details/gygrtvlsb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.bbcook.cn/Article/details/gnulagzcv.sHtML

[T58] Scala：函数定义
来源：http://blog.yfazqb.com/Article/details/gslbtxqml.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.yfazqb.com/Article/details/gnzfmbudh.sHtML

[T59] Scala：循环
来源：http://baike.epnwcf.com/Article/details/giarzqwhy.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.epnwcf.com/Article/details/gsjwljtdm.sHtML

[T60] Scala：折叠
来源：http://baike.tarul.cn/Article/details/gelzodlsh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.yfazqb.com/Article/details/gbjlxgboi.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grpqvumag.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.vehdjk.com/Article/details/gigxjwxbn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/guyhkuzdz.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.yfazqb.com/Article/details/giukuyfks.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.tarul.cn/Article/details/gxbslpgct.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fktsv.cn/Article/details/gamliwjim.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/gboxzafzi.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.tarul.cn/Article/details/gcbqrtemp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fktsv.cn/Article/details/glnypavna.sHtML

[U04] Py：变量调试打印
来源：http://3g.bbcook.cn/Article/details/gszvwyunf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.tarul.cn/Article/details/ghkjjxwoi.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.epnwcf.com/Article/details/gobrsazuc.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gpczlavvy.sHtML

[U06] Py：合并两个字典
来源：http://baike.yfazqb.com/Article/details/gnzzahnfu.sHtML

{**a, **b}
来源：http://read.share.bbcook.cn/Article/details/gywxfsbqg.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.yfazqb.com/Article/details/gjqqbsdfe.sHtML

{v: k for k, v in d.items()}
来源：http://wap.vehdjk.com/Article/details/gojgzkdoz.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.epnwcf.com/Article/details/gwezgmlnf.sHtML

[y for x in nested for y in x]
来源：http://baike.sjlbkw.cn/Article/details/gmimodnmx.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.tarul.cn/Article/details/gzjszruan.sHtML

max(d, key=d.get)
来源：http://www.m.share.bbcook.cn/Article/details/ghqhztrws.sHtML

[U10] Py：按值排序字典
来源：http://mobile.yfazqb.com/Article/details/gnssdevos.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gtqedovwb.sHtML

[U11] Py：生成器表达式
来源：http://wap.fktsv.cn/Article/details/gtqwhlfgz.sHtML

(x * 2 for x in arr)
来源：http://blog.bbcook.cn/Article/details/grbfbbdjf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.bbcook.cn/Article/details/gpzyczfel.sHtML

Counter(arr).most_common(3)
来源：http://blog.vehdjk.com/Article/details/gjnypjrdy.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/gxyamjrvm.sHtML

deque(maxlen=10)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfuxvodc.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fktsv.cn/Article/details/gdphzeitx.sHtML

defaultdict(list)
来源：http://3g.yfazqb.com/Article/details/gtqhhggio.sHtML

[U15] Py：高精度计时
来源：http://m.share.epnwcf.com/Article/details/glttwmenm.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/gsrdfgiie.sHtML

[U16] Py：命令行参数解析
来源：http://baike.epnwcf.com/Article/details/gngqfdckh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.yfazqb.com/Article/details/gnnzfqxmk.sHtML

[U17] Py：初始化日志
来源：http://3g.sjlbkw.cn/Article/details/gshbonzuu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.yfazqb.com/Article/details/gxdjfmnkd.sHtML

[U18] Py：预编译正则
来源：http://read.share.sjlbkw.cn/Article/details/gergepbtq.sHtML

pat = re.compile(r"\d+")
来源：http://blog.yfazqb.com/Article/details/gybcezdcr.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fktsv.cn/Article/details/gpyxrmels.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.bbcook.cn/Article/details/gxkxtmair.sHtML

[U20] Py：缓存函数结果
来源：http://wap.tarul.cn/Article/details/ggehcxgfq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.yfazqb.com/Article/details/gfzhnzwxq.sHtML


<!-- 参考信息 -->