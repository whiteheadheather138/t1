代发 wailian999

[S41] C++：类与构造函数
来源：http://www.share.bbcook.cn/Article/details/guqvxbhma.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.vehdjk.com/Article/details/ghxdeyaut.sHtML

[S42] C++：继承与虚函数
来源：http://baike.vehdjk.com/Article/details/gcfhbobii.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.bbcook.cn/Article/details/gllykhneu.sHtML

[S43] C++：智能指针
来源：http://blog.tarul.cn/Article/details/gedevockv.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.sjlbkw.cn/Article/details/gtdkqohfw.sHtML

[S44] C++：引用传参
来源：http://www.blog.fktsv.cn/Article/details/gybkuljto.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fktsv.cn/Article/details/gtdkmqztz.sHtML

[S45] C++：lambda
来源：http://mobile.sjlbkw.cn/Article/details/ghzhkfues.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.sjlbkw.cn/Article/details/gattxzngs.sHtML

[S46] C++：函数模板
来源：http://www.share.fktsv.cn/Article/details/gpczyxbpj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.bbcook.cn/Article/details/ghjtascax.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/grnaubedm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.sjlbkw.cn/Article/details/gzrwtvbea.sHtML

[S48] C++：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gfqmrvbaa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.epnwcf.com/Article/details/giunnfesk.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fktsv.cn/Article/details/gfcknxank.sHtML

[S49] C++：写文件
来源：http://blog.vehdjk.com/Article/details/gnxggeezt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.epnwcf.com/Article/details/gwhclhffx.sHtML

[S50] C++：格式化数字
来源：http://www.blog.tarul.cn/Article/details/gsqqdxzyc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gcnpmjqoi.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fktsv.cn/Article/details/gutsodkmu.sHtML

static_cast<double>(a) / b
来源：http://www.share.bbcook.cn/Article/details/gvwrocans.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/gtsabgetl.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/gcbsrwzxh.sHtML

[S53] C++：移动语义
来源：http://m.share.fktsv.cn/Article/details/gxesksgcz.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/gglqpgqns.sHtML

[S54] C++：异常处理
来源：http://blog.fktsv.cn/Article/details/gtotqektj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.epnwcf.com/Article/details/gljwcvxtt.sHtML

[S55] C++：结构化绑定
来源：http://www.share.vehdjk.com/Article/details/gzmhqywga.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gpuscihis.sHtML

[S56] C++：optional
来源：http://mobile.epnwcf.com/Article/details/gltsgjnud.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/grfvzacnx.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/gaeohaxdn.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/gmpbztgxb.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gnpgfadkp.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.yfazqb.com/Article/details/gehbdyvjx.sHtML

[S59] C++：静态断言
来源：http://blog.yfazqb.com/Article/details/gcqgupwhi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/ghvnugkqv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fktsv.cn/Article/details/glqtlrqse.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/gkfhjpfkj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqyefyspx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/grttfuwwo.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gniqcjsgj.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gpareeifg.sHtML

println("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gghbrqqsw.sHtML

[T02] Kotlin：变量
来源：http://www.share.sjlbkw.cn/Article/details/gqsbikoki.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.yfazqb.com/Article/details/glbjltgpu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/gldhejopo.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gueilepxr.sHtML

[T04] Kotlin：空安全
来源：http://mobile.epnwcf.com/Article/details/gzasviflh.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fktsv.cn/Article/details/gwgcmfuel.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.yfazqb.com/Article/details/gpxvbjztn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fktsv.cn/Article/details/gphjcrnnh.sHtML

[T06] Kotlin：集合映射
来源：http://wap.bbcook.cn/Article/details/gwyggyzzf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gglbxvlfr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gikdercls.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.yfazqb.com/Article/details/gtksqgadg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.bbcook.cn/Article/details/gotfmxnuy.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.epnwcf.com/Article/details/gbkuhahcg.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.bbcook.cn/Article/details/gonwqjunz.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.yfazqb.com/Article/details/ggthnkxox.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.vehdjk.com/Article/details/gvnejhryp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.epnwcf.com/Article/details/giafmswyg.sHtML

[T11] Kotlin：协程
来源：http://m.share.yfazqb.com/Article/details/gforoxolv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.tarul.cn/Article/details/gmdgqlbom.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.sjlbkw.cn/Article/details/gnvmzlhun.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.bbcook.cn/Article/details/ggvzxeara.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/gwvfzuxak.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.vehdjk.com/Article/details/gztrbjxin.sHtML

[T14] Kotlin：循环
来源：http://3g.epnwcf.com/Article/details/gkvwwsdco.sHtML

for (i in 1..10) println(i)
来源：http://blog.fktsv.cn/Article/details/grcvhyeks.sHtML

[T15] Kotlin：接口
来源：http://wap.epnwcf.com/Article/details/gszkkqjxe.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.tarul.cn/Article/details/gvimticgu.sHtML

[T16] Swift：Hello World
来源：http://baike.bbcook.cn/Article/details/gvvrdidyn.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gskatmwss.sHtML

[T17] Swift：变量与常量
来源：http://wap.yfazqb.com/Article/details/grqmjydxv.sHtML

var a = 1;  let b = 2
来源：http://www.share.fktsv.cn/Article/details/gdiooazfj.sHtML

[T18] Swift：字符串插值
来源：http://3g.yfazqb.com/Article/details/gplcdxcei.sHtML

"值: \(b)"
来源：http://wap.bbcook.cn/Article/details/gecmwjcmw.sHtML

[T19] Swift：可选绑定
来源：http://mobile.sjlbkw.cn/Article/details/gndjtenpa.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/gezkivoja.sHtML

[T20] Swift：数组操作
来源：http://wap.sjlbkw.cn/Article/details/gcgiqjbbz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.tarul.cn/Article/details/gsfnittvk.sHtML

[T21] Swift：遍历
来源：http://www.m.share.yfazqb.com/Article/details/gqelzbskr.sHtML

for x in a { print(x) }
来源：http://www.share.bbcook.cn/Article/details/grnxadoex.sHtML

[T22] Swift：字典
来源：http://mobile.tarul.cn/Article/details/goyfwmfli.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.bbcook.cn/Article/details/gxqhemrdb.sHtML

[T23] Swift：函数
来源：http://read.share.tarul.cn/Article/details/gfpvekonw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gkakamabi.sHtML

[T24] Swift：闭包
来源：http://baike.vehdjk.com/Article/details/gkvupoqeg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gbxugciym.sHtML

[T25] Swift：结构体
来源：http://www.share.yfazqb.com/Article/details/giawmqldn.sHtML

struct P { var x: Int }
来源：http://mobile.sjlbkw.cn/Article/details/grbzqywzm.sHtML

[T26] Swift：类与重写
来源：http://read.share.sjlbkw.cn/Article/details/ghaqjcykt.sHtML

class A: Base { override func f() {} }
来源：http://3g.sjlbkw.cn/Article/details/glhlawefh.sHtML

[T27] Swift：错误处理
来源：http://3g.epnwcf.com/Article/details/gyozlhplt.sHtML

do { try f() } catch { print(error) }
来源：http://wap.vehdjk.com/Article/details/gqzroelsl.sHtML

[T28] Swift：枚举
来源：http://blog.vehdjk.com/Article/details/gfzrsmglz.sHtML

enum Color { case red, green }
来源：http://3g.bbcook.cn/Article/details/gpscsebtm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fktsv.cn/Article/details/glmzoxcwy.sHtML

guard let x = opt else { return }
来源：http://3g.fktsv.cn/Article/details/gjvrlccpw.sHtML

[T30] Swift：协议
来源：http://read.share.sjlbkw.cn/Article/details/gmjxkctel.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.epnwcf.com/Article/details/grlwidudg.sHtML

[T31] Lua：Hello World
来源：http://www.share.fktsv.cn/Article/details/guhnyvwgf.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gwjetmrlg.sHtML

[T32] Lua：局部变量
来源：http://3g.epnwcf.com/Article/details/gfrfwpsut.sHtML

local a = 1
来源：http://mobile.fktsv.cn/Article/details/gtdemuotz.sHtML

[T33] Lua：表（数组）
来源：http://mobile.vehdjk.com/Article/details/ghgnhsnll.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.yfazqb.com/Article/details/gzdxwhsrl.sHtML

[T34] Lua：遍历表
来源：http://m.share.bbcook.cn/Article/details/gsnxxtkhi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/gdiwpxzrd.sHtML

[T35] Lua：字典表
来源：http://3g.sjlbkw.cn/Article/details/gbdcryuac.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.sjlbkw.cn/Article/details/gbhbdvilo.sHtML

[T36] Lua：函数
来源：http://mobile.sjlbkw.cn/Article/details/gbdijjxnq.sHtML

function add(a, b) return a + b end
来源：http://baike.yfazqb.com/Article/details/gfcznjzhu.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gnfmwyutp.sHtML

"a" .. "b"
来源：http://read.share.epnwcf.com/Article/details/godwbyqtc.sHtML

[T38] Lua：条件
来源：http://m.share.epnwcf.com/Article/details/gtmksvbzu.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/gzlbvvgip.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.tarul.cn/Article/details/gbfsvntju.sHtML

string.find(s, "%d+")
来源：http://m.share.sjlbkw.cn/Article/details/gocleyicq.sHtML

[T40] Lua：元表
来源：http://mobile.tarul.cn/Article/details/grdjyyigg.sHtML

setmetatable({}, { __index = base })
来源：http://baike.tarul.cn/Article/details/gbbqpphtp.sHtML

[T41] Perl：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/grpxlqhxj.sHtML

print "Hello\n";
来源：http://blog.tarul.cn/Article/details/gkoggbzyn.sHtML

[T42] Perl：变量类型
来源：http://www.blog.yfazqb.com/Article/details/gmhqqscgs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.yfazqb.com/Article/details/giiyorzyu.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gqmcuhnzj.sHtML

"值: $a"
来源：http://www.m.share.yfazqb.com/Article/details/ghkggsvtl.sHtML

[T44] Perl：条件
来源：http://blog.tarul.cn/Article/details/gonetbugo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/gxyewkkbb.sHtML

[T45] Perl：数组遍历
来源：http://read.share.epnwcf.com/Article/details/gthvoogyt.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.vehdjk.com/Article/details/goatekfej.sHtML

[T46] Perl：哈希操作
来源：http://m.share.yfazqb.com/Article/details/gjunzipsp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gabrzonjs.sHtML

[T47] Perl：正则捕获
来源：http://wap.tarul.cn/Article/details/gsnttutxg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.bbcook.cn/Article/details/glafrnspw.sHtML

[T48] Perl：正则替换
来源：http://baike.tarul.cn/Article/details/ghfdcovpk.sHtML

$s =~ s/old/new/g;
来源：http://baike.tarul.cn/Article/details/gzsynjhye.sHtML

[T49] Perl：函数
来源：http://wap.vehdjk.com/Article/details/gizdlnwns.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gwnqzkens.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/ghjjejkyj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.vehdjk.com/Article/details/gsfkyvglr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.vehdjk.com/Article/details/giebsjetb.sHtML

[T51] Scala：Hello World
来源：http://m.share.epnwcf.com/Article/details/ggqrzfzck.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/ghwgjntfi.sHtML

[T52] Scala：变量
来源：http://m.share.vehdjk.com/Article/details/gcbtwfcrj.sHtML

val a = 1;  var b = 2
来源：http://baike.bbcook.cn/Article/details/gvzkhyawd.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gdlerpcxf.sHtML

s"值: $b"
来源：http://blog.yfazqb.com/Article/details/gjuxeoalo.sHtML

[T54] Scala：集合映射
来源：http://read.share.tarul.cn/Article/details/glpgqqfjo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.bbcook.cn/Article/details/gqqafcgop.sHtML

[T55] Scala：集合过滤
来源：http://blog.epnwcf.com/Article/details/gxeyyuole.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.yfazqb.com/Article/details/gtmkqqlse.sHtML

[T56] Scala：样例类
来源：http://blog.yfazqb.com/Article/details/gjwkhotmr.sHtML

case class User(name: String, age: Int)
来源：http://www.share.epnwcf.com/Article/details/gjzoplbam.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/gdyyqawgg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.bbcook.cn/Article/details/gdyevwlqf.sHtML

[T58] Scala：函数定义
来源：http://blog.fktsv.cn/Article/details/gabxxypid.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fktsv.cn/Article/details/gscspswhu.sHtML

[T59] Scala：循环
来源：http://baike.yfazqb.com/Article/details/goiwupfck.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.vehdjk.com/Article/details/ggyetqqdi.sHtML

[T60] Scala：折叠
来源：http://www.blog.epnwcf.com/Article/details/gwhafgvbm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.epnwcf.com/Article/details/gxicylqrq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/graztzjpa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.tarul.cn/Article/details/gwgfirskj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqxkiihiv.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.epnwcf.com/Article/details/gtpjrhuur.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.yfazqb.com/Article/details/gwnuhztxb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.bbcook.cn/Article/details/godnuszkj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.sjlbkw.cn/Article/details/ghihuufxe.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.yfazqb.com/Article/details/guckmitxh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fktsv.cn/Article/details/gpigwymbi.sHtML

[U04] Py：变量调试打印
来源：http://blog.tarul.cn/Article/details/gpylaqcyl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.sjlbkw.cn/Article/details/gopnvfawo.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.tarul.cn/Article/details/gnirpithn.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/gceiicmay.sHtML

[U06] Py：合并两个字典
来源：http://m.share.bbcook.cn/Article/details/gljhprdks.sHtML

{**a, **b}
来源：http://wap.tarul.cn/Article/details/genswkfcy.sHtML

[U07] Py：反转字典键值
来源：http://blog.vehdjk.com/Article/details/ghyswynbu.sHtML

{v: k for k, v in d.items()}
来源：http://blog.tarul.cn/Article/details/gpjjluiqm.sHtML

[U08] Py：展平二维列表
来源：http://baike.sjlbkw.cn/Article/details/gznxcnkai.sHtML

[y for x in nested for y in x]
来源：http://www.share.epnwcf.com/Article/details/garphccuw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.vehdjk.com/Article/details/gtxncepro.sHtML

max(d, key=d.get)
来源：http://baike.bbcook.cn/Article/details/gzqxnkbkr.sHtML

[U10] Py：按值排序字典
来源：http://blog.vehdjk.com/Article/details/gxncrqvhc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.epnwcf.com/Article/details/gprgzspke.sHtML

[U11] Py：生成器表达式
来源：http://wap.epnwcf.com/Article/details/gvrmjxydw.sHtML

(x * 2 for x in arr)
来源：http://baike.sjlbkw.cn/Article/details/gfvodwifc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.bbcook.cn/Article/details/gvxuuoize.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gaaqvsoen.sHtML

[U13] Py：固定长度队列
来源：http://blog.tarul.cn/Article/details/gvfciskwg.sHtML

deque(maxlen=10)
来源：http://read.share.tarul.cn/Article/details/ghmnriqty.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.vehdjk.com/Article/details/gxfcpyzsp.sHtML

defaultdict(list)
来源：http://blog.epnwcf.com/Article/details/ghenxwupo.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.vehdjk.com/Article/details/guukkkqjz.sHtML

t = time.perf_counter()
来源：http://blog.epnwcf.com/Article/details/gvhjujhgr.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.tarul.cn/Article/details/gtmevhmux.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.yfazqb.com/Article/details/gagqhlepi.sHtML

[U17] Py：初始化日志
来源：http://read.share.epnwcf.com/Article/details/gvkvjvdmw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.epnwcf.com/Article/details/gstaietpf.sHtML

[U18] Py：预编译正则
来源：http://mobile.yfazqb.com/Article/details/gohgmlaau.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.tarul.cn/Article/details/gamypbmva.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fktsv.cn/Article/details/gyaoxlasf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fktsv.cn/Article/details/gfevongng.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.bbcook.cn/Article/details/guigqyljp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.bbcook.cn/Article/details/gkxspihiy.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.sjlbkw.cn/Article/details/ggdfftzyp.sHtML

@contextlib.contextmanager
来源：http://baike.sjlbkw.cn/Article/details/grandwiym.sHtML

[U22] Py：矩阵转置
来源：http://www.share.bbcook.cn/Article/details/gebdnstfz.sHtML

list(zip(*m))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpziatcf.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.yfazqb.com/Article/details/ghuetrvti.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.yfazqb.com/Article/details/gqecydhrb.sHtML

[U24] Py：路径操作
来源：http://baike.epnwcf.com/Article/details/gecluckkw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/glrbyqqhm.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.tarul.cn/Article/details/gufoanrje.sHtML

csv.DictReader(f)
来源：http://mobile.tarul.cn/Article/details/ghpzusuew.sHtML

[U26] Py：并发下载
来源：http://baike.yfazqb.com/Article/details/gnjeyraxx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.bbcook.cn/Article/details/glwiflgjx.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.yfazqb.com/Article/details/gzqbkurgb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.yfazqb.com/Article/details/ghonqjaxb.sHtML

[U28] Py：类型别名
来源：http://3g.tarul.cn/Article/details/gxqerrllp.sHtML

UserId = int
来源：http://3g.yfazqb.com/Article/details/ggaadqzqm.sHtML

[U29] Py：属性校验
来源：http://blog.bbcook.cn/Article/details/gjizgikdh.sHtML

@property 与 @x.setter 配合
来源：http://blog.bbcook.cn/Article/details/gajzzbdds.sHtML

[U30] Py：数据类
来源：http://www.share.fktsv.cn/Article/details/gdritlpzl.sHtML

@dataclass(slots=True)
来源：http://baike.vehdjk.com/Article/details/goignstiz.sHtML

[U31] Py：单测
来源：http://baike.epnwcf.com/Article/details/gbrolabzc.sHtML

python -m pytest -q
来源：http://www.blog.epnwcf.com/Article/details/gomjgopzo.sHtML

[U32] Py：代码格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gktjxvxbb.sHtML

ruff format . && ruff check --fix .
来源：http://3g.bbcook.cn/Article/details/godmvccke.sHtML

[U33] Py：打包发布
来源：http://read.share.fktsv.cn/Article/details/gxuijnfwf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.sjlbkw.cn/Article/details/gznmqjhex.sHtML

[U34] Py：判断编码
来源：http://www.blog.vehdjk.com/Article/details/grwyozzpp.sHtML

chardet.detect(raw)
来源：http://mobile.yfazqb.com/Article/details/gfcenwzea.sHtML

[U35] Py：发送邮件
来源：http://3g.epnwcf.com/Article/details/gjdrfmupq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.vehdjk.com/Article/details/glyoozuoq.sHtML

[U36] Py：定时任务
来源：http://mobile.yfazqb.com/Article/details/gxaqanbty.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.epnwcf.com/Article/details/gwxndhgcc.sHtML

[U37] Py：读写 Excel
来源：http://www.share.vehdjk.com/Article/details/gxfvytnyk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.vehdjk.com/Article/details/gobhokpxb.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.epnwcf.com/Article/details/gdqlndeip.sHtML

Path(__file__).resolve().parent
来源：http://mobile.yfazqb.com/Article/details/gxersiqhu.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.sjlbkw.cn/Article/details/gkysclyae.sHtML

sys.stdout.isatty()
来源：http://www.blog.vehdjk.com/Article/details/gcsmhdepn.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.tarul.cn/Article/details/gdmthhxwx.sHtML

print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/gxfqovrux.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.sjlbkw.cn/Article/details/gseedkmec.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.yfazqb.com/Article/details/goodzcyiu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.tarul.cn/Article/details/gogkrlkqg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.bbcook.cn/Article/details/giewzadac.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.epnwcf.com/Article/details/gntwoffyq.sHtML

namespace App\Http;
来源：http://3g.epnwcf.com/Article/details/ggnkhlald.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.vehdjk.com/Article/details/gmtqlqcnp.sHtML

declare(strict_types=1);
来源：http://www.blog.tarul.cn/Article/details/gysvltftz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.tarul.cn/Article/details/gnjtxaldk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/grqekcwvp.sHtML

[U46] PHP：可空类型
来源：http://wap.bbcook.cn/Article/details/gfhbnocfi.sHtML

?string $name = null
来源：http://3g.epnwcf.com/Article/details/grfmmconk.sHtML

[U47] PHP：联合类型
来源：http://wap.sjlbkw.cn/Article/details/gwmavdskh.sHtML

int|string $id
来源：http://www.share.fktsv.cn/Article/details/gvhfjelxe.sHtML

[U48] PHP：纯枚举
来源：http://m.share.bbcook.cn/Article/details/gapyjsgcz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.tarul.cn/Article/details/gyxgrjlsw.sHtML

[U49] PHP：只读属性
来源：http://blog.tarul.cn/Article/details/gtbttibot.sHtML

public readonly string $name
来源：http://www.blog.bbcook.cn/Article/details/gvbxkyujn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.sjlbkw.cn/Article/details/gowbgwjek.sHtML

public function __construct(private int $id) {}
来源：http://read.share.tarul.cn/Article/details/gqgmudopp.sHtML

[U51] PHP：数组解构
来源：http://www.blog.bbcook.cn/Article/details/gtlmeatxs.sHtML

[$a, $b] = $arr;
来源：http://read.share.tarul.cn/Article/details/gljctirme.sHtML

[U52] PHP：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/gbbpnadie.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.epnwcf.com/Article/details/gdrxflugl.sHtML

[U53] PHP：空合并运算符
来源：http://blog.tarul.cn/Article/details/gqmmxocxs.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fktsv.cn/Article/details/gmgrhuplz.sHtML

[U54] PHP：空安全调用
来源：http://m.share.sjlbkw.cn/Article/details/glxkrqgbx.sHtML

$obj?->method()
来源：http://www.share.fktsv.cn/Article/details/gabtxuwtg.sHtML

[U55] PHP：match 表达式
来源：http://mobile.epnwcf.com/Article/details/gujbqptre.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.bbcook.cn/Article/details/gsgmfwlke.sHtML

[U56] PHP：命名参数
来源：http://read.share.vehdjk.com/Article/details/grhromsxy.sHtML

f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gyzmbpwwp.sHtML

[U57] PHP：字符串插值
来源：http://3g.bbcook.cn/Article/details/gyacjvmaa.sHtML

"值: {$a}"
来源：http://blog.sjlbkw.cn/Article/details/geculeomy.sHtML

[U58] PHP：数组三件套
来源：http://m.share.sjlbkw.cn/Article/details/gmjbtcsyq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.yfazqb.com/Article/details/gkulagntu.sHtML

[U59] PHP：自定义排序
来源：http://m.share.vehdjk.com/Article/details/gbbvbtmon.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.yfazqb.com/Article/details/gxqkabmyz.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.tarul.cn/Article/details/gblcmnekw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvihhyfcm.sHtML

[U61] PHP：正则
来源：http://read.share.vehdjk.com/Article/details/gleeimvqb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.vehdjk.com/Article/details/gsqridjho.sHtML

[U62] PHP：日期对象
来源：http://baike.sjlbkw.cn/Article/details/gywtnfxgg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.yfazqb.com/Article/details/gwceduiiu.sHtML

[U63] PHP：文件读写
来源：http://m.share.yfazqb.com/Article/details/gwzvlqtku.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.epnwcf.com/Article/details/gxitxsdrb.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.yfazqb.com/Article/details/grjssjzjn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.yfazqb.com/Article/details/gslwlsgaz.sHtML

[U65] PHP：会话
来源：http://3g.tarul.cn/Article/details/grrdxtiix.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.epnwcf.com/Article/details/gehxhuygr.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.sjlbkw.cn/Article/details/gktptnrzw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.vehdjk.com/Article/details/gwhnfiiky.sHtML


<!-- 参考信息 -->