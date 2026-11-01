代发 wailian999

[T05] Kotlin：when 表达式
来源：http://m.share.fktsv.cn/Article/details/gueccbzms.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.bbcook.cn/Article/details/gcnxxvsmo.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.epnwcf.com/Article/details/gkgpfasho.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gczderfeh.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gvlypmqsn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.vehdjk.com/Article/details/gyyxtuxxx.sHtML

[T08] Kotlin：数据类
来源：http://wap.yfazqb.com/Article/details/gzvvdzryt.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.bbcook.cn/Article/details/gauaapvdg.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.bbcook.cn/Article/details/glsmidpwr.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.yfazqb.com/Article/details/gslqqsvic.sHtML

[T10] Kotlin：默认参数
来源：http://wap.tarul.cn/Article/details/gjxtlzoct.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.sjlbkw.cn/Article/details/gevhtxkec.sHtML

[T11] Kotlin：协程
来源：http://mobile.tarul.cn/Article/details/ghsxmikpa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.vehdjk.com/Article/details/gawjrctly.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.bbcook.cn/Article/details/gukrnkfqy.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gavzzlmqo.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.bbcook.cn/Article/details/ghhkkbasa.sHtML

val m = mapOf("a" to 1)
来源：http://3g.tarul.cn/Article/details/gdbfbeofe.sHtML

[T14] Kotlin：循环
来源：http://mobile.sjlbkw.cn/Article/details/gngrqazyf.sHtML

for (i in 1..10) println(i)
来源：http://blog.epnwcf.com/Article/details/gibmgyqxs.sHtML

[T15] Kotlin：接口
来源：http://blog.fktsv.cn/Article/details/gnxxgkfvk.sHtML

interface Shape { fun area(): Double }
来源：http://blog.tarul.cn/Article/details/gxdrjyzra.sHtML

[T16] Swift：Hello World
来源：http://www.share.epnwcf.com/Article/details/gsijyzbby.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/gitjkuwfh.sHtML

[T17] Swift：变量与常量
来源：http://www.share.yfazqb.com/Article/details/grrrxutnu.sHtML

var a = 1;  let b = 2
来源：http://mobile.epnwcf.com/Article/details/gybuexmfj.sHtML

[T18] Swift：字符串插值
来源：http://blog.yfazqb.com/Article/details/gomdbshwq.sHtML

"值: \(b)"
来源：http://m.share.vehdjk.com/Article/details/gawlvwpjh.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/gfkpearjv.sHtML

if let n = opt { print(n) }
来源：http://baike.tarul.cn/Article/details/gexuublff.sHtML

[T20] Swift：数组操作
来源：http://mobile.fktsv.cn/Article/details/gchpstogj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.epnwcf.com/Article/details/gdzwqaoec.sHtML

[T21] Swift：遍历
来源：http://blog.tarul.cn/Article/details/gigmbzbiv.sHtML

for x in a { print(x) }
来源：http://baike.tarul.cn/Article/details/gnqfqqyhz.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/gcbiwdfsb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.vehdjk.com/Article/details/gfpcxjrde.sHtML

[T23] Swift：函数
来源：http://www.share.tarul.cn/Article/details/gmdheccwm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.bbcook.cn/Article/details/gyrxkztia.sHtML

[T24] Swift：闭包
来源：http://blog.vehdjk.com/Article/details/glnqegjqq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.epnwcf.com/Article/details/gzdxesicc.sHtML

[T25] Swift：结构体
来源：http://3g.epnwcf.com/Article/details/gzlvnjfbd.sHtML

struct P { var x: Int }
来源：http://www.m.share.tarul.cn/Article/details/gcwmaavvx.sHtML

[T26] Swift：类与重写
来源：http://3g.fktsv.cn/Article/details/ggulraoat.sHtML

class A: Base { override func f() {} }
来源：http://mobile.sjlbkw.cn/Article/details/ghdjcvjsa.sHtML

[T27] Swift：错误处理
来源：http://www.share.yfazqb.com/Article/details/grkqxoont.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.bbcook.cn/Article/details/gmmvjvxej.sHtML

[T28] Swift：枚举
来源：http://blog.vehdjk.com/Article/details/gqpzkrfbp.sHtML

enum Color { case red, green }
来源：http://blog.sjlbkw.cn/Article/details/gdvmmdpom.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/gepcqugrx.sHtML

guard let x = opt else { return }
来源：http://www.share.yfazqb.com/Article/details/gqniulyze.sHtML

[T30] Swift：协议
来源：http://wap.tarul.cn/Article/details/gnrxxsmph.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.tarul.cn/Article/details/grzpriyds.sHtML

[T31] Lua：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gtdgtaebz.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/gragfpgvr.sHtML

[T32] Lua：局部变量
来源：http://read.share.vehdjk.com/Article/details/gidkivchc.sHtML

local a = 1
来源：http://wap.vehdjk.com/Article/details/glnjiqeft.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fktsv.cn/Article/details/gmwzkgusm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.yfazqb.com/Article/details/ggiyzuncs.sHtML

[T34] Lua：遍历表
来源：http://read.share.vehdjk.com/Article/details/guoovgxge.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/gxtmjijny.sHtML

[T35] Lua：字典表
来源：http://m.share.sjlbkw.cn/Article/details/gkdsmouqs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.sjlbkw.cn/Article/details/goygxmtkg.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/gbqtqpsxm.sHtML

function add(a, b) return a + b end
来源：http://read.share.sjlbkw.cn/Article/details/griktyicd.sHtML

[T37] Lua：字符串拼接
来源：http://baike.tarul.cn/Article/details/gdzrnldlk.sHtML

"a" .. "b"
来源：http://baike.yfazqb.com/Article/details/gqdlekqro.sHtML

[T38] Lua：条件
来源：http://m.share.bbcook.cn/Article/details/giwjljhvi.sHtML

if x > 0 then print("正") end
来源：http://read.share.fktsv.cn/Article/details/gbtnwamzf.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/grljttddt.sHtML

string.find(s, "%d+")
来源：http://baike.epnwcf.com/Article/details/gedbywqmj.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/gemrnzszc.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.vehdjk.com/Article/details/gwtdhfkco.sHtML

[T41] Perl：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gauisbiza.sHtML

print "Hello\n";
来源：http://blog.fktsv.cn/Article/details/gjuhgmvbb.sHtML

[T42] Perl：变量类型
来源：http://www.share.tarul.cn/Article/details/gppicnobs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fktsv.cn/Article/details/gsbcmtlmv.sHtML

[T43] Perl：字符串插值
来源：http://baike.tarul.cn/Article/details/ghlodsndb.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/glkaktngg.sHtML

[T44] Perl：条件
来源：http://3g.epnwcf.com/Article/details/gdqsqrcoz.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.bbcook.cn/Article/details/gurabkcmy.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.tarul.cn/Article/details/gmsknpvjv.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.epnwcf.com/Article/details/gnrnubugn.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fktsv.cn/Article/details/gfvwaavdf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.bbcook.cn/Article/details/genjvhkgx.sHtML

[T47] Perl：正则捕获
来源：http://3g.fktsv.cn/Article/details/gnqbnlawn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.sjlbkw.cn/Article/details/gdbawrwui.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fktsv.cn/Article/details/gppizlgkf.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.sjlbkw.cn/Article/details/gdlurehnu.sHtML

[T49] Perl：函数
来源：http://mobile.tarul.cn/Article/details/glxmwynbx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gvmsyfxya.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/giwleudls.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.bbcook.cn/Article/details/gbaasydwt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fktsv.cn/Article/details/gxzsnffoj.sHtML

[T51] Scala：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gchjqwqkf.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gcavchcsf.sHtML

[T52] Scala：变量
来源：http://baike.tarul.cn/Article/details/gsqndpyvz.sHtML

val a = 1;  var b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gfnrneuin.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gztlejhem.sHtML

s"值: $b"
来源：http://wap.yfazqb.com/Article/details/gvrddugcf.sHtML

[T54] Scala：集合映射
来源：http://mobile.tarul.cn/Article/details/grthbsddf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.bbcook.cn/Article/details/gitltbbum.sHtML

[T55] Scala：集合过滤
来源：http://3g.tarul.cn/Article/details/gkusdnuon.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.sjlbkw.cn/Article/details/gevzwfbju.sHtML

[T56] Scala：样例类
来源：http://mobile.yfazqb.com/Article/details/gmqooxywi.sHtML

case class User(name: String, age: Int)
来源：http://blog.vehdjk.com/Article/details/gywmpoezd.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fktsv.cn/Article/details/gkbykduwa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gtajcpbff.sHtML

[T58] Scala：函数定义
来源：http://mobile.epnwcf.com/Article/details/gxvrurkrs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.sjlbkw.cn/Article/details/gagootmyk.sHtML

[T59] Scala：循环
来源：http://baike.epnwcf.com/Article/details/gmjvocecm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/glnqvfcev.sHtML

[T60] Scala：折叠
来源：http://read.share.yfazqb.com/Article/details/glmcevbnb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/gxhatifwq.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gsdxrujso.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.sjlbkw.cn/Article/details/gycgldgnd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gfyfgbhun.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.sjlbkw.cn/Article/details/gowulgene.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.yfazqb.com/Article/details/gcnsxwahj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.yfazqb.com/Article/details/geftrmwfd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.yfazqb.com/Article/details/gshmbqgge.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fktsv.cn/Article/details/gbtrqyczt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.epnwcf.com/Article/details/gizuhszun.sHtML

[U04] Py：变量调试打印
来源：http://www.share.vehdjk.com/Article/details/gybdxnoqe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.epnwcf.com/Article/details/gjjrhjgfy.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.bbcook.cn/Article/details/gjgvvlqwy.sHtML

list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/gjoixhxko.sHtML

[U06] Py：合并两个字典
来源：http://3g.bbcook.cn/Article/details/givczndie.sHtML

{**a, **b}
来源：http://baike.vehdjk.com/Article/details/ggpoyzjhz.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fktsv.cn/Article/details/guvoigbha.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.epnwcf.com/Article/details/ghenyuaoi.sHtML

[U08] Py：展平二维列表
来源：http://www.share.sjlbkw.cn/Article/details/gplbegfxl.sHtML

[y for x in nested for y in x]
来源：http://blog.epnwcf.com/Article/details/gpjyhudxl.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.sjlbkw.cn/Article/details/gbbywyxvt.sHtML

max(d, key=d.get)
来源：http://3g.fktsv.cn/Article/details/gvmzztdlc.sHtML

[U10] Py：按值排序字典
来源：http://3g.vehdjk.com/Article/details/ggiujzmbm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.epnwcf.com/Article/details/ggtyfevyz.sHtML

[U11] Py：生成器表达式
来源：http://baike.fktsv.cn/Article/details/gujitdube.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fktsv.cn/Article/details/gjockxsqq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.epnwcf.com/Article/details/gmkesxrns.sHtML

Counter(arr).most_common(3)
来源：http://read.share.epnwcf.com/Article/details/gxjevycli.sHtML

[U13] Py：固定长度队列
来源：http://m.share.bbcook.cn/Article/details/geqhjzyky.sHtML

deque(maxlen=10)
来源：http://www.m.share.sjlbkw.cn/Article/details/gimgvuacr.sHtML

[U14] Py：分组收集到列表
来源：http://blog.epnwcf.com/Article/details/gclypskxz.sHtML

defaultdict(list)
来源：http://baike.epnwcf.com/Article/details/giyytmlaw.sHtML

[U15] Py：高精度计时
来源：http://www.share.vehdjk.com/Article/details/grjcvofuu.sHtML

t = time.perf_counter()
来源：http://mobile.epnwcf.com/Article/details/ghdolwsrh.sHtML

[U16] Py：命令行参数解析
来源：http://3g.vehdjk.com/Article/details/gdmmnnypy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.yfazqb.com/Article/details/gpbkwevzm.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.bbcook.cn/Article/details/gvxskgxll.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fktsv.cn/Article/details/ghqkhkjyb.sHtML

[U18] Py：预编译正则
来源：http://baike.fktsv.cn/Article/details/gdqbxbrkf.sHtML

pat = re.compile(r"\d+")
来源：http://3g.tarul.cn/Article/details/gdyezribr.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.epnwcf.com/Article/details/gjlpgguys.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fktsv.cn/Article/details/gnyagahjp.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.tarul.cn/Article/details/gjcpmhjfd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fktsv.cn/Article/details/gabrduaqf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.tarul.cn/Article/details/gtxjehsde.sHtML

@contextlib.contextmanager
来源：http://www.blog.epnwcf.com/Article/details/gofupljuc.sHtML

[U22] Py：矩阵转置
来源：http://baike.tarul.cn/Article/details/gdbcifsjz.sHtML

list(zip(*m))
来源：http://baike.vehdjk.com/Article/details/gakgrrrhf.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fktsv.cn/Article/details/gkgyzrvpf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fktsv.cn/Article/details/gfxuvqome.sHtML

[U24] Py：路径操作
来源：http://www.blog.fktsv.cn/Article/details/gqjsqwwyq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.vehdjk.com/Article/details/gfdiuxtkq.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.epnwcf.com/Article/details/gkysxgcje.sHtML

csv.DictReader(f)
来源：http://www.share.sjlbkw.cn/Article/details/gegqjsevn.sHtML

[U26] Py：并发下载
来源：http://www.blog.yfazqb.com/Article/details/guubpwisq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.yfazqb.com/Article/details/gfkblpvwf.sHtML

[U27] Py：异步 HTTP
来源：http://blog.tarul.cn/Article/details/gdptgkmqz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.bbcook.cn/Article/details/ghxsdhlqi.sHtML

[U28] Py：类型别名
来源：http://m.share.yfazqb.com/Article/details/gyfqxevpd.sHtML

UserId = int
来源：http://blog.fktsv.cn/Article/details/gkzkiuqup.sHtML

[U29] Py：属性校验
来源：http://read.share.vehdjk.com/Article/details/ghisudycd.sHtML

@property 与 @x.setter 配合
来源：http://mobile.tarul.cn/Article/details/gxrhxrstv.sHtML

[U30] Py：数据类
来源：http://mobile.bbcook.cn/Article/details/gkoekbzdi.sHtML

@dataclass(slots=True)
来源：http://m.share.vehdjk.com/Article/details/grmzpwljz.sHtML

[U31] Py：单测
来源：http://read.share.fktsv.cn/Article/details/gjsviywlv.sHtML

python -m pytest -q
来源：http://blog.tarul.cn/Article/details/gzkysvnct.sHtML

[U32] Py：代码格式化
来源：http://baike.yfazqb.com/Article/details/geldwuhup.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.sjlbkw.cn/Article/details/gdpuffzpy.sHtML

[U33] Py：打包发布
来源：http://www.m.share.yfazqb.com/Article/details/gdztpgmxq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.epnwcf.com/Article/details/gozuwojwp.sHtML

[U34] Py：判断编码
来源：http://m.share.tarul.cn/Article/details/gqbqgqpcs.sHtML

chardet.detect(raw)
来源：http://www.m.share.bbcook.cn/Article/details/ghzssddfx.sHtML

[U35] Py：发送邮件
来源：http://read.share.vehdjk.com/Article/details/gafhyorqr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.sjlbkw.cn/Article/details/geltkknjf.sHtML

[U36] Py：定时任务
来源：http://www.m.share.epnwcf.com/Article/details/ghpsqbmpp.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fktsv.cn/Article/details/gzqyvioxa.sHtML

[U37] Py：读写 Excel
来源：http://m.share.tarul.cn/Article/details/gtgvnrmbn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.bbcook.cn/Article/details/gztgqjqhn.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.epnwcf.com/Article/details/gdpdzloiz.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fktsv.cn/Article/details/gcgpvgztv.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.epnwcf.com/Article/details/geelbdonr.sHtML

sys.stdout.isatty()
来源：http://baike.epnwcf.com/Article/details/goxbulbei.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.epnwcf.com/Article/details/gqeoazfyq.sHtML

print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/grgwzxolz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.yfazqb.com/Article/details/gosignjrl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.vehdjk.com/Article/details/glrqgqthm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.sjlbkw.cn/Article/details/gaogjlzyh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.vehdjk.com/Article/details/gjilfedlx.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.epnwcf.com/Article/details/gavtrvwur.sHtML

namespace App\Http;
来源：http://m.share.tarul.cn/Article/details/gbricdhat.sHtML

[U44] PHP：开启严格类型
来源：http://wap.vehdjk.com/Article/details/gwvatdntm.sHtML

declare(strict_types=1);
来源：http://mobile.tarul.cn/Article/details/gegcqcqbg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.tarul.cn/Article/details/gzkldbrye.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gaumqsoiu.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.vehdjk.com/Article/details/gextelrvp.sHtML

?string $name = null
来源：http://baike.vehdjk.com/Article/details/gqczggmlk.sHtML

[U47] PHP：联合类型
来源：http://blog.fktsv.cn/Article/details/gpmltlzlm.sHtML

int|string $id
来源：http://mobile.fktsv.cn/Article/details/gnayaiikg.sHtML

[U48] PHP：纯枚举
来源：http://wap.epnwcf.com/Article/details/guvaccbrn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.vehdjk.com/Article/details/gznkvlvef.sHtML

[U49] PHP：只读属性
来源：http://3g.sjlbkw.cn/Article/details/glkjnsbxn.sHtML

public readonly string $name
来源：http://www.blog.sjlbkw.cn/Article/details/gidoqtoms.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.sjlbkw.cn/Article/details/gqrinyqej.sHtML

public function __construct(private int $id) {}
来源：http://www.share.vehdjk.com/Article/details/gnuoynbak.sHtML

[U51] PHP：数组解构
来源：http://baike.yfazqb.com/Article/details/ggmqykgxr.sHtML

[$a, $b] = $arr;
来源：http://3g.sjlbkw.cn/Article/details/gizuytgvx.sHtML

[U52] PHP：箭头函数
来源：http://blog.epnwcf.com/Article/details/gpemdqspx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.vehdjk.com/Article/details/gjojyswzw.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.yfazqb.com/Article/details/gxytzvkri.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.sjlbkw.cn/Article/details/gkysjlftg.sHtML

[U54] PHP：空安全调用
来源：http://mobile.yfazqb.com/Article/details/gqrmabjjd.sHtML

$obj?->method()
来源：http://read.share.sjlbkw.cn/Article/details/glvpcaamr.sHtML

[U55] PHP：match 表达式
来源：http://baike.tarul.cn/Article/details/gddjdooas.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.yfazqb.com/Article/details/guatayreb.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gfqdxdrlx.sHtML

f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gydqnfebx.sHtML

[U57] PHP：字符串插值
来源：http://m.share.yfazqb.com/Article/details/govgsuyqq.sHtML

"值: {$a}"
来源：http://3g.sjlbkw.cn/Article/details/giamgvdgs.sHtML

[U58] PHP：数组三件套
来源：http://read.share.vehdjk.com/Article/details/giignltmq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gvaexfkoa.sHtML

[U59] PHP：自定义排序
来源：http://baike.vehdjk.com/Article/details/gnxsxmhvt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.sjlbkw.cn/Article/details/gtgfkfcmj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.bbcook.cn/Article/details/gwypkaxfj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.sjlbkw.cn/Article/details/gouiecaqx.sHtML

[U61] PHP：正则
来源：http://wap.yfazqb.com/Article/details/gzstxdxsh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.yfazqb.com/Article/details/gvxpzpykl.sHtML

[U62] PHP：日期对象
来源：http://wap.bbcook.cn/Article/details/gnuckeqxp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.vehdjk.com/Article/details/gtjytftgw.sHtML

[U63] PHP：文件读写
来源：http://3g.tarul.cn/Article/details/gwjceongl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.yfazqb.com/Article/details/galocfxqm.sHtML

[U64] PHP：目录遍历
来源：http://baike.epnwcf.com/Article/details/gfqvrptfv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.bbcook.cn/Article/details/gadwgoots.sHtML

[U65] PHP：会话
来源：http://3g.yfazqb.com/Article/details/gugexzaza.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.bbcook.cn/Article/details/gwkvnnnrt.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fktsv.cn/Article/details/gzogtnxxr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.tarul.cn/Article/details/gwnsonkgm.sHtML

[U67] PHP：处理文件上传
来源：http://baike.tarul.cn/Article/details/ghekireep.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.vehdjk.com/Article/details/gwplfikdb.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.epnwcf.com/Article/details/ggnbanexv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.bbcook.cn/Article/details/gqpvlygjy.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.sjlbkw.cn/Article/details/gqenjpuss.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.bbcook.cn/Article/details/gbdssnmae.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.epnwcf.com/Article/details/gwzdrvnoz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.yfazqb.com/Article/details/gopsxvtli.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gqzxvekgg.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.epnwcf.com/Article/details/gczfbiqmp.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.bbcook.cn/Article/details/gqrszlbgx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.bbcook.cn/Article/details/gzsrwjpcn.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fktsv.cn/Article/details/godzuozfm.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.vehdjk.com/Article/details/gcskxvjkb.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gxunvptys.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.tarul.cn/Article/details/gbrmghqrl.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.sjlbkw.cn/Article/details/gvqmjfpjp.sHtML

composer require psr/container
来源：http://www.share.epnwcf.com/Article/details/gomxiwjju.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.epnwcf.com/Article/details/gubezvaft.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.bbcook.cn/Article/details/gmljwwvtc.sHtML

[U77] PHP：模板渲染
来源：http://3g.sjlbkw.cn/Article/details/gonyduljm.sHtML

composer require twig/twig
来源：http://baike.fktsv.cn/Article/details/gtvojzxuc.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.vehdjk.com/Article/details/gkxepbqds.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.tarul.cn/Article/details/gznfatfxd.sHtML

[U79] PHP：静态分析
来源：http://www.share.tarul.cn/Article/details/gnsxzwugs.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.vehdjk.com/Article/details/gdefjskjo.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fktsv.cn/Article/details/ggpzjumzt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.tarul.cn/Article/details/gskcnhpoz.sHtML

[U81] JS：初始化项目
来源：http://m.share.epnwcf.com/Article/details/gdnaedxlq.sHtML

npm init -y;  npm i express
来源：http://blog.tarul.cn/Article/details/gimlxhhgm.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.tarul.cn/Article/details/gndmrxtzl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.epnwcf.com/Article/details/glonkaane.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.bbcook.cn/Article/details/gwblvfjed.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gishtalmz.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fktsv.cn/Article/details/gdoxehwbc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.sjlbkw.cn/Article/details/gufbutjrx.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/gqgdjetpp.sHtML

a?.b?.c
来源：http://read.share.yfazqb.com/Article/details/gyyekveic.sHtML

[U86] JS：空值合并
来源：http://www.blog.epnwcf.com/Article/details/gehqcipnf.sHtML

a ?? b
来源：http://www.blog.sjlbkw.cn/Article/details/gyqxivdze.sHtML

[U87] JS：解构默认值
来源：http://www.blog.bbcook.cn/Article/details/gwhyfillb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.vehdjk.com/Article/details/gulafzmtl.sHtML

[U88] JS：对象展开合并
来源：http://baike.fktsv.cn/Article/details/gfwfansjb.sHtML

{ ...a, ...b }
来源：http://mobile.yfazqb.com/Article/details/gpvdbslcl.sHtML

[U89] JS：数组去重
来源：http://m.share.epnwcf.com/Article/details/gaqxpzhcj.sHtML

[...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gujohxpap.sHtML

[U90] JS：数字数组排序
来源：http://3g.yfazqb.com/Article/details/gpehcsgik.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gajaosjux.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.yfazqb.com/Article/details/gbcizuplb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.epnwcf.com/Article/details/gcyhsifor.sHtML

[U92] JS：深拷贝
来源：http://m.share.bbcook.cn/Article/details/ggoaukuyg.sHtML

structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gqzhjwfpj.sHtML


<!-- 参考信息 -->