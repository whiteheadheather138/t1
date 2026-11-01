代发 wailian999

split -l 1000 big.log part_
来源：http://www.share.tarul.cn/Article/details/gupqzvivd.sHtML

[R74] 批量重命名
来源：http://3g.fktsv.cn/Article/details/gqigttwwx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/grdalrhsv.sHtML

[R75] 导出环境变量
来源：http://m.share.sjlbkw.cn/Article/details/guolydxjw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.sjlbkw.cn/Article/details/gfiypznjj.sHtML

[R76] 使用临时文件
来源：http://mobile.yfazqb.com/Article/details/gwbxzngkl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/grcwpqwjj.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/gveatyxid.sHtML

read -rp "请输入: " ans
来源：http://www.share.sjlbkw.cn/Article/details/gsddtoimy.sHtML

[R78] 交互式菜单
来源：http://read.share.epnwcf.com/Article/details/gtbwrkyqs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.vehdjk.com/Article/details/gjzfjyolg.sHtML

[R79] 解析命令行选项
来源：http://m.share.sjlbkw.cn/Article/details/gkenxqbyx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.yfazqb.com/Article/details/gcfmgitzb.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.vehdjk.com/Article/details/gxlqzpumg.sHtML

time ./run.sh
来源：http://www.m.share.vehdjk.com/Article/details/grixrayxg.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkhdaezgu.sHtML

S. C / C++ 专题
来源：http://3g.epnwcf.com/Article/details/gjqylkhzi.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvuufxgcu.sHtML

[S01] C：Hello World
来源：http://www.share.yfazqb.com/Article/details/gaedndrwx.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/ggztsadmk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.vehdjk.com/Article/details/gybcngqfy.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.tarul.cn/Article/details/giysomtjk.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.vehdjk.com/Article/details/ghjdjkmqn.sHtML

[S03] C：读入整数
来源：http://mobile.tarul.cn/Article/details/gkaqhsbhv.sHtML

int x; scanf("%d", &x);
来源：http://www.share.bbcook.cn/Article/details/gigeagrjc.sHtML

[S04] C：字符串复制
来源：http://3g.fktsv.cn/Article/details/gkycdvexv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/gbqsxamzc.sHtML

[S05] C：字符串长度
来源：http://mobile.vehdjk.com/Article/details/gsdhvfxqh.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/geegibgns.sHtML

[S06] C：字符串比较
来源：http://wap.tarul.cn/Article/details/gcrzdfrck.sHtML

strcmp(a, b) == 0
来源：http://blog.epnwcf.com/Article/details/ggihnwfhe.sHtML

[S07] C：数组遍历求和
来源：http://www.share.vehdjk.com/Article/details/gwenibzih.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfxmwhym.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.yfazqb.com/Article/details/gfmwvuhna.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/gskrounsh.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.vehdjk.com/Article/details/gkhmafppg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fktsv.cn/Article/details/gvmtevgss.sHtML

[S10] C：指针与解引用
来源：http://www.share.bbcook.cn/Article/details/gpqayyaaq.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.yfazqb.com/Article/details/ghibjzygh.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gkirpfvqa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fktsv.cn/Article/details/gqthicspe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.yfazqb.com/Article/details/gugofooub.sHtML

fclose(f);
来源：http://3g.bbcook.cn/Article/details/gaqajsolp.sHtML

[S12] C：写文件
来源：http://m.share.epnwcf.com/Article/details/ghecqbjdu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gocusdepo.sHtML

[S13] C：宏定义
来源：http://www.m.share.vehdjk.com/Article/details/giipxbjgs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.tarul.cn/Article/details/gcvbpqpkt.sHtML

[S14] C：枚举
来源：http://www.blog.fktsv.cn/Article/details/gljmiquwy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.sjlbkw.cn/Article/details/gpauivbuc.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/gxcilzrml.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/gkrlwvwcp.sHtML

[S16] C：位操作置位
来源：http://m.share.epnwcf.com/Article/details/goahipdlx.sHtML

x |= (1 << 3);
来源：http://www.blog.fktsv.cn/Article/details/gboxqreut.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/grvvywnxt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.bbcook.cn/Article/details/gjruqxkfm.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gbrpwdaoi.sHtML

int main(int argc, char **argv)
来源：http://read.share.yfazqb.com/Article/details/gtoszcvdf.sHtML

[S19] C：快速排序
来源：http://www.share.vehdjk.com/Article/details/gslsqoqjf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/glrdmjwdi.sHtML

[S20] C：二分查找
来源：http://read.share.bbcook.cn/Article/details/gbjnksvrd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gkfgdqurf.sHtML

[S21] C：字符类别判断
来源：http://3g.vehdjk.com/Article/details/gdonhfzzt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/guzirregw.sHtML

[S22] C：字符串转数字
来源：http://baike.sjlbkw.cn/Article/details/gedzfstrl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.epnwcf.com/Article/details/gxmqjfnnn.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/gqrtwfkwe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.bbcook.cn/Article/details/goiljdsfz.sHtML

[S24] C：获取本地时间
来源：http://www.share.epnwcf.com/Article/details/gjsnzfaki.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.vehdjk.com/Article/details/ghnjetvcq.sHtML

[S25] C：内存拷贝
来源：http://www.blog.vehdjk.com/Article/details/gwwkyhphc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fktsv.cn/Article/details/gknsbpmsz.sHtML

[S26] C：内存清零
来源：http://www.m.share.vehdjk.com/Article/details/gbemandhm.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fktsv.cn/Article/details/glbkvivut.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/guodlburs.sHtML

const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gqyqxxrvo.sHtML

[S28] C：静态变量
来源：http://www.m.share.tarul.cn/Article/details/ggnqluoou.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/godryyeew.sHtML

[S29] C：变参函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gjazyoros.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.epnwcf.com/Article/details/gboqlcmpr.sHtML

[S30] C：头文件保护
来源：http://blog.vehdjk.com/Article/details/gdyzkxqlc.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gdgukwvuy.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/gvusykkpn.sHtML

#endif
来源：http://read.share.bbcook.cn/Article/details/gcqbftohc.sHtML

[S31] C++：Hello World
来源：http://read.share.bbcook.cn/Article/details/giavecgcl.sHtML

#include <iostream>
来源：http://blog.epnwcf.com/Article/details/gclkdsena.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/guqbgnwoz.sHtML

[S32] C++：字符串
来源：http://baike.yfazqb.com/Article/details/gkghyiext.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.tarul.cn/Article/details/gwkavenpg.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/ggchlhasl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.epnwcf.com/Article/details/gypdxzawg.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/gwxfpyaoy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fktsv.cn/Article/details/gecirkdck.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/guwmsyhlf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gucwrgvfz.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/gizadrgvc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gfahqyuep.sHtML

[S37] C++：set
来源：http://baike.yfazqb.com/Article/details/grnpcgtey.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.tarul.cn/Article/details/gbnxqpxna.sHtML

[S38] C++：排序
来源：http://www.blog.fktsv.cn/Article/details/gakteegnb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.bbcook.cn/Article/details/guaraxtgj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.tarul.cn/Article/details/gymezmnha.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.vehdjk.com/Article/details/gxufwecye.sHtML

[S40] C++：查找元素
来源：http://read.share.sjlbkw.cn/Article/details/ghizifyjq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fktsv.cn/Article/details/gflqrikbs.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/grhmtccev.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.epnwcf.com/Article/details/gvuzodsee.sHtML

[S42] C++：继承与虚函数
来源：http://blog.vehdjk.com/Article/details/geaxmvkxw.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.epnwcf.com/Article/details/glhozxtmj.sHtML

[S43] C++：智能指针
来源：http://blog.epnwcf.com/Article/details/guncpfkxv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gmvrahwuf.sHtML

[S44] C++：引用传参
来源：http://blog.fktsv.cn/Article/details/gnzrlutnj.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fktsv.cn/Article/details/gsmiauzsx.sHtML

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/gavwcwsop.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.bbcook.cn/Article/details/glyuftgwg.sHtML

[S46] C++：函数模板
来源：http://mobile.bbcook.cn/Article/details/gpolehlqw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.tarul.cn/Article/details/gdfhjlvue.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.tarul.cn/Article/details/grvpdzaqx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/gjsrbwxhd.sHtML

[S48] C++：逐行读文件
来源：http://blog.tarul.cn/Article/details/gtrlrzdtw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.sjlbkw.cn/Article/details/gmpenyhsv.sHtML

while (std::getline(in, line)) { }
来源：http://baike.yfazqb.com/Article/details/guicefvof.sHtML

[S49] C++：写文件
来源：http://www.blog.fktsv.cn/Article/details/gufvqrioc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/grkytnhar.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/ghfaaedeh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.tarul.cn/Article/details/glolfylmx.sHtML

[S51] C++：显式类型转换
来源：http://wap.yfazqb.com/Article/details/gzlcdpzbp.sHtML

static_cast<double>(a) / b
来源：http://blog.yfazqb.com/Article/details/gxsmntqzm.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.bbcook.cn/Article/details/goktfgjvv.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.yfazqb.com/Article/details/gbmcavrri.sHtML

[S53] C++：移动语义
来源：http://baike.yfazqb.com/Article/details/gprzdsljv.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.yfazqb.com/Article/details/gldgzdmbm.sHtML

[S54] C++：异常处理
来源：http://blog.bbcook.cn/Article/details/gzvsmtpxc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.vehdjk.com/Article/details/gkmancqjn.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gqtxyecog.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.bbcook.cn/Article/details/gzowrfvzp.sHtML

[S56] C++：optional
来源：http://wap.epnwcf.com/Article/details/glbiecher.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fktsv.cn/Article/details/girgybane.sHtML

[S57] C++：编译期常量
来源：http://wap.fktsv.cn/Article/details/gvdpwirzc.sHtML

constexpr int N = 10;
来源：http://www.m.share.bbcook.cn/Article/details/giucspuat.sHtML

[S58] C++：命名空间
来源：http://www.share.bbcook.cn/Article/details/goejlrufq.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.epnwcf.com/Article/details/gwmpiagnr.sHtML

[S59] C++：静态断言
来源：http://3g.vehdjk.com/Article/details/ggwafffbm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.bbcook.cn/Article/details/gwxiomopu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.epnwcf.com/Article/details/ghhbddfbv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gtqitdcvw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gqznevmtt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/girornvho.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ggdhwvzrt.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/gswzvmnni.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gmwhcyurq.sHtML

[T02] Kotlin：变量
来源：http://3g.bbcook.cn/Article/details/grkuwebne.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/gzngmousk.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gzawtpjkk.sHtML

"值: $b"
来源：http://www.share.tarul.cn/Article/details/gauhszbby.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/glcpabfbp.sHtML

val n: String? = null;  n?.length
来源：http://3g.sjlbkw.cn/Article/details/glydhizii.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/ghghkwlag.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.vehdjk.com/Article/details/gwhjgzjlb.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fktsv.cn/Article/details/gorpuduza.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.bbcook.cn/Article/details/grnsswgns.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.vehdjk.com/Article/details/gsaatdzbe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.tarul.cn/Article/details/gbntwrghy.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.yfazqb.com/Article/details/gcvljessx.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.tarul.cn/Article/details/glnvunfsn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.tarul.cn/Article/details/gakrvukej.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.bbcook.cn/Article/details/gmwuwixfd.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.yfazqb.com/Article/details/gqzbrrrio.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.yfazqb.com/Article/details/gmjpddnml.sHtML

[T11] Kotlin：协程
来源：http://www.blog.bbcook.cn/Article/details/gjkzlvuij.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.vehdjk.com/Article/details/grselshad.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.vehdjk.com/Article/details/gpxvgxuiw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gvuoiqoob.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.vehdjk.com/Article/details/gpamodixg.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.tarul.cn/Article/details/gjmcpmcav.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/gtdcpxhke.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gzlnndhyc.sHtML

[T15] Kotlin：接口
来源：http://www.share.vehdjk.com/Article/details/gnqreynys.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.epnwcf.com/Article/details/gijbwyhxk.sHtML

[T16] Swift：Hello World
来源：http://read.share.epnwcf.com/Article/details/gxvndcecw.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gvqyziqnv.sHtML

[T17] Swift：变量与常量
来源：http://baike.sjlbkw.cn/Article/details/gtumpcnbc.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/gtvyonfle.sHtML

[T18] Swift：字符串插值
来源：http://wap.vehdjk.com/Article/details/gsjlnstre.sHtML

"值: \(b)"
来源：http://read.share.bbcook.cn/Article/details/gxoxrkaqj.sHtML

[T19] Swift：可选绑定
来源：http://mobile.tarul.cn/Article/details/gjhqeyqpo.sHtML

if let n = opt { print(n) }
来源：http://m.share.fktsv.cn/Article/details/grnnnegtp.sHtML

[T20] Swift：数组操作
来源：http://www.blog.sjlbkw.cn/Article/details/gbfpcawzb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/gxwgjxjrz.sHtML

[T21] Swift：遍历
来源：http://blog.tarul.cn/Article/details/gbjxnwuib.sHtML

for x in a { print(x) }
来源：http://read.share.sjlbkw.cn/Article/details/ggdpzhiab.sHtML

[T22] Swift：字典
来源：http://www.share.epnwcf.com/Article/details/gbyuteggn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.epnwcf.com/Article/details/gsdkufffd.sHtML

[T23] Swift：函数
来源：http://wap.epnwcf.com/Article/details/gazxhwgvh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.tarul.cn/Article/details/gcgvwaaba.sHtML

[T24] Swift：闭包
来源：http://m.share.fktsv.cn/Article/details/gtssbcxig.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gkhrjgtzd.sHtML

[T25] Swift：结构体
来源：http://www.m.share.vehdjk.com/Article/details/gaevdjllc.sHtML

struct P { var x: Int }
来源：http://mobile.epnwcf.com/Article/details/gjeqdgdai.sHtML

[T26] Swift：类与重写
来源：http://3g.sjlbkw.cn/Article/details/gynrcfbfx.sHtML

class A: Base { override func f() {} }
来源：http://mobile.sjlbkw.cn/Article/details/gazpkjech.sHtML

[T27] Swift：错误处理
来源：http://m.share.sjlbkw.cn/Article/details/grpxpakbk.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.yfazqb.com/Article/details/gihyixzft.sHtML

[T28] Swift：枚举
来源：http://3g.sjlbkw.cn/Article/details/gkqnykgil.sHtML

enum Color { case red, green }
来源：http://blog.vehdjk.com/Article/details/gumrlxorb.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.yfazqb.com/Article/details/gzwdiggjq.sHtML

guard let x = opt else { return }
来源：http://read.share.vehdjk.com/Article/details/gkvmcaxjc.sHtML

[T30] Swift：协议
来源：http://baike.epnwcf.com/Article/details/gognzrpdv.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/gocnqqtpf.sHtML

[T31] Lua：Hello World
来源：http://3g.fktsv.cn/Article/details/grgnadlgl.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gjahqrsbl.sHtML

[T32] Lua：局部变量
来源：http://mobile.yfazqb.com/Article/details/glmxdquoo.sHtML

local a = 1
来源：http://www.share.yfazqb.com/Article/details/gfxiqmzqx.sHtML

[T33] Lua：表（数组）
来源：http://blog.bbcook.cn/Article/details/gvbhzqsfh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.sjlbkw.cn/Article/details/gaphlczbl.sHtML

[T34] Lua：遍历表
来源：http://www.share.tarul.cn/Article/details/geongldgw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.yfazqb.com/Article/details/gmlfjzcwd.sHtML

[T35] Lua：字典表
来源：http://baike.epnwcf.com/Article/details/gfmksfiga.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.tarul.cn/Article/details/grwhfbyie.sHtML

[T36] Lua：函数
来源：http://www.share.epnwcf.com/Article/details/gynednone.sHtML

function add(a, b) return a + b end
来源：http://mobile.sjlbkw.cn/Article/details/gatckfmec.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fktsv.cn/Article/details/gengfmlgr.sHtML

"a" .. "b"
来源：http://baike.yfazqb.com/Article/details/gyggwwhcw.sHtML

[T38] Lua：条件
来源：http://m.share.bbcook.cn/Article/details/gfizznmqr.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/grhmjfknq.sHtML

[T39] Lua：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gstsmyzar.sHtML

string.find(s, "%d+")
来源：http://www.m.share.yfazqb.com/Article/details/gbiumoreg.sHtML

[T40] Lua：元表
来源：http://blog.yfazqb.com/Article/details/ghpltwrsu.sHtML

setmetatable({}, { __index = base })
来源：http://blog.bbcook.cn/Article/details/gnoqjhran.sHtML

[T41] Perl：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gknrrxncf.sHtML

print "Hello\n";
来源：http://3g.sjlbkw.cn/Article/details/gsvgqikdh.sHtML

[T42] Perl：变量类型
来源：http://www.blog.epnwcf.com/Article/details/gybiffdtd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.sjlbkw.cn/Article/details/gjhoyhnie.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/glowrjeth.sHtML

"值: $a"
来源：http://blog.epnwcf.com/Article/details/gvahuuerg.sHtML

[T44] Perl：条件
来源：http://www.blog.bbcook.cn/Article/details/gulrhapid.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.bbcook.cn/Article/details/grohuqypx.sHtML

[T45] Perl：数组遍历
来源：http://wap.fktsv.cn/Article/details/gcxpvlmyc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.epnwcf.com/Article/details/gikkwixlp.sHtML

[T46] Perl：哈希操作
来源：http://3g.vehdjk.com/Article/details/govnoymoh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fktsv.cn/Article/details/gtivhlams.sHtML

[T47] Perl：正则捕获
来源：http://3g.tarul.cn/Article/details/glierdkip.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.tarul.cn/Article/details/ggkldswid.sHtML

[T48] Perl：正则替换
来源：http://baike.fktsv.cn/Article/details/glclsadmg.sHtML

$s =~ s/old/new/g;
来源：http://m.share.sjlbkw.cn/Article/details/gvjxzyzwf.sHtML

[T49] Perl：函数
来源：http://www.blog.epnwcf.com/Article/details/gmaxfdiwh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gwwfbgvrm.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gvbiaunat.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.bbcook.cn/Article/details/gyfrdnvsy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gspvtpnps.sHtML

[T51] Scala：Hello World
来源：http://3g.tarul.cn/Article/details/ggoeojczf.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/ghwzdqgnc.sHtML

[T52] Scala：变量
来源：http://read.share.sjlbkw.cn/Article/details/gobcwsjpn.sHtML

val a = 1;  var b = 2
来源：http://baike.bbcook.cn/Article/details/gpflfzjgm.sHtML

[T53] Scala：字符串插值
来源：http://baike.yfazqb.com/Article/details/gqffookes.sHtML

s"值: $b"
来源：http://read.share.tarul.cn/Article/details/gcserordw.sHtML

[T54] Scala：集合映射
来源：http://blog.fktsv.cn/Article/details/gzwspquut.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.bbcook.cn/Article/details/gekazhifn.sHtML

[T55] Scala：集合过滤
来源：http://3g.yfazqb.com/Article/details/gnmeskczr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.yfazqb.com/Article/details/gokyhchtp.sHtML

[T56] Scala：样例类
来源：http://read.share.epnwcf.com/Article/details/gntkkkrah.sHtML

case class User(name: String, age: Int)
来源：http://baike.vehdjk.com/Article/details/gpdvdlybo.sHtML

[T57] Scala：模式匹配
来源：http://baike.yfazqb.com/Article/details/gbhdjtjhb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.bbcook.cn/Article/details/gyzlvhecd.sHtML

[T58] Scala：函数定义
来源：http://wap.tarul.cn/Article/details/gdaymzkxw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.sjlbkw.cn/Article/details/geshupboc.sHtML

[T59] Scala：循环
来源：http://www.m.share.tarul.cn/Article/details/gsjwycvhb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.tarul.cn/Article/details/gqbxmolcm.sHtML

[T60] Scala：折叠
来源：http://baike.tarul.cn/Article/details/grkhexxlh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.sjlbkw.cn/Article/details/gwozfgjvt.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glfrbfppi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/gvrvggtra.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzxxsrktr.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.tarul.cn/Article/details/gfofuxsta.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.yfazqb.com/Article/details/gejtsagii.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.vehdjk.com/Article/details/gjdfrbhla.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fktsv.cn/Article/details/guiaxuyul.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fktsv.cn/Article/details/gegojgtcp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.tarul.cn/Article/details/gwcjcmqdr.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fktsv.cn/Article/details/gabkjuzfa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.yfazqb.com/Article/details/gvdcozpfs.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.vehdjk.com/Article/details/gnpbnvqbw.sHtML

list(dict.fromkeys(arr))
来源：http://baike.yfazqb.com/Article/details/giiuagulv.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fktsv.cn/Article/details/gzsweirho.sHtML

{**a, **b}
来源：http://mobile.tarul.cn/Article/details/ghubhdsas.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fktsv.cn/Article/details/gwlhzadjk.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.tarul.cn/Article/details/gofosdiok.sHtML

[U08] Py：展平二维列表
来源：http://read.share.sjlbkw.cn/Article/details/gvtgdrrpt.sHtML

[y for x in nested for y in x]
来源：http://mobile.vehdjk.com/Article/details/gewyluqxu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.yfazqb.com/Article/details/gjbbpulrk.sHtML

max(d, key=d.get)
来源：http://www.blog.fktsv.cn/Article/details/gmyxbwwpy.sHtML

[U10] Py：按值排序字典
来源：http://m.share.sjlbkw.cn/Article/details/gyyauuptv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.epnwcf.com/Article/details/gblzjsike.sHtML

[U11] Py：生成器表达式
来源：http://blog.yfazqb.com/Article/details/gymhsnncq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fktsv.cn/Article/details/gijknqglg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.vehdjk.com/Article/details/ghvcuanhp.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.bbcook.cn/Article/details/gnfcxlgub.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/goebbhgsc.sHtML

deque(maxlen=10)
来源：http://m.share.tarul.cn/Article/details/gmrevwoiq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.tarul.cn/Article/details/gpaycrmcj.sHtML

defaultdict(list)
来源：http://m.share.bbcook.cn/Article/details/ghnpsugpr.sHtML


<!-- 参考信息 -->