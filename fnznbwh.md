代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.vehdjk.com/Article/details/ggpolnjrs.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/gpnsejjbc.sHtML

time ./run.sh
来源：http://baike.yfazqb.com/Article/details/gnvsekger.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbxcjsftv.sHtML

S. C / C++ 专题
来源：http://3g.epnwcf.com/Article/details/grzcddvrb.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkgwttcsi.sHtML

[S01] C：Hello World
来源：http://m.share.fktsv.cn/Article/details/gdncowjom.sHtML

#include <stdio.h>
来源：http://m.share.bbcook.cn/Article/details/gczzbiogc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.yfazqb.com/Article/details/gpvpzhzcr.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.epnwcf.com/Article/details/gaiznypmw.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.bbcook.cn/Article/details/gzkmxrxsz.sHtML

[S03] C：读入整数
来源：http://www.share.epnwcf.com/Article/details/gldzfonhl.sHtML

int x; scanf("%d", &x);
来源：http://3g.tarul.cn/Article/details/gyisnevqx.sHtML

[S04] C：字符串复制
来源：http://read.share.bbcook.cn/Article/details/gxhakcykj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.yfazqb.com/Article/details/gtcriynph.sHtML

[S05] C：字符串长度
来源：http://wap.bbcook.cn/Article/details/gjzjirjjs.sHtML

strlen(s)
来源：http://blog.vehdjk.com/Article/details/gdsfxeqqe.sHtML

[S06] C：字符串比较
来源：http://blog.tarul.cn/Article/details/gwdfbmyoa.sHtML

strcmp(a, b) == 0
来源：http://mobile.fktsv.cn/Article/details/golcypezu.sHtML

[S07] C：数组遍历求和
来源：http://www.share.vehdjk.com/Article/details/gzbfgryew.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.bbcook.cn/Article/details/gczmdltzp.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.vehdjk.com/Article/details/gzmldvoeg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.yfazqb.com/Article/details/gyyvxkinf.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/gdgsozscf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.tarul.cn/Article/details/ghptgmwny.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/ggsbiadja.sHtML

int *p = &a;  *p = 5;
来源：http://blog.sjlbkw.cn/Article/details/godkjaeqy.sHtML

[S11] C：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gblbqlltp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fktsv.cn/Article/details/gtmlvdgqz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.sjlbkw.cn/Article/details/gwsezpkex.sHtML

fclose(f);
来源：http://mobile.tarul.cn/Article/details/gkzdirznk.sHtML

[S12] C：写文件
来源：http://wap.vehdjk.com/Article/details/gbdfqrltg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/georilnpa.sHtML

[S13] C：宏定义
来源：http://www.share.sjlbkw.cn/Article/details/gwyqmdrns.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.tarul.cn/Article/details/gfolraftw.sHtML

[S14] C：枚举
来源：http://blog.epnwcf.com/Article/details/guqvhxvsi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/gyhhuznth.sHtML

[S15] C：类型转换
来源：http://www.blog.fktsv.cn/Article/details/gxmdtlhlh.sHtML

(double) a / b
来源：http://baike.bbcook.cn/Article/details/gzvnyvmqa.sHtML

[S16] C：位操作置位
来源：http://wap.vehdjk.com/Article/details/gaffuvhjl.sHtML

x |= (1 << 3);
来源：http://m.share.tarul.cn/Article/details/gleirnugc.sHtML

[S17] C：安全拼接字符串
来源：http://baike.epnwcf.com/Article/details/gduohpldj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.vehdjk.com/Article/details/gjdkxgpxg.sHtML

[S18] C：命令行参数
来源：http://www.share.tarul.cn/Article/details/gjybnsicz.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/gwavbqefb.sHtML

[S19] C：快速排序
来源：http://3g.epnwcf.com/Article/details/gmepwdapx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gcwmgzwja.sHtML

[S20] C：二分查找
来源：http://www.m.share.tarul.cn/Article/details/guyizagsu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/geobocfof.sHtML

[S21] C：字符类别判断
来源：http://www.share.epnwcf.com/Article/details/gdrloyqcp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.epnwcf.com/Article/details/guckydsbb.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/gskrzoupg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.bbcook.cn/Article/details/ggmcrzcjq.sHtML

[S23] C：随机数
来源：http://www.blog.bbcook.cn/Article/details/gucdqqxyv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.vehdjk.com/Article/details/ghthybszh.sHtML

[S24] C：获取本地时间
来源：http://mobile.fktsv.cn/Article/details/gwwehzpqy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.bbcook.cn/Article/details/gptcujkbo.sHtML

[S25] C：内存拷贝
来源：http://www.share.vehdjk.com/Article/details/gybnffunf.sHtML

memcpy(dst, src, n);
来源：http://baike.yfazqb.com/Article/details/gxcqvrpow.sHtML

[S26] C：内存清零
来源：http://blog.epnwcf.com/Article/details/gakvasmvy.sHtML

memset(a, 0, sizeof a);
来源：http://3g.yfazqb.com/Article/details/gxpghmelk.sHtML

[S27] C：定义常量
来源：http://m.share.yfazqb.com/Article/details/gmgcfiigv.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gsfqbzyno.sHtML

[S28] C：静态变量
来源：http://m.share.yfazqb.com/Article/details/ggaojphaj.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/gwsbjxfwq.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/gnkxcvshq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/grliohdat.sHtML

[S30] C：头文件保护
来源：http://wap.epnwcf.com/Article/details/gtyrtreij.sHtML

#ifndef X_H
来源：http://m.share.fktsv.cn/Article/details/gtddpomfi.sHtML

#define X_H
来源：http://www.share.epnwcf.com/Article/details/ghawlfwat.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/gddsdbmxk.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/gpdzamfum.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/gxtdflyeo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/ggryeajbn.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gubceqdes.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/glplkjcnh.sHtML

[S33] C++：vector 增删
来源：http://read.share.bbcook.cn/Article/details/gxzplzyvk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.bbcook.cn/Article/details/gdvmzknpc.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/gkfrydage.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.tarul.cn/Article/details/gclemyuhd.sHtML

[S35] C++：map
来源：http://blog.bbcook.cn/Article/details/gbryegxqs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gsgpsocde.sHtML

[S36] C++：unordered_map
来源：http://m.share.sjlbkw.cn/Article/details/gptnmygci.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gtbejivjl.sHtML

[S37] C++：set
来源：http://baike.fktsv.cn/Article/details/gtdbhbnam.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.yfazqb.com/Article/details/gskdzmdyz.sHtML

[S38] C++：排序
来源：http://read.share.epnwcf.com/Article/details/ghtgtisee.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/giytzpyqf.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.sjlbkw.cn/Article/details/gplkaszqt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fktsv.cn/Article/details/gtjhxfdzv.sHtML

[S40] C++：查找元素
来源：http://wap.vehdjk.com/Article/details/gbrtajeiq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.sjlbkw.cn/Article/details/gvqsuflnf.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/gjfsyxhiz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.tarul.cn/Article/details/gjercfkky.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.yfazqb.com/Article/details/guvzkxiyq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.tarul.cn/Article/details/gmawtoevh.sHtML

[S43] C++：智能指针
来源：http://www.blog.fktsv.cn/Article/details/gcbeaduvh.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.bbcook.cn/Article/details/gapltkbnl.sHtML

[S44] C++：引用传参
来源：http://3g.fktsv.cn/Article/details/giqjcpyix.sHtML

void inc(int &x) { ++x; }
来源：http://3g.tarul.cn/Article/details/gtwwuywea.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gstvpilav.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fktsv.cn/Article/details/gaiowkavh.sHtML

[S46] C++：函数模板
来源：http://blog.epnwcf.com/Article/details/giewupxcy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gsnrxyjin.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.sjlbkw.cn/Article/details/gzzuokyhu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.bbcook.cn/Article/details/gggrctbho.sHtML

[S48] C++：逐行读文件
来源：http://3g.epnwcf.com/Article/details/ghmfuyghe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.yfazqb.com/Article/details/gyqmjelbg.sHtML

while (std::getline(in, line)) { }
来源：http://baike.epnwcf.com/Article/details/gqmmdswqg.sHtML

[S49] C++：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gxdqsyazy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.vehdjk.com/Article/details/gmawggsnc.sHtML

[S50] C++：格式化数字
来源：http://m.share.sjlbkw.cn/Article/details/gfgfholwf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gchqriqbk.sHtML

[S51] C++：显式类型转换
来源：http://m.share.tarul.cn/Article/details/gzuhahurl.sHtML

static_cast<double>(a) / b
来源：http://blog.vehdjk.com/Article/details/grkjvnplh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/gixjsjyiy.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.yfazqb.com/Article/details/gxcmyieby.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/gjxunnkqw.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.tarul.cn/Article/details/gxcvlzpcj.sHtML

[S54] C++：异常处理
来源：http://read.share.bbcook.cn/Article/details/gvhvacqqy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.vehdjk.com/Article/details/gvypakvmn.sHtML

[S55] C++：结构化绑定
来源：http://m.share.tarul.cn/Article/details/gxhwcovrx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gbmrjgclr.sHtML

[S56] C++：optional
来源：http://www.m.share.fktsv.cn/Article/details/grqfedujr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.tarul.cn/Article/details/gvfiyprvz.sHtML

[S57] C++：编译期常量
来源：http://www.share.fktsv.cn/Article/details/gnrbesfjv.sHtML

constexpr int N = 10;
来源：http://3g.bbcook.cn/Article/details/gjnqgrjwd.sHtML

[S58] C++：命名空间
来源：http://baike.tarul.cn/Article/details/gavjocrjm.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/goqrclapg.sHtML

[S59] C++：静态断言
来源：http://www.m.share.tarul.cn/Article/details/gmbuekmzk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.yfazqb.com/Article/details/grwgugnnh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.vehdjk.com/Article/details/gmgmvydyc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.tarul.cn/Article/details/grvfresfc.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjewymoma.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.tarul.cn/Article/details/gssjjmuqt.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/goryexmzk.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.yfazqb.com/Article/details/gdqwwfcno.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gskgveygm.sHtML

[T02] Kotlin：变量
来源：http://wap.bbcook.cn/Article/details/gxsxblfzg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.bbcook.cn/Article/details/gfghcallh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.tarul.cn/Article/details/gbxpkdmel.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/gontkltsu.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/gvvvdfvhm.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.tarul.cn/Article/details/grsnevodw.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.epnwcf.com/Article/details/gdumlyawt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fktsv.cn/Article/details/gzxmxpiff.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.yfazqb.com/Article/details/gbfnphsla.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.vehdjk.com/Article/details/gyxtdjdef.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fktsv.cn/Article/details/gggwurkke.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.epnwcf.com/Article/details/gxujdbbci.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fktsv.cn/Article/details/gntgipjxx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.epnwcf.com/Article/details/gcqdqrrhb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/ggdsthmpq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fktsv.cn/Article/details/gapblotic.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gthbsyaaj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fktsv.cn/Article/details/gvdclgvwf.sHtML

[T11] Kotlin：协程
来源：http://baike.vehdjk.com/Article/details/gybvlfszg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.tarul.cn/Article/details/glfbvtcoh.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/gacfyuitp.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.yfazqb.com/Article/details/guvybuqkq.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/gqqgwolrl.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gdrrjsnzl.sHtML

[T14] Kotlin：循环
来源：http://wap.sjlbkw.cn/Article/details/gazbvndlq.sHtML

for (i in 1..10) println(i)
来源：http://baike.tarul.cn/Article/details/gfuezznjx.sHtML

[T15] Kotlin：接口
来源：http://wap.bbcook.cn/Article/details/gflxcljqe.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fktsv.cn/Article/details/gymoivqpt.sHtML

[T16] Swift：Hello World
来源：http://blog.yfazqb.com/Article/details/gxvjehkmu.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gwmxzmkdm.sHtML

[T17] Swift：变量与常量
来源：http://www.share.epnwcf.com/Article/details/gkvyskerk.sHtML

var a = 1;  let b = 2
来源：http://read.share.tarul.cn/Article/details/gzraihygy.sHtML

[T18] Swift：字符串插值
来源：http://blog.vehdjk.com/Article/details/gjubmouqq.sHtML

"值: \(b)"
来源：http://baike.epnwcf.com/Article/details/gwotrqgot.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/gtwvaqzap.sHtML

if let n = opt { print(n) }
来源：http://blog.sjlbkw.cn/Article/details/gjecyqxxe.sHtML

[T20] Swift：数组操作
来源：http://read.share.bbcook.cn/Article/details/gilwlyree.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.yfazqb.com/Article/details/gqnfdlmid.sHtML

[T21] Swift：遍历
来源：http://www.blog.tarul.cn/Article/details/grkkucsye.sHtML

for x in a { print(x) }
来源：http://read.share.epnwcf.com/Article/details/gqplqmmxb.sHtML

[T22] Swift：字典
来源：http://wap.bbcook.cn/Article/details/gemgeopgl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fktsv.cn/Article/details/gmatviueg.sHtML

[T23] Swift：函数
来源：http://www.share.bbcook.cn/Article/details/gufwvondl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.tarul.cn/Article/details/gfpyqzpwb.sHtML

[T24] Swift：闭包
来源：http://mobile.tarul.cn/Article/details/gqugfwkig.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.yfazqb.com/Article/details/gxlnfduqo.sHtML

[T25] Swift：结构体
来源：http://m.share.sjlbkw.cn/Article/details/gtpknrhlo.sHtML

struct P { var x: Int }
来源：http://read.share.sjlbkw.cn/Article/details/gvwtepcvz.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/gcropbsvs.sHtML

class A: Base { override func f() {} }
来源：http://blog.yfazqb.com/Article/details/gsqrereix.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.epnwcf.com/Article/details/gsvcdinet.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.sjlbkw.cn/Article/details/ghpcbyrmg.sHtML

[T28] Swift：枚举
来源：http://baike.sjlbkw.cn/Article/details/gkqdxdzze.sHtML

enum Color { case red, green }
来源：http://mobile.epnwcf.com/Article/details/gwtxlqbom.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrjgudkj.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/guzmmuagc.sHtML

[T30] Swift：协议
来源：http://baike.tarul.cn/Article/details/gtqbfvuuo.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.tarul.cn/Article/details/glbxxrpgj.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gnbegunrk.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gjicrlogs.sHtML

[T32] Lua：局部变量
来源：http://3g.yfazqb.com/Article/details/gtssklwpm.sHtML

local a = 1
来源：http://blog.bbcook.cn/Article/details/gqagzerlo.sHtML

[T33] Lua：表（数组）
来源：http://www.share.sjlbkw.cn/Article/details/gwnqoocmv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.sjlbkw.cn/Article/details/gtrcdfyri.sHtML

[T34] Lua：遍历表
来源：http://blog.yfazqb.com/Article/details/gkfwhisfk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.bbcook.cn/Article/details/gufumszja.sHtML

[T35] Lua：字典表
来源：http://www.m.share.epnwcf.com/Article/details/gzkyuomrt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.sjlbkw.cn/Article/details/gdmyzimxp.sHtML

[T36] Lua：函数
来源：http://mobile.sjlbkw.cn/Article/details/groppbqgp.sHtML

function add(a, b) return a + b end
来源：http://3g.yfazqb.com/Article/details/gigofxdlm.sHtML

[T37] Lua：字符串拼接
来源：http://3g.tarul.cn/Article/details/gurjmvuub.sHtML

"a" .. "b"
来源：http://blog.vehdjk.com/Article/details/ggrlfgvzw.sHtML

[T38] Lua：条件
来源：http://mobile.sjlbkw.cn/Article/details/gyrfufkgc.sHtML

if x > 0 then print("正") end
来源：http://baike.fktsv.cn/Article/details/godnflmbj.sHtML

[T39] Lua：模式匹配
来源：http://wap.epnwcf.com/Article/details/gyszshqhh.sHtML

string.find(s, "%d+")
来源：http://www.blog.epnwcf.com/Article/details/gykfcmpga.sHtML

[T40] Lua：元表
来源：http://3g.fktsv.cn/Article/details/gdaopwgqu.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.yfazqb.com/Article/details/gnekakvds.sHtML

[T41] Perl：Hello World
来源：http://mobile.bbcook.cn/Article/details/gohbfhail.sHtML

print "Hello\n";
来源：http://www.blog.yfazqb.com/Article/details/gxxpjcrzz.sHtML

[T42] Perl：变量类型
来源：http://3g.sjlbkw.cn/Article/details/grkbooark.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.sjlbkw.cn/Article/details/grzgzjnwo.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gxvvwtgcv.sHtML

"值: $a"
来源：http://m.share.tarul.cn/Article/details/gvokiwatb.sHtML

[T44] Perl：条件
来源：http://www.blog.fktsv.cn/Article/details/gqiecvhxf.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.bbcook.cn/Article/details/gxrqwpzgq.sHtML

[T45] Perl：数组遍历
来源：http://read.share.vehdjk.com/Article/details/ggvoxpjcx.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.bbcook.cn/Article/details/gokttgljd.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.vehdjk.com/Article/details/gujoeknew.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/gyhznflkj.sHtML

[T47] Perl：正则捕获
来源：http://www.share.epnwcf.com/Article/details/gxgjaaejw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.sjlbkw.cn/Article/details/gdmvzbwuq.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/gxqsjhxqu.sHtML

$s =~ s/old/new/g;
来源：http://mobile.vehdjk.com/Article/details/gldodrdyl.sHtML

[T49] Perl：函数
来源：http://www.share.sjlbkw.cn/Article/details/gnbdrxpfz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gnovvinvl.sHtML

[T50] Perl：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gtflwwanh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.sjlbkw.cn/Article/details/ghvooyywd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.bbcook.cn/Article/details/gynhpbwps.sHtML

[T51] Scala：Hello World
来源：http://blog.fktsv.cn/Article/details/gnzvgraxb.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/gpncpsnrk.sHtML

[T52] Scala：变量
来源：http://read.share.yfazqb.com/Article/details/gbevziozr.sHtML

val a = 1;  var b = 2
来源：http://wap.bbcook.cn/Article/details/gnsslagae.sHtML

[T53] Scala：字符串插值
来源：http://read.share.tarul.cn/Article/details/gdonkgvtm.sHtML

s"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gzliorycb.sHtML

[T54] Scala：集合映射
来源：http://read.share.epnwcf.com/Article/details/gjvdnploi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.bbcook.cn/Article/details/gkdtgcuzn.sHtML

[T55] Scala：集合过滤
来源：http://baike.epnwcf.com/Article/details/gmkgyrpdy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.bbcook.cn/Article/details/guorcsmcg.sHtML

[T56] Scala：样例类
来源：http://wap.epnwcf.com/Article/details/gkakxagdy.sHtML

case class User(name: String, age: Int)
来源：http://mobile.epnwcf.com/Article/details/glbribrlr.sHtML

[T57] Scala：模式匹配
来源：http://mobile.epnwcf.com/Article/details/gcdrcanck.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.bbcook.cn/Article/details/gkfpxfrgs.sHtML

[T58] Scala：函数定义
来源：http://wap.tarul.cn/Article/details/gurmeqnsl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.bbcook.cn/Article/details/gridfncvl.sHtML

[T59] Scala：循环
来源：http://mobile.yfazqb.com/Article/details/gtuvlepvo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gcwtnkytc.sHtML

[T60] Scala：折叠
来源：http://wap.bbcook.cn/Article/details/gxhfvhwxd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.sjlbkw.cn/Article/details/gobbhlhxy.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjptjuetb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.vehdjk.com/Article/details/gjspkujig.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/goztjspzv.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.tarul.cn/Article/details/gucnaxypb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.vehdjk.com/Article/details/gymikzzrc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.sjlbkw.cn/Article/details/gipmhshir.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.yfazqb.com/Article/details/gbyqnlkqa.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.yfazqb.com/Article/details/guglfisyk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.yfazqb.com/Article/details/gwggwffkj.sHtML

[U04] Py：变量调试打印
来源：http://wap.tarul.cn/Article/details/gtsdvaphy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.sjlbkw.cn/Article/details/gdfbnfiut.sHtML

[U05] Py：列表去重且保序
来源：http://baike.bbcook.cn/Article/details/gjowirslh.sHtML

list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/gsxkofxay.sHtML

[U06] Py：合并两个字典
来源：http://m.share.tarul.cn/Article/details/ghnpmdbfk.sHtML

{**a, **b}
来源：http://www.blog.sjlbkw.cn/Article/details/gmtvljkcb.sHtML

[U07] Py：反转字典键值
来源：http://mobile.bbcook.cn/Article/details/ginlgcctz.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.yfazqb.com/Article/details/gqbfappdh.sHtML

[U08] Py：展平二维列表
来源：http://mobile.yfazqb.com/Article/details/gbsyrfwyg.sHtML

[y for x in nested for y in x]
来源：http://m.share.sjlbkw.cn/Article/details/gzcgbmsfn.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.epnwcf.com/Article/details/gnqbwejon.sHtML

max(d, key=d.get)
来源：http://3g.fktsv.cn/Article/details/glxmbzabs.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.tarul.cn/Article/details/getnlxszj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.epnwcf.com/Article/details/gasnvzyfd.sHtML

[U11] Py：生成器表达式
来源：http://wap.bbcook.cn/Article/details/gorpnmbnk.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.tarul.cn/Article/details/gylmbnckq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.sjlbkw.cn/Article/details/gprlydcdq.sHtML

Counter(arr).most_common(3)
来源：http://wap.bbcook.cn/Article/details/gkwmyvldq.sHtML

[U13] Py：固定长度队列
来源：http://3g.fktsv.cn/Article/details/grhelyqfa.sHtML

deque(maxlen=10)
来源：http://blog.fktsv.cn/Article/details/ggcdwydzx.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.bbcook.cn/Article/details/gktxajqgi.sHtML

defaultdict(list)
来源：http://m.share.sjlbkw.cn/Article/details/gyfstwphp.sHtML

[U15] Py：高精度计时
来源：http://wap.bbcook.cn/Article/details/gvywxsgme.sHtML

t = time.perf_counter()
来源：http://read.share.tarul.cn/Article/details/gntevamct.sHtML

[U16] Py：命令行参数解析
来源：http://baike.vehdjk.com/Article/details/gupsxcvrh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.yfazqb.com/Article/details/gaonhlbei.sHtML

[U17] Py：初始化日志
来源：http://m.share.sjlbkw.cn/Article/details/giedtrvlk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.tarul.cn/Article/details/gsextqesf.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.vehdjk.com/Article/details/gdntjgjgs.sHtML

pat = re.compile(r"\d+")
来源：http://blog.yfazqb.com/Article/details/gfxsamfmu.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fktsv.cn/Article/details/gkitxtcdz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.bbcook.cn/Article/details/gkmfmivto.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.yfazqb.com/Article/details/gfeuqqehc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fktsv.cn/Article/details/gwtbcnaaw.sHtML


<!-- 参考信息 -->