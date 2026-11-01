代发 wailian999

[T49] Perl：函数
来源：http://mobile.epnwcf.com/Article/details/gydqpfnxt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gpznlbvmi.sHtML

[T50] Perl：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gjvxlkbbd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.epnwcf.com/Article/details/gyiaoyziw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fktsv.cn/Article/details/gsxzyrosx.sHtML

[T51] Scala：Hello World
来源：http://read.share.tarul.cn/Article/details/gemtfvidf.sHtML

println("Hello")
来源：http://blog.bbcook.cn/Article/details/gcbigslgh.sHtML

[T52] Scala：变量
来源：http://www.m.share.bbcook.cn/Article/details/gpraooyfe.sHtML

val a = 1;  var b = 2
来源：http://mobile.tarul.cn/Article/details/gtbvatvng.sHtML

[T53] Scala：字符串插值
来源：http://baike.vehdjk.com/Article/details/geqrexpid.sHtML

s"值: $b"
来源：http://www.share.vehdjk.com/Article/details/gtneowzse.sHtML

[T54] Scala：集合映射
来源：http://3g.vehdjk.com/Article/details/gswrphiln.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.sjlbkw.cn/Article/details/gdytoufyi.sHtML

[T55] Scala：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/glfwpdloy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.vehdjk.com/Article/details/goaakvqmr.sHtML

[T56] Scala：样例类
来源：http://mobile.yfazqb.com/Article/details/gamhbrwdv.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.yfazqb.com/Article/details/ghastmfte.sHtML

[T57] Scala：模式匹配
来源：http://blog.epnwcf.com/Article/details/gzobmwnzz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.tarul.cn/Article/details/guwfeesge.sHtML

[T58] Scala：函数定义
来源：http://blog.yfazqb.com/Article/details/geepakhkn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.epnwcf.com/Article/details/gzuemhgxr.sHtML

[T59] Scala：循环
来源：http://wap.sjlbkw.cn/Article/details/gfjesfxqn.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.vehdjk.com/Article/details/gzlrbpemd.sHtML

[T60] Scala：折叠
来源：http://blog.vehdjk.com/Article/details/gnlnalvcb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.epnwcf.com/Article/details/gdjpvvcdy.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gnyohwyjt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.epnwcf.com/Article/details/gruzgtgya.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/geavnuveb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.yfazqb.com/Article/details/gfwsspgwy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.epnwcf.com/Article/details/gijgmnxhk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.vehdjk.com/Article/details/gfaumqtzp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.bbcook.cn/Article/details/gtrnigjaj.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fktsv.cn/Article/details/gyweeayys.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fktsv.cn/Article/details/gzdplfeib.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvdonrpg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.tarul.cn/Article/details/gucxkrhxi.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.epnwcf.com/Article/details/gecbesdts.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gugymuntm.sHtML

[U06] Py：合并两个字典
来源：http://blog.fktsv.cn/Article/details/gabyxgkqq.sHtML

{**a, **b}
来源：http://m.share.epnwcf.com/Article/details/gghxdihqq.sHtML

[U07] Py：反转字典键值
来源：http://mobile.tarul.cn/Article/details/gvchvqihv.sHtML

{v: k for k, v in d.items()}
来源：http://3g.tarul.cn/Article/details/gxrmpdomt.sHtML

[U08] Py：展平二维列表
来源：http://wap.fktsv.cn/Article/details/gplznpaio.sHtML

[y for x in nested for y in x]
来源：http://mobile.tarul.cn/Article/details/gjasnuyff.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fktsv.cn/Article/details/gnbftohim.sHtML

max(d, key=d.get)
来源：http://mobile.tarul.cn/Article/details/grdiygtrr.sHtML

[U10] Py：按值排序字典
来源：http://wap.tarul.cn/Article/details/gqdyizfbp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.vehdjk.com/Article/details/gspviezjc.sHtML

[U11] Py：生成器表达式
来源：http://wap.tarul.cn/Article/details/gbitcuutt.sHtML

(x * 2 for x in arr)
来源：http://mobile.bbcook.cn/Article/details/gddvcbstg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.bbcook.cn/Article/details/gmzpfodyb.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.vehdjk.com/Article/details/gamxvymbv.sHtML

[U13] Py：固定长度队列
来源：http://mobile.vehdjk.com/Article/details/ghxfjwidl.sHtML

deque(maxlen=10)
来源：http://www.share.bbcook.cn/Article/details/gjutifgtq.sHtML

[U14] Py：分组收集到列表
来源：http://wap.tarul.cn/Article/details/gkthjiqsy.sHtML

defaultdict(list)
来源：http://www.m.share.tarul.cn/Article/details/gszgimfzw.sHtML

[U15] Py：高精度计时
来源：http://3g.vehdjk.com/Article/details/gsscjamyw.sHtML

t = time.perf_counter()
来源：http://read.share.tarul.cn/Article/details/gzrlhbvgn.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fktsv.cn/Article/details/gvwhuvbhn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.vehdjk.com/Article/details/gjdacffza.sHtML

[U17] Py：初始化日志
来源：http://www.share.vehdjk.com/Article/details/gtwidbjdy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.yfazqb.com/Article/details/ggpvcnhch.sHtML

[U18] Py：预编译正则
来源：http://mobile.sjlbkw.cn/Article/details/ghwldpvnz.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.vehdjk.com/Article/details/gkridlxay.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.epnwcf.com/Article/details/gvqrkpdum.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.sjlbkw.cn/Article/details/gbbhzdpgx.sHtML

[U20] Py：缓存函数结果
来源：http://wap.epnwcf.com/Article/details/ggnfiwcjm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.tarul.cn/Article/details/gaqvcboac.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fktsv.cn/Article/details/geepbylwy.sHtML

@contextlib.contextmanager
来源：http://mobile.fktsv.cn/Article/details/guyetghqk.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.vehdjk.com/Article/details/ggwvggnbr.sHtML

list(zip(*m))
来源：http://3g.bbcook.cn/Article/details/gznpopzay.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.vehdjk.com/Article/details/gebjfqmsq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.tarul.cn/Article/details/gegsofoha.sHtML

[U24] Py：路径操作
来源：http://3g.epnwcf.com/Article/details/gklrqffof.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.yfazqb.com/Article/details/gmszokxij.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.tarul.cn/Article/details/gfmqncdjn.sHtML

csv.DictReader(f)
来源：http://3g.epnwcf.com/Article/details/gbsuoapog.sHtML

[U26] Py：并发下载
来源：http://3g.vehdjk.com/Article/details/gxftnnift.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.tarul.cn/Article/details/gwczegdmu.sHtML

[U27] Py：异步 HTTP
来源：http://baike.vehdjk.com/Article/details/gvnwcwgye.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fktsv.cn/Article/details/grrbsftep.sHtML

[U28] Py：类型别名
来源：http://blog.yfazqb.com/Article/details/gdkhfqhgd.sHtML

UserId = int
来源：http://m.share.bbcook.cn/Article/details/gakwtgyaa.sHtML

[U29] Py：属性校验
来源：http://blog.vehdjk.com/Article/details/gqlgynvjn.sHtML

@property 与 @x.setter 配合
来源：http://3g.sjlbkw.cn/Article/details/gaiaspwfm.sHtML

[U30] Py：数据类
来源：http://www.blog.vehdjk.com/Article/details/gtqswntjf.sHtML

@dataclass(slots=True)
来源：http://m.share.tarul.cn/Article/details/glguncjtn.sHtML

[U31] Py：单测
来源：http://m.share.yfazqb.com/Article/details/gliqpqdam.sHtML

python -m pytest -q
来源：http://mobile.yfazqb.com/Article/details/ggdrmwwtu.sHtML

[U32] Py：代码格式化
来源：http://m.share.epnwcf.com/Article/details/gditnbgkr.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.vehdjk.com/Article/details/gelqtcnda.sHtML

[U33] Py：打包发布
来源：http://wap.vehdjk.com/Article/details/gyfkyderb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.bbcook.cn/Article/details/gguwcpbgx.sHtML

[U34] Py：判断编码
来源：http://www.m.share.vehdjk.com/Article/details/gtgqgqylc.sHtML

chardet.detect(raw)
来源：http://blog.sjlbkw.cn/Article/details/gzqhxpute.sHtML

[U35] Py：发送邮件
来源：http://www.share.sjlbkw.cn/Article/details/gmkvwybar.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.bbcook.cn/Article/details/ghdmzxdza.sHtML

[U36] Py：定时任务
来源：http://www.blog.vehdjk.com/Article/details/gweveyleg.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.yfazqb.com/Article/details/gzmmbnukp.sHtML

[U37] Py：读写 Excel
来源：http://mobile.bbcook.cn/Article/details/glxeefnch.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.vehdjk.com/Article/details/gpeyygnlp.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.vehdjk.com/Article/details/gkthwygfi.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.yfazqb.com/Article/details/gekmmkuvw.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.epnwcf.com/Article/details/gljqmdbnl.sHtML

sys.stdout.isatty()
来源：http://m.share.tarul.cn/Article/details/ganolizgc.sHtML

[U40] Py：打印到标准错误
来源：http://blog.bbcook.cn/Article/details/gyfrbkbww.sHtML

print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/gvslzmhvg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fktsv.cn/Article/details/gjogyuezk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/gslyiowey.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.epnwcf.com/Article/details/gylfkyoiu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.vehdjk.com/Article/details/gqirgozgc.sHtML

[U43] PHP：声明命名空间
来源：http://3g.vehdjk.com/Article/details/gswlnyaca.sHtML

namespace App\Http;
来源：http://mobile.bbcook.cn/Article/details/gjkktobde.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.bbcook.cn/Article/details/gkpszkdeq.sHtML

declare(strict_types=1);
来源：http://read.share.vehdjk.com/Article/details/gytaxoxdx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.sjlbkw.cn/Article/details/gosyfxcwt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gshaspexn.sHtML

[U46] PHP：可空类型
来源：http://www.share.fktsv.cn/Article/details/gdqooiqla.sHtML

?string $name = null
来源：http://3g.vehdjk.com/Article/details/gcjagortp.sHtML

[U47] PHP：联合类型
来源：http://m.share.fktsv.cn/Article/details/gbnrxnaxe.sHtML

int|string $id
来源：http://3g.tarul.cn/Article/details/gntmqhgys.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.sjlbkw.cn/Article/details/ghdxutwqo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.epnwcf.com/Article/details/gnnlwcxfs.sHtML

[U49] PHP：只读属性
来源：http://www.blog.vehdjk.com/Article/details/gzdoknynx.sHtML

public readonly string $name
来源：http://wap.yfazqb.com/Article/details/gbhimmdrc.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.sjlbkw.cn/Article/details/gxjvbrjts.sHtML

public function __construct(private int $id) {}
来源：http://read.share.yfazqb.com/Article/details/gukeevwtf.sHtML

[U51] PHP：数组解构
来源：http://www.blog.sjlbkw.cn/Article/details/gmfvjlvus.sHtML

[$a, $b] = $arr;
来源：http://blog.yfazqb.com/Article/details/gbctekapm.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gisdrhgxn.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.vehdjk.com/Article/details/gykyugxhg.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.tarul.cn/Article/details/giqshetdc.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fktsv.cn/Article/details/ggwykgwqb.sHtML

[U54] PHP：空安全调用
来源：http://wap.yfazqb.com/Article/details/glfkvikrw.sHtML

$obj?->method()
来源：http://m.share.yfazqb.com/Article/details/glfdmmskm.sHtML

[U55] PHP：match 表达式
来源：http://www.share.yfazqb.com/Article/details/gufoqqfbn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.tarul.cn/Article/details/ggpjmxrcq.sHtML

[U56] PHP：命名参数
来源：http://3g.vehdjk.com/Article/details/gyubyhrsg.sHtML

f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/galivcbxt.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gypxslsdu.sHtML

"值: {$a}"
来源：http://www.share.epnwcf.com/Article/details/ghpocorwo.sHtML

[U58] PHP：数组三件套
来源：http://3g.epnwcf.com/Article/details/gqyfywdeq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.tarul.cn/Article/details/ghzydslnp.sHtML

[U59] PHP：自定义排序
来源：http://blog.tarul.cn/Article/details/gzshnwbok.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/glyynlwlo.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.sjlbkw.cn/Article/details/grvhbtemu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.yfazqb.com/Article/details/gqztifhpa.sHtML

[U61] PHP：正则
来源：http://blog.bbcook.cn/Article/details/grmllkzax.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/gdywbmbji.sHtML

[U62] PHP：日期对象
来源：http://read.share.yfazqb.com/Article/details/gozyyxkbn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/gomrclejf.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.yfazqb.com/Article/details/gebqohxjo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.vehdjk.com/Article/details/grwgessbd.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.vehdjk.com/Article/details/glvqviqfj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.yfazqb.com/Article/details/gxxqyyhvo.sHtML

[U65] PHP：会话
来源：http://read.share.sjlbkw.cn/Article/details/gnhapkchg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/getppwkvf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fktsv.cn/Article/details/gyvmefrin.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.yfazqb.com/Article/details/gwuakfirk.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.sjlbkw.cn/Article/details/gigabecvv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.tarul.cn/Article/details/gwpxpiwse.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.epnwcf.com/Article/details/gzkbldvig.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.epnwcf.com/Article/details/gtwydyqru.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.yfazqb.com/Article/details/gqmvaciqp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.yfazqb.com/Article/details/gyrnmilsg.sHtML

[U70] PHP：PDO 事务
来源：http://baike.epnwcf.com/Article/details/gwzwkwerk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.sjlbkw.cn/Article/details/gjmsxcbcj.sHtML

[U71] PHP：抛出异常
来源：http://mobile.bbcook.cn/Article/details/gotpoozva.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.yfazqb.com/Article/details/gzxcemjxe.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.bbcook.cn/Article/details/gpqonkybr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.yfazqb.com/Article/details/glssjswby.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.bbcook.cn/Article/details/guqsuouqx.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.epnwcf.com/Article/details/gxgnqvtai.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.epnwcf.com/Article/details/gvtaohywt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.yfazqb.com/Article/details/gcrvuxczs.sHtML

[U75] PHP：依赖注入
来源：http://mobile.epnwcf.com/Article/details/gziscrfkv.sHtML

composer require psr/container
来源：http://www.m.share.yfazqb.com/Article/details/glvwdwzcb.sHtML

[U76] PHP：简单路由
来源：http://www.share.yfazqb.com/Article/details/gwydcelty.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.yfazqb.com/Article/details/govkzciad.sHtML

[U77] PHP：模板渲染
来源：http://read.share.epnwcf.com/Article/details/gydmcqcbi.sHtML

composer require twig/twig
来源：http://baike.bbcook.cn/Article/details/gkqvlwstv.sHtML

[U78] PHP：单元测试
来源：http://wap.epnwcf.com/Article/details/gtxrdwfln.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.epnwcf.com/Article/details/grdwsklqc.sHtML

[U79] PHP：静态分析
来源：http://read.share.yfazqb.com/Article/details/gozgtgokt.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fktsv.cn/Article/details/gtdmdlffb.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.bbcook.cn/Article/details/ggiihjrhm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fktsv.cn/Article/details/gcamwoskl.sHtML

[U81] JS：初始化项目
来源：http://m.share.tarul.cn/Article/details/ghmalwdri.sHtML

npm init -y;  npm i express
来源：http://blog.tarul.cn/Article/details/gejygkkcl.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.sjlbkw.cn/Article/details/gvdhcgqhb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.yfazqb.com/Article/details/gaucuvdth.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.sjlbkw.cn/Article/details/gydneruuo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gwkrmfzcq.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.bbcook.cn/Article/details/gsymauvon.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.bbcook.cn/Article/details/gmnbxvefv.sHtML

[U85] JS：可选链
来源：http://m.share.yfazqb.com/Article/details/gvujxoukl.sHtML

a?.b?.c
来源：http://www.share.yfazqb.com/Article/details/ghqmcydgr.sHtML

[U86] JS：空值合并
来源：http://mobile.epnwcf.com/Article/details/ghxczslqy.sHtML

a ?? b
来源：http://baike.epnwcf.com/Article/details/gpcutaotw.sHtML

[U87] JS：解构默认值
来源：http://www.blog.yfazqb.com/Article/details/gmikoifon.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fktsv.cn/Article/details/gtnnyvcce.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.yfazqb.com/Article/details/gwihdfexa.sHtML

{ ...a, ...b }
来源：http://www.blog.tarul.cn/Article/details/giipsifum.sHtML

[U89] JS：数组去重
来源：http://m.share.vehdjk.com/Article/details/gmsinoerb.sHtML

[...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/giohozaod.sHtML

[U90] JS：数字数组排序
来源：http://www.share.bbcook.cn/Article/details/gjgvpekiv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gqkclyyem.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.epnwcf.com/Article/details/gddseohfm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.tarul.cn/Article/details/gmnpfdeqw.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gunbkmgyh.sHtML

structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gopqzfyot.sHtML

[U93] JS：模板字符串
来源：http://wap.bbcook.cn/Article/details/ghcrgrrwl.sHtML

`共 ${n} 条`
来源：http://www.m.share.tarul.cn/Article/details/gtxxamtsb.sHtML

[U94] JS：箭头函数
来源：http://mobile.sjlbkw.cn/Article/details/gkwiwnpsj.sHtML

const double = x => x * 2;
来源：http://read.share.fktsv.cn/Article/details/gtpzdlyai.sHtML

[U95] JS：Promise 包装
来源：http://mobile.vehdjk.com/Article/details/gbnfqwjqa.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.sjlbkw.cn/Article/details/gwymfsfvt.sHtML

[U96] JS：async/await 与异常
来源：http://blog.epnwcf.com/Article/details/ghbykkxuc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gnzzbgrmz.sHtML

[U97] JS：并发请求
来源：http://baike.vehdjk.com/Article/details/gitairbmd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/glhqdzbvt.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.tarul.cn/Article/details/gqoapbhsk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.tarul.cn/Article/details/gyipdxlfc.sHtML

[U99] JS：事件监听
来源：http://www.m.share.yfazqb.com/Article/details/gomiltdhc.sHtML

el.addEventListener("click", e => {})
来源：http://wap.tarul.cn/Article/details/gchnrtavm.sHtML

[U100] JS：DOM 查询
来源：http://blog.tarul.cn/Article/details/gntemvsvn.sHtML

document.querySelector(".item")
来源：http://blog.epnwcf.com/Article/details/gyfbuvgxj.sHtML

[U101] JS：classList 操作
来源：http://www.share.sjlbkw.cn/Article/details/gbtefqnzk.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fktsv.cn/Article/details/gklevzuun.sHtML

[U102] JS：本地存储
来源：http://blog.vehdjk.com/Article/details/gyvoifpir.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.yfazqb.com/Article/details/gwvlhjjbw.sHtML

[U103] JS：定时器
来源：http://baike.vehdjk.com/Article/details/gfjhkdtsv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.yfazqb.com/Article/details/gstppjjjc.sHtML

[U104] JS：防抖
来源：http://3g.vehdjk.com/Article/details/gcyvmqdsz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gpjevkasi.sHtML

[U105] JS：节流
来源：http://www.blog.vehdjk.com/Article/details/geujvapfk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fktsv.cn/Article/details/gsnhljvay.sHtML

[U106] JS：日期格式化
来源：http://3g.vehdjk.com/Article/details/gecvcmldc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fktsv.cn/Article/details/glywcogvl.sHtML

[U107] JS：数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/goilwrobj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/gkyfgodvh.sHtML

[U108] JS：随机整数
来源：http://www.share.vehdjk.com/Article/details/gdylnvaeh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.vehdjk.com/Article/details/gbcnywzfg.sHtML

[U109] JS：数组分组
来源：http://3g.vehdjk.com/Article/details/grhgetghm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/gyfixkyfs.sHtML

[U110] JS：数组分块
来源：http://read.share.sjlbkw.cn/Article/details/gtrbynqbn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.tarul.cn/Article/details/gavebpihx.sHtML

[U111] JS：对象转 Map
来源：http://blog.yfazqb.com/Article/details/glzyroxar.sHtML

new Map(Object.entries(obj))
来源：http://read.share.yfazqb.com/Article/details/gpfyecmvx.sHtML

[U112] JS：字符串补位
来源：http://www.share.tarul.cn/Article/details/gbdmyytyq.sHtML

"7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gizuglylg.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.vehdjk.com/Article/details/gfwartdlz.sHtML

s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gpnhtntgk.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.vehdjk.com/Article/details/ghxhlpwve.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.epnwcf.com/Article/details/gthdjhrni.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/guetmbylj.sHtML

crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gqhysswut.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fktsv.cn/Article/details/galjoxbch.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.tarul.cn/Article/details/gyynpcnqs.sHtML

[U117] JS：单元测试
来源：http://www.blog.bbcook.cn/Article/details/gdwnxaerx.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.vehdjk.com/Article/details/gdjbktdoj.sHtML

[U118] JS：开发服务器
来源：http://www.share.sjlbkw.cn/Article/details/ggihogesq.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.bbcook.cn/Article/details/ggtkrknec.sHtML

[U119] JS：生产构建
来源：http://mobile.bbcook.cn/Article/details/gspxudazw.sHtML

npx vite build
来源：http://3g.vehdjk.com/Article/details/guevuiwol.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.yfazqb.com/Article/details/gtbcbhcom.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.vehdjk.com/Article/details/gjljcrjkd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gigdmgzdz.sHtML

统计汇总
来源：http://blog.fktsv.cn/Article/details/gzoulesxt.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gybntyzev.sHtML

按语言统计（条）：
来源：http://www.blog.sjlbkw.cn/Article/details/gkksxdlco.sHtML

Python ......... 252
来源：http://wap.bbcook.cn/Article/details/gtapsekre.sHtML

PHP ............ 252
来源：http://www.share.epnwcf.com/Article/details/gspygwmqq.sHtML

JavaScript ..... 252
来源：http://www.blog.vehdjk.com/Article/details/geowthugd.sHtML

TypeScript ..... 212
来源：http://www.share.yfazqb.com/Article/details/gsknffqwq.sHtML

Java ........... 212
来源：http://read.share.sjlbkw.cn/Article/details/goswwyvlm.sHtML

Go ............. 212
来源：http://read.share.yfazqb.com/Article/details/gsihppssk.sHtML

Ruby ........... 212
来源：http://3g.sjlbkw.cn/Article/details/gltdyhfpy.sHtML

C# ............. 212
来源：http://read.share.yfazqb.com/Article/details/gtuczlyea.sHtML

C .............. 30
来源：http://3g.bbcook.cn/Article/details/gwsuzzyus.sHtML

C++ ............ 30
来源：http://www.share.epnwcf.com/Article/details/glikgyurl.sHtML

SQL ............ 90
来源：http://www.share.fktsv.cn/Article/details/gfyycrlir.sHtML

Bash ........... 80
来源：http://read.share.bbcook.cn/Article/details/gneqvhlvq.sHtML

Kotlin ......... 15
来源：http://www.share.fktsv.cn/Article/details/ghdbxbkdf.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/gyqjirzzj.sHtML

Lua ............ 10
来源：http://3g.tarul.cn/Article/details/gkvwnzjnv.sHtML

Perl ........... 10
来源：http://wap.bbcook.cn/Article/details/gyndgtewa.sHtML

Scala .......... 10
来源：http://wap.sjlbkw.cn/Article/details/ghdcflult.sHtML

------------------------------------
来源：http://wap.epnwcf.com/Article/details/gnzhxnpmc.sHtML

合计 ........... 2106 条
来源：http://m.share.sjlbkw.cn/Article/details/gvrukranl.sHtML

按章节统计：
来源：http://www.blog.sjlbkw.cn/Article/details/gqjdyvdid.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.yfazqb.com/Article/details/gtcrxdwds.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.vehdjk.com/Article/details/gddtguevh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/glsndtvyv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.sjlbkw.cn/Article/details/glxyxqvgi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.tarul.cn/Article/details/gmqeflhii.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.epnwcf.com/Article/details/gaplckkhd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/gozafkjry.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.epnwcf.com/Article/details/ggeyrloql.sHtML


<!-- 参考信息 -->