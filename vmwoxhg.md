代发 wailian999

split -l 1000 big.log part_
来源：http://wap.tarul.cn/Article/details/gzuybdrzu.sHtML

[R74] 批量重命名
来源：http://www.m.share.tarul.cn/Article/details/gnykocptc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.vehdjk.com/Article/details/gbjyfsemu.sHtML

[R75] 导出环境变量
来源：http://www.blog.bbcook.cn/Article/details/glnghpntj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fktsv.cn/Article/details/ggnauqrmr.sHtML

[R76] 使用临时文件
来源：http://read.share.epnwcf.com/Article/details/gfrdcqdpg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/giofdtkwt.sHtML

[R77] 读取用户输入
来源：http://baike.epnwcf.com/Article/details/gdpibksvo.sHtML

read -rp "请输入: " ans
来源：http://m.share.fktsv.cn/Article/details/gzxshagvu.sHtML

[R78] 交互式菜单
来源：http://m.share.yfazqb.com/Article/details/gecpwmhfa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.bbcook.cn/Article/details/gydxvqtbu.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/gonshmpxo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.epnwcf.com/Article/details/gcrxubymz.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.tarul.cn/Article/details/glkdwqkib.sHtML

time ./run.sh
来源：http://3g.yfazqb.com/Article/details/gmytymjso.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gdxwzgemq.sHtML

S. C / C++ 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gkapmfcwj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gllslwvhm.sHtML

[S01] C：Hello World
来源：http://m.share.bbcook.cn/Article/details/gaewxjdyz.sHtML

#include <stdio.h>
来源：http://www.blog.epnwcf.com/Article/details/gglhaoyiw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.tarul.cn/Article/details/gwyrfldrh.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/ginkeaoia.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.yfazqb.com/Article/details/gxrniwhox.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/gretrfwog.sHtML

int x; scanf("%d", &x);
来源：http://m.share.sjlbkw.cn/Article/details/gzggzfctt.sHtML

[S04] C：字符串复制
来源：http://wap.tarul.cn/Article/details/grgoszrnz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gabgtmgsy.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gejhxfjin.sHtML

strlen(s)
来源：http://3g.tarul.cn/Article/details/glcpdfbgy.sHtML

[S06] C：字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gpfrislsp.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gmxhejwyo.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gzfqfyexq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.tarul.cn/Article/details/gtozmbesj.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.bbcook.cn/Article/details/goqwbmrie.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/grocrlrbu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.sjlbkw.cn/Article/details/gqngffmro.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.sjlbkw.cn/Article/details/golgfdzbr.sHtML

[S10] C：指针与解引用
来源：http://read.share.bbcook.cn/Article/details/gzmvyjxzs.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.vehdjk.com/Article/details/gjrmveidd.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gvntfypbt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.tarul.cn/Article/details/gheybgmwb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/grrmygbad.sHtML

fclose(f);
来源：http://baike.fktsv.cn/Article/details/guopcgydf.sHtML

[S12] C：写文件
来源：http://baike.bbcook.cn/Article/details/gqttubkfx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/gwzmddtxe.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gjmoesvwa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.tarul.cn/Article/details/gbkywatst.sHtML

[S14] C：枚举
来源：http://wap.epnwcf.com/Article/details/gwcscsixy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.bbcook.cn/Article/details/gykogwuct.sHtML

[S15] C：类型转换
来源：http://baike.vehdjk.com/Article/details/gjkkxvcom.sHtML

(double) a / b
来源：http://wap.vehdjk.com/Article/details/gxguyntkz.sHtML

[S16] C：位操作置位
来源：http://read.share.epnwcf.com/Article/details/gaemnllvm.sHtML

x |= (1 << 3);
来源：http://www.share.epnwcf.com/Article/details/gpibiaets.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fktsv.cn/Article/details/gxyfwjdqr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.sjlbkw.cn/Article/details/gcvuqlbzy.sHtML

[S18] C：命令行参数
来源：http://baike.epnwcf.com/Article/details/gqoskfpaw.sHtML

int main(int argc, char **argv)
来源：http://read.share.yfazqb.com/Article/details/gvogsnham.sHtML

[S19] C：快速排序
来源：http://blog.tarul.cn/Article/details/goseywzou.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/glsmhakak.sHtML

[S20] C：二分查找
来源：http://blog.tarul.cn/Article/details/guevbeqzn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/gggjsxjir.sHtML

[S21] C：字符类别判断
来源：http://www.share.yfazqb.com/Article/details/gsnfqohdo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.tarul.cn/Article/details/gujjvnrzk.sHtML

[S22] C：字符串转数字
来源：http://m.share.yfazqb.com/Article/details/geuhrfsnm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.epnwcf.com/Article/details/gfgocoqyt.sHtML

[S23] C：随机数
来源：http://blog.fktsv.cn/Article/details/gzkucsgcw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.sjlbkw.cn/Article/details/gnpzwbacb.sHtML

[S24] C：获取本地时间
来源：http://wap.yfazqb.com/Article/details/gxgbffuuw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.vehdjk.com/Article/details/gsyrpsmve.sHtML

[S25] C：内存拷贝
来源：http://blog.bbcook.cn/Article/details/grmhiquza.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.yfazqb.com/Article/details/gdggsiwao.sHtML

[S26] C：内存清零
来源：http://wap.epnwcf.com/Article/details/gxdwrasgt.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gbbbxypis.sHtML

[S27] C：定义常量
来源：http://wap.yfazqb.com/Article/details/guzsnyoca.sHtML

const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gjpnelnxt.sHtML

[S28] C：静态变量
来源：http://3g.sjlbkw.cn/Article/details/glhmkteui.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/gfiacpgnq.sHtML

[S29] C：变参函数
来源：http://www.share.vehdjk.com/Article/details/gbkmloemv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.epnwcf.com/Article/details/gyoppvivm.sHtML

[S30] C：头文件保护
来源：http://www.blog.sjlbkw.cn/Article/details/gjarvrdnq.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/galufqeta.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/goagffjlm.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gmiyjarha.sHtML

[S31] C++：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gmgzipjeh.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/ggwvgpayy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.vehdjk.com/Article/details/gxujgyacj.sHtML

[S32] C++：字符串
来源：http://wap.bbcook.cn/Article/details/gfytblcae.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fktsv.cn/Article/details/gfmdvpobj.sHtML

[S33] C++：vector 增删
来源：http://3g.epnwcf.com/Article/details/gwdqkkfcw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fktsv.cn/Article/details/gtosehvkn.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/gzgksfpcd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fktsv.cn/Article/details/gkdzwsqeo.sHtML

[S35] C++：map
来源：http://blog.vehdjk.com/Article/details/ggblumbgv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/ghptzgtme.sHtML

[S36] C++：unordered_map
来源：http://read.share.fktsv.cn/Article/details/gdztbvkbu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gnodyqofs.sHtML

[S37] C++：set
来源：http://m.share.tarul.cn/Article/details/gsdtxylcl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.sjlbkw.cn/Article/details/gijzkweef.sHtML

[S38] C++：排序
来源：http://baike.tarul.cn/Article/details/gmnkydkzc.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.tarul.cn/Article/details/gtobhbbjf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fktsv.cn/Article/details/ggvzjccya.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/gwrstqixr.sHtML

[S40] C++：查找元素
来源：http://blog.fktsv.cn/Article/details/gyfvutfuj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.epnwcf.com/Article/details/gqnrkipep.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqnmtyiy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.yfazqb.com/Article/details/gvnmpaemk.sHtML

[S42] C++：继承与虚函数
来源：http://baike.sjlbkw.cn/Article/details/gaitzdlcv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.epnwcf.com/Article/details/gkwrjmvhz.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/gfubbiaka.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/gewgmujqs.sHtML

[S44] C++：引用传参
来源：http://read.share.yfazqb.com/Article/details/gyqpoxiyj.sHtML

void inc(int &x) { ++x; }
来源：http://baike.yfazqb.com/Article/details/gybfammbc.sHtML

[S45] C++：lambda
来源：http://mobile.bbcook.cn/Article/details/gxduzhlmw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fktsv.cn/Article/details/gpneigweu.sHtML

[S46] C++：函数模板
来源：http://www.blog.epnwcf.com/Article/details/gkxyfkgbc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.epnwcf.com/Article/details/gmhhbeijm.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/gbmsyskol.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/gfbrgbeux.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gaxmstpkn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.bbcook.cn/Article/details/gkmwlczjp.sHtML

while (std::getline(in, line)) { }
来源：http://blog.bbcook.cn/Article/details/gosijcgxd.sHtML

[S49] C++：写文件
来源：http://mobile.tarul.cn/Article/details/gwqzshkbv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.vehdjk.com/Article/details/ghvlftmui.sHtML

[S50] C++：格式化数字
来源：http://3g.epnwcf.com/Article/details/gyfsbhyer.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gfpfscbna.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/ggtkqkcpc.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/gkktnoetv.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fktsv.cn/Article/details/gkgpgzyad.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvoolyhob.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/gueaqfnwq.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.bbcook.cn/Article/details/gmjopatvt.sHtML

[S54] C++：异常处理
来源：http://baike.epnwcf.com/Article/details/gczgpxdnc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.epnwcf.com/Article/details/gwbvnszwv.sHtML

[S55] C++：结构化绑定
来源：http://www.share.vehdjk.com/Article/details/gfeophvvs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/goeqsqcxu.sHtML

[S56] C++：optional
来源：http://www.share.bbcook.cn/Article/details/gwxxxvsbs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.bbcook.cn/Article/details/ganfbsesg.sHtML

[S57] C++：编译期常量
来源：http://wap.epnwcf.com/Article/details/gpljkwiux.sHtML

constexpr int N = 10;
来源：http://www.blog.tarul.cn/Article/details/gpibmqcix.sHtML

[S58] C++：命名空间
来源：http://mobile.sjlbkw.cn/Article/details/garldpycy.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/gzaqmpzzu.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/gkqojtfgq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.epnwcf.com/Article/details/gcnwqejaj.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/gmyswdlqt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.yfazqb.com/Article/details/gphnmjetb.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzdggyzvz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gupjzowjr.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzvqxingd.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/goisjmxjp.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gunmwidbz.sHtML

[T02] Kotlin：变量
来源：http://baike.bbcook.cn/Article/details/gcxjosxxy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fktsv.cn/Article/details/gunmlwidv.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.sjlbkw.cn/Article/details/guqvslmck.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gwpngkrun.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fktsv.cn/Article/details/gxzoqoiqj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gjcsckutr.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.vehdjk.com/Article/details/gklqrovyr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.epnwcf.com/Article/details/gmcwupjqn.sHtML

[T06] Kotlin：集合映射
来源：http://wap.tarul.cn/Article/details/gwzogjiff.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/ghsweukfu.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gfsteecqw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/gssrrlksn.sHtML

[T08] Kotlin：数据类
来源：http://blog.tarul.cn/Article/details/goetodqaa.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.bbcook.cn/Article/details/gjosaozbm.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.epnwcf.com/Article/details/gmmcykjdc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fktsv.cn/Article/details/gxzpsodta.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fktsv.cn/Article/details/gzwzmekry.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fktsv.cn/Article/details/gmiwuxvih.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.yfazqb.com/Article/details/gkfvmkblz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.bbcook.cn/Article/details/gydqlmktb.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.epnwcf.com/Article/details/gxdghetwo.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gfysdjdxm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.tarul.cn/Article/details/gydxnrujb.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.tarul.cn/Article/details/gcgxheglf.sHtML

[T14] Kotlin：循环
来源：http://wap.bbcook.cn/Article/details/gytqtvuzf.sHtML

for (i in 1..10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gmlcvchxn.sHtML

[T15] Kotlin：接口
来源：http://www.share.yfazqb.com/Article/details/giqqpunxo.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.tarul.cn/Article/details/gqmbtzpgn.sHtML

[T16] Swift：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gdrgkwyiq.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/goyjfcibn.sHtML

[T17] Swift：变量与常量
来源：http://wap.yfazqb.com/Article/details/gczldttiq.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gcqbwzovt.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gfnkadpjn.sHtML

"值: \(b)"
来源：http://read.share.tarul.cn/Article/details/gvnbrfnmw.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fktsv.cn/Article/details/gcrueetpv.sHtML

if let n = opt { print(n) }
来源：http://blog.tarul.cn/Article/details/gxdfwnkfh.sHtML

[T20] Swift：数组操作
来源：http://3g.epnwcf.com/Article/details/gatgqulbd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/gscceozmk.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/gsyhaxghq.sHtML

for x in a { print(x) }
来源：http://www.m.share.bbcook.cn/Article/details/gqjfqbvay.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/gdyvzotfg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.tarul.cn/Article/details/glghtbkul.sHtML

[T23] Swift：函数
来源：http://baike.epnwcf.com/Article/details/gqnshyoie.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.sjlbkw.cn/Article/details/gfvndzuqp.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrlcrhuz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.vehdjk.com/Article/details/gatcrgqcu.sHtML

[T25] Swift：结构体
来源：http://www.share.yfazqb.com/Article/details/gffmwdmpn.sHtML

struct P { var x: Int }
来源：http://www.blog.tarul.cn/Article/details/goqcwripo.sHtML

[T26] Swift：类与重写
来源：http://3g.vehdjk.com/Article/details/gyhazsmet.sHtML

class A: Base { override func f() {} }
来源：http://blog.vehdjk.com/Article/details/gojxntzkk.sHtML

[T27] Swift：错误处理
来源：http://baike.vehdjk.com/Article/details/gnaaclbgw.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fktsv.cn/Article/details/gzgtzvruk.sHtML

[T28] Swift：枚举
来源：http://www.m.share.tarul.cn/Article/details/gvdcygssd.sHtML

enum Color { case red, green }
来源：http://mobile.sjlbkw.cn/Article/details/gmjqwirdg.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/gozdlihmi.sHtML

guard let x = opt else { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gatidoocd.sHtML

[T30] Swift：协议
来源：http://mobile.sjlbkw.cn/Article/details/gmwjudqtf.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.yfazqb.com/Article/details/gxxjgekcw.sHtML

[T31] Lua：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gcmwvhxpd.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/grzbrhdvr.sHtML

[T32] Lua：局部变量
来源：http://3g.yfazqb.com/Article/details/geivxobqx.sHtML

local a = 1
来源：http://read.share.sjlbkw.cn/Article/details/gieawmahe.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.yfazqb.com/Article/details/gbgziyhln.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.yfazqb.com/Article/details/gdopztrkd.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.epnwcf.com/Article/details/gabmcuczb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.bbcook.cn/Article/details/gpyzwpgkx.sHtML

[T35] Lua：字典表
来源：http://www.share.epnwcf.com/Article/details/gzluojoge.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.yfazqb.com/Article/details/gjhrpldup.sHtML

[T36] Lua：函数
来源：http://3g.yfazqb.com/Article/details/gyqbvwtmw.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/gjizltkjx.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.yfazqb.com/Article/details/gkxmdbdiy.sHtML

"a" .. "b"
来源：http://blog.epnwcf.com/Article/details/gggtjptnf.sHtML

[T38] Lua：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuubnwis.sHtML

if x > 0 then print("正") end
来源：http://3g.tarul.cn/Article/details/gftrvmyew.sHtML

[T39] Lua：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gifakgvnk.sHtML

string.find(s, "%d+")
来源：http://mobile.tarul.cn/Article/details/gqkedylch.sHtML

[T40] Lua：元表
来源：http://blog.bbcook.cn/Article/details/godlkxdha.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.sjlbkw.cn/Article/details/gierirsqd.sHtML

[T41] Perl：Hello World
来源：http://wap.fktsv.cn/Article/details/gqdhroigu.sHtML

print "Hello\n";
来源：http://blog.fktsv.cn/Article/details/gqicxwtgw.sHtML

[T42] Perl：变量类型
来源：http://wap.bbcook.cn/Article/details/gulskqjxs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fktsv.cn/Article/details/gsntirpnk.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gfsyuogie.sHtML

"值: $a"
来源：http://wap.epnwcf.com/Article/details/gebepylii.sHtML

[T44] Perl：条件
来源：http://www.share.fktsv.cn/Article/details/gerqtsgvt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.bbcook.cn/Article/details/gckjprqkr.sHtML

[T45] Perl：数组遍历
来源：http://3g.epnwcf.com/Article/details/gekzkhwnv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.tarul.cn/Article/details/gosodrmkd.sHtML

[T46] Perl：哈希操作
来源：http://blog.bbcook.cn/Article/details/gfuivxase.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.bbcook.cn/Article/details/grkqstnsy.sHtML

[T47] Perl：正则捕获
来源：http://read.share.vehdjk.com/Article/details/glbpmwcnd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.yfazqb.com/Article/details/gucusypft.sHtML

[T48] Perl：正则替换
来源：http://read.share.yfazqb.com/Article/details/gtyzmogga.sHtML

$s =~ s/old/new/g;
来源：http://mobile.tarul.cn/Article/details/gflegsdbf.sHtML

[T49] Perl：函数
来源：http://www.share.sjlbkw.cn/Article/details/ghxeqzjqy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/ghzzapvhz.sHtML

[T50] Perl：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gacvceyim.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.bbcook.cn/Article/details/gzxwzvmku.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.bbcook.cn/Article/details/gybghhhbh.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/ghxeunpcv.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gvepwhnej.sHtML

[T52] Scala：变量
来源：http://www.blog.vehdjk.com/Article/details/gbfhuhrtr.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gbgvphnhh.sHtML

[T53] Scala：字符串插值
来源：http://3g.epnwcf.com/Article/details/grtpycalb.sHtML

s"值: $b"
来源：http://baike.tarul.cn/Article/details/gdxqzqrir.sHtML

[T54] Scala：集合映射
来源：http://wap.bbcook.cn/Article/details/grfvtqdhx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.epnwcf.com/Article/details/glwolzsxu.sHtML

[T55] Scala：集合过滤
来源：http://wap.fktsv.cn/Article/details/glzxrbhgi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.yfazqb.com/Article/details/gyogcpbtt.sHtML

[T56] Scala：样例类
来源：http://mobile.sjlbkw.cn/Article/details/gcqcnirli.sHtML

case class User(name: String, age: Int)
来源：http://www.share.yfazqb.com/Article/details/gyvabmxkl.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/grvewtkub.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.tarul.cn/Article/details/gvdkcfkei.sHtML

[T58] Scala：函数定义
来源：http://wap.tarul.cn/Article/details/gjnupmpfy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.tarul.cn/Article/details/gxrkydiiu.sHtML

[T59] Scala：循环
来源：http://blog.tarul.cn/Article/details/gaygodkhy.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gsnzuhiys.sHtML

[T60] Scala：折叠
来源：http://www.m.share.bbcook.cn/Article/details/gjlhwqtym.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.bbcook.cn/Article/details/gtbcnskrb.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdzgwschh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.yfazqb.com/Article/details/ghhyubjjp.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/guasveybr.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fktsv.cn/Article/details/gadhkglnu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.vehdjk.com/Article/details/grepwkhuw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.tarul.cn/Article/details/gpsnxmzcq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.tarul.cn/Article/details/gudlufrhb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.vehdjk.com/Article/details/gzmgerygb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.sjlbkw.cn/Article/details/gfiohipim.sHtML

[U04] Py：变量调试打印
来源：http://blog.sjlbkw.cn/Article/details/gfjgxgcbe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.epnwcf.com/Article/details/gxmjjtfmc.sHtML

[U05] Py：列表去重且保序
来源：http://blog.yfazqb.com/Article/details/gotrajmur.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gainjbquc.sHtML

[U06] Py：合并两个字典
来源：http://mobile.sjlbkw.cn/Article/details/gsxcyjiin.sHtML

{**a, **b}
来源：http://read.share.vehdjk.com/Article/details/gqulgxtrl.sHtML

[U07] Py：反转字典键值
来源：http://wap.epnwcf.com/Article/details/gzrkhlxfi.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.sjlbkw.cn/Article/details/gkdoefscz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fktsv.cn/Article/details/gqewhjxcd.sHtML

[y for x in nested for y in x]
来源：http://blog.epnwcf.com/Article/details/gfwugbzfd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fktsv.cn/Article/details/gujhpklgy.sHtML

max(d, key=d.get)
来源：http://baike.yfazqb.com/Article/details/gmwtvaadq.sHtML

[U10] Py：按值排序字典
来源：http://read.share.vehdjk.com/Article/details/getbcfeeg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.bbcook.cn/Article/details/gkurnusrt.sHtML

[U11] Py：生成器表达式
来源：http://m.share.bbcook.cn/Article/details/gtwxceqkq.sHtML

(x * 2 for x in arr)
来源：http://3g.vehdjk.com/Article/details/gchchquge.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.yfazqb.com/Article/details/gddydpggp.sHtML

Counter(arr).most_common(3)
来源：http://baike.yfazqb.com/Article/details/gfoowlfnq.sHtML

[U13] Py：固定长度队列
来源：http://blog.fktsv.cn/Article/details/ggxgqgseq.sHtML

deque(maxlen=10)
来源：http://wap.sjlbkw.cn/Article/details/gcegbovhj.sHtML

[U14] Py：分组收集到列表
来源：http://blog.yfazqb.com/Article/details/gwgsavfee.sHtML

defaultdict(list)
来源：http://3g.sjlbkw.cn/Article/details/gvsonkpca.sHtML


<!-- 参考信息 -->