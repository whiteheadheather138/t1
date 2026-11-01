代发 wailian999

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/ghndqebic.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.sjlbkw.cn/Article/details/gybywgmmm.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.yfazqb.com/Article/details/gdvgnaxlk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.vehdjk.com/Article/details/gljlzbgez.sHtML

[S43] C++：智能指针
来源：http://baike.bbcook.cn/Article/details/gldyckxvq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gjfjwlgwb.sHtML

[S44] C++：引用传参
来源：http://read.share.sjlbkw.cn/Article/details/goslkrnbj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.vehdjk.com/Article/details/grkellfae.sHtML

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/gzbpfflgb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/getrlihkd.sHtML

[S46] C++：函数模板
来源：http://mobile.sjlbkw.cn/Article/details/gifdgctpy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.epnwcf.com/Article/details/gjznqlplm.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.yfazqb.com/Article/details/gakcyofuu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.sjlbkw.cn/Article/details/gretrdjko.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gdbnrjrhm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.sjlbkw.cn/Article/details/gwlpglcnd.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fktsv.cn/Article/details/gbscjzqhr.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/gfqpehgdj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.sjlbkw.cn/Article/details/gkvdoclbv.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/griljfbyo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.tarul.cn/Article/details/gznkqepwe.sHtML

[S51] C++：显式类型转换
来源：http://m.share.vehdjk.com/Article/details/gsfcdoebi.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/gehieeucu.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.epnwcf.com/Article/details/gblayxvdw.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fktsv.cn/Article/details/gsigslnol.sHtML

[S53] C++：移动语义
来源：http://wap.sjlbkw.cn/Article/details/gxbzyoyop.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.bbcook.cn/Article/details/gwoesyhgv.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fktsv.cn/Article/details/gnrgpuqpr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fktsv.cn/Article/details/gkotxxldv.sHtML

[S55] C++：结构化绑定
来源：http://www.share.tarul.cn/Article/details/gkfywnhqq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/gxejyewbu.sHtML

[S56] C++：optional
来源：http://m.share.yfazqb.com/Article/details/gphrjmubu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.yfazqb.com/Article/details/gkvcexmwj.sHtML

[S57] C++：编译期常量
来源：http://baike.tarul.cn/Article/details/gdvffewdz.sHtML

constexpr int N = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gfuodoxri.sHtML

[S58] C++：命名空间
来源：http://www.share.epnwcf.com/Article/details/gxpqxugaf.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.sjlbkw.cn/Article/details/gtojefinc.sHtML

[S59] C++：静态断言
来源：http://www.share.vehdjk.com/Article/details/gnaxpdqzr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.tarul.cn/Article/details/ghjsofhlu.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.tarul.cn/Article/details/guvyhsmxg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.bbcook.cn/Article/details/griqzmjji.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gljglabyx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gwfrvqrjo.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/glvgegnbe.sHtML

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/grwyrclif.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gjeozrvcz.sHtML

[T02] Kotlin：变量
来源：http://read.share.yfazqb.com/Article/details/gjegjzehx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.bbcook.cn/Article/details/gfrlfsvmo.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gdsgoixrd.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gzjpyeynv.sHtML

[T04] Kotlin：空安全
来源：http://baike.sjlbkw.cn/Article/details/gljkpvjxk.sHtML

val n: String? = null;  n?.length
来源：http://m.share.bbcook.cn/Article/details/gwlzhgdzl.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.epnwcf.com/Article/details/glpcrfdyt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/goorfzbrf.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.epnwcf.com/Article/details/gbjnadwbo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.epnwcf.com/Article/details/gqwvzedns.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.tarul.cn/Article/details/glaiymojq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.bbcook.cn/Article/details/geaupygdq.sHtML

[T08] Kotlin：数据类
来源：http://baike.sjlbkw.cn/Article/details/gwxqgecoj.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.tarul.cn/Article/details/gdzcojrse.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gleukpoqs.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.epnwcf.com/Article/details/gjhtejcli.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.bbcook.cn/Article/details/gvgccahen.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/greapnbyv.sHtML

[T11] Kotlin：协程
来源：http://baike.vehdjk.com/Article/details/gaizkqopy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.epnwcf.com/Article/details/gizitlycc.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.tarul.cn/Article/details/gsjrgiyue.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gimvewuxr.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.tarul.cn/Article/details/gqzeilnfk.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.bbcook.cn/Article/details/gbefxabft.sHtML

[T14] Kotlin：循环
来源：http://m.share.bbcook.cn/Article/details/gsnfmbxtc.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gqswyqaph.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/gijukygoj.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.epnwcf.com/Article/details/gtopicaap.sHtML

[T16] Swift：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gzzmtlank.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/gvmbqhqau.sHtML

[T17] Swift：变量与常量
来源：http://www.share.epnwcf.com/Article/details/gnbconezk.sHtML

var a = 1;  let b = 2
来源：http://3g.epnwcf.com/Article/details/gxhzbgnja.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/givckkgzo.sHtML

"值: \(b)"
来源：http://wap.yfazqb.com/Article/details/ghdxcntaq.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gnvohdxui.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/guvnrwepo.sHtML

[T20] Swift：数组操作
来源：http://3g.epnwcf.com/Article/details/gorqonqyq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.yfazqb.com/Article/details/gckfeszvc.sHtML

[T21] Swift：遍历
来源：http://read.share.sjlbkw.cn/Article/details/gsqxfznsj.sHtML

for x in a { print(x) }
来源：http://3g.vehdjk.com/Article/details/gcjwrbclr.sHtML

[T22] Swift：字典
来源：http://baike.vehdjk.com/Article/details/ggvvanvka.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.bbcook.cn/Article/details/gwuzroibc.sHtML

[T23] Swift：函数
来源：http://www.m.share.yfazqb.com/Article/details/gyqxezsys.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.tarul.cn/Article/details/gmoiytmjn.sHtML

[T24] Swift：闭包
来源：http://www.m.share.vehdjk.com/Article/details/glpobcpkc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.yfazqb.com/Article/details/gcchunddf.sHtML

[T25] Swift：结构体
来源：http://wap.yfazqb.com/Article/details/ggmomqqov.sHtML

struct P { var x: Int }
来源：http://baike.vehdjk.com/Article/details/gtyzbqnck.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.sjlbkw.cn/Article/details/ginjllxys.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gbeooxhqc.sHtML

[T27] Swift：错误处理
来源：http://read.share.bbcook.cn/Article/details/gbjrwxddo.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/glwlisges.sHtML

[T28] Swift：枚举
来源：http://3g.tarul.cn/Article/details/gxonatias.sHtML

enum Color { case red, green }
来源：http://baike.tarul.cn/Article/details/genvrifif.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gxupizpqw.sHtML

guard let x = opt else { return }
来源：http://www.m.share.bbcook.cn/Article/details/gvftaotum.sHtML

[T30] Swift：协议
来源：http://baike.vehdjk.com/Article/details/gzdtvkylj.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.sjlbkw.cn/Article/details/ghgkvmaxv.sHtML

[T31] Lua：Hello World
来源：http://www.share.bbcook.cn/Article/details/gzfkppgur.sHtML

print("Hello")
来源：http://www.blog.tarul.cn/Article/details/gxbpoeoua.sHtML

[T32] Lua：局部变量
来源：http://read.share.fktsv.cn/Article/details/gorbrrkru.sHtML

local a = 1
来源：http://3g.sjlbkw.cn/Article/details/gcrlsrqia.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fktsv.cn/Article/details/ggejfpenf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.bbcook.cn/Article/details/gwcbvxpkm.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/gwougkrhk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.vehdjk.com/Article/details/gcnleaeoc.sHtML

[T35] Lua：字典表
来源：http://3g.vehdjk.com/Article/details/gghayeamd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gtgkauhqe.sHtML

[T36] Lua：函数
来源：http://baike.fktsv.cn/Article/details/gsemrbfrq.sHtML

function add(a, b) return a + b end
来源：http://www.blog.epnwcf.com/Article/details/gmaqygqbv.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gtddxgxat.sHtML

"a" .. "b"
来源：http://blog.vehdjk.com/Article/details/gouuhnzci.sHtML

[T38] Lua：条件
来源：http://www.blog.tarul.cn/Article/details/gpraeingy.sHtML

if x > 0 then print("正") end
来源：http://read.share.fktsv.cn/Article/details/gppmhatya.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gcuprbzfs.sHtML

string.find(s, "%d+")
来源：http://www.blog.yfazqb.com/Article/details/gyfgueatu.sHtML

[T40] Lua：元表
来源：http://mobile.fktsv.cn/Article/details/gjcysyers.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fktsv.cn/Article/details/gkswnbutu.sHtML

[T41] Perl：Hello World
来源：http://www.share.epnwcf.com/Article/details/gauewhknb.sHtML

print "Hello\n";
来源：http://www.blog.fktsv.cn/Article/details/gtmqwrdhy.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gugpyfwtp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.sjlbkw.cn/Article/details/gjgfjilml.sHtML

[T43] Perl：字符串插值
来源：http://m.share.bbcook.cn/Article/details/glsxgcfep.sHtML

"值: $a"
来源：http://m.share.bbcook.cn/Article/details/gpohyhure.sHtML

[T44] Perl：条件
来源：http://www.share.sjlbkw.cn/Article/details/gxahlyfqh.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.sjlbkw.cn/Article/details/gwhgjxpvp.sHtML

[T45] Perl：数组遍历
来源：http://m.share.sjlbkw.cn/Article/details/gamdwahym.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.bbcook.cn/Article/details/gyegjykzi.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjjidwpf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fktsv.cn/Article/details/gmjiqqufg.sHtML

[T47] Perl：正则捕获
来源：http://read.share.bbcook.cn/Article/details/gbnrulwup.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.vehdjk.com/Article/details/gvvuiemcy.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gzhqqtofy.sHtML

$s =~ s/old/new/g;
来源：http://mobile.sjlbkw.cn/Article/details/gzqcagzik.sHtML

[T49] Perl：函数
来源：http://wap.vehdjk.com/Article/details/gpzuqipmd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gvmbxsnvf.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gwnhuuirk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.tarul.cn/Article/details/gbtpvaxzs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.epnwcf.com/Article/details/gxuhehvgj.sHtML

[T51] Scala：Hello World
来源：http://mobile.vehdjk.com/Article/details/gjgeuvart.sHtML

println("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gqoeyrncb.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gpwvyhntn.sHtML

val a = 1;  var b = 2
来源：http://www.share.vehdjk.com/Article/details/ggcfiiscv.sHtML

[T53] Scala：字符串插值
来源：http://3g.yfazqb.com/Article/details/gmuwvydsu.sHtML

s"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/ghhhbvhim.sHtML

[T54] Scala：集合映射
来源：http://mobile.tarul.cn/Article/details/grqhxqeok.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.sjlbkw.cn/Article/details/gubokjlkv.sHtML

[T55] Scala：集合过滤
来源：http://blog.yfazqb.com/Article/details/gpunyntao.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.yfazqb.com/Article/details/gfpqkfypx.sHtML

[T56] Scala：样例类
来源：http://read.share.sjlbkw.cn/Article/details/grocslgbq.sHtML

case class User(name: String, age: Int)
来源：http://mobile.bbcook.cn/Article/details/ghvtymywb.sHtML

[T57] Scala：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/guoawlxti.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.sjlbkw.cn/Article/details/gwqwpmtyn.sHtML

[T58] Scala：函数定义
来源：http://wap.yfazqb.com/Article/details/gtlwayity.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.yfazqb.com/Article/details/gvdznzyzt.sHtML

[T59] Scala：循环
来源：http://baike.yfazqb.com/Article/details/gchooahty.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gyheetlfx.sHtML

[T60] Scala：折叠
来源：http://www.share.sjlbkw.cn/Article/details/glclcueue.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.bbcook.cn/Article/details/gbqxmkjjg.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glhmticbf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gdaseqnii.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpgiexdpr.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.epnwcf.com/Article/details/gjnjalxni.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.bbcook.cn/Article/details/gaycrlrsy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.yfazqb.com/Article/details/gdvkgvikc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/ggfyyablx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.yfazqb.com/Article/details/gmylcesss.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.vehdjk.com/Article/details/grnimokcv.sHtML

[U04] Py：变量调试打印
来源：http://wap.tarul.cn/Article/details/gailgturq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.bbcook.cn/Article/details/gbccxrcdo.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzjvhufs.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gryeaevaw.sHtML

[U06] Py：合并两个字典
来源：http://blog.vehdjk.com/Article/details/glxavnjfy.sHtML

{**a, **b}
来源：http://www.share.vehdjk.com/Article/details/gzpblixxb.sHtML

[U07] Py：反转字典键值
来源：http://m.share.yfazqb.com/Article/details/gjyguegje.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.tarul.cn/Article/details/ggddivbpn.sHtML

[U08] Py：展平二维列表
来源：http://blog.fktsv.cn/Article/details/gnkeleamd.sHtML

[y for x in nested for y in x]
来源：http://read.share.yfazqb.com/Article/details/ghypotjdo.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.bbcook.cn/Article/details/gbgrdcwpp.sHtML

max(d, key=d.get)
来源：http://www.blog.bbcook.cn/Article/details/glzuczpnm.sHtML

[U10] Py：按值排序字典
来源：http://mobile.vehdjk.com/Article/details/gwuoxgvtm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fktsv.cn/Article/details/guwrerzmt.sHtML

[U11] Py：生成器表达式
来源：http://blog.sjlbkw.cn/Article/details/gjzngmefm.sHtML

(x * 2 for x in arr)
来源：http://wap.vehdjk.com/Article/details/gcpfiqjjw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.tarul.cn/Article/details/ghxjtlnli.sHtML

Counter(arr).most_common(3)
来源：http://3g.fktsv.cn/Article/details/gtqpzwgny.sHtML

[U13] Py：固定长度队列
来源：http://wap.yfazqb.com/Article/details/giyjbzhmn.sHtML

deque(maxlen=10)
来源：http://read.share.yfazqb.com/Article/details/galxqnfvz.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.sjlbkw.cn/Article/details/guwiewlch.sHtML

defaultdict(list)
来源：http://www.share.yfazqb.com/Article/details/gqscaeejt.sHtML

[U15] Py：高精度计时
来源：http://m.share.epnwcf.com/Article/details/gmpgosghj.sHtML

t = time.perf_counter()
来源：http://baike.fktsv.cn/Article/details/ggfouepbz.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.bbcook.cn/Article/details/gkucvhubf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.tarul.cn/Article/details/gcszxvfkq.sHtML

[U17] Py：初始化日志
来源：http://baike.epnwcf.com/Article/details/gvlthiqpy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fktsv.cn/Article/details/gdcdtwygi.sHtML

[U18] Py：预编译正则
来源：http://mobile.tarul.cn/Article/details/gelehdayc.sHtML

pat = re.compile(r"\d+")
来源：http://blog.yfazqb.com/Article/details/gqsphnnav.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.vehdjk.com/Article/details/guvyuqiom.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.bbcook.cn/Article/details/gpskkaygc.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.bbcook.cn/Article/details/glayogosx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.sjlbkw.cn/Article/details/gamvecllh.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fktsv.cn/Article/details/gewudmrfx.sHtML

@contextlib.contextmanager
来源：http://wap.tarul.cn/Article/details/gfkpggqgy.sHtML

[U22] Py：矩阵转置
来源：http://www.share.epnwcf.com/Article/details/guzdlvrcd.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/guvakfgpd.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.tarul.cn/Article/details/gsldsiylc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.epnwcf.com/Article/details/gcohigazs.sHtML

[U24] Py：路径操作
来源：http://baike.yfazqb.com/Article/details/guddruwru.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gksrvstlr.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fktsv.cn/Article/details/glvcsrbcw.sHtML

csv.DictReader(f)
来源：http://3g.bbcook.cn/Article/details/goavoalne.sHtML

[U26] Py：并发下载
来源：http://www.blog.tarul.cn/Article/details/gsdgcjoev.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.vehdjk.com/Article/details/gwyqaktcn.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.tarul.cn/Article/details/glztskbrz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fktsv.cn/Article/details/gboflibdx.sHtML

[U28] Py：类型别名
来源：http://m.share.tarul.cn/Article/details/gzglhsafq.sHtML

UserId = int
来源：http://blog.fktsv.cn/Article/details/gaqmhmqjx.sHtML

[U29] Py：属性校验
来源：http://wap.sjlbkw.cn/Article/details/gzythypwj.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fktsv.cn/Article/details/gyvpefjpr.sHtML

[U30] Py：数据类
来源：http://baike.yfazqb.com/Article/details/gcivcpraq.sHtML

@dataclass(slots=True)
来源：http://www.share.tarul.cn/Article/details/gcpoisedm.sHtML

[U31] Py：单测
来源：http://blog.sjlbkw.cn/Article/details/glochlqlc.sHtML

python -m pytest -q
来源：http://m.share.fktsv.cn/Article/details/gaeoolrui.sHtML

[U32] Py：代码格式化
来源：http://mobile.tarul.cn/Article/details/gxeyxsuts.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.bbcook.cn/Article/details/gkqthqvxc.sHtML

[U33] Py：打包发布
来源：http://read.share.tarul.cn/Article/details/ggfeffona.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fktsv.cn/Article/details/gbteqjpzv.sHtML

[U34] Py：判断编码
来源：http://blog.epnwcf.com/Article/details/gvjmvrqpo.sHtML

chardet.detect(raw)
来源：http://www.share.bbcook.cn/Article/details/gpvyudxre.sHtML

[U35] Py：发送邮件
来源：http://mobile.yfazqb.com/Article/details/gqwrvuajw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.epnwcf.com/Article/details/gvkfhmymo.sHtML

[U36] Py：定时任务
来源：http://baike.bbcook.cn/Article/details/gyegokjby.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.bbcook.cn/Article/details/gxtmizdry.sHtML

[U37] Py：读写 Excel
来源：http://m.share.bbcook.cn/Article/details/gekfhplft.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.yfazqb.com/Article/details/gpwlemllv.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.tarul.cn/Article/details/gjcdasfuf.sHtML

Path(__file__).resolve().parent
来源：http://read.share.sjlbkw.cn/Article/details/gwqnroniz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.epnwcf.com/Article/details/gnnihbqgq.sHtML

sys.stdout.isatty()
来源：http://www.blog.sjlbkw.cn/Article/details/grnvfuuip.sHtML

[U40] Py：打印到标准错误
来源：http://wap.vehdjk.com/Article/details/gnwmjkeie.sHtML

print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/ggujjagsn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.yfazqb.com/Article/details/gbajsmgna.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.epnwcf.com/Article/details/gmjxthwcf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.tarul.cn/Article/details/gojrwwyfr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.epnwcf.com/Article/details/gwfuiqzfs.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.yfazqb.com/Article/details/gyfwimefp.sHtML

namespace App\Http;
来源：http://www.share.epnwcf.com/Article/details/grnsofdge.sHtML

[U44] PHP：开启严格类型
来源：http://wap.yfazqb.com/Article/details/gfednbvxq.sHtML

declare(strict_types=1);
来源：http://baike.yfazqb.com/Article/details/gprlczlwj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.sjlbkw.cn/Article/details/ghexipneg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gamgzppom.sHtML

[U46] PHP：可空类型
来源：http://m.share.sjlbkw.cn/Article/details/gjtlvinib.sHtML

?string $name = null
来源：http://www.m.share.epnwcf.com/Article/details/gpyobqvkz.sHtML

[U47] PHP：联合类型
来源：http://blog.tarul.cn/Article/details/gmzmmcbim.sHtML

int|string $id
来源：http://mobile.tarul.cn/Article/details/ghqseuope.sHtML

[U48] PHP：纯枚举
来源：http://read.share.epnwcf.com/Article/details/gnnqdfogg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.bbcook.cn/Article/details/ggjsrjxfy.sHtML

[U49] PHP：只读属性
来源：http://blog.fktsv.cn/Article/details/grckyfzey.sHtML

public readonly string $name
来源：http://read.share.tarul.cn/Article/details/gcmyrpscy.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.sjlbkw.cn/Article/details/gubrtybbu.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fktsv.cn/Article/details/grrdmuzdv.sHtML

[U51] PHP：数组解构
来源：http://read.share.tarul.cn/Article/details/gmccxxxwp.sHtML

[$a, $b] = $arr;
来源：http://3g.vehdjk.com/Article/details/gvhgwdfhr.sHtML

[U52] PHP：箭头函数
来源：http://m.share.bbcook.cn/Article/details/gtcmsxcyd.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fktsv.cn/Article/details/geckmhzgn.sHtML

[U53] PHP：空合并运算符
来源：http://3g.epnwcf.com/Article/details/gtiquxhxy.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.sjlbkw.cn/Article/details/ghtitiwur.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fktsv.cn/Article/details/gntmahkjp.sHtML

$obj?->method()
来源：http://www.share.vehdjk.com/Article/details/gioxducrj.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fktsv.cn/Article/details/getamgewm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/gfqyqwhhi.sHtML

[U56] PHP：命名参数
来源：http://read.share.tarul.cn/Article/details/guouruzjk.sHtML

f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gtpfueivj.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gmzlwzaos.sHtML

"值: {$a}"
来源：http://baike.bbcook.cn/Article/details/gyxdxphyt.sHtML

[U58] PHP：数组三件套
来源：http://baike.bbcook.cn/Article/details/gyusudvwn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fktsv.cn/Article/details/gfexgitob.sHtML

[U59] PHP：自定义排序
来源：http://mobile.bbcook.cn/Article/details/gayythbze.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/gtayzdehg.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.epnwcf.com/Article/details/gsmiwjsuk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.epnwcf.com/Article/details/golkmfgwn.sHtML

[U61] PHP：正则
来源：http://www.share.sjlbkw.cn/Article/details/gdhqlvncs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.sjlbkw.cn/Article/details/goucmcowc.sHtML

[U62] PHP：日期对象
来源：http://m.share.vehdjk.com/Article/details/gtndhwqoh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.sjlbkw.cn/Article/details/gatjuvrre.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.tarul.cn/Article/details/ggpfygfik.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fktsv.cn/Article/details/gyirxwyok.sHtML

[U64] PHP：目录遍历
来源：http://wap.fktsv.cn/Article/details/gqrlngjai.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fktsv.cn/Article/details/ghutqhnff.sHtML

[U65] PHP：会话
来源：http://read.share.tarul.cn/Article/details/ggmteffwc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/geqtjgiei.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.sjlbkw.cn/Article/details/ggybdeklb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.vehdjk.com/Article/details/gscrgiigw.sHtML


<!-- 参考信息 -->