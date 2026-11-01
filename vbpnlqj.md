代发 wailian999

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/gtbbtpjnu.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.vehdjk.com/Article/details/guhookadb.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gatzdmigd.sHtML

void inc(int &x) { ++x; }
来源：http://blog.bbcook.cn/Article/details/gonjqrwew.sHtML

[S45] C++：lambda
来源：http://wap.fktsv.cn/Article/details/greznfbpo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.yfazqb.com/Article/details/gupuwivqk.sHtML

[S46] C++：函数模板
来源：http://baike.tarul.cn/Article/details/gawehqyes.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/gfttxkcvf.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.vehdjk.com/Article/details/gbdidwrki.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.bbcook.cn/Article/details/gaolpuhns.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gxuhqolqb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fktsv.cn/Article/details/gtdsiapft.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gjbyoaksd.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gzhzfdbzm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.yfazqb.com/Article/details/gpzlvnapd.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.vehdjk.com/Article/details/grnpcykuy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gfmwliwsk.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/gkvtehchh.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/gzyesckdd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.sjlbkw.cn/Article/details/gwbznztsk.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/gavtwhvls.sHtML

[S53] C++：移动语义
来源：http://read.share.fktsv.cn/Article/details/gnaexrqtm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.yfazqb.com/Article/details/gnzmdjxxj.sHtML

[S54] C++：异常处理
来源：http://www.share.vehdjk.com/Article/details/gqzokgwvb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.sjlbkw.cn/Article/details/gwwekvjpy.sHtML

[S55] C++：结构化绑定
来源：http://3g.vehdjk.com/Article/details/goggliylt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/ggpclariw.sHtML

[S56] C++：optional
来源：http://baike.vehdjk.com/Article/details/gswmxhvih.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.sjlbkw.cn/Article/details/gkgqmcjix.sHtML

[S57] C++：编译期常量
来源：http://baike.bbcook.cn/Article/details/gyukzryze.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/giqvmkqal.sHtML

[S58] C++：命名空间
来源：http://blog.epnwcf.com/Article/details/gmuwyfnpi.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/gspmrspqt.sHtML

[S59] C++：静态断言
来源：http://3g.fktsv.cn/Article/details/gbylpijnk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.yfazqb.com/Article/details/gtypyaduu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gbhxegcbq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.sjlbkw.cn/Article/details/givyvppjv.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtbwhbzz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gtqskdqfi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/glqnqchmx.sHtML

[T01] Kotlin：Hello World
来源：http://blog.epnwcf.com/Article/details/gmqizihvg.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gwymuekfg.sHtML

[T02] Kotlin：变量
来源：http://mobile.vehdjk.com/Article/details/gxmalrigq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.yfazqb.com/Article/details/gaifdehgj.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fktsv.cn/Article/details/gvoftswyy.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gtzkyuvpu.sHtML

[T04] Kotlin：空安全
来源：http://baike.vehdjk.com/Article/details/gdzpqivrq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.tarul.cn/Article/details/gixtonykj.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fktsv.cn/Article/details/gqnknmmjc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/ggpdwplxy.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmmqotyr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gpxrlvxmz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.yfazqb.com/Article/details/gycqfeodm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gcoupyiry.sHtML

[T08] Kotlin：数据类
来源：http://mobile.tarul.cn/Article/details/gyvtqprvd.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.yfazqb.com/Article/details/gylojhpdv.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.epnwcf.com/Article/details/gatsaxptw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/goszfbvxx.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.sjlbkw.cn/Article/details/gsdzajugu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.epnwcf.com/Article/details/grqxrttlw.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/gjrhcsadv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.epnwcf.com/Article/details/gvsbpzcrm.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/grtmuzrby.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gzqqplyzn.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fktsv.cn/Article/details/gqohdaacf.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.epnwcf.com/Article/details/gbsoxxrjb.sHtML

[T14] Kotlin：循环
来源：http://mobile.yfazqb.com/Article/details/gfmogdozb.sHtML

for (i in 1..10) println(i)
来源：http://www.share.tarul.cn/Article/details/gqxbopteq.sHtML

[T15] Kotlin：接口
来源：http://m.share.yfazqb.com/Article/details/gstugdeck.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.vehdjk.com/Article/details/gqnurynvc.sHtML

[T16] Swift：Hello World
来源：http://baike.epnwcf.com/Article/details/goetwvwld.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/gdttuzddx.sHtML

[T17] Swift：变量与常量
来源：http://baike.bbcook.cn/Article/details/gitjvimmp.sHtML

var a = 1;  let b = 2
来源：http://read.share.epnwcf.com/Article/details/gqzudphic.sHtML

[T18] Swift：字符串插值
来源：http://wap.vehdjk.com/Article/details/gklzurwcl.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gxitzdbdy.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.bbcook.cn/Article/details/glakrowvq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.yfazqb.com/Article/details/gmiiloaeo.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/gwbfyqiph.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.bbcook.cn/Article/details/gmdaqkmgo.sHtML

[T21] Swift：遍历
来源：http://m.share.fktsv.cn/Article/details/gdqeovsxv.sHtML

for x in a { print(x) }
来源：http://3g.bbcook.cn/Article/details/glcdowebu.sHtML

[T22] Swift：字典
来源：http://read.share.yfazqb.com/Article/details/gasrqtqoy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.yfazqb.com/Article/details/gssmdumhd.sHtML

[T23] Swift：函数
来源：http://m.share.bbcook.cn/Article/details/gxjoocdit.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.tarul.cn/Article/details/gzfwankiz.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/grvfvgjis.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.tarul.cn/Article/details/gzjobktyf.sHtML

[T25] Swift：结构体
来源：http://www.share.fktsv.cn/Article/details/ggaydktzq.sHtML

struct P { var x: Int }
来源：http://www.m.share.epnwcf.com/Article/details/gscxogdkb.sHtML

[T26] Swift：类与重写
来源：http://m.share.tarul.cn/Article/details/gtwolypnv.sHtML

class A: Base { override func f() {} }
来源：http://m.share.sjlbkw.cn/Article/details/gkjzfgtmw.sHtML

[T27] Swift：错误处理
来源：http://www.blog.yfazqb.com/Article/details/gasbtwdtp.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fktsv.cn/Article/details/gkmumfszn.sHtML

[T28] Swift：枚举
来源：http://wap.vehdjk.com/Article/details/gdwerobgz.sHtML

enum Color { case red, green }
来源：http://read.share.vehdjk.com/Article/details/gobrnfnow.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.bbcook.cn/Article/details/gwheqfjcd.sHtML

guard let x = opt else { return }
来源：http://www.blog.bbcook.cn/Article/details/ggrwadcpb.sHtML

[T30] Swift：协议
来源：http://3g.vehdjk.com/Article/details/gkqrqgndu.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.bbcook.cn/Article/details/gcimynfho.sHtML

[T31] Lua：Hello World
来源：http://mobile.epnwcf.com/Article/details/gmufszyij.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gfnlvwzkq.sHtML

[T32] Lua：局部变量
来源：http://wap.epnwcf.com/Article/details/gpycwhfpm.sHtML

local a = 1
来源：http://www.blog.vehdjk.com/Article/details/gsmsgjamd.sHtML

[T33] Lua：表（数组）
来源：http://blog.vehdjk.com/Article/details/gkaxqxsvo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fktsv.cn/Article/details/gxlcdqijl.sHtML

[T34] Lua：遍历表
来源：http://www.share.tarul.cn/Article/details/geesfdfrq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.epnwcf.com/Article/details/geyozvcdc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fktsv.cn/Article/details/gbmpivono.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.yfazqb.com/Article/details/gmvgkwsbj.sHtML

[T36] Lua：函数
来源：http://www.share.sjlbkw.cn/Article/details/ghnauicre.sHtML

function add(a, b) return a + b end
来源：http://3g.vehdjk.com/Article/details/gqymkicgs.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.epnwcf.com/Article/details/gyhagrxtv.sHtML

"a" .. "b"
来源：http://m.share.fktsv.cn/Article/details/gmvtivrvv.sHtML

[T38] Lua：条件
来源：http://3g.vehdjk.com/Article/details/gohqpcqda.sHtML

if x > 0 then print("正") end
来源：http://read.share.vehdjk.com/Article/details/gbqqcaxof.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gyryytnwt.sHtML

string.find(s, "%d+")
来源：http://baike.vehdjk.com/Article/details/gkcosrxez.sHtML

[T40] Lua：元表
来源：http://www.blog.tarul.cn/Article/details/gaxixrxpm.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.tarul.cn/Article/details/gphmogxhz.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/gznklgjet.sHtML

print "Hello\n";
来源：http://m.share.sjlbkw.cn/Article/details/gxdgkplhd.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/gowksvwup.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.vehdjk.com/Article/details/gmykxmxgk.sHtML

[T43] Perl：字符串插值
来源：http://m.share.bbcook.cn/Article/details/giigtafws.sHtML

"值: $a"
来源：http://www.blog.bbcook.cn/Article/details/gpfmxcvaq.sHtML

[T44] Perl：条件
来源：http://www.blog.yfazqb.com/Article/details/gxiblsgln.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.vehdjk.com/Article/details/gjjgczmui.sHtML

[T45] Perl：数组遍历
来源：http://wap.bbcook.cn/Article/details/ghdtiqylg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.epnwcf.com/Article/details/gmyuipcgv.sHtML

[T46] Perl：哈希操作
来源：http://wap.bbcook.cn/Article/details/ggdanbmbv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.epnwcf.com/Article/details/gblronvvm.sHtML

[T47] Perl：正则捕获
来源：http://wap.bbcook.cn/Article/details/gnirrcgvt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.yfazqb.com/Article/details/gmultcxxc.sHtML

[T48] Perl：正则替换
来源：http://wap.epnwcf.com/Article/details/gkxjvtmrw.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.vehdjk.com/Article/details/gvnyrrgfx.sHtML

[T49] Perl：函数
来源：http://www.share.yfazqb.com/Article/details/gvnmbknev.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gwuwgeaga.sHtML

[T50] Perl：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gklpaiezh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.yfazqb.com/Article/details/ggdsybslc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.epnwcf.com/Article/details/gefcwleka.sHtML

[T51] Scala：Hello World
来源：http://mobile.fktsv.cn/Article/details/gbduceglw.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gxvfufhzj.sHtML

[T52] Scala：变量
来源：http://mobile.tarul.cn/Article/details/gwwsatgds.sHtML

val a = 1;  var b = 2
来源：http://wap.sjlbkw.cn/Article/details/ghgmmdiuz.sHtML

[T53] Scala：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/grysweene.sHtML

s"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gbdtseuow.sHtML

[T54] Scala：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gaxfuywjt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gusqqruod.sHtML

[T55] Scala：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/ghywdgler.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.yfazqb.com/Article/details/gboctkybu.sHtML

[T56] Scala：样例类
来源：http://wap.epnwcf.com/Article/details/gwcmiweuj.sHtML

case class User(name: String, age: Int)
来源：http://www.share.tarul.cn/Article/details/ghsgduqwn.sHtML

[T57] Scala：模式匹配
来源：http://www.share.vehdjk.com/Article/details/gjhkhsldi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.epnwcf.com/Article/details/gghyhyuwy.sHtML

[T58] Scala：函数定义
来源：http://www.blog.sjlbkw.cn/Article/details/gsaouqcek.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.epnwcf.com/Article/details/gyykoyhlx.sHtML

[T59] Scala：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gamdjffaq.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.epnwcf.com/Article/details/gzyhtonsq.sHtML

[T60] Scala：折叠
来源：http://www.share.fktsv.cn/Article/details/ggjskjmuh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/giezcgkhx.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gnolyjcks.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.yfazqb.com/Article/details/gqebhqqad.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glaczndgx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.epnwcf.com/Article/details/grfqtppxf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.bbcook.cn/Article/details/giohaezxv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.epnwcf.com/Article/details/gavywxbtf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbntzbfp.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.bbcook.cn/Article/details/gospiaqmx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.tarul.cn/Article/details/gtjolhsqt.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.sjlbkw.cn/Article/details/geqoinuut.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.tarul.cn/Article/details/glccsmgme.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fktsv.cn/Article/details/gywrdpvqo.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/gezanjnbu.sHtML

[U06] Py：合并两个字典
来源：http://baike.tarul.cn/Article/details/gogcptyar.sHtML

{**a, **b}
来源：http://m.share.yfazqb.com/Article/details/gigwxyvqf.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.epnwcf.com/Article/details/gmjshptee.sHtML

{v: k for k, v in d.items()}
来源：http://3g.vehdjk.com/Article/details/gdebabvws.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.tarul.cn/Article/details/gqyhvlyfq.sHtML

[y for x in nested for y in x]
来源：http://mobile.tarul.cn/Article/details/gbthbitzx.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.sjlbkw.cn/Article/details/gzchavqpo.sHtML

max(d, key=d.get)
来源：http://wap.vehdjk.com/Article/details/gfaitdmbt.sHtML

[U10] Py：按值排序字典
来源：http://www.share.sjlbkw.cn/Article/details/gdrvgckmc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.vehdjk.com/Article/details/gdvbdhlmv.sHtML

[U11] Py：生成器表达式
来源：http://mobile.epnwcf.com/Article/details/ggnsylzgq.sHtML

(x * 2 for x in arr)
来源：http://baike.fktsv.cn/Article/details/gbcgulrhh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.yfazqb.com/Article/details/gzezgblda.sHtML

Counter(arr).most_common(3)
来源：http://3g.vehdjk.com/Article/details/givmkfemy.sHtML

[U13] Py：固定长度队列
来源：http://blog.fktsv.cn/Article/details/gxbrbpyxd.sHtML

deque(maxlen=10)
来源：http://blog.epnwcf.com/Article/details/gzbasvmeb.sHtML

[U14] Py：分组收集到列表
来源：http://baike.tarul.cn/Article/details/gpaidlxin.sHtML

defaultdict(list)
来源：http://blog.epnwcf.com/Article/details/gragwcudp.sHtML

[U15] Py：高精度计时
来源：http://mobile.bbcook.cn/Article/details/gylpbacbu.sHtML

t = time.perf_counter()
来源：http://www.share.bbcook.cn/Article/details/ggdynifnw.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.tarul.cn/Article/details/gtdpmcalq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fktsv.cn/Article/details/gwbqbubzf.sHtML

[U17] Py：初始化日志
来源：http://wap.epnwcf.com/Article/details/gsldmqute.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.sjlbkw.cn/Article/details/gsqbqepni.sHtML

[U18] Py：预编译正则
来源：http://mobile.sjlbkw.cn/Article/details/gipseihau.sHtML

pat = re.compile(r"\d+")
来源：http://blog.tarul.cn/Article/details/ghkiqaomq.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fktsv.cn/Article/details/gklgzajtq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.sjlbkw.cn/Article/details/gavgtigtr.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.yfazqb.com/Article/details/gqeomlkwv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.tarul.cn/Article/details/gudrcdubr.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.tarul.cn/Article/details/glodjhapd.sHtML

@contextlib.contextmanager
来源：http://wap.tarul.cn/Article/details/gyqolnbvy.sHtML

[U22] Py：矩阵转置
来源：http://wap.fktsv.cn/Article/details/gkulzfyoe.sHtML

list(zip(*m))
来源：http://www.blog.vehdjk.com/Article/details/gsuormdxo.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.yfazqb.com/Article/details/gnpfocjrb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.vehdjk.com/Article/details/gocpzpedj.sHtML

[U24] Py：路径操作
来源：http://www.m.share.yfazqb.com/Article/details/gkkliotlk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/gnwtfjkua.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fktsv.cn/Article/details/gxvqymtji.sHtML

csv.DictReader(f)
来源：http://3g.sjlbkw.cn/Article/details/gxphapfua.sHtML

[U26] Py：并发下载
来源：http://baike.epnwcf.com/Article/details/gzmbiynti.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.yfazqb.com/Article/details/gfacpnyci.sHtML

[U27] Py：异步 HTTP
来源：http://3g.sjlbkw.cn/Article/details/ghvyxfium.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fktsv.cn/Article/details/gahsujdpk.sHtML

[U28] Py：类型别名
来源：http://baike.epnwcf.com/Article/details/gmwpswtit.sHtML

UserId = int
来源：http://read.share.vehdjk.com/Article/details/glffpdtvs.sHtML

[U29] Py：属性校验
来源：http://baike.fktsv.cn/Article/details/grdrztpff.sHtML

@property 与 @x.setter 配合
来源：http://wap.epnwcf.com/Article/details/gidkaeqbe.sHtML

[U30] Py：数据类
来源：http://m.share.bbcook.cn/Article/details/ghnavjgyb.sHtML

@dataclass(slots=True)
来源：http://www.blog.bbcook.cn/Article/details/gztybesne.sHtML

[U31] Py：单测
来源：http://www.blog.fktsv.cn/Article/details/gnpmembzm.sHtML

python -m pytest -q
来源：http://read.share.tarul.cn/Article/details/gnrrgqgeg.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.bbcook.cn/Article/details/gvdxiovem.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fktsv.cn/Article/details/gbczfcdkl.sHtML

[U33] Py：打包发布
来源：http://www.share.epnwcf.com/Article/details/gelupjsuy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.sjlbkw.cn/Article/details/gifuircod.sHtML

[U34] Py：判断编码
来源：http://blog.epnwcf.com/Article/details/gjhchofem.sHtML

chardet.detect(raw)
来源：http://m.share.sjlbkw.cn/Article/details/gureomdzr.sHtML

[U35] Py：发送邮件
来源：http://mobile.fktsv.cn/Article/details/guphdwjlr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.sjlbkw.cn/Article/details/gvciifysv.sHtML

[U36] Py：定时任务
来源：http://blog.vehdjk.com/Article/details/gjlwfhrig.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.bbcook.cn/Article/details/gxikguypz.sHtML

[U37] Py：读写 Excel
来源：http://mobile.tarul.cn/Article/details/galmkurgx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.epnwcf.com/Article/details/gcsbmskml.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.bbcook.cn/Article/details/gryczrmxn.sHtML

Path(__file__).resolve().parent
来源：http://www.share.tarul.cn/Article/details/gkydbqkhp.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.bbcook.cn/Article/details/gsbqnwhog.sHtML

sys.stdout.isatty()
来源：http://m.share.bbcook.cn/Article/details/gbvkeiqft.sHtML

[U40] Py：打印到标准错误
来源：http://blog.sjlbkw.cn/Article/details/giejuxwej.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gtawydmsy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fktsv.cn/Article/details/ghjcsphkt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.sjlbkw.cn/Article/details/grlbsxtvw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.sjlbkw.cn/Article/details/ganjgmjru.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.yfazqb.com/Article/details/gwwtmnoqt.sHtML

[U43] PHP：声明命名空间
来源：http://blog.epnwcf.com/Article/details/gprbyuypv.sHtML

namespace App\Http;
来源：http://3g.epnwcf.com/Article/details/gishsyycf.sHtML

[U44] PHP：开启严格类型
来源：http://baike.epnwcf.com/Article/details/gvnogjkte.sHtML

declare(strict_types=1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcscgvbmr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.yfazqb.com/Article/details/gemihwuoi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gkpxghsdt.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fktsv.cn/Article/details/gkhavknbl.sHtML

?string $name = null
来源：http://blog.fktsv.cn/Article/details/gbgvghxbr.sHtML

[U47] PHP：联合类型
来源：http://3g.bbcook.cn/Article/details/glgisckce.sHtML

int|string $id
来源：http://m.share.fktsv.cn/Article/details/giywdgmjb.sHtML

[U48] PHP：纯枚举
来源：http://www.share.tarul.cn/Article/details/gaxebjnas.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.yfazqb.com/Article/details/gntqeopru.sHtML

[U49] PHP：只读属性
来源：http://www.share.vehdjk.com/Article/details/guzxdedtj.sHtML

public readonly string $name
来源：http://mobile.epnwcf.com/Article/details/gcqxhmloh.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.yfazqb.com/Article/details/goqszippy.sHtML

public function __construct(private int $id) {}
来源：http://mobile.yfazqb.com/Article/details/gyvwnqnap.sHtML

[U51] PHP：数组解构
来源：http://mobile.fktsv.cn/Article/details/gjpiijcph.sHtML

[$a, $b] = $arr;
来源：http://blog.yfazqb.com/Article/details/gxzxctsjl.sHtML

[U52] PHP：箭头函数
来源：http://m.share.sjlbkw.cn/Article/details/ghioaqajz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.epnwcf.com/Article/details/gghdypvxp.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.yfazqb.com/Article/details/gafenpxws.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.vehdjk.com/Article/details/gvxzveaqn.sHtML

[U54] PHP：空安全调用
来源：http://m.share.vehdjk.com/Article/details/gqlnlsoxz.sHtML

$obj?->method()
来源：http://www.blog.epnwcf.com/Article/details/gosvbwotr.sHtML

[U55] PHP：match 表达式
来源：http://baike.sjlbkw.cn/Article/details/gnecrudlu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fktsv.cn/Article/details/gklfquind.sHtML

[U56] PHP：命名参数
来源：http://read.share.tarul.cn/Article/details/gjmfwntnr.sHtML

f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gysvveiau.sHtML

[U57] PHP：字符串插值
来源：http://3g.vehdjk.com/Article/details/ghyebhczc.sHtML

"值: {$a}"
来源：http://wap.tarul.cn/Article/details/gnviznogm.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.sjlbkw.cn/Article/details/ggmsukgeg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fktsv.cn/Article/details/gshhrpxkk.sHtML

[U59] PHP：自定义排序
来源：http://blog.bbcook.cn/Article/details/gkgemynse.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gtitwhcco.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.sjlbkw.cn/Article/details/gyibviutn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.vehdjk.com/Article/details/gfjpvlglq.sHtML

[U61] PHP：正则
来源：http://read.share.fktsv.cn/Article/details/gkuwsbsax.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gmecuvnwb.sHtML

[U62] PHP：日期对象
来源：http://3g.vehdjk.com/Article/details/gkmhjcfbt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fktsv.cn/Article/details/gfiqcollk.sHtML

[U63] PHP：文件读写
来源：http://3g.yfazqb.com/Article/details/gsqpndaie.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fktsv.cn/Article/details/gahmlrija.sHtML

[U64] PHP：目录遍历
来源：http://read.share.yfazqb.com/Article/details/gbxwsdfen.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.yfazqb.com/Article/details/gzwnrhoat.sHtML

[U65] PHP：会话
来源：http://blog.sjlbkw.cn/Article/details/gcoemkosh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gjluhrhcq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.vehdjk.com/Article/details/gmgzkaldi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.bbcook.cn/Article/details/gvgkozoju.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fktsv.cn/Article/details/ggndtcuxa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.bbcook.cn/Article/details/guerxsxpp.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.epnwcf.com/Article/details/gvvxynjon.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.sjlbkw.cn/Article/details/gwsmukpox.sHtML


<!-- 参考信息 -->