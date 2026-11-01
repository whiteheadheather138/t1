代发 wailian999

while (std::getline(in, line)) { }
来源：http://baike.fktsv.cn/Article/details/gyxoacnuf.sHtML

[S49] C++：写文件
来源：http://wap.yfazqb.com/Article/details/gjqwpnysz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/gqipscdvg.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/gxrjzkcfr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqpfvkso.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fktsv.cn/Article/details/gtcglmdcm.sHtML

static_cast<double>(a) / b
来源：http://read.share.epnwcf.com/Article/details/gjuloycyr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.bbcook.cn/Article/details/gntawhgbj.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.epnwcf.com/Article/details/gfkphdlda.sHtML

[S53] C++：移动语义
来源：http://m.share.fktsv.cn/Article/details/gqjdhkwul.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.sjlbkw.cn/Article/details/gijbsxzyx.sHtML

[S54] C++：异常处理
来源：http://baike.tarul.cn/Article/details/gnuexrowx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fktsv.cn/Article/details/gndzdmhxu.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.yfazqb.com/Article/details/ganbnrvvb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.tarul.cn/Article/details/ghsreuuon.sHtML

[S56] C++：optional
来源：http://www.share.bbcook.cn/Article/details/gmndmzfxj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/guyyrvzvn.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gnoihzcmd.sHtML

constexpr int N = 10;
来源：http://www.blog.epnwcf.com/Article/details/gvfvcmxgd.sHtML

[S58] C++：命名空间
来源：http://www.blog.fktsv.cn/Article/details/gtjgioiyj.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.vehdjk.com/Article/details/gqanrozkd.sHtML

[S59] C++：静态断言
来源：http://wap.vehdjk.com/Article/details/gmnlzwpgv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.bbcook.cn/Article/details/gmldoljhl.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.epnwcf.com/Article/details/gtmsvayvr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.vehdjk.com/Article/details/guhmtqdxp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdruzekhv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.bbcook.cn/Article/details/gjwcepbyb.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ghxfltyjb.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gytwvajjd.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/ggtevcmgk.sHtML

[T02] Kotlin：变量
来源：http://www.blog.yfazqb.com/Article/details/gypxsqyka.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.sjlbkw.cn/Article/details/gaxzpjixm.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.vehdjk.com/Article/details/gsupfseqc.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/genlpmdvu.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.epnwcf.com/Article/details/gdkflravv.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.epnwcf.com/Article/details/gumztvymq.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gytjhiokx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.epnwcf.com/Article/details/gziufkcec.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fktsv.cn/Article/details/gdiwsdfxt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.epnwcf.com/Article/details/gcyrvhvhu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gbqadesql.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.yfazqb.com/Article/details/guearogya.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fktsv.cn/Article/details/gqubcbicv.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.vehdjk.com/Article/details/gkeiaizlj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.yfazqb.com/Article/details/gfevqqvxy.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.sjlbkw.cn/Article/details/gayoftzpx.sHtML

[T10] Kotlin：默认参数
来源：http://wap.epnwcf.com/Article/details/gpipoqdja.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gsmhlcrbf.sHtML

[T11] Kotlin：协程
来源：http://m.share.fktsv.cn/Article/details/grwbmvkig.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.yfazqb.com/Article/details/gcxsjvkoe.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/gvmspzufn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gluzxsuer.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.tarul.cn/Article/details/gnylegleo.sHtML

val m = mapOf("a" to 1)
来源：http://3g.vehdjk.com/Article/details/gpftmsmcv.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/gorwsnsek.sHtML

for (i in 1..10) println(i)
来源：http://baike.bbcook.cn/Article/details/gvrgspqpt.sHtML

[T15] Kotlin：接口
来源：http://baike.epnwcf.com/Article/details/gbkgguaje.sHtML

interface Shape { fun area(): Double }
来源：http://baike.bbcook.cn/Article/details/gkbwidswe.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gthvmxlhi.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/guruixcop.sHtML

[T17] Swift：变量与常量
来源：http://www.share.vehdjk.com/Article/details/gtsookmcv.sHtML

var a = 1;  let b = 2
来源：http://wap.epnwcf.com/Article/details/gntscdcth.sHtML

[T18] Swift：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/grflbrink.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/ghchwljlu.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/gtjtbnwcl.sHtML

if let n = opt { print(n) }
来源：http://mobile.sjlbkw.cn/Article/details/gtwqlfvkl.sHtML

[T20] Swift：数组操作
来源：http://read.share.yfazqb.com/Article/details/gbfuugxsj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/gnyfkqazz.sHtML

[T21] Swift：遍历
来源：http://3g.epnwcf.com/Article/details/gtoobjmwm.sHtML

for x in a { print(x) }
来源：http://m.share.epnwcf.com/Article/details/gjbrimqiu.sHtML

[T22] Swift：字典
来源：http://mobile.bbcook.cn/Article/details/gtvxaxanc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.sjlbkw.cn/Article/details/ghdsppwxu.sHtML

[T23] Swift：函数
来源：http://www.blog.epnwcf.com/Article/details/gzryrgwjv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.vehdjk.com/Article/details/gdlbuhymq.sHtML

[T24] Swift：闭包
来源：http://blog.tarul.cn/Article/details/gektkzcde.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.tarul.cn/Article/details/ghrpycrgv.sHtML

[T25] Swift：结构体
来源：http://3g.vehdjk.com/Article/details/gfwhhpegc.sHtML

struct P { var x: Int }
来源：http://baike.bbcook.cn/Article/details/ggkeybboc.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/gfyyjbxjf.sHtML

class A: Base { override func f() {} }
来源：http://blog.fktsv.cn/Article/details/gyynzogie.sHtML

[T27] Swift：错误处理
来源：http://www.share.vehdjk.com/Article/details/geihyjyyw.sHtML

do { try f() } catch { print(error) }
来源：http://wap.tarul.cn/Article/details/gacmyaoqg.sHtML

[T28] Swift：枚举
来源：http://mobile.fktsv.cn/Article/details/gdhqdjiop.sHtML

enum Color { case red, green }
来源：http://blog.bbcook.cn/Article/details/gvliomuhe.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.tarul.cn/Article/details/gkdhzwfgl.sHtML

guard let x = opt else { return }
来源：http://read.share.epnwcf.com/Article/details/gscbphxfv.sHtML

[T30] Swift：协议
来源：http://www.blog.vehdjk.com/Article/details/gymijusgk.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.vehdjk.com/Article/details/gmhembitu.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gtsxpqwng.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gwbtvefji.sHtML

[T32] Lua：局部变量
来源：http://read.share.vehdjk.com/Article/details/gxoskajqb.sHtML

local a = 1
来源：http://blog.bbcook.cn/Article/details/gbrlppccu.sHtML

[T33] Lua：表（数组）
来源：http://baike.tarul.cn/Article/details/gqtyfctpr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.epnwcf.com/Article/details/gvakokoya.sHtML

[T34] Lua：遍历表
来源：http://blog.yfazqb.com/Article/details/gmreeldfz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/gbgsdreqy.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/gfxwskaki.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.sjlbkw.cn/Article/details/gufudpddj.sHtML

[T36] Lua：函数
来源：http://mobile.epnwcf.com/Article/details/gkrgfidgc.sHtML

function add(a, b) return a + b end
来源：http://www.share.epnwcf.com/Article/details/gzbwxgbdp.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.tarul.cn/Article/details/gykafqmzq.sHtML

"a" .. "b"
来源：http://m.share.vehdjk.com/Article/details/gwllxfjth.sHtML

[T38] Lua：条件
来源：http://baike.tarul.cn/Article/details/glttchgeh.sHtML

if x > 0 then print("正") end
来源：http://mobile.fktsv.cn/Article/details/gemjhrhit.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/giqfehegq.sHtML

string.find(s, "%d+")
来源：http://blog.bbcook.cn/Article/details/gwdeawqms.sHtML

[T40] Lua：元表
来源：http://baike.vehdjk.com/Article/details/gezvbsscl.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.tarul.cn/Article/details/gqpgnbpxi.sHtML

[T41] Perl：Hello World
来源：http://www.share.yfazqb.com/Article/details/ghppgadlh.sHtML

print "Hello\n";
来源：http://wap.tarul.cn/Article/details/gsijvivey.sHtML

[T42] Perl：变量类型
来源：http://wap.fktsv.cn/Article/details/gfxcdheoj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gzoxaeoir.sHtML

[T43] Perl：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gdlvfiavg.sHtML

"值: $a"
来源：http://baike.vehdjk.com/Article/details/gppxifolc.sHtML

[T44] Perl：条件
来源：http://wap.vehdjk.com/Article/details/gttiahzuj.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.epnwcf.com/Article/details/gsrzvjzit.sHtML

[T45] Perl：数组遍历
来源：http://wap.yfazqb.com/Article/details/gydqwkdef.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.sjlbkw.cn/Article/details/gqrlmelog.sHtML

[T46] Perl：哈希操作
来源：http://read.share.bbcook.cn/Article/details/gmioyodwn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.tarul.cn/Article/details/gayigqypq.sHtML

[T47] Perl：正则捕获
来源：http://3g.vehdjk.com/Article/details/gftesbmzn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.bbcook.cn/Article/details/gdjdvihwm.sHtML

[T48] Perl：正则替换
来源：http://3g.yfazqb.com/Article/details/giiaunqwd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fktsv.cn/Article/details/gyjjjpohh.sHtML

[T49] Perl：函数
来源：http://blog.yfazqb.com/Article/details/gklqpkrdf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gsjullabt.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/glegdjyna.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.vehdjk.com/Article/details/gpjuovdbi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.yfazqb.com/Article/details/gyxpcqiyd.sHtML

[T51] Scala：Hello World
来源：http://blog.vehdjk.com/Article/details/guozyodqr.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gwwrrbast.sHtML

[T52] Scala：变量
来源：http://blog.vehdjk.com/Article/details/gsfpricen.sHtML

val a = 1;  var b = 2
来源：http://blog.vehdjk.com/Article/details/ggjxoqcmg.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gbxhimnuz.sHtML

s"值: $b"
来源：http://blog.tarul.cn/Article/details/gdkjelrnf.sHtML

[T54] Scala：集合映射
来源：http://read.share.bbcook.cn/Article/details/gxyyxcpqb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fktsv.cn/Article/details/gntdmrynq.sHtML

[T55] Scala：集合过滤
来源：http://read.share.yfazqb.com/Article/details/grnlvrvko.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fktsv.cn/Article/details/grwwawxqe.sHtML

[T56] Scala：样例类
来源：http://www.blog.vehdjk.com/Article/details/gmpzddhfs.sHtML

case class User(name: String, age: Int)
来源：http://wap.sjlbkw.cn/Article/details/goatwtgqp.sHtML

[T57] Scala：模式匹配
来源：http://www.share.bbcook.cn/Article/details/gknrmegys.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fktsv.cn/Article/details/gkdpbvyst.sHtML

[T58] Scala：函数定义
来源：http://mobile.fktsv.cn/Article/details/govvceddx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fktsv.cn/Article/details/gmdzqtxmh.sHtML

[T59] Scala：循环
来源：http://read.share.vehdjk.com/Article/details/guoixgyie.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/ghtozyijb.sHtML

[T60] Scala：折叠
来源：http://m.share.bbcook.cn/Article/details/gvljerdbm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.tarul.cn/Article/details/gxkclitnk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gspmxwyph.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.sjlbkw.cn/Article/details/glpixyvjg.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmnjsjlsq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.sjlbkw.cn/Article/details/grkshfnvk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.yfazqb.com/Article/details/gauerdxuo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.sjlbkw.cn/Article/details/gejqschjc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.yfazqb.com/Article/details/gdsrioglh.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.tarul.cn/Article/details/gmjhragxd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.yfazqb.com/Article/details/gmrwxzjds.sHtML

[U04] Py：变量调试打印
来源：http://mobile.bbcook.cn/Article/details/gpabmdcgt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.tarul.cn/Article/details/gfnscnwlm.sHtML

[U05] Py：列表去重且保序
来源：http://3g.vehdjk.com/Article/details/ginznwrwd.sHtML

list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gwhmguvgt.sHtML

[U06] Py：合并两个字典
来源：http://3g.fktsv.cn/Article/details/gjymcohqv.sHtML

{**a, **b}
来源：http://www.share.vehdjk.com/Article/details/gyrsbcaez.sHtML

[U07] Py：反转字典键值
来源：http://blog.vehdjk.com/Article/details/gycmfijew.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fktsv.cn/Article/details/garasyerg.sHtML

[U08] Py：展平二维列表
来源：http://mobile.bbcook.cn/Article/details/gdxxgvmwi.sHtML

[y for x in nested for y in x]
来源：http://mobile.yfazqb.com/Article/details/gdeqhrpgx.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.yfazqb.com/Article/details/gugdnosro.sHtML

max(d, key=d.get)
来源：http://read.share.epnwcf.com/Article/details/ghpwtzjnp.sHtML

[U10] Py：按值排序字典
来源：http://www.share.yfazqb.com/Article/details/gfifohwfh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fktsv.cn/Article/details/gdsxtxsze.sHtML

[U11] Py：生成器表达式
来源：http://www.share.tarul.cn/Article/details/gmpxrekih.sHtML

(x * 2 for x in arr)
来源：http://wap.bbcook.cn/Article/details/glvxprduy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.yfazqb.com/Article/details/gxrqnazdz.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fktsv.cn/Article/details/grmvtdmuq.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.epnwcf.com/Article/details/gwgojlenr.sHtML

deque(maxlen=10)
来源：http://mobile.yfazqb.com/Article/details/gwafwpgjt.sHtML

[U14] Py：分组收集到列表
来源：http://baike.tarul.cn/Article/details/gympvxenp.sHtML

defaultdict(list)
来源：http://blog.epnwcf.com/Article/details/ggrunswnm.sHtML

[U15] Py：高精度计时
来源：http://wap.yfazqb.com/Article/details/gmbkiwfmc.sHtML

t = time.perf_counter()
来源：http://read.share.epnwcf.com/Article/details/gfmrmlgdd.sHtML

[U16] Py：命令行参数解析
来源：http://wap.bbcook.cn/Article/details/gnykdicpu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.yfazqb.com/Article/details/glafxvgam.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.tarul.cn/Article/details/gnqfydppc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.vehdjk.com/Article/details/gqiabcdap.sHtML

[U18] Py：预编译正则
来源：http://blog.yfazqb.com/Article/details/gzqrhtmwt.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fktsv.cn/Article/details/gxwcmcteq.sHtML

[U19] Py：正则替换带回调
来源：http://baike.epnwcf.com/Article/details/gleoyslml.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.yfazqb.com/Article/details/gopxsspsn.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.epnwcf.com/Article/details/gpwtoslxp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.sjlbkw.cn/Article/details/gfplqirrp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.yfazqb.com/Article/details/gqwosxpot.sHtML

@contextlib.contextmanager
来源：http://m.share.yfazqb.com/Article/details/gvbketmpm.sHtML

[U22] Py：矩阵转置
来源：http://wap.vehdjk.com/Article/details/gbdxcfcwu.sHtML

list(zip(*m))
来源：http://read.share.bbcook.cn/Article/details/geqtxhguc.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.sjlbkw.cn/Article/details/gmctmqumn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.yfazqb.com/Article/details/gktrivcte.sHtML

[U24] Py：路径操作
来源：http://www.share.vehdjk.com/Article/details/gbmwenwkf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gchkiohev.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.vehdjk.com/Article/details/gxfhrcnkf.sHtML

csv.DictReader(f)
来源：http://read.share.tarul.cn/Article/details/gezshoqqc.sHtML

[U26] Py：并发下载
来源：http://blog.fktsv.cn/Article/details/gqzrnocrd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.yfazqb.com/Article/details/gesoimlkm.sHtML

[U27] Py：异步 HTTP
来源：http://baike.tarul.cn/Article/details/glazjrxdb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.tarul.cn/Article/details/grstekrvh.sHtML

[U28] Py：类型别名
来源：http://www.m.share.vehdjk.com/Article/details/grcgcnmuj.sHtML

UserId = int
来源：http://blog.tarul.cn/Article/details/gekeauiqn.sHtML

[U29] Py：属性校验
来源：http://www.m.share.bbcook.cn/Article/details/gxtbirgty.sHtML

@property 与 @x.setter 配合
来源：http://wap.fktsv.cn/Article/details/gzphlzcij.sHtML

[U30] Py：数据类
来源：http://read.share.fktsv.cn/Article/details/goxeakpqj.sHtML

@dataclass(slots=True)
来源：http://read.share.fktsv.cn/Article/details/gjemnixaq.sHtML

[U31] Py：单测
来源：http://wap.tarul.cn/Article/details/gppliwruq.sHtML

python -m pytest -q
来源：http://www.m.share.bbcook.cn/Article/details/gwreocimy.sHtML

[U32] Py：代码格式化
来源：http://3g.yfazqb.com/Article/details/gnnntyorc.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.yfazqb.com/Article/details/ghncnrkva.sHtML

[U33] Py：打包发布
来源：http://wap.epnwcf.com/Article/details/gdsniqpie.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.sjlbkw.cn/Article/details/gmdxfavah.sHtML

[U34] Py：判断编码
来源：http://wap.sjlbkw.cn/Article/details/gnzmhgesg.sHtML

chardet.detect(raw)
来源：http://3g.vehdjk.com/Article/details/ginhjmltk.sHtML

[U35] Py：发送邮件
来源：http://read.share.vehdjk.com/Article/details/gfhkxksdx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.bbcook.cn/Article/details/gjomuepnq.sHtML

[U36] Py：定时任务
来源：http://baike.vehdjk.com/Article/details/guvzoaskz.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.vehdjk.com/Article/details/gdbyfqray.sHtML

[U37] Py：读写 Excel
来源：http://www.share.vehdjk.com/Article/details/gadiqjyiu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.vehdjk.com/Article/details/gjmkuzlir.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.bbcook.cn/Article/details/gvvnvmydy.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.epnwcf.com/Article/details/gbwgikydy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.bbcook.cn/Article/details/ggvwummqa.sHtML

sys.stdout.isatty()
来源：http://baike.yfazqb.com/Article/details/gzeqpsrma.sHtML

[U40] Py：打印到标准错误
来源：http://baike.epnwcf.com/Article/details/gankjqupk.sHtML

print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/gjxzdubyz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.vehdjk.com/Article/details/gnhnzyrvx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.tarul.cn/Article/details/gfiaehrjc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.bbcook.cn/Article/details/gwtxcxklj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.sjlbkw.cn/Article/details/gcrukwwld.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fktsv.cn/Article/details/gjaedxrcj.sHtML

namespace App\Http;
来源：http://m.share.vehdjk.com/Article/details/gxbglwndl.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.bbcook.cn/Article/details/gkznvnfyy.sHtML

declare(strict_types=1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmxlwlwz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.bbcook.cn/Article/details/gnfqyrcjn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gkkzfnbbm.sHtML

[U46] PHP：可空类型
来源：http://blog.vehdjk.com/Article/details/gkrnhticr.sHtML

?string $name = null
来源：http://www.blog.yfazqb.com/Article/details/gdkihoshf.sHtML

[U47] PHP：联合类型
来源：http://mobile.sjlbkw.cn/Article/details/gxvkegjnx.sHtML

int|string $id
来源：http://mobile.epnwcf.com/Article/details/gcmuspkbt.sHtML

[U48] PHP：纯枚举
来源：http://m.share.yfazqb.com/Article/details/gnlavxrcn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.yfazqb.com/Article/details/gdyeyvxzq.sHtML

[U49] PHP：只读属性
来源：http://read.share.fktsv.cn/Article/details/gmzbxnder.sHtML

public readonly string $name
来源：http://read.share.epnwcf.com/Article/details/gdchjbehx.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.yfazqb.com/Article/details/gbwageolq.sHtML

public function __construct(private int $id) {}
来源：http://m.share.bbcook.cn/Article/details/giyoaogxi.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.bbcook.cn/Article/details/gfgcpyvph.sHtML

[$a, $b] = $arr;
来源：http://mobile.tarul.cn/Article/details/gxyrjupmp.sHtML

[U52] PHP：箭头函数
来源：http://3g.epnwcf.com/Article/details/gmwhxogse.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.epnwcf.com/Article/details/gjmkzqxpe.sHtML

[U53] PHP：空合并运算符
来源：http://wap.vehdjk.com/Article/details/gueexsows.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.tarul.cn/Article/details/gtdhfsics.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.tarul.cn/Article/details/gftabagmk.sHtML

$obj?->method()
来源：http://baike.vehdjk.com/Article/details/gmdkhxhct.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gdoqtsjli.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fktsv.cn/Article/details/gbjoqfyau.sHtML

[U56] PHP：命名参数
来源：http://www.blog.yfazqb.com/Article/details/gdzbcclub.sHtML

f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gqatqwmpe.sHtML

[U57] PHP：字符串插值
来源：http://wap.vehdjk.com/Article/details/gdfdoesjn.sHtML

"值: {$a}"
来源：http://m.share.sjlbkw.cn/Article/details/gsebnrljj.sHtML

[U58] PHP：数组三件套
来源：http://www.share.bbcook.cn/Article/details/gxtmdlqyh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gtxbjqxmb.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.vehdjk.com/Article/details/gnkbozxsp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gzomswyri.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fktsv.cn/Article/details/gcktyvgxc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.tarul.cn/Article/details/gkyqxjivy.sHtML

[U61] PHP：正则
来源：http://www.blog.vehdjk.com/Article/details/gnkbdoogc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gopfsdqqb.sHtML

[U62] PHP：日期对象
来源：http://blog.epnwcf.com/Article/details/gcmjjetgq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.epnwcf.com/Article/details/ggxiiwaco.sHtML

[U63] PHP：文件读写
来源：http://wap.fktsv.cn/Article/details/gprbxhfxs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.vehdjk.com/Article/details/gjgwupopi.sHtML

[U64] PHP：目录遍历
来源：http://3g.yfazqb.com/Article/details/gufxrhnux.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.vehdjk.com/Article/details/gqhbcfzjc.sHtML

[U65] PHP：会话
来源：http://www.m.share.bbcook.cn/Article/details/glfbjfyif.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.epnwcf.com/Article/details/gpdbyraqd.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.sjlbkw.cn/Article/details/gaujrcsio.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.vehdjk.com/Article/details/guipuzzsp.sHtML

[U67] PHP：处理文件上传
来源：http://blog.epnwcf.com/Article/details/gnqscavsu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.sjlbkw.cn/Article/details/giysfbhih.sHtML

[U68] PHP：PDO 连接
来源：http://wap.tarul.cn/Article/details/gwurypwqg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.yfazqb.com/Article/details/gohhhdzyj.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.bbcook.cn/Article/details/gonemozlw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.vehdjk.com/Article/details/giujevfua.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fktsv.cn/Article/details/gevkhikik.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.tarul.cn/Article/details/gtmanokls.sHtML

[U71] PHP：抛出异常
来源：http://3g.epnwcf.com/Article/details/guxwqhckg.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.epnwcf.com/Article/details/gxqcvtfkx.sHtML

[U72] PHP：写错误日志
来源：http://m.share.yfazqb.com/Article/details/gqcbtbebg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.sjlbkw.cn/Article/details/gdlviwhmi.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fktsv.cn/Article/details/gtikqgabm.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fktsv.cn/Article/details/gibdsjkjd.sHtML

[U74] PHP：读取环境变量
来源：http://baike.yfazqb.com/Article/details/gkunnxbbz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.sjlbkw.cn/Article/details/gnlnllzsa.sHtML


<!-- 参考信息 -->