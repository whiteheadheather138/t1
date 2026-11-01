代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://3g.bbcook.cn/Article/details/grokwjbqt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/grwkuavca.sHtML

[S48] C++：逐行读文件
来源：http://read.share.tarul.cn/Article/details/grwkpcyhx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.bbcook.cn/Article/details/gshcxocit.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.vehdjk.com/Article/details/goduozstr.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/gjbicsefr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/gyuotwjik.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/godmkrcbe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gyizheghb.sHtML

[S51] C++：显式类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gtpvctkfv.sHtML

static_cast<double>(a) / b
来源：http://wap.tarul.cn/Article/details/gcragrjuo.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.tarul.cn/Article/details/gyasrfvmm.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.sjlbkw.cn/Article/details/gkyyamfim.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gjoagwjdt.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/gvxhryate.sHtML

[S54] C++：异常处理
来源：http://m.share.yfazqb.com/Article/details/gsdmshxbl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.sjlbkw.cn/Article/details/gfapzxtmu.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/giykcilvw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.bbcook.cn/Article/details/ggosaxdug.sHtML

[S56] C++：optional
来源：http://read.share.vehdjk.com/Article/details/gxbugtecp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fktsv.cn/Article/details/gydqbjahi.sHtML

[S57] C++：编译期常量
来源：http://m.share.yfazqb.com/Article/details/grnsheivy.sHtML

constexpr int N = 10;
来源：http://3g.fktsv.cn/Article/details/gnojqagpa.sHtML

[S58] C++：命名空间
来源：http://www.blog.fktsv.cn/Article/details/gbaubyngy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.bbcook.cn/Article/details/gggxwlrxn.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/gkjtjheos.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.bbcook.cn/Article/details/gchsidvmq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.tarul.cn/Article/details/gymezhodc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.tarul.cn/Article/details/gadkmtjre.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gxrldcche.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/gsrepslpz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gbbxhqlkt.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gcjxjzjpd.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gxpfbunja.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fktsv.cn/Article/details/gcbtkjvpd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.vehdjk.com/Article/details/glqylzacl.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.bbcook.cn/Article/details/gzieoxvpd.sHtML

"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gageygvrt.sHtML

[T04] Kotlin：空安全
来源：http://blog.vehdjk.com/Article/details/gwwnumlhq.sHtML

val n: String? = null;  n?.length
来源：http://3g.fktsv.cn/Article/details/glemuyhnd.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.vehdjk.com/Article/details/gvapgjdzg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/gcfyjmhyy.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.epnwcf.com/Article/details/gnucozndl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.vehdjk.com/Article/details/gutvtjlon.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gvdpyxkys.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/ghxptudkh.sHtML

[T08] Kotlin：数据类
来源：http://3g.tarul.cn/Article/details/gokbbweay.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.yfazqb.com/Article/details/gkjljmuhm.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.epnwcf.com/Article/details/gjvaldhtc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.vehdjk.com/Article/details/gjpvaolgp.sHtML

[T10] Kotlin：默认参数
来源：http://3g.vehdjk.com/Article/details/gmbihjouq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.vehdjk.com/Article/details/gcqjvbphd.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gzrhkzfrf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.tarul.cn/Article/details/gtyfffiio.sHtML

[T12] Kotlin：解构声明
来源：http://3g.vehdjk.com/Article/details/gbjgwshgh.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/gammhjtat.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.tarul.cn/Article/details/gmezodwyk.sHtML

val m = mapOf("a" to 1)
来源：http://blog.tarul.cn/Article/details/grudpqzxf.sHtML

[T14] Kotlin：循环
来源：http://m.share.bbcook.cn/Article/details/giyppzjoq.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gteqjhwnf.sHtML

[T15] Kotlin：接口
来源：http://m.share.sjlbkw.cn/Article/details/gzfdzgjfl.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gryhlvxqv.sHtML

[T16] Swift：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gzraudvab.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gyyilvfmh.sHtML

[T17] Swift：变量与常量
来源：http://blog.vehdjk.com/Article/details/gpewcoovo.sHtML

var a = 1;  let b = 2
来源：http://www.blog.vehdjk.com/Article/details/ggkvltrcv.sHtML

[T18] Swift：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gpglcnvor.sHtML

"值: \(b)"
来源：http://read.share.fktsv.cn/Article/details/gaxukaqbv.sHtML

[T19] Swift：可选绑定
来源：http://blog.sjlbkw.cn/Article/details/gvkuqfmbf.sHtML

if let n = opt { print(n) }
来源：http://3g.epnwcf.com/Article/details/gkyhvkpbs.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.bbcook.cn/Article/details/gxttxgiju.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.epnwcf.com/Article/details/gjzwqkgjt.sHtML

[T21] Swift：遍历
来源：http://www.share.bbcook.cn/Article/details/gkobbxzxq.sHtML

for x in a { print(x) }
来源：http://3g.bbcook.cn/Article/details/gpdyfubpz.sHtML

[T22] Swift：字典
来源：http://blog.sjlbkw.cn/Article/details/ghbylfbdr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.epnwcf.com/Article/details/ggpxdayzg.sHtML

[T23] Swift：函数
来源：http://blog.bbcook.cn/Article/details/glztjbqqu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/goxlwjeiq.sHtML

[T24] Swift：闭包
来源：http://www.share.sjlbkw.cn/Article/details/gvngeauvr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/ggvdpfhfa.sHtML

[T25] Swift：结构体
来源：http://m.share.epnwcf.com/Article/details/goeucjzfl.sHtML

struct P { var x: Int }
来源：http://baike.tarul.cn/Article/details/gdwdcqwsy.sHtML

[T26] Swift：类与重写
来源：http://wap.yfazqb.com/Article/details/gvpdjrkae.sHtML

class A: Base { override func f() {} }
来源：http://read.share.bbcook.cn/Article/details/gglrnjamg.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gsgrfpoik.sHtML

do { try f() } catch { print(error) }
来源：http://3g.epnwcf.com/Article/details/ghfxqkhly.sHtML

[T28] Swift：枚举
来源：http://www.blog.epnwcf.com/Article/details/gvsjsfkda.sHtML

enum Color { case red, green }
来源：http://mobile.vehdjk.com/Article/details/gcfjovzda.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/gerquglwn.sHtML

guard let x = opt else { return }
来源：http://read.share.yfazqb.com/Article/details/grfhgswfg.sHtML

[T30] Swift：协议
来源：http://www.blog.tarul.cn/Article/details/gyikoqeoo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fktsv.cn/Article/details/gpumcaoby.sHtML

[T31] Lua：Hello World
来源：http://wap.fktsv.cn/Article/details/grdxmxcnf.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gidsnyxnp.sHtML

[T32] Lua：局部变量
来源：http://www.share.vehdjk.com/Article/details/gguqwrtgx.sHtML

local a = 1
来源：http://read.share.sjlbkw.cn/Article/details/glcsosves.sHtML

[T33] Lua：表（数组）
来源：http://baike.tarul.cn/Article/details/gazdlkjhw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fktsv.cn/Article/details/ggjygomtc.sHtML

[T34] Lua：遍历表
来源：http://blog.yfazqb.com/Article/details/gjkqzzntc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.epnwcf.com/Article/details/gjczlqffv.sHtML

[T35] Lua：字典表
来源：http://mobile.sjlbkw.cn/Article/details/gexlxihhs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.vehdjk.com/Article/details/ggsizrfus.sHtML

[T36] Lua：函数
来源：http://read.share.bbcook.cn/Article/details/ggtuxvqss.sHtML

function add(a, b) return a + b end
来源：http://m.share.epnwcf.com/Article/details/gqvaysteo.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.tarul.cn/Article/details/grgalmewb.sHtML

"a" .. "b"
来源：http://read.share.tarul.cn/Article/details/glyjrhoza.sHtML

[T38] Lua：条件
来源：http://www.blog.fktsv.cn/Article/details/gziruopnk.sHtML

if x > 0 then print("正") end
来源：http://blog.epnwcf.com/Article/details/gcsevabcl.sHtML

[T39] Lua：模式匹配
来源：http://blog.yfazqb.com/Article/details/gsngqjbta.sHtML

string.find(s, "%d+")
来源：http://blog.fktsv.cn/Article/details/gqhwfyiem.sHtML

[T40] Lua：元表
来源：http://www.m.share.vehdjk.com/Article/details/gyittmghk.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fktsv.cn/Article/details/grcbifrdl.sHtML

[T41] Perl：Hello World
来源：http://3g.bbcook.cn/Article/details/gknoszole.sHtML

print "Hello\n";
来源：http://read.share.tarul.cn/Article/details/gosbivzfy.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.vehdjk.com/Article/details/gbtckplwz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.sjlbkw.cn/Article/details/gxwcjkbud.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gnlptayjw.sHtML

"值: $a"
来源：http://blog.bbcook.cn/Article/details/gtixagcrw.sHtML

[T44] Perl：条件
来源：http://wap.epnwcf.com/Article/details/gmzigtmoq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.tarul.cn/Article/details/gpfafmdzh.sHtML

[T45] Perl：数组遍历
来源：http://m.share.bbcook.cn/Article/details/gxkgleqva.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.vehdjk.com/Article/details/gubzsetno.sHtML

[T46] Perl：哈希操作
来源：http://3g.yfazqb.com/Article/details/gftvqfwsj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/gggdsvjyq.sHtML

[T47] Perl：正则捕获
来源：http://3g.yfazqb.com/Article/details/geuwavmga.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.bbcook.cn/Article/details/gqwuareiv.sHtML

[T48] Perl：正则替换
来源：http://www.blog.epnwcf.com/Article/details/gskzobclr.sHtML

$s =~ s/old/new/g;
来源：http://3g.tarul.cn/Article/details/ggqqmxeix.sHtML

[T49] Perl：函数
来源：http://wap.vehdjk.com/Article/details/gzsqlsylg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gbqkrooos.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.tarul.cn/Article/details/gvoyhqilk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fktsv.cn/Article/details/gelhmcwjb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.epnwcf.com/Article/details/guocsrqdj.sHtML

[T51] Scala：Hello World
来源：http://baike.yfazqb.com/Article/details/gcnnhxaxe.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/gvcpzmmra.sHtML

[T52] Scala：变量
来源：http://baike.tarul.cn/Article/details/gszynnscl.sHtML

val a = 1;  var b = 2
来源：http://www.share.tarul.cn/Article/details/gzgvsyinq.sHtML

[T53] Scala：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gxzgywehj.sHtML

s"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/gdidajinf.sHtML

[T54] Scala：集合映射
来源：http://blog.yfazqb.com/Article/details/gmubndbst.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.vehdjk.com/Article/details/gdxpshxad.sHtML

[T55] Scala：集合过滤
来源：http://3g.bbcook.cn/Article/details/ggfwkspqv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.yfazqb.com/Article/details/ghfqkhadj.sHtML

[T56] Scala：样例类
来源：http://www.share.vehdjk.com/Article/details/gsndkvzyh.sHtML

case class User(name: String, age: Int)
来源：http://baike.fktsv.cn/Article/details/gjmkjbvnx.sHtML

[T57] Scala：模式匹配
来源：http://blog.epnwcf.com/Article/details/ggsoiudny.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.bbcook.cn/Article/details/gchtpqeic.sHtML

[T58] Scala：函数定义
来源：http://www.blog.vehdjk.com/Article/details/gybidvtyo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.epnwcf.com/Article/details/gsgstzzhq.sHtML

[T59] Scala：循环
来源：http://m.share.bbcook.cn/Article/details/goyfzgujf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/gtmizsmcm.sHtML

[T60] Scala：折叠
来源：http://www.blog.tarul.cn/Article/details/glqpzquik.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.yfazqb.com/Article/details/grkkdcldw.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gwbspslhe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gvikrdeih.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsvpnsouq.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.tarul.cn/Article/details/ggfmrsyaa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.sjlbkw.cn/Article/details/gpchytfmv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.tarul.cn/Article/details/gyidrxxvi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.yfazqb.com/Article/details/glydfsazy.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.epnwcf.com/Article/details/guzaxbmwq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.epnwcf.com/Article/details/gtrnqcjrk.sHtML

[U04] Py：变量调试打印
来源：http://blog.sjlbkw.cn/Article/details/gxydxbduk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.sjlbkw.cn/Article/details/golgapzdz.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.bbcook.cn/Article/details/gqrjuhnql.sHtML

list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gwtvlqtwc.sHtML

[U06] Py：合并两个字典
来源：http://m.share.tarul.cn/Article/details/geqjkiacb.sHtML

{**a, **b}
来源：http://www.share.yfazqb.com/Article/details/gwfjxrfug.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.epnwcf.com/Article/details/golkszrrv.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gfokcoslb.sHtML

[U08] Py：展平二维列表
来源：http://3g.epnwcf.com/Article/details/gtstbaudt.sHtML

[y for x in nested for y in x]
来源：http://www.blog.yfazqb.com/Article/details/guxcgnwdv.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fktsv.cn/Article/details/gdyjudlbm.sHtML

max(d, key=d.get)
来源：http://blog.yfazqb.com/Article/details/gnclgkpvo.sHtML

[U10] Py：按值排序字典
来源：http://m.share.sjlbkw.cn/Article/details/gicbegbrp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fktsv.cn/Article/details/gmcoowzxo.sHtML

[U11] Py：生成器表达式
来源：http://m.share.epnwcf.com/Article/details/gfcmcyonr.sHtML

(x * 2 for x in arr)
来源：http://read.share.fktsv.cn/Article/details/gqdiocriz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.epnwcf.com/Article/details/gpevndvvr.sHtML

Counter(arr).most_common(3)
来源：http://3g.sjlbkw.cn/Article/details/gjdayrlha.sHtML

[U13] Py：固定长度队列
来源：http://www.share.epnwcf.com/Article/details/gzutrgrwl.sHtML

deque(maxlen=10)
来源：http://read.share.epnwcf.com/Article/details/glxftxsor.sHtML

[U14] Py：分组收集到列表
来源：http://wap.tarul.cn/Article/details/ghwqolnva.sHtML

defaultdict(list)
来源：http://mobile.bbcook.cn/Article/details/gfdgsnovi.sHtML

[U15] Py：高精度计时
来源：http://read.share.tarul.cn/Article/details/gnsaonvpq.sHtML

t = time.perf_counter()
来源：http://read.share.yfazqb.com/Article/details/gannvurux.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.tarul.cn/Article/details/gjxjntqmc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.tarul.cn/Article/details/gmtixrycc.sHtML

[U17] Py：初始化日志
来源：http://m.share.bbcook.cn/Article/details/gxypbdcsr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwczaimdv.sHtML

[U18] Py：预编译正则
来源：http://m.share.epnwcf.com/Article/details/gdnsyyeju.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gtcaacpld.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.tarul.cn/Article/details/gdabwqiir.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.bbcook.cn/Article/details/grvxenpmm.sHtML

[U20] Py：缓存函数结果
来源：http://baike.yfazqb.com/Article/details/gkvlvacwc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.yfazqb.com/Article/details/gkbsaqgfy.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.sjlbkw.cn/Article/details/ginqqcupd.sHtML

@contextlib.contextmanager
来源：http://www.m.share.tarul.cn/Article/details/gfftlkeaf.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhwyqncx.sHtML

list(zip(*m))
来源：http://www.blog.bbcook.cn/Article/details/gftqnrdod.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fktsv.cn/Article/details/gqlkfmsqe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.tarul.cn/Article/details/glswceaiv.sHtML

[U24] Py：路径操作
来源：http://www.blog.sjlbkw.cn/Article/details/gkbhfpqic.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gqeierxbq.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.vehdjk.com/Article/details/govjpmfwg.sHtML

csv.DictReader(f)
来源：http://baike.epnwcf.com/Article/details/gdbzktoqo.sHtML

[U26] Py：并发下载
来源：http://m.share.fktsv.cn/Article/details/gbyotmoui.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.vehdjk.com/Article/details/grtiepxhd.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.vehdjk.com/Article/details/gfgehvdxr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.epnwcf.com/Article/details/ggldhwoow.sHtML

[U28] Py：类型别名
来源：http://wap.vehdjk.com/Article/details/gceaanklh.sHtML

UserId = int
来源：http://3g.tarul.cn/Article/details/gkkvozngw.sHtML

[U29] Py：属性校验
来源：http://3g.epnwcf.com/Article/details/ggiiitppb.sHtML

@property 与 @x.setter 配合
来源：http://wap.sjlbkw.cn/Article/details/gssiysqqh.sHtML

[U30] Py：数据类
来源：http://3g.tarul.cn/Article/details/gxaacklef.sHtML

@dataclass(slots=True)
来源：http://m.share.sjlbkw.cn/Article/details/gutrynnrl.sHtML

[U31] Py：单测
来源：http://www.m.share.sjlbkw.cn/Article/details/gguzhyzrw.sHtML

python -m pytest -q
来源：http://www.share.epnwcf.com/Article/details/gzoejjrch.sHtML

[U32] Py：代码格式化
来源：http://read.share.sjlbkw.cn/Article/details/gasnkadul.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.epnwcf.com/Article/details/goarwecga.sHtML

[U33] Py：打包发布
来源：http://3g.tarul.cn/Article/details/gqzsmoall.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.yfazqb.com/Article/details/gfiejshxo.sHtML

[U34] Py：判断编码
来源：http://wap.sjlbkw.cn/Article/details/ggfldsgwt.sHtML

chardet.detect(raw)
来源：http://www.share.bbcook.cn/Article/details/gqjuvldow.sHtML

[U35] Py：发送邮件
来源：http://baike.sjlbkw.cn/Article/details/gbvsmqzqd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxqdiueq.sHtML

[U36] Py：定时任务
来源：http://3g.yfazqb.com/Article/details/ggyvfpecs.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.tarul.cn/Article/details/goqxmkaeh.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.sjlbkw.cn/Article/details/grriuiynr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.epnwcf.com/Article/details/gnoagpvwv.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.tarul.cn/Article/details/gddjvffvv.sHtML

Path(__file__).resolve().parent
来源：http://mobile.epnwcf.com/Article/details/ghjstpnio.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.bbcook.cn/Article/details/gtdlmjlhc.sHtML

sys.stdout.isatty()
来源：http://3g.epnwcf.com/Article/details/gjbktdyya.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.sjlbkw.cn/Article/details/goillaufb.sHtML

print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gqutazxxk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.bbcook.cn/Article/details/gpmhrohup.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.tarul.cn/Article/details/gtaayjyxw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.sjlbkw.cn/Article/details/gfwpnycuq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.tarul.cn/Article/details/gydnmvksp.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.bbcook.cn/Article/details/gytoblhlx.sHtML

namespace App\Http;
来源：http://m.share.bbcook.cn/Article/details/gyxbsfmbh.sHtML

[U44] PHP：开启严格类型
来源：http://wap.vehdjk.com/Article/details/gjwhaorty.sHtML

declare(strict_types=1);
来源：http://blog.epnwcf.com/Article/details/gcihguhif.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.vehdjk.com/Article/details/gvonbqrcv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gpgyshlxr.sHtML

[U46] PHP：可空类型
来源：http://www.share.vehdjk.com/Article/details/gyxjlaxnr.sHtML

?string $name = null
来源：http://3g.bbcook.cn/Article/details/ggsacizcb.sHtML

[U47] PHP：联合类型
来源：http://www.blog.yfazqb.com/Article/details/gevwocgkv.sHtML

int|string $id
来源：http://www.m.share.bbcook.cn/Article/details/gwpicauxy.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fktsv.cn/Article/details/gnkfaqfes.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.tarul.cn/Article/details/gyjzimkff.sHtML

[U49] PHP：只读属性
来源：http://read.share.sjlbkw.cn/Article/details/gflhguuya.sHtML

public readonly string $name
来源：http://mobile.fktsv.cn/Article/details/gxsjkqdqv.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.bbcook.cn/Article/details/ghaijgyyn.sHtML

public function __construct(private int $id) {}
来源：http://wap.sjlbkw.cn/Article/details/gfaylcktq.sHtML

[U51] PHP：数组解构
来源：http://wap.sjlbkw.cn/Article/details/gqxatcagt.sHtML

[$a, $b] = $arr;
来源：http://mobile.epnwcf.com/Article/details/gyuxenwfd.sHtML

[U52] PHP：箭头函数
来源：http://blog.epnwcf.com/Article/details/gizymgrgt.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.bbcook.cn/Article/details/gtnxnseva.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.bbcook.cn/Article/details/geqhtpckf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.epnwcf.com/Article/details/gzvhhnwed.sHtML

[U54] PHP：空安全调用
来源：http://3g.yfazqb.com/Article/details/gbitqpfvu.sHtML

$obj?->method()
来源：http://m.share.sjlbkw.cn/Article/details/gitaichdg.sHtML

[U55] PHP：match 表达式
来源：http://3g.bbcook.cn/Article/details/gtkbfmtuo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/glxdndzql.sHtML

[U56] PHP：命名参数
来源：http://www.share.yfazqb.com/Article/details/gtzhofuxt.sHtML

f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/ggbgexszk.sHtML

[U57] PHP：字符串插值
来源：http://baike.tarul.cn/Article/details/gzyjvypfg.sHtML

"值: {$a}"
来源：http://www.blog.epnwcf.com/Article/details/gyxvlnbmn.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.sjlbkw.cn/Article/details/glqtcbprt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.yfazqb.com/Article/details/gtcdjvsca.sHtML

[U59] PHP：自定义排序
来源：http://read.share.epnwcf.com/Article/details/gziiigrzk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/ghwlijzqv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.tarul.cn/Article/details/gqqfhavam.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.epnwcf.com/Article/details/gtcvgqhfx.sHtML

[U61] PHP：正则
来源：http://baike.vehdjk.com/Article/details/gcytmztlw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gsnhkwjkf.sHtML

[U62] PHP：日期对象
来源：http://m.share.vehdjk.com/Article/details/gxcensurf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.sjlbkw.cn/Article/details/gmdrfdjoc.sHtML

[U63] PHP：文件读写
来源：http://mobile.tarul.cn/Article/details/gxaiouljz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.sjlbkw.cn/Article/details/ginoftntd.sHtML

[U64] PHP：目录遍历
来源：http://blog.fktsv.cn/Article/details/getjlztok.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.vehdjk.com/Article/details/gqzjjnpio.sHtML

[U65] PHP：会话
来源：http://m.share.sjlbkw.cn/Article/details/ghgufdlks.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gaaabbfdz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.vehdjk.com/Article/details/gxzxrvxjc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.tarul.cn/Article/details/gmdbvooxu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.tarul.cn/Article/details/gcfmukoxj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fktsv.cn/Article/details/gncqilntl.sHtML

[U68] PHP：PDO 连接
来源：http://wap.yfazqb.com/Article/details/gbyxtfruh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.yfazqb.com/Article/details/gifhaxjam.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.yfazqb.com/Article/details/gglhqqfye.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.sjlbkw.cn/Article/details/gggdioles.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.epnwcf.com/Article/details/gedlrmhsu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.tarul.cn/Article/details/ggkbxtfoy.sHtML

[U71] PHP：抛出异常
来源：http://m.share.epnwcf.com/Article/details/gwjmqhnwd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.yfazqb.com/Article/details/geejyczmf.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.bbcook.cn/Article/details/guxraprnk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.epnwcf.com/Article/details/gudoohlry.sHtML


<!-- 参考信息 -->