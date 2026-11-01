代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/gwfkjuvmx.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/ghknmrgbf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/ghmcrdupx.sHtML

[R77] 读取用户输入
来源：http://3g.epnwcf.com/Article/details/gyeftbici.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.bbcook.cn/Article/details/gigozeanw.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/gdkctzizb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.yfazqb.com/Article/details/gmcvhyrwl.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.tarul.cn/Article/details/gowinjxip.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.sjlbkw.cn/Article/details/gpphwqxdn.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.sjlbkw.cn/Article/details/goyzxyvwj.sHtML

time ./run.sh
来源：http://3g.bbcook.cn/Article/details/giaetfrnt.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxrgntdjo.sHtML

S. C / C++ 专题
来源：http://m.share.sjlbkw.cn/Article/details/gnxlpgjja.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmwkmzxxu.sHtML

[S01] C：Hello World
来源：http://m.share.epnwcf.com/Article/details/gnsnnoslq.sHtML

#include <stdio.h>
来源：http://blog.bbcook.cn/Article/details/gtmzklcoz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.sjlbkw.cn/Article/details/gfdrdyfvc.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoltppfj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gswshffok.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/grcnilyfm.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/ggoxsmyia.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/gmecgsjjy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.tarul.cn/Article/details/gwuzymdia.sHtML

[S05] C：字符串长度
来源：http://m.share.bbcook.cn/Article/details/gbgkzkqoc.sHtML

strlen(s)
来源：http://baike.fktsv.cn/Article/details/gkeuwqumu.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/gvfdyfqxd.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.epnwcf.com/Article/details/gbfrrnxam.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjrdbzbe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.sjlbkw.cn/Article/details/gborlptud.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.bbcook.cn/Article/details/gifzhcogn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.bbcook.cn/Article/details/gffdgyszf.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fktsv.cn/Article/details/gubfeykop.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gfottdmoq.sHtML

[S10] C：指针与解引用
来源：http://3g.epnwcf.com/Article/details/gwohfrkey.sHtML

int *p = &a;  *p = 5;
来源：http://baike.sjlbkw.cn/Article/details/gcusbakfb.sHtML

[S11] C：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gukprzszs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/gjdvnsoaq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.yfazqb.com/Article/details/glgnqskhf.sHtML

fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gljhkdcdf.sHtML

[S12] C：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/gnxseggyb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gmjmxcrub.sHtML

[S13] C：宏定义
来源：http://www.share.sjlbkw.cn/Article/details/gcrumxxna.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fktsv.cn/Article/details/gqouckjqq.sHtML

[S14] C：枚举
来源：http://mobile.vehdjk.com/Article/details/gmnwkduzw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.tarul.cn/Article/details/gkzpjfuec.sHtML

[S15] C：类型转换
来源：http://blog.fktsv.cn/Article/details/gxjdpldjb.sHtML

(double) a / b
来源：http://baike.tarul.cn/Article/details/gwiaubzyd.sHtML

[S16] C：位操作置位
来源：http://read.share.epnwcf.com/Article/details/gjzfrodfk.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/gcadtyyhn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gsbbatncg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.bbcook.cn/Article/details/giewoepea.sHtML

[S18] C：命令行参数
来源：http://m.share.bbcook.cn/Article/details/gwjhvnazm.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/giqsyfink.sHtML

[S19] C：快速排序
来源：http://blog.sjlbkw.cn/Article/details/ghydbnaxg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/garaehpuf.sHtML

[S20] C：二分查找
来源：http://m.share.vehdjk.com/Article/details/gounebhwx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gtttbqrhb.sHtML

[S21] C：字符类别判断
来源：http://blog.sjlbkw.cn/Article/details/gjmvmozed.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.epnwcf.com/Article/details/gjjxzuwoh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/gegmfxeyk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.yfazqb.com/Article/details/gghvjmvyc.sHtML

[S23] C：随机数
来源：http://www.share.epnwcf.com/Article/details/guewhaqcv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.vehdjk.com/Article/details/gdlkgvebw.sHtML

[S24] C：获取本地时间
来源：http://mobile.fktsv.cn/Article/details/gvepzggwg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.yfazqb.com/Article/details/gosutdgez.sHtML

[S25] C：内存拷贝
来源：http://wap.fktsv.cn/Article/details/gtdpzqsxg.sHtML

memcpy(dst, src, n);
来源：http://www.share.epnwcf.com/Article/details/godkptfou.sHtML

[S26] C：内存清零
来源：http://mobile.fktsv.cn/Article/details/gvobdbgtc.sHtML

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/gdtcfkbej.sHtML

[S27] C：定义常量
来源：http://baike.tarul.cn/Article/details/grqpwypfs.sHtML

const double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gwbmncdaj.sHtML

[S28] C：静态变量
来源：http://3g.fktsv.cn/Article/details/glephwczs.sHtML

static int counter = 0;
来源：http://baike.bbcook.cn/Article/details/gvseynnzm.sHtML

[S29] C：变参函数
来源：http://read.share.yfazqb.com/Article/details/gunkugafo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.tarul.cn/Article/details/gecztsiua.sHtML

[S30] C：头文件保护
来源：http://www.blog.vehdjk.com/Article/details/gbpfaeget.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gmldfekxn.sHtML

#define X_H
来源：http://blog.tarul.cn/Article/details/gwegzgtih.sHtML

#endif
来源：http://m.share.bbcook.cn/Article/details/ghrloetpo.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gyuukggld.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gzdoxxezf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fktsv.cn/Article/details/goaqsdkgr.sHtML

[S32] C++：字符串
来源：http://3g.vehdjk.com/Article/details/gnqokxkvc.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fktsv.cn/Article/details/gcfoykoij.sHtML

[S33] C++：vector 增删
来源：http://baike.bbcook.cn/Article/details/gupgswrts.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gcmqxtjti.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.tarul.cn/Article/details/gayjcjbfm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gbpocnrqn.sHtML

[S35] C++：map
来源：http://3g.yfazqb.com/Article/details/glmhiaqwt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gnvkccndr.sHtML

[S36] C++：unordered_map
来源：http://3g.yfazqb.com/Article/details/gsorlofuu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/giygupphq.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/gzihhqxht.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.vehdjk.com/Article/details/gywdlukmw.sHtML

[S38] C++：排序
来源：http://3g.vehdjk.com/Article/details/gutfzgtnq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gsdhrcglg.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.bbcook.cn/Article/details/gqrnqoreb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.epnwcf.com/Article/details/glyucdlgz.sHtML

[S40] C++：查找元素
来源：http://blog.tarul.cn/Article/details/gjsqpxlwi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.sjlbkw.cn/Article/details/ghyoesilx.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.yfazqb.com/Article/details/ghinrsqxx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/ghfilcyff.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/gpfwxuwfd.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/gnlzemeai.sHtML

[S43] C++：智能指针
来源：http://wap.yfazqb.com/Article/details/gpqvhuygo.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.yfazqb.com/Article/details/ghniswgpa.sHtML

[S44] C++：引用传参
来源：http://blog.bbcook.cn/Article/details/gvadqdteu.sHtML

void inc(int &x) { ++x; }
来源：http://baike.bbcook.cn/Article/details/gkulrrzyz.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gihlxiirf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.epnwcf.com/Article/details/gcseuxrbb.sHtML

[S46] C++：函数模板
来源：http://wap.tarul.cn/Article/details/gssygfizs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.tarul.cn/Article/details/gcthwszia.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.yfazqb.com/Article/details/gvgemhhen.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fktsv.cn/Article/details/gjtwltjgl.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gkjdxeara.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.epnwcf.com/Article/details/ggoyxbogo.sHtML

while (std::getline(in, line)) { }
来源：http://blog.epnwcf.com/Article/details/gxndebpke.sHtML

[S49] C++：写文件
来源：http://wap.yfazqb.com/Article/details/grwyegxvc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/gollavuox.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/gjbgdfumt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.yfazqb.com/Article/details/ganzigdaf.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fktsv.cn/Article/details/golibsvew.sHtML

static_cast<double>(a) / b
来源：http://3g.sjlbkw.cn/Article/details/gwwfuoojw.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.vehdjk.com/Article/details/gwktobjsr.sHtML

int size() const noexcept { return n_; }
来源：http://blog.yfazqb.com/Article/details/gmffhloik.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/glvqtsvmw.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gftyqnued.sHtML

[S54] C++：异常处理
来源：http://m.share.epnwcf.com/Article/details/gxtrrzwqj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fktsv.cn/Article/details/gkxwugjhm.sHtML

[S55] C++：结构化绑定
来源：http://baike.fktsv.cn/Article/details/gpfdznyir.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.vehdjk.com/Article/details/galvmjvkp.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/gdvkttxht.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/gcfjbgyrt.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.yfazqb.com/Article/details/gwupyosdk.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/ghrxdpabn.sHtML

[S58] C++：命名空间
来源：http://mobile.fktsv.cn/Article/details/gfybqemmt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.vehdjk.com/Article/details/ggrsailaq.sHtML

[S59] C++：静态断言
来源：http://www.share.vehdjk.com/Article/details/grxkxurlc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.tarul.cn/Article/details/gpqzcfguc.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fktsv.cn/Article/details/gusqphalt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fktsv.cn/Article/details/giakvppww.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmskovvcz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/gechnfqjp.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ggeofhiht.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fktsv.cn/Article/details/gqgvcjcgn.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gxvhqxbdq.sHtML

[T02] Kotlin：变量
来源：http://m.share.vehdjk.com/Article/details/gggabbdrb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.epnwcf.com/Article/details/gszjgrazg.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fktsv.cn/Article/details/guhrywauc.sHtML

"值: $b"
来源：http://blog.fktsv.cn/Article/details/gdkwhchts.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/gffhbifxl.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.vehdjk.com/Article/details/gfifpmjeg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.yfazqb.com/Article/details/gtuuyqodf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.tarul.cn/Article/details/gibehvkrp.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fktsv.cn/Article/details/goqyulblm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/gosyyqhvh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gacwuityc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.bbcook.cn/Article/details/gvqhpwiqf.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fktsv.cn/Article/details/gkqifwcpb.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.yfazqb.com/Article/details/gqsiwihcn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.sjlbkw.cn/Article/details/gpygrklmh.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.tarul.cn/Article/details/glczpekni.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.tarul.cn/Article/details/godbjfdgd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.yfazqb.com/Article/details/gzkvosgsl.sHtML

[T11] Kotlin：协程
来源：http://blog.bbcook.cn/Article/details/giexphimp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.bbcook.cn/Article/details/grfjgnyls.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fktsv.cn/Article/details/gnaykbwve.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fktsv.cn/Article/details/guwacmllm.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.sjlbkw.cn/Article/details/gmehbgydi.sHtML

val m = mapOf("a" to 1)
来源：http://baike.tarul.cn/Article/details/gqaeuwxnr.sHtML

[T14] Kotlin：循环
来源：http://baike.sjlbkw.cn/Article/details/gnxduiait.sHtML

for (i in 1..10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gomiiarkz.sHtML

[T15] Kotlin：接口
来源：http://blog.bbcook.cn/Article/details/ghiwomgpe.sHtML

interface Shape { fun area(): Double }
来源：http://wap.sjlbkw.cn/Article/details/gnrjitauv.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gysvcvjke.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gdhymyzed.sHtML

[T17] Swift：变量与常量
来源：http://blog.epnwcf.com/Article/details/gwuvbqlxq.sHtML

var a = 1;  let b = 2
来源：http://www.share.yfazqb.com/Article/details/gyvtwperv.sHtML

[T18] Swift：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gcddamkaz.sHtML

"值: \(b)"
来源：http://blog.fktsv.cn/Article/details/gmytanmma.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjogkaio.sHtML

if let n = opt { print(n) }
来源：http://www.blog.vehdjk.com/Article/details/grfteeqiy.sHtML

[T20] Swift：数组操作
来源：http://read.share.sjlbkw.cn/Article/details/gzjvygfmk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.epnwcf.com/Article/details/gtklojhcu.sHtML

[T21] Swift：遍历
来源：http://m.share.epnwcf.com/Article/details/givxqhgyu.sHtML

for x in a { print(x) }
来源：http://3g.bbcook.cn/Article/details/gvcsdjrdl.sHtML

[T22] Swift：字典
来源：http://blog.epnwcf.com/Article/details/gmncyaysm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.yfazqb.com/Article/details/gxpqygxpx.sHtML

[T23] Swift：函数
来源：http://m.share.vehdjk.com/Article/details/gmreskbve.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fktsv.cn/Article/details/gtdvnboqn.sHtML

[T24] Swift：闭包
来源：http://www.m.share.bbcook.cn/Article/details/glddoinkq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gtkvfdfeo.sHtML

[T25] Swift：结构体
来源：http://www.m.share.sjlbkw.cn/Article/details/gstfpzwqt.sHtML

struct P { var x: Int }
来源：http://www.m.share.bbcook.cn/Article/details/goyccreeb.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fktsv.cn/Article/details/gzohjmevq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.yfazqb.com/Article/details/gzdbydrri.sHtML

[T27] Swift：错误处理
来源：http://mobile.bbcook.cn/Article/details/geqaaojox.sHtML

do { try f() } catch { print(error) }
来源：http://3g.tarul.cn/Article/details/gprlhjbqj.sHtML

[T28] Swift：枚举
来源：http://wap.yfazqb.com/Article/details/gnhguaauk.sHtML

enum Color { case red, green }
来源：http://www.share.vehdjk.com/Article/details/ghwtewyjs.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fktsv.cn/Article/details/gqznbzfab.sHtML

guard let x = opt else { return }
来源：http://www.m.share.tarul.cn/Article/details/ginfyelir.sHtML

[T30] Swift：协议
来源：http://blog.epnwcf.com/Article/details/gxzvrpcxq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.vehdjk.com/Article/details/gywvyuypv.sHtML

[T31] Lua：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gujoxxkey.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/glfsmfavz.sHtML

[T32] Lua：局部变量
来源：http://baike.bbcook.cn/Article/details/gigjehagp.sHtML

local a = 1
来源：http://www.share.epnwcf.com/Article/details/gxbnlkojj.sHtML

[T33] Lua：表（数组）
来源：http://baike.epnwcf.com/Article/details/gntroammc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fktsv.cn/Article/details/gxnayhcaz.sHtML

[T34] Lua：遍历表
来源：http://baike.yfazqb.com/Article/details/gtvuftsma.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.yfazqb.com/Article/details/ghddiwewe.sHtML

[T35] Lua：字典表
来源：http://m.share.epnwcf.com/Article/details/gkvhgvsmn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.yfazqb.com/Article/details/giuuckduv.sHtML

[T36] Lua：函数
来源：http://www.share.epnwcf.com/Article/details/gztrhjvws.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.bbcook.cn/Article/details/gijesqdov.sHtML

[T37] Lua：字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gqamxpeii.sHtML

"a" .. "b"
来源：http://www.share.fktsv.cn/Article/details/ghvxanrmk.sHtML

[T38] Lua：条件
来源：http://wap.fktsv.cn/Article/details/ghwscflhw.sHtML

if x > 0 then print("正") end
来源：http://m.share.vehdjk.com/Article/details/gnxlkvtod.sHtML

[T39] Lua：模式匹配
来源：http://3g.epnwcf.com/Article/details/gqzzncxva.sHtML

string.find(s, "%d+")
来源：http://wap.fktsv.cn/Article/details/gyhvwzchj.sHtML

[T40] Lua：元表
来源：http://www.blog.yfazqb.com/Article/details/gsdmyiwtt.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.sjlbkw.cn/Article/details/gmbyotxik.sHtML

[T41] Perl：Hello World
来源：http://read.share.fktsv.cn/Article/details/gxwsvorbc.sHtML

print "Hello\n";
来源：http://www.blog.vehdjk.com/Article/details/geulhceec.sHtML

[T42] Perl：变量类型
来源：http://baike.bbcook.cn/Article/details/gpzsvcbmp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.yfazqb.com/Article/details/gxrjbdwsu.sHtML

[T43] Perl：字符串插值
来源：http://wap.epnwcf.com/Article/details/grtksesuz.sHtML

"值: $a"
来源：http://www.m.share.epnwcf.com/Article/details/gnabokrru.sHtML

[T44] Perl：条件
来源：http://www.share.yfazqb.com/Article/details/ghxtxixip.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.tarul.cn/Article/details/gbyvmpfjn.sHtML

[T45] Perl：数组遍历
来源：http://m.share.epnwcf.com/Article/details/gwezvrnae.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.yfazqb.com/Article/details/grytcufjj.sHtML

[T46] Perl：哈希操作
来源：http://mobile.tarul.cn/Article/details/giabncnut.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.epnwcf.com/Article/details/gidmtqyub.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fktsv.cn/Article/details/gjmvaltbh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fktsv.cn/Article/details/gjqmkknnl.sHtML

[T48] Perl：正则替换
来源：http://baike.vehdjk.com/Article/details/glzaswqhg.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/giexwqxnd.sHtML

[T49] Perl：函数
来源：http://baike.bbcook.cn/Article/details/glxvgttti.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gydqnynun.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gpxudhqjn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fktsv.cn/Article/details/gaatkkqbt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fktsv.cn/Article/details/gxggxrmje.sHtML

[T51] Scala：Hello World
来源：http://mobile.yfazqb.com/Article/details/gpftmhexy.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gsozauqaz.sHtML

[T52] Scala：变量
来源：http://mobile.yfazqb.com/Article/details/gytvfluzh.sHtML

val a = 1;  var b = 2
来源：http://blog.epnwcf.com/Article/details/grsdrfmcd.sHtML

[T53] Scala：字符串插值
来源：http://3g.yfazqb.com/Article/details/gumnkwvau.sHtML

s"值: $b"
来源：http://wap.tarul.cn/Article/details/gnjdkwrry.sHtML

[T54] Scala：集合映射
来源：http://www.blog.vehdjk.com/Article/details/greesaghx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.yfazqb.com/Article/details/gkrjeejlz.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gjzvkyswh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fktsv.cn/Article/details/gbvjcakyk.sHtML

[T56] Scala：样例类
来源：http://3g.epnwcf.com/Article/details/gmapbpvbh.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/guilrulfq.sHtML

[T57] Scala：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/giynpkihi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.bbcook.cn/Article/details/gunhutyoi.sHtML

[T58] Scala：函数定义
来源：http://baike.vehdjk.com/Article/details/gtjwggldn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fktsv.cn/Article/details/gsjuudajc.sHtML

[T59] Scala：循环
来源：http://www.share.tarul.cn/Article/details/gdzxuwwls.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gbyghsnkq.sHtML

[T60] Scala：折叠
来源：http://read.share.yfazqb.com/Article/details/gurnhlyjb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.sjlbkw.cn/Article/details/ghcumqymj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gyoucbvvf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/gwbipikra.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gaesnlrsf.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/gnfqsxgnw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.vehdjk.com/Article/details/gkvkinxjc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.vehdjk.com/Article/details/glsxzbvdf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.tarul.cn/Article/details/guqaatdqh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.yfazqb.com/Article/details/gwfepvwqf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.bbcook.cn/Article/details/gcdqdosst.sHtML

[U04] Py：变量调试打印
来源：http://baike.yfazqb.com/Article/details/gwaziglqu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.epnwcf.com/Article/details/gzrhgobfm.sHtML

[U05] Py：列表去重且保序
来源：http://3g.sjlbkw.cn/Article/details/gntizoopa.sHtML

list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/ghvfrxgtp.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.epnwcf.com/Article/details/geuwurrxn.sHtML

{**a, **b}
来源：http://www.share.fktsv.cn/Article/details/gdjqaoswr.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fktsv.cn/Article/details/ghrefyfci.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.epnwcf.com/Article/details/genyomabo.sHtML

[U08] Py：展平二维列表
来源：http://baike.tarul.cn/Article/details/gaqtyzfji.sHtML

[y for x in nested for y in x]
来源：http://read.share.fktsv.cn/Article/details/gtusvfvjs.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.vehdjk.com/Article/details/gcznacjpy.sHtML

max(d, key=d.get)
来源：http://wap.tarul.cn/Article/details/gmgypqcvx.sHtML

[U10] Py：按值排序字典
来源：http://wap.fktsv.cn/Article/details/ggscufyhe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.bbcook.cn/Article/details/gjanlwjpy.sHtML

[U11] Py：生成器表达式
来源：http://mobile.tarul.cn/Article/details/gndqcfjer.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.epnwcf.com/Article/details/gxomuvmbm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.epnwcf.com/Article/details/gnvccihrm.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.epnwcf.com/Article/details/goblrnaka.sHtML

[U13] Py：固定长度队列
来源：http://baike.vehdjk.com/Article/details/gygnolkya.sHtML

deque(maxlen=10)
来源：http://read.share.vehdjk.com/Article/details/gbawpffdx.sHtML

[U14] Py：分组收集到列表
来源：http://baike.bbcook.cn/Article/details/gisiqaenp.sHtML

defaultdict(list)
来源：http://m.share.fktsv.cn/Article/details/ghsvvesqa.sHtML

[U15] Py：高精度计时
来源：http://m.share.epnwcf.com/Article/details/gizlkgjgu.sHtML

t = time.perf_counter()
来源：http://3g.tarul.cn/Article/details/gndnjsahu.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.epnwcf.com/Article/details/gblukrrwd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.tarul.cn/Article/details/gbfqvjnmy.sHtML


<!-- 参考信息 -->