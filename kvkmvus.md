代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.vehdjk.com/Article/details/gpqtcfava.sHtML

[R72] 等待端口就绪
来源：http://baike.vehdjk.com/Article/details/ginrtqxvd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gvetkvrcm.sHtML

[R73] 分割大日志
来源：http://m.share.yfazqb.com/Article/details/gvycqqdjk.sHtML

split -l 1000 big.log part_
来源：http://3g.fktsv.cn/Article/details/gwfcpigqi.sHtML

[R74] 批量重命名
来源：http://3g.yfazqb.com/Article/details/gotzsfsng.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.sjlbkw.cn/Article/details/gcpzjdpob.sHtML

[R75] 导出环境变量
来源：http://www.share.epnwcf.com/Article/details/gleouezpi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/gqitupegp.sHtML

[R76] 使用临时文件
来源：http://read.share.vehdjk.com/Article/details/gjxwskumy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gehlhwybm.sHtML

[R77] 读取用户输入
来源：http://m.share.bbcook.cn/Article/details/gouyxpzkk.sHtML

read -rp "请输入: " ans
来源：http://www.share.fktsv.cn/Article/details/gkiynqrtx.sHtML

[R78] 交互式菜单
来源：http://www.share.fktsv.cn/Article/details/gmnjpiggi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.yfazqb.com/Article/details/ghjjlligr.sHtML

[R79] 解析命令行选项
来源：http://read.share.sjlbkw.cn/Article/details/gaxfxobkp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.vehdjk.com/Article/details/gajubthrc.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fktsv.cn/Article/details/gmmkxmpjw.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/grlehtzva.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gpdkkkvel.sHtML

S. C / C++ 专题
来源：http://wap.fktsv.cn/Article/details/gjnqokqoq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gikcikbnh.sHtML

[S01] C：Hello World
来源：http://baike.yfazqb.com/Article/details/gmlttgnzw.sHtML

#include <stdio.h>
来源：http://blog.fktsv.cn/Article/details/gpchgixvp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.vehdjk.com/Article/details/gnwhxdkzn.sHtML

[S02] C：变量与格式化输出
来源：http://baike.yfazqb.com/Article/details/guhmyncoj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.vehdjk.com/Article/details/ggrqxvheq.sHtML

[S03] C：读入整数
来源：http://mobile.sjlbkw.cn/Article/details/gefyacczj.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/gcczvfbaz.sHtML

[S04] C：字符串复制
来源：http://mobile.yfazqb.com/Article/details/gsknrlghu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.vehdjk.com/Article/details/ghmvpmgjy.sHtML

[S05] C：字符串长度
来源：http://read.share.yfazqb.com/Article/details/gmxkzcnlm.sHtML

strlen(s)
来源：http://m.share.epnwcf.com/Article/details/glvumyskx.sHtML

[S06] C：字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gflnckldj.sHtML

strcmp(a, b) == 0
来源：http://m.share.bbcook.cn/Article/details/gsblrhbrb.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/ghfucxeqz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/gfsogxmlc.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.tarul.cn/Article/details/gupgjprdn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.epnwcf.com/Article/details/gcaletgyd.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.yfazqb.com/Article/details/gtbzkrdex.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.bbcook.cn/Article/details/gcwdxjkum.sHtML

[S10] C：指针与解引用
来源：http://m.share.bbcook.cn/Article/details/gkcjmwlax.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/gjbgkyczj.sHtML

[S11] C：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gpahxlxcr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.tarul.cn/Article/details/gsvagnsut.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fktsv.cn/Article/details/gqbapnnxu.sHtML

fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gmujscvgw.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/ghrmhnukw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gqvrmzuxe.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/gsduocsiz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gbltfaifh.sHtML

[S14] C：枚举
来源：http://blog.fktsv.cn/Article/details/gnlatdelr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.bbcook.cn/Article/details/gyfgrxtwd.sHtML

[S15] C：类型转换
来源：http://wap.vehdjk.com/Article/details/gsmtzgblo.sHtML

(double) a / b
来源：http://www.share.bbcook.cn/Article/details/gpnpgvziq.sHtML

[S16] C：位操作置位
来源：http://blog.bbcook.cn/Article/details/gkegfpyjs.sHtML

x |= (1 << 3);
来源：http://mobile.epnwcf.com/Article/details/gpxtjwife.sHtML

[S17] C：安全拼接字符串
来源：http://baike.epnwcf.com/Article/details/gpkhdxrrw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.yfazqb.com/Article/details/gfvokvctn.sHtML

[S18] C：命令行参数
来源：http://3g.vehdjk.com/Article/details/gnrlxjueb.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/gyeiwvmkc.sHtML

[S19] C：快速排序
来源：http://blog.bbcook.cn/Article/details/gwcptnnta.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gaedcgzon.sHtML

[S20] C：二分查找
来源：http://www.m.share.yfazqb.com/Article/details/gwykoetth.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gbuvgosls.sHtML

[S21] C：字符类别判断
来源：http://read.share.bbcook.cn/Article/details/gtbqrrtap.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.epnwcf.com/Article/details/gdzpiuuji.sHtML

[S22] C：字符串转数字
来源：http://read.share.epnwcf.com/Article/details/gqwknhluf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcqttyov.sHtML

[S23] C：随机数
来源：http://baike.tarul.cn/Article/details/gpnlzsniu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gmlklfvjw.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/gmsxegacu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.vehdjk.com/Article/details/grmeipgnm.sHtML

[S25] C：内存拷贝
来源：http://www.blog.bbcook.cn/Article/details/geoasaadt.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/gypjoshgq.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/gtrcwopiq.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/gkuyqzsvs.sHtML

[S27] C：定义常量
来源：http://baike.tarul.cn/Article/details/gavnirfkq.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gvhumnkpc.sHtML

[S28] C：静态变量
来源：http://m.share.bbcook.cn/Article/details/gbpoxfmpq.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gandehdpg.sHtML

[S29] C：变参函数
来源：http://www.m.share.vehdjk.com/Article/details/gupkrcdif.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.vehdjk.com/Article/details/gzhenimpk.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gytmretgk.sHtML

#ifndef X_H
来源：http://read.share.bbcook.cn/Article/details/gxwcguqrh.sHtML

#define X_H
来源：http://www.share.bbcook.cn/Article/details/gwktgunjs.sHtML

#endif
来源：http://blog.bbcook.cn/Article/details/gnlcrfpuq.sHtML

[S31] C++：Hello World
来源：http://blog.bbcook.cn/Article/details/godyjsyqm.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gpzxzkzgb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.epnwcf.com/Article/details/gdornvqba.sHtML

[S32] C++：字符串
来源：http://www.share.epnwcf.com/Article/details/gsfhodvgf.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.bbcook.cn/Article/details/gutataunm.sHtML

[S33] C++：vector 增删
来源：http://3g.epnwcf.com/Article/details/ggvrnctnz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.bbcook.cn/Article/details/geivppono.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.vehdjk.com/Article/details/guewrzpac.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.epnwcf.com/Article/details/gxbygqvnj.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gnrcefibc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gkxqblsgz.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/gjecwvuak.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gztpzsdzc.sHtML

[S37] C++：set
来源：http://www.share.epnwcf.com/Article/details/gngabreda.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.bbcook.cn/Article/details/gmwrnrpru.sHtML

[S38] C++：排序
来源：http://www.share.fktsv.cn/Article/details/glatlvdgp.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.yfazqb.com/Article/details/gpywvczqi.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.epnwcf.com/Article/details/gjwbmsqzi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.vehdjk.com/Article/details/gijrximat.sHtML

[S40] C++：查找元素
来源：http://blog.bbcook.cn/Article/details/gfsjxvmmh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.epnwcf.com/Article/details/gcqycsosd.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/gwrcrrozd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.tarul.cn/Article/details/gcrtepgcb.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/gjpvtlsnw.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.bbcook.cn/Article/details/gaaqwtkfb.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqnzzquf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.vehdjk.com/Article/details/gwsxhbvuc.sHtML

[S44] C++：引用传参
来源：http://blog.sjlbkw.cn/Article/details/gpivugkfd.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gttkiglpu.sHtML

[S45] C++：lambda
来源：http://wap.sjlbkw.cn/Article/details/gykchazkz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.bbcook.cn/Article/details/gqvbpaakc.sHtML

[S46] C++：函数模板
来源：http://www.share.yfazqb.com/Article/details/gwkqsvpdc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/gbugjbwhx.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.bbcook.cn/Article/details/gieltttkd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.epnwcf.com/Article/details/gznietvvk.sHtML

[S48] C++：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gdemwtnsz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.yfazqb.com/Article/details/gfzizxdmf.sHtML

while (std::getline(in, line)) { }
来源：http://blog.bbcook.cn/Article/details/grednieib.sHtML

[S49] C++：写文件
来源：http://blog.epnwcf.com/Article/details/gpwkmlahw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.vehdjk.com/Article/details/ghnvbkygb.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/gndoaaphz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.vehdjk.com/Article/details/gyrnlfmvl.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/ghvqxmipi.sHtML

static_cast<double>(a) / b
来源：http://baike.vehdjk.com/Article/details/gpjyssmnq.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.sjlbkw.cn/Article/details/gvdvfrmdv.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.vehdjk.com/Article/details/gcakrhoeg.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/gtlzlfrdd.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.epnwcf.com/Article/details/gecydlxme.sHtML

[S54] C++：异常处理
来源：http://m.share.tarul.cn/Article/details/gjafkzgbk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.bbcook.cn/Article/details/gkhterysf.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.vehdjk.com/Article/details/gzcnlokzp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.yfazqb.com/Article/details/gleskedzo.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/geswwstjf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.vehdjk.com/Article/details/gzgnfcqwk.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.yfazqb.com/Article/details/gbcgzupmp.sHtML

constexpr int N = 10;
来源：http://m.share.yfazqb.com/Article/details/gzgbtiddh.sHtML

[S58] C++：命名空间
来源：http://mobile.tarul.cn/Article/details/grsbscotp.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.vehdjk.com/Article/details/gulvejkwv.sHtML

[S59] C++：静态断言
来源：http://wap.yfazqb.com/Article/details/gzciszlui.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.tarul.cn/Article/details/giozsdtiv.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.bbcook.cn/Article/details/gtiazwvom.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.vehdjk.com/Article/details/gbbepqghy.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxtojpkjv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/gitlwfors.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyalxosuz.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.bbcook.cn/Article/details/geatuvxvs.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/gzknvfdkj.sHtML

[T02] Kotlin：变量
来源：http://baike.yfazqb.com/Article/details/gusehgppj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.sjlbkw.cn/Article/details/gquskezqi.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.epnwcf.com/Article/details/gppnaksbc.sHtML

"值: $b"
来源：http://read.share.vehdjk.com/Article/details/gszhvagea.sHtML

[T04] Kotlin：空安全
来源：http://m.share.tarul.cn/Article/details/gyxfbvgwx.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/gpdwxzgsr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.epnwcf.com/Article/details/gschgdhvp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.yfazqb.com/Article/details/gwwddimvt.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fktsv.cn/Article/details/gmrhpyttg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fktsv.cn/Article/details/gucrfplwt.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gkykcwxsq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.yfazqb.com/Article/details/gfpwfwaho.sHtML

[T08] Kotlin：数据类
来源：http://www.share.bbcook.cn/Article/details/grcuhvkul.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.yfazqb.com/Article/details/gnzlrdhzk.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/gullognyg.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fktsv.cn/Article/details/gnddroplx.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.vehdjk.com/Article/details/gyzweyhez.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.bbcook.cn/Article/details/gbafmjgwm.sHtML

[T11] Kotlin：协程
来源：http://www.share.yfazqb.com/Article/details/gicaismmb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.bbcook.cn/Article/details/gcgievvlv.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gmztfzwei.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gojxuuvgd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.bbcook.cn/Article/details/guilmdfzf.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fktsv.cn/Article/details/gefftbrnk.sHtML

[T14] Kotlin：循环
来源：http://3g.vehdjk.com/Article/details/gxidxjudq.sHtML

for (i in 1..10) println(i)
来源：http://baike.vehdjk.com/Article/details/gjpdbuweb.sHtML

[T15] Kotlin：接口
来源：http://wap.fktsv.cn/Article/details/gkysjbire.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.sjlbkw.cn/Article/details/gexjnqnix.sHtML

[T16] Swift：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gffmgouir.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gnfqoidlu.sHtML

[T17] Swift：变量与常量
来源：http://wap.vehdjk.com/Article/details/gujydxpsi.sHtML

var a = 1;  let b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gdmeomlyd.sHtML

[T18] Swift：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gydwjcqxn.sHtML

"值: \(b)"
来源：http://www.blog.fktsv.cn/Article/details/ginnmzxzf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.vehdjk.com/Article/details/glfxhijvg.sHtML

if let n = opt { print(n) }
来源：http://www.blog.bbcook.cn/Article/details/gzrbggcol.sHtML

[T20] Swift：数组操作
来源：http://read.share.bbcook.cn/Article/details/gxluburue.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.epnwcf.com/Article/details/gkkwfspeh.sHtML

[T21] Swift：遍历
来源：http://wap.fktsv.cn/Article/details/gghsklzyt.sHtML

for x in a { print(x) }
来源：http://baike.bbcook.cn/Article/details/gelxhjzvb.sHtML

[T22] Swift：字典
来源：http://baike.epnwcf.com/Article/details/goarufjkg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.sjlbkw.cn/Article/details/geilqwzhe.sHtML

[T23] Swift：函数
来源：http://wap.sjlbkw.cn/Article/details/gchfhoova.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.sjlbkw.cn/Article/details/gvgzwbrhh.sHtML

[T24] Swift：闭包
来源：http://www.m.share.tarul.cn/Article/details/gsfupmzvj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.bbcook.cn/Article/details/gsalxkmgm.sHtML

[T25] Swift：结构体
来源：http://baike.bbcook.cn/Article/details/ggffrxwxc.sHtML

struct P { var x: Int }
来源：http://read.share.vehdjk.com/Article/details/gyqgimslr.sHtML

[T26] Swift：类与重写
来源：http://wap.tarul.cn/Article/details/gafsduxic.sHtML

class A: Base { override func f() {} }
来源：http://3g.yfazqb.com/Article/details/gvsttcnjn.sHtML

[T27] Swift：错误处理
来源：http://baike.bbcook.cn/Article/details/grapptiee.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.vehdjk.com/Article/details/gdldgzzdf.sHtML

[T28] Swift：枚举
来源：http://3g.fktsv.cn/Article/details/ggxkfllnd.sHtML

enum Color { case red, green }
来源：http://3g.bbcook.cn/Article/details/genlbfygg.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.sjlbkw.cn/Article/details/gsldrrqef.sHtML

guard let x = opt else { return }
来源：http://3g.vehdjk.com/Article/details/gqrctepdh.sHtML

[T30] Swift：协议
来源：http://mobile.bbcook.cn/Article/details/gjhrmxhrt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/ggzkxpzso.sHtML

[T31] Lua：Hello World
来源：http://wap.epnwcf.com/Article/details/gfpkaziuc.sHtML

print("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gztgeaemb.sHtML

[T32] Lua：局部变量
来源：http://read.share.yfazqb.com/Article/details/gyvpghark.sHtML

local a = 1
来源：http://blog.fktsv.cn/Article/details/gjqiyjnhc.sHtML

[T33] Lua：表（数组）
来源：http://m.share.yfazqb.com/Article/details/gbowozgzn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.bbcook.cn/Article/details/ggygpssfq.sHtML

[T34] Lua：遍历表
来源：http://3g.sjlbkw.cn/Article/details/gpmmkeewi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.epnwcf.com/Article/details/gqyavrouu.sHtML

[T35] Lua：字典表
来源：http://www.blog.sjlbkw.cn/Article/details/gvlrlevzm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.bbcook.cn/Article/details/ggijhopkw.sHtML

[T36] Lua：函数
来源：http://www.m.share.tarul.cn/Article/details/gwwbdlmfg.sHtML

function add(a, b) return a + b end
来源：http://www.blog.yfazqb.com/Article/details/gjjgsvhel.sHtML

[T37] Lua：字符串拼接
来源：http://3g.tarul.cn/Article/details/gyjbszuof.sHtML

"a" .. "b"
来源：http://www.m.share.epnwcf.com/Article/details/gicyoghqm.sHtML

[T38] Lua：条件
来源：http://wap.sjlbkw.cn/Article/details/gtxbklqxu.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.epnwcf.com/Article/details/gifvfotox.sHtML

[T39] Lua：模式匹配
来源：http://wap.epnwcf.com/Article/details/gqqcfvqdh.sHtML

string.find(s, "%d+")
来源：http://wap.fktsv.cn/Article/details/gqkkuwjfx.sHtML

[T40] Lua：元表
来源：http://m.share.vehdjk.com/Article/details/gldflbjxq.sHtML

setmetatable({}, { __index = base })
来源：http://blog.yfazqb.com/Article/details/gvkwerlpo.sHtML

[T41] Perl：Hello World
来源：http://read.share.yfazqb.com/Article/details/gxgamixqh.sHtML

print "Hello\n";
来源：http://www.m.share.bbcook.cn/Article/details/gdqqwcnea.sHtML

[T42] Perl：变量类型
来源：http://3g.sjlbkw.cn/Article/details/glwyxbasw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fktsv.cn/Article/details/ggvhwbzik.sHtML

[T43] Perl：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gkbazgbjf.sHtML

"值: $a"
来源：http://wap.fktsv.cn/Article/details/gsnvgtgfw.sHtML

[T44] Perl：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gfhityftg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.tarul.cn/Article/details/ggxfduuuq.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvuutlnr.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.epnwcf.com/Article/details/gvxnjygsf.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fktsv.cn/Article/details/gwibbteow.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.vehdjk.com/Article/details/gadjvvanz.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.yfazqb.com/Article/details/gbbvceciu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fktsv.cn/Article/details/ggqdvgksl.sHtML

[T48] Perl：正则替换
来源：http://wap.yfazqb.com/Article/details/gcvzycydr.sHtML

$s =~ s/old/new/g;
来源：http://3g.sjlbkw.cn/Article/details/glrtzpaax.sHtML

[T49] Perl：函数
来源：http://wap.vehdjk.com/Article/details/gyxhnzkwk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gcairftdt.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gzgtmyugq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.sjlbkw.cn/Article/details/grovzrogq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fktsv.cn/Article/details/gvuerxhkl.sHtML

[T51] Scala：Hello World
来源：http://read.share.yfazqb.com/Article/details/gjekczftv.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gdsvxshgv.sHtML

[T52] Scala：变量
来源：http://3g.yfazqb.com/Article/details/gxsmrktrn.sHtML

val a = 1;  var b = 2
来源：http://read.share.yfazqb.com/Article/details/gzjrqdzuh.sHtML

[T53] Scala：字符串插值
来源：http://blog.yfazqb.com/Article/details/gqbgolewd.sHtML

s"值: $b"
来源：http://m.share.yfazqb.com/Article/details/gtrgdeptn.sHtML

[T54] Scala：集合映射
来源：http://3g.fktsv.cn/Article/details/ggeiehbdf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.epnwcf.com/Article/details/gbhbwvhfu.sHtML

[T55] Scala：集合过滤
来源：http://read.share.epnwcf.com/Article/details/giaumscik.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpjjzjvw.sHtML

[T56] Scala：样例类
来源：http://wap.yfazqb.com/Article/details/grcnrljrc.sHtML

case class User(name: String, age: Int)
来源：http://blog.tarul.cn/Article/details/gvfnurgwa.sHtML

[T57] Scala：模式匹配
来源：http://www.share.epnwcf.com/Article/details/gksssugun.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gsvxcenkz.sHtML

[T58] Scala：函数定义
来源：http://www.share.fktsv.cn/Article/details/gifxhorjp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.sjlbkw.cn/Article/details/gnrlzpkin.sHtML

[T59] Scala：循环
来源：http://blog.fktsv.cn/Article/details/grlwojiqh.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/ggfsuvowa.sHtML

[T60] Scala：折叠
来源：http://3g.fktsv.cn/Article/details/gglhmeawx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.vehdjk.com/Article/details/gwmflwmhy.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvidsdxui.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.tarul.cn/Article/details/gxnbgabxe.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtykipxcb.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.sjlbkw.cn/Article/details/gnvoqkpgp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fktsv.cn/Article/details/gfmuuiefw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fktsv.cn/Article/details/gkontznpg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.yfazqb.com/Article/details/gqenrmops.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.yfazqb.com/Article/details/gkkssbbst.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.bbcook.cn/Article/details/gulkggwrf.sHtML

[U04] Py：变量调试打印
来源：http://blog.fktsv.cn/Article/details/gnvrfadpg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.yfazqb.com/Article/details/gbxgsonvg.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/gqhcvjsnb.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.tarul.cn/Article/details/gotecfzuf.sHtML

[U06] Py：合并两个字典
来源：http://3g.yfazqb.com/Article/details/gepbdyrxo.sHtML

{**a, **b}
来源：http://www.share.epnwcf.com/Article/details/gkhdfnxla.sHtML

[U07] Py：反转字典键值
来源：http://m.share.sjlbkw.cn/Article/details/ghjrzwmer.sHtML

{v: k for k, v in d.items()}
来源：http://3g.yfazqb.com/Article/details/grmkjpdmb.sHtML

[U08] Py：展平二维列表
来源：http://3g.tarul.cn/Article/details/gakjndaky.sHtML

[y for x in nested for y in x]
来源：http://www.blog.bbcook.cn/Article/details/gfwwuitwc.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.epnwcf.com/Article/details/geqkewioa.sHtML

max(d, key=d.get)
来源：http://www.share.vehdjk.com/Article/details/grdcxukhd.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.yfazqb.com/Article/details/gbvudyrtj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.vehdjk.com/Article/details/gjqistqdy.sHtML

[U11] Py：生成器表达式
来源：http://blog.sjlbkw.cn/Article/details/gggxdyfpg.sHtML

(x * 2 for x in arr)
来源：http://mobile.sjlbkw.cn/Article/details/gewqpquci.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fktsv.cn/Article/details/ggymflyfj.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fktsv.cn/Article/details/gqswmputn.sHtML


<!-- 参考信息 -->