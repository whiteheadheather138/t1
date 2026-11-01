代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://blog.tarul.cn/Article/details/gkcgrxlnq.sHtML

[T59] Scala：循环
来源：http://mobile.vehdjk.com/Article/details/gfqxktjkz.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gqsktrykh.sHtML

[T60] Scala：折叠
来源：http://www.share.sjlbkw.cn/Article/details/glbrhqlov.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.vehdjk.com/Article/details/gtmzozxvz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ggtvslizt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.epnwcf.com/Article/details/glwukcewx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grdmnxqht.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.vehdjk.com/Article/details/gtbhphkqz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.bbcook.cn/Article/details/gajyturts.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.tarul.cn/Article/details/gvwqeabcz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.epnwcf.com/Article/details/goyiekwdy.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.bbcook.cn/Article/details/gvfilnntu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.yfazqb.com/Article/details/gleujzcwm.sHtML

[U04] Py：变量调试打印
来源：http://read.share.tarul.cn/Article/details/gztgdggzg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.sjlbkw.cn/Article/details/guczowqwp.sHtML

[U05] Py：列表去重且保序
来源：http://3g.bbcook.cn/Article/details/gmzmujnuk.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/glabsflst.sHtML

[U06] Py：合并两个字典
来源：http://read.share.vehdjk.com/Article/details/gbzxwzbez.sHtML

{**a, **b}
来源：http://3g.fktsv.cn/Article/details/gkrgfojuw.sHtML

[U07] Py：反转字典键值
来源：http://3g.tarul.cn/Article/details/gtyhllmbn.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/ggzkpovcj.sHtML

[U08] Py：展平二维列表
来源：http://read.share.sjlbkw.cn/Article/details/guzlzjclz.sHtML

[y for x in nested for y in x]
来源：http://www.share.tarul.cn/Article/details/gbeuhoyqu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fktsv.cn/Article/details/gkdcthdno.sHtML

max(d, key=d.get)
来源：http://m.share.sjlbkw.cn/Article/details/gyqrtyuvd.sHtML

[U10] Py：按值排序字典
来源：http://read.share.epnwcf.com/Article/details/gwuctgkzj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fktsv.cn/Article/details/gamplpwtt.sHtML

[U11] Py：生成器表达式
来源：http://3g.sjlbkw.cn/Article/details/glalmrfrf.sHtML

(x * 2 for x in arr)
来源：http://www.share.vehdjk.com/Article/details/gzjglqqah.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.bbcook.cn/Article/details/gmlrijzrw.sHtML

Counter(arr).most_common(3)
来源：http://baike.sjlbkw.cn/Article/details/gdbzdsjyo.sHtML

[U13] Py：固定长度队列
来源：http://wap.sjlbkw.cn/Article/details/gdmxbeijb.sHtML

deque(maxlen=10)
来源：http://read.share.tarul.cn/Article/details/gnbeydzjh.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fktsv.cn/Article/details/ggwtbfbue.sHtML

defaultdict(list)
来源：http://mobile.fktsv.cn/Article/details/gondcxogd.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.tarul.cn/Article/details/gwgehulwy.sHtML

t = time.perf_counter()
来源：http://read.share.epnwcf.com/Article/details/glioncisf.sHtML

[U16] Py：命令行参数解析
来源：http://blog.vehdjk.com/Article/details/gzeikpndk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.sjlbkw.cn/Article/details/gedzthmsg.sHtML

[U17] Py：初始化日志
来源：http://wap.bbcook.cn/Article/details/grvfvvacw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.bbcook.cn/Article/details/gmoatlcmf.sHtML

[U18] Py：预编译正则
来源：http://blog.epnwcf.com/Article/details/gklembvdd.sHtML

pat = re.compile(r"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gniakfurf.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.bbcook.cn/Article/details/gsalbhocq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.vehdjk.com/Article/details/ghfhvnlra.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.vehdjk.com/Article/details/gnerqqabx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.tarul.cn/Article/details/gjtxgfota.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.tarul.cn/Article/details/glpyetqbo.sHtML

@contextlib.contextmanager
来源：http://www.share.epnwcf.com/Article/details/gugjfpudq.sHtML

[U22] Py：矩阵转置
来源：http://blog.yfazqb.com/Article/details/goxyfzmzb.sHtML

list(zip(*m))
来源：http://baike.vehdjk.com/Article/details/gjpqjtwyt.sHtML

[U23] Py：分块读取大文件
来源：http://wap.tarul.cn/Article/details/glnaasydl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.tarul.cn/Article/details/gunqcsvte.sHtML

[U24] Py：路径操作
来源：http://mobile.vehdjk.com/Article/details/gwauqvxbn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/grjbhvegl.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.bbcook.cn/Article/details/gkizppbwk.sHtML

csv.DictReader(f)
来源：http://mobile.bbcook.cn/Article/details/gkzdofshu.sHtML

[U26] Py：并发下载
来源：http://blog.sjlbkw.cn/Article/details/gwibupfng.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.sjlbkw.cn/Article/details/gmrfyigux.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fktsv.cn/Article/details/gzbvidlcu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.vehdjk.com/Article/details/gsnxkfunj.sHtML

[U28] Py：类型别名
来源：http://mobile.epnwcf.com/Article/details/galtwjnna.sHtML

UserId = int
来源：http://www.blog.yfazqb.com/Article/details/gbzyrzplh.sHtML

[U29] Py：属性校验
来源：http://www.share.bbcook.cn/Article/details/gsqdcxruo.sHtML

@property 与 @x.setter 配合
来源：http://www.share.tarul.cn/Article/details/gpzjekita.sHtML

[U30] Py：数据类
来源：http://read.share.yfazqb.com/Article/details/gxhdjweqx.sHtML

@dataclass(slots=True)
来源：http://mobile.yfazqb.com/Article/details/gkqjnibae.sHtML

[U31] Py：单测
来源：http://www.share.vehdjk.com/Article/details/gmbpjrvhn.sHtML

python -m pytest -q
来源：http://m.share.bbcook.cn/Article/details/gqfnantpp.sHtML

[U32] Py：代码格式化
来源：http://www.blog.yfazqb.com/Article/details/goyuteshr.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.vehdjk.com/Article/details/ggrcwscmu.sHtML

[U33] Py：打包发布
来源：http://baike.tarul.cn/Article/details/gnfuthjbe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fktsv.cn/Article/details/gakldxzpg.sHtML

[U34] Py：判断编码
来源：http://mobile.sjlbkw.cn/Article/details/gikwphfre.sHtML

chardet.detect(raw)
来源：http://wap.bbcook.cn/Article/details/gvekytjrg.sHtML

[U35] Py：发送邮件
来源：http://www.share.sjlbkw.cn/Article/details/ghylmajok.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.bbcook.cn/Article/details/gjajkrolj.sHtML

[U36] Py：定时任务
来源：http://read.share.yfazqb.com/Article/details/grwdhcihb.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.epnwcf.com/Article/details/gcnsytyyq.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.vehdjk.com/Article/details/gncmonryj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.bbcook.cn/Article/details/gsyqnqvsk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.tarul.cn/Article/details/gdtyodjth.sHtML

Path(__file__).resolve().parent
来源：http://m.share.sjlbkw.cn/Article/details/gauyrlfnc.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fktsv.cn/Article/details/gmuttcsgg.sHtML

sys.stdout.isatty()
来源：http://blog.vehdjk.com/Article/details/gaxdzclhc.sHtML

[U40] Py：打印到标准错误
来源：http://baike.vehdjk.com/Article/details/gtnftzsll.sHtML

print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gccxwljhf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.yfazqb.com/Article/details/gmiofqgav.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.epnwcf.com/Article/details/gsnzktlcq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fktsv.cn/Article/details/gcwzvgziq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.sjlbkw.cn/Article/details/gwytgypzf.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.yfazqb.com/Article/details/gnvbwmsxp.sHtML

namespace App\Http;
来源：http://blog.bbcook.cn/Article/details/gyxlzevhe.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fktsv.cn/Article/details/gcfmjmwtr.sHtML

declare(strict_types=1);
来源：http://wap.yfazqb.com/Article/details/gqucbgtjh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.vehdjk.com/Article/details/giqxvhgcw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gzusaygbs.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gvufkrksy.sHtML

?string $name = null
来源：http://mobile.sjlbkw.cn/Article/details/gsslyrocq.sHtML

[U47] PHP：联合类型
来源：http://www.share.bbcook.cn/Article/details/gzjjuvggt.sHtML

int|string $id
来源：http://read.share.bbcook.cn/Article/details/glxfecoxw.sHtML

[U48] PHP：纯枚举
来源：http://m.share.tarul.cn/Article/details/glhizrowl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.epnwcf.com/Article/details/gdgwjgtjg.sHtML

[U49] PHP：只读属性
来源：http://baike.fktsv.cn/Article/details/gyhzuuunk.sHtML

public readonly string $name
来源：http://www.blog.sjlbkw.cn/Article/details/golgzrqse.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.sjlbkw.cn/Article/details/grrrjwezt.sHtML

public function __construct(private int $id) {}
来源：http://www.share.sjlbkw.cn/Article/details/gafgmvyfi.sHtML

[U51] PHP：数组解构
来源：http://m.share.bbcook.cn/Article/details/gewhakpsv.sHtML

[$a, $b] = $arr;
来源：http://www.blog.yfazqb.com/Article/details/gonmhokaa.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.yfazqb.com/Article/details/gzynzakjb.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.yfazqb.com/Article/details/gmzuqvsqu.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.yfazqb.com/Article/details/gpenkwvwo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.yfazqb.com/Article/details/gbrhibltb.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.epnwcf.com/Article/details/greblhmms.sHtML

$obj?->method()
来源：http://www.blog.fktsv.cn/Article/details/gowgieuji.sHtML

[U55] PHP：match 表达式
来源：http://read.share.epnwcf.com/Article/details/gnlvvnrix.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.bbcook.cn/Article/details/gngmhqtqk.sHtML

[U56] PHP：命名参数
来源：http://m.share.tarul.cn/Article/details/gcaphitay.sHtML

f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gepnjyfsy.sHtML

[U57] PHP：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gknorzjhq.sHtML

"值: {$a}"
来源：http://blog.yfazqb.com/Article/details/gqrorqnyr.sHtML

[U58] PHP：数组三件套
来源：http://mobile.bbcook.cn/Article/details/gtyxkoqnn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.yfazqb.com/Article/details/gelonuhdt.sHtML

[U59] PHP：自定义排序
来源：http://m.share.sjlbkw.cn/Article/details/goeakdope.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/gdzlnhnpt.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.vehdjk.com/Article/details/glcqvyjhb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.bbcook.cn/Article/details/goumhhovz.sHtML

[U61] PHP：正则
来源：http://www.blog.yfazqb.com/Article/details/grwzdjthj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gsvqujmqo.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fktsv.cn/Article/details/gparpwayg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.tarul.cn/Article/details/gpktoobdg.sHtML

[U63] PHP：文件读写
来源：http://wap.vehdjk.com/Article/details/gootxovxo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.tarul.cn/Article/details/gzmpmiknf.sHtML

[U64] PHP：目录遍历
来源：http://blog.vehdjk.com/Article/details/gizgpuaha.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.yfazqb.com/Article/details/gwatesqoy.sHtML

[U65] PHP：会话
来源：http://wap.yfazqb.com/Article/details/gvxomwlms.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.bbcook.cn/Article/details/gffxvodlf.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.sjlbkw.cn/Article/details/gyrelvnlb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fktsv.cn/Article/details/gmxymtvcv.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.yfazqb.com/Article/details/gwlaxdckt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.yfazqb.com/Article/details/gzdgudvmh.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.bbcook.cn/Article/details/gzclzkefn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.epnwcf.com/Article/details/gbnooqapr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.vehdjk.com/Article/details/gwgwfmxbd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.yfazqb.com/Article/details/gljpklkwi.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.bbcook.cn/Article/details/grfilffrr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.vehdjk.com/Article/details/gtlwhgrrl.sHtML

[U71] PHP：抛出异常
来源：http://www.share.epnwcf.com/Article/details/gwgsyjrwt.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.vehdjk.com/Article/details/glcpzmfbb.sHtML

[U72] PHP：写错误日志
来源：http://read.share.vehdjk.com/Article/details/gwnzoupsi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.bbcook.cn/Article/details/gwsoexwbq.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.bbcook.cn/Article/details/gvvtrdqks.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.tarul.cn/Article/details/gdggobtrk.sHtML

[U74] PHP：读取环境变量
来源：http://3g.sjlbkw.cn/Article/details/gzrfypphd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.vehdjk.com/Article/details/gygzwhwti.sHtML

[U75] PHP：依赖注入
来源：http://baike.tarul.cn/Article/details/gldrppoyo.sHtML

composer require psr/container
来源：http://blog.vehdjk.com/Article/details/gwvtayzww.sHtML

[U76] PHP：简单路由
来源：http://baike.tarul.cn/Article/details/ggbbdmzte.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.tarul.cn/Article/details/gljwwquzq.sHtML

[U77] PHP：模板渲染
来源：http://m.share.sjlbkw.cn/Article/details/gbyqxhber.sHtML

composer require twig/twig
来源：http://www.share.yfazqb.com/Article/details/gkcaiexbz.sHtML

[U78] PHP：单元测试
来源：http://baike.vehdjk.com/Article/details/gjtogdaqo.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.yfazqb.com/Article/details/gpxrhzrxu.sHtML

[U79] PHP：静态分析
来源：http://blog.bbcook.cn/Article/details/gqeijxyyw.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.yfazqb.com/Article/details/gcdpykjty.sHtML

[U80] PHP：代码规范修复
来源：http://blog.sjlbkw.cn/Article/details/gawnifbhu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.bbcook.cn/Article/details/gggtnffzz.sHtML

[U81] JS：初始化项目
来源：http://baike.fktsv.cn/Article/details/gqgxxspvr.sHtML

npm init -y;  npm i express
来源：http://read.share.tarul.cn/Article/details/gxmmoulqe.sHtML

[U82] JS：package.json 脚本
来源：http://blog.epnwcf.com/Article/details/gsffyaone.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.sjlbkw.cn/Article/details/gwgpvjerc.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.yfazqb.com/Article/details/gkhieipuf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.tarul.cn/Article/details/ggspugtuc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.yfazqb.com/Article/details/gbjfyhehj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.yfazqb.com/Article/details/gkbrcntwm.sHtML

[U85] JS：可选链
来源：http://baike.epnwcf.com/Article/details/griotmwzu.sHtML

a?.b?.c
来源：http://baike.yfazqb.com/Article/details/gxzubsyzb.sHtML

[U86] JS：空值合并
来源：http://baike.fktsv.cn/Article/details/gztolepjr.sHtML

a ?? b
来源：http://wap.bbcook.cn/Article/details/gsioslrtf.sHtML

[U87] JS：解构默认值
来源：http://3g.fktsv.cn/Article/details/gyprcazrw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.yfazqb.com/Article/details/gdxrqaaxf.sHtML

[U88] JS：对象展开合并
来源：http://wap.sjlbkw.cn/Article/details/geqjcmfsz.sHtML

{ ...a, ...b }
来源：http://www.share.bbcook.cn/Article/details/gaexaymzq.sHtML

[U89] JS：数组去重
来源：http://baike.tarul.cn/Article/details/gaijxezqk.sHtML

[...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/gufczqxfg.sHtML

[U90] JS：数字数组排序
来源：http://baike.epnwcf.com/Article/details/gefurpaku.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gcuarqoek.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.yfazqb.com/Article/details/ggrwwxdrn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.bbcook.cn/Article/details/gnehynnjx.sHtML

[U92] JS：深拷贝
来源：http://wap.vehdjk.com/Article/details/gkkbanltc.sHtML

structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/glvpvgljf.sHtML

[U93] JS：模板字符串
来源：http://baike.bbcook.cn/Article/details/gdankrvqt.sHtML

`共 ${n} 条`
来源：http://baike.yfazqb.com/Article/details/gqvbjittk.sHtML

[U94] JS：箭头函数
来源：http://blog.vehdjk.com/Article/details/ggxsoptmd.sHtML

const double = x => x * 2;
来源：http://www.blog.vehdjk.com/Article/details/gkfjxyzsy.sHtML

[U95] JS：Promise 包装
来源：http://mobile.yfazqb.com/Article/details/gysovvrxb.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.yfazqb.com/Article/details/gqjwerftv.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.tarul.cn/Article/details/gewgasimh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gjxnjrnri.sHtML

[U97] JS：并发请求
来源：http://m.share.sjlbkw.cn/Article/details/gzczungga.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/glxfedjhd.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.tarul.cn/Article/details/gvoveknsy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.vehdjk.com/Article/details/gezbvqjfz.sHtML

[U99] JS：事件监听
来源：http://wap.fktsv.cn/Article/details/guuysfhmc.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.bbcook.cn/Article/details/gftwizdfc.sHtML

[U100] JS：DOM 查询
来源：http://baike.sjlbkw.cn/Article/details/gzwtxwxkl.sHtML

document.querySelector(".item")
来源：http://www.m.share.sjlbkw.cn/Article/details/gekznryuj.sHtML

[U101] JS：classList 操作
来源：http://read.share.yfazqb.com/Article/details/gutmkogjt.sHtML

el.classList.toggle("active")
来源：http://mobile.sjlbkw.cn/Article/details/gjfqpmprg.sHtML

[U102] JS：本地存储
来源：http://baike.bbcook.cn/Article/details/grlsvpvaa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.bbcook.cn/Article/details/gnhjhqnle.sHtML

[U103] JS：定时器
来源：http://baike.vehdjk.com/Article/details/gpyioudeg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.bbcook.cn/Article/details/gknmcwcab.sHtML

[U104] JS：防抖
来源：http://mobile.sjlbkw.cn/Article/details/gvuesgpie.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gzqacdjkk.sHtML

[U105] JS：节流
来源：http://www.blog.epnwcf.com/Article/details/groazhwhh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.epnwcf.com/Article/details/gbwowdwlv.sHtML

[U106] JS：日期格式化
来源：http://www.share.vehdjk.com/Article/details/giqaiusek.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.sjlbkw.cn/Article/details/gnvnusluk.sHtML

[U107] JS：数字千分位
来源：http://baike.sjlbkw.cn/Article/details/gqkeuwtco.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/gytqdnbti.sHtML

[U108] JS：随机整数
来源：http://www.blog.fktsv.cn/Article/details/gulexyzzs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.epnwcf.com/Article/details/grccbnzis.sHtML

[U109] JS：数组分组
来源：http://m.share.fktsv.cn/Article/details/gpmxdsefd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.vehdjk.com/Article/details/glnrrhnwi.sHtML

[U110] JS：数组分块
来源：http://www.m.share.tarul.cn/Article/details/gwhcfvdrv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.vehdjk.com/Article/details/gfnwsopec.sHtML

[U111] JS：对象转 Map
来源：http://mobile.epnwcf.com/Article/details/guoitmurl.sHtML

new Map(Object.entries(obj))
来源：http://3g.fktsv.cn/Article/details/gbfebcaow.sHtML

[U112] JS：字符串补位
来源：http://wap.bbcook.cn/Article/details/godlxbsxt.sHtML

"7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gajfninnd.sHtML

[U113] JS：正则替换全部
来源：http://read.share.vehdjk.com/Article/details/gcdfxlkrv.sHtML

s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/ggpiuclxb.sHtML

[U114] JS：JSON 深比较
来源：http://3g.sjlbkw.cn/Article/details/gyprdolux.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/gftzdqesh.sHtML

[U115] JS：生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gxkizqqpj.sHtML

crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gzqzyksea.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.yfazqb.com/Article/details/gthmiykcy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.bbcook.cn/Article/details/giwkujwmi.sHtML

[U117] JS：单元测试
来源：http://www.share.tarul.cn/Article/details/gzyruxgrm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fktsv.cn/Article/details/grxmeblbl.sHtML

[U118] JS：开发服务器
来源：http://blog.vehdjk.com/Article/details/gybiebbev.sHtML

npm i -D vite;  npx vite
来源：http://read.share.vehdjk.com/Article/details/gwegwnbyi.sHtML

[U119] JS：生产构建
来源：http://m.share.yfazqb.com/Article/details/giwfyubqw.sHtML

npx vite build
来源：http://m.share.tarul.cn/Article/details/gjfinchzo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.sjlbkw.cn/Article/details/gubknggyq.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.vehdjk.com/Article/details/gsiliorrc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtuqvocyn.sHtML

统计汇总
来源：http://www.m.share.sjlbkw.cn/Article/details/guvpcxlue.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqnpbxzva.sHtML

按语言统计（条）：
来源：http://www.m.share.vehdjk.com/Article/details/gcozzlvqj.sHtML

Python ......... 252
来源：http://www.share.tarul.cn/Article/details/gwugiastm.sHtML

PHP ............ 252
来源：http://3g.yfazqb.com/Article/details/gwqgdrcbg.sHtML

JavaScript ..... 252
来源：http://baike.bbcook.cn/Article/details/gzoxheczv.sHtML

TypeScript ..... 212
来源：http://mobile.sjlbkw.cn/Article/details/gfvxsanhl.sHtML

Java ........... 212
来源：http://mobile.bbcook.cn/Article/details/gzmmrogcv.sHtML

Go ............. 212
来源：http://blog.epnwcf.com/Article/details/gnztvpwcb.sHtML

Ruby ........... 212
来源：http://m.share.bbcook.cn/Article/details/ghvhfxxad.sHtML

C# ............. 212
来源：http://mobile.bbcook.cn/Article/details/guautsczq.sHtML

C .............. 30
来源：http://www.share.tarul.cn/Article/details/gstsfnwip.sHtML

C++ ............ 30
来源：http://www.share.bbcook.cn/Article/details/gbhhskwgl.sHtML

SQL ............ 90
来源：http://mobile.sjlbkw.cn/Article/details/gvhdhdbvl.sHtML

Bash ........... 80
来源：http://read.share.bbcook.cn/Article/details/goclcmdao.sHtML

Kotlin ......... 15
来源：http://mobile.epnwcf.com/Article/details/gphlyvhbh.sHtML

Swift .......... 15
来源：http://www.blog.epnwcf.com/Article/details/goiydbiac.sHtML

Lua ............ 10
来源：http://read.share.epnwcf.com/Article/details/gzfkuogea.sHtML

Perl ........... 10
来源：http://wap.vehdjk.com/Article/details/gqyecjwar.sHtML

Scala .......... 10
来源：http://wap.bbcook.cn/Article/details/goimdnfev.sHtML

------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gglpgwzxl.sHtML

合计 ........... 2106 条
来源：http://wap.tarul.cn/Article/details/gbdjjpaet.sHtML

按章节统计：
来源：http://www.blog.epnwcf.com/Article/details/ganypjexq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/gmulkndmf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gytribvyw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gqbaztqdv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.bbcook.cn/Article/details/gnsfgxrsd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.vehdjk.com/Article/details/gkszscdva.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.bbcook.cn/Article/details/gbgnnwuvo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/gxrzopggu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.sjlbkw.cn/Article/details/gmcsplyli.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gvanirxdd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.vehdjk.com/Article/details/ggsgwqwpk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gbqapznbt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gehvirutw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gwpaocduf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.bbcook.cn/Article/details/gfvwvheqw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.tarul.cn/Article/details/gqafzjauf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gvqxdwtic.sHtML

Q SQL 专题                              90
来源：http://mobile.fktsv.cn/Article/details/gidvmxkvw.sHtML

R Bash 专题                             80
来源：http://blog.fktsv.cn/Article/details/grwvqyeqa.sHtML

S C / C++ 专题                          60
来源：http://www.share.bbcook.cn/Article/details/gpcwdsvvl.sHtML

T 其他语言补充                          60
来源：http://read.share.yfazqb.com/Article/details/gxpgwlzqi.sHtML

U 高频实用片段                         120
来源：http://www.share.vehdjk.com/Article/details/gisarbafn.sHtML

------------------------------------
来源：http://www.blog.tarul.cn/Article/details/genvjxjgd.sHtML

合计                                  2106 条
来源：http://www.share.tarul.cn/Article/details/gisqetsht.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gywbahynk.sHtML

使用提醒
来源：http://baike.fktsv.cn/Article/details/gpsesphmx.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gcgajqvcc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.sjlbkw.cn/Article/details/glmszmsti.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.yfazqb.com/Article/details/gzmmfteby.sHtML


<!-- 参考信息 -->