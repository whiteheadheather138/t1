代发 wailian999

[T05] Kotlin：when 表达式
来源：http://blog.sjlbkw.cn/Article/details/gnlmhqdux.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/gnigwokza.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.epnwcf.com/Article/details/gbpodvfej.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.epnwcf.com/Article/details/gwlpdokev.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fktsv.cn/Article/details/ggorbpfeh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.bbcook.cn/Article/details/ggrifoyxl.sHtML

[T08] Kotlin：数据类
来源：http://baike.sjlbkw.cn/Article/details/gyytbyjwm.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.vehdjk.com/Article/details/gautuhywq.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.sjlbkw.cn/Article/details/gailfgtse.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/gkihksmcv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.epnwcf.com/Article/details/gezteumye.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.yfazqb.com/Article/details/gwxclmwfw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.sjlbkw.cn/Article/details/glzjnehjb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.sjlbkw.cn/Article/details/gcbvpffuy.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fktsv.cn/Article/details/gqonimlxr.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fktsv.cn/Article/details/gjckcwjvm.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/glnrcbfns.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fktsv.cn/Article/details/gsldxysyd.sHtML

[T14] Kotlin：循环
来源：http://wap.epnwcf.com/Article/details/ghvwzhbsm.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gqvbrmfbv.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/gbitnmbqf.sHtML

interface Shape { fun area(): Double }
来源：http://blog.tarul.cn/Article/details/gotrucrvo.sHtML

[T16] Swift：Hello World
来源：http://3g.tarul.cn/Article/details/gmvskizga.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gpyrrosyi.sHtML

[T17] Swift：变量与常量
来源：http://www.share.sjlbkw.cn/Article/details/gimhljsrj.sHtML

var a = 1;  let b = 2
来源：http://baike.fktsv.cn/Article/details/gjazjzdng.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gmzbwwjbc.sHtML

"值: \(b)"
来源：http://www.share.tarul.cn/Article/details/gzcjehnda.sHtML

[T19] Swift：可选绑定
来源：http://www.share.epnwcf.com/Article/details/gfvzzgnua.sHtML

if let n = opt { print(n) }
来源：http://blog.sjlbkw.cn/Article/details/gkijjtdnw.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.epnwcf.com/Article/details/givdpvxbm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.sjlbkw.cn/Article/details/gorcfbusg.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gmfddbxxf.sHtML

for x in a { print(x) }
来源：http://www.blog.bbcook.cn/Article/details/gosnxrajh.sHtML

[T22] Swift：字典
来源：http://3g.bbcook.cn/Article/details/gswzhuibd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.epnwcf.com/Article/details/gsmacaxbo.sHtML

[T23] Swift：函数
来源：http://blog.yfazqb.com/Article/details/grymzfccd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.sjlbkw.cn/Article/details/gpdukicqf.sHtML

[T24] Swift：闭包
来源：http://m.share.epnwcf.com/Article/details/glfyaoezy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gkmkhwvfq.sHtML

[T25] Swift：结构体
来源：http://read.share.tarul.cn/Article/details/gdtedgmia.sHtML

struct P { var x: Int }
来源：http://m.share.fktsv.cn/Article/details/gkdlbvelf.sHtML

[T26] Swift：类与重写
来源：http://3g.epnwcf.com/Article/details/gewmxjluh.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjsuqjok.sHtML

[T27] Swift：错误处理
来源：http://wap.vehdjk.com/Article/details/ghctctgug.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fktsv.cn/Article/details/ghydzzrum.sHtML

[T28] Swift：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/guxxblaff.sHtML

enum Color { case red, green }
来源：http://blog.vehdjk.com/Article/details/ghrawnitv.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.epnwcf.com/Article/details/gbloaycba.sHtML

guard let x = opt else { return }
来源：http://www.blog.sjlbkw.cn/Article/details/glfzwqulb.sHtML

[T30] Swift：协议
来源：http://baike.sjlbkw.cn/Article/details/gbnrozzqj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.vehdjk.com/Article/details/ghzdiqrmd.sHtML

[T31] Lua：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gqmiacqwe.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/gdmqttfzd.sHtML

[T32] Lua：局部变量
来源：http://wap.epnwcf.com/Article/details/gmtktabye.sHtML

local a = 1
来源：http://baike.sjlbkw.cn/Article/details/gyiikweoy.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.vehdjk.com/Article/details/gikzkowec.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.tarul.cn/Article/details/gvmhylixs.sHtML

[T34] Lua：遍历表
来源：http://3g.sjlbkw.cn/Article/details/gdgzgnilf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.vehdjk.com/Article/details/gwcsqovfh.sHtML

[T35] Lua：字典表
来源：http://baike.yfazqb.com/Article/details/gsphikjes.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.vehdjk.com/Article/details/gyukwtihe.sHtML

[T36] Lua：函数
来源：http://3g.fktsv.cn/Article/details/gxhesuwme.sHtML

function add(a, b) return a + b end
来源：http://m.share.tarul.cn/Article/details/gsevhcbxz.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/gnyxdgmdi.sHtML

"a" .. "b"
来源：http://www.blog.yfazqb.com/Article/details/gomljzlmc.sHtML

[T38] Lua：条件
来源：http://mobile.vehdjk.com/Article/details/gzjqktkga.sHtML

if x > 0 then print("正") end
来源：http://blog.fktsv.cn/Article/details/goxqiktie.sHtML

[T39] Lua：模式匹配
来源：http://read.share.tarul.cn/Article/details/gpnfrzmlm.sHtML

string.find(s, "%d+")
来源：http://m.share.sjlbkw.cn/Article/details/gvfkgasfs.sHtML

[T40] Lua：元表
来源：http://read.share.epnwcf.com/Article/details/grquyztdc.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.yfazqb.com/Article/details/glojtvonh.sHtML

[T41] Perl：Hello World
来源：http://baike.bbcook.cn/Article/details/ghnoaixaq.sHtML

print "Hello\n";
来源：http://www.blog.fktsv.cn/Article/details/gxlrcrgrg.sHtML

[T42] Perl：变量类型
来源：http://www.blog.tarul.cn/Article/details/grbhxecci.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.tarul.cn/Article/details/gxotmzwvf.sHtML

[T43] Perl：字符串插值
来源：http://blog.yfazqb.com/Article/details/gsgzdmjih.sHtML

"值: $a"
来源：http://3g.fktsv.cn/Article/details/gxzqfiowa.sHtML

[T44] Perl：条件
来源：http://www.blog.fktsv.cn/Article/details/gqugqmyzr.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.bbcook.cn/Article/details/gzwzsxixq.sHtML

[T45] Perl：数组遍历
来源：http://blog.tarul.cn/Article/details/giixwfgzj.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.sjlbkw.cn/Article/details/gmgoquete.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.vehdjk.com/Article/details/glgqozbfx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.yfazqb.com/Article/details/gswwyzrao.sHtML

[T47] Perl：正则捕获
来源：http://www.share.yfazqb.com/Article/details/glikeuqxi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.yfazqb.com/Article/details/goruofbdc.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/gcevedylv.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fktsv.cn/Article/details/gphvzpfvj.sHtML

[T49] Perl：函数
来源：http://www.m.share.fktsv.cn/Article/details/ghtvmadhj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gygtdviue.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/ghlcxvjaj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.epnwcf.com/Article/details/gybhaxqtm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmgunioo.sHtML

[T51] Scala：Hello World
来源：http://www.share.bbcook.cn/Article/details/gktoebjsz.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gmvmvhzvq.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gvgcdbbkh.sHtML

val a = 1;  var b = 2
来源：http://3g.tarul.cn/Article/details/gckwixdwy.sHtML

[T53] Scala：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gvbaavnvl.sHtML

s"值: $b"
来源：http://3g.yfazqb.com/Article/details/gwoybnsfa.sHtML

[T54] Scala：集合映射
来源：http://m.share.tarul.cn/Article/details/gqhnfhojg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.vehdjk.com/Article/details/ggysutaxi.sHtML

[T55] Scala：集合过滤
来源：http://mobile.epnwcf.com/Article/details/ghpokxxpw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.yfazqb.com/Article/details/gjwjlaijy.sHtML

[T56] Scala：样例类
来源：http://m.share.epnwcf.com/Article/details/gslbyhnut.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/gjigzhuuc.sHtML

[T57] Scala：模式匹配
来源：http://m.share.bbcook.cn/Article/details/gjpjwduhg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gonuqzhet.sHtML

[T58] Scala：函数定义
来源：http://read.share.fktsv.cn/Article/details/gfyvuzpnw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.vehdjk.com/Article/details/geevhhfme.sHtML

[T59] Scala：循环
来源：http://www.m.share.fktsv.cn/Article/details/gvffhblla.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.epnwcf.com/Article/details/gluqonyns.sHtML

[T60] Scala：折叠
来源：http://mobile.tarul.cn/Article/details/gcvbtrrgo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.sjlbkw.cn/Article/details/gshlbyiiu.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gcekkyyrc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.tarul.cn/Article/details/glqkseitz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gsflngkvl.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fktsv.cn/Article/details/gnkqgkmha.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.sjlbkw.cn/Article/details/ghjcywcgr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.tarul.cn/Article/details/gokvgaewt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.tarul.cn/Article/details/guyohxtkj.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fktsv.cn/Article/details/gmtfclmqe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.epnwcf.com/Article/details/gyqoqbeqk.sHtML

[U04] Py：变量调试打印
来源：http://mobile.yfazqb.com/Article/details/gznrzgpjf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.yfazqb.com/Article/details/guvbuzqmd.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.vehdjk.com/Article/details/gbvkkprjg.sHtML

list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/gpkupuail.sHtML

[U06] Py：合并两个字典
来源：http://3g.bbcook.cn/Article/details/gzrhnimng.sHtML

{**a, **b}
来源：http://read.share.fktsv.cn/Article/details/gmrfkliod.sHtML

[U07] Py：反转字典键值
来源：http://mobile.tarul.cn/Article/details/gskitydkl.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.vehdjk.com/Article/details/gcmrteabm.sHtML

[U08] Py：展平二维列表
来源：http://blog.sjlbkw.cn/Article/details/gfkropqqe.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.bbcook.cn/Article/details/gnhbhypmn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fktsv.cn/Article/details/gwzxflxtf.sHtML

max(d, key=d.get)
来源：http://www.m.share.bbcook.cn/Article/details/gxkunhuhy.sHtML

[U10] Py：按值排序字典
来源：http://3g.yfazqb.com/Article/details/glvdeopsi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.tarul.cn/Article/details/gojpagdcy.sHtML

[U11] Py：生成器表达式
来源：http://baike.sjlbkw.cn/Article/details/gjmhxzbqr.sHtML

(x * 2 for x in arr)
来源：http://www.share.tarul.cn/Article/details/gftgzhkto.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.epnwcf.com/Article/details/ggivnfrfp.sHtML

Counter(arr).most_common(3)
来源：http://m.share.epnwcf.com/Article/details/ghnnwgmft.sHtML

[U13] Py：固定长度队列
来源：http://m.share.tarul.cn/Article/details/gagspxnlg.sHtML

deque(maxlen=10)
来源：http://www.m.share.tarul.cn/Article/details/gltukgklt.sHtML

[U14] Py：分组收集到列表
来源：http://3g.bbcook.cn/Article/details/giwwuhshu.sHtML

defaultdict(list)
来源：http://www.share.sjlbkw.cn/Article/details/guxltrrdk.sHtML

[U15] Py：高精度计时
来源：http://blog.fktsv.cn/Article/details/gssqszueg.sHtML

t = time.perf_counter()
来源：http://www.share.sjlbkw.cn/Article/details/gmaednlxn.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.tarul.cn/Article/details/goixlmvpk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.tarul.cn/Article/details/gvfptcduj.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.yfazqb.com/Article/details/gqsnarisf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.tarul.cn/Article/details/gibabbyzf.sHtML

[U18] Py：预编译正则
来源：http://www.share.epnwcf.com/Article/details/gzlndoucu.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gnlgeaxak.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.yfazqb.com/Article/details/gxfaahzkb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fktsv.cn/Article/details/gkuvylyfk.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fktsv.cn/Article/details/gjutmqtrm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.sjlbkw.cn/Article/details/ghrcetpwm.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.bbcook.cn/Article/details/gggkgyvts.sHtML

@contextlib.contextmanager
来源：http://blog.epnwcf.com/Article/details/gajhpzxfg.sHtML

[U22] Py：矩阵转置
来源：http://3g.fktsv.cn/Article/details/ggdzzajoj.sHtML

list(zip(*m))
来源：http://3g.vehdjk.com/Article/details/gqdhaiyfg.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.sjlbkw.cn/Article/details/ghtbxbslk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.sjlbkw.cn/Article/details/gayjqiyoa.sHtML

[U24] Py：路径操作
来源：http://www.share.sjlbkw.cn/Article/details/gpeaylgsi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.sjlbkw.cn/Article/details/gxxudajvb.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fktsv.cn/Article/details/gatpbvfur.sHtML

csv.DictReader(f)
来源：http://3g.epnwcf.com/Article/details/gemwgamtm.sHtML

[U26] Py：并发下载
来源：http://baike.tarul.cn/Article/details/ggeplpouw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fktsv.cn/Article/details/gbideaskf.sHtML

[U27] Py：异步 HTTP
来源：http://blog.tarul.cn/Article/details/gjdlinkad.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.yfazqb.com/Article/details/gciqaqfnj.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fktsv.cn/Article/details/gtpyjjhsx.sHtML

UserId = int
来源：http://3g.vehdjk.com/Article/details/gaqgghztj.sHtML

[U29] Py：属性校验
来源：http://blog.vehdjk.com/Article/details/ghgegmdpd.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.bbcook.cn/Article/details/gpfqighru.sHtML

[U30] Py：数据类
来源：http://www.share.epnwcf.com/Article/details/gioozezit.sHtML

@dataclass(slots=True)
来源：http://blog.fktsv.cn/Article/details/gyjvftkck.sHtML

[U31] Py：单测
来源：http://www.share.sjlbkw.cn/Article/details/gflkldvqc.sHtML

python -m pytest -q
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpxlqhdy.sHtML

[U32] Py：代码格式化
来源：http://read.share.vehdjk.com/Article/details/gvfzfgnsy.sHtML

ruff format . && ruff check --fix .
来源：http://3g.tarul.cn/Article/details/gtduahfpb.sHtML

[U33] Py：打包发布
来源：http://mobile.vehdjk.com/Article/details/gaeusqorm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fktsv.cn/Article/details/glychkqrv.sHtML

[U34] Py：判断编码
来源：http://blog.tarul.cn/Article/details/gbwkvnrnr.sHtML

chardet.detect(raw)
来源：http://m.share.vehdjk.com/Article/details/ghmttcwwm.sHtML

[U35] Py：发送邮件
来源：http://mobile.tarul.cn/Article/details/ghzfmmhcv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.bbcook.cn/Article/details/gqjcmunyr.sHtML

[U36] Py：定时任务
来源：http://www.blog.yfazqb.com/Article/details/gnlrotwgd.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.sjlbkw.cn/Article/details/gtaltcgjs.sHtML

[U37] Py：读写 Excel
来源：http://mobile.yfazqb.com/Article/details/gynxdhdaq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.epnwcf.com/Article/details/gjgbhqash.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fktsv.cn/Article/details/gtvgepfku.sHtML

Path(__file__).resolve().parent
来源：http://mobile.bbcook.cn/Article/details/grjvblasg.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.vehdjk.com/Article/details/grtxcynjz.sHtML

sys.stdout.isatty()
来源：http://read.share.tarul.cn/Article/details/gamjwyduo.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.epnwcf.com/Article/details/gatcalism.sHtML

print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/gsshqtuhk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.bbcook.cn/Article/details/gepghfyia.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.epnwcf.com/Article/details/gznampatw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.bbcook.cn/Article/details/gxzrehhkc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fktsv.cn/Article/details/guhrdpxbp.sHtML

[U43] PHP：声明命名空间
来源：http://blog.sjlbkw.cn/Article/details/grxrhuxnb.sHtML

namespace App\Http;
来源：http://www.m.share.vehdjk.com/Article/details/gquwbyyru.sHtML

[U44] PHP：开启严格类型
来源：http://blog.sjlbkw.cn/Article/details/gpkpzfqlp.sHtML

declare(strict_types=1);
来源：http://baike.yfazqb.com/Article/details/gcwuyslvg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.epnwcf.com/Article/details/gighkdowk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gcyzarjbt.sHtML

[U46] PHP：可空类型
来源：http://blog.tarul.cn/Article/details/gaifumxvn.sHtML

?string $name = null
来源：http://www.blog.sjlbkw.cn/Article/details/gxuvyhumq.sHtML

[U47] PHP：联合类型
来源：http://3g.tarul.cn/Article/details/gvqhfotfw.sHtML

int|string $id
来源：http://wap.bbcook.cn/Article/details/gvqzlgvoa.sHtML

[U48] PHP：纯枚举
来源：http://read.share.tarul.cn/Article/details/grlhkuoeo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.epnwcf.com/Article/details/gqhhcjqiy.sHtML

[U49] PHP：只读属性
来源：http://read.share.vehdjk.com/Article/details/gwwmysrut.sHtML

public readonly string $name
来源：http://blog.sjlbkw.cn/Article/details/gslnkpxpn.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.bbcook.cn/Article/details/gotymbnrj.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fktsv.cn/Article/details/gihcggdce.sHtML

[U51] PHP：数组解构
来源：http://3g.vehdjk.com/Article/details/gjkdtexks.sHtML

[$a, $b] = $arr;
来源：http://baike.sjlbkw.cn/Article/details/giupoxwcj.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.epnwcf.com/Article/details/gmsqalmmh.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.epnwcf.com/Article/details/guagipzuj.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fktsv.cn/Article/details/gygomlfgf.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fktsv.cn/Article/details/gwogifdvp.sHtML

[U54] PHP：空安全调用
来源：http://wap.yfazqb.com/Article/details/gcrysflud.sHtML

$obj?->method()
来源：http://wap.tarul.cn/Article/details/gkofbpzhv.sHtML

[U55] PHP：match 表达式
来源：http://baike.sjlbkw.cn/Article/details/gsdzjgzav.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/gijlexwkw.sHtML

[U56] PHP：命名参数
来源：http://www.share.tarul.cn/Article/details/gycocvfvn.sHtML

f(a: 1, b: 2)
来源：http://baike.vehdjk.com/Article/details/giqpujonx.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gmientvmm.sHtML

"值: {$a}"
来源：http://blog.fktsv.cn/Article/details/gwtfxfavm.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fktsv.cn/Article/details/gpxryvqlq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.tarul.cn/Article/details/gnypbcvwr.sHtML

[U59] PHP：自定义排序
来源：http://baike.tarul.cn/Article/details/gyensrwjs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gcxuyqser.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.yfazqb.com/Article/details/gmzbklsss.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.vehdjk.com/Article/details/gtnqalhtz.sHtML

[U61] PHP：正则
来源：http://www.share.fktsv.cn/Article/details/glzgydxrk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gonzgzvhu.sHtML

[U62] PHP：日期对象
来源：http://wap.bbcook.cn/Article/details/gycrvpyos.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fktsv.cn/Article/details/gwayclkzz.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.bbcook.cn/Article/details/gzqkhettj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fktsv.cn/Article/details/gogfioeoq.sHtML

[U64] PHP：目录遍历
来源：http://blog.tarul.cn/Article/details/gvfxnnkvu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.tarul.cn/Article/details/geqoulzyx.sHtML

[U65] PHP：会话
来源：http://3g.bbcook.cn/Article/details/gnbmttiva.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gcoetssge.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fktsv.cn/Article/details/geosqpayo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.yfazqb.com/Article/details/gafjciyru.sHtML

[U67] PHP：处理文件上传
来源：http://3g.yfazqb.com/Article/details/ganoadfah.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.epnwcf.com/Article/details/glpittrdl.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fktsv.cn/Article/details/gujbxvdmj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.tarul.cn/Article/details/givqricim.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.tarul.cn/Article/details/gxogcysrb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.sjlbkw.cn/Article/details/genbokkhh.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.tarul.cn/Article/details/glapnvrsi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fktsv.cn/Article/details/geetuxbym.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gujrhbyll.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.epnwcf.com/Article/details/gxbwplgsb.sHtML

[U72] PHP：写错误日志
来源：http://read.share.epnwcf.com/Article/details/gvvfpnugc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.vehdjk.com/Article/details/gxfthmadu.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fktsv.cn/Article/details/gkuybqpsw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.yfazqb.com/Article/details/gmpcvljdn.sHtML

[U74] PHP：读取环境变量
来源：http://3g.vehdjk.com/Article/details/geweuydeb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.vehdjk.com/Article/details/gxaaqzqsq.sHtML

[U75] PHP：依赖注入
来源：http://www.share.sjlbkw.cn/Article/details/gjndahvwd.sHtML

composer require psr/container
来源：http://wap.tarul.cn/Article/details/gwixwgxfv.sHtML

[U76] PHP：简单路由
来源：http://wap.epnwcf.com/Article/details/gtjyifcui.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.sjlbkw.cn/Article/details/grigvryav.sHtML

[U77] PHP：模板渲染
来源：http://blog.yfazqb.com/Article/details/gpdjqihdj.sHtML

composer require twig/twig
来源：http://wap.sjlbkw.cn/Article/details/gjcvalwyt.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.vehdjk.com/Article/details/gzfsaclzg.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.bbcook.cn/Article/details/gxsxpyyfk.sHtML

[U79] PHP：静态分析
来源：http://baike.vehdjk.com/Article/details/gluuxjiyk.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.vehdjk.com/Article/details/gzhzmyvxo.sHtML

[U80] PHP：代码规范修复
来源：http://wap.yfazqb.com/Article/details/guezelbqi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.sjlbkw.cn/Article/details/gcffsbbhm.sHtML

[U81] JS：初始化项目
来源：http://blog.tarul.cn/Article/details/gzmldbema.sHtML

npm init -y;  npm i express
来源：http://m.share.fktsv.cn/Article/details/grydqdguy.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.tarul.cn/Article/details/gbyeamlok.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.tarul.cn/Article/details/grtpreozl.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.sjlbkw.cn/Article/details/gcizlixlz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/gflysjfrr.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.tarul.cn/Article/details/gtdrezuet.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.vehdjk.com/Article/details/gcfluewly.sHtML

[U85] JS：可选链
来源：http://wap.yfazqb.com/Article/details/gcxojzbeb.sHtML

a?.b?.c
来源：http://mobile.fktsv.cn/Article/details/ghujxwjcy.sHtML

[U86] JS：空值合并
来源：http://3g.bbcook.cn/Article/details/gqykmhfoq.sHtML

a ?? b
来源：http://read.share.sjlbkw.cn/Article/details/gehuiyxjx.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.epnwcf.com/Article/details/gqnkqbvcs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.epnwcf.com/Article/details/gnvhdivgo.sHtML

[U88] JS：对象展开合并
来源：http://www.share.yfazqb.com/Article/details/gwqmzvaza.sHtML

{ ...a, ...b }
来源：http://mobile.bbcook.cn/Article/details/gqnlwwqfw.sHtML

[U89] JS：数组去重
来源：http://3g.yfazqb.com/Article/details/gghgqtbea.sHtML

[...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gbvtuxqcq.sHtML

[U90] JS：数字数组排序
来源：http://read.share.yfazqb.com/Article/details/gqlenepfo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gqvdcpmhp.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.sjlbkw.cn/Article/details/gpeucpabn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.bbcook.cn/Article/details/glswrqcdz.sHtML

[U92] JS：深拷贝
来源：http://baike.yfazqb.com/Article/details/gvtzhvkjm.sHtML

structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/glcwwaozd.sHtML


<!-- 参考信息 -->