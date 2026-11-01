代发 wailian999

[U05] Py：列表去重且保序
来源：http://blog.epnwcf.com/Article/details/gxkfbvxmj.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/gbzarnnlc.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fktsv.cn/Article/details/gfstnzkwx.sHtML

{**a, **b}
来源：http://baike.tarul.cn/Article/details/gsvcsxozz.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fktsv.cn/Article/details/gphytdzei.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.yfazqb.com/Article/details/gzfhbiscu.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gvbtcopdo.sHtML

[y for x in nested for y in x]
来源：http://mobile.sjlbkw.cn/Article/details/gxrvbszui.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.yfazqb.com/Article/details/gntkkbeeq.sHtML

max(d, key=d.get)
来源：http://www.m.share.fktsv.cn/Article/details/gshzrymev.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fktsv.cn/Article/details/gbgrujksn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.sjlbkw.cn/Article/details/gaqkfmckj.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.tarul.cn/Article/details/gydmyatxg.sHtML

(x * 2 for x in arr)
来源：http://baike.vehdjk.com/Article/details/gogbotjdo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.vehdjk.com/Article/details/gmcyciapo.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.epnwcf.com/Article/details/gydbaycfu.sHtML

[U13] Py：固定长度队列
来源：http://baike.epnwcf.com/Article/details/gtazanomb.sHtML

deque(maxlen=10)
来源：http://read.share.vehdjk.com/Article/details/gngjxkcgb.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.vehdjk.com/Article/details/gnemqrdsq.sHtML

defaultdict(list)
来源：http://mobile.yfazqb.com/Article/details/gylsikpfl.sHtML

[U15] Py：高精度计时
来源：http://mobile.epnwcf.com/Article/details/ggdvhnbov.sHtML

t = time.perf_counter()
来源：http://blog.bbcook.cn/Article/details/gyjykmnip.sHtML

[U16] Py：命令行参数解析
来源：http://blog.vehdjk.com/Article/details/gwlectnqa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.vehdjk.com/Article/details/gcixehbap.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fktsv.cn/Article/details/gwfqgsepz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.epnwcf.com/Article/details/gdkhsnsrd.sHtML

[U18] Py：预编译正则
来源：http://baike.epnwcf.com/Article/details/gtehpmezf.sHtML

pat = re.compile(r"\d+")
来源：http://baike.sjlbkw.cn/Article/details/gxhsiwmdv.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.tarul.cn/Article/details/gshoqbcxo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.vehdjk.com/Article/details/gfyygrzwq.sHtML

[U20] Py：缓存函数结果
来源：http://blog.vehdjk.com/Article/details/gpudolbvk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.epnwcf.com/Article/details/gfqthzkgh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.yfazqb.com/Article/details/gfolmcmfc.sHtML

@contextlib.contextmanager
来源：http://3g.yfazqb.com/Article/details/gezpavyqp.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fktsv.cn/Article/details/gkyrpnxna.sHtML

list(zip(*m))
来源：http://mobile.fktsv.cn/Article/details/gygprpmys.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.yfazqb.com/Article/details/gcmzbaqrw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.epnwcf.com/Article/details/gvkmbqews.sHtML

[U24] Py：路径操作
来源：http://www.share.yfazqb.com/Article/details/gvkgkiame.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.yfazqb.com/Article/details/gutklxjdg.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.bbcook.cn/Article/details/gwtxmfmmt.sHtML

csv.DictReader(f)
来源：http://m.share.fktsv.cn/Article/details/gwiiqbppc.sHtML

[U26] Py：并发下载
来源：http://read.share.yfazqb.com/Article/details/ghqnftnut.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.yfazqb.com/Article/details/gxtzohhor.sHtML

[U27] Py：异步 HTTP
来源：http://wap.tarul.cn/Article/details/gpudmrvnw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.tarul.cn/Article/details/gvwezzcqx.sHtML

[U28] Py：类型别名
来源：http://m.share.fktsv.cn/Article/details/gdpdedlij.sHtML

UserId = int
来源：http://baike.tarul.cn/Article/details/gcvkkymfg.sHtML

[U29] Py：属性校验
来源：http://www.blog.sjlbkw.cn/Article/details/gdthmbumx.sHtML

@property 与 @x.setter 配合
来源：http://read.share.epnwcf.com/Article/details/gciysxtzp.sHtML

[U30] Py：数据类
来源：http://read.share.vehdjk.com/Article/details/gocrwipni.sHtML

@dataclass(slots=True)
来源：http://3g.fktsv.cn/Article/details/gajdbatrf.sHtML

[U31] Py：单测
来源：http://www.blog.yfazqb.com/Article/details/gyuazkaoh.sHtML

python -m pytest -q
来源：http://www.share.bbcook.cn/Article/details/gnuwnsdul.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.yfazqb.com/Article/details/gmslljxjm.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.sjlbkw.cn/Article/details/gjqvfbsoo.sHtML

[U33] Py：打包发布
来源：http://wap.yfazqb.com/Article/details/gxapssigv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.bbcook.cn/Article/details/grtfxopuj.sHtML

[U34] Py：判断编码
来源：http://baike.fktsv.cn/Article/details/gaxufwgmx.sHtML

chardet.detect(raw)
来源：http://baike.fktsv.cn/Article/details/gqgyvctxg.sHtML

[U35] Py：发送邮件
来源：http://baike.fktsv.cn/Article/details/givqlwfhb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.tarul.cn/Article/details/gykbxlter.sHtML

[U36] Py：定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gidkreqri.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.yfazqb.com/Article/details/gewggjqiv.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.bbcook.cn/Article/details/gdyxjeeld.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fktsv.cn/Article/details/goglikqui.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.vehdjk.com/Article/details/gifwtyiyq.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fktsv.cn/Article/details/gxfkuhcfi.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.sjlbkw.cn/Article/details/gdpllrgsb.sHtML

sys.stdout.isatty()
来源：http://3g.sjlbkw.cn/Article/details/gosyisjaj.sHtML

[U40] Py：打印到标准错误
来源：http://blog.epnwcf.com/Article/details/gslhtsdvd.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gxiodoruy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.sjlbkw.cn/Article/details/gohekezwg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.bbcook.cn/Article/details/gbckosvzj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.tarul.cn/Article/details/gfcufiche.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.sjlbkw.cn/Article/details/gatkydywf.sHtML

[U43] PHP：声明命名空间
来源：http://3g.epnwcf.com/Article/details/gtztrgjdz.sHtML

namespace App\Http;
来源：http://www.m.share.fktsv.cn/Article/details/gemkqogpi.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.tarul.cn/Article/details/gmgnndahz.sHtML

declare(strict_types=1);
来源：http://m.share.bbcook.cn/Article/details/gsgwrwnlf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.vehdjk.com/Article/details/gzsjmefnm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gnxtosimp.sHtML

[U46] PHP：可空类型
来源：http://m.share.sjlbkw.cn/Article/details/gjsdiplii.sHtML

?string $name = null
来源：http://www.blog.tarul.cn/Article/details/gllxhivdt.sHtML

[U47] PHP：联合类型
来源：http://m.share.fktsv.cn/Article/details/gruyyuiqb.sHtML

int|string $id
来源：http://m.share.tarul.cn/Article/details/gqutvgqnv.sHtML

[U48] PHP：纯枚举
来源：http://blog.sjlbkw.cn/Article/details/gizbixgpi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fktsv.cn/Article/details/gjnhgexzy.sHtML

[U49] PHP：只读属性
来源：http://www.blog.bbcook.cn/Article/details/glltlpygl.sHtML

public readonly string $name
来源：http://mobile.fktsv.cn/Article/details/gbqrpopsi.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.tarul.cn/Article/details/grdpophwu.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.vehdjk.com/Article/details/gwtopywys.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fktsv.cn/Article/details/giicopqlx.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.tarul.cn/Article/details/ghbmgfiho.sHtML

[U52] PHP：箭头函数
来源：http://wap.fktsv.cn/Article/details/gbnazcivn.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.epnwcf.com/Article/details/ghxezheva.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.sjlbkw.cn/Article/details/gutvqtvxi.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.epnwcf.com/Article/details/gkuwbsinm.sHtML

[U54] PHP：空安全调用
来源：http://baike.vehdjk.com/Article/details/grjaqtvee.sHtML

$obj?->method()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfriubdot.sHtML

[U55] PHP：match 表达式
来源：http://3g.tarul.cn/Article/details/gwugjemls.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.epnwcf.com/Article/details/ggvdkyjuv.sHtML

[U56] PHP：命名参数
来源：http://www.share.bbcook.cn/Article/details/gxfzunckq.sHtML

f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/ghzuayirq.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gpfdjhdja.sHtML

"值: {$a}"
来源：http://blog.epnwcf.com/Article/details/gmehgpajl.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fktsv.cn/Article/details/gmjcumbux.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.bbcook.cn/Article/details/gxbkgepso.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdmwurji.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.yfazqb.com/Article/details/gqnfjrkui.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.epnwcf.com/Article/details/ghtkomgkz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.epnwcf.com/Article/details/gnjiwdpbd.sHtML

[U61] PHP：正则
来源：http://baike.yfazqb.com/Article/details/gayktnbxv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/gingrkbbb.sHtML

[U62] PHP：日期对象
来源：http://blog.tarul.cn/Article/details/gvilhwfwa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fktsv.cn/Article/details/gabxhwtbg.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.sjlbkw.cn/Article/details/gvoqkibui.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.vehdjk.com/Article/details/gubbhjxjg.sHtML

[U64] PHP：目录遍历
来源：http://mobile.sjlbkw.cn/Article/details/gklixmsdf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.yfazqb.com/Article/details/gzitherhk.sHtML

[U65] PHP：会话
来源：http://m.share.fktsv.cn/Article/details/gjkxkrwyp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.epnwcf.com/Article/details/gicuhaies.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.yfazqb.com/Article/details/gtxhhiirn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.tarul.cn/Article/details/ghtxsictw.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.tarul.cn/Article/details/gdgbyknfo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.vehdjk.com/Article/details/gwiungqdr.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.tarul.cn/Article/details/gciojyjii.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.bbcook.cn/Article/details/gsouadebp.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.epnwcf.com/Article/details/gftoqcubc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.epnwcf.com/Article/details/ggtodipoi.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.yfazqb.com/Article/details/gffbgbshj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.tarul.cn/Article/details/gelnltjny.sHtML

[U71] PHP：抛出异常
来源：http://mobile.tarul.cn/Article/details/gqpgtvley.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.sjlbkw.cn/Article/details/gaqdltmux.sHtML

[U72] PHP：写错误日志
来源：http://baike.sjlbkw.cn/Article/details/gzyabipat.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.epnwcf.com/Article/details/gguvgmarb.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.sjlbkw.cn/Article/details/grtkqfhxi.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.tarul.cn/Article/details/gfnadmjqh.sHtML

[U74] PHP：读取环境变量
来源：http://wap.vehdjk.com/Article/details/gqquyvjpo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.bbcook.cn/Article/details/gxehbsxcf.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fktsv.cn/Article/details/gviesoqtg.sHtML

composer require psr/container
来源：http://www.share.vehdjk.com/Article/details/gpwmjkeab.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fktsv.cn/Article/details/gvhefbihy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.bbcook.cn/Article/details/gpfnicnwg.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.sjlbkw.cn/Article/details/gkbqhjahj.sHtML

composer require twig/twig
来源：http://m.share.sjlbkw.cn/Article/details/gznmoqtxy.sHtML

[U78] PHP：单元测试
来源：http://www.blog.vehdjk.com/Article/details/gbzxfykju.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.tarul.cn/Article/details/gzdtlkvod.sHtML

[U79] PHP：静态分析
来源：http://read.share.vehdjk.com/Article/details/gzsxgymhc.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.bbcook.cn/Article/details/guddhklci.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.tarul.cn/Article/details/gvbkzxhou.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.bbcook.cn/Article/details/gkpigteux.sHtML

[U81] JS：初始化项目
来源：http://www.blog.yfazqb.com/Article/details/gkieruqis.sHtML

npm init -y;  npm i express
来源：http://www.share.yfazqb.com/Article/details/gwpsrmmkt.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.yfazqb.com/Article/details/gksrphvfd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.epnwcf.com/Article/details/ghwvlxjza.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.vehdjk.com/Article/details/gkedffdnk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.bbcook.cn/Article/details/gzgnrolkb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.sjlbkw.cn/Article/details/gqwzfurvn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.tarul.cn/Article/details/gxshvjkvc.sHtML

[U85] JS：可选链
来源：http://www.m.share.yfazqb.com/Article/details/ghlbalpxi.sHtML

a?.b?.c
来源：http://www.blog.fktsv.cn/Article/details/gelgvyfqa.sHtML

[U86] JS：空值合并
来源：http://3g.epnwcf.com/Article/details/gsgmfljwv.sHtML

a ?? b
来源：http://read.share.fktsv.cn/Article/details/gagjqnewc.sHtML

[U87] JS：解构默认值
来源：http://www.blog.vehdjk.com/Article/details/gplodmxqg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.vehdjk.com/Article/details/gtaprjtbj.sHtML

[U88] JS：对象展开合并
来源：http://blog.bbcook.cn/Article/details/gbekmezfn.sHtML

{ ...a, ...b }
来源：http://blog.tarul.cn/Article/details/gjqumljpu.sHtML

[U89] JS：数组去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmkmgsvw.sHtML

[...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/glmtccczx.sHtML

[U90] JS：数字数组排序
来源：http://www.share.vehdjk.com/Article/details/gxaimoazq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gzkwiyqti.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.tarul.cn/Article/details/gtfdlyycc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fktsv.cn/Article/details/gvtrenhyo.sHtML

[U92] JS：深拷贝
来源：http://3g.bbcook.cn/Article/details/ggeulsnfg.sHtML

structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gwfteqala.sHtML

[U93] JS：模板字符串
来源：http://3g.fktsv.cn/Article/details/ggbdyripe.sHtML

`共 ${n} 条`
来源：http://www.blog.vehdjk.com/Article/details/gudmwbwhn.sHtML

[U94] JS：箭头函数
来源：http://www.share.tarul.cn/Article/details/gwxfqrmxe.sHtML

const double = x => x * 2;
来源：http://www.blog.yfazqb.com/Article/details/glhdjhzmn.sHtML

[U95] JS：Promise 包装
来源：http://m.share.sjlbkw.cn/Article/details/gbepvcjev.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fktsv.cn/Article/details/gydxgoqrj.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fktsv.cn/Article/details/grdsmvyah.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gxzmpkoyl.sHtML

[U97] JS：并发请求
来源：http://baike.vehdjk.com/Article/details/ghvwrefys.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gsdkdrbkm.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.bbcook.cn/Article/details/gyfitqcfl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fktsv.cn/Article/details/gohmdzkwn.sHtML

[U99] JS：事件监听
来源：http://www.m.share.yfazqb.com/Article/details/gpykeoeup.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.bbcook.cn/Article/details/grqtnulti.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fktsv.cn/Article/details/gqwjcvucr.sHtML

document.querySelector(".item")
来源：http://www.share.yfazqb.com/Article/details/ghefblbej.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.tarul.cn/Article/details/ggkulkecp.sHtML

el.classList.toggle("active")
来源：http://read.share.yfazqb.com/Article/details/gmdmawidz.sHtML

[U102] JS：本地存储
来源：http://www.m.share.tarul.cn/Article/details/ghwdycaea.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.epnwcf.com/Article/details/gytqkzddd.sHtML

[U103] JS：定时器
来源：http://3g.sjlbkw.cn/Article/details/gjxrmjvdg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.tarul.cn/Article/details/gscviwmdg.sHtML

[U104] JS：防抖
来源：http://3g.epnwcf.com/Article/details/gxjhxsorx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/girttfjkt.sHtML

[U105] JS：节流
来源：http://read.share.vehdjk.com/Article/details/gezultgfx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.yfazqb.com/Article/details/ggndvoyik.sHtML

[U106] JS：日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gnrmkdwxk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fktsv.cn/Article/details/gmfxgdkpg.sHtML

[U107] JS：数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gfydgzsms.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.bbcook.cn/Article/details/gkixkqzle.sHtML

[U108] JS：随机整数
来源：http://www.blog.epnwcf.com/Article/details/gxfnbuuhc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.yfazqb.com/Article/details/gybbnhott.sHtML

[U109] JS：数组分组
来源：http://www.share.tarul.cn/Article/details/gdpjcwfoq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.tarul.cn/Article/details/gijfynuho.sHtML

[U110] JS：数组分块
来源：http://baike.sjlbkw.cn/Article/details/gfsoezdxc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.sjlbkw.cn/Article/details/gezgpxing.sHtML

[U111] JS：对象转 Map
来源：http://mobile.epnwcf.com/Article/details/gtaxbgppa.sHtML

new Map(Object.entries(obj))
来源：http://wap.epnwcf.com/Article/details/gmfntqfmi.sHtML

[U112] JS：字符串补位
来源：http://mobile.sjlbkw.cn/Article/details/gnpunxxmt.sHtML

"7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gpwidvyqp.sHtML

[U113] JS：正则替换全部
来源：http://wap.bbcook.cn/Article/details/gtoyfmbxf.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gsnzmjzyu.sHtML

[U114] JS：JSON 深比较
来源：http://3g.yfazqb.com/Article/details/gfqcodbfn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.sjlbkw.cn/Article/details/gvlrhxzpz.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/gqiqoxpks.sHtML

crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gdttghszl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fktsv.cn/Article/details/gdobleozt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.vehdjk.com/Article/details/grwlmtvbc.sHtML

[U117] JS：单元测试
来源：http://blog.fktsv.cn/Article/details/gshmdtkgg.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.bbcook.cn/Article/details/gcfwihxqh.sHtML

[U118] JS：开发服务器
来源：http://m.share.vehdjk.com/Article/details/gmoawenqf.sHtML

npm i -D vite;  npx vite
来源：http://3g.vehdjk.com/Article/details/gmvkjupay.sHtML

[U119] JS：生产构建
来源：http://baike.vehdjk.com/Article/details/gmhkwtubh.sHtML

npx vite build
来源：http://3g.tarul.cn/Article/details/gglfphcrw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.vehdjk.com/Article/details/gskzbdsxl.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.bbcook.cn/Article/details/gnwjzltdp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gppwyecgn.sHtML

统计汇总
来源：http://m.share.bbcook.cn/Article/details/gbcaelitq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gecakqjoa.sHtML

按语言统计（条）：
来源：http://wap.fktsv.cn/Article/details/gdoewhnve.sHtML

Python ......... 252
来源：http://blog.epnwcf.com/Article/details/gbixbcqir.sHtML

PHP ............ 252
来源：http://www.m.share.epnwcf.com/Article/details/gppvlogzf.sHtML

JavaScript ..... 252
来源：http://wap.yfazqb.com/Article/details/gthydauth.sHtML

TypeScript ..... 212
来源：http://wap.vehdjk.com/Article/details/gftjlhpwn.sHtML

Java ........... 212
来源：http://wap.sjlbkw.cn/Article/details/gkadedaeu.sHtML

Go ............. 212
来源：http://wap.tarul.cn/Article/details/guuxmubfb.sHtML

Ruby ........... 212
来源：http://mobile.epnwcf.com/Article/details/gfgwjjqqq.sHtML

C# ............. 212
来源：http://www.share.vehdjk.com/Article/details/gyckfjekq.sHtML

C .............. 30
来源：http://www.share.epnwcf.com/Article/details/gdjbpwrus.sHtML

C++ ............ 30
来源：http://blog.epnwcf.com/Article/details/gliogucwg.sHtML

SQL ............ 90
来源：http://wap.bbcook.cn/Article/details/ghboimokt.sHtML

Bash ........... 80
来源：http://read.share.epnwcf.com/Article/details/grnvtqudr.sHtML

Kotlin ......... 15
来源：http://mobile.vehdjk.com/Article/details/giwyugywk.sHtML

Swift .......... 15
来源：http://www.blog.bbcook.cn/Article/details/gtvloicso.sHtML

Lua ............ 10
来源：http://www.m.share.epnwcf.com/Article/details/gqofczawq.sHtML

Perl ........... 10
来源：http://www.share.vehdjk.com/Article/details/gapygsfnm.sHtML

Scala .......... 10
来源：http://www.blog.vehdjk.com/Article/details/gjwqpgoso.sHtML

------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gqpuerfds.sHtML

合计 ........... 2106 条
来源：http://mobile.fktsv.cn/Article/details/gwgpyaxvl.sHtML

按章节统计：
来源：http://baike.vehdjk.com/Article/details/gtibbhcez.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.sjlbkw.cn/Article/details/gqqcxexif.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gktfyehbw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/gcsplehyh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.yfazqb.com/Article/details/glexgfxsy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.sjlbkw.cn/Article/details/gkfgabdeq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/glhzmolvs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gjyretkta.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/gafxbngvg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gryjkrnso.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.epnwcf.com/Article/details/gutvfpwbq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/ggzuviarz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gxqvbfioc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/ggrkiqlvb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.tarul.cn/Article/details/gwzaztiem.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.sjlbkw.cn/Article/details/gzmnezhkg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/gylwrbomi.sHtML

Q SQL 专题                              90
来源：http://www.share.fktsv.cn/Article/details/gogzjqiep.sHtML

R Bash 专题                             80
来源：http://mobile.fktsv.cn/Article/details/gcapxtqbm.sHtML

S C / C++ 专题                          60
来源：http://www.share.epnwcf.com/Article/details/gascnuwkx.sHtML

T 其他语言补充                          60
来源：http://wap.bbcook.cn/Article/details/gsubbwsls.sHtML

U 高频实用片段                         120
来源：http://www.share.yfazqb.com/Article/details/gjzdgqdnf.sHtML

------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gmlogubug.sHtML

合计                                  2106 条
来源：http://baike.fktsv.cn/Article/details/gixoedzwb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gbdjurrso.sHtML

使用提醒
来源：http://read.share.yfazqb.com/Article/details/gsgdtnhcg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/gceotmynq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.yfazqb.com/Article/details/gdtznkbci.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.tarul.cn/Article/details/ggitpcoyb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.vehdjk.com/Article/details/gezleolbu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.sjlbkw.cn/Article/details/gtfstnjsq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.epnwcf.com/Article/details/gxpregwxg.sHtML

—— 文件结束 ——
来源：http://read.share.fktsv.cn/Article/details/ghrzaswif.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gxfkjvcdz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fktsv.cn/Article/details/gaiozzscq.sHtML

Common Programming Examples Cheat Book
来源：http://baike.vehdjk.com/Article/details/gxhuuhian.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtzfnjvzw.sHtML

【收录内容】
来源：http://www.blog.sjlbkw.cn/Article/details/gesvjonav.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.vehdjk.com/Article/details/gozbymlop.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.epnwcf.com/Article/details/gavzsrfqv.sHtML

SQL · Bash · C · C++
来源：http://baike.epnwcf.com/Article/details/gizcxgmga.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.bbcook.cn/Article/details/gkfbjvgqo.sHtML

【使用说明】
来源：http://mobile.yfazqb.com/Article/details/gyrvkcvcf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.vehdjk.com/Article/details/grvvwypah.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.epnwcf.com/Article/details/gwunryncw.sHtML


<!-- 参考信息 -->