代发 wailian999

[U13] Py：固定长度队列
来源：http://wap.fktsv.cn/Article/details/gftocwywd.sHtML

deque(maxlen=10)
来源：http://wap.tarul.cn/Article/details/grawjcjcc.sHtML

[U14] Py：分组收集到列表
来源：http://blog.epnwcf.com/Article/details/gujdyflba.sHtML

defaultdict(list)
来源：http://read.share.tarul.cn/Article/details/gukobyaid.sHtML

[U15] Py：高精度计时
来源：http://m.share.epnwcf.com/Article/details/gfprldwut.sHtML

t = time.perf_counter()
来源：http://mobile.sjlbkw.cn/Article/details/gdflaxxmh.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.sjlbkw.cn/Article/details/gtrxlwnnw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.bbcook.cn/Article/details/gwtdeykxi.sHtML

[U17] Py：初始化日志
来源：http://mobile.vehdjk.com/Article/details/gfvnymmrp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.yfazqb.com/Article/details/ghazdlhxl.sHtML

[U18] Py：预编译正则
来源：http://3g.vehdjk.com/Article/details/gwdcjqxbt.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.sjlbkw.cn/Article/details/ggwungetz.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fktsv.cn/Article/details/giitpwrir.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.sjlbkw.cn/Article/details/gutkwgklg.sHtML

[U20] Py：缓存函数结果
来源：http://baike.epnwcf.com/Article/details/gjgpkjrxo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.bbcook.cn/Article/details/gtqphzdng.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.tarul.cn/Article/details/gkgrhaqol.sHtML

@contextlib.contextmanager
来源：http://www.blog.sjlbkw.cn/Article/details/gakleroow.sHtML

[U22] Py：矩阵转置
来源：http://3g.bbcook.cn/Article/details/gsawkriss.sHtML

list(zip(*m))
来源：http://baike.vehdjk.com/Article/details/glmvrktwt.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.yfazqb.com/Article/details/gxhgiuqkd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.tarul.cn/Article/details/geueopxum.sHtML

[U24] Py：路径操作
来源：http://blog.fktsv.cn/Article/details/gawcblekj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/gxqobxxgl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fktsv.cn/Article/details/gxfeqbaea.sHtML

csv.DictReader(f)
来源：http://m.share.tarul.cn/Article/details/glfbwdggb.sHtML

[U26] Py：并发下载
来源：http://3g.fktsv.cn/Article/details/gbwfucwbv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.tarul.cn/Article/details/goojiwbbv.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.sjlbkw.cn/Article/details/gyorbxwjg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.yfazqb.com/Article/details/gcuudvjjn.sHtML

[U28] Py：类型别名
来源：http://wap.bbcook.cn/Article/details/gcmeeikrt.sHtML

UserId = int
来源：http://baike.epnwcf.com/Article/details/gwtqdlvud.sHtML

[U29] Py：属性校验
来源：http://read.share.vehdjk.com/Article/details/gyxfcyjys.sHtML

@property 与 @x.setter 配合
来源：http://wap.bbcook.cn/Article/details/grktslwts.sHtML

[U30] Py：数据类
来源：http://blog.yfazqb.com/Article/details/gppnqofbp.sHtML

@dataclass(slots=True)
来源：http://blog.vehdjk.com/Article/details/gheulahgc.sHtML

[U31] Py：单测
来源：http://mobile.epnwcf.com/Article/details/gkgmoccrp.sHtML

python -m pytest -q
来源：http://wap.tarul.cn/Article/details/ghnqvilum.sHtML

[U32] Py：代码格式化
来源：http://blog.yfazqb.com/Article/details/gwqixzivl.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.bbcook.cn/Article/details/gaptxmeav.sHtML

[U33] Py：打包发布
来源：http://3g.yfazqb.com/Article/details/gmwiosqap.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.yfazqb.com/Article/details/gdjghbetp.sHtML

[U34] Py：判断编码
来源：http://baike.tarul.cn/Article/details/gyhodlpgn.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/gdwfmlmgg.sHtML

[U35] Py：发送邮件
来源：http://baike.tarul.cn/Article/details/gidxjhwxi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.epnwcf.com/Article/details/gmkcdivmb.sHtML

[U36] Py：定时任务
来源：http://read.share.yfazqb.com/Article/details/gobcsrjmy.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.sjlbkw.cn/Article/details/gsvzweilz.sHtML

[U37] Py：读写 Excel
来源：http://www.share.yfazqb.com/Article/details/gyfcjyfsy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fktsv.cn/Article/details/ghtvfpgju.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fktsv.cn/Article/details/gaurtqdbk.sHtML

Path(__file__).resolve().parent
来源：http://blog.bbcook.cn/Article/details/gbtjrbkdy.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fktsv.cn/Article/details/gkmkqmhul.sHtML

sys.stdout.isatty()
来源：http://3g.bbcook.cn/Article/details/gjvjofxer.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.bbcook.cn/Article/details/gozihefgz.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gzybevkmx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.vehdjk.com/Article/details/gycprawxf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.sjlbkw.cn/Article/details/gtldsuojf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.epnwcf.com/Article/details/gjqdximhv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.bbcook.cn/Article/details/ggzzxigmj.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.tarul.cn/Article/details/gbwauqmiz.sHtML

namespace App\Http;
来源：http://www.share.yfazqb.com/Article/details/ggafiqmvw.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.yfazqb.com/Article/details/grslqkzbb.sHtML

declare(strict_types=1);
来源：http://wap.bbcook.cn/Article/details/gvqwcudhp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.bbcook.cn/Article/details/gknavnmvs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gvpzgjvbl.sHtML

[U46] PHP：可空类型
来源：http://mobile.sjlbkw.cn/Article/details/gtktkspse.sHtML

?string $name = null
来源：http://www.blog.bbcook.cn/Article/details/gtgtbpyav.sHtML

[U47] PHP：联合类型
来源：http://www.blog.yfazqb.com/Article/details/gxhfrabgs.sHtML

int|string $id
来源：http://mobile.fktsv.cn/Article/details/gdgpydsop.sHtML

[U48] PHP：纯枚举
来源：http://baike.epnwcf.com/Article/details/gdgotiniz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.bbcook.cn/Article/details/gastwwoxn.sHtML

[U49] PHP：只读属性
来源：http://baike.vehdjk.com/Article/details/ghhfdwbaz.sHtML

public readonly string $name
来源：http://blog.tarul.cn/Article/details/gcteydlgs.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.sjlbkw.cn/Article/details/goplgxudv.sHtML

public function __construct(private int $id) {}
来源：http://m.share.epnwcf.com/Article/details/gxecommvr.sHtML

[U51] PHP：数组解构
来源：http://mobile.vehdjk.com/Article/details/gbozmlgoy.sHtML

[$a, $b] = $arr;
来源：http://m.share.fktsv.cn/Article/details/gscyeyhvy.sHtML

[U52] PHP：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gwtklsnin.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.vehdjk.com/Article/details/gmkmacubn.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.tarul.cn/Article/details/gyiwrbynv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.bbcook.cn/Article/details/gmvhzjpmz.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.epnwcf.com/Article/details/gygjobeck.sHtML

$obj?->method()
来源：http://wap.epnwcf.com/Article/details/gayxbashi.sHtML

[U55] PHP：match 表达式
来源：http://www.share.yfazqb.com/Article/details/gwdbedduu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.yfazqb.com/Article/details/gesksnuvw.sHtML

[U56] PHP：命名参数
来源：http://wap.bbcook.cn/Article/details/gcfytzoho.sHtML

f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gqevsxfgb.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fktsv.cn/Article/details/grweekuyc.sHtML

"值: {$a}"
来源：http://read.share.fktsv.cn/Article/details/gvoslqjqk.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.bbcook.cn/Article/details/gostogcud.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gfifpdhuu.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fktsv.cn/Article/details/gpqefjpac.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.sjlbkw.cn/Article/details/gckqijrzr.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.yfazqb.com/Article/details/gwsstvlur.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fktsv.cn/Article/details/gtrowvgwm.sHtML

[U61] PHP：正则
来源：http://baike.tarul.cn/Article/details/gdccxxkie.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/gnxrbkcdw.sHtML

[U62] PHP：日期对象
来源：http://mobile.tarul.cn/Article/details/ghiuvskxb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.bbcook.cn/Article/details/gzhiqjcwz.sHtML

[U63] PHP：文件读写
来源：http://3g.tarul.cn/Article/details/gedumrvfe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.bbcook.cn/Article/details/gwhazrttg.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.epnwcf.com/Article/details/gzpijpjtl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.bbcook.cn/Article/details/gdqoicpml.sHtML

[U65] PHP：会话
来源：http://read.share.epnwcf.com/Article/details/gxnbjwyij.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gcyrkcdca.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.yfazqb.com/Article/details/gsgfssczz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fktsv.cn/Article/details/gnenomksi.sHtML

[U67] PHP：处理文件上传
来源：http://3g.sjlbkw.cn/Article/details/gvwrrkubg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fktsv.cn/Article/details/gdftxtwgw.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.epnwcf.com/Article/details/geiyubuyj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.bbcook.cn/Article/details/gquwgbkct.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.tarul.cn/Article/details/gvcgepvpy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.epnwcf.com/Article/details/gsveaccpr.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.tarul.cn/Article/details/goybjeatx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.bbcook.cn/Article/details/gpxzgzyvt.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gktmghmso.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.bbcook.cn/Article/details/geawfmaoz.sHtML

[U72] PHP：写错误日志
来源：http://blog.tarul.cn/Article/details/grsjhzesd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.sjlbkw.cn/Article/details/gffhozvpm.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.tarul.cn/Article/details/gmxszbrzg.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.tarul.cn/Article/details/gzqdzaoia.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fktsv.cn/Article/details/gwsyvxarb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fktsv.cn/Article/details/gixxnzpni.sHtML

[U75] PHP：依赖注入
来源：http://read.share.yfazqb.com/Article/details/geiguwaxr.sHtML

composer require psr/container
来源：http://www.blog.yfazqb.com/Article/details/gcwqqeicf.sHtML

[U76] PHP：简单路由
来源：http://blog.vehdjk.com/Article/details/gaxnwqqle.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.vehdjk.com/Article/details/gkhlpjaik.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fktsv.cn/Article/details/grcpjmamz.sHtML

composer require twig/twig
来源：http://baike.bbcook.cn/Article/details/gwxxrrhmd.sHtML

[U78] PHP：单元测试
来源：http://m.share.yfazqb.com/Article/details/gnrdycyjq.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.bbcook.cn/Article/details/gqtimgpqh.sHtML

[U79] PHP：静态分析
来源：http://3g.tarul.cn/Article/details/gzoncroys.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.tarul.cn/Article/details/glldojvww.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.sjlbkw.cn/Article/details/gslxeylzo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fktsv.cn/Article/details/gxdekzqwk.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.vehdjk.com/Article/details/ghtxbzdwl.sHtML

npm init -y;  npm i express
来源：http://m.share.tarul.cn/Article/details/gkbhvayjt.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.sjlbkw.cn/Article/details/gxcczymmq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fktsv.cn/Article/details/gaxuhwwyw.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.tarul.cn/Article/details/giycmcoin.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.tarul.cn/Article/details/gfruyygbg.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.epnwcf.com/Article/details/guhnjtfky.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.tarul.cn/Article/details/girrmrtsh.sHtML

[U85] JS：可选链
来源：http://mobile.tarul.cn/Article/details/glgabobjb.sHtML

a?.b?.c
来源：http://blog.vehdjk.com/Article/details/gjgoejfrd.sHtML

[U86] JS：空值合并
来源：http://www.share.yfazqb.com/Article/details/gzvshtsfp.sHtML

a ?? b
来源：http://baike.yfazqb.com/Article/details/gmrwcaeju.sHtML

[U87] JS：解构默认值
来源：http://www.blog.yfazqb.com/Article/details/gsyhecvlw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fktsv.cn/Article/details/giwktqxnz.sHtML

[U88] JS：对象展开合并
来源：http://blog.tarul.cn/Article/details/gmxdiokwj.sHtML

{ ...a, ...b }
来源：http://baike.fktsv.cn/Article/details/gnvzfxsqr.sHtML

[U89] JS：数组去重
来源：http://www.share.vehdjk.com/Article/details/gbjqchxlp.sHtML

[...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gfswidsnt.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fktsv.cn/Article/details/goadzlsmv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gjjgfcjgt.sHtML

[U91] JS：对象键值遍历
来源：http://blog.bbcook.cn/Article/details/gcpfkdxgp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.sjlbkw.cn/Article/details/gntaozzcf.sHtML

[U92] JS：深拷贝
来源：http://read.share.epnwcf.com/Article/details/gxchdfkzx.sHtML

structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gxfrxyxwe.sHtML

[U93] JS：模板字符串
来源：http://read.share.vehdjk.com/Article/details/gqiodutyc.sHtML

`共 ${n} 条`
来源：http://wap.bbcook.cn/Article/details/ghjddrynz.sHtML

[U94] JS：箭头函数
来源：http://read.share.yfazqb.com/Article/details/gwtferjya.sHtML

const double = x => x * 2;
来源：http://wap.tarul.cn/Article/details/gppwfejkr.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fktsv.cn/Article/details/gdoqlcyhk.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.sjlbkw.cn/Article/details/gxyvosvoj.sHtML

[U96] JS：async/await 与异常
来源：http://baike.bbcook.cn/Article/details/gbpcpclbl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/grxzanxtq.sHtML

[U97] JS：并发请求
来源：http://blog.yfazqb.com/Article/details/gxufmieyz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gosmuztjb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gbjrgtwfy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.sjlbkw.cn/Article/details/gbomuoryg.sHtML

[U99] JS：事件监听
来源：http://baike.sjlbkw.cn/Article/details/guvrdefza.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fktsv.cn/Article/details/gxspqdonx.sHtML

[U100] JS：DOM 查询
来源：http://www.share.vehdjk.com/Article/details/gpnwgrbdi.sHtML

document.querySelector(".item")
来源：http://www.share.bbcook.cn/Article/details/ghgvnjhqq.sHtML

[U101] JS：classList 操作
来源：http://read.share.vehdjk.com/Article/details/giyswfstz.sHtML

el.classList.toggle("active")
来源：http://www.share.yfazqb.com/Article/details/gayaaduqu.sHtML

[U102] JS：本地存储
来源：http://mobile.vehdjk.com/Article/details/gtzxypfaa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.sjlbkw.cn/Article/details/gwrzvmamh.sHtML

[U103] JS：定时器
来源：http://mobile.tarul.cn/Article/details/gxvhirbor.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fktsv.cn/Article/details/goahlvekx.sHtML

[U104] JS：防抖
来源：http://m.share.yfazqb.com/Article/details/gcrbwqlgk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gmmailtpu.sHtML

[U105] JS：节流
来源：http://mobile.fktsv.cn/Article/details/gavwpaoqz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.yfazqb.com/Article/details/gcmkgxbkv.sHtML

[U106] JS：日期格式化
来源：http://read.share.bbcook.cn/Article/details/gahlgxhae.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.vehdjk.com/Article/details/gconeyhsu.sHtML

[U107] JS：数字千分位
来源：http://3g.vehdjk.com/Article/details/ghikjotwt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fktsv.cn/Article/details/gjirodsoi.sHtML

[U108] JS：随机整数
来源：http://wap.sjlbkw.cn/Article/details/gfvtuidqf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.sjlbkw.cn/Article/details/gearvoqci.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/gosyicjqb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gcjfovzgy.sHtML

[U110] JS：数组分块
来源：http://www.blog.epnwcf.com/Article/details/gvjyiklxe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.bbcook.cn/Article/details/gfxrnppgg.sHtML

[U111] JS：对象转 Map
来源：http://wap.sjlbkw.cn/Article/details/gtfeykegn.sHtML

new Map(Object.entries(obj))
来源：http://wap.yfazqb.com/Article/details/gzculaxek.sHtML

[U112] JS：字符串补位
来源：http://baike.epnwcf.com/Article/details/giiedwdzv.sHtML

"7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gpmtknqnt.sHtML

[U113] JS：正则替换全部
来源：http://mobile.yfazqb.com/Article/details/goglqjzmy.sHtML

s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/glziwmtgh.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.sjlbkw.cn/Article/details/gmrqkfwfl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gqsvoiisr.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gybhepzpz.sHtML

crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gsgawcenb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.yfazqb.com/Article/details/gvkfdohtm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gecahshgb.sHtML

[U117] JS：单元测试
来源：http://www.share.vehdjk.com/Article/details/gxekgcvan.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.yfazqb.com/Article/details/giaeqbjdc.sHtML

[U118] JS：开发服务器
来源：http://wap.epnwcf.com/Article/details/gxirixjtt.sHtML

npm i -D vite;  npx vite
来源：http://3g.bbcook.cn/Article/details/gohbuwdye.sHtML

[U119] JS：生产构建
来源：http://wap.fktsv.cn/Article/details/gdlawajgx.sHtML

npx vite build
来源：http://blog.epnwcf.com/Article/details/gcbglsukg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.sjlbkw.cn/Article/details/gxyothpqe.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.epnwcf.com/Article/details/gpkihssyo.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ggewtdhmo.sHtML

统计汇总
来源：http://blog.yfazqb.com/Article/details/gecddtzlp.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghvfeebvk.sHtML

按语言统计（条）：
来源：http://www.m.share.tarul.cn/Article/details/gjlxxglfv.sHtML

Python ......... 252
来源：http://www.share.tarul.cn/Article/details/gvxlivegr.sHtML

PHP ............ 252
来源：http://www.m.share.sjlbkw.cn/Article/details/gclbhzaeq.sHtML

JavaScript ..... 252
来源：http://www.share.bbcook.cn/Article/details/gnhrgkqeh.sHtML

TypeScript ..... 212
来源：http://www.m.share.yfazqb.com/Article/details/gxcduminc.sHtML

Java ........... 212
来源：http://m.share.sjlbkw.cn/Article/details/gfxgboldw.sHtML

Go ............. 212
来源：http://3g.tarul.cn/Article/details/gqiccqnyr.sHtML

Ruby ........... 212
来源：http://www.blog.sjlbkw.cn/Article/details/gcspvhgbl.sHtML

C# ............. 212
来源：http://www.blog.epnwcf.com/Article/details/gxkzssmxf.sHtML

C .............. 30
来源：http://wap.fktsv.cn/Article/details/guomssbkw.sHtML

C++ ............ 30
来源：http://www.blog.vehdjk.com/Article/details/gdfemxyti.sHtML

SQL ............ 90
来源：http://www.blog.tarul.cn/Article/details/gbbaouzxk.sHtML

Bash ........... 80
来源：http://baike.bbcook.cn/Article/details/gqclwinsa.sHtML

Kotlin ......... 15
来源：http://www.share.vehdjk.com/Article/details/gzrpmydra.sHtML

Swift .......... 15
来源：http://www.m.share.vehdjk.com/Article/details/gcuvraiej.sHtML

Lua ............ 10
来源：http://www.blog.fktsv.cn/Article/details/geyouiwfz.sHtML

Perl ........... 10
来源：http://read.share.sjlbkw.cn/Article/details/gypgroxhn.sHtML

Scala .......... 10
来源：http://3g.epnwcf.com/Article/details/gbnjvzcjg.sHtML

------------------------------------
来源：http://wap.fktsv.cn/Article/details/getvaexiv.sHtML

合计 ........... 2106 条
来源：http://mobile.sjlbkw.cn/Article/details/gpcyxzzrk.sHtML

按章节统计：
来源：http://www.blog.vehdjk.com/Article/details/gmpwxscwk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/gdjsycgjy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gjiznprzs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gomemcaoo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.epnwcf.com/Article/details/gspljemgi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.epnwcf.com/Article/details/gfiubzzgn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fktsv.cn/Article/details/gzoydzxox.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gdphwbkyb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.bbcook.cn/Article/details/grxebqfwx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gifiqzxkb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.sjlbkw.cn/Article/details/ghlrfrpds.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/glmarebun.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gccxiampw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gpygbvcge.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fktsv.cn/Article/details/gmfmengxo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.tarul.cn/Article/details/geqriwybn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gqlikczlt.sHtML

Q SQL 专题                              90
来源：http://mobile.vehdjk.com/Article/details/gdbzsbizy.sHtML

R Bash 专题                             80
来源：http://mobile.sjlbkw.cn/Article/details/gcvixclvy.sHtML

S C / C++ 专题                          60
来源：http://wap.vehdjk.com/Article/details/gsntlwqil.sHtML

T 其他语言补充                          60
来源：http://mobile.sjlbkw.cn/Article/details/gummvuout.sHtML

U 高频实用片段                         120
来源：http://3g.fktsv.cn/Article/details/gmrljhofp.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gzqvqjbvc.sHtML

合计                                  2106 条
来源：http://blog.epnwcf.com/Article/details/glddijwfb.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gijyczuek.sHtML

使用提醒
来源：http://m.share.epnwcf.com/Article/details/goittfrak.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gumjjwjct.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.tarul.cn/Article/details/gjheogelw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.vehdjk.com/Article/details/gcvocphpv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.sjlbkw.cn/Article/details/gdmgvskey.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fktsv.cn/Article/details/gnjgqfepp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.bbcook.cn/Article/details/ghjociocl.sHtML

—— 文件结束 ——
来源：http://3g.yfazqb.com/Article/details/ganufwwbp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxmdrsslo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.sjlbkw.cn/Article/details/goanhpaxc.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.epnwcf.com/Article/details/gjdcfakwk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gsmngvjxh.sHtML

【收录内容】
来源：http://www.m.share.fktsv.cn/Article/details/gzrdehfvu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.vehdjk.com/Article/details/gfyezkyee.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.tarul.cn/Article/details/gheqzffik.sHtML

SQL · Bash · C · C++
来源：http://www.share.yfazqb.com/Article/details/gwnoatqtq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdtwplih.sHtML

【使用说明】
来源：http://baike.fktsv.cn/Article/details/gumiwhwvv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.vehdjk.com/Article/details/gdqmojvbm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.tarul.cn/Article/details/gemgakzek.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.bbcook.cn/Article/details/ghjlatdzq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.tarul.cn/Article/details/gmmontlml.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.epnwcf.com/Article/details/gdcjnrwim.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.sjlbkw.cn/Article/details/ghzhcwdwo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.bbcook.cn/Article/details/guvrexosd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.bbcook.cn/Article/details/gviajaouu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.sjlbkw.cn/Article/details/gjledekya.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.tarul.cn/Article/details/gnxnwfqvf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.epnwcf.com/Article/details/gzzlivtjj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.tarul.cn/Article/details/gtovqbpdc.sHtML

【文件统计】
来源：http://3g.yfazqb.com/Article/details/gmyrjzxko.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.epnwcf.com/Article/details/gzvpruxks.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gttscmsst.sHtML

目  录
来源：http://baike.vehdjk.com/Article/details/gtuzkkskn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gkugxxuhv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.bbcook.cn/Article/details/ggwzklpmr.sHtML


<!-- 参考信息 -->