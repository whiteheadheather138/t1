代发 wailian999

[U03] Py：加载 .env 配置
来源：http://read.share.epnwcf.com/Article/details/gxebncguc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.sjlbkw.cn/Article/details/gaokabbrx.sHtML

[U04] Py：变量调试打印
来源：http://m.share.vehdjk.com/Article/details/gimuoahag.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.bbcook.cn/Article/details/grhlamrcq.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/glxywekrk.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/grpcvjmkl.sHtML

[U06] Py：合并两个字典
来源：http://read.share.vehdjk.com/Article/details/gxhufzhsq.sHtML

{**a, **b}
来源：http://baike.yfazqb.com/Article/details/gpmhemnbc.sHtML

[U07] Py：反转字典键值
来源：http://read.share.vehdjk.com/Article/details/gdfdvbgrg.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fktsv.cn/Article/details/gnqzdotke.sHtML

[U08] Py：展平二维列表
来源：http://wap.epnwcf.com/Article/details/gcusbqwwx.sHtML

[y for x in nested for y in x]
来源：http://baike.fktsv.cn/Article/details/gnlcxjwvj.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.yfazqb.com/Article/details/grwcrlppa.sHtML

max(d, key=d.get)
来源：http://blog.tarul.cn/Article/details/gnsuhrxqp.sHtML

[U10] Py：按值排序字典
来源：http://read.share.epnwcf.com/Article/details/gfpzazbvz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fktsv.cn/Article/details/gxekrursm.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.epnwcf.com/Article/details/gzyysdkee.sHtML

(x * 2 for x in arr)
来源：http://read.share.sjlbkw.cn/Article/details/gzkpzmkqd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.tarul.cn/Article/details/gnajtlcxj.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.vehdjk.com/Article/details/glovgnizh.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fktsv.cn/Article/details/gzcmjobyj.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/gpnnuxnrk.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.tarul.cn/Article/details/gibrgwigg.sHtML

defaultdict(list)
来源：http://www.m.share.bbcook.cn/Article/details/glzgyyeht.sHtML

[U15] Py：高精度计时
来源：http://baike.epnwcf.com/Article/details/gxkakhaij.sHtML

t = time.perf_counter()
来源：http://baike.yfazqb.com/Article/details/gvflmyruu.sHtML

[U16] Py：命令行参数解析
来源：http://wap.tarul.cn/Article/details/glzhtdytc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.vehdjk.com/Article/details/gcdyjgnay.sHtML

[U17] Py：初始化日志
来源：http://mobile.epnwcf.com/Article/details/gfvloydgq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.tarul.cn/Article/details/gvchmiedy.sHtML

[U18] Py：预编译正则
来源：http://wap.tarul.cn/Article/details/gsrdshttw.sHtML

pat = re.compile(r"\d+")
来源：http://3g.yfazqb.com/Article/details/glnwfqtpb.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.vehdjk.com/Article/details/gbnbfjcsf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.epnwcf.com/Article/details/gdrfinktj.sHtML

[U20] Py：缓存函数结果
来源：http://3g.yfazqb.com/Article/details/gmsdfpvxv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.sjlbkw.cn/Article/details/gfssgujjj.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.sjlbkw.cn/Article/details/gxjrjwots.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/gplaursnj.sHtML

[U22] Py：矩阵转置
来源：http://www.share.vehdjk.com/Article/details/ggjcxrcei.sHtML

list(zip(*m))
来源：http://www.share.sjlbkw.cn/Article/details/gdbdqzsod.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.epnwcf.com/Article/details/gflohbrez.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fktsv.cn/Article/details/gcincvnrb.sHtML

[U24] Py：路径操作
来源：http://m.share.tarul.cn/Article/details/gutkljtgq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gastaubax.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.tarul.cn/Article/details/gyxaytijt.sHtML

csv.DictReader(f)
来源：http://wap.tarul.cn/Article/details/gwivyusgi.sHtML

[U26] Py：并发下载
来源：http://blog.epnwcf.com/Article/details/genkywpem.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.bbcook.cn/Article/details/gftjefsik.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.bbcook.cn/Article/details/gxodxmegz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.sjlbkw.cn/Article/details/gmhqbzbgo.sHtML

[U28] Py：类型别名
来源：http://www.share.yfazqb.com/Article/details/gpvtshdbl.sHtML

UserId = int
来源：http://wap.bbcook.cn/Article/details/gmdmcswwr.sHtML

[U29] Py：属性校验
来源：http://mobile.bbcook.cn/Article/details/gjuhiknon.sHtML

@property 与 @x.setter 配合
来源：http://blog.sjlbkw.cn/Article/details/gewqsztxr.sHtML

[U30] Py：数据类
来源：http://baike.yfazqb.com/Article/details/ghnichxoh.sHtML

@dataclass(slots=True)
来源：http://baike.tarul.cn/Article/details/gmntwcblz.sHtML

[U31] Py：单测
来源：http://www.share.vehdjk.com/Article/details/gbfxughzu.sHtML

python -m pytest -q
来源：http://3g.tarul.cn/Article/details/gvifmwypv.sHtML

[U32] Py：代码格式化
来源：http://read.share.yfazqb.com/Article/details/grkhmqifg.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.vehdjk.com/Article/details/gbmpswqhy.sHtML

[U33] Py：打包发布
来源：http://m.share.fktsv.cn/Article/details/gjumgfyes.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.tarul.cn/Article/details/gyabwzksb.sHtML

[U34] Py：判断编码
来源：http://wap.bbcook.cn/Article/details/gcmlwznal.sHtML

chardet.detect(raw)
来源：http://blog.sjlbkw.cn/Article/details/gffqncvub.sHtML

[U35] Py：发送邮件
来源：http://3g.yfazqb.com/Article/details/gzfnvwlhg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.tarul.cn/Article/details/gvuqsrqnb.sHtML

[U36] Py：定时任务
来源：http://blog.sjlbkw.cn/Article/details/gqpsyaprv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.yfazqb.com/Article/details/gwkxiqfuy.sHtML

[U37] Py：读写 Excel
来源：http://baike.bbcook.cn/Article/details/gpbvrgzoe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.yfazqb.com/Article/details/gadxtbuei.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fktsv.cn/Article/details/gfcpvmpdw.sHtML

Path(__file__).resolve().parent
来源：http://read.share.bbcook.cn/Article/details/guejgscdu.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.sjlbkw.cn/Article/details/gcmhplcml.sHtML

sys.stdout.isatty()
来源：http://wap.epnwcf.com/Article/details/gvaijgfqf.sHtML

[U40] Py：打印到标准错误
来源：http://blog.tarul.cn/Article/details/gortgfbvq.sHtML

print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/geowbpqsz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.yfazqb.com/Article/details/ggcrohdrd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fktsv.cn/Article/details/griypwboz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.vehdjk.com/Article/details/guwaraypm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.yfazqb.com/Article/details/gzwcsafhp.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.bbcook.cn/Article/details/gpmmexkxm.sHtML

namespace App\Http;
来源：http://read.share.bbcook.cn/Article/details/gzswgmfpt.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.epnwcf.com/Article/details/gfrtlvchp.sHtML

declare(strict_types=1);
来源：http://m.share.epnwcf.com/Article/details/gfuzxtbmr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.yfazqb.com/Article/details/gmvxcrgmo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gtawvpjrf.sHtML

[U46] PHP：可空类型
来源：http://m.share.epnwcf.com/Article/details/gcjriirlx.sHtML

?string $name = null
来源：http://blog.sjlbkw.cn/Article/details/gpcjrscpm.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gajazqiod.sHtML

int|string $id
来源：http://m.share.tarul.cn/Article/details/ghtqjbcsj.sHtML

[U48] PHP：纯枚举
来源：http://3g.bbcook.cn/Article/details/gmrvarngn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.bbcook.cn/Article/details/gyfomirag.sHtML

[U49] PHP：只读属性
来源：http://wap.epnwcf.com/Article/details/gnxeomztc.sHtML

public readonly string $name
来源：http://3g.bbcook.cn/Article/details/gjmsrrmek.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fktsv.cn/Article/details/gfpmrfqbx.sHtML

public function __construct(private int $id) {}
来源：http://m.share.sjlbkw.cn/Article/details/gmhiegtbz.sHtML

[U51] PHP：数组解构
来源：http://www.share.epnwcf.com/Article/details/gkatumkvy.sHtML

[$a, $b] = $arr;
来源：http://www.share.fktsv.cn/Article/details/goktnnxna.sHtML

[U52] PHP：箭头函数
来源：http://www.share.bbcook.cn/Article/details/gabifslmg.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.tarul.cn/Article/details/gafbfalan.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.vehdjk.com/Article/details/gblbsdzag.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.sjlbkw.cn/Article/details/geuwukcis.sHtML

[U54] PHP：空安全调用
来源：http://baike.epnwcf.com/Article/details/gjparlpzr.sHtML

$obj?->method()
来源：http://3g.yfazqb.com/Article/details/gbtzdjxwf.sHtML

[U55] PHP：match 表达式
来源：http://baike.vehdjk.com/Article/details/gfnsekyff.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.bbcook.cn/Article/details/gmouvarpc.sHtML

[U56] PHP：命名参数
来源：http://baike.fktsv.cn/Article/details/gwbokjfmp.sHtML

f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gyrerpyjo.sHtML

[U57] PHP：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gwmrpvekn.sHtML

"值: {$a}"
来源：http://m.share.bbcook.cn/Article/details/gyufbmbbc.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fktsv.cn/Article/details/gbreduzyn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gkzaghwwa.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fktsv.cn/Article/details/gbtklfqzh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gpkozgtnm.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/gtelmmtja.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.epnwcf.com/Article/details/glpgpjimj.sHtML

[U61] PHP：正则
来源：http://baike.vehdjk.com/Article/details/gnwahugkx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gqwkiyakt.sHtML

[U62] PHP：日期对象
来源：http://blog.yfazqb.com/Article/details/gnihtqpaz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.tarul.cn/Article/details/glsidkkjt.sHtML

[U63] PHP：文件读写
来源：http://blog.fktsv.cn/Article/details/gobmlnnmx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.bbcook.cn/Article/details/gqrjjqvta.sHtML

[U64] PHP：目录遍历
来源：http://read.share.sjlbkw.cn/Article/details/gqfbebunw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.sjlbkw.cn/Article/details/gxiddtbgy.sHtML

[U65] PHP：会话
来源：http://blog.yfazqb.com/Article/details/gdfybxdpy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.vehdjk.com/Article/details/gnnkuhqfj.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.yfazqb.com/Article/details/gsdwdbeyj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.yfazqb.com/Article/details/gnmhntopi.sHtML

[U67] PHP：处理文件上传
来源：http://baike.tarul.cn/Article/details/gkualslvu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.bbcook.cn/Article/details/gfjkotgru.sHtML

[U68] PHP：PDO 连接
来源：http://blog.yfazqb.com/Article/details/gcpzsjvvp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.yfazqb.com/Article/details/gmegfrfaf.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.bbcook.cn/Article/details/ggkfjhyfm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.sjlbkw.cn/Article/details/gxbvowass.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fktsv.cn/Article/details/gfxagsazv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fktsv.cn/Article/details/gotupqfbb.sHtML

[U71] PHP：抛出异常
来源：http://read.share.bbcook.cn/Article/details/gbcalujyy.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.epnwcf.com/Article/details/giidroucy.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fktsv.cn/Article/details/gnucmvbto.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.vehdjk.com/Article/details/gdpmsekgo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.tarul.cn/Article/details/gxrdzzfrm.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.tarul.cn/Article/details/gabqnuayk.sHtML

[U74] PHP：读取环境变量
来源：http://blog.vehdjk.com/Article/details/grhqsxwuu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.yfazqb.com/Article/details/gpugdmohg.sHtML

[U75] PHP：依赖注入
来源：http://wap.epnwcf.com/Article/details/ghtbbkrvv.sHtML

composer require psr/container
来源：http://read.share.fktsv.cn/Article/details/gbqbfjtzz.sHtML

[U76] PHP：简单路由
来源：http://www.share.fktsv.cn/Article/details/gnennbgkg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fktsv.cn/Article/details/giekeilre.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.yfazqb.com/Article/details/goofilqmt.sHtML

composer require twig/twig
来源：http://blog.yfazqb.com/Article/details/genkeutse.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.tarul.cn/Article/details/gbyoyzcxx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.yfazqb.com/Article/details/gjbhtaibk.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.vehdjk.com/Article/details/gimbtjtys.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.bbcook.cn/Article/details/gfwzsrqao.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.bbcook.cn/Article/details/gulyqjpev.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.bbcook.cn/Article/details/gqofklszu.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxumnhcv.sHtML

npm init -y;  npm i express
来源：http://www.m.share.tarul.cn/Article/details/gkefjxtwe.sHtML

[U82] JS：package.json 脚本
来源：http://wap.vehdjk.com/Article/details/gunvqhcsh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.epnwcf.com/Article/details/gtujdaine.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.epnwcf.com/Article/details/gpfvdhsxy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/ghdbcjskr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.sjlbkw.cn/Article/details/gtumysrgz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkvxjefy.sHtML

[U85] JS：可选链
来源：http://blog.fktsv.cn/Article/details/gflqnioiz.sHtML

a?.b?.c
来源：http://baike.epnwcf.com/Article/details/gygzpbiyv.sHtML

[U86] JS：空值合并
来源：http://3g.epnwcf.com/Article/details/gqpplrdxa.sHtML

a ?? b
来源：http://www.blog.tarul.cn/Article/details/gpdtfqvfi.sHtML

[U87] JS：解构默认值
来源：http://blog.epnwcf.com/Article/details/gvrozrwaj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.tarul.cn/Article/details/gquaccqpm.sHtML

[U88] JS：对象展开合并
来源：http://mobile.yfazqb.com/Article/details/ggqzurbtc.sHtML

{ ...a, ...b }
来源：http://www.share.vehdjk.com/Article/details/ggbndbsaw.sHtML

[U89] JS：数组去重
来源：http://www.share.fktsv.cn/Article/details/gyhvylocq.sHtML

[...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gvihoistj.sHtML

[U90] JS：数字数组排序
来源：http://blog.fktsv.cn/Article/details/gzybmkmqp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gcawdjkxu.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fktsv.cn/Article/details/gihjrbmen.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.bbcook.cn/Article/details/gnbhmytny.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gavpmbpge.sHtML

structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/ghdsvcrfh.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.yfazqb.com/Article/details/gaezgbpnz.sHtML

`共 ${n} 条`
来源：http://baike.bbcook.cn/Article/details/ghdcmtgso.sHtML

[U94] JS：箭头函数
来源：http://wap.yfazqb.com/Article/details/gwozwssbw.sHtML

const double = x => x * 2;
来源：http://wap.bbcook.cn/Article/details/gwaodwygk.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fktsv.cn/Article/details/ggtiswcug.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.yfazqb.com/Article/details/gwdzdqxwt.sHtML

[U96] JS：async/await 与异常
来源：http://wap.bbcook.cn/Article/details/gehoihvpd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gheuwwhfi.sHtML

[U97] JS：并发请求
来源：http://mobile.bbcook.cn/Article/details/gcbwkyrrc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gzomzgygs.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.bbcook.cn/Article/details/gtrtsrguc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.yfazqb.com/Article/details/gbruyxjhk.sHtML

[U99] JS：事件监听
来源：http://blog.sjlbkw.cn/Article/details/goocyidxr.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fktsv.cn/Article/details/gxldnplmv.sHtML

[U100] JS：DOM 查询
来源：http://wap.yfazqb.com/Article/details/gwhbsokyi.sHtML

document.querySelector(".item")
来源：http://3g.vehdjk.com/Article/details/gzrioorrm.sHtML

[U101] JS：classList 操作
来源：http://read.share.yfazqb.com/Article/details/gcezqwlgo.sHtML

el.classList.toggle("active")
来源：http://baike.yfazqb.com/Article/details/gvuvntngy.sHtML

[U102] JS：本地存储
来源：http://mobile.bbcook.cn/Article/details/gxoytpjpd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fktsv.cn/Article/details/gklrirzng.sHtML

[U103] JS：定时器
来源：http://www.blog.bbcook.cn/Article/details/gefhmwwxm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.yfazqb.com/Article/details/grkuuwwoa.sHtML

[U104] JS：防抖
来源：http://mobile.sjlbkw.cn/Article/details/gjcopwoka.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gfmcxepxp.sHtML

[U105] JS：节流
来源：http://wap.sjlbkw.cn/Article/details/gyhfniufb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.sjlbkw.cn/Article/details/gpwlfjnit.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/gvlshcfut.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.bbcook.cn/Article/details/gyrcgzjsd.sHtML

[U107] JS：数字千分位
来源：http://3g.vehdjk.com/Article/details/gworkbvrd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fktsv.cn/Article/details/gnqgoeyee.sHtML

[U108] JS：随机整数
来源：http://www.share.epnwcf.com/Article/details/gqmefmxpn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.bbcook.cn/Article/details/gnnzgnpxw.sHtML

[U109] JS：数组分组
来源：http://m.share.fktsv.cn/Article/details/gylmfengv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.tarul.cn/Article/details/gnujfhrej.sHtML

[U110] JS：数组分块
来源：http://m.share.fktsv.cn/Article/details/gksmcwzbt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.vehdjk.com/Article/details/ghshwwfct.sHtML

[U111] JS：对象转 Map
来源：http://www.share.tarul.cn/Article/details/guvovcebd.sHtML

new Map(Object.entries(obj))
来源：http://baike.sjlbkw.cn/Article/details/gfwemkdom.sHtML

[U112] JS：字符串补位
来源：http://www.blog.epnwcf.com/Article/details/gubopsvlh.sHtML

"7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gryupyvqp.sHtML

[U113] JS：正则替换全部
来源：http://www.share.epnwcf.com/Article/details/gonyztoba.sHtML

s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/ghubxwrzk.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.bbcook.cn/Article/details/gcmetjtbs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/gvbhyvaba.sHtML

[U115] JS：生成 UUID
来源：http://www.share.epnwcf.com/Article/details/gbipdjojs.sHtML

crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gyesqxcpu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.bbcook.cn/Article/details/gloygpxgc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.bbcook.cn/Article/details/gvqrflaxq.sHtML

[U117] JS：单元测试
来源：http://www.share.epnwcf.com/Article/details/gnutwfzjj.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.bbcook.cn/Article/details/gcbsafwil.sHtML

[U118] JS：开发服务器
来源：http://wap.fktsv.cn/Article/details/gyykacrko.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.sjlbkw.cn/Article/details/gzbmefawm.sHtML

[U119] JS：生产构建
来源：http://mobile.sjlbkw.cn/Article/details/gvucxiuju.sHtML

npx vite build
来源：http://mobile.yfazqb.com/Article/details/gbynujsqr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.epnwcf.com/Article/details/gbyudkcva.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.bbcook.cn/Article/details/gtdbazvdf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gbdheekei.sHtML

统计汇总
来源：http://mobile.sjlbkw.cn/Article/details/gqgdtimwl.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtswzizew.sHtML

按语言统计（条）：
来源：http://www.blog.epnwcf.com/Article/details/gpbtlyvwh.sHtML

Python ......... 252
来源：http://read.share.yfazqb.com/Article/details/gkaicfqal.sHtML

PHP ............ 252
来源：http://blog.bbcook.cn/Article/details/gtxtqgaau.sHtML

JavaScript ..... 252
来源：http://www.m.share.fktsv.cn/Article/details/gerwozuci.sHtML

TypeScript ..... 212
来源：http://m.share.bbcook.cn/Article/details/ghcphyhya.sHtML

Java ........... 212
来源：http://3g.bbcook.cn/Article/details/guaumsuph.sHtML

Go ............. 212
来源：http://read.share.tarul.cn/Article/details/ggcikjsen.sHtML

Ruby ........... 212
来源：http://baike.vehdjk.com/Article/details/gygkzddxm.sHtML

C# ............. 212
来源：http://read.share.vehdjk.com/Article/details/gxhowyuky.sHtML

C .............. 30
来源：http://blog.epnwcf.com/Article/details/gkgjyjkbx.sHtML

C++ ............ 30
来源：http://read.share.fktsv.cn/Article/details/givvlolbp.sHtML

SQL ............ 90
来源：http://www.share.epnwcf.com/Article/details/gsnjoeblw.sHtML

Bash ........... 80
来源：http://baike.sjlbkw.cn/Article/details/gzvqjrhtj.sHtML

Kotlin ......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/gykpvlfvo.sHtML

Swift .......... 15
来源：http://3g.epnwcf.com/Article/details/gbajzsbvq.sHtML

Lua ............ 10
来源：http://mobile.epnwcf.com/Article/details/ggkievmjs.sHtML

Perl ........... 10
来源：http://mobile.fktsv.cn/Article/details/gopbdkkng.sHtML

Scala .......... 10
来源：http://www.m.share.epnwcf.com/Article/details/gzngurvgg.sHtML

------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gqnqnhycn.sHtML

合计 ........... 2106 条
来源：http://baike.yfazqb.com/Article/details/gdoglaofg.sHtML

按章节统计：
来源：http://m.share.vehdjk.com/Article/details/ghevuucen.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fktsv.cn/Article/details/gknxkejko.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gvrmgsqkp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/gceqgimrx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/gkfhgnqsv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.vehdjk.com/Article/details/gyrjcxqcq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.vehdjk.com/Article/details/gqcktbfbb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/gvsudzdoi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/gflhtxbbb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gqqphzggn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/ggshijmda.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/goxsjtigz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gkiyfgmur.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gztmvzear.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gkbqnhuet.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.vehdjk.com/Article/details/gksqblbjd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gvnuqfykv.sHtML

Q SQL 专题                              90
来源：http://m.share.bbcook.cn/Article/details/gjlyqsdvq.sHtML

R Bash 专题                             80
来源：http://wap.epnwcf.com/Article/details/glozosuzu.sHtML

S C / C++ 专题                          60
来源：http://mobile.yfazqb.com/Article/details/guheulnmu.sHtML

T 其他语言补充                          60
来源：http://wap.yfazqb.com/Article/details/ghodkxuvr.sHtML

U 高频实用片段                         120
来源：http://www.share.vehdjk.com/Article/details/gnfehlgdw.sHtML

------------------------------------
来源：http://wap.bbcook.cn/Article/details/glnmkdtml.sHtML

合计                                  2106 条
来源：http://read.share.epnwcf.com/Article/details/gsjzeyeev.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gvhkescef.sHtML

使用提醒
来源：http://www.m.share.fktsv.cn/Article/details/gzpqvcwnv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.epnwcf.com/Article/details/ggugsytkm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fktsv.cn/Article/details/glfwgrtin.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fktsv.cn/Article/details/gznugszem.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.epnwcf.com/Article/details/ggcqjeesv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.yfazqb.com/Article/details/gecmnuarl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.vehdjk.com/Article/details/gkrwoigqe.sHtML

—— 文件结束 ——
来源：http://3g.epnwcf.com/Article/details/guautcmdw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grgsabtkp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.sjlbkw.cn/Article/details/gmhpdizdr.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.yfazqb.com/Article/details/gwxeosuhc.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gcoqdauiq.sHtML

【收录内容】
来源：http://blog.fktsv.cn/Article/details/gkqumglxk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.bbcook.cn/Article/details/giuijodjf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.yfazqb.com/Article/details/gblxgzoap.sHtML

SQL · Bash · C · C++
来源：http://www.share.epnwcf.com/Article/details/gnigbnfph.sHtML


<!-- 参考信息 -->