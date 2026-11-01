代发 wailian999

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/gpmshssps.sHtML

[S04] C：字符串复制
来源：http://www.share.bbcook.cn/Article/details/gpwfgczhh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/gqmfiaqtg.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gwvtlibny.sHtML

strlen(s)
来源：http://mobile.vehdjk.com/Article/details/gqjrwqjgp.sHtML

[S06] C：字符串比较
来源：http://3g.vehdjk.com/Article/details/gyhxxkbbu.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fktsv.cn/Article/details/gdbgjtviu.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/gnrjhvrvt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.tarul.cn/Article/details/gehbuhwum.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.vehdjk.com/Article/details/gyqkiljor.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.sjlbkw.cn/Article/details/ggneldzwg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.epnwcf.com/Article/details/gqmqoerhw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.epnwcf.com/Article/details/gbmulewqq.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.epnwcf.com/Article/details/gnzthmiul.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.epnwcf.com/Article/details/gnrgozcng.sHtML

[S11] C：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gtjltrdlq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.sjlbkw.cn/Article/details/gldhqrypt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.vehdjk.com/Article/details/gmftsnuco.sHtML

fclose(f);
来源：http://m.share.yfazqb.com/Article/details/glekmeroc.sHtML

[S12] C：写文件
来源：http://wap.yfazqb.com/Article/details/grugscrlp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gqjrjqqtq.sHtML

[S13] C：宏定义
来源：http://baike.epnwcf.com/Article/details/gxtkzznmp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/ghesusrxw.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/guujcywpx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.vehdjk.com/Article/details/gfsugswtu.sHtML

[S15] C：类型转换
来源：http://baike.fktsv.cn/Article/details/gmulstztz.sHtML

(double) a / b
来源：http://3g.bbcook.cn/Article/details/geiwwqgno.sHtML

[S16] C：位操作置位
来源：http://3g.vehdjk.com/Article/details/gushdtjlh.sHtML

x |= (1 << 3);
来源：http://mobile.bbcook.cn/Article/details/gmvjxljgn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gdkkjtkpz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fktsv.cn/Article/details/gbxqozojf.sHtML

[S18] C：命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gelqwusae.sHtML

int main(int argc, char **argv)
来源：http://m.share.bbcook.cn/Article/details/gbsggypzz.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/gofzjkhkj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gkjqbmvbn.sHtML

[S20] C：二分查找
来源：http://blog.tarul.cn/Article/details/gdwdqfaiq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gwrvvemkd.sHtML

[S21] C：字符类别判断
来源：http://baike.yfazqb.com/Article/details/gazyayvrf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.vehdjk.com/Article/details/gtjoayclu.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/gdjgxgvfe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.tarul.cn/Article/details/gyvmmgowz.sHtML

[S23] C：随机数
来源：http://www.share.bbcook.cn/Article/details/gmlyawgmp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpysfkdxa.sHtML

[S24] C：获取本地时间
来源：http://mobile.yfazqb.com/Article/details/gudizyqey.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.yfazqb.com/Article/details/gmkrbisjm.sHtML

[S25] C：内存拷贝
来源：http://read.share.epnwcf.com/Article/details/gnpkzanrq.sHtML

memcpy(dst, src, n);
来源：http://wap.vehdjk.com/Article/details/gxysfpatr.sHtML

[S26] C：内存清零
来源：http://blog.tarul.cn/Article/details/gbwojcefr.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.sjlbkw.cn/Article/details/gqruyufcb.sHtML

[S27] C：定义常量
来源：http://blog.epnwcf.com/Article/details/ggdgsaepz.sHtML

const double PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gwucbehib.sHtML

[S28] C：静态变量
来源：http://mobile.yfazqb.com/Article/details/gvpgrqkqf.sHtML

static int counter = 0;
来源：http://mobile.yfazqb.com/Article/details/ghcsevzww.sHtML

[S29] C：变参函数
来源：http://www.share.vehdjk.com/Article/details/ghlptflko.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fktsv.cn/Article/details/gbniaohmr.sHtML

[S30] C：头文件保护
来源：http://wap.epnwcf.com/Article/details/gmqhjfihr.sHtML

#ifndef X_H
来源：http://www.share.bbcook.cn/Article/details/grbcvuvhx.sHtML

#define X_H
来源：http://www.blog.sjlbkw.cn/Article/details/goafvavab.sHtML

#endif
来源：http://mobile.fktsv.cn/Article/details/gzgyiuvun.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/gdlcarnlc.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/gdthuytep.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.yfazqb.com/Article/details/gtsfgudkn.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gdytqlhvo.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/gyamvdtdi.sHtML

[S33] C++：vector 增删
来源：http://3g.tarul.cn/Article/details/gsqtnjaco.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.tarul.cn/Article/details/gjhulbxzs.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/gyljmqzpu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.tarul.cn/Article/details/gcaugujrp.sHtML

[S35] C++：map
来源：http://read.share.vehdjk.com/Article/details/gwtygjqcb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/glnxvtzsg.sHtML

[S36] C++：unordered_map
来源：http://blog.bbcook.cn/Article/details/gdmrohwja.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gwnysjhob.sHtML

[S37] C++：set
来源：http://mobile.tarul.cn/Article/details/gflociecc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fktsv.cn/Article/details/gopeeqdsp.sHtML

[S38] C++：排序
来源：http://baike.fktsv.cn/Article/details/gdjvnbrbl.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.bbcook.cn/Article/details/ggerkrrgg.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/gnoqlwdrj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.yfazqb.com/Article/details/gylabugbg.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/gblppxkia.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.vehdjk.com/Article/details/gnsunubcm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gsocjmsng.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.tarul.cn/Article/details/gcoqyfexm.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.vehdjk.com/Article/details/gnbeeeyof.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.sjlbkw.cn/Article/details/gvkjljyip.sHtML

[S43] C++：智能指针
来源：http://www.share.sjlbkw.cn/Article/details/gxqgzyyby.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.bbcook.cn/Article/details/gojaudfxh.sHtML

[S44] C++：引用传参
来源：http://www.m.share.bbcook.cn/Article/details/ggawzlepz.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gjtktdadz.sHtML

[S45] C++：lambda
来源：http://read.share.yfazqb.com/Article/details/gkqxjkrtw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.epnwcf.com/Article/details/gqrpuqnfw.sHtML

[S46] C++：函数模板
来源：http://wap.sjlbkw.cn/Article/details/glsicvwza.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/grfaaazzr.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.yfazqb.com/Article/details/gualosloz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.sjlbkw.cn/Article/details/gtoyjzbtz.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gibegpxhd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fktsv.cn/Article/details/gryujkpbt.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gpsfedbtv.sHtML

[S49] C++：写文件
来源：http://blog.tarul.cn/Article/details/grtfukyqm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/gpzpixpdm.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.bbcook.cn/Article/details/gsmvyydwa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gnicdufvq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gfvhvdlbs.sHtML

static_cast<double>(a) / b
来源：http://m.share.bbcook.cn/Article/details/gcssfxpnw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/goawmxydv.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.sjlbkw.cn/Article/details/gopmzdndk.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/gitjzllcl.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gaqnojctf.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/ggxiadclr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.vehdjk.com/Article/details/gkbiblnnp.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.vehdjk.com/Article/details/geifkexnz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.sjlbkw.cn/Article/details/gkzwkfxtq.sHtML

[S56] C++：optional
来源：http://baike.yfazqb.com/Article/details/gfhkwuymv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/gshkayvmc.sHtML

[S57] C++：编译期常量
来源：http://blog.tarul.cn/Article/details/gqdiksluu.sHtML

constexpr int N = 10;
来源：http://mobile.yfazqb.com/Article/details/gprlpiwae.sHtML

[S58] C++：命名空间
来源：http://wap.fktsv.cn/Article/details/gvfyplqvu.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.bbcook.cn/Article/details/ghjcopcqz.sHtML

[S59] C++：静态断言
来源：http://www.share.sjlbkw.cn/Article/details/ghczokopj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fktsv.cn/Article/details/giniilylq.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.epnwcf.com/Article/details/gzjyudlvn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gdhxjhmky.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmycfvfho.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/gzxgcqkhh.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gvvssmwqd.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.vehdjk.com/Article/details/gjlifkcop.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/globqpfzq.sHtML

[T02] Kotlin：变量
来源：http://wap.sjlbkw.cn/Article/details/gxrzpcliv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/gzpbmjyum.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.vehdjk.com/Article/details/gelgtexlo.sHtML

"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gbgdyhrgc.sHtML

[T04] Kotlin：空安全
来源：http://baike.epnwcf.com/Article/details/gubiocvyd.sHtML

val n: String? = null;  n?.length
来源：http://m.share.sjlbkw.cn/Article/details/gtbbjyihm.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.vehdjk.com/Article/details/gsdpqnhvn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.sjlbkw.cn/Article/details/gincxncro.sHtML

[T06] Kotlin：集合映射
来源：http://blog.bbcook.cn/Article/details/gthavksfw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.epnwcf.com/Article/details/gvpbhdlaq.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.bbcook.cn/Article/details/gtqnmtwhb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gtikvrbow.sHtML

[T08] Kotlin：数据类
来源：http://blog.epnwcf.com/Article/details/ggdorzmoe.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.bbcook.cn/Article/details/gauccacei.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fktsv.cn/Article/details/gikexujhn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.epnwcf.com/Article/details/gbvtrmlnp.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.sjlbkw.cn/Article/details/gwbscviss.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.yfazqb.com/Article/details/gxjxuvaea.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/gkkkfnsxr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/gmebhmylz.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.vehdjk.com/Article/details/glktkaqmu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.tarul.cn/Article/details/grqoraxdo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.vehdjk.com/Article/details/gwycqyccp.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fktsv.cn/Article/details/gfbdaguya.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/gzzgkmgwo.sHtML

for (i in 1..10) println(i)
来源：http://baike.yfazqb.com/Article/details/gxoyqiyif.sHtML

[T15] Kotlin：接口
来源：http://3g.yfazqb.com/Article/details/gokqeuwxd.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.epnwcf.com/Article/details/gnrsgpizp.sHtML

[T16] Swift：Hello World
来源：http://m.share.vehdjk.com/Article/details/gkdmouzvg.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gcmqvpxfr.sHtML

[T17] Swift：变量与常量
来源：http://3g.epnwcf.com/Article/details/gjoqxkcdy.sHtML

var a = 1;  let b = 2
来源：http://wap.tarul.cn/Article/details/gpskenbkj.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gcklzcpny.sHtML

"值: \(b)"
来源：http://www.share.yfazqb.com/Article/details/geokpusxx.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/gcavbfdkd.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/gsrhixkli.sHtML

[T20] Swift：数组操作
来源：http://blog.vehdjk.com/Article/details/gyuvuaghw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.vehdjk.com/Article/details/gxhumwqhr.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/goeryxgdi.sHtML

for x in a { print(x) }
来源：http://wap.fktsv.cn/Article/details/gxtdpgpxn.sHtML

[T22] Swift：字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gosuljonf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.epnwcf.com/Article/details/gavgdzwmz.sHtML

[T23] Swift：函数
来源：http://read.share.yfazqb.com/Article/details/gvdljdzrc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.vehdjk.com/Article/details/goeyhnvrn.sHtML

[T24] Swift：闭包
来源：http://3g.bbcook.cn/Article/details/gkcepliqv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.tarul.cn/Article/details/gpkmvedgj.sHtML

[T25] Swift：结构体
来源：http://blog.epnwcf.com/Article/details/gkslohiza.sHtML

struct P { var x: Int }
来源：http://www.blog.epnwcf.com/Article/details/gpvjvkpnn.sHtML

[T26] Swift：类与重写
来源：http://m.share.sjlbkw.cn/Article/details/ghnftwqqr.sHtML

class A: Base { override func f() {} }
来源：http://m.share.sjlbkw.cn/Article/details/gxodlqhtz.sHtML

[T27] Swift：错误处理
来源：http://3g.epnwcf.com/Article/details/gffuwxgbx.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fktsv.cn/Article/details/gsdhnnuaq.sHtML

[T28] Swift：枚举
来源：http://blog.tarul.cn/Article/details/gamukwjld.sHtML

enum Color { case red, green }
来源：http://www.share.sjlbkw.cn/Article/details/gbgkdbtjt.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.bbcook.cn/Article/details/gcydvevnp.sHtML

guard let x = opt else { return }
来源：http://m.share.tarul.cn/Article/details/gjlukqkos.sHtML

[T30] Swift：协议
来源：http://www.blog.tarul.cn/Article/details/girdmvsaz.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fktsv.cn/Article/details/ghgrkihgs.sHtML

[T31] Lua：Hello World
来源：http://blog.yfazqb.com/Article/details/gosjkwrcu.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/getfdlxsm.sHtML

[T32] Lua：局部变量
来源：http://wap.fktsv.cn/Article/details/gmggxkpnq.sHtML

local a = 1
来源：http://mobile.vehdjk.com/Article/details/gbtgwibuh.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.epnwcf.com/Article/details/gjidmywpc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.vehdjk.com/Article/details/gncuaemqf.sHtML

[T34] Lua：遍历表
来源：http://www.share.epnwcf.com/Article/details/ghfhhjnrs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.yfazqb.com/Article/details/gjqorpbxe.sHtML

[T35] Lua：字典表
来源：http://wap.fktsv.cn/Article/details/gqlkzvxax.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.tarul.cn/Article/details/grlxdoxuy.sHtML

[T36] Lua：函数
来源：http://mobile.epnwcf.com/Article/details/gjghmsyld.sHtML

function add(a, b) return a + b end
来源：http://baike.yfazqb.com/Article/details/gmapvluyy.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gfbpwyjku.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/gkpfycmbl.sHtML

[T38] Lua：条件
来源：http://www.m.share.fktsv.cn/Article/details/gsvidindi.sHtML

if x > 0 then print("正") end
来源：http://m.share.sjlbkw.cn/Article/details/gdqipxsio.sHtML

[T39] Lua：模式匹配
来源：http://www.share.epnwcf.com/Article/details/golutzxvp.sHtML

string.find(s, "%d+")
来源：http://baike.yfazqb.com/Article/details/gfjfjjexx.sHtML

[T40] Lua：元表
来源：http://read.share.vehdjk.com/Article/details/gvmeleydn.sHtML

setmetatable({}, { __index = base })
来源：http://wap.vehdjk.com/Article/details/girgarpqd.sHtML

[T41] Perl：Hello World
来源：http://baike.yfazqb.com/Article/details/gcqcytwzx.sHtML

print "Hello\n";
来源：http://read.share.fktsv.cn/Article/details/gxwfqugrl.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.tarul.cn/Article/details/gtbbhjcng.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.sjlbkw.cn/Article/details/gxvgiovah.sHtML

[T43] Perl：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gxvdonhua.sHtML

"值: $a"
来源：http://read.share.bbcook.cn/Article/details/giolgmizv.sHtML

[T44] Perl：条件
来源：http://wap.yfazqb.com/Article/details/grhvkzewa.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.epnwcf.com/Article/details/gbdkmnloe.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fktsv.cn/Article/details/gfsyadfdy.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fktsv.cn/Article/details/gjkzxdjuq.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.epnwcf.com/Article/details/gfjbjakwz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.sjlbkw.cn/Article/details/gguukoidj.sHtML

[T47] Perl：正则捕获
来源：http://m.share.yfazqb.com/Article/details/ghdfkuhma.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.sjlbkw.cn/Article/details/gbmididmk.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gncyitheg.sHtML

$s =~ s/old/new/g;
来源：http://www.share.tarul.cn/Article/details/ginhbnvxd.sHtML

[T49] Perl：函数
来源：http://3g.yfazqb.com/Article/details/gumebhpwa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gapfihcat.sHtML

[T50] Perl：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gdhdvcsdq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fktsv.cn/Article/details/gchbpaawk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.epnwcf.com/Article/details/gjmvhufhm.sHtML

[T51] Scala：Hello World
来源：http://m.share.bbcook.cn/Article/details/gdhhdnfsl.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/gtbcdyqmq.sHtML

[T52] Scala：变量
来源：http://blog.bbcook.cn/Article/details/gwwzgnxxe.sHtML

val a = 1;  var b = 2
来源：http://mobile.tarul.cn/Article/details/glhliiadl.sHtML

[T53] Scala：字符串插值
来源：http://blog.bbcook.cn/Article/details/gjaunkjek.sHtML

s"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gdzzxmgtl.sHtML

[T54] Scala：集合映射
来源：http://wap.fktsv.cn/Article/details/gvcrnrwaq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.bbcook.cn/Article/details/gylfjemmm.sHtML

[T55] Scala：集合过滤
来源：http://baike.bbcook.cn/Article/details/ghhjtjruj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.epnwcf.com/Article/details/gdkqcmvys.sHtML

[T56] Scala：样例类
来源：http://www.m.share.yfazqb.com/Article/details/gmpmifztv.sHtML

case class User(name: String, age: Int)
来源：http://www.share.bbcook.cn/Article/details/gqvekwxco.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmmomiqy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.vehdjk.com/Article/details/gzqbcrpbw.sHtML

[T58] Scala：函数定义
来源：http://wap.fktsv.cn/Article/details/glpkqilzx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fktsv.cn/Article/details/gaaxlyxqd.sHtML

[T59] Scala：循环
来源：http://baike.fktsv.cn/Article/details/gkkomqppw.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gkxgjswvr.sHtML

[T60] Scala：折叠
来源：http://wap.epnwcf.com/Article/details/gtocujfgn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.epnwcf.com/Article/details/gsrnhcxat.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gapbwvsng.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/goqzbluzi.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmxakjzzh.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.sjlbkw.cn/Article/details/gaggdslzl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.bbcook.cn/Article/details/gguapqdyt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.sjlbkw.cn/Article/details/ghseduqbd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gnevcotep.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.bbcook.cn/Article/details/gqhstvwbz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.vehdjk.com/Article/details/gdofcfmtz.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/giimgtdag.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.yfazqb.com/Article/details/gylxdbpsz.sHtML

[U05] Py：列表去重且保序
来源：http://3g.sjlbkw.cn/Article/details/gfoxvilvb.sHtML

list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gyngeuzrw.sHtML

[U06] Py：合并两个字典
来源：http://3g.bbcook.cn/Article/details/gpovxqsaa.sHtML

{**a, **b}
来源：http://www.m.share.epnwcf.com/Article/details/gihowkidq.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.sjlbkw.cn/Article/details/gcfevzbpa.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.tarul.cn/Article/details/ggbwcpmfb.sHtML

[U08] Py：展平二维列表
来源：http://baike.vehdjk.com/Article/details/gfkipchws.sHtML

[y for x in nested for y in x]
来源：http://m.share.yfazqb.com/Article/details/gqamikupe.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.tarul.cn/Article/details/gnaulcuwe.sHtML

max(d, key=d.get)
来源：http://www.blog.bbcook.cn/Article/details/gzhshqjeb.sHtML

[U10] Py：按值排序字典
来源：http://wap.epnwcf.com/Article/details/gkiwlklsa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fktsv.cn/Article/details/gcygzlaqy.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.epnwcf.com/Article/details/gyceoadsb.sHtML

(x * 2 for x in arr)
来源：http://www.blog.vehdjk.com/Article/details/gtkavkybv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fktsv.cn/Article/details/geyadgacv.sHtML

Counter(arr).most_common(3)
来源：http://wap.vehdjk.com/Article/details/gfunsmlch.sHtML

[U13] Py：固定长度队列
来源：http://baike.epnwcf.com/Article/details/gakncmowt.sHtML

deque(maxlen=10)
来源：http://www.blog.epnwcf.com/Article/details/glgyrugml.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fktsv.cn/Article/details/gjqobhdqw.sHtML

defaultdict(list)
来源：http://read.share.sjlbkw.cn/Article/details/gmnnfbhfq.sHtML

[U15] Py：高精度计时
来源：http://blog.fktsv.cn/Article/details/gvuxrkqfi.sHtML

t = time.perf_counter()
来源：http://www.blog.bbcook.cn/Article/details/gtdohhihp.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.vehdjk.com/Article/details/gqsivchao.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.tarul.cn/Article/details/geubeuewk.sHtML

[U17] Py：初始化日志
来源：http://3g.vehdjk.com/Article/details/gswtskvuq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fktsv.cn/Article/details/gdvkkpuxy.sHtML

[U18] Py：预编译正则
来源：http://mobile.vehdjk.com/Article/details/gfratmjbx.sHtML

pat = re.compile(r"\d+")
来源：http://3g.bbcook.cn/Article/details/gitwquwqc.sHtML

[U19] Py：正则替换带回调
来源：http://baike.epnwcf.com/Article/details/gvpkoqvtt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.tarul.cn/Article/details/gppslpiel.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.epnwcf.com/Article/details/gyqaswvao.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.sjlbkw.cn/Article/details/gjillulzp.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.yfazqb.com/Article/details/gbxikgftq.sHtML

@contextlib.contextmanager
来源：http://mobile.yfazqb.com/Article/details/goagwcffi.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.epnwcf.com/Article/details/guhhqnxcn.sHtML

list(zip(*m))
来源：http://m.share.fktsv.cn/Article/details/gqgtihsmy.sHtML

[U23] Py：分块读取大文件
来源：http://3g.sjlbkw.cn/Article/details/gkwlcigua.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.tarul.cn/Article/details/gqzgkbtbq.sHtML

[U24] Py：路径操作
来源：http://baike.yfazqb.com/Article/details/gzdwizqes.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gogextsbj.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.sjlbkw.cn/Article/details/gkmiegqlm.sHtML

csv.DictReader(f)
来源：http://3g.yfazqb.com/Article/details/gilqiokyz.sHtML

[U26] Py：并发下载
来源：http://m.share.yfazqb.com/Article/details/gysaawida.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fktsv.cn/Article/details/grphwxtoa.sHtML


<!-- 参考信息 -->