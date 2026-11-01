代发 wailian999

split -l 1000 big.log part_
来源：http://baike.vehdjk.com/Article/details/gspwuajgt.sHtML

[R74] 批量重命名
来源：http://m.share.yfazqb.com/Article/details/gvzmbwjcx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.sjlbkw.cn/Article/details/gvsrvdmwr.sHtML

[R75] 导出环境变量
来源：http://blog.sjlbkw.cn/Article/details/geluqckfk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.vehdjk.com/Article/details/gwvmwzglq.sHtML

[R76] 使用临时文件
来源：http://www.share.bbcook.cn/Article/details/gkyidrqne.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/ggsnphqcv.sHtML

[R77] 读取用户输入
来源：http://read.share.bbcook.cn/Article/details/goonkpzji.sHtML

read -rp "请输入: " ans
来源：http://3g.yfazqb.com/Article/details/gthhrprqg.sHtML

[R78] 交互式菜单
来源：http://www.m.share.epnwcf.com/Article/details/gcobusuoh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/gdniafqhu.sHtML

[R79] 解析命令行选项
来源：http://blog.fktsv.cn/Article/details/grljvfixb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.yfazqb.com/Article/details/grfyxjwuq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.yfazqb.com/Article/details/gwgevrjra.sHtML

time ./run.sh
来源：http://3g.fktsv.cn/Article/details/gwyinhlqv.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwquszgia.sHtML

S. C / C++ 专题
来源：http://read.share.sjlbkw.cn/Article/details/gbgxmxwub.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gkxmpsofg.sHtML

[S01] C：Hello World
来源：http://m.share.bbcook.cn/Article/details/grqyyfhdh.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/gsrkidowi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fktsv.cn/Article/details/gfuhhztlt.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.epnwcf.com/Article/details/gpzbrsuhb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.bbcook.cn/Article/details/gabrfadoq.sHtML

[S03] C：读入整数
来源：http://wap.tarul.cn/Article/details/glogotxhk.sHtML

int x; scanf("%d", &x);
来源：http://www.share.bbcook.cn/Article/details/giimdnesq.sHtML

[S04] C：字符串复制
来源：http://3g.vehdjk.com/Article/details/gzjfegelx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.yfazqb.com/Article/details/gmcuvvqdb.sHtML

[S05] C：字符串长度
来源：http://mobile.vehdjk.com/Article/details/ghtekyrzq.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gzfiejahg.sHtML

[S06] C：字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gkpikpmmt.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gvbxdbhlv.sHtML

[S07] C：数组遍历求和
来源：http://blog.bbcook.cn/Article/details/gacmznsef.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/gejcarmbq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.yfazqb.com/Article/details/gzwyhaarn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.vehdjk.com/Article/details/govjmtvlq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/glyvrcogz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gbmuzcfip.sHtML

[S10] C：指针与解引用
来源：http://read.share.bbcook.cn/Article/details/gislbdgaw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.vehdjk.com/Article/details/gduoiehfq.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gnswzeuyt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/gnqqdwddb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.tarul.cn/Article/details/guvsvwyic.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/gczezhxwl.sHtML

[S12] C：写文件
来源：http://baike.yfazqb.com/Article/details/gqiyihzwk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gfkjterdj.sHtML

[S13] C：宏定义
来源：http://blog.yfazqb.com/Article/details/gejlqmxot.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.tarul.cn/Article/details/gmdaqqmds.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/gypsadhbd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.yfazqb.com/Article/details/gxnhpvebc.sHtML

[S15] C：类型转换
来源：http://www.blog.yfazqb.com/Article/details/ggxkijxta.sHtML

(double) a / b
来源：http://wap.bbcook.cn/Article/details/gjyjxlvid.sHtML

[S16] C：位操作置位
来源：http://read.share.tarul.cn/Article/details/gkxmmapru.sHtML

x |= (1 << 3);
来源：http://baike.fktsv.cn/Article/details/gdmzpkprj.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gxjdrmeik.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.epnwcf.com/Article/details/gglqgvqjf.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gbgygixzl.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/gghtqnnbh.sHtML

[S19] C：快速排序
来源：http://baike.tarul.cn/Article/details/goxqtqnfm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/gxyfefcrt.sHtML

[S20] C：二分查找
来源：http://read.share.bbcook.cn/Article/details/gnirkbmsz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/gkaaxpjob.sHtML

[S21] C：字符类别判断
来源：http://blog.epnwcf.com/Article/details/glssofafb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.sjlbkw.cn/Article/details/gmvahkupx.sHtML

[S22] C：字符串转数字
来源：http://m.share.fktsv.cn/Article/details/gecryykzo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.epnwcf.com/Article/details/grndpokdm.sHtML

[S23] C：随机数
来源：http://3g.bbcook.cn/Article/details/gugtlxqbu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.tarul.cn/Article/details/gfwmlzsbz.sHtML

[S24] C：获取本地时间
来源：http://www.blog.tarul.cn/Article/details/gjeaspapk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.vehdjk.com/Article/details/gtksuxigs.sHtML

[S25] C：内存拷贝
来源：http://wap.yfazqb.com/Article/details/gnuumqssq.sHtML

memcpy(dst, src, n);
来源：http://baike.tarul.cn/Article/details/gzxwdxkoz.sHtML

[S26] C：内存清零
来源：http://read.share.sjlbkw.cn/Article/details/gvibiwzsm.sHtML

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/gptuqwvvg.sHtML

[S27] C：定义常量
来源：http://www.m.share.bbcook.cn/Article/details/gcbmxrmqu.sHtML

const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gmrbqrebw.sHtML

[S28] C：静态变量
来源：http://wap.tarul.cn/Article/details/gulzirfls.sHtML

static int counter = 0;
来源：http://blog.tarul.cn/Article/details/gbmmqagdn.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/gwuuvggxq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.sjlbkw.cn/Article/details/gftqqrkzb.sHtML

[S30] C：头文件保护
来源：http://www.blog.yfazqb.com/Article/details/gjsdttyew.sHtML

#ifndef X_H
来源：http://www.m.share.epnwcf.com/Article/details/gwmonzjrw.sHtML

#define X_H
来源：http://m.share.bbcook.cn/Article/details/gecesyfqi.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gffwmhtyv.sHtML

[S31] C++：Hello World
来源：http://wap.yfazqb.com/Article/details/ghgbamvlr.sHtML

#include <iostream>
来源：http://www.blog.vehdjk.com/Article/details/gkrlhtvoa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.yfazqb.com/Article/details/gdmsgfogv.sHtML

[S32] C++：字符串
来源：http://m.share.sjlbkw.cn/Article/details/glhpeehbr.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/gvbawkvxc.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/ganlpelvg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gghidrbyy.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/ggitwydlu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gorxlsmci.sHtML

[S35] C++：map
来源：http://baike.bbcook.cn/Article/details/gmcgysnps.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gzmwbsdfd.sHtML

[S36] C++：unordered_map
来源：http://m.share.vehdjk.com/Article/details/gvvvdvehi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/gjynwdwye.sHtML

[S37] C++：set
来源：http://read.share.epnwcf.com/Article/details/gawetxqgz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.sjlbkw.cn/Article/details/glckofcie.sHtML

[S38] C++：排序
来源：http://blog.epnwcf.com/Article/details/gghfarwvv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gsycurbxh.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/gjbknznbg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/gsamrkiin.sHtML

[S40] C++：查找元素
来源：http://www.blog.fktsv.cn/Article/details/gersrdowj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/gyoexulmo.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gfuxlctdi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/gekgbzixa.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.sjlbkw.cn/Article/details/gxzdfgett.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.yfazqb.com/Article/details/gtgbdklcz.sHtML

[S43] C++：智能指针
来源：http://m.share.yfazqb.com/Article/details/gdirmowwj.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fktsv.cn/Article/details/gchtekcjc.sHtML

[S44] C++：引用传参
来源：http://3g.tarul.cn/Article/details/gqnmqwmmj.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.yfazqb.com/Article/details/gilvfabyh.sHtML

[S45] C++：lambda
来源：http://wap.tarul.cn/Article/details/gkflrosqv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.tarul.cn/Article/details/gtwtdixtj.sHtML

[S46] C++：函数模板
来源：http://www.blog.vehdjk.com/Article/details/gxtntdxzn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.bbcook.cn/Article/details/glioajzqq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.yfazqb.com/Article/details/gizgvscko.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.yfazqb.com/Article/details/gkfrpamsd.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gqfufpmyx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gosbppeju.sHtML

while (std::getline(in, line)) { }
来源：http://baike.vehdjk.com/Article/details/gohjufhsp.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/gzcbmncvn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.bbcook.cn/Article/details/gepcckzxf.sHtML

[S50] C++：格式化数字
来源：http://3g.epnwcf.com/Article/details/gqcvtmecv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gmhwfsben.sHtML

[S51] C++：显式类型转换
来源：http://baike.fktsv.cn/Article/details/gljkbponc.sHtML

static_cast<double>(a) / b
来源：http://mobile.yfazqb.com/Article/details/gikejezqj.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.tarul.cn/Article/details/gysrgtwec.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.epnwcf.com/Article/details/gltfzeefx.sHtML

[S53] C++：移动语义
来源：http://www.m.share.yfazqb.com/Article/details/gqenwpxqq.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.tarul.cn/Article/details/guvvuidab.sHtML

[S54] C++：异常处理
来源：http://wap.yfazqb.com/Article/details/geonjyjjr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.tarul.cn/Article/details/gmuhqrnih.sHtML

[S55] C++：结构化绑定
来源：http://3g.sjlbkw.cn/Article/details/gpxupxoxe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.epnwcf.com/Article/details/giubmzayg.sHtML

[S56] C++：optional
来源：http://read.share.yfazqb.com/Article/details/gzjojxyqu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmxkiavhp.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/gyvhwaihv.sHtML

constexpr int N = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gupovgkay.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gmrwheilk.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.sjlbkw.cn/Article/details/gihclrnlm.sHtML

[S59] C++：静态断言
来源：http://blog.sjlbkw.cn/Article/details/gmqbuadav.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.vehdjk.com/Article/details/gymodhhak.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.bbcook.cn/Article/details/gnkbhdjvz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.vehdjk.com/Article/details/gvgfytlhl.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gdsqmlnok.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/gfusyyoia.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gjiinlytq.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gjhdmkcwk.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/guwttnztv.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gtnyatzer.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.tarul.cn/Article/details/gbaeoqxip.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.tarul.cn/Article/details/gxpgxvmwv.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/gnvjcofke.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.sjlbkw.cn/Article/details/gwmxvkjcf.sHtML

val n: String? = null;  n?.length
来源：http://3g.epnwcf.com/Article/details/gisqfqmds.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.vehdjk.com/Article/details/gjtfusefm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/giefrleyb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.yfazqb.com/Article/details/gmnyknyhw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gggtskprm.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gupjjtfwm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.epnwcf.com/Article/details/gvygjfals.sHtML

[T08] Kotlin：数据类
来源：http://www.share.epnwcf.com/Article/details/gpeqjqibx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.vehdjk.com/Article/details/gswnzrudt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.epnwcf.com/Article/details/gdaxxbdbd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/ghesarvby.sHtML

[T10] Kotlin：默认参数
来源：http://3g.vehdjk.com/Article/details/gqdndfjeg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.yfazqb.com/Article/details/gzkwulruf.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fktsv.cn/Article/details/gyvfdorks.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.epnwcf.com/Article/details/gvgqevzyv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.yfazqb.com/Article/details/gcuwdhjip.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gnfqcbyhg.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fktsv.cn/Article/details/glkjfaavw.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.vehdjk.com/Article/details/gujlkzwod.sHtML

[T14] Kotlin：循环
来源：http://wap.fktsv.cn/Article/details/gcgisblmh.sHtML

for (i in 1..10) println(i)
来源：http://wap.vehdjk.com/Article/details/gdspxgjjl.sHtML

[T15] Kotlin：接口
来源：http://m.share.vehdjk.com/Article/details/gbgbddwdx.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.tarul.cn/Article/details/grtbdkyty.sHtML

[T16] Swift：Hello World
来源：http://www.share.tarul.cn/Article/details/gmqzlckyd.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/glfkyspba.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.tarul.cn/Article/details/gcfnbzjlb.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/gvlhdhbnw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gbemqkbyz.sHtML

"值: \(b)"
来源：http://read.share.epnwcf.com/Article/details/gdohbpowr.sHtML

[T19] Swift：可选绑定
来源：http://m.share.tarul.cn/Article/details/giuqqfvyx.sHtML

if let n = opt { print(n) }
来源：http://wap.bbcook.cn/Article/details/gmynhoasb.sHtML

[T20] Swift：数组操作
来源：http://mobile.tarul.cn/Article/details/gjwvpzqap.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/gdtodnlvu.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fktsv.cn/Article/details/gjywyxbbw.sHtML

for x in a { print(x) }
来源：http://baike.epnwcf.com/Article/details/gptlzmgpe.sHtML

[T22] Swift：字典
来源：http://www.blog.epnwcf.com/Article/details/gdzsfbxic.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.epnwcf.com/Article/details/gswvoglsy.sHtML

[T23] Swift：函数
来源：http://www.share.bbcook.cn/Article/details/glmezlewc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fktsv.cn/Article/details/gchxkwpsg.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/grtfnoivk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.yfazqb.com/Article/details/gtuhrsczq.sHtML

[T25] Swift：结构体
来源：http://www.share.fktsv.cn/Article/details/gsjnalcpt.sHtML

struct P { var x: Int }
来源：http://www.share.yfazqb.com/Article/details/ghlvqhzkt.sHtML

[T26] Swift：类与重写
来源：http://3g.fktsv.cn/Article/details/ggnyexvfs.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gtkaymldr.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/ghssuxhne.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fktsv.cn/Article/details/givtlzbew.sHtML

[T28] Swift：枚举
来源：http://blog.bbcook.cn/Article/details/gfaxfoygf.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/gysvpzxvl.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.epnwcf.com/Article/details/gkpkjmzsb.sHtML

guard let x = opt else { return }
来源：http://mobile.fktsv.cn/Article/details/giuzspwml.sHtML

[T30] Swift：协议
来源：http://baike.bbcook.cn/Article/details/gxssfgovi.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.sjlbkw.cn/Article/details/gzljnfipf.sHtML

[T31] Lua：Hello World
来源：http://www.share.bbcook.cn/Article/details/gvllbjnno.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gqurvmvao.sHtML

[T32] Lua：局部变量
来源：http://mobile.epnwcf.com/Article/details/gzktfwbxv.sHtML

local a = 1
来源：http://blog.sjlbkw.cn/Article/details/glitqxsln.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/gnvpsgpws.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.epnwcf.com/Article/details/gzbzpqwkw.sHtML

[T34] Lua：遍历表
来源：http://wap.fktsv.cn/Article/details/geqegmfof.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.tarul.cn/Article/details/glzwpmeow.sHtML

[T35] Lua：字典表
来源：http://m.share.fktsv.cn/Article/details/guioqnbyq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.vehdjk.com/Article/details/guyfvarpa.sHtML

[T36] Lua：函数
来源：http://blog.epnwcf.com/Article/details/gbveiptum.sHtML

function add(a, b) return a + b end
来源：http://blog.bbcook.cn/Article/details/gkqtcvzvo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.vehdjk.com/Article/details/giyfcddsg.sHtML

"a" .. "b"
来源：http://wap.bbcook.cn/Article/details/gzpscmdcv.sHtML

[T38] Lua：条件
来源：http://blog.epnwcf.com/Article/details/gxemhnfcz.sHtML

if x > 0 then print("正") end
来源：http://mobile.sjlbkw.cn/Article/details/gdwqmvrbe.sHtML

[T39] Lua：模式匹配
来源：http://baike.vehdjk.com/Article/details/gxoqngeng.sHtML

string.find(s, "%d+")
来源：http://www.share.tarul.cn/Article/details/grgrhpiac.sHtML

[T40] Lua：元表
来源：http://wap.sjlbkw.cn/Article/details/gmpnlkqjm.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.yfazqb.com/Article/details/gkbjjyuty.sHtML

[T41] Perl：Hello World
来源：http://read.share.tarul.cn/Article/details/gqsmmnpme.sHtML

print "Hello\n";
来源：http://www.blog.sjlbkw.cn/Article/details/gultwrvhx.sHtML

[T42] Perl：变量类型
来源：http://mobile.tarul.cn/Article/details/gqmordjee.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.tarul.cn/Article/details/gzhgebojy.sHtML

[T43] Perl：字符串插值
来源：http://wap.vehdjk.com/Article/details/goykrvdcb.sHtML

"值: $a"
来源：http://blog.vehdjk.com/Article/details/gdfokzucm.sHtML

[T44] Perl：条件
来源：http://www.share.bbcook.cn/Article/details/gbwuqjrjm.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.bbcook.cn/Article/details/gwbycayas.sHtML

[T45] Perl：数组遍历
来源：http://baike.yfazqb.com/Article/details/gpautnbnr.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.yfazqb.com/Article/details/gkgfchowz.sHtML

[T46] Perl：哈希操作
来源：http://wap.epnwcf.com/Article/details/gmqpplibh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fktsv.cn/Article/details/ghycjvcig.sHtML

[T47] Perl：正则捕获
来源：http://blog.sjlbkw.cn/Article/details/gfnxdrpls.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.yfazqb.com/Article/details/gkmsaatvx.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/grwnrcagm.sHtML

$s =~ s/old/new/g;
来源：http://3g.bbcook.cn/Article/details/gibyfqeis.sHtML

[T49] Perl：函数
来源：http://blog.vehdjk.com/Article/details/gzpnjpwcz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gbemklwad.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gwigfawom.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.sjlbkw.cn/Article/details/gbkgzsgum.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gwsqhwweo.sHtML

[T51] Scala：Hello World
来源：http://baike.fktsv.cn/Article/details/gxydsxznt.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gcdpaecvr.sHtML

[T52] Scala：变量
来源：http://www.share.sjlbkw.cn/Article/details/gdqxfyrcu.sHtML

val a = 1;  var b = 2
来源：http://baike.vehdjk.com/Article/details/grkjdvpzi.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gauwdwswv.sHtML

s"值: $b"
来源：http://m.share.tarul.cn/Article/details/ghlovcbif.sHtML

[T54] Scala：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gjwufydll.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fktsv.cn/Article/details/gbzccqhnl.sHtML

[T55] Scala：集合过滤
来源：http://blog.yfazqb.com/Article/details/gcbsvhxgv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.sjlbkw.cn/Article/details/gyjyrkycn.sHtML

[T56] Scala：样例类
来源：http://blog.vehdjk.com/Article/details/gosewcyoa.sHtML

case class User(name: String, age: Int)
来源：http://www.share.vehdjk.com/Article/details/gsjmuupmv.sHtML

[T57] Scala：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gsdbvxizj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.vehdjk.com/Article/details/gkqjifeie.sHtML

[T58] Scala：函数定义
来源：http://www.blog.tarul.cn/Article/details/gkuotcjkl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.tarul.cn/Article/details/gvxzunkme.sHtML

[T59] Scala：循环
来源：http://3g.yfazqb.com/Article/details/gbmunksju.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.vehdjk.com/Article/details/gxighecoq.sHtML

[T60] Scala：折叠
来源：http://www.share.vehdjk.com/Article/details/gfczydafl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.vehdjk.com/Article/details/gysgyjplb.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gdjbhiuir.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.tarul.cn/Article/details/gvhvedwrj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gxzeziube.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fktsv.cn/Article/details/ggrdxbxbt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fktsv.cn/Article/details/gjgdqzfqe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fktsv.cn/Article/details/gqxxylbnq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.yfazqb.com/Article/details/gouehkfud.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/gzcedavfy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.bbcook.cn/Article/details/gyegfmxdd.sHtML

[U04] Py：变量调试打印
来源：http://read.share.tarul.cn/Article/details/gktumsbdg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.tarul.cn/Article/details/gbymhilzn.sHtML

[U05] Py：列表去重且保序
来源：http://blog.yfazqb.com/Article/details/gozjbfrzg.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/gylqkqgpl.sHtML

[U06] Py：合并两个字典
来源：http://3g.bbcook.cn/Article/details/gpatnxmva.sHtML

{**a, **b}
来源：http://wap.sjlbkw.cn/Article/details/gwhfxuesj.sHtML

[U07] Py：反转字典键值
来源：http://blog.tarul.cn/Article/details/gdmtfspxo.sHtML

{v: k for k, v in d.items()}
来源：http://baike.bbcook.cn/Article/details/gzlywrwbt.sHtML

[U08] Py：展平二维列表
来源：http://wap.bbcook.cn/Article/details/gbhprjmww.sHtML

[y for x in nested for y in x]
来源：http://3g.tarul.cn/Article/details/gzywndflv.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.epnwcf.com/Article/details/gdszntbvm.sHtML

max(d, key=d.get)
来源：http://m.share.vehdjk.com/Article/details/gfkaatokc.sHtML

[U10] Py：按值排序字典
来源：http://3g.vehdjk.com/Article/details/gfodbhtoa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.yfazqb.com/Article/details/gizybnngg.sHtML

[U11] Py：生成器表达式
来源：http://blog.tarul.cn/Article/details/gcffkhwqh.sHtML

(x * 2 for x in arr)
来源：http://3g.epnwcf.com/Article/details/galvdbryy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.epnwcf.com/Article/details/gdwgtqxou.sHtML

Counter(arr).most_common(3)
来源：http://m.share.tarul.cn/Article/details/gdxxebidt.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.bbcook.cn/Article/details/gcyjxnmqo.sHtML

deque(maxlen=10)
来源：http://www.m.share.bbcook.cn/Article/details/gxrjdpdba.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.tarul.cn/Article/details/gcostlhvi.sHtML

defaultdict(list)
来源：http://read.share.vehdjk.com/Article/details/gqjtwyire.sHtML


<!-- 参考信息 -->