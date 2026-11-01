代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gczfczrmd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.sjlbkw.cn/Article/details/gqeqolrxb.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/guryhpiaf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gdvlfbcpz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/guyjpyfxb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gkranvtms.sHtML

[T08] Kotlin：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gklnawdzy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gdygmlqby.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.vehdjk.com/Article/details/gbwhcvdyk.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.tarul.cn/Article/details/gnkhxfmxl.sHtML

[T10] Kotlin：默认参数
来源：http://wap.bbcook.cn/Article/details/ggfempekt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.tarul.cn/Article/details/gsczoqvpg.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gyqphikey.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.tarul.cn/Article/details/gzdjrsnbz.sHtML

[T12] Kotlin：解构声明
来源：http://blog.vehdjk.com/Article/details/grranpwrc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/getiunfmh.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/gntdowcrf.sHtML

val m = mapOf("a" to 1)
来源：http://baike.epnwcf.com/Article/details/gynsehbka.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/gybgqeubv.sHtML

for (i in 1..10) println(i)
来源：http://read.share.tarul.cn/Article/details/gowgibguf.sHtML

[T15] Kotlin：接口
来源：http://www.blog.tarul.cn/Article/details/gyxobokol.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.tarul.cn/Article/details/grzwfpuai.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gcsjghusa.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/geefsrwtz.sHtML

[T17] Swift：变量与常量
来源：http://3g.sjlbkw.cn/Article/details/gbxtcfmmn.sHtML

var a = 1;  let b = 2
来源：http://blog.yfazqb.com/Article/details/gruioohsp.sHtML

[T18] Swift：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gtziywiiv.sHtML

"值: \(b)"
来源：http://wap.vehdjk.com/Article/details/gmovfirbx.sHtML

[T19] Swift：可选绑定
来源：http://www.share.tarul.cn/Article/details/gkbvtguey.sHtML

if let n = opt { print(n) }
来源：http://blog.vehdjk.com/Article/details/gwcdrlbpb.sHtML

[T20] Swift：数组操作
来源：http://mobile.fktsv.cn/Article/details/gsqgvcrqu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.epnwcf.com/Article/details/gmgzevjfi.sHtML

[T21] Swift：遍历
来源：http://wap.tarul.cn/Article/details/gynujcpqz.sHtML

for x in a { print(x) }
来源：http://www.share.fktsv.cn/Article/details/gvneckuxr.sHtML

[T22] Swift：字典
来源：http://read.share.vehdjk.com/Article/details/gnrtxnznc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.bbcook.cn/Article/details/gtnecskzd.sHtML

[T23] Swift：函数
来源：http://www.share.sjlbkw.cn/Article/details/gzouxjnvq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.yfazqb.com/Article/details/gvjvvjjon.sHtML

[T24] Swift：闭包
来源：http://3g.sjlbkw.cn/Article/details/grkvfcqkm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gwtvjsthi.sHtML

[T25] Swift：结构体
来源：http://read.share.tarul.cn/Article/details/gudfdholj.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/gzjdljlwu.sHtML

[T26] Swift：类与重写
来源：http://mobile.sjlbkw.cn/Article/details/gxbitzzfl.sHtML

class A: Base { override func f() {} }
来源：http://mobile.vehdjk.com/Article/details/ggcnmnsxh.sHtML

[T27] Swift：错误处理
来源：http://wap.tarul.cn/Article/details/gnxwyjkup.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.tarul.cn/Article/details/goqtfwqhu.sHtML

[T28] Swift：枚举
来源：http://wap.tarul.cn/Article/details/gtmsdkuvc.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gbibkgylj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.epnwcf.com/Article/details/gbihnkofw.sHtML

guard let x = opt else { return }
来源：http://3g.bbcook.cn/Article/details/gsaojtdoj.sHtML

[T30] Swift：协议
来源：http://mobile.fktsv.cn/Article/details/ggmpcqqom.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.sjlbkw.cn/Article/details/gigvwljag.sHtML

[T31] Lua：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gbsjlkdwp.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gfuxaybih.sHtML

[T32] Lua：局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gejumvnlm.sHtML

local a = 1
来源：http://3g.yfazqb.com/Article/details/gikgghxvw.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fktsv.cn/Article/details/gtapdfkfu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.tarul.cn/Article/details/gpgrffhgd.sHtML

[T34] Lua：遍历表
来源：http://read.share.vehdjk.com/Article/details/grkxvygxq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.tarul.cn/Article/details/ghzaqzrwh.sHtML

[T35] Lua：字典表
来源：http://blog.epnwcf.com/Article/details/gxksdftxo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.vehdjk.com/Article/details/ghoxdiqse.sHtML

[T36] Lua：函数
来源：http://www.m.share.yfazqb.com/Article/details/gfoqzgvno.sHtML

function add(a, b) return a + b end
来源：http://blog.fktsv.cn/Article/details/glbvphqfq.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gghlwtrts.sHtML

"a" .. "b"
来源：http://m.share.fktsv.cn/Article/details/gezqnkzic.sHtML

[T38] Lua：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gyeuydcqa.sHtML

if x > 0 then print("正") end
来源：http://read.share.epnwcf.com/Article/details/ghwxkisqn.sHtML

[T39] Lua：模式匹配
来源：http://3g.yfazqb.com/Article/details/gdwaahecc.sHtML

string.find(s, "%d+")
来源：http://blog.bbcook.cn/Article/details/gzqnbajie.sHtML

[T40] Lua：元表
来源：http://wap.bbcook.cn/Article/details/grugmyohr.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.yfazqb.com/Article/details/ghdyaypdy.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gzebpxxto.sHtML

print "Hello\n";
来源：http://wap.tarul.cn/Article/details/gvhretdyb.sHtML

[T42] Perl：变量类型
来源：http://mobile.bbcook.cn/Article/details/gpuycyvgb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.yfazqb.com/Article/details/getsulccs.sHtML

[T43] Perl：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gviylqfgg.sHtML

"值: $a"
来源：http://mobile.vehdjk.com/Article/details/gsfzoeaci.sHtML

[T44] Perl：条件
来源：http://baike.epnwcf.com/Article/details/gcpaisweo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fktsv.cn/Article/details/gbakbwucp.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.yfazqb.com/Article/details/gteymcemv.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.sjlbkw.cn/Article/details/gplfwcyzi.sHtML

[T46] Perl：哈希操作
来源：http://3g.epnwcf.com/Article/details/glvnybmyc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.bbcook.cn/Article/details/gqziimpad.sHtML

[T47] Perl：正则捕获
来源：http://www.share.yfazqb.com/Article/details/gajxpujcn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.bbcook.cn/Article/details/gylgxwamq.sHtML

[T48] Perl：正则替换
来源：http://www.blog.tarul.cn/Article/details/gkjiyhbma.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fktsv.cn/Article/details/gfbvusapk.sHtML

[T49] Perl：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbeibpnz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gdotjnwto.sHtML

[T50] Perl：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gdneoisxv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.vehdjk.com/Article/details/gbujjqnrf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fktsv.cn/Article/details/gehcrjjfb.sHtML

[T51] Scala：Hello World
来源：http://m.share.bbcook.cn/Article/details/glccfzrku.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gtyjawcnj.sHtML

[T52] Scala：变量
来源：http://www.m.share.fktsv.cn/Article/details/gouvoriqu.sHtML

val a = 1;  var b = 2
来源：http://read.share.vehdjk.com/Article/details/gbaxakenn.sHtML

[T53] Scala：字符串插值
来源：http://blog.epnwcf.com/Article/details/ghgpmidpe.sHtML

s"值: $b"
来源：http://www.share.epnwcf.com/Article/details/gfznlcdbl.sHtML

[T54] Scala：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gyengghrw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gpjftyxta.sHtML

[T55] Scala：集合过滤
来源：http://baike.yfazqb.com/Article/details/gseyfoine.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.yfazqb.com/Article/details/gaeoetmyy.sHtML

[T56] Scala：样例类
来源：http://m.share.tarul.cn/Article/details/goythjjgx.sHtML

case class User(name: String, age: Int)
来源：http://mobile.epnwcf.com/Article/details/gpxbkwpeo.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/gwjzqedfe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fktsv.cn/Article/details/gcyusjlik.sHtML

[T58] Scala：函数定义
来源：http://baike.vehdjk.com/Article/details/ghvzdifzd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fktsv.cn/Article/details/gydrcyast.sHtML

[T59] Scala：循环
来源：http://www.blog.epnwcf.com/Article/details/gbtucuhwc.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gtagqitst.sHtML

[T60] Scala：折叠
来源：http://blog.sjlbkw.cn/Article/details/ghcusflbc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.vehdjk.com/Article/details/grzfnuqgt.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gzavpjdsm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.vehdjk.com/Article/details/gcixlxjvu.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gzuouwktw.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.vehdjk.com/Article/details/grqygafig.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fktsv.cn/Article/details/gnmpnaexr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.epnwcf.com/Article/details/gzpeflnaf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fktsv.cn/Article/details/ghbyxmoxg.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/gfmjxcdbm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gxgbthgvo.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.bbcook.cn/Article/details/gafvvykru.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.bbcook.cn/Article/details/gtvbfkkie.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.vehdjk.com/Article/details/gblmkkeqc.sHtML

list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/gkmpjsbcp.sHtML

[U06] Py：合并两个字典
来源：http://www.share.yfazqb.com/Article/details/gxhebyrya.sHtML

{**a, **b}
来源：http://www.blog.yfazqb.com/Article/details/gozixrrnq.sHtML

[U07] Py：反转字典键值
来源：http://baike.tarul.cn/Article/details/gvtowlyuv.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.sjlbkw.cn/Article/details/gdlkthois.sHtML

[U08] Py：展平二维列表
来源：http://mobile.sjlbkw.cn/Article/details/gkvctpzov.sHtML

[y for x in nested for y in x]
来源：http://blog.tarul.cn/Article/details/gxbfqobru.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/gsopjhbzd.sHtML

max(d, key=d.get)
来源：http://wap.yfazqb.com/Article/details/ggealazdk.sHtML

[U10] Py：按值排序字典
来源：http://baike.fktsv.cn/Article/details/gswtsjmbz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.vehdjk.com/Article/details/gksjziuxe.sHtML

[U11] Py：生成器表达式
来源：http://mobile.sjlbkw.cn/Article/details/gmaunxzvl.sHtML

(x * 2 for x in arr)
来源：http://read.share.vehdjk.com/Article/details/goenybzak.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.sjlbkw.cn/Article/details/gelcguonn.sHtML

Counter(arr).most_common(3)
来源：http://mobile.epnwcf.com/Article/details/gktpveqzu.sHtML

[U13] Py：固定长度队列
来源：http://wap.bbcook.cn/Article/details/gudvzphns.sHtML

deque(maxlen=10)
来源：http://www.blog.epnwcf.com/Article/details/gqfoncroh.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.yfazqb.com/Article/details/gvkylrjka.sHtML

defaultdict(list)
来源：http://3g.bbcook.cn/Article/details/gcmpolynq.sHtML

[U15] Py：高精度计时
来源：http://m.share.fktsv.cn/Article/details/gwesaugzn.sHtML

t = time.perf_counter()
来源：http://www.share.fktsv.cn/Article/details/gwhtoirjh.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.vehdjk.com/Article/details/glrhndtdd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.bbcook.cn/Article/details/gycagptkf.sHtML

[U17] Py：初始化日志
来源：http://read.share.fktsv.cn/Article/details/gpfqbntrm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.bbcook.cn/Article/details/gbxseyxdz.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.yfazqb.com/Article/details/gtpzqwncp.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.bbcook.cn/Article/details/giwexjtqe.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fktsv.cn/Article/details/gvscmctuz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.bbcook.cn/Article/details/gwnwzxhel.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fktsv.cn/Article/details/gdjjrsack.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fktsv.cn/Article/details/gdpbqgcsl.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.sjlbkw.cn/Article/details/gerkhxcke.sHtML

@contextlib.contextmanager
来源：http://blog.epnwcf.com/Article/details/glrgstnmd.sHtML

[U22] Py：矩阵转置
来源：http://3g.bbcook.cn/Article/details/gfnjevkhx.sHtML

list(zip(*m))
来源：http://www.blog.fktsv.cn/Article/details/gbfwilyli.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.bbcook.cn/Article/details/gkjqxknmg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.epnwcf.com/Article/details/gvpmbygxt.sHtML

[U24] Py：路径操作
来源：http://baike.vehdjk.com/Article/details/gtgzlucen.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gbysiqpiz.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.sjlbkw.cn/Article/details/gbhbrehnp.sHtML

csv.DictReader(f)
来源：http://blog.vehdjk.com/Article/details/gnwupdztd.sHtML

[U26] Py：并发下载
来源：http://read.share.sjlbkw.cn/Article/details/glhfivedb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.yfazqb.com/Article/details/gonwgikxu.sHtML

[U27] Py：异步 HTTP
来源：http://baike.bbcook.cn/Article/details/gpinbledx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.tarul.cn/Article/details/ghcovbpkh.sHtML

[U28] Py：类型别名
来源：http://wap.epnwcf.com/Article/details/gycvhrjcl.sHtML

UserId = int
来源：http://m.share.fktsv.cn/Article/details/gduvtgmfi.sHtML

[U29] Py：属性校验
来源：http://m.share.epnwcf.com/Article/details/gfvnjbaok.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fktsv.cn/Article/details/gjsxjglyz.sHtML

[U30] Py：数据类
来源：http://blog.sjlbkw.cn/Article/details/gffanukvd.sHtML

@dataclass(slots=True)
来源：http://www.blog.vehdjk.com/Article/details/ghtqzofcl.sHtML

[U31] Py：单测
来源：http://read.share.bbcook.cn/Article/details/gfeyzhhkk.sHtML

python -m pytest -q
来源：http://m.share.epnwcf.com/Article/details/geodhjins.sHtML

[U32] Py：代码格式化
来源：http://www.blog.epnwcf.com/Article/details/grrmidtgu.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.yfazqb.com/Article/details/gxfryptxl.sHtML

[U33] Py：打包发布
来源：http://www.share.fktsv.cn/Article/details/gixxmtezt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.vehdjk.com/Article/details/glaoylkla.sHtML

[U34] Py：判断编码
来源：http://www.m.share.yfazqb.com/Article/details/geophvkfv.sHtML

chardet.detect(raw)
来源：http://3g.vehdjk.com/Article/details/gxpobadhr.sHtML

[U35] Py：发送邮件
来源：http://baike.vehdjk.com/Article/details/guietdbbc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fktsv.cn/Article/details/givlmolsc.sHtML

[U36] Py：定时任务
来源：http://wap.yfazqb.com/Article/details/gjukdqkeg.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.sjlbkw.cn/Article/details/gwypthqsl.sHtML

[U37] Py：读写 Excel
来源：http://read.share.bbcook.cn/Article/details/gtowuiqbi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.vehdjk.com/Article/details/gmrbpuscb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.tarul.cn/Article/details/grxhngaue.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fktsv.cn/Article/details/gblbfdppe.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.yfazqb.com/Article/details/gcxuilpkj.sHtML

sys.stdout.isatty()
来源：http://read.share.yfazqb.com/Article/details/gaaesxlcf.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.vehdjk.com/Article/details/gwimkicek.sHtML

print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/gxgtmxnoe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.vehdjk.com/Article/details/gxburzrrn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.epnwcf.com/Article/details/gpnkwfybo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.sjlbkw.cn/Article/details/gcdexblbd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.tarul.cn/Article/details/glunqvqnn.sHtML

[U43] PHP：声明命名空间
来源：http://blog.sjlbkw.cn/Article/details/gyzrfcqmi.sHtML

namespace App\Http;
来源：http://blog.vehdjk.com/Article/details/gwameoiol.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.bbcook.cn/Article/details/gyjjkgway.sHtML

declare(strict_types=1);
来源：http://www.m.share.tarul.cn/Article/details/gwbutnvcf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.vehdjk.com/Article/details/glqcpxays.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gequytzki.sHtML

[U46] PHP：可空类型
来源：http://www.share.fktsv.cn/Article/details/gtdlpbhul.sHtML

?string $name = null
来源：http://baike.vehdjk.com/Article/details/goerfcexv.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.yfazqb.com/Article/details/gegngkjuy.sHtML

int|string $id
来源：http://3g.sjlbkw.cn/Article/details/gfklczzeg.sHtML

[U48] PHP：纯枚举
来源：http://3g.yfazqb.com/Article/details/geireacgi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.epnwcf.com/Article/details/ghqomzyqk.sHtML

[U49] PHP：只读属性
来源：http://read.share.fktsv.cn/Article/details/gqztnwqov.sHtML

public readonly string $name
来源：http://www.share.vehdjk.com/Article/details/gparzjyaw.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.epnwcf.com/Article/details/gcsbaejwp.sHtML

public function __construct(private int $id) {}
来源：http://www.share.sjlbkw.cn/Article/details/gouhdghfo.sHtML

[U51] PHP：数组解构
来源：http://mobile.epnwcf.com/Article/details/gcfzunrls.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fktsv.cn/Article/details/gnllvjxuh.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gfjbopjim.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.bbcook.cn/Article/details/gcrcwigro.sHtML

[U53] PHP：空合并运算符
来源：http://3g.bbcook.cn/Article/details/gqeoosqux.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.tarul.cn/Article/details/gwspneeiw.sHtML

[U54] PHP：空安全调用
来源：http://blog.sjlbkw.cn/Article/details/gzbgytveo.sHtML

$obj?->method()
来源：http://read.share.vehdjk.com/Article/details/ggcvakqkb.sHtML

[U55] PHP：match 表达式
来源：http://3g.sjlbkw.cn/Article/details/gzccqewzw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.tarul.cn/Article/details/gdiiaboqd.sHtML

[U56] PHP：命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gqsmdfapv.sHtML

f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gatsxvbym.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/glpsplzkj.sHtML

"值: {$a}"
来源：http://m.share.epnwcf.com/Article/details/gyprcyrif.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fktsv.cn/Article/details/gmcsopvkg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.epnwcf.com/Article/details/gvgtqmupg.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fktsv.cn/Article/details/gvwliqaas.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gkrzsvvtu.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.sjlbkw.cn/Article/details/gantdpvpa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.vehdjk.com/Article/details/guodnrebi.sHtML

[U61] PHP：正则
来源：http://www.share.bbcook.cn/Article/details/gnamfydhz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/gcpfsqhqc.sHtML

[U62] PHP：日期对象
来源：http://m.share.vehdjk.com/Article/details/ghhxiulzi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.bbcook.cn/Article/details/giucyqjkd.sHtML

[U63] PHP：文件读写
来源：http://www.blog.bbcook.cn/Article/details/gjmotgxjd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.tarul.cn/Article/details/gbenwdaqe.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.yfazqb.com/Article/details/glykhdfiy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fktsv.cn/Article/details/gtgoqcssd.sHtML

[U65] PHP：会话
来源：http://wap.tarul.cn/Article/details/glfrkchiz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gerykjonr.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.sjlbkw.cn/Article/details/gpvqfvtjo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.yfazqb.com/Article/details/gymnmpjad.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.tarul.cn/Article/details/gkvdzpphi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.epnwcf.com/Article/details/gdnduzanf.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.tarul.cn/Article/details/gtccduahh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fktsv.cn/Article/details/gzkrfnvpx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.vehdjk.com/Article/details/gkwlwdmso.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.tarul.cn/Article/details/gbzugtmmj.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fktsv.cn/Article/details/gfhirxbdt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.sjlbkw.cn/Article/details/gjnrsbbju.sHtML

[U71] PHP：抛出异常
来源：http://blog.sjlbkw.cn/Article/details/gntrvsabu.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fktsv.cn/Article/details/getebmwbq.sHtML

[U72] PHP：写错误日志
来源：http://3g.yfazqb.com/Article/details/gglofwgap.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.vehdjk.com/Article/details/gguhewsji.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.sjlbkw.cn/Article/details/gwgbovabb.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.sjlbkw.cn/Article/details/gyvwobtgk.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.epnwcf.com/Article/details/gvlcgqaql.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.vehdjk.com/Article/details/gwiarrzwz.sHtML

[U75] PHP：依赖注入
来源：http://m.share.yfazqb.com/Article/details/groqflzhx.sHtML

composer require psr/container
来源：http://3g.epnwcf.com/Article/details/gbkkfbvyo.sHtML

[U76] PHP：简单路由
来源：http://read.share.yfazqb.com/Article/details/guxbestsc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.sjlbkw.cn/Article/details/gbezxexdf.sHtML

[U77] PHP：模板渲染
来源：http://www.share.sjlbkw.cn/Article/details/gmziejtte.sHtML

composer require twig/twig
来源：http://blog.yfazqb.com/Article/details/gwjkzsbar.sHtML

[U78] PHP：单元测试
来源：http://baike.epnwcf.com/Article/details/gqfiddmxp.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.epnwcf.com/Article/details/gpgbdtwqy.sHtML

[U79] PHP：静态分析
来源：http://baike.yfazqb.com/Article/details/ghdmftico.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.epnwcf.com/Article/details/goafpxuwb.sHtML

[U80] PHP：代码规范修复
来源：http://blog.epnwcf.com/Article/details/glatqeuit.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.bbcook.cn/Article/details/gnmcluqdo.sHtML

[U81] JS：初始化项目
来源：http://www.share.fktsv.cn/Article/details/gboxnhenn.sHtML

npm init -y;  npm i express
来源：http://read.share.epnwcf.com/Article/details/gdqfekcth.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.epnwcf.com/Article/details/gysdsfnws.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.sjlbkw.cn/Article/details/ghxkuoikr.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.epnwcf.com/Article/details/gqzkvhslx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fktsv.cn/Article/details/gjanbwboq.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.yfazqb.com/Article/details/gnctburbc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.tarul.cn/Article/details/gzmxpvveg.sHtML

[U85] JS：可选链
来源：http://3g.tarul.cn/Article/details/gnhjgpjmd.sHtML

a?.b?.c
来源：http://wap.sjlbkw.cn/Article/details/gcbuumqsc.sHtML

[U86] JS：空值合并
来源：http://www.m.share.tarul.cn/Article/details/gnrqmnsnh.sHtML

a ?? b
来源：http://wap.bbcook.cn/Article/details/gtexltkgj.sHtML

[U87] JS：解构默认值
来源：http://3g.fktsv.cn/Article/details/gdaksawxi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.epnwcf.com/Article/details/gntnnapxg.sHtML

[U88] JS：对象展开合并
来源：http://baike.bbcook.cn/Article/details/gicvaqpmy.sHtML

{ ...a, ...b }
来源：http://blog.fktsv.cn/Article/details/gqhmvplis.sHtML

[U89] JS：数组去重
来源：http://3g.vehdjk.com/Article/details/gpzopgdzz.sHtML

[...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gdqndqboz.sHtML

[U90] JS：数字数组排序
来源：http://www.share.vehdjk.com/Article/details/gfyepxcaj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gqfuxezrb.sHtML

[U91] JS：对象键值遍历
来源：http://blog.sjlbkw.cn/Article/details/geeakhzcl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.bbcook.cn/Article/details/gvsxnbwbb.sHtML

[U92] JS：深拷贝
来源：http://m.share.epnwcf.com/Article/details/guqdbvjfo.sHtML

structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gahefmezm.sHtML


<!-- 参考信息 -->