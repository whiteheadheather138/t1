代发 wailian999

#include <iostream>
来源：http://m.share.fktsv.cn/Article/details/ggnmxcipz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/gkmwxhxdw.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/glszoivko.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxotltov.sHtML

[S33] C++：vector 增删
来源：http://wap.sjlbkw.cn/Article/details/ggdmtqoxi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.tarul.cn/Article/details/gwelgijzb.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/gtuhwvvzf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fktsv.cn/Article/details/geedeadae.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/glsamllyn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gpfpofxvq.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/gexjumcum.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gmzoejoqo.sHtML

[S37] C++：set
来源：http://3g.bbcook.cn/Article/details/gopjcscnk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.tarul.cn/Article/details/giezxidng.sHtML

[S38] C++：排序
来源：http://www.m.share.bbcook.cn/Article/details/gnxpemgeu.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fktsv.cn/Article/details/glgqvlxru.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.vehdjk.com/Article/details/ggrblmeqr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.sjlbkw.cn/Article/details/gjyzjwlkf.sHtML

[S40] C++：查找元素
来源：http://baike.fktsv.cn/Article/details/gfbjseicy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/gxtrxxdye.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.bbcook.cn/Article/details/grnanxhjq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.epnwcf.com/Article/details/guoviwxxw.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.vehdjk.com/Article/details/gbtqlvefi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/galwxujkb.sHtML

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/gjdypubid.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.tarul.cn/Article/details/grzyicgzc.sHtML

[S44] C++：引用传参
来源：http://baike.tarul.cn/Article/details/gtgdatywh.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/gilxvngth.sHtML

[S45] C++：lambda
来源：http://blog.tarul.cn/Article/details/gcfqunpax.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.tarul.cn/Article/details/guygauyxo.sHtML

[S46] C++：函数模板
来源：http://www.m.share.yfazqb.com/Article/details/galvnysxt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggdfaruhg.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/gpajayepk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.sjlbkw.cn/Article/details/gtdpmzeou.sHtML

[S48] C++：逐行读文件
来源：http://wap.vehdjk.com/Article/details/giaoeavpz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.tarul.cn/Article/details/gxzzqmfjj.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gakqgokrw.sHtML

[S49] C++：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gqkwhvavl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.vehdjk.com/Article/details/gscotthmw.sHtML

[S50] C++：格式化数字
来源：http://baike.vehdjk.com/Article/details/glnyjoldr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gqrbyjprw.sHtML

[S51] C++：显式类型转换
来源：http://blog.fktsv.cn/Article/details/gvniyrzvz.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/grhjemeta.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.vehdjk.com/Article/details/gdndutban.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/guivyjinl.sHtML

[S53] C++：移动语义
来源：http://3g.sjlbkw.cn/Article/details/gxgrwjhsw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.bbcook.cn/Article/details/gkkmwnbba.sHtML

[S54] C++：异常处理
来源：http://mobile.yfazqb.com/Article/details/gdndrjaug.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/gdsipmovl.sHtML

[S55] C++：结构化绑定
来源：http://wap.epnwcf.com/Article/details/gltdijrwz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/gbudbcleg.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/gdndjezpj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.sjlbkw.cn/Article/details/gbkprleph.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/glxlcfgqg.sHtML

constexpr int N = 10;
来源：http://read.share.epnwcf.com/Article/details/gekngvpgd.sHtML

[S58] C++：命名空间
来源：http://mobile.sjlbkw.cn/Article/details/gcrzdjaqf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fktsv.cn/Article/details/gtatwhhlr.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/gesgvfaev.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.bbcook.cn/Article/details/gmdefydon.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.bbcook.cn/Article/details/gzsffzscw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.vehdjk.com/Article/details/gnhlnspcw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqqtfrucg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/grkqmlllq.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggaauxewp.sHtML

[T01] Kotlin：Hello World
来源：http://3g.vehdjk.com/Article/details/goqamzewz.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/gryyvabdo.sHtML

[T02] Kotlin：变量
来源：http://blog.epnwcf.com/Article/details/gbtqbuqpa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.sjlbkw.cn/Article/details/gxxrueizk.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.yfazqb.com/Article/details/gbopwdual.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/guhfcvccx.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fktsv.cn/Article/details/gvqjkfbzf.sHtML

val n: String? = null;  n?.length
来源：http://read.share.bbcook.cn/Article/details/gfzitalds.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gsvnkxeyx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/gmkmofomn.sHtML

[T06] Kotlin：集合映射
来源：http://baike.bbcook.cn/Article/details/gasuytjik.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.yfazqb.com/Article/details/gwrmjcven.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/ggneenvnw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/geyfhvcwh.sHtML

[T08] Kotlin：数据类
来源：http://3g.vehdjk.com/Article/details/ggyftlemu.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.epnwcf.com/Article/details/gttwtleei.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fktsv.cn/Article/details/gzgetwqid.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwistoix.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gnqhvomod.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.bbcook.cn/Article/details/gpajwnsey.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.vehdjk.com/Article/details/gegwboasm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/getkczllg.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.bbcook.cn/Article/details/glqeckakw.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.bbcook.cn/Article/details/gnudpxpff.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.yfazqb.com/Article/details/gzrziomfd.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.bbcook.cn/Article/details/gzxuwufpc.sHtML

[T14] Kotlin：循环
来源：http://m.share.yfazqb.com/Article/details/gosfncvww.sHtML

for (i in 1..10) println(i)
来源：http://3g.tarul.cn/Article/details/grmbhfbgr.sHtML

[T15] Kotlin：接口
来源：http://3g.fktsv.cn/Article/details/gzpjlybta.sHtML

interface Shape { fun area(): Double }
来源：http://3g.epnwcf.com/Article/details/gokxwyivj.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gqfbxotkx.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gzcwyynbh.sHtML

[T17] Swift：变量与常量
来源：http://read.share.bbcook.cn/Article/details/gnhlvrzuv.sHtML

var a = 1;  let b = 2
来源：http://3g.vehdjk.com/Article/details/gjldhdfah.sHtML

[T18] Swift：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gyfyqvpve.sHtML

"值: \(b)"
来源：http://blog.sjlbkw.cn/Article/details/gqatbmnoi.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.epnwcf.com/Article/details/goalupqai.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/gqveevefl.sHtML

[T20] Swift：数组操作
来源：http://m.share.tarul.cn/Article/details/gxzefrwuq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fktsv.cn/Article/details/gsmygwyhj.sHtML

[T21] Swift：遍历
来源：http://baike.yfazqb.com/Article/details/gnzqqpehl.sHtML

for x in a { print(x) }
来源：http://www.blog.sjlbkw.cn/Article/details/ggcbjysim.sHtML

[T22] Swift：字典
来源：http://m.share.vehdjk.com/Article/details/glghgrnhl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.epnwcf.com/Article/details/gdvfqmumw.sHtML

[T23] Swift：函数
来源：http://read.share.yfazqb.com/Article/details/grdyogmaf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.yfazqb.com/Article/details/gbeywltvd.sHtML

[T24] Swift：闭包
来源：http://www.m.share.yfazqb.com/Article/details/gnnftuzvp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.tarul.cn/Article/details/gkkvynepi.sHtML

[T25] Swift：结构体
来源：http://www.blog.bbcook.cn/Article/details/gfehchuvn.sHtML

struct P { var x: Int }
来源：http://3g.sjlbkw.cn/Article/details/gkoqsccqu.sHtML

[T26] Swift：类与重写
来源：http://3g.fktsv.cn/Article/details/ghqurkofg.sHtML

class A: Base { override func f() {} }
来源：http://www.share.sjlbkw.cn/Article/details/guiahyfyv.sHtML

[T27] Swift：错误处理
来源：http://read.share.vehdjk.com/Article/details/gvrqlsuux.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.yfazqb.com/Article/details/gyenaqecg.sHtML

[T28] Swift：枚举
来源：http://baike.fktsv.cn/Article/details/gdhzyncov.sHtML

enum Color { case red, green }
来源：http://read.share.bbcook.cn/Article/details/gwpwrdfdh.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.yfazqb.com/Article/details/gamyfiivk.sHtML

guard let x = opt else { return }
来源：http://baike.fktsv.cn/Article/details/gyaiakpxu.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/gqbhgjnwb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.bbcook.cn/Article/details/gdmrjxsra.sHtML

[T31] Lua：Hello World
来源：http://read.share.tarul.cn/Article/details/gnktvmdpn.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/gbfhumylk.sHtML

[T32] Lua：局部变量
来源：http://blog.vehdjk.com/Article/details/gjmzjqtkd.sHtML

local a = 1
来源：http://wap.tarul.cn/Article/details/gqafjswhr.sHtML

[T33] Lua：表（数组）
来源：http://wap.yfazqb.com/Article/details/ggtdgjaxw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.vehdjk.com/Article/details/gdhpuaxhm.sHtML

[T34] Lua：遍历表
来源：http://baike.vehdjk.com/Article/details/gxoaspttp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fktsv.cn/Article/details/ghmnenwto.sHtML

[T35] Lua：字典表
来源：http://baike.yfazqb.com/Article/details/glduoicii.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gzkxonmur.sHtML

[T36] Lua：函数
来源：http://baike.fktsv.cn/Article/details/gmnkqocfd.sHtML

function add(a, b) return a + b end
来源：http://www.blog.yfazqb.com/Article/details/gltylypfz.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fktsv.cn/Article/details/gbeufecid.sHtML

"a" .. "b"
来源：http://www.share.epnwcf.com/Article/details/gdygpvrty.sHtML

[T38] Lua：条件
来源：http://blog.fktsv.cn/Article/details/gjrqeqigz.sHtML

if x > 0 then print("正") end
来源：http://m.share.tarul.cn/Article/details/glwfoyosc.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gfrebrzoq.sHtML

string.find(s, "%d+")
来源：http://mobile.vehdjk.com/Article/details/gpdervkox.sHtML

[T40] Lua：元表
来源：http://m.share.fktsv.cn/Article/details/gujymyoph.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.vehdjk.com/Article/details/giuylhbgr.sHtML

[T41] Perl：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gvftnazxe.sHtML

print "Hello\n";
来源：http://mobile.vehdjk.com/Article/details/gmoohdags.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.vehdjk.com/Article/details/gazevmack.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.sjlbkw.cn/Article/details/gntlcxpty.sHtML

[T43] Perl：字符串插值
来源：http://3g.bbcook.cn/Article/details/gnzxlqsmt.sHtML

"值: $a"
来源：http://wap.fktsv.cn/Article/details/grzymftwp.sHtML

[T44] Perl：条件
来源：http://blog.fktsv.cn/Article/details/gtdpvvwyy.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.yfazqb.com/Article/details/gwspiiczt.sHtML

[T45] Perl：数组遍历
来源：http://read.share.vehdjk.com/Article/details/getezcwms.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fktsv.cn/Article/details/gbhbjxfkk.sHtML

[T46] Perl：哈希操作
来源：http://blog.fktsv.cn/Article/details/gieryqega.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.tarul.cn/Article/details/ghmdednka.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fktsv.cn/Article/details/ghbcnjjhc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.vehdjk.com/Article/details/gialfucww.sHtML

[T48] Perl：正则替换
来源：http://www.blog.epnwcf.com/Article/details/gijqnbkwv.sHtML

$s =~ s/old/new/g;
来源：http://mobile.yfazqb.com/Article/details/gpywhiarc.sHtML

[T49] Perl：函数
来源：http://www.share.epnwcf.com/Article/details/gwkyicogj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gcncjjvwc.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gdmetstwb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.epnwcf.com/Article/details/gtmighryu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.tarul.cn/Article/details/gauodbjhe.sHtML

[T51] Scala：Hello World
来源：http://www.share.epnwcf.com/Article/details/ghwrtugfj.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gjgcpdzpc.sHtML

[T52] Scala：变量
来源：http://www.share.tarul.cn/Article/details/getctrkva.sHtML

val a = 1;  var b = 2
来源：http://m.share.yfazqb.com/Article/details/gjkpaaaob.sHtML

[T53] Scala：字符串插值
来源：http://read.share.tarul.cn/Article/details/gulvotvjk.sHtML

s"值: $b"
来源：http://blog.yfazqb.com/Article/details/gwpnsrktj.sHtML

[T54] Scala：集合映射
来源：http://3g.epnwcf.com/Article/details/gtmlrcxgy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.epnwcf.com/Article/details/ggudjligg.sHtML

[T55] Scala：集合过滤
来源：http://blog.epnwcf.com/Article/details/gkfzvpyta.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/getjtqawf.sHtML

[T56] Scala：样例类
来源：http://www.m.share.yfazqb.com/Article/details/gymydmpuh.sHtML

case class User(name: String, age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gdkeciijh.sHtML

[T57] Scala：模式匹配
来源：http://wap.epnwcf.com/Article/details/gcuwrtete.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/galqcliqz.sHtML

[T58] Scala：函数定义
来源：http://3g.fktsv.cn/Article/details/gkcmhlfvj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.vehdjk.com/Article/details/gvqbtzatm.sHtML

[T59] Scala：循环
来源：http://read.share.sjlbkw.cn/Article/details/gfuumhdgb.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.tarul.cn/Article/details/gbcvpvzsp.sHtML

[T60] Scala：折叠
来源：http://mobile.yfazqb.com/Article/details/gcujcztye.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.bbcook.cn/Article/details/ghtbmbdyz.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqgtfqzwb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.bbcook.cn/Article/details/gbwnsbdwp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmmhpxeib.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.vehdjk.com/Article/details/geopxwzuk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.vehdjk.com/Article/details/gymcoyvmk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.tarul.cn/Article/details/gthivoenu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.yfazqb.com/Article/details/gzihdfnmn.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/gusbpopbj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.tarul.cn/Article/details/gwhbhbuay.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/guuvqhbdu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.sjlbkw.cn/Article/details/ggnbjxdei.sHtML

[U05] Py：列表去重且保序
来源：http://wap.vehdjk.com/Article/details/gbywqcftr.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gugmlfnjm.sHtML

[U06] Py：合并两个字典
来源：http://www.share.epnwcf.com/Article/details/gufqjmoek.sHtML

{**a, **b}
来源：http://blog.yfazqb.com/Article/details/ggrjfuvrc.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.sjlbkw.cn/Article/details/gubljtmeh.sHtML

{v: k for k, v in d.items()}
来源：http://3g.yfazqb.com/Article/details/gdgixspzu.sHtML

[U08] Py：展平二维列表
来源：http://wap.bbcook.cn/Article/details/gpgajpcou.sHtML

[y for x in nested for y in x]
来源：http://www.share.tarul.cn/Article/details/gfsnyihlt.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.vehdjk.com/Article/details/gsktjhmzp.sHtML

max(d, key=d.get)
来源：http://m.share.yfazqb.com/Article/details/ghlaiksdd.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.bbcook.cn/Article/details/gcbgfzxib.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.sjlbkw.cn/Article/details/gogzdocds.sHtML

[U11] Py：生成器表达式
来源：http://www.share.sjlbkw.cn/Article/details/grlodbzgy.sHtML

(x * 2 for x in arr)
来源：http://www.share.sjlbkw.cn/Article/details/gnxbhxgkc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.tarul.cn/Article/details/gmapspyhm.sHtML

Counter(arr).most_common(3)
来源：http://mobile.bbcook.cn/Article/details/guoyfoshd.sHtML

[U13] Py：固定长度队列
来源：http://www.share.bbcook.cn/Article/details/gyurglewi.sHtML

deque(maxlen=10)
来源：http://www.blog.fktsv.cn/Article/details/gwfxwodjb.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.sjlbkw.cn/Article/details/gotafdvqy.sHtML

defaultdict(list)
来源：http://3g.vehdjk.com/Article/details/gcgmvujtd.sHtML

[U15] Py：高精度计时
来源：http://blog.bbcook.cn/Article/details/gwxegxdfh.sHtML

t = time.perf_counter()
来源：http://www.blog.tarul.cn/Article/details/gcgktcmrb.sHtML

[U16] Py：命令行参数解析
来源：http://baike.bbcook.cn/Article/details/gatlnmamg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.sjlbkw.cn/Article/details/gtpbvvjnf.sHtML

[U17] Py：初始化日志
来源：http://m.share.bbcook.cn/Article/details/gdxawduvx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.epnwcf.com/Article/details/gjpvbdcng.sHtML

[U18] Py：预编译正则
来源：http://www.blog.epnwcf.com/Article/details/grvzwxfei.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.tarul.cn/Article/details/gmbxzimnf.sHtML

[U19] Py：正则替换带回调
来源：http://3g.sjlbkw.cn/Article/details/gulyazeug.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.tarul.cn/Article/details/gjldarirq.sHtML

[U20] Py：缓存函数结果
来源：http://baike.bbcook.cn/Article/details/gujbglyfi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.yfazqb.com/Article/details/gqmxpxgzp.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.sjlbkw.cn/Article/details/gszkqgppt.sHtML

@contextlib.contextmanager
来源：http://3g.bbcook.cn/Article/details/gshhuagzl.sHtML

[U22] Py：矩阵转置
来源：http://wap.sjlbkw.cn/Article/details/gmvbxpxxz.sHtML

list(zip(*m))
来源：http://www.share.tarul.cn/Article/details/gqxgxyqkz.sHtML

[U23] Py：分块读取大文件
来源：http://3g.tarul.cn/Article/details/gsrzwtlwk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.bbcook.cn/Article/details/gqhlwkycl.sHtML

[U24] Py：路径操作
来源：http://3g.bbcook.cn/Article/details/gltehwuga.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.yfazqb.com/Article/details/grtistzid.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fktsv.cn/Article/details/grvbabvaq.sHtML

csv.DictReader(f)
来源：http://www.blog.vehdjk.com/Article/details/gakksltak.sHtML

[U26] Py：并发下载
来源：http://mobile.bbcook.cn/Article/details/gdmkrrxzw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.sjlbkw.cn/Article/details/gjaukadwv.sHtML

[U27] Py：异步 HTTP
来源：http://baike.sjlbkw.cn/Article/details/genrtgnum.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.bbcook.cn/Article/details/gvwydwcra.sHtML

[U28] Py：类型别名
来源：http://mobile.vehdjk.com/Article/details/gazpiunsr.sHtML

UserId = int
来源：http://mobile.vehdjk.com/Article/details/gfynckklj.sHtML

[U29] Py：属性校验
来源：http://www.blog.tarul.cn/Article/details/gegidhxhc.sHtML

@property 与 @x.setter 配合
来源：http://3g.vehdjk.com/Article/details/gifqgktbk.sHtML

[U30] Py：数据类
来源：http://mobile.fktsv.cn/Article/details/gxkhqxmys.sHtML

@dataclass(slots=True)
来源：http://mobile.fktsv.cn/Article/details/gbwkylsho.sHtML

[U31] Py：单测
来源：http://wap.bbcook.cn/Article/details/gewmyorqk.sHtML

python -m pytest -q
来源：http://www.m.share.yfazqb.com/Article/details/glhikhhbj.sHtML

[U32] Py：代码格式化
来源：http://www.blog.tarul.cn/Article/details/gpngboors.sHtML

ruff format . && ruff check --fix .
来源：http://wap.tarul.cn/Article/details/glalqpspc.sHtML

[U33] Py：打包发布
来源：http://read.share.tarul.cn/Article/details/gpfcamkqy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fktsv.cn/Article/details/gdqdeslkk.sHtML

[U34] Py：判断编码
来源：http://read.share.bbcook.cn/Article/details/gmoawqpme.sHtML

chardet.detect(raw)
来源：http://mobile.sjlbkw.cn/Article/details/gmirkmnbx.sHtML

[U35] Py：发送邮件
来源：http://baike.bbcook.cn/Article/details/gfgpqcarq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fktsv.cn/Article/details/ghjgcxxdw.sHtML

[U36] Py：定时任务
来源：http://read.share.tarul.cn/Article/details/gzayriniz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fktsv.cn/Article/details/gyzowhccc.sHtML

[U37] Py：读写 Excel
来源：http://m.share.sjlbkw.cn/Article/details/gsmgvwzkz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.epnwcf.com/Article/details/gwbpmwslf.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fktsv.cn/Article/details/gamdnsrig.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.sjlbkw.cn/Article/details/gwwbuixif.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.bbcook.cn/Article/details/gupercaml.sHtML

sys.stdout.isatty()
来源：http://www.blog.vehdjk.com/Article/details/gjitdbqct.sHtML

[U40] Py：打印到标准错误
来源：http://blog.bbcook.cn/Article/details/gptszgxgu.sHtML

print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/geaoaegld.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.tarul.cn/Article/details/gvtfnmdiz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.sjlbkw.cn/Article/details/gjnwzchgo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.bbcook.cn/Article/details/gfxvbypnu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.vehdjk.com/Article/details/giwqugdpp.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fktsv.cn/Article/details/gerlohins.sHtML

namespace App\Http;
来源：http://blog.tarul.cn/Article/details/gjhvrgjqr.sHtML

[U44] PHP：开启严格类型
来源：http://3g.bbcook.cn/Article/details/gorqbvorx.sHtML

declare(strict_types=1);
来源：http://baike.tarul.cn/Article/details/gdlnblhff.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.sjlbkw.cn/Article/details/gyiodmlim.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gorltvitv.sHtML

[U46] PHP：可空类型
来源：http://read.share.epnwcf.com/Article/details/gcaxyizya.sHtML

?string $name = null
来源：http://mobile.sjlbkw.cn/Article/details/gfhkpuliz.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdeerkpk.sHtML

int|string $id
来源：http://wap.fktsv.cn/Article/details/gzclpggzw.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.tarul.cn/Article/details/gsymyhagj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fktsv.cn/Article/details/gpeynjdxb.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fktsv.cn/Article/details/gdnhaqeha.sHtML

public readonly string $name
来源：http://wap.yfazqb.com/Article/details/gommzsfmo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fktsv.cn/Article/details/gpecufwuv.sHtML

public function __construct(private int $id) {}
来源：http://read.share.tarul.cn/Article/details/gnvxmitvf.sHtML

[U51] PHP：数组解构
来源：http://mobile.sjlbkw.cn/Article/details/gyunowuwi.sHtML

[$a, $b] = $arr;
来源：http://blog.sjlbkw.cn/Article/details/gilhslwch.sHtML

[U52] PHP：箭头函数
来源：http://mobile.yfazqb.com/Article/details/gencsqmmt.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.sjlbkw.cn/Article/details/gmglpruii.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.vehdjk.com/Article/details/gvqtydlov.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.bbcook.cn/Article/details/gjjqpdjrw.sHtML

[U54] PHP：空安全调用
来源：http://wap.bbcook.cn/Article/details/gxbnmnchd.sHtML

$obj?->method()
来源：http://www.blog.yfazqb.com/Article/details/gcuqblpjg.sHtML

[U55] PHP：match 表达式
来源：http://blog.sjlbkw.cn/Article/details/grgqimnlt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.vehdjk.com/Article/details/gugukxgnh.sHtML

[U56] PHP：命名参数
来源：http://www.share.fktsv.cn/Article/details/gwxgrphfr.sHtML

f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gtaxpdgpi.sHtML


<!-- 参考信息 -->