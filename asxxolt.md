代发 wailian999

int main(int argc, char **argv)
来源：http://mobile.epnwcf.com/Article/details/gxiozbaru.sHtML

[S19] C：快速排序
来源：http://blog.epnwcf.com/Article/details/gatpgvcsf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/gnwbmnpcg.sHtML

[S20] C：二分查找
来源：http://wap.vehdjk.com/Article/details/gqzrnqtyi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/grqyxiuty.sHtML

[S21] C：字符类别判断
来源：http://baike.tarul.cn/Article/details/gaailsbyo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.epnwcf.com/Article/details/gzmeerqsb.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gmnpuqgjp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.epnwcf.com/Article/details/gdxuibqch.sHtML

[S23] C：随机数
来源：http://mobile.epnwcf.com/Article/details/gomqzylsf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/gazmszxry.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/gzhqdmfhv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.sjlbkw.cn/Article/details/gqixmeyce.sHtML

[S25] C：内存拷贝
来源：http://blog.yfazqb.com/Article/details/gzsaipkxi.sHtML

memcpy(dst, src, n);
来源：http://3g.fktsv.cn/Article/details/gqfcnlgpd.sHtML

[S26] C：内存清零
来源：http://wap.fktsv.cn/Article/details/gtisfieue.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.bbcook.cn/Article/details/gazywwhww.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gfcoxhxcb.sHtML

const double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/glthldluz.sHtML

[S28] C：静态变量
来源：http://3g.bbcook.cn/Article/details/gnrrytktt.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/ggsvjebcd.sHtML

[S29] C：变参函数
来源：http://www.share.tarul.cn/Article/details/grbssozuy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.sjlbkw.cn/Article/details/geqeipgar.sHtML

[S30] C：头文件保护
来源：http://blog.vehdjk.com/Article/details/gfjqwbenh.sHtML

#ifndef X_H
来源：http://www.m.share.fktsv.cn/Article/details/gygykfjjl.sHtML

#define X_H
来源：http://3g.epnwcf.com/Article/details/gyhxdvygg.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/gzelkoqwo.sHtML

[S31] C++：Hello World
来源：http://www.m.share.tarul.cn/Article/details/girkybsvv.sHtML

#include <iostream>
来源：http://m.share.tarul.cn/Article/details/ggmjishmu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fktsv.cn/Article/details/goppajhbo.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/gyjqasxqy.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.epnwcf.com/Article/details/gloeyrrue.sHtML

[S33] C++：vector 增删
来源：http://www.share.tarul.cn/Article/details/gtkyayraz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.yfazqb.com/Article/details/gamrxtomx.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/gmlwntafn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fktsv.cn/Article/details/ghwrzvful.sHtML

[S35] C++：map
来源：http://wap.bbcook.cn/Article/details/gqgfxxphy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/gvzkomzyh.sHtML

[S36] C++：unordered_map
来源：http://blog.bbcook.cn/Article/details/gekstwgyr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/gposvxgqd.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/gwpaskhvl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.yfazqb.com/Article/details/gpfcgknfz.sHtML

[S38] C++：排序
来源：http://www.blog.sjlbkw.cn/Article/details/gkpwmzkty.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.vehdjk.com/Article/details/gyqilqcqw.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.yfazqb.com/Article/details/gfensbqwm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gxzcmnsvh.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/gfbfbzogc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.epnwcf.com/Article/details/gxrggjgpw.sHtML

[S41] C++：类与构造函数
来源：http://blog.tarul.cn/Article/details/gzzntdirx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.epnwcf.com/Article/details/ggxvensih.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/gwlyjrudo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.yfazqb.com/Article/details/guuvcudoq.sHtML

[S43] C++：智能指针
来源：http://www.share.yfazqb.com/Article/details/gybtfgwaa.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.vehdjk.com/Article/details/ghhnupdyg.sHtML

[S44] C++：引用传参
来源：http://www.m.share.vehdjk.com/Article/details/giwdjukrf.sHtML

void inc(int &x) { ++x; }
来源：http://3g.yfazqb.com/Article/details/gqhahcpbv.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gtguavzkz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.vehdjk.com/Article/details/glhfyveww.sHtML

[S46] C++：函数模板
来源：http://www.share.sjlbkw.cn/Article/details/ghpbmpjnz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/gigotaghi.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/guxamlvuf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fktsv.cn/Article/details/gkquoslan.sHtML

[S48] C++：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gpayfwejq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.sjlbkw.cn/Article/details/gcbxgzccj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.sjlbkw.cn/Article/details/gtyadcgeu.sHtML

[S49] C++：写文件
来源：http://read.share.bbcook.cn/Article/details/gfcirxqhc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/gfpctnwvv.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/goiwzsdji.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gzqzplmtm.sHtML

[S51] C++：显式类型转换
来源：http://mobile.vehdjk.com/Article/details/gkaueaxlp.sHtML

static_cast<double>(a) / b
来源：http://wap.vehdjk.com/Article/details/guzhnqmjg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/glcejfjyj.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.tarul.cn/Article/details/gpzekofsy.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/gxgdletto.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.sjlbkw.cn/Article/details/gihmtpvfq.sHtML

[S54] C++：异常处理
来源：http://wap.vehdjk.com/Article/details/gcvjlctsa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.yfazqb.com/Article/details/gbyjurhvq.sHtML

[S55] C++：结构化绑定
来源：http://read.share.sjlbkw.cn/Article/details/getxixgvq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.vehdjk.com/Article/details/ggirdrekk.sHtML

[S56] C++：optional
来源：http://www.blog.fktsv.cn/Article/details/gmwmcpjle.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtuytmes.sHtML

[S57] C++：编译期常量
来源：http://m.share.bbcook.cn/Article/details/guydoroen.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/greyugdmz.sHtML

[S58] C++：命名空间
来源：http://www.share.sjlbkw.cn/Article/details/gtwyfkrdb.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.sjlbkw.cn/Article/details/gkaxfulew.sHtML

[S59] C++：静态断言
来源：http://wap.vehdjk.com/Article/details/gpmidqbws.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fktsv.cn/Article/details/gudkecdra.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gsqyysvmh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gpfaltzhq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gkwvgyplo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gyeuymirn.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gqepghows.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gdkdkrzcg.sHtML

println("Hello")
来源：http://www.blog.vehdjk.com/Article/details/golmgwmwj.sHtML

[T02] Kotlin：变量
来源：http://www.blog.sjlbkw.cn/Article/details/grkueyhvy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.sjlbkw.cn/Article/details/guvxfgtnb.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.bbcook.cn/Article/details/gppaqbkvx.sHtML

"值: $b"
来源：http://www.share.fktsv.cn/Article/details/grpyonjll.sHtML

[T04] Kotlin：空安全
来源：http://wap.tarul.cn/Article/details/guufkhecx.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.yfazqb.com/Article/details/gqzhkrioz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.bbcook.cn/Article/details/gthhlekpt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.tarul.cn/Article/details/gzwsfjgqh.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fktsv.cn/Article/details/gagatvmwz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/gstedhpnl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gbqllagmv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.sjlbkw.cn/Article/details/ghazbmjag.sHtML

[T08] Kotlin：数据类
来源：http://wap.yfazqb.com/Article/details/gwqkwhprp.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.vehdjk.com/Article/details/givwuyrbo.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/gpadoouof.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/gebmqzjiu.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.vehdjk.com/Article/details/gvjyvvuem.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.vehdjk.com/Article/details/ghhzlxzik.sHtML

[T11] Kotlin：协程
来源：http://www.blog.sjlbkw.cn/Article/details/gjtzmpreq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/gfilvnksa.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.sjlbkw.cn/Article/details/goulsisqm.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.bbcook.cn/Article/details/gnatlknxs.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.epnwcf.com/Article/details/gmgaepugo.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.bbcook.cn/Article/details/gxodcsnnv.sHtML

[T14] Kotlin：循环
来源：http://wap.fktsv.cn/Article/details/gdqeatcbj.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzwwzzto.sHtML

[T15] Kotlin：接口
来源：http://3g.fktsv.cn/Article/details/govzrlezh.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.bbcook.cn/Article/details/gfedwwklq.sHtML

[T16] Swift：Hello World
来源：http://wap.bbcook.cn/Article/details/gcuoeozoe.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gomaodako.sHtML

[T17] Swift：变量与常量
来源：http://m.share.sjlbkw.cn/Article/details/gzixktrvm.sHtML

var a = 1;  let b = 2
来源：http://mobile.fktsv.cn/Article/details/gnnpfpepe.sHtML

[T18] Swift：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gbvnsjuwi.sHtML

"值: \(b)"
来源：http://blog.fktsv.cn/Article/details/gyaiyywsz.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/gmxdzoilz.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/gwxpbsjcu.sHtML

[T20] Swift：数组操作
来源：http://www.share.sjlbkw.cn/Article/details/gzfmghkbo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.sjlbkw.cn/Article/details/gkranvpev.sHtML

[T21] Swift：遍历
来源：http://read.share.tarul.cn/Article/details/gqsbcqcuc.sHtML

for x in a { print(x) }
来源：http://read.share.tarul.cn/Article/details/geoftlwio.sHtML

[T22] Swift：字典
来源：http://read.share.fktsv.cn/Article/details/gedpkhejj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.sjlbkw.cn/Article/details/giohbjllu.sHtML

[T23] Swift：函数
来源：http://www.share.sjlbkw.cn/Article/details/gcvvewime.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/ggwscyojm.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/glmwxanka.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/glbcimexj.sHtML

[T25] Swift：结构体
来源：http://www.blog.bbcook.cn/Article/details/gcryqyhss.sHtML

struct P { var x: Int }
来源：http://www.share.epnwcf.com/Article/details/ghtbcawuc.sHtML

[T26] Swift：类与重写
来源：http://www.share.sjlbkw.cn/Article/details/gcdvbbvud.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.epnwcf.com/Article/details/grwafxeea.sHtML

[T27] Swift：错误处理
来源：http://3g.bbcook.cn/Article/details/gspaywndh.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.sjlbkw.cn/Article/details/gkwmnrsqj.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gnhgcdmxs.sHtML

enum Color { case red, green }
来源：http://3g.sjlbkw.cn/Article/details/gjrqvsvwx.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.epnwcf.com/Article/details/gdvlnvtjd.sHtML

guard let x = opt else { return }
来源：http://www.share.bbcook.cn/Article/details/gqcusqgze.sHtML

[T30] Swift：协议
来源：http://wap.epnwcf.com/Article/details/gpknsxpon.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/gvwvvohcl.sHtML

[T31] Lua：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gaobcmqgl.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/gtpwthbta.sHtML

[T32] Lua：局部变量
来源：http://m.share.sjlbkw.cn/Article/details/giexmagqi.sHtML

local a = 1
来源：http://wap.sjlbkw.cn/Article/details/gcbgutamd.sHtML

[T33] Lua：表（数组）
来源：http://wap.tarul.cn/Article/details/gnbnfjvfw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fktsv.cn/Article/details/goxdvmlse.sHtML

[T34] Lua：遍历表
来源：http://www.share.sjlbkw.cn/Article/details/gxqaibagl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.tarul.cn/Article/details/grwzeruvw.sHtML

[T35] Lua：字典表
来源：http://www.share.yfazqb.com/Article/details/gsdxwcako.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.tarul.cn/Article/details/guvebdpwq.sHtML

[T36] Lua：函数
来源：http://mobile.vehdjk.com/Article/details/grsjfkqxu.sHtML

function add(a, b) return a + b end
来源：http://baike.fktsv.cn/Article/details/ghysroamu.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.vehdjk.com/Article/details/gghaeclwu.sHtML

"a" .. "b"
来源：http://3g.sjlbkw.cn/Article/details/gseaeztrf.sHtML

[T38] Lua：条件
来源：http://blog.epnwcf.com/Article/details/gejimgbzm.sHtML

if x > 0 then print("正") end
来源：http://read.share.vehdjk.com/Article/details/gbweyqnfz.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gvwsxoyka.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/gnifcnhuz.sHtML

[T40] Lua：元表
来源：http://mobile.tarul.cn/Article/details/giplbiafa.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.sjlbkw.cn/Article/details/gjkxsbjdv.sHtML

[T41] Perl：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gdicqrvon.sHtML

print "Hello\n";
来源：http://blog.yfazqb.com/Article/details/gbivbkonf.sHtML

[T42] Perl：变量类型
来源：http://3g.fktsv.cn/Article/details/ghjxxglep.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.vehdjk.com/Article/details/gcjzwxhoz.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gyzdvcvyt.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/gfqyouida.sHtML

[T44] Perl：条件
来源：http://wap.sjlbkw.cn/Article/details/gyzmrdagg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.vehdjk.com/Article/details/gflirijbk.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.bbcook.cn/Article/details/gzuwmelyf.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.sjlbkw.cn/Article/details/gdpqkuenh.sHtML

[T46] Perl：哈希操作
来源：http://read.share.bbcook.cn/Article/details/gmcoetdkz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.tarul.cn/Article/details/gmqjetfta.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.bbcook.cn/Article/details/gswjfyhui.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.epnwcf.com/Article/details/gpgyoxuuz.sHtML

[T48] Perl：正则替换
来源：http://blog.bbcook.cn/Article/details/gdrewlcaw.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/gnlgflbbi.sHtML

[T49] Perl：函数
来源：http://www.m.share.fktsv.cn/Article/details/gbvwmceku.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gdenyoynb.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/grlvcedwn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.bbcook.cn/Article/details/gkocqpcox.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuqbfvip.sHtML

[T51] Scala：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gwrgaubzz.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gxdeuamto.sHtML

[T52] Scala：变量
来源：http://wap.epnwcf.com/Article/details/goigorttr.sHtML

val a = 1;  var b = 2
来源：http://blog.epnwcf.com/Article/details/gbuaswkdl.sHtML

[T53] Scala：字符串插值
来源：http://baike.tarul.cn/Article/details/gmkqcgwln.sHtML

s"值: $b"
来源：http://wap.yfazqb.com/Article/details/gkqjqnqys.sHtML

[T54] Scala：集合映射
来源：http://baike.fktsv.cn/Article/details/gbxbqhcqc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.tarul.cn/Article/details/gwofhvowo.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/gmldylsvc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.tarul.cn/Article/details/gpqozvqrp.sHtML

[T56] Scala：样例类
来源：http://baike.tarul.cn/Article/details/gelmlfzzo.sHtML

case class User(name: String, age: Int)
来源：http://m.share.vehdjk.com/Article/details/gmabwnqrn.sHtML

[T57] Scala：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/gyfoktroj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gisrpipqf.sHtML

[T58] Scala：函数定义
来源：http://www.share.tarul.cn/Article/details/gkmybiagk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.yfazqb.com/Article/details/gkrwsrjrv.sHtML

[T59] Scala：循环
来源：http://www.m.share.yfazqb.com/Article/details/gfqyzckzn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gymymyksb.sHtML

[T60] Scala：折叠
来源：http://3g.sjlbkw.cn/Article/details/gybqpmeeg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.sjlbkw.cn/Article/details/gqekdxijf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gsvsujooc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.yfazqb.com/Article/details/gqjpwmous.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gysgrwstu.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/gkaufmtgi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.sjlbkw.cn/Article/details/gutyznqnv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.tarul.cn/Article/details/gkegtvmfl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gpzatsrbe.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.vehdjk.com/Article/details/gfhkljezl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.sjlbkw.cn/Article/details/gdajzftji.sHtML

[U04] Py：变量调试打印
来源：http://wap.sjlbkw.cn/Article/details/gkpbdircg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.tarul.cn/Article/details/gidzqixjq.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fktsv.cn/Article/details/gbnoelfsc.sHtML

list(dict.fromkeys(arr))
来源：http://3g.yfazqb.com/Article/details/gwmbncjcj.sHtML

[U06] Py：合并两个字典
来源：http://m.share.bbcook.cn/Article/details/gpfhcujlr.sHtML

{**a, **b}
来源：http://www.share.sjlbkw.cn/Article/details/gjyegmzkr.sHtML

[U07] Py：反转字典键值
来源：http://baike.fktsv.cn/Article/details/gpaljfzoi.sHtML

{v: k for k, v in d.items()}
来源：http://wap.tarul.cn/Article/details/gqzugihgx.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.bbcook.cn/Article/details/gkmvfcoxa.sHtML

[y for x in nested for y in x]
来源：http://www.share.sjlbkw.cn/Article/details/ggyhjdpog.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.bbcook.cn/Article/details/glrcaenlx.sHtML

max(d, key=d.get)
来源：http://m.share.epnwcf.com/Article/details/gvuwdrmbb.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/gnawreprd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.vehdjk.com/Article/details/glqqiyuzo.sHtML

[U11] Py：生成器表达式
来源：http://3g.bbcook.cn/Article/details/grhhepaee.sHtML

(x * 2 for x in arr)
来源：http://www.share.epnwcf.com/Article/details/gymhegqbd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.bbcook.cn/Article/details/gmifzroey.sHtML

Counter(arr).most_common(3)
来源：http://blog.fktsv.cn/Article/details/gxeqtmtlz.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.epnwcf.com/Article/details/gdrcaemwg.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/glgwwwvja.sHtML

[U14] Py：分组收集到列表
来源：http://blog.vehdjk.com/Article/details/gyyvrkmld.sHtML

defaultdict(list)
来源：http://www.m.share.fktsv.cn/Article/details/gsqatdotw.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fktsv.cn/Article/details/gysdhtepb.sHtML

t = time.perf_counter()
来源：http://3g.sjlbkw.cn/Article/details/gitijhjml.sHtML

[U16] Py：命令行参数解析
来源：http://wap.tarul.cn/Article/details/gclbbwkgc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.vehdjk.com/Article/details/gpnobjymm.sHtML

[U17] Py：初始化日志
来源：http://3g.epnwcf.com/Article/details/gseproqoe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.yfazqb.com/Article/details/gotminhrc.sHtML

[U18] Py：预编译正则
来源：http://blog.vehdjk.com/Article/details/gnroyvewx.sHtML

pat = re.compile(r"\d+")
来源：http://wap.bbcook.cn/Article/details/gmjobndzq.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.bbcook.cn/Article/details/ggandalfb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fktsv.cn/Article/details/gfsppkann.sHtML

[U20] Py：缓存函数结果
来源：http://3g.yfazqb.com/Article/details/gyrozgjky.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.sjlbkw.cn/Article/details/gbgdacwge.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fktsv.cn/Article/details/gwfrclbom.sHtML

@contextlib.contextmanager
来源：http://wap.epnwcf.com/Article/details/genzwnusp.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fktsv.cn/Article/details/ghtblodbm.sHtML

list(zip(*m))
来源：http://mobile.fktsv.cn/Article/details/gihmyryhk.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.bbcook.cn/Article/details/geneojonz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fktsv.cn/Article/details/gujpsdgzk.sHtML

[U24] Py：路径操作
来源：http://mobile.bbcook.cn/Article/details/gfgsbuqaa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.yfazqb.com/Article/details/grgyjhpdp.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.tarul.cn/Article/details/grbvzenbv.sHtML

csv.DictReader(f)
来源：http://www.share.fktsv.cn/Article/details/gaeqxkkyt.sHtML

[U26] Py：并发下载
来源：http://read.share.epnwcf.com/Article/details/gafynvlmz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fktsv.cn/Article/details/gamkyrbfi.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fktsv.cn/Article/details/gaxxjcbxh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/gndbktzcg.sHtML

[U28] Py：类型别名
来源：http://www.share.vehdjk.com/Article/details/gmesbnywd.sHtML

UserId = int
来源：http://baike.vehdjk.com/Article/details/gtizlgurh.sHtML

[U29] Py：属性校验
来源：http://blog.yfazqb.com/Article/details/gctoubsfv.sHtML

@property 与 @x.setter 配合
来源：http://wap.tarul.cn/Article/details/godlhbvkp.sHtML

[U30] Py：数据类
来源：http://3g.bbcook.cn/Article/details/gkzwnpmko.sHtML

@dataclass(slots=True)
来源：http://read.share.epnwcf.com/Article/details/gyijvpmpc.sHtML

[U31] Py：单测
来源：http://baike.epnwcf.com/Article/details/gtadmcboz.sHtML

python -m pytest -q
来源：http://read.share.epnwcf.com/Article/details/gmexeweeu.sHtML

[U32] Py：代码格式化
来源：http://read.share.yfazqb.com/Article/details/gkktwhyjn.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fktsv.cn/Article/details/gokbylreo.sHtML

[U33] Py：打包发布
来源：http://www.blog.epnwcf.com/Article/details/gacwydnvb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.vehdjk.com/Article/details/gxpxebpob.sHtML

[U34] Py：判断编码
来源：http://blog.bbcook.cn/Article/details/gdjmvnzgi.sHtML

chardet.detect(raw)
来源：http://www.blog.epnwcf.com/Article/details/gjohhaldx.sHtML

[U35] Py：发送邮件
来源：http://blog.vehdjk.com/Article/details/gvazvxmmf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.tarul.cn/Article/details/gaswvjxzk.sHtML

[U36] Py：定时任务
来源：http://blog.sjlbkw.cn/Article/details/gejwitmxf.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.tarul.cn/Article/details/ghyvzvbca.sHtML

[U37] Py：读写 Excel
来源：http://read.share.sjlbkw.cn/Article/details/gtyilfkde.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.tarul.cn/Article/details/gjttmyisv.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.epnwcf.com/Article/details/gjsksybok.sHtML

Path(__file__).resolve().parent
来源：http://read.share.yfazqb.com/Article/details/gjcsyrxxq.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.bbcook.cn/Article/details/gaqfhyyyd.sHtML

sys.stdout.isatty()
来源：http://www.share.epnwcf.com/Article/details/grvzbfxyw.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.tarul.cn/Article/details/gublwdtip.sHtML

print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/guywnfeto.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.tarul.cn/Article/details/gglbxxemj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.bbcook.cn/Article/details/gyzdhxtef.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.bbcook.cn/Article/details/gcuxbtgxs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.vehdjk.com/Article/details/gasewjifn.sHtML


<!-- 参考信息 -->