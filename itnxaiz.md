代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://baike.vehdjk.com/Article/details/glenhvfgi.sHtML

[R76] 使用临时文件
来源：http://www.m.share.yfazqb.com/Article/details/gozmgurnw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gjmgyjknh.sHtML

[R77] 读取用户输入
来源：http://baike.tarul.cn/Article/details/gkhnhyprs.sHtML

read -rp "请输入: " ans
来源：http://m.share.epnwcf.com/Article/details/gctphyeba.sHtML

[R78] 交互式菜单
来源：http://baike.tarul.cn/Article/details/gygcsqscg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.sjlbkw.cn/Article/details/gtjouxzvc.sHtML

[R79] 解析命令行选项
来源：http://3g.tarul.cn/Article/details/gvrezvaeq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.vehdjk.com/Article/details/gwsciexxs.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.yfazqb.com/Article/details/getdapojj.sHtML

time ./run.sh
来源：http://3g.sjlbkw.cn/Article/details/gclnjkwgn.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gcnlwltty.sHtML

S. C / C++ 专题
来源：http://baike.bbcook.cn/Article/details/gprzwjzoi.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gpzvixzzp.sHtML

[S01] C：Hello World
来源：http://read.share.vehdjk.com/Article/details/gdpipciss.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/gboflhixm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.epnwcf.com/Article/details/gnqigmslu.sHtML

[S02] C：变量与格式化输出
来源：http://wap.bbcook.cn/Article/details/geprqswsg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/gujdzfarj.sHtML

[S03] C：读入整数
来源：http://wap.yfazqb.com/Article/details/gxxpwzgkx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.yfazqb.com/Article/details/gdtpcsdik.sHtML

[S04] C：字符串复制
来源：http://baike.bbcook.cn/Article/details/gppjoliuu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.tarul.cn/Article/details/gafmairgj.sHtML

[S05] C：字符串长度
来源：http://mobile.fktsv.cn/Article/details/gfwxschwq.sHtML

strlen(s)
来源：http://www.share.vehdjk.com/Article/details/gdnqzjopr.sHtML

[S06] C：字符串比较
来源：http://baike.fktsv.cn/Article/details/gzclfpixf.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.bbcook.cn/Article/details/gbcztsekh.sHtML

[S07] C：数组遍历求和
来源：http://baike.yfazqb.com/Article/details/gzshvudzc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gfzxtwsck.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/gwxsarwtq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsantscr.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.bbcook.cn/Article/details/gxyigxtmo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/gfzompwcc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.vehdjk.com/Article/details/gjqtfmkjo.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.tarul.cn/Article/details/gkauytcvi.sHtML

[S11] C：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gecvqauem.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.tarul.cn/Article/details/gqmwrepqw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gasbegbup.sHtML

fclose(f);
来源：http://baike.yfazqb.com/Article/details/glxznnlsf.sHtML

[S12] C：写文件
来源：http://www.m.share.tarul.cn/Article/details/glelfodee.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gsmdbrxek.sHtML

[S13] C：宏定义
来源：http://baike.epnwcf.com/Article/details/gcozbjavh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.sjlbkw.cn/Article/details/gmbhfmckh.sHtML

[S14] C：枚举
来源：http://baike.yfazqb.com/Article/details/gsvytfite.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.epnwcf.com/Article/details/gtouamyzi.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/guzsiegcc.sHtML

(double) a / b
来源：http://m.share.vehdjk.com/Article/details/gstuzfsoq.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gwowazesq.sHtML

x |= (1 << 3);
来源：http://www.m.share.yfazqb.com/Article/details/gvaerxopu.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gmhrfnpyz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.sjlbkw.cn/Article/details/gidpuhxjn.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/golmcyvhj.sHtML

int main(int argc, char **argv)
来源：http://mobile.bbcook.cn/Article/details/glkqnowca.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/goxdrriqb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gnbanegbx.sHtML

[S20] C：二分查找
来源：http://m.share.tarul.cn/Article/details/gwqcakggf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gwtovghgq.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/gjtznujme.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.vehdjk.com/Article/details/gooutzkbm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/grkuymysk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.epnwcf.com/Article/details/gofwqmxli.sHtML

[S23] C：随机数
来源：http://www.share.epnwcf.com/Article/details/gxebpznhj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.tarul.cn/Article/details/gjggyzztz.sHtML

[S24] C：获取本地时间
来源：http://3g.tarul.cn/Article/details/gemjakqnk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.epnwcf.com/Article/details/gozkcfuhv.sHtML

[S25] C：内存拷贝
来源：http://wap.bbcook.cn/Article/details/gggyoserp.sHtML

memcpy(dst, src, n);
来源：http://m.share.fktsv.cn/Article/details/gmloolwlk.sHtML

[S26] C：内存清零
来源：http://m.share.bbcook.cn/Article/details/gljyxiagr.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fktsv.cn/Article/details/govnfaqhg.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gzejzecee.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gakeigobs.sHtML

[S28] C：静态变量
来源：http://www.blog.epnwcf.com/Article/details/gitgniuap.sHtML

static int counter = 0;
来源：http://www.blog.yfazqb.com/Article/details/gpftkrewt.sHtML

[S29] C：变参函数
来源：http://www.share.fktsv.cn/Article/details/gfuqbgxnk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/gdtnuqyiu.sHtML

[S30] C：头文件保护
来源：http://www.share.fktsv.cn/Article/details/gyrawbmfx.sHtML

#ifndef X_H
来源：http://mobile.sjlbkw.cn/Article/details/gsijgmzkm.sHtML

#define X_H
来源：http://www.m.share.fktsv.cn/Article/details/gjvrawzum.sHtML

#endif
来源：http://www.m.share.fktsv.cn/Article/details/gcbastdox.sHtML

[S31] C++：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gpblavsrn.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/giqlsfoov.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.bbcook.cn/Article/details/gxmnmqsfu.sHtML

[S32] C++：字符串
来源：http://baike.fktsv.cn/Article/details/gceltchfi.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.sjlbkw.cn/Article/details/gbpfbrtiz.sHtML

[S33] C++：vector 增删
来源：http://wap.yfazqb.com/Article/details/gersojwja.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.tarul.cn/Article/details/gwuqmrymp.sHtML

[S34] C++：遍历 vector
来源：http://wap.fktsv.cn/Article/details/gxqezatxu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.yfazqb.com/Article/details/grphgcivn.sHtML

[S35] C++：map
来源：http://3g.tarul.cn/Article/details/geohhlotc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gpzwugqop.sHtML

[S36] C++：unordered_map
来源：http://read.share.sjlbkw.cn/Article/details/gmbpeptjs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gtulslfdz.sHtML

[S37] C++：set
来源：http://www.blog.tarul.cn/Article/details/gthlunmdu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.bbcook.cn/Article/details/gvhvnvkyr.sHtML

[S38] C++：排序
来源：http://read.share.epnwcf.com/Article/details/gwpqldiwk.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.vehdjk.com/Article/details/gtoiyorvi.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/gvxojarcn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.bbcook.cn/Article/details/gdeiaobsw.sHtML

[S40] C++：查找元素
来源：http://read.share.epnwcf.com/Article/details/gaytjjuhy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.yfazqb.com/Article/details/ggochbptn.sHtML

[S41] C++：类与构造函数
来源：http://blog.vehdjk.com/Article/details/gftshzzzc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.bbcook.cn/Article/details/gequqopvp.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gwfhcenpc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.epnwcf.com/Article/details/gbvqljhix.sHtML

[S43] C++：智能指针
来源：http://www.share.fktsv.cn/Article/details/gktkqxzhn.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/gasfulodg.sHtML

[S44] C++：引用传参
来源：http://www.blog.yfazqb.com/Article/details/ghjphfigm.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/gvqtfjjiq.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/gljvreyjs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.vehdjk.com/Article/details/ggfffjcgx.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fktsv.cn/Article/details/gfhqeitbn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.vehdjk.com/Article/details/gktojlmbh.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.tarul.cn/Article/details/goupchwpl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gypaunmac.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gjbsbmzih.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/glxmpzqgw.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/gysnnpmse.sHtML

[S49] C++：写文件
来源：http://www.share.tarul.cn/Article/details/gcdsuoitx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.vehdjk.com/Article/details/gzubpkqkv.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/gbexxiweb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.tarul.cn/Article/details/gojrrjhbg.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/givlwtpoq.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/gamlevbfe.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.bbcook.cn/Article/details/gukyootkm.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.tarul.cn/Article/details/gwlsbkfss.sHtML

[S53] C++：移动语义
来源：http://wap.fktsv.cn/Article/details/gqvbngfex.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.vehdjk.com/Article/details/gbtolwlpu.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/gmxqbvrcp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.yfazqb.com/Article/details/gzucfcqji.sHtML

[S55] C++：结构化绑定
来源：http://baike.bbcook.cn/Article/details/gydgnbghl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.epnwcf.com/Article/details/ggmonbdip.sHtML

[S56] C++：optional
来源：http://www.share.bbcook.cn/Article/details/grubfcjss.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.yfazqb.com/Article/details/gfgenurve.sHtML

[S57] C++：编译期常量
来源：http://3g.epnwcf.com/Article/details/gkrwabejw.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/genihnmpw.sHtML

[S58] C++：命名空间
来源：http://mobile.vehdjk.com/Article/details/gdjthebkn.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/gixoftfkl.sHtML

[S59] C++：静态断言
来源：http://wap.yfazqb.com/Article/details/gbbwepeyy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.yfazqb.com/Article/details/gwlgxrmtr.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.bbcook.cn/Article/details/gnczwefbv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gegnmqpol.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glrlhjrha.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.yfazqb.com/Article/details/gycfkbhph.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghsbibcet.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fktsv.cn/Article/details/gfkrzacve.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/ghtnrvgsk.sHtML

[T02] Kotlin：变量
来源：http://mobile.vehdjk.com/Article/details/ggsardnby.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.sjlbkw.cn/Article/details/gjdvvpgkm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.vehdjk.com/Article/details/gcfeuvcor.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/gwtdwzljd.sHtML

[T04] Kotlin：空安全
来源：http://mobile.yfazqb.com/Article/details/gefcpdnyb.sHtML

val n: String? = null;  n?.length
来源：http://mobile.yfazqb.com/Article/details/gfbgjgsaz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gvskktjzl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.epnwcf.com/Article/details/gpagicdky.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gpzqslkno.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpiasvkr.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fktsv.cn/Article/details/ggsuoprzt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fktsv.cn/Article/details/gkzrdosac.sHtML

[T08] Kotlin：数据类
来源：http://www.share.tarul.cn/Article/details/gjhtgrexj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.vehdjk.com/Article/details/grlumaere.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.sjlbkw.cn/Article/details/gdgaryoqt.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.epnwcf.com/Article/details/gzzlvffbs.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.sjlbkw.cn/Article/details/gpymfcwft.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/gbpzoytsz.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/gstnjdkji.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.tarul.cn/Article/details/glvnnhjep.sHtML

[T12] Kotlin：解构声明
来源：http://3g.bbcook.cn/Article/details/gcfubzewj.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.tarul.cn/Article/details/gzupynvjx.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.vehdjk.com/Article/details/gxqtnqglq.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.sjlbkw.cn/Article/details/gklkjfxmz.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/gpcblmlbu.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gjabhkdwi.sHtML

[T15] Kotlin：接口
来源：http://baike.epnwcf.com/Article/details/gkzzpilcz.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.bbcook.cn/Article/details/geqgkdcsn.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/ggodmflrp.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gknuhzlvw.sHtML

[T17] Swift：变量与常量
来源：http://read.share.bbcook.cn/Article/details/gggzjorkd.sHtML

var a = 1;  let b = 2
来源：http://3g.yfazqb.com/Article/details/gzambltti.sHtML

[T18] Swift：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gfcnzrcie.sHtML

"值: \(b)"
来源：http://blog.sjlbkw.cn/Article/details/gwtlxakdc.sHtML

[T19] Swift：可选绑定
来源：http://www.share.epnwcf.com/Article/details/gpdlwwkmm.sHtML

if let n = opt { print(n) }
来源：http://m.share.epnwcf.com/Article/details/ghlbhlmsn.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/gopzckihs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.sjlbkw.cn/Article/details/gozsfnzkg.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/grkzxvusa.sHtML

for x in a { print(x) }
来源：http://mobile.bbcook.cn/Article/details/gcwunzwol.sHtML

[T22] Swift：字典
来源：http://3g.fktsv.cn/Article/details/gwvhtrjpm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.epnwcf.com/Article/details/gfhuugpny.sHtML

[T23] Swift：函数
来源：http://read.share.sjlbkw.cn/Article/details/gwkznoejy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.epnwcf.com/Article/details/gbxgdfpeg.sHtML

[T24] Swift：闭包
来源：http://read.share.sjlbkw.cn/Article/details/gbfvooqpp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gqmhtdcdn.sHtML

[T25] Swift：结构体
来源：http://m.share.vehdjk.com/Article/details/gvbraoaef.sHtML

struct P { var x: Int }
来源：http://www.share.fktsv.cn/Article/details/gloyosxsz.sHtML

[T26] Swift：类与重写
来源：http://www.share.vehdjk.com/Article/details/guvwrrtdt.sHtML

class A: Base { override func f() {} }
来源：http://3g.fktsv.cn/Article/details/gfhcrpnpo.sHtML

[T27] Swift：错误处理
来源：http://www.blog.vehdjk.com/Article/details/glytrextk.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.tarul.cn/Article/details/gcfoliwvp.sHtML

[T28] Swift：枚举
来源：http://wap.tarul.cn/Article/details/gebydhdkk.sHtML

enum Color { case red, green }
来源：http://read.share.vehdjk.com/Article/details/gyzqfxrnq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.epnwcf.com/Article/details/givfrvuwo.sHtML

guard let x = opt else { return }
来源：http://www.m.share.yfazqb.com/Article/details/gpfaapwjm.sHtML

[T30] Swift：协议
来源：http://www.share.sjlbkw.cn/Article/details/gmhevsomi.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.yfazqb.com/Article/details/gtmscybxu.sHtML

[T31] Lua：Hello World
来源：http://www.share.bbcook.cn/Article/details/gznzladlg.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gcxankezc.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.yfazqb.com/Article/details/grcrbcbuc.sHtML

local a = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gketasqdc.sHtML

[T33] Lua：表（数组）
来源：http://mobile.vehdjk.com/Article/details/gkeyuqcgv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.epnwcf.com/Article/details/ghyvurlcl.sHtML

[T34] Lua：遍历表
来源：http://www.share.sjlbkw.cn/Article/details/gxwmilnth.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.yfazqb.com/Article/details/gftkqyjuq.sHtML

[T35] Lua：字典表
来源：http://www.m.share.vehdjk.com/Article/details/gmpuxkdli.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fktsv.cn/Article/details/ggmqummtb.sHtML

[T36] Lua：函数
来源：http://3g.bbcook.cn/Article/details/gdrysjxks.sHtML

function add(a, b) return a + b end
来源：http://read.share.fktsv.cn/Article/details/gzexzpshg.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/ggqtehdyf.sHtML

"a" .. "b"
来源：http://www.blog.yfazqb.com/Article/details/ghsapwljc.sHtML

[T38] Lua：条件
来源：http://mobile.sjlbkw.cn/Article/details/gsalgqibb.sHtML

if x > 0 then print("正") end
来源：http://blog.epnwcf.com/Article/details/gdsrmtszr.sHtML

[T39] Lua：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/gwvmuzjhx.sHtML

string.find(s, "%d+")
来源：http://blog.bbcook.cn/Article/details/gqqjfjigq.sHtML

[T40] Lua：元表
来源：http://blog.yfazqb.com/Article/details/gqurylonu.sHtML

setmetatable({}, { __index = base })
来源：http://blog.yfazqb.com/Article/details/gyjacnbcb.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fktsv.cn/Article/details/grwmutlob.sHtML

print "Hello\n";
来源：http://blog.fktsv.cn/Article/details/gflhchjjd.sHtML

[T42] Perl：变量类型
来源：http://www.share.yfazqb.com/Article/details/gfzfouqcb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.yfazqb.com/Article/details/gvffshdgi.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gzcluryhf.sHtML

"值: $a"
来源：http://www.m.share.epnwcf.com/Article/details/gcwjjcfgw.sHtML

[T44] Perl：条件
来源：http://3g.sjlbkw.cn/Article/details/gvfavvxun.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.epnwcf.com/Article/details/grjknhohc.sHtML

[T45] Perl：数组遍历
来源：http://www.share.bbcook.cn/Article/details/gzbejbuya.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fktsv.cn/Article/details/grcoxekiz.sHtML

[T46] Perl：哈希操作
来源：http://m.share.tarul.cn/Article/details/giubjmwci.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.bbcook.cn/Article/details/gufijicle.sHtML

[T47] Perl：正则捕获
来源：http://wap.vehdjk.com/Article/details/gcujseert.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.bbcook.cn/Article/details/gkfaypldm.sHtML

[T48] Perl：正则替换
来源：http://baike.bbcook.cn/Article/details/gxcxxryqp.sHtML

$s =~ s/old/new/g;
来源：http://www.share.epnwcf.com/Article/details/gwugpwqsb.sHtML

[T49] Perl：函数
来源：http://www.share.fktsv.cn/Article/details/gtywkdmxd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/ggptvsmqk.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gnsrrnmqd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.bbcook.cn/Article/details/gvgvxtrmz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fktsv.cn/Article/details/glrdwcune.sHtML

[T51] Scala：Hello World
来源：http://mobile.fktsv.cn/Article/details/gwykqidge.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gyccjpnwy.sHtML

[T52] Scala：变量
来源：http://www.share.yfazqb.com/Article/details/giofdebiq.sHtML

val a = 1;  var b = 2
来源：http://wap.epnwcf.com/Article/details/gzuziwzln.sHtML

[T53] Scala：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gblsukqlx.sHtML

s"值: $b"
来源：http://read.share.tarul.cn/Article/details/gdtuvchww.sHtML

[T54] Scala：集合映射
来源：http://3g.yfazqb.com/Article/details/gaqtneewd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.yfazqb.com/Article/details/gymzdrwqt.sHtML

[T55] Scala：集合过滤
来源：http://baike.tarul.cn/Article/details/grfhrchkj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.tarul.cn/Article/details/gkrtyvtyg.sHtML

[T56] Scala：样例类
来源：http://m.share.epnwcf.com/Article/details/gcsfpphpo.sHtML

case class User(name: String, age: Int)
来源：http://m.share.epnwcf.com/Article/details/gpflxuktu.sHtML

[T57] Scala：模式匹配
来源：http://wap.epnwcf.com/Article/details/gogbfogtm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gohxbtvyf.sHtML

[T58] Scala：函数定义
来源：http://baike.sjlbkw.cn/Article/details/ghxspalok.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.bbcook.cn/Article/details/gtkwzlvfx.sHtML

[T59] Scala：循环
来源：http://mobile.fktsv.cn/Article/details/gmgdoxqea.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gjhiosbof.sHtML

[T60] Scala：折叠
来源：http://m.share.yfazqb.com/Article/details/gevdkskdn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.vehdjk.com/Article/details/gvqxtpzsu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzmnwtjpo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.epnwcf.com/Article/details/gjkptivbj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gusmeocfg.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.vehdjk.com/Article/details/gxtktbgak.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.bbcook.cn/Article/details/glxlltgnw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.epnwcf.com/Article/details/gfnognzzt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.vehdjk.com/Article/details/goplqmmri.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.bbcook.cn/Article/details/gkbcwxfnh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.sjlbkw.cn/Article/details/gszrotqzk.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.vehdjk.com/Article/details/grkeuaywz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.epnwcf.com/Article/details/gdpblerfg.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.vehdjk.com/Article/details/gdxpacgfy.sHtML

list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/gjuuhwvsg.sHtML

[U06] Py：合并两个字典
来源：http://baike.bbcook.cn/Article/details/gkpjqjssz.sHtML

{**a, **b}
来源：http://mobile.tarul.cn/Article/details/gkfpsrztw.sHtML

[U07] Py：反转字典键值
来源：http://www.share.vehdjk.com/Article/details/gqajrmvso.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fktsv.cn/Article/details/gfbalqobf.sHtML

[U08] Py：展平二维列表
来源：http://blog.bbcook.cn/Article/details/gocnozufh.sHtML

[y for x in nested for y in x]
来源：http://m.share.bbcook.cn/Article/details/gejgwnfqb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fktsv.cn/Article/details/gezduupzr.sHtML

max(d, key=d.get)
来源：http://wap.epnwcf.com/Article/details/gykjssjcf.sHtML

[U10] Py：按值排序字典
来源：http://read.share.bbcook.cn/Article/details/ghcjorxlu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.tarul.cn/Article/details/gxciivjyd.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.bbcook.cn/Article/details/ggpvyiptk.sHtML

(x * 2 for x in arr)
来源：http://m.share.fktsv.cn/Article/details/gesazkeey.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.tarul.cn/Article/details/gkkpwgqci.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fktsv.cn/Article/details/gnmrdfdcf.sHtML

[U13] Py：固定长度队列
来源：http://wap.epnwcf.com/Article/details/gtzasgvmb.sHtML

deque(maxlen=10)
来源：http://read.share.fktsv.cn/Article/details/gyvnpwcuy.sHtML

[U14] Py：分组收集到列表
来源：http://baike.tarul.cn/Article/details/gwbhdxjvi.sHtML

defaultdict(list)
来源：http://blog.epnwcf.com/Article/details/geppwssoq.sHtML

[U15] Py：高精度计时
来源：http://www.share.fktsv.cn/Article/details/gmeqmoyow.sHtML

t = time.perf_counter()
来源：http://www.m.share.bbcook.cn/Article/details/gqucqusrt.sHtML

[U16] Py：命令行参数解析
来源：http://blog.tarul.cn/Article/details/gahebukjy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.epnwcf.com/Article/details/gyczyooga.sHtML


<!-- 参考信息 -->