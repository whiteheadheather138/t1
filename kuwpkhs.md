代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/gcqoxqluc.sHtML

[S59] C++：静态断言
来源：http://baike.bbcook.cn/Article/details/gtxwqbnkz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.sjlbkw.cn/Article/details/gkejkvayn.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fktsv.cn/Article/details/gjolkbcju.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/gvyaipncm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/guglgcdmg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/gydrdebrp.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gginqadut.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/grospdznc.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/gzciunypw.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gbntolibe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.yfazqb.com/Article/details/ghvjqmqnm.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.tarul.cn/Article/details/gacvcyhdv.sHtML

"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/grqpwbywu.sHtML

[T04] Kotlin：空安全
来源：http://3g.vehdjk.com/Article/details/gafordyjr.sHtML

val n: String? = null;  n?.length
来源：http://m.share.yfazqb.com/Article/details/givablmki.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fktsv.cn/Article/details/gegynarkq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.epnwcf.com/Article/details/gdsmhkogs.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/glrqdoszq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gbdmbinwg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.tarul.cn/Article/details/goypkokof.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.bbcook.cn/Article/details/gvdxxubir.sHtML

[T08] Kotlin：数据类
来源：http://m.share.tarul.cn/Article/details/gzmiqfebo.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fktsv.cn/Article/details/grmoylrxi.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.bbcook.cn/Article/details/gvvcmrurf.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.bbcook.cn/Article/details/glyzuefni.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/gzradkmsd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.tarul.cn/Article/details/gxbijefla.sHtML

[T11] Kotlin：协程
来源：http://mobile.epnwcf.com/Article/details/gtgdhjiuv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.tarul.cn/Article/details/ggioghjuo.sHtML

[T12] Kotlin：解构声明
来源：http://baike.bbcook.cn/Article/details/gjryzcsqb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.epnwcf.com/Article/details/gpvfektrs.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/gzuntldpp.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.vehdjk.com/Article/details/gtbspktri.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fktsv.cn/Article/details/gpxcfbgra.sHtML

for (i in 1..10) println(i)
来源：http://wap.epnwcf.com/Article/details/gwndkcslg.sHtML

[T15] Kotlin：接口
来源：http://blog.fktsv.cn/Article/details/gxbqppwmm.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fktsv.cn/Article/details/gijkiolbz.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/ggfmtavpi.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/ghwigfxwu.sHtML

[T17] Swift：变量与常量
来源：http://baike.fktsv.cn/Article/details/gxwecsbdw.sHtML

var a = 1;  let b = 2
来源：http://www.share.bbcook.cn/Article/details/gpgqsbahw.sHtML

[T18] Swift：字符串插值
来源：http://baike.tarul.cn/Article/details/gkvpsbkyf.sHtML

"值: \(b)"
来源：http://baike.bbcook.cn/Article/details/gittxlemz.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/gnuwtnuqm.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.vehdjk.com/Article/details/gvxdmfnan.sHtML

[T20] Swift：数组操作
来源：http://m.share.bbcook.cn/Article/details/gnphtxmwr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.sjlbkw.cn/Article/details/gmrilnues.sHtML

[T21] Swift：遍历
来源：http://3g.epnwcf.com/Article/details/geaysczvd.sHtML

for x in a { print(x) }
来源：http://3g.bbcook.cn/Article/details/gvihhxnpe.sHtML

[T22] Swift：字典
来源：http://baike.tarul.cn/Article/details/gxgmqslch.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.yfazqb.com/Article/details/grracupws.sHtML

[T23] Swift：函数
来源：http://3g.vehdjk.com/Article/details/gkzljuiqw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.sjlbkw.cn/Article/details/ghwtdmlqb.sHtML

[T24] Swift：闭包
来源：http://www.m.share.tarul.cn/Article/details/gowbvdslf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.bbcook.cn/Article/details/gukksovok.sHtML

[T25] Swift：结构体
来源：http://baike.bbcook.cn/Article/details/gdsbuxuiz.sHtML

struct P { var x: Int }
来源：http://blog.bbcook.cn/Article/details/gikanezdb.sHtML

[T26] Swift：类与重写
来源：http://read.share.bbcook.cn/Article/details/gqcgojvcf.sHtML

class A: Base { override func f() {} }
来源：http://baike.sjlbkw.cn/Article/details/gllxmcqqj.sHtML

[T27] Swift：错误处理
来源：http://www.blog.tarul.cn/Article/details/gknzjslmf.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/gserpsfkp.sHtML

[T28] Swift：枚举
来源：http://read.share.vehdjk.com/Article/details/giazrvzor.sHtML

enum Color { case red, green }
来源：http://www.blog.yfazqb.com/Article/details/gyzfmtmwc.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.epnwcf.com/Article/details/ggcdttish.sHtML

guard let x = opt else { return }
来源：http://wap.vehdjk.com/Article/details/gbufwrtaa.sHtML

[T30] Swift：协议
来源：http://mobile.vehdjk.com/Article/details/guudqhejf.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.tarul.cn/Article/details/gfgzwuftz.sHtML

[T31] Lua：Hello World
来源：http://blog.epnwcf.com/Article/details/gyfobgjzj.sHtML

print("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gpsrgshjc.sHtML

[T32] Lua：局部变量
来源：http://m.share.fktsv.cn/Article/details/gbfylabjg.sHtML

local a = 1
来源：http://baike.fktsv.cn/Article/details/gjmdvjjyz.sHtML

[T33] Lua：表（数组）
来源：http://3g.fktsv.cn/Article/details/gszmxjdzs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fktsv.cn/Article/details/girslnehb.sHtML

[T34] Lua：遍历表
来源：http://wap.bbcook.cn/Article/details/gonnpwmzq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/gxwneeskn.sHtML

[T35] Lua：字典表
来源：http://3g.tarul.cn/Article/details/gkwygwnfl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.sjlbkw.cn/Article/details/gtdbhkgjd.sHtML

[T36] Lua：函数
来源：http://baike.tarul.cn/Article/details/gdxgjrohq.sHtML

function add(a, b) return a + b end
来源：http://wap.tarul.cn/Article/details/gszhapxms.sHtML

[T37] Lua：字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gpwqyokdj.sHtML

"a" .. "b"
来源：http://www.share.bbcook.cn/Article/details/glphhlrts.sHtML

[T38] Lua：条件
来源：http://read.share.vehdjk.com/Article/details/gmvqitved.sHtML

if x > 0 then print("正") end
来源：http://mobile.vehdjk.com/Article/details/gkxsbibob.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gdbnzyldn.sHtML

string.find(s, "%d+")
来源：http://3g.epnwcf.com/Article/details/gjegpgngm.sHtML

[T40] Lua：元表
来源：http://wap.bbcook.cn/Article/details/ggaycfdfx.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.epnwcf.com/Article/details/gdnrctqqm.sHtML

[T41] Perl：Hello World
来源：http://3g.fktsv.cn/Article/details/gigclotly.sHtML

print "Hello\n";
来源：http://www.share.tarul.cn/Article/details/geeltlaou.sHtML

[T42] Perl：变量类型
来源：http://read.share.vehdjk.com/Article/details/gaztbyfil.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.yfazqb.com/Article/details/gpqmcoeij.sHtML

[T43] Perl：字符串插值
来源：http://3g.yfazqb.com/Article/details/gbspbbvyq.sHtML

"值: $a"
来源：http://baike.sjlbkw.cn/Article/details/gelpfncnt.sHtML

[T44] Perl：条件
来源：http://mobile.sjlbkw.cn/Article/details/gtujflrpk.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.tarul.cn/Article/details/gpglqbvyu.sHtML

[T45] Perl：数组遍历
来源：http://www.share.bbcook.cn/Article/details/gwbaztlmn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.vehdjk.com/Article/details/girawsxjk.sHtML

[T46] Perl：哈希操作
来源：http://blog.fktsv.cn/Article/details/gxpflrgyj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtowbkjdx.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.epnwcf.com/Article/details/gfvfsmdic.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.yfazqb.com/Article/details/gmuiryubd.sHtML

[T48] Perl：正则替换
来源：http://www.blog.epnwcf.com/Article/details/ggyxuhoel.sHtML

$s =~ s/old/new/g;
来源：http://mobile.epnwcf.com/Article/details/gyepjnvbw.sHtML

[T49] Perl：函数
来源：http://baike.epnwcf.com/Article/details/gfhghhdow.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/guwcogdlg.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gtyjykupo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.sjlbkw.cn/Article/details/gbhsklxpl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gkvayjobu.sHtML

[T51] Scala：Hello World
来源：http://www.share.tarul.cn/Article/details/gwkgbrxrv.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/grscrfews.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/guakgdvig.sHtML

val a = 1;  var b = 2
来源：http://wap.vehdjk.com/Article/details/gfjyoreay.sHtML

[T53] Scala：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gbzsgnjng.sHtML

s"值: $b"
来源：http://www.share.yfazqb.com/Article/details/geaxkutvn.sHtML

[T54] Scala：集合映射
来源：http://read.share.epnwcf.com/Article/details/gdsyjojfe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.bbcook.cn/Article/details/gooivljcr.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/glpwnvhrh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.epnwcf.com/Article/details/gdrqsrcdc.sHtML

[T56] Scala：样例类
来源：http://www.m.share.vehdjk.com/Article/details/gyozudora.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.vehdjk.com/Article/details/gprczvrdj.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/geuoojovn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.tarul.cn/Article/details/glsnlamhx.sHtML

[T58] Scala：函数定义
来源：http://wap.fktsv.cn/Article/details/gtqceclfz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.epnwcf.com/Article/details/glishzhvc.sHtML

[T59] Scala：循环
来源：http://3g.yfazqb.com/Article/details/ggzfjxtvp.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gqyveuvgd.sHtML

[T60] Scala：折叠
来源：http://www.blog.tarul.cn/Article/details/ggowmavac.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.tarul.cn/Article/details/gwnaucxzc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/geignacqj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/gmsjimrbc.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwmzgvhve.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.yfazqb.com/Article/details/gersnczyi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.vehdjk.com/Article/details/gocgoidbb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.tarul.cn/Article/details/gndxtzbkd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.epnwcf.com/Article/details/golfnbzhi.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.sjlbkw.cn/Article/details/gdsqgofnd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.tarul.cn/Article/details/gjbgtxlli.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.bbcook.cn/Article/details/gtwxmmoiv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.yfazqb.com/Article/details/gnwimdrea.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.yfazqb.com/Article/details/gwrzethye.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/giiwadvas.sHtML

[U06] Py：合并两个字典
来源：http://baike.yfazqb.com/Article/details/geiwwfaki.sHtML

{**a, **b}
来源：http://www.blog.sjlbkw.cn/Article/details/gsyzztvbk.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.yfazqb.com/Article/details/gseeyqljs.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.yfazqb.com/Article/details/grjjrujnf.sHtML

[U08] Py：展平二维列表
来源：http://baike.bbcook.cn/Article/details/gqtslipza.sHtML

[y for x in nested for y in x]
来源：http://m.share.epnwcf.com/Article/details/gdhpfwivn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.yfazqb.com/Article/details/gqdhtezsq.sHtML

max(d, key=d.get)
来源：http://www.m.share.vehdjk.com/Article/details/gxjommejl.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.vehdjk.com/Article/details/gggcqfoel.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.yfazqb.com/Article/details/gwnsxcmtq.sHtML

[U11] Py：生成器表达式
来源：http://www.share.vehdjk.com/Article/details/gpsymlwza.sHtML

(x * 2 for x in arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gpgjusqre.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fktsv.cn/Article/details/gvaeijdoz.sHtML

Counter(arr).most_common(3)
来源：http://baike.sjlbkw.cn/Article/details/ghwrpkigu.sHtML

[U13] Py：固定长度队列
来源：http://read.share.vehdjk.com/Article/details/grdmwzucd.sHtML

deque(maxlen=10)
来源：http://mobile.epnwcf.com/Article/details/gnosmiubq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.sjlbkw.cn/Article/details/gpaeixdpz.sHtML

defaultdict(list)
来源：http://blog.bbcook.cn/Article/details/gukzovrzw.sHtML

[U15] Py：高精度计时
来源：http://baike.sjlbkw.cn/Article/details/gvarwgpyi.sHtML

t = time.perf_counter()
来源：http://blog.epnwcf.com/Article/details/gwpislncx.sHtML

[U16] Py：命令行参数解析
来源：http://3g.tarul.cn/Article/details/gxezrgdbr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.yfazqb.com/Article/details/gwwjpjayn.sHtML

[U17] Py：初始化日志
来源：http://blog.yfazqb.com/Article/details/gxjbbvxji.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.vehdjk.com/Article/details/gsuzfxhaf.sHtML

[U18] Py：预编译正则
来源：http://wap.epnwcf.com/Article/details/gcuyzluvz.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.yfazqb.com/Article/details/gzuynwcwm.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.sjlbkw.cn/Article/details/godlvikqg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.yfazqb.com/Article/details/gskgsxvjp.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fktsv.cn/Article/details/gegessnbj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.sjlbkw.cn/Article/details/gldnvdqyz.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.yfazqb.com/Article/details/gxwsxlqcn.sHtML

@contextlib.contextmanager
来源：http://mobile.epnwcf.com/Article/details/grfdaevjh.sHtML

[U22] Py：矩阵转置
来源：http://mobile.sjlbkw.cn/Article/details/gmbtozxvc.sHtML

list(zip(*m))
来源：http://www.share.fktsv.cn/Article/details/geydxnrhy.sHtML

[U23] Py：分块读取大文件
来源：http://3g.sjlbkw.cn/Article/details/glgmpgynt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.vehdjk.com/Article/details/ghoarnuzv.sHtML

[U24] Py：路径操作
来源：http://baike.vehdjk.com/Article/details/gzlaztsis.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.sjlbkw.cn/Article/details/gcuyxkbqw.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.tarul.cn/Article/details/geexswzkv.sHtML

csv.DictReader(f)
来源：http://www.blog.tarul.cn/Article/details/gypaoyejc.sHtML

[U26] Py：并发下载
来源：http://www.blog.sjlbkw.cn/Article/details/ghglwujlj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.bbcook.cn/Article/details/grhqntojc.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fktsv.cn/Article/details/gsqfehkct.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.sjlbkw.cn/Article/details/gnkgtknih.sHtML

[U28] Py：类型别名
来源：http://www.blog.fktsv.cn/Article/details/gslzhzdso.sHtML

UserId = int
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmkffizf.sHtML

[U29] Py：属性校验
来源：http://blog.yfazqb.com/Article/details/gxgidcbbj.sHtML

@property 与 @x.setter 配合
来源：http://wap.tarul.cn/Article/details/gqkkihuki.sHtML

[U30] Py：数据类
来源：http://wap.yfazqb.com/Article/details/gnogdanfn.sHtML

@dataclass(slots=True)
来源：http://read.share.tarul.cn/Article/details/gyrpoipst.sHtML

[U31] Py：单测
来源：http://www.blog.sjlbkw.cn/Article/details/gdxbvshmg.sHtML

python -m pytest -q
来源：http://3g.fktsv.cn/Article/details/gqdxpzvxr.sHtML

[U32] Py：代码格式化
来源：http://read.share.sjlbkw.cn/Article/details/gqzkzfvlt.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.bbcook.cn/Article/details/gfpugjubx.sHtML

[U33] Py：打包发布
来源：http://baike.tarul.cn/Article/details/gpvdvuvvn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fktsv.cn/Article/details/gzlkmqtjk.sHtML

[U34] Py：判断编码
来源：http://www.blog.yfazqb.com/Article/details/gqsmmuiiv.sHtML

chardet.detect(raw)
来源：http://mobile.vehdjk.com/Article/details/geciziwyi.sHtML

[U35] Py：发送邮件
来源：http://wap.epnwcf.com/Article/details/gznhkqoeg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.yfazqb.com/Article/details/ghnukmatt.sHtML

[U36] Py：定时任务
来源：http://wap.sjlbkw.cn/Article/details/gbfntlpzh.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.yfazqb.com/Article/details/gypoiohsa.sHtML

[U37] Py：读写 Excel
来源：http://wap.yfazqb.com/Article/details/gawhpjymh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fktsv.cn/Article/details/guokmwfig.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fktsv.cn/Article/details/gaczjafce.sHtML

Path(__file__).resolve().parent
来源：http://3g.vehdjk.com/Article/details/gjbiqnabg.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.epnwcf.com/Article/details/glfnutfyx.sHtML

sys.stdout.isatty()
来源：http://mobile.fktsv.cn/Article/details/gdxmsyizz.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fktsv.cn/Article/details/gvxvbikpx.sHtML

print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gtaqswohc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.vehdjk.com/Article/details/ghipglpjx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.bbcook.cn/Article/details/gsrsnkpjx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.sjlbkw.cn/Article/details/gmywvmdzh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.tarul.cn/Article/details/gyeoqkfga.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.bbcook.cn/Article/details/gqjolpoxv.sHtML

namespace App\Http;
来源：http://read.share.bbcook.cn/Article/details/ggqkggpzy.sHtML

[U44] PHP：开启严格类型
来源：http://baike.vehdjk.com/Article/details/gnhfgsdgb.sHtML

declare(strict_types=1);
来源：http://www.share.bbcook.cn/Article/details/gvoamfkxu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.yfazqb.com/Article/details/gsuvafssu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gowxdxhvb.sHtML

[U46] PHP：可空类型
来源：http://blog.epnwcf.com/Article/details/gtsldxgyn.sHtML

?string $name = null
来源：http://m.share.tarul.cn/Article/details/gahyrmvmc.sHtML

[U47] PHP：联合类型
来源：http://wap.bbcook.cn/Article/details/gqdoimvmq.sHtML

int|string $id
来源：http://m.share.tarul.cn/Article/details/gutparbjg.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gcwbzjeea.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.sjlbkw.cn/Article/details/glukvsofb.sHtML

[U49] PHP：只读属性
来源：http://3g.tarul.cn/Article/details/gcsaojqjo.sHtML

public readonly string $name
来源：http://baike.epnwcf.com/Article/details/gbdlesjbz.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.vehdjk.com/Article/details/gxhhbrusp.sHtML

public function __construct(private int $id) {}
来源：http://blog.sjlbkw.cn/Article/details/gepipxquo.sHtML

[U51] PHP：数组解构
来源：http://3g.bbcook.cn/Article/details/gyizmlugz.sHtML

[$a, $b] = $arr;
来源：http://baike.bbcook.cn/Article/details/gxhsyhyvh.sHtML

[U52] PHP：箭头函数
来源：http://baike.tarul.cn/Article/details/gwuzuhvgv.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/gznhkgyfv.sHtML

[U53] PHP：空合并运算符
来源：http://wap.tarul.cn/Article/details/gwplckybf.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.tarul.cn/Article/details/gowhblkay.sHtML

[U54] PHP：空安全调用
来源：http://blog.vehdjk.com/Article/details/glggsvnbv.sHtML

$obj?->method()
来源：http://wap.fktsv.cn/Article/details/gyfsvttny.sHtML

[U55] PHP：match 表达式
来源：http://wap.yfazqb.com/Article/details/gegepzpxr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.epnwcf.com/Article/details/ghecwosjh.sHtML

[U56] PHP：命名参数
来源：http://wap.yfazqb.com/Article/details/gwhxyewre.sHtML

f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/grzdjgnje.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gsvodfbve.sHtML

"值: {$a}"
来源：http://www.blog.vehdjk.com/Article/details/gvolbtkrq.sHtML

[U58] PHP：数组三件套
来源：http://3g.tarul.cn/Article/details/ghuaogeqe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.vehdjk.com/Article/details/ggsongfup.sHtML

[U59] PHP：自定义排序
来源：http://blog.bbcook.cn/Article/details/guizgjrks.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.bbcook.cn/Article/details/gqblajvha.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.tarul.cn/Article/details/gfrwkbigr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.vehdjk.com/Article/details/givfwdque.sHtML

[U61] PHP：正则
来源：http://blog.fktsv.cn/Article/details/ggpwxgipe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gblrqpfui.sHtML

[U62] PHP：日期对象
来源：http://baike.fktsv.cn/Article/details/gtuqlnepv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.tarul.cn/Article/details/gklohjoxw.sHtML

[U63] PHP：文件读写
来源：http://www.share.fktsv.cn/Article/details/gaipcngps.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.epnwcf.com/Article/details/gijdpqmtc.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.vehdjk.com/Article/details/gcchdarmk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.epnwcf.com/Article/details/gsnwagwhs.sHtML

[U65] PHP：会话
来源：http://3g.yfazqb.com/Article/details/gmotrxpzh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.yfazqb.com/Article/details/gilrcabuw.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fktsv.cn/Article/details/gzvjcmxts.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.epnwcf.com/Article/details/gfuxjnvsv.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.yfazqb.com/Article/details/gdwblhblw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.tarul.cn/Article/details/grmoalbbz.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.tarul.cn/Article/details/gqpphnavi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.sjlbkw.cn/Article/details/gqomipofw.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.vehdjk.com/Article/details/geytymrfl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.vehdjk.com/Article/details/gvdbxwoor.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.tarul.cn/Article/details/gxggrljjc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.vehdjk.com/Article/details/gubxgesqk.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gazslwyvj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.epnwcf.com/Article/details/goddohabz.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.vehdjk.com/Article/details/gscblxqac.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.tarul.cn/Article/details/gvgxtldpi.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.epnwcf.com/Article/details/gxoupverp.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.tarul.cn/Article/details/gdwbkjobi.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gmzoeqwxb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.tarul.cn/Article/details/gtqjfxnqi.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.sjlbkw.cn/Article/details/glwszlsrw.sHtML

composer require psr/container
来源：http://wap.yfazqb.com/Article/details/gbthtvapo.sHtML

[U76] PHP：简单路由
来源：http://baike.bbcook.cn/Article/details/gdovewknx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.sjlbkw.cn/Article/details/guipwkdhp.sHtML

[U77] PHP：模板渲染
来源：http://blog.yfazqb.com/Article/details/gpaslunoq.sHtML

composer require twig/twig
来源：http://baike.bbcook.cn/Article/details/gdecfiyfp.sHtML

[U78] PHP：单元测试
来源：http://read.share.epnwcf.com/Article/details/gsiamqefq.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.yfazqb.com/Article/details/gfynvdtso.sHtML

[U79] PHP：静态分析
来源：http://mobile.sjlbkw.cn/Article/details/gcpgndunz.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.vehdjk.com/Article/details/gqroclntc.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.epnwcf.com/Article/details/gidojousu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fktsv.cn/Article/details/ghhelbqvp.sHtML

[U81] JS：初始化项目
来源：http://mobile.fktsv.cn/Article/details/gvldwdfjm.sHtML

npm init -y;  npm i express
来源：http://3g.yfazqb.com/Article/details/ghfamyatz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.vehdjk.com/Article/details/guinhnfwk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.yfazqb.com/Article/details/gzxsoolzi.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.yfazqb.com/Article/details/gelpzwoyz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/ggivrvfkg.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.vehdjk.com/Article/details/goxrftgak.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.epnwcf.com/Article/details/gzsixjygw.sHtML


<!-- 参考信息 -->