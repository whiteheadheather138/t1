代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://read.share.tarul.cn/Article/details/gooemlwme.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfidlxyr.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gearnrcif.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfefeqsxq.sHtML

while (std::getline(in, line)) { }
来源：http://wap.vehdjk.com/Article/details/gbpzbpfin.sHtML

[S49] C++：写文件
来源：http://wap.sjlbkw.cn/Article/details/gdhiougox.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/gafjtqvim.sHtML

[S50] C++：格式化数字
来源：http://www.blog.epnwcf.com/Article/details/gxyfdpasn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/gndnblhei.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/gszziidlu.sHtML

static_cast<double>(a) / b
来源：http://read.share.bbcook.cn/Article/details/gtmadjmor.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.bbcook.cn/Article/details/gnxbabhla.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/gcqxxbfeh.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/gnclcsyxb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.sjlbkw.cn/Article/details/gosksqtad.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/gbollnklq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.bbcook.cn/Article/details/ghsmomkjn.sHtML

[S55] C++：结构化绑定
来源：http://read.share.epnwcf.com/Article/details/gdggsfyfl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.vehdjk.com/Article/details/gxdigyest.sHtML

[S56] C++：optional
来源：http://www.share.sjlbkw.cn/Article/details/gyubozvli.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.bbcook.cn/Article/details/gmmnyzlzm.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/gnlexebhe.sHtML

constexpr int N = 10;
来源：http://mobile.fktsv.cn/Article/details/gafkhudrx.sHtML

[S58] C++：命名空间
来源：http://mobile.yfazqb.com/Article/details/gojheqhph.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.yfazqb.com/Article/details/gwygtzvrw.sHtML

[S59] C++：静态断言
来源：http://www.share.vehdjk.com/Article/details/guxsxhvir.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.sjlbkw.cn/Article/details/gzphxwgex.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/gosktflym.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gsompgwre.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gckjnqvox.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gxvbqcdli.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdfineaus.sHtML

[T01] Kotlin：Hello World
来源：http://baike.epnwcf.com/Article/details/gpnbxqwlc.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gtqhyucod.sHtML

[T02] Kotlin：变量
来源：http://www.blog.tarul.cn/Article/details/gzxrjtcex.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.epnwcf.com/Article/details/gkomdyjvn.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.vehdjk.com/Article/details/gonqljnzz.sHtML

"值: $b"
来源：http://blog.yfazqb.com/Article/details/giuqejdob.sHtML

[T04] Kotlin：空安全
来源：http://m.share.sjlbkw.cn/Article/details/gjkwtnlin.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/gnktdxtii.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.vehdjk.com/Article/details/guswsyyyr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.vehdjk.com/Article/details/gwfqobpzn.sHtML

[T06] Kotlin：集合映射
来源：http://3g.yfazqb.com/Article/details/gpiuxyofg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.bbcook.cn/Article/details/glnjgavoy.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.tarul.cn/Article/details/gayoyvvdb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.epnwcf.com/Article/details/gxsgrfjia.sHtML

[T08] Kotlin：数据类
来源：http://www.share.bbcook.cn/Article/details/gyuqfqzpl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gackjxstk.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/gsndfducy.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.tarul.cn/Article/details/gvlkllilh.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.bbcook.cn/Article/details/grpnhlbrd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.vehdjk.com/Article/details/gcwnmnpsz.sHtML

[T11] Kotlin：协程
来源：http://3g.fktsv.cn/Article/details/giefntgtz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.yfazqb.com/Article/details/gtlfnmfgn.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/gtmtnturd.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gmmghqorg.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.yfazqb.com/Article/details/grwzcwjwe.sHtML

val m = mapOf("a" to 1)
来源：http://baike.epnwcf.com/Article/details/gqgxktrzn.sHtML

[T14] Kotlin：循环
来源：http://blog.fktsv.cn/Article/details/gyknpwzfp.sHtML

for (i in 1..10) println(i)
来源：http://mobile.tarul.cn/Article/details/gzfscscpb.sHtML

[T15] Kotlin：接口
来源：http://baike.sjlbkw.cn/Article/details/gskkblzrk.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fktsv.cn/Article/details/gxhkmpzgp.sHtML

[T16] Swift：Hello World
来源：http://blog.bbcook.cn/Article/details/gslahwxzk.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/gvjfvayry.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.epnwcf.com/Article/details/gmvyrwlif.sHtML

var a = 1;  let b = 2
来源：http://3g.yfazqb.com/Article/details/gjspjwkbr.sHtML

[T18] Swift：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gvoymdndg.sHtML

"值: \(b)"
来源：http://mobile.yfazqb.com/Article/details/gerqqshih.sHtML

[T19] Swift：可选绑定
来源：http://m.share.tarul.cn/Article/details/guogshyct.sHtML

if let n = opt { print(n) }
来源：http://baike.fktsv.cn/Article/details/guazwljly.sHtML

[T20] Swift：数组操作
来源：http://read.share.vehdjk.com/Article/details/gxoxmeoyi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/gqmnhzoeb.sHtML

[T21] Swift：遍历
来源：http://mobile.epnwcf.com/Article/details/gqqfxenjm.sHtML

for x in a { print(x) }
来源：http://3g.sjlbkw.cn/Article/details/gmootoace.sHtML

[T22] Swift：字典
来源：http://www.share.vehdjk.com/Article/details/gvjqmivyi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.tarul.cn/Article/details/ghmyuzhdc.sHtML

[T23] Swift：函数
来源：http://wap.fktsv.cn/Article/details/glchqybeq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fktsv.cn/Article/details/gbnuqxjrz.sHtML

[T24] Swift：闭包
来源：http://m.share.yfazqb.com/Article/details/ggsgnaepo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gwunijznw.sHtML

[T25] Swift：结构体
来源：http://read.share.vehdjk.com/Article/details/gioqjnrwy.sHtML

struct P { var x: Int }
来源：http://wap.tarul.cn/Article/details/gzvftjlzr.sHtML

[T26] Swift：类与重写
来源：http://read.share.sjlbkw.cn/Article/details/gtpesdboz.sHtML

class A: Base { override func f() {} }
来源：http://3g.sjlbkw.cn/Article/details/ghvobgcxg.sHtML

[T27] Swift：错误处理
来源：http://blog.yfazqb.com/Article/details/govhatlpv.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.yfazqb.com/Article/details/ghzefizkz.sHtML

[T28] Swift：枚举
来源：http://m.share.tarul.cn/Article/details/gpfsztdzj.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/gowmxlaqk.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.epnwcf.com/Article/details/gjxfutwzj.sHtML

guard let x = opt else { return }
来源：http://www.share.vehdjk.com/Article/details/gkbacjsbg.sHtML

[T30] Swift：协议
来源：http://www.m.share.fktsv.cn/Article/details/gvqjdmbjf.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fktsv.cn/Article/details/gooaltixz.sHtML

[T31] Lua：Hello World
来源：http://blog.fktsv.cn/Article/details/gjtddpeqf.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gbntxgaok.sHtML

[T32] Lua：局部变量
来源：http://wap.vehdjk.com/Article/details/gjptermnk.sHtML

local a = 1
来源：http://mobile.yfazqb.com/Article/details/ghtnpifix.sHtML

[T33] Lua：表（数组）
来源：http://m.share.sjlbkw.cn/Article/details/gpftrqxun.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.vehdjk.com/Article/details/gisxvvxfu.sHtML

[T34] Lua：遍历表
来源：http://www.share.fktsv.cn/Article/details/glbvqkoee.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.bbcook.cn/Article/details/gszdrstrb.sHtML

[T35] Lua：字典表
来源：http://www.share.yfazqb.com/Article/details/gyjmdsucg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.tarul.cn/Article/details/gymlaedwe.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/govupcujq.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.bbcook.cn/Article/details/geealxdzk.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.tarul.cn/Article/details/gvapbcawj.sHtML

"a" .. "b"
来源：http://www.blog.fktsv.cn/Article/details/gbxiykuwf.sHtML

[T38] Lua：条件
来源：http://wap.bbcook.cn/Article/details/gelgwrnht.sHtML

if x > 0 then print("正") end
来源：http://blog.sjlbkw.cn/Article/details/gtleoxelk.sHtML

[T39] Lua：模式匹配
来源：http://m.share.yfazqb.com/Article/details/goqdcjqdy.sHtML

string.find(s, "%d+")
来源：http://blog.epnwcf.com/Article/details/grdawcbyu.sHtML

[T40] Lua：元表
来源：http://www.share.yfazqb.com/Article/details/gudegewci.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fktsv.cn/Article/details/gwjpylrln.sHtML

[T41] Perl：Hello World
来源：http://3g.tarul.cn/Article/details/gkvjtuzua.sHtML

print "Hello\n";
来源：http://www.m.share.vehdjk.com/Article/details/gbjqordjp.sHtML

[T42] Perl：变量类型
来源：http://blog.sjlbkw.cn/Article/details/gobtpjgep.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.tarul.cn/Article/details/ggdhhzoqt.sHtML

[T43] Perl：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gnkccrezy.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/gozpymdqg.sHtML

[T44] Perl：条件
来源：http://3g.vehdjk.com/Article/details/gzltbhyrx.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.bbcook.cn/Article/details/glrtxuwoy.sHtML

[T45] Perl：数组遍历
来源：http://wap.bbcook.cn/Article/details/gfxgwjefc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.tarul.cn/Article/details/gaaeavovs.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fktsv.cn/Article/details/gykaxtirz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.bbcook.cn/Article/details/gqlheacjc.sHtML

[T47] Perl：正则捕获
来源：http://blog.bbcook.cn/Article/details/gajrjmlcm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.epnwcf.com/Article/details/gvcllvlcw.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gusqxprnn.sHtML

$s =~ s/old/new/g;
来源：http://wap.bbcook.cn/Article/details/gqcnlkglo.sHtML

[T49] Perl：函数
来源：http://www.share.epnwcf.com/Article/details/gkxifmyal.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gfimxxapf.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.tarul.cn/Article/details/ghzisgdqz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.epnwcf.com/Article/details/gcmuahcbs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.yfazqb.com/Article/details/gzbfqffbf.sHtML

[T51] Scala：Hello World
来源：http://mobile.tarul.cn/Article/details/gzxbhsnum.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/ggbbzcumi.sHtML

[T52] Scala：变量
来源：http://www.blog.vehdjk.com/Article/details/grlzojzks.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fktsv.cn/Article/details/ghrcfodtq.sHtML

[T53] Scala：字符串插值
来源：http://3g.yfazqb.com/Article/details/gqnzwqora.sHtML

s"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gdspcrgwm.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fktsv.cn/Article/details/gsakoopmu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.sjlbkw.cn/Article/details/gergtbgtg.sHtML

[T55] Scala：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gctkirqaq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.epnwcf.com/Article/details/gfxqxnnmq.sHtML

[T56] Scala：样例类
来源：http://www.share.epnwcf.com/Article/details/gwlvgqxcl.sHtML

case class User(name: String, age: Int)
来源：http://baike.yfazqb.com/Article/details/gbseajvpv.sHtML

[T57] Scala：模式匹配
来源：http://wap.vehdjk.com/Article/details/gpawpyzxu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.epnwcf.com/Article/details/gjtrcgnqi.sHtML

[T58] Scala：函数定义
来源：http://baike.tarul.cn/Article/details/gevqssthg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.tarul.cn/Article/details/gkueqfqmu.sHtML

[T59] Scala：循环
来源：http://wap.sjlbkw.cn/Article/details/gkvrwhuuf.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gqqgdmpuv.sHtML

[T60] Scala：折叠
来源：http://blog.epnwcf.com/Article/details/gunstusmj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.yfazqb.com/Article/details/gsutdxkfz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gnzvxijex.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/glvaymzog.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxyefndgi.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.tarul.cn/Article/details/griiczsmo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.sjlbkw.cn/Article/details/gzlnboico.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.tarul.cn/Article/details/gmfgvbwrn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fktsv.cn/Article/details/guerpvutw.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.tarul.cn/Article/details/gcwwyewcx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.tarul.cn/Article/details/gsyakcdzj.sHtML

[U04] Py：变量调试打印
来源：http://mobile.tarul.cn/Article/details/giaupluwq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.sjlbkw.cn/Article/details/gllsewliw.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.epnwcf.com/Article/details/gqqfzkduy.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gtqrgdcdn.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.vehdjk.com/Article/details/gfzzriolw.sHtML

{**a, **b}
来源：http://3g.tarul.cn/Article/details/gojrrvxcl.sHtML

[U07] Py：反转字典键值
来源：http://3g.bbcook.cn/Article/details/gnnkdoqpx.sHtML

{v: k for k, v in d.items()}
来源：http://wap.bbcook.cn/Article/details/gsemfzhzi.sHtML

[U08] Py：展平二维列表
来源：http://mobile.yfazqb.com/Article/details/gshrutgqt.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.tarul.cn/Article/details/gkeqtnizi.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.vehdjk.com/Article/details/gjtpoayuo.sHtML

max(d, key=d.get)
来源：http://read.share.tarul.cn/Article/details/gznnvbfta.sHtML

[U10] Py：按值排序字典
来源：http://baike.vehdjk.com/Article/details/ggqrhhbdc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.epnwcf.com/Article/details/gzfkkqzio.sHtML

[U11] Py：生成器表达式
来源：http://mobile.sjlbkw.cn/Article/details/gggvccepp.sHtML

(x * 2 for x in arr)
来源：http://3g.sjlbkw.cn/Article/details/gjoxjzlef.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.yfazqb.com/Article/details/ggcqysisj.sHtML

Counter(arr).most_common(3)
来源：http://blog.sjlbkw.cn/Article/details/gwzndojkr.sHtML

[U13] Py：固定长度队列
来源：http://m.share.yfazqb.com/Article/details/gruvhjipr.sHtML

deque(maxlen=10)
来源：http://wap.sjlbkw.cn/Article/details/gbwgbakza.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.vehdjk.com/Article/details/gcxvdamla.sHtML

defaultdict(list)
来源：http://baike.fktsv.cn/Article/details/gslqiturz.sHtML

[U15] Py：高精度计时
来源：http://www.share.fktsv.cn/Article/details/gmfdnoymk.sHtML

t = time.perf_counter()
来源：http://m.share.epnwcf.com/Article/details/gmkdyrtsi.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.epnwcf.com/Article/details/gjvbawbyq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fktsv.cn/Article/details/gvtwahykh.sHtML

[U17] Py：初始化日志
来源：http://mobile.fktsv.cn/Article/details/gokkcughx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.vehdjk.com/Article/details/gkvgupigs.sHtML

[U18] Py：预编译正则
来源：http://www.share.tarul.cn/Article/details/gsxulusrn.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.epnwcf.com/Article/details/gaqigltqv.sHtML

[U19] Py：正则替换带回调
来源：http://3g.sjlbkw.cn/Article/details/gflgrrrnf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.bbcook.cn/Article/details/gkhpmkrgy.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.vehdjk.com/Article/details/gkonohioz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.tarul.cn/Article/details/gvecsbzen.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fktsv.cn/Article/details/gjfxoasxd.sHtML

@contextlib.contextmanager
来源：http://read.share.yfazqb.com/Article/details/gablwquwd.sHtML

[U22] Py：矩阵转置
来源：http://www.share.tarul.cn/Article/details/gyixujmmj.sHtML

list(zip(*m))
来源：http://wap.tarul.cn/Article/details/gporxczbv.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.vehdjk.com/Article/details/gwurdhumw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.sjlbkw.cn/Article/details/gcksrylxw.sHtML

[U24] Py：路径操作
来源：http://baike.sjlbkw.cn/Article/details/gqaqbavkh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gqrwdfqwx.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.tarul.cn/Article/details/gickqbhry.sHtML

csv.DictReader(f)
来源：http://baike.bbcook.cn/Article/details/ghqntxnxd.sHtML

[U26] Py：并发下载
来源：http://mobile.tarul.cn/Article/details/gabemvlca.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.epnwcf.com/Article/details/gmcnauumd.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.sjlbkw.cn/Article/details/guerqblwt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.sjlbkw.cn/Article/details/gtgcfaljd.sHtML

[U28] Py：类型别名
来源：http://blog.fktsv.cn/Article/details/gwxhicpyu.sHtML

UserId = int
来源：http://m.share.vehdjk.com/Article/details/gvwpfjizt.sHtML

[U29] Py：属性校验
来源：http://www.blog.sjlbkw.cn/Article/details/gsbncgzxh.sHtML

@property 与 @x.setter 配合
来源：http://3g.fktsv.cn/Article/details/gbjtwldcw.sHtML

[U30] Py：数据类
来源：http://baike.tarul.cn/Article/details/gvfgocxqc.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fktsv.cn/Article/details/gztzafkfa.sHtML

[U31] Py：单测
来源：http://www.share.vehdjk.com/Article/details/gqiacnryw.sHtML

python -m pytest -q
来源：http://www.m.share.sjlbkw.cn/Article/details/gsofnvstn.sHtML

[U32] Py：代码格式化
来源：http://wap.yfazqb.com/Article/details/gfavlruwd.sHtML

ruff format . && ruff check --fix .
来源：http://wap.yfazqb.com/Article/details/gsajretry.sHtML

[U33] Py：打包发布
来源：http://m.share.fktsv.cn/Article/details/guwtganwn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.tarul.cn/Article/details/gmbpcoudh.sHtML

[U34] Py：判断编码
来源：http://www.m.share.yfazqb.com/Article/details/guswdanff.sHtML

chardet.detect(raw)
来源：http://3g.vehdjk.com/Article/details/gsguhnzcs.sHtML

[U35] Py：发送邮件
来源：http://baike.epnwcf.com/Article/details/gqfnoyalv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.yfazqb.com/Article/details/gutgtmzql.sHtML

[U36] Py：定时任务
来源：http://www.share.tarul.cn/Article/details/gvfaduzlo.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.bbcook.cn/Article/details/goiesgqqp.sHtML

[U37] Py：读写 Excel
来源：http://read.share.bbcook.cn/Article/details/gyvulsqsk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.vehdjk.com/Article/details/gyccdaloe.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.sjlbkw.cn/Article/details/gsmxpvpeu.sHtML

Path(__file__).resolve().parent
来源：http://www.share.tarul.cn/Article/details/gzwwtarsn.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.tarul.cn/Article/details/gdbyjfwts.sHtML

sys.stdout.isatty()
来源：http://wap.epnwcf.com/Article/details/gjmhaaehe.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.vehdjk.com/Article/details/geowekmwx.sHtML

print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gbudpkudr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.bbcook.cn/Article/details/gtlwalkzu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/gsoteyewn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.epnwcf.com/Article/details/ghiczmgwv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.vehdjk.com/Article/details/gyqbdivui.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fktsv.cn/Article/details/gedlijwkb.sHtML

namespace App\Http;
来源：http://baike.tarul.cn/Article/details/gnixzedbo.sHtML

[U44] PHP：开启严格类型
来源：http://3g.epnwcf.com/Article/details/gkdyjmorb.sHtML

declare(strict_types=1);
来源：http://wap.yfazqb.com/Article/details/gacjplleq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.yfazqb.com/Article/details/gaurnbmxc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gpklbqkym.sHtML

[U46] PHP：可空类型
来源：http://www.blog.yfazqb.com/Article/details/gozdnhhsc.sHtML

?string $name = null
来源：http://3g.tarul.cn/Article/details/gdrhtcmal.sHtML

[U47] PHP：联合类型
来源：http://wap.fktsv.cn/Article/details/ggggkaule.sHtML

int|string $id
来源：http://www.m.share.bbcook.cn/Article/details/gjhlpoklv.sHtML

[U48] PHP：纯枚举
来源：http://mobile.yfazqb.com/Article/details/goratlwum.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fktsv.cn/Article/details/gmdataljj.sHtML

[U49] PHP：只读属性
来源：http://m.share.sjlbkw.cn/Article/details/gsagfevca.sHtML

public readonly string $name
来源：http://m.share.vehdjk.com/Article/details/ggokukcjq.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.vehdjk.com/Article/details/gszxaesxb.sHtML

public function __construct(private int $id) {}
来源：http://blog.vehdjk.com/Article/details/gbltvrvbo.sHtML

[U51] PHP：数组解构
来源：http://blog.epnwcf.com/Article/details/grvdqkrlz.sHtML

[$a, $b] = $arr;
来源：http://3g.yfazqb.com/Article/details/gqzzefhad.sHtML

[U52] PHP：箭头函数
来源：http://3g.tarul.cn/Article/details/gojltvgow.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.tarul.cn/Article/details/gqqtecgcp.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.tarul.cn/Article/details/grkjopvsf.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.epnwcf.com/Article/details/gpcvxmmzd.sHtML

[U54] PHP：空安全调用
来源：http://3g.yfazqb.com/Article/details/gdkogcfvu.sHtML

$obj?->method()
来源：http://3g.yfazqb.com/Article/details/gdhwbzlgr.sHtML

[U55] PHP：match 表达式
来源：http://m.share.vehdjk.com/Article/details/gfzlnphlj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/gmtdacsew.sHtML

[U56] PHP：命名参数
来源：http://3g.sjlbkw.cn/Article/details/gypplndny.sHtML

f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/geibogxgf.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuxnxjjp.sHtML

"值: {$a}"
来源：http://www.m.share.epnwcf.com/Article/details/gnxpvrilu.sHtML

[U58] PHP：数组三件套
来源：http://baike.epnwcf.com/Article/details/gqbxwdbmq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.bbcook.cn/Article/details/gtexrssvz.sHtML

[U59] PHP：自定义排序
来源：http://www.share.vehdjk.com/Article/details/gdvtbistq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gyfijyfyw.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.sjlbkw.cn/Article/details/gdeqwgnin.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.tarul.cn/Article/details/gyznosyqj.sHtML

[U61] PHP：正则
来源：http://wap.epnwcf.com/Article/details/gpiztkchd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gckqqijjw.sHtML

[U62] PHP：日期对象
来源：http://www.blog.yfazqb.com/Article/details/gpsnjcpop.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.tarul.cn/Article/details/gxddbrliz.sHtML

[U63] PHP：文件读写
来源：http://wap.fktsv.cn/Article/details/goqhiauyf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.epnwcf.com/Article/details/gmfqqbsts.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gehxcyspl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.yfazqb.com/Article/details/glusrabzc.sHtML

[U65] PHP：会话
来源：http://baike.bbcook.cn/Article/details/gcbovgnpc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gekbygmlt.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fktsv.cn/Article/details/gnzvnjcop.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwkkpqqo.sHtML

[U67] PHP：处理文件上传
来源：http://baike.epnwcf.com/Article/details/gqpmvysxj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.bbcook.cn/Article/details/gxcgpcfty.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fktsv.cn/Article/details/gpnpfturo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.sjlbkw.cn/Article/details/gysbbpmdp.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fktsv.cn/Article/details/gtiahyquf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.sjlbkw.cn/Article/details/giuxfqwvg.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.bbcook.cn/Article/details/gvkatwefr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.tarul.cn/Article/details/gejcrdtvn.sHtML

[U71] PHP：抛出异常
来源：http://m.share.epnwcf.com/Article/details/gsgohggyu.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.epnwcf.com/Article/details/gbonsgvue.sHtML

[U72] PHP：写错误日志
来源：http://www.share.bbcook.cn/Article/details/gtyijzeaa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.tarul.cn/Article/details/ghrrpvork.sHtML


<!-- 参考信息 -->