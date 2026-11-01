代发 wailian999

int size() const noexcept { return n_; }
来源：http://read.share.fktsv.cn/Article/details/ghgidnqmo.sHtML

[S53] C++：移动语义
来源：http://m.share.epnwcf.com/Article/details/ggevvafcl.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.vehdjk.com/Article/details/gxquwosib.sHtML

[S54] C++：异常处理
来源：http://baike.bbcook.cn/Article/details/gnylobivy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.vehdjk.com/Article/details/gfxyrwybe.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fktsv.cn/Article/details/gyvhttpqf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.tarul.cn/Article/details/ghnmyzxrx.sHtML

[S56] C++：optional
来源：http://www.m.share.bbcook.cn/Article/details/gfzrlukkw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/geiljwqiq.sHtML

[S57] C++：编译期常量
来源：http://3g.sjlbkw.cn/Article/details/gyclmndtt.sHtML

constexpr int N = 10;
来源：http://wap.epnwcf.com/Article/details/gkmycvscu.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gphhyufhp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/grbkphftq.sHtML

[S59] C++：静态断言
来源：http://m.share.yfazqb.com/Article/details/gmtjkquys.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.vehdjk.com/Article/details/gwgqkwvcp.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/gusbfpzkl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.epnwcf.com/Article/details/gdopvptvs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdtupzpwl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gjmkncfzd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtvaeblja.sHtML

[T01] Kotlin：Hello World
来源：http://wap.bbcook.cn/Article/details/gznyjlmpk.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/grjibefgw.sHtML

[T02] Kotlin：变量
来源：http://mobile.sjlbkw.cn/Article/details/gtyvqmwfn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.yfazqb.com/Article/details/gbfvawwan.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fktsv.cn/Article/details/gidhrwrgw.sHtML

"值: $b"
来源：http://baike.tarul.cn/Article/details/gnvqpbooq.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fktsv.cn/Article/details/gfcxeuuat.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fktsv.cn/Article/details/gbytegbyj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gbboapzvz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.sjlbkw.cn/Article/details/gpcettseh.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gulgoiwuh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/ghcforplf.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.tarul.cn/Article/details/gxgpacnnt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/gkylzyknf.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/goliqxwor.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.bbcook.cn/Article/details/gyetdbhlf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtpynvkbt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fktsv.cn/Article/details/ggdvoqftr.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.epnwcf.com/Article/details/ghvvrhzja.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.epnwcf.com/Article/details/gdjjlerge.sHtML

[T11] Kotlin：协程
来源：http://m.share.bbcook.cn/Article/details/gcpbbluue.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.bbcook.cn/Article/details/gfskxpwoz.sHtML

[T12] Kotlin：解构声明
来源：http://blog.sjlbkw.cn/Article/details/ggwtqruik.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gamyeydnv.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/gjgdojpge.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/gxmvktwwa.sHtML

[T14] Kotlin：循环
来源：http://www.share.fktsv.cn/Article/details/ghnelneho.sHtML

for (i in 1..10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gbenyryit.sHtML

[T15] Kotlin：接口
来源：http://www.share.tarul.cn/Article/details/gwryzlhet.sHtML

interface Shape { fun area(): Double }
来源：http://3g.tarul.cn/Article/details/grtpoavum.sHtML

[T16] Swift：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gpmxhccuc.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gjflxvccl.sHtML

[T17] Swift：变量与常量
来源：http://mobile.sjlbkw.cn/Article/details/gydwyaluh.sHtML

var a = 1;  let b = 2
来源：http://baike.epnwcf.com/Article/details/gduebfwzf.sHtML

[T18] Swift：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gqzuqofko.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gvgwrtwip.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxqmsbai.sHtML

if let n = opt { print(n) }
来源：http://3g.epnwcf.com/Article/details/gmxprgyme.sHtML

[T20] Swift：数组操作
来源：http://www.blog.epnwcf.com/Article/details/gvgopyyuj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.tarul.cn/Article/details/gpuahoqtq.sHtML

[T21] Swift：遍历
来源：http://mobile.fktsv.cn/Article/details/gpbjswolu.sHtML

for x in a { print(x) }
来源：http://read.share.sjlbkw.cn/Article/details/gmjijcjii.sHtML

[T22] Swift：字典
来源：http://read.share.vehdjk.com/Article/details/glhixazfi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.epnwcf.com/Article/details/gxtonekwh.sHtML

[T23] Swift：函数
来源：http://baike.sjlbkw.cn/Article/details/gqfejfbtp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fktsv.cn/Article/details/gayndzmmf.sHtML

[T24] Swift：闭包
来源：http://www.m.share.bbcook.cn/Article/details/gscndqtnt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.vehdjk.com/Article/details/grcgstlsw.sHtML

[T25] Swift：结构体
来源：http://blog.bbcook.cn/Article/details/gtqshxggy.sHtML

struct P { var x: Int }
来源：http://www.share.sjlbkw.cn/Article/details/gwdmjzobh.sHtML

[T26] Swift：类与重写
来源：http://www.blog.yfazqb.com/Article/details/gzsltlfvg.sHtML

class A: Base { override func f() {} }
来源：http://blog.tarul.cn/Article/details/gpwxahwqp.sHtML

[T27] Swift：错误处理
来源：http://mobile.fktsv.cn/Article/details/gqzjxbqfc.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fktsv.cn/Article/details/gefuaalgc.sHtML

[T28] Swift：枚举
来源：http://wap.tarul.cn/Article/details/geamsclqd.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/gjvulpsnh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fktsv.cn/Article/details/gxqadmzwo.sHtML

guard let x = opt else { return }
来源：http://m.share.bbcook.cn/Article/details/gvdtvzkbg.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/gjxnjqcwf.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.bbcook.cn/Article/details/gohygagec.sHtML

[T31] Lua：Hello World
来源：http://m.share.bbcook.cn/Article/details/gmrwtthvu.sHtML

print("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gxbrmjyys.sHtML

[T32] Lua：局部变量
来源：http://www.share.fktsv.cn/Article/details/geimbhetd.sHtML

local a = 1
来源：http://baike.bbcook.cn/Article/details/grdqxqwro.sHtML

[T33] Lua：表（数组）
来源：http://mobile.bbcook.cn/Article/details/ghbdbjokq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.bbcook.cn/Article/details/gexypuozq.sHtML

[T34] Lua：遍历表
来源：http://read.share.vehdjk.com/Article/details/gomsacvbh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.sjlbkw.cn/Article/details/gbqwearij.sHtML

[T35] Lua：字典表
来源：http://m.share.yfazqb.com/Article/details/gdeannpnr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fktsv.cn/Article/details/gsachfogi.sHtML

[T36] Lua：函数
来源：http://www.blog.bbcook.cn/Article/details/gvegoowhk.sHtML

function add(a, b) return a + b end
来源：http://www.blog.bbcook.cn/Article/details/gtxjkevjv.sHtML

[T37] Lua：字符串拼接
来源：http://blog.bbcook.cn/Article/details/gcxjiybco.sHtML

"a" .. "b"
来源：http://3g.epnwcf.com/Article/details/gcmvadcxe.sHtML

[T38] Lua：条件
来源：http://3g.sjlbkw.cn/Article/details/gjtbquaog.sHtML

if x > 0 then print("正") end
来源：http://m.share.epnwcf.com/Article/details/gambxxbau.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fktsv.cn/Article/details/gpufxccvd.sHtML

string.find(s, "%d+")
来源：http://blog.vehdjk.com/Article/details/gpycsyxur.sHtML

[T40] Lua：元表
来源：http://www.blog.yfazqb.com/Article/details/gizwcdjhj.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fktsv.cn/Article/details/gzlpkyxqn.sHtML

[T41] Perl：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gquycxnnx.sHtML

print "Hello\n";
来源：http://read.share.sjlbkw.cn/Article/details/glmzrowlm.sHtML

[T42] Perl：变量类型
来源：http://read.share.bbcook.cn/Article/details/gcjovhlzk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.sjlbkw.cn/Article/details/grrdodtzu.sHtML

[T43] Perl：字符串插值
来源：http://blog.epnwcf.com/Article/details/gngmxbhqb.sHtML

"值: $a"
来源：http://www.blog.epnwcf.com/Article/details/getwogezj.sHtML

[T44] Perl：条件
来源：http://baike.tarul.cn/Article/details/gbratrohg.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fktsv.cn/Article/details/gkvftdjgq.sHtML

[T45] Perl：数组遍历
来源：http://mobile.epnwcf.com/Article/details/grmbdlfhs.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.bbcook.cn/Article/details/gnzbhkkki.sHtML

[T46] Perl：哈希操作
来源：http://m.share.epnwcf.com/Article/details/gnqabrzpt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.bbcook.cn/Article/details/gujavakgx.sHtML

[T47] Perl：正则捕获
来源：http://baike.epnwcf.com/Article/details/gqtjlfkev.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.yfazqb.com/Article/details/gblcgufmd.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.yfazqb.com/Article/details/guefksmnw.sHtML

$s =~ s/old/new/g;
来源：http://3g.epnwcf.com/Article/details/gfauyinrb.sHtML

[T49] Perl：函数
来源：http://baike.bbcook.cn/Article/details/gplpebduj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/giiwkngkb.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.tarul.cn/Article/details/gecvoxqhi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.tarul.cn/Article/details/gywouojcg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.bbcook.cn/Article/details/gbdeizwpm.sHtML

[T51] Scala：Hello World
来源：http://www.share.fktsv.cn/Article/details/gayrkstji.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gvodplktr.sHtML

[T52] Scala：变量
来源：http://read.share.yfazqb.com/Article/details/gtfzhxgjs.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fktsv.cn/Article/details/giumgvxno.sHtML

[T53] Scala：字符串插值
来源：http://3g.tarul.cn/Article/details/gujnlsjzc.sHtML

s"值: $b"
来源：http://read.share.tarul.cn/Article/details/gqillwgcp.sHtML

[T54] Scala：集合映射
来源：http://www.share.fktsv.cn/Article/details/gcflhpntq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.bbcook.cn/Article/details/gweihmdlc.sHtML

[T55] Scala：集合过滤
来源：http://wap.yfazqb.com/Article/details/gewmgfbpq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.epnwcf.com/Article/details/gkblkxddw.sHtML

[T56] Scala：样例类
来源：http://m.share.vehdjk.com/Article/details/gldaqtzoi.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fktsv.cn/Article/details/gpyefyudy.sHtML

[T57] Scala：模式匹配
来源：http://wap.tarul.cn/Article/details/gncjuehkz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gihvzqwap.sHtML

[T58] Scala：函数定义
来源：http://blog.sjlbkw.cn/Article/details/gtopjlyyr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.tarul.cn/Article/details/gwnpnsmrx.sHtML

[T59] Scala：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gmvtfmcoj.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fktsv.cn/Article/details/gbpdtldfl.sHtML

[T60] Scala：折叠
来源：http://www.blog.bbcook.cn/Article/details/ggsexpzrr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.tarul.cn/Article/details/gblawwlgl.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gyhlejkpn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fktsv.cn/Article/details/gusjbjxhf.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gnyneqevt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.vehdjk.com/Article/details/gccydhddp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fktsv.cn/Article/details/gpyqxblmd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.bbcook.cn/Article/details/gujhlmogr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.vehdjk.com/Article/details/ghjxugoon.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.yfazqb.com/Article/details/gizyajiju.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.vehdjk.com/Article/details/ghbmnuvqy.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/gjcerffao.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.epnwcf.com/Article/details/gnpktbcse.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.bbcook.cn/Article/details/gejrqfybl.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gzhlmprmv.sHtML

[U06] Py：合并两个字典
来源：http://baike.vehdjk.com/Article/details/grfkpcwqx.sHtML

{**a, **b}
来源：http://wap.bbcook.cn/Article/details/gnfwarwes.sHtML

[U07] Py：反转字典键值
来源：http://m.share.vehdjk.com/Article/details/giuhstcgm.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fktsv.cn/Article/details/gltswdghc.sHtML

[U08] Py：展平二维列表
来源：http://wap.bbcook.cn/Article/details/gvduxhkax.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.epnwcf.com/Article/details/gztzljhfk.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.bbcook.cn/Article/details/gvlktoorf.sHtML

max(d, key=d.get)
来源：http://mobile.vehdjk.com/Article/details/gquwbysoy.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/gppokmpoz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.bbcook.cn/Article/details/glhnsfnyh.sHtML

[U11] Py：生成器表达式
来源：http://www.share.epnwcf.com/Article/details/gpnjakqba.sHtML

(x * 2 for x in arr)
来源：http://3g.bbcook.cn/Article/details/gymbyysds.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.epnwcf.com/Article/details/gxzjqaodf.sHtML

Counter(arr).most_common(3)
来源：http://3g.vehdjk.com/Article/details/gyfwtcncj.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.bbcook.cn/Article/details/gkcoypsuw.sHtML

deque(maxlen=10)
来源：http://3g.yfazqb.com/Article/details/gzifsqkbm.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fktsv.cn/Article/details/gxtgsmhzv.sHtML

defaultdict(list)
来源：http://www.share.tarul.cn/Article/details/goafohuky.sHtML

[U15] Py：高精度计时
来源：http://www.share.vehdjk.com/Article/details/gyghxyvui.sHtML

t = time.perf_counter()
来源：http://www.blog.epnwcf.com/Article/details/grzoowtcr.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.bbcook.cn/Article/details/glcpxgqch.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.tarul.cn/Article/details/grrzftiks.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fktsv.cn/Article/details/gawxdolgb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.vehdjk.com/Article/details/ghqlpswla.sHtML

[U18] Py：预编译正则
来源：http://3g.tarul.cn/Article/details/gpocihate.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/gwwrmwhyf.sHtML

[U19] Py：正则替换带回调
来源：http://baike.epnwcf.com/Article/details/gdbvubdwl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.yfazqb.com/Article/details/ggnttebyo.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.yfazqb.com/Article/details/gkhvpxlyc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.yfazqb.com/Article/details/gkucptlda.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fktsv.cn/Article/details/gqqympeqx.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/gyyesfnsk.sHtML

[U22] Py：矩阵转置
来源：http://m.share.epnwcf.com/Article/details/gwwfedudd.sHtML

list(zip(*m))
来源：http://blog.sjlbkw.cn/Article/details/gnpwmbeba.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.bbcook.cn/Article/details/gugkgqmpk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.yfazqb.com/Article/details/geuxblpyg.sHtML

[U24] Py：路径操作
来源：http://www.m.share.tarul.cn/Article/details/gjbayxrdl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gvvuooeth.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fktsv.cn/Article/details/gljxsirmk.sHtML

csv.DictReader(f)
来源：http://read.share.epnwcf.com/Article/details/ghoexxqec.sHtML

[U26] Py：并发下载
来源：http://3g.yfazqb.com/Article/details/gdavrqomf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fktsv.cn/Article/details/gfaarfinc.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fktsv.cn/Article/details/ghmtmhckz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.yfazqb.com/Article/details/gplsrbwqk.sHtML

[U28] Py：类型别名
来源：http://mobile.vehdjk.com/Article/details/gfxggatef.sHtML

UserId = int
来源：http://read.share.tarul.cn/Article/details/gkyxmvpcp.sHtML

[U29] Py：属性校验
来源：http://m.share.vehdjk.com/Article/details/gcxgfgzca.sHtML

@property 与 @x.setter 配合
来源：http://wap.sjlbkw.cn/Article/details/gzvpdjfui.sHtML

[U30] Py：数据类
来源：http://www.blog.epnwcf.com/Article/details/giwtzoogz.sHtML

@dataclass(slots=True)
来源：http://www.blog.tarul.cn/Article/details/gabnwpsps.sHtML

[U31] Py：单测
来源：http://blog.bbcook.cn/Article/details/gbygntdel.sHtML

python -m pytest -q
来源：http://read.share.vehdjk.com/Article/details/gzhomjkaa.sHtML

[U32] Py：代码格式化
来源：http://3g.vehdjk.com/Article/details/gzjmnmxlb.sHtML

ruff format . && ruff check --fix .
来源：http://blog.yfazqb.com/Article/details/glztmtllg.sHtML

[U33] Py：打包发布
来源：http://www.m.share.epnwcf.com/Article/details/grwsuehfi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.yfazqb.com/Article/details/gkjjzvbiu.sHtML

[U34] Py：判断编码
来源：http://blog.fktsv.cn/Article/details/gfxgmdgjh.sHtML

chardet.detect(raw)
来源：http://www.share.epnwcf.com/Article/details/gdpietpvj.sHtML

[U35] Py：发送邮件
来源：http://3g.bbcook.cn/Article/details/ggbfnylpr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.epnwcf.com/Article/details/gaaivlcgi.sHtML

[U36] Py：定时任务
来源：http://baike.sjlbkw.cn/Article/details/gnmrmwshs.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.bbcook.cn/Article/details/guavdcflh.sHtML

[U37] Py：读写 Excel
来源：http://wap.bbcook.cn/Article/details/gpbhtwyms.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.epnwcf.com/Article/details/gezzmbvnc.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fktsv.cn/Article/details/glzwokgqs.sHtML

Path(__file__).resolve().parent
来源：http://www.share.tarul.cn/Article/details/gccgddzdr.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fktsv.cn/Article/details/gikmakswu.sHtML

sys.stdout.isatty()
来源：http://read.share.sjlbkw.cn/Article/details/gaziyrfxn.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.bbcook.cn/Article/details/gomgpaonp.sHtML

print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/glrnhjwov.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.yfazqb.com/Article/details/gyjlxdvxt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.tarul.cn/Article/details/ghkxwpxts.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.tarul.cn/Article/details/ghvfmarmq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.sjlbkw.cn/Article/details/gwhhgsgxg.sHtML

[U43] PHP：声明命名空间
来源：http://blog.vehdjk.com/Article/details/gqeiomsyy.sHtML

namespace App\Http;
来源：http://baike.bbcook.cn/Article/details/gtusnnlec.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fktsv.cn/Article/details/gbgrxlejg.sHtML

declare(strict_types=1);
来源：http://m.share.tarul.cn/Article/details/gzesvgvwa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fktsv.cn/Article/details/gojqunnra.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gusmtfymx.sHtML

[U46] PHP：可空类型
来源：http://wap.tarul.cn/Article/details/gqcgipnjo.sHtML

?string $name = null
来源：http://www.m.share.sjlbkw.cn/Article/details/gbseixzzz.sHtML

[U47] PHP：联合类型
来源：http://www.share.sjlbkw.cn/Article/details/gzzuidsij.sHtML

int|string $id
来源：http://wap.epnwcf.com/Article/details/grkbwsgsv.sHtML

[U48] PHP：纯枚举
来源：http://baike.epnwcf.com/Article/details/gljlwynks.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.tarul.cn/Article/details/gwkwxwgfy.sHtML

[U49] PHP：只读属性
来源：http://3g.bbcook.cn/Article/details/gttrvapko.sHtML

public readonly string $name
来源：http://mobile.vehdjk.com/Article/details/gylkqloyj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.vehdjk.com/Article/details/gpkymdwaq.sHtML

public function __construct(private int $id) {}
来源：http://www.share.yfazqb.com/Article/details/geqbdonpm.sHtML

[U51] PHP：数组解构
来源：http://wap.tarul.cn/Article/details/gblcxibwu.sHtML

[$a, $b] = $arr;
来源：http://wap.epnwcf.com/Article/details/gvtfqahmy.sHtML

[U52] PHP：箭头函数
来源：http://wap.yfazqb.com/Article/details/gbyerjhry.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.bbcook.cn/Article/details/gazzupyqs.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.tarul.cn/Article/details/gvybiemvq.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.sjlbkw.cn/Article/details/gshmkzmse.sHtML

[U54] PHP：空安全调用
来源：http://blog.sjlbkw.cn/Article/details/gyvuzgwah.sHtML

$obj?->method()
来源：http://mobile.yfazqb.com/Article/details/gwemvmlbl.sHtML

[U55] PHP：match 表达式
来源：http://www.share.sjlbkw.cn/Article/details/gyoxbtsgh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.vehdjk.com/Article/details/geavkutxh.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.vehdjk.com/Article/details/ghtgmxgqz.sHtML

f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gsxsuthzx.sHtML

[U57] PHP：字符串插值
来源：http://3g.yfazqb.com/Article/details/gtdetyhmt.sHtML

"值: {$a}"
来源：http://www.share.yfazqb.com/Article/details/gskrqjrrh.sHtML

[U58] PHP：数组三件套
来源：http://www.share.sjlbkw.cn/Article/details/gamjxmoun.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.yfazqb.com/Article/details/ghnetknrb.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fktsv.cn/Article/details/ggbrrvmnd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fktsv.cn/Article/details/ghofxuhvu.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.sjlbkw.cn/Article/details/gwvewnvbv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.tarul.cn/Article/details/gnxgenjud.sHtML

[U61] PHP：正则
来源：http://www.share.bbcook.cn/Article/details/gqwtaenws.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.bbcook.cn/Article/details/gevwhpihj.sHtML

[U62] PHP：日期对象
来源：http://3g.tarul.cn/Article/details/ghcxkfoqe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.tarul.cn/Article/details/gfnaghdje.sHtML

[U63] PHP：文件读写
来源：http://read.share.sjlbkw.cn/Article/details/gvqeksdny.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.bbcook.cn/Article/details/gbfpvvjin.sHtML

[U64] PHP：目录遍历
来源：http://read.share.vehdjk.com/Article/details/gcciucfcm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.sjlbkw.cn/Article/details/ganadifbj.sHtML

[U65] PHP：会话
来源：http://www.share.fktsv.cn/Article/details/gkvgjxxqw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gwjgfvysx.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.vehdjk.com/Article/details/gdeiytwln.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fktsv.cn/Article/details/gvzqdnyfo.sHtML

[U67] PHP：处理文件上传
来源：http://baike.epnwcf.com/Article/details/gdfiizxqi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fktsv.cn/Article/details/gicxjidkg.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.epnwcf.com/Article/details/gglltwlhu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.tarul.cn/Article/details/gncejckif.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.tarul.cn/Article/details/glgepvknt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.tarul.cn/Article/details/gfawwvvtl.sHtML

[U70] PHP：PDO 事务
来源：http://blog.sjlbkw.cn/Article/details/giavsppxn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fktsv.cn/Article/details/gsochvppc.sHtML

[U71] PHP：抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gbrzetbhv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.bbcook.cn/Article/details/gaevkglvu.sHtML

[U72] PHP：写错误日志
来源：http://m.share.epnwcf.com/Article/details/gelxpvavr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fktsv.cn/Article/details/ghjtewgys.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.tarul.cn/Article/details/gvvuelzwx.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.epnwcf.com/Article/details/ginclibtk.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fktsv.cn/Article/details/gpbvyziyn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.epnwcf.com/Article/details/gzcjtmvup.sHtML

[U75] PHP：依赖注入
来源：http://wap.epnwcf.com/Article/details/gpnstnkbr.sHtML

composer require psr/container
来源：http://m.share.vehdjk.com/Article/details/gsozafztz.sHtML

[U76] PHP：简单路由
来源：http://read.share.epnwcf.com/Article/details/gejqmhlfl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.yfazqb.com/Article/details/gjqehoajy.sHtML

[U77] PHP：模板渲染
来源：http://wap.sjlbkw.cn/Article/details/ggnmmqgiu.sHtML

composer require twig/twig
来源：http://3g.yfazqb.com/Article/details/godpshoqb.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/glvyhkaft.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.vehdjk.com/Article/details/grlztxqgl.sHtML


<!-- 参考信息 -->