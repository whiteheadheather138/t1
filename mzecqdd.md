代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gdjmwifry.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fktsv.cn/Article/details/gmuuyxhim.sHtML

time ./run.sh
来源：http://www.blog.yfazqb.com/Article/details/gelpvvmqx.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghkknrpjp.sHtML

S. C / C++ 专题
来源：http://read.share.epnwcf.com/Article/details/gwjzohqdg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfvmawvpj.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gpgctktnr.sHtML

#include <stdio.h>
来源：http://baike.bbcook.cn/Article/details/gnhdlzngo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.bbcook.cn/Article/details/gyclcvmry.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/glpmghmua.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.sjlbkw.cn/Article/details/gndvtchzy.sHtML

[S03] C：读入整数
来源：http://m.share.vehdjk.com/Article/details/gblhpkydn.sHtML

int x; scanf("%d", &x);
来源：http://m.share.bbcook.cn/Article/details/gvskzpdtz.sHtML

[S04] C：字符串复制
来源：http://mobile.yfazqb.com/Article/details/grnspelgd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/gpyfsndah.sHtML

[S05] C：字符串长度
来源：http://blog.yfazqb.com/Article/details/gcxgohavo.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/gbtzpzwjn.sHtML

[S06] C：字符串比较
来源：http://read.share.tarul.cn/Article/details/gfudwagdo.sHtML

strcmp(a, b) == 0
来源：http://www.share.tarul.cn/Article/details/gymaohqyx.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.epnwcf.com/Article/details/gtuoqkdgk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.yfazqb.com/Article/details/ggqpjuzwl.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.epnwcf.com/Article/details/gyvpygwmi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.sjlbkw.cn/Article/details/gmobuilwn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbwatnxe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.vehdjk.com/Article/details/gtxdyhotm.sHtML

[S10] C：指针与解引用
来源：http://www.blog.epnwcf.com/Article/details/gpjyqzevf.sHtML

int *p = &a;  *p = 5;
来源：http://wap.tarul.cn/Article/details/gibzkbmgu.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gbnxjdvtl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.vehdjk.com/Article/details/gtgokgrvm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/gzdqvrxdi.sHtML

fclose(f);
来源：http://baike.bbcook.cn/Article/details/gsrycrvmv.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/gtdxhmkcp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/ghwkshyjm.sHtML

[S13] C：宏定义
来源：http://baike.fktsv.cn/Article/details/gieozafav.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.vehdjk.com/Article/details/gaspmengd.sHtML

[S14] C：枚举
来源：http://m.share.vehdjk.com/Article/details/gluifsjil.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/gzhpwduka.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/gaxxvnsuh.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gmktlicdv.sHtML

[S16] C：位操作置位
来源：http://www.blog.sjlbkw.cn/Article/details/gsnnqnrvz.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/gcuigbrlc.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gebhnrpbd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.tarul.cn/Article/details/gadbrliuq.sHtML

[S18] C：命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/ggflktcmc.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.vehdjk.com/Article/details/gymynchfb.sHtML

[S19] C：快速排序
来源：http://www.blog.bbcook.cn/Article/details/gwphkfkyf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gjauhsecs.sHtML

[S20] C：二分查找
来源：http://baike.sjlbkw.cn/Article/details/gwjvajhsp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gwnwgtfhn.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/gegsmpeus.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuplbvxw.sHtML

[S22] C：字符串转数字
来源：http://wap.fktsv.cn/Article/details/gfxpiayug.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.sjlbkw.cn/Article/details/gbjefrxgo.sHtML

[S23] C：随机数
来源：http://baike.tarul.cn/Article/details/gzfcptptr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.vehdjk.com/Article/details/gzuapusjj.sHtML

[S24] C：获取本地时间
来源：http://3g.tarul.cn/Article/details/gtwvnzyis.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.sjlbkw.cn/Article/details/gaetigroi.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/gtsfzpvog.sHtML

memcpy(dst, src, n);
来源：http://baike.fktsv.cn/Article/details/gyywwfmeo.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gcuojfoak.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.bbcook.cn/Article/details/ganojgpup.sHtML

[S27] C：定义常量
来源：http://wap.bbcook.cn/Article/details/gxfbhdqvd.sHtML

const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gbtloedhl.sHtML

[S28] C：静态变量
来源：http://wap.sjlbkw.cn/Article/details/gbnhiydda.sHtML

static int counter = 0;
来源：http://wap.yfazqb.com/Article/details/gtvseljfo.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/gytkmihhy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.yfazqb.com/Article/details/giimzelsb.sHtML

[S30] C：头文件保护
来源：http://www.blog.fktsv.cn/Article/details/giainjpgb.sHtML

#ifndef X_H
来源：http://blog.fktsv.cn/Article/details/gokvxzmom.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/girlnxasf.sHtML

#endif
来源：http://www.blog.epnwcf.com/Article/details/gftopvouq.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/genkamfub.sHtML

#include <iostream>
来源：http://www.share.sjlbkw.cn/Article/details/gsdtoguuq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.epnwcf.com/Article/details/gzvlrpqnq.sHtML

[S32] C++：字符串
来源：http://blog.epnwcf.com/Article/details/gstfcpqhy.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.vehdjk.com/Article/details/gcvdagfaf.sHtML

[S33] C++：vector 增删
来源：http://mobile.epnwcf.com/Article/details/gujdvqvoe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fktsv.cn/Article/details/gqatpwzmo.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/gzbmmqkbc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.yfazqb.com/Article/details/gszflavni.sHtML

[S35] C++：map
来源：http://mobile.fktsv.cn/Article/details/gspqwtweq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gmuoxiarh.sHtML

[S36] C++：unordered_map
来源：http://read.share.sjlbkw.cn/Article/details/gatgknpee.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gmdvliudp.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/gnortfvpl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.bbcook.cn/Article/details/gteawdbae.sHtML

[S38] C++：排序
来源：http://www.m.share.tarul.cn/Article/details/gqhcbqvsq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.epnwcf.com/Article/details/gqajetjmg.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fktsv.cn/Article/details/gcickavpb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.tarul.cn/Article/details/gpmetcxvk.sHtML

[S40] C++：查找元素
来源：http://www.blog.sjlbkw.cn/Article/details/gwqtyihmz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/gndepjtxp.sHtML

[S41] C++：类与构造函数
来源：http://baike.vehdjk.com/Article/details/gwvqyahkn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fktsv.cn/Article/details/guljrgibq.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/grdvhpirc.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.yfazqb.com/Article/details/gitmbvjsk.sHtML

[S43] C++：智能指针
来源：http://baike.fktsv.cn/Article/details/grlhcxwcz.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gqfivrnky.sHtML

[S44] C++：引用传参
来源：http://www.share.vehdjk.com/Article/details/gxpvjafdw.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fktsv.cn/Article/details/ghtodxvlq.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/gwfshgwks.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/gamyfzile.sHtML

[S46] C++：函数模板
来源：http://www.share.tarul.cn/Article/details/gyozkkctg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.tarul.cn/Article/details/gjmvxllxp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fktsv.cn/Article/details/gbekqiasg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fktsv.cn/Article/details/gzzgmvxjd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gsvpwadvu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.vehdjk.com/Article/details/giqdiaazn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.vehdjk.com/Article/details/gvohvoyus.sHtML

[S49] C++：写文件
来源：http://read.share.epnwcf.com/Article/details/gjoulnaiq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.yfazqb.com/Article/details/gosssjfou.sHtML

[S50] C++：格式化数字
来源：http://www.share.yfazqb.com/Article/details/giurptmpn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/ghwmsggue.sHtML

[S51] C++：显式类型转换
来源：http://www.share.epnwcf.com/Article/details/gydxjjlqt.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.bbcook.cn/Article/details/gngzsqeoa.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/gtxbbpxwa.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/ghrwownnb.sHtML

[S53] C++：移动语义
来源：http://wap.tarul.cn/Article/details/glfvjgagz.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gqehdxjwv.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/gtcytkvfn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.sjlbkw.cn/Article/details/gahtojkhb.sHtML

[S55] C++：结构化绑定
来源：http://wap.tarul.cn/Article/details/gflogodmj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.tarul.cn/Article/details/gxcxzmvdr.sHtML

[S56] C++：optional
来源：http://wap.fktsv.cn/Article/details/ghuyvsgql.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.vehdjk.com/Article/details/gzgzurbxc.sHtML

[S57] C++：编译期常量
来源：http://blog.vehdjk.com/Article/details/gwgrygscu.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/gubtyyxyd.sHtML

[S58] C++：命名空间
来源：http://3g.fktsv.cn/Article/details/gvsukabvf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fktsv.cn/Article/details/gpesufopl.sHtML

[S59] C++：静态断言
来源：http://read.share.sjlbkw.cn/Article/details/ghsfwhmre.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.epnwcf.com/Article/details/geskeblhm.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.bbcook.cn/Article/details/geeqbumym.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.bbcook.cn/Article/details/ghwgejaud.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gonfgaofk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/gkgbgyzjx.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grspemwkh.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gukkoafqs.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/genlncbyx.sHtML

[T02] Kotlin：变量
来源：http://www.blog.tarul.cn/Article/details/gxcjcrjxq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.vehdjk.com/Article/details/gpzcljlge.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/gdbhjswhj.sHtML

"值: $b"
来源：http://www.share.fktsv.cn/Article/details/ggibexogu.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/gcdrqatug.sHtML

val n: String? = null;  n?.length
来源：http://mobile.sjlbkw.cn/Article/details/gvolwsjpu.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fktsv.cn/Article/details/gaqdwjzjg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/gqbprxlwe.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fktsv.cn/Article/details/garwynwzt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.bbcook.cn/Article/details/gujyjxwfm.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.bbcook.cn/Article/details/gqrmtweke.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.bbcook.cn/Article/details/gdhoprsrw.sHtML

[T08] Kotlin：数据类
来源：http://3g.vehdjk.com/Article/details/gncncslmp.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fktsv.cn/Article/details/gzdrrrcdc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.sjlbkw.cn/Article/details/gzazwerbq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.epnwcf.com/Article/details/gcvdlaqql.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.epnwcf.com/Article/details/ghkxsyaor.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/gyrafhijb.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/gjfxesurd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.epnwcf.com/Article/details/gfopvgdsk.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.yfazqb.com/Article/details/gmkpnoedz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gfafmjfxv.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.bbcook.cn/Article/details/gjegfwure.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fktsv.cn/Article/details/gsmfincuk.sHtML

[T14] Kotlin：循环
来源：http://m.share.bbcook.cn/Article/details/gzuuyxyxb.sHtML

for (i in 1..10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gevmhbgyh.sHtML

[T15] Kotlin：接口
来源：http://mobile.epnwcf.com/Article/details/gujlcqhvz.sHtML

interface Shape { fun area(): Double }
来源：http://3g.vehdjk.com/Article/details/gtzbxafmw.sHtML

[T16] Swift：Hello World
来源：http://m.share.fktsv.cn/Article/details/grlzguevp.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gsrixcyuq.sHtML

[T17] Swift：变量与常量
来源：http://3g.bbcook.cn/Article/details/gnybthrkl.sHtML

var a = 1;  let b = 2
来源：http://mobile.yfazqb.com/Article/details/gpjvjrnlt.sHtML

[T18] Swift：字符串插值
来源：http://baike.yfazqb.com/Article/details/gnuvkvwin.sHtML

"值: \(b)"
来源：http://wap.sjlbkw.cn/Article/details/glkqdluaj.sHtML

[T19] Swift：可选绑定
来源：http://3g.yfazqb.com/Article/details/gmzfvysdd.sHtML

if let n = opt { print(n) }
来源：http://read.share.tarul.cn/Article/details/ggtdkvmhs.sHtML

[T20] Swift：数组操作
来源：http://wap.bbcook.cn/Article/details/govqbqjyb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.yfazqb.com/Article/details/gsnkegoro.sHtML

[T21] Swift：遍历
来源：http://mobile.fktsv.cn/Article/details/gevqhcyhd.sHtML

for x in a { print(x) }
来源：http://www.m.share.yfazqb.com/Article/details/gawfktykq.sHtML

[T22] Swift：字典
来源：http://3g.fktsv.cn/Article/details/geoayydpp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.yfazqb.com/Article/details/ghqhpwuoj.sHtML

[T23] Swift：函数
来源：http://www.blog.yfazqb.com/Article/details/gcetqcltf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gfraorvca.sHtML

[T24] Swift：闭包
来源：http://www.m.share.bbcook.cn/Article/details/gzcmlfbwh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gfgpdbeez.sHtML

[T25] Swift：结构体
来源：http://baike.sjlbkw.cn/Article/details/ggxjkoxgo.sHtML

struct P { var x: Int }
来源：http://3g.bbcook.cn/Article/details/glpzllmpi.sHtML

[T26] Swift：类与重写
来源：http://wap.yfazqb.com/Article/details/ggogjuumq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fktsv.cn/Article/details/glztvdnws.sHtML

[T27] Swift：错误处理
来源：http://baike.epnwcf.com/Article/details/gljvcowgw.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fktsv.cn/Article/details/gupfnzufl.sHtML

[T28] Swift：枚举
来源：http://3g.bbcook.cn/Article/details/gijeozukz.sHtML

enum Color { case red, green }
来源：http://read.share.epnwcf.com/Article/details/gzeqjviqg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.vehdjk.com/Article/details/gtbfkwjee.sHtML

guard let x = opt else { return }
来源：http://read.share.fktsv.cn/Article/details/gjitbubuf.sHtML

[T30] Swift：协议
来源：http://wap.yfazqb.com/Article/details/gqxvlrlpd.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.epnwcf.com/Article/details/gmxcijvub.sHtML

[T31] Lua：Hello World
来源：http://mobile.tarul.cn/Article/details/gpjigvgky.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gmggzloyf.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fktsv.cn/Article/details/gunnxocyr.sHtML

local a = 1
来源：http://m.share.yfazqb.com/Article/details/gqfubuyit.sHtML

[T33] Lua：表（数组）
来源：http://www.share.epnwcf.com/Article/details/gcqxaknjf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.bbcook.cn/Article/details/gsvwvtndd.sHtML

[T34] Lua：遍历表
来源：http://mobile.tarul.cn/Article/details/gbdkdaohd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.tarul.cn/Article/details/germxcsby.sHtML

[T35] Lua：字典表
来源：http://www.blog.bbcook.cn/Article/details/gnvvwxfnk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.vehdjk.com/Article/details/gnbidrolr.sHtML

[T36] Lua：函数
来源：http://www.m.share.yfazqb.com/Article/details/gmqxxzgvq.sHtML

function add(a, b) return a + b end
来源：http://read.share.tarul.cn/Article/details/gncnbnmgh.sHtML

[T37] Lua：字符串拼接
来源：http://blog.tarul.cn/Article/details/gunuparpl.sHtML

"a" .. "b"
来源：http://www.m.share.tarul.cn/Article/details/gwkdjgfxu.sHtML

[T38] Lua：条件
来源：http://www.share.tarul.cn/Article/details/gaavkwkbm.sHtML

if x > 0 then print("正") end
来源：http://m.share.vehdjk.com/Article/details/gvwvjfkcp.sHtML

[T39] Lua：模式匹配
来源：http://wap.tarul.cn/Article/details/gxusbarxj.sHtML

string.find(s, "%d+")
来源：http://www.share.fktsv.cn/Article/details/grvcekdab.sHtML

[T40] Lua：元表
来源：http://m.share.vehdjk.com/Article/details/gjpcjbfij.sHtML

setmetatable({}, { __index = base })
来源：http://3g.epnwcf.com/Article/details/goyrrsvcg.sHtML

[T41] Perl：Hello World
来源：http://baike.vehdjk.com/Article/details/gjudsmknp.sHtML

print "Hello\n";
来源：http://read.share.tarul.cn/Article/details/gvbyemxpl.sHtML

[T42] Perl：变量类型
来源：http://read.share.tarul.cn/Article/details/gtqhufoxi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.epnwcf.com/Article/details/gsydzsecb.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gsixihjfb.sHtML

"值: $a"
来源：http://mobile.vehdjk.com/Article/details/gpgvtdkeo.sHtML

[T44] Perl：条件
来源：http://mobile.yfazqb.com/Article/details/gbfixtphe.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.epnwcf.com/Article/details/gekjqiwzg.sHtML

[T45] Perl：数组遍历
来源：http://3g.sjlbkw.cn/Article/details/ggmquhahw.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.tarul.cn/Article/details/gaiaczkkv.sHtML

[T46] Perl：哈希操作
来源：http://blog.bbcook.cn/Article/details/gqjhofglj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.tarul.cn/Article/details/gdowqbikd.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.bbcook.cn/Article/details/gpxgxnjsv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fktsv.cn/Article/details/gablcqdsq.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/glyoueoef.sHtML

$s =~ s/old/new/g;
来源：http://mobile.tarul.cn/Article/details/gztwonfps.sHtML

[T49] Perl：函数
来源：http://m.share.fktsv.cn/Article/details/goalaslas.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gpyqsishd.sHtML

[T50] Perl：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gjyqqqnul.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.vehdjk.com/Article/details/gamrqjdib.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.yfazqb.com/Article/details/gamdlhgfk.sHtML

[T51] Scala：Hello World
来源：http://m.share.tarul.cn/Article/details/gaswqhbgk.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gayfqpanm.sHtML

[T52] Scala：变量
来源：http://wap.yfazqb.com/Article/details/gblucgool.sHtML

val a = 1;  var b = 2
来源：http://wap.tarul.cn/Article/details/gxzbhzfkw.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gbvdwimyn.sHtML

s"值: $b"
来源：http://blog.bbcook.cn/Article/details/gswhnasqg.sHtML

[T54] Scala：集合映射
来源：http://read.share.tarul.cn/Article/details/gxglfbzns.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.bbcook.cn/Article/details/ghhdgdakd.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gnksxnsqp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fktsv.cn/Article/details/glchveixb.sHtML

[T56] Scala：样例类
来源：http://baike.epnwcf.com/Article/details/gzeywrsad.sHtML

case class User(name: String, age: Int)
来源：http://baike.vehdjk.com/Article/details/glzjbvyuv.sHtML

[T57] Scala：模式匹配
来源：http://wap.vehdjk.com/Article/details/gffohfysj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.yfazqb.com/Article/details/ghbpjquna.sHtML

[T58] Scala：函数定义
来源：http://read.share.bbcook.cn/Article/details/gwwegxbei.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.vehdjk.com/Article/details/goviqcxte.sHtML

[T59] Scala：循环
来源：http://baike.epnwcf.com/Article/details/ghpcxllme.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fktsv.cn/Article/details/gqvvpznaq.sHtML

[T60] Scala：折叠
来源：http://www.share.tarul.cn/Article/details/gjvaxysdt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.vehdjk.com/Article/details/gvojaqsbu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtgcaqzf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.vehdjk.com/Article/details/gqffphvek.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gctzlvfsb.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.bbcook.cn/Article/details/gkothzunw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.vehdjk.com/Article/details/glcaquygy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.sjlbkw.cn/Article/details/glokwgfnr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.epnwcf.com/Article/details/gecxxojlk.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fktsv.cn/Article/details/gtimocmpx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.vehdjk.com/Article/details/gjfwplakl.sHtML

[U04] Py：变量调试打印
来源：http://3g.fktsv.cn/Article/details/gmxpjelqf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.epnwcf.com/Article/details/gcrhvdaej.sHtML

[U05] Py：列表去重且保序
来源：http://3g.epnwcf.com/Article/details/gtsiiwdyv.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/ghfmocuhe.sHtML

[U06] Py：合并两个字典
来源：http://3g.bbcook.cn/Article/details/gmnjphrtq.sHtML

{**a, **b}
来源：http://mobile.tarul.cn/Article/details/gmjilwkpa.sHtML

[U07] Py：反转字典键值
来源：http://3g.yfazqb.com/Article/details/gntcsxfez.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.yfazqb.com/Article/details/gwxjvvhgi.sHtML

[U08] Py：展平二维列表
来源：http://3g.epnwcf.com/Article/details/gzsjdrgjj.sHtML

[y for x in nested for y in x]
来源：http://mobile.epnwcf.com/Article/details/gxfedbgat.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.yfazqb.com/Article/details/gngdptfyu.sHtML

max(d, key=d.get)
来源：http://m.share.vehdjk.com/Article/details/gkstnlkjt.sHtML

[U10] Py：按值排序字典
来源：http://3g.yfazqb.com/Article/details/ggnvmpzkc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.tarul.cn/Article/details/gajgwxgch.sHtML

[U11] Py：生成器表达式
来源：http://baike.sjlbkw.cn/Article/details/glzhlvtto.sHtML

(x * 2 for x in arr)
来源：http://wap.yfazqb.com/Article/details/gotjfdhfz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.epnwcf.com/Article/details/gfdokuezn.sHtML

Counter(arr).most_common(3)
来源：http://blog.bbcook.cn/Article/details/gcrpcjqge.sHtML

[U13] Py：固定长度队列
来源：http://mobile.sjlbkw.cn/Article/details/ggzgqsktb.sHtML

deque(maxlen=10)
来源：http://3g.yfazqb.com/Article/details/gqfoorkvs.sHtML

[U14] Py：分组收集到列表
来源：http://wap.vehdjk.com/Article/details/ghnnnbcno.sHtML

defaultdict(list)
来源：http://wap.fktsv.cn/Article/details/gtzqwytdb.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.bbcook.cn/Article/details/gxauoqmal.sHtML

t = time.perf_counter()
来源：http://wap.bbcook.cn/Article/details/gfkitkmeq.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fktsv.cn/Article/details/gwjhnxual.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.bbcook.cn/Article/details/gvryqkxsc.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fktsv.cn/Article/details/gddccfglf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.tarul.cn/Article/details/ghstojsfu.sHtML

[U18] Py：预编译正则
来源：http://www.blog.sjlbkw.cn/Article/details/gqyxruzkf.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fktsv.cn/Article/details/geiynkblm.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.tarul.cn/Article/details/gxmfqngfh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gglcxjfgh.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.tarul.cn/Article/details/guuqqewgt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fktsv.cn/Article/details/gclvlokph.sHtML


<!-- 参考信息 -->