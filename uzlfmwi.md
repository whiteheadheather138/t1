代发 wailian999

int main(int argc, char **argv)
来源：http://www.m.share.tarul.cn/Article/details/grsipqhfs.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/grpwjvhqj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gowsgcpjk.sHtML

[S20] C：二分查找
来源：http://www.share.vehdjk.com/Article/details/gpysryvca.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gbxdhvggr.sHtML

[S21] C：字符类别判断
来源：http://www.share.bbcook.cn/Article/details/gnqyifjju.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/genmcdfqq.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gluccjyph.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.tarul.cn/Article/details/gqwqbxtnz.sHtML

[S23] C：随机数
来源：http://read.share.bbcook.cn/Article/details/gzfslvdxq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/gwanlfmyq.sHtML

[S24] C：获取本地时间
来源：http://wap.epnwcf.com/Article/details/gdjfyjhfj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.tarul.cn/Article/details/grxzlsgcx.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fktsv.cn/Article/details/gjhhrygky.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/grksjhwtv.sHtML

[S26] C：内存清零
来源：http://3g.yfazqb.com/Article/details/glmylkrhm.sHtML

memset(a, 0, sizeof a);
来源：http://blog.sjlbkw.cn/Article/details/gvprqykqs.sHtML

[S27] C：定义常量
来源：http://blog.sjlbkw.cn/Article/details/ggwloakag.sHtML

const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gosukhrnj.sHtML

[S28] C：静态变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzuwqyls.sHtML

static int counter = 0;
来源：http://mobile.bbcook.cn/Article/details/gkqwhznlv.sHtML

[S29] C：变参函数
来源：http://wap.tarul.cn/Article/details/gtflxeeot.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/gjdszhuyh.sHtML

[S30] C：头文件保护
来源：http://read.share.fktsv.cn/Article/details/gnzgptmbt.sHtML

#ifndef X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gihwckhzt.sHtML

#define X_H
来源：http://read.share.epnwcf.com/Article/details/gtxqudorc.sHtML

#endif
来源：http://3g.bbcook.cn/Article/details/gbafnhokp.sHtML

[S31] C++：Hello World
来源：http://blog.vehdjk.com/Article/details/gbndtgwml.sHtML

#include <iostream>
来源：http://wap.bbcook.cn/Article/details/gscnifayi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.sjlbkw.cn/Article/details/gfeptgpre.sHtML

[S32] C++：字符串
来源：http://www.blog.vehdjk.com/Article/details/ghboyelzi.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fktsv.cn/Article/details/gtmnbgheo.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/gcmfvabdi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gueppkruk.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/gyduyiezq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.sjlbkw.cn/Article/details/gyurwcgjr.sHtML

[S35] C++：map
来源：http://mobile.yfazqb.com/Article/details/gciwmlano.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gxgecfyac.sHtML

[S36] C++：unordered_map
来源：http://read.share.epnwcf.com/Article/details/grploedto.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gkjrufqpq.sHtML

[S37] C++：set
来源：http://m.share.bbcook.cn/Article/details/gckxtcham.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.vehdjk.com/Article/details/gcjnubrgy.sHtML

[S38] C++：排序
来源：http://blog.bbcook.cn/Article/details/gxpujcwjs.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.bbcook.cn/Article/details/gbsojoipt.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.sjlbkw.cn/Article/details/gkwsdjecn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fktsv.cn/Article/details/gmsxeehmn.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/gnfzbaytj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.vehdjk.com/Article/details/gnbbikjnv.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fktsv.cn/Article/details/grjzxkbmz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.yfazqb.com/Article/details/gkgmcnkds.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fktsv.cn/Article/details/gpyoanvjl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.yfazqb.com/Article/details/grlechcru.sHtML

[S43] C++：智能指针
来源：http://3g.tarul.cn/Article/details/gouwcyyya.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.sjlbkw.cn/Article/details/gexxzgfse.sHtML

[S44] C++：引用传参
来源：http://www.m.share.epnwcf.com/Article/details/gftznuqpc.sHtML

void inc(int &x) { ++x; }
来源：http://baike.sjlbkw.cn/Article/details/gdohxsixg.sHtML

[S45] C++：lambda
来源：http://read.share.vehdjk.com/Article/details/gadljtwzd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/grxwzyaig.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/gdyqihouh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/gwncvvexw.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.yfazqb.com/Article/details/gnjlixuxq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.yfazqb.com/Article/details/gjjqbzwnl.sHtML

[S48] C++：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gsarubtmt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.epnwcf.com/Article/details/gjrbjtzzo.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gfvwmipak.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gbbvuziix.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.bbcook.cn/Article/details/gjuksfqbk.sHtML

[S50] C++：格式化数字
来源：http://read.share.sjlbkw.cn/Article/details/ghcvwjikh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gkdalnzfi.sHtML

[S51] C++：显式类型转换
来源：http://wap.epnwcf.com/Article/details/gnuqrqsmx.sHtML

static_cast<double>(a) / b
来源：http://wap.yfazqb.com/Article/details/gvxqifshb.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.vehdjk.com/Article/details/gkylywwfr.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.sjlbkw.cn/Article/details/gdzykkohb.sHtML

[S53] C++：移动语义
来源：http://blog.yfazqb.com/Article/details/gmuvnewde.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.tarul.cn/Article/details/gunegxlxg.sHtML

[S54] C++：异常处理
来源：http://mobile.yfazqb.com/Article/details/gumhatkey.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/gkwgdbqje.sHtML

[S55] C++：结构化绑定
来源：http://m.share.vehdjk.com/Article/details/gvvipmzol.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.vehdjk.com/Article/details/gdvyomrey.sHtML

[S56] C++：optional
来源：http://baike.vehdjk.com/Article/details/gxismjght.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.yfazqb.com/Article/details/gpeqfoqee.sHtML

[S57] C++：编译期常量
来源：http://mobile.bbcook.cn/Article/details/gxecynutd.sHtML

constexpr int N = 10;
来源：http://www.blog.epnwcf.com/Article/details/gswdoxyrs.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fktsv.cn/Article/details/ggqdrogoc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gerbgihhu.sHtML

[S59] C++：静态断言
来源：http://www.m.share.epnwcf.com/Article/details/gwcfzfjqx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.bbcook.cn/Article/details/gtrnyypfg.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.bbcook.cn/Article/details/gyhmwvgmv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/geakkkmag.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqkdqeusp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gygeqbmdy.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/golpnaowd.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gmznyrmcv.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gkwdeadzo.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gblijrmxs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.vehdjk.com/Article/details/gzvgumdmd.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.tarul.cn/Article/details/gclrnuydr.sHtML

"值: $b"
来源：http://mobile.fktsv.cn/Article/details/gwuymmptv.sHtML

[T04] Kotlin：空安全
来源：http://www.share.sjlbkw.cn/Article/details/gwurgliju.sHtML

val n: String? = null;  n?.length
来源：http://www.share.vehdjk.com/Article/details/gcbnzahap.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.sjlbkw.cn/Article/details/gzgtyvrwy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.epnwcf.com/Article/details/gntcqykzg.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.epnwcf.com/Article/details/guxsfppju.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/geiydppwa.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.vehdjk.com/Article/details/gpliivvsi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.vehdjk.com/Article/details/gvtfyzppr.sHtML

[T08] Kotlin：数据类
来源：http://read.share.yfazqb.com/Article/details/ggleqgzfv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fktsv.cn/Article/details/gqmfeggax.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/gheslklfv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.tarul.cn/Article/details/gljuinfvw.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.epnwcf.com/Article/details/gylikaman.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/gdsfaukvg.sHtML

[T11] Kotlin：协程
来源：http://www.share.bbcook.cn/Article/details/gzyawbdni.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.bbcook.cn/Article/details/gmzrngten.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.yfazqb.com/Article/details/gdtykdfhi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbphrhtz.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.vehdjk.com/Article/details/gummtolbs.sHtML

val m = mapOf("a" to 1)
来源：http://3g.tarul.cn/Article/details/ghnisqxif.sHtML

[T14] Kotlin：循环
来源：http://baike.yfazqb.com/Article/details/gkzfvehhf.sHtML

for (i in 1..10) println(i)
来源：http://m.share.tarul.cn/Article/details/giwdhwzmu.sHtML

[T15] Kotlin：接口
来源：http://3g.bbcook.cn/Article/details/gvsmglhhz.sHtML

interface Shape { fun area(): Double }
来源：http://wap.sjlbkw.cn/Article/details/gkqafbznz.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gilfrnscy.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/galwymhfb.sHtML

[T17] Swift：变量与常量
来源：http://www.share.bbcook.cn/Article/details/gnrpsclnm.sHtML

var a = 1;  let b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gdapenkzz.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gkpdyzwzm.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gblqzorgx.sHtML

[T19] Swift：可选绑定
来源：http://m.share.epnwcf.com/Article/details/glvkeiwot.sHtML

if let n = opt { print(n) }
来源：http://www.share.fktsv.cn/Article/details/greqeszwd.sHtML

[T20] Swift：数组操作
来源：http://www.share.epnwcf.com/Article/details/gvenqpqjq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.vehdjk.com/Article/details/gnxujtfvh.sHtML

[T21] Swift：遍历
来源：http://m.share.sjlbkw.cn/Article/details/gaeqcobls.sHtML

for x in a { print(x) }
来源：http://mobile.tarul.cn/Article/details/gatpswycf.sHtML

[T22] Swift：字典
来源：http://www.m.share.bbcook.cn/Article/details/gymxtlfxx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.sjlbkw.cn/Article/details/gdalfrwoj.sHtML

[T23] Swift：函数
来源：http://baike.tarul.cn/Article/details/gmdqrzcnd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.bbcook.cn/Article/details/gcrvewzyj.sHtML

[T24] Swift：闭包
来源：http://www.blog.vehdjk.com/Article/details/gqqrrkcoc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.tarul.cn/Article/details/gjqvdhaei.sHtML

[T25] Swift：结构体
来源：http://read.share.yfazqb.com/Article/details/gwvcucmhy.sHtML

struct P { var x: Int }
来源：http://mobile.bbcook.cn/Article/details/gaegmdrck.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.bbcook.cn/Article/details/gsbpzwarw.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fktsv.cn/Article/details/gbncpsasc.sHtML

[T27] Swift：错误处理
来源：http://3g.sjlbkw.cn/Article/details/ghofuufcw.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.yfazqb.com/Article/details/gkvvpojsp.sHtML

[T28] Swift：枚举
来源：http://blog.yfazqb.com/Article/details/gonftyrfl.sHtML

enum Color { case red, green }
来源：http://mobile.yfazqb.com/Article/details/ghbxthhdu.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.tarul.cn/Article/details/gxhquofom.sHtML

guard let x = opt else { return }
来源：http://read.share.tarul.cn/Article/details/gxiyqftvw.sHtML

[T30] Swift：协议
来源：http://baike.tarul.cn/Article/details/gslgjszam.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.epnwcf.com/Article/details/gmatiogtw.sHtML

[T31] Lua：Hello World
来源：http://baike.vehdjk.com/Article/details/gxvifnuvs.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/gyayfeeel.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.tarul.cn/Article/details/gbbridxdo.sHtML

local a = 1
来源：http://blog.vehdjk.com/Article/details/guadnfsrf.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.yfazqb.com/Article/details/gjlwrnyyv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.vehdjk.com/Article/details/gznwnodlb.sHtML

[T34] Lua：遍历表
来源：http://baike.sjlbkw.cn/Article/details/grpxiaqdh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/goemvrhpc.sHtML

[T35] Lua：字典表
来源：http://baike.vehdjk.com/Article/details/gamucyiva.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.yfazqb.com/Article/details/grutgyuus.sHtML

[T36] Lua：函数
来源：http://www.blog.tarul.cn/Article/details/gqlsodpbc.sHtML

function add(a, b) return a + b end
来源：http://m.share.epnwcf.com/Article/details/gnrehrmqf.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.vehdjk.com/Article/details/gymveuovn.sHtML

"a" .. "b"
来源：http://m.share.yfazqb.com/Article/details/gbjpxghkt.sHtML

[T38] Lua：条件
来源：http://read.share.fktsv.cn/Article/details/gwtgpsmsu.sHtML

if x > 0 then print("正") end
来源：http://read.share.vehdjk.com/Article/details/gxhqgghje.sHtML

[T39] Lua：模式匹配
来源：http://mobile.yfazqb.com/Article/details/grlkgjnkp.sHtML

string.find(s, "%d+")
来源：http://wap.fktsv.cn/Article/details/gizvpgawm.sHtML

[T40] Lua：元表
来源：http://baike.yfazqb.com/Article/details/gstbaefgd.sHtML

setmetatable({}, { __index = base })
来源：http://blog.vehdjk.com/Article/details/gdgtrzgqa.sHtML

[T41] Perl：Hello World
来源：http://baike.tarul.cn/Article/details/gmvnrfigb.sHtML

print "Hello\n";
来源：http://read.share.tarul.cn/Article/details/gtytavcyt.sHtML

[T42] Perl：变量类型
来源：http://3g.vehdjk.com/Article/details/gxjcqmqef.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.yfazqb.com/Article/details/guvasymts.sHtML

[T43] Perl：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gujnrfuur.sHtML

"值: $a"
来源：http://m.share.yfazqb.com/Article/details/gytstykgf.sHtML

[T44] Perl：条件
来源：http://www.share.tarul.cn/Article/details/gnldswpyk.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.bbcook.cn/Article/details/gpytregow.sHtML

[T45] Perl：数组遍历
来源：http://www.share.bbcook.cn/Article/details/gjhxyolys.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.bbcook.cn/Article/details/gooycrodh.sHtML

[T46] Perl：哈希操作
来源：http://3g.epnwcf.com/Article/details/gyrofbwag.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fktsv.cn/Article/details/gxkzzsclm.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.tarul.cn/Article/details/gvvpvbnfa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.epnwcf.com/Article/details/glvgqvxti.sHtML

[T48] Perl：正则替换
来源：http://mobile.tarul.cn/Article/details/gkmzoxjdu.sHtML

$s =~ s/old/new/g;
来源：http://baike.epnwcf.com/Article/details/gyjpxeqhf.sHtML

[T49] Perl：函数
来源：http://baike.vehdjk.com/Article/details/gyxiwzbcy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gxoakturm.sHtML

[T50] Perl：逐行读文件
来源：http://blog.tarul.cn/Article/details/gtujimriy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.yfazqb.com/Article/details/gkwcgdjrk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.bbcook.cn/Article/details/gxcpozpgp.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/grbefidex.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gxgmjtpcr.sHtML

[T52] Scala：变量
来源：http://3g.epnwcf.com/Article/details/gdvitwten.sHtML

val a = 1;  var b = 2
来源：http://m.share.epnwcf.com/Article/details/gbblubxyz.sHtML

[T53] Scala：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gvdhstqgj.sHtML

s"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gsgvxsynh.sHtML

[T54] Scala：集合映射
来源：http://3g.vehdjk.com/Article/details/gvybmaroj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.sjlbkw.cn/Article/details/gsrirpftk.sHtML

[T55] Scala：集合过滤
来源：http://read.share.tarul.cn/Article/details/gpgomhfsf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.epnwcf.com/Article/details/guvrunqel.sHtML

[T56] Scala：样例类
来源：http://wap.yfazqb.com/Article/details/gsmtpftjq.sHtML

case class User(name: String, age: Int)
来源：http://blog.sjlbkw.cn/Article/details/glueiomhc.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/gvusvgezm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyeieysux.sHtML

[T58] Scala：函数定义
来源：http://m.share.tarul.cn/Article/details/galuxqzmg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.bbcook.cn/Article/details/gjcyiobxt.sHtML

[T59] Scala：循环
来源：http://read.share.bbcook.cn/Article/details/ghefpnevz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gfmkhaljx.sHtML

[T60] Scala：折叠
来源：http://3g.yfazqb.com/Article/details/gjqtnmfws.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.vehdjk.com/Article/details/gzcddrtfe.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwsmbeuee.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.epnwcf.com/Article/details/gwgyykjgu.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gztvrajfa.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.epnwcf.com/Article/details/gxzhfpmcc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.vehdjk.com/Article/details/gorglvqlk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.bbcook.cn/Article/details/guukfhaps.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.epnwcf.com/Article/details/gapialjol.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.sjlbkw.cn/Article/details/gxthhaxvl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.yfazqb.com/Article/details/gyqyduowi.sHtML

[U04] Py：变量调试打印
来源：http://blog.epnwcf.com/Article/details/gaakajmsg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.yfazqb.com/Article/details/gpjyfuzkl.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.epnwcf.com/Article/details/gbdbutdyc.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.bbcook.cn/Article/details/gquyfixot.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.vehdjk.com/Article/details/gyhprkjwk.sHtML

{**a, **b}
来源：http://wap.epnwcf.com/Article/details/gxirayzmo.sHtML

[U07] Py：反转字典键值
来源：http://baike.yfazqb.com/Article/details/gkyixnqoj.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fktsv.cn/Article/details/gkimzjvsf.sHtML

[U08] Py：展平二维列表
来源：http://m.share.yfazqb.com/Article/details/gwzqolbnz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.vehdjk.com/Article/details/gmxigevgg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.yfazqb.com/Article/details/gclhsbanz.sHtML

max(d, key=d.get)
来源：http://wap.fktsv.cn/Article/details/gqulsdtdh.sHtML

[U10] Py：按值排序字典
来源：http://blog.tarul.cn/Article/details/gylatpwtg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.yfazqb.com/Article/details/gwvzezhzr.sHtML

[U11] Py：生成器表达式
来源：http://baike.tarul.cn/Article/details/gvqksarye.sHtML

(x * 2 for x in arr)
来源：http://baike.tarul.cn/Article/details/gfdmvhshk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fktsv.cn/Article/details/gytlcearq.sHtML

Counter(arr).most_common(3)
来源：http://baike.sjlbkw.cn/Article/details/gqkrrmvuq.sHtML

[U13] Py：固定长度队列
来源：http://3g.bbcook.cn/Article/details/gcbakvkmk.sHtML

deque(maxlen=10)
来源：http://3g.yfazqb.com/Article/details/gbmnhdxmq.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.epnwcf.com/Article/details/gbdrvcmvv.sHtML

defaultdict(list)
来源：http://3g.tarul.cn/Article/details/gkewqfbsi.sHtML

[U15] Py：高精度计时
来源：http://3g.tarul.cn/Article/details/gmswandlg.sHtML

t = time.perf_counter()
来源：http://m.share.sjlbkw.cn/Article/details/gmenhpaul.sHtML

[U16] Py：命令行参数解析
来源：http://3g.bbcook.cn/Article/details/gpzbzufou.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.sjlbkw.cn/Article/details/gwrdkpkil.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fktsv.cn/Article/details/gfsdbtrbx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/gjfcpydej.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/gxfiuqieq.sHtML

pat = re.compile(r"\d+")
来源：http://3g.epnwcf.com/Article/details/gcqaljkwu.sHtML

[U19] Py：正则替换带回调
来源：http://3g.epnwcf.com/Article/details/gnnudakmd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.vehdjk.com/Article/details/giqxlevgj.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fktsv.cn/Article/details/getlpuzqf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fktsv.cn/Article/details/gkkciwtmi.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fktsv.cn/Article/details/gcuzrdpgd.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/geackogpw.sHtML

[U22] Py：矩阵转置
来源：http://wap.sjlbkw.cn/Article/details/gbrpnynla.sHtML

list(zip(*m))
来源：http://read.share.vehdjk.com/Article/details/gpmejzbex.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.vehdjk.com/Article/details/gmvvverhc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.vehdjk.com/Article/details/gwqyqkezq.sHtML

[U24] Py：路径操作
来源：http://blog.fktsv.cn/Article/details/gquzymiyv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gacvuxdty.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.epnwcf.com/Article/details/gemuhkxvd.sHtML

csv.DictReader(f)
来源：http://3g.yfazqb.com/Article/details/gpgxmmtbg.sHtML

[U26] Py：并发下载
来源：http://3g.bbcook.cn/Article/details/gisnagvxl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.vehdjk.com/Article/details/gsbupakgu.sHtML

[U27] Py：异步 HTTP
来源：http://blog.vehdjk.com/Article/details/grvlzcssd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.sjlbkw.cn/Article/details/gehrdemvx.sHtML

[U28] Py：类型别名
来源：http://www.m.share.epnwcf.com/Article/details/gonnzebht.sHtML

UserId = int
来源：http://baike.vehdjk.com/Article/details/gjpxdnjri.sHtML

[U29] Py：属性校验
来源：http://www.m.share.vehdjk.com/Article/details/gdsxhjehz.sHtML

@property 与 @x.setter 配合
来源：http://m.share.bbcook.cn/Article/details/gslmzczfm.sHtML

[U30] Py：数据类
来源：http://www.share.tarul.cn/Article/details/ggxmvqffw.sHtML

@dataclass(slots=True)
来源：http://mobile.tarul.cn/Article/details/gqesjxvbi.sHtML

[U31] Py：单测
来源：http://mobile.fktsv.cn/Article/details/gxgqefycx.sHtML

python -m pytest -q
来源：http://www.m.share.bbcook.cn/Article/details/gmjadesvo.sHtML

[U32] Py：代码格式化
来源：http://m.share.bbcook.cn/Article/details/gzkaleraj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.vehdjk.com/Article/details/gmrxwnkal.sHtML

[U33] Py：打包发布
来源：http://3g.fktsv.cn/Article/details/gsnlyqeru.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.epnwcf.com/Article/details/ggmdwdomi.sHtML

[U34] Py：判断编码
来源：http://www.m.share.vehdjk.com/Article/details/gkxzakipr.sHtML

chardet.detect(raw)
来源：http://read.share.epnwcf.com/Article/details/gqanztemr.sHtML

[U35] Py：发送邮件
来源：http://read.share.tarul.cn/Article/details/glvqtbcip.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.epnwcf.com/Article/details/gxsgnvqhx.sHtML

[U36] Py：定时任务
来源：http://mobile.epnwcf.com/Article/details/gfltzixzv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.bbcook.cn/Article/details/gekxtpiuf.sHtML

[U37] Py：读写 Excel
来源：http://read.share.yfazqb.com/Article/details/gvldabgwt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.yfazqb.com/Article/details/goitsgfwh.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.yfazqb.com/Article/details/gomrqotch.sHtML

Path(__file__).resolve().parent
来源：http://baike.tarul.cn/Article/details/ggyffxkbr.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.epnwcf.com/Article/details/gmbayrkiu.sHtML

sys.stdout.isatty()
来源：http://mobile.tarul.cn/Article/details/gzzjdlode.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.vehdjk.com/Article/details/gzakpgonj.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gyqlywjyc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.epnwcf.com/Article/details/guvvxexlm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.epnwcf.com/Article/details/ggdtdmxzg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.tarul.cn/Article/details/grjwwrdar.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.tarul.cn/Article/details/gqciuikff.sHtML


<!-- 参考信息 -->