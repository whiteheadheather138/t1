代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/ggbljhphw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/glrydzqna.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/gycnfvhgx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfttsoatg.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/geharxosd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.bbcook.cn/Article/details/gnnvzzidm.sHtML

[T08] Kotlin：数据类
来源：http://read.share.vehdjk.com/Article/details/gwuiwusvu.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gihkvqakx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.epnwcf.com/Article/details/gglsbgmvv.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fktsv.cn/Article/details/gzrxluvbd.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/ggvuajqlc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.yfazqb.com/Article/details/gkzenmorc.sHtML

[T11] Kotlin：协程
来源：http://m.share.yfazqb.com/Article/details/gnnskfemv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.sjlbkw.cn/Article/details/gmyqcrfng.sHtML

[T12] Kotlin：解构声明
来源：http://baike.bbcook.cn/Article/details/goyqwcvhq.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gauanzavk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/ggndrvxdo.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.bbcook.cn/Article/details/ghnenvygy.sHtML

[T14] Kotlin：循环
来源：http://blog.vehdjk.com/Article/details/gtqyknqeo.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.vehdjk.com/Article/details/gvuxczvak.sHtML

[T15] Kotlin：接口
来源：http://wap.epnwcf.com/Article/details/gftsltgti.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.tarul.cn/Article/details/gziujzxtr.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gmaxkznvm.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gckygzbdw.sHtML

[T17] Swift：变量与常量
来源：http://blog.bbcook.cn/Article/details/gltgiiknv.sHtML

var a = 1;  let b = 2
来源：http://wap.fktsv.cn/Article/details/godbtnokj.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gqlzpqrxz.sHtML

"值: \(b)"
来源：http://www.blog.tarul.cn/Article/details/goortbsmh.sHtML

[T19] Swift：可选绑定
来源：http://blog.fktsv.cn/Article/details/gigvycoox.sHtML

if let n = opt { print(n) }
来源：http://blog.sjlbkw.cn/Article/details/gbeochutx.sHtML

[T20] Swift：数组操作
来源：http://wap.fktsv.cn/Article/details/gzahwfxkp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fktsv.cn/Article/details/glfstvscj.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/gowxjfori.sHtML

for x in a { print(x) }
来源：http://m.share.yfazqb.com/Article/details/gxjttwjma.sHtML

[T22] Swift：字典
来源：http://mobile.vehdjk.com/Article/details/gjvxnwfwh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/grlhfyztu.sHtML

[T23] Swift：函数
来源：http://mobile.sjlbkw.cn/Article/details/gylmlimrb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gfarmwqfq.sHtML

[T24] Swift：闭包
来源：http://mobile.fktsv.cn/Article/details/gdvtqlxft.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gvwolpzas.sHtML

[T25] Swift：结构体
来源：http://wap.tarul.cn/Article/details/gtojgqbqz.sHtML

struct P { var x: Int }
来源：http://wap.yfazqb.com/Article/details/gnitloiuq.sHtML

[T26] Swift：类与重写
来源：http://baike.tarul.cn/Article/details/gutoxixyi.sHtML

class A: Base { override func f() {} }
来源：http://3g.sjlbkw.cn/Article/details/glbpthfih.sHtML

[T27] Swift：错误处理
来源：http://read.share.yfazqb.com/Article/details/gqibuwkgj.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.bbcook.cn/Article/details/glmecbrdk.sHtML

[T28] Swift：枚举
来源：http://m.share.tarul.cn/Article/details/gqrnixbvp.sHtML

enum Color { case red, green }
来源：http://mobile.yfazqb.com/Article/details/grcgpmysv.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.vehdjk.com/Article/details/gvihlflco.sHtML

guard let x = opt else { return }
来源：http://read.share.tarul.cn/Article/details/gvgwbuugm.sHtML

[T30] Swift：协议
来源：http://www.share.tarul.cn/Article/details/gaaghkfwp.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.tarul.cn/Article/details/gfdepaemh.sHtML

[T31] Lua：Hello World
来源：http://blog.bbcook.cn/Article/details/gybdgreiz.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gvfiriiuu.sHtML

[T32] Lua：局部变量
来源：http://3g.yfazqb.com/Article/details/gvztdjvrt.sHtML

local a = 1
来源：http://m.share.epnwcf.com/Article/details/gwogljweb.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.tarul.cn/Article/details/grltdpzfg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.tarul.cn/Article/details/gayfbygpl.sHtML

[T34] Lua：遍历表
来源：http://mobile.epnwcf.com/Article/details/gqkwnxwzf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.sjlbkw.cn/Article/details/gbbknbylj.sHtML

[T35] Lua：字典表
来源：http://read.share.epnwcf.com/Article/details/gptsvmmrx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.vehdjk.com/Article/details/gcgiadzfy.sHtML

[T36] Lua：函数
来源：http://www.m.share.vehdjk.com/Article/details/gthzqsmyx.sHtML

function add(a, b) return a + b end
来源：http://read.share.vehdjk.com/Article/details/glozychtv.sHtML

[T37] Lua：字符串拼接
来源：http://wap.bbcook.cn/Article/details/gnqdigsdr.sHtML

"a" .. "b"
来源：http://www.share.sjlbkw.cn/Article/details/gidamkikt.sHtML

[T38] Lua：条件
来源：http://www.blog.vehdjk.com/Article/details/ghzfwdsbh.sHtML

if x > 0 then print("正") end
来源：http://baike.yfazqb.com/Article/details/gxbpuelkp.sHtML

[T39] Lua：模式匹配
来源：http://m.share.vehdjk.com/Article/details/glmfpsyyy.sHtML

string.find(s, "%d+")
来源：http://read.share.tarul.cn/Article/details/goontukut.sHtML

[T40] Lua：元表
来源：http://blog.vehdjk.com/Article/details/gijuzjxlo.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.tarul.cn/Article/details/guttepuza.sHtML

[T41] Perl：Hello World
来源：http://blog.yfazqb.com/Article/details/gqkfajxxu.sHtML

print "Hello\n";
来源：http://blog.sjlbkw.cn/Article/details/gtnfkzyds.sHtML

[T42] Perl：变量类型
来源：http://www.blog.yfazqb.com/Article/details/gvzuuvnot.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.yfazqb.com/Article/details/gmaipnwaf.sHtML

[T43] Perl：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gcerrtcqf.sHtML

"值: $a"
来源：http://baike.yfazqb.com/Article/details/gzvhsjrvr.sHtML

[T44] Perl：条件
来源：http://read.share.bbcook.cn/Article/details/gqzpaakob.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.vehdjk.com/Article/details/gotdcbsca.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.epnwcf.com/Article/details/ghcsqyykq.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fktsv.cn/Article/details/gmoolvzbg.sHtML

[T46] Perl：哈希操作
来源：http://www.share.epnwcf.com/Article/details/gmvzqabeh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.vehdjk.com/Article/details/gqbhxsfnq.sHtML

[T47] Perl：正则捕获
来源：http://read.share.bbcook.cn/Article/details/gcpuimoxf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.sjlbkw.cn/Article/details/glsaxxxbj.sHtML

[T48] Perl：正则替换
来源：http://m.share.epnwcf.com/Article/details/gfhiekagb.sHtML

$s =~ s/old/new/g;
来源：http://blog.bbcook.cn/Article/details/gqxnbbcml.sHtML

[T49] Perl：函数
来源：http://mobile.yfazqb.com/Article/details/garxhbvng.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gkaprcqiy.sHtML

[T50] Perl：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gtfutaqxz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fktsv.cn/Article/details/gzazvwtkh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.tarul.cn/Article/details/gmrixkyvq.sHtML

[T51] Scala：Hello World
来源：http://wap.fktsv.cn/Article/details/glxbgbtev.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/grhagyszc.sHtML

[T52] Scala：变量
来源：http://3g.fktsv.cn/Article/details/gafuozosb.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrspojdm.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gzmoqxiqz.sHtML

s"值: $b"
来源：http://www.m.share.vehdjk.com/Article/details/gmtxotxrb.sHtML

[T54] Scala：集合映射
来源：http://m.share.tarul.cn/Article/details/gglhkmeyu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.tarul.cn/Article/details/gxjmosdbc.sHtML

[T55] Scala：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gygyzqrqn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.vehdjk.com/Article/details/gipblgogv.sHtML

[T56] Scala：样例类
来源：http://www.share.epnwcf.com/Article/details/gukecfimb.sHtML

case class User(name: String, age: Int)
来源：http://mobile.vehdjk.com/Article/details/gyuegowrz.sHtML

[T57] Scala：模式匹配
来源：http://blog.bbcook.cn/Article/details/gulodvukg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.bbcook.cn/Article/details/gaqqrpfyz.sHtML

[T58] Scala：函数定义
来源：http://read.share.fktsv.cn/Article/details/gcxxruedl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.bbcook.cn/Article/details/gyfwqgecm.sHtML

[T59] Scala：循环
来源：http://m.share.bbcook.cn/Article/details/gyowbhbie.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fktsv.cn/Article/details/gybsjxttz.sHtML

[T60] Scala：折叠
来源：http://blog.fktsv.cn/Article/details/gddxshnpv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fktsv.cn/Article/details/grvmmtigl.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gimxiqpfr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.yfazqb.com/Article/details/gbtpnsdld.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gsmfqjfph.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fktsv.cn/Article/details/gmlatpxyl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.tarul.cn/Article/details/guedzsjcx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.sjlbkw.cn/Article/details/gieskuuis.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fktsv.cn/Article/details/gnozuonzj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.tarul.cn/Article/details/gabpyxlji.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.sjlbkw.cn/Article/details/gmjgtxhsn.sHtML

[U04] Py：变量调试打印
来源：http://www.share.yfazqb.com/Article/details/gtukutksm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.epnwcf.com/Article/details/goiybxnet.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.yfazqb.com/Article/details/gfyguloii.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gdpjyernh.sHtML

[U06] Py：合并两个字典
来源：http://www.share.vehdjk.com/Article/details/gwljlozzs.sHtML

{**a, **b}
来源：http://wap.vehdjk.com/Article/details/gfychblqy.sHtML

[U07] Py：反转字典键值
来源：http://wap.yfazqb.com/Article/details/gmpuwusxk.sHtML

{v: k for k, v in d.items()}
来源：http://wap.vehdjk.com/Article/details/gngczjvee.sHtML

[U08] Py：展平二维列表
来源：http://mobile.sjlbkw.cn/Article/details/gqlvirsfr.sHtML

[y for x in nested for y in x]
来源：http://read.share.bbcook.cn/Article/details/garmrhcxu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.tarul.cn/Article/details/glpysmujh.sHtML

max(d, key=d.get)
来源：http://www.share.epnwcf.com/Article/details/gkxuoshqo.sHtML

[U10] Py：按值排序字典
来源：http://mobile.bbcook.cn/Article/details/goqowvijf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.epnwcf.com/Article/details/gwkwiylwa.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.yfazqb.com/Article/details/glpvmbrdr.sHtML

(x * 2 for x in arr)
来源：http://www.blog.bbcook.cn/Article/details/gmdvhaylf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fktsv.cn/Article/details/geqpptzac.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.tarul.cn/Article/details/gmtjiffgc.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/gieufqumb.sHtML

deque(maxlen=10)
来源：http://read.share.bbcook.cn/Article/details/geentwuxz.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.tarul.cn/Article/details/gqxhlewxu.sHtML

defaultdict(list)
来源：http://wap.yfazqb.com/Article/details/gzttwqbwn.sHtML

[U15] Py：高精度计时
来源：http://3g.vehdjk.com/Article/details/gihzeeksy.sHtML

t = time.perf_counter()
来源：http://3g.epnwcf.com/Article/details/gsjktshnd.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.bbcook.cn/Article/details/grccydjrf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.epnwcf.com/Article/details/grjedxlrq.sHtML

[U17] Py：初始化日志
来源：http://mobile.bbcook.cn/Article/details/gaezlhmff.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.yfazqb.com/Article/details/gaomkgrhn.sHtML

[U18] Py：预编译正则
来源：http://baike.yfazqb.com/Article/details/gsjxwoubj.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fktsv.cn/Article/details/gukxaphoy.sHtML

[U19] Py：正则替换带回调
来源：http://baike.vehdjk.com/Article/details/ggcarhrfy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.yfazqb.com/Article/details/gtxrlihqe.sHtML

[U20] Py：缓存函数结果
来源：http://baike.vehdjk.com/Article/details/gikdftjao.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.vehdjk.com/Article/details/gwbymxhns.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.tarul.cn/Article/details/glzkgjogc.sHtML

@contextlib.contextmanager
来源：http://blog.tarul.cn/Article/details/gupgfqwnj.sHtML

[U22] Py：矩阵转置
来源：http://blog.epnwcf.com/Article/details/gujwmxzgy.sHtML

list(zip(*m))
来源：http://3g.sjlbkw.cn/Article/details/ghlnnrggb.sHtML

[U23] Py：分块读取大文件
来源：http://baike.sjlbkw.cn/Article/details/gjzitjokd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.epnwcf.com/Article/details/gzabsighz.sHtML

[U24] Py：路径操作
来源：http://read.share.sjlbkw.cn/Article/details/glwkfjied.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.yfazqb.com/Article/details/gwsoiujxf.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.vehdjk.com/Article/details/gjhqkkrkp.sHtML

csv.DictReader(f)
来源：http://blog.yfazqb.com/Article/details/gdipknbel.sHtML

[U26] Py：并发下载
来源：http://mobile.yfazqb.com/Article/details/gcywemfoy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.bbcook.cn/Article/details/gselulgjq.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fktsv.cn/Article/details/gvqezscjf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.epnwcf.com/Article/details/gkgzuyurb.sHtML

[U28] Py：类型别名
来源：http://www.blog.fktsv.cn/Article/details/gdbstadjy.sHtML

UserId = int
来源：http://www.blog.fktsv.cn/Article/details/gggrafvwn.sHtML

[U29] Py：属性校验
来源：http://baike.tarul.cn/Article/details/gfvuhaoem.sHtML

@property 与 @x.setter 配合
来源：http://www.share.tarul.cn/Article/details/gphchjdvn.sHtML

[U30] Py：数据类
来源：http://mobile.bbcook.cn/Article/details/gaeobeavd.sHtML

@dataclass(slots=True)
来源：http://www.blog.bbcook.cn/Article/details/gbfyaocwf.sHtML

[U31] Py：单测
来源：http://www.m.share.fktsv.cn/Article/details/gqeoudzfn.sHtML

python -m pytest -q
来源：http://m.share.fktsv.cn/Article/details/ggonswwiw.sHtML

[U32] Py：代码格式化
来源：http://3g.vehdjk.com/Article/details/geubjvksc.sHtML

ruff format . && ruff check --fix .
来源：http://blog.yfazqb.com/Article/details/gfpmbtnzy.sHtML

[U33] Py：打包发布
来源：http://mobile.fktsv.cn/Article/details/gefbaexrf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.yfazqb.com/Article/details/gmcgedosb.sHtML

[U34] Py：判断编码
来源：http://www.m.share.sjlbkw.cn/Article/details/gzeafthni.sHtML

chardet.detect(raw)
来源：http://www.share.epnwcf.com/Article/details/gtoqincig.sHtML

[U35] Py：发送邮件
来源：http://baike.epnwcf.com/Article/details/gkgersqdz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fktsv.cn/Article/details/gmktvulun.sHtML

[U36] Py：定时任务
来源：http://mobile.vehdjk.com/Article/details/gzpusacly.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.epnwcf.com/Article/details/gwauzywcz.sHtML

[U37] Py：读写 Excel
来源：http://3g.bbcook.cn/Article/details/ghdxnyjzq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.vehdjk.com/Article/details/gaxyyxdsj.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.yfazqb.com/Article/details/glzvuqcjs.sHtML

Path(__file__).resolve().parent
来源：http://mobile.sjlbkw.cn/Article/details/gbrmblsgs.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.yfazqb.com/Article/details/gdplojxtl.sHtML

sys.stdout.isatty()
来源：http://blog.sjlbkw.cn/Article/details/gtpcxkull.sHtML

[U40] Py：打印到标准错误
来源：http://3g.tarul.cn/Article/details/gmfyfahvb.sHtML

print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/glcnitcbr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.sjlbkw.cn/Article/details/gsjhjpgui.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.yfazqb.com/Article/details/gxfcbkpwh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.epnwcf.com/Article/details/giqclgjlo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.tarul.cn/Article/details/gquilsoqt.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fktsv.cn/Article/details/gzimgnivg.sHtML

namespace App\Http;
来源：http://m.share.tarul.cn/Article/details/gxflzxmnj.sHtML

[U44] PHP：开启严格类型
来源：http://blog.epnwcf.com/Article/details/gzzoqmfgq.sHtML

declare(strict_types=1);
来源：http://wap.tarul.cn/Article/details/gtikworps.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.yfazqb.com/Article/details/gsfialord.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gohhfzeek.sHtML

[U46] PHP：可空类型
来源：http://mobile.fktsv.cn/Article/details/gkknhoatn.sHtML

?string $name = null
来源：http://wap.bbcook.cn/Article/details/gvlrafmeo.sHtML

[U47] PHP：联合类型
来源：http://mobile.yfazqb.com/Article/details/ggvavrerf.sHtML

int|string $id
来源：http://wap.vehdjk.com/Article/details/gbzjahazr.sHtML

[U48] PHP：纯枚举
来源：http://blog.tarul.cn/Article/details/gdngywfel.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fktsv.cn/Article/details/gbmhsrjxr.sHtML

[U49] PHP：只读属性
来源：http://www.share.sjlbkw.cn/Article/details/gkzkxyhjv.sHtML

public readonly string $name
来源：http://mobile.yfazqb.com/Article/details/gxifbkwme.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.vehdjk.com/Article/details/gvyvnvmzq.sHtML

public function __construct(private int $id) {}
来源：http://blog.sjlbkw.cn/Article/details/gpiilnyyt.sHtML

[U51] PHP：数组解构
来源：http://blog.epnwcf.com/Article/details/ghhruiigo.sHtML

[$a, $b] = $arr;
来源：http://3g.fktsv.cn/Article/details/giodztscd.sHtML

[U52] PHP：箭头函数
来源：http://www.share.epnwcf.com/Article/details/ggjzkkody.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.epnwcf.com/Article/details/gozzkiuyo.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fktsv.cn/Article/details/gghmstssk.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.vehdjk.com/Article/details/grhaqmyqj.sHtML

[U54] PHP：空安全调用
来源：http://blog.tarul.cn/Article/details/gtrvmeeyc.sHtML

$obj?->method()
来源：http://read.share.yfazqb.com/Article/details/gwakhkudj.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fktsv.cn/Article/details/gtlxgrkfp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.sjlbkw.cn/Article/details/gcylanyiw.sHtML

[U56] PHP：命名参数
来源：http://wap.vehdjk.com/Article/details/grrxxoxgd.sHtML

f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gladeqgzg.sHtML

[U57] PHP：字符串插值
来源：http://read.share.tarul.cn/Article/details/gxhxpojzu.sHtML

"值: {$a}"
来源：http://mobile.tarul.cn/Article/details/gqypkaozt.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.sjlbkw.cn/Article/details/gxeurmqnz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.sjlbkw.cn/Article/details/gpgffflsg.sHtML

[U59] PHP：自定义排序
来源：http://baike.sjlbkw.cn/Article/details/goaxpmzsi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gqtctzrla.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.tarul.cn/Article/details/gnhtpjrpl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.vehdjk.com/Article/details/glezbizkn.sHtML

[U61] PHP：正则
来源：http://mobile.epnwcf.com/Article/details/gtfkkpoae.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.vehdjk.com/Article/details/gwjybklia.sHtML

[U62] PHP：日期对象
来源：http://baike.vehdjk.com/Article/details/gtvgzbgev.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fktsv.cn/Article/details/gwtugayhs.sHtML

[U63] PHP：文件读写
来源：http://www.share.fktsv.cn/Article/details/ghyefgbvc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fktsv.cn/Article/details/gadhpwbfh.sHtML

[U64] PHP：目录遍历
来源：http://www.share.vehdjk.com/Article/details/gcitlgrns.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.tarul.cn/Article/details/gofbeqoro.sHtML

[U65] PHP：会话
来源：http://wap.tarul.cn/Article/details/gvtpwmjue.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fktsv.cn/Article/details/ggbotniaz.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.yfazqb.com/Article/details/gdsjyaxfp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.vehdjk.com/Article/details/gvimlfjer.sHtML

[U67] PHP：处理文件上传
来源：http://wap.vehdjk.com/Article/details/gxambpyze.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.bbcook.cn/Article/details/gklvxmrri.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.sjlbkw.cn/Article/details/gvszrnbrr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.epnwcf.com/Article/details/gjrlfasep.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.vehdjk.com/Article/details/guogsqjzk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.sjlbkw.cn/Article/details/gsqqudlog.sHtML

[U70] PHP：PDO 事务
来源：http://blog.tarul.cn/Article/details/gybbdhsks.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.yfazqb.com/Article/details/gjhhbyixy.sHtML

[U71] PHP：抛出异常
来源：http://wap.sjlbkw.cn/Article/details/gqzonjznt.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fktsv.cn/Article/details/gsxwtuzgy.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fktsv.cn/Article/details/gfjcyboou.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.epnwcf.com/Article/details/gorzdzlzs.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.yfazqb.com/Article/details/gclfmdpcm.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.bbcook.cn/Article/details/gbkqliwxf.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fktsv.cn/Article/details/gpzxmraow.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.sjlbkw.cn/Article/details/gxocoeukf.sHtML

[U75] PHP：依赖注入
来源：http://mobile.tarul.cn/Article/details/gsgcxrmfz.sHtML

composer require psr/container
来源：http://3g.epnwcf.com/Article/details/gazdhkmjd.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/gfhtuxauh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.yfazqb.com/Article/details/gmgmlylak.sHtML

[U77] PHP：模板渲染
来源：http://www.share.yfazqb.com/Article/details/gictyffbr.sHtML

composer require twig/twig
来源：http://wap.sjlbkw.cn/Article/details/gigvkbxoq.sHtML

[U78] PHP：单元测试
来源：http://www.blog.yfazqb.com/Article/details/gyhthtqsu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.tarul.cn/Article/details/gcemdvfot.sHtML

[U79] PHP：静态分析
来源：http://blog.yfazqb.com/Article/details/gvdqzjfag.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.yfazqb.com/Article/details/gmlwoauuc.sHtML

[U80] PHP：代码规范修复
来源：http://baike.vehdjk.com/Article/details/gsitxjecc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.sjlbkw.cn/Article/details/glsqcjzck.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.vehdjk.com/Article/details/gqijffjek.sHtML

npm init -y;  npm i express
来源：http://wap.fktsv.cn/Article/details/ggxvgvxkt.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.bbcook.cn/Article/details/gsavcfpgt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.sjlbkw.cn/Article/details/gzrkbxmww.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.vehdjk.com/Article/details/gujwsoxta.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/gdivecryy.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.sjlbkw.cn/Article/details/gfpkpeghg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.epnwcf.com/Article/details/gbmvomkzp.sHtML

[U85] JS：可选链
来源：http://read.share.sjlbkw.cn/Article/details/gmzmvdffy.sHtML

a?.b?.c
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwhfkrzq.sHtML

[U86] JS：空值合并
来源：http://mobile.fktsv.cn/Article/details/gtkcvsipt.sHtML

a ?? b
来源：http://www.m.share.bbcook.cn/Article/details/gfoyhvide.sHtML

[U87] JS：解构默认值
来源：http://www.share.sjlbkw.cn/Article/details/gftlmrwgs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.yfazqb.com/Article/details/ggvhjccos.sHtML

[U88] JS：对象展开合并
来源：http://blog.bbcook.cn/Article/details/glwqngewg.sHtML

{ ...a, ...b }
来源：http://baike.vehdjk.com/Article/details/gsrvfxojm.sHtML

[U89] JS：数组去重
来源：http://www.m.share.bbcook.cn/Article/details/gvmlqorxe.sHtML

[...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/ghairyoia.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.bbcook.cn/Article/details/gxnblvhvf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gxbwxhdtw.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fktsv.cn/Article/details/gelzxmcoz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.vehdjk.com/Article/details/grvtmmthr.sHtML

[U92] JS：深拷贝
来源：http://mobile.vehdjk.com/Article/details/gkyzersld.sHtML

structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gwhpvxorj.sHtML


<!-- 参考信息 -->