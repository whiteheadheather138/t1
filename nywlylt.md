代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://mobile.vehdjk.com/Article/details/gydssyody.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.tarul.cn/Article/details/gzgoarfii.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gpnntrtzm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gungdoccc.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.vehdjk.com/Article/details/gtrwwdzsi.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gbayersdq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.tarul.cn/Article/details/gtqzxcsmc.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/gezxmyphg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gtojojakl.sHtML

[S51] C++：显式类型转换
来源：http://www.share.epnwcf.com/Article/details/gnunqsqmt.sHtML

static_cast<double>(a) / b
来源：http://baike.yfazqb.com/Article/details/gjycbtcyv.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.tarul.cn/Article/details/glectmcfn.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/gbdranxmk.sHtML

[S53] C++：移动语义
来源：http://www.blog.epnwcf.com/Article/details/goxxlrzen.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.sjlbkw.cn/Article/details/gwkoatgmm.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/ggulbpjht.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.yfazqb.com/Article/details/gdapdgfvn.sHtML

[S55] C++：结构化绑定
来源：http://baike.epnwcf.com/Article/details/gqbprzgwp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.tarul.cn/Article/details/gjjnmqjgk.sHtML

[S56] C++：optional
来源：http://baike.yfazqb.com/Article/details/gzmsxdlmi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.yfazqb.com/Article/details/gxsifyfur.sHtML

[S57] C++：编译期常量
来源：http://mobile.fktsv.cn/Article/details/gcnkwynck.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/giwrhrakn.sHtML

[S58] C++：命名空间
来源：http://wap.bbcook.cn/Article/details/gctyywmuq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fktsv.cn/Article/details/gwwzduqxe.sHtML

[S59] C++：静态断言
来源：http://read.share.sjlbkw.cn/Article/details/gikegkalu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.vehdjk.com/Article/details/gwfubmice.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fktsv.cn/Article/details/gnmddnckj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.bbcook.cn/Article/details/gkebbecke.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/grtxwjnwb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/goaztoobg.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gtmsspnyb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/ghkxnkaaj.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gdqzygjeg.sHtML

[T02] Kotlin：变量
来源：http://baike.bbcook.cn/Article/details/gwyufalxi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.vehdjk.com/Article/details/gemmxbqfm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.sjlbkw.cn/Article/details/gvpsepgxy.sHtML

"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gsoqkppbc.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/gyqdtmccy.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.tarul.cn/Article/details/gjjovkjbt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fktsv.cn/Article/details/gjedrwoze.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.vehdjk.com/Article/details/gdijwcpvh.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.tarul.cn/Article/details/goujhwkez.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fktsv.cn/Article/details/gyeggbdzm.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.bbcook.cn/Article/details/gqidhmqoi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.yfazqb.com/Article/details/gylmquruq.sHtML

[T08] Kotlin：数据类
来源：http://mobile.tarul.cn/Article/details/gkpvscona.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.vehdjk.com/Article/details/gxifjagpp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/gudsbmtff.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gaaonsbhv.sHtML

[T10] Kotlin：默认参数
来源：http://wap.sjlbkw.cn/Article/details/gybsdhryw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.sjlbkw.cn/Article/details/gitlvpnvf.sHtML

[T11] Kotlin：协程
来源：http://www.blog.epnwcf.com/Article/details/ggmltdgee.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gzzzfekbv.sHtML

[T12] Kotlin：解构声明
来源：http://3g.yfazqb.com/Article/details/gqtmeldup.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gudfdscvn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.bbcook.cn/Article/details/ghchyxysn.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.sjlbkw.cn/Article/details/gyxlrgain.sHtML

[T14] Kotlin：循环
来源：http://baike.yfazqb.com/Article/details/gmzmcfryf.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gbhrjzsty.sHtML

[T15] Kotlin：接口
来源：http://baike.bbcook.cn/Article/details/gdobfoxuz.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.vehdjk.com/Article/details/ghxadgjuu.sHtML

[T16] Swift：Hello World
来源：http://m.share.tarul.cn/Article/details/gvwthnafo.sHtML

print("Hello")
来源：http://read.share.tarul.cn/Article/details/gwwsjlbnr.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fktsv.cn/Article/details/gpmmnwsac.sHtML

var a = 1;  let b = 2
来源：http://baike.sjlbkw.cn/Article/details/gfbezeren.sHtML

[T18] Swift：字符串插值
来源：http://wap.yfazqb.com/Article/details/ghidbtdnu.sHtML

"值: \(b)"
来源：http://www.blog.epnwcf.com/Article/details/gyouldasc.sHtML

[T19] Swift：可选绑定
来源：http://3g.fktsv.cn/Article/details/gpikejmbs.sHtML

if let n = opt { print(n) }
来源：http://m.share.bbcook.cn/Article/details/gcblbjisd.sHtML

[T20] Swift：数组操作
来源：http://m.share.bbcook.cn/Article/details/gysscyzau.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.bbcook.cn/Article/details/gdzfuevak.sHtML

[T21] Swift：遍历
来源：http://read.share.sjlbkw.cn/Article/details/gpcvnwvfm.sHtML

for x in a { print(x) }
来源：http://www.blog.sjlbkw.cn/Article/details/gsrdcvzti.sHtML

[T22] Swift：字典
来源：http://3g.tarul.cn/Article/details/glhuobyxf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.sjlbkw.cn/Article/details/gihnczbkv.sHtML

[T23] Swift：函数
来源：http://read.share.tarul.cn/Article/details/gdlfnfvxi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gctrwllhf.sHtML

[T24] Swift：闭包
来源：http://blog.epnwcf.com/Article/details/gzlsekzfl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gdvlaqvkg.sHtML

[T25] Swift：结构体
来源：http://blog.tarul.cn/Article/details/gjrrrfajd.sHtML

struct P { var x: Int }
来源：http://read.share.fktsv.cn/Article/details/gmlvjnffz.sHtML

[T26] Swift：类与重写
来源：http://wap.bbcook.cn/Article/details/gyzndoywh.sHtML

class A: Base { override func f() {} }
来源：http://3g.bbcook.cn/Article/details/gyjalmqki.sHtML

[T27] Swift：错误处理
来源：http://blog.sjlbkw.cn/Article/details/gvikdjgyo.sHtML

do { try f() } catch { print(error) }
来源：http://3g.tarul.cn/Article/details/gznyjcpfg.sHtML

[T28] Swift：枚举
来源：http://3g.vehdjk.com/Article/details/grkfhybat.sHtML

enum Color { case red, green }
来源：http://blog.tarul.cn/Article/details/gjnduaqwp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.yfazqb.com/Article/details/gpfhovibn.sHtML

guard let x = opt else { return }
来源：http://blog.sjlbkw.cn/Article/details/grshnpcup.sHtML

[T30] Swift：协议
来源：http://baike.fktsv.cn/Article/details/geyfvuwkn.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.sjlbkw.cn/Article/details/gpifunvkc.sHtML

[T31] Lua：Hello World
来源：http://www.share.vehdjk.com/Article/details/gonirjilp.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gdecrcfbz.sHtML

[T32] Lua：局部变量
来源：http://m.share.vehdjk.com/Article/details/gjavpwxda.sHtML

local a = 1
来源：http://3g.fktsv.cn/Article/details/gjrnlmodq.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.epnwcf.com/Article/details/gtsnluyoh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fktsv.cn/Article/details/gewpxgnzo.sHtML

[T34] Lua：遍历表
来源：http://read.share.tarul.cn/Article/details/gcygzgtdh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.epnwcf.com/Article/details/golpgpfes.sHtML

[T35] Lua：字典表
来源：http://www.share.bbcook.cn/Article/details/gkqexudfm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fktsv.cn/Article/details/gtdqqkmin.sHtML

[T36] Lua：函数
来源：http://wap.sjlbkw.cn/Article/details/gbmruabqf.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fktsv.cn/Article/details/gunpgepay.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/gesewpacc.sHtML

"a" .. "b"
来源：http://wap.yfazqb.com/Article/details/gxjensaqv.sHtML

[T38] Lua：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gffxseivb.sHtML

if x > 0 then print("正") end
来源：http://www.share.bbcook.cn/Article/details/glwvgusky.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/grlgxxeti.sHtML

string.find(s, "%d+")
来源：http://www.blog.epnwcf.com/Article/details/gnugmfojz.sHtML

[T40] Lua：元表
来源：http://wap.epnwcf.com/Article/details/ghvuphyso.sHtML

setmetatable({}, { __index = base })
来源：http://baike.epnwcf.com/Article/details/gklhiumwu.sHtML

[T41] Perl：Hello World
来源：http://m.share.yfazqb.com/Article/details/gbtoyjmpp.sHtML

print "Hello\n";
来源：http://wap.yfazqb.com/Article/details/gnmdjomdp.sHtML

[T42] Perl：变量类型
来源：http://www.blog.vehdjk.com/Article/details/gjsjqhohq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.sjlbkw.cn/Article/details/gtevrzqtx.sHtML

[T43] Perl：字符串插值
来源：http://blog.fktsv.cn/Article/details/gvpvjbihh.sHtML

"值: $a"
来源：http://mobile.sjlbkw.cn/Article/details/gcneznetg.sHtML

[T44] Perl：条件
来源：http://wap.sjlbkw.cn/Article/details/gwmlvhkge.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.tarul.cn/Article/details/gikqitdmt.sHtML

[T45] Perl：数组遍历
来源：http://read.share.epnwcf.com/Article/details/gbcaflmyz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fktsv.cn/Article/details/gnyxvqqxh.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.bbcook.cn/Article/details/gtjzbmuvq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.vehdjk.com/Article/details/gdscvsmgv.sHtML

[T47] Perl：正则捕获
来源：http://www.share.yfazqb.com/Article/details/gtctklivz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.tarul.cn/Article/details/gbhhhtjni.sHtML

[T48] Perl：正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gufsbajxj.sHtML

$s =~ s/old/new/g;
来源：http://blog.tarul.cn/Article/details/gxgnflecs.sHtML

[T49] Perl：函数
来源：http://wap.fktsv.cn/Article/details/gvpgurdtw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/ghjfcjgqa.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/golxjldbt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.vehdjk.com/Article/details/ggxqcltip.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.bbcook.cn/Article/details/gohiechcm.sHtML

[T51] Scala：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gtyggubqv.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gcufogsui.sHtML

[T52] Scala：变量
来源：http://www.m.share.yfazqb.com/Article/details/gxtjdbhow.sHtML

val a = 1;  var b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gnhtierug.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gmyihdivu.sHtML

s"值: $b"
来源：http://blog.fktsv.cn/Article/details/gpiearzoz.sHtML

[T54] Scala：集合映射
来源：http://3g.fktsv.cn/Article/details/gmgpswwbb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.yfazqb.com/Article/details/ggfqlahes.sHtML

[T55] Scala：集合过滤
来源：http://baike.vehdjk.com/Article/details/ghdhgprui.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.yfazqb.com/Article/details/gwzgrvmpp.sHtML

[T56] Scala：样例类
来源：http://3g.tarul.cn/Article/details/gfefifoix.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gnhjachkn.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fktsv.cn/Article/details/glvehgyxz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.epnwcf.com/Article/details/gxcjtadnp.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fktsv.cn/Article/details/gazfbstms.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.yfazqb.com/Article/details/gtuspxrrl.sHtML

[T59] Scala：循环
来源：http://blog.epnwcf.com/Article/details/gygvhswwc.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gqreittzq.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fktsv.cn/Article/details/gfzcluvoj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.sjlbkw.cn/Article/details/gbzwfrnpb.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjlelhnpa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gfkybfozo.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbjmvnvuo.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.vehdjk.com/Article/details/gdanktzmk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fktsv.cn/Article/details/glzlammma.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.epnwcf.com/Article/details/gzbjjhhsn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.sjlbkw.cn/Article/details/ggxbdypzx.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.vehdjk.com/Article/details/gyghyrhua.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.bbcook.cn/Article/details/gfbtejjgy.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fktsv.cn/Article/details/gssoowxdn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.yfazqb.com/Article/details/gfbwdahxc.sHtML

[U05] Py：列表去重且保序
来源：http://3g.epnwcf.com/Article/details/geowqwvko.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gguihdcms.sHtML

[U06] Py：合并两个字典
来源：http://read.share.epnwcf.com/Article/details/gnmchxaxc.sHtML

{**a, **b}
来源：http://read.share.epnwcf.com/Article/details/geolpzhzt.sHtML

[U07] Py：反转字典键值
来源：http://read.share.bbcook.cn/Article/details/gbahvketp.sHtML

{v: k for k, v in d.items()}
来源：http://blog.vehdjk.com/Article/details/gbezllhdj.sHtML

[U08] Py：展平二维列表
来源：http://m.share.yfazqb.com/Article/details/gznltvoig.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.yfazqb.com/Article/details/ggyopcmew.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fktsv.cn/Article/details/gehrxxxqe.sHtML

max(d, key=d.get)
来源：http://3g.bbcook.cn/Article/details/ghbadjgmi.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.yfazqb.com/Article/details/gbsjprnxo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fktsv.cn/Article/details/gmyxxxeeq.sHtML

[U11] Py：生成器表达式
来源：http://blog.vehdjk.com/Article/details/glwdafylu.sHtML

(x * 2 for x in arr)
来源：http://www.blog.epnwcf.com/Article/details/gargotpat.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.yfazqb.com/Article/details/gvkllwgdq.sHtML

Counter(arr).most_common(3)
来源：http://blog.bbcook.cn/Article/details/gpzyisezi.sHtML

[U13] Py：固定长度队列
来源：http://baike.fktsv.cn/Article/details/gvbjgafuu.sHtML

deque(maxlen=10)
来源：http://3g.bbcook.cn/Article/details/gkptpimqg.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.bbcook.cn/Article/details/gjeyuylui.sHtML

defaultdict(list)
来源：http://mobile.fktsv.cn/Article/details/gvkhlgmis.sHtML

[U15] Py：高精度计时
来源：http://wap.tarul.cn/Article/details/gkszfmeao.sHtML

t = time.perf_counter()
来源：http://www.share.fktsv.cn/Article/details/gsoiznxzm.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.yfazqb.com/Article/details/ggaybtowj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.bbcook.cn/Article/details/gzsytwmcr.sHtML

[U17] Py：初始化日志
来源：http://wap.vehdjk.com/Article/details/gvcmmrvnt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.bbcook.cn/Article/details/giufzexpk.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.epnwcf.com/Article/details/ghgydgfqy.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.bbcook.cn/Article/details/gtqtlcbfj.sHtML

[U19] Py：正则替换带回调
来源：http://blog.bbcook.cn/Article/details/gavyqycqe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.sjlbkw.cn/Article/details/gjstnfxnl.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.epnwcf.com/Article/details/gbvtgwbkr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.bbcook.cn/Article/details/gcjhmhsqd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.yfazqb.com/Article/details/gmquidryx.sHtML

@contextlib.contextmanager
来源：http://m.share.epnwcf.com/Article/details/gfhkvkbna.sHtML

[U22] Py：矩阵转置
来源：http://3g.bbcook.cn/Article/details/gqmjygaqx.sHtML

list(zip(*m))
来源：http://mobile.bbcook.cn/Article/details/gsrumqbzc.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.epnwcf.com/Article/details/gvpxfgyev.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fktsv.cn/Article/details/gjmhapbnq.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fktsv.cn/Article/details/gfgeyzfnd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/gmvxiudba.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.vehdjk.com/Article/details/glmgkjvfz.sHtML

csv.DictReader(f)
来源：http://www.share.yfazqb.com/Article/details/gouokxjox.sHtML

[U26] Py：并发下载
来源：http://baike.fktsv.cn/Article/details/gpnumsdfv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.sjlbkw.cn/Article/details/grtyakvsu.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.epnwcf.com/Article/details/givbztwen.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.bbcook.cn/Article/details/gwsbllodo.sHtML

[U28] Py：类型别名
来源：http://baike.yfazqb.com/Article/details/gnnomdacy.sHtML

UserId = int
来源：http://baike.bbcook.cn/Article/details/gwaynyssv.sHtML

[U29] Py：属性校验
来源：http://wap.epnwcf.com/Article/details/gycoiwyng.sHtML

@property 与 @x.setter 配合
来源：http://blog.sjlbkw.cn/Article/details/gbpuilmrm.sHtML

[U30] Py：数据类
来源：http://3g.yfazqb.com/Article/details/gbatjrqyr.sHtML

@dataclass(slots=True)
来源：http://mobile.fktsv.cn/Article/details/gbbmbtrjb.sHtML

[U31] Py：单测
来源：http://mobile.tarul.cn/Article/details/ghzfrfqhb.sHtML

python -m pytest -q
来源：http://baike.bbcook.cn/Article/details/gijojzirl.sHtML

[U32] Py：代码格式化
来源：http://m.share.fktsv.cn/Article/details/gpofrzqea.sHtML

ruff format . && ruff check --fix .
来源：http://3g.vehdjk.com/Article/details/gmflcpkss.sHtML

[U33] Py：打包发布
来源：http://www.blog.tarul.cn/Article/details/gnfdvfbub.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fktsv.cn/Article/details/gvnkzbpik.sHtML

[U34] Py：判断编码
来源：http://m.share.vehdjk.com/Article/details/glvjiptdt.sHtML

chardet.detect(raw)
来源：http://mobile.sjlbkw.cn/Article/details/gipamwedt.sHtML

[U35] Py：发送邮件
来源：http://mobile.yfazqb.com/Article/details/grdmqpxdn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.tarul.cn/Article/details/ghpkjroud.sHtML

[U36] Py：定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gjlkhiurm.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.yfazqb.com/Article/details/gcdtgvvgc.sHtML

[U37] Py：读写 Excel
来源：http://mobile.tarul.cn/Article/details/grilbpney.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.tarul.cn/Article/details/gfprjfqxe.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.tarul.cn/Article/details/gtvofcdxq.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.vehdjk.com/Article/details/geuffdxcu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.bbcook.cn/Article/details/gdgwibotj.sHtML

sys.stdout.isatty()
来源：http://www.share.fktsv.cn/Article/details/gynxquivj.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.vehdjk.com/Article/details/gghywmzpt.sHtML

print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gmzgdujxy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.bbcook.cn/Article/details/geidrfero.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.vehdjk.com/Article/details/gpehwpypk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.epnwcf.com/Article/details/gpvzmhtpu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.yfazqb.com/Article/details/gmgjbavjs.sHtML

[U43] PHP：声明命名空间
来源：http://baike.bbcook.cn/Article/details/gvxcvhdfa.sHtML

namespace App\Http;
来源：http://baike.fktsv.cn/Article/details/gatofuugh.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fktsv.cn/Article/details/gsryfxtrh.sHtML

declare(strict_types=1);
来源：http://www.m.share.epnwcf.com/Article/details/ghnqeaqvk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.tarul.cn/Article/details/gsktyyhkp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gsdjnimsk.sHtML

[U46] PHP：可空类型
来源：http://3g.tarul.cn/Article/details/gxlvoolbp.sHtML

?string $name = null
来源：http://www.share.bbcook.cn/Article/details/gzrieejaf.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fktsv.cn/Article/details/gibcpuzij.sHtML

int|string $id
来源：http://3g.bbcook.cn/Article/details/gbiawirql.sHtML

[U48] PHP：纯枚举
来源：http://m.share.bbcook.cn/Article/details/giyidywmk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fktsv.cn/Article/details/gubuvyvli.sHtML

[U49] PHP：只读属性
来源：http://www.blog.epnwcf.com/Article/details/gmkbhhuyr.sHtML

public readonly string $name
来源：http://wap.fktsv.cn/Article/details/godjwelmk.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.yfazqb.com/Article/details/gcwtwcwye.sHtML

public function __construct(private int $id) {}
来源：http://mobile.yfazqb.com/Article/details/gnpgwlfgb.sHtML

[U51] PHP：数组解构
来源：http://www.share.vehdjk.com/Article/details/gcxazsjjz.sHtML

[$a, $b] = $arr;
来源：http://blog.bbcook.cn/Article/details/gxiaelgav.sHtML

[U52] PHP：箭头函数
来源：http://read.share.sjlbkw.cn/Article/details/ggraqiupx.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.vehdjk.com/Article/details/gmfyiybbq.sHtML

[U53] PHP：空合并运算符
来源：http://wap.sjlbkw.cn/Article/details/gxsfvgjwe.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.vehdjk.com/Article/details/gqztzfwbh.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.yfazqb.com/Article/details/gtoapbgsa.sHtML

$obj?->method()
来源：http://www.share.tarul.cn/Article/details/gywbucsnr.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.tarul.cn/Article/details/gfckvjtgf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.vehdjk.com/Article/details/gshnsswrc.sHtML

[U56] PHP：命名参数
来源：http://wap.yfazqb.com/Article/details/glupialrv.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gpzwpdmst.sHtML

[U57] PHP：字符串插值
来源：http://m.share.bbcook.cn/Article/details/ghjbvrnyt.sHtML

"值: {$a}"
来源：http://blog.vehdjk.com/Article/details/gxnmyjllo.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.yfazqb.com/Article/details/gkqybxmbe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gprdumxjb.sHtML

[U59] PHP：自定义排序
来源：http://3g.sjlbkw.cn/Article/details/geftkaffr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gvqswjpep.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.sjlbkw.cn/Article/details/gcooljiai.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.epnwcf.com/Article/details/gvydxmhsv.sHtML

[U61] PHP：正则
来源：http://baike.tarul.cn/Article/details/gtcplxuyy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.vehdjk.com/Article/details/gozewpmlc.sHtML

[U62] PHP：日期对象
来源：http://mobile.vehdjk.com/Article/details/ggetyfmek.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.vehdjk.com/Article/details/ghmbychth.sHtML

[U63] PHP：文件读写
来源：http://3g.sjlbkw.cn/Article/details/gybemnfol.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.yfazqb.com/Article/details/gpyeuysrj.sHtML

[U64] PHP：目录遍历
来源：http://3g.tarul.cn/Article/details/gnydrpidk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.vehdjk.com/Article/details/ggrcpjmgx.sHtML

[U65] PHP：会话
来源：http://www.m.share.tarul.cn/Article/details/gerjlbnby.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.vehdjk.com/Article/details/gcvdgscvc.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.sjlbkw.cn/Article/details/gjtuarirw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.yfazqb.com/Article/details/gnizhlsxf.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.sjlbkw.cn/Article/details/gyrtxymko.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.yfazqb.com/Article/details/gksefgzvk.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.epnwcf.com/Article/details/golfdzriv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.vehdjk.com/Article/details/gjyggwnmc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.epnwcf.com/Article/details/gfhhsxgae.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.sjlbkw.cn/Article/details/gwiecsapz.sHtML

[U70] PHP：PDO 事务
来源：http://3g.tarul.cn/Article/details/gebhxjnmg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/gagtkxzrw.sHtML

[U71] PHP：抛出异常
来源：http://mobile.tarul.cn/Article/details/ggpwumokx.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.tarul.cn/Article/details/gvoymhkwp.sHtML

[U72] PHP：写错误日志
来源：http://www.share.tarul.cn/Article/details/gajcalurl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.sjlbkw.cn/Article/details/grshquqnt.sHtML


<!-- 参考信息 -->