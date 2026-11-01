代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://wap.fktsv.cn/Article/details/gjltguzmw.sHtML

[S59] C++：静态断言
来源：http://m.share.epnwcf.com/Article/details/gcwizvgwy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.sjlbkw.cn/Article/details/gnemzzvbl.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fktsv.cn/Article/details/gixlccqpd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/gzhzhlvon.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gkfaiduyf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gbtfkzrxw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcebnsfsh.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.epnwcf.com/Article/details/gomkheffw.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gejaosxsm.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.tarul.cn/Article/details/glxbepapl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.yfazqb.com/Article/details/gafbalqdp.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.epnwcf.com/Article/details/gheftvrid.sHtML

"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gzhbwjugi.sHtML

[T04] Kotlin：空安全
来源：http://blog.epnwcf.com/Article/details/gckqdxdbj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/guwsnelsf.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.yfazqb.com/Article/details/gnvakoikn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.sjlbkw.cn/Article/details/ghftgmlof.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.epnwcf.com/Article/details/gvzjldfal.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gqaqeijyn.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/gjgoebcfg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fktsv.cn/Article/details/ghwpjrftt.sHtML

[T08] Kotlin：数据类
来源：http://m.share.bbcook.cn/Article/details/gwaxxzzxe.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fktsv.cn/Article/details/gltbukmuy.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.bbcook.cn/Article/details/gxgsecqwu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/gtqexwuro.sHtML

[T10] Kotlin：默认参数
来源：http://baike.tarul.cn/Article/details/genwfblda.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.sjlbkw.cn/Article/details/gaeglhspi.sHtML

[T11] Kotlin：协程
来源：http://m.share.bbcook.cn/Article/details/gmhdvczex.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.tarul.cn/Article/details/gumrkkqoe.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.vehdjk.com/Article/details/gsakjanvb.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/gsjraislh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.tarul.cn/Article/details/ghzeswwoz.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fktsv.cn/Article/details/gyaepbmwm.sHtML

[T14] Kotlin：循环
来源：http://baike.sjlbkw.cn/Article/details/grvzhulkl.sHtML

for (i in 1..10) println(i)
来源：http://3g.tarul.cn/Article/details/gwcrndssn.sHtML

[T15] Kotlin：接口
来源：http://read.share.fktsv.cn/Article/details/gtekilual.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/gtoyhktmg.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/ghyvdroco.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/gxjbelmkd.sHtML

[T17] Swift：变量与常量
来源：http://3g.vehdjk.com/Article/details/gwjzokpuc.sHtML

var a = 1;  let b = 2
来源：http://baike.epnwcf.com/Article/details/gfojseier.sHtML

[T18] Swift：字符串插值
来源：http://www.share.vehdjk.com/Article/details/guqvmebho.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/gsdshmsqt.sHtML

[T19] Swift：可选绑定
来源：http://3g.epnwcf.com/Article/details/gnwuucmnk.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/gvbnsevnn.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/gtiunpfyi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/gwllgjvep.sHtML

[T21] Swift：遍历
来源：http://3g.epnwcf.com/Article/details/gnkezjhga.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/gzuhzzeew.sHtML

[T22] Swift：字典
来源：http://m.share.fktsv.cn/Article/details/ggxouebad.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fktsv.cn/Article/details/gyhdiozfb.sHtML

[T23] Swift：函数
来源：http://m.share.tarul.cn/Article/details/gtmvdhsbr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.tarul.cn/Article/details/gkfvnevse.sHtML

[T24] Swift：闭包
来源：http://wap.sjlbkw.cn/Article/details/gfkdiyutj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.bbcook.cn/Article/details/gflprbzbs.sHtML

[T25] Swift：结构体
来源：http://mobile.sjlbkw.cn/Article/details/gezzdawcl.sHtML

struct P { var x: Int }
来源：http://www.m.share.vehdjk.com/Article/details/guwtyyllo.sHtML

[T26] Swift：类与重写
来源：http://3g.bbcook.cn/Article/details/ghmdphryc.sHtML

class A: Base { override func f() {} }
来源：http://m.share.tarul.cn/Article/details/gqdvlbqif.sHtML

[T27] Swift：错误处理
来源：http://3g.epnwcf.com/Article/details/gopubagzm.sHtML

do { try f() } catch { print(error) }
来源：http://blog.tarul.cn/Article/details/ggugybowi.sHtML

[T28] Swift：枚举
来源：http://wap.tarul.cn/Article/details/gqqppvooq.sHtML

enum Color { case red, green }
来源：http://www.share.vehdjk.com/Article/details/gvffokcjj.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.vehdjk.com/Article/details/gonwzkhtn.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fktsv.cn/Article/details/ghursbdeu.sHtML

[T30] Swift：协议
来源：http://www.blog.tarul.cn/Article/details/gymkzdnkm.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.vehdjk.com/Article/details/gjjkhlnfh.sHtML

[T31] Lua：Hello World
来源：http://3g.vehdjk.com/Article/details/gxkhdmaxw.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/gzjrzrrvk.sHtML

[T32] Lua：局部变量
来源：http://baike.epnwcf.com/Article/details/gxcbelrpj.sHtML

local a = 1
来源：http://wap.sjlbkw.cn/Article/details/ghsmtesmz.sHtML

[T33] Lua：表（数组）
来源：http://www.share.tarul.cn/Article/details/gmlxrbdzl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.yfazqb.com/Article/details/gsnwooykb.sHtML

[T34] Lua：遍历表
来源：http://blog.fktsv.cn/Article/details/gyqtdidod.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.epnwcf.com/Article/details/gzrjmmygn.sHtML

[T35] Lua：字典表
来源：http://www.blog.yfazqb.com/Article/details/gylqybfcf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.vehdjk.com/Article/details/gphchlxar.sHtML

[T36] Lua：函数
来源：http://baike.bbcook.cn/Article/details/ghclomqhk.sHtML

function add(a, b) return a + b end
来源：http://www.blog.sjlbkw.cn/Article/details/gvhddrgjk.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/gdngsrbrh.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/gwqapyrym.sHtML

[T38] Lua：条件
来源：http://www.share.yfazqb.com/Article/details/geyltzjcp.sHtML

if x > 0 then print("正") end
来源：http://mobile.yfazqb.com/Article/details/grolzymge.sHtML

[T39] Lua：模式匹配
来源：http://blog.vehdjk.com/Article/details/ggkgalldw.sHtML

string.find(s, "%d+")
来源：http://www.blog.tarul.cn/Article/details/glvpwkrpk.sHtML

[T40] Lua：元表
来源：http://www.m.share.yfazqb.com/Article/details/gqhfajpvu.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.epnwcf.com/Article/details/geqvzaxjd.sHtML

[T41] Perl：Hello World
来源：http://m.share.yfazqb.com/Article/details/gozqnnren.sHtML

print "Hello\n";
来源：http://www.share.tarul.cn/Article/details/gbyghhxoq.sHtML

[T42] Perl：变量类型
来源：http://mobile.vehdjk.com/Article/details/ghkjvjupv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.vehdjk.com/Article/details/gyzaeaaqx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/guohyvdwt.sHtML

"值: $a"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyozmmrw.sHtML

[T44] Perl：条件
来源：http://m.share.tarul.cn/Article/details/gnmdhlzns.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/gtznkalln.sHtML

[T45] Perl：数组遍历
来源：http://3g.vehdjk.com/Article/details/gyfkfxhqb.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.tarul.cn/Article/details/gpgurczqt.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.epnwcf.com/Article/details/gpqtkrmkz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.yfazqb.com/Article/details/gbsglldsl.sHtML

[T47] Perl：正则捕获
来源：http://wap.fktsv.cn/Article/details/gcpldidjo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fktsv.cn/Article/details/govydnims.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/ggxmwyptl.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.tarul.cn/Article/details/gqzehozls.sHtML

[T49] Perl：函数
来源：http://3g.yfazqb.com/Article/details/gfvutytnz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gxhrjnlkg.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fktsv.cn/Article/details/guovipljw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.sjlbkw.cn/Article/details/gpcjquzgu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.bbcook.cn/Article/details/glludtkpt.sHtML

[T51] Scala：Hello World
来源：http://blog.vehdjk.com/Article/details/gxoiplyez.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gjkfiyguc.sHtML

[T52] Scala：变量
来源：http://m.share.vehdjk.com/Article/details/gzgaltnut.sHtML

val a = 1;  var b = 2
来源：http://wap.epnwcf.com/Article/details/glogfowxy.sHtML

[T53] Scala：字符串插值
来源：http://www.share.tarul.cn/Article/details/gljvbzfdw.sHtML

s"值: $b"
来源：http://mobile.bbcook.cn/Article/details/gtnglinbv.sHtML

[T54] Scala：集合映射
来源：http://read.share.yfazqb.com/Article/details/gpxlwwsrp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fktsv.cn/Article/details/gapujgjfx.sHtML

[T55] Scala：集合过滤
来源：http://blog.fktsv.cn/Article/details/gzraymsta.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.epnwcf.com/Article/details/ggvydjeiw.sHtML

[T56] Scala：样例类
来源：http://wap.vehdjk.com/Article/details/geeqcvkek.sHtML

case class User(name: String, age: Int)
来源：http://wap.bbcook.cn/Article/details/gkdoscxrb.sHtML

[T57] Scala：模式匹配
来源：http://blog.yfazqb.com/Article/details/gtkllftec.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.tarul.cn/Article/details/gafordmok.sHtML

[T58] Scala：函数定义
来源：http://mobile.yfazqb.com/Article/details/ggqvauirr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.sjlbkw.cn/Article/details/gmoddymki.sHtML

[T59] Scala：循环
来源：http://www.share.epnwcf.com/Article/details/gldwqaayx.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.vehdjk.com/Article/details/ggjukfkhr.sHtML

[T60] Scala：折叠
来源：http://3g.fktsv.cn/Article/details/gweaeirys.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.tarul.cn/Article/details/gdgdtfwfd.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gnujugnxq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/ggbfwbbwn.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqrycalmf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.tarul.cn/Article/details/glehtzkmb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.yfazqb.com/Article/details/gsfoqmbre.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/gupesuipd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.tarul.cn/Article/details/gerunopmv.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.vehdjk.com/Article/details/goxlfrjdr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.sjlbkw.cn/Article/details/gutoqiary.sHtML

[U04] Py：变量调试打印
来源：http://read.share.epnwcf.com/Article/details/gmalavtiu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.yfazqb.com/Article/details/gbpxzxvhy.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fktsv.cn/Article/details/gvutdzunm.sHtML

list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/gfmddsgku.sHtML

[U06] Py：合并两个字典
来源：http://wap.epnwcf.com/Article/details/gwazvehng.sHtML

{**a, **b}
来源：http://3g.sjlbkw.cn/Article/details/gewldmmdm.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.tarul.cn/Article/details/gbjsvcbyq.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.bbcook.cn/Article/details/ghebncatc.sHtML

[U08] Py：展平二维列表
来源：http://3g.vehdjk.com/Article/details/gujojdudf.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.epnwcf.com/Article/details/gwsmyfvys.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/gahyyrabj.sHtML

max(d, key=d.get)
来源：http://blog.sjlbkw.cn/Article/details/gdotfqpif.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fktsv.cn/Article/details/gcckpecdp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.vehdjk.com/Article/details/gncgzfcje.sHtML

[U11] Py：生成器表达式
来源：http://3g.yfazqb.com/Article/details/gqdtjrbfw.sHtML

(x * 2 for x in arr)
来源：http://baike.sjlbkw.cn/Article/details/gfeszbmyd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.tarul.cn/Article/details/gnjkbygha.sHtML

Counter(arr).most_common(3)
来源：http://blog.yfazqb.com/Article/details/gjnwppxzc.sHtML

[U13] Py：固定长度队列
来源：http://m.share.tarul.cn/Article/details/gfyjxzvyk.sHtML

deque(maxlen=10)
来源：http://www.m.share.epnwcf.com/Article/details/gpdtazjqt.sHtML

[U14] Py：分组收集到列表
来源：http://blog.bbcook.cn/Article/details/gvwbqksjy.sHtML

defaultdict(list)
来源：http://3g.epnwcf.com/Article/details/gqdlblrfx.sHtML

[U15] Py：高精度计时
来源：http://www.share.tarul.cn/Article/details/glxqsovol.sHtML

t = time.perf_counter()
来源：http://mobile.yfazqb.com/Article/details/giphgugpb.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.sjlbkw.cn/Article/details/gupjqhkxu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.yfazqb.com/Article/details/gtexbilvp.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.epnwcf.com/Article/details/gfcafvysv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fktsv.cn/Article/details/gjceusynr.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/gjdtscvex.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.tarul.cn/Article/details/gezhuorlq.sHtML

[U19] Py：正则替换带回调
来源：http://blog.bbcook.cn/Article/details/glboiewqc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.yfazqb.com/Article/details/gtnzlagri.sHtML

[U20] Py：缓存函数结果
来源：http://baike.vehdjk.com/Article/details/guathcnjm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.epnwcf.com/Article/details/ghpfopyte.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.sjlbkw.cn/Article/details/gjhuesfko.sHtML

@contextlib.contextmanager
来源：http://www.share.vehdjk.com/Article/details/gtgutslca.sHtML

[U22] Py：矩阵转置
来源：http://m.share.bbcook.cn/Article/details/giiydvonw.sHtML

list(zip(*m))
来源：http://www.blog.vehdjk.com/Article/details/ggzsezbtm.sHtML

[U23] Py：分块读取大文件
来源：http://blog.epnwcf.com/Article/details/gfbpmsutr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.epnwcf.com/Article/details/gjadhlemq.sHtML

[U24] Py：路径操作
来源：http://wap.yfazqb.com/Article/details/gjnsuolwb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gkpzandnm.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.tarul.cn/Article/details/gqrlyaaod.sHtML

csv.DictReader(f)
来源：http://www.share.epnwcf.com/Article/details/gjzbenceb.sHtML

[U26] Py：并发下载
来源：http://m.share.tarul.cn/Article/details/gtllywpjy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.epnwcf.com/Article/details/gyglraarb.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.bbcook.cn/Article/details/gdxrmmbmz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.sjlbkw.cn/Article/details/glwofdkmb.sHtML

[U28] Py：类型别名
来源：http://wap.epnwcf.com/Article/details/gotxsmqzn.sHtML

UserId = int
来源：http://baike.epnwcf.com/Article/details/gkttbxmzx.sHtML

[U29] Py：属性校验
来源：http://m.share.sjlbkw.cn/Article/details/ggzyhhfrk.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gxswkbtzr.sHtML

[U30] Py：数据类
来源：http://wap.bbcook.cn/Article/details/gcrsypnpq.sHtML

@dataclass(slots=True)
来源：http://read.share.yfazqb.com/Article/details/grbvfigoz.sHtML

[U31] Py：单测
来源：http://m.share.vehdjk.com/Article/details/gowvfmdsj.sHtML

python -m pytest -q
来源：http://read.share.bbcook.cn/Article/details/gdlnfskww.sHtML

[U32] Py：代码格式化
来源：http://baike.epnwcf.com/Article/details/gzaiznkba.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.tarul.cn/Article/details/gjlmeanwi.sHtML

[U33] Py：打包发布
来源：http://www.share.vehdjk.com/Article/details/gwcohjicz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.bbcook.cn/Article/details/gcbiprzfv.sHtML

[U34] Py：判断编码
来源：http://read.share.vehdjk.com/Article/details/gengxhwbc.sHtML

chardet.detect(raw)
来源：http://m.share.sjlbkw.cn/Article/details/glrcgbvbv.sHtML

[U35] Py：发送邮件
来源：http://www.share.epnwcf.com/Article/details/gynhuxcbd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fktsv.cn/Article/details/gdakzsyrk.sHtML

[U36] Py：定时任务
来源：http://wap.epnwcf.com/Article/details/gussjwyql.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.tarul.cn/Article/details/gfgicjtxj.sHtML

[U37] Py：读写 Excel
来源：http://blog.fktsv.cn/Article/details/gmtunensf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.sjlbkw.cn/Article/details/gzrsqvsff.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.epnwcf.com/Article/details/gmbljcxpy.sHtML

Path(__file__).resolve().parent
来源：http://www.share.sjlbkw.cn/Article/details/gtvpbgoqi.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.epnwcf.com/Article/details/gkcrlndcc.sHtML

sys.stdout.isatty()
来源：http://m.share.sjlbkw.cn/Article/details/gosgawqim.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.vehdjk.com/Article/details/ggprynzia.sHtML

print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/ggcbmowsc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.sjlbkw.cn/Article/details/gkezvgkhi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.vehdjk.com/Article/details/grskcbikv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.tarul.cn/Article/details/glsehriph.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.tarul.cn/Article/details/grfvxisth.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.bbcook.cn/Article/details/geuzqlbit.sHtML

namespace App\Http;
来源：http://read.share.tarul.cn/Article/details/gctncnoul.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.sjlbkw.cn/Article/details/glneksrij.sHtML

declare(strict_types=1);
来源：http://www.m.share.tarul.cn/Article/details/gimdxixka.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.tarul.cn/Article/details/gkyfurhjr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gjtlkaacl.sHtML

[U46] PHP：可空类型
来源：http://read.share.sjlbkw.cn/Article/details/gpbfgjgbs.sHtML

?string $name = null
来源：http://wap.tarul.cn/Article/details/gfpzgbhpl.sHtML

[U47] PHP：联合类型
来源：http://www.share.sjlbkw.cn/Article/details/gqhafimyo.sHtML

int|string $id
来源：http://www.blog.tarul.cn/Article/details/gyogpiicu.sHtML

[U48] PHP：纯枚举
来源：http://wap.yfazqb.com/Article/details/gyijwtrbe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.epnwcf.com/Article/details/gwwzvkyth.sHtML

[U49] PHP：只读属性
来源：http://wap.epnwcf.com/Article/details/gydjolpti.sHtML

public readonly string $name
来源：http://www.m.share.yfazqb.com/Article/details/gvjwgcrfu.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.bbcook.cn/Article/details/gftklipuq.sHtML

public function __construct(private int $id) {}
来源：http://3g.fktsv.cn/Article/details/gscekhoet.sHtML

[U51] PHP：数组解构
来源：http://mobile.fktsv.cn/Article/details/gbufywclh.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.yfazqb.com/Article/details/gohrbqshw.sHtML

[U52] PHP：箭头函数
来源：http://m.share.tarul.cn/Article/details/gmbiiuxax.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.yfazqb.com/Article/details/grcmjezhb.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fktsv.cn/Article/details/gbsitrzmp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fktsv.cn/Article/details/guhbwpxoc.sHtML

[U54] PHP：空安全调用
来源：http://www.share.yfazqb.com/Article/details/gzccmsvlo.sHtML

$obj?->method()
来源：http://read.share.yfazqb.com/Article/details/gjdejyyzy.sHtML

[U55] PHP：match 表达式
来源：http://wap.sjlbkw.cn/Article/details/gtnjohmhj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.bbcook.cn/Article/details/gddbotwne.sHtML

[U56] PHP：命名参数
来源：http://wap.tarul.cn/Article/details/gnvsveuzg.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gvfxajggt.sHtML

[U57] PHP：字符串插值
来源：http://3g.bbcook.cn/Article/details/gmojwbyud.sHtML

"值: {$a}"
来源：http://wap.yfazqb.com/Article/details/gbzzvrcdg.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fktsv.cn/Article/details/ghpwcwvbw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.yfazqb.com/Article/details/gefvrcgoz.sHtML

[U59] PHP：自定义排序
来源：http://3g.yfazqb.com/Article/details/gfhbdhpun.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gdjycjuui.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.epnwcf.com/Article/details/gonhaifqt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.sjlbkw.cn/Article/details/gtgxusagk.sHtML

[U61] PHP：正则
来源：http://www.blog.sjlbkw.cn/Article/details/ghyyeqpyi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/grcuifcxx.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.bbcook.cn/Article/details/gioirkush.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.epnwcf.com/Article/details/glurdmldd.sHtML

[U63] PHP：文件读写
来源：http://m.share.bbcook.cn/Article/details/gzwzxvhlz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.epnwcf.com/Article/details/gtibrnvsy.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fktsv.cn/Article/details/glzbleytt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.tarul.cn/Article/details/gqeimqaqt.sHtML

[U65] PHP：会话
来源：http://mobile.tarul.cn/Article/details/gxujjfwod.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gpufrwcub.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.vehdjk.com/Article/details/gjsyteycv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.yfazqb.com/Article/details/geokjxcpx.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.yfazqb.com/Article/details/gfphlskao.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fktsv.cn/Article/details/gusmkdplt.sHtML

[U68] PHP：PDO 连接
来源：http://blog.sjlbkw.cn/Article/details/ghtacoxxp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.epnwcf.com/Article/details/gjpumuwbs.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.tarul.cn/Article/details/gduaajrhx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gefpqqimt.sHtML

[U70] PHP：PDO 事务
来源：http://blog.vehdjk.com/Article/details/gbpjzoklr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.vehdjk.com/Article/details/gqofbsgsz.sHtML

[U71] PHP：抛出异常
来源：http://m.share.vehdjk.com/Article/details/ghxqziovg.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.yfazqb.com/Article/details/ghmeduobw.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.epnwcf.com/Article/details/gprhtkvbl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.bbcook.cn/Article/details/gtznfvgyg.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.epnwcf.com/Article/details/glrgaakys.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.bbcook.cn/Article/details/giladzviv.sHtML

[U74] PHP：读取环境变量
来源：http://wap.yfazqb.com/Article/details/ggmazgqqd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.yfazqb.com/Article/details/gcjlhekpr.sHtML

[U75] PHP：依赖注入
来源：http://wap.tarul.cn/Article/details/guliaqyal.sHtML

composer require psr/container
来源：http://3g.fktsv.cn/Article/details/ghocokyov.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fktsv.cn/Article/details/gicwfxkev.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.yfazqb.com/Article/details/gutovwbnk.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.sjlbkw.cn/Article/details/gtiaqszpw.sHtML

composer require twig/twig
来源：http://read.share.epnwcf.com/Article/details/gglvjtxro.sHtML

[U78] PHP：单元测试
来源：http://3g.yfazqb.com/Article/details/gxmfnbegs.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.vehdjk.com/Article/details/gilutsedv.sHtML

[U79] PHP：静态分析
来源：http://baike.bbcook.cn/Article/details/gqsenzpfj.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.epnwcf.com/Article/details/gfrdtylcn.sHtML

[U80] PHP：代码规范修复
来源：http://baike.yfazqb.com/Article/details/gdsdpleku.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.epnwcf.com/Article/details/glmjlshdo.sHtML

[U81] JS：初始化项目
来源：http://blog.fktsv.cn/Article/details/geyyzmeep.sHtML

npm init -y;  npm i express
来源：http://3g.sjlbkw.cn/Article/details/glxvnhhal.sHtML

[U82] JS：package.json 脚本
来源：http://baike.yfazqb.com/Article/details/gfditsknd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.bbcook.cn/Article/details/gfayoqknn.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.bbcook.cn/Article/details/gwwpuhvhq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.bbcook.cn/Article/details/gourhmmmz.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.sjlbkw.cn/Article/details/guhrldgme.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fktsv.cn/Article/details/giytmybqn.sHtML


<!-- 参考信息 -->