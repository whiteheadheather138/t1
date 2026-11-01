代发 wailian999

int main(int argc, char **argv)
来源：http://baike.tarul.cn/Article/details/gvlfjopii.sHtML

[S19] C：快速排序
来源：http://baike.sjlbkw.cn/Article/details/gkygoeiqb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gborjnywe.sHtML

[S20] C：二分查找
来源：http://wap.fktsv.cn/Article/details/gqhgjfzca.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gjtmxfuut.sHtML

[S21] C：字符类别判断
来源：http://www.blog.epnwcf.com/Article/details/glnjypwvg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.bbcook.cn/Article/details/gypktdouc.sHtML

[S22] C：字符串转数字
来源：http://wap.sjlbkw.cn/Article/details/ggjfhrdcz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.yfazqb.com/Article/details/gdgzkulgw.sHtML

[S23] C：随机数
来源：http://baike.fktsv.cn/Article/details/guinzdcug.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.tarul.cn/Article/details/gmdpursog.sHtML

[S24] C：获取本地时间
来源：http://blog.sjlbkw.cn/Article/details/gvapjvlkj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.epnwcf.com/Article/details/gjszzeuni.sHtML

[S25] C：内存拷贝
来源：http://baike.epnwcf.com/Article/details/ggufzrpro.sHtML

memcpy(dst, src, n);
来源：http://www.blog.tarul.cn/Article/details/gsjeslxxe.sHtML

[S26] C：内存清零
来源：http://wap.tarul.cn/Article/details/gokwzjjep.sHtML

memset(a, 0, sizeof a);
来源：http://baike.sjlbkw.cn/Article/details/gqqlzpsmt.sHtML

[S27] C：定义常量
来源：http://wap.vehdjk.com/Article/details/gccmnzbnn.sHtML

const double PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gxpswpasu.sHtML

[S28] C：静态变量
来源：http://mobile.fktsv.cn/Article/details/gpllexasc.sHtML

static int counter = 0;
来源：http://3g.sjlbkw.cn/Article/details/ggqjzylmq.sHtML

[S29] C：变参函数
来源：http://m.share.yfazqb.com/Article/details/genlmnfmn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.yfazqb.com/Article/details/gmnqcebsn.sHtML

[S30] C：头文件保护
来源：http://www.share.bbcook.cn/Article/details/gqlicxtwi.sHtML

#ifndef X_H
来源：http://3g.bbcook.cn/Article/details/gyephqpvu.sHtML

#define X_H
来源：http://m.share.fktsv.cn/Article/details/gapulrjla.sHtML

#endif
来源：http://3g.epnwcf.com/Article/details/gacynlyov.sHtML

[S31] C++：Hello World
来源：http://blog.bbcook.cn/Article/details/gptxtshcn.sHtML

#include <iostream>
来源：http://mobile.tarul.cn/Article/details/gzslpvoph.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.tarul.cn/Article/details/gsagdxhpo.sHtML

[S32] C++：字符串
来源：http://m.share.sjlbkw.cn/Article/details/gpccmxayq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fktsv.cn/Article/details/gdfqultwu.sHtML

[S33] C++：vector 增删
来源：http://www.blog.bbcook.cn/Article/details/ggchlcaoi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/gsinldohz.sHtML

[S34] C++：遍历 vector
来源：http://3g.yfazqb.com/Article/details/ggziruhfr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.yfazqb.com/Article/details/gwxtqwiju.sHtML

[S35] C++：map
来源：http://3g.bbcook.cn/Article/details/gtegantwf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gaqyzkfcl.sHtML

[S36] C++：unordered_map
来源：http://3g.bbcook.cn/Article/details/gzvlcqqtx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gfryfdxtu.sHtML

[S37] C++：set
来源：http://baike.sjlbkw.cn/Article/details/gzubxyatv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.sjlbkw.cn/Article/details/gnjudcabh.sHtML

[S38] C++：排序
来源：http://read.share.yfazqb.com/Article/details/guqbmrwkl.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.tarul.cn/Article/details/gbvxhhlmf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gfptxkbth.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.epnwcf.com/Article/details/gektfzrwr.sHtML

[S40] C++：查找元素
来源：http://3g.fktsv.cn/Article/details/ghdldtace.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/gwzlojndl.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/gwgpujmuy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.vehdjk.com/Article/details/gplcmdbba.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/gitxcgray.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.yfazqb.com/Article/details/gwmnxztph.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/gujvfcztn.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.sjlbkw.cn/Article/details/gsbaxxlkg.sHtML

[S44] C++：引用传参
来源：http://wap.fktsv.cn/Article/details/gapwuqjkg.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fktsv.cn/Article/details/gxvzpsgfc.sHtML

[S45] C++：lambda
来源：http://mobile.sjlbkw.cn/Article/details/gtjspnzdb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.tarul.cn/Article/details/gcnyshbiv.sHtML

[S46] C++：函数模板
来源：http://www.m.share.bbcook.cn/Article/details/ggelqngea.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.epnwcf.com/Article/details/ghesytwei.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.yfazqb.com/Article/details/gemcuwmjf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.bbcook.cn/Article/details/gbewfnskn.sHtML

[S48] C++：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gruzdrlzy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.yfazqb.com/Article/details/gxbtgbfka.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/gvzpdhwgo.sHtML

[S49] C++：写文件
来源：http://blog.sjlbkw.cn/Article/details/gisigcjxq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.vehdjk.com/Article/details/gqaldbxfv.sHtML

[S50] C++：格式化数字
来源：http://m.share.sjlbkw.cn/Article/details/gncowxqof.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gyoopqpia.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/gvihtzebb.sHtML

static_cast<double>(a) / b
来源：http://read.share.yfazqb.com/Article/details/gexevkmbz.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.vehdjk.com/Article/details/gmsasuphh.sHtML

int size() const noexcept { return n_; }
来源：http://blog.epnwcf.com/Article/details/gnfbcpdmx.sHtML

[S53] C++：移动语义
来源：http://blog.fktsv.cn/Article/details/glklbvdxr.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fktsv.cn/Article/details/gvakkyskv.sHtML

[S54] C++：异常处理
来源：http://wap.bbcook.cn/Article/details/gyneebldf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.vehdjk.com/Article/details/gzjapjhqo.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/glmfldvfx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.sjlbkw.cn/Article/details/gyeznzigd.sHtML

[S56] C++：optional
来源：http://mobile.bbcook.cn/Article/details/gijufmqav.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.tarul.cn/Article/details/guogfphcc.sHtML

[S57] C++：编译期常量
来源：http://m.share.yfazqb.com/Article/details/gvuhyvhmn.sHtML

constexpr int N = 10;
来源：http://blog.bbcook.cn/Article/details/gylghytbi.sHtML

[S58] C++：命名空间
来源：http://mobile.vehdjk.com/Article/details/gvnkpvapn.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.bbcook.cn/Article/details/gnkrkhgfi.sHtML

[S59] C++：静态断言
来源：http://3g.yfazqb.com/Article/details/ggedadpco.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.vehdjk.com/Article/details/gsqzawqci.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/gjeegzehi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fktsv.cn/Article/details/gvhjqksiq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gliqdpadq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.sjlbkw.cn/Article/details/gqthdkrbo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqfipdkci.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gwkdshgwj.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gmuyadlsu.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gbattxpyh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.epnwcf.com/Article/details/gxzdlhncz.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fktsv.cn/Article/details/gvaeriqra.sHtML

"值: $b"
来源：http://blog.yfazqb.com/Article/details/gvgpwhoaj.sHtML

[T04] Kotlin：空安全
来源：http://3g.tarul.cn/Article/details/glvggunaw.sHtML

val n: String? = null;  n?.length
来源：http://m.share.yfazqb.com/Article/details/gqfvuavvx.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.bbcook.cn/Article/details/ggolerxfw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.sjlbkw.cn/Article/details/gdkpbizmr.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.yfazqb.com/Article/details/ghqugmubi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.epnwcf.com/Article/details/guzpczjzn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gglwflfbm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.tarul.cn/Article/details/grwgupzod.sHtML

[T08] Kotlin：数据类
来源：http://blog.tarul.cn/Article/details/gcreklrwq.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.tarul.cn/Article/details/gnljfgnel.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.bbcook.cn/Article/details/gpxiwyelr.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fktsv.cn/Article/details/gixewpxht.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.yfazqb.com/Article/details/gjupesmki.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.bbcook.cn/Article/details/gzxejmxkn.sHtML

[T11] Kotlin：协程
来源：http://blog.vehdjk.com/Article/details/gcwhnzoxz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.tarul.cn/Article/details/grozlghth.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.sjlbkw.cn/Article/details/gheqkshtv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/goyzmuazx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fktsv.cn/Article/details/gllakuapy.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.yfazqb.com/Article/details/glexnohdg.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gvobpsazs.sHtML

for (i in 1..10) println(i)
来源：http://wap.sjlbkw.cn/Article/details/gubzvffos.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/guvmuhfmz.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fktsv.cn/Article/details/gdahzjqvx.sHtML

[T16] Swift：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gireshpao.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gungaweik.sHtML

[T17] Swift：变量与常量
来源：http://mobile.vehdjk.com/Article/details/govgtpwyw.sHtML

var a = 1;  let b = 2
来源：http://read.share.vehdjk.com/Article/details/goquoinfb.sHtML

[T18] Swift：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/ghrzskooc.sHtML

"值: \(b)"
来源：http://wap.tarul.cn/Article/details/gpwwqskeb.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/ghfgsbdqr.sHtML

if let n = opt { print(n) }
来源：http://www.share.yfazqb.com/Article/details/gwqvjwswd.sHtML

[T20] Swift：数组操作
来源：http://blog.vehdjk.com/Article/details/gvupowovm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/gqdfvzbcc.sHtML

[T21] Swift：遍历
来源：http://m.share.sjlbkw.cn/Article/details/guxnjefoh.sHtML

for x in a { print(x) }
来源：http://blog.epnwcf.com/Article/details/gdzcamvvv.sHtML

[T22] Swift：字典
来源：http://blog.vehdjk.com/Article/details/gyxfepzvr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.yfazqb.com/Article/details/gkwjvomhy.sHtML

[T23] Swift：函数
来源：http://www.share.tarul.cn/Article/details/gpbcsmgmx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.tarul.cn/Article/details/gfanztwdp.sHtML

[T24] Swift：闭包
来源：http://read.share.vehdjk.com/Article/details/ggcmrlczd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/giayokird.sHtML

[T25] Swift：结构体
来源：http://blog.fktsv.cn/Article/details/gtvajofur.sHtML

struct P { var x: Int }
来源：http://wap.sjlbkw.cn/Article/details/gpglgkeif.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/gtiaxivlt.sHtML

class A: Base { override func f() {} }
来源：http://mobile.bbcook.cn/Article/details/gkckwcqzi.sHtML

[T27] Swift：错误处理
来源：http://www.share.tarul.cn/Article/details/gkshgrcmc.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.vehdjk.com/Article/details/gykzfauog.sHtML

[T28] Swift：枚举
来源：http://m.share.bbcook.cn/Article/details/gzfzbvepo.sHtML

enum Color { case red, green }
来源：http://www.share.tarul.cn/Article/details/gusngrgwh.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.yfazqb.com/Article/details/gyqklxzuj.sHtML

guard let x = opt else { return }
来源：http://www.blog.tarul.cn/Article/details/gymfnqthc.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/glbnnbysr.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.yfazqb.com/Article/details/gkdrbvbid.sHtML

[T31] Lua：Hello World
来源：http://m.share.yfazqb.com/Article/details/gnxqhrhir.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/garzpozwb.sHtML

[T32] Lua：局部变量
来源：http://www.share.epnwcf.com/Article/details/gsvleyuxx.sHtML

local a = 1
来源：http://read.share.tarul.cn/Article/details/gkloximhx.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/gsisotjez.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fktsv.cn/Article/details/ggcqssgvx.sHtML

[T34] Lua：遍历表
来源：http://www.blog.bbcook.cn/Article/details/gyoiooryg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fktsv.cn/Article/details/grsmqxvnh.sHtML

[T35] Lua：字典表
来源：http://www.share.sjlbkw.cn/Article/details/ggbhxcsow.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gkfsbnxgz.sHtML

[T36] Lua：函数
来源：http://wap.sjlbkw.cn/Article/details/gxbjmpsgf.sHtML

function add(a, b) return a + b end
来源：http://www.blog.tarul.cn/Article/details/grxjjjlbe.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gmykqwklh.sHtML

"a" .. "b"
来源：http://baike.vehdjk.com/Article/details/geonyejum.sHtML

[T38] Lua：条件
来源：http://wap.vehdjk.com/Article/details/gkkhsbjrr.sHtML

if x > 0 then print("正") end
来源：http://3g.vehdjk.com/Article/details/glscipgwp.sHtML

[T39] Lua：模式匹配
来源：http://baike.vehdjk.com/Article/details/gcbgarzws.sHtML

string.find(s, "%d+")
来源：http://baike.tarul.cn/Article/details/gunrqupqy.sHtML

[T40] Lua：元表
来源：http://wap.tarul.cn/Article/details/gkkoarpye.sHtML

setmetatable({}, { __index = base })
来源：http://3g.yfazqb.com/Article/details/gaighqhvw.sHtML

[T41] Perl：Hello World
来源：http://mobile.yfazqb.com/Article/details/gzqevclbx.sHtML

print "Hello\n";
来源：http://read.share.sjlbkw.cn/Article/details/gogsmcnwh.sHtML

[T42] Perl：变量类型
来源：http://3g.epnwcf.com/Article/details/gdeusalvg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.bbcook.cn/Article/details/gtqtndefr.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gdafwhlcc.sHtML

"值: $a"
来源：http://read.share.sjlbkw.cn/Article/details/gwosrrdee.sHtML

[T44] Perl：条件
来源：http://www.m.share.fktsv.cn/Article/details/gzsablgez.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/gzbtzihbu.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gcmiiuekq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.epnwcf.com/Article/details/gjuittrhk.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fktsv.cn/Article/details/gatltrpco.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.bbcook.cn/Article/details/grnqeuhxo.sHtML

[T47] Perl：正则捕获
来源：http://m.share.bbcook.cn/Article/details/gnrxkeaqy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fktsv.cn/Article/details/gjpumbckg.sHtML

[T48] Perl：正则替换
来源：http://blog.bbcook.cn/Article/details/gtcauyrds.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.bbcook.cn/Article/details/gaonbkymd.sHtML

[T49] Perl：函数
来源：http://mobile.yfazqb.com/Article/details/gvquqfdum.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gxuwteosk.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gezvvqjfm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.vehdjk.com/Article/details/geukndoqi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fktsv.cn/Article/details/gqblksdvn.sHtML

[T51] Scala：Hello World
来源：http://m.share.bbcook.cn/Article/details/gzcffresl.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gnyokjgyu.sHtML

[T52] Scala：变量
来源：http://read.share.yfazqb.com/Article/details/gekviwaeo.sHtML

val a = 1;  var b = 2
来源：http://wap.epnwcf.com/Article/details/gfkdsobzv.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gjkircarr.sHtML

s"值: $b"
来源：http://wap.yfazqb.com/Article/details/gjhmhtgxh.sHtML

[T54] Scala：集合映射
来源：http://m.share.vehdjk.com/Article/details/gbqzndsxh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.epnwcf.com/Article/details/gvbfxibto.sHtML

[T55] Scala：集合过滤
来源：http://wap.bbcook.cn/Article/details/gdjvvpbik.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.epnwcf.com/Article/details/gdaxjxdcg.sHtML

[T56] Scala：样例类
来源：http://www.m.share.yfazqb.com/Article/details/gtfxzymqk.sHtML

case class User(name: String, age: Int)
来源：http://wap.bbcook.cn/Article/details/gwbxilnbk.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gjhwfdahm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fktsv.cn/Article/details/grodprdxd.sHtML

[T58] Scala：函数定义
来源：http://blog.fktsv.cn/Article/details/gckcomtob.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fktsv.cn/Article/details/grihgmcgh.sHtML

[T59] Scala：循环
来源：http://mobile.epnwcf.com/Article/details/giixbouxe.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gmwqboqxj.sHtML

[T60] Scala：折叠
来源：http://wap.fktsv.cn/Article/details/gxfvimdir.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.sjlbkw.cn/Article/details/gmbpagcug.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfszxigmi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.bbcook.cn/Article/details/gilrcotky.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gpqjcrmbo.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.sjlbkw.cn/Article/details/gnogibwjt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.bbcook.cn/Article/details/geegdnvod.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.yfazqb.com/Article/details/gapxsxvgk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.yfazqb.com/Article/details/gfcguqwrn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.tarul.cn/Article/details/gykrzjazq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.bbcook.cn/Article/details/gjxltdugq.sHtML

[U04] Py：变量调试打印
来源：http://3g.bbcook.cn/Article/details/gccwqwogy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.sjlbkw.cn/Article/details/gcwughrtm.sHtML

[U05] Py：列表去重且保序
来源：http://baike.yfazqb.com/Article/details/gxlfavexw.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fktsv.cn/Article/details/ggtovckfr.sHtML

[U06] Py：合并两个字典
来源：http://blog.tarul.cn/Article/details/gkqhrvmsu.sHtML

{**a, **b}
来源：http://blog.bbcook.cn/Article/details/gnliezdcz.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fktsv.cn/Article/details/gaexqqqtx.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/geslicsiz.sHtML

[U08] Py：展平二维列表
来源：http://baike.epnwcf.com/Article/details/giepjcnfb.sHtML

[y for x in nested for y in x]
来源：http://3g.bbcook.cn/Article/details/gtpmvglkw.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.tarul.cn/Article/details/grqbokxlt.sHtML

max(d, key=d.get)
来源：http://3g.bbcook.cn/Article/details/glwqzltcw.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fktsv.cn/Article/details/gkjrsbppj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.vehdjk.com/Article/details/ggnvgnicu.sHtML

[U11] Py：生成器表达式
来源：http://wap.sjlbkw.cn/Article/details/gzbyssbcr.sHtML

(x * 2 for x in arr)
来源：http://baike.yfazqb.com/Article/details/gtchjwixi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.vehdjk.com/Article/details/ggmlsdmrk.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.sjlbkw.cn/Article/details/ghmfuizud.sHtML

[U13] Py：固定长度队列
来源：http://m.share.epnwcf.com/Article/details/glgbtomef.sHtML

deque(maxlen=10)
来源：http://www.blog.epnwcf.com/Article/details/gpmciyikt.sHtML

[U14] Py：分组收集到列表
来源：http://baike.epnwcf.com/Article/details/grgfjbdoz.sHtML

defaultdict(list)
来源：http://read.share.yfazqb.com/Article/details/gmdrzmequ.sHtML

[U15] Py：高精度计时
来源：http://www.share.fktsv.cn/Article/details/gjdukcaic.sHtML

t = time.perf_counter()
来源：http://3g.tarul.cn/Article/details/gspnpntma.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.epnwcf.com/Article/details/gnsaugakt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.bbcook.cn/Article/details/gywjphoeo.sHtML

[U17] Py：初始化日志
来源：http://mobile.fktsv.cn/Article/details/gpljgalij.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.tarul.cn/Article/details/glfhuskwc.sHtML

[U18] Py：预编译正则
来源：http://m.share.bbcook.cn/Article/details/ggjxsluit.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.yfazqb.com/Article/details/gzxnimyvn.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.tarul.cn/Article/details/gimqqwcub.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.vehdjk.com/Article/details/gteeeqwaj.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fktsv.cn/Article/details/giluwuefg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.vehdjk.com/Article/details/gwxibgrfm.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.epnwcf.com/Article/details/gmpjauwdv.sHtML

@contextlib.contextmanager
来源：http://m.share.fktsv.cn/Article/details/gmljggvjh.sHtML

[U22] Py：矩阵转置
来源：http://blog.tarul.cn/Article/details/gnufvpgxz.sHtML

list(zip(*m))
来源：http://www.m.share.bbcook.cn/Article/details/gvanuauwa.sHtML

[U23] Py：分块读取大文件
来源：http://wap.bbcook.cn/Article/details/gnlcbbpko.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.tarul.cn/Article/details/gmtmdwzjq.sHtML

[U24] Py：路径操作
来源：http://wap.vehdjk.com/Article/details/gpbpeybty.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.yfazqb.com/Article/details/gfrfnlwlg.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.epnwcf.com/Article/details/gjpcobtux.sHtML

csv.DictReader(f)
来源：http://wap.vehdjk.com/Article/details/gchcdrafd.sHtML

[U26] Py：并发下载
来源：http://blog.bbcook.cn/Article/details/gspkacmoj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fktsv.cn/Article/details/gqaptzxdn.sHtML

[U27] Py：异步 HTTP
来源：http://baike.yfazqb.com/Article/details/gbtqgcelf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.tarul.cn/Article/details/gimwgwxuh.sHtML

[U28] Py：类型别名
来源：http://m.share.sjlbkw.cn/Article/details/gpvgmjxdz.sHtML

UserId = int
来源：http://www.m.share.fktsv.cn/Article/details/gqxqbkold.sHtML

[U29] Py：属性校验
来源：http://www.share.tarul.cn/Article/details/glxidjgqk.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fktsv.cn/Article/details/gwtnjyhff.sHtML

[U30] Py：数据类
来源：http://www.share.epnwcf.com/Article/details/gxbauflcb.sHtML

@dataclass(slots=True)
来源：http://www.share.vehdjk.com/Article/details/ggvocmpog.sHtML

[U31] Py：单测
来源：http://blog.fktsv.cn/Article/details/gltoznsju.sHtML

python -m pytest -q
来源：http://www.blog.tarul.cn/Article/details/gbdysdhao.sHtML

[U32] Py：代码格式化
来源：http://mobile.vehdjk.com/Article/details/gpsnlkxgn.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.epnwcf.com/Article/details/gkpkynmqs.sHtML

[U33] Py：打包发布
来源：http://mobile.fktsv.cn/Article/details/ginuomcle.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.bbcook.cn/Article/details/gjtrzniad.sHtML

[U34] Py：判断编码
来源：http://www.m.share.epnwcf.com/Article/details/gsuexykis.sHtML

chardet.detect(raw)
来源：http://read.share.fktsv.cn/Article/details/gxslpgdbe.sHtML

[U35] Py：发送邮件
来源：http://mobile.yfazqb.com/Article/details/gampmtyfr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.vehdjk.com/Article/details/gcmuegvna.sHtML

[U36] Py：定时任务
来源：http://read.share.fktsv.cn/Article/details/grjcaaplq.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.bbcook.cn/Article/details/gewlqnpme.sHtML

[U37] Py：读写 Excel
来源：http://www.share.vehdjk.com/Article/details/gkslqoyyn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.vehdjk.com/Article/details/gharkzpzg.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.epnwcf.com/Article/details/gihkgjjxa.sHtML

Path(__file__).resolve().parent
来源：http://baike.fktsv.cn/Article/details/ggiiirwgt.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.sjlbkw.cn/Article/details/ghrereryz.sHtML

sys.stdout.isatty()
来源：http://www.blog.vehdjk.com/Article/details/gthhpgpzi.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fktsv.cn/Article/details/gskbpgkgb.sHtML

print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gsikfuyea.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.yfazqb.com/Article/details/gucdfbfbe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.epnwcf.com/Article/details/gyovvubjb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.tarul.cn/Article/details/gczrwuwos.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.epnwcf.com/Article/details/gjwnzkxuk.sHtML


<!-- 参考信息 -->