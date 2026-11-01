代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.sjlbkw.cn/Article/details/grzucpixh.sHtML

[R72] 等待端口就绪
来源：http://mobile.fktsv.cn/Article/details/gtqysvylr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gwgfjuldv.sHtML

[R73] 分割大日志
来源：http://read.share.yfazqb.com/Article/details/gbngaunmn.sHtML

split -l 1000 big.log part_
来源：http://3g.bbcook.cn/Article/details/gtumcuscf.sHtML

[R74] 批量重命名
来源：http://m.share.fktsv.cn/Article/details/gbeblzhor.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/gokvixwwq.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/gcxnzlshr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fktsv.cn/Article/details/gfwndekbh.sHtML

[R76] 使用临时文件
来源：http://m.share.tarul.cn/Article/details/gmsvyrnac.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gstbxoxxy.sHtML

[R77] 读取用户输入
来源：http://wap.tarul.cn/Article/details/gbluoklxp.sHtML

read -rp "请输入: " ans
来源：http://read.share.fktsv.cn/Article/details/gqtvasexz.sHtML

[R78] 交互式菜单
来源：http://www.share.sjlbkw.cn/Article/details/guwdmirfv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.sjlbkw.cn/Article/details/gumvloqse.sHtML

[R79] 解析命令行选项
来源：http://www.blog.yfazqb.com/Article/details/glqakrhln.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.bbcook.cn/Article/details/ggjsbqivx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fktsv.cn/Article/details/ghqssogfu.sHtML

time ./run.sh
来源：http://wap.epnwcf.com/Article/details/gioxagrdo.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpkyjwtxl.sHtML

S. C / C++ 专题
来源：http://www.share.fktsv.cn/Article/details/grlodqhwu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbzdlcahd.sHtML

[S01] C：Hello World
来源：http://baike.vehdjk.com/Article/details/gblzzbsnz.sHtML

#include <stdio.h>
来源：http://3g.epnwcf.com/Article/details/gtscedyvt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.bbcook.cn/Article/details/ghdpintob.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/gdyrpksvq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fktsv.cn/Article/details/gdkcuockt.sHtML

[S03] C：读入整数
来源：http://m.share.yfazqb.com/Article/details/gypmdbacs.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/gbpdixvqh.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/gehmzcejk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/gyddvfhgo.sHtML

[S05] C：字符串长度
来源：http://read.share.vehdjk.com/Article/details/gnhjntldf.sHtML

strlen(s)
来源：http://read.share.bbcook.cn/Article/details/gzokcrhyh.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdzhmlyy.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/gyewylaoo.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.epnwcf.com/Article/details/gtibrezpc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.epnwcf.com/Article/details/gavxmdqra.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.tarul.cn/Article/details/gfvozlfpo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.bbcook.cn/Article/details/gnajwkuyp.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.bbcook.cn/Article/details/guzbtxlej.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.bbcook.cn/Article/details/gytlvfkjc.sHtML

[S10] C：指针与解引用
来源：http://wap.epnwcf.com/Article/details/gwfmwvmai.sHtML

int *p = &a;  *p = 5;
来源：http://baike.tarul.cn/Article/details/gtuyrvpop.sHtML

[S11] C：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gusyemfct.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.bbcook.cn/Article/details/gnpcyhjrj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.epnwcf.com/Article/details/ghrdezoci.sHtML

fclose(f);
来源：http://mobile.vehdjk.com/Article/details/grctxuach.sHtML

[S12] C：写文件
来源：http://mobile.fktsv.cn/Article/details/gewnngvkl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.vehdjk.com/Article/details/geyllqxob.sHtML

[S13] C：宏定义
来源：http://3g.yfazqb.com/Article/details/gvtklkvkv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.vehdjk.com/Article/details/gphemsssz.sHtML

[S14] C：枚举
来源：http://baike.tarul.cn/Article/details/gspukthhp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.bbcook.cn/Article/details/gkoqbemkl.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/gfozviqnj.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/gmdsncezf.sHtML

[S16] C：位操作置位
来源：http://mobile.tarul.cn/Article/details/gcvkjhumg.sHtML

x |= (1 << 3);
来源：http://3g.fktsv.cn/Article/details/grctqiyaj.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gpohcucnn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.epnwcf.com/Article/details/gykfmydyp.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/gbavlodvc.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.tarul.cn/Article/details/gfismukhn.sHtML

[S19] C：快速排序
来源：http://m.share.vehdjk.com/Article/details/gaprlbdiy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gwniueocf.sHtML

[S20] C：二分查找
来源：http://blog.vehdjk.com/Article/details/gcjonfwwg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gbpnoyqbv.sHtML

[S21] C：字符类别判断
来源：http://www.share.fktsv.cn/Article/details/gfnmzkoul.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/gilclepub.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/ggdadyxyi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.tarul.cn/Article/details/govnncmhs.sHtML

[S23] C：随机数
来源：http://www.share.vehdjk.com/Article/details/gtnruxbdo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.yfazqb.com/Article/details/gpwbrhmhz.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/gimxlkowv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/gspfjfydb.sHtML

[S25] C：内存拷贝
来源：http://mobile.yfazqb.com/Article/details/gimgrozzs.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/gensrqafb.sHtML

[S26] C：内存清零
来源：http://www.blog.fktsv.cn/Article/details/gtdnrfcti.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.vehdjk.com/Article/details/guxrebfrt.sHtML

[S27] C：定义常量
来源：http://www.share.yfazqb.com/Article/details/gtdpzvlpy.sHtML

const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/glbakfymt.sHtML

[S28] C：静态变量
来源：http://read.share.fktsv.cn/Article/details/gbqpzcqda.sHtML

static int counter = 0;
来源：http://read.share.epnwcf.com/Article/details/gziidnzbu.sHtML

[S29] C：变参函数
来源：http://www.m.share.fktsv.cn/Article/details/guasxmjzp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.sjlbkw.cn/Article/details/gtqozscyf.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/gokrbrpmb.sHtML

#ifndef X_H
来源：http://www.blog.vehdjk.com/Article/details/ghldincvx.sHtML

#define X_H
来源：http://baike.bbcook.cn/Article/details/giefsegph.sHtML

#endif
来源：http://read.share.tarul.cn/Article/details/gfndefsxw.sHtML

[S31] C++：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gdghuxgil.sHtML

#include <iostream>
来源：http://www.share.tarul.cn/Article/details/glbquzbax.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.sjlbkw.cn/Article/details/giqdmkqvf.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/ghnfruswy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/gryszcxyo.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gswjnreal.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.tarul.cn/Article/details/gsvpuownd.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fktsv.cn/Article/details/gyvbmpwmn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.yfazqb.com/Article/details/gxefzncqj.sHtML

[S35] C++：map
来源：http://www.share.yfazqb.com/Article/details/gumhavzai.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gburiwktk.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/geebxlltc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/ghhkbklfd.sHtML

[S37] C++：set
来源：http://www.share.vehdjk.com/Article/details/givyjffcf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpjmrblt.sHtML

[S38] C++：排序
来源：http://baike.epnwcf.com/Article/details/ggdzozjyy.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/gpkffzmht.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.vehdjk.com/Article/details/ginozysri.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.bbcook.cn/Article/details/gxzfmmnyk.sHtML

[S40] C++：查找元素
来源：http://m.share.vehdjk.com/Article/details/goujhhfbf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.bbcook.cn/Article/details/gdfsxmkcx.sHtML

[S41] C++：类与构造函数
来源：http://wap.yfazqb.com/Article/details/gcjwoucso.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.tarul.cn/Article/details/gwerlfimp.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.epnwcf.com/Article/details/gslhyvbzd.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.tarul.cn/Article/details/giirlyeub.sHtML

[S43] C++：智能指针
来源：http://www.blog.tarul.cn/Article/details/gbcpxvwwb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.bbcook.cn/Article/details/gtapuxvdf.sHtML

[S44] C++：引用传参
来源：http://www.blog.sjlbkw.cn/Article/details/gszurwqcw.sHtML

void inc(int &x) { ++x; }
来源：http://blog.yfazqb.com/Article/details/gafvjnnza.sHtML

[S45] C++：lambda
来源：http://m.share.yfazqb.com/Article/details/gnlfovgbr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.bbcook.cn/Article/details/glbgvfnoj.sHtML

[S46] C++：函数模板
来源：http://mobile.fktsv.cn/Article/details/gistdouuf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.epnwcf.com/Article/details/gnsnbzzvd.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.vehdjk.com/Article/details/gchtmpwwu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.vehdjk.com/Article/details/gtahbwfjt.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gdjzdbmvr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/gyilbmxiv.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gameiaadl.sHtML

[S49] C++：写文件
来源：http://www.blog.tarul.cn/Article/details/gtrqusjim.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.epnwcf.com/Article/details/gsfdbqahh.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gitkwtmxw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gpguwvgsl.sHtML

[S51] C++：显式类型转换
来源：http://3g.vehdjk.com/Article/details/gvjtztpas.sHtML

static_cast<double>(a) / b
来源：http://www.blog.tarul.cn/Article/details/gisqnprpn.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.yfazqb.com/Article/details/gkbutkttj.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.tarul.cn/Article/details/gyazsmptc.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/gexvxwkau.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.vehdjk.com/Article/details/gmretnezf.sHtML

[S54] C++：异常处理
来源：http://www.m.share.bbcook.cn/Article/details/gsyjndcqq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.bbcook.cn/Article/details/gfrkcclrh.sHtML

[S55] C++：结构化绑定
来源：http://baike.sjlbkw.cn/Article/details/gohkphehr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/gbokqzrzs.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/gpjuyutxy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.tarul.cn/Article/details/ghvqdvjje.sHtML

[S57] C++：编译期常量
来源：http://3g.bbcook.cn/Article/details/ghvmjlhje.sHtML

constexpr int N = 10;
来源：http://blog.vehdjk.com/Article/details/gjpwzawhk.sHtML

[S58] C++：命名空间
来源：http://www.blog.epnwcf.com/Article/details/gtajulmik.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/gfwrddgxm.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/gclyudhsa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fktsv.cn/Article/details/gsnfaehii.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.yfazqb.com/Article/details/gnweuraxb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.yfazqb.com/Article/details/geppbywdg.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gikerqkhj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gpxdksadm.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gskvhcbjy.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/grydirbxa.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/gblsxejrp.sHtML

[T02] Kotlin：变量
来源：http://baike.sjlbkw.cn/Article/details/gvjmjjqmu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.epnwcf.com/Article/details/ghhvvyayi.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.vehdjk.com/Article/details/gqgppaonc.sHtML

"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/gixcurihz.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fktsv.cn/Article/details/gkcubbcpm.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.vehdjk.com/Article/details/gvveuwjuq.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.tarul.cn/Article/details/gyrrqljps.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fktsv.cn/Article/details/gfxamgifz.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fktsv.cn/Article/details/grozfcujf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gsbtmpbzx.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.tarul.cn/Article/details/gvskftwvh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.vehdjk.com/Article/details/gbllczwcv.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/gnrfravcd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gibuadooz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.tarul.cn/Article/details/gythlmzpc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.bbcook.cn/Article/details/gluoaejau.sHtML

[T10] Kotlin：默认参数
来源：http://blog.epnwcf.com/Article/details/gmianihci.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.sjlbkw.cn/Article/details/gwsgzjptk.sHtML

[T11] Kotlin：协程
来源：http://m.share.yfazqb.com/Article/details/gxtfvqsqw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.bbcook.cn/Article/details/glnqzzojn.sHtML

[T12] Kotlin：解构声明
来源：http://baike.bbcook.cn/Article/details/gceqhcajo.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.vehdjk.com/Article/details/gbobakbbe.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.yfazqb.com/Article/details/gviolslnx.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.vehdjk.com/Article/details/gfbcaudqq.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.tarul.cn/Article/details/gfwdgiyav.sHtML

for (i in 1..10) println(i)
来源：http://wap.epnwcf.com/Article/details/glkaodcfy.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcawthvm.sHtML

interface Shape { fun area(): Double }
来源：http://wap.epnwcf.com/Article/details/gzrjrebhc.sHtML

[T16] Swift：Hello World
来源：http://wap.vehdjk.com/Article/details/gjrygrsmi.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/gfykhprgk.sHtML

[T17] Swift：变量与常量
来源：http://3g.bbcook.cn/Article/details/gviakrqxg.sHtML

var a = 1;  let b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gcgftcjat.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gtwhzfkjr.sHtML

"值: \(b)"
来源：http://wap.sjlbkw.cn/Article/details/gnqweasqc.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.bbcook.cn/Article/details/gwisveocn.sHtML

if let n = opt { print(n) }
来源：http://blog.fktsv.cn/Article/details/glgssrckr.sHtML

[T20] Swift：数组操作
来源：http://mobile.fktsv.cn/Article/details/gfqtpinza.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.bbcook.cn/Article/details/gybrhdqne.sHtML

[T21] Swift：遍历
来源：http://baike.yfazqb.com/Article/details/gdtstvuik.sHtML

for x in a { print(x) }
来源：http://mobile.tarul.cn/Article/details/gtlhvfuxa.sHtML

[T22] Swift：字典
来源：http://www.blog.sjlbkw.cn/Article/details/gqgsdndot.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.bbcook.cn/Article/details/gdeszbjfc.sHtML

[T23] Swift：函数
来源：http://baike.sjlbkw.cn/Article/details/gzfvomrsm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.tarul.cn/Article/details/gofnzrcwi.sHtML

[T24] Swift：闭包
来源：http://www.blog.tarul.cn/Article/details/gvfjjthmn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzxqtwfd.sHtML

[T25] Swift：结构体
来源：http://blog.fktsv.cn/Article/details/ggpqdoktr.sHtML

struct P { var x: Int }
来源：http://read.share.sjlbkw.cn/Article/details/gmccmwguf.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/girkesspy.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.yfazqb.com/Article/details/gokuzemuh.sHtML

[T27] Swift：错误处理
来源：http://read.share.tarul.cn/Article/details/grcidcklf.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fktsv.cn/Article/details/gtyutfazr.sHtML

[T28] Swift：枚举
来源：http://www.share.tarul.cn/Article/details/gdfleoodz.sHtML

enum Color { case red, green }
来源：http://mobile.bbcook.cn/Article/details/gltzibqpj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gelzohdci.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/gmmvgttdg.sHtML

[T30] Swift：协议
来源：http://www.blog.epnwcf.com/Article/details/gwpiltlbd.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.epnwcf.com/Article/details/gpmcvtdux.sHtML

[T31] Lua：Hello World
来源：http://blog.yfazqb.com/Article/details/gundrpeks.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/gyipjysby.sHtML

[T32] Lua：局部变量
来源：http://m.share.sjlbkw.cn/Article/details/guphmkatm.sHtML

local a = 1
来源：http://3g.tarul.cn/Article/details/gmapxemxk.sHtML

[T33] Lua：表（数组）
来源：http://3g.vehdjk.com/Article/details/gvxwaohnv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fktsv.cn/Article/details/gynxgriix.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/gcqvkvswr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/gjosqmymo.sHtML

[T35] Lua：字典表
来源：http://www.share.tarul.cn/Article/details/gsqtlujji.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.epnwcf.com/Article/details/gyaoebqka.sHtML

[T36] Lua：函数
来源：http://www.share.vehdjk.com/Article/details/gucfjnwpp.sHtML

function add(a, b) return a + b end
来源：http://mobile.fktsv.cn/Article/details/gckiqsdam.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/gnimihxdn.sHtML

"a" .. "b"
来源：http://baike.fktsv.cn/Article/details/gqvyjgnwl.sHtML

[T38] Lua：条件
来源：http://baike.epnwcf.com/Article/details/guarxnppr.sHtML

if x > 0 then print("正") end
来源：http://www.blog.bbcook.cn/Article/details/gfpgcizlm.sHtML

[T39] Lua：模式匹配
来源：http://baike.tarul.cn/Article/details/ggdvewucp.sHtML

string.find(s, "%d+")
来源：http://read.share.epnwcf.com/Article/details/gkhcnxakz.sHtML

[T40] Lua：元表
来源：http://blog.yfazqb.com/Article/details/gilqodrqa.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.vehdjk.com/Article/details/gghgxzmxi.sHtML

[T41] Perl：Hello World
来源：http://3g.yfazqb.com/Article/details/gshvlmsib.sHtML

print "Hello\n";
来源：http://www.m.share.yfazqb.com/Article/details/grjomdpqz.sHtML

[T42] Perl：变量类型
来源：http://mobile.vehdjk.com/Article/details/grmexweul.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.yfazqb.com/Article/details/gwzmrttbl.sHtML

[T43] Perl：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gaqmfdjtz.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/gbfpyaxmn.sHtML

[T44] Perl：条件
来源：http://www.blog.yfazqb.com/Article/details/gyxnrhslb.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fktsv.cn/Article/details/gsvzefngy.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.epnwcf.com/Article/details/gpltboqcw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.yfazqb.com/Article/details/gepztarqs.sHtML

[T46] Perl：哈希操作
来源：http://m.share.bbcook.cn/Article/details/gsqoroswo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.epnwcf.com/Article/details/gpcimiudq.sHtML

[T47] Perl：正则捕获
来源：http://m.share.yfazqb.com/Article/details/gfoosduot.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.yfazqb.com/Article/details/gafkmsotg.sHtML

[T48] Perl：正则替换
来源：http://wap.tarul.cn/Article/details/ghzyoyaoa.sHtML

$s =~ s/old/new/g;
来源：http://3g.vehdjk.com/Article/details/gaqtslioj.sHtML

[T49] Perl：函数
来源：http://www.share.vehdjk.com/Article/details/grqhqtuny.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gzbvsosqx.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gpzsyposa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.yfazqb.com/Article/details/gtkmouzom.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.sjlbkw.cn/Article/details/gajlrhriu.sHtML

[T51] Scala：Hello World
来源：http://3g.bbcook.cn/Article/details/ggkpctemh.sHtML

println("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/grxawzrml.sHtML

[T52] Scala：变量
来源：http://blog.sjlbkw.cn/Article/details/gqgkfkoac.sHtML

val a = 1;  var b = 2
来源：http://www.blog.vehdjk.com/Article/details/gzxddurbh.sHtML

[T53] Scala：字符串插值
来源：http://3g.fktsv.cn/Article/details/ggmmtaibk.sHtML

s"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/glvfqipfk.sHtML

[T54] Scala：集合映射
来源：http://baike.sjlbkw.cn/Article/details/gmjyhstbt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gyrlkoapc.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/glwpwxrtj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.sjlbkw.cn/Article/details/gwzlmqbza.sHtML

[T56] Scala：样例类
来源：http://read.share.fktsv.cn/Article/details/gkuqmmflh.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fktsv.cn/Article/details/gdvusmsus.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gsutihmwx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.tarul.cn/Article/details/gdxjssuch.sHtML

[T58] Scala：函数定义
来源：http://www.share.epnwcf.com/Article/details/gowowfrmx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.bbcook.cn/Article/details/gqowncopz.sHtML

[T59] Scala：循环
来源：http://mobile.fktsv.cn/Article/details/guutheepq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gyspsfzkv.sHtML

[T60] Scala：折叠
来源：http://m.share.vehdjk.com/Article/details/gankkevix.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fktsv.cn/Article/details/gunbotusb.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxbqvpsqy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gcftckfam.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvsrfbgrt.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.bbcook.cn/Article/details/gqjcvjwsr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fktsv.cn/Article/details/gmxjdnjnm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.tarul.cn/Article/details/glsnbytct.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.yfazqb.com/Article/details/gsxxpnjux.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.epnwcf.com/Article/details/gvtimntqv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.yfazqb.com/Article/details/gfjbvkbdo.sHtML

[U04] Py：变量调试打印
来源：http://m.share.vehdjk.com/Article/details/gawwpshsq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.vehdjk.com/Article/details/gjntiucfb.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.vehdjk.com/Article/details/gmrkdtpbv.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gjmjulpqo.sHtML

[U06] Py：合并两个字典
来源：http://3g.sjlbkw.cn/Article/details/gybgpvjqy.sHtML

{**a, **b}
来源：http://wap.epnwcf.com/Article/details/ggxhwrsxn.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.tarul.cn/Article/details/grhwsxggt.sHtML

{v: k for k, v in d.items()}
来源：http://blog.yfazqb.com/Article/details/gfqwwwgml.sHtML

[U08] Py：展平二维列表
来源：http://m.share.tarul.cn/Article/details/gcomwureu.sHtML

[y for x in nested for y in x]
来源：http://wap.tarul.cn/Article/details/gffxqcqir.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.epnwcf.com/Article/details/gkjbyueee.sHtML

max(d, key=d.get)
来源：http://www.m.share.epnwcf.com/Article/details/gcnebhidw.sHtML

[U10] Py：按值排序字典
来源：http://baike.yfazqb.com/Article/details/gohemibnx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.yfazqb.com/Article/details/gsoefzcmw.sHtML

[U11] Py：生成器表达式
来源：http://www.share.tarul.cn/Article/details/ghbhcnymq.sHtML

(x * 2 for x in arr)
来源：http://www.blog.epnwcf.com/Article/details/gptvgsyyx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.vehdjk.com/Article/details/gvfqjamlo.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/grgpwsdae.sHtML


<!-- 参考信息 -->