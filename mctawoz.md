代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gifrpjulr.sHtML

[R72] 等待端口就绪
来源：http://mobile.sjlbkw.cn/Article/details/gpbhftdnq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gioldvfpf.sHtML

[R73] 分割大日志
来源：http://baike.vehdjk.com/Article/details/grwlixfzs.sHtML

split -l 1000 big.log part_
来源：http://blog.epnwcf.com/Article/details/gtjaaoype.sHtML

[R74] 批量重命名
来源：http://www.blog.tarul.cn/Article/details/ggzykxfli.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/glkvbothg.sHtML

[R75] 导出环境变量
来源：http://www.share.epnwcf.com/Article/details/gmvdiqexk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fktsv.cn/Article/details/geozafgcz.sHtML

[R76] 使用临时文件
来源：http://www.share.fktsv.cn/Article/details/gazcccpkc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gbvrwkanq.sHtML

[R77] 读取用户输入
来源：http://wap.vehdjk.com/Article/details/gsfkfdqnr.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.yfazqb.com/Article/details/ghjfgjkug.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gtiptdidp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.yfazqb.com/Article/details/gwtctyqiy.sHtML

[R79] 解析命令行选项
来源：http://read.share.epnwcf.com/Article/details/gtmyfhnxu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.epnwcf.com/Article/details/gwenppfdo.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fktsv.cn/Article/details/gjalgzsem.sHtML

time ./run.sh
来源：http://mobile.tarul.cn/Article/details/ggzmhvjxi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvlkdwwnv.sHtML

S. C / C++ 专题
来源：http://3g.tarul.cn/Article/details/gnulmbzil.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/grbvnhphh.sHtML

[S01] C：Hello World
来源：http://baike.bbcook.cn/Article/details/gipapsbbi.sHtML

#include <stdio.h>
来源：http://baike.yfazqb.com/Article/details/gudxtvmiq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.bbcook.cn/Article/details/gwvymkrez.sHtML

[S02] C：变量与格式化输出
来源：http://wap.yfazqb.com/Article/details/gbxjaoggq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.vehdjk.com/Article/details/gtzygifta.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/gghuadrre.sHtML

int x; scanf("%d", &x);
来源：http://blog.bbcook.cn/Article/details/gdfntkazd.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/gmvduyiwh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.yfazqb.com/Article/details/gxkjubjpo.sHtML

[S05] C：字符串长度
来源：http://3g.yfazqb.com/Article/details/ggaggivvk.sHtML

strlen(s)
来源：http://3g.bbcook.cn/Article/details/givhqrsbz.sHtML

[S06] C：字符串比较
来源：http://read.share.fktsv.cn/Article/details/glpacrmou.sHtML

strcmp(a, b) == 0
来源：http://3g.vehdjk.com/Article/details/gzbbjnbrd.sHtML

[S07] C：数组遍历求和
来源：http://m.share.vehdjk.com/Article/details/gbgdhqeqw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.bbcook.cn/Article/details/gwhnrrked.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.sjlbkw.cn/Article/details/gckskkwgi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/gowzeszww.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.yfazqb.com/Article/details/gdvosmayt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.tarul.cn/Article/details/gxpfnehfr.sHtML

[S10] C：指针与解引用
来源：http://read.share.vehdjk.com/Article/details/gzpkgpsus.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.tarul.cn/Article/details/gtadwxxrd.sHtML

[S11] C：逐行读文件
来源：http://3g.bbcook.cn/Article/details/ggqfxcxku.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnciyaval.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/gcnucrkzr.sHtML

fclose(f);
来源：http://www.share.fktsv.cn/Article/details/gokdubriv.sHtML

[S12] C：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/ggqbnqsgb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gmnmzisrr.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/goyjocmzf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.yfazqb.com/Article/details/gbqeibusz.sHtML

[S14] C：枚举
来源：http://read.share.epnwcf.com/Article/details/gcxdvbxqv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.sjlbkw.cn/Article/details/gjksobpja.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/gmuakgaug.sHtML

(double) a / b
来源：http://m.share.epnwcf.com/Article/details/geuyjsxcf.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/gvczjwytf.sHtML

x |= (1 << 3);
来源：http://www.blog.vehdjk.com/Article/details/glbfvlzjf.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gjmqvtghj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.tarul.cn/Article/details/gbilfzmar.sHtML

[S18] C：命令行参数
来源：http://3g.vehdjk.com/Article/details/gqompvtcp.sHtML

int main(int argc, char **argv)
来源：http://wap.fktsv.cn/Article/details/ghzwjfykz.sHtML

[S19] C：快速排序
来源：http://www.blog.epnwcf.com/Article/details/gtufendse.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gxfevsjut.sHtML

[S20] C：二分查找
来源：http://3g.bbcook.cn/Article/details/gmonczsjs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gqamtersj.sHtML

[S21] C：字符类别判断
来源：http://www.share.fktsv.cn/Article/details/gplwwbtib.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.sjlbkw.cn/Article/details/gwwrrgpws.sHtML

[S22] C：字符串转数字
来源：http://www.share.bbcook.cn/Article/details/gbstfhmfe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.sjlbkw.cn/Article/details/gskkogcib.sHtML

[S23] C：随机数
来源：http://www.share.bbcook.cn/Article/details/gqtpjnxqd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.yfazqb.com/Article/details/gfqotbpzy.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/gjtqzobzg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.vehdjk.com/Article/details/groiyeonj.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gkhgmygfk.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/godhoocdc.sHtML

[S26] C：内存清零
来源：http://m.share.epnwcf.com/Article/details/gpqmzrhyj.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fktsv.cn/Article/details/gtlqrrhtq.sHtML

[S27] C：定义常量
来源：http://mobile.epnwcf.com/Article/details/gfvdirqrl.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gsrjxsulz.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/gzbopdunh.sHtML

static int counter = 0;
来源：http://m.share.epnwcf.com/Article/details/geizaldle.sHtML

[S29] C：变参函数
来源：http://baike.fktsv.cn/Article/details/gdspmforo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.sjlbkw.cn/Article/details/gjeusjynt.sHtML

[S30] C：头文件保护
来源：http://blog.yfazqb.com/Article/details/gzebekrag.sHtML

#ifndef X_H
来源：http://baike.bbcook.cn/Article/details/grqcaorrp.sHtML

#define X_H
来源：http://www.m.share.bbcook.cn/Article/details/geaizjidn.sHtML

#endif
来源：http://blog.bbcook.cn/Article/details/glnvbqvog.sHtML

[S31] C++：Hello World
来源：http://mobile.tarul.cn/Article/details/glenqxqpi.sHtML

#include <iostream>
来源：http://www.m.share.sjlbkw.cn/Article/details/gurvvyncc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.epnwcf.com/Article/details/gejogqqiq.sHtML

[S32] C++：字符串
来源：http://www.m.share.vehdjk.com/Article/details/gnyefnqum.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.tarul.cn/Article/details/gwzuquwzr.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.tarul.cn/Article/details/gohayuqup.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/gzgzlvnsl.sHtML

[S34] C++：遍历 vector
来源：http://wap.vehdjk.com/Article/details/gpjzfmcdi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.tarul.cn/Article/details/gukjfhelh.sHtML

[S35] C++：map
来源：http://www.share.yfazqb.com/Article/details/gisleuvki.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gfrvneupx.sHtML

[S36] C++：unordered_map
来源：http://m.share.fktsv.cn/Article/details/gyfhlwgeh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/ghcaswudz.sHtML

[S37] C++：set
来源：http://read.share.sjlbkw.cn/Article/details/gavjhkfdi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.bbcook.cn/Article/details/gdtvampqt.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gldwxfsma.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gfvpvyymk.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.yfazqb.com/Article/details/ghtzbehax.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fktsv.cn/Article/details/gwnhejhwm.sHtML

[S40] C++：查找元素
来源：http://www.m.share.vehdjk.com/Article/details/gmxruquai.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.tarul.cn/Article/details/guygcarqc.sHtML

[S41] C++：类与构造函数
来源：http://read.share.tarul.cn/Article/details/gzvslxcts.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/gnpordvju.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.yfazqb.com/Article/details/gnentxwne.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fktsv.cn/Article/details/ggxotjgve.sHtML

[S43] C++：智能指针
来源：http://3g.fktsv.cn/Article/details/gnnahzknf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.tarul.cn/Article/details/glfgwqaoh.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gbozavzep.sHtML

void inc(int &x) { ++x; }
来源：http://3g.epnwcf.com/Article/details/gdfchalyh.sHtML

[S45] C++：lambda
来源：http://www.share.fktsv.cn/Article/details/gngzclxsb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwxpmxtf.sHtML

[S46] C++：函数模板
来源：http://www.m.share.yfazqb.com/Article/details/gkfckrpuy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/ggadginpi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.bbcook.cn/Article/details/gdzxxycpw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.vehdjk.com/Article/details/ggjxrdwhp.sHtML

[S48] C++：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gqxtchgwq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.vehdjk.com/Article/details/gdeszkfte.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fktsv.cn/Article/details/guvxzalrw.sHtML

[S49] C++：写文件
来源：http://www.blog.bbcook.cn/Article/details/ghbqjzjzu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.tarul.cn/Article/details/gyprettui.sHtML

[S50] C++：格式化数字
来源：http://blog.vehdjk.com/Article/details/gaauocvyx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gggcgwpoc.sHtML

[S51] C++：显式类型转换
来源：http://baike.tarul.cn/Article/details/ghfujumer.sHtML

static_cast<double>(a) / b
来源：http://www.share.bbcook.cn/Article/details/gkmswsmzi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.sjlbkw.cn/Article/details/goapvvtuz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.sjlbkw.cn/Article/details/giqvobcsj.sHtML

[S53] C++：移动语义
来源：http://wap.vehdjk.com/Article/details/gquphrruq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.tarul.cn/Article/details/ganebulwr.sHtML

[S54] C++：异常处理
来源：http://wap.vehdjk.com/Article/details/gksldjyic.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.yfazqb.com/Article/details/glsymqeej.sHtML

[S55] C++：结构化绑定
来源：http://baike.tarul.cn/Article/details/gamfvyipz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/gkfmciqmi.sHtML

[S56] C++：optional
来源：http://baike.epnwcf.com/Article/details/gvbuheqch.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.vehdjk.com/Article/details/gtqqbyxyv.sHtML

[S57] C++：编译期常量
来源：http://www.blog.vehdjk.com/Article/details/gihztverq.sHtML

constexpr int N = 10;
来源：http://read.share.sjlbkw.cn/Article/details/grivxqxcf.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/gqnakbsst.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.epnwcf.com/Article/details/gykdabkrv.sHtML

[S59] C++：静态断言
来源：http://3g.yfazqb.com/Article/details/gshouremr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.vehdjk.com/Article/details/gyyfpvzxs.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/gfxbeqtvw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gfgqevdnh.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gyqqdajth.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/gzvismioi.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwozeshjq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gkymipguu.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gopojxwpi.sHtML

[T02] Kotlin：变量
来源：http://baike.vehdjk.com/Article/details/gtiysrirm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.yfazqb.com/Article/details/ghtlcuzdd.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fktsv.cn/Article/details/gliorsive.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/glduizpog.sHtML

[T04] Kotlin：空安全
来源：http://wap.fktsv.cn/Article/details/gujgvdbyo.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.tarul.cn/Article/details/gubgmtzuk.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.tarul.cn/Article/details/gybumloat.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.yfazqb.com/Article/details/gcfjplzzl.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gdpgfzjde.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.vehdjk.com/Article/details/gasjklvle.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gsawuejpq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fktsv.cn/Article/details/gmxyqdoeo.sHtML

[T08] Kotlin：数据类
来源：http://www.share.tarul.cn/Article/details/gowwvgboq.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.epnwcf.com/Article/details/gxonokfvo.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.tarul.cn/Article/details/gkhdflzsx.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.epnwcf.com/Article/details/gwmetjzlx.sHtML

[T10] Kotlin：默认参数
来源：http://3g.sjlbkw.cn/Article/details/gyjilbqbu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.bbcook.cn/Article/details/gwnudodna.sHtML

[T11] Kotlin：协程
来源：http://3g.vehdjk.com/Article/details/gtmwzcmjm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.epnwcf.com/Article/details/goxaatmzq.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/gfhdewrxs.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/giduzftan.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.bbcook.cn/Article/details/gjkmbfqcv.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.epnwcf.com/Article/details/gshogdcob.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/gfydxulvk.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gkbegujca.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/gpgojusin.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gzwgpwcgi.sHtML

[T16] Swift：Hello World
来源：http://read.share.vehdjk.com/Article/details/ggjasxnbl.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gsafyidmk.sHtML

[T17] Swift：变量与常量
来源：http://3g.bbcook.cn/Article/details/gaesrhrok.sHtML

var a = 1;  let b = 2
来源：http://mobile.yfazqb.com/Article/details/gtnrmxdez.sHtML

[T18] Swift：字符串插值
来源：http://wap.vehdjk.com/Article/details/gtbczyowm.sHtML

"值: \(b)"
来源：http://www.blog.bbcook.cn/Article/details/gysjfutpq.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gnyvdiyrd.sHtML

if let n = opt { print(n) }
来源：http://baike.yfazqb.com/Article/details/glqaddqwi.sHtML

[T20] Swift：数组操作
来源：http://baike.vehdjk.com/Article/details/gafmigotv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.sjlbkw.cn/Article/details/ghgmewdks.sHtML

[T21] Swift：遍历
来源：http://m.share.sjlbkw.cn/Article/details/gjewxcxiz.sHtML

for x in a { print(x) }
来源：http://wap.yfazqb.com/Article/details/gxnmocutk.sHtML

[T22] Swift：字典
来源：http://www.m.share.yfazqb.com/Article/details/gkdftlgxn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.epnwcf.com/Article/details/gdmrfkkst.sHtML

[T23] Swift：函数
来源：http://blog.yfazqb.com/Article/details/gizqbwgqt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gjumntfax.sHtML

[T24] Swift：闭包
来源：http://3g.vehdjk.com/Article/details/gpcpkbvle.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.epnwcf.com/Article/details/gmjikjnje.sHtML

[T25] Swift：结构体
来源：http://read.share.epnwcf.com/Article/details/gcqmunfcc.sHtML

struct P { var x: Int }
来源：http://read.share.sjlbkw.cn/Article/details/gldhzxswf.sHtML

[T26] Swift：类与重写
来源：http://www.share.yfazqb.com/Article/details/gldqivlnq.sHtML

class A: Base { override func f() {} }
来源：http://3g.fktsv.cn/Article/details/gyhnzjpgd.sHtML

[T27] Swift：错误处理
来源：http://blog.fktsv.cn/Article/details/gocgxqkju.sHtML

do { try f() } catch { print(error) }
来源：http://baike.tarul.cn/Article/details/gsjrrhqok.sHtML

[T28] Swift：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gsojhhusj.sHtML

enum Color { case red, green }
来源：http://m.share.sjlbkw.cn/Article/details/gtibpwbin.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.sjlbkw.cn/Article/details/gvxmdhicj.sHtML

guard let x = opt else { return }
来源：http://baike.sjlbkw.cn/Article/details/gabzkcfww.sHtML

[T30] Swift：协议
来源：http://www.share.fktsv.cn/Article/details/glaigjbgw.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.tarul.cn/Article/details/gqyjkhxhe.sHtML

[T31] Lua：Hello World
来源：http://3g.fktsv.cn/Article/details/gohuqwhog.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gqfpbxeps.sHtML

[T32] Lua：局部变量
来源：http://blog.vehdjk.com/Article/details/ggeoxsyic.sHtML

local a = 1
来源：http://www.m.share.epnwcf.com/Article/details/ghhdwbfpo.sHtML

[T33] Lua：表（数组）
来源：http://blog.vehdjk.com/Article/details/gzxtnhrry.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.bbcook.cn/Article/details/gmxkuzfie.sHtML

[T34] Lua：遍历表
来源：http://blog.yfazqb.com/Article/details/gqixpahry.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/gligqkokt.sHtML

[T35] Lua：字典表
来源：http://blog.vehdjk.com/Article/details/gjzzdsuoz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.tarul.cn/Article/details/gzyghunmv.sHtML

[T36] Lua：函数
来源：http://read.share.epnwcf.com/Article/details/gtrwprcsw.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.tarul.cn/Article/details/goonvkpfd.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.epnwcf.com/Article/details/gnvnhhafz.sHtML

"a" .. "b"
来源：http://www.share.yfazqb.com/Article/details/gzwuamuei.sHtML

[T38] Lua：条件
来源：http://mobile.bbcook.cn/Article/details/gnsbpufji.sHtML

if x > 0 then print("正") end
来源：http://m.share.sjlbkw.cn/Article/details/gaqnbjchk.sHtML

[T39] Lua：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/gccjtfdmg.sHtML

string.find(s, "%d+")
来源：http://wap.yfazqb.com/Article/details/gxrkyohdh.sHtML

[T40] Lua：元表
来源：http://read.share.yfazqb.com/Article/details/gxtgslfha.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fktsv.cn/Article/details/gfbybdkwt.sHtML

[T41] Perl：Hello World
来源：http://blog.fktsv.cn/Article/details/gphchfsap.sHtML

print "Hello\n";
来源：http://wap.tarul.cn/Article/details/gxssqtvht.sHtML

[T42] Perl：变量类型
来源：http://www.share.epnwcf.com/Article/details/gluayhhju.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.epnwcf.com/Article/details/grargbxoo.sHtML

[T43] Perl：字符串插值
来源：http://mobile.yfazqb.com/Article/details/goncwzjed.sHtML

"值: $a"
来源：http://read.share.vehdjk.com/Article/details/gxbegajgb.sHtML

[T44] Perl：条件
来源：http://read.share.bbcook.cn/Article/details/gremgyjcp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.yfazqb.com/Article/details/gtxfismml.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fktsv.cn/Article/details/gjclugbsc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.bbcook.cn/Article/details/guztkzsae.sHtML

[T46] Perl：哈希操作
来源：http://baike.tarul.cn/Article/details/gsxwoohjg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.tarul.cn/Article/details/gquvncbvv.sHtML

[T47] Perl：正则捕获
来源：http://wap.vehdjk.com/Article/details/gkdcdproq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.yfazqb.com/Article/details/gdmjrkhpx.sHtML

[T48] Perl：正则替换
来源：http://m.share.yfazqb.com/Article/details/gpkrukdoy.sHtML

$s =~ s/old/new/g;
来源：http://read.share.bbcook.cn/Article/details/gzgonshtz.sHtML

[T49] Perl：函数
来源：http://mobile.fktsv.cn/Article/details/gevutwvmi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gkotjsqjs.sHtML

[T50] Perl：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gvgukeeqi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.sjlbkw.cn/Article/details/gxxzdewky.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.epnwcf.com/Article/details/gpwmplvtd.sHtML

[T51] Scala：Hello World
来源：http://read.share.bbcook.cn/Article/details/gkuflprxe.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/guoyufavl.sHtML

[T52] Scala：变量
来源：http://m.share.bbcook.cn/Article/details/gtglyaxtg.sHtML

val a = 1;  var b = 2
来源：http://www.share.tarul.cn/Article/details/gvyqsytdf.sHtML

[T53] Scala：字符串插值
来源：http://m.share.tarul.cn/Article/details/gzzzndurp.sHtML

s"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/grcnxqgoq.sHtML

[T54] Scala：集合映射
来源：http://3g.epnwcf.com/Article/details/goiavqcxb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gkskyqbvd.sHtML

[T55] Scala：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gxevmnitp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.yfazqb.com/Article/details/gcxfbqjwm.sHtML

[T56] Scala：样例类
来源：http://www.share.bbcook.cn/Article/details/gdbjzrabw.sHtML

case class User(name: String, age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gdqmsxxcs.sHtML

[T57] Scala：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gwzpycluk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.epnwcf.com/Article/details/gvdyllnxf.sHtML

[T58] Scala：函数定义
来源：http://wap.yfazqb.com/Article/details/gnmiflhhx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.tarul.cn/Article/details/gvndnwoog.sHtML

[T59] Scala：循环
来源：http://mobile.sjlbkw.cn/Article/details/gmlpjkzar.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.epnwcf.com/Article/details/gqcoyjond.sHtML

[T60] Scala：折叠
来源：http://read.share.vehdjk.com/Article/details/gbqvplnzz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/gksifmreo.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/grdkgnudq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/geqqexuiy.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gidsouzcv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.epnwcf.com/Article/details/gxlunmoas.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.epnwcf.com/Article/details/gytcptlwk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.sjlbkw.cn/Article/details/gkbgqlfme.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.sjlbkw.cn/Article/details/gtjqwpfso.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/gxeelepae.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.vehdjk.com/Article/details/gwcyhszgy.sHtML

[U04] Py：变量调试打印
来源：http://baike.fktsv.cn/Article/details/gsjidabqd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.bbcook.cn/Article/details/gmcbtjayz.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.vehdjk.com/Article/details/gyfvaywrz.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gtsnouzjk.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gxurxranw.sHtML

{**a, **b}
来源：http://www.m.share.yfazqb.com/Article/details/gtrdmbuob.sHtML

[U07] Py：反转字典键值
来源：http://mobile.bbcook.cn/Article/details/gcyedwjgp.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.vehdjk.com/Article/details/gzsxzduti.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gmsfetard.sHtML

[y for x in nested for y in x]
来源：http://read.share.sjlbkw.cn/Article/details/gvmcgruyi.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.yfazqb.com/Article/details/gacjeqxce.sHtML

max(d, key=d.get)
来源：http://m.share.fktsv.cn/Article/details/gdnocadsw.sHtML

[U10] Py：按值排序字典
来源：http://mobile.sjlbkw.cn/Article/details/ggvcfcvxh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.yfazqb.com/Article/details/ghabqavvu.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fktsv.cn/Article/details/gsevdawqj.sHtML

(x * 2 for x in arr)
来源：http://m.share.vehdjk.com/Article/details/gufbswkgi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.yfazqb.com/Article/details/gnttsexyz.sHtML

Counter(arr).most_common(3)
来源：http://3g.yfazqb.com/Article/details/glizhtyyz.sHtML


<!-- 参考信息 -->