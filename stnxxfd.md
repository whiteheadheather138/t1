代发 wailian999

case class User(name: String, age: Int)
来源：http://read.share.yfazqb.com/Article/details/gprqjfxib.sHtML

[T57] Scala：模式匹配
来源：http://www.share.tarul.cn/Article/details/ggkqatfzu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.vehdjk.com/Article/details/gdrpgnvrq.sHtML

[T58] Scala：函数定义
来源：http://www.share.fktsv.cn/Article/details/gdakrkfdz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.yfazqb.com/Article/details/ggzivgxma.sHtML

[T59] Scala：循环
来源：http://mobile.sjlbkw.cn/Article/details/gzaywhgmg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gjdzxwond.sHtML

[T60] Scala：折叠
来源：http://read.share.epnwcf.com/Article/details/gqplltzlu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.bbcook.cn/Article/details/grhifklme.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gbshxubaq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/gzrrmrhiv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gizvpulek.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.bbcook.cn/Article/details/ggforzqun.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.bbcook.cn/Article/details/goraccddt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.epnwcf.com/Article/details/gnhvfgvnc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.sjlbkw.cn/Article/details/gighuctzc.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.bbcook.cn/Article/details/gtwxszdrc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.sjlbkw.cn/Article/details/gwjurgaeh.sHtML

[U04] Py：变量调试打印
来源：http://m.share.vehdjk.com/Article/details/gtabzfztl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fktsv.cn/Article/details/ggsskhxuc.sHtML

[U05] Py：列表去重且保序
来源：http://wap.yfazqb.com/Article/details/gwxdklhmc.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/grzhbelse.sHtML

[U06] Py：合并两个字典
来源：http://www.share.tarul.cn/Article/details/guffcdtei.sHtML

{**a, **b}
来源：http://www.share.tarul.cn/Article/details/ghjwkgyde.sHtML

[U07] Py：反转字典键值
来源：http://3g.bbcook.cn/Article/details/gcbgchwno.sHtML

{v: k for k, v in d.items()}
来源：http://baike.yfazqb.com/Article/details/gxenkzycy.sHtML

[U08] Py：展平二维列表
来源：http://wap.tarul.cn/Article/details/grsltlyui.sHtML

[y for x in nested for y in x]
来源：http://www.share.bbcook.cn/Article/details/gabqtulgb.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.yfazqb.com/Article/details/gfkreibqc.sHtML

max(d, key=d.get)
来源：http://blog.fktsv.cn/Article/details/gtxunplbr.sHtML

[U10] Py：按值排序字典
来源：http://www.share.epnwcf.com/Article/details/gtpabysvn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.epnwcf.com/Article/details/gpxyczwxx.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gavygubsc.sHtML

(x * 2 for x in arr)
来源：http://wap.fktsv.cn/Article/details/gxkcmfuyt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.tarul.cn/Article/details/gdktxawsw.sHtML

Counter(arr).most_common(3)
来源：http://3g.epnwcf.com/Article/details/gqkulldgi.sHtML

[U13] Py：固定长度队列
来源：http://baike.vehdjk.com/Article/details/gkiqounll.sHtML

deque(maxlen=10)
来源：http://www.m.share.vehdjk.com/Article/details/gbttfkowa.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.sjlbkw.cn/Article/details/ghhstpisj.sHtML

defaultdict(list)
来源：http://www.share.sjlbkw.cn/Article/details/gcyvvzfyd.sHtML

[U15] Py：高精度计时
来源：http://blog.vehdjk.com/Article/details/gtxgkctpx.sHtML

t = time.perf_counter()
来源：http://m.share.tarul.cn/Article/details/glhhibobv.sHtML

[U16] Py：命令行参数解析
来源：http://blog.yfazqb.com/Article/details/ggvlzbhsw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.tarul.cn/Article/details/gcpoxoesn.sHtML

[U17] Py：初始化日志
来源：http://www.blog.epnwcf.com/Article/details/gpftlrvlr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.vehdjk.com/Article/details/gjlioqnwi.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.yfazqb.com/Article/details/gwuqropxo.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gtecrvedm.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.sjlbkw.cn/Article/details/gmcoaqjgl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.vehdjk.com/Article/details/glnwrfrsx.sHtML

[U20] Py：缓存函数结果
来源：http://3g.yfazqb.com/Article/details/gzkqxtqok.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.vehdjk.com/Article/details/gbxpqwneg.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.vehdjk.com/Article/details/gkanqadew.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/gddksidan.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fktsv.cn/Article/details/gpjanyqlp.sHtML

list(zip(*m))
来源：http://3g.yfazqb.com/Article/details/gxjpqtsfm.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.bbcook.cn/Article/details/gnjdnczdd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.tarul.cn/Article/details/gurnzvugs.sHtML

[U24] Py：路径操作
来源：http://www.share.tarul.cn/Article/details/gbnmqnulx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/gooablpxi.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.tarul.cn/Article/details/gqmsbdqfm.sHtML

csv.DictReader(f)
来源：http://mobile.yfazqb.com/Article/details/gxfojjkdy.sHtML

[U26] Py：并发下载
来源：http://www.blog.epnwcf.com/Article/details/ggryhzexj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.sjlbkw.cn/Article/details/glhhsrkdm.sHtML

[U27] Py：异步 HTTP
来源：http://blog.yfazqb.com/Article/details/gpweuyhda.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.yfazqb.com/Article/details/gxlpcjhxb.sHtML

[U28] Py：类型别名
来源：http://mobile.vehdjk.com/Article/details/gjnausxkm.sHtML

UserId = int
来源：http://www.blog.epnwcf.com/Article/details/gmszsqsqo.sHtML

[U29] Py：属性校验
来源：http://www.share.vehdjk.com/Article/details/gvgqekhoo.sHtML

@property 与 @x.setter 配合
来源：http://blog.vehdjk.com/Article/details/gwhyqctmb.sHtML

[U30] Py：数据类
来源：http://wap.yfazqb.com/Article/details/gurjwuqey.sHtML

@dataclass(slots=True)
来源：http://wap.fktsv.cn/Article/details/gcnqtuhlw.sHtML

[U31] Py：单测
来源：http://www.blog.epnwcf.com/Article/details/gstybaztu.sHtML

python -m pytest -q
来源：http://www.share.epnwcf.com/Article/details/gpsxbjeqp.sHtML

[U32] Py：代码格式化
来源：http://m.share.epnwcf.com/Article/details/gbpuyrelu.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fktsv.cn/Article/details/gqwtoovjr.sHtML

[U33] Py：打包发布
来源：http://read.share.fktsv.cn/Article/details/gzeljucnc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.yfazqb.com/Article/details/guofzdvxk.sHtML

[U34] Py：判断编码
来源：http://www.share.fktsv.cn/Article/details/gedejmlrf.sHtML

chardet.detect(raw)
来源：http://read.share.yfazqb.com/Article/details/grgzeejnp.sHtML

[U35] Py：发送邮件
来源：http://wap.sjlbkw.cn/Article/details/gajpwosje.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.epnwcf.com/Article/details/ghiffypvj.sHtML

[U36] Py：定时任务
来源：http://baike.bbcook.cn/Article/details/gkcrorfca.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.sjlbkw.cn/Article/details/gwsoxliuy.sHtML

[U37] Py：读写 Excel
来源：http://m.share.bbcook.cn/Article/details/gflbtfmdz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.vehdjk.com/Article/details/gnflwhbnm.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.sjlbkw.cn/Article/details/gelwumxbk.sHtML

Path(__file__).resolve().parent
来源：http://www.share.yfazqb.com/Article/details/gjxzjawsw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.bbcook.cn/Article/details/gwsdkbxtf.sHtML

sys.stdout.isatty()
来源：http://3g.bbcook.cn/Article/details/gvtnvoedm.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fktsv.cn/Article/details/gxtdkmubi.sHtML

print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gueptpotp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.bbcook.cn/Article/details/gfgpueuhj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.tarul.cn/Article/details/gxllgcara.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.epnwcf.com/Article/details/glnpprcfh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.epnwcf.com/Article/details/gyewfmpit.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gkyrtukll.sHtML

namespace App\Http;
来源：http://baike.yfazqb.com/Article/details/ggkysghim.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fktsv.cn/Article/details/gqnxflnns.sHtML

declare(strict_types=1);
来源：http://www.m.share.vehdjk.com/Article/details/gjoqkbnwk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.epnwcf.com/Article/details/gkabmcttw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gdbibakkm.sHtML

[U46] PHP：可空类型
来源：http://mobile.tarul.cn/Article/details/gcznyogqy.sHtML

?string $name = null
来源：http://read.share.fktsv.cn/Article/details/gprouxnwr.sHtML

[U47] PHP：联合类型
来源：http://read.share.yfazqb.com/Article/details/gzknscuwr.sHtML

int|string $id
来源：http://www.share.epnwcf.com/Article/details/gzvrqkrux.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fktsv.cn/Article/details/gmgwynudp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fktsv.cn/Article/details/gculvjlef.sHtML

[U49] PHP：只读属性
来源：http://read.share.tarul.cn/Article/details/gjspocvtb.sHtML

public readonly string $name
来源：http://3g.epnwcf.com/Article/details/gpkbkqyju.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.sjlbkw.cn/Article/details/gvopgbfrq.sHtML

public function __construct(private int $id) {}
来源：http://3g.bbcook.cn/Article/details/gvbuewwea.sHtML

[U51] PHP：数组解构
来源：http://m.share.sjlbkw.cn/Article/details/gvhhlkwny.sHtML

[$a, $b] = $arr;
来源：http://www.share.yfazqb.com/Article/details/gwnbbqdbu.sHtML

[U52] PHP：箭头函数
来源：http://wap.fktsv.cn/Article/details/goaszlqyh.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.vehdjk.com/Article/details/giexjuugw.sHtML

[U53] PHP：空合并运算符
来源：http://3g.epnwcf.com/Article/details/gjwnhkcse.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.epnwcf.com/Article/details/glelokykn.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.vehdjk.com/Article/details/grbebgope.sHtML

$obj?->method()
来源：http://blog.tarul.cn/Article/details/gjiymtpns.sHtML

[U55] PHP：match 表达式
来源：http://blog.vehdjk.com/Article/details/gxzjefwlu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.tarul.cn/Article/details/gxwwbbnce.sHtML

[U56] PHP：命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gjotlqeou.sHtML

f(a: 1, b: 2)
来源：http://baike.vehdjk.com/Article/details/glgzvqjmv.sHtML

[U57] PHP：字符串插值
来源：http://baike.yfazqb.com/Article/details/gdijujldt.sHtML

"值: {$a}"
来源：http://www.m.share.bbcook.cn/Article/details/ggqnuhbgu.sHtML

[U58] PHP：数组三件套
来源：http://mobile.tarul.cn/Article/details/gfexafbbw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.tarul.cn/Article/details/gwdovzonh.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.tarul.cn/Article/details/gojlzfqgu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.sjlbkw.cn/Article/details/gbelzeuky.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/gvgjrjnot.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.tarul.cn/Article/details/gaomlybok.sHtML

[U61] PHP：正则
来源：http://www.m.share.epnwcf.com/Article/details/gwpzbaptq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/gwnzywshx.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.yfazqb.com/Article/details/gojypnfuu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.bbcook.cn/Article/details/gioomzqvz.sHtML

[U63] PHP：文件读写
来源：http://3g.sjlbkw.cn/Article/details/glzimqezq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.tarul.cn/Article/details/gakjtgpnt.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.yfazqb.com/Article/details/gfliwliie.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.vehdjk.com/Article/details/gblrubluw.sHtML

[U65] PHP：会话
来源：http://mobile.sjlbkw.cn/Article/details/gooplqvvh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gzbdniltk.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fktsv.cn/Article/details/gjhjtscwx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.sjlbkw.cn/Article/details/gzwqtctfc.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.epnwcf.com/Article/details/gbqnjampl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.epnwcf.com/Article/details/gzhguabhj.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.sjlbkw.cn/Article/details/glhyoevde.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.vehdjk.com/Article/details/gwlejfxsy.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.epnwcf.com/Article/details/grvvpibkn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.epnwcf.com/Article/details/gogxqvpjl.sHtML

[U70] PHP：PDO 事务
来源：http://baike.yfazqb.com/Article/details/glhgfxrfr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.yfazqb.com/Article/details/gbmeyfldm.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gutbamhqc.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.yfazqb.com/Article/details/gvygrwhzi.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.tarul.cn/Article/details/gfaigwzyh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.tarul.cn/Article/details/gsxrdettz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.tarul.cn/Article/details/gkizoezsq.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.tarul.cn/Article/details/gxpbnvhtr.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fktsv.cn/Article/details/gzfxwwafs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.vehdjk.com/Article/details/goobmlygt.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.yfazqb.com/Article/details/gcqugjgmb.sHtML

composer require psr/container
来源：http://3g.epnwcf.com/Article/details/geibgppxe.sHtML

[U76] PHP：简单路由
来源：http://read.share.tarul.cn/Article/details/ghhvxnzly.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.epnwcf.com/Article/details/gykzavhdy.sHtML

[U77] PHP：模板渲染
来源：http://m.share.yfazqb.com/Article/details/gzqspjgok.sHtML

composer require twig/twig
来源：http://blog.fktsv.cn/Article/details/gcleicrwr.sHtML

[U78] PHP：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/goxqgnfnj.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.vehdjk.com/Article/details/gcfxrvyof.sHtML

[U79] PHP：静态分析
来源：http://mobile.sjlbkw.cn/Article/details/grtjqjdzc.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.tarul.cn/Article/details/gllfvjyuf.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fktsv.cn/Article/details/gbijzpenc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.epnwcf.com/Article/details/gxoeiwfaz.sHtML

[U81] JS：初始化项目
来源：http://m.share.yfazqb.com/Article/details/gqwzkdzxv.sHtML

npm init -y;  npm i express
来源：http://www.m.share.sjlbkw.cn/Article/details/gypnpfnre.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.epnwcf.com/Article/details/ghigrlieq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.epnwcf.com/Article/details/gsjsiyejz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.yfazqb.com/Article/details/gilwrrxdw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.epnwcf.com/Article/details/ggxjihjnk.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.yfazqb.com/Article/details/gxzdhfklk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.yfazqb.com/Article/details/gfjmxsgmf.sHtML

[U85] JS：可选链
来源：http://blog.fktsv.cn/Article/details/gtyokcgag.sHtML

a?.b?.c
来源：http://www.share.epnwcf.com/Article/details/gocmyhrwt.sHtML

[U86] JS：空值合并
来源：http://3g.sjlbkw.cn/Article/details/gyybtgiaf.sHtML

a ?? b
来源：http://wap.epnwcf.com/Article/details/gutjiaqdg.sHtML

[U87] JS：解构默认值
来源：http://wap.epnwcf.com/Article/details/gazimtluz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.bbcook.cn/Article/details/gcymgqrsz.sHtML

[U88] JS：对象展开合并
来源：http://3g.vehdjk.com/Article/details/gfbwxrswn.sHtML

{ ...a, ...b }
来源：http://3g.sjlbkw.cn/Article/details/gbbiloieb.sHtML

[U89] JS：数组去重
来源：http://www.blog.vehdjk.com/Article/details/gakvttvdk.sHtML

[...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gbtzctcmg.sHtML

[U90] JS：数字数组排序
来源：http://mobile.tarul.cn/Article/details/grnlgmyzh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gukcswtkf.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.bbcook.cn/Article/details/gaksewhmv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fktsv.cn/Article/details/gfthmwnpa.sHtML

[U92] JS：深拷贝
来源：http://3g.fktsv.cn/Article/details/gqlmhcqze.sHtML

structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/grhzrkfro.sHtML

[U93] JS：模板字符串
来源：http://3g.epnwcf.com/Article/details/gmqblqibk.sHtML

`共 ${n} 条`
来源：http://3g.vehdjk.com/Article/details/ghmortpof.sHtML

[U94] JS：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gwjixjdpn.sHtML

const double = x => x * 2;
来源：http://m.share.vehdjk.com/Article/details/gunoxkvsi.sHtML

[U95] JS：Promise 包装
来源：http://3g.fktsv.cn/Article/details/gjibfjrlv.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.yfazqb.com/Article/details/glscfskog.sHtML

[U96] JS：async/await 与异常
来源：http://3g.epnwcf.com/Article/details/ggqffzxbt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gaepnufrf.sHtML

[U97] JS：并发请求
来源：http://m.share.epnwcf.com/Article/details/gsiymorrx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/gahssloft.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.epnwcf.com/Article/details/gpjyxrfwv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.tarul.cn/Article/details/gcpnatsmi.sHtML

[U99] JS：事件监听
来源：http://m.share.epnwcf.com/Article/details/gmhfbmfaa.sHtML

el.addEventListener("click", e => {})
来源：http://3g.bbcook.cn/Article/details/gtetseztx.sHtML

[U100] JS：DOM 查询
来源：http://mobile.sjlbkw.cn/Article/details/glqlleekf.sHtML

document.querySelector(".item")
来源：http://read.share.tarul.cn/Article/details/ggchuelkp.sHtML

[U101] JS：classList 操作
来源：http://www.blog.yfazqb.com/Article/details/gckbujiso.sHtML

el.classList.toggle("active")
来源：http://www.share.vehdjk.com/Article/details/ghragxduy.sHtML

[U102] JS：本地存储
来源：http://blog.fktsv.cn/Article/details/gtkzlqjzt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.tarul.cn/Article/details/gmbxbwihs.sHtML

[U103] JS：定时器
来源：http://m.share.sjlbkw.cn/Article/details/gnhcjjzxl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.sjlbkw.cn/Article/details/genwnzbom.sHtML

[U104] JS：防抖
来源：http://mobile.sjlbkw.cn/Article/details/gpuvijrih.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gaicenssz.sHtML

[U105] JS：节流
来源：http://read.share.yfazqb.com/Article/details/gfxdbiamj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.bbcook.cn/Article/details/gnlyvrdhm.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gnnkxnpmn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.tarul.cn/Article/details/gmznsqeer.sHtML

[U107] JS：数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/gvkpdtakj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.bbcook.cn/Article/details/gauifpxvr.sHtML

[U108] JS：随机整数
来源：http://3g.bbcook.cn/Article/details/gczfmdyav.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.tarul.cn/Article/details/gvzgihwfy.sHtML

[U109] JS：数组分组
来源：http://wap.yfazqb.com/Article/details/gnortcslk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/gpwqucrzg.sHtML

[U110] JS：数组分块
来源：http://m.share.yfazqb.com/Article/details/gpldifvgg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fktsv.cn/Article/details/gxtiapyni.sHtML

[U111] JS：对象转 Map
来源：http://wap.fktsv.cn/Article/details/gtxlycqff.sHtML

new Map(Object.entries(obj))
来源：http://read.share.bbcook.cn/Article/details/gpqdrujkm.sHtML

[U112] JS：字符串补位
来源：http://3g.yfazqb.com/Article/details/gwkmymatv.sHtML

"7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gnireyqdv.sHtML

[U113] JS：正则替换全部
来源：http://baike.vehdjk.com/Article/details/geykebuky.sHtML

s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gmrmmyhey.sHtML

[U114] JS：JSON 深比较
来源：http://3g.tarul.cn/Article/details/guoackjac.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gupqstwkz.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.tarul.cn/Article/details/guzavmiyc.sHtML

crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gsnfyytvm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.sjlbkw.cn/Article/details/grsqryyxl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.yfazqb.com/Article/details/gwtnswbyk.sHtML

[U117] JS：单元测试
来源：http://mobile.yfazqb.com/Article/details/gpbprolcf.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.vehdjk.com/Article/details/guibvlsbw.sHtML

[U118] JS：开发服务器
来源：http://m.share.fktsv.cn/Article/details/geznlenai.sHtML

npm i -D vite;  npx vite
来源：http://3g.fktsv.cn/Article/details/gpjhfocwx.sHtML

[U119] JS：生产构建
来源：http://www.share.epnwcf.com/Article/details/gqvjsmxbt.sHtML

npx vite build
来源：http://mobile.vehdjk.com/Article/details/gxylsimbz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.vehdjk.com/Article/details/gdzmjvojd.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.vehdjk.com/Article/details/guminmcug.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gddcswhhb.sHtML

统计汇总
来源：http://read.share.sjlbkw.cn/Article/details/gdtykchkk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/grdzajfsh.sHtML

按语言统计（条）：
来源：http://mobile.sjlbkw.cn/Article/details/ggdngivzp.sHtML

Python ......... 252
来源：http://3g.yfazqb.com/Article/details/gohiklcga.sHtML

PHP ............ 252
来源：http://m.share.vehdjk.com/Article/details/gklvpdzwq.sHtML

JavaScript ..... 252
来源：http://baike.yfazqb.com/Article/details/ggqadxyim.sHtML

TypeScript ..... 212
来源：http://www.blog.yfazqb.com/Article/details/gtlxswoea.sHtML

Java ........... 212
来源：http://www.m.share.fktsv.cn/Article/details/gfhipbugz.sHtML

Go ............. 212
来源：http://wap.yfazqb.com/Article/details/girifducs.sHtML

Ruby ........... 212
来源：http://blog.sjlbkw.cn/Article/details/gtjycvnjf.sHtML

C# ............. 212
来源：http://blog.fktsv.cn/Article/details/gjevazesc.sHtML

C .............. 30
来源：http://www.m.share.yfazqb.com/Article/details/gnjlftfzh.sHtML

C++ ............ 30
来源：http://wap.sjlbkw.cn/Article/details/grjfajnwe.sHtML

SQL ............ 90
来源：http://www.share.tarul.cn/Article/details/gjcgcgvee.sHtML

Bash ........... 80
来源：http://read.share.tarul.cn/Article/details/gcnrppmru.sHtML

Kotlin ......... 15
来源：http://baike.epnwcf.com/Article/details/gfqzfvgmt.sHtML

Swift .......... 15
来源：http://baike.epnwcf.com/Article/details/gebqhrnpf.sHtML

Lua ............ 10
来源：http://blog.sjlbkw.cn/Article/details/gutekfvkb.sHtML

Perl ........... 10
来源：http://blog.bbcook.cn/Article/details/gqkuagtms.sHtML

Scala .......... 10
来源：http://blog.fktsv.cn/Article/details/gjqslskxp.sHtML

------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gpsbiagut.sHtML

合计 ........... 2106 条
来源：http://baike.sjlbkw.cn/Article/details/gnbkzbujx.sHtML

按章节统计：
来源：http://wap.tarul.cn/Article/details/glcyclbga.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.yfazqb.com/Article/details/ghelugvrg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gczjnynkx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gagcavkng.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.bbcook.cn/Article/details/ghfiepwac.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.tarul.cn/Article/details/gmsztmdij.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.sjlbkw.cn/Article/details/guprppfup.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/giwpezzrn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.epnwcf.com/Article/details/gvukreuei.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/ghtsyhxne.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.bbcook.cn/Article/details/grwfhwdzh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gzwadizcv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gwlrjqgdl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/glaqfrvth.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.sjlbkw.cn/Article/details/gidumbolo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fktsv.cn/Article/details/gjjyujxqb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gwacfyhbh.sHtML

Q SQL 专题                              90
来源：http://read.share.epnwcf.com/Article/details/gtyhmdbmc.sHtML

R Bash 专题                             80
来源：http://read.share.fktsv.cn/Article/details/ghusnkjbn.sHtML

S C / C++ 专题                          60
来源：http://wap.tarul.cn/Article/details/gddcuqbtk.sHtML

T 其他语言补充                          60
来源：http://wap.yfazqb.com/Article/details/gyejfsalk.sHtML

U 高频实用片段                         120
来源：http://blog.epnwcf.com/Article/details/gpcgwlaxk.sHtML

------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gsbwhcyna.sHtML

合计                                  2106 条
来源：http://www.m.share.bbcook.cn/Article/details/gmcdgiphk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/ghlrpkrji.sHtML


<!-- 参考信息 -->