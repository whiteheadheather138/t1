代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.tarul.cn/Article/details/gmqbuhegd.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.bbcook.cn/Article/details/gmzqudnlz.sHtML

time ./run.sh
来源：http://read.share.yfazqb.com/Article/details/gexcqpgky.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gaqtbtygi.sHtML

S. C / C++ 专题
来源：http://blog.tarul.cn/Article/details/gbghicpxv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glqadkwre.sHtML

[S01] C：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gpgnktdmn.sHtML

#include <stdio.h>
来源：http://3g.bbcook.cn/Article/details/gosvcqlay.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.tarul.cn/Article/details/gorycanza.sHtML

[S02] C：变量与格式化输出
来源：http://3g.epnwcf.com/Article/details/gdzypzens.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.epnwcf.com/Article/details/gtyownwnw.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/guzuwyzgl.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/gvotslnlg.sHtML

[S04] C：字符串复制
来源：http://www.blog.tarul.cn/Article/details/gfvwpdrqb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gunxkpmof.sHtML

[S05] C：字符串长度
来源：http://3g.yfazqb.com/Article/details/gozvmvcvk.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/gnitfjsug.sHtML

[S06] C：字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gfritqqnr.sHtML

strcmp(a, b) == 0
来源：http://mobile.tarul.cn/Article/details/gkgoojwsn.sHtML

[S07] C：数组遍历求和
来源：http://read.share.bbcook.cn/Article/details/gacnwoyld.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.bbcook.cn/Article/details/gwbwavklt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.tarul.cn/Article/details/gtocvjxtg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.vehdjk.com/Article/details/gsrwxghuj.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.bbcook.cn/Article/details/grspaiabg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fktsv.cn/Article/details/gmkrqdkck.sHtML

[S10] C：指针与解引用
来源：http://blog.tarul.cn/Article/details/ggedjquaf.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.yfazqb.com/Article/details/gatchyjts.sHtML

[S11] C：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gtijevozy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.bbcook.cn/Article/details/gaplpyuis.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fktsv.cn/Article/details/ggkdzhxks.sHtML

fclose(f);
来源：http://blog.yfazqb.com/Article/details/gjlypiuxg.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/gftkdbpvq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gwhcjfjbd.sHtML

[S13] C：宏定义
来源：http://3g.tarul.cn/Article/details/gxpfsgojg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fktsv.cn/Article/details/gnyirdgrk.sHtML

[S14] C：枚举
来源：http://mobile.epnwcf.com/Article/details/gkshpzvay.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/grkfhiyrm.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/ggwkbhoew.sHtML

(double) a / b
来源：http://read.share.bbcook.cn/Article/details/glczvutte.sHtML

[S16] C：位操作置位
来源：http://baike.bbcook.cn/Article/details/gmgnluafq.sHtML

x |= (1 << 3);
来源：http://3g.fktsv.cn/Article/details/gvuorrqgl.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/goqfzormt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.vehdjk.com/Article/details/gliwyixlj.sHtML

[S18] C：命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/glhzrnvhg.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gpcgpuxxx.sHtML

[S19] C：快速排序
来源：http://www.blog.sjlbkw.cn/Article/details/gfyfimypf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gackkbqbq.sHtML

[S20] C：二分查找
来源：http://www.share.vehdjk.com/Article/details/gbchajhsi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gwampsntd.sHtML

[S21] C：字符类别判断
来源：http://wap.fktsv.cn/Article/details/gcmzedzqm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.sjlbkw.cn/Article/details/gltdgdcaa.sHtML

[S22] C：字符串转数字
来源：http://mobile.epnwcf.com/Article/details/gkzwbvsup.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.bbcook.cn/Article/details/gkftrowyb.sHtML

[S23] C：随机数
来源：http://www.blog.vehdjk.com/Article/details/ggwicfcux.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.tarul.cn/Article/details/gqkydtqna.sHtML

[S24] C：获取本地时间
来源：http://read.share.sjlbkw.cn/Article/details/gxdtajxit.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.epnwcf.com/Article/details/gzkikblun.sHtML

[S25] C：内存拷贝
来源：http://www.blog.epnwcf.com/Article/details/gpyvxwmja.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gunkywpxp.sHtML

[S26] C：内存清零
来源：http://3g.epnwcf.com/Article/details/gdzubwyhx.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/gfwjmvdms.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/gdqtjixug.sHtML

const double PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gvsdyfycz.sHtML

[S28] C：静态变量
来源：http://mobile.yfazqb.com/Article/details/goktjnwfb.sHtML

static int counter = 0;
来源：http://m.share.sjlbkw.cn/Article/details/gsrwnwyxn.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/galraykxd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.yfazqb.com/Article/details/ggqlergrd.sHtML

[S30] C：头文件保护
来源：http://www.share.epnwcf.com/Article/details/gdowqxanz.sHtML

#ifndef X_H
来源：http://wap.sjlbkw.cn/Article/details/gcfjqijrx.sHtML

#define X_H
来源：http://www.share.tarul.cn/Article/details/gpslihrkq.sHtML

#endif
来源：http://m.share.epnwcf.com/Article/details/gkwvedtkg.sHtML

[S31] C++：Hello World
来源：http://read.share.yfazqb.com/Article/details/gpuybrzio.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/gjqwfilsz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fktsv.cn/Article/details/gutuyxdna.sHtML

[S32] C++：字符串
来源：http://blog.fktsv.cn/Article/details/gbmohxhmg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbvnbwkm.sHtML

[S33] C++：vector 增删
来源：http://mobile.vehdjk.com/Article/details/gyfmonmow.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fktsv.cn/Article/details/gqxcvzvtd.sHtML

[S34] C++：遍历 vector
来源：http://wap.epnwcf.com/Article/details/gknkbnleo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.epnwcf.com/Article/details/gohmviznd.sHtML

[S35] C++：map
来源：http://wap.epnwcf.com/Article/details/gnvsgxiqj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gzjlgfoua.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gvtnkbztm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/guwvvawas.sHtML

[S37] C++：set
来源：http://baike.sjlbkw.cn/Article/details/ggpofavik.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.vehdjk.com/Article/details/gddlakyrg.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/ghftkhaxs.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gmbrkunvx.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fktsv.cn/Article/details/gmfelwivj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.tarul.cn/Article/details/gfahwkbew.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/ghcwftdyh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.tarul.cn/Article/details/gljikllft.sHtML

[S41] C++：类与构造函数
来源：http://m.share.yfazqb.com/Article/details/gpbeqxybp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.epnwcf.com/Article/details/grsgognlk.sHtML

[S42] C++：继承与虚函数
来源：http://3g.tarul.cn/Article/details/gmyafolli.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/gkagdjnou.sHtML

[S43] C++：智能指针
来源：http://read.share.epnwcf.com/Article/details/gktxfchpa.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/goidzcjkf.sHtML

[S44] C++：引用传参
来源：http://m.share.tarul.cn/Article/details/gqdyppekp.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.bbcook.cn/Article/details/gdlegbkwk.sHtML

[S45] C++：lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/glnowiaiv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/gaensvrtm.sHtML

[S46] C++：函数模板
来源：http://baike.sjlbkw.cn/Article/details/gtectprce.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.epnwcf.com/Article/details/gqtmbazvt.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.yfazqb.com/Article/details/gvpkryyru.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.yfazqb.com/Article/details/gztaifqed.sHtML

[S48] C++：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/glftcodpm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.bbcook.cn/Article/details/gqkjiaedn.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fktsv.cn/Article/details/gpcevekwq.sHtML

[S49] C++：写文件
来源：http://www.blog.vehdjk.com/Article/details/gmdolukou.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.yfazqb.com/Article/details/gsxundvmx.sHtML

[S50] C++：格式化数字
来源：http://www.share.vehdjk.com/Article/details/gyuornbsh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.vehdjk.com/Article/details/gjlocvsep.sHtML

[S51] C++：显式类型转换
来源：http://read.share.epnwcf.com/Article/details/gniyadija.sHtML

static_cast<double>(a) / b
来源：http://wap.sjlbkw.cn/Article/details/gvlabxjqj.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.epnwcf.com/Article/details/gictrwpno.sHtML

int size() const noexcept { return n_; }
来源：http://3g.yfazqb.com/Article/details/gojqiiyer.sHtML

[S53] C++：移动语义
来源：http://baike.vehdjk.com/Article/details/gwjlrxsqt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.epnwcf.com/Article/details/guhnetcok.sHtML

[S54] C++：异常处理
来源：http://www.m.share.yfazqb.com/Article/details/ggchhxinw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.epnwcf.com/Article/details/gnyhkbazc.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfxogfua.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.bbcook.cn/Article/details/gjnmratmo.sHtML

[S56] C++：optional
来源：http://read.share.yfazqb.com/Article/details/goaoltifq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.tarul.cn/Article/details/gaedykvrv.sHtML

[S57] C++：编译期常量
来源：http://www.share.epnwcf.com/Article/details/gulxmqhgv.sHtML

constexpr int N = 10;
来源：http://wap.fktsv.cn/Article/details/gjqitturh.sHtML

[S58] C++：命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gwqahbeuy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/gzzqphjxq.sHtML

[S59] C++：静态断言
来源：http://blog.bbcook.cn/Article/details/gsyhyngyy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.bbcook.cn/Article/details/glyjydwgo.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.epnwcf.com/Article/details/glwsmsovx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/ggyjqgkvh.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gwwwbvkzi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/ggcrwwcvq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqlaaxwax.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.vehdjk.com/Article/details/gqgumrmte.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/guxadnbxt.sHtML

[T02] Kotlin：变量
来源：http://m.share.bbcook.cn/Article/details/gekuruqud.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.sjlbkw.cn/Article/details/greccaqml.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.epnwcf.com/Article/details/gteoipmqr.sHtML

"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/gbcimwpnr.sHtML

[T04] Kotlin：空安全
来源：http://m.share.bbcook.cn/Article/details/gxciwastn.sHtML

val n: String? = null;  n?.length
来源：http://mobile.epnwcf.com/Article/details/gksroiozx.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.yfazqb.com/Article/details/grgrevzsq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.bbcook.cn/Article/details/gscsdxjkk.sHtML

[T06] Kotlin：集合映射
来源：http://blog.vehdjk.com/Article/details/gsibycqpm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.bbcook.cn/Article/details/gwnwvsjsm.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.tarul.cn/Article/details/gdudwtquy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.bbcook.cn/Article/details/gqoaewzxq.sHtML

[T08] Kotlin：数据类
来源：http://wap.bbcook.cn/Article/details/gpncsjmdd.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.bbcook.cn/Article/details/gcvdsrfhn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.tarul.cn/Article/details/gryqwtezb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/gcgyokojb.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.yfazqb.com/Article/details/gyafovjnk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/gkzbqrjyz.sHtML

[T11] Kotlin：协程
来源：http://blog.vehdjk.com/Article/details/geqzmajax.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.tarul.cn/Article/details/gzichjmuj.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.sjlbkw.cn/Article/details/getindkbr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gzggfxtel.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/ggeutmsec.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/ghcceuvbs.sHtML

[T14] Kotlin：循环
来源：http://read.share.yfazqb.com/Article/details/gawrfmbsj.sHtML

for (i in 1..10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/ghxkdlmfq.sHtML

[T15] Kotlin：接口
来源：http://www.blog.vehdjk.com/Article/details/gzaqcnklp.sHtML

interface Shape { fun area(): Double }
来源：http://blog.tarul.cn/Article/details/gouqdyqvr.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/gpzuzjecj.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gcgswykiu.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fktsv.cn/Article/details/gqlautikb.sHtML

var a = 1;  let b = 2
来源：http://baike.vehdjk.com/Article/details/gxdwzycwu.sHtML

[T18] Swift：字符串插值
来源：http://3g.bbcook.cn/Article/details/gvtqkiqwz.sHtML

"值: \(b)"
来源：http://3g.epnwcf.com/Article/details/ggobcaapg.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/gkmrcczil.sHtML

if let n = opt { print(n) }
来源：http://3g.yfazqb.com/Article/details/gvofiscnd.sHtML

[T20] Swift：数组操作
来源：http://blog.epnwcf.com/Article/details/gcbkcxjmp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/godkrczit.sHtML

[T21] Swift：遍历
来源：http://www.share.vehdjk.com/Article/details/gwaglicep.sHtML

for x in a { print(x) }
来源：http://3g.sjlbkw.cn/Article/details/gqucxbkhi.sHtML

[T22] Swift：字典
来源：http://m.share.sjlbkw.cn/Article/details/gmctkuwcq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.sjlbkw.cn/Article/details/grbxlefeg.sHtML

[T23] Swift：函数
来源：http://www.blog.yfazqb.com/Article/details/gjvtyvkew.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.epnwcf.com/Article/details/grbknssge.sHtML

[T24] Swift：闭包
来源：http://read.share.bbcook.cn/Article/details/gkfzrtjjf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.tarul.cn/Article/details/gcmacpkag.sHtML

[T25] Swift：结构体
来源：http://blog.tarul.cn/Article/details/gmgausqnw.sHtML

struct P { var x: Int }
来源：http://www.blog.fktsv.cn/Article/details/gzzzigyws.sHtML

[T26] Swift：类与重写
来源：http://blog.epnwcf.com/Article/details/gvifhetam.sHtML

class A: Base { override func f() {} }
来源：http://wap.fktsv.cn/Article/details/gqnguaunn.sHtML

[T27] Swift：错误处理
来源：http://www.blog.epnwcf.com/Article/details/gqijxmpnw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.sjlbkw.cn/Article/details/grqhrqgrf.sHtML

[T28] Swift：枚举
来源：http://www.share.vehdjk.com/Article/details/grprbucti.sHtML

enum Color { case red, green }
来源：http://3g.yfazqb.com/Article/details/guviavbax.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fktsv.cn/Article/details/guxmtuojv.sHtML

guard let x = opt else { return }
来源：http://read.share.yfazqb.com/Article/details/gsxtdqcmz.sHtML

[T30] Swift：协议
来源：http://mobile.sjlbkw.cn/Article/details/gmjgozoms.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.vehdjk.com/Article/details/glltvlmav.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/ggpjzadcg.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/guxqnfiqv.sHtML

[T32] Lua：局部变量
来源：http://www.blog.yfazqb.com/Article/details/gpdhgffau.sHtML

local a = 1
来源：http://mobile.epnwcf.com/Article/details/gdjwmewde.sHtML

[T33] Lua：表（数组）
来源：http://3g.epnwcf.com/Article/details/galkvtybr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.bbcook.cn/Article/details/gltztlubf.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.tarul.cn/Article/details/gdaxxtogv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.yfazqb.com/Article/details/gvgoirgja.sHtML

[T35] Lua：字典表
来源：http://www.m.share.yfazqb.com/Article/details/gudtzrmhz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.bbcook.cn/Article/details/gudwfjpiu.sHtML

[T36] Lua：函数
来源：http://read.share.sjlbkw.cn/Article/details/gzbiodcsi.sHtML

function add(a, b) return a + b end
来源：http://m.share.epnwcf.com/Article/details/gjopldoxx.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fktsv.cn/Article/details/ggjwwmgzi.sHtML

"a" .. "b"
来源：http://blog.fktsv.cn/Article/details/gzjerogpb.sHtML

[T38] Lua：条件
来源：http://read.share.tarul.cn/Article/details/gqygqwnun.sHtML

if x > 0 then print("正") end
来源：http://3g.bbcook.cn/Article/details/gheywupaq.sHtML

[T39] Lua：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gbhxmoann.sHtML

string.find(s, "%d+")
来源：http://m.share.epnwcf.com/Article/details/gdkpndgba.sHtML

[T40] Lua：元表
来源：http://blog.yfazqb.com/Article/details/gfidyxtly.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fktsv.cn/Article/details/gwgelbqjo.sHtML

[T41] Perl：Hello World
来源：http://blog.fktsv.cn/Article/details/gnfuflqbl.sHtML

print "Hello\n";
来源：http://www.blog.fktsv.cn/Article/details/gckjthgcb.sHtML

[T42] Perl：变量类型
来源：http://3g.fktsv.cn/Article/details/gkigdxgqo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.bbcook.cn/Article/details/gxvjeqwlk.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gsmbgubzf.sHtML

"值: $a"
来源：http://m.share.tarul.cn/Article/details/gyuypnmnr.sHtML

[T44] Perl：条件
来源：http://mobile.vehdjk.com/Article/details/gpejwkudl.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fktsv.cn/Article/details/ghybkjegd.sHtML

[T45] Perl：数组遍历
来源：http://read.share.tarul.cn/Article/details/ggxqujlmj.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.vehdjk.com/Article/details/gxlxmrnvk.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gjerkaqqm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fktsv.cn/Article/details/gktwsbspy.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.tarul.cn/Article/details/gpjshkehj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.epnwcf.com/Article/details/grpfsdwgo.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/goqihsxes.sHtML

$s =~ s/old/new/g;
来源：http://www.share.yfazqb.com/Article/details/ghhekfjep.sHtML

[T49] Perl：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gulrzafav.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gauwbhqrf.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/grnnkaowy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fktsv.cn/Article/details/gboqvtrqw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fktsv.cn/Article/details/gdfrpxohg.sHtML

[T51] Scala：Hello World
来源：http://mobile.vehdjk.com/Article/details/glgovfhbt.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gmxupobfm.sHtML

[T52] Scala：变量
来源：http://read.share.vehdjk.com/Article/details/ghheotvux.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhohnweo.sHtML

[T53] Scala：字符串插值
来源：http://3g.vehdjk.com/Article/details/gsbexuriw.sHtML

s"值: $b"
来源：http://3g.fktsv.cn/Article/details/gpenduwdn.sHtML

[T54] Scala：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gydeczcyf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.yfazqb.com/Article/details/gbnhhjpai.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gybludtez.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.yfazqb.com/Article/details/goaawiicq.sHtML

[T56] Scala：样例类
来源：http://baike.epnwcf.com/Article/details/gevaafujp.sHtML

case class User(name: String, age: Int)
来源：http://wap.sjlbkw.cn/Article/details/gxgcdrhos.sHtML

[T57] Scala：模式匹配
来源：http://3g.fktsv.cn/Article/details/gxcbhvsey.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gjarkulxr.sHtML

[T58] Scala：函数定义
来源：http://read.share.fktsv.cn/Article/details/gdqfbtdgm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.vehdjk.com/Article/details/grwayggnq.sHtML

[T59] Scala：循环
来源：http://read.share.bbcook.cn/Article/details/gsukouahn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gmwcjgflf.sHtML

[T60] Scala：折叠
来源：http://blog.bbcook.cn/Article/details/gxmcpvhcq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/gegladwfr.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxeinlgul.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/gnvujswtt.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gybcxizgd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.sjlbkw.cn/Article/details/gkjaevkay.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/gbnjqoggw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.vehdjk.com/Article/details/gbggsmdiv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fktsv.cn/Article/details/gjgtcelub.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.tarul.cn/Article/details/gzsoulhms.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.bbcook.cn/Article/details/gkjdnuaae.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.vehdjk.com/Article/details/gvfbdttdu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/gugbwqavs.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.bbcook.cn/Article/details/gvmnuttzx.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fktsv.cn/Article/details/gadaldesd.sHtML

[U06] Py：合并两个字典
来源：http://read.share.sjlbkw.cn/Article/details/gydbmrkbv.sHtML

{**a, **b}
来源：http://baike.epnwcf.com/Article/details/gmjtowyuj.sHtML

[U07] Py：反转字典键值
来源：http://wap.epnwcf.com/Article/details/gpihhorxl.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.epnwcf.com/Article/details/gcaxqglsk.sHtML

[U08] Py：展平二维列表
来源：http://wap.yfazqb.com/Article/details/gxuwpfjdd.sHtML

[y for x in nested for y in x]
来源：http://www.share.vehdjk.com/Article/details/gqunqjglu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.yfazqb.com/Article/details/gbrescsxs.sHtML

max(d, key=d.get)
来源：http://www.share.vehdjk.com/Article/details/gdkgonthu.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/gkmpnbjaj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.tarul.cn/Article/details/gmpyukpuu.sHtML

[U11] Py：生成器表达式
来源：http://wap.epnwcf.com/Article/details/gaaokawxp.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.epnwcf.com/Article/details/glitcvqve.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fktsv.cn/Article/details/gcvkjqaud.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/gxmnvyejn.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fktsv.cn/Article/details/ghfvibaav.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/gegrwzlfs.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fktsv.cn/Article/details/gcwiczpzr.sHtML

defaultdict(list)
来源：http://blog.vehdjk.com/Article/details/gkbaenvwr.sHtML

[U15] Py：高精度计时
来源：http://blog.vehdjk.com/Article/details/gkujuckrm.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/grtdfzvwi.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.bbcook.cn/Article/details/gzzfdhcjh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.yfazqb.com/Article/details/grxdgbnxz.sHtML

[U17] Py：初始化日志
来源：http://mobile.sjlbkw.cn/Article/details/gkjyngehi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.tarul.cn/Article/details/gqhzdslcp.sHtML

[U18] Py：预编译正则
来源：http://mobile.fktsv.cn/Article/details/gpvqdtljf.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.tarul.cn/Article/details/ghndqpwtr.sHtML

[U19] Py：正则替换带回调
来源：http://wap.bbcook.cn/Article/details/goqxygkpy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.bbcook.cn/Article/details/gxloynxfr.sHtML

[U20] Py：缓存函数结果
来源：http://blog.yfazqb.com/Article/details/gcvzhkzqi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.tarul.cn/Article/details/gstrzpewf.sHtML


<!-- 参考信息 -->