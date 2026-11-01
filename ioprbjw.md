代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://read.share.epnwcf.com/Article/details/gbuofczse.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gjwavdwkj.sHtML

(double) a / b
来源：http://www.m.share.yfazqb.com/Article/details/ghzvwdkgc.sHtML

[S16] C：位操作置位
来源：http://m.share.tarul.cn/Article/details/gnueubtsb.sHtML

x |= (1 << 3);
来源：http://www.share.tarul.cn/Article/details/gjnrywqls.sHtML

[S17] C：安全拼接字符串
来源：http://3g.yfazqb.com/Article/details/ghnaaaffw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.bbcook.cn/Article/details/gqmowpipq.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/gzfbwjyta.sHtML

int main(int argc, char **argv)
来源：http://www.share.fktsv.cn/Article/details/grjmdzuqb.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/gpuhgbprw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gidfvgwiw.sHtML

[S20] C：二分查找
来源：http://read.share.epnwcf.com/Article/details/gpyzomrqx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/gzsroqujj.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/gquclyxqe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.sjlbkw.cn/Article/details/gybrhhido.sHtML

[S22] C：字符串转数字
来源：http://blog.vehdjk.com/Article/details/gwrhqfwuh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gszugbnsg.sHtML

[S23] C：随机数
来源：http://mobile.vehdjk.com/Article/details/gwiwqgcun.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.yfazqb.com/Article/details/gclljmbde.sHtML

[S24] C：获取本地时间
来源：http://m.share.tarul.cn/Article/details/glhtygdgf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/ggoklkqgt.sHtML

[S25] C：内存拷贝
来源：http://m.share.fktsv.cn/Article/details/gvsasfhtj.sHtML

memcpy(dst, src, n);
来源：http://www.share.yfazqb.com/Article/details/gdqbayvmv.sHtML

[S26] C：内存清零
来源：http://baike.yfazqb.com/Article/details/gkneryqhi.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjagwoyqo.sHtML

[S27] C：定义常量
来源：http://www.share.sjlbkw.cn/Article/details/gjeydqyxj.sHtML

const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gqtzwxtjl.sHtML

[S28] C：静态变量
来源：http://www.blog.epnwcf.com/Article/details/gurbvaena.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/gdtfrozjq.sHtML

[S29] C：变参函数
来源：http://mobile.sjlbkw.cn/Article/details/gjnspcegk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.bbcook.cn/Article/details/gahfizspc.sHtML

[S30] C：头文件保护
来源：http://www.share.sjlbkw.cn/Article/details/gjeirspiu.sHtML

#ifndef X_H
来源：http://www.blog.yfazqb.com/Article/details/gpwcvhyoe.sHtML

#define X_H
来源：http://www.share.fktsv.cn/Article/details/gourzrnkj.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gktsmpmrc.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/gyoorayng.sHtML

#include <iostream>
来源：http://3g.tarul.cn/Article/details/gkhjxwhld.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.bbcook.cn/Article/details/gvycmuxak.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gmwbepwjw.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/glzdedudf.sHtML

[S33] C++：vector 增删
来源：http://read.share.bbcook.cn/Article/details/gnyipfxou.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fktsv.cn/Article/details/gptwhknfs.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/ggjdfhcac.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.bbcook.cn/Article/details/gfysnnqzc.sHtML

[S35] C++：map
来源：http://www.m.share.yfazqb.com/Article/details/ggezlvewj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gepvpvxwe.sHtML

[S36] C++：unordered_map
来源：http://blog.yfazqb.com/Article/details/gsxohrnkq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/gjgggmtuz.sHtML

[S37] C++：set
来源：http://read.share.sjlbkw.cn/Article/details/gahjnskjj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.vehdjk.com/Article/details/gfyzlggfs.sHtML

[S38] C++：排序
来源：http://www.m.share.yfazqb.com/Article/details/gwtnrejrj.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.epnwcf.com/Article/details/gdiqxitci.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/gkenyumla.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.bbcook.cn/Article/details/giqamfdra.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/grxnddork.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/gfumxfvii.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/ghicsihyu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/gkblcssgi.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fktsv.cn/Article/details/gldwjkhza.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.sjlbkw.cn/Article/details/gsorurtih.sHtML

[S43] C++：智能指针
来源：http://3g.sjlbkw.cn/Article/details/gtxmlchqx.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fktsv.cn/Article/details/gumtoqopu.sHtML

[S44] C++：引用传参
来源：http://3g.bbcook.cn/Article/details/gnsbhmdzq.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.sjlbkw.cn/Article/details/ggiaxztyo.sHtML

[S45] C++：lambda
来源：http://read.share.yfazqb.com/Article/details/goulqrqpq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.epnwcf.com/Article/details/gktqegbkw.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/gtqeawsya.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.bbcook.cn/Article/details/ggnaravnk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.sjlbkw.cn/Article/details/gionkjagh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fktsv.cn/Article/details/gqlqmoglu.sHtML

[S48] C++：逐行读文件
来源：http://wap.vehdjk.com/Article/details/ghbpnngiy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gvizdvqvy.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.epnwcf.com/Article/details/grqjlkmxt.sHtML

[S49] C++：写文件
来源：http://mobile.vehdjk.com/Article/details/gztoawbjs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/gjnpyycnd.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/gxzavafba.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.tarul.cn/Article/details/ghomstnvh.sHtML

[S51] C++：显式类型转换
来源：http://mobile.yfazqb.com/Article/details/goxwmobjr.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/gkjubkqzl.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fktsv.cn/Article/details/gticvnlpn.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/gpznagopd.sHtML

[S53] C++：移动语义
来源：http://baike.sjlbkw.cn/Article/details/gibbcamhc.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/gkroarylt.sHtML

[S54] C++：异常处理
来源：http://m.share.fktsv.cn/Article/details/gsvehllsh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.epnwcf.com/Article/details/gmtgnvmsb.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fktsv.cn/Article/details/gvejqlvpu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/gaatvdxnm.sHtML

[S56] C++：optional
来源：http://3g.epnwcf.com/Article/details/gtwqybkka.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.sjlbkw.cn/Article/details/glsxvujwj.sHtML

[S57] C++：编译期常量
来源：http://read.share.yfazqb.com/Article/details/gdsilnwwb.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/gjmdcxdla.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/gitkzozci.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.sjlbkw.cn/Article/details/gsdnogony.sHtML

[S59] C++：静态断言
来源：http://read.share.bbcook.cn/Article/details/gddpyxnja.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.yfazqb.com/Article/details/gtuhpgskj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.epnwcf.com/Article/details/ggsqgyyux.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.bbcook.cn/Article/details/gpaxmakwx.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxdcynymb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gnsnvofgn.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gmtkmmqzp.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.epnwcf.com/Article/details/gvykovmxq.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gcxkbjbci.sHtML

[T02] Kotlin：变量
来源：http://m.share.tarul.cn/Article/details/ghknfgkqk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fktsv.cn/Article/details/gjmzeqgoy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gchlchrom.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gwvavqzny.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/gdnqyjppw.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/ggsvhtfyc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gcwiwevdj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.tarul.cn/Article/details/gjbknfgdg.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gfeollydy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.epnwcf.com/Article/details/gbgckisce.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fktsv.cn/Article/details/giaghwvvl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/grvakkgzq.sHtML

[T08] Kotlin：数据类
来源：http://wap.tarul.cn/Article/details/gakpwwztg.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.epnwcf.com/Article/details/gvzlkqspn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.tarul.cn/Article/details/gyetyidiz.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.sjlbkw.cn/Article/details/gpgpplvjt.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.yfazqb.com/Article/details/gmndkabsv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.sjlbkw.cn/Article/details/gpjqjofbe.sHtML

[T11] Kotlin：协程
来源：http://www.blog.yfazqb.com/Article/details/gjemdtkti.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.epnwcf.com/Article/details/gsvgmrzyo.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fktsv.cn/Article/details/gvbklvnij.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.epnwcf.com/Article/details/ggxchvdxf.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fktsv.cn/Article/details/gljzytaes.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.bbcook.cn/Article/details/gtshknvbo.sHtML

[T14] Kotlin：循环
来源：http://3g.fktsv.cn/Article/details/gsmhgczjc.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gjqrdowdc.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.bbcook.cn/Article/details/gqobqeydj.sHtML

interface Shape { fun area(): Double }
来源：http://baike.epnwcf.com/Article/details/gimsxeolm.sHtML

[T16] Swift：Hello World
来源：http://blog.vehdjk.com/Article/details/gjpbizwds.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gkybrtzqd.sHtML

[T17] Swift：变量与常量
来源：http://mobile.epnwcf.com/Article/details/gcstowqcx.sHtML

var a = 1;  let b = 2
来源：http://www.share.bbcook.cn/Article/details/gchmturlu.sHtML

[T18] Swift：字符串插值
来源：http://3g.epnwcf.com/Article/details/gvltxysyv.sHtML

"值: \(b)"
来源：http://www.blog.sjlbkw.cn/Article/details/gsrhdtulo.sHtML

[T19] Swift：可选绑定
来源：http://3g.bbcook.cn/Article/details/gomzkiecy.sHtML

if let n = opt { print(n) }
来源：http://mobile.epnwcf.com/Article/details/gdknejlhq.sHtML

[T20] Swift：数组操作
来源：http://wap.fktsv.cn/Article/details/gtvsgjgll.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.epnwcf.com/Article/details/gqtwskxlf.sHtML

[T21] Swift：遍历
来源：http://3g.bbcook.cn/Article/details/gnutrtplj.sHtML

for x in a { print(x) }
来源：http://m.share.vehdjk.com/Article/details/giluuifkz.sHtML

[T22] Swift：字典
来源：http://3g.yfazqb.com/Article/details/gxcqanmgc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.yfazqb.com/Article/details/gzghgpgwj.sHtML

[T23] Swift：函数
来源：http://wap.yfazqb.com/Article/details/gipldejou.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.tarul.cn/Article/details/gulrgerdg.sHtML

[T24] Swift：闭包
来源：http://wap.bbcook.cn/Article/details/gfvxfwpvu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.tarul.cn/Article/details/gqfkggulv.sHtML

[T25] Swift：结构体
来源：http://www.m.share.vehdjk.com/Article/details/gmydfiyqk.sHtML

struct P { var x: Int }
来源：http://3g.tarul.cn/Article/details/gsjuqoyod.sHtML

[T26] Swift：类与重写
来源：http://m.share.bbcook.cn/Article/details/giczgfwoo.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fktsv.cn/Article/details/gpxqlflcg.sHtML

[T27] Swift：错误处理
来源：http://baike.yfazqb.com/Article/details/gcixgmovp.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fktsv.cn/Article/details/gpbdieulm.sHtML

[T28] Swift：枚举
来源：http://baike.tarul.cn/Article/details/gambuvwau.sHtML

enum Color { case red, green }
来源：http://read.share.tarul.cn/Article/details/gfzjqbamp.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.epnwcf.com/Article/details/gtmujmlne.sHtML

guard let x = opt else { return }
来源：http://mobile.bbcook.cn/Article/details/gdrelgsbq.sHtML

[T30] Swift：协议
来源：http://3g.vehdjk.com/Article/details/gjanhoqzc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fktsv.cn/Article/details/gtyskjtlq.sHtML

[T31] Lua：Hello World
来源：http://www.share.fktsv.cn/Article/details/giwlngwgb.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gfhyrxear.sHtML

[T32] Lua：局部变量
来源：http://www.blog.tarul.cn/Article/details/grlyahwfq.sHtML

local a = 1
来源：http://baike.yfazqb.com/Article/details/grrpucgyu.sHtML

[T33] Lua：表（数组）
来源：http://mobile.tarul.cn/Article/details/gasptksnk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.tarul.cn/Article/details/gjdammolr.sHtML

[T34] Lua：遍历表
来源：http://baike.sjlbkw.cn/Article/details/gskyqqrlp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.yfazqb.com/Article/details/gnowwcfrz.sHtML

[T35] Lua：字典表
来源：http://m.share.vehdjk.com/Article/details/gyznrvrnd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.bbcook.cn/Article/details/gncmxxijs.sHtML

[T36] Lua：函数
来源：http://3g.sjlbkw.cn/Article/details/grpjhgyns.sHtML

function add(a, b) return a + b end
来源：http://mobile.bbcook.cn/Article/details/gfrtvkjfc.sHtML

[T37] Lua：字符串拼接
来源：http://3g.epnwcf.com/Article/details/ghimdrslu.sHtML

"a" .. "b"
来源：http://blog.yfazqb.com/Article/details/guygognzv.sHtML

[T38] Lua：条件
来源：http://mobile.bbcook.cn/Article/details/gshcddxct.sHtML

if x > 0 then print("正") end
来源：http://mobile.yfazqb.com/Article/details/gyiwgudgq.sHtML

[T39] Lua：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/gtkterhch.sHtML

string.find(s, "%d+")
来源：http://www.blog.vehdjk.com/Article/details/gwictsbxl.sHtML

[T40] Lua：元表
来源：http://wap.yfazqb.com/Article/details/givufmejy.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.epnwcf.com/Article/details/gavilguli.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/gusrrecnf.sHtML

print "Hello\n";
来源：http://m.share.yfazqb.com/Article/details/glwshzcwe.sHtML

[T42] Perl：变量类型
来源：http://mobile.yfazqb.com/Article/details/ggvfjgogw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.bbcook.cn/Article/details/gwsabnmof.sHtML

[T43] Perl：字符串插值
来源：http://wap.fktsv.cn/Article/details/gtzfsphka.sHtML

"值: $a"
来源：http://wap.tarul.cn/Article/details/gagaimfrt.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/gzkenuodr.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.yfazqb.com/Article/details/gxgvyifbx.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gfosrwmjk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.epnwcf.com/Article/details/gfeagpmvc.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.tarul.cn/Article/details/gxorllfni.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.vehdjk.com/Article/details/gjcgyuyje.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.tarul.cn/Article/details/ggvhxqvxi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.yfazqb.com/Article/details/gkqvceeld.sHtML

[T48] Perl：正则替换
来源：http://3g.epnwcf.com/Article/details/galkhtpfg.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/gyrhqwgkc.sHtML

[T49] Perl：函数
来源：http://www.share.tarul.cn/Article/details/glfdrzryj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gmebylufi.sHtML

[T50] Perl：逐行读文件
来源：http://baike.epnwcf.com/Article/details/geoitclgt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/gcatvsnam.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.vehdjk.com/Article/details/gchsbqkxc.sHtML

[T51] Scala：Hello World
来源：http://blog.epnwcf.com/Article/details/gdwagewhv.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gozwecudl.sHtML

[T52] Scala：变量
来源：http://www.share.bbcook.cn/Article/details/gvpeukmwz.sHtML

val a = 1;  var b = 2
来源：http://mobile.fktsv.cn/Article/details/gicikbbpy.sHtML

[T53] Scala：字符串插值
来源：http://baike.vehdjk.com/Article/details/gfblynxok.sHtML

s"值: $b"
来源：http://mobile.epnwcf.com/Article/details/gfqkfkjql.sHtML

[T54] Scala：集合映射
来源：http://www.share.tarul.cn/Article/details/geeiviwrf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.epnwcf.com/Article/details/gpiowkkuc.sHtML

[T55] Scala：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gwpygugdg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.tarul.cn/Article/details/gbbfhrgup.sHtML

[T56] Scala：样例类
来源：http://wap.yfazqb.com/Article/details/gxpjaxfvn.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.bbcook.cn/Article/details/ggmasoafr.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fktsv.cn/Article/details/gnekitdos.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.tarul.cn/Article/details/glilekksb.sHtML

[T58] Scala：函数定义
来源：http://www.share.vehdjk.com/Article/details/gjpeousio.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.epnwcf.com/Article/details/gsxejmycr.sHtML

[T59] Scala：循环
来源：http://www.share.sjlbkw.cn/Article/details/gqniovpyo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gcaqvswxd.sHtML

[T60] Scala：折叠
来源：http://m.share.tarul.cn/Article/details/gyjwduyub.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.bbcook.cn/Article/details/gexfdyqcf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnkaxwtvm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gbtfabqot.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsvldisgc.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.epnwcf.com/Article/details/ghumxixvd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.sjlbkw.cn/Article/details/gvfxycocs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fktsv.cn/Article/details/gwmkgrbhw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.sjlbkw.cn/Article/details/gpzicvped.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.tarul.cn/Article/details/grpkifugi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.vehdjk.com/Article/details/gylfrfeas.sHtML

[U04] Py：变量调试打印
来源：http://3g.bbcook.cn/Article/details/graprxqwn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.tarul.cn/Article/details/grwdbpaxm.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.epnwcf.com/Article/details/gonxqufja.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gqoruelye.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.yfazqb.com/Article/details/gdyindcmu.sHtML

{**a, **b}
来源：http://baike.vehdjk.com/Article/details/gbjhjvpej.sHtML

[U07] Py：反转字典键值
来源：http://www.share.yfazqb.com/Article/details/gdeozkmxb.sHtML

{v: k for k, v in d.items()}
来源：http://baike.epnwcf.com/Article/details/gxtkuwfvm.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/geyfmxfot.sHtML

[y for x in nested for y in x]
来源：http://3g.sjlbkw.cn/Article/details/gigrlpwlr.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.vehdjk.com/Article/details/gfouibapf.sHtML

max(d, key=d.get)
来源：http://mobile.fktsv.cn/Article/details/gjanuqmui.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.bbcook.cn/Article/details/gwqunlbnb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.yfazqb.com/Article/details/ggvcjtztm.sHtML

[U11] Py：生成器表达式
来源：http://wap.epnwcf.com/Article/details/ggjbbuxxb.sHtML

(x * 2 for x in arr)
来源：http://mobile.epnwcf.com/Article/details/gdqdhwqdp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.vehdjk.com/Article/details/gjghdgiqc.sHtML

Counter(arr).most_common(3)
来源：http://m.share.yfazqb.com/Article/details/gejxjoefy.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fktsv.cn/Article/details/gdnmhmtlc.sHtML

deque(maxlen=10)
来源：http://baike.yfazqb.com/Article/details/grwiscirz.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.yfazqb.com/Article/details/gjiveklpu.sHtML

defaultdict(list)
来源：http://wap.sjlbkw.cn/Article/details/gxfkvwmpd.sHtML

[U15] Py：高精度计时
来源：http://mobile.fktsv.cn/Article/details/gpszordnm.sHtML

t = time.perf_counter()
来源：http://m.share.sjlbkw.cn/Article/details/gzmxpryqd.sHtML

[U16] Py：命令行参数解析
来源：http://baike.bbcook.cn/Article/details/gwranuosk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.yfazqb.com/Article/details/gcxvudodo.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.yfazqb.com/Article/details/gaaqqiigb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.epnwcf.com/Article/details/gimfiuzmf.sHtML

[U18] Py：预编译正则
来源：http://www.blog.yfazqb.com/Article/details/gsmbbwoxu.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.epnwcf.com/Article/details/grknsgdtg.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fktsv.cn/Article/details/gfcjzzkqi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fktsv.cn/Article/details/ggmuqbkof.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.tarul.cn/Article/details/gzulspnmh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.vehdjk.com/Article/details/ggkkiysad.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.tarul.cn/Article/details/graprttpp.sHtML

@contextlib.contextmanager
来源：http://m.share.epnwcf.com/Article/details/gtfaqkylx.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.yfazqb.com/Article/details/glogvupkw.sHtML

list(zip(*m))
来源：http://wap.bbcook.cn/Article/details/gesmmndmk.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fktsv.cn/Article/details/guwugydsq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.bbcook.cn/Article/details/gzeaosfcz.sHtML

[U24] Py：路径操作
来源：http://www.blog.vehdjk.com/Article/details/gjmjkjxvy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/gviaqbrfw.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/gvlhiajfh.sHtML

csv.DictReader(f)
来源：http://m.share.tarul.cn/Article/details/gvmqbnqrd.sHtML

[U26] Py：并发下载
来源：http://3g.bbcook.cn/Article/details/gtkigxxsw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.yfazqb.com/Article/details/gmvsmdxzq.sHtML

[U27] Py：异步 HTTP
来源：http://baike.bbcook.cn/Article/details/gywaabnzx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.vehdjk.com/Article/details/ggdoadafc.sHtML

[U28] Py：类型别名
来源：http://blog.bbcook.cn/Article/details/gerjgyfhn.sHtML

UserId = int
来源：http://www.blog.bbcook.cn/Article/details/gmaolmdhp.sHtML

[U29] Py：属性校验
来源：http://m.share.epnwcf.com/Article/details/gozzbhyeb.sHtML

@property 与 @x.setter 配合
来源：http://read.share.sjlbkw.cn/Article/details/grpbtukac.sHtML

[U30] Py：数据类
来源：http://m.share.tarul.cn/Article/details/ghfbixpgh.sHtML

@dataclass(slots=True)
来源：http://www.share.bbcook.cn/Article/details/gulmptxsa.sHtML

[U31] Py：单测
来源：http://www.blog.tarul.cn/Article/details/gvhaabfch.sHtML

python -m pytest -q
来源：http://www.blog.sjlbkw.cn/Article/details/gybfstmhd.sHtML

[U32] Py：代码格式化
来源：http://baike.fktsv.cn/Article/details/gqryjkzsn.sHtML

ruff format . && ruff check --fix .
来源：http://3g.sjlbkw.cn/Article/details/gjpntulov.sHtML

[U33] Py：打包发布
来源：http://www.m.share.bbcook.cn/Article/details/gtiyrakmo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.yfazqb.com/Article/details/gfsknuqna.sHtML

[U34] Py：判断编码
来源：http://www.share.fktsv.cn/Article/details/gvtbdngew.sHtML

chardet.detect(raw)
来源：http://www.m.share.epnwcf.com/Article/details/gncvkzjvn.sHtML

[U35] Py：发送邮件
来源：http://blog.yfazqb.com/Article/details/gajrqhbdq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fktsv.cn/Article/details/gyxaulgfp.sHtML

[U36] Py：定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gdgfcpcxm.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.sjlbkw.cn/Article/details/gsjqbbbqp.sHtML

[U37] Py：读写 Excel
来源：http://read.share.sjlbkw.cn/Article/details/grzhcfydp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fktsv.cn/Article/details/gyfmcusdx.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.bbcook.cn/Article/details/gkmfwxtxn.sHtML

Path(__file__).resolve().parent
来源：http://www.share.epnwcf.com/Article/details/gjfpzjgmc.sHtML


<!-- 参考信息 -->