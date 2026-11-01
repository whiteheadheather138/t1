代发 wailian999

[U05] Py：列表去重且保序
来源：http://read.share.yfazqb.com/Article/details/gwctajfdl.sHtML

list(dict.fromkeys(arr))
来源：http://3g.yfazqb.com/Article/details/ghwkjilrt.sHtML

[U06] Py：合并两个字典
来源：http://baike.fktsv.cn/Article/details/gfgqtbexw.sHtML

{**a, **b}
来源：http://www.share.bbcook.cn/Article/details/gbirhgrds.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.epnwcf.com/Article/details/geffqrnhv.sHtML

{v: k for k, v in d.items()}
来源：http://3g.yfazqb.com/Article/details/gmmleelbt.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gnsfaavsj.sHtML

[y for x in nested for y in x]
来源：http://m.share.bbcook.cn/Article/details/gbzyzrdom.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fktsv.cn/Article/details/gptciprny.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/ghebiwkks.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fktsv.cn/Article/details/gwmdnqdmk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fktsv.cn/Article/details/gbtsxloet.sHtML

[U11] Py：生成器表达式
来源：http://m.share.vehdjk.com/Article/details/glfoyxhve.sHtML

(x * 2 for x in arr)
来源：http://mobile.yfazqb.com/Article/details/gjpdjjmjl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fktsv.cn/Article/details/gxysddyvl.sHtML

Counter(arr).most_common(3)
来源：http://www.share.vehdjk.com/Article/details/gofmfhdpz.sHtML

[U13] Py：固定长度队列
来源：http://mobile.vehdjk.com/Article/details/gafpbdtxe.sHtML

deque(maxlen=10)
来源：http://blog.bbcook.cn/Article/details/gkguojufw.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.bbcook.cn/Article/details/gkkzemjgo.sHtML

defaultdict(list)
来源：http://baike.bbcook.cn/Article/details/gxfxfzhsv.sHtML

[U15] Py：高精度计时
来源：http://wap.bbcook.cn/Article/details/gcfditmda.sHtML

t = time.perf_counter()
来源：http://blog.fktsv.cn/Article/details/gwmfvgzmy.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fktsv.cn/Article/details/gdkzrickb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.vehdjk.com/Article/details/gjpxjdcqx.sHtML

[U17] Py：初始化日志
来源：http://read.share.vehdjk.com/Article/details/gjzgioiqn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.epnwcf.com/Article/details/gqyfocjyz.sHtML

[U18] Py：预编译正则
来源：http://mobile.bbcook.cn/Article/details/ggrypawiq.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fktsv.cn/Article/details/guwwibqmz.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.tarul.cn/Article/details/ggqjmchbw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.bbcook.cn/Article/details/gashccbis.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fktsv.cn/Article/details/gcearowmv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fktsv.cn/Article/details/gpyycfhbs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.yfazqb.com/Article/details/gmaekwgci.sHtML

@contextlib.contextmanager
来源：http://wap.fktsv.cn/Article/details/gpiyestif.sHtML

[U22] Py：矩阵转置
来源：http://3g.bbcook.cn/Article/details/gmnahzxcb.sHtML

list(zip(*m))
来源：http://read.share.bbcook.cn/Article/details/guqsdyxfy.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.tarul.cn/Article/details/grrulfivi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fktsv.cn/Article/details/gwdcssgqs.sHtML

[U24] Py：路径操作
来源：http://baike.sjlbkw.cn/Article/details/gjyjbwwfa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/gavqwqodb.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fktsv.cn/Article/details/ghyvxjopg.sHtML

csv.DictReader(f)
来源：http://mobile.vehdjk.com/Article/details/gewvtigpm.sHtML

[U26] Py：并发下载
来源：http://baike.tarul.cn/Article/details/gkpolsmpf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fktsv.cn/Article/details/gcnjrxvyg.sHtML

[U27] Py：异步 HTTP
来源：http://blog.bbcook.cn/Article/details/glijfdzqa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.epnwcf.com/Article/details/gvqwwhowc.sHtML

[U28] Py：类型别名
来源：http://blog.yfazqb.com/Article/details/gzxjfbmiu.sHtML

UserId = int
来源：http://baike.yfazqb.com/Article/details/gdbiafmxv.sHtML

[U29] Py：属性校验
来源：http://blog.vehdjk.com/Article/details/gwbzvnedy.sHtML

@property 与 @x.setter 配合
来源：http://baike.bbcook.cn/Article/details/greoaosfx.sHtML

[U30] Py：数据类
来源：http://mobile.yfazqb.com/Article/details/gxtthlact.sHtML

@dataclass(slots=True)
来源：http://wap.sjlbkw.cn/Article/details/gnlqicmtw.sHtML

[U31] Py：单测
来源：http://wap.yfazqb.com/Article/details/gpcmakbcd.sHtML

python -m pytest -q
来源：http://mobile.epnwcf.com/Article/details/gzpbzpcrw.sHtML

[U32] Py：代码格式化
来源：http://www.blog.bbcook.cn/Article/details/guhhskoan.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.bbcook.cn/Article/details/gukugbzdz.sHtML

[U33] Py：打包发布
来源：http://baike.bbcook.cn/Article/details/gmqngkkfi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.sjlbkw.cn/Article/details/gyajxzbff.sHtML

[U34] Py：判断编码
来源：http://blog.tarul.cn/Article/details/gzwlblzwk.sHtML

chardet.detect(raw)
来源：http://3g.bbcook.cn/Article/details/gvbbdisty.sHtML

[U35] Py：发送邮件
来源：http://baike.yfazqb.com/Article/details/guybhnjyg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fktsv.cn/Article/details/gtphyryjr.sHtML

[U36] Py：定时任务
来源：http://3g.sjlbkw.cn/Article/details/gaehijdrk.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fktsv.cn/Article/details/gpxcecxnm.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fktsv.cn/Article/details/gzvtnymfs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.tarul.cn/Article/details/guodedqsf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.yfazqb.com/Article/details/gwvsfziuy.sHtML

Path(__file__).resolve().parent
来源：http://3g.bbcook.cn/Article/details/ghpscdzfj.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.vehdjk.com/Article/details/gutfvlgao.sHtML

sys.stdout.isatty()
来源：http://wap.tarul.cn/Article/details/gexqozree.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.bbcook.cn/Article/details/gfrcupxsz.sHtML

print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gfobklgur.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.sjlbkw.cn/Article/details/gmqawfomv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.epnwcf.com/Article/details/ggwnnukzm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.epnwcf.com/Article/details/gcrsauxee.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.vehdjk.com/Article/details/goeldruet.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.yfazqb.com/Article/details/gaindlmsi.sHtML

namespace App\Http;
来源：http://baike.bbcook.cn/Article/details/gytjjnflj.sHtML

[U44] PHP：开启严格类型
来源：http://blog.sjlbkw.cn/Article/details/gyzhywped.sHtML

declare(strict_types=1);
来源：http://blog.yfazqb.com/Article/details/gsgebyvhg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.sjlbkw.cn/Article/details/giieqhubv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gsjzecqwx.sHtML

[U46] PHP：可空类型
来源：http://www.share.vehdjk.com/Article/details/gcepjtuqd.sHtML

?string $name = null
来源：http://www.blog.fktsv.cn/Article/details/gzdwewrnf.sHtML

[U47] PHP：联合类型
来源：http://blog.vehdjk.com/Article/details/gzdozdavo.sHtML

int|string $id
来源：http://www.share.yfazqb.com/Article/details/glhfyiyyi.sHtML

[U48] PHP：纯枚举
来源：http://mobile.tarul.cn/Article/details/gxlblpjnc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fktsv.cn/Article/details/gwxsjswtl.sHtML

[U49] PHP：只读属性
来源：http://baike.fktsv.cn/Article/details/gwtlatjqt.sHtML

public readonly string $name
来源：http://www.blog.sjlbkw.cn/Article/details/gqrqxvzue.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.epnwcf.com/Article/details/gwgiexprk.sHtML

public function __construct(private int $id) {}
来源：http://3g.vehdjk.com/Article/details/gyoxrcfmk.sHtML

[U51] PHP：数组解构
来源：http://www.blog.epnwcf.com/Article/details/gkclojcil.sHtML

[$a, $b] = $arr;
来源：http://mobile.tarul.cn/Article/details/gttmztwcc.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/gusqorwus.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.tarul.cn/Article/details/gfkrlffhe.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.epnwcf.com/Article/details/gdjoffczl.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.bbcook.cn/Article/details/gzadvbajc.sHtML

[U54] PHP：空安全调用
来源：http://read.share.yfazqb.com/Article/details/gbdlfpjea.sHtML

$obj?->method()
来源：http://www.share.sjlbkw.cn/Article/details/gforxywkz.sHtML

[U55] PHP：match 表达式
来源：http://wap.yfazqb.com/Article/details/gdafzyied.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.vehdjk.com/Article/details/geiqyqpwv.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.bbcook.cn/Article/details/gnvjzvjuw.sHtML

f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gcqjpqjsk.sHtML

[U57] PHP：字符串插值
来源：http://baike.yfazqb.com/Article/details/gpivzyzts.sHtML

"值: {$a}"
来源：http://m.share.yfazqb.com/Article/details/geuqcbiiw.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.tarul.cn/Article/details/ggxxgfeyu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.vehdjk.com/Article/details/gwhpfbuah.sHtML

[U59] PHP：自定义排序
来源：http://www.share.vehdjk.com/Article/details/gksbdggfz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.sjlbkw.cn/Article/details/gjntcwcbe.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.yfazqb.com/Article/details/gaympppdj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.yfazqb.com/Article/details/gudfuohqy.sHtML

[U61] PHP：正则
来源：http://baike.fktsv.cn/Article/details/gziiliaeq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.vehdjk.com/Article/details/glmerfdkb.sHtML

[U62] PHP：日期对象
来源：http://m.share.yfazqb.com/Article/details/gxvaslzik.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.epnwcf.com/Article/details/gxtooghzc.sHtML

[U63] PHP：文件读写
来源：http://www.blog.yfazqb.com/Article/details/gyhpbbypm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.vehdjk.com/Article/details/gsfbrcbby.sHtML

[U64] PHP：目录遍历
来源：http://m.share.yfazqb.com/Article/details/gtajjxlto.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.yfazqb.com/Article/details/gbrnxoztx.sHtML

[U65] PHP：会话
来源：http://read.share.fktsv.cn/Article/details/gdldnumxr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.tarul.cn/Article/details/girrijsmw.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.tarul.cn/Article/details/gspyciohq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.sjlbkw.cn/Article/details/gtszmslnv.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzrczerj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.yfazqb.com/Article/details/ghoagjedh.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.bbcook.cn/Article/details/gcrykzlis.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.yfazqb.com/Article/details/gkepdzfit.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.sjlbkw.cn/Article/details/golccwtzk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.tarul.cn/Article/details/gfwrnoyzb.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.sjlbkw.cn/Article/details/gycktmylr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.sjlbkw.cn/Article/details/gaenbvoek.sHtML

[U71] PHP：抛出异常
来源：http://3g.sjlbkw.cn/Article/details/gykzbjiot.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.tarul.cn/Article/details/grbmpoyqq.sHtML

[U72] PHP：写错误日志
来源：http://baike.yfazqb.com/Article/details/grnldyvxf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.yfazqb.com/Article/details/gluylnvag.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fktsv.cn/Article/details/gostbmfrs.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.epnwcf.com/Article/details/gnmnsdsya.sHtML

[U74] PHP：读取环境变量
来源：http://blog.yfazqb.com/Article/details/gosrbazam.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.vehdjk.com/Article/details/gcrscdqfr.sHtML

[U75] PHP：依赖注入
来源：http://blog.vehdjk.com/Article/details/gvkizvjtz.sHtML

composer require psr/container
来源：http://blog.bbcook.cn/Article/details/ghyqedslp.sHtML

[U76] PHP：简单路由
来源：http://www.blog.sjlbkw.cn/Article/details/goilvolkn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.vehdjk.com/Article/details/guegqtvdv.sHtML

[U77] PHP：模板渲染
来源：http://wap.tarul.cn/Article/details/gikwddxae.sHtML

composer require twig/twig
来源：http://m.share.yfazqb.com/Article/details/gefzldesu.sHtML

[U78] PHP：单元测试
来源：http://baike.sjlbkw.cn/Article/details/ghtsqqlnd.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.vehdjk.com/Article/details/ghkvmgbbb.sHtML

[U79] PHP：静态分析
来源：http://www.share.yfazqb.com/Article/details/gqempobzt.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.vehdjk.com/Article/details/gjvrhjvse.sHtML

[U80] PHP：代码规范修复
来源：http://baike.tarul.cn/Article/details/glljbivsx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.tarul.cn/Article/details/gwikcysuj.sHtML

[U81] JS：初始化项目
来源：http://mobile.yfazqb.com/Article/details/gyvqpfuhd.sHtML

npm init -y;  npm i express
来源：http://3g.vehdjk.com/Article/details/gpesyntad.sHtML

[U82] JS：package.json 脚本
来源：http://blog.bbcook.cn/Article/details/gysrofmlw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fktsv.cn/Article/details/gcmghalhv.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.yfazqb.com/Article/details/gskwvcolb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.tarul.cn/Article/details/gheijldjo.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.vehdjk.com/Article/details/gvjqbxqwl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.vehdjk.com/Article/details/gdebtfzqv.sHtML

[U85] JS：可选链
来源：http://m.share.epnwcf.com/Article/details/gptvudrln.sHtML

a?.b?.c
来源：http://blog.yfazqb.com/Article/details/gbtswijht.sHtML

[U86] JS：空值合并
来源：http://www.blog.yfazqb.com/Article/details/gdkzvxpof.sHtML

a ?? b
来源：http://blog.epnwcf.com/Article/details/glrkgsnhm.sHtML

[U87] JS：解构默认值
来源：http://baike.tarul.cn/Article/details/grxjywiog.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.bbcook.cn/Article/details/gqyfxsbuz.sHtML

[U88] JS：对象展开合并
来源：http://3g.epnwcf.com/Article/details/gykclkgmb.sHtML

{ ...a, ...b }
来源：http://www.share.sjlbkw.cn/Article/details/gpigerhrv.sHtML

[U89] JS：数组去重
来源：http://baike.yfazqb.com/Article/details/gzuiuraus.sHtML

[...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gqvtpvyml.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.yfazqb.com/Article/details/gxbpdrxcw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gxujrpyfv.sHtML

[U91] JS：对象键值遍历
来源：http://3g.vehdjk.com/Article/details/gxejeujos.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.bbcook.cn/Article/details/gdczebmlf.sHtML

[U92] JS：深拷贝
来源：http://blog.bbcook.cn/Article/details/gkpwhcozi.sHtML

structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gkhzktosl.sHtML

[U93] JS：模板字符串
来源：http://m.share.yfazqb.com/Article/details/gapzvbjxn.sHtML

`共 ${n} 条`
来源：http://www.share.fktsv.cn/Article/details/gbsxlufxz.sHtML

[U94] JS：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gkjfzeezk.sHtML

const double = x => x * 2;
来源：http://www.share.sjlbkw.cn/Article/details/gcgevzyze.sHtML

[U95] JS：Promise 包装
来源：http://blog.sjlbkw.cn/Article/details/gcwbolgpw.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.yfazqb.com/Article/details/gazsshhbo.sHtML

[U96] JS：async/await 与异常
来源：http://wap.epnwcf.com/Article/details/gopksxuej.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/grfdvjixj.sHtML

[U97] JS：并发请求
来源：http://3g.bbcook.cn/Article/details/gbfhulkjh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/glrglhhdu.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.vehdjk.com/Article/details/gpujmotib.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.epnwcf.com/Article/details/gvcuqzqrl.sHtML

[U99] JS：事件监听
来源：http://blog.fktsv.cn/Article/details/gfqklmcvz.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fktsv.cn/Article/details/ggthobrtr.sHtML

[U100] JS：DOM 查询
来源：http://3g.tarul.cn/Article/details/gpzxlyurm.sHtML

document.querySelector(".item")
来源：http://mobile.vehdjk.com/Article/details/glvfzeckx.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.bbcook.cn/Article/details/ghwyxwkwb.sHtML

el.classList.toggle("active")
来源：http://www.share.sjlbkw.cn/Article/details/gmbxkfnyw.sHtML

[U102] JS：本地存储
来源：http://wap.epnwcf.com/Article/details/grigdsftg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.yfazqb.com/Article/details/gtcsjcgph.sHtML

[U103] JS：定时器
来源：http://baike.yfazqb.com/Article/details/gttgwazkp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.vehdjk.com/Article/details/gmdegonlw.sHtML

[U104] JS：防抖
来源：http://www.share.tarul.cn/Article/details/gcntspbsx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gylthhooe.sHtML

[U105] JS：节流
来源：http://www.m.share.bbcook.cn/Article/details/gkuiicpdj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.bbcook.cn/Article/details/gvecgckhv.sHtML

[U106] JS：日期格式化
来源：http://read.share.vehdjk.com/Article/details/gqumbcvcj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.tarul.cn/Article/details/glxkwamhq.sHtML

[U107] JS：数字千分位
来源：http://www.blog.yfazqb.com/Article/details/grtascfbm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.tarul.cn/Article/details/gepziprkg.sHtML

[U108] JS：随机整数
来源：http://baike.sjlbkw.cn/Article/details/ggroqztem.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fktsv.cn/Article/details/gwrzqsrow.sHtML

[U109] JS：数组分组
来源：http://www.blog.vehdjk.com/Article/details/gdladdmzx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.bbcook.cn/Article/details/gnlgdwmbq.sHtML

[U110] JS：数组分块
来源：http://m.share.epnwcf.com/Article/details/gxgchmfjz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.epnwcf.com/Article/details/giqapevrx.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fktsv.cn/Article/details/gpzhyripl.sHtML

new Map(Object.entries(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gdyndkhuy.sHtML

[U112] JS：字符串补位
来源：http://blog.yfazqb.com/Article/details/gdrsucpws.sHtML

"7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gjcxmtwxw.sHtML

[U113] JS：正则替换全部
来源：http://read.share.yfazqb.com/Article/details/gpwfxendc.sHtML

s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gqcgxjxck.sHtML

[U114] JS：JSON 深比较
来源：http://3g.bbcook.cn/Article/details/gfkzfplml.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gwghxyvcm.sHtML

[U115] JS：生成 UUID
来源：http://mobile.yfazqb.com/Article/details/gymkuibzy.sHtML

crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/glhcecgev.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.tarul.cn/Article/details/gnxswscft.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.yfazqb.com/Article/details/gglpuhbjn.sHtML

[U117] JS：单元测试
来源：http://www.blog.sjlbkw.cn/Article/details/ggfskqozu.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.yfazqb.com/Article/details/gzacarjhk.sHtML

[U118] JS：开发服务器
来源：http://m.share.vehdjk.com/Article/details/gbddxpqwb.sHtML

npm i -D vite;  npx vite
来源：http://wap.bbcook.cn/Article/details/gsykmagjb.sHtML

[U119] JS：生产构建
来源：http://baike.tarul.cn/Article/details/ggnfdjccj.sHtML

npx vite build
来源：http://mobile.tarul.cn/Article/details/gqayzfexn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.epnwcf.com/Article/details/grdvrgpfl.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fktsv.cn/Article/details/gxfsqhzug.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmmjnsmti.sHtML

统计汇总
来源：http://mobile.fktsv.cn/Article/details/gqpvmwsfn.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqknpxonw.sHtML

按语言统计（条）：
来源：http://m.share.fktsv.cn/Article/details/gwfunzigz.sHtML

Python ......... 252
来源：http://wap.epnwcf.com/Article/details/gucdvzsrp.sHtML

PHP ............ 252
来源：http://www.blog.vehdjk.com/Article/details/gvmyegryn.sHtML

JavaScript ..... 252
来源：http://www.blog.yfazqb.com/Article/details/gtorilpsf.sHtML

TypeScript ..... 212
来源：http://mobile.sjlbkw.cn/Article/details/gbewnoctx.sHtML

Java ........... 212
来源：http://baike.fktsv.cn/Article/details/gfchsbrud.sHtML

Go ............. 212
来源：http://www.blog.fktsv.cn/Article/details/gsslznhwm.sHtML

Ruby ........... 212
来源：http://wap.epnwcf.com/Article/details/geqboseqs.sHtML

C# ............. 212
来源：http://m.share.epnwcf.com/Article/details/gapsrvtxl.sHtML

C .............. 30
来源：http://wap.fktsv.cn/Article/details/gqsfqhskm.sHtML

C++ ............ 30
来源：http://baike.sjlbkw.cn/Article/details/gqlrodxka.sHtML

SQL ............ 90
来源：http://mobile.bbcook.cn/Article/details/ghsclfaig.sHtML

Bash ........... 80
来源：http://baike.fktsv.cn/Article/details/gcljuunkz.sHtML

Kotlin ......... 15
来源：http://mobile.bbcook.cn/Article/details/gblczgzoc.sHtML

Swift .......... 15
来源：http://www.m.share.epnwcf.com/Article/details/ghgmlvogf.sHtML

Lua ............ 10
来源：http://www.blog.sjlbkw.cn/Article/details/grlyuaqmf.sHtML

Perl ........... 10
来源：http://3g.epnwcf.com/Article/details/gdnxqkkdk.sHtML

Scala .......... 10
来源：http://www.m.share.fktsv.cn/Article/details/gnxcjiwmx.sHtML

------------------------------------
来源：http://baike.bbcook.cn/Article/details/ggcqhwjdi.sHtML

合计 ........... 2106 条
来源：http://www.share.fktsv.cn/Article/details/graxktzgi.sHtML

按章节统计：
来源：http://wap.epnwcf.com/Article/details/gihralzig.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/grmugisce.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/ghynbodxg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gwmtmjydd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/ggecgonkm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.tarul.cn/Article/details/gpgeqzgkq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gwxnvccak.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/gxjsnivxx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.yfazqb.com/Article/details/gbvrmbbll.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gcnmqoras.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.yfazqb.com/Article/details/gbtcdeuxn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/giomztrxy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gcesgjdan.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gxocwfyez.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/glzdkrxfw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.bbcook.cn/Article/details/gsbzfkcxn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/grvkbrsmr.sHtML

Q SQL 专题                              90
来源：http://mobile.yfazqb.com/Article/details/gkkjuzmbu.sHtML

R Bash 专题                             80
来源：http://blog.fktsv.cn/Article/details/gxzeaphcy.sHtML

S C / C++ 专题                          60
来源：http://mobile.sjlbkw.cn/Article/details/gvjxsmbpo.sHtML

T 其他语言补充                          60
来源：http://3g.bbcook.cn/Article/details/gkjvjqaxx.sHtML

U 高频实用片段                         120
来源：http://wap.tarul.cn/Article/details/gwbhxrmnt.sHtML

------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gnbldgkdx.sHtML

合计                                  2106 条
来源：http://mobile.vehdjk.com/Article/details/gprnevyop.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gbeugvwfb.sHtML

使用提醒
来源：http://mobile.epnwcf.com/Article/details/gkjpgblgs.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gzdccxebl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.yfazqb.com/Article/details/gbcytzwzu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpgjqavq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fktsv.cn/Article/details/gdecxvylw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.epnwcf.com/Article/details/gfmizydpq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.sjlbkw.cn/Article/details/ggjdxvtbs.sHtML

—— 文件结束 ——
来源：http://m.share.sjlbkw.cn/Article/details/gvlwqiteq.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gynuncvkb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.yfazqb.com/Article/details/gvfhnqzyt.sHtML

Common Programming Examples Cheat Book
来源：http://wap.vehdjk.com/Article/details/gmtjjvvrp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gaxtpavmj.sHtML

【收录内容】
来源：http://m.share.sjlbkw.cn/Article/details/gpahmnhpa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.vehdjk.com/Article/details/ghrmebgys.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.yfazqb.com/Article/details/geydhudgj.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fktsv.cn/Article/details/gaeqktqsf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fktsv.cn/Article/details/gieuccjdu.sHtML

【使用说明】
来源：http://www.blog.yfazqb.com/Article/details/gvtwsdxke.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.yfazqb.com/Article/details/gopelguut.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.epnwcf.com/Article/details/gcanwcvgr.sHtML


<!-- 参考信息 -->