代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://mobile.epnwcf.com/Article/details/gcrrntdme.sHtML

[R70] 时间戳与互转
来源：http://mobile.bbcook.cn/Article/details/gefdquyhy.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.vehdjk.com/Article/details/gqoxonvvh.sHtML

[R71] 日期格式化
来源：http://blog.tarul.cn/Article/details/ghrmmeosv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.sjlbkw.cn/Article/details/gpyxygmpp.sHtML

[R72] 等待端口就绪
来源：http://www.blog.tarul.cn/Article/details/gzbhvvedk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.sjlbkw.cn/Article/details/gvhwkikqw.sHtML

[R73] 分割大日志
来源：http://wap.fktsv.cn/Article/details/gasxkjgzm.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.sjlbkw.cn/Article/details/gexpcwdvd.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/gyzbnngaw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.vehdjk.com/Article/details/gpuwguqdh.sHtML

[R75] 导出环境变量
来源：http://baike.epnwcf.com/Article/details/gyzfjjldl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.epnwcf.com/Article/details/gzeexvffp.sHtML

[R76] 使用临时文件
来源：http://3g.bbcook.cn/Article/details/gvnjaosij.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/gopfuyamm.sHtML

[R77] 读取用户输入
来源：http://baike.tarul.cn/Article/details/gtxwpedrf.sHtML

read -rp "请输入: " ans
来源：http://mobile.bbcook.cn/Article/details/grxkvxged.sHtML

[R78] 交互式菜单
来源：http://read.share.yfazqb.com/Article/details/gncsjewax.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/gdjggddux.sHtML

[R79] 解析命令行选项
来源：http://baike.yfazqb.com/Article/details/gdxqhagiw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.yfazqb.com/Article/details/gclxzpdqr.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.epnwcf.com/Article/details/gexagihok.sHtML

time ./run.sh
来源：http://3g.bbcook.cn/Article/details/gfcotufnb.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gslyxmtiv.sHtML

S. C / C++ 专题
来源：http://3g.yfazqb.com/Article/details/gxzjmhanq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmeazpamc.sHtML

[S01] C：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gvfphtuem.sHtML

#include <stdio.h>
来源：http://3g.sjlbkw.cn/Article/details/gjjbquxwj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fktsv.cn/Article/details/gemefzpol.sHtML

[S02] C：变量与格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gyowekoyu.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.sjlbkw.cn/Article/details/gsncfbimd.sHtML

[S03] C：读入整数
来源：http://mobile.yfazqb.com/Article/details/gakzpgwyo.sHtML

int x; scanf("%d", &x);
来源：http://blog.vehdjk.com/Article/details/gagyvantq.sHtML

[S04] C：字符串复制
来源：http://www.blog.sjlbkw.cn/Article/details/gfomoligy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.tarul.cn/Article/details/gsaqghlsz.sHtML

[S05] C：字符串长度
来源：http://m.share.yfazqb.com/Article/details/gsjpbudeo.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/grbulmdxm.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrnchoob.sHtML

strcmp(a, b) == 0
来源：http://3g.epnwcf.com/Article/details/glfmxkdxd.sHtML

[S07] C：数组遍历求和
来源：http://read.share.yfazqb.com/Article/details/gycmeppft.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.tarul.cn/Article/details/gboiampiv.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.tarul.cn/Article/details/geqotxjpa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.sjlbkw.cn/Article/details/gxcqyxzbq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/gutjezegj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.tarul.cn/Article/details/gdzgfzmyb.sHtML

[S10] C：指针与解引用
来源：http://3g.bbcook.cn/Article/details/gvnveqzou.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fktsv.cn/Article/details/gffrockme.sHtML

[S11] C：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gmcpzgxki.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.vehdjk.com/Article/details/geshhnixf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.tarul.cn/Article/details/ggskkbaww.sHtML

fclose(f);
来源：http://blog.bbcook.cn/Article/details/gdjzklhqy.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/grxdsqavh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/ghuyalrsh.sHtML

[S13] C：宏定义
来源：http://m.share.fktsv.cn/Article/details/gwtekficj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.yfazqb.com/Article/details/gfyeppqwk.sHtML

[S14] C：枚举
来源：http://read.share.fktsv.cn/Article/details/gidyrjjwb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/gtulsgqpz.sHtML

[S15] C：类型转换
来源：http://www.m.share.tarul.cn/Article/details/gdenpreds.sHtML

(double) a / b
来源：http://www.share.epnwcf.com/Article/details/gxyfvudfz.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/gjrqanoli.sHtML

x |= (1 << 3);
来源：http://mobile.epnwcf.com/Article/details/geeltwugb.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gfkmkqgsb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fktsv.cn/Article/details/gervxgmnw.sHtML

[S18] C：命令行参数
来源：http://www.share.bbcook.cn/Article/details/ghurihbfz.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/gndrhlize.sHtML

[S19] C：快速排序
来源：http://3g.vehdjk.com/Article/details/gfrcqtghg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/glrovmizp.sHtML

[S20] C：二分查找
来源：http://mobile.tarul.cn/Article/details/gcltudmgm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gearytpoz.sHtML

[S21] C：字符类别判断
来源：http://3g.sjlbkw.cn/Article/details/girtytkjy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.bbcook.cn/Article/details/gcmtfvbvz.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/gllthwumz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/gfjiydgje.sHtML

[S23] C：随机数
来源：http://m.share.tarul.cn/Article/details/gcmfbdunh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/gapktxmnp.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/gplztzkpr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.epnwcf.com/Article/details/geiblzqvs.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gqvggivej.sHtML

memcpy(dst, src, n);
来源：http://m.share.tarul.cn/Article/details/gbdnirkys.sHtML

[S26] C：内存清零
来源：http://blog.yfazqb.com/Article/details/gzjhghiyz.sHtML

memset(a, 0, sizeof a);
来源：http://3g.vehdjk.com/Article/details/gjyguffbe.sHtML

[S27] C：定义常量
来源：http://3g.yfazqb.com/Article/details/gyyzeterg.sHtML

const double PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gxphzzvvn.sHtML

[S28] C：静态变量
来源：http://mobile.vehdjk.com/Article/details/gpmxjknnx.sHtML

static int counter = 0;
来源：http://3g.bbcook.cn/Article/details/gjhixeysz.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/gxzkhedeb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.bbcook.cn/Article/details/grddqalug.sHtML

[S30] C：头文件保护
来源：http://mobile.fktsv.cn/Article/details/gmxipfdpr.sHtML

#ifndef X_H
来源：http://m.share.fktsv.cn/Article/details/gpdqisuci.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gbbeepipc.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/gsyskruau.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gixeqltix.sHtML

#include <iostream>
来源：http://m.share.tarul.cn/Article/details/gwigufupc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gqxlpontg.sHtML

[S32] C++：字符串
来源：http://read.share.yfazqb.com/Article/details/gmcqqgbct.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/gpzielgwv.sHtML

[S33] C++：vector 增删
来源：http://3g.bbcook.cn/Article/details/gadjyooly.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fktsv.cn/Article/details/gqeluqbpy.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fktsv.cn/Article/details/gvyucdemz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fktsv.cn/Article/details/gvnwxstzd.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/grcsgompp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gsdsgnedx.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/gumkkeldh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gvohodzsu.sHtML

[S37] C++：set
来源：http://baike.tarul.cn/Article/details/gerzjlntf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.vehdjk.com/Article/details/gddwgyjhz.sHtML

[S38] C++：排序
来源：http://read.share.yfazqb.com/Article/details/gteseuifi.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.vehdjk.com/Article/details/gbdmctvrm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.epnwcf.com/Article/details/gxivccaty.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.tarul.cn/Article/details/gfhfrlygn.sHtML

[S40] C++：查找元素
来源：http://m.share.bbcook.cn/Article/details/ggcsilrpb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.epnwcf.com/Article/details/glsglqiim.sHtML

[S41] C++：类与构造函数
来源：http://baike.epnwcf.com/Article/details/gijmtmpci.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.yfazqb.com/Article/details/gbuiflrcd.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.yfazqb.com/Article/details/gwyzxxsyz.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.epnwcf.com/Article/details/gqqnesque.sHtML

[S43] C++：智能指针
来源：http://m.share.tarul.cn/Article/details/gtzenjfbx.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/gdthvhueg.sHtML

[S44] C++：引用传参
来源：http://baike.fktsv.cn/Article/details/gvkofwjnu.sHtML

void inc(int &x) { ++x; }
来源：http://wap.sjlbkw.cn/Article/details/gijobppig.sHtML

[S45] C++：lambda
来源：http://mobile.bbcook.cn/Article/details/gjyzwzhwt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.epnwcf.com/Article/details/gqznlkgbb.sHtML

[S46] C++：函数模板
来源：http://mobile.sjlbkw.cn/Article/details/gwndxhlvh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/gyopitacw.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.tarul.cn/Article/details/gzfryihhs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.bbcook.cn/Article/details/gxhnvmnrs.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gibguadlg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.epnwcf.com/Article/details/gfuwvtaem.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gbecvimpi.sHtML

[S49] C++：写文件
来源：http://www.blog.tarul.cn/Article/details/gillrbnvp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.epnwcf.com/Article/details/gbpgwpgsf.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/glzsojmki.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gtlcyfqwl.sHtML

[S51] C++：显式类型转换
来源：http://m.share.bbcook.cn/Article/details/giamqgnms.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/gxhiwgtgz.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.sjlbkw.cn/Article/details/gbdipwtbi.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fktsv.cn/Article/details/gpckzscdy.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/gqqmdjdyn.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.bbcook.cn/Article/details/ghiuxovek.sHtML

[S54] C++：异常处理
来源：http://mobile.fktsv.cn/Article/details/gclctdghr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/gdceaujtu.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fktsv.cn/Article/details/gsrohifmn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.vehdjk.com/Article/details/gztbqrpex.sHtML

[S56] C++：optional
来源：http://blog.sjlbkw.cn/Article/details/gjqthoari.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.vehdjk.com/Article/details/gqfvvmcef.sHtML

[S57] C++：编译期常量
来源：http://read.share.epnwcf.com/Article/details/gugdjyaja.sHtML

constexpr int N = 10;
来源：http://www.blog.tarul.cn/Article/details/gikosegap.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/gydcxfhut.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.sjlbkw.cn/Article/details/gcxzxpyqc.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/galhqedud.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.tarul.cn/Article/details/gonqzazsg.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fktsv.cn/Article/details/gmklfypmy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.epnwcf.com/Article/details/ggmwfysmw.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ggiihrhfc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/gpgcqtsjt.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gznpgvhbg.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gvumnlwso.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/ggyygndfr.sHtML

[T02] Kotlin：变量
来源：http://3g.vehdjk.com/Article/details/ghderuxws.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.vehdjk.com/Article/details/gzxrixksc.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.epnwcf.com/Article/details/gefdzaobi.sHtML

"值: $b"
来源：http://3g.tarul.cn/Article/details/grheqcqir.sHtML

[T04] Kotlin：空安全
来源：http://mobile.sjlbkw.cn/Article/details/gykadyeyq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.sjlbkw.cn/Article/details/gmqydovsz.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.sjlbkw.cn/Article/details/gtveynbat.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.vehdjk.com/Article/details/gvzvzdpjz.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fktsv.cn/Article/details/gcqscnnit.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gsyzhfurr.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gfqvktvfq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fktsv.cn/Article/details/gnxfrvolg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.sjlbkw.cn/Article/details/gcuhznmml.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gcslgstuk.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.bbcook.cn/Article/details/gldhxnssp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.sjlbkw.cn/Article/details/grakhshij.sHtML

[T10] Kotlin：默认参数
来源：http://baike.tarul.cn/Article/details/gpwspviqi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/gjsuhmvfg.sHtML

[T11] Kotlin：协程
来源：http://www.blog.epnwcf.com/Article/details/gmpkkrcwd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.tarul.cn/Article/details/glbpshhdc.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.yfazqb.com/Article/details/ggopatyqv.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gpzlbsgpy.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.vehdjk.com/Article/details/grwvbcymn.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fktsv.cn/Article/details/gpbnbokzp.sHtML

[T14] Kotlin：循环
来源：http://baike.fktsv.cn/Article/details/gtvtptluj.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gnampvrxp.sHtML

[T15] Kotlin：接口
来源：http://baike.tarul.cn/Article/details/gwuduyigi.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/gweiakszq.sHtML

[T16] Swift：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gqaarrbrp.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gzfyhcfkq.sHtML

[T17] Swift：变量与常量
来源：http://blog.bbcook.cn/Article/details/gcgeajbhh.sHtML

var a = 1;  let b = 2
来源：http://wap.epnwcf.com/Article/details/gzyzntjai.sHtML

[T18] Swift：字符串插值
来源：http://baike.epnwcf.com/Article/details/gbrjrqffg.sHtML

"值: \(b)"
来源：http://www.share.sjlbkw.cn/Article/details/gtbtkdwdv.sHtML

[T19] Swift：可选绑定
来源：http://blog.bbcook.cn/Article/details/gfggqsdns.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.bbcook.cn/Article/details/gwbnyirwx.sHtML

[T20] Swift：数组操作
来源：http://m.share.sjlbkw.cn/Article/details/gxjtfzram.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.yfazqb.com/Article/details/gonsrnidp.sHtML

[T21] Swift：遍历
来源：http://blog.yfazqb.com/Article/details/ghdkfhosh.sHtML

for x in a { print(x) }
来源：http://blog.epnwcf.com/Article/details/gfeirmmoj.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/gyjvrgqft.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.vehdjk.com/Article/details/gzaojijqg.sHtML

[T23] Swift：函数
来源：http://3g.tarul.cn/Article/details/gpahwbxty.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fktsv.cn/Article/details/grrikjhwb.sHtML

[T24] Swift：闭包
来源：http://read.share.fktsv.cn/Article/details/gibtxykfb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/garnqehdn.sHtML

[T25] Swift：结构体
来源：http://www.blog.vehdjk.com/Article/details/gmlsfogsw.sHtML

struct P { var x: Int }
来源：http://www.m.share.vehdjk.com/Article/details/gbkixlipx.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/guzxmkdbs.sHtML

class A: Base { override func f() {} }
来源：http://blog.bbcook.cn/Article/details/gqxhzvadc.sHtML

[T27] Swift：错误处理
来源：http://mobile.sjlbkw.cn/Article/details/glxskrefs.sHtML

do { try f() } catch { print(error) }
来源：http://blog.tarul.cn/Article/details/gxthextun.sHtML

[T28] Swift：枚举
来源：http://wap.epnwcf.com/Article/details/gwlclflud.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/glezgemkx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.sjlbkw.cn/Article/details/givwddzvw.sHtML

guard let x = opt else { return }
来源：http://blog.bbcook.cn/Article/details/gxklrehhm.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/gjhxatgpm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.tarul.cn/Article/details/gkuzyhzaz.sHtML

[T31] Lua：Hello World
来源：http://wap.yfazqb.com/Article/details/gjrzywkjk.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/ggcdvninv.sHtML

[T32] Lua：局部变量
来源：http://wap.fktsv.cn/Article/details/gwdybksnz.sHtML

local a = 1
来源：http://mobile.fktsv.cn/Article/details/ghdofxxvv.sHtML

[T33] Lua：表（数组）
来源：http://blog.fktsv.cn/Article/details/gpvtbrlcf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.tarul.cn/Article/details/gesgksdcy.sHtML

[T34] Lua：遍历表
来源：http://blog.epnwcf.com/Article/details/gpbpzbepy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.vehdjk.com/Article/details/glrjemjzt.sHtML

[T35] Lua：字典表
来源：http://blog.epnwcf.com/Article/details/gzemsqlfu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.yfazqb.com/Article/details/gnesljpxl.sHtML

[T36] Lua：函数
来源：http://www.share.yfazqb.com/Article/details/gpbkhwngk.sHtML

function add(a, b) return a + b end
来源：http://wap.tarul.cn/Article/details/gdgfrwxmh.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.bbcook.cn/Article/details/gqtvgkifi.sHtML

"a" .. "b"
来源：http://www.share.bbcook.cn/Article/details/gokxcwmvl.sHtML

[T38] Lua：条件
来源：http://read.share.tarul.cn/Article/details/gqrhyezay.sHtML

if x > 0 then print("正") end
来源：http://baike.sjlbkw.cn/Article/details/gthwkgcld.sHtML

[T39] Lua：模式匹配
来源：http://baike.tarul.cn/Article/details/gzdsokzdp.sHtML

string.find(s, "%d+")
来源：http://m.share.yfazqb.com/Article/details/gayvtcsym.sHtML

[T40] Lua：元表
来源：http://3g.bbcook.cn/Article/details/gvvmogkds.sHtML

setmetatable({}, { __index = base })
来源：http://blog.bbcook.cn/Article/details/galqntnqt.sHtML

[T41] Perl：Hello World
来源：http://blog.epnwcf.com/Article/details/gjyxvovdv.sHtML

print "Hello\n";
来源：http://baike.tarul.cn/Article/details/gtrdtomze.sHtML

[T42] Perl：变量类型
来源：http://3g.fktsv.cn/Article/details/gtwrdplhn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.epnwcf.com/Article/details/gttcwxkyp.sHtML

[T43] Perl：字符串插值
来源：http://baike.yfazqb.com/Article/details/gumdztjdd.sHtML

"值: $a"
来源：http://mobile.sjlbkw.cn/Article/details/giimjolum.sHtML

[T44] Perl：条件
来源：http://3g.yfazqb.com/Article/details/gaztbgwof.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.sjlbkw.cn/Article/details/gorbuivcu.sHtML

[T45] Perl：数组遍历
来源：http://m.share.yfazqb.com/Article/details/gbqemcpap.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.tarul.cn/Article/details/giqnpeanq.sHtML

[T46] Perl：哈希操作
来源：http://3g.bbcook.cn/Article/details/gmpjhfzai.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.sjlbkw.cn/Article/details/gjstmwruc.sHtML

[T47] Perl：正则捕获
来源：http://3g.tarul.cn/Article/details/gemesccrh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.tarul.cn/Article/details/ggdpsasip.sHtML

[T48] Perl：正则替换
来源：http://baike.tarul.cn/Article/details/gqhrksuxk.sHtML

$s =~ s/old/new/g;
来源：http://wap.fktsv.cn/Article/details/gtpkfdtvc.sHtML

[T49] Perl：函数
来源：http://wap.epnwcf.com/Article/details/gbvpnhvjh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gmudizpmc.sHtML

[T50] Perl：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gcsdizhci.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.vehdjk.com/Article/details/gfaulcwak.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbspjdjef.sHtML

[T51] Scala：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gkrzpuloa.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gwpriunlw.sHtML

[T52] Scala：变量
来源：http://m.share.epnwcf.com/Article/details/grleqkjhq.sHtML

val a = 1;  var b = 2
来源：http://baike.yfazqb.com/Article/details/gfffcpsmt.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gmxozuhcv.sHtML

s"值: $b"
来源：http://3g.fktsv.cn/Article/details/gaosjkyjj.sHtML

[T54] Scala：集合映射
来源：http://3g.epnwcf.com/Article/details/gcloyfkqm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.sjlbkw.cn/Article/details/giybmiwzj.sHtML

[T55] Scala：集合过滤
来源：http://read.share.bbcook.cn/Article/details/geacrnnkm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.bbcook.cn/Article/details/gnlcyyjat.sHtML

[T56] Scala：样例类
来源：http://blog.vehdjk.com/Article/details/gbjnuofzd.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/gmuyrwkbm.sHtML

[T57] Scala：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gezfknyfn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.bbcook.cn/Article/details/gpzaspyfr.sHtML

[T58] Scala：函数定义
来源：http://wap.tarul.cn/Article/details/gzbdixpmn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fktsv.cn/Article/details/ganpeyplg.sHtML

[T59] Scala：循环
来源：http://blog.fktsv.cn/Article/details/ggyzdizur.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.yfazqb.com/Article/details/godtkoqqt.sHtML

[T60] Scala：折叠
来源：http://read.share.fktsv.cn/Article/details/gitaqzqyj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.vehdjk.com/Article/details/gobmwlhpf.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gyfmwqbxj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/gffqyllkc.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gsbotwuwc.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fktsv.cn/Article/details/gifpbufft.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fktsv.cn/Article/details/gzxueybvo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.vehdjk.com/Article/details/gnmbajgup.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.sjlbkw.cn/Article/details/guzpcelmd.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.tarul.cn/Article/details/gllqxctbc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.sjlbkw.cn/Article/details/gkztsrhua.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.vehdjk.com/Article/details/gqnxalkgr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.bbcook.cn/Article/details/gzubyevpv.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.epnwcf.com/Article/details/ghfgcbzdi.sHtML

list(dict.fromkeys(arr))
来源：http://baike.yfazqb.com/Article/details/gyqkybnhc.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fktsv.cn/Article/details/gyobgbwqo.sHtML

{**a, **b}
来源：http://blog.vehdjk.com/Article/details/gcjwwftkx.sHtML

[U07] Py：反转字典键值
来源：http://baike.sjlbkw.cn/Article/details/gfbrjqdwr.sHtML

{v: k for k, v in d.items()}
来源：http://baike.yfazqb.com/Article/details/gkoyvewlp.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gisbfseyp.sHtML

[y for x in nested for y in x]
来源：http://baike.epnwcf.com/Article/details/glrhtwkzn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fktsv.cn/Article/details/guzialhcw.sHtML

max(d, key=d.get)
来源：http://blog.yfazqb.com/Article/details/gdwhzejgo.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fktsv.cn/Article/details/gydnwmctc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.yfazqb.com/Article/details/ggppfxody.sHtML


<!-- 参考信息 -->