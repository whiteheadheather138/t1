代发 wailian999

strlen(s)
来源：http://wap.yfazqb.com/Article/details/gablsximj.sHtML

[S06] C：字符串比较
来源：http://mobile.fktsv.cn/Article/details/gjseusjfj.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gkyuzdyez.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gliwhdvsq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/gqeozszqm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/gehefslfo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.epnwcf.com/Article/details/grwkochle.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.yfazqb.com/Article/details/gefyaxlhh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.tarul.cn/Article/details/gzzqwjxod.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gzfcdcefg.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.bbcook.cn/Article/details/gpitvqnkf.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gudmxqpkq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fktsv.cn/Article/details/gufuhctdk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.bbcook.cn/Article/details/gbflxamdj.sHtML

fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gfhctkmmi.sHtML

[S12] C：写文件
来源：http://wap.bbcook.cn/Article/details/gkhvqnjoc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gkzbgztkw.sHtML

[S13] C：宏定义
来源：http://www.blog.epnwcf.com/Article/details/ggoegjqpb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/gevqxrbdi.sHtML

[S14] C：枚举
来源：http://blog.yfazqb.com/Article/details/grvewyula.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.epnwcf.com/Article/details/gtumfkifz.sHtML

[S15] C：类型转换
来源：http://m.share.sjlbkw.cn/Article/details/gbwhhrhzl.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/gknoomcor.sHtML

[S16] C：位操作置位
来源：http://blog.epnwcf.com/Article/details/ghoybkosp.sHtML

x |= (1 << 3);
来源：http://www.m.share.fktsv.cn/Article/details/guetcnzhl.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.tarul.cn/Article/details/gxmefpbep.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.yfazqb.com/Article/details/guguqmejw.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/gikzwnruc.sHtML

int main(int argc, char **argv)
来源：http://blog.fktsv.cn/Article/details/gcagjuwhs.sHtML

[S19] C：快速排序
来源：http://3g.yfazqb.com/Article/details/gmyemhzcg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/glwcgwbfr.sHtML

[S20] C：二分查找
来源：http://wap.bbcook.cn/Article/details/glrzmnspv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gkbdiipae.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gavwuitgg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fktsv.cn/Article/details/gekxzxtkk.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/gevftyjxa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fktsv.cn/Article/details/glurmqvqd.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gmtvgesvu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.vehdjk.com/Article/details/gkcfkrwuh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/gwpvhvoaw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.yfazqb.com/Article/details/gzulqpmzj.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gynuwadui.sHtML

memcpy(dst, src, n);
来源：http://baike.sjlbkw.cn/Article/details/gojphceya.sHtML

[S26] C：内存清零
来源：http://read.share.tarul.cn/Article/details/gqqyxqejr.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.tarul.cn/Article/details/gbfovtwnp.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/ganuupzpn.sHtML

const double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gvlnykmhm.sHtML

[S28] C：静态变量
来源：http://baike.yfazqb.com/Article/details/gdidwpbzo.sHtML

static int counter = 0;
来源：http://www.share.fktsv.cn/Article/details/gioiopprk.sHtML

[S29] C：变参函数
来源：http://mobile.sjlbkw.cn/Article/details/gypdvcwue.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.yfazqb.com/Article/details/glfqhwtqe.sHtML

[S30] C：头文件保护
来源：http://www.m.share.tarul.cn/Article/details/gunzbovib.sHtML

#ifndef X_H
来源：http://www.blog.sjlbkw.cn/Article/details/geynjhubm.sHtML

#define X_H
来源：http://www.m.share.vehdjk.com/Article/details/gmwhazril.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/gvczhmjkb.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/gmerqgdxk.sHtML

#include <iostream>
来源：http://m.share.bbcook.cn/Article/details/gqhyjtklz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/gonfncjoq.sHtML

[S32] C++：字符串
来源：http://3g.fktsv.cn/Article/details/gyucxrput.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.yfazqb.com/Article/details/gbspfynfy.sHtML

[S33] C++：vector 增删
来源：http://wap.sjlbkw.cn/Article/details/gydzjinhf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.sjlbkw.cn/Article/details/glfzfqyoq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.yfazqb.com/Article/details/gbyeypfwc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fktsv.cn/Article/details/ghdxmotwr.sHtML

[S35] C++：map
来源：http://www.blog.fktsv.cn/Article/details/gsxcpauub.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/ghqahtayt.sHtML

[S36] C++：unordered_map
来源：http://www.share.sjlbkw.cn/Article/details/gqzvtoemr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gzrqumylo.sHtML

[S37] C++：set
来源：http://3g.fktsv.cn/Article/details/glqlmrdas.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.epnwcf.com/Article/details/ggffpmqlt.sHtML

[S38] C++：排序
来源：http://wap.bbcook.cn/Article/details/gasrvamce.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gwylmirmn.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.sjlbkw.cn/Article/details/gccxnkzxq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/gfnenkdwv.sHtML

[S40] C++：查找元素
来源：http://mobile.yfazqb.com/Article/details/ggyqngiab.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/gkuqwqjkx.sHtML

[S41] C++：类与构造函数
来源：http://3g.tarul.cn/Article/details/gkxqbphcd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.bbcook.cn/Article/details/gmzriihex.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gvmuyigkd.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.epnwcf.com/Article/details/gxsdmkgna.sHtML

[S43] C++：智能指针
来源：http://blog.vehdjk.com/Article/details/gpjbccrnf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.bbcook.cn/Article/details/gzspuncfg.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/gclhuravk.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/gzgljkslg.sHtML

[S45] C++：lambda
来源：http://www.share.tarul.cn/Article/details/gpeknqjuy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.bbcook.cn/Article/details/ghsvittzh.sHtML

[S46] C++：函数模板
来源：http://3g.tarul.cn/Article/details/goaryzuag.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/gyuiojnsp.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.sjlbkw.cn/Article/details/gvcochrvm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/grczogyfw.sHtML

[S48] C++：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gyvkebccc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gjgjkkhvr.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.tarul.cn/Article/details/gpomlctic.sHtML

[S49] C++：写文件
来源：http://wap.tarul.cn/Article/details/gpjysdkpb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.yfazqb.com/Article/details/gfabikgua.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gigtswrzc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gaaokkcpq.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/gedrvqmrr.sHtML

static_cast<double>(a) / b
来源：http://blog.tarul.cn/Article/details/gbuuvtpld.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gjggbzxng.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/gstwqxbcr.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/guqirrydk.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.bbcook.cn/Article/details/gvbepxgeu.sHtML

[S54] C++：异常处理
来源：http://www.m.share.yfazqb.com/Article/details/gkretuvdh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/gvanunyui.sHtML

[S55] C++：结构化绑定
来源：http://read.share.yfazqb.com/Article/details/gpdwysjcr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.vehdjk.com/Article/details/gxttexvdu.sHtML

[S56] C++：optional
来源：http://baike.epnwcf.com/Article/details/gykgsizkf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/ggnsdcbmg.sHtML

[S57] C++：编译期常量
来源：http://www.share.vehdjk.com/Article/details/glvcqatyq.sHtML

constexpr int N = 10;
来源：http://www.share.bbcook.cn/Article/details/gdrnlwvei.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gzrobaabr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.sjlbkw.cn/Article/details/ghpjlogct.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/geqjqmxdw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/gjagaztib.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.tarul.cn/Article/details/glaqncone.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.vehdjk.com/Article/details/gxysogjch.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gygcnhwtd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gxazwfvfw.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwjkxlsvb.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gixjwdtwc.sHtML

println("Hello")
来源：http://wap.tarul.cn/Article/details/gdzslabjj.sHtML

[T02] Kotlin：变量
来源：http://3g.yfazqb.com/Article/details/gizeyfiwu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.yfazqb.com/Article/details/ghbkvuwth.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/gxxhcizbj.sHtML

"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/getlgytst.sHtML

[T04] Kotlin：空安全
来源：http://wap.tarul.cn/Article/details/gwiqdebfz.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fktsv.cn/Article/details/gudckkspk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.vehdjk.com/Article/details/gitvzvpfl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/gsqjjukje.sHtML

[T06] Kotlin：集合映射
来源：http://3g.epnwcf.com/Article/details/gkerkndix.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gwmyushjg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/glvxenoyd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/gfrghaarh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.sjlbkw.cn/Article/details/genbntozh.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.sjlbkw.cn/Article/details/gvpnznylg.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.vehdjk.com/Article/details/gcufyewnv.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.tarul.cn/Article/details/gqfrqmhas.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.tarul.cn/Article/details/gmyniodvb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.vehdjk.com/Article/details/gbwrpmqrr.sHtML

[T11] Kotlin：协程
来源：http://mobile.epnwcf.com/Article/details/gwuxnajcu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.yfazqb.com/Article/details/ghhcfyiky.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.yfazqb.com/Article/details/gdzmdndlx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/girwfmgzy.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/gbyijbuol.sHtML

val m = mapOf("a" to 1)
来源：http://3g.epnwcf.com/Article/details/gqnhtukbq.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gykftkljo.sHtML

for (i in 1..10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gzhtjlisd.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/gfpasoiuq.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.sjlbkw.cn/Article/details/gqdrwmfzr.sHtML

[T16] Swift：Hello World
来源：http://read.share.fktsv.cn/Article/details/goxdmsfgs.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gqwkofjpx.sHtML

[T17] Swift：变量与常量
来源：http://read.share.epnwcf.com/Article/details/gcowwuapx.sHtML

var a = 1;  let b = 2
来源：http://mobile.epnwcf.com/Article/details/gapwioefa.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gqvffskji.sHtML

"值: \(b)"
来源：http://www.share.bbcook.cn/Article/details/gtehnjihd.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjweklrw.sHtML

if let n = opt { print(n) }
来源：http://blog.vehdjk.com/Article/details/gjhfyvwkn.sHtML

[T20] Swift：数组操作
来源：http://m.share.vehdjk.com/Article/details/gwmwxpbvo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.bbcook.cn/Article/details/gtpxiduqr.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/gbuivvvfx.sHtML

for x in a { print(x) }
来源：http://www.share.sjlbkw.cn/Article/details/grzqkpxrt.sHtML

[T22] Swift：字典
来源：http://read.share.epnwcf.com/Article/details/gwlykknox.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.vehdjk.com/Article/details/gyvqfdgwz.sHtML

[T23] Swift：函数
来源：http://blog.bbcook.cn/Article/details/gmuzndgkr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.vehdjk.com/Article/details/gqgmdigzo.sHtML

[T24] Swift：闭包
来源：http://wap.bbcook.cn/Article/details/gkurnizcn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fktsv.cn/Article/details/gfwapwuea.sHtML

[T25] Swift：结构体
来源：http://3g.vehdjk.com/Article/details/gfabyghaz.sHtML

struct P { var x: Int }
来源：http://mobile.yfazqb.com/Article/details/gougxdxon.sHtML

[T26] Swift：类与重写
来源：http://read.share.vehdjk.com/Article/details/grwarazsf.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.vehdjk.com/Article/details/gashsoxbv.sHtML

[T27] Swift：错误处理
来源：http://blog.epnwcf.com/Article/details/goscitltb.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.vehdjk.com/Article/details/gcvcpjujp.sHtML

[T28] Swift：枚举
来源：http://baike.sjlbkw.cn/Article/details/gxyomokzb.sHtML

enum Color { case red, green }
来源：http://baike.bbcook.cn/Article/details/gbnxiipza.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fktsv.cn/Article/details/gnoywvjbf.sHtML

guard let x = opt else { return }
来源：http://wap.bbcook.cn/Article/details/gzailkzeo.sHtML

[T30] Swift：协议
来源：http://www.m.share.yfazqb.com/Article/details/grkcwpopr.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.vehdjk.com/Article/details/gvzngvbpw.sHtML

[T31] Lua：Hello World
来源：http://read.share.fktsv.cn/Article/details/gpydcbkzg.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gojotgyih.sHtML

[T32] Lua：局部变量
来源：http://baike.epnwcf.com/Article/details/grdktoxpl.sHtML

local a = 1
来源：http://3g.fktsv.cn/Article/details/gvonghjut.sHtML

[T33] Lua：表（数组）
来源：http://3g.yfazqb.com/Article/details/gktptpqst.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.tarul.cn/Article/details/gdkrbyciq.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.tarul.cn/Article/details/gqwotoakb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/gkdiqggvd.sHtML

[T35] Lua：字典表
来源：http://baike.sjlbkw.cn/Article/details/gmscnxake.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gskkfqnew.sHtML

[T36] Lua：函数
来源：http://m.share.sjlbkw.cn/Article/details/gtgefplfj.sHtML

function add(a, b) return a + b end
来源：http://www.blog.tarul.cn/Article/details/ggxfzxcmy.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.tarul.cn/Article/details/gywbiukcv.sHtML

"a" .. "b"
来源：http://mobile.tarul.cn/Article/details/gtjtdqniv.sHtML

[T38] Lua：条件
来源：http://www.blog.sjlbkw.cn/Article/details/ghuebqfia.sHtML

if x > 0 then print("正") end
来源：http://baike.epnwcf.com/Article/details/gubabavcv.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/glnnwzlsx.sHtML

string.find(s, "%d+")
来源：http://m.share.bbcook.cn/Article/details/glmouzflt.sHtML

[T40] Lua：元表
来源：http://m.share.epnwcf.com/Article/details/gmonswygk.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.yfazqb.com/Article/details/gyagxfuhw.sHtML

[T41] Perl：Hello World
来源：http://mobile.tarul.cn/Article/details/gjmddskid.sHtML

print "Hello\n";
来源：http://read.share.fktsv.cn/Article/details/gethurtmj.sHtML

[T42] Perl：变量类型
来源：http://wap.sjlbkw.cn/Article/details/giatvpmlc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.tarul.cn/Article/details/gnoosukxd.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfpwjxzg.sHtML

"值: $a"
来源：http://read.share.fktsv.cn/Article/details/gkyexpjvj.sHtML

[T44] Perl：条件
来源：http://www.share.fktsv.cn/Article/details/gplmeoaof.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.epnwcf.com/Article/details/gtdsglzqy.sHtML

[T45] Perl：数组遍历
来源：http://blog.sjlbkw.cn/Article/details/gsffzjdkb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.yfazqb.com/Article/details/gpfmawrbv.sHtML

[T46] Perl：哈希操作
来源：http://mobile.yfazqb.com/Article/details/gpxwhpowk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/gqjauritb.sHtML

[T47] Perl：正则捕获
来源：http://www.share.tarul.cn/Article/details/gvhrmhsir.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fktsv.cn/Article/details/gucdcuvnn.sHtML

[T48] Perl：正则替换
来源：http://wap.fktsv.cn/Article/details/gxemlmowd.sHtML

$s =~ s/old/new/g;
来源：http://m.share.tarul.cn/Article/details/gfcetdhsv.sHtML

[T49] Perl：函数
来源：http://www.m.share.vehdjk.com/Article/details/gacfeohpj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gqjuizuip.sHtML

[T50] Perl：逐行读文件
来源：http://wap.epnwcf.com/Article/details/glxahrkrv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyepdebq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/guqfocmzq.sHtML

[T51] Scala：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/grvlbukyf.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gojcibkid.sHtML

[T52] Scala：变量
来源：http://mobile.vehdjk.com/Article/details/gqoirjwuz.sHtML

val a = 1;  var b = 2
来源：http://mobile.epnwcf.com/Article/details/gupsgpvdc.sHtML

[T53] Scala：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gnydrklwk.sHtML

s"值: $b"
来源：http://3g.bbcook.cn/Article/details/gcsxmddle.sHtML

[T54] Scala：集合映射
来源：http://www.blog.tarul.cn/Article/details/gijpfwlui.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.vehdjk.com/Article/details/gohqlelui.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gnqwactmz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fktsv.cn/Article/details/gtakgclra.sHtML

[T56] Scala：样例类
来源：http://read.share.fktsv.cn/Article/details/gzlrbliqg.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fktsv.cn/Article/details/glefbxjxf.sHtML

[T57] Scala：模式匹配
来源：http://blog.fktsv.cn/Article/details/ghwdgktej.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.sjlbkw.cn/Article/details/gqwewenez.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/gvuukznfq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.sjlbkw.cn/Article/details/gxoatbyod.sHtML

[T59] Scala：循环
来源：http://blog.sjlbkw.cn/Article/details/gvctpelcm.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.vehdjk.com/Article/details/gkdorbfbe.sHtML

[T60] Scala：折叠
来源：http://mobile.yfazqb.com/Article/details/ghkgmslzz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.vehdjk.com/Article/details/gepiyjypc.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdufxgdck.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/gobmotoom.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gdwuuxszy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.sjlbkw.cn/Article/details/gosvxbtll.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.vehdjk.com/Article/details/gicokswbg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/ghnhdmdpb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.tarul.cn/Article/details/giirhkfcx.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.tarul.cn/Article/details/gsxhxeleq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.epnwcf.com/Article/details/gyhmbpdgt.sHtML

[U04] Py：变量调试打印
来源：http://m.share.tarul.cn/Article/details/gsitwglmy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.tarul.cn/Article/details/gvbvbqtay.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.epnwcf.com/Article/details/goadaaoft.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gyaftilly.sHtML

[U06] Py：合并两个字典
来源：http://baike.vehdjk.com/Article/details/gqbsfzzje.sHtML

{**a, **b}
来源：http://mobile.vehdjk.com/Article/details/gjzedlzpz.sHtML

[U07] Py：反转字典键值
来源：http://3g.epnwcf.com/Article/details/glesswuss.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/ghwppuujv.sHtML

[U08] Py：展平二维列表
来源：http://3g.yfazqb.com/Article/details/gsnlzbrrt.sHtML

[y for x in nested for y in x]
来源：http://www.share.fktsv.cn/Article/details/gaonfbcjj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.vehdjk.com/Article/details/gsbbyikmv.sHtML

max(d, key=d.get)
来源：http://www.share.yfazqb.com/Article/details/goyhhityo.sHtML

[U10] Py：按值排序字典
来源：http://3g.fktsv.cn/Article/details/gtteqnuyy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.tarul.cn/Article/details/gsnquzdau.sHtML

[U11] Py：生成器表达式
来源：http://www.share.bbcook.cn/Article/details/gnpiajrcb.sHtML

(x * 2 for x in arr)
来源：http://3g.fktsv.cn/Article/details/gmieswvsy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.bbcook.cn/Article/details/gtioswtwr.sHtML

Counter(arr).most_common(3)
来源：http://3g.epnwcf.com/Article/details/guvbowivo.sHtML

[U13] Py：固定长度队列
来源：http://www.share.yfazqb.com/Article/details/gmtqbwisw.sHtML

deque(maxlen=10)
来源：http://www.blog.sjlbkw.cn/Article/details/gefffkkce.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.tarul.cn/Article/details/gotdbpsrg.sHtML

defaultdict(list)
来源：http://www.blog.fktsv.cn/Article/details/gdrrmcslm.sHtML

[U15] Py：高精度计时
来源：http://read.share.fktsv.cn/Article/details/gxbopgxkl.sHtML

t = time.perf_counter()
来源：http://www.share.bbcook.cn/Article/details/gtietrrgo.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.bbcook.cn/Article/details/gsplusafh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.bbcook.cn/Article/details/gcznlvddm.sHtML

[U17] Py：初始化日志
来源：http://wap.epnwcf.com/Article/details/gmkhlrthk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.bbcook.cn/Article/details/glugufwlr.sHtML

[U18] Py：预编译正则
来源：http://wap.vehdjk.com/Article/details/gyfdvgmny.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.vehdjk.com/Article/details/glfzajjxj.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.epnwcf.com/Article/details/gdtgjeopp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.vehdjk.com/Article/details/gitcukpqh.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/gxdplfren.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.sjlbkw.cn/Article/details/gdmtzugdh.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.tarul.cn/Article/details/gahfheyus.sHtML

@contextlib.contextmanager
来源：http://baike.tarul.cn/Article/details/gwdkeucbn.sHtML

[U22] Py：矩阵转置
来源：http://baike.yfazqb.com/Article/details/gcszsqxvi.sHtML

list(zip(*m))
来源：http://baike.epnwcf.com/Article/details/geiavfhlt.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.yfazqb.com/Article/details/gsozrjnee.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.sjlbkw.cn/Article/details/ghfnibhdo.sHtML

[U24] Py：路径操作
来源：http://wap.tarul.cn/Article/details/gwnxiahjz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gbiroepap.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.bbcook.cn/Article/details/ggdxkshcv.sHtML

csv.DictReader(f)
来源：http://m.share.vehdjk.com/Article/details/gvxvrktbz.sHtML

[U26] Py：并发下载
来源：http://www.m.share.sjlbkw.cn/Article/details/gccxyihvj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.vehdjk.com/Article/details/grvgffhpi.sHtML

[U27] Py：异步 HTTP
来源：http://3g.tarul.cn/Article/details/glufgvyoo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.vehdjk.com/Article/details/gkrhmmeir.sHtML

[U28] Py：类型别名
来源：http://baike.fktsv.cn/Article/details/gefvhmjrz.sHtML

UserId = int
来源：http://3g.epnwcf.com/Article/details/gszyrykgc.sHtML


<!-- 参考信息 -->