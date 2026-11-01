代发 wailian999

[U07] Py：反转字典键值
来源：http://baike.epnwcf.com/Article/details/gdnlzheal.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.bbcook.cn/Article/details/gzsqdezmw.sHtML

[U08] Py：展平二维列表
来源：http://3g.epnwcf.com/Article/details/gvuseupwa.sHtML

[y for x in nested for y in x]
来源：http://3g.tarul.cn/Article/details/gqzmmeagz.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.vehdjk.com/Article/details/gcbdiwkrl.sHtML

max(d, key=d.get)
来源：http://wap.epnwcf.com/Article/details/gbejriugn.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fktsv.cn/Article/details/gdxnvsqur.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.tarul.cn/Article/details/gpxojtxgs.sHtML

[U11] Py：生成器表达式
来源：http://wap.epnwcf.com/Article/details/grehswdqa.sHtML

(x * 2 for x in arr)
来源：http://m.share.epnwcf.com/Article/details/gswftsozb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.epnwcf.com/Article/details/gpcvvsgqo.sHtML

Counter(arr).most_common(3)
来源：http://m.share.sjlbkw.cn/Article/details/garbdpmyp.sHtML

[U13] Py：固定长度队列
来源：http://www.share.yfazqb.com/Article/details/gxumjxenw.sHtML

deque(maxlen=10)
来源：http://read.share.vehdjk.com/Article/details/gfduhfrdv.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.vehdjk.com/Article/details/ghuyeknru.sHtML

defaultdict(list)
来源：http://read.share.sjlbkw.cn/Article/details/glfoghupe.sHtML

[U15] Py：高精度计时
来源：http://read.share.vehdjk.com/Article/details/ghyluyvnd.sHtML

t = time.perf_counter()
来源：http://baike.vehdjk.com/Article/details/ggwlmwjfw.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fktsv.cn/Article/details/gyluuwwbt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgybtfgy.sHtML

[U17] Py：初始化日志
来源：http://baike.tarul.cn/Article/details/gyebtlvrh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.bbcook.cn/Article/details/gtnxjivtk.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.epnwcf.com/Article/details/geelzngjx.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.sjlbkw.cn/Article/details/gjlbwwapg.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.vehdjk.com/Article/details/gkrseixqo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.tarul.cn/Article/details/gsyxgudoq.sHtML

[U20] Py：缓存函数结果
来源：http://baike.vehdjk.com/Article/details/gozrzcjiu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.vehdjk.com/Article/details/gejvgumge.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.sjlbkw.cn/Article/details/gocfibuyv.sHtML

@contextlib.contextmanager
来源：http://www.m.share.vehdjk.com/Article/details/grssxyreu.sHtML

[U22] Py：矩阵转置
来源：http://www.share.yfazqb.com/Article/details/gznbtqrmd.sHtML

list(zip(*m))
来源：http://www.m.share.vehdjk.com/Article/details/gtojckzqa.sHtML

[U23] Py：分块读取大文件
来源：http://baike.epnwcf.com/Article/details/gueqjqyik.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.yfazqb.com/Article/details/ghtuvkjdw.sHtML

[U24] Py：路径操作
来源：http://baike.fktsv.cn/Article/details/gzfkxcpak.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.sjlbkw.cn/Article/details/gyhuvumqo.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.bbcook.cn/Article/details/gxoiqdezy.sHtML

csv.DictReader(f)
来源：http://www.m.share.fktsv.cn/Article/details/gqlehkxhg.sHtML

[U26] Py：并发下载
来源：http://m.share.tarul.cn/Article/details/gdesttuyl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.sjlbkw.cn/Article/details/gqcnbxwgx.sHtML

[U27] Py：异步 HTTP
来源：http://3g.bbcook.cn/Article/details/gfowllinl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdmfyiuj.sHtML

[U28] Py：类型别名
来源：http://mobile.tarul.cn/Article/details/gowishzfz.sHtML

UserId = int
来源：http://wap.yfazqb.com/Article/details/ghcesfpjt.sHtML

[U29] Py：属性校验
来源：http://www.blog.sjlbkw.cn/Article/details/gxumfaopn.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.vehdjk.com/Article/details/grvxfscbs.sHtML

[U30] Py：数据类
来源：http://www.share.yfazqb.com/Article/details/gtwygkcxl.sHtML

@dataclass(slots=True)
来源：http://www.blog.tarul.cn/Article/details/gmwfegdzg.sHtML

[U31] Py：单测
来源：http://www.blog.epnwcf.com/Article/details/guaxlskcu.sHtML

python -m pytest -q
来源：http://3g.yfazqb.com/Article/details/gnncrmmvj.sHtML

[U32] Py：代码格式化
来源：http://mobile.yfazqb.com/Article/details/gzaotclnk.sHtML

ruff format . && ruff check --fix .
来源：http://wap.epnwcf.com/Article/details/glkdhhckl.sHtML

[U33] Py：打包发布
来源：http://mobile.vehdjk.com/Article/details/gtuwuefhy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.yfazqb.com/Article/details/gknuaitju.sHtML

[U34] Py：判断编码
来源：http://blog.epnwcf.com/Article/details/gqxqsmwfw.sHtML

chardet.detect(raw)
来源：http://mobile.vehdjk.com/Article/details/glaspsyrl.sHtML

[U35] Py：发送邮件
来源：http://blog.yfazqb.com/Article/details/gphbddpou.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.tarul.cn/Article/details/gwktezgtm.sHtML

[U36] Py：定时任务
来源：http://blog.fktsv.cn/Article/details/gqncfoarp.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.vehdjk.com/Article/details/gmdmhztpr.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/gmabbyecm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.tarul.cn/Article/details/gbycibvma.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.vehdjk.com/Article/details/gskedsedx.sHtML

Path(__file__).resolve().parent
来源：http://baike.vehdjk.com/Article/details/gimmcqxbo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.tarul.cn/Article/details/gdvlroogw.sHtML

sys.stdout.isatty()
来源：http://baike.epnwcf.com/Article/details/gnretnjkm.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fktsv.cn/Article/details/gydvykxdw.sHtML

print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gbtioknng.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.yfazqb.com/Article/details/gdllmpuxw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.epnwcf.com/Article/details/gryteenqc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.epnwcf.com/Article/details/gkltikjtk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fktsv.cn/Article/details/gvcjffcib.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.vehdjk.com/Article/details/ggeecvzkg.sHtML

namespace App\Http;
来源：http://3g.fktsv.cn/Article/details/gwyzxdllp.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.epnwcf.com/Article/details/gsixcqyfk.sHtML

declare(strict_types=1);
来源：http://3g.bbcook.cn/Article/details/gqoiuecct.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.vehdjk.com/Article/details/ggcsujfey.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gnigeuxsl.sHtML

[U46] PHP：可空类型
来源：http://www.share.sjlbkw.cn/Article/details/gbuyxypyo.sHtML

?string $name = null
来源：http://m.share.sjlbkw.cn/Article/details/ghqneogyd.sHtML

[U47] PHP：联合类型
来源：http://3g.tarul.cn/Article/details/gpgnogifl.sHtML

int|string $id
来源：http://www.share.bbcook.cn/Article/details/gceztatke.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fktsv.cn/Article/details/gmbtmarun.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjelzseof.sHtML

[U49] PHP：只读属性
来源：http://m.share.epnwcf.com/Article/details/gntxumvgx.sHtML

public readonly string $name
来源：http://blog.vehdjk.com/Article/details/gezfokptl.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.vehdjk.com/Article/details/gytzbunih.sHtML

public function __construct(private int $id) {}
来源：http://www.share.epnwcf.com/Article/details/gjudeynet.sHtML

[U51] PHP：数组解构
来源：http://blog.bbcook.cn/Article/details/gplnetwps.sHtML

[$a, $b] = $arr;
来源：http://wap.bbcook.cn/Article/details/gobzuonbh.sHtML

[U52] PHP：箭头函数
来源：http://www.share.bbcook.cn/Article/details/gsrczzteb.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.epnwcf.com/Article/details/gigphbbmr.sHtML

[U53] PHP：空合并运算符
来源：http://baike.epnwcf.com/Article/details/gsztqlzhv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fktsv.cn/Article/details/grtbaheky.sHtML

[U54] PHP：空安全调用
来源：http://m.share.epnwcf.com/Article/details/ghgoexdmw.sHtML

$obj?->method()
来源：http://read.share.fktsv.cn/Article/details/geksdnyvq.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.tarul.cn/Article/details/grghuabmr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.yfazqb.com/Article/details/gwqfpbamk.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fktsv.cn/Article/details/gmkxnwbve.sHtML

f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gjfomvtpl.sHtML

[U57] PHP：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gkegybygf.sHtML

"值: {$a}"
来源：http://blog.vehdjk.com/Article/details/gmkkdgurq.sHtML

[U58] PHP：数组三件套
来源：http://m.share.yfazqb.com/Article/details/gsalpqyvm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.yfazqb.com/Article/details/gtoxxlqgl.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.bbcook.cn/Article/details/gsvutwwge.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.bbcook.cn/Article/details/gplplnord.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.sjlbkw.cn/Article/details/gzkppzcvo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.epnwcf.com/Article/details/gxcxtxaou.sHtML

[U61] PHP：正则
来源：http://www.blog.yfazqb.com/Article/details/gapksuftb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/gzabijtbt.sHtML

[U62] PHP：日期对象
来源：http://3g.tarul.cn/Article/details/gnyksroiv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.vehdjk.com/Article/details/gqkoqkizv.sHtML

[U63] PHP：文件读写
来源：http://3g.bbcook.cn/Article/details/gtynkxhxv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fktsv.cn/Article/details/glwgzigxm.sHtML

[U64] PHP：目录遍历
来源：http://blog.bbcook.cn/Article/details/gmrtuqygj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fktsv.cn/Article/details/goebxoqrx.sHtML

[U65] PHP：会话
来源：http://www.m.share.vehdjk.com/Article/details/gtwurvycx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.yfazqb.com/Article/details/grbkwubjx.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.bbcook.cn/Article/details/geukcvmqq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.yfazqb.com/Article/details/gpverdods.sHtML

[U67] PHP：处理文件上传
来源：http://blog.sjlbkw.cn/Article/details/gaajeyngg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.sjlbkw.cn/Article/details/gxnjiiymk.sHtML

[U68] PHP：PDO 连接
来源：http://baike.epnwcf.com/Article/details/givdfgnry.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.tarul.cn/Article/details/gixnhjyvb.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.sjlbkw.cn/Article/details/gfeznjisu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fktsv.cn/Article/details/gsswmchdd.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fktsv.cn/Article/details/gvtpezvwb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.epnwcf.com/Article/details/ggxaurvmg.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gychlnkfo.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.tarul.cn/Article/details/gqqvzahmx.sHtML

[U72] PHP：写错误日志
来源：http://www.share.yfazqb.com/Article/details/gebsgleoj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.bbcook.cn/Article/details/gipyfxkcv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fktsv.cn/Article/details/gkdildxmy.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.bbcook.cn/Article/details/gaanucjgf.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fktsv.cn/Article/details/gtkrsatml.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.yfazqb.com/Article/details/gitscwugb.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.epnwcf.com/Article/details/ghotmbnbh.sHtML

composer require psr/container
来源：http://www.share.tarul.cn/Article/details/gkahcwnov.sHtML

[U76] PHP：简单路由
来源：http://www.share.tarul.cn/Article/details/gfgnhnjfp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.epnwcf.com/Article/details/gzycjmnut.sHtML

[U77] PHP：模板渲染
来源：http://www.share.epnwcf.com/Article/details/gwlbwicns.sHtML

composer require twig/twig
来源：http://www.share.tarul.cn/Article/details/gdkofdqrm.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.yfazqb.com/Article/details/gnpjkqhet.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fktsv.cn/Article/details/gmjroxfge.sHtML

[U79] PHP：静态分析
来源：http://wap.vehdjk.com/Article/details/gduuhugln.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.vehdjk.com/Article/details/gkjamatsu.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.sjlbkw.cn/Article/details/gkpxbetuh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.sjlbkw.cn/Article/details/gupskikmv.sHtML

[U81] JS：初始化项目
来源：http://www.share.yfazqb.com/Article/details/gdoqptxil.sHtML

npm init -y;  npm i express
来源：http://m.share.vehdjk.com/Article/details/gxvlziyko.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.bbcook.cn/Article/details/gsswzrpwk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.tarul.cn/Article/details/gmxzpgdvn.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.tarul.cn/Article/details/gtqccvter.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwrtbrvv.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.sjlbkw.cn/Article/details/gzqihgwuf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.yfazqb.com/Article/details/gsnarwscc.sHtML

[U85] JS：可选链
来源：http://mobile.fktsv.cn/Article/details/gfmbshdsb.sHtML

a?.b?.c
来源：http://3g.epnwcf.com/Article/details/gxpfxjelo.sHtML

[U86] JS：空值合并
来源：http://baike.tarul.cn/Article/details/gorvdnwyv.sHtML

a ?? b
来源：http://www.share.sjlbkw.cn/Article/details/gcpckdtsd.sHtML

[U87] JS：解构默认值
来源：http://m.share.sjlbkw.cn/Article/details/grmfudnfg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.epnwcf.com/Article/details/gzjkiqhzp.sHtML

[U88] JS：对象展开合并
来源：http://read.share.sjlbkw.cn/Article/details/gvmktfvii.sHtML

{ ...a, ...b }
来源：http://www.share.vehdjk.com/Article/details/gmuslhvrc.sHtML

[U89] JS：数组去重
来源：http://www.blog.epnwcf.com/Article/details/ggpbevwxc.sHtML

[...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gpmmuvnwx.sHtML

[U90] JS：数字数组排序
来源：http://read.share.epnwcf.com/Article/details/gmhjriwof.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gfavlrrom.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.vehdjk.com/Article/details/gsxabnhwn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.sjlbkw.cn/Article/details/ggeukckyo.sHtML

[U92] JS：深拷贝
来源：http://3g.vehdjk.com/Article/details/giiaysaul.sHtML

structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gyoeoyigd.sHtML

[U93] JS：模板字符串
来源：http://m.share.fktsv.cn/Article/details/gcecgvtpx.sHtML

`共 ${n} 条`
来源：http://read.share.vehdjk.com/Article/details/gfhgiuewf.sHtML

[U94] JS：箭头函数
来源：http://www.share.tarul.cn/Article/details/gvwfqqeqb.sHtML

const double = x => x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/glyksjals.sHtML

[U95] JS：Promise 包装
来源：http://wap.epnwcf.com/Article/details/gnpkcikcj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fktsv.cn/Article/details/glejgyvpj.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.bbcook.cn/Article/details/guwhicnwk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gyjqrhphz.sHtML

[U97] JS：并发请求
来源：http://baike.yfazqb.com/Article/details/gaijnuxps.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/grtkxrajj.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fktsv.cn/Article/details/grqxfidnv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.epnwcf.com/Article/details/geighusnk.sHtML

[U99] JS：事件监听
来源：http://blog.yfazqb.com/Article/details/gbwiynpva.sHtML

el.addEventListener("click", e => {})
来源：http://3g.tarul.cn/Article/details/gvfsixune.sHtML

[U100] JS：DOM 查询
来源：http://blog.bbcook.cn/Article/details/gauthkkdl.sHtML

document.querySelector(".item")
来源：http://read.share.epnwcf.com/Article/details/givitaook.sHtML

[U101] JS：classList 操作
来源：http://read.share.fktsv.cn/Article/details/ggxvxlbnb.sHtML

el.classList.toggle("active")
来源：http://blog.sjlbkw.cn/Article/details/gbtjcjlce.sHtML

[U102] JS：本地存储
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhjlzcxm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.vehdjk.com/Article/details/gqpgdxwpy.sHtML

[U103] JS：定时器
来源：http://m.share.yfazqb.com/Article/details/gvivehkwg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.sjlbkw.cn/Article/details/gysegcsha.sHtML

[U104] JS：防抖
来源：http://m.share.yfazqb.com/Article/details/gfsbjlztq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gepwogwwn.sHtML

[U105] JS：节流
来源：http://baike.fktsv.cn/Article/details/gvwmdykpa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.vehdjk.com/Article/details/gbvhvsfny.sHtML

[U106] JS：日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gqaicbmxg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.vehdjk.com/Article/details/gbaggywvd.sHtML

[U107] JS：数字千分位
来源：http://baike.tarul.cn/Article/details/gwbixdwte.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fktsv.cn/Article/details/gxgeiscsb.sHtML

[U108] JS：随机整数
来源：http://www.blog.sjlbkw.cn/Article/details/gtadnrhdm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.tarul.cn/Article/details/geslbhsdl.sHtML

[U109] JS：数组分组
来源：http://blog.epnwcf.com/Article/details/golqxdkns.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/gajmnlhjb.sHtML

[U110] JS：数组分块
来源：http://blog.fktsv.cn/Article/details/gbhlmftcs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.vehdjk.com/Article/details/gckojkdtr.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fktsv.cn/Article/details/gqmgoajxs.sHtML

new Map(Object.entries(obj))
来源：http://read.share.vehdjk.com/Article/details/gzaedjmjq.sHtML

[U112] JS：字符串补位
来源：http://www.share.tarul.cn/Article/details/gfdsdwxzk.sHtML

"7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gyvdbdsbf.sHtML

[U113] JS：正则替换全部
来源：http://wap.bbcook.cn/Article/details/gunxlieti.sHtML

s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/glupwhotc.sHtML

[U114] JS：JSON 深比较
来源：http://3g.bbcook.cn/Article/details/gpepqftkg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gqqcejbcx.sHtML

[U115] JS：生成 UUID
来源：http://m.share.epnwcf.com/Article/details/gpbcstwug.sHtML

crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gbxehincc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.yfazqb.com/Article/details/gaxdfirds.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.yfazqb.com/Article/details/gpzpwqskc.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gwlubptvf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fktsv.cn/Article/details/glmqgwcdv.sHtML

[U118] JS：开发服务器
来源：http://3g.tarul.cn/Article/details/gmxpycdnb.sHtML

npm i -D vite;  npx vite
来源：http://m.share.yfazqb.com/Article/details/gswhydpfs.sHtML

[U119] JS：生产构建
来源：http://3g.yfazqb.com/Article/details/gvponyyfh.sHtML

npx vite build
来源：http://mobile.vehdjk.com/Article/details/gtvcrezbn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fktsv.cn/Article/details/gsvkqiihi.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.yfazqb.com/Article/details/gqplemnbf.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gztvonfyl.sHtML

统计汇总
来源：http://wap.tarul.cn/Article/details/gymvnwjgo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ggtuiqddb.sHtML

按语言统计（条）：
来源：http://wap.yfazqb.com/Article/details/gdkljcehe.sHtML

Python ......... 252
来源：http://3g.sjlbkw.cn/Article/details/gtjkwpwoy.sHtML

PHP ............ 252
来源：http://read.share.tarul.cn/Article/details/gxfqttwvd.sHtML

JavaScript ..... 252
来源：http://baike.bbcook.cn/Article/details/gannyskaq.sHtML

TypeScript ..... 212
来源：http://wap.vehdjk.com/Article/details/grhcjtchh.sHtML

Java ........... 212
来源：http://www.m.share.vehdjk.com/Article/details/ggfsuencm.sHtML

Go ............. 212
来源：http://wap.bbcook.cn/Article/details/gpimkdqgi.sHtML

Ruby ........... 212
来源：http://wap.yfazqb.com/Article/details/gffkkgcna.sHtML

C# ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/ghiaoaher.sHtML

C .............. 30
来源：http://baike.vehdjk.com/Article/details/gvyrpgbqe.sHtML

C++ ............ 30
来源：http://mobile.vehdjk.com/Article/details/gliwuerqn.sHtML

SQL ............ 90
来源：http://3g.vehdjk.com/Article/details/gftinquao.sHtML

Bash ........... 80
来源：http://blog.tarul.cn/Article/details/gzfvqjdwt.sHtML

Kotlin ......... 15
来源：http://www.m.share.tarul.cn/Article/details/gqbfdywlh.sHtML

Swift .......... 15
来源：http://mobile.tarul.cn/Article/details/gojtgjfks.sHtML

Lua ............ 10
来源：http://www.m.share.sjlbkw.cn/Article/details/ghetqhkeb.sHtML

Perl ........... 10
来源：http://baike.fktsv.cn/Article/details/gbdbeqrvu.sHtML

Scala .......... 10
来源：http://blog.bbcook.cn/Article/details/gjmgwsyts.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gvgufrgsv.sHtML

合计 ........... 2106 条
来源：http://wap.tarul.cn/Article/details/gxunwppjh.sHtML

按章节统计：
来源：http://m.share.epnwcf.com/Article/details/gxfbwmikv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.yfazqb.com/Article/details/gpvzircir.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gcsbyovfq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gchnsmpoi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/gebtrfrod.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.sjlbkw.cn/Article/details/gcqhmpmmw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.epnwcf.com/Article/details/ggukswumv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gescalggr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fktsv.cn/Article/details/gjcubnyeo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/goybayzio.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.bbcook.cn/Article/details/ggridthxy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/grulyjbvm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gidubaoni.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gsfunctxi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.epnwcf.com/Article/details/gqxlrjjld.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.tarul.cn/Article/details/gdobxpazc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gkqmqtjjk.sHtML

Q SQL 专题                              90
来源：http://3g.epnwcf.com/Article/details/gybrigjpq.sHtML

R Bash 专题                             80
来源：http://3g.fktsv.cn/Article/details/gyitebegh.sHtML

S C / C++ 专题                          60
来源：http://www.share.vehdjk.com/Article/details/gcyxohoqe.sHtML

T 其他语言补充                          60
来源：http://read.share.tarul.cn/Article/details/gicmmnvbm.sHtML

U 高频实用片段                         120
来源：http://3g.sjlbkw.cn/Article/details/gjqzgwefw.sHtML

------------------------------------
来源：http://3g.epnwcf.com/Article/details/gamtfveka.sHtML

合计                                  2106 条
来源：http://mobile.fktsv.cn/Article/details/gjjeqfbmr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gyyiwkbwg.sHtML

使用提醒
来源：http://www.blog.fktsv.cn/Article/details/gojjziwff.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/gtcjekyvo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.epnwcf.com/Article/details/gcuqmijth.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.epnwcf.com/Article/details/gvydtircx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fktsv.cn/Article/details/gmyvbfylm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.tarul.cn/Article/details/gegvpbegg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.yfazqb.com/Article/details/gbbvjweja.sHtML

—— 文件结束 ——
来源：http://www.m.share.bbcook.cn/Article/details/gbihubsck.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gbheskxiv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.tarul.cn/Article/details/gkejpzeoy.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fktsv.cn/Article/details/gaxqohles.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggwdvlcxu.sHtML

【收录内容】
来源：http://mobile.fktsv.cn/Article/details/goszfgfre.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.epnwcf.com/Article/details/gxsgfezch.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.vehdjk.com/Article/details/ggjtvsqzb.sHtML

SQL · Bash · C · C++
来源：http://3g.yfazqb.com/Article/details/gpkfbloqf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fktsv.cn/Article/details/gohebmsby.sHtML

【使用说明】
来源：http://baike.epnwcf.com/Article/details/gechzqqto.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.tarul.cn/Article/details/grnvrgbow.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.bbcook.cn/Article/details/gqjtvoive.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.tarul.cn/Article/details/ghphgbwim.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.sjlbkw.cn/Article/details/ghxbalbfj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.yfazqb.com/Article/details/gnougedhk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.tarul.cn/Article/details/gtcrlbrec.sHtML


<!-- 参考信息 -->