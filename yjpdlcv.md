代发 wailian999

[T03] Kotlin：字符串模板
来源：http://blog.tarul.cn/Article/details/gdnhfkcmz.sHtML

"值: $b"
来源：http://mobile.bbcook.cn/Article/details/gohungpmn.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.yfazqb.com/Article/details/goaijmmzj.sHtML

val n: String? = null;  n?.length
来源：http://blog.yfazqb.com/Article/details/glevbhyiy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.epnwcf.com/Article/details/gfqsmtfmx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.yfazqb.com/Article/details/gmdgjdyqj.sHtML

[T06] Kotlin：集合映射
来源：http://baike.sjlbkw.cn/Article/details/gfskdyjwf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gyljzznpx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.yfazqb.com/Article/details/gutvrsivp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fktsv.cn/Article/details/gjuuwwlqg.sHtML

[T08] Kotlin：数据类
来源：http://mobile.tarul.cn/Article/details/geglufgnw.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fktsv.cn/Article/details/gzlfhplqa.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.sjlbkw.cn/Article/details/gbbuipwun.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/gajnkgtnj.sHtML

[T10] Kotlin：默认参数
来源：http://3g.tarul.cn/Article/details/gebjpiazv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.tarul.cn/Article/details/gqcsgyoef.sHtML

[T11] Kotlin：协程
来源：http://www.blog.tarul.cn/Article/details/gradtoqly.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.bbcook.cn/Article/details/golouyjlo.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fktsv.cn/Article/details/grooaelnw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gieborayv.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fktsv.cn/Article/details/gnqkpwlri.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/gmregbpen.sHtML

[T14] Kotlin：循环
来源：http://3g.epnwcf.com/Article/details/gxqzafhwk.sHtML

for (i in 1..10) println(i)
来源：http://blog.tarul.cn/Article/details/gmaxoxhvw.sHtML

[T15] Kotlin：接口
来源：http://m.share.fktsv.cn/Article/details/gzxffrxtp.sHtML

interface Shape { fun area(): Double }
来源：http://wap.bbcook.cn/Article/details/gpbztffjs.sHtML

[T16] Swift：Hello World
来源：http://m.share.epnwcf.com/Article/details/gycpnnsjj.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/gbzvpdhql.sHtML

[T17] Swift：变量与常量
来源：http://blog.bbcook.cn/Article/details/gtssbhyvg.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/gbvkrwpch.sHtML

[T18] Swift：字符串插值
来源：http://m.share.bbcook.cn/Article/details/glckgbtui.sHtML

"值: \(b)"
来源：http://www.blog.vehdjk.com/Article/details/grioxpgex.sHtML

[T19] Swift：可选绑定
来源：http://read.share.epnwcf.com/Article/details/gkpbxqbcy.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.yfazqb.com/Article/details/gfhuouwhw.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/grzwbvexc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.tarul.cn/Article/details/gwnervajd.sHtML

[T21] Swift：遍历
来源：http://www.blog.sjlbkw.cn/Article/details/ghfaiicbj.sHtML

for x in a { print(x) }
来源：http://m.share.bbcook.cn/Article/details/guwlyipmq.sHtML

[T22] Swift：字典
来源：http://blog.tarul.cn/Article/details/guewxsxee.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.epnwcf.com/Article/details/gtfuftfdq.sHtML

[T23] Swift：函数
来源：http://read.share.bbcook.cn/Article/details/gniqyevua.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.bbcook.cn/Article/details/gfvayxfjo.sHtML

[T24] Swift：闭包
来源：http://3g.yfazqb.com/Article/details/ghhbhpltx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.tarul.cn/Article/details/gmfhydxxy.sHtML

[T25] Swift：结构体
来源：http://baike.sjlbkw.cn/Article/details/gwoqfkvjo.sHtML

struct P { var x: Int }
来源：http://www.share.vehdjk.com/Article/details/ggsksodqt.sHtML

[T26] Swift：类与重写
来源：http://baike.yfazqb.com/Article/details/ggqdtpztz.sHtML

class A: Base { override func f() {} }
来源：http://wap.sjlbkw.cn/Article/details/gquoomxsr.sHtML

[T27] Swift：错误处理
来源：http://blog.tarul.cn/Article/details/gxxwsnzxw.sHtML

do { try f() } catch { print(error) }
来源：http://3g.bbcook.cn/Article/details/gkwggczaq.sHtML

[T28] Swift：枚举
来源：http://wap.yfazqb.com/Article/details/gqxsiwpms.sHtML

enum Color { case red, green }
来源：http://www.m.share.vehdjk.com/Article/details/gmpccmsab.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/guaoviabs.sHtML

guard let x = opt else { return }
来源：http://wap.epnwcf.com/Article/details/gmfibzzse.sHtML

[T30] Swift：协议
来源：http://read.share.yfazqb.com/Article/details/gzrpxnxyc.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.tarul.cn/Article/details/gybesgegl.sHtML

[T31] Lua：Hello World
来源：http://3g.yfazqb.com/Article/details/gpknjsysj.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gwtzozdqr.sHtML

[T32] Lua：局部变量
来源：http://www.share.epnwcf.com/Article/details/ginbyfdkl.sHtML

local a = 1
来源：http://blog.vehdjk.com/Article/details/gsogmyjed.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fktsv.cn/Article/details/gjouokiwn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fktsv.cn/Article/details/ghubtspsy.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/gfbkdncyi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.yfazqb.com/Article/details/giyaptnge.sHtML

[T35] Lua：字典表
来源：http://read.share.bbcook.cn/Article/details/gxpgwtdxa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fktsv.cn/Article/details/gihhbagzz.sHtML

[T36] Lua：函数
来源：http://www.share.tarul.cn/Article/details/gxrjeavhc.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.tarul.cn/Article/details/gtxekicud.sHtML

[T37] Lua：字符串拼接
来源：http://baike.sjlbkw.cn/Article/details/ghbqhhjpq.sHtML

"a" .. "b"
来源：http://read.share.tarul.cn/Article/details/gismamvci.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/gojaylquc.sHtML

if x > 0 then print("正") end
来源：http://wap.vehdjk.com/Article/details/gdjeqwvrk.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gqjchmpcw.sHtML

string.find(s, "%d+")
来源：http://www.m.share.epnwcf.com/Article/details/gkpqvjnle.sHtML

[T40] Lua：元表
来源：http://mobile.yfazqb.com/Article/details/gbyrzhduk.sHtML

setmetatable({}, { __index = base })
来源：http://baike.bbcook.cn/Article/details/gloswdglm.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/golqdegbz.sHtML

print "Hello\n";
来源：http://m.share.tarul.cn/Article/details/gnfxtbvvu.sHtML

[T42] Perl：变量类型
来源：http://www.blog.bbcook.cn/Article/details/gzuefjmlq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.yfazqb.com/Article/details/gdrunwrjz.sHtML

[T43] Perl：字符串插值
来源：http://wap.tarul.cn/Article/details/godusiowz.sHtML

"值: $a"
来源：http://m.share.vehdjk.com/Article/details/gjiuxsgip.sHtML

[T44] Perl：条件
来源：http://3g.epnwcf.com/Article/details/gafpidyav.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.bbcook.cn/Article/details/gbgyuabhk.sHtML

[T45] Perl：数组遍历
来源：http://read.share.epnwcf.com/Article/details/gqszhwqst.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.yfazqb.com/Article/details/gwptckzau.sHtML

[T46] Perl：哈希操作
来源：http://mobile.bbcook.cn/Article/details/gzqlflczc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fktsv.cn/Article/details/gpmrectsm.sHtML

[T47] Perl：正则捕获
来源：http://m.share.epnwcf.com/Article/details/guxubasph.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.tarul.cn/Article/details/gdmvsxgha.sHtML

[T48] Perl：正则替换
来源：http://mobile.vehdjk.com/Article/details/gqgnuqfks.sHtML

$s =~ s/old/new/g;
来源：http://baike.tarul.cn/Article/details/gstizsbpr.sHtML

[T49] Perl：函数
来源：http://www.m.share.bbcook.cn/Article/details/grqjqnrck.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gqmyyfirr.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gocpaujpp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fktsv.cn/Article/details/gdayarsxu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.bbcook.cn/Article/details/ggffdczvp.sHtML

[T51] Scala：Hello World
来源：http://3g.yfazqb.com/Article/details/gqeirvaup.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/gvqwbmjev.sHtML

[T52] Scala：变量
来源：http://baike.tarul.cn/Article/details/gqvluxefs.sHtML

val a = 1;  var b = 2
来源：http://read.share.bbcook.cn/Article/details/gslsacjwr.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gfmewxsww.sHtML

s"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gljimlkkg.sHtML

[T54] Scala：集合映射
来源：http://www.blog.tarul.cn/Article/details/gbjnutmqa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.epnwcf.com/Article/details/gwljangan.sHtML

[T55] Scala：集合过滤
来源：http://baike.fktsv.cn/Article/details/gorkhapmd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.tarul.cn/Article/details/gvpniiqki.sHtML

[T56] Scala：样例类
来源：http://mobile.bbcook.cn/Article/details/gqurowgcg.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.tarul.cn/Article/details/gmvvgsbyt.sHtML

[T57] Scala：模式匹配
来源：http://www.share.epnwcf.com/Article/details/gyswqeuvi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.bbcook.cn/Article/details/gyefxczrd.sHtML

[T58] Scala：函数定义
来源：http://3g.sjlbkw.cn/Article/details/gmiffsbaj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.epnwcf.com/Article/details/gcfndufvz.sHtML

[T59] Scala：循环
来源：http://www.blog.bbcook.cn/Article/details/gkeglpqpc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gmdneqbed.sHtML

[T60] Scala：折叠
来源：http://www.share.sjlbkw.cn/Article/details/gvbukboqe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fktsv.cn/Article/details/gajxpopdb.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gjzjfjgqh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/gvxfikpkw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gaietypbe.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.tarul.cn/Article/details/gxlcenubj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.vehdjk.com/Article/details/gjdzrcyal.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.yfazqb.com/Article/details/goumtnrux.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fktsv.cn/Article/details/gfnxmzbce.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.epnwcf.com/Article/details/gxezzbayi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.sjlbkw.cn/Article/details/gbbxbycdc.sHtML

[U04] Py：变量调试打印
来源：http://read.share.bbcook.cn/Article/details/grtkanmpi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.yfazqb.com/Article/details/goljlrtey.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fktsv.cn/Article/details/gqevxqtji.sHtML

list(dict.fromkeys(arr))
来源：http://3g.vehdjk.com/Article/details/gthuxqkbj.sHtML

[U06] Py：合并两个字典
来源：http://3g.bbcook.cn/Article/details/gotwmpjyy.sHtML

{**a, **b}
来源：http://3g.sjlbkw.cn/Article/details/gzahrrvin.sHtML

[U07] Py：反转字典键值
来源：http://mobile.epnwcf.com/Article/details/gpewkysok.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fktsv.cn/Article/details/gxcroigxb.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fktsv.cn/Article/details/gmedehfqm.sHtML

[y for x in nested for y in x]
来源：http://www.share.fktsv.cn/Article/details/gzoukogcj.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fktsv.cn/Article/details/gzixwjjez.sHtML

max(d, key=d.get)
来源：http://read.share.yfazqb.com/Article/details/gnipgbncr.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.tarul.cn/Article/details/gtjlupwkg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.tarul.cn/Article/details/gpvurncok.sHtML

[U11] Py：生成器表达式
来源：http://wap.epnwcf.com/Article/details/gdtadeavk.sHtML

(x * 2 for x in arr)
来源：http://blog.sjlbkw.cn/Article/details/ggawnzxos.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/gujijdzsg.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fktsv.cn/Article/details/gmtdbrars.sHtML

[U13] Py：固定长度队列
来源：http://baike.epnwcf.com/Article/details/gadpezssm.sHtML

deque(maxlen=10)
来源：http://www.blog.vehdjk.com/Article/details/gkwcpxbpj.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.bbcook.cn/Article/details/gwsghtqin.sHtML

defaultdict(list)
来源：http://baike.vehdjk.com/Article/details/gpbiaebdr.sHtML

[U15] Py：高精度计时
来源：http://blog.tarul.cn/Article/details/gvpgjuyqv.sHtML

t = time.perf_counter()
来源：http://wap.fktsv.cn/Article/details/gbedyvvli.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fktsv.cn/Article/details/ggeqthrrp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fktsv.cn/Article/details/ggdezmxha.sHtML

[U17] Py：初始化日志
来源：http://www.blog.epnwcf.com/Article/details/ghjfdamlp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.bbcook.cn/Article/details/gzzydhalu.sHtML

[U18] Py：预编译正则
来源：http://read.share.epnwcf.com/Article/details/gphwacort.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.vehdjk.com/Article/details/gadwyyvse.sHtML

[U19] Py：正则替换带回调
来源：http://baike.tarul.cn/Article/details/gkufpqqgx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.vehdjk.com/Article/details/gmdmeyymn.sHtML

[U20] Py：缓存函数结果
来源：http://3g.vehdjk.com/Article/details/gvwwjorvs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.tarul.cn/Article/details/gbpxjmcng.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.epnwcf.com/Article/details/gpbxervaf.sHtML

@contextlib.contextmanager
来源：http://m.share.yfazqb.com/Article/details/gqitrqhks.sHtML

[U22] Py：矩阵转置
来源：http://baike.tarul.cn/Article/details/gnzjvxdbs.sHtML

list(zip(*m))
来源：http://read.share.yfazqb.com/Article/details/gujcctvoh.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.tarul.cn/Article/details/gdllnmizq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fktsv.cn/Article/details/gcjpjjhyw.sHtML

[U24] Py：路径操作
来源：http://baike.yfazqb.com/Article/details/gyaapzgsp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/gvywgulkb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.bbcook.cn/Article/details/gyyfqgaop.sHtML

csv.DictReader(f)
来源：http://baike.epnwcf.com/Article/details/gaalmhsvd.sHtML

[U26] Py：并发下载
来源：http://www.m.share.vehdjk.com/Article/details/gizscupor.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.bbcook.cn/Article/details/genbongov.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fktsv.cn/Article/details/gyutqmjgl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.sjlbkw.cn/Article/details/grvukwhfn.sHtML

[U28] Py：类型别名
来源：http://wap.epnwcf.com/Article/details/gmtnqukcr.sHtML

UserId = int
来源：http://read.share.yfazqb.com/Article/details/gziemxhrn.sHtML

[U29] Py：属性校验
来源：http://wap.tarul.cn/Article/details/gwnhznxgy.sHtML

@property 与 @x.setter 配合
来源：http://m.share.epnwcf.com/Article/details/gnwmrqask.sHtML

[U30] Py：数据类
来源：http://blog.vehdjk.com/Article/details/gpiovpqqw.sHtML

@dataclass(slots=True)
来源：http://www.blog.tarul.cn/Article/details/gcacgxnwf.sHtML

[U31] Py：单测
来源：http://blog.vehdjk.com/Article/details/gpbjoompg.sHtML

python -m pytest -q
来源：http://blog.bbcook.cn/Article/details/goavqcfnm.sHtML

[U32] Py：代码格式化
来源：http://www.share.yfazqb.com/Article/details/gjkxzfsre.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.vehdjk.com/Article/details/gmggqtjfu.sHtML

[U33] Py：打包发布
来源：http://3g.sjlbkw.cn/Article/details/gspzvsmmi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.vehdjk.com/Article/details/gqubmauni.sHtML

[U34] Py：判断编码
来源：http://blog.epnwcf.com/Article/details/gihxhuoor.sHtML

chardet.detect(raw)
来源：http://www.blog.yfazqb.com/Article/details/gckvfhpjc.sHtML

[U35] Py：发送邮件
来源：http://read.share.epnwcf.com/Article/details/grzsuggqr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.epnwcf.com/Article/details/gpwjyobqa.sHtML

[U36] Py：定时任务
来源：http://blog.vehdjk.com/Article/details/gcnqltjko.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.tarul.cn/Article/details/gkmqvkvft.sHtML

[U37] Py：读写 Excel
来源：http://blog.fktsv.cn/Article/details/grnlagjsr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.sjlbkw.cn/Article/details/gcltcpqsm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.yfazqb.com/Article/details/ghaahwtsm.sHtML

Path(__file__).resolve().parent
来源：http://blog.sjlbkw.cn/Article/details/gihularwg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.vehdjk.com/Article/details/gfrvfirmz.sHtML

sys.stdout.isatty()
来源：http://www.blog.tarul.cn/Article/details/gktevzmzf.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fktsv.cn/Article/details/gwfxvybko.sHtML

print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gqszbkrfn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.bbcook.cn/Article/details/grggknrhs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.yfazqb.com/Article/details/gxhgjlyen.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.bbcook.cn/Article/details/gtcfbwxsv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fktsv.cn/Article/details/gqbjjrlcq.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.vehdjk.com/Article/details/gtcudvcyt.sHtML

namespace App\Http;
来源：http://3g.fktsv.cn/Article/details/gcxyqzedz.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fktsv.cn/Article/details/gdadlztur.sHtML

declare(strict_types=1);
来源：http://www.share.epnwcf.com/Article/details/gcokcvbkm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.bbcook.cn/Article/details/gozaawzzs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gwyzfuwrx.sHtML

[U46] PHP：可空类型
来源：http://m.share.yfazqb.com/Article/details/gxiquwscc.sHtML

?string $name = null
来源：http://mobile.tarul.cn/Article/details/gdyvxdupl.sHtML

[U47] PHP：联合类型
来源：http://m.share.epnwcf.com/Article/details/gzhdllnad.sHtML

int|string $id
来源：http://baike.yfazqb.com/Article/details/gvncaaosq.sHtML

[U48] PHP：纯枚举
来源：http://baike.tarul.cn/Article/details/gfrygohdd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.sjlbkw.cn/Article/details/gnlcztgfd.sHtML

[U49] PHP：只读属性
来源：http://www.share.bbcook.cn/Article/details/gzdncgbqc.sHtML

public readonly string $name
来源：http://wap.yfazqb.com/Article/details/gynrnznmh.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.vehdjk.com/Article/details/gtznkfabf.sHtML

public function __construct(private int $id) {}
来源：http://3g.bbcook.cn/Article/details/ghnamitbu.sHtML

[U51] PHP：数组解构
来源：http://www.share.epnwcf.com/Article/details/gnymlnwkm.sHtML

[$a, $b] = $arr;
来源：http://m.share.tarul.cn/Article/details/goxkfatls.sHtML

[U52] PHP：箭头函数
来源：http://blog.yfazqb.com/Article/details/gtttchaji.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.yfazqb.com/Article/details/glopscjan.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fktsv.cn/Article/details/gnhnwwkav.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fktsv.cn/Article/details/ggxwimizd.sHtML

[U54] PHP：空安全调用
来源：http://blog.bbcook.cn/Article/details/gogpnibii.sHtML

$obj?->method()
来源：http://3g.vehdjk.com/Article/details/gyxkiscwa.sHtML

[U55] PHP：match 表达式
来源：http://read.share.epnwcf.com/Article/details/gxcrrdxcx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.vehdjk.com/Article/details/gbapefcvh.sHtML

[U56] PHP：命名参数
来源：http://3g.yfazqb.com/Article/details/gogknpgdx.sHtML

f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gqbsptlxh.sHtML

[U57] PHP：字符串插值
来源：http://blog.epnwcf.com/Article/details/gkdbmvkgh.sHtML

"值: {$a}"
来源：http://www.share.yfazqb.com/Article/details/glzixddol.sHtML

[U58] PHP：数组三件套
来源：http://mobile.epnwcf.com/Article/details/gweyinuji.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.epnwcf.com/Article/details/gioamstzj.sHtML

[U59] PHP：自定义排序
来源：http://wap.sjlbkw.cn/Article/details/gdmpshatm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gwsmwfitf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqwnabrv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.epnwcf.com/Article/details/gibsgykim.sHtML

[U61] PHP：正则
来源：http://baike.bbcook.cn/Article/details/gjgunkqqq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.yfazqb.com/Article/details/gszggpmnu.sHtML

[U62] PHP：日期对象
来源：http://baike.yfazqb.com/Article/details/gwdaqdgih.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fktsv.cn/Article/details/gogdwrnur.sHtML

[U63] PHP：文件读写
来源：http://blog.epnwcf.com/Article/details/ggubutbdu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.bbcook.cn/Article/details/gppjdsgjr.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gzhdmjgbt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.vehdjk.com/Article/details/gtollxyke.sHtML

[U65] PHP：会话
来源：http://wap.bbcook.cn/Article/details/gaggxxkfx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gfobfuytd.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.epnwcf.com/Article/details/glgikahyi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.tarul.cn/Article/details/gjllxnzrg.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.vehdjk.com/Article/details/gcdwbmdtv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.epnwcf.com/Article/details/gzdxxayih.sHtML

[U68] PHP：PDO 连接
来源：http://baike.epnwcf.com/Article/details/gewntvlob.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.sjlbkw.cn/Article/details/gxuvibvfu.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.vehdjk.com/Article/details/ghemuqvlv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.sjlbkw.cn/Article/details/gobajgjfb.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fktsv.cn/Article/details/gubegfahj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.yfazqb.com/Article/details/gkwhqprnp.sHtML

[U71] PHP：抛出异常
来源：http://m.share.yfazqb.com/Article/details/gzpnybxfh.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.tarul.cn/Article/details/gjffucqde.sHtML

[U72] PHP：写错误日志
来源：http://read.share.tarul.cn/Article/details/ggisbefea.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.sjlbkw.cn/Article/details/gvjoaupvj.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.yfazqb.com/Article/details/gsejphdlb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.bbcook.cn/Article/details/gcaozrhrj.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fktsv.cn/Article/details/gvpqhoiso.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.tarul.cn/Article/details/gyrplnqas.sHtML

[U75] PHP：依赖注入
来源：http://m.share.yfazqb.com/Article/details/gmqhsvatk.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/grpdvcjsj.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fktsv.cn/Article/details/ghjoqizhx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fktsv.cn/Article/details/gyznjkymv.sHtML

[U77] PHP：模板渲染
来源：http://blog.vehdjk.com/Article/details/gohohsgoq.sHtML

composer require twig/twig
来源：http://www.m.share.tarul.cn/Article/details/guqslqrky.sHtML

[U78] PHP：单元测试
来源：http://blog.fktsv.cn/Article/details/glljuuitk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.vehdjk.com/Article/details/gzerrelni.sHtML

[U79] PHP：静态分析
来源：http://blog.fktsv.cn/Article/details/gjpmswhhu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.yfazqb.com/Article/details/ghbkbggxb.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.sjlbkw.cn/Article/details/gzmcbrvix.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fktsv.cn/Article/details/glmpeoxrd.sHtML

[U81] JS：初始化项目
来源：http://mobile.sjlbkw.cn/Article/details/gvwvtpajp.sHtML

npm init -y;  npm i express
来源：http://wap.vehdjk.com/Article/details/gffsgdihn.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fktsv.cn/Article/details/gadomjvhn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.tarul.cn/Article/details/gutbukjjb.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.epnwcf.com/Article/details/gpngjxktq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.bbcook.cn/Article/details/ginafyque.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.bbcook.cn/Article/details/gnwgrvhee.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.sjlbkw.cn/Article/details/ghcvhjxwo.sHtML

[U85] JS：可选链
来源：http://read.share.bbcook.cn/Article/details/gczybvaan.sHtML

a?.b?.c
来源：http://www.share.vehdjk.com/Article/details/gdodaavqn.sHtML

[U86] JS：空值合并
来源：http://www.blog.tarul.cn/Article/details/gkwdjjsvu.sHtML

a ?? b
来源：http://3g.tarul.cn/Article/details/gdkijnunp.sHtML

[U87] JS：解构默认值
来源：http://mobile.yfazqb.com/Article/details/gfvshrwzh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.sjlbkw.cn/Article/details/gpyvsysvf.sHtML

[U88] JS：对象展开合并
来源：http://mobile.bbcook.cn/Article/details/gujselgma.sHtML

{ ...a, ...b }
来源：http://m.share.epnwcf.com/Article/details/ghymnzomw.sHtML

[U89] JS：数组去重
来源：http://m.share.yfazqb.com/Article/details/gujvocvwo.sHtML

[...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gjrkfctpr.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.vehdjk.com/Article/details/gwlrqpopv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gcvfjgxrt.sHtML


<!-- 参考信息 -->