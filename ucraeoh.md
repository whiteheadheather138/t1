代发 wailian999

S. C / C++ 专题
来源：http://3g.tarul.cn/Article/details/gxdmhiqlx.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtmdmzieg.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/ggtnwjfic.sHtML

#include <stdio.h>
来源：http://wap.sjlbkw.cn/Article/details/glzzolfxx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/gapeljcxj.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.vehdjk.com/Article/details/gzrfgquyv.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.tarul.cn/Article/details/gprzyjiwm.sHtML

[S03] C：读入整数
来源：http://blog.fktsv.cn/Article/details/gagzlpokq.sHtML

int x; scanf("%d", &x);
来源：http://3g.epnwcf.com/Article/details/gmljdfsiv.sHtML

[S04] C：字符串复制
来源：http://3g.tarul.cn/Article/details/gxgxmxnef.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fktsv.cn/Article/details/gsafoctnv.sHtML

[S05] C：字符串长度
来源：http://m.share.fktsv.cn/Article/details/gincthvyl.sHtML

strlen(s)
来源：http://blog.vehdjk.com/Article/details/gkswxijmy.sHtML

[S06] C：字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gevhocyvo.sHtML

strcmp(a, b) == 0
来源：http://3g.vehdjk.com/Article/details/gmiwdqwhv.sHtML

[S07] C：数组遍历求和
来源：http://baike.yfazqb.com/Article/details/geywwswyg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/gqhryywbr.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.sjlbkw.cn/Article/details/gaqutpevn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.yfazqb.com/Article/details/gdwaktynh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.yfazqb.com/Article/details/ggaymjelo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.epnwcf.com/Article/details/giimykato.sHtML

[S10] C：指针与解引用
来源：http://baike.bbcook.cn/Article/details/gfydcaqro.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gclfuvalx.sHtML

[S11] C：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gslfpuwab.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrchrowt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.vehdjk.com/Article/details/glbofwrho.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/gotctramu.sHtML

[S12] C：写文件
来源：http://www.blog.fktsv.cn/Article/details/gbfzaevey.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.yfazqb.com/Article/details/glzthyznl.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gqbzwrggp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.epnwcf.com/Article/details/goqelzvon.sHtML

[S14] C：枚举
来源：http://read.share.tarul.cn/Article/details/ggwyoyydb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/gjoiuvlzn.sHtML

[S15] C：类型转换
来源：http://m.share.bbcook.cn/Article/details/gcxcjpwxr.sHtML

(double) a / b
来源：http://wap.vehdjk.com/Article/details/gksnlszur.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gadrpzijf.sHtML

x |= (1 << 3);
来源：http://www.share.sjlbkw.cn/Article/details/gtpmymvsl.sHtML

[S17] C：安全拼接字符串
来源：http://blog.bbcook.cn/Article/details/ghswlnhaz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fktsv.cn/Article/details/gpirfktnp.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/gdcyvqqmj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.bbcook.cn/Article/details/gojoritmd.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/gannwdlxz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/govoobgfx.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gkntlucsa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gvswesytq.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/ggnoqbqas.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.tarul.cn/Article/details/gbddpsoeo.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fktsv.cn/Article/details/gsayzwxay.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.vehdjk.com/Article/details/gxsnrdqmm.sHtML

[S23] C：随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlbmauin.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/gvxznptbj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.vehdjk.com/Article/details/gavtfrgii.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.tarul.cn/Article/details/gtjiuslgp.sHtML

[S25] C：内存拷贝
来源：http://mobile.vehdjk.com/Article/details/gfqmsbnsn.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.yfazqb.com/Article/details/gisokcaor.sHtML

[S26] C：内存清零
来源：http://www.share.bbcook.cn/Article/details/gepptkyiw.sHtML

memset(a, 0, sizeof a);
来源：http://3g.yfazqb.com/Article/details/gjqzehwzs.sHtML

[S27] C：定义常量
来源：http://3g.sjlbkw.cn/Article/details/gyvqpgwwr.sHtML

const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gbueoyogt.sHtML

[S28] C：静态变量
来源：http://www.m.share.tarul.cn/Article/details/ghawdwflp.sHtML

static int counter = 0;
来源：http://www.m.share.vehdjk.com/Article/details/gteqqqdtp.sHtML

[S29] C：变参函数
来源：http://read.share.fktsv.cn/Article/details/gpioepjnv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.sjlbkw.cn/Article/details/gwkyendme.sHtML

[S30] C：头文件保护
来源：http://www.share.epnwcf.com/Article/details/gcusxuonq.sHtML

#ifndef X_H
来源：http://www.share.vehdjk.com/Article/details/gpvrpdcby.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/ghwxbavbj.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/gqynhgcrj.sHtML

[S31] C++：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gbutrqiyx.sHtML

#include <iostream>
来源：http://www.share.epnwcf.com/Article/details/gcmzwdged.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.sjlbkw.cn/Article/details/gphsxyjyy.sHtML

[S32] C++：字符串
来源：http://baike.tarul.cn/Article/details/gpfchhsar.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.yfazqb.com/Article/details/gzinexlvv.sHtML

[S33] C++：vector 增删
来源：http://baike.tarul.cn/Article/details/ggtjndqif.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.vehdjk.com/Article/details/gcoqzlbjb.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/gxgsufqme.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.sjlbkw.cn/Article/details/gogiqzljh.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/goywjaerx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/ggzaofmmk.sHtML

[S36] C++：unordered_map
来源：http://mobile.epnwcf.com/Article/details/gtpprzdwp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gxzftwvqr.sHtML

[S37] C++：set
来源：http://wap.vehdjk.com/Article/details/gkjnvteza.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.vehdjk.com/Article/details/gbtskjqdr.sHtML

[S38] C++：排序
来源：http://mobile.tarul.cn/Article/details/gnrdlelxn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gqrcfjrjm.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/gxaucjzyd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/guualcaka.sHtML

[S40] C++：查找元素
来源：http://baike.vehdjk.com/Article/details/gpzhvpylh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.yfazqb.com/Article/details/gurgyxhuu.sHtML

[S41] C++：类与构造函数
来源：http://baike.vehdjk.com/Article/details/gihhuxngt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.yfazqb.com/Article/details/gcqpfwdxh.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/gzreupkbt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.epnwcf.com/Article/details/gtjdczzwy.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/gqdscssqs.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdbvixnf.sHtML

[S44] C++：引用传参
来源：http://www.m.share.vehdjk.com/Article/details/gmaiyqrld.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/gmmfmhkig.sHtML

[S45] C++：lambda
来源：http://mobile.epnwcf.com/Article/details/gwjulkxma.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/genlvfqba.sHtML

[S46] C++：函数模板
来源：http://www.blog.epnwcf.com/Article/details/gcqglyvjw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.vehdjk.com/Article/details/gcfnmfuqh.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/gbqizlxuc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.vehdjk.com/Article/details/gwkttodct.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gzddzbams.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.bbcook.cn/Article/details/gzrulrzmq.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/gebnrbxdk.sHtML

[S49] C++：写文件
来源：http://wap.epnwcf.com/Article/details/gdrsmaomv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.tarul.cn/Article/details/guetyxpug.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fktsv.cn/Article/details/gdzetzepa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gvjpendjl.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gcypxnfck.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gdkmxgzkz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.vehdjk.com/Article/details/gtxqosjfc.sHtML

int size() const noexcept { return n_; }
来源：http://3g.bbcook.cn/Article/details/gvaaxzvzo.sHtML

[S53] C++：移动语义
来源：http://www.m.share.tarul.cn/Article/details/gsgusaqvu.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fktsv.cn/Article/details/gotgpkqtb.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/gifcklnwe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fktsv.cn/Article/details/grpqumiis.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gloebkizo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.bbcook.cn/Article/details/gzudlofqu.sHtML

[S56] C++：optional
来源：http://3g.yfazqb.com/Article/details/gosjyvewl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/gjuetssub.sHtML

[S57] C++：编译期常量
来源：http://mobile.fktsv.cn/Article/details/gaeodmzgp.sHtML

constexpr int N = 10;
来源：http://read.share.vehdjk.com/Article/details/gsnogrjms.sHtML

[S58] C++：命名空间
来源：http://www.blog.vehdjk.com/Article/details/gixstvauh.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.tarul.cn/Article/details/gwwrouxfy.sHtML

[S59] C++：静态断言
来源：http://3g.bbcook.cn/Article/details/ghdwuljrf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.yfazqb.com/Article/details/gtigtbpcg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.epnwcf.com/Article/details/glsffzrnt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.yfazqb.com/Article/details/gzjqunzbt.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqqthdzdy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/gykursyld.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gtuduyebu.sHtML

[T01] Kotlin：Hello World
来源：http://3g.bbcook.cn/Article/details/gnrafwmka.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gbvnqjvpx.sHtML

[T02] Kotlin：变量
来源：http://wap.bbcook.cn/Article/details/gvggirdya.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.vehdjk.com/Article/details/gtctkyzst.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.bbcook.cn/Article/details/gkyazzcsb.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gbuyvhrit.sHtML

[T04] Kotlin：空安全
来源：http://read.share.epnwcf.com/Article/details/ghbdteqaa.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.epnwcf.com/Article/details/ghicxtreb.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.yfazqb.com/Article/details/gfckzgdhu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.sjlbkw.cn/Article/details/ggbxkhchr.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.tarul.cn/Article/details/gdazgrspc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gsseynmsv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gfirevkop.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.sjlbkw.cn/Article/details/ggiplwspe.sHtML

[T08] Kotlin：数据类
来源：http://read.share.vehdjk.com/Article/details/gaxsrhqca.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.bbcook.cn/Article/details/gbchxhgmj.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.bbcook.cn/Article/details/gqcolosdv.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.sjlbkw.cn/Article/details/gsdridzln.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.epnwcf.com/Article/details/ggcskkebr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fktsv.cn/Article/details/gdzpzkuop.sHtML

[T11] Kotlin：协程
来源：http://blog.yfazqb.com/Article/details/ggimywloh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.sjlbkw.cn/Article/details/gdosyqaar.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.vehdjk.com/Article/details/gohzqxasc.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.epnwcf.com/Article/details/gozttulcj.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.bbcook.cn/Article/details/gtblxaflv.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fktsv.cn/Article/details/gexptusdh.sHtML

[T14] Kotlin：循环
来源：http://read.share.sjlbkw.cn/Article/details/gpjgnopkj.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/guvhgdjtx.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.sjlbkw.cn/Article/details/goneuwdlz.sHtML

interface Shape { fun area(): Double }
来源：http://baike.yfazqb.com/Article/details/gcmlenvrn.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/guxcvgqym.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gocerpapt.sHtML

[T17] Swift：变量与常量
来源：http://3g.tarul.cn/Article/details/grqthufsx.sHtML

var a = 1;  let b = 2
来源：http://baike.sjlbkw.cn/Article/details/gvupgxymo.sHtML

[T18] Swift：字符串插值
来源：http://baike.vehdjk.com/Article/details/gyuweryen.sHtML

"值: \(b)"
来源：http://www.share.tarul.cn/Article/details/gccjfnfwa.sHtML

[T19] Swift：可选绑定
来源：http://3g.epnwcf.com/Article/details/gcntkmvhq.sHtML

if let n = opt { print(n) }
来源：http://read.share.sjlbkw.cn/Article/details/gdsyvxopc.sHtML

[T20] Swift：数组操作
来源：http://m.share.epnwcf.com/Article/details/grtbwovkn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.tarul.cn/Article/details/gwpahfbvt.sHtML

[T21] Swift：遍历
来源：http://baike.yfazqb.com/Article/details/gqnxlhglx.sHtML

for x in a { print(x) }
来源：http://m.share.tarul.cn/Article/details/gjlfrnlgo.sHtML

[T22] Swift：字典
来源：http://read.share.fktsv.cn/Article/details/gijykfotz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.tarul.cn/Article/details/gshrhfedi.sHtML

[T23] Swift：函数
来源：http://www.m.share.vehdjk.com/Article/details/glbsihusz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.yfazqb.com/Article/details/gkrxvlhlg.sHtML

[T24] Swift：闭包
来源：http://blog.epnwcf.com/Article/details/ggvgliqnt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.tarul.cn/Article/details/guwfcperw.sHtML

[T25] Swift：结构体
来源：http://www.m.share.sjlbkw.cn/Article/details/gsldtbcqa.sHtML

struct P { var x: Int }
来源：http://m.share.yfazqb.com/Article/details/gyrzmmmjj.sHtML

[T26] Swift：类与重写
来源：http://m.share.yfazqb.com/Article/details/grwwpeosz.sHtML

class A: Base { override func f() {} }
来源：http://wap.bbcook.cn/Article/details/gazalpfsp.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/gzmkoxfbw.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.bbcook.cn/Article/details/gmzvsagtz.sHtML

[T28] Swift：枚举
来源：http://3g.sjlbkw.cn/Article/details/gfcmbmdcj.sHtML

enum Color { case red, green }
来源：http://baike.yfazqb.com/Article/details/gdvuihoal.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.tarul.cn/Article/details/glnlfmlzz.sHtML

guard let x = opt else { return }
来源：http://www.blog.vehdjk.com/Article/details/gchaoskjj.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/gezgwadix.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.sjlbkw.cn/Article/details/gctmlzfaw.sHtML

[T31] Lua：Hello World
来源：http://baike.tarul.cn/Article/details/gifbxwvyl.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gryhrngqz.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsrgwodf.sHtML

local a = 1
来源：http://www.m.share.tarul.cn/Article/details/gkowywrzm.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.vehdjk.com/Article/details/gyglaqlet.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.yfazqb.com/Article/details/gyyqrggps.sHtML

[T34] Lua：遍历表
来源：http://www.share.yfazqb.com/Article/details/gdzqdinos.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.tarul.cn/Article/details/gggqneydz.sHtML

[T35] Lua：字典表
来源：http://wap.tarul.cn/Article/details/gldnbkyyd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.tarul.cn/Article/details/gwmxdvqix.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/gcfomarss.sHtML

function add(a, b) return a + b end
来源：http://www.share.yfazqb.com/Article/details/gdoihoaua.sHtML

[T37] Lua：字符串拼接
来源：http://baike.tarul.cn/Article/details/gwhmtcypf.sHtML

"a" .. "b"
来源：http://wap.yfazqb.com/Article/details/gjfxpvpep.sHtML

[T38] Lua：条件
来源：http://m.share.fktsv.cn/Article/details/gqalgyzwy.sHtML

if x > 0 then print("正") end
来源：http://www.share.epnwcf.com/Article/details/grzomkdjk.sHtML

[T39] Lua：模式匹配
来源：http://m.share.epnwcf.com/Article/details/gmusbagcj.sHtML

string.find(s, "%d+")
来源：http://m.share.epnwcf.com/Article/details/gjgkjjbhm.sHtML

[T40] Lua：元表
来源：http://3g.yfazqb.com/Article/details/gytwyvweo.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.tarul.cn/Article/details/gjtjmtzyv.sHtML

[T41] Perl：Hello World
来源：http://wap.fktsv.cn/Article/details/ggutmximm.sHtML

print "Hello\n";
来源：http://www.m.share.tarul.cn/Article/details/gnvbwdssy.sHtML

[T42] Perl：变量类型
来源：http://m.share.bbcook.cn/Article/details/goegnedmb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fktsv.cn/Article/details/glvdizsvs.sHtML

[T43] Perl：字符串插值
来源：http://wap.tarul.cn/Article/details/gzxkktucz.sHtML

"值: $a"
来源：http://www.blog.fktsv.cn/Article/details/gacpltgpx.sHtML

[T44] Perl：条件
来源：http://3g.fktsv.cn/Article/details/gwxhivxwu.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.vehdjk.com/Article/details/gfbjaahez.sHtML

[T45] Perl：数组遍历
来源：http://read.share.vehdjk.com/Article/details/gzhxevzov.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.tarul.cn/Article/details/gixkqfmea.sHtML

[T46] Perl：哈希操作
来源：http://www.share.sjlbkw.cn/Article/details/guiaazwmg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.vehdjk.com/Article/details/goiiljnyv.sHtML

[T47] Perl：正则捕获
来源：http://blog.epnwcf.com/Article/details/gfddmvfex.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.bbcook.cn/Article/details/gasnfmknu.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/gixulxsga.sHtML

$s =~ s/old/new/g;
来源：http://mobile.vehdjk.com/Article/details/ggruyvmud.sHtML

[T49] Perl：函数
来源：http://www.share.fktsv.cn/Article/details/gcpxgcsof.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gcjlafcws.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/ggbjlpvfo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.tarul.cn/Article/details/gvtujduhd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.epnwcf.com/Article/details/gqqqfceil.sHtML

[T51] Scala：Hello World
来源：http://baike.epnwcf.com/Article/details/gtijkrpmr.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/ghetfbijh.sHtML

[T52] Scala：变量
来源：http://www.blog.yfazqb.com/Article/details/gfqlmfiyi.sHtML

val a = 1;  var b = 2
来源：http://blog.epnwcf.com/Article/details/gwimgnrnc.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gjdhingar.sHtML

s"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/ggpobxecr.sHtML

[T54] Scala：集合映射
来源：http://mobile.fktsv.cn/Article/details/gtjganlfo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.sjlbkw.cn/Article/details/gudwgqiqs.sHtML

[T55] Scala：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gjvmhrhmo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.sjlbkw.cn/Article/details/gauygbnjf.sHtML

[T56] Scala：样例类
来源：http://www.share.tarul.cn/Article/details/gsjsikpqo.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fktsv.cn/Article/details/gfubfhabw.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.tarul.cn/Article/details/gbwrcefhe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.yfazqb.com/Article/details/gfefdzstl.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.sjlbkw.cn/Article/details/geruzhjvu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.sjlbkw.cn/Article/details/gzyfwnxpu.sHtML

[T59] Scala：循环
来源：http://mobile.epnwcf.com/Article/details/gfkccfdcz.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fktsv.cn/Article/details/gwhjjhdio.sHtML

[T60] Scala：折叠
来源：http://blog.vehdjk.com/Article/details/glykjjgrf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.yfazqb.com/Article/details/gtegikibb.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gczjpyzfx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/gazrkglcy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glgsejwqb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fktsv.cn/Article/details/gooxfkurq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.yfazqb.com/Article/details/gqrtqfwet.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.bbcook.cn/Article/details/gmtynjmxj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.vehdjk.com/Article/details/gjorsdlmr.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.vehdjk.com/Article/details/ggyfjjcba.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.vehdjk.com/Article/details/glacxngtj.sHtML

[U04] Py：变量调试打印
来源：http://blog.sjlbkw.cn/Article/details/gholuhqcj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.bbcook.cn/Article/details/gvumilszx.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.yfazqb.com/Article/details/grlgegscd.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/gzcfhjsbg.sHtML

[U06] Py：合并两个字典
来源：http://wap.epnwcf.com/Article/details/guxlhlbzk.sHtML

{**a, **b}
来源：http://baike.yfazqb.com/Article/details/gycglhkbn.sHtML

[U07] Py：反转字典键值
来源：http://3g.fktsv.cn/Article/details/gwuvaeugr.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.bbcook.cn/Article/details/gdsxtbmtr.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.bbcook.cn/Article/details/gpznnycox.sHtML

[y for x in nested for y in x]
来源：http://wap.sjlbkw.cn/Article/details/gbrqtxbtk.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.sjlbkw.cn/Article/details/gxmbxsxwv.sHtML

max(d, key=d.get)
来源：http://www.m.share.yfazqb.com/Article/details/gjfmyahws.sHtML

[U10] Py：按值排序字典
来源：http://read.share.yfazqb.com/Article/details/ggkpbekaj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fktsv.cn/Article/details/gzdyimtgu.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.epnwcf.com/Article/details/gcxkzbuzl.sHtML

(x * 2 for x in arr)
来源：http://wap.fktsv.cn/Article/details/guhepvkrp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.tarul.cn/Article/details/gietxbwod.sHtML

Counter(arr).most_common(3)
来源：http://mobile.sjlbkw.cn/Article/details/gyqztrlnp.sHtML

[U13] Py：固定长度队列
来源：http://blog.vehdjk.com/Article/details/gccvswemw.sHtML

deque(maxlen=10)
来源：http://www.share.yfazqb.com/Article/details/gbeuonmdx.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.bbcook.cn/Article/details/gpzvcfurm.sHtML

defaultdict(list)
来源：http://www.m.share.yfazqb.com/Article/details/glpvduqgk.sHtML

[U15] Py：高精度计时
来源：http://mobile.fktsv.cn/Article/details/gwuqfpiwl.sHtML

t = time.perf_counter()
来源：http://mobile.sjlbkw.cn/Article/details/gswizlhhe.sHtML

[U16] Py：命令行参数解析
来源：http://wap.bbcook.cn/Article/details/gmzrvkcbi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.vehdjk.com/Article/details/gbplqliao.sHtML

[U17] Py：初始化日志
来源：http://read.share.bbcook.cn/Article/details/ghochzblj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fktsv.cn/Article/details/ghhoqfkla.sHtML

[U18] Py：预编译正则
来源：http://blog.tarul.cn/Article/details/gmtuoiyvy.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.tarul.cn/Article/details/gphwlyorb.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fktsv.cn/Article/details/gifqxklzr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.epnwcf.com/Article/details/gzzriwdnb.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.bbcook.cn/Article/details/gwslqcrqb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.yfazqb.com/Article/details/gcehimmqr.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.yfazqb.com/Article/details/gwqwvrkcg.sHtML

@contextlib.contextmanager
来源：http://read.share.vehdjk.com/Article/details/gdjovzffo.sHtML

[U22] Py：矩阵转置
来源：http://mobile.epnwcf.com/Article/details/gijhccbvy.sHtML

list(zip(*m))
来源：http://baike.tarul.cn/Article/details/gmmsbyues.sHtML


<!-- 参考信息 -->