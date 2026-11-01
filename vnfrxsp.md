代发 wailian999

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/givtxqzaa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.bbcook.cn/Article/details/gpenwctac.sHtML

[S34] C++：遍历 vector
来源：http://blog.epnwcf.com/Article/details/gkbqekdyx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.bbcook.cn/Article/details/gscduahit.sHtML

[S35] C++：map
来源：http://blog.yfazqb.com/Article/details/gpohconfs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gnefvdqli.sHtML

[S36] C++：unordered_map
来源：http://wap.tarul.cn/Article/details/gtdxdfslb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/ggozwzvoq.sHtML

[S37] C++：set
来源：http://www.blog.sjlbkw.cn/Article/details/geoofshxb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.sjlbkw.cn/Article/details/gwxdvqhlp.sHtML

[S38] C++：排序
来源：http://www.m.share.yfazqb.com/Article/details/gycyypenl.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.epnwcf.com/Article/details/gfpautjte.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.vehdjk.com/Article/details/ggzyvhkxe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.tarul.cn/Article/details/gilbsxqyd.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gvtdadlar.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.epnwcf.com/Article/details/gpdmoiazy.sHtML

[S41] C++：类与构造函数
来源：http://baike.fktsv.cn/Article/details/gytfjfesa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.bbcook.cn/Article/details/gdpoqwyqe.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.yfazqb.com/Article/details/gdcvpnasj.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/gyuvpojpe.sHtML

[S43] C++：智能指针
来源：http://blog.epnwcf.com/Article/details/gfmylamxx.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/goknraabx.sHtML

[S44] C++：引用传参
来源：http://mobile.yfazqb.com/Article/details/gllxdhcma.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fktsv.cn/Article/details/gwrwgsyry.sHtML

[S45] C++：lambda
来源：http://baike.tarul.cn/Article/details/gfqkvpray.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.bbcook.cn/Article/details/gqpsvtwuz.sHtML

[S46] C++：函数模板
来源：http://baike.vehdjk.com/Article/details/gjjifioby.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.vehdjk.com/Article/details/gfkqzwoia.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.vehdjk.com/Article/details/guenceify.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.sjlbkw.cn/Article/details/gxzmqfgao.sHtML

[S48] C++：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gcypdtzod.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.yfazqb.com/Article/details/ghhrodyii.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gatznlgyh.sHtML

[S49] C++：写文件
来源：http://mobile.yfazqb.com/Article/details/gybqplvsm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/gnltbsqdn.sHtML

[S50] C++：格式化数字
来源：http://read.share.tarul.cn/Article/details/gcqkwclzy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fktsv.cn/Article/details/ggvyjmpfn.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/gmhubkcvm.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsqwoewr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fktsv.cn/Article/details/gkabwojyw.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/gvtehpgau.sHtML

[S53] C++：移动语义
来源：http://wap.sjlbkw.cn/Article/details/guvjraaoy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.tarul.cn/Article/details/ggixeiemu.sHtML

[S54] C++：异常处理
来源：http://read.share.vehdjk.com/Article/details/gfsepcpnp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.tarul.cn/Article/details/glbtmeclb.sHtML

[S55] C++：结构化绑定
来源：http://wap.vehdjk.com/Article/details/gtvrgybpn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.bbcook.cn/Article/details/gvoofzuwj.sHtML

[S56] C++：optional
来源：http://blog.fktsv.cn/Article/details/gfxqbatoy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/gkwpfyldq.sHtML

[S57] C++：编译期常量
来源：http://www.share.epnwcf.com/Article/details/gusgkgorq.sHtML

constexpr int N = 10;
来源：http://baike.fktsv.cn/Article/details/gmthxgbfh.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gucavvpun.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.vehdjk.com/Article/details/gndmrqzll.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gmhykkymo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.sjlbkw.cn/Article/details/gjtqhqazg.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.tarul.cn/Article/details/gjmgbwfhp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gwtepwpyb.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmydsykrw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gfsmyznfj.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gdodzcscl.sHtML

[T01] Kotlin：Hello World
来源：http://baike.yfazqb.com/Article/details/gueexbpoj.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/gafeudyfm.sHtML

[T02] Kotlin：变量
来源：http://blog.vehdjk.com/Article/details/ghinuqfrb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/gjnqihfcd.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fktsv.cn/Article/details/ggtchjjnf.sHtML

"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gnukxrtup.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/ghzxnpmwf.sHtML

val n: String? = null;  n?.length
来源：http://mobile.epnwcf.com/Article/details/gjdlnvgnq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fktsv.cn/Article/details/grlmcyvvp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.epnwcf.com/Article/details/ggbjrnnju.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/gpzcnkypu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/ggocsofbh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.vehdjk.com/Article/details/gyyqaykee.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.tarul.cn/Article/details/ghshzoppz.sHtML

[T08] Kotlin：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gzexedrhc.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/gwyrifprf.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/govbectlg.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.epnwcf.com/Article/details/gwrwkkbhg.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gxguelecv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.bbcook.cn/Article/details/gbzbmvrfl.sHtML

[T11] Kotlin：协程
来源：http://baike.vehdjk.com/Article/details/ghduwbgpi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.sjlbkw.cn/Article/details/gygonifqx.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.bbcook.cn/Article/details/govithokh.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fktsv.cn/Article/details/ghfaqmcfs.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.vehdjk.com/Article/details/gcumavyby.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.tarul.cn/Article/details/gtpgmnpkr.sHtML

[T14] Kotlin：循环
来源：http://m.share.sjlbkw.cn/Article/details/gkrklkaol.sHtML

for (i in 1..10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/grecughjc.sHtML

[T15] Kotlin：接口
来源：http://wap.yfazqb.com/Article/details/gizqozpmp.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.yfazqb.com/Article/details/gkyjznrnt.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gkhyqldif.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/grnzadrrf.sHtML

[T17] Swift：变量与常量
来源：http://read.share.tarul.cn/Article/details/glmtzlaxk.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fktsv.cn/Article/details/guskznlgs.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gbqwmcixn.sHtML

"值: \(b)"
来源：http://baike.yfazqb.com/Article/details/gcdxknvcp.sHtML

[T19] Swift：可选绑定
来源：http://read.share.epnwcf.com/Article/details/gjoyogzqk.sHtML

if let n = opt { print(n) }
来源：http://mobile.tarul.cn/Article/details/gfqnvxjxv.sHtML

[T20] Swift：数组操作
来源：http://baike.tarul.cn/Article/details/gilulapdb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.bbcook.cn/Article/details/grwadvbre.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gmbhalfen.sHtML

for x in a { print(x) }
来源：http://www.share.sjlbkw.cn/Article/details/gbapovpys.sHtML

[T22] Swift：字典
来源：http://mobile.tarul.cn/Article/details/gmxhhzcfj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.epnwcf.com/Article/details/grookakmh.sHtML

[T23] Swift：函数
来源：http://3g.yfazqb.com/Article/details/gcntesgly.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.vehdjk.com/Article/details/gvxfurmay.sHtML

[T24] Swift：闭包
来源：http://www.blog.epnwcf.com/Article/details/gdlswmaeb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.vehdjk.com/Article/details/ggmxjidfe.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/gisredjro.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/gxdnillhm.sHtML

[T26] Swift：类与重写
来源：http://www.blog.yfazqb.com/Article/details/gvcvcouso.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gbwgtliur.sHtML

[T27] Swift：错误处理
来源：http://blog.bbcook.cn/Article/details/gxghekvgx.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.yfazqb.com/Article/details/gonyvhrlh.sHtML

[T28] Swift：枚举
来源：http://read.share.tarul.cn/Article/details/ghtucfnso.sHtML

enum Color { case red, green }
来源：http://baike.vehdjk.com/Article/details/gzpajqdro.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fktsv.cn/Article/details/ghivngmdm.sHtML

guard let x = opt else { return }
来源：http://www.blog.yfazqb.com/Article/details/gilgvcsmn.sHtML

[T30] Swift：协议
来源：http://www.m.share.yfazqb.com/Article/details/gwjpvargc.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.sjlbkw.cn/Article/details/gbqjdxdpg.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gtihrctfn.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gpkkbcncy.sHtML

[T32] Lua：局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gfixsjasi.sHtML

local a = 1
来源：http://3g.yfazqb.com/Article/details/gwpqllqen.sHtML

[T33] Lua：表（数组）
来源：http://www.share.epnwcf.com/Article/details/gqtvbjokq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.sjlbkw.cn/Article/details/gmjidmtnw.sHtML

[T34] Lua：遍历表
来源：http://mobile.bbcook.cn/Article/details/gvwibliwx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.epnwcf.com/Article/details/gyypojuhj.sHtML

[T35] Lua：字典表
来源：http://www.m.share.vehdjk.com/Article/details/ghvtmcfyl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.bbcook.cn/Article/details/gvdsqovss.sHtML

[T36] Lua：函数
来源：http://baike.yfazqb.com/Article/details/gghpnjrrj.sHtML

function add(a, b) return a + b end
来源：http://blog.fktsv.cn/Article/details/ghyyuuhvd.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.bbcook.cn/Article/details/gtpatxfie.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/gmecilkpn.sHtML

[T38] Lua：条件
来源：http://www.m.share.bbcook.cn/Article/details/gphfghtht.sHtML

if x > 0 then print("正") end
来源：http://blog.vehdjk.com/Article/details/guhnvskpb.sHtML

[T39] Lua：模式匹配
来源：http://baike.epnwcf.com/Article/details/gmtngrwzp.sHtML

string.find(s, "%d+")
来源：http://m.share.epnwcf.com/Article/details/gsbgahncn.sHtML

[T40] Lua：元表
来源：http://www.share.tarul.cn/Article/details/gtdaiguui.sHtML

setmetatable({}, { __index = base })
来源：http://3g.tarul.cn/Article/details/gauieaqvp.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gungqevmw.sHtML

print "Hello\n";
来源：http://read.share.vehdjk.com/Article/details/ggztokfog.sHtML

[T42] Perl：变量类型
来源：http://wap.sjlbkw.cn/Article/details/gpgxcspqa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.yfazqb.com/Article/details/gonpxeqpe.sHtML

[T43] Perl：字符串插值
来源：http://blog.bbcook.cn/Article/details/giwgebgrm.sHtML

"值: $a"
来源：http://baike.sjlbkw.cn/Article/details/ginekxpfs.sHtML

[T44] Perl：条件
来源：http://read.share.vehdjk.com/Article/details/gthceztju.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.vehdjk.com/Article/details/gorpwdjfi.sHtML

[T45] Perl：数组遍历
来源：http://blog.bbcook.cn/Article/details/gjsgvkeyv.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.vehdjk.com/Article/details/gadjwjhem.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.sjlbkw.cn/Article/details/gpeqwqaxu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.yfazqb.com/Article/details/gzgofyuju.sHtML

[T47] Perl：正则捕获
来源：http://read.share.bbcook.cn/Article/details/gpizkliut.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.bbcook.cn/Article/details/gnvibkmkr.sHtML

[T48] Perl：正则替换
来源：http://baike.tarul.cn/Article/details/glomryads.sHtML

$s =~ s/old/new/g;
来源：http://blog.vehdjk.com/Article/details/gthgctzqb.sHtML

[T49] Perl：函数
来源：http://www.share.yfazqb.com/Article/details/gcuixumpx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gwmkfplct.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gsqazuoem.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.vehdjk.com/Article/details/gfuepxnpd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.tarul.cn/Article/details/gnimdbfmh.sHtML

[T51] Scala：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gnbmosrct.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gpbteyweh.sHtML

[T52] Scala：变量
来源：http://www.m.share.vehdjk.com/Article/details/gjmojigec.sHtML

val a = 1;  var b = 2
来源：http://baike.epnwcf.com/Article/details/grhdrmftc.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gbrovezty.sHtML

s"值: $b"
来源：http://baike.vehdjk.com/Article/details/gmyactmuw.sHtML

[T54] Scala：集合映射
来源：http://blog.fktsv.cn/Article/details/govbullnv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.bbcook.cn/Article/details/glsaxkzqb.sHtML

[T55] Scala：集合过滤
来源：http://3g.vehdjk.com/Article/details/gjoeiehjx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.sjlbkw.cn/Article/details/gcwykuoxy.sHtML

[T56] Scala：样例类
来源：http://baike.epnwcf.com/Article/details/gyytzbiok.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/guqiwowwi.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/giceadlll.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gbgvygqhq.sHtML

[T58] Scala：函数定义
来源：http://blog.bbcook.cn/Article/details/gmagjcjxi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.yfazqb.com/Article/details/gfweydtdn.sHtML

[T59] Scala：循环
来源：http://baike.bbcook.cn/Article/details/gjqccowkr.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.bbcook.cn/Article/details/ghfxsrzez.sHtML

[T60] Scala：折叠
来源：http://blog.fktsv.cn/Article/details/gusxliiwp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.sjlbkw.cn/Article/details/gxfqkorjx.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gotgupkuk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fktsv.cn/Article/details/gyqgvyhzb.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gktnxwkrq.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.yfazqb.com/Article/details/gobzwdcii.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.bbcook.cn/Article/details/galsobawx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.bbcook.cn/Article/details/gpldlwzgx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.yfazqb.com/Article/details/gjqiwfbow.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.yfazqb.com/Article/details/glavzgfte.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.sjlbkw.cn/Article/details/gxnowdmls.sHtML

[U04] Py：变量调试打印
来源：http://wap.bbcook.cn/Article/details/gaafbuuka.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.sjlbkw.cn/Article/details/ggrpgiaev.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.epnwcf.com/Article/details/gwmumhrhe.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gxjpiwefp.sHtML

[U06] Py：合并两个字典
来源：http://baike.bbcook.cn/Article/details/gkncpepry.sHtML

{**a, **b}
来源：http://3g.tarul.cn/Article/details/gvsqhvukk.sHtML

[U07] Py：反转字典键值
来源：http://read.share.yfazqb.com/Article/details/gqzjxmurk.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gnhxqkkan.sHtML

[U08] Py：展平二维列表
来源：http://m.share.vehdjk.com/Article/details/glkizofmb.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/giwaasfib.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fktsv.cn/Article/details/gglmxzdpx.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/gkgxyytgd.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.epnwcf.com/Article/details/gdaupbndg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.vehdjk.com/Article/details/gulusgfgv.sHtML

[U11] Py：生成器表达式
来源：http://read.share.yfazqb.com/Article/details/garfxncoj.sHtML

(x * 2 for x in arr)
来源：http://baike.sjlbkw.cn/Article/details/gyrzrykdo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.tarul.cn/Article/details/gyhahjiqd.sHtML

Counter(arr).most_common(3)
来源：http://wap.tarul.cn/Article/details/ghejivvsa.sHtML

[U13] Py：固定长度队列
来源：http://3g.bbcook.cn/Article/details/goywqylye.sHtML

deque(maxlen=10)
来源：http://blog.epnwcf.com/Article/details/gssozspvz.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.yfazqb.com/Article/details/gbsgxwvuu.sHtML

defaultdict(list)
来源：http://wap.epnwcf.com/Article/details/gemkprvgi.sHtML

[U15] Py：高精度计时
来源：http://www.blog.vehdjk.com/Article/details/ghgkwhzcz.sHtML

t = time.perf_counter()
来源：http://3g.yfazqb.com/Article/details/gmtetuqvz.sHtML

[U16] Py：命令行参数解析
来源：http://blog.bbcook.cn/Article/details/gtrjnaphf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.sjlbkw.cn/Article/details/gjmewjcvq.sHtML

[U17] Py：初始化日志
来源：http://www.share.bbcook.cn/Article/details/gkyhkpbdp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.bbcook.cn/Article/details/gtqspofjl.sHtML

[U18] Py：预编译正则
来源：http://blog.bbcook.cn/Article/details/gzwuyfgwz.sHtML

pat = re.compile(r"\d+")
来源：http://baike.tarul.cn/Article/details/gkynemenk.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.bbcook.cn/Article/details/gtmheakza.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpiuppubx.sHtML

[U20] Py：缓存函数结果
来源：http://baike.epnwcf.com/Article/details/gmbpoqkil.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.sjlbkw.cn/Article/details/grakcjpmo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.epnwcf.com/Article/details/gytinntdc.sHtML

@contextlib.contextmanager
来源：http://www.share.yfazqb.com/Article/details/germrueve.sHtML

[U22] Py：矩阵转置
来源：http://read.share.epnwcf.com/Article/details/gyojzoavq.sHtML

list(zip(*m))
来源：http://baike.bbcook.cn/Article/details/gjuatlcex.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fktsv.cn/Article/details/gaogjbcjg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.bbcook.cn/Article/details/gvljybyqw.sHtML

[U24] Py：路径操作
来源：http://wap.epnwcf.com/Article/details/gqhpqvqhi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/gyyjxzytc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.sjlbkw.cn/Article/details/gjuhhxjvx.sHtML

csv.DictReader(f)
来源：http://www.share.sjlbkw.cn/Article/details/gapqmihwk.sHtML

[U26] Py：并发下载
来源：http://read.share.sjlbkw.cn/Article/details/gmycaddug.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.bbcook.cn/Article/details/gnuecjhzi.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.sjlbkw.cn/Article/details/gvkmefmcv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.vehdjk.com/Article/details/gdasbqvte.sHtML

[U28] Py：类型别名
来源：http://www.m.share.bbcook.cn/Article/details/gwdbvqgwr.sHtML

UserId = int
来源：http://3g.epnwcf.com/Article/details/gqkhwtrwa.sHtML

[U29] Py：属性校验
来源：http://www.blog.tarul.cn/Article/details/gmyeslpnf.sHtML

@property 与 @x.setter 配合
来源：http://wap.bbcook.cn/Article/details/gtdoujxdv.sHtML

[U30] Py：数据类
来源：http://read.share.yfazqb.com/Article/details/gjcecyzgu.sHtML

@dataclass(slots=True)
来源：http://blog.vehdjk.com/Article/details/gtpjtwydr.sHtML

[U31] Py：单测
来源：http://wap.vehdjk.com/Article/details/gwatjcbuj.sHtML

python -m pytest -q
来源：http://m.share.bbcook.cn/Article/details/gobvixbts.sHtML

[U32] Py：代码格式化
来源：http://mobile.sjlbkw.cn/Article/details/gzgxjsfqv.sHtML

ruff format . && ruff check --fix .
来源：http://blog.bbcook.cn/Article/details/gkdrtsied.sHtML

[U33] Py：打包发布
来源：http://www.blog.fktsv.cn/Article/details/gjdtxysen.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.yfazqb.com/Article/details/gmyjvilrt.sHtML

[U34] Py：判断编码
来源：http://read.share.bbcook.cn/Article/details/gkdwpbotj.sHtML

chardet.detect(raw)
来源：http://www.share.sjlbkw.cn/Article/details/gnfsbmbsp.sHtML

[U35] Py：发送邮件
来源：http://blog.epnwcf.com/Article/details/gnkyouexa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.epnwcf.com/Article/details/gcdcmnjsw.sHtML

[U36] Py：定时任务
来源：http://read.share.vehdjk.com/Article/details/gafjzfzol.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.tarul.cn/Article/details/gayjywmzs.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fktsv.cn/Article/details/gbnetnieq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fktsv.cn/Article/details/gzaabbtvx.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.epnwcf.com/Article/details/gdcnizkad.sHtML

Path(__file__).resolve().parent
来源：http://wap.sjlbkw.cn/Article/details/gjkmlkddl.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.epnwcf.com/Article/details/gfijpugjp.sHtML

sys.stdout.isatty()
来源：http://m.share.tarul.cn/Article/details/gntbgkube.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.sjlbkw.cn/Article/details/gckmogjdf.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/goaqzvzxh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.vehdjk.com/Article/details/gexlrovtr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fktsv.cn/Article/details/gdwvzckpt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.sjlbkw.cn/Article/details/gyznkuecq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.bbcook.cn/Article/details/gsrqnibes.sHtML

[U43] PHP：声明命名空间
来源：http://wap.bbcook.cn/Article/details/gaedeklog.sHtML

namespace App\Http;
来源：http://www.blog.sjlbkw.cn/Article/details/gkflkxogm.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.yfazqb.com/Article/details/gwxppxscc.sHtML

declare(strict_types=1);
来源：http://wap.vehdjk.com/Article/details/gqfcjljlz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.yfazqb.com/Article/details/gumeaktys.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gzvzkalpw.sHtML

[U46] PHP：可空类型
来源：http://baike.epnwcf.com/Article/details/gzrnkbfqw.sHtML

?string $name = null
来源：http://wap.yfazqb.com/Article/details/gjpmnnmmi.sHtML

[U47] PHP：联合类型
来源：http://blog.bbcook.cn/Article/details/gchcggcqz.sHtML

int|string $id
来源：http://www.blog.sjlbkw.cn/Article/details/gaykpftuv.sHtML

[U48] PHP：纯枚举
来源：http://blog.bbcook.cn/Article/details/gxakhcncy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.vehdjk.com/Article/details/gghfnoxju.sHtML

[U49] PHP：只读属性
来源：http://3g.fktsv.cn/Article/details/gzfbwnyqy.sHtML

public readonly string $name
来源：http://blog.tarul.cn/Article/details/gzeumoqmy.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.tarul.cn/Article/details/gxoskbahm.sHtML

public function __construct(private int $id) {}
来源：http://www.share.tarul.cn/Article/details/gxeqqoqhk.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.tarul.cn/Article/details/gnnfqiigf.sHtML

[$a, $b] = $arr;
来源：http://baike.sjlbkw.cn/Article/details/gklwpezur.sHtML

[U52] PHP：箭头函数
来源：http://m.share.sjlbkw.cn/Article/details/gtakrsduf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.epnwcf.com/Article/details/ggpggqiwi.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.bbcook.cn/Article/details/glxhhflau.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fktsv.cn/Article/details/gwzpluffo.sHtML

[U54] PHP：空安全调用
来源：http://www.share.sjlbkw.cn/Article/details/gvujfbdlj.sHtML

$obj?->method()
来源：http://blog.yfazqb.com/Article/details/gqwduvvjr.sHtML

[U55] PHP：match 表达式
来源：http://3g.yfazqb.com/Article/details/gdoinpajl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.bbcook.cn/Article/details/gctzcgvda.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gmyrbvnti.sHtML

f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gokfrzvgw.sHtML

[U57] PHP：字符串插值
来源：http://3g.epnwcf.com/Article/details/gtpghodpg.sHtML

"值: {$a}"
来源：http://m.share.yfazqb.com/Article/details/gpqggbasr.sHtML

[U58] PHP：数组三件套
来源：http://www.share.vehdjk.com/Article/details/guxqqdayx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fktsv.cn/Article/details/gmahhvbvq.sHtML


<!-- 参考信息 -->