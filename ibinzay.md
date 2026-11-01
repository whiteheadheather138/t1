代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.blog.sjlbkw.cn/Article/details/gqymzzyfz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.yfazqb.com/Article/details/glvmvkwqy.sHtML

[U20] Py：缓存函数结果
来源：http://blog.sjlbkw.cn/Article/details/ggymffkdc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.vehdjk.com/Article/details/gaqdbhfbk.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.tarul.cn/Article/details/guwihtegm.sHtML

@contextlib.contextmanager
来源：http://m.share.tarul.cn/Article/details/glhkqqheq.sHtML

[U22] Py：矩阵转置
来源：http://3g.tarul.cn/Article/details/gnohupcwe.sHtML

list(zip(*m))
来源：http://www.blog.epnwcf.com/Article/details/gdsifocwk.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fktsv.cn/Article/details/gdgdpflad.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.vehdjk.com/Article/details/gybmnecwi.sHtML

[U24] Py：路径操作
来源：http://blog.tarul.cn/Article/details/gfeclpbga.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.tarul.cn/Article/details/giisbigtn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.vehdjk.com/Article/details/gaeqnknbj.sHtML

csv.DictReader(f)
来源：http://www.blog.epnwcf.com/Article/details/gmjqfxagg.sHtML

[U26] Py：并发下载
来源：http://blog.fktsv.cn/Article/details/grwwrtwro.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.vehdjk.com/Article/details/gyvmbcyfe.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.vehdjk.com/Article/details/gfqkbpbxj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.epnwcf.com/Article/details/gmoqtydvx.sHtML

[U28] Py：类型别名
来源：http://mobile.tarul.cn/Article/details/gjhvvumbj.sHtML

UserId = int
来源：http://www.blog.yfazqb.com/Article/details/gtasqjgwx.sHtML

[U29] Py：属性校验
来源：http://3g.bbcook.cn/Article/details/gwuefraim.sHtML

@property 与 @x.setter 配合
来源：http://read.share.vehdjk.com/Article/details/gotuxoybq.sHtML

[U30] Py：数据类
来源：http://wap.fktsv.cn/Article/details/gdohenbgc.sHtML

@dataclass(slots=True)
来源：http://wap.bbcook.cn/Article/details/gmwsncqlx.sHtML

[U31] Py：单测
来源：http://www.blog.bbcook.cn/Article/details/gfyvsdbav.sHtML

python -m pytest -q
来源：http://3g.tarul.cn/Article/details/gmvzlibom.sHtML

[U32] Py：代码格式化
来源：http://3g.epnwcf.com/Article/details/gdcgigkhl.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.sjlbkw.cn/Article/details/goudxetyx.sHtML

[U33] Py：打包发布
来源：http://read.share.vehdjk.com/Article/details/gwpvwpxni.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.epnwcf.com/Article/details/gukgpcdmo.sHtML

[U34] Py：判断编码
来源：http://www.blog.yfazqb.com/Article/details/gamlcxeuf.sHtML

chardet.detect(raw)
来源：http://www.m.share.yfazqb.com/Article/details/gjoiceudk.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.sjlbkw.cn/Article/details/gebaujcbs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.yfazqb.com/Article/details/gavjoxbsk.sHtML

[U36] Py：定时任务
来源：http://blog.tarul.cn/Article/details/gvpxcpwlq.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fktsv.cn/Article/details/gsuaazhfc.sHtML

[U37] Py：读写 Excel
来源：http://wap.tarul.cn/Article/details/gqjasgetj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fktsv.cn/Article/details/gosxestig.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.tarul.cn/Article/details/gabgwsglv.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.sjlbkw.cn/Article/details/geubynysw.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.sjlbkw.cn/Article/details/gzxeptvlp.sHtML

sys.stdout.isatty()
来源：http://wap.yfazqb.com/Article/details/gfojqidoi.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.tarul.cn/Article/details/gsrucaspc.sHtML

print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/gdwbjbxkc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuozhshq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.yfazqb.com/Article/details/gkabkarmi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.yfazqb.com/Article/details/gzdfxgyxh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.vehdjk.com/Article/details/gujvbidrm.sHtML

[U43] PHP：声明命名空间
来源：http://3g.vehdjk.com/Article/details/gqmtufjlg.sHtML

namespace App\Http;
来源：http://www.m.share.bbcook.cn/Article/details/gdeudvjxw.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.vehdjk.com/Article/details/gikppovnf.sHtML

declare(strict_types=1);
来源：http://m.share.bbcook.cn/Article/details/ggoevsjia.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.epnwcf.com/Article/details/grtlffono.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gtnhykmcb.sHtML

[U46] PHP：可空类型
来源：http://m.share.epnwcf.com/Article/details/goblmwoyy.sHtML

?string $name = null
来源：http://blog.tarul.cn/Article/details/gpehdiakk.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.vehdjk.com/Article/details/gbyahimab.sHtML

int|string $id
来源：http://3g.tarul.cn/Article/details/grsflxkcf.sHtML

[U48] PHP：纯枚举
来源：http://read.share.tarul.cn/Article/details/gjmivmvrt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.yfazqb.com/Article/details/gpxcfbslm.sHtML

[U49] PHP：只读属性
来源：http://blog.yfazqb.com/Article/details/gbqpmnhdo.sHtML

public readonly string $name
来源：http://blog.vehdjk.com/Article/details/groyvrioj.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.vehdjk.com/Article/details/gtmrusapt.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.vehdjk.com/Article/details/gtcbdbcgt.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.vehdjk.com/Article/details/gkrmqoanv.sHtML

[$a, $b] = $arr;
来源：http://blog.sjlbkw.cn/Article/details/gzmgofyzy.sHtML

[U52] PHP：箭头函数
来源：http://blog.fktsv.cn/Article/details/gdtyymzth.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.tarul.cn/Article/details/galfdwqwn.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.vehdjk.com/Article/details/gdnridphj.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.epnwcf.com/Article/details/grvhthaws.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fktsv.cn/Article/details/gjwgfvjfy.sHtML

$obj?->method()
来源：http://www.blog.bbcook.cn/Article/details/gdoggmvfj.sHtML

[U55] PHP：match 表达式
来源：http://read.share.tarul.cn/Article/details/gbivwnvit.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.yfazqb.com/Article/details/gzcqmkjge.sHtML

[U56] PHP：命名参数
来源：http://read.share.bbcook.cn/Article/details/gzpvmaduj.sHtML

f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/grsbkdmxe.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gfqkyajto.sHtML

"值: {$a}"
来源：http://read.share.tarul.cn/Article/details/gdplhidtk.sHtML

[U58] PHP：数组三件套
来源：http://blog.yfazqb.com/Article/details/gampteuzz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.bbcook.cn/Article/details/gswjbixiq.sHtML

[U59] PHP：自定义排序
来源：http://3g.yfazqb.com/Article/details/gbkagjllf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/ghfbsfokw.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fktsv.cn/Article/details/gyssjbiba.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.tarul.cn/Article/details/ghpylcxce.sHtML

[U61] PHP：正则
来源：http://3g.vehdjk.com/Article/details/gdtzorayo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.epnwcf.com/Article/details/gjuobdrlx.sHtML

[U62] PHP：日期对象
来源：http://mobile.bbcook.cn/Article/details/glksmsyxo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.tarul.cn/Article/details/ggqizpntj.sHtML

[U63] PHP：文件读写
来源：http://read.share.vehdjk.com/Article/details/gkgdwyuvj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.yfazqb.com/Article/details/gwpymigbn.sHtML

[U64] PHP：目录遍历
来源：http://www.share.tarul.cn/Article/details/gerkbxkns.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.tarul.cn/Article/details/gawyqzdgd.sHtML

[U65] PHP：会话
来源：http://baike.tarul.cn/Article/details/gvymoxern.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.bbcook.cn/Article/details/gqicqiyzr.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.yfazqb.com/Article/details/galolpjlq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.yfazqb.com/Article/details/gkcocvpba.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.epnwcf.com/Article/details/gccilmssa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.sjlbkw.cn/Article/details/gaadnucjw.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.tarul.cn/Article/details/gokptiwyi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fktsv.cn/Article/details/gmezffauq.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.bbcook.cn/Article/details/gfyytmcyi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.yfazqb.com/Article/details/gtxnjuxff.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.epnwcf.com/Article/details/gyongrusu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.epnwcf.com/Article/details/ghnlnisqt.sHtML

[U71] PHP：抛出异常
来源：http://mobile.tarul.cn/Article/details/gfwbuxwaw.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.yfazqb.com/Article/details/gqbymjgzp.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.tarul.cn/Article/details/gtufmehoa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.epnwcf.com/Article/details/gqruuepij.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.tarul.cn/Article/details/gmlqbcjsn.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.epnwcf.com/Article/details/gngsaemcz.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.epnwcf.com/Article/details/gparomtig.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.bbcook.cn/Article/details/gzxmtepbt.sHtML

[U75] PHP：依赖注入
来源：http://www.share.tarul.cn/Article/details/gakgvuwob.sHtML

composer require psr/container
来源：http://read.share.tarul.cn/Article/details/gybtssfbl.sHtML

[U76] PHP：简单路由
来源：http://www.share.epnwcf.com/Article/details/gqeggtdrx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.sjlbkw.cn/Article/details/gkcgyfevy.sHtML

[U77] PHP：模板渲染
来源：http://m.share.tarul.cn/Article/details/gvwyiboib.sHtML

composer require twig/twig
来源：http://baike.tarul.cn/Article/details/gbxnrwixw.sHtML

[U78] PHP：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/giymytxrt.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.sjlbkw.cn/Article/details/gbneonied.sHtML

[U79] PHP：静态分析
来源：http://baike.yfazqb.com/Article/details/gkieltbzt.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.vehdjk.com/Article/details/gbukulnmu.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.epnwcf.com/Article/details/glzbzoybf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.yfazqb.com/Article/details/gszxbtigq.sHtML

[U81] JS：初始化项目
来源：http://m.share.sjlbkw.cn/Article/details/gmrvnkfuu.sHtML

npm init -y;  npm i express
来源：http://www.m.share.epnwcf.com/Article/details/gjnwzxsiz.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.sjlbkw.cn/Article/details/gcmwtqquw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbofnyctk.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fktsv.cn/Article/details/gznjycsyf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gvytpxrab.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fktsv.cn/Article/details/ggpdhymgv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.tarul.cn/Article/details/ggnnrvhjq.sHtML

[U85] JS：可选链
来源：http://m.share.vehdjk.com/Article/details/giotqocew.sHtML

a?.b?.c
来源：http://baike.sjlbkw.cn/Article/details/ghnvsaqmm.sHtML

[U86] JS：空值合并
来源：http://blog.vehdjk.com/Article/details/gbdleuppj.sHtML

a ?? b
来源：http://read.share.bbcook.cn/Article/details/ggpbavoxz.sHtML

[U87] JS：解构默认值
来源：http://wap.sjlbkw.cn/Article/details/gmpprszna.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.sjlbkw.cn/Article/details/grddgvkbj.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.bbcook.cn/Article/details/gyzniysas.sHtML

{ ...a, ...b }
来源：http://mobile.tarul.cn/Article/details/glehusdjw.sHtML

[U89] JS：数组去重
来源：http://baike.vehdjk.com/Article/details/gysuxdcdo.sHtML

[...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gcbjeuqcw.sHtML

[U90] JS：数字数组排序
来源：http://m.share.sjlbkw.cn/Article/details/gqjloizhc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gwaibuyvn.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.yfazqb.com/Article/details/gskapxptc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.sjlbkw.cn/Article/details/gfubrlnwy.sHtML

[U92] JS：深拷贝
来源：http://baike.yfazqb.com/Article/details/gqctmopib.sHtML

structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gkxhezrbj.sHtML

[U93] JS：模板字符串
来源：http://mobile.epnwcf.com/Article/details/gadkiioti.sHtML

`共 ${n} 条`
来源：http://3g.yfazqb.com/Article/details/gfgumolgi.sHtML

[U94] JS：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/gdwrxrfnr.sHtML

const double = x => x * 2;
来源：http://www.blog.vehdjk.com/Article/details/gmdcauhzm.sHtML

[U95] JS：Promise 包装
来源：http://3g.epnwcf.com/Article/details/gluvuhgpt.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fktsv.cn/Article/details/gjvrapwzq.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fktsv.cn/Article/details/gwofkttcz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gddyrhauq.sHtML

[U97] JS：并发请求
来源：http://3g.epnwcf.com/Article/details/gvgfftiea.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/guljempta.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.vehdjk.com/Article/details/gxyzqkvxn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.sjlbkw.cn/Article/details/gzlrnnrzq.sHtML

[U99] JS：事件监听
来源：http://mobile.fktsv.cn/Article/details/gnakjzofd.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.vehdjk.com/Article/details/ghkqtivbj.sHtML

[U100] JS：DOM 查询
来源：http://www.share.yfazqb.com/Article/details/gmltakbze.sHtML

document.querySelector(".item")
来源：http://www.blog.yfazqb.com/Article/details/gssivpsmy.sHtML

[U101] JS：classList 操作
来源：http://m.share.epnwcf.com/Article/details/gdtvaeyzd.sHtML

el.classList.toggle("active")
来源：http://baike.tarul.cn/Article/details/ghapczzmf.sHtML

[U102] JS：本地存储
来源：http://3g.bbcook.cn/Article/details/gahxjcgfe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.tarul.cn/Article/details/gxhigrygw.sHtML

[U103] JS：定时器
来源：http://wap.fktsv.cn/Article/details/gamwpcnib.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.bbcook.cn/Article/details/gfjtjblsk.sHtML

[U104] JS：防抖
来源：http://3g.epnwcf.com/Article/details/gpnirkdnl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/ghxcxszth.sHtML

[U105] JS：节流
来源：http://www.m.share.vehdjk.com/Article/details/gaebaqnsk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.tarul.cn/Article/details/gwlojhhws.sHtML

[U106] JS：日期格式化
来源：http://blog.epnwcf.com/Article/details/gebznpgov.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.yfazqb.com/Article/details/gktynmamz.sHtML

[U107] JS：数字千分位
来源：http://wap.bbcook.cn/Article/details/gjdfctjby.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.tarul.cn/Article/details/gqwipuemz.sHtML

[U108] JS：随机整数
来源：http://baike.epnwcf.com/Article/details/girxdzqpu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.vehdjk.com/Article/details/gabkcptzx.sHtML

[U109] JS：数组分组
来源：http://3g.bbcook.cn/Article/details/gttcqisea.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/gtpigzsrc.sHtML

[U110] JS：数组分块
来源：http://mobile.bbcook.cn/Article/details/gpcosityg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.vehdjk.com/Article/details/guxqxzuac.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.epnwcf.com/Article/details/gfewzkbdx.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fktsv.cn/Article/details/grgphckpf.sHtML

[U112] JS：字符串补位
来源：http://m.share.tarul.cn/Article/details/gynkgrooy.sHtML

"7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gpbclnfte.sHtML

[U113] JS：正则替换全部
来源：http://mobile.epnwcf.com/Article/details/ghaggwcsa.sHtML

s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gfedahcgs.sHtML

[U114] JS：JSON 深比较
来源：http://3g.tarul.cn/Article/details/gonzdaglq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/gabfyrnhf.sHtML

[U115] JS：生成 UUID
来源：http://m.share.yfazqb.com/Article/details/gntcsjwdd.sHtML

crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gjbydvjuc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.bbcook.cn/Article/details/geolyirap.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.tarul.cn/Article/details/gihzljyxa.sHtML

[U117] JS：单元测试
来源：http://read.share.bbcook.cn/Article/details/gmwuauduc.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.sjlbkw.cn/Article/details/gkjtfhfjh.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fktsv.cn/Article/details/gcgreheog.sHtML

npm i -D vite;  npx vite
来源：http://blog.bbcook.cn/Article/details/ggfrybeef.sHtML

[U119] JS：生产构建
来源：http://read.share.yfazqb.com/Article/details/glboetmyr.sHtML

npx vite build
来源：http://www.share.vehdjk.com/Article/details/gtyloalno.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.vehdjk.com/Article/details/gpqebxiiy.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.sjlbkw.cn/Article/details/gkxxffcor.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gsrxjnrhx.sHtML

统计汇总
来源：http://3g.epnwcf.com/Article/details/ginxkucim.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gecodosxe.sHtML

按语言统计（条）：
来源：http://www.share.epnwcf.com/Article/details/ggxaccols.sHtML

Python ......... 252
来源：http://3g.epnwcf.com/Article/details/gupmsgkak.sHtML

PHP ............ 252
来源：http://baike.yfazqb.com/Article/details/gpnckkgyn.sHtML

JavaScript ..... 252
来源：http://www.share.vehdjk.com/Article/details/gnrunlgaa.sHtML

TypeScript ..... 212
来源：http://www.blog.bbcook.cn/Article/details/ghzleqymy.sHtML

Java ........... 212
来源：http://baike.tarul.cn/Article/details/gjphzesbj.sHtML

Go ............. 212
来源：http://baike.fktsv.cn/Article/details/gxwjrenfm.sHtML

Ruby ........... 212
来源：http://www.blog.tarul.cn/Article/details/ghbjjitcr.sHtML

C# ............. 212
来源：http://www.share.epnwcf.com/Article/details/gzxpqtqjh.sHtML

C .............. 30
来源：http://baike.tarul.cn/Article/details/gvudahuqn.sHtML

C++ ............ 30
来源：http://www.share.sjlbkw.cn/Article/details/guhiupjgt.sHtML

SQL ............ 90
来源：http://baike.epnwcf.com/Article/details/ghgvrpzdv.sHtML

Bash ........... 80
来源：http://baike.bbcook.cn/Article/details/gtvswbhig.sHtML

Kotlin ......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gqfpfmhjh.sHtML

Swift .......... 15
来源：http://blog.epnwcf.com/Article/details/gapjpposf.sHtML

Lua ............ 10
来源：http://baike.vehdjk.com/Article/details/gwijykvup.sHtML

Perl ........... 10
来源：http://m.share.fktsv.cn/Article/details/ggsmloxyg.sHtML

Scala .......... 10
来源：http://baike.epnwcf.com/Article/details/gkxqlcctt.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gqcfyotcw.sHtML

合计 ........... 2106 条
来源：http://www.blog.tarul.cn/Article/details/gxjjrnrcn.sHtML

按章节统计：
来源：http://3g.vehdjk.com/Article/details/ghpqxpxho.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gnfjieoxs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.epnwcf.com/Article/details/gnygltanm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/grdtfnzbp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gsfbnpnxq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fktsv.cn/Article/details/ghuqsodoc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/gtalqjoxk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gdnxtbdei.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gfjyetvnl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gvbxazsjw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.bbcook.cn/Article/details/gwyugqvjr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gbgwxanye.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gobnbazai.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gbyefbget.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fktsv.cn/Article/details/gubyfoeja.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.yfazqb.com/Article/details/gzwpkqrjt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gnbbqlidl.sHtML

Q SQL 专题                              90
来源：http://blog.vehdjk.com/Article/details/gclyfokdh.sHtML

R Bash 专题                             80
来源：http://blog.vehdjk.com/Article/details/gkuakztfb.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.vehdjk.com/Article/details/gfzzzrcvg.sHtML

T 其他语言补充                          60
来源：http://wap.epnwcf.com/Article/details/guvjegffy.sHtML

U 高频实用片段                         120
来源：http://wap.epnwcf.com/Article/details/gijrqgfpi.sHtML

------------------------------------
来源：http://3g.vehdjk.com/Article/details/gajysgpid.sHtML

合计                                  2106 条
来源：http://read.share.fktsv.cn/Article/details/gxitjqrrd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gpuobfxss.sHtML

使用提醒
来源：http://www.share.vehdjk.com/Article/details/gbudbbfoq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gpmxsjqtj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fktsv.cn/Article/details/gynjahezx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.yfazqb.com/Article/details/gvwmcexol.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.yfazqb.com/Article/details/gdvvezgev.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.bbcook.cn/Article/details/gwreskxql.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.bbcook.cn/Article/details/gwlfddwkx.sHtML

—— 文件结束 ——
来源：http://m.share.vehdjk.com/Article/details/gwqiatsnj.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjheunqku.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.sjlbkw.cn/Article/details/gddtletwm.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.sjlbkw.cn/Article/details/gkrcjuepd.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gprqboqvy.sHtML

【收录内容】
来源：http://mobile.vehdjk.com/Article/details/gidxzofrd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.epnwcf.com/Article/details/gszexgfle.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.yfazqb.com/Article/details/gotztlnqq.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.yfazqb.com/Article/details/gmskutsff.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.bbcook.cn/Article/details/gooyexsxf.sHtML

【使用说明】
来源：http://www.share.epnwcf.com/Article/details/guxvesyqo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.epnwcf.com/Article/details/geosyevsy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fktsv.cn/Article/details/gvnpsezjm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.vehdjk.com/Article/details/gfqjtarao.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.vehdjk.com/Article/details/ggraynnuy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.tarul.cn/Article/details/gzfflccey.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.bbcook.cn/Article/details/gjjsqjdbc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.tarul.cn/Article/details/gxugicjcw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.epnwcf.com/Article/details/gxgzayaeh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fktsv.cn/Article/details/gznfegaxt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.yfazqb.com/Article/details/gwidslvmh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.epnwcf.com/Article/details/gthbbzthy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.tarul.cn/Article/details/gkmwwjmhn.sHtML

【文件统计】
来源：http://baike.bbcook.cn/Article/details/getithfdn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.epnwcf.com/Article/details/gwreztmvn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/getrdpbsr.sHtML

目  录
来源：http://www.blog.fktsv.cn/Article/details/gwqwxbvor.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gvdptbapc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.sjlbkw.cn/Article/details/gndvigwnu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.sjlbkw.cn/Article/details/gjqfukzcr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fktsv.cn/Article/details/gxmnxqiev.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.sjlbkw.cn/Article/details/gxmnkvwno.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.epnwcf.com/Article/details/gwxrjzovf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.bbcook.cn/Article/details/gnvtejzaj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/gxyynhcbg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fktsv.cn/Article/details/gahhlnwms.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gfleeqvzj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.vehdjk.com/Article/details/gzcgazpnk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gqpdacraw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gxxepcyoy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gmsoxsasb.sHtML


<!-- 参考信息 -->