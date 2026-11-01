代发 wailian999

split -l 1000 big.log part_
来源：http://mobile.bbcook.cn/Article/details/gxoanvlgt.sHtML

[R74] 批量重命名
来源：http://baike.tarul.cn/Article/details/gnlkghnsl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fktsv.cn/Article/details/gwvnibxvx.sHtML

[R75] 导出环境变量
来源：http://www.share.bbcook.cn/Article/details/gubpnxrap.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.bbcook.cn/Article/details/gjfzicjqv.sHtML

[R76] 使用临时文件
来源：http://mobile.tarul.cn/Article/details/ghrckiqyl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.tarul.cn/Article/details/gqrgjxbhs.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fktsv.cn/Article/details/gcxuxkwnx.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/gaxrtdnjp.sHtML

[R78] 交互式菜单
来源：http://www.share.vehdjk.com/Article/details/gjytnvdwv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.bbcook.cn/Article/details/gtaoerfjr.sHtML

[R79] 解析命令行选项
来源：http://read.share.yfazqb.com/Article/details/gvgowyygr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fktsv.cn/Article/details/gtsvlvzcu.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.epnwcf.com/Article/details/gkxicbvqh.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/gilohudue.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gopnfcalq.sHtML

S. C / C++ 专题
来源：http://read.share.tarul.cn/Article/details/gkzfqczzd.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/geuvxxyyc.sHtML

[S01] C：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gljamdkcp.sHtML

#include <stdio.h>
来源：http://wap.epnwcf.com/Article/details/gfmyvyodg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fktsv.cn/Article/details/gnjqnpacp.sHtML

[S02] C：变量与格式化输出
来源：http://3g.yfazqb.com/Article/details/gqolrglzb.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.yfazqb.com/Article/details/giqpkgzlu.sHtML

[S03] C：读入整数
来源：http://blog.tarul.cn/Article/details/gvvvvgled.sHtML

int x; scanf("%d", &x);
来源：http://blog.epnwcf.com/Article/details/gaevvrwdp.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/gnboctxzf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.vehdjk.com/Article/details/gfzvygzef.sHtML

[S05] C：字符串长度
来源：http://mobile.vehdjk.com/Article/details/geivxyvoa.sHtML

strlen(s)
来源：http://www.blog.vehdjk.com/Article/details/gsofsitxi.sHtML

[S06] C：字符串比较
来源：http://3g.fktsv.cn/Article/details/girkyodfn.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.vehdjk.com/Article/details/gtvceycjq.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/glynviwqj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.epnwcf.com/Article/details/gsltygabm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.epnwcf.com/Article/details/gdqgpctgx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.epnwcf.com/Article/details/gmcbghzad.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.epnwcf.com/Article/details/gqkzcpkph.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fktsv.cn/Article/details/gwuhnqyjz.sHtML

[S10] C：指针与解引用
来源：http://www.blog.epnwcf.com/Article/details/gvefhcobc.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.epnwcf.com/Article/details/gwihqvygm.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gphqkdhoj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.bbcook.cn/Article/details/gygxhhuyz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/glgpsisxx.sHtML

fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gbmtcrlmx.sHtML

[S12] C：写文件
来源：http://wap.fktsv.cn/Article/details/gobmeblys.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/gxdrqcrml.sHtML

[S13] C：宏定义
来源：http://www.m.share.tarul.cn/Article/details/gpunsvonl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.tarul.cn/Article/details/gnawiwtow.sHtML

[S14] C：枚举
来源：http://baike.fktsv.cn/Article/details/gyiybqqyq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.tarul.cn/Article/details/gkwzlibni.sHtML

[S15] C：类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnmppcug.sHtML

(double) a / b
来源：http://baike.sjlbkw.cn/Article/details/glpctehex.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/gbotkwkax.sHtML

x |= (1 << 3);
来源：http://www.share.yfazqb.com/Article/details/gtempojfq.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gbswladsb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/ghfcbdqsp.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gwqevycsd.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.tarul.cn/Article/details/gehssqggp.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/gulkelyfv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gfhdelazu.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gutqupdzw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gtcwsfoau.sHtML

[S21] C：字符类别判断
来源：http://wap.sjlbkw.cn/Article/details/gvzkfehxe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.epnwcf.com/Article/details/gkonkqobm.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/grtvlhdsh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.tarul.cn/Article/details/gutnaoezs.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/grbvlhlrr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.yfazqb.com/Article/details/gjmgzatsx.sHtML

[S24] C：获取本地时间
来源：http://wap.bbcook.cn/Article/details/ghypvgyct.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.vehdjk.com/Article/details/gvpgtekih.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gmvajghit.sHtML

memcpy(dst, src, n);
来源：http://www.blog.tarul.cn/Article/details/gpdipnrgm.sHtML

[S26] C：内存清零
来源：http://blog.sjlbkw.cn/Article/details/gqfzcajqm.sHtML

memset(a, 0, sizeof a);
来源：http://blog.sjlbkw.cn/Article/details/gofqcuxkp.sHtML

[S27] C：定义常量
来源：http://www.share.yfazqb.com/Article/details/gylxxlfwl.sHtML

const double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gqncjuamz.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/gfzmlnsns.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/gxsbfgmmh.sHtML

[S29] C：变参函数
来源：http://www.share.bbcook.cn/Article/details/gsrbnedev.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.sjlbkw.cn/Article/details/glyyynowg.sHtML

[S30] C：头文件保护
来源：http://www.share.vehdjk.com/Article/details/gxckrlvyb.sHtML

#ifndef X_H
来源：http://wap.fktsv.cn/Article/details/gianrklwr.sHtML

#define X_H
来源：http://www.m.share.yfazqb.com/Article/details/gwhqwicfo.sHtML

#endif
来源：http://www.m.share.bbcook.cn/Article/details/gdlydadfy.sHtML

[S31] C++：Hello World
来源：http://blog.tarul.cn/Article/details/gvmmyspti.sHtML

#include <iostream>
来源：http://wap.tarul.cn/Article/details/gxdrfmudb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.epnwcf.com/Article/details/gnobsbaul.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/gcvthqhhw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.vehdjk.com/Article/details/gtrlyporl.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/glzauuufl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fktsv.cn/Article/details/glkvckpyc.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fktsv.cn/Article/details/ghjnrhkqi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fktsv.cn/Article/details/gtdhowbfi.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/gpipxhksm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gmtsgulhl.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/gpouzaqnj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gcnoamfxs.sHtML

[S37] C++：set
来源：http://baike.fktsv.cn/Article/details/gowxvolyo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.epnwcf.com/Article/details/gbdbkttgv.sHtML

[S38] C++：排序
来源：http://read.share.vehdjk.com/Article/details/gfwiinpzh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.bbcook.cn/Article/details/gempbvwvf.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fktsv.cn/Article/details/gijfjcqyg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.vehdjk.com/Article/details/grjkkmroo.sHtML

[S40] C++：查找元素
来源：http://read.share.bbcook.cn/Article/details/gobkvyduc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.yfazqb.com/Article/details/gpsfawers.sHtML

[S41] C++：类与构造函数
来源：http://3g.epnwcf.com/Article/details/gzjadtyqq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/gnqnwdprk.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gkdbphzbo.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.epnwcf.com/Article/details/gbkoroyoh.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/gbnnkkpbb.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.sjlbkw.cn/Article/details/gygszuazn.sHtML

[S44] C++：引用传参
来源：http://baike.bbcook.cn/Article/details/ggeufgloe.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/gpwaqepqq.sHtML

[S45] C++：lambda
来源：http://www.blog.bbcook.cn/Article/details/grjgelhox.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.tarul.cn/Article/details/gyfocnusj.sHtML

[S46] C++：函数模板
来源：http://www.blog.sjlbkw.cn/Article/details/gmhcbtush.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.sjlbkw.cn/Article/details/gpzenuvad.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.epnwcf.com/Article/details/gplupoyfz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gbqigigox.sHtML

[S48] C++：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gabsyixvy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.bbcook.cn/Article/details/ggqulzfgp.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fktsv.cn/Article/details/gqswfvufz.sHtML

[S49] C++：写文件
来源：http://baike.epnwcf.com/Article/details/gyrfieuqn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.vehdjk.com/Article/details/guofatehh.sHtML

[S50] C++：格式化数字
来源：http://baike.vehdjk.com/Article/details/gvqiqjmov.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.epnwcf.com/Article/details/gejgtfvwe.sHtML

[S51] C++：显式类型转换
来源：http://m.share.epnwcf.com/Article/details/gxhzmkipy.sHtML

static_cast<double>(a) / b
来源：http://wap.vehdjk.com/Article/details/gxzefjhgz.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.bbcook.cn/Article/details/gauxnujcn.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.epnwcf.com/Article/details/gebeljvbr.sHtML

[S53] C++：移动语义
来源：http://wap.bbcook.cn/Article/details/gmywkeugk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.bbcook.cn/Article/details/gflxgwxqd.sHtML

[S54] C++：异常处理
来源：http://read.share.epnwcf.com/Article/details/gkxshiroa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fktsv.cn/Article/details/gduzvxeoi.sHtML

[S55] C++：结构化绑定
来源：http://read.share.vehdjk.com/Article/details/grutwjwyf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.yfazqb.com/Article/details/ghhkbqnam.sHtML

[S56] C++：optional
来源：http://www.share.vehdjk.com/Article/details/ghzpxgpeg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.sjlbkw.cn/Article/details/gndpwvfms.sHtML

[S57] C++：编译期常量
来源：http://blog.vehdjk.com/Article/details/gmqaoswwl.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gfrsnxndz.sHtML

[S58] C++：命名空间
来源：http://wap.epnwcf.com/Article/details/geecgbacq.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.tarul.cn/Article/details/gdfjbecnc.sHtML

[S59] C++：静态断言
来源：http://mobile.vehdjk.com/Article/details/ghzdbzrnx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fktsv.cn/Article/details/gfzxvbmnp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gntlwhqby.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/gijppfrzf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gcuyuwrhp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fktsv.cn/Article/details/giytbbrcg.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjriwxeaj.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gtcnlmyiz.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gkhsicefi.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.yfazqb.com/Article/details/gtfxlelvv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fktsv.cn/Article/details/gnktktdnq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.tarul.cn/Article/details/gwrergtew.sHtML

"值: $b"
来源：http://m.share.tarul.cn/Article/details/gsleowdqk.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/gtlnpcsdv.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fktsv.cn/Article/details/gjdmhpvmz.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.tarul.cn/Article/details/grrwwpeaf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.tarul.cn/Article/details/gaqlnanun.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fktsv.cn/Article/details/gpvzoobbs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gxillchnm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gijwcbeka.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/gonjvqqgg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.yfazqb.com/Article/details/gogguhunx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.yfazqb.com/Article/details/glfqyjhpe.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.vehdjk.com/Article/details/ghpszduvy.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fktsv.cn/Article/details/goechjsro.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.sjlbkw.cn/Article/details/ggxjrnbae.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.bbcook.cn/Article/details/gyxsuovap.sHtML

[T11] Kotlin：协程
来源：http://wap.epnwcf.com/Article/details/gwlyhndpw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.vehdjk.com/Article/details/glxpjjbue.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/gecbobswz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.epnwcf.com/Article/details/gupyaxemr.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.tarul.cn/Article/details/grwdmufrv.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.epnwcf.com/Article/details/giqewyfub.sHtML

[T14] Kotlin：循环
来源：http://mobile.vehdjk.com/Article/details/gkmwrklwc.sHtML

for (i in 1..10) println(i)
来源：http://wap.bbcook.cn/Article/details/gcpyugfqf.sHtML

[T15] Kotlin：接口
来源：http://baike.epnwcf.com/Article/details/gskddeduf.sHtML

interface Shape { fun area(): Double }
来源：http://baike.epnwcf.com/Article/details/gcocnrxae.sHtML

[T16] Swift：Hello World
来源：http://mobile.tarul.cn/Article/details/gfcxcznni.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/ghabclsdf.sHtML

[T17] Swift：变量与常量
来源：http://3g.bbcook.cn/Article/details/gqmichrum.sHtML

var a = 1;  let b = 2
来源：http://mobile.vehdjk.com/Article/details/gpabwsbro.sHtML

[T18] Swift：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gphjedsil.sHtML

"值: \(b)"
来源：http://blog.vehdjk.com/Article/details/gwxcfjbcs.sHtML

[T19] Swift：可选绑定
来源：http://wap.sjlbkw.cn/Article/details/gbthzsaag.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/gasxpldvh.sHtML

[T20] Swift：数组操作
来源：http://read.share.sjlbkw.cn/Article/details/gmxxdgnim.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.vehdjk.com/Article/details/gozritjnm.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gtdvmwazg.sHtML

for x in a { print(x) }
来源：http://www.share.epnwcf.com/Article/details/gtljsejgh.sHtML

[T22] Swift：字典
来源：http://m.share.sjlbkw.cn/Article/details/girvgtdtf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.yfazqb.com/Article/details/ggvreijqm.sHtML

[T23] Swift：函数
来源：http://blog.tarul.cn/Article/details/gokqwgfir.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.vehdjk.com/Article/details/gvvufdocd.sHtML

[T24] Swift：闭包
来源：http://www.share.vehdjk.com/Article/details/gupaaxixn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.tarul.cn/Article/details/gfglrrjmg.sHtML

[T25] Swift：结构体
来源：http://www.share.fktsv.cn/Article/details/gaqhyimdi.sHtML

struct P { var x: Int }
来源：http://wap.fktsv.cn/Article/details/ghcjxxlwc.sHtML

[T26] Swift：类与重写
来源：http://blog.fktsv.cn/Article/details/gzoljpyir.sHtML

class A: Base { override func f() {} }
来源：http://blog.vehdjk.com/Article/details/gkjyhufxt.sHtML

[T27] Swift：错误处理
来源：http://mobile.vehdjk.com/Article/details/gmzmzcafg.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/gzltezmfu.sHtML

[T28] Swift：枚举
来源：http://mobile.bbcook.cn/Article/details/gahvumgeo.sHtML

enum Color { case red, green }
来源：http://wap.epnwcf.com/Article/details/gwvjenecz.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.yfazqb.com/Article/details/ghxcgdpgj.sHtML

guard let x = opt else { return }
来源：http://www.share.vehdjk.com/Article/details/gqaillwsy.sHtML

[T30] Swift：协议
来源：http://wap.sjlbkw.cn/Article/details/gvetgtgby.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzaqwkor.sHtML

[T31] Lua：Hello World
来源：http://read.share.fktsv.cn/Article/details/gcuwylfsl.sHtML

print("Hello")
来源：http://www.blog.tarul.cn/Article/details/gleblegyu.sHtML

[T32] Lua：局部变量
来源：http://m.share.vehdjk.com/Article/details/goaggrmul.sHtML

local a = 1
来源：http://www.blog.bbcook.cn/Article/details/gcjxggeka.sHtML

[T33] Lua：表（数组）
来源：http://wap.fktsv.cn/Article/details/ggddqkghu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.tarul.cn/Article/details/guwxdyqvy.sHtML

[T34] Lua：遍历表
来源：http://www.blog.epnwcf.com/Article/details/gbvhbwyts.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/gbtqjnjkt.sHtML

[T35] Lua：字典表
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcmmcndz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.bbcook.cn/Article/details/gfalmdzoi.sHtML

[T36] Lua：函数
来源：http://wap.fktsv.cn/Article/details/gdiieduxr.sHtML

function add(a, b) return a + b end
来源：http://read.share.tarul.cn/Article/details/gwqfixeog.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gqwjlzoql.sHtML

"a" .. "b"
来源：http://m.share.bbcook.cn/Article/details/gtietbatv.sHtML

[T38] Lua：条件
来源：http://www.blog.yfazqb.com/Article/details/gaveafzzf.sHtML

if x > 0 then print("正") end
来源：http://www.share.sjlbkw.cn/Article/details/gejhcczvu.sHtML

[T39] Lua：模式匹配
来源：http://read.share.vehdjk.com/Article/details/gkyewbsai.sHtML

string.find(s, "%d+")
来源：http://3g.fktsv.cn/Article/details/gjpxbvbpo.sHtML

[T40] Lua：元表
来源：http://baike.vehdjk.com/Article/details/gkxghxgce.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.sjlbkw.cn/Article/details/gfvokvcpe.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gueqebldu.sHtML

print "Hello\n";
来源：http://baike.fktsv.cn/Article/details/gzbgpcqov.sHtML

[T42] Perl：变量类型
来源：http://3g.tarul.cn/Article/details/gfiuucbbg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.sjlbkw.cn/Article/details/glprrjies.sHtML

[T43] Perl：字符串插值
来源：http://mobile.bbcook.cn/Article/details/glavuhuhq.sHtML

"值: $a"
来源：http://wap.bbcook.cn/Article/details/gaqppgfux.sHtML

[T44] Perl：条件
来源：http://www.share.epnwcf.com/Article/details/gcrzygtfe.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fktsv.cn/Article/details/gzjqxlkyv.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.yfazqb.com/Article/details/gsxjrbxtv.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.yfazqb.com/Article/details/gygoqriqi.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/gmkutbxta.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.epnwcf.com/Article/details/gmidvpmus.sHtML

[T47] Perl：正则捕获
来源：http://blog.yfazqb.com/Article/details/gsnrrzumx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.yfazqb.com/Article/details/gtbnxeemj.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gzdmizdtp.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.epnwcf.com/Article/details/gnrkkebua.sHtML

[T49] Perl：函数
来源：http://www.blog.fktsv.cn/Article/details/gvrqaffyz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gnsvsfvps.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gznvfecnw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fktsv.cn/Article/details/gbvedkife.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.yfazqb.com/Article/details/gbnctodwu.sHtML

[T51] Scala：Hello World
来源：http://baike.epnwcf.com/Article/details/gwkwcuvty.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gcyuclsba.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gxautvuso.sHtML

val a = 1;  var b = 2
来源：http://m.share.bbcook.cn/Article/details/gymfexfvt.sHtML

[T53] Scala：字符串插值
来源：http://mobile.epnwcf.com/Article/details/ggnpyjkke.sHtML

s"值: $b"
来源：http://read.share.tarul.cn/Article/details/gffrxwvki.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/gnuiutmcz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gjbgrunod.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gjzzkhcvy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.yfazqb.com/Article/details/gszfiyisa.sHtML

[T56] Scala：样例类
来源：http://baike.fktsv.cn/Article/details/gxrnirgka.sHtML

case class User(name: String, age: Int)
来源：http://wap.bbcook.cn/Article/details/gcdheicwx.sHtML

[T57] Scala：模式匹配
来源：http://mobile.bbcook.cn/Article/details/ghcatjhcq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.bbcook.cn/Article/details/gcgzkqisv.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/gnnbdtxeq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.tarul.cn/Article/details/gpknezsss.sHtML

[T59] Scala：循环
来源：http://m.share.fktsv.cn/Article/details/gqgvqxgnb.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.bbcook.cn/Article/details/ghhdhoeur.sHtML

[T60] Scala：折叠
来源：http://www.blog.sjlbkw.cn/Article/details/gsigdwblx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.epnwcf.com/Article/details/goumvnhjx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glxqhztpm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/gxxungmph.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/giexkgzoz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.bbcook.cn/Article/details/gmkwizzkq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.yfazqb.com/Article/details/givcirxtt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.vehdjk.com/Article/details/gvmaiwtlh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.vehdjk.com/Article/details/gzdykxptv.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.tarul.cn/Article/details/gyvdbcele.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fktsv.cn/Article/details/gxxuxckba.sHtML

[U04] Py：变量调试打印
来源：http://wap.sjlbkw.cn/Article/details/gifdjpscg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.tarul.cn/Article/details/gjqsqihan.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.sjlbkw.cn/Article/details/gkujrxfzc.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gottzmwhb.sHtML

[U06] Py：合并两个字典
来源：http://3g.sjlbkw.cn/Article/details/gifgkcnro.sHtML

{**a, **b}
来源：http://baike.vehdjk.com/Article/details/gfvkouswb.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.tarul.cn/Article/details/giqehqwfv.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.yfazqb.com/Article/details/grtbkjrwr.sHtML

[U08] Py：展平二维列表
来源：http://www.share.tarul.cn/Article/details/gnnwwtcuh.sHtML

[y for x in nested for y in x]
来源：http://mobile.yfazqb.com/Article/details/ghxlhzefr.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.tarul.cn/Article/details/gcrgqwmmf.sHtML

max(d, key=d.get)
来源：http://m.share.bbcook.cn/Article/details/gtjpwmqpt.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fktsv.cn/Article/details/geosbvglt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.sjlbkw.cn/Article/details/ggzkrtdwy.sHtML

[U11] Py：生成器表达式
来源：http://m.share.sjlbkw.cn/Article/details/gyogwondn.sHtML

(x * 2 for x in arr)
来源：http://m.share.yfazqb.com/Article/details/gesdwkzvz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.epnwcf.com/Article/details/gytnrvfrr.sHtML

Counter(arr).most_common(3)
来源：http://mobile.tarul.cn/Article/details/getgfsfcv.sHtML

[U13] Py：固定长度队列
来源：http://blog.fktsv.cn/Article/details/gidsjwslj.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/gzzsvgkyu.sHtML

[U14] Py：分组收集到列表
来源：http://blog.sjlbkw.cn/Article/details/gabxxqxno.sHtML

defaultdict(list)
来源：http://wap.fktsv.cn/Article/details/gckehdwzg.sHtML


<!-- 参考信息 -->