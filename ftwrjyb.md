代发 wailian999

[S33] C++：vector 增删
来源：http://mobile.sjlbkw.cn/Article/details/gckxvrkzp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.yfazqb.com/Article/details/gslokczpa.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gabcknbsm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.tarul.cn/Article/details/gsnmdcwhy.sHtML

[S35] C++：map
来源：http://3g.vehdjk.com/Article/details/gbmypogtb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gnkitwkzw.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/guwzmjsds.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gonuirdke.sHtML

[S37] C++：set
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvtdcmnd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.tarul.cn/Article/details/gobzngfeb.sHtML

[S38] C++：排序
来源：http://3g.yfazqb.com/Article/details/gpucsamqw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/gkenhexkf.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.sjlbkw.cn/Article/details/ghmpwqqga.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.yfazqb.com/Article/details/gixqdukln.sHtML

[S40] C++：查找元素
来源：http://mobile.sjlbkw.cn/Article/details/gjncmtbhj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.vehdjk.com/Article/details/gxvwbajss.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fktsv.cn/Article/details/gaevpssec.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.yfazqb.com/Article/details/gtsnmlkjf.sHtML

[S42] C++：继承与虚函数
来源：http://wap.epnwcf.com/Article/details/gcxuncfku.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/gmeyvyivm.sHtML

[S43] C++：智能指针
来源：http://wap.fktsv.cn/Article/details/gxrsqjcwj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.tarul.cn/Article/details/ghygshqlz.sHtML

[S44] C++：引用传参
来源：http://3g.sjlbkw.cn/Article/details/gsmqnvjoo.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.tarul.cn/Article/details/ghhhjftps.sHtML

[S45] C++：lambda
来源：http://read.share.epnwcf.com/Article/details/gtqntzcuh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.yfazqb.com/Article/details/ghzjhggvc.sHtML

[S46] C++：函数模板
来源：http://read.share.fktsv.cn/Article/details/gwanitbfc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtohviqtg.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.vehdjk.com/Article/details/gwcnrdxcl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.tarul.cn/Article/details/gdvqhvvod.sHtML

[S48] C++：逐行读文件
来源：http://3g.vehdjk.com/Article/details/geqfqxusl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.epnwcf.com/Article/details/grkzhmcmj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.epnwcf.com/Article/details/gxvwoelni.sHtML

[S49] C++：写文件
来源：http://read.share.vehdjk.com/Article/details/gfmkwbptb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.epnwcf.com/Article/details/gqvzwhyah.sHtML

[S50] C++：格式化数字
来源：http://m.share.fktsv.cn/Article/details/gazvghsgr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.bbcook.cn/Article/details/gagrniakl.sHtML

[S51] C++：显式类型转换
来源：http://baike.tarul.cn/Article/details/grtktlgri.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gcxotairk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.bbcook.cn/Article/details/gogtyxnba.sHtML

int size() const noexcept { return n_; }
来源：http://blog.sjlbkw.cn/Article/details/grdqibyep.sHtML

[S53] C++：移动语义
来源：http://blog.yfazqb.com/Article/details/gfqyvgemy.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.epnwcf.com/Article/details/gcpoovrku.sHtML

[S54] C++：异常处理
来源：http://mobile.sjlbkw.cn/Article/details/gbkvextiy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.sjlbkw.cn/Article/details/ghausxzuy.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.epnwcf.com/Article/details/gysdhrjae.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.tarul.cn/Article/details/gekfmxgzq.sHtML

[S56] C++：optional
来源：http://mobile.tarul.cn/Article/details/gsrursgow.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.yfazqb.com/Article/details/giupoianl.sHtML

[S57] C++：编译期常量
来源：http://wap.epnwcf.com/Article/details/grtjvniuz.sHtML

constexpr int N = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gjjdqdavg.sHtML

[S58] C++：命名空间
来源：http://baike.yfazqb.com/Article/details/gjeqnvaxi.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.sjlbkw.cn/Article/details/gkeolkoca.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/gdhpucydo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.tarul.cn/Article/details/giemajdag.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.vehdjk.com/Article/details/ggzdvfzoh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.bbcook.cn/Article/details/guvifulzd.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkbvmocif.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.sjlbkw.cn/Article/details/gyipkxdsy.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpjytehpa.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/gdflvwvsr.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/gofgaubxa.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/goshsmgfc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.epnwcf.com/Article/details/gwpqutwij.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.vehdjk.com/Article/details/gfentrifo.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/galquldnw.sHtML

[T04] Kotlin：空安全
来源：http://3g.bbcook.cn/Article/details/gjwoslnrz.sHtML

val n: String? = null;  n?.length
来源：http://wap.sjlbkw.cn/Article/details/gxoelmbpj.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.vehdjk.com/Article/details/gevudwdim.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gqchsyjfv.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.tarul.cn/Article/details/geulsrsep.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fktsv.cn/Article/details/genjjrpyd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.vehdjk.com/Article/details/gmoegvglv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.tarul.cn/Article/details/gknrzpyam.sHtML

[T08] Kotlin：数据类
来源：http://blog.tarul.cn/Article/details/gndwxgzxh.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.yfazqb.com/Article/details/gxkgmgwlm.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.yfazqb.com/Article/details/gnlirhpjr.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.epnwcf.com/Article/details/glggkopze.sHtML

[T10] Kotlin：默认参数
来源：http://wap.epnwcf.com/Article/details/gqxprwoqa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.sjlbkw.cn/Article/details/gnwhsgmjj.sHtML

[T11] Kotlin：协程
来源：http://read.share.epnwcf.com/Article/details/geevhowxn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fktsv.cn/Article/details/gkkyazxjh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/gmcvmnsco.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/ghxwlgsfi.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.sjlbkw.cn/Article/details/gwqossspr.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gewueinta.sHtML

[T14] Kotlin：循环
来源：http://blog.tarul.cn/Article/details/ggcjdvywb.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/gfqiiyffj.sHtML

[T15] Kotlin：接口
来源：http://baike.sjlbkw.cn/Article/details/gxhfsehfc.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.epnwcf.com/Article/details/gzzasfrvl.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/ghunnzdex.sHtML

print("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gbiiszmqj.sHtML

[T17] Swift：变量与常量
来源：http://wap.tarul.cn/Article/details/grlhafmdx.sHtML

var a = 1;  let b = 2
来源：http://read.share.epnwcf.com/Article/details/goemgmjyq.sHtML

[T18] Swift：字符串插值
来源：http://3g.fktsv.cn/Article/details/gtkuixwmi.sHtML

"值: \(b)"
来源：http://wap.vehdjk.com/Article/details/gptvoawyw.sHtML

[T19] Swift：可选绑定
来源：http://read.share.vehdjk.com/Article/details/gtlfresve.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/ggogzkxhc.sHtML

[T20] Swift：数组操作
来源：http://m.share.bbcook.cn/Article/details/gxlcpaevj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/gtfqwmbge.sHtML

[T21] Swift：遍历
来源：http://wap.bbcook.cn/Article/details/gvvrpcynl.sHtML

for x in a { print(x) }
来源：http://www.m.share.fktsv.cn/Article/details/gevvaknme.sHtML

[T22] Swift：字典
来源：http://www.blog.tarul.cn/Article/details/gqltckdqq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.tarul.cn/Article/details/gdyzdyaet.sHtML

[T23] Swift：函数
来源：http://m.share.fktsv.cn/Article/details/gebdvoryt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/gwhetvqbh.sHtML

[T24] Swift：闭包
来源：http://mobile.sjlbkw.cn/Article/details/glomlbmey.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/ganttscom.sHtML

[T25] Swift：结构体
来源：http://blog.sjlbkw.cn/Article/details/gtxnkrcwg.sHtML

struct P { var x: Int }
来源：http://wap.tarul.cn/Article/details/gznvzfune.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fktsv.cn/Article/details/gfyywldoc.sHtML

class A: Base { override func f() {} }
来源：http://blog.tarul.cn/Article/details/gtjjnbckz.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gdswmwiqf.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.bbcook.cn/Article/details/gadqduquh.sHtML

[T28] Swift：枚举
来源：http://baike.vehdjk.com/Article/details/gqfnedypv.sHtML

enum Color { case red, green }
来源：http://read.share.bbcook.cn/Article/details/gjnrybful.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fktsv.cn/Article/details/gbguresyo.sHtML

guard let x = opt else { return }
来源：http://m.share.epnwcf.com/Article/details/gzgfcnkpb.sHtML

[T30] Swift：协议
来源：http://3g.sjlbkw.cn/Article/details/gnysyoylo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/gzkqmpzop.sHtML

[T31] Lua：Hello World
来源：http://baike.vehdjk.com/Article/details/ghzuhetjc.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gekucbxmx.sHtML

[T32] Lua：局部变量
来源：http://blog.epnwcf.com/Article/details/ggbpnemxq.sHtML

local a = 1
来源：http://mobile.fktsv.cn/Article/details/gklkxixgp.sHtML

[T33] Lua：表（数组）
来源：http://wap.fktsv.cn/Article/details/geiflvezc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.sjlbkw.cn/Article/details/gcioncayb.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/gxonvxbln.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.epnwcf.com/Article/details/ghobjuwki.sHtML

[T35] Lua：字典表
来源：http://mobile.epnwcf.com/Article/details/gzayyrbnh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.yfazqb.com/Article/details/gsubbvcug.sHtML

[T36] Lua：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gqdwoecke.sHtML

function add(a, b) return a + b end
来源：http://3g.sjlbkw.cn/Article/details/gwsjtfhim.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gyhryafjs.sHtML

"a" .. "b"
来源：http://mobile.yfazqb.com/Article/details/ggwmdxzsh.sHtML

[T38] Lua：条件
来源：http://www.m.share.fktsv.cn/Article/details/gpytlowgg.sHtML

if x > 0 then print("正") end
来源：http://read.share.tarul.cn/Article/details/gywjivzbu.sHtML

[T39] Lua：模式匹配
来源：http://baike.bbcook.cn/Article/details/gquldpcba.sHtML

string.find(s, "%d+")
来源：http://www.share.epnwcf.com/Article/details/gtsdrztjm.sHtML

[T40] Lua：元表
来源：http://m.share.bbcook.cn/Article/details/grxazxsbb.sHtML

setmetatable({}, { __index = base })
来源：http://wap.sjlbkw.cn/Article/details/gzzkpdszp.sHtML

[T41] Perl：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gpjqddsbn.sHtML

print "Hello\n";
来源：http://baike.yfazqb.com/Article/details/gzepyneiv.sHtML

[T42] Perl：变量类型
来源：http://baike.yfazqb.com/Article/details/gphlrxuqr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fktsv.cn/Article/details/gyhjzbdoq.sHtML

[T43] Perl：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gytplaild.sHtML

"值: $a"
来源：http://www.share.bbcook.cn/Article/details/giojgtlqv.sHtML

[T44] Perl：条件
来源：http://blog.fktsv.cn/Article/details/gqiwjlcir.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gufqcuurv.sHtML

[T45] Perl：数组遍历
来源：http://m.share.bbcook.cn/Article/details/gkjwccgmq.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.sjlbkw.cn/Article/details/gnntbulzs.sHtML

[T46] Perl：哈希操作
来源：http://read.share.tarul.cn/Article/details/gxzsyowma.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.epnwcf.com/Article/details/giqswhame.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fktsv.cn/Article/details/gfphtjllp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.epnwcf.com/Article/details/glgriehrt.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.vehdjk.com/Article/details/glqwvxujs.sHtML

$s =~ s/old/new/g;
来源：http://mobile.sjlbkw.cn/Article/details/gzivpgoml.sHtML

[T49] Perl：函数
来源：http://read.share.yfazqb.com/Article/details/gqjiyqhqj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gzjgxjkit.sHtML

[T50] Perl：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/giyhmspde.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.tarul.cn/Article/details/geabxcren.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.bbcook.cn/Article/details/gwbrxiblg.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gshljhjsx.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gweimzblo.sHtML

[T52] Scala：变量
来源：http://www.m.share.fktsv.cn/Article/details/gwnwjrywz.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.yfazqb.com/Article/details/ggzrbxlpb.sHtML

[T53] Scala：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gxcgpernd.sHtML

s"值: $b"
来源：http://3g.vehdjk.com/Article/details/gvoqvycre.sHtML

[T54] Scala：集合映射
来源：http://www.share.epnwcf.com/Article/details/gsqksamnr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.vehdjk.com/Article/details/gdakluuir.sHtML

[T55] Scala：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/geabmzjwx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fktsv.cn/Article/details/gvlrqgxii.sHtML

[T56] Scala：样例类
来源：http://www.blog.yfazqb.com/Article/details/ghcymnswy.sHtML

case class User(name: String, age: Int)
来源：http://3g.yfazqb.com/Article/details/gclbemhbr.sHtML

[T57] Scala：模式匹配
来源：http://www.share.vehdjk.com/Article/details/gydrqiseu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.sjlbkw.cn/Article/details/gbxznjhkr.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fktsv.cn/Article/details/gkvwsnljj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.yfazqb.com/Article/details/gmopjczkc.sHtML

[T59] Scala：循环
来源：http://mobile.bbcook.cn/Article/details/ggrziboul.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gwxmfilsg.sHtML

[T60] Scala：折叠
来源：http://wap.bbcook.cn/Article/details/gwcrugpml.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.vehdjk.com/Article/details/gcmqfcdnd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gewucirhu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.yfazqb.com/Article/details/gsmbwwzia.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gyescbeny.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.tarul.cn/Article/details/gledyegmu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.yfazqb.com/Article/details/gblbirdyy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.epnwcf.com/Article/details/gueymayyv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fktsv.cn/Article/details/gbpvhixlw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.vehdjk.com/Article/details/gttoysjzm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.sjlbkw.cn/Article/details/gfeksxjfn.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fktsv.cn/Article/details/gpfggfavx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fktsv.cn/Article/details/gpebhblsl.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fktsv.cn/Article/details/gxoyfdblw.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/gjtubsgze.sHtML

[U06] Py：合并两个字典
来源：http://m.share.vehdjk.com/Article/details/glbhlybjc.sHtML

{**a, **b}
来源：http://3g.yfazqb.com/Article/details/gwzrqcnmc.sHtML

[U07] Py：反转字典键值
来源：http://mobile.bbcook.cn/Article/details/gpeuznncx.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fktsv.cn/Article/details/gxtkejbuh.sHtML

[U08] Py：展平二维列表
来源：http://m.share.tarul.cn/Article/details/ghoeeumyx.sHtML

[y for x in nested for y in x]
来源：http://baike.tarul.cn/Article/details/gauxafgkc.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.tarul.cn/Article/details/gxligkeoq.sHtML

max(d, key=d.get)
来源：http://www.m.share.tarul.cn/Article/details/gwtyeynkg.sHtML

[U10] Py：按值排序字典
来源：http://wap.fktsv.cn/Article/details/gbvkxxmit.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.vehdjk.com/Article/details/gexicrocx.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.bbcook.cn/Article/details/gilksyizi.sHtML

(x * 2 for x in arr)
来源：http://www.blog.bbcook.cn/Article/details/gpjsnsczh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.bbcook.cn/Article/details/gprhdzzlg.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.bbcook.cn/Article/details/gplksxsqy.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.bbcook.cn/Article/details/goaehpsjc.sHtML

deque(maxlen=10)
来源：http://m.share.sjlbkw.cn/Article/details/gmwlysoxx.sHtML

[U14] Py：分组收集到列表
来源：http://baike.yfazqb.com/Article/details/ghhortsus.sHtML

defaultdict(list)
来源：http://www.share.epnwcf.com/Article/details/gnhwqrdbu.sHtML

[U15] Py：高精度计时
来源：http://3g.fktsv.cn/Article/details/gtkletvvs.sHtML

t = time.perf_counter()
来源：http://www.blog.tarul.cn/Article/details/gtymddzvd.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.vehdjk.com/Article/details/gblrcuslz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.vehdjk.com/Article/details/ggruaddiz.sHtML

[U17] Py：初始化日志
来源：http://www.share.sjlbkw.cn/Article/details/gqlxcnhxj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fktsv.cn/Article/details/goyjpertq.sHtML

[U18] Py：预编译正则
来源：http://m.share.yfazqb.com/Article/details/goesvnpsg.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.bbcook.cn/Article/details/gzqvabzcm.sHtML

[U19] Py：正则替换带回调
来源：http://3g.epnwcf.com/Article/details/ghcmbtgmc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.bbcook.cn/Article/details/gdktfpnse.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.vehdjk.com/Article/details/gclsfgaqf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.sjlbkw.cn/Article/details/gkkslyfux.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.bbcook.cn/Article/details/gkyrsgifv.sHtML

@contextlib.contextmanager
来源：http://m.share.sjlbkw.cn/Article/details/gjoaulwet.sHtML

[U22] Py：矩阵转置
来源：http://3g.yfazqb.com/Article/details/gzznamcer.sHtML

list(zip(*m))
来源：http://www.blog.fktsv.cn/Article/details/gnkihamej.sHtML

[U23] Py：分块读取大文件
来源：http://blog.tarul.cn/Article/details/gnuxoqlka.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.epnwcf.com/Article/details/gnspkiilw.sHtML

[U24] Py：路径操作
来源：http://blog.sjlbkw.cn/Article/details/gumqguvmc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/gdceeoxnj.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.vehdjk.com/Article/details/gbmuabwjz.sHtML

csv.DictReader(f)
来源：http://www.share.vehdjk.com/Article/details/gxcdearlf.sHtML

[U26] Py：并发下载
来源：http://mobile.fktsv.cn/Article/details/gilmnmawq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.vehdjk.com/Article/details/gqgoimmxl.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.bbcook.cn/Article/details/gyrymzloe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.bbcook.cn/Article/details/gibyfyfwu.sHtML

[U28] Py：类型别名
来源：http://wap.yfazqb.com/Article/details/gmnrjakuk.sHtML

UserId = int
来源：http://read.share.epnwcf.com/Article/details/grwksbmdo.sHtML

[U29] Py：属性校验
来源：http://m.share.vehdjk.com/Article/details/gmvqxkbgw.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.tarul.cn/Article/details/ghikdeajn.sHtML

[U30] Py：数据类
来源：http://m.share.fktsv.cn/Article/details/gyyllfauu.sHtML

@dataclass(slots=True)
来源：http://3g.vehdjk.com/Article/details/ghuspsxpg.sHtML

[U31] Py：单测
来源：http://www.m.share.fktsv.cn/Article/details/gwirytrds.sHtML

python -m pytest -q
来源：http://www.blog.vehdjk.com/Article/details/gkybnmnvl.sHtML

[U32] Py：代码格式化
来源：http://blog.epnwcf.com/Article/details/giabowsuj.sHtML

ruff format . && ruff check --fix .
来源：http://wap.vehdjk.com/Article/details/gspnkyqgb.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fktsv.cn/Article/details/gojjyirhf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.sjlbkw.cn/Article/details/gpwurdtxs.sHtML

[U34] Py：判断编码
来源：http://mobile.vehdjk.com/Article/details/gkhyhndep.sHtML

chardet.detect(raw)
来源：http://wap.bbcook.cn/Article/details/gwtjjtrks.sHtML

[U35] Py：发送邮件
来源：http://mobile.bbcook.cn/Article/details/grkykcipi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.yfazqb.com/Article/details/gjqhkeikq.sHtML

[U36] Py：定时任务
来源：http://www.blog.fktsv.cn/Article/details/ghmqpbqsf.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.yfazqb.com/Article/details/gkfiivena.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.yfazqb.com/Article/details/gofsthbue.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fktsv.cn/Article/details/ghiprhouv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.epnwcf.com/Article/details/gydoybjgs.sHtML

Path(__file__).resolve().parent
来源：http://read.share.vehdjk.com/Article/details/gsjfytdyk.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.vehdjk.com/Article/details/guuoleece.sHtML

sys.stdout.isatty()
来源：http://m.share.epnwcf.com/Article/details/gethjpzux.sHtML

[U40] Py：打印到标准错误
来源：http://blog.yfazqb.com/Article/details/gdvqnlxwe.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/glxuvylle.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.bbcook.cn/Article/details/gnudvovzq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.vehdjk.com/Article/details/ghzlzzifi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.epnwcf.com/Article/details/gtxxuupyt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.epnwcf.com/Article/details/goqvszbem.sHtML

[U43] PHP：声明命名空间
来源：http://3g.vehdjk.com/Article/details/gaibhmkmc.sHtML

namespace App\Http;
来源：http://wap.vehdjk.com/Article/details/gqaazcavg.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.vehdjk.com/Article/details/gnawktpme.sHtML

declare(strict_types=1);
来源：http://wap.tarul.cn/Article/details/galbkxkhc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.bbcook.cn/Article/details/ggxelysvf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxfstazf.sHtML

[U46] PHP：可空类型
来源：http://baike.yfazqb.com/Article/details/glkzswrbt.sHtML

?string $name = null
来源：http://www.blog.yfazqb.com/Article/details/gwjdkbgud.sHtML

[U47] PHP：联合类型
来源：http://blog.tarul.cn/Article/details/gfyonpkle.sHtML

int|string $id
来源：http://wap.vehdjk.com/Article/details/glkspksul.sHtML

[U48] PHP：纯枚举
来源：http://blog.sjlbkw.cn/Article/details/gkqrokygt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.epnwcf.com/Article/details/grytnebqb.sHtML

[U49] PHP：只读属性
来源：http://read.share.vehdjk.com/Article/details/gevbakxlj.sHtML

public readonly string $name
来源：http://www.m.share.tarul.cn/Article/details/gkwvuucai.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.sjlbkw.cn/Article/details/gqcjfzwwl.sHtML

public function __construct(private int $id) {}
来源：http://3g.tarul.cn/Article/details/gvyaugbuo.sHtML

[U51] PHP：数组解构
来源：http://read.share.tarul.cn/Article/details/ggfkcaicv.sHtML

[$a, $b] = $arr;
来源：http://baike.fktsv.cn/Article/details/gbionjxva.sHtML

[U52] PHP：箭头函数
来源：http://3g.fktsv.cn/Article/details/gehayyumj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.bbcook.cn/Article/details/gmlacaiti.sHtML

[U53] PHP：空合并运算符
来源：http://baike.bbcook.cn/Article/details/gtvuutemp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fktsv.cn/Article/details/gmqtvrzyf.sHtML

[U54] PHP：空安全调用
来源：http://baike.bbcook.cn/Article/details/gdrdhtnbm.sHtML

$obj?->method()
来源：http://www.blog.yfazqb.com/Article/details/gquxmgmzo.sHtML

[U55] PHP：match 表达式
来源：http://read.share.sjlbkw.cn/Article/details/gwnzaejuq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/guscjyhcu.sHtML

[U56] PHP：命名参数
来源：http://baike.sjlbkw.cn/Article/details/gabxgsehn.sHtML

f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gyeyalqxh.sHtML

[U57] PHP：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gsuqfqrtb.sHtML

"值: {$a}"
来源：http://www.blog.epnwcf.com/Article/details/gxycpbdij.sHtML

[U58] PHP：数组三件套
来源：http://blog.bbcook.cn/Article/details/gltsdxbjy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.bbcook.cn/Article/details/ghrcftwxp.sHtML


<!-- 参考信息 -->