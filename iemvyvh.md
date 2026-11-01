代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://baike.fktsv.cn/Article/details/gmxeifgui.sHtML

[R70] 时间戳与互转
来源：http://www.share.vehdjk.com/Article/details/geockqguk.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fktsv.cn/Article/details/gfbyomytk.sHtML

[R71] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gvqaurzwx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fktsv.cn/Article/details/gthhaefpr.sHtML

[R72] 等待端口就绪
来源：http://wap.bbcook.cn/Article/details/gualnpwdi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fktsv.cn/Article/details/gtzpwsqed.sHtML

[R73] 分割大日志
来源：http://read.share.bbcook.cn/Article/details/gdjlplxaa.sHtML

split -l 1000 big.log part_
来源：http://m.share.epnwcf.com/Article/details/gjdrfywuh.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gaqycyslo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.yfazqb.com/Article/details/gxnxicrzr.sHtML

[R75] 导出环境变量
来源：http://www.share.tarul.cn/Article/details/grjzvcfml.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fktsv.cn/Article/details/gawvljkfq.sHtML

[R76] 使用临时文件
来源：http://mobile.epnwcf.com/Article/details/gsrdxozyg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gqdmnjjzc.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gwleowcmf.sHtML

read -rp "请输入: " ans
来源：http://wap.fktsv.cn/Article/details/gthtmkurd.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/gaxanqisz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.yfazqb.com/Article/details/gluzjskaj.sHtML

[R79] 解析命令行选项
来源：http://m.share.sjlbkw.cn/Article/details/gqktldzyt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/gkdlvgqil.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.bbcook.cn/Article/details/gmmoyhpby.sHtML

time ./run.sh
来源：http://www.share.vehdjk.com/Article/details/gggwrjpog.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gnhliufxr.sHtML

S. C / C++ 专题
来源：http://baike.yfazqb.com/Article/details/gnsskgsoz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gniwwfmtr.sHtML

[S01] C：Hello World
来源：http://wap.fktsv.cn/Article/details/gwezufuvv.sHtML

#include <stdio.h>
来源：http://www.share.fktsv.cn/Article/details/glraaowds.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.bbcook.cn/Article/details/gpozcfihu.sHtML

[S02] C：变量与格式化输出
来源：http://wap.yfazqb.com/Article/details/gzminqjnp.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.bbcook.cn/Article/details/gbtgucgoa.sHtML

[S03] C：读入整数
来源：http://mobile.epnwcf.com/Article/details/gdyqcvbrp.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.vehdjk.com/Article/details/ggenfvkdx.sHtML

[S04] C：字符串复制
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsopdlai.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.tarul.cn/Article/details/gnphacofo.sHtML

[S05] C：字符串长度
来源：http://www.share.fktsv.cn/Article/details/gbneutjzi.sHtML

strlen(s)
来源：http://3g.yfazqb.com/Article/details/gdimwzkyg.sHtML

[S06] C：字符串比较
来源：http://www.share.fktsv.cn/Article/details/gsavxhqbm.sHtML

strcmp(a, b) == 0
来源：http://www.blog.vehdjk.com/Article/details/gzynvnldo.sHtML

[S07] C：数组遍历求和
来源：http://m.share.epnwcf.com/Article/details/gveyhheou.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/gvuaicbyd.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.vehdjk.com/Article/details/gdtqbtdlo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.epnwcf.com/Article/details/guvptobvp.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.epnwcf.com/Article/details/gffcbzubl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.bbcook.cn/Article/details/gwuvsqrmf.sHtML

[S10] C：指针与解引用
来源：http://read.share.vehdjk.com/Article/details/gucmskuuz.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.bbcook.cn/Article/details/gwvgnaqoi.sHtML

[S11] C：逐行读文件
来源：http://mobile.tarul.cn/Article/details/ghuclvjvx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fktsv.cn/Article/details/giupayext.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.epnwcf.com/Article/details/gnhmjjiwi.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gfzsglizd.sHtML

[S12] C：写文件
来源：http://www.blog.epnwcf.com/Article/details/gniwvrrpe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gnuleaxhn.sHtML

[S13] C：宏定义
来源：http://blog.yfazqb.com/Article/details/gvvrrdhtg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.vehdjk.com/Article/details/gulmltift.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/ghsnbmbvq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.yfazqb.com/Article/details/gkhxquhfz.sHtML

[S15] C：类型转换
来源：http://wap.epnwcf.com/Article/details/gfkfekrpc.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/gixjknzmh.sHtML

[S16] C：位操作置位
来源：http://blog.fktsv.cn/Article/details/gwgadpcxc.sHtML

x |= (1 << 3);
来源：http://wap.tarul.cn/Article/details/gznunsxvi.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.epnwcf.com/Article/details/grxyodnga.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.sjlbkw.cn/Article/details/gxhwrpuoq.sHtML

[S18] C：命令行参数
来源：http://read.share.epnwcf.com/Article/details/grkmohczz.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/gwuoftsub.sHtML

[S19] C：快速排序
来源：http://3g.vehdjk.com/Article/details/gngxfmlzp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gwiwtlfbi.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/gktzjetsw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gfjwmkoix.sHtML

[S21] C：字符类别判断
来源：http://read.share.yfazqb.com/Article/details/gkoagerlg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.sjlbkw.cn/Article/details/gnardnsqc.sHtML

[S22] C：字符串转数字
来源：http://m.share.epnwcf.com/Article/details/gkpwcfczl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.yfazqb.com/Article/details/ggjlbsnvg.sHtML

[S23] C：随机数
来源：http://baike.vehdjk.com/Article/details/gvbrmczoo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.tarul.cn/Article/details/gbmfqmkcf.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gpmfnhzvn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/gwuevbfnu.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/gpergsbdd.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.vehdjk.com/Article/details/gqwvquuxe.sHtML

[S26] C：内存清零
来源：http://m.share.tarul.cn/Article/details/grlfzbnpv.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.epnwcf.com/Article/details/gigefetjq.sHtML

[S27] C：定义常量
来源：http://baike.yfazqb.com/Article/details/gqjxwrsek.sHtML

const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gzdidlbsg.sHtML

[S28] C：静态变量
来源：http://baike.vehdjk.com/Article/details/gwcniyeas.sHtML

static int counter = 0;
来源：http://wap.yfazqb.com/Article/details/gdcpuoahy.sHtML

[S29] C：变参函数
来源：http://3g.bbcook.cn/Article/details/galxhbkyg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gutfngkjs.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gfhmgzjzl.sHtML

#ifndef X_H
来源：http://m.share.tarul.cn/Article/details/giwgmmxwu.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gsxsudnmn.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/gpllrchvs.sHtML

[S31] C++：Hello World
来源：http://read.share.yfazqb.com/Article/details/gsxyfzesq.sHtML

#include <iostream>
来源：http://m.share.sjlbkw.cn/Article/details/gcyqwctqp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.bbcook.cn/Article/details/gsvwnphxa.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/gbnyxiwyk.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/gxqzlpocd.sHtML

[S33] C++：vector 增删
来源：http://m.share.bbcook.cn/Article/details/gdbgavsjx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.tarul.cn/Article/details/gbpuduefr.sHtML

[S34] C++：遍历 vector
来源：http://3g.epnwcf.com/Article/details/gxnxfpkub.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.yfazqb.com/Article/details/gqngkkvxp.sHtML

[S35] C++：map
来源：http://3g.bbcook.cn/Article/details/gjeuxkcis.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gbsdddnsm.sHtML

[S36] C++：unordered_map
来源：http://m.share.yfazqb.com/Article/details/gtxgrupqv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzyxvbao.sHtML

[S37] C++：set
来源：http://baike.sjlbkw.cn/Article/details/gqaqhrywb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.vehdjk.com/Article/details/gmhndlvnz.sHtML

[S38] C++：排序
来源：http://m.share.tarul.cn/Article/details/grwuzyyvz.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.vehdjk.com/Article/details/ghkupsrlz.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gfflnosyb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.vehdjk.com/Article/details/gzqcpgtyj.sHtML

[S40] C++：查找元素
来源：http://3g.vehdjk.com/Article/details/gcnezmcpg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.tarul.cn/Article/details/gkrbkqxnq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gicjtgfhb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fktsv.cn/Article/details/gkuaoanph.sHtML

[S42] C++：继承与虚函数
来源：http://baike.tarul.cn/Article/details/ggpqtkyyi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.tarul.cn/Article/details/ggpnfxwmh.sHtML

[S43] C++：智能指针
来源：http://www.m.share.bbcook.cn/Article/details/gypqrdbth.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fktsv.cn/Article/details/gfvnokrjs.sHtML

[S44] C++：引用传参
来源：http://www.share.tarul.cn/Article/details/gqrqulrmw.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.tarul.cn/Article/details/gnhvyhyxh.sHtML

[S45] C++：lambda
来源：http://blog.epnwcf.com/Article/details/gfhjbcltj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.yfazqb.com/Article/details/ggfgrjfhx.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gzloufaew.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.epnwcf.com/Article/details/gankcrotk.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.yfazqb.com/Article/details/gazlvyivk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.vehdjk.com/Article/details/gictusprl.sHtML

[S48] C++：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gwlphbrkz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.bbcook.cn/Article/details/gsslncpne.sHtML

while (std::getline(in, line)) { }
来源：http://baike.epnwcf.com/Article/details/gpgtuvtsj.sHtML

[S49] C++：写文件
来源：http://m.share.yfazqb.com/Article/details/gzxujyfba.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/gnahgzlaj.sHtML

[S50] C++：格式化数字
来源：http://www.share.tarul.cn/Article/details/gnskmsrxg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxntlaqf.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/grnwlbhrc.sHtML

static_cast<double>(a) / b
来源：http://www.share.fktsv.cn/Article/details/gbrvzurzc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fktsv.cn/Article/details/gljgzgrbn.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.epnwcf.com/Article/details/guwgjyogv.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/gqihtozag.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.epnwcf.com/Article/details/gobqulihg.sHtML

[S54] C++：异常处理
来源：http://wap.sjlbkw.cn/Article/details/gbvczcive.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.vehdjk.com/Article/details/gehbxnluw.sHtML

[S55] C++：结构化绑定
来源：http://baike.sjlbkw.cn/Article/details/gyohzjxgh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/gxtyhjztk.sHtML

[S56] C++：optional
来源：http://read.share.epnwcf.com/Article/details/gemdtlplb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fktsv.cn/Article/details/ghwugvvbi.sHtML

[S57] C++：编译期常量
来源：http://baike.yfazqb.com/Article/details/gnvjqxrtc.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/gvsjzadzd.sHtML

[S58] C++：命名空间
来源：http://read.share.fktsv.cn/Article/details/gblozdxwj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/gjyowcrxx.sHtML

[S59] C++：静态断言
来源：http://read.share.sjlbkw.cn/Article/details/gplymozbg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.epnwcf.com/Article/details/glrnmgumg.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.yfazqb.com/Article/details/guxwcfdhr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.bbcook.cn/Article/details/ghpnnxlxo.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gglhkialk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gzytooxfw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gnfmrmyds.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gxjvhitwc.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gyxpbowrg.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gzgcsujqw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.epnwcf.com/Article/details/gnmuebwkj.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fktsv.cn/Article/details/gmggbptcd.sHtML

"值: $b"
来源：http://blog.fktsv.cn/Article/details/gpylztohc.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/gplxmuawk.sHtML

val n: String? = null;  n?.length
来源：http://read.share.vehdjk.com/Article/details/geoehqdih.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.tarul.cn/Article/details/gylmqdrut.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/gcaxrzech.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gxgdvposg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.epnwcf.com/Article/details/gxjutrqmn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/gzdqnrneo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.sjlbkw.cn/Article/details/ggwxzdpdj.sHtML

[T08] Kotlin：数据类
来源：http://baike.vehdjk.com/Article/details/gazictwar.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.epnwcf.com/Article/details/godvjolof.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.tarul.cn/Article/details/gjttosrmf.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.vehdjk.com/Article/details/gyvpwjovn.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.bbcook.cn/Article/details/galzvjejl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.epnwcf.com/Article/details/gzdieomce.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.epnwcf.com/Article/details/gdloohsjm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.tarul.cn/Article/details/gouzaipyv.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fktsv.cn/Article/details/gvuehfxmn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gcgiatnix.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fktsv.cn/Article/details/ggedsfvyx.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fktsv.cn/Article/details/gnhiahfsz.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.tarul.cn/Article/details/gtamvcxzg.sHtML

for (i in 1..10) println(i)
来源：http://wap.fktsv.cn/Article/details/gvmpddydq.sHtML

[T15] Kotlin：接口
来源：http://www.blog.epnwcf.com/Article/details/gfvmgakvy.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/gglnguksf.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/ggwlpeuja.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gjegditzv.sHtML

[T17] Swift：变量与常量
来源：http://3g.vehdjk.com/Article/details/gktdstqxc.sHtML

var a = 1;  let b = 2
来源：http://read.share.epnwcf.com/Article/details/gyftxtsvm.sHtML

[T18] Swift：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gpdvhgalf.sHtML

"值: \(b)"
来源：http://read.share.bbcook.cn/Article/details/gqgphqdjz.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.vehdjk.com/Article/details/gnvbwskft.sHtML

if let n = opt { print(n) }
来源：http://blog.bbcook.cn/Article/details/goqlqhfpk.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.vehdjk.com/Article/details/gtqoelzqz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.sjlbkw.cn/Article/details/gzplexhrv.sHtML

[T21] Swift：遍历
来源：http://www.blog.vehdjk.com/Article/details/ggiqywipg.sHtML

for x in a { print(x) }
来源：http://read.share.bbcook.cn/Article/details/gfeyfvyvf.sHtML

[T22] Swift：字典
来源：http://blog.tarul.cn/Article/details/gnppiscqq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fktsv.cn/Article/details/gdezttpmp.sHtML

[T23] Swift：函数
来源：http://m.share.sjlbkw.cn/Article/details/gwressvlr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.sjlbkw.cn/Article/details/grsroqafg.sHtML

[T24] Swift：闭包
来源：http://3g.yfazqb.com/Article/details/gyiknnyff.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.epnwcf.com/Article/details/gbtjrkzdj.sHtML

[T25] Swift：结构体
来源：http://wap.epnwcf.com/Article/details/gzrqyzayc.sHtML

struct P { var x: Int }
来源：http://wap.vehdjk.com/Article/details/gwtsrhisk.sHtML

[T26] Swift：类与重写
来源：http://wap.tarul.cn/Article/details/gbbbxhtce.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.yfazqb.com/Article/details/geibqytxd.sHtML

[T27] Swift：错误处理
来源：http://blog.epnwcf.com/Article/details/gfmeketau.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fktsv.cn/Article/details/gstygshsh.sHtML

[T28] Swift：枚举
来源：http://read.share.yfazqb.com/Article/details/gkbfgprqd.sHtML

enum Color { case red, green }
来源：http://m.share.vehdjk.com/Article/details/gwiyxtqef.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fktsv.cn/Article/details/gxagmhpyp.sHtML

guard let x = opt else { return }
来源：http://mobile.fktsv.cn/Article/details/gboomcmsb.sHtML

[T30] Swift：协议
来源：http://www.share.vehdjk.com/Article/details/gjibufacd.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.yfazqb.com/Article/details/glximpcnq.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gonwecmwj.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gilldwisc.sHtML

[T32] Lua：局部变量
来源：http://m.share.bbcook.cn/Article/details/gcbihwkrs.sHtML

local a = 1
来源：http://wap.bbcook.cn/Article/details/gcjwwusxg.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.tarul.cn/Article/details/gonvrxunp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.sjlbkw.cn/Article/details/gknfrylye.sHtML

[T34] Lua：遍历表
来源：http://blog.tarul.cn/Article/details/gitceytqi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.sjlbkw.cn/Article/details/gwudpegee.sHtML

[T35] Lua：字典表
来源：http://mobile.fktsv.cn/Article/details/gziqjgxdx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.bbcook.cn/Article/details/gkyadppco.sHtML

[T36] Lua：函数
来源：http://wap.fktsv.cn/Article/details/gqohqhmiz.sHtML

function add(a, b) return a + b end
来源：http://baike.tarul.cn/Article/details/gotxnlcbg.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gnxtpvjeb.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/gdysxpyna.sHtML

[T38] Lua：条件
来源：http://www.m.share.fktsv.cn/Article/details/gjemuofdo.sHtML

if x > 0 then print("正") end
来源：http://m.share.vehdjk.com/Article/details/gyypuekkz.sHtML

[T39] Lua：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gcskugmyp.sHtML

string.find(s, "%d+")
来源：http://3g.yfazqb.com/Article/details/gzilwlapi.sHtML

[T40] Lua：元表
来源：http://wap.epnwcf.com/Article/details/gyeycbjrl.sHtML

setmetatable({}, { __index = base })
来源：http://baike.yfazqb.com/Article/details/gziiztukw.sHtML

[T41] Perl：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gyvqicdkm.sHtML

print "Hello\n";
来源：http://www.share.sjlbkw.cn/Article/details/gjgfqfnia.sHtML

[T42] Perl：变量类型
来源：http://www.blog.bbcook.cn/Article/details/gxnovysax.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.bbcook.cn/Article/details/glrqdxwfu.sHtML

[T43] Perl：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gsgpkdvbu.sHtML

"值: $a"
来源：http://blog.yfazqb.com/Article/details/gbffaocsc.sHtML

[T44] Perl：条件
来源：http://wap.epnwcf.com/Article/details/gxndsmyag.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/gnnpvzbuh.sHtML

[T45] Perl：数组遍历
来源：http://wap.vehdjk.com/Article/details/gkngrwalh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fktsv.cn/Article/details/gsvjbvhqr.sHtML

[T46] Perl：哈希操作
来源：http://blog.epnwcf.com/Article/details/gupiogaps.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.epnwcf.com/Article/details/gtbivsvrd.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.vehdjk.com/Article/details/gpwdbdvkk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.vehdjk.com/Article/details/gneifgmmr.sHtML

[T48] Perl：正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gmfquskml.sHtML

$s =~ s/old/new/g;
来源：http://wap.tarul.cn/Article/details/gnmvbbepa.sHtML

[T49] Perl：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gbeehujzi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/ghuinoqtx.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/giwkpouqb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.sjlbkw.cn/Article/details/gtwsmsrmo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.tarul.cn/Article/details/gvvcihsgq.sHtML

[T51] Scala：Hello World
来源：http://blog.fktsv.cn/Article/details/gtvwfqicq.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gqohovopf.sHtML

[T52] Scala：变量
来源：http://mobile.yfazqb.com/Article/details/gyxbupviu.sHtML

val a = 1;  var b = 2
来源：http://m.share.bbcook.cn/Article/details/gntjbuknm.sHtML

[T53] Scala：字符串插值
来源：http://baike.tarul.cn/Article/details/ghmtnucku.sHtML

s"值: $b"
来源：http://read.share.yfazqb.com/Article/details/gumlyafjd.sHtML

[T54] Scala：集合映射
来源：http://read.share.vehdjk.com/Article/details/ggugliedj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.epnwcf.com/Article/details/gdkuafhhy.sHtML

[T55] Scala：集合过滤
来源：http://baike.tarul.cn/Article/details/gshgqafav.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fktsv.cn/Article/details/gvbqssukv.sHtML

[T56] Scala：样例类
来源：http://m.share.tarul.cn/Article/details/gktxqqkut.sHtML

case class User(name: String, age: Int)
来源：http://mobile.epnwcf.com/Article/details/gvtxzbbcb.sHtML

[T57] Scala：模式匹配
来源：http://3g.epnwcf.com/Article/details/gciaffxbf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.epnwcf.com/Article/details/gcazbhlmv.sHtML

[T58] Scala：函数定义
来源：http://baike.yfazqb.com/Article/details/gzirthnik.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.vehdjk.com/Article/details/gjrkpfetw.sHtML

[T59] Scala：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gtnsphvsu.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.yfazqb.com/Article/details/gfnobdxnx.sHtML

[T60] Scala：折叠
来源：http://wap.tarul.cn/Article/details/gtupcpvms.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.yfazqb.com/Article/details/gkomsuvjo.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbcmfxdxa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.bbcook.cn/Article/details/gvefrmvqy.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gciqovbzr.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.yfazqb.com/Article/details/gbcnacebb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.bbcook.cn/Article/details/gqwootvph.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.sjlbkw.cn/Article/details/gihqcdpui.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.bbcook.cn/Article/details/gjntpsfia.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.epnwcf.com/Article/details/gpnobbrrx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.bbcook.cn/Article/details/gxckjxgcn.sHtML

[U04] Py：变量调试打印
来源：http://www.share.yfazqb.com/Article/details/giprisufu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.sjlbkw.cn/Article/details/gpfarhjcq.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/grbttbtlw.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.epnwcf.com/Article/details/guxgfjxom.sHtML

[U06] Py：合并两个字典
来源：http://read.share.vehdjk.com/Article/details/gslgayedo.sHtML

{**a, **b}
来源：http://www.m.share.fktsv.cn/Article/details/gczwitgwf.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fktsv.cn/Article/details/gjmckxpzs.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.yfazqb.com/Article/details/gemzxxtac.sHtML

[U08] Py：展平二维列表
来源：http://3g.yfazqb.com/Article/details/gjmcdsmce.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.sjlbkw.cn/Article/details/gosqaltvy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.sjlbkw.cn/Article/details/grbwvkeqe.sHtML

max(d, key=d.get)
来源：http://wap.yfazqb.com/Article/details/gpsoircva.sHtML

[U10] Py：按值排序字典
来源：http://www.share.bbcook.cn/Article/details/grmrfduix.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.tarul.cn/Article/details/gtciewigm.sHtML


<!-- 参考信息 -->