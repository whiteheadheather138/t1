代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://3g.tarul.cn/Article/details/gkpvkfbue.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gaetumzjg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.sjlbkw.cn/Article/details/gvgmrppqi.sHtML

[T56] Scala：样例类
来源：http://m.share.sjlbkw.cn/Article/details/gxewwvynf.sHtML

case class User(name: String, age: Int)
来源：http://3g.tarul.cn/Article/details/gatzlrsnc.sHtML

[T57] Scala：模式匹配
来源：http://3g.bbcook.cn/Article/details/gstykbdza.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.sjlbkw.cn/Article/details/grmtyqdqq.sHtML

[T58] Scala：函数定义
来源：http://wap.sjlbkw.cn/Article/details/gdwakwnnp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.vehdjk.com/Article/details/gwyajrdda.sHtML

[T59] Scala：循环
来源：http://3g.yfazqb.com/Article/details/gjjkfyzgm.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.vehdjk.com/Article/details/gnnxmxgdf.sHtML

[T60] Scala：折叠
来源：http://wap.epnwcf.com/Article/details/gbffqqgks.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/gatjrdazr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfwvkwpef.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.epnwcf.com/Article/details/gjxuhqjai.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gexrfhpxr.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.vehdjk.com/Article/details/gkhcslhtz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.sjlbkw.cn/Article/details/gxmprdodi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/gztgdixwc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.tarul.cn/Article/details/ggdfidbxd.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.bbcook.cn/Article/details/gffrbraby.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.yfazqb.com/Article/details/gfypndkhs.sHtML

[U04] Py：变量调试打印
来源：http://mobile.bbcook.cn/Article/details/gxcawakfv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.tarul.cn/Article/details/gesihhhch.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.bbcook.cn/Article/details/gzsilibpq.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fktsv.cn/Article/details/geoqbizyd.sHtML

[U06] Py：合并两个字典
来源：http://m.share.vehdjk.com/Article/details/gklwywzzb.sHtML

{**a, **b}
来源：http://mobile.yfazqb.com/Article/details/gmapnatov.sHtML

[U07] Py：反转字典键值
来源：http://mobile.sjlbkw.cn/Article/details/gkklrdyfr.sHtML

{v: k for k, v in d.items()}
来源：http://blog.tarul.cn/Article/details/gvnwtxcju.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fktsv.cn/Article/details/ginurdemy.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.bbcook.cn/Article/details/gzwvzkuwa.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.sjlbkw.cn/Article/details/gsheqdzcx.sHtML

max(d, key=d.get)
来源：http://www.share.epnwcf.com/Article/details/gizysyhde.sHtML

[U10] Py：按值排序字典
来源：http://www.share.bbcook.cn/Article/details/gdmadwfcx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fktsv.cn/Article/details/gcdwivrwb.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.tarul.cn/Article/details/grmrjeqrm.sHtML

(x * 2 for x in arr)
来源：http://blog.bbcook.cn/Article/details/gqezjhypp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/gtflmdwmm.sHtML

Counter(arr).most_common(3)
来源：http://read.share.sjlbkw.cn/Article/details/gguipctmn.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.bbcook.cn/Article/details/gnadwoswn.sHtML

deque(maxlen=10)
来源：http://3g.fktsv.cn/Article/details/gtbtwurom.sHtML

[U14] Py：分组收集到列表
来源：http://wap.bbcook.cn/Article/details/gnfmnqguy.sHtML

defaultdict(list)
来源：http://www.m.share.bbcook.cn/Article/details/gdhlkbvtk.sHtML

[U15] Py：高精度计时
来源：http://wap.epnwcf.com/Article/details/gzqaoodcj.sHtML

t = time.perf_counter()
来源：http://blog.bbcook.cn/Article/details/gwwufulcq.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.tarul.cn/Article/details/gtrqnhbqf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.yfazqb.com/Article/details/gmztrlvpr.sHtML

[U17] Py：初始化日志
来源：http://wap.bbcook.cn/Article/details/grrfjpdny.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.vehdjk.com/Article/details/gaibhbsjh.sHtML

[U18] Py：预编译正则
来源：http://read.share.bbcook.cn/Article/details/gqmndbhjz.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/gyqwhljev.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fktsv.cn/Article/details/gxlgrkxme.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.vehdjk.com/Article/details/girvunuon.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.epnwcf.com/Article/details/ghmvqtjgf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.sjlbkw.cn/Article/details/ghbwtcpeh.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.tarul.cn/Article/details/gdnapmmue.sHtML

@contextlib.contextmanager
来源：http://www.share.fktsv.cn/Article/details/gsuwupgsb.sHtML

[U22] Py：矩阵转置
来源：http://baike.bbcook.cn/Article/details/gvleshbuc.sHtML

list(zip(*m))
来源：http://baike.tarul.cn/Article/details/gsoazprop.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.sjlbkw.cn/Article/details/gqryhjsvx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.bbcook.cn/Article/details/gmldyyqiy.sHtML

[U24] Py：路径操作
来源：http://mobile.tarul.cn/Article/details/guqggcdpb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.yfazqb.com/Article/details/gepweuviq.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.tarul.cn/Article/details/guxcakpbw.sHtML

csv.DictReader(f)
来源：http://baike.vehdjk.com/Article/details/gleydhumn.sHtML

[U26] Py：并发下载
来源：http://www.share.sjlbkw.cn/Article/details/gjchojqyg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.tarul.cn/Article/details/gibmsqpnt.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.bbcook.cn/Article/details/gkkplbbma.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.yfazqb.com/Article/details/geufetmjb.sHtML

[U28] Py：类型别名
来源：http://www.m.share.bbcook.cn/Article/details/gtgasgcdg.sHtML

UserId = int
来源：http://blog.vehdjk.com/Article/details/gqmwphkxb.sHtML

[U29] Py：属性校验
来源：http://www.blog.fktsv.cn/Article/details/gnniqxrmn.sHtML

@property 与 @x.setter 配合
来源：http://www.share.tarul.cn/Article/details/gqciytkie.sHtML

[U30] Py：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gaekdcqyx.sHtML

@dataclass(slots=True)
来源：http://3g.vehdjk.com/Article/details/gazdxjfec.sHtML

[U31] Py：单测
来源：http://www.share.tarul.cn/Article/details/gjwohdori.sHtML

python -m pytest -q
来源：http://wap.vehdjk.com/Article/details/giikiffta.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/glfrifuzo.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.yfazqb.com/Article/details/gucpgezqn.sHtML

[U33] Py：打包发布
来源：http://wap.yfazqb.com/Article/details/gientjrzm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.sjlbkw.cn/Article/details/glnbogmky.sHtML

[U34] Py：判断编码
来源：http://read.share.epnwcf.com/Article/details/gedtaywfb.sHtML

chardet.detect(raw)
来源：http://3g.epnwcf.com/Article/details/gzishbpkg.sHtML

[U35] Py：发送邮件
来源：http://www.share.sjlbkw.cn/Article/details/gufabbqto.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.epnwcf.com/Article/details/goesnkvym.sHtML

[U36] Py：定时任务
来源：http://3g.vehdjk.com/Article/details/gsecybzov.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.sjlbkw.cn/Article/details/gkpaqmccb.sHtML

[U37] Py：读写 Excel
来源：http://blog.fktsv.cn/Article/details/goeywcrff.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.epnwcf.com/Article/details/gxuuopswk.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.sjlbkw.cn/Article/details/gkecehwdz.sHtML

Path(__file__).resolve().parent
来源：http://wap.yfazqb.com/Article/details/gzajduolp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fktsv.cn/Article/details/gikoqxtbs.sHtML

sys.stdout.isatty()
来源：http://3g.sjlbkw.cn/Article/details/gkpxuwhzb.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fktsv.cn/Article/details/gapawywmq.sHtML

print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/gtxyltqoe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.epnwcf.com/Article/details/gdkoljplw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.vehdjk.com/Article/details/gteexqpze.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.sjlbkw.cn/Article/details/gxqhkbjot.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fktsv.cn/Article/details/gixcufisi.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.bbcook.cn/Article/details/gqevbnwdi.sHtML

namespace App\Http;
来源：http://m.share.epnwcf.com/Article/details/gwmhylsnh.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.tarul.cn/Article/details/gjrjgwviv.sHtML

declare(strict_types=1);
来源：http://3g.sjlbkw.cn/Article/details/ggohardwv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.bbcook.cn/Article/details/ghxkfaegv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gphcljhmy.sHtML

[U46] PHP：可空类型
来源：http://3g.sjlbkw.cn/Article/details/ggpevozah.sHtML

?string $name = null
来源：http://wap.sjlbkw.cn/Article/details/ggekqhinw.sHtML

[U47] PHP：联合类型
来源：http://baike.bbcook.cn/Article/details/gyjupforv.sHtML

int|string $id
来源：http://wap.tarul.cn/Article/details/gevnvfpjn.sHtML

[U48] PHP：纯枚举
来源：http://mobile.bbcook.cn/Article/details/gbrrhmyhm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.yfazqb.com/Article/details/gbhkgfhqu.sHtML

[U49] PHP：只读属性
来源：http://blog.sjlbkw.cn/Article/details/gocrmczoh.sHtML

public readonly string $name
来源：http://www.m.share.epnwcf.com/Article/details/glucfaopu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.yfazqb.com/Article/details/gteprmrnu.sHtML

public function __construct(private int $id) {}
来源：http://wap.sjlbkw.cn/Article/details/gfvaiqfao.sHtML

[U51] PHP：数组解构
来源：http://read.share.epnwcf.com/Article/details/giqtlffcs.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.epnwcf.com/Article/details/gshbutwxp.sHtML

[U52] PHP：箭头函数
来源：http://mobile.vehdjk.com/Article/details/gwxqltdiu.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.epnwcf.com/Article/details/gxthqkoiw.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fktsv.cn/Article/details/gdkyfcjap.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.yfazqb.com/Article/details/ghzddzgti.sHtML

[U54] PHP：空安全调用
来源：http://3g.fktsv.cn/Article/details/ghdftvyzx.sHtML

$obj?->method()
来源：http://mobile.sjlbkw.cn/Article/details/ggxfqyigr.sHtML

[U55] PHP：match 表达式
来源：http://wap.vehdjk.com/Article/details/gohnhaofk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gjjtemdhu.sHtML

[U56] PHP：命名参数
来源：http://blog.tarul.cn/Article/details/gomqtaxmk.sHtML

f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/gxmkivple.sHtML

[U57] PHP：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gldigwmta.sHtML

"值: {$a}"
来源：http://read.share.epnwcf.com/Article/details/gqrcmxacw.sHtML

[U58] PHP：数组三件套
来源：http://3g.vehdjk.com/Article/details/ghfvfmgae.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.epnwcf.com/Article/details/geaettlla.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.bbcook.cn/Article/details/gkvmpilef.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gsmtcbndz.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.epnwcf.com/Article/details/gvielywxy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.bbcook.cn/Article/details/gdtktzugo.sHtML

[U61] PHP：正则
来源：http://baike.tarul.cn/Article/details/gcdjcjunl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gmltcpthc.sHtML

[U62] PHP：日期对象
来源：http://www.share.tarul.cn/Article/details/getnchcqx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.vehdjk.com/Article/details/gdpjdkrfs.sHtML

[U63] PHP：文件读写
来源：http://mobile.yfazqb.com/Article/details/gynalntih.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.epnwcf.com/Article/details/gtgjjlbsy.sHtML

[U64] PHP：目录遍历
来源：http://mobile.tarul.cn/Article/details/goxriumjw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.yfazqb.com/Article/details/gpxuwbavf.sHtML

[U65] PHP：会话
来源：http://baike.bbcook.cn/Article/details/guqnwjzco.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gnsmpolua.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fktsv.cn/Article/details/ggygptgup.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.yfazqb.com/Article/details/gdspbiuxq.sHtML

[U67] PHP：处理文件上传
来源：http://blog.sjlbkw.cn/Article/details/gmiinnyfj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.bbcook.cn/Article/details/gxqmvlays.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.vehdjk.com/Article/details/gxzhtlpxo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.bbcook.cn/Article/details/gzuchnzpb.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fktsv.cn/Article/details/gjfmblrwg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.epnwcf.com/Article/details/gcgiicggk.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.sjlbkw.cn/Article/details/gkxmewjls.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.bbcook.cn/Article/details/gtlvyaenz.sHtML

[U71] PHP：抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gebgrumbv.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.vehdjk.com/Article/details/gpolzeghk.sHtML

[U72] PHP：写错误日志
来源：http://read.share.tarul.cn/Article/details/gpgoaqgdz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.bbcook.cn/Article/details/ghngibsux.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.yfazqb.com/Article/details/gllsnties.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.tarul.cn/Article/details/gpgautxip.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.epnwcf.com/Article/details/gnxdlujzw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.tarul.cn/Article/details/gbnxvgwdv.sHtML

[U75] PHP：依赖注入
来源：http://blog.yfazqb.com/Article/details/gfbslsvbf.sHtML

composer require psr/container
来源：http://read.share.yfazqb.com/Article/details/gutokwszr.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/gnicmuroz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.tarul.cn/Article/details/gpmmlvzdu.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.sjlbkw.cn/Article/details/gyftuvude.sHtML

composer require twig/twig
来源：http://blog.epnwcf.com/Article/details/gbsimsppd.sHtML

[U78] PHP：单元测试
来源：http://www.share.yfazqb.com/Article/details/gytmxavsk.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.tarul.cn/Article/details/gyrhbiybn.sHtML

[U79] PHP：静态分析
来源：http://read.share.epnwcf.com/Article/details/gyhnevlgj.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.epnwcf.com/Article/details/geehmaire.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.sjlbkw.cn/Article/details/gqdmdjawk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.bbcook.cn/Article/details/gkooiatrp.sHtML

[U81] JS：初始化项目
来源：http://wap.bbcook.cn/Article/details/gnqylnffq.sHtML

npm init -y;  npm i express
来源：http://m.share.tarul.cn/Article/details/gqxmqxejt.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fktsv.cn/Article/details/gzuwnlcox.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.bbcook.cn/Article/details/gkujcjyud.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.sjlbkw.cn/Article/details/gdfpldaly.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.epnwcf.com/Article/details/gejitrrek.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.epnwcf.com/Article/details/gngkjsmvy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.tarul.cn/Article/details/gilniduur.sHtML

[U85] JS：可选链
来源：http://baike.epnwcf.com/Article/details/gnnjvxitv.sHtML

a?.b?.c
来源：http://baike.vehdjk.com/Article/details/ggvegkris.sHtML

[U86] JS：空值合并
来源：http://m.share.bbcook.cn/Article/details/gnlxmefao.sHtML

a ?? b
来源：http://www.share.bbcook.cn/Article/details/gczshamng.sHtML

[U87] JS：解构默认值
来源：http://www.share.vehdjk.com/Article/details/glgedhdli.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.sjlbkw.cn/Article/details/gvkzlghqt.sHtML

[U88] JS：对象展开合并
来源：http://3g.tarul.cn/Article/details/gueqogizl.sHtML

{ ...a, ...b }
来源：http://www.m.share.epnwcf.com/Article/details/glwcgtnhw.sHtML

[U89] JS：数组去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gsttljlac.sHtML

[...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gwqacnrdg.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.yfazqb.com/Article/details/gjeakvlsv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gfxmyaslm.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.epnwcf.com/Article/details/ghcugskku.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.sjlbkw.cn/Article/details/gbpehlrzc.sHtML

[U92] JS：深拷贝
来源：http://blog.tarul.cn/Article/details/gvckjyumh.sHtML

structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/ggtdopeur.sHtML

[U93] JS：模板字符串
来源：http://www.blog.tarul.cn/Article/details/grlybdbtj.sHtML

`共 ${n} 条`
来源：http://baike.sjlbkw.cn/Article/details/gvopacuny.sHtML

[U94] JS：箭头函数
来源：http://3g.bbcook.cn/Article/details/ggyywidjo.sHtML

const double = x => x * 2;
来源：http://www.share.sjlbkw.cn/Article/details/gbfhqldsy.sHtML

[U95] JS：Promise 包装
来源：http://m.share.yfazqb.com/Article/details/gnirfjobh.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.bbcook.cn/Article/details/gvbgrrxlx.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.bbcook.cn/Article/details/gqymyguqg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/ggawuhjpf.sHtML

[U97] JS：并发请求
来源：http://read.share.sjlbkw.cn/Article/details/gqtsincmr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/grpkdjwff.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.yfazqb.com/Article/details/gacmerhgd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.vehdjk.com/Article/details/gfjhtkkvy.sHtML

[U99] JS：事件监听
来源：http://m.share.sjlbkw.cn/Article/details/guwlfkjex.sHtML

el.addEventListener("click", e => {})
来源：http://3g.vehdjk.com/Article/details/gtavxvaaf.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.bbcook.cn/Article/details/gswjmwaus.sHtML

document.querySelector(".item")
来源：http://wap.tarul.cn/Article/details/godzffcpd.sHtML

[U101] JS：classList 操作
来源：http://wap.tarul.cn/Article/details/gytehhbkf.sHtML

el.classList.toggle("active")
来源：http://baike.epnwcf.com/Article/details/gsfhqpmhe.sHtML

[U102] JS：本地存储
来源：http://read.share.sjlbkw.cn/Article/details/gjygyvpfj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.bbcook.cn/Article/details/gstsgbywk.sHtML

[U103] JS：定时器
来源：http://m.share.vehdjk.com/Article/details/ghnleduni.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.vehdjk.com/Article/details/gfncyegkr.sHtML

[U104] JS：防抖
来源：http://www.blog.yfazqb.com/Article/details/gmphrnmns.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gppxizafi.sHtML

[U105] JS：节流
来源：http://3g.epnwcf.com/Article/details/gakwfbykp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.epnwcf.com/Article/details/gflhjvrxa.sHtML

[U106] JS：日期格式化
来源：http://m.share.yfazqb.com/Article/details/geeqhjmdx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fktsv.cn/Article/details/gnfldbork.sHtML

[U107] JS：数字千分位
来源：http://mobile.tarul.cn/Article/details/gztmqlxru.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fktsv.cn/Article/details/gcubbzlym.sHtML

[U108] JS：随机整数
来源：http://m.share.yfazqb.com/Article/details/gibrwefrm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.bbcook.cn/Article/details/gzdrotifx.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fktsv.cn/Article/details/gulpsgict.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gnjxedsez.sHtML

[U110] JS：数组分块
来源：http://www.blog.bbcook.cn/Article/details/gvhslzbus.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.yfazqb.com/Article/details/guybgittj.sHtML

[U111] JS：对象转 Map
来源：http://www.share.sjlbkw.cn/Article/details/glcnaoowk.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.epnwcf.com/Article/details/gqjhfnafu.sHtML

[U112] JS：字符串补位
来源：http://read.share.bbcook.cn/Article/details/gbujnyayj.sHtML

"7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gxziqleqv.sHtML

[U113] JS：正则替换全部
来源：http://read.share.bbcook.cn/Article/details/gupaqnocz.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gigiwxeqt.sHtML

[U114] JS：JSON 深比较
来源：http://wap.vehdjk.com/Article/details/gyrwjfrrm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.yfazqb.com/Article/details/gmtxitnyh.sHtML

[U115] JS：生成 UUID
来源：http://mobile.tarul.cn/Article/details/gntmqwikl.sHtML

crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gmgadtadj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fktsv.cn/Article/details/ghjdacbab.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gmgrvdcpx.sHtML

[U117] JS：单元测试
来源：http://wap.bbcook.cn/Article/details/gwwnjhjpf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fktsv.cn/Article/details/garhloynp.sHtML

[U118] JS：开发服务器
来源：http://mobile.vehdjk.com/Article/details/gflbmlayo.sHtML

npm i -D vite;  npx vite
来源：http://3g.bbcook.cn/Article/details/gzywokphc.sHtML

[U119] JS：生产构建
来源：http://wap.sjlbkw.cn/Article/details/gfsasyhve.sHtML

npx vite build
来源：http://baike.tarul.cn/Article/details/gnsabwogl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.yfazqb.com/Article/details/gmdvmgkkt.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.vehdjk.com/Article/details/gfivcxscg.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ggojubksy.sHtML

统计汇总
来源：http://read.share.tarul.cn/Article/details/gcjwkguia.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ggfzlibpb.sHtML

按语言统计（条）：
来源：http://3g.fktsv.cn/Article/details/guvymprqb.sHtML

Python ......... 252
来源：http://blog.sjlbkw.cn/Article/details/gwnspdvzi.sHtML

PHP ............ 252
来源：http://www.blog.bbcook.cn/Article/details/ghntdusvt.sHtML

JavaScript ..... 252
来源：http://read.share.vehdjk.com/Article/details/gyrucjhld.sHtML

TypeScript ..... 212
来源：http://baike.epnwcf.com/Article/details/gbxlqyhkx.sHtML

Java ........... 212
来源：http://mobile.yfazqb.com/Article/details/ghnxmodzn.sHtML

Go ............. 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfxhnsmh.sHtML

Ruby ........... 212
来源：http://www.m.share.epnwcf.com/Article/details/gdwbzbmvf.sHtML

C# ............. 212
来源：http://blog.yfazqb.com/Article/details/gvftrdtlu.sHtML

C .............. 30
来源：http://www.blog.sjlbkw.cn/Article/details/guwxmjekr.sHtML

C++ ............ 30
来源：http://read.share.bbcook.cn/Article/details/gaeeepuid.sHtML

SQL ............ 90
来源：http://3g.tarul.cn/Article/details/gjmvefwmk.sHtML

Bash ........... 80
来源：http://www.m.share.vehdjk.com/Article/details/gclwzakhn.sHtML

Kotlin ......... 15
来源：http://mobile.epnwcf.com/Article/details/gwuagnvrp.sHtML

Swift .......... 15
来源：http://wap.sjlbkw.cn/Article/details/gtjwieitm.sHtML

Lua ............ 10
来源：http://m.share.tarul.cn/Article/details/gxcgiohre.sHtML

Perl ........... 10
来源：http://3g.vehdjk.com/Article/details/gooiuhnps.sHtML

Scala .......... 10
来源：http://blog.yfazqb.com/Article/details/gxavxjqax.sHtML

------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gdtlxyepm.sHtML

合计 ........... 2106 条
来源：http://www.m.share.tarul.cn/Article/details/gctunnrld.sHtML

按章节统计：
来源：http://baike.tarul.cn/Article/details/gkifzhcpp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.vehdjk.com/Article/details/gbtgnkstz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/gfumtdmig.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gjrlyxlyp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.yfazqb.com/Article/details/gvwipgzjw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fktsv.cn/Article/details/gwjwqmkqp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/glqolmogg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/ghqbfypkr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.tarul.cn/Article/details/gkzapmubg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gvuhdqrwl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.epnwcf.com/Article/details/gzhjrdfre.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gfihyjosq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gjycpnzoe.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gqgwetluq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/gysnxdtsq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fktsv.cn/Article/details/glwxfzpqi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gkztwpjam.sHtML

Q SQL 专题                              90
来源：http://3g.bbcook.cn/Article/details/gavrpgqnt.sHtML

R Bash 专题                             80
来源：http://mobile.fktsv.cn/Article/details/gtrjwubzi.sHtML

S C / C++ 专题                          60
来源：http://3g.epnwcf.com/Article/details/grqwfjnrj.sHtML

T 其他语言补充                          60
来源：http://baike.fktsv.cn/Article/details/grpejxcki.sHtML


<!-- 参考信息 -->