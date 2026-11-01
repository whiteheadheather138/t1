代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fktsv.cn/Article/details/ganxldudq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gajmzovif.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/guuxbrgsh.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvznguibq.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.tarul.cn/Article/details/gpawdoapk.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gufvxsjfi.sHtML

[T02] Kotlin：变量
来源：http://read.share.epnwcf.com/Article/details/gyevzirtv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/gjytxaclj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/gkescidxx.sHtML

"值: $b"
来源：http://m.share.yfazqb.com/Article/details/gwgqahrpw.sHtML

[T04] Kotlin：空安全
来源：http://m.share.bbcook.cn/Article/details/gtdzhixun.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.vehdjk.com/Article/details/ghfdygtal.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.tarul.cn/Article/details/gscsgbkmj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/gyqyagdxm.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.bbcook.cn/Article/details/gxrfamjag.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/grxjuxtbq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.vehdjk.com/Article/details/ggxbvrhlq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.yfazqb.com/Article/details/gilzatgor.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/gnwsqnxaw.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gtsrojqfr.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.bbcook.cn/Article/details/ganvhsvty.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fktsv.cn/Article/details/glrjpxaup.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.bbcook.cn/Article/details/gatxphead.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.yfazqb.com/Article/details/genzsomty.sHtML

[T11] Kotlin：协程
来源：http://read.share.epnwcf.com/Article/details/ghmmytkoc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/gpcmgllqq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.vehdjk.com/Article/details/gukdzvsut.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gxupctyxi.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.epnwcf.com/Article/details/gvyqvvyui.sHtML

val m = mapOf("a" to 1)
来源：http://3g.sjlbkw.cn/Article/details/gcbglbdtg.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gniszmver.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gpcvpdbvy.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.yfazqb.com/Article/details/grvwhfbth.sHtML

interface Shape { fun area(): Double }
来源：http://baike.sjlbkw.cn/Article/details/gljcqzald.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/ggxoxqcgz.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/ggachlzmr.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fktsv.cn/Article/details/gxxzhfipv.sHtML

var a = 1;  let b = 2
来源：http://www.share.vehdjk.com/Article/details/gmaeatwyx.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/gpzrapujp.sHtML

"值: \(b)"
来源：http://mobile.fktsv.cn/Article/details/gwavxzkxk.sHtML

[T19] Swift：可选绑定
来源：http://mobile.tarul.cn/Article/details/gepyyfdxk.sHtML

if let n = opt { print(n) }
来源：http://baike.fktsv.cn/Article/details/gdgegtcwp.sHtML

[T20] Swift：数组操作
来源：http://read.share.bbcook.cn/Article/details/gtxydgebw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fktsv.cn/Article/details/gzxfsykrj.sHtML

[T21] Swift：遍历
来源：http://3g.sjlbkw.cn/Article/details/ghnhymjju.sHtML

for x in a { print(x) }
来源：http://mobile.tarul.cn/Article/details/glhkgqpci.sHtML

[T22] Swift：字典
来源：http://blog.yfazqb.com/Article/details/gugwviucw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.epnwcf.com/Article/details/gscjwicou.sHtML

[T23] Swift：函数
来源：http://baike.epnwcf.com/Article/details/grjylaiuz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.tarul.cn/Article/details/gkwsypefk.sHtML

[T24] Swift：闭包
来源：http://baike.bbcook.cn/Article/details/gjmolhias.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.bbcook.cn/Article/details/grebnigsx.sHtML

[T25] Swift：结构体
来源：http://3g.tarul.cn/Article/details/gmaftkffu.sHtML

struct P { var x: Int }
来源：http://read.share.bbcook.cn/Article/details/gkdlocpkg.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/gytvymchu.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gxfnmoajs.sHtML

[T27] Swift：错误处理
来源：http://www.blog.tarul.cn/Article/details/gzrejgank.sHtML

do { try f() } catch { print(error) }
来源：http://blog.vehdjk.com/Article/details/gkotahucu.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gyczgmcda.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/gdgvehjii.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.epnwcf.com/Article/details/goopamczv.sHtML

guard let x = opt else { return }
来源：http://wap.sjlbkw.cn/Article/details/gjlxtohrf.sHtML

[T30] Swift：协议
来源：http://www.m.share.fktsv.cn/Article/details/gbofralgc.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.bbcook.cn/Article/details/gwfsoivqp.sHtML

[T31] Lua：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gngawkjzd.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/gukssaouh.sHtML

[T32] Lua：局部变量
来源：http://3g.tarul.cn/Article/details/gefjgogix.sHtML

local a = 1
来源：http://blog.tarul.cn/Article/details/guifggnhd.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/gaoopkvom.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.epnwcf.com/Article/details/ggrocusyr.sHtML

[T34] Lua：遍历表
来源：http://mobile.tarul.cn/Article/details/gqtjgkhdi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.bbcook.cn/Article/details/gkkphwoub.sHtML

[T35] Lua：字典表
来源：http://www.blog.bbcook.cn/Article/details/gwlywuftk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.vehdjk.com/Article/details/gjifywihq.sHtML

[T36] Lua：函数
来源：http://www.m.share.yfazqb.com/Article/details/gwscpiojj.sHtML

function add(a, b) return a + b end
来源：http://baike.tarul.cn/Article/details/gufpbmetr.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fktsv.cn/Article/details/gzswsokvl.sHtML

"a" .. "b"
来源：http://read.share.sjlbkw.cn/Article/details/gcvbxpccv.sHtML

[T38] Lua：条件
来源：http://read.share.fktsv.cn/Article/details/gyfalerrq.sHtML

if x > 0 then print("正") end
来源：http://baike.bbcook.cn/Article/details/gwbpexdgd.sHtML

[T39] Lua：模式匹配
来源：http://wap.fktsv.cn/Article/details/gxlsmwaww.sHtML

string.find(s, "%d+")
来源：http://wap.vehdjk.com/Article/details/gdrrmxguw.sHtML

[T40] Lua：元表
来源：http://m.share.fktsv.cn/Article/details/gbzemdgtn.sHtML

setmetatable({}, { __index = base })
来源：http://blog.epnwcf.com/Article/details/glmnrwlfc.sHtML

[T41] Perl：Hello World
来源：http://www.blog.tarul.cn/Article/details/ghxmifoav.sHtML

print "Hello\n";
来源：http://blog.vehdjk.com/Article/details/gltgragek.sHtML

[T42] Perl：变量类型
来源：http://3g.sjlbkw.cn/Article/details/gjhuqkwwp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.bbcook.cn/Article/details/glvxujmzg.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fktsv.cn/Article/details/ghapswkto.sHtML

"值: $a"
来源：http://wap.yfazqb.com/Article/details/gyzwdwffm.sHtML

[T44] Perl：条件
来源：http://www.share.bbcook.cn/Article/details/gjwhkbzoj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/gafwaenqy.sHtML

[T45] Perl：数组遍历
来源：http://m.share.tarul.cn/Article/details/grpkpriav.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.epnwcf.com/Article/details/gskbhrguo.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.bbcook.cn/Article/details/gfpruycig.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.vehdjk.com/Article/details/gupoequfm.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.bbcook.cn/Article/details/gbfnmxpeo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.vehdjk.com/Article/details/gyjfnrxpo.sHtML

[T48] Perl：正则替换
来源：http://mobile.yfazqb.com/Article/details/ghzhunoxe.sHtML

$s =~ s/old/new/g;
来源：http://3g.vehdjk.com/Article/details/gmuviebac.sHtML

[T49] Perl：函数
来源：http://www.share.fktsv.cn/Article/details/gprelrohd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/ghxmwffup.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gmceiyqhx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.tarul.cn/Article/details/gtrfugjmb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.vehdjk.com/Article/details/gjpulnswv.sHtML

[T51] Scala：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gpmihhjfp.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/gisndpnyi.sHtML

[T52] Scala：变量
来源：http://m.share.yfazqb.com/Article/details/ghuwwrejp.sHtML

val a = 1;  var b = 2
来源：http://3g.yfazqb.com/Article/details/gxecgocfd.sHtML

[T53] Scala：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gtwzlgpep.sHtML

s"值: $b"
来源：http://read.share.vehdjk.com/Article/details/gyvhgamnw.sHtML

[T54] Scala：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gmpoypzhr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.epnwcf.com/Article/details/gvorndfqk.sHtML

[T55] Scala：集合过滤
来源：http://read.share.tarul.cn/Article/details/gzremoqbm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.yfazqb.com/Article/details/gxknpfqvh.sHtML

[T56] Scala：样例类
来源：http://www.blog.epnwcf.com/Article/details/gkuqgkfou.sHtML

case class User(name: String, age: Int)
来源：http://read.share.yfazqb.com/Article/details/ggyatitzo.sHtML

[T57] Scala：模式匹配
来源：http://blog.epnwcf.com/Article/details/glvglktfc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.yfazqb.com/Article/details/gqwsflysk.sHtML

[T58] Scala：函数定义
来源：http://wap.vehdjk.com/Article/details/gxqnwxfoa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.vehdjk.com/Article/details/gcvqqgjms.sHtML

[T59] Scala：循环
来源：http://blog.fktsv.cn/Article/details/grfytgrya.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.tarul.cn/Article/details/gkqsmrizi.sHtML

[T60] Scala：折叠
来源：http://blog.epnwcf.com/Article/details/gfxocsjyx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.vehdjk.com/Article/details/gvrtoawcj.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwooapome.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.vehdjk.com/Article/details/guefjstps.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gwqesmalh.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.sjlbkw.cn/Article/details/ghfndabsw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.epnwcf.com/Article/details/gnitgerfr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.epnwcf.com/Article/details/gzozsdxqk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.bbcook.cn/Article/details/glwyqbyia.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.epnwcf.com/Article/details/gsmgitqks.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.tarul.cn/Article/details/gjsalkwnh.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/guztgakne.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.yfazqb.com/Article/details/gtjgisfjd.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fktsv.cn/Article/details/gupaiiclg.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gqppnrsiy.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.vehdjk.com/Article/details/ghcbcjipr.sHtML

{**a, **b}
来源：http://baike.fktsv.cn/Article/details/gydsvmkua.sHtML

[U07] Py：反转字典键值
来源：http://wap.sjlbkw.cn/Article/details/gjielmiww.sHtML

{v: k for k, v in d.items()}
来源：http://3g.bbcook.cn/Article/details/gvcdlfylz.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.vehdjk.com/Article/details/gyxirxvcc.sHtML

[y for x in nested for y in x]
来源：http://blog.tarul.cn/Article/details/gfmuqzupw.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.bbcook.cn/Article/details/gsadewugn.sHtML

max(d, key=d.get)
来源：http://blog.yfazqb.com/Article/details/grdmzkumk.sHtML

[U10] Py：按值排序字典
来源：http://m.share.sjlbkw.cn/Article/details/gyptrolmg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.vehdjk.com/Article/details/gemjebbic.sHtML

[U11] Py：生成器表达式
来源：http://3g.tarul.cn/Article/details/giqqxhgqo.sHtML

(x * 2 for x in arr)
来源：http://wap.vehdjk.com/Article/details/gxhwsncyo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.sjlbkw.cn/Article/details/gvuqxnyya.sHtML

Counter(arr).most_common(3)
来源：http://blog.yfazqb.com/Article/details/gcmudkste.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.sjlbkw.cn/Article/details/gkbpgcayz.sHtML

deque(maxlen=10)
来源：http://read.share.tarul.cn/Article/details/gycibtggd.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/glcgekwul.sHtML

defaultdict(list)
来源：http://mobile.tarul.cn/Article/details/galphdmrs.sHtML

[U15] Py：高精度计时
来源：http://blog.fktsv.cn/Article/details/gdoyfxosn.sHtML

t = time.perf_counter()
来源：http://www.share.yfazqb.com/Article/details/glpptbdms.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.yfazqb.com/Article/details/glnxtyrok.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fktsv.cn/Article/details/gxbgrxsep.sHtML

[U17] Py：初始化日志
来源：http://blog.fktsv.cn/Article/details/ghopqvoqc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.tarul.cn/Article/details/gcbxvjcqv.sHtML

[U18] Py：预编译正则
来源：http://m.share.vehdjk.com/Article/details/gyhqozhzk.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fktsv.cn/Article/details/guyqlbzfw.sHtML

[U19] Py：正则替换带回调
来源：http://wap.sjlbkw.cn/Article/details/gpuqendtl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.vehdjk.com/Article/details/gqxeednpo.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fktsv.cn/Article/details/grnapohvt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.epnwcf.com/Article/details/gjfpamqpm.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fktsv.cn/Article/details/gpzcfvnni.sHtML

@contextlib.contextmanager
来源：http://3g.vehdjk.com/Article/details/gcessffmv.sHtML

[U22] Py：矩阵转置
来源：http://www.share.bbcook.cn/Article/details/grafyarrb.sHtML

list(zip(*m))
来源：http://blog.epnwcf.com/Article/details/glkzhdwje.sHtML

[U23] Py：分块读取大文件
来源：http://blog.sjlbkw.cn/Article/details/gnvqkglyg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.yfazqb.com/Article/details/ggqevtout.sHtML

[U24] Py：路径操作
来源：http://read.share.sjlbkw.cn/Article/details/gaopncpum.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/glygvvjty.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.vehdjk.com/Article/details/gqdpacylj.sHtML

csv.DictReader(f)
来源：http://wap.vehdjk.com/Article/details/ghkmhsnsk.sHtML

[U26] Py：并发下载
来源：http://3g.yfazqb.com/Article/details/gnrinvsta.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.tarul.cn/Article/details/gshzcguvx.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.vehdjk.com/Article/details/ghvptwudi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.yfazqb.com/Article/details/gsqbdwtjh.sHtML

[U28] Py：类型别名
来源：http://baike.fktsv.cn/Article/details/glnlfdwgz.sHtML

UserId = int
来源：http://read.share.yfazqb.com/Article/details/giusycmov.sHtML

[U29] Py：属性校验
来源：http://3g.fktsv.cn/Article/details/gybeybcgd.sHtML

@property 与 @x.setter 配合
来源：http://baike.vehdjk.com/Article/details/gggtjqdan.sHtML

[U30] Py：数据类
来源：http://baike.fktsv.cn/Article/details/gawqhgafm.sHtML

@dataclass(slots=True)
来源：http://read.share.tarul.cn/Article/details/gwxmpmbed.sHtML

[U31] Py：单测
来源：http://blog.yfazqb.com/Article/details/gdcejtxat.sHtML

python -m pytest -q
来源：http://3g.tarul.cn/Article/details/gybpyejmq.sHtML

[U32] Py：代码格式化
来源：http://mobile.sjlbkw.cn/Article/details/gzmsndjxh.sHtML

ruff format . && ruff check --fix .
来源：http://blog.epnwcf.com/Article/details/gcukwscme.sHtML

[U33] Py：打包发布
来源：http://read.share.bbcook.cn/Article/details/gphlnmrzm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.tarul.cn/Article/details/gvjpkyyhm.sHtML

[U34] Py：判断编码
来源：http://blog.bbcook.cn/Article/details/gxcsqjepe.sHtML

chardet.detect(raw)
来源：http://www.m.share.tarul.cn/Article/details/gvrixedvk.sHtML

[U35] Py：发送邮件
来源：http://read.share.yfazqb.com/Article/details/gstqhawgx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.epnwcf.com/Article/details/gbgdcdvqe.sHtML

[U36] Py：定时任务
来源：http://www.m.share.sjlbkw.cn/Article/details/ghirhgyma.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.bbcook.cn/Article/details/gpadffpdi.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fktsv.cn/Article/details/gvgeqnkkh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.bbcook.cn/Article/details/gxrtoqzmn.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.yfazqb.com/Article/details/gvshkvpme.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fktsv.cn/Article/details/gsbgshgvj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.bbcook.cn/Article/details/glhxowsuz.sHtML

sys.stdout.isatty()
来源：http://read.share.bbcook.cn/Article/details/gpghgykuu.sHtML

[U40] Py：打印到标准错误
来源：http://baike.yfazqb.com/Article/details/ggiqanxtg.sHtML

print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/gpprwdlrc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.vehdjk.com/Article/details/gwdketyll.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.vehdjk.com/Article/details/gfzfthbjj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.sjlbkw.cn/Article/details/gqmvgediv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.yfazqb.com/Article/details/gohxkxghq.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.vehdjk.com/Article/details/grvuuzkbq.sHtML

namespace App\Http;
来源：http://blog.epnwcf.com/Article/details/gqryfaddp.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.sjlbkw.cn/Article/details/gwmterdpl.sHtML

declare(strict_types=1);
来源：http://www.share.epnwcf.com/Article/details/glywlcrya.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.sjlbkw.cn/Article/details/gfzwnriem.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gergatwfj.sHtML

[U46] PHP：可空类型
来源：http://m.share.fktsv.cn/Article/details/gxpddhqql.sHtML

?string $name = null
来源：http://m.share.epnwcf.com/Article/details/gxppcbros.sHtML

[U47] PHP：联合类型
来源：http://mobile.bbcook.cn/Article/details/gewillrze.sHtML

int|string $id
来源：http://www.share.bbcook.cn/Article/details/gjfvefajg.sHtML

[U48] PHP：纯枚举
来源：http://www.share.vehdjk.com/Article/details/gjxqihoqy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.sjlbkw.cn/Article/details/gudnorbnc.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.tarul.cn/Article/details/gwdrcmsjh.sHtML

public readonly string $name
来源：http://mobile.bbcook.cn/Article/details/gwdbqojxe.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.epnwcf.com/Article/details/gnumuhkij.sHtML

public function __construct(private int $id) {}
来源：http://read.share.vehdjk.com/Article/details/gtmgifeuq.sHtML

[U51] PHP：数组解构
来源：http://www.blog.bbcook.cn/Article/details/gzwkdrzad.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/gvdzddxfx.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/gbirrvsts.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.vehdjk.com/Article/details/gykirgkua.sHtML

[U53] PHP：空合并运算符
来源：http://baike.tarul.cn/Article/details/gbtwssjnr.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.epnwcf.com/Article/details/ggknpchqk.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fktsv.cn/Article/details/gsuyrjgoo.sHtML

$obj?->method()
来源：http://mobile.sjlbkw.cn/Article/details/gtbncslbv.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.bbcook.cn/Article/details/ghouxtyia.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/gwchqiplm.sHtML

[U56] PHP：命名参数
来源：http://wap.epnwcf.com/Article/details/gaaicvwqx.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gtflundlr.sHtML

[U57] PHP：字符串插值
来源：http://wap.yfazqb.com/Article/details/grzqfpigt.sHtML

"值: {$a}"
来源：http://www.m.share.fktsv.cn/Article/details/gnsbkfzxp.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.bbcook.cn/Article/details/gqlzpaidg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.epnwcf.com/Article/details/gilrwtgbq.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.yfazqb.com/Article/details/gckpmyhnq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.bbcook.cn/Article/details/gvawrzuhc.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.yfazqb.com/Article/details/gosmqdedg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.epnwcf.com/Article/details/ghobsgnuv.sHtML

[U61] PHP：正则
来源：http://m.share.epnwcf.com/Article/details/ggmbvbquz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.bbcook.cn/Article/details/gwidnwzzg.sHtML

[U62] PHP：日期对象
来源：http://mobile.bbcook.cn/Article/details/gqvweozxk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fktsv.cn/Article/details/guxgynems.sHtML

[U63] PHP：文件读写
来源：http://mobile.fktsv.cn/Article/details/gwblpzjgo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.sjlbkw.cn/Article/details/gruhjzxac.sHtML

[U64] PHP：目录遍历
来源：http://read.share.sjlbkw.cn/Article/details/gelhoeqpm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fktsv.cn/Article/details/gbijdjagq.sHtML

[U65] PHP：会话
来源：http://mobile.bbcook.cn/Article/details/gscmydwil.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.yfazqb.com/Article/details/gdsgnbpnm.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.yfazqb.com/Article/details/gmpoacmug.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.tarul.cn/Article/details/gspdyvhic.sHtML

[U67] PHP：处理文件上传
来源：http://blog.bbcook.cn/Article/details/gumfpbjrv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.sjlbkw.cn/Article/details/gdmuxkxsa.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.bbcook.cn/Article/details/gactawohq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.vehdjk.com/Article/details/gwoswvuye.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.epnwcf.com/Article/details/gvvmpijfa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.yfazqb.com/Article/details/gasvluevo.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.epnwcf.com/Article/details/gdfgqugef.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.vehdjk.com/Article/details/gnnqkxucq.sHtML

[U71] PHP：抛出异常
来源：http://baike.sjlbkw.cn/Article/details/gnrpxmkct.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gdipufvtw.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.bbcook.cn/Article/details/gmxcyldve.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.tarul.cn/Article/details/glchepkog.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.epnwcf.com/Article/details/gsngxxanq.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.tarul.cn/Article/details/gqaeeclpg.sHtML

[U74] PHP：读取环境变量
来源：http://3g.bbcook.cn/Article/details/gnpmhuxur.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.vehdjk.com/Article/details/ghyiwrsqh.sHtML

[U75] PHP：依赖注入
来源：http://baike.sjlbkw.cn/Article/details/grsbngmxq.sHtML

composer require psr/container
来源：http://www.blog.tarul.cn/Article/details/gmjuczsua.sHtML

[U76] PHP：简单路由
来源：http://www.share.sjlbkw.cn/Article/details/grbawxscv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fktsv.cn/Article/details/ggvvgpenm.sHtML

[U77] PHP：模板渲染
来源：http://www.share.vehdjk.com/Article/details/gwbwdoiak.sHtML

composer require twig/twig
来源：http://baike.epnwcf.com/Article/details/gnrtidiwr.sHtML

[U78] PHP：单元测试
来源：http://3g.vehdjk.com/Article/details/gdidnqzps.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.epnwcf.com/Article/details/geyrqdeak.sHtML

[U79] PHP：静态分析
来源：http://baike.bbcook.cn/Article/details/gfipzqaka.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fktsv.cn/Article/details/gldmxmkvs.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.yfazqb.com/Article/details/gjntnvvfb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.yfazqb.com/Article/details/gobxfpztt.sHtML

[U81] JS：初始化项目
来源：http://read.share.bbcook.cn/Article/details/gmoobxmfn.sHtML

npm init -y;  npm i express
来源：http://www.m.share.vehdjk.com/Article/details/gnttitetb.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.tarul.cn/Article/details/gsmsjabak.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.epnwcf.com/Article/details/gcxiyxoxt.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.tarul.cn/Article/details/gorrhozho.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fktsv.cn/Article/details/gluconyzl.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.tarul.cn/Article/details/geagocejh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fktsv.cn/Article/details/gjnlkcnzb.sHtML

[U85] JS：可选链
来源：http://blog.bbcook.cn/Article/details/gyrwfkspg.sHtML

a?.b?.c
来源：http://www.blog.fktsv.cn/Article/details/gemukwfii.sHtML

[U86] JS：空值合并
来源：http://www.blog.bbcook.cn/Article/details/gsfwjgqfp.sHtML

a ?? b
来源：http://www.share.fktsv.cn/Article/details/gzsasvdkl.sHtML


<!-- 参考信息 -->