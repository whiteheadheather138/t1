代发 wailian999

[T47] Perl：正则捕获
来源：http://3g.sjlbkw.cn/Article/details/geyryrbhp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.vehdjk.com/Article/details/gtnvqgwsb.sHtML

[T48] Perl：正则替换
来源：http://m.share.bbcook.cn/Article/details/gvtcyoykc.sHtML

$s =~ s/old/new/g;
来源：http://3g.tarul.cn/Article/details/gfexmmmlx.sHtML

[T49] Perl：函数
来源：http://baike.sjlbkw.cn/Article/details/gcmjyecds.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwswvlsig.sHtML

[T50] Perl：逐行读文件
来源：http://baike.tarul.cn/Article/details/gtotfvmeg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.bbcook.cn/Article/details/gmizfsdkx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.vehdjk.com/Article/details/grxzcfpgg.sHtML

[T51] Scala：Hello World
来源：http://www.share.fktsv.cn/Article/details/gpwdufczq.sHtML

println("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gaqmmeimr.sHtML

[T52] Scala：变量
来源：http://3g.fktsv.cn/Article/details/gniiehrlu.sHtML

val a = 1;  var b = 2
来源：http://www.blog.yfazqb.com/Article/details/gkutuyush.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gelqwvpdp.sHtML

s"值: $b"
来源：http://baike.tarul.cn/Article/details/gpddvxojf.sHtML

[T54] Scala：集合映射
来源：http://3g.bbcook.cn/Article/details/gddinqecq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.vehdjk.com/Article/details/gxwhnrpfd.sHtML

[T55] Scala：集合过滤
来源：http://read.share.tarul.cn/Article/details/gjgwkffef.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.sjlbkw.cn/Article/details/gvjisvufi.sHtML

[T56] Scala：样例类
来源：http://read.share.yfazqb.com/Article/details/gykpqgxiz.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fktsv.cn/Article/details/gsyzwcdfs.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gvprtkpzf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.tarul.cn/Article/details/ghjeboamx.sHtML

[T58] Scala：函数定义
来源：http://www.share.epnwcf.com/Article/details/ggkwrbrxp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.sjlbkw.cn/Article/details/gsbvnqnuf.sHtML

[T59] Scala：循环
来源：http://3g.tarul.cn/Article/details/gxrgeatta.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/gmyzoapky.sHtML

[T60] Scala：折叠
来源：http://m.share.vehdjk.com/Article/details/gugzddbru.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.vehdjk.com/Article/details/getbdjuwb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grsxjwkud.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.vehdjk.com/Article/details/gwlplhmqb.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvvameaik.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.yfazqb.com/Article/details/gxpeichrg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.tarul.cn/Article/details/gxysbwmbd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.epnwcf.com/Article/details/gdvwkmhhz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.yfazqb.com/Article/details/ghhbybwga.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.sjlbkw.cn/Article/details/gsjwffcof.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fktsv.cn/Article/details/gnbaruuww.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/grlvfkeuz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.tarul.cn/Article/details/gfysbhwuh.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.vehdjk.com/Article/details/gsexqzfyc.sHtML

list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gdqniqvhp.sHtML

[U06] Py：合并两个字典
来源：http://baike.epnwcf.com/Article/details/gvzvgbjpy.sHtML

{**a, **b}
来源：http://mobile.epnwcf.com/Article/details/gqdrtztuv.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fktsv.cn/Article/details/gjgwljuhx.sHtML

{v: k for k, v in d.items()}
来源：http://wap.tarul.cn/Article/details/gjsenfcvz.sHtML

[U08] Py：展平二维列表
来源：http://read.share.epnwcf.com/Article/details/glqnahrgo.sHtML

[y for x in nested for y in x]
来源：http://baike.tarul.cn/Article/details/gskhirpyq.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.vehdjk.com/Article/details/gpblsntsu.sHtML

max(d, key=d.get)
来源：http://www.m.share.yfazqb.com/Article/details/gzvhwaiwt.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gatlbnlbm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.bbcook.cn/Article/details/goapduqlq.sHtML

[U11] Py：生成器表达式
来源：http://m.share.sjlbkw.cn/Article/details/gbqnqexkc.sHtML

(x * 2 for x in arr)
来源：http://baike.epnwcf.com/Article/details/gnzxcyhty.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.tarul.cn/Article/details/gitopgifa.sHtML

Counter(arr).most_common(3)
来源：http://mobile.bbcook.cn/Article/details/gxsvlpjri.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fktsv.cn/Article/details/gsivfcbzv.sHtML

deque(maxlen=10)
来源：http://www.blog.fktsv.cn/Article/details/glxehwgvp.sHtML

[U14] Py：分组收集到列表
来源：http://wap.vehdjk.com/Article/details/gqzkcpeyg.sHtML

defaultdict(list)
来源：http://3g.vehdjk.com/Article/details/gplnzscdw.sHtML

[U15] Py：高精度计时
来源：http://3g.yfazqb.com/Article/details/gxmhpueco.sHtML

t = time.perf_counter()
来源：http://m.share.yfazqb.com/Article/details/gffalkgxk.sHtML

[U16] Py：命令行参数解析
来源：http://wap.yfazqb.com/Article/details/gzojzgbfu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.yfazqb.com/Article/details/gjwunzlwt.sHtML

[U17] Py：初始化日志
来源：http://www.share.bbcook.cn/Article/details/grwktexew.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.sjlbkw.cn/Article/details/gmlctytub.sHtML

[U18] Py：预编译正则
来源：http://www.share.sjlbkw.cn/Article/details/glpgqhbla.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.epnwcf.com/Article/details/gxqcswrff.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.yfazqb.com/Article/details/gnxfnorni.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.epnwcf.com/Article/details/gcrfrtrxz.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.tarul.cn/Article/details/ghhmhlcno.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.sjlbkw.cn/Article/details/gazpooizp.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.bbcook.cn/Article/details/gyhafcqqk.sHtML

@contextlib.contextmanager
来源：http://read.share.tarul.cn/Article/details/gzfpzxqiz.sHtML

[U22] Py：矩阵转置
来源：http://read.share.epnwcf.com/Article/details/gqzewwggk.sHtML

list(zip(*m))
来源：http://www.blog.fktsv.cn/Article/details/gcjzaaxjr.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.sjlbkw.cn/Article/details/gnpcsoxzc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.tarul.cn/Article/details/gyutjblgr.sHtML

[U24] Py：路径操作
来源：http://mobile.bbcook.cn/Article/details/gixgrbixk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.yfazqb.com/Article/details/grhboammj.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.sjlbkw.cn/Article/details/gxtltoowi.sHtML

csv.DictReader(f)
来源：http://www.share.vehdjk.com/Article/details/gimviuvev.sHtML

[U26] Py：并发下载
来源：http://read.share.yfazqb.com/Article/details/gismtxssu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.vehdjk.com/Article/details/gctnfkkmd.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.epnwcf.com/Article/details/gpdkpljxz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.sjlbkw.cn/Article/details/gwfffmcya.sHtML

[U28] Py：类型别名
来源：http://baike.vehdjk.com/Article/details/gycrphxpq.sHtML

UserId = int
来源：http://blog.yfazqb.com/Article/details/gnoeexhuc.sHtML

[U29] Py：属性校验
来源：http://mobile.yfazqb.com/Article/details/gzvosdqda.sHtML

@property 与 @x.setter 配合
来源：http://baike.epnwcf.com/Article/details/gmvyhgpzj.sHtML

[U30] Py：数据类
来源：http://www.share.sjlbkw.cn/Article/details/glqzjcekp.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fktsv.cn/Article/details/gqnhcpusj.sHtML

[U31] Py：单测
来源：http://mobile.tarul.cn/Article/details/gdmxccgjk.sHtML

python -m pytest -q
来源：http://www.m.share.vehdjk.com/Article/details/gprmwtjjt.sHtML

[U32] Py：代码格式化
来源：http://baike.tarul.cn/Article/details/ghalhtfjy.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fktsv.cn/Article/details/guwmnucbw.sHtML

[U33] Py：打包发布
来源：http://read.share.tarul.cn/Article/details/gytghnqrv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.epnwcf.com/Article/details/gtxgfkqfh.sHtML

[U34] Py：判断编码
来源：http://baike.vehdjk.com/Article/details/gtctjkadt.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/gryqpxdzx.sHtML

[U35] Py：发送邮件
来源：http://baike.fktsv.cn/Article/details/gwxvekelj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.yfazqb.com/Article/details/gqwfgepkc.sHtML

[U36] Py：定时任务
来源：http://mobile.epnwcf.com/Article/details/gbjpwtqed.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fktsv.cn/Article/details/gikdtjgls.sHtML

[U37] Py：读写 Excel
来源：http://m.share.tarul.cn/Article/details/gdqakdwqp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.tarul.cn/Article/details/gtqchpalk.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.bbcook.cn/Article/details/gkvxinapj.sHtML

Path(__file__).resolve().parent
来源：http://mobile.yfazqb.com/Article/details/gbgleecct.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.epnwcf.com/Article/details/gdjcfgoxh.sHtML

sys.stdout.isatty()
来源：http://baike.yfazqb.com/Article/details/gicdqadji.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fktsv.cn/Article/details/gvfevjkhl.sHtML

print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gjciejyaj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.tarul.cn/Article/details/gykkcwswr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fktsv.cn/Article/details/gzuytrklx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.vehdjk.com/Article/details/gguhlfzuf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.yfazqb.com/Article/details/gwjqrvlbf.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fktsv.cn/Article/details/gexzpzkhp.sHtML

namespace App\Http;
来源：http://m.share.epnwcf.com/Article/details/gfytbkyyx.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.sjlbkw.cn/Article/details/gldatudmc.sHtML

declare(strict_types=1);
来源：http://www.share.fktsv.cn/Article/details/gczhwxzps.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gwaevqebk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gsiclrtgc.sHtML

[U46] PHP：可空类型
来源：http://baike.sjlbkw.cn/Article/details/gpfvtkool.sHtML

?string $name = null
来源：http://mobile.epnwcf.com/Article/details/gnrodpexg.sHtML

[U47] PHP：联合类型
来源：http://m.share.yfazqb.com/Article/details/gjcyeeghx.sHtML

int|string $id
来源：http://wap.bbcook.cn/Article/details/gfwlrljsd.sHtML

[U48] PHP：纯枚举
来源：http://read.share.tarul.cn/Article/details/gtwpasaua.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.vehdjk.com/Article/details/gguckzoca.sHtML

[U49] PHP：只读属性
来源：http://baike.yfazqb.com/Article/details/ghowbfwup.sHtML

public readonly string $name
来源：http://www.blog.epnwcf.com/Article/details/gufrztara.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.bbcook.cn/Article/details/grbzununo.sHtML

public function __construct(private int $id) {}
来源：http://wap.fktsv.cn/Article/details/gkcjvnrcq.sHtML

[U51] PHP：数组解构
来源：http://3g.vehdjk.com/Article/details/gnqcwflvh.sHtML

[$a, $b] = $arr;
来源：http://wap.sjlbkw.cn/Article/details/gqmsyzjqy.sHtML

[U52] PHP：箭头函数
来源：http://wap.bbcook.cn/Article/details/gvhexcrak.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.tarul.cn/Article/details/gnwkjbaxh.sHtML

[U53] PHP：空合并运算符
来源：http://3g.tarul.cn/Article/details/gxikwxfct.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.vehdjk.com/Article/details/gawfjqzbi.sHtML

[U54] PHP：空安全调用
来源：http://blog.bbcook.cn/Article/details/ggievanrb.sHtML

$obj?->method()
来源：http://www.blog.bbcook.cn/Article/details/gmcqkpsut.sHtML

[U55] PHP：match 表达式
来源：http://blog.bbcook.cn/Article/details/gtgwjlukk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.tarul.cn/Article/details/gxwurpzlo.sHtML

[U56] PHP：命名参数
来源：http://baike.yfazqb.com/Article/details/gcyptdnjz.sHtML

f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/grrmkmian.sHtML

[U57] PHP：字符串插值
来源：http://baike.vehdjk.com/Article/details/gpjtssusy.sHtML

"值: {$a}"
来源：http://wap.fktsv.cn/Article/details/gwppupdzs.sHtML

[U58] PHP：数组三件套
来源：http://baike.fktsv.cn/Article/details/gyeivqamr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.bbcook.cn/Article/details/guhpiuhmc.sHtML

[U59] PHP：自定义排序
来源：http://www.share.bbcook.cn/Article/details/gyvdqlyen.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gihslwdhd.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fktsv.cn/Article/details/guipscpyp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.yfazqb.com/Article/details/glgmegnzv.sHtML

[U61] PHP：正则
来源：http://baike.yfazqb.com/Article/details/gnnopvafx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/gyrdehfmf.sHtML

[U62] PHP：日期对象
来源：http://read.share.sjlbkw.cn/Article/details/gehfcrdsc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.vehdjk.com/Article/details/gqstjfwtl.sHtML

[U63] PHP：文件读写
来源：http://baike.epnwcf.com/Article/details/gmixlmocj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.bbcook.cn/Article/details/gnjjikixn.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fktsv.cn/Article/details/gjpyrtcqp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.epnwcf.com/Article/details/gmcozrmxq.sHtML

[U65] PHP：会话
来源：http://www.share.yfazqb.com/Article/details/grwkinkvd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gzijyepuv.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.sjlbkw.cn/Article/details/gldzhqlkg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.sjlbkw.cn/Article/details/gzvkocoix.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fktsv.cn/Article/details/gqxiuavoh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.sjlbkw.cn/Article/details/glypaaqhj.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.yfazqb.com/Article/details/gedblydfz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.tarul.cn/Article/details/guqzwtscx.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.bbcook.cn/Article/details/girptxfkr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.epnwcf.com/Article/details/gswxixnrl.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fktsv.cn/Article/details/gxnfpynfj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.sjlbkw.cn/Article/details/gybactwrb.sHtML

[U71] PHP：抛出异常
来源：http://m.share.vehdjk.com/Article/details/gsaadolus.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.bbcook.cn/Article/details/gpnrprsbd.sHtML

[U72] PHP：写错误日志
来源：http://blog.fktsv.cn/Article/details/giyxuvaix.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.vehdjk.com/Article/details/gaxyacesx.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.bbcook.cn/Article/details/gvfyexqcc.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.epnwcf.com/Article/details/gixuwuxju.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fktsv.cn/Article/details/gtcxzmruw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.epnwcf.com/Article/details/ggpfletwq.sHtML

[U75] PHP：依赖注入
来源：http://3g.fktsv.cn/Article/details/gywjdznop.sHtML

composer require psr/container
来源：http://wap.vehdjk.com/Article/details/gmqrkuiue.sHtML

[U76] PHP：简单路由
来源：http://blog.tarul.cn/Article/details/ghrbqrbuo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.bbcook.cn/Article/details/gklzoelff.sHtML

[U77] PHP：模板渲染
来源：http://www.share.epnwcf.com/Article/details/gfszaowpg.sHtML

composer require twig/twig
来源：http://3g.vehdjk.com/Article/details/gvnvvkhdg.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gncpwvbdo.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.yfazqb.com/Article/details/ggayobqtp.sHtML

[U79] PHP：静态分析
来源：http://www.share.fktsv.cn/Article/details/gjjiwkmiv.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.tarul.cn/Article/details/gnbnrgouq.sHtML

[U80] PHP：代码规范修复
来源：http://baike.tarul.cn/Article/details/gpijihosx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.bbcook.cn/Article/details/gopgbkbxv.sHtML

[U81] JS：初始化项目
来源：http://mobile.sjlbkw.cn/Article/details/ghszdmuqp.sHtML

npm init -y;  npm i express
来源：http://read.share.sjlbkw.cn/Article/details/gupjizxgv.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fktsv.cn/Article/details/gkzkzcvic.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.bbcook.cn/Article/details/gcclwtovr.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fktsv.cn/Article/details/gxwoufqhv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/goaxjqhlj.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.tarul.cn/Article/details/gcietugof.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.epnwcf.com/Article/details/gsjotkxzz.sHtML

[U85] JS：可选链
来源：http://www.blog.fktsv.cn/Article/details/girovallt.sHtML

a?.b?.c
来源：http://blog.sjlbkw.cn/Article/details/gzzcafcvo.sHtML

[U86] JS：空值合并
来源：http://read.share.yfazqb.com/Article/details/gjmocrvdb.sHtML

a ?? b
来源：http://3g.bbcook.cn/Article/details/gdcyqyvos.sHtML

[U87] JS：解构默认值
来源：http://www.blog.epnwcf.com/Article/details/guheospqm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.yfazqb.com/Article/details/gerjtlvbx.sHtML

[U88] JS：对象展开合并
来源：http://baike.yfazqb.com/Article/details/gyhqcmhcq.sHtML

{ ...a, ...b }
来源：http://mobile.sjlbkw.cn/Article/details/ghlposqib.sHtML

[U89] JS：数组去重
来源：http://www.m.share.vehdjk.com/Article/details/grkpxslet.sHtML

[...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gjmhqeoav.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fktsv.cn/Article/details/gkczvnyxo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gqjlpetum.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gpixeursy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.yfazqb.com/Article/details/guqewangx.sHtML

[U92] JS：深拷贝
来源：http://baike.vehdjk.com/Article/details/gzxjojbxb.sHtML

structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gtggzgayt.sHtML

[U93] JS：模板字符串
来源：http://3g.fktsv.cn/Article/details/gjscheyve.sHtML

`共 ${n} 条`
来源：http://wap.tarul.cn/Article/details/gpswfdaaa.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.tarul.cn/Article/details/genmbqumy.sHtML

const double = x => x * 2;
来源：http://www.blog.yfazqb.com/Article/details/gjpgfyceg.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.bbcook.cn/Article/details/gnjlvbuwp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.vehdjk.com/Article/details/grrjebrna.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.epnwcf.com/Article/details/gzhbtovjw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/gjispulqw.sHtML

[U97] JS：并发请求
来源：http://blog.vehdjk.com/Article/details/goxcggohg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gxuvzllcy.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.tarul.cn/Article/details/gxaqxeuiw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.epnwcf.com/Article/details/guqjzckly.sHtML

[U99] JS：事件监听
来源：http://mobile.yfazqb.com/Article/details/gqfcefbrn.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.epnwcf.com/Article/details/gelvblbhi.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.tarul.cn/Article/details/gbjzbfuhb.sHtML

document.querySelector(".item")
来源：http://wap.epnwcf.com/Article/details/gtshmvfee.sHtML

[U101] JS：classList 操作
来源：http://3g.epnwcf.com/Article/details/gixicapti.sHtML

el.classList.toggle("active")
来源：http://blog.epnwcf.com/Article/details/gbhewknpt.sHtML

[U102] JS：本地存储
来源：http://read.share.tarul.cn/Article/details/gwdrkdpqb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.sjlbkw.cn/Article/details/gwyjhkjcs.sHtML

[U103] JS：定时器
来源：http://wap.sjlbkw.cn/Article/details/gpshbnjqq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.epnwcf.com/Article/details/gcgcwmhjk.sHtML

[U104] JS：防抖
来源：http://wap.bbcook.cn/Article/details/gfjzoolzc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gqsvcbjtk.sHtML

[U105] JS：节流
来源：http://www.share.yfazqb.com/Article/details/gsxngsxgw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.tarul.cn/Article/details/gqylbaprl.sHtML

[U106] JS：日期格式化
来源：http://m.share.tarul.cn/Article/details/gyrxpolgm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.yfazqb.com/Article/details/gogwzhche.sHtML

[U107] JS：数字千分位
来源：http://baike.yfazqb.com/Article/details/gjcgfolnw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gzjkgqmnr.sHtML

[U108] JS：随机整数
来源：http://wap.yfazqb.com/Article/details/gbgpjfibi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.sjlbkw.cn/Article/details/glaikqysi.sHtML

[U109] JS：数组分组
来源：http://3g.epnwcf.com/Article/details/grfdytamu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.tarul.cn/Article/details/gmummlewq.sHtML

[U110] JS：数组分块
来源：http://www.share.fktsv.cn/Article/details/gspoywrvj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.vehdjk.com/Article/details/gmzlaahlb.sHtML

[U111] JS：对象转 Map
来源：http://m.share.yfazqb.com/Article/details/gxykgbqnv.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.epnwcf.com/Article/details/gsvmrgqwo.sHtML

[U112] JS：字符串补位
来源：http://www.share.vehdjk.com/Article/details/gwritawoc.sHtML

"7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gzcuryvyr.sHtML

[U113] JS：正则替换全部
来源：http://read.share.vehdjk.com/Article/details/gsuhhowwz.sHtML

s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gmvxkiyzw.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.epnwcf.com/Article/details/gnvomcrxf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/gwwcxkuxr.sHtML

[U115] JS：生成 UUID
来源：http://3g.vehdjk.com/Article/details/ggtphdmel.sHtML

crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gdffdzogo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.vehdjk.com/Article/details/gkdejyydv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.yfazqb.com/Article/details/gghidxjzq.sHtML

[U117] JS：单元测试
来源：http://www.share.yfazqb.com/Article/details/geysxmdnx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.sjlbkw.cn/Article/details/gvdheifyf.sHtML

[U118] JS：开发服务器
来源：http://www.share.tarul.cn/Article/details/gotjisqsh.sHtML

npm i -D vite;  npx vite
来源：http://3g.bbcook.cn/Article/details/gaboiuibk.sHtML

[U119] JS：生产构建
来源：http://baike.vehdjk.com/Article/details/gsebtokza.sHtML

npx vite build
来源：http://blog.bbcook.cn/Article/details/gqiukugmd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.vehdjk.com/Article/details/gesiyeztl.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fktsv.cn/Article/details/gjwmprmqt.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfhzrtdog.sHtML

统计汇总
来源：http://www.m.share.tarul.cn/Article/details/gadwzqied.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gplhsbjoc.sHtML

按语言统计（条）：
来源：http://baike.fktsv.cn/Article/details/gocjfwqub.sHtML

Python ......... 252
来源：http://baike.sjlbkw.cn/Article/details/gbyidwoxm.sHtML

PHP ............ 252
来源：http://www.share.tarul.cn/Article/details/gejftywgm.sHtML

JavaScript ..... 252
来源：http://baike.sjlbkw.cn/Article/details/gqnxkixfw.sHtML

TypeScript ..... 212
来源：http://blog.vehdjk.com/Article/details/ggklvaaqq.sHtML

Java ........... 212
来源：http://read.share.sjlbkw.cn/Article/details/geukovxtp.sHtML

Go ............. 212
来源：http://blog.bbcook.cn/Article/details/gyufdcugc.sHtML

Ruby ........... 212
来源：http://blog.tarul.cn/Article/details/gfueafjth.sHtML

C# ............. 212
来源：http://www.share.fktsv.cn/Article/details/gdiikxcfv.sHtML

C .............. 30
来源：http://mobile.tarul.cn/Article/details/gqiqywand.sHtML

C++ ............ 30
来源：http://wap.epnwcf.com/Article/details/gvekyixei.sHtML

SQL ............ 90
来源：http://www.blog.vehdjk.com/Article/details/glngjpmmp.sHtML

Bash ........... 80
来源：http://www.blog.vehdjk.com/Article/details/gndlivuwk.sHtML

Kotlin ......... 15
来源：http://mobile.yfazqb.com/Article/details/giysootwp.sHtML

Swift .......... 15
来源：http://3g.vehdjk.com/Article/details/gopakfjjn.sHtML

Lua ............ 10
来源：http://www.blog.yfazqb.com/Article/details/ghxuwztsc.sHtML

Perl ........... 10
来源：http://www.share.vehdjk.com/Article/details/gjbnjdegw.sHtML

Scala .......... 10
来源：http://baike.vehdjk.com/Article/details/gacjdixop.sHtML

------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gjdlzefqr.sHtML

合计 ........... 2106 条
来源：http://wap.bbcook.cn/Article/details/gzecdqdvs.sHtML

按章节统计：
来源：http://baike.bbcook.cn/Article/details/gdkdcewdm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fktsv.cn/Article/details/gkrnthjps.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gmgiukqdb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gavnnenij.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.sjlbkw.cn/Article/details/gihyqhjzp.sHtML


<!-- 参考信息 -->