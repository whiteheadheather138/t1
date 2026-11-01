代发 wailian999

[T05] Kotlin：when 表达式
来源：http://baike.yfazqb.com/Article/details/gzzuhjcje.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.yfazqb.com/Article/details/gcgzmjzrs.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gqobopybf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/guwopyjfg.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fktsv.cn/Article/details/gxkhwhrkj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.vehdjk.com/Article/details/gsnvtdymo.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fktsv.cn/Article/details/gymaragnk.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.tarul.cn/Article/details/gyzfsyhar.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/glzjrfdpq.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.yfazqb.com/Article/details/geoxbhpxh.sHtML

[T10] Kotlin：默认参数
来源：http://blog.sjlbkw.cn/Article/details/gltwyfaob.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/gotfcgjrj.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fktsv.cn/Article/details/gtwcupagu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.yfazqb.com/Article/details/gicnswzqo.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/gpbolruwg.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.epnwcf.com/Article/details/giijariff.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gssjiqlmw.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.vehdjk.com/Article/details/gdzpikijn.sHtML

[T14] Kotlin：循环
来源：http://m.share.fktsv.cn/Article/details/gqnxaddjd.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/gwlsmxoun.sHtML

[T15] Kotlin：接口
来源：http://blog.sjlbkw.cn/Article/details/glkqsfguq.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/gtnijkeic.sHtML

[T16] Swift：Hello World
来源：http://3g.epnwcf.com/Article/details/grwokzjpf.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gnezgkego.sHtML

[T17] Swift：变量与常量
来源：http://blog.fktsv.cn/Article/details/gkdxlrlnp.sHtML

var a = 1;  let b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gifatmemi.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gcjirjfzx.sHtML

"值: \(b)"
来源：http://blog.tarul.cn/Article/details/gjadafiwe.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlvlcipl.sHtML

if let n = opt { print(n) }
来源：http://mobile.tarul.cn/Article/details/gxuwosetj.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fktsv.cn/Article/details/gaqkeuvdt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/gvcyeofza.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/gidyrhmxl.sHtML

for x in a { print(x) }
来源：http://blog.tarul.cn/Article/details/gpkjptoll.sHtML

[T22] Swift：字典
来源：http://m.share.vehdjk.com/Article/details/grmgwrmhv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/gpsmasqvk.sHtML

[T23] Swift：函数
来源：http://www.blog.epnwcf.com/Article/details/gczavtlqx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.vehdjk.com/Article/details/gbvqyvelk.sHtML

[T24] Swift：闭包
来源：http://m.share.yfazqb.com/Article/details/gxmpoaoxs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.tarul.cn/Article/details/gcbgnflps.sHtML

[T25] Swift：结构体
来源：http://m.share.bbcook.cn/Article/details/gmwexmdpv.sHtML

struct P { var x: Int }
来源：http://mobile.tarul.cn/Article/details/gqcuymvog.sHtML

[T26] Swift：类与重写
来源：http://m.share.sjlbkw.cn/Article/details/gqkitbqhw.sHtML

class A: Base { override func f() {} }
来源：http://mobile.tarul.cn/Article/details/ghasgfhsi.sHtML

[T27] Swift：错误处理
来源：http://3g.sjlbkw.cn/Article/details/gjwynirbp.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.bbcook.cn/Article/details/gvhmkigbi.sHtML

[T28] Swift：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gmeqxwjcb.sHtML

enum Color { case red, green }
来源：http://read.share.yfazqb.com/Article/details/gljgjhsvy.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.sjlbkw.cn/Article/details/gsvfezfmj.sHtML

guard let x = opt else { return }
来源：http://mobile.tarul.cn/Article/details/gwofvrktt.sHtML

[T30] Swift：协议
来源：http://blog.bbcook.cn/Article/details/gfllnsxrw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.bbcook.cn/Article/details/gwdozpvqu.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gclastzlx.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/ggvckqtbt.sHtML

[T32] Lua：局部变量
来源：http://3g.tarul.cn/Article/details/gtgrceues.sHtML

local a = 1
来源：http://www.share.yfazqb.com/Article/details/gzpnajeii.sHtML

[T33] Lua：表（数组）
来源：http://baike.bbcook.cn/Article/details/gvnytdnic.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.bbcook.cn/Article/details/ggzccfpqy.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gqykdxcru.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.yfazqb.com/Article/details/gskuqswqv.sHtML

[T35] Lua：字典表
来源：http://blog.epnwcf.com/Article/details/gxzwhwhsp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.epnwcf.com/Article/details/gonytjjqk.sHtML

[T36] Lua：函数
来源：http://m.share.yfazqb.com/Article/details/gdxifipuo.sHtML

function add(a, b) return a + b end
来源：http://3g.yfazqb.com/Article/details/gaturscnw.sHtML

[T37] Lua：字符串拼接
来源：http://3g.tarul.cn/Article/details/garpfbpps.sHtML

"a" .. "b"
来源：http://3g.sjlbkw.cn/Article/details/gytavnzkn.sHtML

[T38] Lua：条件
来源：http://baike.yfazqb.com/Article/details/gycqfqrbu.sHtML

if x > 0 then print("正") end
来源：http://wap.epnwcf.com/Article/details/ghpazhmpv.sHtML

[T39] Lua：模式匹配
来源：http://3g.tarul.cn/Article/details/gagycanzm.sHtML

string.find(s, "%d+")
来源：http://mobile.tarul.cn/Article/details/gedxknwtv.sHtML

[T40] Lua：元表
来源：http://www.m.share.fktsv.cn/Article/details/gwgqvvcfp.sHtML

setmetatable({}, { __index = base })
来源：http://wap.sjlbkw.cn/Article/details/gqkxsxcap.sHtML

[T41] Perl：Hello World
来源：http://mobile.bbcook.cn/Article/details/gawpqualm.sHtML

print "Hello\n";
来源：http://blog.sjlbkw.cn/Article/details/gfbafmkgo.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.bbcook.cn/Article/details/geltwbivv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.epnwcf.com/Article/details/gfhetcxnl.sHtML

[T43] Perl：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gkzpdkcbd.sHtML

"值: $a"
来源：http://read.share.vehdjk.com/Article/details/goypyhswa.sHtML

[T44] Perl：条件
来源：http://mobile.epnwcf.com/Article/details/gxnnakbki.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/geappuvkw.sHtML

[T45] Perl：数组遍历
来源：http://blog.tarul.cn/Article/details/gfwdwjyjr.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.sjlbkw.cn/Article/details/gboerpnsa.sHtML

[T46] Perl：哈希操作
来源：http://mobile.sjlbkw.cn/Article/details/gwmhqqxmn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.epnwcf.com/Article/details/gnbfwltkl.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.yfazqb.com/Article/details/gmvtnrpeg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.tarul.cn/Article/details/gnwvmuaww.sHtML

[T48] Perl：正则替换
来源：http://mobile.sjlbkw.cn/Article/details/gmobaznsu.sHtML

$s =~ s/old/new/g;
来源：http://mobile.yfazqb.com/Article/details/gitlujeif.sHtML

[T49] Perl：函数
来源：http://mobile.sjlbkw.cn/Article/details/gadrnkquz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/ghmuudxav.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gfnxuxhmb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.bbcook.cn/Article/details/gggrysyyz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.tarul.cn/Article/details/gwvpffrdr.sHtML

[T51] Scala：Hello World
来源：http://www.blog.tarul.cn/Article/details/ghaykafrv.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gdetitfod.sHtML

[T52] Scala：变量
来源：http://baike.fktsv.cn/Article/details/gyjzoaidg.sHtML

val a = 1;  var b = 2
来源：http://wap.tarul.cn/Article/details/gdoapawnk.sHtML

[T53] Scala：字符串插值
来源：http://blog.fktsv.cn/Article/details/gtzoinmwc.sHtML

s"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gbjwlndhr.sHtML

[T54] Scala：集合映射
来源：http://baike.tarul.cn/Article/details/gfppdmhec.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.tarul.cn/Article/details/gecneqknv.sHtML

[T55] Scala：集合过滤
来源：http://blog.fktsv.cn/Article/details/gmolqthoo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gherznida.sHtML

[T56] Scala：样例类
来源：http://wap.vehdjk.com/Article/details/gumtxkcvr.sHtML

case class User(name: String, age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gszvsaqtt.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/gdzzuwcna.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.tarul.cn/Article/details/gmuwpmbuf.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.sjlbkw.cn/Article/details/glqqjvebk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.vehdjk.com/Article/details/ggqjrnnxj.sHtML

[T59] Scala：循环
来源：http://baike.sjlbkw.cn/Article/details/gjknrkldu.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gmdfbcgvd.sHtML

[T60] Scala：折叠
来源：http://3g.bbcook.cn/Article/details/gzqahrvhc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/gvqhyhpcv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gndbwfeeo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.vehdjk.com/Article/details/gvikomrtd.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gzccalsdv.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.epnwcf.com/Article/details/gqicflrbg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.epnwcf.com/Article/details/gcvrhvpkk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fktsv.cn/Article/details/ggtsrhrkf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.yfazqb.com/Article/details/gdpqmcmbi.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.yfazqb.com/Article/details/gjiaaeohp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.vehdjk.com/Article/details/gjnenevqa.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/gfbaulgif.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.yfazqb.com/Article/details/gstaqgcmv.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/gpehdgbfr.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gduidxqhj.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.sjlbkw.cn/Article/details/gpfmrdkde.sHtML

{**a, **b}
来源：http://mobile.tarul.cn/Article/details/gdqdpwpgk.sHtML

[U07] Py：反转字典键值
来源：http://mobile.vehdjk.com/Article/details/gbtexkqsy.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fktsv.cn/Article/details/guzqzadms.sHtML

[U08] Py：展平二维列表
来源：http://3g.vehdjk.com/Article/details/gvjnmmfqa.sHtML

[y for x in nested for y in x]
来源：http://baike.vehdjk.com/Article/details/gfsfeglhq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.yfazqb.com/Article/details/gujdsiejc.sHtML

max(d, key=d.get)
来源：http://m.share.epnwcf.com/Article/details/gnpozzxhw.sHtML

[U10] Py：按值排序字典
来源：http://m.share.epnwcf.com/Article/details/gcnudilee.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fktsv.cn/Article/details/gputsbqoj.sHtML

[U11] Py：生成器表达式
来源：http://www.share.sjlbkw.cn/Article/details/gwxabraog.sHtML

(x * 2 for x in arr)
来源：http://baike.fktsv.cn/Article/details/gwgljogkr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.tarul.cn/Article/details/gtzikrgsz.sHtML

Counter(arr).most_common(3)
来源：http://read.share.sjlbkw.cn/Article/details/gethuzrac.sHtML

[U13] Py：固定长度队列
来源：http://read.share.sjlbkw.cn/Article/details/gmjelgcta.sHtML

deque(maxlen=10)
来源：http://mobile.tarul.cn/Article/details/gsmkjqqlx.sHtML

[U14] Py：分组收集到列表
来源：http://wap.sjlbkw.cn/Article/details/gjaomptcr.sHtML

defaultdict(list)
来源：http://read.share.vehdjk.com/Article/details/gpgkrtdzn.sHtML

[U15] Py：高精度计时
来源：http://wap.vehdjk.com/Article/details/grctjizej.sHtML

t = time.perf_counter()
来源：http://3g.epnwcf.com/Article/details/gbexzxcfi.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.tarul.cn/Article/details/gpdypgllo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.sjlbkw.cn/Article/details/gpvxdjxae.sHtML

[U17] Py：初始化日志
来源：http://blog.tarul.cn/Article/details/gdzfmvqhn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fktsv.cn/Article/details/gkmfwiqoz.sHtML

[U18] Py：预编译正则
来源：http://www.blog.yfazqb.com/Article/details/gsqvqkdrl.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fktsv.cn/Article/details/gidtcxuiw.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.bbcook.cn/Article/details/gqrztfprk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.yfazqb.com/Article/details/gnjrjihvt.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.yfazqb.com/Article/details/gkevervuu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.yfazqb.com/Article/details/gtwmkmfrh.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.bbcook.cn/Article/details/gaaqjobau.sHtML

@contextlib.contextmanager
来源：http://read.share.vehdjk.com/Article/details/gldknfkwe.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.bbcook.cn/Article/details/ghswkcwnl.sHtML

list(zip(*m))
来源：http://www.share.vehdjk.com/Article/details/gqjzbdgon.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvbhmxew.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.yfazqb.com/Article/details/gecrtxbwx.sHtML

[U24] Py：路径操作
来源：http://mobile.sjlbkw.cn/Article/details/gzoucmuqz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/ghshopgut.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fktsv.cn/Article/details/gewroozuc.sHtML

csv.DictReader(f)
来源：http://www.blog.fktsv.cn/Article/details/gddowmaqk.sHtML

[U26] Py：并发下载
来源：http://wap.yfazqb.com/Article/details/geiarmxdv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.bbcook.cn/Article/details/gsujpxojb.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.yfazqb.com/Article/details/graupiqei.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.vehdjk.com/Article/details/gcnwchugg.sHtML

[U28] Py：类型别名
来源：http://www.share.tarul.cn/Article/details/gfbqossea.sHtML

UserId = int
来源：http://baike.tarul.cn/Article/details/gptnjjpst.sHtML

[U29] Py：属性校验
来源：http://mobile.fktsv.cn/Article/details/gsvsmbwot.sHtML

@property 与 @x.setter 配合
来源：http://www.share.bbcook.cn/Article/details/gfvedjqbn.sHtML

[U30] Py：数据类
来源：http://www.share.tarul.cn/Article/details/gcyooydpf.sHtML

@dataclass(slots=True)
来源：http://m.share.tarul.cn/Article/details/gvirgxfwk.sHtML

[U31] Py：单测
来源：http://www.m.share.bbcook.cn/Article/details/gmbezmhbz.sHtML

python -m pytest -q
来源：http://wap.epnwcf.com/Article/details/golwbkuvp.sHtML

[U32] Py：代码格式化
来源：http://3g.epnwcf.com/Article/details/gkkkgrngc.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.vehdjk.com/Article/details/gnpxnnwqe.sHtML

[U33] Py：打包发布
来源：http://www.blog.sjlbkw.cn/Article/details/gknoacnbn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.epnwcf.com/Article/details/gplovigwr.sHtML

[U34] Py：判断编码
来源：http://blog.yfazqb.com/Article/details/ghyfxvbdv.sHtML

chardet.detect(raw)
来源：http://www.m.share.tarul.cn/Article/details/gevmpojdj.sHtML

[U35] Py：发送邮件
来源：http://mobile.fktsv.cn/Article/details/gifoyvhvn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.bbcook.cn/Article/details/gtntibbzj.sHtML

[U36] Py：定时任务
来源：http://baike.epnwcf.com/Article/details/gjewrjsma.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.bbcook.cn/Article/details/gdosthuqd.sHtML

[U37] Py：读写 Excel
来源：http://3g.tarul.cn/Article/details/gveqpdpyc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.bbcook.cn/Article/details/gxplhyprs.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.bbcook.cn/Article/details/gixkamrbo.sHtML

Path(__file__).resolve().parent
来源：http://3g.epnwcf.com/Article/details/gdxxurxmy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnyeegst.sHtML

sys.stdout.isatty()
来源：http://www.m.share.tarul.cn/Article/details/gfwkyoddu.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fktsv.cn/Article/details/gojkrahsn.sHtML

print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/gqwvwpvsc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.bbcook.cn/Article/details/gbvhszvqg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.yfazqb.com/Article/details/gresmifbt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.epnwcf.com/Article/details/gdsosysss.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fktsv.cn/Article/details/gpggfjchu.sHtML

[U43] PHP：声明命名空间
来源：http://3g.sjlbkw.cn/Article/details/gtzsvefaj.sHtML

namespace App\Http;
来源：http://baike.sjlbkw.cn/Article/details/gcwuhucys.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.bbcook.cn/Article/details/gmisgwfiw.sHtML

declare(strict_types=1);
来源：http://baike.sjlbkw.cn/Article/details/gdakbyklz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.yfazqb.com/Article/details/gpfkdnbra.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gzaefwjjg.sHtML

[U46] PHP：可空类型
来源：http://www.blog.tarul.cn/Article/details/gbmmcsitp.sHtML

?string $name = null
来源：http://baike.bbcook.cn/Article/details/gtbskymar.sHtML

[U47] PHP：联合类型
来源：http://mobile.fktsv.cn/Article/details/ggeuwtguv.sHtML

int|string $id
来源：http://3g.fktsv.cn/Article/details/gwnnmdlah.sHtML

[U48] PHP：纯枚举
来源：http://mobile.yfazqb.com/Article/details/gytnphbtj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.epnwcf.com/Article/details/gualwzlkt.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.tarul.cn/Article/details/gltuwobap.sHtML

public readonly string $name
来源：http://www.blog.tarul.cn/Article/details/gatojynbm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.vehdjk.com/Article/details/gncljdbzn.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fktsv.cn/Article/details/gpojqwiuw.sHtML

[U51] PHP：数组解构
来源：http://3g.sjlbkw.cn/Article/details/gupoaptzh.sHtML

[$a, $b] = $arr;
来源：http://www.blog.tarul.cn/Article/details/gqtyoarnk.sHtML

[U52] PHP：箭头函数
来源：http://mobile.sjlbkw.cn/Article/details/gvtiehyty.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fktsv.cn/Article/details/gxicejrkq.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.epnwcf.com/Article/details/gkenoypnd.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.sjlbkw.cn/Article/details/goanypnia.sHtML

[U54] PHP：空安全调用
来源：http://baike.tarul.cn/Article/details/gmvfamvmh.sHtML

$obj?->method()
来源：http://read.share.yfazqb.com/Article/details/gmrsimdhg.sHtML

[U55] PHP：match 表达式
来源：http://read.share.tarul.cn/Article/details/ggxknlhku.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.tarul.cn/Article/details/grbqhpasw.sHtML

[U56] PHP：命名参数
来源：http://3g.tarul.cn/Article/details/gocnrnukc.sHtML

f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gkzqonvfb.sHtML

[U57] PHP：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gzhzqlcqc.sHtML

"值: {$a}"
来源：http://mobile.tarul.cn/Article/details/gnfxgyrjl.sHtML

[U58] PHP：数组三件套
来源：http://read.share.tarul.cn/Article/details/gmvdfxxqs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gnlvwkncs.sHtML

[U59] PHP：自定义排序
来源：http://3g.yfazqb.com/Article/details/gecfuzzxw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.bbcook.cn/Article/details/gockfeypr.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.bbcook.cn/Article/details/gxvzojwmz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.vehdjk.com/Article/details/gwfmdnlrw.sHtML

[U61] PHP：正则
来源：http://www.blog.fktsv.cn/Article/details/gmihchkue.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/grzxlnqtu.sHtML

[U62] PHP：日期对象
来源：http://m.share.sjlbkw.cn/Article/details/gtpenvkjt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fktsv.cn/Article/details/gabhlqisb.sHtML

[U63] PHP：文件读写
来源：http://read.share.tarul.cn/Article/details/gwgdulsir.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.bbcook.cn/Article/details/gwbsybsox.sHtML

[U64] PHP：目录遍历
来源：http://3g.fktsv.cn/Article/details/gotqwrpum.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.yfazqb.com/Article/details/gahzdatec.sHtML

[U65] PHP：会话
来源：http://wap.sjlbkw.cn/Article/details/gkjgkfrhm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/ghrbzqgvf.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.epnwcf.com/Article/details/gjmuybqau.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fktsv.cn/Article/details/gvudfetdg.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.tarul.cn/Article/details/gdghtrvdd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.tarul.cn/Article/details/gsdsewzfp.sHtML

[U68] PHP：PDO 连接
来源：http://wap.sjlbkw.cn/Article/details/gyjscyvge.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fktsv.cn/Article/details/gchtewgql.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.vehdjk.com/Article/details/gupslxsfv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fktsv.cn/Article/details/glehelfty.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.tarul.cn/Article/details/goheeroca.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.epnwcf.com/Article/details/gxjhdfmen.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/gzadglpay.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.bbcook.cn/Article/details/ggmvzmxgu.sHtML

[U72] PHP：写错误日志
来源：http://m.share.bbcook.cn/Article/details/grvqufxlh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.bbcook.cn/Article/details/getfdtupm.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.bbcook.cn/Article/details/guzzudcvw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.yfazqb.com/Article/details/ggvefynho.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.tarul.cn/Article/details/gpmuvpaas.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.epnwcf.com/Article/details/gqiacuzmd.sHtML

[U75] PHP：依赖注入
来源：http://m.share.vehdjk.com/Article/details/gxpjbmvkk.sHtML

composer require psr/container
来源：http://www.blog.fktsv.cn/Article/details/gakkiubid.sHtML

[U76] PHP：简单路由
来源：http://3g.fktsv.cn/Article/details/gwlqgcnhi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.bbcook.cn/Article/details/ghmynsfkh.sHtML

[U77] PHP：模板渲染
来源：http://www.share.sjlbkw.cn/Article/details/gsfdqrzft.sHtML

composer require twig/twig
来源：http://baike.tarul.cn/Article/details/grpxwbocy.sHtML

[U78] PHP：单元测试
来源：http://www.share.fktsv.cn/Article/details/gkjxujuec.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.epnwcf.com/Article/details/gmirgwixh.sHtML

[U79] PHP：静态分析
来源：http://wap.bbcook.cn/Article/details/gjdsxptqu.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.vehdjk.com/Article/details/gesfgdxul.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.yfazqb.com/Article/details/gdpconwsq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.vehdjk.com/Article/details/gvzrnmstf.sHtML

[U81] JS：初始化项目
来源：http://m.share.sjlbkw.cn/Article/details/gpbhbyuzp.sHtML

npm init -y;  npm i express
来源：http://read.share.tarul.cn/Article/details/guqfxpzpd.sHtML

[U82] JS：package.json 脚本
来源：http://3g.yfazqb.com/Article/details/gaayvuyfp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.sjlbkw.cn/Article/details/geefueqjf.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.tarul.cn/Article/details/ggcehqwdz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gsizeqmjb.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.yfazqb.com/Article/details/ggonnedyp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.tarul.cn/Article/details/gsjossdij.sHtML

[U85] JS：可选链
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnqouxgr.sHtML

a?.b?.c
来源：http://www.share.sjlbkw.cn/Article/details/gmyhzkzbs.sHtML

[U86] JS：空值合并
来源：http://read.share.yfazqb.com/Article/details/glxpdztww.sHtML

a ?? b
来源：http://www.m.share.sjlbkw.cn/Article/details/gghzwhllf.sHtML

[U87] JS：解构默认值
来源：http://wap.yfazqb.com/Article/details/gmkvnrden.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.epnwcf.com/Article/details/gmzyhztao.sHtML

[U88] JS：对象展开合并
来源：http://blog.tarul.cn/Article/details/gucqvkdbz.sHtML

{ ...a, ...b }
来源：http://read.share.tarul.cn/Article/details/gbzscabks.sHtML

[U89] JS：数组去重
来源：http://wap.epnwcf.com/Article/details/gxsqwbivh.sHtML

[...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gmlsaksnx.sHtML

[U90] JS：数字数组排序
来源：http://baike.epnwcf.com/Article/details/gfelvebqi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/glszqxbww.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.tarul.cn/Article/details/gqoauslry.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.epnwcf.com/Article/details/gapzlvtmx.sHtML

[U92] JS：深拷贝
来源：http://www.share.epnwcf.com/Article/details/gpnyvunyd.sHtML

structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/ghcrmvcli.sHtML


<!-- 参考信息 -->