代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gkxmmsohk.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.tarul.cn/Article/details/gzglrjsvr.sHtML

static_cast<double>(a) / b
来源：http://blog.fktsv.cn/Article/details/gmeeairvk.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.sjlbkw.cn/Article/details/gzpcjxwdn.sHtML

int size() const noexcept { return n_; }
来源：http://wap.sjlbkw.cn/Article/details/gojgsmtxd.sHtML

[S53] C++：移动语义
来源：http://baike.vehdjk.com/Article/details/guekwjcey.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fktsv.cn/Article/details/gbpleluoz.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/gbipcxpff.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.tarul.cn/Article/details/gzfvvykuq.sHtML

[S55] C++：结构化绑定
来源：http://mobile.sjlbkw.cn/Article/details/gsgtwppjm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/gofojdudv.sHtML

[S56] C++：optional
来源：http://www.blog.vehdjk.com/Article/details/gumrjflgq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/gfapgmhev.sHtML

[S57] C++：编译期常量
来源：http://baike.bbcook.cn/Article/details/gtonlpnbs.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/gxgsrqkxs.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/gyksicvwu.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.sjlbkw.cn/Article/details/goxjuzsfa.sHtML

[S59] C++：静态断言
来源：http://mobile.yfazqb.com/Article/details/gbwwkhitw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.epnwcf.com/Article/details/geheaubxu.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.vehdjk.com/Article/details/gtbfohavz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gkyzkgybr.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gvcwneqfa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.vehdjk.com/Article/details/gtvdefmbt.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gurverhlw.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.bbcook.cn/Article/details/grglvajls.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gqhfoxzdf.sHtML

[T02] Kotlin：变量
来源：http://read.share.vehdjk.com/Article/details/gjpmmnscc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.yfazqb.com/Article/details/gguavlqgg.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.vehdjk.com/Article/details/gkndglbjn.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gzktzskht.sHtML

[T04] Kotlin：空安全
来源：http://read.share.epnwcf.com/Article/details/gkgiuqmdk.sHtML

val n: String? = null;  n?.length
来源：http://wap.bbcook.cn/Article/details/gztreohui.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.bbcook.cn/Article/details/glfsbpwix.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.tarul.cn/Article/details/gfyiycwvi.sHtML

[T06] Kotlin：集合映射
来源：http://wap.bbcook.cn/Article/details/gzpojrwfd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.yfazqb.com/Article/details/gjfqjemns.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.tarul.cn/Article/details/goathvsnd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.sjlbkw.cn/Article/details/gelclrbfu.sHtML

[T08] Kotlin：数据类
来源：http://blog.vehdjk.com/Article/details/ggthrqfvy.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.bbcook.cn/Article/details/gejtnoctu.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.yfazqb.com/Article/details/gunbcyjvg.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.yfazqb.com/Article/details/gojlnlriz.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.vehdjk.com/Article/details/gtlggayzt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.yfazqb.com/Article/details/gywsipoyc.sHtML

[T11] Kotlin：协程
来源：http://m.share.sjlbkw.cn/Article/details/gldekzkxu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.tarul.cn/Article/details/gvlvdhipo.sHtML

[T12] Kotlin：解构声明
来源：http://baike.sjlbkw.cn/Article/details/gwfsenncv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gosncomfo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.vehdjk.com/Article/details/ghrirbwhi.sHtML

val m = mapOf("a" to 1)
来源：http://blog.tarul.cn/Article/details/gsjkzmwaz.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fktsv.cn/Article/details/ggddrsefx.sHtML

for (i in 1..10) println(i)
来源：http://wap.fktsv.cn/Article/details/ggtiuchdv.sHtML

[T15] Kotlin：接口
来源：http://blog.tarul.cn/Article/details/gilplzkvd.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.vehdjk.com/Article/details/gyqvigyrz.sHtML

[T16] Swift：Hello World
来源：http://wap.sjlbkw.cn/Article/details/ggueralon.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/glplploxa.sHtML

[T17] Swift：变量与常量
来源：http://baike.fktsv.cn/Article/details/gvdpuhxmq.sHtML

var a = 1;  let b = 2
来源：http://mobile.fktsv.cn/Article/details/gkgibdyyf.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gflhepmrg.sHtML

"值: \(b)"
来源：http://www.blog.sjlbkw.cn/Article/details/gcphnjejj.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fktsv.cn/Article/details/ghcxsqyre.sHtML

if let n = opt { print(n) }
来源：http://www.blog.vehdjk.com/Article/details/ghlqjtnju.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.tarul.cn/Article/details/guccjvarh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/gnkenvfov.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/glzkejzal.sHtML

for x in a { print(x) }
来源：http://3g.vehdjk.com/Article/details/gjgeouubc.sHtML

[T22] Swift：字典
来源：http://blog.sjlbkw.cn/Article/details/gmvqotrzm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fktsv.cn/Article/details/gkhgivsya.sHtML

[T23] Swift：函数
来源：http://m.share.epnwcf.com/Article/details/goxsmqnrn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.yfazqb.com/Article/details/gjyspdwdq.sHtML

[T24] Swift：闭包
来源：http://wap.fktsv.cn/Article/details/giukdqwrz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.vehdjk.com/Article/details/gieyhslxy.sHtML

[T25] Swift：结构体
来源：http://baike.tarul.cn/Article/details/gsbzitkqt.sHtML

struct P { var x: Int }
来源：http://www.m.share.epnwcf.com/Article/details/goqlguxgr.sHtML

[T26] Swift：类与重写
来源：http://www.share.epnwcf.com/Article/details/guvszwamg.sHtML

class A: Base { override func f() {} }
来源：http://3g.yfazqb.com/Article/details/gdcnfvxfc.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/gmbfvltyt.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/gbwgaarqc.sHtML

[T28] Swift：枚举
来源：http://blog.tarul.cn/Article/details/gtmqbqovp.sHtML

enum Color { case red, green }
来源：http://blog.epnwcf.com/Article/details/gkpsnmjfg.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gkdqeumhu.sHtML

guard let x = opt else { return }
来源：http://www.m.share.bbcook.cn/Article/details/gocynpbso.sHtML

[T30] Swift：协议
来源：http://baike.yfazqb.com/Article/details/ggetmnmtk.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.tarul.cn/Article/details/gvnvrvmtp.sHtML

[T31] Lua：Hello World
来源：http://3g.vehdjk.com/Article/details/gvxdhsyay.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/gjkgxphvj.sHtML

[T32] Lua：局部变量
来源：http://3g.vehdjk.com/Article/details/gzemmkavj.sHtML

local a = 1
来源：http://www.share.vehdjk.com/Article/details/gchfnekua.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fktsv.cn/Article/details/gujcaxuir.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.tarul.cn/Article/details/gjstevngw.sHtML

[T34] Lua：遍历表
来源：http://mobile.bbcook.cn/Article/details/gebyiengq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.bbcook.cn/Article/details/gaglqyvns.sHtML

[T35] Lua：字典表
来源：http://m.share.vehdjk.com/Article/details/gbrtcmmwc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.vehdjk.com/Article/details/gcgziyzej.sHtML

[T36] Lua：函数
来源：http://read.share.vehdjk.com/Article/details/gjnsexalg.sHtML

function add(a, b) return a + b end
来源：http://m.share.vehdjk.com/Article/details/gvuyaclbl.sHtML

[T37] Lua：字符串拼接
来源：http://blog.tarul.cn/Article/details/gjppoamwi.sHtML

"a" .. "b"
来源：http://blog.epnwcf.com/Article/details/gmnqxqutm.sHtML

[T38] Lua：条件
来源：http://m.share.bbcook.cn/Article/details/gcxvcadno.sHtML

if x > 0 then print("正") end
来源：http://www.blog.bbcook.cn/Article/details/gxxfhmgrl.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gugaswxav.sHtML

string.find(s, "%d+")
来源：http://www.m.share.tarul.cn/Article/details/gndlqkaic.sHtML

[T40] Lua：元表
来源：http://blog.epnwcf.com/Article/details/gwyphsgel.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.yfazqb.com/Article/details/gwmmvvtyr.sHtML

[T41] Perl：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gmtehqmts.sHtML

print "Hello\n";
来源：http://3g.sjlbkw.cn/Article/details/gctfnsdoy.sHtML

[T42] Perl：变量类型
来源：http://www.share.fktsv.cn/Article/details/gwxroqaim.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.yfazqb.com/Article/details/gnbffxexi.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gclrtiqgd.sHtML

"值: $a"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtmvqcjw.sHtML

[T44] Perl：条件
来源：http://3g.tarul.cn/Article/details/ggqcowvbx.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.bbcook.cn/Article/details/gxepijxuo.sHtML

[T45] Perl：数组遍历
来源：http://read.share.bbcook.cn/Article/details/gzkeccgzk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.sjlbkw.cn/Article/details/gesoicgzy.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.vehdjk.com/Article/details/gujwqrahe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fktsv.cn/Article/details/gbkldjlsg.sHtML

[T47] Perl：正则捕获
来源：http://mobile.bbcook.cn/Article/details/ghfqfhcgu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fktsv.cn/Article/details/gdtubhpyv.sHtML

[T48] Perl：正则替换
来源：http://wap.epnwcf.com/Article/details/gfihsaxyo.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/ggmbfiwjb.sHtML

[T49] Perl：函数
来源：http://www.share.bbcook.cn/Article/details/gxxwehbzj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/goxhowczk.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.tarul.cn/Article/details/ghkfofran.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.yfazqb.com/Article/details/gmjmfziaa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.bbcook.cn/Article/details/gxdknxuzi.sHtML

[T51] Scala：Hello World
来源：http://www.blog.vehdjk.com/Article/details/ghkhfcpbt.sHtML

println("Hello")
来源：http://wap.fktsv.cn/Article/details/gzvhpmsbo.sHtML

[T52] Scala：变量
来源：http://blog.fktsv.cn/Article/details/gymdvgebh.sHtML

val a = 1;  var b = 2
来源：http://blog.tarul.cn/Article/details/gsuxradcg.sHtML

[T53] Scala：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gbjzmsyww.sHtML

s"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gxrjpdbzk.sHtML

[T54] Scala：集合映射
来源：http://blog.tarul.cn/Article/details/gicjkhdrl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.epnwcf.com/Article/details/gtjfgjnzp.sHtML

[T55] Scala：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gnkjmzlmg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.vehdjk.com/Article/details/ggforehsp.sHtML

[T56] Scala：样例类
来源：http://mobile.bbcook.cn/Article/details/ggojepteh.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/ggnsluhjr.sHtML

[T57] Scala：模式匹配
来源：http://read.share.tarul.cn/Article/details/gidkvrxxn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.tarul.cn/Article/details/ghosavwkj.sHtML

[T58] Scala：函数定义
来源：http://read.share.tarul.cn/Article/details/gukwsdxtu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.vehdjk.com/Article/details/gkgrxcafs.sHtML

[T59] Scala：循环
来源：http://m.share.bbcook.cn/Article/details/gxcpffkrl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gfpeigjot.sHtML

[T60] Scala：折叠
来源：http://wap.yfazqb.com/Article/details/gqmjhnuoq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/grhmsdtnw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gutuyobyc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/gahamfthx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gocyejhgi.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fktsv.cn/Article/details/gpmgumkvn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.bbcook.cn/Article/details/grxmjbakn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fktsv.cn/Article/details/gieltsdtt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.sjlbkw.cn/Article/details/ghaxfvgkq.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fktsv.cn/Article/details/gkdafadyh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gczfsrpfa.sHtML

[U04] Py：变量调试打印
来源：http://mobile.vehdjk.com/Article/details/gltzquwlk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.tarul.cn/Article/details/gigejywvn.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.yfazqb.com/Article/details/gzsstkypy.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gtwbeksga.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fktsv.cn/Article/details/ggatwpgwc.sHtML

{**a, **b}
来源：http://www.blog.epnwcf.com/Article/details/gcnxdguic.sHtML

[U07] Py：反转字典键值
来源：http://baike.fktsv.cn/Article/details/gazndomxt.sHtML

{v: k for k, v in d.items()}
来源：http://wap.bbcook.cn/Article/details/gksfbosih.sHtML

[U08] Py：展平二维列表
来源：http://mobile.vehdjk.com/Article/details/gkmodjkhq.sHtML

[y for x in nested for y in x]
来源：http://3g.bbcook.cn/Article/details/gluardvdi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.vehdjk.com/Article/details/gbekskfze.sHtML

max(d, key=d.get)
来源：http://mobile.sjlbkw.cn/Article/details/gybbuiwqe.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/gwnvvbhyz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.bbcook.cn/Article/details/guvlhxvec.sHtML

[U11] Py：生成器表达式
来源：http://mobile.vehdjk.com/Article/details/gdnteqneq.sHtML

(x * 2 for x in arr)
来源：http://m.share.yfazqb.com/Article/details/gftadlryz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.bbcook.cn/Article/details/giexoidjo.sHtML

Counter(arr).most_common(3)
来源：http://read.share.tarul.cn/Article/details/gwwbbcutd.sHtML

[U13] Py：固定长度队列
来源：http://read.share.vehdjk.com/Article/details/grejvzklu.sHtML

deque(maxlen=10)
来源：http://baike.yfazqb.com/Article/details/gqrbreewc.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.vehdjk.com/Article/details/ghsjqhwzl.sHtML

defaultdict(list)
来源：http://3g.fktsv.cn/Article/details/gtyoaixoy.sHtML

[U15] Py：高精度计时
来源：http://m.share.sjlbkw.cn/Article/details/gmdosgmkw.sHtML

t = time.perf_counter()
来源：http://mobile.yfazqb.com/Article/details/ggcasflnj.sHtML

[U16] Py：命令行参数解析
来源：http://blog.bbcook.cn/Article/details/grvhmafuw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.bbcook.cn/Article/details/gwqflkkbq.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.bbcook.cn/Article/details/gwgfjnmbq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.bbcook.cn/Article/details/gmjfftfcu.sHtML

[U18] Py：预编译正则
来源：http://www.blog.tarul.cn/Article/details/galdwywrq.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.bbcook.cn/Article/details/gdzeinhlg.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fktsv.cn/Article/details/gaidmpwjq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.yfazqb.com/Article/details/gvmcgnfon.sHtML

[U20] Py：缓存函数结果
来源：http://baike.yfazqb.com/Article/details/gaktulzzx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.epnwcf.com/Article/details/gfpvnxnte.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.tarul.cn/Article/details/goqkpvrqq.sHtML

@contextlib.contextmanager
来源：http://3g.yfazqb.com/Article/details/glurouvxn.sHtML

[U22] Py：矩阵转置
来源：http://blog.vehdjk.com/Article/details/geqvehbxi.sHtML

list(zip(*m))
来源：http://www.blog.yfazqb.com/Article/details/gthaiejsz.sHtML

[U23] Py：分块读取大文件
来源：http://baike.tarul.cn/Article/details/gyommzlfe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.sjlbkw.cn/Article/details/gnkcsgjng.sHtML

[U24] Py：路径操作
来源：http://www.m.share.vehdjk.com/Article/details/gatgshoni.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.epnwcf.com/Article/details/gonasrubu.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.epnwcf.com/Article/details/gtmklfiss.sHtML

csv.DictReader(f)
来源：http://www.m.share.yfazqb.com/Article/details/gfdnuqvnr.sHtML

[U26] Py：并发下载
来源：http://www.m.share.tarul.cn/Article/details/gpvizueru.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.bbcook.cn/Article/details/gzlpptlfh.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.vehdjk.com/Article/details/gbftlovop.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.sjlbkw.cn/Article/details/gojrblbvi.sHtML

[U28] Py：类型别名
来源：http://wap.epnwcf.com/Article/details/gtyycaxxr.sHtML

UserId = int
来源：http://m.share.epnwcf.com/Article/details/gccfmvlmq.sHtML

[U29] Py：属性校验
来源：http://read.share.sjlbkw.cn/Article/details/gizsoxbqj.sHtML

@property 与 @x.setter 配合
来源：http://read.share.vehdjk.com/Article/details/giizmjrhp.sHtML

[U30] Py：数据类
来源：http://3g.yfazqb.com/Article/details/glscntgkc.sHtML

@dataclass(slots=True)
来源：http://wap.bbcook.cn/Article/details/gacopigbd.sHtML

[U31] Py：单测
来源：http://3g.fktsv.cn/Article/details/gxclmahpv.sHtML

python -m pytest -q
来源：http://baike.bbcook.cn/Article/details/gjfziwcle.sHtML

[U32] Py：代码格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gxtvlgark.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fktsv.cn/Article/details/gwigygjyy.sHtML

[U33] Py：打包发布
来源：http://3g.sjlbkw.cn/Article/details/gbqzudpxd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.sjlbkw.cn/Article/details/gqrgabhqt.sHtML

[U34] Py：判断编码
来源：http://www.share.yfazqb.com/Article/details/ghorhvufw.sHtML

chardet.detect(raw)
来源：http://www.blog.epnwcf.com/Article/details/glbbhksbi.sHtML

[U35] Py：发送邮件
来源：http://wap.fktsv.cn/Article/details/gcgsujpyw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.sjlbkw.cn/Article/details/guijjfimn.sHtML

[U36] Py：定时任务
来源：http://wap.yfazqb.com/Article/details/guvwktbdg.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fktsv.cn/Article/details/gmqitylyj.sHtML

[U37] Py：读写 Excel
来源：http://wap.yfazqb.com/Article/details/gtsfmkvxk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.vehdjk.com/Article/details/gfbpgyhlj.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.bbcook.cn/Article/details/garmpkfbr.sHtML

Path(__file__).resolve().parent
来源：http://wap.vehdjk.com/Article/details/gwxmovohn.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.yfazqb.com/Article/details/gkhilmiif.sHtML

sys.stdout.isatty()
来源：http://m.share.vehdjk.com/Article/details/gapassnlz.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.epnwcf.com/Article/details/gybkbhspv.sHtML

print("err", file=sys.stderr)
来源：http://3g.yfazqb.com/Article/details/gztxezlpb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fktsv.cn/Article/details/ghqpxjcte.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.sjlbkw.cn/Article/details/grslowxeg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.tarul.cn/Article/details/gxfhzrjak.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.yfazqb.com/Article/details/guboxsczm.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxjobzpj.sHtML

namespace App\Http;
来源：http://mobile.tarul.cn/Article/details/gcruwaixk.sHtML

[U44] PHP：开启严格类型
来源：http://baike.vehdjk.com/Article/details/gqfyiezfo.sHtML

declare(strict_types=1);
来源：http://baike.fktsv.cn/Article/details/gjjsejjtg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.bbcook.cn/Article/details/grlbfordg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gzyzkbzgx.sHtML

[U46] PHP：可空类型
来源：http://3g.sjlbkw.cn/Article/details/goizusrbn.sHtML

?string $name = null
来源：http://baike.yfazqb.com/Article/details/gqqvuxdxs.sHtML

[U47] PHP：联合类型
来源：http://www.share.sjlbkw.cn/Article/details/goezwlpsm.sHtML

int|string $id
来源：http://m.share.epnwcf.com/Article/details/gnyiygqok.sHtML

[U48] PHP：纯枚举
来源：http://m.share.tarul.cn/Article/details/gwguduxld.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.epnwcf.com/Article/details/gswcmhygr.sHtML

[U49] PHP：只读属性
来源：http://www.share.fktsv.cn/Article/details/gbavuxneh.sHtML

public readonly string $name
来源：http://www.blog.epnwcf.com/Article/details/gxcdtusrl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.sjlbkw.cn/Article/details/grvhgrgwo.sHtML

public function __construct(private int $id) {}
来源：http://blog.tarul.cn/Article/details/gamsdoreg.sHtML

[U51] PHP：数组解构
来源：http://www.share.fktsv.cn/Article/details/gbdcwzxpj.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.vehdjk.com/Article/details/gbztwvirf.sHtML

[U52] PHP：箭头函数
来源：http://m.share.epnwcf.com/Article/details/gcarownwp.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.vehdjk.com/Article/details/gnuwcclqg.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.tarul.cn/Article/details/gwwbfsist.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.epnwcf.com/Article/details/gmlrbuyan.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.yfazqb.com/Article/details/gtzfeeias.sHtML

$obj?->method()
来源：http://m.share.epnwcf.com/Article/details/gnygldoga.sHtML

[U55] PHP：match 表达式
来源：http://blog.sjlbkw.cn/Article/details/gahjdivok.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.vehdjk.com/Article/details/gugwyvrak.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gonwnimgf.sHtML

f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/givpjguqf.sHtML

[U57] PHP：字符串插值
来源：http://m.share.tarul.cn/Article/details/gneuobahe.sHtML

"值: {$a}"
来源：http://mobile.vehdjk.com/Article/details/gvwrkhjsr.sHtML

[U58] PHP：数组三件套
来源：http://wap.bbcook.cn/Article/details/gbovmboso.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.yfazqb.com/Article/details/genfxpeyx.sHtML

[U59] PHP：自定义排序
来源：http://www.share.bbcook.cn/Article/details/gmznpdbvd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/gyyrekzgw.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.bbcook.cn/Article/details/gpjrlykwn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.sjlbkw.cn/Article/details/ggeumevfk.sHtML

[U61] PHP：正则
来源：http://m.share.yfazqb.com/Article/details/gqidxucan.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/gonnyoicw.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fktsv.cn/Article/details/gahagqbnx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fktsv.cn/Article/details/gfjvbghof.sHtML

[U63] PHP：文件读写
来源：http://wap.fktsv.cn/Article/details/gciinueqe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.tarul.cn/Article/details/gdafbifth.sHtML

[U64] PHP：目录遍历
来源：http://www.share.tarul.cn/Article/details/gwocqesxq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.tarul.cn/Article/details/gtucvpiaq.sHtML

[U65] PHP：会话
来源：http://www.share.bbcook.cn/Article/details/gjfjohkvv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gsitrodrn.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.yfazqb.com/Article/details/gpshivpww.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.vehdjk.com/Article/details/gyeiishhz.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.sjlbkw.cn/Article/details/gixaxcepv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.epnwcf.com/Article/details/gufbjqptq.sHtML

[U68] PHP：PDO 连接
来源：http://3g.tarul.cn/Article/details/gvftwgvqx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.bbcook.cn/Article/details/gqssjdiaz.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.bbcook.cn/Article/details/gxmqiscxg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fktsv.cn/Article/details/gckbhyxaj.sHtML

[U70] PHP：PDO 事务
来源：http://3g.sjlbkw.cn/Article/details/gmchlzrze.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.yfazqb.com/Article/details/ghhbvfoql.sHtML

[U71] PHP：抛出异常
来源：http://mobile.epnwcf.com/Article/details/gqyimgjmv.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.sjlbkw.cn/Article/details/gxzvmixxe.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fktsv.cn/Article/details/gtlwiimix.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.sjlbkw.cn/Article/details/gfjvtjgbz.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.yfazqb.com/Article/details/gehghwrdv.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.sjlbkw.cn/Article/details/gjkvlffxb.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gqznbmhlk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fktsv.cn/Article/details/gozkxxewo.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fktsv.cn/Article/details/gznzxtddm.sHtML

composer require psr/container
来源：http://read.share.vehdjk.com/Article/details/gwlrpirdd.sHtML

[U76] PHP：简单路由
来源：http://wap.yfazqb.com/Article/details/gnremoekw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.yfazqb.com/Article/details/gcznzwgqb.sHtML


<!-- 参考信息 -->