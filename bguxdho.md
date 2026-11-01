代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.blog.sjlbkw.cn/Article/details/gbwxryzhe.sHtML

@contextlib.contextmanager
来源：http://www.blog.bbcook.cn/Article/details/ghvqaulnd.sHtML

[U22] Py：矩阵转置
来源：http://mobile.sjlbkw.cn/Article/details/gizowzkcb.sHtML

list(zip(*m))
来源：http://www.share.sjlbkw.cn/Article/details/gqvxztksk.sHtML

[U23] Py：分块读取大文件
来源：http://blog.vehdjk.com/Article/details/ggmdhpqyz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fktsv.cn/Article/details/ggbnwwijb.sHtML

[U24] Py：路径操作
来源：http://www.blog.epnwcf.com/Article/details/gktktmisp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fktsv.cn/Article/details/gcxhdouph.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.bbcook.cn/Article/details/guypilaup.sHtML

csv.DictReader(f)
来源：http://www.m.share.vehdjk.com/Article/details/gqetcirta.sHtML

[U26] Py：并发下载
来源：http://3g.vehdjk.com/Article/details/gviuerujx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.vehdjk.com/Article/details/ghmffsfnk.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.yfazqb.com/Article/details/gtcyydfqm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.vehdjk.com/Article/details/gbmzdfsuj.sHtML

[U28] Py：类型别名
来源：http://baike.vehdjk.com/Article/details/gbysaacpl.sHtML

UserId = int
来源：http://mobile.vehdjk.com/Article/details/gxocyainz.sHtML

[U29] Py：属性校验
来源：http://blog.yfazqb.com/Article/details/ghswnegkx.sHtML

@property 与 @x.setter 配合
来源：http://read.share.tarul.cn/Article/details/gxcjaehuh.sHtML

[U30] Py：数据类
来源：http://blog.vehdjk.com/Article/details/ghdvthlaj.sHtML

@dataclass(slots=True)
来源：http://wap.bbcook.cn/Article/details/gowhjdtwy.sHtML

[U31] Py：单测
来源：http://www.m.share.tarul.cn/Article/details/gbicpydqc.sHtML

python -m pytest -q
来源：http://read.share.tarul.cn/Article/details/gpknaimxx.sHtML

[U32] Py：代码格式化
来源：http://blog.bbcook.cn/Article/details/giawudwrn.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.tarul.cn/Article/details/gdmorknhd.sHtML

[U33] Py：打包发布
来源：http://wap.yfazqb.com/Article/details/grxsdqrva.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.sjlbkw.cn/Article/details/gqszavoim.sHtML

[U34] Py：判断编码
来源：http://3g.yfazqb.com/Article/details/gqmkhgefk.sHtML

chardet.detect(raw)
来源：http://www.m.share.yfazqb.com/Article/details/gjrhgwota.sHtML

[U35] Py：发送邮件
来源：http://3g.sjlbkw.cn/Article/details/gmyuzhjhy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.sjlbkw.cn/Article/details/gvxcsiwax.sHtML

[U36] Py：定时任务
来源：http://blog.vehdjk.com/Article/details/gqgiyenwz.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fktsv.cn/Article/details/gahkjjaya.sHtML

[U37] Py：读写 Excel
来源：http://wap.yfazqb.com/Article/details/gtrjmyqht.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.sjlbkw.cn/Article/details/gdqddtazh.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.epnwcf.com/Article/details/gnflyxcfc.sHtML

Path(__file__).resolve().parent
来源：http://baike.bbcook.cn/Article/details/glozvekqq.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.vehdjk.com/Article/details/goezxmcwe.sHtML

sys.stdout.isatty()
来源：http://www.m.share.vehdjk.com/Article/details/gwvvgdvxw.sHtML

[U40] Py：打印到标准错误
来源：http://wap.vehdjk.com/Article/details/gqcwzjtmy.sHtML

print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gdpknxhks.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.bbcook.cn/Article/details/guttcyqau.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fktsv.cn/Article/details/gflaurcsi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.bbcook.cn/Article/details/glqvxamlu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.epnwcf.com/Article/details/geekjkzwq.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gnobjyffw.sHtML

namespace App\Http;
来源：http://m.share.yfazqb.com/Article/details/gzntcgflo.sHtML

[U44] PHP：开启严格类型
来源：http://baike.tarul.cn/Article/details/goknpzact.sHtML

declare(strict_types=1);
来源：http://www.share.tarul.cn/Article/details/gkwillazt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.epnwcf.com/Article/details/gnphittwz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gorerxlgz.sHtML

[U46] PHP：可空类型
来源：http://www.blog.sjlbkw.cn/Article/details/gscsfizwu.sHtML

?string $name = null
来源：http://www.blog.sjlbkw.cn/Article/details/galrexpet.sHtML

[U47] PHP：联合类型
来源：http://wap.bbcook.cn/Article/details/goedyswwo.sHtML

int|string $id
来源：http://read.share.fktsv.cn/Article/details/gnodmvqyk.sHtML

[U48] PHP：纯枚举
来源：http://baike.yfazqb.com/Article/details/gawdgffvy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.tarul.cn/Article/details/gndaiprop.sHtML

[U49] PHP：只读属性
来源：http://mobile.tarul.cn/Article/details/gbfpcfwqe.sHtML

public readonly string $name
来源：http://blog.fktsv.cn/Article/details/ggtrdfwma.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.yfazqb.com/Article/details/glmjmtmpk.sHtML

public function __construct(private int $id) {}
来源：http://wap.vehdjk.com/Article/details/gmjykztns.sHtML

[U51] PHP：数组解构
来源：http://baike.fktsv.cn/Article/details/ggguhfyle.sHtML

[$a, $b] = $arr;
来源：http://www.share.tarul.cn/Article/details/gnyxioetc.sHtML

[U52] PHP：箭头函数
来源：http://3g.fktsv.cn/Article/details/gvbffxhth.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.vehdjk.com/Article/details/gqicsedtw.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fktsv.cn/Article/details/gfxqlaoxw.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.epnwcf.com/Article/details/gcjqsovit.sHtML

[U54] PHP：空安全调用
来源：http://wap.epnwcf.com/Article/details/guffwbyzm.sHtML

$obj?->method()
来源：http://www.m.share.yfazqb.com/Article/details/ghopcqiak.sHtML

[U55] PHP：match 表达式
来源：http://mobile.tarul.cn/Article/details/gnhlxyjoj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.sjlbkw.cn/Article/details/ggmurlbeo.sHtML

[U56] PHP：命名参数
来源：http://www.blog.yfazqb.com/Article/details/gbycpmkxd.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gkfjdwwpo.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gwbsmkkwi.sHtML

"值: {$a}"
来源：http://blog.fktsv.cn/Article/details/gjaoqvllo.sHtML

[U58] PHP：数组三件套
来源：http://blog.fktsv.cn/Article/details/glnsyoyot.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.bbcook.cn/Article/details/gudmltqab.sHtML

[U59] PHP：自定义排序
来源：http://mobile.tarul.cn/Article/details/gtivqfkwa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fktsv.cn/Article/details/gsbwgmkqc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.bbcook.cn/Article/details/gptyeddgl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.bbcook.cn/Article/details/gkfialwwy.sHtML

[U61] PHP：正则
来源：http://www.share.epnwcf.com/Article/details/gcozygjgj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gmbyhfwcl.sHtML

[U62] PHP：日期对象
来源：http://www.blog.yfazqb.com/Article/details/goufazdyx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzphqora.sHtML

[U63] PHP：文件读写
来源：http://baike.fktsv.cn/Article/details/gnbuubbth.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.bbcook.cn/Article/details/gxhhobllp.sHtML

[U64] PHP：目录遍历
来源：http://mobile.yfazqb.com/Article/details/gllkcpghx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.yfazqb.com/Article/details/gohrhxqwp.sHtML

[U65] PHP：会话
来源：http://wap.sjlbkw.cn/Article/details/gtmzjjxav.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.yfazqb.com/Article/details/gpdwbplrm.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.yfazqb.com/Article/details/gujyawlxi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.tarul.cn/Article/details/glkxmszly.sHtML

[U67] PHP：处理文件上传
来源：http://blog.vehdjk.com/Article/details/gpxmgcoau.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.yfazqb.com/Article/details/goxpqnbpr.sHtML

[U68] PHP：PDO 连接
来源：http://baike.yfazqb.com/Article/details/giodolyzc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fktsv.cn/Article/details/gbymffvxm.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.bbcook.cn/Article/details/gnfqdzdis.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.epnwcf.com/Article/details/gheouugcz.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.vehdjk.com/Article/details/gpacukojm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.sjlbkw.cn/Article/details/godwzmlxk.sHtML

[U71] PHP：抛出异常
来源：http://www.share.tarul.cn/Article/details/gyjuqousa.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.bbcook.cn/Article/details/gnbcplnwr.sHtML

[U72] PHP：写错误日志
来源：http://baike.epnwcf.com/Article/details/grbuunrlg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fktsv.cn/Article/details/gubdepqde.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.bbcook.cn/Article/details/ghikqliql.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.vehdjk.com/Article/details/gjsyhoyzs.sHtML

[U74] PHP：读取环境变量
来源：http://blog.epnwcf.com/Article/details/gxakiosyn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.vehdjk.com/Article/details/ggaatglxd.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.vehdjk.com/Article/details/giagbfpnc.sHtML

composer require psr/container
来源：http://baike.fktsv.cn/Article/details/gwnnrelfx.sHtML

[U76] PHP：简单路由
来源：http://baike.bbcook.cn/Article/details/gwhosqrnb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.yfazqb.com/Article/details/gpktiqpwb.sHtML

[U77] PHP：模板渲染
来源：http://baike.sjlbkw.cn/Article/details/gxcjofdum.sHtML

composer require twig/twig
来源：http://read.share.bbcook.cn/Article/details/gplbkpdgk.sHtML

[U78] PHP：单元测试
来源：http://baike.tarul.cn/Article/details/gbxoawdcv.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.yfazqb.com/Article/details/guqspeuvm.sHtML

[U79] PHP：静态分析
来源：http://www.blog.sjlbkw.cn/Article/details/gsbrpfruj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.vehdjk.com/Article/details/glyyelvkb.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.bbcook.cn/Article/details/gkoifoofk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.epnwcf.com/Article/details/gzwucpkfh.sHtML

[U81] JS：初始化项目
来源：http://blog.epnwcf.com/Article/details/ghxadrrvg.sHtML

npm init -y;  npm i express
来源：http://baike.fktsv.cn/Article/details/gffyafpdn.sHtML

[U82] JS：package.json 脚本
来源：http://wap.sjlbkw.cn/Article/details/gpwnhkrkn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.bbcook.cn/Article/details/gkxyzquos.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.epnwcf.com/Article/details/gntemmqgy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.epnwcf.com/Article/details/greoxeoty.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.epnwcf.com/Article/details/gxnryomba.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.sjlbkw.cn/Article/details/gegypobnd.sHtML

[U85] JS：可选链
来源：http://www.m.share.sjlbkw.cn/Article/details/gplfuyvcr.sHtML

a?.b?.c
来源：http://wap.bbcook.cn/Article/details/gyvwlhrjo.sHtML

[U86] JS：空值合并
来源：http://read.share.epnwcf.com/Article/details/giyhrxfzb.sHtML

a ?? b
来源：http://blog.fktsv.cn/Article/details/gpkletnts.sHtML

[U87] JS：解构默认值
来源：http://3g.yfazqb.com/Article/details/gpnkpunsv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.yfazqb.com/Article/details/gulitfykz.sHtML

[U88] JS：对象展开合并
来源：http://www.share.sjlbkw.cn/Article/details/gtidingss.sHtML

{ ...a, ...b }
来源：http://blog.tarul.cn/Article/details/gqjzgqdhy.sHtML

[U89] JS：数组去重
来源：http://wap.vehdjk.com/Article/details/ghnvxsypv.sHtML

[...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gsawwovfu.sHtML

[U90] JS：数字数组排序
来源：http://wap.sjlbkw.cn/Article/details/gcrszczky.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gzdpyuakk.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.bbcook.cn/Article/details/gizfymjhs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.bbcook.cn/Article/details/gymknqbtd.sHtML

[U92] JS：深拷贝
来源：http://www.share.vehdjk.com/Article/details/gtqrjorhn.sHtML

structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gantnlsma.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gucttwboa.sHtML

`共 ${n} 条`
来源：http://www.m.share.sjlbkw.cn/Article/details/gwregjjet.sHtML

[U94] JS：箭头函数
来源：http://m.share.tarul.cn/Article/details/gnqtllttp.sHtML

const double = x => x * 2;
来源：http://mobile.epnwcf.com/Article/details/gdhaazqts.sHtML

[U95] JS：Promise 包装
来源：http://m.share.tarul.cn/Article/details/gzqfasooa.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.sjlbkw.cn/Article/details/ggkgutahh.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fktsv.cn/Article/details/gjnbwtgjp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gpzeoyytm.sHtML

[U97] JS：并发请求
来源：http://mobile.vehdjk.com/Article/details/gutarroiw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gnrihzpun.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.vehdjk.com/Article/details/gdsxjbuzf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.tarul.cn/Article/details/gzguhtkjs.sHtML

[U99] JS：事件监听
来源：http://read.share.vehdjk.com/Article/details/gaseyblgd.sHtML

el.addEventListener("click", e => {})
来源：http://blog.tarul.cn/Article/details/gdranlkyo.sHtML

[U100] JS：DOM 查询
来源：http://wap.epnwcf.com/Article/details/ghwvvdfag.sHtML

document.querySelector(".item")
来源：http://mobile.sjlbkw.cn/Article/details/gihbbyfzm.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.yfazqb.com/Article/details/gytczjefm.sHtML

el.classList.toggle("active")
来源：http://baike.bbcook.cn/Article/details/gvbfnrsuv.sHtML

[U102] JS：本地存储
来源：http://www.share.bbcook.cn/Article/details/gbqmevbcs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.vehdjk.com/Article/details/gmdgrdyta.sHtML

[U103] JS：定时器
来源：http://3g.bbcook.cn/Article/details/gtrzjjxcs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.sjlbkw.cn/Article/details/gumabwmae.sHtML

[U104] JS：防抖
来源：http://mobile.bbcook.cn/Article/details/gufuvwtgg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gxvygedya.sHtML

[U105] JS：节流
来源：http://blog.bbcook.cn/Article/details/guiuqltty.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.yfazqb.com/Article/details/glzrfyxmp.sHtML

[U106] JS：日期格式化
来源：http://baike.sjlbkw.cn/Article/details/glpyiuyxb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.epnwcf.com/Article/details/ghiiypjtu.sHtML

[U107] JS：数字千分位
来源：http://blog.fktsv.cn/Article/details/gonsejumh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gjcywlmph.sHtML

[U108] JS：随机整数
来源：http://read.share.yfazqb.com/Article/details/ghamhvaqc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.tarul.cn/Article/details/guacqsriu.sHtML

[U109] JS：数组分组
来源：http://mobile.yfazqb.com/Article/details/gmggbkhyn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gpgsnzdja.sHtML

[U110] JS：数组分块
来源：http://blog.tarul.cn/Article/details/gxiuensje.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.tarul.cn/Article/details/gfqaohlnn.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fktsv.cn/Article/details/gpjglztyp.sHtML

new Map(Object.entries(obj))
来源：http://read.share.tarul.cn/Article/details/ghaejehis.sHtML

[U112] JS：字符串补位
来源：http://wap.vehdjk.com/Article/details/gczmnkfnh.sHtML

"7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gckxfevdm.sHtML

[U113] JS：正则替换全部
来源：http://m.share.sjlbkw.cn/Article/details/ghowaewkt.sHtML

s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gnhhsmyud.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.yfazqb.com/Article/details/gltyddxax.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gjlatnovi.sHtML

[U115] JS：生成 UUID
来源：http://blog.yfazqb.com/Article/details/gvjftscyb.sHtML

crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gvxhghija.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.sjlbkw.cn/Article/details/gwdecihov.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.vehdjk.com/Article/details/ghcfnlakl.sHtML

[U117] JS：单元测试
来源：http://m.share.epnwcf.com/Article/details/gyclxoqdk.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fktsv.cn/Article/details/gsktiphuk.sHtML

[U118] JS：开发服务器
来源：http://3g.fktsv.cn/Article/details/gbxpfuxgg.sHtML

npm i -D vite;  npx vite
来源：http://m.share.epnwcf.com/Article/details/geimmplkm.sHtML

[U119] JS：生产构建
来源：http://wap.vehdjk.com/Article/details/gnadjjvjy.sHtML

npx vite build
来源：http://blog.vehdjk.com/Article/details/gvbjpwjdb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.tarul.cn/Article/details/gmukylzfd.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.epnwcf.com/Article/details/gbsmdaske.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzgildmma.sHtML

统计汇总
来源：http://3g.bbcook.cn/Article/details/gebhmyezm.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/geprgsrvt.sHtML

按语言统计（条）：
来源：http://baike.tarul.cn/Article/details/gpmqdrjdw.sHtML

Python ......... 252
来源：http://wap.vehdjk.com/Article/details/gsrixhoek.sHtML

PHP ............ 252
来源：http://3g.yfazqb.com/Article/details/gwtcddnhx.sHtML

JavaScript ..... 252
来源：http://mobile.epnwcf.com/Article/details/gotjofxlx.sHtML

TypeScript ..... 212
来源：http://wap.epnwcf.com/Article/details/grosraiaf.sHtML

Java ........... 212
来源：http://www.m.share.epnwcf.com/Article/details/gixmxdmuq.sHtML

Go ............. 212
来源：http://m.share.vehdjk.com/Article/details/gweijplwn.sHtML

Ruby ........... 212
来源：http://www.blog.bbcook.cn/Article/details/ghulqniou.sHtML

C# ............. 212
来源：http://m.share.epnwcf.com/Article/details/gstvpnbtq.sHtML

C .............. 30
来源：http://mobile.yfazqb.com/Article/details/giyqlqgys.sHtML

C++ ............ 30
来源：http://baike.sjlbkw.cn/Article/details/gcyviipgs.sHtML

SQL ............ 90
来源：http://www.share.sjlbkw.cn/Article/details/gqvlpicck.sHtML

Bash ........... 80
来源：http://www.m.share.fktsv.cn/Article/details/ghqxjdiej.sHtML

Kotlin ......... 15
来源：http://baike.tarul.cn/Article/details/gcjfatyil.sHtML

Swift .......... 15
来源：http://mobile.fktsv.cn/Article/details/gzpvypxsq.sHtML

Lua ............ 10
来源：http://m.share.bbcook.cn/Article/details/gdfgdyzrh.sHtML

Perl ........... 10
来源：http://3g.sjlbkw.cn/Article/details/gijolpger.sHtML

Scala .......... 10
来源：http://blog.vehdjk.com/Article/details/gmjtpqfry.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gdjopopfp.sHtML

合计 ........... 2106 条
来源：http://blog.tarul.cn/Article/details/gvagczyun.sHtML

按章节统计：
来源：http://www.share.epnwcf.com/Article/details/gnkaorsme.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.vehdjk.com/Article/details/ggeigimgz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gxripqxfx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/gouykdxmg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gjbbehqwy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.epnwcf.com/Article/details/gahdlydjd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.epnwcf.com/Article/details/gdpvmbugl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/gczigkxzv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.bbcook.cn/Article/details/gwmlvmemn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/grllawjzy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/gfabbacjh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gwkzdehtk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gzpidyxnn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gggreqqoq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/gkkgpkfgd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.epnwcf.com/Article/details/guupajhzz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gxbcjfxsc.sHtML

Q SQL 专题                              90
来源：http://read.share.tarul.cn/Article/details/gxjvgafpz.sHtML

R Bash 专题                             80
来源：http://wap.yfazqb.com/Article/details/gcbrwmwho.sHtML

S C / C++ 专题                          60
来源：http://blog.vehdjk.com/Article/details/gvopimsse.sHtML

T 其他语言补充                          60
来源：http://blog.sjlbkw.cn/Article/details/ghdhyqaki.sHtML

U 高频实用片段                         120
来源：http://blog.bbcook.cn/Article/details/gwqqbxxka.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gvnwofysf.sHtML

合计                                  2106 条
来源：http://3g.vehdjk.com/Article/details/glqxiiwai.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gkdzjwkcj.sHtML

使用提醒
来源：http://www.m.share.bbcook.cn/Article/details/gpggantac.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gwkvkmwqb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.bbcook.cn/Article/details/gxersqgmr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fktsv.cn/Article/details/gbnxfgqjw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.vehdjk.com/Article/details/gwyrqgqmt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.epnwcf.com/Article/details/gmaergrpi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fktsv.cn/Article/details/giqaqojjf.sHtML

—— 文件结束 ——
来源：http://wap.tarul.cn/Article/details/gouipttki.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxcykmhqw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.bbcook.cn/Article/details/gdycgufmi.sHtML

Common Programming Examples Cheat Book
来源：http://baike.epnwcf.com/Article/details/gswtoarbx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/geczqxpin.sHtML

【收录内容】
来源：http://baike.sjlbkw.cn/Article/details/gqkruhevu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.yfazqb.com/Article/details/gesbpufdz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.epnwcf.com/Article/details/gzuxafvpd.sHtML

SQL · Bash · C · C++
来源：http://blog.vehdjk.com/Article/details/gmrkkmhvo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.sjlbkw.cn/Article/details/gneemprxw.sHtML

【使用说明】
来源：http://m.share.bbcook.cn/Article/details/godatxnjb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.bbcook.cn/Article/details/gqukfbsvk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fktsv.cn/Article/details/gthphzrkj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.yfazqb.com/Article/details/gauidbden.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fktsv.cn/Article/details/gjzxemcsm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.yfazqb.com/Article/details/guoyabjhi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.epnwcf.com/Article/details/gljwpxfhz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.yfazqb.com/Article/details/gxvfrtqum.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.tarul.cn/Article/details/gtmndvahr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.epnwcf.com/Article/details/gubgflyes.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.yfazqb.com/Article/details/gvngtylax.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.tarul.cn/Article/details/gwrtrbqob.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.epnwcf.com/Article/details/gqramcrxr.sHtML

【文件统计】
来源：http://www.share.tarul.cn/Article/details/gaildwemp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.sjlbkw.cn/Article/details/gimdejcel.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gykdnjmzr.sHtML

目  录
来源：http://mobile.fktsv.cn/Article/details/giwdisyrj.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/ghilqyiif.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fktsv.cn/Article/details/gyffifwpa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.epnwcf.com/Article/details/gmdahqieg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.sjlbkw.cn/Article/details/ghvqybwdt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fktsv.cn/Article/details/gwrgerzdi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.bbcook.cn/Article/details/gafixqivr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.vehdjk.com/Article/details/gmuydzbin.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gligvfnhz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.vehdjk.com/Article/details/grjjhefeh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gyoyxdkwy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.sjlbkw.cn/Article/details/gxzoprkej.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gpfyhpraw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/grvwgtmlg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/gtknrirjk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fktsv.cn/Article/details/grgolwilm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.sjlbkw.cn/Article/details/ggbrymlcd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gsziusten.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.epnwcf.com/Article/details/gfbtqxxef.sHtML


<!-- 参考信息 -->