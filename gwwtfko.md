代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/ggjcuncfm.sHtML

[R76] 使用临时文件
来源：http://www.share.vehdjk.com/Article/details/glvkxqqsc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gipstdlou.sHtML

[R77] 读取用户输入
来源：http://wap.tarul.cn/Article/details/gchmrukfj.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/gjdsqjlpk.sHtML

[R78] 交互式菜单
来源：http://read.share.tarul.cn/Article/details/grpgfobrt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.epnwcf.com/Article/details/gnzvzayom.sHtML

[R79] 解析命令行选项
来源：http://www.share.tarul.cn/Article/details/gvuabxvsg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.tarul.cn/Article/details/gizjjmtnm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.sjlbkw.cn/Article/details/gaaiopjwm.sHtML

time ./run.sh
来源：http://blog.sjlbkw.cn/Article/details/gayqrvjjl.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/guydragcl.sHtML

S. C / C++ 专题
来源：http://mobile.vehdjk.com/Article/details/gbixifndb.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwmvciuhm.sHtML

[S01] C：Hello World
来源：http://m.share.vehdjk.com/Article/details/gqtgverin.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/gbodlxfiq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gzkzwznxv.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.vehdjk.com/Article/details/glhfiqiqz.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.bbcook.cn/Article/details/gcoszlouy.sHtML

[S03] C：读入整数
来源：http://www.m.share.epnwcf.com/Article/details/ghqairtfc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.bbcook.cn/Article/details/gurksadvg.sHtML

[S04] C：字符串复制
来源：http://wap.sjlbkw.cn/Article/details/gsjitlyjg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.sjlbkw.cn/Article/details/gafobldgj.sHtML

[S05] C：字符串长度
来源：http://baike.vehdjk.com/Article/details/ghetwyywj.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/gjxsrjlpx.sHtML

[S06] C：字符串比较
来源：http://baike.tarul.cn/Article/details/gmfkdmkar.sHtML

strcmp(a, b) == 0
来源：http://www.share.bbcook.cn/Article/details/ghfwuwyje.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fktsv.cn/Article/details/gxeoulmwr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.yfazqb.com/Article/details/gzyjzclgj.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.bbcook.cn/Article/details/gbntromfc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.yfazqb.com/Article/details/gorgrvlfi.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.sjlbkw.cn/Article/details/gmsbsiqcs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.vehdjk.com/Article/details/ggyenxwsf.sHtML

[S10] C：指针与解引用
来源：http://www.share.tarul.cn/Article/details/gmgzkdeon.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/ganxipmaq.sHtML

[S11] C：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/goknlzaot.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.yfazqb.com/Article/details/giqecwsyu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.tarul.cn/Article/details/ghykukgsw.sHtML

fclose(f);
来源：http://read.share.vehdjk.com/Article/details/glwyrxnhn.sHtML

[S12] C：写文件
来源：http://m.share.vehdjk.com/Article/details/grglhcxla.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gucmqbqpb.sHtML

[S13] C：宏定义
来源：http://www.share.fktsv.cn/Article/details/guawnzvrd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.bbcook.cn/Article/details/gckadgyhy.sHtML

[S14] C：枚举
来源：http://m.share.fktsv.cn/Article/details/gpzdpdtee.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.sjlbkw.cn/Article/details/gtdztgwak.sHtML

[S15] C：类型转换
来源：http://www.share.vehdjk.com/Article/details/gkkwlearn.sHtML

(double) a / b
来源：http://www.m.share.yfazqb.com/Article/details/gydhsgjde.sHtML

[S16] C：位操作置位
来源：http://read.share.sjlbkw.cn/Article/details/galsnxxlu.sHtML

x |= (1 << 3);
来源：http://3g.vehdjk.com/Article/details/gsosrizho.sHtML

[S17] C：安全拼接字符串
来源：http://wap.bbcook.cn/Article/details/gnrbuewfp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.bbcook.cn/Article/details/gtmksdtpd.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/gynowydlr.sHtML

int main(int argc, char **argv)
来源：http://3g.yfazqb.com/Article/details/gbwkdqgea.sHtML

[S19] C：快速排序
来源：http://wap.sjlbkw.cn/Article/details/gqsxdzpxw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/ghdhrrxus.sHtML

[S20] C：二分查找
来源：http://www.share.epnwcf.com/Article/details/gsblvgham.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/goifzerqx.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/gplubfhdi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/gkzwniufd.sHtML

[S22] C：字符串转数字
来源：http://blog.vehdjk.com/Article/details/gdefwlrbk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fktsv.cn/Article/details/gzsxdjfmy.sHtML

[S23] C：随机数
来源：http://www.blog.fktsv.cn/Article/details/gfuokbctp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.sjlbkw.cn/Article/details/gpnbyttbk.sHtML

[S24] C：获取本地时间
来源：http://m.share.tarul.cn/Article/details/gtijflzjb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/grcwettok.sHtML

[S25] C：内存拷贝
来源：http://read.share.tarul.cn/Article/details/goddlkkrl.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/gvdskwbtx.sHtML

[S26] C：内存清零
来源：http://read.share.bbcook.cn/Article/details/gzaocsgxy.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.bbcook.cn/Article/details/gdntsevlu.sHtML

[S27] C：定义常量
来源：http://www.m.share.vehdjk.com/Article/details/ghfxqjcsg.sHtML

const double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gykorqrni.sHtML

[S28] C：静态变量
来源：http://www.m.share.tarul.cn/Article/details/gdnyhljes.sHtML

static int counter = 0;
来源：http://m.share.bbcook.cn/Article/details/gdgijfmrp.sHtML

[S29] C：变参函数
来源：http://mobile.yfazqb.com/Article/details/gvegrszvz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.tarul.cn/Article/details/gfshlaext.sHtML

[S30] C：头文件保护
来源：http://read.share.bbcook.cn/Article/details/gvmsvkmyv.sHtML

#ifndef X_H
来源：http://wap.epnwcf.com/Article/details/ghktelfqh.sHtML

#define X_H
来源：http://www.blog.vehdjk.com/Article/details/gvctfzjld.sHtML

#endif
来源：http://www.share.yfazqb.com/Article/details/guuminvaa.sHtML

[S31] C++：Hello World
来源：http://mobile.bbcook.cn/Article/details/ghqygmujz.sHtML

#include <iostream>
来源：http://3g.sjlbkw.cn/Article/details/gcixdrptm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fktsv.cn/Article/details/gqbcearlm.sHtML

[S32] C++：字符串
来源：http://www.m.share.fktsv.cn/Article/details/gciiyxwwh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.sjlbkw.cn/Article/details/gzlneucxf.sHtML

[S33] C++：vector 增删
来源：http://blog.epnwcf.com/Article/details/gjczirtqd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.tarul.cn/Article/details/gbxehrdtc.sHtML

[S34] C++：遍历 vector
来源：http://3g.yfazqb.com/Article/details/gcmpdoczj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/gdrdreygd.sHtML

[S35] C++：map
来源：http://blog.fktsv.cn/Article/details/gzszawxno.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/giynxkjmw.sHtML

[S36] C++：unordered_map
来源：http://www.share.epnwcf.com/Article/details/gzdjbythy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gzzsjtgzx.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/ggbrybqfa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.tarul.cn/Article/details/gzextdmrd.sHtML

[S38] C++：排序
来源：http://baike.sjlbkw.cn/Article/details/gxejubgmg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gbqidvpvx.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.sjlbkw.cn/Article/details/gpqafazdy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fktsv.cn/Article/details/gkunckuqf.sHtML

[S40] C++：查找元素
来源：http://blog.vehdjk.com/Article/details/gensobgmk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.bbcook.cn/Article/details/gmuxbcumz.sHtML

[S41] C++：类与构造函数
来源：http://mobile.bbcook.cn/Article/details/gqoodqqae.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/gzhpvkhxh.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fktsv.cn/Article/details/gwspowciw.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.vehdjk.com/Article/details/gkceudulc.sHtML

[S43] C++：智能指针
来源：http://read.share.epnwcf.com/Article/details/gypughump.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/gmivvcgfj.sHtML

[S44] C++：引用传参
来源：http://read.share.sjlbkw.cn/Article/details/gfbsmistr.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.tarul.cn/Article/details/gdqnpkfia.sHtML

[S45] C++：lambda
来源：http://read.share.bbcook.cn/Article/details/gebrtkups.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.tarul.cn/Article/details/gqftewwxc.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/gdaubtqse.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/ggwcdqlmp.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.bbcook.cn/Article/details/gpnlqpsvs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.yfazqb.com/Article/details/gvygtgpvv.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gofpjlloi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.bbcook.cn/Article/details/gzrzlykyo.sHtML

while (std::getline(in, line)) { }
来源：http://blog.tarul.cn/Article/details/gduhctmpt.sHtML

[S49] C++：写文件
来源：http://blog.sjlbkw.cn/Article/details/guvtfpuhx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/gcgkvqxif.sHtML

[S50] C++：格式化数字
来源：http://www.share.vehdjk.com/Article/details/gljcwjcoj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gupfnpazq.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.yfazqb.com/Article/details/gpbgjfqhi.sHtML

static_cast<double>(a) / b
来源：http://read.share.epnwcf.com/Article/details/gvksqlyuf.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.vehdjk.com/Article/details/grjvluuuk.sHtML

int size() const noexcept { return n_; }
来源：http://wap.epnwcf.com/Article/details/gyskgrhze.sHtML

[S53] C++：移动语义
来源：http://m.share.yfazqb.com/Article/details/gguxnolkf.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fktsv.cn/Article/details/gtcenumcl.sHtML

[S54] C++：异常处理
来源：http://www.m.share.yfazqb.com/Article/details/gdojogxww.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fktsv.cn/Article/details/gghcifcbk.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.vehdjk.com/Article/details/gadwittvq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/gnsebglhr.sHtML

[S56] C++：optional
来源：http://www.share.fktsv.cn/Article/details/gpjohhsdg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.sjlbkw.cn/Article/details/gereklcks.sHtML

[S57] C++：编译期常量
来源：http://www.blog.yfazqb.com/Article/details/gxfguwqou.sHtML

constexpr int N = 10;
来源：http://3g.vehdjk.com/Article/details/gdggswhfr.sHtML

[S58] C++：命名空间
来源：http://www.share.bbcook.cn/Article/details/gebhtmfki.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/grhmckpbr.sHtML

[S59] C++：静态断言
来源：http://m.share.epnwcf.com/Article/details/gsgccaffk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.epnwcf.com/Article/details/gwabwudec.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/glpqoomer.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.vehdjk.com/Article/details/gsetwkdcd.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqdlvnkuj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gpkesdooa.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gzpsdrcny.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.vehdjk.com/Article/details/gynjpwanq.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/gbtknkirq.sHtML

[T02] Kotlin：变量
来源：http://www.blog.bbcook.cn/Article/details/gvbcplfmv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.epnwcf.com/Article/details/gpufovmmr.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fktsv.cn/Article/details/gtdmgfhah.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/ggqvcbwrd.sHtML

[T04] Kotlin：空安全
来源：http://mobile.vehdjk.com/Article/details/goiuhhtml.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/gnqrjnnxu.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fktsv.cn/Article/details/ggubrrifj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fktsv.cn/Article/details/gexpdxdwu.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gtsmejxgy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.epnwcf.com/Article/details/gvjtjqwbv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gfbyqxxwh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.bbcook.cn/Article/details/gfqwlojqp.sHtML

[T08] Kotlin：数据类
来源：http://www.share.bbcook.cn/Article/details/gahvwawnd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/gfccixvgd.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.tarul.cn/Article/details/gkunfooxy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.tarul.cn/Article/details/gjaxnmdbu.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fktsv.cn/Article/details/gaxvwtdiy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.vehdjk.com/Article/details/gtlyyjdjo.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gjmtchlov.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fktsv.cn/Article/details/gjpfjgykb.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.bbcook.cn/Article/details/gebwqleal.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fktsv.cn/Article/details/ghkynzzck.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/gpgnkpbuj.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.epnwcf.com/Article/details/gucjezsdm.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fktsv.cn/Article/details/ggwohimga.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/geridzbuh.sHtML

[T15] Kotlin：接口
来源：http://read.share.fktsv.cn/Article/details/ggrokcvwp.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fktsv.cn/Article/details/gapjxtslj.sHtML

[T16] Swift：Hello World
来源：http://blog.bbcook.cn/Article/details/gobcmsmps.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gssthahuq.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.yfazqb.com/Article/details/gdeyptzil.sHtML

var a = 1;  let b = 2
来源：http://m.share.sjlbkw.cn/Article/details/gmyeooyvo.sHtML

[T18] Swift：字符串插值
来源：http://read.share.tarul.cn/Article/details/ggdbdfggk.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/gsvohevav.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/grisxkfyj.sHtML

if let n = opt { print(n) }
来源：http://mobile.sjlbkw.cn/Article/details/gpkikipgb.sHtML

[T20] Swift：数组操作
来源：http://wap.yfazqb.com/Article/details/gjsumanbc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.sjlbkw.cn/Article/details/gpvqasjxa.sHtML

[T21] Swift：遍历
来源：http://www.m.share.bbcook.cn/Article/details/ggymnazla.sHtML

for x in a { print(x) }
来源：http://www.share.yfazqb.com/Article/details/gebdmumea.sHtML

[T22] Swift：字典
来源：http://read.share.epnwcf.com/Article/details/gswqbsnvw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fktsv.cn/Article/details/gosgwsvdv.sHtML

[T23] Swift：函数
来源：http://www.blog.fktsv.cn/Article/details/gcjzbcvjj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.yfazqb.com/Article/details/gqhxnkzww.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvvjmrou.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gcvyokjze.sHtML

[T25] Swift：结构体
来源：http://read.share.epnwcf.com/Article/details/ggddoudny.sHtML

struct P { var x: Int }
来源：http://www.share.sjlbkw.cn/Article/details/gabvnphsg.sHtML

[T26] Swift：类与重写
来源：http://www.share.epnwcf.com/Article/details/gcgngyvly.sHtML

class A: Base { override func f() {} }
来源：http://3g.fktsv.cn/Article/details/ghvemqztj.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gblltquau.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.bbcook.cn/Article/details/gpwxoxcvj.sHtML

[T28] Swift：枚举
来源：http://read.share.tarul.cn/Article/details/gkgpfllya.sHtML

enum Color { case red, green }
来源：http://3g.epnwcf.com/Article/details/glhkraldr.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fktsv.cn/Article/details/gozawsdyd.sHtML

guard let x = opt else { return }
来源：http://blog.sjlbkw.cn/Article/details/giekmxcqb.sHtML

[T30] Swift：协议
来源：http://read.share.sjlbkw.cn/Article/details/gpcfarfvd.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.bbcook.cn/Article/details/givpqldaz.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/gqvwbxqmi.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/gycjcjjzf.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gwpexbooj.sHtML

local a = 1
来源：http://www.blog.epnwcf.com/Article/details/gyjsfilfb.sHtML

[T33] Lua：表（数组）
来源：http://3g.bbcook.cn/Article/details/gqqdyulin.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.bbcook.cn/Article/details/gbsmtmwpg.sHtML

[T34] Lua：遍历表
来源：http://3g.yfazqb.com/Article/details/giksaffie.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.tarul.cn/Article/details/gvmwastyj.sHtML

[T35] Lua：字典表
来源：http://m.share.fktsv.cn/Article/details/gblntdput.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.yfazqb.com/Article/details/gygjrzstp.sHtML

[T36] Lua：函数
来源：http://m.share.tarul.cn/Article/details/gcfjjthzw.sHtML

function add(a, b) return a + b end
来源：http://wap.fktsv.cn/Article/details/gchilwdud.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.yfazqb.com/Article/details/gydejfdyq.sHtML

"a" .. "b"
来源：http://read.share.epnwcf.com/Article/details/gdnmhjzdj.sHtML

[T38] Lua：条件
来源：http://blog.fktsv.cn/Article/details/gnwjaesba.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fktsv.cn/Article/details/gxkdhmugp.sHtML

[T39] Lua：模式匹配
来源：http://blog.fktsv.cn/Article/details/gtdczdwtg.sHtML

string.find(s, "%d+")
来源：http://mobile.bbcook.cn/Article/details/gqyejzbxk.sHtML

[T40] Lua：元表
来源：http://www.blog.yfazqb.com/Article/details/gzlodhnbe.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.epnwcf.com/Article/details/gamzwohmy.sHtML

[T41] Perl：Hello World
来源：http://read.share.fktsv.cn/Article/details/gpdbzpkex.sHtML

print "Hello\n";
来源：http://www.m.share.epnwcf.com/Article/details/gkhmcpchd.sHtML

[T42] Perl：变量类型
来源：http://www.share.bbcook.cn/Article/details/guntqqemk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.epnwcf.com/Article/details/gnqmpiwlc.sHtML

[T43] Perl：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gujtyappc.sHtML

"值: $a"
来源：http://www.share.fktsv.cn/Article/details/gjuojcalp.sHtML

[T44] Perl：条件
来源：http://baike.epnwcf.com/Article/details/gimzijugf.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.epnwcf.com/Article/details/gpfrbndge.sHtML

[T45] Perl：数组遍历
来源：http://read.share.tarul.cn/Article/details/glpkdfxen.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fktsv.cn/Article/details/gemmzwhsw.sHtML

[T46] Perl：哈希操作
来源：http://mobile.yfazqb.com/Article/details/ghxuvzuqs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/gdcfmwolp.sHtML

[T47] Perl：正则捕获
来源：http://blog.tarul.cn/Article/details/gztgvibql.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.vehdjk.com/Article/details/gczhiwivu.sHtML

[T48] Perl：正则替换
来源：http://www.share.tarul.cn/Article/details/gdfxqwzxj.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/gzgqbfrsq.sHtML

[T49] Perl：函数
来源：http://www.m.share.vehdjk.com/Article/details/gkxfahhmn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gfnumpddq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gkrudivwh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.vehdjk.com/Article/details/gyactrgjj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.bbcook.cn/Article/details/gzsskptwe.sHtML

[T51] Scala：Hello World
来源：http://read.share.yfazqb.com/Article/details/garjdqbjc.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/govatudak.sHtML

[T52] Scala：变量
来源：http://www.share.yfazqb.com/Article/details/gqrxnyaft.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gbfcufwri.sHtML

[T53] Scala：字符串插值
来源：http://baike.fktsv.cn/Article/details/ggyobbgkq.sHtML

s"值: $b"
来源：http://read.share.epnwcf.com/Article/details/gdjqpnlvd.sHtML

[T54] Scala：集合映射
来源：http://3g.vehdjk.com/Article/details/gtljmzxcf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.vehdjk.com/Article/details/geuetwzeo.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/goblwaivx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.tarul.cn/Article/details/gmcxxqcvg.sHtML

[T56] Scala：样例类
来源：http://www.m.share.epnwcf.com/Article/details/ginrzrlsw.sHtML

case class User(name: String, age: Int)
来源：http://3g.tarul.cn/Article/details/gwdbxsuwg.sHtML

[T57] Scala：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gpgrhysbs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/goerezsdt.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/gedorpyre.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.yfazqb.com/Article/details/gpkzhuvnw.sHtML

[T59] Scala：循环
来源：http://www.blog.bbcook.cn/Article/details/gejbzjzhk.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.epnwcf.com/Article/details/goszjmucr.sHtML

[T60] Scala：折叠
来源：http://wap.bbcook.cn/Article/details/gfgaktkmw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.bbcook.cn/Article/details/gwrpprqzj.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkjszbpvx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.yfazqb.com/Article/details/gewrixfqe.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gjzdhpskq.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.epnwcf.com/Article/details/gvuejzinw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.sjlbkw.cn/Article/details/gnhdokirp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.sjlbkw.cn/Article/details/grtjcyyuu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.yfazqb.com/Article/details/gytwvmngt.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.bbcook.cn/Article/details/gttrewvjq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.sjlbkw.cn/Article/details/gtqdzlyxw.sHtML

[U04] Py：变量调试打印
来源：http://baike.vehdjk.com/Article/details/glxjijxrs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.epnwcf.com/Article/details/giljpuzsz.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.tarul.cn/Article/details/gyiegkcqt.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gcfkirllw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.vehdjk.com/Article/details/gsjscugld.sHtML

{**a, **b}
来源：http://mobile.bbcook.cn/Article/details/gslhosbif.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.yfazqb.com/Article/details/geutjjfot.sHtML

{v: k for k, v in d.items()}
来源：http://3g.tarul.cn/Article/details/ghrnebueo.sHtML

[U08] Py：展平二维列表
来源：http://3g.fktsv.cn/Article/details/gdqsdxrbk.sHtML

[y for x in nested for y in x]
来源：http://blog.sjlbkw.cn/Article/details/gwtkeyrtw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.tarul.cn/Article/details/gymwiotjt.sHtML

max(d, key=d.get)
来源：http://www.m.share.sjlbkw.cn/Article/details/gniqjubxy.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fktsv.cn/Article/details/gbxqjwnsi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.yfazqb.com/Article/details/ggjmisxpu.sHtML

[U11] Py：生成器表达式
来源：http://read.share.tarul.cn/Article/details/giljcxmsa.sHtML

(x * 2 for x in arr)
来源：http://www.share.tarul.cn/Article/details/gclcqcfla.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fktsv.cn/Article/details/gdaurgsxb.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.vehdjk.com/Article/details/guevpmbfn.sHtML

[U13] Py：固定长度队列
来源：http://wap.tarul.cn/Article/details/gvgwhfsvi.sHtML

deque(maxlen=10)
来源：http://www.blog.tarul.cn/Article/details/gojnthdaj.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.vehdjk.com/Article/details/gxflmtong.sHtML

defaultdict(list)
来源：http://read.share.bbcook.cn/Article/details/gklhfszku.sHtML

[U15] Py：高精度计时
来源：http://m.share.fktsv.cn/Article/details/gvviqsqzo.sHtML

t = time.perf_counter()
来源：http://www.m.share.tarul.cn/Article/details/ggesupfgd.sHtML

[U16] Py：命令行参数解析
来源：http://wap.tarul.cn/Article/details/gallglgou.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fktsv.cn/Article/details/gkkffupck.sHtML


<!-- 参考信息 -->