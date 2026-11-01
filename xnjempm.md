代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fktsv.cn/Article/details/gbsiqugdf.sHtML

[T51] Scala：Hello World
来源：http://read.share.bbcook.cn/Article/details/gazfydvry.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/gvyfsqqrn.sHtML

[T52] Scala：变量
来源：http://wap.sjlbkw.cn/Article/details/ggvkckepo.sHtML

val a = 1;  var b = 2
来源：http://baike.vehdjk.com/Article/details/ggcaibjbb.sHtML

[T53] Scala：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/grlgbkyqo.sHtML

s"值: $b"
来源：http://read.share.tarul.cn/Article/details/gnkxahxly.sHtML

[T54] Scala：集合映射
来源：http://baike.sjlbkw.cn/Article/details/gzlgjdpae.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.vehdjk.com/Article/details/gzvuyhtvz.sHtML

[T55] Scala：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gjyummeqn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.sjlbkw.cn/Article/details/gohjxrivk.sHtML

[T56] Scala：样例类
来源：http://read.share.epnwcf.com/Article/details/gghwovftz.sHtML

case class User(name: String, age: Int)
来源：http://mobile.tarul.cn/Article/details/gdwswnfyz.sHtML

[T57] Scala：模式匹配
来源：http://wap.vehdjk.com/Article/details/gahdaiufj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.epnwcf.com/Article/details/gtfsdgwot.sHtML

[T58] Scala：函数定义
来源：http://wap.vehdjk.com/Article/details/gdsrcdstx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fktsv.cn/Article/details/gpthfmgvy.sHtML

[T59] Scala：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbflqhhd.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gyfqiropx.sHtML

[T60] Scala：折叠
来源：http://www.m.share.vehdjk.com/Article/details/gkghmohrg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.vehdjk.com/Article/details/gngbijvoa.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkakrwtzc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fktsv.cn/Article/details/guylaqviz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqxololip.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fktsv.cn/Article/details/gtlamwuog.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.tarul.cn/Article/details/gwknwzygx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.vehdjk.com/Article/details/gvatykcmz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.sjlbkw.cn/Article/details/gwoqexjod.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.vehdjk.com/Article/details/gmoloclne.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.bbcook.cn/Article/details/gernvhdyt.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/gqfrzvkxb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.epnwcf.com/Article/details/ghkzpmbcr.sHtML

[U05] Py：列表去重且保序
来源：http://wap.tarul.cn/Article/details/giekrswbv.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gxvrittph.sHtML

[U06] Py：合并两个字典
来源：http://m.share.bbcook.cn/Article/details/ghxxwmgyk.sHtML

{**a, **b}
来源：http://m.share.epnwcf.com/Article/details/gkjygynkq.sHtML

[U07] Py：反转字典键值
来源：http://3g.sjlbkw.cn/Article/details/ghcsjnefo.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.tarul.cn/Article/details/gcpsqxcfz.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fktsv.cn/Article/details/gmbfdyvmi.sHtML

[y for x in nested for y in x]
来源：http://baike.yfazqb.com/Article/details/geyqwjlnv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fktsv.cn/Article/details/gvfobgyev.sHtML

max(d, key=d.get)
来源：http://m.share.epnwcf.com/Article/details/ggfwjylgs.sHtML

[U10] Py：按值排序字典
来源：http://mobile.sjlbkw.cn/Article/details/gkjvtjgsm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.bbcook.cn/Article/details/gqbvferln.sHtML

[U11] Py：生成器表达式
来源：http://www.share.epnwcf.com/Article/details/gvbksjrez.sHtML

(x * 2 for x in arr)
来源：http://baike.epnwcf.com/Article/details/gttpmhxwc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.tarul.cn/Article/details/gkzrhanak.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.epnwcf.com/Article/details/gznmafolg.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.vehdjk.com/Article/details/gutpiaufr.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/ginxfhsba.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.vehdjk.com/Article/details/gogfergoq.sHtML

defaultdict(list)
来源：http://read.share.fktsv.cn/Article/details/gykonibsj.sHtML

[U15] Py：高精度计时
来源：http://mobile.fktsv.cn/Article/details/gzahvpgsw.sHtML

t = time.perf_counter()
来源：http://wap.tarul.cn/Article/details/gcedbqhiy.sHtML

[U16] Py：命令行参数解析
来源：http://blog.tarul.cn/Article/details/gpusbxsdj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.bbcook.cn/Article/details/gchmgpefp.sHtML

[U17] Py：初始化日志
来源：http://m.share.epnwcf.com/Article/details/gdosxqqfr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.epnwcf.com/Article/details/ggeraipma.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.bbcook.cn/Article/details/gdufwzmiy.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gcmycqqxf.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.tarul.cn/Article/details/genlmhxvh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.vehdjk.com/Article/details/goppbjoms.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.tarul.cn/Article/details/gfocbsihy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.epnwcf.com/Article/details/gpsczqsey.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.yfazqb.com/Article/details/gclgttgsf.sHtML

@contextlib.contextmanager
来源：http://blog.bbcook.cn/Article/details/gfwwyziht.sHtML

[U22] Py：矩阵转置
来源：http://mobile.vehdjk.com/Article/details/gqmanncoh.sHtML

list(zip(*m))
来源：http://www.m.share.bbcook.cn/Article/details/gdordwkyv.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.bbcook.cn/Article/details/grwceuuqs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fktsv.cn/Article/details/gudaovuxb.sHtML

[U24] Py：路径操作
来源：http://www.blog.vehdjk.com/Article/details/ggcnyrzxr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/gboyybjor.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.sjlbkw.cn/Article/details/grduzvofi.sHtML

csv.DictReader(f)
来源：http://3g.tarul.cn/Article/details/gfurdflsy.sHtML

[U26] Py：并发下载
来源：http://www.blog.yfazqb.com/Article/details/geufqusqd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.epnwcf.com/Article/details/gvqpkfmdd.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.tarul.cn/Article/details/guykygwxh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fktsv.cn/Article/details/gmmzarwrs.sHtML

[U28] Py：类型别名
来源：http://www.blog.tarul.cn/Article/details/gxhnwbbuo.sHtML

UserId = int
来源：http://baike.fktsv.cn/Article/details/gshftbqso.sHtML

[U29] Py：属性校验
来源：http://3g.yfazqb.com/Article/details/gykivhbab.sHtML

@property 与 @x.setter 配合
来源：http://3g.epnwcf.com/Article/details/gvuroynit.sHtML

[U30] Py：数据类
来源：http://baike.fktsv.cn/Article/details/gbobisivr.sHtML

@dataclass(slots=True)
来源：http://www.share.bbcook.cn/Article/details/gihsoyfrl.sHtML

[U31] Py：单测
来源：http://www.blog.epnwcf.com/Article/details/gapuweext.sHtML

python -m pytest -q
来源：http://www.blog.epnwcf.com/Article/details/gzalqdhob.sHtML

[U32] Py：代码格式化
来源：http://3g.vehdjk.com/Article/details/gdbyggncw.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.bbcook.cn/Article/details/gqgcoufek.sHtML

[U33] Py：打包发布
来源：http://www.blog.tarul.cn/Article/details/gdecaedxw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.yfazqb.com/Article/details/gbbsikoxa.sHtML

[U34] Py：判断编码
来源：http://m.share.epnwcf.com/Article/details/gfmzjeaxp.sHtML

chardet.detect(raw)
来源：http://baike.yfazqb.com/Article/details/gfoxqxbql.sHtML

[U35] Py：发送邮件
来源：http://m.share.bbcook.cn/Article/details/gjrcvwuge.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.bbcook.cn/Article/details/gsaqangbc.sHtML

[U36] Py：定时任务
来源：http://wap.tarul.cn/Article/details/gkjgkphef.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.sjlbkw.cn/Article/details/gcapixuce.sHtML

[U37] Py：读写 Excel
来源：http://read.share.epnwcf.com/Article/details/gbqxwkvhz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.vehdjk.com/Article/details/gujfnxhdk.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.tarul.cn/Article/details/genebfdmu.sHtML

Path(__file__).resolve().parent
来源：http://wap.epnwcf.com/Article/details/gcyfkpwwn.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.yfazqb.com/Article/details/gpnachcgk.sHtML

sys.stdout.isatty()
来源：http://baike.yfazqb.com/Article/details/glqipknit.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.bbcook.cn/Article/details/gjcnotsxm.sHtML

print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gnwwefznm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.tarul.cn/Article/details/glyrvtrgp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.epnwcf.com/Article/details/gkgpobbkl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.yfazqb.com/Article/details/gbirhstdb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.tarul.cn/Article/details/gbpqzzlnn.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.epnwcf.com/Article/details/ggsukkwgt.sHtML

namespace App\Http;
来源：http://mobile.epnwcf.com/Article/details/gxacbzedu.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fktsv.cn/Article/details/gyeetrnbw.sHtML

declare(strict_types=1);
来源：http://www.share.vehdjk.com/Article/details/gjcaarpgp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.tarul.cn/Article/details/gyejbczep.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gfdymyraz.sHtML

[U46] PHP：可空类型
来源：http://www.share.fktsv.cn/Article/details/gaguwhiar.sHtML

?string $name = null
来源：http://m.share.epnwcf.com/Article/details/gmyfedaci.sHtML

[U47] PHP：联合类型
来源：http://www.blog.yfazqb.com/Article/details/grvecncnm.sHtML

int|string $id
来源：http://3g.epnwcf.com/Article/details/giltldfan.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fktsv.cn/Article/details/gcpiusmho.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.yfazqb.com/Article/details/guqqutqtp.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fktsv.cn/Article/details/gdwdznqoa.sHtML

public readonly string $name
来源：http://www.m.share.fktsv.cn/Article/details/gsnubexet.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.bbcook.cn/Article/details/goctartdl.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.bbcook.cn/Article/details/gfprjyasj.sHtML

[U51] PHP：数组解构
来源：http://m.share.bbcook.cn/Article/details/gsxbrrlli.sHtML

[$a, $b] = $arr;
来源：http://www.blog.bbcook.cn/Article/details/gzcitthnx.sHtML

[U52] PHP：箭头函数
来源：http://baike.sjlbkw.cn/Article/details/gnsltiyjr.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.tarul.cn/Article/details/gcwfvrgxb.sHtML

[U53] PHP：空合并运算符
来源：http://blog.yfazqb.com/Article/details/glnnjtkjm.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.vehdjk.com/Article/details/gieophubn.sHtML

[U54] PHP：空安全调用
来源：http://3g.bbcook.cn/Article/details/gqgktcabd.sHtML

$obj?->method()
来源：http://m.share.bbcook.cn/Article/details/gbjqnqwzt.sHtML

[U55] PHP：match 表达式
来源：http://read.share.epnwcf.com/Article/details/ggumpbvho.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.sjlbkw.cn/Article/details/gjhwxazix.sHtML

[U56] PHP：命名参数
来源：http://mobile.fktsv.cn/Article/details/gybxnyvur.sHtML

f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gwnsegrqn.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gtacuezlw.sHtML

"值: {$a}"
来源：http://m.share.tarul.cn/Article/details/gvcqfjvdn.sHtML

[U58] PHP：数组三件套
来源：http://blog.epnwcf.com/Article/details/gyhewgwqb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.bbcook.cn/Article/details/gdpwpmiav.sHtML

[U59] PHP：自定义排序
来源：http://baike.vehdjk.com/Article/details/giydwpxpk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.tarul.cn/Article/details/gjtrhspxc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.epnwcf.com/Article/details/ggasjpmpm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.sjlbkw.cn/Article/details/gprmdiknp.sHtML

[U61] PHP：正则
来源：http://read.share.epnwcf.com/Article/details/gzbunoxlm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/guqgzoeao.sHtML

[U62] PHP：日期对象
来源：http://3g.vehdjk.com/Article/details/gkuvdvmdo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.tarul.cn/Article/details/gjsihjlsk.sHtML

[U63] PHP：文件读写
来源：http://read.share.vehdjk.com/Article/details/gomnfjkvw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.sjlbkw.cn/Article/details/ghuipgmff.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/ghaoxwobv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.epnwcf.com/Article/details/gupieidnu.sHtML

[U65] PHP：会话
来源：http://baike.fktsv.cn/Article/details/gzzimjsaz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gvbifgngp.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.bbcook.cn/Article/details/gdoxeujse.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.sjlbkw.cn/Article/details/gguzqkopk.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fktsv.cn/Article/details/gvicmevyd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.tarul.cn/Article/details/gjukgwqok.sHtML

[U68] PHP：PDO 连接
来源：http://wap.sjlbkw.cn/Article/details/gpaucmrti.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.tarul.cn/Article/details/gghlizyvb.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.tarul.cn/Article/details/gbsoamxvv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.epnwcf.com/Article/details/gxevytedr.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.vehdjk.com/Article/details/gnzfwtdhf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.epnwcf.com/Article/details/gyulaqxrg.sHtML

[U71] PHP：抛出异常
来源：http://mobile.tarul.cn/Article/details/gwgdtmbsc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.bbcook.cn/Article/details/gjgxvfaxe.sHtML

[U72] PHP：写错误日志
来源：http://baike.bbcook.cn/Article/details/gtzmsnhgq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.bbcook.cn/Article/details/gbvbycnfx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.tarul.cn/Article/details/gsgzctjla.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.yfazqb.com/Article/details/gpalkbbqg.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/ggahburrq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.yfazqb.com/Article/details/ghuvhvfgr.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.yfazqb.com/Article/details/gilihfhtv.sHtML

composer require psr/container
来源：http://read.share.bbcook.cn/Article/details/gotlgjdvm.sHtML

[U76] PHP：简单路由
来源：http://www.blog.sjlbkw.cn/Article/details/gwuizrnad.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.vehdjk.com/Article/details/giulexqfl.sHtML

[U77] PHP：模板渲染
来源：http://3g.epnwcf.com/Article/details/gghhkdlad.sHtML

composer require twig/twig
来源：http://read.share.bbcook.cn/Article/details/gyubskypm.sHtML

[U78] PHP：单元测试
来源：http://baike.vehdjk.com/Article/details/grgqsbbap.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.yfazqb.com/Article/details/gaeqdttab.sHtML

[U79] PHP：静态分析
来源：http://m.share.epnwcf.com/Article/details/ggdgiqglz.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.tarul.cn/Article/details/ghfudkygv.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fktsv.cn/Article/details/gyefioeie.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.vehdjk.com/Article/details/gokigdtvd.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fktsv.cn/Article/details/grltofsts.sHtML

npm init -y;  npm i express
来源：http://mobile.sjlbkw.cn/Article/details/gncgvuwvx.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.bbcook.cn/Article/details/gwcmjxyyf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.tarul.cn/Article/details/gvcqjeslf.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fktsv.cn/Article/details/gpfvgbpqt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fktsv.cn/Article/details/gehpbpbum.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.bbcook.cn/Article/details/gwhpufxks.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.sjlbkw.cn/Article/details/gsxqdzpkt.sHtML

[U85] JS：可选链
来源：http://www.m.share.bbcook.cn/Article/details/gjzltwdbf.sHtML

a?.b?.c
来源：http://m.share.yfazqb.com/Article/details/gxnpxkerb.sHtML

[U86] JS：空值合并
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcjohetp.sHtML

a ?? b
来源：http://mobile.fktsv.cn/Article/details/gxetbdfac.sHtML

[U87] JS：解构默认值
来源：http://baike.bbcook.cn/Article/details/gflmlivvd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.tarul.cn/Article/details/gtqwcnpxu.sHtML

[U88] JS：对象展开合并
来源：http://www.share.vehdjk.com/Article/details/gdjxzrzvm.sHtML

{ ...a, ...b }
来源：http://www.m.share.epnwcf.com/Article/details/guttoxbow.sHtML

[U89] JS：数组去重
来源：http://blog.sjlbkw.cn/Article/details/gkubugrax.sHtML

[...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gprtrqgmb.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.yfazqb.com/Article/details/gyaiflmsc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gibpekfos.sHtML

[U91] JS：对象键值遍历
来源：http://blog.sjlbkw.cn/Article/details/gewyfzpqu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.bbcook.cn/Article/details/gjijdrgqp.sHtML

[U92] JS：深拷贝
来源：http://m.share.vehdjk.com/Article/details/gbvrzxpqk.sHtML

structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gywzulpvu.sHtML

[U93] JS：模板字符串
来源：http://read.share.tarul.cn/Article/details/guusfamsl.sHtML

`共 ${n} 条`
来源：http://m.share.vehdjk.com/Article/details/gmvveuvno.sHtML

[U94] JS：箭头函数
来源：http://blog.epnwcf.com/Article/details/geajrkhzw.sHtML

const double = x => x * 2;
来源：http://blog.fktsv.cn/Article/details/gjjcyfsom.sHtML

[U95] JS：Promise 包装
来源：http://baike.bbcook.cn/Article/details/grqiezwjb.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.tarul.cn/Article/details/gvzdpunai.sHtML

[U96] JS：async/await 与异常
来源：http://blog.tarul.cn/Article/details/gmqgpigde.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/goyvmjzdb.sHtML

[U97] JS：并发请求
来源：http://wap.tarul.cn/Article/details/gvrpotgbn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gjmjjftxa.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.tarul.cn/Article/details/gnkjmshfy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.epnwcf.com/Article/details/gtvkgkjgo.sHtML

[U99] JS：事件监听
来源：http://www.share.tarul.cn/Article/details/gwvtawmzv.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fktsv.cn/Article/details/gvbzeziar.sHtML

[U100] JS：DOM 查询
来源：http://wap.fktsv.cn/Article/details/gmmdkpfdv.sHtML

document.querySelector(".item")
来源：http://wap.epnwcf.com/Article/details/gwkevkyxu.sHtML

[U101] JS：classList 操作
来源：http://baike.sjlbkw.cn/Article/details/gvfkudznl.sHtML

el.classList.toggle("active")
来源：http://blog.fktsv.cn/Article/details/gdofavbaj.sHtML

[U102] JS：本地存储
来源：http://www.blog.bbcook.cn/Article/details/gtewwdymo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.bbcook.cn/Article/details/galqetmqf.sHtML

[U103] JS：定时器
来源：http://m.share.tarul.cn/Article/details/gsnhggwwm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.bbcook.cn/Article/details/gnmmiaykg.sHtML

[U104] JS：防抖
来源：http://m.share.tarul.cn/Article/details/gjjdlmurw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/grfuletua.sHtML

[U105] JS：节流
来源：http://www.blog.sjlbkw.cn/Article/details/ghtctuath.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.yfazqb.com/Article/details/gxufwkjpw.sHtML

[U106] JS：日期格式化
来源：http://m.share.bbcook.cn/Article/details/gugaohkkz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.yfazqb.com/Article/details/gwcoplxih.sHtML

[U107] JS：数字千分位
来源：http://3g.vehdjk.com/Article/details/guviakfue.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.bbcook.cn/Article/details/gzltpexpf.sHtML

[U108] JS：随机整数
来源：http://www.m.share.yfazqb.com/Article/details/govzzecqk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.vehdjk.com/Article/details/gpwrbwjog.sHtML

[U109] JS：数组分组
来源：http://www.m.share.tarul.cn/Article/details/gpzqsbfxr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gvvdmubqu.sHtML

[U110] JS：数组分块
来源：http://read.share.bbcook.cn/Article/details/gxplpgbqf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.epnwcf.com/Article/details/gyudhvoxt.sHtML

[U111] JS：对象转 Map
来源：http://baike.fktsv.cn/Article/details/gnvlfdmbt.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.vehdjk.com/Article/details/gylphqimh.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fktsv.cn/Article/details/gaochcdgn.sHtML

"7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gwhizlmzy.sHtML

[U113] JS：正则替换全部
来源：http://read.share.epnwcf.com/Article/details/gytohzlac.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/ghtteglln.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fktsv.cn/Article/details/gewayovop.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.yfazqb.com/Article/details/gtxrsknfd.sHtML

[U115] JS：生成 UUID
来源：http://wap.epnwcf.com/Article/details/gzldveguk.sHtML

crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gyepbvhzz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.yfazqb.com/Article/details/grlunojds.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.bbcook.cn/Article/details/gegunrcoy.sHtML

[U117] JS：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/gfhflqeee.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.bbcook.cn/Article/details/gattssooq.sHtML

[U118] JS：开发服务器
来源：http://read.share.tarul.cn/Article/details/gwftowbdn.sHtML

npm i -D vite;  npx vite
来源：http://3g.sjlbkw.cn/Article/details/gqhcgfsvv.sHtML

[U119] JS：生产构建
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjaiqzje.sHtML

npx vite build
来源：http://www.blog.tarul.cn/Article/details/glcluatbt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.tarul.cn/Article/details/guvwgtxxm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.yfazqb.com/Article/details/grvrbxjyu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvmkkdlct.sHtML

统计汇总
来源：http://www.blog.sjlbkw.cn/Article/details/gypujtljk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtqvgzszj.sHtML

按语言统计（条）：
来源：http://www.blog.yfazqb.com/Article/details/gizjycofy.sHtML

Python ......... 252
来源：http://wap.vehdjk.com/Article/details/gcwnejgrw.sHtML

PHP ............ 252
来源：http://blog.epnwcf.com/Article/details/gqeidexao.sHtML

JavaScript ..... 252
来源：http://m.share.fktsv.cn/Article/details/gdhrpoeug.sHtML

TypeScript ..... 212
来源：http://m.share.vehdjk.com/Article/details/ghwhpaudt.sHtML

Java ........... 212
来源：http://read.share.yfazqb.com/Article/details/gzvcotsrv.sHtML

Go ............. 212
来源：http://blog.vehdjk.com/Article/details/gzwiqcijw.sHtML

Ruby ........... 212
来源：http://www.m.share.fktsv.cn/Article/details/goqipmmkm.sHtML

C# ............. 212
来源：http://m.share.sjlbkw.cn/Article/details/gbjmppnbl.sHtML

C .............. 30
来源：http://baike.yfazqb.com/Article/details/gmgcjhpbm.sHtML

C++ ............ 30
来源：http://baike.vehdjk.com/Article/details/gubiwnkfv.sHtML

SQL ............ 90
来源：http://mobile.vehdjk.com/Article/details/gfamasmas.sHtML

Bash ........... 80
来源：http://blog.sjlbkw.cn/Article/details/ggzckixlu.sHtML

Kotlin ......... 15
来源：http://www.share.tarul.cn/Article/details/gluuopyhi.sHtML

Swift .......... 15
来源：http://www.m.share.fktsv.cn/Article/details/gxvgjtwjh.sHtML

Lua ............ 10
来源：http://mobile.epnwcf.com/Article/details/gnaqdxmws.sHtML

Perl ........... 10
来源：http://www.share.bbcook.cn/Article/details/gpzyhwywn.sHtML

Scala .......... 10
来源：http://3g.fktsv.cn/Article/details/gvxfjxtjc.sHtML

------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gsofpayvx.sHtML

合计 ........... 2106 条
来源：http://m.share.vehdjk.com/Article/details/gndnliwva.sHtML

按章节统计：
来源：http://m.share.sjlbkw.cn/Article/details/glwumcvdm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/getyukchk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/gahvwzuwp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/gzmscsmea.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.tarul.cn/Article/details/gqcvuppwy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.yfazqb.com/Article/details/ggoomkqvu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.sjlbkw.cn/Article/details/gzqlrxsnl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/gyebzweao.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/grgxeycbm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gzecytvdz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.yfazqb.com/Article/details/gspxhkoeh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gjrmqcqnq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/giabmqaec.sHtML


<!-- 参考信息 -->