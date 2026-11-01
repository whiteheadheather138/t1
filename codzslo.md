代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://wap.tarul.cn/Article/details/guujvqdiq.sHtML

[S15] C：类型转换
来源：http://read.share.yfazqb.com/Article/details/ghiovzllw.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/gewmkegbe.sHtML

[S16] C：位操作置位
来源：http://wap.vehdjk.com/Article/details/gprwfzvzv.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/gowhppmkw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.yfazqb.com/Article/details/gbquxmhbg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/gtxyiywgo.sHtML

[S18] C：命令行参数
来源：http://read.share.epnwcf.com/Article/details/guqwxgcgo.sHtML

int main(int argc, char **argv)
来源：http://3g.bbcook.cn/Article/details/gobbzvalc.sHtML

[S19] C：快速排序
来源：http://read.share.sjlbkw.cn/Article/details/guuafmezx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gjqkppxhx.sHtML

[S20] C：二分查找
来源：http://mobile.bbcook.cn/Article/details/gyfovyltx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gglzheqjv.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/gofarcrua.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fktsv.cn/Article/details/gaqogwgkm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gcsqbhzmo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.bbcook.cn/Article/details/ghvygmvga.sHtML

[S23] C：随机数
来源：http://m.share.bbcook.cn/Article/details/gskenjovq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.vehdjk.com/Article/details/gbvkqiwfg.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/gjhaqxbki.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/gukukzpyv.sHtML

[S25] C：内存拷贝
来源：http://www.blog.yfazqb.com/Article/details/gbzelnllo.sHtML

memcpy(dst, src, n);
来源：http://www.blog.tarul.cn/Article/details/gamqrkfts.sHtML

[S26] C：内存清零
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfydhdct.sHtML

memset(a, 0, sizeof a);
来源：http://wap.epnwcf.com/Article/details/gemgegxmr.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gurjxaxqi.sHtML

const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gfabpmemc.sHtML

[S28] C：静态变量
来源：http://baike.bbcook.cn/Article/details/gmwwciogs.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/gyzwzzzxt.sHtML

[S29] C：变参函数
来源：http://www.share.bbcook.cn/Article/details/ggciseatx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/gsuhjsewm.sHtML

[S30] C：头文件保护
来源：http://mobile.sjlbkw.cn/Article/details/giovkvwup.sHtML

#ifndef X_H
来源：http://wap.tarul.cn/Article/details/gqqxpiqra.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gqwtptjle.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/gmicnmrlf.sHtML

[S31] C++：Hello World
来源：http://3g.yfazqb.com/Article/details/gjeaxmwnx.sHtML

#include <iostream>
来源：http://wap.epnwcf.com/Article/details/gktsabcqx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.tarul.cn/Article/details/gazkigbgm.sHtML

[S32] C++：字符串
来源：http://wap.epnwcf.com/Article/details/geirvyuwz.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.sjlbkw.cn/Article/details/gsbpeavax.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/gbakuhqru.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/girfmkkhw.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.tarul.cn/Article/details/gsnxmfcoi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.vehdjk.com/Article/details/gdremqlzs.sHtML

[S35] C++：map
来源：http://baike.vehdjk.com/Article/details/gymuvevwa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/givbxxzul.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjujpwdl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/ghjgggryi.sHtML

[S37] C++：set
来源：http://3g.bbcook.cn/Article/details/glvhyedgt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.yfazqb.com/Article/details/gryxsxfep.sHtML

[S38] C++：排序
来源：http://baike.tarul.cn/Article/details/ghqjkwqqp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gcqyjuaad.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/girpwicxa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/ghbslpthr.sHtML

[S40] C++：查找元素
来源：http://blog.tarul.cn/Article/details/ggjzkbevm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.bbcook.cn/Article/details/gzvnaleph.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fktsv.cn/Article/details/gcmksdlrq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.tarul.cn/Article/details/gbpaotkno.sHtML

[S42] C++：继承与虚函数
来源：http://3g.vehdjk.com/Article/details/gxzzbcxhv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.tarul.cn/Article/details/gmxvdzmzt.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/gzydhespj.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.vehdjk.com/Article/details/gffgweroh.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/ghzdqciki.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/gylziquiu.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gwoajlrcv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.sjlbkw.cn/Article/details/gytyztxaj.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fktsv.cn/Article/details/gzebekphk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fktsv.cn/Article/details/gatswhnlv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/gccrznoje.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.sjlbkw.cn/Article/details/gtrhbrnzs.sHtML

[S48] C++：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gblxvtapj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.epnwcf.com/Article/details/gmyyesplv.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.vehdjk.com/Article/details/gvroiswxq.sHtML

[S49] C++：写文件
来源：http://mobile.tarul.cn/Article/details/gzfugbpsj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/gqubuozie.sHtML

[S50] C++：格式化数字
来源：http://www.blog.epnwcf.com/Article/details/gdozalezy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gbtzgmjwu.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/gqllujaae.sHtML

static_cast<double>(a) / b
来源：http://www.share.epnwcf.com/Article/details/grdkwwdbh.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.yfazqb.com/Article/details/gbxhvlghl.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.sjlbkw.cn/Article/details/gdwfksjml.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/gydopdlxj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.sjlbkw.cn/Article/details/gssufgfzm.sHtML

[S54] C++：异常处理
来源：http://wap.sjlbkw.cn/Article/details/gpfcmfqsx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fktsv.cn/Article/details/gcdnnwsdj.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/gyfcdqgqq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.epnwcf.com/Article/details/gknpsqkwm.sHtML

[S56] C++：optional
来源：http://m.share.tarul.cn/Article/details/girgdsvfn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.sjlbkw.cn/Article/details/guyspjmyl.sHtML

[S57] C++：编译期常量
来源：http://wap.epnwcf.com/Article/details/ghoutftbp.sHtML

constexpr int N = 10;
来源：http://m.share.yfazqb.com/Article/details/gyclehgxk.sHtML

[S58] C++：命名空间
来源：http://wap.bbcook.cn/Article/details/gjjhenssc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.tarul.cn/Article/details/gvffxfhfc.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gscibjpkv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fktsv.cn/Article/details/gccjbbszz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gueuwalau.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.bbcook.cn/Article/details/galwlfkvo.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfywsnxqn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.sjlbkw.cn/Article/details/gfgplfghs.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gqdiywubg.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/gmawushii.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gwxyuyxpo.sHtML

[T02] Kotlin：变量
来源：http://m.share.fktsv.cn/Article/details/gwemqsmuc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.tarul.cn/Article/details/gaizplauu.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.sjlbkw.cn/Article/details/gdlfpvegm.sHtML

"值: $b"
来源：http://m.share.epnwcf.com/Article/details/gjhngcjsi.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/gimjlcjht.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.yfazqb.com/Article/details/gvmzrysvs.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gauprjajt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.yfazqb.com/Article/details/gpirtrwgd.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fktsv.cn/Article/details/gsrkzikkz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gbrbpwwmd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gqodhtrsl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.tarul.cn/Article/details/geijpzwro.sHtML

[T08] Kotlin：数据类
来源：http://www.share.bbcook.cn/Article/details/gyndtdckr.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fktsv.cn/Article/details/gkmcnadgj.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fktsv.cn/Article/details/ggzyyeozg.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fktsv.cn/Article/details/gawtcvfvi.sHtML

[T10] Kotlin：默认参数
来源：http://baike.epnwcf.com/Article/details/geqpvgeqd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.bbcook.cn/Article/details/gxodnmexq.sHtML

[T11] Kotlin：协程
来源：http://read.share.fktsv.cn/Article/details/gnptxyulg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.bbcook.cn/Article/details/guafekare.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.sjlbkw.cn/Article/details/guxltujci.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.tarul.cn/Article/details/gtsymdbwv.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.yfazqb.com/Article/details/gebxchfui.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/gmbzgnpwa.sHtML

[T14] Kotlin：循环
来源：http://3g.fktsv.cn/Article/details/gzapvtshr.sHtML

for (i in 1..10) println(i)
来源：http://baike.bbcook.cn/Article/details/gifscoevh.sHtML

[T15] Kotlin：接口
来源：http://mobile.yfazqb.com/Article/details/gypvalwhb.sHtML

interface Shape { fun area(): Double }
来源：http://wap.tarul.cn/Article/details/gxkjsmanq.sHtML

[T16] Swift：Hello World
来源：http://mobile.epnwcf.com/Article/details/gbemcqusm.sHtML

print("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gwvehjhsv.sHtML

[T17] Swift：变量与常量
来源：http://baike.tarul.cn/Article/details/gmxcsqdvy.sHtML

var a = 1;  let b = 2
来源：http://3g.sjlbkw.cn/Article/details/gvfooohgc.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/gtcbzmubd.sHtML

"值: \(b)"
来源：http://mobile.sjlbkw.cn/Article/details/gigceeamu.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/gpqqhyaxj.sHtML

if let n = opt { print(n) }
来源：http://m.share.bbcook.cn/Article/details/gmyzntkag.sHtML

[T20] Swift：数组操作
来源：http://3g.bbcook.cn/Article/details/glkmmcvum.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.tarul.cn/Article/details/gwcmdqedf.sHtML

[T21] Swift：遍历
来源：http://wap.sjlbkw.cn/Article/details/gsvgufgew.sHtML

for x in a { print(x) }
来源：http://mobile.tarul.cn/Article/details/gfkoscyio.sHtML

[T22] Swift：字典
来源：http://blog.vehdjk.com/Article/details/gapbmjolt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.yfazqb.com/Article/details/ggofibzov.sHtML

[T23] Swift：函数
来源：http://read.share.vehdjk.com/Article/details/gcelzmyhn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.tarul.cn/Article/details/gvwhpiinf.sHtML

[T24] Swift：闭包
来源：http://baike.fktsv.cn/Article/details/gkktmjswn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gfogmasxx.sHtML

[T25] Swift：结构体
来源：http://www.blog.tarul.cn/Article/details/ghzmoeuoj.sHtML

struct P { var x: Int }
来源：http://www.blog.sjlbkw.cn/Article/details/guushxest.sHtML

[T26] Swift：类与重写
来源：http://read.share.tarul.cn/Article/details/ganydotfb.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gwmcmufmu.sHtML

[T27] Swift：错误处理
来源：http://baike.sjlbkw.cn/Article/details/gmdsoxkuo.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.vehdjk.com/Article/details/gwxnkkdsr.sHtML

[T28] Swift：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gtxbmalmn.sHtML

enum Color { case red, green }
来源：http://blog.vehdjk.com/Article/details/gtxqllrhp.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.tarul.cn/Article/details/gspbzzkay.sHtML

guard let x = opt else { return }
来源：http://www.m.share.bbcook.cn/Article/details/gvllrrynt.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/gqsrtpflp.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.tarul.cn/Article/details/glzihdlcb.sHtML

[T31] Lua：Hello World
来源：http://read.share.epnwcf.com/Article/details/gndzbtufg.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gtefolfor.sHtML

[T32] Lua：局部变量
来源：http://wap.yfazqb.com/Article/details/gpmtoudxu.sHtML

local a = 1
来源：http://m.share.fktsv.cn/Article/details/geowvenpj.sHtML

[T33] Lua：表（数组）
来源：http://mobile.epnwcf.com/Article/details/gvbldhyya.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.yfazqb.com/Article/details/glpkqcwqq.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.tarul.cn/Article/details/grcuothda.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.yfazqb.com/Article/details/gyzefijiy.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fktsv.cn/Article/details/gyasnresn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fktsv.cn/Article/details/gzrkpepjr.sHtML

[T36] Lua：函数
来源：http://mobile.bbcook.cn/Article/details/gttslankk.sHtML

function add(a, b) return a + b end
来源：http://m.share.bbcook.cn/Article/details/gelsghwyl.sHtML

[T37] Lua：字符串拼接
来源：http://baike.vehdjk.com/Article/details/ghisholrb.sHtML

"a" .. "b"
来源：http://3g.bbcook.cn/Article/details/gbaprtijk.sHtML

[T38] Lua：条件
来源：http://www.blog.yfazqb.com/Article/details/gpkocclmz.sHtML

if x > 0 then print("正") end
来源：http://wap.fktsv.cn/Article/details/gahdfprnd.sHtML

[T39] Lua：模式匹配
来源：http://blog.yfazqb.com/Article/details/gusbparcz.sHtML

string.find(s, "%d+")
来源：http://blog.epnwcf.com/Article/details/gtiqqkqsg.sHtML

[T40] Lua：元表
来源：http://read.share.yfazqb.com/Article/details/gatcdxxsf.sHtML

setmetatable({}, { __index = base })
来源：http://3g.vehdjk.com/Article/details/gajnwyuaz.sHtML

[T41] Perl：Hello World
来源：http://read.share.fktsv.cn/Article/details/gcqxgjnfg.sHtML

print "Hello\n";
来源：http://wap.bbcook.cn/Article/details/genwzzimq.sHtML

[T42] Perl：变量类型
来源：http://blog.epnwcf.com/Article/details/gwaryucff.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.bbcook.cn/Article/details/ghkukiyhd.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gmqcmfuhc.sHtML

"值: $a"
来源：http://blog.bbcook.cn/Article/details/gkieeykdg.sHtML

[T44] Perl：条件
来源：http://baike.vehdjk.com/Article/details/gplaqsqwm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.vehdjk.com/Article/details/grjahklni.sHtML

[T45] Perl：数组遍历
来源：http://m.share.bbcook.cn/Article/details/gmswihgsk.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.yfazqb.com/Article/details/gsohetlad.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fktsv.cn/Article/details/gfqtnlcyf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fktsv.cn/Article/details/gcspsyxmf.sHtML

[T47] Perl：正则捕获
来源：http://blog.sjlbkw.cn/Article/details/gsrmusklo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fktsv.cn/Article/details/gbvwmbfsi.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcfhlsih.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fktsv.cn/Article/details/gbmxsqvgz.sHtML

[T49] Perl：函数
来源：http://www.m.share.vehdjk.com/Article/details/gvobixcmi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gvaqdzusc.sHtML

[T50] Perl：逐行读文件
来源：http://blog.tarul.cn/Article/details/ggnxbsrjm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.tarul.cn/Article/details/gdmckkefo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.yfazqb.com/Article/details/gqibkgthj.sHtML

[T51] Scala：Hello World
来源：http://blog.epnwcf.com/Article/details/goruswbwz.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/gvcgbcpri.sHtML

[T52] Scala：变量
来源：http://3g.bbcook.cn/Article/details/gtxblvqas.sHtML

val a = 1;  var b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gdewaeslk.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gtpjcyzuw.sHtML

s"值: $b"
来源：http://mobile.bbcook.cn/Article/details/glbzikflt.sHtML

[T54] Scala：集合映射
来源：http://read.share.yfazqb.com/Article/details/gkblpzwcg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.sjlbkw.cn/Article/details/ggbfrunbu.sHtML

[T55] Scala：集合过滤
来源：http://baike.epnwcf.com/Article/details/gfbgtpnbj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.bbcook.cn/Article/details/geutoaxym.sHtML

[T56] Scala：样例类
来源：http://m.share.tarul.cn/Article/details/gbcvceflx.sHtML

case class User(name: String, age: Int)
来源：http://wap.fktsv.cn/Article/details/gubxybatf.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/gossptuby.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.vehdjk.com/Article/details/glythulgy.sHtML

[T58] Scala：函数定义
来源：http://www.blog.tarul.cn/Article/details/gavegbykl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.yfazqb.com/Article/details/gimjvckxw.sHtML

[T59] Scala：循环
来源：http://wap.tarul.cn/Article/details/gzpqwdeuc.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gjbmbykwe.sHtML

[T60] Scala：折叠
来源：http://wap.sjlbkw.cn/Article/details/gfwzukkxo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fktsv.cn/Article/details/gqockmquu.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqkgbmknd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/guibxfnqy.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/geacsnoth.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/gtzsmcees.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.yfazqb.com/Article/details/gxbofywqk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.vehdjk.com/Article/details/ggbmoutiu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gbbevgwwm.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.epnwcf.com/Article/details/gupotfksy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.vehdjk.com/Article/details/gtznhgrir.sHtML

[U04] Py：变量调试打印
来源：http://www.share.epnwcf.com/Article/details/gsohocyqb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.sjlbkw.cn/Article/details/gwwekufzz.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fktsv.cn/Article/details/gqwfjknoz.sHtML

list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/ggbvwwujv.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.yfazqb.com/Article/details/geirnnltq.sHtML

{**a, **b}
来源：http://read.share.bbcook.cn/Article/details/gcfnmciox.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fktsv.cn/Article/details/ghotxojuw.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.sjlbkw.cn/Article/details/grljarexw.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.bbcook.cn/Article/details/gwzycjqje.sHtML

[y for x in nested for y in x]
来源：http://www.blog.yfazqb.com/Article/details/gkautgppd.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fktsv.cn/Article/details/gfdibegzr.sHtML

max(d, key=d.get)
来源：http://read.share.bbcook.cn/Article/details/gunwryoaw.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fktsv.cn/Article/details/ggriylovq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fktsv.cn/Article/details/glnuzibfj.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fktsv.cn/Article/details/ggsimdtaf.sHtML

(x * 2 for x in arr)
来源：http://baike.fktsv.cn/Article/details/gpbgsmzti.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.yfazqb.com/Article/details/gamcdqcsm.sHtML

Counter(arr).most_common(3)
来源：http://baike.sjlbkw.cn/Article/details/gxbcpkgxo.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.epnwcf.com/Article/details/gcgqsycto.sHtML

deque(maxlen=10)
来源：http://blog.vehdjk.com/Article/details/gwcccqcpz.sHtML

[U14] Py：分组收集到列表
来源：http://wap.epnwcf.com/Article/details/ggrvlzdki.sHtML

defaultdict(list)
来源：http://www.share.tarul.cn/Article/details/gsdtqpgyr.sHtML

[U15] Py：高精度计时
来源：http://m.share.fktsv.cn/Article/details/grmzlfgux.sHtML

t = time.perf_counter()
来源：http://www.share.yfazqb.com/Article/details/gcsibktbn.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.epnwcf.com/Article/details/gvmtqalgp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fktsv.cn/Article/details/gsxmmzedp.sHtML

[U17] Py：初始化日志
来源：http://3g.tarul.cn/Article/details/guuasztqv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fktsv.cn/Article/details/gyuzycxka.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.yfazqb.com/Article/details/gghxejwpn.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fktsv.cn/Article/details/gjlufcrqy.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.epnwcf.com/Article/details/gheoiwapw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.bbcook.cn/Article/details/gnnvcazpo.sHtML

[U20] Py：缓存函数结果
来源：http://wap.epnwcf.com/Article/details/gihohrsoj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.sjlbkw.cn/Article/details/gqafatrio.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.epnwcf.com/Article/details/gcmnezkhu.sHtML

@contextlib.contextmanager
来源：http://blog.fktsv.cn/Article/details/gyjvkbzrn.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fktsv.cn/Article/details/gkdlgogip.sHtML

list(zip(*m))
来源：http://blog.fktsv.cn/Article/details/grjhxhltv.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fktsv.cn/Article/details/guyetsrsa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.sjlbkw.cn/Article/details/ghnsenxlo.sHtML

[U24] Py：路径操作
来源：http://www.share.tarul.cn/Article/details/gaquyknpa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gtzzhmgji.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.sjlbkw.cn/Article/details/gidramfwk.sHtML

csv.DictReader(f)
来源：http://m.share.bbcook.cn/Article/details/gporfdxtl.sHtML

[U26] Py：并发下载
来源：http://www.m.share.yfazqb.com/Article/details/gmjcihcvq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fktsv.cn/Article/details/gxosfytmt.sHtML

[U27] Py：异步 HTTP
来源：http://3g.sjlbkw.cn/Article/details/gtzwbjdag.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.yfazqb.com/Article/details/gingpmdmv.sHtML

[U28] Py：类型别名
来源：http://www.share.vehdjk.com/Article/details/gipepbpqf.sHtML

UserId = int
来源：http://baike.fktsv.cn/Article/details/ggyxfcnyx.sHtML

[U29] Py：属性校验
来源：http://www.blog.vehdjk.com/Article/details/gyysvqcqt.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.epnwcf.com/Article/details/geeoxftks.sHtML

[U30] Py：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/gijpwtles.sHtML

@dataclass(slots=True)
来源：http://www.m.share.vehdjk.com/Article/details/gexykmmxk.sHtML

[U31] Py：单测
来源：http://m.share.epnwcf.com/Article/details/gigksxzmj.sHtML

python -m pytest -q
来源：http://wap.vehdjk.com/Article/details/grtljokra.sHtML

[U32] Py：代码格式化
来源：http://3g.epnwcf.com/Article/details/grjjvlhcv.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.bbcook.cn/Article/details/gyofuaapv.sHtML

[U33] Py：打包发布
来源：http://blog.fktsv.cn/Article/details/govzsqqky.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.vehdjk.com/Article/details/gshlfwdkm.sHtML

[U34] Py：判断编码
来源：http://wap.vehdjk.com/Article/details/gkrquwixi.sHtML

chardet.detect(raw)
来源：http://baike.sjlbkw.cn/Article/details/gxoqgjahl.sHtML

[U35] Py：发送邮件
来源：http://mobile.bbcook.cn/Article/details/gmjzrvtja.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.tarul.cn/Article/details/gzpgwfzrx.sHtML

[U36] Py：定时任务
来源：http://3g.yfazqb.com/Article/details/giymsbjdw.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fktsv.cn/Article/details/gfmqjujzb.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.vehdjk.com/Article/details/gmhfkaskc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.epnwcf.com/Article/details/gesqipkhx.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfvhgufw.sHtML

Path(__file__).resolve().parent
来源：http://www.share.tarul.cn/Article/details/grgqmfino.sHtML


<!-- 参考信息 -->