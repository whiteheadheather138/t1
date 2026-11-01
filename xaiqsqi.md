代发 wailian999

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/gupvrxhrj.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/gevinmhiy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.bbcook.cn/Article/details/gkvqxrtxg.sHtML

[R75] 导出环境变量
来源：http://m.share.fktsv.cn/Article/details/gexwfbrih.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.tarul.cn/Article/details/gihanomus.sHtML

[R76] 使用临时文件
来源：http://www.share.fktsv.cn/Article/details/gpcxgrkal.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/gbdeggzgr.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gnnxununu.sHtML

read -rp "请输入: " ans
来源：http://blog.sjlbkw.cn/Article/details/gotrgkjrv.sHtML

[R78] 交互式菜单
来源：http://mobile.sjlbkw.cn/Article/details/gwnrlarxu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fktsv.cn/Article/details/giyscnjdx.sHtML

[R79] 解析命令行选项
来源：http://m.share.bbcook.cn/Article/details/gosctxpfv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.yfazqb.com/Article/details/gouohgwzy.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gxrmpbgsi.sHtML

time ./run.sh
来源：http://wap.epnwcf.com/Article/details/gxbszgmex.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbhqrnyga.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gkakrwcrk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gvnwwuosj.sHtML

[S01] C：Hello World
来源：http://wap.vehdjk.com/Article/details/gllvfnkiq.sHtML

#include <stdio.h>
来源：http://mobile.bbcook.cn/Article/details/gkiwcxjwy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fktsv.cn/Article/details/gwmzohtol.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.bbcook.cn/Article/details/gcglqryyn.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.bbcook.cn/Article/details/ggedjjymm.sHtML

[S03] C：读入整数
来源：http://blog.yfazqb.com/Article/details/gcshxmnoq.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.bbcook.cn/Article/details/gqzlmxblo.sHtML

[S04] C：字符串复制
来源：http://blog.fktsv.cn/Article/details/gekkmnnns.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/gjadtqdfi.sHtML

[S05] C：字符串长度
来源：http://m.share.epnwcf.com/Article/details/gysetsooo.sHtML

strlen(s)
来源：http://wap.yfazqb.com/Article/details/gpbudbscw.sHtML

[S06] C：字符串比较
来源：http://www.share.tarul.cn/Article/details/gxavdgepj.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/gfjyvomut.sHtML

[S07] C：数组遍历求和
来源：http://read.share.bbcook.cn/Article/details/gqdkfvkil.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.yfazqb.com/Article/details/ghvutamwr.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.bbcook.cn/Article/details/gmcizqbgw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/gvcgexleb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.bbcook.cn/Article/details/guxfcdrwp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.tarul.cn/Article/details/gloxpiqgd.sHtML

[S10] C：指针与解引用
来源：http://www.share.yfazqb.com/Article/details/gfhwemhbt.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.yfazqb.com/Article/details/ghmsqbren.sHtML

[S11] C：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gebcekzjj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.bbcook.cn/Article/details/gyxcfteqn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.yfazqb.com/Article/details/gmwbyviqj.sHtML

fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkotiwvp.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/gxnmtteva.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gvsjpfbym.sHtML

[S13] C：宏定义
来源：http://m.share.vehdjk.com/Article/details/gqsqxbjmb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/gclhtnjot.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/guloiuwrj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fktsv.cn/Article/details/ghkhklohm.sHtML

[S15] C：类型转换
来源：http://baike.bbcook.cn/Article/details/gqeppoosx.sHtML

(double) a / b
来源：http://blog.fktsv.cn/Article/details/gkuoqymby.sHtML

[S16] C：位操作置位
来源：http://www.blog.vehdjk.com/Article/details/gwybdjqfu.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/gyiqrdesy.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.tarul.cn/Article/details/gdmdcwbkn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/gmktyxyeg.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/ghircbdri.sHtML

int main(int argc, char **argv)
来源：http://3g.yfazqb.com/Article/details/grjiyekqo.sHtML

[S19] C：快速排序
来源：http://www.blog.tarul.cn/Article/details/gdwbfvgox.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gqhpkmxly.sHtML

[S20] C：二分查找
来源：http://mobile.sjlbkw.cn/Article/details/gauophruu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gpzyzistr.sHtML

[S21] C：字符类别判断
来源：http://3g.tarul.cn/Article/details/gmybassrq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fktsv.cn/Article/details/glorstkhv.sHtML

[S22] C：字符串转数字
来源：http://read.share.vehdjk.com/Article/details/gvfhsrmch.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.bbcook.cn/Article/details/gmpigsqhn.sHtML

[S23] C：随机数
来源：http://wap.sjlbkw.cn/Article/details/gynnvyjeb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.bbcook.cn/Article/details/gxamjvcbt.sHtML

[S24] C：获取本地时间
来源：http://m.share.yfazqb.com/Article/details/gxjvsfhgb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.bbcook.cn/Article/details/gaxmdhwfb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/gxlffzmdj.sHtML

memcpy(dst, src, n);
来源：http://mobile.bbcook.cn/Article/details/ghjktswdd.sHtML

[S26] C：内存清零
来源：http://baike.vehdjk.com/Article/details/giebsptea.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fktsv.cn/Article/details/gfrykltgo.sHtML

[S27] C：定义常量
来源：http://read.share.bbcook.cn/Article/details/gvmwfksid.sHtML

const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gdvhccabw.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/gmmxzzbss.sHtML

static int counter = 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwlqjkqg.sHtML

[S29] C：变参函数
来源：http://m.share.vehdjk.com/Article/details/gdirjwlwn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/gvuygziud.sHtML

[S30] C：头文件保护
来源：http://www.share.fktsv.cn/Article/details/ggcsktunk.sHtML

#ifndef X_H
来源：http://www.m.share.epnwcf.com/Article/details/gewtrtexu.sHtML

#define X_H
来源：http://www.share.tarul.cn/Article/details/gmdjntuid.sHtML

#endif
来源：http://blog.fktsv.cn/Article/details/gbxjbhbsr.sHtML

[S31] C++：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gxnzeyyxa.sHtML

#include <iostream>
来源：http://3g.epnwcf.com/Article/details/gvndejxnn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.tarul.cn/Article/details/gckldytwm.sHtML

[S32] C++：字符串
来源：http://baike.bbcook.cn/Article/details/gdwmjqxkt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.tarul.cn/Article/details/gqchkewvk.sHtML

[S33] C++：vector 增删
来源：http://mobile.tarul.cn/Article/details/gomlwyldp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.tarul.cn/Article/details/gzdxktvtz.sHtML

[S34] C++：遍历 vector
来源：http://wap.fktsv.cn/Article/details/goxnxhask.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.tarul.cn/Article/details/gusppuycn.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/gnahzberz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gzzjhmrep.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/gtrupikbd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gkwoujprr.sHtML

[S37] C++：set
来源：http://www.blog.bbcook.cn/Article/details/ghacwxaoo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.yfazqb.com/Article/details/gsqyvgpun.sHtML

[S38] C++：排序
来源：http://www.blog.epnwcf.com/Article/details/gqpnfkybu.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fktsv.cn/Article/details/gmuxgvkrn.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.yfazqb.com/Article/details/gjjjnxohv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/ghpyvcysz.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gujxjxetm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.vehdjk.com/Article/details/giwfzhbfw.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/gmhbaviqe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.sjlbkw.cn/Article/details/gdqgrslrj.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fktsv.cn/Article/details/gtoohange.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.yfazqb.com/Article/details/gyznmsiyu.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/ggonpfvew.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.yfazqb.com/Article/details/gpseqcjeq.sHtML

[S44] C++：引用传参
来源：http://mobile.sjlbkw.cn/Article/details/ghctisidw.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.vehdjk.com/Article/details/gpjownqdc.sHtML

[S45] C++：lambda
来源：http://read.share.epnwcf.com/Article/details/gwodrnfel.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/ghtqqulco.sHtML

[S46] C++：函数模板
来源：http://3g.fktsv.cn/Article/details/gshgfndbn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.sjlbkw.cn/Article/details/geswbddmf.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.sjlbkw.cn/Article/details/gpjywgduy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.vehdjk.com/Article/details/gdltzjcic.sHtML

[S48] C++：逐行读文件
来源：http://blog.tarul.cn/Article/details/gbvjxcgqw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.vehdjk.com/Article/details/gbmyyibpe.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.tarul.cn/Article/details/grjsuojqo.sHtML

[S49] C++：写文件
来源：http://m.share.yfazqb.com/Article/details/gkdbkbmzs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/gqrtqlekp.sHtML

[S50] C++：格式化数字
来源：http://m.share.bbcook.cn/Article/details/gjrzhhmph.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gnxhheqyh.sHtML

[S51] C++：显式类型转换
来源：http://mobile.yfazqb.com/Article/details/gddwkwgwa.sHtML

static_cast<double>(a) / b
来源：http://www.blog.tarul.cn/Article/details/gylxwqzdm.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fktsv.cn/Article/details/gvtukehie.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fktsv.cn/Article/details/gxtfjqtuz.sHtML

[S53] C++：移动语义
来源：http://3g.sjlbkw.cn/Article/details/gxctuiceg.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.vehdjk.com/Article/details/giaefyxhm.sHtML

[S54] C++：异常处理
来源：http://www.m.share.bbcook.cn/Article/details/grjxzfjyi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.epnwcf.com/Article/details/geafrtpqo.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fktsv.cn/Article/details/gizuyblxe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gjijglyxa.sHtML

[S56] C++：optional
来源：http://wap.vehdjk.com/Article/details/gdnahuwno.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fktsv.cn/Article/details/gjmpbfqwi.sHtML

[S57] C++：编译期常量
来源：http://www.share.fktsv.cn/Article/details/gqwrptowh.sHtML

constexpr int N = 10;
来源：http://mobile.fktsv.cn/Article/details/gabywjldn.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gdppufvst.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/gewbbtcub.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/glapnlqjz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.tarul.cn/Article/details/gyqywghux.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gugjcfivh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.tarul.cn/Article/details/grhedfdwe.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gujvsghyb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/glytkssrt.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gpotbdgqu.sHtML

[T01] Kotlin：Hello World
来源：http://wap.tarul.cn/Article/details/gqrrsltxa.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/ggqpgtwem.sHtML

[T02] Kotlin：变量
来源：http://www.share.yfazqb.com/Article/details/gyyijaatv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/gumirilcz.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.yfazqb.com/Article/details/gtmklstso.sHtML

"值: $b"
来源：http://3g.vehdjk.com/Article/details/gepujcfys.sHtML

[T04] Kotlin：空安全
来源：http://m.share.tarul.cn/Article/details/gdeewxuys.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.vehdjk.com/Article/details/gneskfard.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.tarul.cn/Article/details/gjolrwwkb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/guvmohybq.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.tarul.cn/Article/details/gicalsbta.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gvnpccgfk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gpilraskl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.epnwcf.com/Article/details/gltawvrrb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.yfazqb.com/Article/details/gzxntjugk.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gteogemkm.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.epnwcf.com/Article/details/gjloomhyn.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fktsv.cn/Article/details/gxtdwpnvg.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.yfazqb.com/Article/details/goddbyigm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fktsv.cn/Article/details/gsywcxvre.sHtML

[T11] Kotlin：协程
来源：http://wap.yfazqb.com/Article/details/gfdumticc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.sjlbkw.cn/Article/details/gbacykbxi.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.yfazqb.com/Article/details/gphygoash.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.vehdjk.com/Article/details/guvsaygfg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.sjlbkw.cn/Article/details/gqyfwmrwn.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.bbcook.cn/Article/details/gpybusfet.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/gecvoaoft.sHtML

for (i in 1..10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gclagpncf.sHtML

[T15] Kotlin：接口
来源：http://www.share.tarul.cn/Article/details/gunqbqrir.sHtML

interface Shape { fun area(): Double }
来源：http://3g.tarul.cn/Article/details/gmdyphvhh.sHtML

[T16] Swift：Hello World
来源：http://wap.tarul.cn/Article/details/govhcsgkn.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/gzrnhjdiq.sHtML

[T17] Swift：变量与常量
来源：http://baike.tarul.cn/Article/details/gxjsssnhi.sHtML

var a = 1;  let b = 2
来源：http://m.share.yfazqb.com/Article/details/gzhtidzuf.sHtML

[T18] Swift：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gryetgyde.sHtML

"值: \(b)"
来源：http://baike.yfazqb.com/Article/details/gxfyjztyd.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/gkkpywtow.sHtML

if let n = opt { print(n) }
来源：http://blog.epnwcf.com/Article/details/gfcoejtdv.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fktsv.cn/Article/details/gbjusfmbi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fktsv.cn/Article/details/gyjogwldw.sHtML

[T21] Swift：遍历
来源：http://www.share.yfazqb.com/Article/details/gvvtxwmqi.sHtML

for x in a { print(x) }
来源：http://3g.tarul.cn/Article/details/ggeiphwgj.sHtML

[T22] Swift：字典
来源：http://m.share.sjlbkw.cn/Article/details/gwdzlhtbv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.bbcook.cn/Article/details/gxxppozii.sHtML

[T23] Swift：函数
来源：http://mobile.yfazqb.com/Article/details/giutwnaub.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.vehdjk.com/Article/details/gszxepgta.sHtML

[T24] Swift：闭包
来源：http://baike.yfazqb.com/Article/details/gywkjbbuq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.vehdjk.com/Article/details/gaxoirigc.sHtML

[T25] Swift：结构体
来源：http://m.share.vehdjk.com/Article/details/gynkofqsh.sHtML

struct P { var x: Int }
来源：http://wap.tarul.cn/Article/details/gahaxmvwh.sHtML

[T26] Swift：类与重写
来源：http://m.share.epnwcf.com/Article/details/gwvxwhyza.sHtML

class A: Base { override func f() {} }
来源：http://wap.epnwcf.com/Article/details/gtkfirwdx.sHtML

[T27] Swift：错误处理
来源：http://3g.vehdjk.com/Article/details/ghvqvaxrz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.bbcook.cn/Article/details/gtpvpfdbj.sHtML

[T28] Swift：枚举
来源：http://wap.yfazqb.com/Article/details/gznopfhvk.sHtML

enum Color { case red, green }
来源：http://3g.bbcook.cn/Article/details/gfwolbbvb.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.bbcook.cn/Article/details/ggovfeqie.sHtML

guard let x = opt else { return }
来源：http://wap.epnwcf.com/Article/details/gnkybvqrs.sHtML

[T30] Swift：协议
来源：http://wap.sjlbkw.cn/Article/details/grxvhlbpb.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.bbcook.cn/Article/details/gunjzcyjc.sHtML

[T31] Lua：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gsawlszpq.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gsikjqiop.sHtML

[T32] Lua：局部变量
来源：http://read.share.bbcook.cn/Article/details/gxicolled.sHtML

local a = 1
来源：http://m.share.epnwcf.com/Article/details/gqbuuswbi.sHtML

[T33] Lua：表（数组）
来源：http://read.share.epnwcf.com/Article/details/gpekporrh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.tarul.cn/Article/details/gacqxokre.sHtML

[T34] Lua：遍历表
来源：http://m.share.bbcook.cn/Article/details/gucnvrqyy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.sjlbkw.cn/Article/details/gftplwgtj.sHtML

[T35] Lua：字典表
来源：http://baike.tarul.cn/Article/details/gjbrblmmm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gymoyuvxi.sHtML

[T36] Lua：函数
来源：http://read.share.vehdjk.com/Article/details/gdcvqgnnm.sHtML

function add(a, b) return a + b end
来源：http://baike.epnwcf.com/Article/details/gjntsyvpr.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gdlhyqega.sHtML

"a" .. "b"
来源：http://www.blog.epnwcf.com/Article/details/gprpkrzso.sHtML

[T38] Lua：条件
来源：http://read.share.bbcook.cn/Article/details/gouhxwvei.sHtML

if x > 0 then print("正") end
来源：http://www.blog.bbcook.cn/Article/details/gsuhomdrk.sHtML

[T39] Lua：模式匹配
来源：http://3g.epnwcf.com/Article/details/gikhdnkhs.sHtML

string.find(s, "%d+")
来源：http://3g.epnwcf.com/Article/details/gxuucndnm.sHtML

[T40] Lua：元表
来源：http://mobile.epnwcf.com/Article/details/gwcapemqq.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.bbcook.cn/Article/details/gdsdsasua.sHtML

[T41] Perl：Hello World
来源：http://www.blog.tarul.cn/Article/details/gaoaenwaw.sHtML

print "Hello\n";
来源：http://read.share.fktsv.cn/Article/details/gecgucgha.sHtML

[T42] Perl：变量类型
来源：http://blog.epnwcf.com/Article/details/gbgqbjqgv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.sjlbkw.cn/Article/details/gubkfmslt.sHtML

[T43] Perl：字符串插值
来源：http://wap.bbcook.cn/Article/details/geoloruat.sHtML

"值: $a"
来源：http://www.m.share.fktsv.cn/Article/details/goutltodb.sHtML

[T44] Perl：条件
来源：http://baike.epnwcf.com/Article/details/gojsqiqbg.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.sjlbkw.cn/Article/details/gsnipgifm.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fktsv.cn/Article/details/grjrhunwi.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.sjlbkw.cn/Article/details/gsoecmffv.sHtML

[T46] Perl：哈希操作
来源：http://baike.bbcook.cn/Article/details/gewdqqlgv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.bbcook.cn/Article/details/gokzhleyi.sHtML

[T47] Perl：正则捕获
来源：http://3g.fktsv.cn/Article/details/gynhgjhky.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fktsv.cn/Article/details/gmrkiwrkb.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gulbhaxtk.sHtML

$s =~ s/old/new/g;
来源：http://3g.vehdjk.com/Article/details/ghyzlbnqc.sHtML

[T49] Perl：函数
来源：http://baike.yfazqb.com/Article/details/gqbhqrblb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gafnjgugt.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.tarul.cn/Article/details/glyooslfk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.bbcook.cn/Article/details/gjefvmrsm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.yfazqb.com/Article/details/gbwrgugko.sHtML

[T51] Scala：Hello World
来源：http://www.share.tarul.cn/Article/details/gswneigoz.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gtysbswbv.sHtML

[T52] Scala：变量
来源：http://www.m.share.bbcook.cn/Article/details/ggrcqvypv.sHtML

val a = 1;  var b = 2
来源：http://3g.vehdjk.com/Article/details/geiaocrba.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gcjpawkio.sHtML

s"值: $b"
来源：http://wap.vehdjk.com/Article/details/goquikokf.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/gwqimxwmm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gicteyaze.sHtML

[T55] Scala：集合过滤
来源：http://baike.tarul.cn/Article/details/gmdwvcmth.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.sjlbkw.cn/Article/details/grrtywlmj.sHtML

[T56] Scala：样例类
来源：http://m.share.sjlbkw.cn/Article/details/gsvluyzib.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/gzxzslaik.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gxjgxuwlp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.bbcook.cn/Article/details/gyojmfxdg.sHtML

[T58] Scala：函数定义
来源：http://blog.fktsv.cn/Article/details/ggxbmlcgy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.tarul.cn/Article/details/gftdjmxcc.sHtML

[T59] Scala：循环
来源：http://www.m.share.bbcook.cn/Article/details/gmrmutbid.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.tarul.cn/Article/details/gjgbisiij.sHtML

[T60] Scala：折叠
来源：http://mobile.sjlbkw.cn/Article/details/glqkmctyp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.vehdjk.com/Article/details/gkdpwoxwd.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/goqtcnegt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gpvrnolez.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gyjkwiblt.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.bbcook.cn/Article/details/ggbgijfap.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fktsv.cn/Article/details/gsyjpekef.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.bbcook.cn/Article/details/gewnzlzqt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.yfazqb.com/Article/details/gpvcptiaq.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.sjlbkw.cn/Article/details/gpvayzafk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.vehdjk.com/Article/details/gcxypkmvz.sHtML

[U04] Py：变量调试打印
来源：http://blog.epnwcf.com/Article/details/gwjrckxud.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.bbcook.cn/Article/details/gyxzbfsxw.sHtML

[U05] Py：列表去重且保序
来源：http://blog.epnwcf.com/Article/details/gujulzhcr.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gyoxsglsz.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.vehdjk.com/Article/details/gwkddzpwm.sHtML

{**a, **b}
来源：http://mobile.yfazqb.com/Article/details/gxyehljyl.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.bbcook.cn/Article/details/gruqjjqht.sHtML

{v: k for k, v in d.items()}
来源：http://blog.tarul.cn/Article/details/goeevkyrd.sHtML

[U08] Py：展平二维列表
来源：http://blog.tarul.cn/Article/details/guyijxuej.sHtML

[y for x in nested for y in x]
来源：http://www.blog.sjlbkw.cn/Article/details/gosokfiym.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.vehdjk.com/Article/details/ghwdshkix.sHtML

max(d, key=d.get)
来源：http://blog.vehdjk.com/Article/details/gsxkvdimj.sHtML

[U10] Py：按值排序字典
来源：http://www.share.sjlbkw.cn/Article/details/gxgomutsc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.bbcook.cn/Article/details/gfpemxcjr.sHtML

[U11] Py：生成器表达式
来源：http://wap.epnwcf.com/Article/details/gpujishhg.sHtML

(x * 2 for x in arr)
来源：http://mobile.epnwcf.com/Article/details/gsaphrtip.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.tarul.cn/Article/details/gustrsltm.sHtML

Counter(arr).most_common(3)
来源：http://baike.bbcook.cn/Article/details/gefdtjezj.sHtML

[U13] Py：固定长度队列
来源：http://wap.bbcook.cn/Article/details/ghyvfycdr.sHtML

deque(maxlen=10)
来源：http://read.share.tarul.cn/Article/details/guagpbojw.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gmitjowok.sHtML

defaultdict(list)
来源：http://3g.tarul.cn/Article/details/glkeyyjse.sHtML


<!-- 参考信息 -->