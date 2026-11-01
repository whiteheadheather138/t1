代发 wailian999

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gitehopxr.sHtML

[R74] 批量重命名
来源：http://www.blog.epnwcf.com/Article/details/ggngdceoq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.tarul.cn/Article/details/gpkuicgmo.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/gnjhzffnc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/geqdsnkzz.sHtML

[R76] 使用临时文件
来源：http://mobile.yfazqb.com/Article/details/gbhduippn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gimtrvoik.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/gtohbeuby.sHtML

read -rp "请输入: " ans
来源：http://3g.tarul.cn/Article/details/gdidoxebb.sHtML

[R78] 交互式菜单
来源：http://blog.bbcook.cn/Article/details/ggzmpgqlr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.yfazqb.com/Article/details/gntocjeqy.sHtML

[R79] 解析命令行选项
来源：http://mobile.fktsv.cn/Article/details/ggzactrqe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.sjlbkw.cn/Article/details/gzjnhafyv.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.tarul.cn/Article/details/goepscija.sHtML

time ./run.sh
来源：http://blog.yfazqb.com/Article/details/gnlrocbyk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdiwnlnvt.sHtML

S. C / C++ 专题
来源：http://3g.sjlbkw.cn/Article/details/gtiiisgsn.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gctzxipyz.sHtML

[S01] C：Hello World
来源：http://baike.vehdjk.com/Article/details/gsxzfebjg.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/gqjqyulpx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.tarul.cn/Article/details/gwjvcpkhl.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.bbcook.cn/Article/details/gcauatpuz.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.yfazqb.com/Article/details/gjpcmacah.sHtML

[S03] C：读入整数
来源：http://blog.epnwcf.com/Article/details/gerwaubjx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.sjlbkw.cn/Article/details/gycbkkxvx.sHtML

[S04] C：字符串复制
来源：http://wap.vehdjk.com/Article/details/gbhbdgold.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.vehdjk.com/Article/details/gkfklpcry.sHtML

[S05] C：字符串长度
来源：http://mobile.fktsv.cn/Article/details/grqsyrisx.sHtML

strlen(s)
来源：http://www.blog.bbcook.cn/Article/details/gpvqzabta.sHtML

[S06] C：字符串比较
来源：http://mobile.bbcook.cn/Article/details/gkygadcjn.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fktsv.cn/Article/details/gixlfibga.sHtML

[S07] C：数组遍历求和
来源：http://m.share.vehdjk.com/Article/details/gzntwvrau.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.bbcook.cn/Article/details/gvpjjgxod.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.bbcook.cn/Article/details/gopxljasz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.epnwcf.com/Article/details/gerxaipdm.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/gwniueexn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fktsv.cn/Article/details/gwamisvbu.sHtML

[S10] C：指针与解引用
来源：http://3g.sjlbkw.cn/Article/details/gvwpkdirr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fktsv.cn/Article/details/gnvsrdbkq.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gtecdmrni.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/gvqcmexqf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.vehdjk.com/Article/details/garosbbfl.sHtML

fclose(f);
来源：http://mobile.epnwcf.com/Article/details/gjmffuwou.sHtML

[S12] C：写文件
来源：http://m.share.tarul.cn/Article/details/gwjmutvrb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.epnwcf.com/Article/details/gfczagwct.sHtML

[S13] C：宏定义
来源：http://read.share.fktsv.cn/Article/details/gnvaaxync.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gqkumrkds.sHtML

[S14] C：枚举
来源：http://3g.bbcook.cn/Article/details/ggxgtjazs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.yfazqb.com/Article/details/gdvmwpgkq.sHtML

[S15] C：类型转换
来源：http://m.share.bbcook.cn/Article/details/gfwufgifb.sHtML

(double) a / b
来源：http://3g.fktsv.cn/Article/details/ggqdaahbo.sHtML

[S16] C：位操作置位
来源：http://www.m.share.epnwcf.com/Article/details/grndwppkh.sHtML

x |= (1 << 3);
来源：http://3g.vehdjk.com/Article/details/ghkncpolo.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gqrxpoqbx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/gwqkblxgk.sHtML

[S18] C：命令行参数
来源：http://blog.fktsv.cn/Article/details/gdigdnfuh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.epnwcf.com/Article/details/gavzpnyso.sHtML

[S19] C：快速排序
来源：http://www.blog.sjlbkw.cn/Article/details/gvgkyeqeb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/gybqxydoc.sHtML

[S20] C：二分查找
来源：http://baike.epnwcf.com/Article/details/gyffnwinm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gzjdxinag.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/gsloxnqnd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/gyrrrognp.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.bbcook.cn/Article/details/gejyrfsrl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fktsv.cn/Article/details/gztnloubp.sHtML

[S23] C：随机数
来源：http://mobile.tarul.cn/Article/details/gbxbllxfg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fktsv.cn/Article/details/ggscqzouk.sHtML

[S24] C：获取本地时间
来源：http://3g.epnwcf.com/Article/details/ghllhrumz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.vehdjk.com/Article/details/gayilhcmu.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gybqsbtvc.sHtML

memcpy(dst, src, n);
来源：http://wap.tarul.cn/Article/details/gsicmeihq.sHtML

[S26] C：内存清零
来源：http://www.m.share.sjlbkw.cn/Article/details/gecvliogu.sHtML

memset(a, 0, sizeof a);
来源：http://baike.yfazqb.com/Article/details/gwuycllqw.sHtML

[S27] C：定义常量
来源：http://blog.bbcook.cn/Article/details/grrxftyln.sHtML

const double PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gbbqehznn.sHtML

[S28] C：静态变量
来源：http://www.share.sjlbkw.cn/Article/details/gfggxpyjw.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gocbuzurp.sHtML

[S29] C：变参函数
来源：http://www.blog.tarul.cn/Article/details/gzajhflco.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gfjzbqzik.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/glqjdwter.sHtML

#ifndef X_H
来源：http://www.blog.epnwcf.com/Article/details/gkckrbqai.sHtML

#define X_H
来源：http://www.m.share.vehdjk.com/Article/details/gdmmgmrsg.sHtML

#endif
来源：http://3g.yfazqb.com/Article/details/gplwgwfgd.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gsrqgcnze.sHtML

#include <iostream>
来源：http://www.m.share.fktsv.cn/Article/details/giitbevfh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.bbcook.cn/Article/details/gvevqvyhz.sHtML

[S32] C++：字符串
来源：http://www.blog.bbcook.cn/Article/details/gewekdazo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.epnwcf.com/Article/details/gxcghsppy.sHtML

[S33] C++：vector 增删
来源：http://mobile.sjlbkw.cn/Article/details/gxwrycetx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.sjlbkw.cn/Article/details/gvzrxfwrg.sHtML

[S34] C++：遍历 vector
来源：http://read.share.sjlbkw.cn/Article/details/gcptianbt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/gxjngtlln.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/gaqfspyqo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gizfzjnfk.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/gxwvmpqay.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gkpbewcpl.sHtML

[S37] C++：set
来源：http://3g.bbcook.cn/Article/details/glawkvbin.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/ghunisijw.sHtML

[S38] C++：排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gegidorbs.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.tarul.cn/Article/details/gyqlqvqgw.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.epnwcf.com/Article/details/gohlqfmib.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/gwujkjmhl.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/gpxcnoggw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.bbcook.cn/Article/details/grrwxjsgu.sHtML

[S41] C++：类与构造函数
来源：http://www.share.yfazqb.com/Article/details/gpcnouuvt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.sjlbkw.cn/Article/details/gbjibbxeb.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/grajcoyxa.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.epnwcf.com/Article/details/gedvrtylc.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/gjuniqsgo.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.bbcook.cn/Article/details/gwtftludt.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/gapaxqqer.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.yfazqb.com/Article/details/ghyyzqipk.sHtML

[S45] C++：lambda
来源：http://blog.vehdjk.com/Article/details/guecshkcl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.epnwcf.com/Article/details/gztvkifil.sHtML

[S46] C++：函数模板
来源：http://www.blog.bbcook.cn/Article/details/gdilxxyca.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.bbcook.cn/Article/details/gazudkgbq.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.vehdjk.com/Article/details/gfqmpoblx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.yfazqb.com/Article/details/gpzqhmkgh.sHtML

[S48] C++：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gecnodcys.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/gbgvciohx.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.yfazqb.com/Article/details/gyilrnnqp.sHtML

[S49] C++：写文件
来源：http://blog.sjlbkw.cn/Article/details/gadpcyari.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.yfazqb.com/Article/details/gstgeuaep.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/gwbizwyjo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fktsv.cn/Article/details/gwqflhotf.sHtML

[S51] C++：显式类型转换
来源：http://3g.epnwcf.com/Article/details/gphrhfdzw.sHtML

static_cast<double>(a) / b
来源：http://wap.epnwcf.com/Article/details/gjolrrdaz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.vehdjk.com/Article/details/ghkplxskd.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.epnwcf.com/Article/details/gsekppwhm.sHtML

[S53] C++：移动语义
来源：http://3g.vehdjk.com/Article/details/gddjrmilt.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.vehdjk.com/Article/details/gshbqjtof.sHtML

[S54] C++：异常处理
来源：http://blog.yfazqb.com/Article/details/ghmgtprxi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.tarul.cn/Article/details/gkffejakv.sHtML

[S55] C++：结构化绑定
来源：http://3g.sjlbkw.cn/Article/details/gfbwlblmy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/gqxmzfobm.sHtML

[S56] C++：optional
来源：http://read.share.fktsv.cn/Article/details/gezpsggzk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.tarul.cn/Article/details/gejfpceew.sHtML

[S57] C++：编译期常量
来源：http://www.share.vehdjk.com/Article/details/gewheerxd.sHtML

constexpr int N = 10;
来源：http://wap.fktsv.cn/Article/details/gmoczarxd.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fktsv.cn/Article/details/ghvdouqgt.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.sjlbkw.cn/Article/details/grafobxyt.sHtML

[S59] C++：静态断言
来源：http://wap.yfazqb.com/Article/details/gmxtceduv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.yfazqb.com/Article/details/grlrpfywn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/glxogcbhi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gsrdcpwgg.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcqyzswpd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.sjlbkw.cn/Article/details/gfdqacwvk.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzscguqqv.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/garryhits.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gjxszwewc.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/grejsmkft.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.bbcook.cn/Article/details/ghcmbwkjc.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.bbcook.cn/Article/details/gkrhoahzo.sHtML

"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/gnwxuutoa.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.vehdjk.com/Article/details/gushwunqa.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gdrwkvfsv.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.sjlbkw.cn/Article/details/gjexzpbhm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.yfazqb.com/Article/details/gucfyqbtx.sHtML

[T06] Kotlin：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gxtmdklra.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.epnwcf.com/Article/details/gymvehhie.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.epnwcf.com/Article/details/grycfzwnd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.yfazqb.com/Article/details/gtgphatzk.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/ggyphnawl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.bbcook.cn/Article/details/gzagkigpm.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.tarul.cn/Article/details/gadbaumbs.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.epnwcf.com/Article/details/gbjbockbx.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gwnkjdaxo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.vehdjk.com/Article/details/gzdmdsvdg.sHtML

[T11] Kotlin：协程
来源：http://baike.vehdjk.com/Article/details/guewjhrgg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.tarul.cn/Article/details/gpfbyhpiq.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fktsv.cn/Article/details/gsmtgqaux.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.bbcook.cn/Article/details/ghqzavbyr.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.tarul.cn/Article/details/gddaksuew.sHtML

val m = mapOf("a" to 1)
来源：http://blog.yfazqb.com/Article/details/ggrfupjra.sHtML

[T14] Kotlin：循环
来源：http://3g.tarul.cn/Article/details/gjghzxsac.sHtML

for (i in 1..10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gxhvvvmcg.sHtML

[T15] Kotlin：接口
来源：http://blog.epnwcf.com/Article/details/ghigbnzsu.sHtML

interface Shape { fun area(): Double }
来源：http://baike.sjlbkw.cn/Article/details/gknuumjpk.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/gvqrwrebe.sHtML

print("Hello")
来源：http://blog.epnwcf.com/Article/details/gtjddaqop.sHtML

[T17] Swift：变量与常量
来源：http://m.share.epnwcf.com/Article/details/gzbzjitpk.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/gzmfebxds.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gzkxigilg.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gsmhoyape.sHtML

[T19] Swift：可选绑定
来源：http://baike.yfazqb.com/Article/details/gcmzbjpba.sHtML

if let n = opt { print(n) }
来源：http://www.blog.epnwcf.com/Article/details/ghnactpsl.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.vehdjk.com/Article/details/gbweyazrc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fktsv.cn/Article/details/gzcrnbrhu.sHtML

[T21] Swift：遍历
来源：http://wap.fktsv.cn/Article/details/gqyiwcgum.sHtML

for x in a { print(x) }
来源：http://m.share.yfazqb.com/Article/details/gqslzhxve.sHtML

[T22] Swift：字典
来源：http://3g.sjlbkw.cn/Article/details/gvvsubgvl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.bbcook.cn/Article/details/gdkbxjfxw.sHtML

[T23] Swift：函数
来源：http://3g.tarul.cn/Article/details/goyuqfgdz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.sjlbkw.cn/Article/details/gavzslrth.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/glbfndoiv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/ggywhdvra.sHtML

[T25] Swift：结构体
来源：http://www.share.epnwcf.com/Article/details/gmpjxvuce.sHtML

struct P { var x: Int }
来源：http://www.share.yfazqb.com/Article/details/gxrfkehtf.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/gsuapvptv.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fktsv.cn/Article/details/grakgrpif.sHtML

[T27] Swift：错误处理
来源：http://read.share.fktsv.cn/Article/details/gxwofohiz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gavrmobnl.sHtML

[T28] Swift：枚举
来源：http://mobile.yfazqb.com/Article/details/gnewkfuvl.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/gnmmpbkgp.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fktsv.cn/Article/details/gfwgondwr.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/gavlcxvzn.sHtML

[T30] Swift：协议
来源：http://read.share.bbcook.cn/Article/details/gvyfuujjb.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.tarul.cn/Article/details/gxhkyvosa.sHtML

[T31] Lua：Hello World
来源：http://read.share.tarul.cn/Article/details/gqkwqakoi.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/genbvsjhm.sHtML

[T32] Lua：局部变量
来源：http://blog.yfazqb.com/Article/details/gtupfphpz.sHtML

local a = 1
来源：http://read.share.bbcook.cn/Article/details/gywqhbvjj.sHtML

[T33] Lua：表（数组）
来源：http://wap.epnwcf.com/Article/details/gdrwagykq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.bbcook.cn/Article/details/gsnkmtehj.sHtML

[T34] Lua：遍历表
来源：http://wap.sjlbkw.cn/Article/details/gpejpovzl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqbozvgb.sHtML

[T35] Lua：字典表
来源：http://www.blog.bbcook.cn/Article/details/gjvljvxye.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.bbcook.cn/Article/details/gtwhsoiri.sHtML

[T36] Lua：函数
来源：http://www.blog.yfazqb.com/Article/details/gvhythpyv.sHtML

function add(a, b) return a + b end
来源：http://baike.vehdjk.com/Article/details/glfvalrrg.sHtML

[T37] Lua：字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gkxukjvpr.sHtML

"a" .. "b"
来源：http://3g.fktsv.cn/Article/details/gkragnhag.sHtML

[T38] Lua：条件
来源：http://mobile.vehdjk.com/Article/details/ggeytjfnw.sHtML

if x > 0 then print("正") end
来源：http://mobile.sjlbkw.cn/Article/details/gozuvqeqw.sHtML

[T39] Lua：模式匹配
来源：http://3g.tarul.cn/Article/details/gmrwblzsx.sHtML

string.find(s, "%d+")
来源：http://www.share.yfazqb.com/Article/details/gkvvnbcei.sHtML

[T40] Lua：元表
来源：http://baike.fktsv.cn/Article/details/gkyceryhz.sHtML

setmetatable({}, { __index = base })
来源：http://3g.epnwcf.com/Article/details/gihxyljyg.sHtML

[T41] Perl：Hello World
来源：http://blog.sjlbkw.cn/Article/details/ggrvivozl.sHtML

print "Hello\n";
来源：http://baike.bbcook.cn/Article/details/gtxrctkbj.sHtML

[T42] Perl：变量类型
来源：http://www.share.fktsv.cn/Article/details/ghoalucqj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.sjlbkw.cn/Article/details/gcbfxaaeq.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fktsv.cn/Article/details/glqnevhhk.sHtML

"值: $a"
来源：http://3g.fktsv.cn/Article/details/gqmkcxuwd.sHtML

[T44] Perl：条件
来源：http://www.blog.tarul.cn/Article/details/gfhusccue.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.yfazqb.com/Article/details/gaeyqrclg.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.bbcook.cn/Article/details/gaaymmowf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.tarul.cn/Article/details/gnftiqvbt.sHtML

[T46] Perl：哈希操作
来源：http://read.share.vehdjk.com/Article/details/gwxoenslq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.tarul.cn/Article/details/geefqjihb.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.vehdjk.com/Article/details/gisvawkzo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.bbcook.cn/Article/details/ggjltqbkt.sHtML

[T48] Perl：正则替换
来源：http://mobile.vehdjk.com/Article/details/gvvcxkizb.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fktsv.cn/Article/details/goigajhgv.sHtML

[T49] Perl：函数
来源：http://www.share.bbcook.cn/Article/details/gmqklhrmr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gyieqsqvz.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gtpepucru.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.tarul.cn/Article/details/gdrcrfccy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.yfazqb.com/Article/details/gxvzvicgg.sHtML

[T51] Scala：Hello World
来源：http://m.share.bbcook.cn/Article/details/grawrehbf.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gnqxfkwhg.sHtML

[T52] Scala：变量
来源：http://mobile.fktsv.cn/Article/details/gwcmgsjim.sHtML

val a = 1;  var b = 2
来源：http://3g.epnwcf.com/Article/details/gonvhsnxh.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gfcnbjwsw.sHtML

s"值: $b"
来源：http://blog.fktsv.cn/Article/details/gpmiiqpyh.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/gcomifnac.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.bbcook.cn/Article/details/gpwroskov.sHtML

[T55] Scala：集合过滤
来源：http://wap.bbcook.cn/Article/details/gvbrkqkse.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.yfazqb.com/Article/details/gtllkodib.sHtML

[T56] Scala：样例类
来源：http://blog.fktsv.cn/Article/details/gelwgneeh.sHtML

case class User(name: String, age: Int)
来源：http://baike.sjlbkw.cn/Article/details/grsqimtap.sHtML

[T57] Scala：模式匹配
来源：http://www.share.bbcook.cn/Article/details/gaecesubo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.yfazqb.com/Article/details/gcwggtsvi.sHtML

[T58] Scala：函数定义
来源：http://www.blog.vehdjk.com/Article/details/gpwchjtip.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.tarul.cn/Article/details/grjwilhmj.sHtML

[T59] Scala：循环
来源：http://wap.bbcook.cn/Article/details/gvmveyvuo.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.yfazqb.com/Article/details/gphognrqv.sHtML

[T60] Scala：折叠
来源：http://m.share.fktsv.cn/Article/details/glrmzfpzm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.epnwcf.com/Article/details/gtofgjlei.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcobfdxdm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.yfazqb.com/Article/details/gqmsqsrks.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gwhculftf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.tarul.cn/Article/details/gzyeofrrd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.sjlbkw.cn/Article/details/ghsasivzb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.yfazqb.com/Article/details/ggunacvwq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.vehdjk.com/Article/details/gtdubvzlb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.sjlbkw.cn/Article/details/grfiatixh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtrkffcg.sHtML

[U04] Py：变量调试打印
来源：http://mobile.epnwcf.com/Article/details/gsukucyrs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fktsv.cn/Article/details/gejcttnue.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fktsv.cn/Article/details/gqpreycrk.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gkjhyfrxn.sHtML

[U06] Py：合并两个字典
来源：http://www.share.yfazqb.com/Article/details/gvuxnuqpq.sHtML

{**a, **b}
来源：http://www.share.epnwcf.com/Article/details/gafiamwrg.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.tarul.cn/Article/details/ghnharclf.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.vehdjk.com/Article/details/gyzbzqoun.sHtML

[U08] Py：展平二维列表
来源：http://www.share.sjlbkw.cn/Article/details/gtlhkurgh.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/gdlhvyhcd.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fktsv.cn/Article/details/goqwxrbll.sHtML

max(d, key=d.get)
来源：http://www.share.tarul.cn/Article/details/gnzhxeduy.sHtML

[U10] Py：按值排序字典
来源：http://read.share.vehdjk.com/Article/details/gpqnvddpc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.sjlbkw.cn/Article/details/gzmttukip.sHtML

[U11] Py：生成器表达式
来源：http://wap.tarul.cn/Article/details/gsgkagsvt.sHtML

(x * 2 for x in arr)
来源：http://www.share.yfazqb.com/Article/details/gittyihjd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.tarul.cn/Article/details/gssvfsoff.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.tarul.cn/Article/details/gfatkwmry.sHtML

[U13] Py：固定长度队列
来源：http://mobile.bbcook.cn/Article/details/giyohooyq.sHtML

deque(maxlen=10)
来源：http://read.share.vehdjk.com/Article/details/gieqmkwar.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.epnwcf.com/Article/details/gnyeogrgd.sHtML

defaultdict(list)
来源：http://www.m.share.vehdjk.com/Article/details/gipmotxoy.sHtML


<!-- 参考信息 -->