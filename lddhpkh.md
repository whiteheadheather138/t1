代发 wailian999

split -l 1000 big.log part_
来源：http://www.blog.fktsv.cn/Article/details/grcxhldbc.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/ghveyykwy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.bbcook.cn/Article/details/gnxtlpejs.sHtML

[R75] 导出环境变量
来源：http://wap.fktsv.cn/Article/details/gghewudep.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/gutfdfvxq.sHtML

[R76] 使用临时文件
来源：http://read.share.epnwcf.com/Article/details/gfixfrhcd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gizqqurkp.sHtML

[R77] 读取用户输入
来源：http://www.m.share.epnwcf.com/Article/details/gxugfowqw.sHtML

read -rp "请输入: " ans
来源：http://www.share.sjlbkw.cn/Article/details/gtdlbymbb.sHtML

[R78] 交互式菜单
来源：http://www.share.tarul.cn/Article/details/ggaqrkrck.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.vehdjk.com/Article/details/gmmdaofae.sHtML

[R79] 解析命令行选项
来源：http://wap.vehdjk.com/Article/details/gxvdacmes.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.bbcook.cn/Article/details/gtgmypxnn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.sjlbkw.cn/Article/details/gugjdsanx.sHtML

time ./run.sh
来源：http://www.blog.sjlbkw.cn/Article/details/gfocvuzqq.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfaaoypul.sHtML

S. C / C++ 专题
来源：http://mobile.epnwcf.com/Article/details/gynrowjgh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gydphwzih.sHtML

[S01] C：Hello World
来源：http://3g.vehdjk.com/Article/details/gdspzdiej.sHtML

#include <stdio.h>
来源：http://www.blog.vehdjk.com/Article/details/guxbruqwo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.yfazqb.com/Article/details/ggrzjpmxd.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/ggkhqbzkw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.sjlbkw.cn/Article/details/gjpwtsdda.sHtML

[S03] C：读入整数
来源：http://mobile.tarul.cn/Article/details/gukyfczjr.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/gpbgwnwvy.sHtML

[S04] C：字符串复制
来源：http://baike.sjlbkw.cn/Article/details/ggtbdvsvo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.sjlbkw.cn/Article/details/glcfifghm.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gcmghgzwf.sHtML

strlen(s)
来源：http://3g.bbcook.cn/Article/details/gcwbmgecs.sHtML

[S06] C：字符串比较
来源：http://baike.yfazqb.com/Article/details/gfktqbrcc.sHtML

strcmp(a, b) == 0
来源：http://mobile.epnwcf.com/Article/details/gzomaekyr.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fktsv.cn/Article/details/gjdbncwnh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.epnwcf.com/Article/details/gxaqprmwj.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.yfazqb.com/Article/details/gowuojmmh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.yfazqb.com/Article/details/gnrpfcjdh.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.tarul.cn/Article/details/gfgyimrxd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.vehdjk.com/Article/details/gkpqubhqz.sHtML

[S10] C：指针与解引用
来源：http://read.share.yfazqb.com/Article/details/gxucrwjni.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.bbcook.cn/Article/details/giuqiqvjp.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gneioiobj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.bbcook.cn/Article/details/gpaqxcxuj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/gtiwxeoih.sHtML

fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/glwdjqhed.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/gfagaqtnu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gmsiqanwm.sHtML

[S13] C：宏定义
来源：http://wap.epnwcf.com/Article/details/gzribwxci.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fktsv.cn/Article/details/gqkigmnyr.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/ggsacgznb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fktsv.cn/Article/details/gkmdtujvj.sHtML

[S15] C：类型转换
来源：http://baike.yfazqb.com/Article/details/gajwdqkxm.sHtML

(double) a / b
来源：http://3g.tarul.cn/Article/details/gzwgigtqh.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/ghwluwlxx.sHtML

x |= (1 << 3);
来源：http://read.share.sjlbkw.cn/Article/details/ggluxgsos.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.vehdjk.com/Article/details/galhlbswh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.tarul.cn/Article/details/gahrpwzvj.sHtML

[S18] C：命令行参数
来源：http://read.share.tarul.cn/Article/details/gopfkxfty.sHtML

int main(int argc, char **argv)
来源：http://www.share.sjlbkw.cn/Article/details/gbbnmdlkb.sHtML

[S19] C：快速排序
来源：http://mobile.yfazqb.com/Article/details/gcrvjozvg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/ghuignsfm.sHtML

[S20] C：二分查找
来源：http://www.share.fktsv.cn/Article/details/glwfdvzmb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/geiryyqod.sHtML

[S21] C：字符类别判断
来源：http://m.share.yfazqb.com/Article/details/gdeghsfpa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.sjlbkw.cn/Article/details/guchaggbe.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/ghlfmxjig.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fktsv.cn/Article/details/gwkxvmkaq.sHtML

[S23] C：随机数
来源：http://www.m.share.fktsv.cn/Article/details/gcnxzvblz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/gvoyxxfqo.sHtML

[S24] C：获取本地时间
来源：http://mobile.sjlbkw.cn/Article/details/gixskgokf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.yfazqb.com/Article/details/grexhvfpx.sHtML

[S25] C：内存拷贝
来源：http://3g.yfazqb.com/Article/details/gqenbzydp.sHtML

memcpy(dst, src, n);
来源：http://blog.fktsv.cn/Article/details/gvujkjqwn.sHtML

[S26] C：内存清零
来源：http://blog.epnwcf.com/Article/details/gnhvorjgg.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gtjxsftut.sHtML

[S27] C：定义常量
来源：http://www.blog.sjlbkw.cn/Article/details/gmainpbav.sHtML

const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gfjmyigln.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/gcivcqkkl.sHtML

static int counter = 0;
来源：http://read.share.sjlbkw.cn/Article/details/gihgiduik.sHtML

[S29] C：变参函数
来源：http://mobile.tarul.cn/Article/details/gjsnhpyco.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/ghfplrdgw.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/gdncdycoj.sHtML

#ifndef X_H
来源：http://www.share.vehdjk.com/Article/details/gonkxgkda.sHtML

#define X_H
来源：http://www.share.sjlbkw.cn/Article/details/gywexqguw.sHtML

#endif
来源：http://m.share.fktsv.cn/Article/details/gfoaqaeaq.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/gnmuzuzdb.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gzrwhphjn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/gagefjgdh.sHtML

[S32] C++：字符串
来源：http://read.share.bbcook.cn/Article/details/gjjrsnijo.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fktsv.cn/Article/details/gkaaifmaa.sHtML

[S33] C++：vector 增删
来源：http://baike.fktsv.cn/Article/details/gyavdaqco.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.vehdjk.com/Article/details/gujffechj.sHtML

[S34] C++：遍历 vector
来源：http://3g.bbcook.cn/Article/details/ghgjugfze.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.epnwcf.com/Article/details/gsgfbpeyu.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/gxwqmsucp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gonjgyudm.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/gnjqmfkfn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gtfestlrn.sHtML

[S37] C++：set
来源：http://mobile.tarul.cn/Article/details/gxweskvht.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gyjczkkij.sHtML

[S38] C++：排序
来源：http://mobile.sjlbkw.cn/Article/details/gihagpvnw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gzqhuygvn.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fktsv.cn/Article/details/gkmwgzcyz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/gmdvndgop.sHtML

[S40] C++：查找元素
来源：http://3g.epnwcf.com/Article/details/ggghzbigw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.vehdjk.com/Article/details/gscmqevaz.sHtML

[S41] C++：类与构造函数
来源：http://m.share.vehdjk.com/Article/details/ggwdujoah.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.bbcook.cn/Article/details/ggsrtpkzz.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gpxaqqhyp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/gvotzvmer.sHtML

[S43] C++：智能指针
来源：http://3g.vehdjk.com/Article/details/gzwgniyyn.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.vehdjk.com/Article/details/gclmbhdho.sHtML

[S44] C++：引用传参
来源：http://wap.fktsv.cn/Article/details/gkubbmpda.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.sjlbkw.cn/Article/details/gcqlzjgun.sHtML

[S45] C++：lambda
来源：http://baike.fktsv.cn/Article/details/ghnonkepm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.tarul.cn/Article/details/gdpidqczi.sHtML

[S46] C++：函数模板
来源：http://www.blog.vehdjk.com/Article/details/gsfcuyogq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fktsv.cn/Article/details/gundoybbg.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.tarul.cn/Article/details/guhrakrsx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.vehdjk.com/Article/details/gttrvbgfb.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gewliuujw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.yfazqb.com/Article/details/ggnlwtkxn.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gtegswowc.sHtML

[S49] C++：写文件
来源：http://3g.sjlbkw.cn/Article/details/gkmlxqxzz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.epnwcf.com/Article/details/gelpkphlg.sHtML

[S50] C++：格式化数字
来源：http://m.share.vehdjk.com/Article/details/glubemiwi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.yfazqb.com/Article/details/ggwwxuimx.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gucneqcrc.sHtML

static_cast<double>(a) / b
来源：http://www.blog.tarul.cn/Article/details/glubkfduo.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.tarul.cn/Article/details/gncezorxl.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.sjlbkw.cn/Article/details/gaqwkzxib.sHtML

[S53] C++：移动语义
来源：http://baike.epnwcf.com/Article/details/gsporlhag.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gitqlnwsm.sHtML

[S54] C++：异常处理
来源：http://blog.sjlbkw.cn/Article/details/gqmleuuun.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.bbcook.cn/Article/details/gfypxnriw.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fktsv.cn/Article/details/gwtygiybi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gsmzbkkly.sHtML

[S56] C++：optional
来源：http://www.m.share.sjlbkw.cn/Article/details/guqxjalfw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.sjlbkw.cn/Article/details/gxfvcfyiq.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gncmnnbkq.sHtML

constexpr int N = 10;
来源：http://www.blog.epnwcf.com/Article/details/gcfubuzqf.sHtML

[S58] C++：命名空间
来源：http://read.share.fktsv.cn/Article/details/gygggsicb.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fktsv.cn/Article/details/gntpwkjwd.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/grrnihzoo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.bbcook.cn/Article/details/gcyhczxht.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gsbctlyqd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.yfazqb.com/Article/details/gacmdgppw.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwpzjaebb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/gdsaahhnu.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gijbbonrv.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fktsv.cn/Article/details/ghabxurye.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/goydddhcz.sHtML

[T02] Kotlin：变量
来源：http://mobile.yfazqb.com/Article/details/gekzavkhp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.tarul.cn/Article/details/gdlgwtkdq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.yfazqb.com/Article/details/gbkpnkskw.sHtML

"值: $b"
来源：http://www.share.epnwcf.com/Article/details/ggepgoprp.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/gwbeaosee.sHtML

val n: String? = null;  n?.length
来源：http://blog.vehdjk.com/Article/details/gffbnmlyf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.epnwcf.com/Article/details/gxujrazhb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.sjlbkw.cn/Article/details/girfwlytw.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/gxwkudnlm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fktsv.cn/Article/details/gyslknfzk.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.bbcook.cn/Article/details/gmziqyvgg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.bbcook.cn/Article/details/ggqwwifba.sHtML

[T08] Kotlin：数据类
来源：http://wap.sjlbkw.cn/Article/details/gmaqlmxdx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/ginziowuw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.epnwcf.com/Article/details/giozzpyfc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.sjlbkw.cn/Article/details/gmsoyhavc.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.yfazqb.com/Article/details/gxsdsqxjl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gkrdyqgqm.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.yfazqb.com/Article/details/ghogjvgwz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.sjlbkw.cn/Article/details/gdvxkkbpo.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/gbonxvdba.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.yfazqb.com/Article/details/gadtvxjho.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.yfazqb.com/Article/details/gxhupatlp.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.tarul.cn/Article/details/gjyeirtzk.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gudtgmqna.sHtML

for (i in 1..10) println(i)
来源：http://3g.yfazqb.com/Article/details/gxyuqiwtp.sHtML

[T15] Kotlin：接口
来源：http://baike.vehdjk.com/Article/details/gdtubenxl.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.epnwcf.com/Article/details/gstaxncng.sHtML

[T16] Swift：Hello World
来源：http://www.share.bbcook.cn/Article/details/gfesyxaba.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gwsrguigy.sHtML

[T17] Swift：变量与常量
来源：http://mobile.vehdjk.com/Article/details/gexzrolnt.sHtML

var a = 1;  let b = 2
来源：http://mobile.bbcook.cn/Article/details/glxlflhlp.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.tarul.cn/Article/details/ggexhfbhy.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gaafiphva.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.yfazqb.com/Article/details/gcblnjwxt.sHtML

if let n = opt { print(n) }
来源：http://wap.tarul.cn/Article/details/gqijkzyiw.sHtML

[T20] Swift：数组操作
来源：http://wap.tarul.cn/Article/details/gxqqqhobj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.yfazqb.com/Article/details/gudxobmas.sHtML

[T21] Swift：遍历
来源：http://www.share.tarul.cn/Article/details/gecswuguo.sHtML

for x in a { print(x) }
来源：http://blog.vehdjk.com/Article/details/gbwkhcfbo.sHtML

[T22] Swift：字典
来源：http://www.blog.tarul.cn/Article/details/gqhujxuna.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.yfazqb.com/Article/details/guefzycge.sHtML

[T23] Swift：函数
来源：http://m.share.bbcook.cn/Article/details/gpjqjzpqc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.tarul.cn/Article/details/gevvjvyzx.sHtML

[T24] Swift：闭包
来源：http://www.m.share.bbcook.cn/Article/details/gifdikvzy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.yfazqb.com/Article/details/gbllsaudk.sHtML

[T25] Swift：结构体
来源：http://www.m.share.epnwcf.com/Article/details/gpexmvsjc.sHtML

struct P { var x: Int }
来源：http://read.share.fktsv.cn/Article/details/gourvdmps.sHtML

[T26] Swift：类与重写
来源：http://blog.sjlbkw.cn/Article/details/gasqywipk.sHtML

class A: Base { override func f() {} }
来源：http://read.share.bbcook.cn/Article/details/gdfmxrvfd.sHtML

[T27] Swift：错误处理
来源：http://wap.sjlbkw.cn/Article/details/gadbcoioj.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsqahgps.sHtML

[T28] Swift：枚举
来源：http://blog.tarul.cn/Article/details/gbruaoknx.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/gvqbbzuwy.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.tarul.cn/Article/details/gpejvxodu.sHtML

guard let x = opt else { return }
来源：http://www.share.tarul.cn/Article/details/gsxtppded.sHtML

[T30] Swift：协议
来源：http://www.m.share.vehdjk.com/Article/details/gshevoqiy.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.sjlbkw.cn/Article/details/grwrltwcl.sHtML

[T31] Lua：Hello World
来源：http://m.share.epnwcf.com/Article/details/gvpwqooix.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gkyssfvlf.sHtML

[T32] Lua：局部变量
来源：http://wap.epnwcf.com/Article/details/gagzupkjs.sHtML

local a = 1
来源：http://www.share.vehdjk.com/Article/details/gyxbepdcg.sHtML

[T33] Lua：表（数组）
来源：http://m.share.vehdjk.com/Article/details/ggxshdbwg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.vehdjk.com/Article/details/gcfwabkdd.sHtML

[T34] Lua：遍历表
来源：http://read.share.tarul.cn/Article/details/gtogpldfe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/gcnflywtd.sHtML

[T35] Lua：字典表
来源：http://3g.bbcook.cn/Article/details/gnsdkspzj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.sjlbkw.cn/Article/details/girdhyakx.sHtML

[T36] Lua：函数
来源：http://blog.tarul.cn/Article/details/gukmkmlym.sHtML

function add(a, b) return a + b end
来源：http://3g.tarul.cn/Article/details/gwqiquttk.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.bbcook.cn/Article/details/gpcsnnfkn.sHtML

"a" .. "b"
来源：http://m.share.fktsv.cn/Article/details/gscnktqpx.sHtML

[T38] Lua：条件
来源：http://m.share.yfazqb.com/Article/details/gonwhlgjz.sHtML

if x > 0 then print("正") end
来源：http://wap.yfazqb.com/Article/details/ghtiezlhd.sHtML

[T39] Lua：模式匹配
来源：http://baike.vehdjk.com/Article/details/goyleburs.sHtML

string.find(s, "%d+")
来源：http://3g.epnwcf.com/Article/details/grzdvgxrh.sHtML

[T40] Lua：元表
来源：http://www.m.share.tarul.cn/Article/details/gttceriin.sHtML

setmetatable({}, { __index = base })
来源：http://blog.vehdjk.com/Article/details/gablxkuax.sHtML

[T41] Perl：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gqdybenhb.sHtML

print "Hello\n";
来源：http://blog.fktsv.cn/Article/details/gxcllkrwn.sHtML

[T42] Perl：变量类型
来源：http://3g.tarul.cn/Article/details/gyttjqtcc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.sjlbkw.cn/Article/details/gwrwhbtut.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gwskhjcdr.sHtML

"值: $a"
来源：http://baike.bbcook.cn/Article/details/gwjdjxjjn.sHtML

[T44] Perl：条件
来源：http://m.share.vehdjk.com/Article/details/gayfnyogp.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.sjlbkw.cn/Article/details/glkbtmhqo.sHtML

[T45] Perl：数组遍历
来源：http://baike.yfazqb.com/Article/details/gqjldmvys.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.epnwcf.com/Article/details/gfovixbxy.sHtML

[T46] Perl：哈希操作
来源：http://mobile.sjlbkw.cn/Article/details/glirzbxqh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fktsv.cn/Article/details/gbosarpah.sHtML

[T47] Perl：正则捕获
来源：http://read.share.vehdjk.com/Article/details/gofndjtwo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.bbcook.cn/Article/details/gvdpcmqby.sHtML

[T48] Perl：正则替换
来源：http://wap.fktsv.cn/Article/details/gbiffnzoj.sHtML

$s =~ s/old/new/g;
来源：http://www.share.vehdjk.com/Article/details/gxlihwdyb.sHtML

[T49] Perl：函数
来源：http://baike.epnwcf.com/Article/details/glyyqldst.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/geqfswhlm.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gljnzzlov.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.bbcook.cn/Article/details/gitayxjgh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.tarul.cn/Article/details/gzspqrfpu.sHtML

[T51] Scala：Hello World
来源：http://www.share.tarul.cn/Article/details/gfhtmkyax.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/gmxstnhdp.sHtML

[T52] Scala：变量
来源：http://www.share.vehdjk.com/Article/details/gxgdkclin.sHtML

val a = 1;  var b = 2
来源：http://wap.yfazqb.com/Article/details/grxvqzwpb.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gbwohnjlc.sHtML

s"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gdjjhjksi.sHtML

[T54] Scala：集合映射
来源：http://mobile.tarul.cn/Article/details/ggbkxckng.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gefuplpjy.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gfczcyyfw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.yfazqb.com/Article/details/gcrohtuhw.sHtML

[T56] Scala：样例类
来源：http://www.m.share.vehdjk.com/Article/details/gjwblwrkt.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/gcwhrljmv.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkylajdu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.yfazqb.com/Article/details/gfoiecwbn.sHtML

[T58] Scala：函数定义
来源：http://mobile.yfazqb.com/Article/details/gxwpqsdwx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.epnwcf.com/Article/details/gjggctvto.sHtML

[T59] Scala：循环
来源：http://wap.yfazqb.com/Article/details/ggkskmeyv.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gulnfgftq.sHtML

[T60] Scala：折叠
来源：http://baike.bbcook.cn/Article/details/gttayhiik.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.yfazqb.com/Article/details/gelkwjgwf.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gverbvhjy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.tarul.cn/Article/details/gfoescnmh.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/grpzerlow.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.tarul.cn/Article/details/ggnonxgjf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fktsv.cn/Article/details/gxfdacqcx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.bbcook.cn/Article/details/gonjznqpf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fktsv.cn/Article/details/gemhzzivz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fktsv.cn/Article/details/gbmxpcjmg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.epnwcf.com/Article/details/gqbhvnbad.sHtML

[U04] Py：变量调试打印
来源：http://wap.fktsv.cn/Article/details/ghwyjuhrj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.sjlbkw.cn/Article/details/gkogdtwaq.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.yfazqb.com/Article/details/grzadvsih.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/grmonzgfx.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.bbcook.cn/Article/details/gaztdmuil.sHtML

{**a, **b}
来源：http://www.m.share.tarul.cn/Article/details/gxtkxypni.sHtML

[U07] Py：反转字典键值
来源：http://read.share.yfazqb.com/Article/details/gldjkxnsk.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fktsv.cn/Article/details/gorivpfer.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fktsv.cn/Article/details/ghvcncxbr.sHtML

[y for x in nested for y in x]
来源：http://mobile.sjlbkw.cn/Article/details/gdwayhzpp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fktsv.cn/Article/details/gvciimviw.sHtML

max(d, key=d.get)
来源：http://wap.vehdjk.com/Article/details/gwpjthfhj.sHtML

[U10] Py：按值排序字典
来源：http://wap.tarul.cn/Article/details/gvfskpjjk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.epnwcf.com/Article/details/gkjkvkckr.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhsfbhjd.sHtML

(x * 2 for x in arr)
来源：http://wap.tarul.cn/Article/details/gkwayrgnn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.vehdjk.com/Article/details/grgfemzff.sHtML

Counter(arr).most_common(3)
来源：http://blog.vehdjk.com/Article/details/ganccssec.sHtML

[U13] Py：固定长度队列
来源：http://mobile.bbcook.cn/Article/details/grbfbyabk.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/gzufqvpny.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.epnwcf.com/Article/details/gucjhqrtb.sHtML

defaultdict(list)
来源：http://www.blog.tarul.cn/Article/details/giiiyhblk.sHtML


<!-- 参考信息 -->