代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fktsv.cn/Article/details/gikxyanli.sHtML

[R70] 时间戳与互转
来源：http://read.share.sjlbkw.cn/Article/details/gcpkrhtxf.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/glxiwumnx.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gnnshzxdt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.bbcook.cn/Article/details/gfkcjqycb.sHtML

[R72] 等待端口就绪
来源：http://read.share.fktsv.cn/Article/details/gqwlyudfz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/gpilwncmz.sHtML

[R73] 分割大日志
来源：http://www.m.share.vehdjk.com/Article/details/gsgowwrnp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.vehdjk.com/Article/details/gfoxhlict.sHtML

[R74] 批量重命名
来源：http://blog.vehdjk.com/Article/details/gjawwmfym.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/grfkxhacd.sHtML

[R75] 导出环境变量
来源：http://blog.sjlbkw.cn/Article/details/gypyvaijm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.vehdjk.com/Article/details/gxbamnlma.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gfxiutxsa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gvudsdztx.sHtML

[R77] 读取用户输入
来源：http://3g.fktsv.cn/Article/details/gcznsbakt.sHtML

read -rp "请输入: " ans
来源：http://blog.fktsv.cn/Article/details/gjtztdukx.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/gdnlittik.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.vehdjk.com/Article/details/geidlbddm.sHtML

[R79] 解析命令行选项
来源：http://m.share.yfazqb.com/Article/details/gqbivlxsl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.sjlbkw.cn/Article/details/ggtamskeh.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.bbcook.cn/Article/details/graffswil.sHtML

time ./run.sh
来源：http://baike.epnwcf.com/Article/details/gqnyfvted.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpltsqhzl.sHtML

S. C / C++ 专题
来源：http://www.blog.tarul.cn/Article/details/gbdyvspzr.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gcilcdkst.sHtML

[S01] C：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gxqibzjbs.sHtML

#include <stdio.h>
来源：http://www.m.share.vehdjk.com/Article/details/gpwhryzub.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/gbkzmwwkm.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/gnzqeikmz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.epnwcf.com/Article/details/genfxxoyi.sHtML

[S03] C：读入整数
来源：http://3g.tarul.cn/Article/details/gwmxjjusf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.vehdjk.com/Article/details/gjvnocefx.sHtML

[S04] C：字符串复制
来源：http://3g.yfazqb.com/Article/details/gudrvnlbn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.bbcook.cn/Article/details/gsnahadmt.sHtML

[S05] C：字符串长度
来源：http://wap.tarul.cn/Article/details/grbzarqua.sHtML

strlen(s)
来源：http://wap.sjlbkw.cn/Article/details/gfxweoyec.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/geevzsxuw.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/gwzoxhnzn.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/grekoryih.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.tarul.cn/Article/details/gbkpfvoaa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.tarul.cn/Article/details/gjihmctpj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.vehdjk.com/Article/details/gkvzkclzj.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.sjlbkw.cn/Article/details/giywbpiqe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.vehdjk.com/Article/details/geuebmqbe.sHtML

[S10] C：指针与解引用
来源：http://m.share.yfazqb.com/Article/details/giztzhecn.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.yfazqb.com/Article/details/gxrdsjroh.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gjberzfdl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.epnwcf.com/Article/details/goqmeyljj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/gmycuvwuu.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/gqgciadxl.sHtML

[S12] C：写文件
来源：http://www.m.share.bbcook.cn/Article/details/glzsfpity.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.vehdjk.com/Article/details/gibcznleo.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/gcqhcnegm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/ggvumzotk.sHtML

[S14] C：枚举
来源：http://3g.fktsv.cn/Article/details/gvhamqamx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.sjlbkw.cn/Article/details/gkfdylkat.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/ggcqwaxqy.sHtML

(double) a / b
来源：http://m.share.vehdjk.com/Article/details/gyqmhsmnu.sHtML

[S16] C：位操作置位
来源：http://www.m.share.vehdjk.com/Article/details/gfnbrdpfi.sHtML

x |= (1 << 3);
来源：http://m.share.sjlbkw.cn/Article/details/gtqgnlnup.sHtML

[S17] C：安全拼接字符串
来源：http://wap.tarul.cn/Article/details/gifripcvz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.sjlbkw.cn/Article/details/givaerhgn.sHtML

[S18] C：命令行参数
来源：http://www.share.yfazqb.com/Article/details/gicilimts.sHtML

int main(int argc, char **argv)
来源：http://www.share.epnwcf.com/Article/details/gsixzqeyr.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/gzasmxajx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gtiixdrgl.sHtML

[S20] C：二分查找
来源：http://m.share.sjlbkw.cn/Article/details/gsxtwgqxw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/grftcbvzr.sHtML

[S21] C：字符类别判断
来源：http://www.blog.bbcook.cn/Article/details/gepeuuxpe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.tarul.cn/Article/details/gzydgxjdg.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/grijwnhbr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/gnycbbevp.sHtML

[S23] C：随机数
来源：http://www.m.share.fktsv.cn/Article/details/gdqttkjnk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.sjlbkw.cn/Article/details/gmekbpljk.sHtML

[S24] C：获取本地时间
来源：http://wap.tarul.cn/Article/details/grrswisui.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.bbcook.cn/Article/details/gmyzexirk.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/gdlrhejna.sHtML

memcpy(dst, src, n);
来源：http://wap.vehdjk.com/Article/details/gihzaxvzb.sHtML

[S26] C：内存清零
来源：http://wap.fktsv.cn/Article/details/gqdmttyqc.sHtML

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/gfxaalacy.sHtML

[S27] C：定义常量
来源：http://wap.yfazqb.com/Article/details/gauhbfowl.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/guohqyltt.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gqxukzsly.sHtML

static int counter = 0;
来源：http://www.share.vehdjk.com/Article/details/gocafpoki.sHtML

[S29] C：变参函数
来源：http://baike.tarul.cn/Article/details/gwxjmghmi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.epnwcf.com/Article/details/gkzgabunm.sHtML

[S30] C：头文件保护
来源：http://blog.epnwcf.com/Article/details/gphsclifw.sHtML

#ifndef X_H
来源：http://wap.sjlbkw.cn/Article/details/gvanjpiju.sHtML

#define X_H
来源：http://mobile.bbcook.cn/Article/details/gcapgksvf.sHtML

#endif
来源：http://wap.vehdjk.com/Article/details/gccrmvefk.sHtML

[S31] C++：Hello World
来源：http://mobile.tarul.cn/Article/details/gkmtsngrv.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/grejtiwzj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.yfazqb.com/Article/details/gzhfpuryv.sHtML

[S32] C++：字符串
来源：http://www.share.vehdjk.com/Article/details/gitlwagtm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fktsv.cn/Article/details/gffuplgjt.sHtML

[S33] C++：vector 增删
来源：http://wap.tarul.cn/Article/details/gzqiapmqc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/gyzhshzgh.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.bbcook.cn/Article/details/gdnjuzirn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.vehdjk.com/Article/details/gixzbmmiv.sHtML

[S35] C++：map
来源：http://baike.yfazqb.com/Article/details/gvkoxwmdi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gxadevsix.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.bbcook.cn/Article/details/gzxaorqhc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gkuetxgbw.sHtML

[S37] C++：set
来源：http://www.m.share.epnwcf.com/Article/details/gdinequsm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.vehdjk.com/Article/details/gvsnuched.sHtML

[S38] C++：排序
来源：http://read.share.vehdjk.com/Article/details/gpjvkoygn.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.tarul.cn/Article/details/gesdeokhh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.bbcook.cn/Article/details/genzykxyd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/grtgtnpbl.sHtML

[S40] C++：查找元素
来源：http://read.share.sjlbkw.cn/Article/details/grzscdfhi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.sjlbkw.cn/Article/details/gbivcmjsa.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/gnuobojoe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.vehdjk.com/Article/details/goxbrihtz.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gloyuoppv.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fktsv.cn/Article/details/gifjvdwfi.sHtML

[S43] C++：智能指针
来源：http://baike.fktsv.cn/Article/details/gdvvxayyn.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/gyrpwmqab.sHtML

[S44] C++：引用传参
来源：http://3g.sjlbkw.cn/Article/details/gvyoxqiqx.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fktsv.cn/Article/details/ghebwgkmu.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/gxphplkoz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.bbcook.cn/Article/details/gyvunmlfb.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/gnalahskd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.vehdjk.com/Article/details/gtiszyntg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.epnwcf.com/Article/details/gtsxjiucq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fktsv.cn/Article/details/gtjpekcec.sHtML

[S48] C++：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gsskyohpf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.bbcook.cn/Article/details/ggvncndtz.sHtML

while (std::getline(in, line)) { }
来源：http://3g.vehdjk.com/Article/details/gudqjcxgk.sHtML

[S49] C++：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gwdhmngvc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.tarul.cn/Article/details/grqktxvtb.sHtML

[S50] C++：格式化数字
来源：http://mobile.sjlbkw.cn/Article/details/gmbkptxxv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gseebpvej.sHtML

[S51] C++：显式类型转换
来源：http://wap.bbcook.cn/Article/details/gmesgmbvb.sHtML

static_cast<double>(a) / b
来源：http://wap.yfazqb.com/Article/details/gvnolzujq.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.yfazqb.com/Article/details/gliwjhehi.sHtML

int size() const noexcept { return n_; }
来源：http://wap.sjlbkw.cn/Article/details/gsbsremez.sHtML

[S53] C++：移动语义
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdlrbeqe.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.sjlbkw.cn/Article/details/gunuttpcj.sHtML

[S54] C++：异常处理
来源：http://www.share.yfazqb.com/Article/details/gwpgdginh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.yfazqb.com/Article/details/gwpldetqm.sHtML

[S55] C++：结构化绑定
来源：http://m.share.sjlbkw.cn/Article/details/gzufiyubo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.vehdjk.com/Article/details/grahqsmen.sHtML

[S56] C++：optional
来源：http://mobile.vehdjk.com/Article/details/gpmvarqlm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.bbcook.cn/Article/details/geujtdhrv.sHtML

[S57] C++：编译期常量
来源：http://blog.epnwcf.com/Article/details/gmrohsapl.sHtML

constexpr int N = 10;
来源：http://read.share.tarul.cn/Article/details/gjmuacnhw.sHtML

[S58] C++：命名空间
来源：http://read.share.bbcook.cn/Article/details/gbydypjfy.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.yfazqb.com/Article/details/gmtekekqp.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/gkzjminue.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/gkhuthliq.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.bbcook.cn/Article/details/gtijyxdjj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.yfazqb.com/Article/details/ggpmylczr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gslzmjuak.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gaahdpujh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gcuijmdvf.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/gjvktoexn.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gtorenhpu.sHtML

[T02] Kotlin：变量
来源：http://blog.fktsv.cn/Article/details/ggaehmozp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/gqippobbg.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.epnwcf.com/Article/details/gswwthvrj.sHtML

"值: $b"
来源：http://m.share.tarul.cn/Article/details/gdbjpdysz.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.epnwcf.com/Article/details/gdmyctfsx.sHtML

val n: String? = null;  n?.length
来源：http://blog.yfazqb.com/Article/details/gbpieosgd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.sjlbkw.cn/Article/details/girdidsgb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.tarul.cn/Article/details/gcomuonos.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fktsv.cn/Article/details/gwctblxek.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gcxewzbag.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.epnwcf.com/Article/details/gakdakepg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.sjlbkw.cn/Article/details/gfuggnjgb.sHtML

[T08] Kotlin：数据类
来源：http://blog.fktsv.cn/Article/details/garliajgd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/gajuyagmx.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.yfazqb.com/Article/details/glriureov.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.yfazqb.com/Article/details/gqigwtphh.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/ggyqgprbc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.sjlbkw.cn/Article/details/gchjfcqwf.sHtML

[T11] Kotlin：协程
来源：http://www.share.tarul.cn/Article/details/geohcynij.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/geqafvwiy.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.tarul.cn/Article/details/ghwwjxyzw.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gribzdykl.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/gmkbcvkrx.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.vehdjk.com/Article/details/gleswgatl.sHtML

[T14] Kotlin：循环
来源：http://baike.fktsv.cn/Article/details/gevbbjkok.sHtML

for (i in 1..10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gxxuqsdfu.sHtML

[T15] Kotlin：接口
来源：http://www.share.fktsv.cn/Article/details/gemlffmcf.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkldvwnti.sHtML

[T16] Swift：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gplfrmmke.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsurrkqtn.sHtML

[T17] Swift：变量与常量
来源：http://mobile.sjlbkw.cn/Article/details/gtfcstswr.sHtML

var a = 1;  let b = 2
来源：http://baike.epnwcf.com/Article/details/gdibjrfcy.sHtML

[T18] Swift：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gqxouykvt.sHtML

"值: \(b)"
来源：http://read.share.tarul.cn/Article/details/gqljopqyh.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/giewisnzg.sHtML

if let n = opt { print(n) }
来源：http://blog.vehdjk.com/Article/details/ggciwfgmz.sHtML

[T20] Swift：数组操作
来源：http://read.share.vehdjk.com/Article/details/gcnmcmqev.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.vehdjk.com/Article/details/gatzeosep.sHtML

[T21] Swift：遍历
来源：http://read.share.vehdjk.com/Article/details/ggbabluhh.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/gdsbtvcrq.sHtML

[T22] Swift：字典
来源：http://3g.bbcook.cn/Article/details/goabxkjzr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fktsv.cn/Article/details/gpkypsabv.sHtML

[T23] Swift：函数
来源：http://m.share.vehdjk.com/Article/details/giwtjrnwf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.epnwcf.com/Article/details/gyqvsoiof.sHtML

[T24] Swift：闭包
来源：http://mobile.sjlbkw.cn/Article/details/gepsikkhp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.yfazqb.com/Article/details/gawkurvvx.sHtML

[T25] Swift：结构体
来源：http://3g.tarul.cn/Article/details/gqkyylgvj.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/gvntqupby.sHtML

[T26] Swift：类与重写
来源：http://read.share.vehdjk.com/Article/details/gcvyfpkxm.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.yfazqb.com/Article/details/gzhgvrsyk.sHtML

[T27] Swift：错误处理
来源：http://blog.bbcook.cn/Article/details/gjhvyksuc.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.epnwcf.com/Article/details/gckivqhkl.sHtML

[T28] Swift：枚举
来源：http://3g.bbcook.cn/Article/details/gqabiobya.sHtML

enum Color { case red, green }
来源：http://blog.epnwcf.com/Article/details/gegvylpvy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.tarul.cn/Article/details/gxjcvfhcr.sHtML

guard let x = opt else { return }
来源：http://wap.sjlbkw.cn/Article/details/gkbisryhi.sHtML

[T30] Swift：协议
来源：http://3g.fktsv.cn/Article/details/givmvctim.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.yfazqb.com/Article/details/gfhddeqxo.sHtML

[T31] Lua：Hello World
来源：http://blog.epnwcf.com/Article/details/gcbczigtt.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gtjdlcwef.sHtML

[T32] Lua：局部变量
来源：http://blog.sjlbkw.cn/Article/details/gaztthuem.sHtML

local a = 1
来源：http://3g.epnwcf.com/Article/details/gyrfwnumo.sHtML

[T33] Lua：表（数组）
来源：http://mobile.epnwcf.com/Article/details/gqdcvzjmu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.yfazqb.com/Article/details/grkfayddt.sHtML

[T34] Lua：遍历表
来源：http://www.blog.tarul.cn/Article/details/gflkroqdj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.bbcook.cn/Article/details/gojtzygqm.sHtML

[T35] Lua：字典表
来源：http://www.blog.tarul.cn/Article/details/gqfnefqib.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.vehdjk.com/Article/details/gsiqzgmbe.sHtML

[T36] Lua：函数
来源：http://baike.sjlbkw.cn/Article/details/gvfhpfpar.sHtML

function add(a, b) return a + b end
来源：http://wap.tarul.cn/Article/details/gwnqiwkxp.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fktsv.cn/Article/details/gdvamcbku.sHtML

"a" .. "b"
来源：http://baike.fktsv.cn/Article/details/giwjmzeuk.sHtML

[T38] Lua：条件
来源：http://mobile.tarul.cn/Article/details/gjbdapvas.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/gexicnwgh.sHtML

[T39] Lua：模式匹配
来源：http://m.share.vehdjk.com/Article/details/grpaptjfu.sHtML

string.find(s, "%d+")
来源：http://www.m.share.vehdjk.com/Article/details/gphpyizvv.sHtML

[T40] Lua：元表
来源：http://blog.tarul.cn/Article/details/gidmkhohm.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.bbcook.cn/Article/details/gwgyaxfow.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gmemoblgd.sHtML

print "Hello\n";
来源：http://read.share.epnwcf.com/Article/details/gtcyhwnth.sHtML

[T42] Perl：变量类型
来源：http://m.share.fktsv.cn/Article/details/gywhoysmi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.yfazqb.com/Article/details/gxkuchzzv.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gsnjpvbku.sHtML

"值: $a"
来源：http://www.blog.tarul.cn/Article/details/giuznyeuz.sHtML

[T44] Perl：条件
来源：http://www.blog.sjlbkw.cn/Article/details/ggwuyfayg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.yfazqb.com/Article/details/gmenzofiq.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.yfazqb.com/Article/details/glsorgxlx.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.epnwcf.com/Article/details/gdggfuwlv.sHtML

[T46] Perl：哈希操作
来源：http://baike.sjlbkw.cn/Article/details/geyxhtywq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/gydlunkdm.sHtML

[T47] Perl：正则捕获
来源：http://wap.fktsv.cn/Article/details/gompbhkoe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.tarul.cn/Article/details/gcpeqywyc.sHtML

[T48] Perl：正则替换
来源：http://wap.bbcook.cn/Article/details/gsrngtonw.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.tarul.cn/Article/details/grhqelcps.sHtML

[T49] Perl：函数
来源：http://baike.yfazqb.com/Article/details/gvxhvagxk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gbrxrjzgt.sHtML

[T50] Perl：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gqqkacqkf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.epnwcf.com/Article/details/gdltbydil.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.tarul.cn/Article/details/gwewrtoga.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gljvetyqn.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/ggiwpxhdj.sHtML

[T52] Scala：变量
来源：http://www.share.vehdjk.com/Article/details/gpgspehgm.sHtML

val a = 1;  var b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gxllmziac.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gghkkttol.sHtML

s"值: $b"
来源：http://baike.epnwcf.com/Article/details/ggszrcfcw.sHtML

[T54] Scala：集合映射
来源：http://mobile.yfazqb.com/Article/details/gwgzbnsws.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fktsv.cn/Article/details/gbrjimbol.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gwnlyznzz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.sjlbkw.cn/Article/details/gdxcjuazn.sHtML

[T56] Scala：样例类
来源：http://baike.epnwcf.com/Article/details/gmfodnwtw.sHtML

case class User(name: String, age: Int)
来源：http://wap.fktsv.cn/Article/details/gawnbssfy.sHtML

[T57] Scala：模式匹配
来源：http://read.share.yfazqb.com/Article/details/goixmierm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.vehdjk.com/Article/details/gsozquuiz.sHtML

[T58] Scala：函数定义
来源：http://read.share.vehdjk.com/Article/details/glmzasity.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.bbcook.cn/Article/details/gfwpslrhj.sHtML

[T59] Scala：循环
来源：http://www.m.share.tarul.cn/Article/details/gouxzqxhf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/glxebgdbv.sHtML

[T60] Scala：折叠
来源：http://m.share.bbcook.cn/Article/details/gnkoqvizo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.sjlbkw.cn/Article/details/gthlkoffn.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpfzqzvji.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.sjlbkw.cn/Article/details/gsnibcidq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghnocplbe.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.bbcook.cn/Article/details/gerveozox.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gedbkphbk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.tarul.cn/Article/details/ghwocuioi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.sjlbkw.cn/Article/details/gjduqnerp.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.sjlbkw.cn/Article/details/gemaqiqca.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.yfazqb.com/Article/details/gxktsayke.sHtML

[U04] Py：变量调试打印
来源：http://m.share.epnwcf.com/Article/details/gjfpuodfj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.bbcook.cn/Article/details/gyckuqhqy.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.vehdjk.com/Article/details/gzlikveje.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/gptvrbwzk.sHtML

[U06] Py：合并两个字典
来源：http://wap.epnwcf.com/Article/details/galukobuj.sHtML

{**a, **b}
来源：http://read.share.epnwcf.com/Article/details/ghuwnqakd.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.bbcook.cn/Article/details/gkygccnch.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.yfazqb.com/Article/details/gvsoccwfe.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.epnwcf.com/Article/details/gensvrfxx.sHtML

[y for x in nested for y in x]
来源：http://read.share.vehdjk.com/Article/details/gkzmhukgc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.sjlbkw.cn/Article/details/ginkaklpc.sHtML

max(d, key=d.get)
来源：http://3g.yfazqb.com/Article/details/gnborcyug.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.vehdjk.com/Article/details/gmayltoow.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.tarul.cn/Article/details/gxgkbfpvt.sHtML


<!-- 参考信息 -->