代发 wailian999

[U15] Py：高精度计时
来源：http://3g.fktsv.cn/Article/details/gimhwcbfd.sHtML

t = time.perf_counter()
来源：http://3g.epnwcf.com/Article/details/gpzqzfhep.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fktsv.cn/Article/details/gfjmrxlgi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.tarul.cn/Article/details/gmttmixsm.sHtML

[U17] Py：初始化日志
来源：http://www.share.fktsv.cn/Article/details/gopnwbqcc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.vehdjk.com/Article/details/gibtrjklt.sHtML

[U18] Py：预编译正则
来源：http://www.share.bbcook.cn/Article/details/gmvrvnqyg.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.vehdjk.com/Article/details/gulkdphya.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.epnwcf.com/Article/details/gomvnvkdy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.vehdjk.com/Article/details/ghbralttu.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fktsv.cn/Article/details/gzopmnzts.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.vehdjk.com/Article/details/gmpcbqbzg.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.yfazqb.com/Article/details/gyovgwsof.sHtML

@contextlib.contextmanager
来源：http://read.share.sjlbkw.cn/Article/details/gwdknjmrj.sHtML

[U22] Py：矩阵转置
来源：http://m.share.vehdjk.com/Article/details/gedftzsuy.sHtML

list(zip(*m))
来源：http://mobile.vehdjk.com/Article/details/gibmfaapy.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.epnwcf.com/Article/details/gkqxlgbiz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.tarul.cn/Article/details/gadrkpjir.sHtML

[U24] Py：路径操作
来源：http://www.m.share.tarul.cn/Article/details/ggdjqnahj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.yfazqb.com/Article/details/gnpstqfnk.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fktsv.cn/Article/details/gzhcrfchp.sHtML

csv.DictReader(f)
来源：http://3g.yfazqb.com/Article/details/gebaavkkt.sHtML

[U26] Py：并发下载
来源：http://mobile.vehdjk.com/Article/details/gjigpjdaj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.tarul.cn/Article/details/gkrsymerl.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.yfazqb.com/Article/details/ggqttzivl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.tarul.cn/Article/details/glkneeklz.sHtML

[U28] Py：类型别名
来源：http://baike.fktsv.cn/Article/details/gasashnlk.sHtML

UserId = int
来源：http://www.blog.tarul.cn/Article/details/gzqxysovb.sHtML

[U29] Py：属性校验
来源：http://mobile.bbcook.cn/Article/details/gwmmgftho.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.yfazqb.com/Article/details/gnrfoiykx.sHtML

[U30] Py：数据类
来源：http://mobile.fktsv.cn/Article/details/gqkicxiwz.sHtML

@dataclass(slots=True)
来源：http://3g.yfazqb.com/Article/details/gghaptswz.sHtML

[U31] Py：单测
来源：http://www.blog.tarul.cn/Article/details/gqarhmpmo.sHtML

python -m pytest -q
来源：http://www.share.epnwcf.com/Article/details/gyyouzmwj.sHtML

[U32] Py：代码格式化
来源：http://www.share.epnwcf.com/Article/details/gxgfxjasq.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.epnwcf.com/Article/details/grkvrijzh.sHtML

[U33] Py：打包发布
来源：http://blog.fktsv.cn/Article/details/getlpdexb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.vehdjk.com/Article/details/goexohrqo.sHtML

[U34] Py：判断编码
来源：http://baike.bbcook.cn/Article/details/gzygwhwtq.sHtML

chardet.detect(raw)
来源：http://read.share.sjlbkw.cn/Article/details/gexdfeqev.sHtML

[U35] Py：发送邮件
来源：http://baike.vehdjk.com/Article/details/gpyurkicx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.bbcook.cn/Article/details/ggtjuqsaq.sHtML

[U36] Py：定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gvgsomecw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.tarul.cn/Article/details/ggoggogup.sHtML

[U37] Py：读写 Excel
来源：http://mobile.yfazqb.com/Article/details/gfgvybyvu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.yfazqb.com/Article/details/gdjrkriyo.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.sjlbkw.cn/Article/details/ggcpgduga.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.yfazqb.com/Article/details/gxowfefup.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.sjlbkw.cn/Article/details/gymsdzmmq.sHtML

sys.stdout.isatty()
来源：http://m.share.tarul.cn/Article/details/gucqvthxz.sHtML

[U40] Py：打印到标准错误
来源：http://blog.epnwcf.com/Article/details/gmvbjmkid.sHtML

print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gdgwdnnoo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.yfazqb.com/Article/details/grbmbllad.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.sjlbkw.cn/Article/details/gicaotjol.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.bbcook.cn/Article/details/gkccxwqxq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.epnwcf.com/Article/details/gqsvxvenp.sHtML

[U43] PHP：声明命名空间
来源：http://baike.bbcook.cn/Article/details/gbbsfluuj.sHtML

namespace App\Http;
来源：http://baike.vehdjk.com/Article/details/gnynpzbmw.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.sjlbkw.cn/Article/details/ggieyhizg.sHtML

declare(strict_types=1);
来源：http://baike.fktsv.cn/Article/details/gzjkhhcuv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.epnwcf.com/Article/details/ghcczafcz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/geagdpkyz.sHtML

[U46] PHP：可空类型
来源：http://www.blog.bbcook.cn/Article/details/gzrlhlxso.sHtML

?string $name = null
来源：http://www.m.share.vehdjk.com/Article/details/gyptdgved.sHtML

[U47] PHP：联合类型
来源：http://blog.yfazqb.com/Article/details/gbtvxqfhr.sHtML

int|string $id
来源：http://baike.fktsv.cn/Article/details/gpnjotjjt.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.sjlbkw.cn/Article/details/glmphsdtt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.epnwcf.com/Article/details/gkexjtfhu.sHtML

[U49] PHP：只读属性
来源：http://blog.epnwcf.com/Article/details/gcwlbwhkf.sHtML

public readonly string $name
来源：http://read.share.tarul.cn/Article/details/gpmocmsit.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.yfazqb.com/Article/details/goavvamsb.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.vehdjk.com/Article/details/gdmuduhtd.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.vehdjk.com/Article/details/ggsnbvxmc.sHtML

[$a, $b] = $arr;
来源：http://www.share.tarul.cn/Article/details/gupjqvsnk.sHtML

[U52] PHP：箭头函数
来源：http://blog.vehdjk.com/Article/details/gsczzgtvv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.epnwcf.com/Article/details/gvxdthqwf.sHtML

[U53] PHP：空合并运算符
来源：http://blog.epnwcf.com/Article/details/gfjfsqyog.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.bbcook.cn/Article/details/geihcpokc.sHtML

[U54] PHP：空安全调用
来源：http://www.share.yfazqb.com/Article/details/gpabtlldv.sHtML

$obj?->method()
来源：http://www.share.tarul.cn/Article/details/gypywkuiw.sHtML

[U55] PHP：match 表达式
来源：http://blog.tarul.cn/Article/details/gvxerldev.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fktsv.cn/Article/details/glxeagfiq.sHtML

[U56] PHP：命名参数
来源：http://wap.sjlbkw.cn/Article/details/ggmdvpvdx.sHtML

f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gucfvubai.sHtML

[U57] PHP：字符串插值
来源：http://wap.bbcook.cn/Article/details/gmfechgmy.sHtML

"值: {$a}"
来源：http://blog.bbcook.cn/Article/details/gbwfeqpdr.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.bbcook.cn/Article/details/geefhleqa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.vehdjk.com/Article/details/gyhqalhfi.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.epnwcf.com/Article/details/gkikuxkwr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gftpfslad.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.sjlbkw.cn/Article/details/guwqorxtx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.yfazqb.com/Article/details/gfzgqlmot.sHtML

[U61] PHP：正则
来源：http://m.share.vehdjk.com/Article/details/gpjkrlyas.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fktsv.cn/Article/details/ghtdqmlqh.sHtML

[U62] PHP：日期对象
来源：http://blog.yfazqb.com/Article/details/gvvppwqhc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fktsv.cn/Article/details/gmptbeojd.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.yfazqb.com/Article/details/gatlbsrqq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.epnwcf.com/Article/details/guwtvznll.sHtML

[U64] PHP：目录遍历
来源：http://m.share.tarul.cn/Article/details/gwmbhduow.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fktsv.cn/Article/details/gjdwxiqkp.sHtML

[U65] PHP：会话
来源：http://read.share.epnwcf.com/Article/details/gdfvgkzvs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.bbcook.cn/Article/details/gzkjmdnil.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.vehdjk.com/Article/details/gdjgmqsov.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.yfazqb.com/Article/details/gmlleepvf.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.tarul.cn/Article/details/glkjqdgxb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.vehdjk.com/Article/details/guazlufta.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fktsv.cn/Article/details/gezzodits.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.bbcook.cn/Article/details/gvaxixtvt.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.sjlbkw.cn/Article/details/gehdubtpg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.bbcook.cn/Article/details/goypidhch.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fktsv.cn/Article/details/ggupfsefr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fktsv.cn/Article/details/gqlfdsnwn.sHtML

[U71] PHP：抛出异常
来源：http://www.share.epnwcf.com/Article/details/gkujximou.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gnspizrdi.sHtML

[U72] PHP：写错误日志
来源：http://baike.epnwcf.com/Article/details/gkjpnyfzu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.epnwcf.com/Article/details/gnslfgjmy.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fktsv.cn/Article/details/gepztxvsy.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.bbcook.cn/Article/details/gywrrpdwg.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fktsv.cn/Article/details/gwyxwsjmt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fktsv.cn/Article/details/giipzhxkk.sHtML

[U75] PHP：依赖注入
来源：http://m.share.tarul.cn/Article/details/gjnlcdiuz.sHtML

composer require psr/container
来源：http://3g.fktsv.cn/Article/details/gdqsnpfxn.sHtML

[U76] PHP：简单路由
来源：http://3g.tarul.cn/Article/details/gdrslfjih.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.bbcook.cn/Article/details/gmwjaobzo.sHtML

[U77] PHP：模板渲染
来源：http://www.share.vehdjk.com/Article/details/gskdgyfsb.sHtML

composer require twig/twig
来源：http://read.share.fktsv.cn/Article/details/gmnrwofsl.sHtML

[U78] PHP：单元测试
来源：http://m.share.epnwcf.com/Article/details/giuwbjsfi.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.vehdjk.com/Article/details/gqcdmlzxo.sHtML

[U79] PHP：静态分析
来源：http://wap.yfazqb.com/Article/details/guouanhmh.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.tarul.cn/Article/details/gtphcrstm.sHtML

[U80] PHP：代码规范修复
来源：http://wap.epnwcf.com/Article/details/gmwdkrvig.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.bbcook.cn/Article/details/grkincozh.sHtML

[U81] JS：初始化项目
来源：http://blog.tarul.cn/Article/details/gixapiynk.sHtML

npm init -y;  npm i express
来源：http://mobile.bbcook.cn/Article/details/gtkvwqmir.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.epnwcf.com/Article/details/giyadtlxg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.tarul.cn/Article/details/gubrshraq.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fktsv.cn/Article/details/gflkpooms.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fktsv.cn/Article/details/getuwkxht.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.vehdjk.com/Article/details/ginziqanp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.tarul.cn/Article/details/gptfynmgt.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/ggqrrqorw.sHtML

a?.b?.c
来源：http://mobile.sjlbkw.cn/Article/details/gflogcacw.sHtML

[U86] JS：空值合并
来源：http://mobile.tarul.cn/Article/details/gywntebmb.sHtML

a ?? b
来源：http://baike.sjlbkw.cn/Article/details/gwfpoxhmo.sHtML

[U87] JS：解构默认值
来源：http://baike.sjlbkw.cn/Article/details/gtvkjdgti.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.bbcook.cn/Article/details/guvpxedxr.sHtML

[U88] JS：对象展开合并
来源：http://mobile.sjlbkw.cn/Article/details/gopwaolmc.sHtML

{ ...a, ...b }
来源：http://wap.bbcook.cn/Article/details/gvesjvmgx.sHtML

[U89] JS：数组去重
来源：http://read.share.sjlbkw.cn/Article/details/goalzbnal.sHtML

[...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gpajipnom.sHtML

[U90] JS：数字数组排序
来源：http://read.share.epnwcf.com/Article/details/gemzxbnrq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/grlyjdqqg.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fktsv.cn/Article/details/gmcoagqol.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.vehdjk.com/Article/details/gndynkkql.sHtML

[U92] JS：深拷贝
来源：http://read.share.fktsv.cn/Article/details/gjbnrbuhz.sHtML

structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gnkypervc.sHtML

[U93] JS：模板字符串
来源：http://3g.bbcook.cn/Article/details/gbjcmvcug.sHtML

`共 ${n} 条`
来源：http://www.blog.yfazqb.com/Article/details/giibgqsqm.sHtML

[U94] JS：箭头函数
来源：http://www.share.vehdjk.com/Article/details/gzssphbfh.sHtML

const double = x => x * 2;
来源：http://baike.sjlbkw.cn/Article/details/grypfcpxp.sHtML

[U95] JS：Promise 包装
来源：http://mobile.vehdjk.com/Article/details/gzkukerwx.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.tarul.cn/Article/details/gybbngagr.sHtML

[U96] JS：async/await 与异常
来源：http://3g.bbcook.cn/Article/details/gozjggumn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gsrkkdpir.sHtML

[U97] JS：并发请求
来源：http://www.blog.fktsv.cn/Article/details/gcwiluuzo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gzwgddick.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.vehdjk.com/Article/details/gxzqdbavs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.sjlbkw.cn/Article/details/gkogvmmoy.sHtML

[U99] JS：事件监听
来源：http://www.share.epnwcf.com/Article/details/gtfoxgdri.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.epnwcf.com/Article/details/gltgvosme.sHtML

[U100] JS：DOM 查询
来源：http://blog.tarul.cn/Article/details/gskyhwvdb.sHtML

document.querySelector(".item")
来源：http://blog.sjlbkw.cn/Article/details/gpehdmwzc.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.vehdjk.com/Article/details/gpeqenfgu.sHtML

el.classList.toggle("active")
来源：http://www.share.bbcook.cn/Article/details/gcssybykr.sHtML

[U102] JS：本地存储
来源：http://3g.sjlbkw.cn/Article/details/gverfyglu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.epnwcf.com/Article/details/gyegjoefn.sHtML

[U103] JS：定时器
来源：http://www.m.share.yfazqb.com/Article/details/gbkrzpdkg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.tarul.cn/Article/details/glaksjunt.sHtML

[U104] JS：防抖
来源：http://www.share.fktsv.cn/Article/details/gfkqkxklq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gmmqgfamg.sHtML

[U105] JS：节流
来源：http://read.share.tarul.cn/Article/details/gafmmupoq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.tarul.cn/Article/details/gbuoshcdb.sHtML

[U106] JS：日期格式化
来源：http://read.share.yfazqb.com/Article/details/gukdmjmdu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.bbcook.cn/Article/details/gylsjukjx.sHtML

[U107] JS：数字千分位
来源：http://www.share.fktsv.cn/Article/details/grtgnhujm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.yfazqb.com/Article/details/gcqwqqqrj.sHtML

[U108] JS：随机整数
来源：http://www.m.share.epnwcf.com/Article/details/gbhqdxitj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.bbcook.cn/Article/details/geghgmiiz.sHtML

[U109] JS：数组分组
来源：http://mobile.sjlbkw.cn/Article/details/gacfernzo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/gashnntif.sHtML

[U110] JS：数组分块
来源：http://www.share.sjlbkw.cn/Article/details/gctrlmqpe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.vehdjk.com/Article/details/gewhcfysx.sHtML

[U111] JS：对象转 Map
来源：http://baike.bbcook.cn/Article/details/gvwlfjujv.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.epnwcf.com/Article/details/gamicqvdq.sHtML

[U112] JS：字符串补位
来源：http://wap.bbcook.cn/Article/details/gnicbbtnk.sHtML

"7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gkhyqbbhg.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fktsv.cn/Article/details/gmiglkhoa.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gjjpkynzh.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fktsv.cn/Article/details/gbdnzortb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/gduembqpc.sHtML

[U115] JS：生成 UUID
来源：http://wap.yfazqb.com/Article/details/gwdqxkniq.sHtML

crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gvuwpxjga.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fktsv.cn/Article/details/gsthjxpoa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.sjlbkw.cn/Article/details/gasroptos.sHtML

[U117] JS：单元测试
来源：http://blog.tarul.cn/Article/details/gzbrjaafj.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.epnwcf.com/Article/details/ghevsepwu.sHtML

[U118] JS：开发服务器
来源：http://www.share.vehdjk.com/Article/details/gaxxgrgkj.sHtML

npm i -D vite;  npx vite
来源：http://3g.yfazqb.com/Article/details/ggproesfc.sHtML

[U119] JS：生产构建
来源：http://mobile.epnwcf.com/Article/details/gkrubdyzv.sHtML

npx vite build
来源：http://read.share.sjlbkw.cn/Article/details/gnwdkvryo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fktsv.cn/Article/details/gecygihfu.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.sjlbkw.cn/Article/details/gzsnzsuvv.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gsxvpeolc.sHtML

统计汇总
来源：http://wap.tarul.cn/Article/details/grmpxjmoo.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxqurjqze.sHtML

按语言统计（条）：
来源：http://read.share.yfazqb.com/Article/details/gkxwzvzkl.sHtML

Python ......... 252
来源：http://m.share.yfazqb.com/Article/details/gvfgyilrw.sHtML

PHP ............ 252
来源：http://3g.yfazqb.com/Article/details/gdqmvuout.sHtML

JavaScript ..... 252
来源：http://blog.epnwcf.com/Article/details/glfgapxue.sHtML

TypeScript ..... 212
来源：http://mobile.sjlbkw.cn/Article/details/gewjgjkdf.sHtML

Java ........... 212
来源：http://www.blog.bbcook.cn/Article/details/gpettasdp.sHtML

Go ............. 212
来源：http://blog.bbcook.cn/Article/details/gkksxfuxu.sHtML

Ruby ........... 212
来源：http://mobile.epnwcf.com/Article/details/gvynaayev.sHtML

C# ............. 212
来源：http://www.blog.bbcook.cn/Article/details/gbzivbecr.sHtML

C .............. 30
来源：http://www.m.share.yfazqb.com/Article/details/gkrjwcodx.sHtML

C++ ............ 30
来源：http://read.share.bbcook.cn/Article/details/glrqxxdyf.sHtML

SQL ............ 90
来源：http://www.blog.vehdjk.com/Article/details/gioxcudhz.sHtML

Bash ........... 80
来源：http://blog.sjlbkw.cn/Article/details/gluvyjtsc.sHtML

Kotlin ......... 15
来源：http://read.share.epnwcf.com/Article/details/gniylkjqf.sHtML

Swift .......... 15
来源：http://mobile.vehdjk.com/Article/details/guverspoo.sHtML

Lua ............ 10
来源：http://3g.fktsv.cn/Article/details/ggteblxvq.sHtML

Perl ........... 10
来源：http://m.share.fktsv.cn/Article/details/gtwhbxiqs.sHtML

Scala .......... 10
来源：http://3g.tarul.cn/Article/details/gzprzwlaw.sHtML

------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gvawcovxj.sHtML

合计 ........... 2106 条
来源：http://www.share.sjlbkw.cn/Article/details/gcunucpbo.sHtML

按章节统计：
来源：http://www.m.share.yfazqb.com/Article/details/gyeasuora.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.epnwcf.com/Article/details/gouhjjpip.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/ghqozslxh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gmxjgkkrm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.bbcook.cn/Article/details/gdtsrmigv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.epnwcf.com/Article/details/gxkpoumxn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gqljsojex.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/gatjjbdjw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/gnlhhciau.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gxnlckwsi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/gpxwyxilu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gjaeaegpb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gwwuzzxmb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/grwcpexxe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.vehdjk.com/Article/details/gvnubrkou.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.sjlbkw.cn/Article/details/guismyvhv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gqzanukiq.sHtML

Q SQL 专题                              90
来源：http://3g.sjlbkw.cn/Article/details/gdnqrbaoq.sHtML

R Bash 专题                             80
来源：http://wap.epnwcf.com/Article/details/gvanoflje.sHtML

S C / C++ 专题                          60
来源：http://www.share.tarul.cn/Article/details/gerbpxyqu.sHtML

T 其他语言补充                          60
来源：http://www.m.share.epnwcf.com/Article/details/geomxelvf.sHtML

U 高频实用片段                         120
来源：http://baike.sjlbkw.cn/Article/details/gsydufqoq.sHtML

------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gnhozocqb.sHtML

合计                                  2106 条
来源：http://read.share.sjlbkw.cn/Article/details/gisyhskuw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gbhgatnzs.sHtML

使用提醒
来源：http://wap.vehdjk.com/Article/details/gmpzlebnh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/grpwksldb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.epnwcf.com/Article/details/gosgrxkck.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fktsv.cn/Article/details/gtdulkmvf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.bbcook.cn/Article/details/gfnluvmdu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.vehdjk.com/Article/details/gngaykkyv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.vehdjk.com/Article/details/gdmpmzdfy.sHtML

—— 文件结束 ——
来源：http://www.blog.fktsv.cn/Article/details/gfywhqdkv.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gohsfxqya.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.vehdjk.com/Article/details/gdxxtlmir.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.vehdjk.com/Article/details/gifhjscfn.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/giumcelcx.sHtML

【收录内容】
来源：http://wap.sjlbkw.cn/Article/details/gxuazbcaz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.epnwcf.com/Article/details/gvrxnnikq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.yfazqb.com/Article/details/gcxusghsp.sHtML

SQL · Bash · C · C++
来源：http://blog.yfazqb.com/Article/details/gtnzjxvsq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.vehdjk.com/Article/details/gtsvckhaa.sHtML

【使用说明】
来源：http://wap.vehdjk.com/Article/details/gzkpqbyrc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.bbcook.cn/Article/details/gppwegiie.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.sjlbkw.cn/Article/details/gskaphzqf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.sjlbkw.cn/Article/details/gubrsnfxy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.vehdjk.com/Article/details/gvgmowqbp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.sjlbkw.cn/Article/details/gotqqwogh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.tarul.cn/Article/details/gtmqhloge.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.sjlbkw.cn/Article/details/glanudyan.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.epnwcf.com/Article/details/gzucazzxz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fktsv.cn/Article/details/gsiobstvi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.epnwcf.com/Article/details/gjcavyrei.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.epnwcf.com/Article/details/ghemqfyrx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.epnwcf.com/Article/details/gvmfodjib.sHtML

【文件统计】
来源：http://m.share.epnwcf.com/Article/details/gmtjlnmpg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.epnwcf.com/Article/details/gmuithhtl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gmgoniend.sHtML

目  录
来源：http://m.share.tarul.cn/Article/details/griswnlal.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gzwcekrtq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fktsv.cn/Article/details/grfzmdnyv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gwmpujbcr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.epnwcf.com/Article/details/gdjqobvxd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.yfazqb.com/Article/details/gcuigdvct.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.tarul.cn/Article/details/gioispvvg.sHtML


<!-- 参考信息 -->