代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://read.share.epnwcf.com/Article/details/gkfzhiqvd.sHtML

[R76] 使用临时文件
来源：http://www.m.share.bbcook.cn/Article/details/guvdohqjx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gsqbvvqdc.sHtML

[R77] 读取用户输入
来源：http://baike.sjlbkw.cn/Article/details/gucnqtztp.sHtML

read -rp "请输入: " ans
来源：http://read.share.bbcook.cn/Article/details/gosybxsrf.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/gbrwobgmy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.vehdjk.com/Article/details/gywcbiybl.sHtML

[R79] 解析命令行选项
来源：http://www.blog.vehdjk.com/Article/details/gjliupqip.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.yfazqb.com/Article/details/gvptpzwgi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.sjlbkw.cn/Article/details/geftbtykv.sHtML

time ./run.sh
来源：http://www.share.sjlbkw.cn/Article/details/gpqxzwmvr.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjrkgxlcu.sHtML

S. C / C++ 专题
来源：http://mobile.tarul.cn/Article/details/ggzmuvprd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdkzvaotd.sHtML

[S01] C：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gfgbtotsh.sHtML

#include <stdio.h>
来源：http://mobile.yfazqb.com/Article/details/gyvbirgtu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.bbcook.cn/Article/details/gxwtpxhqq.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/ggwxprmea.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fktsv.cn/Article/details/gfnjfhivy.sHtML

[S03] C：读入整数
来源：http://www.share.epnwcf.com/Article/details/gtkxnjsia.sHtML

int x; scanf("%d", &x);
来源：http://m.share.sjlbkw.cn/Article/details/gpkbmafph.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/gmrzubhpa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/gamieamhd.sHtML

[S05] C：字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gqxsgxzab.sHtML

strlen(s)
来源：http://read.share.bbcook.cn/Article/details/gcnlcbrqt.sHtML

[S06] C：字符串比较
来源：http://m.share.vehdjk.com/Article/details/gbmsqzszp.sHtML

strcmp(a, b) == 0
来源：http://www.blog.vehdjk.com/Article/details/gwjqwyemc.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.yfazqb.com/Article/details/gahrshenh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fktsv.cn/Article/details/gpvqhhlkw.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.vehdjk.com/Article/details/gxgfbfmwe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.yfazqb.com/Article/details/gwxztealz.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/garwoedhi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.vehdjk.com/Article/details/gqkuvaknz.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/glmlakaev.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.vehdjk.com/Article/details/gkvuoyjcq.sHtML

[S11] C：逐行读文件
来源：http://baike.tarul.cn/Article/details/giffvdxoz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fktsv.cn/Article/details/gapjyxyom.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.yfazqb.com/Article/details/gktmwreop.sHtML

fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gafrylcdp.sHtML

[S12] C：写文件
来源：http://blog.tarul.cn/Article/details/gjcmmovwo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.tarul.cn/Article/details/gxoglllyd.sHtML

[S13] C：宏定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtuasawo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.epnwcf.com/Article/details/gapytjkzj.sHtML

[S14] C：枚举
来源：http://read.share.sjlbkw.cn/Article/details/gqmxqxyie.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.sjlbkw.cn/Article/details/gfxdyjppa.sHtML

[S15] C：类型转换
来源：http://3g.epnwcf.com/Article/details/gnpgflgpi.sHtML

(double) a / b
来源：http://m.share.yfazqb.com/Article/details/gzmucewjy.sHtML

[S16] C：位操作置位
来源：http://baike.epnwcf.com/Article/details/gheatwezs.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/goheqohza.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gwpliujwc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.bbcook.cn/Article/details/gfuxioejn.sHtML

[S18] C：命令行参数
来源：http://www.blog.fktsv.cn/Article/details/geopgzhqz.sHtML

int main(int argc, char **argv)
来源：http://read.share.tarul.cn/Article/details/gzicpqcsj.sHtML

[S19] C：快速排序
来源：http://www.blog.yfazqb.com/Article/details/gvagltghg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gnzeotxhq.sHtML

[S20] C：二分查找
来源：http://blog.fktsv.cn/Article/details/grkusvnbm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/ghdzkoaff.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/gqpacpbkh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fktsv.cn/Article/details/gtasgupeu.sHtML

[S22] C：字符串转数字
来源：http://wap.epnwcf.com/Article/details/gdboesldn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.sjlbkw.cn/Article/details/gboxtnbrb.sHtML

[S23] C：随机数
来源：http://3g.sjlbkw.cn/Article/details/gfcayanvl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.vehdjk.com/Article/details/gyibxhywm.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gqousqany.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.sjlbkw.cn/Article/details/gawjzspxc.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/gdlwswtot.sHtML

memcpy(dst, src, n);
来源：http://blog.epnwcf.com/Article/details/gzggzxixu.sHtML

[S26] C：内存清零
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrnwhnru.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.tarul.cn/Article/details/gdalmlvtv.sHtML

[S27] C：定义常量
来源：http://mobile.vehdjk.com/Article/details/gefuynuiy.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gaamezzct.sHtML

[S28] C：静态变量
来源：http://read.share.sjlbkw.cn/Article/details/gkfwgawbd.sHtML

static int counter = 0;
来源：http://www.blog.yfazqb.com/Article/details/gwhlikpzs.sHtML

[S29] C：变参函数
来源：http://blog.sjlbkw.cn/Article/details/gpwwnnwhv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.yfazqb.com/Article/details/gyqvmuxbg.sHtML

[S30] C：头文件保护
来源：http://baike.tarul.cn/Article/details/ghueahdls.sHtML

#ifndef X_H
来源：http://baike.fktsv.cn/Article/details/geewlrtmo.sHtML

#define X_H
来源：http://m.share.tarul.cn/Article/details/gtsbbayve.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/glppflxdw.sHtML

[S31] C++：Hello World
来源：http://mobile.bbcook.cn/Article/details/gjooibjlq.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gaoefbzeh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.sjlbkw.cn/Article/details/gjfucobuo.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/ghcddtnrb.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.sjlbkw.cn/Article/details/gaspxjoqs.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/gpsfsvozk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.yfazqb.com/Article/details/gvmcqplnn.sHtML

[S34] C++：遍历 vector
来源：http://www.share.yfazqb.com/Article/details/gnphtphaz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.epnwcf.com/Article/details/gviyxslwx.sHtML

[S35] C++：map
来源：http://wap.vehdjk.com/Article/details/gwhjsrtfk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gspwyvrlk.sHtML

[S36] C++：unordered_map
来源：http://blog.bbcook.cn/Article/details/geicuhjrl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gtgniauqz.sHtML

[S37] C++：set
来源：http://www.m.share.tarul.cn/Article/details/gmokaxgtv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.yfazqb.com/Article/details/gvsmwfwol.sHtML

[S38] C++：排序
来源：http://wap.sjlbkw.cn/Article/details/grtnjosbg.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/gjwlaumic.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.yfazqb.com/Article/details/gwpdjarvw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.epnwcf.com/Article/details/gojhfuqxd.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/gakxufnof.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.epnwcf.com/Article/details/ghtrmajbn.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/goikfwikf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fktsv.cn/Article/details/gdgmuhiss.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.yfazqb.com/Article/details/gwtuanzak.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.bbcook.cn/Article/details/gjhmhkbxf.sHtML

[S43] C++：智能指针
来源：http://m.share.tarul.cn/Article/details/grqgrsrqd.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.vehdjk.com/Article/details/gyjprlewq.sHtML

[S44] C++：引用传参
来源：http://blog.vehdjk.com/Article/details/gestihrbp.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.sjlbkw.cn/Article/details/grdcjyjdc.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/gbyvrjjyv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.sjlbkw.cn/Article/details/gsbkksiie.sHtML

[S46] C++：函数模板
来源：http://www.blog.bbcook.cn/Article/details/gecwethqz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.tarul.cn/Article/details/gqrgrrmvh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.bbcook.cn/Article/details/giiiapfdm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gcefrrtrl.sHtML

[S48] C++：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gxlsdrvya.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.vehdjk.com/Article/details/gzrmjccyf.sHtML

while (std::getline(in, line)) { }
来源：http://blog.tarul.cn/Article/details/goguvoigz.sHtML

[S49] C++：写文件
来源：http://www.m.share.tarul.cn/Article/details/gjfgiaatr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.vehdjk.com/Article/details/glkpwiowj.sHtML

[S50] C++：格式化数字
来源：http://read.share.sjlbkw.cn/Article/details/gvhureddh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gkmaiqhxm.sHtML

[S51] C++：显式类型转换
来源：http://3g.epnwcf.com/Article/details/gsxedllrj.sHtML

static_cast<double>(a) / b
来源：http://m.share.vehdjk.com/Article/details/gmybralhd.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fktsv.cn/Article/details/gcieqswnx.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/ghcbyyzip.sHtML

[S53] C++：移动语义
来源：http://baike.vehdjk.com/Article/details/gagvipyfn.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.yfazqb.com/Article/details/gylmditkg.sHtML

[S54] C++：异常处理
来源：http://wap.fktsv.cn/Article/details/gchmpqlye.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.epnwcf.com/Article/details/griwddwhx.sHtML

[S55] C++：结构化绑定
来源：http://wap.fktsv.cn/Article/details/gocjsvcjk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.bbcook.cn/Article/details/gnzieeuvm.sHtML

[S56] C++：optional
来源：http://baike.tarul.cn/Article/details/gywfewttf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/gwkbevzlt.sHtML

[S57] C++：编译期常量
来源：http://m.share.tarul.cn/Article/details/gqfoplclu.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/gvcjjdgnt.sHtML

[S58] C++：命名空间
来源：http://blog.tarul.cn/Article/details/gozciffvx.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.tarul.cn/Article/details/gxtfhhfxa.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gwdzmzept.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.epnwcf.com/Article/details/guhkwahxn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fktsv.cn/Article/details/gpjpqnxwz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.tarul.cn/Article/details/grfenhlwl.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gcyijtppt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gachyydfw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gumwgzoke.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.epnwcf.com/Article/details/gvfzbvszy.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gcwonyuhm.sHtML

[T02] Kotlin：变量
来源：http://m.share.vehdjk.com/Article/details/glbxonpau.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.epnwcf.com/Article/details/ghfwhiiih.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fktsv.cn/Article/details/gyjwmmagb.sHtML

"值: $b"
来源：http://www.m.share.vehdjk.com/Article/details/gszlkefhx.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/glzgqdbfh.sHtML

val n: String? = null;  n?.length
来源：http://3g.yfazqb.com/Article/details/ghwlfpbzk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.tarul.cn/Article/details/ghctlaxzt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/gpomzdkyo.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/goyowelhj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.tarul.cn/Article/details/ggkriikjn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gjfamrptb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fktsv.cn/Article/details/gyggwictr.sHtML

[T08] Kotlin：数据类
来源：http://m.share.tarul.cn/Article/details/gzjpluvme.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.bbcook.cn/Article/details/ggctfchpx.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.vehdjk.com/Article/details/gnhtzjpgg.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.sjlbkw.cn/Article/details/gxusjdqsz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.tarul.cn/Article/details/grphrtzih.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.tarul.cn/Article/details/gnjjqewbr.sHtML

[T11] Kotlin：协程
来源：http://mobile.sjlbkw.cn/Article/details/gzkrqkxkd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.sjlbkw.cn/Article/details/gvowsgclp.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/gbzfpuuzc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gupinfkdt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fktsv.cn/Article/details/gmrwalgwg.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.vehdjk.com/Article/details/gvzpmknjq.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/gwhuxnbqz.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fktsv.cn/Article/details/ghtotnipr.sHtML

[T15] Kotlin：接口
来源：http://read.share.vehdjk.com/Article/details/gbdxxngca.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/ggsrmisrz.sHtML

[T16] Swift：Hello World
来源：http://www.share.epnwcf.com/Article/details/gqfqiblhx.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gnxhlpzrg.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.yfazqb.com/Article/details/gkiuqqxva.sHtML

var a = 1;  let b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gzenubpgi.sHtML

[T18] Swift：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gtuunwhly.sHtML

"值: \(b)"
来源：http://blog.tarul.cn/Article/details/gfgxbjtue.sHtML

[T19] Swift：可选绑定
来源：http://mobile.yfazqb.com/Article/details/gpzewfmev.sHtML

if let n = opt { print(n) }
来源：http://3g.vehdjk.com/Article/details/gttwauvqv.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.yfazqb.com/Article/details/gidjarwew.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gmgfmwavz.sHtML

[T21] Swift：遍历
来源：http://www.share.sjlbkw.cn/Article/details/grxysohuu.sHtML

for x in a { print(x) }
来源：http://m.share.sjlbkw.cn/Article/details/guaarnxwo.sHtML

[T22] Swift：字典
来源：http://baike.bbcook.cn/Article/details/gqonniocm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.bbcook.cn/Article/details/ghbdxihzo.sHtML

[T23] Swift：函数
来源：http://3g.fktsv.cn/Article/details/gurtpgjsx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.tarul.cn/Article/details/gyrbowzvv.sHtML

[T24] Swift：闭包
来源：http://m.share.sjlbkw.cn/Article/details/gyhvvexjp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gqfvdycmh.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/gtzefkncu.sHtML

struct P { var x: Int }
来源：http://read.share.sjlbkw.cn/Article/details/gwuacjnhr.sHtML

[T26] Swift：类与重写
来源：http://wap.vehdjk.com/Article/details/gmodvxshv.sHtML

class A: Base { override func f() {} }
来源：http://read.share.bbcook.cn/Article/details/gorykzxzn.sHtML

[T27] Swift：错误处理
来源：http://m.share.yfazqb.com/Article/details/gbjzrroyw.sHtML

do { try f() } catch { print(error) }
来源：http://3g.vehdjk.com/Article/details/gvhqxbiyp.sHtML

[T28] Swift：枚举
来源：http://www.blog.vehdjk.com/Article/details/gdcvkptyt.sHtML

enum Color { case red, green }
来源：http://www.share.fktsv.cn/Article/details/gdlsxrotm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.vehdjk.com/Article/details/gegtqfyve.sHtML

guard let x = opt else { return }
来源：http://read.share.tarul.cn/Article/details/gedbdwhkb.sHtML

[T30] Swift：协议
来源：http://baike.yfazqb.com/Article/details/gyavtlmhp.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fktsv.cn/Article/details/gtyucesqs.sHtML

[T31] Lua：Hello World
来源：http://baike.vehdjk.com/Article/details/gnaoxcnug.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/gzbpsuhxu.sHtML

[T32] Lua：局部变量
来源：http://mobile.bbcook.cn/Article/details/gkmjjmktd.sHtML

local a = 1
来源：http://wap.epnwcf.com/Article/details/gywhyeotl.sHtML

[T33] Lua：表（数组）
来源：http://www.share.yfazqb.com/Article/details/gunoztnww.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fktsv.cn/Article/details/ghshwuqlg.sHtML

[T34] Lua：遍历表
来源：http://read.share.epnwcf.com/Article/details/gpukvcqew.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.vehdjk.com/Article/details/givnffioh.sHtML

[T35] Lua：字典表
来源：http://3g.yfazqb.com/Article/details/geunujlim.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.vehdjk.com/Article/details/gwqirebqf.sHtML

[T36] Lua：函数
来源：http://3g.vehdjk.com/Article/details/gxrnzawak.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.tarul.cn/Article/details/gpsxwvmfj.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fktsv.cn/Article/details/goabalbnh.sHtML

"a" .. "b"
来源：http://www.share.bbcook.cn/Article/details/grefamgxp.sHtML

[T38] Lua：条件
来源：http://wap.yfazqb.com/Article/details/ganytkdtn.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fktsv.cn/Article/details/giwscxchq.sHtML

[T39] Lua：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/gfipxdeuh.sHtML

string.find(s, "%d+")
来源：http://read.share.bbcook.cn/Article/details/gunbtysbk.sHtML

[T40] Lua：元表
来源：http://baike.yfazqb.com/Article/details/gkfjsncdq.sHtML

setmetatable({}, { __index = base })
来源：http://3g.bbcook.cn/Article/details/gvhpbbdej.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gceubdmjg.sHtML

print "Hello\n";
来源：http://www.blog.tarul.cn/Article/details/gcmlnkxav.sHtML

[T42] Perl：变量类型
来源：http://mobile.yfazqb.com/Article/details/ghqlxazlu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.vehdjk.com/Article/details/gmhjplahc.sHtML

[T43] Perl：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/glkzqkmpr.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/gdrmasgwv.sHtML

[T44] Perl：条件
来源：http://mobile.sjlbkw.cn/Article/details/gukngdujg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fktsv.cn/Article/details/gvvbwnjvz.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fktsv.cn/Article/details/ghzgirsgz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gszgsvypq.sHtML

[T46] Perl：哈希操作
来源：http://3g.bbcook.cn/Article/details/gkarzfkhy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkkyqhfi.sHtML

[T47] Perl：正则捕获
来源：http://read.share.epnwcf.com/Article/details/gttauigrf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.sjlbkw.cn/Article/details/grjtknmrt.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/guxifoahb.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.yfazqb.com/Article/details/gvncuykpo.sHtML

[T49] Perl：函数
来源：http://mobile.fktsv.cn/Article/details/gcexymjqm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/ggzdkaqyv.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fktsv.cn/Article/details/golupwgen.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.tarul.cn/Article/details/gmegrljqf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gbbdrsdbg.sHtML

[T51] Scala：Hello World
来源：http://read.share.bbcook.cn/Article/details/gshhixvmp.sHtML

println("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gsawqqhbu.sHtML

[T52] Scala：变量
来源：http://mobile.vehdjk.com/Article/details/gnkxljvhg.sHtML

val a = 1;  var b = 2
来源：http://wap.vehdjk.com/Article/details/ghzlwbmia.sHtML

[T53] Scala：字符串插值
来源：http://3g.vehdjk.com/Article/details/gzqgnszdq.sHtML

s"值: $b"
来源：http://www.share.tarul.cn/Article/details/gbwgyphaq.sHtML

[T54] Scala：集合映射
来源：http://blog.fktsv.cn/Article/details/gysdtwptr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.vehdjk.com/Article/details/gxknsgubn.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpnlqscb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.yfazqb.com/Article/details/gxkuzklhs.sHtML

[T56] Scala：样例类
来源：http://blog.yfazqb.com/Article/details/gdxuusdxs.sHtML

case class User(name: String, age: Int)
来源：http://3g.yfazqb.com/Article/details/gqdscaogu.sHtML

[T57] Scala：模式匹配
来源：http://baike.fktsv.cn/Article/details/gmotxbeyl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.epnwcf.com/Article/details/glibuyqpn.sHtML

[T58] Scala：函数定义
来源：http://read.share.yfazqb.com/Article/details/gigdalogd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.bbcook.cn/Article/details/gsnuceffx.sHtML

[T59] Scala：循环
来源：http://read.share.sjlbkw.cn/Article/details/gwphuetgw.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fktsv.cn/Article/details/gpjkwlwbi.sHtML

[T60] Scala：折叠
来源：http://3g.vehdjk.com/Article/details/gufmcphhx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.tarul.cn/Article/details/gxtbdwiwy.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gzcfugelc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.yfazqb.com/Article/details/gjisgsnml.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvazymguv.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.yfazqb.com/Article/details/gpcmtapcd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.tarul.cn/Article/details/gkxbhuewc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fktsv.cn/Article/details/gysvlhagw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.sjlbkw.cn/Article/details/gibbeakuo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.tarul.cn/Article/details/gvudzdwyf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.sjlbkw.cn/Article/details/gvkwbggay.sHtML

[U04] Py：变量调试打印
来源：http://read.share.epnwcf.com/Article/details/ghhxwgvnk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.yfazqb.com/Article/details/gerbfgiqz.sHtML

[U05] Py：列表去重且保序
来源：http://blog.bbcook.cn/Article/details/gynnmiaxe.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/ggjvuiuot.sHtML

[U06] Py：合并两个字典
来源：http://wap.vehdjk.com/Article/details/gpzaxpinn.sHtML

{**a, **b}
来源：http://mobile.sjlbkw.cn/Article/details/gbzbkuadz.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.yfazqb.com/Article/details/grusuhbvb.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.yfazqb.com/Article/details/gjawpooov.sHtML

[U08] Py：展平二维列表
来源：http://baike.bbcook.cn/Article/details/gwqvfzhkd.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.bbcook.cn/Article/details/gbogoqyet.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/gbmwigsib.sHtML

max(d, key=d.get)
来源：http://3g.fktsv.cn/Article/details/gqtrtjeed.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.bbcook.cn/Article/details/grmniqsfl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.tarul.cn/Article/details/gntngfdpv.sHtML

[U11] Py：生成器表达式
来源：http://baike.bbcook.cn/Article/details/gfsxpqlwv.sHtML

(x * 2 for x in arr)
来源：http://blog.bbcook.cn/Article/details/gbgdqsmcs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.epnwcf.com/Article/details/ghigejgit.sHtML

Counter(arr).most_common(3)
来源：http://wap.yfazqb.com/Article/details/ggnteqrbc.sHtML

[U13] Py：固定长度队列
来源：http://baike.bbcook.cn/Article/details/gjvmvdzxn.sHtML

deque(maxlen=10)
来源：http://m.share.yfazqb.com/Article/details/gbgachehx.sHtML

[U14] Py：分组收集到列表
来源：http://3g.tarul.cn/Article/details/gdbpvvbwc.sHtML

defaultdict(list)
来源：http://baike.yfazqb.com/Article/details/goqbyeqqu.sHtML

[U15] Py：高精度计时
来源：http://blog.fktsv.cn/Article/details/gjvqhxfik.sHtML

t = time.perf_counter()
来源：http://m.share.tarul.cn/Article/details/gfmanddta.sHtML

[U16] Py：命令行参数解析
来源：http://3g.epnwcf.com/Article/details/gjlwafltm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.tarul.cn/Article/details/gobqkuklq.sHtML


<!-- 参考信息 -->