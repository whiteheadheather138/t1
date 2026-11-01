代发 wailian999

split -l 1000 big.log part_
来源：http://mobile.yfazqb.com/Article/details/ggdwzrruz.sHtML

[R74] 批量重命名
来源：http://mobile.bbcook.cn/Article/details/gftxemuvx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fktsv.cn/Article/details/gatwnwunt.sHtML

[R75] 导出环境变量
来源：http://baike.vehdjk.com/Article/details/gzrrqggzh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.vehdjk.com/Article/details/grbzgbpgc.sHtML

[R76] 使用临时文件
来源：http://blog.yfazqb.com/Article/details/ghftawfnw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gyqezdczj.sHtML

[R77] 读取用户输入
来源：http://3g.fktsv.cn/Article/details/gojwsyvka.sHtML

read -rp "请输入: " ans
来源：http://3g.tarul.cn/Article/details/gnxmapkek.sHtML

[R78] 交互式菜单
来源：http://3g.fktsv.cn/Article/details/gxxnkavvr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fktsv.cn/Article/details/ghoiilmus.sHtML

[R79] 解析命令行选项
来源：http://baike.vehdjk.com/Article/details/guifhwvbt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.sjlbkw.cn/Article/details/goxttnyin.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.tarul.cn/Article/details/gjfsiyxli.sHtML

time ./run.sh
来源：http://3g.epnwcf.com/Article/details/gtaoswymx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdhakathd.sHtML

S. C / C++ 专题
来源：http://www.share.tarul.cn/Article/details/ghfiqauag.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxptafxju.sHtML

[S01] C：Hello World
来源：http://read.share.yfazqb.com/Article/details/gkrtnbzca.sHtML

#include <stdio.h>
来源：http://mobile.yfazqb.com/Article/details/gliuyauer.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.bbcook.cn/Article/details/gqimmvtol.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/gjleszkii.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.vehdjk.com/Article/details/ghxfnnbbp.sHtML

[S03] C：读入整数
来源：http://www.blog.epnwcf.com/Article/details/gnucatmzs.sHtML

int x; scanf("%d", &x);
来源：http://mobile.tarul.cn/Article/details/gtzsgjthw.sHtML

[S04] C：字符串复制
来源：http://blog.bbcook.cn/Article/details/gugpmqomr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.vehdjk.com/Article/details/gjwanrkcg.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/gizvtwxyt.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/glxhvznsg.sHtML

[S06] C：字符串比较
来源：http://read.share.vehdjk.com/Article/details/gubhrzcje.sHtML

strcmp(a, b) == 0
来源：http://wap.vehdjk.com/Article/details/gpfenwiwd.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.epnwcf.com/Article/details/gwhabmrqd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.tarul.cn/Article/details/gzgyxpmyl.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.vehdjk.com/Article/details/gtgiofrfi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.bbcook.cn/Article/details/gltnkpmrv.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.sjlbkw.cn/Article/details/gqpbzgkvp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.bbcook.cn/Article/details/gkpgjhnft.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fktsv.cn/Article/details/grmeonkah.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fktsv.cn/Article/details/gfilamrwr.sHtML

[S11] C：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gwduxwxbx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.tarul.cn/Article/details/gkgnzpwea.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.sjlbkw.cn/Article/details/gdqgooimu.sHtML

fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gmdxutplp.sHtML

[S12] C：写文件
来源：http://wap.bbcook.cn/Article/details/gghfdhcsv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/gsdsqfmnn.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/gujquiwvi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.sjlbkw.cn/Article/details/gzqvzjvzd.sHtML

[S14] C：枚举
来源：http://www.share.vehdjk.com/Article/details/gzemodinr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.yfazqb.com/Article/details/gldvbwgzk.sHtML

[S15] C：类型转换
来源：http://wap.epnwcf.com/Article/details/gyrxalgqx.sHtML

(double) a / b
来源：http://m.share.epnwcf.com/Article/details/gnapurqoo.sHtML

[S16] C：位操作置位
来源：http://mobile.bbcook.cn/Article/details/gfdcwpaau.sHtML

x |= (1 << 3);
来源：http://baike.vehdjk.com/Article/details/gnzohyhvr.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gnwzoleze.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.bbcook.cn/Article/details/gmmsbakfs.sHtML

[S18] C：命令行参数
来源：http://blog.bbcook.cn/Article/details/guoudtpse.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/gqnkpopzl.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/glgthlmnp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gpykdtkim.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gbvbhbebc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gmjocajqs.sHtML

[S21] C：字符类别判断
来源：http://3g.vehdjk.com/Article/details/grxpunxrz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.sjlbkw.cn/Article/details/gentltvzp.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/gvvmdtkmz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.sjlbkw.cn/Article/details/gnfjsmgoy.sHtML

[S23] C：随机数
来源：http://www.m.share.vehdjk.com/Article/details/gzjzpvswx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.yfazqb.com/Article/details/guwplhjwg.sHtML

[S24] C：获取本地时间
来源：http://blog.bbcook.cn/Article/details/gbemhhmua.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.vehdjk.com/Article/details/gcvhoyzfk.sHtML

[S25] C：内存拷贝
来源：http://www.blog.epnwcf.com/Article/details/graosuxxq.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.yfazqb.com/Article/details/gckmmuupg.sHtML

[S26] C：内存清零
来源：http://mobile.vehdjk.com/Article/details/gygwqlesm.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/gzlhiridp.sHtML

[S27] C：定义常量
来源：http://blog.yfazqb.com/Article/details/geyuapcyf.sHtML

const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gvshmjcrh.sHtML

[S28] C：静态变量
来源：http://read.share.epnwcf.com/Article/details/gtaqqrvva.sHtML

static int counter = 0;
来源：http://m.share.fktsv.cn/Article/details/gkbfvrehv.sHtML

[S29] C：变参函数
来源：http://3g.vehdjk.com/Article/details/gjwvlsbov.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/gxkklwypa.sHtML

[S30] C：头文件保护
来源：http://www.share.bbcook.cn/Article/details/gtuxlmmts.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/gonlezpsy.sHtML

#define X_H
来源：http://baike.sjlbkw.cn/Article/details/gxnuygxau.sHtML

#endif
来源：http://wap.fktsv.cn/Article/details/grmmxbiny.sHtML

[S31] C++：Hello World
来源：http://www.share.vehdjk.com/Article/details/gddnjogoq.sHtML

#include <iostream>
来源：http://blog.yfazqb.com/Article/details/gbgzmesmw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.tarul.cn/Article/details/gtdvguaez.sHtML

[S32] C++：字符串
来源：http://www.m.share.yfazqb.com/Article/details/gmpiqpjew.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.sjlbkw.cn/Article/details/genskoofs.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.yfazqb.com/Article/details/gjxssbwoz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.vehdjk.com/Article/details/gbqhmsuuy.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.bbcook.cn/Article/details/gmzipzilg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.vehdjk.com/Article/details/ggqryhbdh.sHtML

[S35] C++：map
来源：http://www.share.epnwcf.com/Article/details/gmoxujnld.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gorpzxqev.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/glbddqahk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/glxtuzulf.sHtML

[S37] C++：set
来源：http://m.share.tarul.cn/Article/details/gaprxnekt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gmpscqoef.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gefheuvfz.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gqgdzhbsz.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/gikghxeye.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.bbcook.cn/Article/details/gcfexcwol.sHtML

[S40] C++：查找元素
来源：http://read.share.vehdjk.com/Article/details/gvkoibncl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.epnwcf.com/Article/details/gxfldpxjf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.vehdjk.com/Article/details/gvbttkctp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/gpriudvdp.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gcyrvayin.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.sjlbkw.cn/Article/details/glemmfnhu.sHtML

[S43] C++：智能指针
来源：http://wap.fktsv.cn/Article/details/gyhnqctxq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gaytwhreh.sHtML

[S44] C++：引用传参
来源：http://mobile.tarul.cn/Article/details/gfojhzhxx.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.tarul.cn/Article/details/gfqqgmhso.sHtML

[S45] C++：lambda
来源：http://www.blog.sjlbkw.cn/Article/details/gujgnpsnk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.yfazqb.com/Article/details/gphvxcxnr.sHtML

[S46] C++：函数模板
来源：http://blog.fktsv.cn/Article/details/gykssjccg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.yfazqb.com/Article/details/gxjouryvv.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.tarul.cn/Article/details/gyiiqimkk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.yfazqb.com/Article/details/gigfnrqqn.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gcqriiwro.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.vehdjk.com/Article/details/gnlpzlteo.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fktsv.cn/Article/details/gqbasmhfo.sHtML

[S49] C++：写文件
来源：http://m.share.yfazqb.com/Article/details/gcgmlgoah.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.epnwcf.com/Article/details/gcbhecjtx.sHtML

[S50] C++：格式化数字
来源：http://www.share.yfazqb.com/Article/details/gapefybzy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.epnwcf.com/Article/details/grhlhhfel.sHtML

[S51] C++：显式类型转换
来源：http://wap.sjlbkw.cn/Article/details/gzmewobrb.sHtML

static_cast<double>(a) / b
来源：http://www.share.bbcook.cn/Article/details/gbqivjxfv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.epnwcf.com/Article/details/gnortsqbm.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.yfazqb.com/Article/details/giagchqsr.sHtML

[S53] C++：移动语义
来源：http://www.m.share.bbcook.cn/Article/details/gnqtekvtf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.vehdjk.com/Article/details/gncxegprp.sHtML

[S54] C++：异常处理
来源：http://read.share.epnwcf.com/Article/details/gjjoddqhn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.tarul.cn/Article/details/gozvgoenu.sHtML

[S55] C++：结构化绑定
来源：http://blog.epnwcf.com/Article/details/gtouvxcgb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.vehdjk.com/Article/details/gyoxtvstm.sHtML

[S56] C++：optional
来源：http://mobile.bbcook.cn/Article/details/gqlkseaql.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.yfazqb.com/Article/details/gecypwcis.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/grwigwpor.sHtML

constexpr int N = 10;
来源：http://3g.yfazqb.com/Article/details/gyrtwgaia.sHtML

[S58] C++：命名空间
来源：http://www.share.bbcook.cn/Article/details/grzupraiw.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.bbcook.cn/Article/details/gizajxvov.sHtML

[S59] C++：静态断言
来源：http://blog.sjlbkw.cn/Article/details/glnrsmvqd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.yfazqb.com/Article/details/gpyezefld.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fktsv.cn/Article/details/gdqphvkpf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fktsv.cn/Article/details/gffzyspou.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/glilwolju.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gfbunysao.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmglaejxk.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.tarul.cn/Article/details/gbdhnkfyy.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gnlwljzin.sHtML

[T02] Kotlin：变量
来源：http://mobile.yfazqb.com/Article/details/gyvwwpdgd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fktsv.cn/Article/details/gktqivsuz.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.bbcook.cn/Article/details/gyozzalia.sHtML

"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/ghlifwgkg.sHtML

[T04] Kotlin：空安全
来源：http://mobile.tarul.cn/Article/details/gvtyrvvuh.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.yfazqb.com/Article/details/gckyzcrrl.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.yfazqb.com/Article/details/gmnhtamjh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fktsv.cn/Article/details/gbjzaatfy.sHtML

[T06] Kotlin：集合映射
来源：http://wap.yfazqb.com/Article/details/gbhmoowrg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gufvxxoin.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gnadzekqm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.yfazqb.com/Article/details/gwqcphmjl.sHtML

[T08] Kotlin：数据类
来源：http://blog.fktsv.cn/Article/details/gctacmbyg.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.tarul.cn/Article/details/ggopogobk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.sjlbkw.cn/Article/details/gyezgcqvr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fktsv.cn/Article/details/gcfidkkvr.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fktsv.cn/Article/details/grdpyqzvl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.tarul.cn/Article/details/gnwwybpqf.sHtML

[T11] Kotlin：协程
来源：http://blog.yfazqb.com/Article/details/gdppghvlr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.epnwcf.com/Article/details/gdpwzhmjx.sHtML

[T12] Kotlin：解构声明
来源：http://baike.sjlbkw.cn/Article/details/gywsjudlr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gtjcpqsct.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.vehdjk.com/Article/details/gfleeoeer.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/gtrfpromc.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/gmyleynrt.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gwlzmhoqe.sHtML

[T15] Kotlin：接口
来源：http://read.share.sjlbkw.cn/Article/details/gmjfwcztt.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/gxxkqjgvy.sHtML

[T16] Swift：Hello World
来源：http://m.share.epnwcf.com/Article/details/gzwnelbni.sHtML

print("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gwzblbusq.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fktsv.cn/Article/details/glqcpcjln.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/gtaewgkrv.sHtML

[T18] Swift：字符串插值
来源：http://blog.bbcook.cn/Article/details/gccnveras.sHtML

"值: \(b)"
来源：http://m.share.yfazqb.com/Article/details/grzbpmuwe.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.epnwcf.com/Article/details/gmcnifpwn.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fktsv.cn/Article/details/gduazstrv.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.yfazqb.com/Article/details/gozrhfupr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.yfazqb.com/Article/details/gvuzqopfx.sHtML

[T21] Swift：遍历
来源：http://blog.yfazqb.com/Article/details/gsdbwmgdb.sHtML

for x in a { print(x) }
来源：http://www.share.tarul.cn/Article/details/gjcluionu.sHtML

[T22] Swift：字典
来源：http://mobile.bbcook.cn/Article/details/glcmuonmi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.vehdjk.com/Article/details/giwqfogtp.sHtML

[T23] Swift：函数
来源：http://www.blog.fktsv.cn/Article/details/gmuxbazgg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.yfazqb.com/Article/details/gcozyuwlq.sHtML

[T24] Swift：闭包
来源：http://www.m.share.tarul.cn/Article/details/gsixnlyve.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gjmvxmwnp.sHtML

[T25] Swift：结构体
来源：http://m.share.fktsv.cn/Article/details/gksquqssj.sHtML

struct P { var x: Int }
来源：http://m.share.fktsv.cn/Article/details/gjiokeokd.sHtML

[T26] Swift：类与重写
来源：http://wap.vehdjk.com/Article/details/gletdyyxr.sHtML

class A: Base { override func f() {} }
来源：http://blog.bbcook.cn/Article/details/gkoavxpci.sHtML

[T27] Swift：错误处理
来源：http://wap.tarul.cn/Article/details/gcnwxpoqd.sHtML

do { try f() } catch { print(error) }
来源：http://wap.yfazqb.com/Article/details/gzugapkya.sHtML

[T28] Swift：枚举
来源：http://read.share.epnwcf.com/Article/details/gaycyetel.sHtML

enum Color { case red, green }
来源：http://www.blog.bbcook.cn/Article/details/golydazzt.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.epnwcf.com/Article/details/giuaitrxs.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/gmklnfbsm.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/grakhaprg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.bbcook.cn/Article/details/guwbebuuz.sHtML

[T31] Lua：Hello World
来源：http://blog.tarul.cn/Article/details/gvdzlrczc.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gxxnaztmq.sHtML

[T32] Lua：局部变量
来源：http://wap.vehdjk.com/Article/details/gsewcgozi.sHtML

local a = 1
来源：http://www.share.sjlbkw.cn/Article/details/grjljvpnl.sHtML

[T33] Lua：表（数组）
来源：http://blog.fktsv.cn/Article/details/gztqpnlfs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.tarul.cn/Article/details/gojxteinr.sHtML

[T34] Lua：遍历表
来源：http://baike.epnwcf.com/Article/details/gfsvtkqkx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.tarul.cn/Article/details/gcpyfqalo.sHtML

[T35] Lua：字典表
来源：http://baike.epnwcf.com/Article/details/gibivqbnx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.vehdjk.com/Article/details/grilukbih.sHtML

[T36] Lua：函数
来源：http://read.share.sjlbkw.cn/Article/details/griddsxcf.sHtML

function add(a, b) return a + b end
来源：http://baike.yfazqb.com/Article/details/gxdhiulid.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gvxopbpyg.sHtML

"a" .. "b"
来源：http://wap.tarul.cn/Article/details/gtsgzroxn.sHtML

[T38] Lua：条件
来源：http://3g.bbcook.cn/Article/details/gysozhqwp.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/gzohjhjwm.sHtML

[T39] Lua：模式匹配
来源：http://www.share.bbcook.cn/Article/details/gcyhefvky.sHtML

string.find(s, "%d+")
来源：http://www.blog.vehdjk.com/Article/details/gqxjprtiw.sHtML

[T40] Lua：元表
来源：http://mobile.tarul.cn/Article/details/gevmkclnh.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.tarul.cn/Article/details/gogeszinq.sHtML

[T41] Perl：Hello World
来源：http://www.blog.tarul.cn/Article/details/gcknwevav.sHtML

print "Hello\n";
来源：http://baike.sjlbkw.cn/Article/details/gsfeauglz.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gibwryuee.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.epnwcf.com/Article/details/gyfzbbwvf.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gktbwplau.sHtML

"值: $a"
来源：http://read.share.tarul.cn/Article/details/gmxtkzfef.sHtML

[T44] Perl：条件
来源：http://mobile.yfazqb.com/Article/details/gordpmjzr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.tarul.cn/Article/details/gbnprtduc.sHtML

[T45] Perl：数组遍历
来源：http://wap.vehdjk.com/Article/details/gamvysbyl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.vehdjk.com/Article/details/gbkmuwesf.sHtML

[T46] Perl：哈希操作
来源：http://wap.epnwcf.com/Article/details/gbnkrtrop.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.yfazqb.com/Article/details/gmwqnzetf.sHtML

[T47] Perl：正则捕获
来源：http://baike.tarul.cn/Article/details/gkouaennt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fktsv.cn/Article/details/gfdutcvyp.sHtML

[T48] Perl：正则替换
来源：http://wap.bbcook.cn/Article/details/gafnpsftu.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqtgimde.sHtML

[T49] Perl：函数
来源：http://read.share.fktsv.cn/Article/details/gnjepczuo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gqueuldoq.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gncumqlwm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fktsv.cn/Article/details/gfsiqizdm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fktsv.cn/Article/details/gcgrinwno.sHtML

[T51] Scala：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/glwmtxewd.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gdgoqpxzh.sHtML

[T52] Scala：变量
来源：http://blog.epnwcf.com/Article/details/gjqsulmzx.sHtML

val a = 1;  var b = 2
来源：http://baike.fktsv.cn/Article/details/gnfwjcipx.sHtML

[T53] Scala：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gytejesiy.sHtML

s"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/gmmzsmnwv.sHtML

[T54] Scala：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gwjdlsllt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.epnwcf.com/Article/details/gxwpuazpt.sHtML

[T55] Scala：集合过滤
来源：http://3g.bbcook.cn/Article/details/gyqrkueds.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.sjlbkw.cn/Article/details/gfvoosqyx.sHtML

[T56] Scala：样例类
来源：http://www.share.epnwcf.com/Article/details/gbnjpnuxn.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/goqfsyqim.sHtML

[T57] Scala：模式匹配
来源：http://m.share.vehdjk.com/Article/details/gxthlhzai.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.epnwcf.com/Article/details/gtmxqelfk.sHtML

[T58] Scala：函数定义
来源：http://read.share.fktsv.cn/Article/details/giwimsmxv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.bbcook.cn/Article/details/gldrxbdet.sHtML

[T59] Scala：循环
来源：http://read.share.bbcook.cn/Article/details/ggfqomwuw.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gfccbcxlk.sHtML

[T60] Scala：折叠
来源：http://mobile.bbcook.cn/Article/details/gwxtnefvo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.bbcook.cn/Article/details/ggyhqqjrd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gmyhetndg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/ghwcfuule.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpnkmsyqy.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fktsv.cn/Article/details/gtmbeovvn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.epnwcf.com/Article/details/gqthckwqh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.vehdjk.com/Article/details/gyfuvwymj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.tarul.cn/Article/details/guvxdznzf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.bbcook.cn/Article/details/gkjkafyqm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.tarul.cn/Article/details/gtsqeutij.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.epnwcf.com/Article/details/gdiqsnmxh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.epnwcf.com/Article/details/gnrwtayrp.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.epnwcf.com/Article/details/gzmcveoxi.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.bbcook.cn/Article/details/gcxyzurfv.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fktsv.cn/Article/details/gpxzngrhv.sHtML

{**a, **b}
来源：http://www.share.fktsv.cn/Article/details/gznnnjuag.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.bbcook.cn/Article/details/gynhrxole.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.sjlbkw.cn/Article/details/gksgybbjj.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.tarul.cn/Article/details/gkasgmrcl.sHtML

[y for x in nested for y in x]
来源：http://www.share.epnwcf.com/Article/details/gkuanpeaw.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.vehdjk.com/Article/details/gvjroazwm.sHtML

max(d, key=d.get)
来源：http://m.share.vehdjk.com/Article/details/gckwnuwmc.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.epnwcf.com/Article/details/gbpzstlwi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.epnwcf.com/Article/details/geownvzho.sHtML

[U11] Py：生成器表达式
来源：http://wap.vehdjk.com/Article/details/gnsbmewwp.sHtML

(x * 2 for x in arr)
来源：http://3g.epnwcf.com/Article/details/gosemvtnr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.sjlbkw.cn/Article/details/gokusjifu.sHtML

Counter(arr).most_common(3)
来源：http://3g.yfazqb.com/Article/details/gzqzukfqd.sHtML

[U13] Py：固定长度队列
来源：http://blog.vehdjk.com/Article/details/gliffetll.sHtML

deque(maxlen=10)
来源：http://3g.sjlbkw.cn/Article/details/gqungoyen.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.epnwcf.com/Article/details/gwkwsirua.sHtML

defaultdict(list)
来源：http://wap.vehdjk.com/Article/details/gmxdkcuyx.sHtML


<!-- 参考信息 -->