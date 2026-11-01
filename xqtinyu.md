代发 wailian999

[T33] Lua：表（数组）
来源：http://3g.yfazqb.com/Article/details/gpjwsewtq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.yfazqb.com/Article/details/gtwbujjpg.sHtML

[T34] Lua：遍历表
来源：http://baike.fktsv.cn/Article/details/gxnedlsqi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.epnwcf.com/Article/details/goxgcpaiw.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/gmxdyswfs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fktsv.cn/Article/details/gjoglqowc.sHtML

[T36] Lua：函数
来源：http://mobile.bbcook.cn/Article/details/gksrctryn.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fktsv.cn/Article/details/gcpyludkv.sHtML

[T37] Lua：字符串拼接
来源：http://3g.yfazqb.com/Article/details/gqtntmkkg.sHtML

"a" .. "b"
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrroggzn.sHtML

[T38] Lua：条件
来源：http://wap.sjlbkw.cn/Article/details/gmlyvytxl.sHtML

if x > 0 then print("正") end
来源：http://wap.epnwcf.com/Article/details/gzliwktrx.sHtML

[T39] Lua：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gyiiirnqy.sHtML

string.find(s, "%d+")
来源：http://read.share.yfazqb.com/Article/details/gjqwxdewj.sHtML

[T40] Lua：元表
来源：http://wap.fktsv.cn/Article/details/gqxafdktd.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.vehdjk.com/Article/details/gqrjlgmkd.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gqvcjytly.sHtML

print "Hello\n";
来源：http://baike.vehdjk.com/Article/details/gjzalelzg.sHtML

[T42] Perl：变量类型
来源：http://baike.epnwcf.com/Article/details/gdxfdubri.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.sjlbkw.cn/Article/details/gqlpxhcgr.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/glpcnfxzd.sHtML

"值: $a"
来源：http://mobile.fktsv.cn/Article/details/gjcpeesnt.sHtML

[T44] Perl：条件
来源：http://blog.bbcook.cn/Article/details/glfhrefmw.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.vehdjk.com/Article/details/gmsnrszar.sHtML

[T45] Perl：数组遍历
来源：http://read.share.epnwcf.com/Article/details/guktyhrwe.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.vehdjk.com/Article/details/gwhmclaav.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.tarul.cn/Article/details/gyixhjyoq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.bbcook.cn/Article/details/glkyhmhdc.sHtML

[T47] Perl：正则捕获
来源：http://mobile.bbcook.cn/Article/details/gocttjxlq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.vehdjk.com/Article/details/gszngeizy.sHtML

[T48] Perl：正则替换
来源：http://blog.tarul.cn/Article/details/gqxinzycy.sHtML

$s =~ s/old/new/g;
来源：http://baike.tarul.cn/Article/details/gsralxjpl.sHtML

[T49] Perl：函数
来源：http://3g.bbcook.cn/Article/details/gcruklrph.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gzorjdgns.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gvnkrebek.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.bbcook.cn/Article/details/gespwroqn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.epnwcf.com/Article/details/goyhzpeyl.sHtML

[T51] Scala：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gwgrigwnn.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/ghjphnqnr.sHtML

[T52] Scala：变量
来源：http://read.share.tarul.cn/Article/details/ghstujilz.sHtML

val a = 1;  var b = 2
来源：http://www.share.yfazqb.com/Article/details/goprrsfsl.sHtML

[T53] Scala：字符串插值
来源：http://baike.yfazqb.com/Article/details/gdvzyroqi.sHtML

s"值: $b"
来源：http://www.share.tarul.cn/Article/details/gdhnuktse.sHtML

[T54] Scala：集合映射
来源：http://www.share.epnwcf.com/Article/details/gjfyudijz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.bbcook.cn/Article/details/gavkwfxxw.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gfozegxlr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fktsv.cn/Article/details/gaprowwwn.sHtML

[T56] Scala：样例类
来源：http://wap.bbcook.cn/Article/details/gjnvptypb.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcdtpmiz.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fktsv.cn/Article/details/gpdjfksyn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.bbcook.cn/Article/details/ggqvvqcvn.sHtML

[T58] Scala：函数定义
来源：http://blog.epnwcf.com/Article/details/gfsqsegdz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.sjlbkw.cn/Article/details/gmxhlzmmf.sHtML

[T59] Scala：循环
来源：http://mobile.tarul.cn/Article/details/gzqgctblf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gpazbrckf.sHtML

[T60] Scala：折叠
来源：http://baike.sjlbkw.cn/Article/details/gpkiimnkb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.bbcook.cn/Article/details/grjiduzzk.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxxrboqck.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.bbcook.cn/Article/details/gfuvvanyn.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gifmovzkc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fktsv.cn/Article/details/gddpcitda.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.sjlbkw.cn/Article/details/gdnkusahf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.vehdjk.com/Article/details/gbgwukmzl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.epnwcf.com/Article/details/ggwxuibpf.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fktsv.cn/Article/details/geyksuozc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.tarul.cn/Article/details/gtqfvbmud.sHtML

[U04] Py：变量调试打印
来源：http://baike.bbcook.cn/Article/details/gsihucvcr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.vehdjk.com/Article/details/gumjjidnq.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.bbcook.cn/Article/details/gizgaqauk.sHtML

list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/ghezzmtxg.sHtML

[U06] Py：合并两个字典
来源：http://mobile.yfazqb.com/Article/details/gojagfzmq.sHtML

{**a, **b}
来源：http://wap.bbcook.cn/Article/details/gnjabkuho.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fktsv.cn/Article/details/gkmasquxf.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fktsv.cn/Article/details/guqhekglw.sHtML

[U08] Py：展平二维列表
来源：http://wap.bbcook.cn/Article/details/gunvuzdja.sHtML

[y for x in nested for y in x]
来源：http://read.share.epnwcf.com/Article/details/gqjanufyz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.sjlbkw.cn/Article/details/gstbwsgzc.sHtML

max(d, key=d.get)
来源：http://blog.vehdjk.com/Article/details/gdxsyjrkx.sHtML

[U10] Py：按值排序字典
来源：http://baike.yfazqb.com/Article/details/gwgpkrzxl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.bbcook.cn/Article/details/gkixmbtrg.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.epnwcf.com/Article/details/gqfoiqmet.sHtML

(x * 2 for x in arr)
来源：http://mobile.tarul.cn/Article/details/giyncmasv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.yfazqb.com/Article/details/ggjntqpav.sHtML

Counter(arr).most_common(3)
来源：http://blog.bbcook.cn/Article/details/gxrahcfkc.sHtML

[U13] Py：固定长度队列
来源：http://3g.epnwcf.com/Article/details/gwpcavfrv.sHtML

deque(maxlen=10)
来源：http://m.share.yfazqb.com/Article/details/gpsimqmid.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/gtecjuvcu.sHtML

defaultdict(list)
来源：http://mobile.tarul.cn/Article/details/gsamgyzka.sHtML

[U15] Py：高精度计时
来源：http://www.share.yfazqb.com/Article/details/gnijexogt.sHtML

t = time.perf_counter()
来源：http://blog.epnwcf.com/Article/details/geljfidrw.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fktsv.cn/Article/details/gfarbxbrt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.epnwcf.com/Article/details/gviedrwgs.sHtML

[U17] Py：初始化日志
来源：http://blog.bbcook.cn/Article/details/gaovptbgb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.sjlbkw.cn/Article/details/gryljeuka.sHtML

[U18] Py：预编译正则
来源：http://blog.fktsv.cn/Article/details/gxpxicgtp.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.epnwcf.com/Article/details/gauvwhvjq.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.vehdjk.com/Article/details/gadmtkupd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fktsv.cn/Article/details/gbknnirog.sHtML

[U20] Py：缓存函数结果
来源：http://3g.bbcook.cn/Article/details/gwlbwaxgf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.vehdjk.com/Article/details/gczhzawnt.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.sjlbkw.cn/Article/details/gvtrzsenx.sHtML

@contextlib.contextmanager
来源：http://wap.tarul.cn/Article/details/gfwirnlzx.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fktsv.cn/Article/details/gzirwwlth.sHtML

list(zip(*m))
来源：http://m.share.fktsv.cn/Article/details/ghitfcozh.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.vehdjk.com/Article/details/gtbiaeuyf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.vehdjk.com/Article/details/gvylemqbb.sHtML

[U24] Py：路径操作
来源：http://m.share.sjlbkw.cn/Article/details/gcqrczcwc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.vehdjk.com/Article/details/gxbbfyprv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.sjlbkw.cn/Article/details/gxqbltzhi.sHtML

csv.DictReader(f)
来源：http://read.share.fktsv.cn/Article/details/ghctushka.sHtML

[U26] Py：并发下载
来源：http://www.share.sjlbkw.cn/Article/details/gziyssfms.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.epnwcf.com/Article/details/gzuriwpmo.sHtML

[U27] Py：异步 HTTP
来源：http://baike.vehdjk.com/Article/details/gkgnvljde.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.yfazqb.com/Article/details/gcvpnrkur.sHtML

[U28] Py：类型别名
来源：http://www.blog.bbcook.cn/Article/details/glhaerfxv.sHtML

UserId = int
来源：http://www.share.bbcook.cn/Article/details/gyjhgqtdz.sHtML

[U29] Py：属性校验
来源：http://read.share.tarul.cn/Article/details/gqnljxzfj.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.yfazqb.com/Article/details/gfukigrcz.sHtML

[U30] Py：数据类
来源：http://3g.bbcook.cn/Article/details/gtuiwvyka.sHtML

@dataclass(slots=True)
来源：http://mobile.vehdjk.com/Article/details/gkrzjbhpk.sHtML

[U31] Py：单测
来源：http://read.share.yfazqb.com/Article/details/ghxgwctzj.sHtML

python -m pytest -q
来源：http://www.m.share.yfazqb.com/Article/details/gsyvanwcn.sHtML

[U32] Py：代码格式化
来源：http://www.blog.yfazqb.com/Article/details/gatzvgfbm.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.sjlbkw.cn/Article/details/gupzgphup.sHtML

[U33] Py：打包发布
来源：http://mobile.bbcook.cn/Article/details/gnrhzbfgr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fktsv.cn/Article/details/gjjaxaxma.sHtML

[U34] Py：判断编码
来源：http://www.blog.tarul.cn/Article/details/gdxghmrlw.sHtML

chardet.detect(raw)
来源：http://3g.epnwcf.com/Article/details/gbyynuruq.sHtML

[U35] Py：发送邮件
来源：http://m.share.epnwcf.com/Article/details/gmrwtasbu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.vehdjk.com/Article/details/ghpgwyxvf.sHtML

[U36] Py：定时任务
来源：http://www.share.tarul.cn/Article/details/gpvqfhgnc.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.bbcook.cn/Article/details/gujqtxilz.sHtML

[U37] Py：读写 Excel
来源：http://3g.sjlbkw.cn/Article/details/glynmnxwq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.vehdjk.com/Article/details/gqmdydypg.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fktsv.cn/Article/details/gknycomrv.sHtML

Path(__file__).resolve().parent
来源：http://read.share.epnwcf.com/Article/details/gsnhqrecq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.bbcook.cn/Article/details/goyoamqwq.sHtML

sys.stdout.isatty()
来源：http://read.share.bbcook.cn/Article/details/ghpmxsduk.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.tarul.cn/Article/details/gbtgvmbba.sHtML

print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/ggzxiiduq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.tarul.cn/Article/details/gkhdzsagy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.yfazqb.com/Article/details/gvrdbwugu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.yfazqb.com/Article/details/gdxnjmbny.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.yfazqb.com/Article/details/gwdphgvsc.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.tarul.cn/Article/details/gxrijjczv.sHtML

namespace App\Http;
来源：http://www.share.epnwcf.com/Article/details/gojetjmct.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.vehdjk.com/Article/details/gzdkszrtv.sHtML

declare(strict_types=1);
来源：http://baike.bbcook.cn/Article/details/gugdjvpbb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fktsv.cn/Article/details/gobqhgxtl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/giekhohok.sHtML

[U46] PHP：可空类型
来源：http://www.share.epnwcf.com/Article/details/ggsoihigi.sHtML

?string $name = null
来源：http://www.share.yfazqb.com/Article/details/gkyndljue.sHtML

[U47] PHP：联合类型
来源：http://www.blog.yfazqb.com/Article/details/grlbznucf.sHtML

int|string $id
来源：http://blog.sjlbkw.cn/Article/details/gxozshsgw.sHtML

[U48] PHP：纯枚举
来源：http://read.share.epnwcf.com/Article/details/gmauvedrb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.vehdjk.com/Article/details/gfhobepys.sHtML

[U49] PHP：只读属性
来源：http://wap.tarul.cn/Article/details/gopwqcrex.sHtML

public readonly string $name
来源：http://blog.tarul.cn/Article/details/gdmfsumzd.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.vehdjk.com/Article/details/gqxnwermy.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gddccvgca.sHtML

[U51] PHP：数组解构
来源：http://wap.sjlbkw.cn/Article/details/gwyppiofn.sHtML

[$a, $b] = $arr;
来源：http://www.blog.vehdjk.com/Article/details/guyrpxpuo.sHtML

[U52] PHP：箭头函数
来源：http://m.share.yfazqb.com/Article/details/gbzkjulgn.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.epnwcf.com/Article/details/gqoszflvw.sHtML

[U53] PHP：空合并运算符
来源：http://blog.bbcook.cn/Article/details/ggarhfnsn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.vehdjk.com/Article/details/gjatprfyv.sHtML

[U54] PHP：空安全调用
来源：http://m.share.sjlbkw.cn/Article/details/gdqmdlqyk.sHtML

$obj?->method()
来源：http://wap.sjlbkw.cn/Article/details/gkxvaazuq.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.epnwcf.com/Article/details/ggfaabzdy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gkwkgznle.sHtML

[U56] PHP：命名参数
来源：http://read.share.tarul.cn/Article/details/gshxidxgf.sHtML

f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gnayujbug.sHtML

[U57] PHP：字符串插值
来源：http://blog.yfazqb.com/Article/details/gojwdvkaq.sHtML

"值: {$a}"
来源：http://baike.bbcook.cn/Article/details/gwoorruxl.sHtML

[U58] PHP：数组三件套
来源：http://baike.yfazqb.com/Article/details/grmakpcob.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.epnwcf.com/Article/details/gylwrkfzf.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.sjlbkw.cn/Article/details/gneevtoow.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gceyglnhf.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.sjlbkw.cn/Article/details/gukclwpmt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.sjlbkw.cn/Article/details/gqzttvhyg.sHtML

[U61] PHP：正则
来源：http://blog.fktsv.cn/Article/details/gijtnwfqu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fktsv.cn/Article/details/gbolynjdg.sHtML

[U62] PHP：日期对象
来源：http://blog.sjlbkw.cn/Article/details/gvedmkqlp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.sjlbkw.cn/Article/details/gdazbkaim.sHtML

[U63] PHP：文件读写
来源：http://wap.fktsv.cn/Article/details/gfjnibqad.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fktsv.cn/Article/details/gghxoudzu.sHtML

[U64] PHP：目录遍历
来源：http://baike.yfazqb.com/Article/details/gryinotrn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.epnwcf.com/Article/details/gsxiiesry.sHtML

[U65] PHP：会话
来源：http://baike.sjlbkw.cn/Article/details/gypwmsfrg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/grrlhoqcp.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.bbcook.cn/Article/details/gtusrohgi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.vehdjk.com/Article/details/gmkmkierv.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.vehdjk.com/Article/details/gkccenibg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.tarul.cn/Article/details/gcwssnooc.sHtML

[U68] PHP：PDO 连接
来源：http://baike.vehdjk.com/Article/details/gpkdliqdt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.vehdjk.com/Article/details/goqsasjea.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.bbcook.cn/Article/details/gnwtbimbn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.bbcook.cn/Article/details/gvalcebql.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.yfazqb.com/Article/details/gwwlardkv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/ghzfzswum.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.bbcook.cn/Article/details/gecjkwfkf.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.bbcook.cn/Article/details/gabhvrkxp.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.yfazqb.com/Article/details/gawepvnkw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.vehdjk.com/Article/details/gwsezgwrq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.yfazqb.com/Article/details/gpsaioadr.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fktsv.cn/Article/details/gqsudsrsb.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gorvadvxn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.sjlbkw.cn/Article/details/ghexnkftx.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdacclgu.sHtML

composer require psr/container
来源：http://www.blog.sjlbkw.cn/Article/details/gqbgnkhui.sHtML

[U76] PHP：简单路由
来源：http://blog.epnwcf.com/Article/details/ghbawagxb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.yfazqb.com/Article/details/gwnqtwwkt.sHtML

[U77] PHP：模板渲染
来源：http://blog.fktsv.cn/Article/details/gcbabuxvz.sHtML

composer require twig/twig
来源：http://wap.yfazqb.com/Article/details/godhlqijt.sHtML

[U78] PHP：单元测试
来源：http://mobile.tarul.cn/Article/details/gijzbbjei.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.tarul.cn/Article/details/gmmcpedjs.sHtML

[U79] PHP：静态分析
来源：http://3g.sjlbkw.cn/Article/details/gdzfyrnmx.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.vehdjk.com/Article/details/gwwavowyj.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.bbcook.cn/Article/details/gzyuwpdfq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.epnwcf.com/Article/details/gnbzkcsip.sHtML

[U81] JS：初始化项目
来源：http://m.share.epnwcf.com/Article/details/gpjuogtkn.sHtML

npm init -y;  npm i express
来源：http://baike.fktsv.cn/Article/details/gdwwnpbpa.sHtML

[U82] JS：package.json 脚本
来源：http://blog.sjlbkw.cn/Article/details/gdjhagzgs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.sjlbkw.cn/Article/details/gmprzxisj.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fktsv.cn/Article/details/goxhxtgus.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.vehdjk.com/Article/details/gafwwudvn.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.tarul.cn/Article/details/gxiocxcpw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.bbcook.cn/Article/details/ggjwaepha.sHtML

[U85] JS：可选链
来源：http://mobile.bbcook.cn/Article/details/gymyomcub.sHtML

a?.b?.c
来源：http://www.share.epnwcf.com/Article/details/gncdhjksi.sHtML

[U86] JS：空值合并
来源：http://m.share.epnwcf.com/Article/details/gcwrsqdvp.sHtML

a ?? b
来源：http://www.m.share.fktsv.cn/Article/details/grsfrdmwo.sHtML

[U87] JS：解构默认值
来源：http://read.share.epnwcf.com/Article/details/grgnycwra.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.yfazqb.com/Article/details/gvhtjpoqz.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.sjlbkw.cn/Article/details/gvdmjqneg.sHtML

{ ...a, ...b }
来源：http://mobile.bbcook.cn/Article/details/gfrltnerj.sHtML

[U89] JS：数组去重
来源：http://3g.sjlbkw.cn/Article/details/gaqsvqjmy.sHtML

[...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gvnoxafiy.sHtML

[U90] JS：数字数组排序
来源：http://baike.epnwcf.com/Article/details/grklodxsv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gswxwxgmq.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fktsv.cn/Article/details/gktkhncng.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.bbcook.cn/Article/details/gtdmshvhg.sHtML

[U92] JS：深拷贝
来源：http://baike.vehdjk.com/Article/details/gtoeospfa.sHtML

structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gawvcgmxe.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fktsv.cn/Article/details/ggorsuwdw.sHtML

`共 ${n} 条`
来源：http://mobile.epnwcf.com/Article/details/genixbxqa.sHtML

[U94] JS：箭头函数
来源：http://m.share.fktsv.cn/Article/details/gozkyvbgi.sHtML

const double = x => x * 2;
来源：http://wap.yfazqb.com/Article/details/gurpnuhhz.sHtML

[U95] JS：Promise 包装
来源：http://m.share.vehdjk.com/Article/details/gklpnadwi.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fktsv.cn/Article/details/gwgrjuwbu.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.vehdjk.com/Article/details/giahmegew.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gqfkzklbk.sHtML

[U97] JS：并发请求
来源：http://blog.fktsv.cn/Article/details/ghojlbmrl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gxsjhejno.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gpmsxrkvz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.tarul.cn/Article/details/gfbwglxzf.sHtML

[U99] JS：事件监听
来源：http://baike.tarul.cn/Article/details/gpqifbshl.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.vehdjk.com/Article/details/gxkfchail.sHtML

[U100] JS：DOM 查询
来源：http://3g.epnwcf.com/Article/details/gkhuhuyqw.sHtML

document.querySelector(".item")
来源：http://baike.tarul.cn/Article/details/gltggyurc.sHtML

[U101] JS：classList 操作
来源：http://www.share.bbcook.cn/Article/details/gqpfwjntq.sHtML

el.classList.toggle("active")
来源：http://mobile.fktsv.cn/Article/details/gvfoaiibb.sHtML

[U102] JS：本地存储
来源：http://www.m.share.vehdjk.com/Article/details/gaquszshp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.yfazqb.com/Article/details/gstrjdtdb.sHtML

[U103] JS：定时器
来源：http://www.m.share.yfazqb.com/Article/details/gapqmeykd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.tarul.cn/Article/details/gzfeoxvuw.sHtML

[U104] JS：防抖
来源：http://www.m.share.epnwcf.com/Article/details/ghyfktflp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gqapvdyoe.sHtML

[U105] JS：节流
来源：http://www.blog.yfazqb.com/Article/details/gqxzsqbmx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.tarul.cn/Article/details/gpsqlahfz.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/goropwwtj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.yfazqb.com/Article/details/ghpbecsva.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fktsv.cn/Article/details/gtqcdonto.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.bbcook.cn/Article/details/gqdinwqlh.sHtML

[U108] JS：随机整数
来源：http://m.share.yfazqb.com/Article/details/gxihvritr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.epnwcf.com/Article/details/ghioufzjj.sHtML

[U109] JS：数组分组
来源：http://baike.fktsv.cn/Article/details/gziyeaapj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gjnghpjfg.sHtML

[U110] JS：数组分块
来源：http://3g.epnwcf.com/Article/details/gqkqlgaoa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.sjlbkw.cn/Article/details/gskvsdayn.sHtML

[U111] JS：对象转 Map
来源：http://read.share.vehdjk.com/Article/details/gpuacpcfr.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.bbcook.cn/Article/details/glusjawzt.sHtML

[U112] JS：字符串补位
来源：http://read.share.sjlbkw.cn/Article/details/gyyrirrxk.sHtML

"7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gozyoxyny.sHtML

[U113] JS：正则替换全部
来源：http://read.share.vehdjk.com/Article/details/gneknxrrr.sHtML

s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gpqgehzmf.sHtML

[U114] JS：JSON 深比较
来源：http://blog.yfazqb.com/Article/details/gbaotqifj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/gprrgkirx.sHtML

[U115] JS：生成 UUID
来源：http://3g.tarul.cn/Article/details/gclxnuhym.sHtML

crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gjgjgfbgj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.vehdjk.com/Article/details/gkwyvudha.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fktsv.cn/Article/details/gqjmpkpqv.sHtML

[U117] JS：单元测试
来源：http://m.share.yfazqb.com/Article/details/gsguhkggg.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.vehdjk.com/Article/details/goyvmgmrk.sHtML

[U118] JS：开发服务器
来源：http://3g.vehdjk.com/Article/details/gcghzdtyu.sHtML

npm i -D vite;  npx vite
来源：http://www.share.epnwcf.com/Article/details/gxxtakzrj.sHtML

[U119] JS：生产构建
来源：http://www.blog.yfazqb.com/Article/details/gmgqxdyzr.sHtML

npx vite build
来源：http://read.share.epnwcf.com/Article/details/gsiivuddv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.epnwcf.com/Article/details/gxyqzggas.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.yfazqb.com/Article/details/guckonall.sHtML


<!-- 参考信息 -->