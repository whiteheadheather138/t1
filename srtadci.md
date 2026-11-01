代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://mobile.bbcook.cn/Article/details/gnsnciyay.sHtML

[R70] 时间戳与互转
来源：http://baike.sjlbkw.cn/Article/details/gldaxjjez.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.sjlbkw.cn/Article/details/glcxeftsv.sHtML

[R71] 日期格式化
来源：http://wap.fktsv.cn/Article/details/gfkppdqoq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.sjlbkw.cn/Article/details/gkmcbirsh.sHtML

[R72] 等待端口就绪
来源：http://blog.vehdjk.com/Article/details/gbxbjqbuu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gffbmktbz.sHtML

[R73] 分割大日志
来源：http://3g.bbcook.cn/Article/details/gribkbhze.sHtML

split -l 1000 big.log part_
来源：http://wap.yfazqb.com/Article/details/gxuuxloiz.sHtML

[R74] 批量重命名
来源：http://blog.bbcook.cn/Article/details/gwrfhuebg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.bbcook.cn/Article/details/gigryvqme.sHtML

[R75] 导出环境变量
来源：http://mobile.vehdjk.com/Article/details/gjouwalow.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fktsv.cn/Article/details/gahunalih.sHtML

[R76] 使用临时文件
来源：http://www.share.bbcook.cn/Article/details/ggskgszrk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gkrbquqfc.sHtML

[R77] 读取用户输入
来源：http://baike.bbcook.cn/Article/details/geggwkdzu.sHtML

read -rp "请输入: " ans
来源：http://www.blog.sjlbkw.cn/Article/details/gqhjopldb.sHtML

[R78] 交互式菜单
来源：http://www.blog.sjlbkw.cn/Article/details/gnwcfjgie.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.tarul.cn/Article/details/gecaqfhzi.sHtML

[R79] 解析命令行选项
来源：http://3g.sjlbkw.cn/Article/details/gxhhxocow.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.epnwcf.com/Article/details/gqlzhwbvl.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.yfazqb.com/Article/details/gusoevzoi.sHtML

time ./run.sh
来源：http://www.share.vehdjk.com/Article/details/gqzfoevwe.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjvuoudzo.sHtML

S. C / C++ 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gpashfpwt.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gnhhakjxl.sHtML

[S01] C：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/geajfokuo.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/gjwgbsxpz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.vehdjk.com/Article/details/gcvffmknz.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.vehdjk.com/Article/details/gyiyppmla.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.sjlbkw.cn/Article/details/gromzasux.sHtML

[S03] C：读入整数
来源：http://m.share.epnwcf.com/Article/details/gjcmvmlbv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.tarul.cn/Article/details/gxpuhfbri.sHtML

[S04] C：字符串复制
来源：http://mobile.fktsv.cn/Article/details/glprumdyk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/givojpoxd.sHtML

[S05] C：字符串长度
来源：http://wap.tarul.cn/Article/details/gspauvaog.sHtML

strlen(s)
来源：http://www.blog.fktsv.cn/Article/details/gzjthnfoq.sHtML

[S06] C：字符串比较
来源：http://www.share.tarul.cn/Article/details/gcbedefte.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/gwmxjoewi.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/gqqsyxmvb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.epnwcf.com/Article/details/glyrfyuun.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fktsv.cn/Article/details/gbjuplgwj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fktsv.cn/Article/details/gvpvfhjuc.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.epnwcf.com/Article/details/guhjsmylp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fktsv.cn/Article/details/gczxjyqja.sHtML

[S10] C：指针与解引用
来源：http://baike.yfazqb.com/Article/details/gywezwtfj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gqieikwrh.sHtML

[S11] C：逐行读文件
来源：http://wap.tarul.cn/Article/details/gwdylblmh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.yfazqb.com/Article/details/gpockhpkg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gurbquxcl.sHtML

fclose(f);
来源：http://wap.tarul.cn/Article/details/gmqdpojwe.sHtML

[S12] C：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gipvummeb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gczkzxvcd.sHtML

[S13] C：宏定义
来源：http://m.share.yfazqb.com/Article/details/gzydwzvhf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.tarul.cn/Article/details/gehzunuaq.sHtML

[S14] C：枚举
来源：http://www.share.vehdjk.com/Article/details/gjjpugpxx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.vehdjk.com/Article/details/gpvddosev.sHtML

[S15] C：类型转换
来源：http://m.share.bbcook.cn/Article/details/gzcrytuvp.sHtML

(double) a / b
来源：http://3g.epnwcf.com/Article/details/gfjrfsoda.sHtML

[S16] C：位操作置位
来源：http://3g.vehdjk.com/Article/details/gqoecqlua.sHtML

x |= (1 << 3);
来源：http://baike.tarul.cn/Article/details/gnbzbkovh.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gnjclhdez.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.sjlbkw.cn/Article/details/gpkvjyzkg.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/giagfnekf.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/gpcoizljf.sHtML

[S19] C：快速排序
来源：http://baike.tarul.cn/Article/details/gloslcpva.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gdkudfsoq.sHtML

[S20] C：二分查找
来源：http://www.blog.sjlbkw.cn/Article/details/gkdfqksli.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/gpkkypxhv.sHtML

[S21] C：字符类别判断
来源：http://m.share.epnwcf.com/Article/details/guudljtab.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/gsiczdnxm.sHtML

[S22] C：字符串转数字
来源：http://3g.vehdjk.com/Article/details/gtsdpxnbw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.yfazqb.com/Article/details/gtgtlrglq.sHtML

[S23] C：随机数
来源：http://mobile.yfazqb.com/Article/details/gbqhvsreh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.vehdjk.com/Article/details/gnqweyacx.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.epnwcf.com/Article/details/gphojxjwi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/gsyjobxcv.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gzjagfvss.sHtML

memcpy(dst, src, n);
来源：http://mobile.bbcook.cn/Article/details/goluuvaqm.sHtML

[S26] C：内存清零
来源：http://read.share.yfazqb.com/Article/details/gtlcfjusc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/gvbkbbkhv.sHtML

[S27] C：定义常量
来源：http://baike.yfazqb.com/Article/details/gzemmcykh.sHtML

const double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gsbfnmkdp.sHtML

[S28] C：静态变量
来源：http://blog.sjlbkw.cn/Article/details/gsmkbclbd.sHtML

static int counter = 0;
来源：http://blog.tarul.cn/Article/details/grudljtiz.sHtML

[S29] C：变参函数
来源：http://3g.vehdjk.com/Article/details/gzfkfodgt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/gaqeosikh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.tarul.cn/Article/details/gwmqkuxvk.sHtML

#ifndef X_H
来源：http://mobile.sjlbkw.cn/Article/details/gcbmkflpd.sHtML

#define X_H
来源：http://www.m.share.epnwcf.com/Article/details/gvthypsab.sHtML

#endif
来源：http://mobile.fktsv.cn/Article/details/gbylsfxgo.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/geqntobpe.sHtML

#include <iostream>
来源：http://mobile.sjlbkw.cn/Article/details/gynjvxkqv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.vehdjk.com/Article/details/gebtnswvj.sHtML

[S32] C++：字符串
来源：http://blog.fktsv.cn/Article/details/gxgwxytjk.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.sjlbkw.cn/Article/details/gofixomjv.sHtML

[S33] C++：vector 增删
来源：http://mobile.bbcook.cn/Article/details/gwllcfjjm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fktsv.cn/Article/details/gpdahcylr.sHtML

[S34] C++：遍历 vector
来源：http://wap.yfazqb.com/Article/details/gyjpmhrgd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.bbcook.cn/Article/details/ggnwangof.sHtML

[S35] C++：map
来源：http://mobile.fktsv.cn/Article/details/gbdxvggbu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gduzeuhiq.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/gfzlvbqww.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gaqfrgoyp.sHtML

[S37] C++：set
来源：http://m.share.tarul.cn/Article/details/gmpjdeyfu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fktsv.cn/Article/details/gbyzwihxi.sHtML

[S38] C++：排序
来源：http://blog.vehdjk.com/Article/details/givllzwah.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.tarul.cn/Article/details/gppeqjlac.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.yfazqb.com/Article/details/grqzpjipt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/gzdtagfhc.sHtML

[S40] C++：查找元素
来源：http://wap.fktsv.cn/Article/details/gqarjcevd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fktsv.cn/Article/details/gnxembftu.sHtML

[S41] C++：类与构造函数
来源：http://www.share.epnwcf.com/Article/details/gduioveiq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.epnwcf.com/Article/details/gzrsdvgqm.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/glctoixhe.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.sjlbkw.cn/Article/details/gtjezzajd.sHtML

[S43] C++：智能指针
来源：http://www.m.share.vehdjk.com/Article/details/gblkdlygl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.vehdjk.com/Article/details/gakgzdmzd.sHtML

[S44] C++：引用传参
来源：http://wap.epnwcf.com/Article/details/gtkxqqikb.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.tarul.cn/Article/details/goprgyuiy.sHtML

[S45] C++：lambda
来源：http://baike.vehdjk.com/Article/details/gqrfssnvv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.epnwcf.com/Article/details/gtqvonlnq.sHtML

[S46] C++：函数模板
来源：http://baike.epnwcf.com/Article/details/gzrurctzu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.bbcook.cn/Article/details/gpuyjhkhv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.bbcook.cn/Article/details/ggzuevzjh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fktsv.cn/Article/details/gajsnnjtc.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gzfnjqvde.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.vehdjk.com/Article/details/gdzngzavn.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.yfazqb.com/Article/details/gjisrzwnr.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/gduxrthyq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.epnwcf.com/Article/details/gtcrdybod.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gldyiwefk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.epnwcf.com/Article/details/ghbebrixh.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/ggibjlwps.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fktsv.cn/Article/details/gvgkxxxiq.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.sjlbkw.cn/Article/details/gglnwlgcq.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/guqtctvkp.sHtML

[S53] C++：移动语义
来源：http://wap.tarul.cn/Article/details/gwducqued.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.vehdjk.com/Article/details/gejegvbic.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/goermhbju.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/gswgbubgq.sHtML

[S55] C++：结构化绑定
来源：http://www.share.epnwcf.com/Article/details/gwsjdcmon.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.bbcook.cn/Article/details/gdckcdjbd.sHtML

[S56] C++：optional
来源：http://mobile.epnwcf.com/Article/details/ggniwhgam.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/gbmvfxepk.sHtML

[S57] C++：编译期常量
来源：http://wap.yfazqb.com/Article/details/gddubrfyp.sHtML

constexpr int N = 10;
来源：http://baike.tarul.cn/Article/details/gudwoiggv.sHtML

[S58] C++：命名空间
来源：http://baike.epnwcf.com/Article/details/glgwbadxb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.yfazqb.com/Article/details/geqgdrhbn.sHtML

[S59] C++：静态断言
来源：http://www.share.bbcook.cn/Article/details/gzljygdxp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fktsv.cn/Article/details/gjrthogal.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.vehdjk.com/Article/details/gckidslfh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.epnwcf.com/Article/details/gzyyvtjqp.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/geowjczct.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gxpruzfyo.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gxnftdqqo.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.tarul.cn/Article/details/gavuuogwa.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/ghfssivzr.sHtML

[T02] Kotlin：变量
来源：http://baike.tarul.cn/Article/details/gdegjkbbn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fktsv.cn/Article/details/gbjavovlb.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.tarul.cn/Article/details/gjdtvlfwt.sHtML

"值: $b"
来源：http://3g.fktsv.cn/Article/details/gldjzdtys.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.yfazqb.com/Article/details/ggpheopev.sHtML

val n: String? = null;  n?.length
来源：http://3g.fktsv.cn/Article/details/ganmieuke.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.bbcook.cn/Article/details/gevqrjfzv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fktsv.cn/Article/details/ggukdlqzp.sHtML

[T06] Kotlin：集合映射
来源：http://wap.epnwcf.com/Article/details/gqmjcimti.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gnknaichk.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/gazayeusv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.bbcook.cn/Article/details/gpxontezw.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.bbcook.cn/Article/details/gxapkssnv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.yfazqb.com/Article/details/grpwcmjix.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.epnwcf.com/Article/details/gfymnlnsl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/gyotpwbsm.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fktsv.cn/Article/details/gigbsjzyq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.vehdjk.com/Article/details/giuxfcjfw.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.tarul.cn/Article/details/gdkodapye.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/ghbswpqfb.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fktsv.cn/Article/details/gknfyhdco.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gfvsdtthn.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.yfazqb.com/Article/details/gfrbydiqc.sHtML

val m = mapOf("a" to 1)
来源：http://baike.yfazqb.com/Article/details/geaxsilkm.sHtML

[T14] Kotlin：循环
来源：http://www.share.bbcook.cn/Article/details/glolkxqfy.sHtML

for (i in 1..10) println(i)
来源：http://m.share.epnwcf.com/Article/details/ghzspkazz.sHtML

[T15] Kotlin：接口
来源：http://mobile.yfazqb.com/Article/details/ggkhmsagl.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.vehdjk.com/Article/details/gysoxoonl.sHtML

[T16] Swift：Hello World
来源：http://www.share.epnwcf.com/Article/details/gukqwtpmn.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gxlezjfkn.sHtML

[T17] Swift：变量与常量
来源：http://read.share.bbcook.cn/Article/details/gslavjufr.sHtML

var a = 1;  let b = 2
来源：http://m.share.yfazqb.com/Article/details/gmrihewer.sHtML

[T18] Swift：字符串插值
来源：http://baike.fktsv.cn/Article/details/gnkensirg.sHtML

"值: \(b)"
来源：http://www.share.sjlbkw.cn/Article/details/gmzdzirlv.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.tarul.cn/Article/details/geximkbqv.sHtML

if let n = opt { print(n) }
来源：http://baike.vehdjk.com/Article/details/ggvrezamp.sHtML

[T20] Swift：数组操作
来源：http://baike.fktsv.cn/Article/details/gumzgmbhx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/gtlsgycgi.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/guizvafpt.sHtML

for x in a { print(x) }
来源：http://www.m.share.bbcook.cn/Article/details/gjhaavhiz.sHtML

[T22] Swift：字典
来源：http://www.blog.yfazqb.com/Article/details/gfuzynjhv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.tarul.cn/Article/details/gnmdfuevd.sHtML

[T23] Swift：函数
来源：http://mobile.sjlbkw.cn/Article/details/gnhpgcjxq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.yfazqb.com/Article/details/glsaoctbh.sHtML

[T24] Swift：闭包
来源：http://www.m.share.tarul.cn/Article/details/gforsjhjb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwtovjbd.sHtML

[T25] Swift：结构体
来源：http://baike.vehdjk.com/Article/details/guolkskju.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/ggnmzsmji.sHtML

[T26] Swift：类与重写
来源：http://baike.bbcook.cn/Article/details/gvthwxwev.sHtML

class A: Base { override func f() {} }
来源：http://blog.sjlbkw.cn/Article/details/gcchqrwuo.sHtML

[T27] Swift：错误处理
来源：http://www.share.fktsv.cn/Article/details/gunheilkd.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.vehdjk.com/Article/details/gycfhufmm.sHtML

[T28] Swift：枚举
来源：http://www.blog.bbcook.cn/Article/details/glpxnwevf.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gxjshesnj.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.tarul.cn/Article/details/gulkpudva.sHtML

guard let x = opt else { return }
来源：http://wap.bbcook.cn/Article/details/gbudvmnew.sHtML

[T30] Swift：协议
来源：http://www.share.bbcook.cn/Article/details/gkepkahck.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.tarul.cn/Article/details/gfxpourjd.sHtML

[T31] Lua：Hello World
来源：http://baike.fktsv.cn/Article/details/gexcambok.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gsckjgrht.sHtML

[T32] Lua：局部变量
来源：http://blog.fktsv.cn/Article/details/gjqbjbcjk.sHtML

local a = 1
来源：http://3g.fktsv.cn/Article/details/germmlyrs.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fktsv.cn/Article/details/gskeegjrp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fktsv.cn/Article/details/gcuwbharf.sHtML

[T34] Lua：遍历表
来源：http://m.share.bbcook.cn/Article/details/gwhyqsidy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.sjlbkw.cn/Article/details/gloufkrep.sHtML

[T35] Lua：字典表
来源：http://wap.bbcook.cn/Article/details/gpstrxtax.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.bbcook.cn/Article/details/givhhirak.sHtML

[T36] Lua：函数
来源：http://3g.sjlbkw.cn/Article/details/gketavkya.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.tarul.cn/Article/details/gpzglszkf.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.epnwcf.com/Article/details/glhrwlsdh.sHtML

"a" .. "b"
来源：http://www.m.share.bbcook.cn/Article/details/gnngaabpl.sHtML

[T38] Lua：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/grxzlokuu.sHtML

if x > 0 then print("正") end
来源：http://www.share.tarul.cn/Article/details/gunxrtjep.sHtML

[T39] Lua：模式匹配
来源：http://blog.epnwcf.com/Article/details/gceudifzh.sHtML

string.find(s, "%d+")
来源：http://blog.bbcook.cn/Article/details/gwzdzbrvh.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/gjyagjcnm.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.sjlbkw.cn/Article/details/glzpcfqdg.sHtML

[T41] Perl：Hello World
来源：http://read.share.vehdjk.com/Article/details/gvjnrvbxm.sHtML

print "Hello\n";
来源：http://www.share.bbcook.cn/Article/details/gtjxycplm.sHtML

[T42] Perl：变量类型
来源：http://m.share.vehdjk.com/Article/details/gamxzkwse.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.vehdjk.com/Article/details/gpgkmiutq.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gjmoavdua.sHtML

"值: $a"
来源：http://www.blog.fktsv.cn/Article/details/gdnjyiwrq.sHtML

[T44] Perl：条件
来源：http://read.share.epnwcf.com/Article/details/ghzwfhqkg.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.vehdjk.com/Article/details/geodiyipi.sHtML

[T45] Perl：数组遍历
来源：http://blog.bbcook.cn/Article/details/gtxouaoaq.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.bbcook.cn/Article/details/gsobcqatw.sHtML

[T46] Perl：哈希操作
来源：http://wap.tarul.cn/Article/details/gsndoerii.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpwflcjs.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.yfazqb.com/Article/details/gjvfdplsx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvlyewqz.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/grzydcbyi.sHtML

$s =~ s/old/new/g;
来源：http://m.share.tarul.cn/Article/details/grranqhuh.sHtML

[T49] Perl：函数
来源：http://www.blog.epnwcf.com/Article/details/gzzgafuqy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gxbjyoxku.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gpjtgwvww.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fktsv.cn/Article/details/gdfaexful.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwyjshryi.sHtML

[T51] Scala：Hello World
来源：http://wap.tarul.cn/Article/details/grvkqycqx.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gocitpqvq.sHtML

[T52] Scala：变量
来源：http://3g.epnwcf.com/Article/details/gxogbddsq.sHtML

val a = 1;  var b = 2
来源：http://www.share.epnwcf.com/Article/details/geoslprcf.sHtML

[T53] Scala：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gpdbqcfee.sHtML

s"值: $b"
来源：http://mobile.tarul.cn/Article/details/gwhtokxwt.sHtML

[T54] Scala：集合映射
来源：http://m.share.bbcook.cn/Article/details/ggidieisi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.epnwcf.com/Article/details/gxlonnsmc.sHtML

[T55] Scala：集合过滤
来源：http://wap.epnwcf.com/Article/details/glpmliphl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.yfazqb.com/Article/details/gzgqqvofl.sHtML

[T56] Scala：样例类
来源：http://3g.epnwcf.com/Article/details/ggxheqiqy.sHtML

case class User(name: String, age: Int)
来源：http://read.share.vehdjk.com/Article/details/grpflbjam.sHtML

[T57] Scala：模式匹配
来源：http://blog.vehdjk.com/Article/details/gqisdpaqf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.yfazqb.com/Article/details/gzaokmqrw.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fktsv.cn/Article/details/ggjiaeazs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.bbcook.cn/Article/details/gjuuocgpf.sHtML

[T59] Scala：循环
来源：http://www.share.tarul.cn/Article/details/gjtmgttys.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.vehdjk.com/Article/details/gromppplw.sHtML

[T60] Scala：折叠
来源：http://baike.sjlbkw.cn/Article/details/glivvorhg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.vehdjk.com/Article/details/gxseazqzx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvthcmaii.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/gnwellrut.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqgignywy.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.yfazqb.com/Article/details/gzummorgo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.yfazqb.com/Article/details/grqnxilqx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.sjlbkw.cn/Article/details/givskntpa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.epnwcf.com/Article/details/gytmoejsb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.tarul.cn/Article/details/grtptysvb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.epnwcf.com/Article/details/gfnphvivj.sHtML

[U04] Py：变量调试打印
来源：http://www.share.vehdjk.com/Article/details/gwhvfgpuf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.bbcook.cn/Article/details/grbnxiayi.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/ggqyauptz.sHtML

list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/ggzvtusdy.sHtML

[U06] Py：合并两个字典
来源：http://mobile.vehdjk.com/Article/details/gmgwuwwpm.sHtML

{**a, **b}
来源：http://blog.tarul.cn/Article/details/gugukitwe.sHtML

[U07] Py：反转字典键值
来源：http://www.share.sjlbkw.cn/Article/details/ggkqrwrif.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.yfazqb.com/Article/details/gawfpixnz.sHtML

[U08] Py：展平二维列表
来源：http://mobile.tarul.cn/Article/details/gzuudrwap.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.epnwcf.com/Article/details/gobeueije.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.yfazqb.com/Article/details/grcmzznuj.sHtML

max(d, key=d.get)
来源：http://read.share.yfazqb.com/Article/details/gziolkujf.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.tarul.cn/Article/details/gyyrhosfb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcmdyicw.sHtML


<!-- 参考信息 -->