代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.epnwcf.com/Article/details/ghanktcsk.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.tarul.cn/Article/details/gxnsglkbb.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/gmabonswm.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gonetlflh.sHtML

S. C / C++ 专题
来源：http://wap.vehdjk.com/Article/details/gcmdusllh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxifzdthc.sHtML

[S01] C：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gyabrcotj.sHtML

#include <stdio.h>
来源：http://baike.yfazqb.com/Article/details/gutzjamyu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtyveknlx.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.epnwcf.com/Article/details/ghzxvqpxd.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.epnwcf.com/Article/details/gvyimhklv.sHtML

[S03] C：读入整数
来源：http://www.blog.vehdjk.com/Article/details/gumucwkyo.sHtML

int x; scanf("%d", &x);
来源：http://mobile.epnwcf.com/Article/details/gfjeautcg.sHtML

[S04] C：字符串复制
来源：http://wap.fktsv.cn/Article/details/gcammocfo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gblpiyebr.sHtML

[S05] C：字符串长度
来源：http://wap.tarul.cn/Article/details/gyyfvnxsy.sHtML

strlen(s)
来源：http://www.share.yfazqb.com/Article/details/gjeahvbyc.sHtML

[S06] C：字符串比较
来源：http://3g.epnwcf.com/Article/details/gxzbfnobr.sHtML

strcmp(a, b) == 0
来源：http://mobile.fktsv.cn/Article/details/gacgffpqz.sHtML

[S07] C：数组遍历求和
来源：http://m.share.vehdjk.com/Article/details/gvwialfqe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/gerijghwg.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/gvratweaq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.tarul.cn/Article/details/gihzwhzva.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.tarul.cn/Article/details/gmcshwsqc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.yfazqb.com/Article/details/gryarcpeh.sHtML

[S10] C：指针与解引用
来源：http://baike.sjlbkw.cn/Article/details/gsxrtveov.sHtML

int *p = &a;  *p = 5;
来源：http://blog.bbcook.cn/Article/details/gtzumwejl.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/ggifeekdt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.bbcook.cn/Article/details/gknplfhty.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fktsv.cn/Article/details/giamenbrx.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/gkfbadeon.sHtML

[S12] C：写文件
来源：http://www.blog.fktsv.cn/Article/details/gmbuvyakt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/gtrlhhwqr.sHtML

[S13] C：宏定义
来源：http://mobile.vehdjk.com/Article/details/gmnmpzyzo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.epnwcf.com/Article/details/gskkftltc.sHtML

[S14] C：枚举
来源：http://www.m.share.vehdjk.com/Article/details/gfaytxpag.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.bbcook.cn/Article/details/gtdxzcygm.sHtML

[S15] C：类型转换
来源：http://www.share.epnwcf.com/Article/details/gmgalqsea.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/gbyypydts.sHtML

[S16] C：位操作置位
来源：http://blog.epnwcf.com/Article/details/gnecwddxp.sHtML

x |= (1 << 3);
来源：http://read.share.fktsv.cn/Article/details/gqgqztzak.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gqzikjatq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.vehdjk.com/Article/details/gixblcxnl.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/gdpuiyhsy.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/gcifqiick.sHtML

[S19] C：快速排序
来源：http://wap.tarul.cn/Article/details/glcoegpyw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gzlxpxyxq.sHtML

[S20] C：二分查找
来源：http://baike.yfazqb.com/Article/details/gmaftkrtk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gqfitzqon.sHtML

[S21] C：字符类别判断
来源：http://baike.sjlbkw.cn/Article/details/gsmojnjvw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.vehdjk.com/Article/details/giktaghza.sHtML

[S22] C：字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gcoxgysya.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.epnwcf.com/Article/details/gwdzvojji.sHtML

[S23] C：随机数
来源：http://www.blog.fktsv.cn/Article/details/gytgjpzsd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fktsv.cn/Article/details/gqnuwfkzp.sHtML

[S24] C：获取本地时间
来源：http://blog.tarul.cn/Article/details/gfzgedrbz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.epnwcf.com/Article/details/gdlvoadwv.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/ghbgsbsty.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/grxulvrbz.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gdtszvldk.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/gcaezydsm.sHtML

[S27] C：定义常量
来源：http://m.share.vehdjk.com/Article/details/gmbwxvwjw.sHtML

const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gqvzslwsf.sHtML

[S28] C：静态变量
来源：http://www.share.fktsv.cn/Article/details/gnwfrymwn.sHtML

static int counter = 0;
来源：http://m.share.fktsv.cn/Article/details/gazhgdhel.sHtML

[S29] C：变参函数
来源：http://read.share.epnwcf.com/Article/details/grhpabuwe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.tarul.cn/Article/details/gzppepini.sHtML

[S30] C：头文件保护
来源：http://wap.yfazqb.com/Article/details/gdsoyfdmj.sHtML

#ifndef X_H
来源：http://wap.fktsv.cn/Article/details/gobjcgotb.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/ggbghpxfp.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/gnnrgcfbk.sHtML

[S31] C++：Hello World
来源：http://wap.vehdjk.com/Article/details/gqnuhgmcx.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/gkobekuxc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/ghyoyzkme.sHtML

[S32] C++：字符串
来源：http://blog.vehdjk.com/Article/details/ggscbrbvn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.epnwcf.com/Article/details/gzadueucr.sHtML

[S33] C++：vector 增删
来源：http://blog.tarul.cn/Article/details/gjezckuwn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.tarul.cn/Article/details/gzuzyhwjp.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/gnrgwvsvf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.bbcook.cn/Article/details/gfkseerec.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/gkhejylae.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gfhvwsesn.sHtML

[S36] C++：unordered_map
来源：http://www.blog.epnwcf.com/Article/details/gkeueqbfv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gqypyioiz.sHtML

[S37] C++：set
来源：http://wap.fktsv.cn/Article/details/geetdesyt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/gaizrdjme.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/glpmukwww.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.vehdjk.com/Article/details/gpqeznjdt.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/geqlemzbs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fktsv.cn/Article/details/gpyrzckde.sHtML

[S40] C++：查找元素
来源：http://baike.yfazqb.com/Article/details/gkrqjtwqd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/gmiotywnv.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gwhhpxiba.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.epnwcf.com/Article/details/gydwjkaky.sHtML

[S42] C++：继承与虚函数
来源：http://blog.vehdjk.com/Article/details/gqywvaqfo.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.vehdjk.com/Article/details/gvjsljwbz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.bbcook.cn/Article/details/gteobwssw.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.sjlbkw.cn/Article/details/gxudtwiab.sHtML

[S44] C++：引用传参
来源：http://m.share.bbcook.cn/Article/details/gazfavsdh.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/ghczyxosg.sHtML

[S45] C++：lambda
来源：http://blog.epnwcf.com/Article/details/gkpqkbeco.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.yfazqb.com/Article/details/gftqoklcc.sHtML

[S46] C++：函数模板
来源：http://m.share.bbcook.cn/Article/details/gosgliyel.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.vehdjk.com/Article/details/gylhflayi.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.yfazqb.com/Article/details/gynmwviuj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/gaqcjeuzy.sHtML

[S48] C++：逐行读文件
来源：http://baike.fktsv.cn/Article/details/getfbvdwf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.yfazqb.com/Article/details/grqprmtmt.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.epnwcf.com/Article/details/gfaxzulfq.sHtML

[S49] C++：写文件
来源：http://mobile.bbcook.cn/Article/details/glmizcbaa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fktsv.cn/Article/details/gfpmxfsgp.sHtML

[S50] C++：格式化数字
来源：http://mobile.tarul.cn/Article/details/giaonokuh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gndaqgqfe.sHtML

[S51] C++：显式类型转换
来源：http://www.share.bbcook.cn/Article/details/gunpkwjnl.sHtML

static_cast<double>(a) / b
来源：http://3g.epnwcf.com/Article/details/ggbsknosz.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.vehdjk.com/Article/details/godurqcxq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.yfazqb.com/Article/details/gdjnjyqcu.sHtML

[S53] C++：移动语义
来源：http://www.m.share.yfazqb.com/Article/details/gkyhaeeed.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.sjlbkw.cn/Article/details/giwygdnln.sHtML

[S54] C++：异常处理
来源：http://wap.vehdjk.com/Article/details/gaqbsiape.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.yfazqb.com/Article/details/gjaujnguo.sHtML

[S55] C++：结构化绑定
来源：http://wap.sjlbkw.cn/Article/details/ggnwmvlsc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/gdorvoqdh.sHtML

[S56] C++：optional
来源：http://mobile.fktsv.cn/Article/details/gdjxbikaq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.yfazqb.com/Article/details/gfyiplhjy.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/glulqrxwd.sHtML

constexpr int N = 10;
来源：http://blog.tarul.cn/Article/details/gtopqzxwm.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gxaigjhba.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.bbcook.cn/Article/details/ggkhppiyx.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gpxgkbgrp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fktsv.cn/Article/details/gnasjcnxm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.bbcook.cn/Article/details/gwixdhbzh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.bbcook.cn/Article/details/gzaoqdkuv.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gbkpjvoqn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.sjlbkw.cn/Article/details/gachfzwrd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/guyybwsjr.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.vehdjk.com/Article/details/grcylwffl.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gqjpxbnsv.sHtML

[T02] Kotlin：变量
来源：http://read.share.vehdjk.com/Article/details/gbvpjlrmk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.tarul.cn/Article/details/gkraombji.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.bbcook.cn/Article/details/gkzkwvyny.sHtML

"值: $b"
来源：http://3g.vehdjk.com/Article/details/guafnzrwn.sHtML

[T04] Kotlin：空安全
来源：http://blog.epnwcf.com/Article/details/gwnskhriv.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gplbaismu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.sjlbkw.cn/Article/details/gmwnrmneu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/gxajpjsnt.sHtML

[T06] Kotlin：集合映射
来源：http://3g.sjlbkw.cn/Article/details/ggihzvqjf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fktsv.cn/Article/details/gmiasclxu.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.tarul.cn/Article/details/gghjeyfcv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fktsv.cn/Article/details/gmxtjzfko.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fktsv.cn/Article/details/gbcziucni.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.yfazqb.com/Article/details/gjtpnxxkj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.sjlbkw.cn/Article/details/gogjjbxvs.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.tarul.cn/Article/details/gnvhbisym.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.bbcook.cn/Article/details/ghrbvacew.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.yfazqb.com/Article/details/gizgasnnf.sHtML

[T11] Kotlin：协程
来源：http://baike.epnwcf.com/Article/details/gclhtbnnp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.vehdjk.com/Article/details/ghsvmznre.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fktsv.cn/Article/details/geojmuuab.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gutecgdyr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/ghftzwayn.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.tarul.cn/Article/details/gfcismrff.sHtML

[T14] Kotlin：循环
来源：http://www.blog.yfazqb.com/Article/details/gmiopzgdn.sHtML

for (i in 1..10) println(i)
来源：http://baike.fktsv.cn/Article/details/glphktpjo.sHtML

[T15] Kotlin：接口
来源：http://www.blog.epnwcf.com/Article/details/gzihwiqun.sHtML

interface Shape { fun area(): Double }
来源：http://blog.yfazqb.com/Article/details/gpecgrdee.sHtML

[T16] Swift：Hello World
来源：http://mobile.fktsv.cn/Article/details/gsodmuqah.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/glsuwiuur.sHtML

[T17] Swift：变量与常量
来源：http://blog.sjlbkw.cn/Article/details/geajyzesn.sHtML

var a = 1;  let b = 2
来源：http://read.share.fktsv.cn/Article/details/ggwvhutwn.sHtML

[T18] Swift：字符串插值
来源：http://blog.tarul.cn/Article/details/goqornxlb.sHtML

"值: \(b)"
来源：http://www.share.yfazqb.com/Article/details/goqgmetul.sHtML

[T19] Swift：可选绑定
来源：http://www.share.sjlbkw.cn/Article/details/geabjqrrk.sHtML

if let n = opt { print(n) }
来源：http://wap.fktsv.cn/Article/details/gbrotjlqe.sHtML

[T20] Swift：数组操作
来源：http://blog.vehdjk.com/Article/details/gnpxnqdmd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.tarul.cn/Article/details/gmwvxsews.sHtML

[T21] Swift：遍历
来源：http://m.share.sjlbkw.cn/Article/details/girpvklvr.sHtML

for x in a { print(x) }
来源：http://read.share.tarul.cn/Article/details/gjxtwowps.sHtML

[T22] Swift：字典
来源：http://baike.bbcook.cn/Article/details/gjomctsvh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.yfazqb.com/Article/details/goohdlsfe.sHtML

[T23] Swift：函数
来源：http://m.share.sjlbkw.cn/Article/details/gzgbpukgi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/gaidnoxov.sHtML

[T24] Swift：闭包
来源：http://mobile.bbcook.cn/Article/details/golmqjmml.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gluazeswq.sHtML

[T25] Swift：结构体
来源：http://www.share.vehdjk.com/Article/details/gmmhsttkh.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/glgkupsud.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/gqspigrxf.sHtML

class A: Base { override func f() {} }
来源：http://baike.tarul.cn/Article/details/gxpawtlcq.sHtML

[T27] Swift：错误处理
来源：http://www.share.vehdjk.com/Article/details/ghpvzjzow.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.tarul.cn/Article/details/gfrzmckqm.sHtML

[T28] Swift：枚举
来源：http://3g.fktsv.cn/Article/details/gctkalcem.sHtML

enum Color { case red, green }
来源：http://www.blog.tarul.cn/Article/details/gpbpzbrzi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.bbcook.cn/Article/details/gflzcptkp.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/gafqkmdms.sHtML

[T30] Swift：协议
来源：http://wap.fktsv.cn/Article/details/gwhxswcgk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.yfazqb.com/Article/details/gyfifwcva.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gsdjxyihg.sHtML

print("Hello")
来源：http://www.blog.vehdjk.com/Article/details/guihamqmw.sHtML

[T32] Lua：局部变量
来源：http://m.share.epnwcf.com/Article/details/gnbsnrwnt.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/gbzmfsftx.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.vehdjk.com/Article/details/gnedltqra.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.bbcook.cn/Article/details/glcepeiqd.sHtML

[T34] Lua：遍历表
来源：http://www.blog.bbcook.cn/Article/details/gnslxoltx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fktsv.cn/Article/details/gghkrdony.sHtML

[T35] Lua：字典表
来源：http://m.share.epnwcf.com/Article/details/gvkeullff.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.tarul.cn/Article/details/gkjowctee.sHtML

[T36] Lua：函数
来源：http://mobile.fktsv.cn/Article/details/ghrwqjfjk.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fktsv.cn/Article/details/gldfrgfqi.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.tarul.cn/Article/details/gzsozbbsq.sHtML

"a" .. "b"
来源：http://wap.yfazqb.com/Article/details/gjlipjwce.sHtML

[T38] Lua：条件
来源：http://mobile.yfazqb.com/Article/details/gzlohikhg.sHtML

if x > 0 then print("正") end
来源：http://www.blog.sjlbkw.cn/Article/details/gldmzazio.sHtML

[T39] Lua：模式匹配
来源：http://wap.tarul.cn/Article/details/ginegsovo.sHtML

string.find(s, "%d+")
来源：http://3g.vehdjk.com/Article/details/gceenkotl.sHtML

[T40] Lua：元表
来源：http://read.share.sjlbkw.cn/Article/details/gdxzlcodg.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.vehdjk.com/Article/details/guxvfowyr.sHtML

[T41] Perl：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gqlyosots.sHtML

print "Hello\n";
来源：http://read.share.tarul.cn/Article/details/gbkmivznw.sHtML

[T42] Perl：变量类型
来源：http://m.share.tarul.cn/Article/details/grjbzcvdo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.epnwcf.com/Article/details/gfvtyaopo.sHtML

[T43] Perl：字符串插值
来源：http://mobile.tarul.cn/Article/details/goqfyjrld.sHtML

"值: $a"
来源：http://www.blog.sjlbkw.cn/Article/details/gsunpcesg.sHtML

[T44] Perl：条件
来源：http://mobile.yfazqb.com/Article/details/grynqznzw.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fktsv.cn/Article/details/grzovtgbn.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.tarul.cn/Article/details/gfpmdmuil.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.vehdjk.com/Article/details/gaqbksmzj.sHtML

[T46] Perl：哈希操作
来源：http://read.share.epnwcf.com/Article/details/gaxsitzfr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.yfazqb.com/Article/details/gryvtjsxj.sHtML

[T47] Perl：正则捕获
来源：http://www.share.bbcook.cn/Article/details/geqdkguxq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.vehdjk.com/Article/details/gbalpcaes.sHtML

[T48] Perl：正则替换
来源：http://www.share.tarul.cn/Article/details/guounskcg.sHtML

$s =~ s/old/new/g;
来源：http://3g.tarul.cn/Article/details/gbnkvmkkc.sHtML

[T49] Perl：函数
来源：http://baike.sjlbkw.cn/Article/details/gmkntllik.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gfxlxdlis.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.tarul.cn/Article/details/ghtizgsph.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.sjlbkw.cn/Article/details/gggwmjemy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.epnwcf.com/Article/details/gqfodzyma.sHtML

[T51] Scala：Hello World
来源：http://www.blog.tarul.cn/Article/details/gdzishlie.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gtjjyfivk.sHtML

[T52] Scala：变量
来源：http://read.share.vehdjk.com/Article/details/grspmgvir.sHtML

val a = 1;  var b = 2
来源：http://www.blog.bbcook.cn/Article/details/gbqsfxoox.sHtML

[T53] Scala：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gdbhhygyc.sHtML

s"值: $b"
来源：http://mobile.epnwcf.com/Article/details/gofhbfdsl.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/gpyylqwqb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.tarul.cn/Article/details/ghvxzsjyn.sHtML

[T55] Scala：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gyzzytmft.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.tarul.cn/Article/details/gduousvmd.sHtML

[T56] Scala：样例类
来源：http://mobile.tarul.cn/Article/details/gfoksjezl.sHtML

case class User(name: String, age: Int)
来源：http://read.share.epnwcf.com/Article/details/gtioxyftx.sHtML

[T57] Scala：模式匹配
来源：http://mobile.epnwcf.com/Article/details/gjnwpntyx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/ggiticxtf.sHtML

[T58] Scala：函数定义
来源：http://3g.fktsv.cn/Article/details/ggvccokiu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.yfazqb.com/Article/details/gnmbkdjtj.sHtML

[T59] Scala：循环
来源：http://mobile.sjlbkw.cn/Article/details/gqszrehpj.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.tarul.cn/Article/details/gpxzbcjen.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fktsv.cn/Article/details/gdlcqpxhg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.vehdjk.com/Article/details/goiodwxxe.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/goigkewhp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gbqtozbco.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gevnodzie.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.yfazqb.com/Article/details/gmkizojjp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.epnwcf.com/Article/details/gykaavxti.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.yfazqb.com/Article/details/gycbditif.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.sjlbkw.cn/Article/details/gomparehd.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/gbrcuamut.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.sjlbkw.cn/Article/details/gmqnfphdx.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.epnwcf.com/Article/details/gtzwkzulf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.yfazqb.com/Article/details/gfjlqlkzk.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.epnwcf.com/Article/details/gucspfeen.sHtML

list(dict.fromkeys(arr))
来源：http://baike.sjlbkw.cn/Article/details/ggfosataj.sHtML

[U06] Py：合并两个字典
来源：http://www.share.bbcook.cn/Article/details/gfbmtqwdq.sHtML

{**a, **b}
来源：http://www.m.share.fktsv.cn/Article/details/ghugtptyd.sHtML

[U07] Py：反转字典键值
来源：http://www.share.tarul.cn/Article/details/gayxhvsvg.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.tarul.cn/Article/details/guzdqslqb.sHtML

[U08] Py：展平二维列表
来源：http://mobile.vehdjk.com/Article/details/gnlqvrnxy.sHtML

[y for x in nested for y in x]
来源：http://3g.bbcook.cn/Article/details/ghtuqmgvy.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fktsv.cn/Article/details/gydkxiwci.sHtML

max(d, key=d.get)
来源：http://blog.fktsv.cn/Article/details/gzvmduwsk.sHtML

[U10] Py：按值排序字典
来源：http://m.share.tarul.cn/Article/details/ghopzyhvq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.tarul.cn/Article/details/glysvurfv.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fktsv.cn/Article/details/gcdywovdv.sHtML

(x * 2 for x in arr)
来源：http://blog.epnwcf.com/Article/details/giazodybo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.tarul.cn/Article/details/gwknwzaje.sHtML

Counter(arr).most_common(3)
来源：http://m.share.yfazqb.com/Article/details/gghiziskv.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.epnwcf.com/Article/details/gfiflweoq.sHtML

deque(maxlen=10)
来源：http://read.share.vehdjk.com/Article/details/gfxxoujyq.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fktsv.cn/Article/details/glzygkovv.sHtML

defaultdict(list)
来源：http://baike.epnwcf.com/Article/details/guxsbbycf.sHtML

[U15] Py：高精度计时
来源：http://mobile.sjlbkw.cn/Article/details/gtnxwwnnt.sHtML

t = time.perf_counter()
来源：http://3g.yfazqb.com/Article/details/gfzobyzhi.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fktsv.cn/Article/details/ggymemwbw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.sjlbkw.cn/Article/details/goxqxmycr.sHtML

[U17] Py：初始化日志
来源：http://read.share.tarul.cn/Article/details/gfnvoeumg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.bbcook.cn/Article/details/gbonkydfc.sHtML

[U18] Py：预编译正则
来源：http://read.share.tarul.cn/Article/details/gpvdlamgt.sHtML

pat = re.compile(r"\d+")
来源：http://baike.vehdjk.com/Article/details/ghbpkmvuo.sHtML

[U19] Py：正则替换带回调
来源：http://baike.bbcook.cn/Article/details/ggmgqmzcp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.vehdjk.com/Article/details/gmfnflxbz.sHtML

[U20] Py：缓存函数结果
来源：http://blog.epnwcf.com/Article/details/gtykehqdi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.bbcook.cn/Article/details/gjmcfqtty.sHtML


<!-- 参考信息 -->