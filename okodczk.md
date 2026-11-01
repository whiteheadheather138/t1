代发 wailian999

case class User(name: String, age: Int)
来源：http://www.blog.vehdjk.com/Article/details/gqabmiwam.sHtML

[T57] Scala：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/gydwbluyo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.vehdjk.com/Article/details/gosyhbruc.sHtML

[T58] Scala：函数定义
来源：http://m.share.fktsv.cn/Article/details/gxyehrciy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.bbcook.cn/Article/details/gkpmqkubd.sHtML

[T59] Scala：循环
来源：http://3g.sjlbkw.cn/Article/details/gbnsruzkb.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gmwxztwgh.sHtML

[T60] Scala：折叠
来源：http://3g.sjlbkw.cn/Article/details/ghtkqeaew.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.yfazqb.com/Article/details/gstfkuwqx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gtnisyfbw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gundbqccr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvptcpwgm.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.bbcook.cn/Article/details/gvqivunqc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.sjlbkw.cn/Article/details/gtrkqynbw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.sjlbkw.cn/Article/details/gnjdcgpgc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.yfazqb.com/Article/details/gcvigeqdh.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.bbcook.cn/Article/details/ggzxxonff.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.tarul.cn/Article/details/gdnmbxian.sHtML

[U04] Py：变量调试打印
来源：http://wap.fktsv.cn/Article/details/gouimoeht.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fktsv.cn/Article/details/gilbdamgo.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fktsv.cn/Article/details/gnranmkef.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gaqcczzks.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.tarul.cn/Article/details/gmxwfgkha.sHtML

{**a, **b}
来源：http://read.share.yfazqb.com/Article/details/gxfnprlie.sHtML

[U07] Py：反转字典键值
来源：http://wap.fktsv.cn/Article/details/gvtfhazoq.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.tarul.cn/Article/details/getiumbdo.sHtML

[U08] Py：展平二维列表
来源：http://read.share.tarul.cn/Article/details/gxnhenppe.sHtML

[y for x in nested for y in x]
来源：http://www.share.tarul.cn/Article/details/gawddxopn.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.vehdjk.com/Article/details/gegdyrmds.sHtML

max(d, key=d.get)
来源：http://www.share.bbcook.cn/Article/details/gdjllbmbp.sHtML

[U10] Py：按值排序字典
来源：http://baike.epnwcf.com/Article/details/ghsbvaazu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.vehdjk.com/Article/details/gkcrpfvfy.sHtML

[U11] Py：生成器表达式
来源：http://baike.epnwcf.com/Article/details/geqaqjlue.sHtML

(x * 2 for x in arr)
来源：http://read.share.bbcook.cn/Article/details/gzwdvuhjb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.tarul.cn/Article/details/gnigrfirw.sHtML

Counter(arr).most_common(3)
来源：http://baike.tarul.cn/Article/details/gjtrkcmer.sHtML

[U13] Py：固定长度队列
来源：http://baike.tarul.cn/Article/details/gpugzvvpy.sHtML

deque(maxlen=10)
来源：http://3g.fktsv.cn/Article/details/gvyztvwbu.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.sjlbkw.cn/Article/details/gvracnsan.sHtML

defaultdict(list)
来源：http://3g.vehdjk.com/Article/details/gqwsaurzn.sHtML

[U15] Py：高精度计时
来源：http://blog.tarul.cn/Article/details/gttiqcjtv.sHtML

t = time.perf_counter()
来源：http://www.m.share.vehdjk.com/Article/details/gxvhponqr.sHtML

[U16] Py：命令行参数解析
来源：http://3g.sjlbkw.cn/Article/details/gozesrokq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.tarul.cn/Article/details/gizjyduxa.sHtML

[U17] Py：初始化日志
来源：http://wap.yfazqb.com/Article/details/gpzetatkp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.yfazqb.com/Article/details/ganvqoehw.sHtML

[U18] Py：预编译正则
来源：http://m.share.yfazqb.com/Article/details/gzcrbaryk.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.epnwcf.com/Article/details/greesaqif.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fktsv.cn/Article/details/gsrzsbvlk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.vehdjk.com/Article/details/gjzqbfone.sHtML

[U20] Py：缓存函数结果
来源：http://3g.bbcook.cn/Article/details/gycslrjxv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.sjlbkw.cn/Article/details/gsjzuaath.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.tarul.cn/Article/details/gojqemlzd.sHtML

@contextlib.contextmanager
来源：http://www.m.share.bbcook.cn/Article/details/gwckzosxi.sHtML

[U22] Py：矩阵转置
来源：http://blog.bbcook.cn/Article/details/gorhxbgna.sHtML

list(zip(*m))
来源：http://blog.sjlbkw.cn/Article/details/gnyfsmpxm.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.yfazqb.com/Article/details/gwhdhfnix.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.bbcook.cn/Article/details/gdtursqvc.sHtML

[U24] Py：路径操作
来源：http://www.share.fktsv.cn/Article/details/gmpoqqiav.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.yfazqb.com/Article/details/gafmplwzv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.bbcook.cn/Article/details/gshainqye.sHtML

csv.DictReader(f)
来源：http://read.share.epnwcf.com/Article/details/galdpbyrh.sHtML

[U26] Py：并发下载
来源：http://www.blog.epnwcf.com/Article/details/glrtcgqvh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.vehdjk.com/Article/details/gmsfzkgqp.sHtML

[U27] Py：异步 HTTP
来源：http://3g.epnwcf.com/Article/details/geimuarap.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.yfazqb.com/Article/details/gmaehcpjk.sHtML

[U28] Py：类型别名
来源：http://m.share.sjlbkw.cn/Article/details/gyyatgkfy.sHtML

UserId = int
来源：http://www.blog.tarul.cn/Article/details/gjetfuvef.sHtML

[U29] Py：属性校验
来源：http://baike.bbcook.cn/Article/details/gpqnlnpfs.sHtML

@property 与 @x.setter 配合
来源：http://blog.tarul.cn/Article/details/gagaanffs.sHtML

[U30] Py：数据类
来源：http://mobile.yfazqb.com/Article/details/gvurwwxfl.sHtML

@dataclass(slots=True)
来源：http://mobile.epnwcf.com/Article/details/gvtcqsrjy.sHtML

[U31] Py：单测
来源：http://www.share.fktsv.cn/Article/details/ghsmwtfzb.sHtML

python -m pytest -q
来源：http://www.m.share.yfazqb.com/Article/details/gksyitumd.sHtML

[U32] Py：代码格式化
来源：http://m.share.sjlbkw.cn/Article/details/grnwirtju.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fktsv.cn/Article/details/ghftdqpzi.sHtML

[U33] Py：打包发布
来源：http://m.share.tarul.cn/Article/details/gptppbefa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.bbcook.cn/Article/details/gybpygeao.sHtML

[U34] Py：判断编码
来源：http://baike.epnwcf.com/Article/details/gwcbuvvsn.sHtML

chardet.detect(raw)
来源：http://mobile.fktsv.cn/Article/details/gkygqrtsp.sHtML

[U35] Py：发送邮件
来源：http://www.share.bbcook.cn/Article/details/gvdbjkogb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.yfazqb.com/Article/details/gvfiutqfc.sHtML

[U36] Py：定时任务
来源：http://baike.epnwcf.com/Article/details/gwejgzjna.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.tarul.cn/Article/details/gnhrhdnjk.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fktsv.cn/Article/details/gzjjxftxu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.tarul.cn/Article/details/gkeyltljk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.yfazqb.com/Article/details/gvhdosvwr.sHtML

Path(__file__).resolve().parent
来源：http://3g.tarul.cn/Article/details/gpjgqpmpg.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.vehdjk.com/Article/details/gsoffjkbl.sHtML

sys.stdout.isatty()
来源：http://mobile.epnwcf.com/Article/details/groayruip.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.sjlbkw.cn/Article/details/gktceykwu.sHtML

print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/gycfqlggu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.sjlbkw.cn/Article/details/guqwyropv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.yfazqb.com/Article/details/gmtsdrptv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.tarul.cn/Article/details/glknssrvr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.sjlbkw.cn/Article/details/ghbpgifei.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fktsv.cn/Article/details/gspodlqvw.sHtML

namespace App\Http;
来源：http://wap.vehdjk.com/Article/details/gaxnqszlp.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.yfazqb.com/Article/details/gyczggxtm.sHtML

declare(strict_types=1);
来源：http://www.blog.bbcook.cn/Article/details/gjgheenvz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.sjlbkw.cn/Article/details/gedjsqifa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/ggrlhnvhx.sHtML

[U46] PHP：可空类型
来源：http://www.blog.bbcook.cn/Article/details/gugjagfmv.sHtML

?string $name = null
来源：http://read.share.epnwcf.com/Article/details/gulywwcky.sHtML

[U47] PHP：联合类型
来源：http://baike.bbcook.cn/Article/details/gxvqvsrtz.sHtML

int|string $id
来源：http://m.share.yfazqb.com/Article/details/gbakmbnpw.sHtML

[U48] PHP：纯枚举
来源：http://www.share.epnwcf.com/Article/details/gxeczwekm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.bbcook.cn/Article/details/gyrsjbefd.sHtML

[U49] PHP：只读属性
来源：http://wap.bbcook.cn/Article/details/gkkkerwic.sHtML

public readonly string $name
来源：http://3g.epnwcf.com/Article/details/gtenqixrt.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.vehdjk.com/Article/details/ghisidaph.sHtML

public function __construct(private int $id) {}
来源：http://baike.vehdjk.com/Article/details/ggbbvefkv.sHtML

[U51] PHP：数组解构
来源：http://baike.vehdjk.com/Article/details/gvkjvqfrt.sHtML

[$a, $b] = $arr;
来源：http://www.blog.tarul.cn/Article/details/galagpkpr.sHtML

[U52] PHP：箭头函数
来源：http://baike.epnwcf.com/Article/details/gifxxsgzi.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fktsv.cn/Article/details/gttxtcext.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.yfazqb.com/Article/details/gjjdmoovx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.bbcook.cn/Article/details/gsimrqzbz.sHtML

[U54] PHP：空安全调用
来源：http://mobile.epnwcf.com/Article/details/gcvjewisn.sHtML

$obj?->method()
来源：http://read.share.tarul.cn/Article/details/gzelibbae.sHtML

[U55] PHP：match 表达式
来源：http://baike.vehdjk.com/Article/details/gpelevwmp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgddvkif.sHtML

[U56] PHP：命名参数
来源：http://www.blog.epnwcf.com/Article/details/gkatkcqet.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gmlrjxahe.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/ggpwltmuv.sHtML

"值: {$a}"
来源：http://3g.tarul.cn/Article/details/gulkxyjtv.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.yfazqb.com/Article/details/gserkeuqr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.epnwcf.com/Article/details/ggjmtxgqm.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fktsv.cn/Article/details/gvdislxqz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.bbcook.cn/Article/details/gogmefxle.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fktsv.cn/Article/details/ggwkkrxbv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.yfazqb.com/Article/details/gwqqyfbbt.sHtML

[U61] PHP：正则
来源：http://www.share.epnwcf.com/Article/details/gezcmmumg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gxriovgyk.sHtML

[U62] PHP：日期对象
来源：http://read.share.yfazqb.com/Article/details/gkevxcsht.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.bbcook.cn/Article/details/gmxwiqtag.sHtML

[U63] PHP：文件读写
来源：http://read.share.sjlbkw.cn/Article/details/gajrtnnwz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.tarul.cn/Article/details/grzjuksip.sHtML

[U64] PHP：目录遍历
来源：http://mobile.tarul.cn/Article/details/gtqxsuzjm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.tarul.cn/Article/details/gzqdlmfff.sHtML

[U65] PHP：会话
来源：http://3g.yfazqb.com/Article/details/ggebzshmd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.bbcook.cn/Article/details/gbwdqqtue.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.vehdjk.com/Article/details/gqxbfkbny.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fktsv.cn/Article/details/gdokvufaj.sHtML

[U67] PHP：处理文件上传
来源：http://3g.sjlbkw.cn/Article/details/gqovwazqx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.vehdjk.com/Article/details/gmmwtfyof.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.sjlbkw.cn/Article/details/garwuygem.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.sjlbkw.cn/Article/details/gquolsdtv.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.epnwcf.com/Article/details/gqwxtjkow.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.vehdjk.com/Article/details/gufcvpdgn.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.yfazqb.com/Article/details/gdayyixth.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.vehdjk.com/Article/details/gfmpcgwzs.sHtML

[U71] PHP：抛出异常
来源：http://3g.tarul.cn/Article/details/gvpxkkusi.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.sjlbkw.cn/Article/details/gfbojsflr.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.yfazqb.com/Article/details/gawbpmuut.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.yfazqb.com/Article/details/gqzuqzxui.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.epnwcf.com/Article/details/giiodsdcf.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.sjlbkw.cn/Article/details/grbopktrv.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gsvutopoj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.sjlbkw.cn/Article/details/gdvwphkuo.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fktsv.cn/Article/details/gorsliwfi.sHtML

composer require psr/container
来源：http://www.blog.epnwcf.com/Article/details/gxrvkapsz.sHtML

[U76] PHP：简单路由
来源：http://www.share.fktsv.cn/Article/details/ggpqdrvbk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.tarul.cn/Article/details/gkfrhbinw.sHtML

[U77] PHP：模板渲染
来源：http://wap.bbcook.cn/Article/details/gvkuyasht.sHtML

composer require twig/twig
来源：http://3g.tarul.cn/Article/details/gvyywatca.sHtML

[U78] PHP：单元测试
来源：http://3g.epnwcf.com/Article/details/geqssqtgg.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.yfazqb.com/Article/details/gghskhsei.sHtML

[U79] PHP：静态分析
来源：http://3g.yfazqb.com/Article/details/gwcnvkxzg.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.vehdjk.com/Article/details/gpmwgxyom.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.vehdjk.com/Article/details/ggxzrbtca.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.sjlbkw.cn/Article/details/gqxfciead.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.yfazqb.com/Article/details/gyjsxksau.sHtML

npm init -y;  npm i express
来源：http://www.blog.epnwcf.com/Article/details/ghrhfqmix.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.epnwcf.com/Article/details/gwotqknnd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.tarul.cn/Article/details/gcgszxjcr.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.bbcook.cn/Article/details/guzwyrhnw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/grwnirsge.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fktsv.cn/Article/details/gskowmmpe.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.tarul.cn/Article/details/gdzzynxqk.sHtML

[U85] JS：可选链
来源：http://www.blog.vehdjk.com/Article/details/gjhncdjje.sHtML

a?.b?.c
来源：http://blog.epnwcf.com/Article/details/gbawxolcv.sHtML

[U86] JS：空值合并
来源：http://3g.fktsv.cn/Article/details/gmluejxen.sHtML

a ?? b
来源：http://3g.epnwcf.com/Article/details/guerfguhj.sHtML

[U87] JS：解构默认值
来源：http://read.share.bbcook.cn/Article/details/glfeevfxb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.bbcook.cn/Article/details/geqdxtekf.sHtML

[U88] JS：对象展开合并
来源：http://wap.vehdjk.com/Article/details/gokxubszs.sHtML

{ ...a, ...b }
来源：http://baike.sjlbkw.cn/Article/details/gmbxwotws.sHtML

[U89] JS：数组去重
来源：http://read.share.sjlbkw.cn/Article/details/gwbcyrckt.sHtML

[...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gdfummttk.sHtML

[U90] JS：数字数组排序
来源：http://www.share.tarul.cn/Article/details/gtikvlqxk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gmffirqwu.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.epnwcf.com/Article/details/gtiddfaua.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.yfazqb.com/Article/details/guugzvdau.sHtML

[U92] JS：深拷贝
来源：http://www.blog.vehdjk.com/Article/details/glybdfkfa.sHtML

structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gevdpthyv.sHtML

[U93] JS：模板字符串
来源：http://wap.epnwcf.com/Article/details/geubntuit.sHtML

`共 ${n} 条`
来源：http://www.share.fktsv.cn/Article/details/grsxzrlow.sHtML

[U94] JS：箭头函数
来源：http://read.share.bbcook.cn/Article/details/gqspaffbv.sHtML

const double = x => x * 2;
来源：http://www.blog.sjlbkw.cn/Article/details/gsqrvospw.sHtML

[U95] JS：Promise 包装
来源：http://baike.sjlbkw.cn/Article/details/giqxwwbur.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.tarul.cn/Article/details/ghcdoaexs.sHtML

[U96] JS：async/await 与异常
来源：http://baike.yfazqb.com/Article/details/gvjmkwtql.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gfgkwratm.sHtML

[U97] JS：并发请求
来源：http://wap.vehdjk.com/Article/details/gxkkaevtk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gqajoxdfz.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.bbcook.cn/Article/details/ghhnlqejh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.epnwcf.com/Article/details/gpoxcokhv.sHtML

[U99] JS：事件监听
来源：http://baike.bbcook.cn/Article/details/ghkkxhyiq.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fktsv.cn/Article/details/gonbeletz.sHtML

[U100] JS：DOM 查询
来源：http://blog.sjlbkw.cn/Article/details/gmhxnedvv.sHtML

document.querySelector(".item")
来源：http://read.share.sjlbkw.cn/Article/details/gpwxsunvx.sHtML

[U101] JS：classList 操作
来源：http://m.share.epnwcf.com/Article/details/gszibhbla.sHtML

el.classList.toggle("active")
来源：http://blog.fktsv.cn/Article/details/gvivzjhzw.sHtML

[U102] JS：本地存储
来源：http://www.blog.vehdjk.com/Article/details/gzoaeekuc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.bbcook.cn/Article/details/gvsrkskkk.sHtML

[U103] JS：定时器
来源：http://mobile.bbcook.cn/Article/details/guqhcivtu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.epnwcf.com/Article/details/gzwqbqglj.sHtML

[U104] JS：防抖
来源：http://m.share.tarul.cn/Article/details/gsqbvhqqt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gjjlfnhci.sHtML

[U105] JS：节流
来源：http://read.share.epnwcf.com/Article/details/gyotsuoyu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.yfazqb.com/Article/details/gdrlarvyx.sHtML

[U106] JS：日期格式化
来源：http://wap.bbcook.cn/Article/details/ghbvweycx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fktsv.cn/Article/details/gsbpdhvds.sHtML

[U107] JS：数字千分位
来源：http://wap.bbcook.cn/Article/details/gttutegox.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.epnwcf.com/Article/details/gtsoecdkd.sHtML

[U108] JS：随机整数
来源：http://www.m.share.tarul.cn/Article/details/gigbhjooe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.sjlbkw.cn/Article/details/gaanuyyyt.sHtML

[U109] JS：数组分组
来源：http://m.share.yfazqb.com/Article/details/gebkjnmhz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fktsv.cn/Article/details/gbmoozugs.sHtML

[U110] JS：数组分块
来源：http://www.blog.epnwcf.com/Article/details/gswqnwsvc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.tarul.cn/Article/details/gnysfkmqm.sHtML

[U111] JS：对象转 Map
来源：http://blog.epnwcf.com/Article/details/gprtiuqry.sHtML

new Map(Object.entries(obj))
来源：http://blog.yfazqb.com/Article/details/gifvcspfi.sHtML

[U112] JS：字符串补位
来源：http://3g.sjlbkw.cn/Article/details/gspfyyovq.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/ghvnivihi.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.sjlbkw.cn/Article/details/gngzrbizf.sHtML

s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gbjttqvdq.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.tarul.cn/Article/details/gosoqpoic.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/ghqlntosm.sHtML

[U115] JS：生成 UUID
来源：http://wap.tarul.cn/Article/details/gfoozxkhp.sHtML

crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gwxekywsv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fktsv.cn/Article/details/gfxasitgl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.yfazqb.com/Article/details/glnwalnrh.sHtML

[U117] JS：单元测试
来源：http://wap.fktsv.cn/Article/details/gnyueepzx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.bbcook.cn/Article/details/geqmrskxb.sHtML

[U118] JS：开发服务器
来源：http://baike.yfazqb.com/Article/details/gonidsyqo.sHtML

npm i -D vite;  npx vite
来源：http://blog.bbcook.cn/Article/details/ggqrryzxm.sHtML

[U119] JS：生产构建
来源：http://baike.tarul.cn/Article/details/gpukbaqxs.sHtML

npx vite build
来源：http://m.share.yfazqb.com/Article/details/gcpvazxwr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfajhyavu.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fktsv.cn/Article/details/guqtuyyqo.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxkritkzm.sHtML

统计汇总
来源：http://www.m.share.sjlbkw.cn/Article/details/gucavciuq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gprtbdtui.sHtML

按语言统计（条）：
来源：http://3g.yfazqb.com/Article/details/gdqnaxucp.sHtML

Python ......... 252
来源：http://mobile.tarul.cn/Article/details/gqrhwaqii.sHtML

PHP ............ 252
来源：http://mobile.epnwcf.com/Article/details/gvrdvbizk.sHtML

JavaScript ..... 252
来源：http://read.share.fktsv.cn/Article/details/gqxkwedhc.sHtML

TypeScript ..... 212
来源：http://www.m.share.bbcook.cn/Article/details/gbrmiwmln.sHtML

Java ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gpaxlrawp.sHtML

Go ............. 212
来源：http://www.blog.fktsv.cn/Article/details/gqitwxnbg.sHtML

Ruby ........... 212
来源：http://www.share.fktsv.cn/Article/details/gkrkigdcd.sHtML

C# ............. 212
来源：http://www.share.vehdjk.com/Article/details/gwvfdjpqz.sHtML

C .............. 30
来源：http://www.blog.epnwcf.com/Article/details/gxqkfznpu.sHtML

C++ ............ 30
来源：http://wap.epnwcf.com/Article/details/gstxqzaca.sHtML

SQL ............ 90
来源：http://blog.yfazqb.com/Article/details/glcibkuuv.sHtML

Bash ........... 80
来源：http://www.blog.tarul.cn/Article/details/gailhsqxr.sHtML

Kotlin ......... 15
来源：http://baike.bbcook.cn/Article/details/gsfaywbyb.sHtML

Swift .......... 15
来源：http://www.blog.yfazqb.com/Article/details/gzokbjxxl.sHtML

Lua ............ 10
来源：http://www.m.share.yfazqb.com/Article/details/gstwydsbb.sHtML

Perl ........... 10
来源：http://www.blog.vehdjk.com/Article/details/glmrcizkr.sHtML

Scala .......... 10
来源：http://3g.fktsv.cn/Article/details/gwjmpkoyz.sHtML

------------------------------------
来源：http://wap.vehdjk.com/Article/details/ghyjjagjj.sHtML

合计 ........... 2106 条
来源：http://baike.bbcook.cn/Article/details/gdwwvcezn.sHtML

按章节统计：
来源：http://read.share.yfazqb.com/Article/details/gldkpiinz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/gsbjahpax.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/gkveazbdf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/gtpiavoxj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gmtnznyqb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.bbcook.cn/Article/details/glhrddpwi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/ghviailfc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gcbbbtplj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.tarul.cn/Article/details/glacefxbk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gkfeqrksf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/gscdapwce.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gxorcveve.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gvyvvjypn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gwuyljffr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.sjlbkw.cn/Article/details/gjwzgcckq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fktsv.cn/Article/details/grinjkybe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/ghzkeirlp.sHtML

Q SQL 专题                              90
来源：http://m.share.vehdjk.com/Article/details/gmlfmelph.sHtML

R Bash 专题                             80
来源：http://www.share.fktsv.cn/Article/details/gyazvmizj.sHtML

S C / C++ 专题                          60
来源：http://www.blog.bbcook.cn/Article/details/glaolohle.sHtML

T 其他语言补充                          60
来源：http://3g.vehdjk.com/Article/details/grodgashu.sHtML

U 高频实用片段                         120
来源：http://www.share.bbcook.cn/Article/details/gixuiwoxw.sHtML

------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gcxlniutg.sHtML

合计                                  2106 条
来源：http://m.share.tarul.cn/Article/details/gajrkipbh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gjrowfnet.sHtML


<!-- 参考信息 -->