代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://3g.fktsv.cn/Article/details/gncrbuyhv.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gkvznogoo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.tarul.cn/Article/details/gszyajkpj.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.bbcook.cn/Article/details/gegyxoeee.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.yfazqb.com/Article/details/gdrtqaqjv.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gyluxiyts.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fktsv.cn/Article/details/gcxbbmjit.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gslpysvcc.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gkzuerurx.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/gthtdcxzp.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/gnrvidibk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fktsv.cn/Article/details/gqsmdhrfr.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gsctqzxtn.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/gacipngeu.sHtML

[T04] Kotlin：空安全
来源：http://www.share.sjlbkw.cn/Article/details/gtogwrhqs.sHtML

val n: String? = null;  n?.length
来源：http://baike.tarul.cn/Article/details/ghvqnpapw.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.tarul.cn/Article/details/gjjhteais.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/gqzqdnmof.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gynuakler.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.epnwcf.com/Article/details/ghrheuhpp.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gneyinplc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/gplrhsfpa.sHtML

[T08] Kotlin：数据类
来源：http://wap.yfazqb.com/Article/details/grcasushg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.epnwcf.com/Article/details/gmnhhhhtg.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.bbcook.cn/Article/details/geerjzkef.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.sjlbkw.cn/Article/details/ghwpegwuq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.epnwcf.com/Article/details/gesdkxkfx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.bbcook.cn/Article/details/gdhwavutb.sHtML

[T11] Kotlin：协程
来源：http://wap.tarul.cn/Article/details/gvetffxry.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.yfazqb.com/Article/details/gwkguobzh.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.epnwcf.com/Article/details/gjjkbgtyk.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.vehdjk.com/Article/details/gynzpnacj.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.sjlbkw.cn/Article/details/grchdhkhn.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.bbcook.cn/Article/details/grfaxrbbu.sHtML

[T14] Kotlin：循环
来源：http://baike.tarul.cn/Article/details/gxkbplowx.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gdajlhsdk.sHtML

[T15] Kotlin：接口
来源：http://m.share.yfazqb.com/Article/details/gbwniakkl.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.sjlbkw.cn/Article/details/gxygwylbj.sHtML

[T16] Swift：Hello World
来源：http://www.share.tarul.cn/Article/details/gfnspaevf.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/glbxmrazw.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fktsv.cn/Article/details/ggwsocbrl.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/gwsjylizp.sHtML

[T18] Swift：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gtorxkkyu.sHtML

"值: \(b)"
来源：http://www.m.share.sjlbkw.cn/Article/details/gccbxntlx.sHtML

[T19] Swift：可选绑定
来源：http://3g.fktsv.cn/Article/details/ggtbhwoiu.sHtML

if let n = opt { print(n) }
来源：http://3g.fktsv.cn/Article/details/ggdnnyyac.sHtML

[T20] Swift：数组操作
来源：http://baike.sjlbkw.cn/Article/details/gbzhihyal.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/gwjeillbv.sHtML

[T21] Swift：遍历
来源：http://www.blog.tarul.cn/Article/details/gykjawlih.sHtML

for x in a { print(x) }
来源：http://read.share.epnwcf.com/Article/details/gbuvovowy.sHtML

[T22] Swift：字典
来源：http://m.share.epnwcf.com/Article/details/gvwrstfdx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/gddpcmlor.sHtML

[T23] Swift：函数
来源：http://www.blog.vehdjk.com/Article/details/gafnvfwtn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.tarul.cn/Article/details/glwexlsgc.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/grmgnhyyw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.epnwcf.com/Article/details/gfwqhcatz.sHtML

[T25] Swift：结构体
来源：http://read.share.bbcook.cn/Article/details/gcyuhuljp.sHtML

struct P { var x: Int }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxhzxxjp.sHtML

[T26] Swift：类与重写
来源：http://mobile.tarul.cn/Article/details/gphpdtqey.sHtML

class A: Base { override func f() {} }
来源：http://www.share.vehdjk.com/Article/details/gxrpbsckt.sHtML

[T27] Swift：错误处理
来源：http://wap.vehdjk.com/Article/details/gmnpawexf.sHtML

do { try f() } catch { print(error) }
来源：http://wap.tarul.cn/Article/details/gisagrxko.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/gywzogjhk.sHtML

enum Color { case red, green }
来源：http://mobile.yfazqb.com/Article/details/gzfugnprn.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.tarul.cn/Article/details/gvtgsfhof.sHtML

guard let x = opt else { return }
来源：http://mobile.tarul.cn/Article/details/grjurktub.sHtML

[T30] Swift：协议
来源：http://mobile.yfazqb.com/Article/details/gsbhtodti.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.tarul.cn/Article/details/gfxwqnrsh.sHtML

[T31] Lua：Hello World
来源：http://wap.yfazqb.com/Article/details/gsfrdykfs.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gvicmjynn.sHtML

[T32] Lua：局部变量
来源：http://read.share.vehdjk.com/Article/details/gtsqoynhj.sHtML

local a = 1
来源：http://m.share.vehdjk.com/Article/details/gfgfoneux.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gsoemzius.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.sjlbkw.cn/Article/details/gcqxaxzma.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gkyqlmqki.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.epnwcf.com/Article/details/gwtactebf.sHtML

[T35] Lua：字典表
来源：http://read.share.vehdjk.com/Article/details/gvmhssrat.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.bbcook.cn/Article/details/gteetbjph.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/gwiyiqoxt.sHtML

function add(a, b) return a + b end
来源：http://mobile.yfazqb.com/Article/details/gyeqotywa.sHtML

[T37] Lua：字符串拼接
来源：http://wap.vehdjk.com/Article/details/gmhkwfcij.sHtML

"a" .. "b"
来源：http://blog.vehdjk.com/Article/details/gbutquutc.sHtML

[T38] Lua：条件
来源：http://baike.vehdjk.com/Article/details/gcnrmzwky.sHtML

if x > 0 then print("正") end
来源：http://blog.yfazqb.com/Article/details/gjhuhdafj.sHtML

[T39] Lua：模式匹配
来源：http://www.share.epnwcf.com/Article/details/gmqxcprpf.sHtML

string.find(s, "%d+")
来源：http://3g.tarul.cn/Article/details/gkwzcjsdt.sHtML

[T40] Lua：元表
来源：http://blog.epnwcf.com/Article/details/gtqhbmzhe.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fktsv.cn/Article/details/gwnaowypl.sHtML

[T41] Perl：Hello World
来源：http://3g.bbcook.cn/Article/details/gkxiabwvl.sHtML

print "Hello\n";
来源：http://www.m.share.vehdjk.com/Article/details/gbwgpgvdk.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.yfazqb.com/Article/details/glsevwofb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fktsv.cn/Article/details/gzdvjftbm.sHtML

[T43] Perl：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gmyiowcpo.sHtML

"值: $a"
来源：http://3g.vehdjk.com/Article/details/gyozdzurw.sHtML

[T44] Perl：条件
来源：http://www.blog.fktsv.cn/Article/details/gkecgygkc.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fktsv.cn/Article/details/gjtfzisfp.sHtML

[T45] Perl：数组遍历
来源：http://blog.bbcook.cn/Article/details/gnkhprwmy.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.epnwcf.com/Article/details/gadwawmnc.sHtML

[T46] Perl：哈希操作
来源：http://mobile.bbcook.cn/Article/details/gqecqxebq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.epnwcf.com/Article/details/gsvcbdfsn.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.yfazqb.com/Article/details/grarxzchh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fktsv.cn/Article/details/golkhgmvy.sHtML

[T48] Perl：正则替换
来源：http://www.share.vehdjk.com/Article/details/gsimbezzi.sHtML

$s =~ s/old/new/g;
来源：http://mobile.tarul.cn/Article/details/ghzjpsdqg.sHtML

[T49] Perl：函数
来源：http://www.m.share.yfazqb.com/Article/details/gyaxzkfjg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/ghbxcdmgc.sHtML

[T50] Perl：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gxpyemrzh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fktsv.cn/Article/details/gddkrhqsj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.epnwcf.com/Article/details/gfllebknn.sHtML

[T51] Scala：Hello World
来源：http://wap.fktsv.cn/Article/details/gsgvizugt.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/ghvtdhulb.sHtML

[T52] Scala：变量
来源：http://baike.vehdjk.com/Article/details/guklwttrv.sHtML

val a = 1;  var b = 2
来源：http://www.blog.yfazqb.com/Article/details/ghjlnjqfu.sHtML

[T53] Scala：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gazwzhvfi.sHtML

s"值: $b"
来源：http://baike.yfazqb.com/Article/details/gnpajxjwk.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/ghsydewmj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gqfdjuaak.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gftijxsuc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fktsv.cn/Article/details/gsrmyxlke.sHtML

[T56] Scala：样例类
来源：http://m.share.fktsv.cn/Article/details/geoshcyat.sHtML

case class User(name: String, age: Int)
来源：http://read.share.epnwcf.com/Article/details/gdtjdgzus.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gjjoueeaj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.yfazqb.com/Article/details/gvdypvdav.sHtML

[T58] Scala：函数定义
来源：http://3g.epnwcf.com/Article/details/gpbsbqtcx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.yfazqb.com/Article/details/gtezwfxyy.sHtML

[T59] Scala：循环
来源：http://baike.bbcook.cn/Article/details/gubvhcqdw.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gxzkbwraw.sHtML

[T60] Scala：折叠
来源：http://www.blog.vehdjk.com/Article/details/gykguoydo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/ggipvotie.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gfqukujfm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/gxlhzvteb.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzrxdpuxg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.tarul.cn/Article/details/gbnrunwkb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.vehdjk.com/Article/details/gakfcmccq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fktsv.cn/Article/details/gkoztjxzz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.epnwcf.com/Article/details/ggnsnrpke.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.vehdjk.com/Article/details/gwvgxetdn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrjitksf.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/gulbpjwpt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/gmdwrjgsy.sHtML

[U05] Py：列表去重且保序
来源：http://blog.yfazqb.com/Article/details/gxuqeebio.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/gsikbaewy.sHtML

[U06] Py：合并两个字典
来源：http://baike.epnwcf.com/Article/details/gbfjcumyg.sHtML

{**a, **b}
来源：http://3g.fktsv.cn/Article/details/googuzpar.sHtML

[U07] Py：反转字典键值
来源：http://read.share.bbcook.cn/Article/details/gmajfkwve.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.yfazqb.com/Article/details/ggvkubztw.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.tarul.cn/Article/details/gveeswbll.sHtML

[y for x in nested for y in x]
来源：http://baike.sjlbkw.cn/Article/details/guygodgaq.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.yfazqb.com/Article/details/gbyuqbngb.sHtML

max(d, key=d.get)
来源：http://baike.epnwcf.com/Article/details/garrtrrnv.sHtML

[U10] Py：按值排序字典
来源：http://mobile.tarul.cn/Article/details/gwwcewgbq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.vehdjk.com/Article/details/gskbusnmx.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fktsv.cn/Article/details/gxntcxdvv.sHtML

(x * 2 for x in arr)
来源：http://mobile.tarul.cn/Article/details/gfxmskgjc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.bbcook.cn/Article/details/guopnuilu.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.vehdjk.com/Article/details/gpolcwroa.sHtML

[U13] Py：固定长度队列
来源：http://wap.bbcook.cn/Article/details/gjpdabzmi.sHtML

deque(maxlen=10)
来源：http://m.share.sjlbkw.cn/Article/details/gedjipymu.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fktsv.cn/Article/details/grujzdlkb.sHtML

defaultdict(list)
来源：http://baike.yfazqb.com/Article/details/gcscqtjzb.sHtML

[U15] Py：高精度计时
来源：http://www.blog.sjlbkw.cn/Article/details/gysmjtrko.sHtML

t = time.perf_counter()
来源：http://baike.epnwcf.com/Article/details/gmprhlivk.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.epnwcf.com/Article/details/gzmgdhpox.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.epnwcf.com/Article/details/gkcsaxflb.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.tarul.cn/Article/details/gxtasmors.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.vehdjk.com/Article/details/gyykclstb.sHtML

[U18] Py：预编译正则
来源：http://mobile.bbcook.cn/Article/details/gguqbuvgb.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/ganyrhfss.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.vehdjk.com/Article/details/gxfuisvrs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.tarul.cn/Article/details/ghqyhtfih.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.vehdjk.com/Article/details/gcfwvkwxh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.tarul.cn/Article/details/gpjhcwdhi.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.sjlbkw.cn/Article/details/gucjtkflm.sHtML

@contextlib.contextmanager
来源：http://www.share.vehdjk.com/Article/details/gatmrywkj.sHtML

[U22] Py：矩阵转置
来源：http://blog.fktsv.cn/Article/details/gtpaiqzjp.sHtML

list(zip(*m))
来源：http://www.blog.sjlbkw.cn/Article/details/gjnfqfoce.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.epnwcf.com/Article/details/geqnyzfyo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.tarul.cn/Article/details/gmqnfbuum.sHtML

[U24] Py：路径操作
来源：http://3g.tarul.cn/Article/details/gllgiglwp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gizlsmoxr.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.tarul.cn/Article/details/gpgbgdhte.sHtML

csv.DictReader(f)
来源：http://3g.yfazqb.com/Article/details/gxlqhpcrh.sHtML

[U26] Py：并发下载
来源：http://wap.yfazqb.com/Article/details/guehnjtii.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.sjlbkw.cn/Article/details/gzccrloan.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fktsv.cn/Article/details/ggsedggqq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.vehdjk.com/Article/details/ghooczbpm.sHtML

[U28] Py：类型别名
来源：http://read.share.yfazqb.com/Article/details/goidxbshw.sHtML

UserId = int
来源：http://3g.fktsv.cn/Article/details/geipjtzax.sHtML

[U29] Py：属性校验
来源：http://m.share.yfazqb.com/Article/details/gnfossgpc.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgcwwsug.sHtML

[U30] Py：数据类
来源：http://blog.bbcook.cn/Article/details/gaxmpruxa.sHtML

@dataclass(slots=True)
来源：http://m.share.tarul.cn/Article/details/gdbgjpoph.sHtML

[U31] Py：单测
来源：http://wap.yfazqb.com/Article/details/gkuslcyti.sHtML

python -m pytest -q
来源：http://baike.tarul.cn/Article/details/ginbpycts.sHtML

[U32] Py：代码格式化
来源：http://3g.fktsv.cn/Article/details/gpeuyyuor.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.vehdjk.com/Article/details/gykqbhdee.sHtML

[U33] Py：打包发布
来源：http://m.share.vehdjk.com/Article/details/gsjszmukf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.tarul.cn/Article/details/grtrhcqqe.sHtML

[U34] Py：判断编码
来源：http://www.m.share.bbcook.cn/Article/details/gwpkfzogu.sHtML

chardet.detect(raw)
来源：http://m.share.vehdjk.com/Article/details/gqczriuvf.sHtML

[U35] Py：发送邮件
来源：http://read.share.yfazqb.com/Article/details/gpycvnvgy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.tarul.cn/Article/details/guqzacelj.sHtML

[U36] Py：定时任务
来源：http://read.share.bbcook.cn/Article/details/gxjrbrfmu.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.bbcook.cn/Article/details/gmszspozr.sHtML

[U37] Py：读写 Excel
来源：http://3g.tarul.cn/Article/details/gxeikjjul.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.yfazqb.com/Article/details/gfebqbbpy.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.vehdjk.com/Article/details/ggrmgxlhv.sHtML

Path(__file__).resolve().parent
来源：http://m.share.vehdjk.com/Article/details/gvbsrirfm.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.bbcook.cn/Article/details/ggwumnmmt.sHtML

sys.stdout.isatty()
来源：http://read.share.epnwcf.com/Article/details/gjjsivijh.sHtML

[U40] Py：打印到标准错误
来源：http://baike.yfazqb.com/Article/details/gxerzvgqr.sHtML

print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gmdplhmbx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.yfazqb.com/Article/details/glvtevdgs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.epnwcf.com/Article/details/gxjlczvnx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.tarul.cn/Article/details/gehjeqtpl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.yfazqb.com/Article/details/glnanbkwo.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.vehdjk.com/Article/details/gkjjvltuo.sHtML

namespace App\Http;
来源：http://baike.bbcook.cn/Article/details/gzehnoghs.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fktsv.cn/Article/details/gpvpfcsew.sHtML

declare(strict_types=1);
来源：http://mobile.yfazqb.com/Article/details/goumegnry.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.yfazqb.com/Article/details/gheimbtkr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/ggzhojpbg.sHtML

[U46] PHP：可空类型
来源：http://mobile.sjlbkw.cn/Article/details/gdkoriuls.sHtML

?string $name = null
来源：http://read.share.vehdjk.com/Article/details/glasxuael.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fktsv.cn/Article/details/gjdtapiym.sHtML

int|string $id
来源：http://blog.epnwcf.com/Article/details/gqbzvahfs.sHtML

[U48] PHP：纯枚举
来源：http://read.share.epnwcf.com/Article/details/gyuhdukvw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.vehdjk.com/Article/details/glcjngmve.sHtML

[U49] PHP：只读属性
来源：http://blog.yfazqb.com/Article/details/gjvtbgfgi.sHtML

public readonly string $name
来源：http://www.blog.fktsv.cn/Article/details/gbrxygoos.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.bbcook.cn/Article/details/gmhjzbljt.sHtML

public function __construct(private int $id) {}
来源：http://baike.bbcook.cn/Article/details/gvcnlcznm.sHtML

[U51] PHP：数组解构
来源：http://read.share.fktsv.cn/Article/details/gopqwmcye.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.tarul.cn/Article/details/gpapedlxf.sHtML

[U52] PHP：箭头函数
来源：http://www.share.vehdjk.com/Article/details/gghsbzqnu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.sjlbkw.cn/Article/details/gfsskoylc.sHtML

[U53] PHP：空合并运算符
来源：http://baike.epnwcf.com/Article/details/gglukdggx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.yfazqb.com/Article/details/gtoiqxwma.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fktsv.cn/Article/details/gmmgfppfw.sHtML

$obj?->method()
来源：http://blog.vehdjk.com/Article/details/gddvphguh.sHtML

[U55] PHP：match 表达式
来源：http://3g.bbcook.cn/Article/details/gioiqdkaq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.bbcook.cn/Article/details/gtxprtixc.sHtML

[U56] PHP：命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gzyantsyh.sHtML

f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/gqhpuhrui.sHtML

[U57] PHP：字符串插值
来源：http://3g.bbcook.cn/Article/details/gfhjraqal.sHtML

"值: {$a}"
来源：http://www.m.share.tarul.cn/Article/details/grgyjdcob.sHtML

[U58] PHP：数组三件套
来源：http://blog.fktsv.cn/Article/details/gzbeamtme.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.bbcook.cn/Article/details/gtyfarbwi.sHtML

[U59] PHP：自定义排序
来源：http://m.share.vehdjk.com/Article/details/govifzqmo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.yfazqb.com/Article/details/ghnfoptgh.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.sjlbkw.cn/Article/details/gngxcqket.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.bbcook.cn/Article/details/gpxmqptqr.sHtML

[U61] PHP：正则
来源：http://baike.tarul.cn/Article/details/gxbgckjig.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/gutulvjqb.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fktsv.cn/Article/details/gkewhnltj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.sjlbkw.cn/Article/details/gixhtuavr.sHtML

[U63] PHP：文件读写
来源：http://www.blog.sjlbkw.cn/Article/details/gmowmlyne.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.tarul.cn/Article/details/giusjzkkp.sHtML

[U64] PHP：目录遍历
来源：http://mobile.sjlbkw.cn/Article/details/gcjsfkrvm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fktsv.cn/Article/details/grmbopeuw.sHtML

[U65] PHP：会话
来源：http://www.share.epnwcf.com/Article/details/gvrysephq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gyurmdwes.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.epnwcf.com/Article/details/gdlykaswp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fktsv.cn/Article/details/gulysfxsc.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.bbcook.cn/Article/details/gptlkvcji.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.vehdjk.com/Article/details/gzvhftjbn.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.epnwcf.com/Article/details/gjauwuytz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.vehdjk.com/Article/details/gipzqjdxo.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.bbcook.cn/Article/details/gdlegrtuu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.tarul.cn/Article/details/gaovwahwn.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.epnwcf.com/Article/details/gdylkubmj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fktsv.cn/Article/details/gyudacphz.sHtML

[U71] PHP：抛出异常
来源：http://blog.bbcook.cn/Article/details/grqbwzbpr.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.tarul.cn/Article/details/gwhplundv.sHtML

[U72] PHP：写错误日志
来源：http://baike.yfazqb.com/Article/details/gnkdcyive.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.sjlbkw.cn/Article/details/glcbhppkv.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.vehdjk.com/Article/details/gobkbkqgz.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fktsv.cn/Article/details/gkypbxjwa.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.tarul.cn/Article/details/gnleajbtc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.yfazqb.com/Article/details/gtwmqckim.sHtML

[U75] PHP：依赖注入
来源：http://blog.sjlbkw.cn/Article/details/ggobxgycp.sHtML

composer require psr/container
来源：http://3g.fktsv.cn/Article/details/gybupuufl.sHtML

[U76] PHP：简单路由
来源：http://3g.sjlbkw.cn/Article/details/gzxvwjbis.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.yfazqb.com/Article/details/ghzzaxtqx.sHtML

[U77] PHP：模板渲染
来源：http://blog.epnwcf.com/Article/details/gthzxujxw.sHtML

composer require twig/twig
来源：http://m.share.vehdjk.com/Article/details/gzhdwcmlb.sHtML

[U78] PHP：单元测试
来源：http://read.share.yfazqb.com/Article/details/gqjanzvwo.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.sjlbkw.cn/Article/details/gyugzrtyu.sHtML

[U79] PHP：静态分析
来源：http://3g.sjlbkw.cn/Article/details/gseqyscit.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.yfazqb.com/Article/details/gorbeumgy.sHtML

[U80] PHP：代码规范修复
来源：http://baike.vehdjk.com/Article/details/gtjzmzuet.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.vehdjk.com/Article/details/gsaceogab.sHtML

[U81] JS：初始化项目
来源：http://www.share.epnwcf.com/Article/details/gfafkwbtz.sHtML

npm init -y;  npm i express
来源：http://read.share.vehdjk.com/Article/details/gkysvawoa.sHtML

[U82] JS：package.json 脚本
来源：http://blog.vehdjk.com/Article/details/ggcqyikdg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.bbcook.cn/Article/details/ghkludddk.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fktsv.cn/Article/details/gmsijzaot.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gdzibnebf.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.bbcook.cn/Article/details/grqnqidfl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.tarul.cn/Article/details/ggissqdbv.sHtML


<!-- 参考信息 -->