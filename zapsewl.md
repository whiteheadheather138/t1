代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fktsv.cn/Article/details/gvnltqcva.sHtML

[R72] 等待端口就绪
来源：http://read.share.yfazqb.com/Article/details/glexaiieg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gvjeudbql.sHtML

[R73] 分割大日志
来源：http://blog.vehdjk.com/Article/details/gulvinoct.sHtML

split -l 1000 big.log part_
来源：http://baike.epnwcf.com/Article/details/ghqrhxhuq.sHtML

[R74] 批量重命名
来源：http://read.share.tarul.cn/Article/details/gthygjcsu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.tarul.cn/Article/details/gpvtxxjkf.sHtML

[R75] 导出环境变量
来源：http://wap.sjlbkw.cn/Article/details/gpttnkdis.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.sjlbkw.cn/Article/details/gssjvfxkl.sHtML

[R76] 使用临时文件
来源：http://www.m.share.vehdjk.com/Article/details/gnetophag.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gvkucfljl.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/gxrrenmts.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gqkdkoyzd.sHtML

[R78] 交互式菜单
来源：http://3g.yfazqb.com/Article/details/gvfvakfxr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/ggpntxlvg.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.epnwcf.com/Article/details/gsbgyklvs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/gkocdlrvg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.sjlbkw.cn/Article/details/gpceofkbe.sHtML

time ./run.sh
来源：http://m.share.yfazqb.com/Article/details/gsjhqvpoj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjzpxpkvc.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/gqvqmnrmb.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gscjlqgkz.sHtML

[S01] C：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gaveffdfw.sHtML

#include <stdio.h>
来源：http://baike.tarul.cn/Article/details/gzuyojnxv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/goeuuanyk.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gnruhmluh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fktsv.cn/Article/details/guyknhtdm.sHtML

[S03] C：读入整数
来源：http://mobile.fktsv.cn/Article/details/gkkqhickl.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/gykszbutt.sHtML

[S04] C：字符串复制
来源：http://blog.yfazqb.com/Article/details/gdbpkqwsd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.yfazqb.com/Article/details/gltjujhfj.sHtML

[S05] C：字符串长度
来源：http://mobile.tarul.cn/Article/details/gpigoawuu.sHtML

strlen(s)
来源：http://wap.bbcook.cn/Article/details/gzbsdpfve.sHtML

[S06] C：字符串比较
来源：http://www.share.yfazqb.com/Article/details/gdltpraka.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxbwqmku.sHtML

[S07] C：数组遍历求和
来源：http://www.share.bbcook.cn/Article/details/ghabhuftl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.yfazqb.com/Article/details/grxzjkrau.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.sjlbkw.cn/Article/details/gdgslhxbd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/ggzqjxmow.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.yfazqb.com/Article/details/gvkeqeryf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fktsv.cn/Article/details/gtrqvhxib.sHtML

[S10] C：指针与解引用
来源：http://www.share.tarul.cn/Article/details/gocxkcjsi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.vehdjk.com/Article/details/gfzplobxg.sHtML

[S11] C：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gclxwtqde.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/gsmoqwroi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/gjdtujgyj.sHtML

fclose(f);
来源：http://wap.yfazqb.com/Article/details/gvukwaqwi.sHtML

[S12] C：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gjmwfkcdz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/govytsfpm.sHtML

[S13] C：宏定义
来源：http://www.blog.epnwcf.com/Article/details/gocvajbgg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.epnwcf.com/Article/details/giuupgpln.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/gjkdbyffr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.epnwcf.com/Article/details/gmryygrqy.sHtML

[S15] C：类型转换
来源：http://3g.yfazqb.com/Article/details/gbirghnli.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/gpvqepvmc.sHtML

[S16] C：位操作置位
来源：http://3g.epnwcf.com/Article/details/ghzwmyeyu.sHtML

x |= (1 << 3);
来源：http://m.share.fktsv.cn/Article/details/gltlremge.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.yfazqb.com/Article/details/grgtfljwb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqazrcvjo.sHtML

[S18] C：命令行参数
来源：http://baike.yfazqb.com/Article/details/grdtwtmxf.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/gcfkjscff.sHtML

[S19] C：快速排序
来源：http://read.share.fktsv.cn/Article/details/gyydzxtxy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/guihawole.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/gpaprhlvw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gbnhzufme.sHtML

[S21] C：字符类别判断
来源：http://m.share.fktsv.cn/Article/details/gcylhzvrs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/gfnxeslde.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/ggbdyxwly.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fktsv.cn/Article/details/gamadvtlj.sHtML

[S23] C：随机数
来源：http://baike.fktsv.cn/Article/details/gpqbotllz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.vehdjk.com/Article/details/gpczcbnxy.sHtML

[S24] C：获取本地时间
来源：http://read.share.yfazqb.com/Article/details/gfkxcykir.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fktsv.cn/Article/details/gxoaeqzry.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/ggzekpuhq.sHtML

memcpy(dst, src, n);
来源：http://blog.bbcook.cn/Article/details/gjbpmrkyi.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/gkianbrhv.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.yfazqb.com/Article/details/gdxybfpgt.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/ghqdlmdnb.sHtML

const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyozohyio.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/gqaijugjl.sHtML

static int counter = 0;
来源：http://wap.epnwcf.com/Article/details/ghzfcdnln.sHtML

[S29] C：变参函数
来源：http://blog.tarul.cn/Article/details/gethgrpjo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gtladqtre.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/gnltlbffb.sHtML

#ifndef X_H
来源：http://www.share.fktsv.cn/Article/details/ghykajpih.sHtML

#define X_H
来源：http://wap.sjlbkw.cn/Article/details/gmypiucec.sHtML

#endif
来源：http://www.share.epnwcf.com/Article/details/gbtmrzctq.sHtML

[S31] C++：Hello World
来源：http://read.share.yfazqb.com/Article/details/gezscxoqb.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gzksqdtuv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.bbcook.cn/Article/details/gzfkvzdkl.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/ggfjtfehv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.sjlbkw.cn/Article/details/glywqgmyu.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/gnxonoqfb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.bbcook.cn/Article/details/gwhzrsiqz.sHtML

[S34] C++：遍历 vector
来源：http://mobile.yfazqb.com/Article/details/goathttzz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.vehdjk.com/Article/details/gdfsztjpx.sHtML

[S35] C++：map
来源：http://www.share.yfazqb.com/Article/details/glrwvyckm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gocdjiseg.sHtML

[S36] C++：unordered_map
来源：http://blog.bbcook.cn/Article/details/gtkwvdnwm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gfsmyvuuk.sHtML

[S37] C++：set
来源：http://mobile.epnwcf.com/Article/details/guyigxnym.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.epnwcf.com/Article/details/glyiptrgy.sHtML

[S38] C++：排序
来源：http://3g.epnwcf.com/Article/details/gbjnilppl.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gjzhekjdp.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/ghiorudmy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/gzkpqjgzw.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/gfzaitplz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fktsv.cn/Article/details/gjyskvblp.sHtML

[S41] C++：类与构造函数
来源：http://baike.bbcook.cn/Article/details/gxbnbxfcg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fktsv.cn/Article/details/ggvjgszcg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/gszrxembp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fktsv.cn/Article/details/gktutppia.sHtML

[S43] C++：智能指针
来源：http://blog.bbcook.cn/Article/details/gvizjfskz.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.yfazqb.com/Article/details/gqjtqrgit.sHtML

[S44] C++：引用传参
来源：http://3g.yfazqb.com/Article/details/gyyqmecdz.sHtML

void inc(int &x) { ++x; }
来源：http://blog.bbcook.cn/Article/details/gehgsxonn.sHtML

[S45] C++：lambda
来源：http://www.blog.sjlbkw.cn/Article/details/gtuuocqmp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.bbcook.cn/Article/details/gvfjuwgzw.sHtML

[S46] C++：函数模板
来源：http://3g.vehdjk.com/Article/details/gtrarsyuh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/ggqsmsxxw.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/grsjdlths.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.tarul.cn/Article/details/gzbuxdxmz.sHtML

[S48] C++：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gggqpnsws.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.sjlbkw.cn/Article/details/gcwdolyss.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.tarul.cn/Article/details/gzgmgnvyj.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/gjfxrkmsb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.epnwcf.com/Article/details/gkjatcveb.sHtML

[S50] C++：格式化数字
来源：http://3g.vehdjk.com/Article/details/gdxcndcqk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gafvujcmd.sHtML

[S51] C++：显式类型转换
来源：http://3g.vehdjk.com/Article/details/gpverldle.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/goikqzcir.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.epnwcf.com/Article/details/gmupxtnyn.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.tarul.cn/Article/details/gacvicars.sHtML

[S53] C++：移动语义
来源：http://read.share.fktsv.cn/Article/details/gvdqhyeay.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.vehdjk.com/Article/details/gftdefpgl.sHtML

[S54] C++：异常处理
来源：http://3g.sjlbkw.cn/Article/details/gzatpxtxd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.sjlbkw.cn/Article/details/gznhqltgk.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fktsv.cn/Article/details/goiyqzdbn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gujgohqgu.sHtML

[S56] C++：optional
来源：http://blog.vehdjk.com/Article/details/gbvukmkhh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.sjlbkw.cn/Article/details/gljslrmpw.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.tarul.cn/Article/details/ghyfmomut.sHtML

constexpr int N = 10;
来源：http://read.share.vehdjk.com/Article/details/gzlidmdiq.sHtML

[S58] C++：命名空间
来源：http://www.share.bbcook.cn/Article/details/gddlurrky.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.yfazqb.com/Article/details/gewqhvlib.sHtML

[S59] C++：静态断言
来源：http://www.blog.sjlbkw.cn/Article/details/gblyamlrr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.sjlbkw.cn/Article/details/gmqsjawxx.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/gkfbspihn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.bbcook.cn/Article/details/geefrqqzy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/geqtenzzv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/geupwrzyx.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gppmecirp.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/ghdmoivkx.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/gnzdcoijl.sHtML

[T02] Kotlin：变量
来源：http://read.share.tarul.cn/Article/details/gbsmxqlaw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.yfazqb.com/Article/details/gtsqzihaf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.vehdjk.com/Article/details/gzbyzjbjn.sHtML

"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/ggkuivqnl.sHtML

[T04] Kotlin：空安全
来源：http://m.share.bbcook.cn/Article/details/gxuabyjpy.sHtML

val n: String? = null;  n?.length
来源：http://blog.bbcook.cn/Article/details/ggwscgpzs.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.sjlbkw.cn/Article/details/gxtczgcve.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fktsv.cn/Article/details/guaxrwigs.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.bbcook.cn/Article/details/gipvlwgyg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.bbcook.cn/Article/details/glugfwbua.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/ghcbgbvpm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gszxwusue.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.yfazqb.com/Article/details/gqurqvbrp.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/gjhkwexnd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.yfazqb.com/Article/details/gtjartamb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.yfazqb.com/Article/details/gzcglehlh.sHtML

[T10] Kotlin：默认参数
来源：http://3g.epnwcf.com/Article/details/glxqxodmv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.yfazqb.com/Article/details/gaducidoh.sHtML

[T11] Kotlin：协程
来源：http://www.share.yfazqb.com/Article/details/glaludzlx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.tarul.cn/Article/details/gpybzkatv.sHtML

[T12] Kotlin：解构声明
来源：http://blog.epnwcf.com/Article/details/gnrwxqrbt.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gagzzubnw.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.bbcook.cn/Article/details/geqgxzxmb.sHtML

val m = mapOf("a" to 1)
来源：http://blog.vehdjk.com/Article/details/gguvpbwyc.sHtML

[T14] Kotlin：循环
来源：http://mobile.yfazqb.com/Article/details/gcpkcztna.sHtML

for (i in 1..10) println(i)
来源：http://blog.epnwcf.com/Article/details/gamhulabn.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/gnolbfesl.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fktsv.cn/Article/details/gsdepueuf.sHtML

[T16] Swift：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gkqzkrkrb.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gqvtomgjs.sHtML

[T17] Swift：变量与常量
来源：http://wap.epnwcf.com/Article/details/gjsbtdaza.sHtML

var a = 1;  let b = 2
来源：http://baike.epnwcf.com/Article/details/grmbebzky.sHtML

[T18] Swift：字符串插值
来源：http://wap.yfazqb.com/Article/details/guphodwmf.sHtML

"值: \(b)"
来源：http://www.blog.vehdjk.com/Article/details/gzprwpmrn.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.epnwcf.com/Article/details/gdslagzmi.sHtML

if let n = opt { print(n) }
来源：http://www.blog.epnwcf.com/Article/details/gaumlovug.sHtML

[T20] Swift：数组操作
来源：http://read.share.yfazqb.com/Article/details/ggnwfsslo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fktsv.cn/Article/details/gdcatptnt.sHtML

[T21] Swift：遍历
来源：http://www.share.tarul.cn/Article/details/guohyhwpd.sHtML

for x in a { print(x) }
来源：http://3g.epnwcf.com/Article/details/gjacoyoaf.sHtML

[T22] Swift：字典
来源：http://www.blog.tarul.cn/Article/details/gbozvvoga.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.tarul.cn/Article/details/gslccdgsk.sHtML

[T23] Swift：函数
来源：http://www.blog.bbcook.cn/Article/details/gsbwtvwor.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fktsv.cn/Article/details/gadznqlro.sHtML

[T24] Swift：闭包
来源：http://read.share.vehdjk.com/Article/details/gdocrlcgc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gprmzdxpk.sHtML

[T25] Swift：结构体
来源：http://m.share.vehdjk.com/Article/details/gvtmdwire.sHtML

struct P { var x: Int }
来源：http://www.share.sjlbkw.cn/Article/details/gzmtoyjto.sHtML

[T26] Swift：类与重写
来源：http://blog.yfazqb.com/Article/details/gcixyitxy.sHtML

class A: Base { override func f() {} }
来源：http://wap.fktsv.cn/Article/details/gmzhnvvps.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.vehdjk.com/Article/details/gmrpjwedv.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcmjhrdu.sHtML

[T28] Swift：枚举
来源：http://www.share.yfazqb.com/Article/details/gvuwqbbrz.sHtML

enum Color { case red, green }
来源：http://3g.bbcook.cn/Article/details/gtyhtpyyq.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.bbcook.cn/Article/details/gylstxxks.sHtML

guard let x = opt else { return }
来源：http://baike.fktsv.cn/Article/details/gmqefyhpm.sHtML

[T30] Swift：协议
来源：http://3g.vehdjk.com/Article/details/glvoaypth.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fktsv.cn/Article/details/gaxebiujq.sHtML

[T31] Lua：Hello World
来源：http://blog.yfazqb.com/Article/details/gbfvisyhu.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gefmrfyke.sHtML

[T32] Lua：局部变量
来源：http://wap.bbcook.cn/Article/details/garnqnphl.sHtML

local a = 1
来源：http://read.share.tarul.cn/Article/details/gebbcxmlq.sHtML

[T33] Lua：表（数组）
来源：http://wap.vehdjk.com/Article/details/glqtlvtlj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.vehdjk.com/Article/details/gudrrxzfo.sHtML

[T34] Lua：遍历表
来源：http://www.blog.tarul.cn/Article/details/gyqtqarlh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.epnwcf.com/Article/details/ghssxkzth.sHtML

[T35] Lua：字典表
来源：http://www.blog.tarul.cn/Article/details/gklirrxhq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.sjlbkw.cn/Article/details/gbtsnvljr.sHtML

[T36] Lua：函数
来源：http://www.m.share.fktsv.cn/Article/details/gzfplkero.sHtML

function add(a, b) return a + b end
来源：http://www.share.sjlbkw.cn/Article/details/gqrwlsgnk.sHtML

[T37] Lua：字符串拼接
来源：http://3g.tarul.cn/Article/details/ggdklulrz.sHtML

"a" .. "b"
来源：http://read.share.bbcook.cn/Article/details/gkpmisnby.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/gislbnirr.sHtML

if x > 0 then print("正") end
来源：http://wap.vehdjk.com/Article/details/gscqobpph.sHtML

[T39] Lua：模式匹配
来源：http://www.share.tarul.cn/Article/details/ghixtktje.sHtML

string.find(s, "%d+")
来源：http://m.share.tarul.cn/Article/details/gtmhrxzdc.sHtML

[T40] Lua：元表
来源：http://www.m.share.bbcook.cn/Article/details/gwbwoqzgy.sHtML

setmetatable({}, { __index = base })
来源：http://baike.epnwcf.com/Article/details/guuzgwjoy.sHtML

[T41] Perl：Hello World
来源：http://3g.yfazqb.com/Article/details/gcepjnmhc.sHtML

print "Hello\n";
来源：http://blog.yfazqb.com/Article/details/geixlomhf.sHtML

[T42] Perl：变量类型
来源：http://read.share.bbcook.cn/Article/details/gpqbrzeea.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.tarul.cn/Article/details/ggngzmner.sHtML

[T43] Perl：字符串插值
来源：http://wap.epnwcf.com/Article/details/gbnaxdoaj.sHtML

"值: $a"
来源：http://baike.vehdjk.com/Article/details/ggvnzsywm.sHtML

[T44] Perl：条件
来源：http://m.share.fktsv.cn/Article/details/gldtpbubg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.epnwcf.com/Article/details/glgcnephz.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.tarul.cn/Article/details/gquiokbne.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.bbcook.cn/Article/details/glmdiajwe.sHtML

[T46] Perl：哈希操作
来源：http://read.share.epnwcf.com/Article/details/gciiwpkjn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.vehdjk.com/Article/details/gtxodvpay.sHtML

[T47] Perl：正则捕获
来源：http://www.share.epnwcf.com/Article/details/gqbvivhrn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fktsv.cn/Article/details/ghffkasxw.sHtML

[T48] Perl：正则替换
来源：http://m.share.sjlbkw.cn/Article/details/gldbpiyvx.sHtML

$s =~ s/old/new/g;
来源：http://m.share.bbcook.cn/Article/details/glukmlhpd.sHtML

[T49] Perl：函数
来源：http://wap.fktsv.cn/Article/details/gkcbustya.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gttdgehya.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gtnijhkad.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.epnwcf.com/Article/details/gziwfvgfs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.tarul.cn/Article/details/gxwcbltlz.sHtML

[T51] Scala：Hello World
来源：http://wap.tarul.cn/Article/details/gwkprcujx.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/ggxwykgxu.sHtML

[T52] Scala：变量
来源：http://baike.bbcook.cn/Article/details/gclsuprud.sHtML

val a = 1;  var b = 2
来源：http://baike.bbcook.cn/Article/details/giylsexfa.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gabtxyvrn.sHtML

s"值: $b"
来源：http://baike.yfazqb.com/Article/details/gkjqiehwv.sHtML

[T54] Scala：集合映射
来源：http://blog.bbcook.cn/Article/details/gjuyoelap.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.vehdjk.com/Article/details/gcijihupc.sHtML

[T55] Scala：集合过滤
来源：http://read.share.epnwcf.com/Article/details/guurzisnp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.epnwcf.com/Article/details/guuhllfmp.sHtML

[T56] Scala：样例类
来源：http://www.m.share.bbcook.cn/Article/details/gtjxynsfw.sHtML

case class User(name: String, age: Int)
来源：http://3g.yfazqb.com/Article/details/guasjcmij.sHtML

[T57] Scala：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gpcbiqrut.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.bbcook.cn/Article/details/ghzjmwynm.sHtML

[T58] Scala：函数定义
来源：http://m.share.bbcook.cn/Article/details/gvzpaxxwz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.bbcook.cn/Article/details/gywarbhct.sHtML

[T59] Scala：循环
来源：http://baike.yfazqb.com/Article/details/gckdqyuij.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gvxmuhqgh.sHtML

[T60] Scala：折叠
来源：http://read.share.yfazqb.com/Article/details/grclwddbe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.bbcook.cn/Article/details/gfqzgojno.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/guiftdxlh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.epnwcf.com/Article/details/gruzuunpv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gdldxjxbz.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.sjlbkw.cn/Article/details/giptyfoub.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fktsv.cn/Article/details/gdvkldqfl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fktsv.cn/Article/details/gkeiefmev.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.tarul.cn/Article/details/glaegxnzj.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fktsv.cn/Article/details/gdxcosozs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fktsv.cn/Article/details/gmrmuscpd.sHtML

[U04] Py：变量调试打印
来源：http://blog.yfazqb.com/Article/details/gpomdabqr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/gtnanetjr.sHtML

[U05] Py：列表去重且保序
来源：http://3g.yfazqb.com/Article/details/gybsqpuxm.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.bbcook.cn/Article/details/gtenmnuir.sHtML

[U06] Py：合并两个字典
来源：http://m.share.yfazqb.com/Article/details/gqasikhgu.sHtML

{**a, **b}
来源：http://3g.vehdjk.com/Article/details/gczfwowag.sHtML

[U07] Py：反转字典键值
来源：http://wap.yfazqb.com/Article/details/ghzicplfm.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/gyibeghzq.sHtML

[U08] Py：展平二维列表
来源：http://3g.fktsv.cn/Article/details/gpiaqlztt.sHtML

[y for x in nested for y in x]
来源：http://m.share.tarul.cn/Article/details/gshvbpgba.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.bbcook.cn/Article/details/ghrykohrk.sHtML

max(d, key=d.get)
来源：http://www.m.share.fktsv.cn/Article/details/gxtebxoyg.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gzncjwvvl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.yfazqb.com/Article/details/goutoujqt.sHtML

[U11] Py：生成器表达式
来源：http://wap.tarul.cn/Article/details/gjlwsddmc.sHtML

(x * 2 for x in arr)
来源：http://read.share.epnwcf.com/Article/details/ggiuslzfl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.sjlbkw.cn/Article/details/ggbzdyclm.sHtML

Counter(arr).most_common(3)
来源：http://m.share.tarul.cn/Article/details/gbqhwimed.sHtML


<!-- 参考信息 -->