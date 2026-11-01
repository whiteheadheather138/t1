代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://mobile.epnwcf.com/Article/details/gwktejniz.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/gwmyuxpjo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gvtkujlnw.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/ghoubmjjr.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/gudqurbia.sHtML

[R78] 交互式菜单
来源：http://3g.tarul.cn/Article/details/gmaujgquw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.yfazqb.com/Article/details/gbappgrsk.sHtML

[R79] 解析命令行选项
来源：http://read.share.bbcook.cn/Article/details/gljzdfuok.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gmfmjxuzf.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.vehdjk.com/Article/details/gwjmlwpxt.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/gctjptehr.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gbkjvfmnj.sHtML

S. C / C++ 专题
来源：http://mobile.vehdjk.com/Article/details/gymvfhxhh.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtepsphxp.sHtML

[S01] C：Hello World
来源：http://read.share.bbcook.cn/Article/details/gkucqdhal.sHtML

#include <stdio.h>
来源：http://3g.epnwcf.com/Article/details/geypldfim.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.yfazqb.com/Article/details/gxeetidyg.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.tarul.cn/Article/details/gqkxwklnb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fktsv.cn/Article/details/gqtzujkec.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gswdxlhiw.sHtML

int x; scanf("%d", &x);
来源：http://baike.epnwcf.com/Article/details/gjlmvwyxo.sHtML

[S04] C：字符串复制
来源：http://mobile.epnwcf.com/Article/details/ggenvlvro.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.vehdjk.com/Article/details/gfwnyekyl.sHtML

[S05] C：字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gkhslgatd.sHtML

strlen(s)
来源：http://m.share.sjlbkw.cn/Article/details/gpqwvllef.sHtML

[S06] C：字符串比较
来源：http://mobile.bbcook.cn/Article/details/gpxsfizpr.sHtML

strcmp(a, b) == 0
来源：http://mobile.bbcook.cn/Article/details/gskbsbxqb.sHtML

[S07] C：数组遍历求和
来源：http://mobile.yfazqb.com/Article/details/grnzxvfde.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/grhmyklcv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.bbcook.cn/Article/details/gstqofree.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/gcdzkwfba.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/gjcqlelta.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.yfazqb.com/Article/details/gkezszhfa.sHtML

[S10] C：指针与解引用
来源：http://www.blog.tarul.cn/Article/details/gzybqqyns.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fktsv.cn/Article/details/gxvfwvdel.sHtML

[S11] C：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/ggartjfxo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.bbcook.cn/Article/details/gnvtdruex.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.vehdjk.com/Article/details/grsuneelb.sHtML

fclose(f);
来源：http://3g.yfazqb.com/Article/details/gjmfuxebq.sHtML

[S12] C：写文件
来源：http://mobile.bbcook.cn/Article/details/gqrzrjeux.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gjsbaddlx.sHtML

[S13] C：宏定义
来源：http://wap.bbcook.cn/Article/details/gntizpeex.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.tarul.cn/Article/details/gywnirdej.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/gzmbshefz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.tarul.cn/Article/details/gijwgwkyw.sHtML

[S15] C：类型转换
来源：http://www.share.vehdjk.com/Article/details/gosaqyutp.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/gismqgayc.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gixxelebw.sHtML

x |= (1 << 3);
来源：http://m.share.tarul.cn/Article/details/gyojzkcfy.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbhgcrdc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.yfazqb.com/Article/details/gironubno.sHtML

[S18] C：命令行参数
来源：http://mobile.bbcook.cn/Article/details/gwsakqnyp.sHtML

int main(int argc, char **argv)
来源：http://3g.fktsv.cn/Article/details/gjfvvdlzc.sHtML

[S19] C：快速排序
来源：http://www.m.share.bbcook.cn/Article/details/gpovtnbbu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/glfachzxm.sHtML

[S20] C：二分查找
来源：http://m.share.sjlbkw.cn/Article/details/gxadaftda.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gspqcppee.sHtML

[S21] C：字符类别判断
来源：http://www.blog.yfazqb.com/Article/details/gpwjuikzk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.epnwcf.com/Article/details/glhundcmg.sHtML

[S22] C：字符串转数字
来源：http://blog.tarul.cn/Article/details/gtenjyisp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.vehdjk.com/Article/details/gfuehyzpg.sHtML

[S23] C：随机数
来源：http://baike.vehdjk.com/Article/details/gqkhjfpbs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fktsv.cn/Article/details/gzcoazgzv.sHtML

[S24] C：获取本地时间
来源：http://www.share.epnwcf.com/Article/details/gezexfilq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/gdvuvheza.sHtML

[S25] C：内存拷贝
来源：http://mobile.vehdjk.com/Article/details/gfbraohaf.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/gkphvfhby.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/gpqrvbqjq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.sjlbkw.cn/Article/details/gmlkgondk.sHtML

[S27] C：定义常量
来源：http://baike.tarul.cn/Article/details/gnfuxqnnx.sHtML

const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gyyoarkil.sHtML

[S28] C：静态变量
来源：http://baike.tarul.cn/Article/details/gnyddnbmv.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/gimdcjvol.sHtML

[S29] C：变参函数
来源：http://baike.vehdjk.com/Article/details/gmcesceay.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.tarul.cn/Article/details/gggynrwny.sHtML

[S30] C：头文件保护
来源：http://www.blog.yfazqb.com/Article/details/gislvzdjq.sHtML

#ifndef X_H
来源：http://baike.bbcook.cn/Article/details/gauslztuf.sHtML

#define X_H
来源：http://www.share.vehdjk.com/Article/details/ghkdvqsty.sHtML

#endif
来源：http://mobile.bbcook.cn/Article/details/gqyiduxha.sHtML

[S31] C++：Hello World
来源：http://3g.tarul.cn/Article/details/goyppmdhy.sHtML

#include <iostream>
来源：http://wap.epnwcf.com/Article/details/gdcncqxrd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.sjlbkw.cn/Article/details/govlhudpt.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/graqcbzqb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.yfazqb.com/Article/details/gtmbtffqg.sHtML

[S33] C++：vector 增删
来源：http://read.share.fktsv.cn/Article/details/gddyzbinz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.yfazqb.com/Article/details/gcdtizoic.sHtML

[S34] C++：遍历 vector
来源：http://www.share.sjlbkw.cn/Article/details/gicgsfbdu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.yfazqb.com/Article/details/ggyxaeklb.sHtML

[S35] C++：map
来源：http://m.share.tarul.cn/Article/details/gonkinrwd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gttcydvfi.sHtML

[S36] C++：unordered_map
来源：http://3g.epnwcf.com/Article/details/grcypuvnq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/giafccjif.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/gkpeyisjs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gsguhntgr.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/gqofywmkq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.tarul.cn/Article/details/grdtrxlez.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.epnwcf.com/Article/details/gpnawiwjv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.vehdjk.com/Article/details/gkimsoukq.sHtML

[S40] C++：查找元素
来源：http://www.blog.yfazqb.com/Article/details/geteocvdn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fktsv.cn/Article/details/gqutkylhv.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gnosmoqsj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fktsv.cn/Article/details/gqkmfwmtx.sHtML

[S42] C++：继承与虚函数
来源：http://3g.vehdjk.com/Article/details/ghunltnil.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.vehdjk.com/Article/details/gmilopgth.sHtML

[S43] C++：智能指针
来源：http://www.blog.epnwcf.com/Article/details/gicqzvmxm.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.vehdjk.com/Article/details/gpmiokyuw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.vehdjk.com/Article/details/gelrtnckz.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fktsv.cn/Article/details/goeekhook.sHtML

[S45] C++：lambda
来源：http://www.m.share.fktsv.cn/Article/details/gxcwbhxgk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.tarul.cn/Article/details/gdmnkggxq.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/gijppnwsj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.tarul.cn/Article/details/gndstgsgb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.sjlbkw.cn/Article/details/grdqlmrwj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.sjlbkw.cn/Article/details/gknlmhaxh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gmjhfyfon.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.tarul.cn/Article/details/gfpkprjhl.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fktsv.cn/Article/details/ggmejjoav.sHtML

[S49] C++：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/grugwiove.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.bbcook.cn/Article/details/goubmjnzf.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/ggmlsechs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gogekejoo.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/gzlsureby.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fktsv.cn/Article/details/gqxcsxqfr.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.epnwcf.com/Article/details/gpycgkokn.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fktsv.cn/Article/details/gruzyvqxi.sHtML

[S53] C++：移动语义
来源：http://mobile.sjlbkw.cn/Article/details/ghmdaxncf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.sjlbkw.cn/Article/details/grrpeqbet.sHtML

[S54] C++：异常处理
来源：http://www.blog.vehdjk.com/Article/details/gsukuecqm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.yfazqb.com/Article/details/gwkoqbhok.sHtML

[S55] C++：结构化绑定
来源：http://3g.fktsv.cn/Article/details/gtvhekkto.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.epnwcf.com/Article/details/gofkcpmbg.sHtML

[S56] C++：optional
来源：http://www.share.yfazqb.com/Article/details/guupyfntb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.bbcook.cn/Article/details/gvkcibevz.sHtML

[S57] C++：编译期常量
来源：http://m.share.tarul.cn/Article/details/gvxqlidbd.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gmxhwlnqc.sHtML

[S58] C++：命名空间
来源：http://www.share.fktsv.cn/Article/details/gfqqexfhy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.yfazqb.com/Article/details/gpvyhktcq.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/gxqtakblf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.yfazqb.com/Article/details/ghsdzrxpo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.bbcook.cn/Article/details/gkdhlgqyt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gbmdhvonu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqqocrakr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.sjlbkw.cn/Article/details/gnqeqamen.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grkqtmoch.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.epnwcf.com/Article/details/gtcnezykz.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gvyhutebe.sHtML

[T02] Kotlin：变量
来源：http://3g.epnwcf.com/Article/details/gffbgsiak.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/gpjoawcrd.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/gegvrbbuj.sHtML

"值: $b"
来源：http://blog.epnwcf.com/Article/details/gihcucldg.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/gekoaahsl.sHtML

val n: String? = null;  n?.length
来源：http://www.share.yfazqb.com/Article/details/gpvigmbhu.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.yfazqb.com/Article/details/gfgsebnsk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.sjlbkw.cn/Article/details/ghjafuyqy.sHtML

[T06] Kotlin：集合映射
来源：http://blog.epnwcf.com/Article/details/gxhfknyll.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/guwfhsobj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.yfazqb.com/Article/details/grwmhjdni.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fktsv.cn/Article/details/ggmogrbti.sHtML

[T08] Kotlin：数据类
来源：http://read.share.yfazqb.com/Article/details/grjonapwk.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.epnwcf.com/Article/details/gcjwxplnk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fktsv.cn/Article/details/gmwaownvt.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.yfazqb.com/Article/details/geudabnsf.sHtML

[T10] Kotlin：默认参数
来源：http://baike.bbcook.cn/Article/details/gnzdmfiha.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.epnwcf.com/Article/details/gevxsfocf.sHtML

[T11] Kotlin：协程
来源：http://read.share.bbcook.cn/Article/details/gamzybabs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.epnwcf.com/Article/details/gbwrqgayg.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.vehdjk.com/Article/details/giegofprs.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gfsoqgwtu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.vehdjk.com/Article/details/gbwntjuwg.sHtML

val m = mapOf("a" to 1)
来源：http://baike.epnwcf.com/Article/details/gyilmozcr.sHtML

[T14] Kotlin：循环
来源：http://www.share.fktsv.cn/Article/details/gsmraqrqj.sHtML

for (i in 1..10) println(i)
来源：http://baike.fktsv.cn/Article/details/giiyrqoym.sHtML

[T15] Kotlin：接口
来源：http://baike.vehdjk.com/Article/details/gtdbuwyrh.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/gbuhvvxbr.sHtML

[T16] Swift：Hello World
来源：http://read.share.bbcook.cn/Article/details/gpceiyxtm.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gfnjldhnk.sHtML

[T17] Swift：变量与常量
来源：http://m.share.sjlbkw.cn/Article/details/guupadsvn.sHtML

var a = 1;  let b = 2
来源：http://wap.fktsv.cn/Article/details/gdetzjlfp.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/ggrnjrabl.sHtML

"值: \(b)"
来源：http://wap.bbcook.cn/Article/details/ggcsyjkch.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.yfazqb.com/Article/details/gfwypwysl.sHtML

if let n = opt { print(n) }
来源：http://www.share.yfazqb.com/Article/details/ggspghmyp.sHtML

[T20] Swift：数组操作
来源：http://3g.epnwcf.com/Article/details/gbvbcnfxa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.bbcook.cn/Article/details/gfqhxgfep.sHtML

[T21] Swift：遍历
来源：http://www.share.yfazqb.com/Article/details/gkewlhxau.sHtML

for x in a { print(x) }
来源：http://mobile.bbcook.cn/Article/details/gyhmjyell.sHtML

[T22] Swift：字典
来源：http://blog.yfazqb.com/Article/details/gfjdmdecw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.bbcook.cn/Article/details/gsifqjwvo.sHtML

[T23] Swift：函数
来源：http://read.share.sjlbkw.cn/Article/details/gpszgcrum.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gbecfkczj.sHtML

[T24] Swift：闭包
来源：http://read.share.bbcook.cn/Article/details/gpiyhdtde.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.yfazqb.com/Article/details/gulfwvnpo.sHtML

[T25] Swift：结构体
来源：http://m.share.epnwcf.com/Article/details/gxckablzr.sHtML

struct P { var x: Int }
来源：http://www.blog.epnwcf.com/Article/details/gpfuxblpm.sHtML

[T26] Swift：类与重写
来源：http://mobile.fktsv.cn/Article/details/gxdoxlkml.sHtML

class A: Base { override func f() {} }
来源：http://read.share.epnwcf.com/Article/details/gelitwigp.sHtML

[T27] Swift：错误处理
来源：http://blog.tarul.cn/Article/details/gosuksfyt.sHtML

do { try f() } catch { print(error) }
来源：http://wap.bbcook.cn/Article/details/gqbiliyxk.sHtML

[T28] Swift：枚举
来源：http://3g.yfazqb.com/Article/details/glqnzusyw.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/ggfiwdnjc.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.vehdjk.com/Article/details/gbajtypyw.sHtML

guard let x = opt else { return }
来源：http://wap.epnwcf.com/Article/details/gappiebmv.sHtML

[T30] Swift：协议
来源：http://mobile.sjlbkw.cn/Article/details/gmtofzvef.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.yfazqb.com/Article/details/gqnjhjkpk.sHtML

[T31] Lua：Hello World
来源：http://3g.epnwcf.com/Article/details/giupdewqq.sHtML

print("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gcdtjawuw.sHtML

[T32] Lua：局部变量
来源：http://baike.yfazqb.com/Article/details/guwjzxpsb.sHtML

local a = 1
来源：http://m.share.fktsv.cn/Article/details/gqvwjncrf.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.bbcook.cn/Article/details/gfjamefrd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fktsv.cn/Article/details/gkexysxeo.sHtML

[T34] Lua：遍历表
来源：http://read.share.yfazqb.com/Article/details/govicjgsu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.epnwcf.com/Article/details/glqoocyue.sHtML

[T35] Lua：字典表
来源：http://www.share.tarul.cn/Article/details/gtsvgzggp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.tarul.cn/Article/details/gzolhzucw.sHtML

[T36] Lua：函数
来源：http://m.share.epnwcf.com/Article/details/gukmkkeuk.sHtML

function add(a, b) return a + b end
来源：http://3g.bbcook.cn/Article/details/gkucoopvw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/grecrrpqc.sHtML

"a" .. "b"
来源：http://blog.tarul.cn/Article/details/gnwcydlhi.sHtML

[T38] Lua：条件
来源：http://wap.tarul.cn/Article/details/grhrsyrth.sHtML

if x > 0 then print("正") end
来源：http://www.share.vehdjk.com/Article/details/gtiouuayi.sHtML

[T39] Lua：模式匹配
来源：http://www.share.tarul.cn/Article/details/gajafnnwu.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fktsv.cn/Article/details/gxmhxmmwr.sHtML

[T40] Lua：元表
来源：http://www.blog.fktsv.cn/Article/details/gkvibxbpg.sHtML

setmetatable({}, { __index = base })
来源：http://blog.vehdjk.com/Article/details/gvpchtrsj.sHtML

[T41] Perl：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gxqfyevbh.sHtML

print "Hello\n";
来源：http://baike.bbcook.cn/Article/details/gwmifdmhf.sHtML

[T42] Perl：变量类型
来源：http://read.share.epnwcf.com/Article/details/gzvalxelq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.yfazqb.com/Article/details/gusfifgec.sHtML

[T43] Perl：字符串插值
来源：http://mobile.tarul.cn/Article/details/gqtmagljt.sHtML

"值: $a"
来源：http://wap.epnwcf.com/Article/details/gwcrrtxow.sHtML

[T44] Perl：条件
来源：http://wap.epnwcf.com/Article/details/gzaflzqnk.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fktsv.cn/Article/details/gdqkdpysb.sHtML

[T45] Perl：数组遍历
来源：http://m.share.vehdjk.com/Article/details/gkmohglpv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.bbcook.cn/Article/details/gdlqizeyx.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.tarul.cn/Article/details/geevzcibm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.yfazqb.com/Article/details/gbibisowy.sHtML

[T47] Perl：正则捕获
来源：http://www.share.bbcook.cn/Article/details/glmtcrawy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.yfazqb.com/Article/details/grvypvtzr.sHtML

[T48] Perl：正则替换
来源：http://wap.tarul.cn/Article/details/gyxacrfwo.sHtML

$s =~ s/old/new/g;
来源：http://read.share.tarul.cn/Article/details/geybasqrd.sHtML

[T49] Perl：函数
来源：http://www.m.share.vehdjk.com/Article/details/ggdyvlhuf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gicgqksnk.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gxcvfuhrh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.vehdjk.com/Article/details/gddojlpsq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.bbcook.cn/Article/details/grpolopzx.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/gllpgghxn.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gobjjftfz.sHtML

[T52] Scala：变量
来源：http://baike.epnwcf.com/Article/details/gczljaeum.sHtML

val a = 1;  var b = 2
来源：http://3g.vehdjk.com/Article/details/gosdrefaq.sHtML

[T53] Scala：字符串插值
来源：http://wap.epnwcf.com/Article/details/grgdnntwp.sHtML

s"值: $b"
来源：http://m.share.bbcook.cn/Article/details/geuonfvuj.sHtML

[T54] Scala：集合映射
来源：http://3g.tarul.cn/Article/details/gyztagklp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.epnwcf.com/Article/details/gwnbrnedn.sHtML

[T55] Scala：集合过滤
来源：http://wap.tarul.cn/Article/details/gekqeavyc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.vehdjk.com/Article/details/gdmelkrjl.sHtML

[T56] Scala：样例类
来源：http://m.share.bbcook.cn/Article/details/gvutiilvw.sHtML

case class User(name: String, age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gnxjhiqbg.sHtML

[T57] Scala：模式匹配
来源：http://3g.yfazqb.com/Article/details/ghodjrplt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.tarul.cn/Article/details/gcvjjioma.sHtML

[T58] Scala：函数定义
来源：http://mobile.fktsv.cn/Article/details/gxgxdclen.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.bbcook.cn/Article/details/guwjeojfs.sHtML

[T59] Scala：循环
来源：http://3g.epnwcf.com/Article/details/gzksbpgzw.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.tarul.cn/Article/details/gdunbxhux.sHtML

[T60] Scala：折叠
来源：http://www.blog.bbcook.cn/Article/details/geiwzwqui.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.vehdjk.com/Article/details/gvggwxsat.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gyznpkwoz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.yfazqb.com/Article/details/gmdidbrvk.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gcmeerwgy.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.tarul.cn/Article/details/gbttsdiso.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.vehdjk.com/Article/details/gndnafvav.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.vehdjk.com/Article/details/ggfqarywz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.yfazqb.com/Article/details/gsjmnhccf.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.vehdjk.com/Article/details/gwywsgeir.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.epnwcf.com/Article/details/gqxxdbndr.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.yfazqb.com/Article/details/gizhwnrzy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.vehdjk.com/Article/details/gtfjqcnwg.sHtML

[U05] Py：列表去重且保序
来源：http://wap.tarul.cn/Article/details/gijxaqtgk.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/guxzkndiw.sHtML

[U06] Py：合并两个字典
来源：http://mobile.vehdjk.com/Article/details/grqqburjq.sHtML

{**a, **b}
来源：http://baike.epnwcf.com/Article/details/gwngqptfe.sHtML

[U07] Py：反转字典键值
来源：http://wap.sjlbkw.cn/Article/details/gnjikssrv.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.epnwcf.com/Article/details/gyjildrcr.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fktsv.cn/Article/details/guzzkhjzc.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/gdptqygam.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fktsv.cn/Article/details/gigbornon.sHtML

max(d, key=d.get)
来源：http://www.m.share.bbcook.cn/Article/details/gkznfnqgb.sHtML

[U10] Py：按值排序字典
来源：http://blog.vehdjk.com/Article/details/glryyvoym.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.vehdjk.com/Article/details/gvohpstgi.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fktsv.cn/Article/details/gjqztpnjq.sHtML

(x * 2 for x in arr)
来源：http://3g.epnwcf.com/Article/details/glkmnbgxm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/gdsvdlgiq.sHtML

Counter(arr).most_common(3)
来源：http://baike.bbcook.cn/Article/details/gwazijarm.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.vehdjk.com/Article/details/gsgfmajkh.sHtML

deque(maxlen=10)
来源：http://3g.fktsv.cn/Article/details/gzyxkoyev.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/gsfiiglhu.sHtML

defaultdict(list)
来源：http://baike.sjlbkw.cn/Article/details/gvpzjsxrx.sHtML

[U15] Py：高精度计时
来源：http://mobile.sjlbkw.cn/Article/details/gcjtsbgui.sHtML

t = time.perf_counter()
来源：http://www.blog.tarul.cn/Article/details/gvyljblrp.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.yfazqb.com/Article/details/gaodtofou.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fktsv.cn/Article/details/gcypfgrye.sHtML


<!-- 参考信息 -->