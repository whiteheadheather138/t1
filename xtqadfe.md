代发 wailian999

while (std::getline(in, line)) { }
来源：http://mobile.yfazqb.com/Article/details/gmoikezeb.sHtML

[S49] C++：写文件
来源：http://blog.bbcook.cn/Article/details/glvuiyjqy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/gciyhyuho.sHtML

[S50] C++：格式化数字
来源：http://m.share.bbcook.cn/Article/details/gzqafrbcw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.vehdjk.com/Article/details/gzmaiymdq.sHtML

[S51] C++：显式类型转换
来源：http://3g.epnwcf.com/Article/details/gldmimacr.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/grgalqqhc.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.tarul.cn/Article/details/glcsdexzu.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.tarul.cn/Article/details/gelaplqtq.sHtML

[S53] C++：移动语义
来源：http://wap.vehdjk.com/Article/details/gqshwneyv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.yfazqb.com/Article/details/gilpbxohp.sHtML

[S54] C++：异常处理
来源：http://baike.vehdjk.com/Article/details/glppvlztm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.sjlbkw.cn/Article/details/gkyegtlwu.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.vehdjk.com/Article/details/glzvemggt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.yfazqb.com/Article/details/gkafunjmv.sHtML

[S56] C++：optional
来源：http://blog.vehdjk.com/Article/details/gmzormmal.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/giglhfkon.sHtML

[S57] C++：编译期常量
来源：http://wap.bbcook.cn/Article/details/gxqlonwkz.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gxjmxvdqu.sHtML

[S58] C++：命名空间
来源：http://read.share.yfazqb.com/Article/details/grxbqltgs.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.tarul.cn/Article/details/gnwipygzk.sHtML

[S59] C++：静态断言
来源：http://blog.sjlbkw.cn/Article/details/gihgujdzn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fktsv.cn/Article/details/gllzwouzm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.bbcook.cn/Article/details/gulbfhucz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.yfazqb.com/Article/details/gzybpmgjf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/giolifrla.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/gbgfewjet.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/goylfdctv.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gcfxamflo.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gmicgjyvt.sHtML

[T02] Kotlin：变量
来源：http://read.share.yfazqb.com/Article/details/ggpydhdzb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.bbcook.cn/Article/details/gjuwbbmpr.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fktsv.cn/Article/details/gbibgswag.sHtML

"值: $b"
来源：http://3g.bbcook.cn/Article/details/golxtnabm.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.tarul.cn/Article/details/grhaxitmb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gathnoyci.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gmrdpvewc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/ggxfkilmh.sHtML

[T06] Kotlin：集合映射
来源：http://wap.epnwcf.com/Article/details/gpzjvsbll.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.tarul.cn/Article/details/gdqfttlvb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.vehdjk.com/Article/details/gkwspdgtj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.yfazqb.com/Article/details/gfzwmisnv.sHtML

[T08] Kotlin：数据类
来源：http://read.share.sjlbkw.cn/Article/details/gsjeahpeu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.vehdjk.com/Article/details/gdwwsqfos.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.vehdjk.com/Article/details/gmhjqufub.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.yfazqb.com/Article/details/gkemgiyph.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.vehdjk.com/Article/details/givezyfrp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.tarul.cn/Article/details/gqlkhgrfv.sHtML

[T11] Kotlin：协程
来源：http://m.share.yfazqb.com/Article/details/girfsryze.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.tarul.cn/Article/details/gankhuoqh.sHtML

[T12] Kotlin：解构声明
来源：http://baike.sjlbkw.cn/Article/details/gapufbkmm.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gdamcgayt.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.epnwcf.com/Article/details/gcpgtjrrf.sHtML

val m = mapOf("a" to 1)
来源：http://wap.tarul.cn/Article/details/gtivfscrj.sHtML

[T14] Kotlin：循环
来源：http://baike.sjlbkw.cn/Article/details/ghgaxhflu.sHtML

for (i in 1..10) println(i)
来源：http://3g.bbcook.cn/Article/details/gtovcgqhk.sHtML

[T15] Kotlin：接口
来源：http://m.share.vehdjk.com/Article/details/gavhennhk.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.vehdjk.com/Article/details/gpwvdcvnr.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/goypjyxtx.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/ghzliqnsz.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fktsv.cn/Article/details/gkjbqhxju.sHtML

var a = 1;  let b = 2
来源：http://wap.sjlbkw.cn/Article/details/glcnwyemm.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gtdccecbj.sHtML

"值: \(b)"
来源：http://www.blog.bbcook.cn/Article/details/grwwuqxcq.sHtML

[T19] Swift：可选绑定
来源：http://blog.epnwcf.com/Article/details/gljgbzrrs.sHtML

if let n = opt { print(n) }
来源：http://baike.sjlbkw.cn/Article/details/gbztqolet.sHtML

[T20] Swift：数组操作
来源：http://www.share.vehdjk.com/Article/details/goavhfxws.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/gxxwnqrij.sHtML

[T21] Swift：遍历
来源：http://m.share.sjlbkw.cn/Article/details/gypmhqfvo.sHtML

for x in a { print(x) }
来源：http://blog.sjlbkw.cn/Article/details/gfiovtvou.sHtML

[T22] Swift：字典
来源：http://mobile.vehdjk.com/Article/details/gdwdcrqnt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.yfazqb.com/Article/details/glnbyeahm.sHtML

[T23] Swift：函数
来源：http://3g.sjlbkw.cn/Article/details/gvaklimep.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/gsokzmzdg.sHtML

[T24] Swift：闭包
来源：http://www.share.epnwcf.com/Article/details/gxilgsddf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.vehdjk.com/Article/details/ggowpnxnk.sHtML

[T25] Swift：结构体
来源：http://www.share.bbcook.cn/Article/details/gfjslfwtn.sHtML

struct P { var x: Int }
来源：http://www.share.bbcook.cn/Article/details/gtigbccyc.sHtML

[T26] Swift：类与重写
来源：http://blog.epnwcf.com/Article/details/geqczhxqw.sHtML

class A: Base { override func f() {} }
来源：http://m.share.bbcook.cn/Article/details/gylasnwjc.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/giyvvfodr.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.yfazqb.com/Article/details/gvgkmfgrx.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gcqvdlvdi.sHtML

enum Color { case red, green }
来源：http://baike.sjlbkw.cn/Article/details/gefmqcely.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.tarul.cn/Article/details/guyaudawa.sHtML

guard let x = opt else { return }
来源：http://mobile.bbcook.cn/Article/details/gtpcgemfq.sHtML

[T30] Swift：协议
来源：http://m.share.epnwcf.com/Article/details/gmzjspwvc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.bbcook.cn/Article/details/gzohffgqw.sHtML

[T31] Lua：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gunhtpold.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gdxcatgjo.sHtML

[T32] Lua：局部变量
来源：http://3g.yfazqb.com/Article/details/gsjpmdqqr.sHtML

local a = 1
来源：http://blog.fktsv.cn/Article/details/gflyxwxve.sHtML

[T33] Lua：表（数组）
来源：http://blog.sjlbkw.cn/Article/details/gnvpenbei.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.epnwcf.com/Article/details/gsfdraemv.sHtML

[T34] Lua：遍历表
来源：http://m.share.bbcook.cn/Article/details/glujzcnqm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.vehdjk.com/Article/details/ggldrkncs.sHtML

[T35] Lua：字典表
来源：http://baike.yfazqb.com/Article/details/gtbdrolpz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.epnwcf.com/Article/details/gpzkzqxxr.sHtML

[T36] Lua：函数
来源：http://mobile.tarul.cn/Article/details/ghvpshvuy.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fktsv.cn/Article/details/gxlapllqx.sHtML

[T37] Lua：字符串拼接
来源：http://wap.yfazqb.com/Article/details/gldlkpqzt.sHtML

"a" .. "b"
来源：http://3g.yfazqb.com/Article/details/gskmcmchz.sHtML

[T38] Lua：条件
来源：http://mobile.sjlbkw.cn/Article/details/goljrjhtk.sHtML

if x > 0 then print("正") end
来源：http://baike.yfazqb.com/Article/details/gsmrnvtrm.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gwbhqcmqt.sHtML

string.find(s, "%d+")
来源：http://wap.vehdjk.com/Article/details/gtnvqfygi.sHtML

[T40] Lua：元表
来源：http://baike.vehdjk.com/Article/details/gdyyfordi.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.vehdjk.com/Article/details/gehjgzsqh.sHtML

[T41] Perl：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gbrdbfzbr.sHtML

print "Hello\n";
来源：http://blog.vehdjk.com/Article/details/gbhavnkyw.sHtML

[T42] Perl：变量类型
来源：http://wap.bbcook.cn/Article/details/gebettrov.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fktsv.cn/Article/details/guosmifjq.sHtML

[T43] Perl：字符串插值
来源：http://baike.tarul.cn/Article/details/giqcmcjus.sHtML

"值: $a"
来源：http://baike.tarul.cn/Article/details/gldqjbouo.sHtML

[T44] Perl：条件
来源：http://m.share.tarul.cn/Article/details/grwptloor.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/gcwlhungu.sHtML

[T45] Perl：数组遍历
来源：http://m.share.tarul.cn/Article/details/gwknyztus.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.vehdjk.com/Article/details/ghpdkwhqk.sHtML

[T46] Perl：哈希操作
来源：http://mobile.tarul.cn/Article/details/gzarxgumq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.vehdjk.com/Article/details/gzqkhghnh.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.sjlbkw.cn/Article/details/gltoxadfg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.vehdjk.com/Article/details/gohapjvde.sHtML

[T48] Perl：正则替换
来源：http://www.share.bbcook.cn/Article/details/gozyaizsu.sHtML

$s =~ s/old/new/g;
来源：http://blog.tarul.cn/Article/details/ggqrtaxsm.sHtML

[T49] Perl：函数
来源：http://www.share.sjlbkw.cn/Article/details/gomidfxmz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gqubeanyy.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gxcxuetrj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.tarul.cn/Article/details/glthrgekd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.bbcook.cn/Article/details/guyslnudj.sHtML

[T51] Scala：Hello World
来源：http://blog.yfazqb.com/Article/details/glnsqrutr.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gmxpyjgap.sHtML

[T52] Scala：变量
来源：http://baike.bbcook.cn/Article/details/gdkivsmnv.sHtML

val a = 1;  var b = 2
来源：http://read.share.epnwcf.com/Article/details/gqsqcbqek.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/galpbljfx.sHtML

s"值: $b"
来源：http://read.share.yfazqb.com/Article/details/gmrbuhjxn.sHtML

[T54] Scala：集合映射
来源：http://mobile.yfazqb.com/Article/details/gcnuarzhf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.bbcook.cn/Article/details/gclpwphiw.sHtML

[T55] Scala：集合过滤
来源：http://3g.yfazqb.com/Article/details/glqaxunci.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.epnwcf.com/Article/details/glgvdgtoo.sHtML

[T56] Scala：样例类
来源：http://baike.bbcook.cn/Article/details/giuffxspx.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fktsv.cn/Article/details/glldvsrgf.sHtML

[T57] Scala：模式匹配
来源：http://mobile.epnwcf.com/Article/details/ginfpklmz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.epnwcf.com/Article/details/gzfvrfokq.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/gmmmskzxj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.sjlbkw.cn/Article/details/grdcxgdtm.sHtML

[T59] Scala：循环
来源：http://wap.vehdjk.com/Article/details/gbvynfmdu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gzitnidyb.sHtML

[T60] Scala：折叠
来源：http://blog.bbcook.cn/Article/details/glvectean.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.yfazqb.com/Article/details/gezgnnkvd.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gyasffrzo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fktsv.cn/Article/details/gmbunxjef.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzgjdzozd.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.bbcook.cn/Article/details/gqyvmqzvr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.tarul.cn/Article/details/gkktnwyez.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.tarul.cn/Article/details/gczklslye.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.bbcook.cn/Article/details/ggxeozrrz.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.epnwcf.com/Article/details/gndrvouby.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.epnwcf.com/Article/details/gulswrixs.sHtML

[U04] Py：变量调试打印
来源：http://blog.sjlbkw.cn/Article/details/gmgtzdelv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.yfazqb.com/Article/details/gcluqkvfq.sHtML

[U05] Py：列表去重且保序
来源：http://wap.sjlbkw.cn/Article/details/grngsqzia.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gpfaeilqo.sHtML

[U06] Py：合并两个字典
来源：http://wap.epnwcf.com/Article/details/gcxgblkqw.sHtML

{**a, **b}
来源：http://www.blog.yfazqb.com/Article/details/grfbvbgny.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gnkkthvbh.sHtML

{v: k for k, v in d.items()}
来源：http://blog.bbcook.cn/Article/details/gpdezhmml.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fktsv.cn/Article/details/gixmznxyj.sHtML

[y for x in nested for y in x]
来源：http://m.share.vehdjk.com/Article/details/ggiykcdyw.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.sjlbkw.cn/Article/details/gtgkvwiey.sHtML

max(d, key=d.get)
来源：http://m.share.epnwcf.com/Article/details/gyygiewda.sHtML

[U10] Py：按值排序字典
来源：http://baike.yfazqb.com/Article/details/gsprbdslf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.tarul.cn/Article/details/gszlrrmym.sHtML

[U11] Py：生成器表达式
来源：http://www.share.bbcook.cn/Article/details/gmnpcchme.sHtML

(x * 2 for x in arr)
来源：http://www.share.epnwcf.com/Article/details/gbjymrtgj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.epnwcf.com/Article/details/gzgsdkskp.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gmgujeumw.sHtML

[U13] Py：固定长度队列
来源：http://blog.tarul.cn/Article/details/gyvchifyz.sHtML

deque(maxlen=10)
来源：http://www.share.yfazqb.com/Article/details/gzxedpzaz.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fktsv.cn/Article/details/ghmhunusp.sHtML

defaultdict(list)
来源：http://www.m.share.fktsv.cn/Article/details/gffwttwdk.sHtML

[U15] Py：高精度计时
来源：http://www.blog.yfazqb.com/Article/details/gewdcuarm.sHtML

t = time.perf_counter()
来源：http://mobile.tarul.cn/Article/details/geflfjoum.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.sjlbkw.cn/Article/details/gtybtkixl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.epnwcf.com/Article/details/gkofhkcoi.sHtML

[U17] Py：初始化日志
来源：http://www.share.tarul.cn/Article/details/gqryvgcsw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.epnwcf.com/Article/details/gblecipuw.sHtML

[U18] Py：预编译正则
来源：http://mobile.tarul.cn/Article/details/gxeqsupjl.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fktsv.cn/Article/details/glsqgonec.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.vehdjk.com/Article/details/gofzbbbxw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fktsv.cn/Article/details/grqcdmsyd.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.bbcook.cn/Article/details/gakodokwa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.vehdjk.com/Article/details/glozfcnwk.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.yfazqb.com/Article/details/gmzbtkdjh.sHtML

@contextlib.contextmanager
来源：http://www.m.share.sjlbkw.cn/Article/details/gzeemgzga.sHtML

[U22] Py：矩阵转置
来源：http://3g.tarul.cn/Article/details/gydtbyzyh.sHtML

list(zip(*m))
来源：http://wap.fktsv.cn/Article/details/gtjbjcdfl.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.yfazqb.com/Article/details/gaxtqrqgk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.yfazqb.com/Article/details/gdcvcpafx.sHtML

[U24] Py：路径操作
来源：http://read.share.yfazqb.com/Article/details/grxmulevl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.vehdjk.com/Article/details/gffmupbcl.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.epnwcf.com/Article/details/gvnqwexsx.sHtML

csv.DictReader(f)
来源：http://m.share.sjlbkw.cn/Article/details/gvinbhock.sHtML

[U26] Py：并发下载
来源：http://read.share.bbcook.cn/Article/details/gyutlyymv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.vehdjk.com/Article/details/gwgrsbxox.sHtML

[U27] Py：异步 HTTP
来源：http://blog.epnwcf.com/Article/details/gbacjssfo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.bbcook.cn/Article/details/gkailqkwe.sHtML

[U28] Py：类型别名
来源：http://3g.tarul.cn/Article/details/gdzpfkzmt.sHtML

UserId = int
来源：http://mobile.epnwcf.com/Article/details/gbpuowjxn.sHtML

[U29] Py：属性校验
来源：http://www.m.share.tarul.cn/Article/details/gvswpmkvr.sHtML

@property 与 @x.setter 配合
来源：http://baike.vehdjk.com/Article/details/gcemzojiz.sHtML

[U30] Py：数据类
来源：http://wap.yfazqb.com/Article/details/gunoqubqa.sHtML

@dataclass(slots=True)
来源：http://wap.bbcook.cn/Article/details/gigjdwfru.sHtML

[U31] Py：单测
来源：http://baike.epnwcf.com/Article/details/guzohyftk.sHtML

python -m pytest -q
来源：http://m.share.yfazqb.com/Article/details/gefiggwzw.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fktsv.cn/Article/details/gztfdxhqg.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.tarul.cn/Article/details/glesycicj.sHtML

[U33] Py：打包发布
来源：http://www.blog.fktsv.cn/Article/details/gwvekhrgw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.yfazqb.com/Article/details/gvxkmeehb.sHtML

[U34] Py：判断编码
来源：http://wap.epnwcf.com/Article/details/gwtbvjbrv.sHtML

chardet.detect(raw)
来源：http://www.m.share.yfazqb.com/Article/details/gkmgzdsgb.sHtML

[U35] Py：发送邮件
来源：http://blog.sjlbkw.cn/Article/details/gqyefmrhg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.vehdjk.com/Article/details/gqcrrsrhg.sHtML

[U36] Py：定时任务
来源：http://wap.sjlbkw.cn/Article/details/gwgqkzqzx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fktsv.cn/Article/details/gutdsdfat.sHtML

[U37] Py：读写 Excel
来源：http://wap.yfazqb.com/Article/details/gralplpon.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.yfazqb.com/Article/details/gyqxmlakp.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.tarul.cn/Article/details/gtnqeokzb.sHtML

Path(__file__).resolve().parent
来源：http://3g.epnwcf.com/Article/details/gvucnrswl.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.tarul.cn/Article/details/gdqgdwvkn.sHtML

sys.stdout.isatty()
来源：http://mobile.fktsv.cn/Article/details/gfrdcympc.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fktsv.cn/Article/details/gxgzmmqmz.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/grdndcwos.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.vehdjk.com/Article/details/gvrdxvlxw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fktsv.cn/Article/details/gagtgwjoc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.tarul.cn/Article/details/gymmyuopd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.yfazqb.com/Article/details/gjghfgwip.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.bbcook.cn/Article/details/ghpnrkopp.sHtML

namespace App\Http;
来源：http://m.share.tarul.cn/Article/details/ggkukaeuv.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.sjlbkw.cn/Article/details/gkbmjjomu.sHtML

declare(strict_types=1);
来源：http://read.share.yfazqb.com/Article/details/gcqlnnnvr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fktsv.cn/Article/details/grgcjeqtk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/goblizpxw.sHtML

[U46] PHP：可空类型
来源：http://www.blog.tarul.cn/Article/details/ggwnhsiwx.sHtML

?string $name = null
来源：http://www.m.share.sjlbkw.cn/Article/details/gzczwjviv.sHtML

[U47] PHP：联合类型
来源：http://read.share.vehdjk.com/Article/details/gzsvjaabr.sHtML

int|string $id
来源：http://www.blog.tarul.cn/Article/details/geqqqhxhu.sHtML

[U48] PHP：纯枚举
来源：http://blog.fktsv.cn/Article/details/gnscvmvjq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.yfazqb.com/Article/details/gwirrffvu.sHtML

[U49] PHP：只读属性
来源：http://blog.epnwcf.com/Article/details/gfudexdff.sHtML

public readonly string $name
来源：http://read.share.tarul.cn/Article/details/gmlbtnbid.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.yfazqb.com/Article/details/geqqwrtyz.sHtML

public function __construct(private int $id) {}
来源：http://wap.bbcook.cn/Article/details/geuklahgy.sHtML

[U51] PHP：数组解构
来源：http://wap.fktsv.cn/Article/details/groaiufql.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdpanbcy.sHtML

[U52] PHP：箭头函数
来源：http://3g.fktsv.cn/Article/details/gxzfwzqkj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.sjlbkw.cn/Article/details/gnmvfdxmk.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.bbcook.cn/Article/details/gcmnpwubl.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.sjlbkw.cn/Article/details/ggvjpbxgz.sHtML

[U54] PHP：空安全调用
来源：http://www.share.tarul.cn/Article/details/gwlaktqky.sHtML

$obj?->method()
来源：http://m.share.epnwcf.com/Article/details/gfnzlunby.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.tarul.cn/Article/details/gnukkuerd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.vehdjk.com/Article/details/gwhzgtaqi.sHtML

[U56] PHP：命名参数
来源：http://www.share.bbcook.cn/Article/details/gkvsbeijw.sHtML

f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gorwllxma.sHtML

[U57] PHP：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/grontxpiv.sHtML

"值: {$a}"
来源：http://www.m.share.epnwcf.com/Article/details/grfnrmmwo.sHtML

[U58] PHP：数组三件套
来源：http://blog.epnwcf.com/Article/details/gescptsui.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.sjlbkw.cn/Article/details/gjswrwkyf.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.yfazqb.com/Article/details/gvkgkhkyk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.vehdjk.com/Article/details/gaojorles.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.bbcook.cn/Article/details/gnnitmgvm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.sjlbkw.cn/Article/details/gruspuynx.sHtML

[U61] PHP：正则
来源：http://3g.tarul.cn/Article/details/gyqxdtncb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gphzfvsoz.sHtML

[U62] PHP：日期对象
来源：http://read.share.sjlbkw.cn/Article/details/gskowanqk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fktsv.cn/Article/details/glqvzopcx.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.epnwcf.com/Article/details/gikztulsp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.sjlbkw.cn/Article/details/gjotwexom.sHtML

[U64] PHP：目录遍历
来源：http://3g.tarul.cn/Article/details/gncxkwhib.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fktsv.cn/Article/details/gurudvlvx.sHtML

[U65] PHP：会话
来源：http://read.share.vehdjk.com/Article/details/gysflnckq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gsaixxcfa.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.bbcook.cn/Article/details/gieblpvfs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.yfazqb.com/Article/details/gkglvmani.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.tarul.cn/Article/details/gzpoinfqp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.yfazqb.com/Article/details/ghfidmwfj.sHtML

[U68] PHP：PDO 连接
来源：http://wap.yfazqb.com/Article/details/grlcwggmv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.sjlbkw.cn/Article/details/gdpyonrnw.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.tarul.cn/Article/details/gpadgezns.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.bbcook.cn/Article/details/gytkhxgvi.sHtML

[U70] PHP：PDO 事务
来源：http://blog.tarul.cn/Article/details/glcwpoojk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.yfazqb.com/Article/details/gkwsvkcru.sHtML

[U71] PHP：抛出异常
来源：http://baike.fktsv.cn/Article/details/gevjtuifj.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.vehdjk.com/Article/details/gbmjszuqy.sHtML

[U72] PHP：写错误日志
来源：http://blog.tarul.cn/Article/details/gsbtntfvy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.epnwcf.com/Article/details/glvkynlfk.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.bbcook.cn/Article/details/gbnebmpiy.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.yfazqb.com/Article/details/gildjbtrg.sHtML

[U74] PHP：读取环境变量
来源：http://blog.bbcook.cn/Article/details/gaincvjic.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fktsv.cn/Article/details/grfybazjt.sHtML


<!-- 参考信息 -->