代发 wailian999

[S41] C++：类与构造函数
来源：http://www.blog.tarul.cn/Article/details/giqxecfdr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.vehdjk.com/Article/details/gvzaixchu.sHtML

[S42] C++：继承与虚函数
来源：http://3g.sjlbkw.cn/Article/details/gpafnlqkv.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.sjlbkw.cn/Article/details/gevulacmb.sHtML

[S43] C++：智能指针
来源：http://www.blog.bbcook.cn/Article/details/gibgglger.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.yfazqb.com/Article/details/gbxawnhze.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/ggkqwdxis.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fktsv.cn/Article/details/gkkaovtom.sHtML

[S45] C++：lambda
来源：http://www.m.share.tarul.cn/Article/details/gwdyoaemu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.yfazqb.com/Article/details/gfxgcyofw.sHtML

[S46] C++：函数模板
来源：http://baike.epnwcf.com/Article/details/gzhhniaee.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fktsv.cn/Article/details/grypgpmdq.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.yfazqb.com/Article/details/gnwrugqhy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fktsv.cn/Article/details/goqchoeik.sHtML

[S48] C++：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/grzhhqqjh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gsunovwcx.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gjsbdthna.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/gktfxoyoy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.sjlbkw.cn/Article/details/gmmuartzr.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/gcsjnfzhg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gzojqmycx.sHtML

[S51] C++：显式类型转换
来源：http://blog.yfazqb.com/Article/details/gfdfnaski.sHtML

static_cast<double>(a) / b
来源：http://www.blog.vehdjk.com/Article/details/guvhpczsi.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.tarul.cn/Article/details/gsykiukpv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gkozgvcpi.sHtML

[S53] C++：移动语义
来源：http://www.m.share.epnwcf.com/Article/details/gibjtrcue.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fktsv.cn/Article/details/gqfajwike.sHtML

[S54] C++：异常处理
来源：http://m.share.tarul.cn/Article/details/gsjchsybb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.sjlbkw.cn/Article/details/gqmqfikxq.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/gkxtlejdp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/gwumjetnh.sHtML

[S56] C++：optional
来源：http://baike.bbcook.cn/Article/details/gbrddvaoy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.tarul.cn/Article/details/gghykiwyu.sHtML

[S57] C++：编译期常量
来源：http://blog.epnwcf.com/Article/details/gpljsjryz.sHtML

constexpr int N = 10;
来源：http://www.m.share.epnwcf.com/Article/details/grxcfyier.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/glwygrdue.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.sjlbkw.cn/Article/details/gbwjbqxqf.sHtML

[S59] C++：静态断言
来源：http://www.blog.bbcook.cn/Article/details/gsaulvlna.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.bbcook.cn/Article/details/gulwlqjxd.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.epnwcf.com/Article/details/grlnlgwmz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gvorcgzkg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gifpufmne.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gbmgxmxrm.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqalihouw.sHtML

[T01] Kotlin：Hello World
来源：http://baike.epnwcf.com/Article/details/gelgqlzpe.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gbmyhbvpx.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gvqdruoxr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.yfazqb.com/Article/details/galtmqctn.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fktsv.cn/Article/details/gkhcfabbm.sHtML

"值: $b"
来源：http://baike.bbcook.cn/Article/details/gufwguhfr.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/gmmdtlpnq.sHtML

val n: String? = null;  n?.length
来源：http://mobile.sjlbkw.cn/Article/details/gyjtxgijf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fktsv.cn/Article/details/geejwmhoj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.yfazqb.com/Article/details/gtmbfylom.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fktsv.cn/Article/details/glklcrich.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.bbcook.cn/Article/details/gqwfwtynx.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/geftkbrzc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/gvgjqqbsj.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/gploxuksv.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fktsv.cn/Article/details/gywecasgi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.yfazqb.com/Article/details/gfpfnpnha.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.epnwcf.com/Article/details/gcwwwzpvu.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fktsv.cn/Article/details/gxgszcpgn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.tarul.cn/Article/details/gznsknilj.sHtML

[T11] Kotlin：协程
来源：http://baike.sjlbkw.cn/Article/details/gocywcmef.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.tarul.cn/Article/details/gewxpplml.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fktsv.cn/Article/details/gqqllzewm.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gebssqsgz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.vehdjk.com/Article/details/gejffcpej.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.epnwcf.com/Article/details/gyvrxcgwb.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/gklivfekr.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gbvewezuj.sHtML

[T15] Kotlin：接口
来源：http://www.share.bbcook.cn/Article/details/gpbwjdnxc.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.vehdjk.com/Article/details/godpgkjdj.sHtML

[T16] Swift：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gnworelvc.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gioiqwyqm.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.epnwcf.com/Article/details/gutzdeiyx.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/gvrukgmsp.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gfpwozvpn.sHtML

"值: \(b)"
来源：http://3g.sjlbkw.cn/Article/details/gmtxneyza.sHtML

[T19] Swift：可选绑定
来源：http://blog.yfazqb.com/Article/details/grrvkehwr.sHtML

if let n = opt { print(n) }
来源：http://wap.yfazqb.com/Article/details/grzthuxku.sHtML

[T20] Swift：数组操作
来源：http://blog.yfazqb.com/Article/details/glaysxjgc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.epnwcf.com/Article/details/gozicviba.sHtML

[T21] Swift：遍历
来源：http://3g.fktsv.cn/Article/details/gugtoitop.sHtML

for x in a { print(x) }
来源：http://www.blog.fktsv.cn/Article/details/gltslythg.sHtML

[T22] Swift：字典
来源：http://www.blog.bbcook.cn/Article/details/ggcshlpqy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.yfazqb.com/Article/details/ghzcdyxbw.sHtML

[T23] Swift：函数
来源：http://3g.epnwcf.com/Article/details/gxbbdwuxz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.bbcook.cn/Article/details/gustafrpt.sHtML

[T24] Swift：闭包
来源：http://www.share.yfazqb.com/Article/details/ghlrnercn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.epnwcf.com/Article/details/gfvejkiqa.sHtML

[T25] Swift：结构体
来源：http://read.share.bbcook.cn/Article/details/gqtmfqbvl.sHtML

struct P { var x: Int }
来源：http://www.blog.epnwcf.com/Article/details/grfxecpay.sHtML

[T26] Swift：类与重写
来源：http://wap.epnwcf.com/Article/details/gmjogcjwl.sHtML

class A: Base { override func f() {} }
来源：http://www.share.vehdjk.com/Article/details/ghzogdptb.sHtML

[T27] Swift：错误处理
来源：http://wap.sjlbkw.cn/Article/details/gdcbkgzks.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.sjlbkw.cn/Article/details/gxrvchrvd.sHtML

[T28] Swift：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gynzhhgku.sHtML

enum Color { case red, green }
来源：http://read.share.bbcook.cn/Article/details/glqsjxbvc.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.tarul.cn/Article/details/gsqzidkgd.sHtML

guard let x = opt else { return }
来源：http://www.m.share.bbcook.cn/Article/details/gjzfpuadu.sHtML

[T30] Swift：协议
来源：http://www.m.share.yfazqb.com/Article/details/gocskaqqh.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.tarul.cn/Article/details/gabeklucl.sHtML

[T31] Lua：Hello World
来源：http://baike.fktsv.cn/Article/details/gkhjheynl.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/gbukchfpe.sHtML

[T32] Lua：局部变量
来源：http://blog.yfazqb.com/Article/details/grzqozhmw.sHtML

local a = 1
来源：http://wap.vehdjk.com/Article/details/guobwwlpx.sHtML

[T33] Lua：表（数组）
来源：http://mobile.sjlbkw.cn/Article/details/gievnutrn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.sjlbkw.cn/Article/details/gfogodvbu.sHtML

[T34] Lua：遍历表
来源：http://www.share.sjlbkw.cn/Article/details/gvwhqjbbd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.yfazqb.com/Article/details/grcinbwvg.sHtML

[T35] Lua：字典表
来源：http://read.share.bbcook.cn/Article/details/gcajzzbva.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gcvgkfgne.sHtML

[T36] Lua：函数
来源：http://m.share.yfazqb.com/Article/details/gzbntxuuc.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/gmdqmmgta.sHtML

[T37] Lua：字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gdeibbdam.sHtML

"a" .. "b"
来源：http://mobile.sjlbkw.cn/Article/details/gahhfgdku.sHtML

[T38] Lua：条件
来源：http://mobile.sjlbkw.cn/Article/details/gzaghdinr.sHtML

if x > 0 then print("正") end
来源：http://blog.sjlbkw.cn/Article/details/gwvognlwv.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fktsv.cn/Article/details/gmdvruakf.sHtML

string.find(s, "%d+")
来源：http://www.share.vehdjk.com/Article/details/gzfdsajhh.sHtML

[T40] Lua：元表
来源：http://www.m.share.epnwcf.com/Article/details/gmhurdinr.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fktsv.cn/Article/details/gmvpidfhh.sHtML

[T41] Perl：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gtkltiwba.sHtML

print "Hello\n";
来源：http://blog.bbcook.cn/Article/details/gpyrtqagf.sHtML

[T42] Perl：变量类型
来源：http://3g.sjlbkw.cn/Article/details/ghprwzolq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.yfazqb.com/Article/details/gjfjypvmo.sHtML

[T43] Perl：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gbiovwues.sHtML

"值: $a"
来源：http://www.share.vehdjk.com/Article/details/gbatqsnqv.sHtML

[T44] Perl：条件
来源：http://3g.fktsv.cn/Article/details/grxkviusz.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fktsv.cn/Article/details/giyvenajc.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.epnwcf.com/Article/details/gbhpurkea.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.bbcook.cn/Article/details/gdfdlqvdp.sHtML

[T46] Perl：哈希操作
来源：http://read.share.yfazqb.com/Article/details/gfwjdyler.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.epnwcf.com/Article/details/glzcunozb.sHtML

[T47] Perl：正则捕获
来源：http://baike.tarul.cn/Article/details/gprjxhadq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fktsv.cn/Article/details/glzfiyadb.sHtML

[T48] Perl：正则替换
来源：http://www.blog.epnwcf.com/Article/details/gmvcdoocx.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.epnwcf.com/Article/details/gsihxbtut.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/gggfhhgse.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gmjdhyguw.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/glnjmlbmd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.sjlbkw.cn/Article/details/gefuxtjci.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.epnwcf.com/Article/details/gozucsndq.sHtML

[T51] Scala：Hello World
来源：http://www.share.vehdjk.com/Article/details/gfgketxwv.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gblufasqn.sHtML

[T52] Scala：变量
来源：http://blog.fktsv.cn/Article/details/grfenhhsg.sHtML

val a = 1;  var b = 2
来源：http://baike.fktsv.cn/Article/details/gmpppxmfu.sHtML

[T53] Scala：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gbparzwbz.sHtML

s"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/gcoqidehf.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkxbvidt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.tarul.cn/Article/details/gcueyhxlp.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gxgjvwvly.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.sjlbkw.cn/Article/details/gqmpwwwni.sHtML

[T56] Scala：样例类
来源：http://read.share.vehdjk.com/Article/details/gssvgqbxt.sHtML

case class User(name: String, age: Int)
来源：http://m.share.epnwcf.com/Article/details/gkqtggutz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gfhiipyng.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.tarul.cn/Article/details/gznkscton.sHtML

[T58] Scala：函数定义
来源：http://www.share.tarul.cn/Article/details/gzmrurahq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.epnwcf.com/Article/details/gotiiphek.sHtML

[T59] Scala：循环
来源：http://read.share.epnwcf.com/Article/details/gvscimuqo.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.vehdjk.com/Article/details/grhsjsoxf.sHtML

[T60] Scala：折叠
来源：http://mobile.epnwcf.com/Article/details/grhtuaobe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fktsv.cn/Article/details/gshrgzaym.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gybeyqjbx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gwhuwlztk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gchfxzpbi.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.sjlbkw.cn/Article/details/gjdymbdkm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.vehdjk.com/Article/details/gpeovasas.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.yfazqb.com/Article/details/grernlbln.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.bbcook.cn/Article/details/gnpsserxj.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.sjlbkw.cn/Article/details/grpxdbmov.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fktsv.cn/Article/details/gugdmohsc.sHtML

[U04] Py：变量调试打印
来源：http://www.share.sjlbkw.cn/Article/details/glmdppkme.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhpvxzwy.sHtML

[U05] Py：列表去重且保序
来源：http://3g.yfazqb.com/Article/details/gjxiopbps.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/gnxbtweed.sHtML

[U06] Py：合并两个字典
来源：http://mobile.tarul.cn/Article/details/gpwweeeyp.sHtML

{**a, **b}
来源：http://blog.vehdjk.com/Article/details/gidoosqyg.sHtML

[U07] Py：反转字典键值
来源：http://3g.sjlbkw.cn/Article/details/gxmzncujl.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fktsv.cn/Article/details/guctylmht.sHtML

[U08] Py：展平二维列表
来源：http://blog.fktsv.cn/Article/details/gdtkxofek.sHtML

[y for x in nested for y in x]
来源：http://m.share.bbcook.cn/Article/details/gumimstfs.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.yfazqb.com/Article/details/gafaqjmql.sHtML

max(d, key=d.get)
来源：http://baike.sjlbkw.cn/Article/details/glegcbyrp.sHtML

[U10] Py：按值排序字典
来源：http://read.share.sjlbkw.cn/Article/details/gvxthjgbv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.sjlbkw.cn/Article/details/gmdufolhy.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.tarul.cn/Article/details/gplymebhr.sHtML

(x * 2 for x in arr)
来源：http://m.share.tarul.cn/Article/details/gpyyxerkk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.bbcook.cn/Article/details/gzxnogxqf.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.vehdjk.com/Article/details/gqgtesern.sHtML

[U13] Py：固定长度队列
来源：http://blog.sjlbkw.cn/Article/details/gevskwdvz.sHtML

deque(maxlen=10)
来源：http://blog.fktsv.cn/Article/details/gdxjfpnpz.sHtML

[U14] Py：分组收集到列表
来源：http://wap.bbcook.cn/Article/details/glpemxnfv.sHtML

defaultdict(list)
来源：http://www.share.sjlbkw.cn/Article/details/gwkmntjti.sHtML

[U15] Py：高精度计时
来源：http://www.blog.vehdjk.com/Article/details/gzfejbstn.sHtML

t = time.perf_counter()
来源：http://3g.sjlbkw.cn/Article/details/glqfjwvyw.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.sjlbkw.cn/Article/details/gogjtafpw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fktsv.cn/Article/details/gcfkeswcs.sHtML

[U17] Py：初始化日志
来源：http://mobile.fktsv.cn/Article/details/ghlcugmmh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.tarul.cn/Article/details/ghlsdmdxa.sHtML

[U18] Py：预编译正则
来源：http://m.share.bbcook.cn/Article/details/gfcjhdzwn.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gheapafyx.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fktsv.cn/Article/details/gaylbovmg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.vehdjk.com/Article/details/ghbzupdhh.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.bbcook.cn/Article/details/gikxwloey.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.tarul.cn/Article/details/gkhnamskw.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.tarul.cn/Article/details/gpipcaian.sHtML

@contextlib.contextmanager
来源：http://baike.vehdjk.com/Article/details/gbxlvqrtu.sHtML

[U22] Py：矩阵转置
来源：http://baike.vehdjk.com/Article/details/gdthinren.sHtML

list(zip(*m))
来源：http://www.blog.sjlbkw.cn/Article/details/gtzlrjwno.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.bbcook.cn/Article/details/gmicvofuv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.epnwcf.com/Article/details/gnuaiurab.sHtML

[U24] Py：路径操作
来源：http://mobile.vehdjk.com/Article/details/gfixyrsqz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/grytqwgwq.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.sjlbkw.cn/Article/details/gcuurmczw.sHtML

csv.DictReader(f)
来源：http://blog.tarul.cn/Article/details/gptnjjbpl.sHtML

[U26] Py：并发下载
来源：http://www.share.sjlbkw.cn/Article/details/gxoikohje.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.vehdjk.com/Article/details/gmvclnptx.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.epnwcf.com/Article/details/garhvxwkm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.vehdjk.com/Article/details/glcaajlac.sHtML

[U28] Py：类型别名
来源：http://read.share.epnwcf.com/Article/details/gzvcunbki.sHtML

UserId = int
来源：http://3g.vehdjk.com/Article/details/gmxuogycw.sHtML

[U29] Py：属性校验
来源：http://read.share.fktsv.cn/Article/details/gypwijiuj.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fktsv.cn/Article/details/gcmxwmakc.sHtML

[U30] Py：数据类
来源：http://www.share.vehdjk.com/Article/details/gwlqmbtyj.sHtML

@dataclass(slots=True)
来源：http://www.m.share.epnwcf.com/Article/details/gdbvljgys.sHtML

[U31] Py：单测
来源：http://read.share.epnwcf.com/Article/details/grodtltth.sHtML

python -m pytest -q
来源：http://www.share.epnwcf.com/Article/details/gmjpsafci.sHtML

[U32] Py：代码格式化
来源：http://mobile.vehdjk.com/Article/details/gstuaxpvk.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.bbcook.cn/Article/details/gmzncxnbc.sHtML

[U33] Py：打包发布
来源：http://wap.tarul.cn/Article/details/gfhlozefb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.sjlbkw.cn/Article/details/gultqcvsw.sHtML

[U34] Py：判断编码
来源：http://baike.epnwcf.com/Article/details/ginxlmvpn.sHtML

chardet.detect(raw)
来源：http://read.share.vehdjk.com/Article/details/gjrpzozvf.sHtML

[U35] Py：发送邮件
来源：http://m.share.yfazqb.com/Article/details/glcwcexuf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.tarul.cn/Article/details/gkgsjdzkh.sHtML

[U36] Py：定时任务
来源：http://baike.epnwcf.com/Article/details/gnvvvwlfi.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.vehdjk.com/Article/details/gqeebnklv.sHtML

[U37] Py：读写 Excel
来源：http://m.share.vehdjk.com/Article/details/gsgivjbhm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.vehdjk.com/Article/details/gevinmkxo.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.yfazqb.com/Article/details/glfrlukng.sHtML

Path(__file__).resolve().parent
来源：http://m.share.bbcook.cn/Article/details/gtfcxjraj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.bbcook.cn/Article/details/gdckksnlx.sHtML

sys.stdout.isatty()
来源：http://mobile.vehdjk.com/Article/details/gowxmhjkm.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.sjlbkw.cn/Article/details/ghbextqot.sHtML

print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/gzwrblqdq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.yfazqb.com/Article/details/gxtegvmwr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.yfazqb.com/Article/details/ghedumcuy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.yfazqb.com/Article/details/gboppymmg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.yfazqb.com/Article/details/goxlsozcc.sHtML

[U43] PHP：声明命名空间
来源：http://wap.tarul.cn/Article/details/guhilwpio.sHtML

namespace App\Http;
来源：http://blog.bbcook.cn/Article/details/gheaqbiqn.sHtML

[U44] PHP：开启严格类型
来源：http://baike.yfazqb.com/Article/details/gcowsyjpe.sHtML

declare(strict_types=1);
来源：http://m.share.sjlbkw.cn/Article/details/gkxwtrmrn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.epnwcf.com/Article/details/gwhsegezh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gdndkbreh.sHtML

[U46] PHP：可空类型
来源：http://m.share.epnwcf.com/Article/details/gtqioudvf.sHtML

?string $name = null
来源：http://3g.epnwcf.com/Article/details/gkhuuyinx.sHtML

[U47] PHP：联合类型
来源：http://read.share.bbcook.cn/Article/details/gghodqvdv.sHtML

int|string $id
来源：http://baike.sjlbkw.cn/Article/details/gjwbnjvpi.sHtML

[U48] PHP：纯枚举
来源：http://wap.tarul.cn/Article/details/gvzcgcyxa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.bbcook.cn/Article/details/goanrdsad.sHtML

[U49] PHP：只读属性
来源：http://m.share.sjlbkw.cn/Article/details/gpuicjbyo.sHtML

public readonly string $name
来源：http://wap.fktsv.cn/Article/details/grofcqplx.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.epnwcf.com/Article/details/gcmvnukjc.sHtML

public function __construct(private int $id) {}
来源：http://m.share.yfazqb.com/Article/details/gshpthrkq.sHtML

[U51] PHP：数组解构
来源：http://3g.bbcook.cn/Article/details/gmlxrnrit.sHtML

[$a, $b] = $arr;
来源：http://wap.tarul.cn/Article/details/gzhjerhmu.sHtML

[U52] PHP：箭头函数
来源：http://wap.epnwcf.com/Article/details/gbqhmbzge.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.yfazqb.com/Article/details/gbfxsfatc.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.vehdjk.com/Article/details/gtxhswiet.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.tarul.cn/Article/details/gbcbeynwu.sHtML

[U54] PHP：空安全调用
来源：http://wap.bbcook.cn/Article/details/gqmhrzwdp.sHtML

$obj?->method()
来源：http://baike.sjlbkw.cn/Article/details/grfgqlpsg.sHtML

[U55] PHP：match 表达式
来源：http://baike.vehdjk.com/Article/details/gceiqwbou.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/gkrnlbeov.sHtML

[U56] PHP：命名参数
来源：http://mobile.fktsv.cn/Article/details/gaokookjr.sHtML

f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gvhmwrjpm.sHtML

[U57] PHP：字符串插值
来源：http://blog.bbcook.cn/Article/details/gwvnheadz.sHtML

"值: {$a}"
来源：http://baike.tarul.cn/Article/details/gritazxka.sHtML

[U58] PHP：数组三件套
来源：http://m.share.epnwcf.com/Article/details/gtycvmsgm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fktsv.cn/Article/details/gzkzvdzey.sHtML

[U59] PHP：自定义排序
来源：http://mobile.yfazqb.com/Article/details/gpsdsjezt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.yfazqb.com/Article/details/gomtghluz.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.epnwcf.com/Article/details/gpoelxymb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fktsv.cn/Article/details/geyhasdzd.sHtML

[U61] PHP：正则
来源：http://m.share.bbcook.cn/Article/details/gsobmwwqv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.sjlbkw.cn/Article/details/gczjnnykx.sHtML

[U62] PHP：日期对象
来源：http://m.share.vehdjk.com/Article/details/gmrviwfdy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.vehdjk.com/Article/details/gshvvaeto.sHtML

[U63] PHP：文件读写
来源：http://mobile.vehdjk.com/Article/details/gbujlarga.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.epnwcf.com/Article/details/gogufexzs.sHtML

[U64] PHP：目录遍历
来源：http://baike.bbcook.cn/Article/details/gqzhbvdwh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.epnwcf.com/Article/details/gomxnscgk.sHtML

[U65] PHP：会话
来源：http://m.share.bbcook.cn/Article/details/gevtwogxj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.bbcook.cn/Article/details/ghuguclzf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fktsv.cn/Article/details/gmwsihmzx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.tarul.cn/Article/details/gjgerekxr.sHtML


<!-- 参考信息 -->