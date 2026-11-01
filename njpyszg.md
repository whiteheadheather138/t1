代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fktsv.cn/Article/details/gfmgowjsp.sHtML

[R76] 使用临时文件
来源：http://read.share.tarul.cn/Article/details/gyxlwjeba.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gdzjxkhuv.sHtML

[R77] 读取用户输入
来源：http://blog.sjlbkw.cn/Article/details/gvuaeuced.sHtML

read -rp "请输入: " ans
来源：http://wap.sjlbkw.cn/Article/details/ggfmkmxba.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/gwdxuhcdi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.epnwcf.com/Article/details/gdivubdhx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fktsv.cn/Article/details/gbsjwhxom.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.epnwcf.com/Article/details/gkmlvitpv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnylwkvz.sHtML

time ./run.sh
来源：http://www.blog.vehdjk.com/Article/details/gkxwwezcq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gpzeyoqps.sHtML

S. C / C++ 专题
来源：http://read.share.sjlbkw.cn/Article/details/gtainmnei.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ggurssauf.sHtML

[S01] C：Hello World
来源：http://3g.epnwcf.com/Article/details/gweqtdbhi.sHtML

#include <stdio.h>
来源：http://baike.fktsv.cn/Article/details/gnyqmdeev.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/glkdekfgk.sHtML

[S02] C：变量与格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gmyrxgiyl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.yfazqb.com/Article/details/gwuzpectz.sHtML

[S03] C：读入整数
来源：http://www.blog.epnwcf.com/Article/details/gwbjfuwrr.sHtML

int x; scanf("%d", &x);
来源：http://3g.tarul.cn/Article/details/guuososiz.sHtML

[S04] C：字符串复制
来源：http://wap.sjlbkw.cn/Article/details/gjyygbydb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/grreivwbz.sHtML

[S05] C：字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gtewlmmrs.sHtML

strlen(s)
来源：http://blog.tarul.cn/Article/details/gjhvrbrri.sHtML

[S06] C：字符串比较
来源：http://blog.bbcook.cn/Article/details/gzwoqqqor.sHtML

strcmp(a, b) == 0
来源：http://www.share.bbcook.cn/Article/details/gfbajpeuf.sHtML

[S07] C：数组遍历求和
来源：http://www.share.bbcook.cn/Article/details/guffxcevg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/gbasosdqm.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fktsv.cn/Article/details/gxzyykxop.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.vehdjk.com/Article/details/gmhrawpzf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/ggxguryod.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gwhxmbrbp.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.yfazqb.com/Article/details/ggojbhsxr.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.bbcook.cn/Article/details/ghjmqkjkg.sHtML

[S11] C：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gzhvsmerf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.yfazqb.com/Article/details/grrkdztri.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fktsv.cn/Article/details/gbmzkyine.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gkodzrkdl.sHtML

[S12] C：写文件
来源：http://3g.yfazqb.com/Article/details/givddckqx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/glanoguwf.sHtML

[S13] C：宏定义
来源：http://baike.vehdjk.com/Article/details/gbyyvbmwi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.yfazqb.com/Article/details/gkviaeqtn.sHtML

[S14] C：枚举
来源：http://www.share.sjlbkw.cn/Article/details/glbpjyppt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.yfazqb.com/Article/details/gewteqabu.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/gpbmczyfk.sHtML

(double) a / b
来源：http://mobile.epnwcf.com/Article/details/gdehixiho.sHtML

[S16] C：位操作置位
来源：http://baike.sjlbkw.cn/Article/details/gmllhrfpd.sHtML

x |= (1 << 3);
来源：http://www.m.share.yfazqb.com/Article/details/garsknsot.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gwvepfcix.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.sjlbkw.cn/Article/details/ghufqonfj.sHtML

[S18] C：命令行参数
来源：http://wap.epnwcf.com/Article/details/gyqcenbof.sHtML

int main(int argc, char **argv)
来源：http://blog.sjlbkw.cn/Article/details/gwhpiadyb.sHtML

[S19] C：快速排序
来源：http://www.m.share.vehdjk.com/Article/details/gboqcyqia.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gyqqmzyov.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gsnwderyc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gmttjltvl.sHtML

[S21] C：字符类别判断
来源：http://3g.fktsv.cn/Article/details/gehhtmvdb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.sjlbkw.cn/Article/details/gatmwtiwn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gkrkzsnlk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.tarul.cn/Article/details/gdffeysab.sHtML

[S23] C：随机数
来源：http://baike.yfazqb.com/Article/details/gscdkkbtp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.sjlbkw.cn/Article/details/glytotird.sHtML

[S24] C：获取本地时间
来源：http://wap.tarul.cn/Article/details/gyhlcidrk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/gjpkgamzw.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gpziplimg.sHtML

memcpy(dst, src, n);
来源：http://read.share.bbcook.cn/Article/details/gtcopnhke.sHtML

[S26] C：内存清零
来源：http://blog.fktsv.cn/Article/details/gvuwrcuns.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.sjlbkw.cn/Article/details/ggsczojqu.sHtML

[S27] C：定义常量
来源：http://www.share.tarul.cn/Article/details/glpnkxuex.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gmwplrwri.sHtML

[S28] C：静态变量
来源：http://baike.vehdjk.com/Article/details/gfgmkczdo.sHtML

static int counter = 0;
来源：http://3g.bbcook.cn/Article/details/ggwaevsrf.sHtML

[S29] C：变参函数
来源：http://baike.tarul.cn/Article/details/gnqgvcqku.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.yfazqb.com/Article/details/gipfxjlrq.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fktsv.cn/Article/details/gkfrtbvgk.sHtML

#ifndef X_H
来源：http://mobile.epnwcf.com/Article/details/goumpxmsq.sHtML

#define X_H
来源：http://baike.bbcook.cn/Article/details/gmsxmwutq.sHtML

#endif
来源：http://read.share.bbcook.cn/Article/details/gpsaixnem.sHtML

[S31] C++：Hello World
来源：http://mobile.bbcook.cn/Article/details/glrmkfkmd.sHtML

#include <iostream>
来源：http://read.share.tarul.cn/Article/details/giurghohg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.bbcook.cn/Article/details/gcnckisam.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gexfftwue.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.vehdjk.com/Article/details/gkszrlpgq.sHtML

[S33] C++：vector 增删
来源：http://m.share.vehdjk.com/Article/details/gixvqspyw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.yfazqb.com/Article/details/giegtbfzz.sHtML

[S34] C++：遍历 vector
来源：http://3g.sjlbkw.cn/Article/details/guoecukng.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/gmrrgnqto.sHtML

[S35] C++：map
来源：http://read.share.epnwcf.com/Article/details/gytcraeqw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/gynuhyyfw.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gpqfcflrz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gfjugppam.sHtML

[S37] C++：set
来源：http://3g.epnwcf.com/Article/details/gednjawyi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gqwhckmnu.sHtML

[S38] C++：排序
来源：http://3g.vehdjk.com/Article/details/gyevdkjxf.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.tarul.cn/Article/details/gewobbbqx.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/ggdpaiwgx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.sjlbkw.cn/Article/details/guxzhjzqi.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/gfhhihbkk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.yfazqb.com/Article/details/gmskrotgb.sHtML

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/gkdfstsll.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.yfazqb.com/Article/details/gciccatgs.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gzqfzqexi.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gmtvtudqx.sHtML

[S43] C++：智能指针
来源：http://mobile.yfazqb.com/Article/details/ggohxvyqj.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/gtouueygb.sHtML

[S44] C++：引用传参
来源：http://mobile.fktsv.cn/Article/details/gidhcpets.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.epnwcf.com/Article/details/gxyxmeoes.sHtML

[S45] C++：lambda
来源：http://mobile.vehdjk.com/Article/details/gjtvdseuc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.epnwcf.com/Article/details/gbiczausd.sHtML

[S46] C++：函数模板
来源：http://baike.tarul.cn/Article/details/gwapuzxip.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.vehdjk.com/Article/details/gmnzhhfob.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.vehdjk.com/Article/details/ggepkkytm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fktsv.cn/Article/details/gpecthsvm.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gtqrvxnsu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gtnlervqp.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.epnwcf.com/Article/details/glccawdle.sHtML

[S49] C++：写文件
来源：http://wap.sjlbkw.cn/Article/details/gtrshuuuw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.epnwcf.com/Article/details/glyizwucy.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.bbcook.cn/Article/details/gzomchchg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gphznmshh.sHtML

[S51] C++：显式类型转换
来源：http://wap.bbcook.cn/Article/details/ggeayuwxq.sHtML

static_cast<double>(a) / b
来源：http://blog.sjlbkw.cn/Article/details/giceyhvdq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.epnwcf.com/Article/details/gnantchxh.sHtML

int size() const noexcept { return n_; }
来源：http://wap.vehdjk.com/Article/details/gaocvybrm.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/gszvdcann.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.sjlbkw.cn/Article/details/gmdnyzqae.sHtML

[S54] C++：异常处理
来源：http://www.blog.yfazqb.com/Article/details/gxkdjhyml.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.epnwcf.com/Article/details/gjaxgwcra.sHtML

[S55] C++：结构化绑定
来源：http://baike.yfazqb.com/Article/details/gkwfvybli.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/gfjkmkubt.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/grixtxwus.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/gyjnzdxfd.sHtML

[S57] C++：编译期常量
来源：http://blog.sjlbkw.cn/Article/details/gvdjnhysi.sHtML

constexpr int N = 10;
来源：http://wap.bbcook.cn/Article/details/gkurmuhrh.sHtML

[S58] C++：命名空间
来源：http://blog.fktsv.cn/Article/details/grrcbpeyg.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.epnwcf.com/Article/details/gzkzdtapv.sHtML

[S59] C++：静态断言
来源：http://blog.yfazqb.com/Article/details/ggvnmowiq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.yfazqb.com/Article/details/gaydbazep.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.sjlbkw.cn/Article/details/ggfrmbasy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.tarul.cn/Article/details/gzwnnaenl.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmaphyxwv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.sjlbkw.cn/Article/details/gaxyyefyj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzvacyxtb.sHtML

[T01] Kotlin：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gzponksrd.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/ganpddbql.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.yfazqb.com/Article/details/gmeepazqq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.bbcook.cn/Article/details/gwxenptog.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/gwtsfebtc.sHtML

"值: $b"
来源：http://blog.fktsv.cn/Article/details/gloceqycb.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.bbcook.cn/Article/details/gzvwsxjpn.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/glqvvodnk.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.bbcook.cn/Article/details/gzhwdqnid.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.tarul.cn/Article/details/gavrdieis.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.bbcook.cn/Article/details/geiyrgunw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fktsv.cn/Article/details/gdoxugubf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/goxyjdsuu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.epnwcf.com/Article/details/godpkpknl.sHtML

[T08] Kotlin：数据类
来源：http://baike.yfazqb.com/Article/details/gqwpdyxqk.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gzcdqodis.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fktsv.cn/Article/details/gctzyigkr.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.epnwcf.com/Article/details/gisgxjojg.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fktsv.cn/Article/details/gavpssmub.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.sjlbkw.cn/Article/details/gsavelwxy.sHtML

[T11] Kotlin：协程
来源：http://www.share.epnwcf.com/Article/details/gcvldaidl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.yfazqb.com/Article/details/gcvguixee.sHtML

[T12] Kotlin：解构声明
来源：http://3g.sjlbkw.cn/Article/details/gpbmasozr.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gfyzbmiid.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/gwlaxunwt.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.vehdjk.com/Article/details/gtenkdotr.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/gzrgeuvhs.sHtML

for (i in 1..10) println(i)
来源：http://read.share.epnwcf.com/Article/details/gtvpeityk.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.vehdjk.com/Article/details/ghmvcitda.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fktsv.cn/Article/details/gxwvhjexs.sHtML

[T16] Swift：Hello World
来源：http://wap.vehdjk.com/Article/details/gunjaizux.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gxptfjeqz.sHtML

[T17] Swift：变量与常量
来源：http://wap.tarul.cn/Article/details/glpdbxiut.sHtML

var a = 1;  let b = 2
来源：http://baike.epnwcf.com/Article/details/ghtfyjryp.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpczihrt.sHtML

"值: \(b)"
来源：http://www.blog.vehdjk.com/Article/details/gjmumaiuq.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.vehdjk.com/Article/details/gjcvlgehs.sHtML

if let n = opt { print(n) }
来源：http://baike.vehdjk.com/Article/details/gjtsoidlk.sHtML

[T20] Swift：数组操作
来源：http://www.blog.epnwcf.com/Article/details/gnufsgutl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.yfazqb.com/Article/details/glonghjos.sHtML

[T21] Swift：遍历
来源：http://3g.fktsv.cn/Article/details/gkjbkcfpf.sHtML

for x in a { print(x) }
来源：http://mobile.vehdjk.com/Article/details/gkensncym.sHtML

[T22] Swift：字典
来源：http://www.m.share.tarul.cn/Article/details/glugdpfxo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/gkzqzjtvq.sHtML

[T23] Swift：函数
来源：http://www.share.fktsv.cn/Article/details/gpuexjbqs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.epnwcf.com/Article/details/glsbtohvb.sHtML

[T24] Swift：闭包
来源：http://m.share.yfazqb.com/Article/details/gnpwmltya.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fktsv.cn/Article/details/gzpvfhtsk.sHtML

[T25] Swift：结构体
来源：http://www.share.sjlbkw.cn/Article/details/gbbagevng.sHtML

struct P { var x: Int }
来源：http://www.blog.epnwcf.com/Article/details/gicdwcyiq.sHtML

[T26] Swift：类与重写
来源：http://baike.tarul.cn/Article/details/gojszvagx.sHtML

class A: Base { override func f() {} }
来源：http://www.share.epnwcf.com/Article/details/gahbltyfq.sHtML

[T27] Swift：错误处理
来源：http://mobile.sjlbkw.cn/Article/details/gjsngxchb.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.epnwcf.com/Article/details/gprhbehsp.sHtML

[T28] Swift：枚举
来源：http://read.share.epnwcf.com/Article/details/gahifzynt.sHtML

enum Color { case red, green }
来源：http://wap.sjlbkw.cn/Article/details/ghhbgtrkt.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fktsv.cn/Article/details/gvahzhgtm.sHtML

guard let x = opt else { return }
来源：http://blog.epnwcf.com/Article/details/gzjqsfbun.sHtML

[T30] Swift：协议
来源：http://www.m.share.sjlbkw.cn/Article/details/glcbliwhv.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.tarul.cn/Article/details/gfogzsxfs.sHtML

[T31] Lua：Hello World
来源：http://m.share.tarul.cn/Article/details/ggtgheyzj.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gjxakipvb.sHtML

[T32] Lua：局部变量
来源：http://3g.epnwcf.com/Article/details/gpcrtkczq.sHtML

local a = 1
来源：http://www.share.fktsv.cn/Article/details/gvapjgewm.sHtML

[T33] Lua：表（数组）
来源：http://www.share.epnwcf.com/Article/details/gvmetxsmt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.vehdjk.com/Article/details/gulxrhrpi.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.sjlbkw.cn/Article/details/gvofztaon.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.sjlbkw.cn/Article/details/grjlosqdm.sHtML

[T35] Lua：字典表
来源：http://m.share.bbcook.cn/Article/details/gjbidojfi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.epnwcf.com/Article/details/gifnfnvtr.sHtML

[T36] Lua：函数
来源：http://baike.fktsv.cn/Article/details/gafpxwkrj.sHtML

function add(a, b) return a + b end
来源：http://blog.epnwcf.com/Article/details/gpiwjmkfp.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.tarul.cn/Article/details/grjcnyvwa.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/gpydbpjyq.sHtML

[T38] Lua：条件
来源：http://mobile.vehdjk.com/Article/details/gcgzaxzag.sHtML

if x > 0 then print("正") end
来源：http://3g.tarul.cn/Article/details/gcoepfixb.sHtML

[T39] Lua：模式匹配
来源：http://blog.fktsv.cn/Article/details/gxqcfccem.sHtML

string.find(s, "%d+")
来源：http://wap.sjlbkw.cn/Article/details/gihsosdtn.sHtML

[T40] Lua：元表
来源：http://m.share.fktsv.cn/Article/details/gqkmeojgs.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.vehdjk.com/Article/details/gdishoggk.sHtML

[T41] Perl：Hello World
来源：http://wap.tarul.cn/Article/details/gqfnydxax.sHtML

print "Hello\n";
来源：http://3g.sjlbkw.cn/Article/details/gffhcsncb.sHtML

[T42] Perl：变量类型
来源：http://blog.fktsv.cn/Article/details/gnqhmjfpk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.sjlbkw.cn/Article/details/gajshpxeq.sHtML

[T43] Perl：字符串插值
来源：http://blog.tarul.cn/Article/details/gnqiegzys.sHtML

"值: $a"
来源：http://3g.yfazqb.com/Article/details/govpeyoos.sHtML

[T44] Perl：条件
来源：http://3g.fktsv.cn/Article/details/gtzjsqreo.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.yfazqb.com/Article/details/ggkxxyhdp.sHtML

[T45] Perl：数组遍历
来源：http://3g.tarul.cn/Article/details/gthbfaesj.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.bbcook.cn/Article/details/gzcvnkmuw.sHtML

[T46] Perl：哈希操作
来源：http://3g.epnwcf.com/Article/details/gspevznrs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.tarul.cn/Article/details/gmahyllqs.sHtML

[T47] Perl：正则捕获
来源：http://www.share.sjlbkw.cn/Article/details/gzihysvwb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.sjlbkw.cn/Article/details/gnonycbov.sHtML

[T48] Perl：正则替换
来源：http://wap.yfazqb.com/Article/details/gmimvstqn.sHtML

$s =~ s/old/new/g;
来源：http://m.share.vehdjk.com/Article/details/gouufzswr.sHtML

[T49] Perl：函数
来源：http://baike.sjlbkw.cn/Article/details/gycpdgilc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gyiqdjqam.sHtML

[T50] Perl：逐行读文件
来源：http://baike.tarul.cn/Article/details/gzhxjiaqp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.yfazqb.com/Article/details/gieanklnz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.epnwcf.com/Article/details/grgtbtcro.sHtML

[T51] Scala：Hello World
来源：http://www.share.epnwcf.com/Article/details/gaaxdhggl.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gexbqrnbb.sHtML

[T52] Scala：变量
来源：http://wap.vehdjk.com/Article/details/gpvldggnx.sHtML

val a = 1;  var b = 2
来源：http://www.blog.vehdjk.com/Article/details/gohbyyjoo.sHtML

[T53] Scala：字符串插值
来源：http://wap.tarul.cn/Article/details/gcnykigqc.sHtML

s"值: $b"
来源：http://mobile.yfazqb.com/Article/details/gyzkvihwx.sHtML

[T54] Scala：集合映射
来源：http://baike.fktsv.cn/Article/details/gokqjdrnv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.vehdjk.com/Article/details/gzyofnknj.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gxzcmcmny.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.sjlbkw.cn/Article/details/gbhddenpx.sHtML

[T56] Scala：样例类
来源：http://mobile.epnwcf.com/Article/details/gnfowznty.sHtML

case class User(name: String, age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/guvnfqugd.sHtML

[T57] Scala：模式匹配
来源：http://read.share.epnwcf.com/Article/details/ggnqibqpc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.tarul.cn/Article/details/glybnfuby.sHtML

[T58] Scala：函数定义
来源：http://read.share.bbcook.cn/Article/details/gdcazypud.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.vehdjk.com/Article/details/gwmevhrzk.sHtML

[T59] Scala：循环
来源：http://read.share.fktsv.cn/Article/details/gvsbhondd.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gdnvyswvq.sHtML

[T60] Scala：折叠
来源：http://wap.sjlbkw.cn/Article/details/giurbzbnw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.tarul.cn/Article/details/gioyfrlfs.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxgdnrjbg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gpesijujf.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gohlbrnzp.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.bbcook.cn/Article/details/gmlgmgtvj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.bbcook.cn/Article/details/grntzjpad.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/gqofrgsxb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.sjlbkw.cn/Article/details/gvfmvnhlv.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.bbcook.cn/Article/details/gsybcqbkm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.vehdjk.com/Article/details/gkyjenfqn.sHtML

[U04] Py：变量调试打印
来源：http://m.share.tarul.cn/Article/details/gfddmovxl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.yfazqb.com/Article/details/gvlbmrqrm.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.bbcook.cn/Article/details/gubomuhzv.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/ggbtauwpm.sHtML

[U06] Py：合并两个字典
来源：http://blog.epnwcf.com/Article/details/glvhovaio.sHtML

{**a, **b}
来源：http://3g.sjlbkw.cn/Article/details/guayyhtln.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.yfazqb.com/Article/details/gyfxfofqb.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.yfazqb.com/Article/details/gocclfaxx.sHtML

[U08] Py：展平二维列表
来源：http://mobile.tarul.cn/Article/details/ghzumlgvz.sHtML

[y for x in nested for y in x]
来源：http://www.share.tarul.cn/Article/details/gxugeraqk.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.tarul.cn/Article/details/grbwdbaot.sHtML

max(d, key=d.get)
来源：http://read.share.yfazqb.com/Article/details/gmwjctvtf.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.yfazqb.com/Article/details/gquvwbzac.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.vehdjk.com/Article/details/gjwkmvenl.sHtML

[U11] Py：生成器表达式
来源：http://m.share.bbcook.cn/Article/details/gftjuswfy.sHtML

(x * 2 for x in arr)
来源：http://wap.tarul.cn/Article/details/gdbifneku.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.epnwcf.com/Article/details/glrkozvrt.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/gotwnmtqm.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.sjlbkw.cn/Article/details/gpwkqxouo.sHtML

deque(maxlen=10)
来源：http://read.share.vehdjk.com/Article/details/gfiqpewqf.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fktsv.cn/Article/details/gubfwwsrq.sHtML

defaultdict(list)
来源：http://3g.fktsv.cn/Article/details/gujumopnb.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.yfazqb.com/Article/details/gwssslwzm.sHtML

t = time.perf_counter()
来源：http://www.blog.tarul.cn/Article/details/gdsbvwfpo.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.yfazqb.com/Article/details/ghpzwgtcd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.tarul.cn/Article/details/gzhkcteft.sHtML


<!-- 参考信息 -->