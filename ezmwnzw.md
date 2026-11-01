代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://wap.yfazqb.com/Article/details/gwcorxldw.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/gudzrvtit.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fktsv.cn/Article/details/gmifbgugv.sHtML

[R71] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gxlpdzybn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.epnwcf.com/Article/details/gwgbmztfa.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.epnwcf.com/Article/details/gxhfsxcma.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gggenrbly.sHtML

[R73] 分割大日志
来源：http://mobile.tarul.cn/Article/details/gsaklygzm.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/gropmmgvc.sHtML

[R74] 批量重命名
来源：http://www.blog.sjlbkw.cn/Article/details/gagmgwdmh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.sjlbkw.cn/Article/details/ghbmrfarn.sHtML

[R75] 导出环境变量
来源：http://m.share.epnwcf.com/Article/details/ggnqqwohu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.bbcook.cn/Article/details/gqemhvqjf.sHtML

[R76] 使用临时文件
来源：http://read.share.fktsv.cn/Article/details/gkjomsrai.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gxmugrysf.sHtML

[R77] 读取用户输入
来源：http://baike.tarul.cn/Article/details/gmonozeta.sHtML

read -rp "请输入: " ans
来源：http://www.blog.sjlbkw.cn/Article/details/ghjovcwoq.sHtML

[R78] 交互式菜单
来源：http://wap.bbcook.cn/Article/details/gmzntbrtl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.vehdjk.com/Article/details/gslqkoobe.sHtML

[R79] 解析命令行选项
来源：http://m.share.vehdjk.com/Article/details/gyztinvyv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fktsv.cn/Article/details/gcveadbdj.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.sjlbkw.cn/Article/details/ggwzmrcuv.sHtML

time ./run.sh
来源：http://www.blog.yfazqb.com/Article/details/grttjjauf.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gkolgwbwm.sHtML

S. C / C++ 专题
来源：http://www.blog.bbcook.cn/Article/details/gnbjfmqke.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzcnlhqnu.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/grudbzqet.sHtML

#include <stdio.h>
来源：http://www.blog.epnwcf.com/Article/details/gllivdbkt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.epnwcf.com/Article/details/gfhpbxqel.sHtML

[S02] C：变量与格式化输出
来源：http://3g.tarul.cn/Article/details/gwwfsiqur.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.sjlbkw.cn/Article/details/gwbtjgene.sHtML

[S03] C：读入整数
来源：http://mobile.bbcook.cn/Article/details/gbgybbwkm.sHtML

int x; scanf("%d", &x);
来源：http://baike.tarul.cn/Article/details/gqisgiqjk.sHtML

[S04] C：字符串复制
来源：http://read.share.tarul.cn/Article/details/gfhyimygu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.epnwcf.com/Article/details/ggspgmqwd.sHtML

[S05] C：字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gkcfvlyau.sHtML

strlen(s)
来源：http://m.share.yfazqb.com/Article/details/gocbyxiuw.sHtML

[S06] C：字符串比较
来源：http://read.share.vehdjk.com/Article/details/gbbylprxw.sHtML

strcmp(a, b) == 0
来源：http://www.blog.tarul.cn/Article/details/gxrhaeedd.sHtML

[S07] C：数组遍历求和
来源：http://mobile.bbcook.cn/Article/details/gdundkqvj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.yfazqb.com/Article/details/ghtglzkqe.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fktsv.cn/Article/details/ggbzcdtdv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.sjlbkw.cn/Article/details/gwtshvzmk.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.vehdjk.com/Article/details/gqkfpbpec.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.yfazqb.com/Article/details/gpgfozbdq.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.tarul.cn/Article/details/gjfbgrazo.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fktsv.cn/Article/details/gqedpmpuo.sHtML

[S11] C：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gurjzzsvj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.yfazqb.com/Article/details/gxfbqvtjd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fktsv.cn/Article/details/guhvcildq.sHtML

fclose(f);
来源：http://blog.bbcook.cn/Article/details/gslwiknpk.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/gabsbeiwv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.bbcook.cn/Article/details/gfekxyadq.sHtML

[S13] C：宏定义
来源：http://baike.vehdjk.com/Article/details/gyjbxwtse.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.sjlbkw.cn/Article/details/gdmtgtgws.sHtML

[S14] C：枚举
来源：http://blog.epnwcf.com/Article/details/gdhklvemg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.bbcook.cn/Article/details/gnmklnjel.sHtML

[S15] C：类型转换
来源：http://read.share.fktsv.cn/Article/details/gtmbzvgnc.sHtML

(double) a / b
来源：http://www.share.vehdjk.com/Article/details/gfclcbqem.sHtML

[S16] C：位操作置位
来源：http://m.share.fktsv.cn/Article/details/gvppmrgpg.sHtML

x |= (1 << 3);
来源：http://mobile.sjlbkw.cn/Article/details/gslbcsfbd.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gjwrjpaas.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.epnwcf.com/Article/details/gssrxoaht.sHtML

[S18] C：命令行参数
来源：http://3g.vehdjk.com/Article/details/gwczpmash.sHtML

int main(int argc, char **argv)
来源：http://read.share.yfazqb.com/Article/details/gwkhzwhqn.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/gukjnsrol.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/gqxfbbneo.sHtML

[S20] C：二分查找
来源：http://www.share.epnwcf.com/Article/details/gjptnvwjk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gskfbhofc.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.vehdjk.com/Article/details/gtfpbgfoj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.vehdjk.com/Article/details/gfnqtphmp.sHtML

[S22] C：字符串转数字
来源：http://baike.vehdjk.com/Article/details/gfvexdkan.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.yfazqb.com/Article/details/gbikgadrc.sHtML

[S23] C：随机数
来源：http://baike.bbcook.cn/Article/details/gayezxxot.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.bbcook.cn/Article/details/gailsckuy.sHtML

[S24] C：获取本地时间
来源：http://blog.yfazqb.com/Article/details/gmsfpcgqz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.yfazqb.com/Article/details/gatfbcdpz.sHtML

[S25] C：内存拷贝
来源：http://baike.fktsv.cn/Article/details/gfzqygqsg.sHtML

memcpy(dst, src, n);
来源：http://3g.fktsv.cn/Article/details/gbfvmuuwx.sHtML

[S26] C：内存清零
来源：http://3g.epnwcf.com/Article/details/gnfzlgerx.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gbjzjyyvs.sHtML

[S27] C：定义常量
来源：http://baike.tarul.cn/Article/details/ghliduosf.sHtML

const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gexjuicwp.sHtML

[S28] C：静态变量
来源：http://blog.fktsv.cn/Article/details/gcykulyuf.sHtML

static int counter = 0;
来源：http://www.m.share.yfazqb.com/Article/details/gtjuvkagx.sHtML

[S29] C：变参函数
来源：http://read.share.epnwcf.com/Article/details/gnianunva.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.tarul.cn/Article/details/gvdqgbzvw.sHtML

[S30] C：头文件保护
来源：http://3g.yfazqb.com/Article/details/gxvqdrsom.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/guihrornj.sHtML

#define X_H
来源：http://read.share.sjlbkw.cn/Article/details/gisibthhe.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/gsvbqzccy.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/gswipvveg.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/gdntegkvz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.yfazqb.com/Article/details/gtqtbeiuy.sHtML

[S32] C++：字符串
来源：http://m.share.bbcook.cn/Article/details/gtuudfgqz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gmdfvedlt.sHtML

[S33] C++：vector 增删
来源：http://blog.epnwcf.com/Article/details/gvrxftahm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.epnwcf.com/Article/details/gajknbaik.sHtML

[S34] C++：遍历 vector
来源：http://blog.tarul.cn/Article/details/gnztywwsi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.tarul.cn/Article/details/gbokbzair.sHtML

[S35] C++：map
来源：http://3g.bbcook.cn/Article/details/guodgtjwl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gqrnuptde.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/gvtojbogz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gpvagqzao.sHtML

[S37] C++：set
来源：http://m.share.fktsv.cn/Article/details/ghntkrbhb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gdqvrvfva.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/gyyortpaz.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gnjcxogkl.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/gjhsejnkh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.sjlbkw.cn/Article/details/gpehejloo.sHtML

[S40] C++：查找元素
来源：http://www.share.epnwcf.com/Article/details/gwrkiwyeo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.tarul.cn/Article/details/giivqlvmc.sHtML

[S41] C++：类与构造函数
来源：http://baike.epnwcf.com/Article/details/gxpnbnefc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gevafpvnf.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/glqvacovs.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fktsv.cn/Article/details/gtbllsdwe.sHtML

[S43] C++：智能指针
来源：http://www.m.share.bbcook.cn/Article/details/gfglfcste.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/gnsgikpvu.sHtML

[S44] C++：引用传参
来源：http://www.share.vehdjk.com/Article/details/gbywgekvr.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.bbcook.cn/Article/details/godrtzscc.sHtML

[S45] C++：lambda
来源：http://read.share.vehdjk.com/Article/details/gpbrtzhjn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.sjlbkw.cn/Article/details/gtnslorls.sHtML

[S46] C++：函数模板
来源：http://mobile.fktsv.cn/Article/details/gmdtgkjmn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.vehdjk.com/Article/details/gvtxdkpxv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.yfazqb.com/Article/details/gefeqsugg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.bbcook.cn/Article/details/giwlbvbwt.sHtML

[S48] C++：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gmsznjqqe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.vehdjk.com/Article/details/gmibcgvcs.sHtML

while (std::getline(in, line)) { }
来源：http://3g.vehdjk.com/Article/details/gjrhzlroz.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gjxvwmuma.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/giydswees.sHtML

[S50] C++：格式化数字
来源：http://3g.vehdjk.com/Article/details/gesgckncc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gxcdzswvy.sHtML

[S51] C++：显式类型转换
来源：http://blog.bbcook.cn/Article/details/gyapujxxv.sHtML

static_cast<double>(a) / b
来源：http://read.share.bbcook.cn/Article/details/gzdqyrspn.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.bbcook.cn/Article/details/gxyidfmvh.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/gantpujzz.sHtML

[S53] C++：移动语义
来源：http://blog.tarul.cn/Article/details/gfkqkltrh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.bbcook.cn/Article/details/gnbbxwuad.sHtML

[S54] C++：异常处理
来源：http://read.share.vehdjk.com/Article/details/gesdgfkfi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fktsv.cn/Article/details/gassonyzp.sHtML

[S55] C++：结构化绑定
来源：http://wap.yfazqb.com/Article/details/gotdtldas.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/glgtjiwis.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/gpnuobnej.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.yfazqb.com/Article/details/gtvvvhrvy.sHtML

[S57] C++：编译期常量
来源：http://wap.bbcook.cn/Article/details/gqglgvizu.sHtML

constexpr int N = 10;
来源：http://read.share.yfazqb.com/Article/details/ghkbqqrgt.sHtML

[S58] C++：命名空间
来源：http://wap.fktsv.cn/Article/details/glopfknys.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.sjlbkw.cn/Article/details/gplvrqmoi.sHtML

[S59] C++：静态断言
来源：http://3g.yfazqb.com/Article/details/gedqcfbmy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.epnwcf.com/Article/details/gpattknfg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.tarul.cn/Article/details/goehoqjpx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.tarul.cn/Article/details/ghbqtcmxu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grjrroimt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/gmpywigrz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gglzaktjs.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fktsv.cn/Article/details/geqsdodvv.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gvoihlmrc.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.epnwcf.com/Article/details/gvsxaebve.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.bbcook.cn/Article/details/gryxldavh.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.epnwcf.com/Article/details/ghwxhqobw.sHtML

"值: $b"
来源：http://3g.tarul.cn/Article/details/gcigfezvq.sHtML

[T04] Kotlin：空安全
来源：http://read.share.bbcook.cn/Article/details/glhdxgvcp.sHtML

val n: String? = null;  n?.length
来源：http://www.share.tarul.cn/Article/details/gdjhuzaxs.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.vehdjk.com/Article/details/gwsmubzyg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.tarul.cn/Article/details/gmtbfjtjp.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.epnwcf.com/Article/details/gfcypxjgq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gdobmxomb.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gnxfumydp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.yfazqb.com/Article/details/goemzfqlv.sHtML

[T08] Kotlin：数据类
来源：http://baike.sjlbkw.cn/Article/details/gmligbcic.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.yfazqb.com/Article/details/giwllalcz.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/grglaucrv.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fktsv.cn/Article/details/gatbkbsmd.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gwsuozwvy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.yfazqb.com/Article/details/ggdovbfmg.sHtML

[T11] Kotlin：协程
来源：http://read.share.epnwcf.com/Article/details/gkbvzikhp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/gcntxuqpj.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.vehdjk.com/Article/details/gsoewrmfg.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/gkdhoheww.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.sjlbkw.cn/Article/details/gosvowcne.sHtML

val m = mapOf("a" to 1)
来源：http://wap.bbcook.cn/Article/details/gfwxbdmsf.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.yfazqb.com/Article/details/grikfxyfe.sHtML

for (i in 1..10) println(i)
来源：http://mobile.vehdjk.com/Article/details/gfqledpug.sHtML

[T15] Kotlin：接口
来源：http://blog.sjlbkw.cn/Article/details/goqbpjahl.sHtML

interface Shape { fun area(): Double }
来源：http://baike.yfazqb.com/Article/details/gunkwwtuv.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gtycwduqt.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gzczbfaog.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fktsv.cn/Article/details/ggoluskmt.sHtML

var a = 1;  let b = 2
来源：http://baike.fktsv.cn/Article/details/gjvdhpmil.sHtML

[T18] Swift：字符串插值
来源：http://blog.vehdjk.com/Article/details/grxonskne.sHtML

"值: \(b)"
来源：http://blog.bbcook.cn/Article/details/guklbqfps.sHtML

[T19] Swift：可选绑定
来源：http://3g.yfazqb.com/Article/details/gnydatzwg.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fktsv.cn/Article/details/gjnjfysje.sHtML

[T20] Swift：数组操作
来源：http://www.share.fktsv.cn/Article/details/gnzppfkqg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fktsv.cn/Article/details/gvfunhlym.sHtML

[T21] Swift：遍历
来源：http://blog.tarul.cn/Article/details/gfezhdjum.sHtML

for x in a { print(x) }
来源：http://mobile.vehdjk.com/Article/details/ghicalqxe.sHtML

[T22] Swift：字典
来源：http://www.blog.sjlbkw.cn/Article/details/gkrfoibhp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gfemtcauj.sHtML

[T23] Swift：函数
来源：http://m.share.tarul.cn/Article/details/gazzwxtwd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gxheidoty.sHtML

[T24] Swift：闭包
来源：http://www.m.share.tarul.cn/Article/details/gjafbyjdw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.epnwcf.com/Article/details/gosvzjkvh.sHtML

[T25] Swift：结构体
来源：http://wap.vehdjk.com/Article/details/glbzlurpy.sHtML

struct P { var x: Int }
来源：http://www.m.share.bbcook.cn/Article/details/gxwyhegzy.sHtML

[T26] Swift：类与重写
来源：http://www.share.bbcook.cn/Article/details/glujhdtgi.sHtML

class A: Base { override func f() {} }
来源：http://wap.fktsv.cn/Article/details/gciyrxxvh.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.yfazqb.com/Article/details/geohcnirw.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/ghzajpivh.sHtML

[T28] Swift：枚举
来源：http://3g.bbcook.cn/Article/details/geyyqmecp.sHtML

enum Color { case red, green }
来源：http://www.blog.bbcook.cn/Article/details/gcorfkjxq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.bbcook.cn/Article/details/gyxlaudid.sHtML

guard let x = opt else { return }
来源：http://read.share.epnwcf.com/Article/details/gzjwglops.sHtML

[T30] Swift：协议
来源：http://read.share.fktsv.cn/Article/details/geuclvaui.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.tarul.cn/Article/details/gncywlfzy.sHtML

[T31] Lua：Hello World
来源：http://3g.epnwcf.com/Article/details/gjoxckljg.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/gvfnoimmo.sHtML

[T32] Lua：局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/gsozivlwj.sHtML

local a = 1
来源：http://3g.bbcook.cn/Article/details/genizmiql.sHtML

[T33] Lua：表（数组）
来源：http://baike.vehdjk.com/Article/details/gtiszluxs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.sjlbkw.cn/Article/details/gadqqwlaj.sHtML

[T34] Lua：遍历表
来源：http://mobile.bbcook.cn/Article/details/gojpnempr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/gbfwvmame.sHtML

[T35] Lua：字典表
来源：http://read.share.tarul.cn/Article/details/gfxmifzdp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.sjlbkw.cn/Article/details/ghhsbdwsu.sHtML

[T36] Lua：函数
来源：http://baike.yfazqb.com/Article/details/gonztukjd.sHtML

function add(a, b) return a + b end
来源：http://blog.bbcook.cn/Article/details/gswircvax.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gdgwzxqmt.sHtML

"a" .. "b"
来源：http://blog.epnwcf.com/Article/details/gswvsjmxe.sHtML

[T38] Lua：条件
来源：http://read.share.tarul.cn/Article/details/gxpvydqed.sHtML

if x > 0 then print("正") end
来源：http://mobile.vehdjk.com/Article/details/gwjugqhtf.sHtML

[T39] Lua：模式匹配
来源：http://m.share.epnwcf.com/Article/details/gjylmxvpj.sHtML

string.find(s, "%d+")
来源：http://blog.yfazqb.com/Article/details/gprztkbfo.sHtML

[T40] Lua：元表
来源：http://www.m.share.yfazqb.com/Article/details/gsbesyfnu.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.yfazqb.com/Article/details/gwkifvlbn.sHtML

[T41] Perl：Hello World
来源：http://read.share.yfazqb.com/Article/details/gsljrnuic.sHtML

print "Hello\n";
来源：http://blog.vehdjk.com/Article/details/gxkxaveid.sHtML

[T42] Perl：变量类型
来源：http://mobile.bbcook.cn/Article/details/glisiycga.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.sjlbkw.cn/Article/details/gwpvedolj.sHtML

[T43] Perl：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gresxxoeb.sHtML

"值: $a"
来源：http://mobile.tarul.cn/Article/details/gylcowtok.sHtML

[T44] Perl：条件
来源：http://read.share.tarul.cn/Article/details/gjnqsdgpt.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fktsv.cn/Article/details/gzxgsuqea.sHtML

[T45] Perl：数组遍历
来源：http://read.share.yfazqb.com/Article/details/gtuthunzs.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.vehdjk.com/Article/details/gicijlexx.sHtML

[T46] Perl：哈希操作
来源：http://read.share.sjlbkw.cn/Article/details/gbadvjesl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.vehdjk.com/Article/details/gtyvqfbpj.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fktsv.cn/Article/details/ghesrgvow.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.vehdjk.com/Article/details/gdhpyyksn.sHtML

[T48] Perl：正则替换
来源：http://www.blog.epnwcf.com/Article/details/gjqsqprid.sHtML

$s =~ s/old/new/g;
来源：http://m.share.yfazqb.com/Article/details/gpjmfmfat.sHtML

[T49] Perl：函数
来源：http://www.share.sjlbkw.cn/Article/details/gmywkvqhj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gamtxwzlr.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gmnzgtnyq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.sjlbkw.cn/Article/details/gaqvladdw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.epnwcf.com/Article/details/gflhecajl.sHtML

[T51] Scala：Hello World
来源：http://www.share.yfazqb.com/Article/details/gahqaokvv.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gxhntxqkq.sHtML

[T52] Scala：变量
来源：http://m.share.yfazqb.com/Article/details/gjdnjrgbm.sHtML

val a = 1;  var b = 2
来源：http://3g.epnwcf.com/Article/details/gwqkqgzkz.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gejgmnowp.sHtML

s"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gpritdlpf.sHtML

[T54] Scala：集合映射
来源：http://mobile.tarul.cn/Article/details/gjsqatxxv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.vehdjk.com/Article/details/gyezuuhel.sHtML

[T55] Scala：集合过滤
来源：http://blog.bbcook.cn/Article/details/ghpxcbpti.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fktsv.cn/Article/details/gmlgwihxk.sHtML

[T56] Scala：样例类
来源：http://www.share.vehdjk.com/Article/details/gdubbzqys.sHtML

case class User(name: String, age: Int)
来源：http://read.share.vehdjk.com/Article/details/goxlzvihj.sHtML

[T57] Scala：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gvpjfrsee.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.epnwcf.com/Article/details/gatdlmnfs.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.sjlbkw.cn/Article/details/glpiwiisi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fktsv.cn/Article/details/gctvzfvdg.sHtML

[T59] Scala：循环
来源：http://mobile.bbcook.cn/Article/details/gglczvzgw.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gtodtvcyq.sHtML

[T60] Scala：折叠
来源：http://read.share.vehdjk.com/Article/details/gloxgtdda.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.vehdjk.com/Article/details/gaqxdeght.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grznoljcj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.epnwcf.com/Article/details/gatigoifp.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggcefkugq.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.vehdjk.com/Article/details/gunzlwrdb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fktsv.cn/Article/details/gorjntqdv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.tarul.cn/Article/details/ghruqywgp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.bbcook.cn/Article/details/gaaalftxz.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.epnwcf.com/Article/details/gbbezixad.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.epnwcf.com/Article/details/grqvuivmi.sHtML

[U04] Py：变量调试打印
来源：http://baike.yfazqb.com/Article/details/gzjxqbpoa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.vehdjk.com/Article/details/gfaivnxab.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.vehdjk.com/Article/details/guhuskdhw.sHtML

list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/ghruiqhsw.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.epnwcf.com/Article/details/gywwoucyh.sHtML

{**a, **b}
来源：http://read.share.fktsv.cn/Article/details/godgnylsy.sHtML

[U07] Py：反转字典键值
来源：http://3g.epnwcf.com/Article/details/ginocojif.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.vehdjk.com/Article/details/gzkkemrqy.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.tarul.cn/Article/details/ghlzelisj.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/gcupcmjev.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.sjlbkw.cn/Article/details/gmoixvbmc.sHtML

max(d, key=d.get)
来源：http://m.share.yfazqb.com/Article/details/gzagwbygj.sHtML

[U10] Py：按值排序字典
来源：http://www.share.tarul.cn/Article/details/gnelzbqrx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.sjlbkw.cn/Article/details/gvguvwiwh.sHtML


<!-- 参考信息 -->