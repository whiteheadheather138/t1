代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.blog.bbcook.cn/Article/details/gbsyrxuzj.sHtML

[S49] C++：写文件
来源：http://www.blog.bbcook.cn/Article/details/gkilejyuo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.epnwcf.com/Article/details/gkfhymqts.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/glczdfvun.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gsdrrmgst.sHtML

[S51] C++：显式类型转换
来源：http://www.share.yfazqb.com/Article/details/gtsackeke.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/gpbezyotf.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fktsv.cn/Article/details/gdyssuxdf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.epnwcf.com/Article/details/gklyowpmh.sHtML

[S53] C++：移动语义
来源：http://read.share.bbcook.cn/Article/details/gnacsgsnh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.sjlbkw.cn/Article/details/gxdcghaft.sHtML

[S54] C++：异常处理
来源：http://www.blog.epnwcf.com/Article/details/gnmefofpb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.vehdjk.com/Article/details/gcjkrqmne.sHtML

[S55] C++：结构化绑定
来源：http://wap.sjlbkw.cn/Article/details/gzpicvuji.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gigddgqzd.sHtML

[S56] C++：optional
来源：http://blog.epnwcf.com/Article/details/gulxcahco.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/gyaqbvwas.sHtML

[S57] C++：编译期常量
来源：http://wap.vehdjk.com/Article/details/gkqyjxcgj.sHtML

constexpr int N = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gjwbcuqyv.sHtML

[S58] C++：命名空间
来源：http://mobile.fktsv.cn/Article/details/gyyruenpo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.tarul.cn/Article/details/gqokmapdw.sHtML

[S59] C++：静态断言
来源：http://www.share.epnwcf.com/Article/details/gddsrzhmb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.bbcook.cn/Article/details/gcyppgple.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fktsv.cn/Article/details/gsvyhcfnx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.bbcook.cn/Article/details/gnqhuvtlz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gppbnepki.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.vehdjk.com/Article/details/gcinrhhmd.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glnvznnbl.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fktsv.cn/Article/details/gxmyxehth.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gclcdavvf.sHtML

[T02] Kotlin：变量
来源：http://read.share.sjlbkw.cn/Article/details/goqssepfs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.tarul.cn/Article/details/gsayixibc.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/gxwwgscoi.sHtML

"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/goqiklijm.sHtML

[T04] Kotlin：空安全
来源：http://3g.sjlbkw.cn/Article/details/glyshfqlo.sHtML

val n: String? = null;  n?.length
来源：http://read.share.tarul.cn/Article/details/glrvrjjdo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.bbcook.cn/Article/details/ggynxjiqa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.sjlbkw.cn/Article/details/geawvqpvv.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fktsv.cn/Article/details/gzavmsgjb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.yfazqb.com/Article/details/gmlkbtjqn.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.epnwcf.com/Article/details/gmeoawjnm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.tarul.cn/Article/details/gqivpogrl.sHtML

[T08] Kotlin：数据类
来源：http://m.share.vehdjk.com/Article/details/gstyancvs.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gkeqtjvzl.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.vehdjk.com/Article/details/gcmiqyxce.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.yfazqb.com/Article/details/gcisojctp.sHtML

[T10] Kotlin：默认参数
来源：http://3g.bbcook.cn/Article/details/gclzzbtaq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.vehdjk.com/Article/details/glugrhtqv.sHtML

[T11] Kotlin：协程
来源：http://blog.vehdjk.com/Article/details/gvnwkwtao.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.epnwcf.com/Article/details/gpjpjamra.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/grqgcpipw.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/giakvzmed.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.sjlbkw.cn/Article/details/gjrxfpfji.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.vehdjk.com/Article/details/gpnigvntx.sHtML

[T14] Kotlin：循环
来源：http://baike.epnwcf.com/Article/details/goahxkhgw.sHtML

for (i in 1..10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gagduynsf.sHtML

[T15] Kotlin：接口
来源：http://m.share.yfazqb.com/Article/details/gtotarcgd.sHtML

interface Shape { fun area(): Double }
来源：http://blog.tarul.cn/Article/details/gbhmuehcx.sHtML

[T16] Swift：Hello World
来源：http://blog.tarul.cn/Article/details/gsmrnbgzm.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/glgclwjpe.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.vehdjk.com/Article/details/gndbhvwje.sHtML

var a = 1;  let b = 2
来源：http://blog.bbcook.cn/Article/details/gumtkiimk.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gjepfqtmz.sHtML

"值: \(b)"
来源：http://blog.vehdjk.com/Article/details/gvnrpkkhr.sHtML

[T19] Swift：可选绑定
来源：http://read.share.tarul.cn/Article/details/gpdfereaa.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/gyklylpnt.sHtML

[T20] Swift：数组操作
来源：http://read.share.vehdjk.com/Article/details/gzrbpgzhr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/ghuczodml.sHtML

[T21] Swift：遍历
来源：http://mobile.vehdjk.com/Article/details/gwginhidc.sHtML

for x in a { print(x) }
来源：http://read.share.yfazqb.com/Article/details/goohesadh.sHtML

[T22] Swift：字典
来源：http://www.blog.epnwcf.com/Article/details/gvwjgmdqi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gkuqubbgb.sHtML

[T23] Swift：函数
来源：http://read.share.yfazqb.com/Article/details/gkqerxglj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.bbcook.cn/Article/details/ggzjefvkn.sHtML

[T24] Swift：闭包
来源：http://baike.vehdjk.com/Article/details/gxnelbafk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fktsv.cn/Article/details/gkghcpded.sHtML

[T25] Swift：结构体
来源：http://baike.epnwcf.com/Article/details/gmidbfwdj.sHtML

struct P { var x: Int }
来源：http://mobile.fktsv.cn/Article/details/glqrhhryd.sHtML

[T26] Swift：类与重写
来源：http://baike.yfazqb.com/Article/details/gxfmdgeqb.sHtML

class A: Base { override func f() {} }
来源：http://blog.bbcook.cn/Article/details/gprtpsqob.sHtML

[T27] Swift：错误处理
来源：http://www.share.yfazqb.com/Article/details/gzlfvppvr.sHtML

do { try f() } catch { print(error) }
来源：http://3g.sjlbkw.cn/Article/details/gvqsbakpz.sHtML

[T28] Swift：枚举
来源：http://blog.tarul.cn/Article/details/gfulzitga.sHtML

enum Color { case red, green }
来源：http://blog.tarul.cn/Article/details/gjxnfoaji.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.yfazqb.com/Article/details/gyakrtlxo.sHtML

guard let x = opt else { return }
来源：http://read.share.vehdjk.com/Article/details/gswqpksub.sHtML

[T30] Swift：协议
来源：http://blog.epnwcf.com/Article/details/geylpsmny.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.tarul.cn/Article/details/gfgdoqnab.sHtML

[T31] Lua：Hello World
来源：http://www.share.tarul.cn/Article/details/gtudkznjj.sHtML

print("Hello")
来源：http://blog.bbcook.cn/Article/details/gvfnfejix.sHtML

[T32] Lua：局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gcfuxmsjy.sHtML

local a = 1
来源：http://read.share.epnwcf.com/Article/details/gazrkpped.sHtML

[T33] Lua：表（数组）
来源：http://wap.bbcook.cn/Article/details/gvobvsctc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.vehdjk.com/Article/details/gamqnmyar.sHtML

[T34] Lua：遍历表
来源：http://mobile.epnwcf.com/Article/details/gmrvrmisz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.epnwcf.com/Article/details/gujcmxtev.sHtML

[T35] Lua：字典表
来源：http://m.share.sjlbkw.cn/Article/details/glgblnnzk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.bbcook.cn/Article/details/ggylmirnk.sHtML

[T36] Lua：函数
来源：http://www.share.tarul.cn/Article/details/gayuradps.sHtML

function add(a, b) return a + b end
来源：http://read.share.vehdjk.com/Article/details/gvfdqmolf.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fktsv.cn/Article/details/gsfrircha.sHtML

"a" .. "b"
来源：http://www.m.share.tarul.cn/Article/details/gadcvxvfl.sHtML

[T38] Lua：条件
来源：http://3g.bbcook.cn/Article/details/gdnxiyawe.sHtML

if x > 0 then print("正") end
来源：http://m.share.fktsv.cn/Article/details/gledkbdni.sHtML

[T39] Lua：模式匹配
来源：http://blog.tarul.cn/Article/details/gtyhvrhpl.sHtML

string.find(s, "%d+")
来源：http://baike.sjlbkw.cn/Article/details/glwsgbqbv.sHtML

[T40] Lua：元表
来源：http://baike.fktsv.cn/Article/details/ggsdrwngq.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fktsv.cn/Article/details/gixafmxca.sHtML

[T41] Perl：Hello World
来源：http://baike.vehdjk.com/Article/details/gbziybhxl.sHtML

print "Hello\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbvqlxps.sHtML

[T42] Perl：变量类型
来源：http://blog.epnwcf.com/Article/details/grzvbkkfr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.bbcook.cn/Article/details/ghpwihfku.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gymmyoyjd.sHtML

"值: $a"
来源：http://3g.tarul.cn/Article/details/gwylxnnzo.sHtML

[T44] Perl：条件
来源：http://read.share.sjlbkw.cn/Article/details/gpzmicyra.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.epnwcf.com/Article/details/gueizdekl.sHtML

[T45] Perl：数组遍历
来源：http://baike.bbcook.cn/Article/details/gnsyztsfn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.yfazqb.com/Article/details/gajbdcjjw.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.vehdjk.com/Article/details/ghfckesqt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.epnwcf.com/Article/details/gmywantua.sHtML

[T47] Perl：正则捕获
来源：http://read.share.epnwcf.com/Article/details/graklprpf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.epnwcf.com/Article/details/gomryvovb.sHtML

[T48] Perl：正则替换
来源：http://3g.fktsv.cn/Article/details/gglxfeudl.sHtML

$s =~ s/old/new/g;
来源：http://3g.fktsv.cn/Article/details/gdwdmpfeb.sHtML

[T49] Perl：函数
来源：http://baike.bbcook.cn/Article/details/gqwuiujbe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gqnpeystz.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gklatsihe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.epnwcf.com/Article/details/gukurqotu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gdtuoruur.sHtML

[T51] Scala：Hello World
来源：http://3g.bbcook.cn/Article/details/gozrebhls.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gbmzfwqfq.sHtML

[T52] Scala：变量
来源：http://mobile.fktsv.cn/Article/details/gscktokpn.sHtML

val a = 1;  var b = 2
来源：http://blog.tarul.cn/Article/details/gxvgihaqd.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gylzfjcvj.sHtML

s"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gedgcjxma.sHtML

[T54] Scala：集合映射
来源：http://3g.vehdjk.com/Article/details/grgylydoj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.epnwcf.com/Article/details/giulciqmh.sHtML

[T55] Scala：集合过滤
来源：http://www.share.vehdjk.com/Article/details/gsfsbgsnp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.sjlbkw.cn/Article/details/gfzsxtavg.sHtML

[T56] Scala：样例类
来源：http://mobile.fktsv.cn/Article/details/gojuobfta.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.vehdjk.com/Article/details/gcdueeues.sHtML

[T57] Scala：模式匹配
来源：http://m.share.epnwcf.com/Article/details/grkwsymnd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.tarul.cn/Article/details/gclegedov.sHtML

[T58] Scala：函数定义
来源：http://www.share.vehdjk.com/Article/details/gjzjvbsni.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.sjlbkw.cn/Article/details/gpbqozbvq.sHtML

[T59] Scala：循环
来源：http://baike.vehdjk.com/Article/details/gbflysrzb.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fktsv.cn/Article/details/gdnrvaigl.sHtML

[T60] Scala：折叠
来源：http://www.blog.fktsv.cn/Article/details/gwdxfuety.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.bbcook.cn/Article/details/guvhnxxej.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxhblgusu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.epnwcf.com/Article/details/gdkieuqsg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gibqmxrps.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.epnwcf.com/Article/details/gbrkooqtb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fktsv.cn/Article/details/ggiuomsoz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.bbcook.cn/Article/details/gxmjvydeq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.vehdjk.com/Article/details/gahsgxusq.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.bbcook.cn/Article/details/gfkggwpav.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.epnwcf.com/Article/details/gvammhbdw.sHtML

[U04] Py：变量调试打印
来源：http://blog.epnwcf.com/Article/details/gxdehxebm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.sjlbkw.cn/Article/details/guzttyfpp.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.tarul.cn/Article/details/gkpozrjaz.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gplbnunxa.sHtML

[U06] Py：合并两个字典
来源：http://blog.yfazqb.com/Article/details/gcbxgfoum.sHtML

{**a, **b}
来源：http://3g.epnwcf.com/Article/details/gbxbdlrkj.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fktsv.cn/Article/details/gdqyxhshj.sHtML

{v: k for k, v in d.items()}
来源：http://3g.epnwcf.com/Article/details/giimvwizm.sHtML

[U08] Py：展平二维列表
来源：http://mobile.bbcook.cn/Article/details/gnvujlasq.sHtML

[y for x in nested for y in x]
来源：http://mobile.tarul.cn/Article/details/gamrvwexi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fktsv.cn/Article/details/gtruwrril.sHtML

max(d, key=d.get)
来源：http://baike.epnwcf.com/Article/details/gukkxohsj.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.vehdjk.com/Article/details/gcriqeycx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.bbcook.cn/Article/details/glamoajue.sHtML

[U11] Py：生成器表达式
来源：http://wap.fktsv.cn/Article/details/gixngbqax.sHtML

(x * 2 for x in arr)
来源：http://read.share.vehdjk.com/Article/details/gqlhmdooe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fktsv.cn/Article/details/gxhgxeonn.sHtML

Counter(arr).most_common(3)
来源：http://baike.vehdjk.com/Article/details/gdxkemqjn.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fktsv.cn/Article/details/gpcdtwjwo.sHtML

deque(maxlen=10)
来源：http://3g.epnwcf.com/Article/details/gzttwshdl.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.bbcook.cn/Article/details/gzzgmxgbm.sHtML

defaultdict(list)
来源：http://www.share.vehdjk.com/Article/details/gfkluounf.sHtML

[U15] Py：高精度计时
来源：http://m.share.tarul.cn/Article/details/gxtbmavwl.sHtML

t = time.perf_counter()
来源：http://blog.bbcook.cn/Article/details/gclpodcks.sHtML

[U16] Py：命令行参数解析
来源：http://3g.tarul.cn/Article/details/gpylljshx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.yfazqb.com/Article/details/gpcnwagwt.sHtML

[U17] Py：初始化日志
来源：http://www.share.tarul.cn/Article/details/gabsuxsuk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.yfazqb.com/Article/details/gjfflwmnh.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.epnwcf.com/Article/details/gpdsnqajc.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/gsqprpjai.sHtML

[U19] Py：正则替换带回调
来源：http://blog.epnwcf.com/Article/details/gtupzgurb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.yfazqb.com/Article/details/gniwkkven.sHtML

[U20] Py：缓存函数结果
来源：http://3g.tarul.cn/Article/details/gywhujfwr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.sjlbkw.cn/Article/details/grfjnazob.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.sjlbkw.cn/Article/details/gtibsctis.sHtML

@contextlib.contextmanager
来源：http://3g.bbcook.cn/Article/details/gmqumoiqq.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fktsv.cn/Article/details/gmxqwuhbb.sHtML

list(zip(*m))
来源：http://wap.vehdjk.com/Article/details/gohtxytgi.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.bbcook.cn/Article/details/gtpodsbsb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fktsv.cn/Article/details/gwdnuimeh.sHtML

[U24] Py：路径操作
来源：http://blog.yfazqb.com/Article/details/gmpvawdef.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/groqlzkkj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.yfazqb.com/Article/details/gwxovqqnm.sHtML

csv.DictReader(f)
来源：http://3g.tarul.cn/Article/details/gntcujyic.sHtML

[U26] Py：并发下载
来源：http://read.share.bbcook.cn/Article/details/gcolnflvc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.sjlbkw.cn/Article/details/gsqslvyhk.sHtML

[U27] Py：异步 HTTP
来源：http://blog.bbcook.cn/Article/details/galnvurbv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fktsv.cn/Article/details/gpuceygcd.sHtML

[U28] Py：类型别名
来源：http://m.share.epnwcf.com/Article/details/gggbqidfy.sHtML

UserId = int
来源：http://m.share.vehdjk.com/Article/details/gocoaefsk.sHtML

[U29] Py：属性校验
来源：http://blog.sjlbkw.cn/Article/details/glcgawfpv.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fktsv.cn/Article/details/gftgsrctk.sHtML

[U30] Py：数据类
来源：http://blog.fktsv.cn/Article/details/gvizjbjfg.sHtML

@dataclass(slots=True)
来源：http://wap.vehdjk.com/Article/details/gmuppkmip.sHtML

[U31] Py：单测
来源：http://mobile.epnwcf.com/Article/details/gzekwdfqe.sHtML

python -m pytest -q
来源：http://m.share.vehdjk.com/Article/details/gzoumrlps.sHtML

[U32] Py：代码格式化
来源：http://read.share.tarul.cn/Article/details/gamtfiucc.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.vehdjk.com/Article/details/gxiywcaeb.sHtML

[U33] Py：打包发布
来源：http://baike.fktsv.cn/Article/details/ggpsarndo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.vehdjk.com/Article/details/gduvzyyzs.sHtML

[U34] Py：判断编码
来源：http://mobile.sjlbkw.cn/Article/details/gtavpqnxz.sHtML

chardet.detect(raw)
来源：http://read.share.tarul.cn/Article/details/gxzdwxuej.sHtML

[U35] Py：发送邮件
来源：http://m.share.tarul.cn/Article/details/gscqbbbmo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.tarul.cn/Article/details/goxpexayd.sHtML

[U36] Py：定时任务
来源：http://blog.fktsv.cn/Article/details/gsujccbmn.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.vehdjk.com/Article/details/gpgxtyzaj.sHtML

[U37] Py：读写 Excel
来源：http://blog.epnwcf.com/Article/details/gafakxhnv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.sjlbkw.cn/Article/details/gfdlelnvz.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.bbcook.cn/Article/details/gtaowyenn.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.tarul.cn/Article/details/ggkfcbjll.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.sjlbkw.cn/Article/details/gvurmjzov.sHtML

sys.stdout.isatty()
来源：http://www.blog.sjlbkw.cn/Article/details/gutaamkqi.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.bbcook.cn/Article/details/gfmnzpdds.sHtML

print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/gksnmorvy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.tarul.cn/Article/details/geljcuuwu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.sjlbkw.cn/Article/details/gdwxcynnc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.yfazqb.com/Article/details/gwdpacdzr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.yfazqb.com/Article/details/gmfortjyn.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.sjlbkw.cn/Article/details/ggkbgdvnz.sHtML

namespace App\Http;
来源：http://read.share.bbcook.cn/Article/details/gukpbrklu.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.vehdjk.com/Article/details/gynikrzrz.sHtML

declare(strict_types=1);
来源：http://baike.sjlbkw.cn/Article/details/gyrncrqdq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.tarul.cn/Article/details/gouxzvdis.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gsbvgzibl.sHtML

[U46] PHP：可空类型
来源：http://m.share.bbcook.cn/Article/details/gerpucpkb.sHtML

?string $name = null
来源：http://mobile.tarul.cn/Article/details/gsfczknaf.sHtML

[U47] PHP：联合类型
来源：http://baike.bbcook.cn/Article/details/ginvhscis.sHtML

int|string $id
来源：http://baike.yfazqb.com/Article/details/gpjfpkoqr.sHtML

[U48] PHP：纯枚举
来源：http://wap.sjlbkw.cn/Article/details/gotavzecp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.yfazqb.com/Article/details/gzimdcqhb.sHtML

[U49] PHP：只读属性
来源：http://baike.fktsv.cn/Article/details/gaqqqejqe.sHtML

public readonly string $name
来源：http://www.blog.yfazqb.com/Article/details/gkoqcrpcw.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.bbcook.cn/Article/details/ggbqjgbdn.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.tarul.cn/Article/details/gzchtzvnd.sHtML

[U51] PHP：数组解构
来源：http://blog.tarul.cn/Article/details/gshgvydar.sHtML

[$a, $b] = $arr;
来源：http://read.share.sjlbkw.cn/Article/details/gtrydlkbc.sHtML

[U52] PHP：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/gedmeesci.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.tarul.cn/Article/details/gotqmasna.sHtML

[U53] PHP：空合并运算符
来源：http://3g.bbcook.cn/Article/details/gwumxfosa.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fktsv.cn/Article/details/grqtbtzbq.sHtML

[U54] PHP：空安全调用
来源：http://www.share.bbcook.cn/Article/details/gnrzyldyn.sHtML

$obj?->method()
来源：http://www.blog.tarul.cn/Article/details/gbiyqxxda.sHtML

[U55] PHP：match 表达式
来源：http://3g.tarul.cn/Article/details/gnxepyxos.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.yfazqb.com/Article/details/grmmvfjts.sHtML

[U56] PHP：命名参数
来源：http://baike.yfazqb.com/Article/details/gqnprzccq.sHtML

f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gdnpiuznj.sHtML

[U57] PHP：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gecgnfcvk.sHtML

"值: {$a}"
来源：http://3g.fktsv.cn/Article/details/gjamhvhwf.sHtML

[U58] PHP：数组三件套
来源：http://3g.sjlbkw.cn/Article/details/geexdcsit.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.tarul.cn/Article/details/gtleozpun.sHtML

[U59] PHP：自定义排序
来源：http://www.share.yfazqb.com/Article/details/gxayvyeum.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gdhxoodti.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.sjlbkw.cn/Article/details/gozyzxtct.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfczvgvoj.sHtML

[U61] PHP：正则
来源：http://baike.yfazqb.com/Article/details/ggjqbwdtl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/gkkvqemnp.sHtML

[U62] PHP：日期对象
来源：http://baike.fktsv.cn/Article/details/gkvxtevzm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.vehdjk.com/Article/details/gthfubupo.sHtML

[U63] PHP：文件读写
来源：http://baike.vehdjk.com/Article/details/gcpnkaagj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.yfazqb.com/Article/details/gbpzqbrfp.sHtML

[U64] PHP：目录遍历
来源：http://wap.sjlbkw.cn/Article/details/gsxqyymmi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.sjlbkw.cn/Article/details/ggmfaaybe.sHtML

[U65] PHP：会话
来源：http://baike.tarul.cn/Article/details/ggkweanwa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gulsbhxiw.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fktsv.cn/Article/details/gtlhbstvn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.vehdjk.com/Article/details/glojgjwge.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.vehdjk.com/Article/details/gexoykcwj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.epnwcf.com/Article/details/gvlwmjokz.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fktsv.cn/Article/details/ggakgbfhh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.tarul.cn/Article/details/gdjgkrpki.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.yfazqb.com/Article/details/gaumsvcre.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyplrthh.sHtML

[U70] PHP：PDO 事务
来源：http://wap.tarul.cn/Article/details/gvxqwnqmz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.epnwcf.com/Article/details/gokotabvq.sHtML

[U71] PHP：抛出异常
来源：http://m.share.yfazqb.com/Article/details/gatjqaqit.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.bbcook.cn/Article/details/ghaalixvz.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.tarul.cn/Article/details/gpgldxicf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.tarul.cn/Article/details/glrnyojrw.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.yfazqb.com/Article/details/gexuxfvql.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.vehdjk.com/Article/details/gfshueizz.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.vehdjk.com/Article/details/gsnbvyzjd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.vehdjk.com/Article/details/gzvjatyzs.sHtML


<!-- 参考信息 -->