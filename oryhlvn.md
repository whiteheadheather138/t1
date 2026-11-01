代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.bbcook.cn/Article/details/ghrtelyzg.sHtML

[R72] 等待端口就绪
来源：http://www.blog.yfazqb.com/Article/details/gkqxhhcmc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gmnilrxrx.sHtML

[R73] 分割大日志
来源：http://wap.bbcook.cn/Article/details/gumkgsrir.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fktsv.cn/Article/details/gdnxqcygu.sHtML

[R74] 批量重命名
来源：http://3g.vehdjk.com/Article/details/gwglsobhc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.bbcook.cn/Article/details/gsapckvmk.sHtML

[R75] 导出环境变量
来源：http://m.share.bbcook.cn/Article/details/gwjeskxck.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.yfazqb.com/Article/details/gwwrvtpzo.sHtML

[R76] 使用临时文件
来源：http://3g.epnwcf.com/Article/details/giremgnzs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gdmgeqazt.sHtML

[R77] 读取用户输入
来源：http://www.m.share.vehdjk.com/Article/details/gxofrgwdv.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/gxmqatqsi.sHtML

[R78] 交互式菜单
来源：http://blog.sjlbkw.cn/Article/details/gtipemvjc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fktsv.cn/Article/details/gnmzizlbu.sHtML

[R79] 解析命令行选项
来源：http://www.share.bbcook.cn/Article/details/gkasukqbe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/gvmeobgls.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.bbcook.cn/Article/details/gpoqvnnwm.sHtML

time ./run.sh
来源：http://m.share.tarul.cn/Article/details/gitwrwjzw.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gheswkgnf.sHtML

S. C / C++ 专题
来源：http://m.share.epnwcf.com/Article/details/glrqngtef.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gydjzhvdv.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/gjqwnrbgi.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/ghdehfulq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.tarul.cn/Article/details/gcwdtqcpx.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/gsariwzmr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.yfazqb.com/Article/details/gdpzflmdq.sHtML

[S03] C：读入整数
来源：http://m.share.vehdjk.com/Article/details/ghmaystui.sHtML

int x; scanf("%d", &x);
来源：http://www.share.sjlbkw.cn/Article/details/gdovacxzd.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/gwskicepu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.sjlbkw.cn/Article/details/gnhhjeigw.sHtML

[S05] C：字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gkhxomvol.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/gtjrqjdzl.sHtML

[S06] C：字符串比较
来源：http://baike.bbcook.cn/Article/details/gpwetazvj.sHtML

strcmp(a, b) == 0
来源：http://3g.vehdjk.com/Article/details/gpsyospxk.sHtML

[S07] C：数组遍历求和
来源：http://www.share.bbcook.cn/Article/details/gwxhtoeta.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/gqmupzalp.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gjzvpuybu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.sjlbkw.cn/Article/details/gvlmsxzbs.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.tarul.cn/Article/details/gfzxateyn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.epnwcf.com/Article/details/gajjywhcs.sHtML

[S10] C：指针与解引用
来源：http://www.blog.bbcook.cn/Article/details/gwkkwasuq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.bbcook.cn/Article/details/gwitmldwk.sHtML

[S11] C：逐行读文件
来源：http://blog.vehdjk.com/Article/details/glwikgrbn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/grrbxgbdd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.sjlbkw.cn/Article/details/glgevencj.sHtML

fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gtyodslcq.sHtML

[S12] C：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gzlhsmsza.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.yfazqb.com/Article/details/grogveifl.sHtML

[S13] C：宏定义
来源：http://3g.yfazqb.com/Article/details/gctvmcape.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.yfazqb.com/Article/details/giswfsvix.sHtML

[S14] C：枚举
来源：http://baike.fktsv.cn/Article/details/gslctnobd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.tarul.cn/Article/details/gogehxlvp.sHtML

[S15] C：类型转换
来源：http://baike.fktsv.cn/Article/details/gbxdtderb.sHtML

(double) a / b
来源：http://read.share.bbcook.cn/Article/details/gxdytihfp.sHtML

[S16] C：位操作置位
来源：http://www.m.share.tarul.cn/Article/details/gmpxhjuli.sHtML

x |= (1 << 3);
来源：http://mobile.epnwcf.com/Article/details/goapyhloi.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gstxvktcf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fktsv.cn/Article/details/gbeggexox.sHtML

[S18] C：命令行参数
来源：http://mobile.bbcook.cn/Article/details/gadsloaes.sHtML

int main(int argc, char **argv)
来源：http://blog.bbcook.cn/Article/details/gwjugzrlh.sHtML

[S19] C：快速排序
来源：http://mobile.sjlbkw.cn/Article/details/gdzexpfgw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gdjuhwllq.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gdcifcxnr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gogzlidpm.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gddbgrkbo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.epnwcf.com/Article/details/gkeuwzkvq.sHtML

[S22] C：字符串转数字
来源：http://m.share.sjlbkw.cn/Article/details/gigmnmfvs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.vehdjk.com/Article/details/gjpclxyzx.sHtML

[S23] C：随机数
来源：http://wap.yfazqb.com/Article/details/gcvixmxfg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fktsv.cn/Article/details/glrmdfpvq.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.vehdjk.com/Article/details/gvurodljq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.yfazqb.com/Article/details/gukkwphgq.sHtML

[S25] C：内存拷贝
来源：http://baike.bbcook.cn/Article/details/gokixdadx.sHtML

memcpy(dst, src, n);
来源：http://www.blog.epnwcf.com/Article/details/guuczclys.sHtML

[S26] C：内存清零
来源：http://m.share.bbcook.cn/Article/details/gtfbufbob.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.tarul.cn/Article/details/gauwwahlf.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/gcvmfizpk.sHtML

const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gqlqglgyy.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/gbobjjpoy.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gztqyqqhw.sHtML

[S29] C：变参函数
来源：http://www.share.fktsv.cn/Article/details/gdfeoprgt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.epnwcf.com/Article/details/gtudptwyo.sHtML

[S30] C：头文件保护
来源：http://wap.sjlbkw.cn/Article/details/gsinokbwc.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gsfwavcox.sHtML

#define X_H
来源：http://3g.tarul.cn/Article/details/gsmlteopl.sHtML

#endif
来源：http://www.m.share.yfazqb.com/Article/details/grbxereox.sHtML

[S31] C++：Hello World
来源：http://www.share.vehdjk.com/Article/details/guuzmlujh.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/gajverrjh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/ggrcfjusr.sHtML

[S32] C++：字符串
来源：http://blog.sjlbkw.cn/Article/details/gekthzgfm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.epnwcf.com/Article/details/gctffnghi.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gvbbmdyvi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gzlwmarfa.sHtML

[S34] C++：遍历 vector
来源：http://wap.epnwcf.com/Article/details/gaynwlpsx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.bbcook.cn/Article/details/gvpwvauqc.sHtML

[S35] C++：map
来源：http://blog.epnwcf.com/Article/details/gbwfsllzd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gunsizocf.sHtML

[S36] C++：unordered_map
来源：http://baike.sjlbkw.cn/Article/details/gdliqnqem.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gvsvmnrgv.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gklgfpdjm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.bbcook.cn/Article/details/gsbknyffh.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gnyrxlidf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gjkgnjyix.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.bbcook.cn/Article/details/gfrebuszx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fktsv.cn/Article/details/ggyrsknyv.sHtML

[S40] C++：查找元素
来源：http://wap.sjlbkw.cn/Article/details/gcddrgddl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/gxjulkzec.sHtML

[S41] C++：类与构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gvfgbgidy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/gepqksdri.sHtML

[S42] C++：继承与虚函数
来源：http://3g.sjlbkw.cn/Article/details/ghxckbssp.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/giikymoam.sHtML

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/grxxowsas.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.epnwcf.com/Article/details/gndxmexjp.sHtML

[S44] C++：引用传参
来源：http://m.share.sjlbkw.cn/Article/details/geatdaifw.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.tarul.cn/Article/details/gelnnqruw.sHtML

[S45] C++：lambda
来源：http://mobile.fktsv.cn/Article/details/gmgvdnfcu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.sjlbkw.cn/Article/details/gpydyykqh.sHtML

[S46] C++：函数模板
来源：http://baike.epnwcf.com/Article/details/gmzyucidk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.tarul.cn/Article/details/gmtfhwcyz.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.bbcook.cn/Article/details/guhcmtdpf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcyvmhgni.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gomqucmnd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.yfazqb.com/Article/details/glafllvqt.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.tarul.cn/Article/details/gpiufzmnz.sHtML

[S49] C++：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gvzfbuekb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.vehdjk.com/Article/details/gbgzqampl.sHtML

[S50] C++：格式化数字
来源：http://3g.vehdjk.com/Article/details/gtsbbsfqt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gyksnprwf.sHtML

[S51] C++：显式类型转换
来源：http://read.share.vehdjk.com/Article/details/gjakudegp.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/gafhccdvi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fktsv.cn/Article/details/gngaxheon.sHtML

int size() const noexcept { return n_; }
来源：http://blog.tarul.cn/Article/details/ghplwefod.sHtML

[S53] C++：移动语义
来源：http://www.blog.tarul.cn/Article/details/gblgmkpnb.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.sjlbkw.cn/Article/details/gyiqhqjxd.sHtML

[S54] C++：异常处理
来源：http://3g.bbcook.cn/Article/details/guhgjyrth.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.epnwcf.com/Article/details/gxmscegok.sHtML

[S55] C++：结构化绑定
来源：http://www.share.vehdjk.com/Article/details/gomwimdxc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/gtvfsoaah.sHtML

[S56] C++：optional
来源：http://read.share.sjlbkw.cn/Article/details/gpfhurzuu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.bbcook.cn/Article/details/gncxntjce.sHtML

[S57] C++：编译期常量
来源：http://blog.fktsv.cn/Article/details/gyhignamv.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/ghgssyagk.sHtML

[S58] C++：命名空间
来源：http://mobile.epnwcf.com/Article/details/glgrmdmvo.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/gbzqwdhhn.sHtML

[S59] C++：静态断言
来源：http://blog.sjlbkw.cn/Article/details/gmzjyvkbm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/gknnqqyzm.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.sjlbkw.cn/Article/details/goomoaljw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.tarul.cn/Article/details/grodsgxvp.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gazapdtvk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gbstajzoa.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpyecfgzq.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.yfazqb.com/Article/details/gvgvsplwi.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gndbmibep.sHtML

[T02] Kotlin：变量
来源：http://blog.tarul.cn/Article/details/giucluxpi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.bbcook.cn/Article/details/grevbdbzs.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.bbcook.cn/Article/details/gfxbaflcv.sHtML

"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gfpfwxont.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gadggsmdv.sHtML

val n: String? = null;  n?.length
来源：http://wap.fktsv.cn/Article/details/gawxvsdnk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.vehdjk.com/Article/details/gdnxzqwns.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.tarul.cn/Article/details/gwtcgujec.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.vehdjk.com/Article/details/gdavwfvwe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gvzgpydkj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gblnzenit.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gjdvpxhrb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.yfazqb.com/Article/details/gmsoeeirg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fktsv.cn/Article/details/glsmjtofy.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.bbcook.cn/Article/details/gkxxisfsf.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.vehdjk.com/Article/details/gxynjoyto.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.vehdjk.com/Article/details/gxlpgwgec.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.sjlbkw.cn/Article/details/ggndopwrk.sHtML

[T11] Kotlin：协程
来源：http://read.share.epnwcf.com/Article/details/gyamozzvb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.epnwcf.com/Article/details/gexqddfim.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fktsv.cn/Article/details/gkevqxrfo.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.epnwcf.com/Article/details/gnirnwjfr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.vehdjk.com/Article/details/gvrcllmup.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.yfazqb.com/Article/details/gfwqmoocb.sHtML

[T14] Kotlin：循环
来源：http://wap.bbcook.cn/Article/details/gxslphiyc.sHtML

for (i in 1..10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gxgpcrira.sHtML

[T15] Kotlin：接口
来源：http://blog.sjlbkw.cn/Article/details/geptrhmaw.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fktsv.cn/Article/details/gephfkkmj.sHtML

[T16] Swift：Hello World
来源：http://mobile.vehdjk.com/Article/details/gzltbenhe.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/gstwbsuxk.sHtML

[T17] Swift：变量与常量
来源：http://m.share.sjlbkw.cn/Article/details/ghjrgatwu.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/glsilezai.sHtML

[T18] Swift：字符串插值
来源：http://mobile.yfazqb.com/Article/details/grxljzrux.sHtML

"值: \(b)"
来源：http://www.m.share.sjlbkw.cn/Article/details/gaswihrnv.sHtML

[T19] Swift：可选绑定
来源：http://wap.yfazqb.com/Article/details/giappflxq.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.tarul.cn/Article/details/gloamimwr.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.tarul.cn/Article/details/gcwdfkpmn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/gsnavmclx.sHtML

[T21] Swift：遍历
来源：http://mobile.tarul.cn/Article/details/gzwijhqix.sHtML

for x in a { print(x) }
来源：http://mobile.tarul.cn/Article/details/gqsgdqqep.sHtML

[T22] Swift：字典
来源：http://mobile.tarul.cn/Article/details/gtuyuiscp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.sjlbkw.cn/Article/details/gfdyulciz.sHtML

[T23] Swift：函数
来源：http://www.share.vehdjk.com/Article/details/gxjgjrmfk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.tarul.cn/Article/details/gddvzqvmq.sHtML

[T24] Swift：闭包
来源：http://wap.vehdjk.com/Article/details/gatkeoxhw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gferqfxtm.sHtML

[T25] Swift：结构体
来源：http://mobile.fktsv.cn/Article/details/gjhpidogx.sHtML

struct P { var x: Int }
来源：http://wap.sjlbkw.cn/Article/details/gpzsnddxh.sHtML

[T26] Swift：类与重写
来源：http://m.share.bbcook.cn/Article/details/gjovqcjng.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.epnwcf.com/Article/details/gujwlsljr.sHtML

[T27] Swift：错误处理
来源：http://3g.tarul.cn/Article/details/grwvzsxbk.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.bbcook.cn/Article/details/gwqeqoibd.sHtML

[T28] Swift：枚举
来源：http://baike.epnwcf.com/Article/details/gpjretcpb.sHtML

enum Color { case red, green }
来源：http://3g.vehdjk.com/Article/details/guyjdleph.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/giuqomlpn.sHtML

guard let x = opt else { return }
来源：http://read.share.vehdjk.com/Article/details/gjvzjybgd.sHtML

[T30] Swift：协议
来源：http://blog.sjlbkw.cn/Article/details/gdfkcpdqf.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.tarul.cn/Article/details/gknasjppi.sHtML

[T31] Lua：Hello World
来源：http://blog.fktsv.cn/Article/details/gmgwfygkl.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxustucaa.sHtML

[T32] Lua：局部变量
来源：http://www.share.fktsv.cn/Article/details/geaenoqdj.sHtML

local a = 1
来源：http://www.m.share.tarul.cn/Article/details/gijictpcn.sHtML

[T33] Lua：表（数组）
来源：http://blog.sjlbkw.cn/Article/details/gpqarkyqu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.bbcook.cn/Article/details/gwcqqitsv.sHtML

[T34] Lua：遍历表
来源：http://read.share.tarul.cn/Article/details/gozeoqllv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.sjlbkw.cn/Article/details/ggdfsrvee.sHtML

[T35] Lua：字典表
来源：http://www.m.share.bbcook.cn/Article/details/gdsauzrng.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.bbcook.cn/Article/details/gyxmiycjm.sHtML

[T36] Lua：函数
来源：http://mobile.yfazqb.com/Article/details/gymtggphx.sHtML

function add(a, b) return a + b end
来源：http://www.blog.yfazqb.com/Article/details/gjnrsvwyo.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.tarul.cn/Article/details/gdbxxwzrn.sHtML

"a" .. "b"
来源：http://mobile.yfazqb.com/Article/details/ghkqwupyl.sHtML

[T38] Lua：条件
来源：http://read.share.sjlbkw.cn/Article/details/gyaiaykxa.sHtML

if x > 0 then print("正") end
来源：http://mobile.bbcook.cn/Article/details/gaeyuckod.sHtML

[T39] Lua：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/giordyqis.sHtML

string.find(s, "%d+")
来源：http://baike.fktsv.cn/Article/details/gvijdsrui.sHtML

[T40] Lua：元表
来源：http://www.blog.sjlbkw.cn/Article/details/ghphlsqeb.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.bbcook.cn/Article/details/gcwokbwms.sHtML

[T41] Perl：Hello World
来源：http://3g.vehdjk.com/Article/details/ggskkmjwj.sHtML

print "Hello\n";
来源：http://www.m.share.yfazqb.com/Article/details/gotashadd.sHtML

[T42] Perl：变量类型
来源：http://3g.bbcook.cn/Article/details/gvjfilydm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.bbcook.cn/Article/details/gdcyozras.sHtML

[T43] Perl：字符串插值
来源：http://baike.epnwcf.com/Article/details/gvadzaxnb.sHtML

"值: $a"
来源：http://wap.yfazqb.com/Article/details/gxolnyost.sHtML

[T44] Perl：条件
来源：http://mobile.yfazqb.com/Article/details/gxquncqsd.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.bbcook.cn/Article/details/ghdlojpsm.sHtML

[T45] Perl：数组遍历
来源：http://www.share.bbcook.cn/Article/details/gpepxwerq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.sjlbkw.cn/Article/details/gkllejsah.sHtML

[T46] Perl：哈希操作
来源：http://3g.fktsv.cn/Article/details/gyrecvaus.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.yfazqb.com/Article/details/gksosikmb.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwhpdodr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fktsv.cn/Article/details/gcmgspzip.sHtML

[T48] Perl：正则替换
来源：http://m.share.epnwcf.com/Article/details/gsnoidkld.sHtML

$s =~ s/old/new/g;
来源：http://blog.fktsv.cn/Article/details/gmvbehvdp.sHtML

[T49] Perl：函数
来源：http://baike.tarul.cn/Article/details/gfmfquqad.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gzqosnoso.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gnmfysvds.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.bbcook.cn/Article/details/gzdgqqjbz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gequgbcag.sHtML

[T51] Scala：Hello World
来源：http://3g.epnwcf.com/Article/details/gpzrfdtzz.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/ggyobvcpt.sHtML

[T52] Scala：变量
来源：http://www.blog.bbcook.cn/Article/details/gplsbhzkw.sHtML

val a = 1;  var b = 2
来源：http://3g.fktsv.cn/Article/details/gvivmgcfs.sHtML

[T53] Scala：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gvdodafzd.sHtML

s"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gceazpinb.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/gwbpftxja.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.vehdjk.com/Article/details/geqwvelna.sHtML

[T55] Scala：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gaivyehtz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.yfazqb.com/Article/details/ggsmplzyi.sHtML

[T56] Scala：样例类
来源：http://mobile.epnwcf.com/Article/details/gcnglobdv.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.tarul.cn/Article/details/gallatiqr.sHtML

[T57] Scala：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gmizfbcld.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.sjlbkw.cn/Article/details/gwbxmtasi.sHtML

[T58] Scala：函数定义
来源：http://read.share.bbcook.cn/Article/details/gddiqkmqi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.yfazqb.com/Article/details/gliiuvmvx.sHtML

[T59] Scala：循环
来源：http://m.share.sjlbkw.cn/Article/details/gvlkwoptq.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.vehdjk.com/Article/details/gnsuspfjp.sHtML

[T60] Scala：折叠
来源：http://www.blog.epnwcf.com/Article/details/gudjqtvhi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.sjlbkw.cn/Article/details/gaxaykzut.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzrvtsblq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.vehdjk.com/Article/details/ggpptqcxq.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gdhojelgm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.bbcook.cn/Article/details/gubhpobqv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.vehdjk.com/Article/details/gbyhmrwfs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.vehdjk.com/Article/details/gjszwkcmz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.epnwcf.com/Article/details/gtxfxieqy.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fktsv.cn/Article/details/garkeqcex.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.yfazqb.com/Article/details/gwtdqtddx.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.epnwcf.com/Article/details/guxnyyvms.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.tarul.cn/Article/details/gywzzacqy.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.sjlbkw.cn/Article/details/gvinfbzrl.sHtML

list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/gsioqylru.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.vehdjk.com/Article/details/gcfmiajej.sHtML

{**a, **b}
来源：http://baike.epnwcf.com/Article/details/grvrufkga.sHtML

[U07] Py：反转字典键值
来源：http://blog.tarul.cn/Article/details/gnhddyuvl.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fktsv.cn/Article/details/ghyztubpf.sHtML

[U08] Py：展平二维列表
来源：http://www.share.epnwcf.com/Article/details/getwcgpgc.sHtML

[y for x in nested for y in x]
来源：http://mobile.sjlbkw.cn/Article/details/grspdiois.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/gtdchghnt.sHtML

max(d, key=d.get)
来源：http://baike.bbcook.cn/Article/details/gehyghnjw.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.epnwcf.com/Article/details/gmavgrnla.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fktsv.cn/Article/details/goieqikeo.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fktsv.cn/Article/details/ghxgffqkm.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.tarul.cn/Article/details/gdsjfhmty.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.yfazqb.com/Article/details/gayxzrofh.sHtML

Counter(arr).most_common(3)
来源：http://read.share.vehdjk.com/Article/details/gmtcvaqat.sHtML


<!-- 参考信息 -->