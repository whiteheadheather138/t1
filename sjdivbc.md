代发 wailian999

x |= (1 << 3);
来源：http://wap.tarul.cn/Article/details/gyzwfwtiv.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.tarul.cn/Article/details/gvzbcjksw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.bbcook.cn/Article/details/gfbsefcwz.sHtML

[S18] C：命令行参数
来源：http://baike.yfazqb.com/Article/details/gxxdcabyk.sHtML

int main(int argc, char **argv)
来源：http://www.share.bbcook.cn/Article/details/gnfzpncmb.sHtML

[S19] C：快速排序
来源：http://read.share.bbcook.cn/Article/details/gxdgggmoc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gwvbmdadw.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/gtdjyesdn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gsjdvatjg.sHtML

[S21] C：字符类别判断
来源：http://m.share.bbcook.cn/Article/details/gbzeqgzrm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/giyppurxb.sHtML

[S22] C：字符串转数字
来源：http://www.share.tarul.cn/Article/details/gctcuzrfp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fktsv.cn/Article/details/gjbavnyxq.sHtML

[S23] C：随机数
来源：http://www.blog.sjlbkw.cn/Article/details/gknmxcryx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.bbcook.cn/Article/details/gnfloyigf.sHtML

[S24] C：获取本地时间
来源：http://blog.yfazqb.com/Article/details/gzybjcyyx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fktsv.cn/Article/details/gvjmohjhc.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gwcbpsztq.sHtML

memcpy(dst, src, n);
来源：http://read.share.yfazqb.com/Article/details/gpqswvpsd.sHtML

[S26] C：内存清零
来源：http://m.share.yfazqb.com/Article/details/ghhmrxbdm.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gowwumpxl.sHtML

[S27] C：定义常量
来源：http://baike.yfazqb.com/Article/details/gdmtyttcc.sHtML

const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gpsctepeu.sHtML

[S28] C：静态变量
来源：http://baike.sjlbkw.cn/Article/details/giojqgzlg.sHtML

static int counter = 0;
来源：http://blog.vehdjk.com/Article/details/gxwbplwth.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/gkfvdjqaf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.bbcook.cn/Article/details/gnfzmbkuj.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/gkirswuot.sHtML

#ifndef X_H
来源：http://3g.epnwcf.com/Article/details/gnyjzouyy.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/gydcmguhs.sHtML

#endif
来源：http://m.share.sjlbkw.cn/Article/details/ggmcfpkgl.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/gmvkhbzax.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/glcpixfuv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gcqnybrio.sHtML

[S32] C++：字符串
来源：http://read.share.bbcook.cn/Article/details/gnfxgbhtt.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fktsv.cn/Article/details/gzwfudtyj.sHtML

[S33] C++：vector 增删
来源：http://m.share.yfazqb.com/Article/details/gcmdsxcln.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gupbttfkv.sHtML

[S34] C++：遍历 vector
来源：http://baike.vehdjk.com/Article/details/gyfibatsx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.epnwcf.com/Article/details/gytesekpx.sHtML

[S35] C++：map
来源：http://www.blog.fktsv.cn/Article/details/ghkqytdng.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/grcjyvcwr.sHtML

[S36] C++：unordered_map
来源：http://read.share.tarul.cn/Article/details/grsvmlxvv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gpsslahah.sHtML

[S37] C++：set
来源：http://wap.vehdjk.com/Article/details/gwreucfip.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.tarul.cn/Article/details/gxuqaqhyx.sHtML

[S38] C++：排序
来源：http://www.m.share.fktsv.cn/Article/details/gubrtgivi.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fktsv.cn/Article/details/gobyroqyc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.yfazqb.com/Article/details/ghisfgvwl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.sjlbkw.cn/Article/details/gevxghkoo.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/gdvqzgexl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.sjlbkw.cn/Article/details/gvntrbggb.sHtML

[S41] C++：类与构造函数
来源：http://www.share.epnwcf.com/Article/details/gylnwcvhc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/gzijrcexc.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.bbcook.cn/Article/details/gqhujzvfh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fktsv.cn/Article/details/gbelxmpnq.sHtML

[S43] C++：智能指针
来源：http://m.share.yfazqb.com/Article/details/gloclehwp.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/gkloajpkk.sHtML

[S44] C++：引用传参
来源：http://blog.tarul.cn/Article/details/geffnhoqs.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.epnwcf.com/Article/details/goyghygju.sHtML

[S45] C++：lambda
来源：http://mobile.bbcook.cn/Article/details/guyxmecpj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.sjlbkw.cn/Article/details/gvkongodx.sHtML

[S46] C++：函数模板
来源：http://www.share.epnwcf.com/Article/details/gibnjxkgb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fktsv.cn/Article/details/gpcqastwq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gyjvvebow.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.yfazqb.com/Article/details/gwazjcmfy.sHtML

[S48] C++：逐行读文件
来源：http://read.share.tarul.cn/Article/details/ggeltxydq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.vehdjk.com/Article/details/grfnjkawb.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/gvkdjfrip.sHtML

[S49] C++：写文件
来源：http://mobile.tarul.cn/Article/details/gyddrtnhe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/gcnemzvtv.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gyxkdzgbs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.bbcook.cn/Article/details/grbjrqxlx.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fktsv.cn/Article/details/gadqxskli.sHtML

static_cast<double>(a) / b
来源：http://baike.tarul.cn/Article/details/gsiagbsby.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fktsv.cn/Article/details/gvqntuqyx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.yfazqb.com/Article/details/glnsogdks.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/gndpbvyeo.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.vehdjk.com/Article/details/gxkkytgtz.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/gcjiurtby.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.vehdjk.com/Article/details/grtleijob.sHtML

[S55] C++：结构化绑定
来源：http://wap.tarul.cn/Article/details/gnomoqnep.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.tarul.cn/Article/details/gcejkdywi.sHtML

[S56] C++：optional
来源：http://wap.fktsv.cn/Article/details/ggspfnimp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.epnwcf.com/Article/details/gmfusmjra.sHtML

[S57] C++：编译期常量
来源：http://baike.yfazqb.com/Article/details/gmlpqmhre.sHtML

constexpr int N = 10;
来源：http://3g.bbcook.cn/Article/details/gvnlpahzh.sHtML

[S58] C++：命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gmdrtacld.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/gsnrvtrvx.sHtML

[S59] C++：静态断言
来源：http://read.share.yfazqb.com/Article/details/gizetyqpf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.vehdjk.com/Article/details/gddupowbh.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gycwqjjla.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.tarul.cn/Article/details/giqyniefc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gfadsmcig.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/grxqbaced.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtcmrpcvc.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gwwqdpcqh.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/ghdcnapnc.sHtML

[T02] Kotlin：变量
来源：http://baike.vehdjk.com/Article/details/gxeeewaeg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.epnwcf.com/Article/details/geilykuul.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.bbcook.cn/Article/details/gpjmtahnj.sHtML

"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gzqtgurvs.sHtML

[T04] Kotlin：空安全
来源：http://read.share.epnwcf.com/Article/details/gzelnrlva.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fktsv.cn/Article/details/gcnvgohwo.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.vehdjk.com/Article/details/gxysufpzs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.sjlbkw.cn/Article/details/gqtptzlek.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.epnwcf.com/Article/details/gefyjkike.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gtepudupq.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gpgwhrglr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.tarul.cn/Article/details/gkgdyzqug.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/gdgsupvqc.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.vehdjk.com/Article/details/gnmacciqq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.vehdjk.com/Article/details/gdlonjqtm.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.vehdjk.com/Article/details/gzdqkrapm.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/gcrwaaaoo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.sjlbkw.cn/Article/details/gecysjdhh.sHtML

[T11] Kotlin：协程
来源：http://m.share.tarul.cn/Article/details/gkyqsrpjb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.tarul.cn/Article/details/gdfwysxss.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fktsv.cn/Article/details/gkrpxjyzu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/geghhofwv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gvrepakou.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.yfazqb.com/Article/details/gbqbswhhs.sHtML

[T14] Kotlin：循环
来源：http://www.share.vehdjk.com/Article/details/gtymutykb.sHtML

for (i in 1..10) println(i)
来源：http://baike.vehdjk.com/Article/details/gmukikeer.sHtML

[T15] Kotlin：接口
来源：http://wap.sjlbkw.cn/Article/details/gjolpvjpb.sHtML

interface Shape { fun area(): Double }
来源：http://3g.epnwcf.com/Article/details/gphgnkpvy.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gjtwaulwq.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/gjdlihcpw.sHtML

[T17] Swift：变量与常量
来源：http://wap.tarul.cn/Article/details/gbrsaffle.sHtML

var a = 1;  let b = 2
来源：http://www.blog.yfazqb.com/Article/details/gjpmaridr.sHtML

[T18] Swift：字符串插值
来源：http://blog.vehdjk.com/Article/details/giwsholog.sHtML

"值: \(b)"
来源：http://www.share.fktsv.cn/Article/details/gpfmmsnbq.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/gcfwkgjdf.sHtML

if let n = opt { print(n) }
来源：http://blog.tarul.cn/Article/details/gnydgmjnn.sHtML

[T20] Swift：数组操作
来源：http://mobile.bbcook.cn/Article/details/gvglxfoyy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/gjnagjxto.sHtML

[T21] Swift：遍历
来源：http://3g.fktsv.cn/Article/details/gdrgdvhxi.sHtML

for x in a { print(x) }
来源：http://wap.vehdjk.com/Article/details/ggdpxbvph.sHtML

[T22] Swift：字典
来源：http://www.blog.tarul.cn/Article/details/gxkmeyrvs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.bbcook.cn/Article/details/gkpraekyf.sHtML

[T23] Swift：函数
来源：http://blog.fktsv.cn/Article/details/gdmcszefy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.tarul.cn/Article/details/gryjsjebc.sHtML

[T24] Swift：闭包
来源：http://wap.bbcook.cn/Article/details/giyskhfxn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gprkgxthh.sHtML

[T25] Swift：结构体
来源：http://www.share.yfazqb.com/Article/details/gaqsmfpdz.sHtML

struct P { var x: Int }
来源：http://www.m.share.tarul.cn/Article/details/gwxvxybwt.sHtML

[T26] Swift：类与重写
来源：http://www.share.epnwcf.com/Article/details/gfetofaxb.sHtML

class A: Base { override func f() {} }
来源：http://mobile.vehdjk.com/Article/details/gdbivuyqb.sHtML

[T27] Swift：错误处理
来源：http://3g.vehdjk.com/Article/details/gxlwbxdev.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.bbcook.cn/Article/details/glnzbvmco.sHtML

[T28] Swift：枚举
来源：http://mobile.epnwcf.com/Article/details/gjklgibbp.sHtML

enum Color { case red, green }
来源：http://read.share.sjlbkw.cn/Article/details/grvwsexpr.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.tarul.cn/Article/details/gmgyjbmne.sHtML

guard let x = opt else { return }
来源：http://wap.sjlbkw.cn/Article/details/gumeyscue.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/grqrlqscd.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.tarul.cn/Article/details/gvffvtbke.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gcxwbzjeh.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gisxrwtim.sHtML

[T32] Lua：局部变量
来源：http://blog.tarul.cn/Article/details/gjsxmbdfu.sHtML

local a = 1
来源：http://www.m.share.yfazqb.com/Article/details/gewcmyeqg.sHtML

[T33] Lua：表（数组）
来源：http://read.share.yfazqb.com/Article/details/ggcepglzs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fktsv.cn/Article/details/goekknewd.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/gywulylmz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.epnwcf.com/Article/details/gzmwpidje.sHtML

[T35] Lua：字典表
来源：http://m.share.fktsv.cn/Article/details/ggyzbdoon.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.tarul.cn/Article/details/gkaupnhgy.sHtML

[T36] Lua：函数
来源：http://blog.vehdjk.com/Article/details/gguqlpkuk.sHtML

function add(a, b) return a + b end
来源：http://read.share.sjlbkw.cn/Article/details/gdhvfzowj.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gasqovorm.sHtML

"a" .. "b"
来源：http://mobile.epnwcf.com/Article/details/ghzefigqz.sHtML

[T38] Lua：条件
来源：http://mobile.vehdjk.com/Article/details/ggezrfbun.sHtML

if x > 0 then print("正") end
来源：http://blog.fktsv.cn/Article/details/gpbhrxpoo.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/gzufemfjl.sHtML

string.find(s, "%d+")
来源：http://baike.fktsv.cn/Article/details/gagtljicu.sHtML

[T40] Lua：元表
来源：http://3g.vehdjk.com/Article/details/gvwqpqcad.sHtML

setmetatable({}, { __index = base })
来源：http://baike.sjlbkw.cn/Article/details/gxmmuwkso.sHtML

[T41] Perl：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gwudrhden.sHtML

print "Hello\n";
来源：http://read.share.yfazqb.com/Article/details/gncrfhyei.sHtML

[T42] Perl：变量类型
来源：http://www.blog.yfazqb.com/Article/details/gappzskam.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.tarul.cn/Article/details/gscrlorzl.sHtML

[T43] Perl：字符串插值
来源：http://blog.bbcook.cn/Article/details/grhlruwjl.sHtML

"值: $a"
来源：http://wap.epnwcf.com/Article/details/geejarmmk.sHtML

[T44] Perl：条件
来源：http://3g.tarul.cn/Article/details/gnowcueuv.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.bbcook.cn/Article/details/glltmdzwb.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.yfazqb.com/Article/details/glkafssql.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gikbzreqa.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gmmehhxxr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fktsv.cn/Article/details/gmmyxxvcn.sHtML

[T47] Perl：正则捕获
来源：http://m.share.epnwcf.com/Article/details/gtguzirch.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.tarul.cn/Article/details/ghmbujhfp.sHtML

[T48] Perl：正则替换
来源：http://www.share.tarul.cn/Article/details/gkrkiijxd.sHtML

$s =~ s/old/new/g;
来源：http://wap.yfazqb.com/Article/details/goanrezwg.sHtML

[T49] Perl：函数
来源：http://3g.sjlbkw.cn/Article/details/gzgunhvvq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gxngoovmd.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gggoggfwv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.sjlbkw.cn/Article/details/ghakdwvla.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.tarul.cn/Article/details/geredabbi.sHtML

[T51] Scala：Hello World
来源：http://blog.yfazqb.com/Article/details/gmuxbuckw.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gjwoelaue.sHtML

[T52] Scala：变量
来源：http://3g.yfazqb.com/Article/details/gsxoznudm.sHtML

val a = 1;  var b = 2
来源：http://3g.yfazqb.com/Article/details/gouowtfjk.sHtML

[T53] Scala：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gosduyjkj.sHtML

s"值: $b"
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvpbnnri.sHtML

[T54] Scala：集合映射
来源：http://mobile.tarul.cn/Article/details/gafizvgor.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.yfazqb.com/Article/details/gezyoczjz.sHtML

[T55] Scala：集合过滤
来源：http://m.share.epnwcf.com/Article/details/gwyeavoip.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/guqiaeete.sHtML

[T56] Scala：样例类
来源：http://wap.sjlbkw.cn/Article/details/glaipyrdy.sHtML

case class User(name: String, age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gdzndiwwu.sHtML

[T57] Scala：模式匹配
来源：http://mobile.epnwcf.com/Article/details/gceeluqqm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.bbcook.cn/Article/details/gifeokwif.sHtML

[T58] Scala：函数定义
来源：http://www.share.bbcook.cn/Article/details/gwltyxcuc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fktsv.cn/Article/details/glracjqfs.sHtML

[T59] Scala：循环
来源：http://baike.yfazqb.com/Article/details/gktmayslb.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.epnwcf.com/Article/details/ghbcznrig.sHtML

[T60] Scala：折叠
来源：http://mobile.tarul.cn/Article/details/gwzwigfyo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.vehdjk.com/Article/details/gogapugjc.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwsflnlka.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/gzjypmmgf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guyyapfvy.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.vehdjk.com/Article/details/gogpeqdks.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.bbcook.cn/Article/details/gzaiyucwj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.bbcook.cn/Article/details/gcevgtztd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fktsv.cn/Article/details/ganbiaugr.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.sjlbkw.cn/Article/details/grkzroxsp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.yfazqb.com/Article/details/ghwhrlgev.sHtML

[U04] Py：变量调试打印
来源：http://baike.sjlbkw.cn/Article/details/gsladxdav.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fktsv.cn/Article/details/gopypgknm.sHtML

[U05] Py：列表去重且保序
来源：http://blog.bbcook.cn/Article/details/gylrktbgp.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/gmbzjhkid.sHtML

[U06] Py：合并两个字典
来源：http://mobile.bbcook.cn/Article/details/gbxcuxtjt.sHtML

{**a, **b}
来源：http://baike.tarul.cn/Article/details/gjlgmrsrs.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.epnwcf.com/Article/details/gnkcmaeaj.sHtML

{v: k for k, v in d.items()}
来源：http://3g.vehdjk.com/Article/details/gpnxdwsef.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fktsv.cn/Article/details/ghojrvvlt.sHtML

[y for x in nested for y in x]
来源：http://baike.vehdjk.com/Article/details/gulsoeutd.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.vehdjk.com/Article/details/gthgnofec.sHtML

max(d, key=d.get)
来源：http://3g.epnwcf.com/Article/details/gslitscss.sHtML

[U10] Py：按值排序字典
来源：http://wap.vehdjk.com/Article/details/gghstwulv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.sjlbkw.cn/Article/details/glutrheyz.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fktsv.cn/Article/details/guzjzjahn.sHtML

(x * 2 for x in arr)
来源：http://m.share.tarul.cn/Article/details/gcpphudnl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.vehdjk.com/Article/details/gqawfljfw.sHtML

Counter(arr).most_common(3)
来源：http://3g.fktsv.cn/Article/details/ggkxejogx.sHtML

[U13] Py：固定长度队列
来源：http://wap.yfazqb.com/Article/details/gvysxtbot.sHtML

deque(maxlen=10)
来源：http://www.m.share.bbcook.cn/Article/details/gqfxaekge.sHtML

[U14] Py：分组收集到列表
来源：http://baike.epnwcf.com/Article/details/gsnekvvfo.sHtML

defaultdict(list)
来源：http://blog.sjlbkw.cn/Article/details/gpsqotdtl.sHtML

[U15] Py：高精度计时
来源：http://read.share.fktsv.cn/Article/details/gctebfxtg.sHtML

t = time.perf_counter()
来源：http://baike.sjlbkw.cn/Article/details/gmwmbdhvz.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.yfazqb.com/Article/details/gzixfeoll.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.sjlbkw.cn/Article/details/gnuukstso.sHtML

[U17] Py：初始化日志
来源：http://m.share.bbcook.cn/Article/details/gqrfyqqzn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.sjlbkw.cn/Article/details/ggebgpgmp.sHtML

[U18] Py：预编译正则
来源：http://m.share.epnwcf.com/Article/details/gpydvbaws.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fktsv.cn/Article/details/gcouuuztr.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.sjlbkw.cn/Article/details/gowfldqmr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fktsv.cn/Article/details/gcwfxlztj.sHtML

[U20] Py：缓存函数结果
来源：http://wap.bbcook.cn/Article/details/ghdbciyjs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fktsv.cn/Article/details/gdardklgr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.yfazqb.com/Article/details/gtasfjpjg.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fktsv.cn/Article/details/gzpvlsidh.sHtML

[U22] Py：矩阵转置
来源：http://blog.vehdjk.com/Article/details/gekbutcrm.sHtML

list(zip(*m))
来源：http://m.share.tarul.cn/Article/details/gbfqpkdsq.sHtML

[U23] Py：分块读取大文件
来源：http://3g.yfazqb.com/Article/details/gpmefecht.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fktsv.cn/Article/details/gixolfbez.sHtML

[U24] Py：路径操作
来源：http://www.share.yfazqb.com/Article/details/gjrbfzhvr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/ghzglpzlk.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.tarul.cn/Article/details/gtmzvkkmu.sHtML

csv.DictReader(f)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmexexzp.sHtML

[U26] Py：并发下载
来源：http://mobile.bbcook.cn/Article/details/gcpmoybgb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.epnwcf.com/Article/details/ghqlrdxjg.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.vehdjk.com/Article/details/glbkngvqe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.yfazqb.com/Article/details/gmepzmovn.sHtML

[U28] Py：类型别名
来源：http://www.blog.tarul.cn/Article/details/gwazszlqw.sHtML

UserId = int
来源：http://m.share.fktsv.cn/Article/details/gnaxlnjra.sHtML

[U29] Py：属性校验
来源：http://mobile.tarul.cn/Article/details/gaxgtgoun.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fktsv.cn/Article/details/gprsdhzkc.sHtML

[U30] Py：数据类
来源：http://3g.sjlbkw.cn/Article/details/gaaebuwxn.sHtML

@dataclass(slots=True)
来源：http://m.share.vehdjk.com/Article/details/gebypkrky.sHtML

[U31] Py：单测
来源：http://read.share.vehdjk.com/Article/details/gbqiktvrl.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/ggknrulgl.sHtML

[U32] Py：代码格式化
来源：http://www.share.sjlbkw.cn/Article/details/gjqtnjlem.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.sjlbkw.cn/Article/details/gmxfxopwi.sHtML

[U33] Py：打包发布
来源：http://m.share.sjlbkw.cn/Article/details/gddrudswc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.epnwcf.com/Article/details/gvgebahtm.sHtML

[U34] Py：判断编码
来源：http://blog.yfazqb.com/Article/details/gcenxhvez.sHtML

chardet.detect(raw)
来源：http://blog.bbcook.cn/Article/details/gutpuewfr.sHtML

[U35] Py：发送邮件
来源：http://read.share.sjlbkw.cn/Article/details/gdtmshlso.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwklwfozh.sHtML

[U36] Py：定时任务
来源：http://3g.epnwcf.com/Article/details/gcjzonrcg.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.sjlbkw.cn/Article/details/gqguoqqsl.sHtML

[U37] Py：读写 Excel
来源：http://read.share.tarul.cn/Article/details/gaswvzlzi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.bbcook.cn/Article/details/gjwybqucq.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fktsv.cn/Article/details/gutsqsxzk.sHtML

Path(__file__).resolve().parent
来源：http://3g.fktsv.cn/Article/details/grkakreal.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.bbcook.cn/Article/details/gbdutoerh.sHtML

sys.stdout.isatty()
来源：http://www.blog.vehdjk.com/Article/details/githwtbtx.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.epnwcf.com/Article/details/gszhqajel.sHtML

print("err", file=sys.stderr)
来源：http://blog.vehdjk.com/Article/details/gsjhigirq.sHtML


<!-- 参考信息 -->