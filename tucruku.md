代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gnhwpyebg.sHtML

[S13] C：宏定义
来源：http://baike.fktsv.cn/Article/details/gcmvjyhxa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.vehdjk.com/Article/details/glgwwpssa.sHtML

[S14] C：枚举
来源：http://3g.tarul.cn/Article/details/gooamavll.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.tarul.cn/Article/details/gudzbhcky.sHtML

[S15] C：类型转换
来源：http://blog.tarul.cn/Article/details/gsshhcgzl.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/gcnbfeelv.sHtML

[S16] C：位操作置位
来源：http://m.share.epnwcf.com/Article/details/gdrhhpjmz.sHtML

x |= (1 << 3);
来源：http://www.share.yfazqb.com/Article/details/gzfyxanwa.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gvbozorxo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.bbcook.cn/Article/details/gcwzyjhmz.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gcvzkqtdw.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fktsv.cn/Article/details/gplkrcfem.sHtML

[S19] C：快速排序
来源：http://wap.epnwcf.com/Article/details/glapthpkq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/glyvbwvhg.sHtML

[S20] C：二分查找
来源：http://wap.fktsv.cn/Article/details/gmvbrncnk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/ggvglxbjq.sHtML

[S21] C：字符类别判断
来源：http://blog.yfazqb.com/Article/details/gdtqwxxsy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.vehdjk.com/Article/details/gwwpjmdwe.sHtML

[S22] C：字符串转数字
来源：http://mobile.yfazqb.com/Article/details/gsjfoyiww.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.epnwcf.com/Article/details/giccitiod.sHtML

[S23] C：随机数
来源：http://baike.vehdjk.com/Article/details/gxhfcyncj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.sjlbkw.cn/Article/details/gzpcaawil.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/ggdcgcvex.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fktsv.cn/Article/details/ggqjieter.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/grzxptnhw.sHtML

memcpy(dst, src, n);
来源：http://www.blog.epnwcf.com/Article/details/glcqhdjqg.sHtML

[S26] C：内存清零
来源：http://www.m.share.sjlbkw.cn/Article/details/gxsnravss.sHtML

memset(a, 0, sizeof a);
来源：http://baike.vehdjk.com/Article/details/gsfluuvhd.sHtML

[S27] C：定义常量
来源：http://www.share.bbcook.cn/Article/details/gofypfmth.sHtML

const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gxqvadpzg.sHtML

[S28] C：静态变量
来源：http://baike.vehdjk.com/Article/details/gvsukkxry.sHtML

static int counter = 0;
来源：http://3g.sjlbkw.cn/Article/details/gbhgppdgf.sHtML

[S29] C：变参函数
来源：http://baike.yfazqb.com/Article/details/gyiktpnnv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.bbcook.cn/Article/details/guiumgnpq.sHtML

[S30] C：头文件保护
来源：http://mobile.epnwcf.com/Article/details/gfifauxqr.sHtML

#ifndef X_H
来源：http://read.share.tarul.cn/Article/details/gjjajxqlv.sHtML

#define X_H
来源：http://m.share.epnwcf.com/Article/details/geelbojzh.sHtML

#endif
来源：http://mobile.tarul.cn/Article/details/gyykahjlv.sHtML

[S31] C++：Hello World
来源：http://baike.tarul.cn/Article/details/gqpdyyypk.sHtML

#include <iostream>
来源：http://m.share.yfazqb.com/Article/details/gzadpvgun.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gesituysi.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/gtlzivchj.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.tarul.cn/Article/details/gqfhwfqpb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.vehdjk.com/Article/details/gefeonvan.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.epnwcf.com/Article/details/ghjagstyz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.vehdjk.com/Article/details/gshguhdzi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.yfazqb.com/Article/details/gnogqoqiy.sHtML

[S35] C++：map
来源：http://blog.fktsv.cn/Article/details/gfxgjdvke.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gxlnkfegk.sHtML

[S36] C++：unordered_map
来源：http://baike.vehdjk.com/Article/details/geuawpwkz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.tarul.cn/Article/details/gsjdyhqck.sHtML

[S37] C++：set
来源：http://mobile.bbcook.cn/Article/details/gxbtwkxks.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.sjlbkw.cn/Article/details/gpjranryg.sHtML

[S38] C++：排序
来源：http://baike.yfazqb.com/Article/details/gssgmzjxa.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.vehdjk.com/Article/details/gvoqjstzn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.sjlbkw.cn/Article/details/gqcnlllcm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.bbcook.cn/Article/details/gsflfjvoz.sHtML

[S40] C++：查找元素
来源：http://read.share.sjlbkw.cn/Article/details/gnhacwtob.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gbzublycy.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fktsv.cn/Article/details/goayofbfh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.vehdjk.com/Article/details/gmmxkdotk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fktsv.cn/Article/details/gskxqyjck.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.vehdjk.com/Article/details/gjfjrbfst.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/gbljnijth.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.bbcook.cn/Article/details/gdcgtsgsh.sHtML

[S44] C++：引用传参
来源：http://3g.vehdjk.com/Article/details/gjvrdfshe.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.vehdjk.com/Article/details/glwbeohio.sHtML

[S45] C++：lambda
来源：http://www.share.fktsv.cn/Article/details/gwxnscbgh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.tarul.cn/Article/details/guijgropc.sHtML

[S46] C++：函数模板
来源：http://mobile.tarul.cn/Article/details/gapexvmba.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/gxdbuoeth.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/grsnaywll.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/gletecrbu.sHtML

[S48] C++：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gsieghxul.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.epnwcf.com/Article/details/gwiewjezw.sHtML

while (std::getline(in, line)) { }
来源：http://baike.yfazqb.com/Article/details/gwhohbgmt.sHtML

[S49] C++：写文件
来源：http://mobile.yfazqb.com/Article/details/gxtmaxcjz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fktsv.cn/Article/details/gwwhqjukr.sHtML

[S50] C++：格式化数字
来源：http://mobile.sjlbkw.cn/Article/details/gktogbjnj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fktsv.cn/Article/details/gmqksgeus.sHtML

[S51] C++：显式类型转换
来源：http://m.share.sjlbkw.cn/Article/details/gdqekdsnh.sHtML

static_cast<double>(a) / b
来源：http://m.share.vehdjk.com/Article/details/gyxiennob.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.vehdjk.com/Article/details/gjkrlnfoe.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/gynzgiqec.sHtML

[S53] C++：移动语义
来源：http://3g.epnwcf.com/Article/details/gvgmngtoi.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.vehdjk.com/Article/details/glnyglcru.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/glvfpifae.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.vehdjk.com/Article/details/gzbzfxlhb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.tarul.cn/Article/details/gjzzknvoe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/gjrlbfklw.sHtML

[S56] C++：optional
来源：http://m.share.vehdjk.com/Article/details/gjxiwzfox.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.sjlbkw.cn/Article/details/gflxpgkax.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.yfazqb.com/Article/details/gxoguvzef.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/gyaiewpbi.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gigzfsfri.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.epnwcf.com/Article/details/gjahmsvhi.sHtML

[S59] C++：静态断言
来源：http://blog.vehdjk.com/Article/details/gkdvgbkin.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.sjlbkw.cn/Article/details/geygkbjgp.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.epnwcf.com/Article/details/glucubvoo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.yfazqb.com/Article/details/geiounqin.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gakssphsf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fktsv.cn/Article/details/gxmrkzsnk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gyxstuvsf.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gnboruuic.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gklfpfynf.sHtML

[T02] Kotlin：变量
来源：http://blog.fktsv.cn/Article/details/ghapizlxq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.yfazqb.com/Article/details/gfodnngfg.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.sjlbkw.cn/Article/details/gneoqxcef.sHtML

"值: $b"
来源：http://wap.vehdjk.com/Article/details/gvdatmzdh.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.epnwcf.com/Article/details/gznltvrlj.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/gzledfitq.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.tarul.cn/Article/details/gtmgekhrh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.sjlbkw.cn/Article/details/gawowjqxd.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gyrwdtuuj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.vehdjk.com/Article/details/ggfhgpfzo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.tarul.cn/Article/details/gxrhdqrfl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gfqgbkjim.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fktsv.cn/Article/details/gerasorop.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.epnwcf.com/Article/details/gfyofccyu.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.tarul.cn/Article/details/gyjmdxnml.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.bbcook.cn/Article/details/glrxxstqj.sHtML

[T10] Kotlin：默认参数
来源：http://3g.vehdjk.com/Article/details/gqncjpsux.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.yfazqb.com/Article/details/gmgacmmwf.sHtML

[T11] Kotlin：协程
来源：http://www.share.bbcook.cn/Article/details/gydxbengc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fktsv.cn/Article/details/gercxqdyz.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/gcrtzakwi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gilwzrncx.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.epnwcf.com/Article/details/gbelnbdrh.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/geyjbwczc.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/glzfsxcpd.sHtML

for (i in 1..10) println(i)
来源：http://wap.vehdjk.com/Article/details/gqsevxcsb.sHtML

[T15] Kotlin：接口
来源：http://www.share.sjlbkw.cn/Article/details/ghxmarwoe.sHtML

interface Shape { fun area(): Double }
来源：http://baike.vehdjk.com/Article/details/gdtralasj.sHtML

[T16] Swift：Hello World
来源：http://mobile.fktsv.cn/Article/details/gqesnvzfn.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gxtypjfur.sHtML

[T17] Swift：变量与常量
来源：http://www.share.tarul.cn/Article/details/gawikodly.sHtML

var a = 1;  let b = 2
来源：http://www.share.tarul.cn/Article/details/gkmaytpul.sHtML

[T18] Swift：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gjifpbxsx.sHtML

"值: \(b)"
来源：http://www.share.tarul.cn/Article/details/gdbyqslrc.sHtML

[T19] Swift：可选绑定
来源：http://wap.yfazqb.com/Article/details/gkqzcxhmq.sHtML

if let n = opt { print(n) }
来源：http://www.share.bbcook.cn/Article/details/guzeawlas.sHtML

[T20] Swift：数组操作
来源：http://www.share.sjlbkw.cn/Article/details/ggtjoqmpd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.yfazqb.com/Article/details/gzkvnkxfx.sHtML

[T21] Swift：遍历
来源：http://wap.vehdjk.com/Article/details/goyfjbrlw.sHtML

for x in a { print(x) }
来源：http://wap.vehdjk.com/Article/details/gapfpqfjh.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/gnxnkvefw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.epnwcf.com/Article/details/gsrktwpoj.sHtML

[T23] Swift：函数
来源：http://wap.tarul.cn/Article/details/gmwtslpgf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.bbcook.cn/Article/details/gkxlgmsch.sHtML

[T24] Swift：闭包
来源：http://baike.sjlbkw.cn/Article/details/gvhbrggas.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.yfazqb.com/Article/details/gvqrwyunc.sHtML

[T25] Swift：结构体
来源：http://3g.vehdjk.com/Article/details/gwrkdjzad.sHtML

struct P { var x: Int }
来源：http://blog.tarul.cn/Article/details/gewhourru.sHtML

[T26] Swift：类与重写
来源：http://read.share.epnwcf.com/Article/details/gveaxopdf.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gstburrhl.sHtML

[T27] Swift：错误处理
来源：http://3g.bbcook.cn/Article/details/ggppgdzbf.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.tarul.cn/Article/details/gxhufbene.sHtML

[T28] Swift：枚举
来源：http://m.share.fktsv.cn/Article/details/gvxmvkvov.sHtML

enum Color { case red, green }
来源：http://www.blog.tarul.cn/Article/details/girtdczie.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fktsv.cn/Article/details/glunstwbf.sHtML

guard let x = opt else { return }
来源：http://www.m.share.tarul.cn/Article/details/gubfzglvt.sHtML

[T30] Swift：协议
来源：http://3g.fktsv.cn/Article/details/gtejplekt.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.yfazqb.com/Article/details/ghlmpiako.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gtxnpymrz.sHtML

print("Hello")
来源：http://m.share.epnwcf.com/Article/details/gmqikdlgz.sHtML

[T32] Lua：局部变量
来源：http://www.share.fktsv.cn/Article/details/gjopmhlwx.sHtML

local a = 1
来源：http://m.share.fktsv.cn/Article/details/gxdavkura.sHtML

[T33] Lua：表（数组）
来源：http://wap.tarul.cn/Article/details/gxsdurskw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.tarul.cn/Article/details/gbrtgtliw.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.yfazqb.com/Article/details/grpsjikcn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.bbcook.cn/Article/details/gwizxwidx.sHtML

[T35] Lua：字典表
来源：http://m.share.vehdjk.com/Article/details/gwjvglkpo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fktsv.cn/Article/details/ghjidrhyh.sHtML

[T36] Lua：函数
来源：http://3g.vehdjk.com/Article/details/gtptpwdfz.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.bbcook.cn/Article/details/ghibemhko.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gguknnztv.sHtML

"a" .. "b"
来源：http://3g.fktsv.cn/Article/details/ghglysyuh.sHtML

[T38] Lua：条件
来源：http://m.share.tarul.cn/Article/details/gscqyloih.sHtML

if x > 0 then print("正") end
来源：http://read.share.sjlbkw.cn/Article/details/gkdswhlgx.sHtML

[T39] Lua：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gogsnjigg.sHtML

string.find(s, "%d+")
来源：http://wap.bbcook.cn/Article/details/gddpweswa.sHtML

[T40] Lua：元表
来源：http://mobile.epnwcf.com/Article/details/gquywbtdu.sHtML

setmetatable({}, { __index = base })
来源：http://3g.sjlbkw.cn/Article/details/gmljauzto.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gfmtpcezs.sHtML

print "Hello\n";
来源：http://wap.epnwcf.com/Article/details/gxyirmxcg.sHtML

[T42] Perl：变量类型
来源：http://blog.yfazqb.com/Article/details/gsbnfmbow.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.yfazqb.com/Article/details/gdbfoifjq.sHtML

[T43] Perl：字符串插值
来源：http://read.share.bbcook.cn/Article/details/ghsoyhwye.sHtML

"值: $a"
来源：http://read.share.tarul.cn/Article/details/gfmttvdjw.sHtML

[T44] Perl：条件
来源：http://www.share.tarul.cn/Article/details/gjdkeakpx.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.tarul.cn/Article/details/gqwhvsxhn.sHtML

[T45] Perl：数组遍历
来源：http://3g.fktsv.cn/Article/details/gnqvpdstr.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fktsv.cn/Article/details/gtbkwtyhn.sHtML

[T46] Perl：哈希操作
来源：http://www.share.epnwcf.com/Article/details/gpwlinybs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwluorjea.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.bbcook.cn/Article/details/gfxsgwmyp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.tarul.cn/Article/details/gzejjqywp.sHtML

[T48] Perl：正则替换
来源：http://read.share.tarul.cn/Article/details/gsganadmd.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.epnwcf.com/Article/details/grkazawxw.sHtML

[T49] Perl：函数
来源：http://3g.tarul.cn/Article/details/glbrnpgfr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gvtzzouaj.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/goxbtqcsw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.tarul.cn/Article/details/gwffkfwqx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.epnwcf.com/Article/details/gqfsfwmqm.sHtML

[T51] Scala：Hello World
来源：http://www.share.yfazqb.com/Article/details/gutjiasfx.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/ggythwpwb.sHtML

[T52] Scala：变量
来源：http://mobile.tarul.cn/Article/details/gjzphvwim.sHtML

val a = 1;  var b = 2
来源：http://read.share.bbcook.cn/Article/details/gnmztrvhm.sHtML

[T53] Scala：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gfavztrzp.sHtML

s"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/gdjqfjbnc.sHtML

[T54] Scala：集合映射
来源：http://read.share.bbcook.cn/Article/details/gjjtkdhom.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.yfazqb.com/Article/details/gpovohzqe.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fktsv.cn/Article/details/gwwsgdduh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.epnwcf.com/Article/details/ggueeensh.sHtML

[T56] Scala：样例类
来源：http://baike.yfazqb.com/Article/details/gefrneudo.sHtML

case class User(name: String, age: Int)
来源：http://read.share.bbcook.cn/Article/details/ggqrgguhs.sHtML

[T57] Scala：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/glodmeemt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/govhupudb.sHtML

[T58] Scala：函数定义
来源：http://www.share.bbcook.cn/Article/details/gbppohjhm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.bbcook.cn/Article/details/gwczxpyzc.sHtML

[T59] Scala：循环
来源：http://blog.sjlbkw.cn/Article/details/gbxvtewpl.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.vehdjk.com/Article/details/gnmpflxgp.sHtML

[T60] Scala：折叠
来源：http://blog.tarul.cn/Article/details/glkqxwknl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fktsv.cn/Article/details/gzbubtpjq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdqzmnkyw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.epnwcf.com/Article/details/gbeiblaqu.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxnfxbimv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.vehdjk.com/Article/details/gyhiqooyr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.tarul.cn/Article/details/gtuqpwxzo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.vehdjk.com/Article/details/gysjlkvvg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.vehdjk.com/Article/details/gnqwpmjvd.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.sjlbkw.cn/Article/details/gngrdeygu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.sjlbkw.cn/Article/details/gsytrdpns.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/grsgrbtap.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.tarul.cn/Article/details/gdqxjgxlx.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fktsv.cn/Article/details/gupwzgjfc.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gfmagutyt.sHtML

[U06] Py：合并两个字典
来源：http://blog.yfazqb.com/Article/details/gsilbympf.sHtML

{**a, **b}
来源：http://3g.tarul.cn/Article/details/gmkysksnu.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/ggvajxzig.sHtML

{v: k for k, v in d.items()}
来源：http://blog.yfazqb.com/Article/details/gzswiqsia.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.epnwcf.com/Article/details/gifkqqhii.sHtML

[y for x in nested for y in x]
来源：http://3g.sjlbkw.cn/Article/details/gzcfgimda.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.epnwcf.com/Article/details/gagscuuhw.sHtML

max(d, key=d.get)
来源：http://wap.tarul.cn/Article/details/gkqxeywka.sHtML

[U10] Py：按值排序字典
来源：http://read.share.bbcook.cn/Article/details/gaoegnhyg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.bbcook.cn/Article/details/gihprowgr.sHtML

[U11] Py：生成器表达式
来源：http://mobile.yfazqb.com/Article/details/glyprazqx.sHtML

(x * 2 for x in arr)
来源：http://m.share.yfazqb.com/Article/details/gktxahido.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.yfazqb.com/Article/details/gdjcfdfop.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.epnwcf.com/Article/details/gzbeukgrw.sHtML

[U13] Py：固定长度队列
来源：http://www.share.bbcook.cn/Article/details/gevfugzcm.sHtML

deque(maxlen=10)
来源：http://wap.bbcook.cn/Article/details/gauzgbexi.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.tarul.cn/Article/details/gsypzvzxb.sHtML

defaultdict(list)
来源：http://www.m.share.fktsv.cn/Article/details/gwxogvrgt.sHtML

[U15] Py：高精度计时
来源：http://www.share.vehdjk.com/Article/details/gwcivrkgc.sHtML

t = time.perf_counter()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqemnlfdf.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fktsv.cn/Article/details/gnrlirfwj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.bbcook.cn/Article/details/gxmtmxgzn.sHtML

[U17] Py：初始化日志
来源：http://m.share.fktsv.cn/Article/details/gpekznrmm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.tarul.cn/Article/details/gjywiniqw.sHtML

[U18] Py：预编译正则
来源：http://m.share.yfazqb.com/Article/details/giapdncgx.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.epnwcf.com/Article/details/gtnkbhbgk.sHtML

[U19] Py：正则替换带回调
来源：http://wap.epnwcf.com/Article/details/gbfmzacni.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.tarul.cn/Article/details/gbplemgje.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.yfazqb.com/Article/details/gkafxwull.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.epnwcf.com/Article/details/gruaqtbpx.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.bbcook.cn/Article/details/grpjdcppb.sHtML

@contextlib.contextmanager
来源：http://baike.fktsv.cn/Article/details/gwhjwjpps.sHtML

[U22] Py：矩阵转置
来源：http://wap.tarul.cn/Article/details/gubpraquy.sHtML

list(zip(*m))
来源：http://3g.tarul.cn/Article/details/gfbgssqoi.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.yfazqb.com/Article/details/glfhgyxnw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.epnwcf.com/Article/details/grdwlalix.sHtML

[U24] Py：路径操作
来源：http://blog.yfazqb.com/Article/details/gloexdhsf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.vehdjk.com/Article/details/gjiyqcfrx.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.bbcook.cn/Article/details/gsmdfvdtd.sHtML

csv.DictReader(f)
来源：http://www.blog.fktsv.cn/Article/details/gtstgmazb.sHtML

[U26] Py：并发下载
来源：http://wap.sjlbkw.cn/Article/details/gvmbvwglc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.yfazqb.com/Article/details/gnmkezbpf.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.bbcook.cn/Article/details/gwagpddxc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.yfazqb.com/Article/details/gkcihiobl.sHtML

[U28] Py：类型别名
来源：http://read.share.epnwcf.com/Article/details/gexvtphql.sHtML

UserId = int
来源：http://read.share.sjlbkw.cn/Article/details/gcwjkinbx.sHtML

[U29] Py：属性校验
来源：http://wap.fktsv.cn/Article/details/giugctadr.sHtML

@property 与 @x.setter 配合
来源：http://wap.epnwcf.com/Article/details/gskjvkhqf.sHtML

[U30] Py：数据类
来源：http://3g.vehdjk.com/Article/details/gtmxiwixa.sHtML

@dataclass(slots=True)
来源：http://3g.vehdjk.com/Article/details/gxftbevge.sHtML

[U31] Py：单测
来源：http://m.share.vehdjk.com/Article/details/gcespdiyq.sHtML

python -m pytest -q
来源：http://blog.yfazqb.com/Article/details/gyjqqypcr.sHtML

[U32] Py：代码格式化
来源：http://blog.bbcook.cn/Article/details/gaqfopexz.sHtML

ruff format . && ruff check --fix .
来源：http://blog.epnwcf.com/Article/details/gqrubslef.sHtML

[U33] Py：打包发布
来源：http://read.share.yfazqb.com/Article/details/gdnxgsdoc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.bbcook.cn/Article/details/geaqrlimp.sHtML

[U34] Py：判断编码
来源：http://www.blog.sjlbkw.cn/Article/details/guscgikhs.sHtML

chardet.detect(raw)
来源：http://3g.yfazqb.com/Article/details/grrfjxudh.sHtML

[U35] Py：发送邮件
来源：http://mobile.bbcook.cn/Article/details/gjygqvnyg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.epnwcf.com/Article/details/gewifzdhh.sHtML

[U36] Py：定时任务
来源：http://m.share.yfazqb.com/Article/details/gfkthmbvo.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.bbcook.cn/Article/details/gziktidbc.sHtML


<!-- 参考信息 -->