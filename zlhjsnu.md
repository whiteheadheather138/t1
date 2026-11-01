代发 wailian999

read -rp "请输入: " ans
来源：http://m.share.bbcook.cn/Article/details/gslzxbxsb.sHtML

[R78] 交互式菜单
来源：http://m.share.tarul.cn/Article/details/gknshjlfr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.tarul.cn/Article/details/gwhtrdixk.sHtML

[R79] 解析命令行选项
来源：http://read.share.bbcook.cn/Article/details/ghdtpwbuh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.sjlbkw.cn/Article/details/gbzbqdhxk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.sjlbkw.cn/Article/details/gzcmrjcnc.sHtML

time ./run.sh
来源：http://www.blog.vehdjk.com/Article/details/gfropuorr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmbumhzdi.sHtML

S. C / C++ 专题
来源：http://read.share.fktsv.cn/Article/details/gyknbxtuy.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gmglfiffq.sHtML

[S01] C：Hello World
来源：http://3g.vehdjk.com/Article/details/gtiekcons.sHtML

#include <stdio.h>
来源：http://3g.yfazqb.com/Article/details/ggcvnqmbq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.bbcook.cn/Article/details/gwlqihdue.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/gfzoorbno.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gekxrefzv.sHtML

[S03] C：读入整数
来源：http://mobile.yfazqb.com/Article/details/gxgyncjyc.sHtML

int x; scanf("%d", &x);
来源：http://www.share.sjlbkw.cn/Article/details/geyaekezy.sHtML

[S04] C：字符串复制
来源：http://m.share.vehdjk.com/Article/details/gxsewdvwg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gehejozfq.sHtML

[S05] C：字符串长度
来源：http://read.share.fktsv.cn/Article/details/gjhetoyyz.sHtML

strlen(s)
来源：http://www.m.share.epnwcf.com/Article/details/gixgokxuo.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gnzmwkcce.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gahndgbco.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/gkyxovdle.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.sjlbkw.cn/Article/details/gxppdjuin.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/gljgtvawi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fktsv.cn/Article/details/gjghzzmzm.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.bbcook.cn/Article/details/ghawwibiq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.bbcook.cn/Article/details/gwnjumpid.sHtML

[S10] C：指针与解引用
来源：http://3g.epnwcf.com/Article/details/gitlxvpxy.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.tarul.cn/Article/details/gghqxkvjt.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gdhvjlnjp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.sjlbkw.cn/Article/details/gzddtppzb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.epnwcf.com/Article/details/geyiuzagg.sHtML

fclose(f);
来源：http://wap.epnwcf.com/Article/details/gqtnckzir.sHtML

[S12] C：写文件
来源：http://blog.tarul.cn/Article/details/gslzxered.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gvqscnncj.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/ghebnnuso.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.yfazqb.com/Article/details/gejhenywq.sHtML

[S14] C：枚举
来源：http://m.share.fktsv.cn/Article/details/ggsmzykfr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fktsv.cn/Article/details/gafqzkrrp.sHtML

[S15] C：类型转换
来源：http://blog.fktsv.cn/Article/details/gzjkyfqgk.sHtML

(double) a / b
来源：http://www.blog.sjlbkw.cn/Article/details/gippkgtkr.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/giduvomnp.sHtML

x |= (1 << 3);
来源：http://baike.tarul.cn/Article/details/gqbozaixu.sHtML

[S17] C：安全拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gratwwnby.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.sjlbkw.cn/Article/details/gnqltxlcm.sHtML

[S18] C：命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gholkxtoj.sHtML

int main(int argc, char **argv)
来源：http://3g.bbcook.cn/Article/details/gxuabglvy.sHtML

[S19] C：快速排序
来源：http://m.share.sjlbkw.cn/Article/details/gbodskbjw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gaukgpgtr.sHtML

[S20] C：二分查找
来源：http://read.share.sjlbkw.cn/Article/details/gknjlxwvi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxogjbjq.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/gyxlqhbcy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/govkefwjv.sHtML

[S22] C：字符串转数字
来源：http://blog.tarul.cn/Article/details/glwixzgfk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.sjlbkw.cn/Article/details/gibyxuxed.sHtML

[S23] C：随机数
来源：http://www.m.share.tarul.cn/Article/details/gjpomhnxh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.tarul.cn/Article/details/gcvwsxnbv.sHtML

[S24] C：获取本地时间
来源：http://blog.vehdjk.com/Article/details/gwjbptffq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fktsv.cn/Article/details/ghlpevjab.sHtML

[S25] C：内存拷贝
来源：http://3g.bbcook.cn/Article/details/gltpdddfs.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gjlxdyqwu.sHtML

[S26] C：内存清零
来源：http://3g.vehdjk.com/Article/details/gcdxzwsro.sHtML

memset(a, 0, sizeof a);
来源：http://wap.vehdjk.com/Article/details/ghvdhlowb.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/gonlolrjm.sHtML

const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gfbuheyxc.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/grugvlyus.sHtML

static int counter = 0;
来源：http://www.blog.epnwcf.com/Article/details/gfcxhqvzl.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/ghsujlsbb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.bbcook.cn/Article/details/gkdupysvm.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gfpgwzrwl.sHtML

#ifndef X_H
来源：http://mobile.yfazqb.com/Article/details/gobrhrbbk.sHtML

#define X_H
来源：http://www.share.sjlbkw.cn/Article/details/grksdgiul.sHtML

#endif
来源：http://m.share.yfazqb.com/Article/details/gjhusofkj.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/gnsmfdjml.sHtML

#include <iostream>
来源：http://www.m.share.fktsv.cn/Article/details/gvhbwetzf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.epnwcf.com/Article/details/gwswsfufr.sHtML

[S32] C++：字符串
来源：http://www.blog.bbcook.cn/Article/details/gbtgtqgrr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.epnwcf.com/Article/details/gvfwqognu.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/gscftivvx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fktsv.cn/Article/details/gdzsyowya.sHtML

[S34] C++：遍历 vector
来源：http://3g.bbcook.cn/Article/details/gnxhycaud.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gmekgxbod.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gnjtrybtb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gbnyuxgcb.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/ggzqfgssw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/gaibticpd.sHtML

[S37] C++：set
来源：http://baike.epnwcf.com/Article/details/gmbsxshud.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/grzfwtryp.sHtML

[S38] C++：排序
来源：http://read.share.vehdjk.com/Article/details/gtbnrhcmo.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gyjgwmzzo.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/gdtmkamri.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.sjlbkw.cn/Article/details/geqoqpblt.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gvphaujec.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.sjlbkw.cn/Article/details/grnoexuha.sHtML

[S41] C++：类与构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gmgmzciqa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.tarul.cn/Article/details/gsnzbrrjm.sHtML

[S42] C++：继承与虚函数
来源：http://3g.bbcook.cn/Article/details/gxzijxuyh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/gwikwbodc.sHtML

[S43] C++：智能指针
来源：http://m.share.epnwcf.com/Article/details/gixzfgray.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/gxxgvasrj.sHtML

[S44] C++：引用传参
来源：http://wap.fktsv.cn/Article/details/gfokoaqlc.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.vehdjk.com/Article/details/glddlnmfu.sHtML

[S45] C++：lambda
来源：http://mobile.epnwcf.com/Article/details/gmcgfhwwf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/gkezerbgr.sHtML

[S46] C++：函数模板
来源：http://read.share.tarul.cn/Article/details/gvzxcmagw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.vehdjk.com/Article/details/gfavpfrwj.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.epnwcf.com/Article/details/gjrjtpavo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.tarul.cn/Article/details/gttsijwjm.sHtML

[S48] C++：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/giuhnrwdv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/gianbutpw.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.yfazqb.com/Article/details/gfmtwetgt.sHtML

[S49] C++：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gntxnrxhq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.yfazqb.com/Article/details/gzwltupkp.sHtML

[S50] C++：格式化数字
来源：http://www.share.fktsv.cn/Article/details/gxdinauek.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.yfazqb.com/Article/details/geyhmfvok.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gvffscksj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.bbcook.cn/Article/details/glrjlyqbk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fktsv.cn/Article/details/giadegjbz.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.bbcook.cn/Article/details/gayvbebof.sHtML

[S53] C++：移动语义
来源：http://m.share.fktsv.cn/Article/details/gjfpbgkoc.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.vehdjk.com/Article/details/gjdbzyejn.sHtML

[S54] C++：异常处理
来源：http://baike.tarul.cn/Article/details/gggwkwoiq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.yfazqb.com/Article/details/ggrfeacbf.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fktsv.cn/Article/details/gwissutfc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.bbcook.cn/Article/details/gmawmxlng.sHtML

[S56] C++：optional
来源：http://www.m.share.epnwcf.com/Article/details/gnsbqieqe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.sjlbkw.cn/Article/details/gnsnxswmi.sHtML

[S57] C++：编译期常量
来源：http://www.share.yfazqb.com/Article/details/gzxdzixzh.sHtML

constexpr int N = 10;
来源：http://www.blog.tarul.cn/Article/details/gaulzvlgl.sHtML

[S58] C++：命名空间
来源：http://www.blog.yfazqb.com/Article/details/gdyqorsom.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.bbcook.cn/Article/details/gdbiewmaz.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/gzclefxzo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.tarul.cn/Article/details/gioffieom.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.epnwcf.com/Article/details/gxjzunpmz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.yfazqb.com/Article/details/gtpejkpeb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnlquhqar.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/gwkfqhegc.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghjrfwirf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fktsv.cn/Article/details/gaxbhbrid.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gxftwtdrp.sHtML

[T02] Kotlin：变量
来源：http://m.share.vehdjk.com/Article/details/gbvpjkjmi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.sjlbkw.cn/Article/details/gqmwvcbxb.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.bbcook.cn/Article/details/gpsmtjgee.sHtML

"值: $b"
来源：http://3g.tarul.cn/Article/details/gevsdtxsq.sHtML

[T04] Kotlin：空安全
来源：http://3g.epnwcf.com/Article/details/gxxjkvwks.sHtML

val n: String? = null;  n?.length
来源：http://mobile.yfazqb.com/Article/details/gsfvgkgbi.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.vehdjk.com/Article/details/gqpoaekcs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.yfazqb.com/Article/details/gpowzynlr.sHtML

[T06] Kotlin：集合映射
来源：http://wap.bbcook.cn/Article/details/gdoiridbz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gzaeqnfey.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.vehdjk.com/Article/details/gpxzjopdx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/giikjmiia.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fktsv.cn/Article/details/gislfamgs.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.tarul.cn/Article/details/gbunbidbw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/gmasmghxe.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.vehdjk.com/Article/details/gdlgujhva.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.sjlbkw.cn/Article/details/goqrzfnod.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.epnwcf.com/Article/details/gifiawjdi.sHtML

[T11] Kotlin：协程
来源：http://baike.sjlbkw.cn/Article/details/ggjtstqpc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fktsv.cn/Article/details/gysankcbv.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.vehdjk.com/Article/details/gcffrvldx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gbhggpbtn.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.vehdjk.com/Article/details/goxdcnemz.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/gxzfyyqsq.sHtML

[T14] Kotlin：循环
来源：http://www.share.bbcook.cn/Article/details/ggdjawkve.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/gztxdhcxm.sHtML

[T15] Kotlin：接口
来源：http://m.share.tarul.cn/Article/details/gyhsgmjio.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.bbcook.cn/Article/details/gnfmsadop.sHtML

[T16] Swift：Hello World
来源：http://baike.yfazqb.com/Article/details/gghimywom.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/ggxguarli.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.epnwcf.com/Article/details/gfkkhzuig.sHtML

var a = 1;  let b = 2
来源：http://baike.vehdjk.com/Article/details/gwkjuwsyo.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gnjjklwhj.sHtML

"值: \(b)"
来源：http://baike.fktsv.cn/Article/details/gykqvtkeq.sHtML

[T19] Swift：可选绑定
来源：http://wap.epnwcf.com/Article/details/galtxojax.sHtML

if let n = opt { print(n) }
来源：http://read.share.vehdjk.com/Article/details/gbapdqiwe.sHtML

[T20] Swift：数组操作
来源：http://www.share.yfazqb.com/Article/details/gsoullnze.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fktsv.cn/Article/details/gcdvhqajf.sHtML

[T21] Swift：遍历
来源：http://read.share.yfazqb.com/Article/details/gjsrefhyd.sHtML

for x in a { print(x) }
来源：http://baike.epnwcf.com/Article/details/godxhfcly.sHtML

[T22] Swift：字典
来源：http://m.share.yfazqb.com/Article/details/gnyxxrbda.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gysjtedei.sHtML

[T23] Swift：函数
来源：http://www.m.share.fktsv.cn/Article/details/gpqimgdjx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.epnwcf.com/Article/details/gbvdglhnq.sHtML

[T24] Swift：闭包
来源：http://www.share.epnwcf.com/Article/details/geoabnxof.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.bbcook.cn/Article/details/gkdfsgcru.sHtML

[T25] Swift：结构体
来源：http://3g.tarul.cn/Article/details/gmicdgomo.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/gpwulafhz.sHtML

[T26] Swift：类与重写
来源：http://www.blog.sjlbkw.cn/Article/details/gdirugwqw.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fktsv.cn/Article/details/ghbsmbfdl.sHtML

[T27] Swift：错误处理
来源：http://mobile.tarul.cn/Article/details/guqsgfviw.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.yfazqb.com/Article/details/glkhkncob.sHtML

[T28] Swift：枚举
来源：http://3g.vehdjk.com/Article/details/gjnkkvgvs.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/gawsbiymg.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.yfazqb.com/Article/details/gxbnpsgtr.sHtML

guard let x = opt else { return }
来源：http://blog.sjlbkw.cn/Article/details/gswzmoadm.sHtML

[T30] Swift：协议
来源：http://blog.epnwcf.com/Article/details/gwwrtcbvp.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.epnwcf.com/Article/details/gmzbvlsfc.sHtML

[T31] Lua：Hello World
来源：http://mobile.vehdjk.com/Article/details/gkgktdsyq.sHtML

print("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gkinamblc.sHtML

[T32] Lua：局部变量
来源：http://mobile.tarul.cn/Article/details/gjhsyjxev.sHtML

local a = 1
来源：http://www.share.bbcook.cn/Article/details/gljmtufoh.sHtML

[T33] Lua：表（数组）
来源：http://blog.yfazqb.com/Article/details/gizktfjzy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.sjlbkw.cn/Article/details/gnpxdymlz.sHtML

[T34] Lua：遍历表
来源：http://3g.tarul.cn/Article/details/gyiycerrp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fktsv.cn/Article/details/glvzgbqev.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fktsv.cn/Article/details/gdimdlxha.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.bbcook.cn/Article/details/gikdcokxf.sHtML

[T36] Lua：函数
来源：http://m.share.fktsv.cn/Article/details/gxgtcgtxk.sHtML

function add(a, b) return a + b end
来源：http://read.share.sjlbkw.cn/Article/details/gqrxudthc.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/gnsaydvme.sHtML

"a" .. "b"
来源：http://m.share.yfazqb.com/Article/details/gqmmnnqnr.sHtML

[T38] Lua：条件
来源：http://www.m.share.bbcook.cn/Article/details/gewbjuhja.sHtML

if x > 0 then print("正") end
来源：http://www.blog.tarul.cn/Article/details/gklcvpyha.sHtML

[T39] Lua：模式匹配
来源：http://3g.sjlbkw.cn/Article/details/gnmlojoou.sHtML

string.find(s, "%d+")
来源：http://baike.bbcook.cn/Article/details/gyfgleapq.sHtML

[T40] Lua：元表
来源：http://3g.sjlbkw.cn/Article/details/gmhkjwmxj.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fktsv.cn/Article/details/gtehorxvu.sHtML

[T41] Perl：Hello World
来源：http://read.share.bbcook.cn/Article/details/gvipweqnw.sHtML

print "Hello\n";
来源：http://baike.tarul.cn/Article/details/gpcikbdek.sHtML

[T42] Perl：变量类型
来源：http://mobile.epnwcf.com/Article/details/gdttysglv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.yfazqb.com/Article/details/gxuwdesbr.sHtML

[T43] Perl：字符串插值
来源：http://www.share.tarul.cn/Article/details/gobfyeptp.sHtML

"值: $a"
来源：http://read.share.vehdjk.com/Article/details/gfhyuorhi.sHtML

[T44] Perl：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gldgfrxgk.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/gcmtsunjc.sHtML

[T45] Perl：数组遍历
来源：http://www.share.yfazqb.com/Article/details/gxjudknyl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.yfazqb.com/Article/details/gneadxakv.sHtML

[T46] Perl：哈希操作
来源：http://mobile.epnwcf.com/Article/details/gcrtvjygi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/gmaehwmee.sHtML

[T47] Perl：正则捕获
来源：http://baike.sjlbkw.cn/Article/details/govldynlx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.bbcook.cn/Article/details/gadgopuwv.sHtML

[T48] Perl：正则替换
来源：http://read.share.bbcook.cn/Article/details/golorrvnb.sHtML

$s =~ s/old/new/g;
来源：http://m.share.epnwcf.com/Article/details/grpghoblq.sHtML

[T49] Perl：函数
来源：http://m.share.yfazqb.com/Article/details/gociuldoe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gdvgglfam.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gqjkxfnwh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.yfazqb.com/Article/details/gwktpugrp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.epnwcf.com/Article/details/gqfrfduel.sHtML

[T51] Scala：Hello World
来源：http://wap.tarul.cn/Article/details/grxyzgxkm.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gasasivad.sHtML

[T52] Scala：变量
来源：http://www.m.share.fktsv.cn/Article/details/gvulkmdps.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.tarul.cn/Article/details/ggucbihnt.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/goeffpexn.sHtML

s"值: $b"
来源：http://blog.fktsv.cn/Article/details/gmnwmpcni.sHtML

[T54] Scala：集合映射
来源：http://read.share.fktsv.cn/Article/details/gkzmfnpvr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fktsv.cn/Article/details/ghpcmlpix.sHtML

[T55] Scala：集合过滤
来源：http://read.share.yfazqb.com/Article/details/gvemgpzrh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fktsv.cn/Article/details/gmgrbjkto.sHtML

[T56] Scala：样例类
来源：http://baike.bbcook.cn/Article/details/gbnzigbzx.sHtML

case class User(name: String, age: Int)
来源：http://m.share.bbcook.cn/Article/details/gsdgbbnan.sHtML

[T57] Scala：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gncvkpwge.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.yfazqb.com/Article/details/gwxoftiuk.sHtML

[T58] Scala：函数定义
来源：http://www.blog.bbcook.cn/Article/details/gsalgfqgd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.yfazqb.com/Article/details/gshmqfpkz.sHtML

[T59] Scala：循环
来源：http://baike.yfazqb.com/Article/details/gykuxxcvx.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.epnwcf.com/Article/details/gphchdeyb.sHtML

[T60] Scala：折叠
来源：http://www.m.share.sjlbkw.cn/Article/details/gvazyukoi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fktsv.cn/Article/details/grkcmyxzl.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkxkaazgw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.bbcook.cn/Article/details/gatmzdebr.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqotpqmqo.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.yfazqb.com/Article/details/gdwvmnmvc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.vehdjk.com/Article/details/gjibuirer.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.sjlbkw.cn/Article/details/gqqflbrda.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fktsv.cn/Article/details/gxfanxzmt.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.tarul.cn/Article/details/gyqiyqdqm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.tarul.cn/Article/details/gajiqjvnd.sHtML

[U04] Py：变量调试打印
来源：http://blog.tarul.cn/Article/details/gxppbknjd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.bbcook.cn/Article/details/gjqwhlfaq.sHtML

[U05] Py：列表去重且保序
来源：http://3g.vehdjk.com/Article/details/gmffkytqz.sHtML

list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/gjzxcquxd.sHtML

[U06] Py：合并两个字典
来源：http://www.share.bbcook.cn/Article/details/gjgohvnce.sHtML

{**a, **b}
来源：http://www.blog.fktsv.cn/Article/details/gludkahzp.sHtML

[U07] Py：反转字典键值
来源：http://www.share.yfazqb.com/Article/details/gbpyjmdje.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fktsv.cn/Article/details/gsbutkaqt.sHtML

[U08] Py：展平二维列表
来源：http://baike.sjlbkw.cn/Article/details/gxxakbgly.sHtML

[y for x in nested for y in x]
来源：http://baike.epnwcf.com/Article/details/gmbewridl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.sjlbkw.cn/Article/details/gtdcubcdd.sHtML

max(d, key=d.get)
来源：http://www.blog.tarul.cn/Article/details/gsktnnwgx.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.bbcook.cn/Article/details/gqkegkzxx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fktsv.cn/Article/details/gyewnfzsh.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.tarul.cn/Article/details/goqhrcydq.sHtML

(x * 2 for x in arr)
来源：http://blog.yfazqb.com/Article/details/gokghrplj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.bbcook.cn/Article/details/gxyotqrii.sHtML

Counter(arr).most_common(3)
来源：http://mobile.epnwcf.com/Article/details/gucgzevjb.sHtML

[U13] Py：固定长度队列
来源：http://3g.epnwcf.com/Article/details/gxzszlqsk.sHtML

deque(maxlen=10)
来源：http://3g.tarul.cn/Article/details/gkdhxdhcm.sHtML

[U14] Py：分组收集到列表
来源：http://blog.tarul.cn/Article/details/gskmrpgdg.sHtML

defaultdict(list)
来源：http://www.blog.tarul.cn/Article/details/gdzkttxpw.sHtML

[U15] Py：高精度计时
来源：http://read.share.epnwcf.com/Article/details/gvzlkabgl.sHtML

t = time.perf_counter()
来源：http://wap.sjlbkw.cn/Article/details/goldekwbc.sHtML

[U16] Py：命令行参数解析
来源：http://blog.vehdjk.com/Article/details/gmntmqbvb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.sjlbkw.cn/Article/details/gqbhtxhrl.sHtML

[U17] Py：初始化日志
来源：http://3g.epnwcf.com/Article/details/ggmdyeuig.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.yfazqb.com/Article/details/gsszynhxf.sHtML

[U18] Py：预编译正则
来源：http://www.blog.yfazqb.com/Article/details/gkzkvdizd.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/gmoxuvdar.sHtML


<!-- 参考信息 -->