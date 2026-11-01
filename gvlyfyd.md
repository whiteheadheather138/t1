代发 wailian999

[S37] C++：set
来源：http://www.blog.epnwcf.com/Article/details/gzxqlehnc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.epnwcf.com/Article/details/gupsoukla.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/goubjslsk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gswmjcsca.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/gonskmonb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.bbcook.cn/Article/details/gsokpnkkq.sHtML

[S40] C++：查找元素
来源：http://wap.sjlbkw.cn/Article/details/gkzmejfba.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/gyoapklnf.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gssmanqbu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.yfazqb.com/Article/details/goshokbte.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fktsv.cn/Article/details/gbyopijvw.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.sjlbkw.cn/Article/details/guhtiepod.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/ginjhgkox.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fktsv.cn/Article/details/gbdnltqwt.sHtML

[S44] C++：引用传参
来源：http://m.share.sjlbkw.cn/Article/details/gwtpelmuu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.vehdjk.com/Article/details/githmjqco.sHtML

[S45] C++：lambda
来源：http://www.share.bbcook.cn/Article/details/gkuqmxcap.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.bbcook.cn/Article/details/gylzzxuxw.sHtML

[S46] C++：函数模板
来源：http://blog.fktsv.cn/Article/details/gfcbjwpsc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.epnwcf.com/Article/details/geslqvcxf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.epnwcf.com/Article/details/gldymyakl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/genjomqph.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gfnjdlycw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.epnwcf.com/Article/details/ghwojnmzz.sHtML

while (std::getline(in, line)) { }
来源：http://3g.tarul.cn/Article/details/gocbxobid.sHtML

[S49] C++：写文件
来源：http://mobile.epnwcf.com/Article/details/gawxhnspl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.yfazqb.com/Article/details/gvypblqnp.sHtML

[S50] C++：格式化数字
来源：http://wap.vehdjk.com/Article/details/gvhwabeav.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gbqenvmrm.sHtML

[S51] C++：显式类型转换
来源：http://read.share.yfazqb.com/Article/details/gynylduns.sHtML

static_cast<double>(a) / b
来源：http://mobile.yfazqb.com/Article/details/gfntakkpi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.yfazqb.com/Article/details/gxvyjmmrl.sHtML

int size() const noexcept { return n_; }
来源：http://3g.sjlbkw.cn/Article/details/gnbktogyl.sHtML

[S53] C++：移动语义
来源：http://3g.sjlbkw.cn/Article/details/grrhfpqop.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.tarul.cn/Article/details/ghgwwqjay.sHtML

[S54] C++：异常处理
来源：http://blog.fktsv.cn/Article/details/grxyjgvju.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.tarul.cn/Article/details/gfjxsdhiv.sHtML

[S55] C++：结构化绑定
来源：http://wap.epnwcf.com/Article/details/gddplmzww.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/gpyfgcyzw.sHtML

[S56] C++：optional
来源：http://read.share.bbcook.cn/Article/details/gncasikvg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.epnwcf.com/Article/details/gtwuubouf.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fktsv.cn/Article/details/gcdrwivys.sHtML

constexpr int N = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gqybdnwgh.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gpfqqfcrn.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.tarul.cn/Article/details/gynljuobm.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gfjwohlzr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.yfazqb.com/Article/details/gefazdcbh.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.yfazqb.com/Article/details/gwbcshgwj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.yfazqb.com/Article/details/gyfvqcieu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmnuqkoop.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gazrhlsve.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gvblfavct.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fktsv.cn/Article/details/geldttwfa.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/grhvwprto.sHtML

[T02] Kotlin：变量
来源：http://baike.tarul.cn/Article/details/gfvmzvpsw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fktsv.cn/Article/details/gdluomyrr.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.sjlbkw.cn/Article/details/gwwicamxv.sHtML

"值: $b"
来源：http://3g.epnwcf.com/Article/details/glkphhdcc.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.bbcook.cn/Article/details/gcglwdtec.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fktsv.cn/Article/details/gitdmmqzn.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fktsv.cn/Article/details/gflbpykia.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fktsv.cn/Article/details/gcmyiqmnl.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/guouatpuh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/ghrizshck.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.yfazqb.com/Article/details/gnfbjdtid.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.tarul.cn/Article/details/gnokibhxr.sHtML

[T08] Kotlin：数据类
来源：http://www.share.tarul.cn/Article/details/gwlhjblmc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/gxlggofyl.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/gkxuxhtvc.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.yfazqb.com/Article/details/gphhoowsu.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.epnwcf.com/Article/details/gdrcypqgn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/gatlvqvyd.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fktsv.cn/Article/details/gynimkesv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.epnwcf.com/Article/details/gnggvvodd.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.yfazqb.com/Article/details/gmwtnjceh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gcclvhmiu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fktsv.cn/Article/details/gkgcbqnig.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.vehdjk.com/Article/details/ggzyzmwcw.sHtML

[T14] Kotlin：循环
来源：http://wap.tarul.cn/Article/details/ghnfxnsgg.sHtML

for (i in 1..10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gooxcztkw.sHtML

[T15] Kotlin：接口
来源：http://read.share.fktsv.cn/Article/details/gwmclatok.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.bbcook.cn/Article/details/giteiaian.sHtML

[T16] Swift：Hello World
来源：http://3g.yfazqb.com/Article/details/godihtzdq.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gamzwsejb.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.sjlbkw.cn/Article/details/gfswxxkeo.sHtML

var a = 1;  let b = 2
来源：http://m.share.tarul.cn/Article/details/gssfyizny.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/gkfoksmhu.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/grndjhnnb.sHtML

[T19] Swift：可选绑定
来源：http://www.share.tarul.cn/Article/details/glghhtvdn.sHtML

if let n = opt { print(n) }
来源：http://3g.sjlbkw.cn/Article/details/gfnlhialb.sHtML

[T20] Swift：数组操作
来源：http://www.blog.vehdjk.com/Article/details/gzfqhzawj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.sjlbkw.cn/Article/details/glwigvisu.sHtML

[T21] Swift：遍历
来源：http://www.share.fktsv.cn/Article/details/gyvfpwlvc.sHtML

for x in a { print(x) }
来源：http://read.share.epnwcf.com/Article/details/gzwinefox.sHtML

[T22] Swift：字典
来源：http://www.m.share.bbcook.cn/Article/details/gmnuxujcs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgemwvvw.sHtML

[T23] Swift：函数
来源：http://mobile.vehdjk.com/Article/details/ginexhcuo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.sjlbkw.cn/Article/details/gpsnqvtkz.sHtML

[T24] Swift：闭包
来源：http://baike.sjlbkw.cn/Article/details/gfjmyhjmf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.bbcook.cn/Article/details/glgogbald.sHtML

[T25] Swift：结构体
来源：http://baike.vehdjk.com/Article/details/glfpbvhvi.sHtML

struct P { var x: Int }
来源：http://www.blog.sjlbkw.cn/Article/details/gcipjsdyx.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fktsv.cn/Article/details/gibtxlacy.sHtML

class A: Base { override func f() {} }
来源：http://read.share.vehdjk.com/Article/details/giivpdqjy.sHtML

[T27] Swift：错误处理
来源：http://3g.epnwcf.com/Article/details/gbtuasnej.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.vehdjk.com/Article/details/gdinwpdth.sHtML

[T28] Swift：枚举
来源：http://baike.fktsv.cn/Article/details/gjbksemxa.sHtML

enum Color { case red, green }
来源：http://www.blog.sjlbkw.cn/Article/details/gezrlpxml.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.epnwcf.com/Article/details/gkvjacshm.sHtML

guard let x = opt else { return }
来源：http://read.share.tarul.cn/Article/details/gsvovkskd.sHtML

[T30] Swift：协议
来源：http://baike.tarul.cn/Article/details/gqjqykkjt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.epnwcf.com/Article/details/grlvfqwtx.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gwzmbjcfd.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gleevlsmx.sHtML

[T32] Lua：局部变量
来源：http://read.share.tarul.cn/Article/details/gffqsotaf.sHtML

local a = 1
来源：http://www.blog.bbcook.cn/Article/details/gmgksrqew.sHtML

[T33] Lua：表（数组）
来源：http://3g.sjlbkw.cn/Article/details/glhcdswsz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.sjlbkw.cn/Article/details/gzkfsrwqj.sHtML

[T34] Lua：遍历表
来源：http://baike.bbcook.cn/Article/details/guxrknewi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.epnwcf.com/Article/details/gebjygiea.sHtML

[T35] Lua：字典表
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfqpmhuz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fktsv.cn/Article/details/giqyhhcud.sHtML

[T36] Lua：函数
来源：http://www.blog.yfazqb.com/Article/details/glqpuauzq.sHtML

function add(a, b) return a + b end
来源：http://wap.epnwcf.com/Article/details/gznozrquv.sHtML

[T37] Lua：字符串拼接
来源：http://3g.epnwcf.com/Article/details/gfhizjqmc.sHtML

"a" .. "b"
来源：http://www.share.sjlbkw.cn/Article/details/golidvnxi.sHtML

[T38] Lua：条件
来源：http://3g.yfazqb.com/Article/details/glveuonrg.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.sjlbkw.cn/Article/details/gantudgbv.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.tarul.cn/Article/details/glqkpnubc.sHtML

string.find(s, "%d+")
来源：http://baike.vehdjk.com/Article/details/gmarmsigx.sHtML

[T40] Lua：元表
来源：http://mobile.fktsv.cn/Article/details/ggkfdccga.sHtML

setmetatable({}, { __index = base })
来源：http://blog.epnwcf.com/Article/details/gmmtnjatb.sHtML

[T41] Perl：Hello World
来源：http://baike.yfazqb.com/Article/details/ghglilvbx.sHtML

print "Hello\n";
来源：http://wap.bbcook.cn/Article/details/gyvvoczfr.sHtML

[T42] Perl：变量类型
来源：http://read.share.vehdjk.com/Article/details/gpgwtiwpu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.bbcook.cn/Article/details/gosgwcxzl.sHtML

[T43] Perl：字符串插值
来源：http://3g.tarul.cn/Article/details/guhxfzfmi.sHtML

"值: $a"
来源：http://www.blog.tarul.cn/Article/details/gvdpejyna.sHtML

[T44] Perl：条件
来源：http://wap.vehdjk.com/Article/details/gazubsdod.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.epnwcf.com/Article/details/gehelnlmh.sHtML

[T45] Perl：数组遍历
来源：http://wap.tarul.cn/Article/details/glfxibpyy.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.bbcook.cn/Article/details/geyptuzsv.sHtML

[T46] Perl：哈希操作
来源：http://blog.fktsv.cn/Article/details/gmlepqaqr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fktsv.cn/Article/details/gyapntful.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.vehdjk.com/Article/details/gvlocpkrc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.tarul.cn/Article/details/gnhkyfnso.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gcryxryps.sHtML

$s =~ s/old/new/g;
来源：http://3g.sjlbkw.cn/Article/details/gwngtxhde.sHtML

[T49] Perl：函数
来源：http://3g.epnwcf.com/Article/details/gdnhkmwwi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gsuumpdgq.sHtML

[T50] Perl：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gyyeeybfo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.epnwcf.com/Article/details/grbayslus.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.yfazqb.com/Article/details/gvtrorxhe.sHtML

[T51] Scala：Hello World
来源：http://blog.fktsv.cn/Article/details/gqvvwfokz.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gzjpobrnx.sHtML

[T52] Scala：变量
来源：http://www.share.epnwcf.com/Article/details/gwgkljorr.sHtML

val a = 1;  var b = 2
来源：http://baike.bbcook.cn/Article/details/gtqbrmiix.sHtML

[T53] Scala：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/ghxhtopmp.sHtML

s"值: $b"
来源：http://3g.bbcook.cn/Article/details/gwnwcrzba.sHtML

[T54] Scala：集合映射
来源：http://read.share.yfazqb.com/Article/details/gaajuidhu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fktsv.cn/Article/details/gkjwnmbvm.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/gcgbkedov.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.tarul.cn/Article/details/gppwaeqmi.sHtML

[T56] Scala：样例类
来源：http://baike.vehdjk.com/Article/details/gsrjuanbr.sHtML

case class User(name: String, age: Int)
来源：http://3g.fktsv.cn/Article/details/gcepdupxt.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.tarul.cn/Article/details/gmcbnipuz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.vehdjk.com/Article/details/gjkpqydfv.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.tarul.cn/Article/details/gpornbwde.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.epnwcf.com/Article/details/gmugliael.sHtML

[T59] Scala：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gfcffaksd.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/ghfsedbqp.sHtML

[T60] Scala：折叠
来源：http://www.share.tarul.cn/Article/details/ghdczqawo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.epnwcf.com/Article/details/gujatwdtn.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gffjqbcjx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.epnwcf.com/Article/details/grdjbiroy.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gsysyjuta.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/gsfeulyjo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.epnwcf.com/Article/details/gfzooeisy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.vehdjk.com/Article/details/gmifyrqzw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.bbcook.cn/Article/details/gfsettwgu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.bbcook.cn/Article/details/gjhnzjoyu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.yfazqb.com/Article/details/gixotltpe.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcasnklt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fktsv.cn/Article/details/gkguexvfp.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.vehdjk.com/Article/details/gugruflic.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gqdubwlbj.sHtML

[U06] Py：合并两个字典
来源：http://3g.fktsv.cn/Article/details/gyflhmcgo.sHtML

{**a, **b}
来源：http://www.blog.vehdjk.com/Article/details/gpsulgjcb.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fktsv.cn/Article/details/gdyeywidh.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fktsv.cn/Article/details/grokeefgq.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.tarul.cn/Article/details/gutpzcnad.sHtML

[y for x in nested for y in x]
来源：http://mobile.vehdjk.com/Article/details/gvyrddudq.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fktsv.cn/Article/details/glndpdigb.sHtML

max(d, key=d.get)
来源：http://m.share.sjlbkw.cn/Article/details/gwnxoufmk.sHtML

[U10] Py：按值排序字典
来源：http://read.share.tarul.cn/Article/details/gvkuhxpau.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fktsv.cn/Article/details/gozejkajd.sHtML

[U11] Py：生成器表达式
来源：http://read.share.yfazqb.com/Article/details/gvboybssu.sHtML

(x * 2 for x in arr)
来源：http://www.blog.yfazqb.com/Article/details/gqmmdsnwc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.yfazqb.com/Article/details/gynecumzd.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.yfazqb.com/Article/details/gtxizufgv.sHtML

[U13] Py：固定长度队列
来源：http://mobile.vehdjk.com/Article/details/gxhpldhel.sHtML

deque(maxlen=10)
来源：http://3g.sjlbkw.cn/Article/details/gonkmxhhn.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fktsv.cn/Article/details/gijpnivrc.sHtML

defaultdict(list)
来源：http://baike.yfazqb.com/Article/details/grfiysodw.sHtML

[U15] Py：高精度计时
来源：http://wap.epnwcf.com/Article/details/guglcmxmt.sHtML

t = time.perf_counter()
来源：http://mobile.bbcook.cn/Article/details/gghmcxonj.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fktsv.cn/Article/details/gjcspaugu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.bbcook.cn/Article/details/gsyirthqs.sHtML

[U17] Py：初始化日志
来源：http://m.share.sjlbkw.cn/Article/details/ghztsusmw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fktsv.cn/Article/details/gtovqthnu.sHtML

[U18] Py：预编译正则
来源：http://m.share.tarul.cn/Article/details/gwprosmvu.sHtML

pat = re.compile(r"\d+")
来源：http://baike.sjlbkw.cn/Article/details/goyryects.sHtML

[U19] Py：正则替换带回调
来源：http://wap.epnwcf.com/Article/details/gyvtqzmed.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fktsv.cn/Article/details/gjmhfsiqh.sHtML

[U20] Py：缓存函数结果
来源：http://baike.epnwcf.com/Article/details/giswxhzva.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.yfazqb.com/Article/details/gkvskrfkb.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.epnwcf.com/Article/details/gluxtfjbb.sHtML

@contextlib.contextmanager
来源：http://wap.yfazqb.com/Article/details/ghocxnmhd.sHtML

[U22] Py：矩阵转置
来源：http://mobile.yfazqb.com/Article/details/gospavjku.sHtML

list(zip(*m))
来源：http://read.share.yfazqb.com/Article/details/goonvxnxt.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.yfazqb.com/Article/details/ggrsmetjc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.sjlbkw.cn/Article/details/gjadfmeus.sHtML

[U24] Py：路径操作
来源：http://blog.sjlbkw.cn/Article/details/gqypbhmqm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/gcdisrnry.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/gcfcphquw.sHtML

csv.DictReader(f)
来源：http://wap.tarul.cn/Article/details/gjwtrxhbq.sHtML

[U26] Py：并发下载
来源：http://www.blog.yfazqb.com/Article/details/gxcffddot.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.epnwcf.com/Article/details/gwfctzfqr.sHtML

[U27] Py：异步 HTTP
来源：http://wap.yfazqb.com/Article/details/gdsndbzpo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.sjlbkw.cn/Article/details/ggkjuagjh.sHtML

[U28] Py：类型别名
来源：http://read.share.sjlbkw.cn/Article/details/gokswzhtl.sHtML

UserId = int
来源：http://blog.epnwcf.com/Article/details/gybvsnvje.sHtML

[U29] Py：属性校验
来源：http://m.share.fktsv.cn/Article/details/gijqjxurb.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.yfazqb.com/Article/details/gkzzgbvcx.sHtML

[U30] Py：数据类
来源：http://mobile.tarul.cn/Article/details/gykehewog.sHtML

@dataclass(slots=True)
来源：http://www.blog.bbcook.cn/Article/details/gesxekxzh.sHtML

[U31] Py：单测
来源：http://wap.sjlbkw.cn/Article/details/gnpvmmksz.sHtML

python -m pytest -q
来源：http://wap.vehdjk.com/Article/details/gyekrvjyr.sHtML

[U32] Py：代码格式化
来源：http://mobile.yfazqb.com/Article/details/gddyzkbga.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.epnwcf.com/Article/details/gwatbzjdj.sHtML

[U33] Py：打包发布
来源：http://m.share.bbcook.cn/Article/details/gfajqfnir.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.bbcook.cn/Article/details/gfwlynvdn.sHtML

[U34] Py：判断编码
来源：http://wap.fktsv.cn/Article/details/gfvtkbbdl.sHtML

chardet.detect(raw)
来源：http://read.share.vehdjk.com/Article/details/gswkhzyzj.sHtML

[U35] Py：发送邮件
来源：http://mobile.vehdjk.com/Article/details/gwyucterl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.sjlbkw.cn/Article/details/gjfhiotam.sHtML

[U36] Py：定时任务
来源：http://3g.fktsv.cn/Article/details/goyycsazt.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.vehdjk.com/Article/details/gqtibpzfa.sHtML

[U37] Py：读写 Excel
来源：http://baike.sjlbkw.cn/Article/details/gouldcuwz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.epnwcf.com/Article/details/gsncmnwte.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.bbcook.cn/Article/details/geedafnnd.sHtML

Path(__file__).resolve().parent
来源：http://mobile.sjlbkw.cn/Article/details/gnxobayak.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.yfazqb.com/Article/details/gfkjmwnyg.sHtML

sys.stdout.isatty()
来源：http://www.blog.fktsv.cn/Article/details/gnwfpyceu.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.tarul.cn/Article/details/garlnhvrc.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gugzmhcuw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.epnwcf.com/Article/details/gawmxsuzh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.bbcook.cn/Article/details/gpsohpmhb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.vehdjk.com/Article/details/gdmapidit.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.bbcook.cn/Article/details/gtkqgdhlp.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.vehdjk.com/Article/details/gezwnlvhb.sHtML

namespace App\Http;
来源：http://m.share.tarul.cn/Article/details/gfbtgonpa.sHtML

[U44] PHP：开启严格类型
来源：http://baike.sjlbkw.cn/Article/details/guisjzloi.sHtML

declare(strict_types=1);
来源：http://3g.fktsv.cn/Article/details/ghvcamxjg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.bbcook.cn/Article/details/gzhesfxvj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/ghbmzqkap.sHtML

[U46] PHP：可空类型
来源：http://wap.tarul.cn/Article/details/gmbgnvmvu.sHtML

?string $name = null
来源：http://www.share.bbcook.cn/Article/details/gcvygavnm.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.yfazqb.com/Article/details/gmtyzljyj.sHtML

int|string $id
来源：http://read.share.fktsv.cn/Article/details/glfhtwxge.sHtML

[U48] PHP：纯枚举
来源：http://m.share.epnwcf.com/Article/details/gingjfnmi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.bbcook.cn/Article/details/gbtlxebam.sHtML

[U49] PHP：只读属性
来源：http://baike.yfazqb.com/Article/details/gudvfcesf.sHtML

public readonly string $name
来源：http://read.share.tarul.cn/Article/details/gbfpveyfa.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.sjlbkw.cn/Article/details/gzppmcgif.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwyecigxs.sHtML

[U51] PHP：数组解构
来源：http://www.share.vehdjk.com/Article/details/gpocyhuxg.sHtML

[$a, $b] = $arr;
来源：http://baike.fktsv.cn/Article/details/gtdjknmeq.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gbishmmpr.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.bbcook.cn/Article/details/gcaajammi.sHtML

[U53] PHP：空合并运算符
来源：http://blog.epnwcf.com/Article/details/gmdzcaepy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.tarul.cn/Article/details/grbguvpcq.sHtML

[U54] PHP：空安全调用
来源：http://baike.sjlbkw.cn/Article/details/gavjyqfxx.sHtML

$obj?->method()
来源：http://www.m.share.epnwcf.com/Article/details/gtdktdbrl.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.epnwcf.com/Article/details/glfdwpprr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.bbcook.cn/Article/details/giefehqhd.sHtML

[U56] PHP：命名参数
来源：http://mobile.sjlbkw.cn/Article/details/gndhfhdjn.sHtML

f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/grqbtkmtm.sHtML

[U57] PHP：字符串插值
来源：http://blog.fktsv.cn/Article/details/gzuzbrzso.sHtML

"值: {$a}"
来源：http://www.share.tarul.cn/Article/details/gpftvofkg.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.tarul.cn/Article/details/gvoaieeez.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.yfazqb.com/Article/details/genjpgvyl.sHtML

[U59] PHP：自定义排序
来源：http://mobile.vehdjk.com/Article/details/ggxljrymf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.bbcook.cn/Article/details/gdiwyxoaw.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.bbcook.cn/Article/details/gtthbpnbi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fktsv.cn/Article/details/gecogcisr.sHtML

[U61] PHP：正则
来源：http://www.blog.fktsv.cn/Article/details/gfyenoitz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gpwlwtmwa.sHtML

[U62] PHP：日期对象
来源：http://m.share.bbcook.cn/Article/details/gwzuwohpp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.vehdjk.com/Article/details/gdgzgjnfq.sHtML


<!-- 参考信息 -->