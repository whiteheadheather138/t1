代发 wailian999

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/ginuwdryq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gtxghqeox.sHtML

[S34] C++：遍历 vector
来源：http://m.share.tarul.cn/Article/details/grvvhsqhe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.tarul.cn/Article/details/gygrwktqd.sHtML

[S35] C++：map
来源：http://www.m.share.vehdjk.com/Article/details/ggvtkufle.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyegdefc.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gjoyioauu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gponeeyad.sHtML

[S37] C++：set
来源：http://mobile.bbcook.cn/Article/details/gidgmuesc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.tarul.cn/Article/details/ggdhcenys.sHtML

[S38] C++：排序
来源：http://wap.epnwcf.com/Article/details/gzletbkta.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.epnwcf.com/Article/details/gibmtyomw.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/gekanjfhh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.bbcook.cn/Article/details/gofukcznw.sHtML

[S40] C++：查找元素
来源：http://blog.fktsv.cn/Article/details/gbkaasxiv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.sjlbkw.cn/Article/details/grkvduvhr.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/girsflhon.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.tarul.cn/Article/details/gfehqhcld.sHtML

[S42] C++：继承与虚函数
来源：http://blog.epnwcf.com/Article/details/gvkirtaee.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.bbcook.cn/Article/details/ghgozqqtq.sHtML

[S43] C++：智能指针
来源：http://blog.sjlbkw.cn/Article/details/gbbicvwta.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/gvtfjzomi.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gehqnkzxx.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.sjlbkw.cn/Article/details/gsesgdgji.sHtML

[S45] C++：lambda
来源：http://www.blog.yfazqb.com/Article/details/gobjqzbqz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.epnwcf.com/Article/details/golokkgrm.sHtML

[S46] C++：函数模板
来源：http://3g.vehdjk.com/Article/details/ghnligszi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwftebxru.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/gfmpuqdjf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.tarul.cn/Article/details/gwebdnpom.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gujasgpad.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.tarul.cn/Article/details/gzavbmpki.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.tarul.cn/Article/details/gfejoaecu.sHtML

[S49] C++：写文件
来源：http://read.share.tarul.cn/Article/details/gyhvcbitl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/gxscvchiv.sHtML

[S50] C++：格式化数字
来源：http://read.share.fktsv.cn/Article/details/glpypnmnq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fktsv.cn/Article/details/gbfdhumgz.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gwilymbkb.sHtML

static_cast<double>(a) / b
来源：http://m.share.fktsv.cn/Article/details/ggauxjikr.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/getyvkrli.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/ggeqwjjxd.sHtML

[S53] C++：移动语义
来源：http://baike.epnwcf.com/Article/details/gsiudatdt.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.epnwcf.com/Article/details/gtsntmyja.sHtML

[S54] C++：异常处理
来源：http://www.m.share.yfazqb.com/Article/details/gmvrpfvnj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.bbcook.cn/Article/details/gvsroivqa.sHtML

[S55] C++：结构化绑定
来源：http://m.share.yfazqb.com/Article/details/gdlslbekr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/geamnuwdb.sHtML

[S56] C++：optional
来源：http://m.share.bbcook.cn/Article/details/ghmqqxcsq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.vehdjk.com/Article/details/gmmhxdmvh.sHtML

[S57] C++：编译期常量
来源：http://wap.yfazqb.com/Article/details/gjqfhdemt.sHtML

constexpr int N = 10;
来源：http://3g.epnwcf.com/Article/details/gyjkddhsa.sHtML

[S58] C++：命名空间
来源：http://3g.sjlbkw.cn/Article/details/gzsxyrwig.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.yfazqb.com/Article/details/gtrgzxrqn.sHtML

[S59] C++：静态断言
来源：http://blog.vehdjk.com/Article/details/gmrcuimyp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/gcpztnovx.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.bbcook.cn/Article/details/ghougllpt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.vehdjk.com/Article/details/gjwpkfuhb.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbzriqhdr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.sjlbkw.cn/Article/details/gznsvhomu.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtmzophlr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.bbcook.cn/Article/details/gmrknjzso.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/gookfjnhr.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gcguzdkxh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.epnwcf.com/Article/details/ghwoafooh.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gnwkerlqf.sHtML

"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gdbxbqtbq.sHtML

[T04] Kotlin：空安全
来源：http://www.share.bbcook.cn/Article/details/gxmpmrvgv.sHtML

val n: String? = null;  n?.length
来源：http://baike.fktsv.cn/Article/details/gsywgmbgg.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.tarul.cn/Article/details/gbxmuxhxe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/gjlisxpnt.sHtML

[T06] Kotlin：集合映射
来源：http://blog.vehdjk.com/Article/details/goszuoxur.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gebhsnoci.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gizldqdjn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fktsv.cn/Article/details/gqrnlssyb.sHtML

[T08] Kotlin：数据类
来源：http://wap.sjlbkw.cn/Article/details/gigcxjqjr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/growojsqj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.sjlbkw.cn/Article/details/gqhsfophm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.tarul.cn/Article/details/gnkkyxsgf.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.tarul.cn/Article/details/gefjobsns.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fktsv.cn/Article/details/gknesrygu.sHtML

[T11] Kotlin：协程
来源：http://3g.fktsv.cn/Article/details/gwppjpgim.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.yfazqb.com/Article/details/gapzrxkne.sHtML

[T12] Kotlin：解构声明
来源：http://baike.bbcook.cn/Article/details/gqbyoyvur.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.epnwcf.com/Article/details/grzmypwzt.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.epnwcf.com/Article/details/gesehazts.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbmmnbzm.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/ggxuvnkna.sHtML

for (i in 1..10) println(i)
来源：http://m.share.tarul.cn/Article/details/ggvzmglak.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.yfazqb.com/Article/details/gfysiolfe.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.vehdjk.com/Article/details/gwvrgdkkc.sHtML

[T16] Swift：Hello World
来源：http://www.share.tarul.cn/Article/details/gaiqscgap.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gayhvvfew.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.yfazqb.com/Article/details/gmqywxhbb.sHtML

var a = 1;  let b = 2
来源：http://baike.tarul.cn/Article/details/gjlffegml.sHtML

[T18] Swift：字符串插值
来源：http://3g.vehdjk.com/Article/details/gwfvstcss.sHtML

"值: \(b)"
来源：http://read.share.vehdjk.com/Article/details/gbtiwxfkg.sHtML

[T19] Swift：可选绑定
来源：http://baike.vehdjk.com/Article/details/gcldjotcc.sHtML

if let n = opt { print(n) }
来源：http://wap.tarul.cn/Article/details/gqmmkoeqj.sHtML

[T20] Swift：数组操作
来源：http://read.share.yfazqb.com/Article/details/glbudwjqv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.yfazqb.com/Article/details/gcfrngzsj.sHtML

[T21] Swift：遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gbvsmlcwz.sHtML

for x in a { print(x) }
来源：http://m.share.yfazqb.com/Article/details/gwhewyydz.sHtML

[T22] Swift：字典
来源：http://blog.epnwcf.com/Article/details/gikrmssls.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.sjlbkw.cn/Article/details/gblszdizg.sHtML

[T23] Swift：函数
来源：http://www.share.vehdjk.com/Article/details/gxwfmfpuu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.yfazqb.com/Article/details/guthivxar.sHtML

[T24] Swift：闭包
来源：http://blog.bbcook.cn/Article/details/gjdhglkkd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gcumllgmd.sHtML

[T25] Swift：结构体
来源：http://m.share.sjlbkw.cn/Article/details/gxluqnpgp.sHtML

struct P { var x: Int }
来源：http://3g.yfazqb.com/Article/details/gqljneinc.sHtML

[T26] Swift：类与重写
来源：http://read.share.vehdjk.com/Article/details/gkwcgfcui.sHtML

class A: Base { override func f() {} }
来源：http://wap.yfazqb.com/Article/details/gdmtqjjin.sHtML

[T27] Swift：错误处理
来源：http://www.share.bbcook.cn/Article/details/ggwuyfqgi.sHtML

do { try f() } catch { print(error) }
来源：http://3g.vehdjk.com/Article/details/gvstuxsds.sHtML

[T28] Swift：枚举
来源：http://blog.yfazqb.com/Article/details/gurbtnyie.sHtML

enum Color { case red, green }
来源：http://read.share.fktsv.cn/Article/details/gcdzhwcrr.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.yfazqb.com/Article/details/goeizjyhn.sHtML

guard let x = opt else { return }
来源：http://wap.bbcook.cn/Article/details/gbaoyvxwj.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/gopqpfjpz.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.bbcook.cn/Article/details/gccmowcbv.sHtML

[T31] Lua：Hello World
来源：http://m.share.bbcook.cn/Article/details/ghgqneswg.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gjfwbfxpz.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gsmjratti.sHtML

local a = 1
来源：http://wap.sjlbkw.cn/Article/details/gkwbhbhrv.sHtML

[T33] Lua：表（数组）
来源：http://blog.sjlbkw.cn/Article/details/gicvbfikj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.sjlbkw.cn/Article/details/grecwclee.sHtML

[T34] Lua：遍历表
来源：http://www.blog.sjlbkw.cn/Article/details/gexxrtuxp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.yfazqb.com/Article/details/gmyhntzgk.sHtML

[T35] Lua：字典表
来源：http://www.blog.vehdjk.com/Article/details/gcujfiajd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.yfazqb.com/Article/details/gilkroxpl.sHtML

[T36] Lua：函数
来源：http://blog.vehdjk.com/Article/details/gfkaxuxvf.sHtML

function add(a, b) return a + b end
来源：http://www.blog.vehdjk.com/Article/details/gpyypqpuc.sHtML

[T37] Lua：字符串拼接
来源：http://baike.yfazqb.com/Article/details/gimpnbhkw.sHtML

"a" .. "b"
来源：http://3g.sjlbkw.cn/Article/details/gotgffcsx.sHtML

[T38] Lua：条件
来源：http://www.m.share.bbcook.cn/Article/details/gudnxfueu.sHtML

if x > 0 then print("正") end
来源：http://blog.epnwcf.com/Article/details/gorvkszfj.sHtML

[T39] Lua：模式匹配
来源：http://mobile.epnwcf.com/Article/details/gcztxssdp.sHtML

string.find(s, "%d+")
来源：http://baike.fktsv.cn/Article/details/gizoffzrb.sHtML

[T40] Lua：元表
来源：http://read.share.epnwcf.com/Article/details/gggcivmvy.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.yfazqb.com/Article/details/gllpaahuf.sHtML

[T41] Perl：Hello World
来源：http://m.share.tarul.cn/Article/details/gvobbopyc.sHtML

print "Hello\n";
来源：http://blog.sjlbkw.cn/Article/details/gqytexkxq.sHtML

[T42] Perl：变量类型
来源：http://www.share.vehdjk.com/Article/details/gfcuvsyan.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.epnwcf.com/Article/details/gernnhpzv.sHtML

[T43] Perl：字符串插值
来源：http://wap.yfazqb.com/Article/details/gnrsoqvbs.sHtML

"值: $a"
来源：http://www.share.vehdjk.com/Article/details/gqperegyp.sHtML

[T44] Perl：条件
来源：http://wap.epnwcf.com/Article/details/ghukixxwt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.yfazqb.com/Article/details/gwxdfaqyu.sHtML

[T45] Perl：数组遍历
来源：http://m.share.vehdjk.com/Article/details/gomvixbnt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.bbcook.cn/Article/details/gxrnerzsc.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.sjlbkw.cn/Article/details/gzdgsbvmc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.yfazqb.com/Article/details/gjnomnrmm.sHtML

[T47] Perl：正则捕获
来源：http://read.share.bbcook.cn/Article/details/gyaeaolpt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.sjlbkw.cn/Article/details/gxyadgshn.sHtML

[T48] Perl：正则替换
来源：http://baike.bbcook.cn/Article/details/gbupxyotb.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fktsv.cn/Article/details/ggrcptyvk.sHtML

[T49] Perl：函数
来源：http://www.share.sjlbkw.cn/Article/details/gsjzbvpdj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gjkmzqdcy.sHtML

[T50] Perl：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gqkxyxqrl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.bbcook.cn/Article/details/glthmjuzm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.epnwcf.com/Article/details/glbstgkee.sHtML

[T51] Scala：Hello World
来源：http://blog.vehdjk.com/Article/details/gmvovplwf.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gfdhyeyub.sHtML

[T52] Scala：变量
来源：http://baike.bbcook.cn/Article/details/gqjmbbugd.sHtML

val a = 1;  var b = 2
来源：http://baike.tarul.cn/Article/details/geqfpmnls.sHtML

[T53] Scala：字符串插值
来源：http://wap.yfazqb.com/Article/details/gupbxhcvf.sHtML

s"值: $b"
来源：http://baike.fktsv.cn/Article/details/guxmjbusn.sHtML

[T54] Scala：集合映射
来源：http://read.share.epnwcf.com/Article/details/gnmfylfpf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.yfazqb.com/Article/details/grvjyugtb.sHtML

[T55] Scala：集合过滤
来源：http://baike.fktsv.cn/Article/details/gxwiwqxav.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.tarul.cn/Article/details/gqkvbrrzr.sHtML

[T56] Scala：样例类
来源：http://read.share.epnwcf.com/Article/details/grratvnhv.sHtML

case class User(name: String, age: Int)
来源：http://wap.yfazqb.com/Article/details/gwthcjvty.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/gnwydixjo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.tarul.cn/Article/details/gdxkaefrb.sHtML

[T58] Scala：函数定义
来源：http://blog.vehdjk.com/Article/details/ganclxuzg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.yfazqb.com/Article/details/gnwhxrwkj.sHtML

[T59] Scala：循环
来源：http://3g.yfazqb.com/Article/details/gyxzkrmnm.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.epnwcf.com/Article/details/gqlzaufyi.sHtML

[T60] Scala：折叠
来源：http://blog.epnwcf.com/Article/details/gzpgxaouh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.tarul.cn/Article/details/gbfjsmchn.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkvizctml.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.sjlbkw.cn/Article/details/gogtdxxuz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxvrajdyh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.bbcook.cn/Article/details/glgrxqvqj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.yfazqb.com/Article/details/gweudbqub.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.bbcook.cn/Article/details/gfwyfsimq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fktsv.cn/Article/details/gsahdylhl.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.vehdjk.com/Article/details/gsrnpzuij.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.yfazqb.com/Article/details/gwcuaitru.sHtML

[U04] Py：变量调试打印
来源：http://read.share.vehdjk.com/Article/details/gsltniwhb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.tarul.cn/Article/details/gxfklucxb.sHtML

[U05] Py：列表去重且保序
来源：http://blog.tarul.cn/Article/details/gduvoejhm.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/gczrnlwxf.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.bbcook.cn/Article/details/gkeoblgqw.sHtML

{**a, **b}
来源：http://blog.fktsv.cn/Article/details/ggusehyof.sHtML

[U07] Py：反转字典键值
来源：http://blog.fktsv.cn/Article/details/gxlpsnbis.sHtML

{v: k for k, v in d.items()}
来源：http://3g.yfazqb.com/Article/details/gxyvvvwbr.sHtML

[U08] Py：展平二维列表
来源：http://read.share.vehdjk.com/Article/details/gjgxtyzsu.sHtML

[y for x in nested for y in x]
来源：http://baike.fktsv.cn/Article/details/gcubgsfwu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.epnwcf.com/Article/details/gyqmoarij.sHtML

max(d, key=d.get)
来源：http://m.share.vehdjk.com/Article/details/gyiikwzsu.sHtML

[U10] Py：按值排序字典
来源：http://3g.yfazqb.com/Article/details/gheetcqpe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fktsv.cn/Article/details/guuylhdaw.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.vehdjk.com/Article/details/gujrjyaht.sHtML

(x * 2 for x in arr)
来源：http://read.share.yfazqb.com/Article/details/gvboryzln.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.bbcook.cn/Article/details/gpjxxygng.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.bbcook.cn/Article/details/gmbrkivzh.sHtML

[U13] Py：固定长度队列
来源：http://read.share.sjlbkw.cn/Article/details/gvwjwlyfk.sHtML

deque(maxlen=10)
来源：http://wap.fktsv.cn/Article/details/gjcegiyno.sHtML

[U14] Py：分组收集到列表
来源：http://baike.epnwcf.com/Article/details/gvoygfdbg.sHtML

defaultdict(list)
来源：http://www.share.yfazqb.com/Article/details/geusqcgge.sHtML

[U15] Py：高精度计时
来源：http://m.share.yfazqb.com/Article/details/gholkbpyg.sHtML

t = time.perf_counter()
来源：http://mobile.yfazqb.com/Article/details/guhwrxvzk.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.tarul.cn/Article/details/gopprbmas.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.tarul.cn/Article/details/gbdzjtebp.sHtML

[U17] Py：初始化日志
来源：http://read.share.yfazqb.com/Article/details/gbkqzhzjm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.bbcook.cn/Article/details/gazdodhrj.sHtML

[U18] Py：预编译正则
来源：http://baike.sjlbkw.cn/Article/details/gpzavcytq.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.yfazqb.com/Article/details/gdvmbuseb.sHtML

[U19] Py：正则替换带回调
来源：http://baike.epnwcf.com/Article/details/gfgrboexr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.bbcook.cn/Article/details/gkffhxsnd.sHtML

[U20] Py：缓存函数结果
来源：http://wap.tarul.cn/Article/details/gmgcdnxoq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.vehdjk.com/Article/details/gyfqokbig.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fktsv.cn/Article/details/gofebzrpt.sHtML

@contextlib.contextmanager
来源：http://m.share.fktsv.cn/Article/details/geifjdnyd.sHtML

[U22] Py：矩阵转置
来源：http://blog.yfazqb.com/Article/details/gvecsswml.sHtML

list(zip(*m))
来源：http://blog.vehdjk.com/Article/details/gnukrevpe.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fktsv.cn/Article/details/gpjcgwlbg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.epnwcf.com/Article/details/gnqkhiujd.sHtML

[U24] Py：路径操作
来源：http://www.blog.fktsv.cn/Article/details/gwnyehkrj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/gxxhyuqfn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.epnwcf.com/Article/details/ggjvcqjtt.sHtML

csv.DictReader(f)
来源：http://blog.bbcook.cn/Article/details/gwvqmjytp.sHtML

[U26] Py：并发下载
来源：http://m.share.fktsv.cn/Article/details/gponwfvld.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.tarul.cn/Article/details/gjilwidos.sHtML

[U27] Py：异步 HTTP
来源：http://3g.yfazqb.com/Article/details/gnjqlorxu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fktsv.cn/Article/details/grgwsondq.sHtML

[U28] Py：类型别名
来源：http://m.share.epnwcf.com/Article/details/gcdjvgucv.sHtML

UserId = int
来源：http://read.share.sjlbkw.cn/Article/details/ggjzlusmi.sHtML

[U29] Py：属性校验
来源：http://www.m.share.vehdjk.com/Article/details/gzczxrstd.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.bbcook.cn/Article/details/gpfvogxet.sHtML

[U30] Py：数据类
来源：http://m.share.fktsv.cn/Article/details/gjxxsvcfg.sHtML

@dataclass(slots=True)
来源：http://read.share.tarul.cn/Article/details/gxssroanv.sHtML

[U31] Py：单测
来源：http://www.m.share.yfazqb.com/Article/details/guzfmqivw.sHtML

python -m pytest -q
来源：http://blog.epnwcf.com/Article/details/ghyjwqhmo.sHtML

[U32] Py：代码格式化
来源：http://3g.epnwcf.com/Article/details/gmhkccvka.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.sjlbkw.cn/Article/details/gvaltxmbf.sHtML

[U33] Py：打包发布
来源：http://mobile.sjlbkw.cn/Article/details/gaauacdby.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.yfazqb.com/Article/details/gpvewgqrm.sHtML

[U34] Py：判断编码
来源：http://baike.bbcook.cn/Article/details/gsnwirygu.sHtML

chardet.detect(raw)
来源：http://mobile.vehdjk.com/Article/details/gmhgxrcys.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.yfazqb.com/Article/details/gwmenjcgz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fktsv.cn/Article/details/gzefboyqd.sHtML

[U36] Py：定时任务
来源：http://wap.epnwcf.com/Article/details/gyuwyhwyk.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.epnwcf.com/Article/details/giiaeoqgi.sHtML

[U37] Py：读写 Excel
来源：http://read.share.vehdjk.com/Article/details/gfrrahzsc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.vehdjk.com/Article/details/guozxuddv.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.epnwcf.com/Article/details/gkujxarxr.sHtML

Path(__file__).resolve().parent
来源：http://m.share.tarul.cn/Article/details/gimatexrn.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fktsv.cn/Article/details/gtbgkvzut.sHtML

sys.stdout.isatty()
来源：http://mobile.sjlbkw.cn/Article/details/ggzdlgpxt.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fktsv.cn/Article/details/gzfoysmbl.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gcbcxbgnq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.sjlbkw.cn/Article/details/goeelzmww.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.sjlbkw.cn/Article/details/gdzgtgoqe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.yfazqb.com/Article/details/gcjgduqhu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.sjlbkw.cn/Article/details/ghqpehcaq.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.bbcook.cn/Article/details/gwerinkqp.sHtML

namespace App\Http;
来源：http://baike.yfazqb.com/Article/details/gjdmcgias.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.sjlbkw.cn/Article/details/gsaehjthl.sHtML

declare(strict_types=1);
来源：http://wap.fktsv.cn/Article/details/gahbmmbdt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.epnwcf.com/Article/details/gbxnsvpav.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/giasflgvd.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.bbcook.cn/Article/details/gtddykaua.sHtML

?string $name = null
来源：http://mobile.epnwcf.com/Article/details/geussknub.sHtML

[U47] PHP：联合类型
来源：http://mobile.bbcook.cn/Article/details/gfuegvmuk.sHtML

int|string $id
来源：http://m.share.vehdjk.com/Article/details/gkrnhmmgf.sHtML

[U48] PHP：纯枚举
来源：http://www.share.sjlbkw.cn/Article/details/gxvafgiqt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fktsv.cn/Article/details/gwwwqyeci.sHtML

[U49] PHP：只读属性
来源：http://wap.vehdjk.com/Article/details/gywgbovjn.sHtML

public readonly string $name
来源：http://wap.sjlbkw.cn/Article/details/gksomucqd.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.yfazqb.com/Article/details/gnmqxnxjg.sHtML

public function __construct(private int $id) {}
来源：http://mobile.tarul.cn/Article/details/godmfmsla.sHtML

[U51] PHP：数组解构
来源：http://mobile.yfazqb.com/Article/details/gevieouyb.sHtML

[$a, $b] = $arr;
来源：http://mobile.yfazqb.com/Article/details/gthuwymro.sHtML

[U52] PHP：箭头函数
来源：http://baike.vehdjk.com/Article/details/gbikmgqip.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fktsv.cn/Article/details/ggagavahm.sHtML

[U53] PHP：空合并运算符
来源：http://wap.yfazqb.com/Article/details/gclhisoky.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.bbcook.cn/Article/details/glzcdhbta.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.sjlbkw.cn/Article/details/gvjkxlyty.sHtML

$obj?->method()
来源：http://m.share.tarul.cn/Article/details/gaxqdzocf.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.vehdjk.com/Article/details/gsputdlwh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fktsv.cn/Article/details/ghgtnkagu.sHtML

[U56] PHP：命名参数
来源：http://wap.yfazqb.com/Article/details/gtevpnzqv.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gsagpupfh.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/ghtnyfwwp.sHtML

"值: {$a}"
来源：http://baike.yfazqb.com/Article/details/gsonxkjwp.sHtML

[U58] PHP：数组三件套
来源：http://3g.fktsv.cn/Article/details/gcqmuhgia.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.epnwcf.com/Article/details/gtxtxmitw.sHtML


<!-- 参考信息 -->