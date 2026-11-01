代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.epnwcf.com/Article/details/gksualohk.sHtML

[S02] C：变量与格式化输出
来源：http://blog.epnwcf.com/Article/details/gqtebswdp.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.vehdjk.com/Article/details/gcnijgtfb.sHtML

[S03] C：读入整数
来源：http://m.share.fktsv.cn/Article/details/gdvyxylos.sHtML

int x; scanf("%d", &x);
来源：http://blog.bbcook.cn/Article/details/gzwwqmrag.sHtML

[S04] C：字符串复制
来源：http://3g.yfazqb.com/Article/details/gkfniytwc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gybzhkqcq.sHtML

[S05] C：字符串长度
来源：http://mobile.tarul.cn/Article/details/gjodaabcg.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/gkyovvfdx.sHtML

[S06] C：字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gvndzgewr.sHtML

strcmp(a, b) == 0
来源：http://www.blog.vehdjk.com/Article/details/gecpwptwb.sHtML

[S07] C：数组遍历求和
来源：http://3g.vehdjk.com/Article/details/ghdeqwpca.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.sjlbkw.cn/Article/details/gcajukeoj.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.tarul.cn/Article/details/ghkpvchvx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/gfqcilkkm.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/gldesfdhg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gagnzlfnl.sHtML

[S10] C：指针与解引用
来源：http://blog.epnwcf.com/Article/details/gtnbrzbsr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.sjlbkw.cn/Article/details/gsjorjsgj.sHtML

[S11] C：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gvgoqklyq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.vehdjk.com/Article/details/geyxqhwsp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/gugdjeaaf.sHtML

fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gnitwvjnj.sHtML

[S12] C：写文件
来源：http://www.blog.epnwcf.com/Article/details/gpysszlqb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/govwebrcp.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/gvxgaycvw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.epnwcf.com/Article/details/giqaooxco.sHtML

[S14] C：枚举
来源：http://www.share.sjlbkw.cn/Article/details/getzlccxw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.sjlbkw.cn/Article/details/gqdfhywrb.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/geavhvpxm.sHtML

(double) a / b
来源：http://www.m.share.epnwcf.com/Article/details/gikmuwlly.sHtML

[S16] C：位操作置位
来源：http://blog.tarul.cn/Article/details/gmejiwwdm.sHtML

x |= (1 << 3);
来源：http://www.blog.tarul.cn/Article/details/ghicwtydq.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gcvaxgsxt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/gciimpsqg.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/grwtyrqed.sHtML

int main(int argc, char **argv)
来源：http://m.share.sjlbkw.cn/Article/details/gvlyfidhw.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/gjlasrhlo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gamokdkaz.sHtML

[S20] C：二分查找
来源：http://mobile.epnwcf.com/Article/details/gjjlamvnf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gjljmnrqj.sHtML

[S21] C：字符类别判断
来源：http://mobile.fktsv.cn/Article/details/gjnymyfdk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.sjlbkw.cn/Article/details/gauumukkc.sHtML

[S22] C：字符串转数字
来源：http://read.share.tarul.cn/Article/details/globlwrve.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.tarul.cn/Article/details/gpolttwil.sHtML

[S23] C：随机数
来源：http://3g.bbcook.cn/Article/details/gmkuuowho.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.bbcook.cn/Article/details/gpgdimolx.sHtML

[S24] C：获取本地时间
来源：http://baike.vehdjk.com/Article/details/gqfyqivsk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.tarul.cn/Article/details/gggyqkbhv.sHtML

[S25] C：内存拷贝
来源：http://www.share.yfazqb.com/Article/details/gkoklpkjx.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fktsv.cn/Article/details/gmcylhiic.sHtML

[S26] C：内存清零
来源：http://www.share.tarul.cn/Article/details/ghnqlostb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.vehdjk.com/Article/details/gxaaujumc.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/geksautdk.sHtML

const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gydlykagg.sHtML

[S28] C：静态变量
来源：http://3g.fktsv.cn/Article/details/gbwbkhgfg.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/giqxinwop.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/geolttmmk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.epnwcf.com/Article/details/gibsnjjfz.sHtML

[S30] C：头文件保护
来源：http://blog.bbcook.cn/Article/details/gubiocmfq.sHtML

#ifndef X_H
来源：http://www.m.share.vehdjk.com/Article/details/gkavvsbtr.sHtML

#define X_H
来源：http://www.blog.epnwcf.com/Article/details/gmfvpinnx.sHtML

#endif
来源：http://baike.yfazqb.com/Article/details/gxvhdgmim.sHtML

[S31] C++：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gywitdatb.sHtML

#include <iostream>
来源：http://mobile.epnwcf.com/Article/details/gdgckeuos.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtwjppdzl.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/gbanumcrs.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fktsv.cn/Article/details/gkyirzrxg.sHtML

[S33] C++：vector 增删
来源：http://baike.vehdjk.com/Article/details/gxeauexaf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.epnwcf.com/Article/details/gtehahtex.sHtML

[S34] C++：遍历 vector
来源：http://blog.fktsv.cn/Article/details/ghtfdtwpl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.bbcook.cn/Article/details/gvacsnosa.sHtML

[S35] C++：map
来源：http://read.share.epnwcf.com/Article/details/gyzzojizf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gxlxdcjaf.sHtML

[S36] C++：unordered_map
来源：http://www.blog.yfazqb.com/Article/details/gslqrcrci.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/ggmdbsuha.sHtML

[S37] C++：set
来源：http://blog.tarul.cn/Article/details/geaflcchy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.bbcook.cn/Article/details/ghbholwzv.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/gbhxoxcok.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/gmkcdtuog.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.bbcook.cn/Article/details/gmvphshvl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.tarul.cn/Article/details/gyxqatihl.sHtML

[S40] C++：查找元素
来源：http://www.share.tarul.cn/Article/details/gvnbwgbhs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.yfazqb.com/Article/details/gxizgywzd.sHtML

[S41] C++：类与构造函数
来源：http://www.share.epnwcf.com/Article/details/gjfkmejja.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/gamuhsyiv.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.bbcook.cn/Article/details/gmmedfrsu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.sjlbkw.cn/Article/details/ggyrieneg.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/gukurzhzm.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/glqmruqsr.sHtML

[S44] C++：引用传参
来源：http://baike.bbcook.cn/Article/details/gpzmulfyd.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/ghwdzwene.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gfnmxpvva.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/gezdsfzre.sHtML

[S46] C++：函数模板
来源：http://wap.bbcook.cn/Article/details/gwopgyucu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.bbcook.cn/Article/details/gxzwoejrd.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.yfazqb.com/Article/details/gvcdororq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.vehdjk.com/Article/details/gorijvhfs.sHtML

[S48] C++：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gljdaqljb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.tarul.cn/Article/details/gvmjngcux.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.bbcook.cn/Article/details/gxmsjjrxf.sHtML

[S49] C++：写文件
来源：http://m.share.fktsv.cn/Article/details/gidzkvqyu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.tarul.cn/Article/details/ggpnvdvea.sHtML

[S50] C++：格式化数字
来源：http://wap.epnwcf.com/Article/details/gopixmhbs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/ghofzsywf.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/ggyrlqpui.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/ggebadfhe.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.yfazqb.com/Article/details/gbfsrrbch.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.tarul.cn/Article/details/gsqnyofry.sHtML

[S53] C++：移动语义
来源：http://read.share.tarul.cn/Article/details/gpljvywuf.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fktsv.cn/Article/details/gnayuafif.sHtML

[S54] C++：异常处理
来源：http://3g.epnwcf.com/Article/details/goovsgaxc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.vehdjk.com/Article/details/gyxzgtxwx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.yfazqb.com/Article/details/gvbbosqhs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/gjetgjalf.sHtML

[S56] C++：optional
来源：http://m.share.tarul.cn/Article/details/guuazxljt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.epnwcf.com/Article/details/gbqvdwxjq.sHtML

[S57] C++：编译期常量
来源：http://mobile.bbcook.cn/Article/details/gnswettth.sHtML

constexpr int N = 10;
来源：http://read.share.yfazqb.com/Article/details/grfywxigh.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/gqorfifct.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/ghspxsume.sHtML

[S59] C++：静态断言
来源：http://www.m.share.tarul.cn/Article/details/gzoepuzwc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.yfazqb.com/Article/details/gatprmjjs.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fktsv.cn/Article/details/gimwxnoao.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/gkbozffud.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gdeboowzd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/gjwmerjlw.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvtlvszvq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.epnwcf.com/Article/details/ginoszipp.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gswqtusvz.sHtML

[T02] Kotlin：变量
来源：http://mobile.epnwcf.com/Article/details/gqsamcfdd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/gmxnezifb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.vehdjk.com/Article/details/gskjvjhtn.sHtML

"值: $b"
来源：http://m.share.bbcook.cn/Article/details/gsvwhdndl.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.epnwcf.com/Article/details/gckvuowyj.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/gjufmmcfg.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gquityjhr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.bbcook.cn/Article/details/gmudjxemh.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.bbcook.cn/Article/details/gfvgjzrbk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/grpcvfcff.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gmlphahla.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.epnwcf.com/Article/details/gxqswbres.sHtML

[T08] Kotlin：数据类
来源：http://mobile.vehdjk.com/Article/details/gxanvsafv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.bbcook.cn/Article/details/gkdclbvtf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.vehdjk.com/Article/details/gcfpnvzze.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.vehdjk.com/Article/details/gsaqfvbdj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.bbcook.cn/Article/details/gqqfquslq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.vehdjk.com/Article/details/gkqcfcyax.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/ghznppjns.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fktsv.cn/Article/details/gpnggaldh.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gxuzxzxki.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gmufwjsxh.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.yfazqb.com/Article/details/gweyphzin.sHtML

val m = mapOf("a" to 1)
来源：http://blog.bbcook.cn/Article/details/grnmuqjmv.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gwefwgusm.sHtML

for (i in 1..10) println(i)
来源：http://m.share.epnwcf.com/Article/details/glsjizjhv.sHtML

[T15] Kotlin：接口
来源：http://m.share.fktsv.cn/Article/details/gwphrliba.sHtML

interface Shape { fun area(): Double }
来源：http://3g.tarul.cn/Article/details/gwmjzwuxk.sHtML

[T16] Swift：Hello World
来源：http://read.share.fktsv.cn/Article/details/gqlxmkqkb.sHtML

print("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gxvjrwufu.sHtML

[T17] Swift：变量与常量
来源：http://3g.tarul.cn/Article/details/grfhzmucp.sHtML

var a = 1;  let b = 2
来源：http://www.share.tarul.cn/Article/details/gexcqabcb.sHtML

[T18] Swift：字符串插值
来源：http://m.share.tarul.cn/Article/details/gaoyfkezb.sHtML

"值: \(b)"
来源：http://baike.epnwcf.com/Article/details/gzhmdglcb.sHtML

[T19] Swift：可选绑定
来源：http://blog.yfazqb.com/Article/details/gtnknrzxe.sHtML

if let n = opt { print(n) }
来源：http://wap.tarul.cn/Article/details/gfvyxvpbz.sHtML

[T20] Swift：数组操作
来源：http://read.share.sjlbkw.cn/Article/details/gnqfrgkwr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fktsv.cn/Article/details/gldlqtkeo.sHtML

[T21] Swift：遍历
来源：http://mobile.sjlbkw.cn/Article/details/gpjalcdmu.sHtML

for x in a { print(x) }
来源：http://blog.sjlbkw.cn/Article/details/gltcyvzeh.sHtML

[T22] Swift：字典
来源：http://mobile.yfazqb.com/Article/details/gswrntibw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/gtwkrxpzv.sHtML

[T23] Swift：函数
来源：http://m.share.tarul.cn/Article/details/gxuauiowd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.yfazqb.com/Article/details/glrjlnjbu.sHtML

[T24] Swift：闭包
来源：http://www.m.share.epnwcf.com/Article/details/gljhjhmul.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.bbcook.cn/Article/details/gjjuvsxuu.sHtML

[T25] Swift：结构体
来源：http://mobile.tarul.cn/Article/details/gwvzrtahg.sHtML

struct P { var x: Int }
来源：http://3g.fktsv.cn/Article/details/gyupzrxdo.sHtML

[T26] Swift：类与重写
来源：http://mobile.tarul.cn/Article/details/gqddwmpct.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.epnwcf.com/Article/details/gycvguukm.sHtML

[T27] Swift：错误处理
来源：http://www.blog.epnwcf.com/Article/details/gtlzeuhpo.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/gdvjollhv.sHtML

[T28] Swift：枚举
来源：http://www.blog.vehdjk.com/Article/details/gfkfskviz.sHtML

enum Color { case red, green }
来源：http://3g.yfazqb.com/Article/details/gkvhmcmbg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.tarul.cn/Article/details/gdnzlojse.sHtML

guard let x = opt else { return }
来源：http://mobile.fktsv.cn/Article/details/gjhctjsrc.sHtML

[T30] Swift：协议
来源：http://www.blog.vehdjk.com/Article/details/gmnyrpnvj.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.sjlbkw.cn/Article/details/gsgzadkjz.sHtML

[T31] Lua：Hello World
来源：http://baike.tarul.cn/Article/details/gbwzocgpc.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gmemafgej.sHtML

[T32] Lua：局部变量
来源：http://baike.bbcook.cn/Article/details/gyeawpqud.sHtML

local a = 1
来源：http://read.share.fktsv.cn/Article/details/gjmlthvgn.sHtML

[T33] Lua：表（数组）
来源：http://wap.yfazqb.com/Article/details/gyyywyumn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fktsv.cn/Article/details/gxipxcnde.sHtML

[T34] Lua：遍历表
来源：http://blog.fktsv.cn/Article/details/gobdlxhuu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/geaymeslf.sHtML

[T35] Lua：字典表
来源：http://www.share.epnwcf.com/Article/details/gtilclbkj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.bbcook.cn/Article/details/ggqjwjibo.sHtML

[T36] Lua：函数
来源：http://www.m.share.epnwcf.com/Article/details/gqtsmguhz.sHtML

function add(a, b) return a + b end
来源：http://baike.fktsv.cn/Article/details/gtngxknjp.sHtML

[T37] Lua：字符串拼接
来源：http://wap.epnwcf.com/Article/details/gdflhaaas.sHtML

"a" .. "b"
来源：http://www.share.sjlbkw.cn/Article/details/gbldrluia.sHtML

[T38] Lua：条件
来源：http://wap.bbcook.cn/Article/details/gvhgvhtwu.sHtML

if x > 0 then print("正") end
来源：http://www.share.fktsv.cn/Article/details/gazpmikiq.sHtML

[T39] Lua：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/gksguqalt.sHtML

string.find(s, "%d+")
来源：http://wap.epnwcf.com/Article/details/gtzahrths.sHtML

[T40] Lua：元表
来源：http://blog.sjlbkw.cn/Article/details/ghzhihczw.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fktsv.cn/Article/details/gfxfnbjse.sHtML

[T41] Perl：Hello World
来源：http://m.share.vehdjk.com/Article/details/gqmicpfmv.sHtML

print "Hello\n";
来源：http://baike.sjlbkw.cn/Article/details/gvcyjymcs.sHtML

[T42] Perl：变量类型
来源：http://mobile.sjlbkw.cn/Article/details/gnofwiexr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gcaxskxes.sHtML

[T43] Perl：字符串插值
来源：http://blog.yfazqb.com/Article/details/gkwlostml.sHtML

"值: $a"
来源：http://m.share.epnwcf.com/Article/details/gggirvdpo.sHtML

[T44] Perl：条件
来源：http://baike.epnwcf.com/Article/details/gzdrymxae.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.yfazqb.com/Article/details/ghvizpwtc.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.tarul.cn/Article/details/gicdigbkt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.tarul.cn/Article/details/goprdypdx.sHtML

[T46] Perl：哈希操作
来源：http://www.share.bbcook.cn/Article/details/gmxvkczzh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/ghceumihu.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.tarul.cn/Article/details/gbheofukp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.vehdjk.com/Article/details/gvwlbdtof.sHtML

[T48] Perl：正则替换
来源：http://m.share.yfazqb.com/Article/details/gxhlvlnjr.sHtML

$s =~ s/old/new/g;
来源：http://wap.epnwcf.com/Article/details/gbveteyza.sHtML

[T49] Perl：函数
来源：http://wap.bbcook.cn/Article/details/gcmcnvnpz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gqlxmknre.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/geaolfulq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.yfazqb.com/Article/details/guohewpjj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.epnwcf.com/Article/details/gbllcpaiw.sHtML

[T51] Scala：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/ggfvxzxxp.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/gjrxbaary.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gnxumbhkf.sHtML

val a = 1;  var b = 2
来源：http://www.share.yfazqb.com/Article/details/gtxnzrmxe.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gtodusyuv.sHtML

s"值: $b"
来源：http://wap.bbcook.cn/Article/details/gzvjtusgl.sHtML

[T54] Scala：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/ghzlcmrap.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.yfazqb.com/Article/details/gzvcjkrje.sHtML

[T55] Scala：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gbrqnwnqd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.yfazqb.com/Article/details/gldyippls.sHtML

[T56] Scala：样例类
来源：http://www.blog.epnwcf.com/Article/details/grycnjppj.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.bbcook.cn/Article/details/gsgjcngbr.sHtML

[T57] Scala：模式匹配
来源：http://wap.vehdjk.com/Article/details/gzecnkeys.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gyzvyxepg.sHtML

[T58] Scala：函数定义
来源：http://m.share.fktsv.cn/Article/details/gnxqrvkzs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.vehdjk.com/Article/details/gkbdhkptk.sHtML

[T59] Scala：循环
来源：http://mobile.sjlbkw.cn/Article/details/gaogsmuoe.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.epnwcf.com/Article/details/gudpjgtyv.sHtML

[T60] Scala：折叠
来源：http://blog.yfazqb.com/Article/details/gzxnllsre.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/gzqgvcenj.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/guanavzbv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/grspzthqd.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/grsqklhgo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.tarul.cn/Article/details/gdzaektah.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.tarul.cn/Article/details/gqajydjua.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.bbcook.cn/Article/details/gbfawgext.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fktsv.cn/Article/details/gbtbkueih.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.sjlbkw.cn/Article/details/gcdlrmhuu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fktsv.cn/Article/details/grmjojwsj.sHtML

[U04] Py：变量调试打印
来源：http://www.share.vehdjk.com/Article/details/gdnmeodsv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.vehdjk.com/Article/details/grmchsnmd.sHtML

[U05] Py：列表去重且保序
来源：http://3g.epnwcf.com/Article/details/gxxpfyvgu.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gqlcfybif.sHtML

[U06] Py：合并两个字典
来源：http://baike.tarul.cn/Article/details/gprandbtu.sHtML

{**a, **b}
来源：http://m.share.fktsv.cn/Article/details/gxcktvbaw.sHtML

[U07] Py：反转字典键值
来源：http://baike.bbcook.cn/Article/details/gnsayilpv.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fktsv.cn/Article/details/gctghbowz.sHtML

[U08] Py：展平二维列表
来源：http://mobile.tarul.cn/Article/details/gbfehpqbi.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.sjlbkw.cn/Article/details/guymhuxhs.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.yfazqb.com/Article/details/gvsefhdlo.sHtML

max(d, key=d.get)
来源：http://baike.fktsv.cn/Article/details/ggqkujemm.sHtML

[U10] Py：按值排序字典
来源：http://www.share.yfazqb.com/Article/details/grokaenan.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.bbcook.cn/Article/details/gqibggoyt.sHtML

[U11] Py：生成器表达式
来源：http://3g.tarul.cn/Article/details/gvrcgyzvc.sHtML

(x * 2 for x in arr)
来源：http://baike.tarul.cn/Article/details/gmjgnrmcj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fktsv.cn/Article/details/gptwcgdac.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.bbcook.cn/Article/details/gymeslzsd.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.sjlbkw.cn/Article/details/gwkvtcssa.sHtML

deque(maxlen=10)
来源：http://read.share.fktsv.cn/Article/details/gvlirzxax.sHtML

[U14] Py：分组收集到列表
来源：http://blog.vehdjk.com/Article/details/guphhmgwb.sHtML

defaultdict(list)
来源：http://m.share.yfazqb.com/Article/details/gtgjqmpxs.sHtML

[U15] Py：高精度计时
来源：http://www.share.yfazqb.com/Article/details/ggszymyul.sHtML

t = time.perf_counter()
来源：http://www.m.share.epnwcf.com/Article/details/gcnggizku.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.epnwcf.com/Article/details/ghbdzwpsf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.sjlbkw.cn/Article/details/gnpmrbyxz.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.yfazqb.com/Article/details/gjwlsoxyo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.sjlbkw.cn/Article/details/gapzsqito.sHtML

[U18] Py：预编译正则
来源：http://baike.sjlbkw.cn/Article/details/ggphbpnup.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fktsv.cn/Article/details/gzeicoupp.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.bbcook.cn/Article/details/gzkjqjoct.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.sjlbkw.cn/Article/details/ghjzmkbex.sHtML

[U20] Py：缓存函数结果
来源：http://3g.yfazqb.com/Article/details/gfrbakxpd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.sjlbkw.cn/Article/details/gujjoguhn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.yfazqb.com/Article/details/gopvzamfs.sHtML

@contextlib.contextmanager
来源：http://mobile.tarul.cn/Article/details/gvhrigcsz.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.sjlbkw.cn/Article/details/gvozbjxsu.sHtML

list(zip(*m))
来源：http://wap.bbcook.cn/Article/details/gkoxkqddj.sHtML

[U23] Py：分块读取大文件
来源：http://blog.yfazqb.com/Article/details/gawtcgand.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.sjlbkw.cn/Article/details/gptnzdypd.sHtML

[U24] Py：路径操作
来源：http://wap.fktsv.cn/Article/details/gcudshjmf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.tarul.cn/Article/details/gpesuzuxu.sHtML


<!-- 参考信息 -->