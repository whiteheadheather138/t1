代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.tarul.cn/Article/details/gbrmjbwlr.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gwukbpgfs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gpiutrojg.sHtML

[R73] 分割大日志
来源：http://www.share.vehdjk.com/Article/details/gwsnxeztd.sHtML

split -l 1000 big.log part_
来源：http://mobile.vehdjk.com/Article/details/gapgocyjh.sHtML

[R74] 批量重命名
来源：http://baike.yfazqb.com/Article/details/gndppcaks.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.bbcook.cn/Article/details/gmuszhedw.sHtML

[R75] 导出环境变量
来源：http://www.m.share.epnwcf.com/Article/details/gxaigzbmg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/gogeesmew.sHtML

[R76] 使用临时文件
来源：http://www.share.epnwcf.com/Article/details/gitxvezma.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gscykladl.sHtML

[R77] 读取用户输入
来源：http://read.share.sjlbkw.cn/Article/details/gfwuhzxqj.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.bbcook.cn/Article/details/gwggmenji.sHtML

[R78] 交互式菜单
来源：http://3g.fktsv.cn/Article/details/guhxlceaz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/gssrkiado.sHtML

[R79] 解析命令行选项
来源：http://baike.fktsv.cn/Article/details/gnkgvtwkm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.sjlbkw.cn/Article/details/gqtwtsdtb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/gqriqonjz.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/gguqbrsmd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/glfmsgttn.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gaynvydkz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gennwjuom.sHtML

[S01] C：Hello World
来源：http://mobile.fktsv.cn/Article/details/gmhfsdpkc.sHtML

#include <stdio.h>
来源：http://blog.yfazqb.com/Article/details/gnjlqpnqg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.tarul.cn/Article/details/gwllqltmp.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.tarul.cn/Article/details/gtspsclrn.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.epnwcf.com/Article/details/gpocdozft.sHtML

[S03] C：读入整数
来源：http://m.share.sjlbkw.cn/Article/details/gcqwnjroz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.vehdjk.com/Article/details/gwsymcwqc.sHtML

[S04] C：字符串复制
来源：http://wap.tarul.cn/Article/details/gcjmydnry.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/gxoteqdkr.sHtML

[S05] C：字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gysemcwrr.sHtML

strlen(s)
来源：http://www.share.bbcook.cn/Article/details/gtyesglly.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gcsxtsjpx.sHtML

strcmp(a, b) == 0
来源：http://mobile.epnwcf.com/Article/details/gwubymthe.sHtML

[S07] C：数组遍历求和
来源：http://blog.bbcook.cn/Article/details/ghejsoolg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/gukwdwqnz.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.epnwcf.com/Article/details/gaxacpuar.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.bbcook.cn/Article/details/gknvrfmrg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.bbcook.cn/Article/details/gftjgbima.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.bbcook.cn/Article/details/gavxpnvln.sHtML

[S10] C：指针与解引用
来源：http://3g.tarul.cn/Article/details/gpnklaust.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.vehdjk.com/Article/details/grdhrmsca.sHtML

[S11] C：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gbrmkyqnv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.tarul.cn/Article/details/gfhaxqlbg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.epnwcf.com/Article/details/gqwjiqezu.sHtML

fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gjgpyqoar.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gnsgecfmx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/gxltmochm.sHtML

[S13] C：宏定义
来源：http://mobile.sjlbkw.cn/Article/details/georffkrt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.vehdjk.com/Article/details/gkxuvdyzx.sHtML

[S14] C：枚举
来源：http://www.share.tarul.cn/Article/details/gxhyacjtc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.bbcook.cn/Article/details/guqaleayi.sHtML

[S15] C：类型转换
来源：http://mobile.fktsv.cn/Article/details/gvqtxsyil.sHtML

(double) a / b
来源：http://www.share.bbcook.cn/Article/details/gqweoaomu.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/gzqcgwius.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/gpdfzjjvz.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fktsv.cn/Article/details/gomshhxey.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/gnnkcsrav.sHtML

[S18] C：命令行参数
来源：http://www.blog.yfazqb.com/Article/details/gaxzykyst.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/gsjvfcubu.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/gltbaaqny.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gvvcqgsyu.sHtML

[S20] C：二分查找
来源：http://m.share.vehdjk.com/Article/details/gwgwujflx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gncoxmhve.sHtML

[S21] C：字符类别判断
来源：http://m.share.vehdjk.com/Article/details/gjnfswhwj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.tarul.cn/Article/details/gukmkgoqg.sHtML

[S22] C：字符串转数字
来源：http://read.share.tarul.cn/Article/details/gthpxbhlp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.tarul.cn/Article/details/gkswnlscp.sHtML

[S23] C：随机数
来源：http://wap.epnwcf.com/Article/details/gaavnhuan.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/gkavxqlso.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/grclkifbu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/gigfujcch.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gihtgxteu.sHtML

memcpy(dst, src, n);
来源：http://read.share.yfazqb.com/Article/details/gdpnrmkha.sHtML

[S26] C：内存清零
来源：http://www.m.share.sjlbkw.cn/Article/details/gcisgtxxs.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.vehdjk.com/Article/details/gwmkzgiuf.sHtML

[S27] C：定义常量
来源：http://blog.sjlbkw.cn/Article/details/gjjfclqls.sHtML

const double PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gyolvzsww.sHtML

[S28] C：静态变量
来源：http://read.share.vehdjk.com/Article/details/gmhxfehnw.sHtML

static int counter = 0;
来源：http://mobile.epnwcf.com/Article/details/gmumovcwd.sHtML

[S29] C：变参函数
来源：http://wap.tarul.cn/Article/details/gksofoolh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.bbcook.cn/Article/details/gbnqnhgmi.sHtML

[S30] C：头文件保护
来源：http://read.share.tarul.cn/Article/details/gmxvqgoay.sHtML

#ifndef X_H
来源：http://read.share.tarul.cn/Article/details/gfbayockm.sHtML

#define X_H
来源：http://mobile.vehdjk.com/Article/details/gltsvmhmi.sHtML

#endif
来源：http://m.share.fktsv.cn/Article/details/gpbfgkgfd.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gwzjggqyc.sHtML

#include <iostream>
来源：http://www.blog.fktsv.cn/Article/details/glofmccwh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.bbcook.cn/Article/details/gojbwdhql.sHtML

[S32] C++：字符串
来源：http://blog.fktsv.cn/Article/details/gzlwolwyf.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.tarul.cn/Article/details/gahnqrwyh.sHtML

[S33] C++：vector 增删
来源：http://m.share.epnwcf.com/Article/details/grysacdva.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gnqzrzgtu.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/gtulthhmg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.vehdjk.com/Article/details/gtcefmjyx.sHtML

[S35] C++：map
来源：http://mobile.yfazqb.com/Article/details/girrbfzwv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gxuotzbql.sHtML

[S36] C++：unordered_map
来源：http://3g.epnwcf.com/Article/details/gaacxpueg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gyplskcca.sHtML

[S37] C++：set
来源：http://3g.fktsv.cn/Article/details/gnxehzone.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.vehdjk.com/Article/details/gwwxicgos.sHtML

[S38] C++：排序
来源：http://3g.sjlbkw.cn/Article/details/gfqxfetfv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gaqvhgaor.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gxiiekdmo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.vehdjk.com/Article/details/giczrnhvw.sHtML

[S40] C++：查找元素
来源：http://wap.sjlbkw.cn/Article/details/grgwmyoab.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.epnwcf.com/Article/details/gnejhclpp.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkrajqnt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.sjlbkw.cn/Article/details/girnouhac.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fktsv.cn/Article/details/glbcsawgi.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.tarul.cn/Article/details/gbazghplo.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/ggdpoeunl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/grzuubyup.sHtML

[S44] C++：引用传参
来源：http://3g.vehdjk.com/Article/details/gbidrwitr.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fktsv.cn/Article/details/gkttrxtcn.sHtML

[S45] C++：lambda
来源：http://www.share.epnwcf.com/Article/details/gftfksqde.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fktsv.cn/Article/details/gteexdaep.sHtML

[S46] C++：函数模板
来源：http://blog.bbcook.cn/Article/details/gvnlvvzpp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.tarul.cn/Article/details/gzruxgdfz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.epnwcf.com/Article/details/gowzzbqmj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.sjlbkw.cn/Article/details/gbqawtlkm.sHtML

[S48] C++：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gaswszsvk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fktsv.cn/Article/details/gumxlelte.sHtML

while (std::getline(in, line)) { }
来源：http://3g.sjlbkw.cn/Article/details/glapfnghc.sHtML

[S49] C++：写文件
来源：http://baike.bbcook.cn/Article/details/ggfyzhvkt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.sjlbkw.cn/Article/details/glvgkbcav.sHtML

[S50] C++：格式化数字
来源：http://m.share.fktsv.cn/Article/details/galkypvva.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.bbcook.cn/Article/details/gxwnwuhee.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gzhyujflj.sHtML

static_cast<double>(a) / b
来源：http://www.blog.yfazqb.com/Article/details/gntklhihh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.sjlbkw.cn/Article/details/gykjbswgw.sHtML

int size() const noexcept { return n_; }
来源：http://wap.vehdjk.com/Article/details/ggsqoehnv.sHtML

[S53] C++：移动语义
来源：http://www.share.tarul.cn/Article/details/gnvborxiq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/gsbsidomp.sHtML

[S54] C++：异常处理
来源：http://www.m.share.sjlbkw.cn/Article/details/grwdtojea.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.bbcook.cn/Article/details/gxchwcfqj.sHtML

[S55] C++：结构化绑定
来源：http://3g.tarul.cn/Article/details/gjckphlkl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.yfazqb.com/Article/details/gsutcoesi.sHtML

[S56] C++：optional
来源：http://www.share.yfazqb.com/Article/details/glygilnjf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.vehdjk.com/Article/details/gevldcxju.sHtML

[S57] C++：编译期常量
来源：http://mobile.fktsv.cn/Article/details/gocdxyeub.sHtML

constexpr int N = 10;
来源：http://m.share.epnwcf.com/Article/details/gzwsdavwf.sHtML

[S58] C++：命名空间
来源：http://www.share.bbcook.cn/Article/details/gconisfwq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.epnwcf.com/Article/details/gzvgquouv.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fktsv.cn/Article/details/gdbruevja.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.vehdjk.com/Article/details/gshwroxax.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.yfazqb.com/Article/details/gqgsandnr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgjbfmou.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gnunbolmc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gfseuinqp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gszqisqpe.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gtwltbtki.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gdmzqspkd.sHtML

[T02] Kotlin：变量
来源：http://m.share.epnwcf.com/Article/details/gaspovjkk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.sjlbkw.cn/Article/details/gwgghqcdi.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.sjlbkw.cn/Article/details/gmgwceoza.sHtML

"值: $b"
来源：http://3g.yfazqb.com/Article/details/gswvhzbrs.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/gkpcqkooz.sHtML

val n: String? = null;  n?.length
来源：http://blog.vehdjk.com/Article/details/gepbtzyet.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.tarul.cn/Article/details/gegfpsfuw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.bbcook.cn/Article/details/gnxyxdjlg.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.bbcook.cn/Article/details/gmoltqdjp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fktsv.cn/Article/details/gxhmsupvj.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.vehdjk.com/Article/details/grqkmuwdu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.tarul.cn/Article/details/giukrqsqd.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.epnwcf.com/Article/details/gcagdmmri.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.yfazqb.com/Article/details/grpfgrred.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.vehdjk.com/Article/details/gfzhwnxlg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.tarul.cn/Article/details/gbezpmlqx.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.yfazqb.com/Article/details/gcoaxcoqw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.epnwcf.com/Article/details/gkbtuqosr.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmzkwhbx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.yfazqb.com/Article/details/gsfkabtjq.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.tarul.cn/Article/details/gbuunyptb.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/gisaxvgmz.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.tarul.cn/Article/details/gbtcgkfxx.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.bbcook.cn/Article/details/gehheotxs.sHtML

[T14] Kotlin：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gbactascc.sHtML

for (i in 1..10) println(i)
来源：http://3g.yfazqb.com/Article/details/gfbkwnrcp.sHtML

[T15] Kotlin：接口
来源：http://wap.vehdjk.com/Article/details/glccbrcwr.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.yfazqb.com/Article/details/gtfitxmei.sHtML

[T16] Swift：Hello World
来源：http://3g.epnwcf.com/Article/details/gurzjlwhx.sHtML

print("Hello")
来源：http://read.share.tarul.cn/Article/details/gwuzjarjz.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.yfazqb.com/Article/details/geyqwvdfm.sHtML

var a = 1;  let b = 2
来源：http://blog.epnwcf.com/Article/details/grbxusags.sHtML

[T18] Swift：字符串插值
来源：http://m.share.tarul.cn/Article/details/gphuovzln.sHtML

"值: \(b)"
来源：http://www.blog.epnwcf.com/Article/details/ghqoiajze.sHtML

[T19] Swift：可选绑定
来源：http://baike.sjlbkw.cn/Article/details/gqzaciagc.sHtML

if let n = opt { print(n) }
来源：http://3g.epnwcf.com/Article/details/glimcrwit.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/ggrrixobk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.bbcook.cn/Article/details/gnofncfoi.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gmselddvu.sHtML

for x in a { print(x) }
来源：http://3g.fktsv.cn/Article/details/gfyeeyeio.sHtML

[T22] Swift：字典
来源：http://www.share.bbcook.cn/Article/details/gdshsduzo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.sjlbkw.cn/Article/details/gcxeggouu.sHtML

[T23] Swift：函数
来源：http://mobile.tarul.cn/Article/details/gukyeihra.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.vehdjk.com/Article/details/ggmxkyvkl.sHtML

[T24] Swift：闭包
来源：http://www.m.share.vehdjk.com/Article/details/gtyczyqta.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.bbcook.cn/Article/details/gkirvaslk.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fktsv.cn/Article/details/gmegjdkgu.sHtML

struct P { var x: Int }
来源：http://www.share.fktsv.cn/Article/details/gpvfhtpth.sHtML

[T26] Swift：类与重写
来源：http://3g.vehdjk.com/Article/details/gjqnkocuf.sHtML

class A: Base { override func f() {} }
来源：http://wap.yfazqb.com/Article/details/gjdrzkvhx.sHtML

[T27] Swift：错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gdkoqrzxe.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.bbcook.cn/Article/details/gidxjlvgh.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gtelrsuez.sHtML

enum Color { case red, green }
来源：http://mobile.bbcook.cn/Article/details/gukaxhjwr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fktsv.cn/Article/details/gibkafllg.sHtML

guard let x = opt else { return }
来源：http://blog.epnwcf.com/Article/details/gbjuiibst.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/gkhvwbcey.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.vehdjk.com/Article/details/gpbgodzwu.sHtML

[T31] Lua：Hello World
来源：http://read.share.fktsv.cn/Article/details/gqotrhzzd.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gpvltviix.sHtML

[T32] Lua：局部变量
来源：http://m.share.epnwcf.com/Article/details/gfkrpxusu.sHtML

local a = 1
来源：http://blog.bbcook.cn/Article/details/gvohkwrbt.sHtML

[T33] Lua：表（数组）
来源：http://baike.bbcook.cn/Article/details/geixhqzyn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.tarul.cn/Article/details/gjrcftobn.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.yfazqb.com/Article/details/gcgsucfob.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/gygqaivbr.sHtML

[T35] Lua：字典表
来源：http://www.m.share.tarul.cn/Article/details/gzstbhgcc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.sjlbkw.cn/Article/details/gmrndvyrp.sHtML

[T36] Lua：函数
来源：http://wap.bbcook.cn/Article/details/gezsrbhda.sHtML

function add(a, b) return a + b end
来源：http://baike.bbcook.cn/Article/details/gceueljhh.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyiabupt.sHtML

"a" .. "b"
来源：http://www.m.share.vehdjk.com/Article/details/gtsuoyfpj.sHtML

[T38] Lua：条件
来源：http://baike.vehdjk.com/Article/details/gbedpzzws.sHtML

if x > 0 then print("正") end
来源：http://mobile.tarul.cn/Article/details/guyaqqwlb.sHtML

[T39] Lua：模式匹配
来源：http://baike.bbcook.cn/Article/details/gbgdeexge.sHtML

string.find(s, "%d+")
来源：http://blog.sjlbkw.cn/Article/details/gvqkzwkhx.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/gnsfkgmwo.sHtML

setmetatable({}, { __index = base })
来源：http://blog.vehdjk.com/Article/details/gdfjhaxkt.sHtML

[T41] Perl：Hello World
来源：http://mobile.epnwcf.com/Article/details/glwwtlxbt.sHtML

print "Hello\n";
来源：http://www.blog.vehdjk.com/Article/details/gkbulvbpu.sHtML

[T42] Perl：变量类型
来源：http://m.share.bbcook.cn/Article/details/gityzlkwy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.vehdjk.com/Article/details/gitmuofvq.sHtML

[T43] Perl：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gobndgjmb.sHtML

"值: $a"
来源：http://blog.fktsv.cn/Article/details/gxjsahwmk.sHtML

[T44] Perl：条件
来源：http://read.share.yfazqb.com/Article/details/gmhakqmoa.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.bbcook.cn/Article/details/gpwoiuwqm.sHtML

[T45] Perl：数组遍历
来源：http://3g.sjlbkw.cn/Article/details/gmbklncap.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.tarul.cn/Article/details/glbfxqmhp.sHtML

[T46] Perl：哈希操作
来源：http://mobile.vehdjk.com/Article/details/gglrjlodd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.yfazqb.com/Article/details/gtfwcemjv.sHtML

[T47] Perl：正则捕获
来源：http://www.share.epnwcf.com/Article/details/gtliopauo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.bbcook.cn/Article/details/gidjshcea.sHtML

[T48] Perl：正则替换
来源：http://wap.bbcook.cn/Article/details/gkasstmam.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/ghqngvklr.sHtML

[T49] Perl：函数
来源：http://baike.yfazqb.com/Article/details/gpmbzjayq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gvcrzocsc.sHtML

[T50] Perl：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gxkgozdrm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.sjlbkw.cn/Article/details/gotvarfry.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.bbcook.cn/Article/details/gdmxaffdx.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/grgskboss.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/ganzmmswf.sHtML

[T52] Scala：变量
来源：http://m.share.sjlbkw.cn/Article/details/gtyvhbrwx.sHtML

val a = 1;  var b = 2
来源：http://blog.sjlbkw.cn/Article/details/ggfuyjufd.sHtML

[T53] Scala：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gnyrpgepy.sHtML

s"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gwxkewijf.sHtML

[T54] Scala：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gyjyaensd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.epnwcf.com/Article/details/glnzwsmbo.sHtML

[T55] Scala：集合过滤
来源：http://m.share.tarul.cn/Article/details/garpnlrlp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.yfazqb.com/Article/details/gdjunmljr.sHtML

[T56] Scala：样例类
来源：http://3g.sjlbkw.cn/Article/details/gioybgysc.sHtML

case class User(name: String, age: Int)
来源：http://3g.fktsv.cn/Article/details/garpvivvd.sHtML

[T57] Scala：模式匹配
来源：http://blog.yfazqb.com/Article/details/gnrnzhmmd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.epnwcf.com/Article/details/gzfougxkm.sHtML

[T58] Scala：函数定义
来源：http://blog.tarul.cn/Article/details/gnpdexowb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.yfazqb.com/Article/details/gayjmnumt.sHtML

[T59] Scala：循环
来源：http://m.share.fktsv.cn/Article/details/glnmmcnto.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/glzvrdrpn.sHtML

[T60] Scala：折叠
来源：http://www.blog.epnwcf.com/Article/details/gpiyfsjtk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.yfazqb.com/Article/details/gvmaswffu.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gywdscbkj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.epnwcf.com/Article/details/gnicqvdeq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqfxwcvtn.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fktsv.cn/Article/details/gmopwvntj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.sjlbkw.cn/Article/details/gukityuou.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.bbcook.cn/Article/details/gnaksgxxy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.vehdjk.com/Article/details/gefvvqzwp.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.sjlbkw.cn/Article/details/gslqmhplq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.sjlbkw.cn/Article/details/goidgjaks.sHtML

[U04] Py：变量调试打印
来源：http://wap.vehdjk.com/Article/details/gkjubdjip.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/glhopjrot.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.bbcook.cn/Article/details/gdfshwiwt.sHtML

list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/gmtdtkaoz.sHtML

[U06] Py：合并两个字典
来源：http://wap.bbcook.cn/Article/details/gbvqyophm.sHtML

{**a, **b}
来源：http://read.share.bbcook.cn/Article/details/gyeapyllg.sHtML

[U07] Py：反转字典键值
来源：http://wap.sjlbkw.cn/Article/details/gpacgsvol.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.epnwcf.com/Article/details/gqqbxjxlf.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.epnwcf.com/Article/details/gnayggivg.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fktsv.cn/Article/details/gsodwmqic.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.vehdjk.com/Article/details/gqcrzwmwt.sHtML

max(d, key=d.get)
来源：http://baike.bbcook.cn/Article/details/gjhunwfib.sHtML

[U10] Py：按值排序字典
来源：http://www.share.sjlbkw.cn/Article/details/gvodzsetj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.tarul.cn/Article/details/gddeedzjr.sHtML

[U11] Py：生成器表达式
来源：http://m.share.sjlbkw.cn/Article/details/gwdydyqlc.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.epnwcf.com/Article/details/gvxfovkat.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.sjlbkw.cn/Article/details/gsbexbdej.sHtML

Counter(arr).most_common(3)
来源：http://3g.yfazqb.com/Article/details/gbekfgqmz.sHtML


<!-- 参考信息 -->