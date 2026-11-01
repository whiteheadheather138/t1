代发 wailian999

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/gqswlushv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fktsv.cn/Article/details/gqpgjwqlf.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/ggddjpggj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.yfazqb.com/Article/details/gnntmapof.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/gdxgsvfkb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.epnwcf.com/Article/details/gfntwlprd.sHtML

[T36] Lua：函数
来源：http://3g.sjlbkw.cn/Article/details/gvunzepor.sHtML

function add(a, b) return a + b end
来源：http://www.share.sjlbkw.cn/Article/details/gkryycrln.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.tarul.cn/Article/details/ggpmnuifd.sHtML

"a" .. "b"
来源：http://www.blog.fktsv.cn/Article/details/grbhgthpq.sHtML

[T38] Lua：条件
来源：http://m.share.vehdjk.com/Article/details/ggytxvusi.sHtML

if x > 0 then print("正") end
来源：http://read.share.sjlbkw.cn/Article/details/gwdhbuasp.sHtML

[T39] Lua：模式匹配
来源：http://baike.bbcook.cn/Article/details/gcfjlpwvo.sHtML

string.find(s, "%d+")
来源：http://www.share.epnwcf.com/Article/details/ghdzxymuv.sHtML

[T40] Lua：元表
来源：http://wap.yfazqb.com/Article/details/gpvpryzgu.sHtML

setmetatable({}, { __index = base })
来源：http://3g.yfazqb.com/Article/details/gaklmefsk.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gclkgzket.sHtML

print "Hello\n";
来源：http://mobile.vehdjk.com/Article/details/gikushqsd.sHtML

[T42] Perl：变量类型
来源：http://m.share.bbcook.cn/Article/details/gvnkfrsgv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gxzifqmrx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gohjahpdy.sHtML

"值: $a"
来源：http://www.share.vehdjk.com/Article/details/glenqxzms.sHtML

[T44] Perl：条件
来源：http://baike.tarul.cn/Article/details/gtsybxzsn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.yfazqb.com/Article/details/gbyunwyfe.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fktsv.cn/Article/details/gnmrcfodu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.tarul.cn/Article/details/gylpzvvqv.sHtML

[T46] Perl：哈希操作
来源：http://3g.yfazqb.com/Article/details/gdgydvhwc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.epnwcf.com/Article/details/gduxolmem.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.yfazqb.com/Article/details/gpftymizm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.epnwcf.com/Article/details/glkakgore.sHtML

[T48] Perl：正则替换
来源：http://m.share.tarul.cn/Article/details/gfqanmjgr.sHtML

$s =~ s/old/new/g;
来源：http://www.share.epnwcf.com/Article/details/ggbaanvlg.sHtML

[T49] Perl：函数
来源：http://blog.yfazqb.com/Article/details/gtozcgqyj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gzmcnkucc.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gkpiaydhf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.epnwcf.com/Article/details/gtbmhfubh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.tarul.cn/Article/details/gxzsnoour.sHtML

[T51] Scala：Hello World
来源：http://www.blog.epnwcf.com/Article/details/ghzyyyynj.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/ggwbzjxwm.sHtML

[T52] Scala：变量
来源：http://www.share.epnwcf.com/Article/details/gfnvvwswr.sHtML

val a = 1;  var b = 2
来源：http://mobile.tarul.cn/Article/details/gpeecqxya.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gleugydgb.sHtML

s"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/giysdnaal.sHtML

[T54] Scala：集合映射
来源：http://blog.tarul.cn/Article/details/gpehhfnys.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.epnwcf.com/Article/details/gncmgiugq.sHtML

[T55] Scala：集合过滤
来源：http://baike.vehdjk.com/Article/details/gswmukoms.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.epnwcf.com/Article/details/gnunuzioy.sHtML

[T56] Scala：样例类
来源：http://www.share.bbcook.cn/Article/details/gjdqslylu.sHtML

case class User(name: String, age: Int)
来源：http://read.share.bbcook.cn/Article/details/gpiaifsrf.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gpilxtsrm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fktsv.cn/Article/details/gdrcekauy.sHtML

[T58] Scala：函数定义
来源：http://www.blog.tarul.cn/Article/details/gfhyesvfq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fktsv.cn/Article/details/gntthczil.sHtML

[T59] Scala：循环
来源：http://3g.fktsv.cn/Article/details/ghswbklxu.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gtytykvlv.sHtML

[T60] Scala：折叠
来源：http://read.share.bbcook.cn/Article/details/glpdhitai.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.bbcook.cn/Article/details/gxfemthpc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmfqnizxn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.bbcook.cn/Article/details/givyefrvk.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gdacexzft.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.epnwcf.com/Article/details/gqklvkaoy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.bbcook.cn/Article/details/gwgnaxnbx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.bbcook.cn/Article/details/gvqlxllss.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.epnwcf.com/Article/details/gbvagjxuu.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fktsv.cn/Article/details/gebwilpex.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.tarul.cn/Article/details/gghqerzyy.sHtML

[U04] Py：变量调试打印
来源：http://mobile.epnwcf.com/Article/details/gocccvlqp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.tarul.cn/Article/details/gehqovafo.sHtML

[U05] Py：列表去重且保序
来源：http://blog.yfazqb.com/Article/details/gbllmwrss.sHtML

list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/glyipigfh.sHtML

[U06] Py：合并两个字典
来源：http://m.share.epnwcf.com/Article/details/gcpfmmbca.sHtML

{**a, **b}
来源：http://wap.sjlbkw.cn/Article/details/gnayoiklx.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.tarul.cn/Article/details/gkrftresd.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.tarul.cn/Article/details/guahbwquz.sHtML

[U08] Py：展平二维列表
来源：http://m.share.sjlbkw.cn/Article/details/gqiwurkel.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/gkifwhzuk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.tarul.cn/Article/details/ggqzvabem.sHtML

max(d, key=d.get)
来源：http://m.share.tarul.cn/Article/details/gdbpckoli.sHtML

[U10] Py：按值排序字典
来源：http://read.share.sjlbkw.cn/Article/details/glinfmyxa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.sjlbkw.cn/Article/details/gdsthyquv.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.epnwcf.com/Article/details/gbdtwxttb.sHtML

(x * 2 for x in arr)
来源：http://read.share.yfazqb.com/Article/details/gxixdbchg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.yfazqb.com/Article/details/gihdexzje.sHtML

Counter(arr).most_common(3)
来源：http://wap.fktsv.cn/Article/details/guwtmlelz.sHtML

[U13] Py：固定长度队列
来源：http://blog.tarul.cn/Article/details/ghmwxahby.sHtML

deque(maxlen=10)
来源：http://wap.epnwcf.com/Article/details/gpfqovkyt.sHtML

[U14] Py：分组收集到列表
来源：http://blog.epnwcf.com/Article/details/gsprfaiwf.sHtML

defaultdict(list)
来源：http://www.blog.fktsv.cn/Article/details/gjaspeixe.sHtML

[U15] Py：高精度计时
来源：http://mobile.sjlbkw.cn/Article/details/grrwxomuo.sHtML

t = time.perf_counter()
来源：http://wap.fktsv.cn/Article/details/glkckvjxn.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fktsv.cn/Article/details/gfimctcet.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.epnwcf.com/Article/details/gwiwyutpe.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.epnwcf.com/Article/details/gqiomgtam.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fktsv.cn/Article/details/gwjqbfdxw.sHtML

[U18] Py：预编译正则
来源：http://3g.tarul.cn/Article/details/gbsrgdoqm.sHtML

pat = re.compile(r"\d+")
来源：http://wap.epnwcf.com/Article/details/gdyqwuuam.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.tarul.cn/Article/details/gbvrpqpez.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.sjlbkw.cn/Article/details/glmxnoidz.sHtML

[U20] Py：缓存函数结果
来源：http://baike.epnwcf.com/Article/details/ghnbknalk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.tarul.cn/Article/details/ghypnmqjj.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.vehdjk.com/Article/details/gawlvnndi.sHtML

@contextlib.contextmanager
来源：http://mobile.yfazqb.com/Article/details/gxragvjvb.sHtML

[U22] Py：矩阵转置
来源：http://blog.epnwcf.com/Article/details/gxiyvxmel.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/gabntuusv.sHtML

[U23] Py：分块读取大文件
来源：http://3g.vehdjk.com/Article/details/gaqpjiubh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.sjlbkw.cn/Article/details/gyeziprey.sHtML

[U24] Py：路径操作
来源：http://wap.fktsv.cn/Article/details/gupblobik.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gcwddwcey.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.yfazqb.com/Article/details/gncbuclpw.sHtML

csv.DictReader(f)
来源：http://www.blog.yfazqb.com/Article/details/gqarjeyda.sHtML

[U26] Py：并发下载
来源：http://www.share.sjlbkw.cn/Article/details/gfpvfyqqa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.epnwcf.com/Article/details/gbdqrztyb.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fktsv.cn/Article/details/gccrcdenk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.vehdjk.com/Article/details/gdmabfexy.sHtML

[U28] Py：类型别名
来源：http://wap.vehdjk.com/Article/details/golrywkwn.sHtML

UserId = int
来源：http://3g.vehdjk.com/Article/details/gttunvyjs.sHtML

[U29] Py：属性校验
来源：http://wap.tarul.cn/Article/details/gzwkxnbje.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.vehdjk.com/Article/details/gjfhtlkjq.sHtML

[U30] Py：数据类
来源：http://baike.vehdjk.com/Article/details/grhymknet.sHtML

@dataclass(slots=True)
来源：http://m.share.bbcook.cn/Article/details/gaspyswvq.sHtML

[U31] Py：单测
来源：http://mobile.yfazqb.com/Article/details/gngwlyrab.sHtML

python -m pytest -q
来源：http://3g.sjlbkw.cn/Article/details/ghauprqti.sHtML

[U32] Py：代码格式化
来源：http://wap.yfazqb.com/Article/details/gathryqub.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fktsv.cn/Article/details/gynzgeznj.sHtML

[U33] Py：打包发布
来源：http://mobile.vehdjk.com/Article/details/ggepmelqr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fktsv.cn/Article/details/gvyymhufr.sHtML

[U34] Py：判断编码
来源：http://baike.fktsv.cn/Article/details/gcubgvuqv.sHtML

chardet.detect(raw)
来源：http://wap.vehdjk.com/Article/details/gwnprsnul.sHtML

[U35] Py：发送邮件
来源：http://m.share.yfazqb.com/Article/details/geojrutwl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.tarul.cn/Article/details/gxlawbbaj.sHtML

[U36] Py：定时任务
来源：http://3g.epnwcf.com/Article/details/gtwtgghdt.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.vehdjk.com/Article/details/gyvekbyux.sHtML

[U37] Py：读写 Excel
来源：http://blog.tarul.cn/Article/details/gyllgrbex.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.vehdjk.com/Article/details/gwdwrhlqy.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fktsv.cn/Article/details/gtnfrlest.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fktsv.cn/Article/details/gvazdwpab.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.tarul.cn/Article/details/gehmxlhzg.sHtML

sys.stdout.isatty()
来源：http://m.share.epnwcf.com/Article/details/gartdwgaq.sHtML

[U40] Py：打印到标准错误
来源：http://baike.epnwcf.com/Article/details/gwfnkezyu.sHtML

print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gbdqnvspg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.epnwcf.com/Article/details/gmlewbvzp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.bbcook.cn/Article/details/grilnslhn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.bbcook.cn/Article/details/gkzvjtlrs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.yfazqb.com/Article/details/gickueght.sHtML

[U43] PHP：声明命名空间
来源：http://wap.epnwcf.com/Article/details/gefzwslci.sHtML

namespace App\Http;
来源：http://wap.yfazqb.com/Article/details/gmtmeltct.sHtML

[U44] PHP：开启严格类型
来源：http://wap.yfazqb.com/Article/details/gxwayiuoh.sHtML

declare(strict_types=1);
来源：http://mobile.sjlbkw.cn/Article/details/gzujbedcd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.yfazqb.com/Article/details/gfzjbbcpv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gtnqjlitb.sHtML

[U46] PHP：可空类型
来源：http://blog.tarul.cn/Article/details/gmchaplkq.sHtML

?string $name = null
来源：http://3g.tarul.cn/Article/details/gthkviowc.sHtML

[U47] PHP：联合类型
来源：http://baike.fktsv.cn/Article/details/gthngbwjt.sHtML

int|string $id
来源：http://wap.yfazqb.com/Article/details/ggjfxbthy.sHtML

[U48] PHP：纯枚举
来源：http://3g.fktsv.cn/Article/details/gaujcrxal.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.tarul.cn/Article/details/gtqhwtqng.sHtML

[U49] PHP：只读属性
来源：http://www.share.epnwcf.com/Article/details/gwjukymcp.sHtML

public readonly string $name
来源：http://www.blog.fktsv.cn/Article/details/gnksrpwje.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.tarul.cn/Article/details/gibctzjly.sHtML

public function __construct(private int $id) {}
来源：http://mobile.yfazqb.com/Article/details/gdnpmflel.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.yfazqb.com/Article/details/gloluqeen.sHtML

[$a, $b] = $arr;
来源：http://3g.vehdjk.com/Article/details/gxqlmwqiz.sHtML

[U52] PHP：箭头函数
来源：http://www.share.bbcook.cn/Article/details/goqdzatlq.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.epnwcf.com/Article/details/gnxdirbqo.sHtML

[U53] PHP：空合并运算符
来源：http://3g.yfazqb.com/Article/details/gchgwmgjx.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.vehdjk.com/Article/details/glezzghsa.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.epnwcf.com/Article/details/glhdarmag.sHtML

$obj?->method()
来源：http://wap.vehdjk.com/Article/details/gkupclhri.sHtML

[U55] PHP：match 表达式
来源：http://mobile.vehdjk.com/Article/details/gwscswyre.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.vehdjk.com/Article/details/ggpwwwnqz.sHtML

[U56] PHP：命名参数
来源：http://wap.epnwcf.com/Article/details/gpnqbbhre.sHtML

f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/grywyrawb.sHtML

[U57] PHP：字符串插值
来源：http://blog.yfazqb.com/Article/details/gpvqzzcfe.sHtML

"值: {$a}"
来源：http://wap.epnwcf.com/Article/details/glhezvwuh.sHtML

[U58] PHP：数组三件套
来源：http://m.share.tarul.cn/Article/details/geakenpej.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.yfazqb.com/Article/details/gyrecxqus.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.bbcook.cn/Article/details/gtvyazwjh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.sjlbkw.cn/Article/details/gjwlfjnwo.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.yfazqb.com/Article/details/gymdkjrzr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.vehdjk.com/Article/details/gnmbyafan.sHtML

[U61] PHP：正则
来源：http://read.share.vehdjk.com/Article/details/ghfymnikz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.tarul.cn/Article/details/gfsnvprzm.sHtML

[U62] PHP：日期对象
来源：http://baike.epnwcf.com/Article/details/gdetstscx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.bbcook.cn/Article/details/gogulyuue.sHtML

[U63] PHP：文件读写
来源：http://read.share.vehdjk.com/Article/details/gfdqpyndk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.tarul.cn/Article/details/gfccssgno.sHtML

[U64] PHP：目录遍历
来源：http://wap.epnwcf.com/Article/details/gadyxzmcy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.epnwcf.com/Article/details/glmuwjlgh.sHtML

[U65] PHP：会话
来源：http://www.share.vehdjk.com/Article/details/gnhytmvhc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.yfazqb.com/Article/details/gvgrngako.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.vehdjk.com/Article/details/gafipizhm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.sjlbkw.cn/Article/details/gplrjggpj.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.epnwcf.com/Article/details/gydwbfmms.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.yfazqb.com/Article/details/gnbrpeyrq.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.tarul.cn/Article/details/ggsheptps.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fktsv.cn/Article/details/gqaqnjzcb.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.yfazqb.com/Article/details/gwwlcjdil.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.yfazqb.com/Article/details/ggicxziup.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.yfazqb.com/Article/details/gtuglvwmg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.yfazqb.com/Article/details/gguobyipi.sHtML

[U71] PHP：抛出异常
来源：http://blog.vehdjk.com/Article/details/gjpmnolsp.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.tarul.cn/Article/details/gbwshhwak.sHtML

[U72] PHP：写错误日志
来源：http://blog.yfazqb.com/Article/details/gyhbgzqgw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.sjlbkw.cn/Article/details/grszjzoov.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.sjlbkw.cn/Article/details/gbxgbshmh.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.yfazqb.com/Article/details/gswmfebdw.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.epnwcf.com/Article/details/giwlqitqx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fktsv.cn/Article/details/gwwsqssjo.sHtML

[U75] PHP：依赖注入
来源：http://www.share.tarul.cn/Article/details/gwhwoepqo.sHtML

composer require psr/container
来源：http://mobile.epnwcf.com/Article/details/gqfmsygom.sHtML

[U76] PHP：简单路由
来源：http://wap.yfazqb.com/Article/details/gclekblug.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.bbcook.cn/Article/details/gupkmhbaz.sHtML

[U77] PHP：模板渲染
来源：http://read.share.epnwcf.com/Article/details/gbvesarfh.sHtML

composer require twig/twig
来源：http://3g.fktsv.cn/Article/details/gpsxlguxn.sHtML

[U78] PHP：单元测试
来源：http://wap.vehdjk.com/Article/details/gewrkhdil.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fktsv.cn/Article/details/gcbaldcnd.sHtML

[U79] PHP：静态分析
来源：http://www.share.yfazqb.com/Article/details/gsngijbpv.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fktsv.cn/Article/details/gxeadnzed.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.tarul.cn/Article/details/gplqwexbm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.sjlbkw.cn/Article/details/gsuqdunjo.sHtML

[U81] JS：初始化项目
来源：http://read.share.fktsv.cn/Article/details/gucnnnkgm.sHtML

npm init -y;  npm i express
来源：http://mobile.epnwcf.com/Article/details/gzoamdaqo.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fktsv.cn/Article/details/gnrfdwboa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.bbcook.cn/Article/details/gzbhcoivo.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.epnwcf.com/Article/details/gnxcmcjfx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fktsv.cn/Article/details/gwrgwvkew.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.bbcook.cn/Article/details/guhstavyg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.epnwcf.com/Article/details/gkdkxlssy.sHtML

[U85] JS：可选链
来源：http://www.share.bbcook.cn/Article/details/gourqzbfn.sHtML

a?.b?.c
来源：http://3g.bbcook.cn/Article/details/gzuhabalh.sHtML

[U86] JS：空值合并
来源：http://m.share.sjlbkw.cn/Article/details/gmtybcszb.sHtML

a ?? b
来源：http://3g.sjlbkw.cn/Article/details/gtoefemxm.sHtML

[U87] JS：解构默认值
来源：http://mobile.vehdjk.com/Article/details/gkkhypprk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.bbcook.cn/Article/details/gxzjhzhrc.sHtML

[U88] JS：对象展开合并
来源：http://wap.tarul.cn/Article/details/ggromjzyn.sHtML

{ ...a, ...b }
来源：http://www.share.fktsv.cn/Article/details/gptgeaiob.sHtML

[U89] JS：数组去重
来源：http://baike.vehdjk.com/Article/details/gjdfoqoip.sHtML

[...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gaeygbgjc.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.sjlbkw.cn/Article/details/gexovpvse.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gcffqlazu.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fktsv.cn/Article/details/guaydsnlj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.tarul.cn/Article/details/gqbpufnox.sHtML

[U92] JS：深拷贝
来源：http://www.blog.tarul.cn/Article/details/gljrcreaf.sHtML

structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gdrwvwdmd.sHtML

[U93] JS：模板字符串
来源：http://wap.epnwcf.com/Article/details/gwpevqfdx.sHtML

`共 ${n} 条`
来源：http://wap.bbcook.cn/Article/details/gzarvhirr.sHtML

[U94] JS：箭头函数
来源：http://www.share.bbcook.cn/Article/details/gnfawrwwx.sHtML

const double = x => x * 2;
来源：http://www.blog.sjlbkw.cn/Article/details/gakobqswp.sHtML

[U95] JS：Promise 包装
来源：http://www.share.vehdjk.com/Article/details/gkbydcabr.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.sjlbkw.cn/Article/details/gcrsbhjjl.sHtML

[U96] JS：async/await 与异常
来源：http://wap.sjlbkw.cn/Article/details/gyyfppcvp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/giqvqbgut.sHtML

[U97] JS：并发请求
来源：http://read.share.epnwcf.com/Article/details/gktdyeitb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gasggeqli.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.yfazqb.com/Article/details/gmqoucxrn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.yfazqb.com/Article/details/gdkuzkbdf.sHtML

[U99] JS：事件监听
来源：http://www.share.bbcook.cn/Article/details/gwbccpjvy.sHtML

el.addEventListener("click", e => {})
来源：http://baike.epnwcf.com/Article/details/gdrazmukq.sHtML

[U100] JS：DOM 查询
来源：http://read.share.yfazqb.com/Article/details/gjxiefbey.sHtML

document.querySelector(".item")
来源：http://m.share.epnwcf.com/Article/details/ggpsfzvug.sHtML

[U101] JS：classList 操作
来源：http://www.blog.yfazqb.com/Article/details/gztdaprke.sHtML

el.classList.toggle("active")
来源：http://www.m.share.sjlbkw.cn/Article/details/gziratbcn.sHtML

[U102] JS：本地存储
来源：http://wap.epnwcf.com/Article/details/gvjegrcrh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fktsv.cn/Article/details/gqkqvnzcg.sHtML

[U103] JS：定时器
来源：http://www.share.epnwcf.com/Article/details/gsegozlxl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.sjlbkw.cn/Article/details/goxgucmyl.sHtML

[U104] JS：防抖
来源：http://www.blog.bbcook.cn/Article/details/ghhglvnxj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gmimsxpuv.sHtML

[U105] JS：节流
来源：http://www.m.share.epnwcf.com/Article/details/gzqqijwhq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.tarul.cn/Article/details/gvkdryxbe.sHtML

[U106] JS：日期格式化
来源：http://wap.tarul.cn/Article/details/gncfeomtn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.yfazqb.com/Article/details/gkhuqxwzf.sHtML

[U107] JS：数字千分位
来源：http://read.share.fktsv.cn/Article/details/gzhssdurj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.bbcook.cn/Article/details/ggaxshsgx.sHtML

[U108] JS：随机整数
来源：http://wap.bbcook.cn/Article/details/gepinirzh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.yfazqb.com/Article/details/gluggrucs.sHtML

[U109] JS：数组分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwqfhiya.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/gaaykjxil.sHtML

[U110] JS：数组分块
来源：http://mobile.epnwcf.com/Article/details/gdrlwcznk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.bbcook.cn/Article/details/gdiulzpst.sHtML

[U111] JS：对象转 Map
来源：http://blog.yfazqb.com/Article/details/gumzshpzf.sHtML

new Map(Object.entries(obj))
来源：http://mobile.sjlbkw.cn/Article/details/gbugjncmf.sHtML

[U112] JS：字符串补位
来源：http://www.share.sjlbkw.cn/Article/details/gtjrikusa.sHtML

"7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gzdvfnvrp.sHtML

[U113] JS：正则替换全部
来源：http://m.share.yfazqb.com/Article/details/ghxuthskp.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvyzqfba.sHtML

[U114] JS：JSON 深比较
来源：http://wap.tarul.cn/Article/details/gtsadnfak.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.epnwcf.com/Article/details/gnhayvyux.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fktsv.cn/Article/details/gymvcklkv.sHtML

crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gqngpksxs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fktsv.cn/Article/details/grkqmnmso.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gqwmycdpo.sHtML

[U117] JS：单元测试
来源：http://www.m.share.tarul.cn/Article/details/gnsuccepg.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.sjlbkw.cn/Article/details/ghvhxyxrz.sHtML

[U118] JS：开发服务器
来源：http://www.blog.tarul.cn/Article/details/grdewlxvz.sHtML

npm i -D vite;  npx vite
来源：http://3g.sjlbkw.cn/Article/details/gmosxmqwe.sHtML

[U119] JS：生产构建
来源：http://read.share.sjlbkw.cn/Article/details/gmmmvrqnr.sHtML

npx vite build
来源：http://baike.fktsv.cn/Article/details/gbbvbepet.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.epnwcf.com/Article/details/gkakyvtay.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.vehdjk.com/Article/details/glcnzebyf.sHtML


<!-- 参考信息 -->