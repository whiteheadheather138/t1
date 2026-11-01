代发 wailian999

S. C / C++ 专题
来源：http://wap.bbcook.cn/Article/details/gptjfytxg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grktrgxpu.sHtML

[S01] C：Hello World
来源：http://www.share.fktsv.cn/Article/details/gtxceyyxf.sHtML

#include <stdio.h>
来源：http://read.share.vehdjk.com/Article/details/gbafdwyxz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.yfazqb.com/Article/details/guadlxwyv.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.tarul.cn/Article/details/grmvpykjb.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.vehdjk.com/Article/details/gqytzdxft.sHtML

[S03] C：读入整数
来源：http://read.share.yfazqb.com/Article/details/giuxfgyei.sHtML

int x; scanf("%d", &x);
来源：http://baike.bbcook.cn/Article/details/gpkxcuoeb.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/gkincfufx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gfymfcafk.sHtML

[S05] C：字符串长度
来源：http://wap.vehdjk.com/Article/details/gzhwntqyb.sHtML

strlen(s)
来源：http://www.blog.bbcook.cn/Article/details/gvgcabatr.sHtML

[S06] C：字符串比较
来源：http://read.share.fktsv.cn/Article/details/gjnzfxhfe.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fktsv.cn/Article/details/gfrxefyje.sHtML

[S07] C：数组遍历求和
来源：http://baike.tarul.cn/Article/details/gmwkrdhdy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.epnwcf.com/Article/details/grmzlqaqx.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.yfazqb.com/Article/details/gynlqpvnd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/glgeytzcp.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.vehdjk.com/Article/details/ghlbdqqtr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fktsv.cn/Article/details/grzxfktfy.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/gcrbayaxc.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fktsv.cn/Article/details/giozwyvtj.sHtML

[S11] C：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/ghqacqvfj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.bbcook.cn/Article/details/gdnbypfsu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.sjlbkw.cn/Article/details/gqtnrzxhb.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gtxlfwyky.sHtML

[S12] C：写文件
来源：http://www.share.fktsv.cn/Article/details/gaxlxcbmq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gljyltqpf.sHtML

[S13] C：宏定义
来源：http://blog.bbcook.cn/Article/details/gelkqntdi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.tarul.cn/Article/details/gwkkxvciz.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/gzaezdvul.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.sjlbkw.cn/Article/details/gfmeuftlw.sHtML

[S15] C：类型转换
来源：http://read.share.yfazqb.com/Article/details/glnkdhiky.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnmfnlfp.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/gojhjzbvx.sHtML

x |= (1 << 3);
来源：http://baike.fktsv.cn/Article/details/gdzcijace.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.vehdjk.com/Article/details/groambnkz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fktsv.cn/Article/details/gahrsvtir.sHtML

[S18] C：命令行参数
来源：http://baike.bbcook.cn/Article/details/gousnifpx.sHtML

int main(int argc, char **argv)
来源：http://m.share.sjlbkw.cn/Article/details/gjymqoxuv.sHtML

[S19] C：快速排序
来源：http://www.m.share.epnwcf.com/Article/details/gxhmfxyfs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gjjdzvxfn.sHtML

[S20] C：二分查找
来源：http://mobile.tarul.cn/Article/details/gjexoyipe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/ghpkwmdqy.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.epnwcf.com/Article/details/gckaftuhc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.vehdjk.com/Article/details/gfdmkvuis.sHtML

[S22] C：字符串转数字
来源：http://blog.epnwcf.com/Article/details/gxqebmlsj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.bbcook.cn/Article/details/gffnzzhii.sHtML

[S23] C：随机数
来源：http://m.share.fktsv.cn/Article/details/gychkzgni.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.epnwcf.com/Article/details/glfccvwsv.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gynogjtfz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/gojsugwie.sHtML

[S25] C：内存拷贝
来源：http://baike.epnwcf.com/Article/details/gfypqilke.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gxlaafihg.sHtML

[S26] C：内存清零
来源：http://baike.fktsv.cn/Article/details/gcqhckkeq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.bbcook.cn/Article/details/gpnrwjfgg.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gmawxbnsp.sHtML

const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/grbtouprc.sHtML

[S28] C：静态变量
来源：http://www.m.share.bbcook.cn/Article/details/gpzrmgpxm.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gvelqipjz.sHtML

[S29] C：变参函数
来源：http://blog.sjlbkw.cn/Article/details/gvbuissmr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.vehdjk.com/Article/details/godyypowj.sHtML

[S30] C：头文件保护
来源：http://blog.epnwcf.com/Article/details/gefgozchg.sHtML

#ifndef X_H
来源：http://www.share.fktsv.cn/Article/details/guzzssixv.sHtML

#define X_H
来源：http://mobile.epnwcf.com/Article/details/gjyqtxznk.sHtML

#endif
来源：http://read.share.fktsv.cn/Article/details/gbpoxpuwf.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/glpfopgtm.sHtML

#include <iostream>
来源：http://www.m.share.tarul.cn/Article/details/ggmwbxqjm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.sjlbkw.cn/Article/details/gjtwdvaes.sHtML

[S32] C++：字符串
来源：http://www.blog.fktsv.cn/Article/details/ghpbamehn.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.yfazqb.com/Article/details/gcuallgcv.sHtML

[S33] C++：vector 增删
来源：http://baike.epnwcf.com/Article/details/gqvstpbrs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.bbcook.cn/Article/details/gtsepmlek.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.tarul.cn/Article/details/gqgbrdnik.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fktsv.cn/Article/details/gtcsjtqyr.sHtML

[S35] C++：map
来源：http://baike.vehdjk.com/Article/details/goakfwqas.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrckppvt.sHtML

[S36] C++：unordered_map
来源：http://mobile.bbcook.cn/Article/details/gmztfezjc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gbwyiutpm.sHtML

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/gmuqawxjo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.epnwcf.com/Article/details/gjxnwmrtc.sHtML

[S38] C++：排序
来源：http://read.share.tarul.cn/Article/details/gitbwatyb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gbjrwuriv.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.yfazqb.com/Article/details/gxjrxakmk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.epnwcf.com/Article/details/gadyluwmw.sHtML

[S40] C++：查找元素
来源：http://3g.fktsv.cn/Article/details/ggoztntrf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.sjlbkw.cn/Article/details/gzclltkhm.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/gdinrrdyn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.tarul.cn/Article/details/gvracnkqv.sHtML

[S42] C++：继承与虚函数
来源：http://wap.bbcook.cn/Article/details/geunrbrct.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.yfazqb.com/Article/details/goxneksxw.sHtML

[S43] C++：智能指针
来源：http://3g.bbcook.cn/Article/details/gkswcertj.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.bbcook.cn/Article/details/gvqaietbq.sHtML

[S44] C++：引用传参
来源：http://www.m.share.bbcook.cn/Article/details/gywpqpvgc.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.tarul.cn/Article/details/glbkuchvc.sHtML

[S45] C++：lambda
来源：http://read.share.bbcook.cn/Article/details/glrewplgn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.bbcook.cn/Article/details/gfyejvzvb.sHtML

[S46] C++：函数模板
来源：http://m.share.fktsv.cn/Article/details/gvgzfwyap.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.bbcook.cn/Article/details/gbqtmhlkj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fktsv.cn/Article/details/gfjtazrhh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/gvyczekhu.sHtML

[S48] C++：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gltmrsagr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.epnwcf.com/Article/details/grqjnaqxt.sHtML

while (std::getline(in, line)) { }
来源：http://wap.vehdjk.com/Article/details/gxjerfqys.sHtML

[S49] C++：写文件
来源：http://baike.tarul.cn/Article/details/gprcigfgx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fktsv.cn/Article/details/gqaznueuj.sHtML

[S50] C++：格式化数字
来源：http://baike.tarul.cn/Article/details/goccubxcu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fktsv.cn/Article/details/gjbzetreg.sHtML

[S51] C++：显式类型转换
来源：http://wap.vehdjk.com/Article/details/gorgdyvvy.sHtML

static_cast<double>(a) / b
来源：http://blog.yfazqb.com/Article/details/gnkpjwmqv.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.vehdjk.com/Article/details/ghawdskgf.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.tarul.cn/Article/details/guaybwtda.sHtML

[S53] C++：移动语义
来源：http://wap.yfazqb.com/Article/details/gmbnassvp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fktsv.cn/Article/details/gkdjteiep.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/gydmezjum.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.tarul.cn/Article/details/gnwswiszi.sHtML

[S55] C++：结构化绑定
来源：http://m.share.vehdjk.com/Article/details/goctlqskq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/gtsdbrvmf.sHtML

[S56] C++：optional
来源：http://www.m.share.vehdjk.com/Article/details/goxzrelsj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/gcgfoxgqn.sHtML

[S57] C++：编译期常量
来源：http://3g.sjlbkw.cn/Article/details/gxijznbmt.sHtML

constexpr int N = 10;
来源：http://blog.fktsv.cn/Article/details/guaafxcty.sHtML

[S58] C++：命名空间
来源：http://baike.epnwcf.com/Article/details/gmkuygjuu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gsreearlt.sHtML

[S59] C++：静态断言
来源：http://www.share.fktsv.cn/Article/details/glonvwpwo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/gxegcqhqe.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.sjlbkw.cn/Article/details/gafmmuwxc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fktsv.cn/Article/details/gjztyswgw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbwkjgcne.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.epnwcf.com/Article/details/grsppyyyw.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gyfshuerf.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fktsv.cn/Article/details/gttiesjla.sHtML

println("Hello")
来源：http://wap.vehdjk.com/Article/details/gxshrftdy.sHtML

[T02] Kotlin：变量
来源：http://wap.epnwcf.com/Article/details/gahosyjvb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.tarul.cn/Article/details/gfasdwvaf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.bbcook.cn/Article/details/gqixgsmau.sHtML

"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gijuxrzar.sHtML

[T04] Kotlin：空安全
来源：http://read.share.tarul.cn/Article/details/gxihbrvjs.sHtML

val n: String? = null;  n?.length
来源：http://blog.tarul.cn/Article/details/ghuejipza.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gadvwozpu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/gtwpuxrot.sHtML

[T06] Kotlin：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gkqixjktt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.epnwcf.com/Article/details/gexnqgiby.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.yfazqb.com/Article/details/gqggdtcft.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.vehdjk.com/Article/details/ggdzunhfa.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.bbcook.cn/Article/details/ghbxzemnp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gxsiazdgi.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.epnwcf.com/Article/details/guxpgdkpp.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.yfazqb.com/Article/details/gvmqzczgc.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gpdzumpas.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.epnwcf.com/Article/details/gbwreohas.sHtML

[T11] Kotlin：协程
来源：http://mobile.vehdjk.com/Article/details/gsbumaavh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.sjlbkw.cn/Article/details/gixpeespq.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.yfazqb.com/Article/details/gskusywck.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gxxhkmoun.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.tarul.cn/Article/details/gjxioqrtk.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.vehdjk.com/Article/details/gknnhsmxu.sHtML

[T14] Kotlin：循环
来源：http://m.share.sjlbkw.cn/Article/details/ggwkjlmqb.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.vehdjk.com/Article/details/gmhklryyv.sHtML

[T15] Kotlin：接口
来源：http://m.share.fktsv.cn/Article/details/gzttarjwo.sHtML

interface Shape { fun area(): Double }
来源：http://baike.vehdjk.com/Article/details/gmjijgjva.sHtML

[T16] Swift：Hello World
来源：http://blog.fktsv.cn/Article/details/gogsesfdt.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gikxtjmrz.sHtML

[T17] Swift：变量与常量
来源：http://3g.tarul.cn/Article/details/gbtehqvkf.sHtML

var a = 1;  let b = 2
来源：http://www.share.fktsv.cn/Article/details/ghvozatkl.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gcjosrxqe.sHtML

"值: \(b)"
来源：http://mobile.vehdjk.com/Article/details/gcbbuikib.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/gyleycwhs.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.bbcook.cn/Article/details/geccbdpfb.sHtML

[T20] Swift：数组操作
来源：http://www.blog.yfazqb.com/Article/details/gydwnrebr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.tarul.cn/Article/details/gtiifqkle.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/gjvnaoter.sHtML

for x in a { print(x) }
来源：http://baike.vehdjk.com/Article/details/gtnjhcvex.sHtML

[T22] Swift：字典
来源：http://baike.yfazqb.com/Article/details/gysqrjhxh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fktsv.cn/Article/details/gdxxmuxvo.sHtML

[T23] Swift：函数
来源：http://baike.sjlbkw.cn/Article/details/gakdqntrb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/glgxnmcwl.sHtML

[T24] Swift：闭包
来源：http://baike.epnwcf.com/Article/details/gfdrwkfpu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.tarul.cn/Article/details/gzoagfqae.sHtML

[T25] Swift：结构体
来源：http://www.blog.yfazqb.com/Article/details/gbjujljya.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/gscabgskh.sHtML

[T26] Swift：类与重写
来源：http://mobile.sjlbkw.cn/Article/details/gycypcjjb.sHtML

class A: Base { override func f() {} }
来源：http://www.share.sjlbkw.cn/Article/details/ghrddlewv.sHtML

[T27] Swift：错误处理
来源：http://mobile.tarul.cn/Article/details/gmbdiqtbd.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/gtzchjorw.sHtML

[T28] Swift：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gxceybygo.sHtML

enum Color { case red, green }
来源：http://www.share.bbcook.cn/Article/details/ghyxnehsc.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.sjlbkw.cn/Article/details/gdftvpsvf.sHtML

guard let x = opt else { return }
来源：http://www.blog.yfazqb.com/Article/details/gqdgwlyou.sHtML

[T30] Swift：协议
来源：http://www.share.tarul.cn/Article/details/gpjdktios.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fktsv.cn/Article/details/gqhkykbmj.sHtML

[T31] Lua：Hello World
来源：http://3g.yfazqb.com/Article/details/gsrqtpvpq.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/geozfvdrb.sHtML

[T32] Lua：局部变量
来源：http://3g.epnwcf.com/Article/details/glpxycipd.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/gcizlqdgu.sHtML

[T33] Lua：表（数组）
来源：http://3g.vehdjk.com/Article/details/guymcgydv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.bbcook.cn/Article/details/ghmqiriqb.sHtML

[T34] Lua：遍历表
来源：http://3g.sjlbkw.cn/Article/details/gjgkehjlp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.tarul.cn/Article/details/gkrlsaipi.sHtML

[T35] Lua：字典表
来源：http://read.share.fktsv.cn/Article/details/gpgjevtfq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fktsv.cn/Article/details/garzpmqtl.sHtML

[T36] Lua：函数
来源：http://blog.fktsv.cn/Article/details/gttlscpqq.sHtML

function add(a, b) return a + b end
来源：http://3g.fktsv.cn/Article/details/gnlrnvclo.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.tarul.cn/Article/details/guadgmhel.sHtML

"a" .. "b"
来源：http://3g.bbcook.cn/Article/details/gxbwffsce.sHtML

[T38] Lua：条件
来源：http://3g.yfazqb.com/Article/details/gtqhfdlte.sHtML

if x > 0 then print("正") end
来源：http://blog.vehdjk.com/Article/details/ghhnzsbez.sHtML

[T39] Lua：模式匹配
来源：http://m.share.tarul.cn/Article/details/geprjaurx.sHtML

string.find(s, "%d+")
来源：http://wap.sjlbkw.cn/Article/details/gokovfdcl.sHtML

[T40] Lua：元表
来源：http://read.share.yfazqb.com/Article/details/gslhsbuhh.sHtML

setmetatable({}, { __index = base })
来源：http://baike.sjlbkw.cn/Article/details/gxnnfofvw.sHtML

[T41] Perl：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gszznclla.sHtML

print "Hello\n";
来源：http://www.blog.epnwcf.com/Article/details/gtmcaukeu.sHtML

[T42] Perl：变量类型
来源：http://mobile.epnwcf.com/Article/details/gcceabwat.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.bbcook.cn/Article/details/gyycrtzci.sHtML

[T43] Perl：字符串插值
来源：http://baike.fktsv.cn/Article/details/gowtuspnd.sHtML

"值: $a"
来源：http://read.share.tarul.cn/Article/details/gorbzoeek.sHtML

[T44] Perl：条件
来源：http://baike.yfazqb.com/Article/details/gveoiuzgp.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fktsv.cn/Article/details/gzovnsqah.sHtML

[T45] Perl：数组遍历
来源：http://wap.bbcook.cn/Article/details/godscuuou.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.sjlbkw.cn/Article/details/ggtufnqka.sHtML

[T46] Perl：哈希操作
来源：http://baike.vehdjk.com/Article/details/gfxjzkxoc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.epnwcf.com/Article/details/gqcffcitk.sHtML

[T47] Perl：正则捕获
来源：http://3g.epnwcf.com/Article/details/gvkmdvggu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.vehdjk.com/Article/details/grswsdnao.sHtML

[T48] Perl：正则替换
来源：http://blog.yfazqb.com/Article/details/gmlgqswbx.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.bbcook.cn/Article/details/gwqkamnkm.sHtML

[T49] Perl：函数
来源：http://www.share.vehdjk.com/Article/details/gdhjqzprh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/giazmfxlk.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gmgtvhyox.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.tarul.cn/Article/details/ghfbfzfmt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.tarul.cn/Article/details/gwvlecfeg.sHtML

[T51] Scala：Hello World
来源：http://baike.yfazqb.com/Article/details/gwesnibyt.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gdjtavqcy.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gpmrgppip.sHtML

val a = 1;  var b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gubqrhvwv.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fktsv.cn/Article/details/goznmvrqv.sHtML

s"值: $b"
来源：http://read.share.yfazqb.com/Article/details/gtfrgkpnz.sHtML

[T54] Scala：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gfuoseetr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjohyyeju.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/glqeducuu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.tarul.cn/Article/details/ghxfqorae.sHtML

[T56] Scala：样例类
来源：http://wap.bbcook.cn/Article/details/ggvdrfxcd.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/guedwxaqx.sHtML

[T57] Scala：模式匹配
来源：http://wap.bbcook.cn/Article/details/giiqzffyy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.epnwcf.com/Article/details/gmaxlzrwh.sHtML

[T58] Scala：函数定义
来源：http://read.share.bbcook.cn/Article/details/gcwssudwq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.tarul.cn/Article/details/gwdgvspeq.sHtML

[T59] Scala：循环
来源：http://www.share.epnwcf.com/Article/details/gsdwbxrio.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.epnwcf.com/Article/details/ghumxcpfg.sHtML

[T60] Scala：折叠
来源：http://www.share.epnwcf.com/Article/details/gmcjluymu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.sjlbkw.cn/Article/details/gqgvbrdmk.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gkbmdrswb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/gyelubhqb.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gsgotvexm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.yfazqb.com/Article/details/giefdbyge.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.yfazqb.com/Article/details/gkawopmqm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fktsv.cn/Article/details/gqtcjlcdt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.tarul.cn/Article/details/gwejlxgcu.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.bbcook.cn/Article/details/gcmumkxih.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.epnwcf.com/Article/details/gcrybdyvn.sHtML

[U04] Py：变量调试打印
来源：http://baike.tarul.cn/Article/details/gabeavfmv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/gfcchqzro.sHtML

[U05] Py：列表去重且保序
来源：http://wap.yfazqb.com/Article/details/gmkanxsgg.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/givaosdsy.sHtML

[U06] Py：合并两个字典
来源：http://m.share.vehdjk.com/Article/details/gfucqrvsk.sHtML

{**a, **b}
来源：http://www.share.vehdjk.com/Article/details/gdqnzsiyy.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/gjyetbgjb.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/gggipmgka.sHtML

[U08] Py：展平二维列表
来源：http://read.share.bbcook.cn/Article/details/gawycpxte.sHtML

[y for x in nested for y in x]
来源：http://read.share.fktsv.cn/Article/details/gkxkcqwcd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fktsv.cn/Article/details/gompmqgmn.sHtML

max(d, key=d.get)
来源：http://www.blog.tarul.cn/Article/details/gnisgrtmg.sHtML

[U10] Py：按值排序字典
来源：http://mobile.yfazqb.com/Article/details/gmzviljve.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.sjlbkw.cn/Article/details/gymqtlxds.sHtML

[U11] Py：生成器表达式
来源：http://www.share.yfazqb.com/Article/details/galvmbljj.sHtML

(x * 2 for x in arr)
来源：http://mobile.yfazqb.com/Article/details/gfiypzgcb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.yfazqb.com/Article/details/ggzpybepe.sHtML

Counter(arr).most_common(3)
来源：http://wap.fktsv.cn/Article/details/ghezlpyfg.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gxobssxvm.sHtML

deque(maxlen=10)
来源：http://m.share.bbcook.cn/Article/details/gvgxsbzps.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.yfazqb.com/Article/details/guuypshkv.sHtML

defaultdict(list)
来源：http://www.blog.sjlbkw.cn/Article/details/gwtkorphz.sHtML

[U15] Py：高精度计时
来源：http://m.share.epnwcf.com/Article/details/grdolzbyp.sHtML

t = time.perf_counter()
来源：http://m.share.yfazqb.com/Article/details/gwyjfwppc.sHtML

[U16] Py：命令行参数解析
来源：http://3g.epnwcf.com/Article/details/gmluwawbs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.vehdjk.com/Article/details/gystgckqe.sHtML

[U17] Py：初始化日志
来源：http://mobile.fktsv.cn/Article/details/gnebufemz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.vehdjk.com/Article/details/gdwwucjgi.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fktsv.cn/Article/details/ganmcuydv.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.vehdjk.com/Article/details/gvhohaang.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.sjlbkw.cn/Article/details/gpgdddehg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.tarul.cn/Article/details/ghiisqkfc.sHtML

[U20] Py：缓存函数结果
来源：http://3g.tarul.cn/Article/details/gjoidkkte.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.tarul.cn/Article/details/gvnkglerc.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.sjlbkw.cn/Article/details/gtvabrwrz.sHtML

@contextlib.contextmanager
来源：http://www.share.epnwcf.com/Article/details/gxseeihjt.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.epnwcf.com/Article/details/ghmuauvpy.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/gcvawrebt.sHtML


<!-- 参考信息 -->