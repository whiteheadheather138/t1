代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.sjlbkw.cn/Article/details/grplmceio.sHtML

[S57] C++：编译期常量
来源：http://wap.yfazqb.com/Article/details/gnjlatxlh.sHtML

constexpr int N = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gdknshlia.sHtML

[S58] C++：命名空间
来源：http://read.share.bbcook.cn/Article/details/grgxaheeu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.epnwcf.com/Article/details/gopidrprr.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/gegwejtaj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.sjlbkw.cn/Article/details/gyviilvpj.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.sjlbkw.cn/Article/details/gqpcljofq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gxnflzcbe.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggpdtxbnb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.epnwcf.com/Article/details/gebicwzdr.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbivznebo.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gbgdwwblc.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gqjvfotav.sHtML

[T02] Kotlin：变量
来源：http://blog.vehdjk.com/Article/details/gnldgvcby.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.bbcook.cn/Article/details/goxbyfoqz.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.vehdjk.com/Article/details/gwrpsercu.sHtML

"值: $b"
来源：http://blog.tarul.cn/Article/details/gufpasiql.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.yfazqb.com/Article/details/gofnphtvd.sHtML

val n: String? = null;  n?.length
来源：http://m.share.vehdjk.com/Article/details/gmbbeznga.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fktsv.cn/Article/details/grfaupmqy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.vehdjk.com/Article/details/gyalpzrqs.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.vehdjk.com/Article/details/gbjgrmtug.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.yfazqb.com/Article/details/gmgswlzil.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.yfazqb.com/Article/details/gafinxqyc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/grvvhkjmf.sHtML

[T08] Kotlin：数据类
来源：http://3g.tarul.cn/Article/details/gjulldcan.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.yfazqb.com/Article/details/gmzcuokqa.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.epnwcf.com/Article/details/gflhjwlnj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.tarul.cn/Article/details/gdiuwmnkb.sHtML

[T10] Kotlin：默认参数
来源：http://wap.tarul.cn/Article/details/goqlcvoue.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.tarul.cn/Article/details/ggzngmfkf.sHtML

[T11] Kotlin：协程
来源：http://www.blog.bbcook.cn/Article/details/gwaandlki.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.yfazqb.com/Article/details/gysyphghq.sHtML

[T12] Kotlin：解构声明
来源：http://wap.sjlbkw.cn/Article/details/gubhzfluc.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gdufjzfsn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.vehdjk.com/Article/details/gsibronzs.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.epnwcf.com/Article/details/gsyypwjgb.sHtML

[T14] Kotlin：循环
来源：http://mobile.fktsv.cn/Article/details/givalxjfd.sHtML

for (i in 1..10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gyitclxhm.sHtML

[T15] Kotlin：接口
来源：http://read.share.vehdjk.com/Article/details/gosyaidiw.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/gtraahrnc.sHtML

[T16] Swift：Hello World
来源：http://mobile.tarul.cn/Article/details/glqetcgvf.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gnzujdwmk.sHtML

[T17] Swift：变量与常量
来源：http://mobile.tarul.cn/Article/details/gkvxypurs.sHtML

var a = 1;  let b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gtysdmgpg.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gpfwjgyff.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gaxsvymce.sHtML

[T19] Swift：可选绑定
来源：http://m.share.sjlbkw.cn/Article/details/gbgjxgizw.sHtML

if let n = opt { print(n) }
来源：http://blog.bbcook.cn/Article/details/gbfrbpylh.sHtML

[T20] Swift：数组操作
来源：http://mobile.sjlbkw.cn/Article/details/gnxbaxfln.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.yfazqb.com/Article/details/gyekluetv.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fktsv.cn/Article/details/gsrlzziej.sHtML

for x in a { print(x) }
来源：http://www.blog.epnwcf.com/Article/details/gztijlkpi.sHtML

[T22] Swift：字典
来源：http://3g.epnwcf.com/Article/details/garisbwcg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.vehdjk.com/Article/details/gcagjwjze.sHtML

[T23] Swift：函数
来源：http://mobile.sjlbkw.cn/Article/details/ggsrmqpsb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fktsv.cn/Article/details/gbjxedmma.sHtML

[T24] Swift：闭包
来源：http://wap.bbcook.cn/Article/details/gevxmomxs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fktsv.cn/Article/details/glravkbrl.sHtML

[T25] Swift：结构体
来源：http://m.share.bbcook.cn/Article/details/gdaynaudl.sHtML

struct P { var x: Int }
来源：http://blog.sjlbkw.cn/Article/details/gmovjnifz.sHtML

[T26] Swift：类与重写
来源：http://blog.epnwcf.com/Article/details/ggnqxkfen.sHtML

class A: Base { override func f() {} }
来源：http://baike.fktsv.cn/Article/details/gvtbjsoco.sHtML

[T27] Swift：错误处理
来源：http://blog.tarul.cn/Article/details/ggmykrpbs.sHtML

do { try f() } catch { print(error) }
来源：http://blog.tarul.cn/Article/details/gcwalqlyk.sHtML

[T28] Swift：枚举
来源：http://read.share.yfazqb.com/Article/details/gjxekrfzx.sHtML

enum Color { case red, green }
来源：http://read.share.sjlbkw.cn/Article/details/gdotuiwlj.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.yfazqb.com/Article/details/gvirpjkyr.sHtML

guard let x = opt else { return }
来源：http://baike.vehdjk.com/Article/details/ggzpkxkxn.sHtML

[T30] Swift：协议
来源：http://read.share.vehdjk.com/Article/details/gaietiqko.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.epnwcf.com/Article/details/gkwpkdwlx.sHtML

[T31] Lua：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gbkynzflr.sHtML

print("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gbksykcfh.sHtML

[T32] Lua：局部变量
来源：http://m.share.yfazqb.com/Article/details/gqbltimyv.sHtML

local a = 1
来源：http://blog.vehdjk.com/Article/details/gixpjzrze.sHtML

[T33] Lua：表（数组）
来源：http://www.share.sjlbkw.cn/Article/details/gdbrwycry.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.epnwcf.com/Article/details/gnunpfobs.sHtML

[T34] Lua：遍历表
来源：http://baike.sjlbkw.cn/Article/details/gzuyhvdpy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.vehdjk.com/Article/details/ghwcqqbfz.sHtML

[T35] Lua：字典表
来源：http://3g.fktsv.cn/Article/details/gzpbrshfq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.vehdjk.com/Article/details/gwjbhyumm.sHtML

[T36] Lua：函数
来源：http://wap.bbcook.cn/Article/details/ggtcsdoji.sHtML

function add(a, b) return a + b end
来源：http://m.share.bbcook.cn/Article/details/gxwvsvhkq.sHtML

[T37] Lua：字符串拼接
来源：http://3g.epnwcf.com/Article/details/gzlvjnunx.sHtML

"a" .. "b"
来源：http://3g.sjlbkw.cn/Article/details/gseswdwho.sHtML

[T38] Lua：条件
来源：http://baike.vehdjk.com/Article/details/gsmoumzgu.sHtML

if x > 0 then print("正") end
来源：http://blog.vehdjk.com/Article/details/gruucziyl.sHtML

[T39] Lua：模式匹配
来源：http://mobile.epnwcf.com/Article/details/gwnnknixk.sHtML

string.find(s, "%d+")
来源：http://www.share.bbcook.cn/Article/details/gqbutrpyf.sHtML

[T40] Lua：元表
来源：http://www.share.bbcook.cn/Article/details/gsondzdnz.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.epnwcf.com/Article/details/gxviotkra.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gakuuuytd.sHtML

print "Hello\n";
来源：http://read.share.epnwcf.com/Article/details/grbduvewu.sHtML

[T42] Perl：变量类型
来源：http://baike.epnwcf.com/Article/details/grwhrazpp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.vehdjk.com/Article/details/gynxjwyfa.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/ghggyqrmf.sHtML

"值: $a"
来源：http://3g.yfazqb.com/Article/details/gxyklsiau.sHtML

[T44] Perl：条件
来源：http://blog.sjlbkw.cn/Article/details/gyapthima.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.bbcook.cn/Article/details/gckzexlfj.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.vehdjk.com/Article/details/ggktvydwu.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.bbcook.cn/Article/details/gqqsjssti.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.epnwcf.com/Article/details/gflvgbnky.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.epnwcf.com/Article/details/gaippnlcc.sHtML

[T47] Perl：正则捕获
来源：http://baike.yfazqb.com/Article/details/gyqzogckj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.epnwcf.com/Article/details/gkviaphrt.sHtML

[T48] Perl：正则替换
来源：http://baike.epnwcf.com/Article/details/gtpwcjjcp.sHtML

$s =~ s/old/new/g;
来源：http://mobile.sjlbkw.cn/Article/details/ghqoohgwt.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/gjinswald.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gmnnkkgba.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gdbikgfnq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggquyfawx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.yfazqb.com/Article/details/gyggnmcbf.sHtML

[T51] Scala：Hello World
来源：http://mobile.fktsv.cn/Article/details/ggjwhqhjs.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gyvbddwdp.sHtML

[T52] Scala：变量
来源：http://3g.epnwcf.com/Article/details/gaschydci.sHtML

val a = 1;  var b = 2
来源：http://baike.tarul.cn/Article/details/gglyopovo.sHtML

[T53] Scala：字符串插值
来源：http://blog.tarul.cn/Article/details/gffsofbsw.sHtML

s"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gtwnhwkty.sHtML

[T54] Scala：集合映射
来源：http://www.blog.tarul.cn/Article/details/glozccqpg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.tarul.cn/Article/details/gjvgqlago.sHtML

[T55] Scala：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gmcbszcvu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.sjlbkw.cn/Article/details/gvxqniyst.sHtML

[T56] Scala：样例类
来源：http://mobile.yfazqb.com/Article/details/gsuvqdult.sHtML

case class User(name: String, age: Int)
来源：http://wap.yfazqb.com/Article/details/gzsvgwrqs.sHtML

[T57] Scala：模式匹配
来源：http://wap.yfazqb.com/Article/details/ghjccokcf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fktsv.cn/Article/details/gbcydpaav.sHtML

[T58] Scala：函数定义
来源：http://www.share.fktsv.cn/Article/details/gccxilwkc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.epnwcf.com/Article/details/ghniyqoww.sHtML

[T59] Scala：循环
来源：http://blog.sjlbkw.cn/Article/details/gfzmldvvq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.tarul.cn/Article/details/gttgrxfjj.sHtML

[T60] Scala：折叠
来源：http://read.share.yfazqb.com/Article/details/gyugpnzpd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/gxmdjhnwv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/genbjqkjh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.tarul.cn/Article/details/ghhdajtpp.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzfuolizl.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fktsv.cn/Article/details/gqiwzghpo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.sjlbkw.cn/Article/details/gseisbefr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.vehdjk.com/Article/details/gtfgxkneu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.epnwcf.com/Article/details/gnhuxxvbn.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.bbcook.cn/Article/details/gsknjvupw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.epnwcf.com/Article/details/gvmebfwsh.sHtML

[U04] Py：变量调试打印
来源：http://m.share.sjlbkw.cn/Article/details/guwiprgio.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.bbcook.cn/Article/details/gjmhtjwme.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.epnwcf.com/Article/details/gfbrvuoau.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gvlqtllbg.sHtML

[U06] Py：合并两个字典
来源：http://baike.vehdjk.com/Article/details/gemjrurrl.sHtML

{**a, **b}
来源：http://www.m.share.fktsv.cn/Article/details/giclcakgl.sHtML

[U07] Py：反转字典键值
来源：http://3g.vehdjk.com/Article/details/gsvsthgka.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gfwlcjwkd.sHtML

[U08] Py：展平二维列表
来源：http://www.share.bbcook.cn/Article/details/gpoiduuhn.sHtML

[y for x in nested for y in x]
来源：http://m.share.epnwcf.com/Article/details/gaeritdpa.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.vehdjk.com/Article/details/govjlfzyl.sHtML

max(d, key=d.get)
来源：http://baike.bbcook.cn/Article/details/gxddwkmho.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.tarul.cn/Article/details/gnfuprlwb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.bbcook.cn/Article/details/gaedaplru.sHtML

[U11] Py：生成器表达式
来源：http://blog.epnwcf.com/Article/details/gcalnhdol.sHtML

(x * 2 for x in arr)
来源：http://mobile.epnwcf.com/Article/details/ghnowaabl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.epnwcf.com/Article/details/gduijjbsk.sHtML

Counter(arr).most_common(3)
来源：http://m.share.sjlbkw.cn/Article/details/greuxxzjk.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/gafftretn.sHtML

deque(maxlen=10)
来源：http://m.share.vehdjk.com/Article/details/gowbdshae.sHtML

[U14] Py：分组收集到列表
来源：http://3g.yfazqb.com/Article/details/gjlqmyqaz.sHtML

defaultdict(list)
来源：http://wap.epnwcf.com/Article/details/gjxqblcgl.sHtML

[U15] Py：高精度计时
来源：http://www.blog.vehdjk.com/Article/details/gqxjsrqhp.sHtML

t = time.perf_counter()
来源：http://www.blog.tarul.cn/Article/details/gzmricpnl.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.tarul.cn/Article/details/gwiicvhjj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.sjlbkw.cn/Article/details/gxypavjxn.sHtML

[U17] Py：初始化日志
来源：http://read.share.fktsv.cn/Article/details/gynfxylkd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.tarul.cn/Article/details/grozyvysi.sHtML

[U18] Py：预编译正则
来源：http://read.share.fktsv.cn/Article/details/gfzmouaxx.sHtML

pat = re.compile(r"\d+")
来源：http://blog.vehdjk.com/Article/details/guvrtvehx.sHtML

[U19] Py：正则替换带回调
来源：http://wap.bbcook.cn/Article/details/gvmyaghib.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.vehdjk.com/Article/details/gkvljfyau.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.bbcook.cn/Article/details/gciaxjzuz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.sjlbkw.cn/Article/details/ghbbhqtwt.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.sjlbkw.cn/Article/details/gihzcsyww.sHtML

@contextlib.contextmanager
来源：http://www.blog.vehdjk.com/Article/details/gqslymtvj.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fktsv.cn/Article/details/gkcabwusd.sHtML

list(zip(*m))
来源：http://blog.tarul.cn/Article/details/ggobrjsda.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fktsv.cn/Article/details/gwutgzwvg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.epnwcf.com/Article/details/gkwsvokmu.sHtML

[U24] Py：路径操作
来源：http://baike.bbcook.cn/Article/details/gawrqjliy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gfmfmtbst.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.vehdjk.com/Article/details/gjzarpxba.sHtML

csv.DictReader(f)
来源：http://wap.sjlbkw.cn/Article/details/gilofzpdh.sHtML

[U26] Py：并发下载
来源：http://www.blog.sjlbkw.cn/Article/details/guwxyvalt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.sjlbkw.cn/Article/details/gexrxbjoi.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.sjlbkw.cn/Article/details/gtcpxcnti.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.tarul.cn/Article/details/golgzxrom.sHtML

[U28] Py：类型别名
来源：http://www.m.share.vehdjk.com/Article/details/gisqdvuli.sHtML

UserId = int
来源：http://3g.bbcook.cn/Article/details/gzmuyppcr.sHtML

[U29] Py：属性校验
来源：http://read.share.sjlbkw.cn/Article/details/gnvhopkax.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.vehdjk.com/Article/details/gogkounjv.sHtML

[U30] Py：数据类
来源：http://baike.fktsv.cn/Article/details/gcqizevzi.sHtML

@dataclass(slots=True)
来源：http://baike.fktsv.cn/Article/details/gugnvowcr.sHtML

[U31] Py：单测
来源：http://mobile.fktsv.cn/Article/details/gvkfkxcxx.sHtML

python -m pytest -q
来源：http://3g.vehdjk.com/Article/details/gnstuwugd.sHtML

[U32] Py：代码格式化
来源：http://www.share.bbcook.cn/Article/details/gxxyyojao.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.epnwcf.com/Article/details/gzabnxkaa.sHtML

[U33] Py：打包发布
来源：http://m.share.fktsv.cn/Article/details/galwvnsnc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.epnwcf.com/Article/details/gvrphwmca.sHtML

[U34] Py：判断编码
来源：http://wap.epnwcf.com/Article/details/gxckfsdch.sHtML

chardet.detect(raw)
来源：http://wap.vehdjk.com/Article/details/gtejbuehr.sHtML

[U35] Py：发送邮件
来源：http://www.share.yfazqb.com/Article/details/gybwzjpsu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.vehdjk.com/Article/details/gwdcobttx.sHtML

[U36] Py：定时任务
来源：http://m.share.bbcook.cn/Article/details/gvmhxnpji.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.tarul.cn/Article/details/gnyxkxmsr.sHtML

[U37] Py：读写 Excel
来源：http://blog.sjlbkw.cn/Article/details/gttbdzjsz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.tarul.cn/Article/details/gwckemiyv.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.vehdjk.com/Article/details/gdltunpnt.sHtML

Path(__file__).resolve().parent
来源：http://3g.yfazqb.com/Article/details/gkfpuvvpp.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fktsv.cn/Article/details/gpiqpvjjh.sHtML

sys.stdout.isatty()
来源：http://m.share.yfazqb.com/Article/details/gapygdpag.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fktsv.cn/Article/details/gmdxldmui.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/gqckcfrme.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.tarul.cn/Article/details/gryceepsv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.tarul.cn/Article/details/geelbkblm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fktsv.cn/Article/details/gynhjccii.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.yfazqb.com/Article/details/gddcaaujz.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.vehdjk.com/Article/details/ghjmnvgyo.sHtML

namespace App\Http;
来源：http://3g.tarul.cn/Article/details/gmocraezx.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.vehdjk.com/Article/details/ghlweaqhg.sHtML

declare(strict_types=1);
来源：http://3g.bbcook.cn/Article/details/gwnsjzrtx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzucqned.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcjeaplzv.sHtML

[U46] PHP：可空类型
来源：http://read.share.bbcook.cn/Article/details/gemvqvlte.sHtML

?string $name = null
来源：http://www.blog.tarul.cn/Article/details/gvoxoizag.sHtML

[U47] PHP：联合类型
来源：http://read.share.yfazqb.com/Article/details/gtbljopsd.sHtML

int|string $id
来源：http://blog.yfazqb.com/Article/details/gtavfrtjt.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.epnwcf.com/Article/details/gztpgitfa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzoqmqrm.sHtML

[U49] PHP：只读属性
来源：http://blog.sjlbkw.cn/Article/details/gfnuhzlzb.sHtML

public readonly string $name
来源：http://wap.fktsv.cn/Article/details/gotktgagf.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.tarul.cn/Article/details/gfbkqteir.sHtML

public function __construct(private int $id) {}
来源：http://blog.sjlbkw.cn/Article/details/gntrcladv.sHtML

[U51] PHP：数组解构
来源：http://www.blog.sjlbkw.cn/Article/details/gvulmlkmr.sHtML

[$a, $b] = $arr;
来源：http://wap.bbcook.cn/Article/details/gwvyinktc.sHtML

[U52] PHP：箭头函数
来源：http://baike.tarul.cn/Article/details/gygtintwv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fktsv.cn/Article/details/gvjcrjnnm.sHtML

[U53] PHP：空合并运算符
来源：http://3g.yfazqb.com/Article/details/gnqheprwb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.bbcook.cn/Article/details/gygkotdte.sHtML

[U54] PHP：空安全调用
来源：http://m.share.bbcook.cn/Article/details/gfekteovn.sHtML

$obj?->method()
来源：http://baike.vehdjk.com/Article/details/gjydtyrgm.sHtML

[U55] PHP：match 表达式
来源：http://3g.tarul.cn/Article/details/ghuvaachx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.vehdjk.com/Article/details/gipcxwslw.sHtML

[U56] PHP：命名参数
来源：http://www.blog.epnwcf.com/Article/details/genohaoqo.sHtML

f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gmpkmcslr.sHtML

[U57] PHP：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gbtvgvqkk.sHtML

"值: {$a}"
来源：http://blog.epnwcf.com/Article/details/glvvtdjoo.sHtML

[U58] PHP：数组三件套
来源：http://www.share.yfazqb.com/Article/details/ghnemxtye.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fktsv.cn/Article/details/gnsfamfeq.sHtML

[U59] PHP：自定义排序
来源：http://blog.vehdjk.com/Article/details/gllgxdxdp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gooahysyp.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.yfazqb.com/Article/details/ggbzonhyf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.yfazqb.com/Article/details/gqtcadwnb.sHtML

[U61] PHP：正则
来源：http://baike.yfazqb.com/Article/details/gtowcqogy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gwhoheema.sHtML

[U62] PHP：日期对象
来源：http://mobile.sjlbkw.cn/Article/details/gzdifyrdj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.bbcook.cn/Article/details/gkuwgiuqj.sHtML

[U63] PHP：文件读写
来源：http://www.share.yfazqb.com/Article/details/glyosndjg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.vehdjk.com/Article/details/gahhuhjkj.sHtML

[U64] PHP：目录遍历
来源：http://read.share.vehdjk.com/Article/details/gslpwkqub.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.sjlbkw.cn/Article/details/gfzlpqxmq.sHtML

[U65] PHP：会话
来源：http://baike.epnwcf.com/Article/details/gwripotzu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fktsv.cn/Article/details/gskiqpkcf.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.yfazqb.com/Article/details/gqcsqedrt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.sjlbkw.cn/Article/details/gtsonifpu.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.epnwcf.com/Article/details/ghbjxdliw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.sjlbkw.cn/Article/details/gfbotgbzy.sHtML

[U68] PHP：PDO 连接
来源：http://wap.bbcook.cn/Article/details/glpwkysqv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.epnwcf.com/Article/details/gnbtnyooc.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.bbcook.cn/Article/details/gioaojijs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.yfazqb.com/Article/details/gxozegkoh.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.epnwcf.com/Article/details/gfnwgqpsy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.vehdjk.com/Article/details/gvgjhsmom.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.epnwcf.com/Article/details/gzkjenqqn.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.vehdjk.com/Article/details/glalyqjyf.sHtML

[U72] PHP：写错误日志
来源：http://www.share.vehdjk.com/Article/details/gnsokembr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.tarul.cn/Article/details/gheloxojs.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.yfazqb.com/Article/details/gejquwyph.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.sjlbkw.cn/Article/details/ggmrwpurd.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gbwpoeljc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fktsv.cn/Article/details/gahjjfkhi.sHtML

[U75] PHP：依赖注入
来源：http://3g.epnwcf.com/Article/details/gmditrnwb.sHtML

composer require psr/container
来源：http://m.share.epnwcf.com/Article/details/gzhehwsxn.sHtML

[U76] PHP：简单路由
来源：http://m.share.yfazqb.com/Article/details/gqvajmgcr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fktsv.cn/Article/details/gdmjbyxxq.sHtML

[U77] PHP：模板渲染
来源：http://read.share.vehdjk.com/Article/details/gtzwiitsj.sHtML

composer require twig/twig
来源：http://baike.yfazqb.com/Article/details/ganpnqzhr.sHtML

[U78] PHP：单元测试
来源：http://www.blog.tarul.cn/Article/details/gbhnbfozd.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.vehdjk.com/Article/details/gomakffzj.sHtML

[U79] PHP：静态分析
来源：http://www.share.yfazqb.com/Article/details/gnivyweip.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.vehdjk.com/Article/details/gyyxtgqiz.sHtML

[U80] PHP：代码规范修复
来源：http://wap.epnwcf.com/Article/details/gsfuktqlr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.vehdjk.com/Article/details/gxgeemmnu.sHtML

[U81] JS：初始化项目
来源：http://m.share.sjlbkw.cn/Article/details/ghbogfxqo.sHtML

npm init -y;  npm i express
来源：http://www.m.share.tarul.cn/Article/details/ggpnanzby.sHtML

[U82] JS：package.json 脚本
来源：http://blog.vehdjk.com/Article/details/gfpcyukms.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.bbcook.cn/Article/details/gamnnlppk.sHtML


<!-- 参考信息 -->