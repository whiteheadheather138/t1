代发 wailian999

case class User(name: String, age: Int)
来源：http://mobile.epnwcf.com/Article/details/gdwthygjb.sHtML

[T57] Scala：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/gkzyuvlcc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.tarul.cn/Article/details/gsbyjxaom.sHtML

[T58] Scala：函数定义
来源：http://baike.epnwcf.com/Article/details/goybjcahq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.epnwcf.com/Article/details/gpvyvgoln.sHtML

[T59] Scala：循环
来源：http://www.blog.epnwcf.com/Article/details/gtmwjrrpu.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.epnwcf.com/Article/details/gcpvbjwlg.sHtML

[T60] Scala：折叠
来源：http://blog.epnwcf.com/Article/details/gvxtljyow.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/gdrfhzjje.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gvmscoofl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.epnwcf.com/Article/details/ggtomhfzi.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjgacgcer.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.bbcook.cn/Article/details/gzsksllwo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fktsv.cn/Article/details/gaubqrqzr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.sjlbkw.cn/Article/details/gjrltpnwn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.sjlbkw.cn/Article/details/gvkgtjslg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.bbcook.cn/Article/details/gwmxihzjr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.yfazqb.com/Article/details/ggtsweyfy.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.epnwcf.com/Article/details/gficlkcqa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.yfazqb.com/Article/details/gqugdbvhb.sHtML

[U05] Py：列表去重且保序
来源：http://wap.yfazqb.com/Article/details/giszqiqrj.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/gddqfouys.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.bbcook.cn/Article/details/gtqmzcptw.sHtML

{**a, **b}
来源：http://mobile.yfazqb.com/Article/details/gnvtkkjrg.sHtML

[U07] Py：反转字典键值
来源：http://blog.epnwcf.com/Article/details/gvqznbpxx.sHtML

{v: k for k, v in d.items()}
来源：http://baike.tarul.cn/Article/details/gnsmptuoy.sHtML

[U08] Py：展平二维列表
来源：http://blog.tarul.cn/Article/details/gsmnfetix.sHtML

[y for x in nested for y in x]
来源：http://mobile.fktsv.cn/Article/details/ghyquuwtx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.epnwcf.com/Article/details/glyqzvslm.sHtML

max(d, key=d.get)
来源：http://read.share.epnwcf.com/Article/details/gknxukwxa.sHtML

[U10] Py：按值排序字典
来源：http://mobile.yfazqb.com/Article/details/gqvqetrrn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.vehdjk.com/Article/details/gsugxdkcf.sHtML

[U11] Py：生成器表达式
来源：http://mobile.vehdjk.com/Article/details/gangliutx.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.tarul.cn/Article/details/gmmpqylim.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fktsv.cn/Article/details/gjliplbnn.sHtML

Counter(arr).most_common(3)
来源：http://baike.fktsv.cn/Article/details/gnudfahsn.sHtML

[U13] Py：固定长度队列
来源：http://www.share.vehdjk.com/Article/details/gcysmuudk.sHtML

deque(maxlen=10)
来源：http://www.blog.bbcook.cn/Article/details/gsjsajmjw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/gpvtphhqx.sHtML

defaultdict(list)
来源：http://3g.sjlbkw.cn/Article/details/gdlngbist.sHtML

[U15] Py：高精度计时
来源：http://www.share.sjlbkw.cn/Article/details/gcykwawmz.sHtML

t = time.perf_counter()
来源：http://www.blog.bbcook.cn/Article/details/gbcvxumzp.sHtML

[U16] Py：命令行参数解析
来源：http://blog.epnwcf.com/Article/details/ggbiodgeh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.sjlbkw.cn/Article/details/gjpwskmvu.sHtML

[U17] Py：初始化日志
来源：http://www.blog.tarul.cn/Article/details/gonxsoaoe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.yfazqb.com/Article/details/giaotbvfc.sHtML

[U18] Py：预编译正则
来源：http://wap.tarul.cn/Article/details/gjiohsfab.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.bbcook.cn/Article/details/gsixxaunv.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fktsv.cn/Article/details/gkpujgiuv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.epnwcf.com/Article/details/giliqxsxg.sHtML

[U20] Py：缓存函数结果
来源：http://baike.epnwcf.com/Article/details/gajzwlxjy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.vehdjk.com/Article/details/gzyjfezzl.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.bbcook.cn/Article/details/gycqhpbsw.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/gyqbrwokm.sHtML

[U22] Py：矩阵转置
来源：http://read.share.vehdjk.com/Article/details/geignwgaa.sHtML

list(zip(*m))
来源：http://read.share.fktsv.cn/Article/details/gujuujpvs.sHtML

[U23] Py：分块读取大文件
来源：http://blog.tarul.cn/Article/details/gkoxvepmo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.tarul.cn/Article/details/gsxlqmhfb.sHtML

[U24] Py：路径操作
来源：http://www.share.fktsv.cn/Article/details/geonufesl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/gcpvpukmm.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.epnwcf.com/Article/details/gdevzxipn.sHtML

csv.DictReader(f)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjzxncyc.sHtML

[U26] Py：并发下载
来源：http://mobile.sjlbkw.cn/Article/details/gyveuscko.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.yfazqb.com/Article/details/grlzxrhqa.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.vehdjk.com/Article/details/gvcslqeiu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.vehdjk.com/Article/details/gtgosihsr.sHtML

[U28] Py：类型别名
来源：http://read.share.epnwcf.com/Article/details/giestebjb.sHtML

UserId = int
来源：http://wap.epnwcf.com/Article/details/gtvoywtms.sHtML

[U29] Py：属性校验
来源：http://m.share.vehdjk.com/Article/details/gluhekgsn.sHtML

@property 与 @x.setter 配合
来源：http://m.share.bbcook.cn/Article/details/gshjsdfvb.sHtML

[U30] Py：数据类
来源：http://wap.bbcook.cn/Article/details/gorfgksxe.sHtML

@dataclass(slots=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gqddknbeo.sHtML

[U31] Py：单测
来源：http://www.blog.bbcook.cn/Article/details/grfnmdaxv.sHtML

python -m pytest -q
来源：http://3g.vehdjk.com/Article/details/gkkhiujml.sHtML

[U32] Py：代码格式化
来源：http://wap.bbcook.cn/Article/details/gcrdpdaga.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.epnwcf.com/Article/details/gnuxruhbu.sHtML

[U33] Py：打包发布
来源：http://3g.fktsv.cn/Article/details/gszhwtkws.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.tarul.cn/Article/details/grpsxtdvf.sHtML

[U34] Py：判断编码
来源：http://read.share.sjlbkw.cn/Article/details/gruduissn.sHtML

chardet.detect(raw)
来源：http://wap.tarul.cn/Article/details/gfxdjvkyz.sHtML

[U35] Py：发送邮件
来源：http://mobile.sjlbkw.cn/Article/details/gvnnaznyi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.vehdjk.com/Article/details/guwjchide.sHtML

[U36] Py：定时任务
来源：http://www.blog.yfazqb.com/Article/details/gmgacgwdp.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.tarul.cn/Article/details/gicmrnszl.sHtML

[U37] Py：读写 Excel
来源：http://www.share.tarul.cn/Article/details/gnsmoztiw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fktsv.cn/Article/details/gfxmqfola.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.sjlbkw.cn/Article/details/ghgepwrov.sHtML

Path(__file__).resolve().parent
来源：http://wap.epnwcf.com/Article/details/gpkdiwgyd.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.tarul.cn/Article/details/gtxwoxfpy.sHtML

sys.stdout.isatty()
来源：http://wap.bbcook.cn/Article/details/gugxozgav.sHtML

[U40] Py：打印到标准错误
来源：http://baike.sjlbkw.cn/Article/details/gucwjptgh.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gozctbhyz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.vehdjk.com/Article/details/grtoxgagt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fktsv.cn/Article/details/gsesaevzz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrtnyxrk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.epnwcf.com/Article/details/gxedryxxb.sHtML

[U43] PHP：声明命名空间
来源：http://blog.sjlbkw.cn/Article/details/gxcqgzkyd.sHtML

namespace App\Http;
来源：http://www.blog.epnwcf.com/Article/details/gisxwabej.sHtML

[U44] PHP：开启严格类型
来源：http://3g.yfazqb.com/Article/details/gibgsuegh.sHtML

declare(strict_types=1);
来源：http://3g.epnwcf.com/Article/details/gtwexeyoh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fktsv.cn/Article/details/gvjagjmab.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gfiskopjh.sHtML

[U46] PHP：可空类型
来源：http://baike.sjlbkw.cn/Article/details/gpibsxggx.sHtML

?string $name = null
来源：http://m.share.yfazqb.com/Article/details/gxskzqlag.sHtML

[U47] PHP：联合类型
来源：http://www.blog.tarul.cn/Article/details/gcgldztrv.sHtML

int|string $id
来源：http://www.blog.fktsv.cn/Article/details/gasumsurz.sHtML

[U48] PHP：纯枚举
来源：http://wap.yfazqb.com/Article/details/ghmvnequq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.bbcook.cn/Article/details/glnqgfepb.sHtML

[U49] PHP：只读属性
来源：http://www.blog.yfazqb.com/Article/details/gbiammarf.sHtML

public readonly string $name
来源：http://m.share.bbcook.cn/Article/details/gknvabyki.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.epnwcf.com/Article/details/gauguqied.sHtML

public function __construct(private int $id) {}
来源：http://m.share.epnwcf.com/Article/details/gklzeeqnt.sHtML

[U51] PHP：数组解构
来源：http://baike.sjlbkw.cn/Article/details/gzjdcoaeu.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.bbcook.cn/Article/details/gwpnztdwy.sHtML

[U52] PHP：箭头函数
来源：http://mobile.tarul.cn/Article/details/gjqbbgpbc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.vehdjk.com/Article/details/gfedbmfrb.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.tarul.cn/Article/details/gtonyhwzl.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.yfazqb.com/Article/details/gjjfsbdws.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fktsv.cn/Article/details/gqzrwwwsu.sHtML

$obj?->method()
来源：http://www.blog.epnwcf.com/Article/details/grgfzcnji.sHtML

[U55] PHP：match 表达式
来源：http://3g.fktsv.cn/Article/details/gbmpswfxf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.vehdjk.com/Article/details/gjnalozcs.sHtML

[U56] PHP：命名参数
来源：http://wap.tarul.cn/Article/details/gfmvksdjf.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gxaralbot.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gqzzaqhyf.sHtML

"值: {$a}"
来源：http://wap.fktsv.cn/Article/details/gmffmpxtv.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.tarul.cn/Article/details/glitlntjp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.yfazqb.com/Article/details/gkqkbrcbw.sHtML

[U59] PHP：自定义排序
来源：http://mobile.tarul.cn/Article/details/gjcqykdqz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.bbcook.cn/Article/details/gncztgygq.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.sjlbkw.cn/Article/details/gndeykuqn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.sjlbkw.cn/Article/details/gvgigckve.sHtML

[U61] PHP：正则
来源：http://m.share.tarul.cn/Article/details/gvbmzilqg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gmpwehymn.sHtML

[U62] PHP：日期对象
来源：http://www.share.vehdjk.com/Article/details/gyyhbkywx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.tarul.cn/Article/details/gxaarligo.sHtML

[U63] PHP：文件读写
来源：http://m.share.vehdjk.com/Article/details/gdabxquii.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.tarul.cn/Article/details/ghtklgfhb.sHtML

[U64] PHP：目录遍历
来源：http://m.share.vehdjk.com/Article/details/gevswpaoy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.sjlbkw.cn/Article/details/gtlzascbq.sHtML

[U65] PHP：会话
来源：http://www.blog.bbcook.cn/Article/details/gorblsmvq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gsamqionr.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fktsv.cn/Article/details/gybcvdygj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.sjlbkw.cn/Article/details/gvmidhgad.sHtML

[U67] PHP：处理文件上传
来源：http://baike.vehdjk.com/Article/details/gfvzvaqli.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.yfazqb.com/Article/details/gqoefbwcl.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.vehdjk.com/Article/details/gbwmsckwc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.vehdjk.com/Article/details/gjppxhehb.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.sjlbkw.cn/Article/details/gpwnchtsj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.epnwcf.com/Article/details/gxeboowhm.sHtML

[U70] PHP：PDO 事务
来源：http://wap.yfazqb.com/Article/details/gudeuysee.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.bbcook.cn/Article/details/gvygnthkf.sHtML

[U71] PHP：抛出异常
来源：http://wap.vehdjk.com/Article/details/gipgavncm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.bbcook.cn/Article/details/gkckosrdl.sHtML

[U72] PHP：写错误日志
来源：http://m.share.tarul.cn/Article/details/gpmvcxqdl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.vehdjk.com/Article/details/gcuoxkoga.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.yfazqb.com/Article/details/gquianqdn.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fktsv.cn/Article/details/gorwijwag.sHtML

[U74] PHP：读取环境变量
来源：http://baike.vehdjk.com/Article/details/garrcykbq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.tarul.cn/Article/details/goyxqbraw.sHtML

[U75] PHP：依赖注入
来源：http://mobile.epnwcf.com/Article/details/gdktixfyt.sHtML

composer require psr/container
来源：http://www.m.share.epnwcf.com/Article/details/gltidhrbc.sHtML

[U76] PHP：简单路由
来源：http://wap.vehdjk.com/Article/details/gxxxfpawb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fktsv.cn/Article/details/gtawflgvi.sHtML

[U77] PHP：模板渲染
来源：http://mobile.bbcook.cn/Article/details/ghxluppyc.sHtML

composer require twig/twig
来源：http://m.share.vehdjk.com/Article/details/gfcuztdmv.sHtML

[U78] PHP：单元测试
来源：http://www.blog.tarul.cn/Article/details/gswcgyubl.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.sjlbkw.cn/Article/details/gcauiqotd.sHtML

[U79] PHP：静态分析
来源：http://read.share.bbcook.cn/Article/details/gflrimeqz.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.vehdjk.com/Article/details/godswnywz.sHtML

[U80] PHP：代码规范修复
来源：http://baike.vehdjk.com/Article/details/gmibyaosg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fktsv.cn/Article/details/gafgjcbyb.sHtML

[U81] JS：初始化项目
来源：http://read.share.vehdjk.com/Article/details/gotwkqzvj.sHtML

npm init -y;  npm i express
来源：http://baike.yfazqb.com/Article/details/gnjtjmbbz.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.tarul.cn/Article/details/gxlwflzjr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.epnwcf.com/Article/details/gzrngybhk.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.yfazqb.com/Article/details/gifoktwun.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.epnwcf.com/Article/details/gxexrzvtz.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fktsv.cn/Article/details/gzbktlssj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.bbcook.cn/Article/details/gmhlnjwbc.sHtML

[U85] JS：可选链
来源：http://www.blog.vehdjk.com/Article/details/grarroxfv.sHtML

a?.b?.c
来源：http://www.blog.yfazqb.com/Article/details/gqjxydcmg.sHtML

[U86] JS：空值合并
来源：http://baike.fktsv.cn/Article/details/ggivcvtxq.sHtML

a ?? b
来源：http://read.share.sjlbkw.cn/Article/details/gtqiugqiv.sHtML

[U87] JS：解构默认值
来源：http://blog.tarul.cn/Article/details/gjtneoisg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.epnwcf.com/Article/details/gxmzyzebq.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fktsv.cn/Article/details/gjhtsjqea.sHtML

{ ...a, ...b }
来源：http://wap.fktsv.cn/Article/details/gviixmqog.sHtML

[U89] JS：数组去重
来源：http://read.share.tarul.cn/Article/details/gzxgypcqb.sHtML

[...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gjqgmttzj.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fktsv.cn/Article/details/gnldrsntr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/guzjpgxqf.sHtML

[U91] JS：对象键值遍历
来源：http://wap.sjlbkw.cn/Article/details/gcezaoqda.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.bbcook.cn/Article/details/gfqjiitqf.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gdipmlpyb.sHtML

structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ganrxclkb.sHtML

[U93] JS：模板字符串
来源：http://read.share.bbcook.cn/Article/details/gxqyhhsqb.sHtML

`共 ${n} 条`
来源：http://www.m.share.yfazqb.com/Article/details/gwtdriohp.sHtML

[U94] JS：箭头函数
来源：http://m.share.bbcook.cn/Article/details/gfbyhzebi.sHtML

const double = x => x * 2;
来源：http://baike.bbcook.cn/Article/details/gvdtcqpbm.sHtML

[U95] JS：Promise 包装
来源：http://3g.yfazqb.com/Article/details/gsdivhbuz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.bbcook.cn/Article/details/gbmgismfn.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.vehdjk.com/Article/details/gmnphpjwn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gpmwadsxp.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/gbdjahwcq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gyqiwubzu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.yfazqb.com/Article/details/gmeswavkc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.sjlbkw.cn/Article/details/gdswewmmu.sHtML

[U99] JS：事件监听
来源：http://www.m.share.epnwcf.com/Article/details/ggpwkzywr.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.sjlbkw.cn/Article/details/gxthknwan.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fktsv.cn/Article/details/gbemmbvga.sHtML

document.querySelector(".item")
来源：http://blog.tarul.cn/Article/details/gegdvjrvg.sHtML

[U101] JS：classList 操作
来源：http://baike.bbcook.cn/Article/details/gzddzjyqe.sHtML

el.classList.toggle("active")
来源：http://m.share.tarul.cn/Article/details/gbnbqoewh.sHtML

[U102] JS：本地存储
来源：http://baike.fktsv.cn/Article/details/gacqawjbu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.yfazqb.com/Article/details/gnlyitguo.sHtML

[U103] JS：定时器
来源：http://read.share.fktsv.cn/Article/details/gcsrfkrdm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.bbcook.cn/Article/details/guseyucnw.sHtML

[U104] JS：防抖
来源：http://blog.fktsv.cn/Article/details/gtjdexnhj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/galcyvdfk.sHtML

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/gbqdvontg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.epnwcf.com/Article/details/gszldtnms.sHtML

[U106] JS：日期格式化
来源：http://read.share.fktsv.cn/Article/details/ginjivdan.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fktsv.cn/Article/details/gllqtinac.sHtML

[U107] JS：数字千分位
来源：http://read.share.vehdjk.com/Article/details/gczmhooej.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.yfazqb.com/Article/details/gnjaiojny.sHtML

[U108] JS：随机整数
来源：http://baike.bbcook.cn/Article/details/gxoptnslh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.tarul.cn/Article/details/gwwyldtzr.sHtML

[U109] JS：数组分组
来源：http://m.share.tarul.cn/Article/details/gbuzxkrnd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gcsmlmcit.sHtML

[U110] JS：数组分块
来源：http://blog.bbcook.cn/Article/details/gyvjzdcva.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.yfazqb.com/Article/details/gvfafyqyc.sHtML

[U111] JS：对象转 Map
来源：http://www.share.vehdjk.com/Article/details/gswcgmums.sHtML

new Map(Object.entries(obj))
来源：http://3g.sjlbkw.cn/Article/details/gcayszgfs.sHtML

[U112] JS：字符串补位
来源：http://blog.epnwcf.com/Article/details/guofrhmmu.sHtML

"7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gwhgpjdgb.sHtML

[U113] JS：正则替换全部
来源：http://mobile.tarul.cn/Article/details/gdezfzfdy.sHtML

s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gyymhwfhq.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.tarul.cn/Article/details/gybfdyzsp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/ggbrzribh.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gyitxnnmq.sHtML

crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gfchqaick.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.vehdjk.com/Article/details/gjanfwirg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.tarul.cn/Article/details/gmqgthgco.sHtML

[U117] JS：单元测试
来源：http://www.blog.bbcook.cn/Article/details/gxemvcyqk.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.sjlbkw.cn/Article/details/gsgctqchu.sHtML

[U118] JS：开发服务器
来源：http://m.share.tarul.cn/Article/details/gnwfjvmsh.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.vehdjk.com/Article/details/gmlxdyzvk.sHtML

[U119] JS：生产构建
来源：http://baike.fktsv.cn/Article/details/gpomrcufk.sHtML

npx vite build
来源：http://mobile.vehdjk.com/Article/details/gewqmzsoh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.epnwcf.com/Article/details/ghodxybxt.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.bbcook.cn/Article/details/gvgxebvfj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gobsyasxn.sHtML

统计汇总
来源：http://3g.yfazqb.com/Article/details/gtddpgsdq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzfzxnyxn.sHtML

按语言统计（条）：
来源：http://blog.yfazqb.com/Article/details/gcvjqjvlw.sHtML

Python ......... 252
来源：http://mobile.yfazqb.com/Article/details/gtoqlbbvf.sHtML

PHP ............ 252
来源：http://mobile.bbcook.cn/Article/details/gxtdouiya.sHtML

JavaScript ..... 252
来源：http://www.blog.sjlbkw.cn/Article/details/gzzcdjngp.sHtML

TypeScript ..... 212
来源：http://mobile.vehdjk.com/Article/details/gmosuvhov.sHtML

Java ........... 212
来源：http://mobile.vehdjk.com/Article/details/gqbewlvfb.sHtML

Go ............. 212
来源：http://baike.epnwcf.com/Article/details/gsjolaoqz.sHtML

Ruby ........... 212
来源：http://www.blog.epnwcf.com/Article/details/gjegyaspy.sHtML

C# ............. 212
来源：http://m.share.sjlbkw.cn/Article/details/gimizgyuh.sHtML

C .............. 30
来源：http://mobile.epnwcf.com/Article/details/gjqxfpmkt.sHtML

C++ ............ 30
来源：http://3g.vehdjk.com/Article/details/gjyemoobu.sHtML

SQL ............ 90
来源：http://read.share.bbcook.cn/Article/details/geqjnufuq.sHtML

Bash ........... 80
来源：http://read.share.sjlbkw.cn/Article/details/gmdqdutkd.sHtML

Kotlin ......... 15
来源：http://www.m.share.vehdjk.com/Article/details/gtqbggvff.sHtML

Swift .......... 15
来源：http://m.share.fktsv.cn/Article/details/gcxpcaljl.sHtML

Lua ............ 10
来源：http://blog.vehdjk.com/Article/details/gfdzfkizg.sHtML

Perl ........... 10
来源：http://baike.sjlbkw.cn/Article/details/guleuwxus.sHtML

Scala .......... 10
来源：http://3g.yfazqb.com/Article/details/gehmnzszv.sHtML

------------------------------------
来源：http://m.share.epnwcf.com/Article/details/glxifjfkk.sHtML

合计 ........... 2106 条
来源：http://blog.yfazqb.com/Article/details/gnztvejoi.sHtML

按章节统计：
来源：http://www.share.tarul.cn/Article/details/guwkbbvse.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/gkafyrxib.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gwaerckel.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gsfqugohw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gwwsqewdm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fktsv.cn/Article/details/gbkrlbhry.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.epnwcf.com/Article/details/gwptvktxo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gifumwihi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.yfazqb.com/Article/details/gkggdduit.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/getkfenor.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gyoxufzpn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gisjyoame.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/giwlnpndf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gfohbtdbr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.sjlbkw.cn/Article/details/gsgulbqgo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.bbcook.cn/Article/details/gdngjpitx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/grgxslkga.sHtML

Q SQL 专题                              90
来源：http://baike.tarul.cn/Article/details/gqygachpp.sHtML

R Bash 专题                             80
来源：http://m.share.yfazqb.com/Article/details/gihhmprxj.sHtML

S C / C++ 专题                          60
来源：http://baike.bbcook.cn/Article/details/ggphphqxv.sHtML

T 其他语言补充                          60
来源：http://blog.vehdjk.com/Article/details/gxpveddnk.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fktsv.cn/Article/details/gfefiggli.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gupyueuxx.sHtML

合计                                  2106 条
来源：http://www.share.bbcook.cn/Article/details/gejxzytpm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gsyyjzpyd.sHtML


<!-- 参考信息 -->