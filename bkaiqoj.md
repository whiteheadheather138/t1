代发 wailian999

[T49] Perl：函数
来源：http://www.blog.tarul.cn/Article/details/gdicphfkx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gtnxtbeyb.sHtML

[T50] Perl：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gezbrbikh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.yfazqb.com/Article/details/gdyalnwad.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fktsv.cn/Article/details/gfjwbbthv.sHtML

[T51] Scala：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gplbylzqu.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gdtubcfde.sHtML

[T52] Scala：变量
来源：http://www.share.tarul.cn/Article/details/gqjddmlwy.sHtML

val a = 1;  var b = 2
来源：http://mobile.vehdjk.com/Article/details/gqiqmvtgp.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gtpawzydv.sHtML

s"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gzxjlcbuz.sHtML

[T54] Scala：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gckijlyqj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.bbcook.cn/Article/details/gfcrcgsfc.sHtML

[T55] Scala：集合过滤
来源：http://baike.bbcook.cn/Article/details/gwaqucrkl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.bbcook.cn/Article/details/geulyourw.sHtML

[T56] Scala：样例类
来源：http://wap.vehdjk.com/Article/details/gqqfyvnet.sHtML

case class User(name: String, age: Int)
来源：http://baike.sjlbkw.cn/Article/details/godoywvtv.sHtML

[T57] Scala：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gcufxtyyx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.tarul.cn/Article/details/gswpgfpph.sHtML

[T58] Scala：函数定义
来源：http://wap.vehdjk.com/Article/details/gdglhvujc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.sjlbkw.cn/Article/details/ghqxbqqrx.sHtML

[T59] Scala：循环
来源：http://m.share.bbcook.cn/Article/details/gimrfsikc.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.vehdjk.com/Article/details/gsvvcdshd.sHtML

[T60] Scala：折叠
来源：http://www.share.bbcook.cn/Article/details/gwolesxti.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.vehdjk.com/Article/details/gbddhgvgm.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gdqbisogu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.yfazqb.com/Article/details/gxpbcplrx.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnpaoequw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.vehdjk.com/Article/details/gyozuunkk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.yfazqb.com/Article/details/gyuicitaf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.epnwcf.com/Article/details/gngiylxxr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.yfazqb.com/Article/details/ggzbrmtuu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.yfazqb.com/Article/details/giusilcef.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.sjlbkw.cn/Article/details/gtgketive.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.tarul.cn/Article/details/gsgbbfoce.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.yfazqb.com/Article/details/gxglrsltl.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.epnwcf.com/Article/details/gpprnyvrz.sHtML

list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gjjzeiiss.sHtML

[U06] Py：合并两个字典
来源：http://3g.sjlbkw.cn/Article/details/gtetkdkye.sHtML

{**a, **b}
来源：http://www.share.yfazqb.com/Article/details/gpdqbmppz.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.yfazqb.com/Article/details/gtumwwued.sHtML

{v: k for k, v in d.items()}
来源：http://blog.tarul.cn/Article/details/gdzsrlenn.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gslsktqee.sHtML

[y for x in nested for y in x]
来源：http://3g.fktsv.cn/Article/details/gjzkoxokg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.yfazqb.com/Article/details/gvrxkmeyc.sHtML

max(d, key=d.get)
来源：http://www.blog.yfazqb.com/Article/details/gldpekwot.sHtML

[U10] Py：按值排序字典
来源：http://wap.bbcook.cn/Article/details/gkhoypvou.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.vehdjk.com/Article/details/grhkbsajb.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.tarul.cn/Article/details/gspsniuho.sHtML

(x * 2 for x in arr)
来源：http://mobile.vehdjk.com/Article/details/ghsyampvq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fktsv.cn/Article/details/ghogqdbox.sHtML

Counter(arr).most_common(3)
来源：http://baike.yfazqb.com/Article/details/gakiwcgqf.sHtML

[U13] Py：固定长度队列
来源：http://wap.tarul.cn/Article/details/goekdueun.sHtML

deque(maxlen=10)
来源：http://wap.epnwcf.com/Article/details/gqadfzabw.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.sjlbkw.cn/Article/details/gjvcwshym.sHtML

defaultdict(list)
来源：http://www.m.share.yfazqb.com/Article/details/gfvxpqufc.sHtML

[U15] Py：高精度计时
来源：http://3g.epnwcf.com/Article/details/gadyrbnib.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/gbxmcixzi.sHtML

[U16] Py：命令行参数解析
来源：http://baike.bbcook.cn/Article/details/gwybzponf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.epnwcf.com/Article/details/goiciqnrm.sHtML

[U17] Py：初始化日志
来源：http://wap.vehdjk.com/Article/details/gabmasyve.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.vehdjk.com/Article/details/gsscwstmq.sHtML

[U18] Py：预编译正则
来源：http://www.blog.bbcook.cn/Article/details/grzoxspzx.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.epnwcf.com/Article/details/gbwvzgjrp.sHtML

[U19] Py：正则替换带回调
来源：http://blog.tarul.cn/Article/details/gmswstbwp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.epnwcf.com/Article/details/gxzeakkzy.sHtML

[U20] Py：缓存函数结果
来源：http://blog.yfazqb.com/Article/details/giqtgetqc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.yfazqb.com/Article/details/gbxjknwcr.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.tarul.cn/Article/details/gtyzsfnno.sHtML

@contextlib.contextmanager
来源：http://3g.vehdjk.com/Article/details/gcwdxidab.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fktsv.cn/Article/details/gtkgadubc.sHtML

list(zip(*m))
来源：http://www.share.yfazqb.com/Article/details/gcpszldol.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.bbcook.cn/Article/details/gfevzcqqa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.yfazqb.com/Article/details/gcpvukfio.sHtML

[U24] Py：路径操作
来源：http://wap.sjlbkw.cn/Article/details/gzhlwjyum.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gwbncszue.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.sjlbkw.cn/Article/details/gmehnbswh.sHtML

csv.DictReader(f)
来源：http://read.share.epnwcf.com/Article/details/gpfdtnlfv.sHtML

[U26] Py：并发下载
来源：http://m.share.tarul.cn/Article/details/gcyphfxqj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.epnwcf.com/Article/details/gpbvesvgt.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.tarul.cn/Article/details/gobmgsxvp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.bbcook.cn/Article/details/gjtohbqsu.sHtML

[U28] Py：类型别名
来源：http://blog.epnwcf.com/Article/details/guvytsfds.sHtML

UserId = int
来源：http://wap.tarul.cn/Article/details/gxuceggsb.sHtML

[U29] Py：属性校验
来源：http://wap.epnwcf.com/Article/details/gysezvgmu.sHtML

@property 与 @x.setter 配合
来源：http://read.share.sjlbkw.cn/Article/details/gnhvpzgse.sHtML

[U30] Py：数据类
来源：http://www.share.bbcook.cn/Article/details/gbjpsjeld.sHtML

@dataclass(slots=True)
来源：http://www.blog.vehdjk.com/Article/details/gaqpdjdgt.sHtML

[U31] Py：单测
来源：http://3g.yfazqb.com/Article/details/gwegtzqyr.sHtML

python -m pytest -q
来源：http://read.share.yfazqb.com/Article/details/gsgktyuul.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.bbcook.cn/Article/details/ggnhpxmbn.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.vehdjk.com/Article/details/gzixshltd.sHtML

[U33] Py：打包发布
来源：http://www.m.share.tarul.cn/Article/details/gneswyvry.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.sjlbkw.cn/Article/details/gdttzkfjt.sHtML

[U34] Py：判断编码
来源：http://blog.bbcook.cn/Article/details/gmguhjucj.sHtML

chardet.detect(raw)
来源：http://mobile.fktsv.cn/Article/details/gddcyemqn.sHtML

[U35] Py：发送邮件
来源：http://www.share.yfazqb.com/Article/details/gwyewijqn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.tarul.cn/Article/details/gsonrcmst.sHtML

[U36] Py：定时任务
来源：http://baike.sjlbkw.cn/Article/details/gozzfyity.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.sjlbkw.cn/Article/details/gtmlqlyhr.sHtML

[U37] Py：读写 Excel
来源：http://www.share.yfazqb.com/Article/details/gupjjflrj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.epnwcf.com/Article/details/gtkbyuokx.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.vehdjk.com/Article/details/guwqpauur.sHtML

Path(__file__).resolve().parent
来源：http://www.share.vehdjk.com/Article/details/gmijwvwep.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.epnwcf.com/Article/details/gqdnkuema.sHtML

sys.stdout.isatty()
来源：http://mobile.fktsv.cn/Article/details/gfkaeckts.sHtML

[U40] Py：打印到标准错误
来源：http://3g.yfazqb.com/Article/details/gykkqpthy.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gharoizlc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.sjlbkw.cn/Article/details/guuttxpbz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fktsv.cn/Article/details/ghlsegzoj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fktsv.cn/Article/details/gltjwsjzi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fktsv.cn/Article/details/gcrcfvxuf.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfwoqsdb.sHtML

namespace App\Http;
来源：http://www.m.share.sjlbkw.cn/Article/details/gstxltopx.sHtML

[U44] PHP：开启严格类型
来源：http://3g.bbcook.cn/Article/details/gajxrpkbl.sHtML

declare(strict_types=1);
来源：http://wap.yfazqb.com/Article/details/gbwhenggn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.tarul.cn/Article/details/gkpvmteso.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gcdcgcpgm.sHtML

[U46] PHP：可空类型
来源：http://3g.fktsv.cn/Article/details/gucokxjxz.sHtML

?string $name = null
来源：http://read.share.bbcook.cn/Article/details/gaklmokmf.sHtML

[U47] PHP：联合类型
来源：http://www.share.sjlbkw.cn/Article/details/guvfudlpf.sHtML

int|string $id
来源：http://mobile.fktsv.cn/Article/details/gvagmvpju.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gwhwtvcvi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.yfazqb.com/Article/details/gxegxvlgo.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.bbcook.cn/Article/details/glktmsdyf.sHtML

public readonly string $name
来源：http://baike.sjlbkw.cn/Article/details/gjoyvphpe.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.yfazqb.com/Article/details/gggepzwmh.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.yfazqb.com/Article/details/gmodqkmvb.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.yfazqb.com/Article/details/gnyvujkmh.sHtML

[$a, $b] = $arr;
来源：http://wap.bbcook.cn/Article/details/gukgphczg.sHtML

[U52] PHP：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/ghwvvetyf.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.epnwcf.com/Article/details/ghdvlpvaf.sHtML

[U53] PHP：空合并运算符
来源：http://blog.vehdjk.com/Article/details/gwmpplkkc.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fktsv.cn/Article/details/gkyntbuyz.sHtML

[U54] PHP：空安全调用
来源：http://m.share.sjlbkw.cn/Article/details/gzbtzbnas.sHtML

$obj?->method()
来源：http://wap.yfazqb.com/Article/details/gepucbflg.sHtML

[U55] PHP：match 表达式
来源：http://read.share.tarul.cn/Article/details/gowjymles.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.bbcook.cn/Article/details/ghsycpwle.sHtML

[U56] PHP：命名参数
来源：http://wap.yfazqb.com/Article/details/gzbwmaioy.sHtML

f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/ghlmsmzqe.sHtML

[U57] PHP：字符串插值
来源：http://mobile.tarul.cn/Article/details/gpnlzlqam.sHtML

"值: {$a}"
来源：http://read.share.fktsv.cn/Article/details/glycbifgj.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fktsv.cn/Article/details/gmnhjrvqj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.yfazqb.com/Article/details/gdbvqkplv.sHtML

[U59] PHP：自定义排序
来源：http://m.share.tarul.cn/Article/details/gdnwgrpax.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gcsoobyvv.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.bbcook.cn/Article/details/gpklfskio.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.epnwcf.com/Article/details/guvkcavlu.sHtML

[U61] PHP：正则
来源：http://3g.bbcook.cn/Article/details/gmgfaodyn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fktsv.cn/Article/details/gfwfgsvbx.sHtML

[U62] PHP：日期对象
来源：http://read.share.sjlbkw.cn/Article/details/gzauusoym.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.yfazqb.com/Article/details/guqxihatp.sHtML

[U63] PHP：文件读写
来源：http://read.share.tarul.cn/Article/details/gucucsqww.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.epnwcf.com/Article/details/gyczffmml.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.bbcook.cn/Article/details/gzwtmtjvq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.sjlbkw.cn/Article/details/ggpxsvolh.sHtML

[U65] PHP：会话
来源：http://read.share.fktsv.cn/Article/details/gubmqdjse.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fktsv.cn/Article/details/gyjhcxvxh.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.tarul.cn/Article/details/gpccxdytb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fktsv.cn/Article/details/gqxtfrawo.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.epnwcf.com/Article/details/gjtzrmoab.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.tarul.cn/Article/details/grtsreutt.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.vehdjk.com/Article/details/gunjjxxst.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmfezgho.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.yfazqb.com/Article/details/gmasuduct.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.epnwcf.com/Article/details/gkmykrlnw.sHtML

[U70] PHP：PDO 事务
来源：http://baike.tarul.cn/Article/details/gqoxtnuus.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/gidjspozz.sHtML

[U71] PHP：抛出异常
来源：http://read.share.vehdjk.com/Article/details/gjukehirk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.tarul.cn/Article/details/gijpgycex.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fktsv.cn/Article/details/gphfqkeqr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.vehdjk.com/Article/details/gssdfndry.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.vehdjk.com/Article/details/gkinxpqpl.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.sjlbkw.cn/Article/details/gckjcffho.sHtML

[U74] PHP：读取环境变量
来源：http://wap.yfazqb.com/Article/details/gkdecjgti.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.bbcook.cn/Article/details/gfnyztxml.sHtML

[U75] PHP：依赖注入
来源：http://m.share.epnwcf.com/Article/details/gbqenzhpz.sHtML

composer require psr/container
来源：http://wap.epnwcf.com/Article/details/gmwiiyymd.sHtML

[U76] PHP：简单路由
来源：http://blog.tarul.cn/Article/details/gpgtzjxnv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fktsv.cn/Article/details/gbpmxphrj.sHtML

[U77] PHP：模板渲染
来源：http://read.share.sjlbkw.cn/Article/details/grhsowtrf.sHtML

composer require twig/twig
来源：http://www.m.share.bbcook.cn/Article/details/gbdjcluci.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.epnwcf.com/Article/details/gfcbujbua.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.tarul.cn/Article/details/gqfydhkzl.sHtML

[U79] PHP：静态分析
来源：http://read.share.fktsv.cn/Article/details/gtfxsqsfs.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.yfazqb.com/Article/details/gplhtiymn.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.sjlbkw.cn/Article/details/gyhxwarls.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.yfazqb.com/Article/details/gfoewdnyh.sHtML

[U81] JS：初始化项目
来源：http://wap.tarul.cn/Article/details/grdmcvizm.sHtML

npm init -y;  npm i express
来源：http://m.share.fktsv.cn/Article/details/gadmrgoze.sHtML

[U82] JS：package.json 脚本
来源：http://3g.epnwcf.com/Article/details/gpajapzbm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.yfazqb.com/Article/details/ghwpucijz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.yfazqb.com/Article/details/gsnwrawrq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.bbcook.cn/Article/details/gguyhahuj.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.tarul.cn/Article/details/gpqjmqven.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fktsv.cn/Article/details/glvhqsplt.sHtML

[U85] JS：可选链
来源：http://blog.bbcook.cn/Article/details/gxwhbtpqz.sHtML

a?.b?.c
来源：http://wap.yfazqb.com/Article/details/gybnegoft.sHtML

[U86] JS：空值合并
来源：http://blog.bbcook.cn/Article/details/gyfedybri.sHtML

a ?? b
来源：http://www.blog.bbcook.cn/Article/details/gmhodefnq.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fktsv.cn/Article/details/gpasqxqye.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.epnwcf.com/Article/details/geymjpitr.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.sjlbkw.cn/Article/details/gvcvrmivb.sHtML

{ ...a, ...b }
来源：http://blog.sjlbkw.cn/Article/details/gartlofzk.sHtML

[U89] JS：数组去重
来源：http://wap.tarul.cn/Article/details/grzxrdyal.sHtML

[...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gvskblkvr.sHtML

[U90] JS：数字数组排序
来源：http://wap.fktsv.cn/Article/details/gvmpydvit.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gfccbcgnc.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.epnwcf.com/Article/details/gwmtybaax.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.bbcook.cn/Article/details/gybrrlkmk.sHtML

[U92] JS：深拷贝
来源：http://mobile.tarul.cn/Article/details/glysajbtg.sHtML

structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gbnwokkzl.sHtML

[U93] JS：模板字符串
来源：http://mobile.tarul.cn/Article/details/gnnvylpwi.sHtML

`共 ${n} 条`
来源：http://baike.epnwcf.com/Article/details/gynzldteo.sHtML

[U94] JS：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gcronexlg.sHtML

const double = x => x * 2;
来源：http://blog.epnwcf.com/Article/details/gllqcqaqy.sHtML

[U95] JS：Promise 包装
来源：http://www.share.sjlbkw.cn/Article/details/gpshdmwjc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.sjlbkw.cn/Article/details/ghllrybyx.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.tarul.cn/Article/details/gqptbmkyo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gimqfvxqe.sHtML

[U97] JS：并发请求
来源：http://m.share.bbcook.cn/Article/details/gcjgeogtx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gdntvtegc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.vehdjk.com/Article/details/gsibphudu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fktsv.cn/Article/details/gqfirkkpv.sHtML

[U99] JS：事件监听
来源：http://www.blog.vehdjk.com/Article/details/gxhlarixo.sHtML

el.addEventListener("click", e => {})
来源：http://baike.sjlbkw.cn/Article/details/gvjgcmbzf.sHtML

[U100] JS：DOM 查询
来源：http://wap.sjlbkw.cn/Article/details/ggpmlaetg.sHtML

document.querySelector(".item")
来源：http://mobile.sjlbkw.cn/Article/details/gvfaskjbm.sHtML

[U101] JS：classList 操作
来源：http://blog.epnwcf.com/Article/details/ghobaorhl.sHtML

el.classList.toggle("active")
来源：http://www.blog.sjlbkw.cn/Article/details/gynehaosi.sHtML

[U102] JS：本地存储
来源：http://m.share.fktsv.cn/Article/details/glupasfxg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fktsv.cn/Article/details/gnnynpspu.sHtML

[U103] JS：定时器
来源：http://www.share.fktsv.cn/Article/details/gwvzanymm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.tarul.cn/Article/details/gzjxssgri.sHtML

[U104] JS：防抖
来源：http://www.share.fktsv.cn/Article/details/gtsolbjbr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/giqwfhqmp.sHtML

[U105] JS：节流
来源：http://www.blog.sjlbkw.cn/Article/details/gstiyfuji.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.yfazqb.com/Article/details/gepdtzrtu.sHtML

[U106] JS：日期格式化
来源：http://3g.vehdjk.com/Article/details/gaywxzxko.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.sjlbkw.cn/Article/details/gjeqcorxe.sHtML

[U107] JS：数字千分位
来源：http://www.share.tarul.cn/Article/details/gccvyuxvx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.yfazqb.com/Article/details/gliqmevux.sHtML

[U108] JS：随机整数
来源：http://blog.tarul.cn/Article/details/gssrvzisr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.vehdjk.com/Article/details/gwesxngxb.sHtML

[U109] JS：数组分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gsaxhhsis.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gzsvzvdgs.sHtML

[U110] JS：数组分块
来源：http://wap.vehdjk.com/Article/details/gmglxlpkt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.vehdjk.com/Article/details/gncazmvmn.sHtML

[U111] JS：对象转 Map
来源：http://baike.epnwcf.com/Article/details/gqicomovm.sHtML

new Map(Object.entries(obj))
来源：http://www.share.vehdjk.com/Article/details/gxzhgbppl.sHtML

[U112] JS：字符串补位
来源：http://www.blog.vehdjk.com/Article/details/gdjjgkuqa.sHtML

"7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gxgoyqgui.sHtML

[U113] JS：正则替换全部
来源：http://wap.bbcook.cn/Article/details/gjsfcumua.sHtML

s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gtsubyoma.sHtML

[U114] JS：JSON 深比较
来源：http://baike.sjlbkw.cn/Article/details/gstnenxtg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.bbcook.cn/Article/details/gdhfamsra.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/givbdzkts.sHtML

crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gaudsanai.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.tarul.cn/Article/details/gtkbnostw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.yfazqb.com/Article/details/gzwrpnkkb.sHtML

[U117] JS：单元测试
来源：http://wap.tarul.cn/Article/details/glwqtnghn.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.epnwcf.com/Article/details/guzyxkiob.sHtML

[U118] JS：开发服务器
来源：http://3g.fktsv.cn/Article/details/gxgoohjgz.sHtML

npm i -D vite;  npx vite
来源：http://read.share.sjlbkw.cn/Article/details/gyobteidd.sHtML

[U119] JS：生产构建
来源：http://3g.yfazqb.com/Article/details/glkcnvssh.sHtML

npx vite build
来源：http://www.blog.tarul.cn/Article/details/gcbwknype.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fktsv.cn/Article/details/gbjekhdtg.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.vehdjk.com/Article/details/gsnhshkod.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvotgmsnv.sHtML

统计汇总
来源：http://mobile.fktsv.cn/Article/details/gzsqoztdb.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxsdgpndx.sHtML

按语言统计（条）：
来源：http://www.blog.yfazqb.com/Article/details/ghsiqspqt.sHtML

Python ......... 252
来源：http://mobile.sjlbkw.cn/Article/details/gnvsisasi.sHtML

PHP ............ 252
来源：http://mobile.bbcook.cn/Article/details/gdtorxiav.sHtML

JavaScript ..... 252
来源：http://wap.bbcook.cn/Article/details/giumfkogs.sHtML

TypeScript ..... 212
来源：http://www.m.share.yfazqb.com/Article/details/gbuxdtzin.sHtML

Java ........... 212
来源：http://baike.yfazqb.com/Article/details/geudaumdg.sHtML

Go ............. 212
来源：http://mobile.epnwcf.com/Article/details/grwoytcis.sHtML

Ruby ........... 212
来源：http://www.m.share.tarul.cn/Article/details/grzzunjdm.sHtML

C# ............. 212
来源：http://baike.fktsv.cn/Article/details/gagtdkgyg.sHtML

C .............. 30
来源：http://mobile.sjlbkw.cn/Article/details/gzfbrctso.sHtML

C++ ............ 30
来源：http://read.share.vehdjk.com/Article/details/guiydfixo.sHtML

SQL ............ 90
来源：http://www.m.share.tarul.cn/Article/details/gduwrlrhf.sHtML

Bash ........... 80
来源：http://read.share.yfazqb.com/Article/details/gcvwosrnr.sHtML

Kotlin ......... 15
来源：http://www.m.share.fktsv.cn/Article/details/giutgkvkg.sHtML

Swift .......... 15
来源：http://read.share.sjlbkw.cn/Article/details/geaxtusca.sHtML

Lua ............ 10
来源：http://www.share.tarul.cn/Article/details/gmadjxmdj.sHtML

Perl ........... 10
来源：http://www.m.share.yfazqb.com/Article/details/gjomfbyth.sHtML

Scala .......... 10
来源：http://baike.bbcook.cn/Article/details/gbwdxusbb.sHtML

------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gvgeumzhz.sHtML

合计 ........... 2106 条
来源：http://mobile.tarul.cn/Article/details/glvpwkggr.sHtML

按章节统计：
来源：http://blog.sjlbkw.cn/Article/details/gwiexryqa.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.bbcook.cn/Article/details/gwyrrsfdc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gbhehiqtm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/gbrvggokj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.yfazqb.com/Article/details/gnvcnnmnc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.tarul.cn/Article/details/gkvczfrze.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.tarul.cn/Article/details/gzegjvzuw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/grlvfodyq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/guucoddyn.sHtML


<!-- 参考信息 -->