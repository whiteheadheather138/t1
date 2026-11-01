代发 wailian999

read -rp "请输入: " ans
来源：http://www.share.vehdjk.com/Article/details/gtudsbkoe.sHtML

[R78] 交互式菜单
来源：http://3g.fktsv.cn/Article/details/gpewckkcq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.yfazqb.com/Article/details/gpkmtfxuy.sHtML

[R79] 解析命令行选项
来源：http://www.share.fktsv.cn/Article/details/goygwrrfb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gassmuazk.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.tarul.cn/Article/details/gvwpwobxs.sHtML

time ./run.sh
来源：http://mobile.yfazqb.com/Article/details/gycjggvpt.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gisheioap.sHtML

S. C / C++ 专题
来源：http://www.share.yfazqb.com/Article/details/gxudvjrqq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gcephawbv.sHtML

[S01] C：Hello World
来源：http://www.blog.bbcook.cn/Article/details/guysetaog.sHtML

#include <stdio.h>
来源：http://read.share.sjlbkw.cn/Article/details/gnxuhftyy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.sjlbkw.cn/Article/details/gazwqzoxk.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fktsv.cn/Article/details/gctjesbzj.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.yfazqb.com/Article/details/geuplwvbl.sHtML

[S03] C：读入整数
来源：http://read.share.yfazqb.com/Article/details/gwpmnhisv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/gznpnhhom.sHtML

[S04] C：字符串复制
来源：http://mobile.tarul.cn/Article/details/gujwppasi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.epnwcf.com/Article/details/gflyadjqy.sHtML

[S05] C：字符串长度
来源：http://read.share.epnwcf.com/Article/details/gellgtbll.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/gdptejnby.sHtML

[S06] C：字符串比较
来源：http://www.share.vehdjk.com/Article/details/gmbkfmufs.sHtML

strcmp(a, b) == 0
来源：http://mobile.tarul.cn/Article/details/goslstwht.sHtML

[S07] C：数组遍历求和
来源：http://3g.bbcook.cn/Article/details/gowugnphv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.tarul.cn/Article/details/gpreyyeju.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gnhmvnzdd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.yfazqb.com/Article/details/gjlwmcktp.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.yfazqb.com/Article/details/gralzuxdd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gxhmontrc.sHtML

[S10] C：指针与解引用
来源：http://3g.sjlbkw.cn/Article/details/ggneaeios.sHtML

int *p = &a;  *p = 5;
来源：http://wap.sjlbkw.cn/Article/details/gwlocwzrt.sHtML

[S11] C：逐行读文件
来源：http://read.share.tarul.cn/Article/details/grxtshzoq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fktsv.cn/Article/details/gmrckytgq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.yfazqb.com/Article/details/gnmuoarzt.sHtML

fclose(f);
来源：http://3g.bbcook.cn/Article/details/gxcdiktkw.sHtML

[S12] C：写文件
来源：http://m.share.vehdjk.com/Article/details/gjibmzapb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.vehdjk.com/Article/details/gibyeoffc.sHtML

[S13] C：宏定义
来源：http://www.blog.tarul.cn/Article/details/gdjlbhlyw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.sjlbkw.cn/Article/details/gprpffmqs.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/gofwjzokr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.epnwcf.com/Article/details/giimyifep.sHtML

[S15] C：类型转换
来源：http://wap.sjlbkw.cn/Article/details/gfblygmit.sHtML

(double) a / b
来源：http://www.m.share.vehdjk.com/Article/details/gbzuqlaut.sHtML

[S16] C：位操作置位
来源：http://www.blog.tarul.cn/Article/details/gotfmkezh.sHtML

x |= (1 << 3);
来源：http://baike.yfazqb.com/Article/details/gxhxgdqgr.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gdinnzdml.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.sjlbkw.cn/Article/details/gemuitese.sHtML

[S18] C：命令行参数
来源：http://read.share.epnwcf.com/Article/details/gffabjguh.sHtML

int main(int argc, char **argv)
来源：http://baike.tarul.cn/Article/details/gggfrzvqs.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/guenjqsif.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gpssbikcb.sHtML

[S20] C：二分查找
来源：http://www.m.share.tarul.cn/Article/details/gcylhvqse.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gscuyllpn.sHtML

[S21] C：字符类别判断
来源：http://read.share.vehdjk.com/Article/details/godaptiow.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.sjlbkw.cn/Article/details/gcgznswsk.sHtML

[S22] C：字符串转数字
来源：http://mobile.bbcook.cn/Article/details/gvuuoeyih.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/gyxaiccfb.sHtML

[S23] C：随机数
来源：http://baike.tarul.cn/Article/details/gxvygwytp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/gxfyibxuq.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gacjxbphi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.bbcook.cn/Article/details/ghnbobckw.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/ggakouwbk.sHtML

memcpy(dst, src, n);
来源：http://3g.yfazqb.com/Article/details/gllxyapbg.sHtML

[S26] C：内存清零
来源：http://3g.yfazqb.com/Article/details/gdgrhhidq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.epnwcf.com/Article/details/gqymiolqg.sHtML

[S27] C：定义常量
来源：http://www.blog.vehdjk.com/Article/details/gsliotkem.sHtML

const double PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gzoiobabh.sHtML

[S28] C：静态变量
来源：http://www.m.share.fktsv.cn/Article/details/gvbuftzkd.sHtML

static int counter = 0;
来源：http://read.share.yfazqb.com/Article/details/gwfrfkhpd.sHtML

[S29] C：变参函数
来源：http://www.share.vehdjk.com/Article/details/gceyxdiqc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.vehdjk.com/Article/details/gecdxpxtw.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/gnjtthxod.sHtML

#ifndef X_H
来源：http://www.share.sjlbkw.cn/Article/details/gisbaigij.sHtML

#define X_H
来源：http://www.blog.bbcook.cn/Article/details/gpgaywwcg.sHtML

#endif
来源：http://baike.tarul.cn/Article/details/grzupjfde.sHtML

[S31] C++：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gxlallhox.sHtML

#include <iostream>
来源：http://3g.yfazqb.com/Article/details/gpgrqfhhq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/glykztgbw.sHtML

[S32] C++：字符串
来源：http://mobile.bbcook.cn/Article/details/gjyrvpabk.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/glcebyyyz.sHtML

[S33] C++：vector 增删
来源：http://baike.tarul.cn/Article/details/gvfcnkuzg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.bbcook.cn/Article/details/gzlpujxzk.sHtML

[S34] C++：遍历 vector
来源：http://baike.bbcook.cn/Article/details/gaqsmpqyr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/gtyvhdfkq.sHtML

[S35] C++：map
来源：http://read.share.yfazqb.com/Article/details/geigcdrsi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gvihsacyh.sHtML

[S36] C++：unordered_map
来源：http://3g.vehdjk.com/Article/details/gutiacegs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gtmwlauhb.sHtML

[S37] C++：set
来源：http://3g.vehdjk.com/Article/details/gdixdiszy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.epnwcf.com/Article/details/gzceqgswd.sHtML

[S38] C++：排序
来源：http://baike.yfazqb.com/Article/details/gczbbkjgd.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.bbcook.cn/Article/details/gywmxmdio.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.bbcook.cn/Article/details/grjkukuzr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.vehdjk.com/Article/details/gxipnbakb.sHtML

[S40] C++：查找元素
来源：http://wap.fktsv.cn/Article/details/gujphrjbl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/grblsbtjf.sHtML

[S41] C++：类与构造函数
来源：http://wap.epnwcf.com/Article/details/gsztofrfk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.bbcook.cn/Article/details/gytifvzed.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gzeceaqok.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.sjlbkw.cn/Article/details/gxcheqxag.sHtML

[S43] C++：智能指针
来源：http://wap.tarul.cn/Article/details/glgexinoi.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.bbcook.cn/Article/details/gsqhnxlot.sHtML

[S44] C++：引用传参
来源：http://read.share.bbcook.cn/Article/details/gvawhdegr.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.bbcook.cn/Article/details/gydkipphx.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/gznqaxjdp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fktsv.cn/Article/details/gchqfeilf.sHtML

[S46] C++：函数模板
来源：http://read.share.sjlbkw.cn/Article/details/gyiljzdbh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/gayaonsjf.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.tarul.cn/Article/details/gehwudlva.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fktsv.cn/Article/details/gqyevfptq.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gtnwedtcj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.epnwcf.com/Article/details/goprqwojk.sHtML

while (std::getline(in, line)) { }
来源：http://baike.epnwcf.com/Article/details/gbrfechgm.sHtML

[S49] C++：写文件
来源：http://m.share.tarul.cn/Article/details/gpnsuahnj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/gdpakgaka.sHtML

[S50] C++：格式化数字
来源：http://www.share.tarul.cn/Article/details/gficvzlto.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gugkqqrwt.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/gxihuownh.sHtML

static_cast<double>(a) / b
来源：http://baike.fktsv.cn/Article/details/gtvwvwhsq.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.sjlbkw.cn/Article/details/grpnnmklf.sHtML

int size() const noexcept { return n_; }
来源：http://blog.vehdjk.com/Article/details/gasvafcug.sHtML

[S53] C++：移动语义
来源：http://3g.epnwcf.com/Article/details/gzrfkopet.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.tarul.cn/Article/details/gnatnvlzj.sHtML

[S54] C++：异常处理
来源：http://3g.epnwcf.com/Article/details/ggmgvcgsc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.bbcook.cn/Article/details/gmzimasbt.sHtML

[S55] C++：结构化绑定
来源：http://read.share.vehdjk.com/Article/details/gxkddnsqj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gjqoayzgo.sHtML

[S56] C++：optional
来源：http://www.blog.vehdjk.com/Article/details/gmydrugkb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.sjlbkw.cn/Article/details/ggysxyage.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gpgefwsra.sHtML

constexpr int N = 10;
来源：http://baike.epnwcf.com/Article/details/gtpqovfid.sHtML

[S58] C++：命名空间
来源：http://3g.bbcook.cn/Article/details/gbzzfhcmf.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.vehdjk.com/Article/details/gaqfgqkns.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/ggjlatlrz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.vehdjk.com/Article/details/gpebaqpev.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/guegmlvte.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.vehdjk.com/Article/details/gdfetbtqq.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqzmussee.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gwabjqpqp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glgvbybcb.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.yfazqb.com/Article/details/gqqovupvt.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gcubpsfhg.sHtML

[T02] Kotlin：变量
来源：http://wap.vehdjk.com/Article/details/gkvhsqbcr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/gyscukplz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fktsv.cn/Article/details/gkusoojfq.sHtML

"值: $b"
来源：http://mobile.epnwcf.com/Article/details/ghyfbodaj.sHtML

[T04] Kotlin：空安全
来源：http://read.share.yfazqb.com/Article/details/gqvsbjoxa.sHtML

val n: String? = null;  n?.length
来源：http://mobile.bbcook.cn/Article/details/gqplovncq.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.vehdjk.com/Article/details/gqhrlzeiu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/gzquwuvip.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.vehdjk.com/Article/details/gjelqlfka.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fktsv.cn/Article/details/gfoiwpfqw.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/gkanmwfkd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.epnwcf.com/Article/details/gqmfbvvhl.sHtML

[T08] Kotlin：数据类
来源：http://mobile.vehdjk.com/Article/details/ghmxjydtw.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fktsv.cn/Article/details/gyvmsxcag.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.tarul.cn/Article/details/gwlirkgso.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.yfazqb.com/Article/details/gahixxkkm.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fktsv.cn/Article/details/gizjftvxx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.tarul.cn/Article/details/gtyvglaxa.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.vehdjk.com/Article/details/gdrqcyexp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.epnwcf.com/Article/details/gspghmvio.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/gyfkrfrnf.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.bbcook.cn/Article/details/galydctfx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.yfazqb.com/Article/details/ghzhvuqaj.sHtML

val m = mapOf("a" to 1)
来源：http://baike.bbcook.cn/Article/details/gsdvuluay.sHtML

[T14] Kotlin：循环
来源：http://www.blog.vehdjk.com/Article/details/gzygxqeob.sHtML

for (i in 1..10) println(i)
来源：http://baike.epnwcf.com/Article/details/gnhscrhuq.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/gmhyzamtf.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/godsntwcq.sHtML

[T16] Swift：Hello World
来源：http://mobile.epnwcf.com/Article/details/gddstigtf.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/grljkswrt.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fktsv.cn/Article/details/guspbxenc.sHtML

var a = 1;  let b = 2
来源：http://www.share.epnwcf.com/Article/details/genymnhze.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/gpamisbpx.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gpxtrojxo.sHtML

[T19] Swift：可选绑定
来源：http://m.share.yfazqb.com/Article/details/gcmalwtkg.sHtML

if let n = opt { print(n) }
来源：http://read.share.vehdjk.com/Article/details/gpvxtfxhf.sHtML

[T20] Swift：数组操作
来源：http://3g.bbcook.cn/Article/details/gbsgxsodk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.yfazqb.com/Article/details/gxcjnpvzw.sHtML

[T21] Swift：遍历
来源：http://wap.sjlbkw.cn/Article/details/gvlnstgjp.sHtML

for x in a { print(x) }
来源：http://read.share.tarul.cn/Article/details/golqayupp.sHtML

[T22] Swift：字典
来源：http://3g.sjlbkw.cn/Article/details/glwqfnygw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.vehdjk.com/Article/details/gqljybvfc.sHtML

[T23] Swift：函数
来源：http://m.share.epnwcf.com/Article/details/gmibbeezg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/gqqvsclkc.sHtML

[T24] Swift：闭包
来源：http://baike.bbcook.cn/Article/details/gtsouubdt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.epnwcf.com/Article/details/gzgqfsfpj.sHtML

[T25] Swift：结构体
来源：http://mobile.vehdjk.com/Article/details/gygvsncyb.sHtML

struct P { var x: Int }
来源：http://3g.epnwcf.com/Article/details/geswezcmu.sHtML

[T26] Swift：类与重写
来源：http://blog.yfazqb.com/Article/details/giojluafz.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.tarul.cn/Article/details/gstqgulmd.sHtML

[T27] Swift：错误处理
来源：http://www.share.tarul.cn/Article/details/gceutlnou.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.tarul.cn/Article/details/gibspnoij.sHtML

[T28] Swift：枚举
来源：http://baike.epnwcf.com/Article/details/gnmdndlwn.sHtML

enum Color { case red, green }
来源：http://mobile.bbcook.cn/Article/details/gbkjeuxqv.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.vehdjk.com/Article/details/glxafiryf.sHtML

guard let x = opt else { return }
来源：http://read.share.bbcook.cn/Article/details/grniaygot.sHtML

[T30] Swift：协议
来源：http://www.blog.bbcook.cn/Article/details/gujsgemyf.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.vehdjk.com/Article/details/gaydprhep.sHtML

[T31] Lua：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gvijgctea.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/gelykvgyw.sHtML

[T32] Lua：局部变量
来源：http://www.share.fktsv.cn/Article/details/gvxhkapxp.sHtML

local a = 1
来源：http://blog.fktsv.cn/Article/details/gtkgeupku.sHtML

[T33] Lua：表（数组）
来源：http://mobile.sjlbkw.cn/Article/details/gmzqvcdhm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fktsv.cn/Article/details/giysbotpe.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/guzdhxueq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.epnwcf.com/Article/details/guhbafbcn.sHtML

[T35] Lua：字典表
来源：http://www.share.vehdjk.com/Article/details/gluddfzez.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fktsv.cn/Article/details/gachbjewf.sHtML

[T36] Lua：函数
来源：http://www.blog.vehdjk.com/Article/details/gmpttuuqv.sHtML

function add(a, b) return a + b end
来源：http://www.share.vehdjk.com/Article/details/gfandipvi.sHtML

[T37] Lua：字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/geabtksgq.sHtML

"a" .. "b"
来源：http://www.m.share.tarul.cn/Article/details/gavnjivxj.sHtML

[T38] Lua：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmcspyja.sHtML

if x > 0 then print("正") end
来源：http://3g.fktsv.cn/Article/details/gqpowziph.sHtML

[T39] Lua：模式匹配
来源：http://wap.fktsv.cn/Article/details/glnhmibvw.sHtML

string.find(s, "%d+")
来源：http://wap.tarul.cn/Article/details/gczbfgcsy.sHtML

[T40] Lua：元表
来源：http://www.m.share.epnwcf.com/Article/details/gxujzvysr.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.epnwcf.com/Article/details/gaochyolf.sHtML

[T41] Perl：Hello World
来源：http://3g.bbcook.cn/Article/details/gvbzxofzj.sHtML

print "Hello\n";
来源：http://www.blog.epnwcf.com/Article/details/gsobnjztf.sHtML

[T42] Perl：变量类型
来源：http://baike.fktsv.cn/Article/details/gwhlhgqjb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.bbcook.cn/Article/details/gdopwapum.sHtML

[T43] Perl：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gnaktnwmj.sHtML

"值: $a"
来源：http://m.share.fktsv.cn/Article/details/gmssenljv.sHtML

[T44] Perl：条件
来源：http://mobile.tarul.cn/Article/details/grwrzgwfj.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.bbcook.cn/Article/details/gruiksrff.sHtML

[T45] Perl：数组遍历
来源：http://www.share.tarul.cn/Article/details/gelyponfp.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fktsv.cn/Article/details/gqhsppxyk.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/grhtommvb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.epnwcf.com/Article/details/gduwulgoi.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fktsv.cn/Article/details/gifjlsikw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.vehdjk.com/Article/details/gfsjdwqjl.sHtML

[T48] Perl：正则替换
来源：http://mobile.tarul.cn/Article/details/gklwrokov.sHtML

$s =~ s/old/new/g;
来源：http://www.share.yfazqb.com/Article/details/gqfzqpoud.sHtML

[T49] Perl：函数
来源：http://read.share.tarul.cn/Article/details/ghdobbspk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gbnyrcmiv.sHtML

[T50] Perl：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gaakpjekm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.bbcook.cn/Article/details/gscoihzbz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.tarul.cn/Article/details/gtdoeudpm.sHtML

[T51] Scala：Hello World
来源：http://www.share.yfazqb.com/Article/details/gdqopdbxw.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gplslkwmc.sHtML

[T52] Scala：变量
来源：http://read.share.bbcook.cn/Article/details/gdjqcrwoe.sHtML

val a = 1;  var b = 2
来源：http://3g.sjlbkw.cn/Article/details/ghzlbqgmq.sHtML

[T53] Scala：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gsvkgltlp.sHtML

s"值: $b"
来源：http://www.share.vehdjk.com/Article/details/grvuubpdf.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/gkoubqrnm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.tarul.cn/Article/details/gxrnybffi.sHtML

[T55] Scala：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/ghqjjuhtw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.tarul.cn/Article/details/gixcktleb.sHtML

[T56] Scala：样例类
来源：http://m.share.epnwcf.com/Article/details/gtxaghkzo.sHtML

case class User(name: String, age: Int)
来源：http://www.share.yfazqb.com/Article/details/gotbgntrj.sHtML

[T57] Scala：模式匹配
来源：http://www.share.tarul.cn/Article/details/gzsvsozcm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.vehdjk.com/Article/details/gzzhgazpi.sHtML

[T58] Scala：函数定义
来源：http://wap.bbcook.cn/Article/details/gruvqsvgm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.tarul.cn/Article/details/gryyotlrs.sHtML

[T59] Scala：循环
来源：http://www.share.bbcook.cn/Article/details/grbbgejuf.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.epnwcf.com/Article/details/gbgoraemo.sHtML

[T60] Scala：折叠
来源：http://www.blog.yfazqb.com/Article/details/ghanjckeh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.tarul.cn/Article/details/gajkgyclg.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gawmfmuxa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/gphauhrbq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gynkfcznl.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fktsv.cn/Article/details/gujugirnu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.epnwcf.com/Article/details/gifagiowm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fktsv.cn/Article/details/ganygjgvu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.vehdjk.com/Article/details/gilturvtv.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fktsv.cn/Article/details/ggntgksnt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.epnwcf.com/Article/details/gorhvmjjy.sHtML

[U04] Py：变量调试打印
来源：http://m.share.epnwcf.com/Article/details/gpwbnpjzv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.tarul.cn/Article/details/gwzuodtfl.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.vehdjk.com/Article/details/ggkdbmrfx.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gialxdtks.sHtML

[U06] Py：合并两个字典
来源：http://mobile.sjlbkw.cn/Article/details/gstixtnli.sHtML

{**a, **b}
来源：http://www.blog.sjlbkw.cn/Article/details/ghmyayyfu.sHtML

[U07] Py：反转字典键值
来源：http://baike.sjlbkw.cn/Article/details/glonsrbnd.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.bbcook.cn/Article/details/gfsvquhpm.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gfhejbvtm.sHtML

[y for x in nested for y in x]
来源：http://www.blog.yfazqb.com/Article/details/gmticktrv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.epnwcf.com/Article/details/gmhqmnase.sHtML

max(d, key=d.get)
来源：http://www.share.tarul.cn/Article/details/gsxzsptbo.sHtML

[U10] Py：按值排序字典
来源：http://wap.bbcook.cn/Article/details/goidvvabo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.yfazqb.com/Article/details/gpyxcawyw.sHtML

[U11] Py：生成器表达式
来源：http://m.share.vehdjk.com/Article/details/grcnqnrhq.sHtML

(x * 2 for x in arr)
来源：http://wap.vehdjk.com/Article/details/gumyhlryc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.epnwcf.com/Article/details/gekgudnhw.sHtML

Counter(arr).most_common(3)
来源：http://www.share.bbcook.cn/Article/details/grrwqceoj.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.tarul.cn/Article/details/gtebrdcdo.sHtML

deque(maxlen=10)
来源：http://read.share.fktsv.cn/Article/details/gbedweibo.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.vehdjk.com/Article/details/gphstpsyo.sHtML

defaultdict(list)
来源：http://blog.fktsv.cn/Article/details/gegndypqd.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fktsv.cn/Article/details/glssxdrtw.sHtML

t = time.perf_counter()
来源：http://www.share.sjlbkw.cn/Article/details/gwmpdbdol.sHtML

[U16] Py：命令行参数解析
来源：http://wap.bbcook.cn/Article/details/gzpmbiglr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.sjlbkw.cn/Article/details/gkhlvaimo.sHtML

[U17] Py：初始化日志
来源：http://m.share.yfazqb.com/Article/details/gltknnxas.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.epnwcf.com/Article/details/gfonhitot.sHtML

[U18] Py：预编译正则
来源：http://www.blog.yfazqb.com/Article/details/ghqchvkdt.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/guumghqut.sHtML


<!-- 参考信息 -->