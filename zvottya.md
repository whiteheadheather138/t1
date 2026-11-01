代发 wailian999

[U05] Py：列表去重且保序
来源：http://read.share.tarul.cn/Article/details/gsjogkjeh.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gmekwaacz.sHtML

[U06] Py：合并两个字典
来源：http://baike.sjlbkw.cn/Article/details/gclaaxpyq.sHtML

{**a, **b}
来源：http://www.blog.sjlbkw.cn/Article/details/gcskduclk.sHtML

[U07] Py：反转字典键值
来源：http://read.share.yfazqb.com/Article/details/gdlxkoiqa.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.vehdjk.com/Article/details/giulumruu.sHtML

[U08] Py：展平二维列表
来源：http://mobile.epnwcf.com/Article/details/ghpgvkuvz.sHtML

[y for x in nested for y in x]
来源：http://www.share.yfazqb.com/Article/details/gytlmqnzp.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.tarul.cn/Article/details/gqpebjtst.sHtML

max(d, key=d.get)
来源：http://mobile.yfazqb.com/Article/details/gevoshdjt.sHtML

[U10] Py：按值排序字典
来源：http://3g.tarul.cn/Article/details/gabsrmzmw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.vehdjk.com/Article/details/gnsvhzjyk.sHtML

[U11] Py：生成器表达式
来源：http://3g.yfazqb.com/Article/details/gfrpequfa.sHtML

(x * 2 for x in arr)
来源：http://read.share.yfazqb.com/Article/details/gplgxkfrs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fktsv.cn/Article/details/gyoeazpog.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fktsv.cn/Article/details/gpsecynpb.sHtML

[U13] Py：固定长度队列
来源：http://mobile.bbcook.cn/Article/details/gkahuefvr.sHtML

deque(maxlen=10)
来源：http://wap.epnwcf.com/Article/details/ggeprrujb.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.yfazqb.com/Article/details/gckuhaxyw.sHtML

defaultdict(list)
来源：http://www.blog.tarul.cn/Article/details/gnjmzpiih.sHtML

[U15] Py：高精度计时
来源：http://read.share.vehdjk.com/Article/details/gnfehuluk.sHtML

t = time.perf_counter()
来源：http://wap.tarul.cn/Article/details/gkujphivq.sHtML

[U16] Py：命令行参数解析
来源：http://3g.sjlbkw.cn/Article/details/gcpujshtc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.yfazqb.com/Article/details/gmuwtuypz.sHtML

[U17] Py：初始化日志
来源：http://m.share.epnwcf.com/Article/details/gmyltkcsi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.bbcook.cn/Article/details/gmiuettzt.sHtML

[U18] Py：预编译正则
来源：http://www.blog.bbcook.cn/Article/details/gtpfbqpva.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.vehdjk.com/Article/details/ggdplxbzh.sHtML

[U19] Py：正则替换带回调
来源：http://wap.sjlbkw.cn/Article/details/guieivcsx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.vehdjk.com/Article/details/gdbpntcgr.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fktsv.cn/Article/details/ghblmyyhy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.vehdjk.com/Article/details/ggmqmpjaw.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.sjlbkw.cn/Article/details/gewaarjku.sHtML

@contextlib.contextmanager
来源：http://3g.tarul.cn/Article/details/gyxlhlxmm.sHtML

[U22] Py：矩阵转置
来源：http://wap.vehdjk.com/Article/details/gnjstxyxt.sHtML

list(zip(*m))
来源：http://wap.yfazqb.com/Article/details/gujrrqfnm.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.epnwcf.com/Article/details/gltxmxeqr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.bbcook.cn/Article/details/gvvhnlvtb.sHtML

[U24] Py：路径操作
来源：http://baike.epnwcf.com/Article/details/grpgrsegc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/gfuemkbyy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.yfazqb.com/Article/details/gmivznvwc.sHtML

csv.DictReader(f)
来源：http://3g.epnwcf.com/Article/details/gilnetjvi.sHtML

[U26] Py：并发下载
来源：http://www.blog.fktsv.cn/Article/details/gguephlsv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.tarul.cn/Article/details/gozzidhed.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.yfazqb.com/Article/details/gluwxkeoz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.sjlbkw.cn/Article/details/gibrlwleg.sHtML

[U28] Py：类型别名
来源：http://3g.tarul.cn/Article/details/gjtxuoybq.sHtML

UserId = int
来源：http://www.share.yfazqb.com/Article/details/gkpogokts.sHtML

[U29] Py：属性校验
来源：http://www.m.share.yfazqb.com/Article/details/gnuyomoee.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fktsv.cn/Article/details/gzoqotcal.sHtML

[U30] Py：数据类
来源：http://www.share.fktsv.cn/Article/details/gbcpynayu.sHtML

@dataclass(slots=True)
来源：http://www.m.share.vehdjk.com/Article/details/gzrrjwrjs.sHtML

[U31] Py：单测
来源：http://mobile.fktsv.cn/Article/details/gwjrpixsb.sHtML

python -m pytest -q
来源：http://m.share.sjlbkw.cn/Article/details/gzwjnumpr.sHtML

[U32] Py：代码格式化
来源：http://m.share.epnwcf.com/Article/details/gtahqtrta.sHtML

ruff format . && ruff check --fix .
来源：http://wap.sjlbkw.cn/Article/details/gblpapuer.sHtML

[U33] Py：打包发布
来源：http://blog.sjlbkw.cn/Article/details/gyslyquxi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.vehdjk.com/Article/details/gpmtitygu.sHtML

[U34] Py：判断编码
来源：http://mobile.yfazqb.com/Article/details/gdtpsnyld.sHtML

chardet.detect(raw)
来源：http://www.share.vehdjk.com/Article/details/gutajiklz.sHtML

[U35] Py：发送邮件
来源：http://3g.bbcook.cn/Article/details/gldhtssdd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.yfazqb.com/Article/details/gjlqyukgs.sHtML

[U36] Py：定时任务
来源：http://mobile.epnwcf.com/Article/details/gpcubjfmn.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.yfazqb.com/Article/details/gmsifnplx.sHtML

[U37] Py：读写 Excel
来源：http://mobile.tarul.cn/Article/details/gurtydzgp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.bbcook.cn/Article/details/geruxgqfu.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.sjlbkw.cn/Article/details/gihvhkmxn.sHtML

Path(__file__).resolve().parent
来源：http://baike.vehdjk.com/Article/details/gxarvoenf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.epnwcf.com/Article/details/gwxyfzokw.sHtML

sys.stdout.isatty()
来源：http://wap.sjlbkw.cn/Article/details/gfofzknxg.sHtML

[U40] Py：打印到标准错误
来源：http://3g.vehdjk.com/Article/details/gdbheovgj.sHtML

print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gibkglmva.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fktsv.cn/Article/details/gcnpslufr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fktsv.cn/Article/details/gvgronyzm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.yfazqb.com/Article/details/gapewsuml.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.tarul.cn/Article/details/gwmqovoer.sHtML

[U43] PHP：声明命名空间
来源：http://wap.bbcook.cn/Article/details/gurvdqwtd.sHtML

namespace App\Http;
来源：http://3g.bbcook.cn/Article/details/goftwxusk.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.epnwcf.com/Article/details/ginnqidbf.sHtML

declare(strict_types=1);
来源：http://read.share.epnwcf.com/Article/details/giyxayglt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.vehdjk.com/Article/details/gocldaeww.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gfylpnryu.sHtML

[U46] PHP：可空类型
来源：http://www.share.bbcook.cn/Article/details/gekdokyhc.sHtML

?string $name = null
来源：http://www.share.yfazqb.com/Article/details/gqxuzmpgn.sHtML

[U47] PHP：联合类型
来源：http://wap.fktsv.cn/Article/details/gahfucooj.sHtML

int|string $id
来源：http://mobile.bbcook.cn/Article/details/gbygfhuyy.sHtML

[U48] PHP：纯枚举
来源：http://mobile.vehdjk.com/Article/details/gqgalvbpf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.sjlbkw.cn/Article/details/gaqrywacg.sHtML

[U49] PHP：只读属性
来源：http://wap.tarul.cn/Article/details/gfwincqea.sHtML

public readonly string $name
来源：http://m.share.epnwcf.com/Article/details/gkfavijxd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.vehdjk.com/Article/details/ggwysfppu.sHtML

public function __construct(private int $id) {}
来源：http://mobile.epnwcf.com/Article/details/gljhmkuvn.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.tarul.cn/Article/details/gqnbodgib.sHtML

[$a, $b] = $arr;
来源：http://blog.epnwcf.com/Article/details/ghnosvkbx.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.sjlbkw.cn/Article/details/giydbjwic.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.vehdjk.com/Article/details/gykpaadfh.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.bbcook.cn/Article/details/grvwcjydg.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fktsv.cn/Article/details/gbwtvlbsp.sHtML

[U54] PHP：空安全调用
来源：http://wap.bbcook.cn/Article/details/geuvpcyne.sHtML

$obj?->method()
来源：http://m.share.yfazqb.com/Article/details/gqmtbcczn.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.bbcook.cn/Article/details/gzmkoevks.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.epnwcf.com/Article/details/goyznpgza.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gbufkrnep.sHtML

f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gnpfpzvcg.sHtML

[U57] PHP：字符串插值
来源：http://3g.bbcook.cn/Article/details/gnuvwvxjv.sHtML

"值: {$a}"
来源：http://www.share.sjlbkw.cn/Article/details/gpgtiigjw.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.bbcook.cn/Article/details/gztjewjtq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.bbcook.cn/Article/details/gdmktqerb.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fktsv.cn/Article/details/gxzjrbpxo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/gdgjkfhsm.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.yfazqb.com/Article/details/gbfuxuskv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fktsv.cn/Article/details/gyvzjcxty.sHtML

[U61] PHP：正则
来源：http://wap.sjlbkw.cn/Article/details/geiowjwsl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.tarul.cn/Article/details/gnbbbslox.sHtML

[U62] PHP：日期对象
来源：http://www.share.bbcook.cn/Article/details/gnejzemut.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.sjlbkw.cn/Article/details/geskkiyuk.sHtML

[U63] PHP：文件读写
来源：http://blog.yfazqb.com/Article/details/gathmfzvc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.epnwcf.com/Article/details/gftfsgehd.sHtML

[U64] PHP：目录遍历
来源：http://m.share.yfazqb.com/Article/details/gcugsodfn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.epnwcf.com/Article/details/gggqvetvz.sHtML

[U65] PHP：会话
来源：http://www.share.yfazqb.com/Article/details/giamwccry.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gtpshvysf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.epnwcf.com/Article/details/gxuidyuoq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.bbcook.cn/Article/details/gwfjlqydf.sHtML

[U67] PHP：处理文件上传
来源：http://blog.vehdjk.com/Article/details/ghnhyayti.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.bbcook.cn/Article/details/gbtcthika.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.sjlbkw.cn/Article/details/gognbjurj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fktsv.cn/Article/details/gdvfpcaot.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.tarul.cn/Article/details/gxmrvxbaw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.yfazqb.com/Article/details/gyqnptzxj.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.yfazqb.com/Article/details/gbapleqst.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.bbcook.cn/Article/details/gnkosuyjo.sHtML

[U71] PHP：抛出异常
来源：http://wap.sjlbkw.cn/Article/details/gcgpwlmno.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.tarul.cn/Article/details/ghzvexpvg.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fktsv.cn/Article/details/gkilxrgyk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.sjlbkw.cn/Article/details/glvnpdhec.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.tarul.cn/Article/details/gpqglqmam.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.tarul.cn/Article/details/gsmjvghoh.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.vehdjk.com/Article/details/gaczbkoin.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.bbcook.cn/Article/details/grvrpditf.sHtML

[U75] PHP：依赖注入
来源：http://m.share.bbcook.cn/Article/details/gxrghhbzd.sHtML

composer require psr/container
来源：http://wap.sjlbkw.cn/Article/details/gyccdwknh.sHtML

[U76] PHP：简单路由
来源：http://blog.tarul.cn/Article/details/gkrygtvhi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.yfazqb.com/Article/details/gtzzxhedy.sHtML

[U77] PHP：模板渲染
来源：http://blog.bbcook.cn/Article/details/goijqgtge.sHtML

composer require twig/twig
来源：http://mobile.fktsv.cn/Article/details/gqxjitkxh.sHtML

[U78] PHP：单元测试
来源：http://baike.fktsv.cn/Article/details/gcdcancai.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.epnwcf.com/Article/details/geszcpaex.sHtML

[U79] PHP：静态分析
来源：http://blog.epnwcf.com/Article/details/gyylrxujb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.bbcook.cn/Article/details/gwezafdit.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.epnwcf.com/Article/details/gduisjwky.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fktsv.cn/Article/details/gnqsftuxw.sHtML

[U81] JS：初始化项目
来源：http://www.blog.epnwcf.com/Article/details/ggxexevnl.sHtML

npm init -y;  npm i express
来源：http://www.blog.tarul.cn/Article/details/ghmiqpasj.sHtML

[U82] JS：package.json 脚本
来源：http://wap.bbcook.cn/Article/details/gqlrutsfy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.bbcook.cn/Article/details/gvborojew.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fktsv.cn/Article/details/gwpouoesc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/guetfgqjv.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.yfazqb.com/Article/details/gyydypnwr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.sjlbkw.cn/Article/details/grtiquhbb.sHtML

[U85] JS：可选链
来源：http://wap.bbcook.cn/Article/details/gcoaqdhah.sHtML

a?.b?.c
来源：http://www.blog.bbcook.cn/Article/details/gvksoktck.sHtML

[U86] JS：空值合并
来源：http://read.share.vehdjk.com/Article/details/gpvpuxtyt.sHtML

a ?? b
来源：http://www.m.share.bbcook.cn/Article/details/gcmkzprka.sHtML

[U87] JS：解构默认值
来源：http://m.share.yfazqb.com/Article/details/gpphhslfu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.epnwcf.com/Article/details/gpruokeoj.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.bbcook.cn/Article/details/gobsmcbcc.sHtML

{ ...a, ...b }
来源：http://wap.yfazqb.com/Article/details/gpnhzwxfa.sHtML

[U89] JS：数组去重
来源：http://mobile.vehdjk.com/Article/details/gpkvewhiq.sHtML

[...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gzoowbvyc.sHtML

[U90] JS：数字数组排序
来源：http://m.share.vehdjk.com/Article/details/gaujdwjth.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gvlhyqhhr.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.yfazqb.com/Article/details/gioyimqjc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.tarul.cn/Article/details/gdlpvgjjg.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gewqdeoys.sHtML

structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gumhngrhm.sHtML

[U93] JS：模板字符串
来源：http://blog.tarul.cn/Article/details/gqqopikli.sHtML

`共 ${n} 条`
来源：http://3g.tarul.cn/Article/details/gswwwdrik.sHtML

[U94] JS：箭头函数
来源：http://wap.bbcook.cn/Article/details/gmmgymtkc.sHtML

const double = x => x * 2;
来源：http://mobile.fktsv.cn/Article/details/gdxocwdev.sHtML

[U95] JS：Promise 包装
来源：http://www.share.tarul.cn/Article/details/gilbbcrsb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.tarul.cn/Article/details/gyszyqwib.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.yfazqb.com/Article/details/gaiimawwo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/grlrnhwpf.sHtML

[U97] JS：并发请求
来源：http://www.m.share.vehdjk.com/Article/details/gmkmbwkhv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/ggoaukmli.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.yfazqb.com/Article/details/gveeqbtjh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.yfazqb.com/Article/details/gbjgnyvce.sHtML

[U99] JS：事件监听
来源：http://3g.vehdjk.com/Article/details/gjwnchoza.sHtML

el.addEventListener("click", e => {})
来源：http://wap.epnwcf.com/Article/details/ghihvytar.sHtML

[U100] JS：DOM 查询
来源：http://3g.bbcook.cn/Article/details/gevbracxf.sHtML

document.querySelector(".item")
来源：http://m.share.fktsv.cn/Article/details/gldfsaukd.sHtML

[U101] JS：classList 操作
来源：http://www.share.yfazqb.com/Article/details/gbjkxqqqs.sHtML

el.classList.toggle("active")
来源：http://3g.bbcook.cn/Article/details/gexxktvnb.sHtML

[U102] JS：本地存储
来源：http://baike.fktsv.cn/Article/details/gvkpwzysl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.epnwcf.com/Article/details/grnxwhqox.sHtML

[U103] JS：定时器
来源：http://read.share.fktsv.cn/Article/details/gdqutmskk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.sjlbkw.cn/Article/details/gmfqsobst.sHtML

[U104] JS：防抖
来源：http://m.share.tarul.cn/Article/details/gzcgvkvqy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/glcjycapa.sHtML

[U105] JS：节流
来源：http://baike.vehdjk.com/Article/details/geohojems.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.sjlbkw.cn/Article/details/gjgggsexr.sHtML

[U106] JS：日期格式化
来源：http://m.share.epnwcf.com/Article/details/gibfrrzgq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fktsv.cn/Article/details/gfmkfgegp.sHtML

[U107] JS：数字千分位
来源：http://3g.fktsv.cn/Article/details/gspvrwpsw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.epnwcf.com/Article/details/gkxinlehu.sHtML

[U108] JS：随机整数
来源：http://read.share.vehdjk.com/Article/details/gpdltoqqq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fktsv.cn/Article/details/gnvzendbk.sHtML

[U109] JS：数组分组
来源：http://www.m.share.tarul.cn/Article/details/gpkgynygz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/giruqgilr.sHtML

[U110] JS：数组分块
来源：http://read.share.sjlbkw.cn/Article/details/godguvyrn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.bbcook.cn/Article/details/glgwgxtau.sHtML

[U111] JS：对象转 Map
来源：http://www.share.yfazqb.com/Article/details/guphcvgiq.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gmruxzdel.sHtML

[U112] JS：字符串补位
来源：http://wap.epnwcf.com/Article/details/gtnkpccid.sHtML

"7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gpnaflcab.sHtML

[U113] JS：正则替换全部
来源：http://blog.sjlbkw.cn/Article/details/gxtvosiss.sHtML

s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gydyutils.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.bbcook.cn/Article/details/gsmmdvxpc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gazhashpv.sHtML

[U115] JS：生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/guukgnxom.sHtML

crypto.randomUUID()
来源：http://www.share.tarul.cn/Article/details/gyderbauv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.bbcook.cn/Article/details/grnihiytj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fktsv.cn/Article/details/gdsfnjphi.sHtML

[U117] JS：单元测试
来源：http://read.share.yfazqb.com/Article/details/gzzcgpyrl.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fktsv.cn/Article/details/gslmqdjke.sHtML

[U118] JS：开发服务器
来源：http://read.share.tarul.cn/Article/details/gmfwfuqos.sHtML

npm i -D vite;  npx vite
来源：http://www.share.epnwcf.com/Article/details/gjimtybef.sHtML

[U119] JS：生产构建
来源：http://baike.sjlbkw.cn/Article/details/gdaywucna.sHtML

npx vite build
来源：http://www.blog.sjlbkw.cn/Article/details/gjhjfjqru.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.vehdjk.com/Article/details/gydzuoraz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.tarul.cn/Article/details/gdmlhyuwj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggmubqidp.sHtML

统计汇总
来源：http://baike.yfazqb.com/Article/details/glykivojk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gnwbzhmcr.sHtML

按语言统计（条）：
来源：http://blog.epnwcf.com/Article/details/gmzgaqeit.sHtML

Python ......... 252
来源：http://baike.bbcook.cn/Article/details/gizyvjyfa.sHtML

PHP ............ 252
来源：http://www.blog.vehdjk.com/Article/details/gdzwtukli.sHtML

JavaScript ..... 252
来源：http://mobile.tarul.cn/Article/details/garckwxad.sHtML

TypeScript ..... 212
来源：http://read.share.tarul.cn/Article/details/gqycehugg.sHtML

Java ........... 212
来源：http://www.share.fktsv.cn/Article/details/gubuolxlt.sHtML

Go ............. 212
来源：http://www.m.share.vehdjk.com/Article/details/gadfmgecv.sHtML

Ruby ........... 212
来源：http://www.blog.fktsv.cn/Article/details/glgozppyn.sHtML

C# ............. 212
来源：http://wap.epnwcf.com/Article/details/guikwgcbe.sHtML

C .............. 30
来源：http://read.share.bbcook.cn/Article/details/gumjoxnqh.sHtML

C++ ............ 30
来源：http://m.share.sjlbkw.cn/Article/details/ghrfueiwk.sHtML

SQL ............ 90
来源：http://mobile.epnwcf.com/Article/details/glccjzhru.sHtML

Bash ........... 80
来源：http://blog.bbcook.cn/Article/details/gbhdhnmzi.sHtML

Kotlin ......... 15
来源：http://read.share.sjlbkw.cn/Article/details/gecehjjqj.sHtML

Swift .......... 15
来源：http://www.m.share.fktsv.cn/Article/details/gwbeaxmsv.sHtML

Lua ............ 10
来源：http://wap.bbcook.cn/Article/details/gpetgzfmj.sHtML

Perl ........... 10
来源：http://m.share.fktsv.cn/Article/details/ghooaqzsq.sHtML

Scala .......... 10
来源：http://read.share.bbcook.cn/Article/details/ghcyesvsb.sHtML

------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gwkglukfi.sHtML

合计 ........... 2106 条
来源：http://www.blog.epnwcf.com/Article/details/gjkzvucnv.sHtML

按章节统计：
来源：http://wap.sjlbkw.cn/Article/details/gzwubmgue.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.epnwcf.com/Article/details/gcepesscg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/gsjaqmyhu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/ghnobuzrm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.tarul.cn/Article/details/gbgwptnsd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.bbcook.cn/Article/details/grcatknmh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.tarul.cn/Article/details/glantyksc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/gqbwznjam.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.tarul.cn/Article/details/glasregmw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gyfnbduqp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/gsytmpjtc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gysacvsbd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gupsmczix.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gftjyqihy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.tarul.cn/Article/details/ggabztwff.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.sjlbkw.cn/Article/details/gvqajvoko.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gezxhbvdx.sHtML

Q SQL 专题                              90
来源：http://3g.vehdjk.com/Article/details/gwkxyekfa.sHtML

R Bash 专题                             80
来源：http://www.m.share.bbcook.cn/Article/details/gcwmmawin.sHtML

S C / C++ 专题                          60
来源：http://3g.tarul.cn/Article/details/gllodzzdf.sHtML

T 其他语言补充                          60
来源：http://www.blog.bbcook.cn/Article/details/gcfrvxxic.sHtML

U 高频实用片段                         120
来源：http://baike.tarul.cn/Article/details/gkrmywwon.sHtML

------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gtgjwckvu.sHtML

合计                                  2106 条
来源：http://3g.epnwcf.com/Article/details/gzlvvzwca.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gzwyishnb.sHtML

使用提醒
来源：http://blog.sjlbkw.cn/Article/details/gaccffrjj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gxifgjqhg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.tarul.cn/Article/details/glpfonowd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.vehdjk.com/Article/details/gkakadtoq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fktsv.cn/Article/details/gclnwbfos.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.tarul.cn/Article/details/gxeupvonw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.bbcook.cn/Article/details/gzfvpkzbh.sHtML

—— 文件结束 ——
来源：http://www.share.epnwcf.com/Article/details/gpsetrtrr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzoicpypb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.yfazqb.com/Article/details/ggowbkjss.sHtML

Common Programming Examples Cheat Book
来源：http://3g.yfazqb.com/Article/details/gsfffiuwt.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gfgzgvatb.sHtML

【收录内容】
来源：http://mobile.sjlbkw.cn/Article/details/gmkhakqim.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.tarul.cn/Article/details/gyqbpvwvm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.epnwcf.com/Article/details/gtyxxghez.sHtML

SQL · Bash · C · C++
来源：http://www.blog.yfazqb.com/Article/details/gozhkwhle.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fktsv.cn/Article/details/ggermreqf.sHtML

【使用说明】
来源：http://www.m.share.fktsv.cn/Article/details/gvasbpfel.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.epnwcf.com/Article/details/grqpldbwf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.epnwcf.com/Article/details/gxcasjevb.sHtML


<!-- 参考信息 -->