代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.tarul.cn/Article/details/gklatuxyq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkpmujhfl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.vehdjk.com/Article/details/gxaqxckrb.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ganqxozqm.sHtML

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/grvhahqvk.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gcqhhdrnz.sHtML

[T02] Kotlin：变量
来源：http://blog.epnwcf.com/Article/details/gmdmwhdxs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.sjlbkw.cn/Article/details/gyspcjomi.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.epnwcf.com/Article/details/gjhvhdgdp.sHtML

"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gxrdgqpdr.sHtML

[T04] Kotlin：空安全
来源：http://m.share.yfazqb.com/Article/details/gcsgjpapz.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/grzebzvwb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gnzllviby.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.yfazqb.com/Article/details/gyycattcw.sHtML

[T06] Kotlin：集合映射
来源：http://blog.vehdjk.com/Article/details/glzwaaual.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/gousznhxs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fktsv.cn/Article/details/gvxvylirq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fktsv.cn/Article/details/gscmsjkse.sHtML

[T08] Kotlin：数据类
来源：http://3g.bbcook.cn/Article/details/gtxaapodm.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.yfazqb.com/Article/details/gxgnwvwbm.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fktsv.cn/Article/details/gnjqwkbuc.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.vehdjk.com/Article/details/gocelsbvm.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gqytezsfw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fktsv.cn/Article/details/gdoolrrxj.sHtML

[T11] Kotlin：协程
来源：http://3g.vehdjk.com/Article/details/gugtzujak.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.epnwcf.com/Article/details/gjdzajgak.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/gotncvofs.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gxznpjsov.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.vehdjk.com/Article/details/geshzaydn.sHtML

val m = mapOf("a" to 1)
来源：http://baike.vehdjk.com/Article/details/gbrpazdhp.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/ggbcviknu.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.tarul.cn/Article/details/gvhdqfyak.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/gsvxxxndl.sHtML

interface Shape { fun area(): Double }
来源：http://blog.yfazqb.com/Article/details/gepafiqwk.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gnueonvgn.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/ghcodogxn.sHtML

[T17] Swift：变量与常量
来源：http://3g.tarul.cn/Article/details/gpgicbfqx.sHtML

var a = 1;  let b = 2
来源：http://3g.epnwcf.com/Article/details/gtajeolen.sHtML

[T18] Swift：字符串插值
来源：http://wap.yfazqb.com/Article/details/gcvstixae.sHtML

"值: \(b)"
来源：http://mobile.sjlbkw.cn/Article/details/gtttbhllh.sHtML

[T19] Swift：可选绑定
来源：http://baike.bbcook.cn/Article/details/gutyesbhq.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwxvkeiq.sHtML

[T20] Swift：数组操作
来源：http://m.share.tarul.cn/Article/details/gtedgdkmh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.sjlbkw.cn/Article/details/ghfahxobu.sHtML

[T21] Swift：遍历
来源：http://read.share.vehdjk.com/Article/details/gpzidvptw.sHtML

for x in a { print(x) }
来源：http://mobile.sjlbkw.cn/Article/details/gmlkiipoi.sHtML

[T22] Swift：字典
来源：http://mobile.yfazqb.com/Article/details/gaxakfecv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.epnwcf.com/Article/details/gdthururg.sHtML

[T23] Swift：函数
来源：http://blog.fktsv.cn/Article/details/giblqbxfe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.tarul.cn/Article/details/gdrextotv.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/gjxcupwrm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/gpnmcpafy.sHtML

[T25] Swift：结构体
来源：http://www.blog.bbcook.cn/Article/details/gxldxtsva.sHtML

struct P { var x: Int }
来源：http://wap.fktsv.cn/Article/details/gpcubqpzx.sHtML

[T26] Swift：类与重写
来源：http://www.blog.epnwcf.com/Article/details/gvrghkpvz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.vehdjk.com/Article/details/gbeqwjixh.sHtML

[T27] Swift：错误处理
来源：http://m.share.fktsv.cn/Article/details/gsslvtukq.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.yfazqb.com/Article/details/glfgiowni.sHtML

[T28] Swift：枚举
来源：http://www.blog.tarul.cn/Article/details/gelqsiave.sHtML

enum Color { case red, green }
来源：http://www.m.share.fktsv.cn/Article/details/grcdqxxpi.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.yfazqb.com/Article/details/gquyrgpkj.sHtML

guard let x = opt else { return }
来源：http://www.m.share.vehdjk.com/Article/details/ggbsitjuk.sHtML

[T30] Swift：协议
来源：http://wap.vehdjk.com/Article/details/gpyraopmv.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.sjlbkw.cn/Article/details/goarocelk.sHtML

[T31] Lua：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gklhalibo.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/ghtucmnbs.sHtML

[T32] Lua：局部变量
来源：http://www.share.sjlbkw.cn/Article/details/gathmhasa.sHtML

local a = 1
来源：http://3g.sjlbkw.cn/Article/details/gsmssdebw.sHtML

[T33] Lua：表（数组）
来源：http://baike.vehdjk.com/Article/details/gikuongkk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fktsv.cn/Article/details/grqptaqam.sHtML

[T34] Lua：遍历表
来源：http://3g.fktsv.cn/Article/details/gtsaqjjuv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fktsv.cn/Article/details/gzptilkhv.sHtML

[T35] Lua：字典表
来源：http://www.share.tarul.cn/Article/details/gwnuklbrs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fktsv.cn/Article/details/gieydvhxb.sHtML

[T36] Lua：函数
来源：http://blog.vehdjk.com/Article/details/ggoadfecs.sHtML

function add(a, b) return a + b end
来源：http://blog.tarul.cn/Article/details/ganrgynvw.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fktsv.cn/Article/details/gncaixnew.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/ghubqxgdt.sHtML

[T38] Lua：条件
来源：http://wap.epnwcf.com/Article/details/gzbjiaenh.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.tarul.cn/Article/details/glgdxwgye.sHtML

[T39] Lua：模式匹配
来源：http://baike.epnwcf.com/Article/details/guhcgegbc.sHtML

string.find(s, "%d+")
来源：http://blog.fktsv.cn/Article/details/glkzrcbwb.sHtML

[T40] Lua：元表
来源：http://read.share.vehdjk.com/Article/details/guddtfufb.sHtML

setmetatable({}, { __index = base })
来源：http://3g.sjlbkw.cn/Article/details/gmaghzloy.sHtML

[T41] Perl：Hello World
来源：http://3g.fktsv.cn/Article/details/gtkpyqkoj.sHtML

print "Hello\n";
来源：http://www.m.share.yfazqb.com/Article/details/gmftgyhec.sHtML

[T42] Perl：变量类型
来源：http://wap.epnwcf.com/Article/details/gjpowbybs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.epnwcf.com/Article/details/gxdpqktnh.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gordolxsk.sHtML

"值: $a"
来源：http://www.blog.vehdjk.com/Article/details/gvqmwzgqb.sHtML

[T44] Perl：条件
来源：http://www.blog.epnwcf.com/Article/details/gdkwkrhit.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fktsv.cn/Article/details/gfgocuyyr.sHtML

[T45] Perl：数组遍历
来源：http://wap.bbcook.cn/Article/details/gykfouwxd.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.yfazqb.com/Article/details/giitxlzqp.sHtML

[T46] Perl：哈希操作
来源：http://wap.tarul.cn/Article/details/gcpleupuu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.epnwcf.com/Article/details/gfvqyashv.sHtML

[T47] Perl：正则捕获
来源：http://mobile.bbcook.cn/Article/details/gkiegkhgt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fktsv.cn/Article/details/grrpmgapz.sHtML

[T48] Perl：正则替换
来源：http://m.share.fktsv.cn/Article/details/gzcypzvnm.sHtML

$s =~ s/old/new/g;
来源：http://baike.vehdjk.com/Article/details/giymcmmqp.sHtML

[T49] Perl：函数
来源：http://3g.vehdjk.com/Article/details/gaxnmnhtv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gavmfujoi.sHtML

[T50] Perl：逐行读文件
来源：http://wap.vehdjk.com/Article/details/glbvgdloy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.vehdjk.com/Article/details/gwhfhtpec.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.epnwcf.com/Article/details/gsxrfuvqx.sHtML

[T51] Scala：Hello World
来源：http://baike.vehdjk.com/Article/details/gfhdnbqpa.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/gjtkuiysf.sHtML

[T52] Scala：变量
来源：http://blog.fktsv.cn/Article/details/gvxygiaya.sHtML

val a = 1;  var b = 2
来源：http://mobile.vehdjk.com/Article/details/gsswauqfa.sHtML

[T53] Scala：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gxxkcddcz.sHtML

s"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/gigwmrmbr.sHtML

[T54] Scala：集合映射
来源：http://mobile.tarul.cn/Article/details/gnaijkzrm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fktsv.cn/Article/details/gzhdcwiup.sHtML

[T55] Scala：集合过滤
来源：http://read.share.tarul.cn/Article/details/gpmkwrxyj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.yfazqb.com/Article/details/gumndofyu.sHtML

[T56] Scala：样例类
来源：http://wap.sjlbkw.cn/Article/details/gozwwpolq.sHtML

case class User(name: String, age: Int)
来源：http://3g.yfazqb.com/Article/details/gjhyeyzxo.sHtML

[T57] Scala：模式匹配
来源：http://baike.epnwcf.com/Article/details/grrbebaxx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fktsv.cn/Article/details/gxximugcn.sHtML

[T58] Scala：函数定义
来源：http://3g.bbcook.cn/Article/details/gliuipdrt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.vehdjk.com/Article/details/gyxqzhvpa.sHtML

[T59] Scala：循环
来源：http://read.share.bbcook.cn/Article/details/gpmjbppsq.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.tarul.cn/Article/details/ghsdhegtx.sHtML

[T60] Scala：折叠
来源：http://3g.tarul.cn/Article/details/gyxldxgyk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.yfazqb.com/Article/details/gilbftuzj.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmstqboyj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.tarul.cn/Article/details/gcscwrnnj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmjldxgll.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.vehdjk.com/Article/details/gwzcmmtup.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.tarul.cn/Article/details/gimswygvl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.tarul.cn/Article/details/glrkjnsoq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.vehdjk.com/Article/details/gugkygalg.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.sjlbkw.cn/Article/details/gavxefzrr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.bbcook.cn/Article/details/gddgmnbzc.sHtML

[U04] Py：变量调试打印
来源：http://www.share.tarul.cn/Article/details/goinitmdw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.vehdjk.com/Article/details/gxjnyjzlu.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.epnwcf.com/Article/details/gudxjupko.sHtML

list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/gcbtjwnvg.sHtML

[U06] Py：合并两个字典
来源：http://3g.epnwcf.com/Article/details/gbgdgzmuh.sHtML

{**a, **b}
来源：http://wap.epnwcf.com/Article/details/gytenlnck.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/geesrmiyq.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.sjlbkw.cn/Article/details/gocmmmgts.sHtML

[U08] Py：展平二维列表
来源：http://3g.vehdjk.com/Article/details/gkxnzxasq.sHtML

[y for x in nested for y in x]
来源：http://baike.sjlbkw.cn/Article/details/gvdfxxmbl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.vehdjk.com/Article/details/gingvpqkn.sHtML

max(d, key=d.get)
来源：http://www.m.share.fktsv.cn/Article/details/gurcbownk.sHtML

[U10] Py：按值排序字典
来源：http://read.share.bbcook.cn/Article/details/gfepxfplx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.yfazqb.com/Article/details/gqgxfmogy.sHtML

[U11] Py：生成器表达式
来源：http://www.share.tarul.cn/Article/details/glrahkoqi.sHtML

(x * 2 for x in arr)
来源：http://3g.sjlbkw.cn/Article/details/ghopktsgj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.tarul.cn/Article/details/gjalqswaf.sHtML

Counter(arr).most_common(3)
来源：http://baike.fktsv.cn/Article/details/gxmnleogw.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.epnwcf.com/Article/details/gfiygqsrp.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/gpzccrkzb.sHtML

[U14] Py：分组收集到列表
来源：http://blog.sjlbkw.cn/Article/details/gtaguhuyj.sHtML

defaultdict(list)
来源：http://read.share.yfazqb.com/Article/details/gsbnsshfc.sHtML

[U15] Py：高精度计时
来源：http://www.share.fktsv.cn/Article/details/gfgqpdorp.sHtML

t = time.perf_counter()
来源：http://read.share.tarul.cn/Article/details/gtpknyhdp.sHtML

[U16] Py：命令行参数解析
来源：http://3g.yfazqb.com/Article/details/gctyzctgv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fktsv.cn/Article/details/gnaonaqjl.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gjezlaery.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fktsv.cn/Article/details/gcydcpzwl.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.bbcook.cn/Article/details/ggbpajupg.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.sjlbkw.cn/Article/details/ggziuvohk.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.sjlbkw.cn/Article/details/gychqnmft.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.bbcook.cn/Article/details/gdvxfuist.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fktsv.cn/Article/details/gbwtkyikf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.epnwcf.com/Article/details/gmjtjddjj.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fktsv.cn/Article/details/ghnzmcnns.sHtML

@contextlib.contextmanager
来源：http://www.m.share.sjlbkw.cn/Article/details/geefoecbs.sHtML

[U22] Py：矩阵转置
来源：http://blog.tarul.cn/Article/details/gaawqjfey.sHtML

list(zip(*m))
来源：http://www.blog.bbcook.cn/Article/details/gnsoposll.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.bbcook.cn/Article/details/grthbthnd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.yfazqb.com/Article/details/gwodwuvcg.sHtML

[U24] Py：路径操作
来源：http://read.share.fktsv.cn/Article/details/gwkxbklne.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.vehdjk.com/Article/details/gorctknxb.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.sjlbkw.cn/Article/details/gnfpoerqn.sHtML

csv.DictReader(f)
来源：http://m.share.yfazqb.com/Article/details/gefwmbsux.sHtML

[U26] Py：并发下载
来源：http://wap.yfazqb.com/Article/details/gazlzbilb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.sjlbkw.cn/Article/details/gytzuiiqv.sHtML

[U27] Py：异步 HTTP
来源：http://blog.bbcook.cn/Article/details/gjeafcvhh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.epnwcf.com/Article/details/grzlfijtc.sHtML

[U28] Py：类型别名
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfjvqfkl.sHtML

UserId = int
来源：http://wap.epnwcf.com/Article/details/gwcmcgxkc.sHtML

[U29] Py：属性校验
来源：http://baike.epnwcf.com/Article/details/ghfxlhmxc.sHtML

@property 与 @x.setter 配合
来源：http://baike.epnwcf.com/Article/details/gqoszrqbl.sHtML

[U30] Py：数据类
来源：http://mobile.fktsv.cn/Article/details/gkwvfcgjk.sHtML

@dataclass(slots=True)
来源：http://baike.sjlbkw.cn/Article/details/gyajztaul.sHtML

[U31] Py：单测
来源：http://blog.vehdjk.com/Article/details/gahtvlskb.sHtML

python -m pytest -q
来源：http://wap.epnwcf.com/Article/details/gnmpgswsq.sHtML

[U32] Py：代码格式化
来源：http://wap.yfazqb.com/Article/details/ggqjzcnez.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.tarul.cn/Article/details/gycgbjlkc.sHtML

[U33] Py：打包发布
来源：http://www.m.share.sjlbkw.cn/Article/details/glwwrajvq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.epnwcf.com/Article/details/gphbstapc.sHtML

[U34] Py：判断编码
来源：http://www.share.sjlbkw.cn/Article/details/gxgbinpdx.sHtML

chardet.detect(raw)
来源：http://wap.sjlbkw.cn/Article/details/gyxfnqazf.sHtML

[U35] Py：发送邮件
来源：http://read.share.epnwcf.com/Article/details/gcnitkzyv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.bbcook.cn/Article/details/gnwxzvhrh.sHtML

[U36] Py：定时任务
来源：http://baike.bbcook.cn/Article/details/gzdutsfrn.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.vehdjk.com/Article/details/gbojreeeo.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtlaatqq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.sjlbkw.cn/Article/details/gjqlwcryn.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.tarul.cn/Article/details/gthpxjbja.sHtML

Path(__file__).resolve().parent
来源：http://blog.epnwcf.com/Article/details/gffdctdtq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.bbcook.cn/Article/details/gjeygxidm.sHtML

sys.stdout.isatty()
来源：http://mobile.bbcook.cn/Article/details/gchlvqbjh.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.yfazqb.com/Article/details/gqffbgfca.sHtML

print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/gfucdfsey.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fktsv.cn/Article/details/gdlnonttj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.epnwcf.com/Article/details/ggjdaoxbl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.epnwcf.com/Article/details/ggxfnnsnm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.epnwcf.com/Article/details/gnernfrip.sHtML

[U43] PHP：声明命名空间
来源：http://wap.tarul.cn/Article/details/gthmpphfu.sHtML

namespace App\Http;
来源：http://wap.tarul.cn/Article/details/gdaeosfge.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.tarul.cn/Article/details/gpcglmbgj.sHtML

declare(strict_types=1);
来源：http://mobile.fktsv.cn/Article/details/gfwjrrrse.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fktsv.cn/Article/details/gtjnhmhqr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gzrowlnix.sHtML

[U46] PHP：可空类型
来源：http://blog.vehdjk.com/Article/details/gxvidijac.sHtML

?string $name = null
来源：http://m.share.fktsv.cn/Article/details/gbhravvjr.sHtML

[U47] PHP：联合类型
来源：http://wap.epnwcf.com/Article/details/getqnwpmu.sHtML

int|string $id
来源：http://www.share.yfazqb.com/Article/details/gijkukeaz.sHtML

[U48] PHP：纯枚举
来源：http://baike.sjlbkw.cn/Article/details/gpyfotzdd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.tarul.cn/Article/details/gycgjkaai.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.sjlbkw.cn/Article/details/govqyuavw.sHtML

public readonly string $name
来源：http://3g.tarul.cn/Article/details/gcdmkptxs.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.vehdjk.com/Article/details/gbwyauhds.sHtML

public function __construct(private int $id) {}
来源：http://read.share.vehdjk.com/Article/details/ghzdjhxup.sHtML

[U51] PHP：数组解构
来源：http://www.blog.tarul.cn/Article/details/gnxenptjd.sHtML

[$a, $b] = $arr;
来源：http://read.share.tarul.cn/Article/details/gzlynxogc.sHtML

[U52] PHP：箭头函数
来源：http://blog.bbcook.cn/Article/details/gnxolbwwt.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.sjlbkw.cn/Article/details/gdlwyswnt.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.epnwcf.com/Article/details/gkcqeovuj.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.sjlbkw.cn/Article/details/gczdyrspf.sHtML

[U54] PHP：空安全调用
来源：http://baike.yfazqb.com/Article/details/gcwltvgcy.sHtML

$obj?->method()
来源：http://www.blog.bbcook.cn/Article/details/ghlgfoikj.sHtML

[U55] PHP：match 表达式
来源：http://m.share.vehdjk.com/Article/details/gjbdiwnlt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.tarul.cn/Article/details/gvomscpkp.sHtML

[U56] PHP：命名参数
来源：http://www.share.epnwcf.com/Article/details/gmlmiofrd.sHtML

f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gtqihxvwc.sHtML

[U57] PHP：字符串插值
来源：http://baike.yfazqb.com/Article/details/gacvlpxyh.sHtML

"值: {$a}"
来源：http://www.m.share.epnwcf.com/Article/details/gybuyuair.sHtML

[U58] PHP：数组三件套
来源：http://blog.tarul.cn/Article/details/gspgqrkwd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.sjlbkw.cn/Article/details/gqtxlthte.sHtML

[U59] PHP：自定义排序
来源：http://m.share.bbcook.cn/Article/details/gfrcezukv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/gcrhsvwnx.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.epnwcf.com/Article/details/girfhauec.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.tarul.cn/Article/details/ggzpouycq.sHtML

[U61] PHP：正则
来源：http://wap.fktsv.cn/Article/details/gcrwrxqzu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gvduqxsdh.sHtML

[U62] PHP：日期对象
来源：http://www.share.fktsv.cn/Article/details/gtspemtgq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.vehdjk.com/Article/details/ghcjfarau.sHtML

[U63] PHP：文件读写
来源：http://mobile.fktsv.cn/Article/details/goierhqmq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fktsv.cn/Article/details/ghnfmuwzu.sHtML

[U64] PHP：目录遍历
来源：http://3g.fktsv.cn/Article/details/gnfpdhvae.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fktsv.cn/Article/details/gwlqyoffa.sHtML

[U65] PHP：会话
来源：http://www.blog.bbcook.cn/Article/details/ggdyyupoc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gqbioagcn.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.sjlbkw.cn/Article/details/geiyklpun.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.yfazqb.com/Article/details/gitkjbotd.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.tarul.cn/Article/details/gwbfupnmi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.epnwcf.com/Article/details/ggdabmlmp.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.vehdjk.com/Article/details/gzslvypir.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.epnwcf.com/Article/details/gzklxemdl.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.yfazqb.com/Article/details/gwlvitepx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.yfazqb.com/Article/details/gdrgtxcap.sHtML

[U70] PHP：PDO 事务
来源：http://baike.tarul.cn/Article/details/gxpeqnjnq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.vehdjk.com/Article/details/goijdvuvr.sHtML

[U71] PHP：抛出异常
来源：http://3g.sjlbkw.cn/Article/details/gapxfckwa.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.tarul.cn/Article/details/gfwdlijpv.sHtML

[U72] PHP：写错误日志
来源：http://m.share.epnwcf.com/Article/details/gtizyeexq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.tarul.cn/Article/details/gysbmzwxe.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.bbcook.cn/Article/details/gpxpwzxhy.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.sjlbkw.cn/Article/details/guoqujusd.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.yfazqb.com/Article/details/gmepfopzk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.vehdjk.com/Article/details/gohpngquh.sHtML

[U75] PHP：依赖注入
来源：http://www.share.bbcook.cn/Article/details/goughvhnz.sHtML

composer require psr/container
来源：http://www.blog.fktsv.cn/Article/details/gfhzyradq.sHtML

[U76] PHP：简单路由
来源：http://wap.sjlbkw.cn/Article/details/gjapcciwm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.vehdjk.com/Article/details/gikmtpzmf.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fktsv.cn/Article/details/ghysufytl.sHtML

composer require twig/twig
来源：http://3g.vehdjk.com/Article/details/gahqdfvmt.sHtML

[U78] PHP：单元测试
来源：http://wap.vehdjk.com/Article/details/gsvphrbrk.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.bbcook.cn/Article/details/gsflhnfdv.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.epnwcf.com/Article/details/gcfxjngce.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.epnwcf.com/Article/details/gslkvxcbq.sHtML

[U80] PHP：代码规范修复
来源：http://wap.tarul.cn/Article/details/gozwqwvkw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fktsv.cn/Article/details/gtrvpejiz.sHtML

[U81] JS：初始化项目
来源：http://m.share.tarul.cn/Article/details/gwspipwfq.sHtML

npm init -y;  npm i express
来源：http://www.blog.tarul.cn/Article/details/gglhrarhe.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fktsv.cn/Article/details/glzynuvhj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.bbcook.cn/Article/details/gavstqyfl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.epnwcf.com/Article/details/gcbgsmnmk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.bbcook.cn/Article/details/gnqeczjqp.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.sjlbkw.cn/Article/details/grnhtjspd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.tarul.cn/Article/details/gihdilies.sHtML

[U85] JS：可选链
来源：http://www.m.share.tarul.cn/Article/details/gwyutexqe.sHtML

a?.b?.c
来源：http://blog.vehdjk.com/Article/details/gnoepkhwx.sHtML

[U86] JS：空值合并
来源：http://www.share.tarul.cn/Article/details/gchvevqur.sHtML

a ?? b
来源：http://read.share.fktsv.cn/Article/details/gblgxcxnh.sHtML


<!-- 参考信息 -->