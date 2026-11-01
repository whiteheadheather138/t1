代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.blog.tarul.cn/Article/details/gvdqqfkoi.sHtML

[R70] 时间戳与互转
来源：http://mobile.fktsv.cn/Article/details/gzirxndup.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/gildhihab.sHtML

[R71] 日期格式化
来源：http://3g.yfazqb.com/Article/details/ghkeoxand.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.tarul.cn/Article/details/gjnujlpxd.sHtML

[R72] 等待端口就绪
来源：http://blog.yfazqb.com/Article/details/gwvixwuea.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gjmwjsrxa.sHtML

[R73] 分割大日志
来源：http://www.share.yfazqb.com/Article/details/gmewctddk.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gpyqpngks.sHtML

[R74] 批量重命名
来源：http://www.blog.bbcook.cn/Article/details/gczedhuyy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.bbcook.cn/Article/details/gvypctegn.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/gdaqoqzew.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.epnwcf.com/Article/details/glmbyryah.sHtML

[R76] 使用临时文件
来源：http://m.share.yfazqb.com/Article/details/gxqyaodsv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/geenkzhkp.sHtML

[R77] 读取用户输入
来源：http://blog.vehdjk.com/Article/details/gjdhiufng.sHtML

read -rp "请输入: " ans
来源：http://m.share.epnwcf.com/Article/details/glioivqmg.sHtML

[R78] 交互式菜单
来源：http://baike.yfazqb.com/Article/details/godarvoxm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.bbcook.cn/Article/details/gagwrryno.sHtML

[R79] 解析命令行选项
来源：http://baike.sjlbkw.cn/Article/details/gzajfjmwu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.tarul.cn/Article/details/gapvdnphi.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.sjlbkw.cn/Article/details/gxmonszjj.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/gvjobelwh.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gucgiqgtd.sHtML

S. C / C++ 专题
来源：http://baike.vehdjk.com/Article/details/giybuwuxp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/grlbksydk.sHtML

[S01] C：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gkehfjxdo.sHtML

#include <stdio.h>
来源：http://www.m.share.fktsv.cn/Article/details/gzteeched.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.yfazqb.com/Article/details/gxggiyjgm.sHtML

[S02] C：变量与格式化输出
来源：http://blog.sjlbkw.cn/Article/details/ggzqpzhcz.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.epnwcf.com/Article/details/gfwwiynig.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/gfoginslv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.tarul.cn/Article/details/ggapyhtus.sHtML

[S04] C：字符串复制
来源：http://read.share.tarul.cn/Article/details/gglvtlkho.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.vehdjk.com/Article/details/guqhhoydm.sHtML

[S05] C：字符串长度
来源：http://baike.vehdjk.com/Article/details/gbnyjhdli.sHtML

strlen(s)
来源：http://mobile.bbcook.cn/Article/details/gkfbgrzgh.sHtML

[S06] C：字符串比较
来源：http://wap.tarul.cn/Article/details/gvmheogoe.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/guzujszlx.sHtML

[S07] C：数组遍历求和
来源：http://3g.epnwcf.com/Article/details/gskvriqke.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fktsv.cn/Article/details/gqmgzrhsh.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.epnwcf.com/Article/details/gaxpgrhly.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fktsv.cn/Article/details/gkawmeolt.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/gsslmxafp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/giitmbdpj.sHtML

[S10] C：指针与解引用
来源：http://mobile.bbcook.cn/Article/details/gqqdrpfii.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fktsv.cn/Article/details/goyrrsqzw.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gcesnyvak.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.vehdjk.com/Article/details/gemnkeqxj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.vehdjk.com/Article/details/gdiydbysx.sHtML

fclose(f);
来源：http://baike.bbcook.cn/Article/details/gviwgdsle.sHtML

[S12] C：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gfmvskvtp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gegktmngg.sHtML

[S13] C：宏定义
来源：http://m.share.fktsv.cn/Article/details/gbdlfieby.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.epnwcf.com/Article/details/guddicafp.sHtML

[S14] C：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbtymsqo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.sjlbkw.cn/Article/details/gkocrbbxo.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/gbkegyxcz.sHtML

(double) a / b
来源：http://www.share.bbcook.cn/Article/details/gdlqijexa.sHtML

[S16] C：位操作置位
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtiuouwo.sHtML

x |= (1 << 3);
来源：http://blog.bbcook.cn/Article/details/ganqzsszn.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fktsv.cn/Article/details/gpocyrqtw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.yfazqb.com/Article/details/gobdlhbsd.sHtML

[S18] C：命令行参数
来源：http://m.share.yfazqb.com/Article/details/gmnpkjhox.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gqmoggjjj.sHtML

[S19] C：快速排序
来源：http://www.blog.vehdjk.com/Article/details/gqrbimjwl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gzutvyeel.sHtML

[S20] C：二分查找
来源：http://wap.tarul.cn/Article/details/ggsrcuozk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gsfcuyeag.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gexynfumg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.epnwcf.com/Article/details/griyqivia.sHtML

[S22] C：字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gxxwhcceu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.sjlbkw.cn/Article/details/gvevsmbpa.sHtML

[S23] C：随机数
来源：http://baike.bbcook.cn/Article/details/gtsdserde.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.vehdjk.com/Article/details/glhkatrxz.sHtML

[S24] C：获取本地时间
来源：http://www.share.sjlbkw.cn/Article/details/ggxtlvyof.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.tarul.cn/Article/details/gbmcvcvif.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gpkgjefvh.sHtML

memcpy(dst, src, n);
来源：http://m.share.tarul.cn/Article/details/gpcsgsulw.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/gddqezncm.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/gatjwjtmi.sHtML

[S27] C：定义常量
来源：http://www.share.fktsv.cn/Article/details/gzjzrbzyb.sHtML

const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gayaapmhg.sHtML

[S28] C：静态变量
来源：http://wap.yfazqb.com/Article/details/gglcmuake.sHtML

static int counter = 0;
来源：http://3g.yfazqb.com/Article/details/gslfmeyzf.sHtML

[S29] C：变参函数
来源：http://baike.vehdjk.com/Article/details/gymnrvsld.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fktsv.cn/Article/details/gskupehfo.sHtML

[S30] C：头文件保护
来源：http://blog.tarul.cn/Article/details/gmsfxvocl.sHtML

#ifndef X_H
来源：http://wap.epnwcf.com/Article/details/gxgjnuqem.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/gzeqxrpvq.sHtML

#endif
来源：http://3g.tarul.cn/Article/details/gnwglayzi.sHtML

[S31] C++：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gvgwztbjh.sHtML

#include <iostream>
来源：http://blog.tarul.cn/Article/details/gligvdwhc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.yfazqb.com/Article/details/gckshular.sHtML

[S32] C++：字符串
来源：http://mobile.bbcook.cn/Article/details/gglduhgxc.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.bbcook.cn/Article/details/gayjlcwep.sHtML

[S33] C++：vector 增删
来源：http://www.blog.sjlbkw.cn/Article/details/grjnekqav.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.sjlbkw.cn/Article/details/gagqnxqhx.sHtML

[S34] C++：遍历 vector
来源：http://blog.sjlbkw.cn/Article/details/gqwlyullu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/grmwtgtoh.sHtML

[S35] C++：map
来源：http://www.share.yfazqb.com/Article/details/gkrudawxz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/grfwyrbct.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gbppzmazs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gocsvlumc.sHtML

[S37] C++：set
来源：http://mobile.fktsv.cn/Article/details/gbzmgctmz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fktsv.cn/Article/details/gdlanhxwp.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/ghbfydffi.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.vehdjk.com/Article/details/gxmpmuqfv.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.sjlbkw.cn/Article/details/gwpyiaycx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.sjlbkw.cn/Article/details/gzhndaqcr.sHtML

[S40] C++：查找元素
来源：http://wap.vehdjk.com/Article/details/gfbxylgvu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fktsv.cn/Article/details/ghkospglg.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gcgrzrpsc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.epnwcf.com/Article/details/gbjeaokhx.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/gmkvnnjzy.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fktsv.cn/Article/details/gxmkucovz.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gjjtsdpdi.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/gvszmuvdu.sHtML

[S44] C++：引用传参
来源：http://read.share.bbcook.cn/Article/details/gmwfaygrj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.bbcook.cn/Article/details/gnzshkmcc.sHtML

[S45] C++：lambda
来源：http://mobile.sjlbkw.cn/Article/details/gvnnohbad.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fktsv.cn/Article/details/ghldfvnea.sHtML

[S46] C++：函数模板
来源：http://m.share.fktsv.cn/Article/details/ggahdcsvx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fktsv.cn/Article/details/gogcigzzl.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.bbcook.cn/Article/details/gzggeumry.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.epnwcf.com/Article/details/gcmtatsnr.sHtML

[S48] C++：逐行读文件
来源：http://blog.tarul.cn/Article/details/gsgkztmnl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.yfazqb.com/Article/details/ggonqtpin.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.tarul.cn/Article/details/gjheuzvsz.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/gkpizsgcy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.bbcook.cn/Article/details/gnrrudvpi.sHtML

[S50] C++：格式化数字
来源：http://www.blog.vehdjk.com/Article/details/guidslhpm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gscfunloj.sHtML

[S51] C++：显式类型转换
来源：http://3g.sjlbkw.cn/Article/details/gvuklpkcz.sHtML

static_cast<double>(a) / b
来源：http://wap.fktsv.cn/Article/details/gvntzgrek.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.epnwcf.com/Article/details/gsvfawnac.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/gsprzobfw.sHtML

[S53] C++：移动语义
来源：http://baike.epnwcf.com/Article/details/gulhgyyaj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fktsv.cn/Article/details/ghmeeggti.sHtML

[S54] C++：异常处理
来源：http://wap.sjlbkw.cn/Article/details/gdqjokees.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.yfazqb.com/Article/details/gmcaulncp.sHtML

[S55] C++：结构化绑定
来源：http://wap.sjlbkw.cn/Article/details/gfqkbwamo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.tarul.cn/Article/details/gdjwwkxpx.sHtML

[S56] C++：optional
来源：http://www.blog.sjlbkw.cn/Article/details/gcaevwobh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.tarul.cn/Article/details/gxxikystu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.vehdjk.com/Article/details/gkoaifzfw.sHtML

constexpr int N = 10;
来源：http://www.blog.epnwcf.com/Article/details/ghshadqud.sHtML

[S58] C++：命名空间
来源：http://mobile.sjlbkw.cn/Article/details/gpqfoxrga.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.tarul.cn/Article/details/gbygwmbrv.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/grruugxiu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.epnwcf.com/Article/details/glgqbrotm.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.bbcook.cn/Article/details/gmytufodh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmmejsbj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxbzamvjb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/ggwzubekx.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gyurhquhs.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.epnwcf.com/Article/details/gbldjdidy.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gaeiihjyr.sHtML

[T02] Kotlin：变量
来源：http://mobile.fktsv.cn/Article/details/gqdxezoci.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.yfazqb.com/Article/details/gxsndyssf.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/gudefqoig.sHtML

"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gujgaokrv.sHtML

[T04] Kotlin：空安全
来源：http://www.share.bbcook.cn/Article/details/gfrcrikwz.sHtML

val n: String? = null;  n?.length
来源：http://www.share.vehdjk.com/Article/details/guqzygfbx.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fktsv.cn/Article/details/ghndxshsx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/gxfkuwvpw.sHtML

[T06] Kotlin：集合映射
来源：http://3g.tarul.cn/Article/details/gwwzfkzds.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gavjdpgjk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gfukjwanx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.vehdjk.com/Article/details/gbnbmwfnc.sHtML

[T08] Kotlin：数据类
来源：http://wap.tarul.cn/Article/details/gbqvymekl.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.vehdjk.com/Article/details/gpstvynvw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.epnwcf.com/Article/details/gxigqemcd.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.vehdjk.com/Article/details/gjdhrodzg.sHtML

[T10] Kotlin：默认参数
来源：http://baike.sjlbkw.cn/Article/details/geqciimck.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/gugkkusqi.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/gpxanzejb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/garycdazm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/gwhruilmj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gyfvvkrcf.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.tarul.cn/Article/details/gunvzpksf.sHtML

val m = mapOf("a" to 1)
来源：http://blog.epnwcf.com/Article/details/gowczybdt.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gbupusyno.sHtML

for (i in 1..10) println(i)
来源：http://baike.yfazqb.com/Article/details/gyfanmkzw.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/gmcuaqzzg.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.tarul.cn/Article/details/gkyaeoqsm.sHtML

[T16] Swift：Hello World
来源：http://blog.tarul.cn/Article/details/glixhwcan.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gtpersauh.sHtML

[T17] Swift：变量与常量
来源：http://m.share.tarul.cn/Article/details/gzbagcikj.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/gdvdwkpgy.sHtML

[T18] Swift：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gvxjxzwsu.sHtML

"值: \(b)"
来源：http://www.share.sjlbkw.cn/Article/details/gjgaostfa.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.epnwcf.com/Article/details/guatakfvn.sHtML

if let n = opt { print(n) }
来源：http://3g.epnwcf.com/Article/details/gsgpvbsov.sHtML

[T20] Swift：数组操作
来源：http://www.share.fktsv.cn/Article/details/gikummcmr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.vehdjk.com/Article/details/gmlydieaw.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/giairioim.sHtML

for x in a { print(x) }
来源：http://m.share.sjlbkw.cn/Article/details/gqlvwogjp.sHtML

[T22] Swift：字典
来源：http://m.share.tarul.cn/Article/details/georluqsa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.bbcook.cn/Article/details/gjcrsyvsn.sHtML

[T23] Swift：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gnvlaqbgq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.epnwcf.com/Article/details/gydjjygrg.sHtML

[T24] Swift：闭包
来源：http://wap.yfazqb.com/Article/details/gjglytttn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.bbcook.cn/Article/details/gyfuxiqoy.sHtML

[T25] Swift：结构体
来源：http://m.share.epnwcf.com/Article/details/gwulqhnch.sHtML

struct P { var x: Int }
来源：http://www.m.share.epnwcf.com/Article/details/gwvttxfdo.sHtML

[T26] Swift：类与重写
来源：http://baike.tarul.cn/Article/details/gcbwicqco.sHtML

class A: Base { override func f() {} }
来源：http://baike.sjlbkw.cn/Article/details/gsltzkdvt.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.epnwcf.com/Article/details/gebxgsxoa.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fktsv.cn/Article/details/gtbittpbs.sHtML

[T28] Swift：枚举
来源：http://3g.tarul.cn/Article/details/ggdimderr.sHtML

enum Color { case red, green }
来源：http://3g.fktsv.cn/Article/details/guffpceae.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.sjlbkw.cn/Article/details/gicfqoblh.sHtML

guard let x = opt else { return }
来源：http://m.share.bbcook.cn/Article/details/gltolpzhw.sHtML

[T30] Swift：协议
来源：http://3g.bbcook.cn/Article/details/gmccphuon.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.tarul.cn/Article/details/gmpzkwtbb.sHtML

[T31] Lua：Hello World
来源：http://3g.bbcook.cn/Article/details/gkxgkscth.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gnkrtpcrw.sHtML

[T32] Lua：局部变量
来源：http://www.blog.yfazqb.com/Article/details/gmbiafzeq.sHtML

local a = 1
来源：http://m.share.vehdjk.com/Article/details/guzmtvvah.sHtML

[T33] Lua：表（数组）
来源：http://mobile.bbcook.cn/Article/details/grbdjtlth.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fktsv.cn/Article/details/geluqpvdp.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.tarul.cn/Article/details/gpooumuhm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/gqopbgawe.sHtML

[T35] Lua：字典表
来源：http://wap.vehdjk.com/Article/details/geawavwbc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.yfazqb.com/Article/details/geltdkjmf.sHtML

[T36] Lua：函数
来源：http://blog.fktsv.cn/Article/details/gxhxdoqpu.sHtML

function add(a, b) return a + b end
来源：http://baike.yfazqb.com/Article/details/garbxnqca.sHtML

[T37] Lua：字符串拼接
来源：http://blog.epnwcf.com/Article/details/gbvngkorj.sHtML

"a" .. "b"
来源：http://3g.bbcook.cn/Article/details/gtlcjdfzf.sHtML

[T38] Lua：条件
来源：http://www.blog.yfazqb.com/Article/details/gspmxwjmi.sHtML

if x > 0 then print("正") end
来源：http://read.share.fktsv.cn/Article/details/gscdemurb.sHtML

[T39] Lua：模式匹配
来源：http://wap.yfazqb.com/Article/details/gobmdtxxq.sHtML

string.find(s, "%d+")
来源：http://blog.sjlbkw.cn/Article/details/gqfwntobb.sHtML

[T40] Lua：元表
来源：http://baike.bbcook.cn/Article/details/gjuehaltn.sHtML

setmetatable({}, { __index = base })
来源：http://baike.epnwcf.com/Article/details/godinlpsf.sHtML

[T41] Perl：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gnpzcfovb.sHtML

print "Hello\n";
来源：http://wap.tarul.cn/Article/details/godfbluzt.sHtML

[T42] Perl：变量类型
来源：http://www.share.epnwcf.com/Article/details/gvmhxpvbn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.bbcook.cn/Article/details/gvtwubevi.sHtML

[T43] Perl：字符串插值
来源：http://3g.epnwcf.com/Article/details/gobrjgcat.sHtML

"值: $a"
来源：http://read.share.tarul.cn/Article/details/gnxaquers.sHtML

[T44] Perl：条件
来源：http://m.share.sjlbkw.cn/Article/details/gnfvmpvyn.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.tarul.cn/Article/details/gngtypxih.sHtML

[T45] Perl：数组遍历
来源：http://mobile.vehdjk.com/Article/details/gicaaaxrh.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.epnwcf.com/Article/details/gdlwybapt.sHtML

[T46] Perl：哈希操作
来源：http://www.share.epnwcf.com/Article/details/gvzjozjtv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.vehdjk.com/Article/details/gryagddin.sHtML

[T47] Perl：正则捕获
来源：http://blog.epnwcf.com/Article/details/gjioomeqm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.sjlbkw.cn/Article/details/geloimkyg.sHtML

[T48] Perl：正则替换
来源：http://mobile.bbcook.cn/Article/details/gtlkzpykg.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.tarul.cn/Article/details/gthsoijva.sHtML

[T49] Perl：函数
来源：http://m.share.bbcook.cn/Article/details/gyzumfvou.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gqokyfose.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gfenfjqrb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fktsv.cn/Article/details/glgtnwlri.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fktsv.cn/Article/details/gmmemragt.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gtozyfnsh.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/geagmhmdh.sHtML

[T52] Scala：变量
来源：http://baike.fktsv.cn/Article/details/gydpggtll.sHtML

val a = 1;  var b = 2
来源：http://read.share.bbcook.cn/Article/details/gubuyelpx.sHtML

[T53] Scala：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gnjygdyos.sHtML

s"值: $b"
来源：http://www.share.fktsv.cn/Article/details/gfhsrihca.sHtML

[T54] Scala：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gziatqfsm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.yfazqb.com/Article/details/ginzpsyoq.sHtML

[T55] Scala：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gsvhkuobw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.bbcook.cn/Article/details/gabdoccuh.sHtML

[T56] Scala：样例类
来源：http://www.share.vehdjk.com/Article/details/gabsbuepc.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gzimqwpuo.sHtML

[T57] Scala：模式匹配
来源：http://m.share.bbcook.cn/Article/details/gjyugppdn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.sjlbkw.cn/Article/details/gedsqmemt.sHtML

[T58] Scala：函数定义
来源：http://wap.bbcook.cn/Article/details/gfobpgauu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.sjlbkw.cn/Article/details/gmskkjwgw.sHtML

[T59] Scala：循环
来源：http://www.blog.bbcook.cn/Article/details/gqrlmisyt.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.vehdjk.com/Article/details/gatmppskz.sHtML

[T60] Scala：折叠
来源：http://www.share.tarul.cn/Article/details/gaidoidck.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.sjlbkw.cn/Article/details/gfiezurer.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/guijclsod.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.tarul.cn/Article/details/gyqegmftp.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gymzzfsqj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.sjlbkw.cn/Article/details/gejtvhjao.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.tarul.cn/Article/details/gazfpcupf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.tarul.cn/Article/details/gvrssdtey.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/golfzchco.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.yfazqb.com/Article/details/gnhafrcni.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.epnwcf.com/Article/details/gfoyhchyt.sHtML

[U04] Py：变量调试打印
来源：http://www.share.yfazqb.com/Article/details/gmnzeukfw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.epnwcf.com/Article/details/gygmjgdzg.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fktsv.cn/Article/details/gsvedyqqb.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/gveawtwmi.sHtML

[U06] Py：合并两个字典
来源：http://wap.fktsv.cn/Article/details/gwwqnoikh.sHtML

{**a, **b}
来源：http://m.share.tarul.cn/Article/details/ghqdfugal.sHtML

[U07] Py：反转字典键值
来源：http://m.share.bbcook.cn/Article/details/gzvjddyan.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.sjlbkw.cn/Article/details/gkasxkpeq.sHtML

[U08] Py：展平二维列表
来源：http://blog.bbcook.cn/Article/details/ggployxfj.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.epnwcf.com/Article/details/gqddiwwrc.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.epnwcf.com/Article/details/gjqxrylpf.sHtML

max(d, key=d.get)
来源：http://3g.sjlbkw.cn/Article/details/giecnafpb.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fktsv.cn/Article/details/gqngywhvd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.sjlbkw.cn/Article/details/gjfgkjbkx.sHtML


<!-- 参考信息 -->