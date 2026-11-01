代发 wailian999

[S45] C++：lambda
来源：http://mobile.vehdjk.com/Article/details/gszhrjyey.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.bbcook.cn/Article/details/goaqioabh.sHtML

[S46] C++：函数模板
来源：http://wap.fktsv.cn/Article/details/gpzrslkcs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/gymjcfmeq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/gdlmlskwp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gmmobalsa.sHtML

[S48] C++：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gvygxoxse.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fktsv.cn/Article/details/gslhqxuxw.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.tarul.cn/Article/details/glzvxzrcp.sHtML

[S49] C++：写文件
来源：http://baike.tarul.cn/Article/details/gayyhuumo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fktsv.cn/Article/details/glekbwhzm.sHtML

[S50] C++：格式化数字
来源：http://wap.bbcook.cn/Article/details/ggfrxuhpf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.bbcook.cn/Article/details/grnfyqumy.sHtML

[S51] C++：显式类型转换
来源：http://3g.bbcook.cn/Article/details/gynkdpyai.sHtML

static_cast<double>(a) / b
来源：http://www.share.fktsv.cn/Article/details/gbqegmhva.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/gtwwmhjst.sHtML

int size() const noexcept { return n_; }
来源：http://3g.sjlbkw.cn/Article/details/glbriduel.sHtML

[S53] C++：移动语义
来源：http://baike.tarul.cn/Article/details/gimhehjle.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fktsv.cn/Article/details/gulckyfhu.sHtML

[S54] C++：异常处理
来源：http://www.blog.yfazqb.com/Article/details/golxjezxs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.tarul.cn/Article/details/gksrrzdgd.sHtML

[S55] C++：结构化绑定
来源：http://m.share.bbcook.cn/Article/details/gejmspxno.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gclcsvyeq.sHtML

[S56] C++：optional
来源：http://blog.tarul.cn/Article/details/gchqalqyj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.epnwcf.com/Article/details/gykwvlkou.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gshurgknk.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/gvsvoywbm.sHtML

[S58] C++：命名空间
来源：http://read.share.bbcook.cn/Article/details/gasqbkjdl.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.tarul.cn/Article/details/gbmihjvof.sHtML

[S59] C++：静态断言
来源：http://read.share.yfazqb.com/Article/details/gmzeujjrw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.sjlbkw.cn/Article/details/gockattxj.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.yfazqb.com/Article/details/gwdogcriy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.bbcook.cn/Article/details/gqptmxvnd.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrsyfiuf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gpjdjeyql.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbsrpllpg.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/grzsuodmu.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/glderhxne.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/ghocaxjkd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.tarul.cn/Article/details/gxsabyiwm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.epnwcf.com/Article/details/goznchqys.sHtML

"值: $b"
来源：http://baike.tarul.cn/Article/details/gmypcdaor.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fktsv.cn/Article/details/gcvlbqjki.sHtML

val n: String? = null;  n?.length
来源：http://www.share.bbcook.cn/Article/details/gplzsmdmu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyafproo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/grxhzaiwj.sHtML

[T06] Kotlin：集合映射
来源：http://3g.epnwcf.com/Article/details/gsptuagcn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.epnwcf.com/Article/details/gojxutbcn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/geflztegq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.sjlbkw.cn/Article/details/gsqkdptng.sHtML

[T08] Kotlin：数据类
来源：http://mobile.sjlbkw.cn/Article/details/goyacdvfc.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/ghznepjqe.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/gtrmrfayt.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fktsv.cn/Article/details/guihrgxfr.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gnkufrjpa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.bbcook.cn/Article/details/ghloaqxwy.sHtML

[T11] Kotlin：协程
来源：http://m.share.sjlbkw.cn/Article/details/gnivaectw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.tarul.cn/Article/details/gvvsufkna.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.epnwcf.com/Article/details/gydaqaxjd.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.tarul.cn/Article/details/glmdtfpsj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.vehdjk.com/Article/details/giezftzvh.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.tarul.cn/Article/details/gczwppbxx.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gwwidsmqm.sHtML

for (i in 1..10) println(i)
来源：http://mobile.vehdjk.com/Article/details/guwwnklwt.sHtML

[T15] Kotlin：接口
来源：http://3g.epnwcf.com/Article/details/gqgthudlc.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.sjlbkw.cn/Article/details/gyzlprbtn.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gkvfobyfh.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gusoabdlq.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.vehdjk.com/Article/details/gbvvcnhrn.sHtML

var a = 1;  let b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gdtvksepc.sHtML

[T18] Swift：字符串插值
来源：http://wap.bbcook.cn/Article/details/gpouisitv.sHtML

"值: \(b)"
来源：http://mobile.sjlbkw.cn/Article/details/gvizxrpwa.sHtML

[T19] Swift：可选绑定
来源：http://wap.fktsv.cn/Article/details/gatrzbcpa.sHtML

if let n = opt { print(n) }
来源：http://mobile.epnwcf.com/Article/details/gqmrcsvay.sHtML

[T20] Swift：数组操作
来源：http://mobile.tarul.cn/Article/details/glqjpopfm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.vehdjk.com/Article/details/gfiybnmzq.sHtML

[T21] Swift：遍历
来源：http://blog.bbcook.cn/Article/details/gopjspsyr.sHtML

for x in a { print(x) }
来源：http://3g.yfazqb.com/Article/details/gxlzjjsdd.sHtML

[T22] Swift：字典
来源：http://3g.yfazqb.com/Article/details/gydenjdwr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.epnwcf.com/Article/details/gspocodpk.sHtML

[T23] Swift：函数
来源：http://mobile.epnwcf.com/Article/details/gisykvlix.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.sjlbkw.cn/Article/details/gvcbwfygb.sHtML

[T24] Swift：闭包
来源：http://3g.fktsv.cn/Article/details/gtmnhhzia.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.yfazqb.com/Article/details/gqtfwrcki.sHtML

[T25] Swift：结构体
来源：http://www.share.epnwcf.com/Article/details/gcduthnhw.sHtML

struct P { var x: Int }
来源：http://baike.vehdjk.com/Article/details/gemhhvdkx.sHtML

[T26] Swift：类与重写
来源：http://www.share.bbcook.cn/Article/details/gejpldann.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gsyamdfws.sHtML

[T27] Swift：错误处理
来源：http://3g.sjlbkw.cn/Article/details/gidlkgmdi.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fktsv.cn/Article/details/gsrpzpcnc.sHtML

[T28] Swift：枚举
来源：http://m.share.yfazqb.com/Article/details/gfapgteii.sHtML

enum Color { case red, green }
来源：http://mobile.epnwcf.com/Article/details/gkwamwlva.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.yfazqb.com/Article/details/grsavguzv.sHtML

guard let x = opt else { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gkjkmkqlf.sHtML

[T30] Swift：协议
来源：http://baike.epnwcf.com/Article/details/gtvdpfdgs.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.epnwcf.com/Article/details/gjzmiwdwl.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gakvpyupo.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gvurnqfoj.sHtML

[T32] Lua：局部变量
来源：http://read.share.bbcook.cn/Article/details/gwkocodgb.sHtML

local a = 1
来源：http://read.share.bbcook.cn/Article/details/guhsxxxvl.sHtML

[T33] Lua：表（数组）
来源：http://baike.vehdjk.com/Article/details/gmljznbej.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fktsv.cn/Article/details/gjszlarbo.sHtML

[T34] Lua：遍历表
来源：http://3g.bbcook.cn/Article/details/gibfkfwly.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.bbcook.cn/Article/details/gqecmcrum.sHtML

[T35] Lua：字典表
来源：http://read.share.yfazqb.com/Article/details/gakxikpno.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.sjlbkw.cn/Article/details/gmtjqrxoh.sHtML

[T36] Lua：函数
来源：http://baike.epnwcf.com/Article/details/gvfwmogbe.sHtML

function add(a, b) return a + b end
来源：http://mobile.vehdjk.com/Article/details/gkqltzxek.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/gbddcxlzc.sHtML

"a" .. "b"
来源：http://wap.yfazqb.com/Article/details/gvoiuadlx.sHtML

[T38] Lua：条件
来源：http://mobile.tarul.cn/Article/details/gijlembfj.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/gdbvbbyjv.sHtML

[T39] Lua：模式匹配
来源：http://wap.bbcook.cn/Article/details/gixgqktem.sHtML

string.find(s, "%d+")
来源：http://blog.sjlbkw.cn/Article/details/gqveqndyd.sHtML

[T40] Lua：元表
来源：http://www.share.bbcook.cn/Article/details/gfsxylpkg.sHtML

setmetatable({}, { __index = base })
来源：http://blog.tarul.cn/Article/details/gqyrlksja.sHtML

[T41] Perl：Hello World
来源：http://m.share.tarul.cn/Article/details/gximgafmq.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/givznmtva.sHtML

[T42] Perl：变量类型
来源：http://www.blog.epnwcf.com/Article/details/gsgyjbcjc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.yfazqb.com/Article/details/groxmoggc.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.tarul.cn/Article/details/geeqbptuv.sHtML

"值: $a"
来源：http://m.share.bbcook.cn/Article/details/ghkrizodh.sHtML

[T44] Perl：条件
来源：http://blog.yfazqb.com/Article/details/gticgkkga.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.bbcook.cn/Article/details/godsrvopl.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.yfazqb.com/Article/details/gxabaezrq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmupbgzx.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fktsv.cn/Article/details/gmbgaqosl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.vehdjk.com/Article/details/gcvwybkqj.sHtML

[T47] Perl：正则捕获
来源：http://blog.yfazqb.com/Article/details/gxkkzjtul.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.vehdjk.com/Article/details/gskokoecz.sHtML

[T48] Perl：正则替换
来源：http://3g.epnwcf.com/Article/details/gsdccevzc.sHtML

$s =~ s/old/new/g;
来源：http://www.share.epnwcf.com/Article/details/gcxbklqtx.sHtML

[T49] Perl：函数
来源：http://www.m.share.bbcook.cn/Article/details/gtotpylmx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gpoxgyqse.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gkqhxhoju.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.epnwcf.com/Article/details/gxgcwinoq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.sjlbkw.cn/Article/details/grkpyrkfg.sHtML

[T51] Scala：Hello World
来源：http://mobile.yfazqb.com/Article/details/gdhwdgsjl.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/grdzuwrae.sHtML

[T52] Scala：变量
来源：http://mobile.fktsv.cn/Article/details/gvprsxnxf.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.yfazqb.com/Article/details/ggoqfnnqy.sHtML

[T53] Scala：字符串插值
来源：http://blog.yfazqb.com/Article/details/gjawjicoo.sHtML

s"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gudqnmvcr.sHtML

[T54] Scala：集合映射
来源：http://mobile.vehdjk.com/Article/details/gbuqnjpba.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.vehdjk.com/Article/details/gyjmpchie.sHtML

[T55] Scala：集合过滤
来源：http://wap.fktsv.cn/Article/details/gmjzsxsxz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.sjlbkw.cn/Article/details/gcjuskxti.sHtML

[T56] Scala：样例类
来源：http://m.share.tarul.cn/Article/details/gwkzsogvw.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.tarul.cn/Article/details/gzfstqxrx.sHtML

[T57] Scala：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/glkeirfil.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.yfazqb.com/Article/details/gyqabewap.sHtML

[T58] Scala：函数定义
来源：http://baike.yfazqb.com/Article/details/gxyscqgcs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gctovosyz.sHtML

[T59] Scala：循环
来源：http://blog.fktsv.cn/Article/details/gxyaqsfzf.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gpmkttsld.sHtML

[T60] Scala：折叠
来源：http://read.share.epnwcf.com/Article/details/gyioplvnn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.sjlbkw.cn/Article/details/gxvqpztpy.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gtdnwmhvt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/guaowvpdt.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gssbvvuhe.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.epnwcf.com/Article/details/grvwchpql.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.tarul.cn/Article/details/gtpffczuw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.epnwcf.com/Article/details/gqpvoqpit.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/gxrqfaduz.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.yfazqb.com/Article/details/gybohtbis.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fktsv.cn/Article/details/gbgoorxos.sHtML

[U04] Py：变量调试打印
来源：http://mobile.bbcook.cn/Article/details/gzgiqwyaq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fktsv.cn/Article/details/gkxqqzqhv.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.vehdjk.com/Article/details/gmfpyaezr.sHtML

list(dict.fromkeys(arr))
来源：http://3g.vehdjk.com/Article/details/gqojjriob.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.tarul.cn/Article/details/gvatndoei.sHtML

{**a, **b}
来源：http://www.m.share.fktsv.cn/Article/details/gjzgwskkr.sHtML

[U07] Py：反转字典键值
来源：http://www.share.bbcook.cn/Article/details/gfjsxqlxv.sHtML

{v: k for k, v in d.items()}
来源：http://baike.sjlbkw.cn/Article/details/gjpskpqnc.sHtML

[U08] Py：展平二维列表
来源：http://3g.yfazqb.com/Article/details/gggwxzifz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.sjlbkw.cn/Article/details/gxunzpdgo.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.tarul.cn/Article/details/gfckimtfe.sHtML

max(d, key=d.get)
来源：http://www.blog.tarul.cn/Article/details/gmuochctm.sHtML

[U10] Py：按值排序字典
来源：http://m.share.epnwcf.com/Article/details/gozugdbie.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.bbcook.cn/Article/details/gdibkdqhn.sHtML

[U11] Py：生成器表达式
来源：http://m.share.tarul.cn/Article/details/gnuhgkcxu.sHtML

(x * 2 for x in arr)
来源：http://wap.epnwcf.com/Article/details/gusuqmzhj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.epnwcf.com/Article/details/godkidpfw.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.vehdjk.com/Article/details/gijrzuuul.sHtML

[U13] Py：固定长度队列
来源：http://www.share.epnwcf.com/Article/details/gxjyjcrnb.sHtML

deque(maxlen=10)
来源：http://www.blog.sjlbkw.cn/Article/details/glicwirjg.sHtML

[U14] Py：分组收集到列表
来源：http://3g.bbcook.cn/Article/details/gahgsahyl.sHtML

defaultdict(list)
来源：http://3g.sjlbkw.cn/Article/details/gygrsihjk.sHtML

[U15] Py：高精度计时
来源：http://mobile.tarul.cn/Article/details/gudufsyyl.sHtML

t = time.perf_counter()
来源：http://m.share.bbcook.cn/Article/details/gyedxcghf.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.sjlbkw.cn/Article/details/gmxbnimei.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.yfazqb.com/Article/details/gjsanrdha.sHtML

[U17] Py：初始化日志
来源：http://wap.tarul.cn/Article/details/gkxcskfuv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.tarul.cn/Article/details/godkmtsbu.sHtML

[U18] Py：预编译正则
来源：http://read.share.epnwcf.com/Article/details/grharkuxm.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fktsv.cn/Article/details/gkwvlcgfx.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.epnwcf.com/Article/details/gbyieftkw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.yfazqb.com/Article/details/gkxbhikzy.sHtML

[U20] Py：缓存函数结果
来源：http://3g.yfazqb.com/Article/details/ghlfhppab.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.epnwcf.com/Article/details/gwhtyvllq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.tarul.cn/Article/details/gmanlszlv.sHtML

@contextlib.contextmanager
来源：http://www.share.vehdjk.com/Article/details/ggrmroujp.sHtML

[U22] Py：矩阵转置
来源：http://wap.epnwcf.com/Article/details/giynerdln.sHtML

list(zip(*m))
来源：http://www.m.share.fktsv.cn/Article/details/gntfmalwa.sHtML

[U23] Py：分块读取大文件
来源：http://blog.tarul.cn/Article/details/gouupgqbz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.vehdjk.com/Article/details/gftxwxizs.sHtML

[U24] Py：路径操作
来源：http://m.share.tarul.cn/Article/details/gmmgwkeme.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.yfazqb.com/Article/details/gzjomflgm.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.tarul.cn/Article/details/gyvduykco.sHtML

csv.DictReader(f)
来源：http://m.share.bbcook.cn/Article/details/gwmbpanfm.sHtML

[U26] Py：并发下载
来源：http://www.m.share.vehdjk.com/Article/details/gdnlawtma.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.bbcook.cn/Article/details/gedgoqxet.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fktsv.cn/Article/details/grvbvrxri.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.sjlbkw.cn/Article/details/gdrnazcvx.sHtML

[U28] Py：类型别名
来源：http://www.share.tarul.cn/Article/details/geejhzybr.sHtML

UserId = int
来源：http://wap.fktsv.cn/Article/details/gucdyusrh.sHtML

[U29] Py：属性校验
来源：http://www.blog.yfazqb.com/Article/details/gbeajcnlr.sHtML

@property 与 @x.setter 配合
来源：http://blog.epnwcf.com/Article/details/gymtxyjed.sHtML

[U30] Py：数据类
来源：http://3g.sjlbkw.cn/Article/details/gzjunmbcb.sHtML

@dataclass(slots=True)
来源：http://baike.tarul.cn/Article/details/gkkbukmnl.sHtML

[U31] Py：单测
来源：http://www.m.share.bbcook.cn/Article/details/gixevyrtr.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/gnjbfawhd.sHtML

[U32] Py：代码格式化
来源：http://blog.tarul.cn/Article/details/gzztephuy.sHtML

ruff format . && ruff check --fix .
来源：http://blog.yfazqb.com/Article/details/gciwnlyda.sHtML

[U33] Py：打包发布
来源：http://www.share.yfazqb.com/Article/details/gksgtgqyd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.sjlbkw.cn/Article/details/grpybufwo.sHtML

[U34] Py：判断编码
来源：http://m.share.tarul.cn/Article/details/gzeicgvrj.sHtML

chardet.detect(raw)
来源：http://mobile.epnwcf.com/Article/details/gcagaumex.sHtML

[U35] Py：发送邮件
来源：http://www.blog.bbcook.cn/Article/details/gvuppwazr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fktsv.cn/Article/details/gpdhalvje.sHtML

[U36] Py：定时任务
来源：http://baike.yfazqb.com/Article/details/gqqtcljsp.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.epnwcf.com/Article/details/gpbkhlvxb.sHtML

[U37] Py：读写 Excel
来源：http://mobile.tarul.cn/Article/details/gcpvvgeis.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.yfazqb.com/Article/details/gulluwsqw.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.yfazqb.com/Article/details/gjylothxz.sHtML

Path(__file__).resolve().parent
来源：http://blog.bbcook.cn/Article/details/gktyobnzb.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.epnwcf.com/Article/details/gqjqhbmlb.sHtML

sys.stdout.isatty()
来源：http://m.share.fktsv.cn/Article/details/gdfkltnyr.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fktsv.cn/Article/details/geetxxdtj.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gotytemvq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.yfazqb.com/Article/details/gcfgopipu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.vehdjk.com/Article/details/gzceapxnq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.vehdjk.com/Article/details/gptfbswvt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fktsv.cn/Article/details/glzfszuna.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.bbcook.cn/Article/details/gjgroadys.sHtML

namespace App\Http;
来源：http://blog.fktsv.cn/Article/details/giwcbvscr.sHtML

[U44] PHP：开启严格类型
来源：http://baike.sjlbkw.cn/Article/details/geocrgrif.sHtML

declare(strict_types=1);
来源：http://m.share.yfazqb.com/Article/details/geejzgqgp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.epnwcf.com/Article/details/gygzcvzku.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gmhhppmqw.sHtML

[U46] PHP：可空类型
来源：http://www.share.tarul.cn/Article/details/gwfcysuoi.sHtML

?string $name = null
来源：http://3g.vehdjk.com/Article/details/gmrcvblfv.sHtML

[U47] PHP：联合类型
来源：http://blog.epnwcf.com/Article/details/gugcvpphe.sHtML

int|string $id
来源：http://www.m.share.epnwcf.com/Article/details/gyaleqslo.sHtML

[U48] PHP：纯枚举
来源：http://blog.fktsv.cn/Article/details/gqfcmtcqn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.epnwcf.com/Article/details/gwqegbvhn.sHtML

[U49] PHP：只读属性
来源：http://blog.vehdjk.com/Article/details/gcdpmuccw.sHtML

public readonly string $name
来源：http://m.share.yfazqb.com/Article/details/ggaufzpvo.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.vehdjk.com/Article/details/gchegibwb.sHtML

public function __construct(private int $id) {}
来源：http://baike.vehdjk.com/Article/details/glmljivbz.sHtML

[U51] PHP：数组解构
来源：http://mobile.yfazqb.com/Article/details/gtxmhuzkh.sHtML

[$a, $b] = $arr;
来源：http://read.share.yfazqb.com/Article/details/gqlcacqnh.sHtML

[U52] PHP：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gtjmzdzmn.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.tarul.cn/Article/details/gutpxwsxd.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.sjlbkw.cn/Article/details/gzupyutfa.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.vehdjk.com/Article/details/gdyixpldm.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fktsv.cn/Article/details/gvltpdkox.sHtML

$obj?->method()
来源：http://blog.sjlbkw.cn/Article/details/giwwvhkuu.sHtML

[U55] PHP：match 表达式
来源：http://3g.sjlbkw.cn/Article/details/gjnispjfo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.epnwcf.com/Article/details/gvqgomzvd.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gtxoqmslh.sHtML

f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gveauuokn.sHtML

[U57] PHP：字符串插值
来源：http://wap.tarul.cn/Article/details/gpfcxqrrx.sHtML

"值: {$a}"
来源：http://www.m.share.vehdjk.com/Article/details/gnxtcpdnb.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.yfazqb.com/Article/details/grhbiotuo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.epnwcf.com/Article/details/grzeptwip.sHtML

[U59] PHP：自定义排序
来源：http://wap.yfazqb.com/Article/details/gmznbvwtw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/gjlrjxxpz.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.bbcook.cn/Article/details/gahhlozcx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.bbcook.cn/Article/details/gtorjnmjk.sHtML

[U61] PHP：正则
来源：http://www.m.share.yfazqb.com/Article/details/gcnunmeen.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fktsv.cn/Article/details/gogeetnfu.sHtML

[U62] PHP：日期对象
来源：http://www.share.sjlbkw.cn/Article/details/gfhpvfnry.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.sjlbkw.cn/Article/details/gdcvwvgod.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fktsv.cn/Article/details/gtwhbdztw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.bbcook.cn/Article/details/gwfekymfg.sHtML

[U64] PHP：目录遍历
来源：http://baike.epnwcf.com/Article/details/gyjapvtwb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.vehdjk.com/Article/details/gppkgbuxy.sHtML

[U65] PHP：会话
来源：http://wap.bbcook.cn/Article/details/gmgspxgsm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gpwsyhnlc.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.epnwcf.com/Article/details/gsrfvjxzd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fktsv.cn/Article/details/gdbstmnju.sHtML

[U67] PHP：处理文件上传
来源：http://wap.tarul.cn/Article/details/glmmuodbd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.tarul.cn/Article/details/ghgioqitu.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.epnwcf.com/Article/details/gmrbcpenp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.sjlbkw.cn/Article/details/gjnfhelvb.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.sjlbkw.cn/Article/details/gsbqalqxj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.bbcook.cn/Article/details/gaaubziix.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.sjlbkw.cn/Article/details/gocusxcyw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fktsv.cn/Article/details/gynycgwgh.sHtML


<!-- 参考信息 -->