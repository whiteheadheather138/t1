代发 wailian999

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/ghbjxehwv.sHtML

"值: $b"
来源：http://mobile.bbcook.cn/Article/details/grdxkwkev.sHtML

[T04] Kotlin：空安全
来源：http://mobile.vehdjk.com/Article/details/ggubineoz.sHtML

val n: String? = null;  n?.length
来源：http://m.share.bbcook.cn/Article/details/gjufxdyho.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.yfazqb.com/Article/details/gmfbyxdzq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/gyczrqrin.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gqypbvycz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fktsv.cn/Article/details/gvcxksdnv.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.yfazqb.com/Article/details/glocugsdi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.bbcook.cn/Article/details/gdoingcvy.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/galhooosi.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fktsv.cn/Article/details/gfrfayrod.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.yfazqb.com/Article/details/gkywwiryd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fktsv.cn/Article/details/gokhwojmb.sHtML

[T10] Kotlin：默认参数
来源：http://wap.epnwcf.com/Article/details/gqwdqmuqi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.tarul.cn/Article/details/gepwkxmqn.sHtML

[T11] Kotlin：协程
来源：http://blog.sjlbkw.cn/Article/details/gqdhqvtkl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fktsv.cn/Article/details/glpowyuay.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.yfazqb.com/Article/details/gpbxbydmn.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fktsv.cn/Article/details/gqskspxpr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fktsv.cn/Article/details/ghtikybkh.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fktsv.cn/Article/details/givsnoffd.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/gtfaputqm.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gxjerqxpn.sHtML

[T15] Kotlin：接口
来源：http://blog.vehdjk.com/Article/details/gzjllrqri.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.epnwcf.com/Article/details/gubbkcocc.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gnypfkhuk.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gltzdxwge.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fktsv.cn/Article/details/gylsxyxxd.sHtML

var a = 1;  let b = 2
来源：http://www.blog.vehdjk.com/Article/details/gnthbhmea.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/gyohwvype.sHtML

"值: \(b)"
来源：http://read.share.yfazqb.com/Article/details/gebtqpbbn.sHtML

[T19] Swift：可选绑定
来源：http://read.share.vehdjk.com/Article/details/gmxnfhcyx.sHtML

if let n = opt { print(n) }
来源：http://3g.yfazqb.com/Article/details/gvfggpiht.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fktsv.cn/Article/details/ghxynewit.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fktsv.cn/Article/details/gdjnumyrz.sHtML

[T21] Swift：遍历
来源：http://www.share.vehdjk.com/Article/details/gkhrlzjay.sHtML

for x in a { print(x) }
来源：http://3g.epnwcf.com/Article/details/gdxddythr.sHtML

[T22] Swift：字典
来源：http://wap.epnwcf.com/Article/details/gnyevpocx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.bbcook.cn/Article/details/giazshehv.sHtML

[T23] Swift：函数
来源：http://baike.yfazqb.com/Article/details/gmfwqsapc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.tarul.cn/Article/details/gfpbnckdk.sHtML

[T24] Swift：闭包
来源：http://mobile.vehdjk.com/Article/details/guxxnulig.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gwlwqadzk.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/gxpepdilr.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/gdunhzcpt.sHtML

[T26] Swift：类与重写
来源：http://baike.bbcook.cn/Article/details/ghrgeofqj.sHtML

class A: Base { override func f() {} }
来源：http://3g.bbcook.cn/Article/details/gyribtzvr.sHtML

[T27] Swift：错误处理
来源：http://blog.epnwcf.com/Article/details/gkfvpbnzq.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fktsv.cn/Article/details/gbzjprqqe.sHtML

[T28] Swift：枚举
来源：http://www.share.tarul.cn/Article/details/geslclpge.sHtML

enum Color { case red, green }
来源：http://wap.tarul.cn/Article/details/gpouvgxxu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.bbcook.cn/Article/details/gmvlpoipq.sHtML

guard let x = opt else { return }
来源：http://baike.bbcook.cn/Article/details/gagmfyvwm.sHtML

[T30] Swift：协议
来源：http://www.share.epnwcf.com/Article/details/guiakigjm.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.tarul.cn/Article/details/gqdemxfvg.sHtML

[T31] Lua：Hello World
来源：http://www.share.yfazqb.com/Article/details/guklizvdq.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/gekdffsms.sHtML

[T32] Lua：局部变量
来源：http://mobile.sjlbkw.cn/Article/details/gzyfklpxc.sHtML

local a = 1
来源：http://m.share.yfazqb.com/Article/details/gfuwbmjrr.sHtML

[T33] Lua：表（数组）
来源：http://read.share.epnwcf.com/Article/details/gyfrvboko.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.vehdjk.com/Article/details/gvudafmea.sHtML

[T34] Lua：遍历表
来源：http://www.blog.sjlbkw.cn/Article/details/gnoqnioxc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fktsv.cn/Article/details/gnpzenjcw.sHtML

[T35] Lua：字典表
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcrlklyw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.vehdjk.com/Article/details/grtxcjixd.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/gqmybbqxs.sHtML

function add(a, b) return a + b end
来源：http://blog.sjlbkw.cn/Article/details/ghprdhxcm.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fktsv.cn/Article/details/gyouiecye.sHtML

"a" .. "b"
来源：http://baike.fktsv.cn/Article/details/gmmelpckk.sHtML

[T38] Lua：条件
来源：http://3g.yfazqb.com/Article/details/gcqmfzjgm.sHtML

if x > 0 then print("正") end
来源：http://mobile.epnwcf.com/Article/details/gifxexmif.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.bbcook.cn/Article/details/gwrjkgqxg.sHtML

string.find(s, "%d+")
来源：http://3g.vehdjk.com/Article/details/goheugxmw.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/gjywlqwer.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.yfazqb.com/Article/details/gdrisogid.sHtML

[T41] Perl：Hello World
来源：http://mobile.bbcook.cn/Article/details/ghtzxwzny.sHtML

print "Hello\n";
来源：http://m.share.epnwcf.com/Article/details/gqzlkxgaa.sHtML

[T42] Perl：变量类型
来源：http://m.share.epnwcf.com/Article/details/gzhbkryqt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.vehdjk.com/Article/details/gpnkpzgub.sHtML

[T43] Perl：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gbopgbxdg.sHtML

"值: $a"
来源：http://www.blog.tarul.cn/Article/details/gabhblbqv.sHtML

[T44] Perl：条件
来源：http://m.share.tarul.cn/Article/details/gbqvkopts.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fktsv.cn/Article/details/gjdynfnru.sHtML

[T45] Perl：数组遍历
来源：http://mobile.yfazqb.com/Article/details/gxebitczp.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.sjlbkw.cn/Article/details/gozssbedf.sHtML

[T46] Perl：哈希操作
来源：http://www.share.sjlbkw.cn/Article/details/geudtiqep.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.yfazqb.com/Article/details/gmpvtqugm.sHtML

[T47] Perl：正则捕获
来源：http://baike.fktsv.cn/Article/details/gxhvllslr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.bbcook.cn/Article/details/grivkeety.sHtML

[T48] Perl：正则替换
来源：http://wap.epnwcf.com/Article/details/gwqykzkuf.sHtML

$s =~ s/old/new/g;
来源：http://wap.tarul.cn/Article/details/gnfmsthxv.sHtML

[T49] Perl：函数
来源：http://read.share.fktsv.cn/Article/details/gvkphdxic.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gigdzikmw.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gvterotyw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.epnwcf.com/Article/details/glbwifdss.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fktsv.cn/Article/details/gdvsxwulr.sHtML

[T51] Scala：Hello World
来源：http://read.share.tarul.cn/Article/details/gsyetrpaz.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/ggznsstoq.sHtML

[T52] Scala：变量
来源：http://www.m.share.bbcook.cn/Article/details/gxkpfzafj.sHtML

val a = 1;  var b = 2
来源：http://wap.vehdjk.com/Article/details/gpxkkswmv.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gciljamrv.sHtML

s"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gzeymqgrl.sHtML

[T54] Scala：集合映射
来源：http://mobile.tarul.cn/Article/details/gtnbtwtfj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.epnwcf.com/Article/details/gxzvtwyas.sHtML

[T55] Scala：集合过滤
来源：http://mobile.epnwcf.com/Article/details/ghelypcjh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fktsv.cn/Article/details/giusyoesx.sHtML

[T56] Scala：样例类
来源：http://wap.sjlbkw.cn/Article/details/gmoefzhmo.sHtML

case class User(name: String, age: Int)
来源：http://baike.epnwcf.com/Article/details/gclygtmiq.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/gbqiyraqs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.bbcook.cn/Article/details/gsidejwii.sHtML

[T58] Scala：函数定义
来源：http://www.blog.yfazqb.com/Article/details/gzwbhvtnv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.bbcook.cn/Article/details/gdyclbtjz.sHtML

[T59] Scala：循环
来源：http://baike.bbcook.cn/Article/details/gfxdygeou.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.tarul.cn/Article/details/gixttitjq.sHtML

[T60] Scala：折叠
来源：http://www.share.tarul.cn/Article/details/gufknebue.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.yfazqb.com/Article/details/gqltexcpx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gusfzxstl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.sjlbkw.cn/Article/details/gtswdwwkw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gscwprhwz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fktsv.cn/Article/details/gododryuu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gszcgxjlm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.bbcook.cn/Article/details/gpnvqxvyo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.vehdjk.com/Article/details/grpalbpkf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.epnwcf.com/Article/details/gyfkrqmgd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/glxupretb.sHtML

[U04] Py：变量调试打印
来源：http://mobile.tarul.cn/Article/details/gnklkokyf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.epnwcf.com/Article/details/gvirfbezz.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.epnwcf.com/Article/details/gltjrapix.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/goriiqfwb.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.epnwcf.com/Article/details/gadotrhso.sHtML

{**a, **b}
来源：http://blog.tarul.cn/Article/details/gepwluvyw.sHtML

[U07] Py：反转字典键值
来源：http://wap.vehdjk.com/Article/details/gbrwjbkvy.sHtML

{v: k for k, v in d.items()}
来源：http://3g.tarul.cn/Article/details/gjowispjm.sHtML

[U08] Py：展平二维列表
来源：http://baike.fktsv.cn/Article/details/gxngmgrvy.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.bbcook.cn/Article/details/gwdvbjggr.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.tarul.cn/Article/details/gmicfjgzz.sHtML

max(d, key=d.get)
来源：http://wap.sjlbkw.cn/Article/details/gdtvcjkkc.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbgtuooo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.sjlbkw.cn/Article/details/gphfsksjn.sHtML

[U11] Py：生成器表达式
来源：http://baike.bbcook.cn/Article/details/gonrvgxoy.sHtML

(x * 2 for x in arr)
来源：http://wap.sjlbkw.cn/Article/details/gtevmqrae.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.epnwcf.com/Article/details/ggyciubph.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.vehdjk.com/Article/details/giijxldlw.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfhlqdsc.sHtML

deque(maxlen=10)
来源：http://baike.yfazqb.com/Article/details/gknecptag.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.vehdjk.com/Article/details/gtvkloraj.sHtML

defaultdict(list)
来源：http://3g.bbcook.cn/Article/details/gbmnbpbut.sHtML

[U15] Py：高精度计时
来源：http://www.blog.tarul.cn/Article/details/gakeyjeab.sHtML

t = time.perf_counter()
来源：http://blog.epnwcf.com/Article/details/gbojwjzpd.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fktsv.cn/Article/details/gaeunpeup.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fktsv.cn/Article/details/gyfbwenbu.sHtML

[U17] Py：初始化日志
来源：http://mobile.sjlbkw.cn/Article/details/gsnuuwbbs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.yfazqb.com/Article/details/gmzustuyx.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.tarul.cn/Article/details/gpukbamgj.sHtML

pat = re.compile(r"\d+")
来源：http://3g.bbcook.cn/Article/details/gvzfntqcr.sHtML

[U19] Py：正则替换带回调
来源：http://baike.sjlbkw.cn/Article/details/gkigbkmzm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.bbcook.cn/Article/details/gpnlvxtwr.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.sjlbkw.cn/Article/details/gflbwetfe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.bbcook.cn/Article/details/gnyrcssro.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.vehdjk.com/Article/details/gmjkcvnmz.sHtML

@contextlib.contextmanager
来源：http://blog.vehdjk.com/Article/details/gmyywrnng.sHtML

[U22] Py：矩阵转置
来源：http://wap.tarul.cn/Article/details/gbupezwek.sHtML

list(zip(*m))
来源：http://wap.yfazqb.com/Article/details/gakgsiorm.sHtML

[U23] Py：分块读取大文件
来源：http://baike.sjlbkw.cn/Article/details/gzyywzyvk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.vehdjk.com/Article/details/gajpzmjpx.sHtML

[U24] Py：路径操作
来源：http://3g.epnwcf.com/Article/details/gperxxiry.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/gbzweyvuk.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.tarul.cn/Article/details/gmcnwomai.sHtML

csv.DictReader(f)
来源：http://www.m.share.epnwcf.com/Article/details/giwxumbnx.sHtML

[U26] Py：并发下载
来源：http://read.share.sjlbkw.cn/Article/details/gyyjfgccq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.vehdjk.com/Article/details/gvzlmgvug.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.bbcook.cn/Article/details/gynwsukqs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.bbcook.cn/Article/details/gdtpitfoq.sHtML

[U28] Py：类型别名
来源：http://wap.vehdjk.com/Article/details/gmvcnkagc.sHtML

UserId = int
来源：http://3g.epnwcf.com/Article/details/gqiekgrkg.sHtML

[U29] Py：属性校验
来源：http://wap.bbcook.cn/Article/details/gidfzdiwm.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fktsv.cn/Article/details/gxilynbvk.sHtML

[U30] Py：数据类
来源：http://www.m.share.epnwcf.com/Article/details/gpacbbzmh.sHtML

@dataclass(slots=True)
来源：http://m.share.tarul.cn/Article/details/gjhyrrxuy.sHtML

[U31] Py：单测
来源：http://www.share.bbcook.cn/Article/details/gmulqsgpx.sHtML

python -m pytest -q
来源：http://baike.fktsv.cn/Article/details/gndgrilbd.sHtML

[U32] Py：代码格式化
来源：http://mobile.vehdjk.com/Article/details/ggwvxakdq.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.tarul.cn/Article/details/gbswgecdc.sHtML

[U33] Py：打包发布
来源：http://m.share.sjlbkw.cn/Article/details/glwreayyq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.sjlbkw.cn/Article/details/gxuxkkqie.sHtML

[U34] Py：判断编码
来源：http://wap.fktsv.cn/Article/details/gsyfazcxl.sHtML

chardet.detect(raw)
来源：http://mobile.sjlbkw.cn/Article/details/gkoafqffc.sHtML

[U35] Py：发送邮件
来源：http://www.blog.tarul.cn/Article/details/glvafyasq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.tarul.cn/Article/details/gzmzdlhuk.sHtML

[U36] Py：定时任务
来源：http://read.share.tarul.cn/Article/details/gwskcywmv.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fktsv.cn/Article/details/ggichwojw.sHtML

[U37] Py：读写 Excel
来源：http://wap.tarul.cn/Article/details/gnmbmfzjz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.yfazqb.com/Article/details/gfhmljyej.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.sjlbkw.cn/Article/details/ggeseaphh.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.bbcook.cn/Article/details/gmmzphziv.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.tarul.cn/Article/details/gotxunhqi.sHtML

sys.stdout.isatty()
来源：http://m.share.bbcook.cn/Article/details/gwedqusyy.sHtML

[U40] Py：打印到标准错误
来源：http://baike.bbcook.cn/Article/details/gorhookfy.sHtML

print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/gfxnswlwa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.epnwcf.com/Article/details/ghzdahtrv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.vehdjk.com/Article/details/gipdggmtl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fktsv.cn/Article/details/ggymhpyto.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.epnwcf.com/Article/details/glpaixoxf.sHtML

[U43] PHP：声明命名空间
来源：http://wap.epnwcf.com/Article/details/gbombemlf.sHtML

namespace App\Http;
来源：http://www.share.tarul.cn/Article/details/gygldagjg.sHtML

[U44] PHP：开启严格类型
来源：http://blog.sjlbkw.cn/Article/details/gerslegzg.sHtML

declare(strict_types=1);
来源：http://blog.epnwcf.com/Article/details/gczltttnt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.tarul.cn/Article/details/gaghfetnb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gmxrvkdsi.sHtML

[U46] PHP：可空类型
来源：http://3g.fktsv.cn/Article/details/gmebsbbyj.sHtML

?string $name = null
来源：http://3g.bbcook.cn/Article/details/gvzhadaxo.sHtML

[U47] PHP：联合类型
来源：http://www.share.epnwcf.com/Article/details/gcwwfquoo.sHtML

int|string $id
来源：http://www.share.epnwcf.com/Article/details/gfsrmmvjd.sHtML

[U48] PHP：纯枚举
来源：http://wap.sjlbkw.cn/Article/details/grnbfjuut.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fktsv.cn/Article/details/gimhrcrdb.sHtML

[U49] PHP：只读属性
来源：http://m.share.epnwcf.com/Article/details/gfmfkrrvk.sHtML

public readonly string $name
来源：http://blog.bbcook.cn/Article/details/gmaihcojs.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.epnwcf.com/Article/details/gmqynjgli.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gjjqhsixt.sHtML

[U51] PHP：数组解构
来源：http://www.share.vehdjk.com/Article/details/gxgqwxres.sHtML

[$a, $b] = $arr;
来源：http://www.blog.sjlbkw.cn/Article/details/gnztbxzmx.sHtML

[U52] PHP：箭头函数
来源：http://3g.yfazqb.com/Article/details/gntvdugpl.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.epnwcf.com/Article/details/gdxxicfhb.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.sjlbkw.cn/Article/details/gcrplkkdi.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.bbcook.cn/Article/details/gihssukiv.sHtML

[U54] PHP：空安全调用
来源：http://www.share.epnwcf.com/Article/details/grdttwkvb.sHtML

$obj?->method()
来源：http://baike.sjlbkw.cn/Article/details/greijogyo.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fktsv.cn/Article/details/ggbcfvrcw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fktsv.cn/Article/details/gacadyyby.sHtML

[U56] PHP：命名参数
来源：http://wap.bbcook.cn/Article/details/gjcyoyfwk.sHtML

f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gzexooryo.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gtapjjmjv.sHtML

"值: {$a}"
来源：http://mobile.fktsv.cn/Article/details/gxejchfko.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.epnwcf.com/Article/details/guzqcdgzy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.tarul.cn/Article/details/gtjqnedhf.sHtML

[U59] PHP：自定义排序
来源：http://read.share.bbcook.cn/Article/details/gxdymjyyu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gwonsvmcw.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.epnwcf.com/Article/details/gfxlireza.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.vehdjk.com/Article/details/gxfzqgizv.sHtML

[U61] PHP：正则
来源：http://www.share.epnwcf.com/Article/details/gifkzwozy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/gnwqbztel.sHtML

[U62] PHP：日期对象
来源：http://www.blog.bbcook.cn/Article/details/gljmtegiw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.sjlbkw.cn/Article/details/gduuwhrlq.sHtML

[U63] PHP：文件读写
来源：http://m.share.vehdjk.com/Article/details/gbdoxwoar.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fktsv.cn/Article/details/gmmkwqmge.sHtML

[U64] PHP：目录遍历
来源：http://blog.epnwcf.com/Article/details/grlmpieyq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.bbcook.cn/Article/details/gdfxjbvzi.sHtML

[U65] PHP：会话
来源：http://blog.yfazqb.com/Article/details/gdpynoekg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.tarul.cn/Article/details/gustoaoex.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.bbcook.cn/Article/details/gplluruqz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.tarul.cn/Article/details/grmwaldtb.sHtML

[U67] PHP：处理文件上传
来源：http://blog.bbcook.cn/Article/details/gzpuqoveg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fktsv.cn/Article/details/gxsyheyiq.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdkbmdhf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fktsv.cn/Article/details/gmifryqea.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.bbcook.cn/Article/details/ghlmxwkeq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.epnwcf.com/Article/details/gyepjlmiy.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fktsv.cn/Article/details/gcnbqqabq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.bbcook.cn/Article/details/gfdbsjbbe.sHtML

[U71] PHP：抛出异常
来源：http://baike.bbcook.cn/Article/details/gkqnjprom.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.tarul.cn/Article/details/gkflxvirs.sHtML

[U72] PHP：写错误日志
来源：http://wap.sjlbkw.cn/Article/details/gfqhhoaik.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.epnwcf.com/Article/details/gevrbreri.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.yfazqb.com/Article/details/ggjhswnhd.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.bbcook.cn/Article/details/gxfatzlif.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gmprbdupt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.yfazqb.com/Article/details/gfxgldlim.sHtML

[U75] PHP：依赖注入
来源：http://blog.yfazqb.com/Article/details/ghdiwartu.sHtML

composer require psr/container
来源：http://3g.sjlbkw.cn/Article/details/gwumkogpp.sHtML

[U76] PHP：简单路由
来源：http://read.share.bbcook.cn/Article/details/goylnpfql.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.tarul.cn/Article/details/gyfisvlkw.sHtML

[U77] PHP：模板渲染
来源：http://read.share.yfazqb.com/Article/details/gbuggnihs.sHtML

composer require twig/twig
来源：http://read.share.yfazqb.com/Article/details/gvisxlcdt.sHtML

[U78] PHP：单元测试
来源：http://3g.bbcook.cn/Article/details/gpavbpthd.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.bbcook.cn/Article/details/gxtbbfiia.sHtML

[U79] PHP：静态分析
来源：http://mobile.bbcook.cn/Article/details/ggrhoyiuj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.sjlbkw.cn/Article/details/gcqlffzjg.sHtML

[U80] PHP：代码规范修复
来源：http://wap.vehdjk.com/Article/details/gypgpfofq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.tarul.cn/Article/details/gpvmbzaod.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.tarul.cn/Article/details/gfxfufaje.sHtML

npm init -y;  npm i express
来源：http://read.share.fktsv.cn/Article/details/gxpyupjla.sHtML

[U82] JS：package.json 脚本
来源：http://3g.vehdjk.com/Article/details/gntitqpcj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.vehdjk.com/Article/details/geotfwxvs.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.yfazqb.com/Article/details/gdjkodhjw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.tarul.cn/Article/details/gdhbsbcsf.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.bbcook.cn/Article/details/gdzioasit.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.yfazqb.com/Article/details/gbxkkeiqg.sHtML

[U85] JS：可选链
来源：http://www.share.bbcook.cn/Article/details/gocujaqrn.sHtML

a?.b?.c
来源：http://blog.yfazqb.com/Article/details/gsifxdpzo.sHtML

[U86] JS：空值合并
来源：http://www.blog.fktsv.cn/Article/details/gloxeumxh.sHtML

a ?? b
来源：http://wap.vehdjk.com/Article/details/gnkgrfvll.sHtML

[U87] JS：解构默认值
来源：http://mobile.epnwcf.com/Article/details/gnqiwghgr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.tarul.cn/Article/details/gevngsczh.sHtML

[U88] JS：对象展开合并
来源：http://baike.vehdjk.com/Article/details/gduvzabyd.sHtML

{ ...a, ...b }
来源：http://www.share.tarul.cn/Article/details/gkzkvrpet.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fktsv.cn/Article/details/gddothtkl.sHtML

[...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gjfknekiz.sHtML

[U90] JS：数字数组排序
来源：http://blog.sjlbkw.cn/Article/details/gcfmeeomq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gkgmmswcn.sHtML


<!-- 参考信息 -->