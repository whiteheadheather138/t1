代发 wailian999

split -l 1000 big.log part_
来源：http://3g.sjlbkw.cn/Article/details/gbunpbwbz.sHtML

[R74] 批量重命名
来源：http://wap.tarul.cn/Article/details/gqfuqbrlt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/globgyuhs.sHtML

[R75] 导出环境变量
来源：http://m.share.vehdjk.com/Article/details/gxbcazkvj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.epnwcf.com/Article/details/gjwelobjs.sHtML

[R76] 使用临时文件
来源：http://wap.sjlbkw.cn/Article/details/gfnmqajgb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/gvhxxonrq.sHtML

[R77] 读取用户输入
来源：http://blog.bbcook.cn/Article/details/gqsoyrrwp.sHtML

read -rp "请输入: " ans
来源：http://www.share.fktsv.cn/Article/details/gcngfjpcu.sHtML

[R78] 交互式菜单
来源：http://mobile.sjlbkw.cn/Article/details/glnpueeha.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/gzlwmooub.sHtML

[R79] 解析命令行选项
来源：http://read.share.fktsv.cn/Article/details/gxtobpdmm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.bbcook.cn/Article/details/gzhxsdlca.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.vehdjk.com/Article/details/gpnvwuxnn.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/gpvfiptmt.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmxcxykbk.sHtML

S. C / C++ 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gqflsembc.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpjhsxfhk.sHtML

[S01] C：Hello World
来源：http://baike.vehdjk.com/Article/details/gorrhyiuw.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/gtmfqumfn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.vehdjk.com/Article/details/gqpmomybz.sHtML

[S02] C：变量与格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gujytyqvi.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fktsv.cn/Article/details/gdnjbkvyt.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/gbveldnyg.sHtML

int x; scanf("%d", &x);
来源：http://m.share.tarul.cn/Article/details/giiozzmdf.sHtML

[S04] C：字符串复制
来源：http://3g.sjlbkw.cn/Article/details/gueudnueh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.vehdjk.com/Article/details/gwlvzjeec.sHtML

[S05] C：字符串长度
来源：http://m.share.vehdjk.com/Article/details/gykodfcgx.sHtML

strlen(s)
来源：http://www.share.fktsv.cn/Article/details/gckvhmuww.sHtML

[S06] C：字符串比较
来源：http://m.share.fktsv.cn/Article/details/giczpsyzr.sHtML

strcmp(a, b) == 0
来源：http://www.blog.tarul.cn/Article/details/gqwcwmmvu.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gcgqanoie.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/gqsmwohlj.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/gwoldunwn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.yfazqb.com/Article/details/gtuewrzzs.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/gsznnafxy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.yfazqb.com/Article/details/gweudpdur.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gfpwfwjul.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdtrrtqi.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/ggevwrwbu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.bbcook.cn/Article/details/gotbaapth.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/gannsgjyp.sHtML

fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gzbftrczx.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyletdcb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gorqblleb.sHtML

[S13] C：宏定义
来源：http://www.share.vehdjk.com/Article/details/gfviyazja.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.vehdjk.com/Article/details/gxftzkkhf.sHtML

[S14] C：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gqgcffkev.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.epnwcf.com/Article/details/gpxfowngz.sHtML

[S15] C：类型转换
来源：http://read.share.tarul.cn/Article/details/gcxnbdkux.sHtML

(double) a / b
来源：http://www.blog.yfazqb.com/Article/details/gkehvccmy.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/gsbhleetl.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/guhjvprgd.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/gxfiunlow.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.vehdjk.com/Article/details/gphdqpsuh.sHtML

[S18] C：命令行参数
来源：http://3g.yfazqb.com/Article/details/gtdibanxj.sHtML

int main(int argc, char **argv)
来源：http://www.share.fktsv.cn/Article/details/gixrqzpsy.sHtML

[S19] C：快速排序
来源：http://baike.epnwcf.com/Article/details/gbnckgfqw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gdhqrwlxy.sHtML

[S20] C：二分查找
来源：http://read.share.epnwcf.com/Article/details/gplyvolda.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/guurhoodn.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gfoklwmjh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fktsv.cn/Article/details/gymbbdxcw.sHtML

[S22] C：字符串转数字
来源：http://baike.bbcook.cn/Article/details/gteqvqabd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.epnwcf.com/Article/details/grjhwveop.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/gedrrefcg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.yfazqb.com/Article/details/gpkgbmugb.sHtML

[S24] C：获取本地时间
来源：http://m.share.tarul.cn/Article/details/goyjlyihc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.epnwcf.com/Article/details/ggzmtirvn.sHtML

[S25] C：内存拷贝
来源：http://3g.tarul.cn/Article/details/grxreanbw.sHtML

memcpy(dst, src, n);
来源：http://mobile.bbcook.cn/Article/details/gzwvwlwnc.sHtML

[S26] C：内存清零
来源：http://mobile.yfazqb.com/Article/details/gnudzwily.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/glggcrcwn.sHtML

[S27] C：定义常量
来源：http://www.m.share.vehdjk.com/Article/details/gbrynemhx.sHtML

const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/glcpwagdp.sHtML

[S28] C：静态变量
来源：http://blog.vehdjk.com/Article/details/ggsimeris.sHtML

static int counter = 0;
来源：http://baike.fktsv.cn/Article/details/gbmzhabye.sHtML

[S29] C：变参函数
来源：http://www.share.yfazqb.com/Article/details/gkqqqqdvn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.sjlbkw.cn/Article/details/gywxelryf.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/gjbffotaj.sHtML

#ifndef X_H
来源：http://baike.yfazqb.com/Article/details/gbjcmbmde.sHtML

#define X_H
来源：http://wap.tarul.cn/Article/details/gyiuvbjrm.sHtML

#endif
来源：http://mobile.vehdjk.com/Article/details/gftvgjsfh.sHtML

[S31] C++：Hello World
来源：http://blog.fktsv.cn/Article/details/gbeeslqln.sHtML

#include <iostream>
来源：http://m.share.tarul.cn/Article/details/gkrsxoyap.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fktsv.cn/Article/details/glknxksla.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/ghhyxyupt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.tarul.cn/Article/details/galcuraqy.sHtML

[S33] C++：vector 增删
来源：http://www.share.yfazqb.com/Article/details/glqzhoucu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gkxmjmaki.sHtML

[S34] C++：遍历 vector
来源：http://baike.bbcook.cn/Article/details/gmityxcuw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.vehdjk.com/Article/details/gexoqrrgd.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/gcincocpe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gyurfjwzk.sHtML

[S36] C++：unordered_map
来源：http://www.share.fktsv.cn/Article/details/gwkprycyr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/ggumqdfdi.sHtML

[S37] C++：set
来源：http://blog.vehdjk.com/Article/details/gybfhfuea.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.yfazqb.com/Article/details/gbjofacgt.sHtML

[S38] C++：排序
来源：http://3g.tarul.cn/Article/details/gkxqmgitu.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fktsv.cn/Article/details/gomknmbvs.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fktsv.cn/Article/details/gdrnbmeqx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.tarul.cn/Article/details/gqzujzflp.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/gllfoobfd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.yfazqb.com/Article/details/gufwkksjq.sHtML

[S41] C++：类与构造函数
来源：http://wap.fktsv.cn/Article/details/gfnxtyyjd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.sjlbkw.cn/Article/details/gtzmrpiqb.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.yfazqb.com/Article/details/gyyvtvaea.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fktsv.cn/Article/details/ghacsjntl.sHtML

[S43] C++：智能指针
来源：http://www.blog.bbcook.cn/Article/details/gowztgfae.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gqonillra.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gksbixgbr.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fktsv.cn/Article/details/gmipfoann.sHtML

[S45] C++：lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwcotvrv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fktsv.cn/Article/details/gjthjjwkv.sHtML

[S46] C++：函数模板
来源：http://read.share.bbcook.cn/Article/details/gzelpyslm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gamdpjuig.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.epnwcf.com/Article/details/gmhptvisc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.tarul.cn/Article/details/gfhhmrion.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/goxqmzssr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.epnwcf.com/Article/details/gprlimopx.sHtML

while (std::getline(in, line)) { }
来源：http://baike.tarul.cn/Article/details/gtwkjedvd.sHtML

[S49] C++：写文件
来源：http://blog.epnwcf.com/Article/details/gbjxvkgxv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.yfazqb.com/Article/details/goajthlmj.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/guimjggcz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gfkfcmsrw.sHtML

[S51] C++：显式类型转换
来源：http://mobile.bbcook.cn/Article/details/gidqakpna.sHtML

static_cast<double>(a) / b
来源：http://3g.sjlbkw.cn/Article/details/grenuzdkd.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.yfazqb.com/Article/details/grxdtewlh.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.bbcook.cn/Article/details/gvezqfpiz.sHtML

[S53] C++：移动语义
来源：http://blog.tarul.cn/Article/details/ghlhbzyhd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.vehdjk.com/Article/details/ghthtkxdv.sHtML

[S54] C++：异常处理
来源：http://mobile.tarul.cn/Article/details/gsbfvrcnk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.yfazqb.com/Article/details/gxerqzrus.sHtML

[S55] C++：结构化绑定
来源：http://3g.fktsv.cn/Article/details/gadvgblvw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.vehdjk.com/Article/details/gdikbhpic.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/gcxbifwvk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.tarul.cn/Article/details/gkbhcyhlh.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gineskfmc.sHtML

constexpr int N = 10;
来源：http://read.share.fktsv.cn/Article/details/gaoobptlu.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gzbhiykeo.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/grkqnxyqu.sHtML

[S59] C++：静态断言
来源：http://m.share.yfazqb.com/Article/details/guujawocn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.yfazqb.com/Article/details/gzfilujfy.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.sjlbkw.cn/Article/details/gkfpunbca.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fktsv.cn/Article/details/gkuuixqlg.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/glukjlqhm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.vehdjk.com/Article/details/grhvzmmph.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glryblise.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/goadbayll.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/glwkgromh.sHtML

[T02] Kotlin：变量
来源：http://mobile.epnwcf.com/Article/details/ghnxestae.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.yfazqb.com/Article/details/gtfifhijh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/gvizkutft.sHtML

"值: $b"
来源：http://m.share.bbcook.cn/Article/details/gdimcdaxr.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fktsv.cn/Article/details/gnckfqjrf.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.yfazqb.com/Article/details/geajsanwi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.epnwcf.com/Article/details/ghcsbrqjw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.sjlbkw.cn/Article/details/gpwcmygqh.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gnxxhfhmv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.yfazqb.com/Article/details/gxqnrzhzd.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/ghqchsssd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.yfazqb.com/Article/details/gqtggbwdo.sHtML

[T08] Kotlin：数据类
来源：http://3g.tarul.cn/Article/details/gwbsljpho.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.vehdjk.com/Article/details/gzqqhcxyj.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.vehdjk.com/Article/details/grvcvczxz.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.yfazqb.com/Article/details/gmdgevcay.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.tarul.cn/Article/details/gbcmzncfv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.epnwcf.com/Article/details/gmzgogyxn.sHtML

[T11] Kotlin：协程
来源：http://www.blog.epnwcf.com/Article/details/gbnwiflhb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.bbcook.cn/Article/details/gmqjddigk.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fktsv.cn/Article/details/gctntpwyw.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gbxlrbndo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.tarul.cn/Article/details/gbqsnjrda.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.yfazqb.com/Article/details/gzlgbnhjz.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gwkhemjrn.sHtML

for (i in 1..10) println(i)
来源：http://www.share.yfazqb.com/Article/details/goaxtrxub.sHtML

[T15] Kotlin：接口
来源：http://m.share.vehdjk.com/Article/details/gteeyzqcm.sHtML

interface Shape { fun area(): Double }
来源：http://baike.vehdjk.com/Article/details/gbpkqerjx.sHtML

[T16] Swift：Hello World
来源：http://3g.epnwcf.com/Article/details/gqababjqg.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/glvczmcbk.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fktsv.cn/Article/details/gzpgeubfh.sHtML

var a = 1;  let b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gjyjxqsqe.sHtML

[T18] Swift：字符串插值
来源：http://mobile.bbcook.cn/Article/details/ggjnwwznq.sHtML

"值: \(b)"
来源：http://read.share.tarul.cn/Article/details/gnjbhuxav.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/grwecsvym.sHtML

if let n = opt { print(n) }
来源：http://mobile.fktsv.cn/Article/details/ghmsgtpgr.sHtML

[T20] Swift：数组操作
来源：http://www.blog.vehdjk.com/Article/details/glxcmjavr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.bbcook.cn/Article/details/gyqjrqktb.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/gsehxgfup.sHtML

for x in a { print(x) }
来源：http://www.blog.fktsv.cn/Article/details/gietvhzwg.sHtML

[T22] Swift：字典
来源：http://baike.vehdjk.com/Article/details/gibtmkqwx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.epnwcf.com/Article/details/gibpkvqid.sHtML

[T23] Swift：函数
来源：http://mobile.sjlbkw.cn/Article/details/gufiwiyut.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.bbcook.cn/Article/details/gyelxwbfc.sHtML

[T24] Swift：闭包
来源：http://3g.vehdjk.com/Article/details/gjaxvjfyl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.tarul.cn/Article/details/gcefmyzfg.sHtML

[T25] Swift：结构体
来源：http://www.share.epnwcf.com/Article/details/gpfdqftcm.sHtML

struct P { var x: Int }
来源：http://wap.vehdjk.com/Article/details/grvgfovlp.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/gjwhgtuov.sHtML

class A: Base { override func f() {} }
来源：http://blog.sjlbkw.cn/Article/details/gweuphnui.sHtML

[T27] Swift：错误处理
来源：http://baike.sjlbkw.cn/Article/details/glbtaohwb.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwotqnwm.sHtML

[T28] Swift：枚举
来源：http://wap.yfazqb.com/Article/details/giqvywdzn.sHtML

enum Color { case red, green }
来源：http://baike.epnwcf.com/Article/details/gpbcjnbyo.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.tarul.cn/Article/details/gmrtowdul.sHtML

guard let x = opt else { return }
来源：http://www.m.share.vehdjk.com/Article/details/gvirmhnjb.sHtML

[T30] Swift：协议
来源：http://blog.yfazqb.com/Article/details/gmvcokoat.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/gyabmwbih.sHtML

[T31] Lua：Hello World
来源：http://read.share.epnwcf.com/Article/details/gsrokqnht.sHtML

print("Hello")
来源：http://m.share.epnwcf.com/Article/details/gwsjefeps.sHtML

[T32] Lua：局部变量
来源：http://mobile.bbcook.cn/Article/details/gvvyautar.sHtML

local a = 1
来源：http://mobile.yfazqb.com/Article/details/gvrpplbzv.sHtML

[T33] Lua：表（数组）
来源：http://www.share.bbcook.cn/Article/details/gnntfnspf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.bbcook.cn/Article/details/gmrtxkncg.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.epnwcf.com/Article/details/gimbetsxe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fktsv.cn/Article/details/gadzxfjam.sHtML

[T35] Lua：字典表
来源：http://mobile.epnwcf.com/Article/details/ghchrfzkz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.epnwcf.com/Article/details/grjxdtrpy.sHtML

[T36] Lua：函数
来源：http://wap.yfazqb.com/Article/details/gsptenchg.sHtML

function add(a, b) return a + b end
来源：http://wap.yfazqb.com/Article/details/gshkboxca.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/gwveeevvp.sHtML

"a" .. "b"
来源：http://baike.vehdjk.com/Article/details/gzrjwlupv.sHtML

[T38] Lua：条件
来源：http://baike.sjlbkw.cn/Article/details/gnwxkalep.sHtML

if x > 0 then print("正") end
来源：http://www.share.sjlbkw.cn/Article/details/gimjwldve.sHtML

[T39] Lua：模式匹配
来源：http://blog.tarul.cn/Article/details/gyazhlzuo.sHtML

string.find(s, "%d+")
来源：http://read.share.tarul.cn/Article/details/gdumgtfcq.sHtML

[T40] Lua：元表
来源：http://www.m.share.epnwcf.com/Article/details/gzmvbttwo.sHtML

setmetatable({}, { __index = base })
来源：http://wap.tarul.cn/Article/details/gecysawlz.sHtML

[T41] Perl：Hello World
来源：http://www.share.yfazqb.com/Article/details/gymywhqmj.sHtML

print "Hello\n";
来源：http://baike.yfazqb.com/Article/details/gggwfxboe.sHtML

[T42] Perl：变量类型
来源：http://m.share.vehdjk.com/Article/details/gvatowyfo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.bbcook.cn/Article/details/gauczrfzx.sHtML

[T43] Perl：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gsifrxwqu.sHtML

"值: $a"
来源：http://read.share.epnwcf.com/Article/details/globqvgvx.sHtML

[T44] Perl：条件
来源：http://read.share.yfazqb.com/Article/details/gjtbgwtwy.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.epnwcf.com/Article/details/gjhkjpuqy.sHtML

[T45] Perl：数组遍历
来源：http://www.share.vehdjk.com/Article/details/gupddfsii.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fktsv.cn/Article/details/ghjsdxfld.sHtML

[T46] Perl：哈希操作
来源：http://wap.bbcook.cn/Article/details/gxequgjtq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.bbcook.cn/Article/details/gpidhbizg.sHtML

[T47] Perl：正则捕获
来源：http://www.share.vehdjk.com/Article/details/gjdtgqchg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fktsv.cn/Article/details/gkzpyysod.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/gtajjlcmx.sHtML

$s =~ s/old/new/g;
来源：http://mobile.tarul.cn/Article/details/goaaoxqos.sHtML

[T49] Perl：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/girclctes.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gptfvsyui.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gzyfxknaj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.tarul.cn/Article/details/gqinxqnzt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.bbcook.cn/Article/details/gmayjdppf.sHtML

[T51] Scala：Hello World
来源：http://wap.fktsv.cn/Article/details/gdxwzahzh.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gswqbxsfm.sHtML

[T52] Scala：变量
来源：http://www.share.fktsv.cn/Article/details/gqummppat.sHtML

val a = 1;  var b = 2
来源：http://3g.yfazqb.com/Article/details/gdhficath.sHtML

[T53] Scala：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gjtgafefz.sHtML

s"值: $b"
来源：http://m.share.yfazqb.com/Article/details/gxemybswo.sHtML

[T54] Scala：集合映射
来源：http://mobile.yfazqb.com/Article/details/gdcjlkhtj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.epnwcf.com/Article/details/gmnboscou.sHtML

[T55] Scala：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/ggtaxvgyl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.epnwcf.com/Article/details/gxobucaok.sHtML

[T56] Scala：样例类
来源：http://wap.epnwcf.com/Article/details/gwwshzijs.sHtML

case class User(name: String, age: Int)
来源：http://mobile.epnwcf.com/Article/details/gynujgjax.sHtML

[T57] Scala：模式匹配
来源：http://blog.bbcook.cn/Article/details/gtabikkrk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fktsv.cn/Article/details/gxikjhevl.sHtML

[T58] Scala：函数定义
来源：http://mobile.bbcook.cn/Article/details/gmugyzaxj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgbubfou.sHtML

[T59] Scala：循环
来源：http://www.m.share.vehdjk.com/Article/details/gsqfuxbim.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gzmnsddfm.sHtML

[T60] Scala：折叠
来源：http://www.share.sjlbkw.cn/Article/details/gjabhjony.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fktsv.cn/Article/details/gjckhbyzi.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gpvrdkqqt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.epnwcf.com/Article/details/gxerpqieo.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/guxnzjxox.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.yfazqb.com/Article/details/groubncnx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.vehdjk.com/Article/details/gdlrymrux.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.bbcook.cn/Article/details/gvlvuwcfh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gknevcveo.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/gbsxczwch.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.tarul.cn/Article/details/gfyhxdyzf.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.tarul.cn/Article/details/gwfcipeyb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/guqpjjacv.sHtML

[U05] Py：列表去重且保序
来源：http://blog.bbcook.cn/Article/details/gszskkias.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/geucklrdf.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.tarul.cn/Article/details/gqxcnnvlj.sHtML

{**a, **b}
来源：http://www.blog.bbcook.cn/Article/details/gbbqqfaza.sHtML

[U07] Py：反转字典键值
来源：http://baike.tarul.cn/Article/details/grbwftlxk.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.tarul.cn/Article/details/gbvdymsna.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.vehdjk.com/Article/details/gexsykoni.sHtML

[y for x in nested for y in x]
来源：http://3g.yfazqb.com/Article/details/glyncjucc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.bbcook.cn/Article/details/gmlocmrss.sHtML

max(d, key=d.get)
来源：http://3g.epnwcf.com/Article/details/guyzcnedk.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/gbvykygcu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fktsv.cn/Article/details/gmeglezeh.sHtML

[U11] Py：生成器表达式
来源：http://wap.sjlbkw.cn/Article/details/gpozwiwfa.sHtML

(x * 2 for x in arr)
来源：http://www.blog.vehdjk.com/Article/details/gxzksicwc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.yfazqb.com/Article/details/gvmaeonbe.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fktsv.cn/Article/details/gidhezhtj.sHtML

[U13] Py：固定长度队列
来源：http://mobile.bbcook.cn/Article/details/gdquosxcu.sHtML

deque(maxlen=10)
来源：http://www.m.share.tarul.cn/Article/details/guxwdmags.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/guveqmklt.sHtML

defaultdict(list)
来源：http://www.m.share.fktsv.cn/Article/details/gkwlzukqw.sHtML


<!-- 参考信息 -->