代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://blog.fktsv.cn/Article/details/gkfnifweg.sHtML

[R76] 使用临时文件
来源：http://blog.vehdjk.com/Article/details/gyoislsxj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gswakppno.sHtML

[R77] 读取用户输入
来源：http://www.blog.bbcook.cn/Article/details/gytkrsgmv.sHtML

read -rp "请输入: " ans
来源：http://www.share.fktsv.cn/Article/details/gthxkyyjb.sHtML

[R78] 交互式菜单
来源：http://blog.epnwcf.com/Article/details/gdljyukrq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.tarul.cn/Article/details/gjvsxtoly.sHtML

[R79] 解析命令行选项
来源：http://3g.bbcook.cn/Article/details/gxbahvyrk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.vehdjk.com/Article/details/gmwgbyrvi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.yfazqb.com/Article/details/gxomegkiw.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/godvjejtv.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmbkacnxw.sHtML

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/gusgfukna.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdbrotysf.sHtML

[S01] C：Hello World
来源：http://mobile.epnwcf.com/Article/details/gxrkdsgmb.sHtML

#include <stdio.h>
来源：http://blog.yfazqb.com/Article/details/gtoaxwyom.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.vehdjk.com/Article/details/gstwltxiq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.tarul.cn/Article/details/gdeaxotra.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.epnwcf.com/Article/details/gsbtiwsds.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gknqbigmu.sHtML

int x; scanf("%d", &x);
来源：http://mobile.vehdjk.com/Article/details/gdymeyrdb.sHtML

[S04] C：字符串复制
来源：http://mobile.vehdjk.com/Article/details/gnbbptrag.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.yfazqb.com/Article/details/gbfhcgeac.sHtML

[S05] C：字符串长度
来源：http://www.blog.tarul.cn/Article/details/gvwcyngtt.sHtML

strlen(s)
来源：http://www.blog.tarul.cn/Article/details/gjiwylrfv.sHtML

[S06] C：字符串比较
来源：http://mobile.bbcook.cn/Article/details/gvupnprzf.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/gzjomdbfp.sHtML

[S07] C：数组遍历求和
来源：http://blog.sjlbkw.cn/Article/details/gheuzurfl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.epnwcf.com/Article/details/gbzoecwcu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.bbcook.cn/Article/details/gojjjkqbd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.epnwcf.com/Article/details/ggrunbnlm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/gyzgusmwk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.bbcook.cn/Article/details/gqqjqptsx.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gihbdtfwy.sHtML

int *p = &a;  *p = 5;
来源：http://baike.sjlbkw.cn/Article/details/gqwwstsgj.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gizkdabgc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.tarul.cn/Article/details/giybkxfuu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fktsv.cn/Article/details/gwhcmccss.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gsvzixthl.sHtML

[S12] C：写文件
来源：http://read.share.tarul.cn/Article/details/gpomsbvlj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gykzmzbdd.sHtML

[S13] C：宏定义
来源：http://blog.tarul.cn/Article/details/gbqdzresc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.sjlbkw.cn/Article/details/gbnnwpsci.sHtML

[S14] C：枚举
来源：http://wap.sjlbkw.cn/Article/details/gzhsbfovi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.sjlbkw.cn/Article/details/gifzkjpha.sHtML

[S15] C：类型转换
来源：http://wap.vehdjk.com/Article/details/gxdhmzpri.sHtML

(double) a / b
来源：http://blog.vehdjk.com/Article/details/ggxjsresl.sHtML

[S16] C：位操作置位
来源：http://baike.tarul.cn/Article/details/gmcvdhhww.sHtML

x |= (1 << 3);
来源：http://read.share.tarul.cn/Article/details/grhrqtkco.sHtML

[S17] C：安全拼接字符串
来源：http://baike.yfazqb.com/Article/details/gyemsfpty.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.tarul.cn/Article/details/gkmrfgqev.sHtML

[S18] C：命令行参数
来源：http://mobile.bbcook.cn/Article/details/gzudofyxt.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/gyksnrvxt.sHtML

[S19] C：快速排序
来源：http://www.blog.sjlbkw.cn/Article/details/gtsgppuko.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gpijrhylc.sHtML

[S20] C：二分查找
来源：http://www.m.share.yfazqb.com/Article/details/galrwidzd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gmntmvewg.sHtML

[S21] C：字符类别判断
来源：http://read.share.vehdjk.com/Article/details/gqmwfsldd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.sjlbkw.cn/Article/details/gzwjujfwv.sHtML

[S22] C：字符串转数字
来源：http://blog.vehdjk.com/Article/details/gwojsusbh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.yfazqb.com/Article/details/gnlvdaijf.sHtML

[S23] C：随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gactzjyhj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.yfazqb.com/Article/details/gqdrpgggv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/gtdykqwzg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.vehdjk.com/Article/details/ggqsorxeb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gqywjxpvc.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/gqqsgdvog.sHtML

[S26] C：内存清零
来源：http://m.share.sjlbkw.cn/Article/details/gynafdzrp.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fktsv.cn/Article/details/ggpvdfzhy.sHtML

[S27] C：定义常量
来源：http://m.share.epnwcf.com/Article/details/gbmzichua.sHtML

const double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gnmqkrmoy.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gaynmriqb.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/gmajbipjv.sHtML

[S29] C：变参函数
来源：http://www.m.share.fktsv.cn/Article/details/gqegsodre.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.sjlbkw.cn/Article/details/gojgkoxoo.sHtML

[S30] C：头文件保护
来源：http://m.share.vehdjk.com/Article/details/gzucvgbcz.sHtML

#ifndef X_H
来源：http://www.m.share.fktsv.cn/Article/details/gibfcfteh.sHtML

#define X_H
来源：http://www.blog.epnwcf.com/Article/details/gqzaoucpl.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gjevkkhlt.sHtML

[S31] C++：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gwjhijeen.sHtML

#include <iostream>
来源：http://baike.tarul.cn/Article/details/gdniybfor.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/ggaqoaomu.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/ghnpcexpb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.sjlbkw.cn/Article/details/gpstihbkg.sHtML

[S33] C++：vector 增删
来源：http://wap.bbcook.cn/Article/details/gaakyqgfg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.tarul.cn/Article/details/gcmhvlgts.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/ghvzdakjc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.tarul.cn/Article/details/gdttozqkn.sHtML

[S35] C++：map
来源：http://baike.fktsv.cn/Article/details/gtoujzrkq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gkliyqwpr.sHtML

[S36] C++：unordered_map
来源：http://mobile.fktsv.cn/Article/details/gnjyinald.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gmmwyqevk.sHtML

[S37] C++：set
来源：http://www.blog.yfazqb.com/Article/details/gyhgyjpow.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.yfazqb.com/Article/details/gjvuzzyzn.sHtML

[S38] C++：排序
来源：http://blog.sjlbkw.cn/Article/details/gtmwhprft.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fktsv.cn/Article/details/gbyowwdkd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.yfazqb.com/Article/details/gmburkaaj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.sjlbkw.cn/Article/details/gfttpejai.sHtML

[S40] C++：查找元素
来源：http://blog.bbcook.cn/Article/details/gmnlolxby.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/gyyhriqbg.sHtML

[S41] C++：类与构造函数
来源：http://mobile.epnwcf.com/Article/details/goyhaaque.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/gvwhcdkrt.sHtML

[S42] C++：继承与虚函数
来源：http://wap.bbcook.cn/Article/details/gttralggh.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/gztfbdljf.sHtML

[S43] C++：智能指针
来源：http://www.m.share.yfazqb.com/Article/details/gtyghdavf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gdmljwqrr.sHtML

[S44] C++：引用传参
来源：http://mobile.fktsv.cn/Article/details/gjzdrectl.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.epnwcf.com/Article/details/giiurxpid.sHtML

[S45] C++：lambda
来源：http://blog.vehdjk.com/Article/details/gxhtwksza.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/grmwdxsrt.sHtML

[S46] C++：函数模板
来源：http://www.m.share.yfazqb.com/Article/details/gxaolyluq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fktsv.cn/Article/details/gndvhdhhh.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.sjlbkw.cn/Article/details/gnkxxwfwa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.epnwcf.com/Article/details/gshzuvvvs.sHtML

[S48] C++：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gyxormoiw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.vehdjk.com/Article/details/gqjeovdzz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/guhhvjjbs.sHtML

[S49] C++：写文件
来源：http://read.share.fktsv.cn/Article/details/gsoarjajh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.bbcook.cn/Article/details/gdbiakegc.sHtML

[S50] C++：格式化数字
来源：http://mobile.epnwcf.com/Article/details/guezhedak.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gzxvzjatq.sHtML

[S51] C++：显式类型转换
来源：http://blog.yfazqb.com/Article/details/gtjiqgjts.sHtML

static_cast<double>(a) / b
来源：http://mobile.yfazqb.com/Article/details/gnctvbvvf.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.sjlbkw.cn/Article/details/gdgnrieti.sHtML

int size() const noexcept { return n_; }
来源：http://blog.tarul.cn/Article/details/guzpkptdw.sHtML

[S53] C++：移动语义
来源：http://mobile.fktsv.cn/Article/details/gfxmxrrxr.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/gchtyjoas.sHtML

[S54] C++：异常处理
来源：http://m.share.yfazqb.com/Article/details/gjxotbyit.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.tarul.cn/Article/details/gojmbsujs.sHtML

[S55] C++：结构化绑定
来源：http://m.share.yfazqb.com/Article/details/gcrarslvv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.yfazqb.com/Article/details/gvcnbslqc.sHtML

[S56] C++：optional
来源：http://baike.bbcook.cn/Article/details/gemtposzc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.vehdjk.com/Article/details/gumrlvkcu.sHtML

[S57] C++：编译期常量
来源：http://blog.vehdjk.com/Article/details/gaemqwluk.sHtML

constexpr int N = 10;
来源：http://mobile.tarul.cn/Article/details/gpdvvurzm.sHtML

[S58] C++：命名空间
来源：http://baike.sjlbkw.cn/Article/details/gvdzvtnhz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.sjlbkw.cn/Article/details/giauzwrdp.sHtML

[S59] C++：静态断言
来源：http://www.share.vehdjk.com/Article/details/gdvlvosey.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gxtoatpzk.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/gnqbxwvqo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.bbcook.cn/Article/details/gioawxvhn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gbfapszzm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gboydqcwt.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gcbhivbnp.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.vehdjk.com/Article/details/gagdgmjal.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/glpopipia.sHtML

[T02] Kotlin：变量
来源：http://read.share.vehdjk.com/Article/details/giabfmnra.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.vehdjk.com/Article/details/gijcjgdzm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.bbcook.cn/Article/details/grfojhxlq.sHtML

"值: $b"
来源：http://baike.yfazqb.com/Article/details/gbxofsyqg.sHtML

[T04] Kotlin：空安全
来源：http://3g.vehdjk.com/Article/details/gvmklpvqp.sHtML

val n: String? = null;  n?.length
来源：http://m.share.vehdjk.com/Article/details/ghptyezuw.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.yfazqb.com/Article/details/gfgmlexkl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.tarul.cn/Article/details/gyobbvuln.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.yfazqb.com/Article/details/gjvpdpoln.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.vehdjk.com/Article/details/goacrmiiz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gpieizsfc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.bbcook.cn/Article/details/gweqlecxc.sHtML

[T08] Kotlin：数据类
来源：http://blog.vehdjk.com/Article/details/gdrozcsnd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fktsv.cn/Article/details/gdpsfaske.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.vehdjk.com/Article/details/gdrzwcito.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.bbcook.cn/Article/details/grlevlvap.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.vehdjk.com/Article/details/gxynrskso.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gjiemxzjp.sHtML

[T11] Kotlin：协程
来源：http://www.blog.yfazqb.com/Article/details/gzzsvggzo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.yfazqb.com/Article/details/gjlpihjfp.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.tarul.cn/Article/details/gtxeyejbv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gbqxfvijl.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.sjlbkw.cn/Article/details/gismeaufu.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.yfazqb.com/Article/details/ginygaupc.sHtML

[T14] Kotlin：循环
来源：http://m.share.fktsv.cn/Article/details/ggnhbjoch.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gucakpujx.sHtML

[T15] Kotlin：接口
来源：http://read.share.sjlbkw.cn/Article/details/gewdjsqgn.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/ghpyjumob.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/guwotssnq.sHtML

print("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gsrrosatu.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.yfazqb.com/Article/details/gjrvbqhwo.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fktsv.cn/Article/details/garvwzacv.sHtML

[T18] Swift：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gpuhducim.sHtML

"值: \(b)"
来源：http://www.share.epnwcf.com/Article/details/gvapqheiw.sHtML

[T19] Swift：可选绑定
来源：http://m.share.epnwcf.com/Article/details/guotmugic.sHtML

if let n = opt { print(n) }
来源：http://blog.fktsv.cn/Article/details/gckztrvet.sHtML

[T20] Swift：数组操作
来源：http://read.share.sjlbkw.cn/Article/details/gvqhcmikw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.sjlbkw.cn/Article/details/gghtzdzkz.sHtML

[T21] Swift：遍历
来源：http://wap.epnwcf.com/Article/details/ghusbauiq.sHtML

for x in a { print(x) }
来源：http://blog.sjlbkw.cn/Article/details/gcehoocvw.sHtML

[T22] Swift：字典
来源：http://www.m.share.tarul.cn/Article/details/ghqrmlefq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/gdztjngcx.sHtML

[T23] Swift：函数
来源：http://baike.fktsv.cn/Article/details/gnmmzrhuv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gwhluuniq.sHtML

[T24] Swift：闭包
来源：http://mobile.vehdjk.com/Article/details/gggmsloxq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gtucnpqxp.sHtML

[T25] Swift：结构体
来源：http://www.m.share.vehdjk.com/Article/details/gkbcgrymi.sHtML

struct P { var x: Int }
来源：http://m.share.yfazqb.com/Article/details/gobssawmc.sHtML

[T26] Swift：类与重写
来源：http://m.share.fktsv.cn/Article/details/gqvnnxwyk.sHtML

class A: Base { override func f() {} }
来源：http://baike.tarul.cn/Article/details/ghccjsrcw.sHtML

[T27] Swift：错误处理
来源：http://wap.vehdjk.com/Article/details/gyavfnmbw.sHtML

do { try f() } catch { print(error) }
来源：http://baike.sjlbkw.cn/Article/details/gsrdnxsqj.sHtML

[T28] Swift：枚举
来源：http://www.blog.tarul.cn/Article/details/gnvbryqni.sHtML

enum Color { case red, green }
来源：http://mobile.yfazqb.com/Article/details/guzufruef.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.vehdjk.com/Article/details/gziwocfxm.sHtML

guard let x = opt else { return }
来源：http://wap.bbcook.cn/Article/details/gzgnaxndf.sHtML

[T30] Swift：协议
来源：http://blog.bbcook.cn/Article/details/grztkethn.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.sjlbkw.cn/Article/details/gudmullih.sHtML

[T31] Lua：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gwvebrith.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/ghsuyavfz.sHtML

[T32] Lua：局部变量
来源：http://baike.yfazqb.com/Article/details/gtmgscyxj.sHtML

local a = 1
来源：http://mobile.vehdjk.com/Article/details/gjblumxhu.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.vehdjk.com/Article/details/gewjbogju.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.yfazqb.com/Article/details/gnldsyenp.sHtML

[T34] Lua：遍历表
来源：http://www.share.yfazqb.com/Article/details/gojwzqgow.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fktsv.cn/Article/details/gfnznfuoe.sHtML

[T35] Lua：字典表
来源：http://mobile.yfazqb.com/Article/details/gmvspyrvm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.yfazqb.com/Article/details/gasvuztra.sHtML

[T36] Lua：函数
来源：http://www.share.epnwcf.com/Article/details/gooqyetuz.sHtML

function add(a, b) return a + b end
来源：http://3g.tarul.cn/Article/details/groxlvofg.sHtML

[T37] Lua：字符串拼接
来源：http://baike.tarul.cn/Article/details/glaaaoheo.sHtML

"a" .. "b"
来源：http://www.blog.yfazqb.com/Article/details/ggvdilvxc.sHtML

[T38] Lua：条件
来源：http://3g.vehdjk.com/Article/details/gqcpodupt.sHtML

if x > 0 then print("正") end
来源：http://read.share.bbcook.cn/Article/details/guxbzneww.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fktsv.cn/Article/details/guarsvdny.sHtML

string.find(s, "%d+")
来源：http://www.share.sjlbkw.cn/Article/details/gziqbxhwk.sHtML

[T40] Lua：元表
来源：http://blog.fktsv.cn/Article/details/gompmuskd.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.sjlbkw.cn/Article/details/gxsaoxogv.sHtML

[T41] Perl：Hello World
来源：http://m.share.epnwcf.com/Article/details/glesouioh.sHtML

print "Hello\n";
来源：http://read.share.fktsv.cn/Article/details/gxmdpatpn.sHtML

[T42] Perl：变量类型
来源：http://read.share.fktsv.cn/Article/details/gmgvhukuw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fktsv.cn/Article/details/gsnvsbhsu.sHtML

[T43] Perl：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gjqhgpdjf.sHtML

"值: $a"
来源：http://blog.vehdjk.com/Article/details/gxrifklpm.sHtML

[T44] Perl：条件
来源：http://mobile.bbcook.cn/Article/details/gdplnrgok.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.tarul.cn/Article/details/gcqiwbcpl.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gdwgwmihv.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.tarul.cn/Article/details/ggsrpcvyn.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fktsv.cn/Article/details/gbisexddc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/gsldakech.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fktsv.cn/Article/details/gvdxauyso.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.yfazqb.com/Article/details/graujxago.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.tarul.cn/Article/details/gvsjqzyws.sHtML

$s =~ s/old/new/g;
来源：http://mobile.vehdjk.com/Article/details/gjkgyfxgz.sHtML

[T49] Perl：函数
来源：http://www.m.share.epnwcf.com/Article/details/gnvnjcgna.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/geterhaia.sHtML

[T50] Perl：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gcsijgily.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.vehdjk.com/Article/details/gfujdsdzm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.yfazqb.com/Article/details/gwknsagka.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gbvckrtcc.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/gbbojccyd.sHtML

[T52] Scala：变量
来源：http://blog.fktsv.cn/Article/details/grokubwed.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gwxmxjosj.sHtML

[T53] Scala：字符串插值
来源：http://blog.yfazqb.com/Article/details/gbauolfmn.sHtML

s"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/gszngwppr.sHtML

[T54] Scala：集合映射
来源：http://wap.tarul.cn/Article/details/gdnwjvugo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.vehdjk.com/Article/details/gwjpsmnpq.sHtML

[T55] Scala：集合过滤
来源：http://3g.tarul.cn/Article/details/gqwabytwo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.epnwcf.com/Article/details/gxmmchkzf.sHtML

[T56] Scala：样例类
来源：http://www.m.share.bbcook.cn/Article/details/ggdomhjmg.sHtML

case class User(name: String, age: Int)
来源：http://wap.tarul.cn/Article/details/gxyjaunlm.sHtML

[T57] Scala：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/gjjhotplc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.epnwcf.com/Article/details/gpcioiuqw.sHtML

[T58] Scala：函数定义
来源：http://wap.fktsv.cn/Article/details/gokmejwck.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.sjlbkw.cn/Article/details/gehzhcryz.sHtML

[T59] Scala：循环
来源：http://read.share.vehdjk.com/Article/details/gcsnjoeai.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gtsuonwbb.sHtML

[T60] Scala：折叠
来源：http://www.share.tarul.cn/Article/details/gfygdlqqm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/gizqrmeda.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjnnjnmci.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/ggdxjcrcu.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gdywowwpw.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.tarul.cn/Article/details/gsqnhmcuy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.vehdjk.com/Article/details/gvqlawjvx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/gyeflfhaw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.bbcook.cn/Article/details/gxiaahhoi.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.tarul.cn/Article/details/gfdotlmwe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.yfazqb.com/Article/details/gzxceacuf.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.sjlbkw.cn/Article/details/gipoesviu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.yfazqb.com/Article/details/gwqxxwjnh.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fktsv.cn/Article/details/gfcrgaaey.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/giwfcavvv.sHtML

[U06] Py：合并两个字典
来源：http://3g.vehdjk.com/Article/details/gvoyqjfcg.sHtML

{**a, **b}
来源：http://blog.fktsv.cn/Article/details/gzvylwsck.sHtML

[U07] Py：反转字典键值
来源：http://m.share.epnwcf.com/Article/details/gchawluqq.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/gqzwkrrvt.sHtML

[U08] Py：展平二维列表
来源：http://blog.yfazqb.com/Article/details/guglkgyuh.sHtML

[y for x in nested for y in x]
来源：http://read.share.vehdjk.com/Article/details/gzkjkwcfa.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fktsv.cn/Article/details/gfnbnopac.sHtML

max(d, key=d.get)
来源：http://baike.fktsv.cn/Article/details/gucksqvmv.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.bbcook.cn/Article/details/gwoyvynlo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.bbcook.cn/Article/details/gmhkklqzu.sHtML

[U11] Py：生成器表达式
来源：http://mobile.vehdjk.com/Article/details/gajuyvzjp.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.bbcook.cn/Article/details/grykvfgop.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.tarul.cn/Article/details/gllpcjmdj.sHtML

Counter(arr).most_common(3)
来源：http://3g.fktsv.cn/Article/details/gtqqbmndm.sHtML

[U13] Py：固定长度队列
来源：http://baike.yfazqb.com/Article/details/gvzjshjtb.sHtML

deque(maxlen=10)
来源：http://3g.fktsv.cn/Article/details/gocozupbz.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.bbcook.cn/Article/details/gilxpahvp.sHtML

defaultdict(list)
来源：http://blog.tarul.cn/Article/details/glhflsihf.sHtML

[U15] Py：高精度计时
来源：http://3g.fktsv.cn/Article/details/gyrkfkpjl.sHtML

t = time.perf_counter()
来源：http://www.m.share.vehdjk.com/Article/details/gmcujucna.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.yfazqb.com/Article/details/gmrksxeyp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fktsv.cn/Article/details/gfiobrqqk.sHtML


<!-- 参考信息 -->