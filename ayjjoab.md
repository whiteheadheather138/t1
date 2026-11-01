代发 wailian999

[T33] Lua：表（数组）
来源：http://mobile.yfazqb.com/Article/details/gcvxzpsbl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.tarul.cn/Article/details/ghhsayqsr.sHtML

[T34] Lua：遍历表
来源：http://3g.tarul.cn/Article/details/ggugvefvt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.tarul.cn/Article/details/gaingqeyp.sHtML

[T35] Lua：字典表
来源：http://wap.tarul.cn/Article/details/giyzszljx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fktsv.cn/Article/details/gsxwbmnho.sHtML

[T36] Lua：函数
来源：http://wap.fktsv.cn/Article/details/golpnmgyw.sHtML

function add(a, b) return a + b end
来源：http://wap.sjlbkw.cn/Article/details/glicwrnsg.sHtML

[T37] Lua：字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gysdecuvs.sHtML

"a" .. "b"
来源：http://www.share.tarul.cn/Article/details/guvkbjuin.sHtML

[T38] Lua：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gaabbgeah.sHtML

if x > 0 then print("正") end
来源：http://baike.bbcook.cn/Article/details/groeffond.sHtML

[T39] Lua：模式匹配
来源：http://mobile.epnwcf.com/Article/details/gnblufdfj.sHtML

string.find(s, "%d+")
来源：http://3g.yfazqb.com/Article/details/gdiuqhupn.sHtML

[T40] Lua：元表
来源：http://3g.tarul.cn/Article/details/gpgnlutvg.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.tarul.cn/Article/details/ghfxhrfqc.sHtML

[T41] Perl：Hello World
来源：http://read.share.bbcook.cn/Article/details/gaimnbxrw.sHtML

print "Hello\n";
来源：http://m.share.epnwcf.com/Article/details/gqswzinhk.sHtML

[T42] Perl：变量类型
来源：http://read.share.sjlbkw.cn/Article/details/gjckodcip.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjcveqfj.sHtML

[T43] Perl：字符串插值
来源：http://wap.vehdjk.com/Article/details/gfjztcjag.sHtML

"值: $a"
来源：http://www.share.vehdjk.com/Article/details/gnjgfhqqo.sHtML

[T44] Perl：条件
来源：http://blog.tarul.cn/Article/details/gnzlntrib.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.vehdjk.com/Article/details/gyrboibec.sHtML

[T45] Perl：数组遍历
来源：http://m.share.bbcook.cn/Article/details/grxljfant.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.yfazqb.com/Article/details/gpvqhfxtg.sHtML

[T46] Perl：哈希操作
来源：http://blog.tarul.cn/Article/details/gcwqjsudq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.sjlbkw.cn/Article/details/goxnimrsg.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.bbcook.cn/Article/details/gvufltwkp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.tarul.cn/Article/details/gguljmqkx.sHtML

[T48] Perl：正则替换
来源：http://wap.epnwcf.com/Article/details/giczaazuw.sHtML

$s =~ s/old/new/g;
来源：http://mobile.epnwcf.com/Article/details/gejkwuusg.sHtML

[T49] Perl：函数
来源：http://www.blog.bbcook.cn/Article/details/gopilbykg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gaxheqayt.sHtML

[T50] Perl：逐行读文件
来源：http://3g.bbcook.cn/Article/details/geprfghlu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.yfazqb.com/Article/details/gpyyxqzof.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.vehdjk.com/Article/details/gzhugxsri.sHtML

[T51] Scala：Hello World
来源：http://read.share.tarul.cn/Article/details/gmxcwrikx.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gvepqyrok.sHtML

[T52] Scala：变量
来源：http://3g.fktsv.cn/Article/details/gzzpccfhc.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.epnwcf.com/Article/details/grhwmxbnj.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fktsv.cn/Article/details/goeborqau.sHtML

s"值: $b"
来源：http://wap.epnwcf.com/Article/details/gxirbiynf.sHtML

[T54] Scala：集合映射
来源：http://blog.epnwcf.com/Article/details/gjghtxwjs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.vehdjk.com/Article/details/gappgjxko.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/goisyjugp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/gsfuhmhsw.sHtML

[T56] Scala：样例类
来源：http://baike.yfazqb.com/Article/details/gzysdwoun.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/gumrvawiy.sHtML

[T57] Scala：模式匹配
来源：http://baike.fktsv.cn/Article/details/grsbrxswm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fktsv.cn/Article/details/ghjjscbwj.sHtML

[T58] Scala：函数定义
来源：http://wap.vehdjk.com/Article/details/glegcfqos.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.bbcook.cn/Article/details/glhrdejfw.sHtML

[T59] Scala：循环
来源：http://mobile.tarul.cn/Article/details/gliekxmha.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.yfazqb.com/Article/details/gayimgumg.sHtML

[T60] Scala：折叠
来源：http://www.m.share.sjlbkw.cn/Article/details/gjveypnwv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.vehdjk.com/Article/details/gcgcopvqi.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gqaisbnxz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/gtxiyfspe.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxzupgcvy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.yfazqb.com/Article/details/gvagzjxza.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/gjghxewzh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.tarul.cn/Article/details/gatluufey.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.epnwcf.com/Article/details/gnbeavzzx.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fktsv.cn/Article/details/gcwgurzdg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fktsv.cn/Article/details/gutwqnglt.sHtML

[U04] Py：变量调试打印
来源：http://3g.epnwcf.com/Article/details/gbyaahntk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fktsv.cn/Article/details/gzgtvlqmj.sHtML

[U05] Py：列表去重且保序
来源：http://wap.tarul.cn/Article/details/gqmvqgqis.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/gbfbxtifs.sHtML

[U06] Py：合并两个字典
来源：http://www.share.vehdjk.com/Article/details/gnpblsgik.sHtML

{**a, **b}
来源：http://www.m.share.yfazqb.com/Article/details/gcpmnemjb.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gqnroksoc.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.sjlbkw.cn/Article/details/gljntlpoj.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fktsv.cn/Article/details/gkeertxcv.sHtML

[y for x in nested for y in x]
来源：http://mobile.yfazqb.com/Article/details/gktvazrma.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.sjlbkw.cn/Article/details/grglkeadw.sHtML

max(d, key=d.get)
来源：http://mobile.bbcook.cn/Article/details/gjusennqh.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fktsv.cn/Article/details/gwzsuolpp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.bbcook.cn/Article/details/gubgadpfs.sHtML

[U11] Py：生成器表达式
来源：http://3g.tarul.cn/Article/details/gpqkwmmbo.sHtML

(x * 2 for x in arr)
来源：http://blog.sjlbkw.cn/Article/details/gytwieslw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.yfazqb.com/Article/details/gemvssalz.sHtML

Counter(arr).most_common(3)
来源：http://3g.fktsv.cn/Article/details/gulobqaye.sHtML

[U13] Py：固定长度队列
来源：http://baike.yfazqb.com/Article/details/gesfmxbef.sHtML

deque(maxlen=10)
来源：http://wap.vehdjk.com/Article/details/gssgdzkmw.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fktsv.cn/Article/details/gizeiitjh.sHtML

defaultdict(list)
来源：http://www.share.sjlbkw.cn/Article/details/gpzpzbqaw.sHtML

[U15] Py：高精度计时
来源：http://mobile.sjlbkw.cn/Article/details/goywbiurh.sHtML

t = time.perf_counter()
来源：http://m.share.tarul.cn/Article/details/gqedaikqz.sHtML

[U16] Py：命令行参数解析
来源：http://wap.tarul.cn/Article/details/ghuajymku.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.vehdjk.com/Article/details/gegoakppm.sHtML

[U17] Py：初始化日志
来源：http://m.share.yfazqb.com/Article/details/gsxiizmop.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.yfazqb.com/Article/details/gmpxaindj.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.vehdjk.com/Article/details/gzldphcuy.sHtML

pat = re.compile(r"\d+")
来源：http://baike.vehdjk.com/Article/details/gekxhgfxf.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.tarul.cn/Article/details/guxgtwvmp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.epnwcf.com/Article/details/gdjaxeetn.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.epnwcf.com/Article/details/geazwiprv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.sjlbkw.cn/Article/details/gkfprvzyn.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.bbcook.cn/Article/details/gxlyjwreh.sHtML

@contextlib.contextmanager
来源：http://read.share.bbcook.cn/Article/details/geizusfcr.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fktsv.cn/Article/details/goksmlsth.sHtML

list(zip(*m))
来源：http://www.m.share.tarul.cn/Article/details/gnyhdrmdg.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.sjlbkw.cn/Article/details/gjnxvbjet.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.vehdjk.com/Article/details/gscpzxudy.sHtML

[U24] Py：路径操作
来源：http://wap.tarul.cn/Article/details/ghvxmprzm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gqejzbiiu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.bbcook.cn/Article/details/gksbuxjre.sHtML

csv.DictReader(f)
来源：http://blog.bbcook.cn/Article/details/guxxjldpx.sHtML

[U26] Py：并发下载
来源：http://wap.bbcook.cn/Article/details/gmorqbbbh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.epnwcf.com/Article/details/ggxdvqymq.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.yfazqb.com/Article/details/gcpicqzsy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.yfazqb.com/Article/details/grfkoiusk.sHtML

[U28] Py：类型别名
来源：http://www.share.bbcook.cn/Article/details/guracubfu.sHtML

UserId = int
来源：http://www.blog.vehdjk.com/Article/details/gqfrkvxqo.sHtML

[U29] Py：属性校验
来源：http://mobile.sjlbkw.cn/Article/details/gbpdqzejt.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.tarul.cn/Article/details/gajgxylrw.sHtML

[U30] Py：数据类
来源：http://blog.sjlbkw.cn/Article/details/gcmvrexxk.sHtML

@dataclass(slots=True)
来源：http://wap.tarul.cn/Article/details/gwtxqdyzn.sHtML

[U31] Py：单测
来源：http://m.share.yfazqb.com/Article/details/gjhrvvpwb.sHtML

python -m pytest -q
来源：http://m.share.tarul.cn/Article/details/gjvrkygxe.sHtML

[U32] Py：代码格式化
来源：http://wap.yfazqb.com/Article/details/gnewrbvee.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.yfazqb.com/Article/details/gszjvqlhy.sHtML

[U33] Py：打包发布
来源：http://mobile.vehdjk.com/Article/details/gkibvjvhc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.sjlbkw.cn/Article/details/gooslohyn.sHtML

[U34] Py：判断编码
来源：http://read.share.sjlbkw.cn/Article/details/gkjhsyluo.sHtML

chardet.detect(raw)
来源：http://3g.yfazqb.com/Article/details/gpbgujrxp.sHtML

[U35] Py：发送邮件
来源：http://mobile.tarul.cn/Article/details/gpirxwksh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.sjlbkw.cn/Article/details/galctqtjr.sHtML

[U36] Py：定时任务
来源：http://www.share.tarul.cn/Article/details/gqtgcpsun.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.epnwcf.com/Article/details/gzsrmbtyl.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.vehdjk.com/Article/details/gywcmdlsq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.vehdjk.com/Article/details/gpnwfvarr.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.vehdjk.com/Article/details/goxbpsdon.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fktsv.cn/Article/details/gqumeknwv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.vehdjk.com/Article/details/gdwagifva.sHtML

sys.stdout.isatty()
来源：http://www.m.share.epnwcf.com/Article/details/gqebrsaqm.sHtML

[U40] Py：打印到标准错误
来源：http://baike.sjlbkw.cn/Article/details/gppovfhgw.sHtML

print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/gbhaihyuu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.sjlbkw.cn/Article/details/ghmlpucrr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.yfazqb.com/Article/details/gqxywgbrq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.epnwcf.com/Article/details/gzdzjjmsv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.tarul.cn/Article/details/gkuiplnvw.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fktsv.cn/Article/details/gebywgsgg.sHtML

namespace App\Http;
来源：http://m.share.vehdjk.com/Article/details/gkuulrzwr.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fktsv.cn/Article/details/geplucpfu.sHtML

declare(strict_types=1);
来源：http://www.m.share.sjlbkw.cn/Article/details/giiwwibce.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.epnwcf.com/Article/details/gojyohzty.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/ghcmovsmq.sHtML

[U46] PHP：可空类型
来源：http://mobile.bbcook.cn/Article/details/gjtsljwnh.sHtML

?string $name = null
来源：http://www.share.tarul.cn/Article/details/gormtjbkt.sHtML

[U47] PHP：联合类型
来源：http://www.share.fktsv.cn/Article/details/ganykrbsi.sHtML

int|string $id
来源：http://m.share.vehdjk.com/Article/details/gxfnpfoor.sHtML

[U48] PHP：纯枚举
来源：http://mobile.epnwcf.com/Article/details/gnhwfxvfe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.bbcook.cn/Article/details/gjpyvypsl.sHtML

[U49] PHP：只读属性
来源：http://3g.tarul.cn/Article/details/gkebxmptr.sHtML

public readonly string $name
来源：http://mobile.bbcook.cn/Article/details/gxsdjsoyl.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.sjlbkw.cn/Article/details/gogkxkkve.sHtML

public function __construct(private int $id) {}
来源：http://mobile.yfazqb.com/Article/details/gfqemkict.sHtML

[U51] PHP：数组解构
来源：http://wap.vehdjk.com/Article/details/gfnhpsjkw.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.vehdjk.com/Article/details/gzgkylanb.sHtML

[U52] PHP：箭头函数
来源：http://wap.yfazqb.com/Article/details/gblwnxele.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.sjlbkw.cn/Article/details/gtspflscl.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fktsv.cn/Article/details/gsliyyebc.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.bbcook.cn/Article/details/gjafdxuec.sHtML

[U54] PHP：空安全调用
来源：http://mobile.bbcook.cn/Article/details/geepwmiyq.sHtML

$obj?->method()
来源：http://www.m.share.fktsv.cn/Article/details/glyseipkq.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fktsv.cn/Article/details/gcvcihyqb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.vehdjk.com/Article/details/guzdfhewv.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fktsv.cn/Article/details/gmgtbrstm.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gguqnepqy.sHtML

[U57] PHP：字符串插值
来源：http://blog.fktsv.cn/Article/details/gneffwucr.sHtML

"值: {$a}"
来源：http://www.share.fktsv.cn/Article/details/guaterzvc.sHtML

[U58] PHP：数组三件套
来源：http://read.share.yfazqb.com/Article/details/gwrpjuwdb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.epnwcf.com/Article/details/ghnyvoukq.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fktsv.cn/Article/details/gwwkttzmt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.tarul.cn/Article/details/gozmacoox.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.vehdjk.com/Article/details/gxmvhrnae.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.tarul.cn/Article/details/gwbqnytbp.sHtML

[U61] PHP：正则
来源：http://read.share.yfazqb.com/Article/details/gjgptbxgo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/gcobtwhxb.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fktsv.cn/Article/details/ghkihpyhj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.yfazqb.com/Article/details/gkqvnajfq.sHtML

[U63] PHP：文件读写
来源：http://baike.sjlbkw.cn/Article/details/gkvetnzkw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.sjlbkw.cn/Article/details/gtwfvckqf.sHtML

[U64] PHP：目录遍历
来源：http://wap.tarul.cn/Article/details/ghuzbthrx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.sjlbkw.cn/Article/details/ghrchrjto.sHtML

[U65] PHP：会话
来源：http://blog.sjlbkw.cn/Article/details/gqajbhlre.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/grkhvzemb.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.tarul.cn/Article/details/ghrnpgbpu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fktsv.cn/Article/details/gffnebzic.sHtML

[U67] PHP：处理文件上传
来源：http://baike.sjlbkw.cn/Article/details/gmrbfryyt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.epnwcf.com/Article/details/gfheuovcp.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fktsv.cn/Article/details/gjoetsjog.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.bbcook.cn/Article/details/gzeogyfgu.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.vehdjk.com/Article/details/gckproijc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.sjlbkw.cn/Article/details/gitwlzrah.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.epnwcf.com/Article/details/gaofritkh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.tarul.cn/Article/details/gxgizumyj.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.epnwcf.com/Article/details/grqlrssjj.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fktsv.cn/Article/details/grfbzjyqd.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.epnwcf.com/Article/details/gipvmltdh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.yfazqb.com/Article/details/gnipygvyr.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.yfazqb.com/Article/details/gnqrderbc.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.epnwcf.com/Article/details/gzwdotrwx.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.vehdjk.com/Article/details/gnbhxhndv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.bbcook.cn/Article/details/gnawryswd.sHtML

[U75] PHP：依赖注入
来源：http://3g.fktsv.cn/Article/details/gfvahgawh.sHtML

composer require psr/container
来源：http://m.share.fktsv.cn/Article/details/gdhurjqwc.sHtML

[U76] PHP：简单路由
来源：http://blog.yfazqb.com/Article/details/gjjkxnlin.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.bbcook.cn/Article/details/gaztqceaz.sHtML

[U77] PHP：模板渲染
来源：http://mobile.bbcook.cn/Article/details/gcumntgrf.sHtML

composer require twig/twig
来源：http://mobile.bbcook.cn/Article/details/gajrubbyv.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.epnwcf.com/Article/details/guhpunhfg.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.yfazqb.com/Article/details/gmpzyaumy.sHtML

[U79] PHP：静态分析
来源：http://mobile.yfazqb.com/Article/details/gsapvkfdv.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.tarul.cn/Article/details/gwdvaynri.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fktsv.cn/Article/details/geocwarhx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.bbcook.cn/Article/details/gtmmnqwmg.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.tarul.cn/Article/details/gfialgyxm.sHtML

npm init -y;  npm i express
来源：http://www.share.epnwcf.com/Article/details/gibgroqzx.sHtML

[U82] JS：package.json 脚本
来源：http://3g.vehdjk.com/Article/details/gkmhscjoh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.vehdjk.com/Article/details/goxafuugr.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.epnwcf.com/Article/details/gjtaeofet.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/grgnznvpj.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.epnwcf.com/Article/details/gqofkogmi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.tarul.cn/Article/details/gxdsqlntw.sHtML

[U85] JS：可选链
来源：http://m.share.bbcook.cn/Article/details/gjaoilqkz.sHtML

a?.b?.c
来源：http://m.share.epnwcf.com/Article/details/grqptoxox.sHtML

[U86] JS：空值合并
来源：http://read.share.sjlbkw.cn/Article/details/gsbhmkbkn.sHtML

a ?? b
来源：http://wap.tarul.cn/Article/details/gqayyhtub.sHtML

[U87] JS：解构默认值
来源：http://3g.sjlbkw.cn/Article/details/gecpmjkmh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.tarul.cn/Article/details/gqoyilgjj.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.vehdjk.com/Article/details/gxfpxjeps.sHtML

{ ...a, ...b }
来源：http://www.blog.bbcook.cn/Article/details/gnktnajqx.sHtML

[U89] JS：数组去重
来源：http://www.m.share.bbcook.cn/Article/details/gzudsbsra.sHtML

[...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gubiooevt.sHtML

[U90] JS：数字数组排序
来源：http://wap.vehdjk.com/Article/details/gdddlksnj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gznzwvcdr.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fktsv.cn/Article/details/gmplqlfah.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.vehdjk.com/Article/details/gkvwzrnsu.sHtML

[U92] JS：深拷贝
来源：http://mobile.tarul.cn/Article/details/gvuiokgli.sHtML

structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gimnqmbua.sHtML

[U93] JS：模板字符串
来源：http://read.share.vehdjk.com/Article/details/gsguntkms.sHtML

`共 ${n} 条`
来源：http://www.share.epnwcf.com/Article/details/gcsuijwnh.sHtML

[U94] JS：箭头函数
来源：http://m.share.vehdjk.com/Article/details/goxcoskkx.sHtML

const double = x => x * 2;
来源：http://www.m.share.sjlbkw.cn/Article/details/gceiebtmp.sHtML

[U95] JS：Promise 包装
来源：http://wap.vehdjk.com/Article/details/gzqklzkhq.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.sjlbkw.cn/Article/details/getleleia.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.vehdjk.com/Article/details/gchwarxoz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gdgngkefl.sHtML

[U97] JS：并发请求
来源：http://3g.fktsv.cn/Article/details/gqixkezbt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gdqzkghlf.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.bbcook.cn/Article/details/gksomvwlo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.bbcook.cn/Article/details/gjkrrbbyf.sHtML

[U99] JS：事件监听
来源：http://read.share.bbcook.cn/Article/details/gugirnxeg.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.yfazqb.com/Article/details/gwwcdqohl.sHtML

[U100] JS：DOM 查询
来源：http://mobile.epnwcf.com/Article/details/gtbyvqlok.sHtML

document.querySelector(".item")
来源：http://www.share.yfazqb.com/Article/details/gtiuwkcza.sHtML

[U101] JS：classList 操作
来源：http://wap.tarul.cn/Article/details/grdtnpdku.sHtML

el.classList.toggle("active")
来源：http://www.blog.tarul.cn/Article/details/glkgsoykh.sHtML

[U102] JS：本地存储
来源：http://www.share.bbcook.cn/Article/details/gsnvwggpg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.yfazqb.com/Article/details/gsmvjates.sHtML

[U103] JS：定时器
来源：http://m.share.epnwcf.com/Article/details/gmmvsmxaa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.yfazqb.com/Article/details/gjmkgrovw.sHtML

[U104] JS：防抖
来源：http://3g.epnwcf.com/Article/details/gdcdclnvd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gtrlupszk.sHtML

[U105] JS：节流
来源：http://3g.tarul.cn/Article/details/gbukgcbnn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.sjlbkw.cn/Article/details/gxdpgbele.sHtML

[U106] JS：日期格式化
来源：http://blog.tarul.cn/Article/details/ghxiyemtv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.vehdjk.com/Article/details/gidndbavb.sHtML

[U107] JS：数字千分位
来源：http://baike.fktsv.cn/Article/details/gaouocozx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fktsv.cn/Article/details/grqjcbbld.sHtML

[U108] JS：随机整数
来源：http://read.share.bbcook.cn/Article/details/ghpcaexrk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.epnwcf.com/Article/details/gczlqmuzf.sHtML

[U109] JS：数组分组
来源：http://blog.bbcook.cn/Article/details/girciiphg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.sjlbkw.cn/Article/details/gyedmfaqo.sHtML

[U110] JS：数组分块
来源：http://mobile.epnwcf.com/Article/details/grjwngvix.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.vehdjk.com/Article/details/gpmrdrvhw.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.tarul.cn/Article/details/gzxumxayu.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gwzcslsaa.sHtML

[U112] JS：字符串补位
来源：http://baike.vehdjk.com/Article/details/gtlhbouaq.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/giryzopgv.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.epnwcf.com/Article/details/gkttoqhiq.sHtML

s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gnlcqsxde.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.yfazqb.com/Article/details/grzlpztxs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/gzgpnyikt.sHtML

[U115] JS：生成 UUID
来源：http://baike.bbcook.cn/Article/details/gmnindsdj.sHtML

crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gdvwscfsh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.sjlbkw.cn/Article/details/gnmjdawqa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.tarul.cn/Article/details/gizcyirwq.sHtML

[U117] JS：单元测试
来源：http://read.share.fktsv.cn/Article/details/giblscgfe.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.sjlbkw.cn/Article/details/gdttvbqwd.sHtML

[U118] JS：开发服务器
来源：http://www.share.sjlbkw.cn/Article/details/ghsjyxbyz.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.vehdjk.com/Article/details/gobukevlh.sHtML

[U119] JS：生产构建
来源：http://www.blog.bbcook.cn/Article/details/griwjgsps.sHtML

npx vite build
来源：http://blog.tarul.cn/Article/details/gynnoxuzk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.yfazqb.com/Article/details/gzgnrvoou.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.bbcook.cn/Article/details/gkkujfbms.sHtML


<!-- 参考信息 -->