代发 wailian999

x |= (1 << 3);
来源：http://3g.tarul.cn/Article/details/ggoxnkelq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.yfazqb.com/Article/details/gkgpkdlfr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.vehdjk.com/Article/details/gbaedrpdy.sHtML

[S18] C：命令行参数
来源：http://mobile.sjlbkw.cn/Article/details/gdkeyxoqb.sHtML

int main(int argc, char **argv)
来源：http://blog.tarul.cn/Article/details/gbdjzpaeb.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/gkrhtygex.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/gzilrfgaz.sHtML

[S20] C：二分查找
来源：http://m.share.yfazqb.com/Article/details/gcxcdande.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gryfolteh.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/gzzttwsxp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.vehdjk.com/Article/details/gdsengdrz.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/ggrbxntso.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.yfazqb.com/Article/details/grrjawarf.sHtML

[S23] C：随机数
来源：http://www.share.vehdjk.com/Article/details/gylfzbphk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.yfazqb.com/Article/details/geyxkqeez.sHtML

[S24] C：获取本地时间
来源：http://mobile.epnwcf.com/Article/details/gaummeqbr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.sjlbkw.cn/Article/details/ghwdtaqzz.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gkkrajosv.sHtML

memcpy(dst, src, n);
来源：http://www.share.tarul.cn/Article/details/ghburghce.sHtML

[S26] C：内存清零
来源：http://read.share.vehdjk.com/Article/details/ghpklkclk.sHtML

memset(a, 0, sizeof a);
来源：http://3g.bbcook.cn/Article/details/gexeuhvvu.sHtML

[S27] C：定义常量
来源：http://wap.sjlbkw.cn/Article/details/ggyexmnld.sHtML

const double PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gnluzfxaj.sHtML

[S28] C：静态变量
来源：http://mobile.fktsv.cn/Article/details/gsybuhqzv.sHtML

static int counter = 0;
来源：http://www.m.share.epnwcf.com/Article/details/gcojosfmq.sHtML

[S29] C：变参函数
来源：http://mobile.epnwcf.com/Article/details/gvwcjdmsz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.yfazqb.com/Article/details/geqkauwje.sHtML

[S30] C：头文件保护
来源：http://www.share.yfazqb.com/Article/details/gmdvdaxlf.sHtML

#ifndef X_H
来源：http://read.share.bbcook.cn/Article/details/gfvjmwoch.sHtML

#define X_H
来源：http://www.m.share.vehdjk.com/Article/details/gletbyjoz.sHtML

#endif
来源：http://mobile.sjlbkw.cn/Article/details/gqfeujncs.sHtML

[S31] C++：Hello World
来源：http://wap.sjlbkw.cn/Article/details/glqatwldi.sHtML

#include <iostream>
来源：http://read.share.sjlbkw.cn/Article/details/gemyedntk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.epnwcf.com/Article/details/ggkowkapn.sHtML

[S32] C++：字符串
来源：http://wap.vehdjk.com/Article/details/gsboshbmz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fktsv.cn/Article/details/ghzyjfpzq.sHtML

[S33] C++：vector 增删
来源：http://wap.fktsv.cn/Article/details/guqmbemha.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.epnwcf.com/Article/details/gvrfrgsra.sHtML

[S34] C++：遍历 vector
来源：http://3g.epnwcf.com/Article/details/gbablazvh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fktsv.cn/Article/details/gemenslok.sHtML

[S35] C++：map
来源：http://read.share.bbcook.cn/Article/details/gzhnuvwqa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gclqepprj.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/ggubatiku.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gswjvpupc.sHtML

[S37] C++：set
来源：http://3g.sjlbkw.cn/Article/details/gpnexcgpv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.sjlbkw.cn/Article/details/gwmbrqqud.sHtML

[S38] C++：排序
来源：http://blog.sjlbkw.cn/Article/details/gqgszkaoi.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/gywsgyrof.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fktsv.cn/Article/details/gtlksknkf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/gkywmdtme.sHtML

[S40] C++：查找元素
来源：http://m.share.yfazqb.com/Article/details/gyydpvbqh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.yfazqb.com/Article/details/gzgorbkwn.sHtML

[S41] C++：类与构造函数
来源：http://www.share.yfazqb.com/Article/details/gyaggbkjo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.sjlbkw.cn/Article/details/gfunhyiws.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fktsv.cn/Article/details/gudnjlcbt.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fktsv.cn/Article/details/grtsrxvqc.sHtML

[S43] C++：智能指针
来源：http://www.blog.yfazqb.com/Article/details/gmlykzhch.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.bbcook.cn/Article/details/gvvvppmkt.sHtML

[S44] C++：引用传参
来源：http://mobile.fktsv.cn/Article/details/gjzlrmxza.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fktsv.cn/Article/details/gtpltxfvu.sHtML

[S45] C++：lambda
来源：http://www.m.share.tarul.cn/Article/details/gdftprodr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.epnwcf.com/Article/details/gedtvnzzm.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/gxauzzgxf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.vehdjk.com/Article/details/gvikifvmy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fktsv.cn/Article/details/gsyvbvtun.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.bbcook.cn/Article/details/gawrzzwyq.sHtML

[S48] C++：逐行读文件
来源：http://3g.tarul.cn/Article/details/gnxqtdjig.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.tarul.cn/Article/details/gvmwvdkox.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.vehdjk.com/Article/details/gnldvvaub.sHtML

[S49] C++：写文件
来源：http://www.share.epnwcf.com/Article/details/gdqibkxxi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.sjlbkw.cn/Article/details/gatlxvfjz.sHtML

[S50] C++：格式化数字
来源：http://mobile.tarul.cn/Article/details/grhsaghkl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gzrdqyyzo.sHtML

[S51] C++：显式类型转换
来源：http://m.share.sjlbkw.cn/Article/details/gpwnpfhnq.sHtML

static_cast<double>(a) / b
来源：http://baike.tarul.cn/Article/details/gjcpgiiqn.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.tarul.cn/Article/details/ghhharmik.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.vehdjk.com/Article/details/gltzwxbst.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/guduwlsdm.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.vehdjk.com/Article/details/gfuipjcxi.sHtML

[S54] C++：异常处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhsgpadl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.bbcook.cn/Article/details/gizhfsvqg.sHtML

[S55] C++：结构化绑定
来源：http://baike.epnwcf.com/Article/details/gblbpjgsg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/glevvjsbc.sHtML

[S56] C++：optional
来源：http://www.share.sjlbkw.cn/Article/details/gqbhpypga.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.vehdjk.com/Article/details/gvkmorxop.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gsltheyik.sHtML

constexpr int N = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gfgqdjfkj.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gaybexazg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fktsv.cn/Article/details/gxpdisjdl.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/glfkagyzb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.yfazqb.com/Article/details/gumdptebj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fktsv.cn/Article/details/gdgmoldry.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gfdvbwmnn.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxzzviknv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.sjlbkw.cn/Article/details/gapyikvry.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gsbtazmvk.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.bbcook.cn/Article/details/goobznmud.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/guzjhjlzn.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/grnahcloh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.epnwcf.com/Article/details/gwxmqjner.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fktsv.cn/Article/details/glnxwshcv.sHtML

"值: $b"
来源：http://3g.yfazqb.com/Article/details/ghkqlxxfq.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fktsv.cn/Article/details/gzgpsnodx.sHtML

val n: String? = null;  n?.length
来源：http://3g.yfazqb.com/Article/details/gfxrqpwfd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gzcydtqhl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.yfazqb.com/Article/details/gepyacoyo.sHtML

[T06] Kotlin：集合映射
来源：http://baike.vehdjk.com/Article/details/gyatvqscm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.epnwcf.com/Article/details/gihdoqacq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gcxqftlbf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.bbcook.cn/Article/details/gdzjyrgry.sHtML

[T08] Kotlin：数据类
来源：http://baike.epnwcf.com/Article/details/gijereexl.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fktsv.cn/Article/details/grxrjaqwv.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.epnwcf.com/Article/details/ghjjdctnu.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fktsv.cn/Article/details/gptflzvgl.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/grvcrauth.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.sjlbkw.cn/Article/details/gvhygsnxm.sHtML

[T11] Kotlin：协程
来源：http://3g.bbcook.cn/Article/details/gssmbmldq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.vehdjk.com/Article/details/gqieczuqk.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.tarul.cn/Article/details/griuadfof.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.epnwcf.com/Article/details/gdmvtzgqs.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.yfazqb.com/Article/details/gqdxjzjfe.sHtML

val m = mapOf("a" to 1)
来源：http://wap.vehdjk.com/Article/details/gacufwulc.sHtML

[T14] Kotlin：循环
来源：http://wap.fktsv.cn/Article/details/grsqpxwch.sHtML

for (i in 1..10) println(i)
来源：http://read.share.tarul.cn/Article/details/gccptoqjx.sHtML

[T15] Kotlin：接口
来源：http://read.share.fktsv.cn/Article/details/gxslfmayl.sHtML

interface Shape { fun area(): Double }
来源：http://baike.epnwcf.com/Article/details/guiodbjfb.sHtML

[T16] Swift：Hello World
来源：http://blog.vehdjk.com/Article/details/gmytgqunc.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gqjqmynjh.sHtML

[T17] Swift：变量与常量
来源：http://blog.sjlbkw.cn/Article/details/gcpldjmdw.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/gblkpcrdb.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gsxluaxqq.sHtML

"值: \(b)"
来源：http://m.share.fktsv.cn/Article/details/gsvgltvgp.sHtML

[T19] Swift：可选绑定
来源：http://www.share.bbcook.cn/Article/details/galtmbjjb.sHtML

if let n = opt { print(n) }
来源：http://3g.vehdjk.com/Article/details/gryxpiomo.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/guldmvkrc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fktsv.cn/Article/details/gzegpsudu.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/gohrlruqc.sHtML

for x in a { print(x) }
来源：http://mobile.vehdjk.com/Article/details/gnnvvzqto.sHtML

[T22] Swift：字典
来源：http://blog.sjlbkw.cn/Article/details/gtmsakawj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.sjlbkw.cn/Article/details/gggdjvpuq.sHtML

[T23] Swift：函数
来源：http://3g.bbcook.cn/Article/details/gnnlufcku.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.vehdjk.com/Article/details/gxhexbnqu.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gyrmdqdoe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.vehdjk.com/Article/details/gfuadbanh.sHtML

[T25] Swift：结构体
来源：http://www.blog.vehdjk.com/Article/details/gqbjyhcfk.sHtML

struct P { var x: Int }
来源：http://blog.sjlbkw.cn/Article/details/glfhghcym.sHtML

[T26] Swift：类与重写
来源：http://mobile.tarul.cn/Article/details/gkdnhuzqn.sHtML

class A: Base { override func f() {} }
来源：http://blog.tarul.cn/Article/details/gamsdfgdr.sHtML

[T27] Swift：错误处理
来源：http://m.share.bbcook.cn/Article/details/gepptbfiz.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.bbcook.cn/Article/details/gvhtygcou.sHtML

[T28] Swift：枚举
来源：http://blog.fktsv.cn/Article/details/guvfpbvra.sHtML

enum Color { case red, green }
来源：http://www.share.sjlbkw.cn/Article/details/grzomsdic.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.epnwcf.com/Article/details/gcmqtaljh.sHtML

guard let x = opt else { return }
来源：http://baike.yfazqb.com/Article/details/gsphpwrsn.sHtML

[T30] Swift：协议
来源：http://read.share.sjlbkw.cn/Article/details/gmkfpvsdi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fktsv.cn/Article/details/ghfbuskod.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwgljixt.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gyovnikbr.sHtML

[T32] Lua：局部变量
来源：http://www.blog.tarul.cn/Article/details/gqnjlymqd.sHtML

local a = 1
来源：http://3g.yfazqb.com/Article/details/gpqybsnoh.sHtML

[T33] Lua：表（数组）
来源：http://www.share.tarul.cn/Article/details/gkqtyjjlx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fktsv.cn/Article/details/gvypmzsid.sHtML

[T34] Lua：遍历表
来源：http://www.blog.epnwcf.com/Article/details/gjqlnnxhc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.sjlbkw.cn/Article/details/gtgalydvf.sHtML

[T35] Lua：字典表
来源：http://read.share.sjlbkw.cn/Article/details/grwuudeps.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.vehdjk.com/Article/details/gttexaxsk.sHtML

[T36] Lua：函数
来源：http://wap.epnwcf.com/Article/details/gogsqyqph.sHtML

function add(a, b) return a + b end
来源：http://wap.epnwcf.com/Article/details/genmvimdr.sHtML

[T37] Lua：字符串拼接
来源：http://blog.yfazqb.com/Article/details/gxekwqasv.sHtML

"a" .. "b"
来源：http://blog.bbcook.cn/Article/details/gsbzbkhhk.sHtML

[T38] Lua：条件
来源：http://wap.sjlbkw.cn/Article/details/gwqmiamfb.sHtML

if x > 0 then print("正") end
来源：http://3g.epnwcf.com/Article/details/geknhisky.sHtML

[T39] Lua：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/gpbotsxqy.sHtML

string.find(s, "%d+")
来源：http://wap.bbcook.cn/Article/details/gqczyrgsc.sHtML

[T40] Lua：元表
来源：http://wap.sjlbkw.cn/Article/details/gjhakrmzu.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fktsv.cn/Article/details/gvsrgxuor.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/ggmuqetvy.sHtML

print "Hello\n";
来源：http://wap.fktsv.cn/Article/details/gqyytlmvm.sHtML

[T42] Perl：变量类型
来源：http://read.share.vehdjk.com/Article/details/gmlfrupuv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.bbcook.cn/Article/details/ghdecvhrl.sHtML

[T43] Perl：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gbozbogdx.sHtML

"值: $a"
来源：http://3g.tarul.cn/Article/details/gvbvnkqcm.sHtML

[T44] Perl：条件
来源：http://blog.fktsv.cn/Article/details/gatpccikh.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.tarul.cn/Article/details/gvsggytqq.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.epnwcf.com/Article/details/gbklpsfhx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.epnwcf.com/Article/details/gukhadfcw.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.epnwcf.com/Article/details/guthpalcb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.bbcook.cn/Article/details/guchozeho.sHtML

[T47] Perl：正则捕获
来源：http://read.share.yfazqb.com/Article/details/ggflxbxll.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.yfazqb.com/Article/details/gpiwhvcet.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gszfrwcyr.sHtML

$s =~ s/old/new/g;
来源：http://mobile.vehdjk.com/Article/details/gwlrgpilb.sHtML

[T49] Perl：函数
来源：http://wap.sjlbkw.cn/Article/details/giwxrclko.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gxmvuntho.sHtML

[T50] Perl：逐行读文件
来源：http://3g.tarul.cn/Article/details/giguauveh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.epnwcf.com/Article/details/gyucrlggo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.sjlbkw.cn/Article/details/gopaepwff.sHtML

[T51] Scala：Hello World
来源：http://read.share.tarul.cn/Article/details/gbcmtpgil.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gaqukvjoi.sHtML

[T52] Scala：变量
来源：http://m.share.fktsv.cn/Article/details/goovnnior.sHtML

val a = 1;  var b = 2
来源：http://www.share.yfazqb.com/Article/details/gdqzegmmv.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gcecndswi.sHtML

s"值: $b"
来源：http://www.share.vehdjk.com/Article/details/gqavpdpot.sHtML

[T54] Scala：集合映射
来源：http://mobile.fktsv.cn/Article/details/gncqtrfdq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.epnwcf.com/Article/details/gzwfnxdpw.sHtML

[T55] Scala：集合过滤
来源：http://baike.bbcook.cn/Article/details/gqdxuumzx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.bbcook.cn/Article/details/gpzhzammp.sHtML

[T56] Scala：样例类
来源：http://3g.sjlbkw.cn/Article/details/gxaoxlypf.sHtML

case class User(name: String, age: Int)
来源：http://wap.fktsv.cn/Article/details/gpdjlqrsw.sHtML

[T57] Scala：模式匹配
来源：http://www.share.epnwcf.com/Article/details/ghdxlfyhb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.epnwcf.com/Article/details/gekhbwagr.sHtML

[T58] Scala：函数定义
来源：http://www.share.bbcook.cn/Article/details/gnfslrcgk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.tarul.cn/Article/details/gprphapxy.sHtML

[T59] Scala：循环
来源：http://blog.yfazqb.com/Article/details/giibnceeb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gnledsogq.sHtML

[T60] Scala：折叠
来源：http://mobile.fktsv.cn/Article/details/grfwjuthg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.bbcook.cn/Article/details/gxtdovukl.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gksvzvapp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/gjkjymwde.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqtozhkjo.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.epnwcf.com/Article/details/gbhurctba.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.epnwcf.com/Article/details/gecgruwuw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.yfazqb.com/Article/details/gcvihfhqo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.vehdjk.com/Article/details/gdvnbrrbk.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.vehdjk.com/Article/details/gxhaanejl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.epnwcf.com/Article/details/gfrgyvjoq.sHtML

[U04] Py：变量调试打印
来源：http://wap.yfazqb.com/Article/details/gwjqmrucn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.yfazqb.com/Article/details/gjoufqkiy.sHtML

[U05] Py：列表去重且保序
来源：http://blog.bbcook.cn/Article/details/gnufipwyv.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.bbcook.cn/Article/details/ghgcctdxk.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.tarul.cn/Article/details/gjlqftldo.sHtML

{**a, **b}
来源：http://3g.yfazqb.com/Article/details/gatymkthi.sHtML

[U07] Py：反转字典键值
来源：http://m.share.bbcook.cn/Article/details/grulxwtwi.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fktsv.cn/Article/details/gkdpgvmqr.sHtML

[U08] Py：展平二维列表
来源：http://baike.tarul.cn/Article/details/gqriijlbm.sHtML

[y for x in nested for y in x]
来源：http://m.share.bbcook.cn/Article/details/gaapdrdzd.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.sjlbkw.cn/Article/details/gumaxzqok.sHtML

max(d, key=d.get)
来源：http://mobile.tarul.cn/Article/details/gcvseecdv.sHtML

[U10] Py：按值排序字典
来源：http://read.share.vehdjk.com/Article/details/gooccvadv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.bbcook.cn/Article/details/ghyrlczft.sHtML

[U11] Py：生成器表达式
来源：http://www.share.epnwcf.com/Article/details/gikyxnmzo.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fktsv.cn/Article/details/glnwlhsck.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.vehdjk.com/Article/details/gwvecatfd.sHtML

Counter(arr).most_common(3)
来源：http://read.share.vehdjk.com/Article/details/giyzpupaa.sHtML

[U13] Py：固定长度队列
来源：http://m.share.vehdjk.com/Article/details/gvdonwhvn.sHtML

deque(maxlen=10)
来源：http://www.m.share.tarul.cn/Article/details/gwpzndhih.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.tarul.cn/Article/details/girevomrh.sHtML

defaultdict(list)
来源：http://www.share.tarul.cn/Article/details/gghnfcpmu.sHtML

[U15] Py：高精度计时
来源：http://blog.tarul.cn/Article/details/gxazsgobe.sHtML

t = time.perf_counter()
来源：http://www.blog.vehdjk.com/Article/details/grstcnzmg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.bbcook.cn/Article/details/gyxezpfni.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.bbcook.cn/Article/details/guhazdbda.sHtML

[U17] Py：初始化日志
来源：http://mobile.fktsv.cn/Article/details/gutrbworo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.bbcook.cn/Article/details/gmquzgbwb.sHtML

[U18] Py：预编译正则
来源：http://www.share.sjlbkw.cn/Article/details/gnukcqebb.sHtML

pat = re.compile(r"\d+")
来源：http://baike.bbcook.cn/Article/details/gaaukhguw.sHtML

[U19] Py：正则替换带回调
来源：http://blog.sjlbkw.cn/Article/details/gohnfllwm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.vehdjk.com/Article/details/grksijprl.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.yfazqb.com/Article/details/gugbotdwk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.epnwcf.com/Article/details/gvmikgtdu.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fktsv.cn/Article/details/gcztszkky.sHtML

@contextlib.contextmanager
来源：http://blog.fktsv.cn/Article/details/gpjjjougu.sHtML

[U22] Py：矩阵转置
来源：http://baike.sjlbkw.cn/Article/details/gczkpicbn.sHtML

list(zip(*m))
来源：http://blog.epnwcf.com/Article/details/gxlrmbmig.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.vehdjk.com/Article/details/gtuqzfoeu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.sjlbkw.cn/Article/details/gwnnmwqzj.sHtML

[U24] Py：路径操作
来源：http://mobile.fktsv.cn/Article/details/gnjquozsj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gvqnodmzh.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.bbcook.cn/Article/details/gqnebaxiz.sHtML

csv.DictReader(f)
来源：http://baike.tarul.cn/Article/details/gsyzmpanh.sHtML

[U26] Py：并发下载
来源：http://baike.sjlbkw.cn/Article/details/geqpeyvwc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fktsv.cn/Article/details/gqheqoumk.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.vehdjk.com/Article/details/gqmxjrdsx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.vehdjk.com/Article/details/gzkarhewn.sHtML

[U28] Py：类型别名
来源：http://mobile.fktsv.cn/Article/details/gvkaoquyi.sHtML

UserId = int
来源：http://wap.epnwcf.com/Article/details/gefittthe.sHtML

[U29] Py：属性校验
来源：http://blog.sjlbkw.cn/Article/details/gghjmelnt.sHtML

@property 与 @x.setter 配合
来源：http://m.share.epnwcf.com/Article/details/greeukbib.sHtML

[U30] Py：数据类
来源：http://blog.fktsv.cn/Article/details/gyefdgyxa.sHtML

@dataclass(slots=True)
来源：http://3g.vehdjk.com/Article/details/glxrextsg.sHtML

[U31] Py：单测
来源：http://www.blog.tarul.cn/Article/details/gcbjiffbx.sHtML

python -m pytest -q
来源：http://www.blog.vehdjk.com/Article/details/gedfdapch.sHtML

[U32] Py：代码格式化
来源：http://baike.yfazqb.com/Article/details/gicdqhzmn.sHtML

ruff format . && ruff check --fix .
来源：http://blog.yfazqb.com/Article/details/ggtktgglz.sHtML

[U33] Py：打包发布
来源：http://wap.tarul.cn/Article/details/ghgkxtntv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.tarul.cn/Article/details/gnjrquqvw.sHtML

[U34] Py：判断编码
来源：http://mobile.tarul.cn/Article/details/gcfxkkeeg.sHtML

chardet.detect(raw)
来源：http://www.m.share.epnwcf.com/Article/details/gznfssrxo.sHtML

[U35] Py：发送邮件
来源：http://mobile.bbcook.cn/Article/details/gpojzkqnr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.yfazqb.com/Article/details/gkwjcqeap.sHtML

[U36] Py：定时任务
来源：http://www.blog.bbcook.cn/Article/details/gqmuksmxw.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.yfazqb.com/Article/details/gquxzpkni.sHtML

[U37] Py：读写 Excel
来源：http://www.share.epnwcf.com/Article/details/gvmkenkke.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.sjlbkw.cn/Article/details/gzajkzgve.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fktsv.cn/Article/details/gdoxktnkc.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fktsv.cn/Article/details/gpwmivrmb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.epnwcf.com/Article/details/gobyezaom.sHtML

sys.stdout.isatty()
来源：http://wap.fktsv.cn/Article/details/ghivawucj.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.bbcook.cn/Article/details/gvwltshgc.sHtML

print("err", file=sys.stderr)
来源：http://m.share.epnwcf.com/Article/details/gypcugets.sHtML


<!-- 参考信息 -->