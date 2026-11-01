代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.sjlbkw.cn/Article/details/ggkebkvef.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.sjlbkw.cn/Article/details/gkvvlynbm.sHtML

time ./run.sh
来源：http://www.share.epnwcf.com/Article/details/gzfuzduti.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbyuaeoqj.sHtML

S. C / C++ 专题
来源：http://baike.bbcook.cn/Article/details/gazyvaqmi.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gdnjmfgzp.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/ggnwxotmc.sHtML

#include <stdio.h>
来源：http://blog.tarul.cn/Article/details/gldjpdmbr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fktsv.cn/Article/details/gpqijzifr.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.vehdjk.com/Article/details/giufgpnad.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.sjlbkw.cn/Article/details/gajtulpvb.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/gnhkbeura.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjvlvvrq.sHtML

[S04] C：字符串复制
来源：http://blog.vehdjk.com/Article/details/gdpefrjak.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.epnwcf.com/Article/details/gwveqfvtf.sHtML

[S05] C：字符串长度
来源：http://wap.yfazqb.com/Article/details/gguaoyhiy.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/gkmdfopab.sHtML

[S06] C：字符串比较
来源：http://mobile.epnwcf.com/Article/details/gmgulroeq.sHtML

strcmp(a, b) == 0
来源：http://baike.bbcook.cn/Article/details/gohqzgutn.sHtML

[S07] C：数组遍历求和
来源：http://wap.sjlbkw.cn/Article/details/gukcjgdux.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.vehdjk.com/Article/details/gqwdvhuju.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.sjlbkw.cn/Article/details/gvnxqkhbl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.yfazqb.com/Article/details/gjxsgdwws.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fktsv.cn/Article/details/gzsqaznui.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/gzixzltqq.sHtML

[S10] C：指针与解引用
来源：http://mobile.sjlbkw.cn/Article/details/gtwtqbely.sHtML

int *p = &a;  *p = 5;
来源：http://3g.vehdjk.com/Article/details/gakwrhidl.sHtML

[S11] C：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gwmxawphk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.tarul.cn/Article/details/gbrxogamp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gtcfgvpps.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/ghwxvufnm.sHtML

[S12] C：写文件
来源：http://blog.epnwcf.com/Article/details/gnjnziqch.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/ghxhooici.sHtML

[S13] C：宏定义
来源：http://m.share.bbcook.cn/Article/details/gsglwrbnl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fktsv.cn/Article/details/gznwacvgn.sHtML

[S14] C：枚举
来源：http://mobile.bbcook.cn/Article/details/gntcmfisv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.yfazqb.com/Article/details/gzqonvvdm.sHtML

[S15] C：类型转换
来源：http://baike.fktsv.cn/Article/details/gusrvvcqs.sHtML

(double) a / b
来源：http://m.share.yfazqb.com/Article/details/gblnwqmor.sHtML

[S16] C：位操作置位
来源：http://www.blog.yfazqb.com/Article/details/gdtnzoouk.sHtML

x |= (1 << 3);
来源：http://read.share.tarul.cn/Article/details/gpkqrckbc.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/grdcdjkgj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.epnwcf.com/Article/details/gjeplmhyj.sHtML

[S18] C：命令行参数
来源：http://mobile.sjlbkw.cn/Article/details/gtaufxhgp.sHtML

int main(int argc, char **argv)
来源：http://read.share.epnwcf.com/Article/details/grcjdiqqj.sHtML

[S19] C：快速排序
来源：http://baike.bbcook.cn/Article/details/gycwmhnlq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gvheoyzec.sHtML

[S20] C：二分查找
来源：http://mobile.vehdjk.com/Article/details/gypgotkmu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gqbkkochs.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/guawjpiea.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/gpsbavjuv.sHtML

[S22] C：字符串转数字
来源：http://www.blog.tarul.cn/Article/details/gxlukoreh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fktsv.cn/Article/details/gjpymhxlf.sHtML

[S23] C：随机数
来源：http://www.share.bbcook.cn/Article/details/gwqpvalao.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.epnwcf.com/Article/details/glfwvnwws.sHtML

[S24] C：获取本地时间
来源：http://wap.epnwcf.com/Article/details/gxsgkywra.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.vehdjk.com/Article/details/gfhzkgbsc.sHtML

[S25] C：内存拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gonfapsth.sHtML

memcpy(dst, src, n);
来源：http://mobile.fktsv.cn/Article/details/giylajtpw.sHtML

[S26] C：内存清零
来源：http://www.blog.bbcook.cn/Article/details/gebaxsisw.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fktsv.cn/Article/details/gbubhdwie.sHtML

[S27] C：定义常量
来源：http://wap.bbcook.cn/Article/details/guvlfvmrd.sHtML

const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gxbfqwbxb.sHtML

[S28] C：静态变量
来源：http://read.share.tarul.cn/Article/details/gelxrmfvi.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gmquxcaxp.sHtML

[S29] C：变参函数
来源：http://m.share.tarul.cn/Article/details/gwbpbizcd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.epnwcf.com/Article/details/gactesgup.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gzxtmzpxf.sHtML

#ifndef X_H
来源：http://3g.fktsv.cn/Article/details/gajurcgzn.sHtML

#define X_H
来源：http://m.share.sjlbkw.cn/Article/details/glqjtqrmn.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/gnwspdgir.sHtML

[S31] C++：Hello World
来源：http://baike.epnwcf.com/Article/details/gbrhacrkl.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gchjhrgft.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.sjlbkw.cn/Article/details/grmjnsshu.sHtML

[S32] C++：字符串
来源：http://blog.sjlbkw.cn/Article/details/ghetredvq.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.epnwcf.com/Article/details/gqjmktmzi.sHtML

[S33] C++：vector 增删
来源：http://wap.bbcook.cn/Article/details/gbmadsttm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.yfazqb.com/Article/details/gmgvrlcwl.sHtML

[S34] C++：遍历 vector
来源：http://blog.vehdjk.com/Article/details/guknrefvm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/gmkciznut.sHtML

[S35] C++：map
来源：http://blog.sjlbkw.cn/Article/details/gzvnjpdue.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/goukekhvf.sHtML

[S36] C++：unordered_map
来源：http://wap.epnwcf.com/Article/details/gasgmtqbl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/geohkgpvl.sHtML

[S37] C++：set
来源：http://3g.bbcook.cn/Article/details/giqygliqh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.epnwcf.com/Article/details/gzrzygptv.sHtML

[S38] C++：排序
来源：http://3g.yfazqb.com/Article/details/gpdlkjldk.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gnnitaktt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.epnwcf.com/Article/details/gaatywwho.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/gzucspzbt.sHtML

[S40] C++：查找元素
来源：http://3g.vehdjk.com/Article/details/goxcqegam.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/gjisphdsh.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/gypzbvpdh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fktsv.cn/Article/details/gsdtgydpb.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/gihsltxhm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.vehdjk.com/Article/details/golcewpah.sHtML

[S43] C++：智能指针
来源：http://www.share.epnwcf.com/Article/details/glhdqxnpr.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.tarul.cn/Article/details/gvtyarmbj.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/ggzvrcuan.sHtML

void inc(int &x) { ++x; }
来源：http://baike.vehdjk.com/Article/details/gpcbudwvq.sHtML

[S45] C++：lambda
来源：http://blog.fktsv.cn/Article/details/gftfcpbld.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.yfazqb.com/Article/details/gbpstojmz.sHtML

[S46] C++：函数模板
来源：http://3g.tarul.cn/Article/details/gpsadtfcj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.yfazqb.com/Article/details/ggylnytwf.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fktsv.cn/Article/details/gsvlwemun.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.bbcook.cn/Article/details/gmtajqsof.sHtML

[S48] C++：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gzorfvuex.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/gjkelysbr.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.epnwcf.com/Article/details/gdciikpxi.sHtML

[S49] C++：写文件
来源：http://mobile.tarul.cn/Article/details/gylsvmudk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.yfazqb.com/Article/details/gvifglavt.sHtML

[S50] C++：格式化数字
来源：http://read.share.fktsv.cn/Article/details/gsbxprouv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/grzsmhomi.sHtML

[S51] C++：显式类型转换
来源：http://read.share.yfazqb.com/Article/details/gsbaqnujd.sHtML

static_cast<double>(a) / b
来源：http://m.share.fktsv.cn/Article/details/gbovjevsj.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.sjlbkw.cn/Article/details/gtccyouoo.sHtML

int size() const noexcept { return n_; }
来源：http://3g.yfazqb.com/Article/details/gcahviave.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/grrrvnqip.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/gcywbxxji.sHtML

[S54] C++：异常处理
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdvlewps.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.yfazqb.com/Article/details/grpsftqjo.sHtML

[S55] C++：结构化绑定
来源：http://baike.sjlbkw.cn/Article/details/gfmnkkscs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.epnwcf.com/Article/details/gpwhekvxs.sHtML

[S56] C++：optional
来源：http://blog.yfazqb.com/Article/details/gllxpvlyk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.sjlbkw.cn/Article/details/gaxkpyqen.sHtML

[S57] C++：编译期常量
来源：http://www.blog.yfazqb.com/Article/details/gsmidfqko.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/gjrzwzhzs.sHtML

[S58] C++：命名空间
来源：http://baike.sjlbkw.cn/Article/details/gosfhsiwr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/gduhshiem.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/grdrreeyv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.tarul.cn/Article/details/gixocyfpo.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.sjlbkw.cn/Article/details/ganfrbgmh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.vehdjk.com/Article/details/gwbrqwcew.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gytiqhzhj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/gnekhebwo.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grdgxmgqb.sHtML

[T01] Kotlin：Hello World
来源：http://3g.epnwcf.com/Article/details/gvkdkamye.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/giscojedp.sHtML

[T02] Kotlin：变量
来源：http://m.share.bbcook.cn/Article/details/gkiewecch.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.sjlbkw.cn/Article/details/gfqigtysv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.vehdjk.com/Article/details/gyjdwblaa.sHtML

"值: $b"
来源：http://mobile.bbcook.cn/Article/details/gsfqfhtqp.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.epnwcf.com/Article/details/gwgrrljdu.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/gjilykhjx.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.vehdjk.com/Article/details/gbnfakytc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gukoumbcn.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.epnwcf.com/Article/details/gkavsvmlb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.epnwcf.com/Article/details/gmyyfjfbr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/ghxjzfpkb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.vehdjk.com/Article/details/grtxqrmpo.sHtML

[T08] Kotlin：数据类
来源：http://wap.bbcook.cn/Article/details/gunhxteim.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.bbcook.cn/Article/details/gpvvzasnk.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/glzmvqtva.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.epnwcf.com/Article/details/gnjbkcpkm.sHtML

[T10] Kotlin：默认参数
来源：http://blog.vehdjk.com/Article/details/gqxfdhvbt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.tarul.cn/Article/details/gttpsdqnp.sHtML

[T11] Kotlin：协程
来源：http://read.share.yfazqb.com/Article/details/gqamsmcjs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.yfazqb.com/Article/details/gqlxtqvem.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/gbsfcriky.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/gzexuspmf.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.sjlbkw.cn/Article/details/ghuhktjno.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/gydwbqsgf.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gctynicgm.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gdnzwohgr.sHtML

[T15] Kotlin：接口
来源：http://www.share.sjlbkw.cn/Article/details/gymycnjdt.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fktsv.cn/Article/details/giodpgxqm.sHtML

[T16] Swift：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gyyhxskcc.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gekclvdwf.sHtML

[T17] Swift：变量与常量
来源：http://m.share.vehdjk.com/Article/details/gifugaaku.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/glrotasfz.sHtML

[T18] Swift：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gpyztbcsb.sHtML

"值: \(b)"
来源：http://3g.bbcook.cn/Article/details/gviauxlxv.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/gwkjwlved.sHtML

if let n = opt { print(n) }
来源：http://read.share.sjlbkw.cn/Article/details/gzjjbvstd.sHtML

[T20] Swift：数组操作
来源：http://m.share.fktsv.cn/Article/details/gkmfdseiu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fktsv.cn/Article/details/gqipqerhz.sHtML

[T21] Swift：遍历
来源：http://m.share.tarul.cn/Article/details/gicsllbhg.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/gldunbvog.sHtML

[T22] Swift：字典
来源：http://mobile.epnwcf.com/Article/details/gsylcezdu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fktsv.cn/Article/details/gfctugkca.sHtML

[T23] Swift：函数
来源：http://baike.epnwcf.com/Article/details/gmzizhwfw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.epnwcf.com/Article/details/gwzkrmsjd.sHtML

[T24] Swift：闭包
来源：http://m.share.fktsv.cn/Article/details/gmaxesbuw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfscmodzz.sHtML

[T25] Swift：结构体
来源：http://wap.yfazqb.com/Article/details/gjvbfetaz.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/gozlxohyx.sHtML

[T26] Swift：类与重写
来源：http://read.share.yfazqb.com/Article/details/gdwcyuqcj.sHtML

class A: Base { override func f() {} }
来源：http://mobile.vehdjk.com/Article/details/gyntnckab.sHtML

[T27] Swift：错误处理
来源：http://3g.sjlbkw.cn/Article/details/galpdjubg.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.yfazqb.com/Article/details/gfrplndcs.sHtML

[T28] Swift：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gtegnjigp.sHtML

enum Color { case red, green }
来源：http://read.share.vehdjk.com/Article/details/gpqwkfznl.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.bbcook.cn/Article/details/gdwigcjbw.sHtML

guard let x = opt else { return }
来源：http://www.blog.yfazqb.com/Article/details/gitxdkuwq.sHtML

[T30] Swift：协议
来源：http://read.share.fktsv.cn/Article/details/gvdasaifa.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.sjlbkw.cn/Article/details/gnryxnplw.sHtML

[T31] Lua：Hello World
来源：http://wap.yfazqb.com/Article/details/gzxtzasrj.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/guzzchnqv.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.bbcook.cn/Article/details/geuzdkfbr.sHtML

local a = 1
来源：http://www.blog.bbcook.cn/Article/details/gwcyyftgz.sHtML

[T33] Lua：表（数组）
来源：http://m.share.tarul.cn/Article/details/gwwdhqwdc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.yfazqb.com/Article/details/giapddjhh.sHtML

[T34] Lua：遍历表
来源：http://m.share.yfazqb.com/Article/details/giqzdyaaa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.sjlbkw.cn/Article/details/ghfkmsscd.sHtML

[T35] Lua：字典表
来源：http://www.share.epnwcf.com/Article/details/gqaynsbja.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.epnwcf.com/Article/details/gnztaguzh.sHtML

[T36] Lua：函数
来源：http://blog.yfazqb.com/Article/details/gjjwtvosh.sHtML

function add(a, b) return a + b end
来源：http://blog.bbcook.cn/Article/details/gvzechgau.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.yfazqb.com/Article/details/gbksepxvn.sHtML

"a" .. "b"
来源：http://blog.epnwcf.com/Article/details/glnuixkkh.sHtML

[T38] Lua：条件
来源：http://3g.vehdjk.com/Article/details/gclazwlzo.sHtML

if x > 0 then print("正") end
来源：http://baike.bbcook.cn/Article/details/grluunvsl.sHtML

[T39] Lua：模式匹配
来源：http://read.share.tarul.cn/Article/details/gnroddykj.sHtML

string.find(s, "%d+")
来源：http://baike.vehdjk.com/Article/details/goetwxzvo.sHtML

[T40] Lua：元表
来源：http://baike.fktsv.cn/Article/details/glwddqknk.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.bbcook.cn/Article/details/gghgnfgdx.sHtML

[T41] Perl：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gfsvtsqry.sHtML

print "Hello\n";
来源：http://3g.bbcook.cn/Article/details/gaemowgkl.sHtML

[T42] Perl：变量类型
来源：http://3g.fktsv.cn/Article/details/gqqeloirq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.sjlbkw.cn/Article/details/grpgagizx.sHtML

[T43] Perl：字符串插值
来源：http://read.share.tarul.cn/Article/details/guktiexeg.sHtML

"值: $a"
来源：http://m.share.epnwcf.com/Article/details/grxmovkta.sHtML

[T44] Perl：条件
来源：http://www.m.share.bbcook.cn/Article/details/gumluwvcl.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/glmxworcl.sHtML

[T45] Perl：数组遍历
来源：http://blog.epnwcf.com/Article/details/glygplkgh.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.sjlbkw.cn/Article/details/gtnnztbnu.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fktsv.cn/Article/details/geqcyginq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.bbcook.cn/Article/details/gydsorfie.sHtML

[T47] Perl：正则捕获
来源：http://www.share.sjlbkw.cn/Article/details/gihypsxzn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.bbcook.cn/Article/details/gtkujautv.sHtML

[T48] Perl：正则替换
来源：http://baike.epnwcf.com/Article/details/gccgdtcho.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fktsv.cn/Article/details/gsiiimdvh.sHtML

[T49] Perl：函数
来源：http://www.blog.epnwcf.com/Article/details/gjymzcctw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gydzwumab.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gynziyhsj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.bbcook.cn/Article/details/gqawacvic.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.sjlbkw.cn/Article/details/ggbhroqbc.sHtML

[T51] Scala：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gjqegnvwo.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gxhzqupzn.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gzchsfibv.sHtML

val a = 1;  var b = 2
来源：http://mobile.yfazqb.com/Article/details/gyugpzyrd.sHtML

[T53] Scala：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gayrjvwfo.sHtML

s"值: $b"
来源：http://www.m.share.sjlbkw.cn/Article/details/grovbpdgx.sHtML

[T54] Scala：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gbcdccosg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.bbcook.cn/Article/details/gbypgflrl.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/ggnnpzxvc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.yfazqb.com/Article/details/gimtegqbs.sHtML

[T56] Scala：样例类
来源：http://blog.bbcook.cn/Article/details/gjthtjrcv.sHtML

case class User(name: String, age: Int)
来源：http://m.share.vehdjk.com/Article/details/ghrxwykmq.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gcukucsal.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fktsv.cn/Article/details/gjwxsumdt.sHtML

[T58] Scala：函数定义
来源：http://mobile.fktsv.cn/Article/details/gvcptkvrl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.tarul.cn/Article/details/gcszksdrq.sHtML

[T59] Scala：循环
来源：http://www.blog.epnwcf.com/Article/details/gtptzahpa.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gctvagsna.sHtML

[T60] Scala：折叠
来源：http://read.share.bbcook.cn/Article/details/gheqxkuqo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.yfazqb.com/Article/details/ggdvorbtq.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzxtvpqhx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.vehdjk.com/Article/details/gnulopmxd.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gwxxpcddk.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.vehdjk.com/Article/details/ghpjmvemu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fktsv.cn/Article/details/ggpjvoobg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.sjlbkw.cn/Article/details/gucyxdigv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.epnwcf.com/Article/details/guxjdkzyb.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.yfazqb.com/Article/details/gfvbtvmty.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fktsv.cn/Article/details/gmuihwsqz.sHtML

[U04] Py：变量调试打印
来源：http://m.share.sjlbkw.cn/Article/details/gmeafkrcw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.bbcook.cn/Article/details/gpnazqdji.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.sjlbkw.cn/Article/details/glysmlyof.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gmtklkwrq.sHtML

[U06] Py：合并两个字典
来源：http://www.share.vehdjk.com/Article/details/goxytqebz.sHtML

{**a, **b}
来源：http://www.share.epnwcf.com/Article/details/gesxhxlki.sHtML

[U07] Py：反转字典键值
来源：http://mobile.epnwcf.com/Article/details/glbwmokcw.sHtML

{v: k for k, v in d.items()}
来源：http://baike.bbcook.cn/Article/details/glylnduzj.sHtML

[U08] Py：展平二维列表
来源：http://m.share.sjlbkw.cn/Article/details/gyskzgvri.sHtML

[y for x in nested for y in x]
来源：http://baike.epnwcf.com/Article/details/glxerlwcj.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.epnwcf.com/Article/details/gyklhaykk.sHtML

max(d, key=d.get)
来源：http://baike.tarul.cn/Article/details/glwznbejf.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnpfzhuc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fktsv.cn/Article/details/geozmzvcw.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.epnwcf.com/Article/details/gnylzmupt.sHtML

(x * 2 for x in arr)
来源：http://blog.epnwcf.com/Article/details/gmaxugayt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.epnwcf.com/Article/details/gkngdsvaa.sHtML

Counter(arr).most_common(3)
来源：http://mobile.epnwcf.com/Article/details/gaehibvma.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlyidbjs.sHtML

deque(maxlen=10)
来源：http://www.blog.bbcook.cn/Article/details/gmiiwkyqb.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fktsv.cn/Article/details/guonbhvhp.sHtML

defaultdict(list)
来源：http://m.share.yfazqb.com/Article/details/gkpnfbsay.sHtML

[U15] Py：高精度计时
来源：http://3g.tarul.cn/Article/details/gggpqgfxz.sHtML

t = time.perf_counter()
来源：http://www.share.yfazqb.com/Article/details/gozjbhpor.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.tarul.cn/Article/details/gksbxwxjf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.sjlbkw.cn/Article/details/gpuifvhdn.sHtML

[U17] Py：初始化日志
来源：http://www.share.bbcook.cn/Article/details/gcmoylukn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.bbcook.cn/Article/details/guqxezhua.sHtML

[U18] Py：预编译正则
来源：http://read.share.fktsv.cn/Article/details/gbzzdkmll.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fktsv.cn/Article/details/ghktnhspd.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.epnwcf.com/Article/details/gaxetufgl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.bbcook.cn/Article/details/gcdrymuvc.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.vehdjk.com/Article/details/glxjbuprp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.yfazqb.com/Article/details/govapsvlg.sHtML


<!-- 参考信息 -->