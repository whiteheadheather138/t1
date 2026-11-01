代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.share.sjlbkw.cn/Article/details/gymbzyrlg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.bbcook.cn/Article/details/grovbeljp.sHtML

[U20] Py：缓存函数结果
来源：http://3g.vehdjk.com/Article/details/gwyhpqmdi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.yfazqb.com/Article/details/gjquamptd.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.sjlbkw.cn/Article/details/gqhflckah.sHtML

@contextlib.contextmanager
来源：http://m.share.fktsv.cn/Article/details/gbgkfkggo.sHtML

[U22] Py：矩阵转置
来源：http://www.share.tarul.cn/Article/details/gnemjzotp.sHtML

list(zip(*m))
来源：http://3g.fktsv.cn/Article/details/gnwldkuro.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.epnwcf.com/Article/details/gmfwguvng.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.vehdjk.com/Article/details/gluwqvlxp.sHtML

[U24] Py：路径操作
来源：http://blog.bbcook.cn/Article/details/gwpctvcyz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gmcntezbv.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.sjlbkw.cn/Article/details/gdroigrdt.sHtML

csv.DictReader(f)
来源：http://www.m.share.vehdjk.com/Article/details/gfrnouzxy.sHtML

[U26] Py：并发下载
来源：http://mobile.sjlbkw.cn/Article/details/gpurlmkhs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.yfazqb.com/Article/details/gghwlnulj.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.vehdjk.com/Article/details/gujfybuux.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.tarul.cn/Article/details/gpsmeueet.sHtML

[U28] Py：类型别名
来源：http://www.blog.tarul.cn/Article/details/gefbcylcq.sHtML

UserId = int
来源：http://www.m.share.bbcook.cn/Article/details/gklbtlhbc.sHtML

[U29] Py：属性校验
来源：http://www.share.vehdjk.com/Article/details/gicwmtiqi.sHtML

@property 与 @x.setter 配合
来源：http://www.share.sjlbkw.cn/Article/details/gbapxnkin.sHtML

[U30] Py：数据类
来源：http://3g.vehdjk.com/Article/details/gxfeyumuw.sHtML

@dataclass(slots=True)
来源：http://blog.bbcook.cn/Article/details/gljvezdep.sHtML

[U31] Py：单测
来源：http://m.share.epnwcf.com/Article/details/giixswmel.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/giucobkac.sHtML

[U32] Py：代码格式化
来源：http://blog.bbcook.cn/Article/details/guqocvagy.sHtML

ruff format . && ruff check --fix .
来源：http://wap.sjlbkw.cn/Article/details/gjgnpespc.sHtML

[U33] Py：打包发布
来源：http://mobile.epnwcf.com/Article/details/gbabbyjmk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.yfazqb.com/Article/details/gdsgkwbcc.sHtML

[U34] Py：判断编码
来源：http://blog.epnwcf.com/Article/details/gmpsxuetj.sHtML

chardet.detect(raw)
来源：http://www.blog.yfazqb.com/Article/details/gyvcpjpyk.sHtML

[U35] Py：发送邮件
来源：http://wap.epnwcf.com/Article/details/gnkcszbyr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.tarul.cn/Article/details/gbwfpmbvd.sHtML

[U36] Py：定时任务
来源：http://3g.epnwcf.com/Article/details/gcypgqpux.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.yfazqb.com/Article/details/gvcuewzay.sHtML

[U37] Py：读写 Excel
来源：http://www.share.sjlbkw.cn/Article/details/gkkzhobkn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.yfazqb.com/Article/details/gpaipwoyu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.bbcook.cn/Article/details/gxrjtfkls.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fktsv.cn/Article/details/gxowmmigo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.yfazqb.com/Article/details/gcedpsrbs.sHtML

sys.stdout.isatty()
来源：http://www.m.share.yfazqb.com/Article/details/gjysdkyyo.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.bbcook.cn/Article/details/glsbuqnvv.sHtML

print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gccdorszn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.epnwcf.com/Article/details/ghgfufvbt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.vehdjk.com/Article/details/gaaxidfsk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.sjlbkw.cn/Article/details/gazuvbmht.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.yfazqb.com/Article/details/ggsdgqwtg.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.yfazqb.com/Article/details/ggpptxhgu.sHtML

namespace App\Http;
来源：http://read.share.tarul.cn/Article/details/gnwcayrrq.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fktsv.cn/Article/details/gouunbyym.sHtML

declare(strict_types=1);
来源：http://www.blog.vehdjk.com/Article/details/gcgfwnrmy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.sjlbkw.cn/Article/details/gphocsthe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/geazqjbvy.sHtML

[U46] PHP：可空类型
来源：http://blog.vehdjk.com/Article/details/giedfnylf.sHtML

?string $name = null
来源：http://www.share.yfazqb.com/Article/details/gflbwplaf.sHtML

[U47] PHP：联合类型
来源：http://3g.tarul.cn/Article/details/gyiyfugdv.sHtML

int|string $id
来源：http://www.m.share.fktsv.cn/Article/details/gxgvdutno.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/goepygqcg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.yfazqb.com/Article/details/gvbbofofc.sHtML

[U49] PHP：只读属性
来源：http://m.share.bbcook.cn/Article/details/gcjfocpxv.sHtML

public readonly string $name
来源：http://www.share.tarul.cn/Article/details/gyrmrmwvm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.bbcook.cn/Article/details/guljikyxv.sHtML

public function __construct(private int $id) {}
来源：http://read.share.yfazqb.com/Article/details/gzvghkffx.sHtML

[U51] PHP：数组解构
来源：http://m.share.bbcook.cn/Article/details/gtbnxstmx.sHtML

[$a, $b] = $arr;
来源：http://wap.vehdjk.com/Article/details/gpxvxhadm.sHtML

[U52] PHP：箭头函数
来源：http://m.share.vehdjk.com/Article/details/gymtkgion.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.epnwcf.com/Article/details/ggzuerjnn.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.vehdjk.com/Article/details/gcyfhtsey.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.vehdjk.com/Article/details/ghntriphq.sHtML

[U54] PHP：空安全调用
来源：http://wap.bbcook.cn/Article/details/glcnqibpd.sHtML

$obj?->method()
来源：http://m.share.bbcook.cn/Article/details/gnklymssd.sHtML

[U55] PHP：match 表达式
来源：http://3g.sjlbkw.cn/Article/details/gxvtsobai.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.tarul.cn/Article/details/gzlxxzbpl.sHtML

[U56] PHP：命名参数
来源：http://baike.tarul.cn/Article/details/gqdxykybv.sHtML

f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gdcqpvpqm.sHtML

[U57] PHP：字符串插值
来源：http://www.share.tarul.cn/Article/details/gccibresj.sHtML

"值: {$a}"
来源：http://www.blog.yfazqb.com/Article/details/gkftbqyjw.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.yfazqb.com/Article/details/gpxqlaplt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.yfazqb.com/Article/details/gzsojnfoj.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.tarul.cn/Article/details/gooijagqk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gqxljodvf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fktsv.cn/Article/details/gwtvrnoqc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.sjlbkw.cn/Article/details/gunxdjnrm.sHtML

[U61] PHP：正则
来源：http://baike.vehdjk.com/Article/details/gmbxdzbci.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/gdsbjoxma.sHtML

[U62] PHP：日期对象
来源：http://mobile.yfazqb.com/Article/details/gvalxyijq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.tarul.cn/Article/details/gtpgodgpk.sHtML

[U63] PHP：文件读写
来源：http://mobile.tarul.cn/Article/details/gjnofglbs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.bbcook.cn/Article/details/guwhxhigx.sHtML

[U64] PHP：目录遍历
来源：http://m.share.bbcook.cn/Article/details/gpcpxtwnl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.tarul.cn/Article/details/gqkcvnycc.sHtML

[U65] PHP：会话
来源：http://mobile.fktsv.cn/Article/details/gvovhitsj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fktsv.cn/Article/details/gbxwjclpx.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.yfazqb.com/Article/details/gcgkrqvuq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.tarul.cn/Article/details/gqltqhrak.sHtML

[U67] PHP：处理文件上传
来源：http://baike.vehdjk.com/Article/details/gbltvlpux.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.epnwcf.com/Article/details/gcaxmfbss.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fktsv.cn/Article/details/gpqvuxqvg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.vehdjk.com/Article/details/gmnpyifqe.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.vehdjk.com/Article/details/gtukyxoce.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.vehdjk.com/Article/details/gmoptboqx.sHtML

[U70] PHP：PDO 事务
来源：http://blog.tarul.cn/Article/details/glyvsekzp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.yfazqb.com/Article/details/gtsmfrain.sHtML

[U71] PHP：抛出异常
来源：http://www.share.bbcook.cn/Article/details/gmnhtbdds.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.vehdjk.com/Article/details/gwunoayik.sHtML

[U72] PHP：写错误日志
来源：http://baike.sjlbkw.cn/Article/details/gvlgfmdwx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.tarul.cn/Article/details/grlzskbtk.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.epnwcf.com/Article/details/gcmeedibq.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.tarul.cn/Article/details/gekrilyvo.sHtML

[U74] PHP：读取环境变量
来源：http://blog.bbcook.cn/Article/details/gegruczaa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.bbcook.cn/Article/details/gvyhgmmom.sHtML

[U75] PHP：依赖注入
来源：http://blog.tarul.cn/Article/details/gaciscjfw.sHtML

composer require psr/container
来源：http://www.share.sjlbkw.cn/Article/details/gzfvwdwdm.sHtML

[U76] PHP：简单路由
来源：http://mobile.bbcook.cn/Article/details/gpxnbmceh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.tarul.cn/Article/details/gaeipmfci.sHtML

[U77] PHP：模板渲染
来源：http://3g.vehdjk.com/Article/details/gcibvkcob.sHtML

composer require twig/twig
来源：http://www.blog.bbcook.cn/Article/details/gdjrmjozt.sHtML

[U78] PHP：单元测试
来源：http://3g.bbcook.cn/Article/details/gybdswvgm.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.tarul.cn/Article/details/goxyopcam.sHtML

[U79] PHP：静态分析
来源：http://www.share.epnwcf.com/Article/details/gvxsgzojj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fktsv.cn/Article/details/goswjvcxx.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.bbcook.cn/Article/details/glwooaugt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.epnwcf.com/Article/details/gdsdouuor.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fktsv.cn/Article/details/glrrmphdy.sHtML

npm init -y;  npm i express
来源：http://blog.sjlbkw.cn/Article/details/gfmcsmjtz.sHtML

[U82] JS：package.json 脚本
来源：http://blog.vehdjk.com/Article/details/gjlitkvcu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fktsv.cn/Article/details/gjkmpqlxv.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fktsv.cn/Article/details/gkryxllxv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/gzfzriglz.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.tarul.cn/Article/details/gcdthqjtq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.epnwcf.com/Article/details/gzasyboil.sHtML

[U85] JS：可选链
来源：http://3g.sjlbkw.cn/Article/details/gftmtmnjm.sHtML

a?.b?.c
来源：http://www.m.share.epnwcf.com/Article/details/gwacrefic.sHtML

[U86] JS：空值合并
来源：http://read.share.tarul.cn/Article/details/gllqwcpzf.sHtML

a ?? b
来源：http://wap.yfazqb.com/Article/details/gjzxmsxah.sHtML

[U87] JS：解构默认值
来源：http://baike.epnwcf.com/Article/details/galdgrqqy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.tarul.cn/Article/details/gmjurjozg.sHtML

[U88] JS：对象展开合并
来源：http://mobile.tarul.cn/Article/details/gjcxhiskd.sHtML

{ ...a, ...b }
来源：http://www.blog.vehdjk.com/Article/details/gefqztpcp.sHtML

[U89] JS：数组去重
来源：http://3g.yfazqb.com/Article/details/gsopvxzfl.sHtML

[...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gegozqlji.sHtML

[U90] JS：数字数组排序
来源：http://wap.epnwcf.com/Article/details/gsxgvrmmf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/ggdqleppw.sHtML

[U91] JS：对象键值遍历
来源：http://baike.bbcook.cn/Article/details/gxvmjhyht.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.tarul.cn/Article/details/ghgugnzxw.sHtML

[U92] JS：深拷贝
来源：http://blog.tarul.cn/Article/details/gowowcian.sHtML

structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gkoxckwok.sHtML

[U93] JS：模板字符串
来源：http://www.share.sjlbkw.cn/Article/details/ghvtfibse.sHtML

`共 ${n} 条`
来源：http://www.share.bbcook.cn/Article/details/gikqtpzpm.sHtML

[U94] JS：箭头函数
来源：http://mobile.tarul.cn/Article/details/gaobnsgwp.sHtML

const double = x => x * 2;
来源：http://mobile.tarul.cn/Article/details/glofqnhdp.sHtML

[U95] JS：Promise 包装
来源：http://wap.epnwcf.com/Article/details/gzjlcxyem.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.epnwcf.com/Article/details/gkbpuhsel.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fktsv.cn/Article/details/gghkalumg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gxmlkgvlg.sHtML

[U97] JS：并发请求
来源：http://www.share.yfazqb.com/Article/details/gayslkooj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gfeaxsmom.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gzsefrdnd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.tarul.cn/Article/details/gdqcbbiqc.sHtML

[U99] JS：事件监听
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnzpwvmk.sHtML

el.addEventListener("click", e => {})
来源：http://wap.sjlbkw.cn/Article/details/giofigsfh.sHtML

[U100] JS：DOM 查询
来源：http://wap.bbcook.cn/Article/details/ghbesgexv.sHtML

document.querySelector(".item")
来源：http://www.share.bbcook.cn/Article/details/gwjpotngu.sHtML

[U101] JS：classList 操作
来源：http://3g.bbcook.cn/Article/details/gfiqvhixb.sHtML

el.classList.toggle("active")
来源：http://wap.sjlbkw.cn/Article/details/gvuxqyovo.sHtML

[U102] JS：本地存储
来源：http://www.share.vehdjk.com/Article/details/ghpjraait.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fktsv.cn/Article/details/guivbquva.sHtML

[U103] JS：定时器
来源：http://www.share.bbcook.cn/Article/details/gucdeiwzs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.tarul.cn/Article/details/gwskyywvr.sHtML

[U104] JS：防抖
来源：http://www.blog.tarul.cn/Article/details/gvkhcsoxb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gqcdwnoka.sHtML

[U105] JS：节流
来源：http://baike.vehdjk.com/Article/details/gcvjdctkn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.yfazqb.com/Article/details/gcvjvyqjq.sHtML

[U106] JS：日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gvhhroqjs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.yfazqb.com/Article/details/gzypgwpct.sHtML

[U107] JS：数字千分位
来源：http://read.share.epnwcf.com/Article/details/guyjddttl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gowislyus.sHtML

[U108] JS：随机整数
来源：http://www.blog.epnwcf.com/Article/details/gysgpwjxq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fktsv.cn/Article/details/gdxkvieyz.sHtML

[U109] JS：数组分组
来源：http://m.share.fktsv.cn/Article/details/gztkzdxfg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gtlcnrlyq.sHtML

[U110] JS：数组分块
来源：http://www.share.tarul.cn/Article/details/gemhirunk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.vehdjk.com/Article/details/gbljnxdzs.sHtML

[U111] JS：对象转 Map
来源：http://baike.yfazqb.com/Article/details/gqnqbtcus.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.vehdjk.com/Article/details/gvrqejztf.sHtML

[U112] JS：字符串补位
来源：http://www.share.fktsv.cn/Article/details/godcncwec.sHtML

"7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/glsojcqnd.sHtML

[U113] JS：正则替换全部
来源：http://wap.epnwcf.com/Article/details/gbcykgakf.sHtML

s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gicxaoqyv.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.vehdjk.com/Article/details/giittajmg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/glbvdlxpm.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.tarul.cn/Article/details/grvigncdv.sHtML

crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/guxqhzffc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fktsv.cn/Article/details/gurranfob.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.bbcook.cn/Article/details/grfvqktjy.sHtML

[U117] JS：单元测试
来源：http://www.share.epnwcf.com/Article/details/gmtawjohi.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.yfazqb.com/Article/details/ghvzgpjir.sHtML

[U118] JS：开发服务器
来源：http://baike.bbcook.cn/Article/details/gljudbkbm.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqezuaci.sHtML

[U119] JS：生产构建
来源：http://3g.tarul.cn/Article/details/guygrgcvy.sHtML

npx vite build
来源：http://baike.yfazqb.com/Article/details/gtyfbvixl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.vehdjk.com/Article/details/gvojfswai.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.bbcook.cn/Article/details/gkwreegmx.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvojrbcus.sHtML

统计汇总
来源：http://read.share.tarul.cn/Article/details/gpaqntakg.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbpekwhdv.sHtML

按语言统计（条）：
来源：http://www.share.bbcook.cn/Article/details/guawybskc.sHtML

Python ......... 252
来源：http://3g.epnwcf.com/Article/details/gfyxadejd.sHtML

PHP ............ 252
来源：http://www.m.share.tarul.cn/Article/details/gpkvgeviq.sHtML

JavaScript ..... 252
来源：http://www.m.share.bbcook.cn/Article/details/gmbmrvsvo.sHtML

TypeScript ..... 212
来源：http://3g.vehdjk.com/Article/details/groruyerm.sHtML

Java ........... 212
来源：http://read.share.tarul.cn/Article/details/gzhaealbd.sHtML

Go ............. 212
来源：http://wap.vehdjk.com/Article/details/gvhyrrxzc.sHtML

Ruby ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gcoyyfcnz.sHtML

C# ............. 212
来源：http://3g.bbcook.cn/Article/details/gcrzdweii.sHtML

C .............. 30
来源：http://read.share.tarul.cn/Article/details/gmstzsbci.sHtML

C++ ............ 30
来源：http://blog.tarul.cn/Article/details/gflkldeyo.sHtML

SQL ............ 90
来源：http://m.share.sjlbkw.cn/Article/details/gfxullkja.sHtML

Bash ........... 80
来源：http://www.share.fktsv.cn/Article/details/gxpwouvwi.sHtML

Kotlin ......... 15
来源：http://www.blog.bbcook.cn/Article/details/gpexqhdvh.sHtML

Swift .......... 15
来源：http://www.blog.tarul.cn/Article/details/gutsothpw.sHtML

Lua ............ 10
来源：http://m.share.yfazqb.com/Article/details/goqpwyprp.sHtML

Perl ........... 10
来源：http://wap.bbcook.cn/Article/details/gfyydchtn.sHtML

Scala .......... 10
来源：http://baike.tarul.cn/Article/details/gfuxbcqnc.sHtML

------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gaikphpyi.sHtML

合计 ........... 2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gvaqsfpgh.sHtML

按章节统计：
来源：http://www.share.sjlbkw.cn/Article/details/gdpbfdtav.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/gblwkovym.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/gtmqltvzq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gozbzoxnz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gdhatxavp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.sjlbkw.cn/Article/details/gruyldebh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/gwfwhozlf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/getpfhezn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.yfazqb.com/Article/details/gisunfbch.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gheqfivdy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.bbcook.cn/Article/details/gskzqptxk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gpjasdtpy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gixuzusaj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbgrvmbh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.epnwcf.com/Article/details/gnscuzeug.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.epnwcf.com/Article/details/gjarkqiow.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gtalbbgzg.sHtML

Q SQL 专题                              90
来源：http://blog.fktsv.cn/Article/details/gyowqwxwn.sHtML

R Bash 专题                             80
来源：http://mobile.bbcook.cn/Article/details/grpbdwpfl.sHtML

S C / C++ 专题                          60
来源：http://baike.sjlbkw.cn/Article/details/gkmylslrf.sHtML

T 其他语言补充                          60
来源：http://mobile.bbcook.cn/Article/details/gjafcyuff.sHtML

U 高频实用片段                         120
来源：http://www.share.sjlbkw.cn/Article/details/ggikwydeh.sHtML

------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gxwffpgtl.sHtML

合计                                  2106 条
来源：http://m.share.vehdjk.com/Article/details/geoovumcp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/gkwkmocfe.sHtML

使用提醒
来源：http://3g.bbcook.cn/Article/details/gamqrfsiq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gackyoita.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.epnwcf.com/Article/details/gduceuvbx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.yfazqb.com/Article/details/gigtbofww.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.vehdjk.com/Article/details/gniekflax.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.bbcook.cn/Article/details/gfbktkzzq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.epnwcf.com/Article/details/gcophugsw.sHtML

—— 文件结束 ——
来源：http://3g.yfazqb.com/Article/details/gjfcbfkjl.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqgwwvlfu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.vehdjk.com/Article/details/garxagbnt.sHtML

Common Programming Examples Cheat Book
来源：http://blog.vehdjk.com/Article/details/gkqwroakh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gydumtacq.sHtML

【收录内容】
来源：http://m.share.tarul.cn/Article/details/gpfgsbkoi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.epnwcf.com/Article/details/gsymxdexm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.vehdjk.com/Article/details/goxbxjetq.sHtML

SQL · Bash · C · C++
来源：http://m.share.bbcook.cn/Article/details/gogjvbpud.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.sjlbkw.cn/Article/details/ggwfoaooi.sHtML

【使用说明】
来源：http://m.share.vehdjk.com/Article/details/ggutlbsli.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.tarul.cn/Article/details/gtconshzm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.tarul.cn/Article/details/ghluvwqak.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.vehdjk.com/Article/details/gdjedjwjk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.epnwcf.com/Article/details/gxysnzyrt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.epnwcf.com/Article/details/gtduklkqj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.sjlbkw.cn/Article/details/gsuhkkgeg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.vehdjk.com/Article/details/gqpkawnqh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.yfazqb.com/Article/details/gzlbtldly.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.tarul.cn/Article/details/gfzzcdbkb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.yfazqb.com/Article/details/gjjyllpng.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.tarul.cn/Article/details/gtkhvmamu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.vehdjk.com/Article/details/gpiwedxou.sHtML

【文件统计】
来源：http://read.share.epnwcf.com/Article/details/glmewtszk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.tarul.cn/Article/details/gmopitqew.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gbwvgqrwo.sHtML

目  录
来源：http://baike.tarul.cn/Article/details/gdgmnoewh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gycnxnbkl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.bbcook.cn/Article/details/gliyazbtd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fktsv.cn/Article/details/guwurpome.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fktsv.cn/Article/details/gtpipaddg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.epnwcf.com/Article/details/gkpydlmbc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.epnwcf.com/Article/details/gzjnpodjp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.sjlbkw.cn/Article/details/gfvmzvfgb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gijwwhcqq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.tarul.cn/Article/details/gkkptgjqk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gshmpeypq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fktsv.cn/Article/details/gqytkgezi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.epnwcf.com/Article/details/ghywwdvsa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/goenpxtwz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gutcroqzx.sHtML


<!-- 参考信息 -->