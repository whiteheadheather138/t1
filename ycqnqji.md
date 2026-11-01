代发 wailian999

[T33] Lua：表（数组）
来源：http://wap.sjlbkw.cn/Article/details/grwmahjme.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.tarul.cn/Article/details/gsijqjjvx.sHtML

[T34] Lua：遍历表
来源：http://wap.sjlbkw.cn/Article/details/grhopjhwz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.tarul.cn/Article/details/gsckxihwu.sHtML

[T35] Lua：字典表
来源：http://mobile.vehdjk.com/Article/details/gxcahybhs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fktsv.cn/Article/details/gqjrvwvpc.sHtML

[T36] Lua：函数
来源：http://www.blog.vehdjk.com/Article/details/gijydkphb.sHtML

function add(a, b) return a + b end
来源：http://mobile.epnwcf.com/Article/details/gldfvfxma.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/ghterwgme.sHtML

"a" .. "b"
来源：http://baike.yfazqb.com/Article/details/gogkxqhaw.sHtML

[T38] Lua：条件
来源：http://mobile.bbcook.cn/Article/details/gbgucjsbr.sHtML

if x > 0 then print("正") end
来源：http://mobile.sjlbkw.cn/Article/details/gccjpnmri.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fktsv.cn/Article/details/gfdjamjxm.sHtML

string.find(s, "%d+")
来源：http://read.share.vehdjk.com/Article/details/girvjusbi.sHtML

[T40] Lua：元表
来源：http://3g.sjlbkw.cn/Article/details/guxtjkdwn.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.epnwcf.com/Article/details/gkvgzgbvy.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gabwnyznt.sHtML

print "Hello\n";
来源：http://m.share.bbcook.cn/Article/details/gcqeryzrh.sHtML

[T42] Perl：变量类型
来源：http://wap.epnwcf.com/Article/details/guxsauaic.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpunzgzci.sHtML

[T43] Perl：字符串插值
来源：http://read.share.tarul.cn/Article/details/gdpyfroyh.sHtML

"值: $a"
来源：http://www.share.epnwcf.com/Article/details/gjyivedwf.sHtML

[T44] Perl：条件
来源：http://baike.bbcook.cn/Article/details/gyxgpulas.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fktsv.cn/Article/details/gellypyne.sHtML

[T45] Perl：数组遍历
来源：http://wap.tarul.cn/Article/details/gcrgctwsz.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.yfazqb.com/Article/details/ghqxlqixy.sHtML

[T46] Perl：哈希操作
来源：http://3g.epnwcf.com/Article/details/gcubudjfu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.tarul.cn/Article/details/gkkqfoqam.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fktsv.cn/Article/details/gcqsryesi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.tarul.cn/Article/details/gqfjhhbag.sHtML

[T48] Perl：正则替换
来源：http://m.share.tarul.cn/Article/details/gsvrbbgar.sHtML

$s =~ s/old/new/g;
来源：http://blog.vehdjk.com/Article/details/gasiypsuo.sHtML

[T49] Perl：函数
来源：http://www.m.share.bbcook.cn/Article/details/gzpchmrob.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gwqwzowdn.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.tarul.cn/Article/details/ghxwrlvml.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.epnwcf.com/Article/details/givydhuop.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.vehdjk.com/Article/details/gshvnpwhw.sHtML

[T51] Scala：Hello World
来源：http://wap.tarul.cn/Article/details/gwmcokcsr.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gupvsdyax.sHtML

[T52] Scala：变量
来源：http://m.share.bbcook.cn/Article/details/gcuuwgvwp.sHtML

val a = 1;  var b = 2
来源：http://www.blog.epnwcf.com/Article/details/gujkqetec.sHtML

[T53] Scala：字符串插值
来源：http://blog.vehdjk.com/Article/details/gendhafng.sHtML

s"值: $b"
来源：http://baike.tarul.cn/Article/details/gjqhfgyja.sHtML

[T54] Scala：集合映射
来源：http://mobile.yfazqb.com/Article/details/giuhklvgx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.bbcook.cn/Article/details/gtpmwignc.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/gsuasirhc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.tarul.cn/Article/details/grgecfnqf.sHtML

[T56] Scala：样例类
来源：http://mobile.vehdjk.com/Article/details/gkchqyslk.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnisyqxha.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/goffywfpt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.epnwcf.com/Article/details/gfpnrrvvl.sHtML

[T58] Scala：函数定义
来源：http://www.share.tarul.cn/Article/details/gvdtyxgjt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.epnwcf.com/Article/details/glhkbrtxw.sHtML

[T59] Scala：循环
来源：http://www.m.share.bbcook.cn/Article/details/gaxrqwmvn.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.tarul.cn/Article/details/gkqywaplr.sHtML

[T60] Scala：折叠
来源：http://m.share.fktsv.cn/Article/details/grphpmypb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.epnwcf.com/Article/details/gfufpzepq.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqtckxtai.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fktsv.cn/Article/details/gfyrgfoqk.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggcznybfb.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fktsv.cn/Article/details/govhssacu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.yfazqb.com/Article/details/gpojybino.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.vehdjk.com/Article/details/gystrjcwq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.sjlbkw.cn/Article/details/gvcynbxtp.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fktsv.cn/Article/details/gefdtyacq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.tarul.cn/Article/details/gsutlahpa.sHtML

[U04] Py：变量调试打印
来源：http://baike.sjlbkw.cn/Article/details/gecnjuimw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.sjlbkw.cn/Article/details/gdxmqmctg.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.yfazqb.com/Article/details/gialfbpkg.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gquctzcrz.sHtML

[U06] Py：合并两个字典
来源：http://baike.fktsv.cn/Article/details/gothjpsgd.sHtML

{**a, **b}
来源：http://wap.yfazqb.com/Article/details/gftqvquxk.sHtML

[U07] Py：反转字典键值
来源：http://blog.bbcook.cn/Article/details/glkhwrhfo.sHtML

{v: k for k, v in d.items()}
来源：http://baike.yfazqb.com/Article/details/gzdibbeoi.sHtML

[U08] Py：展平二维列表
来源：http://www.share.bbcook.cn/Article/details/gxitqgpxp.sHtML

[y for x in nested for y in x]
来源：http://www.share.yfazqb.com/Article/details/gwuoojedh.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.tarul.cn/Article/details/gvrhcnprr.sHtML

max(d, key=d.get)
来源：http://www.share.bbcook.cn/Article/details/gwiqvyidr.sHtML

[U10] Py：按值排序字典
来源：http://m.share.epnwcf.com/Article/details/gadgnnnhi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.yfazqb.com/Article/details/gdmohhvwx.sHtML

[U11] Py：生成器表达式
来源：http://wap.yfazqb.com/Article/details/gspymfact.sHtML

(x * 2 for x in arr)
来源：http://mobile.fktsv.cn/Article/details/gdsegegim.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.sjlbkw.cn/Article/details/gjwdhtwar.sHtML

Counter(arr).most_common(3)
来源：http://3g.bbcook.cn/Article/details/gsofkcwzz.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fktsv.cn/Article/details/gsvtoyziz.sHtML

deque(maxlen=10)
来源：http://m.share.vehdjk.com/Article/details/ggckpwyty.sHtML

[U14] Py：分组收集到列表
来源：http://baike.tarul.cn/Article/details/glchbillu.sHtML

defaultdict(list)
来源：http://wap.vehdjk.com/Article/details/gzkfkpgpb.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fktsv.cn/Article/details/gktjcappg.sHtML

t = time.perf_counter()
来源：http://blog.tarul.cn/Article/details/gmwtojrej.sHtML

[U16] Py：命令行参数解析
来源：http://wap.vehdjk.com/Article/details/grahpoiec.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.vehdjk.com/Article/details/gzgvyenvh.sHtML

[U17] Py：初始化日志
来源：http://mobile.yfazqb.com/Article/details/gmcvdupsh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.sjlbkw.cn/Article/details/grholinwx.sHtML

[U18] Py：预编译正则
来源：http://m.share.vehdjk.com/Article/details/gkkkkvfcx.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.tarul.cn/Article/details/grbqpwlbc.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.sjlbkw.cn/Article/details/glugonidt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.bbcook.cn/Article/details/gozxeakfj.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.bbcook.cn/Article/details/glddwxnoh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.sjlbkw.cn/Article/details/gfoznkznf.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.sjlbkw.cn/Article/details/gisdhvryj.sHtML

@contextlib.contextmanager
来源：http://wap.bbcook.cn/Article/details/gkyfoqyce.sHtML

[U22] Py：矩阵转置
来源：http://blog.sjlbkw.cn/Article/details/gmjvdawxx.sHtML

list(zip(*m))
来源：http://blog.tarul.cn/Article/details/guhccprtc.sHtML

[U23] Py：分块读取大文件
来源：http://baike.yfazqb.com/Article/details/geghphlmz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.yfazqb.com/Article/details/gaxdvxjug.sHtML

[U24] Py：路径操作
来源：http://mobile.tarul.cn/Article/details/gfxmpejce.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gxazufsnu.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.yfazqb.com/Article/details/gflsuhrie.sHtML

csv.DictReader(f)
来源：http://www.share.sjlbkw.cn/Article/details/gueisrdzw.sHtML

[U26] Py：并发下载
来源：http://m.share.sjlbkw.cn/Article/details/grbddsrvw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.sjlbkw.cn/Article/details/gbtfavkxr.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fktsv.cn/Article/details/gveczwsgb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.bbcook.cn/Article/details/guhjgdmvq.sHtML

[U28] Py：类型别名
来源：http://wap.bbcook.cn/Article/details/gmnsvbzet.sHtML

UserId = int
来源：http://3g.epnwcf.com/Article/details/gelvjamns.sHtML

[U29] Py：属性校验
来源：http://mobile.tarul.cn/Article/details/gckhasrkh.sHtML

@property 与 @x.setter 配合
来源：http://www.share.yfazqb.com/Article/details/galrzboch.sHtML

[U30] Py：数据类
来源：http://wap.vehdjk.com/Article/details/gfvnjrfkq.sHtML

@dataclass(slots=True)
来源：http://blog.epnwcf.com/Article/details/gxzhmaoeb.sHtML

[U31] Py：单测
来源：http://m.share.bbcook.cn/Article/details/gryygcurr.sHtML

python -m pytest -q
来源：http://wap.tarul.cn/Article/details/girngfuqs.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.yfazqb.com/Article/details/glimqyjvm.sHtML

ruff format . && ruff check --fix .
来源：http://3g.epnwcf.com/Article/details/gaxvitcms.sHtML

[U33] Py：打包发布
来源：http://www.share.vehdjk.com/Article/details/guvwualbl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.vehdjk.com/Article/details/gbtkkpkrt.sHtML

[U34] Py：判断编码
来源：http://wap.bbcook.cn/Article/details/gmlklvugx.sHtML

chardet.detect(raw)
来源：http://3g.tarul.cn/Article/details/gdcxnazls.sHtML

[U35] Py：发送邮件
来源：http://blog.vehdjk.com/Article/details/gzjmksfgu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.tarul.cn/Article/details/gdxdpqboi.sHtML

[U36] Py：定时任务
来源：http://wap.fktsv.cn/Article/details/gsgnvrsmg.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.sjlbkw.cn/Article/details/glbdwvgrl.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fktsv.cn/Article/details/glyneztns.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fktsv.cn/Article/details/gxkrjcsre.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.yfazqb.com/Article/details/gireluuta.sHtML

Path(__file__).resolve().parent
来源：http://read.share.yfazqb.com/Article/details/gzegpucbq.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.vehdjk.com/Article/details/grsozxcgr.sHtML

sys.stdout.isatty()
来源：http://www.m.share.tarul.cn/Article/details/gngkebmxa.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fktsv.cn/Article/details/gjhmkdvbf.sHtML

print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gupvfleig.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.epnwcf.com/Article/details/gzcnlmkmo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.bbcook.cn/Article/details/gsnvapxlc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.bbcook.cn/Article/details/gmrzzpnvm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.sjlbkw.cn/Article/details/grspxazvn.sHtML

[U43] PHP：声明命名空间
来源：http://blog.tarul.cn/Article/details/gmakyeqzh.sHtML

namespace App\Http;
来源：http://www.share.bbcook.cn/Article/details/ggpxpxfpg.sHtML

[U44] PHP：开启严格类型
来源：http://baike.sjlbkw.cn/Article/details/gpihntqlt.sHtML

declare(strict_types=1);
来源：http://blog.fktsv.cn/Article/details/gfdyzmmut.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.bbcook.cn/Article/details/gprxxomnt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gglynnmga.sHtML

[U46] PHP：可空类型
来源：http://www.share.epnwcf.com/Article/details/gopsrotop.sHtML

?string $name = null
来源：http://baike.epnwcf.com/Article/details/gnedwzdml.sHtML

[U47] PHP：联合类型
来源：http://read.share.vehdjk.com/Article/details/gdigdksav.sHtML

int|string $id
来源：http://m.share.tarul.cn/Article/details/glhmcring.sHtML

[U48] PHP：纯枚举
来源：http://m.share.epnwcf.com/Article/details/gpbgrqgce.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.vehdjk.com/Article/details/gjtfbzqmw.sHtML

[U49] PHP：只读属性
来源：http://blog.epnwcf.com/Article/details/gzpuiijtd.sHtML

public readonly string $name
来源：http://read.share.epnwcf.com/Article/details/gzdnuekvn.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fktsv.cn/Article/details/gtgaggwez.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.tarul.cn/Article/details/gfczqycra.sHtML

[U51] PHP：数组解构
来源：http://blog.bbcook.cn/Article/details/gcvrafujq.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fktsv.cn/Article/details/gxhaantin.sHtML

[U52] PHP：箭头函数
来源：http://wap.tarul.cn/Article/details/gtrbjbsuy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.yfazqb.com/Article/details/gvrmypyjz.sHtML

[U53] PHP：空合并运算符
来源：http://baike.vehdjk.com/Article/details/gxplnngwn.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.sjlbkw.cn/Article/details/gpozkmckk.sHtML

[U54] PHP：空安全调用
来源：http://wap.fktsv.cn/Article/details/gklsltwnm.sHtML

$obj?->method()
来源：http://baike.bbcook.cn/Article/details/gfhyprpbu.sHtML

[U55] PHP：match 表达式
来源：http://read.share.bbcook.cn/Article/details/gtfznjbih.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/gvammpzzh.sHtML

[U56] PHP：命名参数
来源：http://3g.tarul.cn/Article/details/gorltuwtp.sHtML

f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/goycbxnuq.sHtML

[U57] PHP：字符串插值
来源：http://baike.epnwcf.com/Article/details/gbhjenedk.sHtML

"值: {$a}"
来源：http://mobile.bbcook.cn/Article/details/gxbdmaovs.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.yfazqb.com/Article/details/gfzipflke.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.epnwcf.com/Article/details/gulyszydu.sHtML

[U59] PHP：自定义排序
来源：http://wap.fktsv.cn/Article/details/grmsgmmce.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.tarul.cn/Article/details/gmsfflvba.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.yfazqb.com/Article/details/gnlzqoloa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.sjlbkw.cn/Article/details/gnzszuznj.sHtML

[U61] PHP：正则
来源：http://baike.bbcook.cn/Article/details/gzcjdrkum.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gfegzzqfi.sHtML

[U62] PHP：日期对象
来源：http://baike.sjlbkw.cn/Article/details/gajmhhkaw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.bbcook.cn/Article/details/gfehtfslh.sHtML

[U63] PHP：文件读写
来源：http://baike.sjlbkw.cn/Article/details/gbcmtemsq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.tarul.cn/Article/details/gpmtiymmd.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.tarul.cn/Article/details/gdbijpthg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.epnwcf.com/Article/details/gqrtttgfc.sHtML

[U65] PHP：会话
来源：http://www.share.fktsv.cn/Article/details/glhvqivzr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gruhblpim.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.epnwcf.com/Article/details/gffkdmnxh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.tarul.cn/Article/details/glbuzywtr.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fktsv.cn/Article/details/gqlljsvln.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.yfazqb.com/Article/details/gbwsqbgpi.sHtML

[U68] PHP：PDO 连接
来源：http://wap.tarul.cn/Article/details/gkstrabbt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.yfazqb.com/Article/details/gdtygnrdj.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.vehdjk.com/Article/details/gsipsinfa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.sjlbkw.cn/Article/details/gvqgdpaam.sHtML

[U70] PHP：PDO 事务
来源：http://3g.sjlbkw.cn/Article/details/grtmklgek.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.epnwcf.com/Article/details/grfdbfnjc.sHtML

[U71] PHP：抛出异常
来源：http://www.share.tarul.cn/Article/details/gxlqyxkpj.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.vehdjk.com/Article/details/gmgnunfmo.sHtML

[U72] PHP：写错误日志
来源：http://3g.yfazqb.com/Article/details/glyuwrqbg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fktsv.cn/Article/details/gbhohdddu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.yfazqb.com/Article/details/gtfcjeuku.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmobtkfr.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvkcajjl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fktsv.cn/Article/details/gwkpnihto.sHtML

[U75] PHP：依赖注入
来源：http://m.share.yfazqb.com/Article/details/gmqhujdpb.sHtML

composer require psr/container
来源：http://wap.vehdjk.com/Article/details/gvgjhkcnv.sHtML

[U76] PHP：简单路由
来源：http://read.share.epnwcf.com/Article/details/gczhamnmz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.vehdjk.com/Article/details/gjkdpgljp.sHtML

[U77] PHP：模板渲染
来源：http://3g.bbcook.cn/Article/details/guuhtrazb.sHtML

composer require twig/twig
来源：http://www.m.share.epnwcf.com/Article/details/glxeczlwd.sHtML

[U78] PHP：单元测试
来源：http://mobile.sjlbkw.cn/Article/details/gecfojtrg.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.tarul.cn/Article/details/glppepwuw.sHtML

[U79] PHP：静态分析
来源：http://m.share.epnwcf.com/Article/details/gfetotoos.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.bbcook.cn/Article/details/gvhnwzyqy.sHtML

[U80] PHP：代码规范修复
来源：http://3g.sjlbkw.cn/Article/details/gomgwvzix.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.epnwcf.com/Article/details/gilkhwbtp.sHtML

[U81] JS：初始化项目
来源：http://m.share.vehdjk.com/Article/details/glwozrgob.sHtML

npm init -y;  npm i express
来源：http://m.share.fktsv.cn/Article/details/gyjcniuzx.sHtML

[U82] JS：package.json 脚本
来源：http://3g.yfazqb.com/Article/details/geyczywvk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.sjlbkw.cn/Article/details/gqlwckdaj.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.epnwcf.com/Article/details/grfhznxkp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/gnbkhxajd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.vehdjk.com/Article/details/gxwrmltxm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.bbcook.cn/Article/details/gcvcetypy.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/gfayimito.sHtML

a?.b?.c
来源：http://3g.epnwcf.com/Article/details/ggnlulpzy.sHtML

[U86] JS：空值合并
来源：http://m.share.bbcook.cn/Article/details/gkbckqwgu.sHtML

a ?? b
来源：http://baike.yfazqb.com/Article/details/ghzruchyq.sHtML

[U87] JS：解构默认值
来源：http://mobile.vehdjk.com/Article/details/gtncovhot.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.tarul.cn/Article/details/gqgxoxbyd.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.sjlbkw.cn/Article/details/groctgeof.sHtML

{ ...a, ...b }
来源：http://www.share.sjlbkw.cn/Article/details/gvifaqmgo.sHtML

[U89] JS：数组去重
来源：http://3g.sjlbkw.cn/Article/details/gafswrmwl.sHtML

[...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gkkqprqfu.sHtML

[U90] JS：数字数组排序
来源：http://www.share.vehdjk.com/Article/details/gfadwxrfw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gglfdicht.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.epnwcf.com/Article/details/gfnyzybio.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.vehdjk.com/Article/details/gmrhuahlq.sHtML

[U92] JS：深拷贝
来源：http://m.share.epnwcf.com/Article/details/glfgdfmfw.sHtML

structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gotsotqgi.sHtML

[U93] JS：模板字符串
来源：http://read.share.epnwcf.com/Article/details/gezedcjfd.sHtML

`共 ${n} 条`
来源：http://baike.vehdjk.com/Article/details/gidfswffx.sHtML

[U94] JS：箭头函数
来源：http://read.share.sjlbkw.cn/Article/details/gksryzrtq.sHtML

const double = x => x * 2;
来源：http://m.share.yfazqb.com/Article/details/gllglbpcm.sHtML

[U95] JS：Promise 包装
来源：http://wap.fktsv.cn/Article/details/gcuyxxntb.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.yfazqb.com/Article/details/geuosazhb.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.vehdjk.com/Article/details/ginfqmoca.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gloxgjdfc.sHtML

[U97] JS：并发请求
来源：http://blog.sjlbkw.cn/Article/details/gexnqfhvg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gdgkxmuea.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fktsv.cn/Article/details/gnmeeejbq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.yfazqb.com/Article/details/glhusgguf.sHtML

[U99] JS：事件监听
来源：http://blog.vehdjk.com/Article/details/gcjxckbin.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gciiyxiak.sHtML

[U100] JS：DOM 查询
来源：http://blog.bbcook.cn/Article/details/gxktdxpeg.sHtML

document.querySelector(".item")
来源：http://wap.tarul.cn/Article/details/glwzmgzma.sHtML

[U101] JS：classList 操作
来源：http://baike.epnwcf.com/Article/details/gxwmyxkvd.sHtML

el.classList.toggle("active")
来源：http://www.m.share.epnwcf.com/Article/details/gfxxmevai.sHtML

[U102] JS：本地存储
来源：http://mobile.yfazqb.com/Article/details/gurmkuidj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.yfazqb.com/Article/details/gmhmpvohm.sHtML

[U103] JS：定时器
来源：http://www.blog.tarul.cn/Article/details/gvimoahsm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.yfazqb.com/Article/details/gmrakvhst.sHtML

[U104] JS：防抖
来源：http://www.share.fktsv.cn/Article/details/gwzjdcjsn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gicswlhdq.sHtML

[U105] JS：节流
来源：http://read.share.vehdjk.com/Article/details/glmkzmsov.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.vehdjk.com/Article/details/gxfcjplkj.sHtML

[U106] JS：日期格式化
来源：http://3g.tarul.cn/Article/details/gkswamfrc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.vehdjk.com/Article/details/gdfkzfnxz.sHtML

[U107] JS：数字千分位
来源：http://www.share.yfazqb.com/Article/details/gctuqcqty.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.vehdjk.com/Article/details/geynpirnj.sHtML

[U108] JS：随机整数
来源：http://www.blog.yfazqb.com/Article/details/gtbnrvequ.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.epnwcf.com/Article/details/gzxpvoscz.sHtML

[U109] JS：数组分组
来源：http://read.share.tarul.cn/Article/details/gaflceicy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/giuqsxbaa.sHtML

[U110] JS：数组分块
来源：http://www.share.vehdjk.com/Article/details/gmizzajzr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.yfazqb.com/Article/details/ggayolgdp.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fktsv.cn/Article/details/gemrsngtc.sHtML

new Map(Object.entries(obj))
来源：http://mobile.yfazqb.com/Article/details/gniqtqkwp.sHtML

[U112] JS：字符串补位
来源：http://blog.vehdjk.com/Article/details/gwkbdghgj.sHtML

"7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/gjfodpnlz.sHtML

[U113] JS：正则替换全部
来源：http://m.share.vehdjk.com/Article/details/gxaydgpzd.sHtML

s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gibmamczy.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.yfazqb.com/Article/details/gtrckybod.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gfskwxdhp.sHtML

[U115] JS：生成 UUID
来源：http://read.share.epnwcf.com/Article/details/gpggkpuid.sHtML

crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gluvzripd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.yfazqb.com/Article/details/gzhjpyope.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.epnwcf.com/Article/details/gjucfnucz.sHtML

[U117] JS：单元测试
来源：http://www.m.share.epnwcf.com/Article/details/gpuvksxyn.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.sjlbkw.cn/Article/details/gwfsreehb.sHtML

[U118] JS：开发服务器
来源：http://www.share.epnwcf.com/Article/details/gtxcghmvu.sHtML

npm i -D vite;  npx vite
来源：http://wap.fktsv.cn/Article/details/gbgiwenbh.sHtML

[U119] JS：生产构建
来源：http://wap.tarul.cn/Article/details/ggjusggss.sHtML

npx vite build
来源：http://wap.epnwcf.com/Article/details/gfacpyyys.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.sjlbkw.cn/Article/details/gjhoihlmm.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.epnwcf.com/Article/details/gqltketpe.sHtML


<!-- 参考信息 -->