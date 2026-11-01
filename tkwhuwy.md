代发 wailian999

split -l 1000 big.log part_
来源：http://www.m.share.fktsv.cn/Article/details/gkfraiqts.sHtML

[R74] 批量重命名
来源：http://wap.sjlbkw.cn/Article/details/ggedmkapd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.bbcook.cn/Article/details/gtkagqozd.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/gcevxnjwe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/gldgklapy.sHtML

[R76] 使用临时文件
来源：http://read.share.fktsv.cn/Article/details/gqxvcllrx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/ganhvozmz.sHtML

[R77] 读取用户输入
来源：http://blog.sjlbkw.cn/Article/details/gocskyaor.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fktsv.cn/Article/details/gctppetya.sHtML

[R78] 交互式菜单
来源：http://3g.epnwcf.com/Article/details/gnrvxeaoh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.sjlbkw.cn/Article/details/goloigavr.sHtML

[R79] 解析命令行选项
来源：http://m.share.tarul.cn/Article/details/gxlepnwbs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.yfazqb.com/Article/details/gcosfzqiu.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.vehdjk.com/Article/details/ghljoptjn.sHtML

time ./run.sh
来源：http://www.m.share.tarul.cn/Article/details/gpauctgow.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gykkahnzr.sHtML

S. C / C++ 专题
来源：http://m.share.tarul.cn/Article/details/gerlyizos.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpmouorsq.sHtML

[S01] C：Hello World
来源：http://read.share.bbcook.cn/Article/details/gllyvxsun.sHtML

#include <stdio.h>
来源：http://www.blog.bbcook.cn/Article/details/gjiyfjuxe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.vehdjk.com/Article/details/gddswhfgs.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.vehdjk.com/Article/details/gopytfwvg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.epnwcf.com/Article/details/grtfdpvjl.sHtML

[S03] C：读入整数
来源：http://www.m.share.yfazqb.com/Article/details/ggqkffxlu.sHtML

int x; scanf("%d", &x);
来源：http://m.share.yfazqb.com/Article/details/garhxhitt.sHtML

[S04] C：字符串复制
来源：http://www.share.tarul.cn/Article/details/glmcgmddi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fktsv.cn/Article/details/ghyzrslni.sHtML

[S05] C：字符串长度
来源：http://blog.yfazqb.com/Article/details/gchjslvue.sHtML

strlen(s)
来源：http://mobile.bbcook.cn/Article/details/gnrownpuw.sHtML

[S06] C：字符串比较
来源：http://m.share.bbcook.cn/Article/details/gafgrmcam.sHtML

strcmp(a, b) == 0
来源：http://mobile.sjlbkw.cn/Article/details/gjfyywnfv.sHtML

[S07] C：数组遍历求和
来源：http://wap.vehdjk.com/Article/details/gbjppjtrt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.epnwcf.com/Article/details/gujdfxvxf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.yfazqb.com/Article/details/goozkwpsm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.yfazqb.com/Article/details/goaqvvrss.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.yfazqb.com/Article/details/gzdhrlkoj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fktsv.cn/Article/details/gbyrexjeb.sHtML

[S10] C：指针与解引用
来源：http://3g.epnwcf.com/Article/details/gmwpuimtc.sHtML

int *p = &a;  *p = 5;
来源：http://blog.epnwcf.com/Article/details/gyaxyndwp.sHtML

[S11] C：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gphxcscwo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.vehdjk.com/Article/details/gcomzwxoc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fktsv.cn/Article/details/goxayebec.sHtML

fclose(f);
来源：http://baike.vehdjk.com/Article/details/galhynuxj.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/giegvcryc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.bbcook.cn/Article/details/gqmilibgw.sHtML

[S13] C：宏定义
来源：http://mobile.sjlbkw.cn/Article/details/gbizwehkg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.yfazqb.com/Article/details/gljmjdxbt.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/gsdejdhej.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.yfazqb.com/Article/details/gunnkthyt.sHtML

[S15] C：类型转换
来源：http://3g.bbcook.cn/Article/details/gagtbjamp.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/gytmzdxrm.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gsvmgdiqs.sHtML

x |= (1 << 3);
来源：http://m.share.vehdjk.com/Article/details/gckruooaq.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/grenbsbjq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fktsv.cn/Article/details/gsxxqekno.sHtML

[S18] C：命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/gypnwjeza.sHtML

int main(int argc, char **argv)
来源：http://baike.yfazqb.com/Article/details/gtumcyxwz.sHtML

[S19] C：快速排序
来源：http://wap.tarul.cn/Article/details/gzbnjxjwz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmvyipeq.sHtML

[S20] C：二分查找
来源：http://read.share.tarul.cn/Article/details/gisiksfuv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gupxojisv.sHtML

[S21] C：字符类别判断
来源：http://read.share.sjlbkw.cn/Article/details/gptrfjjdq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.bbcook.cn/Article/details/gmnuhzust.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/gwealggrj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.bbcook.cn/Article/details/gjpqffjad.sHtML

[S23] C：随机数
来源：http://baike.sjlbkw.cn/Article/details/gdnzrdqbf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.sjlbkw.cn/Article/details/glajdwigy.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/glcvjwkyb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.bbcook.cn/Article/details/gkdqtakdk.sHtML

[S25] C：内存拷贝
来源：http://wap.epnwcf.com/Article/details/ghurpfllb.sHtML

memcpy(dst, src, n);
来源：http://read.share.vehdjk.com/Article/details/gcyaqkrwh.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/gudjzmqzo.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fktsv.cn/Article/details/gcfmesrjo.sHtML

[S27] C：定义常量
来源：http://m.share.sjlbkw.cn/Article/details/giysladqc.sHtML

const double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gbxqysdjd.sHtML

[S28] C：静态变量
来源：http://baike.vehdjk.com/Article/details/gopzeyhht.sHtML

static int counter = 0;
来源：http://read.share.bbcook.cn/Article/details/gyowtvtai.sHtML

[S29] C：变参函数
来源：http://read.share.yfazqb.com/Article/details/gpgakiooq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.tarul.cn/Article/details/gsptdvzom.sHtML

[S30] C：头文件保护
来源：http://mobile.tarul.cn/Article/details/guotblior.sHtML

#ifndef X_H
来源：http://3g.bbcook.cn/Article/details/gejkyqnzi.sHtML

#define X_H
来源：http://www.m.share.yfazqb.com/Article/details/gkrsrfjts.sHtML

#endif
来源：http://baike.tarul.cn/Article/details/gwfkcjgyq.sHtML

[S31] C++：Hello World
来源：http://3g.yfazqb.com/Article/details/gbqkqmeml.sHtML

#include <iostream>
来源：http://www.m.share.bbcook.cn/Article/details/grhrkqvea.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.tarul.cn/Article/details/gjxsmbwyx.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/gkkxixxkf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.bbcook.cn/Article/details/gpegvccya.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.epnwcf.com/Article/details/gjcvmqfqz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/gotigwlmn.sHtML

[S34] C++：遍历 vector
来源：http://baike.sjlbkw.cn/Article/details/ghvpiqoep.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.vehdjk.com/Article/details/gwirmmwbm.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/ggmlqnwqn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/gglkamrbe.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/ggvbghluj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gmnmhdluo.sHtML

[S37] C++：set
来源：http://www.blog.epnwcf.com/Article/details/gnobmhbfi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.vehdjk.com/Article/details/gnpazamwa.sHtML

[S38] C++：排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxybvglg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.epnwcf.com/Article/details/gmohwtepm.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/gxnvwvbba.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.epnwcf.com/Article/details/gvgtvsuab.sHtML

[S40] C++：查找元素
来源：http://m.share.vehdjk.com/Article/details/gocoawuqy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.vehdjk.com/Article/details/gtptqykwy.sHtML

[S41] C++：类与构造函数
来源：http://www.share.epnwcf.com/Article/details/grruohmnv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fktsv.cn/Article/details/grjeanwym.sHtML

[S42] C++：继承与虚函数
来源：http://blog.tarul.cn/Article/details/gqwffrlzi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/gqamuookp.sHtML

[S43] C++：智能指针
来源：http://wap.epnwcf.com/Article/details/gvnamopgw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fktsv.cn/Article/details/gvwryvwic.sHtML

[S44] C++：引用传参
来源：http://blog.epnwcf.com/Article/details/gdpabtuos.sHtML

void inc(int &x) { ++x; }
来源：http://3g.vehdjk.com/Article/details/gtbhaxwki.sHtML

[S45] C++：lambda
来源：http://m.share.sjlbkw.cn/Article/details/gdkquyvyt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.epnwcf.com/Article/details/geasxwuzq.sHtML

[S46] C++：函数模板
来源：http://read.share.vehdjk.com/Article/details/gmdjtzakh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fktsv.cn/Article/details/gsvlgkqmc.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.vehdjk.com/Article/details/gyxhfidjd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.vehdjk.com/Article/details/gwmvswbdd.sHtML

[S48] C++：逐行读文件
来源：http://blog.tarul.cn/Article/details/gbfnzgseq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.bbcook.cn/Article/details/gqiovcosk.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fktsv.cn/Article/details/gxfhzhlgv.sHtML

[S49] C++：写文件
来源：http://3g.tarul.cn/Article/details/gszhynjcb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.epnwcf.com/Article/details/gizqrkzss.sHtML

[S50] C++：格式化数字
来源：http://www.share.tarul.cn/Article/details/gnehmqyrj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/gwrxdcfnc.sHtML

[S51] C++：显式类型转换
来源：http://blog.tarul.cn/Article/details/gtxakkykx.sHtML

static_cast<double>(a) / b
来源：http://blog.tarul.cn/Article/details/gcjlrlqxd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/gkwqmaoeh.sHtML

int size() const noexcept { return n_; }
来源：http://baike.tarul.cn/Article/details/ggphetgcn.sHtML

[S53] C++：移动语义
来源：http://wap.vehdjk.com/Article/details/gnjpajsbc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.bbcook.cn/Article/details/gympohklk.sHtML

[S54] C++：异常处理
来源：http://3g.epnwcf.com/Article/details/gdsbhjcll.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.sjlbkw.cn/Article/details/gikhnzdbv.sHtML

[S55] C++：结构化绑定
来源：http://3g.fktsv.cn/Article/details/gplkwkhrl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.vehdjk.com/Article/details/gnqqidhkp.sHtML

[S56] C++：optional
来源：http://mobile.bbcook.cn/Article/details/gftmtasjb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.sjlbkw.cn/Article/details/gqnbjlyaf.sHtML

[S57] C++：编译期常量
来源：http://baike.yfazqb.com/Article/details/gugfngahx.sHtML

constexpr int N = 10;
来源：http://3g.bbcook.cn/Article/details/gwmxtvkyv.sHtML

[S58] C++：命名空间
来源：http://wap.tarul.cn/Article/details/gljftikwn.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.yfazqb.com/Article/details/gkakususc.sHtML

[S59] C++：静态断言
来源：http://wap.sjlbkw.cn/Article/details/ghakiptwn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fktsv.cn/Article/details/gjvzdgfka.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.vehdjk.com/Article/details/gpyspvhbi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.epnwcf.com/Article/details/gjonsfbsc.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ggbuxgbgo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/gjdhyjytb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gjiscpfhh.sHtML

[T01] Kotlin：Hello World
来源：http://baike.bbcook.cn/Article/details/gitdccxlj.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gpewpatbj.sHtML

[T02] Kotlin：变量
来源：http://blog.bbcook.cn/Article/details/gdbqjwbvh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/gyivirvar.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gsocfcxzv.sHtML

"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gxijshdpo.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.tarul.cn/Article/details/griyljbwh.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.tarul.cn/Article/details/gkbsydlxw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gooujszyn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.yfazqb.com/Article/details/gnwmoqudq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.vehdjk.com/Article/details/gdvwsjdej.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gtnxffwvq.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gmyhnperk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.tarul.cn/Article/details/gwksqjwkb.sHtML

[T08] Kotlin：数据类
来源：http://m.share.vehdjk.com/Article/details/gbkdhxfim.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.vehdjk.com/Article/details/gcjtpxxec.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/gpsczljxo.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.sjlbkw.cn/Article/details/ggxpidtlr.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.sjlbkw.cn/Article/details/goyqglaqz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.epnwcf.com/Article/details/gvarprjyz.sHtML

[T11] Kotlin：协程
来源：http://m.share.vehdjk.com/Article/details/gzcbibxif.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.epnwcf.com/Article/details/ghbwgzkxn.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.epnwcf.com/Article/details/gjmtxfewq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gdadzooxm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.vehdjk.com/Article/details/gaaylffey.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.yfazqb.com/Article/details/gbelgmymf.sHtML

[T14] Kotlin：循环
来源：http://mobile.sjlbkw.cn/Article/details/gwzywukrc.sHtML

for (i in 1..10) println(i)
来源：http://mobile.vehdjk.com/Article/details/gatggtgss.sHtML

[T15] Kotlin：接口
来源：http://mobile.tarul.cn/Article/details/gmttvjzsr.sHtML

interface Shape { fun area(): Double }
来源：http://wap.bbcook.cn/Article/details/gegbptddc.sHtML

[T16] Swift：Hello World
来源：http://www.blog.tarul.cn/Article/details/gynqnroea.sHtML

print("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gdfhbjtnn.sHtML

[T17] Swift：变量与常量
来源：http://read.share.bbcook.cn/Article/details/gvuiooyjs.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gtpdgkbmm.sHtML

[T18] Swift：字符串插值
来源：http://blog.bbcook.cn/Article/details/gneixuqiy.sHtML

"值: \(b)"
来源：http://wap.fktsv.cn/Article/details/gnojgwfuq.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/gavbsjyqc.sHtML

if let n = opt { print(n) }
来源：http://www.share.tarul.cn/Article/details/gsksgsxkq.sHtML

[T20] Swift：数组操作
来源：http://www.share.yfazqb.com/Article/details/gnqnrvtgr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.yfazqb.com/Article/details/gewtpjlck.sHtML

[T21] Swift：遍历
来源：http://mobile.sjlbkw.cn/Article/details/ggviwenqi.sHtML

for x in a { print(x) }
来源：http://3g.sjlbkw.cn/Article/details/glotpvlze.sHtML

[T22] Swift：字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrroybja.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.vehdjk.com/Article/details/gireekane.sHtML

[T23] Swift：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gyumepgeg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fktsv.cn/Article/details/ggohugzma.sHtML

[T24] Swift：闭包
来源：http://baike.sjlbkw.cn/Article/details/gwbzzqabq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gzpnpugjz.sHtML

[T25] Swift：结构体
来源：http://read.share.epnwcf.com/Article/details/gnxdnhprs.sHtML

struct P { var x: Int }
来源：http://3g.epnwcf.com/Article/details/gnvgcxkup.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/gusoqrwxo.sHtML

class A: Base { override func f() {} }
来源：http://read.share.tarul.cn/Article/details/geefeffba.sHtML

[T27] Swift：错误处理
来源：http://mobile.sjlbkw.cn/Article/details/gcqiajtrh.sHtML

do { try f() } catch { print(error) }
来源：http://blog.vehdjk.com/Article/details/ggphzejbp.sHtML

[T28] Swift：枚举
来源：http://www.blog.epnwcf.com/Article/details/gqfivoedy.sHtML

enum Color { case red, green }
来源：http://m.share.epnwcf.com/Article/details/gvxmqafxn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.yfazqb.com/Article/details/golqtqaca.sHtML

guard let x = opt else { return }
来源：http://www.share.tarul.cn/Article/details/gckjxhosl.sHtML

[T30] Swift：协议
来源：http://www.blog.bbcook.cn/Article/details/gotzbjcgi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.tarul.cn/Article/details/gsklkvgeg.sHtML

[T31] Lua：Hello World
来源：http://mobile.tarul.cn/Article/details/gciwvwxcu.sHtML

print("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/ganpczdrx.sHtML

[T32] Lua：局部变量
来源：http://m.share.fktsv.cn/Article/details/gwcbivvxa.sHtML

local a = 1
来源：http://blog.epnwcf.com/Article/details/giivdaxzr.sHtML

[T33] Lua：表（数组）
来源：http://mobile.tarul.cn/Article/details/gneklkjty.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.vehdjk.com/Article/details/gkxkzipff.sHtML

[T34] Lua：遍历表
来源：http://read.share.vehdjk.com/Article/details/grjmifsqc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/gjfpzkzcs.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/gybcwmiwd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.tarul.cn/Article/details/gifwkitdc.sHtML

[T36] Lua：函数
来源：http://baike.tarul.cn/Article/details/gwkqnxxhi.sHtML

function add(a, b) return a + b end
来源：http://baike.epnwcf.com/Article/details/gufhmkvrd.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gpemqfwuq.sHtML

"a" .. "b"
来源：http://wap.epnwcf.com/Article/details/gvtrixccg.sHtML

[T38] Lua：条件
来源：http://www.m.share.epnwcf.com/Article/details/gvzmxtcvq.sHtML

if x > 0 then print("正") end
来源：http://mobile.vehdjk.com/Article/details/gicptfhtj.sHtML

[T39] Lua：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gcbjaikqd.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/gtlztycsx.sHtML

[T40] Lua：元表
来源：http://www.share.sjlbkw.cn/Article/details/gqmpmtjfo.sHtML

setmetatable({}, { __index = base })
来源：http://blog.vehdjk.com/Article/details/gnvdfbymk.sHtML

[T41] Perl：Hello World
来源：http://www.blog.yfazqb.com/Article/details/ggmlvmstr.sHtML

print "Hello\n";
来源：http://read.share.sjlbkw.cn/Article/details/gouvybpat.sHtML

[T42] Perl：变量类型
来源：http://www.share.epnwcf.com/Article/details/gsigudhet.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.sjlbkw.cn/Article/details/gypanlkpd.sHtML

[T43] Perl：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gnckjdvhd.sHtML

"值: $a"
来源：http://3g.bbcook.cn/Article/details/gpcubuigl.sHtML

[T44] Perl：条件
来源：http://3g.bbcook.cn/Article/details/gfeaxirut.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/glkmzzxcr.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.bbcook.cn/Article/details/gwephqgnt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxtktlsdf.sHtML

[T46] Perl：哈希操作
来源：http://wap.fktsv.cn/Article/details/groevdjkk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.sjlbkw.cn/Article/details/gvfbfjkux.sHtML

[T47] Perl：正则捕获
来源：http://read.share.yfazqb.com/Article/details/gtusiafvq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.epnwcf.com/Article/details/gogjfsyno.sHtML

[T48] Perl：正则替换
来源：http://3g.yfazqb.com/Article/details/gabofiilj.sHtML

$s =~ s/old/new/g;
来源：http://blog.vehdjk.com/Article/details/gelrvmnrf.sHtML

[T49] Perl：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/glefasgtq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gcsecpnps.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gbzziehhh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.sjlbkw.cn/Article/details/gftawljvf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fktsv.cn/Article/details/gackefwar.sHtML

[T51] Scala：Hello World
来源：http://blog.yfazqb.com/Article/details/ghjsimmdb.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/ggspwsjpr.sHtML

[T52] Scala：变量
来源：http://m.share.bbcook.cn/Article/details/gowsrtjqj.sHtML

val a = 1;  var b = 2
来源：http://www.blog.tarul.cn/Article/details/gghseyfck.sHtML

[T53] Scala：字符串插值
来源：http://3g.vehdjk.com/Article/details/gadvtwcoc.sHtML

s"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/ghkxqxyqd.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/gjxrvaeie.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gywmarmfn.sHtML

[T55] Scala：集合过滤
来源：http://baike.fktsv.cn/Article/details/gyitmlzhk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.bbcook.cn/Article/details/gvcgglpcr.sHtML

[T56] Scala：样例类
来源：http://www.share.epnwcf.com/Article/details/gtkjdnuae.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gggtodyrg.sHtML

[T57] Scala：模式匹配
来源：http://www.share.tarul.cn/Article/details/ggxshivbc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fktsv.cn/Article/details/gvqmivtra.sHtML

[T58] Scala：函数定义
来源：http://www.share.epnwcf.com/Article/details/gmievytqq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fktsv.cn/Article/details/guxefcyfs.sHtML

[T59] Scala：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gmeadbqbj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/gtzfytlqk.sHtML

[T60] Scala：折叠
来源：http://www.share.fktsv.cn/Article/details/gqlokgjjv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/gtjgbgzzi.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gwbqabxgf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gmkvorlab.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnsqonput.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.tarul.cn/Article/details/gdquhawgq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fktsv.cn/Article/details/gwvpvzapk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.tarul.cn/Article/details/gqxmrcagf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.bbcook.cn/Article/details/gmmywqzzr.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.epnwcf.com/Article/details/gpderdgcq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.bbcook.cn/Article/details/gnztowexq.sHtML

[U04] Py：变量调试打印
来源：http://m.share.epnwcf.com/Article/details/gqxwvzurz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.epnwcf.com/Article/details/gsetlapqi.sHtML

[U05] Py：列表去重且保序
来源：http://blog.tarul.cn/Article/details/ghcvkrhxt.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/gqmtihohy.sHtML

[U06] Py：合并两个字典
来源：http://3g.sjlbkw.cn/Article/details/getahzimw.sHtML

{**a, **b}
来源：http://www.blog.sjlbkw.cn/Article/details/gzeblzzil.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.tarul.cn/Article/details/gocutbypf.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.tarul.cn/Article/details/gfwyjbpkr.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fktsv.cn/Article/details/gpzgttrqf.sHtML

[y for x in nested for y in x]
来源：http://baike.tarul.cn/Article/details/gubvzbaqp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.yfazqb.com/Article/details/genhdwfpd.sHtML

max(d, key=d.get)
来源：http://m.share.bbcook.cn/Article/details/gxcjzgkwc.sHtML

[U10] Py：按值排序字典
来源：http://m.share.bbcook.cn/Article/details/grttuqcly.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.vehdjk.com/Article/details/gurfspjbb.sHtML

[U11] Py：生成器表达式
来源：http://blog.bbcook.cn/Article/details/groqgkwjt.sHtML

(x * 2 for x in arr)
来源：http://baike.bbcook.cn/Article/details/gwdhovcup.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.yfazqb.com/Article/details/gctjorrfk.sHtML

Counter(arr).most_common(3)
来源：http://read.share.epnwcf.com/Article/details/ghxbniptj.sHtML

[U13] Py：固定长度队列
来源：http://m.share.tarul.cn/Article/details/gpivctlzc.sHtML

deque(maxlen=10)
来源：http://3g.fktsv.cn/Article/details/ghcmfiqqk.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fktsv.cn/Article/details/gbofuwkqj.sHtML

defaultdict(list)
来源：http://read.share.vehdjk.com/Article/details/gbkfgbuoi.sHtML


<!-- 参考信息 -->