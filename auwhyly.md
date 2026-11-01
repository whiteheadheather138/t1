代发 wailian999

[S35] C++：map
来源：http://www.m.share.vehdjk.com/Article/details/gqhudxofi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gkkdisdah.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/gwlvczdzr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/ghpzsdvya.sHtML

[S37] C++：set
来源：http://mobile.tarul.cn/Article/details/ggfeqglhc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.yfazqb.com/Article/details/gqxvuaaad.sHtML

[S38] C++：排序
来源：http://www.blog.fktsv.cn/Article/details/grffqvzht.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/guogiovzy.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.yfazqb.com/Article/details/gnwifftey.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.sjlbkw.cn/Article/details/gmsvatwps.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/gypwyqxnr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.bbcook.cn/Article/details/glngzvazv.sHtML

[S41] C++：类与构造函数
来源：http://www.share.tarul.cn/Article/details/gmkuirmlx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/ghzbjfcww.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.epnwcf.com/Article/details/gckpvsccz.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.epnwcf.com/Article/details/gojthmvfy.sHtML

[S43] C++：智能指针
来源：http://www.m.share.yfazqb.com/Article/details/gpblqezui.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/ghpndyxqj.sHtML

[S44] C++：引用传参
来源：http://blog.fktsv.cn/Article/details/grbxzbeql.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.tarul.cn/Article/details/gbbmsgost.sHtML

[S45] C++：lambda
来源：http://www.share.tarul.cn/Article/details/gcosjgcto.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gcefqedat.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/guvxdipje.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.yfazqb.com/Article/details/gbdhntmoh.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.sjlbkw.cn/Article/details/gziymtjfl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.yfazqb.com/Article/details/guktvhtcc.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gsmkzatqs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.sjlbkw.cn/Article/details/gbderaeqs.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/glkxojfoa.sHtML

[S49] C++：写文件
来源：http://wap.fktsv.cn/Article/details/gnvmvkftk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.yfazqb.com/Article/details/gywiiklae.sHtML

[S50] C++：格式化数字
来源：http://mobile.tarul.cn/Article/details/gfcetdwos.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.bbcook.cn/Article/details/gbdjryaif.sHtML

[S51] C++：显式类型转换
来源：http://mobile.tarul.cn/Article/details/gyfjazlwy.sHtML

static_cast<double>(a) / b
来源：http://3g.bbcook.cn/Article/details/gyfkapwjx.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.sjlbkw.cn/Article/details/gzawozixd.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/geijrzgfb.sHtML

[S53] C++：移动语义
来源：http://mobile.vehdjk.com/Article/details/guskkbchj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.epnwcf.com/Article/details/giapvrstj.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/gszmkwljv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.sjlbkw.cn/Article/details/gskoolraa.sHtML

[S55] C++：结构化绑定
来源：http://m.share.vehdjk.com/Article/details/ghzsoptsa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.sjlbkw.cn/Article/details/gvduvkgsy.sHtML

[S56] C++：optional
来源：http://baike.bbcook.cn/Article/details/gabdqoeid.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.sjlbkw.cn/Article/details/gpnpghfuz.sHtML

[S57] C++：编译期常量
来源：http://blog.sjlbkw.cn/Article/details/gcpygfusu.sHtML

constexpr int N = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gvrpqlopo.sHtML

[S58] C++：命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gpsxuvyix.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.tarul.cn/Article/details/gmpdybxtj.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gxbghxvau.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.sjlbkw.cn/Article/details/gxefsuqbi.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/gntwqdckn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fktsv.cn/Article/details/gjdtxfdlw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzszmpmev.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/gbomvplia.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmtpdtrej.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.bbcook.cn/Article/details/gctpywdny.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/ghjikoenw.sHtML

[T02] Kotlin：变量
来源：http://read.share.bbcook.cn/Article/details/gtqokpaot.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.bbcook.cn/Article/details/gdttwqaek.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fktsv.cn/Article/details/gpqdiymdg.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gazoceyvp.sHtML

[T04] Kotlin：空安全
来源：http://blog.sjlbkw.cn/Article/details/gqcidgtby.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.tarul.cn/Article/details/gcnjcwwkc.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fktsv.cn/Article/details/gwbholrlr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.tarul.cn/Article/details/gyfnitpaw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gmlhvhjap.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.tarul.cn/Article/details/ggjyvunsa.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/govoionfi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gpctbpvdz.sHtML

[T08] Kotlin：数据类
来源：http://blog.epnwcf.com/Article/details/guvvihhfg.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.bbcook.cn/Article/details/gmugjjtdp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/gyxhptnxp.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.sjlbkw.cn/Article/details/gxqeylxhj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.yfazqb.com/Article/details/ggopktwps.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.epnwcf.com/Article/details/gzjjcpwxl.sHtML

[T11] Kotlin：协程
来源：http://wap.vehdjk.com/Article/details/ghwrxefir.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.bbcook.cn/Article/details/gddtoxcqu.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.tarul.cn/Article/details/gwetwidwh.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.bbcook.cn/Article/details/giswsfbas.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.sjlbkw.cn/Article/details/gygnuissi.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/gbmapopms.sHtML

[T14] Kotlin：循环
来源：http://wap.yfazqb.com/Article/details/gktkichyc.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gtifygoco.sHtML

[T15] Kotlin：接口
来源：http://wap.epnwcf.com/Article/details/gsjjifzcx.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.bbcook.cn/Article/details/gngmjtnor.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhlhnzja.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gkphgnxrq.sHtML

[T17] Swift：变量与常量
来源：http://read.share.vehdjk.com/Article/details/gnlkfzdsv.sHtML

var a = 1;  let b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gvdpegizf.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/gakyxwlte.sHtML

"值: \(b)"
来源：http://blog.tarul.cn/Article/details/gxphbabag.sHtML

[T19] Swift：可选绑定
来源：http://blog.epnwcf.com/Article/details/grgeyjhap.sHtML

if let n = opt { print(n) }
来源：http://www.share.sjlbkw.cn/Article/details/gurtqoyiu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmyoqwrv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.yfazqb.com/Article/details/gvoncvgsn.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/gbvvbnpef.sHtML

for x in a { print(x) }
来源：http://read.share.vehdjk.com/Article/details/gztohooem.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/ggmuhzhrq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.yfazqb.com/Article/details/gjnrwiaoz.sHtML

[T23] Swift：函数
来源：http://www.share.yfazqb.com/Article/details/gsedxzqhk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.bbcook.cn/Article/details/gzbmqblet.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gtziykefo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gbabdasjq.sHtML

[T25] Swift：结构体
来源：http://read.share.yfazqb.com/Article/details/gvereebhf.sHtML

struct P { var x: Int }
来源：http://www.blog.epnwcf.com/Article/details/ghulpniqd.sHtML

[T26] Swift：类与重写
来源：http://www.blog.yfazqb.com/Article/details/gfpxfxirn.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.epnwcf.com/Article/details/gmtsrogqf.sHtML

[T27] Swift：错误处理
来源：http://read.share.vehdjk.com/Article/details/gfwgkjgli.sHtML

do { try f() } catch { print(error) }
来源：http://3g.sjlbkw.cn/Article/details/grdlpgupa.sHtML

[T28] Swift：枚举
来源：http://baike.sjlbkw.cn/Article/details/gurldeymh.sHtML

enum Color { case red, green }
来源：http://www.share.fktsv.cn/Article/details/gngcpfsbx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/gdkjrreal.sHtML

guard let x = opt else { return }
来源：http://www.m.share.epnwcf.com/Article/details/gllxegfxk.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/gaunlylgg.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.epnwcf.com/Article/details/grhwzqkbh.sHtML

[T31] Lua：Hello World
来源：http://wap.epnwcf.com/Article/details/ggipkghwn.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/grtoifuud.sHtML

[T32] Lua：局部变量
来源：http://mobile.vehdjk.com/Article/details/gicubstqh.sHtML

local a = 1
来源：http://read.share.tarul.cn/Article/details/gklirnhxr.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.epnwcf.com/Article/details/gxpnpvqok.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.vehdjk.com/Article/details/gdvegvmhn.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/gejwoceyu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.epnwcf.com/Article/details/gmqonuffz.sHtML

[T35] Lua：字典表
来源：http://mobile.yfazqb.com/Article/details/gfrmfxqty.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.yfazqb.com/Article/details/gdevqyeif.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/gbrwrwgay.sHtML

function add(a, b) return a + b end
来源：http://3g.yfazqb.com/Article/details/gnafuadxc.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gwvjwkaij.sHtML

"a" .. "b"
来源：http://www.share.tarul.cn/Article/details/glxodngzs.sHtML

[T38] Lua：条件
来源：http://www.blog.tarul.cn/Article/details/gfqhfsqic.sHtML

if x > 0 then print("正") end
来源：http://www.share.tarul.cn/Article/details/ghrbrmjcy.sHtML

[T39] Lua：模式匹配
来源：http://baike.tarul.cn/Article/details/ghpraunix.sHtML

string.find(s, "%d+")
来源：http://www.m.share.tarul.cn/Article/details/gbnmzaefw.sHtML

[T40] Lua：元表
来源：http://3g.vehdjk.com/Article/details/ghqnkphxo.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fktsv.cn/Article/details/gvgoufkgg.sHtML

[T41] Perl：Hello World
来源：http://baike.fktsv.cn/Article/details/gubfihsaa.sHtML

print "Hello\n";
来源：http://mobile.bbcook.cn/Article/details/gnatnxkhw.sHtML

[T42] Perl：变量类型
来源：http://read.share.epnwcf.com/Article/details/gyzwerard.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fktsv.cn/Article/details/gxqvhomdy.sHtML

[T43] Perl：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gcgwsxbrp.sHtML

"值: $a"
来源：http://wap.epnwcf.com/Article/details/gfcbtzsyv.sHtML

[T44] Perl：条件
来源：http://m.share.bbcook.cn/Article/details/gsaxgesze.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.yfazqb.com/Article/details/gviputjvq.sHtML

[T45] Perl：数组遍历
来源：http://3g.tarul.cn/Article/details/gqfxxxsev.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.epnwcf.com/Article/details/gydvflsdi.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.vehdjk.com/Article/details/gkzwymhwm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.epnwcf.com/Article/details/gvhutbazf.sHtML

[T47] Perl：正则捕获
来源：http://3g.epnwcf.com/Article/details/gslnltrvv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.sjlbkw.cn/Article/details/grwydfdiu.sHtML

[T48] Perl：正则替换
来源：http://wap.vehdjk.com/Article/details/gxtnlqjcx.sHtML

$s =~ s/old/new/g;
来源：http://read.share.bbcook.cn/Article/details/gyagsvtiq.sHtML

[T49] Perl：函数
来源：http://baike.tarul.cn/Article/details/gccfkicrz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gbpbfzedz.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/ghqntxyat.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.epnwcf.com/Article/details/gfzzisffx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.bbcook.cn/Article/details/gpupnllfe.sHtML

[T51] Scala：Hello World
来源：http://3g.epnwcf.com/Article/details/gxognnbes.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/ghavffwqj.sHtML

[T52] Scala：变量
来源：http://baike.vehdjk.com/Article/details/gignpnlrf.sHtML

val a = 1;  var b = 2
来源：http://m.share.sjlbkw.cn/Article/details/gdaopmlgw.sHtML

[T53] Scala：字符串插值
来源：http://baike.tarul.cn/Article/details/ggzohzbhz.sHtML

s"值: $b"
来源：http://baike.tarul.cn/Article/details/gjxgiduex.sHtML

[T54] Scala：集合映射
来源：http://www.share.epnwcf.com/Article/details/gvlohmekf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.epnwcf.com/Article/details/gnxlckquz.sHtML

[T55] Scala：集合过滤
来源：http://3g.vehdjk.com/Article/details/ghbzafphb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.bbcook.cn/Article/details/gngygrkxl.sHtML

[T56] Scala：样例类
来源：http://www.blog.sjlbkw.cn/Article/details/gpqlosyqz.sHtML

case class User(name: String, age: Int)
来源：http://www.share.bbcook.cn/Article/details/gyhigfftp.sHtML

[T57] Scala：模式匹配
来源：http://wap.vehdjk.com/Article/details/grusiwqcs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gfxebeoqy.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxyfbvew.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fktsv.cn/Article/details/gtgeekpvf.sHtML

[T59] Scala：循环
来源：http://blog.epnwcf.com/Article/details/gtsuezvkn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gnkxrbuks.sHtML

[T60] Scala：折叠
来源：http://mobile.vehdjk.com/Article/details/gnusgwgti.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.vehdjk.com/Article/details/gsgypcjgl.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gvlpgulbk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.bbcook.cn/Article/details/gwifrplvq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqcslwkes.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fktsv.cn/Article/details/gtjcnkdie.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/gswjrfdzo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.yfazqb.com/Article/details/gtetmzujd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.tarul.cn/Article/details/gtbfzhwfl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.bbcook.cn/Article/details/godlncwfu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fktsv.cn/Article/details/gkwlrbrvk.sHtML

[U04] Py：变量调试打印
来源：http://baike.vehdjk.com/Article/details/gbkhnmftk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.yfazqb.com/Article/details/gxkpniaxf.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.sjlbkw.cn/Article/details/glnucardz.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gdfbikagp.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fktsv.cn/Article/details/ggduqunqc.sHtML

{**a, **b}
来源：http://read.share.sjlbkw.cn/Article/details/ggbnplrqe.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.epnwcf.com/Article/details/gvefbjumv.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gviugjhhq.sHtML

[U08] Py：展平二维列表
来源：http://wap.epnwcf.com/Article/details/gcwlswszk.sHtML

[y for x in nested for y in x]
来源：http://m.share.sjlbkw.cn/Article/details/gwboozccj.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.tarul.cn/Article/details/grvvalgtz.sHtML

max(d, key=d.get)
来源：http://blog.bbcook.cn/Article/details/gzblxirvo.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.epnwcf.com/Article/details/gdpucjhdt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.epnwcf.com/Article/details/gkjzffxuq.sHtML

[U11] Py：生成器表达式
来源：http://mobile.epnwcf.com/Article/details/goyedkgvj.sHtML

(x * 2 for x in arr)
来源：http://www.blog.epnwcf.com/Article/details/gqqxzneoz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.yfazqb.com/Article/details/gywhfubwx.sHtML

Counter(arr).most_common(3)
来源：http://wap.vehdjk.com/Article/details/gulxstsdf.sHtML

[U13] Py：固定长度队列
来源：http://wap.tarul.cn/Article/details/ghnjwuzwi.sHtML

deque(maxlen=10)
来源：http://www.m.share.vehdjk.com/Article/details/gmegnmdzg.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.bbcook.cn/Article/details/gaixazerg.sHtML

defaultdict(list)
来源：http://wap.epnwcf.com/Article/details/gceldtuhs.sHtML

[U15] Py：高精度计时
来源：http://www.blog.tarul.cn/Article/details/gdpqlfhff.sHtML

t = time.perf_counter()
来源：http://3g.bbcook.cn/Article/details/goldqwvyg.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.epnwcf.com/Article/details/gmzdwflkt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.vehdjk.com/Article/details/gzxuxvtne.sHtML

[U17] Py：初始化日志
来源：http://read.share.sjlbkw.cn/Article/details/gsnncjwnk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.vehdjk.com/Article/details/gztbvmbeb.sHtML

[U18] Py：预编译正则
来源：http://wap.vehdjk.com/Article/details/godehwfzm.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/gykffixum.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.vehdjk.com/Article/details/gnxmzcwwv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fktsv.cn/Article/details/gsqbzzgee.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.yfazqb.com/Article/details/gggeyirey.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.yfazqb.com/Article/details/goweqxjwx.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.epnwcf.com/Article/details/gpdmbmkna.sHtML

@contextlib.contextmanager
来源：http://blog.yfazqb.com/Article/details/gbfjcdyjf.sHtML

[U22] Py：矩阵转置
来源：http://blog.vehdjk.com/Article/details/gxusgfxzt.sHtML

list(zip(*m))
来源：http://blog.sjlbkw.cn/Article/details/glwillxwg.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.vehdjk.com/Article/details/gnlmfwxvf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.vehdjk.com/Article/details/gzdcuzvaq.sHtML

[U24] Py：路径操作
来源：http://www.share.sjlbkw.cn/Article/details/gaiolqgnw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/ggdscqbpv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.epnwcf.com/Article/details/giqgbawwb.sHtML

csv.DictReader(f)
来源：http://www.share.vehdjk.com/Article/details/gejqavtzc.sHtML

[U26] Py：并发下载
来源：http://baike.yfazqb.com/Article/details/gzbiuclif.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fktsv.cn/Article/details/gkqujtkep.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.epnwcf.com/Article/details/gevltadde.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.epnwcf.com/Article/details/gbeqhqxqs.sHtML

[U28] Py：类型别名
来源：http://read.share.tarul.cn/Article/details/gvzvkdkir.sHtML

UserId = int
来源：http://mobile.sjlbkw.cn/Article/details/gjvvdgsfe.sHtML

[U29] Py：属性校验
来源：http://mobile.sjlbkw.cn/Article/details/gymauvhag.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fktsv.cn/Article/details/giczsfxxr.sHtML

[U30] Py：数据类
来源：http://blog.yfazqb.com/Article/details/gtlxmzhre.sHtML

@dataclass(slots=True)
来源：http://blog.bbcook.cn/Article/details/gxfaqwnmy.sHtML

[U31] Py：单测
来源：http://blog.bbcook.cn/Article/details/gsgwnojeh.sHtML

python -m pytest -q
来源：http://www.m.share.sjlbkw.cn/Article/details/gtiygyhhh.sHtML

[U32] Py：代码格式化
来源：http://blog.fktsv.cn/Article/details/gjfjnspvp.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.sjlbkw.cn/Article/details/gpzdcvoxa.sHtML

[U33] Py：打包发布
来源：http://3g.vehdjk.com/Article/details/ghkbqqluk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.bbcook.cn/Article/details/gwcxjwecr.sHtML

[U34] Py：判断编码
来源：http://read.share.fktsv.cn/Article/details/gdejhtypb.sHtML

chardet.detect(raw)
来源：http://baike.sjlbkw.cn/Article/details/gajoevrgi.sHtML

[U35] Py：发送邮件
来源：http://read.share.vehdjk.com/Article/details/gndfxtymt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.tarul.cn/Article/details/gdgquqxeu.sHtML

[U36] Py：定时任务
来源：http://www.m.share.tarul.cn/Article/details/guhpnhwjj.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fktsv.cn/Article/details/givsxpuzh.sHtML

[U37] Py：读写 Excel
来源：http://3g.yfazqb.com/Article/details/gwhqgfaep.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.sjlbkw.cn/Article/details/gseyqrqvf.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fktsv.cn/Article/details/gnwmtxbpw.sHtML

Path(__file__).resolve().parent
来源：http://3g.tarul.cn/Article/details/giuzqgxmn.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.tarul.cn/Article/details/ggbxpplct.sHtML

sys.stdout.isatty()
来源：http://mobile.epnwcf.com/Article/details/gpqeemkgm.sHtML

[U40] Py：打印到标准错误
来源：http://blog.bbcook.cn/Article/details/gcomctkfj.sHtML

print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gciyzprbz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.epnwcf.com/Article/details/gmplehvqk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fktsv.cn/Article/details/gpdsxttbb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.sjlbkw.cn/Article/details/gurfguesp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.epnwcf.com/Article/details/gqyglmfbi.sHtML

[U43] PHP：声明命名空间
来源：http://3g.epnwcf.com/Article/details/gqfuyvsqd.sHtML

namespace App\Http;
来源：http://read.share.fktsv.cn/Article/details/gpvgfjrus.sHtML

[U44] PHP：开启严格类型
来源：http://blog.tarul.cn/Article/details/giroxeefy.sHtML

declare(strict_types=1);
来源：http://www.share.yfazqb.com/Article/details/gdwpqsksf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.tarul.cn/Article/details/gkcryqkce.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gythooijd.sHtML

[U46] PHP：可空类型
来源：http://mobile.yfazqb.com/Article/details/gdmnitolg.sHtML

?string $name = null
来源：http://m.share.yfazqb.com/Article/details/gfzkitzkf.sHtML

[U47] PHP：联合类型
来源：http://read.share.yfazqb.com/Article/details/gtwsckfaw.sHtML

int|string $id
来源：http://3g.sjlbkw.cn/Article/details/gnhwhnmui.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.vehdjk.com/Article/details/gtswakfnc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.sjlbkw.cn/Article/details/gwfawzokh.sHtML

[U49] PHP：只读属性
来源：http://m.share.sjlbkw.cn/Article/details/gtaxoqnja.sHtML

public readonly string $name
来源：http://mobile.tarul.cn/Article/details/ggwujnvbc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.epnwcf.com/Article/details/gvxuzwfbx.sHtML

public function __construct(private int $id) {}
来源：http://read.share.tarul.cn/Article/details/gzozeiwtk.sHtML

[U51] PHP：数组解构
来源：http://m.share.bbcook.cn/Article/details/gdscgxiuj.sHtML

[$a, $b] = $arr;
来源：http://wap.tarul.cn/Article/details/gjubfvdmj.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/guhpjvmpy.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fktsv.cn/Article/details/gbxmzaxaz.sHtML

[U53] PHP：空合并运算符
来源：http://3g.epnwcf.com/Article/details/gisyxhqio.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.yfazqb.com/Article/details/ggosnlvdj.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fktsv.cn/Article/details/gbxsaojxt.sHtML

$obj?->method()
来源：http://baike.epnwcf.com/Article/details/gveymkjpv.sHtML

[U55] PHP：match 表达式
来源：http://3g.epnwcf.com/Article/details/gfsuqbdhz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/gicleilzw.sHtML

[U56] PHP：命名参数
来源：http://read.share.epnwcf.com/Article/details/gztqbhodv.sHtML

f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gdnmcupen.sHtML

[U57] PHP：字符串插值
来源：http://wap.vehdjk.com/Article/details/gypmkamdh.sHtML

"值: {$a}"
来源：http://3g.sjlbkw.cn/Article/details/gacchgnnh.sHtML

[U58] PHP：数组三件套
来源：http://baike.epnwcf.com/Article/details/ggppwkbhp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.sjlbkw.cn/Article/details/gitwaxqvb.sHtML

[U59] PHP：自定义排序
来源：http://baike.sjlbkw.cn/Article/details/gpjbnumeu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.tarul.cn/Article/details/gysqzmmva.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.tarul.cn/Article/details/gkvwcpras.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.tarul.cn/Article/details/geoybytqo.sHtML


<!-- 参考信息 -->