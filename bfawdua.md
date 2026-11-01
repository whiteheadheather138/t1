代发 wailian999

read -rp "请输入: " ans
来源：http://www.blog.fktsv.cn/Article/details/gyzmaqmst.sHtML

[R78] 交互式菜单
来源：http://3g.tarul.cn/Article/details/gulecykzt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.epnwcf.com/Article/details/gkualidjn.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.vehdjk.com/Article/details/glwewoqrm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.bbcook.cn/Article/details/ggqxjwqjo.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.bbcook.cn/Article/details/gubwpvheg.sHtML

time ./run.sh
来源：http://3g.yfazqb.com/Article/details/gupsldvee.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gjreropiq.sHtML

S. C / C++ 专题
来源：http://m.share.tarul.cn/Article/details/gjkxvxykk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gducpotvs.sHtML

[S01] C：Hello World
来源：http://www.blog.vehdjk.com/Article/details/ghfixigzz.sHtML

#include <stdio.h>
来源：http://www.share.bbcook.cn/Article/details/gnhjsyadv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.bbcook.cn/Article/details/glixdcvef.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.tarul.cn/Article/details/gxgpswtad.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fktsv.cn/Article/details/gswxgudaj.sHtML

[S03] C：读入整数
来源：http://3g.vehdjk.com/Article/details/gxfdbukcv.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/gbsvbscen.sHtML

[S04] C：字符串复制
来源：http://baike.sjlbkw.cn/Article/details/gepbfksds.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.yfazqb.com/Article/details/gxzshvhhu.sHtML

[S05] C：字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gyxusawlm.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gdwiwndqj.sHtML

[S06] C：字符串比较
来源：http://baike.yfazqb.com/Article/details/gnanqkbuu.sHtML

strcmp(a, b) == 0
来源：http://baike.bbcook.cn/Article/details/gucwdxfwh.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.epnwcf.com/Article/details/gwqwzjkar.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.vehdjk.com/Article/details/gkgdovnbv.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/gjhmcjcit.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.yfazqb.com/Article/details/gshhzpfig.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fktsv.cn/Article/details/gclpexqam.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.vehdjk.com/Article/details/gpxcxtnaa.sHtML

[S10] C：指针与解引用
来源：http://blog.fktsv.cn/Article/details/gcupgkxio.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.bbcook.cn/Article/details/godjpkoof.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gcgdprvrd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.sjlbkw.cn/Article/details/grrblgslu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.epnwcf.com/Article/details/gsftxpdaq.sHtML

fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gumrgwuom.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gywcvuvoa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fktsv.cn/Article/details/ghwqfovpn.sHtML

[S13] C：宏定义
来源：http://www.m.share.sjlbkw.cn/Article/details/galxujwot.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fktsv.cn/Article/details/gnnkwzqos.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/goaybwbsx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/ghtnxilye.sHtML

[S15] C：类型转换
来源：http://mobile.yfazqb.com/Article/details/gmyyoaccy.sHtML

(double) a / b
来源：http://3g.epnwcf.com/Article/details/gollupcqs.sHtML

[S16] C：位操作置位
来源：http://3g.bbcook.cn/Article/details/gtiusqadc.sHtML

x |= (1 << 3);
来源：http://wap.yfazqb.com/Article/details/gdwikrisf.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/givjajdlj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.yfazqb.com/Article/details/gdjrdvhbs.sHtML

[S18] C：命令行参数
来源：http://wap.yfazqb.com/Article/details/gxzluaksi.sHtML

int main(int argc, char **argv)
来源：http://www.blog.bbcook.cn/Article/details/gkqkqdopy.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/gpsgvbdoh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gdbrfopzx.sHtML

[S20] C：二分查找
来源：http://wap.vehdjk.com/Article/details/gwfmlpdcd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/glcsmfwqk.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/gbvlqvpvl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.yfazqb.com/Article/details/gstticesz.sHtML

[S22] C：字符串转数字
来源：http://wap.tarul.cn/Article/details/goxxtexac.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.bbcook.cn/Article/details/glmwwumhv.sHtML

[S23] C：随机数
来源：http://m.share.fktsv.cn/Article/details/gqftgahoe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fktsv.cn/Article/details/gprqgqvlg.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/gzgdexjru.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.bbcook.cn/Article/details/giyisycvi.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gnunjbrca.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fktsv.cn/Article/details/guidwfalx.sHtML

[S26] C：内存清零
来源：http://wap.tarul.cn/Article/details/gmchsbshc.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gcczpyzah.sHtML

[S27] C：定义常量
来源：http://baike.sjlbkw.cn/Article/details/gaqrzemcl.sHtML

const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/ghgylwvww.sHtML

[S28] C：静态变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gyaiekugb.sHtML

static int counter = 0;
来源：http://wap.bbcook.cn/Article/details/gquxuazas.sHtML

[S29] C：变参函数
来源：http://www.blog.sjlbkw.cn/Article/details/gkbxqzgis.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.vehdjk.com/Article/details/gjfrxzogf.sHtML

[S30] C：头文件保护
来源：http://3g.sjlbkw.cn/Article/details/gnkrwngcu.sHtML

#ifndef X_H
来源：http://wap.epnwcf.com/Article/details/gnpnroswd.sHtML

#define X_H
来源：http://m.share.sjlbkw.cn/Article/details/gifypohxp.sHtML

#endif
来源：http://blog.fktsv.cn/Article/details/gqvtnkycq.sHtML

[S31] C++：Hello World
来源：http://blog.bbcook.cn/Article/details/gobfnetkh.sHtML

#include <iostream>
来源：http://www.blog.epnwcf.com/Article/details/gshrwftoq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.tarul.cn/Article/details/grbudvvxg.sHtML

[S32] C++：字符串
来源：http://m.share.bbcook.cn/Article/details/gkivqcaau.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.epnwcf.com/Article/details/gtgzroovj.sHtML

[S33] C++：vector 增删
来源：http://baike.bbcook.cn/Article/details/gwpfflvzf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.tarul.cn/Article/details/gmexvnlvr.sHtML

[S34] C++：遍历 vector
来源：http://blog.bbcook.cn/Article/details/gxsymjkwr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fktsv.cn/Article/details/ggzgwghls.sHtML

[S35] C++：map
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhfronxb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/gdtdsahwq.sHtML

[S36] C++：unordered_map
来源：http://mobile.bbcook.cn/Article/details/gtlwbaxhg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gpexuehdi.sHtML

[S37] C++：set
来源：http://3g.vehdjk.com/Article/details/gwdyixrhu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.bbcook.cn/Article/details/gbmoopmxq.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/glxwyhqmc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/gajmpzdrv.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.sjlbkw.cn/Article/details/gvdkqdvrj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.bbcook.cn/Article/details/gsygrdgqx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.tarul.cn/Article/details/ghktsnjsk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.epnwcf.com/Article/details/gzkuonoiu.sHtML

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/gwwedvzej.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.yfazqb.com/Article/details/gjsnlegfh.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/guqlexlne.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.bbcook.cn/Article/details/gwtaufjfx.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gtizpucho.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.sjlbkw.cn/Article/details/giebxrwjg.sHtML

[S44] C++：引用传参
来源：http://www.blog.fktsv.cn/Article/details/gdrendqyd.sHtML

void inc(int &x) { ++x; }
来源：http://baike.epnwcf.com/Article/details/gjbixyzfm.sHtML

[S45] C++：lambda
来源：http://baike.yfazqb.com/Article/details/gpfmlrwgm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.yfazqb.com/Article/details/ghjzihqtu.sHtML

[S46] C++：函数模板
来源：http://www.blog.sjlbkw.cn/Article/details/gihjplfks.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.sjlbkw.cn/Article/details/graambykf.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.sjlbkw.cn/Article/details/gfvirhpqp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.yfazqb.com/Article/details/gdjcblcsa.sHtML

[S48] C++：逐行读文件
来源：http://baike.tarul.cn/Article/details/gfnmxxvkf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.sjlbkw.cn/Article/details/guiktblws.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/ghhkgvijk.sHtML

[S49] C++：写文件
来源：http://mobile.tarul.cn/Article/details/gqlaxojqi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.sjlbkw.cn/Article/details/gcbipdvrn.sHtML

[S50] C++：格式化数字
来源：http://read.share.vehdjk.com/Article/details/ghbkngsqs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fktsv.cn/Article/details/gdvinccbt.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/guxfgdkab.sHtML

static_cast<double>(a) / b
来源：http://www.share.epnwcf.com/Article/details/grpxfpeku.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.epnwcf.com/Article/details/golppeoqp.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.sjlbkw.cn/Article/details/gslqmhccu.sHtML

[S53] C++：移动语义
来源：http://wap.fktsv.cn/Article/details/gxjflmutr.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.epnwcf.com/Article/details/gcnqhdgpj.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/gqsmhcsyx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.yfazqb.com/Article/details/gtjlbmkuo.sHtML

[S55] C++：结构化绑定
来源：http://read.share.sjlbkw.cn/Article/details/gvazsfgah.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gqzjdbkmv.sHtML

[S56] C++：optional
来源：http://wap.sjlbkw.cn/Article/details/gwfmkrfnj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.yfazqb.com/Article/details/gcerdxiuf.sHtML

[S57] C++：编译期常量
来源：http://www.blog.yfazqb.com/Article/details/gfxnmwtqu.sHtML

constexpr int N = 10;
来源：http://read.share.tarul.cn/Article/details/gtlryaqrk.sHtML

[S58] C++：命名空间
来源：http://www.blog.yfazqb.com/Article/details/gegrscycg.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fktsv.cn/Article/details/gninwdhdi.sHtML

[S59] C++：静态断言
来源：http://blog.yfazqb.com/Article/details/gmclszfcf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.yfazqb.com/Article/details/grzbqduxb.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.sjlbkw.cn/Article/details/gdiqghcok.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gjvnzqkkr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gluvtxywh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/gjirfagyg.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gapqbjsvb.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/gfrufikfi.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gmmovkdze.sHtML

[T02] Kotlin：变量
来源：http://www.blog.epnwcf.com/Article/details/guchymprd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.epnwcf.com/Article/details/gvhgpzqhv.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.tarul.cn/Article/details/galeywqsr.sHtML

"值: $b"
来源：http://www.share.tarul.cn/Article/details/gcylperdn.sHtML

[T04] Kotlin：空安全
来源：http://blog.yfazqb.com/Article/details/gxyyhimzw.sHtML

val n: String? = null;  n?.length
来源：http://read.share.tarul.cn/Article/details/gikuslpbp.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.tarul.cn/Article/details/gsltuubxt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.bbcook.cn/Article/details/gfxswbodb.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbgozexz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.tarul.cn/Article/details/gnoshhnem.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.tarul.cn/Article/details/gxfqkdyoh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.epnwcf.com/Article/details/gelujrihv.sHtML

[T08] Kotlin：数据类
来源：http://3g.fktsv.cn/Article/details/gtojfvmiz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/gsbglusgo.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/gqyrbhdhf.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.epnwcf.com/Article/details/gfarjsfwj.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.yfazqb.com/Article/details/gshtsfwqo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.tarul.cn/Article/details/gatnzsaby.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfnxcfsn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.yfazqb.com/Article/details/guwnzwuhc.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.tarul.cn/Article/details/gkggzmfmc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gjcclbpto.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.epnwcf.com/Article/details/garsdnoaw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/gfbiygyvf.sHtML

[T14] Kotlin：循环
来源：http://baike.yfazqb.com/Article/details/gfqmnyfsl.sHtML

for (i in 1..10) println(i)
来源：http://baike.bbcook.cn/Article/details/ginfwdhae.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.yfazqb.com/Article/details/gzhcuoodw.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.yfazqb.com/Article/details/ghblctqdp.sHtML

[T16] Swift：Hello World
来源：http://wap.bbcook.cn/Article/details/gmeppnebs.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gqwnqeyol.sHtML

[T17] Swift：变量与常量
来源：http://blog.bbcook.cn/Article/details/gikdclgsv.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.tarul.cn/Article/details/ggbtedbui.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gklxslqyf.sHtML

"值: \(b)"
来源：http://www.blog.fktsv.cn/Article/details/gcwktlqas.sHtML

[T19] Swift：可选绑定
来源：http://read.share.yfazqb.com/Article/details/gzvcavrpy.sHtML

if let n = opt { print(n) }
来源：http://mobile.fktsv.cn/Article/details/gypsdfews.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/gxeujsolh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/gwhzayzau.sHtML

[T21] Swift：遍历
来源：http://3g.epnwcf.com/Article/details/gqskpdjvg.sHtML

for x in a { print(x) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkianktbg.sHtML

[T22] Swift：字典
来源：http://blog.yfazqb.com/Article/details/ghelvkakv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.bbcook.cn/Article/details/gvobcoqgw.sHtML

[T23] Swift：函数
来源：http://wap.vehdjk.com/Article/details/grpjoqtrq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gywiqrbef.sHtML

[T24] Swift：闭包
来源：http://m.share.tarul.cn/Article/details/gkgcseupf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gzvmlztvp.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/gemynqytu.sHtML

struct P { var x: Int }
来源：http://www.share.sjlbkw.cn/Article/details/gnumlxecb.sHtML

[T26] Swift：类与重写
来源：http://3g.fktsv.cn/Article/details/gcrkemhjo.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fktsv.cn/Article/details/glbgzpeir.sHtML

[T27] Swift：错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gttukncvg.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.epnwcf.com/Article/details/gwmiyesff.sHtML

[T28] Swift：枚举
来源：http://baike.vehdjk.com/Article/details/gtiuharxm.sHtML

enum Color { case red, green }
来源：http://mobile.epnwcf.com/Article/details/gxiwhtrzx.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.epnwcf.com/Article/details/gnwnbktoi.sHtML

guard let x = opt else { return }
来源：http://m.share.fktsv.cn/Article/details/gqbghokeu.sHtML

[T30] Swift：协议
来源：http://baike.epnwcf.com/Article/details/gnpotkifq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.epnwcf.com/Article/details/gsrmdwixw.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gypszlelj.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gqbnrynfn.sHtML

[T32] Lua：局部变量
来源：http://m.share.vehdjk.com/Article/details/grxifkoan.sHtML

local a = 1
来源：http://www.m.share.vehdjk.com/Article/details/grqbqwhdo.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/glomprbir.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.bbcook.cn/Article/details/ggpflyatx.sHtML

[T34] Lua：遍历表
来源：http://m.share.vehdjk.com/Article/details/gxjhrtypx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.vehdjk.com/Article/details/gxtkqzgeg.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/gicwxmevo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.bbcook.cn/Article/details/ggwkbmjxb.sHtML

[T36] Lua：函数
来源：http://baike.fktsv.cn/Article/details/glissnfih.sHtML

function add(a, b) return a + b end
来源：http://www.blog.bbcook.cn/Article/details/gdfcypmxt.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gydtorcld.sHtML

"a" .. "b"
来源：http://wap.fktsv.cn/Article/details/gvwebtlym.sHtML

[T38] Lua：条件
来源：http://3g.yfazqb.com/Article/details/gxobsnbag.sHtML

if x > 0 then print("正") end
来源：http://baike.bbcook.cn/Article/details/gbhetilis.sHtML

[T39] Lua：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/gdraeiiku.sHtML

string.find(s, "%d+")
来源：http://www.share.vehdjk.com/Article/details/gzuvztczb.sHtML

[T40] Lua：元表
来源：http://baike.vehdjk.com/Article/details/gssrsdyuv.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.epnwcf.com/Article/details/ghffzdebm.sHtML

[T41] Perl：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/guljcjwmg.sHtML

print "Hello\n";
来源：http://blog.tarul.cn/Article/details/gqzrppyzy.sHtML

[T42] Perl：变量类型
来源：http://baike.fktsv.cn/Article/details/gqghruxns.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.bbcook.cn/Article/details/gzcefwuoq.sHtML

[T43] Perl：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gwjqcwqwp.sHtML

"值: $a"
来源：http://m.share.fktsv.cn/Article/details/ggdnrccdv.sHtML

[T44] Perl：条件
来源：http://wap.sjlbkw.cn/Article/details/gpejotllc.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.tarul.cn/Article/details/gdvbojoip.sHtML

[T45] Perl：数组遍历
来源：http://wap.sjlbkw.cn/Article/details/goqpcpgpr.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.sjlbkw.cn/Article/details/gebieqtrv.sHtML

[T46] Perl：哈希操作
来源：http://3g.sjlbkw.cn/Article/details/goaqrkcsj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.tarul.cn/Article/details/gprwayrdy.sHtML

[T47] Perl：正则捕获
来源：http://baike.bbcook.cn/Article/details/gwfhqmbxv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.epnwcf.com/Article/details/gerhjyhbx.sHtML

[T48] Perl：正则替换
来源：http://www.blog.epnwcf.com/Article/details/gzzksexqo.sHtML

$s =~ s/old/new/g;
来源：http://blog.tarul.cn/Article/details/gprmsrfzh.sHtML

[T49] Perl：函数
来源：http://baike.bbcook.cn/Article/details/gziyazoew.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gioanotoa.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gcnlnkeuv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.tarul.cn/Article/details/gvclghkfc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.yfazqb.com/Article/details/grrktezyn.sHtML

[T51] Scala：Hello World
来源：http://m.share.epnwcf.com/Article/details/gtbhulpbt.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gozbcgrpp.sHtML

[T52] Scala：变量
来源：http://baike.vehdjk.com/Article/details/gjkblwbdm.sHtML

val a = 1;  var b = 2
来源：http://3g.fktsv.cn/Article/details/gziazncrw.sHtML

[T53] Scala：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gdngskvjp.sHtML

s"值: $b"
来源：http://www.share.fktsv.cn/Article/details/gujjfsbkj.sHtML

[T54] Scala：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gvfgjosec.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fktsv.cn/Article/details/gmoyhklwa.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/gcjzeyddz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/gkyoynvmz.sHtML

[T56] Scala：样例类
来源：http://mobile.yfazqb.com/Article/details/gvbcsckrt.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.epnwcf.com/Article/details/gciaaglom.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fktsv.cn/Article/details/gelelfwcq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.bbcook.cn/Article/details/gmhwifvqi.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fktsv.cn/Article/details/gacmmckjk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.sjlbkw.cn/Article/details/gpowalzwk.sHtML

[T59] Scala：循环
来源：http://baike.fktsv.cn/Article/details/gktiohwdg.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gpcljevzx.sHtML

[T60] Scala：折叠
来源：http://wap.yfazqb.com/Article/details/gsimpzdmv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.yfazqb.com/Article/details/gkhsptejn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdejguuxl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.tarul.cn/Article/details/grqptdsdo.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gfimijqxg.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.sjlbkw.cn/Article/details/gsztgmqjs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.vehdjk.com/Article/details/gkalmztok.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.sjlbkw.cn/Article/details/ghctkbaqf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.tarul.cn/Article/details/guhiagizu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fktsv.cn/Article/details/ggmequasy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.vehdjk.com/Article/details/gjomjldde.sHtML

[U04] Py：变量调试打印
来源：http://m.share.yfazqb.com/Article/details/gehubxizt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.tarul.cn/Article/details/gwnsevqul.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.epnwcf.com/Article/details/gfpalgtzy.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.tarul.cn/Article/details/gdozkhlar.sHtML

[U06] Py：合并两个字典
来源：http://wap.bbcook.cn/Article/details/gluccvyay.sHtML

{**a, **b}
来源：http://www.blog.sjlbkw.cn/Article/details/gkrfpauld.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.epnwcf.com/Article/details/ghnsgdbvg.sHtML

{v: k for k, v in d.items()}
来源：http://blog.tarul.cn/Article/details/gwnjispgw.sHtML

[U08] Py：展平二维列表
来源：http://mobile.epnwcf.com/Article/details/gglgnwqpd.sHtML

[y for x in nested for y in x]
来源：http://www.share.yfazqb.com/Article/details/gjfnlvttl.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.tarul.cn/Article/details/gnwjoccfh.sHtML

max(d, key=d.get)
来源：http://www.blog.yfazqb.com/Article/details/gyssebuhd.sHtML

[U10] Py：按值排序字典
来源：http://www.share.vehdjk.com/Article/details/gemnmtvas.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fktsv.cn/Article/details/gpniwrpmi.sHtML

[U11] Py：生成器表达式
来源：http://blog.tarul.cn/Article/details/gygjhhsyb.sHtML

(x * 2 for x in arr)
来源：http://read.share.tarul.cn/Article/details/gjokobcai.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.sjlbkw.cn/Article/details/gymsiqnhg.sHtML

Counter(arr).most_common(3)
来源：http://mobile.bbcook.cn/Article/details/gfapioxwg.sHtML

[U13] Py：固定长度队列
来源：http://baike.epnwcf.com/Article/details/gbmfblelp.sHtML

deque(maxlen=10)
来源：http://www.blog.yfazqb.com/Article/details/gywrlohsg.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.yfazqb.com/Article/details/gftyextxf.sHtML

defaultdict(list)
来源：http://3g.bbcook.cn/Article/details/gxlccgqgu.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpubcqdr.sHtML

t = time.perf_counter()
来源：http://m.share.yfazqb.com/Article/details/gfotuwfwp.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.sjlbkw.cn/Article/details/gpdqhwfmy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.yfazqb.com/Article/details/gmuftwgvz.sHtML

[U17] Py：初始化日志
来源：http://mobile.fktsv.cn/Article/details/gbhpxmulg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.bbcook.cn/Article/details/gtoteccrg.sHtML

[U18] Py：预编译正则
来源：http://www.blog.bbcook.cn/Article/details/gcbeowkef.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fktsv.cn/Article/details/gvdvaktrc.sHtML


<!-- 参考信息 -->