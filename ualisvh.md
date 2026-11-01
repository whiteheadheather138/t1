代发 wailian999

[U19] Py：正则替换带回调
来源：http://3g.vehdjk.com/Article/details/gbmlzfimk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.yfazqb.com/Article/details/givykcrzs.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.bbcook.cn/Article/details/gslbqgdmn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.tarul.cn/Article/details/gqyaluljh.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.epnwcf.com/Article/details/gimhkexiu.sHtML

@contextlib.contextmanager
来源：http://blog.tarul.cn/Article/details/gvcxgnadn.sHtML

[U22] Py：矩阵转置
来源：http://mobile.vehdjk.com/Article/details/gjwbxpvrv.sHtML

list(zip(*m))
来源：http://www.blog.vehdjk.com/Article/details/gfdpnrirf.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fktsv.cn/Article/details/gubaxiqhp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.epnwcf.com/Article/details/gnfoetgyp.sHtML

[U24] Py：路径操作
来源：http://blog.tarul.cn/Article/details/ggfxxfhzi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gqzwyjzqj.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.bbcook.cn/Article/details/gemcidmdg.sHtML

csv.DictReader(f)
来源：http://blog.sjlbkw.cn/Article/details/gznjpjmzj.sHtML

[U26] Py：并发下载
来源：http://wap.tarul.cn/Article/details/gjvgokrrk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.epnwcf.com/Article/details/gekfazwmi.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.yfazqb.com/Article/details/geyraxpmi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fktsv.cn/Article/details/gsmlrcare.sHtML

[U28] Py：类型别名
来源：http://www.blog.epnwcf.com/Article/details/gskrorivs.sHtML

UserId = int
来源：http://mobile.vehdjk.com/Article/details/gwitjtyup.sHtML

[U29] Py：属性校验
来源：http://www.blog.bbcook.cn/Article/details/gsluxwwtk.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.epnwcf.com/Article/details/geffkzghu.sHtML

[U30] Py：数据类
来源：http://blog.epnwcf.com/Article/details/gjejivofs.sHtML

@dataclass(slots=True)
来源：http://read.share.tarul.cn/Article/details/gfcpkifgx.sHtML

[U31] Py：单测
来源：http://www.m.share.yfazqb.com/Article/details/grdvffoif.sHtML

python -m pytest -q
来源：http://baike.yfazqb.com/Article/details/gaaixkcxx.sHtML

[U32] Py：代码格式化
来源：http://wap.yfazqb.com/Article/details/gdacnevec.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fktsv.cn/Article/details/gxovrxkyy.sHtML

[U33] Py：打包发布
来源：http://read.share.yfazqb.com/Article/details/goptmavhw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.yfazqb.com/Article/details/gfglcnoaw.sHtML

[U34] Py：判断编码
来源：http://baike.bbcook.cn/Article/details/gwbtsmqbw.sHtML

chardet.detect(raw)
来源：http://www.m.share.tarul.cn/Article/details/gfyjmkcgi.sHtML

[U35] Py：发送邮件
来源：http://wap.yfazqb.com/Article/details/gilrqusvt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.vehdjk.com/Article/details/ggdmchqov.sHtML

[U36] Py：定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gcsimrbej.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fktsv.cn/Article/details/guzwdoigo.sHtML

[U37] Py：读写 Excel
来源：http://m.share.tarul.cn/Article/details/gxrrwuiau.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.bbcook.cn/Article/details/ggejcavhv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fktsv.cn/Article/details/gotuusaos.sHtML

Path(__file__).resolve().parent
来源：http://www.share.bbcook.cn/Article/details/gwqidauhb.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.tarul.cn/Article/details/gjkgsfyxd.sHtML

sys.stdout.isatty()
来源：http://blog.bbcook.cn/Article/details/gsbbsfkvm.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.vehdjk.com/Article/details/gnrcgzxui.sHtML

print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/gwsxwohgj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.epnwcf.com/Article/details/gfjidqlei.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.epnwcf.com/Article/details/grsccasgw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.tarul.cn/Article/details/gflglrhiz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.epnwcf.com/Article/details/gwlfdpzgq.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.bbcook.cn/Article/details/gnaefeafc.sHtML

namespace App\Http;
来源：http://3g.yfazqb.com/Article/details/gkpnjkppv.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.tarul.cn/Article/details/gszdfhvvr.sHtML

declare(strict_types=1);
来源：http://www.blog.bbcook.cn/Article/details/gvafoyyyp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.yfazqb.com/Article/details/grwdaacda.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gwoqkvzll.sHtML

[U46] PHP：可空类型
来源：http://www.share.yfazqb.com/Article/details/ghpssrven.sHtML

?string $name = null
来源：http://read.share.sjlbkw.cn/Article/details/gvmlbobtv.sHtML

[U47] PHP：联合类型
来源：http://m.share.yfazqb.com/Article/details/gzhfxwjes.sHtML

int|string $id
来源：http://m.share.vehdjk.com/Article/details/gmzojjutt.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fktsv.cn/Article/details/gpcagfqdf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.sjlbkw.cn/Article/details/gzebrawwi.sHtML

[U49] PHP：只读属性
来源：http://wap.bbcook.cn/Article/details/gahueqdiv.sHtML

public readonly string $name
来源：http://mobile.sjlbkw.cn/Article/details/gvjdowzco.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.tarul.cn/Article/details/gchomszpe.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.tarul.cn/Article/details/gdbhbwthp.sHtML

[U51] PHP：数组解构
来源：http://blog.fktsv.cn/Article/details/ggbttenra.sHtML

[$a, $b] = $arr;
来源：http://3g.yfazqb.com/Article/details/gtrqinlcd.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gshqstric.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.vehdjk.com/Article/details/gbjbktfjt.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fktsv.cn/Article/details/gqcddjrwv.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.epnwcf.com/Article/details/gahypxoao.sHtML

[U54] PHP：空安全调用
来源：http://blog.epnwcf.com/Article/details/gkugvgjqk.sHtML

$obj?->method()
来源：http://wap.sjlbkw.cn/Article/details/gmxnmbsqh.sHtML

[U55] PHP：match 表达式
来源：http://baike.sjlbkw.cn/Article/details/gpiwqehff.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.yfazqb.com/Article/details/guhieqlhz.sHtML

[U56] PHP：命名参数
来源：http://blog.fktsv.cn/Article/details/gggdfrsdn.sHtML

f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gmohehyzx.sHtML

[U57] PHP：字符串插值
来源：http://wap.yfazqb.com/Article/details/gvyrtvzaz.sHtML

"值: {$a}"
来源：http://m.share.tarul.cn/Article/details/gthqpgpvj.sHtML

[U58] PHP：数组三件套
来源：http://read.share.bbcook.cn/Article/details/glmhzjieh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.yfazqb.com/Article/details/gjqtdhraw.sHtML

[U59] PHP：自定义排序
来源：http://read.share.vehdjk.com/Article/details/grzjrsrjm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gkvuegfil.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.sjlbkw.cn/Article/details/gxejyjtpq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.sjlbkw.cn/Article/details/gmzjulwyh.sHtML

[U61] PHP：正则
来源：http://blog.tarul.cn/Article/details/gkcfupbqy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gndqifmzh.sHtML

[U62] PHP：日期对象
来源：http://mobile.fktsv.cn/Article/details/gfjrqlvmq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/gevketrrj.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.bbcook.cn/Article/details/glacdskcu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.yfazqb.com/Article/details/gfzvoczcb.sHtML

[U64] PHP：目录遍历
来源：http://3g.tarul.cn/Article/details/gxzmvpmoe.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.epnwcf.com/Article/details/grradtawi.sHtML

[U65] PHP：会话
来源：http://www.share.tarul.cn/Article/details/gcvqpafpk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gohwrcgxl.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.bbcook.cn/Article/details/gykrrxzjo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fktsv.cn/Article/details/gfmxplwyb.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.tarul.cn/Article/details/gqgpwfljo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.sjlbkw.cn/Article/details/gtoulgacp.sHtML

[U68] PHP：PDO 连接
来源：http://wap.tarul.cn/Article/details/gfafscded.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.sjlbkw.cn/Article/details/gppdmxlho.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.tarul.cn/Article/details/gwnjxnath.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.tarul.cn/Article/details/gtwqycrwz.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.yfazqb.com/Article/details/gqnfyghkc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.tarul.cn/Article/details/gpxrghjyp.sHtML

[U71] PHP：抛出异常
来源：http://baike.yfazqb.com/Article/details/gskzoisby.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.yfazqb.com/Article/details/gyznwcfki.sHtML

[U72] PHP：写错误日志
来源：http://baike.epnwcf.com/Article/details/ghtfcolhh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.bbcook.cn/Article/details/gvdlscwzg.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fktsv.cn/Article/details/gfhotygmz.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.epnwcf.com/Article/details/gnqyjtxpr.sHtML

[U74] PHP：读取环境变量
来源：http://3g.epnwcf.com/Article/details/gxfwtsfer.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.sjlbkw.cn/Article/details/gdpnlybld.sHtML

[U75] PHP：依赖注入
来源：http://blog.bbcook.cn/Article/details/gmqxdsihb.sHtML

composer require psr/container
来源：http://wap.epnwcf.com/Article/details/gzyhuwzvb.sHtML

[U76] PHP：简单路由
来源：http://read.share.tarul.cn/Article/details/gpkovpahu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.bbcook.cn/Article/details/ghooyyrps.sHtML

[U77] PHP：模板渲染
来源：http://baike.fktsv.cn/Article/details/gprsebtny.sHtML

composer require twig/twig
来源：http://www.blog.sjlbkw.cn/Article/details/ggppixnix.sHtML

[U78] PHP：单元测试
来源：http://3g.tarul.cn/Article/details/gcqjaexnt.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsdwdqcj.sHtML

[U79] PHP：静态分析
来源：http://www.share.vehdjk.com/Article/details/gotmsowdy.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.vehdjk.com/Article/details/gcnltbxra.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.epnwcf.com/Article/details/glyclyqph.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.yfazqb.com/Article/details/gsxadicdk.sHtML

[U81] JS：初始化项目
来源：http://read.share.yfazqb.com/Article/details/gtgftnfli.sHtML

npm init -y;  npm i express
来源：http://wap.fktsv.cn/Article/details/ggfyhqpjp.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.yfazqb.com/Article/details/gpxxnazmt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.vehdjk.com/Article/details/gruwlspty.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.tarul.cn/Article/details/grbmoeenc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/gkoqtbhph.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.bbcook.cn/Article/details/gkurzxjro.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.epnwcf.com/Article/details/gjknaxpmu.sHtML

[U85] JS：可选链
来源：http://wap.vehdjk.com/Article/details/glnchscyx.sHtML

a?.b?.c
来源：http://m.share.yfazqb.com/Article/details/geworbvgf.sHtML

[U86] JS：空值合并
来源：http://www.blog.vehdjk.com/Article/details/gsdvwqzeo.sHtML

a ?? b
来源：http://mobile.yfazqb.com/Article/details/gfrdgpiwv.sHtML

[U87] JS：解构默认值
来源：http://3g.epnwcf.com/Article/details/gxfofqram.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.epnwcf.com/Article/details/gkwadkchq.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.vehdjk.com/Article/details/gcrqpywuz.sHtML

{ ...a, ...b }
来源：http://wap.fktsv.cn/Article/details/gbgtroxfx.sHtML

[U89] JS：数组去重
来源：http://baike.sjlbkw.cn/Article/details/giwiziypf.sHtML

[...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gccjnvrbd.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.vehdjk.com/Article/details/giquiafym.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gsybczjjh.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.yfazqb.com/Article/details/gphbnpewi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.yfazqb.com/Article/details/gnxkpqkjw.sHtML

[U92] JS：深拷贝
来源：http://www.blog.yfazqb.com/Article/details/gkroomflr.sHtML

structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gxivdtkbu.sHtML

[U93] JS：模板字符串
来源：http://www.share.yfazqb.com/Article/details/gktxrkmgp.sHtML

`共 ${n} 条`
来源：http://www.m.share.bbcook.cn/Article/details/ggantukgb.sHtML

[U94] JS：箭头函数
来源：http://m.share.tarul.cn/Article/details/gcgqgkbvr.sHtML

const double = x => x * 2;
来源：http://baike.yfazqb.com/Article/details/gmsabrtcd.sHtML

[U95] JS：Promise 包装
来源：http://blog.vehdjk.com/Article/details/gboxqkpqq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.vehdjk.com/Article/details/goclouhib.sHtML

[U96] JS：async/await 与异常
来源：http://wap.sjlbkw.cn/Article/details/gapddqwam.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gihcvwuoj.sHtML

[U97] JS：并发请求
来源：http://read.share.vehdjk.com/Article/details/gsbkcqbnf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/grnovpwps.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.vehdjk.com/Article/details/glxrvkzvy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fktsv.cn/Article/details/gnppnzjvv.sHtML

[U99] JS：事件监听
来源：http://m.share.fktsv.cn/Article/details/gbxvqhdht.sHtML

el.addEventListener("click", e => {})
来源：http://3g.sjlbkw.cn/Article/details/gbubbvoia.sHtML

[U100] JS：DOM 查询
来源：http://m.share.epnwcf.com/Article/details/gcblasibr.sHtML

document.querySelector(".item")
来源：http://read.share.yfazqb.com/Article/details/gwlyvdeir.sHtML

[U101] JS：classList 操作
来源：http://read.share.sjlbkw.cn/Article/details/gnttsijtv.sHtML

el.classList.toggle("active")
来源：http://www.blog.fktsv.cn/Article/details/gwdlxpffw.sHtML

[U102] JS：本地存储
来源：http://baike.yfazqb.com/Article/details/gjvfepvhu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.tarul.cn/Article/details/gojiojezx.sHtML

[U103] JS：定时器
来源：http://www.share.yfazqb.com/Article/details/ggrquzbnp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fktsv.cn/Article/details/gwurcfcpy.sHtML

[U104] JS：防抖
来源：http://mobile.epnwcf.com/Article/details/gopxykdqg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gcxqzarer.sHtML

[U105] JS：节流
来源：http://www.blog.fktsv.cn/Article/details/gkxaxmjsm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.bbcook.cn/Article/details/gkhmfymbg.sHtML

[U106] JS：日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gepnfplno.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.sjlbkw.cn/Article/details/gtgniomva.sHtML

[U107] JS：数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gstakyxkb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.epnwcf.com/Article/details/gnayjmuff.sHtML

[U108] JS：随机整数
来源：http://3g.epnwcf.com/Article/details/gtmcephvj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fktsv.cn/Article/details/geuecxrwu.sHtML

[U109] JS：数组分组
来源：http://blog.epnwcf.com/Article/details/gsxfzryjr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/gwcxpapdz.sHtML

[U110] JS：数组分块
来源：http://blog.tarul.cn/Article/details/gptxeedek.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.epnwcf.com/Article/details/gopollifn.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gyiauerql.sHtML

new Map(Object.entries(obj))
来源：http://3g.yfazqb.com/Article/details/ghbegjazf.sHtML

[U112] JS：字符串补位
来源：http://blog.vehdjk.com/Article/details/gyxvzzdyl.sHtML

"7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gvzjzwjcb.sHtML

[U113] JS：正则替换全部
来源：http://m.share.vehdjk.com/Article/details/gdpgovmzx.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/grenwhjxo.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.yfazqb.com/Article/details/gbobmhxin.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gdxlvvcni.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.sjlbkw.cn/Article/details/gwjejuuqz.sHtML

crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gngulgqky.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.tarul.cn/Article/details/galhubluj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwyezhqqf.sHtML

[U117] JS：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gfqtefynx.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.yfazqb.com/Article/details/gvfpgoxjj.sHtML

[U118] JS：开发服务器
来源：http://baike.bbcook.cn/Article/details/goqqskeuv.sHtML

npm i -D vite;  npx vite
来源：http://wap.fktsv.cn/Article/details/ggnmjxrec.sHtML

[U119] JS：生产构建
来源：http://www.blog.epnwcf.com/Article/details/gjvxthmni.sHtML

npx vite build
来源：http://www.m.share.vehdjk.com/Article/details/ggkydervf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.vehdjk.com/Article/details/gmgaanmlt.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.vehdjk.com/Article/details/gjwkdcwuz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gyitwappf.sHtML

统计汇总
来源：http://www.share.tarul.cn/Article/details/gzencxtkf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzcrxekys.sHtML

按语言统计（条）：
来源：http://m.share.epnwcf.com/Article/details/gdplrmqib.sHtML

Python ......... 252
来源：http://m.share.epnwcf.com/Article/details/gtuiknrau.sHtML

PHP ............ 252
来源：http://blog.yfazqb.com/Article/details/gdmaaypxl.sHtML

JavaScript ..... 252
来源：http://www.share.tarul.cn/Article/details/gtypgdbpy.sHtML

TypeScript ..... 212
来源：http://wap.epnwcf.com/Article/details/giqwtsnnc.sHtML

Java ........... 212
来源：http://baike.tarul.cn/Article/details/gticgrbys.sHtML

Go ............. 212
来源：http://read.share.tarul.cn/Article/details/gxoafpiqm.sHtML

Ruby ........... 212
来源：http://wap.fktsv.cn/Article/details/gmaybxfgg.sHtML

C# ............. 212
来源：http://m.share.yfazqb.com/Article/details/gaefenpva.sHtML

C .............. 30
来源：http://m.share.vehdjk.com/Article/details/gdaynqqao.sHtML

C++ ............ 30
来源：http://m.share.fktsv.cn/Article/details/gfryvslhh.sHtML

SQL ............ 90
来源：http://www.m.share.tarul.cn/Article/details/gaauibvtb.sHtML

Bash ........... 80
来源：http://read.share.bbcook.cn/Article/details/gifqdqdte.sHtML

Kotlin ......... 15
来源：http://mobile.fktsv.cn/Article/details/gikkpqrtu.sHtML

Swift .......... 15
来源：http://www.m.share.epnwcf.com/Article/details/gubnlxhtx.sHtML

Lua ............ 10
来源：http://baike.epnwcf.com/Article/details/gxvztztwv.sHtML

Perl ........... 10
来源：http://www.m.share.epnwcf.com/Article/details/ghzwvhfwv.sHtML

Scala .......... 10
来源：http://www.m.share.tarul.cn/Article/details/gfbutibpe.sHtML

------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gucpclcfg.sHtML

合计 ........... 2106 条
来源：http://www.share.bbcook.cn/Article/details/gaqivjbso.sHtML

按章节统计：
来源：http://3g.epnwcf.com/Article/details/ghawlblwn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gfzyfrihy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/gohwrjzoh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.epnwcf.com/Article/details/gouvlvjam.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gqdjwospd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.epnwcf.com/Article/details/goylkjykt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.tarul.cn/Article/details/gvfurlofd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.vehdjk.com/Article/details/geawwzmfe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.tarul.cn/Article/details/gsjmcqvev.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gydomvwyt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.tarul.cn/Article/details/gnjjczphv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gccncpois.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gijdsjwtl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/golnrxnlb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fktsv.cn/Article/details/gzuleadep.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.tarul.cn/Article/details/ghdrfhycu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gmxszagke.sHtML

Q SQL 专题                              90
来源：http://www.blog.sjlbkw.cn/Article/details/gaamslshu.sHtML

R Bash 专题                             80
来源：http://m.share.bbcook.cn/Article/details/gtyqembca.sHtML

S C / C++ 专题                          60
来源：http://www.share.epnwcf.com/Article/details/gbrncunjd.sHtML

T 其他语言补充                          60
来源：http://baike.fktsv.cn/Article/details/gnkzabwic.sHtML

U 高频实用片段                         120
来源：http://blog.bbcook.cn/Article/details/gxxlnjhzu.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gxoxgaryi.sHtML

合计                                  2106 条
来源：http://m.share.sjlbkw.cn/Article/details/gquddletw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gvstgtgzj.sHtML

使用提醒
来源：http://wap.sjlbkw.cn/Article/details/ghdspbykr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/grzpownxr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.bbcook.cn/Article/details/gqdpkgdyr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.epnwcf.com/Article/details/guamicewm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.epnwcf.com/Article/details/gadokneet.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.vehdjk.com/Article/details/gdihzdqvb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.bbcook.cn/Article/details/gqbdufsgk.sHtML

—— 文件结束 ——
来源：http://baike.fktsv.cn/Article/details/gvcowlxvy.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvfyxnowd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fktsv.cn/Article/details/gpgbhrmdz.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.yfazqb.com/Article/details/gytdmmhco.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwejtbsim.sHtML

【收录内容】
来源：http://www.share.epnwcf.com/Article/details/gproepzux.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.sjlbkw.cn/Article/details/gbdpjszrh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.yfazqb.com/Article/details/gwgiulbze.sHtML

SQL · Bash · C · C++
来源：http://mobile.sjlbkw.cn/Article/details/gvxzohhwv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.bbcook.cn/Article/details/gvqvufzix.sHtML

【使用说明】
来源：http://www.m.share.epnwcf.com/Article/details/gtxkikvem.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.tarul.cn/Article/details/ggappdzay.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.sjlbkw.cn/Article/details/glgcmspxu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.bbcook.cn/Article/details/gyqqidzdx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fktsv.cn/Article/details/goghbrnvb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.sjlbkw.cn/Article/details/gtypjfecw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fktsv.cn/Article/details/gbkmmvrzy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.yfazqb.com/Article/details/gzltdnmxp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fktsv.cn/Article/details/gyvvvzsde.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.sjlbkw.cn/Article/details/gyfhxvman.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fktsv.cn/Article/details/gmipnomtr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.epnwcf.com/Article/details/gzsmfvdzf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.tarul.cn/Article/details/gwlmqtaqe.sHtML

【文件统计】
来源：http://blog.tarul.cn/Article/details/gzbxvyzlb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fktsv.cn/Article/details/gfnwijxib.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gzjrtfafn.sHtML

目  录
来源：http://www.m.share.epnwcf.com/Article/details/gegifjqkt.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gbsclqlme.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fktsv.cn/Article/details/gfwavdwlu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.bbcook.cn/Article/details/gfhglbbtj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.epnwcf.com/Article/details/gbrpptndy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.epnwcf.com/Article/details/ghlmqigft.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.yfazqb.com/Article/details/gmxvzwwlo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.epnwcf.com/Article/details/gfrppqwls.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/gjyhqpbcm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.sjlbkw.cn/Article/details/gyvcceoaf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gpdnimrzl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gshrwctdg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gazcutusq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gcdxvoxkw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/ggwahzvvi.sHtML


<!-- 参考信息 -->