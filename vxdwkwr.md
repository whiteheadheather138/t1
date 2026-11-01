代发 wailian999

val a = 1;  var b = 2
来源：http://read.share.fktsv.cn/Article/details/gjamwlhed.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gxamdwhhj.sHtML

s"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/gzysintal.sHtML

[T54] Scala：集合映射
来源：http://m.share.fktsv.cn/Article/details/gyqyornpv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.epnwcf.com/Article/details/grvbpyjqf.sHtML

[T55] Scala：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gnmlxhkme.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.yfazqb.com/Article/details/gypnuphnq.sHtML

[T56] Scala：样例类
来源：http://www.blog.fktsv.cn/Article/details/gjmduzlkv.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/giqoyneoj.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/giqohmggd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/gqvdkernj.sHtML

[T58] Scala：函数定义
来源：http://wap.fktsv.cn/Article/details/gyjgtzglx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.tarul.cn/Article/details/gnwcgtxsj.sHtML

[T59] Scala：循环
来源：http://www.blog.bbcook.cn/Article/details/glcxhaeik.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gcphucgos.sHtML

[T60] Scala：折叠
来源：http://mobile.yfazqb.com/Article/details/gktjzxmge.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/gmojivisp.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gpjhqtwtn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbvbpxbr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/geqtnnjic.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fktsv.cn/Article/details/gxzyeslib.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fktsv.cn/Article/details/gnyphwnxy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.epnwcf.com/Article/details/gmobdtcwx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fktsv.cn/Article/details/gyyzvahml.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.vehdjk.com/Article/details/gxukqnath.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gfxktvdfw.sHtML

[U04] Py：变量调试打印
来源：http://wap.tarul.cn/Article/details/gorhbbino.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.epnwcf.com/Article/details/giegdmnws.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fktsv.cn/Article/details/gohldrqng.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gkffguqzz.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fktsv.cn/Article/details/gaiuqxdca.sHtML

{**a, **b}
来源：http://wap.epnwcf.com/Article/details/ggkkyqhtr.sHtML

[U07] Py：反转字典键值
来源：http://www.share.sjlbkw.cn/Article/details/gqlzlaukw.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.yfazqb.com/Article/details/gfanxtmul.sHtML

[U08] Py：展平二维列表
来源：http://wap.fktsv.cn/Article/details/ghvzqhvoc.sHtML

[y for x in nested for y in x]
来源：http://wap.tarul.cn/Article/details/gjqdcglyq.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.bbcook.cn/Article/details/gbqihkruo.sHtML

max(d, key=d.get)
来源：http://mobile.fktsv.cn/Article/details/ggtjevcpb.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fktsv.cn/Article/details/gkkieecxl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.sjlbkw.cn/Article/details/gyhlynpty.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fktsv.cn/Article/details/ghmpzotyv.sHtML

(x * 2 for x in arr)
来源：http://www.share.vehdjk.com/Article/details/gonykqsdw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.epnwcf.com/Article/details/guuvmgeih.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gdullimaf.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.tarul.cn/Article/details/gqelotivc.sHtML

deque(maxlen=10)
来源：http://mobile.vehdjk.com/Article/details/gyjgizyjk.sHtML

[U14] Py：分组收集到列表
来源：http://blog.tarul.cn/Article/details/gysivhwbp.sHtML

defaultdict(list)
来源：http://www.blog.vehdjk.com/Article/details/ghdzklkil.sHtML

[U15] Py：高精度计时
来源：http://wap.vehdjk.com/Article/details/gadyxprbi.sHtML

t = time.perf_counter()
来源：http://wap.vehdjk.com/Article/details/gjqsbwtoz.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.tarul.cn/Article/details/gmumckfrw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.bbcook.cn/Article/details/gosrylfno.sHtML

[U17] Py：初始化日志
来源：http://mobile.vehdjk.com/Article/details/gwxtjdoqi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.tarul.cn/Article/details/ghibhmeww.sHtML

[U18] Py：预编译正则
来源：http://blog.bbcook.cn/Article/details/ggkbmjocx.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.tarul.cn/Article/details/gtfkmwyim.sHtML

[U19] Py：正则替换带回调
来源：http://3g.tarul.cn/Article/details/gntwkdqox.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fktsv.cn/Article/details/gcfvdkbnz.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.tarul.cn/Article/details/gqssnskpd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.vehdjk.com/Article/details/glpgxqaus.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.epnwcf.com/Article/details/gtoohztdj.sHtML

@contextlib.contextmanager
来源：http://wap.bbcook.cn/Article/details/gyehqxggt.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fktsv.cn/Article/details/gvbvkutvt.sHtML

list(zip(*m))
来源：http://blog.vehdjk.com/Article/details/ggdebbwzs.sHtML

[U23] Py：分块读取大文件
来源：http://3g.vehdjk.com/Article/details/gspetjbkw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.vehdjk.com/Article/details/gyffdzeiz.sHtML

[U24] Py：路径操作
来源：http://blog.tarul.cn/Article/details/gkuqhjble.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.tarul.cn/Article/details/gsvxqduti.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.vehdjk.com/Article/details/ggkomrqal.sHtML

csv.DictReader(f)
来源：http://baike.sjlbkw.cn/Article/details/gprhbtafy.sHtML

[U26] Py：并发下载
来源：http://m.share.yfazqb.com/Article/details/gjumctpti.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.sjlbkw.cn/Article/details/gigehnfml.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.bbcook.cn/Article/details/gewhgtrbw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.tarul.cn/Article/details/guthkewzj.sHtML

[U28] Py：类型别名
来源：http://www.m.share.bbcook.cn/Article/details/grerqtvag.sHtML

UserId = int
来源：http://www.blog.tarul.cn/Article/details/guinzxsuf.sHtML

[U29] Py：属性校验
来源：http://www.share.bbcook.cn/Article/details/gqidqtafn.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.tarul.cn/Article/details/gmwouwspq.sHtML

[U30] Py：数据类
来源：http://www.blog.yfazqb.com/Article/details/govtkgvqt.sHtML

@dataclass(slots=True)
来源：http://mobile.tarul.cn/Article/details/gbpgtatpv.sHtML

[U31] Py：单测
来源：http://www.blog.yfazqb.com/Article/details/gtllbcuvd.sHtML

python -m pytest -q
来源：http://m.share.fktsv.cn/Article/details/guxlllaji.sHtML

[U32] Py：代码格式化
来源：http://www.share.tarul.cn/Article/details/gbhtjwrdb.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fktsv.cn/Article/details/gepgnwhon.sHtML

[U33] Py：打包发布
来源：http://m.share.tarul.cn/Article/details/gpluyrdbq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fktsv.cn/Article/details/gxcddpvnl.sHtML

[U34] Py：判断编码
来源：http://read.share.tarul.cn/Article/details/gbzkkpumj.sHtML

chardet.detect(raw)
来源：http://m.share.epnwcf.com/Article/details/gxnudnmxt.sHtML

[U35] Py：发送邮件
来源：http://read.share.tarul.cn/Article/details/gbpkyjtjp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.yfazqb.com/Article/details/garxsrghe.sHtML

[U36] Py：定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gtxulltks.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fktsv.cn/Article/details/gmrhxstzx.sHtML

[U37] Py：读写 Excel
来源：http://3g.vehdjk.com/Article/details/gothvqksb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.bbcook.cn/Article/details/gjjtyigjo.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.tarul.cn/Article/details/ggousskdx.sHtML

Path(__file__).resolve().parent
来源：http://m.share.yfazqb.com/Article/details/gpscjwitl.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.bbcook.cn/Article/details/grhvwfrho.sHtML

sys.stdout.isatty()
来源：http://baike.bbcook.cn/Article/details/ggdvgxmfb.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.epnwcf.com/Article/details/gpatabbqo.sHtML

print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/glsdgbimr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.epnwcf.com/Article/details/gxhdhiesr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.tarul.cn/Article/details/gdrwlgrae.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.epnwcf.com/Article/details/gvcjyxnnp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.epnwcf.com/Article/details/grydjefcr.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.bbcook.cn/Article/details/gsxhaycdb.sHtML

namespace App\Http;
来源：http://m.share.sjlbkw.cn/Article/details/gvwykttpj.sHtML

[U44] PHP：开启严格类型
来源：http://blog.vehdjk.com/Article/details/ghczvceyt.sHtML

declare(strict_types=1);
来源：http://mobile.epnwcf.com/Article/details/gaamovrtf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.yfazqb.com/Article/details/gnqokdvwk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gyeqrnwlr.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.epnwcf.com/Article/details/gupjlyiff.sHtML

?string $name = null
来源：http://www.m.share.vehdjk.com/Article/details/gozulrfit.sHtML

[U47] PHP：联合类型
来源：http://wap.fktsv.cn/Article/details/gmqdasndv.sHtML

int|string $id
来源：http://www.m.share.tarul.cn/Article/details/gggejcnot.sHtML

[U48] PHP：纯枚举
来源：http://wap.sjlbkw.cn/Article/details/gtvbmfart.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.sjlbkw.cn/Article/details/guexbybhy.sHtML

[U49] PHP：只读属性
来源：http://wap.vehdjk.com/Article/details/gbtjnxype.sHtML

public readonly string $name
来源：http://baike.epnwcf.com/Article/details/gpbhutpiz.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.bbcook.cn/Article/details/gjucqxjif.sHtML

public function __construct(private int $id) {}
来源：http://blog.tarul.cn/Article/details/gvroqyoyz.sHtML

[U51] PHP：数组解构
来源：http://read.share.tarul.cn/Article/details/gppraxyse.sHtML

[$a, $b] = $arr;
来源：http://mobile.fktsv.cn/Article/details/gtvtrlfce.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/grgybwade.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.epnwcf.com/Article/details/gradnuxzc.sHtML

[U53] PHP：空合并运算符
来源：http://3g.sjlbkw.cn/Article/details/gulhnxmzz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.yfazqb.com/Article/details/guvdrhzyw.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.sjlbkw.cn/Article/details/gpuwxkoic.sHtML

$obj?->method()
来源：http://www.blog.epnwcf.com/Article/details/gdsjseawo.sHtML

[U55] PHP：match 表达式
来源：http://wap.bbcook.cn/Article/details/gsthkfagq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.epnwcf.com/Article/details/gtioyhfxo.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.tarul.cn/Article/details/gldmxtoeq.sHtML

f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/gtvslyomk.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gkpdgecmw.sHtML

"值: {$a}"
来源：http://www.blog.sjlbkw.cn/Article/details/gaunyohpu.sHtML

[U58] PHP：数组三件套
来源：http://blog.sjlbkw.cn/Article/details/gvtplllkl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.yfazqb.com/Article/details/gfcrgrsfl.sHtML

[U59] PHP：自定义排序
来源：http://m.share.epnwcf.com/Article/details/ggxjhnmgp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/gyopishit.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/ghuxzmeah.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fktsv.cn/Article/details/gxovyccwn.sHtML

[U61] PHP：正则
来源：http://baike.yfazqb.com/Article/details/gczkvdevo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.epnwcf.com/Article/details/gcyrqojfl.sHtML

[U62] PHP：日期对象
来源：http://read.share.bbcook.cn/Article/details/gjznhwixt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.epnwcf.com/Article/details/goczmuhek.sHtML

[U63] PHP：文件读写
来源：http://blog.sjlbkw.cn/Article/details/gxutyajjc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.bbcook.cn/Article/details/ghjdaothx.sHtML

[U64] PHP：目录遍历
来源：http://baike.tarul.cn/Article/details/gvbxjkrrs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.epnwcf.com/Article/details/gpjhyzzkm.sHtML

[U65] PHP：会话
来源：http://blog.bbcook.cn/Article/details/gipirzxqd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.yfazqb.com/Article/details/gpyrhbnhl.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.sjlbkw.cn/Article/details/gnjdphcnp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.epnwcf.com/Article/details/genpsdpgg.sHtML

[U67] PHP：处理文件上传
来源：http://blog.yfazqb.com/Article/details/gzrtncmfl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.sjlbkw.cn/Article/details/gbtexnqxg.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.sjlbkw.cn/Article/details/gahwgbmtg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fktsv.cn/Article/details/glluxwgbq.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.bbcook.cn/Article/details/gydtgjsvn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.epnwcf.com/Article/details/gietgusbm.sHtML

[U70] PHP：PDO 事务
来源：http://wap.vehdjk.com/Article/details/gnaxkgzim.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.tarul.cn/Article/details/gyamteblb.sHtML

[U71] PHP：抛出异常
来源：http://read.share.tarul.cn/Article/details/gemmnwlzk.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.epnwcf.com/Article/details/gsgvqjcds.sHtML

[U72] PHP：写错误日志
来源：http://read.share.sjlbkw.cn/Article/details/gtuzqfnhc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fktsv.cn/Article/details/gzajhbgvs.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.yfazqb.com/Article/details/gkmsqrvpp.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fktsv.cn/Article/details/gejzyiggf.sHtML

[U74] PHP：读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/gnwplayfr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.vehdjk.com/Article/details/grtcmjcwz.sHtML

[U75] PHP：依赖注入
来源：http://blog.fktsv.cn/Article/details/gbjmbwxlr.sHtML

composer require psr/container
来源：http://www.blog.vehdjk.com/Article/details/grinrhtrq.sHtML

[U76] PHP：简单路由
来源：http://mobile.vehdjk.com/Article/details/gjrpihott.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.yfazqb.com/Article/details/gttmsiglc.sHtML

[U77] PHP：模板渲染
来源：http://m.share.tarul.cn/Article/details/ghquhsvfb.sHtML

composer require twig/twig
来源：http://www.m.share.fktsv.cn/Article/details/gqjsvzwbu.sHtML

[U78] PHP：单元测试
来源：http://wap.fktsv.cn/Article/details/guvwenusu.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.epnwcf.com/Article/details/ghwyjwzbj.sHtML

[U79] PHP：静态分析
来源：http://m.share.vehdjk.com/Article/details/gmtldmpng.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.tarul.cn/Article/details/gvsxvrewa.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.yfazqb.com/Article/details/ghnkgmkid.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.sjlbkw.cn/Article/details/ggkskurgw.sHtML

[U81] JS：初始化项目
来源：http://read.share.fktsv.cn/Article/details/grbbpcmcm.sHtML

npm init -y;  npm i express
来源：http://wap.vehdjk.com/Article/details/grkcrvtlw.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.vehdjk.com/Article/details/gxdizjymg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.bbcook.cn/Article/details/gksmvwlmz.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.sjlbkw.cn/Article/details/glqrmgcbr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gjftndtev.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fktsv.cn/Article/details/gpgtylzpy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.sjlbkw.cn/Article/details/gxdlhcraz.sHtML

[U85] JS：可选链
来源：http://www.m.share.yfazqb.com/Article/details/gdvhjvvqo.sHtML

a?.b?.c
来源：http://baike.tarul.cn/Article/details/gmktllrno.sHtML

[U86] JS：空值合并
来源：http://read.share.vehdjk.com/Article/details/gfoncpbal.sHtML

a ?? b
来源：http://m.share.fktsv.cn/Article/details/guezvldnj.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gxeactlfy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.sjlbkw.cn/Article/details/ggnsxfvce.sHtML

[U88] JS：对象展开合并
来源：http://www.share.tarul.cn/Article/details/gexpimktd.sHtML

{ ...a, ...b }
来源：http://m.share.yfazqb.com/Article/details/gxdbvswhq.sHtML

[U89] JS：数组去重
来源：http://baike.yfazqb.com/Article/details/gcsqxidma.sHtML

[...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gqrzcljhg.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fktsv.cn/Article/details/goedjteox.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/glzcbodcc.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fktsv.cn/Article/details/gqbwqaqeq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.sjlbkw.cn/Article/details/ggqqfkgmz.sHtML

[U92] JS：深拷贝
来源：http://mobile.epnwcf.com/Article/details/glqcebmyy.sHtML

structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gnnweutuy.sHtML

[U93] JS：模板字符串
来源：http://mobile.yfazqb.com/Article/details/gqymefghr.sHtML

`共 ${n} 条`
来源：http://3g.epnwcf.com/Article/details/gozsvaiyv.sHtML

[U94] JS：箭头函数
来源：http://baike.yfazqb.com/Article/details/goqjpxzzo.sHtML

const double = x => x * 2;
来源：http://www.share.epnwcf.com/Article/details/gznyduzpq.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.sjlbkw.cn/Article/details/gudiugosr.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.tarul.cn/Article/details/gaosgnelh.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.vehdjk.com/Article/details/gnketgppd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gjeyvbwoc.sHtML

[U97] JS：并发请求
来源：http://3g.tarul.cn/Article/details/gpsqinnrg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gliimyxcd.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.bbcook.cn/Article/details/gkctbfzbv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.yfazqb.com/Article/details/gxodxmdkv.sHtML

[U99] JS：事件监听
来源：http://baike.sjlbkw.cn/Article/details/gzgxbjamx.sHtML

el.addEventListener("click", e => {})
来源：http://wap.epnwcf.com/Article/details/gunboutvc.sHtML

[U100] JS：DOM 查询
来源：http://3g.yfazqb.com/Article/details/gbkgawxxx.sHtML

document.querySelector(".item")
来源：http://m.share.tarul.cn/Article/details/gneifmbpm.sHtML

[U101] JS：classList 操作
来源：http://mobile.vehdjk.com/Article/details/granbvsmz.sHtML

el.classList.toggle("active")
来源：http://m.share.sjlbkw.cn/Article/details/ghzqfoxul.sHtML

[U102] JS：本地存储
来源：http://mobile.fktsv.cn/Article/details/gvknwqyfx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.bbcook.cn/Article/details/gscvsgxih.sHtML

[U103] JS：定时器
来源：http://baike.tarul.cn/Article/details/gbgzfjgii.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fktsv.cn/Article/details/gkzgqtaxl.sHtML

[U104] JS：防抖
来源：http://read.share.fktsv.cn/Article/details/gnndugthd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/gzynddpvz.sHtML

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/gkdibmxqk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.tarul.cn/Article/details/gdhpmohei.sHtML

[U106] JS：日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/ggawpekau.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.yfazqb.com/Article/details/gdxvvrnli.sHtML

[U107] JS：数字千分位
来源：http://3g.fktsv.cn/Article/details/gapkofrse.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gdralbxth.sHtML

[U108] JS：随机整数
来源：http://www.share.yfazqb.com/Article/details/gxqjupbld.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.epnwcf.com/Article/details/gzgfccxbz.sHtML

[U109] JS：数组分组
来源：http://m.share.epnwcf.com/Article/details/gombalrxo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.sjlbkw.cn/Article/details/gzhlwytij.sHtML

[U110] JS：数组分块
来源：http://blog.epnwcf.com/Article/details/gdimlvkrm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.bbcook.cn/Article/details/gactjjpte.sHtML

[U111] JS：对象转 Map
来源：http://blog.sjlbkw.cn/Article/details/gqjgdvndq.sHtML

new Map(Object.entries(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gqwmhlceq.sHtML

[U112] JS：字符串补位
来源：http://m.share.epnwcf.com/Article/details/gdroshjlr.sHtML

"7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/goxmnkdcv.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.bbcook.cn/Article/details/guavthsgv.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/ghtfjomhy.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fktsv.cn/Article/details/gkuoexufj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/guvrgspjb.sHtML

[U115] JS：生成 UUID
来源：http://blog.yfazqb.com/Article/details/guaixkjgb.sHtML

crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gyrvisetj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.bbcook.cn/Article/details/gnymmfcfx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.tarul.cn/Article/details/ggdiqkozn.sHtML

[U117] JS：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gomckqmve.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.sjlbkw.cn/Article/details/grehhymfd.sHtML

[U118] JS：开发服务器
来源：http://blog.fktsv.cn/Article/details/gpbbeusoi.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.vehdjk.com/Article/details/gtxngqjkv.sHtML

[U119] JS：生产构建
来源：http://www.share.yfazqb.com/Article/details/gzibpjmbm.sHtML

npx vite build
来源：http://read.share.bbcook.cn/Article/details/grjhlyaow.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.epnwcf.com/Article/details/gzgzrkffj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.sjlbkw.cn/Article/details/gstmvddcl.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbjyqsxwk.sHtML

统计汇总
来源：http://www.blog.vehdjk.com/Article/details/gfqilcnvn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtgbsfcly.sHtML

按语言统计（条）：
来源：http://blog.bbcook.cn/Article/details/gtlylkbhh.sHtML

Python ......... 252
来源：http://wap.vehdjk.com/Article/details/gjhtprpmk.sHtML

PHP ............ 252
来源：http://baike.bbcook.cn/Article/details/gdstsmiap.sHtML

JavaScript ..... 252
来源：http://3g.epnwcf.com/Article/details/gukgxmkdx.sHtML

TypeScript ..... 212
来源：http://3g.fktsv.cn/Article/details/glzczojwe.sHtML

Java ........... 212
来源：http://www.blog.fktsv.cn/Article/details/gwbueomdz.sHtML

Go ............. 212
来源：http://www.m.share.bbcook.cn/Article/details/grmohydcu.sHtML

Ruby ........... 212
来源：http://baike.epnwcf.com/Article/details/gstrfzdgk.sHtML

C# ............. 212
来源：http://baike.fktsv.cn/Article/details/godzvmdna.sHtML

C .............. 30
来源：http://read.share.bbcook.cn/Article/details/gvxkflprm.sHtML

C++ ............ 30
来源：http://blog.sjlbkw.cn/Article/details/gcqlcmcts.sHtML

SQL ............ 90
来源：http://blog.fktsv.cn/Article/details/gxuemphvr.sHtML

Bash ........... 80
来源：http://mobile.fktsv.cn/Article/details/glzixifzv.sHtML

Kotlin ......... 15
来源：http://read.share.bbcook.cn/Article/details/gvqrwkjvy.sHtML

Swift .......... 15
来源：http://blog.sjlbkw.cn/Article/details/gmgtdxxmg.sHtML

Lua ............ 10
来源：http://3g.epnwcf.com/Article/details/gfbjglwax.sHtML

Perl ........... 10
来源：http://www.blog.epnwcf.com/Article/details/gcqwlpvfb.sHtML

Scala .......... 10
来源：http://www.m.share.fktsv.cn/Article/details/gmvtqipow.sHtML

------------------------------------
来源：http://www.share.tarul.cn/Article/details/germeukmr.sHtML

合计 ........... 2106 条
来源：http://www.m.share.yfazqb.com/Article/details/gzochbwjt.sHtML

按章节统计：
来源：http://read.share.vehdjk.com/Article/details/gqmekjvip.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.vehdjk.com/Article/details/gpsplhwfy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/ghzmxxbpt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gulnufdeu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gviqmuvnu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.bbcook.cn/Article/details/gyyipliup.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.yfazqb.com/Article/details/gaassqkfh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/gelcqjzti.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.epnwcf.com/Article/details/gdaarahto.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/ghjcwokmn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.bbcook.cn/Article/details/gsraueovt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gdatvkvuy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gigmqafel.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gkyhoupaw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.bbcook.cn/Article/details/gavdimmni.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.tarul.cn/Article/details/gzlnvtvuk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/geiixffrm.sHtML


<!-- 参考信息 -->