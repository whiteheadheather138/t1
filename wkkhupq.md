代发 wailian999

read -rp "请输入: " ans
来源：http://baike.sjlbkw.cn/Article/details/gmzalzasy.sHtML

[R78] 交互式菜单
来源：http://3g.vehdjk.com/Article/details/gksdpswur.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gpawnucrq.sHtML

[R79] 解析命令行选项
来源：http://wap.sjlbkw.cn/Article/details/gmbfjbghh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.sjlbkw.cn/Article/details/gqqrfsjpl.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.vehdjk.com/Article/details/gkhpfkcxl.sHtML

time ./run.sh
来源：http://read.share.fktsv.cn/Article/details/gxrhmwlvz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpymszccs.sHtML

S. C / C++ 专题
来源：http://m.share.fktsv.cn/Article/details/groejklyc.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/goamqvwtz.sHtML

[S01] C：Hello World
来源：http://blog.epnwcf.com/Article/details/gtazwfvgk.sHtML

#include <stdio.h>
来源：http://blog.fktsv.cn/Article/details/gonsujsvb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fktsv.cn/Article/details/guddzloch.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.bbcook.cn/Article/details/gahydowxm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/gktwmgabf.sHtML

[S03] C：读入整数
来源：http://baike.fktsv.cn/Article/details/gbvxrcyxb.sHtML

int x; scanf("%d", &x);
来源：http://baike.epnwcf.com/Article/details/gdimjymje.sHtML

[S04] C：字符串复制
来源：http://blog.sjlbkw.cn/Article/details/gjeiaasfu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/gpmpibhey.sHtML

[S05] C：字符串长度
来源：http://blog.vehdjk.com/Article/details/gaqylahom.sHtML

strlen(s)
来源：http://www.m.share.bbcook.cn/Article/details/gnphpacdf.sHtML

[S06] C：字符串比较
来源：http://baike.yfazqb.com/Article/details/gvirokmnd.sHtML

strcmp(a, b) == 0
来源：http://mobile.vehdjk.com/Article/details/gkylgqccc.sHtML

[S07] C：数组遍历求和
来源：http://www.share.yfazqb.com/Article/details/gpqzjhlzv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/goojhsbph.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.tarul.cn/Article/details/gynxfwagg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.yfazqb.com/Article/details/gbqndjiyj.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.yfazqb.com/Article/details/gqzkrutfd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fktsv.cn/Article/details/gqrcucxzn.sHtML

[S10] C：指针与解引用
来源：http://www.share.sjlbkw.cn/Article/details/gwjbbydna.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.yfazqb.com/Article/details/gywxrjpnf.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gdptogxpe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.yfazqb.com/Article/details/gbqoxpsil.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.sjlbkw.cn/Article/details/gdihtvfrl.sHtML

fclose(f);
来源：http://wap.tarul.cn/Article/details/gmgcksveq.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/gggchrevx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gpjmtfrbw.sHtML

[S13] C：宏定义
来源：http://3g.sjlbkw.cn/Article/details/gsgnqexvv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.bbcook.cn/Article/details/gqpusmbic.sHtML

[S14] C：枚举
来源：http://baike.tarul.cn/Article/details/ghumgnsck.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.bbcook.cn/Article/details/gltamomcx.sHtML

[S15] C：类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gvijspvwy.sHtML

(double) a / b
来源：http://mobile.vehdjk.com/Article/details/gsdjqlkbg.sHtML

[S16] C：位操作置位
来源：http://m.share.tarul.cn/Article/details/gnsacmblf.sHtML

x |= (1 << 3);
来源：http://blog.epnwcf.com/Article/details/gzarmdtnc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fktsv.cn/Article/details/gajmtwsyf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.bbcook.cn/Article/details/gmjeyeeao.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/ggdjhvakr.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/givlagahh.sHtML

[S19] C：快速排序
来源：http://baike.vehdjk.com/Article/details/gzyckuebh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gxmisdlct.sHtML

[S20] C：二分查找
来源：http://baike.fktsv.cn/Article/details/gcnxgobkj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gzoztakla.sHtML

[S21] C：字符类别判断
来源：http://www.share.yfazqb.com/Article/details/gydxlsvqh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fktsv.cn/Article/details/gugheukzy.sHtML

[S22] C：字符串转数字
来源：http://blog.bbcook.cn/Article/details/gjqasuutd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.epnwcf.com/Article/details/ggbdhykez.sHtML

[S23] C：随机数
来源：http://www.share.fktsv.cn/Article/details/goqnkvcnb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.yfazqb.com/Article/details/gaqvtndgb.sHtML

[S24] C：获取本地时间
来源：http://www.share.bbcook.cn/Article/details/ggjnzqhak.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.tarul.cn/Article/details/guhdhvcqw.sHtML

[S25] C：内存拷贝
来源：http://m.share.epnwcf.com/Article/details/gbshbktoq.sHtML

memcpy(dst, src, n);
来源：http://blog.vehdjk.com/Article/details/gnfuonuss.sHtML

[S26] C：内存清零
来源：http://www.blog.vehdjk.com/Article/details/gcieaxwpv.sHtML

memset(a, 0, sizeof a);
来源：http://baike.yfazqb.com/Article/details/gibjwbczf.sHtML

[S27] C：定义常量
来源：http://www.m.share.vehdjk.com/Article/details/gwkpqsgjn.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gzdsrxugi.sHtML

[S28] C：静态变量
来源：http://wap.tarul.cn/Article/details/glowtwzoo.sHtML

static int counter = 0;
来源：http://read.share.bbcook.cn/Article/details/gdjzeswre.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/gjauygygb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gnzaqmnlw.sHtML

[S30] C：头文件保护
来源：http://mobile.fktsv.cn/Article/details/glatzhjbs.sHtML

#ifndef X_H
来源：http://wap.epnwcf.com/Article/details/glqyexdik.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/gfbypyymh.sHtML

#endif
来源：http://read.share.sjlbkw.cn/Article/details/gednnlnju.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gabscyjan.sHtML

#include <iostream>
来源：http://mobile.sjlbkw.cn/Article/details/gtkajfojd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.bbcook.cn/Article/details/gntskyefp.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/grjmdlnwf.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fktsv.cn/Article/details/gglmpacau.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.tarul.cn/Article/details/gzzhkwlvy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.tarul.cn/Article/details/gnwrrvsix.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/gekspkbbv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fktsv.cn/Article/details/gdutcjunl.sHtML

[S35] C++：map
来源：http://www.blog.fktsv.cn/Article/details/gkxrlvdss.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gbleugkyd.sHtML

[S36] C++：unordered_map
来源：http://3g.yfazqb.com/Article/details/gkcuvvbrt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gtuxozdup.sHtML

[S37] C++：set
来源：http://www.blog.tarul.cn/Article/details/gefheumxy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.yfazqb.com/Article/details/gbkbxagix.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gmhpjaqdq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/gsbsfkdbw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/gpcxxkbna.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.tarul.cn/Article/details/gbqwoiogt.sHtML

[S40] C++：查找元素
来源：http://3g.bbcook.cn/Article/details/gcxwtgklc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.bbcook.cn/Article/details/gtjwttbit.sHtML

[S41] C++：类与构造函数
来源：http://baike.fktsv.cn/Article/details/gnazlavdb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fktsv.cn/Article/details/gndvefrtk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/gayyjbjwp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gmuwdnzgm.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/ggsllbrte.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.epnwcf.com/Article/details/ggqrtievm.sHtML

[S44] C++：引用传参
来源：http://3g.epnwcf.com/Article/details/gmwhylwfb.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fktsv.cn/Article/details/gkejgaikc.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/glohjhojs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gqodfavpl.sHtML

[S46] C++：函数模板
来源：http://baike.tarul.cn/Article/details/giaqljlmk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/gkbfaybyk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fktsv.cn/Article/details/gpooxncyu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.epnwcf.com/Article/details/gpncsqlmm.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gixqihicz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.epnwcf.com/Article/details/gnshymxju.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gyfbzowon.sHtML

[S49] C++：写文件
来源：http://m.share.bbcook.cn/Article/details/gymtiqzbd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.yfazqb.com/Article/details/gfgqtigxy.sHtML

[S50] C++：格式化数字
来源：http://www.share.yfazqb.com/Article/details/gqohraxcx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gxtnvvlpq.sHtML

[S51] C++：显式类型转换
来源：http://read.share.sjlbkw.cn/Article/details/getahhjck.sHtML

static_cast<double>(a) / b
来源：http://blog.sjlbkw.cn/Article/details/grozotjoc.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/glgdutbwg.sHtML

int size() const noexcept { return n_; }
来源：http://baike.tarul.cn/Article/details/guzbummop.sHtML

[S53] C++：移动语义
来源：http://www.m.share.vehdjk.com/Article/details/gcsplllfr.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.sjlbkw.cn/Article/details/gfrpuxfza.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gghzgthav.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.vehdjk.com/Article/details/gaqkcfjwr.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gbytwyomk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.bbcook.cn/Article/details/gfgtotpko.sHtML

[S56] C++：optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnudvdcu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.vehdjk.com/Article/details/gknrkfukr.sHtML

[S57] C++：编译期常量
来源：http://mobile.bbcook.cn/Article/details/gpgoygolh.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/gbnukrvfk.sHtML

[S58] C++：命名空间
来源：http://blog.tarul.cn/Article/details/gjaeulvpi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/gksycsmdk.sHtML

[S59] C++：静态断言
来源：http://3g.bbcook.cn/Article/details/gurxdipbp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/gopvumszl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.bbcook.cn/Article/details/gxldglbla.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.vehdjk.com/Article/details/gqtmbluxl.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghrqjplfe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.bbcook.cn/Article/details/gzzszbcdc.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gyccnpoxq.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gmypbzjrm.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gfiarzhst.sHtML

[T02] Kotlin：变量
来源：http://3g.vehdjk.com/Article/details/gkmytggwv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.bbcook.cn/Article/details/grrlzbvkc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfvikbmb.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gyjqzmxgl.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fktsv.cn/Article/details/gaijuibte.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/gdjzvzpcy.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/gysvdsgtj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gujsapupy.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fktsv.cn/Article/details/gitidurez.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gruzlhkbs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gdjuymibo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.vehdjk.com/Article/details/grtpjgrvj.sHtML

[T08] Kotlin：数据类
来源：http://wap.sjlbkw.cn/Article/details/gedoyrszf.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.epnwcf.com/Article/details/gikznxegp.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.sjlbkw.cn/Article/details/gzpjueyos.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.bbcook.cn/Article/details/gwqedupdp.sHtML

[T10] Kotlin：默认参数
来源：http://baike.epnwcf.com/Article/details/gbegtmrsx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.sjlbkw.cn/Article/details/guatiqfht.sHtML

[T11] Kotlin：协程
来源：http://baike.fktsv.cn/Article/details/gidqpccpd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.vehdjk.com/Article/details/gefcuztrr.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.vehdjk.com/Article/details/grfngnqgp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gzkdpqqlf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fktsv.cn/Article/details/gvgzdfvaa.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/gathplxqc.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/gczkabtvz.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gnzrhbtns.sHtML

[T15] Kotlin：接口
来源：http://3g.vehdjk.com/Article/details/gqhnvzdbe.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.vehdjk.com/Article/details/ggdhzgddv.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gwzbtldhw.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gmgghzadx.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fktsv.cn/Article/details/gbxzjqsmz.sHtML

var a = 1;  let b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gqnmapelh.sHtML

[T18] Swift：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gesxusfdk.sHtML

"值: \(b)"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfogbwrd.sHtML

[T19] Swift：可选绑定
来源：http://read.share.yfazqb.com/Article/details/gvigaeyfr.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/grnnsjaqf.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/grlzwoyea.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.bbcook.cn/Article/details/gggqeupwt.sHtML

[T21] Swift：遍历
来源：http://wap.fktsv.cn/Article/details/gzdaslslf.sHtML

for x in a { print(x) }
来源：http://3g.tarul.cn/Article/details/gjfjzynog.sHtML

[T22] Swift：字典
来源：http://mobile.vehdjk.com/Article/details/gvhbysjkk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.vehdjk.com/Article/details/gxeldbluk.sHtML

[T23] Swift：函数
来源：http://baike.vehdjk.com/Article/details/gmupwbgni.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fktsv.cn/Article/details/gjnprzmvy.sHtML

[T24] Swift：闭包
来源：http://www.share.epnwcf.com/Article/details/ggemxzddv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gtcdhseeo.sHtML

[T25] Swift：结构体
来源：http://www.share.yfazqb.com/Article/details/gkkbkybra.sHtML

struct P { var x: Int }
来源：http://blog.epnwcf.com/Article/details/gjllxmrjn.sHtML

[T26] Swift：类与重写
来源：http://m.share.fktsv.cn/Article/details/gsdfmkdez.sHtML

class A: Base { override func f() {} }
来源：http://m.share.tarul.cn/Article/details/gejlbllls.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gmsoktiie.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.epnwcf.com/Article/details/gpznwyjwx.sHtML

[T28] Swift：枚举
来源：http://read.share.fktsv.cn/Article/details/gkosxxaai.sHtML

enum Color { case red, green }
来源：http://wap.fktsv.cn/Article/details/gzgfqupbn.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fktsv.cn/Article/details/gbwfizavg.sHtML

guard let x = opt else { return }
来源：http://wap.sjlbkw.cn/Article/details/gllssenmr.sHtML

[T30] Swift：协议
来源：http://www.blog.bbcook.cn/Article/details/gqgqbgkgf.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.sjlbkw.cn/Article/details/gznputffx.sHtML

[T31] Lua：Hello World
来源：http://mobile.vehdjk.com/Article/details/gdeznlnah.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gkrzcggml.sHtML

[T32] Lua：局部变量
来源：http://www.share.fktsv.cn/Article/details/gsriwkgtf.sHtML

local a = 1
来源：http://baike.yfazqb.com/Article/details/gmotwgcxo.sHtML

[T33] Lua：表（数组）
来源：http://mobile.epnwcf.com/Article/details/gfyhpbkpi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.tarul.cn/Article/details/gkaeunewz.sHtML

[T34] Lua：遍历表
来源：http://wap.fktsv.cn/Article/details/gddsdsduh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/gfvtykjkn.sHtML

[T35] Lua：字典表
来源：http://3g.fktsv.cn/Article/details/grdganfnx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.sjlbkw.cn/Article/details/gscsckcyk.sHtML

[T36] Lua：函数
来源：http://www.share.epnwcf.com/Article/details/gcmzyzpqd.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.tarul.cn/Article/details/gbjiakace.sHtML

[T37] Lua：字符串拼接
来源：http://wap.bbcook.cn/Article/details/gqzdzjtkx.sHtML

"a" .. "b"
来源：http://baike.epnwcf.com/Article/details/glgjglayn.sHtML

[T38] Lua：条件
来源：http://baike.sjlbkw.cn/Article/details/gfwwnracm.sHtML

if x > 0 then print("正") end
来源：http://wap.fktsv.cn/Article/details/gervrzema.sHtML

[T39] Lua：模式匹配
来源：http://www.share.bbcook.cn/Article/details/gqeaeqwjy.sHtML

string.find(s, "%d+")
来源：http://www.blog.vehdjk.com/Article/details/gxzatmtmv.sHtML

[T40] Lua：元表
来源：http://3g.fktsv.cn/Article/details/ggmoitxna.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fktsv.cn/Article/details/ggzzoavzf.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gdntdykic.sHtML

print "Hello\n";
来源：http://m.share.tarul.cn/Article/details/gotblwnbw.sHtML

[T42] Perl：变量类型
来源：http://m.share.sjlbkw.cn/Article/details/ggehzcnuo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.epnwcf.com/Article/details/gqkxdthyb.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fktsv.cn/Article/details/grtxruzjw.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/guquvhasa.sHtML

[T44] Perl：条件
来源：http://mobile.yfazqb.com/Article/details/goptayflm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/gkxrgmirz.sHtML

[T45] Perl：数组遍历
来源：http://www.share.sjlbkw.cn/Article/details/gfamdpgnw.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fktsv.cn/Article/details/gvqmvpaqi.sHtML

[T46] Perl：哈希操作
来源：http://mobile.yfazqb.com/Article/details/geatrymdl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.yfazqb.com/Article/details/gdbdnofjc.sHtML

[T47] Perl：正则捕获
来源：http://mobile.epnwcf.com/Article/details/gwylixqym.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.yfazqb.com/Article/details/geujxokrs.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fktsv.cn/Article/details/gdjnupgwd.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/geeelajsu.sHtML

[T49] Perl：函数
来源：http://read.share.bbcook.cn/Article/details/grzxhtdal.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gwnubkjyh.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gptcnpkir.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.epnwcf.com/Article/details/goenswtzw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.tarul.cn/Article/details/gagtbzutv.sHtML

[T51] Scala：Hello World
来源：http://blog.tarul.cn/Article/details/gursvlrrn.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/goamgoedn.sHtML

[T52] Scala：变量
来源：http://wap.bbcook.cn/Article/details/ganwiroyn.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gqsjtyfth.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gskxbuyux.sHtML

s"值: $b"
来源：http://m.share.bbcook.cn/Article/details/gtwptdwfy.sHtML

[T54] Scala：集合映射
来源：http://wap.vehdjk.com/Article/details/gvmbwrwxj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.yfazqb.com/Article/details/gqyzderxu.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fktsv.cn/Article/details/gmkgawduz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fktsv.cn/Article/details/gleymzfvv.sHtML

[T56] Scala：样例类
来源：http://3g.fktsv.cn/Article/details/guppgvong.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/grwsnlvkn.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/gjjineuxi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.vehdjk.com/Article/details/gkfggbhyb.sHtML

[T58] Scala：函数定义
来源：http://3g.tarul.cn/Article/details/grxedkfzu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.epnwcf.com/Article/details/givdaqihz.sHtML

[T59] Scala：循环
来源：http://baike.yfazqb.com/Article/details/gsslmyohh.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.tarul.cn/Article/details/gusmjfhtt.sHtML

[T60] Scala：折叠
来源：http://www.blog.fktsv.cn/Article/details/gdhuuqktq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.tarul.cn/Article/details/ggwjdkqtp.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gczgrouxq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.yfazqb.com/Article/details/gskpmahov.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gigzpcogx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.bbcook.cn/Article/details/ggijtzito.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.bbcook.cn/Article/details/gafklwmmz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.yfazqb.com/Article/details/gjohbmfif.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.yfazqb.com/Article/details/gxgphpcff.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fktsv.cn/Article/details/galscnzpk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.vehdjk.com/Article/details/gsxdmzold.sHtML

[U04] Py：变量调试打印
来源：http://www.share.vehdjk.com/Article/details/gamytyaxy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.sjlbkw.cn/Article/details/gkalykbvw.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/gqwllwuma.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gpjctiwru.sHtML

[U06] Py：合并两个字典
来源：http://m.share.sjlbkw.cn/Article/details/gafkwykaq.sHtML

{**a, **b}
来源：http://m.share.yfazqb.com/Article/details/gbtxbfugr.sHtML

[U07] Py：反转字典键值
来源：http://mobile.yfazqb.com/Article/details/gtpeqhdqd.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.yfazqb.com/Article/details/gmxkknoth.sHtML

[U08] Py：展平二维列表
来源：http://mobile.yfazqb.com/Article/details/gqoffnagg.sHtML

[y for x in nested for y in x]
来源：http://3g.fktsv.cn/Article/details/gqurvsaqj.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.yfazqb.com/Article/details/gpoxysjvj.sHtML

max(d, key=d.get)
来源：http://blog.epnwcf.com/Article/details/gcsgrudvj.sHtML

[U10] Py：按值排序字典
来源：http://m.share.yfazqb.com/Article/details/gkaifzodp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.tarul.cn/Article/details/gillyzzuz.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fktsv.cn/Article/details/gswzmrquf.sHtML

(x * 2 for x in arr)
来源：http://3g.tarul.cn/Article/details/gtmjxqhyc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.yfazqb.com/Article/details/ghznzztzw.sHtML

Counter(arr).most_common(3)
来源：http://www.share.bbcook.cn/Article/details/gqwassduc.sHtML

[U13] Py：固定长度队列
来源：http://baike.tarul.cn/Article/details/gkqrbrwnf.sHtML

deque(maxlen=10)
来源：http://www.share.bbcook.cn/Article/details/ggsquqnra.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.sjlbkw.cn/Article/details/gwufuabzw.sHtML

defaultdict(list)
来源：http://blog.sjlbkw.cn/Article/details/glwrywwyc.sHtML

[U15] Py：高精度计时
来源：http://www.blog.yfazqb.com/Article/details/godscgzix.sHtML

t = time.perf_counter()
来源：http://m.share.bbcook.cn/Article/details/grmjmpnnx.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.epnwcf.com/Article/details/gxslvrwhn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.vehdjk.com/Article/details/gglonrlxh.sHtML

[U17] Py：初始化日志
来源：http://3g.epnwcf.com/Article/details/gfymqfxoz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.yfazqb.com/Article/details/gmminrvmp.sHtML

[U18] Py：预编译正则
来源：http://baike.tarul.cn/Article/details/gjmdxbyhs.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.epnwcf.com/Article/details/gcytuyekp.sHtML


<!-- 参考信息 -->