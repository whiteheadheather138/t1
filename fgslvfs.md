代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://blog.tarul.cn/Article/details/ghspghnhg.sHtML

[T51] Scala：Hello World
来源：http://3g.fktsv.cn/Article/details/geuljgvzd.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gnzhorzzw.sHtML

[T52] Scala：变量
来源：http://wap.vehdjk.com/Article/details/gwufdpxqv.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gtlfsfucy.sHtML

[T53] Scala：字符串插值
来源：http://3g.fktsv.cn/Article/details/gvpzwonwt.sHtML

s"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gkexgaygq.sHtML

[T54] Scala：集合映射
来源：http://3g.fktsv.cn/Article/details/gyfosaess.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.yfazqb.com/Article/details/gtiinaaae.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fktsv.cn/Article/details/gqzchtrpt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.epnwcf.com/Article/details/ghzprywne.sHtML

[T56] Scala：样例类
来源：http://blog.bbcook.cn/Article/details/gejublnpk.sHtML

case class User(name: String, age: Int)
来源：http://3g.tarul.cn/Article/details/gprwblniu.sHtML

[T57] Scala：模式匹配
来源：http://3g.fktsv.cn/Article/details/gwotacfch.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.epnwcf.com/Article/details/griuysaze.sHtML

[T58] Scala：函数定义
来源：http://m.share.bbcook.cn/Article/details/gpboevico.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.vehdjk.com/Article/details/ggpcrseoa.sHtML

[T59] Scala：循环
来源：http://www.blog.epnwcf.com/Article/details/ggzcnfvre.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gpncpmeyf.sHtML

[T60] Scala：折叠
来源：http://m.share.tarul.cn/Article/details/ghcggbije.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fktsv.cn/Article/details/gvcwtuzrh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/geldaosje.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.yfazqb.com/Article/details/gtpfhbnmw.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdxjjoyhx.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.tarul.cn/Article/details/gsqtxjsha.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.vehdjk.com/Article/details/grelrzzfq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.sjlbkw.cn/Article/details/gjjtenwlz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.tarul.cn/Article/details/gdycnhjca.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.sjlbkw.cn/Article/details/greunthap.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.bbcook.cn/Article/details/gszfdvfnd.sHtML

[U04] Py：变量调试打印
来源：http://m.share.vehdjk.com/Article/details/gdwelxktn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.yfazqb.com/Article/details/ghtodrqpz.sHtML

[U05] Py：列表去重且保序
来源：http://baike.tarul.cn/Article/details/gipxymaks.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gutlvvvgu.sHtML

[U06] Py：合并两个字典
来源：http://m.share.tarul.cn/Article/details/gahgjtdbj.sHtML

{**a, **b}
来源：http://www.blog.tarul.cn/Article/details/gmrbkejbz.sHtML

[U07] Py：反转字典键值
来源：http://blog.vehdjk.com/Article/details/gamhyzzik.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fktsv.cn/Article/details/geoydvpjl.sHtML

[U08] Py：展平二维列表
来源：http://www.share.yfazqb.com/Article/details/gmnztvyaa.sHtML

[y for x in nested for y in x]
来源：http://m.share.epnwcf.com/Article/details/grbztvuse.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fktsv.cn/Article/details/gmlhnvhfe.sHtML

max(d, key=d.get)
来源：http://mobile.fktsv.cn/Article/details/golkgukoq.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.yfazqb.com/Article/details/gfkiserxz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.bbcook.cn/Article/details/gczeplbau.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fktsv.cn/Article/details/gvtphxmpz.sHtML

(x * 2 for x in arr)
来源：http://wap.vehdjk.com/Article/details/gmdjryjix.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.bbcook.cn/Article/details/gwmyjrwhv.sHtML

Counter(arr).most_common(3)
来源：http://m.share.vehdjk.com/Article/details/gbzpguaah.sHtML

[U13] Py：固定长度队列
来源：http://www.share.epnwcf.com/Article/details/gpbaiddga.sHtML

deque(maxlen=10)
来源：http://m.share.tarul.cn/Article/details/gorepwdid.sHtML

[U14] Py：分组收集到列表
来源：http://blog.sjlbkw.cn/Article/details/ghnrrzult.sHtML

defaultdict(list)
来源：http://blog.yfazqb.com/Article/details/ghhrwxkdx.sHtML

[U15] Py：高精度计时
来源：http://blog.tarul.cn/Article/details/gnuodeibr.sHtML

t = time.perf_counter()
来源：http://www.blog.fktsv.cn/Article/details/gpwdkzlea.sHtML

[U16] Py：命令行参数解析
来源：http://wap.sjlbkw.cn/Article/details/gspnzzocc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.bbcook.cn/Article/details/gxoccgmbg.sHtML

[U17] Py：初始化日志
来源：http://blog.epnwcf.com/Article/details/gvzfpgpsa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.yfazqb.com/Article/details/ggmffmjbi.sHtML

[U18] Py：预编译正则
来源：http://mobile.vehdjk.com/Article/details/geipogmin.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.tarul.cn/Article/details/glqwpwnfr.sHtML

[U19] Py：正则替换带回调
来源：http://3g.bbcook.cn/Article/details/gwfsaxdex.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fktsv.cn/Article/details/gkvrgyndu.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.tarul.cn/Article/details/gkyclmmkw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.epnwcf.com/Article/details/gcduklvhc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.vehdjk.com/Article/details/gqnrvordj.sHtML

@contextlib.contextmanager
来源：http://read.share.bbcook.cn/Article/details/gnzxcxigi.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.epnwcf.com/Article/details/gwpdxsnzm.sHtML

list(zip(*m))
来源：http://3g.fktsv.cn/Article/details/guqxozqau.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fktsv.cn/Article/details/ghrxwsaie.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.tarul.cn/Article/details/gisrhntmk.sHtML

[U24] Py：路径操作
来源：http://www.m.share.epnwcf.com/Article/details/gyvefsphw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.sjlbkw.cn/Article/details/gaccfefia.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.sjlbkw.cn/Article/details/ghghmqebl.sHtML

csv.DictReader(f)
来源：http://mobile.fktsv.cn/Article/details/gmlngbodc.sHtML

[U26] Py：并发下载
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcddokzu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.yfazqb.com/Article/details/gxmguvary.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.yfazqb.com/Article/details/gkbbbaldu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.yfazqb.com/Article/details/gccmxkcxu.sHtML

[U28] Py：类型别名
来源：http://blog.bbcook.cn/Article/details/gbdeonxcn.sHtML

UserId = int
来源：http://read.share.tarul.cn/Article/details/gnhtkkrdq.sHtML

[U29] Py：属性校验
来源：http://www.m.share.yfazqb.com/Article/details/guzsqfqla.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fktsv.cn/Article/details/glsqnqtco.sHtML

[U30] Py：数据类
来源：http://wap.epnwcf.com/Article/details/gxqdrbrrl.sHtML

@dataclass(slots=True)
来源：http://3g.yfazqb.com/Article/details/gonmqtlue.sHtML

[U31] Py：单测
来源：http://www.share.yfazqb.com/Article/details/gkxeziqfe.sHtML

python -m pytest -q
来源：http://wap.vehdjk.com/Article/details/gfiouydpz.sHtML

[U32] Py：代码格式化
来源：http://blog.tarul.cn/Article/details/gmffpcmnp.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.sjlbkw.cn/Article/details/gzqcscada.sHtML

[U33] Py：打包发布
来源：http://www.share.bbcook.cn/Article/details/gfvkifgix.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.yfazqb.com/Article/details/gfadgxobw.sHtML

[U34] Py：判断编码
来源：http://wap.vehdjk.com/Article/details/gnxmepsqu.sHtML

chardet.detect(raw)
来源：http://read.share.yfazqb.com/Article/details/gwnlxkqwm.sHtML

[U35] Py：发送邮件
来源：http://m.share.vehdjk.com/Article/details/gjymaqimj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fktsv.cn/Article/details/gbobrckne.sHtML

[U36] Py：定时任务
来源：http://baike.sjlbkw.cn/Article/details/gpwnhuyie.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.yfazqb.com/Article/details/grfsoyvqr.sHtML

[U37] Py：读写 Excel
来源：http://read.share.bbcook.cn/Article/details/gjrfxpuqu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.yfazqb.com/Article/details/guejwmdnx.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.epnwcf.com/Article/details/gaatildqd.sHtML

Path(__file__).resolve().parent
来源：http://mobile.sjlbkw.cn/Article/details/gknhihtgc.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.bbcook.cn/Article/details/gjrjafkce.sHtML

sys.stdout.isatty()
来源：http://3g.yfazqb.com/Article/details/gpdbevfio.sHtML

[U40] Py：打印到标准错误
来源：http://blog.vehdjk.com/Article/details/gpffpucle.sHtML

print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/grrbawuyy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.tarul.cn/Article/details/gvbhejmyk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.bbcook.cn/Article/details/gnxhsegnr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.tarul.cn/Article/details/gfnylzjqm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fktsv.cn/Article/details/gbincstlr.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gtmwcozxh.sHtML

namespace App\Http;
来源：http://mobile.bbcook.cn/Article/details/gsiwhbsfx.sHtML

[U44] PHP：开启严格类型
来源：http://wap.tarul.cn/Article/details/gukfjbltz.sHtML

declare(strict_types=1);
来源：http://wap.epnwcf.com/Article/details/gxgciikiq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.tarul.cn/Article/details/gdmutvdya.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gsoxvzhep.sHtML

[U46] PHP：可空类型
来源：http://baike.vehdjk.com/Article/details/gqgbdklgg.sHtML

?string $name = null
来源：http://3g.tarul.cn/Article/details/gqgxxqkhm.sHtML

[U47] PHP：联合类型
来源：http://www.share.epnwcf.com/Article/details/gehirdhce.sHtML

int|string $id
来源：http://m.share.epnwcf.com/Article/details/gtwiprihn.sHtML

[U48] PHP：纯枚举
来源：http://wap.epnwcf.com/Article/details/gddxdcsci.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fktsv.cn/Article/details/gqagxqpho.sHtML

[U49] PHP：只读属性
来源：http://www.share.fktsv.cn/Article/details/gnhppunwo.sHtML

public readonly string $name
来源：http://www.share.fktsv.cn/Article/details/gbeaftlip.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.tarul.cn/Article/details/gjgxdwynk.sHtML

public function __construct(private int $id) {}
来源：http://wap.tarul.cn/Article/details/glxqsdqns.sHtML

[U51] PHP：数组解构
来源：http://mobile.fktsv.cn/Article/details/gzhsxscgl.sHtML

[$a, $b] = $arr;
来源：http://www.share.fktsv.cn/Article/details/gqpycgxmp.sHtML

[U52] PHP：箭头函数
来源：http://www.share.yfazqb.com/Article/details/groullizz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.vehdjk.com/Article/details/gtippywvw.sHtML

[U53] PHP：空合并运算符
来源：http://3g.yfazqb.com/Article/details/giggwgnzg.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.yfazqb.com/Article/details/gpuasldcv.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fktsv.cn/Article/details/glyrcwhzv.sHtML

$obj?->method()
来源：http://read.share.sjlbkw.cn/Article/details/gceedpltk.sHtML

[U55] PHP：match 表达式
来源：http://wap.sjlbkw.cn/Article/details/ggojxzfwz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.sjlbkw.cn/Article/details/gmtbulbot.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlgmeder.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gbbdjytoj.sHtML

[U57] PHP：字符串插值
来源：http://blog.epnwcf.com/Article/details/gjlfwazno.sHtML

"值: {$a}"
来源：http://blog.yfazqb.com/Article/details/gurcksrvl.sHtML

[U58] PHP：数组三件套
来源：http://baike.bbcook.cn/Article/details/gzuebdbvs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.tarul.cn/Article/details/gbbfwyixb.sHtML

[U59] PHP：自定义排序
来源：http://mobile.tarul.cn/Article/details/ghkpezerv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/gcfqycchw.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.epnwcf.com/Article/details/gezoksstp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fktsv.cn/Article/details/goykwnhzx.sHtML

[U61] PHP：正则
来源：http://www.blog.fktsv.cn/Article/details/gfbxztpll.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.vehdjk.com/Article/details/gheqjrtvd.sHtML

[U62] PHP：日期对象
来源：http://baike.yfazqb.com/Article/details/gvtwqbmap.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.tarul.cn/Article/details/gznblsgdp.sHtML

[U63] PHP：文件读写
来源：http://www.blog.epnwcf.com/Article/details/gjptrbdqg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.epnwcf.com/Article/details/gomxmcvsk.sHtML

[U64] PHP：目录遍历
来源：http://read.share.sjlbkw.cn/Article/details/gimkbvnyd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.yfazqb.com/Article/details/grmegzlvq.sHtML

[U65] PHP：会话
来源：http://blog.tarul.cn/Article/details/gnjffzdjf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gxhmkgxoy.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.bbcook.cn/Article/details/gfblzyejf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.vehdjk.com/Article/details/gpytpoodt.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.bbcook.cn/Article/details/gswixcszh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.tarul.cn/Article/details/glrbmnyda.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.vehdjk.com/Article/details/gpzjkwicy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.epnwcf.com/Article/details/grkhiqnbm.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.tarul.cn/Article/details/gcwtfjtwe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fktsv.cn/Article/details/ggzpybmqb.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.sjlbkw.cn/Article/details/gxxmgeohw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.sjlbkw.cn/Article/details/gkyelryll.sHtML

[U71] PHP：抛出异常
来源：http://read.share.epnwcf.com/Article/details/gkimdgygn.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.vehdjk.com/Article/details/gjglohvdi.sHtML

[U72] PHP：写错误日志
来源：http://3g.yfazqb.com/Article/details/ghxvfzomp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.yfazqb.com/Article/details/gpukenqbl.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.yfazqb.com/Article/details/gmrpmxhpg.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.bbcook.cn/Article/details/gkwewxrbu.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fktsv.cn/Article/details/gqxhldzlp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.sjlbkw.cn/Article/details/gqzgvdopi.sHtML

[U75] PHP：依赖注入
来源：http://m.share.tarul.cn/Article/details/glrjqaizh.sHtML

composer require psr/container
来源：http://baike.sjlbkw.cn/Article/details/guawfujmf.sHtML

[U76] PHP：简单路由
来源：http://3g.vehdjk.com/Article/details/gdqerzofv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.sjlbkw.cn/Article/details/gnafpdnjo.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.tarul.cn/Article/details/ghfnnczvk.sHtML

composer require twig/twig
来源：http://read.share.yfazqb.com/Article/details/gucxbotfa.sHtML

[U78] PHP：单元测试
来源：http://wap.fktsv.cn/Article/details/gbwhaaodi.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.epnwcf.com/Article/details/gfcprioff.sHtML

[U79] PHP：静态分析
来源：http://3g.sjlbkw.cn/Article/details/gpfvaruvl.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.bbcook.cn/Article/details/gccewpkbu.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fktsv.cn/Article/details/gyetepxhm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.bbcook.cn/Article/details/gkquyidxi.sHtML

[U81] JS：初始化项目
来源：http://m.share.sjlbkw.cn/Article/details/gnxbmmvhm.sHtML

npm init -y;  npm i express
来源：http://3g.sjlbkw.cn/Article/details/glcdejbez.sHtML

[U82] JS：package.json 脚本
来源：http://blog.sjlbkw.cn/Article/details/gikgtgssv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.bbcook.cn/Article/details/geqqgictz.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.yfazqb.com/Article/details/gefxmzjhc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.tarul.cn/Article/details/gschdbwna.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.tarul.cn/Article/details/godoppmik.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.sjlbkw.cn/Article/details/gtlagzzxk.sHtML

[U85] JS：可选链
来源：http://blog.bbcook.cn/Article/details/gvgrirzhu.sHtML

a?.b?.c
来源：http://read.share.bbcook.cn/Article/details/gbrzzdcao.sHtML

[U86] JS：空值合并
来源：http://mobile.fktsv.cn/Article/details/gfgpvtbal.sHtML

a ?? b
来源：http://www.blog.yfazqb.com/Article/details/gnlghednf.sHtML

[U87] JS：解构默认值
来源：http://m.share.epnwcf.com/Article/details/gcysnjxdk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.yfazqb.com/Article/details/gbyfnzlel.sHtML

[U88] JS：对象展开合并
来源：http://3g.epnwcf.com/Article/details/gdhdqcnzb.sHtML

{ ...a, ...b }
来源：http://wap.tarul.cn/Article/details/gttqaslbx.sHtML

[U89] JS：数组去重
来源：http://www.share.tarul.cn/Article/details/gyinweqrh.sHtML

[...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gvgqaeltm.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.sjlbkw.cn/Article/details/gzuwozmwg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gmisxtzve.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fktsv.cn/Article/details/ggwwnttkh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.vehdjk.com/Article/details/gteinunqf.sHtML

[U92] JS：深拷贝
来源：http://blog.vehdjk.com/Article/details/gjtjbdygk.sHtML

structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gjbzhayal.sHtML

[U93] JS：模板字符串
来源：http://www.share.epnwcf.com/Article/details/gijumlhbr.sHtML

`共 ${n} 条`
来源：http://3g.sjlbkw.cn/Article/details/gljpfgtuc.sHtML

[U94] JS：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/gwwvstnrw.sHtML

const double = x => x * 2;
来源：http://www.share.bbcook.cn/Article/details/grmowishs.sHtML

[U95] JS：Promise 包装
来源：http://baike.bbcook.cn/Article/details/gvdixzgfn.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.bbcook.cn/Article/details/gbtzzwpsz.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fktsv.cn/Article/details/gyvrfwbqq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gqbvryfgq.sHtML

[U97] JS：并发请求
来源：http://www.share.sjlbkw.cn/Article/details/gjoneingz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gcocpnmal.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.bbcook.cn/Article/details/gemilstda.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.yfazqb.com/Article/details/gcofvznyo.sHtML

[U99] JS：事件监听
来源：http://www.m.share.tarul.cn/Article/details/gltklxlvb.sHtML

el.addEventListener("click", e => {})
来源：http://baike.tarul.cn/Article/details/gvethrljt.sHtML

[U100] JS：DOM 查询
来源：http://m.share.vehdjk.com/Article/details/gbrrhdiey.sHtML

document.querySelector(".item")
来源：http://mobile.vehdjk.com/Article/details/gxwbvyocf.sHtML

[U101] JS：classList 操作
来源：http://3g.epnwcf.com/Article/details/gyxnvyqja.sHtML

el.classList.toggle("active")
来源：http://baike.yfazqb.com/Article/details/gknxizaih.sHtML

[U102] JS：本地存储
来源：http://www.share.sjlbkw.cn/Article/details/gtkkxkwql.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.epnwcf.com/Article/details/gkelcwyqo.sHtML

[U103] JS：定时器
来源：http://blog.tarul.cn/Article/details/gcygnyqvu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.yfazqb.com/Article/details/gcsjaaldw.sHtML

[U104] JS：防抖
来源：http://www.share.yfazqb.com/Article/details/gigmdwgqa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/geuknnowz.sHtML

[U105] JS：节流
来源：http://www.blog.yfazqb.com/Article/details/gvpmfsnon.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.tarul.cn/Article/details/gtdzxrwip.sHtML

[U106] JS：日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gziclrnqy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.bbcook.cn/Article/details/gjmurotcz.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/gylfkfkft.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/gmkwfmjil.sHtML

[U108] JS：随机整数
来源：http://baike.tarul.cn/Article/details/gnlnoxfcf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.yfazqb.com/Article/details/gtkxlxqep.sHtML

[U109] JS：数组分组
来源：http://baike.yfazqb.com/Article/details/gobioenqn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.vehdjk.com/Article/details/gwazpnqyl.sHtML

[U110] JS：数组分块
来源：http://www.blog.vehdjk.com/Article/details/gkivzpydj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fktsv.cn/Article/details/gmxycpyic.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/geohtdszt.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzhwtkit.sHtML

[U112] JS：字符串补位
来源：http://www.share.sjlbkw.cn/Article/details/gppclwyxr.sHtML

"7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gxehgnvpd.sHtML

[U113] JS：正则替换全部
来源：http://blog.epnwcf.com/Article/details/gubvktewg.sHtML

s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gqgwiarza.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.yfazqb.com/Article/details/gwnemollu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.vehdjk.com/Article/details/gpxldjbyp.sHtML

[U115] JS：生成 UUID
来源：http://read.share.vehdjk.com/Article/details/gmugbmenf.sHtML

crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gmixlskyq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fktsv.cn/Article/details/gupasomvv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.vehdjk.com/Article/details/gwqjymokc.sHtML

[U117] JS：单元测试
来源：http://3g.sjlbkw.cn/Article/details/gwvmvdedy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.epnwcf.com/Article/details/glafyetll.sHtML

[U118] JS：开发服务器
来源：http://www.share.tarul.cn/Article/details/gkesvulws.sHtML

npm i -D vite;  npx vite
来源：http://3g.fktsv.cn/Article/details/gkbqxwcrk.sHtML

[U119] JS：生产构建
来源：http://m.share.fktsv.cn/Article/details/ggvtajfwn.sHtML

npx vite build
来源：http://read.share.epnwcf.com/Article/details/gnihdsmfd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fktsv.cn/Article/details/gtivfadzn.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fktsv.cn/Article/details/gvtwpfoeq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmucksyim.sHtML

统计汇总
来源：http://wap.epnwcf.com/Article/details/gxmbjfdnl.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvplpiyer.sHtML

按语言统计（条）：
来源：http://wap.fktsv.cn/Article/details/geordvjfx.sHtML

Python ......... 252
来源：http://www.blog.sjlbkw.cn/Article/details/gtaetvofr.sHtML

PHP ............ 252
来源：http://www.blog.tarul.cn/Article/details/goecuuneq.sHtML

JavaScript ..... 252
来源：http://www.m.share.sjlbkw.cn/Article/details/gdiaphlhk.sHtML

TypeScript ..... 212
来源：http://blog.epnwcf.com/Article/details/gdaksuplx.sHtML

Java ........... 212
来源：http://blog.bbcook.cn/Article/details/grxhyenqb.sHtML

Go ............. 212
来源：http://m.share.tarul.cn/Article/details/gqndejrrh.sHtML

Ruby ........... 212
来源：http://read.share.tarul.cn/Article/details/gzjcdpvgx.sHtML

C# ............. 212
来源：http://m.share.epnwcf.com/Article/details/gswstfnzq.sHtML

C .............. 30
来源：http://www.share.sjlbkw.cn/Article/details/grvggtawv.sHtML

C++ ............ 30
来源：http://baike.vehdjk.com/Article/details/ghcnmzvzg.sHtML

SQL ............ 90
来源：http://www.blog.epnwcf.com/Article/details/gdpjqihxk.sHtML

Bash ........... 80
来源：http://wap.vehdjk.com/Article/details/gibqbuxhk.sHtML

Kotlin ......... 15
来源：http://www.m.share.fktsv.cn/Article/details/ghlamjacd.sHtML

Swift .......... 15
来源：http://www.blog.epnwcf.com/Article/details/glyqwcwcz.sHtML

Lua ............ 10
来源：http://www.blog.yfazqb.com/Article/details/gvuxngtrq.sHtML

Perl ........... 10
来源：http://www.m.share.bbcook.cn/Article/details/gjxfrnujt.sHtML

Scala .......... 10
来源：http://baike.tarul.cn/Article/details/gslpbqatj.sHtML

------------------------------------
来源：http://blog.bbcook.cn/Article/details/gsegjzotk.sHtML

合计 ........... 2106 条
来源：http://read.share.tarul.cn/Article/details/gtenplfqc.sHtML

按章节统计：
来源：http://www.blog.fktsv.cn/Article/details/gxdngcktx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fktsv.cn/Article/details/gxcnjsprt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gojvkjypt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gktdaatgi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gcbvbmbku.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fktsv.cn/Article/details/goenxxnqe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fktsv.cn/Article/details/gtaycxvpv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gkkhzhrdh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.tarul.cn/Article/details/gqmqcyswm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gpeccsjlq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/gfuxlvtsx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/glsrksook.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gmlvqeqkp.sHtML


<!-- 参考信息 -->