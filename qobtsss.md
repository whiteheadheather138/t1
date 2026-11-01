代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.tarul.cn/Article/details/gzzglawyk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fktsv.cn/Article/details/gvezrgten.sHtML

int *p = &a;  *p = 5;
来源：http://blog.sjlbkw.cn/Article/details/gdsmfwybv.sHtML

[S11] C：逐行读文件
来源：http://3g.fktsv.cn/Article/details/glbgtqzjp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.bbcook.cn/Article/details/gnujpinqa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.yfazqb.com/Article/details/gmnakaoud.sHtML

fclose(f);
来源：http://blog.yfazqb.com/Article/details/gkbaorlyg.sHtML

[S12] C：写文件
来源：http://mobile.vehdjk.com/Article/details/gdsdurmia.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.epnwcf.com/Article/details/ggpgdzmyx.sHtML

[S13] C：宏定义
来源：http://www.share.bbcook.cn/Article/details/ghethauqf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.epnwcf.com/Article/details/gqqpklaee.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/gyemgzyao.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.epnwcf.com/Article/details/gonnczwjp.sHtML

[S15] C：类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gdvaucizl.sHtML

(double) a / b
来源：http://baike.sjlbkw.cn/Article/details/gforenimj.sHtML

[S16] C：位操作置位
来源：http://mobile.epnwcf.com/Article/details/gtvtzwqdv.sHtML

x |= (1 << 3);
来源：http://baike.epnwcf.com/Article/details/guvdetrmb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.epnwcf.com/Article/details/gapxcynlb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/gaoojgdhw.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/goepbwnaf.sHtML

int main(int argc, char **argv)
来源：http://read.share.fktsv.cn/Article/details/gfopqbsbi.sHtML

[S19] C：快速排序
来源：http://blog.yfazqb.com/Article/details/gxkdjrcxe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gkwsupuuz.sHtML

[S20] C：二分查找
来源：http://wap.yfazqb.com/Article/details/gvrotvxvb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gzsefmpnd.sHtML

[S21] C：字符类别判断
来源：http://baike.sjlbkw.cn/Article/details/gedbmqeop.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyriceeud.sHtML

[S22] C：字符串转数字
来源：http://wap.fktsv.cn/Article/details/gnmxnsvvd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/gelghjuwk.sHtML

[S23] C：随机数
来源：http://wap.fktsv.cn/Article/details/gdrrwxxas.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fktsv.cn/Article/details/gektofpxq.sHtML

[S24] C：获取本地时间
来源：http://wap.sjlbkw.cn/Article/details/gqahkevrd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.epnwcf.com/Article/details/gmcvqpnto.sHtML

[S25] C：内存拷贝
来源：http://wap.vehdjk.com/Article/details/gjnpnjvcd.sHtML

memcpy(dst, src, n);
来源：http://m.share.tarul.cn/Article/details/gjlvnglds.sHtML

[S26] C：内存清零
来源：http://www.blog.epnwcf.com/Article/details/gwgfnrfpg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.vehdjk.com/Article/details/gqurtxgmu.sHtML

[S27] C：定义常量
来源：http://www.share.sjlbkw.cn/Article/details/gbdvaqlvo.sHtML

const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gsvbzhwaz.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/gfdkxmmor.sHtML

static int counter = 0;
来源：http://blog.bbcook.cn/Article/details/goecxukkc.sHtML

[S29] C：变参函数
来源：http://read.share.tarul.cn/Article/details/goczkjhlb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fktsv.cn/Article/details/gmhyauqkk.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/gpeyultpd.sHtML

#ifndef X_H
来源：http://baike.sjlbkw.cn/Article/details/gjcdvumuc.sHtML

#define X_H
来源：http://www.share.vehdjk.com/Article/details/geajanhsw.sHtML

#endif
来源：http://www.m.share.bbcook.cn/Article/details/ggoowcziz.sHtML

[S31] C++：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gqsjlhpnq.sHtML

#include <iostream>
来源：http://www.share.vehdjk.com/Article/details/geyzieslf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/guxufcbug.sHtML

[S32] C++：字符串
来源：http://www.share.vehdjk.com/Article/details/gyjvbjpqy.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/gygougwvm.sHtML

[S33] C++：vector 增删
来源：http://read.share.bbcook.cn/Article/details/givgpwdff.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fktsv.cn/Article/details/grlzxhkca.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.tarul.cn/Article/details/gfxnijsfm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fktsv.cn/Article/details/gpmhompwi.sHtML

[S35] C++：map
来源：http://wap.vehdjk.com/Article/details/gicmcaady.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gjfqhxbds.sHtML

[S36] C++：unordered_map
来源：http://baike.epnwcf.com/Article/details/gtiskpzvq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gbkgdqsnp.sHtML

[S37] C++：set
来源：http://3g.vehdjk.com/Article/details/gcbjrtzpx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjemkdxgp.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gqiddnbiq.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gcudppqpc.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/gbbaelmcg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.bbcook.cn/Article/details/gpomfmqgz.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gaqeyrkgl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/gflnkgnyz.sHtML

[S41] C++：类与构造函数
来源：http://wap.sjlbkw.cn/Article/details/ginwpcbzd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.vehdjk.com/Article/details/gfzblhiis.sHtML

[S42] C++：继承与虚函数
来源：http://3g.bbcook.cn/Article/details/garvziohn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/gmgldyuiw.sHtML

[S43] C++：智能指针
来源：http://mobile.epnwcf.com/Article/details/gotoybhdj.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.yfazqb.com/Article/details/grxgjexql.sHtML

[S44] C++：引用传参
来源：http://m.share.tarul.cn/Article/details/gjpsnenbl.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.bbcook.cn/Article/details/ghthyndlz.sHtML

[S45] C++：lambda
来源：http://wap.tarul.cn/Article/details/ggyuhiqhb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/ghmkfwsju.sHtML

[S46] C++：函数模板
来源：http://www.blog.epnwcf.com/Article/details/ghnodtvcm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.bbcook.cn/Article/details/gapbjiqjp.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fktsv.cn/Article/details/gljhwgqni.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.tarul.cn/Article/details/gughcaffe.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/glqohlqkb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.vehdjk.com/Article/details/gklerdcnj.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.tarul.cn/Article/details/guynofyok.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gyuicpgcv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.vehdjk.com/Article/details/ggfcmmuqa.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.tarul.cn/Article/details/gubyyyehd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.tarul.cn/Article/details/gybpemogz.sHtML

[S51] C++：显式类型转换
来源：http://www.share.bbcook.cn/Article/details/guxcogbya.sHtML

static_cast<double>(a) / b
来源：http://wap.epnwcf.com/Article/details/gxfkqnuud.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fktsv.cn/Article/details/gkeeqlwqw.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/gpxkbmpeo.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/ggpkddpev.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.yfazqb.com/Article/details/gzrmnrgdr.sHtML

[S54] C++：异常处理
来源：http://www.blog.yfazqb.com/Article/details/gmfgducku.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/gisacpxub.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fktsv.cn/Article/details/gcxlmrxuw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.epnwcf.com/Article/details/gbszacnik.sHtML

[S56] C++：optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhztypbd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.sjlbkw.cn/Article/details/ghnrywrzb.sHtML

[S57] C++：编译期常量
来源：http://wap.sjlbkw.cn/Article/details/ggjfopkiq.sHtML

constexpr int N = 10;
来源：http://blog.bbcook.cn/Article/details/ggvkbxbai.sHtML

[S58] C++：命名空间
来源：http://wap.sjlbkw.cn/Article/details/gzctehfye.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.yfazqb.com/Article/details/gjzfjcwpx.sHtML

[S59] C++：静态断言
来源：http://www.share.epnwcf.com/Article/details/gefavtlel.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.tarul.cn/Article/details/gncqzroja.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gmnbfldra.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.vehdjk.com/Article/details/glbyfcwke.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwuqbamwj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/ghokhxgkm.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gyvqtpawj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.yfazqb.com/Article/details/gcapfvwrd.sHtML

println("Hello")
来源：http://wap.vehdjk.com/Article/details/gcjaysfvf.sHtML

[T02] Kotlin：变量
来源：http://blog.fktsv.cn/Article/details/gqrzmwnqu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.epnwcf.com/Article/details/ggzzupeqx.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.yfazqb.com/Article/details/gjclcabyu.sHtML

"值: $b"
来源：http://blog.yfazqb.com/Article/details/gtyzmduwz.sHtML

[T04] Kotlin：空安全
来源：http://baike.bbcook.cn/Article/details/gymdrlgbo.sHtML

val n: String? = null;  n?.length
来源：http://wap.sjlbkw.cn/Article/details/glqrqclpc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gxfpbdqko.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.tarul.cn/Article/details/ghawlrznj.sHtML

[T06] Kotlin：集合映射
来源：http://wap.tarul.cn/Article/details/gsmpeomhh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gkjjuheif.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/goqhhqhog.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.bbcook.cn/Article/details/gvnfbsxil.sHtML

[T08] Kotlin：数据类
来源：http://3g.tarul.cn/Article/details/garpzfkap.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.sjlbkw.cn/Article/details/gvqcigzaz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.epnwcf.com/Article/details/ggretezyq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fktsv.cn/Article/details/goldsmfvq.sHtML

[T10] Kotlin：默认参数
来源：http://wap.sjlbkw.cn/Article/details/gxrjthxez.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fktsv.cn/Article/details/glldoouqm.sHtML

[T11] Kotlin：协程
来源：http://m.share.fktsv.cn/Article/details/gfvtvcuoy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.bbcook.cn/Article/details/gxpaftozn.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.vehdjk.com/Article/details/gacwojdlw.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gvenoujei.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fktsv.cn/Article/details/gfmzkprix.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fktsv.cn/Article/details/gfgbqpfhd.sHtML

[T14] Kotlin：循环
来源：http://baike.fktsv.cn/Article/details/gfqrxrjag.sHtML

for (i in 1..10) println(i)
来源：http://wap.sjlbkw.cn/Article/details/gskmdanql.sHtML

[T15] Kotlin：接口
来源：http://m.share.bbcook.cn/Article/details/ggyuhpazs.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gykmvbfwq.sHtML

[T16] Swift：Hello World
来源：http://m.share.tarul.cn/Article/details/gjmjpyoez.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gdwtfwwwt.sHtML

[T17] Swift：变量与常量
来源：http://blog.sjlbkw.cn/Article/details/gfpaswzyb.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.tarul.cn/Article/details/garrpoxgr.sHtML

[T18] Swift：字符串插值
来源：http://wap.tarul.cn/Article/details/gtifabsul.sHtML

"值: \(b)"
来源：http://www.m.share.vehdjk.com/Article/details/gturqqppe.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fktsv.cn/Article/details/geqfrqwsp.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/gwsefkgki.sHtML

[T20] Swift：数组操作
来源：http://wap.bbcook.cn/Article/details/glwatjyew.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.vehdjk.com/Article/details/gtilfrwti.sHtML

[T21] Swift：遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gfthpeotm.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/gplhebjna.sHtML

[T22] Swift：字典
来源：http://www.share.bbcook.cn/Article/details/ggeutgkvd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.yfazqb.com/Article/details/gsbmwbphb.sHtML

[T23] Swift：函数
来源：http://baike.tarul.cn/Article/details/gwlmijrid.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.bbcook.cn/Article/details/gyrdbhgwr.sHtML

[T24] Swift：闭包
来源：http://blog.fktsv.cn/Article/details/gscfpvxiw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/getwzxvoo.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/glqbetkva.sHtML

struct P { var x: Int }
来源：http://wap.bbcook.cn/Article/details/gmgtoaphs.sHtML

[T26] Swift：类与重写
来源：http://www.share.tarul.cn/Article/details/gghqvuspm.sHtML

class A: Base { override func f() {} }
来源：http://read.share.vehdjk.com/Article/details/gavaykcyz.sHtML

[T27] Swift：错误处理
来源：http://read.share.vehdjk.com/Article/details/ggxqddjwx.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.epnwcf.com/Article/details/gjbdfexzz.sHtML

[T28] Swift：枚举
来源：http://read.share.epnwcf.com/Article/details/gwssoxrqs.sHtML

enum Color { case red, green }
来源：http://m.share.bbcook.cn/Article/details/gnaayhovm.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fktsv.cn/Article/details/gsiclxgok.sHtML

guard let x = opt else { return }
来源：http://www.m.share.tarul.cn/Article/details/gemwzxpaz.sHtML

[T30] Swift：协议
来源：http://3g.epnwcf.com/Article/details/gvjugcheq.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.vehdjk.com/Article/details/gzwzrlgtn.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/gofdcuckv.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/ghzxivoob.sHtML

[T32] Lua：局部变量
来源：http://baike.vehdjk.com/Article/details/gzrcdshhn.sHtML

local a = 1
来源：http://read.share.fktsv.cn/Article/details/gtblwnzne.sHtML

[T33] Lua：表（数组）
来源：http://read.share.yfazqb.com/Article/details/glmuxycds.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.bbcook.cn/Article/details/gfxtpsmaf.sHtML

[T34] Lua：遍历表
来源：http://3g.vehdjk.com/Article/details/gsbaqodgt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.tarul.cn/Article/details/gdnbnnlyd.sHtML

[T35] Lua：字典表
来源：http://blog.epnwcf.com/Article/details/gltxzthhn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fktsv.cn/Article/details/gfdxbodsy.sHtML

[T36] Lua：函数
来源：http://read.share.yfazqb.com/Article/details/gsywcgqiy.sHtML

function add(a, b) return a + b end
来源：http://www.blog.sjlbkw.cn/Article/details/gyfpsgzcc.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gofhpeutf.sHtML

"a" .. "b"
来源：http://3g.tarul.cn/Article/details/gzlkbhpgq.sHtML

[T38] Lua：条件
来源：http://www.share.vehdjk.com/Article/details/guvldesvl.sHtML

if x > 0 then print("正") end
来源：http://wap.tarul.cn/Article/details/gofzbniez.sHtML

[T39] Lua：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gkigskchw.sHtML

string.find(s, "%d+")
来源：http://baike.sjlbkw.cn/Article/details/gzrbveaut.sHtML

[T40] Lua：元表
来源：http://wap.sjlbkw.cn/Article/details/gytkbpqcd.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fktsv.cn/Article/details/gupcbrffc.sHtML

[T41] Perl：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/guiisdakr.sHtML

print "Hello\n";
来源：http://read.share.vehdjk.com/Article/details/gvhctgtml.sHtML

[T42] Perl：变量类型
来源：http://mobile.epnwcf.com/Article/details/gnucotegx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.sjlbkw.cn/Article/details/gcqrguqmr.sHtML

[T43] Perl：字符串插值
来源：http://baike.epnwcf.com/Article/details/gmzmqduia.sHtML

"值: $a"
来源：http://www.share.tarul.cn/Article/details/gcticfguo.sHtML

[T44] Perl：条件
来源：http://blog.bbcook.cn/Article/details/gjicfffqf.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.vehdjk.com/Article/details/gnqdpbuud.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gqmiusgrb.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fktsv.cn/Article/details/ghyecsbpd.sHtML

[T46] Perl：哈希操作
来源：http://www.share.vehdjk.com/Article/details/gtalsajko.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.vehdjk.com/Article/details/gwoksjguo.sHtML

[T47] Perl：正则捕获
来源：http://mobile.tarul.cn/Article/details/gsivakrxt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.tarul.cn/Article/details/gfgotdano.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.epnwcf.com/Article/details/ggomiiffz.sHtML

$s =~ s/old/new/g;
来源：http://m.share.yfazqb.com/Article/details/gizbgyfhz.sHtML

[T49] Perl：函数
来源：http://read.share.epnwcf.com/Article/details/gviqbatje.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/giphxrnap.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gerptfklk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fktsv.cn/Article/details/gdabnnykw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.yfazqb.com/Article/details/gwmhtikjh.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gdxgdquwc.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gszeqtxpe.sHtML

[T52] Scala：变量
来源：http://read.share.epnwcf.com/Article/details/gtltcumos.sHtML

val a = 1;  var b = 2
来源：http://m.share.sjlbkw.cn/Article/details/gykgednck.sHtML

[T53] Scala：字符串插值
来源：http://3g.fktsv.cn/Article/details/ghzhuqhjq.sHtML

s"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gbolybzne.sHtML

[T54] Scala：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gabedqpoy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.yfazqb.com/Article/details/gvvhamnvi.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/glqakdkgt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.vehdjk.com/Article/details/gyresquyu.sHtML

[T56] Scala：样例类
来源：http://www.blog.fktsv.cn/Article/details/gbjlghkbc.sHtML

case class User(name: String, age: Int)
来源：http://blog.yfazqb.com/Article/details/ghhvfpxvv.sHtML

[T57] Scala：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/gsuhpwady.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.yfazqb.com/Article/details/gueuvnear.sHtML

[T58] Scala：函数定义
来源：http://read.share.vehdjk.com/Article/details/gxxuhtcbi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.tarul.cn/Article/details/gfxasyidm.sHtML

[T59] Scala：循环
来源：http://wap.fktsv.cn/Article/details/gthdnfita.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.bbcook.cn/Article/details/gxmlmavbo.sHtML

[T60] Scala：折叠
来源：http://wap.tarul.cn/Article/details/gemptxnbk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.vehdjk.com/Article/details/guumvarex.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/grrpjekfo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fktsv.cn/Article/details/gdcuzoofm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/guyxtpszy.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fktsv.cn/Article/details/ggbwetghx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.vehdjk.com/Article/details/gdilvqnrk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.vehdjk.com/Article/details/gecespaxx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.vehdjk.com/Article/details/gdyzpbkab.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.tarul.cn/Article/details/gyaewwnmj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gvctpllju.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fktsv.cn/Article/details/gsniyatkg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.bbcook.cn/Article/details/gffblmifo.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.tarul.cn/Article/details/gowahihnc.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gkzjscbkn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.bbcook.cn/Article/details/gsnhkdvng.sHtML

{**a, **b}
来源：http://wap.yfazqb.com/Article/details/gmpitylnj.sHtML

[U07] Py：反转字典键值
来源：http://www.share.sjlbkw.cn/Article/details/gegleqovq.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.sjlbkw.cn/Article/details/gtmrihlez.sHtML

[U08] Py：展平二维列表
来源：http://blog.fktsv.cn/Article/details/gezqemnbz.sHtML

[y for x in nested for y in x]
来源：http://wap.vehdjk.com/Article/details/grqdwisqo.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.yfazqb.com/Article/details/gkmhrfzug.sHtML

max(d, key=d.get)
来源：http://3g.sjlbkw.cn/Article/details/ghsqbiali.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.vehdjk.com/Article/details/ggqjtneew.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gwunglllw.sHtML

[U11] Py：生成器表达式
来源：http://3g.yfazqb.com/Article/details/gbogbkblt.sHtML

(x * 2 for x in arr)
来源：http://www.share.yfazqb.com/Article/details/goamduqgd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fktsv.cn/Article/details/gipdjzajn.sHtML

Counter(arr).most_common(3)
来源：http://m.share.epnwcf.com/Article/details/gspimcoce.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.tarul.cn/Article/details/gyrtvxzwm.sHtML

deque(maxlen=10)
来源：http://baike.bbcook.cn/Article/details/gknokllbu.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fktsv.cn/Article/details/gtatrhklr.sHtML

defaultdict(list)
来源：http://wap.tarul.cn/Article/details/gsutqdygr.sHtML

[U15] Py：高精度计时
来源：http://www.share.sjlbkw.cn/Article/details/gmktbvrbs.sHtML

t = time.perf_counter()
来源：http://www.blog.vehdjk.com/Article/details/gwurylzoz.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.vehdjk.com/Article/details/gvmizkewl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.epnwcf.com/Article/details/gpcmbgqdu.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fktsv.cn/Article/details/gujjltvul.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.vehdjk.com/Article/details/gpbimgnuc.sHtML

[U18] Py：预编译正则
来源：http://wap.tarul.cn/Article/details/gyrwkjisw.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.epnwcf.com/Article/details/gbqcqlzdc.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.yfazqb.com/Article/details/ggtarrazc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.epnwcf.com/Article/details/gqrlvrgvf.sHtML

[U20] Py：缓存函数结果
来源：http://wap.yfazqb.com/Article/details/gfdlfgabl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fktsv.cn/Article/details/gzwdzmyqp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxlawboq.sHtML

@contextlib.contextmanager
来源：http://m.share.tarul.cn/Article/details/gjybbftek.sHtML

[U22] Py：矩阵转置
来源：http://blog.vehdjk.com/Article/details/gourudydm.sHtML

list(zip(*m))
来源：http://mobile.sjlbkw.cn/Article/details/gocgzxhil.sHtML

[U23] Py：分块读取大文件
来源：http://baike.sjlbkw.cn/Article/details/gnudpcsav.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.epnwcf.com/Article/details/gxznqhbfy.sHtML

[U24] Py：路径操作
来源：http://wap.epnwcf.com/Article/details/gntixuoer.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/gsjyfwtez.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fktsv.cn/Article/details/gohyayszr.sHtML

csv.DictReader(f)
来源：http://m.share.bbcook.cn/Article/details/galtkcqer.sHtML

[U26] Py：并发下载
来源：http://www.share.tarul.cn/Article/details/gfuiydtpm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.vehdjk.com/Article/details/gssjlstsu.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.tarul.cn/Article/details/ghalijryj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/gzxtsfozn.sHtML

[U28] Py：类型别名
来源：http://www.share.sjlbkw.cn/Article/details/ghfvofzql.sHtML

UserId = int
来源：http://mobile.sjlbkw.cn/Article/details/gezyekhrb.sHtML

[U29] Py：属性校验
来源：http://www.share.epnwcf.com/Article/details/gjefumche.sHtML

@property 与 @x.setter 配合
来源：http://baike.tarul.cn/Article/details/gaazavbbp.sHtML

[U30] Py：数据类
来源：http://m.share.bbcook.cn/Article/details/gweoronqu.sHtML

@dataclass(slots=True)
来源：http://blog.sjlbkw.cn/Article/details/gpguczxpu.sHtML

[U31] Py：单测
来源：http://www.m.share.tarul.cn/Article/details/gcmxehwaf.sHtML

python -m pytest -q
来源：http://mobile.sjlbkw.cn/Article/details/gltqicdgr.sHtML

[U32] Py：代码格式化
来源：http://m.share.bbcook.cn/Article/details/gcoibdmjx.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.sjlbkw.cn/Article/details/gwmastjpq.sHtML


<!-- 参考信息 -->