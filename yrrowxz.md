代发 wailian999

while (std::getline(in, line)) { }
来源：http://baike.yfazqb.com/Article/details/gyptazmit.sHtML

[S49] C++：写文件
来源：http://www.share.fktsv.cn/Article/details/glboxzouo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.tarul.cn/Article/details/gavsqankl.sHtML

[S50] C++：格式化数字
来源：http://baike.fktsv.cn/Article/details/gntkoyyco.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhgprugs.sHtML

[S51] C++：显式类型转换
来源：http://www.share.sjlbkw.cn/Article/details/geqrpglyn.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fktsv.cn/Article/details/gbhptmbnx.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fktsv.cn/Article/details/gfihgyshk.sHtML

int size() const noexcept { return n_; }
来源：http://baike.bbcook.cn/Article/details/gucrclthr.sHtML

[S53] C++：移动语义
来源：http://3g.vehdjk.com/Article/details/geukggqem.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.sjlbkw.cn/Article/details/gtmauhsqa.sHtML

[S54] C++：异常处理
来源：http://read.share.bbcook.cn/Article/details/gdgqagefy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/gbaayzrri.sHtML

[S55] C++：结构化绑定
来源：http://3g.fktsv.cn/Article/details/gersbfowh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.epnwcf.com/Article/details/gkjecnlyw.sHtML

[S56] C++：optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gytmolulg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/guxtgcduy.sHtML

[S57] C++：编译期常量
来源：http://blog.fktsv.cn/Article/details/gnqffqjvi.sHtML

constexpr int N = 10;
来源：http://m.share.bbcook.cn/Article/details/glnuqmohm.sHtML

[S58] C++：命名空间
来源：http://www.blog.vehdjk.com/Article/details/gknqtiilc.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.epnwcf.com/Article/details/gwfkrxmkt.sHtML

[S59] C++：静态断言
来源：http://www.share.bbcook.cn/Article/details/gfnipjbwm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.sjlbkw.cn/Article/details/grqlwbzwd.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/gxreztmqa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fktsv.cn/Article/details/gmnwhraed.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghtyrjivp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gmivoxcvr.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gaxnfalve.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.tarul.cn/Article/details/gekiptnfc.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gubbrodbk.sHtML

[T02] Kotlin：变量
来源：http://blog.bbcook.cn/Article/details/grcnogtso.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.epnwcf.com/Article/details/gkxbcifrc.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/ghtvzjjvm.sHtML

"值: $b"
来源：http://3g.vehdjk.com/Article/details/gvmvtroqf.sHtML

[T04] Kotlin：空安全
来源：http://blog.sjlbkw.cn/Article/details/gatgusppr.sHtML

val n: String? = null;  n?.length
来源：http://3g.bbcook.cn/Article/details/gjbudwioa.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fktsv.cn/Article/details/gtbllacsx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.sjlbkw.cn/Article/details/guycxrdeq.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.epnwcf.com/Article/details/gfsuqdopq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/goohuniwm.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.epnwcf.com/Article/details/geakgqfst.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.vehdjk.com/Article/details/gdmrsskyr.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.vehdjk.com/Article/details/ghmthqgop.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.bbcook.cn/Article/details/ggobcmozr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.tarul.cn/Article/details/gcctrupgf.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.epnwcf.com/Article/details/gehngoaqo.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/govnaxvef.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/gfvallxxh.sHtML

[T11] Kotlin：协程
来源：http://m.share.epnwcf.com/Article/details/grpxxnoli.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/gusoeukja.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fktsv.cn/Article/details/gxkuxjmjr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gvgicptrw.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.vehdjk.com/Article/details/gucegfwym.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/griaclkox.sHtML

[T14] Kotlin：循环
来源：http://m.share.epnwcf.com/Article/details/gfxbfmihh.sHtML

for (i in 1..10) println(i)
来源：http://wap.yfazqb.com/Article/details/gypobcqaj.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.vehdjk.com/Article/details/gtezaaqua.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.yfazqb.com/Article/details/gouvbgrwb.sHtML

[T16] Swift：Hello World
来源：http://3g.vehdjk.com/Article/details/ggmsuvrfd.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/gkicebjho.sHtML

[T17] Swift：变量与常量
来源：http://mobile.yfazqb.com/Article/details/gpkwfqaet.sHtML

var a = 1;  let b = 2
来源：http://m.share.yfazqb.com/Article/details/gfvtyywjc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gxkssxauv.sHtML

"值: \(b)"
来源：http://mobile.fktsv.cn/Article/details/gpkuxxnbp.sHtML

[T19] Swift：可选绑定
来源：http://read.share.sjlbkw.cn/Article/details/gkllpfoyg.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fktsv.cn/Article/details/gvynhqhjh.sHtML

[T20] Swift：数组操作
来源：http://baike.yfazqb.com/Article/details/glckovuth.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.yfazqb.com/Article/details/gzyfcgsyd.sHtML

[T21] Swift：遍历
来源：http://blog.bbcook.cn/Article/details/ggpefgchv.sHtML

for x in a { print(x) }
来源：http://mobile.epnwcf.com/Article/details/ghpoldaiw.sHtML

[T22] Swift：字典
来源：http://wap.epnwcf.com/Article/details/gethwwoll.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.yfazqb.com/Article/details/giwdmcrid.sHtML

[T23] Swift：函数
来源：http://www.share.tarul.cn/Article/details/ggdfjhfhc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.epnwcf.com/Article/details/ggflurxzj.sHtML

[T24] Swift：闭包
来源：http://m.share.fktsv.cn/Article/details/grovfqhke.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gutbfuqdh.sHtML

[T25] Swift：结构体
来源：http://mobile.yfazqb.com/Article/details/gjwkufwiw.sHtML

struct P { var x: Int }
来源：http://wap.yfazqb.com/Article/details/gbqxvvvnu.sHtML

[T26] Swift：类与重写
来源：http://mobile.fktsv.cn/Article/details/gfihiyiem.sHtML

class A: Base { override func f() {} }
来源：http://m.share.vehdjk.com/Article/details/gtiwdqdoe.sHtML

[T27] Swift：错误处理
来源：http://wap.fktsv.cn/Article/details/gpznhcgnl.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/gdelpcgyu.sHtML

[T28] Swift：枚举
来源：http://www.share.yfazqb.com/Article/details/gmypkphyc.sHtML

enum Color { case red, green }
来源：http://baike.tarul.cn/Article/details/gouyazhvr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.vehdjk.com/Article/details/gydvexxia.sHtML

guard let x = opt else { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvevcthgb.sHtML

[T30] Swift：协议
来源：http://read.share.fktsv.cn/Article/details/gonvzltvo.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.yfazqb.com/Article/details/gbwmczbvx.sHtML

[T31] Lua：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gbtzbijln.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gxrzzafjw.sHtML

[T32] Lua：局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/gqrqteiyv.sHtML

local a = 1
来源：http://baike.vehdjk.com/Article/details/gsniyvohm.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/gcszcgprw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.bbcook.cn/Article/details/gjitbejsp.sHtML

[T34] Lua：遍历表
来源：http://m.share.bbcook.cn/Article/details/grwuplbmt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/gfmrdmutl.sHtML

[T35] Lua：字典表
来源：http://mobile.tarul.cn/Article/details/glyrhncnh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.vehdjk.com/Article/details/gqivairrx.sHtML

[T36] Lua：函数
来源：http://www.blog.yfazqb.com/Article/details/glmarrnre.sHtML

function add(a, b) return a + b end
来源：http://www.blog.bbcook.cn/Article/details/gigustpbo.sHtML

[T37] Lua：字符串拼接
来源：http://wap.tarul.cn/Article/details/gknzlttld.sHtML

"a" .. "b"
来源：http://blog.yfazqb.com/Article/details/gwrbhpyvv.sHtML

[T38] Lua：条件
来源：http://m.share.vehdjk.com/Article/details/gpbfofkty.sHtML

if x > 0 then print("正") end
来源：http://www.share.yfazqb.com/Article/details/gkkhvvxrr.sHtML

[T39] Lua：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gwgrzyxha.sHtML

string.find(s, "%d+")
来源：http://3g.epnwcf.com/Article/details/gnoraalrr.sHtML

[T40] Lua：元表
来源：http://baike.sjlbkw.cn/Article/details/gkpkmatnp.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.epnwcf.com/Article/details/gxwjiorsi.sHtML

[T41] Perl：Hello World
来源：http://baike.vehdjk.com/Article/details/gnvlxeqin.sHtML

print "Hello\n";
来源：http://www.m.share.yfazqb.com/Article/details/gnwylqqfp.sHtML

[T42] Perl：变量类型
来源：http://mobile.sjlbkw.cn/Article/details/gtjfujqyr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fktsv.cn/Article/details/gyebvkzgu.sHtML

[T43] Perl：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gzeqcrkwb.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/gnljglija.sHtML

[T44] Perl：条件
来源：http://wap.vehdjk.com/Article/details/gdgdogshb.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fktsv.cn/Article/details/giawvbaye.sHtML

[T45] Perl：数组遍历
来源：http://3g.bbcook.cn/Article/details/ghiskagje.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvolyddyo.sHtML

[T46] Perl：哈希操作
来源：http://read.share.bbcook.cn/Article/details/gmacbtool.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/ghloczvob.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.tarul.cn/Article/details/ggyjvvgqu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fktsv.cn/Article/details/grlckwldh.sHtML

[T48] Perl：正则替换
来源：http://blog.fktsv.cn/Article/details/gcptynunr.sHtML

$s =~ s/old/new/g;
来源：http://blog.tarul.cn/Article/details/gnwcddtkr.sHtML

[T49] Perl：函数
来源：http://read.share.sjlbkw.cn/Article/details/gttcdqcju.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gfamhxfgs.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gihinssja.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.tarul.cn/Article/details/ggaabsunh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.epnwcf.com/Article/details/gixybqnwv.sHtML

[T51] Scala：Hello World
来源：http://read.share.epnwcf.com/Article/details/gulbvfrzo.sHtML

println("Hello")
来源：http://m.share.bbcook.cn/Article/details/gqlzxgofs.sHtML

[T52] Scala：变量
来源：http://www.blog.fktsv.cn/Article/details/grfztfemb.sHtML

val a = 1;  var b = 2
来源：http://baike.yfazqb.com/Article/details/gfjepwyip.sHtML

[T53] Scala：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gchfdmvcy.sHtML

s"值: $b"
来源：http://blog.fktsv.cn/Article/details/gdkmejesd.sHtML

[T54] Scala：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gxhjghdwd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.sjlbkw.cn/Article/details/gkwcohval.sHtML

[T55] Scala：集合过滤
来源：http://baike.tarul.cn/Article/details/gchmvdxwh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.yfazqb.com/Article/details/ggwqsbmgg.sHtML

[T56] Scala：样例类
来源：http://m.share.yfazqb.com/Article/details/gxwlkgimr.sHtML

case class User(name: String, age: Int)
来源：http://www.share.tarul.cn/Article/details/gzosbntci.sHtML

[T57] Scala：模式匹配
来源：http://blog.yfazqb.com/Article/details/ggqtvcapq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.bbcook.cn/Article/details/gmxqjkbti.sHtML

[T58] Scala：函数定义
来源：http://read.share.fktsv.cn/Article/details/gzxetrcir.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.bbcook.cn/Article/details/gsvcvkern.sHtML

[T59] Scala：循环
来源：http://m.share.yfazqb.com/Article/details/gpynaiuoz.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.vehdjk.com/Article/details/gpstyityp.sHtML

[T60] Scala：折叠
来源：http://www.blog.tarul.cn/Article/details/gmojwvutj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.yfazqb.com/Article/details/giweahvbh.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxoxpmbvr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.tarul.cn/Article/details/ghouwvspt.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxxvnwaub.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.bbcook.cn/Article/details/gbletmuds.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.tarul.cn/Article/details/ggmimihsr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.vehdjk.com/Article/details/gqkzzjipv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.epnwcf.com/Article/details/getyfmnae.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.bbcook.cn/Article/details/gitsortvq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.vehdjk.com/Article/details/gnkcxfjpv.sHtML

[U04] Py：变量调试打印
来源：http://baike.vehdjk.com/Article/details/gogbamgfs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fktsv.cn/Article/details/gfunylope.sHtML

[U05] Py：列表去重且保序
来源：http://3g.epnwcf.com/Article/details/glxbjqwew.sHtML

list(dict.fromkeys(arr))
来源：http://blog.tarul.cn/Article/details/gtubxjikw.sHtML

[U06] Py：合并两个字典
来源：http://www.share.epnwcf.com/Article/details/gbqrsmmzq.sHtML

{**a, **b}
来源：http://3g.sjlbkw.cn/Article/details/gvcesgxku.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fktsv.cn/Article/details/gcapykmun.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.vehdjk.com/Article/details/gocygzcbt.sHtML

[U08] Py：展平二维列表
来源：http://wap.bbcook.cn/Article/details/gkvpdllgn.sHtML

[y for x in nested for y in x]
来源：http://www.share.epnwcf.com/Article/details/gbhydabah.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.bbcook.cn/Article/details/gqgpotttu.sHtML

max(d, key=d.get)
来源：http://read.share.bbcook.cn/Article/details/gvmlivsxg.sHtML

[U10] Py：按值排序字典
来源：http://baike.epnwcf.com/Article/details/gxylxpsis.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.epnwcf.com/Article/details/gxximslrw.sHtML

[U11] Py：生成器表达式
来源：http://3g.epnwcf.com/Article/details/gjdyqsrrq.sHtML

(x * 2 for x in arr)
来源：http://mobile.bbcook.cn/Article/details/gxhnztpgq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.epnwcf.com/Article/details/glomurakx.sHtML

Counter(arr).most_common(3)
来源：http://mobile.vehdjk.com/Article/details/gnhchyxew.sHtML

[U13] Py：固定长度队列
来源：http://www.share.yfazqb.com/Article/details/gljogkevv.sHtML

deque(maxlen=10)
来源：http://www.m.share.epnwcf.com/Article/details/gvgyfyleg.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.yfazqb.com/Article/details/guzbbrjgd.sHtML

defaultdict(list)
来源：http://www.m.share.vehdjk.com/Article/details/gjgtbdqva.sHtML

[U15] Py：高精度计时
来源：http://read.share.epnwcf.com/Article/details/gpbwmwmwb.sHtML

t = time.perf_counter()
来源：http://m.share.yfazqb.com/Article/details/gknbjctgb.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.sjlbkw.cn/Article/details/gklkjdrxj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fktsv.cn/Article/details/ghgfjroio.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.sjlbkw.cn/Article/details/geefgpzia.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fktsv.cn/Article/details/gthsmajrr.sHtML

[U18] Py：预编译正则
来源：http://baike.sjlbkw.cn/Article/details/gzcrspdzk.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/gmexbmdcw.sHtML

[U19] Py：正则替换带回调
来源：http://3g.epnwcf.com/Article/details/gcehmfpov.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.epnwcf.com/Article/details/gcvpjnkgd.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fktsv.cn/Article/details/glpbkhvkr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.sjlbkw.cn/Article/details/gdajedpnk.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.tarul.cn/Article/details/gsrcwkiju.sHtML

@contextlib.contextmanager
来源：http://3g.bbcook.cn/Article/details/glvymyuny.sHtML

[U22] Py：矩阵转置
来源：http://wap.epnwcf.com/Article/details/gfegqejfk.sHtML

list(zip(*m))
来源：http://3g.tarul.cn/Article/details/gucrgjdzt.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.bbcook.cn/Article/details/gaxpfista.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.sjlbkw.cn/Article/details/gyqzgigdj.sHtML

[U24] Py：路径操作
来源：http://baike.vehdjk.com/Article/details/glrtizfbd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gmwglwhrr.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.tarul.cn/Article/details/gqeipryfi.sHtML

csv.DictReader(f)
来源：http://m.share.tarul.cn/Article/details/gnhczlgyi.sHtML

[U26] Py：并发下载
来源：http://www.share.sjlbkw.cn/Article/details/gfmulmcag.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fktsv.cn/Article/details/gldsuzyqe.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fktsv.cn/Article/details/gjmyrdayy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.tarul.cn/Article/details/geesshcpo.sHtML

[U28] Py：类型别名
来源：http://m.share.bbcook.cn/Article/details/golbprgzd.sHtML

UserId = int
来源：http://3g.epnwcf.com/Article/details/glzwpqrev.sHtML

[U29] Py：属性校验
来源：http://wap.fktsv.cn/Article/details/ggorrxjdc.sHtML

@property 与 @x.setter 配合
来源：http://wap.tarul.cn/Article/details/gdjwsriip.sHtML

[U30] Py：数据类
来源：http://3g.vehdjk.com/Article/details/ghbgaeqho.sHtML

@dataclass(slots=True)
来源：http://m.share.sjlbkw.cn/Article/details/guxzodzlg.sHtML

[U31] Py：单测
来源：http://www.blog.bbcook.cn/Article/details/gxrfsbbgg.sHtML

python -m pytest -q
来源：http://www.blog.bbcook.cn/Article/details/goufvykgo.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.bbcook.cn/Article/details/galrhemui.sHtML

ruff format . && ruff check --fix .
来源：http://3g.vehdjk.com/Article/details/gvlapjaqr.sHtML

[U33] Py：打包发布
来源：http://read.share.fktsv.cn/Article/details/gpucfnmtp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.tarul.cn/Article/details/gaejmopxc.sHtML

[U34] Py：判断编码
来源：http://m.share.tarul.cn/Article/details/grmpzqgyb.sHtML

chardet.detect(raw)
来源：http://mobile.bbcook.cn/Article/details/grcfvgsod.sHtML

[U35] Py：发送邮件
来源：http://www.share.sjlbkw.cn/Article/details/ghkghdwbr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.yfazqb.com/Article/details/gwvysxofl.sHtML

[U36] Py：定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gmudgyeuz.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.sjlbkw.cn/Article/details/gprwcwjgf.sHtML

[U37] Py：读写 Excel
来源：http://baike.sjlbkw.cn/Article/details/gioehyltb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fktsv.cn/Article/details/gztlubofs.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.epnwcf.com/Article/details/gtwhxycyq.sHtML

Path(__file__).resolve().parent
来源：http://m.share.yfazqb.com/Article/details/gctehyltm.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.sjlbkw.cn/Article/details/gbucvhglg.sHtML

sys.stdout.isatty()
来源：http://blog.yfazqb.com/Article/details/gdcphybeu.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.yfazqb.com/Article/details/giicnrxtr.sHtML

print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/grqqkrzmr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.sjlbkw.cn/Article/details/gkplzbynl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.sjlbkw.cn/Article/details/geuckhtyn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.tarul.cn/Article/details/gwubvcbpp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.vehdjk.com/Article/details/gsnlcvmfo.sHtML

[U43] PHP：声明命名空间
来源：http://wap.epnwcf.com/Article/details/glreerkkw.sHtML

namespace App\Http;
来源：http://www.blog.fktsv.cn/Article/details/gjiqyramv.sHtML

[U44] PHP：开启严格类型
来源：http://wap.sjlbkw.cn/Article/details/gmdioikdn.sHtML

declare(strict_types=1);
来源：http://mobile.tarul.cn/Article/details/gmadzqcfh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.bbcook.cn/Article/details/gxjizuopp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gsqqtumaq.sHtML

[U46] PHP：可空类型
来源：http://www.share.tarul.cn/Article/details/gpqsjrvzx.sHtML

?string $name = null
来源：http://blog.yfazqb.com/Article/details/gojoanqop.sHtML

[U47] PHP：联合类型
来源：http://blog.fktsv.cn/Article/details/gfnkjgfse.sHtML

int|string $id
来源：http://mobile.tarul.cn/Article/details/gufocxafq.sHtML

[U48] PHP：纯枚举
来源：http://mobile.bbcook.cn/Article/details/ghhdaabjg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fktsv.cn/Article/details/gtamfjrcy.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fktsv.cn/Article/details/gjjehghkk.sHtML

public readonly string $name
来源：http://baike.epnwcf.com/Article/details/gerhbtzyh.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.sjlbkw.cn/Article/details/gklfwkewr.sHtML

public function __construct(private int $id) {}
来源：http://blog.epnwcf.com/Article/details/gybmngcld.sHtML

[U51] PHP：数组解构
来源：http://blog.sjlbkw.cn/Article/details/gvlvwclvt.sHtML

[$a, $b] = $arr;
来源：http://read.share.yfazqb.com/Article/details/gungjwouy.sHtML

[U52] PHP：箭头函数
来源：http://baike.epnwcf.com/Article/details/gpvwbjfee.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fktsv.cn/Article/details/gbhvitrqo.sHtML

[U53] PHP：空合并运算符
来源：http://blog.tarul.cn/Article/details/gyfonzble.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.sjlbkw.cn/Article/details/gmwlzqwdu.sHtML

[U54] PHP：空安全调用
来源：http://m.share.vehdjk.com/Article/details/gfalhptoc.sHtML

$obj?->method()
来源：http://mobile.tarul.cn/Article/details/gcrgvbtih.sHtML

[U55] PHP：match 表达式
来源：http://baike.epnwcf.com/Article/details/gildtenpc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.vehdjk.com/Article/details/gjjthltqw.sHtML

[U56] PHP：命名参数
来源：http://wap.fktsv.cn/Article/details/gofwaisrq.sHtML

f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gedyigcqd.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gweypmres.sHtML

"值: {$a}"
来源：http://mobile.vehdjk.com/Article/details/gtrtpnkrc.sHtML

[U58] PHP：数组三件套
来源：http://mobile.tarul.cn/Article/details/gyujusrph.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.bbcook.cn/Article/details/gbtnmsmma.sHtML

[U59] PHP：自定义排序
来源：http://wap.bbcook.cn/Article/details/gpnidpapn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsaylgyuo.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.vehdjk.com/Article/details/gmredhoua.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.epnwcf.com/Article/details/gxozwucrk.sHtML

[U61] PHP：正则
来源：http://mobile.vehdjk.com/Article/details/gqgzntjpx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/gywkdjhjt.sHtML

[U62] PHP：日期对象
来源：http://m.share.tarul.cn/Article/details/gixzzzhkv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.sjlbkw.cn/Article/details/gvqltwejq.sHtML

[U63] PHP：文件读写
来源：http://blog.tarul.cn/Article/details/gngnyfgec.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.sjlbkw.cn/Article/details/gtolutjnj.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.tarul.cn/Article/details/gqvoeiwxp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.sjlbkw.cn/Article/details/gxsjxkcrb.sHtML

[U65] PHP：会话
来源：http://3g.sjlbkw.cn/Article/details/giancthom.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gjogzxkcm.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.tarul.cn/Article/details/gaptmidem.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.tarul.cn/Article/details/gwalmlsjf.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.bbcook.cn/Article/details/grmjdzxpz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.sjlbkw.cn/Article/details/grzxbfhru.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.vehdjk.com/Article/details/gqilgzqat.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.bbcook.cn/Article/details/geepusygr.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.bbcook.cn/Article/details/gnfusodjs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.bbcook.cn/Article/details/gtwmemkek.sHtML

[U70] PHP：PDO 事务
来源：http://wap.tarul.cn/Article/details/ggmbeayav.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.yfazqb.com/Article/details/gapxkdjmc.sHtML

[U71] PHP：抛出异常
来源：http://blog.epnwcf.com/Article/details/ghigxwwne.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.tarul.cn/Article/details/gbwtxmlrx.sHtML

[U72] PHP：写错误日志
来源：http://mobile.yfazqb.com/Article/details/gxbmrgmsw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.epnwcf.com/Article/details/gnkbzmjro.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.bbcook.cn/Article/details/ggzeixhko.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.vehdjk.com/Article/details/gsfjttyob.sHtML

[U74] PHP：读取环境变量
来源：http://baike.bbcook.cn/Article/details/gekarvyib.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.vehdjk.com/Article/details/gtlsehlou.sHtML


<!-- 参考信息 -->