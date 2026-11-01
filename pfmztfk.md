代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.share.vehdjk.com/Article/details/gbsfzsklv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/gesflqnua.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fktsv.cn/Article/details/gsaydamon.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.vehdjk.com/Article/details/gnruderdc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/ggyglaawy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.yfazqb.com/Article/details/gidqtsrqo.sHtML

[T08] Kotlin：数据类
来源：http://m.share.sjlbkw.cn/Article/details/gulgimrcp.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.tarul.cn/Article/details/gpqmmecql.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/ggyfhalth.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.vehdjk.com/Article/details/goedxipxg.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gdzzckklf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.bbcook.cn/Article/details/gvtfnlrfi.sHtML

[T11] Kotlin：协程
来源：http://baike.fktsv.cn/Article/details/gsnjizvhh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.yfazqb.com/Article/details/grywutcjt.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.sjlbkw.cn/Article/details/goilqmnpk.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gwvttfdwt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.bbcook.cn/Article/details/gfbjgayho.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fktsv.cn/Article/details/gzhfzymct.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.tarul.cn/Article/details/gbbtqrigy.sHtML

for (i in 1..10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/gyxeznndp.sHtML

[T15] Kotlin：接口
来源：http://read.share.vehdjk.com/Article/details/gyodmyrms.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.sjlbkw.cn/Article/details/gshxzmfox.sHtML

[T16] Swift：Hello World
来源：http://3g.tarul.cn/Article/details/geutxlalu.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gvhghdqjf.sHtML

[T17] Swift：变量与常量
来源：http://baike.fktsv.cn/Article/details/geycrjqcm.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fktsv.cn/Article/details/goiufvzpa.sHtML

[T18] Swift：字符串插值
来源：http://3g.epnwcf.com/Article/details/gfetbuqbo.sHtML

"值: \(b)"
来源：http://baike.yfazqb.com/Article/details/gmwjevxij.sHtML

[T19] Swift：可选绑定
来源：http://3g.tarul.cn/Article/details/gyckokjag.sHtML

if let n = opt { print(n) }
来源：http://read.share.bbcook.cn/Article/details/gnrlzussm.sHtML

[T20] Swift：数组操作
来源：http://baike.sjlbkw.cn/Article/details/gayrwgarq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.epnwcf.com/Article/details/gzlskmhnt.sHtML

[T21] Swift：遍历
来源：http://www.m.share.epnwcf.com/Article/details/grszqzeni.sHtML

for x in a { print(x) }
来源：http://3g.fktsv.cn/Article/details/gmxrfvaoq.sHtML

[T22] Swift：字典
来源：http://m.share.bbcook.cn/Article/details/gteqbrbpq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.bbcook.cn/Article/details/gfdyphckr.sHtML

[T23] Swift：函数
来源：http://www.blog.vehdjk.com/Article/details/gxtgrtofa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.bbcook.cn/Article/details/gvbcvwtch.sHtML

[T24] Swift：闭包
来源：http://wap.epnwcf.com/Article/details/gzfsnrpje.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/geulejthv.sHtML

[T25] Swift：结构体
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlkxfrnt.sHtML

struct P { var x: Int }
来源：http://www.m.share.epnwcf.com/Article/details/gttqmwvqp.sHtML

[T26] Swift：类与重写
来源：http://3g.yfazqb.com/Article/details/gfeeeyyje.sHtML

class A: Base { override func f() {} }
来源：http://www.share.yfazqb.com/Article/details/gvsbwnneg.sHtML

[T27] Swift：错误处理
来源：http://baike.tarul.cn/Article/details/gtplxxifl.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fktsv.cn/Article/details/gprqczyuw.sHtML

[T28] Swift：枚举
来源：http://www.share.tarul.cn/Article/details/geiendlvc.sHtML

enum Color { case red, green }
来源：http://3g.yfazqb.com/Article/details/ghvkaeown.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.epnwcf.com/Article/details/gnolioypr.sHtML

guard let x = opt else { return }
来源：http://blog.tarul.cn/Article/details/gmkvtfmpc.sHtML

[T30] Swift：协议
来源：http://3g.sjlbkw.cn/Article/details/gzchiexkw.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.bbcook.cn/Article/details/gyvouqmwm.sHtML

[T31] Lua：Hello World
来源：http://3g.bbcook.cn/Article/details/gtqahsmcg.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/ghbuwupeb.sHtML

[T32] Lua：局部变量
来源：http://www.share.fktsv.cn/Article/details/gvexxftni.sHtML

local a = 1
来源：http://read.share.vehdjk.com/Article/details/gkxhqsxwl.sHtML

[T33] Lua：表（数组）
来源：http://blog.yfazqb.com/Article/details/gjohfiqcz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.bbcook.cn/Article/details/geasdiuor.sHtML

[T34] Lua：遍历表
来源：http://3g.epnwcf.com/Article/details/gzvcgzgfo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.sjlbkw.cn/Article/details/gtrrhmkdc.sHtML

[T35] Lua：字典表
来源：http://m.share.yfazqb.com/Article/details/gwlggdrrk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.bbcook.cn/Article/details/gptjhyaje.sHtML

[T36] Lua：函数
来源：http://baike.vehdjk.com/Article/details/gawrgpsdw.sHtML

function add(a, b) return a + b end
来源：http://wap.epnwcf.com/Article/details/gtidliwcv.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.vehdjk.com/Article/details/guzmgyohc.sHtML

"a" .. "b"
来源：http://baike.bbcook.cn/Article/details/gytwfgglv.sHtML

[T38] Lua：条件
来源：http://mobile.bbcook.cn/Article/details/gxvplwqoy.sHtML

if x > 0 then print("正") end
来源：http://blog.bbcook.cn/Article/details/gsfneyhzf.sHtML

[T39] Lua：模式匹配
来源：http://m.share.tarul.cn/Article/details/gwzwlwdsg.sHtML

string.find(s, "%d+")
来源：http://read.share.bbcook.cn/Article/details/gwioxusjh.sHtML

[T40] Lua：元表
来源：http://mobile.epnwcf.com/Article/details/gfrombfor.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.bbcook.cn/Article/details/gkipipqqy.sHtML

[T41] Perl：Hello World
来源：http://www.share.tarul.cn/Article/details/gjvdkhebv.sHtML

print "Hello\n";
来源：http://mobile.sjlbkw.cn/Article/details/ggbopjoth.sHtML

[T42] Perl：变量类型
来源：http://3g.epnwcf.com/Article/details/gyckljxgz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.vehdjk.com/Article/details/gavdydlul.sHtML

[T43] Perl：字符串插值
来源：http://wap.yfazqb.com/Article/details/gudlhamfo.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/gtzkqmgly.sHtML

[T44] Perl：条件
来源：http://3g.fktsv.cn/Article/details/gmsyzreev.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.epnwcf.com/Article/details/gfsgoxvio.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.tarul.cn/Article/details/gxqhywzay.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.vehdjk.com/Article/details/guqyndjgw.sHtML

[T46] Perl：哈希操作
来源：http://m.share.yfazqb.com/Article/details/gfnlazbgx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/gwinevjqv.sHtML

[T47] Perl：正则捕获
来源：http://read.share.yfazqb.com/Article/details/gsbtqrpgv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.yfazqb.com/Article/details/gcyfdmdvd.sHtML

[T48] Perl：正则替换
来源：http://3g.yfazqb.com/Article/details/ggzrnzdus.sHtML

$s =~ s/old/new/g;
来源：http://3g.tarul.cn/Article/details/gvelradog.sHtML

[T49] Perl：函数
来源：http://3g.bbcook.cn/Article/details/gqjzeodxe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gehrgfjfy.sHtML

[T50] Perl：逐行读文件
来源：http://baike.tarul.cn/Article/details/gfudobphm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.yfazqb.com/Article/details/gdsjnmzha.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.tarul.cn/Article/details/gyuutozau.sHtML

[T51] Scala：Hello World
来源：http://m.share.vehdjk.com/Article/details/gekdmxitk.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/gnbcqyjub.sHtML

[T52] Scala：变量
来源：http://3g.yfazqb.com/Article/details/gymynsplu.sHtML

val a = 1;  var b = 2
来源：http://m.share.tarul.cn/Article/details/gppuigenq.sHtML

[T53] Scala：字符串插值
来源：http://wap.fktsv.cn/Article/details/gdasobjga.sHtML

s"值: $b"
来源：http://3g.vehdjk.com/Article/details/gztusxidt.sHtML

[T54] Scala：集合映射
来源：http://wap.fktsv.cn/Article/details/gyhoibclk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.yfazqb.com/Article/details/gdznuugdr.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gpwnbphxp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.yfazqb.com/Article/details/gqzfpqsrp.sHtML

[T56] Scala：样例类
来源：http://3g.bbcook.cn/Article/details/gbczpnrne.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/gjyrmofeg.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fktsv.cn/Article/details/gzeuiljpa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fktsv.cn/Article/details/gudwicnge.sHtML

[T58] Scala：函数定义
来源：http://www.blog.tarul.cn/Article/details/gpgfwrijy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/gnfgsgwip.sHtML

[T59] Scala：循环
来源：http://mobile.fktsv.cn/Article/details/gwhljobnu.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.yfazqb.com/Article/details/gvbzvgqif.sHtML

[T60] Scala：折叠
来源：http://m.share.sjlbkw.cn/Article/details/ghcoeilrb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fktsv.cn/Article/details/gcqaehxso.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gsgxndvbp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gxrcreajx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/guazkskba.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.tarul.cn/Article/details/gtfqigpkv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.sjlbkw.cn/Article/details/goalippsv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fktsv.cn/Article/details/gagczlqvw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.vehdjk.com/Article/details/gtkvqspuu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.vehdjk.com/Article/details/gbtthveuy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.tarul.cn/Article/details/gfoabgjcd.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/gxapseyym.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.epnwcf.com/Article/details/gxlqmmksm.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fktsv.cn/Article/details/gichhnhlp.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gnzvazbkk.sHtML

[U06] Py：合并两个字典
来源：http://mobile.bbcook.cn/Article/details/gzsbvmlfs.sHtML

{**a, **b}
来源：http://m.share.tarul.cn/Article/details/grbamrgpa.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.yfazqb.com/Article/details/gqiivpcgr.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.sjlbkw.cn/Article/details/glprnnlzk.sHtML

[U08] Py：展平二维列表
来源：http://baike.vehdjk.com/Article/details/gnqzqqpmt.sHtML

[y for x in nested for y in x]
来源：http://read.share.vehdjk.com/Article/details/gzdrccamo.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.vehdjk.com/Article/details/ggpkbzevq.sHtML

max(d, key=d.get)
来源：http://mobile.yfazqb.com/Article/details/gicgxcbis.sHtML

[U10] Py：按值排序字典
来源：http://www.share.sjlbkw.cn/Article/details/gkmzwltkl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.bbcook.cn/Article/details/gitcmgtob.sHtML

[U11] Py：生成器表达式
来源：http://mobile.vehdjk.com/Article/details/gzqfhwnkk.sHtML

(x * 2 for x in arr)
来源：http://m.share.bbcook.cn/Article/details/gpllvwlef.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fktsv.cn/Article/details/gsvvgofdw.sHtML

Counter(arr).most_common(3)
来源：http://baike.epnwcf.com/Article/details/gfbuknwzu.sHtML

[U13] Py：固定长度队列
来源：http://mobile.yfazqb.com/Article/details/gjqmjpvln.sHtML

deque(maxlen=10)
来源：http://read.share.tarul.cn/Article/details/gljzifjeo.sHtML

[U14] Py：分组收集到列表
来源：http://3g.epnwcf.com/Article/details/gnmxgiqzw.sHtML

defaultdict(list)
来源：http://mobile.fktsv.cn/Article/details/gdkphjdfw.sHtML

[U15] Py：高精度计时
来源：http://3g.yfazqb.com/Article/details/gshdsyusd.sHtML

t = time.perf_counter()
来源：http://blog.sjlbkw.cn/Article/details/gymvevkzg.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.tarul.cn/Article/details/gfsukizdy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.vehdjk.com/Article/details/gdebxktxi.sHtML

[U17] Py：初始化日志
来源：http://3g.epnwcf.com/Article/details/gulahdyfr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.epnwcf.com/Article/details/gjtweljou.sHtML

[U18] Py：预编译正则
来源：http://blog.fktsv.cn/Article/details/gwbswbjdb.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.vehdjk.com/Article/details/gzgtkwclg.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.sjlbkw.cn/Article/details/gxwbcmvzx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.bbcook.cn/Article/details/gqugjidoq.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.yfazqb.com/Article/details/gnsotqgku.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fktsv.cn/Article/details/gkalvxnbi.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.vehdjk.com/Article/details/ggqshhgxa.sHtML

@contextlib.contextmanager
来源：http://wap.fktsv.cn/Article/details/gqahzkmat.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.tarul.cn/Article/details/gvvnlfbbg.sHtML

list(zip(*m))
来源：http://3g.vehdjk.com/Article/details/gnvxizhuv.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.yfazqb.com/Article/details/gpgsjkvun.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.epnwcf.com/Article/details/gcrfrdqso.sHtML

[U24] Py：路径操作
来源：http://3g.vehdjk.com/Article/details/gvpypjotp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.yfazqb.com/Article/details/gfzajscyd.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fktsv.cn/Article/details/gcqabdvoq.sHtML

csv.DictReader(f)
来源：http://m.share.yfazqb.com/Article/details/grunppgdr.sHtML

[U26] Py：并发下载
来源：http://www.share.tarul.cn/Article/details/gmdmcdwqz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.vehdjk.com/Article/details/gnxeglqji.sHtML

[U27] Py：异步 HTTP
来源：http://blog.vehdjk.com/Article/details/gnawlconj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.epnwcf.com/Article/details/gczbqwmek.sHtML

[U28] Py：类型别名
来源：http://www.share.sjlbkw.cn/Article/details/gkscfysty.sHtML

UserId = int
来源：http://www.m.share.tarul.cn/Article/details/gtvddntmk.sHtML

[U29] Py：属性校验
来源：http://read.share.yfazqb.com/Article/details/gugeogahp.sHtML

@property 与 @x.setter 配合
来源：http://mobile.bbcook.cn/Article/details/gitjsnquq.sHtML

[U30] Py：数据类
来源：http://baike.epnwcf.com/Article/details/gsoyzcquw.sHtML

@dataclass(slots=True)
来源：http://www.m.share.epnwcf.com/Article/details/gkvknpecl.sHtML

[U31] Py：单测
来源：http://www.share.epnwcf.com/Article/details/gqwcjgzce.sHtML

python -m pytest -q
来源：http://baike.tarul.cn/Article/details/gidyfpoiy.sHtML

[U32] Py：代码格式化
来源：http://www.blog.yfazqb.com/Article/details/gcidwodte.sHtML

ruff format . && ruff check --fix .
来源：http://baike.tarul.cn/Article/details/ggwtursuc.sHtML

[U33] Py：打包发布
来源：http://www.share.vehdjk.com/Article/details/gisfomebi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.vehdjk.com/Article/details/gvgoguwwf.sHtML

[U34] Py：判断编码
来源：http://wap.sjlbkw.cn/Article/details/gtziaekmr.sHtML

chardet.detect(raw)
来源：http://wap.bbcook.cn/Article/details/gmqmdzxam.sHtML

[U35] Py：发送邮件
来源：http://wap.tarul.cn/Article/details/gbitxlqmx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.vehdjk.com/Article/details/grqpwhozn.sHtML

[U36] Py：定时任务
来源：http://read.share.yfazqb.com/Article/details/gaziixcvp.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.tarul.cn/Article/details/grgqepksz.sHtML

[U37] Py：读写 Excel
来源：http://baike.fktsv.cn/Article/details/gnnxfodxh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.bbcook.cn/Article/details/gcprygcsw.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.vehdjk.com/Article/details/gsctokbnd.sHtML

Path(__file__).resolve().parent
来源：http://wap.sjlbkw.cn/Article/details/gedcuabbs.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvchbjdr.sHtML

sys.stdout.isatty()
来源：http://read.share.yfazqb.com/Article/details/grrhlbzlt.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.sjlbkw.cn/Article/details/gmkzjyojt.sHtML

print("err", file=sys.stderr)
来源：http://mobile.yfazqb.com/Article/details/gkzlxdxka.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.yfazqb.com/Article/details/goubjlsva.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.bbcook.cn/Article/details/gqwntvwoj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fktsv.cn/Article/details/gfvhptdqu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.bbcook.cn/Article/details/gdymjtqev.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.vehdjk.com/Article/details/gxycvheqo.sHtML

namespace App\Http;
来源：http://mobile.bbcook.cn/Article/details/gbomphtah.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.sjlbkw.cn/Article/details/grdxzojmr.sHtML

declare(strict_types=1);
来源：http://3g.epnwcf.com/Article/details/gmxrvvwkj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fktsv.cn/Article/details/geaepcyvm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/guroopsnr.sHtML

[U46] PHP：可空类型
来源：http://m.share.vehdjk.com/Article/details/gkmwhzgkc.sHtML

?string $name = null
来源：http://m.share.tarul.cn/Article/details/gdjapuado.sHtML

[U47] PHP：联合类型
来源：http://www.share.vehdjk.com/Article/details/gzmdqvhbl.sHtML

int|string $id
来源：http://wap.sjlbkw.cn/Article/details/gxorvatxb.sHtML

[U48] PHP：纯枚举
来源：http://m.share.epnwcf.com/Article/details/gkdqkiwjn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.bbcook.cn/Article/details/gxyaxrbrk.sHtML

[U49] PHP：只读属性
来源：http://m.share.epnwcf.com/Article/details/gczhqaxrt.sHtML

public readonly string $name
来源：http://read.share.bbcook.cn/Article/details/ghshdjroj.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.sjlbkw.cn/Article/details/gghzuhtag.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gdccvterw.sHtML

[U51] PHP：数组解构
来源：http://mobile.tarul.cn/Article/details/gulvxppti.sHtML

[$a, $b] = $arr;
来源：http://www.share.yfazqb.com/Article/details/gsipejjzf.sHtML

[U52] PHP：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/gcsuhpugd.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.yfazqb.com/Article/details/ghgerlrui.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.tarul.cn/Article/details/gjxneapxa.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.bbcook.cn/Article/details/gxlblzmmr.sHtML

[U54] PHP：空安全调用
来源：http://m.share.tarul.cn/Article/details/gtfmaldrr.sHtML

$obj?->method()
来源：http://www.blog.fktsv.cn/Article/details/gfhompvsv.sHtML

[U55] PHP：match 表达式
来源：http://www.share.sjlbkw.cn/Article/details/gwjhssezk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.yfazqb.com/Article/details/giyzlcfbo.sHtML

[U56] PHP：命名参数
来源：http://baike.bbcook.cn/Article/details/gomsklpyc.sHtML

f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gttyfhtta.sHtML

[U57] PHP：字符串插值
来源：http://3g.tarul.cn/Article/details/gvkrjonsg.sHtML

"值: {$a}"
来源：http://wap.bbcook.cn/Article/details/gbslaxxvp.sHtML

[U58] PHP：数组三件套
来源：http://read.share.yfazqb.com/Article/details/gufuomidh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.epnwcf.com/Article/details/gvejrptbe.sHtML

[U59] PHP：自定义排序
来源：http://www.share.vehdjk.com/Article/details/ghtyrbnje.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/gthxijmfj.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.epnwcf.com/Article/details/gwmgncbxn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.vehdjk.com/Article/details/gzobvvmpu.sHtML

[U61] PHP：正则
来源：http://read.share.sjlbkw.cn/Article/details/gorjrvaxv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/gqvjfemjf.sHtML

[U62] PHP：日期对象
来源：http://www.blog.sjlbkw.cn/Article/details/ggiqaujfz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.bbcook.cn/Article/details/gbfkwuzwv.sHtML

[U63] PHP：文件读写
来源：http://www.blog.tarul.cn/Article/details/gtaqfqjqx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.tarul.cn/Article/details/gnhfctooh.sHtML

[U64] PHP：目录遍历
来源：http://blog.epnwcf.com/Article/details/gxzvebpga.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fktsv.cn/Article/details/gkncflrgm.sHtML

[U65] PHP：会话
来源：http://blog.sjlbkw.cn/Article/details/gyfqnsfvs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.bbcook.cn/Article/details/gmkqkrrbu.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.epnwcf.com/Article/details/gxkrgwabg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.vehdjk.com/Article/details/gltnevnvd.sHtML

[U67] PHP：处理文件上传
来源：http://wap.bbcook.cn/Article/details/gguuyygis.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fktsv.cn/Article/details/gvekophjr.sHtML

[U68] PHP：PDO 连接
来源：http://3g.yfazqb.com/Article/details/gevjatdqo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfilnvzes.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fktsv.cn/Article/details/gruijsgsr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.yfazqb.com/Article/details/gzulabqlw.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fktsv.cn/Article/details/gzgytrfdb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fktsv.cn/Article/details/gyajzhbze.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fktsv.cn/Article/details/gmwzirheg.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.vehdjk.com/Article/details/gmglxxmuk.sHtML

[U72] PHP：写错误日志
来源：http://mobile.bbcook.cn/Article/details/glfvvxhro.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fktsv.cn/Article/details/gfriejhux.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.epnwcf.com/Article/details/gdlnjwhkt.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.bbcook.cn/Article/details/gwqbogrxo.sHtML

[U74] PHP：读取环境变量
来源：http://3g.tarul.cn/Article/details/ggzssvgzg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.epnwcf.com/Article/details/gxjbvsnbu.sHtML

[U75] PHP：依赖注入
来源：http://mobile.tarul.cn/Article/details/gnsizctby.sHtML

composer require psr/container
来源：http://www.blog.tarul.cn/Article/details/gwhpzzkcz.sHtML

[U76] PHP：简单路由
来源：http://read.share.epnwcf.com/Article/details/ghynbtfax.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fktsv.cn/Article/details/gljlzyrxs.sHtML

[U77] PHP：模板渲染
来源：http://wap.vehdjk.com/Article/details/gqglicjcw.sHtML

composer require twig/twig
来源：http://mobile.sjlbkw.cn/Article/details/giuivmitm.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.sjlbkw.cn/Article/details/guurdggeh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fktsv.cn/Article/details/grrdfgrao.sHtML

[U79] PHP：静态分析
来源：http://3g.bbcook.cn/Article/details/gwxvappgh.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.bbcook.cn/Article/details/gdwajutny.sHtML

[U80] PHP：代码规范修复
来源：http://blog.sjlbkw.cn/Article/details/guthlppuz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fktsv.cn/Article/details/ghkwahvnz.sHtML

[U81] JS：初始化项目
来源：http://www.share.sjlbkw.cn/Article/details/gwbegjwzd.sHtML

npm init -y;  npm i express
来源：http://3g.fktsv.cn/Article/details/grgsflykf.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fktsv.cn/Article/details/gzzhsjelu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.bbcook.cn/Article/details/gpassqfog.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.vehdjk.com/Article/details/glugczine.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.bbcook.cn/Article/details/govdfojsx.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.bbcook.cn/Article/details/gcdtzimik.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.yfazqb.com/Article/details/gvaddghck.sHtML

[U85] JS：可选链
来源：http://www.share.fktsv.cn/Article/details/ghmtvxfuc.sHtML

a?.b?.c
来源：http://blog.yfazqb.com/Article/details/gpfjnxqyg.sHtML

[U86] JS：空值合并
来源：http://www.blog.epnwcf.com/Article/details/gsemgeewo.sHtML

a ?? b
来源：http://www.m.share.vehdjk.com/Article/details/gdswjewtg.sHtML

[U87] JS：解构默认值
来源：http://mobile.tarul.cn/Article/details/gbiosmkrl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.bbcook.cn/Article/details/gsaurqfcg.sHtML

[U88] JS：对象展开合并
来源：http://blog.epnwcf.com/Article/details/gggauzoei.sHtML

{ ...a, ...b }
来源：http://mobile.tarul.cn/Article/details/gykuhzduw.sHtML

[U89] JS：数组去重
来源：http://mobile.yfazqb.com/Article/details/gxagrbbxv.sHtML

[...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gdjhrpzti.sHtML

[U90] JS：数字数组排序
来源：http://www.share.vehdjk.com/Article/details/gfkinbnwq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gcevvazlp.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fktsv.cn/Article/details/gaffrggge.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.bbcook.cn/Article/details/gmuxriwtd.sHtML

[U92] JS：深拷贝
来源：http://mobile.tarul.cn/Article/details/gzzyjmina.sHtML

structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gflebhtbt.sHtML


<!-- 参考信息 -->