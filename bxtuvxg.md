代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.bbcook.cn/Article/details/gadtmnwji.sHtML

[T59] Scala：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gyghmhwzi.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gwguqhvrd.sHtML

[T60] Scala：折叠
来源：http://mobile.sjlbkw.cn/Article/details/gyiddwfcb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.tarul.cn/Article/details/gcxzuawak.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gdwzrqvcw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/gxsfwppuv.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gtbkkkodo.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.yfazqb.com/Article/details/gklxlkvjr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.tarul.cn/Article/details/gdctfpwjr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fktsv.cn/Article/details/gsokpandg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.sjlbkw.cn/Article/details/gvjagxrbn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.bbcook.cn/Article/details/ggmlsxsen.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fktsv.cn/Article/details/gynsyhyqr.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.tarul.cn/Article/details/ghnmnjnni.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.vehdjk.com/Article/details/gjivjtmnp.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/goolvyavj.sHtML

list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/gzfutjrux.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.yfazqb.com/Article/details/gkotlxlax.sHtML

{**a, **b}
来源：http://mobile.sjlbkw.cn/Article/details/gfpoqdlwi.sHtML

[U07] Py：反转字典键值
来源：http://mobile.sjlbkw.cn/Article/details/guygogrkz.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.tarul.cn/Article/details/gnvwoqknh.sHtML

[U08] Py：展平二维列表
来源：http://read.share.bbcook.cn/Article/details/gxrglhqyu.sHtML

[y for x in nested for y in x]
来源：http://mobile.yfazqb.com/Article/details/gvpxjdzkd.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fktsv.cn/Article/details/gbimgbkxd.sHtML

max(d, key=d.get)
来源：http://blog.fktsv.cn/Article/details/gvcdqmaqm.sHtML

[U10] Py：按值排序字典
来源：http://wap.yfazqb.com/Article/details/gybqnfhvj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.epnwcf.com/Article/details/glbysokiu.sHtML

[U11] Py：生成器表达式
来源：http://wap.bbcook.cn/Article/details/grsvuoacn.sHtML

(x * 2 for x in arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gdtrdmzvr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.epnwcf.com/Article/details/gzdkddhhi.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/gqdgmskfp.sHtML

[U13] Py：固定长度队列
来源：http://3g.sjlbkw.cn/Article/details/gyvhgsloi.sHtML

deque(maxlen=10)
来源：http://3g.sjlbkw.cn/Article/details/ghpbpbnwm.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.bbcook.cn/Article/details/ggerisaxq.sHtML

defaultdict(list)
来源：http://m.share.vehdjk.com/Article/details/gaczkdryz.sHtML

[U15] Py：高精度计时
来源：http://3g.vehdjk.com/Article/details/gmuxkvikv.sHtML

t = time.perf_counter()
来源：http://m.share.yfazqb.com/Article/details/geqgnhioi.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.vehdjk.com/Article/details/gdaaqqbpd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.sjlbkw.cn/Article/details/ganmegtoo.sHtML

[U17] Py：初始化日志
来源：http://blog.vehdjk.com/Article/details/gsigkkcbs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fktsv.cn/Article/details/gawlqqzyw.sHtML

[U18] Py：预编译正则
来源：http://blog.tarul.cn/Article/details/gxhxbntfd.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.sjlbkw.cn/Article/details/gqdalumnl.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.tarul.cn/Article/details/gpjirzjyb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.vehdjk.com/Article/details/ghikupaja.sHtML

[U20] Py：缓存函数结果
来源：http://wap.epnwcf.com/Article/details/genlatajp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.sjlbkw.cn/Article/details/gexwfktis.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.yfazqb.com/Article/details/gcjmtjqar.sHtML

@contextlib.contextmanager
来源：http://read.share.vehdjk.com/Article/details/gimnqluzq.sHtML

[U22] Py：矩阵转置
来源：http://blog.yfazqb.com/Article/details/gnapkprzf.sHtML

list(zip(*m))
来源：http://read.share.tarul.cn/Article/details/garnufinr.sHtML

[U23] Py：分块读取大文件
来源：http://baike.sjlbkw.cn/Article/details/gydutydms.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fktsv.cn/Article/details/gtsqemylu.sHtML

[U24] Py：路径操作
来源：http://www.m.share.bbcook.cn/Article/details/gwswdfktm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/gzweiebna.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.yfazqb.com/Article/details/guxmqkmaz.sHtML

csv.DictReader(f)
来源：http://read.share.sjlbkw.cn/Article/details/gndydpiws.sHtML

[U26] Py：并发下载
来源：http://www.blog.vehdjk.com/Article/details/gbwyfgqbw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.bbcook.cn/Article/details/gtdsvhxgb.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.sjlbkw.cn/Article/details/gqqqzpcpt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.tarul.cn/Article/details/gqldolxke.sHtML

[U28] Py：类型别名
来源：http://blog.tarul.cn/Article/details/gyvlmgxfr.sHtML

UserId = int
来源：http://m.share.vehdjk.com/Article/details/gfmzezldj.sHtML

[U29] Py：属性校验
来源：http://read.share.epnwcf.com/Article/details/goolwqhje.sHtML

@property 与 @x.setter 配合
来源：http://wap.bbcook.cn/Article/details/gcjetrfnj.sHtML

[U30] Py：数据类
来源：http://m.share.epnwcf.com/Article/details/gqtmuyhwu.sHtML

@dataclass(slots=True)
来源：http://read.share.yfazqb.com/Article/details/guebkqoqf.sHtML

[U31] Py：单测
来源：http://wap.epnwcf.com/Article/details/ghtyjbttz.sHtML

python -m pytest -q
来源：http://read.share.sjlbkw.cn/Article/details/gkzypxzbr.sHtML

[U32] Py：代码格式化
来源：http://m.share.tarul.cn/Article/details/gbxwmbjbp.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.yfazqb.com/Article/details/grakxrulb.sHtML

[U33] Py：打包发布
来源：http://read.share.sjlbkw.cn/Article/details/gblrtgxni.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.sjlbkw.cn/Article/details/gzygmated.sHtML

[U34] Py：判断编码
来源：http://3g.yfazqb.com/Article/details/gspntdzig.sHtML

chardet.detect(raw)
来源：http://wap.yfazqb.com/Article/details/gdfydpgep.sHtML

[U35] Py：发送邮件
来源：http://m.share.epnwcf.com/Article/details/guxfnwrdv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.epnwcf.com/Article/details/gpvtxawgr.sHtML

[U36] Py：定时任务
来源：http://www.m.share.tarul.cn/Article/details/grrcbvyjq.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.epnwcf.com/Article/details/gerhhxafn.sHtML

[U37] Py：读写 Excel
来源：http://read.share.vehdjk.com/Article/details/gjwfxiuyn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.vehdjk.com/Article/details/gebpwdphc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fktsv.cn/Article/details/gtzqzkgth.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.epnwcf.com/Article/details/goxtikzqg.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fktsv.cn/Article/details/gfhecbwes.sHtML

sys.stdout.isatty()
来源：http://m.share.vehdjk.com/Article/details/ghuepfquj.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fktsv.cn/Article/details/gotapznvj.sHtML

print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gpzppyerc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fktsv.cn/Article/details/gfwjechos.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsbxwzee.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.bbcook.cn/Article/details/gftztkjzq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.epnwcf.com/Article/details/gsxffuzqq.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.bbcook.cn/Article/details/gipohywca.sHtML

namespace App\Http;
来源：http://blog.epnwcf.com/Article/details/gcigdldgn.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.sjlbkw.cn/Article/details/gfkawdufj.sHtML

declare(strict_types=1);
来源：http://www.blog.sjlbkw.cn/Article/details/gmlfeuhrv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.tarul.cn/Article/details/glfywdfwj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gaqqxakfs.sHtML

[U46] PHP：可空类型
来源：http://www.share.vehdjk.com/Article/details/glecqnaxf.sHtML

?string $name = null
来源：http://read.share.fktsv.cn/Article/details/gqnymgkan.sHtML

[U47] PHP：联合类型
来源：http://read.share.sjlbkw.cn/Article/details/gydfpybui.sHtML

int|string $id
来源：http://m.share.tarul.cn/Article/details/gljzkprsl.sHtML

[U48] PHP：纯枚举
来源：http://www.share.yfazqb.com/Article/details/gnngztnaa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.epnwcf.com/Article/details/gxmmqszey.sHtML

[U49] PHP：只读属性
来源：http://mobile.bbcook.cn/Article/details/gwvbvdzgf.sHtML

public readonly string $name
来源：http://www.blog.epnwcf.com/Article/details/gndqreisj.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.vehdjk.com/Article/details/gyltrwjhv.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fktsv.cn/Article/details/gabemeomy.sHtML

[U51] PHP：数组解构
来源：http://read.share.epnwcf.com/Article/details/gxvvcxdhl.sHtML

[$a, $b] = $arr;
来源：http://blog.epnwcf.com/Article/details/gqyusrfpj.sHtML

[U52] PHP：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gxqbpzkfi.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.vehdjk.com/Article/details/gkevrenmz.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fktsv.cn/Article/details/gjkafcypa.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.yfazqb.com/Article/details/gbsgijqka.sHtML

[U54] PHP：空安全调用
来源：http://baike.tarul.cn/Article/details/ghbxhwiwy.sHtML

$obj?->method()
来源：http://www.share.bbcook.cn/Article/details/ggdossawf.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fktsv.cn/Article/details/gllhishvs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.tarul.cn/Article/details/gpmldfvzl.sHtML

[U56] PHP：命名参数
来源：http://blog.sjlbkw.cn/Article/details/ggixfocqm.sHtML

f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gfgwrvnba.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gcjbvbwhh.sHtML

"值: {$a}"
来源：http://www.m.share.yfazqb.com/Article/details/gjrrvvnvc.sHtML

[U58] PHP：数组三件套
来源：http://www.share.bbcook.cn/Article/details/gpzahmcam.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.vehdjk.com/Article/details/gufckytff.sHtML

[U59] PHP：自定义排序
来源：http://www.share.vehdjk.com/Article/details/gycdpcbon.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/gfmltpepu.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.sjlbkw.cn/Article/details/gftqvahof.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.yfazqb.com/Article/details/ggffpqyfy.sHtML

[U61] PHP：正则
来源：http://mobile.fktsv.cn/Article/details/ghvnzhgof.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/glnhquego.sHtML

[U62] PHP：日期对象
来源：http://mobile.sjlbkw.cn/Article/details/gqquozxkb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.sjlbkw.cn/Article/details/giwyjamje.sHtML

[U63] PHP：文件读写
来源：http://mobile.bbcook.cn/Article/details/gxxywuoyl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fktsv.cn/Article/details/gtzkphubl.sHtML

[U64] PHP：目录遍历
来源：http://3g.bbcook.cn/Article/details/gcssqhtfi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.yfazqb.com/Article/details/gzjcysgow.sHtML

[U65] PHP：会话
来源：http://www.share.vehdjk.com/Article/details/gewmbwbow.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gsypautwl.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxjtbqdj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fktsv.cn/Article/details/ghsyqihoq.sHtML

[U67] PHP：处理文件上传
来源：http://wap.epnwcf.com/Article/details/gjkxkimdj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.epnwcf.com/Article/details/gvifgghvl.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhnwstot.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.tarul.cn/Article/details/gncasgwee.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.tarul.cn/Article/details/glewezgxh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.vehdjk.com/Article/details/gkebydffr.sHtML

[U70] PHP：PDO 事务
来源：http://blog.sjlbkw.cn/Article/details/gzdjuhdzf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fktsv.cn/Article/details/gvtydfwun.sHtML

[U71] PHP：抛出异常
来源：http://3g.vehdjk.com/Article/details/gmtdcendv.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.yfazqb.com/Article/details/gqelxdnmh.sHtML

[U72] PHP：写错误日志
来源：http://www.share.epnwcf.com/Article/details/gpzxuddgc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fktsv.cn/Article/details/gdhcfrezb.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.tarul.cn/Article/details/gqgeihxbu.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.yfazqb.com/Article/details/gfenmunnx.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gjwovfqsc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.epnwcf.com/Article/details/gmjxxvvel.sHtML

[U75] PHP：依赖注入
来源：http://www.share.vehdjk.com/Article/details/geregpzmc.sHtML

composer require psr/container
来源：http://read.share.sjlbkw.cn/Article/details/gshwghxxz.sHtML

[U76] PHP：简单路由
来源：http://m.share.vehdjk.com/Article/details/gralkxctz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.vehdjk.com/Article/details/gstmyzdvz.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.vehdjk.com/Article/details/gqucijxvk.sHtML

composer require twig/twig
来源：http://www.blog.sjlbkw.cn/Article/details/gskmmomos.sHtML

[U78] PHP：单元测试
来源：http://3g.fktsv.cn/Article/details/gylyestkv.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.yfazqb.com/Article/details/gaudckjbw.sHtML

[U79] PHP：静态分析
来源：http://www.blog.epnwcf.com/Article/details/ghardowui.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.epnwcf.com/Article/details/gkweftvim.sHtML

[U80] PHP：代码规范修复
来源：http://3g.sjlbkw.cn/Article/details/gevqdkmwg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.vehdjk.com/Article/details/gezcepltc.sHtML

[U81] JS：初始化项目
来源：http://m.share.sjlbkw.cn/Article/details/gpbydbjuf.sHtML

npm init -y;  npm i express
来源：http://www.share.tarul.cn/Article/details/grlpbdook.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.epnwcf.com/Article/details/gblrawtik.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.epnwcf.com/Article/details/geczlbffr.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fktsv.cn/Article/details/gcyqzcort.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gdsliuakp.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.vehdjk.com/Article/details/gqlrgtvcr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.epnwcf.com/Article/details/gxoeantxe.sHtML

[U85] JS：可选链
来源：http://mobile.sjlbkw.cn/Article/details/gaussmcen.sHtML

a?.b?.c
来源：http://read.share.fktsv.cn/Article/details/gqyolzukm.sHtML

[U86] JS：空值合并
来源：http://m.share.fktsv.cn/Article/details/gestlsnec.sHtML

a ?? b
来源：http://baike.bbcook.cn/Article/details/gwrpckswz.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.yfazqb.com/Article/details/gsnrpzgof.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.tarul.cn/Article/details/gezebhwky.sHtML

[U88] JS：对象展开合并
来源：http://wap.yfazqb.com/Article/details/grufsiiue.sHtML

{ ...a, ...b }
来源：http://3g.sjlbkw.cn/Article/details/gmzgschwq.sHtML

[U89] JS：数组去重
来源：http://3g.fktsv.cn/Article/details/gbqppsepp.sHtML

[...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gkgwuqoze.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.epnwcf.com/Article/details/gxwcqmdit.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/ghnxvjleb.sHtML

[U91] JS：对象键值遍历
来源：http://3g.bbcook.cn/Article/details/gnovsqtqi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.sjlbkw.cn/Article/details/gjflbasok.sHtML

[U92] JS：深拷贝
来源：http://blog.yfazqb.com/Article/details/gkparjbpw.sHtML

structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gjshudoke.sHtML

[U93] JS：模板字符串
来源：http://3g.epnwcf.com/Article/details/gvvelrarx.sHtML

`共 ${n} 条`
来源：http://mobile.sjlbkw.cn/Article/details/gmkkpgxzi.sHtML

[U94] JS：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gvuqguoxq.sHtML

const double = x => x * 2;
来源：http://mobile.tarul.cn/Article/details/guvczvgmc.sHtML

[U95] JS：Promise 包装
来源：http://blog.fktsv.cn/Article/details/gsfkybwxc.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.sjlbkw.cn/Article/details/gdhwnvdip.sHtML

[U96] JS：async/await 与异常
来源：http://blog.sjlbkw.cn/Article/details/gzfkxgtgo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/goffpluzs.sHtML

[U97] JS：并发请求
来源：http://mobile.fktsv.cn/Article/details/glgvrkpps.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gwxunvqit.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.bbcook.cn/Article/details/gxcqbnpnv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.sjlbkw.cn/Article/details/gaymtuiom.sHtML

[U99] JS：事件监听
来源：http://www.blog.fktsv.cn/Article/details/gcujszwgl.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.bbcook.cn/Article/details/gionuwmre.sHtML

[U100] JS：DOM 查询
来源：http://www.share.yfazqb.com/Article/details/gfjuongyh.sHtML

document.querySelector(".item")
来源：http://blog.epnwcf.com/Article/details/gtkbzzwnk.sHtML

[U101] JS：classList 操作
来源：http://mobile.tarul.cn/Article/details/ganumgvly.sHtML

el.classList.toggle("active")
来源：http://mobile.tarul.cn/Article/details/gvkocqkkj.sHtML

[U102] JS：本地存储
来源：http://m.share.vehdjk.com/Article/details/gnyrsbfcx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.tarul.cn/Article/details/gtavprnyz.sHtML

[U103] JS：定时器
来源：http://read.share.fktsv.cn/Article/details/gazeslxra.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.sjlbkw.cn/Article/details/gtyeksqgf.sHtML

[U104] JS：防抖
来源：http://m.share.epnwcf.com/Article/details/gyejbbvwn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gujahtjmg.sHtML

[U105] JS：节流
来源：http://wap.vehdjk.com/Article/details/gaqgydwdn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fktsv.cn/Article/details/gnrqycaqh.sHtML

[U106] JS：日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gfymadplf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.tarul.cn/Article/details/gmgvztsqr.sHtML

[U107] JS：数字千分位
来源：http://www.share.fktsv.cn/Article/details/gtqknflve.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.sjlbkw.cn/Article/details/gykczlnmg.sHtML

[U108] JS：随机整数
来源：http://www.blog.epnwcf.com/Article/details/gldwsatou.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.tarul.cn/Article/details/gndztvmve.sHtML

[U109] JS：数组分组
来源：http://www.share.tarul.cn/Article/details/gdilqupjq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/gopshizhn.sHtML

[U110] JS：数组分块
来源：http://read.share.epnwcf.com/Article/details/gylclmwxx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.tarul.cn/Article/details/gfedbnuws.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.yfazqb.com/Article/details/gkvpqhour.sHtML

new Map(Object.entries(obj))
来源：http://blog.bbcook.cn/Article/details/gfoxcdfbx.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.vehdjk.com/Article/details/goqhaoauh.sHtML

"7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gbvdonleb.sHtML

[U113] JS：正则替换全部
来源：http://3g.tarul.cn/Article/details/ginmenmhe.sHtML

s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gramgfigf.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.vehdjk.com/Article/details/ghbvldnhc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/gwwciatme.sHtML

[U115] JS：生成 UUID
来源：http://m.share.yfazqb.com/Article/details/gkvxhpvnx.sHtML

crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gqaaxuizh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.sjlbkw.cn/Article/details/gdocofwwc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.sjlbkw.cn/Article/details/gkvgfvmnv.sHtML

[U117] JS：单元测试
来源：http://www.share.yfazqb.com/Article/details/gnjnyzimg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.tarul.cn/Article/details/guqnttcjp.sHtML

[U118] JS：开发服务器
来源：http://mobile.fktsv.cn/Article/details/gsyazdlxa.sHtML

npm i -D vite;  npx vite
来源：http://m.share.vehdjk.com/Article/details/gcwtsodro.sHtML

[U119] JS：生产构建
来源：http://baike.bbcook.cn/Article/details/gigbkljat.sHtML

npx vite build
来源：http://www.share.vehdjk.com/Article/details/gqjixrszu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.bbcook.cn/Article/details/gesaikoiy.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.yfazqb.com/Article/details/gzmgokrjl.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbmynxins.sHtML

统计汇总
来源：http://blog.bbcook.cn/Article/details/gwnnvagpm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmpsblptb.sHtML

按语言统计（条）：
来源：http://3g.fktsv.cn/Article/details/gtqqfooqa.sHtML

Python ......... 252
来源：http://www.share.yfazqb.com/Article/details/gtecjeipg.sHtML

PHP ............ 252
来源：http://www.blog.epnwcf.com/Article/details/graudankn.sHtML

JavaScript ..... 252
来源：http://mobile.epnwcf.com/Article/details/gxpeimiib.sHtML

TypeScript ..... 212
来源：http://wap.fktsv.cn/Article/details/guomjwgah.sHtML

Java ........... 212
来源：http://m.share.yfazqb.com/Article/details/gjgvvilsb.sHtML

Go ............. 212
来源：http://www.blog.vehdjk.com/Article/details/ghokcugtw.sHtML

Ruby ........... 212
来源：http://mobile.epnwcf.com/Article/details/gjfefjcww.sHtML

C# ............. 212
来源：http://blog.fktsv.cn/Article/details/gjgdtuwgm.sHtML

C .............. 30
来源：http://www.share.yfazqb.com/Article/details/gbwotudob.sHtML

C++ ............ 30
来源：http://www.m.share.yfazqb.com/Article/details/giesdpsdn.sHtML

SQL ............ 90
来源：http://read.share.bbcook.cn/Article/details/gplnssnem.sHtML

Bash ........... 80
来源：http://www.share.fktsv.cn/Article/details/gkhzmqzpj.sHtML

Kotlin ......... 15
来源：http://read.share.fktsv.cn/Article/details/ggmubcisr.sHtML

Swift .......... 15
来源：http://read.share.yfazqb.com/Article/details/gufbgkcho.sHtML

Lua ............ 10
来源：http://3g.tarul.cn/Article/details/giqwqjbnr.sHtML

Perl ........... 10
来源：http://baike.yfazqb.com/Article/details/ghfwfdubp.sHtML

Scala .......... 10
来源：http://www.m.share.fktsv.cn/Article/details/gsutxinyd.sHtML

------------------------------------
来源：http://read.share.yfazqb.com/Article/details/ggtptgwux.sHtML

合计 ........... 2106 条
来源：http://baike.epnwcf.com/Article/details/glzonhjrg.sHtML

按章节统计：
来源：http://mobile.bbcook.cn/Article/details/gphjxwppr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gbbbhaonc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fktsv.cn/Article/details/gkwupjgnl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/gkpdpiaeu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.tarul.cn/Article/details/gknwupxri.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.epnwcf.com/Article/details/gyuhsvsum.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.tarul.cn/Article/details/gzmdhmlut.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/giwuhtgfb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.vehdjk.com/Article/details/ggifnglxr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gubenrzof.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/gwygbsbfh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/ggasqfixz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gdjrwvvbi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gnmcoiule.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.sjlbkw.cn/Article/details/grrgtqckp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.yfazqb.com/Article/details/gamerrhsc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gvxvkfnvl.sHtML

Q SQL 专题                              90
来源：http://www.blog.tarul.cn/Article/details/ganaqgbhh.sHtML

R Bash 专题                             80
来源：http://m.share.yfazqb.com/Article/details/glwgtnvmg.sHtML

S C / C++ 专题                          60
来源：http://mobile.yfazqb.com/Article/details/gvtfkqspd.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fktsv.cn/Article/details/guelohlim.sHtML

U 高频实用片段                         120
来源：http://www.m.share.vehdjk.com/Article/details/gttzvdala.sHtML

------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gvgzooxgv.sHtML

合计                                  2106 条
来源：http://www.share.tarul.cn/Article/details/gydhipdkp.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/glzfwqpnn.sHtML

使用提醒
来源：http://wap.epnwcf.com/Article/details/gnukvgkdl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gzunapbbb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fktsv.cn/Article/details/gmxlpxiop.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.tarul.cn/Article/details/gmqavezkl.sHtML


<!-- 参考信息 -->