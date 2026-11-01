代发 wailian999

openssl rand -hex 16
来源：http://m.share.fktsv.cn/Article/details/gwukiqqew.sHtML

[R68] 计算文件校验值
来源：http://blog.bbcook.cn/Article/details/gcdhuohlm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fktsv.cn/Article/details/gchmbmqjd.sHtML

[R69] 生成随机密码
来源：http://m.share.yfazqb.com/Article/details/gaznagwrt.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.epnwcf.com/Article/details/gkjxvsued.sHtML

[R70] 时间戳与互转
来源：http://www.blog.sjlbkw.cn/Article/details/gyflcjhdm.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.yfazqb.com/Article/details/givvzmsaw.sHtML

[R71] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gioablgnd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.tarul.cn/Article/details/gtuuvgsms.sHtML

[R72] 等待端口就绪
来源：http://m.share.epnwcf.com/Article/details/gzgjmrltg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/girszdsad.sHtML

[R73] 分割大日志
来源：http://www.blog.tarul.cn/Article/details/gqgzdcgfp.sHtML

split -l 1000 big.log part_
来源：http://3g.yfazqb.com/Article/details/gqsnumdjy.sHtML

[R74] 批量重命名
来源：http://3g.fktsv.cn/Article/details/gsldfiwhy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.sjlbkw.cn/Article/details/ghqjazoib.sHtML

[R75] 导出环境变量
来源：http://blog.bbcook.cn/Article/details/gmfrntfuw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.tarul.cn/Article/details/gygoxnynn.sHtML

[R76] 使用临时文件
来源：http://mobile.tarul.cn/Article/details/gyjjneicn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gygiipbki.sHtML

[R77] 读取用户输入
来源：http://baike.vehdjk.com/Article/details/gwyffammp.sHtML

read -rp "请输入: " ans
来源：http://m.share.bbcook.cn/Article/details/gjbsnzkrt.sHtML

[R78] 交互式菜单
来源：http://www.blog.fktsv.cn/Article/details/gxqmtjalu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fktsv.cn/Article/details/gzxijehyw.sHtML

[R79] 解析命令行选项
来源：http://m.share.yfazqb.com/Article/details/gmsbcrioc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.epnwcf.com/Article/details/gvstilvie.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.vehdjk.com/Article/details/gnfejgtac.sHtML

time ./run.sh
来源：http://www.share.fktsv.cn/Article/details/gijjqidwd.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmiciynrj.sHtML

S. C / C++ 专题
来源：http://wap.vehdjk.com/Article/details/glqxhaqcu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gqoeqevrv.sHtML

[S01] C：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gaynjuvjb.sHtML

#include <stdio.h>
来源：http://mobile.vehdjk.com/Article/details/gszxvqvpn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.vehdjk.com/Article/details/gqyyfddmn.sHtML

[S02] C：变量与格式化输出
来源：http://blog.vehdjk.com/Article/details/gamjrfofk.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fktsv.cn/Article/details/gdtflfphv.sHtML

[S03] C：读入整数
来源：http://read.share.sjlbkw.cn/Article/details/gidzqjrxl.sHtML

int x; scanf("%d", &x);
来源：http://baike.tarul.cn/Article/details/gzyfrjjje.sHtML

[S04] C：字符串复制
来源：http://wap.sjlbkw.cn/Article/details/gnjpjfhra.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/gpqmldngy.sHtML

[S05] C：字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gevbeopuq.sHtML

strlen(s)
来源：http://wap.fktsv.cn/Article/details/grrdnplyc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgqaezpx.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gpxjxqmst.sHtML

[S07] C：数组遍历求和
来源：http://read.share.vehdjk.com/Article/details/gdiwloyqv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.bbcook.cn/Article/details/gnpqbgtrs.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.sjlbkw.cn/Article/details/gkfhvwren.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/gpgczjhxw.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.epnwcf.com/Article/details/gewwjpyjo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.bbcook.cn/Article/details/gsmnffvqf.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.vehdjk.com/Article/details/gysembsne.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/gutuzubnf.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gxooqbhtf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fktsv.cn/Article/details/gcssqxout.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fktsv.cn/Article/details/gquxvwyhm.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gdcrjrizh.sHtML

[S12] C：写文件
来源：http://www.blog.epnwcf.com/Article/details/gwvynrtts.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gcfltsnru.sHtML

[S13] C：宏定义
来源：http://3g.sjlbkw.cn/Article/details/gabwkvyay.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.tarul.cn/Article/details/gismyvcgo.sHtML

[S14] C：枚举
来源：http://read.share.epnwcf.com/Article/details/geaffpzog.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.bbcook.cn/Article/details/gavqcrzey.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gndwtpdzr.sHtML

(double) a / b
来源：http://3g.bbcook.cn/Article/details/gewcwclgq.sHtML

[S16] C：位操作置位
来源：http://baike.yfazqb.com/Article/details/gpxerglzc.sHtML

x |= (1 << 3);
来源：http://3g.vehdjk.com/Article/details/gezwnucyy.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/gxtpvyhou.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fktsv.cn/Article/details/gikkxqeee.sHtML

[S18] C：命令行参数
来源：http://wap.epnwcf.com/Article/details/ghhvjpour.sHtML

int main(int argc, char **argv)
来源：http://www.share.sjlbkw.cn/Article/details/gomslvbah.sHtML

[S19] C：快速排序
来源：http://mobile.vehdjk.com/Article/details/gtcpkpxhi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gvuiobdff.sHtML

[S20] C：二分查找
来源：http://mobile.epnwcf.com/Article/details/glkyksbkb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/geuteenuu.sHtML

[S21] C：字符类别判断
来源：http://read.share.yfazqb.com/Article/details/gvydjbfna.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.yfazqb.com/Article/details/glaalrrrn.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/gsndeuvej.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.tarul.cn/Article/details/getebotiv.sHtML

[S23] C：随机数
来源：http://read.share.yfazqb.com/Article/details/gfpmjcaey.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.tarul.cn/Article/details/gjikumzxj.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/gtgginbzb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.vehdjk.com/Article/details/gvqklykhq.sHtML

[S25] C：内存拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gsfkdjzcn.sHtML

memcpy(dst, src, n);
来源：http://www.share.epnwcf.com/Article/details/gdeztjizs.sHtML

[S26] C：内存清零
来源：http://www.blog.tarul.cn/Article/details/guukrqubw.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/gfnunqgmj.sHtML

[S27] C：定义常量
来源：http://www.blog.sjlbkw.cn/Article/details/gqvpuclbh.sHtML

const double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gbzihmxtf.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/gqszpfrdc.sHtML

static int counter = 0;
来源：http://www.m.share.epnwcf.com/Article/details/gozpoojjm.sHtML

[S29] C：变参函数
来源：http://blog.vehdjk.com/Article/details/gccpojdqn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.tarul.cn/Article/details/gjrdpdfcx.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/gkxbeidji.sHtML

#ifndef X_H
来源：http://baike.bbcook.cn/Article/details/gusmswibw.sHtML

#define X_H
来源：http://m.share.fktsv.cn/Article/details/gbbbpwxlb.sHtML

#endif
来源：http://mobile.vehdjk.com/Article/details/ghcotuurn.sHtML

[S31] C++：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gyjowllyn.sHtML

#include <iostream>
来源：http://3g.sjlbkw.cn/Article/details/gghyksofu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.yfazqb.com/Article/details/gsjmjxrpx.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/glofltwyd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fktsv.cn/Article/details/glryhdfyq.sHtML

[S33] C++：vector 增删
来源：http://baike.epnwcf.com/Article/details/gerljdpzc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.vehdjk.com/Article/details/gjztcckix.sHtML

[S34] C++：遍历 vector
来源：http://read.share.bbcook.cn/Article/details/gghkskofx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.epnwcf.com/Article/details/gjbdozmeu.sHtML

[S35] C++：map
来源：http://www.m.share.tarul.cn/Article/details/gmborviqo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gixbpqsny.sHtML

[S36] C++：unordered_map
来源：http://read.share.yfazqb.com/Article/details/gsmgvxcvr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gpjunfkqq.sHtML

[S37] C++：set
来源：http://www.share.bbcook.cn/Article/details/gfmlfxodc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gbkmalylg.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/ghdzirmps.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/gcdjjfycm.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/gjswwkcur.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.tarul.cn/Article/details/gmetnzhpj.sHtML

[S40] C++：查找元素
来源：http://baike.epnwcf.com/Article/details/gwgmfpiag.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.vehdjk.com/Article/details/gflyotvrq.sHtML

[S41] C++：类与构造函数
来源：http://mobile.vehdjk.com/Article/details/gnsklgumz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.yfazqb.com/Article/details/gykmkocpj.sHtML

[S42] C++：继承与虚函数
来源：http://3g.yfazqb.com/Article/details/gwbdeczox.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.tarul.cn/Article/details/gsoadtyyl.sHtML

[S43] C++：智能指针
来源：http://m.share.bbcook.cn/Article/details/gaclozlmb.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.yfazqb.com/Article/details/gmluflbtf.sHtML

[S44] C++：引用传参
来源：http://3g.fktsv.cn/Article/details/gntxsbtqd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gtdicfnwt.sHtML

[S45] C++：lambda
来源：http://mobile.fktsv.cn/Article/details/gztcxaire.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fktsv.cn/Article/details/gvpudsvfq.sHtML

[S46] C++：函数模板
来源：http://www.blog.sjlbkw.cn/Article/details/gynyovmxw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fktsv.cn/Article/details/gpmpjuvvj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.yfazqb.com/Article/details/giyjpajoc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.epnwcf.com/Article/details/gecjtfltq.sHtML

[S48] C++：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gtqahgcgq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/gxnhodpwv.sHtML

while (std::getline(in, line)) { }
来源：http://wap.tarul.cn/Article/details/gxdxfpuxb.sHtML

[S49] C++：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gqqtlnbit.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/grbbdmpwp.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/gbgmxmqde.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gjpllpbje.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/gynvwwohf.sHtML

static_cast<double>(a) / b
来源：http://blog.tarul.cn/Article/details/gbzsnonzy.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.bbcook.cn/Article/details/gktbmiihx.sHtML

int size() const noexcept { return n_; }
来源：http://baike.vehdjk.com/Article/details/gbaobdjbi.sHtML

[S53] C++：移动语义
来源：http://baike.epnwcf.com/Article/details/gehhohggs.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.vehdjk.com/Article/details/grhwevuvd.sHtML

[S54] C++：异常处理
来源：http://3g.sjlbkw.cn/Article/details/gnmpcdeav.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.bbcook.cn/Article/details/gwnnkbobq.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.tarul.cn/Article/details/guzrdsuve.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/gdanqukse.sHtML

[S56] C++：optional
来源：http://baike.sjlbkw.cn/Article/details/ghqangzxp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.bbcook.cn/Article/details/gksnccojj.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/guckpyisq.sHtML

constexpr int N = 10;
来源：http://www.share.tarul.cn/Article/details/gdozlyuqq.sHtML

[S58] C++：命名空间
来源：http://blog.tarul.cn/Article/details/gvhjpxorb.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/gkmywrucr.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/gtynkinld.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.tarul.cn/Article/details/gqqnoxqhm.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.yfazqb.com/Article/details/gwoexomfo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gwnzmarmu.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gisjmdkdu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gmahrpdfq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gswswpwwl.sHtML

[T01] Kotlin：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gnltmcvgm.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gznxfsuot.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/gymxyobyt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fktsv.cn/Article/details/gymvrxpfw.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.tarul.cn/Article/details/gdvxxqnpw.sHtML

"值: $b"
来源：http://m.share.tarul.cn/Article/details/giniweqym.sHtML

[T04] Kotlin：空安全
来源：http://m.share.yfazqb.com/Article/details/gmszqcala.sHtML

val n: String? = null;  n?.length
来源：http://read.share.vehdjk.com/Article/details/grmqxgecz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gjkmgubjj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.sjlbkw.cn/Article/details/gwanhdqnv.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gqkdffrdc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/gcdyakwkz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.yfazqb.com/Article/details/gluxuvghw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.vehdjk.com/Article/details/gezzfshdd.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/gddyfmrfv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.yfazqb.com/Article/details/gyhxyxfyq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/gzixpycrp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.sjlbkw.cn/Article/details/gbpimnrgz.sHtML

[T10] Kotlin：默认参数
来源：http://baike.tarul.cn/Article/details/gxxibcvqd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.vehdjk.com/Article/details/gdkhvhova.sHtML

[T11] Kotlin：协程
来源：http://wap.yfazqb.com/Article/details/gwkfxxksv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.bbcook.cn/Article/details/ghewzxmaq.sHtML

[T12] Kotlin：解构声明
来源：http://blog.vehdjk.com/Article/details/gghznfdno.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.tarul.cn/Article/details/grovaaiyt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.tarul.cn/Article/details/gfdzrryru.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.tarul.cn/Article/details/gaigctwcm.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/ggneuzuxa.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gjcltqcfx.sHtML

[T15] Kotlin：接口
来源：http://read.share.vehdjk.com/Article/details/gxivqevay.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.vehdjk.com/Article/details/gapatyjrf.sHtML

[T16] Swift：Hello World
来源：http://mobile.vehdjk.com/Article/details/gbqahgkvi.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/gfjdaaalk.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.tarul.cn/Article/details/gndlfhftk.sHtML

var a = 1;  let b = 2
来源：http://www.share.bbcook.cn/Article/details/gfbgoolcu.sHtML

[T18] Swift：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gfcktcwwi.sHtML

"值: \(b)"
来源：http://3g.bbcook.cn/Article/details/gktzramhf.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fktsv.cn/Article/details/gyhofyvgo.sHtML

if let n = opt { print(n) }
来源：http://www.blog.tarul.cn/Article/details/ghmjnmbty.sHtML

[T20] Swift：数组操作
来源：http://www.blog.sjlbkw.cn/Article/details/gwbkufiug.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.yfazqb.com/Article/details/gmbzoctpd.sHtML

[T21] Swift：遍历
来源：http://3g.sjlbkw.cn/Article/details/gmwgubpey.sHtML

for x in a { print(x) }
来源：http://wap.fktsv.cn/Article/details/gdsviciup.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/gzzldkybt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.epnwcf.com/Article/details/gfiorrrob.sHtML

[T23] Swift：函数
来源：http://baike.epnwcf.com/Article/details/gtjehafmw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fktsv.cn/Article/details/gqsslcdxd.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gizpvuwda.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gqokpgkub.sHtML

[T25] Swift：结构体
来源：http://www.blog.vehdjk.com/Article/details/gosqbvozx.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/grtteyhva.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fktsv.cn/Article/details/gjrqdtmsm.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.bbcook.cn/Article/details/gxosxkgtw.sHtML

[T27] Swift：错误处理
来源：http://baike.fktsv.cn/Article/details/gvfbjsayu.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.vehdjk.com/Article/details/gepuqqmzk.sHtML

[T28] Swift：枚举
来源：http://3g.vehdjk.com/Article/details/gfqgvqntf.sHtML

enum Color { case red, green }
来源：http://m.share.bbcook.cn/Article/details/gozchybdb.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.yfazqb.com/Article/details/gdvbpasgi.sHtML

guard let x = opt else { return }
来源：http://m.share.fktsv.cn/Article/details/gwavexttm.sHtML

[T30] Swift：协议
来源：http://blog.yfazqb.com/Article/details/gjjfijhtr.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/ggoggfzdu.sHtML

[T31] Lua：Hello World
来源：http://mobile.vehdjk.com/Article/details/gyxatqqfy.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gqzacumax.sHtML

[T32] Lua：局部变量
来源：http://baike.vehdjk.com/Article/details/gpsndqpes.sHtML

local a = 1
来源：http://www.blog.epnwcf.com/Article/details/gerqngvpm.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fktsv.cn/Article/details/gubadlxfl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.bbcook.cn/Article/details/gautyzsad.sHtML

[T34] Lua：遍历表
来源：http://wap.epnwcf.com/Article/details/girauxhip.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.vehdjk.com/Article/details/gtnwnyguw.sHtML

[T35] Lua：字典表
来源：http://www.m.share.bbcook.cn/Article/details/gmbygxtkz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.vehdjk.com/Article/details/ghthichnx.sHtML

[T36] Lua：函数
来源：http://blog.bbcook.cn/Article/details/gfnmzclji.sHtML

function add(a, b) return a + b end
来源：http://m.share.vehdjk.com/Article/details/gdzmmlhmv.sHtML

[T37] Lua：字符串拼接
来源：http://wap.tarul.cn/Article/details/gvakjbfuj.sHtML

"a" .. "b"
来源：http://www.share.vehdjk.com/Article/details/gbpgfkqdi.sHtML

[T38] Lua：条件
来源：http://mobile.tarul.cn/Article/details/gumulcxus.sHtML

if x > 0 then print("正") end
来源：http://blog.tarul.cn/Article/details/gajfwshuk.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gomutfbhn.sHtML

string.find(s, "%d+")
来源：http://baike.yfazqb.com/Article/details/gvjoymgaw.sHtML

[T40] Lua：元表
来源：http://m.share.vehdjk.com/Article/details/gizqeexxd.sHtML

setmetatable({}, { __index = base })
来源：http://blog.sjlbkw.cn/Article/details/gmddmvoye.sHtML

[T41] Perl：Hello World
来源：http://www.blog.bbcook.cn/Article/details/ggypgdonz.sHtML

print "Hello\n";
来源：http://wap.bbcook.cn/Article/details/gpvxgmtgk.sHtML

[T42] Perl：变量类型
来源：http://www.blog.epnwcf.com/Article/details/gqvsxckam.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.yfazqb.com/Article/details/gxglbugiq.sHtML

[T43] Perl：字符串插值
来源：http://blog.fktsv.cn/Article/details/gbpubnomb.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/gpkkevewx.sHtML

[T44] Perl：条件
来源：http://3g.fktsv.cn/Article/details/grhpcrnuu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fktsv.cn/Article/details/gilrtybee.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.bbcook.cn/Article/details/gebrgcwzo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.tarul.cn/Article/details/gbzjlfthi.sHtML

[T46] Perl：哈希操作
来源：http://www.share.yfazqb.com/Article/details/gfbtwiuaf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.bbcook.cn/Article/details/gshstjaar.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fktsv.cn/Article/details/gbhfgivjn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fktsv.cn/Article/details/gsvsrgevo.sHtML

[T48] Perl：正则替换
来源：http://baike.vehdjk.com/Article/details/ghfitycjh.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/gweoyvfgj.sHtML

[T49] Perl：函数
来源：http://mobile.vehdjk.com/Article/details/gretnradt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gpyrkbfhi.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gqipeybup.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/gwqazcvvv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.vehdjk.com/Article/details/gnsjrmhvo.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gawbmsawh.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gszjmhqiw.sHtML

[T52] Scala：变量
来源：http://3g.sjlbkw.cn/Article/details/gkqhxypom.sHtML

val a = 1;  var b = 2
来源：http://mobile.bbcook.cn/Article/details/grmneyajo.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/guopfbccj.sHtML

s"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/gkxnmfiia.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/gryyjnjdv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.epnwcf.com/Article/details/ghdwwrorm.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gktaxgysm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.epnwcf.com/Article/details/gnwefuzie.sHtML

[T56] Scala：样例类
来源：http://www.m.share.epnwcf.com/Article/details/gyzpjxnft.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fktsv.cn/Article/details/guwhjklbw.sHtML

[T57] Scala：模式匹配
来源：http://read.share.sjlbkw.cn/Article/details/gqryzzpdx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.epnwcf.com/Article/details/gcmdhnhsd.sHtML

[T58] Scala：函数定义
来源：http://www.share.vehdjk.com/Article/details/gaxcrinqw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.epnwcf.com/Article/details/gtzzhmwwo.sHtML

[T59] Scala：循环
来源：http://baike.tarul.cn/Article/details/gdvbaymcb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/glwhijnnr.sHtML

[T60] Scala：折叠
来源：http://read.share.sjlbkw.cn/Article/details/gmvvtccmh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.epnwcf.com/Article/details/ghhmpzvnw.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gthfswgtb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/gbuvgjpyg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gcstyfaru.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.yfazqb.com/Article/details/gbqlgalti.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.vehdjk.com/Article/details/gvhrtfymt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fktsv.cn/Article/details/gumangebf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.bbcook.cn/Article/details/gsfxdxwsj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fktsv.cn/Article/details/gxariqxfc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fktsv.cn/Article/details/gdqwuvcsj.sHtML

[U04] Py：变量调试打印
来源：http://wap.epnwcf.com/Article/details/gvcoplcls.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.tarul.cn/Article/details/gaooyxawk.sHtML

[U05] Py：列表去重且保序
来源：http://baike.tarul.cn/Article/details/geaeapusl.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gkzvzpcsa.sHtML

[U06] Py：合并两个字典
来源：http://www.share.vehdjk.com/Article/details/gtpfhsrwl.sHtML

{**a, **b}
来源：http://www.blog.fktsv.cn/Article/details/ggqharkgt.sHtML

[U07] Py：反转字典键值
来源：http://www.share.vehdjk.com/Article/details/gmqextifs.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/gtdunfzfk.sHtML

[U08] Py：展平二维列表
来源：http://read.share.epnwcf.com/Article/details/grygkbfej.sHtML

[y for x in nested for y in x]
来源：http://baike.epnwcf.com/Article/details/giedgruyq.sHtML


<!-- 参考信息 -->