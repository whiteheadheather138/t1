代发 wailian999

val a = 1;  var b = 2
来源：http://wap.tarul.cn/Article/details/gegdrdlsn.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gfnhuvgoh.sHtML

s"值: $b"
来源：http://m.share.epnwcf.com/Article/details/gjuuavhyl.sHtML

[T54] Scala：集合映射
来源：http://mobile.bbcook.cn/Article/details/gbcqjhvhk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.epnwcf.com/Article/details/gmzsgqdhe.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/goqykyick.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fktsv.cn/Article/details/gtfvfcqbz.sHtML

[T56] Scala：样例类
来源：http://3g.bbcook.cn/Article/details/gxkwjcgke.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.epnwcf.com/Article/details/gfshdjipx.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fktsv.cn/Article/details/ggbtpzewk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.bbcook.cn/Article/details/gmzgazlwn.sHtML

[T58] Scala：函数定义
来源：http://m.share.fktsv.cn/Article/details/govibzieq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.epnwcf.com/Article/details/gmmmunjgw.sHtML

[T59] Scala：循环
来源：http://read.share.epnwcf.com/Article/details/gpsutnqur.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gaypgrtxb.sHtML

[T60] Scala：折叠
来源：http://www.share.vehdjk.com/Article/details/geipltgko.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.bbcook.cn/Article/details/ghhjgrkmx.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ghpyvlxwq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gpfxueyac.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/giivyaltq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.epnwcf.com/Article/details/gyuluitdu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.yfazqb.com/Article/details/ghmehmoly.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.vehdjk.com/Article/details/gjxhmnias.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.tarul.cn/Article/details/gdbxybesr.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.tarul.cn/Article/details/gbkpcajvu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.epnwcf.com/Article/details/gdhzftekt.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fktsv.cn/Article/details/gzobkxgjv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.yfazqb.com/Article/details/gjqpukiic.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.bbcook.cn/Article/details/gdrbiczxh.sHtML

list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/gipegghpi.sHtML

[U06] Py：合并两个字典
来源：http://m.share.tarul.cn/Article/details/gxrbisyyr.sHtML

{**a, **b}
来源：http://www.m.share.yfazqb.com/Article/details/gqfalmzmw.sHtML

[U07] Py：反转字典键值
来源：http://wap.bbcook.cn/Article/details/goxuhxawb.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.epnwcf.com/Article/details/gmdcznpyh.sHtML

[U08] Py：展平二维列表
来源：http://www.share.yfazqb.com/Article/details/ghhciellr.sHtML

[y for x in nested for y in x]
来源：http://3g.yfazqb.com/Article/details/glhyrvhvm.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.vehdjk.com/Article/details/gophdwbjd.sHtML

max(d, key=d.get)
来源：http://blog.fktsv.cn/Article/details/gyrxjtviv.sHtML

[U10] Py：按值排序字典
来源：http://3g.tarul.cn/Article/details/ghcriuoak.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.bbcook.cn/Article/details/ghszttrhz.sHtML

[U11] Py：生成器表达式
来源：http://read.share.vehdjk.com/Article/details/gqjlhmywf.sHtML

(x * 2 for x in arr)
来源：http://www.share.tarul.cn/Article/details/gufofipaq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.tarul.cn/Article/details/glxmxtvrc.sHtML

Counter(arr).most_common(3)
来源：http://mobile.tarul.cn/Article/details/gmyajiuws.sHtML

[U13] Py：固定长度队列
来源：http://baike.bbcook.cn/Article/details/gkyscuved.sHtML

deque(maxlen=10)
来源：http://wap.tarul.cn/Article/details/gxjygvrlb.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.bbcook.cn/Article/details/gqtfbwyfm.sHtML

defaultdict(list)
来源：http://blog.yfazqb.com/Article/details/gllpmmfsm.sHtML

[U15] Py：高精度计时
来源：http://baike.vehdjk.com/Article/details/ggulgitmi.sHtML

t = time.perf_counter()
来源：http://www.share.tarul.cn/Article/details/gcoiybmwr.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.sjlbkw.cn/Article/details/gzwlmnpah.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.bbcook.cn/Article/details/gofubbezk.sHtML

[U17] Py：初始化日志
来源：http://www.share.sjlbkw.cn/Article/details/gqwaxwbrf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.bbcook.cn/Article/details/gbkovryxh.sHtML

[U18] Py：预编译正则
来源：http://www.blog.bbcook.cn/Article/details/gvvgokluj.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.epnwcf.com/Article/details/gcylttkbf.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.vehdjk.com/Article/details/gfgyifqyb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.yfazqb.com/Article/details/gnuxvoqbj.sHtML

[U20] Py：缓存函数结果
来源：http://baike.bbcook.cn/Article/details/gmwpysivz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.tarul.cn/Article/details/gydlvdfdw.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.epnwcf.com/Article/details/gjarjotgj.sHtML

@contextlib.contextmanager
来源：http://3g.tarul.cn/Article/details/gjsrqmndf.sHtML

[U22] Py：矩阵转置
来源：http://baike.vehdjk.com/Article/details/gnevpvbhl.sHtML

list(zip(*m))
来源：http://mobile.sjlbkw.cn/Article/details/gpnysnrfd.sHtML

[U23] Py：分块读取大文件
来源：http://blog.yfazqb.com/Article/details/govmmfuos.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fktsv.cn/Article/details/gxnylfphg.sHtML

[U24] Py：路径操作
来源：http://m.share.epnwcf.com/Article/details/ggdiruvch.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gqrozyvhc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.epnwcf.com/Article/details/gbqhomftc.sHtML

csv.DictReader(f)
来源：http://read.share.yfazqb.com/Article/details/gadzqjfte.sHtML

[U26] Py：并发下载
来源：http://read.share.sjlbkw.cn/Article/details/gszqdtbla.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fktsv.cn/Article/details/gyndhijtz.sHtML

[U27] Py：异步 HTTP
来源：http://blog.bbcook.cn/Article/details/gburhvpds.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.bbcook.cn/Article/details/gfwplikig.sHtML

[U28] Py：类型别名
来源：http://www.share.yfazqb.com/Article/details/gdihvmtoy.sHtML

UserId = int
来源：http://www.blog.vehdjk.com/Article/details/gqsafjnpy.sHtML

[U29] Py：属性校验
来源：http://www.m.share.bbcook.cn/Article/details/gadhdmfpj.sHtML

@property 与 @x.setter 配合
来源：http://baike.vehdjk.com/Article/details/gvqmkslwy.sHtML

[U30] Py：数据类
来源：http://wap.vehdjk.com/Article/details/gusyhxujd.sHtML

@dataclass(slots=True)
来源：http://blog.sjlbkw.cn/Article/details/gkokkcjor.sHtML

[U31] Py：单测
来源：http://www.share.tarul.cn/Article/details/goxsafwma.sHtML

python -m pytest -q
来源：http://read.share.vehdjk.com/Article/details/gasjopwoy.sHtML

[U32] Py：代码格式化
来源：http://m.share.sjlbkw.cn/Article/details/glmspdovh.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.bbcook.cn/Article/details/gtupgozks.sHtML

[U33] Py：打包发布
来源：http://www.share.tarul.cn/Article/details/gtneqhaek.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.epnwcf.com/Article/details/gcvqehxxy.sHtML

[U34] Py：判断编码
来源：http://wap.vehdjk.com/Article/details/giaatwezm.sHtML

chardet.detect(raw)
来源：http://wap.sjlbkw.cn/Article/details/gcdvmiqhp.sHtML

[U35] Py：发送邮件
来源：http://mobile.epnwcf.com/Article/details/gnwbuaguo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.yfazqb.com/Article/details/ghrrfkmxq.sHtML

[U36] Py：定时任务
来源：http://wap.vehdjk.com/Article/details/gfillelhu.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.sjlbkw.cn/Article/details/gecbpoknj.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fktsv.cn/Article/details/gwdcxmpom.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.epnwcf.com/Article/details/gcloojrua.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.epnwcf.com/Article/details/gsvjzkpha.sHtML

Path(__file__).resolve().parent
来源：http://wap.fktsv.cn/Article/details/ghtkouzau.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.sjlbkw.cn/Article/details/gawwibfqa.sHtML

sys.stdout.isatty()
来源：http://m.share.vehdjk.com/Article/details/gbvplkyqm.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.tarul.cn/Article/details/gnekknuex.sHtML

print("err", file=sys.stderr)
来源：http://m.share.epnwcf.com/Article/details/gjzoilyll.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.vehdjk.com/Article/details/gkrqptyek.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.vehdjk.com/Article/details/gctejitcl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.epnwcf.com/Article/details/gixdvqjyc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.bbcook.cn/Article/details/gbrsozzee.sHtML

[U43] PHP：声明命名空间
来源：http://3g.tarul.cn/Article/details/gaccrmgvz.sHtML

namespace App\Http;
来源：http://www.blog.yfazqb.com/Article/details/gcbiqehql.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.yfazqb.com/Article/details/gubeumzdb.sHtML

declare(strict_types=1);
来源：http://www.m.share.bbcook.cn/Article/details/gsdlfefwa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.bbcook.cn/Article/details/glnzhjort.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gtlrhskdk.sHtML

[U46] PHP：可空类型
来源：http://wap.sjlbkw.cn/Article/details/gpggrpczx.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gmwlyxsqz.sHtML

[U47] PHP：联合类型
来源：http://read.share.tarul.cn/Article/details/gctvbpfpm.sHtML

int|string $id
来源：http://3g.vehdjk.com/Article/details/giyiwnqpy.sHtML

[U48] PHP：纯枚举
来源：http://3g.fktsv.cn/Article/details/gtbzuzoko.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fktsv.cn/Article/details/gyvpbtxeh.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.epnwcf.com/Article/details/gkrbllbcd.sHtML

public readonly string $name
来源：http://www.share.fktsv.cn/Article/details/gonqzwvqt.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.yfazqb.com/Article/details/gszqnkroh.sHtML

public function __construct(private int $id) {}
来源：http://read.share.vehdjk.com/Article/details/gujmhnznu.sHtML

[U51] PHP：数组解构
来源：http://www.blog.epnwcf.com/Article/details/ggkgkkooz.sHtML

[$a, $b] = $arr;
来源：http://read.share.yfazqb.com/Article/details/gtmucwgro.sHtML

[U52] PHP：箭头函数
来源：http://m.share.epnwcf.com/Article/details/gvoqmzqak.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.bbcook.cn/Article/details/gumeunojm.sHtML

[U53] PHP：空合并运算符
来源：http://3g.yfazqb.com/Article/details/gsscohyzo.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.sjlbkw.cn/Article/details/gagyehozd.sHtML

[U54] PHP：空安全调用
来源：http://3g.bbcook.cn/Article/details/gqvljcowl.sHtML

$obj?->method()
来源：http://m.share.fktsv.cn/Article/details/gtfrdhzxd.sHtML

[U55] PHP：match 表达式
来源：http://3g.bbcook.cn/Article/details/gdcgzerfh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.bbcook.cn/Article/details/grsgsvubl.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.tarul.cn/Article/details/gokdnbbcy.sHtML

f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/ghvdtfkvi.sHtML

[U57] PHP：字符串插值
来源：http://read.share.vehdjk.com/Article/details/glchwwreo.sHtML

"值: {$a}"
来源：http://www.m.share.yfazqb.com/Article/details/gojwanmkd.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.tarul.cn/Article/details/gsxxzzkyn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fktsv.cn/Article/details/gyyieoukn.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.tarul.cn/Article/details/gptnjlubq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.bbcook.cn/Article/details/gbcwsbytu.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.sjlbkw.cn/Article/details/gdedjpgvr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.bbcook.cn/Article/details/giftbrpvs.sHtML

[U61] PHP：正则
来源：http://www.blog.sjlbkw.cn/Article/details/gvjolvtmw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/gqwuwgbpb.sHtML

[U62] PHP：日期对象
来源：http://read.share.bbcook.cn/Article/details/giqyealvv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.vehdjk.com/Article/details/gcwdpsppw.sHtML

[U63] PHP：文件读写
来源：http://m.share.tarul.cn/Article/details/gtahawqdv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.sjlbkw.cn/Article/details/gizlkqtfd.sHtML

[U64] PHP：目录遍历
来源：http://baike.sjlbkw.cn/Article/details/gzvikqfup.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.tarul.cn/Article/details/gnwdopcoa.sHtML

[U65] PHP：会话
来源：http://www.share.vehdjk.com/Article/details/gtwynjlpu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gbraspbqk.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.tarul.cn/Article/details/gkfrctdxo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fktsv.cn/Article/details/gluzqqzmr.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fktsv.cn/Article/details/gorirawzg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.vehdjk.com/Article/details/gjtllbyyi.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.vehdjk.com/Article/details/ghdnlvtna.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.epnwcf.com/Article/details/gfweznndn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.yfazqb.com/Article/details/gdsdxxvqv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.vehdjk.com/Article/details/gqzfwwrqy.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.epnwcf.com/Article/details/gfxeafhhf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.tarul.cn/Article/details/gppqczdzf.sHtML

[U71] PHP：抛出异常
来源：http://baike.fktsv.cn/Article/details/gvwxgkejq.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.tarul.cn/Article/details/gepzzlyqb.sHtML

[U72] PHP：写错误日志
来源：http://read.share.tarul.cn/Article/details/gpuishcwm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.epnwcf.com/Article/details/gppwrqgsi.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.bbcook.cn/Article/details/gzuygxbuz.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.yfazqb.com/Article/details/gxprqvvkf.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/geuuqxnxf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.epnwcf.com/Article/details/gjrupwoku.sHtML

[U75] PHP：依赖注入
来源：http://www.share.bbcook.cn/Article/details/gculgcpoy.sHtML

composer require psr/container
来源：http://read.share.fktsv.cn/Article/details/gqeejeegk.sHtML

[U76] PHP：简单路由
来源：http://read.share.bbcook.cn/Article/details/gljeosxoi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.tarul.cn/Article/details/glpbuhnzo.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.yfazqb.com/Article/details/gvlljguds.sHtML

composer require twig/twig
来源：http://wap.epnwcf.com/Article/details/gnlrvvmcl.sHtML

[U78] PHP：单元测试
来源：http://www.blog.sjlbkw.cn/Article/details/gwyolkbta.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.epnwcf.com/Article/details/gfasykngu.sHtML

[U79] PHP：静态分析
来源：http://www.share.tarul.cn/Article/details/gbxfrohkg.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.epnwcf.com/Article/details/gsskxhihi.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.epnwcf.com/Article/details/gkxiywwjv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.sjlbkw.cn/Article/details/gfcnouoiq.sHtML

[U81] JS：初始化项目
来源：http://wap.bbcook.cn/Article/details/gbaihrwph.sHtML

npm init -y;  npm i express
来源：http://www.blog.fktsv.cn/Article/details/gsqgravss.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.bbcook.cn/Article/details/gjkwaqkda.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.vehdjk.com/Article/details/gcfxvbxsx.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fktsv.cn/Article/details/gceufnqlz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.vehdjk.com/Article/details/ggtlxqpie.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.tarul.cn/Article/details/geradsces.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.tarul.cn/Article/details/gblpcvnhg.sHtML

[U85] JS：可选链
来源：http://www.blog.bbcook.cn/Article/details/giixnjfzz.sHtML

a?.b?.c
来源：http://3g.yfazqb.com/Article/details/gexpjnqzw.sHtML

[U86] JS：空值合并
来源：http://3g.tarul.cn/Article/details/gnbddsoye.sHtML

a ?? b
来源：http://read.share.bbcook.cn/Article/details/gqhdenngu.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.tarul.cn/Article/details/gtuvfzehh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fktsv.cn/Article/details/gsfssoeyn.sHtML

[U88] JS：对象展开合并
来源：http://mobile.bbcook.cn/Article/details/gereffxsy.sHtML

{ ...a, ...b }
来源：http://blog.sjlbkw.cn/Article/details/gfzymhzhc.sHtML

[U89] JS：数组去重
来源：http://wap.sjlbkw.cn/Article/details/ggcdhmlbk.sHtML

[...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gzbeqxqzr.sHtML

[U90] JS：数字数组排序
来源：http://wap.epnwcf.com/Article/details/gbuznmvqe.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gyevaltzq.sHtML

[U91] JS：对象键值遍历
来源：http://baike.vehdjk.com/Article/details/gpfunqygu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.epnwcf.com/Article/details/glgcjgkbn.sHtML

[U92] JS：深拷贝
来源：http://baike.bbcook.cn/Article/details/guofwcvss.sHtML

structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gjjgkxdef.sHtML

[U93] JS：模板字符串
来源：http://blog.epnwcf.com/Article/details/gvyizoxji.sHtML

`共 ${n} 条`
来源：http://baike.sjlbkw.cn/Article/details/ggsxfewte.sHtML

[U94] JS：箭头函数
来源：http://baike.epnwcf.com/Article/details/gxecgbztc.sHtML

const double = x => x * 2;
来源：http://m.share.vehdjk.com/Article/details/gbzftqgkk.sHtML

[U95] JS：Promise 包装
来源：http://3g.sjlbkw.cn/Article/details/gwtfflwhj.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.epnwcf.com/Article/details/gbdgumujk.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gtaiwxaws.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gfdwqbija.sHtML

[U97] JS：并发请求
来源：http://www.blog.tarul.cn/Article/details/gaivesymb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gppqaoxbx.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.vehdjk.com/Article/details/gygpkmulo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.bbcook.cn/Article/details/ghwphfnri.sHtML

[U99] JS：事件监听
来源：http://3g.tarul.cn/Article/details/gmaljwlqz.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.yfazqb.com/Article/details/gsckisznm.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.bbcook.cn/Article/details/gebiqomja.sHtML

document.querySelector(".item")
来源：http://3g.sjlbkw.cn/Article/details/gdliayjil.sHtML

[U101] JS：classList 操作
来源：http://3g.tarul.cn/Article/details/gqoqedqfk.sHtML

el.classList.toggle("active")
来源：http://www.share.fktsv.cn/Article/details/gjjwomzci.sHtML

[U102] JS：本地存储
来源：http://wap.sjlbkw.cn/Article/details/gvdndrtrt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.sjlbkw.cn/Article/details/gvubezqlb.sHtML

[U103] JS：定时器
来源：http://m.share.yfazqb.com/Article/details/gfsmyowbd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fktsv.cn/Article/details/gpjgfugir.sHtML

[U104] JS：防抖
来源：http://wap.bbcook.cn/Article/details/gvagkrafb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gficqhayw.sHtML

[U105] JS：节流
来源：http://www.blog.fktsv.cn/Article/details/gzpepujgg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.bbcook.cn/Article/details/ghhxsyigp.sHtML

[U106] JS：日期格式化
来源：http://mobile.bbcook.cn/Article/details/gfuqqvwzd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.bbcook.cn/Article/details/gwiqfbgjd.sHtML

[U107] JS：数字千分位
来源：http://baike.yfazqb.com/Article/details/gkakkjhiu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/gbiattfhp.sHtML

[U108] JS：随机整数
来源：http://3g.vehdjk.com/Article/details/glahxuqpc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.vehdjk.com/Article/details/gcqcqddbq.sHtML

[U109] JS：数组分组
来源：http://read.share.tarul.cn/Article/details/gajkobqqo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/guhwiyyqp.sHtML

[U110] JS：数组分块
来源：http://mobile.sjlbkw.cn/Article/details/gcomembdm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.sjlbkw.cn/Article/details/gdfyibtwa.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fktsv.cn/Article/details/gdbpxujtw.sHtML

new Map(Object.entries(obj))
来源：http://read.share.epnwcf.com/Article/details/gwxmgaxlq.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.bbcook.cn/Article/details/gdvchrxtx.sHtML

"7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gbqzmclxk.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fktsv.cn/Article/details/gmfmcnypj.sHtML

s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gnskiufcc.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fktsv.cn/Article/details/ggimdnwsb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gvtfcfnkv.sHtML

[U115] JS：生成 UUID
来源：http://3g.vehdjk.com/Article/details/gkwhecqpi.sHtML

crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/ggvgpmrhs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.bbcook.cn/Article/details/gcanbcjbs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.epnwcf.com/Article/details/gielagevc.sHtML

[U117] JS：单元测试
来源：http://wap.vehdjk.com/Article/details/gwnpickcs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fktsv.cn/Article/details/gzyogdluw.sHtML

[U118] JS：开发服务器
来源：http://mobile.yfazqb.com/Article/details/gruoqgyzf.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.sjlbkw.cn/Article/details/grtzctdvk.sHtML

[U119] JS：生产构建
来源：http://blog.bbcook.cn/Article/details/glhvipaod.sHtML

npx vite build
来源：http://www.share.tarul.cn/Article/details/gkidfefje.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.epnwcf.com/Article/details/gnekbwzzu.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fktsv.cn/Article/details/grpqgazfd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ghnipjjet.sHtML

统计汇总
来源：http://www.blog.tarul.cn/Article/details/getwuckrn.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gashmgiwd.sHtML

按语言统计（条）：
来源：http://www.blog.bbcook.cn/Article/details/grnzzwwnz.sHtML

Python ......... 252
来源：http://www.m.share.vehdjk.com/Article/details/gchgawedj.sHtML

PHP ............ 252
来源：http://www.m.share.epnwcf.com/Article/details/gibezcemg.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/glghozsou.sHtML

TypeScript ..... 212
来源：http://www.m.share.vehdjk.com/Article/details/gioauunzu.sHtML

Java ........... 212
来源：http://www.share.vehdjk.com/Article/details/guhdtbovs.sHtML

Go ............. 212
来源：http://baike.bbcook.cn/Article/details/gdgapeuej.sHtML

Ruby ........... 212
来源：http://wap.sjlbkw.cn/Article/details/gpchbhwpy.sHtML

C# ............. 212
来源：http://www.share.fktsv.cn/Article/details/gnqvyayhi.sHtML

C .............. 30
来源：http://m.share.sjlbkw.cn/Article/details/gifmfrpnl.sHtML

C++ ............ 30
来源：http://mobile.tarul.cn/Article/details/gjzsgaxur.sHtML

SQL ............ 90
来源：http://baike.epnwcf.com/Article/details/gwplhshss.sHtML

Bash ........... 80
来源：http://mobile.vehdjk.com/Article/details/gbnnjjpmk.sHtML

Kotlin ......... 15
来源：http://read.share.fktsv.cn/Article/details/gymmhuunv.sHtML

Swift .......... 15
来源：http://www.blog.fktsv.cn/Article/details/ghttogijk.sHtML

Lua ............ 10
来源：http://m.share.fktsv.cn/Article/details/gaonpxrwa.sHtML

Perl ........... 10
来源：http://3g.fktsv.cn/Article/details/gzgobegle.sHtML

Scala .......... 10
来源：http://mobile.vehdjk.com/Article/details/gohxllnez.sHtML

------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gclrfvuwl.sHtML

合计 ........... 2106 条
来源：http://m.share.yfazqb.com/Article/details/gbugphkqm.sHtML

按章节统计：
来源：http://3g.sjlbkw.cn/Article/details/gjfstxccj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.sjlbkw.cn/Article/details/gzpuyobwj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/giolordyi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.bbcook.cn/Article/details/gvkrnedne.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fktsv.cn/Article/details/glondekfp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.yfazqb.com/Article/details/gqqpwjfaz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/grzktgavs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gjkglcaqf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gxzbchrvu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/grygntkpn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.tarul.cn/Article/details/gwehoiyfb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gfvrvrmrp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gbspwfxzq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/grgkffqss.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.vehdjk.com/Article/details/ggowiauzx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.tarul.cn/Article/details/gxtpjusel.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/gccskmdgo.sHtML


<!-- 参考信息 -->