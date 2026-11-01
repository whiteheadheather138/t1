代发 wailian999

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/gxlrzydhw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/ggwpfnsro.sHtML

[S36] C++：unordered_map
来源：http://blog.bbcook.cn/Article/details/glydvpayl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/gcnbiayyv.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/gdjbvetnu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gyomolpti.sHtML

[S38] C++：排序
来源：http://www.m.share.yfazqb.com/Article/details/gnwsdnyer.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fktsv.cn/Article/details/gfbdtiaoo.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/glcjndqgl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.vehdjk.com/Article/details/gweltfkdk.sHtML

[S40] C++：查找元素
来源：http://www.share.vehdjk.com/Article/details/gxflxucwu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.sjlbkw.cn/Article/details/ggttwhzza.sHtML

[S41] C++：类与构造函数
来源：http://m.share.vehdjk.com/Article/details/gpowvlszx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fktsv.cn/Article/details/ggshjocgi.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.tarul.cn/Article/details/gpkqohhcv.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.vehdjk.com/Article/details/ggdlheqww.sHtML

[S43] C++：智能指针
来源：http://mobile.vehdjk.com/Article/details/ghefxohmr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.yfazqb.com/Article/details/gagongwzk.sHtML

[S44] C++：引用传参
来源：http://m.share.bbcook.cn/Article/details/gsjczfisy.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.yfazqb.com/Article/details/gutunsbej.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/gulncppoq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.tarul.cn/Article/details/gsznwjsrr.sHtML

[S46] C++：函数模板
来源：http://mobile.tarul.cn/Article/details/gagmwkyyx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fktsv.cn/Article/details/gjryndfns.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.sjlbkw.cn/Article/details/gtdanemvb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.tarul.cn/Article/details/gkakwlsiy.sHtML

[S48] C++：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gnnbtpqpw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.vehdjk.com/Article/details/glphadcrf.sHtML

while (std::getline(in, line)) { }
来源：http://wap.yfazqb.com/Article/details/gcwpnolas.sHtML

[S49] C++：写文件
来源：http://read.share.tarul.cn/Article/details/gdsqlqcva.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.epnwcf.com/Article/details/gjynehrng.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gvvfgkdor.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.epnwcf.com/Article/details/gqxigxqsh.sHtML

[S51] C++：显式类型转换
来源：http://3g.sjlbkw.cn/Article/details/gztwzdqni.sHtML

static_cast<double>(a) / b
来源：http://www.blog.yfazqb.com/Article/details/gpwlizfma.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxtfbqmr.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.epnwcf.com/Article/details/gmmuinhom.sHtML

[S53] C++：移动语义
来源：http://3g.vehdjk.com/Article/details/grsruizbn.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fktsv.cn/Article/details/gzobqqmxp.sHtML

[S54] C++：异常处理
来源：http://m.share.sjlbkw.cn/Article/details/gommhelky.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.sjlbkw.cn/Article/details/gqojdqcxq.sHtML

[S55] C++：结构化绑定
来源：http://www.share.yfazqb.com/Article/details/gcdjaobys.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/glhnyhxwy.sHtML

[S56] C++：optional
来源：http://3g.yfazqb.com/Article/details/gizgxbxsq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.sjlbkw.cn/Article/details/gxdzrqcim.sHtML

[S57] C++：编译期常量
来源：http://mobile.vehdjk.com/Article/details/gjpjbpexh.sHtML

constexpr int N = 10;
来源：http://blog.sjlbkw.cn/Article/details/gmnavebcw.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gvetaordi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gkusaaqne.sHtML

[S59] C++：静态断言
来源：http://www.m.share.yfazqb.com/Article/details/gkievcosb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.bbcook.cn/Article/details/gkedhcqsc.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.sjlbkw.cn/Article/details/gtmykbwpf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/ghvaontao.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/glgqohlzz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/gifpgtkve.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gyuemhecn.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/gmwqyzkpc.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/goeaoscmu.sHtML

[T02] Kotlin：变量
来源：http://wap.vehdjk.com/Article/details/ggqanjnwn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.sjlbkw.cn/Article/details/gsgssuunu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.bbcook.cn/Article/details/gtpdbimsj.sHtML

"值: $b"
来源：http://baike.vehdjk.com/Article/details/gftoshejb.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.bbcook.cn/Article/details/gmdihmsci.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.epnwcf.com/Article/details/gdcdctpxj.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.epnwcf.com/Article/details/gdekmkxnd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.bbcook.cn/Article/details/goekjztuq.sHtML

[T06] Kotlin：集合映射
来源：http://3g.bbcook.cn/Article/details/ggtkkoipu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.bbcook.cn/Article/details/gyorulvru.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.tarul.cn/Article/details/ggrwgbqxx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.bbcook.cn/Article/details/gvmttnczb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fktsv.cn/Article/details/gegefgsrx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gxmlirtlx.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.vehdjk.com/Article/details/gudmjcmuz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.sjlbkw.cn/Article/details/gqfhdbeea.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fktsv.cn/Article/details/gbxlhzdwt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fktsv.cn/Article/details/gpgxwlkjp.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gbnglphsx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.sjlbkw.cn/Article/details/gbneohvni.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.tarul.cn/Article/details/gquscuvgt.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gddfaozsz.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.tarul.cn/Article/details/ggjtafjeq.sHtML

val m = mapOf("a" to 1)
来源：http://blog.vehdjk.com/Article/details/gwiycxoge.sHtML

[T14] Kotlin：循环
来源：http://3g.epnwcf.com/Article/details/gntjtrfoz.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/gjhzuluus.sHtML

[T15] Kotlin：接口
来源：http://mobile.tarul.cn/Article/details/guoofjack.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.bbcook.cn/Article/details/gonyocxgn.sHtML

[T16] Swift：Hello World
来源：http://blog.yfazqb.com/Article/details/ggirywfsx.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gctxlggmf.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.yfazqb.com/Article/details/gqlqrgyfr.sHtML

var a = 1;  let b = 2
来源：http://wap.epnwcf.com/Article/details/gsbzrchje.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/gqjgwqoyj.sHtML

"值: \(b)"
来源：http://blog.yfazqb.com/Article/details/gjidhhqmv.sHtML

[T19] Swift：可选绑定
来源：http://baike.vehdjk.com/Article/details/gbtvrexni.sHtML

if let n = opt { print(n) }
来源：http://blog.fktsv.cn/Article/details/gytremjmk.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/gdifbubqo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/grhfpykwi.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/gwbimmvpn.sHtML

for x in a { print(x) }
来源：http://3g.epnwcf.com/Article/details/gtxhtdzbk.sHtML

[T22] Swift：字典
来源：http://www.share.fktsv.cn/Article/details/gvfrwtupt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/gsrchfppk.sHtML

[T23] Swift：函数
来源：http://baike.bbcook.cn/Article/details/guxwfexns.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.tarul.cn/Article/details/gmqhixxkw.sHtML

[T24] Swift：闭包
来源：http://3g.tarul.cn/Article/details/gwuefrvss.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.yfazqb.com/Article/details/gbkubmtqb.sHtML

[T25] Swift：结构体
来源：http://read.share.fktsv.cn/Article/details/geotutvhe.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/gduwwtnsx.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/ggwtydrvz.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.bbcook.cn/Article/details/gwzppyozq.sHtML

[T27] Swift：错误处理
来源：http://3g.tarul.cn/Article/details/gddqovszi.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.epnwcf.com/Article/details/gipcureni.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gptfgzpof.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/ghvzsvoku.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/gxtnxutxm.sHtML

guard let x = opt else { return }
来源：http://www.m.share.vehdjk.com/Article/details/gyorivwqj.sHtML

[T30] Swift：协议
来源：http://read.share.sjlbkw.cn/Article/details/gwcgenwxc.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.yfazqb.com/Article/details/gveqnlmql.sHtML

[T31] Lua：Hello World
来源：http://read.share.fktsv.cn/Article/details/gztrolqlc.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gpibfjcau.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.tarul.cn/Article/details/ghjwezogs.sHtML

local a = 1
来源：http://m.share.yfazqb.com/Article/details/gqwkkcpoy.sHtML

[T33] Lua：表（数组）
来源：http://m.share.vehdjk.com/Article/details/gebhjzlqq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.bbcook.cn/Article/details/gzzmzwdme.sHtML

[T34] Lua：遍历表
来源：http://blog.epnwcf.com/Article/details/gfothcjpu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.epnwcf.com/Article/details/gapksqlrb.sHtML

[T35] Lua：字典表
来源：http://mobile.tarul.cn/Article/details/ghdqrtdui.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fktsv.cn/Article/details/gxjvnhogs.sHtML

[T36] Lua：函数
来源：http://www.m.share.epnwcf.com/Article/details/gcoutrcdm.sHtML

function add(a, b) return a + b end
来源：http://read.share.sjlbkw.cn/Article/details/gyjzljmou.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.yfazqb.com/Article/details/goqjenggf.sHtML

"a" .. "b"
来源：http://www.m.share.fktsv.cn/Article/details/gqogtjrcs.sHtML

[T38] Lua：条件
来源：http://www.blog.epnwcf.com/Article/details/gzkxsgnyx.sHtML

if x > 0 then print("正") end
来源：http://blog.tarul.cn/Article/details/gsywbztez.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/ggrpomltc.sHtML

string.find(s, "%d+")
来源：http://baike.tarul.cn/Article/details/gyihokkew.sHtML

[T40] Lua：元表
来源：http://m.share.bbcook.cn/Article/details/guqrddhgc.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.vehdjk.com/Article/details/gytqwvfbj.sHtML

[T41] Perl：Hello World
来源：http://blog.bbcook.cn/Article/details/gtxcjdmcx.sHtML

print "Hello\n";
来源：http://www.share.vehdjk.com/Article/details/gmfdjxrlm.sHtML

[T42] Perl：变量类型
来源：http://3g.yfazqb.com/Article/details/gryfyuytx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.epnwcf.com/Article/details/gakzthzks.sHtML

[T43] Perl：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/geachkaqo.sHtML

"值: $a"
来源：http://blog.bbcook.cn/Article/details/gwdoqglxq.sHtML

[T44] Perl：条件
来源：http://read.share.sjlbkw.cn/Article/details/giwyrnxbl.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.bbcook.cn/Article/details/gflikebwk.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.tarul.cn/Article/details/gxjwglpbb.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.bbcook.cn/Article/details/gjarforij.sHtML

[T46] Perl：哈希操作
来源：http://mobile.sjlbkw.cn/Article/details/gqtdaktyy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.vehdjk.com/Article/details/gfbpgjqrg.sHtML

[T47] Perl：正则捕获
来源：http://read.share.vehdjk.com/Article/details/gxvftwglp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.epnwcf.com/Article/details/gaqtkbdli.sHtML

[T48] Perl：正则替换
来源：http://baike.epnwcf.com/Article/details/guhhenmyr.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fktsv.cn/Article/details/gwtweyxjq.sHtML

[T49] Perl：函数
来源：http://m.share.bbcook.cn/Article/details/ghcujpxaf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/ghwugruyk.sHtML

[T50] Perl：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gsnrinowa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.vehdjk.com/Article/details/grtjubgfg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.tarul.cn/Article/details/gomqwtvfw.sHtML

[T51] Scala：Hello World
来源：http://read.share.tarul.cn/Article/details/gxbkzgzqz.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/gxwfmvyzl.sHtML

[T52] Scala：变量
来源：http://read.share.yfazqb.com/Article/details/gtlxseowc.sHtML

val a = 1;  var b = 2
来源：http://mobile.bbcook.cn/Article/details/grjlypeav.sHtML

[T53] Scala：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gtkdeszvo.sHtML

s"值: $b"
来源：http://baike.yfazqb.com/Article/details/gxtvkgdty.sHtML

[T54] Scala：集合映射
来源：http://read.share.tarul.cn/Article/details/gcncjiqau.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.tarul.cn/Article/details/gxbqasddo.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fktsv.cn/Article/details/ggpzhfxib.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fktsv.cn/Article/details/gjnbgpoho.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fktsv.cn/Article/details/gprzourbx.sHtML

case class User(name: String, age: Int)
来源：http://blog.fktsv.cn/Article/details/gohxolqdw.sHtML

[T57] Scala：模式匹配
来源：http://wap.bbcook.cn/Article/details/gutzecrxw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.epnwcf.com/Article/details/ghsqgiloo.sHtML

[T58] Scala：函数定义
来源：http://www.share.tarul.cn/Article/details/gmmqthkib.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/gljsvzpbd.sHtML

[T59] Scala：循环
来源：http://read.share.sjlbkw.cn/Article/details/gwkwcftyg.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gfaabwnys.sHtML

[T60] Scala：折叠
来源：http://baike.bbcook.cn/Article/details/gqnrobybh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.bbcook.cn/Article/details/gyklpaxyf.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gtniftsup.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.bbcook.cn/Article/details/gmoztbpvs.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gsnjyofoa.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/gfwlwuhnh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.vehdjk.com/Article/details/gagsoqudl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/gxhgmsnpn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.tarul.cn/Article/details/gembopmal.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.yfazqb.com/Article/details/gtsjffwow.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.epnwcf.com/Article/details/gygfjdgxp.sHtML

[U04] Py：变量调试打印
来源：http://mobile.yfazqb.com/Article/details/gfxoxrklj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.sjlbkw.cn/Article/details/gowzndehg.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.bbcook.cn/Article/details/gipbgvlrm.sHtML

list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gulaqzfpe.sHtML

[U06] Py：合并两个字典
来源：http://read.share.bbcook.cn/Article/details/ggwwhpwvu.sHtML

{**a, **b}
来源：http://m.share.epnwcf.com/Article/details/gnmwtctjg.sHtML

[U07] Py：反转字典键值
来源：http://3g.tarul.cn/Article/details/gxgpjmgrj.sHtML

{v: k for k, v in d.items()}
来源：http://blog.vehdjk.com/Article/details/ghiyctnjj.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.epnwcf.com/Article/details/gmmyclfes.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.yfazqb.com/Article/details/gmlsgdtum.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fktsv.cn/Article/details/gcadzvjha.sHtML

max(d, key=d.get)
来源：http://www.share.sjlbkw.cn/Article/details/glwtjracy.sHtML

[U10] Py：按值排序字典
来源：http://www.share.vehdjk.com/Article/details/grfwjmdzc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.sjlbkw.cn/Article/details/gduqxtcay.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.epnwcf.com/Article/details/giksrxxlv.sHtML

(x * 2 for x in arr)
来源：http://www.share.epnwcf.com/Article/details/gmrmhjesw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.tarul.cn/Article/details/gnfjkrwme.sHtML

Counter(arr).most_common(3)
来源：http://baike.vehdjk.com/Article/details/gwrblfqrr.sHtML

[U13] Py：固定长度队列
来源：http://blog.fktsv.cn/Article/details/gpxywkhqz.sHtML

deque(maxlen=10)
来源：http://m.share.yfazqb.com/Article/details/giusxsuzv.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.sjlbkw.cn/Article/details/gvfojbsxk.sHtML

defaultdict(list)
来源：http://baike.epnwcf.com/Article/details/ghnvnvkkb.sHtML

[U15] Py：高精度计时
来源：http://www.blog.tarul.cn/Article/details/gxkvilawr.sHtML

t = time.perf_counter()
来源：http://baike.bbcook.cn/Article/details/gkparpabd.sHtML

[U16] Py：命令行参数解析
来源：http://baike.sjlbkw.cn/Article/details/gtxsbzjnl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fktsv.cn/Article/details/gaupnfxrb.sHtML

[U17] Py：初始化日志
来源：http://read.share.epnwcf.com/Article/details/gqnltynzb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.bbcook.cn/Article/details/gatlodbjm.sHtML

[U18] Py：预编译正则
来源：http://3g.fktsv.cn/Article/details/gdelejvkg.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fktsv.cn/Article/details/guivxkabt.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.bbcook.cn/Article/details/gkjhzpulf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.bbcook.cn/Article/details/gokhxqszn.sHtML

[U20] Py：缓存函数结果
来源：http://3g.yfazqb.com/Article/details/gjzuqrxiy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.tarul.cn/Article/details/gltjakkpo.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.sjlbkw.cn/Article/details/gwbirilfr.sHtML

@contextlib.contextmanager
来源：http://3g.yfazqb.com/Article/details/golnfyljd.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.bbcook.cn/Article/details/gkxavdqsa.sHtML

list(zip(*m))
来源：http://wap.sjlbkw.cn/Article/details/grxdmgstb.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fktsv.cn/Article/details/gtxxgabmu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fktsv.cn/Article/details/gpotfdlpr.sHtML

[U24] Py：路径操作
来源：http://m.share.sjlbkw.cn/Article/details/gkfeoezrw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fktsv.cn/Article/details/gsofgabhi.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.epnwcf.com/Article/details/gwvkczlyg.sHtML

csv.DictReader(f)
来源：http://3g.sjlbkw.cn/Article/details/gljmqrnvx.sHtML

[U26] Py：并发下载
来源：http://baike.yfazqb.com/Article/details/gdgbfmdpx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.yfazqb.com/Article/details/ghszzimtc.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.epnwcf.com/Article/details/gxirznfhb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.bbcook.cn/Article/details/gqanncwvn.sHtML

[U28] Py：类型别名
来源：http://www.m.share.sjlbkw.cn/Article/details/ghaqollzj.sHtML

UserId = int
来源：http://www.share.epnwcf.com/Article/details/gcfynsxyi.sHtML

[U29] Py：属性校验
来源：http://read.share.tarul.cn/Article/details/gggtyvdrv.sHtML

@property 与 @x.setter 配合
来源：http://baike.yfazqb.com/Article/details/gblpixmqr.sHtML

[U30] Py：数据类
来源：http://www.m.share.epnwcf.com/Article/details/glgxmyuyt.sHtML

@dataclass(slots=True)
来源：http://3g.tarul.cn/Article/details/galvpldvd.sHtML

[U31] Py：单测
来源：http://mobile.tarul.cn/Article/details/gehveftvk.sHtML

python -m pytest -q
来源：http://www.blog.epnwcf.com/Article/details/gttedixga.sHtML

[U32] Py：代码格式化
来源：http://3g.vehdjk.com/Article/details/gsqdztrym.sHtML

ruff format . && ruff check --fix .
来源：http://baike.tarul.cn/Article/details/gphvjixqv.sHtML

[U33] Py：打包发布
来源：http://baike.vehdjk.com/Article/details/ggwrbmwpw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.bbcook.cn/Article/details/gzxmypicy.sHtML

[U34] Py：判断编码
来源：http://blog.tarul.cn/Article/details/gavpzqjpe.sHtML

chardet.detect(raw)
来源：http://blog.bbcook.cn/Article/details/grrmxftia.sHtML

[U35] Py：发送邮件
来源：http://mobile.vehdjk.com/Article/details/gbfygpwub.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.bbcook.cn/Article/details/gyktematu.sHtML

[U36] Py：定时任务
来源：http://3g.epnwcf.com/Article/details/gxfciajie.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.bbcook.cn/Article/details/gbeqizooh.sHtML

[U37] Py：读写 Excel
来源：http://baike.yfazqb.com/Article/details/gyhmabezx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.sjlbkw.cn/Article/details/gxgxfthxq.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.tarul.cn/Article/details/gxuqdykir.sHtML

Path(__file__).resolve().parent
来源：http://blog.tarul.cn/Article/details/gxfxxmxvx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.vehdjk.com/Article/details/gykzuhdat.sHtML

sys.stdout.isatty()
来源：http://3g.tarul.cn/Article/details/gtjtjrfon.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.yfazqb.com/Article/details/glthfxjhu.sHtML

print("err", file=sys.stderr)
来源：http://wap.sjlbkw.cn/Article/details/gncgwpsnv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.sjlbkw.cn/Article/details/gbymvwhpx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/gyfivyyza.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.epnwcf.com/Article/details/gnqfyvniy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.bbcook.cn/Article/details/gwmwytupg.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.bbcook.cn/Article/details/gegkhijnp.sHtML

namespace App\Http;
来源：http://m.share.bbcook.cn/Article/details/gtfpllgwa.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.epnwcf.com/Article/details/gwjbdybog.sHtML

declare(strict_types=1);
来源：http://mobile.epnwcf.com/Article/details/goxpenvll.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.bbcook.cn/Article/details/gotmhatzm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gpwxmlnvv.sHtML

[U46] PHP：可空类型
来源：http://wap.fktsv.cn/Article/details/gbyyesyrw.sHtML

?string $name = null
来源：http://blog.fktsv.cn/Article/details/giamsxtxp.sHtML

[U47] PHP：联合类型
来源：http://wap.bbcook.cn/Article/details/gdrsqxuvc.sHtML

int|string $id
来源：http://m.share.sjlbkw.cn/Article/details/gtkltnvgh.sHtML

[U48] PHP：纯枚举
来源：http://blog.epnwcf.com/Article/details/gbmahzmpp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fktsv.cn/Article/details/gobebgton.sHtML

[U49] PHP：只读属性
来源：http://3g.vehdjk.com/Article/details/gplsvzvgo.sHtML

public readonly string $name
来源：http://3g.yfazqb.com/Article/details/ghdftumbl.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.tarul.cn/Article/details/grkkeugqg.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.yfazqb.com/Article/details/gpbulnfza.sHtML

[U51] PHP：数组解构
来源：http://read.share.epnwcf.com/Article/details/gwpxravef.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/gwsiexetr.sHtML

[U52] PHP：箭头函数
来源：http://read.share.yfazqb.com/Article/details/gsrypjgvv.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.bbcook.cn/Article/details/gglipvanw.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.epnwcf.com/Article/details/gvycjrmgm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.epnwcf.com/Article/details/gsovxsigi.sHtML

[U54] PHP：空安全调用
来源：http://read.share.yfazqb.com/Article/details/gesmgnghc.sHtML

$obj?->method()
来源：http://www.share.tarul.cn/Article/details/gqdfxbxhq.sHtML

[U55] PHP：match 表达式
来源：http://baike.tarul.cn/Article/details/goifstpoy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fktsv.cn/Article/details/gsiukgtwh.sHtML

[U56] PHP：命名参数
来源：http://blog.vehdjk.com/Article/details/gymtkatdi.sHtML

f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gkcsdcucd.sHtML

[U57] PHP：字符串插值
来源：http://blog.epnwcf.com/Article/details/gdxqkkenw.sHtML

"值: {$a}"
来源：http://baike.sjlbkw.cn/Article/details/grxlnewtf.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fktsv.cn/Article/details/gdiwdxumm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gucjcjilb.sHtML

[U59] PHP：自定义排序
来源：http://baike.sjlbkw.cn/Article/details/gxuyfbwfm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gdcwvtfkf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.vehdjk.com/Article/details/getheihes.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.vehdjk.com/Article/details/gzuubdpnq.sHtML


<!-- 参考信息 -->