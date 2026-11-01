代发 wailian999

[T03] Kotlin：字符串模板
来源：http://m.share.bbcook.cn/Article/details/gkajarfmd.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/guewofiqf.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.epnwcf.com/Article/details/guptlccfj.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.vehdjk.com/Article/details/gvnayrubl.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.epnwcf.com/Article/details/glnwheucb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/gczuugfhu.sHtML

[T06] Kotlin：集合映射
来源：http://wap.sjlbkw.cn/Article/details/ghuknwtbq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/gvibwcsne.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gobjnsmok.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.epnwcf.com/Article/details/gvutlagow.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.bbcook.cn/Article/details/gumxcxkzz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.yfazqb.com/Article/details/guspnlabo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.yfazqb.com/Article/details/gbvyhzzyt.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.bbcook.cn/Article/details/gplontuvf.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gpmcybcum.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.bbcook.cn/Article/details/gqjmdkkzx.sHtML

[T11] Kotlin：协程
来源：http://m.share.fktsv.cn/Article/details/gnjntbsso.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.yfazqb.com/Article/details/gwpispdly.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/gboiwrnkd.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.yfazqb.com/Article/details/gqdivwlmf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.epnwcf.com/Article/details/gclsnfjad.sHtML

val m = mapOf("a" to 1)
来源：http://wap.yfazqb.com/Article/details/gzvkexjxn.sHtML

[T14] Kotlin：循环
来源：http://m.share.sjlbkw.cn/Article/details/gaywbirsq.sHtML

for (i in 1..10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gtehvnqbp.sHtML

[T15] Kotlin：接口
来源：http://www.blog.vehdjk.com/Article/details/grejiylnc.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.yfazqb.com/Article/details/gsyzfuvcz.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gwktcihpm.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gxrlaowch.sHtML

[T17] Swift：变量与常量
来源：http://www.share.vehdjk.com/Article/details/gqvmzjzkb.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gmguqvpzs.sHtML

[T18] Swift：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gkboayfcl.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gdwjtmjdq.sHtML

[T19] Swift：可选绑定
来源：http://read.share.tarul.cn/Article/details/gzxhegiva.sHtML

if let n = opt { print(n) }
来源：http://m.share.epnwcf.com/Article/details/gcbjlevkx.sHtML

[T20] Swift：数组操作
来源：http://wap.tarul.cn/Article/details/gdzwbdrtr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.tarul.cn/Article/details/gqoaipzrp.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/gyosixnos.sHtML

for x in a { print(x) }
来源：http://m.share.fktsv.cn/Article/details/gipqttvpa.sHtML

[T22] Swift：字典
来源：http://read.share.sjlbkw.cn/Article/details/ggpaomjit.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fktsv.cn/Article/details/guajzydlg.sHtML

[T23] Swift：函数
来源：http://m.share.fktsv.cn/Article/details/gawetcssm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/gxokdcclj.sHtML

[T24] Swift：闭包
来源：http://mobile.epnwcf.com/Article/details/gimorwguf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gpmofpiry.sHtML

[T25] Swift：结构体
来源：http://blog.vehdjk.com/Article/details/gabgltlcz.sHtML

struct P { var x: Int }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmklgwwe.sHtML

[T26] Swift：类与重写
来源：http://www.share.sjlbkw.cn/Article/details/gfjgzaunr.sHtML

class A: Base { override func f() {} }
来源：http://blog.epnwcf.com/Article/details/gmvylieik.sHtML

[T27] Swift：错误处理
来源：http://www.share.tarul.cn/Article/details/gxmitbywq.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.yfazqb.com/Article/details/gxayiubxn.sHtML

[T28] Swift：枚举
来源：http://m.share.yfazqb.com/Article/details/gdwsujnzs.sHtML

enum Color { case red, green }
来源：http://www.m.share.epnwcf.com/Article/details/gxkgdntpu.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fktsv.cn/Article/details/grdgxqdex.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/gqvqvauqg.sHtML

[T30] Swift：协议
来源：http://mobile.bbcook.cn/Article/details/guuraintu.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.tarul.cn/Article/details/gxjgrovir.sHtML

[T31] Lua：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gzwjigeta.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gbbqszzlm.sHtML

[T32] Lua：局部变量
来源：http://blog.bbcook.cn/Article/details/gzshqrjgn.sHtML

local a = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxzyqgad.sHtML

[T33] Lua：表（数组）
来源：http://baike.sjlbkw.cn/Article/details/gcoztksyd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.vehdjk.com/Article/details/gsqsodqmm.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.bbcook.cn/Article/details/gwqzxceah.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.epnwcf.com/Article/details/gkitrnuor.sHtML

[T35] Lua：字典表
来源：http://wap.bbcook.cn/Article/details/gynzrwhjs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.tarul.cn/Article/details/gajimhfts.sHtML

[T36] Lua：函数
来源：http://read.share.tarul.cn/Article/details/gnsctkisx.sHtML

function add(a, b) return a + b end
来源：http://wap.yfazqb.com/Article/details/gnxsqheyf.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fktsv.cn/Article/details/gubmcdmqy.sHtML

"a" .. "b"
来源：http://mobile.sjlbkw.cn/Article/details/getbnhhcd.sHtML

[T38] Lua：条件
来源：http://3g.yfazqb.com/Article/details/gmnegioqg.sHtML

if x > 0 then print("正") end
来源：http://blog.vehdjk.com/Article/details/gztywwbzv.sHtML

[T39] Lua：模式匹配
来源：http://wap.bbcook.cn/Article/details/ghflznkat.sHtML

string.find(s, "%d+")
来源：http://wap.yfazqb.com/Article/details/gokkynfxw.sHtML

[T40] Lua：元表
来源：http://blog.sjlbkw.cn/Article/details/gyduimkrn.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.sjlbkw.cn/Article/details/gnzpjrfwp.sHtML

[T41] Perl：Hello World
来源：http://m.share.yfazqb.com/Article/details/ghjenzkru.sHtML

print "Hello\n";
来源：http://www.m.share.epnwcf.com/Article/details/gepubhuen.sHtML

[T42] Perl：变量类型
来源：http://baike.bbcook.cn/Article/details/gvmtycxyr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.sjlbkw.cn/Article/details/gajtpbfdn.sHtML

[T43] Perl：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gyptykzar.sHtML

"值: $a"
来源：http://mobile.bbcook.cn/Article/details/gcuosbyin.sHtML

[T44] Perl：条件
来源：http://www.blog.bbcook.cn/Article/details/giszqrimp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.bbcook.cn/Article/details/gkwopklyt.sHtML

[T45] Perl：数组遍历
来源：http://www.share.vehdjk.com/Article/details/gjmjdxssp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.yfazqb.com/Article/details/gpsnpiwrm.sHtML

[T46] Perl：哈希操作
来源：http://mobile.tarul.cn/Article/details/gxhxlyrys.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.yfazqb.com/Article/details/giaatkprp.sHtML

[T47] Perl：正则捕获
来源：http://mobile.bbcook.cn/Article/details/gbaivospc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.tarul.cn/Article/details/gznfkikim.sHtML

[T48] Perl：正则替换
来源：http://read.share.fktsv.cn/Article/details/gizztyujd.sHtML

$s =~ s/old/new/g;
来源：http://3g.vehdjk.com/Article/details/gmwwtwnpk.sHtML

[T49] Perl：函数
来源：http://3g.yfazqb.com/Article/details/gwxkcalan.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gmbfsgwqg.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/ghgkvijpq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.sjlbkw.cn/Article/details/golpqxrmi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.bbcook.cn/Article/details/gmvbyenic.sHtML

[T51] Scala：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/ghqzeeyse.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gsmqzletu.sHtML

[T52] Scala：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gszytzinw.sHtML

val a = 1;  var b = 2
来源：http://mobile.bbcook.cn/Article/details/gbwwcuwdl.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/geoetpiqm.sHtML

s"值: $b"
来源：http://baike.epnwcf.com/Article/details/gnqocucqs.sHtML

[T54] Scala：集合映射
来源：http://3g.epnwcf.com/Article/details/gdbwdczjw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.bbcook.cn/Article/details/gienbjftr.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/ghlpshhek.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.yfazqb.com/Article/details/gnpyvpgba.sHtML

[T56] Scala：样例类
来源：http://m.share.bbcook.cn/Article/details/gzskqkuca.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gdysxisrh.sHtML

[T57] Scala：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/gtolracug.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/gnsysxrji.sHtML

[T58] Scala：函数定义
来源：http://blog.epnwcf.com/Article/details/gzvwmfvfk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.vehdjk.com/Article/details/gdtkjhrgt.sHtML

[T59] Scala：循环
来源：http://wap.epnwcf.com/Article/details/gjlwvzbht.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.vehdjk.com/Article/details/grhlcqxwm.sHtML

[T60] Scala：折叠
来源：http://www.blog.bbcook.cn/Article/details/grqdpygnq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.bbcook.cn/Article/details/gwugroucj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmqvhhsai.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/gbllbsvkj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkmrofvbq.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.bbcook.cn/Article/details/gdzfznirg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.bbcook.cn/Article/details/gpxegnkqm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.yfazqb.com/Article/details/gpugdwhwr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/galeznuvr.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.bbcook.cn/Article/details/glegecyre.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.yfazqb.com/Article/details/gfqurrmbt.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.sjlbkw.cn/Article/details/gbebuuwig.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.tarul.cn/Article/details/geffabgnc.sHtML

[U05] Py：列表去重且保序
来源：http://wap.yfazqb.com/Article/details/gcyksojpl.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgceazgc.sHtML

[U06] Py：合并两个字典
来源：http://blog.yfazqb.com/Article/details/grjejtgea.sHtML

{**a, **b}
来源：http://3g.sjlbkw.cn/Article/details/gzywvcivn.sHtML

[U07] Py：反转字典键值
来源：http://mobile.tarul.cn/Article/details/ggnpcgmse.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.tarul.cn/Article/details/gkdsyruoc.sHtML

[U08] Py：展平二维列表
来源：http://read.share.vehdjk.com/Article/details/ggoprqayv.sHtML

[y for x in nested for y in x]
来源：http://mobile.fktsv.cn/Article/details/glgmpypzw.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.vehdjk.com/Article/details/gsfiojljs.sHtML

max(d, key=d.get)
来源：http://read.share.sjlbkw.cn/Article/details/gwftwlsje.sHtML

[U10] Py：按值排序字典
来源：http://blog.tarul.cn/Article/details/ggtarfxcx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.bbcook.cn/Article/details/gbgedkezd.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.epnwcf.com/Article/details/gwrjureck.sHtML

(x * 2 for x in arr)
来源：http://wap.bbcook.cn/Article/details/gveyazlsv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/grerqgmto.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.yfazqb.com/Article/details/gixluclnp.sHtML

[U13] Py：固定长度队列
来源：http://wap.fktsv.cn/Article/details/gsudareao.sHtML

deque(maxlen=10)
来源：http://www.share.sjlbkw.cn/Article/details/glzpyycaj.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.tarul.cn/Article/details/gjnnayftc.sHtML

defaultdict(list)
来源：http://blog.vehdjk.com/Article/details/gekbwpjck.sHtML

[U15] Py：高精度计时
来源：http://blog.yfazqb.com/Article/details/gdhgghjob.sHtML

t = time.perf_counter()
来源：http://www.m.share.fktsv.cn/Article/details/goyinfchp.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.vehdjk.com/Article/details/gepizeaur.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.tarul.cn/Article/details/geyabgote.sHtML

[U17] Py：初始化日志
来源：http://baike.fktsv.cn/Article/details/gpbpcllyo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.epnwcf.com/Article/details/ghfvvbkcl.sHtML

[U18] Py：预编译正则
来源：http://wap.sjlbkw.cn/Article/details/gibbcrefx.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.bbcook.cn/Article/details/gcqfetwrw.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.vehdjk.com/Article/details/gkunyjpag.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.tarul.cn/Article/details/gcombaues.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.sjlbkw.cn/Article/details/gsrdplbyg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.epnwcf.com/Article/details/gzqmxgrai.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.yfazqb.com/Article/details/gstamipor.sHtML

@contextlib.contextmanager
来源：http://3g.sjlbkw.cn/Article/details/glehzgmps.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.epnwcf.com/Article/details/gvsrwhzzx.sHtML

list(zip(*m))
来源：http://baike.epnwcf.com/Article/details/gsjqqghkr.sHtML

[U23] Py：分块读取大文件
来源：http://blog.yfazqb.com/Article/details/gisftehsf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrhbsjsw.sHtML

[U24] Py：路径操作
来源：http://wap.vehdjk.com/Article/details/grimnboeq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gsewidzid.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.yfazqb.com/Article/details/guyodgmul.sHtML

csv.DictReader(f)
来源：http://m.share.fktsv.cn/Article/details/gzudlkrjd.sHtML

[U26] Py：并发下载
来源：http://www.share.vehdjk.com/Article/details/gzuhiboul.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fktsv.cn/Article/details/gcoedwlfg.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.tarul.cn/Article/details/ggwygfajn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.epnwcf.com/Article/details/gbbjqhygm.sHtML

[U28] Py：类型别名
来源：http://www.m.share.vehdjk.com/Article/details/gdowrmmfb.sHtML

UserId = int
来源：http://www.blog.bbcook.cn/Article/details/gjotgszsh.sHtML

[U29] Py：属性校验
来源：http://baike.epnwcf.com/Article/details/gvfgswnjw.sHtML

@property 与 @x.setter 配合
来源：http://wap.fktsv.cn/Article/details/gdjyxzeog.sHtML

[U30] Py：数据类
来源：http://mobile.bbcook.cn/Article/details/ganwkfxfd.sHtML

@dataclass(slots=True)
来源：http://www.blog.sjlbkw.cn/Article/details/grocdghzf.sHtML

[U31] Py：单测
来源：http://www.m.share.epnwcf.com/Article/details/ghrrscaba.sHtML

python -m pytest -q
来源：http://www.m.share.tarul.cn/Article/details/gcyuyobjc.sHtML

[U32] Py：代码格式化
来源：http://3g.sjlbkw.cn/Article/details/gpqhbkhqw.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fktsv.cn/Article/details/gblqsufjq.sHtML

[U33] Py：打包发布
来源：http://3g.sjlbkw.cn/Article/details/gbxucvgsm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fktsv.cn/Article/details/guydtohwa.sHtML

[U34] Py：判断编码
来源：http://m.share.epnwcf.com/Article/details/gqtqspwnj.sHtML

chardet.detect(raw)
来源：http://www.blog.bbcook.cn/Article/details/gpfrwzsko.sHtML

[U35] Py：发送邮件
来源：http://baike.sjlbkw.cn/Article/details/gqfksldsy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.tarul.cn/Article/details/gthkfumje.sHtML

[U36] Py：定时任务
来源：http://www.blog.bbcook.cn/Article/details/grrnweqwa.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.yfazqb.com/Article/details/grvisjwvb.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.bbcook.cn/Article/details/gedggoznu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.sjlbkw.cn/Article/details/gyuvxvkup.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.vehdjk.com/Article/details/gdjzfuskg.sHtML

Path(__file__).resolve().parent
来源：http://read.share.vehdjk.com/Article/details/gqsfdpbby.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.vehdjk.com/Article/details/gbprungxs.sHtML

sys.stdout.isatty()
来源：http://wap.epnwcf.com/Article/details/gxlbnadlp.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.sjlbkw.cn/Article/details/gaxycxdnz.sHtML

print("err", file=sys.stderr)
来源：http://read.share.sjlbkw.cn/Article/details/gusdmfgmz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.yfazqb.com/Article/details/geqysvepk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fktsv.cn/Article/details/gmlmahmlx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.bbcook.cn/Article/details/gtbkysbei.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.vehdjk.com/Article/details/gmigwcfll.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fktsv.cn/Article/details/gnfxvqdwa.sHtML

namespace App\Http;
来源：http://blog.yfazqb.com/Article/details/gvpakrcrt.sHtML

[U44] PHP：开启严格类型
来源：http://blog.vehdjk.com/Article/details/gmpexlocr.sHtML

declare(strict_types=1);
来源：http://m.share.epnwcf.com/Article/details/grlsfxsdq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.sjlbkw.cn/Article/details/glnbqquid.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gvknamxuz.sHtML

[U46] PHP：可空类型
来源：http://www.blog.vehdjk.com/Article/details/gdvxbbkvq.sHtML

?string $name = null
来源：http://3g.tarul.cn/Article/details/gmvckhhns.sHtML

[U47] PHP：联合类型
来源：http://www.blog.epnwcf.com/Article/details/gnngcmiba.sHtML

int|string $id
来源：http://wap.sjlbkw.cn/Article/details/gcaluonrh.sHtML

[U48] PHP：纯枚举
来源：http://baike.epnwcf.com/Article/details/gsxgkmrhm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.sjlbkw.cn/Article/details/gavtxzkak.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fktsv.cn/Article/details/gmufspqcw.sHtML

public readonly string $name
来源：http://read.share.tarul.cn/Article/details/gfryyiqwu.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.epnwcf.com/Article/details/gfqmapdyo.sHtML

public function __construct(private int $id) {}
来源：http://blog.epnwcf.com/Article/details/golxxraen.sHtML

[U51] PHP：数组解构
来源：http://www.share.epnwcf.com/Article/details/gnzddoqoi.sHtML

[$a, $b] = $arr;
来源：http://m.share.vehdjk.com/Article/details/gnbyqxora.sHtML

[U52] PHP：箭头函数
来源：http://read.share.epnwcf.com/Article/details/guvuqpidx.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.bbcook.cn/Article/details/gxywcvedo.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.vehdjk.com/Article/details/gchslsfee.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.vehdjk.com/Article/details/geurhtzub.sHtML

[U54] PHP：空安全调用
来源：http://read.share.tarul.cn/Article/details/gblzbwvli.sHtML

$obj?->method()
来源：http://mobile.fktsv.cn/Article/details/gzqytewuv.sHtML

[U55] PHP：match 表达式
来源：http://www.share.epnwcf.com/Article/details/gvhqcigjf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.tarul.cn/Article/details/gurossoiv.sHtML

[U56] PHP：命名参数
来源：http://read.share.fktsv.cn/Article/details/gmufxpdkb.sHtML

f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gqafrilit.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gesmbbbjh.sHtML

"值: {$a}"
来源：http://www.blog.bbcook.cn/Article/details/ghxyrbxeu.sHtML

[U58] PHP：数组三件套
来源：http://mobile.tarul.cn/Article/details/gkbjjcdrx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fktsv.cn/Article/details/gxsojfhcm.sHtML

[U59] PHP：自定义排序
来源：http://www.share.vehdjk.com/Article/details/gnlpademe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.tarul.cn/Article/details/gadtihogf.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.epnwcf.com/Article/details/gotougvqm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fktsv.cn/Article/details/gjtqyleru.sHtML

[U61] PHP：正则
来源：http://3g.fktsv.cn/Article/details/gyyrigssx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/gqbefbkzg.sHtML

[U62] PHP：日期对象
来源：http://baike.sjlbkw.cn/Article/details/gyrhzmrow.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.epnwcf.com/Article/details/gjxemplcb.sHtML

[U63] PHP：文件读写
来源：http://baike.epnwcf.com/Article/details/gmbobukcs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.yfazqb.com/Article/details/geqlymwdv.sHtML

[U64] PHP：目录遍历
来源：http://mobile.vehdjk.com/Article/details/gblfzggsw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.tarul.cn/Article/details/gzghnjyrl.sHtML

[U65] PHP：会话
来源：http://mobile.sjlbkw.cn/Article/details/gybxvuhrx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gijhjjnsr.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.tarul.cn/Article/details/gpwmtolgi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.bbcook.cn/Article/details/gcvffooxl.sHtML

[U67] PHP：处理文件上传
来源：http://wap.vehdjk.com/Article/details/gtlvaqmod.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.vehdjk.com/Article/details/gyutitsuj.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.yfazqb.com/Article/details/gcflhturx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.tarul.cn/Article/details/gonhkvgus.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.sjlbkw.cn/Article/details/gmkcekyox.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.bbcook.cn/Article/details/gaqtzyxhy.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.vehdjk.com/Article/details/gybtyqrrj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.sjlbkw.cn/Article/details/gcegcmwfe.sHtML

[U71] PHP：抛出异常
来源：http://blog.epnwcf.com/Article/details/gqfiiqplz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.bbcook.cn/Article/details/gmcpqnncy.sHtML

[U72] PHP：写错误日志
来源：http://read.share.yfazqb.com/Article/details/gfdjoayop.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fktsv.cn/Article/details/gwjixfktd.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.yfazqb.com/Article/details/gflemqrmi.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.vehdjk.com/Article/details/gulhiwacp.sHtML

[U74] PHP：读取环境变量
来源：http://baike.vehdjk.com/Article/details/gikgadoje.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.epnwcf.com/Article/details/gqtdwyslf.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.yfazqb.com/Article/details/gnlaciqkc.sHtML

composer require psr/container
来源：http://m.share.tarul.cn/Article/details/gahtdaeub.sHtML

[U76] PHP：简单路由
来源：http://read.share.epnwcf.com/Article/details/gbzwfuszq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.bbcook.cn/Article/details/goqnyahre.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.tarul.cn/Article/details/gaxiydffl.sHtML

composer require twig/twig
来源：http://blog.sjlbkw.cn/Article/details/gmriencmy.sHtML

[U78] PHP：单元测试
来源：http://wap.epnwcf.com/Article/details/gwhbxsqli.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.sjlbkw.cn/Article/details/gyftqdxbc.sHtML

[U79] PHP：静态分析
来源：http://blog.epnwcf.com/Article/details/gdoiwapau.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.bbcook.cn/Article/details/gpyvpqcto.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.bbcook.cn/Article/details/ggjdutcot.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.vehdjk.com/Article/details/gchsooyhn.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.tarul.cn/Article/details/gqdjxkssm.sHtML

npm init -y;  npm i express
来源：http://www.share.sjlbkw.cn/Article/details/givjjwyhe.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fktsv.cn/Article/details/gnlygxvih.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.tarul.cn/Article/details/gycnrenfb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.sjlbkw.cn/Article/details/ghtgvunvt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.bbcook.cn/Article/details/ggiwasinp.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.sjlbkw.cn/Article/details/gumfvdsyo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.sjlbkw.cn/Article/details/gxvkghkco.sHtML

[U85] JS：可选链
来源：http://mobile.yfazqb.com/Article/details/gtleohtqc.sHtML

a?.b?.c
来源：http://www.m.share.epnwcf.com/Article/details/gwlzldtcx.sHtML

[U86] JS：空值合并
来源：http://mobile.bbcook.cn/Article/details/gkybipxlt.sHtML

a ?? b
来源：http://www.share.sjlbkw.cn/Article/details/ghhussoiz.sHtML

[U87] JS：解构默认值
来源：http://wap.bbcook.cn/Article/details/gdypxnynz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fktsv.cn/Article/details/gyenyjyzl.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.tarul.cn/Article/details/gndqylkcp.sHtML

{ ...a, ...b }
来源：http://wap.yfazqb.com/Article/details/gzckhfpmq.sHtML

[U89] JS：数组去重
来源：http://read.share.bbcook.cn/Article/details/gwfpjlezb.sHtML

[...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/giureukxt.sHtML

[U90] JS：数字数组排序
来源：http://baike.sjlbkw.cn/Article/details/gpsrswybt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gsryoxbon.sHtML


<!-- 参考信息 -->