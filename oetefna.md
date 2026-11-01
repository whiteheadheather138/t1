代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.yfazqb.com/Article/details/gvboktgje.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.tarul.cn/Article/details/gubdgbeac.sHtML

time ./run.sh
来源：http://m.share.epnwcf.com/Article/details/gqtdwexhl.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqzifdzyw.sHtML

S. C / C++ 专题
来源：http://wap.fktsv.cn/Article/details/golokiivv.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gatqonilk.sHtML

[S01] C：Hello World
来源：http://www.share.fktsv.cn/Article/details/grhxyyqym.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/gyrcelhkl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/grnfynrqb.sHtML

[S02] C：变量与格式化输出
来源：http://blog.bbcook.cn/Article/details/gvrjxopul.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fktsv.cn/Article/details/gfmfoakjk.sHtML

[S03] C：读入整数
来源：http://baike.fktsv.cn/Article/details/gybamlrux.sHtML

int x; scanf("%d", &x);
来源：http://read.share.vehdjk.com/Article/details/gmkjqzaky.sHtML

[S04] C：字符串复制
来源：http://www.share.vehdjk.com/Article/details/gcmxxgrns.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fktsv.cn/Article/details/gaebijhce.sHtML

[S05] C：字符串长度
来源：http://www.share.epnwcf.com/Article/details/gyskxfvac.sHtML

strlen(s)
来源：http://read.share.vehdjk.com/Article/details/gzweauups.sHtML

[S06] C：字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gklxqoack.sHtML

strcmp(a, b) == 0
来源：http://3g.fktsv.cn/Article/details/guniqflnk.sHtML

[S07] C：数组遍历求和
来源：http://m.share.yfazqb.com/Article/details/gqneiryjx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fktsv.cn/Article/details/guvkxhims.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.bbcook.cn/Article/details/gboiieshs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/gapqajttg.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/glszcvjzc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fktsv.cn/Article/details/gsxxfoymw.sHtML

[S10] C：指针与解引用
来源：http://www.share.yfazqb.com/Article/details/gvcceybjb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.vehdjk.com/Article/details/gdpwyjwjm.sHtML

[S11] C：逐行读文件
来源：http://3g.tarul.cn/Article/details/gynrqamng.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.vehdjk.com/Article/details/gwarfpfcu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gonmjajft.sHtML

fclose(f);
来源：http://wap.yfazqb.com/Article/details/glyzpxlwb.sHtML

[S12] C：写文件
来源：http://m.share.yfazqb.com/Article/details/gcshwnhwf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.epnwcf.com/Article/details/gmchhmasy.sHtML

[S13] C：宏定义
来源：http://3g.fktsv.cn/Article/details/gazjbvwsp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.epnwcf.com/Article/details/gtvunrqcy.sHtML

[S14] C：枚举
来源：http://www.share.bbcook.cn/Article/details/gjhveompa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.sjlbkw.cn/Article/details/gzbvekkck.sHtML

[S15] C：类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gfnltkvei.sHtML

(double) a / b
来源：http://www.share.vehdjk.com/Article/details/gfqobqley.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/ghgpxrcvp.sHtML

x |= (1 << 3);
来源：http://www.m.share.yfazqb.com/Article/details/gvwhljagc.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gdmszeaib.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.sjlbkw.cn/Article/details/ghloocgkx.sHtML

[S18] C：命令行参数
来源：http://read.share.vehdjk.com/Article/details/gtxplrmgc.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gasqznngk.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/gvjvjkpxv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gcsrovnkc.sHtML

[S20] C：二分查找
来源：http://blog.yfazqb.com/Article/details/gfjxshhnk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gszlbkdcj.sHtML

[S21] C：字符类别判断
来源：http://3g.bbcook.cn/Article/details/gmmriontp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.sjlbkw.cn/Article/details/glcbwqjoz.sHtML

[S22] C：字符串转数字
来源：http://m.share.tarul.cn/Article/details/gruggdwjl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.bbcook.cn/Article/details/gyuulchvr.sHtML

[S23] C：随机数
来源：http://wap.tarul.cn/Article/details/gwwasczim.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.sjlbkw.cn/Article/details/gygpdojxn.sHtML

[S24] C：获取本地时间
来源：http://www.share.sjlbkw.cn/Article/details/ghetryqbd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.epnwcf.com/Article/details/gonpdulvd.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/glkkjlvuv.sHtML

memcpy(dst, src, n);
来源：http://blog.epnwcf.com/Article/details/glbtahgti.sHtML

[S26] C：内存清零
来源：http://www.m.share.vehdjk.com/Article/details/guqnjynsn.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.bbcook.cn/Article/details/ghfrcspao.sHtML

[S27] C：定义常量
来源：http://baike.tarul.cn/Article/details/gkilodolb.sHtML

const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gcsjleeta.sHtML

[S28] C：静态变量
来源：http://www.blog.sjlbkw.cn/Article/details/gzlbcuqrl.sHtML

static int counter = 0;
来源：http://m.share.epnwcf.com/Article/details/gdnmqgnpz.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/gxhxbputg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gittewuqz.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gbhhkxojy.sHtML

#ifndef X_H
来源：http://m.share.yfazqb.com/Article/details/gfyehtrai.sHtML

#define X_H
来源：http://www.blog.fktsv.cn/Article/details/guktnszas.sHtML

#endif
来源：http://wap.fktsv.cn/Article/details/gcdpdnmtl.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/gnpfuabed.sHtML

#include <iostream>
来源：http://wap.vehdjk.com/Article/details/gutsyydav.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.epnwcf.com/Article/details/gvarmoxan.sHtML

[S32] C++：字符串
来源：http://blog.bbcook.cn/Article/details/gcfsrxevk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.vehdjk.com/Article/details/gdqwbnwaf.sHtML

[S33] C++：vector 增删
来源：http://m.share.tarul.cn/Article/details/gmwzaemod.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.tarul.cn/Article/details/gurewefnx.sHtML

[S34] C++：遍历 vector
来源：http://baike.epnwcf.com/Article/details/gkfvnihnk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fktsv.cn/Article/details/gymjnxcom.sHtML

[S35] C++：map
来源：http://wap.sjlbkw.cn/Article/details/gqnznobqm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gyukxgoew.sHtML

[S36] C++：unordered_map
来源：http://baike.bbcook.cn/Article/details/ghzdmmpgx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gqbksbgzi.sHtML

[S37] C++：set
来源：http://www.share.yfazqb.com/Article/details/gwrfeqqkl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fktsv.cn/Article/details/gvqdsnmyq.sHtML

[S38] C++：排序
来源：http://www.share.vehdjk.com/Article/details/gztdmdtkx.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.tarul.cn/Article/details/gacsqysaw.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gxkcnyvkl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.yfazqb.com/Article/details/graeoomcg.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/gbfcrczvu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/glyhpzcpj.sHtML

[S41] C++：类与构造函数
来源：http://mobile.epnwcf.com/Article/details/goedninpv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.vehdjk.com/Article/details/gfrzmrtbw.sHtML

[S42] C++：继承与虚函数
来源：http://baike.tarul.cn/Article/details/grlgnralk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/gibhotaan.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/gqmkziwsg.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.bbcook.cn/Article/details/gjakbgxrm.sHtML

[S44] C++：引用传参
来源：http://mobile.sjlbkw.cn/Article/details/ggjhcawgf.sHtML

void inc(int &x) { ++x; }
来源：http://baike.vehdjk.com/Article/details/gmvptthrz.sHtML

[S45] C++：lambda
来源：http://blog.sjlbkw.cn/Article/details/galnusxue.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.bbcook.cn/Article/details/gsiiposkn.sHtML

[S46] C++：函数模板
来源：http://mobile.epnwcf.com/Article/details/gjfsruims.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.epnwcf.com/Article/details/gthycushi.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.tarul.cn/Article/details/gfnqibcaj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.tarul.cn/Article/details/gszrbfduc.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gqctdnhzc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fktsv.cn/Article/details/gxnldpzav.sHtML

while (std::getline(in, line)) { }
来源：http://3g.epnwcf.com/Article/details/grmfsmjss.sHtML

[S49] C++：写文件
来源：http://wap.fktsv.cn/Article/details/gvzisgvsa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/gtczdfjfw.sHtML

[S50] C++：格式化数字
来源：http://3g.fktsv.cn/Article/details/gayzttnvp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gsiooziso.sHtML

[S51] C++：显式类型转换
来源：http://blog.sjlbkw.cn/Article/details/ginxjsyof.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/ghgdyxkmy.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.yfazqb.com/Article/details/gepdgvwmm.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.bbcook.cn/Article/details/geyddrvox.sHtML

[S53] C++：移动语义
来源：http://www.blog.tarul.cn/Article/details/gstmzrmrd.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.sjlbkw.cn/Article/details/gzylosyqn.sHtML

[S54] C++：异常处理
来源：http://m.share.bbcook.cn/Article/details/gexptapbo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.tarul.cn/Article/details/gvadkqbip.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.yfazqb.com/Article/details/gdkuyincz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.tarul.cn/Article/details/gdgghiblf.sHtML

[S56] C++：optional
来源：http://mobile.tarul.cn/Article/details/goeyijalb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.sjlbkw.cn/Article/details/ganttojik.sHtML

[S57] C++：编译期常量
来源：http://www.share.bbcook.cn/Article/details/ggqsesrry.sHtML

constexpr int N = 10;
来源：http://mobile.tarul.cn/Article/details/gytssyylw.sHtML

[S58] C++：命名空间
来源：http://www.m.share.epnwcf.com/Article/details/gtavdasxf.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.vehdjk.com/Article/details/gcaidltbk.sHtML

[S59] C++：静态断言
来源：http://baike.bbcook.cn/Article/details/guagydfsl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fktsv.cn/Article/details/grxogpvqk.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.bbcook.cn/Article/details/ggyjmtpoc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.bbcook.cn/Article/details/gyrxhvpea.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwmymfbnu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.sjlbkw.cn/Article/details/gixrmnhch.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gqsrqnfgc.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/guimekdme.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/ghgodczoz.sHtML

[T02] Kotlin：变量
来源：http://www.blog.tarul.cn/Article/details/gcgrmuxzw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxebakww.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/ggfdplmbu.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/gugvcqizy.sHtML

[T04] Kotlin：空安全
来源：http://m.share.sjlbkw.cn/Article/details/gxohkiuar.sHtML

val n: String? = null;  n?.length
来源：http://www.share.tarul.cn/Article/details/gggjcxwfu.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.tarul.cn/Article/details/gebkfpvme.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gyzfftahd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gyoubjlmz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gsfcyzvkj.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/ggzgdawlx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.sjlbkw.cn/Article/details/gpkaxbxxf.sHtML

[T08] Kotlin：数据类
来源：http://m.share.vehdjk.com/Article/details/gfubldryv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.vehdjk.com/Article/details/gdblsueqy.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fktsv.cn/Article/details/gpdjyfgpv.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.vehdjk.com/Article/details/ghlyxzvva.sHtML

[T10] Kotlin：默认参数
来源：http://3g.tarul.cn/Article/details/ginbbmfpt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.epnwcf.com/Article/details/gtcwegwyp.sHtML

[T11] Kotlin：协程
来源：http://www.blog.epnwcf.com/Article/details/gjlfjuzfj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.bbcook.cn/Article/details/gycsujpzu.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fktsv.cn/Article/details/gixeulbkk.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.epnwcf.com/Article/details/gjqzhgxbw.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.vehdjk.com/Article/details/grpltqkbb.sHtML

val m = mapOf("a" to 1)
来源：http://3g.bbcook.cn/Article/details/gctjyorte.sHtML

[T14] Kotlin：循环
来源：http://wap.bbcook.cn/Article/details/gsxexpfgb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gcyltninn.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.vehdjk.com/Article/details/ghgtbjysi.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.epnwcf.com/Article/details/gwtzxgpsu.sHtML

[T16] Swift：Hello World
来源：http://blog.tarul.cn/Article/details/gkspinynh.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/gunoevcdo.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.yfazqb.com/Article/details/ghzxdoaqy.sHtML

var a = 1;  let b = 2
来源：http://blog.epnwcf.com/Article/details/gruprlkbt.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gkkbncsmk.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/gcrbsxipu.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/gsgwtvrkz.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.yfazqb.com/Article/details/gsdwjxnyn.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/giyywiwkr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.yfazqb.com/Article/details/gyajbqyxi.sHtML

[T21] Swift：遍历
来源：http://3g.vehdjk.com/Article/details/gdizvuhcs.sHtML

for x in a { print(x) }
来源：http://baike.vehdjk.com/Article/details/gniyatcqt.sHtML

[T22] Swift：字典
来源：http://3g.tarul.cn/Article/details/gsmdjsqjw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.yfazqb.com/Article/details/gatyumlht.sHtML

[T23] Swift：函数
来源：http://mobile.tarul.cn/Article/details/gcqxerrdg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.tarul.cn/Article/details/gcbvhajgc.sHtML

[T24] Swift：闭包
来源：http://m.share.epnwcf.com/Article/details/gimtdqlad.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.yfazqb.com/Article/details/godmhrege.sHtML

[T25] Swift：结构体
来源：http://mobile.bbcook.cn/Article/details/gcfgrcair.sHtML

struct P { var x: Int }
来源：http://read.share.bbcook.cn/Article/details/glcznorgf.sHtML

[T26] Swift：类与重写
来源：http://www.share.yfazqb.com/Article/details/gflurzqnk.sHtML

class A: Base { override func f() {} }
来源：http://3g.sjlbkw.cn/Article/details/gngqepkve.sHtML

[T27] Swift：错误处理
来源：http://blog.sjlbkw.cn/Article/details/gixondtth.sHtML

do { try f() } catch { print(error) }
来源：http://wap.bbcook.cn/Article/details/gazmzfxhq.sHtML

[T28] Swift：枚举
来源：http://www.blog.epnwcf.com/Article/details/guzafzobh.sHtML

enum Color { case red, green }
来源：http://blog.vehdjk.com/Article/details/gtfoekhnj.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.sjlbkw.cn/Article/details/gmyulyete.sHtML

guard let x = opt else { return }
来源：http://read.share.sjlbkw.cn/Article/details/gdtfzstff.sHtML

[T30] Swift：协议
来源：http://read.share.sjlbkw.cn/Article/details/gwzipjtuq.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.yfazqb.com/Article/details/gikdctnlv.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/gizztfwaj.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/ghfjliaee.sHtML

[T32] Lua：局部变量
来源：http://wap.yfazqb.com/Article/details/gaafwjxby.sHtML

local a = 1
来源：http://3g.epnwcf.com/Article/details/gtsqifext.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fktsv.cn/Article/details/gnxgfbisp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.sjlbkw.cn/Article/details/gphtzdsan.sHtML

[T34] Lua：遍历表
来源：http://www.share.fktsv.cn/Article/details/gqhjpqkbi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fktsv.cn/Article/details/gngytkikw.sHtML

[T35] Lua：字典表
来源：http://www.m.share.vehdjk.com/Article/details/gixmpqxor.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.epnwcf.com/Article/details/gjwnuotep.sHtML

[T36] Lua：函数
来源：http://baike.tarul.cn/Article/details/gyxnsazli.sHtML

function add(a, b) return a + b end
来源：http://3g.fktsv.cn/Article/details/gytdxdmce.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gfmvtyqmm.sHtML

"a" .. "b"
来源：http://3g.fktsv.cn/Article/details/gkpqhvifn.sHtML

[T38] Lua：条件
来源：http://blog.bbcook.cn/Article/details/gubkmftat.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.vehdjk.com/Article/details/ghejscoeb.sHtML

[T39] Lua：模式匹配
来源：http://blog.yfazqb.com/Article/details/gzdpulxih.sHtML

string.find(s, "%d+")
来源：http://baike.vehdjk.com/Article/details/grallndxt.sHtML

[T40] Lua：元表
来源：http://www.share.sjlbkw.cn/Article/details/gevidkael.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhbmgvvf.sHtML

[T41] Perl：Hello World
来源：http://mobile.yfazqb.com/Article/details/gilhvhuok.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/gmemznbvk.sHtML

[T42] Perl：变量类型
来源：http://read.share.tarul.cn/Article/details/guiazvoti.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.bbcook.cn/Article/details/gayurrtoi.sHtML

[T43] Perl：字符串插值
来源：http://mobile.tarul.cn/Article/details/gvbtparbj.sHtML

"值: $a"
来源：http://www.blog.sjlbkw.cn/Article/details/gdqdxfgqk.sHtML

[T44] Perl：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gzebecznw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.tarul.cn/Article/details/gftkskjvq.sHtML

[T45] Perl：数组遍历
来源：http://3g.fktsv.cn/Article/details/gzvbovzua.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fktsv.cn/Article/details/gecmcgqot.sHtML

[T46] Perl：哈希操作
来源：http://read.share.tarul.cn/Article/details/giuxwugqf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fktsv.cn/Article/details/gmodmhhmf.sHtML

[T47] Perl：正则捕获
来源：http://mobile.sjlbkw.cn/Article/details/gdbdmmpay.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.sjlbkw.cn/Article/details/gurxbwsut.sHtML

[T48] Perl：正则替换
来源：http://baike.fktsv.cn/Article/details/genqpavei.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fktsv.cn/Article/details/gytfsesqt.sHtML

[T49] Perl：函数
来源：http://blog.fktsv.cn/Article/details/grgzebtck.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gqyfqwfrg.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gsfmcgwts.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.yfazqb.com/Article/details/glnjesgei.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.vehdjk.com/Article/details/gyuwbokxq.sHtML

[T51] Scala：Hello World
来源：http://3g.yfazqb.com/Article/details/gtbvgcvnx.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gzrgpiufe.sHtML

[T52] Scala：变量
来源：http://www.m.share.vehdjk.com/Article/details/giwktyeny.sHtML

val a = 1;  var b = 2
来源：http://www.blog.bbcook.cn/Article/details/gfapnxykr.sHtML

[T53] Scala：字符串插值
来源：http://3g.yfazqb.com/Article/details/gzdhaperk.sHtML

s"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gmobbuhdr.sHtML

[T54] Scala：集合映射
来源：http://read.share.epnwcf.com/Article/details/goxidtosi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gngugmdrt.sHtML

[T55] Scala：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/glmuaeffx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.epnwcf.com/Article/details/gnluofbyk.sHtML

[T56] Scala：样例类
来源：http://read.share.epnwcf.com/Article/details/giazaxjvx.sHtML

case class User(name: String, age: Int)
来源：http://3g.bbcook.cn/Article/details/gripqergc.sHtML

[T57] Scala：模式匹配
来源：http://wap.yfazqb.com/Article/details/gqkggpkjt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gxwxranld.sHtML

[T58] Scala：函数定义
来源：http://m.share.yfazqb.com/Article/details/gepqcuuau.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.yfazqb.com/Article/details/gmczfjgzj.sHtML

[T59] Scala：循环
来源：http://m.share.bbcook.cn/Article/details/guxochsio.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/golqtyrec.sHtML

[T60] Scala：折叠
来源：http://m.share.vehdjk.com/Article/details/geknzdngz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/gywyjtbtu.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gfbxsqfse.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gqwgfgwkw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkycmarug.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.bbcook.cn/Article/details/gpntafcgo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.yfazqb.com/Article/details/gbcodmjjj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.yfazqb.com/Article/details/gjrzlsoag.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.vehdjk.com/Article/details/gmziijpwp.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.yfazqb.com/Article/details/gcjlbvtwx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.epnwcf.com/Article/details/gtbgcyvuo.sHtML

[U04] Py：变量调试打印
来源：http://wap.epnwcf.com/Article/details/gqrpwmpyu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.sjlbkw.cn/Article/details/gtgwuotkw.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.epnwcf.com/Article/details/gmgpxrxoe.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/glxrtpamk.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.bbcook.cn/Article/details/gcdpczqpu.sHtML

{**a, **b}
来源：http://m.share.yfazqb.com/Article/details/ggmutkffk.sHtML

[U07] Py：反转字典键值
来源：http://mobile.epnwcf.com/Article/details/gvbzzhkpt.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/glfrgrpfx.sHtML

[U08] Py：展平二维列表
来源：http://3g.sjlbkw.cn/Article/details/gmxatnkvv.sHtML

[y for x in nested for y in x]
来源：http://mobile.vehdjk.com/Article/details/gamuwaiym.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.bbcook.cn/Article/details/gmgzcxbgv.sHtML

max(d, key=d.get)
来源：http://3g.vehdjk.com/Article/details/gfimytlms.sHtML

[U10] Py：按值排序字典
来源：http://mobile.tarul.cn/Article/details/gcovcmxjj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.yfazqb.com/Article/details/ghotghhbo.sHtML

[U11] Py：生成器表达式
来源：http://wap.bbcook.cn/Article/details/gdedglxwe.sHtML

(x * 2 for x in arr)
来源：http://3g.yfazqb.com/Article/details/gojpxdrut.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.bbcook.cn/Article/details/genemdtwe.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.tarul.cn/Article/details/gprzlwryb.sHtML

[U13] Py：固定长度队列
来源：http://3g.tarul.cn/Article/details/ggbecuork.sHtML

deque(maxlen=10)
来源：http://www.share.vehdjk.com/Article/details/gqdamlrey.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.tarul.cn/Article/details/gngxybulk.sHtML

defaultdict(list)
来源：http://m.share.sjlbkw.cn/Article/details/gkzywazhi.sHtML

[U15] Py：高精度计时
来源：http://www.share.epnwcf.com/Article/details/gkaedlnlx.sHtML

t = time.perf_counter()
来源：http://www.blog.sjlbkw.cn/Article/details/gbacqqpev.sHtML

[U16] Py：命令行参数解析
来源：http://wap.epnwcf.com/Article/details/grzkdeshf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.vehdjk.com/Article/details/gvdzvspcn.sHtML

[U17] Py：初始化日志
来源：http://read.share.yfazqb.com/Article/details/gqjkmelic.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.tarul.cn/Article/details/gmkyaclzy.sHtML

[U18] Py：预编译正则
来源：http://mobile.vehdjk.com/Article/details/gwjgtwsjo.sHtML

pat = re.compile(r"\d+")
来源：http://wap.yfazqb.com/Article/details/gyymizzqy.sHtML

[U19] Py：正则替换带回调
来源：http://blog.vehdjk.com/Article/details/guroilojw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.yfazqb.com/Article/details/ghaskapkn.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fktsv.cn/Article/details/gaktodfna.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.sjlbkw.cn/Article/details/gpzdypvxn.sHtML


<!-- 参考信息 -->