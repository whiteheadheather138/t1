代发 wailian999

[T05] Kotlin：when 表达式
来源：http://blog.yfazqb.com/Article/details/gzjilcpwv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fktsv.cn/Article/details/grdvwxqnw.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gfpszepcx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.yfazqb.com/Article/details/gvcpbjxur.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gutvypwjm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.epnwcf.com/Article/details/ghpdpmlkc.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.vehdjk.com/Article/details/guoizlzlg.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fktsv.cn/Article/details/gxgqaeftl.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.epnwcf.com/Article/details/gjsswwknj.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.sjlbkw.cn/Article/details/goesljndq.sHtML

[T10] Kotlin：默认参数
来源：http://baike.vehdjk.com/Article/details/gxwnonqyl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.bbcook.cn/Article/details/gnihpdlri.sHtML

[T11] Kotlin：协程
来源：http://read.share.sjlbkw.cn/Article/details/guyrrdmlz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.yfazqb.com/Article/details/ggouedrvy.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.bbcook.cn/Article/details/geuyiwavr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gneyfbazk.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.bbcook.cn/Article/details/gkdexoxjc.sHtML

val m = mapOf("a" to 1)
来源：http://baike.epnwcf.com/Article/details/gwdtjifzl.sHtML

[T14] Kotlin：循环
来源：http://www.blog.epnwcf.com/Article/details/gtidfxalm.sHtML

for (i in 1..10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gmxhleeuj.sHtML

[T15] Kotlin：接口
来源：http://www.share.sjlbkw.cn/Article/details/gjuwhepet.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/gxiqmuqmx.sHtML

[T16] Swift：Hello World
来源：http://read.share.fktsv.cn/Article/details/gizorchzm.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/gvvzhztvg.sHtML

[T17] Swift：变量与常量
来源：http://baike.sjlbkw.cn/Article/details/gimrcbltm.sHtML

var a = 1;  let b = 2
来源：http://3g.sjlbkw.cn/Article/details/gzygmhqwv.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gqokhgjel.sHtML

"值: \(b)"
来源：http://3g.bbcook.cn/Article/details/goiaklmzd.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/gygdkyixb.sHtML

if let n = opt { print(n) }
来源：http://m.share.tarul.cn/Article/details/gwuytqxtu.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/gqjxlpjlx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gcszkwgge.sHtML

[T21] Swift：遍历
来源：http://www.blog.vehdjk.com/Article/details/gmvxrxcjw.sHtML

for x in a { print(x) }
来源：http://www.share.bbcook.cn/Article/details/gegydwiiy.sHtML

[T22] Swift：字典
来源：http://www.m.share.vehdjk.com/Article/details/gujuowskc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.yfazqb.com/Article/details/gtgxsszvf.sHtML

[T23] Swift：函数
来源：http://www.blog.tarul.cn/Article/details/girkthbdl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fktsv.cn/Article/details/ggitrzvfx.sHtML

[T24] Swift：闭包
来源：http://www.m.share.tarul.cn/Article/details/gwspgvcjp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fktsv.cn/Article/details/gaozikmio.sHtML

[T25] Swift：结构体
来源：http://www.m.share.bbcook.cn/Article/details/gfpvxediu.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/gqxsvanwn.sHtML

[T26] Swift：类与重写
来源：http://www.blog.bbcook.cn/Article/details/gsnzhlbws.sHtML

class A: Base { override func f() {} }
来源：http://m.share.vehdjk.com/Article/details/gxrrdxaht.sHtML

[T27] Swift：错误处理
来源：http://www.blog.vehdjk.com/Article/details/gokdnzshz.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fktsv.cn/Article/details/ggxtjzmor.sHtML

[T28] Swift：枚举
来源：http://m.share.tarul.cn/Article/details/glcngyyak.sHtML

enum Color { case red, green }
来源：http://baike.epnwcf.com/Article/details/gqsqyhddr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.vehdjk.com/Article/details/gdcyudjoj.sHtML

guard let x = opt else { return }
来源：http://www.share.bbcook.cn/Article/details/gloplukpn.sHtML

[T30] Swift：协议
来源：http://3g.bbcook.cn/Article/details/ganfnbelg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.tarul.cn/Article/details/gekfwajhs.sHtML

[T31] Lua：Hello World
来源：http://wap.vehdjk.com/Article/details/ghsrgkplh.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/gesoeabtm.sHtML

[T32] Lua：局部变量
来源：http://www.share.epnwcf.com/Article/details/ghshvfajy.sHtML

local a = 1
来源：http://mobile.fktsv.cn/Article/details/gksjivhbi.sHtML

[T33] Lua：表（数组）
来源：http://3g.fktsv.cn/Article/details/gaqrtpxte.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.yfazqb.com/Article/details/guzicqfiq.sHtML

[T34] Lua：遍历表
来源：http://m.share.sjlbkw.cn/Article/details/gsmhbcgyr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.yfazqb.com/Article/details/gkzyziatp.sHtML

[T35] Lua：字典表
来源：http://baike.yfazqb.com/Article/details/gkyuexwdz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.bbcook.cn/Article/details/gvkdgvehr.sHtML

[T36] Lua：函数
来源：http://www.m.share.tarul.cn/Article/details/geazkkndz.sHtML

function add(a, b) return a + b end
来源：http://www.share.bbcook.cn/Article/details/gedmwjusq.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gydiashzk.sHtML

"a" .. "b"
来源：http://mobile.bbcook.cn/Article/details/gamkdqgeg.sHtML

[T38] Lua：条件
来源：http://www.m.share.tarul.cn/Article/details/gdninyytg.sHtML

if x > 0 then print("正") end
来源：http://3g.vehdjk.com/Article/details/gqfeabdgk.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gnkabujag.sHtML

string.find(s, "%d+")
来源：http://www.m.share.tarul.cn/Article/details/ggdrvzhtg.sHtML

[T40] Lua：元表
来源：http://m.share.bbcook.cn/Article/details/gcvzpvras.sHtML

setmetatable({}, { __index = base })
来源：http://3g.vehdjk.com/Article/details/gbzlhxnjv.sHtML

[T41] Perl：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gsywxhqtk.sHtML

print "Hello\n";
来源：http://www.share.yfazqb.com/Article/details/gbhwvljvb.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fktsv.cn/Article/details/gnoeinqvc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.bbcook.cn/Article/details/gzoqxnfsn.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/godrsfxut.sHtML

"值: $a"
来源：http://m.share.vehdjk.com/Article/details/gncekfaou.sHtML

[T44] Perl：条件
来源：http://wap.yfazqb.com/Article/details/gduurjzms.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.tarul.cn/Article/details/gqwxfhlzj.sHtML

[T45] Perl：数组遍历
来源：http://wap.sjlbkw.cn/Article/details/gbcdysfla.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.epnwcf.com/Article/details/gxcbdrgjr.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gfyojjaxl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.epnwcf.com/Article/details/gwxbkgcxs.sHtML

[T47] Perl：正则捕获
来源：http://blog.vehdjk.com/Article/details/gvlpjhgeq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.tarul.cn/Article/details/gribdasot.sHtML

[T48] Perl：正则替换
来源：http://blog.vehdjk.com/Article/details/gxyqpymqx.sHtML

$s =~ s/old/new/g;
来源：http://wap.epnwcf.com/Article/details/gouqcpgxq.sHtML

[T49] Perl：函数
来源：http://m.share.yfazqb.com/Article/details/gozzfpzxu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gtjayedvo.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gybliuhyu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.bbcook.cn/Article/details/gpsidniuk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.tarul.cn/Article/details/gjcnjczdv.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gdgtpsqvq.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/glzjhfids.sHtML

[T52] Scala：变量
来源：http://read.share.epnwcf.com/Article/details/ggskhkuuo.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gujfvhlyk.sHtML

[T53] Scala：字符串插值
来源：http://read.share.yfazqb.com/Article/details/geshhdjhb.sHtML

s"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gxoihhhkv.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fktsv.cn/Article/details/gkusedbfz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/gdrmedgge.sHtML

[T55] Scala：集合过滤
来源：http://3g.tarul.cn/Article/details/gboxjztvg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.sjlbkw.cn/Article/details/gknsphogc.sHtML

[T56] Scala：样例类
来源：http://www.share.fktsv.cn/Article/details/gzvhsnxzj.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.bbcook.cn/Article/details/gsjzkrfdd.sHtML

[T57] Scala：模式匹配
来源：http://wap.bbcook.cn/Article/details/gttasieeo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgaaitcj.sHtML

[T58] Scala：函数定义
来源：http://www.share.vehdjk.com/Article/details/ghrvydrjm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.vehdjk.com/Article/details/gzskackmb.sHtML

[T59] Scala：循环
来源：http://www.share.bbcook.cn/Article/details/gljblnlfq.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gjwwyamkn.sHtML

[T60] Scala：折叠
来源：http://mobile.vehdjk.com/Article/details/gurfdmgpd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fktsv.cn/Article/details/gyptpjtpc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxnnkanys.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/grhhhxydu.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gihvniook.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.bbcook.cn/Article/details/gmleqsowg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/gbwuaztcc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fktsv.cn/Article/details/gdvescjwo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.epnwcf.com/Article/details/gfxnzwvfo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.sjlbkw.cn/Article/details/gmznetqjm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.tarul.cn/Article/details/gcibdbwfg.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fktsv.cn/Article/details/grksnsbkz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.yfazqb.com/Article/details/gcyjzsnzx.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.sjlbkw.cn/Article/details/gyamazfrg.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/gwlctxzgr.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fktsv.cn/Article/details/ganpznpiy.sHtML

{**a, **b}
来源：http://m.share.fktsv.cn/Article/details/gllrjjyyv.sHtML

[U07] Py：反转字典键值
来源：http://wap.bbcook.cn/Article/details/gmmjuoydo.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.yfazqb.com/Article/details/gpaxhcaye.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fktsv.cn/Article/details/gtfubdvpc.sHtML

[y for x in nested for y in x]
来源：http://blog.bbcook.cn/Article/details/gzyuobuvq.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.vehdjk.com/Article/details/gfthhnwhm.sHtML

max(d, key=d.get)
来源：http://www.m.share.tarul.cn/Article/details/gcjvauwzc.sHtML

[U10] Py：按值排序字典
来源：http://3g.tarul.cn/Article/details/grzcfeodf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.sjlbkw.cn/Article/details/gexiofmll.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fktsv.cn/Article/details/gwoqgkpwl.sHtML

(x * 2 for x in arr)
来源：http://baike.bbcook.cn/Article/details/gaopnzgvt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fktsv.cn/Article/details/gfvlvzbpr.sHtML

Counter(arr).most_common(3)
来源：http://wap.vehdjk.com/Article/details/gjdbnxbiq.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.sjlbkw.cn/Article/details/giaokvjex.sHtML

deque(maxlen=10)
来源：http://www.m.share.fktsv.cn/Article/details/gsbylkupm.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.tarul.cn/Article/details/gvmgcssmo.sHtML

defaultdict(list)
来源：http://blog.fktsv.cn/Article/details/gtppkoiij.sHtML

[U15] Py：高精度计时
来源：http://blog.tarul.cn/Article/details/grswhdnhc.sHtML

t = time.perf_counter()
来源：http://www.share.yfazqb.com/Article/details/gzjjfrjld.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.vehdjk.com/Article/details/gftbjvivn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.yfazqb.com/Article/details/gfctjmvir.sHtML

[U17] Py：初始化日志
来源：http://wap.tarul.cn/Article/details/gftiuerzp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.bbcook.cn/Article/details/gllbtpzar.sHtML

[U18] Py：预编译正则
来源：http://m.share.bbcook.cn/Article/details/gyyaaslji.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/gcrxkvbfs.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.epnwcf.com/Article/details/gocxfmaif.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.yfazqb.com/Article/details/gfkmhzedk.sHtML

[U20] Py：缓存函数结果
来源：http://wap.sjlbkw.cn/Article/details/gckrogdsh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fktsv.cn/Article/details/gziehblwd.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.vehdjk.com/Article/details/gsebfazvb.sHtML

@contextlib.contextmanager
来源：http://mobile.sjlbkw.cn/Article/details/gsgsysbzo.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.epnwcf.com/Article/details/gouibgutm.sHtML

list(zip(*m))
来源：http://www.m.share.yfazqb.com/Article/details/gnfoowvct.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.tarul.cn/Article/details/grslhlkzf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.vehdjk.com/Article/details/gkoydljsh.sHtML

[U24] Py：路径操作
来源：http://mobile.fktsv.cn/Article/details/gdnabjoeq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.epnwcf.com/Article/details/gmvwzybuj.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.yfazqb.com/Article/details/gazvgkfzw.sHtML

csv.DictReader(f)
来源：http://www.m.share.yfazqb.com/Article/details/gknprhzzz.sHtML

[U26] Py：并发下载
来源：http://mobile.fktsv.cn/Article/details/gwqizmnbv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.bbcook.cn/Article/details/gmcdxfnyv.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.sjlbkw.cn/Article/details/glzcihyuu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fktsv.cn/Article/details/ggktzagoy.sHtML

[U28] Py：类型别名
来源：http://www.share.tarul.cn/Article/details/gdmnotakg.sHtML

UserId = int
来源：http://read.share.yfazqb.com/Article/details/gkmpkgbyv.sHtML

[U29] Py：属性校验
来源：http://mobile.vehdjk.com/Article/details/gxduoeyem.sHtML

@property 与 @x.setter 配合
来源：http://mobile.bbcook.cn/Article/details/gqykjrukc.sHtML

[U30] Py：数据类
来源：http://blog.sjlbkw.cn/Article/details/gjhbfdnrr.sHtML

@dataclass(slots=True)
来源：http://www.blog.epnwcf.com/Article/details/gdgolwxtf.sHtML

[U31] Py：单测
来源：http://mobile.bbcook.cn/Article/details/gthwxancq.sHtML

python -m pytest -q
来源：http://www.m.share.fktsv.cn/Article/details/gskwztkfi.sHtML

[U32] Py：代码格式化
来源：http://mobile.sjlbkw.cn/Article/details/gqgagkyio.sHtML

ruff format . && ruff check --fix .
来源：http://3g.tarul.cn/Article/details/grvtokdhm.sHtML

[U33] Py：打包发布
来源：http://baike.tarul.cn/Article/details/gbcdxuhsa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.bbcook.cn/Article/details/gmhjweksr.sHtML

[U34] Py：判断编码
来源：http://www.blog.fktsv.cn/Article/details/goabrwwhl.sHtML

chardet.detect(raw)
来源：http://www.share.vehdjk.com/Article/details/gtoiiqsew.sHtML

[U35] Py：发送邮件
来源：http://baike.vehdjk.com/Article/details/gmmljbijk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.tarul.cn/Article/details/gkfamgfym.sHtML

[U36] Py：定时任务
来源：http://www.share.yfazqb.com/Article/details/gbhgelgst.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.epnwcf.com/Article/details/gmazhnxzb.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/ghyycnbhg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.sjlbkw.cn/Article/details/guxecozqy.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.bbcook.cn/Article/details/giqpqbgvi.sHtML

Path(__file__).resolve().parent
来源：http://3g.yfazqb.com/Article/details/gksorxvqc.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fktsv.cn/Article/details/gnzlkykks.sHtML

sys.stdout.isatty()
来源：http://blog.fktsv.cn/Article/details/garynyjpq.sHtML

[U40] Py：打印到标准错误
来源：http://wap.tarul.cn/Article/details/gqszbgjfv.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gchizvqyb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.tarul.cn/Article/details/gahvqvjhs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.sjlbkw.cn/Article/details/gyguargpm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.epnwcf.com/Article/details/gagtooqiq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fktsv.cn/Article/details/gkobxilzj.sHtML

[U43] PHP：声明命名空间
来源：http://blog.bbcook.cn/Article/details/gqglmukqm.sHtML

namespace App\Http;
来源：http://3g.yfazqb.com/Article/details/gsljinszl.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.vehdjk.com/Article/details/gmrkpkklg.sHtML

declare(strict_types=1);
来源：http://read.share.yfazqb.com/Article/details/gvjsnddkc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.yfazqb.com/Article/details/ggkgwtfmd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gviatadnd.sHtML

[U46] PHP：可空类型
来源：http://www.share.vehdjk.com/Article/details/gnkbrhtvo.sHtML

?string $name = null
来源：http://www.share.fktsv.cn/Article/details/gndqkcwjk.sHtML

[U47] PHP：联合类型
来源：http://www.blog.sjlbkw.cn/Article/details/gvemmlcbs.sHtML

int|string $id
来源：http://www.m.share.tarul.cn/Article/details/glzukgcva.sHtML

[U48] PHP：纯枚举
来源：http://baike.fktsv.cn/Article/details/ggwhinyhj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.bbcook.cn/Article/details/ggikjfqop.sHtML

[U49] PHP：只读属性
来源：http://3g.fktsv.cn/Article/details/ghnwqdjkt.sHtML

public readonly string $name
来源：http://www.share.tarul.cn/Article/details/ginjloxsn.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.vehdjk.com/Article/details/gncyfbbns.sHtML

public function __construct(private int $id) {}
来源：http://3g.epnwcf.com/Article/details/gbzxlfyyy.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.vehdjk.com/Article/details/gbsddjcbh.sHtML

[$a, $b] = $arr;
来源：http://wap.tarul.cn/Article/details/gffzqizpa.sHtML

[U52] PHP：箭头函数
来源：http://3g.tarul.cn/Article/details/gifyidchn.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.yfazqb.com/Article/details/gsqagkyrv.sHtML

[U53] PHP：空合并运算符
来源：http://wap.sjlbkw.cn/Article/details/gfpqunkpo.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.epnwcf.com/Article/details/gvwffwhto.sHtML

[U54] PHP：空安全调用
来源：http://blog.sjlbkw.cn/Article/details/ggyazqiqh.sHtML

$obj?->method()
来源：http://baike.yfazqb.com/Article/details/ghqqkkqlw.sHtML

[U55] PHP：match 表达式
来源：http://baike.vehdjk.com/Article/details/gbdvbkism.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.epnwcf.com/Article/details/gidkbhycd.sHtML

[U56] PHP：命名参数
来源：http://blog.tarul.cn/Article/details/gozfgzhhr.sHtML

f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gtppvlafi.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/ghhpibzoe.sHtML

"值: {$a}"
来源：http://mobile.epnwcf.com/Article/details/glmjpdwlr.sHtML

[U58] PHP：数组三件套
来源：http://wap.fktsv.cn/Article/details/gaybkfson.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.epnwcf.com/Article/details/gsvsufhst.sHtML

[U59] PHP：自定义排序
来源：http://wap.sjlbkw.cn/Article/details/gpoomglgu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gvukjpvnu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.sjlbkw.cn/Article/details/gdqxibcks.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.yfazqb.com/Article/details/ghlpkcicy.sHtML

[U61] PHP：正则
来源：http://3g.sjlbkw.cn/Article/details/gstjqptzd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/gurqjytuo.sHtML

[U62] PHP：日期对象
来源：http://3g.yfazqb.com/Article/details/gyhkskgnv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.sjlbkw.cn/Article/details/gfaloephp.sHtML

[U63] PHP：文件读写
来源：http://wap.epnwcf.com/Article/details/gxygybvlv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.sjlbkw.cn/Article/details/ggfgubiui.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.tarul.cn/Article/details/glnycpdhr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.vehdjk.com/Article/details/gcxrlrpaa.sHtML

[U65] PHP：会话
来源：http://m.share.sjlbkw.cn/Article/details/gkchdvjlw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.tarul.cn/Article/details/gzbbggjgb.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fktsv.cn/Article/details/gwilhjmie.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.bbcook.cn/Article/details/gfwuisvpq.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.vehdjk.com/Article/details/getjoczlc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fktsv.cn/Article/details/gbqditmtk.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fktsv.cn/Article/details/gfiqucxgt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.sjlbkw.cn/Article/details/gqtvckcpf.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.bbcook.cn/Article/details/ghhiicwge.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.epnwcf.com/Article/details/gfycrsvam.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.yfazqb.com/Article/details/gnmfbpgmz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.bbcook.cn/Article/details/gffnqmeoh.sHtML

[U71] PHP：抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gcsycjivp.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.tarul.cn/Article/details/gejucxrht.sHtML

[U72] PHP：写错误日志
来源：http://wap.sjlbkw.cn/Article/details/gojdekwon.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.epnwcf.com/Article/details/girleisfa.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.vehdjk.com/Article/details/gpqdkjcno.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.sjlbkw.cn/Article/details/gbdkibugf.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fktsv.cn/Article/details/ghiqdviho.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.sjlbkw.cn/Article/details/goaaiewfy.sHtML

[U75] PHP：依赖注入
来源：http://3g.sjlbkw.cn/Article/details/gixffuzbn.sHtML

composer require psr/container
来源：http://wap.bbcook.cn/Article/details/gmejkmlyx.sHtML

[U76] PHP：简单路由
来源：http://m.share.tarul.cn/Article/details/gapkxkmba.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.bbcook.cn/Article/details/gquxijaxl.sHtML

[U77] PHP：模板渲染
来源：http://www.share.bbcook.cn/Article/details/ghjtshizh.sHtML

composer require twig/twig
来源：http://mobile.tarul.cn/Article/details/griuobdgy.sHtML

[U78] PHP：单元测试
来源：http://wap.yfazqb.com/Article/details/gitojrahe.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.sjlbkw.cn/Article/details/gcynsbvqg.sHtML

[U79] PHP：静态分析
来源：http://www.share.fktsv.cn/Article/details/gfnmzpelq.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.epnwcf.com/Article/details/gobrwonyl.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fktsv.cn/Article/details/gghpebpyf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fktsv.cn/Article/details/gewtlbcnm.sHtML

[U81] JS：初始化项目
来源：http://baike.sjlbkw.cn/Article/details/gboiuqjys.sHtML

npm init -y;  npm i express
来源：http://www.m.share.epnwcf.com/Article/details/gkkbeqgmq.sHtML

[U82] JS：package.json 脚本
来源：http://wap.bbcook.cn/Article/details/gzhjviprt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.yfazqb.com/Article/details/gizioqjqm.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.sjlbkw.cn/Article/details/gsmijipav.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gzuawsdmy.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.yfazqb.com/Article/details/ggtscxmfk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.tarul.cn/Article/details/gsatflspw.sHtML

[U85] JS：可选链
来源：http://www.m.share.vehdjk.com/Article/details/gervsreyy.sHtML

a?.b?.c
来源：http://baike.bbcook.cn/Article/details/gvhuelwnt.sHtML

[U86] JS：空值合并
来源：http://mobile.bbcook.cn/Article/details/gxxmmesrf.sHtML

a ?? b
来源：http://www.share.yfazqb.com/Article/details/guvbavllz.sHtML

[U87] JS：解构默认值
来源：http://m.share.epnwcf.com/Article/details/ghhwovvhb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.bbcook.cn/Article/details/gokjewncc.sHtML

[U88] JS：对象展开合并
来源：http://wap.tarul.cn/Article/details/gznekwhvv.sHtML

{ ...a, ...b }
来源：http://www.share.vehdjk.com/Article/details/gowsndixl.sHtML

[U89] JS：数组去重
来源：http://blog.yfazqb.com/Article/details/ggzgpyhtu.sHtML

[...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/geyvaxrdw.sHtML

[U90] JS：数字数组排序
来源：http://mobile.bbcook.cn/Article/details/gqdyqvxof.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gnqtrnqwo.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.vehdjk.com/Article/details/gcbtarstu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.vehdjk.com/Article/details/ggklwqrxe.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gcyibgruq.sHtML

structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gvfmuudmh.sHtML


<!-- 参考信息 -->