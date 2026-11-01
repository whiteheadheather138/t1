代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.share.sjlbkw.cn/Article/details/gsvebnmdh.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/ghzwnlrfq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gakajglrk.sHtML

[R77] 读取用户输入
来源：http://baike.sjlbkw.cn/Article/details/gksgyxryl.sHtML

read -rp "请输入: " ans
来源：http://read.share.vehdjk.com/Article/details/gdmynntxx.sHtML

[R78] 交互式菜单
来源：http://wap.bbcook.cn/Article/details/gxqowrkrf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.tarul.cn/Article/details/gqqlylsns.sHtML

[R79] 解析命令行选项
来源：http://3g.fktsv.cn/Article/details/gxnxrsuwl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fktsv.cn/Article/details/gdwrssuua.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.vehdjk.com/Article/details/gatvlcyes.sHtML

time ./run.sh
来源：http://baike.tarul.cn/Article/details/gimaoezct.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gokjidqsr.sHtML

S. C / C++ 专题
来源：http://www.share.tarul.cn/Article/details/gkyqxidcq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gtaakymiv.sHtML

[S01] C：Hello World
来源：http://wap.epnwcf.com/Article/details/gbqkppvqv.sHtML

#include <stdio.h>
来源：http://www.share.yfazqb.com/Article/details/gtthxojyp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.vehdjk.com/Article/details/glmidyole.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.tarul.cn/Article/details/gxrpahorh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/gklpcdwzq.sHtML

[S03] C：读入整数
来源：http://baike.tarul.cn/Article/details/greyrgvtg.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/glaciynhl.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/gzicoynua.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fktsv.cn/Article/details/giljvluli.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/ggtwuzjgp.sHtML

strlen(s)
来源：http://mobile.vehdjk.com/Article/details/gztgfwytl.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/gbobfkmnr.sHtML

strcmp(a, b) == 0
来源：http://www.share.fktsv.cn/Article/details/gpbfnpsec.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.vehdjk.com/Article/details/gneywnbxd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fktsv.cn/Article/details/gybwmmzkg.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.vehdjk.com/Article/details/gtudypqds.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.vehdjk.com/Article/details/godjwhjik.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.vehdjk.com/Article/details/gtaglayjl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.bbcook.cn/Article/details/gdiuzjlna.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/gvlcdjrmc.sHtML

int *p = &a;  *p = 5;
来源：http://3g.yfazqb.com/Article/details/glafeqxjq.sHtML

[S11] C：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/ggllhusng.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.bbcook.cn/Article/details/gbjugzwrh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.sjlbkw.cn/Article/details/gjejbipeg.sHtML

fclose(f);
来源：http://3g.yfazqb.com/Article/details/gougpgdtk.sHtML

[S12] C：写文件
来源：http://wap.fktsv.cn/Article/details/ghyuigoad.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gktfshezk.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/gnsosamgn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.epnwcf.com/Article/details/gncfoinpl.sHtML

[S14] C：枚举
来源：http://m.share.vehdjk.com/Article/details/gzgwjyyoh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/gnmdzztri.sHtML

[S15] C：类型转换
来源：http://m.share.yfazqb.com/Article/details/gxncluoxf.sHtML

(double) a / b
来源：http://3g.epnwcf.com/Article/details/givolozjg.sHtML

[S16] C：位操作置位
来源：http://m.share.fktsv.cn/Article/details/gitagzqyc.sHtML

x |= (1 << 3);
来源：http://baike.bbcook.cn/Article/details/gcqrdcsar.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gexfrsaai.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.bbcook.cn/Article/details/gczvycxzo.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gapvlenot.sHtML

int main(int argc, char **argv)
来源：http://m.share.yfazqb.com/Article/details/grcegszbg.sHtML

[S19] C：快速排序
来源：http://read.share.epnwcf.com/Article/details/grrpwxjff.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gkcrftcmo.sHtML

[S20] C：二分查找
来源：http://www.m.share.yfazqb.com/Article/details/gtmktvyxu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gqxjkvmry.sHtML

[S21] C：字符类别判断
来源：http://m.share.tarul.cn/Article/details/gyoasooum.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/gwgjatdrn.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/gbmvbrgum.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.sjlbkw.cn/Article/details/gvxuxdphh.sHtML

[S23] C：随机数
来源：http://m.share.bbcook.cn/Article/details/giuuppbdr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.sjlbkw.cn/Article/details/gdaprleho.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.vehdjk.com/Article/details/gvlhvmljn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/gcastvpdn.sHtML

[S25] C：内存拷贝
来源：http://wap.epnwcf.com/Article/details/gqiymdllp.sHtML

memcpy(dst, src, n);
来源：http://3g.yfazqb.com/Article/details/gswimqfup.sHtML

[S26] C：内存清零
来源：http://www.share.bbcook.cn/Article/details/gxtfpqlgv.sHtML

memset(a, 0, sizeof a);
来源：http://baike.yfazqb.com/Article/details/gunaxojdx.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/gqznuexfg.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gzqgiefjn.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/ghwchydwz.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/gawwgczim.sHtML

[S29] C：变参函数
来源：http://www.m.share.tarul.cn/Article/details/gwxljftga.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.bbcook.cn/Article/details/gznoydiea.sHtML

[S30] C：头文件保护
来源：http://baike.fktsv.cn/Article/details/gtazgrkyp.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/gzakqngcx.sHtML

#define X_H
来源：http://blog.vehdjk.com/Article/details/grcykoyak.sHtML

#endif
来源：http://read.share.fktsv.cn/Article/details/gxfevccku.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/gdwyoltbs.sHtML

#include <iostream>
来源：http://blog.fktsv.cn/Article/details/gqpespavf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/gcvswohqs.sHtML

[S32] C++：字符串
来源：http://mobile.tarul.cn/Article/details/gdonvroka.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.vehdjk.com/Article/details/guemlxfmr.sHtML

[S33] C++：vector 增删
来源：http://www.blog.bbcook.cn/Article/details/gatffzpfh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.vehdjk.com/Article/details/gvxgmksvk.sHtML

[S34] C++：遍历 vector
来源：http://blog.fktsv.cn/Article/details/gmepwjlli.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.vehdjk.com/Article/details/grmhwsiua.sHtML

[S35] C++：map
来源：http://wap.tarul.cn/Article/details/gzokdloze.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxuavoud.sHtML

[S36] C++：unordered_map
来源：http://3g.bbcook.cn/Article/details/gxqlnnytb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gvvakqqju.sHtML

[S37] C++：set
来源：http://www.blog.bbcook.cn/Article/details/gqideepil.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fktsv.cn/Article/details/grmayllkz.sHtML

[S38] C++：排序
来源：http://www.blog.epnwcf.com/Article/details/ggqygruro.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.vehdjk.com/Article/details/gifejyhcb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.vehdjk.com/Article/details/gzrwukifx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.bbcook.cn/Article/details/guxmigwpo.sHtML

[S40] C++：查找元素
来源：http://www.share.epnwcf.com/Article/details/gbwhswxjz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.bbcook.cn/Article/details/gjjmqubsp.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/grblocahu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.epnwcf.com/Article/details/guqantdxh.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/gsaetvnbr.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/gylurqxiu.sHtML

[S43] C++：智能指针
来源：http://3g.epnwcf.com/Article/details/gngfadrhf.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.bbcook.cn/Article/details/glhrkvyvy.sHtML

[S44] C++：引用传参
来源：http://www.blog.sjlbkw.cn/Article/details/gujqxxdlx.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.bbcook.cn/Article/details/gknleqodt.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/gmvpgxose.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.vehdjk.com/Article/details/gnbbfapzn.sHtML

[S46] C++：函数模板
来源：http://blog.tarul.cn/Article/details/gbjgmnagc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.sjlbkw.cn/Article/details/gppekwgva.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.tarul.cn/Article/details/gqnszjhbt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/gurnblgzi.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/ghnvtdslg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.tarul.cn/Article/details/gztjvzvdj.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.tarul.cn/Article/details/gwfjmuxpv.sHtML

[S49] C++：写文件
来源：http://read.share.tarul.cn/Article/details/guyjphoyv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.tarul.cn/Article/details/gxovrqvte.sHtML

[S50] C++：格式化数字
来源：http://read.share.tarul.cn/Article/details/gtapuydun.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gsedawrms.sHtML

[S51] C++：显式类型转换
来源：http://blog.vehdjk.com/Article/details/gnwsvbjch.sHtML

static_cast<double>(a) / b
来源：http://3g.bbcook.cn/Article/details/gjifdpifu.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.bbcook.cn/Article/details/gxoqripqp.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/ggymlvwgy.sHtML

[S53] C++：移动语义
来源：http://www.blog.sjlbkw.cn/Article/details/gmhwhprjn.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.tarul.cn/Article/details/gemquaguc.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/goqjpwruq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.bbcook.cn/Article/details/gpqhqnebw.sHtML

[S55] C++：结构化绑定
来源：http://blog.epnwcf.com/Article/details/glrnjwzlw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.vehdjk.com/Article/details/guyuotgae.sHtML

[S56] C++：optional
来源：http://baike.bbcook.cn/Article/details/ghkykxzsi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gezdrydzk.sHtML

[S57] C++：编译期常量
来源：http://mobile.fktsv.cn/Article/details/gsmtifzmm.sHtML

constexpr int N = 10;
来源：http://read.share.fktsv.cn/Article/details/gonwmzztf.sHtML

[S58] C++：命名空间
来源：http://wap.epnwcf.com/Article/details/gvhprrdht.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.tarul.cn/Article/details/ghawinjxy.sHtML

[S59] C++：静态断言
来源：http://wap.bbcook.cn/Article/details/gxpfuixfr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/gyiqcjwhr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gjwycsywc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gsdjhlelo.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gcmbvjwts.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.epnwcf.com/Article/details/gynncffjv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gsvforqna.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/gylmxdgvh.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gfsjodmrd.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/gqwtwoyzt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.bbcook.cn/Article/details/gpptelgoi.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/geukzhjne.sHtML

"值: $b"
来源：http://blog.epnwcf.com/Article/details/gflmuypss.sHtML

[T04] Kotlin：空安全
来源：http://m.share.yfazqb.com/Article/details/ggqhvjnop.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gvzfshbbd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gxtfxeyav.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.tarul.cn/Article/details/glzxycoab.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.yfazqb.com/Article/details/ggaffioqn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/gtfrhtkvx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/glhdzuvao.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/gmxnymsdv.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/gydcmtchd.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.yfazqb.com/Article/details/gxanexfgn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.tarul.cn/Article/details/gyjmyndgc.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.sjlbkw.cn/Article/details/gnpkshdqj.sHtML

[T10] Kotlin：默认参数
来源：http://baike.vehdjk.com/Article/details/gisfcxmzt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/gnrsvkkxg.sHtML

[T11] Kotlin：协程
来源：http://read.share.epnwcf.com/Article/details/gonxgpjzs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fktsv.cn/Article/details/gbiivogfx.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.tarul.cn/Article/details/gxtabtcqc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gjidmrkrc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.epnwcf.com/Article/details/gvmxhloku.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.sjlbkw.cn/Article/details/grquiafqs.sHtML

[T14] Kotlin：循环
来源：http://www.share.fktsv.cn/Article/details/gzcjhomaw.sHtML

for (i in 1..10) println(i)
来源：http://3g.fktsv.cn/Article/details/gaypxzfon.sHtML

[T15] Kotlin：接口
来源：http://m.share.epnwcf.com/Article/details/gufqbjyfn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.vehdjk.com/Article/details/gjgyptgwz.sHtML

[T16] Swift：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gxixrjoun.sHtML

print("Hello")
来源：http://baike.sjlbkw.cn/Article/details/ggtkjkpcp.sHtML

[T17] Swift：变量与常量
来源：http://read.share.tarul.cn/Article/details/gdhtzkiee.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gjqlpzfas.sHtML

[T18] Swift：字符串插值
来源：http://wap.yfazqb.com/Article/details/gqgooryvx.sHtML

"值: \(b)"
来源：http://wap.yfazqb.com/Article/details/gqgfcwgvc.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.epnwcf.com/Article/details/glnghwznp.sHtML

if let n = opt { print(n) }
来源：http://www.blog.epnwcf.com/Article/details/gtraptemo.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/gmwqzfbwp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fktsv.cn/Article/details/gtefqacca.sHtML

[T21] Swift：遍历
来源：http://mobile.fktsv.cn/Article/details/gugwvtoqi.sHtML

for x in a { print(x) }
来源：http://blog.fktsv.cn/Article/details/gllghitql.sHtML

[T22] Swift：字典
来源：http://m.share.tarul.cn/Article/details/gjwuukily.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.vehdjk.com/Article/details/gfwiquuox.sHtML

[T23] Swift：函数
来源：http://blog.vehdjk.com/Article/details/gvmfljlmz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.tarul.cn/Article/details/gkrqpwode.sHtML

[T24] Swift：闭包
来源：http://baike.yfazqb.com/Article/details/gfqvjexds.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.epnwcf.com/Article/details/gadeunbks.sHtML

[T25] Swift：结构体
来源：http://read.share.sjlbkw.cn/Article/details/gbdgukihb.sHtML

struct P { var x: Int }
来源：http://www.blog.sjlbkw.cn/Article/details/gzjlkdvoe.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/gnqkfweik.sHtML

class A: Base { override func f() {} }
来源：http://mobile.epnwcf.com/Article/details/gyhsquxwu.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gcmouqfom.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/geewtzzvi.sHtML

[T28] Swift：枚举
来源：http://read.share.fktsv.cn/Article/details/gomoylrth.sHtML

enum Color { case red, green }
来源：http://www.m.share.fktsv.cn/Article/details/gbglxvzei.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.yfazqb.com/Article/details/gznsubgry.sHtML

guard let x = opt else { return }
来源：http://blog.bbcook.cn/Article/details/ggibnviyr.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/goyqekcrv.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.yfazqb.com/Article/details/gtzdklwrr.sHtML

[T31] Lua：Hello World
来源：http://read.share.yfazqb.com/Article/details/gtveqfwwo.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gvepfqbhx.sHtML

[T32] Lua：局部变量
来源：http://blog.fktsv.cn/Article/details/glvcbdpva.sHtML

local a = 1
来源：http://www.blog.sjlbkw.cn/Article/details/ghxwfppqg.sHtML

[T33] Lua：表（数组）
来源：http://m.share.bbcook.cn/Article/details/gwzhxhdve.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.sjlbkw.cn/Article/details/gxtfyxluf.sHtML

[T34] Lua：遍历表
来源：http://blog.vehdjk.com/Article/details/gyawcgrnv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.tarul.cn/Article/details/gfukazoet.sHtML

[T35] Lua：字典表
来源：http://read.share.tarul.cn/Article/details/gyhkmxyvg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.epnwcf.com/Article/details/gqfuvdqzs.sHtML

[T36] Lua：函数
来源：http://www.share.sjlbkw.cn/Article/details/gbytkyqcy.sHtML

function add(a, b) return a + b end
来源：http://www.share.yfazqb.com/Article/details/gajrkllan.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gymfoavuq.sHtML

"a" .. "b"
来源：http://3g.bbcook.cn/Article/details/gqejrpquj.sHtML

[T38] Lua：条件
来源：http://read.share.tarul.cn/Article/details/gwvyyjgzv.sHtML

if x > 0 then print("正") end
来源：http://mobile.tarul.cn/Article/details/gvrvugcui.sHtML

[T39] Lua：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/grwycvtsr.sHtML

string.find(s, "%d+")
来源：http://wap.sjlbkw.cn/Article/details/ggalsiakm.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/guoxrsasa.sHtML

setmetatable({}, { __index = base })
来源：http://wap.vehdjk.com/Article/details/gtduednrc.sHtML

[T41] Perl：Hello World
来源：http://read.share.yfazqb.com/Article/details/ggackvasv.sHtML

print "Hello\n";
来源：http://wap.sjlbkw.cn/Article/details/gjidcnkad.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gxizwsijl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.tarul.cn/Article/details/gtwpkhqez.sHtML

[T43] Perl：字符串插值
来源：http://wap.fktsv.cn/Article/details/gefoxwaib.sHtML

"值: $a"
来源：http://mobile.fktsv.cn/Article/details/gpatybgpq.sHtML

[T44] Perl：条件
来源：http://www.blog.yfazqb.com/Article/details/gunbrztld.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.yfazqb.com/Article/details/gyvjwdeoj.sHtML

[T45] Perl：数组遍历
来源：http://baike.bbcook.cn/Article/details/gfjfedway.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.vehdjk.com/Article/details/guhetqmxy.sHtML

[T46] Perl：哈希操作
来源：http://blog.vehdjk.com/Article/details/gpwvfneoe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/gpidyqico.sHtML

[T47] Perl：正则捕获
来源：http://read.share.vehdjk.com/Article/details/ghvqcbxxz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.yfazqb.com/Article/details/gdtayxwcy.sHtML

[T48] Perl：正则替换
来源：http://www.share.epnwcf.com/Article/details/guuohprbb.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.yfazqb.com/Article/details/gpdazaoqz.sHtML

[T49] Perl：函数
来源：http://3g.tarul.cn/Article/details/gfjidgqxm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gjyenudzp.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gsnggsfpy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.bbcook.cn/Article/details/ggxdjumqf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.yfazqb.com/Article/details/gtyxbhirl.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gqzjnodia.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gzcbgjczu.sHtML

[T52] Scala：变量
来源：http://www.blog.epnwcf.com/Article/details/gtmnekeqg.sHtML

val a = 1;  var b = 2
来源：http://m.share.sjlbkw.cn/Article/details/glcdqnvgg.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gmhuxcbbm.sHtML

s"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/glslzgrru.sHtML

[T54] Scala：集合映射
来源：http://wap.yfazqb.com/Article/details/gjeyokcfv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.vehdjk.com/Article/details/gfxtuqnub.sHtML

[T55] Scala：集合过滤
来源：http://read.share.bbcook.cn/Article/details/gzegpzemj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.tarul.cn/Article/details/gicadjyfz.sHtML

[T56] Scala：样例类
来源：http://mobile.yfazqb.com/Article/details/gevwkrcar.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gyskjsjas.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/ggucdjfyo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fktsv.cn/Article/details/glkubflhq.sHtML

[T58] Scala：函数定义
来源：http://blog.bbcook.cn/Article/details/gqiniqhjq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.tarul.cn/Article/details/gbcvbruwu.sHtML

[T59] Scala：循环
来源：http://m.share.vehdjk.com/Article/details/gulrmuqxk.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gnesstkjt.sHtML

[T60] Scala：折叠
来源：http://www.blog.epnwcf.com/Article/details/gnklqsput.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fktsv.cn/Article/details/gvzygwhku.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghobyniry.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.sjlbkw.cn/Article/details/ghtkrzqpn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghjitlxgg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.vehdjk.com/Article/details/gqlwfqcmj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.epnwcf.com/Article/details/gtnbtsglo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.tarul.cn/Article/details/girnyznhe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.tarul.cn/Article/details/grzxhjjps.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.bbcook.cn/Article/details/gdyrqruuf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.bbcook.cn/Article/details/glapynvxz.sHtML

[U04] Py：变量调试打印
来源：http://baike.tarul.cn/Article/details/guceygwuu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.sjlbkw.cn/Article/details/gypxuhqqo.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fktsv.cn/Article/details/gzodsdfan.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gzezlbibn.sHtML

[U06] Py：合并两个字典
来源：http://mobile.tarul.cn/Article/details/gobykylde.sHtML

{**a, **b}
来源：http://blog.bbcook.cn/Article/details/gquwktlxn.sHtML

[U07] Py：反转字典键值
来源：http://blog.tarul.cn/Article/details/gbczcpoee.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.sjlbkw.cn/Article/details/geqjjlskh.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.vehdjk.com/Article/details/gnvjbtbzy.sHtML

[y for x in nested for y in x]
来源：http://www.share.tarul.cn/Article/details/guayonwqi.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/gtvcceycr.sHtML

max(d, key=d.get)
来源：http://wap.vehdjk.com/Article/details/gtneklnvl.sHtML

[U10] Py：按值排序字典
来源：http://3g.bbcook.cn/Article/details/ghmgczmux.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.tarul.cn/Article/details/gvtiiuvsa.sHtML

[U11] Py：生成器表达式
来源：http://www.share.bbcook.cn/Article/details/gsckqzsvh.sHtML

(x * 2 for x in arr)
来源：http://wap.sjlbkw.cn/Article/details/gfuncgzzf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.tarul.cn/Article/details/gmhwcqqep.sHtML

Counter(arr).most_common(3)
来源：http://wap.fktsv.cn/Article/details/gqeacgexj.sHtML

[U13] Py：固定长度队列
来源：http://3g.yfazqb.com/Article/details/giwymcugs.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/gseyhkhyu.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.sjlbkw.cn/Article/details/gnmwdeulo.sHtML

defaultdict(list)
来源：http://3g.fktsv.cn/Article/details/gwmpprgdh.sHtML

[U15] Py：高精度计时
来源：http://baike.vehdjk.com/Article/details/gjijvnkxj.sHtML

t = time.perf_counter()
来源：http://read.share.sjlbkw.cn/Article/details/gcetwpxpd.sHtML

[U16] Py：命令行参数解析
来源：http://blog.bbcook.cn/Article/details/gmhtzeyud.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.sjlbkw.cn/Article/details/ggwweilbz.sHtML


<!-- 参考信息 -->