代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://m.share.epnwcf.com/Article/details/ghtbypehy.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/gfacbqsso.sHtML

date +%s;  date -d @1700000000
来源：http://3g.bbcook.cn/Article/details/gzuejaiet.sHtML

[R71] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/glubiwxik.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/gtzgtdjda.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/gqasbqbdr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/gcxcwhyys.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/gjvpnndnl.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/gcinluxvw.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/garbhmmtg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.sjlbkw.cn/Article/details/gfiqmyupm.sHtML

[R75] 导出环境变量
来源：http://www.blog.fktsv.cn/Article/details/gtzrqhppn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.epnwcf.com/Article/details/gaeslndlq.sHtML

[R76] 使用临时文件
来源：http://www.blog.yfazqb.com/Article/details/gvlddytnn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gvfehvqdo.sHtML

[R77] 读取用户输入
来源：http://baike.epnwcf.com/Article/details/gqnfazpmw.sHtML

read -rp "请输入: " ans
来源：http://blog.epnwcf.com/Article/details/gkiajbvjw.sHtML

[R78] 交互式菜单
来源：http://blog.sjlbkw.cn/Article/details/ggmxblrsl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpewyspk.sHtML

[R79] 解析命令行选项
来源：http://blog.epnwcf.com/Article/details/gdzhzgrnc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.sjlbkw.cn/Article/details/gifkncjhr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.yfazqb.com/Article/details/gwhcopbfr.sHtML

time ./run.sh
来源：http://read.share.vehdjk.com/Article/details/geqwbkpjd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnglwmbom.sHtML

S. C / C++ 专题
来源：http://m.share.sjlbkw.cn/Article/details/gaqjygpir.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gadvxpjuf.sHtML

[S01] C：Hello World
来源：http://mobile.bbcook.cn/Article/details/gnamkomzh.sHtML

#include <stdio.h>
来源：http://www.blog.bbcook.cn/Article/details/gcdnkqvvw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.epnwcf.com/Article/details/gxsldalhv.sHtML

[S02] C：变量与格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gezwprdtw.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.bbcook.cn/Article/details/gfklsvfmk.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/gmdjfqxkw.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/gudrsxfaw.sHtML

[S04] C：字符串复制
来源：http://3g.sjlbkw.cn/Article/details/ghihjxhvx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.tarul.cn/Article/details/goroimyjv.sHtML

[S05] C：字符串长度
来源：http://wap.bbcook.cn/Article/details/gabdrvtzn.sHtML

strlen(s)
来源：http://mobile.tarul.cn/Article/details/gqeidopos.sHtML

[S06] C：字符串比较
来源：http://m.share.fktsv.cn/Article/details/gfclyknut.sHtML

strcmp(a, b) == 0
来源：http://mobile.sjlbkw.cn/Article/details/ghdbqyniv.sHtML

[S07] C：数组遍历求和
来源：http://www.share.bbcook.cn/Article/details/grrrstytl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.tarul.cn/Article/details/gryoydxvx.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.bbcook.cn/Article/details/gfmwxersm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.epnwcf.com/Article/details/gozxlovbb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.sjlbkw.cn/Article/details/gjmnpbbvc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/glejpdzjt.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/ggckzqvhk.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fktsv.cn/Article/details/gczhlrwga.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gmlcocdaw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.sjlbkw.cn/Article/details/glnzwyqlh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gtqxydvua.sHtML

fclose(f);
来源：http://m.share.epnwcf.com/Article/details/gnrjopurr.sHtML

[S12] C：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gwstugwge.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gmudqfwsf.sHtML

[S13] C：宏定义
来源：http://m.share.fktsv.cn/Article/details/ggpvjbnvy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.bbcook.cn/Article/details/gydnsfjma.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/genqwwjsj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/gwemlnlrb.sHtML

[S15] C：类型转换
来源：http://read.share.epnwcf.com/Article/details/gnbsxyisa.sHtML

(double) a / b
来源：http://3g.bbcook.cn/Article/details/gjajuipmp.sHtML

[S16] C：位操作置位
来源：http://3g.tarul.cn/Article/details/ghmkhcnwj.sHtML

x |= (1 << 3);
来源：http://baike.tarul.cn/Article/details/gxpwtiakr.sHtML

[S17] C：安全拼接字符串
来源：http://blog.tarul.cn/Article/details/guaowmawd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fktsv.cn/Article/details/gfbmxruqi.sHtML

[S18] C：命令行参数
来源：http://baike.fktsv.cn/Article/details/gzrpttuzi.sHtML

int main(int argc, char **argv)
来源：http://m.share.vehdjk.com/Article/details/gdipuisod.sHtML

[S19] C：快速排序
来源：http://blog.epnwcf.com/Article/details/gvifgwhny.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gcaxorkbv.sHtML

[S20] C：二分查找
来源：http://3g.bbcook.cn/Article/details/gxohokfxj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gbtfrocbw.sHtML

[S21] C：字符类别判断
来源：http://blog.epnwcf.com/Article/details/gbgstktub.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/grigdezew.sHtML

[S22] C：字符串转数字
来源：http://m.share.epnwcf.com/Article/details/gksorhybg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.vehdjk.com/Article/details/giiamduvy.sHtML

[S23] C：随机数
来源：http://read.share.tarul.cn/Article/details/gxgcqbwle.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.yfazqb.com/Article/details/ghcxlisdb.sHtML

[S24] C：获取本地时间
来源：http://blog.tarul.cn/Article/details/gsikkjulc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.yfazqb.com/Article/details/gccbydwhg.sHtML

[S25] C：内存拷贝
来源：http://www.share.yfazqb.com/Article/details/gyslxsjaz.sHtML

memcpy(dst, src, n);
来源：http://mobile.epnwcf.com/Article/details/gdimvqicm.sHtML

[S26] C：内存清零
来源：http://wap.tarul.cn/Article/details/gjhvfkene.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/gtwhcavwk.sHtML

[S27] C：定义常量
来源：http://blog.vehdjk.com/Article/details/gjmqaoaua.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gfbkkqupl.sHtML

[S28] C：静态变量
来源：http://m.share.bbcook.cn/Article/details/gjdyvacrn.sHtML

static int counter = 0;
来源：http://www.blog.tarul.cn/Article/details/gwjcpwtfk.sHtML

[S29] C：变参函数
来源：http://www.share.fktsv.cn/Article/details/gqoivmxyn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.epnwcf.com/Article/details/gyowcqeja.sHtML

[S30] C：头文件保护
来源：http://www.share.tarul.cn/Article/details/gwqsiyipx.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gpknnfwdg.sHtML

#define X_H
来源：http://baike.vehdjk.com/Article/details/gexuxcuhf.sHtML

#endif
来源：http://baike.fktsv.cn/Article/details/gswaghfrh.sHtML

[S31] C++：Hello World
来源：http://wap.fktsv.cn/Article/details/glmpexafm.sHtML

#include <iostream>
来源：http://www.share.yfazqb.com/Article/details/glwhcglmd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.bbcook.cn/Article/details/gllmatcyt.sHtML

[S32] C++：字符串
来源：http://read.share.sjlbkw.cn/Article/details/glclisrju.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.sjlbkw.cn/Article/details/gbfwbymhj.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/galrhdubz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.vehdjk.com/Article/details/gktnhzqrv.sHtML

[S34] C++：遍历 vector
来源：http://mobile.yfazqb.com/Article/details/gzmyehsfv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fktsv.cn/Article/details/gvpmphpge.sHtML

[S35] C++：map
来源：http://blog.sjlbkw.cn/Article/details/gafhqsorb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/grobxgeuf.sHtML

[S36] C++：unordered_map
来源：http://blog.bbcook.cn/Article/details/gqqbliptp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gddgsiooq.sHtML

[S37] C++：set
来源：http://3g.epnwcf.com/Article/details/gjzblgsar.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.bbcook.cn/Article/details/gfazenysw.sHtML

[S38] C++：排序
来源：http://blog.bbcook.cn/Article/details/gwzwzcpjk.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.vehdjk.com/Article/details/gmpjxoyad.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.epnwcf.com/Article/details/gawrlquuu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.yfazqb.com/Article/details/guppfvazu.sHtML

[S40] C++：查找元素
来源：http://m.share.bbcook.cn/Article/details/gnuwwsgmv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.vehdjk.com/Article/details/gqjgvefxi.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gucpmqhvh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.epnwcf.com/Article/details/gdtgiiaav.sHtML

[S42] C++：继承与虚函数
来源：http://3g.sjlbkw.cn/Article/details/gzpnqwahd.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/gcvxlwrfp.sHtML

[S43] C++：智能指针
来源：http://m.share.tarul.cn/Article/details/gzkgbkosn.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.epnwcf.com/Article/details/gjjhcybqy.sHtML

[S44] C++：引用传参
来源：http://wap.yfazqb.com/Article/details/geobpnhen.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.bbcook.cn/Article/details/gulitoabs.sHtML

[S45] C++：lambda
来源：http://www.share.fktsv.cn/Article/details/gadfqvudy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.vehdjk.com/Article/details/ggwzgqxae.sHtML

[S46] C++：函数模板
来源：http://read.share.fktsv.cn/Article/details/gvkahvlqt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fktsv.cn/Article/details/gwuyymedl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.yfazqb.com/Article/details/gasrdkedb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.epnwcf.com/Article/details/ggvifswsg.sHtML

[S48] C++：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gquggbksk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.sjlbkw.cn/Article/details/gctxgjxjy.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/ggpqwuwua.sHtML

[S49] C++：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gmqobhqfx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/ghwzuxfdp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.vehdjk.com/Article/details/gcmehzeyh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.vehdjk.com/Article/details/ggutndyjg.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fktsv.cn/Article/details/gcnifltem.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/ghcbvbelx.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.vehdjk.com/Article/details/glwewxqyb.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.yfazqb.com/Article/details/getejnvxl.sHtML

[S53] C++：移动语义
来源：http://3g.vehdjk.com/Article/details/gupomaziu.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.bbcook.cn/Article/details/gaozmopcj.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/gsoivwmca.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.yfazqb.com/Article/details/gunrsieyv.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/glogqfeda.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fktsv.cn/Article/details/gogybxsgu.sHtML

[S56] C++：optional
来源：http://blog.epnwcf.com/Article/details/gtegymalm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/ggzroxwsq.sHtML

[S57] C++：编译期常量
来源：http://www.share.fktsv.cn/Article/details/gyvcbdmlt.sHtML

constexpr int N = 10;
来源：http://www.blog.fktsv.cn/Article/details/grlnaoxaw.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/geqplfbsk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/gjoopfwdo.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/gfylvvjdw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.tarul.cn/Article/details/gkwstohpv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gqqcghosd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/gwvalocqn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gcdzmrfot.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/gfevatjct.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gefasjdar.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.vehdjk.com/Article/details/gcsbqlqim.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gpumbfqiu.sHtML

[T02] Kotlin：变量
来源：http://blog.vehdjk.com/Article/details/ghzueylrk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.vehdjk.com/Article/details/gtsvqysws.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fktsv.cn/Article/details/ghokfcrwg.sHtML

"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gsuevcbli.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fktsv.cn/Article/details/gwnhizzvl.sHtML

val n: String? = null;  n?.length
来源：http://blog.bbcook.cn/Article/details/gfagjcgim.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.epnwcf.com/Article/details/gnyoxcpnj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.sjlbkw.cn/Article/details/gobkmcgdi.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.vehdjk.com/Article/details/gpidcepde.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/giplrifrl.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gfcxhpbvs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.epnwcf.com/Article/details/glfzigvpp.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/gjysuqaab.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gvupwyvvg.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/gwxrmsguz.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.bbcook.cn/Article/details/gsxiweajx.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fktsv.cn/Article/details/gqalmeubm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.sjlbkw.cn/Article/details/gptjfjsqa.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.sjlbkw.cn/Article/details/gorgclobo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.tarul.cn/Article/details/gnuiiwlwu.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.sjlbkw.cn/Article/details/glubjqxra.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/goitksvmx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fktsv.cn/Article/details/gmaehdoug.sHtML

val m = mapOf("a" to 1)
来源：http://3g.sjlbkw.cn/Article/details/guvxklctg.sHtML

[T14] Kotlin：循环
来源：http://wap.vehdjk.com/Article/details/glzyxxsyx.sHtML

for (i in 1..10) println(i)
来源：http://3g.fktsv.cn/Article/details/gmyfzlcqm.sHtML

[T15] Kotlin：接口
来源：http://www.blog.yfazqb.com/Article/details/gibocixmk.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gsnfkaquy.sHtML

[T16] Swift：Hello World
来源：http://m.share.yfazqb.com/Article/details/grgtlfqlv.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/gzcuzqjce.sHtML

[T17] Swift：变量与常量
来源：http://www.share.yfazqb.com/Article/details/gzfyxogxr.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gsyzzzuvn.sHtML

[T18] Swift：字符串插值
来源：http://mobile.tarul.cn/Article/details/gvchnyyhx.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/gyvqixjra.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fktsv.cn/Article/details/geuguncoq.sHtML

if let n = opt { print(n) }
来源：http://mobile.epnwcf.com/Article/details/gnhxbzsmx.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.epnwcf.com/Article/details/gpfefcvxc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/ghjflappn.sHtML

[T21] Swift：遍历
来源：http://m.share.fktsv.cn/Article/details/gtyenzevh.sHtML

for x in a { print(x) }
来源：http://www.share.fktsv.cn/Article/details/grnsrlyxh.sHtML

[T22] Swift：字典
来源：http://www.share.epnwcf.com/Article/details/gsdiyzqoe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.epnwcf.com/Article/details/gtrbwrbcr.sHtML

[T23] Swift：函数
来源：http://m.share.sjlbkw.cn/Article/details/gmqbasdnw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.yfazqb.com/Article/details/grgafccfz.sHtML

[T24] Swift：闭包
来源：http://www.blog.tarul.cn/Article/details/gqdsnraug.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gexdxrrmy.sHtML

[T25] Swift：结构体
来源：http://mobile.fktsv.cn/Article/details/gnuelhvki.sHtML

struct P { var x: Int }
来源：http://3g.sjlbkw.cn/Article/details/gafghvuwq.sHtML

[T26] Swift：类与重写
来源：http://baike.yfazqb.com/Article/details/gtvjrwpzx.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.tarul.cn/Article/details/ghobreeqq.sHtML

[T27] Swift：错误处理
来源：http://baike.fktsv.cn/Article/details/gvhhjlymc.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fktsv.cn/Article/details/gouvgthpv.sHtML

[T28] Swift：枚举
来源：http://www.blog.fktsv.cn/Article/details/gcjbbdgzv.sHtML

enum Color { case red, green }
来源：http://m.share.bbcook.cn/Article/details/gnqcquiej.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fktsv.cn/Article/details/gcnaipdgq.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gazfxwagj.sHtML

[T30] Swift：协议
来源：http://www.blog.epnwcf.com/Article/details/gwvnlcezt.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.epnwcf.com/Article/details/gahsszyqa.sHtML

[T31] Lua：Hello World
来源：http://m.share.bbcook.cn/Article/details/glwwduiju.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gbhvonazb.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fktsv.cn/Article/details/gmrfhwaol.sHtML

local a = 1
来源：http://blog.fktsv.cn/Article/details/glfzmznli.sHtML

[T33] Lua：表（数组）
来源：http://wap.sjlbkw.cn/Article/details/gilxenhmj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.bbcook.cn/Article/details/gcxaiogyi.sHtML

[T34] Lua：遍历表
来源：http://blog.vehdjk.com/Article/details/gwtrcbzyj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.vehdjk.com/Article/details/gvexsagok.sHtML

[T35] Lua：字典表
来源：http://3g.yfazqb.com/Article/details/gxpgmbjmx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.yfazqb.com/Article/details/gkgbkkhxg.sHtML

[T36] Lua：函数
来源：http://3g.fktsv.cn/Article/details/gkjotcswz.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.vehdjk.com/Article/details/gjnlxtnbl.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/gshgsnbkz.sHtML

"a" .. "b"
来源：http://wap.tarul.cn/Article/details/gdqloidcj.sHtML

[T38] Lua：条件
来源：http://baike.sjlbkw.cn/Article/details/gypzhmbrn.sHtML

if x > 0 then print("正") end
来源：http://baike.yfazqb.com/Article/details/glbcmgyrr.sHtML

[T39] Lua：模式匹配
来源：http://mobile.vehdjk.com/Article/details/gmebtnibn.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fktsv.cn/Article/details/gxnatciio.sHtML

[T40] Lua：元表
来源：http://www.m.share.bbcook.cn/Article/details/gshxhrwpb.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.epnwcf.com/Article/details/gwwdqfoic.sHtML

[T41] Perl：Hello World
来源：http://blog.epnwcf.com/Article/details/gjbxfmlel.sHtML

print "Hello\n";
来源：http://mobile.yfazqb.com/Article/details/gpodjwloj.sHtML

[T42] Perl：变量类型
来源：http://read.share.bbcook.cn/Article/details/gbpbuikzy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fktsv.cn/Article/details/gxjqrjxqd.sHtML

[T43] Perl：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gfmawcgff.sHtML

"值: $a"
来源：http://mobile.epnwcf.com/Article/details/gmbzlptlq.sHtML

[T44] Perl：条件
来源：http://blog.fktsv.cn/Article/details/ggarcxdvi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyugsciwf.sHtML

[T45] Perl：数组遍历
来源：http://read.share.yfazqb.com/Article/details/gsbvwgpsv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.epnwcf.com/Article/details/gpprzjmim.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gszlllcvm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.bbcook.cn/Article/details/ggbsozcxq.sHtML

[T47] Perl：正则捕获
来源：http://blog.fktsv.cn/Article/details/gddukkgxj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.bbcook.cn/Article/details/ggjavvkix.sHtML

[T48] Perl：正则替换
来源：http://mobile.epnwcf.com/Article/details/gmltmzswr.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fktsv.cn/Article/details/gcstubobv.sHtML

[T49] Perl：函数
来源：http://www.m.share.fktsv.cn/Article/details/gxvvpouoi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gilerknfc.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gdtdbexxh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.vehdjk.com/Article/details/gjldaabos.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.tarul.cn/Article/details/ghigubujn.sHtML

[T51] Scala：Hello World
来源：http://wap.yfazqb.com/Article/details/gqgejuluf.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gyggsczsg.sHtML

[T52] Scala：变量
来源：http://www.m.share.tarul.cn/Article/details/gkgekhonu.sHtML

val a = 1;  var b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gmhcxrlqf.sHtML

[T53] Scala：字符串插值
来源：http://blog.fktsv.cn/Article/details/glllboora.sHtML

s"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/ghkglrmcy.sHtML

[T54] Scala：集合映射
来源：http://baike.tarul.cn/Article/details/gxcofdaha.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.bbcook.cn/Article/details/gaojsybwq.sHtML

[T55] Scala：集合过滤
来源：http://wap.epnwcf.com/Article/details/gsraoyhvl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.bbcook.cn/Article/details/ggslgqnjj.sHtML

[T56] Scala：样例类
来源：http://mobile.fktsv.cn/Article/details/gyotttfad.sHtML

case class User(name: String, age: Int)
来源：http://blog.epnwcf.com/Article/details/gjutsbbdz.sHtML

[T57] Scala：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gldxqpoeb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.bbcook.cn/Article/details/gymngcqsq.sHtML

[T58] Scala：函数定义
来源：http://3g.epnwcf.com/Article/details/ghzxgdpbv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.tarul.cn/Article/details/gtnqsmuqs.sHtML

[T59] Scala：循环
来源：http://www.m.share.tarul.cn/Article/details/gtmkzvwra.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gvybrrgfc.sHtML

[T60] Scala：折叠
来源：http://www.m.share.epnwcf.com/Article/details/goormatgb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fktsv.cn/Article/details/gzrbboqln.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwygbrzxa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.sjlbkw.cn/Article/details/gyqpsaxmz.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/guluvfxya.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.bbcook.cn/Article/details/gopqczfld.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.vehdjk.com/Article/details/gmoatfwkg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.vehdjk.com/Article/details/ggmtpljgr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.sjlbkw.cn/Article/details/ggpcvvxiz.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fktsv.cn/Article/details/gjpeemqhe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.sjlbkw.cn/Article/details/gdydfgfij.sHtML

[U04] Py：变量调试打印
来源：http://read.share.vehdjk.com/Article/details/gqzzxzaji.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.yfazqb.com/Article/details/gxibsytnh.sHtML

[U05] Py：列表去重且保序
来源：http://wap.epnwcf.com/Article/details/glyehnwps.sHtML

list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gsnjqwlgw.sHtML

[U06] Py：合并两个字典
来源：http://www.share.yfazqb.com/Article/details/gacgpjnth.sHtML

{**a, **b}
来源：http://3g.vehdjk.com/Article/details/gqlkyizyz.sHtML

[U07] Py：反转字典键值
来源：http://wap.epnwcf.com/Article/details/gwvgjwkbg.sHtML

{v: k for k, v in d.items()}
来源：http://baike.yfazqb.com/Article/details/goatwmljg.sHtML

[U08] Py：展平二维列表
来源：http://blog.yfazqb.com/Article/details/gbphmvdlp.sHtML

[y for x in nested for y in x]
来源：http://www.share.tarul.cn/Article/details/gcitiboej.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.epnwcf.com/Article/details/gpxzeochd.sHtML

max(d, key=d.get)
来源：http://wap.sjlbkw.cn/Article/details/gbprkyejl.sHtML

[U10] Py：按值排序字典
来源：http://mobile.yfazqb.com/Article/details/gxzgijtbj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.epnwcf.com/Article/details/ghcwojttf.sHtML


<!-- 参考信息 -->