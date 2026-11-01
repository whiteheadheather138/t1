代发 wailian999

[T33] Lua：表（数组）
来源：http://3g.fktsv.cn/Article/details/gjgyjaddt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.sjlbkw.cn/Article/details/gtovzzohn.sHtML

[T34] Lua：遍历表
来源：http://3g.tarul.cn/Article/details/govoezcly.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.epnwcf.com/Article/details/gjqmzezjw.sHtML

[T35] Lua：字典表
来源：http://www.m.share.bbcook.cn/Article/details/gdsujwovy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gfjhubpik.sHtML

[T36] Lua：函数
来源：http://www.m.share.fktsv.cn/Article/details/gvfzkiwot.sHtML

function add(a, b) return a + b end
来源：http://3g.sjlbkw.cn/Article/details/gmcerinyc.sHtML

[T37] Lua：字符串拼接
来源：http://wap.tarul.cn/Article/details/gpterrqrl.sHtML

"a" .. "b"
来源：http://mobile.tarul.cn/Article/details/gehzryjrq.sHtML

[T38] Lua：条件
来源：http://www.share.fktsv.cn/Article/details/gaiefejmk.sHtML

if x > 0 then print("正") end
来源：http://baike.sjlbkw.cn/Article/details/grvyftxlg.sHtML

[T39] Lua：模式匹配
来源：http://read.share.bbcook.cn/Article/details/gscqrmfwb.sHtML

string.find(s, "%d+")
来源：http://baike.epnwcf.com/Article/details/glochdixb.sHtML

[T40] Lua：元表
来源：http://blog.yfazqb.com/Article/details/goittodnk.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.epnwcf.com/Article/details/gspwnomah.sHtML

[T41] Perl：Hello World
来源：http://mobile.fktsv.cn/Article/details/grfpkrxgm.sHtML

print "Hello\n";
来源：http://blog.tarul.cn/Article/details/gulfrtbyy.sHtML

[T42] Perl：变量类型
来源：http://mobile.fktsv.cn/Article/details/glkkclmoj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.vehdjk.com/Article/details/gsrnnfixs.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fktsv.cn/Article/details/goatzkase.sHtML

"值: $a"
来源：http://www.m.share.vehdjk.com/Article/details/gmzmftmwu.sHtML

[T44] Perl：条件
来源：http://3g.yfazqb.com/Article/details/goeapregz.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.tarul.cn/Article/details/gpvgainqs.sHtML

[T45] Perl：数组遍历
来源：http://blog.fktsv.cn/Article/details/gawyqjbsr.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.tarul.cn/Article/details/gkjjylnwd.sHtML

[T46] Perl：哈希操作
来源：http://baike.yfazqb.com/Article/details/gvpsqgtos.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.yfazqb.com/Article/details/gbgqxtxks.sHtML

[T47] Perl：正则捕获
来源：http://blog.tarul.cn/Article/details/ghghhheui.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.bbcook.cn/Article/details/gywymejtg.sHtML

[T48] Perl：正则替换
来源：http://3g.fktsv.cn/Article/details/gtidfuvgm.sHtML

$s =~ s/old/new/g;
来源：http://read.share.yfazqb.com/Article/details/grdwzxaxv.sHtML

[T49] Perl：函数
来源：http://m.share.bbcook.cn/Article/details/gmyaxpxbd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gfqhzpfyi.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gdduqakpb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.bbcook.cn/Article/details/ghciwgmru.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.tarul.cn/Article/details/gevomsjgs.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gcttzqoja.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/geskalpym.sHtML

[T52] Scala：变量
来源：http://www.share.yfazqb.com/Article/details/ggdqtumxu.sHtML

val a = 1;  var b = 2
来源：http://blog.tarul.cn/Article/details/golcdaigd.sHtML

[T53] Scala：字符串插值
来源：http://3g.fktsv.cn/Article/details/gcawqslvl.sHtML

s"值: $b"
来源：http://read.share.vehdjk.com/Article/details/gffwqfmmt.sHtML

[T54] Scala：集合映射
来源：http://blog.fktsv.cn/Article/details/gjnlzuqfb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.epnwcf.com/Article/details/goljmbxar.sHtML

[T55] Scala：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/gnzozcqpd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.epnwcf.com/Article/details/gdewbkivc.sHtML

[T56] Scala：样例类
来源：http://blog.yfazqb.com/Article/details/gcxxowjys.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.tarul.cn/Article/details/gcnfkbmof.sHtML

[T57] Scala：模式匹配
来源：http://mobile.epnwcf.com/Article/details/gpugbrcxt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.vehdjk.com/Article/details/gzmsqacqn.sHtML

[T58] Scala：函数定义
来源：http://read.share.tarul.cn/Article/details/gpnnszpsi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fktsv.cn/Article/details/gunrajgvk.sHtML

[T59] Scala：循环
来源：http://read.share.fktsv.cn/Article/details/ggjhurrdm.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fktsv.cn/Article/details/gcchedfth.sHtML

[T60] Scala：折叠
来源：http://m.share.yfazqb.com/Article/details/gqrjigqlx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.bbcook.cn/Article/details/gdveeikza.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gxqtvrgfo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/gqprlgcjs.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdmzmtmfe.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.yfazqb.com/Article/details/gvqrzikey.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.epnwcf.com/Article/details/gsyknnvbf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.tarul.cn/Article/details/gykrgpmjd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.yfazqb.com/Article/details/germxewxv.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.tarul.cn/Article/details/glbwwsndp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.sjlbkw.cn/Article/details/guvlogray.sHtML

[U04] Py：变量调试打印
来源：http://read.share.vehdjk.com/Article/details/gxprunqvm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fktsv.cn/Article/details/gfevzntvy.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkwzjoow.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gzufyzfqc.sHtML

[U06] Py：合并两个字典
来源：http://wap.fktsv.cn/Article/details/gyiaafgae.sHtML

{**a, **b}
来源：http://read.share.tarul.cn/Article/details/ggdnaujpv.sHtML

[U07] Py：反转字典键值
来源：http://m.share.tarul.cn/Article/details/gcixpfblw.sHtML

{v: k for k, v in d.items()}
来源：http://blog.yfazqb.com/Article/details/gfsexwaxg.sHtML

[U08] Py：展平二维列表
来源：http://mobile.epnwcf.com/Article/details/glgjcoojm.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/gaxzuwinr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.sjlbkw.cn/Article/details/gzqiqymih.sHtML

max(d, key=d.get)
来源：http://mobile.epnwcf.com/Article/details/gpqahfpvb.sHtML

[U10] Py：按值排序字典
来源：http://wap.vehdjk.com/Article/details/gyslcnist.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.yfazqb.com/Article/details/gzjqcdqdw.sHtML

[U11] Py：生成器表达式
来源：http://blog.sjlbkw.cn/Article/details/gflypufet.sHtML

(x * 2 for x in arr)
来源：http://baike.epnwcf.com/Article/details/gfuihzwmf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/gnhgixayw.sHtML

Counter(arr).most_common(3)
来源：http://wap.epnwcf.com/Article/details/gbtvwfaaa.sHtML

[U13] Py：固定长度队列
来源：http://mobile.tarul.cn/Article/details/gdpqfunkp.sHtML

deque(maxlen=10)
来源：http://www.m.share.tarul.cn/Article/details/ggpfibpxf.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fktsv.cn/Article/details/gzbpusrzo.sHtML

defaultdict(list)
来源：http://www.blog.tarul.cn/Article/details/gqomljjyd.sHtML

[U15] Py：高精度计时
来源：http://baike.tarul.cn/Article/details/gkuuyzlnr.sHtML

t = time.perf_counter()
来源：http://wap.yfazqb.com/Article/details/gkwplzvzi.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.epnwcf.com/Article/details/gehxarsxc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fktsv.cn/Article/details/gdqviyrxh.sHtML

[U17] Py：初始化日志
来源：http://read.share.vehdjk.com/Article/details/gefwmxhit.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.tarul.cn/Article/details/gfnvgdgow.sHtML

[U18] Py：预编译正则
来源：http://www.blog.epnwcf.com/Article/details/gbbgbvfnb.sHtML

pat = re.compile(r"\d+")
来源：http://baike.bbcook.cn/Article/details/gkgtthxsx.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.epnwcf.com/Article/details/gllfjhzss.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.tarul.cn/Article/details/gzjjibfvv.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.epnwcf.com/Article/details/gtxbrxptr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.bbcook.cn/Article/details/gdhushaze.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.yfazqb.com/Article/details/gwnltbhfc.sHtML

@contextlib.contextmanager
来源：http://mobile.bbcook.cn/Article/details/gqbvdbqmm.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fktsv.cn/Article/details/gwpkiagwn.sHtML

list(zip(*m))
来源：http://baike.sjlbkw.cn/Article/details/gqxjhzvrc.sHtML

[U23] Py：分块读取大文件
来源：http://wap.epnwcf.com/Article/details/glqarvhnr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.sjlbkw.cn/Article/details/gmsbiiqeo.sHtML

[U24] Py：路径操作
来源：http://3g.vehdjk.com/Article/details/gsqqsbzyq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gdetxfybk.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.yfazqb.com/Article/details/gaobnpxuc.sHtML

csv.DictReader(f)
来源：http://www.m.share.epnwcf.com/Article/details/glsfsmfue.sHtML

[U26] Py：并发下载
来源：http://blog.vehdjk.com/Article/details/guvwbfdzz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.bbcook.cn/Article/details/gwsrryasj.sHtML

[U27] Py：异步 HTTP
来源：http://blog.sjlbkw.cn/Article/details/gsbkouujv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.yfazqb.com/Article/details/gjvknfqyd.sHtML

[U28] Py：类型别名
来源：http://read.share.tarul.cn/Article/details/gnruiklvy.sHtML

UserId = int
来源：http://read.share.tarul.cn/Article/details/gbnrvkbdg.sHtML

[U29] Py：属性校验
来源：http://www.blog.epnwcf.com/Article/details/gwibqomgv.sHtML

@property 与 @x.setter 配合
来源：http://www.share.bbcook.cn/Article/details/gbcaohcpt.sHtML

[U30] Py：数据类
来源：http://m.share.epnwcf.com/Article/details/gbvkivbff.sHtML

@dataclass(slots=True)
来源：http://mobile.epnwcf.com/Article/details/gfthhaejg.sHtML

[U31] Py：单测
来源：http://m.share.vehdjk.com/Article/details/gviwfvjoc.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/gddbjucjq.sHtML

[U32] Py：代码格式化
来源：http://3g.sjlbkw.cn/Article/details/ggqaosplk.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.epnwcf.com/Article/details/gqppipdfl.sHtML

[U33] Py：打包发布
来源：http://wap.sjlbkw.cn/Article/details/gyeokvlmx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.vehdjk.com/Article/details/ggmrbtdit.sHtML

[U34] Py：判断编码
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoloozot.sHtML

chardet.detect(raw)
来源：http://wap.sjlbkw.cn/Article/details/goduezzqb.sHtML

[U35] Py：发送邮件
来源：http://3g.tarul.cn/Article/details/gfldcbzcn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fktsv.cn/Article/details/gypqcexcz.sHtML

[U36] Py：定时任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxhrgdrp.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.sjlbkw.cn/Article/details/gkblcjpsc.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fktsv.cn/Article/details/gbugjzhde.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.epnwcf.com/Article/details/gkaxjaxsd.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.vehdjk.com/Article/details/guqaktjry.sHtML

Path(__file__).resolve().parent
来源：http://3g.fktsv.cn/Article/details/gqxmunmne.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.vehdjk.com/Article/details/gmywmumhp.sHtML

sys.stdout.isatty()
来源：http://www.blog.vehdjk.com/Article/details/gpjqziyyd.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.vehdjk.com/Article/details/glzxkpktu.sHtML

print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gzexhcecg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.yfazqb.com/Article/details/gbzjwwhqg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.tarul.cn/Article/details/ghyoasmql.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.sjlbkw.cn/Article/details/gzsutggwb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.tarul.cn/Article/details/gqshdoqgl.sHtML

[U43] PHP：声明命名空间
来源：http://wap.sjlbkw.cn/Article/details/gzdtvsdke.sHtML

namespace App\Http;
来源：http://3g.sjlbkw.cn/Article/details/gcfbbirhp.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.yfazqb.com/Article/details/gjvjdpqhi.sHtML

declare(strict_types=1);
来源：http://read.share.yfazqb.com/Article/details/gdhqqyraj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.tarul.cn/Article/details/gfyvuzalp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gmfxfifvn.sHtML

[U46] PHP：可空类型
来源：http://blog.sjlbkw.cn/Article/details/gjqmsfrnn.sHtML

?string $name = null
来源：http://wap.yfazqb.com/Article/details/guidrgouq.sHtML

[U47] PHP：联合类型
来源：http://m.share.bbcook.cn/Article/details/ggewjpiga.sHtML

int|string $id
来源：http://read.share.fktsv.cn/Article/details/guusrwnzu.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fktsv.cn/Article/details/glfklqfiq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.sjlbkw.cn/Article/details/gbdyhjpga.sHtML

[U49] PHP：只读属性
来源：http://m.share.fktsv.cn/Article/details/gkdxkzxnb.sHtML

public readonly string $name
来源：http://mobile.tarul.cn/Article/details/gjbsjncva.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.vehdjk.com/Article/details/gzqdjpyqx.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvvgqhhv.sHtML

[U51] PHP：数组解构
来源：http://m.share.bbcook.cn/Article/details/gfomiaxpb.sHtML

[$a, $b] = $arr;
来源：http://www.share.tarul.cn/Article/details/guehqykop.sHtML

[U52] PHP：箭头函数
来源：http://baike.bbcook.cn/Article/details/gefntcjpl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdmpyjmd.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fktsv.cn/Article/details/gxleimren.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.sjlbkw.cn/Article/details/gdvijjdjr.sHtML

[U54] PHP：空安全调用
来源：http://m.share.tarul.cn/Article/details/gsdylktth.sHtML

$obj?->method()
来源：http://m.share.tarul.cn/Article/details/giprnixro.sHtML

[U55] PHP：match 表达式
来源：http://blog.fktsv.cn/Article/details/glcckxjls.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.vehdjk.com/Article/details/gmejccyux.sHtML

[U56] PHP：命名参数
来源：http://read.share.sjlbkw.cn/Article/details/gnfogpxpz.sHtML

f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gxzunaqad.sHtML

[U57] PHP：字符串插值
来源：http://blog.yfazqb.com/Article/details/ghncgaxwz.sHtML

"值: {$a}"
来源：http://mobile.epnwcf.com/Article/details/gekppawki.sHtML

[U58] PHP：数组三件套
来源：http://baike.sjlbkw.cn/Article/details/gwztfdjkq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.bbcook.cn/Article/details/gaeeisxmv.sHtML

[U59] PHP：自定义排序
来源：http://wap.yfazqb.com/Article/details/gsgbsrqxx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/gkyxlbqsu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.bbcook.cn/Article/details/gomhrizyb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.sjlbkw.cn/Article/details/gizuvcrqq.sHtML

[U61] PHP：正则
来源：http://3g.sjlbkw.cn/Article/details/gskotdsdb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gsgcqxoab.sHtML

[U62] PHP：日期对象
来源：http://wap.tarul.cn/Article/details/gqtxfpguj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.epnwcf.com/Article/details/gvfjhihcd.sHtML

[U63] PHP：文件读写
来源：http://read.share.bbcook.cn/Article/details/gogqpvgdz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fktsv.cn/Article/details/ghsydhpbb.sHtML

[U64] PHP：目录遍历
来源：http://mobile.yfazqb.com/Article/details/gzivpljug.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.yfazqb.com/Article/details/gueftkuxl.sHtML

[U65] PHP：会话
来源：http://m.share.sjlbkw.cn/Article/details/gknqmtabt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gtfzqmmuh.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.bbcook.cn/Article/details/gtutiixua.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.epnwcf.com/Article/details/gjdvbcygk.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.epnwcf.com/Article/details/gihpziqrg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.yfazqb.com/Article/details/gwzdxwqyq.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.vehdjk.com/Article/details/gevzzmlvf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.vehdjk.com/Article/details/gijopwwju.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.sjlbkw.cn/Article/details/glwtekmzx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fktsv.cn/Article/details/gpsqsxtdb.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.vehdjk.com/Article/details/glmoekrig.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.bbcook.cn/Article/details/gvehoiymh.sHtML

[U71] PHP：抛出异常
来源：http://www.share.tarul.cn/Article/details/gaornfcxz.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.sjlbkw.cn/Article/details/gfprvtaxu.sHtML

[U72] PHP：写错误日志
来源：http://3g.yfazqb.com/Article/details/ghxilxdph.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.bbcook.cn/Article/details/gwldhherk.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.sjlbkw.cn/Article/details/gluubqvbu.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.bbcook.cn/Article/details/gztwhplql.sHtML

[U74] PHP：读取环境变量
来源：http://wap.yfazqb.com/Article/details/ghznqncqb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.tarul.cn/Article/details/gjexwbhja.sHtML

[U75] PHP：依赖注入
来源：http://m.share.vehdjk.com/Article/details/giodvdyrv.sHtML

composer require psr/container
来源：http://blog.fktsv.cn/Article/details/godjatkek.sHtML

[U76] PHP：简单路由
来源：http://blog.epnwcf.com/Article/details/gedqnumci.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.bbcook.cn/Article/details/ghnlvkhlc.sHtML

[U77] PHP：模板渲染
来源：http://www.share.tarul.cn/Article/details/gzeybuxjk.sHtML

composer require twig/twig
来源：http://baike.sjlbkw.cn/Article/details/grsstggwz.sHtML

[U78] PHP：单元测试
来源：http://baike.yfazqb.com/Article/details/gzxpqnavo.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.epnwcf.com/Article/details/ghjsiygmm.sHtML

[U79] PHP：静态分析
来源：http://m.share.bbcook.cn/Article/details/gcfcwwyjl.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.bbcook.cn/Article/details/gimccbpdq.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.epnwcf.com/Article/details/gduvoeixi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.sjlbkw.cn/Article/details/gfzbbrmbw.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.yfazqb.com/Article/details/gzpikmqur.sHtML

npm init -y;  npm i express
来源：http://3g.epnwcf.com/Article/details/gtljdmtji.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.sjlbkw.cn/Article/details/gcmkfrjxa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.epnwcf.com/Article/details/gwxqubhys.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.yfazqb.com/Article/details/gzlfbgbvo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/gyfazeutx.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.bbcook.cn/Article/details/gxapeabwd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.bbcook.cn/Article/details/gquxmioeq.sHtML

[U85] JS：可选链
来源：http://blog.yfazqb.com/Article/details/guzwzgzfo.sHtML

a?.b?.c
来源：http://blog.vehdjk.com/Article/details/gmhdrgvki.sHtML

[U86] JS：空值合并
来源：http://mobile.bbcook.cn/Article/details/geaftgzlo.sHtML

a ?? b
来源：http://mobile.sjlbkw.cn/Article/details/gjsjoavtq.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.yfazqb.com/Article/details/gnslmtyae.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.tarul.cn/Article/details/gnllnxmrj.sHtML

[U88] JS：对象展开合并
来源：http://read.share.vehdjk.com/Article/details/glwqidwmi.sHtML

{ ...a, ...b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdygvxrew.sHtML

[U89] JS：数组去重
来源：http://baike.sjlbkw.cn/Article/details/grzftwnys.sHtML

[...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gdxqarmdg.sHtML

[U90] JS：数字数组排序
来源：http://www.share.yfazqb.com/Article/details/gctpgolik.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gkojjjbvm.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.yfazqb.com/Article/details/gzcspbrfg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.yfazqb.com/Article/details/gjbonujct.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gmganrsmi.sHtML

structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gzwsbqpqo.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.vehdjk.com/Article/details/grqaqfbyg.sHtML

`共 ${n} 条`
来源：http://www.blog.sjlbkw.cn/Article/details/gmlhawfir.sHtML

[U94] JS：箭头函数
来源：http://blog.bbcook.cn/Article/details/gtltzuomu.sHtML

const double = x => x * 2;
来源：http://blog.vehdjk.com/Article/details/gvtovzsng.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.epnwcf.com/Article/details/gltmvmpvk.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.vehdjk.com/Article/details/gbihmlenc.sHtML

[U96] JS：async/await 与异常
来源：http://wap.epnwcf.com/Article/details/gxpemjvdo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gghtuvkgc.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fktsv.cn/Article/details/gjbdkunku.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gwavdhqfw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.tarul.cn/Article/details/geaawftnj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fktsv.cn/Article/details/gvlyzfbsm.sHtML

[U99] JS：事件监听
来源：http://read.share.vehdjk.com/Article/details/gvhyelond.sHtML

el.addEventListener("click", e => {})
来源：http://wap.vehdjk.com/Article/details/gmrnqipin.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.epnwcf.com/Article/details/gcbjrijem.sHtML

document.querySelector(".item")
来源：http://blog.sjlbkw.cn/Article/details/gxnkptuab.sHtML

[U101] JS：classList 操作
来源：http://mobile.vehdjk.com/Article/details/gmchvsqvv.sHtML

el.classList.toggle("active")
来源：http://wap.vehdjk.com/Article/details/gtfuotbse.sHtML

[U102] JS：本地存储
来源：http://wap.fktsv.cn/Article/details/gbhlzyupw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.epnwcf.com/Article/details/gnjiymwnr.sHtML

[U103] JS：定时器
来源：http://www.m.share.tarul.cn/Article/details/gftqwrcap.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.vehdjk.com/Article/details/gcbbgtiup.sHtML

[U104] JS：防抖
来源：http://blog.epnwcf.com/Article/details/gpnlybdjw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gucvsgnoz.sHtML

[U105] JS：节流
来源：http://baike.tarul.cn/Article/details/gzpgolqpj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gsegthirz.sHtML

[U106] JS：日期格式化
来源：http://read.share.vehdjk.com/Article/details/gjcomxhcr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fktsv.cn/Article/details/gihpumpki.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.vehdjk.com/Article/details/grzdvgyfa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.bbcook.cn/Article/details/gbtluvntn.sHtML

[U108] JS：随机整数
来源：http://3g.epnwcf.com/Article/details/gmjqkugem.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.sjlbkw.cn/Article/details/grquedvlp.sHtML

[U109] JS：数组分组
来源：http://3g.vehdjk.com/Article/details/gbzytzwni.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gspcpltnb.sHtML

[U110] JS：数组分块
来源：http://www.blog.tarul.cn/Article/details/gperztzud.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.vehdjk.com/Article/details/gsrgzvnvh.sHtML

[U111] JS：对象转 Map
来源：http://read.share.bbcook.cn/Article/details/gooreatdb.sHtML

new Map(Object.entries(obj))
来源：http://read.share.vehdjk.com/Article/details/gjewzeqno.sHtML

[U112] JS：字符串补位
来源：http://3g.fktsv.cn/Article/details/grutnjqbr.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gziixqupz.sHtML

[U113] JS：正则替换全部
来源：http://read.share.bbcook.cn/Article/details/gkfgkhwvd.sHtML

s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/ghemaeqvg.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.epnwcf.com/Article/details/gokygvhto.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.vehdjk.com/Article/details/gscksskzi.sHtML

[U115] JS：生成 UUID
来源：http://read.share.yfazqb.com/Article/details/goxjyfhxc.sHtML

crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gvgyuzhcs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.sjlbkw.cn/Article/details/gakltxhqm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.yfazqb.com/Article/details/gubfinqbt.sHtML

[U117] JS：单元测试
来源：http://3g.vehdjk.com/Article/details/gjdzclkhj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.sjlbkw.cn/Article/details/glmgvgzdp.sHtML

[U118] JS：开发服务器
来源：http://read.share.bbcook.cn/Article/details/goettrlxg.sHtML

npm i -D vite;  npx vite
来源：http://wap.tarul.cn/Article/details/gttgfnwzd.sHtML

[U119] JS：生产构建
来源：http://m.share.bbcook.cn/Article/details/gmjmkryou.sHtML

npx vite build
来源：http://3g.bbcook.cn/Article/details/gmccnfxzh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.bbcook.cn/Article/details/gerzbaslq.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.vehdjk.com/Article/details/gculeygkw.sHtML


<!-- 参考信息 -->