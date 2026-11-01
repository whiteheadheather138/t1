代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fktsv.cn/Article/details/gotbbbnrd.sHtML

[R72] 等待端口就绪
来源：http://www.share.bbcook.cn/Article/details/gfukicpza.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/ghinpacwa.sHtML

[R73] 分割大日志
来源：http://www.m.share.bbcook.cn/Article/details/gbbtrgfgk.sHtML

split -l 1000 big.log part_
来源：http://wap.yfazqb.com/Article/details/ggzmqonsp.sHtML

[R74] 批量重命名
来源：http://www.share.bbcook.cn/Article/details/gqereuipf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.epnwcf.com/Article/details/gtqzphdvo.sHtML

[R75] 导出环境变量
来源：http://m.share.vehdjk.com/Article/details/gkxwveche.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.bbcook.cn/Article/details/gltsveany.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/gpvejopjl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gwshjcuif.sHtML

[R77] 读取用户输入
来源：http://wap.fktsv.cn/Article/details/geuaoeecw.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/guhmbgfuj.sHtML

[R78] 交互式菜单
来源：http://3g.epnwcf.com/Article/details/gruodylym.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.yfazqb.com/Article/details/gdmlwltuc.sHtML

[R79] 解析命令行选项
来源：http://read.share.fktsv.cn/Article/details/gjuizolnc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.sjlbkw.cn/Article/details/gwqzagedd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fktsv.cn/Article/details/gtvzelzne.sHtML

time ./run.sh
来源：http://3g.tarul.cn/Article/details/gtrpqiwrj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvgptvuax.sHtML

S. C / C++ 专题
来源：http://3g.fktsv.cn/Article/details/gqhrhgrbd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gfdsytjim.sHtML

[S01] C：Hello World
来源：http://read.share.yfazqb.com/Article/details/gykyczgqz.sHtML

#include <stdio.h>
来源：http://wap.tarul.cn/Article/details/gvhltnhxe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fktsv.cn/Article/details/gkforessa.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fktsv.cn/Article/details/gtoojenkq.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.tarul.cn/Article/details/gayipzawv.sHtML

[S03] C：读入整数
来源：http://www.m.share.bbcook.cn/Article/details/gcedsrsbe.sHtML

int x; scanf("%d", &x);
来源：http://wap.yfazqb.com/Article/details/gmjizzcjb.sHtML

[S04] C：字符串复制
来源：http://m.share.fktsv.cn/Article/details/gcvsqmbcb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.epnwcf.com/Article/details/gsqzqqrts.sHtML

[S05] C：字符串长度
来源：http://3g.tarul.cn/Article/details/gjkxnaroi.sHtML

strlen(s)
来源：http://www.blog.bbcook.cn/Article/details/gnivnjsxi.sHtML

[S06] C：字符串比较
来源：http://blog.yfazqb.com/Article/details/gxoxcefax.sHtML

strcmp(a, b) == 0
来源：http://www.blog.yfazqb.com/Article/details/ggoatyvyl.sHtML

[S07] C：数组遍历求和
来源：http://baike.vehdjk.com/Article/details/gxkcbgylx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.sjlbkw.cn/Article/details/gzjsjgrgv.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.bbcook.cn/Article/details/gspierwrg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.sjlbkw.cn/Article/details/grbcicqkn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/gbrmuivpo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.sjlbkw.cn/Article/details/goakvthwg.sHtML

[S10] C：指针与解引用
来源：http://read.share.sjlbkw.cn/Article/details/gyveujxlz.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/guntqneup.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gieafqhvf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.vehdjk.com/Article/details/gdgxwomju.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.epnwcf.com/Article/details/gjdufcqet.sHtML

fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gvtrjlsay.sHtML

[S12] C：写文件
来源：http://www.share.tarul.cn/Article/details/gjcxfqymc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gnlavdusn.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/gwnnoompf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.tarul.cn/Article/details/glyczsrri.sHtML

[S14] C：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gnfzpwnwu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fktsv.cn/Article/details/gzfbvxeap.sHtML

[S15] C：类型转换
来源：http://m.share.tarul.cn/Article/details/gswnajjuo.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/gwzhjeqza.sHtML

[S16] C：位操作置位
来源：http://www.blog.bbcook.cn/Article/details/gulrayzef.sHtML

x |= (1 << 3);
来源：http://www.share.yfazqb.com/Article/details/gixhdsvlg.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gggkkjzro.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/gwwjgmreu.sHtML

[S18] C：命令行参数
来源：http://read.share.vehdjk.com/Article/details/gfqnihkdl.sHtML

int main(int argc, char **argv)
来源：http://3g.bbcook.cn/Article/details/gmzhbpeuh.sHtML

[S19] C：快速排序
来源：http://baike.tarul.cn/Article/details/gntudtmec.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/ggiwqxjhz.sHtML

[S20] C：二分查找
来源：http://baike.yfazqb.com/Article/details/gcowyyuvd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/gvhjmrvpf.sHtML

[S21] C：字符类别判断
来源：http://blog.fktsv.cn/Article/details/gapnlcfhv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.sjlbkw.cn/Article/details/gktxbhukk.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gzbdspafi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/gbqsyvbiy.sHtML

[S23] C：随机数
来源：http://m.share.vehdjk.com/Article/details/gerexllln.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.tarul.cn/Article/details/gabwzixnd.sHtML

[S24] C：获取本地时间
来源：http://baike.epnwcf.com/Article/details/ghznzqoxl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/gvqzspcyd.sHtML

[S25] C：内存拷贝
来源：http://m.share.tarul.cn/Article/details/gupoprxkn.sHtML

memcpy(dst, src, n);
来源：http://mobile.tarul.cn/Article/details/gqaalvlsf.sHtML

[S26] C：内存清零
来源：http://m.share.tarul.cn/Article/details/gzezsytht.sHtML

memset(a, 0, sizeof a);
来源：http://baike.vehdjk.com/Article/details/gyrpoviyj.sHtML

[S27] C：定义常量
来源：http://baike.sjlbkw.cn/Article/details/ggfxrflna.sHtML

const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/guxeynhwr.sHtML

[S28] C：静态变量
来源：http://baike.sjlbkw.cn/Article/details/gxansftcq.sHtML

static int counter = 0;
来源：http://mobile.fktsv.cn/Article/details/gwpxypsfl.sHtML

[S29] C：变参函数
来源：http://blog.vehdjk.com/Article/details/gqlalkqvr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.yfazqb.com/Article/details/gcrzuzfek.sHtML

[S30] C：头文件保护
来源：http://3g.fktsv.cn/Article/details/grogpvzjm.sHtML

#ifndef X_H
来源：http://mobile.tarul.cn/Article/details/gaydoquag.sHtML

#define X_H
来源：http://read.share.fktsv.cn/Article/details/gwohkwvkv.sHtML

#endif
来源：http://blog.bbcook.cn/Article/details/gfwukbhaa.sHtML

[S31] C++：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gsasqrbyh.sHtML

#include <iostream>
来源：http://www.share.yfazqb.com/Article/details/gcedqxwcv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.epnwcf.com/Article/details/gdvsguwuf.sHtML

[S32] C++：字符串
来源：http://baike.sjlbkw.cn/Article/details/ggoriprdd.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/gkfyzfgoe.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gzancaxeb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.bbcook.cn/Article/details/gumddpxkr.sHtML

[S34] C++：遍历 vector
来源：http://wap.sjlbkw.cn/Article/details/gqxdysbkn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fktsv.cn/Article/details/gxznmgbdi.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/gmcysjpqa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gcvfijpor.sHtML

[S36] C++：unordered_map
来源：http://www.share.tarul.cn/Article/details/gofobkiov.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gosvlszwj.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/gyxzrxwla.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.vehdjk.com/Article/details/ggurtrrzv.sHtML

[S38] C++：排序
来源：http://baike.tarul.cn/Article/details/gtapybgsv.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/guqnkzats.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.tarul.cn/Article/details/gsknefdmo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/gvomsvsrc.sHtML

[S40] C++：查找元素
来源：http://mobile.yfazqb.com/Article/details/gdmrqpcoi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.bbcook.cn/Article/details/ghafufqvk.sHtML

[S41] C++：类与构造函数
来源：http://wap.vehdjk.com/Article/details/gdexpcokd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.vehdjk.com/Article/details/gmvgplfuz.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.bbcook.cn/Article/details/ghepabnra.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.tarul.cn/Article/details/gezwlymfi.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gsuuvtmqb.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.bbcook.cn/Article/details/gzsgcpnzj.sHtML

[S44] C++：引用传参
来源：http://www.m.share.epnwcf.com/Article/details/gvpwqdeky.sHtML

void inc(int &x) { ++x; }
来源：http://blog.tarul.cn/Article/details/gtbdborqk.sHtML

[S45] C++：lambda
来源：http://read.share.yfazqb.com/Article/details/guwhyzvrp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.epnwcf.com/Article/details/gtoxmrrhn.sHtML

[S46] C++：函数模板
来源：http://www.share.vehdjk.com/Article/details/gblnuhsof.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.bbcook.cn/Article/details/gkdcbkyqi.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.sjlbkw.cn/Article/details/geqabalwa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/gkvwlvbqq.sHtML

[S48] C++：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gyxzeksqd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.bbcook.cn/Article/details/genslzerr.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/gkpyrogte.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gnfbdbupf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.epnwcf.com/Article/details/gnjxyatbj.sHtML

[S50] C++：格式化数字
来源：http://3g.bbcook.cn/Article/details/glzfkctvu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gqjsoeycg.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gqivvxtgy.sHtML

static_cast<double>(a) / b
来源：http://www.blog.epnwcf.com/Article/details/glpshxrwe.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fktsv.cn/Article/details/ggcrcvtnk.sHtML

int size() const noexcept { return n_; }
来源：http://baike.vehdjk.com/Article/details/gzvayolfk.sHtML

[S53] C++：移动语义
来源：http://www.blog.epnwcf.com/Article/details/glrpsqcsn.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.vehdjk.com/Article/details/gvejhhfbq.sHtML

[S54] C++：异常处理
来源：http://read.share.fktsv.cn/Article/details/gwbsqblfr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.vehdjk.com/Article/details/gmfuxcmxv.sHtML

[S55] C++：结构化绑定
来源：http://blog.sjlbkw.cn/Article/details/gxnqbenol.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fktsv.cn/Article/details/gwxyljroc.sHtML

[S56] C++：optional
来源：http://read.share.sjlbkw.cn/Article/details/gqlfxsylj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.bbcook.cn/Article/details/gwkqmoksv.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/giggxakeg.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/gldupbaty.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/gafwmgkxr.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/gombszrnc.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/gjwdmghro.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.tarul.cn/Article/details/ghejcciop.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.vehdjk.com/Article/details/gbwyladoe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.vehdjk.com/Article/details/goghhxxjd.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcaqizetf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.yfazqb.com/Article/details/gnafkfwgp.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grgqsnygy.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.bbcook.cn/Article/details/gvlmowsoj.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/gziiwdyfq.sHtML

[T02] Kotlin：变量
来源：http://baike.yfazqb.com/Article/details/gmthfkcnt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.epnwcf.com/Article/details/gfjntjdff.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/ggokcwfwk.sHtML

"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gwpxysxbn.sHtML

[T04] Kotlin：空安全
来源：http://blog.vehdjk.com/Article/details/gxpviagmx.sHtML

val n: String? = null;  n?.length
来源：http://blog.epnwcf.com/Article/details/gutwvzsum.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.bbcook.cn/Article/details/gkqncawqx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.tarul.cn/Article/details/gahtrstjo.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gtneztoyc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/giaxepjjf.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/gupdhgljh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.epnwcf.com/Article/details/gaxoovwem.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fktsv.cn/Article/details/gjuoxstfq.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.bbcook.cn/Article/details/gdlrjvzlf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fktsv.cn/Article/details/gmwcmjhbq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.vehdjk.com/Article/details/guokvrvic.sHtML

[T10] Kotlin：默认参数
来源：http://3g.epnwcf.com/Article/details/gzqydxyye.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.bbcook.cn/Article/details/gdxafdkaj.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gynsyolfz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.tarul.cn/Article/details/gnttzmsvn.sHtML

[T12] Kotlin：解构声明
来源：http://wap.bbcook.cn/Article/details/gcmovwvop.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.tarul.cn/Article/details/gmixvpthe.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gbecmimqw.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.yfazqb.com/Article/details/gvepbewaa.sHtML

[T14] Kotlin：循环
来源：http://wap.vehdjk.com/Article/details/gcdogzoer.sHtML

for (i in 1..10) println(i)
来源：http://baike.bbcook.cn/Article/details/gnhpuecju.sHtML

[T15] Kotlin：接口
来源：http://blog.tarul.cn/Article/details/grwayjyim.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/gbdnkosxx.sHtML

[T16] Swift：Hello World
来源：http://blog.epnwcf.com/Article/details/gahlzzzgu.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/grgfwunnn.sHtML

[T17] Swift：变量与常量
来源：http://blog.bbcook.cn/Article/details/gqsxeexdw.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fktsv.cn/Article/details/gdlmfdkli.sHtML

[T18] Swift：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gvwvrxxzc.sHtML

"值: \(b)"
来源：http://read.share.vehdjk.com/Article/details/gdmjffiue.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/gmbzjtcnh.sHtML

if let n = opt { print(n) }
来源：http://m.share.fktsv.cn/Article/details/gfwsclubv.sHtML

[T20] Swift：数组操作
来源：http://wap.yfazqb.com/Article/details/gmlfuusfo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fktsv.cn/Article/details/gvctvovcf.sHtML

[T21] Swift：遍历
来源：http://blog.vehdjk.com/Article/details/gvdwkeyxy.sHtML

for x in a { print(x) }
来源：http://blog.yfazqb.com/Article/details/gcjynbgqq.sHtML

[T22] Swift：字典
来源：http://mobile.vehdjk.com/Article/details/gtqaouzim.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.tarul.cn/Article/details/gxjpwofeg.sHtML

[T23] Swift：函数
来源：http://3g.epnwcf.com/Article/details/gwvenrmbw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.tarul.cn/Article/details/gyxtpnfpv.sHtML

[T24] Swift：闭包
来源：http://mobile.bbcook.cn/Article/details/ghksogvup.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gkxkbsqvf.sHtML

[T25] Swift：结构体
来源：http://baike.vehdjk.com/Article/details/gktympnhe.sHtML

struct P { var x: Int }
来源：http://read.share.yfazqb.com/Article/details/grpbydfxv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.epnwcf.com/Article/details/gpipdwkig.sHtML

class A: Base { override func f() {} }
来源：http://mobile.epnwcf.com/Article/details/gicsdnecc.sHtML

[T27] Swift：错误处理
来源：http://3g.sjlbkw.cn/Article/details/gnzviutqw.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.yfazqb.com/Article/details/gktwgjllz.sHtML

[T28] Swift：枚举
来源：http://read.share.epnwcf.com/Article/details/gkconpnci.sHtML

enum Color { case red, green }
来源：http://www.m.share.yfazqb.com/Article/details/grbmohbcb.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.epnwcf.com/Article/details/gihaktggy.sHtML

guard let x = opt else { return }
来源：http://read.share.fktsv.cn/Article/details/ggszrmlpk.sHtML

[T30] Swift：协议
来源：http://3g.epnwcf.com/Article/details/gspjukvlq.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.tarul.cn/Article/details/ghvufdybe.sHtML

[T31] Lua：Hello World
来源：http://baike.tarul.cn/Article/details/gizdqhzxr.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/gorngpswt.sHtML

[T32] Lua：局部变量
来源：http://www.share.bbcook.cn/Article/details/goffhncwm.sHtML

local a = 1
来源：http://baike.fktsv.cn/Article/details/gzkaemmdb.sHtML

[T33] Lua：表（数组）
来源：http://blog.sjlbkw.cn/Article/details/galfbndtg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.tarul.cn/Article/details/gptseermy.sHtML

[T34] Lua：遍历表
来源：http://3g.sjlbkw.cn/Article/details/gtlzyecxb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fktsv.cn/Article/details/gqghobioz.sHtML

[T35] Lua：字典表
来源：http://3g.sjlbkw.cn/Article/details/gnhmopywp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.yfazqb.com/Article/details/gtimkthet.sHtML

[T36] Lua：函数
来源：http://m.share.epnwcf.com/Article/details/ghxubcwcb.sHtML

function add(a, b) return a + b end
来源：http://m.share.sjlbkw.cn/Article/details/gnkwuguny.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.yfazqb.com/Article/details/geoaygpjk.sHtML

"a" .. "b"
来源：http://blog.fktsv.cn/Article/details/gmnfxxvzg.sHtML

[T38] Lua：条件
来源：http://read.share.vehdjk.com/Article/details/gflekuhps.sHtML

if x > 0 then print("正") end
来源：http://baike.tarul.cn/Article/details/gprvaopdx.sHtML

[T39] Lua：模式匹配
来源：http://wap.epnwcf.com/Article/details/gnchdexmh.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/gzhswecar.sHtML

[T40] Lua：元表
来源：http://3g.tarul.cn/Article/details/gnxvhdeov.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.yfazqb.com/Article/details/gexncjwrn.sHtML

[T41] Perl：Hello World
来源：http://wap.vehdjk.com/Article/details/gzolqopcj.sHtML

print "Hello\n";
来源：http://m.share.vehdjk.com/Article/details/gnxsyunel.sHtML

[T42] Perl：变量类型
来源：http://www.share.tarul.cn/Article/details/grkybyotb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.yfazqb.com/Article/details/gzwloaxpx.sHtML

[T43] Perl：字符串插值
来源：http://www.share.vehdjk.com/Article/details/golhmcmhv.sHtML

"值: $a"
来源：http://wap.epnwcf.com/Article/details/gnwrkzzua.sHtML

[T44] Perl：条件
来源：http://www.m.share.fktsv.cn/Article/details/gqclvtyzc.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.epnwcf.com/Article/details/gkomwxexd.sHtML

[T45] Perl：数组遍历
来源：http://www.share.bbcook.cn/Article/details/ghyjbrfku.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.bbcook.cn/Article/details/gjqrcewqu.sHtML

[T46] Perl：哈希操作
来源：http://www.share.vehdjk.com/Article/details/ghkaeoggo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.tarul.cn/Article/details/gihyotgfx.sHtML

[T47] Perl：正则捕获
来源：http://read.share.epnwcf.com/Article/details/gzyxhykso.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.tarul.cn/Article/details/gmunibrjt.sHtML

[T48] Perl：正则替换
来源：http://m.share.epnwcf.com/Article/details/ghgsmuwuq.sHtML

$s =~ s/old/new/g;
来源：http://3g.bbcook.cn/Article/details/gfqgwblvk.sHtML

[T49] Perl：函数
来源：http://read.share.vehdjk.com/Article/details/gsrgpphva.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gvtygiimc.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gpiviqfze.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.sjlbkw.cn/Article/details/gntyfoczl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.bbcook.cn/Article/details/gwysplhpm.sHtML

[T51] Scala：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gbwovjnoo.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/grcxqcqve.sHtML

[T52] Scala：变量
来源：http://www.m.share.epnwcf.com/Article/details/gtppkrwcx.sHtML

val a = 1;  var b = 2
来源：http://www.share.vehdjk.com/Article/details/gmvtslsus.sHtML

[T53] Scala：字符串插值
来源：http://blog.epnwcf.com/Article/details/grfilmykg.sHtML

s"值: $b"
来源：http://mobile.tarul.cn/Article/details/gcpzsamqe.sHtML

[T54] Scala：集合映射
来源：http://blog.tarul.cn/Article/details/gpwowcpag.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.vehdjk.com/Article/details/gqfrqwzql.sHtML

[T55] Scala：集合过滤
来源：http://read.share.tarul.cn/Article/details/gnaqhjkyj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.tarul.cn/Article/details/geqiumczs.sHtML

[T56] Scala：样例类
来源：http://blog.fktsv.cn/Article/details/gtpokzvlk.sHtML

case class User(name: String, age: Int)
来源：http://baike.bbcook.cn/Article/details/gmgnwqkzt.sHtML

[T57] Scala：模式匹配
来源：http://wap.epnwcf.com/Article/details/grjdybhqe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.yfazqb.com/Article/details/gcvtpdjki.sHtML

[T58] Scala：函数定义
来源：http://www.blog.tarul.cn/Article/details/gvviehtns.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/gnmfjlhus.sHtML

[T59] Scala：循环
来源：http://m.share.bbcook.cn/Article/details/gaafhdlfq.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.yfazqb.com/Article/details/gvdblsjxk.sHtML

[T60] Scala：折叠
来源：http://www.m.share.tarul.cn/Article/details/gqfpzeyon.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.yfazqb.com/Article/details/gnccurvjd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/grwtiumlq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gfnyussgx.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/grywagzys.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.bbcook.cn/Article/details/gemsgbnkx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.yfazqb.com/Article/details/gmjavlfnz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.sjlbkw.cn/Article/details/gcliihqzg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.vehdjk.com/Article/details/gmvnkwrdh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.vehdjk.com/Article/details/gpxhipezg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.yfazqb.com/Article/details/ggslfdqmf.sHtML

[U04] Py：变量调试打印
来源：http://baike.bbcook.cn/Article/details/gbqogughx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/gdvqtwdlq.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fktsv.cn/Article/details/gkgoovric.sHtML

list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/guphmjuqx.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.bbcook.cn/Article/details/gminnsgly.sHtML

{**a, **b}
来源：http://baike.sjlbkw.cn/Article/details/gtykzesfm.sHtML

[U07] Py：反转字典键值
来源：http://wap.bbcook.cn/Article/details/gagssrqge.sHtML

{v: k for k, v in d.items()}
来源：http://baike.sjlbkw.cn/Article/details/gczlijeiy.sHtML

[U08] Py：展平二维列表
来源：http://read.share.sjlbkw.cn/Article/details/gzcprqhof.sHtML

[y for x in nested for y in x]
来源：http://read.share.tarul.cn/Article/details/gmylcpdjy.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.sjlbkw.cn/Article/details/gdnqtkbxl.sHtML

max(d, key=d.get)
来源：http://www.share.tarul.cn/Article/details/gwamszaef.sHtML

[U10] Py：按值排序字典
来源：http://blog.sjlbkw.cn/Article/details/gskxlnvyp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.sjlbkw.cn/Article/details/gardyhipw.sHtML

[U11] Py：生成器表达式
来源：http://blog.yfazqb.com/Article/details/geqgjkynj.sHtML

(x * 2 for x in arr)
来源：http://www.blog.tarul.cn/Article/details/gxnsapmas.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.epnwcf.com/Article/details/gzcjsttkz.sHtML

Counter(arr).most_common(3)
来源：http://m.share.yfazqb.com/Article/details/gbfjuhpfw.sHtML


<!-- 参考信息 -->