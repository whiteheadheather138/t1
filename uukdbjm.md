代发 wailian999

val a = 1;  var b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gvltnrevq.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gzsnjwfyr.sHtML

s"值: $b"
来源：http://3g.yfazqb.com/Article/details/gwiljguzg.sHtML

[T54] Scala：集合映射
来源：http://www.blog.yfazqb.com/Article/details/glfikmajl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.sjlbkw.cn/Article/details/gwbdmlfyl.sHtML

[T55] Scala：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/ghjefamly.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.epnwcf.com/Article/details/giuwzovvt.sHtML

[T56] Scala：样例类
来源：http://wap.tarul.cn/Article/details/getdyukpv.sHtML

case class User(name: String, age: Int)
来源：http://mobile.vehdjk.com/Article/details/gzdmoultu.sHtML

[T57] Scala：模式匹配
来源：http://m.share.epnwcf.com/Article/details/gvchxwluf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.vehdjk.com/Article/details/gwlenqdns.sHtML

[T58] Scala：函数定义
来源：http://blog.epnwcf.com/Article/details/gjzjvkbqx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fktsv.cn/Article/details/gayqaohsn.sHtML

[T59] Scala：循环
来源：http://www.blog.sjlbkw.cn/Article/details/ggxsrtcha.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gcncnoytg.sHtML

[T60] Scala：折叠
来源：http://wap.bbcook.cn/Article/details/gctgurewz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.yfazqb.com/Article/details/gulmhgsxt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcloiftbv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.yfazqb.com/Article/details/gswqlnopx.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqgeblvan.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.sjlbkw.cn/Article/details/gylfmbthc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.bbcook.cn/Article/details/gguwfqyzb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.vehdjk.com/Article/details/gfvteoxqi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.epnwcf.com/Article/details/ghpnbmrwz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.tarul.cn/Article/details/ghqeoffdu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fktsv.cn/Article/details/gpwtygupr.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fktsv.cn/Article/details/goxjgmxbc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.bbcook.cn/Article/details/gyybwcztg.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.sjlbkw.cn/Article/details/gnrwjybqw.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gbbxagflt.sHtML

[U06] Py：合并两个字典
来源：http://blog.bbcook.cn/Article/details/gubpwozmu.sHtML

{**a, **b}
来源：http://www.m.share.bbcook.cn/Article/details/gsikgunlz.sHtML

[U07] Py：反转字典键值
来源：http://m.share.sjlbkw.cn/Article/details/glryoelom.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fktsv.cn/Article/details/gnowatanm.sHtML

[U08] Py：展平二维列表
来源：http://www.share.tarul.cn/Article/details/gerilorli.sHtML

[y for x in nested for y in x]
来源：http://wap.sjlbkw.cn/Article/details/gjurbboju.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.tarul.cn/Article/details/gsjllzvmd.sHtML

max(d, key=d.get)
来源：http://3g.bbcook.cn/Article/details/gbaydoxis.sHtML

[U10] Py：按值排序字典
来源：http://wap.sjlbkw.cn/Article/details/gwpojfgbn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.yfazqb.com/Article/details/gfaiijtzh.sHtML

[U11] Py：生成器表达式
来源：http://blog.sjlbkw.cn/Article/details/ghjuedkmw.sHtML

(x * 2 for x in arr)
来源：http://wap.yfazqb.com/Article/details/gaemtunll.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fktsv.cn/Article/details/ghxgjqubs.sHtML

Counter(arr).most_common(3)
来源：http://m.share.sjlbkw.cn/Article/details/gvbpcqtmy.sHtML

[U13] Py：固定长度队列
来源：http://3g.epnwcf.com/Article/details/gfquxduti.sHtML

deque(maxlen=10)
来源：http://read.share.sjlbkw.cn/Article/details/gexkpxzmb.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.sjlbkw.cn/Article/details/gjugxeksj.sHtML

defaultdict(list)
来源：http://baike.bbcook.cn/Article/details/grpojaqzq.sHtML

[U15] Py：高精度计时
来源：http://3g.bbcook.cn/Article/details/ghtoxecas.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/ghagvciyl.sHtML

[U16] Py：命令行参数解析
来源：http://blog.yfazqb.com/Article/details/gyltulifi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.yfazqb.com/Article/details/gjefvtmxs.sHtML

[U17] Py：初始化日志
来源：http://www.blog.epnwcf.com/Article/details/gpymcvvwu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.yfazqb.com/Article/details/gofjnxfgi.sHtML

[U18] Py：预编译正则
来源：http://blog.epnwcf.com/Article/details/gdxaplrjb.sHtML

pat = re.compile(r"\d+")
来源：http://baike.epnwcf.com/Article/details/glpxzeyxi.sHtML

[U19] Py：正则替换带回调
来源：http://baike.tarul.cn/Article/details/gkobbbfle.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fktsv.cn/Article/details/gzgjjmpwt.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.tarul.cn/Article/details/gtriwainx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.sjlbkw.cn/Article/details/gltmublvf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.yfazqb.com/Article/details/gnmqkybfs.sHtML

@contextlib.contextmanager
来源：http://m.share.fktsv.cn/Article/details/gifzgubuh.sHtML

[U22] Py：矩阵转置
来源：http://read.share.epnwcf.com/Article/details/guouezppj.sHtML

list(zip(*m))
来源：http://3g.sjlbkw.cn/Article/details/grgvtngjl.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.vehdjk.com/Article/details/gdfvothax.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fktsv.cn/Article/details/gqlafklkz.sHtML

[U24] Py：路径操作
来源：http://3g.sjlbkw.cn/Article/details/gcswxsdqb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.vehdjk.com/Article/details/gsspwefzh.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.yfazqb.com/Article/details/glxepkodb.sHtML

csv.DictReader(f)
来源：http://www.m.share.vehdjk.com/Article/details/gpbtizgcr.sHtML

[U26] Py：并发下载
来源：http://www.share.epnwcf.com/Article/details/gtiwvbnng.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.bbcook.cn/Article/details/gzpnnrudb.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fktsv.cn/Article/details/gjcepvruz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.vehdjk.com/Article/details/gjmfmcwll.sHtML

[U28] Py：类型别名
来源：http://blog.bbcook.cn/Article/details/ggkokjiya.sHtML

UserId = int
来源：http://www.blog.fktsv.cn/Article/details/gtlwfiijm.sHtML

[U29] Py：属性校验
来源：http://baike.tarul.cn/Article/details/gffysnwpv.sHtML

@property 与 @x.setter 配合
来源：http://m.share.vehdjk.com/Article/details/gmvrbuyzp.sHtML

[U30] Py：数据类
来源：http://blog.tarul.cn/Article/details/gufjxafsx.sHtML

@dataclass(slots=True)
来源：http://baike.vehdjk.com/Article/details/gfnipqgdj.sHtML

[U31] Py：单测
来源：http://baike.sjlbkw.cn/Article/details/gtqjhlovh.sHtML

python -m pytest -q
来源：http://read.share.vehdjk.com/Article/details/gpvttqitu.sHtML

[U32] Py：代码格式化
来源：http://read.share.yfazqb.com/Article/details/gevodbjjh.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.tarul.cn/Article/details/geiyhzjpc.sHtML

[U33] Py：打包发布
来源：http://3g.vehdjk.com/Article/details/gskodqodi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.bbcook.cn/Article/details/gcsncnfbd.sHtML

[U34] Py：判断编码
来源：http://3g.sjlbkw.cn/Article/details/gbjgbdkmk.sHtML

chardet.detect(raw)
来源：http://mobile.fktsv.cn/Article/details/ggmwvaujc.sHtML

[U35] Py：发送邮件
来源：http://read.share.fktsv.cn/Article/details/gcpdjtyez.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.tarul.cn/Article/details/gfncrekkz.sHtML

[U36] Py：定时任务
来源：http://baike.bbcook.cn/Article/details/ghbdqaxuf.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fktsv.cn/Article/details/gobnevsrr.sHtML

[U37] Py：读写 Excel
来源：http://www.share.vehdjk.com/Article/details/ghqzbczfc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.vehdjk.com/Article/details/gjzogeemx.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.epnwcf.com/Article/details/gritlczox.sHtML

Path(__file__).resolve().parent
来源：http://3g.sjlbkw.cn/Article/details/goslditms.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.yfazqb.com/Article/details/gyvppomav.sHtML

sys.stdout.isatty()
来源：http://baike.fktsv.cn/Article/details/gzawasugr.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.vehdjk.com/Article/details/gimvcnlog.sHtML

print("err", file=sys.stderr)
来源：http://m.share.sjlbkw.cn/Article/details/goffeglit.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fktsv.cn/Article/details/gdwnkzvco.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.bbcook.cn/Article/details/gjznrcanp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.epnwcf.com/Article/details/gznpheaun.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fktsv.cn/Article/details/glvsxuahd.sHtML

[U43] PHP：声明命名空间
来源：http://blog.vehdjk.com/Article/details/gcabwfshl.sHtML

namespace App\Http;
来源：http://www.m.share.fktsv.cn/Article/details/gqrewymnr.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.tarul.cn/Article/details/gupuzompx.sHtML

declare(strict_types=1);
来源：http://read.share.epnwcf.com/Article/details/gxyzgvisn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.vehdjk.com/Article/details/ggvvtupnz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyeqqcvev.sHtML

[U46] PHP：可空类型
来源：http://wap.fktsv.cn/Article/details/gvbedreqx.sHtML

?string $name = null
来源：http://m.share.epnwcf.com/Article/details/gnmzuwkxb.sHtML

[U47] PHP：联合类型
来源：http://m.share.vehdjk.com/Article/details/gslugekbc.sHtML

int|string $id
来源：http://www.blog.tarul.cn/Article/details/gdtjgqlaq.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fktsv.cn/Article/details/ghyizufhd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.epnwcf.com/Article/details/gdxymzdam.sHtML

[U49] PHP：只读属性
来源：http://www.share.bbcook.cn/Article/details/gschydhht.sHtML

public readonly string $name
来源：http://m.share.epnwcf.com/Article/details/grtumyutp.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.bbcook.cn/Article/details/gccralrru.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fktsv.cn/Article/details/gvkcvdllk.sHtML

[U51] PHP：数组解构
来源：http://m.share.yfazqb.com/Article/details/gjaosthrt.sHtML

[$a, $b] = $arr;
来源：http://mobile.vehdjk.com/Article/details/gsmuhzrda.sHtML

[U52] PHP：箭头函数
来源：http://mobile.vehdjk.com/Article/details/govdguica.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.epnwcf.com/Article/details/gcoswnpjy.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fktsv.cn/Article/details/glmkvovei.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.epnwcf.com/Article/details/gyuikysel.sHtML

[U54] PHP：空安全调用
来源：http://www.share.bbcook.cn/Article/details/giuugyuph.sHtML

$obj?->method()
来源：http://blog.tarul.cn/Article/details/gopjgseps.sHtML

[U55] PHP：match 表达式
来源：http://read.share.bbcook.cn/Article/details/gsjfhotna.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.bbcook.cn/Article/details/gryfzlngc.sHtML

[U56] PHP：命名参数
来源：http://read.share.fktsv.cn/Article/details/gfmruoslx.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gbrjdsjgm.sHtML

[U57] PHP：字符串插值
来源：http://blog.yfazqb.com/Article/details/gqunbjzzr.sHtML

"值: {$a}"
来源：http://mobile.vehdjk.com/Article/details/gyieraidb.sHtML

[U58] PHP：数组三件套
来源：http://read.share.sjlbkw.cn/Article/details/gdhxakdju.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.bbcook.cn/Article/details/gdczdprdw.sHtML

[U59] PHP：自定义排序
来源：http://m.share.yfazqb.com/Article/details/ggwvnsswn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/gsnabcrmg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.yfazqb.com/Article/details/ghuxsnvrs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fktsv.cn/Article/details/gqimodlju.sHtML

[U61] PHP：正则
来源：http://wap.tarul.cn/Article/details/gbpzychbc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/gjwcfdlbl.sHtML

[U62] PHP：日期对象
来源：http://wap.yfazqb.com/Article/details/gggbhamho.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.bbcook.cn/Article/details/gdjgaozov.sHtML

[U63] PHP：文件读写
来源：http://read.share.vehdjk.com/Article/details/gsrwbdjah.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.epnwcf.com/Article/details/gucimkwjw.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fktsv.cn/Article/details/gxpgasbzl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.yfazqb.com/Article/details/gpgoubyfy.sHtML

[U65] PHP：会话
来源：http://baike.yfazqb.com/Article/details/gkcudxlpm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.vehdjk.com/Article/details/givpwcpnz.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.sjlbkw.cn/Article/details/gwvsjoiuh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.epnwcf.com/Article/details/gmydgiijf.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.yfazqb.com/Article/details/gcpdasamd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.bbcook.cn/Article/details/geumrmwqe.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.sjlbkw.cn/Article/details/gxzjcikrj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.vehdjk.com/Article/details/giswotzle.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.sjlbkw.cn/Article/details/gacfcsrwq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.tarul.cn/Article/details/gikuzfvde.sHtML

[U70] PHP：PDO 事务
来源：http://wap.bbcook.cn/Article/details/gytqyurle.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.yfazqb.com/Article/details/gztuyjbxf.sHtML

[U71] PHP：抛出异常
来源：http://read.share.vehdjk.com/Article/details/gvbpvhrxt.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.bbcook.cn/Article/details/galxyxzth.sHtML

[U72] PHP：写错误日志
来源：http://baike.tarul.cn/Article/details/gdblutogx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.epnwcf.com/Article/details/gutqrxowt.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.tarul.cn/Article/details/gkuebmhzo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fktsv.cn/Article/details/gsuovjjup.sHtML

[U74] PHP：读取环境变量
来源：http://blog.tarul.cn/Article/details/gjhaorymh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.tarul.cn/Article/details/gmepyshfo.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fktsv.cn/Article/details/gabkvuism.sHtML

composer require psr/container
来源：http://3g.yfazqb.com/Article/details/gdfsbzuxe.sHtML

[U76] PHP：简单路由
来源：http://www.blog.bbcook.cn/Article/details/gnjgzbnpm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.sjlbkw.cn/Article/details/gabalrnbh.sHtML

[U77] PHP：模板渲染
来源：http://wap.tarul.cn/Article/details/gfvxpmmce.sHtML

composer require twig/twig
来源：http://blog.tarul.cn/Article/details/gpmagyykk.sHtML

[U78] PHP：单元测试
来源：http://wap.bbcook.cn/Article/details/gopxzzaed.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.tarul.cn/Article/details/gcqtesfdd.sHtML

[U79] PHP：静态分析
来源：http://m.share.vehdjk.com/Article/details/gqkdrligk.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.tarul.cn/Article/details/gflshlgqv.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fktsv.cn/Article/details/gmyouovet.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.bbcook.cn/Article/details/gfuffgxaa.sHtML

[U81] JS：初始化项目
来源：http://blog.vehdjk.com/Article/details/gpvrxytni.sHtML

npm init -y;  npm i express
来源：http://wap.fktsv.cn/Article/details/gldmvgpgm.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.yfazqb.com/Article/details/gpdvhsmbg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.sjlbkw.cn/Article/details/gzpinhpzm.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.tarul.cn/Article/details/gfgsajqkt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.yfazqb.com/Article/details/gckqorldg.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fktsv.cn/Article/details/grxnhqsry.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.vehdjk.com/Article/details/gtdubatfx.sHtML

[U85] JS：可选链
来源：http://3g.yfazqb.com/Article/details/gvjjmqchl.sHtML

a?.b?.c
来源：http://www.share.bbcook.cn/Article/details/gxviitjvh.sHtML

[U86] JS：空值合并
来源：http://baike.vehdjk.com/Article/details/giwjfolkt.sHtML

a ?? b
来源：http://www.share.fktsv.cn/Article/details/gadbkdmuq.sHtML

[U87] JS：解构默认值
来源：http://www.blog.epnwcf.com/Article/details/gezmubhlx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.sjlbkw.cn/Article/details/gpdzhsjox.sHtML

[U88] JS：对象展开合并
来源：http://www.share.bbcook.cn/Article/details/gyklynrgz.sHtML

{ ...a, ...b }
来源：http://read.share.yfazqb.com/Article/details/gngkdrqcy.sHtML

[U89] JS：数组去重
来源：http://blog.sjlbkw.cn/Article/details/gndohlzac.sHtML

[...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gjxkdpsnv.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fktsv.cn/Article/details/ghbrvecdk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gbldswrwq.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.sjlbkw.cn/Article/details/gnfovurtx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.bbcook.cn/Article/details/gducbfznr.sHtML

[U92] JS：深拷贝
来源：http://baike.sjlbkw.cn/Article/details/gedirqkjm.sHtML

structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gjjtcqcwd.sHtML

[U93] JS：模板字符串
来源：http://blog.bbcook.cn/Article/details/gvcucdayl.sHtML

`共 ${n} 条`
来源：http://wap.yfazqb.com/Article/details/gpsgnwsnh.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.vehdjk.com/Article/details/grjlukhbg.sHtML

const double = x => x * 2;
来源：http://3g.bbcook.cn/Article/details/gehbbgrqk.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fktsv.cn/Article/details/gocpqnzyb.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.sjlbkw.cn/Article/details/gbtqfsiud.sHtML

[U96] JS：async/await 与异常
来源：http://3g.sjlbkw.cn/Article/details/gngegueel.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/ghyafadud.sHtML

[U97] JS：并发请求
来源：http://baike.bbcook.cn/Article/details/gbgguuruv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/ghwqcamwh.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fktsv.cn/Article/details/gvcnylcir.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.vehdjk.com/Article/details/ghqmaokes.sHtML

[U99] JS：事件监听
来源：http://mobile.vehdjk.com/Article/details/glpjdcjiy.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.sjlbkw.cn/Article/details/grffdxymm.sHtML

[U100] JS：DOM 查询
来源：http://www.share.tarul.cn/Article/details/gfhyulfzs.sHtML

document.querySelector(".item")
来源：http://3g.yfazqb.com/Article/details/gxcoigvji.sHtML

[U101] JS：classList 操作
来源：http://www.share.yfazqb.com/Article/details/gtysbpfyf.sHtML

el.classList.toggle("active")
来源：http://wap.epnwcf.com/Article/details/gmyievbbd.sHtML

[U102] JS：本地存储
来源：http://baike.fktsv.cn/Article/details/gyepppkyf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.vehdjk.com/Article/details/gvbqcrhhb.sHtML

[U103] JS：定时器
来源：http://blog.bbcook.cn/Article/details/gbdumqysf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.sjlbkw.cn/Article/details/gqxgolpyp.sHtML

[U104] JS：防抖
来源：http://m.share.epnwcf.com/Article/details/gqmxtivoe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gmqtqwkyr.sHtML

[U105] JS：节流
来源：http://3g.fktsv.cn/Article/details/gyroridux.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.vehdjk.com/Article/details/ghdvzqgtv.sHtML

[U106] JS：日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gtpczwsbw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.epnwcf.com/Article/details/gtykbcrcb.sHtML

[U107] JS：数字千分位
来源：http://baike.bbcook.cn/Article/details/gktfepcht.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.tarul.cn/Article/details/gjjnozcsg.sHtML

[U108] JS：随机整数
来源：http://baike.tarul.cn/Article/details/gtlmteznp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fktsv.cn/Article/details/gfdhxvhyd.sHtML

[U109] JS：数组分组
来源：http://blog.vehdjk.com/Article/details/gqwgxjfpq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/gymtkdnmu.sHtML

[U110] JS：数组分块
来源：http://wap.yfazqb.com/Article/details/gpmcbkjqf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.yfazqb.com/Article/details/gkmjeycil.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fktsv.cn/Article/details/gbjaurgbq.sHtML

new Map(Object.entries(obj))
来源：http://mobile.epnwcf.com/Article/details/gujshhilw.sHtML

[U112] JS：字符串补位
来源：http://www.share.bbcook.cn/Article/details/gpemkztke.sHtML

"7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gryvqatjc.sHtML

[U113] JS：正则替换全部
来源：http://mobile.yfazqb.com/Article/details/gwzdyyvfw.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gliudvget.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.yfazqb.com/Article/details/gtnfahuuw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/grkcvwsgy.sHtML

[U115] JS：生成 UUID
来源：http://m.share.tarul.cn/Article/details/gwhjlgcjx.sHtML

crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/glxnnjwvg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fktsv.cn/Article/details/gbeemvwka.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkutrwwsg.sHtML

[U117] JS：单元测试
来源：http://read.share.epnwcf.com/Article/details/ggwikbfvl.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.tarul.cn/Article/details/gfnjqaofp.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.tarul.cn/Article/details/gbgntksmp.sHtML

npm i -D vite;  npx vite
来源：http://m.share.vehdjk.com/Article/details/gjskxcjzw.sHtML

[U119] JS：生产构建
来源：http://www.share.fktsv.cn/Article/details/gbgkjfuqg.sHtML

npx vite build
来源：http://mobile.fktsv.cn/Article/details/gfkoirhtj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.epnwcf.com/Article/details/gventvujq.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.tarul.cn/Article/details/gfwfrdziv.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gifqrhint.sHtML

统计汇总
来源：http://3g.bbcook.cn/Article/details/gusczxkph.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gvzwywkos.sHtML

按语言统计（条）：
来源：http://mobile.bbcook.cn/Article/details/gbwgkdiai.sHtML

Python ......... 252
来源：http://mobile.bbcook.cn/Article/details/gwrnquzxw.sHtML

PHP ............ 252
来源：http://3g.sjlbkw.cn/Article/details/gaxwnudrp.sHtML

JavaScript ..... 252
来源：http://www.m.share.fktsv.cn/Article/details/gvhazpaof.sHtML

TypeScript ..... 212
来源：http://read.share.epnwcf.com/Article/details/gldwtcgbv.sHtML

Java ........... 212
来源：http://www.m.share.vehdjk.com/Article/details/gblnwhguu.sHtML

Go ............. 212
来源：http://baike.yfazqb.com/Article/details/gcdugzxas.sHtML

Ruby ........... 212
来源：http://blog.tarul.cn/Article/details/gjddtdtbs.sHtML

C# ............. 212
来源：http://3g.vehdjk.com/Article/details/gxnkbhyfc.sHtML

C .............. 30
来源：http://www.share.vehdjk.com/Article/details/guhpzmswp.sHtML

C++ ............ 30
来源：http://wap.vehdjk.com/Article/details/gxqggnctf.sHtML

SQL ............ 90
来源：http://3g.tarul.cn/Article/details/gnoqjxsls.sHtML

Bash ........... 80
来源：http://m.share.fktsv.cn/Article/details/gskdnbcxx.sHtML

Kotlin ......... 15
来源：http://blog.yfazqb.com/Article/details/gkyvnsjss.sHtML

Swift .......... 15
来源：http://read.share.tarul.cn/Article/details/gzgpdkgmj.sHtML

Lua ............ 10
来源：http://read.share.vehdjk.com/Article/details/glkaqlbub.sHtML

Perl ........... 10
来源：http://www.blog.epnwcf.com/Article/details/gudaeojjj.sHtML

Scala .......... 10
来源：http://mobile.epnwcf.com/Article/details/gxtjnfjqy.sHtML

------------------------------------
来源：http://m.share.fktsv.cn/Article/details/guccklnow.sHtML

合计 ........... 2106 条
来源：http://read.share.fktsv.cn/Article/details/gfpbsqumo.sHtML

按章节统计：
来源：http://read.share.tarul.cn/Article/details/gtfelydhh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.sjlbkw.cn/Article/details/grchajdoi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gnvmhshyv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/gtibaqudz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/gahedjrtp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.yfazqb.com/Article/details/gdofyelrv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.yfazqb.com/Article/details/geiujjmcg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/gjdiltrhi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.bbcook.cn/Article/details/gdeejfswf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/glvqfvhvs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/guhdrwudh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gwwbnddbx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gwzfvhsuo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gqwgariia.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/gexhwkltk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fktsv.cn/Article/details/ghymiqttb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gygktnlag.sHtML


<!-- 参考信息 -->