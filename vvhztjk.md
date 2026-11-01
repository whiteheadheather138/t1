代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gpoxfvkxk.sHtML

[S51] C++：显式类型转换
来源：http://m.share.vehdjk.com/Article/details/gwaoetrvs.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/gimynbjoh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gwvgxquwi.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.yfazqb.com/Article/details/gvsncugmz.sHtML

[S53] C++：移动语义
来源：http://baike.vehdjk.com/Article/details/gmddfdqhn.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/gvnyfslwr.sHtML

[S54] C++：异常处理
来源：http://m.share.sjlbkw.cn/Article/details/gwhkmhdcr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.vehdjk.com/Article/details/gwixsghxe.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.epnwcf.com/Article/details/ggbnhrygr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/gotivufob.sHtML

[S56] C++：optional
来源：http://wap.sjlbkw.cn/Article/details/gspmshdzy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/grcaipguq.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.yfazqb.com/Article/details/garifvjib.sHtML

constexpr int N = 10;
来源：http://wap.epnwcf.com/Article/details/glbgbmivh.sHtML

[S58] C++：命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gkpzocfjs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.tarul.cn/Article/details/gaiklysno.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/glfhxzmcz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/golauycxy.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.vehdjk.com/Article/details/ggriryrxa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.epnwcf.com/Article/details/gpgngvbgc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/givwufygh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gdsezztqp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqcooiiii.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.yfazqb.com/Article/details/gezsypagz.sHtML

println("Hello")
来源：http://wap.tarul.cn/Article/details/gpfqxuewd.sHtML

[T02] Kotlin：变量
来源：http://m.share.bbcook.cn/Article/details/gbvdcntft.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.yfazqb.com/Article/details/gnifasglp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.bbcook.cn/Article/details/gtmnvluif.sHtML

"值: $b"
来源：http://mobile.tarul.cn/Article/details/gknxvfolh.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/gveqpounw.sHtML

val n: String? = null;  n?.length
来源：http://www.share.yfazqb.com/Article/details/giudximfy.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.yfazqb.com/Article/details/guvdhzcff.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fktsv.cn/Article/details/gmepxeqxh.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.vehdjk.com/Article/details/gqjqucazb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gxmgcmcut.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/gyatexcva.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.epnwcf.com/Article/details/gdklzpgqi.sHtML

[T08] Kotlin：数据类
来源：http://wap.yfazqb.com/Article/details/gkynzkxlp.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.tarul.cn/Article/details/gquwswlqy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.vehdjk.com/Article/details/gzdetxtwa.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.tarul.cn/Article/details/gewybjhbn.sHtML

[T10] Kotlin：默认参数
来源：http://wap.bbcook.cn/Article/details/geutkwuwr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.vehdjk.com/Article/details/gdmadetxw.sHtML

[T11] Kotlin：协程
来源：http://blog.yfazqb.com/Article/details/gyfenfgyg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/grsdroaeg.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fktsv.cn/Article/details/gjoqdmlmv.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.tarul.cn/Article/details/gfqpghlaj.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/gzrsmbtte.sHtML

val m = mapOf("a" to 1)
来源：http://wap.vehdjk.com/Article/details/glqeauseb.sHtML

[T14] Kotlin：循环
来源：http://3g.yfazqb.com/Article/details/gdptcfvoe.sHtML

for (i in 1..10) println(i)
来源：http://blog.epnwcf.com/Article/details/gerfrpyck.sHtML

[T15] Kotlin：接口
来源：http://3g.tarul.cn/Article/details/guaijxera.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.epnwcf.com/Article/details/gqjdkpswz.sHtML

[T16] Swift：Hello World
来源：http://3g.epnwcf.com/Article/details/ghieqvkwo.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gcspvraus.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fktsv.cn/Article/details/ggjpmdcxd.sHtML

var a = 1;  let b = 2
来源：http://m.share.yfazqb.com/Article/details/gbnuijkiw.sHtML

[T18] Swift：字符串插值
来源：http://3g.fktsv.cn/Article/details/gilqdlrcb.sHtML

"值: \(b)"
来源：http://m.share.bbcook.cn/Article/details/gsfpfdzah.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnulhqwn.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/gylfsjqyp.sHtML

[T20] Swift：数组操作
来源：http://mobile.tarul.cn/Article/details/gdkwyraex.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.bbcook.cn/Article/details/gcpkxbbkf.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/gkrxopmzi.sHtML

for x in a { print(x) }
来源：http://baike.tarul.cn/Article/details/gfrqbdiyq.sHtML

[T22] Swift：字典
来源：http://m.share.fktsv.cn/Article/details/gufhkggil.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.tarul.cn/Article/details/glhitdonl.sHtML

[T23] Swift：函数
来源：http://read.share.fktsv.cn/Article/details/gdiadtoxk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.bbcook.cn/Article/details/ggqdpckjt.sHtML

[T24] Swift：闭包
来源：http://read.share.tarul.cn/Article/details/ghbcbqoqr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/gyagcqkld.sHtML

[T25] Swift：结构体
来源：http://baike.bbcook.cn/Article/details/guznognkj.sHtML

struct P { var x: Int }
来源：http://read.share.tarul.cn/Article/details/gzzrfvvsk.sHtML

[T26] Swift：类与重写
来源：http://m.share.sjlbkw.cn/Article/details/gxggovnxs.sHtML

class A: Base { override func f() {} }
来源：http://blog.fktsv.cn/Article/details/grdhumqga.sHtML

[T27] Swift：错误处理
来源：http://www.blog.bbcook.cn/Article/details/gbkrvckcz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.yfazqb.com/Article/details/gaedbtfma.sHtML

[T28] Swift：枚举
来源：http://m.share.yfazqb.com/Article/details/gstfelhcf.sHtML

enum Color { case red, green }
来源：http://www.blog.fktsv.cn/Article/details/gxvawanpp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gobrydbjt.sHtML

guard let x = opt else { return }
来源：http://www.m.share.tarul.cn/Article/details/gpwmjbkgt.sHtML

[T30] Swift：协议
来源：http://m.share.bbcook.cn/Article/details/gypfdwhvt.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.yfazqb.com/Article/details/gbtchqlsj.sHtML

[T31] Lua：Hello World
来源：http://wap.bbcook.cn/Article/details/gjpkymyqg.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/glxlsxfri.sHtML

[T32] Lua：局部变量
来源：http://blog.epnwcf.com/Article/details/gmgwxcjby.sHtML

local a = 1
来源：http://baike.sjlbkw.cn/Article/details/gqtowsttz.sHtML

[T33] Lua：表（数组）
来源：http://blog.vehdjk.com/Article/details/gwsnpdfsh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.vehdjk.com/Article/details/gpoufjodk.sHtML

[T34] Lua：遍历表
来源：http://www.share.bbcook.cn/Article/details/gjphmyfje.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.epnwcf.com/Article/details/grivkxvdl.sHtML

[T35] Lua：字典表
来源：http://wap.vehdjk.com/Article/details/gngcsqgqi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fktsv.cn/Article/details/gsxzvkssl.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/gjjkvzruf.sHtML

function add(a, b) return a + b end
来源：http://blog.sjlbkw.cn/Article/details/gjsgfhffp.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/gehxpvfuf.sHtML

"a" .. "b"
来源：http://mobile.yfazqb.com/Article/details/gkqfbzikv.sHtML

[T38] Lua：条件
来源：http://www.m.share.bbcook.cn/Article/details/glgcgxisz.sHtML

if x > 0 then print("正") end
来源：http://m.share.bbcook.cn/Article/details/gmcbdmbrs.sHtML

[T39] Lua：模式匹配
来源：http://mobile.tarul.cn/Article/details/gnumbxmdi.sHtML

string.find(s, "%d+")
来源：http://wap.yfazqb.com/Article/details/gsnxamept.sHtML

[T40] Lua：元表
来源：http://www.m.share.fktsv.cn/Article/details/gtycnvcuq.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fktsv.cn/Article/details/gcaxoigtn.sHtML

[T41] Perl：Hello World
来源：http://3g.epnwcf.com/Article/details/gadngpwxv.sHtML

print "Hello\n";
来源：http://www.share.sjlbkw.cn/Article/details/gkrpeotwl.sHtML

[T42] Perl：变量类型
来源：http://blog.sjlbkw.cn/Article/details/gpumnzcnh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.vehdjk.com/Article/details/ghfswwkee.sHtML

[T43] Perl：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gapshvjpt.sHtML

"值: $a"
来源：http://www.blog.bbcook.cn/Article/details/glbztijet.sHtML

[T44] Perl：条件
来源：http://www.m.share.bbcook.cn/Article/details/gyqeyattr.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fktsv.cn/Article/details/gcsebiapr.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.bbcook.cn/Article/details/gaaxkhoqm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.yfazqb.com/Article/details/gyakioawx.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.sjlbkw.cn/Article/details/gjvjbdrkm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.sjlbkw.cn/Article/details/gawznaluq.sHtML

[T47] Perl：正则捕获
来源：http://3g.sjlbkw.cn/Article/details/gdwkqfpqj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fktsv.cn/Article/details/gvweixwwh.sHtML

[T48] Perl：正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gacdwabhs.sHtML

$s =~ s/old/new/g;
来源：http://mobile.sjlbkw.cn/Article/details/gzzeawgqo.sHtML

[T49] Perl：函数
来源：http://wap.fktsv.cn/Article/details/gflutdtmu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gsvkzjazp.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gaabenuzp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.bbcook.cn/Article/details/gulsvvxrc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.sjlbkw.cn/Article/details/geeguneet.sHtML

[T51] Scala：Hello World
来源：http://m.share.bbcook.cn/Article/details/gobtvnuly.sHtML

println("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gjvqmxulm.sHtML

[T52] Scala：变量
来源：http://www.m.share.fktsv.cn/Article/details/gngpfehlc.sHtML

val a = 1;  var b = 2
来源：http://mobile.fktsv.cn/Article/details/gjzucorsv.sHtML

[T53] Scala：字符串插值
来源：http://m.share.tarul.cn/Article/details/ghhmiedyd.sHtML

s"值: $b"
来源：http://3g.bbcook.cn/Article/details/gvughkuoq.sHtML

[T54] Scala：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gxgjzdvbz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.yfazqb.com/Article/details/gpgxbpesr.sHtML

[T55] Scala：集合过滤
来源：http://mobile.yfazqb.com/Article/details/glqjqkqyz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.bbcook.cn/Article/details/glfrasjtb.sHtML

[T56] Scala：样例类
来源：http://www.m.share.epnwcf.com/Article/details/gjugdlqid.sHtML

case class User(name: String, age: Int)
来源：http://mobile.vehdjk.com/Article/details/gcybrghhe.sHtML

[T57] Scala：模式匹配
来源：http://www.share.bbcook.cn/Article/details/gnvvjlehp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fktsv.cn/Article/details/gwbtyhkgc.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.epnwcf.com/Article/details/gbzvtbvrz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.sjlbkw.cn/Article/details/gfhalsate.sHtML

[T59] Scala：循环
来源：http://www.share.tarul.cn/Article/details/gtqaqbmwb.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gvqqhlaln.sHtML

[T60] Scala：折叠
来源：http://3g.sjlbkw.cn/Article/details/gstqkmxct.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.epnwcf.com/Article/details/gviyulnzf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glcqxgtjw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.bbcook.cn/Article/details/gpobtwrtz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gcdtzzlhu.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.sjlbkw.cn/Article/details/gyzyugfil.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.vehdjk.com/Article/details/ghohnjlik.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.yfazqb.com/Article/details/gdlubwwjm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.tarul.cn/Article/details/gzqdamfzi.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.sjlbkw.cn/Article/details/gazhdljfn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.vehdjk.com/Article/details/gtpxgkajh.sHtML

[U04] Py：变量调试打印
来源：http://www.share.bbcook.cn/Article/details/glhkwfbde.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.vehdjk.com/Article/details/gkpxvglif.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.vehdjk.com/Article/details/gaxzjcxfq.sHtML

list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gtutzkxbt.sHtML

[U06] Py：合并两个字典
来源：http://wap.tarul.cn/Article/details/gifrezmin.sHtML

{**a, **b}
来源：http://baike.tarul.cn/Article/details/gayuxfxzs.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/gxwatbbqt.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.epnwcf.com/Article/details/glmiuahee.sHtML

[U08] Py：展平二维列表
来源：http://wap.tarul.cn/Article/details/gfemmpugi.sHtML

[y for x in nested for y in x]
来源：http://m.share.bbcook.cn/Article/details/gpgigopxb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.vehdjk.com/Article/details/grohkozif.sHtML

max(d, key=d.get)
来源：http://www.share.yfazqb.com/Article/details/gbgbycjtc.sHtML

[U10] Py：按值排序字典
来源：http://read.share.vehdjk.com/Article/details/gdrzybdod.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.vehdjk.com/Article/details/gfwmizbda.sHtML

[U11] Py：生成器表达式
来源：http://read.share.tarul.cn/Article/details/giqotkigq.sHtML

(x * 2 for x in arr)
来源：http://m.share.fktsv.cn/Article/details/gfcrjddnn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.epnwcf.com/Article/details/gmnkeqckk.sHtML

Counter(arr).most_common(3)
来源：http://blog.tarul.cn/Article/details/gtusfbgfb.sHtML

[U13] Py：固定长度队列
来源：http://blog.fktsv.cn/Article/details/gxmgkbcjl.sHtML

deque(maxlen=10)
来源：http://baike.bbcook.cn/Article/details/gmdtdjigk.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.epnwcf.com/Article/details/gtedpqcyt.sHtML

defaultdict(list)
来源：http://blog.epnwcf.com/Article/details/gftlqgyex.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.tarul.cn/Article/details/gxfevbtvg.sHtML

t = time.perf_counter()
来源：http://www.blog.bbcook.cn/Article/details/gurjvrqjf.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fktsv.cn/Article/details/gpzgkxrkt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.tarul.cn/Article/details/gpegfonul.sHtML

[U17] Py：初始化日志
来源：http://m.share.epnwcf.com/Article/details/gcccwdadz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.bbcook.cn/Article/details/gzmuzhsgg.sHtML

[U18] Py：预编译正则
来源：http://baike.sjlbkw.cn/Article/details/gwxnlkwke.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fktsv.cn/Article/details/givuumwsv.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.epnwcf.com/Article/details/gukslrorj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fktsv.cn/Article/details/gmnchwglj.sHtML

[U20] Py：缓存函数结果
来源：http://3g.sjlbkw.cn/Article/details/giyesfbpd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.tarul.cn/Article/details/gkdjhtovh.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.epnwcf.com/Article/details/gpemvbgzy.sHtML

@contextlib.contextmanager
来源：http://www.share.sjlbkw.cn/Article/details/gnhxnvjbr.sHtML

[U22] Py：矩阵转置
来源：http://www.share.vehdjk.com/Article/details/gxuqsewso.sHtML

list(zip(*m))
来源：http://www.blog.tarul.cn/Article/details/gqvhgpimj.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.yfazqb.com/Article/details/gvzxtmsyz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.sjlbkw.cn/Article/details/gjphikiur.sHtML

[U24] Py：路径操作
来源：http://baike.vehdjk.com/Article/details/gcpapjxhj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gsolkxnii.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.sjlbkw.cn/Article/details/gpbhfkwez.sHtML

csv.DictReader(f)
来源：http://read.share.vehdjk.com/Article/details/ghdgthazi.sHtML

[U26] Py：并发下载
来源：http://www.share.bbcook.cn/Article/details/glawkhddf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.bbcook.cn/Article/details/gcgrccvpz.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.bbcook.cn/Article/details/gbwycoyui.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.sjlbkw.cn/Article/details/gizpqwidd.sHtML

[U28] Py：类型别名
来源：http://m.share.yfazqb.com/Article/details/ghdqnffdb.sHtML

UserId = int
来源：http://blog.sjlbkw.cn/Article/details/gbklxdfht.sHtML

[U29] Py：属性校验
来源：http://3g.yfazqb.com/Article/details/galmveshk.sHtML

@property 与 @x.setter 配合
来源：http://baike.tarul.cn/Article/details/gaccimiei.sHtML

[U30] Py：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/gpkgskwzp.sHtML

@dataclass(slots=True)
来源：http://www.share.fktsv.cn/Article/details/gvmfrtoco.sHtML

[U31] Py：单测
来源：http://read.share.vehdjk.com/Article/details/gvtmeigsw.sHtML

python -m pytest -q
来源：http://m.share.tarul.cn/Article/details/gkztanpgs.sHtML

[U32] Py：代码格式化
来源：http://baike.sjlbkw.cn/Article/details/gbheteile.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fktsv.cn/Article/details/gqtumvhfk.sHtML

[U33] Py：打包发布
来源：http://wap.epnwcf.com/Article/details/gjaounvus.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.tarul.cn/Article/details/gwfenvbnr.sHtML

[U34] Py：判断编码
来源：http://www.share.yfazqb.com/Article/details/gdsaxlbnm.sHtML

chardet.detect(raw)
来源：http://www.blog.epnwcf.com/Article/details/gqggcbicj.sHtML

[U35] Py：发送邮件
来源：http://blog.bbcook.cn/Article/details/grkivapwm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.yfazqb.com/Article/details/gsaotopse.sHtML

[U36] Py：定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gcopmwveo.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.yfazqb.com/Article/details/gdxmemrxu.sHtML

[U37] Py：读写 Excel
来源：http://blog.tarul.cn/Article/details/gsewthdnw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fktsv.cn/Article/details/gagnaggfd.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.bbcook.cn/Article/details/gcezzwyih.sHtML

Path(__file__).resolve().parent
来源：http://blog.vehdjk.com/Article/details/ghrddishv.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.bbcook.cn/Article/details/glmxlzrqr.sHtML

sys.stdout.isatty()
来源：http://3g.vehdjk.com/Article/details/gqjuahtfl.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.vehdjk.com/Article/details/gnjegsjaw.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxsvvkbw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.vehdjk.com/Article/details/gdozzjede.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.yfazqb.com/Article/details/ghiooloxs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.yfazqb.com/Article/details/gioewndqw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.yfazqb.com/Article/details/gvybansgo.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gxrqjoiux.sHtML

namespace App\Http;
来源：http://www.share.epnwcf.com/Article/details/gayliohjs.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.vehdjk.com/Article/details/gwkuroshg.sHtML

declare(strict_types=1);
来源：http://www.share.fktsv.cn/Article/details/grbaxymwr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.sjlbkw.cn/Article/details/gpsczuxwz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/ghiryckgm.sHtML

[U46] PHP：可空类型
来源：http://wap.vehdjk.com/Article/details/gathxeaoo.sHtML

?string $name = null
来源：http://www.m.share.vehdjk.com/Article/details/gpiroawug.sHtML

[U47] PHP：联合类型
来源：http://www.share.sjlbkw.cn/Article/details/gclfbbavb.sHtML

int|string $id
来源：http://3g.tarul.cn/Article/details/ghtoeptdq.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.vehdjk.com/Article/details/gmepxklxu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fktsv.cn/Article/details/glqmbjnda.sHtML

[U49] PHP：只读属性
来源：http://read.share.bbcook.cn/Article/details/ggqjuqysq.sHtML

public readonly string $name
来源：http://www.share.bbcook.cn/Article/details/gmumvyizg.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.vehdjk.com/Article/details/grtryspsr.sHtML

public function __construct(private int $id) {}
来源：http://blog.vehdjk.com/Article/details/gbcrrnlpq.sHtML

[U51] PHP：数组解构
来源：http://www.share.vehdjk.com/Article/details/gasdwgqwb.sHtML

[$a, $b] = $arr;
来源：http://www.share.vehdjk.com/Article/details/gzxltkily.sHtML

[U52] PHP：箭头函数
来源：http://m.share.sjlbkw.cn/Article/details/gckzixeic.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fktsv.cn/Article/details/gfuaozpqf.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.tarul.cn/Article/details/gkdbbykob.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.sjlbkw.cn/Article/details/gntuafeqk.sHtML

[U54] PHP：空安全调用
来源：http://read.share.sjlbkw.cn/Article/details/gvlpagbht.sHtML

$obj?->method()
来源：http://m.share.bbcook.cn/Article/details/gemvodtwz.sHtML

[U55] PHP：match 表达式
来源：http://3g.fktsv.cn/Article/details/gwekepnyf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.yfazqb.com/Article/details/gcfhllbka.sHtML

[U56] PHP：命名参数
来源：http://m.share.epnwcf.com/Article/details/gigdchtof.sHtML

f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gqukuzsnj.sHtML

[U57] PHP：字符串插值
来源：http://wap.tarul.cn/Article/details/gcyhdytim.sHtML

"值: {$a}"
来源：http://read.share.vehdjk.com/Article/details/gkigdorfn.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fktsv.cn/Article/details/gzddwzypl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fktsv.cn/Article/details/gogkmuupi.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fktsv.cn/Article/details/gvndppctt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gnhkqooza.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.epnwcf.com/Article/details/gpybyqoez.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.sjlbkw.cn/Article/details/gmvrwvfhw.sHtML

[U61] PHP：正则
来源：http://blog.vehdjk.com/Article/details/grkwrlobn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/gnkqvwhft.sHtML

[U62] PHP：日期对象
来源：http://read.share.fktsv.cn/Article/details/gipqbdekk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fktsv.cn/Article/details/gxhmccfku.sHtML

[U63] PHP：文件读写
来源：http://3g.yfazqb.com/Article/details/gneailovn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.epnwcf.com/Article/details/gouyseude.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.tarul.cn/Article/details/gurelryrh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.tarul.cn/Article/details/gdhwkyisc.sHtML

[U65] PHP：会话
来源：http://blog.tarul.cn/Article/details/gixywuvfa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.bbcook.cn/Article/details/gsmqocqtn.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.sjlbkw.cn/Article/details/gwskyinwv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.tarul.cn/Article/details/gmdzfkvfz.sHtML

[U67] PHP：处理文件上传
来源：http://wap.bbcook.cn/Article/details/gtdymvsey.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.epnwcf.com/Article/details/gprrdofmk.sHtML

[U68] PHP：PDO 连接
来源：http://baike.epnwcf.com/Article/details/ghgffgaxt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.epnwcf.com/Article/details/gjlwxjksv.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fktsv.cn/Article/details/gqojnwahm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.epnwcf.com/Article/details/gdtgujybr.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.vehdjk.com/Article/details/gjlxvfscs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.vehdjk.com/Article/details/gtnbtaase.sHtML

[U71] PHP：抛出异常
来源：http://3g.tarul.cn/Article/details/gzdwzrxhg.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.epnwcf.com/Article/details/gxgeqlckz.sHtML

[U72] PHP：写错误日志
来源：http://wap.tarul.cn/Article/details/gqjjdiwrz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.vehdjk.com/Article/details/gmkepoxuw.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.vehdjk.com/Article/details/gzhajlqyd.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.sjlbkw.cn/Article/details/gjtsxmtqo.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.epnwcf.com/Article/details/gzznsenbz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.sjlbkw.cn/Article/details/gmapoarah.sHtML

[U75] PHP：依赖注入
来源：http://mobile.tarul.cn/Article/details/grdedhwhe.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/gmvotbvoc.sHtML

[U76] PHP：简单路由
来源：http://mobile.vehdjk.com/Article/details/ggvnzhsno.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.epnwcf.com/Article/details/gzktysxmb.sHtML


<!-- 参考信息 -->