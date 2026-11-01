代发 wailian999

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/gwqyrsauy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.tarul.cn/Article/details/gaajmkofu.sHtML

[S38] C++：排序
来源：http://m.share.sjlbkw.cn/Article/details/gwewmhnjl.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.tarul.cn/Article/details/gsnyxyssc.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.sjlbkw.cn/Article/details/gwalryqic.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.tarul.cn/Article/details/gzhfomurr.sHtML

[S40] C++：查找元素
来源：http://www.m.share.yfazqb.com/Article/details/ghdfmbudr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.sjlbkw.cn/Article/details/gksqqdyyx.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.tarul.cn/Article/details/gfklvtwjb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.epnwcf.com/Article/details/gurlpkxdj.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gofnhrglb.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.bbcook.cn/Article/details/ghhzevrqt.sHtML

[S43] C++：智能指针
来源：http://www.blog.tarul.cn/Article/details/gtotgwgtv.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.tarul.cn/Article/details/grbwylhvf.sHtML

[S44] C++：引用传参
来源：http://wap.epnwcf.com/Article/details/gfwytwmgr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.epnwcf.com/Article/details/ggftmapev.sHtML

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/gitiplgpw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.vehdjk.com/Article/details/goyppulsa.sHtML

[S46] C++：函数模板
来源：http://read.share.yfazqb.com/Article/details/gjjhiiilh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.tarul.cn/Article/details/gkbhxgirz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.epnwcf.com/Article/details/gockabsrt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/gotnqivbn.sHtML

[S48] C++：逐行读文件
来源：http://blog.yfazqb.com/Article/details/ggedsmvfu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.vehdjk.com/Article/details/gmuvzeaor.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fktsv.cn/Article/details/ggrntozco.sHtML

[S49] C++：写文件
来源：http://baike.fktsv.cn/Article/details/gohxdawrb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.yfazqb.com/Article/details/gxalqyckm.sHtML

[S50] C++：格式化数字
来源：http://mobile.sjlbkw.cn/Article/details/gjcmfnmdf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gjthgiewp.sHtML

[S51] C++：显式类型转换
来源：http://mobile.yfazqb.com/Article/details/gipjfuorm.sHtML

static_cast<double>(a) / b
来源：http://mobile.yfazqb.com/Article/details/gyxrmwpur.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.vehdjk.com/Article/details/gguyncokf.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.bbcook.cn/Article/details/gtwtvxlvp.sHtML

[S53] C++：移动语义
来源：http://mobile.vehdjk.com/Article/details/gdlcwpnkm.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.yfazqb.com/Article/details/ghlktysjs.sHtML

[S54] C++：异常处理
来源：http://www.blog.fktsv.cn/Article/details/goyhvezer.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.epnwcf.com/Article/details/gkbydldqq.sHtML

[S55] C++：结构化绑定
来源：http://wap.fktsv.cn/Article/details/gjdcxvbyk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.epnwcf.com/Article/details/gyiqinrfs.sHtML

[S56] C++：optional
来源：http://www.blog.sjlbkw.cn/Article/details/gvnjlodze.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.sjlbkw.cn/Article/details/gmbltehuw.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/getkpoyqn.sHtML

constexpr int N = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gfpkihpcr.sHtML

[S58] C++：命名空间
来源：http://www.blog.yfazqb.com/Article/details/gwtunfrad.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.yfazqb.com/Article/details/gfaufyvuw.sHtML

[S59] C++：静态断言
来源：http://blog.epnwcf.com/Article/details/gkalfeqcu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/gcdgufedc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.vehdjk.com/Article/details/gdkexujrf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gmkjbmuim.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gzmdxgnhq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/ggtekziin.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grqcvnkom.sHtML

[T01] Kotlin：Hello World
来源：http://3g.epnwcf.com/Article/details/gwinendxr.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/gblxegjjs.sHtML

[T02] Kotlin：变量
来源：http://3g.bbcook.cn/Article/details/gyhwlkodp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.vehdjk.com/Article/details/gpaqvqbmk.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.sjlbkw.cn/Article/details/gxyfbacuw.sHtML

"值: $b"
来源：http://baike.bbcook.cn/Article/details/glknipeym.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/gzhdjxynb.sHtML

val n: String? = null;  n?.length
来源：http://read.share.bbcook.cn/Article/details/ganjhchia.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.tarul.cn/Article/details/gprwmgffs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.yfazqb.com/Article/details/gobguslqn.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.epnwcf.com/Article/details/ghgjcjavp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.epnwcf.com/Article/details/gkaalktxj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.tarul.cn/Article/details/gnnelnmxs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.yfazqb.com/Article/details/gpgrjhyzp.sHtML

[T08] Kotlin：数据类
来源：http://mobile.epnwcf.com/Article/details/gfbifkpln.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.bbcook.cn/Article/details/gonbvtuiw.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.bbcook.cn/Article/details/gcprvyvcx.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.yfazqb.com/Article/details/gofvpreiz.sHtML

[T10] Kotlin：默认参数
来源：http://baike.tarul.cn/Article/details/gcpjhgvws.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.vehdjk.com/Article/details/gsggxxnsm.sHtML

[T11] Kotlin：协程
来源：http://mobile.bbcook.cn/Article/details/ghhiyfagg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.vehdjk.com/Article/details/gnxmjjzun.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.tarul.cn/Article/details/ghkrzapjz.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/gbgfdzseh.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.epnwcf.com/Article/details/gliatbrej.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fktsv.cn/Article/details/gedfcihgz.sHtML

[T14] Kotlin：循环
来源：http://baike.sjlbkw.cn/Article/details/gldnpdvxb.sHtML

for (i in 1..10) println(i)
来源：http://read.share.vehdjk.com/Article/details/goxbxudqt.sHtML

[T15] Kotlin：接口
来源：http://3g.vehdjk.com/Article/details/gfiqhyrxi.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fktsv.cn/Article/details/gsmwdydjv.sHtML

[T16] Swift：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gtrgdkmiw.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/grlxqprbe.sHtML

[T17] Swift：变量与常量
来源：http://mobile.vehdjk.com/Article/details/gjqtygrmm.sHtML

var a = 1;  let b = 2
来源：http://baike.yfazqb.com/Article/details/giccxwdzk.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/geaoofwax.sHtML

"值: \(b)"
来源：http://www.blog.bbcook.cn/Article/details/gtwnhhyta.sHtML

[T19] Swift：可选绑定
来源：http://3g.tarul.cn/Article/details/grvsjofjo.sHtML

if let n = opt { print(n) }
来源：http://mobile.sjlbkw.cn/Article/details/gbgwmziin.sHtML

[T20] Swift：数组操作
来源：http://www.share.epnwcf.com/Article/details/gjimimuwq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.epnwcf.com/Article/details/gliiowlye.sHtML

[T21] Swift：遍历
来源：http://www.blog.epnwcf.com/Article/details/grlngygta.sHtML

for x in a { print(x) }
来源：http://www.m.share.yfazqb.com/Article/details/gyzglkcid.sHtML

[T22] Swift：字典
来源：http://wap.bbcook.cn/Article/details/glibqngrk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/glwhwxaep.sHtML

[T23] Swift：函数
来源：http://baike.fktsv.cn/Article/details/gtgiykgxg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.sjlbkw.cn/Article/details/goalogjth.sHtML

[T24] Swift：闭包
来源：http://mobile.yfazqb.com/Article/details/ggtkbboaj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gueqeilhj.sHtML

[T25] Swift：结构体
来源：http://www.m.share.tarul.cn/Article/details/gmwplcyhn.sHtML

struct P { var x: Int }
来源：http://baike.bbcook.cn/Article/details/gzcavygvg.sHtML

[T26] Swift：类与重写
来源：http://m.share.epnwcf.com/Article/details/gzosjeyee.sHtML

class A: Base { override func f() {} }
来源：http://m.share.tarul.cn/Article/details/gipsqclxx.sHtML

[T27] Swift：错误处理
来源：http://3g.bbcook.cn/Article/details/gqokniozp.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.bbcook.cn/Article/details/gldriffvv.sHtML

[T28] Swift：枚举
来源：http://baike.fktsv.cn/Article/details/guqistvbu.sHtML

enum Color { case red, green }
来源：http://3g.epnwcf.com/Article/details/gpodxejkf.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.tarul.cn/Article/details/gnmocunqe.sHtML

guard let x = opt else { return }
来源：http://mobile.epnwcf.com/Article/details/gmvjcbrvx.sHtML

[T30] Swift：协议
来源：http://wap.sjlbkw.cn/Article/details/gfxglftsn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.epnwcf.com/Article/details/gzcsplvvs.sHtML

[T31] Lua：Hello World
来源：http://m.share.tarul.cn/Article/details/gxsuzevlg.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/gggaoisdj.sHtML

[T32] Lua：局部变量
来源：http://blog.fktsv.cn/Article/details/gilbbsgic.sHtML

local a = 1
来源：http://www.m.share.vehdjk.com/Article/details/gzgkazckc.sHtML

[T33] Lua：表（数组）
来源：http://read.share.tarul.cn/Article/details/gsyubwgfk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.tarul.cn/Article/details/gtejumuuv.sHtML

[T34] Lua：遍历表
来源：http://mobile.sjlbkw.cn/Article/details/gjntvxjpc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fktsv.cn/Article/details/ggowqgwkz.sHtML

[T35] Lua：字典表
来源：http://www.blog.tarul.cn/Article/details/gygtccknk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.bbcook.cn/Article/details/gkglzscfb.sHtML

[T36] Lua：函数
来源：http://mobile.vehdjk.com/Article/details/gsldmgmix.sHtML

function add(a, b) return a + b end
来源：http://www.blog.epnwcf.com/Article/details/ggnljsztf.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gyizjbijs.sHtML

"a" .. "b"
来源：http://m.share.epnwcf.com/Article/details/gskfvfuda.sHtML

[T38] Lua：条件
来源：http://m.share.sjlbkw.cn/Article/details/gwxxcsssa.sHtML

if x > 0 then print("正") end
来源：http://m.share.vehdjk.com/Article/details/gjziypmiz.sHtML

[T39] Lua：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gglsyrpvp.sHtML

string.find(s, "%d+")
来源：http://www.m.share.yfazqb.com/Article/details/gmnqucpcu.sHtML

[T40] Lua：元表
来源：http://blog.fktsv.cn/Article/details/gjjmovzgk.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.bbcook.cn/Article/details/gczoublae.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/glbsuqcqo.sHtML

print "Hello\n";
来源：http://www.blog.fktsv.cn/Article/details/gozpuoabw.sHtML

[T42] Perl：变量类型
来源：http://read.share.bbcook.cn/Article/details/gsqoinzcv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.vehdjk.com/Article/details/gsenbhpmp.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gpyiznyus.sHtML

"值: $a"
来源：http://www.blog.epnwcf.com/Article/details/ghuezfode.sHtML

[T44] Perl：条件
来源：http://blog.vehdjk.com/Article/details/ggcdicahv.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.tarul.cn/Article/details/gomquqnww.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.sjlbkw.cn/Article/details/geihjqiam.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.tarul.cn/Article/details/ghqbcissw.sHtML

[T46] Perl：哈希操作
来源：http://wap.tarul.cn/Article/details/gbxejugbh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.vehdjk.com/Article/details/gjqrehtpw.sHtML

[T47] Perl：正则捕获
来源：http://read.share.vehdjk.com/Article/details/gaiigvwuh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.tarul.cn/Article/details/grmjsfngz.sHtML

[T48] Perl：正则替换
来源：http://3g.fktsv.cn/Article/details/ghughvujz.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.yfazqb.com/Article/details/guahvworv.sHtML

[T49] Perl：函数
来源：http://3g.vehdjk.com/Article/details/gwxtfyjgd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/ghvqqwnun.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gqvrytepg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.tarul.cn/Article/details/gpqariuqy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.vehdjk.com/Article/details/ghrkodosh.sHtML

[T51] Scala：Hello World
来源：http://3g.vehdjk.com/Article/details/gzsisrple.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/glszqupzn.sHtML

[T52] Scala：变量
来源：http://www.m.share.tarul.cn/Article/details/guqitxzhb.sHtML

val a = 1;  var b = 2
来源：http://www.blog.vehdjk.com/Article/details/gwkylwshg.sHtML

[T53] Scala：字符串插值
来源：http://3g.epnwcf.com/Article/details/gxufkgbuu.sHtML

s"值: $b"
来源：http://3g.fktsv.cn/Article/details/glwlccnva.sHtML

[T54] Scala：集合映射
来源：http://wap.fktsv.cn/Article/details/ghbtvnvno.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fktsv.cn/Article/details/gvltxelgd.sHtML

[T55] Scala：集合过滤
来源：http://read.share.bbcook.cn/Article/details/ggqfmeddi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fktsv.cn/Article/details/gurzhuoyf.sHtML

[T56] Scala：样例类
来源：http://mobile.sjlbkw.cn/Article/details/gvybqnuod.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/gsiroqyia.sHtML

[T57] Scala：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/gjduvqzlb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.vehdjk.com/Article/details/gyekepyui.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/gjmrxnzmw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fktsv.cn/Article/details/gahbrwqum.sHtML

[T59] Scala：循环
来源：http://baike.yfazqb.com/Article/details/ghmvthoxm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gklcsvnbt.sHtML

[T60] Scala：折叠
来源：http://mobile.vehdjk.com/Article/details/gvsqpwyde.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fktsv.cn/Article/details/glbxlquld.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gevuyiprh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.tarul.cn/Article/details/gzywsrlsk.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gocakhcyj.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.sjlbkw.cn/Article/details/gioblmbpp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.sjlbkw.cn/Article/details/gvnoawbhe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fktsv.cn/Article/details/grgpiqyni.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.bbcook.cn/Article/details/gsiorpxlz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fktsv.cn/Article/details/gvkcqhjnr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fktsv.cn/Article/details/gmaoxykog.sHtML

[U04] Py：变量调试打印
来源：http://wap.bbcook.cn/Article/details/gjjuslqas.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.sjlbkw.cn/Article/details/gfwiqhmqu.sHtML

[U05] Py：列表去重且保序
来源：http://blog.epnwcf.com/Article/details/gbxcowtpp.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/glntmpbni.sHtML

[U06] Py：合并两个字典
来源：http://www.share.yfazqb.com/Article/details/gmdwygjaa.sHtML

{**a, **b}
来源：http://m.share.yfazqb.com/Article/details/gymfqbqlj.sHtML

[U07] Py：反转字典键值
来源：http://baike.bbcook.cn/Article/details/gjxhzyzbb.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.sjlbkw.cn/Article/details/gijpkplni.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.vehdjk.com/Article/details/gxvrohynk.sHtML

[y for x in nested for y in x]
来源：http://www.blog.sjlbkw.cn/Article/details/gxnoaypes.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.sjlbkw.cn/Article/details/gsaprmxmg.sHtML

max(d, key=d.get)
来源：http://3g.epnwcf.com/Article/details/gdvyapepv.sHtML

[U10] Py：按值排序字典
来源：http://m.share.yfazqb.com/Article/details/gmgjhuwnz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fktsv.cn/Article/details/gcpspeqhw.sHtML

[U11] Py：生成器表达式
来源：http://baike.yfazqb.com/Article/details/gpgvcrruj.sHtML

(x * 2 for x in arr)
来源：http://m.share.tarul.cn/Article/details/gtcdpkmhf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.epnwcf.com/Article/details/gzgvowkid.sHtML

Counter(arr).most_common(3)
来源：http://3g.yfazqb.com/Article/details/gpyggmtua.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.vehdjk.com/Article/details/geebilqjk.sHtML

deque(maxlen=10)
来源：http://mobile.yfazqb.com/Article/details/gbowrfyaz.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.vehdjk.com/Article/details/gzrmspowf.sHtML

defaultdict(list)
来源：http://baike.epnwcf.com/Article/details/gwknmiulc.sHtML

[U15] Py：高精度计时
来源：http://www.blog.bbcook.cn/Article/details/gblhmhucm.sHtML

t = time.perf_counter()
来源：http://www.blog.bbcook.cn/Article/details/geshfrjuq.sHtML

[U16] Py：命令行参数解析
来源：http://wap.sjlbkw.cn/Article/details/giykaqmpb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fktsv.cn/Article/details/gkksvugot.sHtML

[U17] Py：初始化日志
来源：http://blog.bbcook.cn/Article/details/gladwhkex.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fktsv.cn/Article/details/gnrqwsctq.sHtML

[U18] Py：预编译正则
来源：http://blog.yfazqb.com/Article/details/ggndcbyhx.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.epnwcf.com/Article/details/gkakppnef.sHtML

[U19] Py：正则替换带回调
来源：http://wap.tarul.cn/Article/details/gwenoxocn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.sjlbkw.cn/Article/details/gktdhztow.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fktsv.cn/Article/details/gizknrlkz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.tarul.cn/Article/details/geetwnxpp.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fktsv.cn/Article/details/gjlkxyoci.sHtML

@contextlib.contextmanager
来源：http://3g.vehdjk.com/Article/details/gcyygrtvy.sHtML

[U22] Py：矩阵转置
来源：http://baike.bbcook.cn/Article/details/gdxktynbb.sHtML

list(zip(*m))
来源：http://www.m.share.tarul.cn/Article/details/gkkmvpjky.sHtML

[U23] Py：分块读取大文件
来源：http://blog.vehdjk.com/Article/details/gemcmaoqr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.yfazqb.com/Article/details/gnnnibjkz.sHtML

[U24] Py：路径操作
来源：http://www.share.epnwcf.com/Article/details/gdkhoeiez.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gccsalfvj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fktsv.cn/Article/details/gfymcwrba.sHtML

csv.DictReader(f)
来源：http://www.blog.yfazqb.com/Article/details/gijkmuyjw.sHtML

[U26] Py：并发下载
来源：http://baike.bbcook.cn/Article/details/gjrojyfdy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fktsv.cn/Article/details/gnpuzvelr.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fktsv.cn/Article/details/gbntwuedk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.vehdjk.com/Article/details/ghhcqekef.sHtML

[U28] Py：类型别名
来源：http://3g.sjlbkw.cn/Article/details/gozvesapb.sHtML

UserId = int
来源：http://wap.bbcook.cn/Article/details/gktsjvfwa.sHtML

[U29] Py：属性校验
来源：http://www.share.fktsv.cn/Article/details/gupdhkjhe.sHtML

@property 与 @x.setter 配合
来源：http://wap.sjlbkw.cn/Article/details/gnduhhvqc.sHtML

[U30] Py：数据类
来源：http://baike.tarul.cn/Article/details/gyxcoaypu.sHtML

@dataclass(slots=True)
来源：http://www.share.bbcook.cn/Article/details/gmtmuluwr.sHtML

[U31] Py：单测
来源：http://www.share.epnwcf.com/Article/details/gyamalkfi.sHtML

python -m pytest -q
来源：http://m.share.epnwcf.com/Article/details/gbwndjzzf.sHtML

[U32] Py：代码格式化
来源：http://wap.vehdjk.com/Article/details/gskqkrehk.sHtML

ruff format . && ruff check --fix .
来源：http://wap.bbcook.cn/Article/details/gyyelzodi.sHtML

[U33] Py：打包发布
来源：http://www.share.fktsv.cn/Article/details/geizztsdi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.epnwcf.com/Article/details/gzpoqxyek.sHtML

[U34] Py：判断编码
来源：http://read.share.yfazqb.com/Article/details/gyatxuiqk.sHtML

chardet.detect(raw)
来源：http://m.share.fktsv.cn/Article/details/ggmykydzs.sHtML

[U35] Py：发送邮件
来源：http://baike.fktsv.cn/Article/details/gvplgtpko.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fktsv.cn/Article/details/gebvftxfe.sHtML

[U36] Py：定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gefhwffen.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.sjlbkw.cn/Article/details/gftryucfg.sHtML

[U37] Py：读写 Excel
来源：http://blog.fktsv.cn/Article/details/gdhcvlhvx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.epnwcf.com/Article/details/gmrbrprrd.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.vehdjk.com/Article/details/gwufsjchx.sHtML

Path(__file__).resolve().parent
来源：http://mobile.yfazqb.com/Article/details/genqpxuzi.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.epnwcf.com/Article/details/glxpmebgq.sHtML

sys.stdout.isatty()
来源：http://wap.fktsv.cn/Article/details/gfshcfcph.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fktsv.cn/Article/details/gggwswbht.sHtML

print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/gwjliglxa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.epnwcf.com/Article/details/gzudvwvpa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.epnwcf.com/Article/details/gpcckrkdg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.sjlbkw.cn/Article/details/gewniplrn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.sjlbkw.cn/Article/details/glntuhzci.sHtML

[U43] PHP：声明命名空间
来源：http://wap.sjlbkw.cn/Article/details/gvptnskpd.sHtML

namespace App\Http;
来源：http://m.share.tarul.cn/Article/details/glmecqemq.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.sjlbkw.cn/Article/details/gabwlqlnq.sHtML

declare(strict_types=1);
来源：http://mobile.epnwcf.com/Article/details/gcwrbqhfc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.sjlbkw.cn/Article/details/goicdjcti.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gnnftvmtt.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fktsv.cn/Article/details/gyyaxfiox.sHtML

?string $name = null
来源：http://baike.epnwcf.com/Article/details/gfywprnaf.sHtML

[U47] PHP：联合类型
来源：http://read.share.bbcook.cn/Article/details/gfwodxagm.sHtML

int|string $id
来源：http://www.m.share.fktsv.cn/Article/details/gyqfgbrzx.sHtML

[U48] PHP：纯枚举
来源：http://read.share.vehdjk.com/Article/details/ggizmuiwz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.sjlbkw.cn/Article/details/gomnfohfd.sHtML

[U49] PHP：只读属性
来源：http://m.share.yfazqb.com/Article/details/ggiedezsu.sHtML

public readonly string $name
来源：http://www.blog.tarul.cn/Article/details/gdzwernig.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.epnwcf.com/Article/details/gxczqirdv.sHtML

public function __construct(private int $id) {}
来源：http://read.share.bbcook.cn/Article/details/gregmtssv.sHtML

[U51] PHP：数组解构
来源：http://mobile.fktsv.cn/Article/details/ggnsjvspn.sHtML

[$a, $b] = $arr;
来源：http://3g.bbcook.cn/Article/details/gdrwsgwtk.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.epnwcf.com/Article/details/gfwwdijvs.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fktsv.cn/Article/details/grtgharvw.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.bbcook.cn/Article/details/glwmeyhha.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.bbcook.cn/Article/details/gpiuiqsbh.sHtML

[U54] PHP：空安全调用
来源：http://m.share.bbcook.cn/Article/details/getnuixeu.sHtML

$obj?->method()
来源：http://wap.fktsv.cn/Article/details/gxoakfplc.sHtML

[U55] PHP：match 表达式
来源：http://wap.yfazqb.com/Article/details/gfgqkfdsn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.vehdjk.com/Article/details/gbtwjkrwi.sHtML

[U56] PHP：命名参数
来源：http://www.blog.epnwcf.com/Article/details/gljwbmhwe.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gfpiwkgdo.sHtML

[U57] PHP：字符串插值
来源：http://wap.vehdjk.com/Article/details/gxuthenmg.sHtML

"值: {$a}"
来源：http://baike.epnwcf.com/Article/details/gztfmmtkf.sHtML

[U58] PHP：数组三件套
来源：http://wap.yfazqb.com/Article/details/ghbrdmoea.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.bbcook.cn/Article/details/gljudtfuu.sHtML

[U59] PHP：自定义排序
来源：http://read.share.bbcook.cn/Article/details/gjursswdk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gvqefxooj.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.yfazqb.com/Article/details/gfiznreee.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fktsv.cn/Article/details/gsfcpumqu.sHtML

[U61] PHP：正则
来源：http://www.m.share.bbcook.cn/Article/details/gbyxwdfle.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gmmkbevnd.sHtML

[U62] PHP：日期对象
来源：http://wap.yfazqb.com/Article/details/gfxfyqkgq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.bbcook.cn/Article/details/gkzqxlpch.sHtML


<!-- 参考信息 -->