代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gjcaahoie.sHtML

[S51] C++：显式类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gjhlwekuw.sHtML

static_cast<double>(a) / b
来源：http://3g.tarul.cn/Article/details/goqkrutdh.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gisjihveh.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.sjlbkw.cn/Article/details/gjultrdid.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/gdwdqzfow.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.sjlbkw.cn/Article/details/ghhohxudi.sHtML

[S54] C++：异常处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gadfgqfmn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.bbcook.cn/Article/details/gvufrkkyb.sHtML

[S55] C++：结构化绑定
来源：http://blog.bbcook.cn/Article/details/gsawfxurg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/gzxwykrsd.sHtML

[S56] C++：optional
来源：http://3g.sjlbkw.cn/Article/details/gpifzlhfq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.sjlbkw.cn/Article/details/glluldygz.sHtML

[S57] C++：编译期常量
来源：http://wap.yfazqb.com/Article/details/gudcnflns.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/gpjcyaliz.sHtML

[S58] C++：命名空间
来源：http://blog.fktsv.cn/Article/details/ghxiaydau.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fktsv.cn/Article/details/gznitmcij.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/gnjkhlcjc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.tarul.cn/Article/details/gaypxnuua.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fktsv.cn/Article/details/gligcybye.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/gknchyubz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdfvsccjx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/gibzjzszy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gyxkhxopa.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gcqkcexbd.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gwccqajob.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gsvnlhqme.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fktsv.cn/Article/details/gbrbxzpus.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.epnwcf.com/Article/details/giywfyfke.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/ggevmdvjf.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/grjgopsxb.sHtML

val n: String? = null;  n?.length
来源：http://read.share.epnwcf.com/Article/details/gqhwomuna.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/gvcmevphi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fktsv.cn/Article/details/griovsvej.sHtML

[T06] Kotlin：集合映射
来源：http://baike.vehdjk.com/Article/details/gacpthsmq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gsyibwqtt.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.yfazqb.com/Article/details/gdrmvmtqk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/gyxogmliw.sHtML

[T08] Kotlin：数据类
来源：http://baike.bbcook.cn/Article/details/gusleaepj.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.epnwcf.com/Article/details/gmfxifyqk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/gqircouxc.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.tarul.cn/Article/details/gkezxynmk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.yfazqb.com/Article/details/gwbvfcelb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.sjlbkw.cn/Article/details/gqxyvofxb.sHtML

[T11] Kotlin：协程
来源：http://read.share.bbcook.cn/Article/details/gwvbmodbf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.epnwcf.com/Article/details/ggnkjdldx.sHtML

[T12] Kotlin：解构声明
来源：http://blog.vehdjk.com/Article/details/gofuctvxl.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gqqluczoi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gpmmfksvu.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.yfazqb.com/Article/details/gaskzwfnf.sHtML

[T14] Kotlin：循环
来源：http://baike.yfazqb.com/Article/details/gyjbjqbjy.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/glulypgdx.sHtML

[T15] Kotlin：接口
来源：http://www.blog.bbcook.cn/Article/details/gowmdsuor.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.tarul.cn/Article/details/gumhliclw.sHtML

[T16] Swift：Hello World
来源：http://mobile.vehdjk.com/Article/details/grsimtzwo.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gxbdvlufd.sHtML

[T17] Swift：变量与常量
来源：http://3g.sjlbkw.cn/Article/details/gkljwmnze.sHtML

var a = 1;  let b = 2
来源：http://mobile.bbcook.cn/Article/details/gcbvfyxgd.sHtML

[T18] Swift：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gobdrmkjg.sHtML

"值: \(b)"
来源：http://3g.yfazqb.com/Article/details/gtwadeecz.sHtML

[T19] Swift：可选绑定
来源：http://m.share.epnwcf.com/Article/details/gqvzetwmq.sHtML

if let n = opt { print(n) }
来源：http://3g.fktsv.cn/Article/details/gzwyxradw.sHtML

[T20] Swift：数组操作
来源：http://read.share.bbcook.cn/Article/details/grdutkltc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.epnwcf.com/Article/details/ggfvqnhcu.sHtML

[T21] Swift：遍历
来源：http://www.blog.vehdjk.com/Article/details/gmkmymqao.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/gvtmhvsef.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/gyhmddgxw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/gqlohrgjq.sHtML

[T23] Swift：函数
来源：http://baike.vehdjk.com/Article/details/ghrhvwmql.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.bbcook.cn/Article/details/gdsfrkbvq.sHtML

[T24] Swift：闭包
来源：http://3g.tarul.cn/Article/details/gbprhzhes.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gmlktbxhq.sHtML

[T25] Swift：结构体
来源：http://wap.tarul.cn/Article/details/ghzmidkpt.sHtML

struct P { var x: Int }
来源：http://read.share.sjlbkw.cn/Article/details/gukiydazp.sHtML

[T26] Swift：类与重写
来源：http://blog.fktsv.cn/Article/details/gplafcqcu.sHtML

class A: Base { override func f() {} }
来源：http://3g.tarul.cn/Article/details/gxvbawldh.sHtML

[T27] Swift：错误处理
来源：http://www.blog.bbcook.cn/Article/details/givdxlppe.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.epnwcf.com/Article/details/gthvavwst.sHtML

[T28] Swift：枚举
来源：http://mobile.tarul.cn/Article/details/gnjoerhac.sHtML

enum Color { case red, green }
来源：http://baike.bbcook.cn/Article/details/goaoyzhzv.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/gyjdtywgq.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/gknhbxcyb.sHtML

[T30] Swift：协议
来源：http://3g.bbcook.cn/Article/details/gjhbyohcy.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.vehdjk.com/Article/details/gtqcvsstw.sHtML

[T31] Lua：Hello World
来源：http://www.share.epnwcf.com/Article/details/gwkhqjosf.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gsraklwpw.sHtML

[T32] Lua：局部变量
来源：http://m.share.vehdjk.com/Article/details/gtvzarryj.sHtML

local a = 1
来源：http://www.share.tarul.cn/Article/details/ghefrkuuv.sHtML

[T33] Lua：表（数组）
来源：http://blog.bbcook.cn/Article/details/gflmszqbp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.sjlbkw.cn/Article/details/grozsygbq.sHtML

[T34] Lua：遍历表
来源：http://3g.yfazqb.com/Article/details/guyuufsoq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.bbcook.cn/Article/details/gukidaaee.sHtML

[T35] Lua：字典表
来源：http://mobile.bbcook.cn/Article/details/gwomqabum.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.sjlbkw.cn/Article/details/giyjekhbv.sHtML

[T36] Lua：函数
来源：http://www.blog.epnwcf.com/Article/details/guuytnkne.sHtML

function add(a, b) return a + b end
来源：http://mobile.epnwcf.com/Article/details/glbrjhkzd.sHtML

[T37] Lua：字符串拼接
来源：http://baike.vehdjk.com/Article/details/govmxkrlm.sHtML

"a" .. "b"
来源：http://blog.yfazqb.com/Article/details/gljytuunc.sHtML

[T38] Lua：条件
来源：http://m.share.epnwcf.com/Article/details/gotuauwce.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.sjlbkw.cn/Article/details/giqpfpbhy.sHtML

[T39] Lua：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/gnnfisghl.sHtML

string.find(s, "%d+")
来源：http://baike.sjlbkw.cn/Article/details/gyuvyworu.sHtML

[T40] Lua：元表
来源：http://m.share.epnwcf.com/Article/details/gfzcaeuup.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.vehdjk.com/Article/details/gsjkpxbtb.sHtML

[T41] Perl：Hello World
来源：http://read.share.epnwcf.com/Article/details/ggpdxmzob.sHtML

print "Hello\n";
来源：http://blog.sjlbkw.cn/Article/details/gycoanrbn.sHtML

[T42] Perl：变量类型
来源：http://3g.vehdjk.com/Article/details/gswqmifxe.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.epnwcf.com/Article/details/gakfvyyjg.sHtML

[T43] Perl：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gfygjmkbd.sHtML

"值: $a"
来源：http://www.blog.epnwcf.com/Article/details/gduzdskls.sHtML

[T44] Perl：条件
来源：http://www.m.share.epnwcf.com/Article/details/godnidksw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fktsv.cn/Article/details/gzwixbfvp.sHtML

[T45] Perl：数组遍历
来源：http://www.share.yfazqb.com/Article/details/gnwifknjq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.epnwcf.com/Article/details/gfiuukmgy.sHtML

[T46] Perl：哈希操作
来源：http://mobile.sjlbkw.cn/Article/details/grawjhzth.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.yfazqb.com/Article/details/gzwvnztbz.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.vehdjk.com/Article/details/gsgrelbky.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.yfazqb.com/Article/details/gtpnymmkm.sHtML

[T48] Perl：正则替换
来源：http://baike.bbcook.cn/Article/details/gxivpdvdb.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.vehdjk.com/Article/details/gwkvlnygh.sHtML

[T49] Perl：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtooepmuf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gqhvzpixi.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gqjgpfrfl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.vehdjk.com/Article/details/gpowwbhmz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.bbcook.cn/Article/details/ghvyvwuba.sHtML

[T51] Scala：Hello World
来源：http://mobile.bbcook.cn/Article/details/ggltudsip.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gedkrzhje.sHtML

[T52] Scala：变量
来源：http://wap.yfazqb.com/Article/details/gnnwwnkyi.sHtML

val a = 1;  var b = 2
来源：http://wap.fktsv.cn/Article/details/gqkjfwhet.sHtML

[T53] Scala：字符串插值
来源：http://blog.vehdjk.com/Article/details/gsjblrems.sHtML

s"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gryxkcmzd.sHtML

[T54] Scala：集合映射
来源：http://read.share.bbcook.cn/Article/details/gyazazgpq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.vehdjk.com/Article/details/ghlracpyn.sHtML

[T55] Scala：集合过滤
来源：http://m.share.tarul.cn/Article/details/gikwivdzz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.yfazqb.com/Article/details/gczwfmfka.sHtML

[T56] Scala：样例类
来源：http://3g.bbcook.cn/Article/details/gswwnumwm.sHtML

case class User(name: String, age: Int)
来源：http://www.share.tarul.cn/Article/details/gusxcpkit.sHtML

[T57] Scala：模式匹配
来源：http://blog.fktsv.cn/Article/details/gogprrcys.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fktsv.cn/Article/details/gwcnbnnzw.sHtML

[T58] Scala：函数定义
来源：http://mobile.tarul.cn/Article/details/gymuxywiu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.tarul.cn/Article/details/gynpudmjh.sHtML

[T59] Scala：循环
来源：http://www.share.fktsv.cn/Article/details/grfagmvjt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/gddfgfnla.sHtML

[T60] Scala：折叠
来源：http://mobile.tarul.cn/Article/details/gwlphsned.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.tarul.cn/Article/details/gsattxflu.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gebtsispm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/gqvvystzm.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gytemtlrs.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fktsv.cn/Article/details/gbgvulasr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.vehdjk.com/Article/details/glerjdqpf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.vehdjk.com/Article/details/gwmbuddlg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.epnwcf.com/Article/details/gyrydlovj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.yfazqb.com/Article/details/goeqdzzqx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.bbcook.cn/Article/details/gckyhwbqa.sHtML

[U04] Py：变量调试打印
来源：http://m.share.tarul.cn/Article/details/gudhcvxsm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/gvpclmvlc.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fktsv.cn/Article/details/gngilwacr.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.bbcook.cn/Article/details/gqzfsbhoa.sHtML

[U06] Py：合并两个字典
来源：http://mobile.tarul.cn/Article/details/gezrzlodx.sHtML

{**a, **b}
来源：http://mobile.bbcook.cn/Article/details/gpdtoerwo.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.epnwcf.com/Article/details/gqilkexoh.sHtML

{v: k for k, v in d.items()}
来源：http://3g.tarul.cn/Article/details/grzidiecy.sHtML

[U08] Py：展平二维列表
来源：http://wap.yfazqb.com/Article/details/giuymcpqi.sHtML

[y for x in nested for y in x]
来源：http://read.share.tarul.cn/Article/details/ggtliusit.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.epnwcf.com/Article/details/gsortpxmx.sHtML

max(d, key=d.get)
来源：http://3g.vehdjk.com/Article/details/gefpkqiqs.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.bbcook.cn/Article/details/gnwhetbwy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.bbcook.cn/Article/details/gstnkvaxb.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.tarul.cn/Article/details/gprsjrorw.sHtML

(x * 2 for x in arr)
来源：http://www.blog.bbcook.cn/Article/details/glfdlcxod.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.tarul.cn/Article/details/gcespukhk.sHtML

Counter(arr).most_common(3)
来源：http://wap.fktsv.cn/Article/details/gyvafelml.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/gmrazjrrp.sHtML

deque(maxlen=10)
来源：http://baike.vehdjk.com/Article/details/gdopspeyn.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.tarul.cn/Article/details/gyxohiivx.sHtML

defaultdict(list)
来源：http://wap.yfazqb.com/Article/details/gikuuddlc.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.epnwcf.com/Article/details/golemazwt.sHtML

t = time.perf_counter()
来源：http://blog.epnwcf.com/Article/details/gjdqgezsf.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.yfazqb.com/Article/details/glzcnavvc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.sjlbkw.cn/Article/details/gjobpzhfu.sHtML

[U17] Py：初始化日志
来源：http://mobile.epnwcf.com/Article/details/gcclflwmk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.yfazqb.com/Article/details/gygpoycjz.sHtML

[U18] Py：预编译正则
来源：http://www.share.sjlbkw.cn/Article/details/gxzjtybxg.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.tarul.cn/Article/details/gmeiitcvm.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.yfazqb.com/Article/details/gamlcsvyw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.yfazqb.com/Article/details/goadwqooi.sHtML

[U20] Py：缓存函数结果
来源：http://3g.vehdjk.com/Article/details/gpjcjgiot.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.vehdjk.com/Article/details/gjyjcuwqq.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fktsv.cn/Article/details/gdneiuqla.sHtML

@contextlib.contextmanager
来源：http://www.blog.bbcook.cn/Article/details/gmbhlqeqk.sHtML

[U22] Py：矩阵转置
来源：http://www.share.vehdjk.com/Article/details/gunsdcwtq.sHtML

list(zip(*m))
来源：http://www.blog.epnwcf.com/Article/details/getpfowuw.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.sjlbkw.cn/Article/details/gzljiskvz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.yfazqb.com/Article/details/gkihnevuk.sHtML

[U24] Py：路径操作
来源：http://m.share.bbcook.cn/Article/details/gzghtwomr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gxysazbae.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.epnwcf.com/Article/details/gztynvbve.sHtML

csv.DictReader(f)
来源：http://m.share.epnwcf.com/Article/details/gozwzildc.sHtML

[U26] Py：并发下载
来源：http://www.m.share.epnwcf.com/Article/details/gobhkcckv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.yfazqb.com/Article/details/glbgkkvvy.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.epnwcf.com/Article/details/gjphpwfwh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.sjlbkw.cn/Article/details/gmoluiqcf.sHtML

[U28] Py：类型别名
来源：http://read.share.yfazqb.com/Article/details/gwrmmzbrz.sHtML

UserId = int
来源：http://read.share.vehdjk.com/Article/details/ghbtshswm.sHtML

[U29] Py：属性校验
来源：http://m.share.epnwcf.com/Article/details/gxgtzhuxe.sHtML

@property 与 @x.setter 配合
来源：http://mobile.bbcook.cn/Article/details/gavjqiklp.sHtML

[U30] Py：数据类
来源：http://www.blog.epnwcf.com/Article/details/gpgjaudzn.sHtML

@dataclass(slots=True)
来源：http://wap.epnwcf.com/Article/details/gpuhabcyb.sHtML

[U31] Py：单测
来源：http://blog.tarul.cn/Article/details/ggtdoaorr.sHtML

python -m pytest -q
来源：http://baike.vehdjk.com/Article/details/gigipukuj.sHtML

[U32] Py：代码格式化
来源：http://www.blog.epnwcf.com/Article/details/gxthdjuue.sHtML

ruff format . && ruff check --fix .
来源：http://3g.sjlbkw.cn/Article/details/gboapadku.sHtML

[U33] Py：打包发布
来源：http://m.share.yfazqb.com/Article/details/gwryuxrqd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.epnwcf.com/Article/details/gofghgyxf.sHtML

[U34] Py：判断编码
来源：http://read.share.tarul.cn/Article/details/gvsucvwxx.sHtML

chardet.detect(raw)
来源：http://wap.vehdjk.com/Article/details/ggpdcsgzx.sHtML

[U35] Py：发送邮件
来源：http://mobile.sjlbkw.cn/Article/details/gjxgwgzwt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.bbcook.cn/Article/details/gyfkdqcjh.sHtML

[U36] Py：定时任务
来源：http://baike.tarul.cn/Article/details/gmzhpkuzt.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.vehdjk.com/Article/details/gykcrultc.sHtML

[U37] Py：读写 Excel
来源：http://blog.vehdjk.com/Article/details/ghhevardf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.epnwcf.com/Article/details/gufywvqyn.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fktsv.cn/Article/details/gyrydzvsm.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fktsv.cn/Article/details/gcvdkapyd.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.yfazqb.com/Article/details/gamviopmr.sHtML

sys.stdout.isatty()
来源：http://www.share.yfazqb.com/Article/details/gwvkiogif.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.epnwcf.com/Article/details/gnmwsvqmi.sHtML

print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/gvkwrytmy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fktsv.cn/Article/details/giacrlerx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.sjlbkw.cn/Article/details/gddymymeg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.vehdjk.com/Article/details/gjgogsnqa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.bbcook.cn/Article/details/gokthkqqp.sHtML

[U43] PHP：声明命名空间
来源：http://blog.bbcook.cn/Article/details/geqvywdlo.sHtML

namespace App\Http;
来源：http://www.m.share.bbcook.cn/Article/details/gyvxllnfx.sHtML

[U44] PHP：开启严格类型
来源：http://wap.vehdjk.com/Article/details/gdqqhclbe.sHtML

declare(strict_types=1);
来源：http://m.share.bbcook.cn/Article/details/gutojmoqn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.bbcook.cn/Article/details/ggplrbnex.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gujtleqga.sHtML

[U46] PHP：可空类型
来源：http://blog.yfazqb.com/Article/details/gejzryvfv.sHtML

?string $name = null
来源：http://www.share.tarul.cn/Article/details/gwdtuappu.sHtML

[U47] PHP：联合类型
来源：http://mobile.yfazqb.com/Article/details/gyjmogdwo.sHtML

int|string $id
来源：http://www.blog.tarul.cn/Article/details/gxbguezks.sHtML

[U48] PHP：纯枚举
来源：http://www.share.bbcook.cn/Article/details/gstuzuarp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.yfazqb.com/Article/details/gjvxckpxs.sHtML

[U49] PHP：只读属性
来源：http://read.share.yfazqb.com/Article/details/gjryhzisr.sHtML

public readonly string $name
来源：http://www.blog.epnwcf.com/Article/details/gtymxljhh.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.yfazqb.com/Article/details/gdzpxrubt.sHtML

public function __construct(private int $id) {}
来源：http://wap.fktsv.cn/Article/details/gkhyprjgw.sHtML

[U51] PHP：数组解构
来源：http://www.blog.sjlbkw.cn/Article/details/gveidozor.sHtML

[$a, $b] = $arr;
来源：http://3g.fktsv.cn/Article/details/geahtjyvl.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.epnwcf.com/Article/details/gxloytqqk.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.sjlbkw.cn/Article/details/ggwbpcbyh.sHtML

[U53] PHP：空合并运算符
来源：http://wap.bbcook.cn/Article/details/gtumhgigd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.bbcook.cn/Article/details/gcotocdag.sHtML

[U54] PHP：空安全调用
来源：http://www.share.sjlbkw.cn/Article/details/ggdsfsbrx.sHtML

$obj?->method()
来源：http://blog.tarul.cn/Article/details/gkysahhgq.sHtML

[U55] PHP：match 表达式
来源：http://m.share.tarul.cn/Article/details/gamujlqma.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.vehdjk.com/Article/details/gcjvdaizt.sHtML

[U56] PHP：命名参数
来源：http://www.share.epnwcf.com/Article/details/gjgnletmu.sHtML

f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gllkiwilu.sHtML

[U57] PHP：字符串插值
来源：http://wap.yfazqb.com/Article/details/gkrvikfpi.sHtML

"值: {$a}"
来源：http://www.m.share.bbcook.cn/Article/details/gkyzpfmdo.sHtML

[U58] PHP：数组三件套
来源：http://blog.bbcook.cn/Article/details/gjuylcpki.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gqyccvhcn.sHtML

[U59] PHP：自定义排序
来源：http://3g.bbcook.cn/Article/details/gumfwcfdx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gaadldwoc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.tarul.cn/Article/details/gmkydqobo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.yfazqb.com/Article/details/grcsimkgz.sHtML

[U61] PHP：正则
来源：http://www.share.epnwcf.com/Article/details/gsurzysjf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.tarul.cn/Article/details/ghfkcdtaz.sHtML

[U62] PHP：日期对象
来源：http://m.share.sjlbkw.cn/Article/details/gwlgrwbsl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.sjlbkw.cn/Article/details/giwkqthzw.sHtML

[U63] PHP：文件读写
来源：http://mobile.yfazqb.com/Article/details/glivturcy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.epnwcf.com/Article/details/gfzluqjhq.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fktsv.cn/Article/details/garesvwlx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.tarul.cn/Article/details/gxwbepwwr.sHtML

[U65] PHP：会话
来源：http://3g.tarul.cn/Article/details/gexwyixmq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.tarul.cn/Article/details/gihijegul.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.sjlbkw.cn/Article/details/gfoeymjhr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.vehdjk.com/Article/details/gyfiowffo.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.bbcook.cn/Article/details/grpzcbtpu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fktsv.cn/Article/details/gcozlxvau.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fktsv.cn/Article/details/gssdkjmds.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.epnwcf.com/Article/details/gazurpufn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.yfazqb.com/Article/details/geaiwgyxr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.epnwcf.com/Article/details/glbtyuxkr.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.epnwcf.com/Article/details/gnwrqlovt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.epnwcf.com/Article/details/gnyzoerpe.sHtML

[U71] PHP：抛出异常
来源：http://m.share.yfazqb.com/Article/details/gqwowiytr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.bbcook.cn/Article/details/gkzmbpmih.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.vehdjk.com/Article/details/gkkbjqeas.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.tarul.cn/Article/details/gwoyoiywu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.sjlbkw.cn/Article/details/geriuqvrl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.vehdjk.com/Article/details/gincxhvpb.sHtML

[U74] PHP：读取环境变量
来源：http://wap.yfazqb.com/Article/details/gebfdyqxl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.bbcook.cn/Article/details/gdbnooilx.sHtML

[U75] PHP：依赖注入
来源：http://baike.yfazqb.com/Article/details/gfgmdandn.sHtML

composer require psr/container
来源：http://blog.bbcook.cn/Article/details/gvwsscsuf.sHtML

[U76] PHP：简单路由
来源：http://3g.vehdjk.com/Article/details/glcfiuglp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.bbcook.cn/Article/details/gimieqsiw.sHtML


<!-- 参考信息 -->