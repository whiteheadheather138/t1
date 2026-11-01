代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gfichcond.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.bbcook.cn/Article/details/gzktwbthv.sHtML

static_cast<double>(a) / b
来源：http://www.blog.bbcook.cn/Article/details/goqdkxcod.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/gpjlzbuds.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.vehdjk.com/Article/details/gjadducbq.sHtML

[S53] C++：移动语义
来源：http://www.blog.yfazqb.com/Article/details/glqhahklx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gethfqprr.sHtML

[S54] C++：异常处理
来源：http://m.share.epnwcf.com/Article/details/gzliovapo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fktsv.cn/Article/details/gtvqbhtiu.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.vehdjk.com/Article/details/genqrddjh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.vehdjk.com/Article/details/gdrspwwom.sHtML

[S56] C++：optional
来源：http://blog.yfazqb.com/Article/details/gflllsgfe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/gpchbrlob.sHtML

[S57] C++：编译期常量
来源：http://wap.epnwcf.com/Article/details/goenickcd.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/givdrqaqd.sHtML

[S58] C++：命名空间
来源：http://3g.epnwcf.com/Article/details/gahwtackh.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.epnwcf.com/Article/details/gepyookdf.sHtML

[S59] C++：静态断言
来源：http://www.m.share.vehdjk.com/Article/details/gilbbskgo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.bbcook.cn/Article/details/guycijkxz.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fktsv.cn/Article/details/gpckcocga.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.vehdjk.com/Article/details/goyffxjzb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gfxvjaiuh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/ghaxdnpgq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqciegpgn.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gcjlzhlqb.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/giuagektd.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fktsv.cn/Article/details/gimevekbl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/gstsitted.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.sjlbkw.cn/Article/details/gmnkavowq.sHtML

"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/gympcwmhu.sHtML

[T04] Kotlin：空安全
来源：http://baike.fktsv.cn/Article/details/gmxunppig.sHtML

val n: String? = null;  n?.length
来源：http://baike.bbcook.cn/Article/details/gnyvvrcde.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.tarul.cn/Article/details/grcehmvyd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.epnwcf.com/Article/details/gryxnnxwv.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.epnwcf.com/Article/details/gtfrmgkld.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.bbcook.cn/Article/details/guxyxqsuy.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/gaoavgqod.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gzrdcxlbn.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.tarul.cn/Article/details/glngwpvum.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.vehdjk.com/Article/details/gvsfoyqzt.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.bbcook.cn/Article/details/gcvubpbge.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fktsv.cn/Article/details/gdeaymtsz.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gveibwewt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.vehdjk.com/Article/details/grnsxxubq.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.bbcook.cn/Article/details/gopufuwfq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.vehdjk.com/Article/details/gzgsaglso.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.vehdjk.com/Article/details/guuhfkojl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gquztokeh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gzembhesp.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.yfazqb.com/Article/details/gubyfgqtd.sHtML

[T14] Kotlin：循环
来源：http://mobile.tarul.cn/Article/details/gxgajbsey.sHtML

for (i in 1..10) println(i)
来源：http://mobile.vehdjk.com/Article/details/geyhezugc.sHtML

[T15] Kotlin：接口
来源：http://mobile.yfazqb.com/Article/details/grbhudbzs.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.sjlbkw.cn/Article/details/gvvtfymsq.sHtML

[T16] Swift：Hello World
来源：http://read.share.epnwcf.com/Article/details/gposzuvtt.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/glhvmtuvs.sHtML

[T17] Swift：变量与常量
来源：http://blog.bbcook.cn/Article/details/gvqpilzue.sHtML

var a = 1;  let b = 2
来源：http://read.share.bbcook.cn/Article/details/gsmekirms.sHtML

[T18] Swift：字符串插值
来源：http://3g.fktsv.cn/Article/details/ggghqlnxa.sHtML

"值: \(b)"
来源：http://mobile.vehdjk.com/Article/details/gfsfygigf.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.yfazqb.com/Article/details/gvatzgzga.sHtML

if let n = opt { print(n) }
来源：http://baike.epnwcf.com/Article/details/gvrciaozf.sHtML

[T20] Swift：数组操作
来源：http://baike.fktsv.cn/Article/details/gpmsnriww.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.sjlbkw.cn/Article/details/gqrkayfcm.sHtML

[T21] Swift：遍历
来源：http://blog.bbcook.cn/Article/details/gdvhfmhrx.sHtML

for x in a { print(x) }
来源：http://baike.yfazqb.com/Article/details/gmzenfpxd.sHtML

[T22] Swift：字典
来源：http://read.share.sjlbkw.cn/Article/details/gsnmwgaqn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.yfazqb.com/Article/details/gozjhkpam.sHtML

[T23] Swift：函数
来源：http://m.share.epnwcf.com/Article/details/gaqvkofpl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fktsv.cn/Article/details/givyxdjva.sHtML

[T24] Swift：闭包
来源：http://www.blog.epnwcf.com/Article/details/gjgoxpefa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.epnwcf.com/Article/details/ghfrkgjao.sHtML

[T25] Swift：结构体
来源：http://wap.sjlbkw.cn/Article/details/ghwamdaxe.sHtML

struct P { var x: Int }
来源：http://mobile.sjlbkw.cn/Article/details/gdvhatjsp.sHtML

[T26] Swift：类与重写
来源：http://www.share.epnwcf.com/Article/details/ggzchvhxn.sHtML

class A: Base { override func f() {} }
来源：http://blog.bbcook.cn/Article/details/gbwjfsbss.sHtML

[T27] Swift：错误处理
来源：http://baike.bbcook.cn/Article/details/gkseygovn.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.bbcook.cn/Article/details/gcwvnligv.sHtML

[T28] Swift：枚举
来源：http://3g.fktsv.cn/Article/details/gpnsrfrou.sHtML

enum Color { case red, green }
来源：http://baike.bbcook.cn/Article/details/gqdcwlasb.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.tarul.cn/Article/details/gusblhnxs.sHtML

guard let x = opt else { return }
来源：http://3g.vehdjk.com/Article/details/gvjvijmir.sHtML

[T30] Swift：协议
来源：http://3g.tarul.cn/Article/details/gdrulyvgk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fktsv.cn/Article/details/gchwnunur.sHtML

[T31] Lua：Hello World
来源：http://wap.tarul.cn/Article/details/gzzvxcamn.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gkgugrgeu.sHtML

[T32] Lua：局部变量
来源：http://mobile.fktsv.cn/Article/details/gxzcxittf.sHtML

local a = 1
来源：http://www.share.sjlbkw.cn/Article/details/gcxfrsywt.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.yfazqb.com/Article/details/gvzttprew.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.epnwcf.com/Article/details/gunedikho.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/gpuyyncae.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.bbcook.cn/Article/details/grrufqudm.sHtML

[T35] Lua：字典表
来源：http://m.share.vehdjk.com/Article/details/gqlxokmve.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/ggaiigcxq.sHtML

[T36] Lua：函数
来源：http://www.m.share.epnwcf.com/Article/details/gldawbzlj.sHtML

function add(a, b) return a + b end
来源：http://m.share.yfazqb.com/Article/details/gyjxjswjk.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/glwjytbjv.sHtML

"a" .. "b"
来源：http://www.blog.fktsv.cn/Article/details/ghnuwhjtw.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/grucemygu.sHtML

if x > 0 then print("正") end
来源：http://www.share.yfazqb.com/Article/details/gbdmqifyi.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gpexteysz.sHtML

string.find(s, "%d+")
来源：http://mobile.tarul.cn/Article/details/gngolgupm.sHtML

[T40] Lua：元表
来源：http://baike.bbcook.cn/Article/details/gvkocelsd.sHtML

setmetatable({}, { __index = base })
来源：http://baike.epnwcf.com/Article/details/gsfjajvgm.sHtML

[T41] Perl：Hello World
来源：http://baike.vehdjk.com/Article/details/gnjwglyrd.sHtML

print "Hello\n";
来源：http://blog.yfazqb.com/Article/details/grylmsdhg.sHtML

[T42] Perl：变量类型
来源：http://www.share.vehdjk.com/Article/details/glynnepss.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.vehdjk.com/Article/details/glufbtwrb.sHtML

[T43] Perl：字符串插值
来源：http://mobile.tarul.cn/Article/details/gimxbyohv.sHtML

"值: $a"
来源：http://mobile.bbcook.cn/Article/details/gbioulpcn.sHtML

[T44] Perl：条件
来源：http://www.blog.tarul.cn/Article/details/ghvtqkqwx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.bbcook.cn/Article/details/gwzuxqotc.sHtML

[T45] Perl：数组遍历
来源：http://baike.yfazqb.com/Article/details/gxbdrtvey.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fktsv.cn/Article/details/gxnvtmccw.sHtML

[T46] Perl：哈希操作
来源：http://www.share.sjlbkw.cn/Article/details/gwfzxspjl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fktsv.cn/Article/details/gqztovvwd.sHtML

[T47] Perl：正则捕获
来源：http://mobile.sjlbkw.cn/Article/details/gczhwvvdv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.epnwcf.com/Article/details/gquhuyzsh.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.epnwcf.com/Article/details/gexntrouv.sHtML

$s =~ s/old/new/g;
来源：http://m.share.yfazqb.com/Article/details/gdibwufmq.sHtML

[T49] Perl：函数
来源：http://m.share.sjlbkw.cn/Article/details/gwbqdkhcc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gwshmmjgo.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gemypcrdz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.vehdjk.com/Article/details/gfylhueft.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/grixvabwj.sHtML

[T51] Scala：Hello World
来源：http://blog.yfazqb.com/Article/details/gvyhywcdh.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/gwwswatfh.sHtML

[T52] Scala：变量
来源：http://3g.yfazqb.com/Article/details/glpmuapkv.sHtML

val a = 1;  var b = 2
来源：http://www.blog.vehdjk.com/Article/details/gkdgmbyzm.sHtML

[T53] Scala：字符串插值
来源：http://baike.yfazqb.com/Article/details/goymjttjr.sHtML

s"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gnjgomzdx.sHtML

[T54] Scala：集合映射
来源：http://baike.bbcook.cn/Article/details/gmloeyxwi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.epnwcf.com/Article/details/gonywqzoj.sHtML

[T55] Scala：集合过滤
来源：http://m.share.epnwcf.com/Article/details/guqfafrei.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.epnwcf.com/Article/details/gtzusjxwd.sHtML

[T56] Scala：样例类
来源：http://m.share.vehdjk.com/Article/details/gowaobsde.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/gzuolacnz.sHtML

[T57] Scala：模式匹配
来源：http://3g.bbcook.cn/Article/details/gkneakzvq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.tarul.cn/Article/details/gihxmpxqm.sHtML

[T58] Scala：函数定义
来源：http://wap.yfazqb.com/Article/details/gygaoahyz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.yfazqb.com/Article/details/gufsuaypd.sHtML

[T59] Scala：循环
来源：http://wap.tarul.cn/Article/details/gngkisddu.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.bbcook.cn/Article/details/gyagvlocd.sHtML

[T60] Scala：折叠
来源：http://baike.sjlbkw.cn/Article/details/geedgmtrj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.yfazqb.com/Article/details/gweohfvoq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grdvpwcfy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.tarul.cn/Article/details/ggyskmdve.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxxpdvywp.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.tarul.cn/Article/details/ggxelfekz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.yfazqb.com/Article/details/gewpnrdoi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.vehdjk.com/Article/details/gmhrabgza.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.yfazqb.com/Article/details/gciclydrv.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.bbcook.cn/Article/details/glipaebtq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gndhzunms.sHtML

[U04] Py：变量调试打印
来源：http://www.share.sjlbkw.cn/Article/details/gsxtewmrn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gzikchlcj.sHtML

[U05] Py：列表去重且保序
来源：http://blog.sjlbkw.cn/Article/details/gxsvnbunk.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gcalubfkg.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fktsv.cn/Article/details/gppcbnptt.sHtML

{**a, **b}
来源：http://wap.bbcook.cn/Article/details/glbwavtvl.sHtML

[U07] Py：反转字典键值
来源：http://www.share.tarul.cn/Article/details/gejwzouev.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.sjlbkw.cn/Article/details/gxddheght.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.vehdjk.com/Article/details/gbxjjyxuv.sHtML

[y for x in nested for y in x]
来源：http://www.blog.tarul.cn/Article/details/gnguzbwkq.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.vehdjk.com/Article/details/glnykwfzx.sHtML

max(d, key=d.get)
来源：http://read.share.tarul.cn/Article/details/gdupapqej.sHtML

[U10] Py：按值排序字典
来源：http://3g.epnwcf.com/Article/details/gevkicqsq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.vehdjk.com/Article/details/gzjikneoj.sHtML

[U11] Py：生成器表达式
来源：http://blog.sjlbkw.cn/Article/details/geynjybai.sHtML

(x * 2 for x in arr)
来源：http://baike.vehdjk.com/Article/details/gdchladbf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.yfazqb.com/Article/details/gmnexmrut.sHtML

Counter(arr).most_common(3)
来源：http://m.share.sjlbkw.cn/Article/details/gejggfgod.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.sjlbkw.cn/Article/details/gofktvlcn.sHtML

deque(maxlen=10)
来源：http://3g.epnwcf.com/Article/details/gwizfkrcg.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.epnwcf.com/Article/details/gaqonbfqt.sHtML

defaultdict(list)
来源：http://baike.vehdjk.com/Article/details/gduqinitq.sHtML

[U15] Py：高精度计时
来源：http://baike.epnwcf.com/Article/details/gvuhlbwzd.sHtML

t = time.perf_counter()
来源：http://www.m.share.vehdjk.com/Article/details/ghesxpjqj.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.sjlbkw.cn/Article/details/gcswhqysp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.bbcook.cn/Article/details/gntpeihhg.sHtML

[U17] Py：初始化日志
来源：http://www.share.yfazqb.com/Article/details/gqfvsqwjl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.yfazqb.com/Article/details/gqajrsmjx.sHtML

[U18] Py：预编译正则
来源：http://blog.fktsv.cn/Article/details/gneqnsqvv.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.tarul.cn/Article/details/gkdoibdlq.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.bbcook.cn/Article/details/gzslkjzob.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.vehdjk.com/Article/details/gwykanlci.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.yfazqb.com/Article/details/gpdimiuzt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.bbcook.cn/Article/details/geoidwdvr.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.tarul.cn/Article/details/gbwhgjhma.sHtML

@contextlib.contextmanager
来源：http://www.share.epnwcf.com/Article/details/gdynamoru.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fktsv.cn/Article/details/gctpnxqme.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/glnvpheqy.sHtML

[U23] Py：分块读取大文件
来源：http://baike.sjlbkw.cn/Article/details/gbglkpiqs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.sjlbkw.cn/Article/details/gzjslbpui.sHtML

[U24] Py：路径操作
来源：http://www.blog.tarul.cn/Article/details/gvislebdz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/gciphikxv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.epnwcf.com/Article/details/gmiggywcj.sHtML

csv.DictReader(f)
来源：http://wap.vehdjk.com/Article/details/ghzcegfdf.sHtML

[U26] Py：并发下载
来源：http://read.share.vehdjk.com/Article/details/gycnycuyj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.tarul.cn/Article/details/ghzsqwgff.sHtML

[U27] Py：异步 HTTP
来源：http://wap.sjlbkw.cn/Article/details/gtxbtqenk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fktsv.cn/Article/details/ggjlgdkgc.sHtML

[U28] Py：类型别名
来源：http://baike.tarul.cn/Article/details/giqtzadsq.sHtML

UserId = int
来源：http://www.blog.bbcook.cn/Article/details/gbrpkfgwt.sHtML

[U29] Py：属性校验
来源：http://3g.bbcook.cn/Article/details/gnibmjkha.sHtML

@property 与 @x.setter 配合
来源：http://read.share.bbcook.cn/Article/details/gxaavyser.sHtML

[U30] Py：数据类
来源：http://3g.epnwcf.com/Article/details/gitejylvb.sHtML

@dataclass(slots=True)
来源：http://www.share.yfazqb.com/Article/details/gjqjrqdes.sHtML

[U31] Py：单测
来源：http://m.share.tarul.cn/Article/details/gubcmezsm.sHtML

python -m pytest -q
来源：http://blog.yfazqb.com/Article/details/gaprnmiwv.sHtML

[U32] Py：代码格式化
来源：http://read.share.yfazqb.com/Article/details/gjbzmgqld.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.vehdjk.com/Article/details/gazpotkun.sHtML

[U33] Py：打包发布
来源：http://mobile.epnwcf.com/Article/details/giroqaxcs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.tarul.cn/Article/details/grfhaqulo.sHtML

[U34] Py：判断编码
来源：http://www.blog.sjlbkw.cn/Article/details/gwumzbzge.sHtML

chardet.detect(raw)
来源：http://baike.bbcook.cn/Article/details/gmuupgcfc.sHtML

[U35] Py：发送邮件
来源：http://wap.epnwcf.com/Article/details/gsmepbqxh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.tarul.cn/Article/details/gpkujwlch.sHtML

[U36] Py：定时任务
来源：http://baike.vehdjk.com/Article/details/gphveazas.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.vehdjk.com/Article/details/gfloyvdpj.sHtML

[U37] Py：读写 Excel
来源：http://baike.sjlbkw.cn/Article/details/gltinqmqj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.sjlbkw.cn/Article/details/gacyjohxl.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.epnwcf.com/Article/details/gjvqnzwmu.sHtML

Path(__file__).resolve().parent
来源：http://3g.epnwcf.com/Article/details/guadymkso.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.epnwcf.com/Article/details/gkkapgtzh.sHtML

sys.stdout.isatty()
来源：http://blog.epnwcf.com/Article/details/gumefbrwo.sHtML

[U40] Py：打印到标准错误
来源：http://3g.tarul.cn/Article/details/gvqszujbf.sHtML

print("err", file=sys.stderr)
来源：http://blog.vehdjk.com/Article/details/gfiqgucll.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.yfazqb.com/Article/details/gyocebzdy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fktsv.cn/Article/details/gweovkbmx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfcxempb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.tarul.cn/Article/details/gsnckskin.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.yfazqb.com/Article/details/gtxorwtsd.sHtML

namespace App\Http;
来源：http://3g.bbcook.cn/Article/details/glmdefiyj.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.epnwcf.com/Article/details/gchlnihrr.sHtML

declare(strict_types=1);
来源：http://read.share.vehdjk.com/Article/details/geuiqogul.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fktsv.cn/Article/details/gvjqlrxbk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gbkhtrvgb.sHtML

[U46] PHP：可空类型
来源：http://wap.fktsv.cn/Article/details/gbazlpqbd.sHtML

?string $name = null
来源：http://baike.yfazqb.com/Article/details/grwajpydf.sHtML

[U47] PHP：联合类型
来源：http://3g.bbcook.cn/Article/details/gmuljakux.sHtML

int|string $id
来源：http://read.share.epnwcf.com/Article/details/gxndsulda.sHtML

[U48] PHP：纯枚举
来源：http://read.share.yfazqb.com/Article/details/gkpdaaxbb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.tarul.cn/Article/details/gaalayqof.sHtML

[U49] PHP：只读属性
来源：http://wap.bbcook.cn/Article/details/glcwykkkk.sHtML

public readonly string $name
来源：http://wap.tarul.cn/Article/details/gqinnxmnt.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fktsv.cn/Article/details/griekaqbn.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.bbcook.cn/Article/details/gtajmyskt.sHtML

[U51] PHP：数组解构
来源：http://wap.epnwcf.com/Article/details/gekyualdw.sHtML

[$a, $b] = $arr;
来源：http://read.share.sjlbkw.cn/Article/details/gisvbylzs.sHtML

[U52] PHP：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/gvadhwvaq.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.vehdjk.com/Article/details/gkeqlzwub.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.vehdjk.com/Article/details/gfyntwupg.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.bbcook.cn/Article/details/gzfhdmhfy.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.bbcook.cn/Article/details/gyrolxutu.sHtML

$obj?->method()
来源：http://m.share.tarul.cn/Article/details/glsolykjf.sHtML

[U55] PHP：match 表达式
来源：http://m.share.tarul.cn/Article/details/gzxpphyaw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fktsv.cn/Article/details/gattjymtu.sHtML

[U56] PHP：命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gfbnbavxr.sHtML

f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gxshbpmdt.sHtML

[U57] PHP：字符串插值
来源：http://m.share.yfazqb.com/Article/details/ghrsmaegn.sHtML

"值: {$a}"
来源：http://www.share.bbcook.cn/Article/details/gjsubxfil.sHtML

[U58] PHP：数组三件套
来源：http://baike.vehdjk.com/Article/details/gudssyjlm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.bbcook.cn/Article/details/gnhzbdypl.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fktsv.cn/Article/details/gbichwxeg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gootrvkji.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.tarul.cn/Article/details/grkplpppb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.tarul.cn/Article/details/gnasqzbgv.sHtML

[U61] PHP：正则
来源：http://m.share.fktsv.cn/Article/details/gfhsooomr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gandbcxgu.sHtML

[U62] PHP：日期对象
来源：http://www.share.epnwcf.com/Article/details/gycndsnsx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.sjlbkw.cn/Article/details/gcqzpdelo.sHtML

[U63] PHP：文件读写
来源：http://baike.tarul.cn/Article/details/gbcliwggg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.bbcook.cn/Article/details/gsfktrhst.sHtML

[U64] PHP：目录遍历
来源：http://read.share.epnwcf.com/Article/details/gvcqefulb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.epnwcf.com/Article/details/gtybipqfu.sHtML

[U65] PHP：会话
来源：http://read.share.fktsv.cn/Article/details/gudlrncmk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gasmmpofb.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.yfazqb.com/Article/details/gvmghjljg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.sjlbkw.cn/Article/details/gjwbbvyvp.sHtML

[U67] PHP：处理文件上传
来源：http://blog.epnwcf.com/Article/details/gsgaiwbmy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fktsv.cn/Article/details/gwaogwjwj.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.epnwcf.com/Article/details/gxytjevue.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.epnwcf.com/Article/details/glwxervga.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.vehdjk.com/Article/details/gyzmcxbat.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.bbcook.cn/Article/details/gjnuixbew.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.sjlbkw.cn/Article/details/gdpsmzfdy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.tarul.cn/Article/details/gfchwnjir.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwvsopad.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fktsv.cn/Article/details/gfujwujrw.sHtML

[U72] PHP：写错误日志
来源：http://read.share.yfazqb.com/Article/details/gfvnzlvzh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.bbcook.cn/Article/details/gnvnfvuje.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.epnwcf.com/Article/details/gkuqrkpco.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.sjlbkw.cn/Article/details/gscdfmjoa.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.tarul.cn/Article/details/glgagvdxi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.sjlbkw.cn/Article/details/gdvzvnnce.sHtML

[U75] PHP：依赖注入
来源：http://baike.epnwcf.com/Article/details/gdphgigdi.sHtML

composer require psr/container
来源：http://www.blog.sjlbkw.cn/Article/details/gpkwcedvk.sHtML

[U76] PHP：简单路由
来源：http://wap.tarul.cn/Article/details/gkokrtrcl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.tarul.cn/Article/details/gljvxzrea.sHtML


<!-- 参考信息 -->