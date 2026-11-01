代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.blog.fktsv.cn/Article/details/gfgqxlfqv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.yfazqb.com/Article/details/gfqtyicvh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.bbcook.cn/Article/details/gmcjmskrk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.vehdjk.com/Article/details/gmfxabywp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fktsv.cn/Article/details/ghtcjwych.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fktsv.cn/Article/details/gmfgqhkoy.sHtML

[U04] Py：变量调试打印
来源：http://blog.epnwcf.com/Article/details/ghnkgiqmx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.bbcook.cn/Article/details/gufsvslpu.sHtML

[U05] Py：列表去重且保序
来源：http://blog.bbcook.cn/Article/details/gwtwggtmy.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/ggivgcplg.sHtML

[U06] Py：合并两个字典
来源：http://3g.vehdjk.com/Article/details/gefedxcxa.sHtML

{**a, **b}
来源：http://m.share.fktsv.cn/Article/details/ghrvpycea.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fktsv.cn/Article/details/gsmbkyoar.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.bbcook.cn/Article/details/ghowkfdrr.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdxkeeoz.sHtML

[y for x in nested for y in x]
来源：http://www.share.bbcook.cn/Article/details/gftedhuyg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.sjlbkw.cn/Article/details/gswhaqdds.sHtML

max(d, key=d.get)
来源：http://www.blog.fktsv.cn/Article/details/gkqwzaahx.sHtML

[U10] Py：按值排序字典
来源：http://blog.tarul.cn/Article/details/gswrveyxa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.bbcook.cn/Article/details/gqwjhrqeu.sHtML

[U11] Py：生成器表达式
来源：http://blog.tarul.cn/Article/details/gmddeuwbq.sHtML

(x * 2 for x in arr)
来源：http://3g.epnwcf.com/Article/details/gndyawsyu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.bbcook.cn/Article/details/gjthepmez.sHtML

Counter(arr).most_common(3)
来源：http://blog.tarul.cn/Article/details/guvoweyxn.sHtML

[U13] Py：固定长度队列
来源：http://mobile.vehdjk.com/Article/details/gwrphlcvm.sHtML

deque(maxlen=10)
来源：http://m.share.tarul.cn/Article/details/gaxueuxyw.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fktsv.cn/Article/details/gmeygwpja.sHtML

defaultdict(list)
来源：http://mobile.tarul.cn/Article/details/glblhseng.sHtML

[U15] Py：高精度计时
来源：http://mobile.bbcook.cn/Article/details/gmbafagkg.sHtML

t = time.perf_counter()
来源：http://blog.yfazqb.com/Article/details/gaxyzstsm.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.vehdjk.com/Article/details/govfphxez.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.epnwcf.com/Article/details/gxeujfjqn.sHtML

[U17] Py：初始化日志
来源：http://mobile.epnwcf.com/Article/details/ghbuuviyw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.bbcook.cn/Article/details/gjljalrgb.sHtML

[U18] Py：预编译正则
来源：http://www.blog.yfazqb.com/Article/details/galodpbuj.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fktsv.cn/Article/details/golckyfro.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.epnwcf.com/Article/details/gwerheupp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.yfazqb.com/Article/details/gwdibzaaa.sHtML

[U20] Py：缓存函数结果
来源：http://wap.vehdjk.com/Article/details/gcmnvwkbu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.bbcook.cn/Article/details/gkbmorors.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.yfazqb.com/Article/details/gofhdllkg.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/grwltlthi.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fktsv.cn/Article/details/gliwpbbjf.sHtML

list(zip(*m))
来源：http://wap.fktsv.cn/Article/details/giwnkxovi.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.epnwcf.com/Article/details/ghxocldsh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.vehdjk.com/Article/details/gszxkkpas.sHtML

[U24] Py：路径操作
来源：http://blog.fktsv.cn/Article/details/guaafvdox.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gcaizvuoq.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.tarul.cn/Article/details/gpwtxxytc.sHtML

csv.DictReader(f)
来源：http://www.m.share.vehdjk.com/Article/details/gnsqlukou.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fktsv.cn/Article/details/gkqqjiqzx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.vehdjk.com/Article/details/ghuydeprx.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.epnwcf.com/Article/details/gotqcgqpu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/gwpxwutkl.sHtML

[U28] Py：类型别名
来源：http://www.m.share.yfazqb.com/Article/details/glmgwswjt.sHtML

UserId = int
来源：http://www.blog.bbcook.cn/Article/details/gxpphlcwg.sHtML

[U29] Py：属性校验
来源：http://www.m.share.epnwcf.com/Article/details/gsjslksab.sHtML

@property 与 @x.setter 配合
来源：http://wap.yfazqb.com/Article/details/gfftfgboy.sHtML

[U30] Py：数据类
来源：http://mobile.vehdjk.com/Article/details/gqhmasiph.sHtML

@dataclass(slots=True)
来源：http://blog.sjlbkw.cn/Article/details/glfseptme.sHtML

[U31] Py：单测
来源：http://3g.yfazqb.com/Article/details/ghwntucxx.sHtML

python -m pytest -q
来源：http://m.share.sjlbkw.cn/Article/details/gswpwrdqp.sHtML

[U32] Py：代码格式化
来源：http://www.blog.tarul.cn/Article/details/gwmbilqna.sHtML

ruff format . && ruff check --fix .
来源：http://blog.tarul.cn/Article/details/guhefspwk.sHtML

[U33] Py：打包发布
来源：http://wap.vehdjk.com/Article/details/gmvogjfyj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.bbcook.cn/Article/details/gxnhgwraj.sHtML

[U34] Py：判断编码
来源：http://wap.bbcook.cn/Article/details/gtpeylghp.sHtML

chardet.detect(raw)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwzbmokm.sHtML

[U35] Py：发送邮件
来源：http://www.blog.tarul.cn/Article/details/gttemqbla.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.bbcook.cn/Article/details/gmoxfrlnc.sHtML

[U36] Py：定时任务
来源：http://www.share.yfazqb.com/Article/details/ghjzhdcdc.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.vehdjk.com/Article/details/ggjqwrwuh.sHtML

[U37] Py：读写 Excel
来源：http://m.share.epnwcf.com/Article/details/gyeipebrs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.vehdjk.com/Article/details/gfnpgtnni.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fktsv.cn/Article/details/gwnbzylnn.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fktsv.cn/Article/details/gyjaxpyxm.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.vehdjk.com/Article/details/gajpepxjq.sHtML

sys.stdout.isatty()
来源：http://mobile.fktsv.cn/Article/details/gelkmcvgc.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.epnwcf.com/Article/details/ggpegjaat.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fktsv.cn/Article/details/gqinpnqru.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fktsv.cn/Article/details/gwnxxpxll.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/gtieodpid.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.bbcook.cn/Article/details/gqwiejadz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.bbcook.cn/Article/details/gjpzzgifp.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gstgquald.sHtML

namespace App\Http;
来源：http://3g.epnwcf.com/Article/details/gzmwoyuvh.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fktsv.cn/Article/details/gzagmpkqm.sHtML

declare(strict_types=1);
来源：http://wap.yfazqb.com/Article/details/gtcftodgu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.vehdjk.com/Article/details/gzspqinfi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/ggewstijk.sHtML

[U46] PHP：可空类型
来源：http://3g.fktsv.cn/Article/details/gqlspzcxo.sHtML

?string $name = null
来源：http://www.m.share.fktsv.cn/Article/details/gpgzoadma.sHtML

[U47] PHP：联合类型
来源：http://3g.sjlbkw.cn/Article/details/gfomlvzyf.sHtML

int|string $id
来源：http://www.blog.tarul.cn/Article/details/gjfhlglui.sHtML

[U48] PHP：纯枚举
来源：http://www.share.sjlbkw.cn/Article/details/gmoclcfri.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.yfazqb.com/Article/details/giwpvdhcf.sHtML

[U49] PHP：只读属性
来源：http://read.share.epnwcf.com/Article/details/grxxmkcwr.sHtML

public readonly string $name
来源：http://3g.epnwcf.com/Article/details/gqnwrkmwv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.tarul.cn/Article/details/gwffhvpdg.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.epnwcf.com/Article/details/gwrngyzxr.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvoqbdjz.sHtML

[$a, $b] = $arr;
来源：http://3g.yfazqb.com/Article/details/gntkbomao.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/grkajkskm.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.bbcook.cn/Article/details/gmymdwwos.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.epnwcf.com/Article/details/gbsaknwia.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fktsv.cn/Article/details/gnzbaxurv.sHtML

[U54] PHP：空安全调用
来源：http://www.share.sjlbkw.cn/Article/details/gahdjxgyo.sHtML

$obj?->method()
来源：http://read.share.fktsv.cn/Article/details/gbcimetfb.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gtjjcbilf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fktsv.cn/Article/details/glihkxqrd.sHtML

[U56] PHP：命名参数
来源：http://blog.fktsv.cn/Article/details/gwuwkstco.sHtML

f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gxtkxkdfb.sHtML

[U57] PHP：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gjjhzoujk.sHtML

"值: {$a}"
来源：http://www.blog.yfazqb.com/Article/details/gpxuuzruz.sHtML

[U58] PHP：数组三件套
来源：http://www.share.yfazqb.com/Article/details/gdvimwxcq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fktsv.cn/Article/details/gndxtcids.sHtML

[U59] PHP：自定义排序
来源：http://mobile.epnwcf.com/Article/details/ghhgkgcsp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/gsvuftjpy.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.yfazqb.com/Article/details/gumrjonnh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.tarul.cn/Article/details/gmitbeffm.sHtML

[U61] PHP：正则
来源：http://read.share.epnwcf.com/Article/details/gfiwsycfq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gxkteypef.sHtML

[U62] PHP：日期对象
来源：http://3g.sjlbkw.cn/Article/details/gitelxxge.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.tarul.cn/Article/details/gnqymjzwf.sHtML

[U63] PHP：文件读写
来源：http://wap.tarul.cn/Article/details/ghzmxflou.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.yfazqb.com/Article/details/gvqvzekex.sHtML

[U64] PHP：目录遍历
来源：http://3g.fktsv.cn/Article/details/gfwmqwbvd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.epnwcf.com/Article/details/greedsoin.sHtML

[U65] PHP：会话
来源：http://read.share.tarul.cn/Article/details/gveihssnb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gngxaaofo.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.sjlbkw.cn/Article/details/giaupbqbu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.vehdjk.com/Article/details/gfkhzsmlw.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fktsv.cn/Article/details/gaxbuaern.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.vehdjk.com/Article/details/gzfsuygne.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fktsv.cn/Article/details/gnzrhbvrc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.vehdjk.com/Article/details/gmcyqxlhn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.yfazqb.com/Article/details/gtkgeuydf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.bbcook.cn/Article/details/gftnpsbti.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.vehdjk.com/Article/details/gccgeuzyw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.yfazqb.com/Article/details/geahtdcfp.sHtML

[U71] PHP：抛出异常
来源：http://mobile.tarul.cn/Article/details/ginasggzk.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.vehdjk.com/Article/details/gbyhsdmwo.sHtML

[U72] PHP：写错误日志
来源：http://www.share.yfazqb.com/Article/details/gxsvvhczu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.vehdjk.com/Article/details/gxbbppvnd.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.bbcook.cn/Article/details/gompxqpin.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgijmqwr.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gvnkqdyzz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.vehdjk.com/Article/details/gqrktoixt.sHtML

[U75] PHP：依赖注入
来源：http://mobile.tarul.cn/Article/details/gggrdogwn.sHtML

composer require psr/container
来源：http://m.share.vehdjk.com/Article/details/glazhkhnl.sHtML

[U76] PHP：简单路由
来源：http://blog.sjlbkw.cn/Article/details/gqraomrth.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.yfazqb.com/Article/details/gypuwbttu.sHtML

[U77] PHP：模板渲染
来源：http://m.share.yfazqb.com/Article/details/gdqmklkrn.sHtML

composer require twig/twig
来源：http://blog.fktsv.cn/Article/details/gzapodgtb.sHtML

[U78] PHP：单元测试
来源：http://blog.epnwcf.com/Article/details/gskoxxfug.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fktsv.cn/Article/details/gjqgkklgg.sHtML

[U79] PHP：静态分析
来源：http://www.share.sjlbkw.cn/Article/details/geaiddwjf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.epnwcf.com/Article/details/gxutvwzkz.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.bbcook.cn/Article/details/gplbsmhtf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.epnwcf.com/Article/details/gqzszmrvr.sHtML

[U81] JS：初始化项目
来源：http://baike.tarul.cn/Article/details/gqtrhjqyv.sHtML

npm init -y;  npm i express
来源：http://read.share.fktsv.cn/Article/details/gutcalvnv.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fktsv.cn/Article/details/gjpnhqrsv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.yfazqb.com/Article/details/gfscslltd.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.sjlbkw.cn/Article/details/gomgagmpk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gznmzvhsb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.sjlbkw.cn/Article/details/guqscyjdq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.tarul.cn/Article/details/gnjzknqsw.sHtML

[U85] JS：可选链
来源：http://www.share.sjlbkw.cn/Article/details/gkqjgirtd.sHtML

a?.b?.c
来源：http://3g.tarul.cn/Article/details/gyaiaimin.sHtML

[U86] JS：空值合并
来源：http://www.blog.epnwcf.com/Article/details/gotnzyzuk.sHtML

a ?? b
来源：http://www.blog.tarul.cn/Article/details/gjyeasszu.sHtML

[U87] JS：解构默认值
来源：http://www.blog.tarul.cn/Article/details/gdubrytbh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.tarul.cn/Article/details/gkboisjnx.sHtML

[U88] JS：对象展开合并
来源：http://blog.sjlbkw.cn/Article/details/gegaiomtp.sHtML

{ ...a, ...b }
来源：http://3g.vehdjk.com/Article/details/grhxnztvq.sHtML

[U89] JS：数组去重
来源：http://www.blog.epnwcf.com/Article/details/gctfukgni.sHtML

[...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gishglorm.sHtML

[U90] JS：数字数组排序
来源：http://3g.yfazqb.com/Article/details/gtimlwwhb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gqhweptis.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.epnwcf.com/Article/details/gwppoxuja.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.yfazqb.com/Article/details/givxnhmoh.sHtML

[U92] JS：深拷贝
来源：http://blog.sjlbkw.cn/Article/details/giewwsdpn.sHtML

structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gyshpwnbh.sHtML

[U93] JS：模板字符串
来源：http://m.share.vehdjk.com/Article/details/gpjujsdey.sHtML

`共 ${n} 条`
来源：http://blog.yfazqb.com/Article/details/gkzcywxgm.sHtML

[U94] JS：箭头函数
来源：http://www.share.fktsv.cn/Article/details/getcvsbyy.sHtML

const double = x => x * 2;
来源：http://www.blog.epnwcf.com/Article/details/glhaayhms.sHtML

[U95] JS：Promise 包装
来源：http://3g.sjlbkw.cn/Article/details/gbjdixexa.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.sjlbkw.cn/Article/details/gahsjdwtw.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.tarul.cn/Article/details/gtxjdvidh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gqoufatsd.sHtML

[U97] JS：并发请求
来源：http://www.share.epnwcf.com/Article/details/gpxyqepun.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gfcfewdxp.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.tarul.cn/Article/details/gnqzuaiwm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.bbcook.cn/Article/details/ggccwkbrl.sHtML

[U99] JS：事件监听
来源：http://m.share.tarul.cn/Article/details/gxzzqsaov.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fktsv.cn/Article/details/gumpoxqkn.sHtML

[U100] JS：DOM 查询
来源：http://mobile.yfazqb.com/Article/details/gmcbveezi.sHtML

document.querySelector(".item")
来源：http://read.share.epnwcf.com/Article/details/gxakaizlb.sHtML

[U101] JS：classList 操作
来源：http://3g.fktsv.cn/Article/details/grgjcbcni.sHtML

el.classList.toggle("active")
来源：http://read.share.vehdjk.com/Article/details/gqybepbgk.sHtML

[U102] JS：本地存储
来源：http://wap.sjlbkw.cn/Article/details/ghxwzzeop.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.bbcook.cn/Article/details/gpypeegup.sHtML

[U103] JS：定时器
来源：http://mobile.vehdjk.com/Article/details/gvnrykhst.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsociqgvo.sHtML

[U104] JS：防抖
来源：http://mobile.tarul.cn/Article/details/gujefykxw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gsqkyyzqc.sHtML

[U105] JS：节流
来源：http://blog.vehdjk.com/Article/details/grgqqoidc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.sjlbkw.cn/Article/details/gamxoixyx.sHtML

[U106] JS：日期格式化
来源：http://wap.vehdjk.com/Article/details/gktzdvcdj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.epnwcf.com/Article/details/gmwpmvhct.sHtML

[U107] JS：数字千分位
来源：http://3g.epnwcf.com/Article/details/gavccsqza.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gvcfocewj.sHtML

[U108] JS：随机整数
来源：http://blog.tarul.cn/Article/details/gnzahehoe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.epnwcf.com/Article/details/ggpjjcqdf.sHtML

[U109] JS：数组分组
来源：http://read.share.tarul.cn/Article/details/gfzptonat.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.tarul.cn/Article/details/gnwezsege.sHtML

[U110] JS：数组分块
来源：http://blog.sjlbkw.cn/Article/details/gmoajepnr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.vehdjk.com/Article/details/genriayjg.sHtML

[U111] JS：对象转 Map
来源：http://blog.bbcook.cn/Article/details/gnbpcxjnc.sHtML

new Map(Object.entries(obj))
来源：http://m.share.vehdjk.com/Article/details/gcyvhlfhy.sHtML

[U112] JS：字符串补位
来源：http://m.share.tarul.cn/Article/details/gsaxvxttp.sHtML

"7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gykirvjbg.sHtML

[U113] JS：正则替换全部
来源：http://m.share.bbcook.cn/Article/details/gcaltaiid.sHtML

s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gjisfebfj.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.epnwcf.com/Article/details/ggxgooqdx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/grotifdnf.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.epnwcf.com/Article/details/gdgtzfhbv.sHtML

crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/ghnrkmcrn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.yfazqb.com/Article/details/gclllhmdi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.yfazqb.com/Article/details/govrmpwrz.sHtML

[U117] JS：单元测试
来源：http://mobile.yfazqb.com/Article/details/gwwctcfim.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.tarul.cn/Article/details/gfsmdehie.sHtML

[U118] JS：开发服务器
来源：http://m.share.bbcook.cn/Article/details/ghdpxiprk.sHtML

npm i -D vite;  npx vite
来源：http://m.share.yfazqb.com/Article/details/gnjaquxma.sHtML

[U119] JS：生产构建
来源：http://3g.bbcook.cn/Article/details/gcxrvludb.sHtML

npx vite build
来源：http://www.share.tarul.cn/Article/details/gbmqpjarw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fktsv.cn/Article/details/gfzcmtulk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.tarul.cn/Article/details/gqdnbhdft.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gszjvxolz.sHtML

统计汇总
来源：http://www.share.fktsv.cn/Article/details/gnpmkjqsd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gukajwcai.sHtML

按语言统计（条）：
来源：http://www.share.epnwcf.com/Article/details/gixhwflfi.sHtML

Python ......... 252
来源：http://3g.sjlbkw.cn/Article/details/ghqfowfqk.sHtML

PHP ............ 252
来源：http://read.share.yfazqb.com/Article/details/gbergeczz.sHtML

JavaScript ..... 252
来源：http://mobile.bbcook.cn/Article/details/ggxwdpshu.sHtML

TypeScript ..... 212
来源：http://read.share.sjlbkw.cn/Article/details/gdgdgmmcf.sHtML

Java ........... 212
来源：http://m.share.epnwcf.com/Article/details/gqloecmfp.sHtML

Go ............. 212
来源：http://3g.vehdjk.com/Article/details/gztkbmvcy.sHtML

Ruby ........... 212
来源：http://www.m.share.yfazqb.com/Article/details/gnzwjojca.sHtML

C# ............. 212
来源：http://blog.epnwcf.com/Article/details/grrluyryw.sHtML

C .............. 30
来源：http://mobile.tarul.cn/Article/details/gcqlsqcmo.sHtML

C++ ............ 30
来源：http://mobile.tarul.cn/Article/details/gddgycdxw.sHtML

SQL ............ 90
来源：http://mobile.vehdjk.com/Article/details/gccbnukbp.sHtML

Bash ........... 80
来源：http://wap.sjlbkw.cn/Article/details/ginxyslcv.sHtML

Kotlin ......... 15
来源：http://m.share.sjlbkw.cn/Article/details/gvudczkqk.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/guqqoympe.sHtML

Lua ............ 10
来源：http://www.m.share.epnwcf.com/Article/details/gkmvjfnku.sHtML

Perl ........... 10
来源：http://read.share.yfazqb.com/Article/details/gcbpgenlj.sHtML

Scala .......... 10
来源：http://baike.vehdjk.com/Article/details/gacdnoltb.sHtML

------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gqeiaszfi.sHtML

合计 ........... 2106 条
来源：http://3g.sjlbkw.cn/Article/details/gdlwmritm.sHtML

按章节统计：
来源：http://mobile.epnwcf.com/Article/details/glymwihbs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.epnwcf.com/Article/details/glkcfuxfb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/glfklanqm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gwtsjpczk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.tarul.cn/Article/details/gkikexymo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.yfazqb.com/Article/details/gmixoxkzm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/gshvahoxb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gaiuzvlqb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.yfazqb.com/Article/details/gzknbwusq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gmspiyats.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/gwhmvfshh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gtcpslgwr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gwcwkjnsk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/gghvzuvqz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/goapxkmdk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.yfazqb.com/Article/details/gohppwvjb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gtnqopqya.sHtML

Q SQL 专题                              90
来源：http://blog.sjlbkw.cn/Article/details/grkhcixaq.sHtML

R Bash 专题                             80
来源：http://www.blog.sjlbkw.cn/Article/details/gaknnfxal.sHtML

S C / C++ 专题                          60
来源：http://wap.bbcook.cn/Article/details/gmlnibkyd.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fktsv.cn/Article/details/gsezoxteh.sHtML

U 高频实用片段                         120
来源：http://wap.vehdjk.com/Article/details/gtdcxheir.sHtML

------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gzbzlfboo.sHtML

合计                                  2106 条
来源：http://wap.vehdjk.com/Article/details/gfsoxdyyu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gmobnfiiq.sHtML

使用提醒
来源：http://read.share.bbcook.cn/Article/details/gcdrhjaev.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gzwsafotf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.bbcook.cn/Article/details/gbsjcugzb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.tarul.cn/Article/details/guyqkyrww.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.sjlbkw.cn/Article/details/gvttsixjb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fktsv.cn/Article/details/gtinqajyo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.epnwcf.com/Article/details/gxpvdblmr.sHtML

—— 文件结束 ——
来源：http://mobile.vehdjk.com/Article/details/gdvqfumcz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gksivvytj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.bbcook.cn/Article/details/ggdfpchsb.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.vehdjk.com/Article/details/glpqaxyli.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwrpcwdkv.sHtML


<!-- 参考信息 -->