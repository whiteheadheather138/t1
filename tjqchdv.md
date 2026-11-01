代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.bbcook.cn/Article/details/gtaxhzsnf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/gijkzmwbk.sHtML

time ./run.sh
来源：http://wap.epnwcf.com/Article/details/gtoahqkho.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gwrdgqxoj.sHtML

S. C / C++ 专题
来源：http://m.share.fktsv.cn/Article/details/glxtsjbfm.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/giulkiaef.sHtML

[S01] C：Hello World
来源：http://read.share.fktsv.cn/Article/details/geroezfjb.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/gswzaqxbv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/gtgplxrqv.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.bbcook.cn/Article/details/gehjrawyf.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/gwysjbttd.sHtML

[S03] C：读入整数
来源：http://www.blog.yfazqb.com/Article/details/gqblthtkd.sHtML

int x; scanf("%d", &x);
来源：http://wap.sjlbkw.cn/Article/details/gkzolcljq.sHtML

[S04] C：字符串复制
来源：http://www.blog.epnwcf.com/Article/details/gwyioemex.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.vehdjk.com/Article/details/glmxvrzud.sHtML

[S05] C：字符串长度
来源：http://mobile.fktsv.cn/Article/details/gceoeediz.sHtML

strlen(s)
来源：http://mobile.vehdjk.com/Article/details/gvxmciisu.sHtML

[S06] C：字符串比较
来源：http://mobile.vehdjk.com/Article/details/gzpsdqohl.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gugqwovds.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/gittqxgyn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.epnwcf.com/Article/details/gnczucnpj.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/gnhrayzai.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.epnwcf.com/Article/details/ghzdbixsd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.sjlbkw.cn/Article/details/gwodvambd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fktsv.cn/Article/details/gjacbshqe.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.tarul.cn/Article/details/guocuhccn.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.tarul.cn/Article/details/gymomivpn.sHtML

[S11] C：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gzzrjfnvc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.yfazqb.com/Article/details/gtdprbyjt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.tarul.cn/Article/details/glmacphbu.sHtML

fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/gmxonwjif.sHtML

[S12] C：写文件
来源：http://www.share.yfazqb.com/Article/details/gpydsysot.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gsgfqsgwq.sHtML

[S13] C：宏定义
来源：http://read.share.fktsv.cn/Article/details/gpjzeyrzp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.vehdjk.com/Article/details/ghujivsdc.sHtML

[S14] C：枚举
来源：http://www.share.tarul.cn/Article/details/gamnikoux.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/gfdufebja.sHtML

[S15] C：类型转换
来源：http://blog.fktsv.cn/Article/details/gvsvufnre.sHtML

(double) a / b
来源：http://blog.vehdjk.com/Article/details/gujsulkha.sHtML

[S16] C：位操作置位
来源：http://wap.sjlbkw.cn/Article/details/grbfxplfy.sHtML

x |= (1 << 3);
来源：http://blog.tarul.cn/Article/details/gmoliakrl.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gitiefwtk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/gjbmbvqox.sHtML

[S18] C：命令行参数
来源：http://3g.epnwcf.com/Article/details/galaftsuw.sHtML

int main(int argc, char **argv)
来源：http://baike.fktsv.cn/Article/details/grvymcifn.sHtML

[S19] C：快速排序
来源：http://blog.sjlbkw.cn/Article/details/gclvwabtb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/gkkfrtczk.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/ghtvyapgx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gjmyokfmk.sHtML

[S21] C：字符类别判断
来源：http://wap.fktsv.cn/Article/details/gpjdivtps.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/grlizmdqo.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gbapcmfmj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.epnwcf.com/Article/details/gwgnsjqxh.sHtML

[S23] C：随机数
来源：http://www.blog.sjlbkw.cn/Article/details/gvjykxhlg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/guyogtwee.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/gohrezgtj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.epnwcf.com/Article/details/gkgkjmrnv.sHtML

[S25] C：内存拷贝
来源：http://m.share.epnwcf.com/Article/details/gakmmxdcy.sHtML

memcpy(dst, src, n);
来源：http://3g.fktsv.cn/Article/details/gquujwndo.sHtML

[S26] C：内存清零
来源：http://m.share.sjlbkw.cn/Article/details/gbtvvmdes.sHtML

memset(a, 0, sizeof a);
来源：http://3g.epnwcf.com/Article/details/gpmirmfky.sHtML

[S27] C：定义常量
来源：http://www.m.share.fktsv.cn/Article/details/gcybcmrop.sHtML

const double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gfxqaupqi.sHtML

[S28] C：静态变量
来源：http://m.share.bbcook.cn/Article/details/gnrinxydn.sHtML

static int counter = 0;
来源：http://wap.yfazqb.com/Article/details/gsbskagph.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/gkdziqxbq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fktsv.cn/Article/details/ggmjsialy.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/ghmutyilv.sHtML

#ifndef X_H
来源：http://m.share.sjlbkw.cn/Article/details/glwpbgrsi.sHtML

#define X_H
来源：http://baike.sjlbkw.cn/Article/details/gyngmipgc.sHtML

#endif
来源：http://read.share.sjlbkw.cn/Article/details/guobphhcr.sHtML

[S31] C++：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gydfiwbim.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gdysefqzs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.tarul.cn/Article/details/gxinilglv.sHtML

[S32] C++：字符串
来源：http://www.m.share.bbcook.cn/Article/details/gubuwsyey.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.tarul.cn/Article/details/ghhvvzakw.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fktsv.cn/Article/details/gmyhzqnkt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/gbmsprboh.sHtML

[S34] C++：遍历 vector
来源：http://read.share.yfazqb.com/Article/details/guyjyyyba.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.epnwcf.com/Article/details/ggziwowmc.sHtML

[S35] C++：map
来源：http://read.share.epnwcf.com/Article/details/gofcojikd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gcyssfimf.sHtML

[S36] C++：unordered_map
来源：http://3g.tarul.cn/Article/details/gunhytmik.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gllmsordy.sHtML

[S37] C++：set
来源：http://wap.tarul.cn/Article/details/grudlxgvm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.yfazqb.com/Article/details/gytepdeta.sHtML

[S38] C++：排序
来源：http://read.share.sjlbkw.cn/Article/details/gwcfwbxws.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/gnclwnoif.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.vehdjk.com/Article/details/gmjusxvra.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/gizgxizjf.sHtML

[S40] C++：查找元素
来源：http://m.share.fktsv.cn/Article/details/gqtevtcrp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.tarul.cn/Article/details/gmicbotny.sHtML

[S41] C++：类与构造函数
来源：http://baike.vehdjk.com/Article/details/gvwqtdwsf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.bbcook.cn/Article/details/gikwmmuxv.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.tarul.cn/Article/details/guzbkytog.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.bbcook.cn/Article/details/gikwdyymi.sHtML

[S43] C++：智能指针
来源：http://www.blog.fktsv.cn/Article/details/grrvgbfyj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fktsv.cn/Article/details/gurzlxmal.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/gnqrvquti.sHtML

void inc(int &x) { ++x; }
来源：http://baike.sjlbkw.cn/Article/details/gnqzfbnzx.sHtML

[S45] C++：lambda
来源：http://baike.yfazqb.com/Article/details/gtwisrvca.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.epnwcf.com/Article/details/ghvpvlatk.sHtML

[S46] C++：函数模板
来源：http://read.share.vehdjk.com/Article/details/godcwvwta.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.tarul.cn/Article/details/grannwlmc.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.bbcook.cn/Article/details/gwvrqasio.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.sjlbkw.cn/Article/details/gwcbsvuod.sHtML

[S48] C++：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gemxbsnuv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/giwfhqkwr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.vehdjk.com/Article/details/gsmkjyknk.sHtML

[S49] C++：写文件
来源：http://www.share.tarul.cn/Article/details/gfwjicwvf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.vehdjk.com/Article/details/gjhguqxkj.sHtML

[S50] C++：格式化数字
来源：http://mobile.epnwcf.com/Article/details/gniufgrcq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gqhegolnh.sHtML

[S51] C++：显式类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gatrjmnji.sHtML

static_cast<double>(a) / b
来源：http://mobile.sjlbkw.cn/Article/details/gxmmbskbp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/gnabzozsa.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/gocdhohii.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fktsv.cn/Article/details/gkdjoprlk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.yfazqb.com/Article/details/guccthiqy.sHtML

[S54] C++：异常处理
来源：http://3g.yfazqb.com/Article/details/gpdvivmsl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.vehdjk.com/Article/details/gqudjirct.sHtML

[S55] C++：结构化绑定
来源：http://wap.epnwcf.com/Article/details/gtdofysgv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/gbxrhencc.sHtML

[S56] C++：optional
来源：http://www.blog.sjlbkw.cn/Article/details/gyicneyua.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/gvybbhorp.sHtML

[S57] C++：编译期常量
来源：http://mobile.epnwcf.com/Article/details/gshergguv.sHtML

constexpr int N = 10;
来源：http://read.share.vehdjk.com/Article/details/gyheoykrd.sHtML

[S58] C++：命名空间
来源：http://mobile.vehdjk.com/Article/details/gttkdvjng.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/gdutbkvho.sHtML

[S59] C++：静态断言
来源：http://m.share.epnwcf.com/Article/details/gzgwrcuqj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.vehdjk.com/Article/details/gowdgskpb.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/gmhjzleco.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gmsfremwl.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwydhzzwk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/givduugbq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwbdqahai.sHtML

[T01] Kotlin：Hello World
来源：http://3g.epnwcf.com/Article/details/gxttfsogc.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gucoxxxik.sHtML

[T02] Kotlin：变量
来源：http://3g.sjlbkw.cn/Article/details/gspkniqsl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.epnwcf.com/Article/details/gcshmurkb.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.epnwcf.com/Article/details/gdvlgfrln.sHtML

"值: $b"
来源：http://www.share.fktsv.cn/Article/details/gwfvuiies.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/gfjapqahc.sHtML

val n: String? = null;  n?.length
来源：http://3g.vehdjk.com/Article/details/gdbtebykh.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/gxicubbfd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.tarul.cn/Article/details/gwhbzpran.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.epnwcf.com/Article/details/getuiyqdq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.vehdjk.com/Article/details/gkohzjpot.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/grtshdkeu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.vehdjk.com/Article/details/goxzrdskf.sHtML

[T08] Kotlin：数据类
来源：http://m.share.epnwcf.com/Article/details/gsdcmtjrb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gczrxnyrh.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.vehdjk.com/Article/details/gozhygxfb.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.tarul.cn/Article/details/gvlxzwzfx.sHtML

[T10] Kotlin：默认参数
来源：http://3g.epnwcf.com/Article/details/gspuearcf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.tarul.cn/Article/details/gxtmulscf.sHtML

[T11] Kotlin：协程
来源：http://blog.bbcook.cn/Article/details/glbioaadr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.sjlbkw.cn/Article/details/gjufzuezh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/gjtlgtrht.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fktsv.cn/Article/details/getvkuchn.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.tarul.cn/Article/details/gtpezdkar.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/gptsoeukv.sHtML

[T14] Kotlin：循环
来源：http://www.share.vehdjk.com/Article/details/gnyevmrxz.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/gaqgkuyid.sHtML

[T15] Kotlin：接口
来源：http://blog.epnwcf.com/Article/details/ggmajoirg.sHtML

interface Shape { fun area(): Double }
来源：http://wap.sjlbkw.cn/Article/details/gnyomweqc.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gpwgycjvp.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gpyqhwgmx.sHtML

[T17] Swift：变量与常量
来源：http://m.share.bbcook.cn/Article/details/gydopzmeh.sHtML

var a = 1;  let b = 2
来源：http://www.share.fktsv.cn/Article/details/gskikctxs.sHtML

[T18] Swift：字符串插值
来源：http://baike.yfazqb.com/Article/details/gczsvgurt.sHtML

"值: \(b)"
来源：http://read.share.fktsv.cn/Article/details/gbwouwekg.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/gxcahbasf.sHtML

if let n = opt { print(n) }
来源：http://read.share.sjlbkw.cn/Article/details/ghjareqsq.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fktsv.cn/Article/details/gjpoxvebc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.vehdjk.com/Article/details/gvjndqwor.sHtML

[T21] Swift：遍历
来源：http://www.share.bbcook.cn/Article/details/gmhnukxph.sHtML

for x in a { print(x) }
来源：http://blog.vehdjk.com/Article/details/gxirjxnkx.sHtML

[T22] Swift：字典
来源：http://baike.tarul.cn/Article/details/gsethdpep.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.tarul.cn/Article/details/ghuqdpjzn.sHtML

[T23] Swift：函数
来源：http://read.share.vehdjk.com/Article/details/gcisvartb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.epnwcf.com/Article/details/gawtgxqif.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/ginmouvmu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.bbcook.cn/Article/details/gbavocidp.sHtML

[T25] Swift：结构体
来源：http://mobile.vehdjk.com/Article/details/gbvurinbh.sHtML

struct P { var x: Int }
来源：http://read.share.vehdjk.com/Article/details/gljnpfjaf.sHtML

[T26] Swift：类与重写
来源：http://blog.bbcook.cn/Article/details/gpvsluogi.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.yfazqb.com/Article/details/gnaasleml.sHtML

[T27] Swift：错误处理
来源：http://blog.sjlbkw.cn/Article/details/gkamlfsqj.sHtML

do { try f() } catch { print(error) }
来源：http://baike.epnwcf.com/Article/details/gugukwoin.sHtML

[T28] Swift：枚举
来源：http://mobile.tarul.cn/Article/details/gxdypgtrj.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/gdekofbcs.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fktsv.cn/Article/details/gsumxnwba.sHtML

guard let x = opt else { return }
来源：http://wap.tarul.cn/Article/details/greszzckx.sHtML

[T30] Swift：协议
来源：http://mobile.fktsv.cn/Article/details/gujgsabnz.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.vehdjk.com/Article/details/gspjbaxbr.sHtML

[T31] Lua：Hello World
来源：http://wap.epnwcf.com/Article/details/giqqmdwpf.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gglvbjcey.sHtML

[T32] Lua：局部变量
来源：http://blog.yfazqb.com/Article/details/gmedxywwz.sHtML

local a = 1
来源：http://www.share.tarul.cn/Article/details/gdodfcsns.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnacjylg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.bbcook.cn/Article/details/grdaqpmts.sHtML

[T34] Lua：遍历表
来源：http://wap.tarul.cn/Article/details/gvpdtvkcy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fktsv.cn/Article/details/gkaslzoim.sHtML

[T35] Lua：字典表
来源：http://3g.tarul.cn/Article/details/grzrlvfuy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.epnwcf.com/Article/details/goutnezzt.sHtML

[T36] Lua：函数
来源：http://baike.epnwcf.com/Article/details/gqbzwnstx.sHtML

function add(a, b) return a + b end
来源：http://wap.vehdjk.com/Article/details/gsyhrwmcw.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fktsv.cn/Article/details/gkfmnghml.sHtML

"a" .. "b"
来源：http://www.blog.tarul.cn/Article/details/glfwtohqy.sHtML

[T38] Lua：条件
来源：http://blog.sjlbkw.cn/Article/details/gurxzwifh.sHtML

if x > 0 then print("正") end
来源：http://m.share.sjlbkw.cn/Article/details/gyezlsqzi.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/giqgkprkq.sHtML

string.find(s, "%d+")
来源：http://3g.tarul.cn/Article/details/gscslvytn.sHtML

[T40] Lua：元表
来源：http://www.blog.bbcook.cn/Article/details/gaztcjxso.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.yfazqb.com/Article/details/gogtokjhn.sHtML

[T41] Perl：Hello World
来源：http://baike.tarul.cn/Article/details/giwslkhbh.sHtML

print "Hello\n";
来源：http://blog.fktsv.cn/Article/details/gyxvhdlhe.sHtML

[T42] Perl：变量类型
来源：http://read.share.fktsv.cn/Article/details/gfmnjxlfk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.yfazqb.com/Article/details/ghbnpbkzg.sHtML

[T43] Perl：字符串插值
来源：http://3g.yfazqb.com/Article/details/gwxlhviwt.sHtML

"值: $a"
来源：http://mobile.sjlbkw.cn/Article/details/gzoxmfcvj.sHtML

[T44] Perl：条件
来源：http://blog.bbcook.cn/Article/details/gmenuifdi.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.tarul.cn/Article/details/gwlwhhwcc.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gkaeqvrqc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.yfazqb.com/Article/details/gytoycbah.sHtML

[T46] Perl：哈希操作
来源：http://blog.fktsv.cn/Article/details/goeiraasv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/gnhqsqwvp.sHtML

[T47] Perl：正则捕获
来源：http://read.share.epnwcf.com/Article/details/gktawuwbq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.epnwcf.com/Article/details/gfzedupdt.sHtML

[T48] Perl：正则替换
来源：http://m.share.sjlbkw.cn/Article/details/grjlmbjos.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fktsv.cn/Article/details/grysbtxsw.sHtML

[T49] Perl：函数
来源：http://read.share.fktsv.cn/Article/details/grxyoqafc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/glqgwrdfi.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gsddgtnor.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fktsv.cn/Article/details/golhvoggx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.sjlbkw.cn/Article/details/glbdnhyox.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gkyzpahck.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/ghcfyuqzv.sHtML

[T52] Scala：变量
来源：http://www.blog.fktsv.cn/Article/details/gpdxztmqt.sHtML

val a = 1;  var b = 2
来源：http://mobile.vehdjk.com/Article/details/gktdlohgs.sHtML

[T53] Scala：字符串插值
来源：http://mobile.epnwcf.com/Article/details/glxuumrad.sHtML

s"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/guuuxackt.sHtML

[T54] Scala：集合映射
来源：http://m.share.tarul.cn/Article/details/gqpjguzht.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.epnwcf.com/Article/details/guyeeaskp.sHtML

[T55] Scala：集合过滤
来源：http://3g.tarul.cn/Article/details/gpmimcaot.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.sjlbkw.cn/Article/details/gprhugcwv.sHtML

[T56] Scala：样例类
来源：http://read.share.tarul.cn/Article/details/gjotjxlbb.sHtML

case class User(name: String, age: Int)
来源：http://blog.tarul.cn/Article/details/ggrbdnjqe.sHtML

[T57] Scala：模式匹配
来源：http://www.share.yfazqb.com/Article/details/grhpmxsex.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.tarul.cn/Article/details/gcnsukhuk.sHtML

[T58] Scala：函数定义
来源：http://read.share.bbcook.cn/Article/details/gnvwtdyiu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.yfazqb.com/Article/details/gcijbfmgj.sHtML

[T59] Scala：循环
来源：http://www.m.share.vehdjk.com/Article/details/glojnijdu.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gyjsroejo.sHtML

[T60] Scala：折叠
来源：http://wap.fktsv.cn/Article/details/gzidswseh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fktsv.cn/Article/details/gliasactf.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gwbjpvtnj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/ggtxwaibg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/giuoyznch.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/ggvxthzyr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.vehdjk.com/Article/details/ghpecatpm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.yfazqb.com/Article/details/gdjkefoby.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gtyuqvloi.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.yfazqb.com/Article/details/gewkngohu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.yfazqb.com/Article/details/gmqdrpgfc.sHtML

[U04] Py：变量调试打印
来源：http://read.share.sjlbkw.cn/Article/details/gctniephd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.tarul.cn/Article/details/gkvehxwui.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.epnwcf.com/Article/details/gqimxtlef.sHtML

list(dict.fromkeys(arr))
来源：http://3g.tarul.cn/Article/details/ghmelssfp.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.vehdjk.com/Article/details/gzsyzbfnb.sHtML

{**a, **b}
来源：http://www.share.epnwcf.com/Article/details/gwomglsaa.sHtML

[U07] Py：反转字典键值
来源：http://m.share.epnwcf.com/Article/details/gxrmzqblz.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.tarul.cn/Article/details/gsgpafbpg.sHtML

[U08] Py：展平二维列表
来源：http://www.share.epnwcf.com/Article/details/gasrjocbs.sHtML

[y for x in nested for y in x]
来源：http://www.blog.tarul.cn/Article/details/gbvjdzkif.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.vehdjk.com/Article/details/gdggquajm.sHtML

max(d, key=d.get)
来源：http://blog.bbcook.cn/Article/details/golyfotfu.sHtML

[U10] Py：按值排序字典
来源：http://blog.sjlbkw.cn/Article/details/gzdildstu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.epnwcf.com/Article/details/gbejbssab.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.vehdjk.com/Article/details/gxirofidn.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.vehdjk.com/Article/details/gtcdafwti.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.vehdjk.com/Article/details/gzxcolwwp.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fktsv.cn/Article/details/gjwrcczgq.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.sjlbkw.cn/Article/details/guqpzvtcq.sHtML

deque(maxlen=10)
来源：http://m.share.yfazqb.com/Article/details/gqegbpiqb.sHtML

[U14] Py：分组收集到列表
来源：http://wap.vehdjk.com/Article/details/gajiuixaw.sHtML

defaultdict(list)
来源：http://www.share.yfazqb.com/Article/details/gubvmzmcg.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkrgajtl.sHtML

t = time.perf_counter()
来源：http://baike.sjlbkw.cn/Article/details/ghacphyey.sHtML

[U16] Py：命令行参数解析
来源：http://blog.bbcook.cn/Article/details/gdsjomece.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.sjlbkw.cn/Article/details/gousfwzym.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.vehdjk.com/Article/details/gesnhirii.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.tarul.cn/Article/details/gmhungmtu.sHtML

[U18] Py：预编译正则
来源：http://wap.fktsv.cn/Article/details/gibgjdltd.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/ggnzqcuoh.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.bbcook.cn/Article/details/ggywlnkqn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.bbcook.cn/Article/details/gvwezovwe.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/gkcdlxbex.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.tarul.cn/Article/details/gmzcwvgiv.sHtML


<!-- 参考信息 -->