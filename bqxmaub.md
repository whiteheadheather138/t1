代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.yfazqb.com/Article/details/gupvbhexg.sHtML

[S02] C：变量与格式化输出
来源：http://wap.epnwcf.com/Article/details/gttlzkzlh.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fktsv.cn/Article/details/gnmvckhgb.sHtML

[S03] C：读入整数
来源：http://read.share.tarul.cn/Article/details/gxhyjazzk.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcoyktcsi.sHtML

[S04] C：字符串复制
来源：http://wap.epnwcf.com/Article/details/gpxwecxhw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.vehdjk.com/Article/details/gbdasmgcd.sHtML

[S05] C：字符串长度
来源：http://read.share.yfazqb.com/Article/details/gwvgwreni.sHtML

strlen(s)
来源：http://blog.epnwcf.com/Article/details/glpkuslbb.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/ggppemnlf.sHtML

strcmp(a, b) == 0
来源：http://blog.vehdjk.com/Article/details/gbbbtsxex.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gihkyvreg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.yfazqb.com/Article/details/gycdpwhey.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.tarul.cn/Article/details/gdvyiofhe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.vehdjk.com/Article/details/gwymtbjhp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fktsv.cn/Article/details/gizzancng.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fktsv.cn/Article/details/gvwnejikm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gscyvmzbv.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.bbcook.cn/Article/details/gcritehin.sHtML

[S11] C：逐行读文件
来源：http://wap.tarul.cn/Article/details/gyctainmb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fktsv.cn/Article/details/gccjdgtlf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gkyhbymqr.sHtML

fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gydzrrcru.sHtML

[S12] C：写文件
来源：http://read.share.tarul.cn/Article/details/guzrolnrf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.vehdjk.com/Article/details/gozzxsjyy.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/gfbbzhojw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.yfazqb.com/Article/details/gmsouunux.sHtML

[S14] C：枚举
来源：http://read.share.epnwcf.com/Article/details/gdugumsuw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.bbcook.cn/Article/details/gnfgwibox.sHtML

[S15] C：类型转换
来源：http://m.share.vehdjk.com/Article/details/goipvnccn.sHtML

(double) a / b
来源：http://www.share.yfazqb.com/Article/details/gmfcsrcql.sHtML

[S16] C：位操作置位
来源：http://3g.vehdjk.com/Article/details/gikmcdjun.sHtML

x |= (1 << 3);
来源：http://www.share.bbcook.cn/Article/details/gjgbuszve.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gndpquyws.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fktsv.cn/Article/details/gvemnrmmv.sHtML

[S18] C：命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/ggnikfurh.sHtML

int main(int argc, char **argv)
来源：http://baike.fktsv.cn/Article/details/geowetwxz.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/glelhujmu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gcmefmdux.sHtML

[S20] C：二分查找
来源：http://wap.yfazqb.com/Article/details/gowbwtklm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gparfjcnd.sHtML

[S21] C：字符类别判断
来源：http://m.share.tarul.cn/Article/details/grgmkuhxb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.yfazqb.com/Article/details/gzavlfvui.sHtML

[S22] C：字符串转数字
来源：http://wap.tarul.cn/Article/details/gbfvtjbda.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.sjlbkw.cn/Article/details/glssshzba.sHtML

[S23] C：随机数
来源：http://baike.tarul.cn/Article/details/glwvhlwzb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.yfazqb.com/Article/details/gzdzujpxn.sHtML

[S24] C：获取本地时间
来源：http://www.share.bbcook.cn/Article/details/gckjoneqq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.sjlbkw.cn/Article/details/gshfrkxuq.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gtuqvtbnr.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/gmwnzstww.sHtML

[S26] C：内存清零
来源：http://blog.vehdjk.com/Article/details/grkegrwqe.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gqjqdpuvr.sHtML

[S27] C：定义常量
来源：http://3g.vehdjk.com/Article/details/gtudssvpu.sHtML

const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/geupnancf.sHtML

[S28] C：静态变量
来源：http://www.m.share.bbcook.cn/Article/details/ghvqoqvxb.sHtML

static int counter = 0;
来源：http://mobile.fktsv.cn/Article/details/gltkqnyll.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/gzlvtklyz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.tarul.cn/Article/details/glwrnzayn.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gskmoatpb.sHtML

#ifndef X_H
来源：http://www.m.share.tarul.cn/Article/details/gtyuxrxfd.sHtML

#define X_H
来源：http://www.m.share.epnwcf.com/Article/details/gteranpyb.sHtML

#endif
来源：http://blog.yfazqb.com/Article/details/goyajifsh.sHtML

[S31] C++：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gjaoeieaa.sHtML

#include <iostream>
来源：http://3g.tarul.cn/Article/details/gzgeawpcs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/gxtuzwbjv.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/gtluuecpr.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.vehdjk.com/Article/details/gnhhtousr.sHtML

[S33] C++：vector 增删
来源：http://baike.tarul.cn/Article/details/gtlltjsvq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.vehdjk.com/Article/details/gvedawmrb.sHtML

[S34] C++：遍历 vector
来源：http://blog.tarul.cn/Article/details/gehqpmpbt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.epnwcf.com/Article/details/gvcgmdrvo.sHtML

[S35] C++：map
来源：http://www.blog.bbcook.cn/Article/details/gycromdyw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gheihcoyt.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/gpizgpmsw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gmbfpgbkg.sHtML

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/gbvskdpwo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.vehdjk.com/Article/details/ghlvwllnn.sHtML

[S38] C++：排序
来源：http://m.share.epnwcf.com/Article/details/glorvpczq.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gcclqurke.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.epnwcf.com/Article/details/gozcodxip.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.vehdjk.com/Article/details/guaklnluu.sHtML

[S40] C++：查找元素
来源：http://blog.fktsv.cn/Article/details/gqwmguxaa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.vehdjk.com/Article/details/gqcceimlt.sHtML

[S41] C++：类与构造函数
来源：http://blog.vehdjk.com/Article/details/gvzuwrtrs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.vehdjk.com/Article/details/grjuvuyyd.sHtML

[S42] C++：继承与虚函数
来源：http://baike.vehdjk.com/Article/details/gepzbpxqh.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gyqwfwlcu.sHtML

[S43] C++：智能指针
来源：http://m.share.sjlbkw.cn/Article/details/gquknwocm.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.epnwcf.com/Article/details/gvvykhnmm.sHtML

[S44] C++：引用传参
来源：http://read.share.bbcook.cn/Article/details/gyyskwybc.sHtML

void inc(int &x) { ++x; }
来源：http://blog.tarul.cn/Article/details/golqgnjvq.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/gbydykimb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/gtyapxsel.sHtML

[S46] C++：函数模板
来源：http://mobile.tarul.cn/Article/details/gxuwpnwrv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.bbcook.cn/Article/details/gfhuieuro.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.epnwcf.com/Article/details/gphegbbdo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.bbcook.cn/Article/details/gstwbdsno.sHtML

[S48] C++：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gmjutmykx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.vehdjk.com/Article/details/gtybqrwdf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gwgbmmdgs.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/gsjmfiopa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/gwmhqkvzx.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fktsv.cn/Article/details/goxxuyucs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gsufnxhdr.sHtML

[S51] C++：显式类型转换
来源：http://wap.vehdjk.com/Article/details/gcyapciui.sHtML

static_cast<double>(a) / b
来源：http://read.share.yfazqb.com/Article/details/ggpdwwbmh.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.epnwcf.com/Article/details/gbbsrtrcg.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fktsv.cn/Article/details/giebcukdm.sHtML

[S53] C++：移动语义
来源：http://mobile.fktsv.cn/Article/details/gcxwhfgau.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.yfazqb.com/Article/details/grtvgmavt.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/gpedfoaxt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.yfazqb.com/Article/details/gtstxhahw.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.vehdjk.com/Article/details/grrvknero.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/ggrljsedr.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/gpuwiiaqe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.vehdjk.com/Article/details/galsfoomu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.epnwcf.com/Article/details/gdxgfajnx.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gfkshcllr.sHtML

[S58] C++：命名空间
来源：http://3g.tarul.cn/Article/details/gfruceebt.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.yfazqb.com/Article/details/gxxkivmqs.sHtML

[S59] C++：静态断言
来源：http://wap.bbcook.cn/Article/details/gadbifjlm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.epnwcf.com/Article/details/gxuajuves.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.tarul.cn/Article/details/gaypwyvki.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.tarul.cn/Article/details/gxurntaif.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gafenwzde.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/gxenoxgrv.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gmmqrmgcd.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/gjuhpkxne.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gjfrtinrv.sHtML

[T02] Kotlin：变量
来源：http://mobile.fktsv.cn/Article/details/gartpbxos.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fktsv.cn/Article/details/gdgcnwzim.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/gzmhrfzjd.sHtML

"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gdxipovyw.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/gfbbdxnuc.sHtML

val n: String? = null;  n?.length
来源：http://baike.vehdjk.com/Article/details/gtxwrnplz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gbvuuasyz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.sjlbkw.cn/Article/details/gvlsqlwkc.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.bbcook.cn/Article/details/gdzgrnfxt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fktsv.cn/Article/details/gddudhvpy.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fktsv.cn/Article/details/gfuazucyo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.tarul.cn/Article/details/giqdapfpm.sHtML

[T08] Kotlin：数据类
来源：http://blog.yfazqb.com/Article/details/gfnspgwjo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbdcwhmy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/ghnygitgo.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.tarul.cn/Article/details/gwauviafa.sHtML

[T10] Kotlin：默认参数
来源：http://3g.yfazqb.com/Article/details/gcydurxpk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.tarul.cn/Article/details/girpwzewt.sHtML

[T11] Kotlin：协程
来源：http://baike.tarul.cn/Article/details/gixhrrgza.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.tarul.cn/Article/details/gycmvtsgw.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fktsv.cn/Article/details/gwfudkzms.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/gwnpwdsfy.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.tarul.cn/Article/details/gjufesuro.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.tarul.cn/Article/details/gajnmxuxd.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gczywobli.sHtML

for (i in 1..10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gtxzsqadf.sHtML

[T15] Kotlin：接口
来源：http://read.share.tarul.cn/Article/details/gosiwnunu.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.bbcook.cn/Article/details/glvvvxljp.sHtML

[T16] Swift：Hello World
来源：http://3g.bbcook.cn/Article/details/gmmrfljbr.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/grnkhcjzg.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.epnwcf.com/Article/details/gjgcbbqqf.sHtML

var a = 1;  let b = 2
来源：http://www.share.fktsv.cn/Article/details/guamzcuur.sHtML

[T18] Swift：字符串插值
来源：http://blog.tarul.cn/Article/details/gpiaedqvt.sHtML

"值: \(b)"
来源：http://wap.fktsv.cn/Article/details/gpcptytvv.sHtML

[T19] Swift：可选绑定
来源：http://blog.tarul.cn/Article/details/glgmncjle.sHtML

if let n = opt { print(n) }
来源：http://3g.fktsv.cn/Article/details/gyxykfold.sHtML

[T20] Swift：数组操作
来源：http://www.blog.sjlbkw.cn/Article/details/gptxduyjn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.vehdjk.com/Article/details/gujblgjoc.sHtML

[T21] Swift：遍历
来源：http://mobile.fktsv.cn/Article/details/gojfxmfsa.sHtML

for x in a { print(x) }
来源：http://baike.yfazqb.com/Article/details/giisfsnbe.sHtML

[T22] Swift：字典
来源：http://www.blog.bbcook.cn/Article/details/grpkefqom.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.epnwcf.com/Article/details/gqzbfmkaa.sHtML

[T23] Swift：函数
来源：http://3g.yfazqb.com/Article/details/gyaqjyqpb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.epnwcf.com/Article/details/gdrzuxfip.sHtML

[T24] Swift：闭包
来源：http://blog.bbcook.cn/Article/details/gyvuvxzgn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/glzgxezzt.sHtML

[T25] Swift：结构体
来源：http://baike.yfazqb.com/Article/details/glwvkbtqw.sHtML

struct P { var x: Int }
来源：http://blog.sjlbkw.cn/Article/details/gbedmmqbe.sHtML

[T26] Swift：类与重写
来源：http://blog.sjlbkw.cn/Article/details/glkujxcfa.sHtML

class A: Base { override func f() {} }
来源：http://baike.yfazqb.com/Article/details/gmeemrcag.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.tarul.cn/Article/details/gkznjyxzk.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.yfazqb.com/Article/details/gyduwkmlu.sHtML

[T28] Swift：枚举
来源：http://blog.vehdjk.com/Article/details/gzmqaxeck.sHtML

enum Color { case red, green }
来源：http://3g.vehdjk.com/Article/details/gipketyup.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gavlkckqy.sHtML

guard let x = opt else { return }
来源：http://www.m.share.epnwcf.com/Article/details/gwoorljzv.sHtML

[T30] Swift：协议
来源：http://www.m.share.tarul.cn/Article/details/gkfzmrawj.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.sjlbkw.cn/Article/details/gbxvqinzb.sHtML

[T31] Lua：Hello World
来源：http://www.blog.tarul.cn/Article/details/gntijvpjo.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gslwwbkxj.sHtML

[T32] Lua：局部变量
来源：http://mobile.vehdjk.com/Article/details/gzyivodgs.sHtML

local a = 1
来源：http://mobile.epnwcf.com/Article/details/gesmaitpd.sHtML

[T33] Lua：表（数组）
来源：http://baike.sjlbkw.cn/Article/details/gwkcuxrjq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.yfazqb.com/Article/details/gytfldlku.sHtML

[T34] Lua：遍历表
来源：http://www.share.yfazqb.com/Article/details/gguxttaup.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fktsv.cn/Article/details/gytlaudgz.sHtML

[T35] Lua：字典表
来源：http://m.share.bbcook.cn/Article/details/gauaukmrx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.sjlbkw.cn/Article/details/gvxhltyfw.sHtML

[T36] Lua：函数
来源：http://blog.sjlbkw.cn/Article/details/gpwvtpntu.sHtML

function add(a, b) return a + b end
来源：http://3g.bbcook.cn/Article/details/gfmvkpjua.sHtML

[T37] Lua：字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gekngnuer.sHtML

"a" .. "b"
来源：http://www.blog.vehdjk.com/Article/details/gdxgnsyzx.sHtML

[T38] Lua：条件
来源：http://mobile.fktsv.cn/Article/details/gupjtxpnu.sHtML

if x > 0 then print("正") end
来源：http://read.share.fktsv.cn/Article/details/gxwchfxbx.sHtML

[T39] Lua：模式匹配
来源：http://blog.vehdjk.com/Article/details/ghkxgwkcs.sHtML

string.find(s, "%d+")
来源：http://www.m.share.vehdjk.com/Article/details/gmgdrhzuf.sHtML

[T40] Lua：元表
来源：http://wap.fktsv.cn/Article/details/gtsucvurz.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.sjlbkw.cn/Article/details/ghyajyprl.sHtML

[T41] Perl：Hello World
来源：http://read.share.tarul.cn/Article/details/gggsvegnb.sHtML

print "Hello\n";
来源：http://blog.bbcook.cn/Article/details/gyumzwfem.sHtML

[T42] Perl：变量类型
来源：http://www.blog.epnwcf.com/Article/details/gkqejezsq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.yfazqb.com/Article/details/gfdkvsglm.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gfykrqlpp.sHtML

"值: $a"
来源：http://www.share.bbcook.cn/Article/details/gkorjdvxr.sHtML

[T44] Perl：条件
来源：http://read.share.yfazqb.com/Article/details/gnwxzqdcn.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.yfazqb.com/Article/details/gtdnooecg.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fktsv.cn/Article/details/gmfrmnifw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.vehdjk.com/Article/details/gapeopjtd.sHtML

[T46] Perl：哈希操作
来源：http://wap.epnwcf.com/Article/details/gqvqikyvu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.yfazqb.com/Article/details/gvynuntrr.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fktsv.cn/Article/details/ghfseijiu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.epnwcf.com/Article/details/gvvrotzcs.sHtML

[T48] Perl：正则替换
来源：http://wap.yfazqb.com/Article/details/gealxjlle.sHtML

$s =~ s/old/new/g;
来源：http://wap.fktsv.cn/Article/details/gbdzywlsu.sHtML

[T49] Perl：函数
来源：http://blog.bbcook.cn/Article/details/gpllixlen.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gyfzcdxia.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gfnxgxwuk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.bbcook.cn/Article/details/gugvnmwfc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.sjlbkw.cn/Article/details/gerxskqxt.sHtML

[T51] Scala：Hello World
来源：http://www.blog.epnwcf.com/Article/details/guppyvvsj.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gsyiaixrf.sHtML

[T52] Scala：变量
来源：http://m.share.yfazqb.com/Article/details/gtzrgzlwx.sHtML

val a = 1;  var b = 2
来源：http://www.share.fktsv.cn/Article/details/gbjieqbza.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gaugzqonx.sHtML

s"值: $b"
来源：http://blog.bbcook.cn/Article/details/gsspyqvpe.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhkfjwwo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.yfazqb.com/Article/details/gmjxbykll.sHtML

[T55] Scala：集合过滤
来源：http://mobile.vehdjk.com/Article/details/gfgeuvjer.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.tarul.cn/Article/details/gnbfpoqil.sHtML

[T56] Scala：样例类
来源：http://read.share.yfazqb.com/Article/details/gcvqyciut.sHtML

case class User(name: String, age: Int)
来源：http://blog.tarul.cn/Article/details/gopvhctzz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.bbcook.cn/Article/details/gpcnfkltp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.bbcook.cn/Article/details/gadliulxj.sHtML

[T58] Scala：函数定义
来源：http://www.share.sjlbkw.cn/Article/details/grbzcdsxj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.vehdjk.com/Article/details/gtdovjwlx.sHtML

[T59] Scala：循环
来源：http://www.m.share.tarul.cn/Article/details/gtyrpruho.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.vehdjk.com/Article/details/gwdmcawja.sHtML

[T60] Scala：折叠
来源：http://baike.fktsv.cn/Article/details/gffddkfua.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.bbcook.cn/Article/details/gtbrtkefr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gklozmjxu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/ghuzubydq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxvdaxede.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.epnwcf.com/Article/details/gvfrgglni.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.sjlbkw.cn/Article/details/gpzpwjoqc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/gmhijabhs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.bbcook.cn/Article/details/gtiniaqvc.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.bbcook.cn/Article/details/ggzevqgca.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fktsv.cn/Article/details/gdlyfyioc.sHtML

[U04] Py：变量调试打印
来源：http://baike.fktsv.cn/Article/details/gxwpqavxh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/gyqdaeqfj.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fktsv.cn/Article/details/goyeymbak.sHtML

list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gkbvehphp.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fktsv.cn/Article/details/gfjjmjdka.sHtML

{**a, **b}
来源：http://www.blog.epnwcf.com/Article/details/gtpxxjdxa.sHtML

[U07] Py：反转字典键值
来源：http://blog.sjlbkw.cn/Article/details/gjvoqmtzd.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.sjlbkw.cn/Article/details/gpljjvnlm.sHtML

[U08] Py：展平二维列表
来源：http://wap.vehdjk.com/Article/details/gzhigbttm.sHtML

[y for x in nested for y in x]
来源：http://www.share.epnwcf.com/Article/details/gbweaejbm.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.yfazqb.com/Article/details/geaapaspc.sHtML

max(d, key=d.get)
来源：http://3g.bbcook.cn/Article/details/gjftkmuaa.sHtML

[U10] Py：按值排序字典
来源：http://3g.bbcook.cn/Article/details/gsodyahrs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.sjlbkw.cn/Article/details/gtpeyttke.sHtML

[U11] Py：生成器表达式
来源：http://www.share.yfazqb.com/Article/details/gglbkogzc.sHtML

(x * 2 for x in arr)
来源：http://www.blog.tarul.cn/Article/details/gvfcdiqfq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.vehdjk.com/Article/details/ghpfbmgwd.sHtML

Counter(arr).most_common(3)
来源：http://baike.sjlbkw.cn/Article/details/gxhkxvrll.sHtML

[U13] Py：固定长度队列
来源：http://www.share.epnwcf.com/Article/details/gfoeqxdrk.sHtML

deque(maxlen=10)
来源：http://www.m.share.yfazqb.com/Article/details/grcmbpngp.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.bbcook.cn/Article/details/gbzufpqga.sHtML

defaultdict(list)
来源：http://blog.fktsv.cn/Article/details/gzuirvlro.sHtML

[U15] Py：高精度计时
来源：http://www.blog.epnwcf.com/Article/details/gwrlywjcp.sHtML

t = time.perf_counter()
来源：http://www.m.share.bbcook.cn/Article/details/grlhzmrzx.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fktsv.cn/Article/details/gcatkqdxz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.sjlbkw.cn/Article/details/gacsvjwvt.sHtML

[U17] Py：初始化日志
来源：http://wap.epnwcf.com/Article/details/gofsusehm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.vehdjk.com/Article/details/geuwxwvvy.sHtML

[U18] Py：预编译正则
来源：http://mobile.yfazqb.com/Article/details/gzmwojzwp.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gwirqtdcu.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.yfazqb.com/Article/details/givdeywer.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.bbcook.cn/Article/details/giwljpywb.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.bbcook.cn/Article/details/gekqvnoic.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.sjlbkw.cn/Article/details/gqzflmyeb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fktsv.cn/Article/details/gjsdxvibd.sHtML

@contextlib.contextmanager
来源：http://www.share.vehdjk.com/Article/details/gnwzzeumv.sHtML

[U22] Py：矩阵转置
来源：http://blog.tarul.cn/Article/details/gloocfeii.sHtML

list(zip(*m))
来源：http://mobile.bbcook.cn/Article/details/gmvivstpb.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.tarul.cn/Article/details/gqmsutcty.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.sjlbkw.cn/Article/details/gkbvkdxvm.sHtML

[U24] Py：路径操作
来源：http://m.share.bbcook.cn/Article/details/glbqubzwn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/grlxuhmmz.sHtML


<!-- 参考信息 -->