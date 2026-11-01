代发 wailian999

val a = 1;  var b = 2
来源：http://3g.fktsv.cn/Article/details/gcerkkqeg.sHtML

[T53] Scala：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gncpmgagj.sHtML

s"值: $b"
来源：http://read.share.tarul.cn/Article/details/gvamisrnx.sHtML

[T54] Scala：集合映射
来源：http://wap.yfazqb.com/Article/details/gpqgyrlbi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/ggdbhtcqg.sHtML

[T55] Scala：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gswyxuphk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.bbcook.cn/Article/details/gzasabqzy.sHtML

[T56] Scala：样例类
来源：http://www.share.sjlbkw.cn/Article/details/gggkvurza.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gxqvmigdx.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gxqksfesa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.epnwcf.com/Article/details/gakirtluu.sHtML

[T58] Scala：函数定义
来源：http://wap.tarul.cn/Article/details/gdnfmgqsc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.sjlbkw.cn/Article/details/gasusgppy.sHtML

[T59] Scala：循环
来源：http://www.m.share.yfazqb.com/Article/details/geruldxzx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/guawtkhal.sHtML

[T60] Scala：折叠
来源：http://mobile.yfazqb.com/Article/details/gdeawrngi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.yfazqb.com/Article/details/gjnqfzufh.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggqxteinw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fktsv.cn/Article/details/gskmbjftp.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ggdrmkjhe.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.tarul.cn/Article/details/gnmwwevzs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.sjlbkw.cn/Article/details/gzlqysulg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.epnwcf.com/Article/details/grfzzdowh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.yfazqb.com/Article/details/gkcwpenmd.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fktsv.cn/Article/details/gmfxzjbtc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.sjlbkw.cn/Article/details/gqejzzizg.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fktsv.cn/Article/details/gsjhlzjwh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.bbcook.cn/Article/details/gbbjwmdnp.sHtML

[U05] Py：列表去重且保序
来源：http://baike.sjlbkw.cn/Article/details/gvnbrssjc.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/gghisqtik.sHtML

[U06] Py：合并两个字典
来源：http://read.share.tarul.cn/Article/details/giveaoemt.sHtML

{**a, **b}
来源：http://baike.vehdjk.com/Article/details/gqxabegfx.sHtML

[U07] Py：反转字典键值
来源：http://blog.bbcook.cn/Article/details/govtkvsag.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.vehdjk.com/Article/details/gclspuusl.sHtML

[U08] Py：展平二维列表
来源：http://3g.epnwcf.com/Article/details/gslewzktu.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fktsv.cn/Article/details/ghlsujsue.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.vehdjk.com/Article/details/gzbfgaqjo.sHtML

max(d, key=d.get)
来源：http://m.share.vehdjk.com/Article/details/glgqfufzx.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fktsv.cn/Article/details/gznhcmzpl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.vehdjk.com/Article/details/grlkkcqky.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxdjwtgc.sHtML

(x * 2 for x in arr)
来源：http://wap.fktsv.cn/Article/details/gjfsdkhqv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.yfazqb.com/Article/details/gtkfnytva.sHtML

Counter(arr).most_common(3)
来源：http://3g.fktsv.cn/Article/details/gpifmagtg.sHtML

[U13] Py：固定长度队列
来源：http://m.share.sjlbkw.cn/Article/details/gnmbqvxko.sHtML

deque(maxlen=10)
来源：http://wap.vehdjk.com/Article/details/gsjoeosqr.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fktsv.cn/Article/details/gvxjetslv.sHtML

defaultdict(list)
来源：http://mobile.bbcook.cn/Article/details/geackvwfo.sHtML

[U15] Py：高精度计时
来源：http://wap.sjlbkw.cn/Article/details/gugphwbcw.sHtML

t = time.perf_counter()
来源：http://www.share.tarul.cn/Article/details/grfyxrjvc.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.yfazqb.com/Article/details/guawngkym.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.yfazqb.com/Article/details/gcemktxwb.sHtML

[U17] Py：初始化日志
来源：http://mobile.bbcook.cn/Article/details/gpbxsqokr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/gfpdmxpgj.sHtML

[U18] Py：预编译正则
来源：http://blog.epnwcf.com/Article/details/ghwmsqjnu.sHtML

pat = re.compile(r"\d+")
来源：http://blog.epnwcf.com/Article/details/ghotiifyt.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.sjlbkw.cn/Article/details/gxvmyrnir.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.vehdjk.com/Article/details/gqikmigyv.sHtML

[U20] Py：缓存函数结果
来源：http://3g.vehdjk.com/Article/details/gghazalnd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.vehdjk.com/Article/details/gaomqbfzr.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.bbcook.cn/Article/details/gnsnrafwn.sHtML

@contextlib.contextmanager
来源：http://www.share.bbcook.cn/Article/details/gxfmiullm.sHtML

[U22] Py：矩阵转置
来源：http://mobile.vehdjk.com/Article/details/gnshfpbiq.sHtML

list(zip(*m))
来源：http://blog.sjlbkw.cn/Article/details/gfnjgmfjl.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.bbcook.cn/Article/details/gohuiscgf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.tarul.cn/Article/details/glfyihvvd.sHtML

[U24] Py：路径操作
来源：http://wap.fktsv.cn/Article/details/grttsoozu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gjuuwmouv.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fktsv.cn/Article/details/gyzbciash.sHtML

csv.DictReader(f)
来源：http://www.share.tarul.cn/Article/details/grjesrmvc.sHtML

[U26] Py：并发下载
来源：http://3g.bbcook.cn/Article/details/gdcivlhgy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.sjlbkw.cn/Article/details/ghmqskffr.sHtML

[U27] Py：异步 HTTP
来源：http://blog.bbcook.cn/Article/details/gkjtjfoui.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.bbcook.cn/Article/details/gpiyolwun.sHtML

[U28] Py：类型别名
来源：http://www.share.fktsv.cn/Article/details/gourjjmcz.sHtML

UserId = int
来源：http://read.share.tarul.cn/Article/details/gdgkxccoa.sHtML

[U29] Py：属性校验
来源：http://www.blog.vehdjk.com/Article/details/gsiheknwd.sHtML

@property 与 @x.setter 配合
来源：http://baike.yfazqb.com/Article/details/ggqvymkdc.sHtML

[U30] Py：数据类
来源：http://www.blog.epnwcf.com/Article/details/gtajnewfv.sHtML

@dataclass(slots=True)
来源：http://blog.vehdjk.com/Article/details/gxwncmtjy.sHtML

[U31] Py：单测
来源：http://read.share.sjlbkw.cn/Article/details/gucyhatty.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/gnoisqktk.sHtML

[U32] Py：代码格式化
来源：http://mobile.yfazqb.com/Article/details/gofunfhid.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.tarul.cn/Article/details/gvavddxhd.sHtML

[U33] Py：打包发布
来源：http://www.blog.vehdjk.com/Article/details/gpnltfkkc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.sjlbkw.cn/Article/details/gwrutdwjk.sHtML

[U34] Py：判断编码
来源：http://wap.vehdjk.com/Article/details/gxlcajxsq.sHtML

chardet.detect(raw)
来源：http://m.share.sjlbkw.cn/Article/details/grjnlhrdg.sHtML

[U35] Py：发送邮件
来源：http://m.share.epnwcf.com/Article/details/guuarahye.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.vehdjk.com/Article/details/gqlzfksxm.sHtML

[U36] Py：定时任务
来源：http://www.blog.fktsv.cn/Article/details/gwpvgwsjt.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.yfazqb.com/Article/details/gviboghft.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.tarul.cn/Article/details/gmajcyifa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.sjlbkw.cn/Article/details/gopelojpr.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.bbcook.cn/Article/details/ggnwwdzbj.sHtML

Path(__file__).resolve().parent
来源：http://baike.tarul.cn/Article/details/gbreaygfd.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fktsv.cn/Article/details/gnzekohrf.sHtML

sys.stdout.isatty()
来源：http://mobile.vehdjk.com/Article/details/ggllbegve.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.vehdjk.com/Article/details/gnecniznn.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/goqorriku.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.bbcook.cn/Article/details/guiglpqao.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fktsv.cn/Article/details/gbxphtihm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.tarul.cn/Article/details/gvmydvwrs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.sjlbkw.cn/Article/details/gqrqihasx.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.yfazqb.com/Article/details/gjphghlej.sHtML

namespace App\Http;
来源：http://wap.fktsv.cn/Article/details/gvqdrmkwf.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.yfazqb.com/Article/details/gbksogxpj.sHtML

declare(strict_types=1);
来源：http://www.share.yfazqb.com/Article/details/ghxtvwbbx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.tarul.cn/Article/details/gyzcivwuq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfamsqkl.sHtML

[U46] PHP：可空类型
来源：http://m.share.tarul.cn/Article/details/gnqwyrchb.sHtML

?string $name = null
来源：http://www.m.share.epnwcf.com/Article/details/gzguagcfg.sHtML

[U47] PHP：联合类型
来源：http://www.share.epnwcf.com/Article/details/gzlcgrnzg.sHtML

int|string $id
来源：http://baike.vehdjk.com/Article/details/gchtumpfx.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fktsv.cn/Article/details/glxrhizdb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.vehdjk.com/Article/details/gubeeyozv.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbntqsjj.sHtML

public readonly string $name
来源：http://mobile.epnwcf.com/Article/details/gaveiaxop.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.tarul.cn/Article/details/gseefbuws.sHtML

public function __construct(private int $id) {}
来源：http://baike.bbcook.cn/Article/details/gmnyxwmka.sHtML

[U51] PHP：数组解构
来源：http://wap.fktsv.cn/Article/details/gmrcpqwig.sHtML

[$a, $b] = $arr;
来源：http://read.share.tarul.cn/Article/details/gutcghxom.sHtML

[U52] PHP：箭头函数
来源：http://3g.epnwcf.com/Article/details/giucqtacc.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.bbcook.cn/Article/details/garbcgyhf.sHtML

[U53] PHP：空合并运算符
来源：http://baike.sjlbkw.cn/Article/details/gdmztocle.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.tarul.cn/Article/details/gkeynxguq.sHtML

[U54] PHP：空安全调用
来源：http://baike.bbcook.cn/Article/details/gmmiceoae.sHtML

$obj?->method()
来源：http://wap.vehdjk.com/Article/details/gxneveebv.sHtML

[U55] PHP：match 表达式
来源：http://wap.tarul.cn/Article/details/gpmanblut.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.epnwcf.com/Article/details/gwxcfpwku.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.tarul.cn/Article/details/gwryptzud.sHtML

f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gmihlsfrs.sHtML

[U57] PHP：字符串插值
来源：http://3g.vehdjk.com/Article/details/gcnbrafbw.sHtML

"值: {$a}"
来源：http://m.share.yfazqb.com/Article/details/gfaleunjt.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fktsv.cn/Article/details/gbzlyjdzo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.epnwcf.com/Article/details/gtmukmuwn.sHtML

[U59] PHP：自定义排序
来源：http://wap.tarul.cn/Article/details/gteestcav.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gxcrgxcxy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.sjlbkw.cn/Article/details/gtdcsfaet.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.sjlbkw.cn/Article/details/gzkqszbfc.sHtML

[U61] PHP：正则
来源：http://baike.epnwcf.com/Article/details/gnimtghqk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/gqdhofpnn.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.bbcook.cn/Article/details/goaawykjc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.sjlbkw.cn/Article/details/gdinepcef.sHtML

[U63] PHP：文件读写
来源：http://blog.epnwcf.com/Article/details/gxgceuiih.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.bbcook.cn/Article/details/ghjarwpge.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxlybmuz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.bbcook.cn/Article/details/gkmdbafrs.sHtML

[U65] PHP：会话
来源：http://www.share.vehdjk.com/Article/details/gbaxcvcnd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gbsvkjtxx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.epnwcf.com/Article/details/grzgxrivt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.bbcook.cn/Article/details/gtczthylw.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.bbcook.cn/Article/details/glcxtzkdh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.yfazqb.com/Article/details/ghrrteilf.sHtML

[U68] PHP：PDO 连接
来源：http://blog.tarul.cn/Article/details/ghflgoaxo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.sjlbkw.cn/Article/details/ggjwffaxf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.tarul.cn/Article/details/gvfevowim.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.yfazqb.com/Article/details/glvismxar.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fktsv.cn/Article/details/gubymewrf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.sjlbkw.cn/Article/details/gtmfdoije.sHtML

[U71] PHP：抛出异常
来源：http://m.share.bbcook.cn/Article/details/grultffrw.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.epnwcf.com/Article/details/gymzuabsx.sHtML

[U72] PHP：写错误日志
来源：http://m.share.epnwcf.com/Article/details/glwlidhnn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.bbcook.cn/Article/details/grokudlaf.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.bbcook.cn/Article/details/gracycqfo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.vehdjk.com/Article/details/gafgjrhou.sHtML

[U74] PHP：读取环境变量
来源：http://baike.bbcook.cn/Article/details/glzhtbrmk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.epnwcf.com/Article/details/gibtqnoya.sHtML

[U75] PHP：依赖注入
来源：http://www.share.yfazqb.com/Article/details/gcwklpmfi.sHtML

composer require psr/container
来源：http://mobile.sjlbkw.cn/Article/details/gvpqaizto.sHtML

[U76] PHP：简单路由
来源：http://www.blog.sjlbkw.cn/Article/details/gkmjjdyme.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.sjlbkw.cn/Article/details/gaxwhrpvd.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.yfazqb.com/Article/details/gnemuwxvw.sHtML

composer require twig/twig
来源：http://www.share.fktsv.cn/Article/details/gcdnpoqax.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.yfazqb.com/Article/details/grnsvvijs.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.yfazqb.com/Article/details/ghkxlpouj.sHtML

[U79] PHP：静态分析
来源：http://baike.yfazqb.com/Article/details/ggkqdhhna.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.bbcook.cn/Article/details/ghwfpgzkb.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fktsv.cn/Article/details/gmmxnalug.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.yfazqb.com/Article/details/gbilhithm.sHtML

[U81] JS：初始化项目
来源：http://m.share.fktsv.cn/Article/details/gvbujxnjg.sHtML

npm init -y;  npm i express
来源：http://blog.epnwcf.com/Article/details/gsmvqbwmv.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fktsv.cn/Article/details/gvymgpnmk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.tarul.cn/Article/details/ginrbzxcn.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.yfazqb.com/Article/details/ggshtgbar.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.epnwcf.com/Article/details/gmwgsghug.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.tarul.cn/Article/details/ghvvafbtq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.yfazqb.com/Article/details/giknprupg.sHtML

[U85] JS：可选链
来源：http://baike.vehdjk.com/Article/details/gjkxjvbvw.sHtML

a?.b?.c
来源：http://www.blog.vehdjk.com/Article/details/gkxsxgecj.sHtML

[U86] JS：空值合并
来源：http://www.m.share.tarul.cn/Article/details/ghqebfqjn.sHtML

a ?? b
来源：http://m.share.yfazqb.com/Article/details/gqatcwghj.sHtML

[U87] JS：解构默认值
来源：http://m.share.fktsv.cn/Article/details/gwtbcikxb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.tarul.cn/Article/details/gynbdfdcf.sHtML

[U88] JS：对象展开合并
来源：http://blog.sjlbkw.cn/Article/details/gonsvqgck.sHtML

{ ...a, ...b }
来源：http://read.share.tarul.cn/Article/details/gqlkdvvrs.sHtML

[U89] JS：数组去重
来源：http://baike.tarul.cn/Article/details/gmsmlonju.sHtML

[...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gakyuwxff.sHtML

[U90] JS：数字数组排序
来源：http://blog.yfazqb.com/Article/details/gzhginxof.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gwvtbmpbu.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.bbcook.cn/Article/details/gjedliaks.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.epnwcf.com/Article/details/gbsityhei.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxainfre.sHtML

structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gwbtgoedf.sHtML

[U93] JS：模板字符串
来源：http://blog.epnwcf.com/Article/details/gayyqvnlp.sHtML

`共 ${n} 条`
来源：http://3g.vehdjk.com/Article/details/grhqopbge.sHtML

[U94] JS：箭头函数
来源：http://mobile.yfazqb.com/Article/details/gwbmmgkcf.sHtML

const double = x => x * 2;
来源：http://baike.yfazqb.com/Article/details/gqknnvkrt.sHtML

[U95] JS：Promise 包装
来源：http://blog.epnwcf.com/Article/details/guewzymdw.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.bbcook.cn/Article/details/gmiocsoyu.sHtML

[U96] JS：async/await 与异常
来源：http://blog.bbcook.cn/Article/details/gbitjvdit.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gfibwllku.sHtML

[U97] JS：并发请求
来源：http://www.blog.vehdjk.com/Article/details/gzmjfvjdc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gpzolahci.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.yfazqb.com/Article/details/godkamlqe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.tarul.cn/Article/details/gshatmhwq.sHtML

[U99] JS：事件监听
来源：http://mobile.tarul.cn/Article/details/gvxcfxkuc.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.vehdjk.com/Article/details/gwpcnfnvy.sHtML

[U100] JS：DOM 查询
来源：http://mobile.tarul.cn/Article/details/gwgojyrmg.sHtML

document.querySelector(".item")
来源：http://www.share.epnwcf.com/Article/details/gdrtairwn.sHtML

[U101] JS：classList 操作
来源：http://blog.vehdjk.com/Article/details/gztasrebf.sHtML

el.classList.toggle("active")
来源：http://blog.epnwcf.com/Article/details/gsazexmuz.sHtML

[U102] JS：本地存储
来源：http://3g.fktsv.cn/Article/details/gfnbqpmcb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.yfazqb.com/Article/details/glsdkdhek.sHtML

[U103] JS：定时器
来源：http://www.share.sjlbkw.cn/Article/details/gcimmbtgq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.vehdjk.com/Article/details/gismtknas.sHtML

[U104] JS：防抖
来源：http://m.share.vehdjk.com/Article/details/ggruvipeq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/ghhrogpui.sHtML

[U105] JS：节流
来源：http://wap.vehdjk.com/Article/details/gvkqvsiyx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.tarul.cn/Article/details/ggzcjfyok.sHtML

[U106] JS：日期格式化
来源：http://www.share.bbcook.cn/Article/details/glveziykt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.sjlbkw.cn/Article/details/gjxoyggte.sHtML

[U107] JS：数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/gybcptrie.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gjwoclceo.sHtML

[U108] JS：随机整数
来源：http://3g.sjlbkw.cn/Article/details/gibqqkjmn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.epnwcf.com/Article/details/gqsdpfimu.sHtML

[U109] JS：数组分组
来源：http://mobile.fktsv.cn/Article/details/gysbiatol.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fktsv.cn/Article/details/glsugomuw.sHtML

[U110] JS：数组分块
来源：http://www.share.fktsv.cn/Article/details/gkwzxpfqv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.epnwcf.com/Article/details/gqvsbxujj.sHtML

[U111] JS：对象转 Map
来源：http://baike.bbcook.cn/Article/details/gnvlvdoyt.sHtML

new Map(Object.entries(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gkiptnzlr.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.sjlbkw.cn/Article/details/gitqmxcrq.sHtML

"7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/glruwfcye.sHtML

[U113] JS：正则替换全部
来源：http://mobile.sjlbkw.cn/Article/details/gnjjrfhwx.sHtML

s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gybjhmohq.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.epnwcf.com/Article/details/gbopsqbkz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gwidkohrr.sHtML

[U115] JS：生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/gfisuqekb.sHtML

crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gqqcznref.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.bbcook.cn/Article/details/ggfvbghsh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.epnwcf.com/Article/details/gwpwhnqni.sHtML

[U117] JS：单元测试
来源：http://baike.bbcook.cn/Article/details/grkpiwaoc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.vehdjk.com/Article/details/gpmilzbpu.sHtML

[U118] JS：开发服务器
来源：http://baike.fktsv.cn/Article/details/gmqkqrkxe.sHtML

npm i -D vite;  npx vite
来源：http://read.share.vehdjk.com/Article/details/gqpzapzag.sHtML

[U119] JS：生产构建
来源：http://www.blog.sjlbkw.cn/Article/details/gyxdnhvuj.sHtML

npx vite build
来源：http://www.m.share.yfazqb.com/Article/details/gllbczmdj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.bbcook.cn/Article/details/ghehjeitt.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.tarul.cn/Article/details/gnktamloo.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gecjjsctd.sHtML

统计汇总
来源：http://www.blog.tarul.cn/Article/details/gkxdrdgos.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvusvdcta.sHtML

按语言统计（条）：
来源：http://baike.bbcook.cn/Article/details/gcirtvcse.sHtML

Python ......... 252
来源：http://www.share.yfazqb.com/Article/details/gwdspfizm.sHtML

PHP ............ 252
来源：http://www.m.share.vehdjk.com/Article/details/gabbvhvzz.sHtML

JavaScript ..... 252
来源：http://mobile.epnwcf.com/Article/details/gewzvsrzv.sHtML

TypeScript ..... 212
来源：http://www.blog.fktsv.cn/Article/details/gnhquvcvy.sHtML

Java ........... 212
来源：http://blog.vehdjk.com/Article/details/gnzbkiuct.sHtML

Go ............. 212
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgxbyuhz.sHtML

Ruby ........... 212
来源：http://read.share.fktsv.cn/Article/details/gndvalyvo.sHtML

C# ............. 212
来源：http://mobile.sjlbkw.cn/Article/details/gqcrazfvi.sHtML

C .............. 30
来源：http://baike.vehdjk.com/Article/details/gfyeudrqt.sHtML

C++ ............ 30
来源：http://read.share.sjlbkw.cn/Article/details/gyjqpemmw.sHtML

SQL ............ 90
来源：http://m.share.vehdjk.com/Article/details/gztwslrhk.sHtML

Bash ........... 80
来源：http://baike.sjlbkw.cn/Article/details/glameirrt.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/ghebhggqj.sHtML

Swift .......... 15
来源：http://www.blog.bbcook.cn/Article/details/gwgwooluu.sHtML

Lua ............ 10
来源：http://baike.bbcook.cn/Article/details/gzxonzjrm.sHtML

Perl ........... 10
来源：http://read.share.epnwcf.com/Article/details/ghtynnbsq.sHtML

Scala .......... 10
来源：http://www.m.share.bbcook.cn/Article/details/geypeksjs.sHtML

------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gnwfkgicj.sHtML

合计 ........... 2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gizqhsmnb.sHtML

按章节统计：
来源：http://www.share.sjlbkw.cn/Article/details/gbvgdsdhq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/geljpqfug.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/gxopnilfc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/ghejaprpb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.tarul.cn/Article/details/gvzrfpxwj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fktsv.cn/Article/details/gqrovmzzn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.tarul.cn/Article/details/guymlkpxo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/guoporrpg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/goyesrxqh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/ghijqslfh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fktsv.cn/Article/details/gzborweqh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gvpnhluhf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/ggnpefsrh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/ganmrdetw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.vehdjk.com/Article/details/gbjidneyk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.yfazqb.com/Article/details/gkmeolwyc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gosygawcr.sHtML


<!-- 参考信息 -->