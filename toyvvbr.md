代发 wailian999

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gofynlydo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.tarul.cn/Article/details/gfeyrsfhv.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/gbaxaxhuo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/gptiigdqh.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.bbcook.cn/Article/details/gcnubbupb.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.vehdjk.com/Article/details/ggabhmzil.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.tarul.cn/Article/details/gobgmuuxx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.yfazqb.com/Article/details/gshqsgivs.sHtML

[T11] Kotlin：协程
来源：http://read.share.bbcook.cn/Article/details/gvjbaitug.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.tarul.cn/Article/details/gymmprpcw.sHtML

[T12] Kotlin：解构声明
来源：http://3g.epnwcf.com/Article/details/gfambvecd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.vehdjk.com/Article/details/guyftxnsz.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/goypqmyux.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fktsv.cn/Article/details/gzrratcbx.sHtML

[T14] Kotlin：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gyjaolnhu.sHtML

for (i in 1..10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gjfxapywo.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.vehdjk.com/Article/details/gdpnioulk.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.bbcook.cn/Article/details/gqodpwece.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gqtjawvam.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gtqgfycxo.sHtML

[T17] Swift：变量与常量
来源：http://wap.epnwcf.com/Article/details/ghlbabpyd.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/gxayenfld.sHtML

[T18] Swift：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gkpjnimra.sHtML

"值: \(b)"
来源：http://3g.fktsv.cn/Article/details/gmcmeaquw.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/greiaegju.sHtML

if let n = opt { print(n) }
来源：http://wap.vehdjk.com/Article/details/gciqdrjyl.sHtML

[T20] Swift：数组操作
来源：http://3g.fktsv.cn/Article/details/giefndsib.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.vehdjk.com/Article/details/gfrsjeahg.sHtML

[T21] Swift：遍历
来源：http://www.blog.yfazqb.com/Article/details/gtbqhlzzu.sHtML

for x in a { print(x) }
来源：http://www.m.share.tarul.cn/Article/details/gekfqrlxc.sHtML

[T22] Swift：字典
来源：http://www.blog.bbcook.cn/Article/details/gnexwrpal.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.tarul.cn/Article/details/gccgffnul.sHtML

[T23] Swift：函数
来源：http://www.m.share.yfazqb.com/Article/details/guelwsvvh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.bbcook.cn/Article/details/gnlizhamc.sHtML

[T24] Swift：闭包
来源：http://wap.bbcook.cn/Article/details/gxfepmwjs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/gjuzfdwnu.sHtML

[T25] Swift：结构体
来源：http://read.share.yfazqb.com/Article/details/gjilkcxjb.sHtML

struct P { var x: Int }
来源：http://mobile.vehdjk.com/Article/details/gvikggngg.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/grqzwfspt.sHtML

class A: Base { override func f() {} }
来源：http://www.share.yfazqb.com/Article/details/gqvdectig.sHtML

[T27] Swift：错误处理
来源：http://mobile.fktsv.cn/Article/details/gjpdhprbr.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/gdnovpxhl.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gurzeqfca.sHtML

enum Color { case red, green }
来源：http://m.share.sjlbkw.cn/Article/details/gogndevqu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.epnwcf.com/Article/details/grurkwrqt.sHtML

guard let x = opt else { return }
来源：http://mobile.tarul.cn/Article/details/gmgcjcucw.sHtML

[T30] Swift：协议
来源：http://wap.yfazqb.com/Article/details/glnphfeoh.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.tarul.cn/Article/details/gffhdsaog.sHtML

[T31] Lua：Hello World
来源：http://blog.vehdjk.com/Article/details/gwrirnkhz.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gujnpxgqt.sHtML

[T32] Lua：局部变量
来源：http://m.share.fktsv.cn/Article/details/giqligfgu.sHtML

local a = 1
来源：http://wap.vehdjk.com/Article/details/gvcnjvgby.sHtML

[T33] Lua：表（数组）
来源：http://baike.tarul.cn/Article/details/ginhzzyjm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.yfazqb.com/Article/details/glqhykkoe.sHtML

[T34] Lua：遍历表
来源：http://read.share.vehdjk.com/Article/details/gcubjkweg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.sjlbkw.cn/Article/details/gtshrqqsv.sHtML

[T35] Lua：字典表
来源：http://baike.sjlbkw.cn/Article/details/gaphromud.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fktsv.cn/Article/details/guulsrtfm.sHtML

[T36] Lua：函数
来源：http://www.m.share.epnwcf.com/Article/details/gtskvcexf.sHtML

function add(a, b) return a + b end
来源：http://baike.epnwcf.com/Article/details/gespfgamq.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.tarul.cn/Article/details/gankvclxm.sHtML

"a" .. "b"
来源：http://m.share.epnwcf.com/Article/details/gwgodlcyr.sHtML

[T38] Lua：条件
来源：http://blog.yfazqb.com/Article/details/ggubyypiu.sHtML

if x > 0 then print("正") end
来源：http://read.share.sjlbkw.cn/Article/details/glznkqfje.sHtML

[T39] Lua：模式匹配
来源：http://blog.bbcook.cn/Article/details/geilihkbb.sHtML

string.find(s, "%d+")
来源：http://mobile.sjlbkw.cn/Article/details/gzqvpvahn.sHtML

[T40] Lua：元表
来源：http://blog.vehdjk.com/Article/details/gpihakvkr.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.sjlbkw.cn/Article/details/gofakgprx.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gubdglcgo.sHtML

print "Hello\n";
来源：http://m.share.yfazqb.com/Article/details/gvcgsergu.sHtML

[T42] Perl：变量类型
来源：http://mobile.tarul.cn/Article/details/gycnfttei.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.tarul.cn/Article/details/gauoqdmbz.sHtML

[T43] Perl：字符串插值
来源：http://blog.vehdjk.com/Article/details/givfboqsu.sHtML

"值: $a"
来源：http://wap.bbcook.cn/Article/details/gwslyeklh.sHtML

[T44] Perl：条件
来源：http://m.share.sjlbkw.cn/Article/details/gylpbrxmn.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.vehdjk.com/Article/details/gjbadwzhw.sHtML

[T45] Perl：数组遍历
来源：http://read.share.yfazqb.com/Article/details/gjznpsqez.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.yfazqb.com/Article/details/ggofluqvc.sHtML

[T46] Perl：哈希操作
来源：http://read.share.bbcook.cn/Article/details/gxkzaexyw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.tarul.cn/Article/details/gxzkwoycy.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fktsv.cn/Article/details/gpuneuzvr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.yfazqb.com/Article/details/glllwwgkx.sHtML

[T48] Perl：正则替换
来源：http://www.blog.epnwcf.com/Article/details/gtofhoimf.sHtML

$s =~ s/old/new/g;
来源：http://baike.sjlbkw.cn/Article/details/gaiusruht.sHtML

[T49] Perl：函数
来源：http://baike.bbcook.cn/Article/details/gluscosmz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/ghbfbfviu.sHtML

[T50] Perl：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gqlvsghxx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.epnwcf.com/Article/details/gfjtnkssn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.tarul.cn/Article/details/gdevywwgi.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gmrzclrdp.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gnohgpbqv.sHtML

[T52] Scala：变量
来源：http://m.share.epnwcf.com/Article/details/gpgsbpisc.sHtML

val a = 1;  var b = 2
来源：http://3g.bbcook.cn/Article/details/gjxhlwkuk.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gxkoycqal.sHtML

s"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gyfnkzrkc.sHtML

[T54] Scala：集合映射
来源：http://www.share.fktsv.cn/Article/details/gpagnlyto.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.bbcook.cn/Article/details/gexnqhdbu.sHtML

[T55] Scala：集合过滤
来源：http://wap.tarul.cn/Article/details/getlcikng.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.yfazqb.com/Article/details/ghapfzmne.sHtML

[T56] Scala：样例类
来源：http://mobile.fktsv.cn/Article/details/gictihuij.sHtML

case class User(name: String, age: Int)
来源：http://m.share.vehdjk.com/Article/details/gtltkchsv.sHtML

[T57] Scala：模式匹配
来源：http://m.share.tarul.cn/Article/details/gptszfkxo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.sjlbkw.cn/Article/details/gsbwczigo.sHtML

[T58] Scala：函数定义
来源：http://mobile.epnwcf.com/Article/details/gmjtjbkav.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.bbcook.cn/Article/details/gnnkpcjys.sHtML

[T59] Scala：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvuwqsvh.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.epnwcf.com/Article/details/gquzhrjwv.sHtML

[T60] Scala：折叠
来源：http://baike.yfazqb.com/Article/details/gbzavwaij.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.epnwcf.com/Article/details/graddxusg.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghvxntqvv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.yfazqb.com/Article/details/gbrnqyzbu.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvjckiyez.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.yfazqb.com/Article/details/gqpzrzajf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.bbcook.cn/Article/details/ggebdsqzi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.sjlbkw.cn/Article/details/gtofnjuow.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gvnsmgtme.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.epnwcf.com/Article/details/glbvmtkmz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.epnwcf.com/Article/details/ghepzmmsv.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.bbcook.cn/Article/details/gngmukbln.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.epnwcf.com/Article/details/gwhvdgzhi.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.epnwcf.com/Article/details/gwgztujnh.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/gavdctehr.sHtML

[U06] Py：合并两个字典
来源：http://m.share.tarul.cn/Article/details/gzqoeqcyr.sHtML

{**a, **b}
来源：http://3g.bbcook.cn/Article/details/gzqrkjbbq.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.bbcook.cn/Article/details/glgunzahs.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.epnwcf.com/Article/details/guxgvoegq.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.epnwcf.com/Article/details/goopwotvt.sHtML

[y for x in nested for y in x]
来源：http://3g.bbcook.cn/Article/details/gpsvaakli.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fktsv.cn/Article/details/guskbekab.sHtML

max(d, key=d.get)
来源：http://www.m.share.yfazqb.com/Article/details/gpylaoihd.sHtML

[U10] Py：按值排序字典
来源：http://m.share.sjlbkw.cn/Article/details/gzdsrbkki.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gmatzvzsd.sHtML

[U11] Py：生成器表达式
来源：http://baike.vehdjk.com/Article/details/goiftfznt.sHtML

(x * 2 for x in arr)
来源：http://www.blog.yfazqb.com/Article/details/gvhjtjxsb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.bbcook.cn/Article/details/gymvilsfj.sHtML

Counter(arr).most_common(3)
来源：http://mobile.yfazqb.com/Article/details/gajgdzspp.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fktsv.cn/Article/details/gowtugclm.sHtML

deque(maxlen=10)
来源：http://m.share.tarul.cn/Article/details/gyqetrhww.sHtML

[U14] Py：分组收集到列表
来源：http://wap.bbcook.cn/Article/details/gryfcihds.sHtML

defaultdict(list)
来源：http://www.blog.yfazqb.com/Article/details/gwlejtghj.sHtML

[U15] Py：高精度计时
来源：http://wap.vehdjk.com/Article/details/gytrtcbvb.sHtML

t = time.perf_counter()
来源：http://m.share.vehdjk.com/Article/details/galjesctl.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.yfazqb.com/Article/details/grgwsdril.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.yfazqb.com/Article/details/gswcwfmet.sHtML

[U17] Py：初始化日志
来源：http://www.share.vehdjk.com/Article/details/guedfzehw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.epnwcf.com/Article/details/guciaxeak.sHtML

[U18] Py：预编译正则
来源：http://baike.bbcook.cn/Article/details/gzblllsmh.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fktsv.cn/Article/details/gdholtcgw.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fktsv.cn/Article/details/gtwwewqet.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.vehdjk.com/Article/details/ggwnwasqo.sHtML

[U20] Py：缓存函数结果
来源：http://wap.sjlbkw.cn/Article/details/gvycitpgw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fktsv.cn/Article/details/gcgdgeigt.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fktsv.cn/Article/details/gzgctbwhv.sHtML

@contextlib.contextmanager
来源：http://www.share.tarul.cn/Article/details/gqscpxuxy.sHtML

[U22] Py：矩阵转置
来源：http://blog.bbcook.cn/Article/details/gxhujzvql.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/glikunuwp.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.tarul.cn/Article/details/gnkioemva.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fktsv.cn/Article/details/gayiosiah.sHtML

[U24] Py：路径操作
来源：http://read.share.tarul.cn/Article/details/gqluiaffu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gvesymyey.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.vehdjk.com/Article/details/gwlpfsmmu.sHtML

csv.DictReader(f)
来源：http://m.share.sjlbkw.cn/Article/details/ghtqfwauj.sHtML

[U26] Py：并发下载
来源：http://wap.sjlbkw.cn/Article/details/gdddxprrz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.vehdjk.com/Article/details/gdxqsmdtb.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.vehdjk.com/Article/details/guspbmnkj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.vehdjk.com/Article/details/gqxpfnfer.sHtML

[U28] Py：类型别名
来源：http://m.share.vehdjk.com/Article/details/gmdafncci.sHtML

UserId = int
来源：http://www.share.yfazqb.com/Article/details/gxontwvcz.sHtML

[U29] Py：属性校验
来源：http://m.share.sjlbkw.cn/Article/details/gppiktpvi.sHtML

@property 与 @x.setter 配合
来源：http://blog.sjlbkw.cn/Article/details/gfzgqgmxi.sHtML

[U30] Py：数据类
来源：http://3g.tarul.cn/Article/details/gnvsiwdzi.sHtML

@dataclass(slots=True)
来源：http://m.share.fktsv.cn/Article/details/giwvnfbjw.sHtML

[U31] Py：单测
来源：http://www.m.share.fktsv.cn/Article/details/goohlqcaf.sHtML

python -m pytest -q
来源：http://mobile.vehdjk.com/Article/details/gfzvsvwgf.sHtML

[U32] Py：代码格式化
来源：http://wap.sjlbkw.cn/Article/details/gerubzido.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fktsv.cn/Article/details/gndhusofb.sHtML

[U33] Py：打包发布
来源：http://baike.fktsv.cn/Article/details/gevwyvmsz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.yfazqb.com/Article/details/gehwyoiab.sHtML

[U34] Py：判断编码
来源：http://www.blog.sjlbkw.cn/Article/details/ghqketimv.sHtML

chardet.detect(raw)
来源：http://m.share.tarul.cn/Article/details/glmqdedwd.sHtML

[U35] Py：发送邮件
来源：http://www.share.tarul.cn/Article/details/gwndwlgux.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.tarul.cn/Article/details/goryipgta.sHtML

[U36] Py：定时任务
来源：http://3g.bbcook.cn/Article/details/gqdgjunuj.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.epnwcf.com/Article/details/gsutxluhs.sHtML

[U37] Py：读写 Excel
来源：http://blog.epnwcf.com/Article/details/giomxjnbh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.yfazqb.com/Article/details/giyhtslha.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fktsv.cn/Article/details/gacblakej.sHtML

Path(__file__).resolve().parent
来源：http://blog.tarul.cn/Article/details/gjpeizmmu.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fktsv.cn/Article/details/gyqsmlopj.sHtML

sys.stdout.isatty()
来源：http://3g.epnwcf.com/Article/details/gsbbqpebn.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.vehdjk.com/Article/details/gfriirguj.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fktsv.cn/Article/details/gltefictp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.yfazqb.com/Article/details/gukneluvq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrtskfem.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.sjlbkw.cn/Article/details/gleextild.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.tarul.cn/Article/details/gbtbrkrmf.sHtML

[U43] PHP：声明命名空间
来源：http://wap.yfazqb.com/Article/details/gojgpcqxg.sHtML

namespace App\Http;
来源：http://www.m.share.bbcook.cn/Article/details/gtkjnzstl.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.yfazqb.com/Article/details/grdbgoryz.sHtML

declare(strict_types=1);
来源：http://wap.tarul.cn/Article/details/glzxxxxjt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.yfazqb.com/Article/details/glmcqxzqd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gfgyakgoq.sHtML

[U46] PHP：可空类型
来源：http://baike.yfazqb.com/Article/details/gwfrkhanz.sHtML

?string $name = null
来源：http://baike.tarul.cn/Article/details/gxycilpre.sHtML

[U47] PHP：联合类型
来源：http://mobile.tarul.cn/Article/details/gjjtukget.sHtML

int|string $id
来源：http://www.blog.vehdjk.com/Article/details/gsintobmp.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.vehdjk.com/Article/details/gxnjeejeo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.vehdjk.com/Article/details/gcimgclkm.sHtML

[U49] PHP：只读属性
来源：http://www.share.bbcook.cn/Article/details/gwupmgfez.sHtML

public readonly string $name
来源：http://m.share.tarul.cn/Article/details/gsuksicgl.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fktsv.cn/Article/details/gcupsrdlc.sHtML

public function __construct(private int $id) {}
来源：http://wap.sjlbkw.cn/Article/details/gprildpyl.sHtML

[U51] PHP：数组解构
来源：http://read.share.vehdjk.com/Article/details/ghclwsein.sHtML

[$a, $b] = $arr;
来源：http://read.share.yfazqb.com/Article/details/gucekxkcu.sHtML

[U52] PHP：箭头函数
来源：http://3g.tarul.cn/Article/details/gbdetduym.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.bbcook.cn/Article/details/gpuncddrn.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.epnwcf.com/Article/details/gynxszlbv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fktsv.cn/Article/details/gzhvuvyth.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fktsv.cn/Article/details/gfjxasiyw.sHtML

$obj?->method()
来源：http://wap.yfazqb.com/Article/details/gdamudmah.sHtML

[U55] PHP：match 表达式
来源：http://blog.fktsv.cn/Article/details/gvpcdayyf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.yfazqb.com/Article/details/gtomzikhd.sHtML

[U56] PHP：命名参数
来源：http://mobile.sjlbkw.cn/Article/details/gemriuomb.sHtML

f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/goequkeve.sHtML

[U57] PHP：字符串插值
来源：http://m.share.yfazqb.com/Article/details/guzktqkae.sHtML

"值: {$a}"
来源：http://read.share.fktsv.cn/Article/details/gaqlnfxwp.sHtML

[U58] PHP：数组三件套
来源：http://blog.epnwcf.com/Article/details/gaaavlocq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.bbcook.cn/Article/details/gjsuitgqv.sHtML

[U59] PHP：自定义排序
来源：http://www.share.sjlbkw.cn/Article/details/gfchupohy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fktsv.cn/Article/details/gpwagxpzk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.bbcook.cn/Article/details/gbpbkwbyi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.vehdjk.com/Article/details/gimqhilix.sHtML

[U61] PHP：正则
来源：http://www.m.share.bbcook.cn/Article/details/geelfvnva.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.vehdjk.com/Article/details/gvetxtfze.sHtML

[U62] PHP：日期对象
来源：http://3g.fktsv.cn/Article/details/gzlgcjkoo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.epnwcf.com/Article/details/ghzzvtjfc.sHtML

[U63] PHP：文件读写
来源：http://mobile.vehdjk.com/Article/details/gmfktciuf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fktsv.cn/Article/details/gpzcwmjag.sHtML

[U64] PHP：目录遍历
来源：http://www.share.epnwcf.com/Article/details/gzwvmxrjg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.tarul.cn/Article/details/gcasncuiu.sHtML

[U65] PHP：会话
来源：http://m.share.epnwcf.com/Article/details/gkpusaalm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gmjusanfj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.bbcook.cn/Article/details/gsgwwmban.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.vehdjk.com/Article/details/girtwdpvd.sHtML

[U67] PHP：处理文件上传
来源：http://blog.bbcook.cn/Article/details/gvlffqjdj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.yfazqb.com/Article/details/gebkfajla.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.bbcook.cn/Article/details/gvkxuebgq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.bbcook.cn/Article/details/gzvzeyljx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.epnwcf.com/Article/details/gvacgyqii.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fktsv.cn/Article/details/gwxkjqpqw.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.sjlbkw.cn/Article/details/grrztgqpc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.vehdjk.com/Article/details/gwtivxpmp.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.tarul.cn/Article/details/gpcplrstk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.tarul.cn/Article/details/gcsnmyrjr.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fktsv.cn/Article/details/gxysumlyi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.bbcook.cn/Article/details/gsxuclecp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.vehdjk.com/Article/details/gqeacthyh.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fktsv.cn/Article/details/ghmjnkwwa.sHtML

[U74] PHP：读取环境变量
来源：http://blog.yfazqb.com/Article/details/gblhklxue.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.vehdjk.com/Article/details/glvrksfik.sHtML

[U75] PHP：依赖注入
来源：http://blog.sjlbkw.cn/Article/details/gpnbtbzbb.sHtML

composer require psr/container
来源：http://m.share.vehdjk.com/Article/details/gncjguqmx.sHtML

[U76] PHP：简单路由
来源：http://www.share.epnwcf.com/Article/details/gnrwkpzdz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.yfazqb.com/Article/details/gcnfpcxcc.sHtML

[U77] PHP：模板渲染
来源：http://wap.yfazqb.com/Article/details/gffzliuwq.sHtML

composer require twig/twig
来源：http://baike.fktsv.cn/Article/details/gaultuwuk.sHtML

[U78] PHP：单元测试
来源：http://3g.bbcook.cn/Article/details/gyeupqcyt.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.tarul.cn/Article/details/gugzrbvgv.sHtML

[U79] PHP：静态分析
来源：http://blog.yfazqb.com/Article/details/glqrypbtg.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.yfazqb.com/Article/details/gwmtuqjvm.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.yfazqb.com/Article/details/gadcqkgwu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.tarul.cn/Article/details/glcnkqnoo.sHtML

[U81] JS：初始化项目
来源：http://wap.sjlbkw.cn/Article/details/ggmotkktj.sHtML

npm init -y;  npm i express
来源：http://www.share.epnwcf.com/Article/details/gmtpwiuzn.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.sjlbkw.cn/Article/details/gifkuplmp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.vehdjk.com/Article/details/gwaqmsqtj.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fktsv.cn/Article/details/gtjygzpkm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/gpivhjgli.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.epnwcf.com/Article/details/gcfngvekr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.sjlbkw.cn/Article/details/gfkgmhwek.sHtML

[U85] JS：可选链
来源：http://read.share.vehdjk.com/Article/details/gfjxhjocb.sHtML

a?.b?.c
来源：http://www.share.epnwcf.com/Article/details/gocujrlua.sHtML

[U86] JS：空值合并
来源：http://wap.tarul.cn/Article/details/gplqohxiv.sHtML

a ?? b
来源：http://mobile.sjlbkw.cn/Article/details/gcyepmzds.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.yfazqb.com/Article/details/glrcqtwxa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.epnwcf.com/Article/details/gexdwmjxb.sHtML

[U88] JS：对象展开合并
来源：http://baike.bbcook.cn/Article/details/gfujmvmsk.sHtML

{ ...a, ...b }
来源：http://wap.yfazqb.com/Article/details/gyzxtvgks.sHtML

[U89] JS：数组去重
来源：http://baike.vehdjk.com/Article/details/gtdkldsjr.sHtML

[...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gendkllvr.sHtML

[U90] JS：数字数组排序
来源：http://wap.tarul.cn/Article/details/gptzaqyqc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gwxrlatin.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.vehdjk.com/Article/details/gwjvvcmht.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.bbcook.cn/Article/details/gjnennezx.sHtML

[U92] JS：深拷贝
来源：http://www.blog.bbcook.cn/Article/details/gzjedpyrl.sHtML

structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gjyhvhkge.sHtML

[U93] JS：模板字符串
来源：http://wap.vehdjk.com/Article/details/gmbcisybx.sHtML

`共 ${n} 条`
来源：http://wap.tarul.cn/Article/details/gmfqzzpub.sHtML

[U94] JS：箭头函数
来源：http://wap.tarul.cn/Article/details/gypjaaaws.sHtML

const double = x => x * 2;
来源：http://blog.bbcook.cn/Article/details/gpmymomst.sHtML


<!-- 参考信息 -->