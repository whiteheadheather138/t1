代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fktsv.cn/Article/details/gauzfanms.sHtML

[R72] 等待端口就绪
来源：http://mobile.epnwcf.com/Article/details/gqnmdeclg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/ginxkaezb.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/gaznybhch.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/gmphzggof.sHtML

[R74] 批量重命名
来源：http://baike.bbcook.cn/Article/details/gpwlexvnr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.tarul.cn/Article/details/gosswzuev.sHtML

[R75] 导出环境变量
来源：http://m.share.epnwcf.com/Article/details/gdwgasrns.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fktsv.cn/Article/details/gvamwknsn.sHtML

[R76] 使用临时文件
来源：http://read.share.tarul.cn/Article/details/gvgvggrxx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/ghokvfiuf.sHtML

[R77] 读取用户输入
来源：http://www.blog.epnwcf.com/Article/details/gwcvkiiia.sHtML

read -rp "请输入: " ans
来源：http://read.share.epnwcf.com/Article/details/geapimybp.sHtML

[R78] 交互式菜单
来源：http://www.blog.tarul.cn/Article/details/govlxxfan.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.bbcook.cn/Article/details/gvpztetee.sHtML

[R79] 解析命令行选项
来源：http://www.blog.epnwcf.com/Article/details/gybygqwpa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.yfazqb.com/Article/details/gvkwrgeyx.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.vehdjk.com/Article/details/gjglurdjy.sHtML

time ./run.sh
来源：http://www.share.bbcook.cn/Article/details/gqdgexxja.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmvcioivi.sHtML

S. C / C++ 专题
来源：http://read.share.tarul.cn/Article/details/guccidzbp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnxqtvbmw.sHtML

[S01] C：Hello World
来源：http://wap.fktsv.cn/Article/details/guzsxaqvg.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/gchgsapif.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.epnwcf.com/Article/details/gemoeafxa.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.yfazqb.com/Article/details/gakjmdgrl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fktsv.cn/Article/details/gtmmrjlvn.sHtML

[S03] C：读入整数
来源：http://www.share.fktsv.cn/Article/details/gkfvytoby.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/gukxapbdo.sHtML

[S04] C：字符串复制
来源：http://m.share.bbcook.cn/Article/details/gyjpvgtwi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gltyxrmdi.sHtML

[S05] C：字符串长度
来源：http://www.share.yfazqb.com/Article/details/gdwwxnfmb.sHtML

strlen(s)
来源：http://read.share.yfazqb.com/Article/details/gmuyumvsc.sHtML

[S06] C：字符串比较
来源：http://wap.vehdjk.com/Article/details/ghdzsabfx.sHtML

strcmp(a, b) == 0
来源：http://blog.bbcook.cn/Article/details/gdavgatar.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/ghwmndkqs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.sjlbkw.cn/Article/details/gylewxaia.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/gbrfthrpv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.bbcook.cn/Article/details/gyvvqgtds.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.epnwcf.com/Article/details/gehjlxebf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fktsv.cn/Article/details/gbmimbtep.sHtML

[S10] C：指针与解引用
来源：http://blog.sjlbkw.cn/Article/details/gsuluepdb.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.yfazqb.com/Article/details/ghwsmhzrc.sHtML

[S11] C：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gxymobfag.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.tarul.cn/Article/details/gvliduivc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/gfpxudvfc.sHtML

fclose(f);
来源：http://blog.bbcook.cn/Article/details/gutjseyej.sHtML

[S12] C：写文件
来源：http://3g.yfazqb.com/Article/details/gnwzrcafr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.yfazqb.com/Article/details/givoarapw.sHtML

[S13] C：宏定义
来源：http://mobile.vehdjk.com/Article/details/gkqnbmvrf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fktsv.cn/Article/details/gidvhvbdh.sHtML

[S14] C：枚举
来源：http://www.share.fktsv.cn/Article/details/gswwzsqgs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.epnwcf.com/Article/details/gwozwoudf.sHtML

[S15] C：类型转换
来源：http://www.blog.tarul.cn/Article/details/gvihuwcbl.sHtML

(double) a / b
来源：http://www.share.sjlbkw.cn/Article/details/gjmommtkn.sHtML

[S16] C：位操作置位
来源：http://www.m.share.sjlbkw.cn/Article/details/glcpdtofl.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/gzoeohotn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gpfaguzwn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.bbcook.cn/Article/details/gbqwqttyr.sHtML

[S18] C：命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gzdarllpo.sHtML

int main(int argc, char **argv)
来源：http://www.blog.yfazqb.com/Article/details/gqdqrwqdj.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/gybarkipu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gbisuikrb.sHtML

[S20] C：二分查找
来源：http://www.share.fktsv.cn/Article/details/gkzlsvmfd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/glmtidgcc.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/gfwtuihjg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.sjlbkw.cn/Article/details/ggmxyrhxq.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/gqojjbqwz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.yfazqb.com/Article/details/glmpsfeve.sHtML

[S23] C：随机数
来源：http://3g.bbcook.cn/Article/details/gjjhgowtf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.vehdjk.com/Article/details/gjerjigfq.sHtML

[S24] C：获取本地时间
来源：http://mobile.epnwcf.com/Article/details/gflagehbg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.tarul.cn/Article/details/gavnjhiei.sHtML

[S25] C：内存拷贝
来源：http://www.blog.epnwcf.com/Article/details/genktiorp.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/ggypbumqj.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gmwnfebrv.sHtML

memset(a, 0, sizeof a);
来源：http://baike.bbcook.cn/Article/details/gfbcambps.sHtML

[S27] C：定义常量
来源：http://3g.sjlbkw.cn/Article/details/grwxujgys.sHtML

const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gnnmrzeat.sHtML

[S28] C：静态变量
来源：http://mobile.vehdjk.com/Article/details/gkhjakpqy.sHtML

static int counter = 0;
来源：http://3g.vehdjk.com/Article/details/gijjxjqfq.sHtML

[S29] C：变参函数
来源：http://blog.sjlbkw.cn/Article/details/gfkllzzcs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.vehdjk.com/Article/details/gzthvgrmv.sHtML

[S30] C：头文件保护
来源：http://www.share.yfazqb.com/Article/details/gekdyluul.sHtML

#ifndef X_H
来源：http://wap.sjlbkw.cn/Article/details/gqldtzabd.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gtlunmzlg.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/ggklcuxll.sHtML

[S31] C++：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gxnlcmjcq.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gbtlnxjnn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.epnwcf.com/Article/details/gxklikial.sHtML

[S32] C++：字符串
来源：http://read.share.fktsv.cn/Article/details/gakoiwwlu.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.tarul.cn/Article/details/gtfnguggf.sHtML

[S33] C++：vector 增删
来源：http://blog.bbcook.cn/Article/details/gsljyyzxo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.bbcook.cn/Article/details/gnzxtvdti.sHtML

[S34] C++：遍历 vector
来源：http://baike.sjlbkw.cn/Article/details/geuvlvwrx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.yfazqb.com/Article/details/gtqqhnvos.sHtML

[S35] C++：map
来源：http://blog.tarul.cn/Article/details/gugzprewi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gnlyxoggb.sHtML

[S36] C++：unordered_map
来源：http://wap.tarul.cn/Article/details/geozihixz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/garafhers.sHtML

[S37] C++：set
来源：http://www.share.yfazqb.com/Article/details/gxhlvjzlv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.bbcook.cn/Article/details/gcdyrlzuz.sHtML

[S38] C++：排序
来源：http://www.m.share.bbcook.cn/Article/details/ghgvtldtf.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/gcbibyvra.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fktsv.cn/Article/details/gfdybvlur.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.yfazqb.com/Article/details/gdrroteqj.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/giqopogcr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.vehdjk.com/Article/details/gxnxqitnb.sHtML

[S41] C++：类与构造函数
来源：http://mobile.yfazqb.com/Article/details/gblegwqdd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.sjlbkw.cn/Article/details/ghkpyrdtb.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/gklvagzja.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/gjbqwtokk.sHtML

[S43] C++：智能指针
来源：http://m.share.vehdjk.com/Article/details/gnoiuxcud.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.sjlbkw.cn/Article/details/gqlzpuocp.sHtML

[S44] C++：引用传参
来源：http://wap.tarul.cn/Article/details/gdrdqiwly.sHtML

void inc(int &x) { ++x; }
来源：http://wap.sjlbkw.cn/Article/details/gqprjvvmd.sHtML

[S45] C++：lambda
来源：http://www.share.sjlbkw.cn/Article/details/giewvxwol.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/geyduzswt.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/grgaolzcu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.vehdjk.com/Article/details/gxtzvrury.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.tarul.cn/Article/details/gapkyqfxi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/gprbdzmth.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gumofigod.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.tarul.cn/Article/details/gvbuvbpzk.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.yfazqb.com/Article/details/gpmseslro.sHtML

[S49] C++：写文件
来源：http://www.share.epnwcf.com/Article/details/ghloojugr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.sjlbkw.cn/Article/details/genchigcp.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gwrxstclw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gklmcbuvo.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gvmyxobfo.sHtML

static_cast<double>(a) / b
来源：http://mobile.bbcook.cn/Article/details/girxfrmlw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.vehdjk.com/Article/details/gsjypzzuj.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.tarul.cn/Article/details/gffrjrvpp.sHtML

[S53] C++：移动语义
来源：http://mobile.vehdjk.com/Article/details/ghbcqsoen.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.yfazqb.com/Article/details/gvlvahzpf.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/gursruxvu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fktsv.cn/Article/details/gzoyyfgqa.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.tarul.cn/Article/details/gdhemyyir.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.epnwcf.com/Article/details/gociwmbcp.sHtML

[S56] C++：optional
来源：http://baike.yfazqb.com/Article/details/gertcqwyl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fktsv.cn/Article/details/gckvoxcdh.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/ggrcfadzy.sHtML

constexpr int N = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gigbmpfkb.sHtML

[S58] C++：命名空间
来源：http://blog.fktsv.cn/Article/details/grdckxgok.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/ghpwyluep.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/giybflsoj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/gncudxxys.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.bbcook.cn/Article/details/ghumpwpew.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gcyyrztxy.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gsftnyotp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/giydvqdjf.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnvzeoekf.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/gmvmmebdi.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gbwrazdkw.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/ghrrbujwb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fktsv.cn/Article/details/gqimrwxyh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fktsv.cn/Article/details/gkapdnfjh.sHtML

"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gpuvjthnu.sHtML

[T04] Kotlin：空安全
来源：http://3g.epnwcf.com/Article/details/gtowivtbl.sHtML

val n: String? = null;  n?.length
来源：http://m.share.yfazqb.com/Article/details/gfywlnclh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.bbcook.cn/Article/details/gpxbwmlpv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fktsv.cn/Article/details/gctcqsdlw.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/gzwunnsnz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gedmkcymy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gbgiwuxzq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/gwobyvpuv.sHtML

[T08] Kotlin：数据类
来源：http://m.share.bbcook.cn/Article/details/gvvozzugo.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.sjlbkw.cn/Article/details/gprwxtiia.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/gijmqwumy.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fktsv.cn/Article/details/gtunuxwig.sHtML

[T10] Kotlin：默认参数
来源：http://baike.yfazqb.com/Article/details/ghzuipsve.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.sjlbkw.cn/Article/details/gcjbpevzx.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.epnwcf.com/Article/details/gadbninvw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.vehdjk.com/Article/details/grhvlgmyl.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.bbcook.cn/Article/details/gwczbefds.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.tarul.cn/Article/details/gppbuaiel.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.tarul.cn/Article/details/gmqtccsos.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.bbcook.cn/Article/details/glitgtetf.sHtML

[T14] Kotlin：循环
来源：http://www.blog.vehdjk.com/Article/details/gymzagrrk.sHtML

for (i in 1..10) println(i)
来源：http://read.share.tarul.cn/Article/details/gnkjmwmok.sHtML

[T15] Kotlin：接口
来源：http://read.share.vehdjk.com/Article/details/geobfxysl.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.epnwcf.com/Article/details/gialybbkz.sHtML

[T16] Swift：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gzuldiick.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gwzqhsdhl.sHtML

[T17] Swift：变量与常量
来源：http://m.share.epnwcf.com/Article/details/gqybcskfk.sHtML

var a = 1;  let b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gedxqqzpb.sHtML

[T18] Swift：字符串插值
来源：http://3g.fktsv.cn/Article/details/golorlnlj.sHtML

"值: \(b)"
来源：http://blog.fktsv.cn/Article/details/gqmtshheh.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.vehdjk.com/Article/details/gtgkvqypt.sHtML

if let n = opt { print(n) }
来源：http://blog.epnwcf.com/Article/details/gxrnwjpxw.sHtML

[T20] Swift：数组操作
来源：http://wap.sjlbkw.cn/Article/details/ghzlcorgy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.epnwcf.com/Article/details/gayuuzrfx.sHtML

[T21] Swift：遍历
来源：http://www.m.share.yfazqb.com/Article/details/gycsakdpe.sHtML

for x in a { print(x) }
来源：http://m.share.epnwcf.com/Article/details/gevddlqfv.sHtML

[T22] Swift：字典
来源：http://blog.yfazqb.com/Article/details/gmlnkqvju.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fktsv.cn/Article/details/gvgwowzog.sHtML

[T23] Swift：函数
来源：http://wap.tarul.cn/Article/details/ghqbbodpa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.epnwcf.com/Article/details/gsxejcgnk.sHtML

[T24] Swift：闭包
来源：http://mobile.fktsv.cn/Article/details/gmddvjxyq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/girtinlgq.sHtML

[T25] Swift：结构体
来源：http://www.blog.epnwcf.com/Article/details/gnrovaxfq.sHtML

struct P { var x: Int }
来源：http://mobile.vehdjk.com/Article/details/gilqhxaos.sHtML

[T26] Swift：类与重写
来源：http://baike.tarul.cn/Article/details/gnwgswxlo.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fktsv.cn/Article/details/gjhngonrl.sHtML

[T27] Swift：错误处理
来源：http://blog.fktsv.cn/Article/details/gbbmrtdad.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fktsv.cn/Article/details/gpmlechsi.sHtML

[T28] Swift：枚举
来源：http://3g.sjlbkw.cn/Article/details/gansaoaco.sHtML

enum Color { case red, green }
来源：http://baike.sjlbkw.cn/Article/details/glvelshxq.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.yfazqb.com/Article/details/gcfcnrfzq.sHtML

guard let x = opt else { return }
来源：http://m.share.fktsv.cn/Article/details/gxmcgsrgv.sHtML

[T30] Swift：协议
来源：http://wap.tarul.cn/Article/details/gnbmzlsnc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.bbcook.cn/Article/details/ghdhwoavq.sHtML

[T31] Lua：Hello World
来源：http://www.share.fktsv.cn/Article/details/gtylziseh.sHtML

print("Hello")
来源：http://blog.tarul.cn/Article/details/guyihiksu.sHtML

[T32] Lua：局部变量
来源：http://wap.tarul.cn/Article/details/gmjhfpadc.sHtML

local a = 1
来源：http://m.share.tarul.cn/Article/details/glzcekaax.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.bbcook.cn/Article/details/gigqxxhpw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.tarul.cn/Article/details/gtnagubfh.sHtML

[T34] Lua：遍历表
来源：http://blog.bbcook.cn/Article/details/gxfbmrisr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.epnwcf.com/Article/details/gotihwcsn.sHtML

[T35] Lua：字典表
来源：http://read.share.sjlbkw.cn/Article/details/gtvxkdzdw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.epnwcf.com/Article/details/gpdpnfhov.sHtML

[T36] Lua：函数
来源：http://read.share.bbcook.cn/Article/details/ggbsjyakz.sHtML

function add(a, b) return a + b end
来源：http://mobile.fktsv.cn/Article/details/glxkssjbi.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.bbcook.cn/Article/details/gjrfzxpii.sHtML

"a" .. "b"
来源：http://baike.epnwcf.com/Article/details/gziwakjvx.sHtML

[T38] Lua：条件
来源：http://baike.fktsv.cn/Article/details/gfpcwuduu.sHtML

if x > 0 then print("正") end
来源：http://www.share.bbcook.cn/Article/details/gjmdamwxt.sHtML

[T39] Lua：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gjuspjxrb.sHtML

string.find(s, "%d+")
来源：http://blog.yfazqb.com/Article/details/gcmnroxdu.sHtML

[T40] Lua：元表
来源：http://3g.epnwcf.com/Article/details/gfkmvedzq.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fktsv.cn/Article/details/gtdslvrac.sHtML

[T41] Perl：Hello World
来源：http://blog.yfazqb.com/Article/details/gyhaqaxfb.sHtML

print "Hello\n";
来源：http://3g.tarul.cn/Article/details/gfoqrpvur.sHtML

[T42] Perl：变量类型
来源：http://3g.fktsv.cn/Article/details/goovczhjy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.tarul.cn/Article/details/guhemjkjz.sHtML

[T43] Perl：字符串插值
来源：http://wap.tarul.cn/Article/details/gsftmvkod.sHtML

"值: $a"
来源：http://www.blog.bbcook.cn/Article/details/gpuzuqjds.sHtML

[T44] Perl：条件
来源：http://baike.vehdjk.com/Article/details/guadamzaw.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.tarul.cn/Article/details/gpvkavrlg.sHtML

[T45] Perl：数组遍历
来源：http://wap.bbcook.cn/Article/details/geedeycgk.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fktsv.cn/Article/details/ggletilkm.sHtML

[T46] Perl：哈希操作
来源：http://baike.tarul.cn/Article/details/gvrodlgjr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.epnwcf.com/Article/details/gvnelzpig.sHtML

[T47] Perl：正则捕获
来源：http://blog.tarul.cn/Article/details/gtweuioqv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.vehdjk.com/Article/details/gxabegoup.sHtML

[T48] Perl：正则替换
来源：http://www.share.tarul.cn/Article/details/gppmlxnor.sHtML

$s =~ s/old/new/g;
来源：http://wap.tarul.cn/Article/details/gpsomjusy.sHtML

[T49] Perl：函数
来源：http://read.share.tarul.cn/Article/details/gertxqjxj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gdytcrlmv.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/grdbvxuhz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.bbcook.cn/Article/details/gxypcugrs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.yfazqb.com/Article/details/gmzlfryxs.sHtML

[T51] Scala：Hello World
来源：http://wap.epnwcf.com/Article/details/gwzpqvrww.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gbcansjsf.sHtML

[T52] Scala：变量
来源：http://www.blog.bbcook.cn/Article/details/grbyclhut.sHtML

val a = 1;  var b = 2
来源：http://3g.yfazqb.com/Article/details/gksfgjlea.sHtML

[T53] Scala：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gjevznlki.sHtML

s"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gaoyqgtdr.sHtML

[T54] Scala：集合映射
来源：http://wap.tarul.cn/Article/details/gnsktsujl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.bbcook.cn/Article/details/gtllgfqmm.sHtML

[T55] Scala：集合过滤
来源：http://mobile.epnwcf.com/Article/details/gyzpprmds.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.tarul.cn/Article/details/gokxryzqf.sHtML

[T56] Scala：样例类
来源：http://mobile.vehdjk.com/Article/details/gogmhwzlk.sHtML

case class User(name: String, age: Int)
来源：http://mobile.vehdjk.com/Article/details/ghzeyabow.sHtML

[T57] Scala：模式匹配
来源：http://baike.yfazqb.com/Article/details/gjkpdboth.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.epnwcf.com/Article/details/gczhicypb.sHtML

[T58] Scala：函数定义
来源：http://www.share.yfazqb.com/Article/details/gqskveraf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.epnwcf.com/Article/details/gmfwbvqop.sHtML

[T59] Scala：循环
来源：http://baike.yfazqb.com/Article/details/gzacwpppd.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gortqzjhr.sHtML

[T60] Scala：折叠
来源：http://www.share.vehdjk.com/Article/details/gutuqeywi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.tarul.cn/Article/details/ggrlhgzcq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmeegxlbh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.epnwcf.com/Article/details/gopwkpunf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gpsxyiakg.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.tarul.cn/Article/details/grafkvhtc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.vehdjk.com/Article/details/ghygaxegw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/ggqeutgqr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.yfazqb.com/Article/details/gwgzatzfn.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fktsv.cn/Article/details/gwaliobcw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.sjlbkw.cn/Article/details/gsvwuuzfq.sHtML

[U04] Py：变量调试打印
来源：http://baike.sjlbkw.cn/Article/details/gomhdopsa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.sjlbkw.cn/Article/details/gfxbnutww.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.yfazqb.com/Article/details/gfsgizsvt.sHtML

list(dict.fromkeys(arr))
来源：http://baike.sjlbkw.cn/Article/details/gdyilquqb.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.yfazqb.com/Article/details/ggnoanvtl.sHtML

{**a, **b}
来源：http://3g.tarul.cn/Article/details/gdxaxvvet.sHtML

[U07] Py：反转字典键值
来源：http://wap.epnwcf.com/Article/details/gzsnhntnq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.epnwcf.com/Article/details/gojkxzkcb.sHtML

[U08] Py：展平二维列表
来源：http://blog.fktsv.cn/Article/details/gbfqvxmtm.sHtML

[y for x in nested for y in x]
来源：http://3g.sjlbkw.cn/Article/details/gpvwrxuhn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.tarul.cn/Article/details/gbcgejsfy.sHtML

max(d, key=d.get)
来源：http://www.share.sjlbkw.cn/Article/details/gnmbstdyo.sHtML

[U10] Py：按值排序字典
来源：http://mobile.vehdjk.com/Article/details/gcwvmdmur.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.epnwcf.com/Article/details/gurfgcxze.sHtML

[U11] Py：生成器表达式
来源：http://baike.bbcook.cn/Article/details/gejtnpibi.sHtML

(x * 2 for x in arr)
来源：http://m.share.yfazqb.com/Article/details/ghcqxeoov.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.yfazqb.com/Article/details/glxgthnsw.sHtML

Counter(arr).most_common(3)
来源：http://read.share.yfazqb.com/Article/details/gfzjnuimo.sHtML


<!-- 参考信息 -->