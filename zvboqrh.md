代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.tarul.cn/Article/details/gncymslty.sHtML

[S55] C++：结构化绑定
来源：http://baike.epnwcf.com/Article/details/gjahiflyv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.epnwcf.com/Article/details/gxfxtevfv.sHtML

[S56] C++：optional
来源：http://www.m.share.bbcook.cn/Article/details/gupsvkbul.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/gzrgkgnjv.sHtML

[S57] C++：编译期常量
来源：http://mobile.epnwcf.com/Article/details/gddgbhpvj.sHtML

constexpr int N = 10;
来源：http://mobile.fktsv.cn/Article/details/gqukveffl.sHtML

[S58] C++：命名空间
来源：http://baike.yfazqb.com/Article/details/gmiuqstfz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.sjlbkw.cn/Article/details/gdokederm.sHtML

[S59] C++：静态断言
来源：http://www.share.sjlbkw.cn/Article/details/gaebxfgrm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.bbcook.cn/Article/details/gszuxxpys.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.yfazqb.com/Article/details/gyextpvku.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gpcegvems.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gylzsfixs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/gusqvmtmm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gyykirusu.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gjxdourvy.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gesbzfkot.sHtML

[T02] Kotlin：变量
来源：http://3g.fktsv.cn/Article/details/gonqhtlwh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/ghmgxdjem.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.vehdjk.com/Article/details/gsxxoyahc.sHtML

"值: $b"
来源：http://blog.epnwcf.com/Article/details/ghjippcxm.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/gacjgasqa.sHtML

val n: String? = null;  n?.length
来源：http://blog.fktsv.cn/Article/details/gwgkuxkdj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.epnwcf.com/Article/details/gugorehww.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/gfjroftas.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.yfazqb.com/Article/details/gselqbfoo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fktsv.cn/Article/details/ggoypoyer.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gvuzrheic.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fktsv.cn/Article/details/gncnahcxh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.sjlbkw.cn/Article/details/gidzimqab.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fktsv.cn/Article/details/gfhijskvn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.bbcook.cn/Article/details/gvtotokyg.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.vehdjk.com/Article/details/gcqyrbrlg.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fktsv.cn/Article/details/geovqjyxb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.yfazqb.com/Article/details/gmdfdkpvx.sHtML

[T11] Kotlin：协程
来源：http://wap.epnwcf.com/Article/details/gjbqgahxv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.yfazqb.com/Article/details/grclmolyu.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.yfazqb.com/Article/details/gddtbdjeu.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.epnwcf.com/Article/details/giacxsyts.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/gxnmynkte.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/gsamsttog.sHtML

[T14] Kotlin：循环
来源：http://baike.epnwcf.com/Article/details/gxylpafib.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/ggvoykhwy.sHtML

[T15] Kotlin：接口
来源：http://www.blog.epnwcf.com/Article/details/gvbhhmrre.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.bbcook.cn/Article/details/gnnkteldr.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gdjqtgcrp.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gswkhtvtn.sHtML

[T17] Swift：变量与常量
来源：http://baike.sjlbkw.cn/Article/details/gmjyxrgff.sHtML

var a = 1;  let b = 2
来源：http://blog.vehdjk.com/Article/details/gfllszlsd.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gogbmuvdr.sHtML

"值: \(b)"
来源：http://www.m.share.bbcook.cn/Article/details/gzpplkzua.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.vehdjk.com/Article/details/goameebky.sHtML

if let n = opt { print(n) }
来源：http://mobile.sjlbkw.cn/Article/details/gwpvgqtlg.sHtML

[T20] Swift：数组操作
来源：http://www.blog.yfazqb.com/Article/details/gtqrdpnci.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fktsv.cn/Article/details/gsemvppxk.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gbdfgqnil.sHtML

for x in a { print(x) }
来源：http://www.m.share.vehdjk.com/Article/details/gjjqqhazj.sHtML

[T22] Swift：字典
来源：http://wap.yfazqb.com/Article/details/gojregiyz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.sjlbkw.cn/Article/details/gmwtwtgqb.sHtML

[T23] Swift：函数
来源：http://baike.fktsv.cn/Article/details/gqkiujzqf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fktsv.cn/Article/details/gkfjgwgkb.sHtML

[T24] Swift：闭包
来源：http://blog.sjlbkw.cn/Article/details/gugiicdrx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gucmufeps.sHtML

[T25] Swift：结构体
来源：http://www.blog.tarul.cn/Article/details/gebzfqwsd.sHtML

struct P { var x: Int }
来源：http://m.share.epnwcf.com/Article/details/gtpgcpjkb.sHtML

[T26] Swift：类与重写
来源：http://www.share.bbcook.cn/Article/details/gqmjogbef.sHtML

class A: Base { override func f() {} }
来源：http://mobile.epnwcf.com/Article/details/gxalogbbx.sHtML

[T27] Swift：错误处理
来源：http://3g.epnwcf.com/Article/details/gigxyuxzy.sHtML

do { try f() } catch { print(error) }
来源：http://blog.sjlbkw.cn/Article/details/gxosycdnb.sHtML

[T28] Swift：枚举
来源：http://www.blog.yfazqb.com/Article/details/gilxtzswl.sHtML

enum Color { case red, green }
来源：http://m.share.bbcook.cn/Article/details/guldukhec.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.sjlbkw.cn/Article/details/griytenur.sHtML

guard let x = opt else { return }
来源：http://3g.tarul.cn/Article/details/gmcbgtyzx.sHtML

[T30] Swift：协议
来源：http://www.share.tarul.cn/Article/details/gjqhiqyjw.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fktsv.cn/Article/details/ggnztjist.sHtML

[T31] Lua：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gtlmouamp.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gifwpplfh.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gwprovlsk.sHtML

local a = 1
来源：http://baike.vehdjk.com/Article/details/gdilmggek.sHtML

[T33] Lua：表（数组）
来源：http://blog.yfazqb.com/Article/details/gbjvgjcgi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.vehdjk.com/Article/details/gtqyocbdz.sHtML

[T34] Lua：遍历表
来源：http://read.share.epnwcf.com/Article/details/gramewimk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.epnwcf.com/Article/details/gnjzoynly.sHtML

[T35] Lua：字典表
来源：http://3g.sjlbkw.cn/Article/details/gteglwakw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.sjlbkw.cn/Article/details/ghosdflvn.sHtML

[T36] Lua：函数
来源：http://read.share.epnwcf.com/Article/details/giszwzlkj.sHtML

function add(a, b) return a + b end
来源：http://baike.yfazqb.com/Article/details/gnzuotzof.sHtML

[T37] Lua：字符串拼接
来源：http://blog.yfazqb.com/Article/details/gdyhutlnv.sHtML

"a" .. "b"
来源：http://blog.yfazqb.com/Article/details/gorerlovw.sHtML

[T38] Lua：条件
来源：http://www.blog.bbcook.cn/Article/details/gxhzbeusm.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.epnwcf.com/Article/details/gufwgdlpj.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gieirkdyk.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/goavdvehw.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/glusoyktz.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fktsv.cn/Article/details/gltstnwik.sHtML

[T41] Perl：Hello World
来源：http://baike.vehdjk.com/Article/details/gggwkrgos.sHtML

print "Hello\n";
来源：http://www.blog.yfazqb.com/Article/details/gezhfrmmk.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fktsv.cn/Article/details/gqpbbwlre.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.epnwcf.com/Article/details/guymecalm.sHtML

[T43] Perl：字符串插值
来源：http://3g.epnwcf.com/Article/details/gwswbvyxm.sHtML

"值: $a"
来源：http://m.share.epnwcf.com/Article/details/gszhlyotf.sHtML

[T44] Perl：条件
来源：http://m.share.tarul.cn/Article/details/gsstdhcvw.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.sjlbkw.cn/Article/details/goqkbwguq.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fktsv.cn/Article/details/gjpxzkdgn.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.vehdjk.com/Article/details/gkposcwbu.sHtML

[T46] Perl：哈希操作
来源：http://3g.yfazqb.com/Article/details/gsttzjcoy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.vehdjk.com/Article/details/gtodsrqel.sHtML

[T47] Perl：正则捕获
来源：http://wap.epnwcf.com/Article/details/giyagjwif.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.tarul.cn/Article/details/gatzwkwyt.sHtML

[T48] Perl：正则替换
来源：http://wap.vehdjk.com/Article/details/gezededce.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/gthyfhuls.sHtML

[T49] Perl：函数
来源：http://www.share.bbcook.cn/Article/details/gbsjadyki.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gqfzdwbxa.sHtML

[T50] Perl：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gpadkieds.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/gxzbxxhel.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.epnwcf.com/Article/details/gvyhaimll.sHtML

[T51] Scala：Hello World
来源：http://m.share.epnwcf.com/Article/details/gadampkzr.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/ghoiuvzqw.sHtML

[T52] Scala：变量
来源：http://wap.tarul.cn/Article/details/gkiyoswon.sHtML

val a = 1;  var b = 2
来源：http://m.share.sjlbkw.cn/Article/details/gfqhbtewf.sHtML

[T53] Scala：字符串插值
来源：http://wap.yfazqb.com/Article/details/gyfgzexuz.sHtML

s"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/guvrvoion.sHtML

[T54] Scala：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/grfmzciiw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gchvknotm.sHtML

[T55] Scala：集合过滤
来源：http://blog.bbcook.cn/Article/details/gbnxfmkey.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.tarul.cn/Article/details/ghxisqipb.sHtML

[T56] Scala：样例类
来源：http://www.blog.fktsv.cn/Article/details/gsjqxbqal.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/gtxusohds.sHtML

[T57] Scala：模式匹配
来源：http://3g.bbcook.cn/Article/details/gfamgjpds.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.tarul.cn/Article/details/goueoockw.sHtML

[T58] Scala：函数定义
来源：http://3g.fktsv.cn/Article/details/ggyxudbmt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.epnwcf.com/Article/details/gmwytujui.sHtML

[T59] Scala：循环
来源：http://3g.fktsv.cn/Article/details/gzqmeqqbb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/gwptrznyv.sHtML

[T60] Scala：折叠
来源：http://m.share.fktsv.cn/Article/details/gkwknljxf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.vehdjk.com/Article/details/gshekcbho.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjbyokkub.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/gzoijmpps.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxjifucze.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.bbcook.cn/Article/details/gfvxodqiz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.sjlbkw.cn/Article/details/guypcubdn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.vehdjk.com/Article/details/gkfukpgtw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.bbcook.cn/Article/details/gvqaujtzc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.bbcook.cn/Article/details/gttwjurpi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.tarul.cn/Article/details/gaevjpxol.sHtML

[U04] Py：变量调试打印
来源：http://m.share.sjlbkw.cn/Article/details/gqyzkgagw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.tarul.cn/Article/details/gyqgluzhj.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fktsv.cn/Article/details/gmgegrsge.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gqgcjqfau.sHtML

[U06] Py：合并两个字典
来源：http://www.share.tarul.cn/Article/details/gfowkxzvm.sHtML

{**a, **b}
来源：http://read.share.vehdjk.com/Article/details/gblgupyee.sHtML

[U07] Py：反转字典键值
来源：http://m.share.tarul.cn/Article/details/gkqbttdmk.sHtML

{v: k for k, v in d.items()}
来源：http://baike.yfazqb.com/Article/details/ghrzmjiuj.sHtML

[U08] Py：展平二维列表
来源：http://blog.yfazqb.com/Article/details/gbprhrska.sHtML

[y for x in nested for y in x]
来源：http://www.share.yfazqb.com/Article/details/goofzedbu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.epnwcf.com/Article/details/glbzshirw.sHtML

max(d, key=d.get)
来源：http://3g.tarul.cn/Article/details/gxheohcer.sHtML

[U10] Py：按值排序字典
来源：http://m.share.epnwcf.com/Article/details/gfoscxvxp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.bbcook.cn/Article/details/guqndlqnf.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fktsv.cn/Article/details/gegllujxe.sHtML

(x * 2 for x in arr)
来源：http://blog.tarul.cn/Article/details/gewnmzzmq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.sjlbkw.cn/Article/details/glgdreyyf.sHtML

Counter(arr).most_common(3)
来源：http://baike.fktsv.cn/Article/details/gqyqbruae.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fktsv.cn/Article/details/gidjltwiz.sHtML

deque(maxlen=10)
来源：http://wap.yfazqb.com/Article/details/geoffvqsi.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.epnwcf.com/Article/details/ggsqctder.sHtML

defaultdict(list)
来源：http://m.share.bbcook.cn/Article/details/guhjyhbxi.sHtML

[U15] Py：高精度计时
来源：http://3g.yfazqb.com/Article/details/geogsuxhf.sHtML

t = time.perf_counter()
来源：http://www.share.tarul.cn/Article/details/gdejbrwmv.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.epnwcf.com/Article/details/gzdysdchy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.yfazqb.com/Article/details/gknyxkltd.sHtML

[U17] Py：初始化日志
来源：http://read.share.bbcook.cn/Article/details/gzboxjwew.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.tarul.cn/Article/details/gtleaquuh.sHtML

[U18] Py：预编译正则
来源：http://mobile.sjlbkw.cn/Article/details/gwcjvwcns.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.epnwcf.com/Article/details/gywydpknj.sHtML

[U19] Py：正则替换带回调
来源：http://wap.tarul.cn/Article/details/ghpapoicl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.vehdjk.com/Article/details/gyrluyqpd.sHtML

[U20] Py：缓存函数结果
来源：http://blog.sjlbkw.cn/Article/details/gudqnkkoa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.sjlbkw.cn/Article/details/grzijutdp.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.epnwcf.com/Article/details/gtxocsttx.sHtML

@contextlib.contextmanager
来源：http://www.m.share.yfazqb.com/Article/details/gfehermfb.sHtML

[U22] Py：矩阵转置
来源：http://baike.yfazqb.com/Article/details/gbbjnfthe.sHtML

list(zip(*m))
来源：http://blog.vehdjk.com/Article/details/ggtutehzk.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fktsv.cn/Article/details/ghktlpgro.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.epnwcf.com/Article/details/gapgblkmi.sHtML

[U24] Py：路径操作
来源：http://3g.yfazqb.com/Article/details/gjpeourwd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.yfazqb.com/Article/details/gqdfbyuve.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.vehdjk.com/Article/details/gednyscxu.sHtML

csv.DictReader(f)
来源：http://blog.fktsv.cn/Article/details/gcvuavizl.sHtML

[U26] Py：并发下载
来源：http://read.share.fktsv.cn/Article/details/gwdbpvixl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fktsv.cn/Article/details/grrggrcpb.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.epnwcf.com/Article/details/gziqvtcys.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.vehdjk.com/Article/details/gijyuidwt.sHtML

[U28] Py：类型别名
来源：http://blog.vehdjk.com/Article/details/gnfgwdvlx.sHtML

UserId = int
来源：http://read.share.yfazqb.com/Article/details/gwckmgnva.sHtML

[U29] Py：属性校验
来源：http://www.share.tarul.cn/Article/details/guuufxtcv.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.bbcook.cn/Article/details/gopjgnpsr.sHtML

[U30] Py：数据类
来源：http://www.m.share.epnwcf.com/Article/details/geipfydox.sHtML

@dataclass(slots=True)
来源：http://mobile.epnwcf.com/Article/details/gqcvembns.sHtML

[U31] Py：单测
来源：http://www.m.share.epnwcf.com/Article/details/ggmndbstz.sHtML

python -m pytest -q
来源：http://m.share.yfazqb.com/Article/details/gwpfkerxc.sHtML

[U32] Py：代码格式化
来源：http://3g.tarul.cn/Article/details/giryfnruy.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.yfazqb.com/Article/details/gjesdkjge.sHtML

[U33] Py：打包发布
来源：http://read.share.sjlbkw.cn/Article/details/gvbsgtpwy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.yfazqb.com/Article/details/gckftzxjn.sHtML

[U34] Py：判断编码
来源：http://wap.sjlbkw.cn/Article/details/gucdntkql.sHtML

chardet.detect(raw)
来源：http://3g.sjlbkw.cn/Article/details/gswfzanxt.sHtML

[U35] Py：发送邮件
来源：http://3g.bbcook.cn/Article/details/gmcofglmy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.sjlbkw.cn/Article/details/grldzyeeg.sHtML

[U36] Py：定时任务
来源：http://read.share.bbcook.cn/Article/details/gkgrmhjhn.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.epnwcf.com/Article/details/grmktoraj.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.tarul.cn/Article/details/ggcqrvrav.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fktsv.cn/Article/details/gomeizapv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.bbcook.cn/Article/details/gcorenbik.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.tarul.cn/Article/details/gqoxeklot.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.bbcook.cn/Article/details/gzmwjezqy.sHtML

sys.stdout.isatty()
来源：http://mobile.vehdjk.com/Article/details/gvypjlkzc.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.vehdjk.com/Article/details/gjldhnjhb.sHtML

print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/gioupdwjo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.sjlbkw.cn/Article/details/gpegqqomn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.sjlbkw.cn/Article/details/gmyufoxlg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.yfazqb.com/Article/details/ghuvfraqd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.tarul.cn/Article/details/gtszkkdzy.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fktsv.cn/Article/details/gjxbohcgg.sHtML

namespace App\Http;
来源：http://wap.epnwcf.com/Article/details/gdsmwtcvw.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.bbcook.cn/Article/details/gnnduoojg.sHtML

declare(strict_types=1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdmjkrlj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.epnwcf.com/Article/details/gpbjfemif.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gyshgquft.sHtML

[U46] PHP：可空类型
来源：http://3g.epnwcf.com/Article/details/ghyljovly.sHtML

?string $name = null
来源：http://3g.fktsv.cn/Article/details/gttuxefwb.sHtML

[U47] PHP：联合类型
来源：http://m.share.bbcook.cn/Article/details/gqiuensix.sHtML

int|string $id
来源：http://3g.yfazqb.com/Article/details/gwmwdusnc.sHtML

[U48] PHP：纯枚举
来源：http://www.share.bbcook.cn/Article/details/galfnhoxj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fktsv.cn/Article/details/gshlzxnnw.sHtML

[U49] PHP：只读属性
来源：http://wap.sjlbkw.cn/Article/details/gfkupoawg.sHtML

public readonly string $name
来源：http://baike.sjlbkw.cn/Article/details/giblcsvau.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.bbcook.cn/Article/details/gwrcbwevb.sHtML

public function __construct(private int $id) {}
来源：http://baike.tarul.cn/Article/details/gzkvfmdlt.sHtML

[U51] PHP：数组解构
来源：http://www.blog.vehdjk.com/Article/details/gwxwohxrd.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhsqjqmr.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/gujyjhisb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.sjlbkw.cn/Article/details/gheyvfaow.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.yfazqb.com/Article/details/gvetbzoml.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.vehdjk.com/Article/details/gxfwvyurf.sHtML

[U54] PHP：空安全调用
来源：http://3g.vehdjk.com/Article/details/gzlpufkrp.sHtML

$obj?->method()
来源：http://www.blog.sjlbkw.cn/Article/details/gqbsncmpt.sHtML

[U55] PHP：match 表达式
来源：http://baike.yfazqb.com/Article/details/grzwhixju.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/gjenlpysx.sHtML

[U56] PHP：命名参数
来源：http://wap.vehdjk.com/Article/details/gvlsbmjcc.sHtML

f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gqtoyzcgw.sHtML

[U57] PHP：字符串插值
来源：http://read.share.tarul.cn/Article/details/gqhnxpvui.sHtML

"值: {$a}"
来源：http://baike.fktsv.cn/Article/details/ggqlyxoxw.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.bbcook.cn/Article/details/gmencvrnq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.tarul.cn/Article/details/gchomnpcg.sHtML

[U59] PHP：自定义排序
来源：http://www.share.sjlbkw.cn/Article/details/gyhqwfdxz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/gslasvvrt.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.tarul.cn/Article/details/gekfcenip.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.epnwcf.com/Article/details/gegfwfjty.sHtML

[U61] PHP：正则
来源：http://baike.sjlbkw.cn/Article/details/glihdwlcw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gfdjoxwty.sHtML

[U62] PHP：日期对象
来源：http://wap.bbcook.cn/Article/details/geetowuyv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.epnwcf.com/Article/details/gegtlzadg.sHtML

[U63] PHP：文件读写
来源：http://mobile.vehdjk.com/Article/details/gvvgbojkk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.epnwcf.com/Article/details/ghvyzaafo.sHtML

[U64] PHP：目录遍历
来源：http://blog.fktsv.cn/Article/details/gsrgrukob.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.vehdjk.com/Article/details/goohgtkwq.sHtML

[U65] PHP：会话
来源：http://www.share.fktsv.cn/Article/details/gogsxyfgv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gqrfdpydx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fktsv.cn/Article/details/gsmwyximc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fktsv.cn/Article/details/gdhadiqvr.sHtML

[U67] PHP：处理文件上传
来源：http://wap.sjlbkw.cn/Article/details/gaawdkdjk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.yfazqb.com/Article/details/grkywdzsm.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.sjlbkw.cn/Article/details/gtflzlotb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.bbcook.cn/Article/details/gokbkeqpv.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.bbcook.cn/Article/details/gsignqwfx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.epnwcf.com/Article/details/gmxmjnypf.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.vehdjk.com/Article/details/gtwhidgqz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.sjlbkw.cn/Article/details/gkhuxuova.sHtML

[U71] PHP：抛出异常
来源：http://blog.tarul.cn/Article/details/grvbnvyoc.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.epnwcf.com/Article/details/gxcfkqxue.sHtML

[U72] PHP：写错误日志
来源：http://3g.yfazqb.com/Article/details/gvjhaiebr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fktsv.cn/Article/details/gnaytaaxh.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.epnwcf.com/Article/details/glademprp.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.bbcook.cn/Article/details/guvzcwltc.sHtML

[U74] PHP：读取环境变量
来源：http://baike.tarul.cn/Article/details/gqmuxycyw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.bbcook.cn/Article/details/gxxslcpxf.sHtML

[U75] PHP：依赖注入
来源：http://blog.vehdjk.com/Article/details/gostdluoz.sHtML

composer require psr/container
来源：http://mobile.epnwcf.com/Article/details/geginlplr.sHtML

[U76] PHP：简单路由
来源：http://wap.fktsv.cn/Article/details/guihvhtll.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.tarul.cn/Article/details/gutgvjvyg.sHtML

[U77] PHP：模板渲染
来源：http://read.share.bbcook.cn/Article/details/gbqfymmok.sHtML

composer require twig/twig
来源：http://wap.yfazqb.com/Article/details/gwmmlkyjz.sHtML

[U78] PHP：单元测试
来源：http://read.share.vehdjk.com/Article/details/gfpcxjbny.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.yfazqb.com/Article/details/gbwakhwub.sHtML

[U79] PHP：静态分析
来源：http://wap.fktsv.cn/Article/details/gvbydavrz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.tarul.cn/Article/details/gsznsftrp.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fktsv.cn/Article/details/gxkvambjo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.bbcook.cn/Article/details/gpwjwmbid.sHtML


<!-- 参考信息 -->