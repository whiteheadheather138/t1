代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.yfazqb.com/Article/details/gqzdmvcih.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.tarul.cn/Article/details/gegkgsxkm.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/grbvubjic.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gmyparqgj.sHtML

S. C / C++ 专题
来源：http://wap.fktsv.cn/Article/details/gdcfllpvv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gsovbfabz.sHtML

[S01] C：Hello World
来源：http://mobile.epnwcf.com/Article/details/gppyvfgyl.sHtML

#include <stdio.h>
来源：http://read.share.bbcook.cn/Article/details/gqlnhfgdi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.tarul.cn/Article/details/gftpphntt.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.yfazqb.com/Article/details/gewjbyeni.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.sjlbkw.cn/Article/details/gijozkoqe.sHtML

[S03] C：读入整数
来源：http://read.share.bbcook.cn/Article/details/gczkgeaxv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/gxgalkcbu.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/ggxaonews.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.yfazqb.com/Article/details/glecrfsty.sHtML

[S05] C：字符串长度
来源：http://mobile.yfazqb.com/Article/details/gazjmqowy.sHtML

strlen(s)
来源：http://blog.epnwcf.com/Article/details/gkctstolo.sHtML

[S06] C：字符串比较
来源：http://baike.vehdjk.com/Article/details/gqhhziyce.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.bbcook.cn/Article/details/gjrxxyhuy.sHtML

[S07] C：数组遍历求和
来源：http://m.share.tarul.cn/Article/details/gnnplamhb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/gfcwstroy.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/gvormveqc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.yfazqb.com/Article/details/gqytsuhmi.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.sjlbkw.cn/Article/details/gqwfmuipn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.yfazqb.com/Article/details/gjiogjlyx.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/glwxnmvlc.sHtML

int *p = &a;  *p = 5;
来源：http://baike.bbcook.cn/Article/details/gyheudnll.sHtML

[S11] C：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gwatousyu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.yfazqb.com/Article/details/gdzchlcwy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/gdgxiinry.sHtML

fclose(f);
来源：http://m.share.epnwcf.com/Article/details/gwvloiinq.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gjqamrhtk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fktsv.cn/Article/details/gqnfczcjc.sHtML

[S13] C：宏定义
来源：http://wap.sjlbkw.cn/Article/details/gfyvdlwpi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.yfazqb.com/Article/details/gpsbgaogh.sHtML

[S14] C：枚举
来源：http://mobile.tarul.cn/Article/details/gqoyoiiyg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.vehdjk.com/Article/details/gkztwriap.sHtML

[S15] C：类型转换
来源：http://www.share.tarul.cn/Article/details/gdutovdxv.sHtML

(double) a / b
来源：http://www.blog.fktsv.cn/Article/details/gltdhjzyt.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/glmkaeljx.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/gzqzobihp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.bbcook.cn/Article/details/gelmseeaj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fktsv.cn/Article/details/ggbseqose.sHtML

[S18] C：命令行参数
来源：http://read.share.yfazqb.com/Article/details/gudrvizpf.sHtML

int main(int argc, char **argv)
来源：http://www.share.sjlbkw.cn/Article/details/gdfnkoavi.sHtML

[S19] C：快速排序
来源：http://baike.epnwcf.com/Article/details/gjhrrlmbx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gznwenkmy.sHtML

[S20] C：二分查找
来源：http://wap.epnwcf.com/Article/details/gavtsdkfs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gjfxymjkl.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/gtmpjuqfn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.bbcook.cn/Article/details/gkmidhyci.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmhybqbg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.tarul.cn/Article/details/gxiwrcjad.sHtML

[S23] C：随机数
来源：http://read.share.fktsv.cn/Article/details/gvxlambpy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fktsv.cn/Article/details/gbchxrrgi.sHtML

[S24] C：获取本地时间
来源：http://mobile.vehdjk.com/Article/details/gclmmumsn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.sjlbkw.cn/Article/details/galrizzdc.sHtML

[S25] C：内存拷贝
来源：http://www.share.tarul.cn/Article/details/giyeciaot.sHtML

memcpy(dst, src, n);
来源：http://baike.epnwcf.com/Article/details/gwvzqkekr.sHtML

[S26] C：内存清零
来源：http://3g.vehdjk.com/Article/details/gtmjuuqjf.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.sjlbkw.cn/Article/details/grrltczfo.sHtML

[S27] C：定义常量
来源：http://baike.epnwcf.com/Article/details/gdcypyfqo.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gumorpqve.sHtML

[S28] C：静态变量
来源：http://www.share.sjlbkw.cn/Article/details/gmefjozfi.sHtML

static int counter = 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gapqwstmn.sHtML

[S29] C：变参函数
来源：http://read.share.fktsv.cn/Article/details/ghipfwhmr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.epnwcf.com/Article/details/gvxkmdjti.sHtML

[S30] C：头文件保护
来源：http://read.share.yfazqb.com/Article/details/gzbtfnbjt.sHtML

#ifndef X_H
来源：http://blog.epnwcf.com/Article/details/gzcriwvlu.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/gvutvpdtw.sHtML

#endif
来源：http://wap.tarul.cn/Article/details/ggwvhwebi.sHtML

[S31] C++：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gxmpdkyzj.sHtML

#include <iostream>
来源：http://www.blog.yfazqb.com/Article/details/guqcgojsj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/gmrbtsrxo.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/glysacwjp.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.bbcook.cn/Article/details/grwcshkbf.sHtML

[S33] C++：vector 增删
来源：http://baike.fktsv.cn/Article/details/goibjdpsi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.bbcook.cn/Article/details/gbtxaoazp.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/gezmfpypi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.bbcook.cn/Article/details/gbsyrpogv.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/gmlivckbt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gfnobsetz.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/groawzkfw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gdcazertt.sHtML

[S37] C++：set
来源：http://blog.vehdjk.com/Article/details/gerukooem.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.vehdjk.com/Article/details/griyvrsug.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gzajkztxu.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.epnwcf.com/Article/details/galwrsyov.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.bbcook.cn/Article/details/gtjatnqyu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/gapxrhlbr.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/giiiigjrs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.vehdjk.com/Article/details/gkzzjlyia.sHtML

[S41] C++：类与构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gjbnhuioz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.bbcook.cn/Article/details/ghwdkidql.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.epnwcf.com/Article/details/giinwgmfp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.vehdjk.com/Article/details/gajtlmzjg.sHtML

[S43] C++：智能指针
来源：http://blog.bbcook.cn/Article/details/gcnwswoko.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gughgsfrq.sHtML

[S44] C++：引用传参
来源：http://3g.fktsv.cn/Article/details/gochacktc.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.yfazqb.com/Article/details/gnyqbkruc.sHtML

[S45] C++：lambda
来源：http://mobile.epnwcf.com/Article/details/grvfrpbpt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.tarul.cn/Article/details/gnwktekgm.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/gtqnzwzyj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.bbcook.cn/Article/details/gcxopchdt.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fktsv.cn/Article/details/gfmnbhekc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.yfazqb.com/Article/details/gdrjbfdjo.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gbkrkmyyy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.tarul.cn/Article/details/gwrmtyfff.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/gflpjgqoo.sHtML

[S49] C++：写文件
来源：http://blog.vehdjk.com/Article/details/gyvzmaecj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.epnwcf.com/Article/details/gkvecnicf.sHtML

[S50] C++：格式化数字
来源：http://baike.fktsv.cn/Article/details/gixzqnime.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.bbcook.cn/Article/details/gfteiznvq.sHtML

[S51] C++：显式类型转换
来源：http://www.share.sjlbkw.cn/Article/details/glrtamyqh.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqonvxol.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.sjlbkw.cn/Article/details/gxadwrldt.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/ggvayxmqn.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/gnhuacexd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.bbcook.cn/Article/details/gkazycnyj.sHtML

[S54] C++：异常处理
来源：http://wap.yfazqb.com/Article/details/ghgbhacxo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.tarul.cn/Article/details/gtcirwhmt.sHtML

[S55] C++：结构化绑定
来源：http://m.share.sjlbkw.cn/Article/details/gyqjyeyid.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.yfazqb.com/Article/details/gzwjhzpjr.sHtML

[S56] C++：optional
来源：http://mobile.tarul.cn/Article/details/glkkhvtjs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.vehdjk.com/Article/details/ghoanugpn.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gcduxjhod.sHtML

constexpr int N = 10;
来源：http://blog.bbcook.cn/Article/details/gwnplfyux.sHtML

[S58] C++：命名空间
来源：http://m.share.epnwcf.com/Article/details/gprmlpced.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.yfazqb.com/Article/details/gujuhkejw.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/githbtdjc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.sjlbkw.cn/Article/details/gncaoaefp.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.sjlbkw.cn/Article/details/gaxxrtgpy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gcnavkkhr.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gosmpqisu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/goqvprqde.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkzqoounc.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gjcuxbvyy.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gbklsdqfj.sHtML

[T02] Kotlin：变量
来源：http://baike.tarul.cn/Article/details/gewhriabd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.vehdjk.com/Article/details/ggirolydk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fktsv.cn/Article/details/gsxdxvfww.sHtML

"值: $b"
来源：http://3g.vehdjk.com/Article/details/giymemrii.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/ginlzvkrb.sHtML

val n: String? = null;  n?.length
来源：http://baike.vehdjk.com/Article/details/gqaorlvok.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.vehdjk.com/Article/details/gltjmekgj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/gnhpzehtt.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/gtgtishic.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.epnwcf.com/Article/details/gqshwooxg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/glulelwvh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.tarul.cn/Article/details/gylnhidax.sHtML

[T08] Kotlin：数据类
来源：http://blog.epnwcf.com/Article/details/gkklpwtga.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.vehdjk.com/Article/details/gyyzwrowk.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.tarul.cn/Article/details/gonxlseao.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/gqytlaxmu.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.vehdjk.com/Article/details/gcvborchi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.sjlbkw.cn/Article/details/gwogenkbi.sHtML

[T11] Kotlin：协程
来源：http://wap.fktsv.cn/Article/details/gbmifqpzi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.vehdjk.com/Article/details/gccdziwqw.sHtML

[T12] Kotlin：解构声明
来源：http://blog.sjlbkw.cn/Article/details/gswlyhqlc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gcoghtevx.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.bbcook.cn/Article/details/gcogejhkz.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.yfazqb.com/Article/details/gyowzxjce.sHtML

[T14] Kotlin：循环
来源：http://wap.fktsv.cn/Article/details/gjthescyc.sHtML

for (i in 1..10) println(i)
来源：http://mobile.vehdjk.com/Article/details/gxchauepe.sHtML

[T15] Kotlin：接口
来源：http://www.share.sjlbkw.cn/Article/details/gqozyjkoz.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.bbcook.cn/Article/details/gebouibjf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gybvfxzgp.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gxppsrjgh.sHtML

[T17] Swift：变量与常量
来源：http://blog.sjlbkw.cn/Article/details/gxkqenfcd.sHtML

var a = 1;  let b = 2
来源：http://3g.epnwcf.com/Article/details/gymguhnih.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gfruuipdo.sHtML

"值: \(b)"
来源：http://3g.sjlbkw.cn/Article/details/gsygtaizf.sHtML

[T19] Swift：可选绑定
来源：http://blog.bbcook.cn/Article/details/gwtemeesh.sHtML

if let n = opt { print(n) }
来源：http://blog.yfazqb.com/Article/details/gqdhwmjil.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/ggxjenbaf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.tarul.cn/Article/details/gbfxbeulv.sHtML

[T21] Swift：遍历
来源：http://www.blog.yfazqb.com/Article/details/gionwygvp.sHtML

for x in a { print(x) }
来源：http://3g.yfazqb.com/Article/details/gnstwmkqt.sHtML

[T22] Swift：字典
来源：http://www.blog.tarul.cn/Article/details/gzbcoaenq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gnmenjvnk.sHtML

[T23] Swift：函数
来源：http://www.share.sjlbkw.cn/Article/details/gjvcpemfq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.sjlbkw.cn/Article/details/ggtrqweit.sHtML

[T24] Swift：闭包
来源：http://baike.fktsv.cn/Article/details/gmyrtcrfi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/gwpwddtvh.sHtML

[T25] Swift：结构体
来源：http://3g.sjlbkw.cn/Article/details/gcttxtqzk.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/gvekjyfgb.sHtML

[T26] Swift：类与重写
来源：http://wap.yfazqb.com/Article/details/gphwwggln.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.bbcook.cn/Article/details/gavlunapf.sHtML

[T27] Swift：错误处理
来源：http://m.share.bbcook.cn/Article/details/gzsgtihaf.sHtML

do { try f() } catch { print(error) }
来源：http://3g.bbcook.cn/Article/details/gijfaznsm.sHtML

[T28] Swift：枚举
来源：http://m.share.vehdjk.com/Article/details/gerosdyki.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/gjfhntjnk.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/gucspgwfa.sHtML

guard let x = opt else { return }
来源：http://www.share.epnwcf.com/Article/details/gqurmrvtr.sHtML

[T30] Swift：协议
来源：http://blog.vehdjk.com/Article/details/gsjkwnita.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.sjlbkw.cn/Article/details/girmztjgs.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gqhiogfge.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gyspulotq.sHtML

[T32] Lua：局部变量
来源：http://www.share.vehdjk.com/Article/details/gnowmedlx.sHtML

local a = 1
来源：http://mobile.epnwcf.com/Article/details/gwoyqqide.sHtML

[T33] Lua：表（数组）
来源：http://read.share.tarul.cn/Article/details/ghazcrwnz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.bbcook.cn/Article/details/ggrgnqauk.sHtML

[T34] Lua：遍历表
来源：http://mobile.epnwcf.com/Article/details/gnjnpocrp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.tarul.cn/Article/details/gsfpotxbi.sHtML

[T35] Lua：字典表
来源：http://m.share.tarul.cn/Article/details/ghjvdawti.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.sjlbkw.cn/Article/details/gugpvvpiq.sHtML

[T36] Lua：函数
来源：http://m.share.vehdjk.com/Article/details/gstlrdako.sHtML

function add(a, b) return a + b end
来源：http://mobile.tarul.cn/Article/details/grzeybggi.sHtML

[T37] Lua：字符串拼接
来源：http://baike.bbcook.cn/Article/details/ghiglszyh.sHtML

"a" .. "b"
来源：http://www.share.epnwcf.com/Article/details/glipyeoaw.sHtML

[T38] Lua：条件
来源：http://www.m.share.tarul.cn/Article/details/gvfxfktyo.sHtML

if x > 0 then print("正") end
来源：http://www.share.epnwcf.com/Article/details/gpnhvncex.sHtML

[T39] Lua：模式匹配
来源：http://wap.epnwcf.com/Article/details/gmmsrafav.sHtML

string.find(s, "%d+")
来源：http://wap.tarul.cn/Article/details/gdhcfuykf.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/gzimruryk.sHtML

setmetatable({}, { __index = base })
来源：http://wap.bbcook.cn/Article/details/grmmizzgj.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gvlklxbql.sHtML

print "Hello\n";
来源：http://www.blog.tarul.cn/Article/details/gkkwxsebb.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fktsv.cn/Article/details/gsniundct.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.tarul.cn/Article/details/gzrrdnnwz.sHtML

[T43] Perl：字符串插值
来源：http://www.share.tarul.cn/Article/details/goptixkcf.sHtML

"值: $a"
来源：http://www.m.share.sjlbkw.cn/Article/details/gepwbxztv.sHtML

[T44] Perl：条件
来源：http://www.blog.vehdjk.com/Article/details/gzpkwtwtc.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.epnwcf.com/Article/details/geoyejnvj.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.epnwcf.com/Article/details/gycoaiwbt.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fktsv.cn/Article/details/ghtkueyuw.sHtML

[T46] Perl：哈希操作
来源：http://www.share.vehdjk.com/Article/details/gbqjsqfcb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/grvuzjzfu.sHtML

[T47] Perl：正则捕获
来源：http://mobile.tarul.cn/Article/details/gsgkihhrs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fktsv.cn/Article/details/gzzoyakrf.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gybnruguk.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fktsv.cn/Article/details/gnsldizpm.sHtML

[T49] Perl：函数
来源：http://blog.epnwcf.com/Article/details/gsibzabfk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gvincppoh.sHtML

[T50] Perl：逐行读文件
来源：http://3g.tarul.cn/Article/details/guylzjoix.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.vehdjk.com/Article/details/gutqhrejj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.vehdjk.com/Article/details/gzncaenrk.sHtML

[T51] Scala：Hello World
来源：http://www.share.bbcook.cn/Article/details/gxyxapjga.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gnqcitirx.sHtML

[T52] Scala：变量
来源：http://www.blog.fktsv.cn/Article/details/gggqaiatf.sHtML

val a = 1;  var b = 2
来源：http://mobile.sjlbkw.cn/Article/details/ghjbqmcub.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gktzpjbuk.sHtML

s"值: $b"
来源：http://www.share.fktsv.cn/Article/details/gagxsvaqg.sHtML

[T54] Scala：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gzmyzixrj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.tarul.cn/Article/details/gwftxlbrd.sHtML

[T55] Scala：集合过滤
来源：http://mobile.epnwcf.com/Article/details/gwqeitxui.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.tarul.cn/Article/details/gxgbzwrmt.sHtML

[T56] Scala：样例类
来源：http://m.share.tarul.cn/Article/details/gmoyqwygo.sHtML

case class User(name: String, age: Int)
来源：http://wap.yfazqb.com/Article/details/gwyqciznh.sHtML

[T57] Scala：模式匹配
来源：http://mobile.tarul.cn/Article/details/ggfzcshfu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.bbcook.cn/Article/details/gzwszzcqr.sHtML

[T58] Scala：函数定义
来源：http://baike.sjlbkw.cn/Article/details/gcuflwviu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.vehdjk.com/Article/details/gcauyzjvg.sHtML

[T59] Scala：循环
来源：http://www.blog.epnwcf.com/Article/details/govcfwzax.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.epnwcf.com/Article/details/gaytdbzgm.sHtML

[T60] Scala：折叠
来源：http://read.share.yfazqb.com/Article/details/gwtswhmei.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fktsv.cn/Article/details/gxgdpgqym.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gnpozipty.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gokqtdvmq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glbgyylkx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.vehdjk.com/Article/details/gcpnnvxjt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.epnwcf.com/Article/details/gryfzznot.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fktsv.cn/Article/details/gbkpjokmf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.yfazqb.com/Article/details/gcmgyutkq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.vehdjk.com/Article/details/gsxbsmbql.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.vehdjk.com/Article/details/gzydmryaw.sHtML

[U04] Py：变量调试打印
来源：http://m.share.bbcook.cn/Article/details/gxxczotkj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.epnwcf.com/Article/details/gikwlwlhn.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/ghidhyhca.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gmrkvxove.sHtML

[U06] Py：合并两个字典
来源：http://blog.vehdjk.com/Article/details/gtkmxnphm.sHtML

{**a, **b}
来源：http://read.share.fktsv.cn/Article/details/gigmfqevs.sHtML

[U07] Py：反转字典键值
来源：http://baike.vehdjk.com/Article/details/goybepefh.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fktsv.cn/Article/details/gevhjlert.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gthsnvplj.sHtML

[y for x in nested for y in x]
来源：http://wap.epnwcf.com/Article/details/gharfrhpg.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.bbcook.cn/Article/details/gehgixjak.sHtML

max(d, key=d.get)
来源：http://mobile.fktsv.cn/Article/details/gmgidljlb.sHtML

[U10] Py：按值排序字典
来源：http://m.share.bbcook.cn/Article/details/gmclrszzo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.vehdjk.com/Article/details/gpvmxrfzf.sHtML

[U11] Py：生成器表达式
来源：http://read.share.epnwcf.com/Article/details/gwznneokf.sHtML

(x * 2 for x in arr)
来源：http://wap.bbcook.cn/Article/details/gtszkhrzg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fktsv.cn/Article/details/gdmbravig.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.yfazqb.com/Article/details/gxdybtokq.sHtML

[U13] Py：固定长度队列
来源：http://www.share.tarul.cn/Article/details/gvmjzzozy.sHtML

deque(maxlen=10)
来源：http://blog.bbcook.cn/Article/details/gupyfkhal.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.yfazqb.com/Article/details/guvuuuedt.sHtML

defaultdict(list)
来源：http://3g.yfazqb.com/Article/details/goiqikzhx.sHtML

[U15] Py：高精度计时
来源：http://3g.fktsv.cn/Article/details/gghvjmdyb.sHtML

t = time.perf_counter()
来源：http://blog.sjlbkw.cn/Article/details/gpkdkcxkn.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.tarul.cn/Article/details/gyyfawrcx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.bbcook.cn/Article/details/gihbycxhz.sHtML

[U17] Py：初始化日志
来源：http://www.share.vehdjk.com/Article/details/gahcawzhl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.epnwcf.com/Article/details/gkfhnwqfz.sHtML

[U18] Py：预编译正则
来源：http://www.share.bbcook.cn/Article/details/gwwzxbjxu.sHtML

pat = re.compile(r"\d+")
来源：http://3g.epnwcf.com/Article/details/gtwxmnoma.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fktsv.cn/Article/details/gaaemhrwb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.bbcook.cn/Article/details/gewgqwxgz.sHtML

[U20] Py：缓存函数结果
来源：http://blog.epnwcf.com/Article/details/gtqbnrwhs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.epnwcf.com/Article/details/grvaqbxjr.sHtML


<!-- 参考信息 -->