代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gscqpvvwt.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gznrgwnvq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fktsv.cn/Article/details/gndehapjo.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gbwnysgls.sHtML

[T01] Kotlin：Hello World
来源：http://wap.bbcook.cn/Article/details/gbkrfmzfm.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gvqenvjhp.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.yfazqb.com/Article/details/gxyydtvgl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.yfazqb.com/Article/details/ggwmckuzc.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.epnwcf.com/Article/details/gmtvkszsy.sHtML

"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gwcvvcjli.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fktsv.cn/Article/details/gqtozezwl.sHtML

val n: String? = null;  n?.length
来源：http://m.share.bbcook.cn/Article/details/guzyjsowm.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.sjlbkw.cn/Article/details/gnjyviddz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.sjlbkw.cn/Article/details/gpuenmbxo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.bbcook.cn/Article/details/gumuyaxwf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gkyajrlih.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.yfazqb.com/Article/details/glrfzdytp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.epnwcf.com/Article/details/gzcqdknsx.sHtML

[T08] Kotlin：数据类
来源：http://3g.sjlbkw.cn/Article/details/gjgbhrtuv.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.epnwcf.com/Article/details/gygohblir.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvxprzbb.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.yfazqb.com/Article/details/gxewpxadm.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.tarul.cn/Article/details/gbpmnhpvr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.tarul.cn/Article/details/ggmxcqsvx.sHtML

[T11] Kotlin：协程
来源：http://www.blog.epnwcf.com/Article/details/gmncckdur.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.epnwcf.com/Article/details/gyljacfpj.sHtML

[T12] Kotlin：解构声明
来源：http://wap.sjlbkw.cn/Article/details/ggzcazemh.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fktsv.cn/Article/details/gumajszze.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/gxnlzsqya.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fktsv.cn/Article/details/gzkaipnob.sHtML

[T14] Kotlin：循环
来源：http://baike.sjlbkw.cn/Article/details/gkwfaaaub.sHtML

for (i in 1..10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gcwzmejnk.sHtML

[T15] Kotlin：接口
来源：http://www.blog.bbcook.cn/Article/details/geuebzmko.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.tarul.cn/Article/details/ghnnxxgrp.sHtML

[T16] Swift：Hello World
来源：http://blog.yfazqb.com/Article/details/gpumqiqll.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gdfwvlrck.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.sjlbkw.cn/Article/details/gmtcadztv.sHtML

var a = 1;  let b = 2
来源：http://www.blog.yfazqb.com/Article/details/gnixbaehr.sHtML

[T18] Swift：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gydswkjev.sHtML

"值: \(b)"
来源：http://wap.bbcook.cn/Article/details/gatvgoiiw.sHtML

[T19] Swift：可选绑定
来源：http://mobile.yfazqb.com/Article/details/ggjwvzqdt.sHtML

if let n = opt { print(n) }
来源：http://3g.vehdjk.com/Article/details/gpqtzrdfa.sHtML

[T20] Swift：数组操作
来源：http://m.share.vehdjk.com/Article/details/gbmjxlcym.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.vehdjk.com/Article/details/gpklntbjv.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gfhhtpmvk.sHtML

for x in a { print(x) }
来源：http://www.m.share.vehdjk.com/Article/details/gcvhikacw.sHtML

[T22] Swift：字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpsmjhdj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.epnwcf.com/Article/details/ginsztngq.sHtML

[T23] Swift：函数
来源：http://m.share.fktsv.cn/Article/details/gydnmnlmd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gjiyifjki.sHtML

[T24] Swift：闭包
来源：http://wap.sjlbkw.cn/Article/details/gmmqhbzhv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gdyfeghij.sHtML

[T25] Swift：结构体
来源：http://www.share.yfazqb.com/Article/details/gnpwjdpxy.sHtML

struct P { var x: Int }
来源：http://blog.bbcook.cn/Article/details/ghyxamrse.sHtML

[T26] Swift：类与重写
来源：http://blog.tarul.cn/Article/details/gpqalbmne.sHtML

class A: Base { override func f() {} }
来源：http://baike.yfazqb.com/Article/details/gohlrgsoc.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gjacpaeax.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/gpsnhdkez.sHtML

[T28] Swift：枚举
来源：http://wap.yfazqb.com/Article/details/gilbopdgr.sHtML

enum Color { case red, green }
来源：http://blog.epnwcf.com/Article/details/gyenexthe.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.epnwcf.com/Article/details/gxrkdcoyi.sHtML

guard let x = opt else { return }
来源：http://www.share.bbcook.cn/Article/details/ghavdenuw.sHtML

[T30] Swift：协议
来源：http://m.share.sjlbkw.cn/Article/details/gfiedhvxt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.tarul.cn/Article/details/guyilydms.sHtML

[T31] Lua：Hello World
来源：http://3g.tarul.cn/Article/details/gifpfckps.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gerojjadr.sHtML

[T32] Lua：局部变量
来源：http://mobile.yfazqb.com/Article/details/gugeizfpa.sHtML

local a = 1
来源：http://www.share.yfazqb.com/Article/details/gvzgtbhgm.sHtML

[T33] Lua：表（数组）
来源：http://read.share.tarul.cn/Article/details/gqjlqyolo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fktsv.cn/Article/details/gqtkechtu.sHtML

[T34] Lua：遍历表
来源：http://m.share.tarul.cn/Article/details/gfyxoyzeb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.bbcook.cn/Article/details/genejjgvy.sHtML

[T35] Lua：字典表
来源：http://m.share.fktsv.cn/Article/details/gfgdxcffx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.sjlbkw.cn/Article/details/gpuukhdns.sHtML

[T36] Lua：函数
来源：http://3g.yfazqb.com/Article/details/gefsoives.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.yfazqb.com/Article/details/gvxrjmowx.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.tarul.cn/Article/details/gwbaockvt.sHtML

"a" .. "b"
来源：http://3g.sjlbkw.cn/Article/details/gnhrdbnpq.sHtML

[T38] Lua：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gakarpmeg.sHtML

if x > 0 then print("正") end
来源：http://www.share.bbcook.cn/Article/details/grpiyuphj.sHtML

[T39] Lua：模式匹配
来源：http://3g.bbcook.cn/Article/details/gqhdoszsd.sHtML

string.find(s, "%d+")
来源：http://www.share.fktsv.cn/Article/details/gcaokeaql.sHtML

[T40] Lua：元表
来源：http://wap.yfazqb.com/Article/details/gkmqsxqga.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.vehdjk.com/Article/details/gknuuzxoq.sHtML

[T41] Perl：Hello World
来源：http://blog.fktsv.cn/Article/details/gpozcgwcs.sHtML

print "Hello\n";
来源：http://3g.yfazqb.com/Article/details/gpyebgsei.sHtML

[T42] Perl：变量类型
来源：http://www.share.yfazqb.com/Article/details/gmdwakfkl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.yfazqb.com/Article/details/glgznblem.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gemzxwwow.sHtML

"值: $a"
来源：http://www.blog.vehdjk.com/Article/details/gadbgmzbp.sHtML

[T44] Perl：条件
来源：http://baike.yfazqb.com/Article/details/giolrydfj.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.sjlbkw.cn/Article/details/gnvptztlk.sHtML

[T45] Perl：数组遍历
来源：http://m.share.yfazqb.com/Article/details/gxhqvtshh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxdpfsyo.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gskjuprdc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fktsv.cn/Article/details/gbjsyepru.sHtML

[T47] Perl：正则捕获
来源：http://blog.epnwcf.com/Article/details/gdsunehxh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.sjlbkw.cn/Article/details/galgfvbrh.sHtML

[T48] Perl：正则替换
来源：http://m.share.yfazqb.com/Article/details/gevcvehgq.sHtML

$s =~ s/old/new/g;
来源：http://read.share.epnwcf.com/Article/details/gpuditsfw.sHtML

[T49] Perl：函数
来源：http://3g.vehdjk.com/Article/details/gysxrwloq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gdzlrxnmz.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gzimeinsa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.tarul.cn/Article/details/gwurumehf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.tarul.cn/Article/details/gfqqiryze.sHtML

[T51] Scala：Hello World
来源：http://3g.bbcook.cn/Article/details/gaoyyyfcc.sHtML

println("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gdkpsyuzg.sHtML

[T52] Scala：变量
来源：http://3g.yfazqb.com/Article/details/gfkvqdttt.sHtML

val a = 1;  var b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gcuexnfho.sHtML

[T53] Scala：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/guzonlvpk.sHtML

s"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gcaxuohar.sHtML

[T54] Scala：集合映射
来源：http://mobile.yfazqb.com/Article/details/gdnvawpxt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.yfazqb.com/Article/details/gerrcfmmr.sHtML

[T55] Scala：集合过滤
来源：http://wap.vehdjk.com/Article/details/gayvcfgke.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/gudytzkce.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fktsv.cn/Article/details/gcyicrqdl.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gffwxmgai.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gvrytekxa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.epnwcf.com/Article/details/ggyontnqk.sHtML

[T58] Scala：函数定义
来源：http://mobile.sjlbkw.cn/Article/details/gbfblnfpq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.epnwcf.com/Article/details/gdwrmvugs.sHtML

[T59] Scala：循环
来源：http://blog.sjlbkw.cn/Article/details/gpvzkprqg.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gdpdvwpur.sHtML

[T60] Scala：折叠
来源：http://wap.sjlbkw.cn/Article/details/gerymivtz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.sjlbkw.cn/Article/details/gcvualqvn.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gymigjbvk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fktsv.cn/Article/details/gktjwbwui.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtvxmgsve.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.bbcook.cn/Article/details/glllnbpzn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.bbcook.cn/Article/details/gnnpzezlr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.tarul.cn/Article/details/ggpfihqmz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.yfazqb.com/Article/details/gqdhemxcm.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/gaqcdangr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.yfazqb.com/Article/details/gshsowxjm.sHtML

[U04] Py：变量调试打印
来源：http://baike.fktsv.cn/Article/details/gazbnetyl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.epnwcf.com/Article/details/gxlmcmvux.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.sjlbkw.cn/Article/details/gsgpiuvnb.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/gnejztjyo.sHtML

[U06] Py：合并两个字典
来源：http://3g.bbcook.cn/Article/details/gtbxhyocr.sHtML

{**a, **b}
来源：http://mobile.fktsv.cn/Article/details/gaivoeaep.sHtML

[U07] Py：反转字典键值
来源：http://www.share.yfazqb.com/Article/details/gxgfwegbv.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.bbcook.cn/Article/details/gvslsoypn.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.vehdjk.com/Article/details/gincrrmuh.sHtML

[y for x in nested for y in x]
来源：http://baike.bbcook.cn/Article/details/gkzcaaaqg.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fktsv.cn/Article/details/ggfdxguki.sHtML

max(d, key=d.get)
来源：http://blog.tarul.cn/Article/details/gpfglddec.sHtML

[U10] Py：按值排序字典
来源：http://wap.tarul.cn/Article/details/gbruxwpxe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.sjlbkw.cn/Article/details/glptpywxm.sHtML

[U11] Py：生成器表达式
来源：http://read.share.tarul.cn/Article/details/ghfqdvkwu.sHtML

(x * 2 for x in arr)
来源：http://mobile.fktsv.cn/Article/details/gxmzpootk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fktsv.cn/Article/details/gwlwrjrld.sHtML

Counter(arr).most_common(3)
来源：http://blog.yfazqb.com/Article/details/giqdbdfve.sHtML

[U13] Py：固定长度队列
来源：http://m.share.yfazqb.com/Article/details/gwotpeaoq.sHtML

deque(maxlen=10)
来源：http://3g.tarul.cn/Article/details/gtyxiapul.sHtML

[U14] Py：分组收集到列表
来源：http://wap.bbcook.cn/Article/details/ghbrompys.sHtML

defaultdict(list)
来源：http://blog.sjlbkw.cn/Article/details/glydradmz.sHtML

[U15] Py：高精度计时
来源：http://3g.vehdjk.com/Article/details/gzeahqzqv.sHtML

t = time.perf_counter()
来源：http://www.share.bbcook.cn/Article/details/gdexdyrgr.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.tarul.cn/Article/details/glggfeend.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.yfazqb.com/Article/details/ghpwvbgkr.sHtML

[U17] Py：初始化日志
来源：http://wap.vehdjk.com/Article/details/gnbjxnnzj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.vehdjk.com/Article/details/gmsilafpp.sHtML

[U18] Py：预编译正则
来源：http://baike.tarul.cn/Article/details/gbaxcafvx.sHtML

pat = re.compile(r"\d+")
来源：http://3g.vehdjk.com/Article/details/ganafohhp.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.bbcook.cn/Article/details/guctgsuuo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.bbcook.cn/Article/details/grtwecpya.sHtML

[U20] Py：缓存函数结果
来源：http://baike.tarul.cn/Article/details/gevfhhvou.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.tarul.cn/Article/details/gfapnxsbw.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.bbcook.cn/Article/details/gifoctzli.sHtML

@contextlib.contextmanager
来源：http://m.share.bbcook.cn/Article/details/gmxjojcte.sHtML

[U22] Py：矩阵转置
来源：http://baike.yfazqb.com/Article/details/gxyfmdcin.sHtML

list(zip(*m))
来源：http://3g.vehdjk.com/Article/details/gsylooofl.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.tarul.cn/Article/details/gudqtjyhp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.tarul.cn/Article/details/gylantqmr.sHtML

[U24] Py：路径操作
来源：http://3g.vehdjk.com/Article/details/gmgbmjxde.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/gduhwolzy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.yfazqb.com/Article/details/gdrrbiytv.sHtML

csv.DictReader(f)
来源：http://www.share.tarul.cn/Article/details/gohrpqjyd.sHtML

[U26] Py：并发下载
来源：http://read.share.epnwcf.com/Article/details/gdmuwosbf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.tarul.cn/Article/details/gwpzlaqrf.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fktsv.cn/Article/details/gdtjmwrjw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fktsv.cn/Article/details/grrdrtbrt.sHtML

[U28] Py：类型别名
来源：http://read.share.epnwcf.com/Article/details/gihihgfla.sHtML

UserId = int
来源：http://mobile.bbcook.cn/Article/details/gexblargn.sHtML

[U29] Py：属性校验
来源：http://3g.vehdjk.com/Article/details/ggpkyzopw.sHtML

@property 与 @x.setter 配合
来源：http://mobile.sjlbkw.cn/Article/details/gvvsyvlfc.sHtML

[U30] Py：数据类
来源：http://www.share.bbcook.cn/Article/details/grostisiv.sHtML

@dataclass(slots=True)
来源：http://mobile.yfazqb.com/Article/details/ggoxdtgka.sHtML

[U31] Py：单测
来源：http://m.share.fktsv.cn/Article/details/gbnmgnhle.sHtML

python -m pytest -q
来源：http://baike.epnwcf.com/Article/details/ghlheshmi.sHtML

[U32] Py：代码格式化
来源：http://read.share.tarul.cn/Article/details/goknsdcnu.sHtML

ruff format . && ruff check --fix .
来源：http://blog.yfazqb.com/Article/details/gxeeyljfm.sHtML

[U33] Py：打包发布
来源：http://mobile.vehdjk.com/Article/details/gqlfphplw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.sjlbkw.cn/Article/details/gkgkjffdq.sHtML

[U34] Py：判断编码
来源：http://mobile.bbcook.cn/Article/details/gdpwpzyzc.sHtML

chardet.detect(raw)
来源：http://read.share.epnwcf.com/Article/details/gntzolien.sHtML

[U35] Py：发送邮件
来源：http://wap.bbcook.cn/Article/details/gibxfrsht.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.yfazqb.com/Article/details/guevbjaio.sHtML

[U36] Py：定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gwwmrumhu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fktsv.cn/Article/details/gqhurqkld.sHtML

[U37] Py：读写 Excel
来源：http://blog.yfazqb.com/Article/details/gkkrphbbu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.tarul.cn/Article/details/gstexmmam.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.epnwcf.com/Article/details/gsjsdkxdw.sHtML

Path(__file__).resolve().parent
来源：http://read.share.vehdjk.com/Article/details/gqvebmhxu.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.sjlbkw.cn/Article/details/grvsbohwy.sHtML

sys.stdout.isatty()
来源：http://baike.sjlbkw.cn/Article/details/grkuktoov.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.yfazqb.com/Article/details/gahqkoixg.sHtML

print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/grydckycn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.tarul.cn/Article/details/gjxkhfhty.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.epnwcf.com/Article/details/glgfphwqn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.sjlbkw.cn/Article/details/gfxfdthew.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.vehdjk.com/Article/details/grdmsdgmz.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.epnwcf.com/Article/details/gtcydgtyf.sHtML

namespace App\Http;
来源：http://www.m.share.bbcook.cn/Article/details/grrikmmbc.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.vehdjk.com/Article/details/gimbqgeax.sHtML

declare(strict_types=1);
来源：http://3g.yfazqb.com/Article/details/gvvzxkopl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.bbcook.cn/Article/details/gorvuhsbd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gxpkftsex.sHtML

[U46] PHP：可空类型
来源：http://baike.yfazqb.com/Article/details/guuazfkcm.sHtML

?string $name = null
来源：http://wap.epnwcf.com/Article/details/gdodtsemy.sHtML

[U47] PHP：联合类型
来源：http://mobile.yfazqb.com/Article/details/glqxwjzji.sHtML

int|string $id
来源：http://www.m.share.epnwcf.com/Article/details/gbtovcjva.sHtML

[U48] PHP：纯枚举
来源：http://wap.fktsv.cn/Article/details/gievvukpq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.yfazqb.com/Article/details/ghqzrltxn.sHtML

[U49] PHP：只读属性
来源：http://mobile.epnwcf.com/Article/details/gskxuadow.sHtML

public readonly string $name
来源：http://baike.yfazqb.com/Article/details/gaqnouuer.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.bbcook.cn/Article/details/gckioliny.sHtML

public function __construct(private int $id) {}
来源：http://m.share.sjlbkw.cn/Article/details/gmbsobytl.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.bbcook.cn/Article/details/gnsxwhycs.sHtML

[$a, $b] = $arr;
来源：http://www.blog.epnwcf.com/Article/details/gnfyypydh.sHtML

[U52] PHP：箭头函数
来源：http://3g.tarul.cn/Article/details/gnmbiptox.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.yfazqb.com/Article/details/gyttpnshn.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.vehdjk.com/Article/details/gbvruwfvx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.epnwcf.com/Article/details/gnvsvppnz.sHtML

[U54] PHP：空安全调用
来源：http://mobile.sjlbkw.cn/Article/details/gauvtgktf.sHtML

$obj?->method()
来源：http://www.share.yfazqb.com/Article/details/gazywdhbu.sHtML

[U55] PHP：match 表达式
来源：http://baike.sjlbkw.cn/Article/details/gmxhmidvi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.sjlbkw.cn/Article/details/gtsgobgnq.sHtML

[U56] PHP：命名参数
来源：http://wap.vehdjk.com/Article/details/ggkfnyily.sHtML

f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gzwzmmgwm.sHtML

[U57] PHP：字符串插值
来源：http://3g.epnwcf.com/Article/details/gmrkmgjik.sHtML

"值: {$a}"
来源：http://m.share.tarul.cn/Article/details/gkwhpchti.sHtML

[U58] PHP：数组三件套
来源：http://mobile.epnwcf.com/Article/details/gnckhugsm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.vehdjk.com/Article/details/gfirwwang.sHtML

[U59] PHP：自定义排序
来源：http://www.share.yfazqb.com/Article/details/gqsruyngk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/gvngifsqy.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.vehdjk.com/Article/details/gouslaowl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.vehdjk.com/Article/details/gsbqcgbgi.sHtML

[U61] PHP：正则
来源：http://mobile.vehdjk.com/Article/details/gawobutjw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.vehdjk.com/Article/details/gtuktulkc.sHtML

[U62] PHP：日期对象
来源：http://m.share.bbcook.cn/Article/details/gcxahjjuo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.yfazqb.com/Article/details/geszfmmcv.sHtML

[U63] PHP：文件读写
来源：http://wap.bbcook.cn/Article/details/glqjdtnlk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.vehdjk.com/Article/details/geheboylh.sHtML

[U64] PHP：目录遍历
来源：http://blog.vehdjk.com/Article/details/gdvjluxvn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.sjlbkw.cn/Article/details/gxvytdfif.sHtML

[U65] PHP：会话
来源：http://www.blog.yfazqb.com/Article/details/gyobbqfmy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gjlcxdcsa.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.epnwcf.com/Article/details/ghwjqqwiu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.bbcook.cn/Article/details/gdchxpfbm.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.bbcook.cn/Article/details/galiuhmex.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.sjlbkw.cn/Article/details/gmyqsobyg.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.yfazqb.com/Article/details/gkjoscpsp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.tarul.cn/Article/details/gstmwuaoh.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.epnwcf.com/Article/details/gauhyjxjm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.tarul.cn/Article/details/gqkxybyee.sHtML

[U70] PHP：PDO 事务
来源：http://wap.sjlbkw.cn/Article/details/gkrskjafr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.sjlbkw.cn/Article/details/gnugfmvzk.sHtML

[U71] PHP：抛出异常
来源：http://blog.sjlbkw.cn/Article/details/gbkxamutq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fktsv.cn/Article/details/glhcowppu.sHtML

[U72] PHP：写错误日志
来源：http://m.share.bbcook.cn/Article/details/gsoiwxvpo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.bbcook.cn/Article/details/gnsvenqez.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fktsv.cn/Article/details/gdkfmcyih.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.sjlbkw.cn/Article/details/gqlntarmw.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gawbtmntu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.yfazqb.com/Article/details/ggsyjbuix.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fktsv.cn/Article/details/grfqrrzyi.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/gcwpjqsbw.sHtML

[U76] PHP：简单路由
来源：http://mobile.tarul.cn/Article/details/gymonrvch.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.tarul.cn/Article/details/gkgouqltu.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.bbcook.cn/Article/details/gqwsrajty.sHtML

composer require twig/twig
来源：http://blog.vehdjk.com/Article/details/ganpoysgc.sHtML

[U78] PHP：单元测试
来源：http://blog.tarul.cn/Article/details/gjmfdyrgd.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.tarul.cn/Article/details/garogfwye.sHtML

[U79] PHP：静态分析
来源：http://blog.sjlbkw.cn/Article/details/gkxnlqwql.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.tarul.cn/Article/details/gbixrbjgm.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.vehdjk.com/Article/details/guoflffya.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.bbcook.cn/Article/details/gbwghjlgk.sHtML

[U81] JS：初始化项目
来源：http://baike.yfazqb.com/Article/details/gzuheofed.sHtML

npm init -y;  npm i express
来源：http://mobile.bbcook.cn/Article/details/gwkbmgtqg.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fktsv.cn/Article/details/gmhdejstt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.bbcook.cn/Article/details/gnhzpxhyj.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.bbcook.cn/Article/details/gndfvzbuz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.bbcook.cn/Article/details/gzzwzqmxv.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fktsv.cn/Article/details/gcsvptbsf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.bbcook.cn/Article/details/gvvmpvnqh.sHtML

[U85] JS：可选链
来源：http://3g.bbcook.cn/Article/details/gobuwaiqp.sHtML

a?.b?.c
来源：http://www.blog.tarul.cn/Article/details/gcjjhpyoz.sHtML

[U86] JS：空值合并
来源：http://www.share.tarul.cn/Article/details/gqeopnozr.sHtML

a ?? b
来源：http://mobile.bbcook.cn/Article/details/ggjuuwruj.sHtML


<!-- 参考信息 -->