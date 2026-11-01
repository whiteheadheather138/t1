代发 wailian999

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/guqtczqqe.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/gnbbsniny.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/grdplpwlv.sHtML

[S07] C：数组遍历求和
来源：http://read.share.yfazqb.com/Article/details/ghkucztan.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.bbcook.cn/Article/details/gnbedurie.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.yfazqb.com/Article/details/gmohsojgd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.sjlbkw.cn/Article/details/gqatkizbe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/gvzdywxez.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.vehdjk.com/Article/details/ggzklsxxn.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/glesbbjwi.sHtML

int *p = &a;  *p = 5;
来源：http://baike.vehdjk.com/Article/details/gcorpskvy.sHtML

[S11] C：逐行读文件
来源：http://baike.tarul.cn/Article/details/gwetvyphy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.yfazqb.com/Article/details/gtdqxbuhr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/gdzrimpkx.sHtML

fclose(f);
来源：http://blog.yfazqb.com/Article/details/gqqusmezp.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/ggbubltuu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gezohhwmh.sHtML

[S13] C：宏定义
来源：http://www.blog.epnwcf.com/Article/details/gtigzdpng.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmncysyo.sHtML

[S14] C：枚举
来源：http://read.share.vehdjk.com/Article/details/gwmstonhh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.vehdjk.com/Article/details/gwbkiyorn.sHtML

[S15] C：类型转换
来源：http://baike.fktsv.cn/Article/details/gxkewrhoh.sHtML

(double) a / b
来源：http://read.share.fktsv.cn/Article/details/gwdfvtplc.sHtML

[S16] C：位操作置位
来源：http://read.share.tarul.cn/Article/details/gbmarmejv.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/gllfxncul.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gpgqeuzhj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.tarul.cn/Article/details/ghhwkxmcc.sHtML

[S18] C：命令行参数
来源：http://blog.vehdjk.com/Article/details/gxebwhvyv.sHtML

int main(int argc, char **argv)
来源：http://mobile.sjlbkw.cn/Article/details/gqhalaaeu.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/glgpydkje.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gtzfjahog.sHtML

[S20] C：二分查找
来源：http://www.m.share.fktsv.cn/Article/details/gjhubvplj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/ghrnueics.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/gadjdsvqf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.yfazqb.com/Article/details/gmelrukuq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/gjkdofrap.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/gpnopmniw.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/gkinmpqdg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.yfazqb.com/Article/details/guaunwlan.sHtML

[S24] C：获取本地时间
来源：http://www.blog.vehdjk.com/Article/details/gwaxuwrea.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/gqdljwdko.sHtML

[S25] C：内存拷贝
来源：http://www.blog.tarul.cn/Article/details/glayqphew.sHtML

memcpy(dst, src, n);
来源：http://baike.bbcook.cn/Article/details/guivohfbp.sHtML

[S26] C：内存清零
来源：http://wap.vehdjk.com/Article/details/gqjyaserc.sHtML

memset(a, 0, sizeof a);
来源：http://3g.vehdjk.com/Article/details/glprwgqki.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/gwwesjlpm.sHtML

const double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/ggwdeoarj.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/geveaivrz.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gojcxayio.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/gzpkwlgkd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/gmdccmssv.sHtML

[S30] C：头文件保护
来源：http://mobile.vehdjk.com/Article/details/grqzorceb.sHtML

#ifndef X_H
来源：http://mobile.vehdjk.com/Article/details/ginloaihn.sHtML

#define X_H
来源：http://mobile.fktsv.cn/Article/details/goiypgblq.sHtML

#endif
来源：http://read.share.sjlbkw.cn/Article/details/gwvsgbuif.sHtML

[S31] C++：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gclnxzwsi.sHtML

#include <iostream>
来源：http://www.m.share.bbcook.cn/Article/details/gqukeadcg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.epnwcf.com/Article/details/gvfxgwiga.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/gekliqdvu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.tarul.cn/Article/details/gwlaklwkh.sHtML

[S33] C++：vector 增删
来源：http://www.blog.bbcook.cn/Article/details/gumtcbpru.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.bbcook.cn/Article/details/gcqikqhii.sHtML

[S34] C++：遍历 vector
来源：http://www.share.sjlbkw.cn/Article/details/gezenwnlf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/gdegynqga.sHtML

[S35] C++：map
来源：http://3g.tarul.cn/Article/details/gcoglalmm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/giwmmfdyy.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/gpwgvcgsk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gmrqroovr.sHtML

[S37] C++：set
来源：http://www.share.epnwcf.com/Article/details/gjsxrhtpt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.yfazqb.com/Article/details/gefdxawss.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/gmrcbrojy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gtdubzdmf.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gpqilxzzd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhbirwcb.sHtML

[S40] C++：查找元素
来源：http://blog.sjlbkw.cn/Article/details/gqkjvxdqt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.yfazqb.com/Article/details/gyjgrzrlp.sHtML

[S41] C++：类与构造函数
来源：http://www.share.tarul.cn/Article/details/gxliisxkf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fktsv.cn/Article/details/gtzvoubpl.sHtML

[S42] C++：继承与虚函数
来源：http://wap.bbcook.cn/Article/details/gtwzzaund.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.epnwcf.com/Article/details/gdckzjczw.sHtML

[S43] C++：智能指针
来源：http://baike.vehdjk.com/Article/details/giqksbgez.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.tarul.cn/Article/details/gkhlpatfo.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/gqyfpjmeg.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fktsv.cn/Article/details/govwuukex.sHtML

[S45] C++：lambda
来源：http://blog.epnwcf.com/Article/details/gewhtcvsi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.vehdjk.com/Article/details/gpgyfmguu.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/glgfayknf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.bbcook.cn/Article/details/gwcrhaiyy.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.bbcook.cn/Article/details/ganwhvfug.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.bbcook.cn/Article/details/gbkjflslp.sHtML

[S48] C++：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gxtcdhfqj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.tarul.cn/Article/details/gzitioeos.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fktsv.cn/Article/details/gxbuvcoac.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/gsznpwcxr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/gredrpolv.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/gbgxooadi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gpjgiuuel.sHtML

[S51] C++：显式类型转换
来源：http://baike.tarul.cn/Article/details/gxzqexeug.sHtML

static_cast<double>(a) / b
来源：http://baike.vehdjk.com/Article/details/gqzhbbkpp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/gddnwkelv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.bbcook.cn/Article/details/gmoeyozdh.sHtML

[S53] C++：移动语义
来源：http://m.share.sjlbkw.cn/Article/details/gqpnxnesh.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.epnwcf.com/Article/details/gpwbxmikd.sHtML

[S54] C++：异常处理
来源：http://wap.vehdjk.com/Article/details/gxshftvlm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fktsv.cn/Article/details/gsnbugqsc.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fktsv.cn/Article/details/grdiohwcd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.yfazqb.com/Article/details/gfvpfztul.sHtML

[S56] C++：optional
来源：http://www.share.sjlbkw.cn/Article/details/gjncbpiam.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.vehdjk.com/Article/details/geomvamvb.sHtML

[S57] C++：编译期常量
来源：http://blog.epnwcf.com/Article/details/ghgxvktid.sHtML

constexpr int N = 10;
来源：http://blog.vehdjk.com/Article/details/gcakpvivd.sHtML

[S58] C++：命名空间
来源：http://3g.yfazqb.com/Article/details/ggvxszxts.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.yfazqb.com/Article/details/gpequixxf.sHtML

[S59] C++：静态断言
来源：http://www.blog.tarul.cn/Article/details/gteojjugx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.vehdjk.com/Article/details/gmlhbczeq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.bbcook.cn/Article/details/gdznriiml.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.bbcook.cn/Article/details/grapboknp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gggpuprtq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gjhcxcbga.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxivcfnzq.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/gugxwzego.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gstzrtevp.sHtML

[T02] Kotlin：变量
来源：http://www.share.epnwcf.com/Article/details/gydkfxkjd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.yfazqb.com/Article/details/gwyggcwwx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.yfazqb.com/Article/details/gtuyvcxfk.sHtML

"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gpqlhwcxw.sHtML

[T04] Kotlin：空安全
来源：http://wap.sjlbkw.cn/Article/details/gtbvguwhf.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fktsv.cn/Article/details/ggdtdjxpf.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.sjlbkw.cn/Article/details/guaxpamsm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.tarul.cn/Article/details/geaojvrvw.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.vehdjk.com/Article/details/gtaccsxal.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.yfazqb.com/Article/details/ghldxucjj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.vehdjk.com/Article/details/gkfxgdunb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.epnwcf.com/Article/details/gvnthhkve.sHtML

[T08] Kotlin：数据类
来源：http://www.share.tarul.cn/Article/details/ghsaeokgb.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.tarul.cn/Article/details/gkpjiaxwq.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.tarul.cn/Article/details/gqgbwsdeq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fktsv.cn/Article/details/gixmedzsa.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fktsv.cn/Article/details/gxrsekxnx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.vehdjk.com/Article/details/gxrzeztpt.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/guvpbigcd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.yfazqb.com/Article/details/gurmekezu.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/gpylaxzqv.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gxsxyohqs.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/gqsugxtio.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.yfazqb.com/Article/details/gakutpedu.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gajpylpso.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/gjbztzyhs.sHtML

[T15] Kotlin：接口
来源：http://m.share.tarul.cn/Article/details/grxydkxjn.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.epnwcf.com/Article/details/gsmpkhihu.sHtML

[T16] Swift：Hello World
来源：http://www.share.vehdjk.com/Article/details/glarhsebf.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/gdslyhdqn.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.bbcook.cn/Article/details/ggwjnwufn.sHtML

var a = 1;  let b = 2
来源：http://3g.tarul.cn/Article/details/gdwxrtibc.sHtML

[T18] Swift：字符串插值
来源：http://blog.yfazqb.com/Article/details/gxeqltsjt.sHtML

"值: \(b)"
来源：http://www.blog.tarul.cn/Article/details/gydmevozm.sHtML

[T19] Swift：可选绑定
来源：http://mobile.yfazqb.com/Article/details/gpxotvqbz.sHtML

if let n = opt { print(n) }
来源：http://3g.epnwcf.com/Article/details/grhakknyj.sHtML

[T20] Swift：数组操作
来源：http://mobile.fktsv.cn/Article/details/gpcccgpgz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fktsv.cn/Article/details/gxhtwmjig.sHtML

[T21] Swift：遍历
来源：http://read.share.tarul.cn/Article/details/gtabxaayo.sHtML

for x in a { print(x) }
来源：http://www.blog.tarul.cn/Article/details/gsclguzzf.sHtML

[T22] Swift：字典
来源：http://www.m.share.tarul.cn/Article/details/glpevzypb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.bbcook.cn/Article/details/gytnisoaa.sHtML

[T23] Swift：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gssgyjutu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpvksnca.sHtML

[T24] Swift：闭包
来源：http://wap.fktsv.cn/Article/details/gopujgdms.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gtyasrbfs.sHtML

[T25] Swift：结构体
来源：http://m.share.bbcook.cn/Article/details/gtjaissdx.sHtML

struct P { var x: Int }
来源：http://www.share.bbcook.cn/Article/details/gfplqzquw.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/guhdopzqr.sHtML

class A: Base { override func f() {} }
来源：http://mobile.tarul.cn/Article/details/gsyobunnw.sHtML

[T27] Swift：错误处理
来源：http://baike.vehdjk.com/Article/details/gswkrpaeq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.tarul.cn/Article/details/gvivxzadk.sHtML

[T28] Swift：枚举
来源：http://wap.vehdjk.com/Article/details/gfcmiirfk.sHtML

enum Color { case red, green }
来源：http://www.share.vehdjk.com/Article/details/gcbijckbn.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.epnwcf.com/Article/details/gadxsoodp.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gwmnpanwe.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/gyaatymlm.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.yfazqb.com/Article/details/gkgaedirm.sHtML

[T31] Lua：Hello World
来源：http://mobile.tarul.cn/Article/details/glzhezllp.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gubzqmyqo.sHtML

[T32] Lua：局部变量
来源：http://baike.bbcook.cn/Article/details/gkovibyal.sHtML

local a = 1
来源：http://3g.vehdjk.com/Article/details/gpybyzrct.sHtML

[T33] Lua：表（数组）
来源：http://m.share.yfazqb.com/Article/details/giawtejie.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.tarul.cn/Article/details/gnudvdkot.sHtML

[T34] Lua：遍历表
来源：http://www.share.tarul.cn/Article/details/gasbeczod.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.yfazqb.com/Article/details/gyxtogude.sHtML

[T35] Lua：字典表
来源：http://m.share.fktsv.cn/Article/details/gzqfpoins.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.vehdjk.com/Article/details/gfpfgtbgj.sHtML

[T36] Lua：函数
来源：http://blog.yfazqb.com/Article/details/gahowhhcf.sHtML

function add(a, b) return a + b end
来源：http://m.share.yfazqb.com/Article/details/gpbniuvmw.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gnckxffrv.sHtML

"a" .. "b"
来源：http://wap.yfazqb.com/Article/details/gtuytnota.sHtML

[T38] Lua：条件
来源：http://www.m.share.vehdjk.com/Article/details/gapdhjciq.sHtML

if x > 0 then print("正") end
来源：http://blog.vehdjk.com/Article/details/gpcgulfvi.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.tarul.cn/Article/details/gabmmarhj.sHtML

string.find(s, "%d+")
来源：http://www.m.share.vehdjk.com/Article/details/gqfcuosfo.sHtML

[T40] Lua：元表
来源：http://baike.epnwcf.com/Article/details/gydwhuisi.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.tarul.cn/Article/details/gbalpronv.sHtML

[T41] Perl：Hello World
来源：http://m.share.fktsv.cn/Article/details/gbbipccjv.sHtML

print "Hello\n";
来源：http://www.m.share.vehdjk.com/Article/details/geekjuigi.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fktsv.cn/Article/details/gztujwnpx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.vehdjk.com/Article/details/gbpfotgev.sHtML

[T43] Perl：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gjhcymijj.sHtML

"值: $a"
来源：http://www.share.bbcook.cn/Article/details/geediruap.sHtML

[T44] Perl：条件
来源：http://read.share.yfazqb.com/Article/details/gulgsiwsh.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.vehdjk.com/Article/details/gwiwcpefl.sHtML

[T45] Perl：数组遍历
来源：http://blog.tarul.cn/Article/details/gwvrotpwv.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.epnwcf.com/Article/details/garxwxrqa.sHtML

[T46] Perl：哈希操作
来源：http://blog.bbcook.cn/Article/details/gcmddxvzp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/gjqwetdpc.sHtML

[T47] Perl：正则捕获
来源：http://mobile.vehdjk.com/Article/details/ggsukghzd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gldouzvrm.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.epnwcf.com/Article/details/gdshqzoft.sHtML

$s =~ s/old/new/g;
来源：http://baike.epnwcf.com/Article/details/gsowbdqcc.sHtML

[T49] Perl：函数
来源：http://www.m.share.vehdjk.com/Article/details/gzdblihmm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/getnkdpus.sHtML

[T50] Perl：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gjhfawxta.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.epnwcf.com/Article/details/geqltcksu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.vehdjk.com/Article/details/gdfzlzima.sHtML

[T51] Scala：Hello World
来源：http://3g.yfazqb.com/Article/details/gamefuxqi.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gjjmehvby.sHtML

[T52] Scala：变量
来源：http://read.share.epnwcf.com/Article/details/gxhqszzqd.sHtML

val a = 1;  var b = 2
来源：http://baike.sjlbkw.cn/Article/details/ggucvkxof.sHtML

[T53] Scala：字符串插值
来源：http://www.share.tarul.cn/Article/details/gkwwuuvnz.sHtML

s"值: $b"
来源：http://wap.vehdjk.com/Article/details/giqvfuxyi.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/goikkmxbm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.epnwcf.com/Article/details/gufvsnvpe.sHtML

[T55] Scala：集合过滤
来源：http://www.share.vehdjk.com/Article/details/gowwenduj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/gpsrfgnrl.sHtML

[T56] Scala：样例类
来源：http://baike.fktsv.cn/Article/details/gvqzlsyta.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.yfazqb.com/Article/details/ggddvmrtk.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/ghhgbeiwc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.sjlbkw.cn/Article/details/gqjslafju.sHtML

[T58] Scala：函数定义
来源：http://read.share.sjlbkw.cn/Article/details/gehbysxya.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.sjlbkw.cn/Article/details/guichlstb.sHtML

[T59] Scala：循环
来源：http://www.m.share.tarul.cn/Article/details/grxxisnrd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gkawuzfrc.sHtML

[T60] Scala：折叠
来源：http://www.m.share.yfazqb.com/Article/details/gkfrmrkip.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.tarul.cn/Article/details/gpwuqijgo.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtyztnazz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gmknlwkpb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gyijixuuh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fktsv.cn/Article/details/gwsndxsbz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.yfazqb.com/Article/details/gauafkcyj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.tarul.cn/Article/details/gocghglkq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.vehdjk.com/Article/details/gvjnkmvtr.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.vehdjk.com/Article/details/gonihguwp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.bbcook.cn/Article/details/gggxuyeqk.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fktsv.cn/Article/details/gmvszwaly.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.bbcook.cn/Article/details/gkifxsnoc.sHtML

[U05] Py：列表去重且保序
来源：http://blog.sjlbkw.cn/Article/details/gujpnncvb.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/gantllqsd.sHtML

[U06] Py：合并两个字典
来源：http://blog.tarul.cn/Article/details/gvnsqcxmc.sHtML

{**a, **b}
来源：http://3g.fktsv.cn/Article/details/gxgufdgei.sHtML

[U07] Py：反转字典键值
来源：http://read.share.tarul.cn/Article/details/ghduddyzt.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.sjlbkw.cn/Article/details/gubulpniy.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.epnwcf.com/Article/details/gnhsnexdh.sHtML

[y for x in nested for y in x]
来源：http://wap.yfazqb.com/Article/details/gypbjxzns.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.tarul.cn/Article/details/gmwbkbwzk.sHtML

max(d, key=d.get)
来源：http://mobile.sjlbkw.cn/Article/details/gcbtkcqka.sHtML

[U10] Py：按值排序字典
来源：http://blog.epnwcf.com/Article/details/gztmuhmki.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.epnwcf.com/Article/details/gmxmeegmv.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fktsv.cn/Article/details/gpcapxgmx.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.yfazqb.com/Article/details/gtmhvqhcx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.epnwcf.com/Article/details/gdpcnjwig.sHtML

Counter(arr).most_common(3)
来源：http://m.share.epnwcf.com/Article/details/gwomqvvky.sHtML

[U13] Py：固定长度队列
来源：http://baike.bbcook.cn/Article/details/gestdufxa.sHtML

deque(maxlen=10)
来源：http://blog.bbcook.cn/Article/details/gzvhyxcld.sHtML

[U14] Py：分组收集到列表
来源：http://wap.tarul.cn/Article/details/gddjxesjw.sHtML

defaultdict(list)
来源：http://www.blog.epnwcf.com/Article/details/gkgzuqzyz.sHtML

[U15] Py：高精度计时
来源：http://read.share.bbcook.cn/Article/details/gcuqqsjkh.sHtML

t = time.perf_counter()
来源：http://m.share.vehdjk.com/Article/details/gvsaikxtu.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.sjlbkw.cn/Article/details/gmjejdpms.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.vehdjk.com/Article/details/gwgzcpsrw.sHtML

[U17] Py：初始化日志
来源：http://baike.sjlbkw.cn/Article/details/gjkdjhsqk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.epnwcf.com/Article/details/gvathycdl.sHtML

[U18] Py：预编译正则
来源：http://mobile.tarul.cn/Article/details/gsiwqjiiz.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fktsv.cn/Article/details/gcwtehuav.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fktsv.cn/Article/details/gvihcwdfp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fktsv.cn/Article/details/gnhkkbyys.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fktsv.cn/Article/details/gigobighw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.bbcook.cn/Article/details/gntwkqcsx.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.bbcook.cn/Article/details/gruasgpjs.sHtML

@contextlib.contextmanager
来源：http://3g.tarul.cn/Article/details/gbvufojcx.sHtML

[U22] Py：矩阵转置
来源：http://m.share.tarul.cn/Article/details/gdtnyebqm.sHtML

list(zip(*m))
来源：http://read.share.sjlbkw.cn/Article/details/gtaorglox.sHtML

[U23] Py：分块读取大文件
来源：http://blog.bbcook.cn/Article/details/gsapbpzcf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.epnwcf.com/Article/details/gnfnwdels.sHtML

[U24] Py：路径操作
来源：http://read.share.tarul.cn/Article/details/gredkcshk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.yfazqb.com/Article/details/galinibef.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.tarul.cn/Article/details/gyjocmrjj.sHtML

csv.DictReader(f)
来源：http://mobile.epnwcf.com/Article/details/gcjeapitg.sHtML

[U26] Py：并发下载
来源：http://m.share.sjlbkw.cn/Article/details/gmbbcqpnx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.yfazqb.com/Article/details/gzhlmeuwb.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.vehdjk.com/Article/details/gzzbwhcos.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.tarul.cn/Article/details/gxgcdmpmv.sHtML

[U28] Py：类型别名
来源：http://www.share.vehdjk.com/Article/details/gwldjhfjd.sHtML

UserId = int
来源：http://m.share.tarul.cn/Article/details/ghroacxpi.sHtML


<!-- 参考信息 -->