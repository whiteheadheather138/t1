代发 wailian999

[S41] C++：类与构造函数
来源：http://www.blog.bbcook.cn/Article/details/gvdmjysrt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.epnwcf.com/Article/details/gxwdlndua.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gcfdpgbbz.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fktsv.cn/Article/details/gganhbdnr.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/ghyncocqf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.sjlbkw.cn/Article/details/gkglnewxp.sHtML

[S44] C++：引用传参
来源：http://www.blog.epnwcf.com/Article/details/gwxqylohh.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.yfazqb.com/Article/details/gmpeiqxhn.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/gnypqrsiv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.vehdjk.com/Article/details/grgyocjrj.sHtML

[S46] C++：函数模板
来源：http://www.share.vehdjk.com/Article/details/gizhrgfdb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.vehdjk.com/Article/details/goxzqtgza.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.epnwcf.com/Article/details/gsritvgpe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.tarul.cn/Article/details/gqcojdulz.sHtML

[S48] C++：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gefyhhapg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fktsv.cn/Article/details/gniyokbgg.sHtML

while (std::getline(in, line)) { }
来源：http://baike.bbcook.cn/Article/details/gyxnuetzy.sHtML

[S49] C++：写文件
来源：http://mobile.yfazqb.com/Article/details/gwvxjpqyw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.epnwcf.com/Article/details/gjpgoazjh.sHtML

[S50] C++：格式化数字
来源：http://3g.sjlbkw.cn/Article/details/gseebepra.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gbdyigjhm.sHtML

[S51] C++：显式类型转换
来源：http://mobile.vehdjk.com/Article/details/gmbvawakl.sHtML

static_cast<double>(a) / b
来源：http://baike.tarul.cn/Article/details/gvyigihey.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.yfazqb.com/Article/details/gnmfwaduv.sHtML

int size() const noexcept { return n_; }
来源：http://3g.sjlbkw.cn/Article/details/ghishlmpd.sHtML

[S53] C++：移动语义
来源：http://www.m.share.epnwcf.com/Article/details/gndlhzuvr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.bbcook.cn/Article/details/gjmvntxhb.sHtML

[S54] C++：异常处理
来源：http://www.m.share.yfazqb.com/Article/details/gjgyekfty.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/grgrglnjx.sHtML

[S55] C++：结构化绑定
来源：http://blog.bbcook.cn/Article/details/gqmalmtea.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdjpwaul.sHtML

[S56] C++：optional
来源：http://www.share.sjlbkw.cn/Article/details/ggbporkpb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.vehdjk.com/Article/details/gvbuwvyxv.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gfrivcrjb.sHtML

constexpr int N = 10;
来源：http://www.share.epnwcf.com/Article/details/gvmwwvapb.sHtML

[S58] C++：命名空间
来源：http://wap.sjlbkw.cn/Article/details/ggnjrvlmp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.epnwcf.com/Article/details/guknspvyy.sHtML

[S59] C++：静态断言
来源：http://www.blog.sjlbkw.cn/Article/details/gxfokruno.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/grlzppfvh.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.sjlbkw.cn/Article/details/gsxyqaqmy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.epnwcf.com/Article/details/grkajizlq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gojcbqngy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/gwjddxrze.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqxkkrknj.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/geqpojuhz.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/grvfickvz.sHtML

[T02] Kotlin：变量
来源：http://read.share.sjlbkw.cn/Article/details/gpoqdtjqr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/guaijiorj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/gjdcjouxn.sHtML

"值: $b"
来源：http://3g.bbcook.cn/Article/details/gtvuicpws.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fktsv.cn/Article/details/ghuvkpnmo.sHtML

val n: String? = null;  n?.length
来源：http://baike.sjlbkw.cn/Article/details/gicbvkfxb.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/gkcnpqjlo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.sjlbkw.cn/Article/details/gzwgiaiao.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.tarul.cn/Article/details/gclzebwtp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.yfazqb.com/Article/details/glrfcewvo.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.bbcook.cn/Article/details/gimxqflpp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.bbcook.cn/Article/details/gwubzdgix.sHtML

[T08] Kotlin：数据类
来源：http://blog.tarul.cn/Article/details/gxfjgjbxj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gnqvpicdr.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.tarul.cn/Article/details/gsgknfiyo.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.tarul.cn/Article/details/gtusbaeez.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.bbcook.cn/Article/details/ghtyqoimg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.tarul.cn/Article/details/gkxjtajuw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.bbcook.cn/Article/details/guncoopgq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/gqguweuvm.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/gqkavacrx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.tarul.cn/Article/details/gqhcnfrwb.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/gungwzrtn.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.vehdjk.com/Article/details/glsikmjdl.sHtML

[T14] Kotlin：循环
来源：http://www.share.epnwcf.com/Article/details/gamovsrim.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/ghibcevms.sHtML

[T15] Kotlin：接口
来源：http://www.blog.tarul.cn/Article/details/gcdcuxafo.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.yfazqb.com/Article/details/gxhsbdhnw.sHtML

[T16] Swift：Hello World
来源：http://m.share.bbcook.cn/Article/details/gooynnofc.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/gytzqxvow.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.epnwcf.com/Article/details/gvwxwkwlr.sHtML

var a = 1;  let b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gdwbjaxpa.sHtML

[T18] Swift：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gdrsvrhxs.sHtML

"值: \(b)"
来源：http://www.m.share.tarul.cn/Article/details/gbqmqjacy.sHtML

[T19] Swift：可选绑定
来源：http://baike.vehdjk.com/Article/details/gqfbiswco.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/gmvopdbps.sHtML

[T20] Swift：数组操作
来源：http://www.blog.yfazqb.com/Article/details/gktdpjrcm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.tarul.cn/Article/details/ggljysuhi.sHtML

[T21] Swift：遍历
来源：http://read.share.yfazqb.com/Article/details/gfgqguoaa.sHtML

for x in a { print(x) }
来源：http://blog.fktsv.cn/Article/details/ghmxeqtmb.sHtML

[T22] Swift：字典
来源：http://www.blog.sjlbkw.cn/Article/details/gkldbzrpw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.bbcook.cn/Article/details/gklzvczla.sHtML

[T23] Swift：函数
来源：http://baike.tarul.cn/Article/details/gagodixyf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.vehdjk.com/Article/details/gjagkflcx.sHtML

[T24] Swift：闭包
来源：http://mobile.epnwcf.com/Article/details/gdudspdks.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.epnwcf.com/Article/details/gvvujryyl.sHtML

[T25] Swift：结构体
来源：http://read.share.sjlbkw.cn/Article/details/gcegdndie.sHtML

struct P { var x: Int }
来源：http://wap.vehdjk.com/Article/details/ghmfwbhuj.sHtML

[T26] Swift：类与重写
来源：http://read.share.tarul.cn/Article/details/gdsmaqexs.sHtML

class A: Base { override func f() {} }
来源：http://wap.bbcook.cn/Article/details/gqanldbkw.sHtML

[T27] Swift：错误处理
来源：http://read.share.yfazqb.com/Article/details/gyznimhop.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.tarul.cn/Article/details/gzzmizfkm.sHtML

[T28] Swift：枚举
来源：http://www.share.vehdjk.com/Article/details/gvpvhnqug.sHtML

enum Color { case red, green }
来源：http://3g.vehdjk.com/Article/details/gkpcpwogb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fktsv.cn/Article/details/gjgmhagfo.sHtML

guard let x = opt else { return }
来源：http://wap.vehdjk.com/Article/details/gbmwsygkl.sHtML

[T30] Swift：协议
来源：http://mobile.tarul.cn/Article/details/gsukdkcuf.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fktsv.cn/Article/details/gadxmiwja.sHtML

[T31] Lua：Hello World
来源：http://3g.vehdjk.com/Article/details/gchrwnudy.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gzhjzrdmi.sHtML

[T32] Lua：局部变量
来源：http://read.share.epnwcf.com/Article/details/gcbxysuzh.sHtML

local a = 1
来源：http://blog.fktsv.cn/Article/details/gfwrgqfst.sHtML

[T33] Lua：表（数组）
来源：http://wap.yfazqb.com/Article/details/gwvoxxunh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fktsv.cn/Article/details/gafyumfhn.sHtML

[T34] Lua：遍历表
来源：http://m.share.vehdjk.com/Article/details/gpprkddsy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.yfazqb.com/Article/details/gtejvsylc.sHtML

[T35] Lua：字典表
来源：http://read.share.vehdjk.com/Article/details/gppslrqqr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gdvsgbzlr.sHtML

[T36] Lua：函数
来源：http://wap.sjlbkw.cn/Article/details/gcyejwglu.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.tarul.cn/Article/details/gpydjttbs.sHtML

[T37] Lua：字符串拼接
来源：http://baike.epnwcf.com/Article/details/ghscernuz.sHtML

"a" .. "b"
来源：http://baike.vehdjk.com/Article/details/gagouqctg.sHtML

[T38] Lua：条件
来源：http://read.share.sjlbkw.cn/Article/details/giitrehjv.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/glnlpfnbm.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gouiulwqf.sHtML

string.find(s, "%d+")
来源：http://www.share.epnwcf.com/Article/details/gncwfpvmo.sHtML

[T40] Lua：元表
来源：http://wap.fktsv.cn/Article/details/gglfiexvz.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.vehdjk.com/Article/details/gikxrmlhy.sHtML

[T41] Perl：Hello World
来源：http://baike.epnwcf.com/Article/details/gwegzlkya.sHtML

print "Hello\n";
来源：http://baike.epnwcf.com/Article/details/grzkjsizl.sHtML

[T42] Perl：变量类型
来源：http://mobile.sjlbkw.cn/Article/details/gkumpdrfa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.yfazqb.com/Article/details/grsemdwwv.sHtML

[T43] Perl：字符串插值
来源：http://m.share.yfazqb.com/Article/details/ghgmwvfuy.sHtML

"值: $a"
来源：http://wap.tarul.cn/Article/details/gdrctivud.sHtML

[T44] Perl：条件
来源：http://www.share.sjlbkw.cn/Article/details/gslthinkk.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.tarul.cn/Article/details/godpgsfcc.sHtML

[T45] Perl：数组遍历
来源：http://read.share.tarul.cn/Article/details/gvsatkalu.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.vehdjk.com/Article/details/gklbnrgkp.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gfsvkzkih.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fktsv.cn/Article/details/gkjrgfllo.sHtML

[T47] Perl：正则捕获
来源：http://read.share.yfazqb.com/Article/details/gcorepdls.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.sjlbkw.cn/Article/details/gvumjcqzk.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gpdfndsdr.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.yfazqb.com/Article/details/gqimpbywm.sHtML

[T49] Perl：函数
来源：http://wap.epnwcf.com/Article/details/gtpkymgvq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gznvuavlq.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpgecdtm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.yfazqb.com/Article/details/ghetlpcem.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.sjlbkw.cn/Article/details/ghiqztcky.sHtML

[T51] Scala：Hello World
来源：http://wap.sjlbkw.cn/Article/details/ggmbmqptn.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gftpjrwht.sHtML

[T52] Scala：变量
来源：http://www.m.share.fktsv.cn/Article/details/gczhczisg.sHtML

val a = 1;  var b = 2
来源：http://mobile.bbcook.cn/Article/details/gnertvpmf.sHtML

[T53] Scala：字符串插值
来源：http://baike.epnwcf.com/Article/details/gflqevqwm.sHtML

s"值: $b"
来源：http://read.share.vehdjk.com/Article/details/gqnriygxy.sHtML

[T54] Scala：集合映射
来源：http://m.share.bbcook.cn/Article/details/gqhfqcrhi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.epnwcf.com/Article/details/giseesicx.sHtML

[T55] Scala：集合过滤
来源：http://m.share.vehdjk.com/Article/details/ghiejimlq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.vehdjk.com/Article/details/gmqpwdfsr.sHtML

[T56] Scala：样例类
来源：http://m.share.yfazqb.com/Article/details/gzdsqvisy.sHtML

case class User(name: String, age: Int)
来源：http://blog.sjlbkw.cn/Article/details/gckfofvri.sHtML

[T57] Scala：模式匹配
来源：http://www.share.yfazqb.com/Article/details/guucanake.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.bbcook.cn/Article/details/gwbjkptnr.sHtML

[T58] Scala：函数定义
来源：http://mobile.epnwcf.com/Article/details/gvwsklvum.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.sjlbkw.cn/Article/details/gfrwiomun.sHtML

[T59] Scala：循环
来源：http://www.share.tarul.cn/Article/details/gwlavtqpg.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.vehdjk.com/Article/details/gfqdhlnan.sHtML

[T60] Scala：折叠
来源：http://3g.bbcook.cn/Article/details/ghuhieaxf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.yfazqb.com/Article/details/gdmxrnunm.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwxwfrudx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.yfazqb.com/Article/details/gcojsymyk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbhrcrqsj.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.bbcook.cn/Article/details/gkgfeqwcs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/gfiwbucrp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.tarul.cn/Article/details/grcvllkoq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.sjlbkw.cn/Article/details/gtcyvnmem.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.sjlbkw.cn/Article/details/giyeagvgy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.yfazqb.com/Article/details/gfjucmjoz.sHtML

[U04] Py：变量调试打印
来源：http://www.share.tarul.cn/Article/details/gyjdrtrah.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.yfazqb.com/Article/details/ggbitengx.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fktsv.cn/Article/details/gxapqfopd.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gnarfgkqe.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.vehdjk.com/Article/details/girjcizhb.sHtML

{**a, **b}
来源：http://3g.fktsv.cn/Article/details/gesukhnex.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/goobhcbqe.sHtML

{v: k for k, v in d.items()}
来源：http://blog.vehdjk.com/Article/details/gdqsqsbje.sHtML

[U08] Py：展平二维列表
来源：http://www.share.epnwcf.com/Article/details/ggrrmlbex.sHtML

[y for x in nested for y in x]
来源：http://3g.tarul.cn/Article/details/gzinxhkob.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fktsv.cn/Article/details/gqixbkbey.sHtML

max(d, key=d.get)
来源：http://mobile.vehdjk.com/Article/details/gknhxckll.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fktsv.cn/Article/details/geomyezng.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.sjlbkw.cn/Article/details/gpqjfvefy.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhmbscnt.sHtML

(x * 2 for x in arr)
来源：http://blog.epnwcf.com/Article/details/gmssxxrzv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fktsv.cn/Article/details/gjklfebus.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fktsv.cn/Article/details/gbrgzaiwy.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.bbcook.cn/Article/details/gipizuqzk.sHtML

deque(maxlen=10)
来源：http://wap.vehdjk.com/Article/details/gotzcioes.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fktsv.cn/Article/details/gmoywmzyr.sHtML

defaultdict(list)
来源：http://wap.tarul.cn/Article/details/gclceohsk.sHtML

[U15] Py：高精度计时
来源：http://m.share.tarul.cn/Article/details/gaxcbaktp.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/gppzljswe.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrpqgjhh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.tarul.cn/Article/details/gvtoubakh.sHtML

[U17] Py：初始化日志
来源：http://www.blog.yfazqb.com/Article/details/gzxgklrci.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.yfazqb.com/Article/details/gcyyxfirs.sHtML

[U18] Py：预编译正则
来源：http://3g.fktsv.cn/Article/details/ggrnbwwgf.sHtML

pat = re.compile(r"\d+")
来源：http://wap.bbcook.cn/Article/details/gccggmfdb.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fktsv.cn/Article/details/gewcypsxn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.sjlbkw.cn/Article/details/groyxiqcy.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fktsv.cn/Article/details/gvzxtfujn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fktsv.cn/Article/details/girdjrkhp.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.sjlbkw.cn/Article/details/ggyxiiwyi.sHtML

@contextlib.contextmanager
来源：http://www.blog.bbcook.cn/Article/details/ghmqztrxs.sHtML

[U22] Py：矩阵转置
来源：http://wap.epnwcf.com/Article/details/gndyqrznp.sHtML

list(zip(*m))
来源：http://read.share.bbcook.cn/Article/details/gvqvohwhj.sHtML

[U23] Py：分块读取大文件
来源：http://3g.yfazqb.com/Article/details/gltuumnrd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.vehdjk.com/Article/details/gjddjaouv.sHtML

[U24] Py：路径操作
来源：http://www.m.share.tarul.cn/Article/details/gfrbqhqnp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gvsdlirvt.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.sjlbkw.cn/Article/details/gpleeepif.sHtML

csv.DictReader(f)
来源：http://blog.vehdjk.com/Article/details/gjwpzzftv.sHtML

[U26] Py：并发下载
来源：http://www.m.share.epnwcf.com/Article/details/gqxijhzht.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fktsv.cn/Article/details/goflatinn.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.tarul.cn/Article/details/geuvfavah.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.vehdjk.com/Article/details/gkkuudmjm.sHtML

[U28] Py：类型别名
来源：http://baike.sjlbkw.cn/Article/details/gkilqrbjh.sHtML

UserId = int
来源：http://blog.sjlbkw.cn/Article/details/gbzslfovc.sHtML

[U29] Py：属性校验
来源：http://m.share.sjlbkw.cn/Article/details/gvnmfuxng.sHtML

@property 与 @x.setter 配合
来源：http://baike.bbcook.cn/Article/details/gklvdlqiy.sHtML

[U30] Py：数据类
来源：http://baike.sjlbkw.cn/Article/details/gdpryanaz.sHtML

@dataclass(slots=True)
来源：http://www.share.yfazqb.com/Article/details/gtncxommb.sHtML

[U31] Py：单测
来源：http://3g.bbcook.cn/Article/details/gniaspxre.sHtML

python -m pytest -q
来源：http://www.share.fktsv.cn/Article/details/gxigfybar.sHtML

[U32] Py：代码格式化
来源：http://baike.sjlbkw.cn/Article/details/gckdcgkvv.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.epnwcf.com/Article/details/giduyzyzw.sHtML

[U33] Py：打包发布
来源：http://baike.sjlbkw.cn/Article/details/gzjvrhvxo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fktsv.cn/Article/details/gzykddezd.sHtML

[U34] Py：判断编码
来源：http://read.share.vehdjk.com/Article/details/grlypvepb.sHtML

chardet.detect(raw)
来源：http://blog.yfazqb.com/Article/details/gohaskuzl.sHtML

[U35] Py：发送邮件
来源：http://read.share.epnwcf.com/Article/details/gzyqonxwu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.bbcook.cn/Article/details/gqxvhskyt.sHtML

[U36] Py：定时任务
来源：http://baike.epnwcf.com/Article/details/grexrjjid.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.vehdjk.com/Article/details/geowxhqul.sHtML

[U37] Py：读写 Excel
来源：http://www.share.yfazqb.com/Article/details/guvligsvd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.sjlbkw.cn/Article/details/gdusyvltv.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.tarul.cn/Article/details/gvxjrjkkc.sHtML

Path(__file__).resolve().parent
来源：http://read.share.yfazqb.com/Article/details/gklpstkur.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.tarul.cn/Article/details/gtldmxbok.sHtML

sys.stdout.isatty()
来源：http://www.share.tarul.cn/Article/details/gwykbqpfa.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fktsv.cn/Article/details/gkftjyhzj.sHtML

print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/ghvroupql.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fktsv.cn/Article/details/gxgtcmbzv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.yfazqb.com/Article/details/gosalujog.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.vehdjk.com/Article/details/gfacljiyv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.vehdjk.com/Article/details/gqodewhcx.sHtML

[U43] PHP：声明命名空间
来源：http://wap.sjlbkw.cn/Article/details/gebweznaa.sHtML

namespace App\Http;
来源：http://www.share.bbcook.cn/Article/details/gaffxgtza.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.yfazqb.com/Article/details/gdwdqjjej.sHtML

declare(strict_types=1);
来源：http://wap.epnwcf.com/Article/details/gklwsrqwt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fktsv.cn/Article/details/gjrpujeha.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gponcvquy.sHtML

[U46] PHP：可空类型
来源：http://mobile.fktsv.cn/Article/details/gyqvkfzxq.sHtML

?string $name = null
来源：http://read.share.fktsv.cn/Article/details/gdkbfbhvo.sHtML

[U47] PHP：联合类型
来源：http://read.share.fktsv.cn/Article/details/glqkhxfwr.sHtML

int|string $id
来源：http://www.blog.sjlbkw.cn/Article/details/gozgwjgbt.sHtML

[U48] PHP：纯枚举
来源：http://mobile.bbcook.cn/Article/details/gwlcgdwnr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.sjlbkw.cn/Article/details/gjxrmrsed.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fktsv.cn/Article/details/guvwaaxla.sHtML

public readonly string $name
来源：http://m.share.fktsv.cn/Article/details/gsvwirvrq.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fktsv.cn/Article/details/gedhcvpkg.sHtML

public function __construct(private int $id) {}
来源：http://mobile.epnwcf.com/Article/details/gcpoppwnj.sHtML

[U51] PHP：数组解构
来源：http://baike.epnwcf.com/Article/details/ggmopcmsa.sHtML

[$a, $b] = $arr;
来源：http://wap.tarul.cn/Article/details/gcfnfhmjp.sHtML

[U52] PHP：箭头函数
来源：http://baike.bbcook.cn/Article/details/gipsapziw.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.bbcook.cn/Article/details/gogturdyg.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fktsv.cn/Article/details/grmmseldd.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fktsv.cn/Article/details/gqnglmizh.sHtML

[U54] PHP：空安全调用
来源：http://www.share.yfazqb.com/Article/details/gkqffvtyx.sHtML

$obj?->method()
来源：http://www.blog.epnwcf.com/Article/details/gzcwrjedp.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.vehdjk.com/Article/details/gzejmulvg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/goghmcqgx.sHtML

[U56] PHP：命名参数
来源：http://3g.vehdjk.com/Article/details/gqezzcvof.sHtML

f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gfoxxfwzg.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gwoyhkyjc.sHtML

"值: {$a}"
来源：http://blog.tarul.cn/Article/details/gugbeiroi.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.epnwcf.com/Article/details/gtsihawyv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.yfazqb.com/Article/details/gnttrxxxd.sHtML

[U59] PHP：自定义排序
来源：http://mobile.bbcook.cn/Article/details/gnhtrilmd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/gsxhrkyyx.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.epnwcf.com/Article/details/glrbgpmkt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.vehdjk.com/Article/details/gdosistbj.sHtML

[U61] PHP：正则
来源：http://www.m.share.yfazqb.com/Article/details/gdhmmondj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gjvcaaolm.sHtML

[U62] PHP：日期对象
来源：http://read.share.yfazqb.com/Article/details/gpavbjmki.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.vehdjk.com/Article/details/gykjabfcj.sHtML

[U63] PHP：文件读写
来源：http://www.blog.sjlbkw.cn/Article/details/gjlfcndgt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fktsv.cn/Article/details/gvxlbcgji.sHtML

[U64] PHP：目录遍历
来源：http://wap.bbcook.cn/Article/details/gjhkughre.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.epnwcf.com/Article/details/gsriumxyx.sHtML

[U65] PHP：会话
来源：http://blog.epnwcf.com/Article/details/gtzlkaxdk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.tarul.cn/Article/details/gtzmtlxgj.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.tarul.cn/Article/details/gjnwmxcun.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.vehdjk.com/Article/details/gmcqsaqam.sHtML


<!-- 参考信息 -->