代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.blog.vehdjk.com/Article/details/gxwmskape.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.tarul.cn/Article/details/gjtzvhldh.sHtML

[S48] C++：逐行读文件
来源：http://blog.vehdjk.com/Article/details/ghoktwezm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fktsv.cn/Article/details/ghtyxmzph.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.bbcook.cn/Article/details/ggjcmoark.sHtML

[S49] C++：写文件
来源：http://blog.yfazqb.com/Article/details/gcgfiywfm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.yfazqb.com/Article/details/goygelzfm.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/ggzyqavgi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gnuupekjf.sHtML

[S51] C++：显式类型转换
来源：http://m.share.bbcook.cn/Article/details/gxwwrjkeo.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/ghkpigqgi.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.sjlbkw.cn/Article/details/gbsuoxjao.sHtML

int size() const noexcept { return n_; }
来源：http://wap.tarul.cn/Article/details/gfhmbemqd.sHtML

[S53] C++：移动语义
来源：http://www.blog.bbcook.cn/Article/details/gnifwaays.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpartypcp.sHtML

[S54] C++：异常处理
来源：http://wap.yfazqb.com/Article/details/gbubycdfk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.bbcook.cn/Article/details/gndzavrrt.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/glaieipaw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.vehdjk.com/Article/details/goqkranaz.sHtML

[S56] C++：optional
来源：http://3g.epnwcf.com/Article/details/gqwpdmnmx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.bbcook.cn/Article/details/gduvmnbkw.sHtML

[S57] C++：编译期常量
来源：http://www.share.fktsv.cn/Article/details/gsjmkdtjk.sHtML

constexpr int N = 10;
来源：http://m.share.bbcook.cn/Article/details/gyvtedfid.sHtML

[S58] C++：命名空间
来源：http://mobile.tarul.cn/Article/details/gvzhqudbh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.vehdjk.com/Article/details/gflyoshvm.sHtML

[S59] C++：静态断言
来源：http://m.share.bbcook.cn/Article/details/gngccmgcp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.bbcook.cn/Article/details/ggceoohcb.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.bbcook.cn/Article/details/gjadltjdv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.tarul.cn/Article/details/guoboqkmf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/guzawjnrt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gsuxdcuyk.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gokguerso.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gaidgfgxt.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gkuvomlyq.sHtML

[T02] Kotlin：变量
来源：http://read.share.epnwcf.com/Article/details/gnijbbiva.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.yfazqb.com/Article/details/gusuekwip.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.vehdjk.com/Article/details/geyyxbgob.sHtML

"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gtpmaoray.sHtML

[T04] Kotlin：空安全
来源：http://3g.vehdjk.com/Article/details/gjlpgmoto.sHtML

val n: String? = null;  n?.length
来源：http://m.share.tarul.cn/Article/details/gvsdbuixh.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.bbcook.cn/Article/details/gulucatcf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/gxlvsfnxl.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/ghrelxlol.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.epnwcf.com/Article/details/geefowuyq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.tarul.cn/Article/details/grnmwacvt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fktsv.cn/Article/details/gyjjtjdvi.sHtML

[T08] Kotlin：数据类
来源：http://m.share.yfazqb.com/Article/details/giosqygax.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.epnwcf.com/Article/details/gabdgkkaj.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.bbcook.cn/Article/details/gonmkezgb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/gnjmtjvlo.sHtML

[T10] Kotlin：默认参数
来源：http://baike.bbcook.cn/Article/details/gngkufpcs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.epnwcf.com/Article/details/gnxjkqjlz.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gvqjqthrl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.tarul.cn/Article/details/gjwccawqd.sHtML

[T12] Kotlin：解构声明
来源：http://wap.bbcook.cn/Article/details/gmacgynsr.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/gckodween.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.epnwcf.com/Article/details/gyswhbtye.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gavwduyip.sHtML

[T14] Kotlin：循环
来源：http://3g.tarul.cn/Article/details/gzrcfotnl.sHtML

for (i in 1..10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gyellkdyn.sHtML

[T15] Kotlin：接口
来源：http://3g.epnwcf.com/Article/details/gmhsmofaz.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.yfazqb.com/Article/details/gcvegpwsm.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gijenydkq.sHtML

print("Hello")
来源：http://blog.epnwcf.com/Article/details/gpxavpden.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fktsv.cn/Article/details/gxrfvntxb.sHtML

var a = 1;  let b = 2
来源：http://m.share.yfazqb.com/Article/details/gxmbxrueq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gmgrtqawy.sHtML

"值: \(b)"
来源：http://baike.vehdjk.com/Article/details/gafizzrty.sHtML

[T19] Swift：可选绑定
来源：http://baike.fktsv.cn/Article/details/gduyjqowy.sHtML

if let n = opt { print(n) }
来源：http://mobile.epnwcf.com/Article/details/gonbkthmc.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/gkbltyqpo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.epnwcf.com/Article/details/gpwxxvrif.sHtML

[T21] Swift：遍历
来源：http://read.share.tarul.cn/Article/details/gcotouned.sHtML

for x in a { print(x) }
来源：http://www.share.vehdjk.com/Article/details/gzewpgync.sHtML

[T22] Swift：字典
来源：http://www.blog.epnwcf.com/Article/details/gxtwzhvkd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.epnwcf.com/Article/details/ghfxjegve.sHtML

[T23] Swift：函数
来源：http://blog.bbcook.cn/Article/details/glebqwjls.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.epnwcf.com/Article/details/gflllhqlm.sHtML

[T24] Swift：闭包
来源：http://www.blog.epnwcf.com/Article/details/gsgbmqdao.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.vehdjk.com/Article/details/gyhxhhvju.sHtML

[T25] Swift：结构体
来源：http://baike.vehdjk.com/Article/details/gxxtrpibj.sHtML

struct P { var x: Int }
来源：http://www.blog.sjlbkw.cn/Article/details/gokxbmhcw.sHtML

[T26] Swift：类与重写
来源：http://mobile.sjlbkw.cn/Article/details/ginxhrcjq.sHtML

class A: Base { override func f() {} }
来源：http://read.share.sjlbkw.cn/Article/details/gxkkvdwmh.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/grnddqtqq.sHtML

do { try f() } catch { print(error) }
来源：http://baike.epnwcf.com/Article/details/guwduzadm.sHtML

[T28] Swift：枚举
来源：http://wap.bbcook.cn/Article/details/gmkqwtafp.sHtML

enum Color { case red, green }
来源：http://www.blog.epnwcf.com/Article/details/gwmnbggoo.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.bbcook.cn/Article/details/ginbxkyyh.sHtML

guard let x = opt else { return }
来源：http://www.blog.tarul.cn/Article/details/gegewxgkv.sHtML

[T30] Swift：协议
来源：http://read.share.vehdjk.com/Article/details/gfebqauki.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.vehdjk.com/Article/details/gsygsypnh.sHtML

[T31] Lua：Hello World
来源：http://read.share.tarul.cn/Article/details/gvgbaqicz.sHtML

print("Hello")
来源：http://www.blog.tarul.cn/Article/details/giwaqdhii.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.bbcook.cn/Article/details/gpssmnktb.sHtML

local a = 1
来源：http://baike.fktsv.cn/Article/details/gkujddxvb.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.vehdjk.com/Article/details/gaootpygy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.sjlbkw.cn/Article/details/gvjkjmqsr.sHtML

[T34] Lua：遍历表
来源：http://read.share.sjlbkw.cn/Article/details/gimzzjijq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.epnwcf.com/Article/details/gvreiixkr.sHtML

[T35] Lua：字典表
来源：http://wap.yfazqb.com/Article/details/gfhymtxeu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.tarul.cn/Article/details/gvdtzarzs.sHtML

[T36] Lua：函数
来源：http://m.share.bbcook.cn/Article/details/gfugdkiqq.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/gdtxloyvz.sHtML

[T37] Lua：字符串拼接
来源：http://wap.vehdjk.com/Article/details/gtlwpeibv.sHtML

"a" .. "b"
来源：http://www.blog.epnwcf.com/Article/details/gmnjgogiw.sHtML

[T38] Lua：条件
来源：http://wap.sjlbkw.cn/Article/details/gvsvdmrid.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/gubmgarxt.sHtML

[T39] Lua：模式匹配
来源：http://3g.tarul.cn/Article/details/gtkfhqxcf.sHtML

string.find(s, "%d+")
来源：http://baike.sjlbkw.cn/Article/details/gxhbvtzsu.sHtML

[T40] Lua：元表
来源：http://m.share.vehdjk.com/Article/details/gzjlaiqbh.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.yfazqb.com/Article/details/gswxewvjh.sHtML

[T41] Perl：Hello World
来源：http://3g.yfazqb.com/Article/details/gltywiecn.sHtML

print "Hello\n";
来源：http://wap.fktsv.cn/Article/details/gbtfwyqyo.sHtML

[T42] Perl：变量类型
来源：http://wap.sjlbkw.cn/Article/details/geiweuzoh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.tarul.cn/Article/details/gutjgekyp.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gzcdrrxgk.sHtML

"值: $a"
来源：http://www.blog.yfazqb.com/Article/details/gukvyurmg.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/glxagrhat.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/giyxaukwu.sHtML

[T45] Perl：数组遍历
来源：http://mobile.yfazqb.com/Article/details/gnwbcyhvb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.epnwcf.com/Article/details/gfzqfrpcr.sHtML

[T46] Perl：哈希操作
来源：http://www.share.tarul.cn/Article/details/gzndsvbmm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.tarul.cn/Article/details/gocpzgcxu.sHtML

[T47] Perl：正则捕获
来源：http://wap.epnwcf.com/Article/details/geghrcxvz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.yfazqb.com/Article/details/getxcrrci.sHtML

[T48] Perl：正则替换
来源：http://blog.epnwcf.com/Article/details/gixnagauy.sHtML

$s =~ s/old/new/g;
来源：http://www.share.yfazqb.com/Article/details/gqxnmcxhh.sHtML

[T49] Perl：函数
来源：http://baike.sjlbkw.cn/Article/details/gabhmjnms.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gmponmpnt.sHtML

[T50] Perl：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gctivkooy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.epnwcf.com/Article/details/gcsgxboos.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.vehdjk.com/Article/details/gdgiasski.sHtML

[T51] Scala：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gxihibeeo.sHtML

println("Hello")
来源：http://blog.bbcook.cn/Article/details/gkrgzcnpw.sHtML

[T52] Scala：变量
来源：http://baike.epnwcf.com/Article/details/guolefenx.sHtML

val a = 1;  var b = 2
来源：http://wap.sjlbkw.cn/Article/details/ghizwzcsx.sHtML

[T53] Scala：字符串插值
来源：http://m.share.bbcook.cn/Article/details/ggrjvyptw.sHtML

s"值: $b"
来源：http://mobile.yfazqb.com/Article/details/gcowsagoh.sHtML

[T54] Scala：集合映射
来源：http://wap.bbcook.cn/Article/details/gslzhueqq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.epnwcf.com/Article/details/gwkjniwpg.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/gcvepxttv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.sjlbkw.cn/Article/details/ggpvnunrl.sHtML

[T56] Scala：样例类
来源：http://read.share.tarul.cn/Article/details/ggtwnkdve.sHtML

case class User(name: String, age: Int)
来源：http://www.share.vehdjk.com/Article/details/gokkwumji.sHtML

[T57] Scala：模式匹配
来源：http://3g.bbcook.cn/Article/details/gjlhlefif.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.tarul.cn/Article/details/gwtaieycg.sHtML

[T58] Scala：函数定义
来源：http://baike.epnwcf.com/Article/details/gqskqfmrk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.yfazqb.com/Article/details/gwgfoxlku.sHtML

[T59] Scala：循环
来源：http://baike.yfazqb.com/Article/details/gezftcetl.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/grhvzqtvr.sHtML

[T60] Scala：折叠
来源：http://wap.bbcook.cn/Article/details/gltbuelbl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.yfazqb.com/Article/details/gkvfxrorm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gelreozfa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.tarul.cn/Article/details/ghmyslvxw.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbmpvrhrz.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fktsv.cn/Article/details/gdmwosvkt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.yfazqb.com/Article/details/ggnionjtg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.epnwcf.com/Article/details/gstcswvos.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fktsv.cn/Article/details/gvbxnpnbs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fktsv.cn/Article/details/goagqirdh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.vehdjk.com/Article/details/gxrensxsg.sHtML

[U04] Py：变量调试打印
来源：http://3g.tarul.cn/Article/details/gpvjzcmqm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.sjlbkw.cn/Article/details/gpbbkfybq.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.tarul.cn/Article/details/gywtyjdzk.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/gbkxunegy.sHtML

[U06] Py：合并两个字典
来源：http://blog.tarul.cn/Article/details/gmmeestbh.sHtML

{**a, **b}
来源：http://blog.tarul.cn/Article/details/gjkiwlgde.sHtML

[U07] Py：反转字典键值
来源：http://3g.fktsv.cn/Article/details/gffhbtedc.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.tarul.cn/Article/details/gtouumugs.sHtML

[U08] Py：展平二维列表
来源：http://read.share.epnwcf.com/Article/details/gwasgsjnn.sHtML

[y for x in nested for y in x]
来源：http://mobile.tarul.cn/Article/details/gmpujpyvd.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.yfazqb.com/Article/details/gsyzdkwsn.sHtML

max(d, key=d.get)
来源：http://read.share.yfazqb.com/Article/details/gowezclgd.sHtML

[U10] Py：按值排序字典
来源：http://www.share.tarul.cn/Article/details/gzqyzywyg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.sjlbkw.cn/Article/details/guvdpkxpg.sHtML

[U11] Py：生成器表达式
来源：http://3g.sjlbkw.cn/Article/details/gvzqzcyez.sHtML

(x * 2 for x in arr)
来源：http://3g.vehdjk.com/Article/details/gjpxjvxze.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.vehdjk.com/Article/details/girhfrmxg.sHtML

Counter(arr).most_common(3)
来源：http://baike.vehdjk.com/Article/details/gzoafrpwk.sHtML

[U13] Py：固定长度队列
来源：http://www.share.tarul.cn/Article/details/gsbkgktdj.sHtML

deque(maxlen=10)
来源：http://m.share.bbcook.cn/Article/details/gbyinyxkx.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.sjlbkw.cn/Article/details/gezjpybzv.sHtML

defaultdict(list)
来源：http://m.share.fktsv.cn/Article/details/gambhwwrk.sHtML

[U15] Py：高精度计时
来源：http://m.share.bbcook.cn/Article/details/gdqktmius.sHtML

t = time.perf_counter()
来源：http://baike.bbcook.cn/Article/details/grksegtqv.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.tarul.cn/Article/details/goyjndlpn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.bbcook.cn/Article/details/gfhfoawoo.sHtML

[U17] Py：初始化日志
来源：http://www.share.tarul.cn/Article/details/gthzmmwol.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.sjlbkw.cn/Article/details/gkeqhbhhf.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.bbcook.cn/Article/details/ghxprzeac.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.epnwcf.com/Article/details/gfiuhiiih.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.bbcook.cn/Article/details/gumsepmho.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.yfazqb.com/Article/details/gqncsskrn.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.bbcook.cn/Article/details/gkfjhiewx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.yfazqb.com/Article/details/gqhmzueci.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.bbcook.cn/Article/details/gtaebdejv.sHtML

@contextlib.contextmanager
来源：http://3g.yfazqb.com/Article/details/goaraalbu.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.epnwcf.com/Article/details/goxeakafq.sHtML

list(zip(*m))
来源：http://mobile.bbcook.cn/Article/details/gnxlfojzd.sHtML

[U23] Py：分块读取大文件
来源：http://blog.bbcook.cn/Article/details/gleqrojdf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.epnwcf.com/Article/details/geycclvvk.sHtML

[U24] Py：路径操作
来源：http://m.share.fktsv.cn/Article/details/gacwlgiie.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gkxpxujqp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.tarul.cn/Article/details/guitvlzri.sHtML

csv.DictReader(f)
来源：http://www.blog.tarul.cn/Article/details/gotzwrors.sHtML

[U26] Py：并发下载
来源：http://m.share.tarul.cn/Article/details/ghgcmvxyx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fktsv.cn/Article/details/gfwdfwwis.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.vehdjk.com/Article/details/gzbdztefh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.epnwcf.com/Article/details/gtytpgfes.sHtML

[U28] Py：类型别名
来源：http://m.share.sjlbkw.cn/Article/details/gxlwdiqvc.sHtML

UserId = int
来源：http://blog.tarul.cn/Article/details/gaavuuavd.sHtML

[U29] Py：属性校验
来源：http://www.share.vehdjk.com/Article/details/gjbfxfakm.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.bbcook.cn/Article/details/gbpjgstsb.sHtML

[U30] Py：数据类
来源：http://www.blog.bbcook.cn/Article/details/gynvjycpo.sHtML

@dataclass(slots=True)
来源：http://www.share.epnwcf.com/Article/details/grzsvdjbp.sHtML

[U31] Py：单测
来源：http://blog.vehdjk.com/Article/details/gymwdvjiu.sHtML

python -m pytest -q
来源：http://www.blog.sjlbkw.cn/Article/details/ggqroyfow.sHtML

[U32] Py：代码格式化
来源：http://www.blog.yfazqb.com/Article/details/gklbppdmd.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.bbcook.cn/Article/details/gvgrrbtmn.sHtML

[U33] Py：打包发布
来源：http://wap.epnwcf.com/Article/details/gchkskdwv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.vehdjk.com/Article/details/goykovuyb.sHtML

[U34] Py：判断编码
来源：http://www.share.tarul.cn/Article/details/gcrnpthyg.sHtML

chardet.detect(raw)
来源：http://www.m.share.epnwcf.com/Article/details/gdqieveie.sHtML

[U35] Py：发送邮件
来源：http://blog.tarul.cn/Article/details/gcctypsnb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.vehdjk.com/Article/details/gonjlglqu.sHtML

[U36] Py：定时任务
来源：http://m.share.tarul.cn/Article/details/gbkijxsdj.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.sjlbkw.cn/Article/details/gsjguvxex.sHtML

[U37] Py：读写 Excel
来源：http://mobile.vehdjk.com/Article/details/giftspflw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.tarul.cn/Article/details/gihqoctnu.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fktsv.cn/Article/details/ggcbonvhs.sHtML

Path(__file__).resolve().parent
来源：http://baike.tarul.cn/Article/details/giesyjouq.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fktsv.cn/Article/details/gmdubnueh.sHtML

sys.stdout.isatty()
来源：http://baike.epnwcf.com/Article/details/gndhulpbr.sHtML

[U40] Py：打印到标准错误
来源：http://3g.vehdjk.com/Article/details/gfwjkmyga.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/gmtdtwaxb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.vehdjk.com/Article/details/gaggsukkk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.vehdjk.com/Article/details/gkfghecer.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.tarul.cn/Article/details/gqmotnmad.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.vehdjk.com/Article/details/ginlluufy.sHtML

[U43] PHP：声明命名空间
来源：http://blog.yfazqb.com/Article/details/gxmqvisrf.sHtML

namespace App\Http;
来源：http://mobile.fktsv.cn/Article/details/goseaxrrv.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.tarul.cn/Article/details/gajfotukm.sHtML

declare(strict_types=1);
来源：http://baike.tarul.cn/Article/details/gyhbersfs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.sjlbkw.cn/Article/details/guglliead.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gdlhdxrbz.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fktsv.cn/Article/details/gozedvxwh.sHtML

?string $name = null
来源：http://blog.epnwcf.com/Article/details/gkskfmsvw.sHtML

[U47] PHP：联合类型
来源：http://baike.epnwcf.com/Article/details/gztorleex.sHtML

int|string $id
来源：http://www.blog.epnwcf.com/Article/details/gzacyxveu.sHtML

[U48] PHP：纯枚举
来源：http://3g.fktsv.cn/Article/details/geqwllpqh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.vehdjk.com/Article/details/gtlwzzgrx.sHtML

[U49] PHP：只读属性
来源：http://www.blog.vehdjk.com/Article/details/grgyaouqx.sHtML

public readonly string $name
来源：http://www.share.sjlbkw.cn/Article/details/gfhzqedal.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.sjlbkw.cn/Article/details/gvrwrsnzk.sHtML

public function __construct(private int $id) {}
来源：http://m.share.epnwcf.com/Article/details/gwlamtcuj.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.epnwcf.com/Article/details/gccpxwyfu.sHtML

[$a, $b] = $arr;
来源：http://mobile.fktsv.cn/Article/details/gpvmzklje.sHtML

[U52] PHP：箭头函数
来源：http://wap.fktsv.cn/Article/details/gggzppwdh.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.bbcook.cn/Article/details/glkqkvcqn.sHtML

[U53] PHP：空合并运算符
来源：http://baike.sjlbkw.cn/Article/details/gtjgyioop.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fktsv.cn/Article/details/gstjnfxve.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.vehdjk.com/Article/details/ghmzmxvyt.sHtML

$obj?->method()
来源：http://blog.epnwcf.com/Article/details/ggnjiewti.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.vehdjk.com/Article/details/ghdlscxhg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/gtgngrjsc.sHtML

[U56] PHP：命名参数
来源：http://3g.sjlbkw.cn/Article/details/gbrpocedy.sHtML

f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gqnetrrsc.sHtML

[U57] PHP：字符串插值
来源：http://blog.vehdjk.com/Article/details/gsjzdzzvj.sHtML

"值: {$a}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxyfsiel.sHtML

[U58] PHP：数组三件套
来源：http://blog.yfazqb.com/Article/details/ggykrbido.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.epnwcf.com/Article/details/gbeebnbyv.sHtML

[U59] PHP：自定义排序
来源：http://mobile.vehdjk.com/Article/details/gvraxncyx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.bbcook.cn/Article/details/ghqwhsjpd.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.epnwcf.com/Article/details/giijrcjpj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fktsv.cn/Article/details/gfkesdbvu.sHtML

[U61] PHP：正则
来源：http://wap.fktsv.cn/Article/details/gfucxlggi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaktcnhhn.sHtML

[U62] PHP：日期对象
来源：http://mobile.fktsv.cn/Article/details/gscjqaqwh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.vehdjk.com/Article/details/gqlhxdtml.sHtML

[U63] PHP：文件读写
来源：http://blog.vehdjk.com/Article/details/gmskvazob.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.vehdjk.com/Article/details/gejwpvjtl.sHtML

[U64] PHP：目录遍历
来源：http://m.share.bbcook.cn/Article/details/gxjysgdfe.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.yfazqb.com/Article/details/gzcrkaxhm.sHtML

[U65] PHP：会话
来源：http://3g.vehdjk.com/Article/details/gphtdtaoz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gnwjvxhra.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.epnwcf.com/Article/details/gtbcasqmh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.bbcook.cn/Article/details/gldwtmkwu.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.vehdjk.com/Article/details/gcieixyfs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fktsv.cn/Article/details/goqcqlgda.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.bbcook.cn/Article/details/ganlweqrp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.epnwcf.com/Article/details/gygzmoypu.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fktsv.cn/Article/details/gwwyieimx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.tarul.cn/Article/details/gcttppcnv.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fktsv.cn/Article/details/gvbjlweyr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.vehdjk.com/Article/details/golrocnak.sHtML

[U71] PHP：抛出异常
来源：http://3g.tarul.cn/Article/details/guicotxjo.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.vehdjk.com/Article/details/guynlvuoq.sHtML

[U72] PHP：写错误日志
来源：http://blog.tarul.cn/Article/details/gbwwuutdc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.bbcook.cn/Article/details/gkzpcgnpr.sHtML


<!-- 参考信息 -->