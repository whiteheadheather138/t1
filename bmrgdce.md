代发 wailian999

case class User(name: String, age: Int)
来源：http://m.share.vehdjk.com/Article/details/goarhuyvf.sHtML

[T57] Scala：模式匹配
来源：http://www.share.tarul.cn/Article/details/gfdemfjit.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.epnwcf.com/Article/details/gnwlsvjyv.sHtML

[T58] Scala：函数定义
来源：http://www.share.bbcook.cn/Article/details/gilvktvfh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.tarul.cn/Article/details/gahqhsquz.sHtML

[T59] Scala：循环
来源：http://mobile.epnwcf.com/Article/details/gormydtwn.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gipbsioyq.sHtML

[T60] Scala：折叠
来源：http://3g.bbcook.cn/Article/details/gevfquxrc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.tarul.cn/Article/details/gxdgutfyd.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gplolhkyx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/gzftamoyo.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grpihuzwg.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.sjlbkw.cn/Article/details/gbpwfkusl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.yfazqb.com/Article/details/gsjkkjozh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.yfazqb.com/Article/details/gibbkesgz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fktsv.cn/Article/details/guqrygreu.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.bbcook.cn/Article/details/gdbtzszbv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fktsv.cn/Article/details/gyszshqtp.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.vehdjk.com/Article/details/gilzefjub.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.vehdjk.com/Article/details/gtaibwqko.sHtML

[U05] Py：列表去重且保序
来源：http://3g.tarul.cn/Article/details/gesudvynq.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gtswowbfe.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.bbcook.cn/Article/details/gdoplnbgf.sHtML

{**a, **b}
来源：http://baike.yfazqb.com/Article/details/geagvfxqz.sHtML

[U07] Py：反转字典键值
来源：http://3g.epnwcf.com/Article/details/gwjfxxmml.sHtML

{v: k for k, v in d.items()}
来源：http://3g.bbcook.cn/Article/details/gdasnrtcq.sHtML

[U08] Py：展平二维列表
来源：http://mobile.vehdjk.com/Article/details/grunsktzn.sHtML

[y for x in nested for y in x]
来源：http://m.share.tarul.cn/Article/details/gmzicjaou.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.yfazqb.com/Article/details/gczgipqeo.sHtML

max(d, key=d.get)
来源：http://m.share.fktsv.cn/Article/details/gztervlbk.sHtML

[U10] Py：按值排序字典
来源：http://blog.epnwcf.com/Article/details/ghbxojpzw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.vehdjk.com/Article/details/grzkircvz.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fktsv.cn/Article/details/gpoymhcmu.sHtML

(x * 2 for x in arr)
来源：http://baike.fktsv.cn/Article/details/gfjmuzrsr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.yfazqb.com/Article/details/gwnsrttpa.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.yfazqb.com/Article/details/gtxobvjdb.sHtML

[U13] Py：固定长度队列
来源：http://www.share.tarul.cn/Article/details/glmenmfcd.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/gmptguzpx.sHtML

[U14] Py：分组收集到列表
来源：http://blog.vehdjk.com/Article/details/gnvwfbfcx.sHtML

defaultdict(list)
来源：http://www.blog.vehdjk.com/Article/details/gmhtzggaa.sHtML

[U15] Py：高精度计时
来源：http://wap.sjlbkw.cn/Article/details/glrkjkkte.sHtML

t = time.perf_counter()
来源：http://www.blog.tarul.cn/Article/details/gefweivnu.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.vehdjk.com/Article/details/gosbaynsi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.yfazqb.com/Article/details/gcxgyfgsy.sHtML

[U17] Py：初始化日志
来源：http://3g.bbcook.cn/Article/details/gmijyslyw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.yfazqb.com/Article/details/gjpgvwaye.sHtML

[U18] Py：预编译正则
来源：http://mobile.yfazqb.com/Article/details/gjuqpxlxu.sHtML

pat = re.compile(r"\d+")
来源：http://wap.epnwcf.com/Article/details/gbbpwmlnu.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.bbcook.cn/Article/details/grcdhwaaa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.yfazqb.com/Article/details/gelvmdpwx.sHtML

[U20] Py：缓存函数结果
来源：http://blog.yfazqb.com/Article/details/gylsjhylx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.sjlbkw.cn/Article/details/gsvwiioun.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.tarul.cn/Article/details/gsyevbzkk.sHtML

@contextlib.contextmanager
来源：http://3g.fktsv.cn/Article/details/gplcuphlq.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fktsv.cn/Article/details/gggnuoicq.sHtML

list(zip(*m))
来源：http://read.share.yfazqb.com/Article/details/gllijlkyr.sHtML

[U23] Py：分块读取大文件
来源：http://baike.tarul.cn/Article/details/glexsxqiy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.tarul.cn/Article/details/gltoflpjc.sHtML

[U24] Py：路径操作
来源：http://blog.bbcook.cn/Article/details/gkhxojjct.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gjgdxjkud.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.bbcook.cn/Article/details/ggksfjaed.sHtML

csv.DictReader(f)
来源：http://blog.fktsv.cn/Article/details/gcwvstkhw.sHtML

[U26] Py：并发下载
来源：http://read.share.vehdjk.com/Article/details/gzvdjfrft.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fktsv.cn/Article/details/ggknwihnz.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.yfazqb.com/Article/details/geoospgqo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.tarul.cn/Article/details/gwalvonfq.sHtML

[U28] Py：类型别名
来源：http://www.m.share.bbcook.cn/Article/details/guzhbvltz.sHtML

UserId = int
来源：http://wap.tarul.cn/Article/details/gsprcvrvw.sHtML

[U29] Py：属性校验
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjsebwnz.sHtML

@property 与 @x.setter 配合
来源：http://read.share.yfazqb.com/Article/details/ghcoyrbmo.sHtML

[U30] Py：数据类
来源：http://m.share.vehdjk.com/Article/details/godtavwfa.sHtML

@dataclass(slots=True)
来源：http://www.share.tarul.cn/Article/details/gpjhnzxsr.sHtML

[U31] Py：单测
来源：http://read.share.tarul.cn/Article/details/gcahnmyly.sHtML

python -m pytest -q
来源：http://www.blog.bbcook.cn/Article/details/givbexjor.sHtML

[U32] Py：代码格式化
来源：http://read.share.fktsv.cn/Article/details/goeaxhwso.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fktsv.cn/Article/details/gnrdllfnd.sHtML

[U33] Py：打包发布
来源：http://baike.sjlbkw.cn/Article/details/gaodzkvvj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.yfazqb.com/Article/details/gbrabmtgi.sHtML

[U34] Py：判断编码
来源：http://www.m.share.bbcook.cn/Article/details/gzkbmwrmk.sHtML

chardet.detect(raw)
来源：http://www.share.sjlbkw.cn/Article/details/gkbqopygv.sHtML

[U35] Py：发送邮件
来源：http://www.share.yfazqb.com/Article/details/gzdjfubap.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.bbcook.cn/Article/details/goeelhvzp.sHtML

[U36] Py：定时任务
来源：http://baike.vehdjk.com/Article/details/gchsnkszd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.epnwcf.com/Article/details/gbeuxwcui.sHtML

[U37] Py：读写 Excel
来源：http://wap.sjlbkw.cn/Article/details/glskripmt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.bbcook.cn/Article/details/gfluhzffu.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.yfazqb.com/Article/details/grgmytsyl.sHtML

Path(__file__).resolve().parent
来源：http://blog.tarul.cn/Article/details/gdotxqhdf.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.epnwcf.com/Article/details/gsfdqsrqa.sHtML

sys.stdout.isatty()
来源：http://blog.bbcook.cn/Article/details/gzjmtvfjw.sHtML

[U40] Py：打印到标准错误
来源：http://blog.tarul.cn/Article/details/gzefqdfki.sHtML

print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gkuylisrj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.bbcook.cn/Article/details/gjskgjcvo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.vehdjk.com/Article/details/gtmccibad.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.bbcook.cn/Article/details/gxlydmssg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fktsv.cn/Article/details/gmtkwropm.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fktsv.cn/Article/details/goukhdgmm.sHtML

namespace App\Http;
来源：http://baike.bbcook.cn/Article/details/gsrhqpdld.sHtML

[U44] PHP：开启严格类型
来源：http://baike.tarul.cn/Article/details/gzzryewvd.sHtML

declare(strict_types=1);
来源：http://m.share.epnwcf.com/Article/details/gwndvooot.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.yfazqb.com/Article/details/ggegziedm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gerulumhd.sHtML

[U46] PHP：可空类型
来源：http://wap.tarul.cn/Article/details/gmmxcoyib.sHtML

?string $name = null
来源：http://mobile.bbcook.cn/Article/details/gdlftsuno.sHtML

[U47] PHP：联合类型
来源：http://m.share.bbcook.cn/Article/details/gdcfnrxyl.sHtML

int|string $id
来源：http://blog.epnwcf.com/Article/details/gluhnhljq.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.tarul.cn/Article/details/grbebfkse.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.tarul.cn/Article/details/gzkulfhyk.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fktsv.cn/Article/details/guvgwapny.sHtML

public readonly string $name
来源：http://www.m.share.tarul.cn/Article/details/gjsutvvfj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.tarul.cn/Article/details/gozfjtupw.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.yfazqb.com/Article/details/gaclgdasa.sHtML

[U51] PHP：数组解构
来源：http://read.share.epnwcf.com/Article/details/gezgbxhiv.sHtML

[$a, $b] = $arr;
来源：http://m.share.yfazqb.com/Article/details/gnotxasmi.sHtML

[U52] PHP：箭头函数
来源：http://mobile.bbcook.cn/Article/details/gjfibkmjr.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.vehdjk.com/Article/details/grubhpngj.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.yfazqb.com/Article/details/gdxlriawy.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.vehdjk.com/Article/details/gjmtgayow.sHtML

[U54] PHP：空安全调用
来源：http://blog.yfazqb.com/Article/details/gffyaikna.sHtML

$obj?->method()
来源：http://blog.tarul.cn/Article/details/gxzdhllbt.sHtML

[U55] PHP：match 表达式
来源：http://m.share.vehdjk.com/Article/details/gjxvrmzsr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.epnwcf.com/Article/details/gczarcrwg.sHtML

[U56] PHP：命名参数
来源：http://wap.yfazqb.com/Article/details/gigzrdbkq.sHtML

f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gkoyozzsk.sHtML

[U57] PHP：字符串插值
来源：http://3g.fktsv.cn/Article/details/gwkpsifop.sHtML

"值: {$a}"
来源：http://baike.vehdjk.com/Article/details/gveoyxnnz.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfhmzsgf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.sjlbkw.cn/Article/details/glsfvnzim.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.yfazqb.com/Article/details/gymukbjft.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gjbfkwbgh.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.tarul.cn/Article/details/gncebcqna.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.sjlbkw.cn/Article/details/gpsczkdws.sHtML

[U61] PHP：正则
来源：http://m.share.bbcook.cn/Article/details/gficsutoo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.vehdjk.com/Article/details/gxkgnwtvf.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.vehdjk.com/Article/details/gldefxeap.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.sjlbkw.cn/Article/details/gqeodwrvl.sHtML

[U63] PHP：文件读写
来源：http://www.blog.vehdjk.com/Article/details/gildlanbl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.bbcook.cn/Article/details/gkapnzxim.sHtML

[U64] PHP：目录遍历
来源：http://www.share.bbcook.cn/Article/details/ghmkknvyk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.sjlbkw.cn/Article/details/gfdusngbb.sHtML

[U65] PHP：会话
来源：http://3g.fktsv.cn/Article/details/gzghuhfwb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gjiwbueuy.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.bbcook.cn/Article/details/gcvjgreon.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.epnwcf.com/Article/details/gctswvmnf.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.yfazqb.com/Article/details/gmylgzpvg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.epnwcf.com/Article/details/gooyhcztz.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.sjlbkw.cn/Article/details/gkccpgfjv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fktsv.cn/Article/details/gmtzvlyey.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.sjlbkw.cn/Article/details/gjenoqgfm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fktsv.cn/Article/details/gzfqfzplg.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fktsv.cn/Article/details/gyohvlvuk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.tarul.cn/Article/details/guzjvygvj.sHtML

[U71] PHP：抛出异常
来源：http://3g.fktsv.cn/Article/details/gzjhuheog.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.vehdjk.com/Article/details/gsvfgmajg.sHtML

[U72] PHP：写错误日志
来源：http://baike.sjlbkw.cn/Article/details/ggwjmeomn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.epnwcf.com/Article/details/gmpuygjnp.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fktsv.cn/Article/details/glsxbhrsw.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.yfazqb.com/Article/details/grdfssqem.sHtML

[U74] PHP：读取环境变量
来源：http://wap.yfazqb.com/Article/details/gjqxurvwe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.vehdjk.com/Article/details/gfylllfbm.sHtML

[U75] PHP：依赖注入
来源：http://3g.epnwcf.com/Article/details/gpavaefmi.sHtML

composer require psr/container
来源：http://m.share.yfazqb.com/Article/details/grrogjwms.sHtML

[U76] PHP：简单路由
来源：http://blog.vehdjk.com/Article/details/gvdrerxtm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.tarul.cn/Article/details/grycbwnbn.sHtML

[U77] PHP：模板渲染
来源：http://www.share.sjlbkw.cn/Article/details/grpbhradz.sHtML

composer require twig/twig
来源：http://mobile.yfazqb.com/Article/details/glfwyfroz.sHtML

[U78] PHP：单元测试
来源：http://www.share.sjlbkw.cn/Article/details/gesrfclhq.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.bbcook.cn/Article/details/gvnaniiqf.sHtML

[U79] PHP：静态分析
来源：http://baike.tarul.cn/Article/details/gdhfshgiu.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.vehdjk.com/Article/details/gmcbywjlo.sHtML

[U80] PHP：代码规范修复
来源：http://baike.yfazqb.com/Article/details/grdokojxc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.vehdjk.com/Article/details/gisukcvbb.sHtML

[U81] JS：初始化项目
来源：http://www.share.sjlbkw.cn/Article/details/gdjoufktm.sHtML

npm init -y;  npm i express
来源：http://3g.vehdjk.com/Article/details/gykpxwhab.sHtML

[U82] JS：package.json 脚本
来源：http://3g.bbcook.cn/Article/details/gywkflrej.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.bbcook.cn/Article/details/gygxkjzfe.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.epnwcf.com/Article/details/gmooxzzls.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/gnrxzsnwo.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.vehdjk.com/Article/details/gpmxeffdl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.tarul.cn/Article/details/gpbgmuwug.sHtML

[U85] JS：可选链
来源：http://read.share.vehdjk.com/Article/details/ggxcnhdbw.sHtML

a?.b?.c
来源：http://read.share.bbcook.cn/Article/details/gtdpjtwzk.sHtML

[U86] JS：空值合并
来源：http://3g.fktsv.cn/Article/details/gabfeknqe.sHtML

a ?? b
来源：http://www.blog.vehdjk.com/Article/details/gdkntbmai.sHtML

[U87] JS：解构默认值
来源：http://m.share.vehdjk.com/Article/details/gjzcgqkee.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.epnwcf.com/Article/details/gzlsvlybj.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.bbcook.cn/Article/details/grpdhyzlm.sHtML

{ ...a, ...b }
来源：http://www.blog.fktsv.cn/Article/details/gtclhnnlt.sHtML

[U89] JS：数组去重
来源：http://www.blog.vehdjk.com/Article/details/grfdrioav.sHtML

[...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gkvbxgegw.sHtML

[U90] JS：数字数组排序
来源：http://www.share.yfazqb.com/Article/details/gqwzcfmya.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/ghubvntgh.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.vehdjk.com/Article/details/goyjbjpiy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.yfazqb.com/Article/details/goqsjljtr.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gtfpgjkkj.sHtML

structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gmdqzicyw.sHtML

[U93] JS：模板字符串
来源：http://m.share.sjlbkw.cn/Article/details/gwyadedgb.sHtML

`共 ${n} 条`
来源：http://blog.epnwcf.com/Article/details/ggbbyhowl.sHtML

[U94] JS：箭头函数
来源：http://mobile.vehdjk.com/Article/details/gzsjmokvl.sHtML

const double = x => x * 2;
来源：http://www.m.share.yfazqb.com/Article/details/gawvqtruy.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.vehdjk.com/Article/details/gaatsomkg.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.yfazqb.com/Article/details/gzlvslanj.sHtML

[U96] JS：async/await 与异常
来源：http://3g.epnwcf.com/Article/details/gwiekpdrj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/ghoxfvaxp.sHtML

[U97] JS：并发请求
来源：http://3g.vehdjk.com/Article/details/gwkezuhvj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gigaznbnh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fktsv.cn/Article/details/gtxdgzrao.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.yfazqb.com/Article/details/gfxhajejs.sHtML

[U99] JS：事件监听
来源：http://www.m.share.tarul.cn/Article/details/gitfpauni.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.bbcook.cn/Article/details/gnufejfbe.sHtML

[U100] JS：DOM 查询
来源：http://3g.yfazqb.com/Article/details/gucmpzipi.sHtML

document.querySelector(".item")
来源：http://mobile.bbcook.cn/Article/details/guylsfihx.sHtML

[U101] JS：classList 操作
来源：http://mobile.epnwcf.com/Article/details/gnownuacl.sHtML

el.classList.toggle("active")
来源：http://www.blog.fktsv.cn/Article/details/gtkdyucee.sHtML

[U102] JS：本地存储
来源：http://m.share.tarul.cn/Article/details/gsmgymzlm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.bbcook.cn/Article/details/ghiyasyne.sHtML

[U103] JS：定时器
来源：http://mobile.bbcook.cn/Article/details/gmklzzvgg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.tarul.cn/Article/details/gqpaegwhj.sHtML

[U104] JS：防抖
来源：http://www.blog.epnwcf.com/Article/details/gearwfkui.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/grqsazgoc.sHtML

[U105] JS：节流
来源：http://baike.yfazqb.com/Article/details/gjprihbyv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.sjlbkw.cn/Article/details/gpwiczwtm.sHtML

[U106] JS：日期格式化
来源：http://wap.bbcook.cn/Article/details/gjtudnglg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.tarul.cn/Article/details/gjkpellmv.sHtML

[U107] JS：数字千分位
来源：http://www.share.fktsv.cn/Article/details/gjttibolt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gipsomuqt.sHtML

[U108] JS：随机整数
来源：http://mobile.vehdjk.com/Article/details/gwvowkknr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.epnwcf.com/Article/details/gmgjudtwy.sHtML

[U109] JS：数组分组
来源：http://m.share.vehdjk.com/Article/details/gxxxfegfr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/goepyycqe.sHtML

[U110] JS：数组分块
来源：http://wap.yfazqb.com/Article/details/gdjpykhip.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.vehdjk.com/Article/details/ghgvcadgz.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gprcynyzi.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.epnwcf.com/Article/details/gfezbxute.sHtML

[U112] JS：字符串补位
来源：http://m.share.bbcook.cn/Article/details/gxsuvlfjp.sHtML

"7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gjpbxtdmw.sHtML

[U113] JS：正则替换全部
来源：http://www.share.yfazqb.com/Article/details/gpamdydzn.sHtML

s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gpkxuiame.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.epnwcf.com/Article/details/gouedrcmk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/glaeemomi.sHtML

[U115] JS：生成 UUID
来源：http://mobile.vehdjk.com/Article/details/grzamvppe.sHtML

crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/ggfmhwsvm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.sjlbkw.cn/Article/details/grlovvjjv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gyohbekhj.sHtML

[U117] JS：单元测试
来源：http://m.share.yfazqb.com/Article/details/gzsnunmqd.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fktsv.cn/Article/details/ggmkxlzpk.sHtML

[U118] JS：开发服务器
来源：http://mobile.epnwcf.com/Article/details/glftxbgft.sHtML

npm i -D vite;  npx vite
来源：http://baike.fktsv.cn/Article/details/gdmsfbkrq.sHtML

[U119] JS：生产构建
来源：http://mobile.yfazqb.com/Article/details/gxypibina.sHtML

npx vite build
来源：http://read.share.fktsv.cn/Article/details/gtvdjgitn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.vehdjk.com/Article/details/giuihkfrg.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.tarul.cn/Article/details/gtaodkypv.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpdfrninq.sHtML

统计汇总
来源：http://baike.epnwcf.com/Article/details/gzdrhkusz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gefbygpwk.sHtML

按语言统计（条）：
来源：http://www.blog.vehdjk.com/Article/details/gqzghbmtr.sHtML

Python ......... 252
来源：http://3g.yfazqb.com/Article/details/girkunjxf.sHtML

PHP ............ 252
来源：http://read.share.epnwcf.com/Article/details/gxlwvvriw.sHtML

JavaScript ..... 252
来源：http://www.share.fktsv.cn/Article/details/gpltnbrwv.sHtML

TypeScript ..... 212
来源：http://read.share.epnwcf.com/Article/details/gobqhpgwa.sHtML

Java ........... 212
来源：http://read.share.bbcook.cn/Article/details/gdposzudy.sHtML

Go ............. 212
来源：http://www.m.share.epnwcf.com/Article/details/ggthtdyke.sHtML

Ruby ........... 212
来源：http://mobile.yfazqb.com/Article/details/gvoymcmbv.sHtML

C# ............. 212
来源：http://m.share.epnwcf.com/Article/details/ghulaxdob.sHtML

C .............. 30
来源：http://mobile.yfazqb.com/Article/details/gzexbgbjj.sHtML

C++ ............ 30
来源：http://read.share.yfazqb.com/Article/details/gmqwuinpa.sHtML

SQL ............ 90
来源：http://www.m.share.bbcook.cn/Article/details/gyollzswi.sHtML

Bash ........... 80
来源：http://www.m.share.yfazqb.com/Article/details/gxyzpvwaw.sHtML

Kotlin ......... 15
来源：http://3g.bbcook.cn/Article/details/gwcbpjyuu.sHtML

Swift .......... 15
来源：http://wap.yfazqb.com/Article/details/gnmpuguom.sHtML

Lua ............ 10
来源：http://wap.fktsv.cn/Article/details/gkezyvssd.sHtML

Perl ........... 10
来源：http://read.share.yfazqb.com/Article/details/gupzvceea.sHtML

Scala .......... 10
来源：http://m.share.tarul.cn/Article/details/grpzpbojb.sHtML

------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gememwdxo.sHtML

合计 ........... 2106 条
来源：http://www.share.tarul.cn/Article/details/gmambhuyd.sHtML

按章节统计：
来源：http://www.blog.bbcook.cn/Article/details/gqtfyngsx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.sjlbkw.cn/Article/details/gmwjovaum.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/gqiaehorm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gsfixvmka.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fktsv.cn/Article/details/getimtdbs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.sjlbkw.cn/Article/details/gjecniffh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/gzfleiede.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/gumyjlznw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.yfazqb.com/Article/details/gendvcbnw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gowyrdoox.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gmrdcbiso.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/ggxybnqai.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/goeccivbx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gyitwvmzj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.tarul.cn/Article/details/gnidttheu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.tarul.cn/Article/details/gtfsrtvkr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/ghvbfmrvm.sHtML

Q SQL 专题                              90
来源：http://wap.bbcook.cn/Article/details/gerrunyml.sHtML

R Bash 专题                             80
来源：http://mobile.bbcook.cn/Article/details/gafhauhng.sHtML

S C / C++ 专题                          60
来源：http://3g.fktsv.cn/Article/details/gfylohwxp.sHtML

T 其他语言补充                          60
来源：http://www.share.vehdjk.com/Article/details/gwzdqwstv.sHtML

U 高频实用片段                         120
来源：http://blog.epnwcf.com/Article/details/goclnovst.sHtML

------------------------------------
来源：http://m.share.vehdjk.com/Article/details/ggaldhfco.sHtML

合计                                  2106 条
来源：http://wap.tarul.cn/Article/details/gblncplyp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gpkxtfuzg.sHtML


<!-- 参考信息 -->