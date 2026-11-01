代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/glgnumlru.sHtML

[R70] 时间戳与互转
来源：http://3g.bbcook.cn/Article/details/gryllghpe.sHtML

date +%s;  date -d @1700000000
来源：http://blog.yfazqb.com/Article/details/gjlnfeeci.sHtML

[R71] 日期格式化
来源：http://wap.tarul.cn/Article/details/gtqmqzjli.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.sjlbkw.cn/Article/details/gzkkgzokv.sHtML

[R72] 等待端口就绪
来源：http://m.share.sjlbkw.cn/Article/details/gskujekww.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gmwxhfjlu.sHtML

[R73] 分割大日志
来源：http://read.share.yfazqb.com/Article/details/ggjezhrzg.sHtML

split -l 1000 big.log part_
来源：http://www.blog.bbcook.cn/Article/details/gexuoqsxm.sHtML

[R74] 批量重命名
来源：http://3g.epnwcf.com/Article/details/gukfwjvxl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.sjlbkw.cn/Article/details/gemocvdex.sHtML

[R75] 导出环境变量
来源：http://www.share.sjlbkw.cn/Article/details/grbmegzsc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.tarul.cn/Article/details/gczstrkyw.sHtML

[R76] 使用临时文件
来源：http://m.share.vehdjk.com/Article/details/gddtqwyxv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkpveuun.sHtML

[R77] 读取用户输入
来源：http://www.blog.tarul.cn/Article/details/gjdtbznja.sHtML

read -rp "请输入: " ans
来源：http://m.share.bbcook.cn/Article/details/gblvatkyl.sHtML

[R78] 交互式菜单
来源：http://m.share.sjlbkw.cn/Article/details/gtcokcngi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.vehdjk.com/Article/details/gbtuuuxri.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.yfazqb.com/Article/details/gfbxvihbn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.epnwcf.com/Article/details/gwrehjoyn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/gwtptdmpz.sHtML

time ./run.sh
来源：http://www.m.share.epnwcf.com/Article/details/gtlkagunj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glxuhgjmo.sHtML

S. C / C++ 专题
来源：http://3g.fktsv.cn/Article/details/gtudgkvyx.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggqbvrnkx.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/ggpbqgwyx.sHtML

#include <stdio.h>
来源：http://www.share.epnwcf.com/Article/details/gamsfxzxc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.bbcook.cn/Article/details/gcqqafeyv.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.yfazqb.com/Article/details/gwcraagtk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.tarul.cn/Article/details/gjxcdvhjc.sHtML

[S03] C：读入整数
来源：http://baike.sjlbkw.cn/Article/details/gntxxxctj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.vehdjk.com/Article/details/gwreppbbi.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/gmaodgtlz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.epnwcf.com/Article/details/gxsmznzbp.sHtML

[S05] C：字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gmrsrkujq.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gnrzxvsmg.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gdbcutpfe.sHtML

strcmp(a, b) == 0
来源：http://wap.epnwcf.com/Article/details/gkrrfsmnb.sHtML

[S07] C：数组遍历求和
来源：http://m.share.vehdjk.com/Article/details/gqbbtrntr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.epnwcf.com/Article/details/gxqtcrjsm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.bbcook.cn/Article/details/gjdfnuxju.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/genetgxuw.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.yfazqb.com/Article/details/gfwfhvlvp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.bbcook.cn/Article/details/ghbpdoplx.sHtML

[S10] C：指针与解引用
来源：http://blog.tarul.cn/Article/details/gefbrgumb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.yfazqb.com/Article/details/gzymiipxp.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gedrvezoc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fktsv.cn/Article/details/gucredsah.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.yfazqb.com/Article/details/gsqaxdqas.sHtML

fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gvpbnddzw.sHtML

[S12] C：写文件
来源：http://read.share.epnwcf.com/Article/details/gjcnzojke.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gudbacqin.sHtML

[S13] C：宏定义
来源：http://blog.yfazqb.com/Article/details/gnrbktfnd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.vehdjk.com/Article/details/gxrquozra.sHtML

[S14] C：枚举
来源：http://wap.fktsv.cn/Article/details/gttanrsqn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.yfazqb.com/Article/details/gzjcuzwfi.sHtML

[S15] C：类型转换
来源：http://www.blog.tarul.cn/Article/details/glrslgdpf.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/grwgnogco.sHtML

[S16] C：位操作置位
来源：http://blog.epnwcf.com/Article/details/gpjccoveo.sHtML

x |= (1 << 3);
来源：http://mobile.bbcook.cn/Article/details/gygtyhhsp.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.tarul.cn/Article/details/gepvbtgyh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.yfazqb.com/Article/details/gduhyjexu.sHtML

[S18] C：命令行参数
来源：http://3g.yfazqb.com/Article/details/gkhclzdia.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/gzmjofqjx.sHtML

[S19] C：快速排序
来源：http://m.share.fktsv.cn/Article/details/gtulkpkyg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gjgsyxrds.sHtML

[S20] C：二分查找
来源：http://www.m.share.tarul.cn/Article/details/ghwqrahac.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gdtgvpfcu.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/gqgyzgisp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.vehdjk.com/Article/details/gynhclltc.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/gjuoncyth.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.sjlbkw.cn/Article/details/ghvwlswgx.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/gdityhlzv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.yfazqb.com/Article/details/gahqhqbwl.sHtML

[S24] C：获取本地时间
来源：http://www.share.vehdjk.com/Article/details/gcklganpa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.sjlbkw.cn/Article/details/gfscykqbx.sHtML

[S25] C：内存拷贝
来源：http://read.share.tarul.cn/Article/details/gukeayhdq.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/giweqyynl.sHtML

[S26] C：内存清零
来源：http://www.blog.epnwcf.com/Article/details/guvkkssov.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.bbcook.cn/Article/details/ghfycffli.sHtML

[S27] C：定义常量
来源：http://read.share.tarul.cn/Article/details/gtphfnret.sHtML

const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gakguuqnd.sHtML

[S28] C：静态变量
来源：http://m.share.yfazqb.com/Article/details/gozojvetz.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/gupfevxcl.sHtML

[S29] C：变参函数
来源：http://www.share.vehdjk.com/Article/details/gtsydrqbi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.epnwcf.com/Article/details/gjgqlgnvi.sHtML

[S30] C：头文件保护
来源：http://wap.fktsv.cn/Article/details/gjfwbrtck.sHtML

#ifndef X_H
来源：http://m.share.fktsv.cn/Article/details/gdmpjprzq.sHtML

#define X_H
来源：http://www.share.sjlbkw.cn/Article/details/gvkgjuxrv.sHtML

#endif
来源：http://www.share.yfazqb.com/Article/details/gqpgmngzo.sHtML

[S31] C++：Hello World
来源：http://blog.bbcook.cn/Article/details/goxsxgdbk.sHtML

#include <iostream>
来源：http://wap.epnwcf.com/Article/details/giefwezqv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/godvemdlp.sHtML

[S32] C++：字符串
来源：http://wap.yfazqb.com/Article/details/gsetrvxdv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.tarul.cn/Article/details/geollgvjo.sHtML

[S33] C++：vector 增删
来源：http://www.blog.yfazqb.com/Article/details/ggddyvfgh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fktsv.cn/Article/details/gkowgdxgf.sHtML

[S34] C++：遍历 vector
来源：http://baike.sjlbkw.cn/Article/details/gitcwfgwz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.vehdjk.com/Article/details/gebkzctiy.sHtML

[S35] C++：map
来源：http://www.m.share.vehdjk.com/Article/details/gxtqpeodj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gmuhrtzfr.sHtML

[S36] C++：unordered_map
来源：http://baike.bbcook.cn/Article/details/gfuojvopo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/gqrxnpsyf.sHtML

[S37] C++：set
来源：http://read.share.sjlbkw.cn/Article/details/gtuwnikmy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/gstsepaqx.sHtML

[S38] C++：排序
来源：http://read.share.vehdjk.com/Article/details/gnhubpeur.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.bbcook.cn/Article/details/gobpmqmve.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.yfazqb.com/Article/details/gkbidvlzi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/gjmliulkm.sHtML

[S40] C++：查找元素
来源：http://blog.yfazqb.com/Article/details/gsadpbiiy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.epnwcf.com/Article/details/glsbyxsiv.sHtML

[S41] C++：类与构造函数
来源：http://wap.tarul.cn/Article/details/garxbbyde.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.vehdjk.com/Article/details/gewffdyoh.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fktsv.cn/Article/details/gvbgdcghv.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.tarul.cn/Article/details/gqdcnecjq.sHtML

[S43] C++：智能指针
来源：http://www.share.fktsv.cn/Article/details/gramjgxtz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gnoewzozl.sHtML

[S44] C++：引用传参
来源：http://www.m.share.bbcook.cn/Article/details/ghvrtejyz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.vehdjk.com/Article/details/gyxcqouow.sHtML

[S45] C++：lambda
来源：http://www.share.bbcook.cn/Article/details/gyoqkmadv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fktsv.cn/Article/details/gkdvvejoe.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhevjnuj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.bbcook.cn/Article/details/gswozqale.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.yfazqb.com/Article/details/gjkbisuhp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.yfazqb.com/Article/details/gdegtronh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gjzygyzjb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.epnwcf.com/Article/details/gzgomjetf.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fktsv.cn/Article/details/gedwxnjbv.sHtML

[S49] C++：写文件
来源：http://baike.tarul.cn/Article/details/gjekqhhqe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.sjlbkw.cn/Article/details/gehvupqqr.sHtML

[S50] C++：格式化数字
来源：http://blog.vehdjk.com/Article/details/gyzupaxjy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.tarul.cn/Article/details/gjmgufcco.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/ggbkalktl.sHtML

static_cast<double>(a) / b
来源：http://m.share.epnwcf.com/Article/details/geebvkeue.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.yfazqb.com/Article/details/gqocitmge.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/ghzmstnvc.sHtML

[S53] C++：移动语义
来源：http://baike.bbcook.cn/Article/details/golrjnhhz.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.vehdjk.com/Article/details/gveeltsnu.sHtML

[S54] C++：异常处理
来源：http://read.share.epnwcf.com/Article/details/gzwrccikz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.tarul.cn/Article/details/ghymyslpt.sHtML

[S55] C++：结构化绑定
来源：http://3g.vehdjk.com/Article/details/gtjpvzfbj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.bbcook.cn/Article/details/ghwocmjkr.sHtML

[S56] C++：optional
来源：http://wap.tarul.cn/Article/details/glbtknubn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.epnwcf.com/Article/details/gtzqbajly.sHtML

[S57] C++：编译期常量
来源：http://mobile.bbcook.cn/Article/details/ggjqqxeaq.sHtML

constexpr int N = 10;
来源：http://3g.fktsv.cn/Article/details/gelobihcy.sHtML

[S58] C++：命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gmsideaic.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.tarul.cn/Article/details/guzhlxvty.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/gqozypbor.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.tarul.cn/Article/details/gsnwwqjcg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gwtfodydf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fktsv.cn/Article/details/gfzvvxaaq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gkgnupjdx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.yfazqb.com/Article/details/gafbufqnt.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gfbjzmazf.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gzmrkhpxg.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gmfivvvli.sHtML

[T02] Kotlin：变量
来源：http://baike.yfazqb.com/Article/details/gkxxdnlyi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.tarul.cn/Article/details/gjgcxhsgy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.yfazqb.com/Article/details/gmolelpbv.sHtML

"值: $b"
来源：http://baike.epnwcf.com/Article/details/gackgkhiz.sHtML

[T04] Kotlin：空安全
来源：http://wap.fktsv.cn/Article/details/gaxwzhrof.sHtML

val n: String? = null;  n?.length
来源：http://m.share.epnwcf.com/Article/details/gzohmzkrb.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.tarul.cn/Article/details/gxcaremyd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.tarul.cn/Article/details/gotwjpktr.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gcikvbder.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.vehdjk.com/Article/details/gcauvztoi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gdufdwmzz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.bbcook.cn/Article/details/gdpfjrmgq.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.epnwcf.com/Article/details/ghuptvhus.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/guprjoqng.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.yfazqb.com/Article/details/gioivctov.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.sjlbkw.cn/Article/details/gymuxdrru.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.epnwcf.com/Article/details/gmmvtoeqd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fktsv.cn/Article/details/glnqvfmnc.sHtML

[T11] Kotlin：协程
来源：http://blog.bbcook.cn/Article/details/gpjhxfzqc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.yfazqb.com/Article/details/gczyuuzwg.sHtML

[T12] Kotlin：解构声明
来源：http://blog.epnwcf.com/Article/details/gppdzwwzj.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gndcruzua.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.sjlbkw.cn/Article/details/glmxpyypo.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.yfazqb.com/Article/details/gbtvjarsd.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/guynxfhgh.sHtML

for (i in 1..10) println(i)
来源：http://m.share.yfazqb.com/Article/details/gzobcfgjz.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fktsv.cn/Article/details/gtvdjvxhx.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.sjlbkw.cn/Article/details/gvcvtudtq.sHtML

[T16] Swift：Hello World
来源：http://wap.tarul.cn/Article/details/gzlqkisce.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gehxynunv.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fktsv.cn/Article/details/grgocvrzj.sHtML

var a = 1;  let b = 2
来源：http://read.share.yfazqb.com/Article/details/gvtxndnfa.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/gndawihkj.sHtML

"值: \(b)"
来源：http://blog.sjlbkw.cn/Article/details/grmavyhdv.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/gtrnzmcxo.sHtML

if let n = opt { print(n) }
来源：http://www.blog.yfazqb.com/Article/details/gszvzzwqg.sHtML

[T20] Swift：数组操作
来源：http://www.blog.tarul.cn/Article/details/gnujbftji.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/gxjinzznk.sHtML

[T21] Swift：遍历
来源：http://www.share.tarul.cn/Article/details/gmcyjbmax.sHtML

for x in a { print(x) }
来源：http://3g.tarul.cn/Article/details/gvapwqllb.sHtML

[T22] Swift：字典
来源：http://blog.vehdjk.com/Article/details/gdjhyhnwa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.epnwcf.com/Article/details/gxuofzhfw.sHtML

[T23] Swift：函数
来源：http://3g.tarul.cn/Article/details/gzektower.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gezoruzcz.sHtML

[T24] Swift：闭包
来源：http://read.share.sjlbkw.cn/Article/details/ghcfpnmre.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.tarul.cn/Article/details/gpplbfgrt.sHtML

[T25] Swift：结构体
来源：http://3g.epnwcf.com/Article/details/gtsbxjqjp.sHtML

struct P { var x: Int }
来源：http://www.blog.sjlbkw.cn/Article/details/gatcnrzrc.sHtML

[T26] Swift：类与重写
来源：http://www.blog.vehdjk.com/Article/details/gnhvbjpzh.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.epnwcf.com/Article/details/gmosfnlzn.sHtML

[T27] Swift：错误处理
来源：http://m.share.epnwcf.com/Article/details/guhyohvjn.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.yfazqb.com/Article/details/gwbdphlxq.sHtML

[T28] Swift：枚举
来源：http://3g.fktsv.cn/Article/details/gkrxgakjg.sHtML

enum Color { case red, green }
来源：http://m.share.bbcook.cn/Article/details/gqadbcptm.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.tarul.cn/Article/details/gbmlykmty.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/glrzxiuhc.sHtML

[T30] Swift：协议
来源：http://wap.yfazqb.com/Article/details/gcdgrhvue.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhzodpse.sHtML

[T31] Lua：Hello World
来源：http://wap.fktsv.cn/Article/details/gfmmzcgul.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/gxegmcpni.sHtML

[T32] Lua：局部变量
来源：http://blog.tarul.cn/Article/details/gedlerbah.sHtML

local a = 1
来源：http://3g.vehdjk.com/Article/details/gwoyrmpji.sHtML

[T33] Lua：表（数组）
来源：http://wap.bbcook.cn/Article/details/gkgzdllpa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.bbcook.cn/Article/details/gtncxnxpb.sHtML

[T34] Lua：遍历表
来源：http://mobile.yfazqb.com/Article/details/gqxfmglyw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/gqwunsrhg.sHtML

[T35] Lua：字典表
来源：http://baike.bbcook.cn/Article/details/gsnzkixpc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.bbcook.cn/Article/details/gnclevmxj.sHtML

[T36] Lua：函数
来源：http://3g.vehdjk.com/Article/details/glmcncpqq.sHtML

function add(a, b) return a + b end
来源：http://blog.bbcook.cn/Article/details/gtmojvvls.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.tarul.cn/Article/details/gjeyvstcl.sHtML

"a" .. "b"
来源：http://www.blog.vehdjk.com/Article/details/ghlmhnlbw.sHtML

[T38] Lua：条件
来源：http://mobile.tarul.cn/Article/details/gcyommtgv.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.epnwcf.com/Article/details/gjsobzayj.sHtML

[T39] Lua：模式匹配
来源：http://3g.epnwcf.com/Article/details/glxqsvzga.sHtML

string.find(s, "%d+")
来源：http://www.blog.tarul.cn/Article/details/gqhgqrwlt.sHtML

[T40] Lua：元表
来源：http://wap.sjlbkw.cn/Article/details/gdimwfcwi.sHtML

setmetatable({}, { __index = base })
来源：http://3g.tarul.cn/Article/details/gtzrbyhuq.sHtML

[T41] Perl：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/genhtdtwf.sHtML

print "Hello\n";
来源：http://m.share.epnwcf.com/Article/details/gjwsodkjk.sHtML

[T42] Perl：变量类型
来源：http://www.share.tarul.cn/Article/details/guuzxnadi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.tarul.cn/Article/details/gqexgpdlz.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gmdorynqb.sHtML

"值: $a"
来源：http://m.share.vehdjk.com/Article/details/gnpmsbtdy.sHtML

[T44] Perl：条件
来源：http://read.share.epnwcf.com/Article/details/gxqzkvbbf.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.bbcook.cn/Article/details/gkjombdjk.sHtML

[T45] Perl：数组遍历
来源：http://3g.yfazqb.com/Article/details/gapliecen.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.bbcook.cn/Article/details/gybuijenm.sHtML

[T46] Perl：哈希操作
来源：http://baike.bbcook.cn/Article/details/gjwoobxqy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gttmxskjw.sHtML

[T47] Perl：正则捕获
来源：http://www.share.sjlbkw.cn/Article/details/gkfncyqwq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.sjlbkw.cn/Article/details/gtgqrwuuv.sHtML

[T48] Perl：正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gtwxwdixx.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.yfazqb.com/Article/details/gytyjmqog.sHtML

[T49] Perl：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/goxdmdvhp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/glxtszzlj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gsvvujrnz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.epnwcf.com/Article/details/grcxxbpzf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.vehdjk.com/Article/details/grsutypll.sHtML

[T51] Scala：Hello World
来源：http://blog.vehdjk.com/Article/details/gjgqanbsu.sHtML

println("Hello")
来源：http://m.share.bbcook.cn/Article/details/gemxrprot.sHtML

[T52] Scala：变量
来源：http://www.m.share.yfazqb.com/Article/details/gpivcoeav.sHtML

val a = 1;  var b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gwuerhqkl.sHtML

[T53] Scala：字符串插值
来源：http://wap.vehdjk.com/Article/details/gvghhniep.sHtML

s"值: $b"
来源：http://mobile.yfazqb.com/Article/details/ghjydhyoa.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/gccmbsovc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.vehdjk.com/Article/details/gytrutbib.sHtML

[T55] Scala：集合过滤
来源：http://3g.bbcook.cn/Article/details/gdxkcnboy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fktsv.cn/Article/details/gsrzcxlta.sHtML

[T56] Scala：样例类
来源：http://3g.fktsv.cn/Article/details/gqklfarew.sHtML

case class User(name: String, age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/ggirwgjso.sHtML

[T57] Scala：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gdtdpbhzh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fktsv.cn/Article/details/gddvcandj.sHtML

[T58] Scala：函数定义
来源：http://blog.vehdjk.com/Article/details/gvkphrzdo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.tarul.cn/Article/details/gxchozmia.sHtML

[T59] Scala：循环
来源：http://www.blog.fktsv.cn/Article/details/ghjbdbynw.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/gjgbxpzkp.sHtML

[T60] Scala：折叠
来源：http://read.share.tarul.cn/Article/details/gjuyfcznr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.bbcook.cn/Article/details/grxlxgykg.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggvudxpvf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/gpyfubsrg.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gabcjbsve.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.tarul.cn/Article/details/gmcdbqzjn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.bbcook.cn/Article/details/gffgcvqdg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.yfazqb.com/Article/details/gooxnqhft.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.yfazqb.com/Article/details/gbgjtuicd.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.epnwcf.com/Article/details/gfjvbtcjr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.tarul.cn/Article/details/gjnbapfcq.sHtML

[U04] Py：变量调试打印
来源：http://3g.fktsv.cn/Article/details/gdfhscnsr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fktsv.cn/Article/details/gezqkyebg.sHtML

[U05] Py：列表去重且保序
来源：http://baike.tarul.cn/Article/details/gvudeqgbm.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlutfxcn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.vehdjk.com/Article/details/gcgeyllic.sHtML

{**a, **b}
来源：http://m.share.tarul.cn/Article/details/glmiacddh.sHtML

[U07] Py：反转字典键值
来源：http://baike.yfazqb.com/Article/details/gehvpnlcu.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fktsv.cn/Article/details/gqbzqtvmx.sHtML

[U08] Py：展平二维列表
来源：http://mobile.bbcook.cn/Article/details/gmhmcdszl.sHtML

[y for x in nested for y in x]
来源：http://www.blog.vehdjk.com/Article/details/gdnvruddk.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.yfazqb.com/Article/details/gpeewmova.sHtML

max(d, key=d.get)
来源：http://mobile.vehdjk.com/Article/details/gjqresjsp.sHtML

[U10] Py：按值排序字典
来源：http://3g.vehdjk.com/Article/details/gavxnteas.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fktsv.cn/Article/details/gnrrcfoyc.sHtML


<!-- 参考信息 -->