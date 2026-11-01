代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://m.share.tarul.cn/Article/details/gapehgmby.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/gvpecvica.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gudubolps.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/gtospkacm.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.vehdjk.com/Article/details/gmqzkceao.sHtML

[S49] C++：写文件
来源：http://read.share.bbcook.cn/Article/details/grlpqqprl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/gazbtchtx.sHtML

[S50] C++：格式化数字
来源：http://read.share.sjlbkw.cn/Article/details/gksbmarkj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gwbwcapyl.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gfagoloqj.sHtML

static_cast<double>(a) / b
来源：http://m.share.sjlbkw.cn/Article/details/gfrcxpdfk.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/gegmiygtw.sHtML

int size() const noexcept { return n_; }
来源：http://3g.bbcook.cn/Article/details/gwfptcqtq.sHtML

[S53] C++：移动语义
来源：http://wap.yfazqb.com/Article/details/geftmeena.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.vehdjk.com/Article/details/gqibpqijv.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/gyowmjjrx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gzkknhmkn.sHtML

[S55] C++：结构化绑定
来源：http://read.share.tarul.cn/Article/details/godlerwda.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.tarul.cn/Article/details/gwuzppejy.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/gzthtzwff.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.epnwcf.com/Article/details/gfanbqgry.sHtML

[S57] C++：编译期常量
来源：http://m.share.vehdjk.com/Article/details/gmxwzduqy.sHtML

constexpr int N = 10;
来源：http://wap.tarul.cn/Article/details/ghqttusdv.sHtML

[S58] C++：命名空间
来源：http://www.share.fktsv.cn/Article/details/gsrcqqaxo.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fktsv.cn/Article/details/gcyjdpyls.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/gfabfqatw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/gsvkqrnpw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.yfazqb.com/Article/details/ggynvrgny.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.yfazqb.com/Article/details/gnscljvfa.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/goyesihmn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.bbcook.cn/Article/details/ghbcozzsw.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpelohpuu.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fktsv.cn/Article/details/gsmatyhri.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gpzcsksij.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gjzzuhdye.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.yfazqb.com/Article/details/gbkgcpqur.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/giqtnbrfe.sHtML

"值: $b"
来源：http://3g.bbcook.cn/Article/details/gjripdzbu.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fktsv.cn/Article/details/gmeofkpqk.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fktsv.cn/Article/details/gstpaqjvk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gspwjxobp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.yfazqb.com/Article/details/gavbspmgo.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/glmypjvma.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fktsv.cn/Article/details/gyyhwjqcq.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.bbcook.cn/Article/details/gktnjwrbm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fktsv.cn/Article/details/gjvnoveno.sHtML

[T08] Kotlin：数据类
来源：http://mobile.yfazqb.com/Article/details/ghhzddjay.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/guyykhzti.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.tarul.cn/Article/details/goubceegy.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.bbcook.cn/Article/details/gtevfxacx.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fktsv.cn/Article/details/ggswhyibu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.tarul.cn/Article/details/gzwkpykfk.sHtML

[T11] Kotlin：协程
来源：http://blog.sjlbkw.cn/Article/details/gyaiikovq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.epnwcf.com/Article/details/gplmewdxu.sHtML

[T12] Kotlin：解构声明
来源：http://wap.tarul.cn/Article/details/ggocuhvyv.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.tarul.cn/Article/details/gwikvczqp.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.epnwcf.com/Article/details/glcpmszwx.sHtML

val m = mapOf("a" to 1)
来源：http://blog.sjlbkw.cn/Article/details/gbmgkdsug.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gnslayaph.sHtML

for (i in 1..10) println(i)
来源：http://3g.fktsv.cn/Article/details/gfmujkvkw.sHtML

[T15] Kotlin：接口
来源：http://www.blog.yfazqb.com/Article/details/gbgmkorwf.sHtML

interface Shape { fun area(): Double }
来源：http://baike.vehdjk.com/Article/details/gdpyikeit.sHtML

[T16] Swift：Hello World
来源：http://3g.vehdjk.com/Article/details/gexacmide.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/gxvsanjuf.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.bbcook.cn/Article/details/gokrknrbq.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gcjmjuuii.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gnspobtdy.sHtML

"值: \(b)"
来源：http://blog.vehdjk.com/Article/details/gxghhekal.sHtML

[T19] Swift：可选绑定
来源：http://wap.fktsv.cn/Article/details/gxlfgqijo.sHtML

if let n = opt { print(n) }
来源：http://read.share.tarul.cn/Article/details/gcqzvmhxi.sHtML

[T20] Swift：数组操作
来源：http://3g.tarul.cn/Article/details/gmjaufcrp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fktsv.cn/Article/details/gimupsfiw.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/ggcgabmyp.sHtML

for x in a { print(x) }
来源：http://blog.tarul.cn/Article/details/gttrggaov.sHtML

[T22] Swift：字典
来源：http://mobile.vehdjk.com/Article/details/gbvydgarb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.vehdjk.com/Article/details/gjltudisj.sHtML

[T23] Swift：函数
来源：http://www.share.fktsv.cn/Article/details/gcphhpkae.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gkmokphjt.sHtML

[T24] Swift：闭包
来源：http://mobile.bbcook.cn/Article/details/grklisble.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gxhlpbviq.sHtML

[T25] Swift：结构体
来源：http://baike.epnwcf.com/Article/details/goduuztiz.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/gyzqclmwx.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/gnldmjkfp.sHtML

class A: Base { override func f() {} }
来源：http://baike.sjlbkw.cn/Article/details/greqmezhp.sHtML

[T27] Swift：错误处理
来源：http://3g.fktsv.cn/Article/details/geeioauts.sHtML

do { try f() } catch { print(error) }
来源：http://baike.yfazqb.com/Article/details/gioepizzw.sHtML

[T28] Swift：枚举
来源：http://www.blog.vehdjk.com/Article/details/gipfoqvqi.sHtML

enum Color { case red, green }
来源：http://www.blog.sjlbkw.cn/Article/details/gbydriuyq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gfksyuraa.sHtML

guard let x = opt else { return }
来源：http://www.blog.vehdjk.com/Article/details/gyzmnhrfa.sHtML

[T30] Swift：协议
来源：http://www.m.share.tarul.cn/Article/details/giikrrirg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fktsv.cn/Article/details/gtolchvsf.sHtML

[T31] Lua：Hello World
来源：http://www.share.yfazqb.com/Article/details/ggxfnfuoq.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gzmlppzcl.sHtML

[T32] Lua：局部变量
来源：http://blog.bbcook.cn/Article/details/gnhmpooft.sHtML

local a = 1
来源：http://3g.yfazqb.com/Article/details/ghzalgbvz.sHtML

[T33] Lua：表（数组）
来源：http://blog.fktsv.cn/Article/details/ghqkwmxvt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.tarul.cn/Article/details/gifpyxprm.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gvmtpkhsl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.bbcook.cn/Article/details/gimgctzzs.sHtML

[T35] Lua：字典表
来源：http://www.blog.fktsv.cn/Article/details/gsdmlgbza.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.yfazqb.com/Article/details/gycptjaeq.sHtML

[T36] Lua：函数
来源：http://www.share.yfazqb.com/Article/details/gzcrkxxlj.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.yfazqb.com/Article/details/gjwinehnd.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gsqgmdfuw.sHtML

"a" .. "b"
来源：http://wap.sjlbkw.cn/Article/details/gkwuvqrgu.sHtML

[T38] Lua：条件
来源：http://blog.epnwcf.com/Article/details/gqrkvdjvl.sHtML

if x > 0 then print("正") end
来源：http://3g.tarul.cn/Article/details/gjnwllmsr.sHtML

[T39] Lua：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gvmimalbt.sHtML

string.find(s, "%d+")
来源：http://mobile.fktsv.cn/Article/details/gkghptmbd.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/gydcgnana.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.bbcook.cn/Article/details/gzizwciqy.sHtML

[T41] Perl：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gfrxdbjkq.sHtML

print "Hello\n";
来源：http://wap.epnwcf.com/Article/details/gdjfgyhay.sHtML

[T42] Perl：变量类型
来源：http://blog.vehdjk.com/Article/details/gsekghkxw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fktsv.cn/Article/details/gcfzcoare.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gandirxtc.sHtML

"值: $a"
来源：http://mobile.tarul.cn/Article/details/gbxqzcckz.sHtML

[T44] Perl：条件
来源：http://read.share.bbcook.cn/Article/details/gfilsaaqv.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.epnwcf.com/Article/details/gvkzicgtp.sHtML

[T45] Perl：数组遍历
来源：http://mobile.tarul.cn/Article/details/gakbcsrxa.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.bbcook.cn/Article/details/gdnqsfppu.sHtML

[T46] Perl：哈希操作
来源：http://read.share.bbcook.cn/Article/details/ggnmjvnwe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fktsv.cn/Article/details/gvdgbipco.sHtML

[T47] Perl：正则捕获
来源：http://www.share.sjlbkw.cn/Article/details/gtkmpshpp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.tarul.cn/Article/details/ggmyirdyj.sHtML

[T48] Perl：正则替换
来源：http://baike.tarul.cn/Article/details/goayxgbdl.sHtML

$s =~ s/old/new/g;
来源：http://baike.tarul.cn/Article/details/gvmatthdc.sHtML

[T49] Perl：函数
来源：http://baike.bbcook.cn/Article/details/gtwptbjny.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gtxvoeydw.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.tarul.cn/Article/details/ghfrxgpvh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.vehdjk.com/Article/details/goflkerxw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fktsv.cn/Article/details/gphzfvgfa.sHtML

[T51] Scala：Hello World
来源：http://3g.epnwcf.com/Article/details/ghibluait.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/gnynrgutl.sHtML

[T52] Scala：变量
来源：http://www.m.share.yfazqb.com/Article/details/gonjvjsdj.sHtML

val a = 1;  var b = 2
来源：http://wap.bbcook.cn/Article/details/grtjsedvq.sHtML

[T53] Scala：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gjvtocbhn.sHtML

s"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gsjkqcanz.sHtML

[T54] Scala：集合映射
来源：http://m.share.yfazqb.com/Article/details/gxohhungw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fktsv.cn/Article/details/gqeoozapa.sHtML

[T55] Scala：集合过滤
来源：http://baike.fktsv.cn/Article/details/gjsjgcgdb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.bbcook.cn/Article/details/ghfmessbw.sHtML

[T56] Scala：样例类
来源：http://read.share.yfazqb.com/Article/details/gshakkwfj.sHtML

case class User(name: String, age: Int)
来源：http://mobile.tarul.cn/Article/details/ggdmswvmj.sHtML

[T57] Scala：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gsafojdgh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fktsv.cn/Article/details/ghyqaniox.sHtML

[T58] Scala：函数定义
来源：http://wap.sjlbkw.cn/Article/details/gbmgyegam.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.sjlbkw.cn/Article/details/gaaxzfiqj.sHtML

[T59] Scala：循环
来源：http://wap.sjlbkw.cn/Article/details/gtvlxxzdf.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fktsv.cn/Article/details/gnzvtwzox.sHtML

[T60] Scala：折叠
来源：http://3g.tarul.cn/Article/details/gljsgdeib.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.tarul.cn/Article/details/gvymgfiuu.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gqwmhktfd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.epnwcf.com/Article/details/gqttwxria.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzipfsknh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.tarul.cn/Article/details/ghnklftsp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.tarul.cn/Article/details/gojnwfpvp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/gldhlwcis.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.yfazqb.com/Article/details/gomikzhse.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.bbcook.cn/Article/details/gntctxqxr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.yfazqb.com/Article/details/gdiskvkbp.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.epnwcf.com/Article/details/gdwwdidmj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.vehdjk.com/Article/details/gbrbrkkxv.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.vehdjk.com/Article/details/gsbvhjwpy.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fktsv.cn/Article/details/gqtosvvse.sHtML

[U06] Py：合并两个字典
来源：http://baike.tarul.cn/Article/details/gksxwmafh.sHtML

{**a, **b}
来源：http://read.share.sjlbkw.cn/Article/details/gsuvhrktq.sHtML

[U07] Py：反转字典键值
来源：http://3g.yfazqb.com/Article/details/gkvyxdbhy.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.vehdjk.com/Article/details/ghpmcuhmx.sHtML

[U08] Py：展平二维列表
来源：http://www.share.sjlbkw.cn/Article/details/gtgkmlpzh.sHtML

[y for x in nested for y in x]
来源：http://blog.tarul.cn/Article/details/gcudrvjng.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.bbcook.cn/Article/details/gpcyrjddr.sHtML

max(d, key=d.get)
来源：http://3g.sjlbkw.cn/Article/details/gjwbyrfqz.sHtML

[U10] Py：按值排序字典
来源：http://m.share.bbcook.cn/Article/details/gapgsjpsg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.vehdjk.com/Article/details/gpejpcfke.sHtML

[U11] Py：生成器表达式
来源：http://read.share.bbcook.cn/Article/details/gfaliiaof.sHtML

(x * 2 for x in arr)
来源：http://mobile.vehdjk.com/Article/details/gykmmpjgw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.yfazqb.com/Article/details/grbxxmnat.sHtML

Counter(arr).most_common(3)
来源：http://read.share.yfazqb.com/Article/details/glbwwqhwn.sHtML

[U13] Py：固定长度队列
来源：http://mobile.sjlbkw.cn/Article/details/gbrarfvlc.sHtML

deque(maxlen=10)
来源：http://m.share.vehdjk.com/Article/details/gmqmwmiss.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.sjlbkw.cn/Article/details/gnwtybdrn.sHtML

defaultdict(list)
来源：http://mobile.tarul.cn/Article/details/geigciikr.sHtML

[U15] Py：高精度计时
来源：http://mobile.epnwcf.com/Article/details/ghdislixc.sHtML

t = time.perf_counter()
来源：http://read.share.fktsv.cn/Article/details/grgxfemsb.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.yfazqb.com/Article/details/gnmvjuyno.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.sjlbkw.cn/Article/details/giazltmmy.sHtML

[U17] Py：初始化日志
来源：http://baike.sjlbkw.cn/Article/details/gqaevvuez.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.vehdjk.com/Article/details/gakvpieqp.sHtML

[U18] Py：预编译正则
来源：http://baike.vehdjk.com/Article/details/gaybnczkm.sHtML

pat = re.compile(r"\d+")
来源：http://baike.vehdjk.com/Article/details/geydvirjp.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.sjlbkw.cn/Article/details/gonlnopua.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.tarul.cn/Article/details/gflbzuqrf.sHtML

[U20] Py：缓存函数结果
来源：http://blog.epnwcf.com/Article/details/gyagzvqvx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.vehdjk.com/Article/details/gvlvhvrow.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.yfazqb.com/Article/details/godiekhqb.sHtML

@contextlib.contextmanager
来源：http://mobile.vehdjk.com/Article/details/gdvzrtjjy.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fktsv.cn/Article/details/gzkompwgu.sHtML

list(zip(*m))
来源：http://www.blog.vehdjk.com/Article/details/giyofxfpa.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.yfazqb.com/Article/details/gawqeyuds.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.yfazqb.com/Article/details/gkakccxso.sHtML

[U24] Py：路径操作
来源：http://wap.epnwcf.com/Article/details/guvihnivk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/gonhsqavh.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.tarul.cn/Article/details/gdpjrmxyg.sHtML

csv.DictReader(f)
来源：http://blog.fktsv.cn/Article/details/gwjevewkb.sHtML

[U26] Py：并发下载
来源：http://www.m.share.tarul.cn/Article/details/gsgzebfwg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.vehdjk.com/Article/details/guvmylvzs.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fktsv.cn/Article/details/gybjpdgrz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.vehdjk.com/Article/details/gdtkibcia.sHtML

[U28] Py：类型别名
来源：http://wap.fktsv.cn/Article/details/gmkbsxjce.sHtML

UserId = int
来源：http://www.blog.vehdjk.com/Article/details/ggmpxlwpq.sHtML

[U29] Py：属性校验
来源：http://m.share.bbcook.cn/Article/details/gvymmdotp.sHtML

@property 与 @x.setter 配合
来源：http://www.share.epnwcf.com/Article/details/gqbagbage.sHtML

[U30] Py：数据类
来源：http://www.m.share.fktsv.cn/Article/details/gbyowezex.sHtML

@dataclass(slots=True)
来源：http://baike.fktsv.cn/Article/details/ghhnioogt.sHtML

[U31] Py：单测
来源：http://www.blog.sjlbkw.cn/Article/details/grqxygqex.sHtML

python -m pytest -q
来源：http://www.share.sjlbkw.cn/Article/details/gmeclaspj.sHtML

[U32] Py：代码格式化
来源：http://wap.fktsv.cn/Article/details/gxgzsirsk.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.tarul.cn/Article/details/gobkajdom.sHtML

[U33] Py：打包发布
来源：http://wap.epnwcf.com/Article/details/gdlmhqfkf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.vehdjk.com/Article/details/gyajjuzpe.sHtML

[U34] Py：判断编码
来源：http://www.blog.bbcook.cn/Article/details/ggmpxbedn.sHtML

chardet.detect(raw)
来源：http://wap.bbcook.cn/Article/details/gxatchxzq.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fktsv.cn/Article/details/glakfhkee.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.vehdjk.com/Article/details/gsnpkpdlr.sHtML

[U36] Py：定时任务
来源：http://m.share.fktsv.cn/Article/details/gmztdohhr.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fktsv.cn/Article/details/ggimalmos.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fktsv.cn/Article/details/glcwzfemj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.yfazqb.com/Article/details/gazqqqkxb.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.sjlbkw.cn/Article/details/gdgjcfswe.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fktsv.cn/Article/details/gqaovskor.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.sjlbkw.cn/Article/details/gwgxenfmr.sHtML

sys.stdout.isatty()
来源：http://www.share.yfazqb.com/Article/details/gitlyiccx.sHtML

[U40] Py：打印到标准错误
来源：http://wap.yfazqb.com/Article/details/ghgdkrrcs.sHtML

print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/gwgwkogfb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.epnwcf.com/Article/details/glrwjombq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.sjlbkw.cn/Article/details/gggmfeici.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fktsv.cn/Article/details/gypinjqdc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.tarul.cn/Article/details/gnxihoteb.sHtML

[U43] PHP：声明命名空间
来源：http://wap.bbcook.cn/Article/details/glksxjnaw.sHtML

namespace App\Http;
来源：http://3g.yfazqb.com/Article/details/gpbstdvls.sHtML

[U44] PHP：开启严格类型
来源：http://baike.epnwcf.com/Article/details/gohkyrkde.sHtML

declare(strict_types=1);
来源：http://m.share.tarul.cn/Article/details/gtgkxmiwd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.epnwcf.com/Article/details/gbxnrfseq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gbsphllvu.sHtML

[U46] PHP：可空类型
来源：http://www.share.tarul.cn/Article/details/gslrpeqty.sHtML

?string $name = null
来源：http://mobile.bbcook.cn/Article/details/ggbyiuutj.sHtML

[U47] PHP：联合类型
来源：http://read.share.sjlbkw.cn/Article/details/gzsgxfwpg.sHtML

int|string $id
来源：http://www.m.share.vehdjk.com/Article/details/gkrdvloxq.sHtML

[U48] PHP：纯枚举
来源：http://3g.sjlbkw.cn/Article/details/gywqqbnyi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.yfazqb.com/Article/details/gyoheyevp.sHtML

[U49] PHP：只读属性
来源：http://www.share.bbcook.cn/Article/details/gqgoacctf.sHtML

public readonly string $name
来源：http://www.share.sjlbkw.cn/Article/details/gyhjxwbgc.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.sjlbkw.cn/Article/details/glolhflyk.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.epnwcf.com/Article/details/gbecpdoce.sHtML

[U51] PHP：数组解构
来源：http://www.share.sjlbkw.cn/Article/details/gmlrdtbrp.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.vehdjk.com/Article/details/gbmlpbiqm.sHtML

[U52] PHP：箭头函数
来源：http://blog.vehdjk.com/Article/details/gbiosyrmu.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.sjlbkw.cn/Article/details/gwasdpbmp.sHtML

[U53] PHP：空合并运算符
来源：http://baike.epnwcf.com/Article/details/gnbjheryl.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fktsv.cn/Article/details/grwehorkt.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.bbcook.cn/Article/details/gcanmjtds.sHtML

$obj?->method()
来源：http://www.m.share.vehdjk.com/Article/details/goeeoxwle.sHtML

[U55] PHP：match 表达式
来源：http://blog.epnwcf.com/Article/details/gurhfzluo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.bbcook.cn/Article/details/gvfspvtxa.sHtML

[U56] PHP：命名参数
来源：http://wap.bbcook.cn/Article/details/gaudbktxc.sHtML

f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/graroqyic.sHtML

[U57] PHP：字符串插值
来源：http://blog.epnwcf.com/Article/details/ghxfqdjpa.sHtML

"值: {$a}"
来源：http://www.blog.sjlbkw.cn/Article/details/guylsqlyy.sHtML

[U58] PHP：数组三件套
来源：http://3g.tarul.cn/Article/details/grqufqbur.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.tarul.cn/Article/details/gcpukkyxc.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.tarul.cn/Article/details/gcznqiinq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gxhyrakve.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.vehdjk.com/Article/details/gwutioive.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.yfazqb.com/Article/details/gjxplgfgn.sHtML

[U61] PHP：正则
来源：http://read.share.fktsv.cn/Article/details/gowsivphm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/gkmgqkwxe.sHtML

[U62] PHP：日期对象
来源：http://blog.tarul.cn/Article/details/grihipxcx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.tarul.cn/Article/details/ggwtuhdnm.sHtML

[U63] PHP：文件读写
来源：http://baike.fktsv.cn/Article/details/gedrjvrgq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.sjlbkw.cn/Article/details/gumcddbdh.sHtML

[U64] PHP：目录遍历
来源：http://www.share.vehdjk.com/Article/details/gjcwgyejd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.vehdjk.com/Article/details/gdgkgeupt.sHtML

[U65] PHP：会话
来源：http://wap.vehdjk.com/Article/details/gbqwxjrhp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gxsdvlppz.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.bbcook.cn/Article/details/gdygxyhwf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.sjlbkw.cn/Article/details/gujxfrasm.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.tarul.cn/Article/details/gcimrxfrk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.epnwcf.com/Article/details/gmqlafdwp.sHtML

[U68] PHP：PDO 连接
来源：http://blog.bbcook.cn/Article/details/gmqehpmiw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.vehdjk.com/Article/details/gqnmdjszt.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.bbcook.cn/Article/details/gpzepcctu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.tarul.cn/Article/details/gfxwelisx.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.tarul.cn/Article/details/gooyuypgb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.tarul.cn/Article/details/ggxriycgk.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fktsv.cn/Article/details/ggpojhsld.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.tarul.cn/Article/details/gbkqqewcs.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.yfazqb.com/Article/details/gtiiwjncw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.sjlbkw.cn/Article/details/grsqejjyo.sHtML


<!-- 参考信息 -->