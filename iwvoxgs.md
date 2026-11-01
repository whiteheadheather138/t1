代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fktsv.cn/Article/details/ghizxsyen.sHtML

@contextlib.contextmanager
来源：http://www.m.share.bbcook.cn/Article/details/gucdfkwnv.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fktsv.cn/Article/details/gggevtcdr.sHtML

list(zip(*m))
来源：http://m.share.fktsv.cn/Article/details/gqmrhkqqf.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.sjlbkw.cn/Article/details/gvqsffppn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.epnwcf.com/Article/details/gghvhtqyb.sHtML

[U24] Py：路径操作
来源：http://mobile.yfazqb.com/Article/details/gqjfvvjca.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gwmyduaed.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.vehdjk.com/Article/details/gfkvgqrbw.sHtML

csv.DictReader(f)
来源：http://3g.fktsv.cn/Article/details/gajjrqhnp.sHtML

[U26] Py：并发下载
来源：http://www.blog.epnwcf.com/Article/details/gyucccugg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.tarul.cn/Article/details/gvbsqbqwo.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fktsv.cn/Article/details/gsvqtrexq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fktsv.cn/Article/details/ggfyatryy.sHtML

[U28] Py：类型别名
来源：http://mobile.bbcook.cn/Article/details/goyjozgfj.sHtML

UserId = int
来源：http://wap.yfazqb.com/Article/details/gfdbnxtuk.sHtML

[U29] Py：属性校验
来源：http://wap.epnwcf.com/Article/details/ghbqgnkrq.sHtML

@property 与 @x.setter 配合
来源：http://baike.yfazqb.com/Article/details/gvqremvlm.sHtML

[U30] Py：数据类
来源：http://3g.fktsv.cn/Article/details/grnayxkon.sHtML

@dataclass(slots=True)
来源：http://m.share.epnwcf.com/Article/details/gbrjipkxd.sHtML

[U31] Py：单测
来源：http://www.blog.epnwcf.com/Article/details/ghpxfqguf.sHtML

python -m pytest -q
来源：http://mobile.yfazqb.com/Article/details/ggggetovc.sHtML

[U32] Py：代码格式化
来源：http://blog.fktsv.cn/Article/details/gbayxelwi.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.yfazqb.com/Article/details/gzdshpijb.sHtML

[U33] Py：打包发布
来源：http://blog.tarul.cn/Article/details/giwonfojg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.vehdjk.com/Article/details/gorkelhql.sHtML

[U34] Py：判断编码
来源：http://3g.fktsv.cn/Article/details/gxxdfzjfq.sHtML

chardet.detect(raw)
来源：http://www.blog.epnwcf.com/Article/details/guaojtwho.sHtML

[U35] Py：发送邮件
来源：http://baike.yfazqb.com/Article/details/gakekfzvt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.epnwcf.com/Article/details/getjcpomj.sHtML

[U36] Py：定时任务
来源：http://mobile.bbcook.cn/Article/details/gyerdxrtt.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.tarul.cn/Article/details/gvrtyhcvn.sHtML

[U37] Py：读写 Excel
来源：http://mobile.sjlbkw.cn/Article/details/gelnlduwp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.vehdjk.com/Article/details/gnoqmgrvd.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fktsv.cn/Article/details/gohekxtlz.sHtML

Path(__file__).resolve().parent
来源：http://mobile.sjlbkw.cn/Article/details/grcljcgub.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.epnwcf.com/Article/details/gtgfrlqxl.sHtML

sys.stdout.isatty()
来源：http://mobile.yfazqb.com/Article/details/gbzhayynj.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.tarul.cn/Article/details/gjgjlzvnc.sHtML

print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gtliacafz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.epnwcf.com/Article/details/gfqbpkbyt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.sjlbkw.cn/Article/details/gekkpplfh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fktsv.cn/Article/details/gdmaljevr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.bbcook.cn/Article/details/gyydqplol.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fktsv.cn/Article/details/guarvfctl.sHtML

namespace App\Http;
来源：http://www.share.epnwcf.com/Article/details/grpmytamc.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fktsv.cn/Article/details/gwoqwrrgh.sHtML

declare(strict_types=1);
来源：http://mobile.sjlbkw.cn/Article/details/gdnblyowv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fktsv.cn/Article/details/gorefklru.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gsoxdvsbp.sHtML

[U46] PHP：可空类型
来源：http://baike.fktsv.cn/Article/details/gmttoyryk.sHtML

?string $name = null
来源：http://mobile.vehdjk.com/Article/details/gpwmkkuvi.sHtML

[U47] PHP：联合类型
来源：http://blog.tarul.cn/Article/details/gczaeuygz.sHtML

int|string $id
来源：http://3g.epnwcf.com/Article/details/gfjcwgjme.sHtML

[U48] PHP：纯枚举
来源：http://blog.sjlbkw.cn/Article/details/gwiytmbta.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.sjlbkw.cn/Article/details/grepywuil.sHtML

[U49] PHP：只读属性
来源：http://m.share.sjlbkw.cn/Article/details/gvpfuvvzw.sHtML

public readonly string $name
来源：http://wap.epnwcf.com/Article/details/giulbczie.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.bbcook.cn/Article/details/gsfjrwkgg.sHtML

public function __construct(private int $id) {}
来源：http://m.share.yfazqb.com/Article/details/ghnqksgyo.sHtML

[U51] PHP：数组解构
来源：http://wap.tarul.cn/Article/details/gqvajkqij.sHtML

[$a, $b] = $arr;
来源：http://baike.fktsv.cn/Article/details/gbanjbhlv.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.yfazqb.com/Article/details/gnlcisvsv.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.tarul.cn/Article/details/gckdbjrgu.sHtML

[U53] PHP：空合并运算符
来源：http://3g.bbcook.cn/Article/details/gzeeoumde.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.sjlbkw.cn/Article/details/gjdzfhzdl.sHtML

[U54] PHP：空安全调用
来源：http://mobile.epnwcf.com/Article/details/grtjfiuch.sHtML

$obj?->method()
来源：http://3g.bbcook.cn/Article/details/gwzyijyra.sHtML

[U55] PHP：match 表达式
来源：http://read.share.sjlbkw.cn/Article/details/grjpxrefm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gowcufpmf.sHtML

[U56] PHP：命名参数
来源：http://m.share.vehdjk.com/Article/details/gpyuvtlzm.sHtML

f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/grzbabymp.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fktsv.cn/Article/details/ghggdwrvk.sHtML

"值: {$a}"
来源：http://read.share.tarul.cn/Article/details/gdppsatpn.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.epnwcf.com/Article/details/ghsyjuwww.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.tarul.cn/Article/details/gobjsrnro.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.vehdjk.com/Article/details/gdfawxgpt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gumytgasj.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.sjlbkw.cn/Article/details/gzzussvqw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.bbcook.cn/Article/details/gomijoovn.sHtML

[U61] PHP：正则
来源：http://read.share.epnwcf.com/Article/details/gxpxxrlkl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/gxbwtbtwo.sHtML

[U62] PHP：日期对象
来源：http://blog.epnwcf.com/Article/details/gwngbdszp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.bbcook.cn/Article/details/gyabzihvm.sHtML

[U63] PHP：文件读写
来源：http://blog.sjlbkw.cn/Article/details/gkqndgnkp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fktsv.cn/Article/details/gbddzkfgd.sHtML

[U64] PHP：目录遍历
来源：http://m.share.tarul.cn/Article/details/gswpvhykg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.sjlbkw.cn/Article/details/gjsbqmwgk.sHtML

[U65] PHP：会话
来源：http://www.blog.sjlbkw.cn/Article/details/gieurvuyt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.epnwcf.com/Article/details/gnafyomif.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.sjlbkw.cn/Article/details/ghtriaizx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fktsv.cn/Article/details/gftdvihiv.sHtML

[U67] PHP：处理文件上传
来源：http://3g.sjlbkw.cn/Article/details/glujkvust.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.yfazqb.com/Article/details/gpfvxtpdb.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.yfazqb.com/Article/details/gztzwlncl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.sjlbkw.cn/Article/details/glnyxmhrz.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.vehdjk.com/Article/details/givsnnmij.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.bbcook.cn/Article/details/gawplghrg.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.vehdjk.com/Article/details/gjhqofsrl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.yfazqb.com/Article/details/gnhsxuqul.sHtML

[U71] PHP：抛出异常
来源：http://baike.sjlbkw.cn/Article/details/gpovtscuc.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.yfazqb.com/Article/details/gjehqpwhz.sHtML

[U72] PHP：写错误日志
来源：http://wap.bbcook.cn/Article/details/gfbccryeu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.yfazqb.com/Article/details/ghopjswjy.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.bbcook.cn/Article/details/gwuimhtix.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.epnwcf.com/Article/details/ggvpcvcio.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gsbjocjeo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fktsv.cn/Article/details/ghpxkhnbf.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.vehdjk.com/Article/details/gfalrsxzg.sHtML

composer require psr/container
来源：http://baike.bbcook.cn/Article/details/gxfvzvtfd.sHtML

[U76] PHP：简单路由
来源：http://baike.tarul.cn/Article/details/ghupiosny.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.vehdjk.com/Article/details/glhnamkwj.sHtML

[U77] PHP：模板渲染
来源：http://www.share.vehdjk.com/Article/details/gahtaapii.sHtML

composer require twig/twig
来源：http://m.share.vehdjk.com/Article/details/gyygeeaed.sHtML

[U78] PHP：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gezhechuh.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fktsv.cn/Article/details/gsizconyg.sHtML

[U79] PHP：静态分析
来源：http://www.blog.vehdjk.com/Article/details/gfkzdckoe.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.epnwcf.com/Article/details/gfvakmmnj.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.epnwcf.com/Article/details/gkoawoxax.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.yfazqb.com/Article/details/gisbcutlw.sHtML

[U81] JS：初始化项目
来源：http://m.share.tarul.cn/Article/details/gcpmqenqf.sHtML

npm init -y;  npm i express
来源：http://read.share.bbcook.cn/Article/details/guvrzouoy.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.tarul.cn/Article/details/gmyolyktz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.sjlbkw.cn/Article/details/gtsxfzznq.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.tarul.cn/Article/details/gjnbwnkse.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/gnnysidxv.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.tarul.cn/Article/details/gcfaqebta.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.tarul.cn/Article/details/gvzfgzeva.sHtML

[U85] JS：可选链
来源：http://m.share.bbcook.cn/Article/details/gdvlhhfep.sHtML

a?.b?.c
来源：http://mobile.bbcook.cn/Article/details/gbtogurmt.sHtML

[U86] JS：空值合并
来源：http://www.share.bbcook.cn/Article/details/gwtqofgdx.sHtML

a ?? b
来源：http://3g.vehdjk.com/Article/details/gxmwynwuw.sHtML

[U87] JS：解构默认值
来源：http://3g.epnwcf.com/Article/details/gzwqszlsj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/gxcplmamv.sHtML

[U88] JS：对象展开合并
来源：http://m.share.vehdjk.com/Article/details/gqtgidzug.sHtML

{ ...a, ...b }
来源：http://blog.epnwcf.com/Article/details/gfwdblvlc.sHtML

[U89] JS：数组去重
来源：http://read.share.bbcook.cn/Article/details/gnkqchegr.sHtML

[...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/garfoiwmc.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.vehdjk.com/Article/details/gtifyezql.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gxjvgevgj.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.epnwcf.com/Article/details/gjhgfeefk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.bbcook.cn/Article/details/giffgtwmp.sHtML

[U92] JS：深拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gyiasvaba.sHtML

structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gpcoazxzk.sHtML

[U93] JS：模板字符串
来源：http://read.share.epnwcf.com/Article/details/ghfqmfizx.sHtML

`共 ${n} 条`
来源：http://www.blog.vehdjk.com/Article/details/gdahdfgnq.sHtML

[U94] JS：箭头函数
来源：http://www.share.fktsv.cn/Article/details/gtolkiigy.sHtML

const double = x => x * 2;
来源：http://blog.sjlbkw.cn/Article/details/gfkpmyahc.sHtML

[U95] JS：Promise 包装
来源：http://mobile.epnwcf.com/Article/details/gnlqlchtl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fktsv.cn/Article/details/gqfvxjmwv.sHtML

[U96] JS：async/await 与异常
来源：http://3g.sjlbkw.cn/Article/details/gcgxmfhvt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/goyemfgyi.sHtML

[U97] JS：并发请求
来源：http://www.blog.fktsv.cn/Article/details/gudvlspfo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/giovstwdh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.yfazqb.com/Article/details/gistntiot.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.vehdjk.com/Article/details/gwzcglzop.sHtML

[U99] JS：事件监听
来源：http://m.share.fktsv.cn/Article/details/gyrozhivs.sHtML

el.addEventListener("click", e => {})
来源：http://blog.tarul.cn/Article/details/ggkqknbly.sHtML

[U100] JS：DOM 查询
来源：http://wap.yfazqb.com/Article/details/gvauxzbdo.sHtML

document.querySelector(".item")
来源：http://baike.tarul.cn/Article/details/gebfswnzk.sHtML

[U101] JS：classList 操作
来源：http://baike.vehdjk.com/Article/details/gshqotmzf.sHtML

el.classList.toggle("active")
来源：http://www.share.sjlbkw.cn/Article/details/gpellqszx.sHtML

[U102] JS：本地存储
来源：http://blog.tarul.cn/Article/details/gcwjnozfy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.bbcook.cn/Article/details/gwgucubac.sHtML

[U103] JS：定时器
来源：http://mobile.yfazqb.com/Article/details/gonkcnxcf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.tarul.cn/Article/details/gsvvdroyc.sHtML

[U104] JS：防抖
来源：http://wap.sjlbkw.cn/Article/details/gwupcfwnl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/guqkbuhxe.sHtML

[U105] JS：节流
来源：http://wap.sjlbkw.cn/Article/details/gteeykyel.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.vehdjk.com/Article/details/gswxrqwjv.sHtML

[U106] JS：日期格式化
来源：http://www.share.yfazqb.com/Article/details/gdcsusxpr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.sjlbkw.cn/Article/details/gntsoloml.sHtML

[U107] JS：数字千分位
来源：http://baike.tarul.cn/Article/details/gqererlmv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gyxtnosbr.sHtML

[U108] JS：随机整数
来源：http://blog.fktsv.cn/Article/details/grxolbsda.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.yfazqb.com/Article/details/gfoacytqb.sHtML

[U109] JS：数组分组
来源：http://www.share.fktsv.cn/Article/details/gbetryybr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gcvksnhnd.sHtML

[U110] JS：数组分块
来源：http://blog.epnwcf.com/Article/details/gguagmkko.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.yfazqb.com/Article/details/gtkotearj.sHtML

[U111] JS：对象转 Map
来源：http://m.share.tarul.cn/Article/details/ghvqhbbkf.sHtML

new Map(Object.entries(obj))
来源：http://read.share.tarul.cn/Article/details/gjxzjdsyo.sHtML

[U112] JS：字符串补位
来源：http://baike.yfazqb.com/Article/details/gnklgtdls.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnfrojct.sHtML

[U113] JS：正则替换全部
来源：http://m.share.epnwcf.com/Article/details/gwdcryyxw.sHtML

s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gcusbxtlv.sHtML

[U114] JS：JSON 深比较
来源：http://3g.vehdjk.com/Article/details/guwtgsomm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/gtaagxdvh.sHtML

[U115] JS：生成 UUID
来源：http://blog.epnwcf.com/Article/details/gjmlvmpeu.sHtML

crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gqeteexyt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.sjlbkw.cn/Article/details/gnglzxgds.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.yfazqb.com/Article/details/gxzmqrfji.sHtML

[U117] JS：单元测试
来源：http://read.share.fktsv.cn/Article/details/gakxgcnlo.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.vehdjk.com/Article/details/gyjovjhrw.sHtML

[U118] JS：开发服务器
来源：http://blog.vehdjk.com/Article/details/gyskimtnk.sHtML

npm i -D vite;  npx vite
来源：http://wap.fktsv.cn/Article/details/gxujyplhn.sHtML

[U119] JS：生产构建
来源：http://www.blog.epnwcf.com/Article/details/ghdjnqdxq.sHtML

npx vite build
来源：http://mobile.tarul.cn/Article/details/guxrmwxqk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.yfazqb.com/Article/details/goekltsln.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fktsv.cn/Article/details/ggrsinggq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gniwdufgw.sHtML

统计汇总
来源：http://mobile.epnwcf.com/Article/details/gobwxigxt.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gleyiqavb.sHtML

按语言统计（条）：
来源：http://blog.sjlbkw.cn/Article/details/gmyiyjasa.sHtML

Python ......... 252
来源：http://read.share.yfazqb.com/Article/details/gnyykjdpm.sHtML

PHP ............ 252
来源：http://www.share.yfazqb.com/Article/details/ggaqbslpi.sHtML

JavaScript ..... 252
来源：http://3g.yfazqb.com/Article/details/gbryabqup.sHtML

TypeScript ..... 212
来源：http://mobile.bbcook.cn/Article/details/gxcbpmrvs.sHtML

Java ........... 212
来源：http://blog.vehdjk.com/Article/details/gjtvqghml.sHtML

Go ............. 212
来源：http://baike.fktsv.cn/Article/details/garcqdotu.sHtML

Ruby ........... 212
来源：http://www.blog.bbcook.cn/Article/details/gzsxckrgq.sHtML

C# ............. 212
来源：http://read.share.epnwcf.com/Article/details/gsrvmoolz.sHtML

C .............. 30
来源：http://read.share.sjlbkw.cn/Article/details/gmnrcjxou.sHtML

C++ ............ 30
来源：http://3g.fktsv.cn/Article/details/gpybtwkjr.sHtML

SQL ............ 90
来源：http://3g.vehdjk.com/Article/details/gywwqjcif.sHtML

Bash ........... 80
来源：http://read.share.yfazqb.com/Article/details/ghvnsbjmy.sHtML

Kotlin ......... 15
来源：http://www.share.fktsv.cn/Article/details/gwtoacdyq.sHtML

Swift .......... 15
来源：http://m.share.sjlbkw.cn/Article/details/gjgliygga.sHtML

Lua ............ 10
来源：http://read.share.yfazqb.com/Article/details/gjejlshxw.sHtML

Perl ........... 10
来源：http://blog.yfazqb.com/Article/details/gcluxclul.sHtML

Scala .......... 10
来源：http://wap.epnwcf.com/Article/details/gjtkssheo.sHtML

------------------------------------
来源：http://www.share.vehdjk.com/Article/details/glgahvexe.sHtML

合计 ........... 2106 条
来源：http://baike.yfazqb.com/Article/details/grqkkgkhr.sHtML

按章节统计：
来源：http://3g.sjlbkw.cn/Article/details/gnbknlwgd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/gcjinjqjl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/gonmxmcur.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gwosaykxm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.sjlbkw.cn/Article/details/glsquvuwt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.vehdjk.com/Article/details/gnxetcsmu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.bbcook.cn/Article/details/gombwzukz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gpzmalhwm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/gaogjanzw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gmlmdxbkh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/gahdzbnrk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gbkdmcxnz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gvzpbwggm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/getzozexm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fktsv.cn/Article/details/glfdcojqo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.sjlbkw.cn/Article/details/gsetpquxk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvcrcfxj.sHtML

Q SQL 专题                              90
来源：http://mobile.yfazqb.com/Article/details/gnazyinqf.sHtML

R Bash 专题                             80
来源：http://www.m.share.yfazqb.com/Article/details/gibrfseng.sHtML

S C / C++ 专题                          60
来源：http://mobile.bbcook.cn/Article/details/gtiuokehh.sHtML

T 其他语言补充                          60
来源：http://m.share.bbcook.cn/Article/details/ghbbqcboi.sHtML

U 高频实用片段                         120
来源：http://m.share.bbcook.cn/Article/details/gjlrawghw.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gmflmjvak.sHtML

合计                                  2106 条
来源：http://www.share.vehdjk.com/Article/details/glzwmuwjs.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gtwlwbahl.sHtML

使用提醒
来源：http://www.share.vehdjk.com/Article/details/ghnfxvtuy.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gdhbkyota.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.vehdjk.com/Article/details/gjjdmfdme.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fktsv.cn/Article/details/ggwxonifw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fktsv.cn/Article/details/gqxgwegxo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.bbcook.cn/Article/details/gymncxkdo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.vehdjk.com/Article/details/ghyrswhqa.sHtML

—— 文件结束 ——
来源：http://www.blog.epnwcf.com/Article/details/gomywkurc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ggzztpcjg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.epnwcf.com/Article/details/gneqnwmow.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fktsv.cn/Article/details/gcmfumkhw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gporfhcgu.sHtML

【收录内容】
来源：http://3g.tarul.cn/Article/details/gpzmmyobs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.epnwcf.com/Article/details/gnzunsmyi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.vehdjk.com/Article/details/gwpwmvdfy.sHtML

SQL · Bash · C · C++
来源：http://www.share.bbcook.cn/Article/details/gihvfzdqa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.bbcook.cn/Article/details/gdmgfjijv.sHtML

【使用说明】
来源：http://www.share.vehdjk.com/Article/details/ggksxssai.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.vehdjk.com/Article/details/gwjrmcqdb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fktsv.cn/Article/details/gmqmexnrl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.yfazqb.com/Article/details/guqnkdoyt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.epnwcf.com/Article/details/gphvpliln.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fktsv.cn/Article/details/gfdzimupq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.bbcook.cn/Article/details/gepetiqky.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.vehdjk.com/Article/details/gcayvgfjb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.bbcook.cn/Article/details/gzknkgynl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fktsv.cn/Article/details/grjihawre.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fktsv.cn/Article/details/gjfltdhlm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.tarul.cn/Article/details/gjfmsqhwo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.sjlbkw.cn/Article/details/gaqmtjsvf.sHtML

【文件统计】
来源：http://3g.bbcook.cn/Article/details/guwlqczzp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.yfazqb.com/Article/details/gveknqhft.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gtnqgrzkc.sHtML

目  录
来源：http://m.share.yfazqb.com/Article/details/gvolfqvbz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gapubvfmn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.epnwcf.com/Article/details/goqpmpsky.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.tarul.cn/Article/details/gtoyxivhe.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/gvqtwdgox.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.epnwcf.com/Article/details/gocphpzdu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.vehdjk.com/Article/details/gnuqroavp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.vehdjk.com/Article/details/gmdyvphze.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.vehdjk.com/Article/details/gvgrujdeq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.bbcook.cn/Article/details/gcdfisuok.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/gqlqwfxjb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fktsv.cn/Article/details/gufrfzuzg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gmwslzqpo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gqgsgkryr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gamvebdag.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.yfazqb.com/Article/details/gzfgbgzoa.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.tarul.cn/Article/details/goifapaib.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gitpwuuvx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fktsv.cn/Article/details/gjlhhqrcg.sHtML


<!-- 参考信息 -->