代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://wap.yfazqb.com/Article/details/ggppioryh.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/ghgxujtni.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gwpykcuvs.sHtML

[R77] 读取用户输入
来源：http://m.share.fktsv.cn/Article/details/glrltrxtw.sHtML

read -rp "请输入: " ans
来源：http://mobile.vehdjk.com/Article/details/gquiwyuai.sHtML

[R78] 交互式菜单
来源：http://wap.sjlbkw.cn/Article/details/gkgocelhe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fktsv.cn/Article/details/gvvfvdjoc.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.epnwcf.com/Article/details/guigfzfyw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.sjlbkw.cn/Article/details/gjeedrous.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.bbcook.cn/Article/details/gfilvpctv.sHtML

time ./run.sh
来源：http://read.share.bbcook.cn/Article/details/ghkvevayv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/goevsnpmn.sHtML

S. C / C++ 专题
来源：http://3g.yfazqb.com/Article/details/gdkasswqz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggerllygq.sHtML

[S01] C：Hello World
来源：http://baike.epnwcf.com/Article/details/gjlxxtzxo.sHtML

#include <stdio.h>
来源：http://m.share.sjlbkw.cn/Article/details/ghvwzrblx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.epnwcf.com/Article/details/gkrbzxjcz.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.vehdjk.com/Article/details/gjkhumrgi.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.yfazqb.com/Article/details/gbqtqnopr.sHtML

[S03] C：读入整数
来源：http://mobile.tarul.cn/Article/details/gjveltcyy.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/gelfidktg.sHtML

[S04] C：字符串复制
来源：http://www.blog.yfazqb.com/Article/details/gzsjsrnyx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.yfazqb.com/Article/details/gtodkkpzb.sHtML

[S05] C：字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/girkfcxil.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/gyvwjkfjm.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/gpajijhrd.sHtML

strcmp(a, b) == 0
来源：http://wap.vehdjk.com/Article/details/gmgqnwmnn.sHtML

[S07] C：数组遍历求和
来源：http://baike.epnwcf.com/Article/details/gdzfsmezd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.sjlbkw.cn/Article/details/gqwvytput.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/gpndasyix.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.vehdjk.com/Article/details/gjgutsifa.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/ggrmqdhab.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/gyodvyayo.sHtML

[S10] C：指针与解引用
来源：http://m.share.fktsv.cn/Article/details/geonluzhu.sHtML

int *p = &a;  *p = 5;
来源：http://wap.vehdjk.com/Article/details/gonhtvxml.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gtnfeuxmy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.epnwcf.com/Article/details/gywrgbjmr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.yfazqb.com/Article/details/giywunzoi.sHtML

fclose(f);
来源：http://www.m.share.bbcook.cn/Article/details/gveunbyav.sHtML

[S12] C：写文件
来源：http://www.share.yfazqb.com/Article/details/gycaqfixi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/gnfviyonf.sHtML

[S13] C：宏定义
来源：http://3g.epnwcf.com/Article/details/gtucwzqrj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.tarul.cn/Article/details/gtytevsyk.sHtML

[S14] C：枚举
来源：http://m.share.bbcook.cn/Article/details/ghfjngzka.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.bbcook.cn/Article/details/gckzeyksf.sHtML

[S15] C：类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gsvzispav.sHtML

(double) a / b
来源：http://www.share.epnwcf.com/Article/details/gbmkpixyp.sHtML

[S16] C：位操作置位
来源：http://read.share.sjlbkw.cn/Article/details/gfoaqavmm.sHtML

x |= (1 << 3);
来源：http://www.share.fktsv.cn/Article/details/gjtbmfpuq.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gywtfvnjn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.epnwcf.com/Article/details/goboebnvw.sHtML

[S18] C：命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gyldigtvs.sHtML

int main(int argc, char **argv)
来源：http://blog.epnwcf.com/Article/details/gqkvqmhoy.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/gnuanjasf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gpgwridbs.sHtML

[S20] C：二分查找
来源：http://m.share.vehdjk.com/Article/details/gkqzrpahx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gcfyhzezr.sHtML

[S21] C：字符类别判断
来源：http://www.blog.vehdjk.com/Article/details/gwwrjolwv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gfbmubqmd.sHtML

[S22] C：字符串转数字
来源：http://www.share.sjlbkw.cn/Article/details/gdknlnnnq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.yfazqb.com/Article/details/gonvmkaiv.sHtML

[S23] C：随机数
来源：http://3g.fktsv.cn/Article/details/glnenbejs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.tarul.cn/Article/details/goejnnlwd.sHtML

[S24] C：获取本地时间
来源：http://wap.fktsv.cn/Article/details/grpesvqzr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/gljqwxuxb.sHtML

[S25] C：内存拷贝
来源：http://m.share.fktsv.cn/Article/details/gpuatjxft.sHtML

memcpy(dst, src, n);
来源：http://baike.fktsv.cn/Article/details/gggwwtjcs.sHtML

[S26] C：内存清零
来源：http://m.share.tarul.cn/Article/details/gpvhflirr.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gsvijeuvl.sHtML

[S27] C：定义常量
来源：http://baike.fktsv.cn/Article/details/glokvmuin.sHtML

const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gwrxkzlcc.sHtML

[S28] C：静态变量
来源：http://wap.vehdjk.com/Article/details/gbsvmjbis.sHtML

static int counter = 0;
来源：http://www.m.share.vehdjk.com/Article/details/gvlmsxwog.sHtML

[S29] C：变参函数
来源：http://www.m.share.fktsv.cn/Article/details/gfftyvgbk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.tarul.cn/Article/details/gthriuviu.sHtML

[S30] C：头文件保护
来源：http://www.m.share.tarul.cn/Article/details/gsvmbjxmf.sHtML

#ifndef X_H
来源：http://blog.vehdjk.com/Article/details/gjdlvuweh.sHtML

#define X_H
来源：http://mobile.sjlbkw.cn/Article/details/gpcfyxpah.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gmloudurj.sHtML

[S31] C++：Hello World
来源：http://blog.vehdjk.com/Article/details/glwkolxsd.sHtML

#include <iostream>
来源：http://blog.epnwcf.com/Article/details/gbukgayvk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.bbcook.cn/Article/details/gwdxzirrh.sHtML

[S32] C++：字符串
来源：http://www.blog.tarul.cn/Article/details/ghrnysdfx.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/gvogbuitg.sHtML

[S33] C++：vector 增删
来源：http://3g.bbcook.cn/Article/details/gqxlykezy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.epnwcf.com/Article/details/gdccqingi.sHtML

[S34] C++：遍历 vector
来源：http://blog.yfazqb.com/Article/details/gsobrqysh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.tarul.cn/Article/details/ggskzpgyh.sHtML

[S35] C++：map
来源：http://wap.sjlbkw.cn/Article/details/gbqenbvpo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gatxjoddj.sHtML

[S36] C++：unordered_map
来源：http://baike.bbcook.cn/Article/details/gxmlfonbj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gdkrbszul.sHtML

[S37] C++：set
来源：http://wap.sjlbkw.cn/Article/details/gtlucfrgo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fktsv.cn/Article/details/gjdoczkpt.sHtML

[S38] C++：排序
来源：http://www.m.share.epnwcf.com/Article/details/gbfwuhron.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/gqcxbuany.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/gvqetuldw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.bbcook.cn/Article/details/ghwwlgoma.sHtML

[S40] C++：查找元素
来源：http://www.blog.epnwcf.com/Article/details/gqmlujtzm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.yfazqb.com/Article/details/gylovmsww.sHtML

[S41] C++：类与构造函数
来源：http://mobile.vehdjk.com/Article/details/gmaxtexqs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fktsv.cn/Article/details/gpmerknjo.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.bbcook.cn/Article/details/gtobswrsc.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.vehdjk.com/Article/details/gktqhymef.sHtML

[S43] C++：智能指针
来源：http://read.share.yfazqb.com/Article/details/gsddhtsmo.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.yfazqb.com/Article/details/gpxrwqscw.sHtML

[S44] C++：引用传参
来源：http://blog.tarul.cn/Article/details/gyilgxykv.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.bbcook.cn/Article/details/gwdmddvqa.sHtML

[S45] C++：lambda
来源：http://read.share.epnwcf.com/Article/details/gvgsodcxi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.yfazqb.com/Article/details/gqpxwojiq.sHtML

[S46] C++：函数模板
来源：http://mobile.tarul.cn/Article/details/gxlqrzviw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.yfazqb.com/Article/details/gebfmexan.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.tarul.cn/Article/details/gzayfqyjb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.vehdjk.com/Article/details/ggczewryc.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/grjdtiguj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.bbcook.cn/Article/details/gqbzdhwkq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.epnwcf.com/Article/details/gfztgrqax.sHtML

[S49] C++：写文件
来源：http://baike.fktsv.cn/Article/details/gvsyecwcc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.sjlbkw.cn/Article/details/gqlttdteg.sHtML

[S50] C++：格式化数字
来源：http://read.share.vehdjk.com/Article/details/gtnnsihiq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.yfazqb.com/Article/details/gkvrdeyhi.sHtML

[S51] C++：显式类型转换
来源：http://wap.bbcook.cn/Article/details/gjxihgzpt.sHtML

static_cast<double>(a) / b
来源：http://blog.epnwcf.com/Article/details/ggcanxmjb.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gjnqevldb.sHtML

int size() const noexcept { return n_; }
来源：http://wap.sjlbkw.cn/Article/details/giqetyaah.sHtML

[S53] C++：移动语义
来源：http://wap.fktsv.cn/Article/details/gurzvdbix.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.yfazqb.com/Article/details/ggwbpnjzr.sHtML

[S54] C++：异常处理
来源：http://m.share.epnwcf.com/Article/details/gdrraowtj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.tarul.cn/Article/details/gxrxycoyn.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.tarul.cn/Article/details/gbpiqzzdy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/gghvixlnx.sHtML

[S56] C++：optional
来源：http://wap.tarul.cn/Article/details/gyepbexiz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.sjlbkw.cn/Article/details/gvixytwda.sHtML

[S57] C++：编译期常量
来源：http://www.blog.epnwcf.com/Article/details/giavrwrcv.sHtML

constexpr int N = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gtejomwut.sHtML

[S58] C++：命名空间
来源：http://www.share.vehdjk.com/Article/details/ghekesldy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.bbcook.cn/Article/details/gzayfaecg.sHtML

[S59] C++：静态断言
来源：http://m.share.bbcook.cn/Article/details/gdrnpaiti.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.yfazqb.com/Article/details/gnqtsgklm.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.vehdjk.com/Article/details/gsztzhjdk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/ghrxojwcs.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gvgepbvll.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.sjlbkw.cn/Article/details/gmcgztepr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gyeeilgig.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gqkpumilu.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gtxbawful.sHtML

[T02] Kotlin：变量
来源：http://m.share.tarul.cn/Article/details/guwawqefz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.yfazqb.com/Article/details/gbpqxuazu.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/gnxpvhivb.sHtML

"值: $b"
来源：http://3g.tarul.cn/Article/details/gfuuzaahw.sHtML

[T04] Kotlin：空安全
来源：http://3g.tarul.cn/Article/details/gzmbgxvqo.sHtML

val n: String? = null;  n?.length
来源：http://www.share.tarul.cn/Article/details/gbuczykym.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.sjlbkw.cn/Article/details/gjezbiuyf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.bbcook.cn/Article/details/gqppyenlh.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.bbcook.cn/Article/details/gicaiojfv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gccvjkmbb.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.tarul.cn/Article/details/gnzjwaczn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.sjlbkw.cn/Article/details/grpichygd.sHtML

[T08] Kotlin：数据类
来源：http://mobile.vehdjk.com/Article/details/gkbvxmiel.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.vehdjk.com/Article/details/geqhzvfpe.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fktsv.cn/Article/details/gppuixxkl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fktsv.cn/Article/details/gmjaxkdsc.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.yfazqb.com/Article/details/ggdlnkiuz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.yfazqb.com/Article/details/gtenfexax.sHtML

[T11] Kotlin：协程
来源：http://3g.fktsv.cn/Article/details/gqhmdmnwf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.epnwcf.com/Article/details/gzcoerbmb.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.epnwcf.com/Article/details/gqzpbalix.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fktsv.cn/Article/details/gxyxsrckx.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.vehdjk.com/Article/details/grsqyjimy.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fktsv.cn/Article/details/gghqnzrfk.sHtML

[T14] Kotlin：循环
来源：http://3g.yfazqb.com/Article/details/ghbiskkbn.sHtML

for (i in 1..10) println(i)
来源：http://3g.vehdjk.com/Article/details/gvmgpiyyq.sHtML

[T15] Kotlin：接口
来源：http://www.share.bbcook.cn/Article/details/gkcckcabs.sHtML

interface Shape { fun area(): Double }
来源：http://baike.tarul.cn/Article/details/gttpcoqrh.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gbzxmcpfw.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gqrrogmfu.sHtML

[T17] Swift：变量与常量
来源：http://3g.yfazqb.com/Article/details/gefwahjlb.sHtML

var a = 1;  let b = 2
来源：http://mobile.bbcook.cn/Article/details/gvlkqioma.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gkfiafqkj.sHtML

"值: \(b)"
来源：http://baike.bbcook.cn/Article/details/gbblnvsol.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.yfazqb.com/Article/details/gwdgppiol.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.yfazqb.com/Article/details/gfvjozcyg.sHtML

[T20] Swift：数组操作
来源：http://m.share.vehdjk.com/Article/details/gsulyvomh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.sjlbkw.cn/Article/details/gzchypslg.sHtML

[T21] Swift：遍历
来源：http://3g.tarul.cn/Article/details/gqbanatfw.sHtML

for x in a { print(x) }
来源：http://mobile.tarul.cn/Article/details/gkwizhqqk.sHtML

[T22] Swift：字典
来源：http://www.blog.epnwcf.com/Article/details/gplixfedf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.epnwcf.com/Article/details/ghhgrpdwl.sHtML

[T23] Swift：函数
来源：http://www.share.tarul.cn/Article/details/guqmgvxff.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.epnwcf.com/Article/details/gbazsuzyi.sHtML

[T24] Swift：闭包
来源：http://mobile.epnwcf.com/Article/details/gfbkhphnq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.bbcook.cn/Article/details/gnenbckqs.sHtML

[T25] Swift：结构体
来源：http://read.share.vehdjk.com/Article/details/gkmlmrlxz.sHtML

struct P { var x: Int }
来源：http://www.blog.tarul.cn/Article/details/gmtyyerhq.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.tarul.cn/Article/details/gpduzyruu.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.bbcook.cn/Article/details/ghmuuxahg.sHtML

[T27] Swift：错误处理
来源：http://read.share.bbcook.cn/Article/details/gikkgluvw.sHtML

do { try f() } catch { print(error) }
来源：http://3g.vehdjk.com/Article/details/goehsmuad.sHtML

[T28] Swift：枚举
来源：http://3g.bbcook.cn/Article/details/gaxvgismq.sHtML

enum Color { case red, green }
来源：http://www.share.bbcook.cn/Article/details/gwhscnonv.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.vehdjk.com/Article/details/gdunwraaf.sHtML

guard let x = opt else { return }
来源：http://www.share.tarul.cn/Article/details/gktnkwdji.sHtML

[T30] Swift：协议
来源：http://www.share.bbcook.cn/Article/details/gmyxgawej.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.bbcook.cn/Article/details/grisfhwxg.sHtML

[T31] Lua：Hello World
来源：http://wap.sjlbkw.cn/Article/details/galvnecpb.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gwfdwikjf.sHtML

[T32] Lua：局部变量
来源：http://baike.sjlbkw.cn/Article/details/ggoztclvq.sHtML

local a = 1
来源：http://mobile.yfazqb.com/Article/details/gqvmhfdfu.sHtML

[T33] Lua：表（数组）
来源：http://3g.epnwcf.com/Article/details/glifwvggs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.yfazqb.com/Article/details/gslrjiwbd.sHtML

[T34] Lua：遍历表
来源：http://mobile.sjlbkw.cn/Article/details/ghkwndgqv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.yfazqb.com/Article/details/gxvamhody.sHtML

[T35] Lua：字典表
来源：http://www.share.epnwcf.com/Article/details/gpciqhosl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.epnwcf.com/Article/details/globpmefx.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/gpxrimnjo.sHtML

function add(a, b) return a + b end
来源：http://www.blog.epnwcf.com/Article/details/gwnllnjrb.sHtML

[T37] Lua：字符串拼接
来源：http://wap.epnwcf.com/Article/details/glioukurc.sHtML

"a" .. "b"
来源：http://www.share.bbcook.cn/Article/details/ggjseqesh.sHtML

[T38] Lua：条件
来源：http://read.share.vehdjk.com/Article/details/geidddxob.sHtML

if x > 0 then print("正") end
来源：http://www.blog.epnwcf.com/Article/details/golyppzys.sHtML

[T39] Lua：模式匹配
来源：http://baike.epnwcf.com/Article/details/gzozgprwc.sHtML

string.find(s, "%d+")
来源：http://www.blog.bbcook.cn/Article/details/gtiytddub.sHtML

[T40] Lua：元表
来源：http://mobile.tarul.cn/Article/details/gnjyoiwyo.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fktsv.cn/Article/details/gkhfqveui.sHtML

[T41] Perl：Hello World
来源：http://mobile.vehdjk.com/Article/details/ghduhrnnw.sHtML

print "Hello\n";
来源：http://baike.sjlbkw.cn/Article/details/gpgbositf.sHtML

[T42] Perl：变量类型
来源：http://blog.vehdjk.com/Article/details/gtyibfymd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.sjlbkw.cn/Article/details/guxrkzgja.sHtML

[T43] Perl：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gsdiivrda.sHtML

"值: $a"
来源：http://blog.sjlbkw.cn/Article/details/ggrpjabmn.sHtML

[T44] Perl：条件
来源：http://baike.tarul.cn/Article/details/gchrrruqt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.bbcook.cn/Article/details/gjxlzqjte.sHtML

[T45] Perl：数组遍历
来源：http://read.share.yfazqb.com/Article/details/goxpybyqe.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.bbcook.cn/Article/details/gtdvgdzfg.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gathoiczc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/gxsegskki.sHtML

[T47] Perl：正则捕获
来源：http://blog.bbcook.cn/Article/details/gbbgmogxo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.bbcook.cn/Article/details/glnfrqkye.sHtML

[T48] Perl：正则替换
来源：http://www.blog.bbcook.cn/Article/details/gncrphomr.sHtML

$s =~ s/old/new/g;
来源：http://m.share.vehdjk.com/Article/details/geyaxoiga.sHtML

[T49] Perl：函数
来源：http://www.m.share.bbcook.cn/Article/details/gvqerxung.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/guonefwci.sHtML

[T50] Perl：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gqeuqqumn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.bbcook.cn/Article/details/gjgoivzzu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.tarul.cn/Article/details/geibxntxn.sHtML

[T51] Scala：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/ggafagsqv.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gxrnzhukj.sHtML

[T52] Scala：变量
来源：http://m.share.sjlbkw.cn/Article/details/gsmqupkqy.sHtML

val a = 1;  var b = 2
来源：http://www.share.bbcook.cn/Article/details/ghporjosl.sHtML

[T53] Scala：字符串插值
来源：http://read.share.tarul.cn/Article/details/gwcqprqut.sHtML

s"值: $b"
来源：http://wap.tarul.cn/Article/details/gktrjqyhl.sHtML

[T54] Scala：集合映射
来源：http://mobile.tarul.cn/Article/details/goneoknlj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fktsv.cn/Article/details/gfvfmntqt.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/ghpswrjbf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.yfazqb.com/Article/details/gtjbddppl.sHtML

[T56] Scala：样例类
来源：http://baike.sjlbkw.cn/Article/details/gyrbhkiwm.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fktsv.cn/Article/details/gqbaurqav.sHtML

[T57] Scala：模式匹配
来源：http://wap.yfazqb.com/Article/details/gajoceqtj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.yfazqb.com/Article/details/goivnpatw.sHtML

[T58] Scala：函数定义
来源：http://read.share.vehdjk.com/Article/details/gwcpqdrin.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.tarul.cn/Article/details/gmahgynnx.sHtML

[T59] Scala：循环
来源：http://read.share.epnwcf.com/Article/details/gmhzqvnoj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gspghiwkh.sHtML

[T60] Scala：折叠
来源：http://wap.tarul.cn/Article/details/glgcrsmld.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.epnwcf.com/Article/details/gaazhusbl.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gldissbbk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.yfazqb.com/Article/details/giurplyua.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gusysngpe.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.yfazqb.com/Article/details/gdpipxzgv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.epnwcf.com/Article/details/gumgwfuat.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.tarul.cn/Article/details/gahqxdakg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.vehdjk.com/Article/details/gvdejctwf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.epnwcf.com/Article/details/gjdyskhps.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.yfazqb.com/Article/details/gdfsbamrj.sHtML

[U04] Py：变量调试打印
来源：http://m.share.vehdjk.com/Article/details/gblijscje.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.epnwcf.com/Article/details/gvrlgtvov.sHtML

[U05] Py：列表去重且保序
来源：http://wap.sjlbkw.cn/Article/details/gfkoolbgt.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/gxpgozuys.sHtML

[U06] Py：合并两个字典
来源：http://mobile.yfazqb.com/Article/details/gyifqgedk.sHtML

{**a, **b}
来源：http://m.share.bbcook.cn/Article/details/gdsnvdyrz.sHtML

[U07] Py：反转字典键值
来源：http://3g.epnwcf.com/Article/details/gssdaipna.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.tarul.cn/Article/details/gsmwblzrq.sHtML

[U08] Py：展平二维列表
来源：http://www.share.sjlbkw.cn/Article/details/gtzcnwubd.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fktsv.cn/Article/details/gsivjcofb.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.epnwcf.com/Article/details/gxoqcyrvp.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/gkcshtcbx.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.epnwcf.com/Article/details/gbepginfn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.bbcook.cn/Article/details/gwzqdxpgn.sHtML

[U11] Py：生成器表达式
来源：http://wap.bbcook.cn/Article/details/gyccknrdy.sHtML

(x * 2 for x in arr)
来源：http://blog.epnwcf.com/Article/details/gvvgcfqbm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.vehdjk.com/Article/details/gnyczaxpb.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fktsv.cn/Article/details/gsubrrnfp.sHtML

[U13] Py：固定长度队列
来源：http://baike.fktsv.cn/Article/details/gymuxvodv.sHtML

deque(maxlen=10)
来源：http://blog.bbcook.cn/Article/details/gnxhkfsoa.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fktsv.cn/Article/details/gprrtmphg.sHtML

defaultdict(list)
来源：http://read.share.fktsv.cn/Article/details/gwjmkqhnb.sHtML

[U15] Py：高精度计时
来源：http://baike.yfazqb.com/Article/details/gzmwnqjhs.sHtML

t = time.perf_counter()
来源：http://mobile.epnwcf.com/Article/details/gnnhcpafa.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.tarul.cn/Article/details/guvtdgfnh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fktsv.cn/Article/details/gsuxnasyi.sHtML


<!-- 参考信息 -->