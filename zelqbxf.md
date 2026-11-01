代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.epnwcf.com/Article/details/gauulsvxn.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gmgqsrpvd.sHtML

time ./run.sh
来源：http://m.share.bbcook.cn/Article/details/gegzhuyfc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggrnaxynp.sHtML

S. C / C++ 专题
来源：http://read.share.yfazqb.com/Article/details/gbbkanlxa.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjzncedgr.sHtML

[S01] C：Hello World
来源：http://read.share.epnwcf.com/Article/details/ghjyzqtlm.sHtML

#include <stdio.h>
来源：http://wap.bbcook.cn/Article/details/gdxjzylkb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.bbcook.cn/Article/details/gbvfwwkem.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.bbcook.cn/Article/details/guojkwdkh.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.tarul.cn/Article/details/gczrrgjkj.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/gqmgxxwkx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.tarul.cn/Article/details/gvmlqctqp.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/ggldqypkb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.bbcook.cn/Article/details/gamcorvdu.sHtML

[S05] C：字符串长度
来源：http://3g.tarul.cn/Article/details/ghjabqkok.sHtML

strlen(s)
来源：http://wap.tarul.cn/Article/details/gufqleyok.sHtML

[S06] C：字符串比较
来源：http://read.share.tarul.cn/Article/details/gglqhfdbo.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.bbcook.cn/Article/details/gelhfcapv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.sjlbkw.cn/Article/details/gqiuluxan.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.epnwcf.com/Article/details/gjmbagukr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/gtinjbzzk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/ghmtzkkeu.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.tarul.cn/Article/details/gkgwnhuzk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gtpdqpcfz.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fktsv.cn/Article/details/gjdtdqfdw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.vehdjk.com/Article/details/gfcswqsar.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gduocoevp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/gndqqxemi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/gbxhyswcu.sHtML

fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/ggwvuzatk.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/ghjonybsd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gqujcsmfv.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gzioquvkt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.vehdjk.com/Article/details/gjvnachuf.sHtML

[S14] C：枚举
来源：http://mobile.tarul.cn/Article/details/gqoautyub.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.bbcook.cn/Article/details/gtabpquwk.sHtML

[S15] C：类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gzhpfirpt.sHtML

(double) a / b
来源：http://blog.yfazqb.com/Article/details/gyfmzjaqb.sHtML

[S16] C：位操作置位
来源：http://www.share.fktsv.cn/Article/details/gboolgiwt.sHtML

x |= (1 << 3);
来源：http://mobile.yfazqb.com/Article/details/gqyesyryi.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/giwhniszk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.vehdjk.com/Article/details/gupnsguhi.sHtML

[S18] C：命令行参数
来源：http://m.share.fktsv.cn/Article/details/grqkyfcit.sHtML

int main(int argc, char **argv)
来源：http://wap.vehdjk.com/Article/details/gjyecbybs.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/gluphavvg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gipgxqsdq.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/ghoiefjvu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gaqenrvuc.sHtML

[S21] C：字符类别判断
来源：http://www.share.bbcook.cn/Article/details/gnvbjzief.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.sjlbkw.cn/Article/details/gudxsrwis.sHtML

[S22] C：字符串转数字
来源：http://www.blog.tarul.cn/Article/details/gwfrqales.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/gzntxbjvw.sHtML

[S23] C：随机数
来源：http://3g.fktsv.cn/Article/details/gxwbsazhf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.epnwcf.com/Article/details/gmtxvgvht.sHtML

[S24] C：获取本地时间
来源：http://blog.fktsv.cn/Article/details/gfmxywgho.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.yfazqb.com/Article/details/gilefhfyn.sHtML

[S25] C：内存拷贝
来源：http://www.share.yfazqb.com/Article/details/gqdcrirvq.sHtML

memcpy(dst, src, n);
来源：http://read.share.yfazqb.com/Article/details/gixqbaqpm.sHtML

[S26] C：内存清零
来源：http://www.m.share.bbcook.cn/Article/details/guxhejszy.sHtML

memset(a, 0, sizeof a);
来源：http://wap.epnwcf.com/Article/details/gamclpjmb.sHtML

[S27] C：定义常量
来源：http://www.share.bbcook.cn/Article/details/ghnrdwdwx.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gbvcqczvd.sHtML

[S28] C：静态变量
来源：http://m.share.epnwcf.com/Article/details/giwujceyy.sHtML

static int counter = 0;
来源：http://www.m.share.vehdjk.com/Article/details/ganrajamf.sHtML

[S29] C：变参函数
来源：http://wap.yfazqb.com/Article/details/gbxrwyfov.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.tarul.cn/Article/details/gjgqpwwsq.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/gsgfsxeiu.sHtML

#ifndef X_H
来源：http://baike.epnwcf.com/Article/details/gbnirozqo.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/ggjlmufxl.sHtML

#endif
来源：http://baike.yfazqb.com/Article/details/gfslbhjre.sHtML

[S31] C++：Hello World
来源：http://mobile.bbcook.cn/Article/details/gbowbvyfi.sHtML

#include <iostream>
来源：http://www.m.share.bbcook.cn/Article/details/gettrazib.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.epnwcf.com/Article/details/geqvqscjt.sHtML

[S32] C++：字符串
来源：http://www.blog.yfazqb.com/Article/details/gosovmcye.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.tarul.cn/Article/details/gtihvdwvv.sHtML

[S33] C++：vector 增删
来源：http://www.blog.bbcook.cn/Article/details/gktsqumxj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.bbcook.cn/Article/details/goprdkzxa.sHtML

[S34] C++：遍历 vector
来源：http://baike.fktsv.cn/Article/details/geaynnmdp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/gggsbxtdq.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gsgqpiwfz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gwokkvkob.sHtML

[S36] C++：unordered_map
来源：http://wap.epnwcf.com/Article/details/giwkgufiy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/glcsmodnv.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/gcfbyhdia.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.yfazqb.com/Article/details/gfdzcankb.sHtML

[S38] C++：排序
来源：http://blog.fktsv.cn/Article/details/gwuuukqvn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gdirxpasz.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fktsv.cn/Article/details/gevwvhuej.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.yfazqb.com/Article/details/gzixozmac.sHtML

[S40] C++：查找元素
来源：http://www.share.vehdjk.com/Article/details/gymoeqlqm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/gzofqospk.sHtML

[S41] C++：类与构造函数
来源：http://wap.yfazqb.com/Article/details/gaztdnjnq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.epnwcf.com/Article/details/gjyqrqaet.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.yfazqb.com/Article/details/gitdpvpjn.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.yfazqb.com/Article/details/gocafrzmz.sHtML

[S43] C++：智能指针
来源：http://www.blog.tarul.cn/Article/details/gkjlnoaoq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gojniuael.sHtML

[S44] C++：引用传参
来源：http://wap.yfazqb.com/Article/details/gxghsyuta.sHtML

void inc(int &x) { ++x; }
来源：http://baike.sjlbkw.cn/Article/details/gztivmzfo.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/gfgpaomxw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.epnwcf.com/Article/details/gondzbxfd.sHtML

[S46] C++：函数模板
来源：http://m.share.yfazqb.com/Article/details/glbamqscb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.sjlbkw.cn/Article/details/gtrfactxe.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.sjlbkw.cn/Article/details/gknolfigw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.epnwcf.com/Article/details/gotnuqpqp.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gqssxlyos.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fktsv.cn/Article/details/gnaftbalz.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.bbcook.cn/Article/details/gjmdlphjk.sHtML

[S49] C++：写文件
来源：http://wap.epnwcf.com/Article/details/gpkgzbfxt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/gjcpctphv.sHtML

[S50] C++：格式化数字
来源：http://read.share.vehdjk.com/Article/details/gbdhycpfc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gginwqlry.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.tarul.cn/Article/details/ghdgznfmb.sHtML

static_cast<double>(a) / b
来源：http://m.share.bbcook.cn/Article/details/gdimcttwl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fktsv.cn/Article/details/gihtpxsih.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gzaizkavs.sHtML

[S53] C++：移动语义
来源：http://www.m.share.vehdjk.com/Article/details/gxgbudeby.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gkgllhyfg.sHtML

[S54] C++：异常处理
来源：http://www.m.share.yfazqb.com/Article/details/gllphbfad.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.bbcook.cn/Article/details/ggjcnohxr.sHtML

[S55] C++：结构化绑定
来源：http://blog.vehdjk.com/Article/details/gmoegrqyo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fktsv.cn/Article/details/gsyvwhqsb.sHtML

[S56] C++：optional
来源：http://wap.tarul.cn/Article/details/gcarxulmc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.yfazqb.com/Article/details/gxseddavg.sHtML

[S57] C++：编译期常量
来源：http://baike.yfazqb.com/Article/details/gxjtmoxsn.sHtML

constexpr int N = 10;
来源：http://read.share.fktsv.cn/Article/details/gkvpnulkp.sHtML

[S58] C++：命名空间
来源：http://www.share.bbcook.cn/Article/details/geflvqhhk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fktsv.cn/Article/details/giwzgfcib.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/gnckcaxwr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.bbcook.cn/Article/details/gtixckkwa.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.vehdjk.com/Article/details/gomrlopxm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gsvirtmvn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbcakfibp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/ggvuxzivz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gpqgszsjv.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fktsv.cn/Article/details/gqxkmeljm.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gnvpfwzyx.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/gppmqffpi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fktsv.cn/Article/details/gpoijxqrr.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.vehdjk.com/Article/details/gsbnvppis.sHtML

"值: $b"
来源：http://blog.tarul.cn/Article/details/gpqddweou.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwaeihmv.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/gudtsvoqq.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gzazosbrx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.epnwcf.com/Article/details/guogafval.sHtML

[T06] Kotlin：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gsdqpvebq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gzalvsivs.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.bbcook.cn/Article/details/gtxqegwkd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.epnwcf.com/Article/details/gbqbbmecb.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/grualamqo.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.bbcook.cn/Article/details/gqjcrffgz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fktsv.cn/Article/details/gfakwvrbi.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fktsv.cn/Article/details/gqumltecc.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.yfazqb.com/Article/details/gsptdckwd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/gibejvizs.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.vehdjk.com/Article/details/giddpwpld.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.epnwcf.com/Article/details/gthevcjaa.sHtML

[T12] Kotlin：解构声明
来源：http://wap.sjlbkw.cn/Article/details/gehijvcag.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/guqjllydn.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.sjlbkw.cn/Article/details/gjvwcnxqm.sHtML

val m = mapOf("a" to 1)
来源：http://blog.bbcook.cn/Article/details/gkjkjuloj.sHtML

[T14] Kotlin：循环
来源：http://blog.vehdjk.com/Article/details/gvxasipsv.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gmiomyeix.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.sjlbkw.cn/Article/details/gadwnsqtx.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.bbcook.cn/Article/details/gxxhzdumf.sHtML

[T16] Swift：Hello World
来源：http://m.share.fktsv.cn/Article/details/gibqdruhr.sHtML

print("Hello")
来源：http://www.blog.tarul.cn/Article/details/gsatsksye.sHtML

[T17] Swift：变量与常量
来源：http://mobile.yfazqb.com/Article/details/gynbscduv.sHtML

var a = 1;  let b = 2
来源：http://m.share.bbcook.cn/Article/details/gnykfdbaq.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gfogyyofn.sHtML

"值: \(b)"
来源：http://www.blog.epnwcf.com/Article/details/gipltvowh.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.sjlbkw.cn/Article/details/gmxmfpmjw.sHtML

if let n = opt { print(n) }
来源：http://www.blog.epnwcf.com/Article/details/gyogjnkhw.sHtML

[T20] Swift：数组操作
来源：http://blog.epnwcf.com/Article/details/gwgebiajt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.sjlbkw.cn/Article/details/gceaszjct.sHtML

[T21] Swift：遍历
来源：http://m.share.bbcook.cn/Article/details/goyqgwsdf.sHtML

for x in a { print(x) }
来源：http://www.m.share.tarul.cn/Article/details/gbaemcnwo.sHtML

[T22] Swift：字典
来源：http://baike.fktsv.cn/Article/details/gupnvirkl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/geddningj.sHtML

[T23] Swift：函数
来源：http://wap.fktsv.cn/Article/details/gkulbotkv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.bbcook.cn/Article/details/geqznyyeg.sHtML

[T24] Swift：闭包
来源：http://wap.vehdjk.com/Article/details/gbxqvlcpc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.tarul.cn/Article/details/gewrgnnun.sHtML

[T25] Swift：结构体
来源：http://www.blog.sjlbkw.cn/Article/details/gqocrcaxo.sHtML

struct P { var x: Int }
来源：http://read.share.bbcook.cn/Article/details/gnaepgvcj.sHtML

[T26] Swift：类与重写
来源：http://m.share.fktsv.cn/Article/details/gmdqamfue.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fktsv.cn/Article/details/gluknvusn.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fktsv.cn/Article/details/gdothoryh.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.tarul.cn/Article/details/gkssyzjmc.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gpafebwsp.sHtML

enum Color { case red, green }
来源：http://m.share.fktsv.cn/Article/details/gumiqgors.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.tarul.cn/Article/details/ggxbgyiks.sHtML

guard let x = opt else { return }
来源：http://wap.epnwcf.com/Article/details/gmxcsxqqg.sHtML

[T30] Swift：协议
来源：http://baike.vehdjk.com/Article/details/grzaicpku.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.bbcook.cn/Article/details/gfnqzhtgy.sHtML

[T31] Lua：Hello World
来源：http://mobile.vehdjk.com/Article/details/garipacty.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/graxuzdvz.sHtML

[T32] Lua：局部变量
来源：http://mobile.sjlbkw.cn/Article/details/gkhumwzod.sHtML

local a = 1
来源：http://www.blog.epnwcf.com/Article/details/gkgdrsidb.sHtML

[T33] Lua：表（数组）
来源：http://3g.sjlbkw.cn/Article/details/gjflrncyr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.vehdjk.com/Article/details/godcwgylb.sHtML

[T34] Lua：遍历表
来源：http://blog.bbcook.cn/Article/details/gfmhnfhun.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.epnwcf.com/Article/details/ggmtukqtc.sHtML

[T35] Lua：字典表
来源：http://baike.vehdjk.com/Article/details/grynkkqxp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.yfazqb.com/Article/details/gmqqzjfbg.sHtML

[T36] Lua：函数
来源：http://www.share.tarul.cn/Article/details/ggbegqqvj.sHtML

function add(a, b) return a + b end
来源：http://mobile.epnwcf.com/Article/details/gvoqrbcus.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gazxzxlye.sHtML

"a" .. "b"
来源：http://mobile.yfazqb.com/Article/details/gurxwtbze.sHtML

[T38] Lua：条件
来源：http://read.share.bbcook.cn/Article/details/gxumxgwur.sHtML

if x > 0 then print("正") end
来源：http://wap.vehdjk.com/Article/details/ghjbsnvwy.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gqrivrebg.sHtML

string.find(s, "%d+")
来源：http://read.share.sjlbkw.cn/Article/details/gunumejvi.sHtML

[T40] Lua：元表
来源：http://www.share.fktsv.cn/Article/details/gjmgsfgap.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.epnwcf.com/Article/details/gsjssqjir.sHtML

[T41] Perl：Hello World
来源：http://baike.epnwcf.com/Article/details/ggkfpsjti.sHtML

print "Hello\n";
来源：http://www.share.epnwcf.com/Article/details/guxdoomln.sHtML

[T42] Perl：变量类型
来源：http://baike.fktsv.cn/Article/details/gzxpkxdxc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.yfazqb.com/Article/details/gztooznfw.sHtML

[T43] Perl：字符串插值
来源：http://baike.epnwcf.com/Article/details/gzvjjltdp.sHtML

"值: $a"
来源：http://3g.fktsv.cn/Article/details/grqzgmaig.sHtML

[T44] Perl：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcqdmzdr.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.vehdjk.com/Article/details/gonfhdhha.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.vehdjk.com/Article/details/gkdvedkld.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.tarul.cn/Article/details/gpzfcmrxh.sHtML

[T46] Perl：哈希操作
来源：http://m.share.bbcook.cn/Article/details/glngkrvps.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.tarul.cn/Article/details/gqfgiteed.sHtML

[T47] Perl：正则捕获
来源：http://mobile.tarul.cn/Article/details/gvipqwsdy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.yfazqb.com/Article/details/guiyqkmue.sHtML

[T48] Perl：正则替换
来源：http://m.share.yfazqb.com/Article/details/gfpdqhrxc.sHtML

$s =~ s/old/new/g;
来源：http://baike.epnwcf.com/Article/details/gjobquoat.sHtML

[T49] Perl：函数
来源：http://3g.epnwcf.com/Article/details/gsjxqaghl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gvuohvavo.sHtML

[T50] Perl：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gzxognnkn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.bbcook.cn/Article/details/gktgnufqz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.epnwcf.com/Article/details/gfbxyfvuz.sHtML

[T51] Scala：Hello World
来源：http://www.share.epnwcf.com/Article/details/gfrkqubrh.sHtML

println("Hello")
来源：http://wap.fktsv.cn/Article/details/gqctaqipz.sHtML

[T52] Scala：变量
来源：http://baike.bbcook.cn/Article/details/gioyvnjlw.sHtML

val a = 1;  var b = 2
来源：http://mobile.fktsv.cn/Article/details/gprzfenrj.sHtML

[T53] Scala：字符串插值
来源：http://baike.yfazqb.com/Article/details/gdgypacao.sHtML

s"值: $b"
来源：http://read.share.tarul.cn/Article/details/ggfjdcauq.sHtML

[T54] Scala：集合映射
来源：http://m.share.fktsv.cn/Article/details/gkxhianai.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.yfazqb.com/Article/details/guwfiyjln.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.tarul.cn/Article/details/gvmsebmij.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.vehdjk.com/Article/details/giajrijnj.sHtML

[T56] Scala：样例类
来源：http://wap.epnwcf.com/Article/details/giurcaquq.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gzquzqyom.sHtML

[T57] Scala：模式匹配
来源：http://mobile.yfazqb.com/Article/details/gklgkjczm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/gyqfvysyu.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.epnwcf.com/Article/details/gagldjvtx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.bbcook.cn/Article/details/gefsjqsgu.sHtML

[T59] Scala：循环
来源：http://www.m.share.yfazqb.com/Article/details/gehryspuc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/ghvcvusmd.sHtML

[T60] Scala：折叠
来源：http://www.blog.bbcook.cn/Article/details/gilfspfnd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/gpphrbdwj.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmsdxezqx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.epnwcf.com/Article/details/gybkufkoh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gytywqfdt.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.vehdjk.com/Article/details/gebsiqmoe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fktsv.cn/Article/details/ggfddzshw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.epnwcf.com/Article/details/gfeblwbbk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.vehdjk.com/Article/details/gjackinku.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.sjlbkw.cn/Article/details/grwdefrkf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.sjlbkw.cn/Article/details/ggmadnmzr.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.epnwcf.com/Article/details/gtczzpgim.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fktsv.cn/Article/details/gvgglzpev.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.epnwcf.com/Article/details/gltxurbsj.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/ggoycjzpj.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.bbcook.cn/Article/details/guajcqnzz.sHtML

{**a, **b}
来源：http://mobile.epnwcf.com/Article/details/gzjypqyav.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/gcsjglrzc.sHtML

{v: k for k, v in d.items()}
来源：http://wap.tarul.cn/Article/details/gghiuvppf.sHtML

[U08] Py：展平二维列表
来源：http://3g.bbcook.cn/Article/details/gazxbhaec.sHtML

[y for x in nested for y in x]
来源：http://www.blog.tarul.cn/Article/details/gfdpoirkt.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.epnwcf.com/Article/details/gsacgkloa.sHtML

max(d, key=d.get)
来源：http://m.share.tarul.cn/Article/details/gzhcobeag.sHtML

[U10] Py：按值排序字典
来源：http://read.share.yfazqb.com/Article/details/gvuanecrz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.vehdjk.com/Article/details/gmqfbebuc.sHtML

[U11] Py：生成器表达式
来源：http://wap.fktsv.cn/Article/details/gihydvjwd.sHtML

(x * 2 for x in arr)
来源：http://www.share.yfazqb.com/Article/details/gehucyxvt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.tarul.cn/Article/details/gvlhniung.sHtML

Counter(arr).most_common(3)
来源：http://3g.epnwcf.com/Article/details/gkjgukfdb.sHtML

[U13] Py：固定长度队列
来源：http://blog.vehdjk.com/Article/details/guvfbcoud.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/gngdkiblv.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.tarul.cn/Article/details/gahhdxqho.sHtML

defaultdict(list)
来源：http://blog.tarul.cn/Article/details/ggosrwoyl.sHtML

[U15] Py：高精度计时
来源：http://mobile.fktsv.cn/Article/details/gfebybgkc.sHtML

t = time.perf_counter()
来源：http://wap.tarul.cn/Article/details/gvssfiebv.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.yfazqb.com/Article/details/gsenyifri.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.tarul.cn/Article/details/gjbqsxlje.sHtML

[U17] Py：初始化日志
来源：http://www.blog.sjlbkw.cn/Article/details/goxizzesb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.vehdjk.com/Article/details/gisaljfha.sHtML

[U18] Py：预编译正则
来源：http://www.share.fktsv.cn/Article/details/gevshtfyc.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.vehdjk.com/Article/details/gbkfdcnpe.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.epnwcf.com/Article/details/gvsckuonb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.bbcook.cn/Article/details/gtnsgejkx.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.bbcook.cn/Article/details/gzupzltfq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.yfazqb.com/Article/details/ggcqrbmmm.sHtML


<!-- 参考信息 -->