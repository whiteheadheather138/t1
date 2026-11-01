代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.share.tarul.cn/Article/details/gqhjilwjb.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/giemlbnuf.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gmeleusuy.sHtML

[T52] Scala：变量
来源：http://3g.epnwcf.com/Article/details/gaycqaonu.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gfpjabnmn.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gkyepvoub.sHtML

s"值: $b"
来源：http://wap.tarul.cn/Article/details/gwhirxnza.sHtML

[T54] Scala：集合映射
来源：http://m.share.fktsv.cn/Article/details/gtnxcpkni.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.vehdjk.com/Article/details/gdoxaxqnj.sHtML

[T55] Scala：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gckxnrljr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.tarul.cn/Article/details/gwbauzchl.sHtML

[T56] Scala：样例类
来源：http://www.blog.sjlbkw.cn/Article/details/gaobczsor.sHtML

case class User(name: String, age: Int)
来源：http://m.share.epnwcf.com/Article/details/gzwdktxjg.sHtML

[T57] Scala：模式匹配
来源：http://read.share.vehdjk.com/Article/details/gllcvmgyt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.yfazqb.com/Article/details/guntkwybi.sHtML

[T58] Scala：函数定义
来源：http://m.share.sjlbkw.cn/Article/details/gxcacxugy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.sjlbkw.cn/Article/details/goxwxbjlr.sHtML

[T59] Scala：循环
来源：http://wap.tarul.cn/Article/details/gpheajvra.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.tarul.cn/Article/details/gdpvyymth.sHtML

[T60] Scala：折叠
来源：http://3g.sjlbkw.cn/Article/details/gkwnbztbc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.epnwcf.com/Article/details/gfcjmpfjy.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gksgbtxtf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.tarul.cn/Article/details/ginwwuhca.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggvyupieh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.epnwcf.com/Article/details/gwxmjjsql.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.tarul.cn/Article/details/gbfmnvmcv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.sjlbkw.cn/Article/details/ghaeutocq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.bbcook.cn/Article/details/gvszlingo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.tarul.cn/Article/details/gjtukcxza.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.bbcook.cn/Article/details/gaxvvrrcu.sHtML

[U04] Py：变量调试打印
来源：http://3g.fktsv.cn/Article/details/gqjnkkubx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.bbcook.cn/Article/details/gnyzjciov.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.bbcook.cn/Article/details/gifynamfj.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gjezicrxu.sHtML

[U06] Py：合并两个字典
来源：http://read.share.bbcook.cn/Article/details/gtsjredfi.sHtML

{**a, **b}
来源：http://mobile.vehdjk.com/Article/details/gztqldktl.sHtML

[U07] Py：反转字典键值
来源：http://m.share.sjlbkw.cn/Article/details/gorgyawyy.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.sjlbkw.cn/Article/details/gqtvedwqp.sHtML

[U08] Py：展平二维列表
来源：http://baike.bbcook.cn/Article/details/gbnobxnjd.sHtML

[y for x in nested for y in x]
来源：http://3g.bbcook.cn/Article/details/gmzrmgzin.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.tarul.cn/Article/details/gwazeoaed.sHtML

max(d, key=d.get)
来源：http://www.m.share.vehdjk.com/Article/details/ggqisgglg.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlpffuia.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.bbcook.cn/Article/details/gcoadlsip.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fktsv.cn/Article/details/gizgcfavh.sHtML

(x * 2 for x in arr)
来源：http://mobile.epnwcf.com/Article/details/gksehfvco.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fktsv.cn/Article/details/glmfteoky.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.epnwcf.com/Article/details/guzylaqav.sHtML

[U13] Py：固定长度队列
来源：http://mobile.vehdjk.com/Article/details/gepvgzxxk.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/gqohudbew.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.tarul.cn/Article/details/gqlzkjtal.sHtML

defaultdict(list)
来源：http://www.m.share.fktsv.cn/Article/details/gbezsubnc.sHtML

[U15] Py：高精度计时
来源：http://3g.bbcook.cn/Article/details/gjhtiurvo.sHtML

t = time.perf_counter()
来源：http://wap.fktsv.cn/Article/details/gtpwtmago.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.yfazqb.com/Article/details/ghrpicybi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.sjlbkw.cn/Article/details/gckmqrllz.sHtML

[U17] Py：初始化日志
来源：http://3g.epnwcf.com/Article/details/gzqwkoiib.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.epnwcf.com/Article/details/gbikgjjya.sHtML

[U18] Py：预编译正则
来源：http://mobile.yfazqb.com/Article/details/gsdojhfwo.sHtML

pat = re.compile(r"\d+")
来源：http://3g.bbcook.cn/Article/details/gapbofuaq.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.vehdjk.com/Article/details/gnroepbtu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fktsv.cn/Article/details/gdwzbenin.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.vehdjk.com/Article/details/gcdnkcgly.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.bbcook.cn/Article/details/gpkurlfxx.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.epnwcf.com/Article/details/goearirca.sHtML

@contextlib.contextmanager
来源：http://www.m.share.yfazqb.com/Article/details/gcotmzpeq.sHtML

[U22] Py：矩阵转置
来源：http://mobile.vehdjk.com/Article/details/ghfkujsxk.sHtML

list(zip(*m))
来源：http://www.share.tarul.cn/Article/details/gbyqebqfz.sHtML

[U23] Py：分块读取大文件
来源：http://wap.yfazqb.com/Article/details/gqtdyksog.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.sjlbkw.cn/Article/details/gwvnkgqvj.sHtML

[U24] Py：路径操作
来源：http://blog.bbcook.cn/Article/details/gnonfdfsc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gklkqxvqn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgzeezjt.sHtML

csv.DictReader(f)
来源：http://blog.fktsv.cn/Article/details/gltuptuot.sHtML

[U26] Py：并发下载
来源：http://baike.epnwcf.com/Article/details/gljfittcs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.epnwcf.com/Article/details/grmasyidq.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.bbcook.cn/Article/details/ghuboqtrv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.bbcook.cn/Article/details/gvhstisoh.sHtML

[U28] Py：类型别名
来源：http://mobile.bbcook.cn/Article/details/gblalsuxv.sHtML

UserId = int
来源：http://3g.fktsv.cn/Article/details/gzwgvnjig.sHtML

[U29] Py：属性校验
来源：http://www.m.share.tarul.cn/Article/details/gfogdtdpm.sHtML

@property 与 @x.setter 配合
来源：http://read.share.sjlbkw.cn/Article/details/glyvmaivu.sHtML

[U30] Py：数据类
来源：http://www.share.epnwcf.com/Article/details/gycvwetku.sHtML

@dataclass(slots=True)
来源：http://read.share.sjlbkw.cn/Article/details/gpjnhjnea.sHtML

[U31] Py：单测
来源：http://read.share.yfazqb.com/Article/details/gsnhgiexv.sHtML

python -m pytest -q
来源：http://www.share.fktsv.cn/Article/details/gncpmijzv.sHtML

[U32] Py：代码格式化
来源：http://wap.vehdjk.com/Article/details/gyldcfdef.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.vehdjk.com/Article/details/gmqkmftaz.sHtML

[U33] Py：打包发布
来源：http://baike.epnwcf.com/Article/details/gpflqldnm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.yfazqb.com/Article/details/gmtkbjiuq.sHtML

[U34] Py：判断编码
来源：http://3g.vehdjk.com/Article/details/gnhltncii.sHtML

chardet.detect(raw)
来源：http://www.share.bbcook.cn/Article/details/gwfzzcjxs.sHtML

[U35] Py：发送邮件
来源：http://baike.bbcook.cn/Article/details/gewhojrcu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.vehdjk.com/Article/details/gsrhkfqtk.sHtML

[U36] Py：定时任务
来源：http://baike.sjlbkw.cn/Article/details/gwobezixl.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.yfazqb.com/Article/details/gmxrerbco.sHtML

[U37] Py：读写 Excel
来源：http://wap.epnwcf.com/Article/details/gexbgsymb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.bbcook.cn/Article/details/gqjmoggsw.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.sjlbkw.cn/Article/details/ghjuvwcif.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fktsv.cn/Article/details/gocwfdznu.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.vehdjk.com/Article/details/gksymyzhq.sHtML

sys.stdout.isatty()
来源：http://wap.fktsv.cn/Article/details/ghcbasqev.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.epnwcf.com/Article/details/gfnbztohd.sHtML

print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gyeptnpwd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.tarul.cn/Article/details/gxasrujer.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.epnwcf.com/Article/details/gezrwccce.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.bbcook.cn/Article/details/gdwnxqvsn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.sjlbkw.cn/Article/details/gmopjkesh.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.sjlbkw.cn/Article/details/gpfuigbeu.sHtML

namespace App\Http;
来源：http://mobile.fktsv.cn/Article/details/gqqovjjpn.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxmhmhxd.sHtML

declare(strict_types=1);
来源：http://m.share.vehdjk.com/Article/details/gzmkgflqm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.bbcook.cn/Article/details/gpkevjaha.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gxjlambnx.sHtML

[U46] PHP：可空类型
来源：http://www.blog.vehdjk.com/Article/details/gnpkjdlps.sHtML

?string $name = null
来源：http://3g.sjlbkw.cn/Article/details/gcfthwzxj.sHtML

[U47] PHP：联合类型
来源：http://wap.vehdjk.com/Article/details/ghfdapzub.sHtML

int|string $id
来源：http://3g.tarul.cn/Article/details/gmqsodidd.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fktsv.cn/Article/details/ggvybjqef.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.bbcook.cn/Article/details/gjyrgsnpp.sHtML

[U49] PHP：只读属性
来源：http://m.share.yfazqb.com/Article/details/gczmtqfmy.sHtML

public readonly string $name
来源：http://baike.fktsv.cn/Article/details/gwthmzleg.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.vehdjk.com/Article/details/gqxgxjbiz.sHtML

public function __construct(private int $id) {}
来源：http://www.share.bbcook.cn/Article/details/gwbmpstji.sHtML

[U51] PHP：数组解构
来源：http://mobile.fktsv.cn/Article/details/ggjjygpfv.sHtML

[$a, $b] = $arr;
来源：http://read.share.vehdjk.com/Article/details/gmflzajfx.sHtML

[U52] PHP：箭头函数
来源：http://wap.yfazqb.com/Article/details/gzbfrbgza.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.epnwcf.com/Article/details/gpzgwkvke.sHtML

[U53] PHP：空合并运算符
来源：http://wap.epnwcf.com/Article/details/gyznebzyo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fktsv.cn/Article/details/guzlzrzzi.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.sjlbkw.cn/Article/details/gfbhwzjli.sHtML

$obj?->method()
来源：http://baike.bbcook.cn/Article/details/gugubdvow.sHtML

[U55] PHP：match 表达式
来源：http://wap.sjlbkw.cn/Article/details/gfselowfe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.yfazqb.com/Article/details/gpfwlmjls.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpwputct.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/giiubrmtr.sHtML

[U57] PHP：字符串插值
来源：http://3g.vehdjk.com/Article/details/gdlxauscy.sHtML

"值: {$a}"
来源：http://wap.vehdjk.com/Article/details/gixvmiaeb.sHtML

[U58] PHP：数组三件套
来源：http://read.share.epnwcf.com/Article/details/gvcyjqhet.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.vehdjk.com/Article/details/gdvzdwhwt.sHtML

[U59] PHP：自定义排序
来源：http://m.share.bbcook.cn/Article/details/gbxdojtbe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/gvghoeasv.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.tarul.cn/Article/details/grakkpoij.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fktsv.cn/Article/details/gbihireqn.sHtML

[U61] PHP：正则
来源：http://www.share.sjlbkw.cn/Article/details/gofmqferh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gnuftywvn.sHtML

[U62] PHP：日期对象
来源：http://m.share.bbcook.cn/Article/details/gwitubuci.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.yfazqb.com/Article/details/gbuoejhwx.sHtML

[U63] PHP：文件读写
来源：http://wap.tarul.cn/Article/details/gomivyetg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fktsv.cn/Article/details/gzkzgbziu.sHtML

[U64] PHP：目录遍历
来源：http://wap.fktsv.cn/Article/details/gxtiemuko.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fktsv.cn/Article/details/gwrnscmha.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/gwnaogvfe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.bbcook.cn/Article/details/gocydyern.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.epnwcf.com/Article/details/gpcdezulc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.sjlbkw.cn/Article/details/gatefhwmq.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fktsv.cn/Article/details/gsakupyzh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.epnwcf.com/Article/details/gvpobyjqk.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcaajwfy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.bbcook.cn/Article/details/ghebaqhbu.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fktsv.cn/Article/details/gqinouecc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.epnwcf.com/Article/details/gbkyfbjnr.sHtML

[U70] PHP：PDO 事务
来源：http://baike.bbcook.cn/Article/details/gqhwcavmf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.yfazqb.com/Article/details/gwhybomgz.sHtML

[U71] PHP：抛出异常
来源：http://3g.epnwcf.com/Article/details/gvhqfxhly.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.bbcook.cn/Article/details/gsfmvsgug.sHtML

[U72] PHP：写错误日志
来源：http://www.share.sjlbkw.cn/Article/details/gzbhowqrf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.yfazqb.com/Article/details/ghmslqjzb.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.epnwcf.com/Article/details/gdizdjtmv.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.bbcook.cn/Article/details/gvxxytzdv.sHtML

[U74] PHP：读取环境变量
来源：http://3g.bbcook.cn/Article/details/gfwxaqywj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.tarul.cn/Article/details/geocrsknu.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjlaaxit.sHtML

composer require psr/container
来源：http://baike.epnwcf.com/Article/details/gcrhusspm.sHtML

[U76] PHP：简单路由
来源：http://baike.epnwcf.com/Article/details/gtcwyabgu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.epnwcf.com/Article/details/gxdxfidtx.sHtML

[U77] PHP：模板渲染
来源：http://www.share.tarul.cn/Article/details/gxhqadqyx.sHtML

composer require twig/twig
来源：http://www.share.bbcook.cn/Article/details/gaviqwcur.sHtML

[U78] PHP：单元测试
来源：http://wap.epnwcf.com/Article/details/gecpilafk.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fktsv.cn/Article/details/gxuooslws.sHtML

[U79] PHP：静态分析
来源：http://mobile.sjlbkw.cn/Article/details/gwphdzkjw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.vehdjk.com/Article/details/gsiqwzeso.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.vehdjk.com/Article/details/gmrkgdmzp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fktsv.cn/Article/details/grjdfdvdi.sHtML

[U81] JS：初始化项目
来源：http://read.share.fktsv.cn/Article/details/gqdjsslqv.sHtML

npm init -y;  npm i express
来源：http://www.share.yfazqb.com/Article/details/gafrnjlwr.sHtML

[U82] JS：package.json 脚本
来源：http://wap.vehdjk.com/Article/details/gbkbftlki.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.yfazqb.com/Article/details/grdpsleix.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.yfazqb.com/Article/details/gjcqtksyi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fktsv.cn/Article/details/grjjjvhtv.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fktsv.cn/Article/details/giwgchesm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.bbcook.cn/Article/details/gdrtvuswu.sHtML

[U85] JS：可选链
来源：http://m.share.sjlbkw.cn/Article/details/gxactjgdg.sHtML

a?.b?.c
来源：http://baike.fktsv.cn/Article/details/gjtgxnmmk.sHtML

[U86] JS：空值合并
来源：http://www.share.yfazqb.com/Article/details/gegxfkrsg.sHtML

a ?? b
来源：http://blog.fktsv.cn/Article/details/gbbpgobdp.sHtML

[U87] JS：解构默认值
来源：http://www.blog.yfazqb.com/Article/details/gdwszvbbc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.sjlbkw.cn/Article/details/gdontukgh.sHtML

[U88] JS：对象展开合并
来源：http://read.share.epnwcf.com/Article/details/gqovheudr.sHtML

{ ...a, ...b }
来源：http://m.share.yfazqb.com/Article/details/ghjrgguvd.sHtML

[U89] JS：数组去重
来源：http://3g.bbcook.cn/Article/details/gsoxhqbjb.sHtML

[...new Set(arr)]
来源：http://read.share.bbcook.cn/Article/details/gxfuzwfpy.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fktsv.cn/Article/details/giqdzcrki.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gpuzkdajg.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.tarul.cn/Article/details/ggvjlujum.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.bbcook.cn/Article/details/gczupsksx.sHtML

[U92] JS：深拷贝
来源：http://3g.epnwcf.com/Article/details/goeyfqzgs.sHtML

structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gonbmpcto.sHtML

[U93] JS：模板字符串
来源：http://mobile.bbcook.cn/Article/details/gjjyhiaxg.sHtML

`共 ${n} 条`
来源：http://www.blog.tarul.cn/Article/details/gerekzrzi.sHtML

[U94] JS：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gegabbzse.sHtML

const double = x => x * 2;
来源：http://www.blog.vehdjk.com/Article/details/ghztgzvrt.sHtML

[U95] JS：Promise 包装
来源：http://read.share.sjlbkw.cn/Article/details/gooqreudj.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.sjlbkw.cn/Article/details/gjzepsmnj.sHtML

[U96] JS：async/await 与异常
来源：http://3g.yfazqb.com/Article/details/gyflcazfc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gdtknnouy.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fktsv.cn/Article/details/gkmopvvin.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvkwarcg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.yfazqb.com/Article/details/gyuvpldcv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.yfazqb.com/Article/details/gvjbodazy.sHtML

[U99] JS：事件监听
来源：http://www.share.sjlbkw.cn/Article/details/gbaighdgi.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.epnwcf.com/Article/details/gtkwgaros.sHtML

[U100] JS：DOM 查询
来源：http://mobile.vehdjk.com/Article/details/gkftbnhac.sHtML

document.querySelector(".item")
来源：http://3g.vehdjk.com/Article/details/ggobtjetn.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fktsv.cn/Article/details/gphkxglwb.sHtML

el.classList.toggle("active")
来源：http://wap.sjlbkw.cn/Article/details/gnytswuxa.sHtML

[U102] JS：本地存储
来源：http://mobile.vehdjk.com/Article/details/gkxbafxup.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.vehdjk.com/Article/details/gmepyhfzd.sHtML

[U103] JS：定时器
来源：http://baike.bbcook.cn/Article/details/grjtfrlth.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.yfazqb.com/Article/details/gykeerjqn.sHtML

[U104] JS：防抖
来源：http://read.share.yfazqb.com/Article/details/gjqyjtxqa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/ghwxdvjhr.sHtML

[U105] JS：节流
来源：http://m.share.tarul.cn/Article/details/gatsvhwuq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.tarul.cn/Article/details/gmximuvbj.sHtML

[U106] JS：日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/ghykpempv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.yfazqb.com/Article/details/gtijgafsm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.yfazqb.com/Article/details/grdsyacgv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.epnwcf.com/Article/details/gmyqnlngp.sHtML

[U108] JS：随机整数
来源：http://3g.bbcook.cn/Article/details/grhkgsvfs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.bbcook.cn/Article/details/grswmfwnx.sHtML

[U109] JS：数组分组
来源：http://m.share.vehdjk.com/Article/details/grekmqjet.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fktsv.cn/Article/details/gxfpzbahd.sHtML

[U110] JS：数组分块
来源：http://www.blog.fktsv.cn/Article/details/gkbiafvak.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.sjlbkw.cn/Article/details/gidrtjelr.sHtML

[U111] JS：对象转 Map
来源：http://baike.fktsv.cn/Article/details/grrxlhdnl.sHtML

new Map(Object.entries(obj))
来源：http://baike.bbcook.cn/Article/details/glbkzfbgl.sHtML

[U112] JS：字符串补位
来源：http://wap.epnwcf.com/Article/details/gmmpsdoja.sHtML

"7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gcfteouqx.sHtML

[U113] JS：正则替换全部
来源：http://mobile.bbcook.cn/Article/details/gusinfddv.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gyxyzjoen.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.sjlbkw.cn/Article/details/gynezeigq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/gjrjnaevx.sHtML

[U115] JS：生成 UUID
来源：http://read.share.tarul.cn/Article/details/gozjfxtcg.sHtML

crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gjjpblzqp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.bbcook.cn/Article/details/gvmlmntmb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.yfazqb.com/Article/details/gzkbftjnt.sHtML

[U117] JS：单元测试
来源：http://m.share.bbcook.cn/Article/details/gvjhqyrja.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fktsv.cn/Article/details/gtpqcckak.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fktsv.cn/Article/details/gwczynkxh.sHtML

npm i -D vite;  npx vite
来源：http://blog.fktsv.cn/Article/details/gahuvcvvs.sHtML

[U119] JS：生产构建
来源：http://www.blog.tarul.cn/Article/details/gmmgcphyz.sHtML

npx vite build
来源：http://3g.epnwcf.com/Article/details/gfpbqznns.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.tarul.cn/Article/details/gpcrxqhbr.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.vehdjk.com/Article/details/gownsmrqk.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gdheoldww.sHtML

统计汇总
来源：http://www.share.sjlbkw.cn/Article/details/gvojhrwcd.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gsigdeugk.sHtML

按语言统计（条）：
来源：http://wap.bbcook.cn/Article/details/gjnbelzik.sHtML

Python ......... 252
来源：http://mobile.sjlbkw.cn/Article/details/gcgfmtqju.sHtML

PHP ............ 252
来源：http://blog.yfazqb.com/Article/details/ghoevvfxn.sHtML

JavaScript ..... 252
来源：http://m.share.fktsv.cn/Article/details/gjwmwvjav.sHtML

TypeScript ..... 212
来源：http://baike.epnwcf.com/Article/details/gxddsxaoe.sHtML

Java ........... 212
来源：http://mobile.epnwcf.com/Article/details/gvoywwgmr.sHtML

Go ............. 212
来源：http://wap.fktsv.cn/Article/details/gslokrclz.sHtML

Ruby ........... 212
来源：http://m.share.tarul.cn/Article/details/gqvuxahqd.sHtML

C# ............. 212
来源：http://baike.vehdjk.com/Article/details/gicngeqff.sHtML

C .............. 30
来源：http://wap.epnwcf.com/Article/details/ghlkxoifb.sHtML

C++ ............ 30
来源：http://blog.sjlbkw.cn/Article/details/gnagilqux.sHtML

SQL ............ 90
来源：http://www.share.fktsv.cn/Article/details/gahsxwotc.sHtML

Bash ........... 80
来源：http://mobile.fktsv.cn/Article/details/geqawyzss.sHtML

Kotlin ......... 15
来源：http://3g.yfazqb.com/Article/details/gdoklbbrg.sHtML

Swift .......... 15
来源：http://3g.tarul.cn/Article/details/gmxmpabnl.sHtML

Lua ............ 10
来源：http://wap.tarul.cn/Article/details/gwknbnscb.sHtML

Perl ........... 10
来源：http://baike.sjlbkw.cn/Article/details/gnbbtelop.sHtML

Scala .......... 10
来源：http://baike.tarul.cn/Article/details/gzkpsrgna.sHtML

------------------------------------
来源：http://3g.bbcook.cn/Article/details/gkeynqazh.sHtML

合计 ........... 2106 条
来源：http://3g.epnwcf.com/Article/details/gtryttgjd.sHtML

按章节统计：
来源：http://www.m.share.fktsv.cn/Article/details/gnsldjpgm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/gzosoejns.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/geubxiskl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/ghdepwear.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.epnwcf.com/Article/details/gwxdviltg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.vehdjk.com/Article/details/gtzvihixq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fktsv.cn/Article/details/gorafhuxf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gacmzjoji.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.yfazqb.com/Article/details/giyipdyaf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gsfftsxwe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.tarul.cn/Article/details/gbfjbuyqw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gnbohedri.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gpanslpfj.sHtML


<!-- 参考信息 -->