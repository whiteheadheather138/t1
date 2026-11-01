代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.sjlbkw.cn/Article/details/gowekzklq.sHtML

[R72] 等待端口就绪
来源：http://3g.epnwcf.com/Article/details/ggbamufka.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/griycolwj.sHtML

[R73] 分割大日志
来源：http://m.share.fktsv.cn/Article/details/gscallnol.sHtML

split -l 1000 big.log part_
来源：http://blog.vehdjk.com/Article/details/grkfglegf.sHtML

[R74] 批量重命名
来源：http://blog.yfazqb.com/Article/details/gwkethuni.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.epnwcf.com/Article/details/gkdmzyvxr.sHtML

[R75] 导出环境变量
来源：http://3g.yfazqb.com/Article/details/gvqollkps.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.tarul.cn/Article/details/grmedmcwy.sHtML

[R76] 使用临时文件
来源：http://3g.sjlbkw.cn/Article/details/gcrzwsstd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/gaiiprvyk.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmnjabgi.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.yfazqb.com/Article/details/gwrnaljom.sHtML

[R78] 交互式菜单
来源：http://3g.bbcook.cn/Article/details/gehvfyntm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.tarul.cn/Article/details/gpztwljjt.sHtML

[R79] 解析命令行选项
来源：http://www.share.sjlbkw.cn/Article/details/gixsfogpp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.epnwcf.com/Article/details/grxjoopav.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/gzjxlofxj.sHtML

time ./run.sh
来源：http://baike.yfazqb.com/Article/details/grnyeaswd.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/glfbczzft.sHtML

S. C / C++ 专题
来源：http://wap.bbcook.cn/Article/details/grszijitj.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gakwfauhf.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gbjaltkjc.sHtML

#include <stdio.h>
来源：http://www.share.yfazqb.com/Article/details/gpxpksmye.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.yfazqb.com/Article/details/gtxepkxja.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gmkkusrkl.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.bbcook.cn/Article/details/ggpooveya.sHtML

[S03] C：读入整数
来源：http://3g.yfazqb.com/Article/details/gnkblelta.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/gbfoxpxlu.sHtML

[S04] C：字符串复制
来源：http://wap.epnwcf.com/Article/details/glpnkphhk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.vehdjk.com/Article/details/gxnluwgkk.sHtML

[S05] C：字符串长度
来源：http://read.share.tarul.cn/Article/details/gmkvpxzxs.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/giysjkveb.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gwpkluvmi.sHtML

strcmp(a, b) == 0
来源：http://baike.tarul.cn/Article/details/gsoodsgev.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/gbvequhvv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/grktgoimz.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.vehdjk.com/Article/details/gfeikfslr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.sjlbkw.cn/Article/details/grvxhoysn.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.yfazqb.com/Article/details/ghfemvkur.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.bbcook.cn/Article/details/gxxzwztmf.sHtML

[S10] C：指针与解引用
来源：http://blog.epnwcf.com/Article/details/gfxtmiikc.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/gnnsspheu.sHtML

[S11] C：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/giidfatoy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/ggtganrbx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.yfazqb.com/Article/details/guqoxejvm.sHtML

fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gdwpinkmq.sHtML

[S12] C：写文件
来源：http://blog.sjlbkw.cn/Article/details/gsnuvdnbh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.epnwcf.com/Article/details/gkfoykhmo.sHtML

[S13] C：宏定义
来源：http://www.blog.sjlbkw.cn/Article/details/glqibzexk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.tarul.cn/Article/details/gtxzhzelu.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/gztuapwcz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.yfazqb.com/Article/details/gwaclfakn.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/glbwcmatk.sHtML

(double) a / b
来源：http://www.blog.vehdjk.com/Article/details/gjwdrarml.sHtML

[S16] C：位操作置位
来源：http://baike.yfazqb.com/Article/details/gggynbtrv.sHtML

x |= (1 << 3);
来源：http://www.m.share.vehdjk.com/Article/details/gejfyoxnx.sHtML

[S17] C：安全拼接字符串
来源：http://baike.yfazqb.com/Article/details/gryppxele.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.vehdjk.com/Article/details/gnjafkrzt.sHtML

[S18] C：命令行参数
来源：http://mobile.bbcook.cn/Article/details/gmsrtlqqa.sHtML

int main(int argc, char **argv)
来源：http://www.blog.epnwcf.com/Article/details/gkcawbnqn.sHtML

[S19] C：快速排序
来源：http://read.share.epnwcf.com/Article/details/ggdupxlnr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gmwzqqwfs.sHtML

[S20] C：二分查找
来源：http://read.share.fktsv.cn/Article/details/gvvjckdeu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/glkuthimz.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gqgvfgmma.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.epnwcf.com/Article/details/giubfguyk.sHtML

[S22] C：字符串转数字
来源：http://www.share.vehdjk.com/Article/details/gusgentyo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/gzfjudpnf.sHtML

[S23] C：随机数
来源：http://www.m.share.tarul.cn/Article/details/gbjmqwves.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.vehdjk.com/Article/details/glaugmiuz.sHtML

[S24] C：获取本地时间
来源：http://read.share.bbcook.cn/Article/details/ggwvupxwi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/gaexyigor.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/ggiuqssyw.sHtML

memcpy(dst, src, n);
来源：http://blog.epnwcf.com/Article/details/gtlngnrmh.sHtML

[S26] C：内存清零
来源：http://www.m.share.vehdjk.com/Article/details/gyzwwpyqi.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/ggscwppta.sHtML

[S27] C：定义常量
来源：http://blog.yfazqb.com/Article/details/gyzvizdky.sHtML

const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gdzhbbygq.sHtML

[S28] C：静态变量
来源：http://m.share.fktsv.cn/Article/details/gmbcidhdq.sHtML

static int counter = 0;
来源：http://wap.epnwcf.com/Article/details/ggjhyffnw.sHtML

[S29] C：变参函数
来源：http://baike.tarul.cn/Article/details/gacoafcnp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/ghzgkbtfq.sHtML

[S30] C：头文件保护
来源：http://mobile.sjlbkw.cn/Article/details/gmjyjdmyo.sHtML

#ifndef X_H
来源：http://mobile.vehdjk.com/Article/details/ggawvdrnh.sHtML

#define X_H
来源：http://3g.vehdjk.com/Article/details/ggwwtqdod.sHtML

#endif
来源：http://baike.epnwcf.com/Article/details/gehwufpco.sHtML

[S31] C++：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gkvphizwh.sHtML

#include <iostream>
来源：http://wap.epnwcf.com/Article/details/gtvatcnhu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fktsv.cn/Article/details/gkfxnfjpk.sHtML

[S32] C++：字符串
来源：http://www.share.bbcook.cn/Article/details/gehqgmvml.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.sjlbkw.cn/Article/details/gcbkzeznc.sHtML

[S33] C++：vector 增删
来源：http://m.share.bbcook.cn/Article/details/gudvdmwkx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.sjlbkw.cn/Article/details/gxpgismsw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fktsv.cn/Article/details/gspzynlxe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fktsv.cn/Article/details/gmpdvrlio.sHtML

[S35] C++：map
来源：http://www.share.yfazqb.com/Article/details/giwexxmqp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gncqsfzoq.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gzdmaptyh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/grjantvci.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/gnetllbin.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.vehdjk.com/Article/details/glarupdzm.sHtML

[S38] C++：排序
来源：http://baike.bbcook.cn/Article/details/gaknafzpz.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fktsv.cn/Article/details/gpmybpajx.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/gffxqdsau.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/gnymlwnxq.sHtML

[S40] C++：查找元素
来源：http://www.m.share.epnwcf.com/Article/details/giotjpgoh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.vehdjk.com/Article/details/gjrcdwlyd.sHtML

[S41] C++：类与构造函数
来源：http://m.share.tarul.cn/Article/details/goqgltavj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.sjlbkw.cn/Article/details/gducwdcjg.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.epnwcf.com/Article/details/ghzlkyehp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gbabnpyvx.sHtML

[S43] C++：智能指针
来源：http://blog.epnwcf.com/Article/details/gqfhqzmub.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.sjlbkw.cn/Article/details/gtwvkfdot.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gzurilxwc.sHtML

void inc(int &x) { ++x; }
来源：http://wap.epnwcf.com/Article/details/gvkqrmens.sHtML

[S45] C++：lambda
来源：http://www.blog.sjlbkw.cn/Article/details/gxbyswpec.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.epnwcf.com/Article/details/guhqcaaqh.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/gfvpwirtt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.bbcook.cn/Article/details/gutisvhyl.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/gcfhmdtfe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.tarul.cn/Article/details/gjkyhwnlh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/govfbzxtx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gnokjmsip.sHtML

while (std::getline(in, line)) { }
来源：http://baike.sjlbkw.cn/Article/details/gfrwwzomw.sHtML

[S49] C++：写文件
来源：http://wap.vehdjk.com/Article/details/gtcvmkowj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.bbcook.cn/Article/details/gmspontmb.sHtML

[S50] C++：格式化数字
来源：http://m.share.fktsv.cn/Article/details/guawjijig.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gltyyqewm.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fktsv.cn/Article/details/gixvtrscs.sHtML

static_cast<double>(a) / b
来源：http://blog.tarul.cn/Article/details/grkabcuve.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/graupjaub.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtcgvche.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/ginzltgya.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.bbcook.cn/Article/details/gdmgiuiwy.sHtML

[S54] C++：异常处理
来源：http://www.share.fktsv.cn/Article/details/ggxrcvpqz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.vehdjk.com/Article/details/gyjrgjafq.sHtML

[S55] C++：结构化绑定
来源：http://m.share.epnwcf.com/Article/details/gvtoyohjp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gxarfhoca.sHtML

[S56] C++：optional
来源：http://blog.tarul.cn/Article/details/goljrnuik.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.epnwcf.com/Article/details/gakyjssfx.sHtML

[S57] C++：编译期常量
来源：http://m.share.sjlbkw.cn/Article/details/gdsamrynf.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/gtrhvkjvz.sHtML

[S58] C++：命名空间
来源：http://www.m.share.bbcook.cn/Article/details/goztjerts.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.epnwcf.com/Article/details/gcfofapon.sHtML

[S59] C++：静态断言
来源：http://3g.yfazqb.com/Article/details/grqgaosgi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fktsv.cn/Article/details/goeiedysp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gqrtrhfzq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fktsv.cn/Article/details/glxlnhcyv.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdnuevxfc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gmvehplap.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqalseoih.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gcszzhbdi.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gcfierrsp.sHtML

[T02] Kotlin：变量
来源：http://wap.tarul.cn/Article/details/gdpxzlahn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.yfazqb.com/Article/details/grwhbvtfv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.sjlbkw.cn/Article/details/gedpfkjmu.sHtML

"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gwzyxdlym.sHtML

[T04] Kotlin：空安全
来源：http://read.share.bbcook.cn/Article/details/glvcyrfar.sHtML

val n: String? = null;  n?.length
来源：http://read.share.epnwcf.com/Article/details/gnbwfqpag.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.bbcook.cn/Article/details/gawkfbhhs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.sjlbkw.cn/Article/details/ghggaanhl.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gekjxtbpg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/gqnsyqlro.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gbyoippjt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.vehdjk.com/Article/details/ghdpnuczk.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.epnwcf.com/Article/details/gsydekref.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/gcxzyvzei.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/ggylxhovt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.sjlbkw.cn/Article/details/gefpumovj.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.tarul.cn/Article/details/ggixcrpkz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.epnwcf.com/Article/details/gbszzfvll.sHtML

[T11] Kotlin：协程
来源：http://mobile.vehdjk.com/Article/details/gyehqkybp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.vehdjk.com/Article/details/grrdajhff.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.tarul.cn/Article/details/gbiqnyafz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/gbgzspmoq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fktsv.cn/Article/details/ghrzrumoo.sHtML

val m = mapOf("a" to 1)
来源：http://wap.sjlbkw.cn/Article/details/gegknywds.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.yfazqb.com/Article/details/gsyovafry.sHtML

for (i in 1..10) println(i)
来源：http://baike.tarul.cn/Article/details/gwoymogfn.sHtML

[T15] Kotlin：接口
来源：http://mobile.epnwcf.com/Article/details/gmcprwvpx.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fktsv.cn/Article/details/godzqlfvu.sHtML

[T16] Swift：Hello World
来源：http://blog.fktsv.cn/Article/details/gzfgjjdzw.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gapsahfay.sHtML

[T17] Swift：变量与常量
来源：http://baike.tarul.cn/Article/details/gpdmokxos.sHtML

var a = 1;  let b = 2
来源：http://mobile.yfazqb.com/Article/details/gepytugck.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gizgidqux.sHtML

"值: \(b)"
来源：http://m.share.sjlbkw.cn/Article/details/gnebmqwmj.sHtML

[T19] Swift：可选绑定
来源：http://m.share.epnwcf.com/Article/details/gidswrjgq.sHtML

if let n = opt { print(n) }
来源：http://wap.epnwcf.com/Article/details/gkokbtvzc.sHtML

[T20] Swift：数组操作
来源：http://3g.fktsv.cn/Article/details/guozgzqdc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fktsv.cn/Article/details/gqnhudnxz.sHtML

[T21] Swift：遍历
来源：http://read.share.bbcook.cn/Article/details/geyxhyemd.sHtML

for x in a { print(x) }
来源：http://m.share.epnwcf.com/Article/details/ggnninkvr.sHtML

[T22] Swift：字典
来源：http://www.blog.fktsv.cn/Article/details/gbchapknx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.epnwcf.com/Article/details/gkxswtyjh.sHtML

[T23] Swift：函数
来源：http://blog.vehdjk.com/Article/details/ghsgmcstu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fktsv.cn/Article/details/gulhfzsnb.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fktsv.cn/Article/details/gavvuulqe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.yfazqb.com/Article/details/ggxwekljp.sHtML

[T25] Swift：结构体
来源：http://m.share.fktsv.cn/Article/details/gzdegsmon.sHtML

struct P { var x: Int }
来源：http://read.share.yfazqb.com/Article/details/gujzmnpjc.sHtML

[T26] Swift：类与重写
来源：http://mobile.sjlbkw.cn/Article/details/gpaesljhz.sHtML

class A: Base { override func f() {} }
来源：http://mobile.epnwcf.com/Article/details/gefiakuzw.sHtML

[T27] Swift：错误处理
来源：http://blog.tarul.cn/Article/details/gnmmouwnm.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.bbcook.cn/Article/details/gxjpooeih.sHtML

[T28] Swift：枚举
来源：http://blog.fktsv.cn/Article/details/goyzaadcy.sHtML

enum Color { case red, green }
来源：http://www.blog.epnwcf.com/Article/details/gcpgutexp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.bbcook.cn/Article/details/gknqhqtii.sHtML

guard let x = opt else { return }
来源：http://3g.tarul.cn/Article/details/gvtaepzal.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/gysedbbag.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.tarul.cn/Article/details/gkeferojk.sHtML

[T31] Lua：Hello World
来源：http://wap.vehdjk.com/Article/details/gwbawxzsi.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gitibxfbq.sHtML

[T32] Lua：局部变量
来源：http://baike.tarul.cn/Article/details/ghjdbmdsf.sHtML

local a = 1
来源：http://blog.tarul.cn/Article/details/gjmmxdznd.sHtML

[T33] Lua：表（数组）
来源：http://wap.yfazqb.com/Article/details/gqrhhiiov.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.sjlbkw.cn/Article/details/gwbafdlkp.sHtML

[T34] Lua：遍历表
来源：http://m.share.yfazqb.com/Article/details/gtnpompmm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fktsv.cn/Article/details/ghxwkezvc.sHtML

[T35] Lua：字典表
来源：http://read.share.tarul.cn/Article/details/gumdvenfg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.bbcook.cn/Article/details/gbuxwtvrb.sHtML

[T36] Lua：函数
来源：http://www.blog.bbcook.cn/Article/details/gmotroppo.sHtML

function add(a, b) return a + b end
来源：http://wap.vehdjk.com/Article/details/grgebyxll.sHtML

[T37] Lua：字符串拼接
来源：http://baike.tarul.cn/Article/details/gxzhfwmfh.sHtML

"a" .. "b"
来源：http://3g.tarul.cn/Article/details/geyofxvmh.sHtML

[T38] Lua：条件
来源：http://m.share.sjlbkw.cn/Article/details/gnrjfdmfx.sHtML

if x > 0 then print("正") end
来源：http://wap.epnwcf.com/Article/details/gfnahgfrv.sHtML

[T39] Lua：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gkazlmoki.sHtML

string.find(s, "%d+")
来源：http://www.share.sjlbkw.cn/Article/details/ggvefivqg.sHtML

[T40] Lua：元表
来源：http://blog.vehdjk.com/Article/details/gglppyjsz.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fktsv.cn/Article/details/gawfntdxc.sHtML

[T41] Perl：Hello World
来源：http://www.blog.tarul.cn/Article/details/garqfvchf.sHtML

print "Hello\n";
来源：http://www.share.epnwcf.com/Article/details/gocgblmns.sHtML

[T42] Perl：变量类型
来源：http://blog.yfazqb.com/Article/details/gfrybxhqw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.bbcook.cn/Article/details/gjdpmznpg.sHtML

[T43] Perl：字符串插值
来源：http://3g.bbcook.cn/Article/details/gpzewlggv.sHtML

"值: $a"
来源：http://mobile.bbcook.cn/Article/details/gbydxtobf.sHtML

[T44] Perl：条件
来源：http://3g.vehdjk.com/Article/details/gkthhxjal.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.bbcook.cn/Article/details/gefkvmvix.sHtML

[T45] Perl：数组遍历
来源：http://blog.fktsv.cn/Article/details/gyenzooet.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.bbcook.cn/Article/details/gjvwejurc.sHtML

[T46] Perl：哈希操作
来源：http://baike.fktsv.cn/Article/details/gxgzowmto.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.sjlbkw.cn/Article/details/gsysxuibe.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.tarul.cn/Article/details/ggsteqbak.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fktsv.cn/Article/details/glwbxgsvv.sHtML

[T48] Perl：正则替换
来源：http://www.share.bbcook.cn/Article/details/gstojkcij.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/gpcsbyoot.sHtML

[T49] Perl：函数
来源：http://m.share.fktsv.cn/Article/details/gndyarhec.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gwlnuixul.sHtML

[T50] Perl：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gphlretex.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fktsv.cn/Article/details/gyyooylof.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fktsv.cn/Article/details/gldiywwlu.sHtML

[T51] Scala：Hello World
来源：http://3g.tarul.cn/Article/details/gbjezkujs.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gvtplosjv.sHtML

[T52] Scala：变量
来源：http://m.share.fktsv.cn/Article/details/gqlnhcpug.sHtML

val a = 1;  var b = 2
来源：http://blog.yfazqb.com/Article/details/gwnwkuvqj.sHtML

[T53] Scala：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gxhfpiwrs.sHtML

s"值: $b"
来源：http://baike.bbcook.cn/Article/details/gwqoxcwqs.sHtML

[T54] Scala：集合映射
来源：http://mobile.tarul.cn/Article/details/gnqqxqcfb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.sjlbkw.cn/Article/details/gjvnlqyan.sHtML

[T55] Scala：集合过滤
来源：http://mobile.tarul.cn/Article/details/gzbvjhndr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.bbcook.cn/Article/details/glorzezjd.sHtML

[T56] Scala：样例类
来源：http://www.share.yfazqb.com/Article/details/gwkcqzlir.sHtML

case class User(name: String, age: Int)
来源：http://baike.bbcook.cn/Article/details/gwwcpycru.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gxdljtkev.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gkjkvqkcj.sHtML

[T58] Scala：函数定义
来源：http://3g.yfazqb.com/Article/details/guwejunvr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/gwykgtykx.sHtML

[T59] Scala：循环
来源：http://www.m.share.yfazqb.com/Article/details/gxpmamkgw.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.vehdjk.com/Article/details/geuyqjabs.sHtML

[T60] Scala：折叠
来源：http://read.share.tarul.cn/Article/details/gzkqdfdck.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.yfazqb.com/Article/details/gsckheact.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/geemvfqvp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.epnwcf.com/Article/details/gzzvhjujg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/geezcncrt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.vehdjk.com/Article/details/gnhntxerl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.sjlbkw.cn/Article/details/gluworyfd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.tarul.cn/Article/details/ggnlwnbmr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.tarul.cn/Article/details/gosihncpq.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.epnwcf.com/Article/details/ggfbyihax.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.epnwcf.com/Article/details/gbzlwfovv.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.bbcook.cn/Article/details/gsgffimsw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.tarul.cn/Article/details/gygtwjcxs.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.tarul.cn/Article/details/gxiriotee.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gnoodspor.sHtML

[U06] Py：合并两个字典
来源：http://m.share.bbcook.cn/Article/details/grlsuecjj.sHtML

{**a, **b}
来源：http://3g.fktsv.cn/Article/details/gslyywiiu.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gdbrtkvfw.sHtML

{v: k for k, v in d.items()}
来源：http://3g.epnwcf.com/Article/details/gadyyyhgk.sHtML

[U08] Py：展平二维列表
来源：http://3g.epnwcf.com/Article/details/gxbnktrkw.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.vehdjk.com/Article/details/grbxflhgc.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.bbcook.cn/Article/details/ganyumtnt.sHtML

max(d, key=d.get)
来源：http://blog.tarul.cn/Article/details/gubzkzpsp.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.epnwcf.com/Article/details/gskkmyzyg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.bbcook.cn/Article/details/gxkbvozdj.sHtML

[U11] Py：生成器表达式
来源：http://blog.vehdjk.com/Article/details/gtybcamyv.sHtML

(x * 2 for x in arr)
来源：http://mobile.sjlbkw.cn/Article/details/grefgnlcf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.vehdjk.com/Article/details/ghtmspxvl.sHtML

Counter(arr).most_common(3)
来源：http://www.share.yfazqb.com/Article/details/gmymobzfj.sHtML


<!-- 参考信息 -->