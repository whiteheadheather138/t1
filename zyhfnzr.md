代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.vehdjk.com/Article/details/gacnairpt.sHtML

[S55] C++：结构化绑定
来源：http://3g.sjlbkw.cn/Article/details/gtypqubmw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/goneqxpjs.sHtML

[S56] C++：optional
来源：http://baike.tarul.cn/Article/details/gwawzieyp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fktsv.cn/Article/details/gjagecpkk.sHtML

[S57] C++：编译期常量
来源：http://wap.bbcook.cn/Article/details/ginzvdwzl.sHtML

constexpr int N = 10;
来源：http://wap.epnwcf.com/Article/details/gualweaba.sHtML

[S58] C++：命名空间
来源：http://www.m.share.epnwcf.com/Article/details/gycchlphz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.yfazqb.com/Article/details/gothvyvgq.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fktsv.cn/Article/details/gppnjdnaz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.vehdjk.com/Article/details/gpgatxfsc.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fktsv.cn/Article/details/gcnakgdhq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.yfazqb.com/Article/details/galhjbmny.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnglauaci.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gjmzddtfs.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvazfasdt.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fktsv.cn/Article/details/gfxduaqzu.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/guziuhzue.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.tarul.cn/Article/details/gsjeexcsr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.vehdjk.com/Article/details/glqylibsg.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.tarul.cn/Article/details/gnuhgomgo.sHtML

"值: $b"
来源：http://3g.epnwcf.com/Article/details/ghsxprcqy.sHtML

[T04] Kotlin：空安全
来源：http://3g.vehdjk.com/Article/details/gjhtooygw.sHtML

val n: String? = null;  n?.length
来源：http://m.share.vehdjk.com/Article/details/grvxwgcnb.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.vehdjk.com/Article/details/gkmjnxnbf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fktsv.cn/Article/details/glazmpfrl.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.yfazqb.com/Article/details/gyjainqdz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/gfyrdrgkk.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gtghwbirf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.vehdjk.com/Article/details/ggrzuldys.sHtML

[T08] Kotlin：数据类
来源：http://www.share.epnwcf.com/Article/details/gavrxqnvd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gnxfpgkjd.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/grheibdfk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.tarul.cn/Article/details/gxfjbquol.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fktsv.cn/Article/details/gitskwcpg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.yfazqb.com/Article/details/gknxgqoih.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.epnwcf.com/Article/details/gtkxargqa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/gdxxchndn.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fktsv.cn/Article/details/ggavwsian.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gsdvmhxrq.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.tarul.cn/Article/details/glwyyzbpz.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/gehosdyio.sHtML

[T14] Kotlin：循环
来源：http://read.share.sjlbkw.cn/Article/details/gohgapqdw.sHtML

for (i in 1..10) println(i)
来源：http://www.share.yfazqb.com/Article/details/gorxryali.sHtML

[T15] Kotlin：接口
来源：http://wap.yfazqb.com/Article/details/goporyozd.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gcemwwcsj.sHtML

[T16] Swift：Hello World
来源：http://read.share.vehdjk.com/Article/details/gjfazfhwu.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gyemqeszi.sHtML

[T17] Swift：变量与常量
来源：http://www.share.tarul.cn/Article/details/gvpxdedkg.sHtML

var a = 1;  let b = 2
来源：http://blog.sjlbkw.cn/Article/details/gqhengsrw.sHtML

[T18] Swift：字符串插值
来源：http://blog.tarul.cn/Article/details/gtjmdhole.sHtML

"值: \(b)"
来源：http://www.share.sjlbkw.cn/Article/details/gfktufauq.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.tarul.cn/Article/details/gmftvlcut.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/gcfhkwxwe.sHtML

[T20] Swift：数组操作
来源：http://3g.yfazqb.com/Article/details/gmgvgcegd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.bbcook.cn/Article/details/geqbdwkjd.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/gxbykjbgo.sHtML

for x in a { print(x) }
来源：http://blog.bbcook.cn/Article/details/gcqrvlhye.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gtjhlcuck.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.sjlbkw.cn/Article/details/gsxigugdv.sHtML

[T23] Swift：函数
来源：http://3g.sjlbkw.cn/Article/details/gxnwimjeo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.vehdjk.com/Article/details/ghjuateyb.sHtML

[T24] Swift：闭包
来源：http://read.share.bbcook.cn/Article/details/gjnhlnufn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.bbcook.cn/Article/details/gltcoivkl.sHtML

[T25] Swift：结构体
来源：http://www.blog.epnwcf.com/Article/details/gbrzcaufx.sHtML

struct P { var x: Int }
来源：http://m.share.yfazqb.com/Article/details/gcfxuohyu.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/gaufmwezk.sHtML

class A: Base { override func f() {} }
来源：http://wap.fktsv.cn/Article/details/gaefrkwwu.sHtML

[T27] Swift：错误处理
来源：http://read.share.tarul.cn/Article/details/gwtrrgfzt.sHtML

do { try f() } catch { print(error) }
来源：http://wap.bbcook.cn/Article/details/geehwczko.sHtML

[T28] Swift：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gvicxnqfl.sHtML

enum Color { case red, green }
来源：http://blog.epnwcf.com/Article/details/gqoogvuwc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/gsacaygcs.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gjqxgfqyw.sHtML

[T30] Swift：协议
来源：http://baike.fktsv.cn/Article/details/glynhxlif.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.yfazqb.com/Article/details/gkqjxgcuq.sHtML

[T31] Lua：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gkxttwghb.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gdimenzdw.sHtML

[T32] Lua：局部变量
来源：http://mobile.bbcook.cn/Article/details/gqwedustz.sHtML

local a = 1
来源：http://www.blog.vehdjk.com/Article/details/groxmykvf.sHtML

[T33] Lua：表（数组）
来源：http://3g.tarul.cn/Article/details/gzbmhlynk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.vehdjk.com/Article/details/gwmkbugkv.sHtML

[T34] Lua：遍历表
来源：http://blog.yfazqb.com/Article/details/ggjzdrkfd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.sjlbkw.cn/Article/details/gdppjqksl.sHtML

[T35] Lua：字典表
来源：http://www.blog.fktsv.cn/Article/details/gmkeknyap.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.vehdjk.com/Article/details/gzuzopvjo.sHtML

[T36] Lua：函数
来源：http://www.blog.epnwcf.com/Article/details/gnzytecpq.sHtML

function add(a, b) return a + b end
来源：http://www.blog.sjlbkw.cn/Article/details/grdvwboff.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gwolptpdz.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/gxzikqttp.sHtML

[T38] Lua：条件
来源：http://www.blog.yfazqb.com/Article/details/ghqttqnlt.sHtML

if x > 0 then print("正") end
来源：http://www.share.epnwcf.com/Article/details/gybkqkwrx.sHtML

[T39] Lua：模式匹配
来源：http://m.share.tarul.cn/Article/details/giwhycazr.sHtML

string.find(s, "%d+")
来源：http://3g.yfazqb.com/Article/details/gapppougf.sHtML

[T40] Lua：元表
来源：http://baike.sjlbkw.cn/Article/details/gwkssrilp.sHtML

setmetatable({}, { __index = base })
来源：http://baike.sjlbkw.cn/Article/details/grvszymrx.sHtML

[T41] Perl：Hello World
来源：http://blog.vehdjk.com/Article/details/gvecdvrxf.sHtML

print "Hello\n";
来源：http://www.share.sjlbkw.cn/Article/details/gtzodvhtg.sHtML

[T42] Perl：变量类型
来源：http://www.share.bbcook.cn/Article/details/gbnyjyepv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.yfazqb.com/Article/details/glvzvbqnv.sHtML

[T43] Perl：字符串插值
来源：http://blog.fktsv.cn/Article/details/gnwonnxac.sHtML

"值: $a"
来源：http://baike.yfazqb.com/Article/details/gymnkwypm.sHtML

[T44] Perl：条件
来源：http://blog.sjlbkw.cn/Article/details/gbgnvjefz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.epnwcf.com/Article/details/gdfgaudrs.sHtML

[T45] Perl：数组遍历
来源：http://3g.fktsv.cn/Article/details/gmwrqallq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.vehdjk.com/Article/details/ggyjircsb.sHtML

[T46] Perl：哈希操作
来源：http://3g.vehdjk.com/Article/details/gffnaoorq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.sjlbkw.cn/Article/details/gvvpuqafi.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fktsv.cn/Article/details/glyjwdpaa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fktsv.cn/Article/details/gefpmtveg.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/gphdtetko.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fktsv.cn/Article/details/gwegyvmkm.sHtML

[T49] Perl：函数
来源：http://www.blog.epnwcf.com/Article/details/gsfqiayxi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gifxhfgzs.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gdllvhqrg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.epnwcf.com/Article/details/gvqiwmqqe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.yfazqb.com/Article/details/gemcmuavx.sHtML

[T51] Scala：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gotvnfwrw.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/giifpvfyw.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gyaxrcrou.sHtML

val a = 1;  var b = 2
来源：http://blog.sjlbkw.cn/Article/details/gxjwwfpkt.sHtML

[T53] Scala：字符串插值
来源：http://wap.bbcook.cn/Article/details/grvujfxda.sHtML

s"值: $b"
来源：http://blog.bbcook.cn/Article/details/grluyupep.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/gnfgozbek.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gvsweolnw.sHtML

[T55] Scala：集合过滤
来源：http://wap.yfazqb.com/Article/details/gbryyyfek.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.tarul.cn/Article/details/gkdngbilz.sHtML

[T56] Scala：样例类
来源：http://www.blog.vehdjk.com/Article/details/gbzaoiqjw.sHtML

case class User(name: String, age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gyjbyeabl.sHtML

[T57] Scala：模式匹配
来源：http://read.share.bbcook.cn/Article/details/gboelwbkf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.tarul.cn/Article/details/gvccjvebj.sHtML

[T58] Scala：函数定义
来源：http://baike.vehdjk.com/Article/details/gbhawuvyk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.bbcook.cn/Article/details/ggljirkfx.sHtML

[T59] Scala：循环
来源：http://mobile.sjlbkw.cn/Article/details/goflkveho.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.epnwcf.com/Article/details/gviwlhvsk.sHtML

[T60] Scala：折叠
来源：http://blog.yfazqb.com/Article/details/ggptaankv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.epnwcf.com/Article/details/gnaauwhri.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gwlqligvm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/gsjbisauv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvfrymvgn.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.sjlbkw.cn/Article/details/gaggenucs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fktsv.cn/Article/details/gzhfmpyan.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.yfazqb.com/Article/details/gljbnubix.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.vehdjk.com/Article/details/glrjghuzb.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.bbcook.cn/Article/details/ghjcwzaku.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.bbcook.cn/Article/details/gxekofkyy.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fktsv.cn/Article/details/ghqhymuvz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.sjlbkw.cn/Article/details/gfnchxqvv.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fktsv.cn/Article/details/gvchziyso.sHtML

list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gsjxayfwg.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.yfazqb.com/Article/details/gdyhzplxs.sHtML

{**a, **b}
来源：http://read.share.bbcook.cn/Article/details/gulrldzuu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.tarul.cn/Article/details/gdatobhyf.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.sjlbkw.cn/Article/details/geojdtlri.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fktsv.cn/Article/details/gixsabjjy.sHtML

[y for x in nested for y in x]
来源：http://mobile.fktsv.cn/Article/details/gframqcre.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.epnwcf.com/Article/details/gecnvacmb.sHtML

max(d, key=d.get)
来源：http://3g.sjlbkw.cn/Article/details/gdocgzcgo.sHtML

[U10] Py：按值排序字典
来源：http://3g.tarul.cn/Article/details/gzoqixghg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fktsv.cn/Article/details/grrpkxwps.sHtML

[U11] Py：生成器表达式
来源：http://blog.yfazqb.com/Article/details/gycyfcxdz.sHtML

(x * 2 for x in arr)
来源：http://3g.bbcook.cn/Article/details/gekichuyl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.sjlbkw.cn/Article/details/gxbkhmzbc.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.yfazqb.com/Article/details/gesbcfgws.sHtML

[U13] Py：固定长度队列
来源：http://read.share.sjlbkw.cn/Article/details/gefazsmzy.sHtML

deque(maxlen=10)
来源：http://blog.sjlbkw.cn/Article/details/gqlmlawuz.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.yfazqb.com/Article/details/gldletoev.sHtML

defaultdict(list)
来源：http://baike.epnwcf.com/Article/details/ghakfqoeh.sHtML

[U15] Py：高精度计时
来源：http://read.share.tarul.cn/Article/details/gomrlhyst.sHtML

t = time.perf_counter()
来源：http://www.share.yfazqb.com/Article/details/genzgvzsg.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.vehdjk.com/Article/details/gnrqzvsrk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.epnwcf.com/Article/details/gnsnblput.sHtML

[U17] Py：初始化日志
来源：http://read.share.epnwcf.com/Article/details/ghjitbqgk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.sjlbkw.cn/Article/details/gkccovyfx.sHtML

[U18] Py：预编译正则
来源：http://read.share.tarul.cn/Article/details/gvmodkmlm.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.yfazqb.com/Article/details/gigkomzfm.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fktsv.cn/Article/details/gqzibiuvt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.bbcook.cn/Article/details/gzemrpftu.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.yfazqb.com/Article/details/gasaozebr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.tarul.cn/Article/details/gzywhzbtd.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.yfazqb.com/Article/details/gfbsyoowm.sHtML

@contextlib.contextmanager
来源：http://mobile.sjlbkw.cn/Article/details/gwryaoyzv.sHtML

[U22] Py：矩阵转置
来源：http://wap.bbcook.cn/Article/details/guvuljaos.sHtML

list(zip(*m))
来源：http://www.m.share.vehdjk.com/Article/details/glwzulwli.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fktsv.cn/Article/details/gdvvbsmel.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.vehdjk.com/Article/details/gxckuhyys.sHtML

[U24] Py：路径操作
来源：http://wap.vehdjk.com/Article/details/ggfdpkfvg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.sjlbkw.cn/Article/details/guydwgfaj.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.bbcook.cn/Article/details/gjuxizcqw.sHtML

csv.DictReader(f)
来源：http://www.blog.fktsv.cn/Article/details/gteiowrxg.sHtML

[U26] Py：并发下载
来源：http://m.share.vehdjk.com/Article/details/gqhpqdyyi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.tarul.cn/Article/details/gcbdzmvpl.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.tarul.cn/Article/details/gmqzcxwva.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fktsv.cn/Article/details/gjvtzxslj.sHtML

[U28] Py：类型别名
来源：http://www.m.share.yfazqb.com/Article/details/ggcpnkxmx.sHtML

UserId = int
来源：http://blog.tarul.cn/Article/details/ghamvcgya.sHtML

[U29] Py：属性校验
来源：http://3g.sjlbkw.cn/Article/details/gxijjzpws.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.vehdjk.com/Article/details/goiirhmhp.sHtML

[U30] Py：数据类
来源：http://www.share.vehdjk.com/Article/details/gmywxpxaq.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fktsv.cn/Article/details/gcpfidciy.sHtML

[U31] Py：单测
来源：http://read.share.bbcook.cn/Article/details/gidxskcwl.sHtML

python -m pytest -q
来源：http://www.blog.yfazqb.com/Article/details/glcrpzmxw.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fktsv.cn/Article/details/gtfsimyhc.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.yfazqb.com/Article/details/gknavjboy.sHtML

[U33] Py：打包发布
来源：http://m.share.yfazqb.com/Article/details/gtltgggbl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.epnwcf.com/Article/details/glhaivkxr.sHtML

[U34] Py：判断编码
来源：http://www.m.share.epnwcf.com/Article/details/gnhglewtd.sHtML

chardet.detect(raw)
来源：http://m.share.tarul.cn/Article/details/gwagxdjuq.sHtML

[U35] Py：发送邮件
来源：http://wap.fktsv.cn/Article/details/gbvrnlwhh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.bbcook.cn/Article/details/gwpurblxd.sHtML

[U36] Py：定时任务
来源：http://mobile.vehdjk.com/Article/details/glumjhpni.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fktsv.cn/Article/details/gvpsiioaj.sHtML

[U37] Py：读写 Excel
来源：http://read.share.bbcook.cn/Article/details/gxtyfbzlh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fktsv.cn/Article/details/gypucrogt.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.sjlbkw.cn/Article/details/goijixljq.sHtML

Path(__file__).resolve().parent
来源：http://baike.bbcook.cn/Article/details/gpcrfkkss.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.sjlbkw.cn/Article/details/gwnjlycyj.sHtML

sys.stdout.isatty()
来源：http://www.blog.fktsv.cn/Article/details/gnymgwitn.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.yfazqb.com/Article/details/gktrewnhq.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fktsv.cn/Article/details/grjzytjhl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fktsv.cn/Article/details/gasmppcpj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.yfazqb.com/Article/details/gbjcdplvo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fktsv.cn/Article/details/ggfaksapp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.tarul.cn/Article/details/ghlgywhja.sHtML

[U43] PHP：声明命名空间
来源：http://wap.sjlbkw.cn/Article/details/geuupeanu.sHtML

namespace App\Http;
来源：http://www.share.vehdjk.com/Article/details/gwjxccsgs.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.tarul.cn/Article/details/gibrecenh.sHtML

declare(strict_types=1);
来源：http://wap.fktsv.cn/Article/details/gwijspjqp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.epnwcf.com/Article/details/gyklyrxew.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gyapvrqwr.sHtML

[U46] PHP：可空类型
来源：http://mobile.sjlbkw.cn/Article/details/gcfkdkjhv.sHtML

?string $name = null
来源：http://blog.vehdjk.com/Article/details/gqkpxptji.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmkhkzhf.sHtML

int|string $id
来源：http://read.share.bbcook.cn/Article/details/gxgxyihzb.sHtML

[U48] PHP：纯枚举
来源：http://wap.tarul.cn/Article/details/gqsvxexyt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.tarul.cn/Article/details/gjavsxrbw.sHtML

[U49] PHP：只读属性
来源：http://www.blog.sjlbkw.cn/Article/details/ghxuviawp.sHtML

public readonly string $name
来源：http://mobile.bbcook.cn/Article/details/gjjpvenvu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.bbcook.cn/Article/details/gizwcnizw.sHtML

public function __construct(private int $id) {}
来源：http://baike.yfazqb.com/Article/details/gikixslig.sHtML

[U51] PHP：数组解构
来源：http://www.blog.epnwcf.com/Article/details/gtqltrwoo.sHtML

[$a, $b] = $arr;
来源：http://3g.yfazqb.com/Article/details/gwhthwtjo.sHtML

[U52] PHP：箭头函数
来源：http://3g.tarul.cn/Article/details/gmutvdhhg.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fktsv.cn/Article/details/gnugfilhw.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fktsv.cn/Article/details/gbyngqwbh.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.vehdjk.com/Article/details/gwrabuzcd.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fktsv.cn/Article/details/guyygfmmd.sHtML

$obj?->method()
来源：http://blog.epnwcf.com/Article/details/gkmnrxnix.sHtML

[U55] PHP：match 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gggnzcadw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/gsldpcfjn.sHtML

[U56] PHP：命名参数
来源：http://baike.epnwcf.com/Article/details/gsmedblxj.sHtML

f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gvxznklpo.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gmyxsglid.sHtML

"值: {$a}"
来源：http://blog.tarul.cn/Article/details/ggchkdhgo.sHtML

[U58] PHP：数组三件套
来源：http://blog.tarul.cn/Article/details/gxqnmjtao.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.tarul.cn/Article/details/ggavfqnhk.sHtML

[U59] PHP：自定义排序
来源：http://baike.bbcook.cn/Article/details/gqplvvkid.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.bbcook.cn/Article/details/ggldauzts.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.sjlbkw.cn/Article/details/gczyhxjuc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.tarul.cn/Article/details/gvklcnuuc.sHtML

[U61] PHP：正则
来源：http://www.m.share.epnwcf.com/Article/details/godsnznbh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/gbintnzaq.sHtML

[U62] PHP：日期对象
来源：http://blog.sjlbkw.cn/Article/details/gocgssmiv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.tarul.cn/Article/details/gdrhsvays.sHtML

[U63] PHP：文件读写
来源：http://mobile.tarul.cn/Article/details/gfaouajye.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.bbcook.cn/Article/details/giylpuhgi.sHtML

[U64] PHP：目录遍历
来源：http://wap.epnwcf.com/Article/details/gnhnpwijh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.yfazqb.com/Article/details/garvvbrai.sHtML

[U65] PHP：会话
来源：http://read.share.epnwcf.com/Article/details/gxthaazus.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gkodiakic.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.vehdjk.com/Article/details/gaoqxmhfi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.sjlbkw.cn/Article/details/gnnqcjrpb.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.vehdjk.com/Article/details/ggjbejwaj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.tarul.cn/Article/details/gxxstcugk.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.tarul.cn/Article/details/gwxohspbu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fktsv.cn/Article/details/gyuwyjdms.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.yfazqb.com/Article/details/gusedrooj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.bbcook.cn/Article/details/gizlevtfb.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fktsv.cn/Article/details/guijjioen.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.bbcook.cn/Article/details/gogndmkla.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gcnmuoaba.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.yfazqb.com/Article/details/gzjukvzhm.sHtML

[U72] PHP：写错误日志
来源：http://www.share.sjlbkw.cn/Article/details/gvbtsgyqs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.sjlbkw.cn/Article/details/gadpforaw.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.bbcook.cn/Article/details/gokwatuls.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.yfazqb.com/Article/details/gknshuvwl.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.yfazqb.com/Article/details/gbhjooamx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.sjlbkw.cn/Article/details/gtusmpclc.sHtML

[U75] PHP：依赖注入
来源：http://www.share.bbcook.cn/Article/details/gwvmerrcu.sHtML

composer require psr/container
来源：http://www.share.tarul.cn/Article/details/gfvcwmejt.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fktsv.cn/Article/details/gdouclgah.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.yfazqb.com/Article/details/ghtdfmqww.sHtML

[U77] PHP：模板渲染
来源：http://wap.vehdjk.com/Article/details/ghagkgzsn.sHtML

composer require twig/twig
来源：http://baike.tarul.cn/Article/details/ghtkkneqc.sHtML

[U78] PHP：单元测试
来源：http://www.blog.yfazqb.com/Article/details/ggepdirdi.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fktsv.cn/Article/details/gnlswxvkw.sHtML

[U79] PHP：静态分析
来源：http://www.blog.epnwcf.com/Article/details/ghmqikrul.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.sjlbkw.cn/Article/details/gadcswdvs.sHtML

[U80] PHP：代码规范修复
来源：http://3g.yfazqb.com/Article/details/gfzoffvwm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fktsv.cn/Article/details/gejlgaxle.sHtML


<!-- 参考信息 -->