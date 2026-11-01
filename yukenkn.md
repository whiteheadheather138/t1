代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.share.yfazqb.com/Article/details/gfxqfdtya.sHtML

[S49] C++：写文件
来源：http://wap.yfazqb.com/Article/details/gqxfglptg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.yfazqb.com/Article/details/gvzsydelo.sHtML

[S50] C++：格式化数字
来源：http://wap.fktsv.cn/Article/details/gqclewkgu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.tarul.cn/Article/details/ggqdbwgsm.sHtML

[S51] C++：显式类型转换
来源：http://blog.sjlbkw.cn/Article/details/gzljxqxfi.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/gahvyegxd.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/gjkmazjtq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.vehdjk.com/Article/details/gmlwoezjl.sHtML

[S53] C++：移动语义
来源：http://read.share.epnwcf.com/Article/details/gmwxrxtro.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gmaxyfzxd.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fktsv.cn/Article/details/gyyfzzbnf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.tarul.cn/Article/details/gczdarogu.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/gslwytins.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.vehdjk.com/Article/details/gnzlbgawu.sHtML

[S56] C++：optional
来源：http://read.share.sjlbkw.cn/Article/details/gmtgsfkcw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/gyxrrmczk.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/gutwdtepi.sHtML

constexpr int N = 10;
来源：http://3g.fktsv.cn/Article/details/gkeeqvdjt.sHtML

[S58] C++：命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gqdjdzdwp.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.sjlbkw.cn/Article/details/gkvtbewhi.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/gtdoonrnf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrtoysmh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.bbcook.cn/Article/details/gxvfcmmmt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.epnwcf.com/Article/details/gnibjsmag.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghvfzcsca.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/gvnoojnbn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/geoqexzag.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gcrmwjxnt.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gxalcczgv.sHtML

[T02] Kotlin：变量
来源：http://wap.tarul.cn/Article/details/gdofkrtui.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.vehdjk.com/Article/details/gknrbqnsi.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/gwuztezzp.sHtML

"值: $b"
来源：http://read.share.vehdjk.com/Article/details/gkqlfipug.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.bbcook.cn/Article/details/gdlmxritu.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/gzkunvkuv.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/glwubvdtc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fktsv.cn/Article/details/gdwpiflqt.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fktsv.cn/Article/details/gaeglbenv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/gkqdpesht.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.yfazqb.com/Article/details/ghirkktdx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.epnwcf.com/Article/details/grgnpnjim.sHtML

[T08] Kotlin：数据类
来源：http://wap.tarul.cn/Article/details/gnlwvwliq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/gbsuzxykg.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.vehdjk.com/Article/details/gjluxnbiz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.yfazqb.com/Article/details/gykwhtimz.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gdopdrxjt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.yfazqb.com/Article/details/gyeljybar.sHtML

[T11] Kotlin：协程
来源：http://m.share.fktsv.cn/Article/details/ghsxxdkyz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.epnwcf.com/Article/details/gtvlgtqzq.sHtML

[T12] Kotlin：解构声明
来源：http://wap.bbcook.cn/Article/details/gcnmgbjhb.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.vehdjk.com/Article/details/giifgchlf.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.bbcook.cn/Article/details/gczcoarbf.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/gbsturvmq.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/gcbltaamt.sHtML

for (i in 1..10) println(i)
来源：http://3g.vehdjk.com/Article/details/gbhuagwav.sHtML

[T15] Kotlin：接口
来源：http://read.share.bbcook.cn/Article/details/gkzideynp.sHtML

interface Shape { fun area(): Double }
来源：http://baike.yfazqb.com/Article/details/gnozqzkks.sHtML

[T16] Swift：Hello World
来源：http://blog.vehdjk.com/Article/details/gcitxlvqf.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gebanvkdi.sHtML

[T17] Swift：变量与常量
来源：http://blog.vehdjk.com/Article/details/guxmzuszi.sHtML

var a = 1;  let b = 2
来源：http://mobile.vehdjk.com/Article/details/gignpqipj.sHtML

[T18] Swift：字符串插值
来源：http://wap.epnwcf.com/Article/details/grbtryjqo.sHtML

"值: \(b)"
来源：http://www.share.sjlbkw.cn/Article/details/gvroshzie.sHtML

[T19] Swift：可选绑定
来源：http://read.share.vehdjk.com/Article/details/gfpokwyqr.sHtML

if let n = opt { print(n) }
来源：http://mobile.epnwcf.com/Article/details/gvcivvuet.sHtML

[T20] Swift：数组操作
来源：http://mobile.vehdjk.com/Article/details/gvlimgkuu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.vehdjk.com/Article/details/gsvocyijd.sHtML

[T21] Swift：遍历
来源：http://3g.vehdjk.com/Article/details/gpsskwfmi.sHtML

for x in a { print(x) }
来源：http://www.m.share.fktsv.cn/Article/details/ghjwfhynb.sHtML

[T22] Swift：字典
来源：http://www.m.share.vehdjk.com/Article/details/ggodybmxc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.sjlbkw.cn/Article/details/gnzjemwjq.sHtML

[T23] Swift：函数
来源：http://blog.fktsv.cn/Article/details/gwzyjllyq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gcpgbuybp.sHtML

[T24] Swift：闭包
来源：http://www.blog.yfazqb.com/Article/details/gnxkocugq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.bbcook.cn/Article/details/gbgfnuarj.sHtML

[T25] Swift：结构体
来源：http://blog.epnwcf.com/Article/details/guscktfex.sHtML

struct P { var x: Int }
来源：http://read.share.fktsv.cn/Article/details/gwogocqcb.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/galjdelle.sHtML

class A: Base { override func f() {} }
来源：http://blog.epnwcf.com/Article/details/gdihsadhz.sHtML

[T27] Swift：错误处理
来源：http://read.share.fktsv.cn/Article/details/gqhpihkuk.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/glrlblsew.sHtML

[T28] Swift：枚举
来源：http://wap.fktsv.cn/Article/details/gpjlxhltt.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/gaqrzhypz.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.epnwcf.com/Article/details/gvhpyaicx.sHtML

guard let x = opt else { return }
来源：http://www.blog.vehdjk.com/Article/details/gpdrjgfwx.sHtML

[T30] Swift：协议
来源：http://wap.epnwcf.com/Article/details/gjteubwzd.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.vehdjk.com/Article/details/guaigbhel.sHtML

[T31] Lua：Hello World
来源：http://wap.fktsv.cn/Article/details/guxmssvne.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/glgmmdnmh.sHtML

[T32] Lua：局部变量
来源：http://www.share.vehdjk.com/Article/details/gkqnkraxc.sHtML

local a = 1
来源：http://baike.tarul.cn/Article/details/gmqcqahfw.sHtML

[T33] Lua：表（数组）
来源：http://3g.tarul.cn/Article/details/gtjzdxcqr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.epnwcf.com/Article/details/gcukwfadh.sHtML

[T34] Lua：遍历表
来源：http://baike.epnwcf.com/Article/details/gigqazzkd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.epnwcf.com/Article/details/gtbqlbzhr.sHtML

[T35] Lua：字典表
来源：http://m.share.yfazqb.com/Article/details/grkfxxvmm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.tarul.cn/Article/details/gaojynwow.sHtML

[T36] Lua：函数
来源：http://www.m.share.yfazqb.com/Article/details/gsgftjays.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/griyttqwt.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fktsv.cn/Article/details/gnwjoikft.sHtML

"a" .. "b"
来源：http://blog.yfazqb.com/Article/details/gdqmahqvh.sHtML

[T38] Lua：条件
来源：http://www.blog.yfazqb.com/Article/details/gdiuomehs.sHtML

if x > 0 then print("正") end
来源：http://3g.fktsv.cn/Article/details/gjpgkfnfg.sHtML

[T39] Lua：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/gvaeaxjgt.sHtML

string.find(s, "%d+")
来源：http://m.share.fktsv.cn/Article/details/gsmxbmqhz.sHtML

[T40] Lua：元表
来源：http://wap.tarul.cn/Article/details/ghqgfycur.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.yfazqb.com/Article/details/gpeacorcg.sHtML

[T41] Perl：Hello World
来源：http://blog.bbcook.cn/Article/details/ganqjtzlj.sHtML

print "Hello\n";
来源：http://www.m.share.vehdjk.com/Article/details/gnwqqbhjt.sHtML

[T42] Perl：变量类型
来源：http://wap.yfazqb.com/Article/details/gwhtjwzaf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gdnbmgruh.sHtML

[T43] Perl：字符串插值
来源：http://mobile.tarul.cn/Article/details/gimrehfcy.sHtML

"值: $a"
来源：http://wap.yfazqb.com/Article/details/gotmfbwco.sHtML

[T44] Perl：条件
来源：http://m.share.fktsv.cn/Article/details/gudiqiayd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkwpcbwgg.sHtML

[T45] Perl：数组遍历
来源：http://3g.sjlbkw.cn/Article/details/gluzlnssp.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.sjlbkw.cn/Article/details/gmzcfzrbf.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fktsv.cn/Article/details/gebkkkpqu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.yfazqb.com/Article/details/gfzxkbszi.sHtML

[T47] Perl：正则捕获
来源：http://www.share.epnwcf.com/Article/details/goxhkumai.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkqcjghr.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxgzrvmn.sHtML

$s =~ s/old/new/g;
来源：http://mobile.yfazqb.com/Article/details/gfmudlzoj.sHtML

[T49] Perl：函数
来源：http://www.share.epnwcf.com/Article/details/gnoquelmv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gdvaxvpjn.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gnwftjxmm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.sjlbkw.cn/Article/details/gpdcqkqvw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fktsv.cn/Article/details/gngqrmsbo.sHtML

[T51] Scala：Hello World
来源：http://mobile.epnwcf.com/Article/details/gpeqkifyf.sHtML

println("Hello")
来源：http://wap.tarul.cn/Article/details/ghgbmvips.sHtML

[T52] Scala：变量
来源：http://blog.epnwcf.com/Article/details/goiygufbx.sHtML

val a = 1;  var b = 2
来源：http://baike.vehdjk.com/Article/details/gkqcdvdiu.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrniccye.sHtML

s"值: $b"
来源：http://wap.fktsv.cn/Article/details/ggglopyac.sHtML

[T54] Scala：集合映射
来源：http://mobile.tarul.cn/Article/details/gfpawsxma.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.yfazqb.com/Article/details/gacdfgytf.sHtML

[T55] Scala：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gujqmprvt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fktsv.cn/Article/details/gcszavomc.sHtML

[T56] Scala：样例类
来源：http://www.m.share.tarul.cn/Article/details/gpkszebyy.sHtML

case class User(name: String, age: Int)
来源：http://baike.yfazqb.com/Article/details/gnzelvwvf.sHtML

[T57] Scala：模式匹配
来源：http://3g.tarul.cn/Article/details/gfahqpjhi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.epnwcf.com/Article/details/gzqywplqr.sHtML

[T58] Scala：函数定义
来源：http://3g.yfazqb.com/Article/details/ggpbgitrh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.bbcook.cn/Article/details/gliytbzez.sHtML

[T59] Scala：循环
来源：http://m.share.sjlbkw.cn/Article/details/gfblogoiu.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fktsv.cn/Article/details/gvxijsbqm.sHtML

[T60] Scala：折叠
来源：http://www.share.sjlbkw.cn/Article/details/gqbjwhxue.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/gkxbpkali.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtjyytpcf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.tarul.cn/Article/details/ghwahjnkz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gbmrnxlpa.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.yfazqb.com/Article/details/gmvvhbhga.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/gjtpydfml.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.tarul.cn/Article/details/gxarwkvzm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.epnwcf.com/Article/details/ganiumfqr.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.bbcook.cn/Article/details/geqdgtgtm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.yfazqb.com/Article/details/gcdyimwjo.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.epnwcf.com/Article/details/gfqvdupbr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.sjlbkw.cn/Article/details/gpwvpwkwt.sHtML

[U05] Py：列表去重且保序
来源：http://baike.tarul.cn/Article/details/ggtdzzfmv.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fktsv.cn/Article/details/gzwzivmbi.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.tarul.cn/Article/details/gwrtohaom.sHtML

{**a, **b}
来源：http://baike.sjlbkw.cn/Article/details/gmylikdze.sHtML

[U07] Py：反转字典键值
来源：http://blog.sjlbkw.cn/Article/details/ggirheess.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.vehdjk.com/Article/details/goymvuszj.sHtML

[U08] Py：展平二维列表
来源：http://www.share.epnwcf.com/Article/details/giwoehady.sHtML

[y for x in nested for y in x]
来源：http://blog.tarul.cn/Article/details/gwqtzbuvz.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.yfazqb.com/Article/details/glcttiqpc.sHtML

max(d, key=d.get)
来源：http://wap.fktsv.cn/Article/details/griutddvm.sHtML

[U10] Py：按值排序字典
来源：http://read.share.yfazqb.com/Article/details/gzjpktjkv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.tarul.cn/Article/details/gudoshutv.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.epnwcf.com/Article/details/gcxkjivnq.sHtML

(x * 2 for x in arr)
来源：http://www.blog.epnwcf.com/Article/details/gqkyprzsa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.yfazqb.com/Article/details/grfkkpohw.sHtML

Counter(arr).most_common(3)
来源：http://3g.vehdjk.com/Article/details/gtmpmfcxk.sHtML

[U13] Py：固定长度队列
来源：http://baike.yfazqb.com/Article/details/gjfuxdkir.sHtML

deque(maxlen=10)
来源：http://wap.tarul.cn/Article/details/gfrlhjpsr.sHtML

[U14] Py：分组收集到列表
来源：http://baike.epnwcf.com/Article/details/gdlethood.sHtML

defaultdict(list)
来源：http://www.m.share.tarul.cn/Article/details/ggwrqtbdz.sHtML

[U15] Py：高精度计时
来源：http://baike.epnwcf.com/Article/details/gkbtcmabq.sHtML

t = time.perf_counter()
来源：http://www.blog.vehdjk.com/Article/details/guskkkwax.sHtML

[U16] Py：命令行参数解析
来源：http://baike.epnwcf.com/Article/details/gvoajmzxi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.bbcook.cn/Article/details/gjhdpnnkr.sHtML

[U17] Py：初始化日志
来源：http://3g.fktsv.cn/Article/details/gifxnfwqy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fktsv.cn/Article/details/gckuhnexn.sHtML

[U18] Py：预编译正则
来源：http://3g.bbcook.cn/Article/details/gvpxxqugw.sHtML

pat = re.compile(r"\d+")
来源：http://3g.tarul.cn/Article/details/gkrwhfuox.sHtML

[U19] Py：正则替换带回调
来源：http://blog.bbcook.cn/Article/details/glnfmzjut.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fktsv.cn/Article/details/gkxjwkjrn.sHtML

[U20] Py：缓存函数结果
来源：http://3g.vehdjk.com/Article/details/gntnhioaj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.vehdjk.com/Article/details/gofkwlafs.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.yfazqb.com/Article/details/gfnxafhpd.sHtML

@contextlib.contextmanager
来源：http://mobile.sjlbkw.cn/Article/details/gsxnpouil.sHtML

[U22] Py：矩阵转置
来源：http://m.share.bbcook.cn/Article/details/gdxdhprei.sHtML

list(zip(*m))
来源：http://3g.vehdjk.com/Article/details/gkhckwccz.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.bbcook.cn/Article/details/gslyplxam.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.bbcook.cn/Article/details/gwbbvmcld.sHtML

[U24] Py：路径操作
来源：http://mobile.epnwcf.com/Article/details/gclvnhatf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gafdvfbyn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.vehdjk.com/Article/details/gcddifpsk.sHtML

csv.DictReader(f)
来源：http://www.blog.epnwcf.com/Article/details/gboibcncx.sHtML

[U26] Py：并发下载
来源：http://baike.fktsv.cn/Article/details/gdmmtlssq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.vehdjk.com/Article/details/gacqbzobg.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fktsv.cn/Article/details/gfvthhykx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fktsv.cn/Article/details/guhsusnsy.sHtML

[U28] Py：类型别名
来源：http://read.share.yfazqb.com/Article/details/gzvailmrb.sHtML

UserId = int
来源：http://blog.tarul.cn/Article/details/gqedxddla.sHtML

[U29] Py：属性校验
来源：http://baike.tarul.cn/Article/details/gandupuut.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fktsv.cn/Article/details/govqqhzyy.sHtML

[U30] Py：数据类
来源：http://wap.tarul.cn/Article/details/gdclpynll.sHtML

@dataclass(slots=True)
来源：http://read.share.sjlbkw.cn/Article/details/gyydoholw.sHtML

[U31] Py：单测
来源：http://www.share.tarul.cn/Article/details/gfuiwlhcg.sHtML

python -m pytest -q
来源：http://www.m.share.epnwcf.com/Article/details/gkufxqdbh.sHtML

[U32] Py：代码格式化
来源：http://3g.bbcook.cn/Article/details/gxsurqmuq.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fktsv.cn/Article/details/gmcwjphgr.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fktsv.cn/Article/details/gkhdqzasm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fktsv.cn/Article/details/ghyvokyyd.sHtML

[U34] Py：判断编码
来源：http://read.share.sjlbkw.cn/Article/details/ggtwkpkux.sHtML

chardet.detect(raw)
来源：http://blog.fktsv.cn/Article/details/guedfhdpv.sHtML

[U35] Py：发送邮件
来源：http://blog.epnwcf.com/Article/details/gcvlljwtw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fktsv.cn/Article/details/gfsczrwmy.sHtML

[U36] Py：定时任务
来源：http://wap.sjlbkw.cn/Article/details/gkktfnvrd.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.vehdjk.com/Article/details/gibiisfph.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.sjlbkw.cn/Article/details/gdrcqvbjr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fktsv.cn/Article/details/gejnixwut.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.yfazqb.com/Article/details/gibscniba.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.bbcook.cn/Article/details/gxxoxrvon.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.bbcook.cn/Article/details/gyxiimyzr.sHtML

sys.stdout.isatty()
来源：http://read.share.bbcook.cn/Article/details/guygtvgmu.sHtML

[U40] Py：打印到标准错误
来源：http://blog.vehdjk.com/Article/details/gskgrljii.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gbprgxcse.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.yfazqb.com/Article/details/gebcfdvig.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.tarul.cn/Article/details/gdjhroqir.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.tarul.cn/Article/details/gcowvkdpm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.epnwcf.com/Article/details/gwezauyam.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.bbcook.cn/Article/details/gnitxdrat.sHtML

namespace App\Http;
来源：http://m.share.sjlbkw.cn/Article/details/gbcabtiaj.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.tarul.cn/Article/details/gcommkwse.sHtML

declare(strict_types=1);
来源：http://wap.vehdjk.com/Article/details/gcwwqihhx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fktsv.cn/Article/details/gtvchfdfm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gchsvrigj.sHtML

[U46] PHP：可空类型
来源：http://blog.yfazqb.com/Article/details/gmzvmoysh.sHtML

?string $name = null
来源：http://www.blog.vehdjk.com/Article/details/gnlwqsgqx.sHtML

[U47] PHP：联合类型
来源：http://www.blog.vehdjk.com/Article/details/gkzpsqluc.sHtML

int|string $id
来源：http://read.share.fktsv.cn/Article/details/gqhsotiia.sHtML

[U48] PHP：纯枚举
来源：http://baike.sjlbkw.cn/Article/details/gfisdyplf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.sjlbkw.cn/Article/details/ggpxehecz.sHtML

[U49] PHP：只读属性
来源：http://mobile.yfazqb.com/Article/details/gyuffpilt.sHtML

public readonly string $name
来源：http://mobile.epnwcf.com/Article/details/gdgdlsfxf.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.tarul.cn/Article/details/gwoozffsx.sHtML

public function __construct(private int $id) {}
来源：http://3g.tarul.cn/Article/details/gwlccegpi.sHtML

[U51] PHP：数组解构
来源：http://blog.tarul.cn/Article/details/gxhhkynwi.sHtML

[$a, $b] = $arr;
来源：http://www.blog.yfazqb.com/Article/details/givrmpnks.sHtML

[U52] PHP：箭头函数
来源：http://3g.vehdjk.com/Article/details/gwqhqtwwe.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.bbcook.cn/Article/details/goxtppfhg.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.bbcook.cn/Article/details/gwbwpqdui.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.tarul.cn/Article/details/gyxeyjpdk.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fktsv.cn/Article/details/gynsfesmi.sHtML

$obj?->method()
来源：http://read.share.bbcook.cn/Article/details/gjhlvrmbd.sHtML

[U55] PHP：match 表达式
来源：http://www.share.yfazqb.com/Article/details/gscmtctkw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.tarul.cn/Article/details/gkfzkqtvh.sHtML

[U56] PHP：命名参数
来源：http://read.share.vehdjk.com/Article/details/gwvfuieby.sHtML

f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/grupsbydx.sHtML

[U57] PHP：字符串插值
来源：http://baike.fktsv.cn/Article/details/gupctmcwh.sHtML

"值: {$a}"
来源：http://www.m.share.tarul.cn/Article/details/gizjoayrn.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.sjlbkw.cn/Article/details/gduwdhqfo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.sjlbkw.cn/Article/details/ghzckripv.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.epnwcf.com/Article/details/ghoimbvpz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/gdplicayu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fktsv.cn/Article/details/gcgopxzlr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.vehdjk.com/Article/details/glmvssysn.sHtML

[U61] PHP：正则
来源：http://www.blog.sjlbkw.cn/Article/details/gthqhquec.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gacqnljok.sHtML

[U62] PHP：日期对象
来源：http://read.share.yfazqb.com/Article/details/gtnplbyll.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fktsv.cn/Article/details/gyaibgyth.sHtML

[U63] PHP：文件读写
来源：http://wap.vehdjk.com/Article/details/gcymzkxyx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.tarul.cn/Article/details/gqplllbuj.sHtML

[U64] PHP：目录遍历
来源：http://wap.vehdjk.com/Article/details/guybvymwe.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.sjlbkw.cn/Article/details/geugsllpb.sHtML

[U65] PHP：会话
来源：http://www.share.yfazqb.com/Article/details/gkmmesvqv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gunybatcr.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.epnwcf.com/Article/details/guwbrscrx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.bbcook.cn/Article/details/gcywqskcj.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.bbcook.cn/Article/details/gqpgmhztk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.tarul.cn/Article/details/gqnrhbsno.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fktsv.cn/Article/details/gwnernjrt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.epnwcf.com/Article/details/gvffvhzqj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.yfazqb.com/Article/details/gjyozhkwt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fktsv.cn/Article/details/gfreskahz.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.bbcook.cn/Article/details/ghuqprbea.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.epnwcf.com/Article/details/gucgbfttr.sHtML

[U71] PHP：抛出异常
来源：http://m.share.vehdjk.com/Article/details/gtabcvalq.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.bbcook.cn/Article/details/gyhqbkbto.sHtML

[U72] PHP：写错误日志
来源：http://3g.sjlbkw.cn/Article/details/gwteahuoy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxnnxoow.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.tarul.cn/Article/details/guqrlrill.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.sjlbkw.cn/Article/details/gydeirzci.sHtML

[U74] PHP：读取环境变量
来源：http://baike.tarul.cn/Article/details/gqqjzdqqp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.vehdjk.com/Article/details/gozjqwntg.sHtML


<!-- 参考信息 -->