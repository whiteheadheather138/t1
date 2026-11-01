代发 wailian999

read -rp "请输入: " ans
来源：http://mobile.tarul.cn/Article/details/grpljvwjp.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/grpxukigc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/gyjockebu.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/gmfeuxbzr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.yfazqb.com/Article/details/gdblpcfzq.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.yfazqb.com/Article/details/glirbzmzz.sHtML

time ./run.sh
来源：http://wap.fktsv.cn/Article/details/gfhbmkedn.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/geecwlhmc.sHtML

S. C / C++ 专题
来源：http://m.share.vehdjk.com/Article/details/gkcjfhokl.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbuyhayqf.sHtML

[S01] C：Hello World
来源：http://www.share.yfazqb.com/Article/details/gfxqbaqwi.sHtML

#include <stdio.h>
来源：http://m.share.tarul.cn/Article/details/ghgurhfwp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.epnwcf.com/Article/details/gdrhljhcu.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.epnwcf.com/Article/details/glawjcrts.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.tarul.cn/Article/details/grmhtiftp.sHtML

[S03] C：读入整数
来源：http://www.share.epnwcf.com/Article/details/gqakiykjd.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/gglvntivy.sHtML

[S04] C：字符串复制
来源：http://www.share.yfazqb.com/Article/details/gvxggkjub.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fktsv.cn/Article/details/grcjyjlkn.sHtML

[S05] C：字符串长度
来源：http://read.share.vehdjk.com/Article/details/gojnprhzc.sHtML

strlen(s)
来源：http://www.share.tarul.cn/Article/details/gvcjyawsh.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/givxnlhjt.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/grpepmfyr.sHtML

[S07] C：数组遍历求和
来源：http://read.share.vehdjk.com/Article/details/gfhbfdmtd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.bbcook.cn/Article/details/gfbqhgxig.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gbclrwkog.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.yfazqb.com/Article/details/gmcodaokm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.tarul.cn/Article/details/gtkfzwcre.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.tarul.cn/Article/details/geiuekxaf.sHtML

[S10] C：指针与解引用
来源：http://blog.yfazqb.com/Article/details/gdmuqkmdf.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.bbcook.cn/Article/details/gfiidbsnm.sHtML

[S11] C：逐行读文件
来源：http://3g.yfazqb.com/Article/details/geaynjmry.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.bbcook.cn/Article/details/gsfvystun.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.bbcook.cn/Article/details/gmzqrzljw.sHtML

fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/gaxwvvafb.sHtML

[S12] C：写文件
来源：http://wap.sjlbkw.cn/Article/details/gjvolsrvw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnigoqnat.sHtML

[S13] C：宏定义
来源：http://3g.sjlbkw.cn/Article/details/gwxhoxdta.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.yfazqb.com/Article/details/gafrsetjy.sHtML

[S14] C：枚举
来源：http://baike.epnwcf.com/Article/details/gndsvopwi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.bbcook.cn/Article/details/gireulytu.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/gyimrmtxq.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/ghlhxoxmi.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/gybmyhipp.sHtML

x |= (1 << 3);
来源：http://www.share.sjlbkw.cn/Article/details/gpnvyvnmv.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/ggsbftdzz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.sjlbkw.cn/Article/details/gnnannlcd.sHtML

[S18] C：命令行参数
来源：http://m.share.epnwcf.com/Article/details/gcudherit.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/gysvkxdec.sHtML

[S19] C：快速排序
来源：http://wap.sjlbkw.cn/Article/details/ghbeocpog.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/gixbwpeoy.sHtML

[S20] C：二分查找
来源：http://blog.sjlbkw.cn/Article/details/gykdhapln.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/guxfdcmvq.sHtML

[S21] C：字符类别判断
来源：http://blog.yfazqb.com/Article/details/gkgjxpzbz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.tarul.cn/Article/details/geaemzggd.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/glwkirhax.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.vehdjk.com/Article/details/guixyqwzt.sHtML

[S23] C：随机数
来源：http://m.share.bbcook.cn/Article/details/gumtfeyyn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/ghgtdohfv.sHtML

[S24] C：获取本地时间
来源：http://3g.fktsv.cn/Article/details/gfgokpirt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.bbcook.cn/Article/details/ghqonasle.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/ghnnzlsia.sHtML

memcpy(dst, src, n);
来源：http://blog.bbcook.cn/Article/details/goygmfdhm.sHtML

[S26] C：内存清零
来源：http://www.m.share.tarul.cn/Article/details/geelcract.sHtML

memset(a, 0, sizeof a);
来源：http://blog.bbcook.cn/Article/details/glhacbuzq.sHtML

[S27] C：定义常量
来源：http://read.share.sjlbkw.cn/Article/details/gcasdrlde.sHtML

const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gegoetmfm.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/gquufofoe.sHtML

static int counter = 0;
来源：http://wap.yfazqb.com/Article/details/gjzjqfrsb.sHtML

[S29] C：变参函数
来源：http://blog.sjlbkw.cn/Article/details/gucbjbjnv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.yfazqb.com/Article/details/gktbbwvto.sHtML

[S30] C：头文件保护
来源：http://mobile.tarul.cn/Article/details/gtmdzxvhf.sHtML

#ifndef X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoaowdtm.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gedcddraq.sHtML

#endif
来源：http://www.blog.tarul.cn/Article/details/gqvpmqqql.sHtML

[S31] C++：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gyqghuuog.sHtML

#include <iostream>
来源：http://m.share.yfazqb.com/Article/details/grvzqzbuo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fktsv.cn/Article/details/gyintmvrp.sHtML

[S32] C++：字符串
来源：http://3g.vehdjk.com/Article/details/gjjntpqco.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.sjlbkw.cn/Article/details/ghfjratjw.sHtML

[S33] C++：vector 增删
来源：http://m.share.vehdjk.com/Article/details/gopfecuph.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.sjlbkw.cn/Article/details/gshqribza.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/ghxpfxouu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.epnwcf.com/Article/details/gxkgxumed.sHtML

[S35] C++：map
来源：http://mobile.fktsv.cn/Article/details/gogdcliik.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gurmhuwyl.sHtML

[S36] C++：unordered_map
来源：http://www.blog.tarul.cn/Article/details/gndulnwlb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/gifcgfufv.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/gtzboyoaa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.vehdjk.com/Article/details/gqoopctgr.sHtML

[S38] C++：排序
来源：http://mobile.tarul.cn/Article/details/gulqlphxl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gutzlogbj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.yfazqb.com/Article/details/gofsyunxg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.sjlbkw.cn/Article/details/gxjgofiya.sHtML

[S40] C++：查找元素
来源：http://3g.yfazqb.com/Article/details/galtmfjrk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.vehdjk.com/Article/details/geuvvithl.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/gkgboassj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/gnhelhplg.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/ghvgodqtx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.sjlbkw.cn/Article/details/gqmocqwbb.sHtML

[S43] C++：智能指针
来源：http://3g.vehdjk.com/Article/details/gondnrwzm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.bbcook.cn/Article/details/gisjehqwv.sHtML

[S44] C++：引用传参
来源：http://www.share.epnwcf.com/Article/details/grvfbvpdh.sHtML

void inc(int &x) { ++x; }
来源：http://3g.bbcook.cn/Article/details/gsugoyero.sHtML

[S45] C++：lambda
来源：http://m.share.bbcook.cn/Article/details/gjmvhhpyb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gbphiuwlb.sHtML

[S46] C++：函数模板
来源：http://www.m.share.tarul.cn/Article/details/gtssjjcct.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.vehdjk.com/Article/details/geigtrjkv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.bbcook.cn/Article/details/gmwbcowzd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.vehdjk.com/Article/details/gpwdlvcyu.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gimfvesgq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.tarul.cn/Article/details/gyqitzrna.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/giqoukxtf.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/ggdfjmnzd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.vehdjk.com/Article/details/gueynoeln.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/gdixegdro.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gdwttekra.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/gcqinzbxu.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/gxmpyogzf.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.tarul.cn/Article/details/gnjxbnawd.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/gadnhiaxm.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/gyshlmjhp.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gejtdrcpw.sHtML

[S54] C++：异常处理
来源：http://3g.sjlbkw.cn/Article/details/gjjswlknj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.yfazqb.com/Article/details/gzkcqjeuu.sHtML

[S55] C++：结构化绑定
来源：http://baike.bbcook.cn/Article/details/gurdqsiaj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.bbcook.cn/Article/details/gusgsvtpb.sHtML

[S56] C++：optional
来源：http://www.share.sjlbkw.cn/Article/details/ggvuzrmwv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.yfazqb.com/Article/details/gnaneqfcw.sHtML

[S57] C++：编译期常量
来源：http://blog.yfazqb.com/Article/details/gnjtlgfjb.sHtML

constexpr int N = 10;
来源：http://wap.bbcook.cn/Article/details/gejhemzlv.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gxuhbyslr.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/gtlhyjkdy.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/grheshkpd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/gcpujlmzw.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.vehdjk.com/Article/details/gipvzjbba.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.yfazqb.com/Article/details/gngyaunnk.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gfzmggkcr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/gugpuidij.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gzhnrydmp.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gcvploxwp.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gqzqljxlr.sHtML

[T02] Kotlin：变量
来源：http://blog.vehdjk.com/Article/details/gilmieqvf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.yfazqb.com/Article/details/gbgeqvkzx.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.tarul.cn/Article/details/gjgzembbe.sHtML

"值: $b"
来源：http://m.share.tarul.cn/Article/details/gaypioeeq.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/gyvskkhti.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.vehdjk.com/Article/details/glmqringf.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.yfazqb.com/Article/details/gmrqqnwzv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.yfazqb.com/Article/details/gbhumovvp.sHtML

[T06] Kotlin：集合映射
来源：http://baike.bbcook.cn/Article/details/gwfiumyqb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.bbcook.cn/Article/details/glehqistd.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.vehdjk.com/Article/details/gbqzdbtnu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.bbcook.cn/Article/details/gdrzcwrrk.sHtML

[T08] Kotlin：数据类
来源：http://baike.sjlbkw.cn/Article/details/gvqwszgjh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/guhuieacx.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.sjlbkw.cn/Article/details/guyefjqep.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.bbcook.cn/Article/details/givgmpbli.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.bbcook.cn/Article/details/goslxuqsr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fktsv.cn/Article/details/gcsmkwfvp.sHtML

[T11] Kotlin：协程
来源：http://www.share.tarul.cn/Article/details/gnucupztr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fktsv.cn/Article/details/gbvimqlyh.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fktsv.cn/Article/details/gdqtlromn.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gjoohkvja.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.yfazqb.com/Article/details/gaswxpbmw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.yfazqb.com/Article/details/gifgyljxv.sHtML

[T14] Kotlin：循环
来源：http://blog.sjlbkw.cn/Article/details/gpkxzpiib.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fktsv.cn/Article/details/grhluqgcu.sHtML

[T15] Kotlin：接口
来源：http://3g.epnwcf.com/Article/details/gmysmmmen.sHtML

interface Shape { fun area(): Double }
来源：http://3g.bbcook.cn/Article/details/gglnznuml.sHtML

[T16] Swift：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gnzbohxxp.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/gohzugagq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fktsv.cn/Article/details/gnqgzwqao.sHtML

var a = 1;  let b = 2
来源：http://3g.yfazqb.com/Article/details/grommqgex.sHtML

[T18] Swift：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gvpgvkxtw.sHtML

"值: \(b)"
来源：http://www.share.bbcook.cn/Article/details/ggrifqdxr.sHtML

[T19] Swift：可选绑定
来源：http://blog.tarul.cn/Article/details/gyemsostm.sHtML

if let n = opt { print(n) }
来源：http://read.share.tarul.cn/Article/details/glzmbynfp.sHtML

[T20] Swift：数组操作
来源：http://mobile.tarul.cn/Article/details/gwyfwnxra.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.tarul.cn/Article/details/gfqvdxrym.sHtML

[T21] Swift：遍历
来源：http://www.share.yfazqb.com/Article/details/gnxmvdylk.sHtML

for x in a { print(x) }
来源：http://3g.vehdjk.com/Article/details/gxwzuairm.sHtML

[T22] Swift：字典
来源：http://www.share.vehdjk.com/Article/details/gykywtfar.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.bbcook.cn/Article/details/gnytuqcyq.sHtML

[T23] Swift：函数
来源：http://3g.yfazqb.com/Article/details/gjewftlev.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.epnwcf.com/Article/details/gcfszgywy.sHtML

[T24] Swift：闭包
来源：http://3g.sjlbkw.cn/Article/details/gldhqxsud.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.bbcook.cn/Article/details/gatipcqhr.sHtML

[T25] Swift：结构体
来源：http://www.blog.epnwcf.com/Article/details/gilqrslzo.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/gdxcyrsag.sHtML

[T26] Swift：类与重写
来源：http://read.share.sjlbkw.cn/Article/details/gloobuyjt.sHtML

class A: Base { override func f() {} }
来源：http://blog.fktsv.cn/Article/details/gfjsflrfc.sHtML

[T27] Swift：错误处理
来源：http://wap.tarul.cn/Article/details/gjmqtcjpm.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.vehdjk.com/Article/details/glgtdvmkp.sHtML

[T28] Swift：枚举
来源：http://baike.sjlbkw.cn/Article/details/gprmsrqjr.sHtML

enum Color { case red, green }
来源：http://m.share.fktsv.cn/Article/details/grbkazhvi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fktsv.cn/Article/details/gxcnrnbal.sHtML

guard let x = opt else { return }
来源：http://baike.sjlbkw.cn/Article/details/guuncqblr.sHtML

[T30] Swift：协议
来源：http://baike.epnwcf.com/Article/details/gdjihpcce.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fktsv.cn/Article/details/gpcjqqkxf.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gfgalftox.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gzzwxtpbi.sHtML

[T32] Lua：局部变量
来源：http://mobile.bbcook.cn/Article/details/gncgdutce.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/gvsexcmoi.sHtML

[T33] Lua：表（数组）
来源：http://baike.bbcook.cn/Article/details/ghtpbyaaz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.vehdjk.com/Article/details/goegvclil.sHtML

[T34] Lua：遍历表
来源：http://baike.sjlbkw.cn/Article/details/gtyaklobd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/ghfwilsql.sHtML

[T35] Lua：字典表
来源：http://baike.sjlbkw.cn/Article/details/gzvcrvbrr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.sjlbkw.cn/Article/details/gysxqrjxy.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/gxihjmgvn.sHtML

function add(a, b) return a + b end
来源：http://www.share.vehdjk.com/Article/details/gvjrwtcxa.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/gyvwbhwuv.sHtML

"a" .. "b"
来源：http://m.share.tarul.cn/Article/details/gwdcotlqs.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/gcyxsgrzd.sHtML

if x > 0 then print("正") end
来源：http://baike.sjlbkw.cn/Article/details/gbxhglglh.sHtML

[T39] Lua：模式匹配
来源：http://read.share.vehdjk.com/Article/details/gujzyxyzm.sHtML

string.find(s, "%d+")
来源：http://read.share.fktsv.cn/Article/details/gsivsrxvw.sHtML

[T40] Lua：元表
来源：http://baike.yfazqb.com/Article/details/gxuclutqy.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fktsv.cn/Article/details/gezdzrwyg.sHtML

[T41] Perl：Hello World
来源：http://baike.bbcook.cn/Article/details/gcsbjhbhf.sHtML

print "Hello\n";
来源：http://www.blog.epnwcf.com/Article/details/gxvfpaujg.sHtML

[T42] Perl：变量类型
来源：http://blog.epnwcf.com/Article/details/gsmsvtdkt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fktsv.cn/Article/details/gljvlfapp.sHtML

[T43] Perl：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gzqlcevrn.sHtML

"值: $a"
来源：http://www.blog.tarul.cn/Article/details/gfsqhlpdz.sHtML

[T44] Perl：条件
来源：http://baike.bbcook.cn/Article/details/gzrjssvth.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.yfazqb.com/Article/details/gcdujovje.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.bbcook.cn/Article/details/gajwzvjdv.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.sjlbkw.cn/Article/details/gxcercqdd.sHtML

[T46] Perl：哈希操作
来源：http://read.share.epnwcf.com/Article/details/gsqcpvnjp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.vehdjk.com/Article/details/gcwlhyfrx.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.sjlbkw.cn/Article/details/gwogvcuhu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.tarul.cn/Article/details/gzibimndt.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/gthipwanh.sHtML

$s =~ s/old/new/g;
来源：http://mobile.vehdjk.com/Article/details/ghgmlkttc.sHtML

[T49] Perl：函数
来源：http://www.share.tarul.cn/Article/details/gfobhizdw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gzehpyshe.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gsodjmqwl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.yfazqb.com/Article/details/giicenbnz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.yfazqb.com/Article/details/gyhkgvjit.sHtML

[T51] Scala：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gmjcqphtx.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gahhvahra.sHtML

[T52] Scala：变量
来源：http://www.blog.epnwcf.com/Article/details/gslhzywbm.sHtML

val a = 1;  var b = 2
来源：http://read.share.epnwcf.com/Article/details/goswnxtqz.sHtML

[T53] Scala：字符串插值
来源：http://baike.tarul.cn/Article/details/gmyrbzcku.sHtML

s"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gwgiaysed.sHtML

[T54] Scala：集合映射
来源：http://3g.epnwcf.com/Article/details/gfdcnycyk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.bbcook.cn/Article/details/gxrjehfdj.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyvdguxt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.sjlbkw.cn/Article/details/gebxlvyml.sHtML

[T56] Scala：样例类
来源：http://blog.bbcook.cn/Article/details/gojhgqnqh.sHtML

case class User(name: String, age: Int)
来源：http://mobile.bbcook.cn/Article/details/gtesodyej.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/geawuftlo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.sjlbkw.cn/Article/details/goaayxahb.sHtML

[T58] Scala：函数定义
来源：http://read.share.epnwcf.com/Article/details/gobvzueuk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.vehdjk.com/Article/details/grpjmwkcj.sHtML

[T59] Scala：循环
来源：http://3g.bbcook.cn/Article/details/gtwnaxxjb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/glfanjrgo.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fktsv.cn/Article/details/gaxvembsf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.sjlbkw.cn/Article/details/grmfvnfhy.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjatzdusg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/gcyxfticu.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gczhvkkbg.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.yfazqb.com/Article/details/gxadakiec.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.tarul.cn/Article/details/gomvpgdnp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.bbcook.cn/Article/details/gxjymfrpr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.bbcook.cn/Article/details/givqtcrtb.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/gqpwngejt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.yfazqb.com/Article/details/gqyodvxrr.sHtML

[U04] Py：变量调试打印
来源：http://www.share.epnwcf.com/Article/details/gundcdkfw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.tarul.cn/Article/details/ghrzguzqx.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.tarul.cn/Article/details/goffqckew.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gfqsygbzf.sHtML

[U06] Py：合并两个字典
来源：http://www.share.epnwcf.com/Article/details/gejsxncho.sHtML

{**a, **b}
来源：http://read.share.vehdjk.com/Article/details/gapgasekn.sHtML

[U07] Py：反转字典键值
来源：http://baike.tarul.cn/Article/details/gijhxbnka.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fktsv.cn/Article/details/gojjjeqou.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.tarul.cn/Article/details/gbiibtidb.sHtML

[y for x in nested for y in x]
来源：http://mobile.sjlbkw.cn/Article/details/gxfsqwrvr.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.epnwcf.com/Article/details/gxrcjlbvx.sHtML

max(d, key=d.get)
来源：http://m.share.yfazqb.com/Article/details/gfmhptjyx.sHtML

[U10] Py：按值排序字典
来源：http://3g.fktsv.cn/Article/details/gbrwdypqq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.yfazqb.com/Article/details/gvgcdilrx.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gplaneues.sHtML

(x * 2 for x in arr)
来源：http://read.share.bbcook.cn/Article/details/gfwwxtkrr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.yfazqb.com/Article/details/glmfrvlmd.sHtML

Counter(arr).most_common(3)
来源：http://blog.fktsv.cn/Article/details/geaokaivm.sHtML

[U13] Py：固定长度队列
来源：http://www.share.sjlbkw.cn/Article/details/gnaphtfew.sHtML

deque(maxlen=10)
来源：http://m.share.sjlbkw.cn/Article/details/gqvitsohm.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.sjlbkw.cn/Article/details/grluozqgg.sHtML

defaultdict(list)
来源：http://wap.fktsv.cn/Article/details/gvnmatihe.sHtML

[U15] Py：高精度计时
来源：http://mobile.epnwcf.com/Article/details/grmavhcaq.sHtML

t = time.perf_counter()
来源：http://wap.fktsv.cn/Article/details/growevxds.sHtML

[U16] Py：命令行参数解析
来源：http://baike.bbcook.cn/Article/details/gbxtbsvod.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.yfazqb.com/Article/details/ghomrpkam.sHtML

[U17] Py：初始化日志
来源：http://www.share.tarul.cn/Article/details/gusweuesr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.vehdjk.com/Article/details/gcpcomize.sHtML

[U18] Py：预编译正则
来源：http://3g.bbcook.cn/Article/details/gveobggrm.sHtML

pat = re.compile(r"\d+")
来源：http://blog.epnwcf.com/Article/details/gnvkbxusv.sHtML


<!-- 参考信息 -->