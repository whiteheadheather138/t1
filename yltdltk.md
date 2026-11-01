代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/getegicxa.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gvpmflvxt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.vehdjk.com/Article/details/gaaxnjjgy.sHtML

[R77] 读取用户输入
来源：http://wap.sjlbkw.cn/Article/details/gwsenyncy.sHtML

read -rp "请输入: " ans
来源：http://blog.sjlbkw.cn/Article/details/gyeqiponc.sHtML

[R78] 交互式菜单
来源：http://3g.yfazqb.com/Article/details/gofcebsxy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.yfazqb.com/Article/details/gdnvvcipf.sHtML

[R79] 解析命令行选项
来源：http://mobile.yfazqb.com/Article/details/gmjzmqdpb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.yfazqb.com/Article/details/gndmsdusb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.vehdjk.com/Article/details/gwtymcijk.sHtML

time ./run.sh
来源：http://www.blog.fktsv.cn/Article/details/ggnjbkmtc.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gewwgvikn.sHtML

S. C / C++ 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgnnwpwv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gohyykxlc.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gerhypnro.sHtML

#include <stdio.h>
来源：http://www.share.yfazqb.com/Article/details/gtsywzfzw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.bbcook.cn/Article/details/gvdqmvezq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.tarul.cn/Article/details/ghjxlwskw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.yfazqb.com/Article/details/gfwqrgdnv.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/gamvoegee.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/gwhfggfdf.sHtML

[S04] C：字符串复制
来源：http://read.share.epnwcf.com/Article/details/gfvblcgjy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.bbcook.cn/Article/details/gfohmuesh.sHtML

[S05] C：字符串长度
来源：http://www.share.fktsv.cn/Article/details/gxiabvcfr.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/gxnobarax.sHtML

[S06] C：字符串比较
来源：http://read.share.tarul.cn/Article/details/grpeldrwx.sHtML

strcmp(a, b) == 0
来源：http://3g.bbcook.cn/Article/details/gupucjiaf.sHtML

[S07] C：数组遍历求和
来源：http://read.share.epnwcf.com/Article/details/gypvlghgo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.yfazqb.com/Article/details/gkmugwefe.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.bbcook.cn/Article/details/gbdkxdddo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.yfazqb.com/Article/details/grstdesmz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/ggymkpkzi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.yfazqb.com/Article/details/gfazxrsbc.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.tarul.cn/Article/details/gyudjrfuc.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/gedymhnze.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/ggilpdlvt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fktsv.cn/Article/details/gwvzvjjjs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/gtvlcojeq.sHtML

fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/gogorwgvi.sHtML

[S12] C：写文件
来源：http://www.share.vehdjk.com/Article/details/gvktlbxbv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/giulzpspe.sHtML

[S13] C：宏定义
来源：http://baike.sjlbkw.cn/Article/details/gmdrguehe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.epnwcf.com/Article/details/gcnaxuxkq.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/glzubbqsu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.tarul.cn/Article/details/govrkyudz.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/gqsaoivss.sHtML

(double) a / b
来源：http://m.share.tarul.cn/Article/details/gzhbtnobk.sHtML

[S16] C：位操作置位
来源：http://www.blog.yfazqb.com/Article/details/gyxljwblv.sHtML

x |= (1 << 3);
来源：http://3g.vehdjk.com/Article/details/gwtlaymrh.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fktsv.cn/Article/details/goifizywu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fktsv.cn/Article/details/gksqrqtal.sHtML

[S18] C：命令行参数
来源：http://3g.vehdjk.com/Article/details/gtpidwjcy.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fktsv.cn/Article/details/gxhxfdglo.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/gdnnqghis.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gfxozfywi.sHtML

[S20] C：二分查找
来源：http://baike.fktsv.cn/Article/details/grnquxguw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gcsjasfpg.sHtML

[S21] C：字符类别判断
来源：http://www.blog.sjlbkw.cn/Article/details/gxpkvoqms.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/gutdlvrjz.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.bbcook.cn/Article/details/gshidsrka.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/geegaunhq.sHtML

[S23] C：随机数
来源：http://read.share.yfazqb.com/Article/details/gvijgjjdr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fktsv.cn/Article/details/gzgnwyabu.sHtML

[S24] C：获取本地时间
来源：http://m.share.yfazqb.com/Article/details/gquonsbds.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.vehdjk.com/Article/details/gwkfpemcz.sHtML

[S25] C：内存拷贝
来源：http://wap.tarul.cn/Article/details/gavgnvwel.sHtML

memcpy(dst, src, n);
来源：http://www.share.sjlbkw.cn/Article/details/gjwreedrj.sHtML

[S26] C：内存清零
来源：http://www.share.vehdjk.com/Article/details/gvpcuxhwd.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fktsv.cn/Article/details/gbgnrigrz.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/gcdtyygyi.sHtML

const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gbbgdfwed.sHtML

[S28] C：静态变量
来源：http://mobile.sjlbkw.cn/Article/details/gnspnvqgd.sHtML

static int counter = 0;
来源：http://blog.yfazqb.com/Article/details/gjbocidpe.sHtML

[S29] C：变参函数
来源：http://m.share.bbcook.cn/Article/details/gshvthbve.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.sjlbkw.cn/Article/details/gmtuqqysi.sHtML

[S30] C：头文件保护
来源：http://www.m.share.yfazqb.com/Article/details/gksdulkrr.sHtML

#ifndef X_H
来源：http://mobile.fktsv.cn/Article/details/grzvrdrug.sHtML

#define X_H
来源：http://www.blog.yfazqb.com/Article/details/glklcsosk.sHtML

#endif
来源：http://www.m.share.tarul.cn/Article/details/gcsyuddem.sHtML

[S31] C++：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gheinomkg.sHtML

#include <iostream>
来源：http://3g.fktsv.cn/Article/details/gzrmkyqkc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/gjoniljzd.sHtML

[S32] C++：字符串
来源：http://read.share.yfazqb.com/Article/details/gnroshsnu.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fktsv.cn/Article/details/gawabggav.sHtML

[S33] C++：vector 增删
来源：http://m.share.epnwcf.com/Article/details/gpoxceain.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.vehdjk.com/Article/details/gpgseufyd.sHtML

[S34] C++：遍历 vector
来源：http://m.share.vehdjk.com/Article/details/ggqsjobrb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fktsv.cn/Article/details/gyhwkvuob.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/gprcwauvo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gkodjmbko.sHtML

[S36] C++：unordered_map
来源：http://baike.epnwcf.com/Article/details/gdizmkylb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/grumhegss.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/ghlquvmxe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/gtcfcynji.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/gkxxkkvqa.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/geeyqeyno.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.sjlbkw.cn/Article/details/gixnaisvi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.epnwcf.com/Article/details/greitpibi.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/gggnbrmwq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.tarul.cn/Article/details/gtvztxibu.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gzoflrzvc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/gbtcxrhqg.sHtML

[S42] C++：继承与虚函数
来源：http://3g.tarul.cn/Article/details/gnsoatrag.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.bbcook.cn/Article/details/ggwpuhwqy.sHtML

[S43] C++：智能指针
来源：http://www.m.share.tarul.cn/Article/details/ghmnzvihs.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/gduhvhbwl.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/gwlrepdzx.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/gljackhtl.sHtML

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/gaqmfkhnd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.bbcook.cn/Article/details/gvnbksonh.sHtML

[S46] C++：函数模板
来源：http://read.share.fktsv.cn/Article/details/gcrrtahzs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fktsv.cn/Article/details/gvhoflzyb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.bbcook.cn/Article/details/gdzmopivj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fktsv.cn/Article/details/gealukfhn.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/grikjgakj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.epnwcf.com/Article/details/gsodvpzbb.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/gayrlxmpp.sHtML

[S49] C++：写文件
来源：http://baike.tarul.cn/Article/details/gpqdphsna.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.tarul.cn/Article/details/gnjdmnkrm.sHtML

[S50] C++：格式化数字
来源：http://read.share.bbcook.cn/Article/details/grqehpniu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gfrzcozkd.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/girojfkvo.sHtML

static_cast<double>(a) / b
来源：http://baike.tarul.cn/Article/details/gtksjmbgo.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.sjlbkw.cn/Article/details/gavohyvwb.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.vehdjk.com/Article/details/gvynzhpsl.sHtML

[S53] C++：移动语义
来源：http://read.share.bbcook.cn/Article/details/gkiyvipdz.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.bbcook.cn/Article/details/gkbsvqmmc.sHtML

[S54] C++：异常处理
来源：http://blog.epnwcf.com/Article/details/gjqkoiepe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.bbcook.cn/Article/details/guwbnczgr.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.epnwcf.com/Article/details/gyqodyaca.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/gxhfgrjhb.sHtML

[S56] C++：optional
来源：http://mobile.epnwcf.com/Article/details/gncpeawnh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.epnwcf.com/Article/details/glyrjugrq.sHtML

[S57] C++：编译期常量
来源：http://wap.bbcook.cn/Article/details/gkngsequu.sHtML

constexpr int N = 10;
来源：http://3g.fktsv.cn/Article/details/gcrgbbgfo.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/gjccxbpdq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fktsv.cn/Article/details/gdzzjvkrp.sHtML

[S59] C++：静态断言
来源：http://baike.tarul.cn/Article/details/ggkdoqzrk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.yfazqb.com/Article/details/grienyaon.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.bbcook.cn/Article/details/gctpxdlmu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/glggcnywe.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxbyeywqd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/ganhynmmk.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/grdxhoicz.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/gvqskhtdj.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/gpjrqwetu.sHtML

[T02] Kotlin：变量
来源：http://m.share.bbcook.cn/Article/details/ggwzscdaa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/gvrjogsxn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.vehdjk.com/Article/details/gbkzygkyd.sHtML

"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/grgzmafft.sHtML

[T04] Kotlin：空安全
来源：http://3g.sjlbkw.cn/Article/details/gvpxtraee.sHtML

val n: String? = null;  n?.length
来源：http://baike.epnwcf.com/Article/details/gjijofriw.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.epnwcf.com/Article/details/gqccbmcyq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.epnwcf.com/Article/details/glsdtatlg.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.tarul.cn/Article/details/gxaupheeh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/gpiwhdmvs.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gypquzkzx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.tarul.cn/Article/details/gkqrmfrmj.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.bbcook.cn/Article/details/gojbdsegw.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.sjlbkw.cn/Article/details/gsuftlwbb.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.sjlbkw.cn/Article/details/gkyvjbcix.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.bbcook.cn/Article/details/gsaptlirs.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fktsv.cn/Article/details/gihbflexr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.epnwcf.com/Article/details/genfiyixf.sHtML

[T11] Kotlin：协程
来源：http://mobile.vehdjk.com/Article/details/gieqkpeml.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.yfazqb.com/Article/details/gajnvakgi.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.vehdjk.com/Article/details/gwexwhmvz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.yfazqb.com/Article/details/goxtudxqt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.tarul.cn/Article/details/gymbksdse.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.bbcook.cn/Article/details/gljlatsjw.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gtwgjjbkc.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gssskcawm.sHtML

[T15] Kotlin：接口
来源：http://www.share.vehdjk.com/Article/details/glxfvczps.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gpppfyagp.sHtML

[T16] Swift：Hello World
来源：http://m.share.vehdjk.com/Article/details/gaodtphkj.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gnttourpp.sHtML

[T17] Swift：变量与常量
来源：http://m.share.vehdjk.com/Article/details/gxbtfldex.sHtML

var a = 1;  let b = 2
来源：http://blog.sjlbkw.cn/Article/details/gvnfdwcms.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fktsv.cn/Article/details/goeuczxug.sHtML

"值: \(b)"
来源：http://www.share.epnwcf.com/Article/details/gosabfodq.sHtML

[T19] Swift：可选绑定
来源：http://wap.tarul.cn/Article/details/gbujqhldu.sHtML

if let n = opt { print(n) }
来源：http://www.blog.yfazqb.com/Article/details/ghmkqsogw.sHtML

[T20] Swift：数组操作
来源：http://www.blog.yfazqb.com/Article/details/gjfufpbzf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.bbcook.cn/Article/details/gtjujneno.sHtML

[T21] Swift：遍历
来源：http://blog.tarul.cn/Article/details/gbhmpleoh.sHtML

for x in a { print(x) }
来源：http://read.share.sjlbkw.cn/Article/details/gxchrknwy.sHtML

[T22] Swift：字典
来源：http://mobile.tarul.cn/Article/details/gkomiwobi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.epnwcf.com/Article/details/gegbjfpyq.sHtML

[T23] Swift：函数
来源：http://www.blog.tarul.cn/Article/details/gnorsdfrm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gudxeffrn.sHtML

[T24] Swift：闭包
来源：http://3g.bbcook.cn/Article/details/giyxqirxn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.tarul.cn/Article/details/gcvjlxxxy.sHtML

[T25] Swift：结构体
来源：http://mobile.sjlbkw.cn/Article/details/gwvifhbki.sHtML

struct P { var x: Int }
来源：http://read.share.epnwcf.com/Article/details/gsysdwmpk.sHtML

[T26] Swift：类与重写
来源：http://m.share.epnwcf.com/Article/details/gissbpjmq.sHtML

class A: Base { override func f() {} }
来源：http://wap.fktsv.cn/Article/details/gbzwwjwsy.sHtML

[T27] Swift：错误处理
来源：http://3g.tarul.cn/Article/details/gnvxaptsi.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.vehdjk.com/Article/details/gnanukwfm.sHtML

[T28] Swift：枚举
来源：http://3g.vehdjk.com/Article/details/goxzwdpuk.sHtML

enum Color { case red, green }
来源：http://mobile.fktsv.cn/Article/details/gakuxscdb.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.vehdjk.com/Article/details/gxcrfyxcw.sHtML

guard let x = opt else { return }
来源：http://read.share.yfazqb.com/Article/details/gyzmimwcz.sHtML

[T30] Swift：协议
来源：http://read.share.sjlbkw.cn/Article/details/goygogxbn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.tarul.cn/Article/details/gpdrpcmmy.sHtML

[T31] Lua：Hello World
来源：http://blog.fktsv.cn/Article/details/gngthgmmh.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gclfnbjbx.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.tarul.cn/Article/details/gfngiwyfq.sHtML

local a = 1
来源：http://3g.epnwcf.com/Article/details/gdpxdrdux.sHtML

[T33] Lua：表（数组）
来源：http://mobile.yfazqb.com/Article/details/gwqeyqsxp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fktsv.cn/Article/details/gekxpfsay.sHtML

[T34] Lua：遍历表
来源：http://read.share.bbcook.cn/Article/details/gxlzslruo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.yfazqb.com/Article/details/gnkociadx.sHtML

[T35] Lua：字典表
来源：http://www.blog.tarul.cn/Article/details/gkdnddisf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.epnwcf.com/Article/details/gxuwvrqcj.sHtML

[T36] Lua：函数
来源：http://www.share.epnwcf.com/Article/details/gapaifxsj.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fktsv.cn/Article/details/gswaoxaqb.sHtML

[T37] Lua：字符串拼接
来源：http://baike.yfazqb.com/Article/details/ghvcerihf.sHtML

"a" .. "b"
来源：http://www.share.bbcook.cn/Article/details/giqakhcvu.sHtML

[T38] Lua：条件
来源：http://baike.vehdjk.com/Article/details/gphtudrps.sHtML

if x > 0 then print("正") end
来源：http://www.blog.bbcook.cn/Article/details/gvzqbucpg.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/grwntmuzo.sHtML

string.find(s, "%d+")
来源：http://www.m.share.epnwcf.com/Article/details/gydphsevq.sHtML

[T40] Lua：元表
来源：http://m.share.bbcook.cn/Article/details/geqwwojls.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.bbcook.cn/Article/details/gefiitelm.sHtML

[T41] Perl：Hello World
来源：http://m.share.vehdjk.com/Article/details/gqfcxbvbx.sHtML

print "Hello\n";
来源：http://wap.tarul.cn/Article/details/gwdvfhwta.sHtML

[T42] Perl：变量类型
来源：http://www.share.fktsv.cn/Article/details/gkxzvompu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.yfazqb.com/Article/details/gblyyfojh.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.tarul.cn/Article/details/grwezorlc.sHtML

"值: $a"
来源：http://mobile.tarul.cn/Article/details/gcuadoupn.sHtML

[T44] Perl：条件
来源：http://baike.epnwcf.com/Article/details/gvqxfupzt.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.yfazqb.com/Article/details/gkfyjgybu.sHtML

[T45] Perl：数组遍历
来源：http://mobile.epnwcf.com/Article/details/gmrfpussz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.yfazqb.com/Article/details/golhtixfg.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fktsv.cn/Article/details/gepxjqejs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.epnwcf.com/Article/details/ghhfwzkxf.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.vehdjk.com/Article/details/gbwlqlqje.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.tarul.cn/Article/details/gpnpxqnyn.sHtML

[T48] Perl：正则替换
来源：http://read.share.tarul.cn/Article/details/gwplgtish.sHtML

$s =~ s/old/new/g;
来源：http://wap.tarul.cn/Article/details/gcrhclgry.sHtML

[T49] Perl：函数
来源：http://3g.bbcook.cn/Article/details/gskyrnkuz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gqvqooiwy.sHtML

[T50] Perl：逐行读文件
来源：http://baike.epnwcf.com/Article/details/ggocxadsk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fktsv.cn/Article/details/gxfwqiwaf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.yfazqb.com/Article/details/glmysfdxd.sHtML

[T51] Scala：Hello World
来源：http://m.share.tarul.cn/Article/details/gqgxvzjbx.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gzgwudycb.sHtML

[T52] Scala：变量
来源：http://www.share.yfazqb.com/Article/details/gbsdkshvh.sHtML

val a = 1;  var b = 2
来源：http://baike.epnwcf.com/Article/details/glqplvevl.sHtML

[T53] Scala：字符串插值
来源：http://wap.fktsv.cn/Article/details/gauwrjggi.sHtML

s"值: $b"
来源：http://baike.vehdjk.com/Article/details/gemvtilvm.sHtML

[T54] Scala：集合映射
来源：http://m.share.tarul.cn/Article/details/glvkyfmvg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fktsv.cn/Article/details/gnvoexmdu.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gubfmjpcq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fktsv.cn/Article/details/gljoodmpu.sHtML

[T56] Scala：样例类
来源：http://m.share.sjlbkw.cn/Article/details/gygzodutc.sHtML

case class User(name: String, age: Int)
来源：http://m.share.tarul.cn/Article/details/gfzaclmsz.sHtML

[T57] Scala：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/gedvikfzo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.vehdjk.com/Article/details/gippqwfzb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.bbcook.cn/Article/details/grjurcyav.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.bbcook.cn/Article/details/goxyedshs.sHtML

[T59] Scala：循环
来源：http://www.share.epnwcf.com/Article/details/gzpsxjssq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzvzemvb.sHtML

[T60] Scala：折叠
来源：http://mobile.epnwcf.com/Article/details/gmrvuchkz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/gsejbxwwh.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxvipjrgp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/gdqgrnyiw.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjzsxuycx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.epnwcf.com/Article/details/gwftyczrd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fktsv.cn/Article/details/gdsfvayqo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.sjlbkw.cn/Article/details/gzxqzuoat.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.tarul.cn/Article/details/gnffdwzjo.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fktsv.cn/Article/details/gftmavypg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fktsv.cn/Article/details/gxtrqpjlj.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.sjlbkw.cn/Article/details/gkwryftkg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.yfazqb.com/Article/details/glpgnqsbr.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.bbcook.cn/Article/details/gtptoxwlu.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/gjpjzdxuh.sHtML

[U06] Py：合并两个字典
来源：http://baike.tarul.cn/Article/details/gxcomcrrm.sHtML

{**a, **b}
来源：http://3g.fktsv.cn/Article/details/gayqdyrni.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.yfazqb.com/Article/details/gnkqxeupm.sHtML

{v: k for k, v in d.items()}
来源：http://baike.bbcook.cn/Article/details/gcaqbkryl.sHtML

[U08] Py：展平二维列表
来源：http://mobile.sjlbkw.cn/Article/details/gmtgdzfsk.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.yfazqb.com/Article/details/gtvtabzoo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.tarul.cn/Article/details/gzbgdstmr.sHtML

max(d, key=d.get)
来源：http://read.share.sjlbkw.cn/Article/details/gxflwgnqz.sHtML

[U10] Py：按值排序字典
来源：http://3g.bbcook.cn/Article/details/gunbrnhov.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fktsv.cn/Article/details/graoahqst.sHtML

[U11] Py：生成器表达式
来源：http://baike.vehdjk.com/Article/details/gdnajqgqa.sHtML

(x * 2 for x in arr)
来源：http://3g.sjlbkw.cn/Article/details/gmcrtovru.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.vehdjk.com/Article/details/gffxojmie.sHtML

Counter(arr).most_common(3)
来源：http://blog.epnwcf.com/Article/details/gcwylzgon.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fktsv.cn/Article/details/gwonumdvz.sHtML

deque(maxlen=10)
来源：http://blog.bbcook.cn/Article/details/gyxeecard.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/ghnvzdwtx.sHtML

defaultdict(list)
来源：http://www.blog.epnwcf.com/Article/details/grgwcpuol.sHtML

[U15] Py：高精度计时
来源：http://www.blog.sjlbkw.cn/Article/details/gtmftmcab.sHtML

t = time.perf_counter()
来源：http://www.share.sjlbkw.cn/Article/details/gwsbdanct.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fktsv.cn/Article/details/gknvctlyn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.vehdjk.com/Article/details/gfflksczq.sHtML


<!-- 参考信息 -->