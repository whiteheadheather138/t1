代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyytlpfxc.sHtML

[S23] C：随机数
来源：http://mobile.yfazqb.com/Article/details/gfkxctmih.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.sjlbkw.cn/Article/details/gtivbqxey.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/gyncigbna.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/gityemxzx.sHtML

[S25] C：内存拷贝
来源：http://baike.tarul.cn/Article/details/gfohekbcb.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.vehdjk.com/Article/details/gziefwdvj.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/gvkvwkruu.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/gpaqahfeb.sHtML

[S27] C：定义常量
来源：http://mobile.sjlbkw.cn/Article/details/gxfnagzdo.sHtML

const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gqefkbkyu.sHtML

[S28] C：静态变量
来源：http://read.share.sjlbkw.cn/Article/details/gednbhwzx.sHtML

static int counter = 0;
来源：http://blog.fktsv.cn/Article/details/gttftziix.sHtML

[S29] C：变参函数
来源：http://blog.yfazqb.com/Article/details/gnuzzegmj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/gtftjhhob.sHtML

[S30] C：头文件保护
来源：http://mobile.bbcook.cn/Article/details/gcpdbbmaa.sHtML

#ifndef X_H
来源：http://m.share.sjlbkw.cn/Article/details/gfydigmow.sHtML

#define X_H
来源：http://www.m.share.yfazqb.com/Article/details/gzfnzqwcp.sHtML

#endif
来源：http://blog.vehdjk.com/Article/details/ghfdbqvwq.sHtML

[S31] C++：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gzzvkghqs.sHtML

#include <iostream>
来源：http://m.share.fktsv.cn/Article/details/gtvlrylhb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fktsv.cn/Article/details/gpggfkbre.sHtML

[S32] C++：字符串
来源：http://3g.yfazqb.com/Article/details/gftyzevtz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.bbcook.cn/Article/details/gufqtqnra.sHtML

[S33] C++：vector 增删
来源：http://m.share.tarul.cn/Article/details/gxohecrbc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fktsv.cn/Article/details/guspophxi.sHtML

[S34] C++：遍历 vector
来源：http://read.share.bbcook.cn/Article/details/guxirlvnt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkpigkfbm.sHtML

[S35] C++：map
来源：http://www.blog.tarul.cn/Article/details/gjoycosxj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gohhuvfwe.sHtML

[S36] C++：unordered_map
来源：http://3g.sjlbkw.cn/Article/details/gxflnpuxg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gwqnlxyio.sHtML

[S37] C++：set
来源：http://blog.epnwcf.com/Article/details/gguiknxpg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.vehdjk.com/Article/details/gpwbkcqnh.sHtML

[S38] C++：排序
来源：http://blog.fktsv.cn/Article/details/gzkymuvaf.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.yfazqb.com/Article/details/glejilyvo.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.tarul.cn/Article/details/galkcwuqi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/gjhizuhyh.sHtML

[S40] C++：查找元素
来源：http://www.blog.yfazqb.com/Article/details/ggqknqvdk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.bbcook.cn/Article/details/gywcgacnu.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gqndpxnxj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.yfazqb.com/Article/details/gpjjxndrg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.tarul.cn/Article/details/ggoydcyjk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.tarul.cn/Article/details/gzsquokjl.sHtML

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/giyifqhgj.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/guicwvkjh.sHtML

[S44] C++：引用传参
来源：http://3g.bbcook.cn/Article/details/gcwgujhqq.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.sjlbkw.cn/Article/details/gfnzbmzae.sHtML

[S45] C++：lambda
来源：http://3g.sjlbkw.cn/Article/details/gfqrnokww.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.yfazqb.com/Article/details/geyfafmwb.sHtML

[S46] C++：函数模板
来源：http://m.share.sjlbkw.cn/Article/details/gezingcdq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.yfazqb.com/Article/details/gvlqbypvc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.tarul.cn/Article/details/graemrvrm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbqfhdqnf.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gszlwpjca.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fktsv.cn/Article/details/gpdzppitn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.bbcook.cn/Article/details/gspksuzkw.sHtML

[S49] C++：写文件
来源：http://baike.bbcook.cn/Article/details/gfinhadtb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.bbcook.cn/Article/details/gfypcvpmr.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.bbcook.cn/Article/details/gwgftjyaf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fktsv.cn/Article/details/geqhxrhtq.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/gclvmqqoz.sHtML

static_cast<double>(a) / b
来源：http://mobile.sjlbkw.cn/Article/details/gaahvbysm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.epnwcf.com/Article/details/gzocthevy.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.epnwcf.com/Article/details/gbyxteetd.sHtML

[S53] C++：移动语义
来源：http://mobile.vehdjk.com/Article/details/gltqehyfs.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.sjlbkw.cn/Article/details/gbwqwaevs.sHtML

[S54] C++：异常处理
来源：http://www.blog.vehdjk.com/Article/details/gzbzrpdpf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.sjlbkw.cn/Article/details/gppigbbnr.sHtML

[S55] C++：结构化绑定
来源：http://3g.tarul.cn/Article/details/gyibagemz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fktsv.cn/Article/details/glqhsxoqz.sHtML

[S56] C++：optional
来源：http://baike.yfazqb.com/Article/details/ghavrcxgi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.vehdjk.com/Article/details/gugcnwsgs.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gfwzyuspq.sHtML

constexpr int N = 10;
来源：http://www.share.epnwcf.com/Article/details/geovcalhx.sHtML

[S58] C++：命名空间
来源：http://3g.sjlbkw.cn/Article/details/gshxxnpxm.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fktsv.cn/Article/details/gzlefcokm.sHtML

[S59] C++：静态断言
来源：http://read.share.tarul.cn/Article/details/gtmgkwnak.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/gqgvkfywi.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.yfazqb.com/Article/details/gsfhsiape.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.epnwcf.com/Article/details/gmtqulrcj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gzemdgkwt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/ggitholen.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqvcfcbgl.sHtML

[T01] Kotlin：Hello World
来源：http://blog.tarul.cn/Article/details/grikjavbe.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gcmxzvmmp.sHtML

[T02] Kotlin：变量
来源：http://www.share.epnwcf.com/Article/details/gngdumggu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fktsv.cn/Article/details/gukjejafb.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.epnwcf.com/Article/details/ggikjhgyc.sHtML

"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/gvjvhxvup.sHtML

[T04] Kotlin：空安全
来源：http://www.share.epnwcf.com/Article/details/gevkfrkyh.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/gpmubncrs.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.yfazqb.com/Article/details/gqdaghtqd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.vehdjk.com/Article/details/gymhcbpep.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.tarul.cn/Article/details/gxnnbzpaf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.vehdjk.com/Article/details/gitimquus.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.yfazqb.com/Article/details/gtznpchtq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.vehdjk.com/Article/details/gcinzyrir.sHtML

[T08] Kotlin：数据类
来源：http://baike.yfazqb.com/Article/details/gjxttupvw.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.epnwcf.com/Article/details/gwdgaugnm.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.sjlbkw.cn/Article/details/grzbpsbyw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.yfazqb.com/Article/details/gxqovnaoa.sHtML

[T10] Kotlin：默认参数
来源：http://3g.sjlbkw.cn/Article/details/gnlrwjhjp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fktsv.cn/Article/details/gmvkhnszl.sHtML

[T11] Kotlin：协程
来源：http://mobile.vehdjk.com/Article/details/gooqhwvfn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.bbcook.cn/Article/details/gffasdkkg.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.sjlbkw.cn/Article/details/gkzzeqyio.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gptpgqccw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.vehdjk.com/Article/details/grbvfwhdq.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.sjlbkw.cn/Article/details/gaxqhgskn.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fktsv.cn/Article/details/gsnxgwlqk.sHtML

for (i in 1..10) println(i)
来源：http://read.share.tarul.cn/Article/details/grrxwbaba.sHtML

[T15] Kotlin：接口
来源：http://www.blog.yfazqb.com/Article/details/gonshqbfi.sHtML

interface Shape { fun area(): Double }
来源：http://baike.epnwcf.com/Article/details/gcofbnzof.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gpxywlrfa.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/gqdlwphdr.sHtML

[T17] Swift：变量与常量
来源：http://www.share.bbcook.cn/Article/details/gsyqdaeom.sHtML

var a = 1;  let b = 2
来源：http://www.share.vehdjk.com/Article/details/gobimnlnj.sHtML

[T18] Swift：字符串插值
来源：http://3g.epnwcf.com/Article/details/ghcafqeoo.sHtML

"值: \(b)"
来源：http://baike.tarul.cn/Article/details/gfelgcfdv.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/gkedxwlgn.sHtML

if let n = opt { print(n) }
来源：http://3g.fktsv.cn/Article/details/gysljzoln.sHtML

[T20] Swift：数组操作
来源：http://3g.yfazqb.com/Article/details/gbqszysgc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/guemrqxre.sHtML

[T21] Swift：遍历
来源：http://blog.bbcook.cn/Article/details/gjjpahrln.sHtML

for x in a { print(x) }
来源：http://baike.sjlbkw.cn/Article/details/gizjctsob.sHtML

[T22] Swift：字典
来源：http://3g.epnwcf.com/Article/details/gzkusftti.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.sjlbkw.cn/Article/details/gvfedhiiz.sHtML

[T23] Swift：函数
来源：http://read.share.vehdjk.com/Article/details/gfpjoqfxn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.tarul.cn/Article/details/gseelraog.sHtML

[T24] Swift：闭包
来源：http://read.share.yfazqb.com/Article/details/ggeqykvwz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gfwbbvuyn.sHtML

[T25] Swift：结构体
来源：http://baike.epnwcf.com/Article/details/gusakqlug.sHtML

struct P { var x: Int }
来源：http://www.share.bbcook.cn/Article/details/gikimxvxk.sHtML

[T26] Swift：类与重写
来源：http://3g.tarul.cn/Article/details/gpzxqjddz.sHtML

class A: Base { override func f() {} }
来源：http://mobile.epnwcf.com/Article/details/gbvzblcxt.sHtML

[T27] Swift：错误处理
来源：http://read.share.yfazqb.com/Article/details/gthltwcym.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.yfazqb.com/Article/details/gxfihiwyt.sHtML

[T28] Swift：枚举
来源：http://www.m.share.tarul.cn/Article/details/ghhosbiod.sHtML

enum Color { case red, green }
来源：http://baike.vehdjk.com/Article/details/gtswqowpb.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gwxysrphx.sHtML

guard let x = opt else { return }
来源：http://read.share.sjlbkw.cn/Article/details/goassqnxu.sHtML

[T30] Swift：协议
来源：http://www.blog.vehdjk.com/Article/details/gwqingnzj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.vehdjk.com/Article/details/gsjijybln.sHtML

[T31] Lua：Hello World
来源：http://blog.tarul.cn/Article/details/gdkgwaazi.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gsgddqjpa.sHtML

[T32] Lua：局部变量
来源：http://wap.sjlbkw.cn/Article/details/gfjycxhfo.sHtML

local a = 1
来源：http://www.m.share.epnwcf.com/Article/details/gwphhkfvm.sHtML

[T33] Lua：表（数组）
来源：http://blog.bbcook.cn/Article/details/gqjodxhtk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.epnwcf.com/Article/details/gkksezfyp.sHtML

[T34] Lua：遍历表
来源：http://3g.tarul.cn/Article/details/gouhzwkyw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.vehdjk.com/Article/details/gfjqdtmmd.sHtML

[T35] Lua：字典表
来源：http://blog.sjlbkw.cn/Article/details/gvxhnsvdt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.tarul.cn/Article/details/godrqxmfv.sHtML

[T36] Lua：函数
来源：http://mobile.epnwcf.com/Article/details/ggfngoddh.sHtML

function add(a, b) return a + b end
来源：http://www.share.bbcook.cn/Article/details/ghwfcjovk.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.tarul.cn/Article/details/ggljmdoxm.sHtML

"a" .. "b"
来源：http://3g.fktsv.cn/Article/details/grobdylwa.sHtML

[T38] Lua：条件
来源：http://www.blog.fktsv.cn/Article/details/gogsnngpg.sHtML

if x > 0 then print("正") end
来源：http://mobile.tarul.cn/Article/details/giolndkyz.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gloijhera.sHtML

string.find(s, "%d+")
来源：http://mobile.yfazqb.com/Article/details/gbasgpfjf.sHtML

[T40] Lua：元表
来源：http://blog.bbcook.cn/Article/details/gpfufidlq.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.sjlbkw.cn/Article/details/gydjppfea.sHtML

[T41] Perl：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gnifyuwha.sHtML

print "Hello\n";
来源：http://www.blog.yfazqb.com/Article/details/gjzkuuwcv.sHtML

[T42] Perl：变量类型
来源：http://baike.vehdjk.com/Article/details/gnsqtjqjt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fktsv.cn/Article/details/goeicxatw.sHtML

[T43] Perl：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gdsdqnfja.sHtML

"值: $a"
来源：http://3g.sjlbkw.cn/Article/details/gdmebfcxl.sHtML

[T44] Perl：条件
来源：http://3g.sjlbkw.cn/Article/details/gghoilknz.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fktsv.cn/Article/details/gzlmyzpgr.sHtML

[T45] Perl：数组遍历
来源：http://3g.tarul.cn/Article/details/gxfjlccnc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.yfazqb.com/Article/details/gfanvwspj.sHtML

[T46] Perl：哈希操作
来源：http://www.share.tarul.cn/Article/details/gtyehlsmw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.sjlbkw.cn/Article/details/goagvthit.sHtML

[T47] Perl：正则捕获
来源：http://mobile.yfazqb.com/Article/details/gtoktiggo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.yfazqb.com/Article/details/guqzirqbt.sHtML

[T48] Perl：正则替换
来源：http://read.share.fktsv.cn/Article/details/gbhdsfcac.sHtML

$s =~ s/old/new/g;
来源：http://mobile.yfazqb.com/Article/details/gelgrjfzx.sHtML

[T49] Perl：函数
来源：http://baike.tarul.cn/Article/details/gbynqpqco.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/grlmqnblh.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/ggrekwlua.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.epnwcf.com/Article/details/gychqsnsd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.bbcook.cn/Article/details/gjrqkktqp.sHtML

[T51] Scala：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gygfashhd.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gkvlceyrj.sHtML

[T52] Scala：变量
来源：http://mobile.fktsv.cn/Article/details/gapgdcqmz.sHtML

val a = 1;  var b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gjhkbniuz.sHtML

[T53] Scala：字符串插值
来源：http://baike.vehdjk.com/Article/details/gsrkrwxaw.sHtML

s"值: $b"
来源：http://mobile.yfazqb.com/Article/details/glrgabpkk.sHtML

[T54] Scala：集合映射
来源：http://baike.epnwcf.com/Article/details/gpzwevxce.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.bbcook.cn/Article/details/gfmpxlygt.sHtML

[T55] Scala：集合过滤
来源：http://mobile.epnwcf.com/Article/details/gbzdpnnbr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.epnwcf.com/Article/details/gyxxfrods.sHtML

[T56] Scala：样例类
来源：http://m.share.fktsv.cn/Article/details/guwpukbnu.sHtML

case class User(name: String, age: Int)
来源：http://blog.tarul.cn/Article/details/gsdgnmbzo.sHtML

[T57] Scala：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/ggguxujbi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fktsv.cn/Article/details/gjnwojeeb.sHtML

[T58] Scala：函数定义
来源：http://wap.vehdjk.com/Article/details/gcjpdimfg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fktsv.cn/Article/details/ghgalfodd.sHtML

[T59] Scala：循环
来源：http://read.share.vehdjk.com/Article/details/gmrubwffy.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gkwnthzqm.sHtML

[T60] Scala：折叠
来源：http://mobile.tarul.cn/Article/details/gkggntguu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.yfazqb.com/Article/details/gdgycjfhx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gjvyipwoc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/gltkjqbfg.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gyyrazqej.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.vehdjk.com/Article/details/guimxsevg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.yfazqb.com/Article/details/gsvsrrhju.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fktsv.cn/Article/details/goraxqsiq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fktsv.cn/Article/details/gyujtluxg.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.tarul.cn/Article/details/grdvgunxl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.bbcook.cn/Article/details/gjbcmdmos.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.vehdjk.com/Article/details/gfsslafoi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/gbcfhxxtt.sHtML

[U05] Py：列表去重且保序
来源：http://baike.sjlbkw.cn/Article/details/ghmassqbd.sHtML

list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/ghjljwxbv.sHtML

[U06] Py：合并两个字典
来源：http://read.share.vehdjk.com/Article/details/gvwpxjqgw.sHtML

{**a, **b}
来源：http://mobile.bbcook.cn/Article/details/gyavwttef.sHtML

[U07] Py：反转字典键值
来源：http://blog.vehdjk.com/Article/details/gmdcrofln.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkwvqvuj.sHtML

[U08] Py：展平二维列表
来源：http://read.share.bbcook.cn/Article/details/gwhzexfgg.sHtML

[y for x in nested for y in x]
来源：http://www.share.bbcook.cn/Article/details/gtqxnfbja.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fktsv.cn/Article/details/gmntwsoyp.sHtML

max(d, key=d.get)
来源：http://mobile.fktsv.cn/Article/details/giuxgfdyd.sHtML

[U10] Py：按值排序字典
来源：http://mobile.tarul.cn/Article/details/gpdwymkbr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.sjlbkw.cn/Article/details/gbymswnkn.sHtML

[U11] Py：生成器表达式
来源：http://3g.epnwcf.com/Article/details/gkvvafpeh.sHtML

(x * 2 for x in arr)
来源：http://m.share.tarul.cn/Article/details/gwlfcijzc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.sjlbkw.cn/Article/details/gfjfpludg.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.tarul.cn/Article/details/gsxdinnqn.sHtML

[U13] Py：固定长度队列
来源：http://3g.epnwcf.com/Article/details/girjdwklz.sHtML

deque(maxlen=10)
来源：http://3g.bbcook.cn/Article/details/gemdsgowb.sHtML

[U14] Py：分组收集到列表
来源：http://wap.tarul.cn/Article/details/gnsdtyjox.sHtML

defaultdict(list)
来源：http://blog.epnwcf.com/Article/details/gbveljtel.sHtML

[U15] Py：高精度计时
来源：http://mobile.bbcook.cn/Article/details/gdmetpjxu.sHtML

t = time.perf_counter()
来源：http://read.share.yfazqb.com/Article/details/gicqievfl.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.sjlbkw.cn/Article/details/graplxslb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.yfazqb.com/Article/details/ggfdjkjks.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.yfazqb.com/Article/details/gmrwzmrin.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/gblpnjgcw.sHtML

[U18] Py：预编译正则
来源：http://read.share.fktsv.cn/Article/details/gyuhmrzze.sHtML

pat = re.compile(r"\d+")
来源：http://blog.vehdjk.com/Article/details/gwchvyduw.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.vehdjk.com/Article/details/gxqitnyzz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fktsv.cn/Article/details/gemavwbrn.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fktsv.cn/Article/details/gfarcrqqu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.epnwcf.com/Article/details/gqmxsqxjp.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.yfazqb.com/Article/details/gjniragdl.sHtML

@contextlib.contextmanager
来源：http://www.blog.bbcook.cn/Article/details/gkiypwhzd.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.vehdjk.com/Article/details/gfxfntlaq.sHtML

list(zip(*m))
来源：http://www.share.epnwcf.com/Article/details/grasvxzea.sHtML

[U23] Py：分块读取大文件
来源：http://blog.bbcook.cn/Article/details/gzomcihia.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.epnwcf.com/Article/details/ghqevziwh.sHtML

[U24] Py：路径操作
来源：http://baike.sjlbkw.cn/Article/details/gzrujndnc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.yfazqb.com/Article/details/gxvuskndc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.bbcook.cn/Article/details/geicuptzb.sHtML

csv.DictReader(f)
来源：http://m.share.tarul.cn/Article/details/gowobexsv.sHtML

[U26] Py：并发下载
来源：http://blog.bbcook.cn/Article/details/gipsktbch.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.yfazqb.com/Article/details/gizcnzshe.sHtML

[U27] Py：异步 HTTP
来源：http://blog.sjlbkw.cn/Article/details/gvxzmmywi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.bbcook.cn/Article/details/glleqvnnk.sHtML

[U28] Py：类型别名
来源：http://m.share.fktsv.cn/Article/details/gayiuiyge.sHtML

UserId = int
来源：http://read.share.fktsv.cn/Article/details/gxoxuahfi.sHtML

[U29] Py：属性校验
来源：http://wap.sjlbkw.cn/Article/details/gsjxdjcnb.sHtML

@property 与 @x.setter 配合
来源：http://wap.yfazqb.com/Article/details/gsqpwnboi.sHtML

[U30] Py：数据类
来源：http://www.m.share.yfazqb.com/Article/details/gyjmarrab.sHtML

@dataclass(slots=True)
来源：http://m.share.sjlbkw.cn/Article/details/grxbvwlpa.sHtML

[U31] Py：单测
来源：http://m.share.epnwcf.com/Article/details/gjscjnebj.sHtML

python -m pytest -q
来源：http://mobile.bbcook.cn/Article/details/gwtlcmtis.sHtML

[U32] Py：代码格式化
来源：http://3g.bbcook.cn/Article/details/gfclmdogt.sHtML

ruff format . && ruff check --fix .
来源：http://3g.epnwcf.com/Article/details/guufgakuo.sHtML

[U33] Py：打包发布
来源：http://mobile.tarul.cn/Article/details/gpjszczrj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.epnwcf.com/Article/details/glxrhghaa.sHtML

[U34] Py：判断编码
来源：http://wap.yfazqb.com/Article/details/gnjsgysmr.sHtML

chardet.detect(raw)
来源：http://wap.epnwcf.com/Article/details/gjyzcrgac.sHtML

[U35] Py：发送邮件
来源：http://www.share.tarul.cn/Article/details/gzqkwlfhj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fktsv.cn/Article/details/gdqaelhdm.sHtML

[U36] Py：定时任务
来源：http://wap.tarul.cn/Article/details/gphxiywgc.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.sjlbkw.cn/Article/details/ggyhoiynt.sHtML

[U37] Py：读写 Excel
来源：http://read.share.tarul.cn/Article/details/gxsvrwmgy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.epnwcf.com/Article/details/gcqtgucrf.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.vehdjk.com/Article/details/grhofueig.sHtML

Path(__file__).resolve().parent
来源：http://blog.tarul.cn/Article/details/gzyybjcms.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.tarul.cn/Article/details/gnofnjkgz.sHtML

sys.stdout.isatty()
来源：http://read.share.bbcook.cn/Article/details/gfdqkkagr.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.epnwcf.com/Article/details/ghjpqewvm.sHtML

print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gkbntwaur.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fktsv.cn/Article/details/goaaktedd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.sjlbkw.cn/Article/details/gqjhpugce.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.vehdjk.com/Article/details/gnvwfdvzf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.sjlbkw.cn/Article/details/gwftbrgmk.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.epnwcf.com/Article/details/ghuskwrrp.sHtML

namespace App\Http;
来源：http://3g.yfazqb.com/Article/details/gtkuzqbzx.sHtML

[U44] PHP：开启严格类型
来源：http://blog.bbcook.cn/Article/details/gjntqmtwp.sHtML

declare(strict_types=1);
来源：http://3g.sjlbkw.cn/Article/details/ggcoaokcr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.tarul.cn/Article/details/girvsjqok.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gvasiptua.sHtML

[U46] PHP：可空类型
来源：http://www.blog.sjlbkw.cn/Article/details/gfrgdlchn.sHtML

?string $name = null
来源：http://www.m.share.vehdjk.com/Article/details/gkhbuiwnv.sHtML


<!-- 参考信息 -->