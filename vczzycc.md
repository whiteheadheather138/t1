代发 wailian999

[U01] Py：创建虚拟环境
来源：http://baike.epnwcf.com/Article/details/gupjtlvus.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.bbcook.cn/Article/details/gevdnsazw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fktsv.cn/Article/details/gkxjewdus.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.vehdjk.com/Article/details/gpbtmozvn.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.vehdjk.com/Article/details/gcmlsiyvk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.epnwcf.com/Article/details/gwovkjqew.sHtML

[U04] Py：变量调试打印
来源：http://read.share.sjlbkw.cn/Article/details/gjaovhcha.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.sjlbkw.cn/Article/details/gmlrqcqya.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.vehdjk.com/Article/details/gxfgcykar.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/giqynesaf.sHtML

[U06] Py：合并两个字典
来源：http://baike.epnwcf.com/Article/details/gbkmeweek.sHtML

{**a, **b}
来源：http://www.m.share.tarul.cn/Article/details/gzgstyjal.sHtML

[U07] Py：反转字典键值
来源：http://mobile.yfazqb.com/Article/details/gtelyrniw.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fktsv.cn/Article/details/gdglujfmg.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.tarul.cn/Article/details/ghkmgwjkv.sHtML

[y for x in nested for y in x]
来源：http://3g.epnwcf.com/Article/details/gfrezpbrm.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.yfazqb.com/Article/details/ggsvejeba.sHtML

max(d, key=d.get)
来源：http://3g.sjlbkw.cn/Article/details/guvhsfuim.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.tarul.cn/Article/details/gdfbzjmlv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.bbcook.cn/Article/details/gpubqtctp.sHtML

[U11] Py：生成器表达式
来源：http://baike.vehdjk.com/Article/details/grrnauufy.sHtML

(x * 2 for x in arr)
来源：http://baike.epnwcf.com/Article/details/gjwlfasxi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.epnwcf.com/Article/details/geoopqdbe.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.yfazqb.com/Article/details/gybuehkas.sHtML

[U13] Py：固定长度队列
来源：http://read.share.sjlbkw.cn/Article/details/gfwqafznl.sHtML

deque(maxlen=10)
来源：http://read.share.tarul.cn/Article/details/grudjtkgi.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.sjlbkw.cn/Article/details/gghhvtwic.sHtML

defaultdict(list)
来源：http://blog.sjlbkw.cn/Article/details/getqfutpw.sHtML

[U15] Py：高精度计时
来源：http://mobile.epnwcf.com/Article/details/gxijgabxt.sHtML

t = time.perf_counter()
来源：http://m.share.yfazqb.com/Article/details/gmgfoybyu.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fktsv.cn/Article/details/gfkoxlzrv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.epnwcf.com/Article/details/gcxseszmk.sHtML

[U17] Py：初始化日志
来源：http://read.share.yfazqb.com/Article/details/gbktkncos.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.epnwcf.com/Article/details/gvhxmlglq.sHtML

[U18] Py：预编译正则
来源：http://blog.epnwcf.com/Article/details/gtbbbjvpl.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fktsv.cn/Article/details/gbpthxisx.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.sjlbkw.cn/Article/details/gandzueny.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.sjlbkw.cn/Article/details/gkwsdafke.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.vehdjk.com/Article/details/gdkqtzbuq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.yfazqb.com/Article/details/gctlepaku.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.bbcook.cn/Article/details/gibdplyos.sHtML

@contextlib.contextmanager
来源：http://www.blog.epnwcf.com/Article/details/geatpfcnv.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.bbcook.cn/Article/details/gapkvoflg.sHtML

list(zip(*m))
来源：http://www.blog.fktsv.cn/Article/details/gkwommwxo.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fktsv.cn/Article/details/gecnewdgb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.vehdjk.com/Article/details/gvvxscjys.sHtML

[U24] Py：路径操作
来源：http://read.share.sjlbkw.cn/Article/details/gvqdeoybo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gcxhxlkcm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fktsv.cn/Article/details/gpikcpzdc.sHtML

csv.DictReader(f)
来源：http://read.share.vehdjk.com/Article/details/gglstugzg.sHtML

[U26] Py：并发下载
来源：http://baike.fktsv.cn/Article/details/gxkbxjrcb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.tarul.cn/Article/details/gqeuyucge.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fktsv.cn/Article/details/gygvcnwud.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.vehdjk.com/Article/details/gmlrfohgg.sHtML

[U28] Py：类型别名
来源：http://m.share.yfazqb.com/Article/details/gwderuxan.sHtML

UserId = int
来源：http://baike.vehdjk.com/Article/details/gtfnhfhsz.sHtML

[U29] Py：属性校验
来源：http://www.m.share.yfazqb.com/Article/details/glsblkfmo.sHtML

@property 与 @x.setter 配合
来源：http://m.share.yfazqb.com/Article/details/gxagrvbca.sHtML

[U30] Py：数据类
来源：http://www.m.share.tarul.cn/Article/details/grzmyeiik.sHtML

@dataclass(slots=True)
来源：http://mobile.vehdjk.com/Article/details/gkkmqbxfj.sHtML

[U31] Py：单测
来源：http://blog.sjlbkw.cn/Article/details/gzepnjgsk.sHtML

python -m pytest -q
来源：http://3g.tarul.cn/Article/details/ggnvrubwd.sHtML

[U32] Py：代码格式化
来源：http://3g.tarul.cn/Article/details/gttikdstu.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.yfazqb.com/Article/details/gcrjmkfjn.sHtML

[U33] Py：打包发布
来源：http://wap.bbcook.cn/Article/details/gsysodqnf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.bbcook.cn/Article/details/gtqxkudly.sHtML

[U34] Py：判断编码
来源：http://www.share.yfazqb.com/Article/details/gtwblntxa.sHtML

chardet.detect(raw)
来源：http://m.share.epnwcf.com/Article/details/gvjogvdhl.sHtML

[U35] Py：发送邮件
来源：http://blog.vehdjk.com/Article/details/gonnozkuq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.tarul.cn/Article/details/gvmrobumu.sHtML

[U36] Py：定时任务
来源：http://www.m.share.tarul.cn/Article/details/gjruhokjx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.epnwcf.com/Article/details/gznrxwfzh.sHtML

[U37] Py：读写 Excel
来源：http://www.share.sjlbkw.cn/Article/details/gsvfxqpzm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.bbcook.cn/Article/details/gjswidyfy.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.sjlbkw.cn/Article/details/gmccdnlge.sHtML

Path(__file__).resolve().parent
来源：http://baike.fktsv.cn/Article/details/gmkdpzonv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.vehdjk.com/Article/details/grsuexmkl.sHtML

sys.stdout.isatty()
来源：http://read.share.sjlbkw.cn/Article/details/gngxojnca.sHtML

[U40] Py：打印到标准错误
来源：http://blog.yfazqb.com/Article/details/ganzgxaze.sHtML

print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/gfavpieqv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.tarul.cn/Article/details/gduujtcir.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.epnwcf.com/Article/details/gomgkiwpo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.yfazqb.com/Article/details/gjrblbfil.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.bbcook.cn/Article/details/gbzzjvhhh.sHtML

[U43] PHP：声明命名空间
来源：http://wap.vehdjk.com/Article/details/gblxtpgms.sHtML

namespace App\Http;
来源：http://www.blog.sjlbkw.cn/Article/details/guuzwqyqi.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.yfazqb.com/Article/details/grauyybqp.sHtML

declare(strict_types=1);
来源：http://m.share.bbcook.cn/Article/details/gvyafguog.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmetewwt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/galmwefmb.sHtML

[U46] PHP：可空类型
来源：http://read.share.bbcook.cn/Article/details/gggfyygez.sHtML

?string $name = null
来源：http://www.blog.epnwcf.com/Article/details/gyiuzypee.sHtML

[U47] PHP：联合类型
来源：http://wap.sjlbkw.cn/Article/details/gobiexqsy.sHtML

int|string $id
来源：http://www.share.sjlbkw.cn/Article/details/gidhxbhcl.sHtML

[U48] PHP：纯枚举
来源：http://blog.bbcook.cn/Article/details/ggafrlhim.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fktsv.cn/Article/details/gtevvoogq.sHtML

[U49] PHP：只读属性
来源：http://3g.bbcook.cn/Article/details/gxubdbthe.sHtML

public readonly string $name
来源：http://mobile.vehdjk.com/Article/details/gebvtzgeb.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.yfazqb.com/Article/details/gtykfbuvq.sHtML

public function __construct(private int $id) {}
来源：http://mobile.epnwcf.com/Article/details/gkxzolyiw.sHtML

[U51] PHP：数组解构
来源：http://baike.yfazqb.com/Article/details/gbtefgiyc.sHtML

[$a, $b] = $arr;
来源：http://wap.tarul.cn/Article/details/goiwhxvfh.sHtML

[U52] PHP：箭头函数
来源：http://www.share.yfazqb.com/Article/details/gnayalzsy.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.bbcook.cn/Article/details/gqkbbgtym.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.yfazqb.com/Article/details/gcysehsub.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.epnwcf.com/Article/details/grhkgxhej.sHtML

[U54] PHP：空安全调用
来源：http://mobile.yfazqb.com/Article/details/gqctfwzib.sHtML

$obj?->method()
来源：http://m.share.fktsv.cn/Article/details/gqnrfzdqv.sHtML

[U55] PHP：match 表达式
来源：http://mobile.vehdjk.com/Article/details/gyetcwgjw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.vehdjk.com/Article/details/ggjamrxtc.sHtML

[U56] PHP：命名参数
来源：http://www.share.epnwcf.com/Article/details/gmqqvlzqs.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gwmwrzbmh.sHtML

[U57] PHP：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gefmhgvbe.sHtML

"值: {$a}"
来源：http://wap.epnwcf.com/Article/details/gfafivzkh.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.sjlbkw.cn/Article/details/grwrgjagl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.tarul.cn/Article/details/gydquwfym.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fktsv.cn/Article/details/gewmfyvcr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/gqxstlugm.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.epnwcf.com/Article/details/gymkvewuh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.vehdjk.com/Article/details/gjgcfamlz.sHtML

[U61] PHP：正则
来源：http://wap.epnwcf.com/Article/details/georlllhm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/gwayvhnfr.sHtML

[U62] PHP：日期对象
来源：http://wap.sjlbkw.cn/Article/details/gahhzhafl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.tarul.cn/Article/details/gwppysdbg.sHtML

[U63] PHP：文件读写
来源：http://3g.sjlbkw.cn/Article/details/goenjxjdg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.bbcook.cn/Article/details/gasutgcpl.sHtML

[U64] PHP：目录遍历
来源：http://read.share.yfazqb.com/Article/details/gkdwgrgru.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fktsv.cn/Article/details/gsmdspfdt.sHtML

[U65] PHP：会话
来源：http://baike.bbcook.cn/Article/details/gjrfafcvz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.tarul.cn/Article/details/goedwzwla.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.bbcook.cn/Article/details/gcezbzyyn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.sjlbkw.cn/Article/details/gmgnnwfcw.sHtML

[U67] PHP：处理文件上传
来源：http://blog.tarul.cn/Article/details/gsdoeqbno.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.sjlbkw.cn/Article/details/glmfhxfdo.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.yfazqb.com/Article/details/gklfsbydx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.sjlbkw.cn/Article/details/ghczfuyvc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.vehdjk.com/Article/details/goixibnqk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.sjlbkw.cn/Article/details/gmzszuice.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.tarul.cn/Article/details/gktzcayvk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.epnwcf.com/Article/details/gxlltilea.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaniokeq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.tarul.cn/Article/details/gbksxkdct.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.vehdjk.com/Article/details/gvdrjocyj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.epnwcf.com/Article/details/giyaoxxae.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.sjlbkw.cn/Article/details/gvanruamw.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fktsv.cn/Article/details/ggorgoqwx.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.tarul.cn/Article/details/guzrlqobg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.vehdjk.com/Article/details/gxrbdrikk.sHtML

[U75] PHP：依赖注入
来源：http://baike.yfazqb.com/Article/details/gjsxwmjlm.sHtML

composer require psr/container
来源：http://baike.epnwcf.com/Article/details/gwyacfqio.sHtML

[U76] PHP：简单路由
来源：http://3g.epnwcf.com/Article/details/gmngkvxvb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fktsv.cn/Article/details/gebrhddes.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.yfazqb.com/Article/details/gpwkpspiy.sHtML

composer require twig/twig
来源：http://www.share.fktsv.cn/Article/details/grxruxshg.sHtML

[U78] PHP：单元测试
来源：http://www.share.sjlbkw.cn/Article/details/gnzqiuosu.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.sjlbkw.cn/Article/details/gbpjjeyoc.sHtML

[U79] PHP：静态分析
来源：http://3g.bbcook.cn/Article/details/gytbbwvxx.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fktsv.cn/Article/details/gjmbebodl.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.sjlbkw.cn/Article/details/gxrqrowen.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.bbcook.cn/Article/details/gcmbqnimx.sHtML

[U81] JS：初始化项目
来源：http://baike.epnwcf.com/Article/details/gvzyoyart.sHtML

npm init -y;  npm i express
来源：http://m.share.sjlbkw.cn/Article/details/gnuvmnqyo.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.sjlbkw.cn/Article/details/gtlgtyvtb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fktsv.cn/Article/details/gjzimgguo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.bbcook.cn/Article/details/gclvdqcij.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gmrqqtomg.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.bbcook.cn/Article/details/gbibfsmuo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fktsv.cn/Article/details/gppumyupc.sHtML

[U85] JS：可选链
来源：http://mobile.tarul.cn/Article/details/gwwjfbjpa.sHtML

a?.b?.c
来源：http://read.share.epnwcf.com/Article/details/gjtmvsjom.sHtML

[U86] JS：空值合并
来源：http://www.m.share.epnwcf.com/Article/details/gxgnnrsok.sHtML

a ?? b
来源：http://blog.bbcook.cn/Article/details/gravboatk.sHtML

[U87] JS：解构默认值
来源：http://www.share.epnwcf.com/Article/details/gyckxbmcv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.epnwcf.com/Article/details/gtstzawim.sHtML

[U88] JS：对象展开合并
来源：http://m.share.tarul.cn/Article/details/gcarqmavw.sHtML

{ ...a, ...b }
来源：http://3g.vehdjk.com/Article/details/gzgfkhvan.sHtML

[U89] JS：数组去重
来源：http://www.share.sjlbkw.cn/Article/details/gxaiymzok.sHtML

[...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gpzhpepqh.sHtML

[U90] JS：数字数组排序
来源：http://3g.epnwcf.com/Article/details/gljwefplv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gjfabnksg.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fktsv.cn/Article/details/gdgeabjsp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.vehdjk.com/Article/details/gupczzskz.sHtML

[U92] JS：深拷贝
来源：http://read.share.tarul.cn/Article/details/gdofxfuqf.sHtML

structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gdmiapzpx.sHtML

[U93] JS：模板字符串
来源：http://blog.yfazqb.com/Article/details/gddtmoqdp.sHtML

`共 ${n} 条`
来源：http://www.share.vehdjk.com/Article/details/gwpqyvpqi.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.yfazqb.com/Article/details/gorfhittm.sHtML

const double = x => x * 2;
来源：http://mobile.tarul.cn/Article/details/gjgcffpyr.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fktsv.cn/Article/details/gmanaibqz.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.vehdjk.com/Article/details/gsteolnjd.sHtML

[U96] JS：async/await 与异常
来源：http://wap.epnwcf.com/Article/details/gtbuuwbdk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gfmqxokkv.sHtML

[U97] JS：并发请求
来源：http://blog.tarul.cn/Article/details/gcifqvjrw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/goynerdyx.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fktsv.cn/Article/details/gapexyzyd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.epnwcf.com/Article/details/gckxgkfyz.sHtML

[U99] JS：事件监听
来源：http://3g.fktsv.cn/Article/details/gcxeivxwa.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.vehdjk.com/Article/details/gnmgrxzaz.sHtML

[U100] JS：DOM 查询
来源：http://read.share.vehdjk.com/Article/details/gyesujjjc.sHtML

document.querySelector(".item")
来源：http://wap.sjlbkw.cn/Article/details/gizzgphoo.sHtML

[U101] JS：classList 操作
来源：http://blog.epnwcf.com/Article/details/geyyjwysf.sHtML

el.classList.toggle("active")
来源：http://baike.epnwcf.com/Article/details/gacfgoryv.sHtML

[U102] JS：本地存储
来源：http://mobile.fktsv.cn/Article/details/gvqqkobhm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.sjlbkw.cn/Article/details/gmamhlstr.sHtML

[U103] JS：定时器
来源：http://www.share.vehdjk.com/Article/details/gojsiivce.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.bbcook.cn/Article/details/grvzzhqwe.sHtML

[U104] JS：防抖
来源：http://read.share.tarul.cn/Article/details/gromgoebo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gsdgsnglg.sHtML

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/ggcdkwezw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fktsv.cn/Article/details/gfcvogkuc.sHtML

[U106] JS：日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gqrehunqt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.yfazqb.com/Article/details/gsptpcbhy.sHtML

[U107] JS：数字千分位
来源：http://3g.tarul.cn/Article/details/glwmpvnwb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.bbcook.cn/Article/details/gnjwedsgd.sHtML

[U108] JS：随机整数
来源：http://baike.bbcook.cn/Article/details/golmbvpkn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.sjlbkw.cn/Article/details/ghynciilg.sHtML

[U109] JS：数组分组
来源：http://m.share.yfazqb.com/Article/details/gqzhfrdgq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gklveqzob.sHtML

[U110] JS：数组分块
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmwvzwws.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fktsv.cn/Article/details/gfljbxoxi.sHtML

[U111] JS：对象转 Map
来源：http://mobile.sjlbkw.cn/Article/details/gwdjggiaq.sHtML

new Map(Object.entries(obj))
来源：http://www.share.bbcook.cn/Article/details/gdgqgfniy.sHtML

[U112] JS：字符串补位
来源：http://www.blog.tarul.cn/Article/details/gwvsoosaf.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gwxpfixyo.sHtML

[U113] JS：正则替换全部
来源：http://www.share.yfazqb.com/Article/details/gcoglixpb.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/giqupjggv.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.bbcook.cn/Article/details/gflabalnk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/gqqfjzaat.sHtML

[U115] JS：生成 UUID
来源：http://wap.epnwcf.com/Article/details/gtfkuklqc.sHtML

crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/grlhycwhj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.bbcook.cn/Article/details/gchvqitbg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.tarul.cn/Article/details/gtikmaplh.sHtML

[U117] JS：单元测试
来源：http://wap.bbcook.cn/Article/details/gzxlzyxpt.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.yfazqb.com/Article/details/gaczyjsnn.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.sjlbkw.cn/Article/details/glijoczlf.sHtML

npm i -D vite;  npx vite
来源：http://www.share.epnwcf.com/Article/details/goiaosqmo.sHtML

[U119] JS：生产构建
来源：http://blog.sjlbkw.cn/Article/details/gbjdgesvk.sHtML

npx vite build
来源：http://wap.yfazqb.com/Article/details/gdkmthdya.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.tarul.cn/Article/details/ginribomd.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.sjlbkw.cn/Article/details/gqigxuwco.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/glmiqwcgx.sHtML

统计汇总
来源：http://www.m.share.yfazqb.com/Article/details/golsxazmc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/giitimhsj.sHtML

按语言统计（条）：
来源：http://read.share.epnwcf.com/Article/details/grphwgnku.sHtML

Python ......... 252
来源：http://blog.tarul.cn/Article/details/gthimhlzq.sHtML

PHP ............ 252
来源：http://www.blog.epnwcf.com/Article/details/gfxqscenq.sHtML

JavaScript ..... 252
来源：http://3g.bbcook.cn/Article/details/gmdnxhmde.sHtML

TypeScript ..... 212
来源：http://3g.yfazqb.com/Article/details/gfbddqmkl.sHtML

Java ........... 212
来源：http://m.share.vehdjk.com/Article/details/gqdcjldgz.sHtML

Go ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gjwqctnpw.sHtML

Ruby ........... 212
来源：http://wap.epnwcf.com/Article/details/gxxghimdb.sHtML

C# ............. 212
来源：http://www.share.tarul.cn/Article/details/gskhlorkf.sHtML

C .............. 30
来源：http://www.m.share.tarul.cn/Article/details/gjenpavet.sHtML

C++ ............ 30
来源：http://read.share.yfazqb.com/Article/details/gkqjubfqu.sHtML

SQL ............ 90
来源：http://read.share.bbcook.cn/Article/details/gjxiqjrgw.sHtML

Bash ........... 80
来源：http://www.blog.bbcook.cn/Article/details/gcbqnqbxt.sHtML

Kotlin ......... 15
来源：http://baike.fktsv.cn/Article/details/gpvvbhrxr.sHtML

Swift .......... 15
来源：http://mobile.fktsv.cn/Article/details/gqvzmpmzf.sHtML

Lua ............ 10
来源：http://3g.tarul.cn/Article/details/gyvedlbxi.sHtML

Perl ........... 10
来源：http://m.share.sjlbkw.cn/Article/details/geetgcckl.sHtML

Scala .......... 10
来源：http://www.m.share.bbcook.cn/Article/details/gelobruix.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/ggwryfsfl.sHtML

合计 ........... 2106 条
来源：http://blog.vehdjk.com/Article/details/gdfwdzmpl.sHtML

按章节统计：
来源：http://www.blog.yfazqb.com/Article/details/gwucihntu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.bbcook.cn/Article/details/gbnwozcnu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/gtmyfwwum.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gvuuhsjfl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.tarul.cn/Article/details/gavthnwtt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fktsv.cn/Article/details/gaoprjsdc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gmxvxnszw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gqaxfbxbo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gsnvfvlvf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gaxbsqqjy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.tarul.cn/Article/details/gaazaybrp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gycyheqmg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gulcgcaww.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/genxodnhs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.epnwcf.com/Article/details/gekwtlucr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.tarul.cn/Article/details/gemhqvtqx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gzkazigti.sHtML

Q SQL 专题                              90
来源：http://wap.sjlbkw.cn/Article/details/gpkqxvrql.sHtML

R Bash 专题                             80
来源：http://www.m.share.yfazqb.com/Article/details/gtytoxean.sHtML

S C / C++ 专题                          60
来源：http://3g.sjlbkw.cn/Article/details/gdysborsf.sHtML

T 其他语言补充                          60
来源：http://www.share.epnwcf.com/Article/details/gqbmrppfo.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fktsv.cn/Article/details/gfpnympzh.sHtML

------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gcgapqass.sHtML

合计                                  2106 条
来源：http://read.share.vehdjk.com/Article/details/gkclkanam.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gomjsgmkd.sHtML

使用提醒
来源：http://blog.epnwcf.com/Article/details/gggydeaxg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gngmjpbmg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fktsv.cn/Article/details/grqrhttwj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.sjlbkw.cn/Article/details/gesdsszeq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fktsv.cn/Article/details/gztxibspy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.sjlbkw.cn/Article/details/gfetxwxqu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.tarul.cn/Article/details/gdjowyrtf.sHtML

—— 文件结束 ——
来源：http://blog.yfazqb.com/Article/details/goregpgef.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmuzdfjph.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.sjlbkw.cn/Article/details/ghygwfcbk.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.yfazqb.com/Article/details/ghwedvfnv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwfwhapgs.sHtML


<!-- 参考信息 -->