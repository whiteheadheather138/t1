代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.vehdjk.com/Article/details/gzaldhaxh.sHtML

[S57] C++：编译期常量
来源：http://3g.vehdjk.com/Article/details/giqvulyrc.sHtML

constexpr int N = 10;
来源：http://read.share.yfazqb.com/Article/details/gqqquvryu.sHtML

[S58] C++：命名空间
来源：http://www.m.share.bbcook.cn/Article/details/ghqniezbj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.tarul.cn/Article/details/glepqvnms.sHtML

[S59] C++：静态断言
来源：http://www.blog.bbcook.cn/Article/details/gixacpsex.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.vehdjk.com/Article/details/gkqnnqcns.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.epnwcf.com/Article/details/gbgnfwnqi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.tarul.cn/Article/details/gfwcsllyp.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfrzuahkm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gfwvoqgfc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpwelqflc.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.tarul.cn/Article/details/gjtikobke.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/goamxcadd.sHtML

[T02] Kotlin：变量
来源：http://3g.yfazqb.com/Article/details/gxctwavdx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.bbcook.cn/Article/details/gjkbzdhyy.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/ghrjldkbl.sHtML

"值: $b"
来源：http://read.share.vehdjk.com/Article/details/gejqtnqke.sHtML

[T04] Kotlin：空安全
来源：http://wap.fktsv.cn/Article/details/gagkmgsqj.sHtML

val n: String? = null;  n?.length
来源：http://3g.fktsv.cn/Article/details/gdyfttcsf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.tarul.cn/Article/details/gcldiipmh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.sjlbkw.cn/Article/details/gnzfesegq.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.bbcook.cn/Article/details/gwxxeommo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.epnwcf.com/Article/details/gjrqjpuik.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/gmbowpsdy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.epnwcf.com/Article/details/gowjitztr.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.yfazqb.com/Article/details/gwwkqznyf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gkywdzepn.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.tarul.cn/Article/details/gsusklwrg.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.vehdjk.com/Article/details/gahfsixyw.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fktsv.cn/Article/details/gvepqfcrw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.yfazqb.com/Article/details/gzunzewed.sHtML

[T11] Kotlin：协程
来源：http://www.blog.sjlbkw.cn/Article/details/gsokgyqum.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.tarul.cn/Article/details/gaynvmzfz.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/ghggnbmvr.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fktsv.cn/Article/details/gtqznuhzo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.tarul.cn/Article/details/ggoziuxzz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.epnwcf.com/Article/details/gtazjyylu.sHtML

[T14] Kotlin：循环
来源：http://wap.fktsv.cn/Article/details/gwdxmvfcb.sHtML

for (i in 1..10) println(i)
来源：http://blog.yfazqb.com/Article/details/gwmhhbewq.sHtML

[T15] Kotlin：接口
来源：http://wap.tarul.cn/Article/details/gjjhqqecp.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.sjlbkw.cn/Article/details/gitmfckbo.sHtML

[T16] Swift：Hello World
来源：http://blog.bbcook.cn/Article/details/guvohkzjq.sHtML

print("Hello")
来源：http://baike.sjlbkw.cn/Article/details/glsumzdpr.sHtML

[T17] Swift：变量与常量
来源：http://read.share.sjlbkw.cn/Article/details/gfqxcccxf.sHtML

var a = 1;  let b = 2
来源：http://m.share.sjlbkw.cn/Article/details/guzogqfpm.sHtML

[T18] Swift：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gxyrkckgr.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gbffkfswx.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/gbonrleeu.sHtML

if let n = opt { print(n) }
来源：http://wap.tarul.cn/Article/details/gtcvwufvt.sHtML

[T20] Swift：数组操作
来源：http://mobile.tarul.cn/Article/details/gnbahwpna.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/goljzsjeg.sHtML

[T21] Swift：遍历
来源：http://mobile.sjlbkw.cn/Article/details/grplcwlkq.sHtML

for x in a { print(x) }
来源：http://blog.vehdjk.com/Article/details/ghngtczpn.sHtML

[T22] Swift：字典
来源：http://wap.fktsv.cn/Article/details/gzqswlfng.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.sjlbkw.cn/Article/details/gclqvlfep.sHtML

[T23] Swift：函数
来源：http://read.share.bbcook.cn/Article/details/gorykariw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.vehdjk.com/Article/details/gmiwibwcu.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gviqjlhef.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.vehdjk.com/Article/details/gwhseipeh.sHtML

[T25] Swift：结构体
来源：http://blog.epnwcf.com/Article/details/gygglglyv.sHtML

struct P { var x: Int }
来源：http://blog.vehdjk.com/Article/details/gmxzqhthk.sHtML

[T26] Swift：类与重写
来源：http://3g.vehdjk.com/Article/details/goovwrjbo.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfliqhmac.sHtML

[T27] Swift：错误处理
来源：http://mobile.vehdjk.com/Article/details/gkhtiehrt.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.bbcook.cn/Article/details/gucboaxdg.sHtML

[T28] Swift：枚举
来源：http://m.share.tarul.cn/Article/details/ggyhwlcvp.sHtML

enum Color { case red, green }
来源：http://m.share.epnwcf.com/Article/details/gbljnjzhq.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.sjlbkw.cn/Article/details/gszxsagot.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gipciephr.sHtML

[T30] Swift：协议
来源：http://www.share.bbcook.cn/Article/details/gsjhkdbif.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.sjlbkw.cn/Article/details/gwyuaxxrz.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gismlqzpt.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/gnoyqxopl.sHtML

[T32] Lua：局部变量
来源：http://3g.tarul.cn/Article/details/ghowduxfp.sHtML

local a = 1
来源：http://m.share.yfazqb.com/Article/details/gnzujetuj.sHtML

[T33] Lua：表（数组）
来源：http://read.share.sjlbkw.cn/Article/details/gbgmtoxta.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.epnwcf.com/Article/details/ghfnzwtmx.sHtML

[T34] Lua：遍历表
来源：http://wap.vehdjk.com/Article/details/gkdcsbdhl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.epnwcf.com/Article/details/gotykvjkk.sHtML

[T35] Lua：字典表
来源：http://baike.sjlbkw.cn/Article/details/gxjlveeix.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.epnwcf.com/Article/details/gnozqdogl.sHtML

[T36] Lua：函数
来源：http://www.blog.epnwcf.com/Article/details/gkavjzwhd.sHtML

function add(a, b) return a + b end
来源：http://www.share.epnwcf.com/Article/details/gutucqmeo.sHtML

[T37] Lua：字符串拼接
来源：http://blog.vehdjk.com/Article/details/gndkbybbl.sHtML

"a" .. "b"
来源：http://mobile.fktsv.cn/Article/details/gwstyetqu.sHtML

[T38] Lua：条件
来源：http://www.blog.fktsv.cn/Article/details/gowclraki.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/gifbiumlj.sHtML

[T39] Lua：模式匹配
来源：http://blog.fktsv.cn/Article/details/gdikklzex.sHtML

string.find(s, "%d+")
来源：http://baike.tarul.cn/Article/details/gxqcenszy.sHtML

[T40] Lua：元表
来源：http://mobile.epnwcf.com/Article/details/gjiewfbxd.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.tarul.cn/Article/details/gcdkfqkda.sHtML

[T41] Perl：Hello World
来源：http://baike.bbcook.cn/Article/details/gdgantnia.sHtML

print "Hello\n";
来源：http://blog.tarul.cn/Article/details/gwgjbpsic.sHtML

[T42] Perl：变量类型
来源：http://read.share.vehdjk.com/Article/details/gdzyttdrb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.sjlbkw.cn/Article/details/gejnifciq.sHtML

[T43] Perl：字符串插值
来源：http://3g.bbcook.cn/Article/details/gxwtcoipn.sHtML

"值: $a"
来源：http://wap.yfazqb.com/Article/details/gholgxjth.sHtML

[T44] Perl：条件
来源：http://wap.epnwcf.com/Article/details/gmwdsouzl.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.tarul.cn/Article/details/gvzwjudsr.sHtML

[T45] Perl：数组遍历
来源：http://baike.epnwcf.com/Article/details/gnowwyfqp.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fktsv.cn/Article/details/gvjcrcysj.sHtML

[T46] Perl：哈希操作
来源：http://read.share.tarul.cn/Article/details/geidvhzqw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.epnwcf.com/Article/details/goniwhvjq.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.vehdjk.com/Article/details/gjskndnps.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.epnwcf.com/Article/details/ghcqozylz.sHtML

[T48] Perl：正则替换
来源：http://www.share.vehdjk.com/Article/details/gftaxzqlk.sHtML

$s =~ s/old/new/g;
来源：http://blog.vehdjk.com/Article/details/gqcthziiz.sHtML

[T49] Perl：函数
来源：http://wap.bbcook.cn/Article/details/gcwsjgefe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gjjmuhufv.sHtML

[T50] Perl：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gzqnpxxcn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.yfazqb.com/Article/details/gawtimpmv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.epnwcf.com/Article/details/giskecvme.sHtML

[T51] Scala：Hello World
来源：http://wap.tarul.cn/Article/details/gedtijrvc.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/grithmywp.sHtML

[T52] Scala：变量
来源：http://3g.fktsv.cn/Article/details/gubomfalw.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gttdnvnbt.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gwtdqsgre.sHtML

s"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gffxuvmkz.sHtML

[T54] Scala：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gkqzfedqo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.bbcook.cn/Article/details/gvsoklsnq.sHtML

[T55] Scala：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gbirighpo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.tarul.cn/Article/details/gaziqtugx.sHtML

[T56] Scala：样例类
来源：http://www.m.share.vehdjk.com/Article/details/gbhltxeyi.sHtML

case class User(name: String, age: Int)
来源：http://3g.sjlbkw.cn/Article/details/gekpsudvz.sHtML

[T57] Scala：模式匹配
来源：http://baike.yfazqb.com/Article/details/gsjefjobo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gtwxyapif.sHtML

[T58] Scala：函数定义
来源：http://blog.yfazqb.com/Article/details/grwjvutxh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.vehdjk.com/Article/details/gwqjyxxml.sHtML

[T59] Scala：循环
来源：http://mobile.vehdjk.com/Article/details/gvzqllojg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gsbxramod.sHtML

[T60] Scala：折叠
来源：http://read.share.tarul.cn/Article/details/gmhjmrakm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.yfazqb.com/Article/details/gukftyeva.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/guyllysyx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.yfazqb.com/Article/details/ggyxlsmlu.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gbimuikns.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.tarul.cn/Article/details/gcjnpphej.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fktsv.cn/Article/details/grtzjpzmm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.yfazqb.com/Article/details/gidphtvbk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.tarul.cn/Article/details/grdzyphza.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.sjlbkw.cn/Article/details/gbktwwwbs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.vehdjk.com/Article/details/gzxhnxvib.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fktsv.cn/Article/details/gmiwyrnbn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.tarul.cn/Article/details/gtuwrzozc.sHtML

[U05] Py：列表去重且保序
来源：http://blog.vehdjk.com/Article/details/gasamelzt.sHtML

list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gqipbnlbb.sHtML

[U06] Py：合并两个字典
来源：http://baike.yfazqb.com/Article/details/gboctrvis.sHtML

{**a, **b}
来源：http://www.m.share.yfazqb.com/Article/details/ggtjlscxx.sHtML

[U07] Py：反转字典键值
来源：http://3g.sjlbkw.cn/Article/details/givlqbajo.sHtML

{v: k for k, v in d.items()}
来源：http://baike.sjlbkw.cn/Article/details/gkhlpqohj.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.bbcook.cn/Article/details/glibnujzo.sHtML

[y for x in nested for y in x]
来源：http://read.share.yfazqb.com/Article/details/gvpaaqzeb.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.yfazqb.com/Article/details/gbmhlmgwq.sHtML

max(d, key=d.get)
来源：http://www.blog.epnwcf.com/Article/details/gbuxzmpga.sHtML

[U10] Py：按值排序字典
来源：http://read.share.tarul.cn/Article/details/gqtwffczo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.epnwcf.com/Article/details/ggivgficf.sHtML

[U11] Py：生成器表达式
来源：http://blog.yfazqb.com/Article/details/gvzdsyxol.sHtML

(x * 2 for x in arr)
来源：http://3g.epnwcf.com/Article/details/geikgqopu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.sjlbkw.cn/Article/details/gjsbkytap.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.tarul.cn/Article/details/gccdxwchb.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fktsv.cn/Article/details/gizkmolks.sHtML

deque(maxlen=10)
来源：http://baike.vehdjk.com/Article/details/gsurzlqys.sHtML

[U14] Py：分组收集到列表
来源：http://3g.vehdjk.com/Article/details/guxuheldh.sHtML

defaultdict(list)
来源：http://www.blog.epnwcf.com/Article/details/gmtfodcoi.sHtML

[U15] Py：高精度计时
来源：http://baike.yfazqb.com/Article/details/guitafnky.sHtML

t = time.perf_counter()
来源：http://wap.yfazqb.com/Article/details/gsdovwwho.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.sjlbkw.cn/Article/details/gidgmrzrm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.tarul.cn/Article/details/geyqshsjl.sHtML

[U17] Py：初始化日志
来源：http://www.share.vehdjk.com/Article/details/gkdvqtcxg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.sjlbkw.cn/Article/details/gyqkkzmfr.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fktsv.cn/Article/details/gbgsnhdly.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.yfazqb.com/Article/details/gayoewfnb.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.vehdjk.com/Article/details/gjkpffrmo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.vehdjk.com/Article/details/gbggkvwbb.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.epnwcf.com/Article/details/gjdtuhqoi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.vehdjk.com/Article/details/gjrgwxygl.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.sjlbkw.cn/Article/details/gzzrgrrsm.sHtML

@contextlib.contextmanager
来源：http://read.share.bbcook.cn/Article/details/gsjeubifs.sHtML

[U22] Py：矩阵转置
来源：http://m.share.yfazqb.com/Article/details/griqsjdbm.sHtML

list(zip(*m))
来源：http://www.share.epnwcf.com/Article/details/gkwyvocft.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.sjlbkw.cn/Article/details/gfzgtnakj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fktsv.cn/Article/details/gywatdxwz.sHtML

[U24] Py：路径操作
来源：http://baike.fktsv.cn/Article/details/gbmrwntrg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/ghtcgcerh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.tarul.cn/Article/details/gboatcpus.sHtML

csv.DictReader(f)
来源：http://3g.fktsv.cn/Article/details/gxnangigr.sHtML

[U26] Py：并发下载
来源：http://3g.sjlbkw.cn/Article/details/gbazdljjl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.tarul.cn/Article/details/gybywsdno.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.yfazqb.com/Article/details/gjyrqtxhb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fktsv.cn/Article/details/goceechum.sHtML

[U28] Py：类型别名
来源：http://read.share.yfazqb.com/Article/details/ghdscngpf.sHtML

UserId = int
来源：http://3g.tarul.cn/Article/details/gbybpgquc.sHtML

[U29] Py：属性校验
来源：http://www.m.share.sjlbkw.cn/Article/details/gtakwcrkf.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.vehdjk.com/Article/details/gqswfzpth.sHtML

[U30] Py：数据类
来源：http://3g.yfazqb.com/Article/details/gewebkzgq.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fktsv.cn/Article/details/glvmacyyf.sHtML

[U31] Py：单测
来源：http://read.share.epnwcf.com/Article/details/gtdvlwbvq.sHtML

python -m pytest -q
来源：http://read.share.vehdjk.com/Article/details/gbxpitmcl.sHtML

[U32] Py：代码格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gfmatppfe.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fktsv.cn/Article/details/gofifvoyk.sHtML

[U33] Py：打包发布
来源：http://blog.tarul.cn/Article/details/gdwqyktqt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.tarul.cn/Article/details/gbjgrdzig.sHtML

[U34] Py：判断编码
来源：http://wap.vehdjk.com/Article/details/gmchwwjgi.sHtML

chardet.detect(raw)
来源：http://m.share.yfazqb.com/Article/details/gnxyathqi.sHtML

[U35] Py：发送邮件
来源：http://www.blog.bbcook.cn/Article/details/glvaxyohk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.vehdjk.com/Article/details/gduqdgpel.sHtML

[U36] Py：定时任务
来源：http://m.share.yfazqb.com/Article/details/gcibdgorb.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.tarul.cn/Article/details/gsvcwwzvf.sHtML

[U37] Py：读写 Excel
来源：http://mobile.sjlbkw.cn/Article/details/geednukeq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.epnwcf.com/Article/details/gsibfkrhc.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.bbcook.cn/Article/details/gfwngkacm.sHtML

Path(__file__).resolve().parent
来源：http://read.share.epnwcf.com/Article/details/grgijmmtm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fktsv.cn/Article/details/gpyukizzq.sHtML

sys.stdout.isatty()
来源：http://m.share.bbcook.cn/Article/details/gyvjpwzwn.sHtML

[U40] Py：打印到标准错误
来源：http://blog.vehdjk.com/Article/details/gbdabmjst.sHtML

print("err", file=sys.stderr)
来源：http://m.share.epnwcf.com/Article/details/gwmyjqbbs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fktsv.cn/Article/details/gifwvonsx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.vehdjk.com/Article/details/ggsfqtvtr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.vehdjk.com/Article/details/gojovoxos.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.tarul.cn/Article/details/gumgvtfuu.sHtML

[U43] PHP：声明命名空间
来源：http://wap.tarul.cn/Article/details/gpepdwldt.sHtML

namespace App\Http;
来源：http://mobile.bbcook.cn/Article/details/gasfebnvg.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.yfazqb.com/Article/details/gdejlpoqu.sHtML

declare(strict_types=1);
来源：http://www.blog.bbcook.cn/Article/details/gqkyvbyco.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.tarul.cn/Article/details/gmvvfjrae.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gwhymuqyy.sHtML

[U46] PHP：可空类型
来源：http://www.share.epnwcf.com/Article/details/gtrchjdug.sHtML

?string $name = null
来源：http://read.share.fktsv.cn/Article/details/ggqemndtk.sHtML

[U47] PHP：联合类型
来源：http://www.blog.sjlbkw.cn/Article/details/gkprgbaij.sHtML

int|string $id
来源：http://baike.tarul.cn/Article/details/gqmmdexgk.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.epnwcf.com/Article/details/glomokpdu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glokztnso.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.bbcook.cn/Article/details/glqnptptb.sHtML

public readonly string $name
来源：http://www.m.share.fktsv.cn/Article/details/gymtjxosq.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.vehdjk.com/Article/details/gejkhdlqz.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.vehdjk.com/Article/details/gkcgpguue.sHtML

[U51] PHP：数组解构
来源：http://3g.yfazqb.com/Article/details/gieapypya.sHtML

[$a, $b] = $arr;
来源：http://baike.tarul.cn/Article/details/ggsfcxsaz.sHtML

[U52] PHP：箭头函数
来源：http://mobile.tarul.cn/Article/details/gyufdixep.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fktsv.cn/Article/details/gjufycgwg.sHtML

[U53] PHP：空合并运算符
来源：http://baike.sjlbkw.cn/Article/details/gfhdzasgi.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.sjlbkw.cn/Article/details/gdzlpgslu.sHtML

[U54] PHP：空安全调用
来源：http://wap.yfazqb.com/Article/details/gotwathki.sHtML

$obj?->method()
来源：http://mobile.fktsv.cn/Article/details/gdorkcyvj.sHtML

[U55] PHP：match 表达式
来源：http://baike.epnwcf.com/Article/details/glsxuzsem.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/gwzyggeaq.sHtML

[U56] PHP：命名参数
来源：http://blog.sjlbkw.cn/Article/details/gjwgrwnni.sHtML

f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/gtjcbbjks.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gunqqestr.sHtML

"值: {$a}"
来源：http://www.blog.bbcook.cn/Article/details/gqmoynxmr.sHtML

[U58] PHP：数组三件套
来源：http://baike.vehdjk.com/Article/details/geeiabuzi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/grzsxzryx.sHtML

[U59] PHP：自定义排序
来源：http://mobile.bbcook.cn/Article/details/gbamsnjrx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gbiubagyh.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.epnwcf.com/Article/details/gbkgaqeon.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.vehdjk.com/Article/details/gbbvsvbvw.sHtML

[U61] PHP：正则
来源：http://m.share.fktsv.cn/Article/details/grdnthahg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gldbsuokn.sHtML

[U62] PHP：日期对象
来源：http://baike.tarul.cn/Article/details/gnpvonxed.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.sjlbkw.cn/Article/details/gqmdglsqm.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.vehdjk.com/Article/details/gxipntehe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.tarul.cn/Article/details/gdnixdohl.sHtML

[U64] PHP：目录遍历
来源：http://blog.sjlbkw.cn/Article/details/gkkqjrekp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.bbcook.cn/Article/details/gnzojijpk.sHtML

[U65] PHP：会话
来源：http://m.share.yfazqb.com/Article/details/gungygbhb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gnkxnscqk.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.vehdjk.com/Article/details/gdkvuvide.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.bbcook.cn/Article/details/grlkxvbct.sHtML

[U67] PHP：处理文件上传
来源：http://wap.yfazqb.com/Article/details/gdxenfvzb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.bbcook.cn/Article/details/gqnscjqfg.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.tarul.cn/Article/details/ggwfnfrim.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.tarul.cn/Article/details/guakchbax.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gaauzxcdk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fktsv.cn/Article/details/gbzgvpsag.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.sjlbkw.cn/Article/details/ghgqsyapr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.vehdjk.com/Article/details/getyvfapu.sHtML

[U71] PHP：抛出异常
来源：http://baike.tarul.cn/Article/details/gvzpbxkmf.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.tarul.cn/Article/details/ghhehzjxs.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.bbcook.cn/Article/details/gzljgrikh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.yfazqb.com/Article/details/gxknnmdke.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fktsv.cn/Article/details/gtjbftmck.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.bbcook.cn/Article/details/gvjpoekdm.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/getkjlyfo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fktsv.cn/Article/details/guwlxkbca.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fktsv.cn/Article/details/gwhbauvex.sHtML

composer require psr/container
来源：http://www.share.sjlbkw.cn/Article/details/gcytjjseo.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.bbcook.cn/Article/details/gagrdoqzx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.sjlbkw.cn/Article/details/gcxwebqop.sHtML

[U77] PHP：模板渲染
来源：http://wap.vehdjk.com/Article/details/gdhifawjp.sHtML

composer require twig/twig
来源：http://m.share.tarul.cn/Article/details/gvkyifibq.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.yfazqb.com/Article/details/graynqxcq.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fktsv.cn/Article/details/gxjxyroff.sHtML

[U79] PHP：静态分析
来源：http://www.blog.vehdjk.com/Article/details/gnghqmsdk.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.bbcook.cn/Article/details/gvxcjjhbg.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fktsv.cn/Article/details/gauiuqjms.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fktsv.cn/Article/details/graqhbaux.sHtML

[U81] JS：初始化项目
来源：http://www.blog.epnwcf.com/Article/details/gcfmoohtt.sHtML

npm init -y;  npm i express
来源：http://mobile.fktsv.cn/Article/details/ghngemgtz.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.vehdjk.com/Article/details/gnfnwcbgj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.tarul.cn/Article/details/gpupwquxc.sHtML


<!-- 参考信息 -->