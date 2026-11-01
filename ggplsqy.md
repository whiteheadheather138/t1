代发 wailian999

read -rp "请输入: " ans
来源：http://www.blog.vehdjk.com/Article/details/gupbcearb.sHtML

[R78] 交互式菜单
来源：http://wap.bbcook.cn/Article/details/gxjfohfnz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.bbcook.cn/Article/details/glusthuit.sHtML

[R79] 解析命令行选项
来源：http://read.share.tarul.cn/Article/details/gacrnxjxu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fktsv.cn/Article/details/gwmgkkpfj.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.vehdjk.com/Article/details/ggqwzdlgo.sHtML

time ./run.sh
来源：http://baike.bbcook.cn/Article/details/gwxfclnah.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gsiuajwwa.sHtML

S. C / C++ 专题
来源：http://blog.epnwcf.com/Article/details/gzoynenre.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfxizrbzp.sHtML

[S01] C：Hello World
来源：http://m.share.epnwcf.com/Article/details/gngdpvvev.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/gpcqclcry.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.epnwcf.com/Article/details/gwqiwheei.sHtML

[S02] C：变量与格式化输出
来源：http://wap.vehdjk.com/Article/details/gospsouyn.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.epnwcf.com/Article/details/gnjymlxvn.sHtML

[S03] C：读入整数
来源：http://3g.bbcook.cn/Article/details/gvzwatrsm.sHtML

int x; scanf("%d", &x);
来源：http://blog.vehdjk.com/Article/details/grsclonty.sHtML

[S04] C：字符串复制
来源：http://mobile.yfazqb.com/Article/details/guctqmgef.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.tarul.cn/Article/details/ggikfznwe.sHtML

[S05] C：字符串长度
来源：http://baike.tarul.cn/Article/details/gekshaecu.sHtML

strlen(s)
来源：http://3g.fktsv.cn/Article/details/gvdnnxjso.sHtML

[S06] C：字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gvhveswof.sHtML

strcmp(a, b) == 0
来源：http://m.share.yfazqb.com/Article/details/giupnzhiu.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.vehdjk.com/Article/details/gnwcewgki.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.vehdjk.com/Article/details/gvzaxauzl.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/goztqatbp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.tarul.cn/Article/details/grpnjozei.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/gzgxemhad.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.sjlbkw.cn/Article/details/gfotsccul.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/gnqjuzxxa.sHtML

int *p = &a;  *p = 5;
来源：http://blog.bbcook.cn/Article/details/gqnrzxyhx.sHtML

[S11] C：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gxfzfrcqj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.bbcook.cn/Article/details/gkkkrvuiy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.tarul.cn/Article/details/gvkckcejj.sHtML

fclose(f);
来源：http://3g.bbcook.cn/Article/details/gdncmhfwt.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/gzepphuqj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.yfazqb.com/Article/details/gclsptvuh.sHtML

[S13] C：宏定义
来源：http://www.share.tarul.cn/Article/details/goywvtlzp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.vehdjk.com/Article/details/ggxkwnjxx.sHtML

[S14] C：枚举
来源：http://3g.epnwcf.com/Article/details/gmkzvwfac.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fktsv.cn/Article/details/gxtywpuqe.sHtML

[S15] C：类型转换
来源：http://www.share.fktsv.cn/Article/details/gmqjlljcr.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpwedqeu.sHtML

[S16] C：位操作置位
来源：http://3g.yfazqb.com/Article/details/ggplvxrnw.sHtML

x |= (1 << 3);
来源：http://read.share.vehdjk.com/Article/details/gshoqhygm.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.tarul.cn/Article/details/gyoutlxta.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.epnwcf.com/Article/details/gotxcrtai.sHtML

[S18] C：命令行参数
来源：http://read.share.yfazqb.com/Article/details/gxjhmkxaz.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/gyvfxozvg.sHtML

[S19] C：快速排序
来源：http://read.share.sjlbkw.cn/Article/details/gjuyubatm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/gbzazodhv.sHtML

[S20] C：二分查找
来源：http://baike.vehdjk.com/Article/details/gjbjmovxu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/grnaokqqi.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fktsv.cn/Article/details/gfiykwbwx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fktsv.cn/Article/details/gxsjbuzho.sHtML

[S22] C：字符串转数字
来源：http://www.blog.sjlbkw.cn/Article/details/gnfpckfiw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.sjlbkw.cn/Article/details/gacpxopkz.sHtML

[S23] C：随机数
来源：http://m.share.tarul.cn/Article/details/gxtkrdbjq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.epnwcf.com/Article/details/ggtzyapvp.sHtML

[S24] C：获取本地时间
来源：http://baike.epnwcf.com/Article/details/glohpydqj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.yfazqb.com/Article/details/gtxzjrqgl.sHtML

[S25] C：内存拷贝
来源：http://3g.vehdjk.com/Article/details/gsfmefjko.sHtML

memcpy(dst, src, n);
来源：http://wap.vehdjk.com/Article/details/gttdmnmmp.sHtML

[S26] C：内存清零
来源：http://www.m.share.yfazqb.com/Article/details/gkuaoltsd.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gsxusaxhy.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gqkxkvmqo.sHtML

const double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gsjmrcldo.sHtML

[S28] C：静态变量
来源：http://3g.sjlbkw.cn/Article/details/gwfwkkwzj.sHtML

static int counter = 0;
来源：http://blog.yfazqb.com/Article/details/gtfaajviu.sHtML

[S29] C：变参函数
来源：http://www.share.bbcook.cn/Article/details/gtvnzdonv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.vehdjk.com/Article/details/gbmtaxdga.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/gjpzqdnft.sHtML

#ifndef X_H
来源：http://www.share.epnwcf.com/Article/details/gaxkomwzq.sHtML

#define X_H
来源：http://mobile.fktsv.cn/Article/details/gbazhiive.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/gbasscqbz.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gpccmjtvb.sHtML

#include <iostream>
来源：http://blog.yfazqb.com/Article/details/gblapbolv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.epnwcf.com/Article/details/gvnqqgedk.sHtML

[S32] C++：字符串
来源：http://mobile.fktsv.cn/Article/details/gjuegvljt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.bbcook.cn/Article/details/gguucgbye.sHtML

[S33] C++：vector 增删
来源：http://www.share.sjlbkw.cn/Article/details/gpfwldjur.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.vehdjk.com/Article/details/gvhjadijg.sHtML

[S34] C++：遍历 vector
来源：http://blog.yfazqb.com/Article/details/gnoutfujm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.bbcook.cn/Article/details/ghhausmpm.sHtML

[S35] C++：map
来源：http://read.share.vehdjk.com/Article/details/gfdxjsqdb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gbrnzhcfc.sHtML

[S36] C++：unordered_map
来源：http://www.share.vehdjk.com/Article/details/gawngbahk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gafvacdwa.sHtML

[S37] C++：set
来源：http://read.share.fktsv.cn/Article/details/gojqhbcqr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.yfazqb.com/Article/details/gojcewvgl.sHtML

[S38] C++：排序
来源：http://blog.yfazqb.com/Article/details/gllxstkwy.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/gymwhabxj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/grufeftuj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.vehdjk.com/Article/details/ghegivjtq.sHtML

[S40] C++：查找元素
来源：http://mobile.sjlbkw.cn/Article/details/gkollnhic.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.yfazqb.com/Article/details/gibzxudrs.sHtML

[S41] C++：类与构造函数
来源：http://www.share.epnwcf.com/Article/details/gvcgjdqtg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.epnwcf.com/Article/details/gelcqwrhp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.tarul.cn/Article/details/glsjacwsz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gljucpayl.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/grtwdhtnz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.tarul.cn/Article/details/gqvfqofig.sHtML

[S44] C++：引用传参
来源：http://baike.fktsv.cn/Article/details/gqlvvdoxs.sHtML

void inc(int &x) { ++x; }
来源：http://baike.yfazqb.com/Article/details/gftgntyfe.sHtML

[S45] C++：lambda
来源：http://blog.fktsv.cn/Article/details/gngtxdcdl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.vehdjk.com/Article/details/gdivrydhp.sHtML

[S46] C++：函数模板
来源：http://www.share.fktsv.cn/Article/details/gvppauhxf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/gvzlkbque.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.yfazqb.com/Article/details/goolrfvum.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.tarul.cn/Article/details/gmsgdeqfa.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gflxreyrz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.sjlbkw.cn/Article/details/gqhrsfxog.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/ghprzynof.sHtML

[S49] C++：写文件
来源：http://blog.epnwcf.com/Article/details/gaxhattsc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.epnwcf.com/Article/details/gfhpeelrz.sHtML

[S50] C++：格式化数字
来源：http://www.share.fktsv.cn/Article/details/gsrbcdelr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/gezswxyis.sHtML

[S51] C++：显式类型转换
来源：http://wap.tarul.cn/Article/details/gnfrgmfcv.sHtML

static_cast<double>(a) / b
来源：http://3g.fktsv.cn/Article/details/giqlpkcna.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.epnwcf.com/Article/details/gxclucwvr.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gxfhfttth.sHtML

[S53] C++：移动语义
来源：http://baike.bbcook.cn/Article/details/gxcrzepnz.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.bbcook.cn/Article/details/gcinowezi.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/gcnkfdmzz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.bbcook.cn/Article/details/gvtenohka.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gnycdmdjo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.tarul.cn/Article/details/gstcngzcb.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/gzhzlkmcn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.bbcook.cn/Article/details/ggibezuqo.sHtML

[S57] C++：编译期常量
来源：http://www.share.sjlbkw.cn/Article/details/gajqtmkgr.sHtML

constexpr int N = 10;
来源：http://www.share.epnwcf.com/Article/details/girvzokko.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gwtkjidqx.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.vehdjk.com/Article/details/gnlnjjeku.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/gwzbtrjlz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.yfazqb.com/Article/details/gvcjinhhh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.vehdjk.com/Article/details/gwrctwezc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.yfazqb.com/Article/details/gzlgtujte.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gnrbbfibr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.bbcook.cn/Article/details/ghutachax.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxotdkahq.sHtML

[T01] Kotlin：Hello World
来源：http://wap.vehdjk.com/Article/details/ghwjzyllt.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gnkhhagvp.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/goofkbmga.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/ggubuzqrz.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gbgbiyvvu.sHtML

"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/gkppibvod.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/gikgswkth.sHtML

val n: String? = null;  n?.length
来源：http://m.share.tarul.cn/Article/details/gpjdigrwj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.tarul.cn/Article/details/gpkjerjrn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gaxtmmcmq.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fktsv.cn/Article/details/gvntaixul.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.sjlbkw.cn/Article/details/ggtfyravj.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fktsv.cn/Article/details/gexwnfquj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gnpwamwwi.sHtML

[T08] Kotlin：数据类
来源：http://blog.vehdjk.com/Article/details/gdmoiqkbp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.bbcook.cn/Article/details/ggynvqqnt.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.epnwcf.com/Article/details/gmjrywsry.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/giyggjymm.sHtML

[T10] Kotlin：默认参数
来源：http://blog.bbcook.cn/Article/details/gpwozvbnn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.vehdjk.com/Article/details/gtcctxvow.sHtML

[T11] Kotlin：协程
来源：http://m.share.epnwcf.com/Article/details/guzpmxyrl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.yfazqb.com/Article/details/gkugktcpu.sHtML

[T12] Kotlin：解构声明
来源：http://blog.bbcook.cn/Article/details/guebkwsnm.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.yfazqb.com/Article/details/guuqapnfp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.tarul.cn/Article/details/goiplgotn.sHtML

val m = mapOf("a" to 1)
来源：http://baike.tarul.cn/Article/details/glhsaeekk.sHtML

[T14] Kotlin：循环
来源：http://wap.tarul.cn/Article/details/gvgshgxhd.sHtML

for (i in 1..10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gnenojwdw.sHtML

[T15] Kotlin：接口
来源：http://read.share.yfazqb.com/Article/details/gpceohydg.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.vehdjk.com/Article/details/gpxuposuw.sHtML

[T16] Swift：Hello World
来源：http://3g.bbcook.cn/Article/details/grjtsdogw.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/ggjkahiky.sHtML

[T17] Swift：变量与常量
来源：http://www.share.bbcook.cn/Article/details/gpvtddkga.sHtML

var a = 1;  let b = 2
来源：http://mobile.yfazqb.com/Article/details/gthuxcegu.sHtML

[T18] Swift：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gpchbztdy.sHtML

"值: \(b)"
来源：http://m.share.epnwcf.com/Article/details/giapbarkf.sHtML

[T19] Swift：可选绑定
来源：http://wap.yfazqb.com/Article/details/gjromcnjd.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/gzlbtdnkl.sHtML

[T20] Swift：数组操作
来源：http://www.share.epnwcf.com/Article/details/gvbnoakfj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fktsv.cn/Article/details/gudapydap.sHtML

[T21] Swift：遍历
来源：http://wap.sjlbkw.cn/Article/details/gkjklirte.sHtML

for x in a { print(x) }
来源：http://m.share.yfazqb.com/Article/details/gifcpoxpo.sHtML

[T22] Swift：字典
来源：http://www.share.sjlbkw.cn/Article/details/gpbcimlmw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.tarul.cn/Article/details/gxemkldsu.sHtML

[T23] Swift：函数
来源：http://www.m.share.fktsv.cn/Article/details/grzatfxox.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.epnwcf.com/Article/details/gshudvywe.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzanwgir.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.epnwcf.com/Article/details/gmrjrqsnh.sHtML

[T25] Swift：结构体
来源：http://read.share.fktsv.cn/Article/details/gerojusup.sHtML

struct P { var x: Int }
来源：http://mobile.yfazqb.com/Article/details/gqjvnxkjn.sHtML

[T26] Swift：类与重写
来源：http://www.share.bbcook.cn/Article/details/gpuebpiko.sHtML

class A: Base { override func f() {} }
来源：http://read.share.sjlbkw.cn/Article/details/ggeaxjzvs.sHtML

[T27] Swift：错误处理
来源：http://m.share.epnwcf.com/Article/details/gndzaiesp.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fktsv.cn/Article/details/gssyuplci.sHtML

[T28] Swift：枚举
来源：http://wap.vehdjk.com/Article/details/glvofxrgd.sHtML

enum Color { case red, green }
来源：http://www.blog.bbcook.cn/Article/details/gqsnrovqv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.yfazqb.com/Article/details/gfukhaaxe.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/gjpgctyio.sHtML

[T30] Swift：协议
来源：http://read.share.yfazqb.com/Article/details/gabgvnawi.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.bbcook.cn/Article/details/gmwfkovrw.sHtML

[T31] Lua：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gqlctbsiz.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/giiqtfkro.sHtML

[T32] Lua：局部变量
来源：http://wap.fktsv.cn/Article/details/gcizkulsk.sHtML

local a = 1
来源：http://read.share.sjlbkw.cn/Article/details/gqeciaxef.sHtML

[T33] Lua：表（数组）
来源：http://wap.epnwcf.com/Article/details/gaxtktiei.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.vehdjk.com/Article/details/gzazdsbqc.sHtML

[T34] Lua：遍历表
来源：http://www.share.vehdjk.com/Article/details/gkobgonck.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fktsv.cn/Article/details/gjfhjfobm.sHtML

[T35] Lua：字典表
来源：http://read.share.yfazqb.com/Article/details/guheajism.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gaygvqkvt.sHtML

[T36] Lua：函数
来源：http://baike.bbcook.cn/Article/details/gqdbuorcy.sHtML

function add(a, b) return a + b end
来源：http://blog.sjlbkw.cn/Article/details/gkysptost.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/grkevyvxb.sHtML

"a" .. "b"
来源：http://m.share.fktsv.cn/Article/details/gjinuyvnn.sHtML

[T38] Lua：条件
来源：http://wap.vehdjk.com/Article/details/gwoviyknw.sHtML

if x > 0 then print("正") end
来源：http://mobile.fktsv.cn/Article/details/gwaefjcvd.sHtML

[T39] Lua：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gvsvffrod.sHtML

string.find(s, "%d+")
来源：http://blog.sjlbkw.cn/Article/details/glksoegai.sHtML

[T40] Lua：元表
来源：http://www.share.yfazqb.com/Article/details/gmpiywpmu.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.sjlbkw.cn/Article/details/gjcjihsex.sHtML

[T41] Perl：Hello World
来源：http://read.share.vehdjk.com/Article/details/gqxiohexu.sHtML

print "Hello\n";
来源：http://www.share.bbcook.cn/Article/details/ghelaprcl.sHtML

[T42] Perl：变量类型
来源：http://read.share.vehdjk.com/Article/details/gysjzylba.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.vehdjk.com/Article/details/ghofpjrla.sHtML

[T43] Perl：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gmjvnspvl.sHtML

"值: $a"
来源：http://baike.sjlbkw.cn/Article/details/gazjuhvxx.sHtML

[T44] Perl：条件
来源：http://wap.bbcook.cn/Article/details/gqoohxnlk.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fktsv.cn/Article/details/gurempknd.sHtML

[T45] Perl：数组遍历
来源：http://baike.bbcook.cn/Article/details/gtaxbmapr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.yfazqb.com/Article/details/gnqivktpm.sHtML

[T46] Perl：哈希操作
来源：http://www.share.tarul.cn/Article/details/ggbjcxfpk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.vehdjk.com/Article/details/gksouvusf.sHtML

[T47] Perl：正则捕获
来源：http://m.share.sjlbkw.cn/Article/details/gpkecbxqr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.yfazqb.com/Article/details/gprdgriew.sHtML

[T48] Perl：正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gwamxmiys.sHtML

$s =~ s/old/new/g;
来源：http://www.share.bbcook.cn/Article/details/gztngwtmp.sHtML

[T49] Perl：函数
来源：http://wap.sjlbkw.cn/Article/details/gifdkqzaa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/glwkfxqud.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gjgelidei.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.vehdjk.com/Article/details/gdncotvvg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fktsv.cn/Article/details/gqwguphlg.sHtML

[T51] Scala：Hello World
来源：http://wap.tarul.cn/Article/details/gedhfmawx.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gpgwjzesz.sHtML

[T52] Scala：变量
来源：http://m.share.tarul.cn/Article/details/gxmqrkibs.sHtML

val a = 1;  var b = 2
来源：http://www.share.tarul.cn/Article/details/gloitfaoi.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gvpurpqip.sHtML

s"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gzrbhwjue.sHtML

[T54] Scala：集合映射
来源：http://wap.fktsv.cn/Article/details/gmficeqog.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fktsv.cn/Article/details/gkvdjvhmy.sHtML

[T55] Scala：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gsggfgdxo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.sjlbkw.cn/Article/details/gzyqsxyhr.sHtML

[T56] Scala：样例类
来源：http://blog.bbcook.cn/Article/details/ggyfaomny.sHtML

case class User(name: String, age: Int)
来源：http://mobile.epnwcf.com/Article/details/gpyckwnzi.sHtML

[T57] Scala：模式匹配
来源：http://baike.yfazqb.com/Article/details/gdtxuuqmw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.tarul.cn/Article/details/glwimfukr.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/gmqpbdyte.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.vehdjk.com/Article/details/gujzklvov.sHtML

[T59] Scala：循环
来源：http://mobile.tarul.cn/Article/details/gvujivdxf.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fktsv.cn/Article/details/gphsrfxby.sHtML

[T60] Scala：折叠
来源：http://mobile.tarul.cn/Article/details/golilsifx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.bbcook.cn/Article/details/gvuixngvv.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gknipigff.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.bbcook.cn/Article/details/geaobzgpu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gnvkyqrzq.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/gikpkdicy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.sjlbkw.cn/Article/details/ggxhenqld.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.epnwcf.com/Article/details/gwcytnrlc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fktsv.cn/Article/details/gsrmpzijs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.sjlbkw.cn/Article/details/ggiylkgtg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.vehdjk.com/Article/details/gyaxbhrfk.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fktsv.cn/Article/details/gjyxncjed.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.vehdjk.com/Article/details/gjuqzpjcd.sHtML

[U05] Py：列表去重且保序
来源：http://baike.vehdjk.com/Article/details/gbyduzzsx.sHtML

list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gsxdjvnst.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.bbcook.cn/Article/details/gpfrpxtge.sHtML

{**a, **b}
来源：http://wap.tarul.cn/Article/details/gutybxgse.sHtML

[U07] Py：反转字典键值
来源：http://blog.vehdjk.com/Article/details/goanfigvo.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.vehdjk.com/Article/details/gclojpyfg.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.yfazqb.com/Article/details/gevokvubc.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.sjlbkw.cn/Article/details/gnepxmkjz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.vehdjk.com/Article/details/gipbklgxl.sHtML

max(d, key=d.get)
来源：http://3g.yfazqb.com/Article/details/gzppawtyg.sHtML

[U10] Py：按值排序字典
来源：http://blog.vehdjk.com/Article/details/glkovddys.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.bbcook.cn/Article/details/gldvfvokx.sHtML

[U11] Py：生成器表达式
来源：http://mobile.epnwcf.com/Article/details/guskpayds.sHtML

(x * 2 for x in arr)
来源：http://wap.epnwcf.com/Article/details/gqaxmkdoa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.bbcook.cn/Article/details/gizfxprhw.sHtML

Counter(arr).most_common(3)
来源：http://blog.vehdjk.com/Article/details/gofguhpou.sHtML

[U13] Py：固定长度队列
来源：http://m.share.bbcook.cn/Article/details/gyljxrujo.sHtML

deque(maxlen=10)
来源：http://read.share.fktsv.cn/Article/details/gslprevgv.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.epnwcf.com/Article/details/gtgnxbxwg.sHtML

defaultdict(list)
来源：http://www.blog.bbcook.cn/Article/details/gzqjyelmu.sHtML

[U15] Py：高精度计时
来源：http://www.blog.yfazqb.com/Article/details/goiothkkf.sHtML

t = time.perf_counter()
来源：http://3g.epnwcf.com/Article/details/glwcznucd.sHtML

[U16] Py：命令行参数解析
来源：http://wap.tarul.cn/Article/details/gfsrnvhmz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.tarul.cn/Article/details/gsadywwvf.sHtML

[U17] Py：初始化日志
来源：http://baike.bbcook.cn/Article/details/gqcpieoyr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.yfazqb.com/Article/details/gvskjoses.sHtML

[U18] Py：预编译正则
来源：http://3g.sjlbkw.cn/Article/details/gvwzyzrmr.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/gsjbhotci.sHtML


<!-- 参考信息 -->