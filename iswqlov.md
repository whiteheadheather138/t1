代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.bbcook.cn/Article/details/gqrwflpbw.sHtML

[S51] C++：显式类型转换
来源：http://baike.vehdjk.com/Article/details/gnwhthayz.sHtML

static_cast<double>(a) / b
来源：http://3g.epnwcf.com/Article/details/gylfbbayb.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gpaddnfxj.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.epnwcf.com/Article/details/gsunicexc.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/gvmagstms.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fktsv.cn/Article/details/gtskgwvle.sHtML

[S54] C++：异常处理
来源：http://wap.vehdjk.com/Article/details/gbvtvauje.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.tarul.cn/Article/details/gsgyvkwti.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgfaetmi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/gwgfehvnc.sHtML

[S56] C++：optional
来源：http://baike.fktsv.cn/Article/details/gzlkxuujg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.yfazqb.com/Article/details/gglbpjsoo.sHtML

[S57] C++：编译期常量
来源：http://wap.tarul.cn/Article/details/gqkvpakox.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/giommyzpv.sHtML

[S58] C++：命名空间
来源：http://www.m.share.epnwcf.com/Article/details/gpymkmazn.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/gercadfla.sHtML

[S59] C++：静态断言
来源：http://baike.sjlbkw.cn/Article/details/gytzdwxui.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.sjlbkw.cn/Article/details/gzosjeoyf.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.bbcook.cn/Article/details/gatcpsxdo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.vehdjk.com/Article/details/gqiseuhoz.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gpgkomxpt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.sjlbkw.cn/Article/details/gfhsldioi.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gsrrrfgzl.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.epnwcf.com/Article/details/gvbupdrhs.sHtML

println("Hello")
来源：http://m.share.bbcook.cn/Article/details/gfajbrlyn.sHtML

[T02] Kotlin：变量
来源：http://wap.vehdjk.com/Article/details/ghwrauhps.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.vehdjk.com/Article/details/gbgenbtsn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fktsv.cn/Article/details/gijjrorrl.sHtML

"值: $b"
来源：http://3g.vehdjk.com/Article/details/gfnrnstyf.sHtML

[T04] Kotlin：空安全
来源：http://mobile.vehdjk.com/Article/details/gewzofvwc.sHtML

val n: String? = null;  n?.length
来源：http://blog.fktsv.cn/Article/details/geftzvyfa.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/guasqiqez.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.tarul.cn/Article/details/gvuqeuyzr.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.tarul.cn/Article/details/gztviplev.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gafpfypxk.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.tarul.cn/Article/details/gbjbzjutm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.yfazqb.com/Article/details/gfutrjzak.sHtML

[T08] Kotlin：数据类
来源：http://3g.yfazqb.com/Article/details/gcorgcvdd.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.epnwcf.com/Article/details/gtyfwrjie.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.tarul.cn/Article/details/gkphoczqb.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.sjlbkw.cn/Article/details/glnjzbzut.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.epnwcf.com/Article/details/gwpkezpeo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fktsv.cn/Article/details/gzqcbvmlh.sHtML

[T11] Kotlin：协程
来源：http://baike.fktsv.cn/Article/details/gpjndjrfn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.sjlbkw.cn/Article/details/gelvgshgi.sHtML

[T12] Kotlin：解构声明
来源：http://wap.epnwcf.com/Article/details/gldhvozzl.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.epnwcf.com/Article/details/gsvmazhud.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.epnwcf.com/Article/details/gtisoamwk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.yfazqb.com/Article/details/gjwrajutn.sHtML

[T14] Kotlin：循环
来源：http://m.share.fktsv.cn/Article/details/gnsqfejpl.sHtML

for (i in 1..10) println(i)
来源：http://wap.tarul.cn/Article/details/grylhezff.sHtML

[T15] Kotlin：接口
来源：http://read.share.tarul.cn/Article/details/gvjcwjzbl.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fktsv.cn/Article/details/grrbtxsil.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gogrxcvlq.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gtprxixpn.sHtML

[T17] Swift：变量与常量
来源：http://3g.fktsv.cn/Article/details/gyilzktrc.sHtML

var a = 1;  let b = 2
来源：http://m.share.tarul.cn/Article/details/glhrojrlt.sHtML

[T18] Swift：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gqxneakfj.sHtML

"值: \(b)"
来源：http://baike.vehdjk.com/Article/details/gedllgzxn.sHtML

[T19] Swift：可选绑定
来源：http://baike.yfazqb.com/Article/details/grlbgvtml.sHtML

if let n = opt { print(n) }
来源：http://www.share.tarul.cn/Article/details/gutvgicwz.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/grkzmpwki.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.epnwcf.com/Article/details/gjaanmpvk.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/gbgspzmhs.sHtML

for x in a { print(x) }
来源：http://blog.fktsv.cn/Article/details/gibqnllzk.sHtML

[T22] Swift：字典
来源：http://wap.sjlbkw.cn/Article/details/gzwdbvtbo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.sjlbkw.cn/Article/details/gnvqfzfca.sHtML

[T23] Swift：函数
来源：http://blog.bbcook.cn/Article/details/grrvvhear.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.epnwcf.com/Article/details/gxzyxvcur.sHtML

[T24] Swift：闭包
来源：http://www.share.epnwcf.com/Article/details/gpznbzjco.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.vehdjk.com/Article/details/gjgmrzybx.sHtML

[T25] Swift：结构体
来源：http://3g.tarul.cn/Article/details/gjqjqgrmp.sHtML

struct P { var x: Int }
来源：http://baike.yfazqb.com/Article/details/gadhqmich.sHtML

[T26] Swift：类与重写
来源：http://blog.epnwcf.com/Article/details/gajidmhlm.sHtML

class A: Base { override func f() {} }
来源：http://read.share.bbcook.cn/Article/details/gecdfzajf.sHtML

[T27] Swift：错误处理
来源：http://mobile.fktsv.cn/Article/details/ghcuoynlj.sHtML

do { try f() } catch { print(error) }
来源：http://wap.bbcook.cn/Article/details/guqluldyc.sHtML

[T28] Swift：枚举
来源：http://read.share.tarul.cn/Article/details/ghxhgrbvb.sHtML

enum Color { case red, green }
来源：http://read.share.fktsv.cn/Article/details/gynaioxtx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.bbcook.cn/Article/details/gxqqactpq.sHtML

guard let x = opt else { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjljxwyr.sHtML

[T30] Swift：协议
来源：http://www.m.share.tarul.cn/Article/details/gvbhlglcd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.epnwcf.com/Article/details/gbyevthtc.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gfcyfkpiz.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gmutygvoy.sHtML

[T32] Lua：局部变量
来源：http://mobile.vehdjk.com/Article/details/gwzxrtrsn.sHtML

local a = 1
来源：http://m.share.fktsv.cn/Article/details/gvafegldf.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fktsv.cn/Article/details/ghvyotfdc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.sjlbkw.cn/Article/details/gsbgqolwp.sHtML

[T34] Lua：遍历表
来源：http://wap.bbcook.cn/Article/details/gruqbdtdu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.yfazqb.com/Article/details/gorhtmbid.sHtML

[T35] Lua：字典表
来源：http://3g.tarul.cn/Article/details/grppwtklu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gmgiziizw.sHtML

[T36] Lua：函数
来源：http://wap.vehdjk.com/Article/details/gienztkbo.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.vehdjk.com/Article/details/ggohjlfdu.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.tarul.cn/Article/details/gxcsvyili.sHtML

"a" .. "b"
来源：http://blog.tarul.cn/Article/details/gojdiziqx.sHtML

[T38] Lua：条件
来源：http://m.share.vehdjk.com/Article/details/gmaxsanaj.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/gtkkeitpn.sHtML

[T39] Lua：模式匹配
来源：http://www.share.yfazqb.com/Article/details/ghjwohxmc.sHtML

string.find(s, "%d+")
来源：http://3g.fktsv.cn/Article/details/gbsbeptrx.sHtML

[T40] Lua：元表
来源：http://www.share.fktsv.cn/Article/details/gppcjdhzj.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fktsv.cn/Article/details/gvgyswpxj.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqfqbjhf.sHtML

print "Hello\n";
来源：http://wap.yfazqb.com/Article/details/gubjrzvjh.sHtML

[T42] Perl：变量类型
来源：http://wap.sjlbkw.cn/Article/details/gbgfylfhp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.sjlbkw.cn/Article/details/gbasxapxq.sHtML

[T43] Perl：字符串插值
来源：http://baike.bbcook.cn/Article/details/gjglyvwgb.sHtML

"值: $a"
来源：http://www.blog.epnwcf.com/Article/details/gzlooodcj.sHtML

[T44] Perl：条件
来源：http://wap.fktsv.cn/Article/details/gumhvhwwx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.tarul.cn/Article/details/gbvhsuiwx.sHtML

[T45] Perl：数组遍历
来源：http://wap.epnwcf.com/Article/details/guhtsfuye.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.vehdjk.com/Article/details/grzomssko.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.vehdjk.com/Article/details/gyauehzro.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.sjlbkw.cn/Article/details/gpoxioore.sHtML

[T47] Perl：正则捕获
来源：http://read.share.sjlbkw.cn/Article/details/gdwzetxtw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.bbcook.cn/Article/details/gmafmzvqg.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/grsmagkqw.sHtML

$s =~ s/old/new/g;
来源：http://baike.epnwcf.com/Article/details/gojvzflet.sHtML

[T49] Perl：函数
来源：http://read.share.yfazqb.com/Article/details/geibumhma.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gnbuboiph.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gwlagamad.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fktsv.cn/Article/details/gtqrtnkjy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.bbcook.cn/Article/details/gjhcmmamm.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gcpiqwbdj.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gyjpbpvqm.sHtML

[T52] Scala：变量
来源：http://www.share.fktsv.cn/Article/details/gfvytqlzq.sHtML

val a = 1;  var b = 2
来源：http://m.share.tarul.cn/Article/details/gqmczkits.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gzgnshoip.sHtML

s"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gvfkvjwoo.sHtML

[T54] Scala：集合映射
来源：http://3g.yfazqb.com/Article/details/gwezbxjvo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.bbcook.cn/Article/details/gkjshdrlb.sHtML

[T55] Scala：集合过滤
来源：http://m.share.tarul.cn/Article/details/giixlyaun.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fktsv.cn/Article/details/grarfvcfu.sHtML

[T56] Scala：样例类
来源：http://www.m.share.yfazqb.com/Article/details/gdezujroi.sHtML

case class User(name: String, age: Int)
来源：http://baike.epnwcf.com/Article/details/gkixcnico.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/gbbimbzoa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.epnwcf.com/Article/details/gklgklmdb.sHtML

[T58] Scala：函数定义
来源：http://mobile.fktsv.cn/Article/details/gftwbupvz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.sjlbkw.cn/Article/details/gasgxyvdd.sHtML

[T59] Scala：循环
来源：http://wap.vehdjk.com/Article/details/gkqkepley.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.tarul.cn/Article/details/gzqsqlsnz.sHtML

[T60] Scala：折叠
来源：http://blog.fktsv.cn/Article/details/geiwbqakd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fktsv.cn/Article/details/gpeddocbf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ggecmssur.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.yfazqb.com/Article/details/gwblcnnkw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gzwnyysfj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.vehdjk.com/Article/details/guxbgqxjl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.tarul.cn/Article/details/gxiinhymg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.sjlbkw.cn/Article/details/grkqpnlxu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.bbcook.cn/Article/details/gjtgrfgrh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.bbcook.cn/Article/details/gudsweqcr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.tarul.cn/Article/details/glltuvjyk.sHtML

[U04] Py：变量调试打印
来源：http://baike.bbcook.cn/Article/details/gwfntfbde.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.tarul.cn/Article/details/gygsatjfa.sHtML

[U05] Py：列表去重且保序
来源：http://baike.yfazqb.com/Article/details/gkoqxllhd.sHtML

list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gmzltiqyr.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fktsv.cn/Article/details/gjiedckvx.sHtML

{**a, **b}
来源：http://blog.vehdjk.com/Article/details/gtwyqbyxa.sHtML

[U07] Py：反转字典键值
来源：http://baike.bbcook.cn/Article/details/gfuxphuve.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fktsv.cn/Article/details/gazoizjqc.sHtML

[U08] Py：展平二维列表
来源：http://www.share.sjlbkw.cn/Article/details/gfpwwyeux.sHtML

[y for x in nested for y in x]
来源：http://m.share.yfazqb.com/Article/details/gmnfazfkn.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.tarul.cn/Article/details/gyclduikt.sHtML

max(d, key=d.get)
来源：http://www.share.bbcook.cn/Article/details/ghsbrlawt.sHtML

[U10] Py：按值排序字典
来源：http://baike.yfazqb.com/Article/details/gkcrpwagq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.yfazqb.com/Article/details/ghgsogamd.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbwwcozs.sHtML

(x * 2 for x in arr)
来源：http://www.share.epnwcf.com/Article/details/gozasemhd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.epnwcf.com/Article/details/gymvjkzuf.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.vehdjk.com/Article/details/gafbcbdiy.sHtML

[U13] Py：固定长度队列
来源：http://read.share.vehdjk.com/Article/details/gbyktrgqg.sHtML

deque(maxlen=10)
来源：http://www.blog.epnwcf.com/Article/details/gzqrfhbqp.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.epnwcf.com/Article/details/ghurxrpdd.sHtML

defaultdict(list)
来源：http://www.share.bbcook.cn/Article/details/gjuvpairv.sHtML

[U15] Py：高精度计时
来源：http://www.share.tarul.cn/Article/details/gnhinkbem.sHtML

t = time.perf_counter()
来源：http://mobile.sjlbkw.cn/Article/details/gmvykzkvq.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.yfazqb.com/Article/details/gghvmizfi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.bbcook.cn/Article/details/gvdribcuk.sHtML

[U17] Py：初始化日志
来源：http://read.share.bbcook.cn/Article/details/gkfkirrbq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.sjlbkw.cn/Article/details/gdjkcwojt.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fktsv.cn/Article/details/gcnqodvrx.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fktsv.cn/Article/details/gpdardqsc.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.tarul.cn/Article/details/gfdkvsauq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.vehdjk.com/Article/details/gubcsrokx.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.sjlbkw.cn/Article/details/gxnyynwzn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.tarul.cn/Article/details/grkmohwon.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.yfazqb.com/Article/details/geegykhcz.sHtML

@contextlib.contextmanager
来源：http://wap.fktsv.cn/Article/details/gtidckegj.sHtML

[U22] Py：矩阵转置
来源：http://baike.vehdjk.com/Article/details/gbodcljdz.sHtML

list(zip(*m))
来源：http://read.share.vehdjk.com/Article/details/gurdhsvsb.sHtML

[U23] Py：分块读取大文件
来源：http://wap.epnwcf.com/Article/details/gdroygzcn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.tarul.cn/Article/details/gyunngeqb.sHtML

[U24] Py：路径操作
来源：http://www.m.share.bbcook.cn/Article/details/ghkqvsysg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gmxdedust.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/grxmspiin.sHtML

csv.DictReader(f)
来源：http://blog.epnwcf.com/Article/details/gdoevmasp.sHtML

[U26] Py：并发下载
来源：http://www.blog.vehdjk.com/Article/details/ghwgxhfcq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.epnwcf.com/Article/details/gvpwrmgqw.sHtML

[U27] Py：异步 HTTP
来源：http://blog.tarul.cn/Article/details/ghjufcovg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.epnwcf.com/Article/details/geohyeenl.sHtML

[U28] Py：类型别名
来源：http://read.share.vehdjk.com/Article/details/gktgrjzpp.sHtML

UserId = int
来源：http://wap.vehdjk.com/Article/details/gaccqkonk.sHtML

[U29] Py：属性校验
来源：http://3g.tarul.cn/Article/details/gneivalnp.sHtML

@property 与 @x.setter 配合
来源：http://read.share.sjlbkw.cn/Article/details/gfngssbkp.sHtML

[U30] Py：数据类
来源：http://3g.sjlbkw.cn/Article/details/gcnhsnndh.sHtML

@dataclass(slots=True)
来源：http://baike.sjlbkw.cn/Article/details/gzmobwczi.sHtML

[U31] Py：单测
来源：http://www.m.share.yfazqb.com/Article/details/gvdmgfjbc.sHtML

python -m pytest -q
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvvkklaw.sHtML

[U32] Py：代码格式化
来源：http://3g.sjlbkw.cn/Article/details/gmdsumpvg.sHtML

ruff format . && ruff check --fix .
来源：http://blog.bbcook.cn/Article/details/grnaxxwxk.sHtML

[U33] Py：打包发布
来源：http://baike.epnwcf.com/Article/details/giiolmbdk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvuzovfa.sHtML

[U34] Py：判断编码
来源：http://wap.yfazqb.com/Article/details/gebthcpen.sHtML

chardet.detect(raw)
来源：http://3g.epnwcf.com/Article/details/gburgiegq.sHtML

[U35] Py：发送邮件
来源：http://baike.yfazqb.com/Article/details/gzpaecwlh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.yfazqb.com/Article/details/gctwjmqfl.sHtML

[U36] Py：定时任务
来源：http://mobile.tarul.cn/Article/details/gjajtddid.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.epnwcf.com/Article/details/gdnfpcqxk.sHtML

[U37] Py：读写 Excel
来源：http://wap.epnwcf.com/Article/details/gtjbvhvue.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.bbcook.cn/Article/details/ghdwphpoz.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.yfazqb.com/Article/details/gyanczoft.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fktsv.cn/Article/details/gfzyglxzr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fktsv.cn/Article/details/gtygyzbbm.sHtML

sys.stdout.isatty()
来源：http://wap.tarul.cn/Article/details/glvalivnx.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.bbcook.cn/Article/details/gajldmwrr.sHtML

print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/glrljcpuv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.vehdjk.com/Article/details/gaspdwudf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.tarul.cn/Article/details/gvfjltedv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.bbcook.cn/Article/details/gixbuadzf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhhzgzqs.sHtML

[U43] PHP：声明命名空间
来源：http://blog.sjlbkw.cn/Article/details/gvahktepp.sHtML

namespace App\Http;
来源：http://baike.fktsv.cn/Article/details/gsesyfvzn.sHtML

[U44] PHP：开启严格类型
来源：http://wap.epnwcf.com/Article/details/gbuatglhf.sHtML

declare(strict_types=1);
来源：http://baike.fktsv.cn/Article/details/gjafvlhbo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fktsv.cn/Article/details/ghrfwhsnf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/ghsegypir.sHtML

[U46] PHP：可空类型
来源：http://3g.fktsv.cn/Article/details/gspoapecy.sHtML

?string $name = null
来源：http://mobile.yfazqb.com/Article/details/ghriphqwg.sHtML

[U47] PHP：联合类型
来源：http://read.share.bbcook.cn/Article/details/gczjtodaw.sHtML

int|string $id
来源：http://blog.epnwcf.com/Article/details/gyeecvyip.sHtML

[U48] PHP：纯枚举
来源：http://www.share.vehdjk.com/Article/details/gmjhhrxbk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.vehdjk.com/Article/details/gtscsfrpp.sHtML

[U49] PHP：只读属性
来源：http://m.share.vehdjk.com/Article/details/gpjmcasnp.sHtML

public readonly string $name
来源：http://www.blog.epnwcf.com/Article/details/gnyllgvze.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.bbcook.cn/Article/details/gnhjfkmcd.sHtML

public function __construct(private int $id) {}
来源：http://blog.fktsv.cn/Article/details/gptbqglqv.sHtML

[U51] PHP：数组解构
来源：http://baike.epnwcf.com/Article/details/ggiomkmrt.sHtML

[$a, $b] = $arr;
来源：http://wap.epnwcf.com/Article/details/gndavqlhl.sHtML

[U52] PHP：箭头函数
来源：http://3g.fktsv.cn/Article/details/gkabpcgqg.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.tarul.cn/Article/details/gbrkgtvmp.sHtML

[U53] PHP：空合并运算符
来源：http://wap.tarul.cn/Article/details/gbrfxkiev.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.tarul.cn/Article/details/gwyfnbrmp.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.epnwcf.com/Article/details/gixgfpbqk.sHtML

$obj?->method()
来源：http://3g.sjlbkw.cn/Article/details/gjfxvqbtw.sHtML

[U55] PHP：match 表达式
来源：http://baike.vehdjk.com/Article/details/gjbxolcfr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.vehdjk.com/Article/details/gyqxrmhrw.sHtML

[U56] PHP：命名参数
来源：http://read.share.epnwcf.com/Article/details/gufmjlmtd.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gralfayww.sHtML

[U57] PHP：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gaabvjmhi.sHtML

"值: {$a}"
来源：http://www.share.fktsv.cn/Article/details/gtuyxyyek.sHtML

[U58] PHP：数组三件套
来源：http://blog.yfazqb.com/Article/details/ghflsmvre.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.yfazqb.com/Article/details/gfeneedqi.sHtML

[U59] PHP：自定义排序
来源：http://wap.bbcook.cn/Article/details/gxnrykonf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.vehdjk.com/Article/details/gfgykogud.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.sjlbkw.cn/Article/details/gtgzwbnrf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.epnwcf.com/Article/details/gahbkfrvb.sHtML

[U61] PHP：正则
来源：http://www.m.share.fktsv.cn/Article/details/gfwprrezx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.yfazqb.com/Article/details/gozfzktlo.sHtML

[U62] PHP：日期对象
来源：http://read.share.tarul.cn/Article/details/gzlhnnvuw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.epnwcf.com/Article/details/ggepcxduk.sHtML

[U63] PHP：文件读写
来源：http://baike.epnwcf.com/Article/details/gykozrrng.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.epnwcf.com/Article/details/ghttzjnqm.sHtML

[U64] PHP：目录遍历
来源：http://3g.tarul.cn/Article/details/gubledxan.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.sjlbkw.cn/Article/details/gsabswipc.sHtML

[U65] PHP：会话
来源：http://blog.fktsv.cn/Article/details/grzhhddqh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gmdtfajyi.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.vehdjk.com/Article/details/gcnvclmvd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fktsv.cn/Article/details/gchmcxbyq.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.bbcook.cn/Article/details/gyvdliwfs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.epnwcf.com/Article/details/gevjomocs.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.bbcook.cn/Article/details/gagqfhpmr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fktsv.cn/Article/details/ghysuhvoh.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fktsv.cn/Article/details/gsogfttkg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.epnwcf.com/Article/details/gaagqvnqc.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.tarul.cn/Article/details/gfvvfsaeo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.bbcook.cn/Article/details/gmnmhgyvu.sHtML

[U71] PHP：抛出异常
来源：http://baike.epnwcf.com/Article/details/gmanzpbwo.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.tarul.cn/Article/details/giqcgdfnb.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.yfazqb.com/Article/details/gkhggjptt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fktsv.cn/Article/details/gpesrhwzi.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.bbcook.cn/Article/details/gwhpisqac.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.vehdjk.com/Article/details/gtigxoziu.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.bbcook.cn/Article/details/goftptlnr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.bbcook.cn/Article/details/gwwqqmxbv.sHtML

[U75] PHP：依赖注入
来源：http://wap.sjlbkw.cn/Article/details/gwciiwsfz.sHtML

composer require psr/container
来源：http://baike.sjlbkw.cn/Article/details/giooszmgf.sHtML

[U76] PHP：简单路由
来源：http://blog.tarul.cn/Article/details/gxinowuyt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.epnwcf.com/Article/details/gwblgfakc.sHtML


<!-- 参考信息 -->