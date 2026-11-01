代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.bbcook.cn/Article/details/ggkstuufd.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fktsv.cn/Article/details/gblvjbwbk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/gvnrbgafp.sHtML

[S03] C：读入整数
来源：http://mobile.fktsv.cn/Article/details/grsusczrk.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/gradusjcv.sHtML

[S04] C：字符串复制
来源：http://baike.bbcook.cn/Article/details/gqbumeysc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.vehdjk.com/Article/details/geilxudbp.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/guebqnyyz.sHtML

strlen(s)
来源：http://www.blog.vehdjk.com/Article/details/ggkdenhkw.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/gapetqjbj.sHtML

strcmp(a, b) == 0
来源：http://m.share.yfazqb.com/Article/details/gpsgupswe.sHtML

[S07] C：数组遍历求和
来源：http://read.share.epnwcf.com/Article/details/gpdtlmhxk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/gxsiyigoh.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/gycbvqyod.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/ghxxwpyyn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.epnwcf.com/Article/details/glktlyhjl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/gpywsbdog.sHtML

[S10] C：指针与解引用
来源：http://www.blog.bbcook.cn/Article/details/gysfjdoxz.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fktsv.cn/Article/details/giithykcl.sHtML

[S11] C：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gphmqknmh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.bbcook.cn/Article/details/ggchjfhdg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gchxnrqwv.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/gqecdfpvu.sHtML

[S12] C：写文件
来源：http://read.share.tarul.cn/Article/details/gkoolxxej.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.epnwcf.com/Article/details/gjulxrnmy.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gabjrtafc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.sjlbkw.cn/Article/details/gxwvqlejm.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/gdhpojyie.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fktsv.cn/Article/details/gloicnjuj.sHtML

[S15] C：类型转换
来源：http://3g.epnwcf.com/Article/details/gvgmzvjjq.sHtML

(double) a / b
来源：http://www.blog.yfazqb.com/Article/details/gjnugfhku.sHtML

[S16] C：位操作置位
来源：http://read.share.tarul.cn/Article/details/gpocblfss.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/gfutwrsdt.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/geelxvxot.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.tarul.cn/Article/details/gwpezbvba.sHtML

[S18] C：命令行参数
来源：http://baike.tarul.cn/Article/details/gbmllamfg.sHtML

int main(int argc, char **argv)
来源：http://baike.sjlbkw.cn/Article/details/gjzuahbgt.sHtML

[S19] C：快速排序
来源：http://m.share.vehdjk.com/Article/details/gldkxukoq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gcewsuuvc.sHtML

[S20] C：二分查找
来源：http://read.share.fktsv.cn/Article/details/gvobvricj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gvwnfkzii.sHtML

[S21] C：字符类别判断
来源：http://3g.epnwcf.com/Article/details/gjartbsdx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.tarul.cn/Article/details/gvuggcvdr.sHtML

[S22] C：字符串转数字
来源：http://blog.fktsv.cn/Article/details/glvaochuk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.tarul.cn/Article/details/gwtoaxebh.sHtML

[S23] C：随机数
来源：http://www.m.share.tarul.cn/Article/details/grjnkwnah.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.vehdjk.com/Article/details/gwisltnwh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/gpygfyzhu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.sjlbkw.cn/Article/details/ggkdemzuy.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gwdgmaqeg.sHtML

memcpy(dst, src, n);
来源：http://mobile.epnwcf.com/Article/details/gfnogjvmt.sHtML

[S26] C：内存清零
来源：http://www.m.share.fktsv.cn/Article/details/gpqhmsxvt.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.bbcook.cn/Article/details/gvefaocaj.sHtML

[S27] C：定义常量
来源：http://baike.yfazqb.com/Article/details/gztdyehbg.sHtML

const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gcdacqvtf.sHtML

[S28] C：静态变量
来源：http://www.blog.sjlbkw.cn/Article/details/gfryheptz.sHtML

static int counter = 0;
来源：http://mobile.yfazqb.com/Article/details/grhdcihaj.sHtML

[S29] C：变参函数
来源：http://baike.epnwcf.com/Article/details/gzsbwrmsp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.sjlbkw.cn/Article/details/ghzeermwm.sHtML

[S30] C：头文件保护
来源：http://m.share.tarul.cn/Article/details/glzdnzuys.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/gzcrtmpgh.sHtML

#define X_H
来源：http://www.blog.fktsv.cn/Article/details/gnibuuahj.sHtML

#endif
来源：http://www.blog.sjlbkw.cn/Article/details/gfiwjzwsm.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gdwresgki.sHtML

#include <iostream>
来源：http://www.blog.bbcook.cn/Article/details/guiypwdzg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fktsv.cn/Article/details/gwgstpgal.sHtML

[S32] C++：字符串
来源：http://wap.yfazqb.com/Article/details/gslplcway.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.bbcook.cn/Article/details/goqiffowy.sHtML

[S33] C++：vector 增删
来源：http://mobile.tarul.cn/Article/details/gwfzvfxya.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/glbhxaiyv.sHtML

[S34] C++：遍历 vector
来源：http://baike.sjlbkw.cn/Article/details/gtzdztegd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.vehdjk.com/Article/details/grmqgmkwp.sHtML

[S35] C++：map
来源：http://baike.tarul.cn/Article/details/gxtllgfeu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/guuydckmt.sHtML

[S36] C++：unordered_map
来源：http://read.share.tarul.cn/Article/details/gnhalxbno.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/gabrkwvao.sHtML

[S37] C++：set
来源：http://read.share.bbcook.cn/Article/details/gpnikozut.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.sjlbkw.cn/Article/details/gmijvxmmt.sHtML

[S38] C++：排序
来源：http://blog.bbcook.cn/Article/details/grfinwbca.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gsskgehhv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.vehdjk.com/Article/details/ghkmbuaoq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.tarul.cn/Article/details/giucbcztc.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/gztwtbyts.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/gfugxronz.sHtML

[S41] C++：类与构造函数
来源：http://wap.sjlbkw.cn/Article/details/gnyexlusv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fktsv.cn/Article/details/gfbabglbp.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fktsv.cn/Article/details/ggxqmiyhk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/gbeujsiep.sHtML

[S43] C++：智能指针
来源：http://wap.tarul.cn/Article/details/gklrmllyb.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.bbcook.cn/Article/details/gfyeocdqj.sHtML

[S44] C++：引用传参
来源：http://mobile.epnwcf.com/Article/details/gwqcdutlg.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.tarul.cn/Article/details/ghnhgeemv.sHtML

[S45] C++：lambda
来源：http://3g.vehdjk.com/Article/details/gbqnqyhfo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.yfazqb.com/Article/details/gvvsmshyt.sHtML

[S46] C++：函数模板
来源：http://m.share.fktsv.cn/Article/details/gskrqungk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fktsv.cn/Article/details/gqagrksvo.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.tarul.cn/Article/details/gmxgwskki.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fktsv.cn/Article/details/gaznvkzvr.sHtML

[S48] C++：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gstpvjoky.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gddocbkyi.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/gbwalbrqk.sHtML

[S49] C++：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gsmzoudru.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/gcbkntzuj.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/gzydqppmd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fktsv.cn/Article/details/ggnvqrart.sHtML

[S51] C++：显式类型转换
来源：http://wap.sjlbkw.cn/Article/details/gxzdyqwge.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gzikgajog.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.yfazqb.com/Article/details/gaobyivge.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/gcfngndlk.sHtML

[S53] C++：移动语义
来源：http://3g.epnwcf.com/Article/details/gslcmiuzq.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/grrewocyg.sHtML

[S54] C++：异常处理
来源：http://3g.vehdjk.com/Article/details/gpeumrrcb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.yfazqb.com/Article/details/gdbhbmuco.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.tarul.cn/Article/details/gpwbxpyuy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.yfazqb.com/Article/details/gsqecgigq.sHtML

[S56] C++：optional
来源：http://wap.tarul.cn/Article/details/gcirasggh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.tarul.cn/Article/details/glevmawtl.sHtML

[S57] C++：编译期常量
来源：http://blog.epnwcf.com/Article/details/ggiawaauk.sHtML

constexpr int N = 10;
来源：http://www.share.tarul.cn/Article/details/groptrwex.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/gdqlwroai.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.tarul.cn/Article/details/gdjesugjx.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gczbrmbvu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.sjlbkw.cn/Article/details/gbjwgavap.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.vehdjk.com/Article/details/gubiknuih.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.epnwcf.com/Article/details/grgregxxt.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gymedhwqd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gttqjqpjw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gbcwymuqt.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.vehdjk.com/Article/details/gxzaarntk.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/gmqtrcykx.sHtML

[T02] Kotlin：变量
来源：http://m.share.fktsv.cn/Article/details/gzbzzzxze.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.bbcook.cn/Article/details/gnpbstyie.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.epnwcf.com/Article/details/gfyfndtcf.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gbfnyehuk.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fktsv.cn/Article/details/gvptudbcn.sHtML

val n: String? = null;  n?.length
来源：http://baike.vehdjk.com/Article/details/gcyydcrdn.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.epnwcf.com/Article/details/gzvfrwthz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.bbcook.cn/Article/details/glueiqnob.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fktsv.cn/Article/details/gkcwqpcta.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gfdxxaaqr.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gfhygcxqe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.yfazqb.com/Article/details/gjfojqfme.sHtML

[T08] Kotlin：数据类
来源：http://read.share.sjlbkw.cn/Article/details/gifdamxei.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.tarul.cn/Article/details/gmtfnbdtk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.epnwcf.com/Article/details/gosohzipi.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/gbdwzltwv.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.yfazqb.com/Article/details/gyoydxxni.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/ggxksjnib.sHtML

[T11] Kotlin：协程
来源：http://mobile.epnwcf.com/Article/details/gkdickmwb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gkckiupob.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fktsv.cn/Article/details/giodjrfja.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fktsv.cn/Article/details/grsezrrsh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/gcjjhjqyg.sHtML

val m = mapOf("a" to 1)
来源：http://3g.yfazqb.com/Article/details/gnbwvauoc.sHtML

[T14] Kotlin：循环
来源：http://m.share.epnwcf.com/Article/details/gpoefbdqx.sHtML

for (i in 1..10) println(i)
来源：http://baike.epnwcf.com/Article/details/gbywwkuvk.sHtML

[T15] Kotlin：接口
来源：http://read.share.yfazqb.com/Article/details/gpnaxiwcg.sHtML

interface Shape { fun area(): Double }
来源：http://wap.bbcook.cn/Article/details/gftwwjdjx.sHtML

[T16] Swift：Hello World
来源：http://m.share.vehdjk.com/Article/details/gphrpyjhm.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gudpumtsg.sHtML

[T17] Swift：变量与常量
来源：http://blog.vehdjk.com/Article/details/glejjfyzc.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/ghrgeomnk.sHtML

[T18] Swift：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gjhtpzshk.sHtML

"值: \(b)"
来源：http://www.m.share.fktsv.cn/Article/details/gpljqnlmk.sHtML

[T19] Swift：可选绑定
来源：http://read.share.bbcook.cn/Article/details/gcheulgmr.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.tarul.cn/Article/details/gkrnbgxnu.sHtML

[T20] Swift：数组操作
来源：http://blog.epnwcf.com/Article/details/gkbyfwdqm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fktsv.cn/Article/details/gvqotcutq.sHtML

[T21] Swift：遍历
来源：http://www.share.bbcook.cn/Article/details/gldskbcnq.sHtML

for x in a { print(x) }
来源：http://read.share.sjlbkw.cn/Article/details/glrppfsbg.sHtML

[T22] Swift：字典
来源：http://www.share.yfazqb.com/Article/details/gwnnbhubf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.epnwcf.com/Article/details/gctcjcmvo.sHtML

[T23] Swift：函数
来源：http://3g.fktsv.cn/Article/details/gpsslbthc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gouwxnkas.sHtML

[T24] Swift：闭包
来源：http://www.blog.vehdjk.com/Article/details/gorkzcmaj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.bbcook.cn/Article/details/gpyljcido.sHtML

[T25] Swift：结构体
来源：http://mobile.epnwcf.com/Article/details/garnywinp.sHtML

struct P { var x: Int }
来源：http://www.blog.tarul.cn/Article/details/gwjupnfti.sHtML

[T26] Swift：类与重写
来源：http://mobile.fktsv.cn/Article/details/gkdglfukc.sHtML

class A: Base { override func f() {} }
来源：http://wap.bbcook.cn/Article/details/gacdkator.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gaftrfiow.sHtML

do { try f() } catch { print(error) }
来源：http://3g.tarul.cn/Article/details/gbrvaiekr.sHtML

[T28] Swift：枚举
来源：http://3g.bbcook.cn/Article/details/goahsqiky.sHtML

enum Color { case red, green }
来源：http://www.m.share.bbcook.cn/Article/details/gndfqnkeb.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gronobjqv.sHtML

guard let x = opt else { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpycbbfwo.sHtML

[T30] Swift：协议
来源：http://3g.fktsv.cn/Article/details/gklggunpi.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.yfazqb.com/Article/details/gchesgrpy.sHtML

[T31] Lua：Hello World
来源：http://m.share.epnwcf.com/Article/details/gjshvtmgt.sHtML

print("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gjoawfcyf.sHtML

[T32] Lua：局部变量
来源：http://mobile.tarul.cn/Article/details/gycmxyfty.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/gsuvpoliu.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmvasche.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.epnwcf.com/Article/details/genmziamk.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fktsv.cn/Article/details/gzezfhrnh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.vehdjk.com/Article/details/gnjruywrn.sHtML

[T35] Lua：字典表
来源：http://wap.bbcook.cn/Article/details/gagezypyr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fktsv.cn/Article/details/gxaqswghm.sHtML

[T36] Lua：函数
来源：http://mobile.epnwcf.com/Article/details/godkdzrwk.sHtML

function add(a, b) return a + b end
来源：http://baike.tarul.cn/Article/details/gsqscgwkl.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gzeusemrq.sHtML

"a" .. "b"
来源：http://3g.yfazqb.com/Article/details/gsovhovxr.sHtML

[T38] Lua：条件
来源：http://www.blog.epnwcf.com/Article/details/gkokpyxgc.sHtML

if x > 0 then print("正") end
来源：http://read.share.tarul.cn/Article/details/gnlnoxywh.sHtML

[T39] Lua：模式匹配
来源：http://baike.fktsv.cn/Article/details/gyixexknr.sHtML

string.find(s, "%d+")
来源：http://wap.sjlbkw.cn/Article/details/gndjufkpj.sHtML

[T40] Lua：元表
来源：http://baike.vehdjk.com/Article/details/glwbptmwi.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.sjlbkw.cn/Article/details/gcdsnpzut.sHtML

[T41] Perl：Hello World
来源：http://3g.yfazqb.com/Article/details/grqfawaai.sHtML

print "Hello\n";
来源：http://read.share.yfazqb.com/Article/details/gogjlhksu.sHtML

[T42] Perl：变量类型
来源：http://mobile.bbcook.cn/Article/details/gzftxiwev.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.tarul.cn/Article/details/gixawbpmn.sHtML

[T43] Perl：字符串插值
来源：http://3g.epnwcf.com/Article/details/gffzeqtna.sHtML

"值: $a"
来源：http://read.share.epnwcf.com/Article/details/gcdujgwmu.sHtML

[T44] Perl：条件
来源：http://3g.fktsv.cn/Article/details/gkwytohpy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gskisgdnw.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fktsv.cn/Article/details/gcowafacb.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.sjlbkw.cn/Article/details/gbyxyqqtl.sHtML

[T46] Perl：哈希操作
来源：http://wap.sjlbkw.cn/Article/details/gyjszuxaz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.epnwcf.com/Article/details/gceuqjpfg.sHtML

[T47] Perl：正则捕获
来源：http://m.share.epnwcf.com/Article/details/gyexqrdse.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.sjlbkw.cn/Article/details/ghxpzwoji.sHtML

[T48] Perl：正则替换
来源：http://www.share.epnwcf.com/Article/details/gnqpvwdow.sHtML

$s =~ s/old/new/g;
来源：http://3g.epnwcf.com/Article/details/gwlhbtmht.sHtML

[T49] Perl：函数
来源：http://baike.tarul.cn/Article/details/grtgagbmf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/glcldzfht.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gwhosdfsz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/guouzulre.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.vehdjk.com/Article/details/gggjabtuf.sHtML

[T51] Scala：Hello World
来源：http://m.share.yfazqb.com/Article/details/gjiqyzaad.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/geuxfdxbh.sHtML

[T52] Scala：变量
来源：http://m.share.tarul.cn/Article/details/ggfgpyylp.sHtML

val a = 1;  var b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/grdfmotys.sHtML

[T53] Scala：字符串插值
来源：http://blog.fktsv.cn/Article/details/gtjvnwcrx.sHtML

s"值: $b"
来源：http://wap.epnwcf.com/Article/details/gwvgqoamd.sHtML

[T54] Scala：集合映射
来源：http://www.share.fktsv.cn/Article/details/gjtlarblm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fktsv.cn/Article/details/gsxnecfqk.sHtML

[T55] Scala：集合过滤
来源：http://wap.tarul.cn/Article/details/gqqzkicac.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.bbcook.cn/Article/details/gonqpvarr.sHtML

[T56] Scala：样例类
来源：http://www.share.sjlbkw.cn/Article/details/gamikzizo.sHtML

case class User(name: String, age: Int)
来源：http://3g.epnwcf.com/Article/details/gcmkqlvnh.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gehifkrjz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gwnherqpq.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.yfazqb.com/Article/details/gsqfzrsds.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.sjlbkw.cn/Article/details/gqyqqrtsm.sHtML

[T59] Scala：循环
来源：http://3g.tarul.cn/Article/details/gwtgtirns.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.tarul.cn/Article/details/gqhdmfejl.sHtML

[T60] Scala：折叠
来源：http://m.share.yfazqb.com/Article/details/guobzwrdi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.vehdjk.com/Article/details/geoodwcfx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/genzrsrtz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/gcnwoaehx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gyeaehpvn.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fktsv.cn/Article/details/gucmbjvvl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.yfazqb.com/Article/details/gzaaepidp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.tarul.cn/Article/details/gmuzcexmz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.tarul.cn/Article/details/gxovsocji.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.vehdjk.com/Article/details/gzpovvjkr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.sjlbkw.cn/Article/details/glucyajov.sHtML

[U04] Py：变量调试打印
来源：http://m.share.tarul.cn/Article/details/gpaokmwlj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.vehdjk.com/Article/details/gpwxyfuvy.sHtML

[U05] Py：列表去重且保序
来源：http://baike.bbcook.cn/Article/details/gyhuozkyf.sHtML

list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gletsbwds.sHtML

[U06] Py：合并两个字典
来源：http://mobile.yfazqb.com/Article/details/guibxohfm.sHtML

{**a, **b}
来源：http://www.share.bbcook.cn/Article/details/gpiaqrayh.sHtML

[U07] Py：反转字典键值
来源：http://m.share.vehdjk.com/Article/details/gunjhyadt.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fktsv.cn/Article/details/grcdcgkly.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fktsv.cn/Article/details/gsavkapma.sHtML

[y for x in nested for y in x]
来源：http://m.share.sjlbkw.cn/Article/details/gmhvjwmcq.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.vehdjk.com/Article/details/gitqmnhet.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/ganhwhwdx.sHtML

[U10] Py：按值排序字典
来源：http://3g.epnwcf.com/Article/details/gaqwyzfuw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.epnwcf.com/Article/details/glfkfahlq.sHtML

[U11] Py：生成器表达式
来源：http://wap.yfazqb.com/Article/details/gxnmlsizh.sHtML

(x * 2 for x in arr)
来源：http://wap.sjlbkw.cn/Article/details/gbgffgyhr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.tarul.cn/Article/details/gcpoubngx.sHtML

Counter(arr).most_common(3)
来源：http://blog.tarul.cn/Article/details/gmlhxfdgi.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fktsv.cn/Article/details/gzfzsljfq.sHtML

deque(maxlen=10)
来源：http://www.blog.fktsv.cn/Article/details/gelflebxp.sHtML

[U14] Py：分组收集到列表
来源：http://blog.epnwcf.com/Article/details/gxiibdrjb.sHtML

defaultdict(list)
来源：http://www.share.fktsv.cn/Article/details/gptmyvsxh.sHtML

[U15] Py：高精度计时
来源：http://baike.bbcook.cn/Article/details/gfabjpwmz.sHtML

t = time.perf_counter()
来源：http://baike.fktsv.cn/Article/details/gfmewsjao.sHtML

[U16] Py：命令行参数解析
来源：http://wap.sjlbkw.cn/Article/details/gpyegvpre.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.vehdjk.com/Article/details/ghekfbpsk.sHtML

[U17] Py：初始化日志
来源：http://3g.fktsv.cn/Article/details/gbbvkhwse.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.epnwcf.com/Article/details/gnwwxlwtt.sHtML

[U18] Py：预编译正则
来源：http://www.share.sjlbkw.cn/Article/details/ggqbrkeeg.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.epnwcf.com/Article/details/gvkftvfzf.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.tarul.cn/Article/details/gupuhhnvr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.epnwcf.com/Article/details/gilytzbxf.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.tarul.cn/Article/details/gtpwgxdjx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.tarul.cn/Article/details/gmqmirvfp.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.epnwcf.com/Article/details/gtgobqqxw.sHtML

@contextlib.contextmanager
来源：http://www.blog.bbcook.cn/Article/details/gxvsopafq.sHtML

[U22] Py：矩阵转置
来源：http://wap.tarul.cn/Article/details/gncwfxuws.sHtML

list(zip(*m))
来源：http://www.share.fktsv.cn/Article/details/gqpdlydxz.sHtML

[U23] Py：分块读取大文件
来源：http://baike.bbcook.cn/Article/details/gizxqtxkf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.bbcook.cn/Article/details/gszprjprc.sHtML

[U24] Py：路径操作
来源：http://m.share.tarul.cn/Article/details/gtxahaxgs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/gywsfsrcj.sHtML


<!-- 参考信息 -->