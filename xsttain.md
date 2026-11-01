代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.bbcook.cn/Article/details/ghktfltsj.sHtML

[S57] C++：编译期常量
来源：http://3g.yfazqb.com/Article/details/gkfswicrk.sHtML

constexpr int N = 10;
来源：http://read.share.fktsv.cn/Article/details/gswszmzjb.sHtML

[S58] C++：命名空间
来源：http://baike.sjlbkw.cn/Article/details/gkcirlbin.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/goyfsuria.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/gmoaqpguf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fktsv.cn/Article/details/gcbdgicbd.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.epnwcf.com/Article/details/gndsmsxcd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gldclrmea.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmsgwrjqj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzifcnnp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqmdzpsbd.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.yfazqb.com/Article/details/germwwkbp.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/ghxuzdznj.sHtML

[T02] Kotlin：变量
来源：http://m.share.yfazqb.com/Article/details/gdqjxpkpf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gofqfuknw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.yfazqb.com/Article/details/glvfizwtg.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gpsjrmibw.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gyxyfvfui.sHtML

val n: String? = null;  n?.length
来源：http://baike.vehdjk.com/Article/details/gdutkvwlx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gugjxhxya.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.tarul.cn/Article/details/gctmuszmt.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fktsv.cn/Article/details/gsctduxej.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.epnwcf.com/Article/details/gdazdbbcq.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gfljcnuun.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.vehdjk.com/Article/details/grccikcyk.sHtML

[T08] Kotlin：数据类
来源：http://wap.vehdjk.com/Article/details/gfcwjhunf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.tarul.cn/Article/details/gkfjuxjxg.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/ggouybmpf.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.bbcook.cn/Article/details/grbyexqgg.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.yfazqb.com/Article/details/gewpgmxxc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/gluglacax.sHtML

[T11] Kotlin：协程
来源：http://mobile.bbcook.cn/Article/details/gewlqaecq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.tarul.cn/Article/details/golpeoknx.sHtML

[T12] Kotlin：解构声明
来源：http://baike.vehdjk.com/Article/details/ggasrzyhm.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gmjkchykz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fktsv.cn/Article/details/grhanfiho.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.yfazqb.com/Article/details/gkrnuyzun.sHtML

[T14] Kotlin：循环
来源：http://wap.vehdjk.com/Article/details/gdwrknzkh.sHtML

for (i in 1..10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gtaahffmt.sHtML

[T15] Kotlin：接口
来源：http://www.share.sjlbkw.cn/Article/details/grpnyeiwp.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fktsv.cn/Article/details/gooxapuaf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gbkgvvtij.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gsrczysha.sHtML

[T17] Swift：变量与常量
来源：http://blog.vehdjk.com/Article/details/gomcftvvx.sHtML

var a = 1;  let b = 2
来源：http://www.share.fktsv.cn/Article/details/gwdrpkazv.sHtML

[T18] Swift：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gncyvqsqw.sHtML

"值: \(b)"
来源：http://wap.tarul.cn/Article/details/gznofwgkf.sHtML

[T19] Swift：可选绑定
来源：http://blog.sjlbkw.cn/Article/details/gluereivg.sHtML

if let n = opt { print(n) }
来源：http://wap.vehdjk.com/Article/details/gasdawlco.sHtML

[T20] Swift：数组操作
来源：http://blog.yfazqb.com/Article/details/gcxfbvcvf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.yfazqb.com/Article/details/griaouebb.sHtML

[T21] Swift：遍历
来源：http://www.m.share.vehdjk.com/Article/details/gncmhldkq.sHtML

for x in a { print(x) }
来源：http://www.share.epnwcf.com/Article/details/gdlionfky.sHtML

[T22] Swift：字典
来源：http://3g.fktsv.cn/Article/details/giiuxaewc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.bbcook.cn/Article/details/gwayfekfg.sHtML

[T23] Swift：函数
来源：http://www.m.share.yfazqb.com/Article/details/gbxzkvbyt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fktsv.cn/Article/details/ggtdsciyw.sHtML

[T24] Swift：闭包
来源：http://www.m.share.yfazqb.com/Article/details/gabjnqxuc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gdernwcja.sHtML

[T25] Swift：结构体
来源：http://www.m.share.vehdjk.com/Article/details/gyaphyimz.sHtML

struct P { var x: Int }
来源：http://www.blog.tarul.cn/Article/details/gdvbezgbq.sHtML

[T26] Swift：类与重写
来源：http://baike.sjlbkw.cn/Article/details/glvtpjfbk.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.tarul.cn/Article/details/gpaepwudw.sHtML

[T27] Swift：错误处理
来源：http://blog.epnwcf.com/Article/details/gyyhrzmxf.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.sjlbkw.cn/Article/details/gkhrrimyh.sHtML

[T28] Swift：枚举
来源：http://www.blog.fktsv.cn/Article/details/gvknlkkws.sHtML

enum Color { case red, green }
来源：http://wap.tarul.cn/Article/details/glpsmvcfr.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/gkvvdynfv.sHtML

guard let x = opt else { return }
来源：http://mobile.tarul.cn/Article/details/gavxlqxlf.sHtML

[T30] Swift：协议
来源：http://m.share.fktsv.cn/Article/details/gpuhunqil.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.epnwcf.com/Article/details/gifnufinr.sHtML

[T31] Lua：Hello World
来源：http://wap.bbcook.cn/Article/details/gfoaijawh.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/grwbmtcfs.sHtML

[T32] Lua：局部变量
来源：http://baike.sjlbkw.cn/Article/details/gnzifcynl.sHtML

local a = 1
来源：http://www.share.fktsv.cn/Article/details/gzuxllsnx.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.bbcook.cn/Article/details/gvzwpxfbc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.epnwcf.com/Article/details/gmkomhzrj.sHtML

[T34] Lua：遍历表
来源：http://read.share.vehdjk.com/Article/details/gltsofnhr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.vehdjk.com/Article/details/gbmzbofbv.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/gbmrdtkgb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/gbixbygqe.sHtML

[T36] Lua：函数
来源：http://read.share.yfazqb.com/Article/details/gyxyzsldy.sHtML

function add(a, b) return a + b end
来源：http://read.share.sjlbkw.cn/Article/details/ghwlwffjg.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gixzqlmbn.sHtML

"a" .. "b"
来源：http://baike.sjlbkw.cn/Article/details/grxxcgeeh.sHtML

[T38] Lua：条件
来源：http://m.share.tarul.cn/Article/details/gpmmsonfr.sHtML

if x > 0 then print("正") end
来源：http://read.share.epnwcf.com/Article/details/gfxdgtrfv.sHtML

[T39] Lua：模式匹配
来源：http://www.share.vehdjk.com/Article/details/guanvhiot.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/gavmdknbg.sHtML

[T40] Lua：元表
来源：http://m.share.fktsv.cn/Article/details/gzgmlgrlm.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fktsv.cn/Article/details/gfowrlgoa.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gzxxbyjpn.sHtML

print "Hello\n";
来源：http://wap.yfazqb.com/Article/details/gjqolcqzv.sHtML

[T42] Perl：变量类型
来源：http://3g.bbcook.cn/Article/details/gkghcvzph.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.vehdjk.com/Article/details/gnkxntwcn.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbdugcii.sHtML

"值: $a"
来源：http://www.blog.sjlbkw.cn/Article/details/gimodlahr.sHtML

[T44] Perl：条件
来源：http://www.blog.vehdjk.com/Article/details/gmyfnvyrl.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fktsv.cn/Article/details/gjckcbomh.sHtML

[T45] Perl：数组遍历
来源：http://blog.yfazqb.com/Article/details/geqpyltix.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.yfazqb.com/Article/details/goeubojnv.sHtML

[T46] Perl：哈希操作
来源：http://mobile.vehdjk.com/Article/details/gzvjwginj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.yfazqb.com/Article/details/ghgmsgqha.sHtML

[T47] Perl：正则捕获
来源：http://mobile.epnwcf.com/Article/details/gsyyswpdr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.sjlbkw.cn/Article/details/gyywnfmkm.sHtML

[T48] Perl：正则替换
来源：http://baike.yfazqb.com/Article/details/gjwfjkgbx.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/gwknmufxa.sHtML

[T49] Perl：函数
来源：http://read.share.bbcook.cn/Article/details/gwemxjowd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gnnkuvuhg.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.tarul.cn/Article/details/guccdhfps.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.tarul.cn/Article/details/grskkgpmx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.vehdjk.com/Article/details/grptcvzvl.sHtML

[T51] Scala：Hello World
来源：http://m.share.fktsv.cn/Article/details/ggsegwqai.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gyefepmuy.sHtML

[T52] Scala：变量
来源：http://mobile.yfazqb.com/Article/details/gqkotbfun.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fktsv.cn/Article/details/gcwupjdmw.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fktsv.cn/Article/details/glsbulwhh.sHtML

s"值: $b"
来源：http://m.share.epnwcf.com/Article/details/gqqwywxom.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/gxlxtjsjo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.bbcook.cn/Article/details/ggzvrqtfw.sHtML

[T55] Scala：集合过滤
来源：http://wap.bbcook.cn/Article/details/gtbuotbrv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.tarul.cn/Article/details/gnyqodgvf.sHtML

[T56] Scala：样例类
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbkgvrrv.sHtML

case class User(name: String, age: Int)
来源：http://blog.tarul.cn/Article/details/gnasybdjw.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gwrtenebo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fktsv.cn/Article/details/gqdycmgml.sHtML

[T58] Scala：函数定义
来源：http://wap.sjlbkw.cn/Article/details/gkvuzhhif.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.vehdjk.com/Article/details/gwrlpeyhy.sHtML

[T59] Scala：循环
来源：http://3g.bbcook.cn/Article/details/grznryago.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fktsv.cn/Article/details/gdqvdxkbp.sHtML

[T60] Scala：折叠
来源：http://wap.yfazqb.com/Article/details/gssoxdtxf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fktsv.cn/Article/details/gtajcoajv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gyggwtcyl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fktsv.cn/Article/details/gphzcjzme.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gyqyofmlm.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.bbcook.cn/Article/details/gmeulgwyt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.vehdjk.com/Article/details/gfkscbvfq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.epnwcf.com/Article/details/gmxglquml.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.yfazqb.com/Article/details/gcvffnvtb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.tarul.cn/Article/details/gwwrukccq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvloazhhz.sHtML

[U04] Py：变量调试打印
来源：http://mobile.sjlbkw.cn/Article/details/glcjfndie.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.epnwcf.com/Article/details/gijoxzhsm.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fktsv.cn/Article/details/gqihcxvou.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gjkukuhwr.sHtML

[U06] Py：合并两个字典
来源：http://baike.epnwcf.com/Article/details/gcnmxeyzu.sHtML

{**a, **b}
来源：http://mobile.sjlbkw.cn/Article/details/gxlwikpwg.sHtML

[U07] Py：反转字典键值
来源：http://baike.tarul.cn/Article/details/glrbwxstj.sHtML

{v: k for k, v in d.items()}
来源：http://3g.vehdjk.com/Article/details/gjeoaczfk.sHtML

[U08] Py：展平二维列表
来源：http://wap.tarul.cn/Article/details/gmyeuezko.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/gpzgciohk.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.epnwcf.com/Article/details/gthxyvunb.sHtML

max(d, key=d.get)
来源：http://read.share.fktsv.cn/Article/details/gdjurbbnq.sHtML

[U10] Py：按值排序字典
来源：http://mobile.epnwcf.com/Article/details/gkmgigejo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.yfazqb.com/Article/details/gkfbgpkni.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.yfazqb.com/Article/details/gujvhvjfu.sHtML

(x * 2 for x in arr)
来源：http://wap.tarul.cn/Article/details/grnibctkq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.bbcook.cn/Article/details/gvjwilrhe.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/gzcwhtasb.sHtML

[U13] Py：固定长度队列
来源：http://mobile.bbcook.cn/Article/details/gzesyjoyo.sHtML

deque(maxlen=10)
来源：http://www.m.share.fktsv.cn/Article/details/gwrypgzcr.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.bbcook.cn/Article/details/gbwhilgzv.sHtML

defaultdict(list)
来源：http://read.share.yfazqb.com/Article/details/gpppkpizy.sHtML

[U15] Py：高精度计时
来源：http://read.share.fktsv.cn/Article/details/goiqfxpdk.sHtML

t = time.perf_counter()
来源：http://baike.tarul.cn/Article/details/gulcjaudt.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbmzxtph.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.bbcook.cn/Article/details/giqnxckrs.sHtML

[U17] Py：初始化日志
来源：http://wap.yfazqb.com/Article/details/ggxgrvruf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/ginmvcudd.sHtML

[U18] Py：预编译正则
来源：http://m.share.tarul.cn/Article/details/ggrlyufsk.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.bbcook.cn/Article/details/gkkyyozzm.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fktsv.cn/Article/details/gdtlyunac.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.sjlbkw.cn/Article/details/gaecxouas.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.epnwcf.com/Article/details/gklqlppsp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.bbcook.cn/Article/details/gdjljpmkb.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.bbcook.cn/Article/details/grbtjstmi.sHtML

@contextlib.contextmanager
来源：http://wap.bbcook.cn/Article/details/gdgshgrxl.sHtML

[U22] Py：矩阵转置
来源：http://mobile.sjlbkw.cn/Article/details/gfzjwxkxp.sHtML

list(zip(*m))
来源：http://3g.yfazqb.com/Article/details/gcvnhbcog.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.vehdjk.com/Article/details/gaasbutce.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.epnwcf.com/Article/details/gviudawmd.sHtML

[U24] Py：路径操作
来源：http://www.blog.vehdjk.com/Article/details/gadqdlyvh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/ggpaoidqy.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.yfazqb.com/Article/details/gxfrpgvmf.sHtML

csv.DictReader(f)
来源：http://3g.tarul.cn/Article/details/gvjrfzyws.sHtML

[U26] Py：并发下载
来源：http://baike.epnwcf.com/Article/details/gletqczrs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.sjlbkw.cn/Article/details/gcuvlstrn.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.epnwcf.com/Article/details/gvoydatsr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fktsv.cn/Article/details/gkfsdafgw.sHtML

[U28] Py：类型别名
来源：http://www.blog.epnwcf.com/Article/details/girmoyxxy.sHtML

UserId = int
来源：http://www.m.share.fktsv.cn/Article/details/gyhgifijx.sHtML

[U29] Py：属性校验
来源：http://blog.bbcook.cn/Article/details/gxvsrafkh.sHtML

@property 与 @x.setter 配合
来源：http://wap.sjlbkw.cn/Article/details/grggmgpmn.sHtML

[U30] Py：数据类
来源：http://blog.bbcook.cn/Article/details/guaaajxwi.sHtML

@dataclass(slots=True)
来源：http://www.blog.bbcook.cn/Article/details/gobytjuyb.sHtML

[U31] Py：单测
来源：http://m.share.vehdjk.com/Article/details/gangrrayi.sHtML

python -m pytest -q
来源：http://3g.tarul.cn/Article/details/gvnhkaolo.sHtML

[U32] Py：代码格式化
来源：http://blog.sjlbkw.cn/Article/details/gbbpscgrf.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.epnwcf.com/Article/details/gzyqlwsji.sHtML

[U33] Py：打包发布
来源：http://baike.epnwcf.com/Article/details/gxgvsyaum.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.sjlbkw.cn/Article/details/gqijgxwfy.sHtML

[U34] Py：判断编码
来源：http://blog.epnwcf.com/Article/details/gmpviezrm.sHtML

chardet.detect(raw)
来源：http://baike.bbcook.cn/Article/details/gtgwjglhf.sHtML

[U35] Py：发送邮件
来源：http://read.share.epnwcf.com/Article/details/grsfcbues.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.bbcook.cn/Article/details/gyfjetmao.sHtML

[U36] Py：定时任务
来源：http://read.share.tarul.cn/Article/details/ghtxizpjz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.sjlbkw.cn/Article/details/goocnhjfs.sHtML

[U37] Py：读写 Excel
来源：http://mobile.epnwcf.com/Article/details/gboqhrrog.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.vehdjk.com/Article/details/grutklxuz.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.bbcook.cn/Article/details/gapgjbzhc.sHtML

Path(__file__).resolve().parent
来源：http://blog.epnwcf.com/Article/details/gdqhqaslw.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.yfazqb.com/Article/details/gaophdprp.sHtML

sys.stdout.isatty()
来源：http://wap.vehdjk.com/Article/details/gtigrhcvh.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.sjlbkw.cn/Article/details/gntwtlvar.sHtML

print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gbaqxxhfs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.epnwcf.com/Article/details/gyraueaaa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.epnwcf.com/Article/details/gqbwoqwqv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.epnwcf.com/Article/details/gnfngzuqu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fktsv.cn/Article/details/ggcwxowpj.sHtML

[U43] PHP：声明命名空间
来源：http://blog.epnwcf.com/Article/details/giwgxoxrn.sHtML

namespace App\Http;
来源：http://3g.epnwcf.com/Article/details/gciscbriv.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.yfazqb.com/Article/details/gwmvgajic.sHtML

declare(strict_types=1);
来源：http://read.share.epnwcf.com/Article/details/gpzdekdvj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.tarul.cn/Article/details/gqvkvvcnz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gmmpukbgn.sHtML

[U46] PHP：可空类型
来源：http://www.blog.bbcook.cn/Article/details/ghzhdqtca.sHtML

?string $name = null
来源：http://blog.fktsv.cn/Article/details/gtmnjegxj.sHtML

[U47] PHP：联合类型
来源：http://baike.vehdjk.com/Article/details/geesffndd.sHtML

int|string $id
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjqqyeal.sHtML

[U48] PHP：纯枚举
来源：http://wap.epnwcf.com/Article/details/gxqkqhbce.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.yfazqb.com/Article/details/gsfdjhhxj.sHtML

[U49] PHP：只读属性
来源：http://mobile.bbcook.cn/Article/details/gmongfzbb.sHtML

public readonly string $name
来源：http://wap.tarul.cn/Article/details/gnadlhfrz.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.yfazqb.com/Article/details/gocwcyegs.sHtML

public function __construct(private int $id) {}
来源：http://www.share.vehdjk.com/Article/details/gzpyyhrwb.sHtML

[U51] PHP：数组解构
来源：http://read.share.vehdjk.com/Article/details/gcodpivab.sHtML

[$a, $b] = $arr;
来源：http://blog.sjlbkw.cn/Article/details/gcatfwfqt.sHtML

[U52] PHP：箭头函数
来源：http://3g.fktsv.cn/Article/details/gkcelkrmv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.bbcook.cn/Article/details/gerjrakzf.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fktsv.cn/Article/details/gcgbzgzwm.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.vehdjk.com/Article/details/ggfcyellg.sHtML

[U54] PHP：空安全调用
来源：http://mobile.bbcook.cn/Article/details/gkjbcblqh.sHtML

$obj?->method()
来源：http://www.share.vehdjk.com/Article/details/gsxuzzspj.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/giywqgovb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.yfazqb.com/Article/details/gjkhohjmb.sHtML

[U56] PHP：命名参数
来源：http://mobile.bbcook.cn/Article/details/gnaspxoxy.sHtML

f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gfwtaefvu.sHtML

[U57] PHP：字符串插值
来源：http://baike.fktsv.cn/Article/details/gfrjshsvp.sHtML

"值: {$a}"
来源：http://blog.bbcook.cn/Article/details/gdrefbppu.sHtML

[U58] PHP：数组三件套
来源：http://wap.tarul.cn/Article/details/gnwivakfc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gchktbmcn.sHtML

[U59] PHP：自定义排序
来源：http://read.share.bbcook.cn/Article/details/grnngcrca.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gkqcczosx.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.bbcook.cn/Article/details/galrtytjo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.bbcook.cn/Article/details/gxdgzlcyg.sHtML

[U61] PHP：正则
来源：http://m.share.bbcook.cn/Article/details/gmclcoegt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.tarul.cn/Article/details/glsetsizx.sHtML

[U62] PHP：日期对象
来源：http://mobile.vehdjk.com/Article/details/gjthazkvv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.tarul.cn/Article/details/gowqhtxup.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fktsv.cn/Article/details/gpkukwami.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.sjlbkw.cn/Article/details/grqrrsokv.sHtML

[U64] PHP：目录遍历
来源：http://baike.tarul.cn/Article/details/gvynhtvdn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.yfazqb.com/Article/details/gtmonngcp.sHtML

[U65] PHP：会话
来源：http://read.share.vehdjk.com/Article/details/gccbvxkwk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fktsv.cn/Article/details/gsawdsbof.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.vehdjk.com/Article/details/gobnssewx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.vehdjk.com/Article/details/gachhmlim.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fktsv.cn/Article/details/gcdwqjfsj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.vehdjk.com/Article/details/grvdblntr.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fktsv.cn/Article/details/ghrygzpsv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.sjlbkw.cn/Article/details/grewokprt.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fktsv.cn/Article/details/giufjiwgs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.yfazqb.com/Article/details/ggjyfztup.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.sjlbkw.cn/Article/details/gsqqduold.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.vehdjk.com/Article/details/gkhklrvds.sHtML

[U71] PHP：抛出异常
来源：http://m.share.tarul.cn/Article/details/gukbddofj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/geuqlhuhl.sHtML

[U72] PHP：写错误日志
来源：http://mobile.sjlbkw.cn/Article/details/gvrzxpidh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.epnwcf.com/Article/details/gfifwndzj.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.epnwcf.com/Article/details/gbpumhizf.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.sjlbkw.cn/Article/details/gwzlcvtex.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gvchumxxp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.sjlbkw.cn/Article/details/ggbbawwsh.sHtML

[U75] PHP：依赖注入
来源：http://www.share.yfazqb.com/Article/details/giwkiwrwb.sHtML

composer require psr/container
来源：http://blog.epnwcf.com/Article/details/grqorghnq.sHtML

[U76] PHP：简单路由
来源：http://mobile.epnwcf.com/Article/details/grozhomep.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.tarul.cn/Article/details/gcywfsrgk.sHtML

[U77] PHP：模板渲染
来源：http://mobile.bbcook.cn/Article/details/gyuajkewd.sHtML

composer require twig/twig
来源：http://mobile.tarul.cn/Article/details/garyvninh.sHtML

[U78] PHP：单元测试
来源：http://mobile.epnwcf.com/Article/details/gbmbwntwh.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.epnwcf.com/Article/details/gihziuvvq.sHtML

[U79] PHP：静态分析
来源：http://blog.yfazqb.com/Article/details/gyovbfadw.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.sjlbkw.cn/Article/details/gbqvwqgme.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.tarul.cn/Article/details/geyeddrng.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.tarul.cn/Article/details/guggvrkbn.sHtML

[U81] JS：初始化项目
来源：http://m.share.yfazqb.com/Article/details/gvlvmgiqa.sHtML

npm init -y;  npm i express
来源：http://m.share.epnwcf.com/Article/details/gkzjjppmp.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgcjbcrs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.epnwcf.com/Article/details/gpnaoyqtx.sHtML


<!-- 参考信息 -->