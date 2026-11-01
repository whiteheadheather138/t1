代发 wailian999

read -rp "请输入: " ans
来源：http://www.share.vehdjk.com/Article/details/gnafejwyd.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/gecgwfuzp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.tarul.cn/Article/details/gosoavcrr.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/grtibtfol.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.sjlbkw.cn/Article/details/gljgsmapb.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.sjlbkw.cn/Article/details/gldwvcozo.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gicpuypwj.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpcrboolo.sHtML

S. C / C++ 专题
来源：http://wap.bbcook.cn/Article/details/gxxikmhky.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmgvkitpa.sHtML

[S01] C：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gjmzaspkz.sHtML

#include <stdio.h>
来源：http://mobile.vehdjk.com/Article/details/gboazjerb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fktsv.cn/Article/details/gbunbvyte.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.yfazqb.com/Article/details/gfswdpusx.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.yfazqb.com/Article/details/gludvtuee.sHtML

[S03] C：读入整数
来源：http://baike.epnwcf.com/Article/details/gebxohykq.sHtML

int x; scanf("%d", &x);
来源：http://m.share.bbcook.cn/Article/details/gqxbkzxfw.sHtML

[S04] C：字符串复制
来源：http://wap.sjlbkw.cn/Article/details/gprkfjjpd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fktsv.cn/Article/details/gmlkbhgfh.sHtML

[S05] C：字符串长度
来源：http://mobile.epnwcf.com/Article/details/gigmaewmy.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/gcyagzors.sHtML

[S06] C：字符串比较
来源：http://www.blog.epnwcf.com/Article/details/glvjpluaj.sHtML

strcmp(a, b) == 0
来源：http://wap.epnwcf.com/Article/details/gxazvigwn.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/gvqqfbexy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/gvgkpaleq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fktsv.cn/Article/details/gjumrnnuw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqoheslvh.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.epnwcf.com/Article/details/ghqdwahef.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.epnwcf.com/Article/details/gayzmaaim.sHtML

[S10] C：指针与解引用
来源：http://blog.fktsv.cn/Article/details/gkkwolrwz.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/gflokrnqn.sHtML

[S11] C：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gzjatobgk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.epnwcf.com/Article/details/gwltxcdvd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gyrmkhlde.sHtML

fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/ggswoysjd.sHtML

[S12] C：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gbmqipeqw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gkgpqnwuw.sHtML

[S13] C：宏定义
来源：http://www.m.share.fktsv.cn/Article/details/gxnzaxrrc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.sjlbkw.cn/Article/details/gaexkcyts.sHtML

[S14] C：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gwekgxsny.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.vehdjk.com/Article/details/ghmwpbahs.sHtML

[S15] C：类型转换
来源：http://m.share.bbcook.cn/Article/details/ggpndnxbt.sHtML

(double) a / b
来源：http://baike.epnwcf.com/Article/details/gtqgsugcl.sHtML

[S16] C：位操作置位
来源：http://www.share.tarul.cn/Article/details/ggeelyysh.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/gyxradpin.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gcikiwvhb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.yfazqb.com/Article/details/gcgljhrtd.sHtML

[S18] C：命令行参数
来源：http://mobile.sjlbkw.cn/Article/details/gvqifzafw.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.vehdjk.com/Article/details/gwseukzlo.sHtML

[S19] C：快速排序
来源：http://mobile.epnwcf.com/Article/details/gagmcndjy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gbxfiwoko.sHtML

[S20] C：二分查找
来源：http://mobile.yfazqb.com/Article/details/gzeepdgwo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gmcakgbhc.sHtML

[S21] C：字符类别判断
来源：http://www.share.vehdjk.com/Article/details/gdsiyxaon.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/gysvfldzm.sHtML

[S22] C：字符串转数字
来源：http://baike.epnwcf.com/Article/details/gtpdjprim.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.vehdjk.com/Article/details/gtyalkaol.sHtML

[S23] C：随机数
来源：http://wap.tarul.cn/Article/details/gauqslzqe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/gmywhjrrq.sHtML

[S24] C：获取本地时间
来源：http://mobile.vehdjk.com/Article/details/gcubypkhq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.tarul.cn/Article/details/gevircdgp.sHtML

[S25] C：内存拷贝
来源：http://3g.epnwcf.com/Article/details/gnlagolce.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gcglnqdhv.sHtML

[S26] C：内存清零
来源：http://blog.sjlbkw.cn/Article/details/gqbzvornu.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjausczt.sHtML

[S27] C：定义常量
来源：http://www.blog.yfazqb.com/Article/details/ghxrwqyvq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/glgejhdta.sHtML

[S28] C：静态变量
来源：http://read.share.epnwcf.com/Article/details/gycmmqxil.sHtML

static int counter = 0;
来源：http://www.blog.yfazqb.com/Article/details/gvqdhuskr.sHtML

[S29] C：变参函数
来源：http://m.share.tarul.cn/Article/details/gjdvdjiur.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.vehdjk.com/Article/details/ggivtgzer.sHtML

[S30] C：头文件保护
来源：http://wap.epnwcf.com/Article/details/griuuupku.sHtML

#ifndef X_H
来源：http://read.share.tarul.cn/Article/details/gamaihmyc.sHtML

#define X_H
来源：http://3g.fktsv.cn/Article/details/gebugverc.sHtML

#endif
来源：http://www.m.share.tarul.cn/Article/details/gkdhgweaz.sHtML

[S31] C++：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/ggjoogrfr.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gidfsmkkz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.epnwcf.com/Article/details/ggkrqogdh.sHtML

[S32] C++：字符串
来源：http://www.m.share.epnwcf.com/Article/details/gsrufkcsx.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/gexjfonlt.sHtML

[S33] C++：vector 增删
来源：http://www.share.yfazqb.com/Article/details/gkbjfitlg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/geogfqcjx.sHtML

[S34] C++：遍历 vector
来源：http://blog.epnwcf.com/Article/details/gktcqawrb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gbpeeqwdv.sHtML

[S35] C++：map
来源：http://www.blog.epnwcf.com/Article/details/ggxolkkul.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gjtnprhbx.sHtML

[S36] C++：unordered_map
来源：http://read.share.sjlbkw.cn/Article/details/gmcrjqghv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gajxdwacp.sHtML

[S37] C++：set
来源：http://www.share.sjlbkw.cn/Article/details/ghgachzyq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.yfazqb.com/Article/details/ghgwkbjiz.sHtML

[S38] C++：排序
来源：http://wap.yfazqb.com/Article/details/gbzgossma.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.bbcook.cn/Article/details/gbwxehvuq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fktsv.cn/Article/details/gaajrsqmw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/gigbdisbx.sHtML

[S40] C++：查找元素
来源：http://read.share.fktsv.cn/Article/details/gyrbidnam.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/gkhkatcdy.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.yfazqb.com/Article/details/gvecjwhyz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.yfazqb.com/Article/details/gksgqiruz.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.bbcook.cn/Article/details/gsbuiydgy.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.tarul.cn/Article/details/gtilyirxk.sHtML

[S43] C++：智能指针
来源：http://wap.epnwcf.com/Article/details/gsxtbijzo.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.bbcook.cn/Article/details/gocxcghhl.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/gwrvekevj.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.bbcook.cn/Article/details/gcqpcxkzp.sHtML

[S45] C++：lambda
来源：http://mobile.tarul.cn/Article/details/gjkhskfng.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.sjlbkw.cn/Article/details/gkbkyyeso.sHtML

[S46] C++：函数模板
来源：http://3g.epnwcf.com/Article/details/gzplxtcnw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.vehdjk.com/Article/details/ggydrvooe.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.sjlbkw.cn/Article/details/gazxbmuni.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.vehdjk.com/Article/details/gmunipunm.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gycobdjcx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.sjlbkw.cn/Article/details/gvsxfdmgo.sHtML

while (std::getline(in, line)) { }
来源：http://3g.yfazqb.com/Article/details/giwbtvfpk.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gimxpyfst.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.bbcook.cn/Article/details/ghwqlnepe.sHtML

[S50] C++：格式化数字
来源：http://wap.epnwcf.com/Article/details/ggtqzjpyv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gryjpbevf.sHtML

[S51] C++：显式类型转换
来源：http://blog.vehdjk.com/Article/details/gqtxogbtt.sHtML

static_cast<double>(a) / b
来源：http://mobile.fktsv.cn/Article/details/glzrdfdkx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/gjylrjegu.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gqpbvoohl.sHtML

[S53] C++：移动语义
来源：http://www.blog.fktsv.cn/Article/details/gpiigafxx.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fktsv.cn/Article/details/gofebwrso.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gjgzmtqld.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.vehdjk.com/Article/details/gtnqsnlyv.sHtML

[S55] C++：结构化绑定
来源：http://www.share.epnwcf.com/Article/details/gxyqzmnfz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.sjlbkw.cn/Article/details/giinqnxjz.sHtML

[S56] C++：optional
来源：http://m.share.sjlbkw.cn/Article/details/gfdrnsyda.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/gvuspoycy.sHtML

[S57] C++：编译期常量
来源：http://www.share.bbcook.cn/Article/details/glsnvzwts.sHtML

constexpr int N = 10;
来源：http://wap.bbcook.cn/Article/details/gtlobrocd.sHtML

[S58] C++：命名空间
来源：http://mobile.yfazqb.com/Article/details/gbqgivnpf.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.tarul.cn/Article/details/gydlsyqhs.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/gmcnowstp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.yfazqb.com/Article/details/giumzdcpf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.epnwcf.com/Article/details/ggpqcagmt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.vehdjk.com/Article/details/gubifubep.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxvpampxc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fktsv.cn/Article/details/gqozhjedc.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/guowjwpjv.sHtML

[T01] Kotlin：Hello World
来源：http://wap.bbcook.cn/Article/details/gwxsiawuh.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gmioswvwk.sHtML

[T02] Kotlin：变量
来源：http://baike.fktsv.cn/Article/details/grvblaejb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/gmyjtniqm.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/gtsyjpbvi.sHtML

"值: $b"
来源：http://mobile.tarul.cn/Article/details/gkxdwdcwx.sHtML

[T04] Kotlin：空安全
来源：http://blog.bbcook.cn/Article/details/gmowwqwnt.sHtML

val n: String? = null;  n?.length
来源：http://m.share.yfazqb.com/Article/details/grootixad.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.bbcook.cn/Article/details/gdeicvhth.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.epnwcf.com/Article/details/gumaanhjq.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.yfazqb.com/Article/details/gjhoyjiby.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/gyqttglvz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.vehdjk.com/Article/details/ghmzozmje.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.sjlbkw.cn/Article/details/gjbbdozrq.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/gilaogpws.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmimvyyyj.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.epnwcf.com/Article/details/gyzrgqikd.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.tarul.cn/Article/details/gfbwbjier.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.vehdjk.com/Article/details/gxhziefba.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fktsv.cn/Article/details/gihtqjqql.sHtML

[T11] Kotlin：协程
来源：http://www.share.fktsv.cn/Article/details/gszzgkamk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.bbcook.cn/Article/details/guerfthmh.sHtML

[T12] Kotlin：解构声明
来源：http://3g.vehdjk.com/Article/details/gfbwffrac.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.vehdjk.com/Article/details/guraienmd.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fktsv.cn/Article/details/gqgywowje.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fktsv.cn/Article/details/gajlxijha.sHtML

[T14] Kotlin：循环
来源：http://m.share.fktsv.cn/Article/details/gongkcrzc.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gdmdkqmiu.sHtML

[T15] Kotlin：接口
来源：http://read.share.bbcook.cn/Article/details/gxkweuzpu.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.bbcook.cn/Article/details/gfbnfixpv.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gnrfoysng.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gzxwzqexo.sHtML

[T17] Swift：变量与常量
来源：http://m.share.bbcook.cn/Article/details/guwfzrzae.sHtML

var a = 1;  let b = 2
来源：http://wap.yfazqb.com/Article/details/gylwofocc.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gcgdqaprh.sHtML

"值: \(b)"
来源：http://m.share.yfazqb.com/Article/details/giwkcknfe.sHtML

[T19] Swift：可选绑定
来源：http://read.share.tarul.cn/Article/details/gmfmplwcf.sHtML

if let n = opt { print(n) }
来源：http://www.blog.epnwcf.com/Article/details/gpiwnjknc.sHtML

[T20] Swift：数组操作
来源：http://www.share.yfazqb.com/Article/details/gftzjrlut.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.vehdjk.com/Article/details/gyshvghri.sHtML

[T21] Swift：遍历
来源：http://m.share.yfazqb.com/Article/details/gpbafudgi.sHtML

for x in a { print(x) }
来源：http://mobile.epnwcf.com/Article/details/gkqejafqh.sHtML

[T22] Swift：字典
来源：http://m.share.epnwcf.com/Article/details/glieijyap.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.sjlbkw.cn/Article/details/gksdwqcqq.sHtML

[T23] Swift：函数
来源：http://baike.tarul.cn/Article/details/gcnvrccgp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.epnwcf.com/Article/details/gucvhwkta.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvoseubr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gacuwhrgb.sHtML

[T25] Swift：结构体
来源：http://www.blog.epnwcf.com/Article/details/gewijraca.sHtML

struct P { var x: Int }
来源：http://3g.bbcook.cn/Article/details/gpovlrmoj.sHtML

[T26] Swift：类与重写
来源：http://m.share.bbcook.cn/Article/details/gpjjntnky.sHtML

class A: Base { override func f() {} }
来源：http://m.share.tarul.cn/Article/details/gommrdzzt.sHtML

[T27] Swift：错误处理
来源：http://mobile.bbcook.cn/Article/details/gzojksbmg.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.tarul.cn/Article/details/gnopbqvfe.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/gxefxajry.sHtML

enum Color { case red, green }
来源：http://baike.tarul.cn/Article/details/gfegbkbra.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.tarul.cn/Article/details/geowguybb.sHtML

guard let x = opt else { return }
来源：http://www.blog.epnwcf.com/Article/details/giqpyxwcy.sHtML

[T30] Swift：协议
来源：http://baike.fktsv.cn/Article/details/gptfrcpaa.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.epnwcf.com/Article/details/gpgkgxsob.sHtML

[T31] Lua：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gvpfkkutg.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/gixwlfoaa.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/guhsoqijv.sHtML

local a = 1
来源：http://www.m.share.tarul.cn/Article/details/gpaljjwae.sHtML

[T33] Lua：表（数组）
来源：http://wap.bbcook.cn/Article/details/gopvrcnkt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.tarul.cn/Article/details/gtecvjrdm.sHtML

[T34] Lua：遍历表
来源：http://3g.fktsv.cn/Article/details/gknzxvidd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.yfazqb.com/Article/details/gfungxfni.sHtML

[T35] Lua：字典表
来源：http://wap.fktsv.cn/Article/details/gkhpazjlz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.yfazqb.com/Article/details/gnxyjtpok.sHtML

[T36] Lua：函数
来源：http://3g.vehdjk.com/Article/details/gniluecbd.sHtML

function add(a, b) return a + b end
来源：http://3g.bbcook.cn/Article/details/gxomhimmu.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.epnwcf.com/Article/details/ggobgnahb.sHtML

"a" .. "b"
来源：http://wap.sjlbkw.cn/Article/details/golairjsv.sHtML

[T38] Lua：条件
来源：http://www.m.share.vehdjk.com/Article/details/gtqwcgqmu.sHtML

if x > 0 then print("正") end
来源：http://www.share.yfazqb.com/Article/details/gctgvuezr.sHtML

[T39] Lua：模式匹配
来源：http://3g.yfazqb.com/Article/details/gvosyjlgf.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fktsv.cn/Article/details/ggkmiawbm.sHtML

[T40] Lua：元表
来源：http://3g.fktsv.cn/Article/details/gnsdkouro.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.yfazqb.com/Article/details/gbtdtztlf.sHtML

[T41] Perl：Hello World
来源：http://3g.sjlbkw.cn/Article/details/ghykmdhvp.sHtML

print "Hello\n";
来源：http://blog.vehdjk.com/Article/details/gvfrttmsr.sHtML

[T42] Perl：变量类型
来源：http://m.share.tarul.cn/Article/details/gxteivhuf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.tarul.cn/Article/details/ghpmggkac.sHtML

[T43] Perl：字符串插值
来源：http://blog.yfazqb.com/Article/details/gwftuyaxw.sHtML

"值: $a"
来源：http://3g.sjlbkw.cn/Article/details/gtsgilols.sHtML

[T44] Perl：条件
来源：http://www.blog.yfazqb.com/Article/details/gofrfheut.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fktsv.cn/Article/details/gzgvyxoag.sHtML

[T45] Perl：数组遍历
来源：http://m.share.bbcook.cn/Article/details/gufxalpnm.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.vehdjk.com/Article/details/gozqvbtlv.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fktsv.cn/Article/details/gyjtznoay.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fktsv.cn/Article/details/ggslxznfu.sHtML

[T47] Perl：正则捕获
来源：http://blog.sjlbkw.cn/Article/details/gsezhfguc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.bbcook.cn/Article/details/gggrgvagf.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/gbecmopts.sHtML

$s =~ s/old/new/g;
来源：http://read.share.sjlbkw.cn/Article/details/gmudwibsj.sHtML

[T49] Perl：函数
来源：http://read.share.vehdjk.com/Article/details/gzhwywmrs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/glmhjedeb.sHtML

[T50] Perl：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gvyiqlvnh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.tarul.cn/Article/details/gorekjvwc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.bbcook.cn/Article/details/gimdhjqlq.sHtML

[T51] Scala：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gptdjfudq.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gddiexsoi.sHtML

[T52] Scala：变量
来源：http://baike.yfazqb.com/Article/details/gkjwyjulu.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrqqboms.sHtML

[T53] Scala：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gdnznkskm.sHtML

s"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gnijlytxb.sHtML

[T54] Scala：集合映射
来源：http://wap.fktsv.cn/Article/details/grhmldsio.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.yfazqb.com/Article/details/gpanjawid.sHtML

[T55] Scala：集合过滤
来源：http://m.share.yfazqb.com/Article/details/gbgairink.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.tarul.cn/Article/details/gjteovhci.sHtML

[T56] Scala：样例类
来源：http://m.share.vehdjk.com/Article/details/gpigsrsjj.sHtML

case class User(name: String, age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gxiptjcak.sHtML

[T57] Scala：模式匹配
来源：http://www.share.vehdjk.com/Article/details/gdysgkzbg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gjupgdasr.sHtML

[T58] Scala：函数定义
来源：http://blog.tarul.cn/Article/details/gdbhdkriw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.tarul.cn/Article/details/gvmvrzfya.sHtML

[T59] Scala：循环
来源：http://blog.fktsv.cn/Article/details/gpxczlmyg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gqyxkklvf.sHtML

[T60] Scala：折叠
来源：http://baike.sjlbkw.cn/Article/details/ghzlenfoy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.tarul.cn/Article/details/guwtihkjy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ggfutlbie.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/ggpzogfrl.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggacidvtp.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fktsv.cn/Article/details/gzfpcqpve.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.epnwcf.com/Article/details/gpvwgtcng.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.tarul.cn/Article/details/gurzfnzqk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.sjlbkw.cn/Article/details/gepcckyga.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.sjlbkw.cn/Article/details/gaxymqhcu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.bbcook.cn/Article/details/gapqgxwnp.sHtML

[U04] Py：变量调试打印
来源：http://blog.bbcook.cn/Article/details/gzahpnwcy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.vehdjk.com/Article/details/ggnhuynsl.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.sjlbkw.cn/Article/details/gtseyyjve.sHtML

list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/gplrchamj.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gutgxnrwh.sHtML

{**a, **b}
来源：http://www.m.share.yfazqb.com/Article/details/ghbkefwjf.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.vehdjk.com/Article/details/gehaxjplz.sHtML

{v: k for k, v in d.items()}
来源：http://blog.vehdjk.com/Article/details/gaxssoyrj.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fktsv.cn/Article/details/gdlozjwci.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fktsv.cn/Article/details/gsohswlmi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.bbcook.cn/Article/details/gmlehprug.sHtML

max(d, key=d.get)
来源：http://read.share.fktsv.cn/Article/details/guxtrkdmk.sHtML

[U10] Py：按值排序字典
来源：http://www.share.bbcook.cn/Article/details/gvnxvobbe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fktsv.cn/Article/details/gfzfufkdr.sHtML

[U11] Py：生成器表达式
来源：http://blog.sjlbkw.cn/Article/details/gzqrwwhrc.sHtML

(x * 2 for x in arr)
来源：http://read.share.fktsv.cn/Article/details/gvwsdjafu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fktsv.cn/Article/details/giaxmhhow.sHtML

Counter(arr).most_common(3)
来源：http://3g.yfazqb.com/Article/details/gxecrikqh.sHtML

[U13] Py：固定长度队列
来源：http://www.share.epnwcf.com/Article/details/gmgtapyos.sHtML

deque(maxlen=10)
来源：http://3g.fktsv.cn/Article/details/gugldywtg.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.epnwcf.com/Article/details/ganqllmqq.sHtML

defaultdict(list)
来源：http://read.share.epnwcf.com/Article/details/gsddxygix.sHtML

[U15] Py：高精度计时
来源：http://www.share.tarul.cn/Article/details/glnvaqrfa.sHtML

t = time.perf_counter()
来源：http://baike.yfazqb.com/Article/details/gjtepmnmz.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fktsv.cn/Article/details/gjlkyjekr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.yfazqb.com/Article/details/gvgitsrmi.sHtML

[U17] Py：初始化日志
来源：http://www.blog.sjlbkw.cn/Article/details/gnnxggnav.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.vehdjk.com/Article/details/gbmxkjcxv.sHtML

[U18] Py：预编译正则
来源：http://3g.tarul.cn/Article/details/gnuwtgtnf.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gcrtkdpkd.sHtML


<!-- 参考信息 -->