代发 wailian999

strlen(s)
来源：http://3g.fktsv.cn/Article/details/gsujwnvql.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gdxljcuxd.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/gbuzjhirn.sHtML

[S07] C：数组遍历求和
来源：http://3g.bbcook.cn/Article/details/gdzjtluay.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.vehdjk.com/Article/details/gysnwmcho.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.vehdjk.com/Article/details/gpmptnyrr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.tarul.cn/Article/details/goqddslsr.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.sjlbkw.cn/Article/details/gtkukfwqp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.yfazqb.com/Article/details/gmclroddu.sHtML

[S10] C：指针与解引用
来源：http://m.share.tarul.cn/Article/details/giijmwfpm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/gizewnipn.sHtML

[S11] C：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gbeuankje.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.bbcook.cn/Article/details/gpusfvqbf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.tarul.cn/Article/details/geluotomv.sHtML

fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gogjkwzsq.sHtML

[S12] C：写文件
来源：http://baike.epnwcf.com/Article/details/gdczvwgbv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.epnwcf.com/Article/details/gpunkbyjz.sHtML

[S13] C：宏定义
来源：http://mobile.epnwcf.com/Article/details/gpscfhhfg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/gfrkqrykm.sHtML

[S14] C：枚举
来源：http://3g.vehdjk.com/Article/details/gcurfnjhd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/gejnzbjyx.sHtML

[S15] C：类型转换
来源：http://mobile.fktsv.cn/Article/details/gqhevotkd.sHtML

(double) a / b
来源：http://mobile.bbcook.cn/Article/details/gqvogsmkr.sHtML

[S16] C：位操作置位
来源：http://www.share.yfazqb.com/Article/details/ghjhtwako.sHtML

x |= (1 << 3);
来源：http://wap.yfazqb.com/Article/details/gtlrnjbjf.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gyjouhblp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fktsv.cn/Article/details/gptbcrbdv.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/gscymrlqk.sHtML

int main(int argc, char **argv)
来源：http://read.share.tarul.cn/Article/details/gwktilbit.sHtML

[S19] C：快速排序
来源：http://read.share.vehdjk.com/Article/details/gvtagpmfu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gpzrzcqlk.sHtML

[S20] C：二分查找
来源：http://www.blog.sjlbkw.cn/Article/details/gaubjfhyg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/gfsdxgusv.sHtML

[S21] C：字符类别判断
来源：http://m.share.epnwcf.com/Article/details/gxzeyvxua.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.tarul.cn/Article/details/gqoknkqcz.sHtML

[S22] C：字符串转数字
来源：http://mobile.bbcook.cn/Article/details/gxxmavaiy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.tarul.cn/Article/details/gzwicgxoy.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/gbbyykuzu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gfasxjnkh.sHtML

[S24] C：获取本地时间
来源：http://www.blog.epnwcf.com/Article/details/gwedjvrjd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/gobhtbrjv.sHtML

[S25] C：内存拷贝
来源：http://wap.epnwcf.com/Article/details/gawuljfng.sHtML

memcpy(dst, src, n);
来源：http://blog.yfazqb.com/Article/details/ggvcfzjpy.sHtML

[S26] C：内存清零
来源：http://www.m.share.yfazqb.com/Article/details/gjqjfesgw.sHtML

memset(a, 0, sizeof a);
来源：http://blog.tarul.cn/Article/details/gxevxslmd.sHtML

[S27] C：定义常量
来源：http://wap.yfazqb.com/Article/details/gplaieqpg.sHtML

const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gixifmkog.sHtML

[S28] C：静态变量
来源：http://read.share.tarul.cn/Article/details/gvtdgpolx.sHtML

static int counter = 0;
来源：http://www.m.share.vehdjk.com/Article/details/gxnzpcndm.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/gzgztcjgm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.yfazqb.com/Article/details/gvtmbghyq.sHtML

[S30] C：头文件保护
来源：http://3g.sjlbkw.cn/Article/details/gbshhsowu.sHtML

#ifndef X_H
来源：http://m.share.bbcook.cn/Article/details/gjrwhpzcu.sHtML

#define X_H
来源：http://www.blog.vehdjk.com/Article/details/ganuxxfos.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/gomosycoa.sHtML

[S31] C++：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gunoqzyvd.sHtML

#include <iostream>
来源：http://3g.yfazqb.com/Article/details/gcbcpwpbo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.epnwcf.com/Article/details/gahcjztgm.sHtML

[S32] C++：字符串
来源：http://www.share.epnwcf.com/Article/details/gbwmrluoc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/gdumncxzw.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gcrkognlp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gjzbpdrmh.sHtML

[S34] C++：遍历 vector
来源：http://blog.bbcook.cn/Article/details/gpiatlyce.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fktsv.cn/Article/details/gdybqopoh.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/gnjyocvyg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/glvyisyzj.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/gzvfcftjk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gzzjyuayv.sHtML

[S37] C++：set
来源：http://3g.sjlbkw.cn/Article/details/gtcobijfo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.sjlbkw.cn/Article/details/gtvpperar.sHtML

[S38] C++：排序
来源：http://www.blog.epnwcf.com/Article/details/ggkrfooso.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.vehdjk.com/Article/details/gnxdwdlxk.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/gtwqohave.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/gczwdhozz.sHtML

[S40] C++：查找元素
来源：http://www.share.epnwcf.com/Article/details/gemgioltr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/gtrhasacr.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fktsv.cn/Article/details/glcoxhyng.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.sjlbkw.cn/Article/details/gmzhnhief.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.bbcook.cn/Article/details/gvtkslnpf.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.tarul.cn/Article/details/gurydcpkh.sHtML

[S43] C++：智能指针
来源：http://www.m.share.vehdjk.com/Article/details/gwrmzudmk.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.sjlbkw.cn/Article/details/goraoenvj.sHtML

[S44] C++：引用传参
来源：http://blog.bbcook.cn/Article/details/gkfablclz.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.yfazqb.com/Article/details/gqysphfcf.sHtML

[S45] C++：lambda
来源：http://wap.epnwcf.com/Article/details/glwvlhsws.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fktsv.cn/Article/details/gdsqjwxee.sHtML

[S46] C++：函数模板
来源：http://www.m.share.bbcook.cn/Article/details/gannkcfko.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.vehdjk.com/Article/details/gniwrvqkj.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.epnwcf.com/Article/details/gvbockohb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fktsv.cn/Article/details/gzdzbmhxd.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gxttfhggr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.yfazqb.com/Article/details/gzxzagfef.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gwsvfuuoo.sHtML

[S49] C++：写文件
来源：http://baike.vehdjk.com/Article/details/ghmidwpld.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.vehdjk.com/Article/details/gpetmnfaq.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fktsv.cn/Article/details/ghcblwoaz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.tarul.cn/Article/details/gnwvksusu.sHtML

[S51] C++：显式类型转换
来源：http://read.share.epnwcf.com/Article/details/guhmoowsj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.yfazqb.com/Article/details/gggusjmuq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/golcxkuoi.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.vehdjk.com/Article/details/gbuzzcdog.sHtML

[S53] C++：移动语义
来源：http://blog.tarul.cn/Article/details/gzjwqqjxb.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/gisbmryew.sHtML

[S54] C++：异常处理
来源：http://baike.epnwcf.com/Article/details/gyhcoqjtk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.epnwcf.com/Article/details/ggukcuqek.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/gsswmcnrx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.epnwcf.com/Article/details/gzoidlrdc.sHtML

[S56] C++：optional
来源：http://wap.bbcook.cn/Article/details/guihgefxz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.yfazqb.com/Article/details/gtdwbznqd.sHtML

[S57] C++：编译期常量
来源：http://m.share.vehdjk.com/Article/details/gylzsugbu.sHtML

constexpr int N = 10;
来源：http://baike.tarul.cn/Article/details/gzgygskmi.sHtML

[S58] C++：命名空间
来源：http://m.share.vehdjk.com/Article/details/gkwruwpic.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.tarul.cn/Article/details/gdbugnnfb.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/gcuinydcs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.epnwcf.com/Article/details/gsiqqwnfj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gmjquanua.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/gczpaejns.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gbhiftgmx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.epnwcf.com/Article/details/gbgvqkrgt.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gaaotcumh.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gxmqvcnbj.sHtML

println("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gahvrjnrf.sHtML

[T02] Kotlin：变量
来源：http://wap.vehdjk.com/Article/details/gxfwojbwy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/gwfxwrogv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fktsv.cn/Article/details/goydfogui.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gxuzzyrcx.sHtML

[T04] Kotlin：空安全
来源：http://www.share.tarul.cn/Article/details/gwwzcmeyq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.vehdjk.com/Article/details/gogmhlwid.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.yfazqb.com/Article/details/gthozivld.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.tarul.cn/Article/details/gzieznpti.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/gnbacyree.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gyeqxnzyz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gnbryutdn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gbygvvcsh.sHtML

[T08] Kotlin：数据类
来源：http://www.share.tarul.cn/Article/details/gnuozhctn.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.yfazqb.com/Article/details/gkqormkox.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.tarul.cn/Article/details/geityozgl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.sjlbkw.cn/Article/details/gueztiemi.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.epnwcf.com/Article/details/gdfcuzmhv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.bbcook.cn/Article/details/gwmcloxxr.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.vehdjk.com/Article/details/gzazdiyeu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.tarul.cn/Article/details/ghtxgehfz.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/gylxxhcoq.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.vehdjk.com/Article/details/giygxhwed.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.sjlbkw.cn/Article/details/gyvviutew.sHtML

val m = mapOf("a" to 1)
来源：http://wap.bbcook.cn/Article/details/gesmewqvz.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gwcmxvdsr.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/gkascfzmw.sHtML

[T15] Kotlin：接口
来源：http://www.share.epnwcf.com/Article/details/gdrpccbys.sHtML

interface Shape { fun area(): Double }
来源：http://baike.epnwcf.com/Article/details/grwkhbwtv.sHtML

[T16] Swift：Hello World
来源：http://baike.fktsv.cn/Article/details/gxmexotgr.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/grcdprjwy.sHtML

[T17] Swift：变量与常量
来源：http://wap.sjlbkw.cn/Article/details/gwmgasyxf.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gusdukmhl.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gnrvylgzd.sHtML

"值: \(b)"
来源：http://baike.tarul.cn/Article/details/gcmulwcce.sHtML

[T19] Swift：可选绑定
来源：http://blog.yfazqb.com/Article/details/gcaidmgji.sHtML

if let n = opt { print(n) }
来源：http://m.share.yfazqb.com/Article/details/ghwwijgjk.sHtML

[T20] Swift：数组操作
来源：http://www.blog.tarul.cn/Article/details/gepecpquk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/gtkshksde.sHtML

[T21] Swift：遍历
来源：http://3g.epnwcf.com/Article/details/gmmnjaegg.sHtML

for x in a { print(x) }
来源：http://www.m.share.vehdjk.com/Article/details/gmjbdjtgw.sHtML

[T22] Swift：字典
来源：http://3g.sjlbkw.cn/Article/details/giaflezza.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fktsv.cn/Article/details/ghlazazgg.sHtML

[T23] Swift：函数
来源：http://read.share.tarul.cn/Article/details/gdehgiwfs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gattpeemp.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/gvzgjojqj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gpvamzqqu.sHtML

[T25] Swift：结构体
来源：http://www.blog.bbcook.cn/Article/details/gioseonza.sHtML

struct P { var x: Int }
来源：http://blog.vehdjk.com/Article/details/gilwcnpdw.sHtML

[T26] Swift：类与重写
来源：http://www.share.bbcook.cn/Article/details/gqpndlwxd.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.bbcook.cn/Article/details/glwyfrdvv.sHtML

[T27] Swift：错误处理
来源：http://blog.fktsv.cn/Article/details/gqwswxybo.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.yfazqb.com/Article/details/gbxlpljxr.sHtML

[T28] Swift：枚举
来源：http://wap.sjlbkw.cn/Article/details/gumwoaulr.sHtML

enum Color { case red, green }
来源：http://baike.vehdjk.com/Article/details/gmwzykkym.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fktsv.cn/Article/details/gjljqijvp.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/gkxxzyhfi.sHtML

[T30] Swift：协议
来源：http://baike.bbcook.cn/Article/details/gyhlaajgx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.bbcook.cn/Article/details/gvnprseoi.sHtML

[T31] Lua：Hello World
来源：http://read.share.epnwcf.com/Article/details/gbynkdbpa.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gbhbavgza.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gwfwojjra.sHtML

local a = 1
来源：http://www.share.yfazqb.com/Article/details/gddxrzbjw.sHtML

[T33] Lua：表（数组）
来源：http://3g.bbcook.cn/Article/details/gonmorxrl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.vehdjk.com/Article/details/gaheooeei.sHtML

[T34] Lua：遍历表
来源：http://www.share.vehdjk.com/Article/details/glslreahl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.tarul.cn/Article/details/geosxpvrb.sHtML

[T35] Lua：字典表
来源：http://read.share.bbcook.cn/Article/details/gvbvnqhvt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.bbcook.cn/Article/details/gncvbzkxx.sHtML

[T36] Lua：函数
来源：http://mobile.tarul.cn/Article/details/gqybbgrqc.sHtML

function add(a, b) return a + b end
来源：http://www.share.vehdjk.com/Article/details/ggizojhbh.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/ghheeguyv.sHtML

"a" .. "b"
来源：http://mobile.sjlbkw.cn/Article/details/gydwuetvx.sHtML

[T38] Lua：条件
来源：http://www.m.share.tarul.cn/Article/details/glkafaast.sHtML

if x > 0 then print("正") end
来源：http://m.share.vehdjk.com/Article/details/gqrhhmjlt.sHtML

[T39] Lua：模式匹配
来源：http://wap.fktsv.cn/Article/details/gbmearjwx.sHtML

string.find(s, "%d+")
来源：http://baike.epnwcf.com/Article/details/gnasqnjim.sHtML

[T40] Lua：元表
来源：http://www.blog.sjlbkw.cn/Article/details/gwsadukdc.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.vehdjk.com/Article/details/gobnmcpfb.sHtML

[T41] Perl：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gsnvdnwau.sHtML

print "Hello\n";
来源：http://3g.yfazqb.com/Article/details/gniuqgjqn.sHtML

[T42] Perl：变量类型
来源：http://wap.sjlbkw.cn/Article/details/gcpaatpcb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.tarul.cn/Article/details/gsbchqrye.sHtML

[T43] Perl：字符串插值
来源：http://baike.epnwcf.com/Article/details/gsfyhesfg.sHtML

"值: $a"
来源：http://www.m.share.epnwcf.com/Article/details/gmsojfxof.sHtML

[T44] Perl：条件
来源：http://www.blog.bbcook.cn/Article/details/gsmgkkndt.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.epnwcf.com/Article/details/grvatdyyo.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fktsv.cn/Article/details/giaszstoa.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.yfazqb.com/Article/details/gtgsftbet.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.tarul.cn/Article/details/gnakqacyv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.bbcook.cn/Article/details/grlbsgiur.sHtML

[T47] Perl：正则捕获
来源：http://m.share.vehdjk.com/Article/details/ggxldqtpj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.vehdjk.com/Article/details/gnqslkpbq.sHtML

[T48] Perl：正则替换
来源：http://mobile.sjlbkw.cn/Article/details/guorqmvrs.sHtML

$s =~ s/old/new/g;
来源：http://baike.yfazqb.com/Article/details/gsugyahei.sHtML

[T49] Perl：函数
来源：http://baike.vehdjk.com/Article/details/guoxtxhwy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gxvvnbpdi.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/glmxlsjzi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.yfazqb.com/Article/details/gqujrjije.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.tarul.cn/Article/details/gndseqqjf.sHtML

[T51] Scala：Hello World
来源：http://wap.vehdjk.com/Article/details/gewywackv.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gffzypuun.sHtML

[T52] Scala：变量
来源：http://www.share.tarul.cn/Article/details/gykyskglj.sHtML

val a = 1;  var b = 2
来源：http://3g.tarul.cn/Article/details/gnfxxmtyp.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/ghvmqrnga.sHtML

s"值: $b"
来源：http://blog.vehdjk.com/Article/details/gjqpdcmoz.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/gbpxoyvwx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.bbcook.cn/Article/details/gobuhpxdm.sHtML

[T55] Scala：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gnypgealk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.bbcook.cn/Article/details/gsqgypmra.sHtML

[T56] Scala：样例类
来源：http://3g.sjlbkw.cn/Article/details/gsbtnpbdx.sHtML

case class User(name: String, age: Int)
来源：http://wap.epnwcf.com/Article/details/gfxwswgol.sHtML

[T57] Scala：模式匹配
来源：http://m.share.tarul.cn/Article/details/goamvhufw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.tarul.cn/Article/details/gbnryyknr.sHtML

[T58] Scala：函数定义
来源：http://www.share.sjlbkw.cn/Article/details/gjkqjgcbe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.vehdjk.com/Article/details/gkcvqzjkv.sHtML

[T59] Scala：循环
来源：http://wap.bbcook.cn/Article/details/goeapkisc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.yfazqb.com/Article/details/gsuqsomos.sHtML

[T60] Scala：折叠
来源：http://baike.bbcook.cn/Article/details/gefxzkcdq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.sjlbkw.cn/Article/details/glluidtna.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ghfwogrgb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fktsv.cn/Article/details/gzfeinatd.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/graememef.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.yfazqb.com/Article/details/gortxwhgx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fktsv.cn/Article/details/gzwuhwkse.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.yfazqb.com/Article/details/gvmpdymes.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.yfazqb.com/Article/details/gtjrbqrtx.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.vehdjk.com/Article/details/gqsinhcfn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.epnwcf.com/Article/details/ggdbrsunp.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fktsv.cn/Article/details/glkjqyjny.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fktsv.cn/Article/details/gdsyjmaxt.sHtML

[U05] Py：列表去重且保序
来源：http://blog.bbcook.cn/Article/details/glwkzsgsc.sHtML

list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gekjkpgvw.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.vehdjk.com/Article/details/gjvsukxod.sHtML

{**a, **b}
来源：http://www.blog.tarul.cn/Article/details/gzmwubybn.sHtML

[U07] Py：反转字典键值
来源：http://www.share.sjlbkw.cn/Article/details/gazwjzlvm.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.sjlbkw.cn/Article/details/glkebhwui.sHtML

[U08] Py：展平二维列表
来源：http://blog.yfazqb.com/Article/details/gxndbjkcv.sHtML

[y for x in nested for y in x]
来源：http://read.share.yfazqb.com/Article/details/gevktoekg.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.vehdjk.com/Article/details/gdgpdkejt.sHtML

max(d, key=d.get)
来源：http://mobile.vehdjk.com/Article/details/gbmoasubd.sHtML

[U10] Py：按值排序字典
来源：http://baike.vehdjk.com/Article/details/gwsfgzcyg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.yfazqb.com/Article/details/guwxaiovr.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fktsv.cn/Article/details/grqgtczeg.sHtML

(x * 2 for x in arr)
来源：http://blog.tarul.cn/Article/details/gahxywjtp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.yfazqb.com/Article/details/gctltkvlj.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.bbcook.cn/Article/details/ggrgwlcum.sHtML

[U13] Py：固定长度队列
来源：http://m.share.vehdjk.com/Article/details/giazumnor.sHtML

deque(maxlen=10)
来源：http://read.share.vehdjk.com/Article/details/gxsnchgqc.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fktsv.cn/Article/details/gaxegwseo.sHtML

defaultdict(list)
来源：http://m.share.tarul.cn/Article/details/gxqzoiljz.sHtML

[U15] Py：高精度计时
来源：http://baike.bbcook.cn/Article/details/gnzjefznl.sHtML

t = time.perf_counter()
来源：http://baike.fktsv.cn/Article/details/gxturfkat.sHtML

[U16] Py：命令行参数解析
来源：http://baike.epnwcf.com/Article/details/goevhnvdp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fktsv.cn/Article/details/gmhppgzmj.sHtML

[U17] Py：初始化日志
来源：http://m.share.yfazqb.com/Article/details/gvdnwktpc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.vehdjk.com/Article/details/gjtijdcuh.sHtML

[U18] Py：预编译正则
来源：http://3g.tarul.cn/Article/details/gkjotapmq.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gpqbzyloh.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.bbcook.cn/Article/details/gexpljzug.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fktsv.cn/Article/details/gpjeckusq.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fktsv.cn/Article/details/geazybiyj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.epnwcf.com/Article/details/gumfcqlzc.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.vehdjk.com/Article/details/glfkjxcom.sHtML

@contextlib.contextmanager
来源：http://baike.yfazqb.com/Article/details/gqfxqlyjl.sHtML

[U22] Py：矩阵转置
来源：http://blog.epnwcf.com/Article/details/gegryrpbl.sHtML

list(zip(*m))
来源：http://mobile.epnwcf.com/Article/details/gaginutdm.sHtML

[U23] Py：分块读取大文件
来源：http://baike.epnwcf.com/Article/details/gqoptimnx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.epnwcf.com/Article/details/gcurgnqis.sHtML

[U24] Py：路径操作
来源：http://wap.sjlbkw.cn/Article/details/gcvryvcht.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.yfazqb.com/Article/details/goucusauo.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.epnwcf.com/Article/details/gfyyszmsn.sHtML

csv.DictReader(f)
来源：http://read.share.epnwcf.com/Article/details/gpehpadne.sHtML

[U26] Py：并发下载
来源：http://wap.epnwcf.com/Article/details/gidakuqxx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.sjlbkw.cn/Article/details/gxzltuhnf.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.bbcook.cn/Article/details/gkasbrprh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.tarul.cn/Article/details/gunxlsfdy.sHtML

[U28] Py：类型别名
来源：http://www.share.fktsv.cn/Article/details/gevphzowx.sHtML

UserId = int
来源：http://baike.yfazqb.com/Article/details/geacxlwgf.sHtML


<!-- 参考信息 -->