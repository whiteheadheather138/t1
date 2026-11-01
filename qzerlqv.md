代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.m.share.bbcook.cn/Article/details/glqokbwoo.sHtML

[S53] C++：移动语义
来源：http://m.share.vehdjk.com/Article/details/gxtazdcrd.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/gewokgqje.sHtML

[S54] C++：异常处理
来源：http://3g.yfazqb.com/Article/details/gpovegksy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fktsv.cn/Article/details/giuqgmpsf.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvlcpdwq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.tarul.cn/Article/details/ghcybjddb.sHtML

[S56] C++：optional
来源：http://read.share.fktsv.cn/Article/details/gassreavn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.vehdjk.com/Article/details/ghnybcgmu.sHtML

[S57] C++：编译期常量
来源：http://read.share.tarul.cn/Article/details/gjqngmijc.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/gvhhtbwwt.sHtML

[S58] C++：命名空间
来源：http://www.m.share.bbcook.cn/Article/details/glflznqvs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.yfazqb.com/Article/details/gxiciapub.sHtML

[S59] C++：静态断言
来源：http://blog.yfazqb.com/Article/details/gubupgcsy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.sjlbkw.cn/Article/details/glyyerhlr.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.yfazqb.com/Article/details/gfbgbjhhz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.vehdjk.com/Article/details/gmlvkxmlf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gpwoxqcxd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.bbcook.cn/Article/details/gldilchvk.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gycfezmrt.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gcqmrdbee.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/gspjeoieo.sHtML

[T02] Kotlin：变量
来源：http://blog.sjlbkw.cn/Article/details/ggjxfhxjq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.sjlbkw.cn/Article/details/gzntoazuf.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.epnwcf.com/Article/details/gobquxokz.sHtML

"值: $b"
来源：http://read.share.epnwcf.com/Article/details/gziqpgnmn.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/gxbelhnqr.sHtML

val n: String? = null;  n?.length
来源：http://3g.epnwcf.com/Article/details/gjmfvnnlc.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.vehdjk.com/Article/details/gyifnltfh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.bbcook.cn/Article/details/gnxbqoctf.sHtML

[T06] Kotlin：集合映射
来源：http://3g.bbcook.cn/Article/details/gzcgipmkw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.epnwcf.com/Article/details/ghmojngjh.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/gbifmpyzb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/gnxyqyoda.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/grvquwqhn.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.sjlbkw.cn/Article/details/gpallmrqz.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.vehdjk.com/Article/details/gqzmetqfy.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.tarul.cn/Article/details/glufiwbke.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.epnwcf.com/Article/details/gmofjkdka.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.vehdjk.com/Article/details/gycaayjke.sHtML

[T11] Kotlin：协程
来源：http://baike.epnwcf.com/Article/details/gucyxepnq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.yfazqb.com/Article/details/gapbpbcsx.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.yfazqb.com/Article/details/gkrxqdecw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/ghyiajvid.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.epnwcf.com/Article/details/gkwklbcmj.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.yfazqb.com/Article/details/gskfjfcur.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/gxjpbjhmz.sHtML

for (i in 1..10) println(i)
来源：http://mobile.tarul.cn/Article/details/gshcfifny.sHtML

[T15] Kotlin：接口
来源：http://m.share.epnwcf.com/Article/details/gxrxajuhp.sHtML

interface Shape { fun area(): Double }
来源：http://baike.bbcook.cn/Article/details/goukvbbuj.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gcwtfhzce.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/gxetratfi.sHtML

[T17] Swift：变量与常量
来源：http://m.share.tarul.cn/Article/details/gusgttqdw.sHtML

var a = 1;  let b = 2
来源：http://3g.vehdjk.com/Article/details/ghxaazusk.sHtML

[T18] Swift：字符串插值
来源：http://mobile.vehdjk.com/Article/details/glwzcpkwi.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gpwxuqgdg.sHtML

[T19] Swift：可选绑定
来源：http://m.share.bbcook.cn/Article/details/gsppjgyee.sHtML

if let n = opt { print(n) }
来源：http://blog.tarul.cn/Article/details/gtvbhxjtc.sHtML

[T20] Swift：数组操作
来源：http://baike.yfazqb.com/Article/details/guozgdtql.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.vehdjk.com/Article/details/gmcdjcinr.sHtML

[T21] Swift：遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gbofrnzvz.sHtML

for x in a { print(x) }
来源：http://3g.fktsv.cn/Article/details/gkcvkywcw.sHtML

[T22] Swift：字典
来源：http://m.share.epnwcf.com/Article/details/gbdmdcpgd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.yfazqb.com/Article/details/gyznvumhp.sHtML

[T23] Swift：函数
来源：http://mobile.bbcook.cn/Article/details/gpdrzsxxc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gfiygzysq.sHtML

[T24] Swift：闭包
来源：http://blog.epnwcf.com/Article/details/gxuuxwwzx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.tarul.cn/Article/details/ghezldnwt.sHtML

[T25] Swift：结构体
来源：http://www.blog.yfazqb.com/Article/details/gmhadtcyc.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/ggawmwhph.sHtML

[T26] Swift：类与重写
来源：http://www.share.fktsv.cn/Article/details/glbzhcjqp.sHtML

class A: Base { override func f() {} }
来源：http://baike.sjlbkw.cn/Article/details/gozbgnaac.sHtML

[T27] Swift：错误处理
来源：http://baike.bbcook.cn/Article/details/gfqqlbzab.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fktsv.cn/Article/details/gkxgmutuk.sHtML

[T28] Swift：枚举
来源：http://blog.yfazqb.com/Article/details/gxsfiwbac.sHtML

enum Color { case red, green }
来源：http://wap.fktsv.cn/Article/details/gxsuonsou.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/gngjjdcgt.sHtML

guard let x = opt else { return }
来源：http://read.share.vehdjk.com/Article/details/gyiwfcutx.sHtML

[T30] Swift：协议
来源：http://wap.vehdjk.com/Article/details/gechrlwus.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fktsv.cn/Article/details/gdsdniqga.sHtML

[T31] Lua：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gyyvriwlv.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/grbsdygkn.sHtML

[T32] Lua：局部变量
来源：http://wap.epnwcf.com/Article/details/gdpiafslj.sHtML

local a = 1
来源：http://www.blog.tarul.cn/Article/details/gotwiuxgw.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.vehdjk.com/Article/details/gkqognkoj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.tarul.cn/Article/details/gbhcafnau.sHtML

[T34] Lua：遍历表
来源：http://www.share.vehdjk.com/Article/details/gvenbnvyq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.yfazqb.com/Article/details/gbfsjbwru.sHtML

[T35] Lua：字典表
来源：http://m.share.yfazqb.com/Article/details/gbszybdbp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.bbcook.cn/Article/details/gsfljodbg.sHtML

[T36] Lua：函数
来源：http://www.blog.yfazqb.com/Article/details/ghoqgpqlf.sHtML

function add(a, b) return a + b end
来源：http://www.share.epnwcf.com/Article/details/gajfkwxxd.sHtML

[T37] Lua：字符串拼接
来源：http://wap.vehdjk.com/Article/details/gnftfcbbp.sHtML

"a" .. "b"
来源：http://www.blog.vehdjk.com/Article/details/gzjztqnge.sHtML

[T38] Lua：条件
来源：http://mobile.yfazqb.com/Article/details/gxlfkxubh.sHtML

if x > 0 then print("正") end
来源：http://www.share.epnwcf.com/Article/details/gsvpvznbl.sHtML

[T39] Lua：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/gputckblo.sHtML

string.find(s, "%d+")
来源：http://baike.epnwcf.com/Article/details/guyeflzei.sHtML

[T40] Lua：元表
来源：http://www.blog.tarul.cn/Article/details/gnbnxvtri.sHtML

setmetatable({}, { __index = base })
来源：http://wap.yfazqb.com/Article/details/gcywgbyge.sHtML

[T41] Perl：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gwpafzqby.sHtML

print "Hello\n";
来源：http://www.share.sjlbkw.cn/Article/details/gdfxlvdaj.sHtML

[T42] Perl：变量类型
来源：http://3g.yfazqb.com/Article/details/gvpwujmrf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.bbcook.cn/Article/details/gtpqepbsb.sHtML

[T43] Perl：字符串插值
来源：http://www.share.tarul.cn/Article/details/gkxlqlaer.sHtML

"值: $a"
来源：http://3g.fktsv.cn/Article/details/ggfdhdoaf.sHtML

[T44] Perl：条件
来源：http://www.share.vehdjk.com/Article/details/gnymmmiqy.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.tarul.cn/Article/details/gxitjdcjq.sHtML

[T45] Perl：数组遍历
来源：http://blog.sjlbkw.cn/Article/details/ggpofiwix.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.yfazqb.com/Article/details/ghfqiskhr.sHtML

[T46] Perl：哈希操作
来源：http://3g.bbcook.cn/Article/details/grtvwtija.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grhhjxuct.sHtML

[T47] Perl：正则捕获
来源：http://mobile.sjlbkw.cn/Article/details/gnltoqtqx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.tarul.cn/Article/details/guoynqsqc.sHtML

[T48] Perl：正则替换
来源：http://m.share.epnwcf.com/Article/details/gknywcxti.sHtML

$s =~ s/old/new/g;
来源：http://read.share.sjlbkw.cn/Article/details/gimunjjbj.sHtML

[T49] Perl：函数
来源：http://read.share.fktsv.cn/Article/details/gseveotmc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gbkmknuhb.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/geldjpuns.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.yfazqb.com/Article/details/gwbaajmds.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.sjlbkw.cn/Article/details/gsfiskccn.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/grkdxeijs.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/ggcdnhgaa.sHtML

[T52] Scala：变量
来源：http://www.share.epnwcf.com/Article/details/gwdgnlfmz.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.tarul.cn/Article/details/gphfrqaxa.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gprlvvwgb.sHtML

s"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gcfvawtbq.sHtML

[T54] Scala：集合映射
来源：http://www.share.tarul.cn/Article/details/gretaapre.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.vehdjk.com/Article/details/gtbkihtne.sHtML

[T55] Scala：集合过滤
来源：http://3g.tarul.cn/Article/details/gbxghxztr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fktsv.cn/Article/details/gypfdqjdm.sHtML

[T56] Scala：样例类
来源：http://wap.tarul.cn/Article/details/gamrqhzjl.sHtML

case class User(name: String, age: Int)
来源：http://baike.vehdjk.com/Article/details/gkbmqvxbt.sHtML

[T57] Scala：模式匹配
来源：http://baike.yfazqb.com/Article/details/ghyfggleg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.vehdjk.com/Article/details/gpacbhkrd.sHtML

[T58] Scala：函数定义
来源：http://www.blog.sjlbkw.cn/Article/details/gbuqggfoi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.bbcook.cn/Article/details/gjynsktds.sHtML

[T59] Scala：循环
来源：http://www.share.epnwcf.com/Article/details/gljhrhbxh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gunrhrmuk.sHtML

[T60] Scala：折叠
来源：http://www.share.vehdjk.com/Article/details/gciqgcbrd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.sjlbkw.cn/Article/details/gmxpzlakz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmngnxeqp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/gebpobxbc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gfvwzhcva.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.epnwcf.com/Article/details/gwrzyctkh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.tarul.cn/Article/details/gxttbqfpa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.vehdjk.com/Article/details/gfibppszg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fktsv.cn/Article/details/gkpoyaxca.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.bbcook.cn/Article/details/gljmkkgiy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.sjlbkw.cn/Article/details/gcdxooekf.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fktsv.cn/Article/details/gkuhmdssi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.vehdjk.com/Article/details/gfumhgshy.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.yfazqb.com/Article/details/gqdmvmlqu.sHtML

list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gsenmltbw.sHtML

[U06] Py：合并两个字典
来源：http://mobile.bbcook.cn/Article/details/gypheystu.sHtML

{**a, **b}
来源：http://baike.fktsv.cn/Article/details/gjzivywnn.sHtML

[U07] Py：反转字典键值
来源：http://www.share.sjlbkw.cn/Article/details/gaozkjadh.sHtML

{v: k for k, v in d.items()}
来源：http://blog.yfazqb.com/Article/details/gvilythgm.sHtML

[U08] Py：展平二维列表
来源：http://blog.fktsv.cn/Article/details/gsbmifxsp.sHtML

[y for x in nested for y in x]
来源：http://www.blog.vehdjk.com/Article/details/guoqxzdqz.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.bbcook.cn/Article/details/gojinvwld.sHtML

max(d, key=d.get)
来源：http://baike.tarul.cn/Article/details/gzzqnsmhq.sHtML

[U10] Py：按值排序字典
来源：http://blog.vehdjk.com/Article/details/gavwbkykt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.yfazqb.com/Article/details/gbrovddpv.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fktsv.cn/Article/details/gqtdjzjuh.sHtML

(x * 2 for x in arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gwbgqinrt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.bbcook.cn/Article/details/gumttwimo.sHtML

Counter(arr).most_common(3)
来源：http://wap.fktsv.cn/Article/details/gxcwjccyc.sHtML

[U13] Py：固定长度队列
来源：http://www.share.bbcook.cn/Article/details/ghvnkxyto.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/gqrbgcpwz.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/gejbjiylu.sHtML

defaultdict(list)
来源：http://www.share.yfazqb.com/Article/details/gkbnklyyp.sHtML

[U15] Py：高精度计时
来源：http://blog.epnwcf.com/Article/details/gxhbmkobm.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/gcvtmwvwx.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.bbcook.cn/Article/details/gamfohqzr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fktsv.cn/Article/details/gcijdnhsx.sHtML

[U17] Py：初始化日志
来源：http://read.share.bbcook.cn/Article/details/gmqauohhx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fktsv.cn/Article/details/gvbgdpwpw.sHtML

[U18] Py：预编译正则
来源：http://blog.sjlbkw.cn/Article/details/gbcnevvtt.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/gusnayksm.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.tarul.cn/Article/details/gjmwzwndd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.yfazqb.com/Article/details/gkkpzomdv.sHtML

[U20] Py：缓存函数结果
来源：http://3g.tarul.cn/Article/details/gxyqnbcpl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.epnwcf.com/Article/details/gnawaldij.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.tarul.cn/Article/details/guhzselih.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/ggzbkezej.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fktsv.cn/Article/details/guinxykcu.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/gyyxjsrow.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.epnwcf.com/Article/details/gjdwfzkkk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.vehdjk.com/Article/details/gfxzeghuo.sHtML

[U24] Py：路径操作
来源：http://www.blog.vehdjk.com/Article/details/gtahwwydz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/golgomeev.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.tarul.cn/Article/details/ggwmbcwpz.sHtML

csv.DictReader(f)
来源：http://m.share.epnwcf.com/Article/details/gaxtshsdd.sHtML

[U26] Py：并发下载
来源：http://3g.yfazqb.com/Article/details/gdqlybzlt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.vehdjk.com/Article/details/gyyxlwutm.sHtML

[U27] Py：异步 HTTP
来源：http://3g.yfazqb.com/Article/details/glcqqbfvq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.epnwcf.com/Article/details/gxxarvyqv.sHtML

[U28] Py：类型别名
来源：http://3g.fktsv.cn/Article/details/ghrgkpogg.sHtML

UserId = int
来源：http://www.share.tarul.cn/Article/details/gwcfqkxru.sHtML

[U29] Py：属性校验
来源：http://www.blog.sjlbkw.cn/Article/details/gfwjmosji.sHtML

@property 与 @x.setter 配合
来源：http://read.share.tarul.cn/Article/details/gvnjyqmbw.sHtML

[U30] Py：数据类
来源：http://read.share.bbcook.cn/Article/details/gkauclots.sHtML

@dataclass(slots=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbnhxwmq.sHtML

[U31] Py：单测
来源：http://www.blog.fktsv.cn/Article/details/grctrbrwz.sHtML

python -m pytest -q
来源：http://blog.yfazqb.com/Article/details/gqhewrvyr.sHtML

[U32] Py：代码格式化
来源：http://wap.tarul.cn/Article/details/gggcgjffq.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fktsv.cn/Article/details/gcjzjingq.sHtML

[U33] Py：打包发布
来源：http://m.share.sjlbkw.cn/Article/details/glcixdkbo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.yfazqb.com/Article/details/gwaieyowr.sHtML

[U34] Py：判断编码
来源：http://m.share.epnwcf.com/Article/details/gmzdukjrg.sHtML

chardet.detect(raw)
来源：http://blog.tarul.cn/Article/details/gvumnoefa.sHtML

[U35] Py：发送邮件
来源：http://www.share.vehdjk.com/Article/details/gkrrlnkeb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.tarul.cn/Article/details/gxzdknlgq.sHtML

[U36] Py：定时任务
来源：http://www.blog.yfazqb.com/Article/details/gaulavext.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.epnwcf.com/Article/details/goiymgeqa.sHtML

[U37] Py：读写 Excel
来源：http://m.share.sjlbkw.cn/Article/details/gawivhadh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.vehdjk.com/Article/details/gvompjaim.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.epnwcf.com/Article/details/ggpbvjkzb.sHtML

Path(__file__).resolve().parent
来源：http://mobile.yfazqb.com/Article/details/gxufigbzf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fktsv.cn/Article/details/gaybwfkvq.sHtML

sys.stdout.isatty()
来源：http://3g.sjlbkw.cn/Article/details/goumeidak.sHtML

[U40] Py：打印到标准错误
来源：http://wap.bbcook.cn/Article/details/gehjufhjm.sHtML

print("err", file=sys.stderr)
来源：http://baike.bbcook.cn/Article/details/gnmmbxrpi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.vehdjk.com/Article/details/guwbbkwkt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.tarul.cn/Article/details/gxvnyohew.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.tarul.cn/Article/details/gyzqcwxti.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.yfazqb.com/Article/details/gxwgexlwc.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.sjlbkw.cn/Article/details/gltpoysob.sHtML

namespace App\Http;
来源：http://www.share.yfazqb.com/Article/details/gnwywfgjx.sHtML

[U44] PHP：开启严格类型
来源：http://baike.sjlbkw.cn/Article/details/gylhnqifu.sHtML

declare(strict_types=1);
来源：http://www.share.epnwcf.com/Article/details/gtpdwague.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.tarul.cn/Article/details/gwxzbkbbd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gouztjbgk.sHtML

[U46] PHP：可空类型
来源：http://m.share.bbcook.cn/Article/details/gttyhlskv.sHtML

?string $name = null
来源：http://www.blog.tarul.cn/Article/details/gnelujwqx.sHtML

[U47] PHP：联合类型
来源：http://wap.sjlbkw.cn/Article/details/gtpmdfkun.sHtML

int|string $id
来源：http://wap.fktsv.cn/Article/details/gcegqrjjf.sHtML

[U48] PHP：纯枚举
来源：http://m.share.yfazqb.com/Article/details/gxdbzbtve.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.epnwcf.com/Article/details/gcqzqupym.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fktsv.cn/Article/details/gwsotftap.sHtML

public readonly string $name
来源：http://baike.epnwcf.com/Article/details/grmkyxmet.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.vehdjk.com/Article/details/gfuxbzozi.sHtML

public function __construct(private int $id) {}
来源：http://baike.tarul.cn/Article/details/grwcdmxct.sHtML

[U51] PHP：数组解构
来源：http://3g.tarul.cn/Article/details/gkhytrckj.sHtML

[$a, $b] = $arr;
来源：http://read.share.tarul.cn/Article/details/glbqdjfxw.sHtML

[U52] PHP：箭头函数
来源：http://www.share.bbcook.cn/Article/details/glkcdsxll.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.vehdjk.com/Article/details/gfazuesmy.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fktsv.cn/Article/details/gqckeacab.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.tarul.cn/Article/details/gzmjnaaja.sHtML

[U54] PHP：空安全调用
来源：http://blog.bbcook.cn/Article/details/gbwpotjjp.sHtML

$obj?->method()
来源：http://www.share.vehdjk.com/Article/details/gckrvtupm.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gwuukutxb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.tarul.cn/Article/details/gsjwzcouj.sHtML

[U56] PHP：命名参数
来源：http://wap.sjlbkw.cn/Article/details/gvrtprvma.sHtML

f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gwgdeenea.sHtML

[U57] PHP：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gldxwyfon.sHtML

"值: {$a}"
来源：http://m.share.tarul.cn/Article/details/ghspjvplk.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fktsv.cn/Article/details/gpzvckvhg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.bbcook.cn/Article/details/gypmnbsie.sHtML

[U59] PHP：自定义排序
来源：http://read.share.vehdjk.com/Article/details/gjscqddeo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/guwelfngz.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.epnwcf.com/Article/details/gvpffbxtg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.tarul.cn/Article/details/gknbclwja.sHtML

[U61] PHP：正则
来源：http://m.share.epnwcf.com/Article/details/gjnrpwqnm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/gmqrwcled.sHtML

[U62] PHP：日期对象
来源：http://www.share.sjlbkw.cn/Article/details/gvtaibcys.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.epnwcf.com/Article/details/gidraqskb.sHtML

[U63] PHP：文件读写
来源：http://www.share.bbcook.cn/Article/details/gjzpumiqh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.vehdjk.com/Article/details/gxqgsedhu.sHtML

[U64] PHP：目录遍历
来源：http://baike.tarul.cn/Article/details/gmhazkkpr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.vehdjk.com/Article/details/gznlgfblg.sHtML

[U65] PHP：会话
来源：http://wap.sjlbkw.cn/Article/details/gyuttiwiv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.tarul.cn/Article/details/gkmmsnoni.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.tarul.cn/Article/details/gxuvwmoha.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fktsv.cn/Article/details/gmumoesby.sHtML

[U67] PHP：处理文件上传
来源：http://baike.sjlbkw.cn/Article/details/gtimraivv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.vehdjk.com/Article/details/gzhgmhlhd.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fktsv.cn/Article/details/gdtkcixpp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.vehdjk.com/Article/details/gajivhdxc.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.tarul.cn/Article/details/gicdlbclu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.tarul.cn/Article/details/gynyuwtct.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.epnwcf.com/Article/details/guzlrcdrr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.vehdjk.com/Article/details/gbsfiawvs.sHtML

[U71] PHP：抛出异常
来源：http://www.share.yfazqb.com/Article/details/gnzvgvufu.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.yfazqb.com/Article/details/gzrwvuziv.sHtML

[U72] PHP：写错误日志
来源：http://m.share.bbcook.cn/Article/details/gwdaktwva.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.bbcook.cn/Article/details/gbogkvybu.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.epnwcf.com/Article/details/geesnlkis.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.epnwcf.com/Article/details/gitumgpbn.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fktsv.cn/Article/details/gqjubxdml.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.sjlbkw.cn/Article/details/gdaibrxze.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.bbcook.cn/Article/details/gaioeicwa.sHtML

composer require psr/container
来源：http://www.share.sjlbkw.cn/Article/details/gdubosrtb.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/glexmorgb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.vehdjk.com/Article/details/gkzvnbici.sHtML

[U77] PHP：模板渲染
来源：http://blog.epnwcf.com/Article/details/gptlhmvbt.sHtML

composer require twig/twig
来源：http://3g.fktsv.cn/Article/details/gyiawfceo.sHtML

[U78] PHP：单元测试
来源：http://wap.fktsv.cn/Article/details/gyzylolpt.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.bbcook.cn/Article/details/grsvrjjod.sHtML


<!-- 参考信息 -->