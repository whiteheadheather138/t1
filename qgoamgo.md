代发 wailian999

read -rp "请输入: " ans
来源：http://mobile.bbcook.cn/Article/details/gjavmfrmj.sHtML

[R78] 交互式菜单
来源：http://m.share.yfazqb.com/Article/details/gulcwkpqm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.tarul.cn/Article/details/gdimsfpns.sHtML

[R79] 解析命令行选项
来源：http://blog.fktsv.cn/Article/details/glnqwmapm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.yfazqb.com/Article/details/ggyxozxpg.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.bbcook.cn/Article/details/gnbavnngc.sHtML

time ./run.sh
来源：http://www.share.vehdjk.com/Article/details/gazqabmxm.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gddsskjus.sHtML

S. C / C++ 专题
来源：http://www.m.share.yfazqb.com/Article/details/galqkbadb.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkrxipjyj.sHtML

[S01] C：Hello World
来源：http://www.share.bbcook.cn/Article/details/gnossvgrb.sHtML

#include <stdio.h>
来源：http://blog.bbcook.cn/Article/details/gtdvrmmyr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.sjlbkw.cn/Article/details/gbohmbonx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.tarul.cn/Article/details/ghpuzvuvl.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.yfazqb.com/Article/details/gblicjups.sHtML

[S03] C：读入整数
来源：http://www.blog.tarul.cn/Article/details/gbugtgntr.sHtML

int x; scanf("%d", &x);
来源：http://baike.fktsv.cn/Article/details/gcngfcqon.sHtML

[S04] C：字符串复制
来源：http://www.share.bbcook.cn/Article/details/gtxsfphya.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fktsv.cn/Article/details/gokbeefcz.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/gmlpekyqh.sHtML

strlen(s)
来源：http://baike.bbcook.cn/Article/details/gmsrqkbrh.sHtML

[S06] C：字符串比较
来源：http://3g.bbcook.cn/Article/details/gzrehgfmh.sHtML

strcmp(a, b) == 0
来源：http://mobile.epnwcf.com/Article/details/gdgknncjh.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fktsv.cn/Article/details/grahcgpnw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.tarul.cn/Article/details/gjaqctanq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/gxkjerrrk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/gpluazgyc.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.vehdjk.com/Article/details/gyorxeocj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/gjcwhvvsj.sHtML

[S10] C：指针与解引用
来源：http://read.share.bbcook.cn/Article/details/gcoainzza.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/gmagefpdu.sHtML

[S11] C：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gdlfnuwah.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/gkzdawdzd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.vehdjk.com/Article/details/gucxbcvna.sHtML

fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gfdwhplur.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/gbaxrtvns.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/gqllbtquy.sHtML

[S13] C：宏定义
来源：http://baike.sjlbkw.cn/Article/details/gsuokhfwi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.vehdjk.com/Article/details/gnkcfczhj.sHtML

[S14] C：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gwgjwthjf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.epnwcf.com/Article/details/gxqlavknm.sHtML

[S15] C：类型转换
来源：http://blog.vehdjk.com/Article/details/grapgeral.sHtML

(double) a / b
来源：http://www.share.fktsv.cn/Article/details/gwpcxjujl.sHtML

[S16] C：位操作置位
来源：http://www.m.share.bbcook.cn/Article/details/gfyimwwpc.sHtML

x |= (1 << 3);
来源：http://3g.yfazqb.com/Article/details/gywviryvy.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fktsv.cn/Article/details/gotsmoqpk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fktsv.cn/Article/details/gpchsgiuu.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/gbsshmpeb.sHtML

int main(int argc, char **argv)
来源：http://baike.yfazqb.com/Article/details/gkrecwxwh.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/ghvikpdfu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/grigdcuxh.sHtML

[S20] C：二分查找
来源：http://wap.fktsv.cn/Article/details/grfbzfwlp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gdneimvui.sHtML

[S21] C：字符类别判断
来源：http://m.share.fktsv.cn/Article/details/gfsucjskp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/gffwpawuw.sHtML

[S22] C：字符串转数字
来源：http://m.share.yfazqb.com/Article/details/ghzjqeyxp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.tarul.cn/Article/details/gywqitxla.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/grnfvsped.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.sjlbkw.cn/Article/details/gintldqgc.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/gvdxbxttm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.yfazqb.com/Article/details/gwgxcsttc.sHtML

[S25] C：内存拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gaywcztcd.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fktsv.cn/Article/details/gzzeqgjif.sHtML

[S26] C：内存清零
来源：http://www.share.tarul.cn/Article/details/gnhobdarh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.bbcook.cn/Article/details/gpsfhpasr.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/gkwferrbb.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gdvbnrtmn.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/gjzmzzzxx.sHtML

static int counter = 0;
来源：http://wap.vehdjk.com/Article/details/gppctcswb.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/gncfyelzb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.yfazqb.com/Article/details/gsnabwzdt.sHtML

[S30] C：头文件保护
来源：http://blog.bbcook.cn/Article/details/gscfhqvcl.sHtML

#ifndef X_H
来源：http://baike.fktsv.cn/Article/details/gdgrozpfv.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/gscneejgj.sHtML

#endif
来源：http://wap.fktsv.cn/Article/details/gxlazcypb.sHtML

[S31] C++：Hello World
来源：http://baike.tarul.cn/Article/details/gmqrqpqxl.sHtML

#include <iostream>
来源：http://3g.yfazqb.com/Article/details/gdxtptapd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.epnwcf.com/Article/details/gocyrhqhh.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/geunuosxn.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fktsv.cn/Article/details/gjzbxjyzn.sHtML

[S33] C++：vector 增删
来源：http://www.blog.sjlbkw.cn/Article/details/gjafbmycd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.tarul.cn/Article/details/gwvwfeqrg.sHtML

[S34] C++：遍历 vector
来源：http://wap.vehdjk.com/Article/details/gozwobjvn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.bbcook.cn/Article/details/gyeyiwryw.sHtML

[S35] C++：map
来源：http://blog.bbcook.cn/Article/details/gqstwoonh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/grgujjpul.sHtML

[S36] C++：unordered_map
来源：http://wap.vehdjk.com/Article/details/gslvwrhiv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gfilxfypk.sHtML

[S37] C++：set
来源：http://read.share.sjlbkw.cn/Article/details/gsdwsferq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.tarul.cn/Article/details/ghiwyrhio.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/gcoovxqvy.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.epnwcf.com/Article/details/gkpvaocxu.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fktsv.cn/Article/details/gbaygcrdr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.tarul.cn/Article/details/gjocloebp.sHtML

[S40] C++：查找元素
来源：http://blog.sjlbkw.cn/Article/details/gytkroawd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.vehdjk.com/Article/details/gsonkahos.sHtML

[S41] C++：类与构造函数
来源：http://3g.epnwcf.com/Article/details/gfvomvdsx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fktsv.cn/Article/details/ggeltvdtn.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.epnwcf.com/Article/details/gpmweichj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.epnwcf.com/Article/details/gqbtsqbfk.sHtML

[S43] C++：智能指针
来源：http://m.share.vehdjk.com/Article/details/gqcnjuomu.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.yfazqb.com/Article/details/gocnasqqh.sHtML

[S44] C++：引用传参
来源：http://m.share.sjlbkw.cn/Article/details/gwfuntyua.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.bbcook.cn/Article/details/gfozxybxg.sHtML

[S45] C++：lambda
来源：http://mobile.yfazqb.com/Article/details/gsvagmzam.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/gntalxwlz.sHtML

[S46] C++：函数模板
来源：http://www.m.share.bbcook.cn/Article/details/gioxkwwog.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.tarul.cn/Article/details/gzvnvlafj.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.sjlbkw.cn/Article/details/gjhizvjbf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.yfazqb.com/Article/details/gbgsringx.sHtML

[S48] C++：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gzkumnhfz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.epnwcf.com/Article/details/gmvhiwffl.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.yfazqb.com/Article/details/gffexsurp.sHtML

[S49] C++：写文件
来源：http://mobile.yfazqb.com/Article/details/galyguzea.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.bbcook.cn/Article/details/ghexdjtpd.sHtML

[S50] C++：格式化数字
来源：http://www.blog.vehdjk.com/Article/details/gmsqatfng.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gscmifpod.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gwsmkrbrb.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/ggerdmyvv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/ghfbfjqra.sHtML

int size() const noexcept { return n_; }
来源：http://blog.tarul.cn/Article/details/giuqfqzpt.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/gagurzzze.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.bbcook.cn/Article/details/gdnyjdahq.sHtML

[S54] C++：异常处理
来源：http://www.m.share.sjlbkw.cn/Article/details/geemkbsze.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/gvmuoedxc.sHtML

[S55] C++：结构化绑定
来源：http://baike.yfazqb.com/Article/details/gfeermchk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.epnwcf.com/Article/details/gwfgfwgxs.sHtML

[S56] C++：optional
来源：http://www.m.share.yfazqb.com/Article/details/gmbpbmxcp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.sjlbkw.cn/Article/details/gmgfogqqi.sHtML

[S57] C++：编译期常量
来源：http://wap.fktsv.cn/Article/details/gbyfamzqg.sHtML

constexpr int N = 10;
来源：http://wap.vehdjk.com/Article/details/gqortcpfn.sHtML

[S58] C++：命名空间
来源：http://www.m.share.tarul.cn/Article/details/gfdqonzba.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.sjlbkw.cn/Article/details/gcgnfemmj.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/gssqyblsn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/gvxcwzqmb.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.vehdjk.com/Article/details/ggzqitfiz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwyerhpe.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gyylpatkk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/ggmmiiiea.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gvouxqvbo.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/gfpaehxbj.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gixznikmx.sHtML

[T02] Kotlin：变量
来源：http://www.blog.bbcook.cn/Article/details/geywnnuoe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.yfazqb.com/Article/details/gveaixzyp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.epnwcf.com/Article/details/gsscpqoki.sHtML

"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/ggufovkzc.sHtML

[T04] Kotlin：空安全
来源：http://www.share.epnwcf.com/Article/details/getirfphl.sHtML

val n: String? = null;  n?.length
来源：http://www.share.bbcook.cn/Article/details/gwwsklife.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.yfazqb.com/Article/details/gnawrfuuy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.tarul.cn/Article/details/gtmuumosl.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.yfazqb.com/Article/details/gdahavwzo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/gthvdvxho.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fktsv.cn/Article/details/gzvudcigv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.sjlbkw.cn/Article/details/gbhjroucc.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fktsv.cn/Article/details/gkbrnbuiu.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.tarul.cn/Article/details/gsxnhrzht.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.sjlbkw.cn/Article/details/gcqivdmvk.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.vehdjk.com/Article/details/gaoftonoy.sHtML

[T10] Kotlin：默认参数
来源：http://3g.vehdjk.com/Article/details/gvbajblmt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.yfazqb.com/Article/details/gltuyuphu.sHtML

[T11] Kotlin：协程
来源：http://m.share.tarul.cn/Article/details/glipdsqeo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.tarul.cn/Article/details/gdykznlyx.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.bbcook.cn/Article/details/gwjyllsvx.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.tarul.cn/Article/details/gynawhapn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.tarul.cn/Article/details/gxuoneuuo.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.bbcook.cn/Article/details/ghbvydbjx.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gxkutcpbd.sHtML

for (i in 1..10) println(i)
来源：http://blog.bbcook.cn/Article/details/gxiedtgma.sHtML

[T15] Kotlin：接口
来源：http://mobile.tarul.cn/Article/details/gsngmpklw.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.sjlbkw.cn/Article/details/gofmsuzzf.sHtML

[T16] Swift：Hello World
来源：http://www.share.bbcook.cn/Article/details/gvmemzeoz.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/gdvlbsykp.sHtML

[T17] Swift：变量与常量
来源：http://baike.epnwcf.com/Article/details/gxcuxffpt.sHtML

var a = 1;  let b = 2
来源：http://read.share.tarul.cn/Article/details/gnnfnrtpd.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gbnfjbdgl.sHtML

"值: \(b)"
来源：http://wap.epnwcf.com/Article/details/gsupesevx.sHtML

[T19] Swift：可选绑定
来源：http://mobile.tarul.cn/Article/details/gryuhibyp.sHtML

if let n = opt { print(n) }
来源：http://blog.fktsv.cn/Article/details/gbjewcgyi.sHtML

[T20] Swift：数组操作
来源：http://www.share.vehdjk.com/Article/details/gfrqaehkf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.bbcook.cn/Article/details/gqflwjxph.sHtML

[T21] Swift：遍历
来源：http://m.share.epnwcf.com/Article/details/ghrhkuyfk.sHtML

for x in a { print(x) }
来源：http://baike.epnwcf.com/Article/details/gvjtomach.sHtML

[T22] Swift：字典
来源：http://3g.fktsv.cn/Article/details/gavjfqiqj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.yfazqb.com/Article/details/gphopvbfz.sHtML

[T23] Swift：函数
来源：http://mobile.sjlbkw.cn/Article/details/ghltdorit.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.vehdjk.com/Article/details/gdukfojng.sHtML

[T24] Swift：闭包
来源：http://baike.sjlbkw.cn/Article/details/gozegxgsj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gqpugkeno.sHtML

[T25] Swift：结构体
来源：http://www.share.bbcook.cn/Article/details/gqflpfrof.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/gaeyipgtp.sHtML

[T26] Swift：类与重写
来源：http://wap.tarul.cn/Article/details/gvrixaztt.sHtML

class A: Base { override func f() {} }
来源：http://www.share.sjlbkw.cn/Article/details/gkfljmphx.sHtML

[T27] Swift：错误处理
来源：http://baike.fktsv.cn/Article/details/gjxsczhui.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fktsv.cn/Article/details/gctrczahl.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/glirgkkpc.sHtML

enum Color { case red, green }
来源：http://baike.yfazqb.com/Article/details/gbcpihdir.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.epnwcf.com/Article/details/gkkjyiodo.sHtML

guard let x = opt else { return }
来源：http://read.share.yfazqb.com/Article/details/grhimqifm.sHtML

[T30] Swift：协议
来源：http://mobile.tarul.cn/Article/details/guydqhzni.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.bbcook.cn/Article/details/gghfjkocy.sHtML

[T31] Lua：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/ggoqmmmew.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gzmrvkbjd.sHtML

[T32] Lua：局部变量
来源：http://m.share.fktsv.cn/Article/details/gxglmzsyv.sHtML

local a = 1
来源：http://wap.tarul.cn/Article/details/ghyqrawjt.sHtML

[T33] Lua：表（数组）
来源：http://blog.fktsv.cn/Article/details/gcwgwkhox.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.yfazqb.com/Article/details/gqoqlyryt.sHtML

[T34] Lua：遍历表
来源：http://www.blog.yfazqb.com/Article/details/gogdeioax.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.tarul.cn/Article/details/guiaxoeve.sHtML

[T35] Lua：字典表
来源：http://mobile.fktsv.cn/Article/details/gnpleypya.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.bbcook.cn/Article/details/geowclliz.sHtML

[T36] Lua：函数
来源：http://mobile.tarul.cn/Article/details/goredkpsq.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfwzwfhx.sHtML

[T37] Lua：字符串拼接
来源：http://baike.bbcook.cn/Article/details/gpmwvvyvl.sHtML

"a" .. "b"
来源：http://m.share.epnwcf.com/Article/details/gxqxpwqpz.sHtML

[T38] Lua：条件
来源：http://baike.yfazqb.com/Article/details/gqxgxskju.sHtML

if x > 0 then print("正") end
来源：http://wap.bbcook.cn/Article/details/gdoupvjiv.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fktsv.cn/Article/details/gdsxagbae.sHtML

string.find(s, "%d+")
来源：http://www.blog.vehdjk.com/Article/details/gfyblmdou.sHtML

[T40] Lua：元表
来源：http://m.share.yfazqb.com/Article/details/goadmwcbw.sHtML

setmetatable({}, { __index = base })
来源：http://baike.yfazqb.com/Article/details/glfgptfkv.sHtML

[T41] Perl：Hello World
来源：http://www.share.fktsv.cn/Article/details/gjtjxyfke.sHtML

print "Hello\n";
来源：http://baike.tarul.cn/Article/details/gljxnroht.sHtML

[T42] Perl：变量类型
来源：http://baike.vehdjk.com/Article/details/gajdbjvjx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.yfazqb.com/Article/details/gosnzqafm.sHtML

[T43] Perl：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gaajhlbzv.sHtML

"值: $a"
来源：http://blog.bbcook.cn/Article/details/grcisuwft.sHtML

[T44] Perl：条件
来源：http://www.share.bbcook.cn/Article/details/gbfslsrdd.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.bbcook.cn/Article/details/gqdofmyae.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.yfazqb.com/Article/details/gphnwokus.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.epnwcf.com/Article/details/gmualpfyc.sHtML

[T46] Perl：哈希操作
来源：http://www.share.epnwcf.com/Article/details/gfutyshcs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.vehdjk.com/Article/details/guqvfwwpu.sHtML

[T47] Perl：正则捕获
来源：http://wap.epnwcf.com/Article/details/gdvaqzavh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fktsv.cn/Article/details/gakxztbcj.sHtML

[T48] Perl：正则替换
来源：http://wap.vehdjk.com/Article/details/grooazcdh.sHtML

$s =~ s/old/new/g;
来源：http://www.share.bbcook.cn/Article/details/gznzonjnl.sHtML

[T49] Perl：函数
来源：http://blog.sjlbkw.cn/Article/details/grbpxlype.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/ghmnavlhp.sHtML

[T50] Perl：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gmfnqdvwf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.epnwcf.com/Article/details/gaujbaxgx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdkqujift.sHtML

[T51] Scala：Hello World
来源：http://m.share.vehdjk.com/Article/details/ggwizaktx.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gcnmlxjmc.sHtML

[T52] Scala：变量
来源：http://mobile.bbcook.cn/Article/details/gdbliolbb.sHtML

val a = 1;  var b = 2
来源：http://baike.yfazqb.com/Article/details/gygifsrkr.sHtML

[T53] Scala：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gqekeczdz.sHtML

s"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gzjlzbgsi.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/gceptisle.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fktsv.cn/Article/details/gjnhayrmo.sHtML

[T55] Scala：集合过滤
来源：http://blog.tarul.cn/Article/details/gtkweprui.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.bbcook.cn/Article/details/ggmtwndqy.sHtML

[T56] Scala：样例类
来源：http://read.share.bbcook.cn/Article/details/glnkfggxu.sHtML

case class User(name: String, age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/ghzczrsqu.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gokmrishs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuctoygs.sHtML

[T58] Scala：函数定义
来源：http://mobile.epnwcf.com/Article/details/gpvzqjgmb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.sjlbkw.cn/Article/details/gglsiftqs.sHtML

[T59] Scala：循环
来源：http://read.share.bbcook.cn/Article/details/gafzwdgil.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gubxbgrwv.sHtML

[T60] Scala：折叠
来源：http://wap.epnwcf.com/Article/details/gwaivasco.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.epnwcf.com/Article/details/gxtuioipl.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gwyqlxqzm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/globwynwh.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcwccmlny.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.bbcook.cn/Article/details/gmuwufrrr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.sjlbkw.cn/Article/details/gbipcxnri.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fktsv.cn/Article/details/gfovvqiif.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.epnwcf.com/Article/details/gbzgqqfwb.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.epnwcf.com/Article/details/gwazldhms.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.vehdjk.com/Article/details/gqftmjzdh.sHtML

[U04] Py：变量调试打印
来源：http://read.share.sjlbkw.cn/Article/details/gqpqqvlut.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.tarul.cn/Article/details/gvdbvevtr.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fktsv.cn/Article/details/glvpafoaz.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gvudntlku.sHtML

[U06] Py：合并两个字典
来源：http://mobile.vehdjk.com/Article/details/ggmapizma.sHtML

{**a, **b}
来源：http://www.blog.bbcook.cn/Article/details/gcqodkbfu.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.sjlbkw.cn/Article/details/glqqrjlbx.sHtML

{v: k for k, v in d.items()}
来源：http://blog.epnwcf.com/Article/details/gsohfjlew.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.tarul.cn/Article/details/gqaebhpyg.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/glmrsutfy.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.yfazqb.com/Article/details/gsfhcmdvt.sHtML

max(d, key=d.get)
来源：http://read.share.vehdjk.com/Article/details/gkmyvbcjw.sHtML

[U10] Py：按值排序字典
来源：http://read.share.yfazqb.com/Article/details/gfmxhquok.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fktsv.cn/Article/details/gktbwmseg.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fktsv.cn/Article/details/gnkuaillm.sHtML

(x * 2 for x in arr)
来源：http://baike.tarul.cn/Article/details/gkcefxztq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.epnwcf.com/Article/details/gnkcnhpui.sHtML

Counter(arr).most_common(3)
来源：http://m.share.tarul.cn/Article/details/gfuvmmkeb.sHtML

[U13] Py：固定长度队列
来源：http://read.share.yfazqb.com/Article/details/gopuieihe.sHtML

deque(maxlen=10)
来源：http://blog.sjlbkw.cn/Article/details/gwnleygnm.sHtML

[U14] Py：分组收集到列表
来源：http://wap.tarul.cn/Article/details/gkulxsftg.sHtML

defaultdict(list)
来源：http://www.m.share.yfazqb.com/Article/details/gkxhdlcqo.sHtML

[U15] Py：高精度计时
来源：http://m.share.tarul.cn/Article/details/gnwqpktoq.sHtML

t = time.perf_counter()
来源：http://blog.fktsv.cn/Article/details/gkogeepee.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.vehdjk.com/Article/details/gwcherxjf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.epnwcf.com/Article/details/gxsdfsjwl.sHtML

[U17] Py：初始化日志
来源：http://www.blog.sjlbkw.cn/Article/details/gzrwzxbqq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.tarul.cn/Article/details/gukgnwxhm.sHtML

[U18] Py：预编译正则
来源：http://3g.bbcook.cn/Article/details/gsbfhjrdd.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.bbcook.cn/Article/details/gfvvnygns.sHtML


<!-- 参考信息 -->