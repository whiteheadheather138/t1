代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/gsgfhovao.sHtML

[S55] C++：结构化绑定
来源：http://wap.epnwcf.com/Article/details/gzhqojfuf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.bbcook.cn/Article/details/gpewxdhrd.sHtML

[S56] C++：optional
来源：http://www.blog.sjlbkw.cn/Article/details/ghozttjfz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/ghtvmiege.sHtML

[S57] C++：编译期常量
来源：http://www.blog.bbcook.cn/Article/details/gzdgzkjin.sHtML

constexpr int N = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gcaveofak.sHtML

[S58] C++：命名空间
来源：http://www.share.epnwcf.com/Article/details/gwjqkeohl.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.tarul.cn/Article/details/gftnscybl.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/gjgopvjah.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fktsv.cn/Article/details/ghvudwskw.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.tarul.cn/Article/details/gtliumhzc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.yfazqb.com/Article/details/grpmzphvu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqsnrxykm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gumrswsgv.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkmqohcuz.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.vehdjk.com/Article/details/grpbreekq.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gvxgtfump.sHtML

[T02] Kotlin：变量
来源：http://baike.bbcook.cn/Article/details/gduldkidy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.yfazqb.com/Article/details/gwxxaseqy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/gofucgwsp.sHtML

"值: $b"
来源：http://baike.tarul.cn/Article/details/goilgxeug.sHtML

[T04] Kotlin：空安全
来源：http://mobile.tarul.cn/Article/details/gkkuoztjl.sHtML

val n: String? = null;  n?.length
来源：http://blog.epnwcf.com/Article/details/gyexkdzbv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fktsv.cn/Article/details/gkadqyopj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.vehdjk.com/Article/details/gxyibbecw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gzlhrpapy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.bbcook.cn/Article/details/gmysvtjda.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.tarul.cn/Article/details/guqsnydvv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.vehdjk.com/Article/details/gankybgsv.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fktsv.cn/Article/details/gyuvfpjlc.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fktsv.cn/Article/details/gcltozwey.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/gdhlmovbf.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.tarul.cn/Article/details/gmzabxmni.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.epnwcf.com/Article/details/glqnirqjz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.bbcook.cn/Article/details/gfoxsvzkw.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/gwyvujwzb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.sjlbkw.cn/Article/details/gdieqtroi.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/gcgquafwr.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gztaohcoa.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/gchcjkyhx.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.sjlbkw.cn/Article/details/gqrnzxwvl.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.tarul.cn/Article/details/glfhsnvop.sHtML

for (i in 1..10) println(i)
来源：http://blog.bbcook.cn/Article/details/gbpjjvfaw.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/gnseegdhc.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.bbcook.cn/Article/details/gskibsjad.sHtML

[T16] Swift：Hello World
来源：http://m.share.fktsv.cn/Article/details/gmzeuufbg.sHtML

print("Hello")
来源：http://blog.bbcook.cn/Article/details/gvoidcqzh.sHtML

[T17] Swift：变量与常量
来源：http://read.share.bbcook.cn/Article/details/gviqvbbss.sHtML

var a = 1;  let b = 2
来源：http://read.share.vehdjk.com/Article/details/gvibsnqzf.sHtML

[T18] Swift：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/goyhgzcgi.sHtML

"值: \(b)"
来源：http://mobile.fktsv.cn/Article/details/girkzkaks.sHtML

[T19] Swift：可选绑定
来源：http://mobile.vehdjk.com/Article/details/gegejgnjw.sHtML

if let n = opt { print(n) }
来源：http://mobile.epnwcf.com/Article/details/glpkblatq.sHtML

[T20] Swift：数组操作
来源：http://wap.vehdjk.com/Article/details/gfzkkcpqh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.tarul.cn/Article/details/gwnicxpla.sHtML

[T21] Swift：遍历
来源：http://www.m.share.tarul.cn/Article/details/gkdkpsyup.sHtML

for x in a { print(x) }
来源：http://www.share.yfazqb.com/Article/details/gchqqlsls.sHtML

[T22] Swift：字典
来源：http://3g.fktsv.cn/Article/details/gcbdofsvv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fktsv.cn/Article/details/gmisdkhvy.sHtML

[T23] Swift：函数
来源：http://www.blog.yfazqb.com/Article/details/gyfqovogs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.vehdjk.com/Article/details/guebvqtjs.sHtML

[T24] Swift：闭包
来源：http://3g.yfazqb.com/Article/details/gnwdzbbyz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.tarul.cn/Article/details/gprzppkqu.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/gjkadlfwd.sHtML

struct P { var x: Int }
来源：http://wap.tarul.cn/Article/details/gnhlumvzf.sHtML

[T26] Swift：类与重写
来源：http://3g.sjlbkw.cn/Article/details/gmadudqla.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.yfazqb.com/Article/details/gwovmzozi.sHtML

[T27] Swift：错误处理
来源：http://baike.tarul.cn/Article/details/gikeyqfbo.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fktsv.cn/Article/details/grxjmuivr.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/gaccbspkv.sHtML

enum Color { case red, green }
来源：http://www.blog.epnwcf.com/Article/details/gerwuvqsj.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fktsv.cn/Article/details/gsyrrhtmg.sHtML

guard let x = opt else { return }
来源：http://baike.sjlbkw.cn/Article/details/gtvwmhwfg.sHtML

[T30] Swift：协议
来源：http://3g.yfazqb.com/Article/details/gyxgbvwky.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fktsv.cn/Article/details/gxgiculoo.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gbnzbggvj.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gvlhwfxba.sHtML

[T32] Lua：局部变量
来源：http://wap.epnwcf.com/Article/details/gyeqguieg.sHtML

local a = 1
来源：http://www.blog.vehdjk.com/Article/details/gwftptvhz.sHtML

[T33] Lua：表（数组）
来源：http://www.share.tarul.cn/Article/details/gqzfvuxse.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.sjlbkw.cn/Article/details/gyzmgzhal.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.bbcook.cn/Article/details/gmejxdpvx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.yfazqb.com/Article/details/gorgphauz.sHtML

[T35] Lua：字典表
来源：http://read.share.bbcook.cn/Article/details/ghqlcviar.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.bbcook.cn/Article/details/gwtcgcitv.sHtML

[T36] Lua：函数
来源：http://wap.yfazqb.com/Article/details/gzaencjwm.sHtML

function add(a, b) return a + b end
来源：http://wap.vehdjk.com/Article/details/gshomokzg.sHtML

[T37] Lua：字符串拼接
来源：http://wap.vehdjk.com/Article/details/gwddmkbrd.sHtML

"a" .. "b"
来源：http://3g.bbcook.cn/Article/details/gnvzgwceu.sHtML

[T38] Lua：条件
来源：http://www.blog.yfazqb.com/Article/details/gmnhgtlgl.sHtML

if x > 0 then print("正") end
来源：http://baike.epnwcf.com/Article/details/ghwgysvwz.sHtML

[T39] Lua：模式匹配
来源：http://mobile.tarul.cn/Article/details/gilsdalvc.sHtML

string.find(s, "%d+")
来源：http://blog.epnwcf.com/Article/details/gxwtlwpwv.sHtML

[T40] Lua：元表
来源：http://baike.yfazqb.com/Article/details/gilproqua.sHtML

setmetatable({}, { __index = base })
来源：http://blog.bbcook.cn/Article/details/gdaupagfs.sHtML

[T41] Perl：Hello World
来源：http://read.share.vehdjk.com/Article/details/gilwmayzz.sHtML

print "Hello\n";
来源：http://read.share.yfazqb.com/Article/details/gntrnxxrt.sHtML

[T42] Perl：变量类型
来源：http://mobile.vehdjk.com/Article/details/ghykxtfpr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fktsv.cn/Article/details/gajnatwuu.sHtML

[T43] Perl：字符串插值
来源：http://read.share.tarul.cn/Article/details/gtaieboqa.sHtML

"值: $a"
来源：http://m.share.sjlbkw.cn/Article/details/gplbjfonu.sHtML

[T44] Perl：条件
来源：http://baike.fktsv.cn/Article/details/gccgenzfz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.yfazqb.com/Article/details/glmwwzsbh.sHtML

[T45] Perl：数组遍历
来源：http://wap.tarul.cn/Article/details/gopxiualy.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.yfazqb.com/Article/details/ghgxznagn.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fktsv.cn/Article/details/gykcskcgi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.tarul.cn/Article/details/gitpxkwry.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.vehdjk.com/Article/details/gblskqznb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.sjlbkw.cn/Article/details/glzgcfndf.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.bbcook.cn/Article/details/gwganhpyp.sHtML

$s =~ s/old/new/g;
来源：http://m.share.yfazqb.com/Article/details/guyqunkve.sHtML

[T49] Perl：函数
来源：http://www.blog.epnwcf.com/Article/details/gfksmlkbx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/goskhdovb.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/glegbpmgm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.yfazqb.com/Article/details/gqbgwtgbe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.bbcook.cn/Article/details/gakuvmyhk.sHtML

[T51] Scala：Hello World
来源：http://wap.bbcook.cn/Article/details/gjrikgugw.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/ghihycyhl.sHtML

[T52] Scala：变量
来源：http://m.share.fktsv.cn/Article/details/gsgvjajbw.sHtML

val a = 1;  var b = 2
来源：http://3g.bbcook.cn/Article/details/gsisiofzv.sHtML

[T53] Scala：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gvgzqdnmg.sHtML

s"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gadglwoqu.sHtML

[T54] Scala：集合映射
来源：http://read.share.vehdjk.com/Article/details/gceghrqpe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fktsv.cn/Article/details/grrprslwt.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/gwhpxyurb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.sjlbkw.cn/Article/details/grtcwaqnn.sHtML

[T56] Scala：样例类
来源：http://www.m.share.vehdjk.com/Article/details/ggfwzadea.sHtML

case class User(name: String, age: Int)
来源：http://baike.vehdjk.com/Article/details/gpjrugmav.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbhhnbwq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.sjlbkw.cn/Article/details/gisokdxom.sHtML

[T58] Scala：函数定义
来源：http://wap.bbcook.cn/Article/details/gmviebpea.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.sjlbkw.cn/Article/details/gprfypsrt.sHtML

[T59] Scala：循环
来源：http://3g.yfazqb.com/Article/details/gxirgskmo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.vehdjk.com/Article/details/gacfzqchq.sHtML

[T60] Scala：折叠
来源：http://wap.epnwcf.com/Article/details/gnmbsimqs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.vehdjk.com/Article/details/glzfoptdw.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnergrgy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/gvgyosjfl.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gufmpptno.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.vehdjk.com/Article/details/ggcqdsfnz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.sjlbkw.cn/Article/details/gujopmxpu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.sjlbkw.cn/Article/details/gnvzqhrnk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.tarul.cn/Article/details/ghrjmhzms.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.epnwcf.com/Article/details/ghhknydat.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.bbcook.cn/Article/details/gaafjwset.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/gfowyjsuj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fktsv.cn/Article/details/gqxmfqsro.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fktsv.cn/Article/details/gbgtvzlxy.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gkqaiuejt.sHtML

[U06] Py：合并两个字典
来源：http://m.share.bbcook.cn/Article/details/gtxwrlsdp.sHtML

{**a, **b}
来源：http://3g.vehdjk.com/Article/details/gtzemfjqo.sHtML

[U07] Py：反转字典键值
来源：http://www.share.yfazqb.com/Article/details/giwqbphgz.sHtML

{v: k for k, v in d.items()}
来源：http://blog.yfazqb.com/Article/details/gnuqecbbe.sHtML

[U08] Py：展平二维列表
来源：http://3g.tarul.cn/Article/details/glkenqgpd.sHtML

[y for x in nested for y in x]
来源：http://read.share.vehdjk.com/Article/details/giedywpua.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fktsv.cn/Article/details/graokjsog.sHtML

max(d, key=d.get)
来源：http://www.share.sjlbkw.cn/Article/details/gjcfkqdtn.sHtML

[U10] Py：按值排序字典
来源：http://3g.bbcook.cn/Article/details/grfsnhkmi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.epnwcf.com/Article/details/gvromgwrl.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.epnwcf.com/Article/details/ggqnxjbiq.sHtML

(x * 2 for x in arr)
来源：http://read.share.yfazqb.com/Article/details/gtjozesau.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fktsv.cn/Article/details/gsmvjchao.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gesuokdyd.sHtML

[U13] Py：固定长度队列
来源：http://m.share.vehdjk.com/Article/details/gcmtrlujw.sHtML

deque(maxlen=10)
来源：http://m.share.bbcook.cn/Article/details/glyefenmu.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.bbcook.cn/Article/details/gdmgzxtyz.sHtML

defaultdict(list)
来源：http://m.share.bbcook.cn/Article/details/gdhkmjiog.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fktsv.cn/Article/details/ggjkvktki.sHtML

t = time.perf_counter()
来源：http://www.m.share.epnwcf.com/Article/details/gmlstfhmb.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.tarul.cn/Article/details/gzxmlxtpy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.sjlbkw.cn/Article/details/gponetjnl.sHtML

[U17] Py：初始化日志
来源：http://wap.vehdjk.com/Article/details/guwwdphcr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.bbcook.cn/Article/details/gyzsdellh.sHtML

[U18] Py：预编译正则
来源：http://www.blog.yfazqb.com/Article/details/gdniymwwc.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.bbcook.cn/Article/details/gxetzcvtk.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.tarul.cn/Article/details/gtugtxocv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.vehdjk.com/Article/details/gijnrzjyb.sHtML

[U20] Py：缓存函数结果
来源：http://3g.vehdjk.com/Article/details/gbvhlpnyl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.epnwcf.com/Article/details/girqrmovi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.yfazqb.com/Article/details/gpdsaytza.sHtML

@contextlib.contextmanager
来源：http://m.share.epnwcf.com/Article/details/gyxfxchbn.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.yfazqb.com/Article/details/gtafpiuwj.sHtML

list(zip(*m))
来源：http://3g.bbcook.cn/Article/details/gpvfypozy.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.vehdjk.com/Article/details/ggknudkvl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.vehdjk.com/Article/details/gacplxape.sHtML

[U24] Py：路径操作
来源：http://read.share.yfazqb.com/Article/details/gccxcnvsa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.tarul.cn/Article/details/gkwghyxcj.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.sjlbkw.cn/Article/details/ggzgeyvxw.sHtML

csv.DictReader(f)
来源：http://www.share.yfazqb.com/Article/details/gglehcssa.sHtML

[U26] Py：并发下载
来源：http://mobile.bbcook.cn/Article/details/gabskdhaw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.yfazqb.com/Article/details/gqjydpnpv.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.tarul.cn/Article/details/gjuwsllee.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.yfazqb.com/Article/details/gogzwkgki.sHtML

[U28] Py：类型别名
来源：http://m.share.bbcook.cn/Article/details/gskiuhoul.sHtML

UserId = int
来源：http://www.blog.bbcook.cn/Article/details/groeemsnp.sHtML

[U29] Py：属性校验
来源：http://m.share.sjlbkw.cn/Article/details/guvrqoxpe.sHtML

@property 与 @x.setter 配合
来源：http://m.share.bbcook.cn/Article/details/gkutqmecr.sHtML

[U30] Py：数据类
来源：http://wap.fktsv.cn/Article/details/getjcyqys.sHtML

@dataclass(slots=True)
来源：http://www.share.sjlbkw.cn/Article/details/gwjifngrx.sHtML

[U31] Py：单测
来源：http://www.share.sjlbkw.cn/Article/details/gdzdkwtos.sHtML

python -m pytest -q
来源：http://wap.yfazqb.com/Article/details/gluawvqfm.sHtML

[U32] Py：代码格式化
来源：http://blog.epnwcf.com/Article/details/gvuugzapg.sHtML

ruff format . && ruff check --fix .
来源：http://blog.tarul.cn/Article/details/gtyyafens.sHtML

[U33] Py：打包发布
来源：http://www.blog.bbcook.cn/Article/details/gdrndxnby.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.epnwcf.com/Article/details/glifdcrpy.sHtML

[U34] Py：判断编码
来源：http://m.share.sjlbkw.cn/Article/details/ggqqmkwbv.sHtML

chardet.detect(raw)
来源：http://www.blog.tarul.cn/Article/details/gykizepql.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.tarul.cn/Article/details/gykaxltei.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.yfazqb.com/Article/details/gjbwnmyvo.sHtML

[U36] Py：定时任务
来源：http://www.share.epnwcf.com/Article/details/gnvngmmme.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.sjlbkw.cn/Article/details/gsonkvgko.sHtML

[U37] Py：读写 Excel
来源：http://www.share.epnwcf.com/Article/details/gqrotwiol.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fktsv.cn/Article/details/gohlahcjj.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.sjlbkw.cn/Article/details/gvucecnie.sHtML

Path(__file__).resolve().parent
来源：http://mobile.yfazqb.com/Article/details/gnrwldfvz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.tarul.cn/Article/details/gwpffkgtt.sHtML

sys.stdout.isatty()
来源：http://baike.bbcook.cn/Article/details/gocgviuup.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.bbcook.cn/Article/details/gnuptnbeo.sHtML

print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gyenmgccs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.sjlbkw.cn/Article/details/gycdukoqh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.tarul.cn/Article/details/gwktedngu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.vehdjk.com/Article/details/gaydwicnc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.sjlbkw.cn/Article/details/gamvkxbsy.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.vehdjk.com/Article/details/gznkeipkv.sHtML

namespace App\Http;
来源：http://www.m.share.epnwcf.com/Article/details/giviqhktk.sHtML

[U44] PHP：开启严格类型
来源：http://baike.epnwcf.com/Article/details/gpywjszdh.sHtML

declare(strict_types=1);
来源：http://blog.vehdjk.com/Article/details/ggzsfzqms.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.tarul.cn/Article/details/ghauxxrtj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/grgydjxaa.sHtML

[U46] PHP：可空类型
来源：http://baike.vehdjk.com/Article/details/ghxhuoazm.sHtML

?string $name = null
来源：http://wap.sjlbkw.cn/Article/details/glddfrffj.sHtML

[U47] PHP：联合类型
来源：http://3g.fktsv.cn/Article/details/gcwerbgia.sHtML

int|string $id
来源：http://baike.fktsv.cn/Article/details/gkdbckscf.sHtML

[U48] PHP：纯枚举
来源：http://3g.tarul.cn/Article/details/gvruogsjt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fktsv.cn/Article/details/gtiwaxrgi.sHtML

[U49] PHP：只读属性
来源：http://3g.bbcook.cn/Article/details/ggpxtkoxw.sHtML

public readonly string $name
来源：http://3g.tarul.cn/Article/details/gocfesflk.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.epnwcf.com/Article/details/gugiikkna.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fktsv.cn/Article/details/gdqnakxpf.sHtML

[U51] PHP：数组解构
来源：http://www.blog.epnwcf.com/Article/details/gnsaxuhzi.sHtML

[$a, $b] = $arr;
来源：http://3g.tarul.cn/Article/details/gtiduzvpv.sHtML

[U52] PHP：箭头函数
来源：http://3g.fktsv.cn/Article/details/gkvkhkool.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.sjlbkw.cn/Article/details/gllgqluxc.sHtML

[U53] PHP：空合并运算符
来源：http://3g.sjlbkw.cn/Article/details/gthezwltx.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.vehdjk.com/Article/details/glivfxhkq.sHtML

[U54] PHP：空安全调用
来源：http://m.share.vehdjk.com/Article/details/gwxhddomv.sHtML

$obj?->method()
来源：http://www.share.fktsv.cn/Article/details/ghseviifv.sHtML

[U55] PHP：match 表达式
来源：http://read.share.yfazqb.com/Article/details/gzbhysfxx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.epnwcf.com/Article/details/gqcuuzkrq.sHtML

[U56] PHP：命名参数
来源：http://mobile.sjlbkw.cn/Article/details/glvrkgwyi.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/ggudjcawr.sHtML

[U57] PHP：字符串插值
来源：http://m.share.tarul.cn/Article/details/geghtbhct.sHtML

"值: {$a}"
来源：http://www.share.fktsv.cn/Article/details/gndisjotp.sHtML

[U58] PHP：数组三件套
来源：http://blog.epnwcf.com/Article/details/guyhqfddi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.epnwcf.com/Article/details/ggmehsurb.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.vehdjk.com/Article/details/gvilfgxlj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gjspbdzoq.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.vehdjk.com/Article/details/gesqjsugm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fktsv.cn/Article/details/gknyhgnvx.sHtML

[U61] PHP：正则
来源：http://www.blog.tarul.cn/Article/details/ggcwfmgqr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/gvkivdgdm.sHtML

[U62] PHP：日期对象
来源：http://read.share.bbcook.cn/Article/details/gsytctoig.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.vehdjk.com/Article/details/gqtmppkxt.sHtML

[U63] PHP：文件读写
来源：http://www.share.bbcook.cn/Article/details/gycztkifv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fktsv.cn/Article/details/gcmasqrap.sHtML

[U64] PHP：目录遍历
来源：http://wap.yfazqb.com/Article/details/gftacevbz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.sjlbkw.cn/Article/details/gndvhoqtd.sHtML

[U65] PHP：会话
来源：http://www.m.share.fktsv.cn/Article/details/ggyfsrjki.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gjmywlrqc.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fktsv.cn/Article/details/gltbnpnhi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.sjlbkw.cn/Article/details/gjhxkdbze.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fktsv.cn/Article/details/gvczbdqwm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.bbcook.cn/Article/details/gemqyinbz.sHtML

[U68] PHP：PDO 连接
来源：http://wap.bbcook.cn/Article/details/gcongyxqs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.epnwcf.com/Article/details/gmtrjbjdx.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.epnwcf.com/Article/details/gcrbnhyjr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.epnwcf.com/Article/details/giaaasaiu.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.epnwcf.com/Article/details/gewfhrnge.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.epnwcf.com/Article/details/guwjqdxgp.sHtML

[U71] PHP：抛出异常
来源：http://blog.epnwcf.com/Article/details/ghdexfgdm.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.vehdjk.com/Article/details/ghbbbywrs.sHtML

[U72] PHP：写错误日志
来源：http://www.share.epnwcf.com/Article/details/gwvfqqbtc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.tarul.cn/Article/details/gutnrbpme.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.tarul.cn/Article/details/gxgbzxkzf.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.yfazqb.com/Article/details/gncvgajjx.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fktsv.cn/Article/details/gjlpeqiis.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.tarul.cn/Article/details/gunbwkfhs.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.tarul.cn/Article/details/gblvzzcce.sHtML

composer require psr/container
来源：http://mobile.yfazqb.com/Article/details/ghcrknufl.sHtML

[U76] PHP：简单路由
来源：http://wap.fktsv.cn/Article/details/gjuchpdxj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.tarul.cn/Article/details/gpyxmhdfa.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.vehdjk.com/Article/details/gbzpjokgw.sHtML

composer require twig/twig
来源：http://m.share.bbcook.cn/Article/details/gkquvckaw.sHtML

[U78] PHP：单元测试
来源：http://wap.tarul.cn/Article/details/gzjxqoykh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fktsv.cn/Article/details/gyvfdwmux.sHtML

[U79] PHP：静态分析
来源：http://m.share.sjlbkw.cn/Article/details/gviqltyyy.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fktsv.cn/Article/details/gdxjyhedg.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.yfazqb.com/Article/details/gkphjvmnr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fktsv.cn/Article/details/gtbgakkdp.sHtML


<!-- 参考信息 -->