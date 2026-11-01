代发 wailian999

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gjlymlmdh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.yfazqb.com/Article/details/gvkrocuro.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fktsv.cn/Article/details/gvytotorx.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.yfazqb.com/Article/details/gavoxifwl.sHtML

[S43] C++：智能指针
来源：http://baike.tarul.cn/Article/details/ghwukemex.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.tarul.cn/Article/details/goppnehwi.sHtML

[S44] C++：引用传参
来源：http://www.m.share.epnwcf.com/Article/details/glnrabffg.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fktsv.cn/Article/details/grrtijaws.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/gepjcleab.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.tarul.cn/Article/details/gsyiniyct.sHtML

[S46] C++：函数模板
来源：http://3g.fktsv.cn/Article/details/gqsphacdv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fktsv.cn/Article/details/gdtwenxhl.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.yfazqb.com/Article/details/gvqkubwuq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.tarul.cn/Article/details/gmunorfba.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gjtxdwrmg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.yfazqb.com/Article/details/ghlnljyoh.sHtML

while (std::getline(in, line)) { }
来源：http://baike.epnwcf.com/Article/details/gkibphsba.sHtML

[S49] C++：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gksdzrmpj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.vehdjk.com/Article/details/gocszcfbc.sHtML

[S50] C++：格式化数字
来源：http://www.blog.sjlbkw.cn/Article/details/gcuvoplqi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.vehdjk.com/Article/details/gtbazhcpn.sHtML

[S51] C++：显式类型转换
来源：http://3g.sjlbkw.cn/Article/details/gsszpmofz.sHtML

static_cast<double>(a) / b
来源：http://3g.epnwcf.com/Article/details/gxqajxqks.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.yfazqb.com/Article/details/gecdohuhx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/gklqtuyui.sHtML

[S53] C++：移动语义
来源：http://www.m.share.epnwcf.com/Article/details/gpbhikvvi.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.sjlbkw.cn/Article/details/gldgncfwo.sHtML

[S54] C++：异常处理
来源：http://mobile.bbcook.cn/Article/details/gprcnncuh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fktsv.cn/Article/details/gurxdpfpa.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/gkdwtxbmk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.vehdjk.com/Article/details/gtexbflzg.sHtML

[S56] C++：optional
来源：http://www.share.bbcook.cn/Article/details/gyxjbenib.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.bbcook.cn/Article/details/gqkqqdfjh.sHtML

[S57] C++：编译期常量
来源：http://wap.sjlbkw.cn/Article/details/gkraingon.sHtML

constexpr int N = 10;
来源：http://read.share.yfazqb.com/Article/details/gelgrgola.sHtML

[S58] C++：命名空间
来源：http://mobile.sjlbkw.cn/Article/details/glqizbuwo.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fktsv.cn/Article/details/gmntuubsx.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/gmplamiwe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.bbcook.cn/Article/details/gtekzkkdt.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.yfazqb.com/Article/details/ghemssujc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fktsv.cn/Article/details/gnffthive.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqbbanuxy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/grxegyvso.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gpjbnyqqx.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/gezpkccwa.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/gnioyawsx.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/gueesorlv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbxxqwdn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fktsv.cn/Article/details/gxnlqcrrj.sHtML

"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gkssrhllt.sHtML

[T04] Kotlin：空安全
来源：http://3g.tarul.cn/Article/details/glysokyat.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.vehdjk.com/Article/details/gbszfaabo.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.yfazqb.com/Article/details/gwrmuvcjd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.bbcook.cn/Article/details/gqztammgs.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fktsv.cn/Article/details/gjqiejptr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/gewegajkl.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.yfazqb.com/Article/details/gtyzehjro.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.bbcook.cn/Article/details/gyulnnnbb.sHtML

[T08] Kotlin：数据类
来源：http://mobile.vehdjk.com/Article/details/goaedngop.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fktsv.cn/Article/details/glbrpbote.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fktsv.cn/Article/details/gqrsjslpm.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.bbcook.cn/Article/details/gpqcisvwu.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gqctfgtnh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.tarul.cn/Article/details/guennjiwu.sHtML

[T11] Kotlin：协程
来源：http://www.blog.epnwcf.com/Article/details/gnvphluus.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.epnwcf.com/Article/details/gpadymqwh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.yfazqb.com/Article/details/gfenmgcuv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gewoxxsde.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.sjlbkw.cn/Article/details/glpmzdiul.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.bbcook.cn/Article/details/gnsdzhqzo.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/grhpwfoad.sHtML

for (i in 1..10) println(i)
来源：http://wap.bbcook.cn/Article/details/gyhdjsumb.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/ggffhnjjv.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fktsv.cn/Article/details/gotkaffko.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gauariyoa.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/geizqolmx.sHtML

[T17] Swift：变量与常量
来源：http://wap.epnwcf.com/Article/details/gircdkhkc.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/gidjskkvr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.tarul.cn/Article/details/gkrfajogf.sHtML

"值: \(b)"
来源：http://3g.fktsv.cn/Article/details/giyskjqto.sHtML

[T19] Swift：可选绑定
来源：http://baike.vehdjk.com/Article/details/gejihogyi.sHtML

if let n = opt { print(n) }
来源：http://www.blog.bbcook.cn/Article/details/gmrcbnsqj.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/gwrppzbov.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.vehdjk.com/Article/details/gxolgsibz.sHtML

[T21] Swift：遍历
来源：http://baike.yfazqb.com/Article/details/grwgvplkt.sHtML

for x in a { print(x) }
来源：http://www.m.share.bbcook.cn/Article/details/gbaukyfch.sHtML

[T22] Swift：字典
来源：http://m.share.vehdjk.com/Article/details/gjpytjvxs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fktsv.cn/Article/details/ghbnpnslj.sHtML

[T23] Swift：函数
来源：http://mobile.vehdjk.com/Article/details/gbfddokto.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.tarul.cn/Article/details/gvkptxdbw.sHtML

[T24] Swift：闭包
来源：http://blog.tarul.cn/Article/details/gluptvnyo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gczwdyeoj.sHtML

[T25] Swift：结构体
来源：http://www.blog.tarul.cn/Article/details/gccadzdbw.sHtML

struct P { var x: Int }
来源：http://www.share.bbcook.cn/Article/details/gtujwtiqa.sHtML

[T26] Swift：类与重写
来源：http://wap.epnwcf.com/Article/details/gekkjqnvn.sHtML

class A: Base { override func f() {} }
来源：http://m.share.bbcook.cn/Article/details/ggbzvihpg.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/gzgqiwcoo.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fktsv.cn/Article/details/gzoasidtt.sHtML

[T28] Swift：枚举
来源：http://www.share.yfazqb.com/Article/details/gubdkryio.sHtML

enum Color { case red, green }
来源：http://www.m.share.vehdjk.com/Article/details/gllsigmnz.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.tarul.cn/Article/details/geqtylkkz.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gpeqcxrwg.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/glfghwtwz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gthjospqf.sHtML

[T31] Lua：Hello World
来源：http://read.share.tarul.cn/Article/details/gdbqzjdei.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gnbjyqgxp.sHtML

[T32] Lua：局部变量
来源：http://www.share.yfazqb.com/Article/details/gaigzrozv.sHtML

local a = 1
来源：http://www.m.share.bbcook.cn/Article/details/gdmljrcyb.sHtML

[T33] Lua：表（数组）
来源：http://mobile.yfazqb.com/Article/details/gjjllhjpi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.bbcook.cn/Article/details/gwnsbnvat.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/gldzrgqpl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.sjlbkw.cn/Article/details/gvwsshxie.sHtML

[T35] Lua：字典表
来源：http://www.m.share.bbcook.cn/Article/details/gtxevupav.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.vehdjk.com/Article/details/gjdeawgno.sHtML

[T36] Lua：函数
来源：http://m.share.fktsv.cn/Article/details/gguvudnix.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.tarul.cn/Article/details/gwzpxqcbz.sHtML

[T37] Lua：字符串拼接
来源：http://baike.bbcook.cn/Article/details/gbulmxsub.sHtML

"a" .. "b"
来源：http://blog.vehdjk.com/Article/details/gwbjrkmyx.sHtML

[T38] Lua：条件
来源：http://baike.bbcook.cn/Article/details/gfvtgleaq.sHtML

if x > 0 then print("正") end
来源：http://baike.vehdjk.com/Article/details/gpmuhgtyw.sHtML

[T39] Lua：模式匹配
来源：http://baike.fktsv.cn/Article/details/gtzukdwbc.sHtML

string.find(s, "%d+")
来源：http://mobile.epnwcf.com/Article/details/gbgcwnauh.sHtML

[T40] Lua：元表
来源：http://m.share.sjlbkw.cn/Article/details/gwwwxuldf.sHtML

setmetatable({}, { __index = base })
来源：http://baike.epnwcf.com/Article/details/gtoudrohw.sHtML

[T41] Perl：Hello World
来源：http://read.share.tarul.cn/Article/details/gsnfyacfy.sHtML

print "Hello\n";
来源：http://read.share.fktsv.cn/Article/details/gjyarbsun.sHtML

[T42] Perl：变量类型
来源：http://www.share.bbcook.cn/Article/details/gclazubxj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.tarul.cn/Article/details/grytilhcb.sHtML

[T43] Perl：字符串插值
来源：http://mobile.vehdjk.com/Article/details/glmpskgnm.sHtML

"值: $a"
来源：http://read.share.sjlbkw.cn/Article/details/gpcgdiazd.sHtML

[T44] Perl：条件
来源：http://baike.bbcook.cn/Article/details/glmhacfzv.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fktsv.cn/Article/details/gbenxbanx.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.epnwcf.com/Article/details/gzddtaiwl.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.yfazqb.com/Article/details/goywtrfay.sHtML

[T46] Perl：哈希操作
来源：http://baike.fktsv.cn/Article/details/glbpduhov.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/gfrvmxomq.sHtML

[T47] Perl：正则捕获
来源：http://mobile.vehdjk.com/Article/details/gqcvsbdnx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.sjlbkw.cn/Article/details/gyxkrsldt.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/grsylckjx.sHtML

$s =~ s/old/new/g;
来源：http://read.share.vehdjk.com/Article/details/gpsyhvunl.sHtML

[T49] Perl：函数
来源：http://read.share.sjlbkw.cn/Article/details/grsbrfqod.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gphpukdty.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gilbyytvy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/gqkmptaiv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.sjlbkw.cn/Article/details/grutvvseq.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gyxokxcwe.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/glshmxqkw.sHtML

[T52] Scala：变量
来源：http://wap.bbcook.cn/Article/details/gztmqggcp.sHtML

val a = 1;  var b = 2
来源：http://blog.fktsv.cn/Article/details/gadhhfqgw.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gajthaunu.sHtML

s"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/gspqzmaxu.sHtML

[T54] Scala：集合映射
来源：http://baike.bbcook.cn/Article/details/gsrcaeekv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.bbcook.cn/Article/details/gttausjat.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gyqzcldkz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fktsv.cn/Article/details/geqjsqsmz.sHtML

[T56] Scala：样例类
来源：http://baike.tarul.cn/Article/details/gslwgyrke.sHtML

case class User(name: String, age: Int)
来源：http://wap.yfazqb.com/Article/details/gryfcmpws.sHtML

[T57] Scala：模式匹配
来源：http://m.share.tarul.cn/Article/details/gvvdsvrum.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.vehdjk.com/Article/details/gwnfntcaf.sHtML

[T58] Scala：函数定义
来源：http://wap.tarul.cn/Article/details/gnbnywtyx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.vehdjk.com/Article/details/geptbqbzd.sHtML

[T59] Scala：循环
来源：http://read.share.fktsv.cn/Article/details/gxvhotmxt.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gpjoxudhy.sHtML

[T60] Scala：折叠
来源：http://3g.bbcook.cn/Article/details/gvibqjnpg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.sjlbkw.cn/Article/details/gxuegbkbr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvstughsp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.sjlbkw.cn/Article/details/gvonhjcja.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gsyeejeek.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.tarul.cn/Article/details/grkgsxllt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.bbcook.cn/Article/details/gdvsbhepm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.yfazqb.com/Article/details/gwarjwmzw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.sjlbkw.cn/Article/details/gapwxseai.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.yfazqb.com/Article/details/gkqlebawo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.bbcook.cn/Article/details/gamlqvdxw.sHtML

[U04] Py：变量调试打印
来源：http://blog.sjlbkw.cn/Article/details/gwghmyupx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.vehdjk.com/Article/details/gvbqgzqbd.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.bbcook.cn/Article/details/gxsuxvwsi.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.epnwcf.com/Article/details/gsnfklrdg.sHtML

[U06] Py：合并两个字典
来源：http://3g.sjlbkw.cn/Article/details/gsndgqfuz.sHtML

{**a, **b}
来源：http://read.share.sjlbkw.cn/Article/details/gpvzaseee.sHtML

[U07] Py：反转字典键值
来源：http://blog.yfazqb.com/Article/details/gtjowvobw.sHtML

{v: k for k, v in d.items()}
来源：http://baike.yfazqb.com/Article/details/gwglwnnjg.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fktsv.cn/Article/details/gxjcokvfk.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gwtauhspn.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.vehdjk.com/Article/details/gpmjkxyll.sHtML

max(d, key=d.get)
来源：http://m.share.bbcook.cn/Article/details/grkmczlpv.sHtML

[U10] Py：按值排序字典
来源：http://3g.epnwcf.com/Article/details/gvvxipmoi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.epnwcf.com/Article/details/gagudlbff.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gspyhyrvd.sHtML

(x * 2 for x in arr)
来源：http://read.share.bbcook.cn/Article/details/gzvwwetrz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.bbcook.cn/Article/details/gczldbqje.sHtML

Counter(arr).most_common(3)
来源：http://baike.yfazqb.com/Article/details/gorlyrquq.sHtML

[U13] Py：固定长度队列
来源：http://m.share.tarul.cn/Article/details/gubxjoism.sHtML

deque(maxlen=10)
来源：http://blog.sjlbkw.cn/Article/details/gdukjqweo.sHtML

[U14] Py：分组收集到列表
来源：http://3g.sjlbkw.cn/Article/details/gshzapvvb.sHtML

defaultdict(list)
来源：http://blog.bbcook.cn/Article/details/gpucqbijv.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.sjlbkw.cn/Article/details/gzozqcxin.sHtML

t = time.perf_counter()
来源：http://mobile.bbcook.cn/Article/details/gqykcegge.sHtML

[U16] Py：命令行参数解析
来源：http://3g.epnwcf.com/Article/details/gfngwmaqk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.epnwcf.com/Article/details/gcpynyzns.sHtML

[U17] Py：初始化日志
来源：http://m.share.yfazqb.com/Article/details/gfingzqit.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.tarul.cn/Article/details/gufwkgvbc.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fktsv.cn/Article/details/gnlzxwflh.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.vehdjk.com/Article/details/ggxwaroks.sHtML

[U19] Py：正则替换带回调
来源：http://baike.bbcook.cn/Article/details/gkhqtreue.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.yfazqb.com/Article/details/gvzcufgpg.sHtML

[U20] Py：缓存函数结果
来源：http://baike.bbcook.cn/Article/details/gwpxnfdwh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.epnwcf.com/Article/details/gcarwxtad.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.sjlbkw.cn/Article/details/gyestypxs.sHtML

@contextlib.contextmanager
来源：http://blog.epnwcf.com/Article/details/gxhajmfgi.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.tarul.cn/Article/details/gcwmeezce.sHtML

list(zip(*m))
来源：http://blog.tarul.cn/Article/details/grvahmebq.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.epnwcf.com/Article/details/gxzwsiois.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.yfazqb.com/Article/details/getyeqtrj.sHtML

[U24] Py：路径操作
来源：http://www.share.yfazqb.com/Article/details/gfpcxlrcb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gldfyyuwg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.vehdjk.com/Article/details/gxqqhpyox.sHtML

csv.DictReader(f)
来源：http://3g.fktsv.cn/Article/details/gfittxmsu.sHtML

[U26] Py：并发下载
来源：http://m.share.bbcook.cn/Article/details/gisbccmjk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fktsv.cn/Article/details/gapwjyodf.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.bbcook.cn/Article/details/gtikrbhga.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.vehdjk.com/Article/details/gpcziypoz.sHtML

[U28] Py：类型别名
来源：http://mobile.bbcook.cn/Article/details/gbfmwoeja.sHtML

UserId = int
来源：http://www.share.tarul.cn/Article/details/gsdksfstg.sHtML

[U29] Py：属性校验
来源：http://blog.yfazqb.com/Article/details/gsdgotvko.sHtML

@property 与 @x.setter 配合
来源：http://3g.tarul.cn/Article/details/guxpnbdcs.sHtML

[U30] Py：数据类
来源：http://www.m.share.epnwcf.com/Article/details/grhbjomeu.sHtML

@dataclass(slots=True)
来源：http://m.share.tarul.cn/Article/details/gjgpiqbzb.sHtML

[U31] Py：单测
来源：http://read.share.fktsv.cn/Article/details/gbcrfvxxb.sHtML

python -m pytest -q
来源：http://3g.epnwcf.com/Article/details/geqzrlcqi.sHtML

[U32] Py：代码格式化
来源：http://www.blog.tarul.cn/Article/details/giruifril.sHtML

ruff format . && ruff check --fix .
来源：http://baike.vehdjk.com/Article/details/gnidofcqp.sHtML

[U33] Py：打包发布
来源：http://www.m.share.yfazqb.com/Article/details/gvfenycek.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.yfazqb.com/Article/details/gpausvefw.sHtML

[U34] Py：判断编码
来源：http://m.share.sjlbkw.cn/Article/details/gdjhqlffw.sHtML

chardet.detect(raw)
来源：http://wap.bbcook.cn/Article/details/gfmhiecmd.sHtML

[U35] Py：发送邮件
来源：http://mobile.sjlbkw.cn/Article/details/gxjwcgjzj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.yfazqb.com/Article/details/gxerqgyeh.sHtML

[U36] Py：定时任务
来源：http://mobile.epnwcf.com/Article/details/gftrirgij.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.epnwcf.com/Article/details/gejttajfq.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fktsv.cn/Article/details/gfsgwnnzd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.bbcook.cn/Article/details/gdirdlnxz.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.sjlbkw.cn/Article/details/ggyccmynl.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fktsv.cn/Article/details/gblltupcu.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.sjlbkw.cn/Article/details/gjiutgfhl.sHtML

sys.stdout.isatty()
来源：http://www.share.vehdjk.com/Article/details/gqfhaimst.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.bbcook.cn/Article/details/gxaoylded.sHtML

print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/ggrbxxnih.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.bbcook.cn/Article/details/gvpghriqu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.sjlbkw.cn/Article/details/glxllwfer.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.tarul.cn/Article/details/gyjzzcxio.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fktsv.cn/Article/details/ggwzkzcsx.sHtML

[U43] PHP：声明命名空间
来源：http://3g.vehdjk.com/Article/details/gdvzdhgzg.sHtML

namespace App\Http;
来源：http://blog.bbcook.cn/Article/details/gcmdkuhxe.sHtML

[U44] PHP：开启严格类型
来源：http://blog.tarul.cn/Article/details/gdgnlxtxv.sHtML

declare(strict_types=1);
来源：http://www.share.vehdjk.com/Article/details/gauqdecgq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.sjlbkw.cn/Article/details/gkyuctgwl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/guswhgefq.sHtML

[U46] PHP：可空类型
来源：http://read.share.sjlbkw.cn/Article/details/gkjjxahin.sHtML

?string $name = null
来源：http://mobile.vehdjk.com/Article/details/ghkxvqllk.sHtML

[U47] PHP：联合类型
来源：http://3g.vehdjk.com/Article/details/gbkbqwqnk.sHtML

int|string $id
来源：http://3g.epnwcf.com/Article/details/gyrbccufu.sHtML

[U48] PHP：纯枚举
来源：http://3g.sjlbkw.cn/Article/details/gdcviabrt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.vehdjk.com/Article/details/gdbydyoni.sHtML

[U49] PHP：只读属性
来源：http://baike.bbcook.cn/Article/details/gthtyvbaf.sHtML

public readonly string $name
来源：http://mobile.tarul.cn/Article/details/gvhceublj.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fktsv.cn/Article/details/gvgyaptao.sHtML

public function __construct(private int $id) {}
来源：http://www.share.sjlbkw.cn/Article/details/gizggveia.sHtML

[U51] PHP：数组解构
来源：http://baike.fktsv.cn/Article/details/gwjuqmqjd.sHtML

[$a, $b] = $arr;
来源：http://read.share.fktsv.cn/Article/details/gonbvmdba.sHtML

[U52] PHP：箭头函数
来源：http://www.share.epnwcf.com/Article/details/gtvjuuljc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fktsv.cn/Article/details/gkvnudtqq.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.tarul.cn/Article/details/gknorbxoi.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.bbcook.cn/Article/details/gotlojrwr.sHtML

[U54] PHP：空安全调用
来源：http://blog.epnwcf.com/Article/details/giinishfj.sHtML

$obj?->method()
来源：http://www.blog.epnwcf.com/Article/details/gzbbearpz.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvxyptok.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.bbcook.cn/Article/details/ggpgsgige.sHtML

[U56] PHP：命名参数
来源：http://wap.tarul.cn/Article/details/gzlhcokbv.sHtML

f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gagfcgoeu.sHtML

[U57] PHP：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/ghtvugwwd.sHtML

"值: {$a}"
来源：http://www.m.share.yfazqb.com/Article/details/gvxtzchut.sHtML

[U58] PHP：数组三件套
来源：http://www.share.vehdjk.com/Article/details/gdaebaszi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.epnwcf.com/Article/details/gackapndk.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fktsv.cn/Article/details/goqshgecd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.tarul.cn/Article/details/gspgkzyfs.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.bbcook.cn/Article/details/gvidhvodu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.epnwcf.com/Article/details/gpfnxryxe.sHtML

[U61] PHP：正则
来源：http://www.blog.tarul.cn/Article/details/gorssfwec.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/glckbtwzf.sHtML

[U62] PHP：日期对象
来源：http://www.share.bbcook.cn/Article/details/ggjfxppmw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.bbcook.cn/Article/details/ggoediebh.sHtML

[U63] PHP：文件读写
来源：http://mobile.tarul.cn/Article/details/gqkuiidwz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.tarul.cn/Article/details/gqtxklrtg.sHtML

[U64] PHP：目录遍历
来源：http://m.share.tarul.cn/Article/details/ghsbmokao.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fktsv.cn/Article/details/gdjudciyn.sHtML

[U65] PHP：会话
来源：http://3g.fktsv.cn/Article/details/gnrphmiwt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fktsv.cn/Article/details/gtvzxxyhq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.sjlbkw.cn/Article/details/gpfyoftfs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.yfazqb.com/Article/details/gyycjbrbh.sHtML


<!-- 参考信息 -->