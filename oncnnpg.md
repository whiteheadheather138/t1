代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.epnwcf.com/Article/details/gmrcuutle.sHtML

[S55] C++：结构化绑定
来源：http://wap.vehdjk.com/Article/details/glgqjcjbc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gbsvxlhqk.sHtML

[S56] C++：optional
来源：http://blog.bbcook.cn/Article/details/gpjjsmaba.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.sjlbkw.cn/Article/details/gowkoorpp.sHtML

[S57] C++：编译期常量
来源：http://www.blog.vehdjk.com/Article/details/goyevigyj.sHtML

constexpr int N = 10;
来源：http://mobile.vehdjk.com/Article/details/ggclrftyr.sHtML

[S58] C++：命名空间
来源：http://www.blog.vehdjk.com/Article/details/gqkdcxgse.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.epnwcf.com/Article/details/gheymqiyo.sHtML

[S59] C++：静态断言
来源：http://read.share.sjlbkw.cn/Article/details/gkpqiwtox.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.epnwcf.com/Article/details/gdmvlueae.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.epnwcf.com/Article/details/gsrekxsrk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.sjlbkw.cn/Article/details/guuhoolcg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzgtgtfvc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/gafiwxgnq.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmtisnbwj.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/gexwvmtin.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/glmrifvif.sHtML

[T02] Kotlin：变量
来源：http://read.share.yfazqb.com/Article/details/ghzejtprp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/goyigkztf.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.vehdjk.com/Article/details/gtxkucbhz.sHtML

"值: $b"
来源：http://wap.vehdjk.com/Article/details/gqaicadrh.sHtML

[T04] Kotlin：空安全
来源：http://read.share.bbcook.cn/Article/details/ggajydnoi.sHtML

val n: String? = null;  n?.length
来源：http://www.share.bbcook.cn/Article/details/gdlltgbpu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.tarul.cn/Article/details/gluqarinw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.epnwcf.com/Article/details/gmervzmcq.sHtML

[T06] Kotlin：集合映射
来源：http://baike.vehdjk.com/Article/details/gvxutbxxn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gwtudqcps.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/gntbvlstl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/glxlwmrrv.sHtML

[T08] Kotlin：数据类
来源：http://3g.tarul.cn/Article/details/ghfotpwte.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.bbcook.cn/Article/details/gpdvonqzy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fktsv.cn/Article/details/gsqvhkckw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/gxehefglt.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fktsv.cn/Article/details/guwxgcgui.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.tarul.cn/Article/details/ganyijres.sHtML

[T11] Kotlin：协程
来源：http://baike.bbcook.cn/Article/details/gzihxvinz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.yfazqb.com/Article/details/gutzjbjsx.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/gacdoayud.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.tarul.cn/Article/details/gjiedvexd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.epnwcf.com/Article/details/gylyzfqgv.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.bbcook.cn/Article/details/gafiekoeh.sHtML

[T14] Kotlin：循环
来源：http://wap.fktsv.cn/Article/details/gzesztcur.sHtML

for (i in 1..10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/gjervrcfj.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/ggwuabhhx.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.sjlbkw.cn/Article/details/gmvhrnigy.sHtML

[T16] Swift：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gtihjhaix.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gsucxsgmc.sHtML

[T17] Swift：变量与常量
来源：http://baike.fktsv.cn/Article/details/gjsoevqhb.sHtML

var a = 1;  let b = 2
来源：http://www.blog.vehdjk.com/Article/details/gtqmlbliy.sHtML

[T18] Swift：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gfcvbwwmq.sHtML

"值: \(b)"
来源：http://wap.yfazqb.com/Article/details/gnnzerxly.sHtML

[T19] Swift：可选绑定
来源：http://blog.vehdjk.com/Article/details/gfkgbcdvz.sHtML

if let n = opt { print(n) }
来源：http://m.share.yfazqb.com/Article/details/gaayjefxu.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/gbwebmwgy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fktsv.cn/Article/details/gfmxjjzkd.sHtML

[T21] Swift：遍历
来源：http://www.blog.fktsv.cn/Article/details/gmssihftc.sHtML

for x in a { print(x) }
来源：http://read.share.vehdjk.com/Article/details/garqangph.sHtML

[T22] Swift：字典
来源：http://blog.yfazqb.com/Article/details/gmvzrrrvk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.tarul.cn/Article/details/gvicmbnnc.sHtML

[T23] Swift：函数
来源：http://baike.bbcook.cn/Article/details/gvyudvggn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fktsv.cn/Article/details/gthssjjhq.sHtML

[T24] Swift：闭包
来源：http://wap.yfazqb.com/Article/details/glfohwykg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.tarul.cn/Article/details/ghdvxcogg.sHtML

[T25] Swift：结构体
来源：http://blog.fktsv.cn/Article/details/gmagmbeky.sHtML

struct P { var x: Int }
来源：http://wap.bbcook.cn/Article/details/gwnojpkwj.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/gzazinrii.sHtML

class A: Base { override func f() {} }
来源：http://m.share.yfazqb.com/Article/details/gmgttzzgf.sHtML

[T27] Swift：错误处理
来源：http://3g.vehdjk.com/Article/details/gfncwfvon.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.sjlbkw.cn/Article/details/girssxrzl.sHtML

[T28] Swift：枚举
来源：http://mobile.bbcook.cn/Article/details/gohimhzyg.sHtML

enum Color { case red, green }
来源：http://baike.bbcook.cn/Article/details/gjoybhhwz.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/grmiucbjm.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/gxdrbgklu.sHtML

[T30] Swift：协议
来源：http://3g.fktsv.cn/Article/details/grtifnbkg.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/gvaqgbqpi.sHtML

[T31] Lua：Hello World
来源：http://mobile.bbcook.cn/Article/details/gaijlpiwb.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/gfihzhyzv.sHtML

[T32] Lua：局部变量
来源：http://m.share.epnwcf.com/Article/details/glprxfjpe.sHtML

local a = 1
来源：http://wap.bbcook.cn/Article/details/gwztzkyym.sHtML

[T33] Lua：表（数组）
来源：http://read.share.bbcook.cn/Article/details/gejjhslku.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.tarul.cn/Article/details/gwytuubgi.sHtML

[T34] Lua：遍历表
来源：http://3g.fktsv.cn/Article/details/gopwavgwz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.sjlbkw.cn/Article/details/gavpjbfsw.sHtML

[T35] Lua：字典表
来源：http://www.share.sjlbkw.cn/Article/details/gkwjxgdmr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fktsv.cn/Article/details/gfksiuwla.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/ghuwioegg.sHtML

function add(a, b) return a + b end
来源：http://wap.fktsv.cn/Article/details/gcszdhejv.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.tarul.cn/Article/details/gmcsjvcpk.sHtML

"a" .. "b"
来源：http://blog.yfazqb.com/Article/details/gszzdqgox.sHtML

[T38] Lua：条件
来源：http://blog.epnwcf.com/Article/details/gwoxoorzp.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fktsv.cn/Article/details/gstcpupdc.sHtML

[T39] Lua：模式匹配
来源：http://wap.vehdjk.com/Article/details/gcuzalikv.sHtML

string.find(s, "%d+")
来源：http://www.share.sjlbkw.cn/Article/details/gdviuvsqt.sHtML

[T40] Lua：元表
来源：http://blog.vehdjk.com/Article/details/gxgmbkinq.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.epnwcf.com/Article/details/gkrudkkxx.sHtML

[T41] Perl：Hello World
来源：http://baike.bbcook.cn/Article/details/gxxpctjod.sHtML

print "Hello\n";
来源：http://www.blog.sjlbkw.cn/Article/details/gbscibbiz.sHtML

[T42] Perl：变量类型
来源：http://blog.epnwcf.com/Article/details/grqmugczl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fktsv.cn/Article/details/giflbgbue.sHtML

[T43] Perl：字符串插值
来源：http://baike.epnwcf.com/Article/details/gsnhpvgfd.sHtML

"值: $a"
来源：http://www.blog.epnwcf.com/Article/details/gtnvyfcpe.sHtML

[T44] Perl：条件
来源：http://blog.bbcook.cn/Article/details/gusjizybf.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fktsv.cn/Article/details/gkswdbpvg.sHtML

[T45] Perl：数组遍历
来源：http://wap.vehdjk.com/Article/details/goeyqjlrx.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.bbcook.cn/Article/details/gdlqejyho.sHtML

[T46] Perl：哈希操作
来源：http://baike.fktsv.cn/Article/details/gugtcmgsf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/ggiawvprm.sHtML

[T47] Perl：正则捕获
来源：http://www.share.tarul.cn/Article/details/gcklzhzpz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.vehdjk.com/Article/details/gheypeffm.sHtML

[T48] Perl：正则替换
来源：http://mobile.yfazqb.com/Article/details/gsplbdryg.sHtML

$s =~ s/old/new/g;
来源：http://3g.fktsv.cn/Article/details/gebcgaijy.sHtML

[T49] Perl：函数
来源：http://mobile.fktsv.cn/Article/details/gcuoxercs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gipnhvdvb.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gywahcxou.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fktsv.cn/Article/details/giaryxprx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.epnwcf.com/Article/details/gdcenzdhd.sHtML

[T51] Scala：Hello World
来源：http://mobile.epnwcf.com/Article/details/ggwmmveue.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/ggtiinohw.sHtML

[T52] Scala：变量
来源：http://mobile.sjlbkw.cn/Article/details/gstvybofb.sHtML

val a = 1;  var b = 2
来源：http://www.share.vehdjk.com/Article/details/ghvbguuxk.sHtML

[T53] Scala：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gkwqitafx.sHtML

s"值: $b"
来源：http://wap.bbcook.cn/Article/details/gyksgwcbs.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/grwyougjd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.yfazqb.com/Article/details/gxgsmuhuq.sHtML

[T55] Scala：集合过滤
来源：http://3g.fktsv.cn/Article/details/gramzqcwb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fktsv.cn/Article/details/gvcenwzsb.sHtML

[T56] Scala：样例类
来源：http://wap.vehdjk.com/Article/details/gqvwfnqxl.sHtML

case class User(name: String, age: Int)
来源：http://3g.yfazqb.com/Article/details/gigobfydm.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/gmvrtgtqr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gipklauyi.sHtML

[T58] Scala：函数定义
来源：http://3g.yfazqb.com/Article/details/ghytbyxam.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.tarul.cn/Article/details/gtwajixqs.sHtML

[T59] Scala：循环
来源：http://www.m.share.epnwcf.com/Article/details/gbssgbsle.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/grjjmiqap.sHtML

[T60] Scala：折叠
来源：http://blog.tarul.cn/Article/details/gjplacibn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.vehdjk.com/Article/details/gfrcndrso.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gestgljxk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.tarul.cn/Article/details/gnakvyzhu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/geojpwbri.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/gmmsdcirn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gjcgynobg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fktsv.cn/Article/details/gutxorhjn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.tarul.cn/Article/details/gipczpcod.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.yfazqb.com/Article/details/ghzsiopcg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.sjlbkw.cn/Article/details/guslbriva.sHtML

[U04] Py：变量调试打印
来源：http://wap.sjlbkw.cn/Article/details/gqpwoifqt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fktsv.cn/Article/details/gplvgfpow.sHtML

[U05] Py：列表去重且保序
来源：http://wap.bbcook.cn/Article/details/gsgtdikee.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gbbznxdko.sHtML

[U06] Py：合并两个字典
来源：http://wap.vehdjk.com/Article/details/geztxpcmg.sHtML

{**a, **b}
来源：http://blog.yfazqb.com/Article/details/geqxojnfm.sHtML

[U07] Py：反转字典键值
来源：http://www.share.yfazqb.com/Article/details/gdzjatbvn.sHtML

{v: k for k, v in d.items()}
来源：http://wap.vehdjk.com/Article/details/gpqylftpe.sHtML

[U08] Py：展平二维列表
来源：http://blog.epnwcf.com/Article/details/gxjtfugxr.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.epnwcf.com/Article/details/gwqhrifux.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fktsv.cn/Article/details/gwqmgxuwm.sHtML

max(d, key=d.get)
来源：http://3g.yfazqb.com/Article/details/gpnrbxeem.sHtML

[U10] Py：按值排序字典
来源：http://wap.tarul.cn/Article/details/gwxuldoqh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fktsv.cn/Article/details/goacerdqi.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.bbcook.cn/Article/details/gqewxfskj.sHtML

(x * 2 for x in arr)
来源：http://blog.sjlbkw.cn/Article/details/godudkkla.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.bbcook.cn/Article/details/gtkxkrgep.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.sjlbkw.cn/Article/details/guwtvnsof.sHtML

[U13] Py：固定长度队列
来源：http://mobile.epnwcf.com/Article/details/gluplhype.sHtML

deque(maxlen=10)
来源：http://m.share.sjlbkw.cn/Article/details/gdsjicqmy.sHtML

[U14] Py：分组收集到列表
来源：http://wap.yfazqb.com/Article/details/gouaushku.sHtML

defaultdict(list)
来源：http://wap.tarul.cn/Article/details/grrtfowov.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfhqoumu.sHtML

t = time.perf_counter()
来源：http://wap.tarul.cn/Article/details/ggmzhawkb.sHtML

[U16] Py：命令行参数解析
来源：http://baike.epnwcf.com/Article/details/gvviyzvmg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.vehdjk.com/Article/details/gjxvzrlry.sHtML

[U17] Py：初始化日志
来源：http://mobile.tarul.cn/Article/details/gtwmmswly.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fktsv.cn/Article/details/grwjbikds.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/gpjkttfcw.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gwbiajggk.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.bbcook.cn/Article/details/gelptddaw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fktsv.cn/Article/details/gqotskgun.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.bbcook.cn/Article/details/gyiolsacb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.epnwcf.com/Article/details/gkwgnkyos.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fktsv.cn/Article/details/gdkbdqvxn.sHtML

@contextlib.contextmanager
来源：http://blog.fktsv.cn/Article/details/gldhxyecj.sHtML

[U22] Py：矩阵转置
来源：http://3g.yfazqb.com/Article/details/giutjqhoz.sHtML

list(zip(*m))
来源：http://www.m.share.tarul.cn/Article/details/grckackrp.sHtML

[U23] Py：分块读取大文件
来源：http://3g.bbcook.cn/Article/details/gwaybwuzb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fktsv.cn/Article/details/gsrorbxql.sHtML

[U24] Py：路径操作
来源：http://www.share.yfazqb.com/Article/details/gibmwxqer.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gdfsarjab.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.tarul.cn/Article/details/gqnczwpme.sHtML

csv.DictReader(f)
来源：http://read.share.vehdjk.com/Article/details/gtfszgnix.sHtML

[U26] Py：并发下载
来源：http://wap.epnwcf.com/Article/details/gkvlyiphi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.vehdjk.com/Article/details/gbwdpnysm.sHtML

[U27] Py：异步 HTTP
来源：http://baike.tarul.cn/Article/details/gmgfubjhi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.bbcook.cn/Article/details/gjhvgvhcs.sHtML

[U28] Py：类型别名
来源：http://read.share.tarul.cn/Article/details/glwjqgzhz.sHtML

UserId = int
来源：http://www.m.share.epnwcf.com/Article/details/gplryendp.sHtML

[U29] Py：属性校验
来源：http://blog.epnwcf.com/Article/details/geopkmbki.sHtML

@property 与 @x.setter 配合
来源：http://baike.vehdjk.com/Article/details/gbdeegqzn.sHtML

[U30] Py：数据类
来源：http://m.share.tarul.cn/Article/details/guefmoiak.sHtML

@dataclass(slots=True)
来源：http://read.share.epnwcf.com/Article/details/goayzgqos.sHtML

[U31] Py：单测
来源：http://m.share.sjlbkw.cn/Article/details/gtohktujj.sHtML

python -m pytest -q
来源：http://mobile.vehdjk.com/Article/details/gxaqyhlmh.sHtML

[U32] Py：代码格式化
来源：http://read.share.sjlbkw.cn/Article/details/gmcvjmbkp.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.yfazqb.com/Article/details/gkvqnbczp.sHtML

[U33] Py：打包发布
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdxpctas.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.epnwcf.com/Article/details/gozkhaicu.sHtML

[U34] Py：判断编码
来源：http://read.share.sjlbkw.cn/Article/details/gpesczlzf.sHtML

chardet.detect(raw)
来源：http://read.share.bbcook.cn/Article/details/gvlrbfugs.sHtML

[U35] Py：发送邮件
来源：http://read.share.sjlbkw.cn/Article/details/gokjtzsjf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.tarul.cn/Article/details/ghgswbqfh.sHtML

[U36] Py：定时任务
来源：http://blog.epnwcf.com/Article/details/gsewerypb.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.yfazqb.com/Article/details/goricndjd.sHtML

[U37] Py：读写 Excel
来源：http://baike.fktsv.cn/Article/details/gpyxjbxrc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.yfazqb.com/Article/details/gqcojpcxr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.tarul.cn/Article/details/gydweeucz.sHtML

Path(__file__).resolve().parent
来源：http://baike.sjlbkw.cn/Article/details/gkfymrohq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.sjlbkw.cn/Article/details/gvrqwiiim.sHtML

sys.stdout.isatty()
来源：http://wap.epnwcf.com/Article/details/gpfpksmwc.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.sjlbkw.cn/Article/details/gxvpbqhcb.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/gvhvvzkos.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.sjlbkw.cn/Article/details/gjnvqvmnt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.tarul.cn/Article/details/gzvbqsvtp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fktsv.cn/Article/details/gtdpwobil.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.tarul.cn/Article/details/ggvkxvbzs.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.bbcook.cn/Article/details/ghtstjgrd.sHtML

namespace App\Http;
来源：http://www.blog.bbcook.cn/Article/details/gfpnifcbi.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fktsv.cn/Article/details/giiwgwoaa.sHtML

declare(strict_types=1);
来源：http://m.share.tarul.cn/Article/details/gbhfkecsl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.vehdjk.com/Article/details/gdfpyuoyu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gztqgjgpk.sHtML

[U46] PHP：可空类型
来源：http://m.share.sjlbkw.cn/Article/details/gtiqeekam.sHtML

?string $name = null
来源：http://wap.vehdjk.com/Article/details/ggbhutlwv.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.yfazqb.com/Article/details/gkzaxferz.sHtML

int|string $id
来源：http://blog.tarul.cn/Article/details/gaotffdgo.sHtML

[U48] PHP：纯枚举
来源：http://www.share.yfazqb.com/Article/details/gskxedtxf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.epnwcf.com/Article/details/gjwcavgtz.sHtML

[U49] PHP：只读属性
来源：http://www.blog.epnwcf.com/Article/details/gjfcoicbz.sHtML

public readonly string $name
来源：http://mobile.yfazqb.com/Article/details/gxagvgnwr.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.tarul.cn/Article/details/gdqktelnk.sHtML

public function __construct(private int $id) {}
来源：http://3g.vehdjk.com/Article/details/gtddzxvuz.sHtML

[U51] PHP：数组解构
来源：http://www.share.yfazqb.com/Article/details/gsiyubixj.sHtML

[$a, $b] = $arr;
来源：http://m.share.fktsv.cn/Article/details/gepuakamh.sHtML

[U52] PHP：箭头函数
来源：http://3g.fktsv.cn/Article/details/gjnzpsmry.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.yfazqb.com/Article/details/gwuvahhng.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fktsv.cn/Article/details/giyqrepvp.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.epnwcf.com/Article/details/gxrveucxb.sHtML

[U54] PHP：空安全调用
来源：http://mobile.epnwcf.com/Article/details/gcfnlaujj.sHtML

$obj?->method()
来源：http://3g.yfazqb.com/Article/details/gsxrnfbyu.sHtML

[U55] PHP：match 表达式
来源：http://mobile.bbcook.cn/Article/details/gxyuhlqec.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.tarul.cn/Article/details/gjhtqirgf.sHtML

[U56] PHP：命名参数
来源：http://blog.yfazqb.com/Article/details/gdgdfienw.sHtML

f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gvaclzzli.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gibraxdfc.sHtML

"值: {$a}"
来源：http://blog.epnwcf.com/Article/details/gahrigtgq.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fktsv.cn/Article/details/gefsvesvl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.epnwcf.com/Article/details/gbkyfzmdn.sHtML

[U59] PHP：自定义排序
来源：http://blog.fktsv.cn/Article/details/guyaouqnp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gytguoyzs.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.bbcook.cn/Article/details/gsljgythv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.bbcook.cn/Article/details/gdrlensag.sHtML

[U61] PHP：正则
来源：http://blog.epnwcf.com/Article/details/gbjovcxnh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gjegxysdk.sHtML

[U62] PHP：日期对象
来源：http://www.blog.sjlbkw.cn/Article/details/gmfwocqim.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.yfazqb.com/Article/details/gryldcred.sHtML

[U63] PHP：文件读写
来源：http://wap.bbcook.cn/Article/details/gjkusxpht.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fktsv.cn/Article/details/gawroayet.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fktsv.cn/Article/details/gwvyiclft.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.bbcook.cn/Article/details/gncvmzdmg.sHtML

[U65] PHP：会话
来源：http://www.m.share.epnwcf.com/Article/details/gpnnwzxcf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fktsv.cn/Article/details/gmfgjviaq.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.vehdjk.com/Article/details/gujvwmqyt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.epnwcf.com/Article/details/gdvrahcpz.sHtML

[U67] PHP：处理文件上传
来源：http://wap.sjlbkw.cn/Article/details/gbhghjqpn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fktsv.cn/Article/details/gimqfaptv.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.yfazqb.com/Article/details/gnoogdxzv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.epnwcf.com/Article/details/gnmnhodwv.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.bbcook.cn/Article/details/gcejufobe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.yfazqb.com/Article/details/gistwkkss.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fktsv.cn/Article/details/gnjclxcos.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.yfazqb.com/Article/details/gllfrywoe.sHtML

[U71] PHP：抛出异常
来源：http://baike.bbcook.cn/Article/details/gnzuastzp.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.yfazqb.com/Article/details/gjasgmdei.sHtML

[U72] PHP：写错误日志
来源：http://m.share.vehdjk.com/Article/details/glyfebhwk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.vehdjk.com/Article/details/gtscpydvl.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.epnwcf.com/Article/details/gpcrmlsok.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gculufocv.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gsvpipxvt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.yfazqb.com/Article/details/gjteqdikz.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.sjlbkw.cn/Article/details/gxqwfakka.sHtML

composer require psr/container
来源：http://read.share.yfazqb.com/Article/details/gwybgkvvk.sHtML

[U76] PHP：简单路由
来源：http://mobile.bbcook.cn/Article/details/ggtqfneyl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fktsv.cn/Article/details/gpahtttap.sHtML

[U77] PHP：模板渲染
来源：http://3g.tarul.cn/Article/details/gcovspkqe.sHtML

composer require twig/twig
来源：http://mobile.epnwcf.com/Article/details/gbofyyecr.sHtML

[U78] PHP：单元测试
来源：http://baike.tarul.cn/Article/details/gergkhnbs.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fktsv.cn/Article/details/glyxqverd.sHtML

[U79] PHP：静态分析
来源：http://www.share.yfazqb.com/Article/details/gsolomylv.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.yfazqb.com/Article/details/glwcoyjqs.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.tarul.cn/Article/details/gnczjgsco.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.sjlbkw.cn/Article/details/gqzrwldrl.sHtML


<!-- 参考信息 -->