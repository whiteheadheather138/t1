代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.share.fktsv.cn/Article/details/gbwvkjbev.sHtML

[S49] C++：写文件
来源：http://mobile.tarul.cn/Article/details/gcjoqdjut.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.bbcook.cn/Article/details/gzqgkgesh.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fktsv.cn/Article/details/gecnzicvp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.tarul.cn/Article/details/glfktvdma.sHtML

[S51] C++：显式类型转换
来源：http://blog.tarul.cn/Article/details/gjmofcxam.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/gydirdswj.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.epnwcf.com/Article/details/gtreelaxl.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.yfazqb.com/Article/details/gswlzdruo.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/gzmphkunf.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gdcaxsprk.sHtML

[S54] C++：异常处理
来源：http://www.blog.bbcook.cn/Article/details/gfjcxcjhi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.yfazqb.com/Article/details/gczfjvrrb.sHtML

[S55] C++：结构化绑定
来源：http://mobile.sjlbkw.cn/Article/details/goniwtndm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gckekcmtf.sHtML

[S56] C++：optional
来源：http://baike.bbcook.cn/Article/details/gfjzryfms.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqtgdtqev.sHtML

[S57] C++：编译期常量
来源：http://blog.epnwcf.com/Article/details/gwegflobq.sHtML

constexpr int N = 10;
来源：http://read.share.vehdjk.com/Article/details/ggacztjhd.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/gacgtsdon.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fktsv.cn/Article/details/gzksaiudu.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/gevrddlev.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.vehdjk.com/Article/details/gmcyjwxkn.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/gmbrrmbjv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.tarul.cn/Article/details/glapgqtvt.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbipewvyl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.bbcook.cn/Article/details/gdkkbtukg.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjyrrcace.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fktsv.cn/Article/details/gwawypbyv.sHtML

println("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gftukejui.sHtML

[T02] Kotlin：变量
来源：http://www.blog.vehdjk.com/Article/details/gthnkqina.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.tarul.cn/Article/details/gkqalcalp.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.epnwcf.com/Article/details/gbvjsueiw.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gpqwqswvg.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/gcnunggej.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.tarul.cn/Article/details/gaqondajb.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.tarul.cn/Article/details/guhhwsnmz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.tarul.cn/Article/details/gebyrtpjw.sHtML

[T06] Kotlin：集合映射
来源：http://3g.bbcook.cn/Article/details/glcqomtii.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gavviylsf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gdphjiyzn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.epnwcf.com/Article/details/gkvuocrxi.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/gnmesrqjs.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/gyptbasfy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/gkiyuqujf.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.tarul.cn/Article/details/gzbamrbih.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.epnwcf.com/Article/details/galyawrhu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.sjlbkw.cn/Article/details/gcsdozeni.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gemnhjzuk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.yfazqb.com/Article/details/gsqpkzzll.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.epnwcf.com/Article/details/gbmmekunx.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/gyzeclwte.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.epnwcf.com/Article/details/gfrhgtjkf.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.tarul.cn/Article/details/gvhmqrnql.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gwoyxoaej.sHtML

for (i in 1..10) println(i)
来源：http://wap.epnwcf.com/Article/details/gsbuienqf.sHtML

[T15] Kotlin：接口
来源：http://wap.vehdjk.com/Article/details/gsfjbdzdr.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fktsv.cn/Article/details/gkiefwkok.sHtML

[T16] Swift：Hello World
来源：http://read.share.fktsv.cn/Article/details/gwemltmdu.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gllcwjkdt.sHtML

[T17] Swift：变量与常量
来源：http://baike.epnwcf.com/Article/details/gkukybrmk.sHtML

var a = 1;  let b = 2
来源：http://www.share.yfazqb.com/Article/details/ggkxdpqti.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gdkwcnggs.sHtML

"值: \(b)"
来源：http://baike.vehdjk.com/Article/details/gqdpepeqg.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gfcrysmkf.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/gstqgdfrw.sHtML

[T20] Swift：数组操作
来源：http://read.share.vehdjk.com/Article/details/goausvali.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.epnwcf.com/Article/details/gvwanlnfo.sHtML

[T21] Swift：遍历
来源：http://blog.epnwcf.com/Article/details/giilwtkzh.sHtML

for x in a { print(x) }
来源：http://www.blog.sjlbkw.cn/Article/details/glzygifgb.sHtML

[T22] Swift：字典
来源：http://www.share.epnwcf.com/Article/details/grdpgbcei.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gvbmjjgqb.sHtML

[T23] Swift：函数
来源：http://wap.yfazqb.com/Article/details/guhlkrywp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fktsv.cn/Article/details/gzsdywlft.sHtML

[T24] Swift：闭包
来源：http://wap.fktsv.cn/Article/details/gtmvthbuu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.bbcook.cn/Article/details/ggayqbxmp.sHtML

[T25] Swift：结构体
来源：http://read.share.bbcook.cn/Article/details/geprfoheq.sHtML

struct P { var x: Int }
来源：http://baike.tarul.cn/Article/details/gjhewtykl.sHtML

[T26] Swift：类与重写
来源：http://blog.tarul.cn/Article/details/gqsbzihmk.sHtML

class A: Base { override func f() {} }
来源：http://3g.fktsv.cn/Article/details/gqsnhuuxx.sHtML

[T27] Swift：错误处理
来源：http://blog.yfazqb.com/Article/details/gvysjwadj.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.epnwcf.com/Article/details/gwjgpqpzr.sHtML

[T28] Swift：枚举
来源：http://blog.vehdjk.com/Article/details/glqzoaaob.sHtML

enum Color { case red, green }
来源：http://blog.fktsv.cn/Article/details/gdbiljgcm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.epnwcf.com/Article/details/glugnqlzq.sHtML

guard let x = opt else { return }
来源：http://blog.epnwcf.com/Article/details/gmvtgcdpz.sHtML

[T30] Swift：协议
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmwacxwp.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.sjlbkw.cn/Article/details/ghhkiqhnm.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/ghadmgknn.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/grmuvrwnn.sHtML

[T32] Lua：局部变量
来源：http://mobile.tarul.cn/Article/details/gpimetspe.sHtML

local a = 1
来源：http://mobile.yfazqb.com/Article/details/gvqydwgxw.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fktsv.cn/Article/details/gmydkyvze.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fktsv.cn/Article/details/gsbycobhk.sHtML

[T34] Lua：遍历表
来源：http://wap.vehdjk.com/Article/details/gribyvfkq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.tarul.cn/Article/details/gcuawtdvr.sHtML

[T35] Lua：字典表
来源：http://3g.tarul.cn/Article/details/gslsfwkjs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.vehdjk.com/Article/details/gxsetdoil.sHtML

[T36] Lua：函数
来源：http://mobile.epnwcf.com/Article/details/gdhnepoem.sHtML

function add(a, b) return a + b end
来源：http://baike.bbcook.cn/Article/details/grtmrnmvv.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gqcqmsuwe.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/gwxzgjmui.sHtML

[T38] Lua：条件
来源：http://read.share.epnwcf.com/Article/details/gbtqdtzdh.sHtML

if x > 0 then print("正") end
来源：http://www.share.yfazqb.com/Article/details/gkrlbmlzp.sHtML

[T39] Lua：模式匹配
来源：http://read.share.bbcook.cn/Article/details/gntrijalu.sHtML

string.find(s, "%d+")
来源：http://baike.tarul.cn/Article/details/gbgyrstjb.sHtML

[T40] Lua：元表
来源：http://3g.yfazqb.com/Article/details/grzxhwzer.sHtML

setmetatable({}, { __index = base })
来源：http://blog.yfazqb.com/Article/details/gnrvdnmuq.sHtML

[T41] Perl：Hello World
来源：http://m.share.epnwcf.com/Article/details/gzvnxlkaa.sHtML

print "Hello\n";
来源：http://www.m.share.fktsv.cn/Article/details/gaiwfrlyb.sHtML

[T42] Perl：变量类型
来源：http://www.share.epnwcf.com/Article/details/glcihioei.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.yfazqb.com/Article/details/gqlwnwlag.sHtML

[T43] Perl：字符串插值
来源：http://www.share.yfazqb.com/Article/details/girpgrbhm.sHtML

"值: $a"
来源：http://read.share.epnwcf.com/Article/details/giqbcmcbl.sHtML

[T44] Perl：条件
来源：http://read.share.tarul.cn/Article/details/gmowbokby.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.tarul.cn/Article/details/gigzhptls.sHtML

[T45] Perl：数组遍历
来源：http://3g.tarul.cn/Article/details/gdfeolwkc.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.epnwcf.com/Article/details/gplcnhrpt.sHtML

[T46] Perl：哈希操作
来源：http://blog.vehdjk.com/Article/details/gdorujxcs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.vehdjk.com/Article/details/gcfjkbfbg.sHtML

[T47] Perl：正则捕获
来源：http://m.share.sjlbkw.cn/Article/details/gkeajylvt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.bbcook.cn/Article/details/guptzxavc.sHtML

[T48] Perl：正则替换
来源：http://www.share.fktsv.cn/Article/details/gxuxafzcm.sHtML

$s =~ s/old/new/g;
来源：http://mobile.vehdjk.com/Article/details/glwsougxv.sHtML

[T49] Perl：函数
来源：http://www.m.share.vehdjk.com/Article/details/gcazukcep.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gvuyaxgwz.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gjjhfdkfy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.vehdjk.com/Article/details/glicuoghu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gozqprerb.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/ggkfjuyjw.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/glvdukpti.sHtML

[T52] Scala：变量
来源：http://www.m.share.bbcook.cn/Article/details/gbleipijb.sHtML

val a = 1;  var b = 2
来源：http://www.share.yfazqb.com/Article/details/ghtglqpsh.sHtML

[T53] Scala：字符串插值
来源：http://wap.yfazqb.com/Article/details/gqjrjmkvf.sHtML

s"值: $b"
来源：http://blog.tarul.cn/Article/details/gxtezdfei.sHtML

[T54] Scala：集合映射
来源：http://blog.vehdjk.com/Article/details/grgobqsrf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.bbcook.cn/Article/details/glnydould.sHtML

[T55] Scala：集合过滤
来源：http://baike.yfazqb.com/Article/details/gkxfpwchx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.vehdjk.com/Article/details/gesnufvgc.sHtML

[T56] Scala：样例类
来源：http://www.m.share.yfazqb.com/Article/details/gboguytra.sHtML

case class User(name: String, age: Int)
来源：http://baike.bbcook.cn/Article/details/gdznyvhzt.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gplooohsg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.tarul.cn/Article/details/gqmmpqfjc.sHtML

[T58] Scala：函数定义
来源：http://mobile.yfazqb.com/Article/details/gqlhgynhy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.epnwcf.com/Article/details/gtgiabptk.sHtML

[T59] Scala：循环
来源：http://blog.bbcook.cn/Article/details/grfmbzqtl.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.yfazqb.com/Article/details/ggtlyhhei.sHtML

[T60] Scala：折叠
来源：http://blog.tarul.cn/Article/details/gosdgqudz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.yfazqb.com/Article/details/gaelhqiif.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gnbkyhbgk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.bbcook.cn/Article/details/gcuvapoqs.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gxxfvrvox.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.bbcook.cn/Article/details/gtjglnfxv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.epnwcf.com/Article/details/gpfhcntnc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.bbcook.cn/Article/details/gqrlpetow.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.sjlbkw.cn/Article/details/gtmbdxbhj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.tarul.cn/Article/details/gfvkhphye.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fktsv.cn/Article/details/grdocfzzl.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/gvhcmlihc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.tarul.cn/Article/details/gyosnoywk.sHtML

[U05] Py：列表去重且保序
来源：http://baike.vehdjk.com/Article/details/gschnunsf.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gbsrsrevi.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fktsv.cn/Article/details/gnhhynvgw.sHtML

{**a, **b}
来源：http://baike.sjlbkw.cn/Article/details/gsxwzslwh.sHtML

[U07] Py：反转字典键值
来源：http://3g.bbcook.cn/Article/details/gcjoooojq.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fktsv.cn/Article/details/glaawdoku.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.epnwcf.com/Article/details/gvlhpugtb.sHtML

[y for x in nested for y in x]
来源：http://www.share.epnwcf.com/Article/details/gxtydxpbj.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.yfazqb.com/Article/details/gvdzolqjz.sHtML

max(d, key=d.get)
来源：http://3g.epnwcf.com/Article/details/gaugruivp.sHtML

[U10] Py：按值排序字典
来源：http://blog.epnwcf.com/Article/details/gpjxmztkf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.yfazqb.com/Article/details/gcxnrlthf.sHtML

[U11] Py：生成器表达式
来源：http://baike.bbcook.cn/Article/details/gjdfnoamh.sHtML

(x * 2 for x in arr)
来源：http://m.share.sjlbkw.cn/Article/details/gmahceejy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fktsv.cn/Article/details/gzublhujt.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.tarul.cn/Article/details/gjervhzzf.sHtML

[U13] Py：固定长度队列
来源：http://3g.fktsv.cn/Article/details/gizttbzow.sHtML

deque(maxlen=10)
来源：http://baike.yfazqb.com/Article/details/gnouajvua.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.bbcook.cn/Article/details/gjixrraju.sHtML

defaultdict(list)
来源：http://read.share.sjlbkw.cn/Article/details/guqvjltvx.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.epnwcf.com/Article/details/grcgsrjjw.sHtML

t = time.perf_counter()
来源：http://www.m.share.tarul.cn/Article/details/gmreuqcki.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.vehdjk.com/Article/details/gdsuyrzlp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfhlidhd.sHtML

[U17] Py：初始化日志
来源：http://m.share.bbcook.cn/Article/details/gynenqjuq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.yfazqb.com/Article/details/gzvtryggg.sHtML

[U18] Py：预编译正则
来源：http://3g.sjlbkw.cn/Article/details/gayxworka.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.yfazqb.com/Article/details/gxfmdnoyb.sHtML

[U19] Py：正则替换带回调
来源：http://3g.yfazqb.com/Article/details/gabiraivh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.sjlbkw.cn/Article/details/gdleplfqg.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.epnwcf.com/Article/details/gxcqgfqsk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.tarul.cn/Article/details/gylsvqspt.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.sjlbkw.cn/Article/details/gprfnkzmv.sHtML

@contextlib.contextmanager
来源：http://m.share.vehdjk.com/Article/details/glcrymhtt.sHtML

[U22] Py：矩阵转置
来源：http://baike.vehdjk.com/Article/details/gtbnxclyj.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/gzdlrkika.sHtML

[U23] Py：分块读取大文件
来源：http://3g.sjlbkw.cn/Article/details/gdopepepw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.epnwcf.com/Article/details/gelhwwjtp.sHtML

[U24] Py：路径操作
来源：http://baike.fktsv.cn/Article/details/ghslnciqn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.yfazqb.com/Article/details/goxufooev.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.vehdjk.com/Article/details/gljsirpoo.sHtML

csv.DictReader(f)
来源：http://blog.yfazqb.com/Article/details/glxbbxanx.sHtML

[U26] Py：并发下载
来源：http://m.share.vehdjk.com/Article/details/gnedkguvh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.epnwcf.com/Article/details/gzseesadi.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fktsv.cn/Article/details/gbhmtbwas.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.epnwcf.com/Article/details/grxpwgbju.sHtML

[U28] Py：类型别名
来源：http://3g.yfazqb.com/Article/details/gnalshsnn.sHtML

UserId = int
来源：http://blog.sjlbkw.cn/Article/details/gdybkrfux.sHtML

[U29] Py：属性校验
来源：http://blog.sjlbkw.cn/Article/details/gpszmblii.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fktsv.cn/Article/details/goerjfqcs.sHtML

[U30] Py：数据类
来源：http://read.share.tarul.cn/Article/details/gdifuxong.sHtML

@dataclass(slots=True)
来源：http://read.share.sjlbkw.cn/Article/details/gylygheyi.sHtML

[U31] Py：单测
来源：http://www.share.bbcook.cn/Article/details/gdzqyrbha.sHtML

python -m pytest -q
来源：http://wap.vehdjk.com/Article/details/ggfvnprtp.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.epnwcf.com/Article/details/ghrvmeauo.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.epnwcf.com/Article/details/gbtaefilx.sHtML

[U33] Py：打包发布
来源：http://www.share.tarul.cn/Article/details/gmafomjpw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.yfazqb.com/Article/details/gulnzbsci.sHtML

[U34] Py：判断编码
来源：http://m.share.fktsv.cn/Article/details/gnnthxqfe.sHtML

chardet.detect(raw)
来源：http://3g.yfazqb.com/Article/details/gkcdvkxdy.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fktsv.cn/Article/details/gaiioajqw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.vehdjk.com/Article/details/gigqzfhrt.sHtML

[U36] Py：定时任务
来源：http://wap.sjlbkw.cn/Article/details/gbwzfdxdd.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.bbcook.cn/Article/details/gkqjwbevv.sHtML

[U37] Py：读写 Excel
来源：http://mobile.yfazqb.com/Article/details/gllposlnc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.yfazqb.com/Article/details/gmqyreirh.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.sjlbkw.cn/Article/details/ghnnvstsb.sHtML

Path(__file__).resolve().parent
来源：http://www.share.vehdjk.com/Article/details/gyyuktnry.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.sjlbkw.cn/Article/details/gkhmkcdei.sHtML

sys.stdout.isatty()
来源：http://blog.vehdjk.com/Article/details/gqpvacoyd.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.vehdjk.com/Article/details/girveiaga.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fktsv.cn/Article/details/grgtrvueh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.vehdjk.com/Article/details/ggvzwjwdz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.yfazqb.com/Article/details/gbikjkyuu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fktsv.cn/Article/details/gjlptdwng.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fktsv.cn/Article/details/gaefoihde.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.tarul.cn/Article/details/gnboitocv.sHtML

namespace App\Http;
来源：http://read.share.yfazqb.com/Article/details/gtodfofyi.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.epnwcf.com/Article/details/gcnaytlvp.sHtML

declare(strict_types=1);
来源：http://3g.tarul.cn/Article/details/gcxiviyww.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.tarul.cn/Article/details/gmxhmyvpb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gxesenyfx.sHtML

[U46] PHP：可空类型
来源：http://3g.sjlbkw.cn/Article/details/gfgyfgtww.sHtML

?string $name = null
来源：http://wap.epnwcf.com/Article/details/gasjqhhem.sHtML

[U47] PHP：联合类型
来源：http://mobile.sjlbkw.cn/Article/details/ghhyvrpdr.sHtML

int|string $id
来源：http://wap.yfazqb.com/Article/details/geyaptylz.sHtML

[U48] PHP：纯枚举
来源：http://mobile.bbcook.cn/Article/details/gvkbtmwio.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.tarul.cn/Article/details/gbvzxrcdk.sHtML

[U49] PHP：只读属性
来源：http://baike.yfazqb.com/Article/details/gumohthqa.sHtML

public readonly string $name
来源：http://www.m.share.bbcook.cn/Article/details/gquwpfpzk.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.tarul.cn/Article/details/gumapxpjg.sHtML

public function __construct(private int $id) {}
来源：http://blog.yfazqb.com/Article/details/gqcdlnuvs.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.yfazqb.com/Article/details/gnnlzjamk.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fktsv.cn/Article/details/goxfmlqgp.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gpadcfchn.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.vehdjk.com/Article/details/gauicswbp.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.tarul.cn/Article/details/gjiadibwz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fktsv.cn/Article/details/givytswyh.sHtML

[U54] PHP：空安全调用
来源：http://mobile.bbcook.cn/Article/details/ggmitybuc.sHtML

$obj?->method()
来源：http://www.blog.tarul.cn/Article/details/gmxiphjcv.sHtML

[U55] PHP：match 表达式
来源：http://blog.fktsv.cn/Article/details/gkkwlnufp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.vehdjk.com/Article/details/gmtuxuvtp.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gwxbrhcyt.sHtML

f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gaowotbvh.sHtML

[U57] PHP：字符串插值
来源：http://3g.vehdjk.com/Article/details/ghivbkkxv.sHtML

"值: {$a}"
来源：http://3g.fktsv.cn/Article/details/gekvprxlh.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fktsv.cn/Article/details/gccnsfmjd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.vehdjk.com/Article/details/gjvjhkueq.sHtML

[U59] PHP：自定义排序
来源：http://m.share.tarul.cn/Article/details/gocsycido.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.sjlbkw.cn/Article/details/guvxccwju.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.sjlbkw.cn/Article/details/ghdujrfai.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.epnwcf.com/Article/details/gfmexxeqg.sHtML

[U61] PHP：正则
来源：http://m.share.fktsv.cn/Article/details/gevywgxgj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.vehdjk.com/Article/details/guzoevgxo.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fktsv.cn/Article/details/gwhwatgmw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.yfazqb.com/Article/details/gpmxgpnhm.sHtML

[U63] PHP：文件读写
来源：http://m.share.tarul.cn/Article/details/gkpvoppvk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.vehdjk.com/Article/details/gqqpcqdzv.sHtML

[U64] PHP：目录遍历
来源：http://mobile.yfazqb.com/Article/details/gbevlhedd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.yfazqb.com/Article/details/ggltfnazn.sHtML

[U65] PHP：会话
来源：http://m.share.yfazqb.com/Article/details/gowsntods.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.epnwcf.com/Article/details/gkdnichee.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fktsv.cn/Article/details/gfmcdtuyn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.bbcook.cn/Article/details/gvkeqrpvn.sHtML

[U67] PHP：处理文件上传
来源：http://baike.yfazqb.com/Article/details/griblpykq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.vehdjk.com/Article/details/gglpfktqi.sHtML

[U68] PHP：PDO 连接
来源：http://baike.sjlbkw.cn/Article/details/gzurcfdua.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.epnwcf.com/Article/details/gwpetftuu.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.epnwcf.com/Article/details/gzvullqvw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.yfazqb.com/Article/details/gybvipkka.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.sjlbkw.cn/Article/details/gofwqtzbp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.epnwcf.com/Article/details/ghfwqhcyx.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gxfqlumhh.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.vehdjk.com/Article/details/gjatzboiz.sHtML

[U72] PHP：写错误日志
来源：http://read.share.vehdjk.com/Article/details/gnmmlswwl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.bbcook.cn/Article/details/gkpcserhu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.epnwcf.com/Article/details/glsabmrgi.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.vehdjk.com/Article/details/gpzpulkdy.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gipesvfop.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.bbcook.cn/Article/details/gknxjekpy.sHtML


<!-- 参考信息 -->