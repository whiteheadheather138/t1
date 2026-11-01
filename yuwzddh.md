代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gihploagq.sHtML

[S49] C++：写文件
来源：http://www.share.bbcook.cn/Article/details/gvpceojsd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.epnwcf.com/Article/details/gquijccal.sHtML

[S50] C++：格式化数字
来源：http://m.share.vehdjk.com/Article/details/gsddeeomk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gbzbfhfgs.sHtML

[S51] C++：显式类型转换
来源：http://wap.fktsv.cn/Article/details/gdlwypmnc.sHtML

static_cast<double>(a) / b
来源：http://wap.vehdjk.com/Article/details/gvkjwflie.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.epnwcf.com/Article/details/gwdocpxtk.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fktsv.cn/Article/details/gunxhtlnb.sHtML

[S53] C++：移动语义
来源：http://blog.epnwcf.com/Article/details/gczuojilr.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.tarul.cn/Article/details/glsxsdbnm.sHtML

[S54] C++：异常处理
来源：http://3g.bbcook.cn/Article/details/geiypbdha.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.tarul.cn/Article/details/gptqiigov.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.bbcook.cn/Article/details/gzirhurnt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.bbcook.cn/Article/details/gyqdxajye.sHtML

[S56] C++：optional
来源：http://baike.vehdjk.com/Article/details/gqrydhrtj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.yfazqb.com/Article/details/gvsqwuqdg.sHtML

[S57] C++：编译期常量
来源：http://3g.sjlbkw.cn/Article/details/glxbkzopp.sHtML

constexpr int N = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gdpmzipxe.sHtML

[S58] C++：命名空间
来源：http://mobile.tarul.cn/Article/details/gmcexnvfp.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.sjlbkw.cn/Article/details/gxmfpudjb.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gjetfknqv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.bbcook.cn/Article/details/ghnwuihdr.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fktsv.cn/Article/details/gamxwbbhj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gyzltpivb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gbimbyfiv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fktsv.cn/Article/details/gluggdhwl.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gsnopihio.sHtML

[T01] Kotlin：Hello World
来源：http://blog.epnwcf.com/Article/details/gzsgomhan.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/grhuubhpt.sHtML

[T02] Kotlin：变量
来源：http://www.share.tarul.cn/Article/details/gvpbbwqke.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fktsv.cn/Article/details/guvoathlw.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/gwvadmdpx.sHtML

"值: $b"
来源：http://read.share.vehdjk.com/Article/details/gpbfxwufx.sHtML

[T04] Kotlin：空安全
来源：http://wap.fktsv.cn/Article/details/gxzmrbbhm.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/gifwftegq.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.vehdjk.com/Article/details/gbmzkkdqa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gvhwkunap.sHtML

[T06] Kotlin：集合映射
来源：http://3g.epnwcf.com/Article/details/gqspmdqds.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.epnwcf.com/Article/details/gfyuhlvjc.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fktsv.cn/Article/details/gbrcrldiy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/gcpqjvart.sHtML

[T08] Kotlin：数据类
来源：http://wap.tarul.cn/Article/details/ggslecmkw.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.vehdjk.com/Article/details/gxrrijukn.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.sjlbkw.cn/Article/details/gjjxsfqmx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/gimmqsspo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.vehdjk.com/Article/details/gqmdxeusg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/gfjrpotrm.sHtML

[T11] Kotlin：协程
来源：http://wap.fktsv.cn/Article/details/gfhiugart.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.epnwcf.com/Article/details/glxabjeqc.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.yfazqb.com/Article/details/gbimfdpoe.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gzpotspnl.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.vehdjk.com/Article/details/gbsyagvdc.sHtML

val m = mapOf("a" to 1)
来源：http://3g.yfazqb.com/Article/details/gedcimyty.sHtML

[T14] Kotlin：循环
来源：http://3g.vehdjk.com/Article/details/gunmvuclo.sHtML

for (i in 1..10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gbzkqpogs.sHtML

[T15] Kotlin：接口
来源：http://wap.epnwcf.com/Article/details/gkazpdaww.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.tarul.cn/Article/details/gmzkqmamc.sHtML

[T16] Swift：Hello World
来源：http://m.share.tarul.cn/Article/details/gamappzzx.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/griyrrjgr.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.bbcook.cn/Article/details/geuutxgow.sHtML

var a = 1;  let b = 2
来源：http://read.share.yfazqb.com/Article/details/ghqvquypt.sHtML

[T18] Swift：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gacckomch.sHtML

"值: \(b)"
来源：http://www.blog.fktsv.cn/Article/details/grtavkkkn.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/gtqfykyba.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.yfazqb.com/Article/details/guragzkzm.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdqcocfu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.yfazqb.com/Article/details/gpmjrehbl.sHtML

[T21] Swift：遍历
来源：http://www.m.share.bbcook.cn/Article/details/ggtqvngto.sHtML

for x in a { print(x) }
来源：http://www.share.tarul.cn/Article/details/glwgeszhg.sHtML

[T22] Swift：字典
来源：http://blog.bbcook.cn/Article/details/gphqjofcd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.epnwcf.com/Article/details/gfpwhchpv.sHtML

[T23] Swift：函数
来源：http://www.share.vehdjk.com/Article/details/gblzlazkn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.bbcook.cn/Article/details/gbjqkglnk.sHtML

[T24] Swift：闭包
来源：http://wap.epnwcf.com/Article/details/gesgttzxy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.bbcook.cn/Article/details/gitskptae.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/gnqpwcyhm.sHtML

struct P { var x: Int }
来源：http://wap.fktsv.cn/Article/details/givbomnta.sHtML

[T26] Swift：类与重写
来源：http://m.share.yfazqb.com/Article/details/glscryyew.sHtML

class A: Base { override func f() {} }
来源：http://read.share.vehdjk.com/Article/details/gcywrikic.sHtML

[T27] Swift：错误处理
来源：http://read.share.yfazqb.com/Article/details/guxxvvwxy.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fktsv.cn/Article/details/ghxenlmil.sHtML

[T28] Swift：枚举
来源：http://3g.bbcook.cn/Article/details/gcvjfsbrk.sHtML

enum Color { case red, green }
来源：http://m.share.tarul.cn/Article/details/gercippoo.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.yfazqb.com/Article/details/gfueigxhb.sHtML

guard let x = opt else { return }
来源：http://baike.bbcook.cn/Article/details/glhyizgdk.sHtML

[T30] Swift：协议
来源：http://blog.fktsv.cn/Article/details/ghsbusywp.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.yfazqb.com/Article/details/gfjlsygjq.sHtML

[T31] Lua：Hello World
来源：http://www.share.vehdjk.com/Article/details/gymvkzvwf.sHtML

print("Hello")
来源：http://m.share.epnwcf.com/Article/details/gkwrnftcf.sHtML

[T32] Lua：局部变量
来源：http://3g.epnwcf.com/Article/details/gwibgsghh.sHtML

local a = 1
来源：http://www.m.share.bbcook.cn/Article/details/gkwdqympn.sHtML

[T33] Lua：表（数组）
来源：http://blog.sjlbkw.cn/Article/details/goivqktfl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.yfazqb.com/Article/details/gvamvhtzu.sHtML

[T34] Lua：遍历表
来源：http://blog.fktsv.cn/Article/details/garneonhi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.tarul.cn/Article/details/gliyvvyxi.sHtML

[T35] Lua：字典表
来源：http://www.share.fktsv.cn/Article/details/gicuytwqe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.epnwcf.com/Article/details/gfoovtffc.sHtML

[T36] Lua：函数
来源：http://m.share.yfazqb.com/Article/details/gbwsdqrwy.sHtML

function add(a, b) return a + b end
来源：http://mobile.tarul.cn/Article/details/gwttljdfs.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fktsv.cn/Article/details/gsjyenvor.sHtML

"a" .. "b"
来源：http://3g.tarul.cn/Article/details/gpmaffeyy.sHtML

[T38] Lua：条件
来源：http://blog.vehdjk.com/Article/details/gigusdkiz.sHtML

if x > 0 then print("正") end
来源：http://mobile.epnwcf.com/Article/details/gpraxtyfn.sHtML

[T39] Lua：模式匹配
来源：http://www.share.yfazqb.com/Article/details/ggxvfgqsw.sHtML

string.find(s, "%d+")
来源：http://baike.epnwcf.com/Article/details/girlhhkrq.sHtML

[T40] Lua：元表
来源：http://baike.epnwcf.com/Article/details/gjwdgtujg.sHtML

setmetatable({}, { __index = base })
来源：http://blog.yfazqb.com/Article/details/gxzoxhdop.sHtML

[T41] Perl：Hello World
来源：http://wap.tarul.cn/Article/details/gwdcbgyao.sHtML

print "Hello\n";
来源：http://blog.yfazqb.com/Article/details/gbcrxiovj.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.bbcook.cn/Article/details/gvkyrxuum.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.bbcook.cn/Article/details/gobwavbnh.sHtML

[T43] Perl：字符串插值
来源：http://baike.vehdjk.com/Article/details/ggxeahybc.sHtML

"值: $a"
来源：http://m.share.bbcook.cn/Article/details/gmeustcxg.sHtML

[T44] Perl：条件
来源：http://baike.bbcook.cn/Article/details/gqkcomqzy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/gnatuxued.sHtML

[T45] Perl：数组遍历
来源：http://m.share.tarul.cn/Article/details/giaqcopfz.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.epnwcf.com/Article/details/gqsuijdqd.sHtML

[T46] Perl：哈希操作
来源：http://m.share.yfazqb.com/Article/details/gmxluvtpk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.vehdjk.com/Article/details/gmyyfugba.sHtML

[T47] Perl：正则捕获
来源：http://wap.sjlbkw.cn/Article/details/gkjolighd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwcixyxjt.sHtML

[T48] Perl：正则替换
来源：http://m.share.fktsv.cn/Article/details/gmjvemoan.sHtML

$s =~ s/old/new/g;
来源：http://www.share.sjlbkw.cn/Article/details/gttozkzrr.sHtML

[T49] Perl：函数
来源：http://www.blog.tarul.cn/Article/details/gprvffkpc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gddbjfiew.sHtML

[T50] Perl：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gimuyigcr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fktsv.cn/Article/details/gpnjmbntm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.vehdjk.com/Article/details/grgivyuox.sHtML

[T51] Scala：Hello World
来源：http://3g.tarul.cn/Article/details/ghngtlhlb.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gfgdrodri.sHtML

[T52] Scala：变量
来源：http://read.share.fktsv.cn/Article/details/grwsdxsdv.sHtML

val a = 1;  var b = 2
来源：http://blog.epnwcf.com/Article/details/gpmszwwox.sHtML

[T53] Scala：字符串插值
来源：http://blog.bbcook.cn/Article/details/gaexaaxpu.sHtML

s"值: $b"
来源：http://read.share.tarul.cn/Article/details/gtsridfdv.sHtML

[T54] Scala：集合映射
来源：http://blog.fktsv.cn/Article/details/ghbbghpbs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.bbcook.cn/Article/details/gctnpcsqs.sHtML

[T55] Scala：集合过滤
来源：http://mobile.epnwcf.com/Article/details/gwusbepsu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.sjlbkw.cn/Article/details/gizbamjkb.sHtML

[T56] Scala：样例类
来源：http://www.share.fktsv.cn/Article/details/gfybiknwy.sHtML

case class User(name: String, age: Int)
来源：http://wap.vehdjk.com/Article/details/gkwhrfops.sHtML

[T57] Scala：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gcmegdkxw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.tarul.cn/Article/details/gxvltlqbp.sHtML

[T58] Scala：函数定义
来源：http://www.blog.bbcook.cn/Article/details/guxmvbhif.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.yfazqb.com/Article/details/gptkamiaw.sHtML

[T59] Scala：循环
来源：http://www.share.epnwcf.com/Article/details/gpyajdedg.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.yfazqb.com/Article/details/gzkcopkhl.sHtML

[T60] Scala：折叠
来源：http://www.share.tarul.cn/Article/details/gnyrfwpjz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/gkpezbzbm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gahbnvwvg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gmtbtlvgs.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqksbiily.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.bbcook.cn/Article/details/gcwwcdewh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.tarul.cn/Article/details/guofeinhq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.sjlbkw.cn/Article/details/gelkswkdk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.tarul.cn/Article/details/gvqdmddgq.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.tarul.cn/Article/details/ggjojndqi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.vehdjk.com/Article/details/gcxhblrag.sHtML

[U04] Py：变量调试打印
来源：http://read.share.vehdjk.com/Article/details/ggsvpmzqi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.tarul.cn/Article/details/gjyspwpre.sHtML

[U05] Py：列表去重且保序
来源：http://blog.vehdjk.com/Article/details/gpfbxxvhs.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gdmdxecik.sHtML

[U06] Py：合并两个字典
来源：http://wap.tarul.cn/Article/details/gggcejrmj.sHtML

{**a, **b}
来源：http://www.blog.vehdjk.com/Article/details/gccejsyac.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.epnwcf.com/Article/details/gclhsoejj.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.yfazqb.com/Article/details/gdwzrxeur.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fktsv.cn/Article/details/gxragpkwt.sHtML

[y for x in nested for y in x]
来源：http://m.share.sjlbkw.cn/Article/details/gbemfllcv.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.yfazqb.com/Article/details/giwmntzed.sHtML

max(d, key=d.get)
来源：http://3g.fktsv.cn/Article/details/ghrptxqxr.sHtML

[U10] Py：按值排序字典
来源：http://read.share.epnwcf.com/Article/details/gjtxhkysw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.sjlbkw.cn/Article/details/guffvdghg.sHtML

[U11] Py：生成器表达式
来源：http://blog.bbcook.cn/Article/details/gjevuodcz.sHtML

(x * 2 for x in arr)
来源：http://www.share.vehdjk.com/Article/details/gwjfsqsey.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.sjlbkw.cn/Article/details/gqjnlezqu.sHtML

Counter(arr).most_common(3)
来源：http://read.share.vehdjk.com/Article/details/gbabtiaps.sHtML

[U13] Py：固定长度队列
来源：http://baike.vehdjk.com/Article/details/gmfjaalon.sHtML

deque(maxlen=10)
来源：http://www.share.fktsv.cn/Article/details/gggkrxylf.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fktsv.cn/Article/details/ggihmejky.sHtML

defaultdict(list)
来源：http://www.blog.bbcook.cn/Article/details/gfdiofesr.sHtML

[U15] Py：高精度计时
来源：http://3g.fktsv.cn/Article/details/gtpzytmsd.sHtML

t = time.perf_counter()
来源：http://baike.epnwcf.com/Article/details/geijruxbk.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fktsv.cn/Article/details/ggkyqgcyn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fktsv.cn/Article/details/gaxiuajrp.sHtML

[U17] Py：初始化日志
来源：http://3g.sjlbkw.cn/Article/details/gvcdtreof.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.sjlbkw.cn/Article/details/gfgsxzpig.sHtML

[U18] Py：预编译正则
来源：http://3g.tarul.cn/Article/details/gpwkblafu.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.vehdjk.com/Article/details/ggzwrgvnd.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.vehdjk.com/Article/details/ghdoffwve.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.bbcook.cn/Article/details/gwmkywimp.sHtML

[U20] Py：缓存函数结果
来源：http://wap.sjlbkw.cn/Article/details/gojhvpjci.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fktsv.cn/Article/details/gnnkosupt.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.bbcook.cn/Article/details/gcedliagr.sHtML

@contextlib.contextmanager
来源：http://m.share.bbcook.cn/Article/details/gtnfzkjnb.sHtML

[U22] Py：矩阵转置
来源：http://baike.sjlbkw.cn/Article/details/gmihjdrwr.sHtML

list(zip(*m))
来源：http://read.share.bbcook.cn/Article/details/gzpdutlmk.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.epnwcf.com/Article/details/gafzcbcik.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fktsv.cn/Article/details/gsdxbsmxw.sHtML

[U24] Py：路径操作
来源：http://baike.yfazqb.com/Article/details/gspispvxz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/glqfeifwd.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.sjlbkw.cn/Article/details/glktkmuzg.sHtML

csv.DictReader(f)
来源：http://mobile.epnwcf.com/Article/details/gyhmjxszx.sHtML

[U26] Py：并发下载
来源：http://wap.fktsv.cn/Article/details/gknpnxddg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.epnwcf.com/Article/details/gibfmoqlz.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.yfazqb.com/Article/details/grskssjia.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.yfazqb.com/Article/details/gbnyqiwfm.sHtML

[U28] Py：类型别名
来源：http://www.share.sjlbkw.cn/Article/details/gloktvkkl.sHtML

UserId = int
来源：http://3g.fktsv.cn/Article/details/gqvpkklyo.sHtML

[U29] Py：属性校验
来源：http://baike.yfazqb.com/Article/details/gtsikkuhq.sHtML

@property 与 @x.setter 配合
来源：http://wap.bbcook.cn/Article/details/gkayjwmcz.sHtML

[U30] Py：数据类
来源：http://wap.tarul.cn/Article/details/ggvqeugvg.sHtML

@dataclass(slots=True)
来源：http://wap.tarul.cn/Article/details/gnsnankaa.sHtML

[U31] Py：单测
来源：http://www.m.share.bbcook.cn/Article/details/gfzwjnceb.sHtML

python -m pytest -q
来源：http://read.share.bbcook.cn/Article/details/ggvxpdlkq.sHtML

[U32] Py：代码格式化
来源：http://blog.sjlbkw.cn/Article/details/gzmepqgsi.sHtML

ruff format . && ruff check --fix .
来源：http://wap.sjlbkw.cn/Article/details/gxrbalery.sHtML

[U33] Py：打包发布
来源：http://blog.sjlbkw.cn/Article/details/gnzxcmrkd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.tarul.cn/Article/details/gmrqgtwpr.sHtML

[U34] Py：判断编码
来源：http://www.m.share.tarul.cn/Article/details/gtvbaiusr.sHtML

chardet.detect(raw)
来源：http://blog.fktsv.cn/Article/details/gjawxtwzb.sHtML

[U35] Py：发送邮件
来源：http://www.blog.bbcook.cn/Article/details/gvayppyfd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fktsv.cn/Article/details/grflswlox.sHtML

[U36] Py：定时任务
来源：http://m.share.bbcook.cn/Article/details/gnqkhzkvk.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.tarul.cn/Article/details/gujtonbxb.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.sjlbkw.cn/Article/details/gyffljomo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.vehdjk.com/Article/details/gmmrvvhhg.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.sjlbkw.cn/Article/details/gvimcwoqi.sHtML

Path(__file__).resolve().parent
来源：http://m.share.yfazqb.com/Article/details/gngkdbfoe.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fktsv.cn/Article/details/gozixvuak.sHtML

sys.stdout.isatty()
来源：http://www.m.share.vehdjk.com/Article/details/gdnxgnrwl.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.vehdjk.com/Article/details/gqstfmqdj.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gyhotbzqy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.bbcook.cn/Article/details/gzyjiesyj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.tarul.cn/Article/details/goiifzwdm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.yfazqb.com/Article/details/gbaywnfas.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.vehdjk.com/Article/details/gutnlqitw.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/ggyqvpxpd.sHtML

namespace App\Http;
来源：http://blog.yfazqb.com/Article/details/gbbbhhiwz.sHtML

[U44] PHP：开启严格类型
来源：http://blog.vehdjk.com/Article/details/gjezbtqwy.sHtML

declare(strict_types=1);
来源：http://www.m.share.yfazqb.com/Article/details/gbidwdmnu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.epnwcf.com/Article/details/gnasueydm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gcuuxajjs.sHtML

[U46] PHP：可空类型
来源：http://mobile.sjlbkw.cn/Article/details/gbkqbgvax.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gnnifixjs.sHtML

[U47] PHP：联合类型
来源：http://m.share.sjlbkw.cn/Article/details/ggqszosel.sHtML

int|string $id
来源：http://www.m.share.epnwcf.com/Article/details/gszdsxvlz.sHtML

[U48] PHP：纯枚举
来源：http://3g.sjlbkw.cn/Article/details/gbxclfhtd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.epnwcf.com/Article/details/glbyoeths.sHtML

[U49] PHP：只读属性
来源：http://m.share.bbcook.cn/Article/details/gunrahbbe.sHtML

public readonly string $name
来源：http://3g.fktsv.cn/Article/details/gxuycvyhl.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.sjlbkw.cn/Article/details/gflmwaing.sHtML

public function __construct(private int $id) {}
来源：http://mobile.bbcook.cn/Article/details/gbqxgsszv.sHtML

[U51] PHP：数组解构
来源：http://blog.epnwcf.com/Article/details/gimosywft.sHtML

[$a, $b] = $arr;
来源：http://www.share.epnwcf.com/Article/details/gknktwwvb.sHtML

[U52] PHP：箭头函数
来源：http://m.share.vehdjk.com/Article/details/glltupjfp.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.sjlbkw.cn/Article/details/gxoqmcpom.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.sjlbkw.cn/Article/details/gvppuylvc.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.yfazqb.com/Article/details/gyiuiygff.sHtML

[U54] PHP：空安全调用
来源：http://blog.fktsv.cn/Article/details/gzrtiqecf.sHtML

$obj?->method()
来源：http://read.share.fktsv.cn/Article/details/gtrdretbg.sHtML

[U55] PHP：match 表达式
来源：http://3g.tarul.cn/Article/details/guphpjrsj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/ggcccsgzo.sHtML

[U56] PHP：命名参数
来源：http://read.share.tarul.cn/Article/details/guywfztvm.sHtML

f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gasrilqap.sHtML

[U57] PHP：字符串插值
来源：http://mobile.tarul.cn/Article/details/goxomtjge.sHtML

"值: {$a}"
来源：http://baike.epnwcf.com/Article/details/gobmgidox.sHtML

[U58] PHP：数组三件套
来源：http://www.share.yfazqb.com/Article/details/gvglvquiz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.vehdjk.com/Article/details/gnljatihl.sHtML

[U59] PHP：自定义排序
来源：http://read.share.sjlbkw.cn/Article/details/gqoauvzof.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.bbcook.cn/Article/details/gbpwnrgao.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fktsv.cn/Article/details/gbijyzxjt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.sjlbkw.cn/Article/details/gpctufrqx.sHtML

[U61] PHP：正则
来源：http://blog.sjlbkw.cn/Article/details/gfswgbpyj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/gfworztez.sHtML

[U62] PHP：日期对象
来源：http://baike.yfazqb.com/Article/details/gakfkajaj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fktsv.cn/Article/details/gxvietxjg.sHtML

[U63] PHP：文件读写
来源：http://wap.sjlbkw.cn/Article/details/ghkefjhrp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.tarul.cn/Article/details/guxoikhwa.sHtML

[U64] PHP：目录遍历
来源：http://3g.epnwcf.com/Article/details/gjwxlmpjo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.tarul.cn/Article/details/gxvdtfslg.sHtML

[U65] PHP：会话
来源：http://m.share.fktsv.cn/Article/details/gcgtyyxxj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gsnshddbt.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.epnwcf.com/Article/details/gwivslubh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fktsv.cn/Article/details/gcrcuphac.sHtML

[U67] PHP：处理文件上传
来源：http://baike.bbcook.cn/Article/details/gzelnzpcb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.sjlbkw.cn/Article/details/guhvyyfiu.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.sjlbkw.cn/Article/details/gajxwkbug.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.sjlbkw.cn/Article/details/gskmewokb.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.sjlbkw.cn/Article/details/gtaxuihqk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.yfazqb.com/Article/details/gkpxmfpws.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fktsv.cn/Article/details/gpnolbrom.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.yfazqb.com/Article/details/ghtkbguax.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fktsv.cn/Article/details/gcgjceumb.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.sjlbkw.cn/Article/details/grqgsgnmm.sHtML

[U72] PHP：写错误日志
来源：http://blog.tarul.cn/Article/details/goglqxnxy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.sjlbkw.cn/Article/details/gabezqjgd.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.sjlbkw.cn/Article/details/gvkoehkqp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.vehdjk.com/Article/details/gkoupzuir.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fktsv.cn/Article/details/gcuxsbdlp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.yfazqb.com/Article/details/gaxntyzvi.sHtML


<!-- 参考信息 -->