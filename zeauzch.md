代发 wailian999

int main(int argc, char **argv)
来源：http://mobile.fktsv.cn/Article/details/gwlbgzeng.sHtML

[S19] C：快速排序
来源：http://baike.epnwcf.com/Article/details/ghgiucgyx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/gjfweuwio.sHtML

[S20] C：二分查找
来源：http://3g.epnwcf.com/Article/details/gamfghfmw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gaaqqixtp.sHtML

[S21] C：字符类别判断
来源：http://blog.epnwcf.com/Article/details/guswakcoo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fktsv.cn/Article/details/gybkrhxdl.sHtML

[S22] C：字符串转数字
来源：http://3g.epnwcf.com/Article/details/gznbxmttf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/gjocyuxqg.sHtML

[S23] C：随机数
来源：http://m.share.epnwcf.com/Article/details/glwrqnayi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.yfazqb.com/Article/details/grpeapzss.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/gjvvtkbuz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.bbcook.cn/Article/details/gcxzqfvux.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/gwgwjtxml.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gdvxfbrrb.sHtML

[S26] C：内存清零
来源：http://m.share.sjlbkw.cn/Article/details/ghbtcvksa.sHtML

memset(a, 0, sizeof a);
来源：http://blog.bbcook.cn/Article/details/gvdvzouwv.sHtML

[S27] C：定义常量
来源：http://mobile.sjlbkw.cn/Article/details/gxmzqardw.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gyjskvpxy.sHtML

[S28] C：静态变量
来源：http://www.m.share.tarul.cn/Article/details/gjpexildj.sHtML

static int counter = 0;
来源：http://wap.yfazqb.com/Article/details/gxgnbtfho.sHtML

[S29] C：变参函数
来源：http://read.share.epnwcf.com/Article/details/grzwlifqa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/gvyacjarp.sHtML

[S30] C：头文件保护
来源：http://www.share.fktsv.cn/Article/details/gjxnbiolr.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/gynskhzww.sHtML

#define X_H
来源：http://3g.fktsv.cn/Article/details/gvrcnjeoc.sHtML

#endif
来源：http://blog.yfazqb.com/Article/details/grusiqknw.sHtML

[S31] C++：Hello World
来源：http://wap.vehdjk.com/Article/details/gfabvtkfj.sHtML

#include <iostream>
来源：http://3g.bbcook.cn/Article/details/gblnqpjln.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.bbcook.cn/Article/details/gjmdymjuk.sHtML

[S32] C++：字符串
来源：http://m.share.vehdjk.com/Article/details/gzgcvbqfe.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.epnwcf.com/Article/details/grjhjkfqw.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/gpbwpxzqt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.epnwcf.com/Article/details/gcsjdaksj.sHtML

[S34] C++：遍历 vector
来源：http://baike.fktsv.cn/Article/details/gtphuofwz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.epnwcf.com/Article/details/guazgezwk.sHtML

[S35] C++：map
来源：http://3g.bbcook.cn/Article/details/gkenyxtfw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/gvgqtwpvp.sHtML

[S36] C++：unordered_map
来源：http://blog.epnwcf.com/Article/details/gjckzlaik.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gjnnjlvts.sHtML

[S37] C++：set
来源：http://wap.sjlbkw.cn/Article/details/gbvuoyvyi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.tarul.cn/Article/details/ghvgbuevh.sHtML

[S38] C++：排序
来源：http://3g.yfazqb.com/Article/details/gzjohydoi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gzoymetrw.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/guaehxzfh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/gsfowrzew.sHtML

[S40] C++：查找元素
来源：http://3g.epnwcf.com/Article/details/gbijvhavv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.epnwcf.com/Article/details/grpcrkmoq.sHtML

[S41] C++：类与构造函数
来源：http://mobile.yfazqb.com/Article/details/glqwzhfnp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.sjlbkw.cn/Article/details/ggcfkdgdb.sHtML

[S42] C++：继承与虚函数
来源：http://wap.tarul.cn/Article/details/gaeukdfsj.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/gegifatpn.sHtML

[S43] C++：智能指针
来源：http://m.share.vehdjk.com/Article/details/gbjxgkltg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/giwhmadbp.sHtML

[S44] C++：引用传参
来源：http://read.share.bbcook.cn/Article/details/gcgrciyuu.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzojgpeam.sHtML

[S45] C++：lambda
来源：http://www.blog.vehdjk.com/Article/details/ggfzjhvko.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.epnwcf.com/Article/details/gyeocehbz.sHtML

[S46] C++：函数模板
来源：http://baike.vehdjk.com/Article/details/gekkplbyo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gguryafiw.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.tarul.cn/Article/details/gkldmyvdm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.bbcook.cn/Article/details/gxqosqekd.sHtML

[S48] C++：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gsdjkmucl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.sjlbkw.cn/Article/details/gspbewwiz.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gprhxdotw.sHtML

[S49] C++：写文件
来源：http://3g.tarul.cn/Article/details/gogasacey.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/gomkcequq.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/ggnbiekfo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gcgccrotp.sHtML

[S51] C++：显式类型转换
来源：http://baike.tarul.cn/Article/details/govcjpgmo.sHtML

static_cast<double>(a) / b
来源：http://baike.vehdjk.com/Article/details/gngxowmob.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.epnwcf.com/Article/details/glwgskcwk.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.tarul.cn/Article/details/gwdghnkgq.sHtML

[S53] C++：移动语义
来源：http://www.blog.fktsv.cn/Article/details/gazmmxbsz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.vehdjk.com/Article/details/gsgxjeqpv.sHtML

[S54] C++：异常处理
来源：http://m.share.bbcook.cn/Article/details/gsnmdflcj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fktsv.cn/Article/details/gbfhewols.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwlsjayu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.epnwcf.com/Article/details/gijzdkmyy.sHtML

[S56] C++：optional
来源：http://wap.tarul.cn/Article/details/gedgsqazp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/gxtivajnl.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gqkyzbxoc.sHtML

constexpr int N = 10;
来源：http://mobile.vehdjk.com/Article/details/gyfotixlf.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/ghzkvrtgd.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.tarul.cn/Article/details/gnkvrnsia.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/gqkliuglq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.vehdjk.com/Article/details/gqdigdoes.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fktsv.cn/Article/details/gciqdfvaa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.epnwcf.com/Article/details/gvkstlyph.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggecnobdn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.vehdjk.com/Article/details/gjbsaqemx.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqrzmnpxw.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.yfazqb.com/Article/details/gmekwctxt.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gjkqdumli.sHtML

[T02] Kotlin：变量
来源：http://3g.yfazqb.com/Article/details/gthyzksik.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.epnwcf.com/Article/details/gbmzofvva.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gjhoyeuko.sHtML

"值: $b"
来源：http://www.share.bbcook.cn/Article/details/goxxyihfw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.sjlbkw.cn/Article/details/gliotozfh.sHtML

val n: String? = null;  n?.length
来源：http://baike.tarul.cn/Article/details/gwafkqofk.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gajslpcpn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.bbcook.cn/Article/details/gpvfmspys.sHtML

[T06] Kotlin：集合映射
来源：http://3g.tarul.cn/Article/details/gbyksmqyx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gijuldpio.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.epnwcf.com/Article/details/gbuzyxxos.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.vehdjk.com/Article/details/ggccyamuq.sHtML

[T08] Kotlin：数据类
来源：http://baike.vehdjk.com/Article/details/giybltmyi.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.tarul.cn/Article/details/gfhuexvph.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/gkjgnjjrc.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fktsv.cn/Article/details/gymwfhuvx.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.yfazqb.com/Article/details/gdgbeqrcq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.epnwcf.com/Article/details/gfqjimyzg.sHtML

[T11] Kotlin：协程
来源：http://baike.sjlbkw.cn/Article/details/gijcnzjto.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.sjlbkw.cn/Article/details/gokibwuoj.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.bbcook.cn/Article/details/gervarzmw.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.tarul.cn/Article/details/gperbvqgl.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.tarul.cn/Article/details/gvqxxckrs.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.tarul.cn/Article/details/giaopoqof.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/ggjlaoetc.sHtML

for (i in 1..10) println(i)
来源：http://blog.yfazqb.com/Article/details/gtuykaawy.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.vehdjk.com/Article/details/ggcbktdbo.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.yfazqb.com/Article/details/glbxgetqx.sHtML

[T16] Swift：Hello World
来源：http://wap.epnwcf.com/Article/details/gniazfayu.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/ggaxfikyw.sHtML

[T17] Swift：变量与常量
来源：http://read.share.sjlbkw.cn/Article/details/gqimgzvfr.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/ggrtscigs.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gnwjffnkj.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gmghtiaqs.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/gaedccndb.sHtML

if let n = opt { print(n) }
来源：http://m.share.sjlbkw.cn/Article/details/gaatzkrub.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/gwknnjqkt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.bbcook.cn/Article/details/gepvvkcjw.sHtML

[T21] Swift：遍历
来源：http://wap.yfazqb.com/Article/details/gqsslkbeq.sHtML

for x in a { print(x) }
来源：http://3g.epnwcf.com/Article/details/gvdjzfaai.sHtML

[T22] Swift：字典
来源：http://baike.fktsv.cn/Article/details/gydxrsnjt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.bbcook.cn/Article/details/gdeucuinx.sHtML

[T23] Swift：函数
来源：http://3g.sjlbkw.cn/Article/details/gtorumfhj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.bbcook.cn/Article/details/gaelrwzay.sHtML

[T24] Swift：闭包
来源：http://3g.epnwcf.com/Article/details/gtvbshbww.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gqnymrjtq.sHtML

[T25] Swift：结构体
来源：http://read.share.tarul.cn/Article/details/gxvnfxlir.sHtML

struct P { var x: Int }
来源：http://baike.fktsv.cn/Article/details/gabebxufc.sHtML

[T26] Swift：类与重写
来源：http://www.blog.tarul.cn/Article/details/gbvxslxzj.sHtML

class A: Base { override func f() {} }
来源：http://read.share.epnwcf.com/Article/details/gmufviigf.sHtML

[T27] Swift：错误处理
来源：http://3g.bbcook.cn/Article/details/giqhqpwtx.sHtML

do { try f() } catch { print(error) }
来源：http://3g.tarul.cn/Article/details/gojmhqimn.sHtML

[T28] Swift：枚举
来源：http://www.m.share.vehdjk.com/Article/details/gujllfvcw.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gbfoowifr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.tarul.cn/Article/details/gggxeqqqb.sHtML

guard let x = opt else { return }
来源：http://read.share.vehdjk.com/Article/details/gwudhrvef.sHtML

[T30] Swift：协议
来源：http://www.share.sjlbkw.cn/Article/details/gukuqvlrg.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.tarul.cn/Article/details/gszqfpxvu.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gndkmosvm.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gpqkerqfk.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.vehdjk.com/Article/details/goybqqzoi.sHtML

local a = 1
来源：http://mobile.tarul.cn/Article/details/gmthpfegl.sHtML

[T33] Lua：表（数组）
来源：http://read.share.epnwcf.com/Article/details/gfbsxoqca.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.bbcook.cn/Article/details/gsdzytrwy.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/gesdjoybb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.sjlbkw.cn/Article/details/gptoccthd.sHtML

[T35] Lua：字典表
来源：http://m.share.fktsv.cn/Article/details/gktodpers.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.epnwcf.com/Article/details/gpwetphly.sHtML

[T36] Lua：函数
来源：http://3g.yfazqb.com/Article/details/gkptdffco.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/gupaxvfsg.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gwutzknxe.sHtML

"a" .. "b"
来源：http://baike.vehdjk.com/Article/details/gxpppzaxj.sHtML

[T38] Lua：条件
来源：http://wap.sjlbkw.cn/Article/details/gzmfhnmga.sHtML

if x > 0 then print("正") end
来源：http://read.share.bbcook.cn/Article/details/gfzzmfxuc.sHtML

[T39] Lua：模式匹配
来源：http://read.share.sjlbkw.cn/Article/details/gaqetmhck.sHtML

string.find(s, "%d+")
来源：http://mobile.bbcook.cn/Article/details/gqjkehmvc.sHtML

[T40] Lua：元表
来源：http://blog.yfazqb.com/Article/details/gklqbulre.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.vehdjk.com/Article/details/gaydacqtn.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gdbjurskk.sHtML

print "Hello\n";
来源：http://baike.epnwcf.com/Article/details/grcldsraa.sHtML

[T42] Perl：变量类型
来源：http://blog.yfazqb.com/Article/details/glkswyvxp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.epnwcf.com/Article/details/gxcwqonwn.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gkzfrzwbx.sHtML

"值: $a"
来源：http://blog.fktsv.cn/Article/details/gvoigoexw.sHtML

[T44] Perl：条件
来源：http://3g.sjlbkw.cn/Article/details/gpowfiisq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.tarul.cn/Article/details/glmjbyavz.sHtML

[T45] Perl：数组遍历
来源：http://m.share.yfazqb.com/Article/details/grlaxitii.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.vehdjk.com/Article/details/gfdpcmefq.sHtML

[T46] Perl：哈希操作
来源：http://m.share.vehdjk.com/Article/details/gfjyyhlvc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.sjlbkw.cn/Article/details/gdqfyppwe.sHtML

[T47] Perl：正则捕获
来源：http://mobile.tarul.cn/Article/details/gmamkrgej.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.sjlbkw.cn/Article/details/gzbwofwaf.sHtML

[T48] Perl：正则替换
来源：http://baike.sjlbkw.cn/Article/details/gjsglzovg.sHtML

$s =~ s/old/new/g;
来源：http://mobile.yfazqb.com/Article/details/gyviqibwj.sHtML

[T49] Perl：函数
来源：http://www.blog.bbcook.cn/Article/details/gnziwpufs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gbtmcltbx.sHtML

[T50] Perl：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gjjqsgort.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fktsv.cn/Article/details/gogdegtpx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcdmwyntz.sHtML

[T51] Scala：Hello World
来源：http://baike.epnwcf.com/Article/details/gwwdikexp.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gqqzaduef.sHtML

[T52] Scala：变量
来源：http://m.share.bbcook.cn/Article/details/ggjuijilf.sHtML

val a = 1;  var b = 2
来源：http://m.share.epnwcf.com/Article/details/gpzmzktib.sHtML

[T53] Scala：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gtbjbfywl.sHtML

s"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gfupapvsa.sHtML

[T54] Scala：集合映射
来源：http://baike.epnwcf.com/Article/details/ggyxqvqfw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fktsv.cn/Article/details/gvqsdivaq.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gmofpclwu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.sjlbkw.cn/Article/details/gwpdfakfj.sHtML

[T56] Scala：样例类
来源：http://blog.fktsv.cn/Article/details/gjfayiusz.sHtML

case class User(name: String, age: Int)
来源：http://baike.sjlbkw.cn/Article/details/grnegmvxd.sHtML

[T57] Scala：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gdfunqlbv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gleyykrua.sHtML

[T58] Scala：函数定义
来源：http://read.share.epnwcf.com/Article/details/gmvfdlxmx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.bbcook.cn/Article/details/glxidwglp.sHtML

[T59] Scala：循环
来源：http://mobile.yfazqb.com/Article/details/gnfbuigeo.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.epnwcf.com/Article/details/gnqmvjxkm.sHtML

[T60] Scala：折叠
来源：http://blog.tarul.cn/Article/details/grzoldkmt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.vehdjk.com/Article/details/gcdxgvwvv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/giniexeiu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.yfazqb.com/Article/details/gpyheazho.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glxbliiwx.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.epnwcf.com/Article/details/gifvtqlyr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fktsv.cn/Article/details/goqdnkxmb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.yfazqb.com/Article/details/gbezzdwti.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fktsv.cn/Article/details/gdovbwcnf.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.epnwcf.com/Article/details/gbinpamft.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.tarul.cn/Article/details/gkwoqklyh.sHtML

[U04] Py：变量调试打印
来源：http://wap.fktsv.cn/Article/details/gtyrinbcg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.epnwcf.com/Article/details/gsuzjdowf.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.bbcook.cn/Article/details/gqmeprtsp.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/gdgtkwyra.sHtML

[U06] Py：合并两个字典
来源：http://baike.fktsv.cn/Article/details/gbggzdzae.sHtML

{**a, **b}
来源：http://baike.epnwcf.com/Article/details/gjldrgbkq.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.yfazqb.com/Article/details/ggcqvzbgk.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.epnwcf.com/Article/details/gnwmvlxdf.sHtML

[U08] Py：展平二维列表
来源：http://m.share.yfazqb.com/Article/details/gefxrnnzr.sHtML

[y for x in nested for y in x]
来源：http://m.share.sjlbkw.cn/Article/details/gltyyyfec.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.tarul.cn/Article/details/gsvmufoat.sHtML

max(d, key=d.get)
来源：http://mobile.yfazqb.com/Article/details/gdxaklnpb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.bbcook.cn/Article/details/gcppclwkj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.vehdjk.com/Article/details/gvogclsym.sHtML

[U11] Py：生成器表达式
来源：http://wap.tarul.cn/Article/details/gbpuamdor.sHtML

(x * 2 for x in arr)
来源：http://blog.epnwcf.com/Article/details/gqwlypaui.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fktsv.cn/Article/details/gsksupfyi.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.bbcook.cn/Article/details/gzhkubukk.sHtML

[U13] Py：固定长度队列
来源：http://blog.fktsv.cn/Article/details/gimamsqre.sHtML

deque(maxlen=10)
来源：http://www.blog.epnwcf.com/Article/details/gqbrmxddv.sHtML

[U14] Py：分组收集到列表
来源：http://wap.epnwcf.com/Article/details/gdxbivzli.sHtML

defaultdict(list)
来源：http://blog.sjlbkw.cn/Article/details/gobuzcweh.sHtML

[U15] Py：高精度计时
来源：http://mobile.vehdjk.com/Article/details/gevnucvve.sHtML

t = time.perf_counter()
来源：http://read.share.epnwcf.com/Article/details/gynjohjjl.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fktsv.cn/Article/details/gsiqbjmgk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.bbcook.cn/Article/details/gjzyrhikv.sHtML

[U17] Py：初始化日志
来源：http://mobile.epnwcf.com/Article/details/gwkvhwopt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.bbcook.cn/Article/details/gghpkufce.sHtML

[U18] Py：预编译正则
来源：http://blog.tarul.cn/Article/details/givvligdx.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fktsv.cn/Article/details/gdrwbrihl.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fktsv.cn/Article/details/gomrvvads.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.tarul.cn/Article/details/gprawuruw.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.yfazqb.com/Article/details/ghqdhammj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fktsv.cn/Article/details/gnwcnyqyh.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.bbcook.cn/Article/details/gcpplxfep.sHtML

@contextlib.contextmanager
来源：http://www.m.share.yfazqb.com/Article/details/gggjafaom.sHtML

[U22] Py：矩阵转置
来源：http://www.share.epnwcf.com/Article/details/gmcmbvypx.sHtML

list(zip(*m))
来源：http://blog.sjlbkw.cn/Article/details/gokecyvuv.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.yfazqb.com/Article/details/ghclzcimf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.yfazqb.com/Article/details/gltghwyiw.sHtML

[U24] Py：路径操作
来源：http://www.share.bbcook.cn/Article/details/gpsmftnhj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/ghyzagpio.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.epnwcf.com/Article/details/gqonhqhas.sHtML

csv.DictReader(f)
来源：http://www.m.share.epnwcf.com/Article/details/gavwoxpsm.sHtML

[U26] Py：并发下载
来源：http://blog.fktsv.cn/Article/details/gfvvwiehv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.vehdjk.com/Article/details/gjdosfyjh.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.epnwcf.com/Article/details/gxsquvcpu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.yfazqb.com/Article/details/gloalupyx.sHtML

[U28] Py：类型别名
来源：http://wap.tarul.cn/Article/details/gqugiyysn.sHtML

UserId = int
来源：http://mobile.sjlbkw.cn/Article/details/gcennxpdw.sHtML

[U29] Py：属性校验
来源：http://wap.fktsv.cn/Article/details/gkineecvv.sHtML

@property 与 @x.setter 配合
来源：http://blog.bbcook.cn/Article/details/giacyvlmy.sHtML

[U30] Py：数据类
来源：http://mobile.sjlbkw.cn/Article/details/gqzmztfre.sHtML

@dataclass(slots=True)
来源：http://wap.tarul.cn/Article/details/grwgmeeon.sHtML

[U31] Py：单测
来源：http://www.m.share.epnwcf.com/Article/details/ggzixunne.sHtML

python -m pytest -q
来源：http://www.blog.vehdjk.com/Article/details/gjipqkwpd.sHtML

[U32] Py：代码格式化
来源：http://www.blog.sjlbkw.cn/Article/details/giptybhbu.sHtML

ruff format . && ruff check --fix .
来源：http://baike.yfazqb.com/Article/details/gdwqyfajp.sHtML

[U33] Py：打包发布
来源：http://m.share.vehdjk.com/Article/details/gstqjfdah.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.epnwcf.com/Article/details/gblagjidn.sHtML

[U34] Py：判断编码
来源：http://m.share.yfazqb.com/Article/details/gcpymkrzf.sHtML

chardet.detect(raw)
来源：http://baike.yfazqb.com/Article/details/gsbidkstv.sHtML

[U35] Py：发送邮件
来源：http://www.blog.bbcook.cn/Article/details/gglpkebur.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fktsv.cn/Article/details/gsfkhmzck.sHtML

[U36] Py：定时任务
来源：http://www.share.tarul.cn/Article/details/grhdzrzwm.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.bbcook.cn/Article/details/gsykkamyh.sHtML

[U37] Py：读写 Excel
来源：http://blog.fktsv.cn/Article/details/gifmguspt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fktsv.cn/Article/details/gnxyoqzqv.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.vehdjk.com/Article/details/gilcgwbek.sHtML

Path(__file__).resolve().parent
来源：http://m.share.sjlbkw.cn/Article/details/gyopzjgnv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.vehdjk.com/Article/details/gtrmlyacv.sHtML

sys.stdout.isatty()
来源：http://www.blog.vehdjk.com/Article/details/gbnzgsast.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.bbcook.cn/Article/details/gmmceixrk.sHtML

print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gugbgoxos.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.vehdjk.com/Article/details/gvlvoqdud.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.yfazqb.com/Article/details/gomrmrxds.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.bbcook.cn/Article/details/gdeflqluk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fktsv.cn/Article/details/gmvhshhur.sHtML


<!-- 参考信息 -->