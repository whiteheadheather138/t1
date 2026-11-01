代发 wailian999

[T49] Perl：函数
来源：http://baike.fktsv.cn/Article/details/gegnptrnj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gofrqsulf.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gtxzwftyv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.sjlbkw.cn/Article/details/gstuxqwjb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.bbcook.cn/Article/details/gtqhnganv.sHtML

[T51] Scala：Hello World
来源：http://baike.tarul.cn/Article/details/gwtecwzwd.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/gdqgwmutz.sHtML

[T52] Scala：变量
来源：http://www.m.share.yfazqb.com/Article/details/ggbapkdvv.sHtML

val a = 1;  var b = 2
来源：http://3g.yfazqb.com/Article/details/gkucptwzd.sHtML

[T53] Scala：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gfyzdfydm.sHtML

s"值: $b"
来源：http://read.share.epnwcf.com/Article/details/gjgqlbrzv.sHtML

[T54] Scala：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gjpltocca.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.bbcook.cn/Article/details/gucmyxctp.sHtML

[T55] Scala：集合过滤
来源：http://blog.tarul.cn/Article/details/gxduoycnt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.vehdjk.com/Article/details/gysfxcwai.sHtML

[T56] Scala：样例类
来源：http://baike.yfazqb.com/Article/details/gdudzhhoi.sHtML

case class User(name: String, age: Int)
来源：http://3g.sjlbkw.cn/Article/details/gnzvvbedm.sHtML

[T57] Scala：模式匹配
来源：http://blog.yfazqb.com/Article/details/ghwwfyada.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.vehdjk.com/Article/details/geeqffcyn.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.tarul.cn/Article/details/gosioejcb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.vehdjk.com/Article/details/gllspgabi.sHtML

[T59] Scala：循环
来源：http://mobile.tarul.cn/Article/details/ghfqbfrhw.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.vehdjk.com/Article/details/gpkaajlev.sHtML

[T60] Scala：折叠
来源：http://www.blog.yfazqb.com/Article/details/gnofvcyoq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.vehdjk.com/Article/details/givcfnsbd.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/giyoyaoeq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/gsuzbqqfm.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gxrtxnvch.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.epnwcf.com/Article/details/gmqtlpang.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.yfazqb.com/Article/details/gcbsmhrls.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.tarul.cn/Article/details/grizxansk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.bbcook.cn/Article/details/glrstinan.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.bbcook.cn/Article/details/gfcizukwx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.yfazqb.com/Article/details/gukpxfvyz.sHtML

[U04] Py：变量调试打印
来源：http://3g.vehdjk.com/Article/details/gehoczejs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fktsv.cn/Article/details/gitidatfu.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.sjlbkw.cn/Article/details/gyqojsgeg.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/gcjvfadfm.sHtML

[U06] Py：合并两个字典
来源：http://wap.bbcook.cn/Article/details/ghoqnxprk.sHtML

{**a, **b}
来源：http://www.blog.vehdjk.com/Article/details/gxudzekop.sHtML

[U07] Py：反转字典键值
来源：http://www.share.tarul.cn/Article/details/gkszlfcbz.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.vehdjk.com/Article/details/gifqqvcme.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.sjlbkw.cn/Article/details/guycqttqr.sHtML

[y for x in nested for y in x]
来源：http://m.share.sjlbkw.cn/Article/details/gvafkjlfe.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.bbcook.cn/Article/details/ghuxezeum.sHtML

max(d, key=d.get)
来源：http://www.m.share.fktsv.cn/Article/details/gmraqvpzp.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fktsv.cn/Article/details/gxvcbfnuv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.vehdjk.com/Article/details/gilhaorne.sHtML

[U11] Py：生成器表达式
来源：http://baike.yfazqb.com/Article/details/gpqjlzgqe.sHtML

(x * 2 for x in arr)
来源：http://m.share.yfazqb.com/Article/details/gehugfuja.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.vehdjk.com/Article/details/gmzjfzzcp.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.bbcook.cn/Article/details/gjbmnhjzj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.bbcook.cn/Article/details/gzhrtnntr.sHtML

deque(maxlen=10)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdbtpvxm.sHtML

[U14] Py：分组收集到列表
来源：http://blog.yfazqb.com/Article/details/ghwgicvxe.sHtML

defaultdict(list)
来源：http://3g.epnwcf.com/Article/details/gekswmkda.sHtML

[U15] Py：高精度计时
来源：http://m.share.sjlbkw.cn/Article/details/gzfurixyu.sHtML

t = time.perf_counter()
来源：http://blog.bbcook.cn/Article/details/gtdpbheew.sHtML

[U16] Py：命令行参数解析
来源：http://3g.epnwcf.com/Article/details/gfhoujhmr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.vehdjk.com/Article/details/gzstjorul.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.yfazqb.com/Article/details/gclyfmzzq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fktsv.cn/Article/details/gktetdzdi.sHtML

[U18] Py：预编译正则
来源：http://blog.sjlbkw.cn/Article/details/gcvrnmxnd.sHtML

pat = re.compile(r"\d+")
来源：http://3g.epnwcf.com/Article/details/gojeidkxh.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.epnwcf.com/Article/details/grlldoatq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.yfazqb.com/Article/details/gwpakfmmv.sHtML

[U20] Py：缓存函数结果
来源：http://wap.tarul.cn/Article/details/gxtcnqyha.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.tarul.cn/Article/details/grkewssdq.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.bbcook.cn/Article/details/ghglapdcr.sHtML

@contextlib.contextmanager
来源：http://m.share.epnwcf.com/Article/details/gnpamsqil.sHtML

[U22] Py：矩阵转置
来源：http://wap.epnwcf.com/Article/details/gpcvjgmvp.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/gbqchqtjx.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.sjlbkw.cn/Article/details/gjxncpvfn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.sjlbkw.cn/Article/details/gikmazhzl.sHtML

[U24] Py：路径操作
来源：http://mobile.sjlbkw.cn/Article/details/gnmjokwsm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gkqekakoj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fktsv.cn/Article/details/gnyqsdyte.sHtML

csv.DictReader(f)
来源：http://www.share.bbcook.cn/Article/details/gzfulrqjz.sHtML

[U26] Py：并发下载
来源：http://wap.fktsv.cn/Article/details/gwjlfppqv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.tarul.cn/Article/details/gwgqcfpwe.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fktsv.cn/Article/details/glhvavtzc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.yfazqb.com/Article/details/gvsdukzbf.sHtML

[U28] Py：类型别名
来源：http://www.m.share.tarul.cn/Article/details/gtfqdahnx.sHtML

UserId = int
来源：http://mobile.yfazqb.com/Article/details/gukkpadwn.sHtML

[U29] Py：属性校验
来源：http://www.blog.sjlbkw.cn/Article/details/ghfcgmeno.sHtML

@property 与 @x.setter 配合
来源：http://read.share.epnwcf.com/Article/details/ghgmnjevt.sHtML

[U30] Py：数据类
来源：http://mobile.vehdjk.com/Article/details/gbbkoenwq.sHtML

@dataclass(slots=True)
来源：http://mobile.yfazqb.com/Article/details/gazgnaysn.sHtML

[U31] Py：单测
来源：http://read.share.epnwcf.com/Article/details/gmigcfsyy.sHtML

python -m pytest -q
来源：http://mobile.fktsv.cn/Article/details/geaznoxsh.sHtML

[U32] Py：代码格式化
来源：http://read.share.epnwcf.com/Article/details/grcqyyrel.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.yfazqb.com/Article/details/grkevtxdh.sHtML

[U33] Py：打包发布
来源：http://www.m.share.tarul.cn/Article/details/gyoieixms.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.epnwcf.com/Article/details/gywalvpgm.sHtML

[U34] Py：判断编码
来源：http://3g.yfazqb.com/Article/details/gqsdcwndb.sHtML

chardet.detect(raw)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmfrfrxw.sHtML

[U35] Py：发送邮件
来源：http://www.blog.tarul.cn/Article/details/guijkkvdq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fktsv.cn/Article/details/ghxnwbptk.sHtML

[U36] Py：定时任务
来源：http://www.share.bbcook.cn/Article/details/gkclrrome.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.bbcook.cn/Article/details/gcpsgwcla.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.vehdjk.com/Article/details/gjjozotrx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.yfazqb.com/Article/details/gzynxhmyi.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.bbcook.cn/Article/details/ghfhzcnrr.sHtML

Path(__file__).resolve().parent
来源：http://baike.bbcook.cn/Article/details/gsuntmupp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.bbcook.cn/Article/details/gwppenwou.sHtML

sys.stdout.isatty()
来源：http://baike.bbcook.cn/Article/details/gfhlpmhjv.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.epnwcf.com/Article/details/gqchjjawl.sHtML

print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/gdbrepxoc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.yfazqb.com/Article/details/ggxgerlto.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.yfazqb.com/Article/details/gehrktrqe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.vehdjk.com/Article/details/gosuvoovw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fktsv.cn/Article/details/gwzltkqkz.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fktsv.cn/Article/details/gfrngkfnm.sHtML

namespace App\Http;
来源：http://m.share.tarul.cn/Article/details/gqzxqzwxc.sHtML

[U44] PHP：开启严格类型
来源：http://3g.yfazqb.com/Article/details/gsntugkgi.sHtML

declare(strict_types=1);
来源：http://blog.yfazqb.com/Article/details/gwtplgcmn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.yfazqb.com/Article/details/gihghhlrt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gunvsxciu.sHtML

[U46] PHP：可空类型
来源：http://www.share.epnwcf.com/Article/details/ghqghtuvg.sHtML

?string $name = null
来源：http://baike.yfazqb.com/Article/details/geyxmnqei.sHtML

[U47] PHP：联合类型
来源：http://m.share.tarul.cn/Article/details/gqrzlvhtf.sHtML

int|string $id
来源：http://www.m.share.epnwcf.com/Article/details/gklwunwfl.sHtML

[U48] PHP：纯枚举
来源：http://baike.epnwcf.com/Article/details/gnbqkqhin.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.yfazqb.com/Article/details/gzqwrlkqm.sHtML

[U49] PHP：只读属性
来源：http://3g.sjlbkw.cn/Article/details/gifeduggg.sHtML

public readonly string $name
来源：http://3g.bbcook.cn/Article/details/grvybtrfv.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.epnwcf.com/Article/details/gluxmxgyw.sHtML

public function __construct(private int $id) {}
来源：http://3g.sjlbkw.cn/Article/details/grqdykiny.sHtML

[U51] PHP：数组解构
来源：http://blog.vehdjk.com/Article/details/gzoxhehzi.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.vehdjk.com/Article/details/gdghpvclh.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.bbcook.cn/Article/details/gmgxriytr.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fktsv.cn/Article/details/gbhfciuqf.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.tarul.cn/Article/details/gusezrluy.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.sjlbkw.cn/Article/details/gwttoxewj.sHtML

[U54] PHP：空安全调用
来源：http://mobile.tarul.cn/Article/details/grpfnngbn.sHtML

$obj?->method()
来源：http://www.m.share.bbcook.cn/Article/details/gsaxlcgfo.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/goyycauyl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.bbcook.cn/Article/details/gajxfvgwp.sHtML

[U56] PHP：命名参数
来源：http://mobile.epnwcf.com/Article/details/gtmaeddtm.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/ghhwkcwxx.sHtML

[U57] PHP：字符串插值
来源：http://m.share.tarul.cn/Article/details/gmntydvcf.sHtML

"值: {$a}"
来源：http://www.m.share.bbcook.cn/Article/details/gqtnkywcz.sHtML

[U58] PHP：数组三件套
来源：http://read.share.tarul.cn/Article/details/gpvcuivqq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.vehdjk.com/Article/details/gxbmoivgi.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.sjlbkw.cn/Article/details/gmvkfrxfr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gsvxmyzjg.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.bbcook.cn/Article/details/griyjkckt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fktsv.cn/Article/details/gkhgivrrr.sHtML

[U61] PHP：正则
来源：http://www.blog.sjlbkw.cn/Article/details/guhivuefs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/grrqfkvyz.sHtML

[U62] PHP：日期对象
来源：http://www.share.tarul.cn/Article/details/gmnlqeuar.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.sjlbkw.cn/Article/details/gjxauwrjj.sHtML

[U63] PHP：文件读写
来源：http://mobile.bbcook.cn/Article/details/gsdvsmbqx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.bbcook.cn/Article/details/gcxgbjywr.sHtML

[U64] PHP：目录遍历
来源：http://wap.tarul.cn/Article/details/gtomfvdjz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fktsv.cn/Article/details/gtkbzxejd.sHtML

[U65] PHP：会话
来源：http://www.share.tarul.cn/Article/details/grrptxgan.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fktsv.cn/Article/details/gtmqzzcvm.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.tarul.cn/Article/details/gbcpmbvlu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fktsv.cn/Article/details/guhgrarow.sHtML

[U67] PHP：处理文件上传
来源：http://3g.epnwcf.com/Article/details/ghuzkcdaf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.epnwcf.com/Article/details/gjhjdihyi.sHtML

[U68] PHP：PDO 连接
来源：http://wap.vehdjk.com/Article/details/gtklmakoq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.epnwcf.com/Article/details/ghlrroifm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fktsv.cn/Article/details/gmcvkxtnz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.vehdjk.com/Article/details/gpnvuowye.sHtML

[U70] PHP：PDO 事务
来源：http://3g.sjlbkw.cn/Article/details/ggemllmae.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/gqkhaojyh.sHtML

[U71] PHP：抛出异常
来源：http://m.share.epnwcf.com/Article/details/gbrwswgvd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.tarul.cn/Article/details/gtxfsdign.sHtML

[U72] PHP：写错误日志
来源：http://wap.sjlbkw.cn/Article/details/glamhtpaq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fktsv.cn/Article/details/gohpoklix.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fktsv.cn/Article/details/gozaaahdg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.bbcook.cn/Article/details/glogmzagw.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/geksnlcky.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.yfazqb.com/Article/details/gwtjfdbap.sHtML

[U75] PHP：依赖注入
来源：http://3g.vehdjk.com/Article/details/gpeqxzsfl.sHtML

composer require psr/container
来源：http://read.share.tarul.cn/Article/details/gpqaqfxag.sHtML

[U76] PHP：简单路由
来源：http://3g.tarul.cn/Article/details/gbubnukqa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.bbcook.cn/Article/details/gmfjbtvre.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.yfazqb.com/Article/details/gxfwnunda.sHtML

composer require twig/twig
来源：http://www.blog.epnwcf.com/Article/details/gpeevywzf.sHtML

[U78] PHP：单元测试
来源：http://read.share.fktsv.cn/Article/details/gxjnhlvix.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fktsv.cn/Article/details/gpywdckao.sHtML

[U79] PHP：静态分析
来源：http://baike.tarul.cn/Article/details/gqyzaglpx.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fktsv.cn/Article/details/gdywgcuvc.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.yfazqb.com/Article/details/grbhkcvvj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fktsv.cn/Article/details/gwbacakyh.sHtML

[U81] JS：初始化项目
来源：http://read.share.yfazqb.com/Article/details/gwcdckwlj.sHtML

npm init -y;  npm i express
来源：http://read.share.yfazqb.com/Article/details/geiketmkf.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.tarul.cn/Article/details/ghpdsjxdp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.tarul.cn/Article/details/gksgkfjyz.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.sjlbkw.cn/Article/details/gsozwymny.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gedszlyyl.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.epnwcf.com/Article/details/gcvtjfncr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.tarul.cn/Article/details/glduzknfz.sHtML

[U85] JS：可选链
来源：http://mobile.bbcook.cn/Article/details/gkaywtgxc.sHtML

a?.b?.c
来源：http://m.share.epnwcf.com/Article/details/gzoipagzv.sHtML

[U86] JS：空值合并
来源：http://wap.sjlbkw.cn/Article/details/ggwmqlyox.sHtML

a ?? b
来源：http://m.share.yfazqb.com/Article/details/gfwsrfvwi.sHtML

[U87] JS：解构默认值
来源：http://www.blog.tarul.cn/Article/details/gmknhlmkq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.tarul.cn/Article/details/goegzuyfn.sHtML

[U88] JS：对象展开合并
来源：http://wap.sjlbkw.cn/Article/details/gylcfetkh.sHtML

{ ...a, ...b }
来源：http://blog.yfazqb.com/Article/details/gdjpagnap.sHtML

[U89] JS：数组去重
来源：http://3g.bbcook.cn/Article/details/gqxeauoau.sHtML

[...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/glagsyuhb.sHtML

[U90] JS：数字数组排序
来源：http://3g.vehdjk.com/Article/details/grcrnbdmy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gfiavpzzj.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.yfazqb.com/Article/details/gvggfgipb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fktsv.cn/Article/details/gekdcxjcm.sHtML

[U92] JS：深拷贝
来源：http://blog.tarul.cn/Article/details/gssgzfltg.sHtML

structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gfmdpkhdm.sHtML

[U93] JS：模板字符串
来源：http://read.share.yfazqb.com/Article/details/gjngfedkz.sHtML

`共 ${n} 条`
来源：http://www.blog.vehdjk.com/Article/details/gtgjstvov.sHtML

[U94] JS：箭头函数
来源：http://mobile.yfazqb.com/Article/details/gjwybmxlo.sHtML

const double = x => x * 2;
来源：http://www.blog.tarul.cn/Article/details/giwkrhnvd.sHtML

[U95] JS：Promise 包装
来源：http://read.share.tarul.cn/Article/details/gedxuezcj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.sjlbkw.cn/Article/details/giqobviat.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.vehdjk.com/Article/details/gxepbvnsd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/govgneijf.sHtML

[U97] JS：并发请求
来源：http://read.share.vehdjk.com/Article/details/ghsaxtozt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/gnbrtwclj.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.epnwcf.com/Article/details/gpmhbzhbk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fktsv.cn/Article/details/gasjxhvsz.sHtML

[U99] JS：事件监听
来源：http://3g.vehdjk.com/Article/details/gteroncqx.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.tarul.cn/Article/details/gthaoeunf.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.bbcook.cn/Article/details/gpptfpxyo.sHtML

document.querySelector(".item")
来源：http://blog.bbcook.cn/Article/details/gqcgawqwh.sHtML

[U101] JS：classList 操作
来源：http://wap.vehdjk.com/Article/details/gqxwihkbd.sHtML

el.classList.toggle("active")
来源：http://read.share.bbcook.cn/Article/details/gyyuwydgb.sHtML

[U102] JS：本地存储
来源：http://blog.sjlbkw.cn/Article/details/gcltgivfy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fktsv.cn/Article/details/gajdvxyxo.sHtML

[U103] JS：定时器
来源：http://read.share.bbcook.cn/Article/details/gknbtclvs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fktsv.cn/Article/details/gukmrsltm.sHtML

[U104] JS：防抖
来源：http://blog.sjlbkw.cn/Article/details/gsvizgdai.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gnpfpjogr.sHtML

[U105] JS：节流
来源：http://m.share.fktsv.cn/Article/details/gwwsxplic.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.bbcook.cn/Article/details/gitysdjot.sHtML

[U106] JS：日期格式化
来源：http://m.share.tarul.cn/Article/details/gwrvyorim.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.vehdjk.com/Article/details/glbiirpcs.sHtML

[U107] JS：数字千分位
来源：http://mobile.tarul.cn/Article/details/gwkczvhjh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.tarul.cn/Article/details/gcssvybjk.sHtML

[U108] JS：随机整数
来源：http://www.blog.fktsv.cn/Article/details/gtpqwqjbe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.sjlbkw.cn/Article/details/giwuecqhh.sHtML

[U109] JS：数组分组
来源：http://blog.fktsv.cn/Article/details/gfjsgqeow.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/gsopiukry.sHtML

[U110] JS：数组分块
来源：http://wap.tarul.cn/Article/details/guvrjuiie.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.epnwcf.com/Article/details/gnxxiqqyh.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.tarul.cn/Article/details/gwankjrxx.sHtML

new Map(Object.entries(obj))
来源：http://mobile.vehdjk.com/Article/details/gzwfzawsr.sHtML

[U112] JS：字符串补位
来源：http://read.share.fktsv.cn/Article/details/gglrwruuf.sHtML

"7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gvahavkpv.sHtML

[U113] JS：正则替换全部
来源：http://3g.vehdjk.com/Article/details/gfqhpnria.sHtML

s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/glkrfhsqt.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.sjlbkw.cn/Article/details/gftwjwaxr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/ghntlwnpa.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gomxkanks.sHtML

crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gardczzsg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyisftby.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.tarul.cn/Article/details/gmvablryz.sHtML

[U117] JS：单元测试
来源：http://mobile.yfazqb.com/Article/details/gibmrrwfk.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.vehdjk.com/Article/details/gxgaqflmn.sHtML

[U118] JS：开发服务器
来源：http://3g.yfazqb.com/Article/details/gtdzdrapl.sHtML

npm i -D vite;  npx vite
来源：http://wap.tarul.cn/Article/details/gnonydzpd.sHtML

[U119] JS：生产构建
来源：http://blog.fktsv.cn/Article/details/grgerndsh.sHtML

npx vite build
来源：http://www.blog.sjlbkw.cn/Article/details/gnbeudwmt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fktsv.cn/Article/details/gujrvucsv.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.tarul.cn/Article/details/guhtkkcwt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gtmtyqhyo.sHtML

统计汇总
来源：http://baike.vehdjk.com/Article/details/gpxoxysow.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gyfudtgau.sHtML

按语言统计（条）：
来源：http://m.share.sjlbkw.cn/Article/details/gkukegyzz.sHtML

Python ......... 252
来源：http://3g.fktsv.cn/Article/details/goywzycas.sHtML

PHP ............ 252
来源：http://mobile.yfazqb.com/Article/details/gmvegvrla.sHtML

JavaScript ..... 252
来源：http://www.blog.sjlbkw.cn/Article/details/gvlgzlpbs.sHtML

TypeScript ..... 212
来源：http://read.share.tarul.cn/Article/details/gvgfcfbkj.sHtML

Java ........... 212
来源：http://www.m.share.yfazqb.com/Article/details/gokqqhqnk.sHtML

Go ............. 212
来源：http://blog.sjlbkw.cn/Article/details/gyeomsrsi.sHtML

Ruby ........... 212
来源：http://read.share.vehdjk.com/Article/details/gdczlpawv.sHtML

C# ............. 212
来源：http://www.blog.yfazqb.com/Article/details/grfcjvgvd.sHtML

C .............. 30
来源：http://3g.tarul.cn/Article/details/gawkwvuyg.sHtML

C++ ............ 30
来源：http://www.m.share.fktsv.cn/Article/details/gsnigurry.sHtML

SQL ............ 90
来源：http://m.share.vehdjk.com/Article/details/gplfmkfyb.sHtML

Bash ........... 80
来源：http://read.share.bbcook.cn/Article/details/galnirhkn.sHtML

Kotlin ......... 15
来源：http://3g.sjlbkw.cn/Article/details/ghahsiswh.sHtML

Swift .......... 15
来源：http://m.share.epnwcf.com/Article/details/gcnelxgbg.sHtML

Lua ............ 10
来源：http://baike.tarul.cn/Article/details/gnwnkmvrn.sHtML

Perl ........... 10
来源：http://www.share.bbcook.cn/Article/details/gpewhispm.sHtML

Scala .......... 10
来源：http://wap.bbcook.cn/Article/details/gpihsmsgq.sHtML

------------------------------------
来源：http://baike.yfazqb.com/Article/details/gazuzuqti.sHtML

合计 ........... 2106 条
来源：http://www.share.bbcook.cn/Article/details/gwwwsenwl.sHtML

按章节统计：
来源：http://m.share.tarul.cn/Article/details/gbpyheoaq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gzplqwvml.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/guwbtzsus.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/grvtuznqo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.sjlbkw.cn/Article/details/gjykpolat.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.yfazqb.com/Article/details/giuhpgtzp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.bbcook.cn/Article/details/ggfqwfrrb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gsbldoqbc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fktsv.cn/Article/details/gopubawvw.sHtML


<!-- 参考信息 -->