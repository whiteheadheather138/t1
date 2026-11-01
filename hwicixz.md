代发 wailian999

[U15] Py：高精度计时
来源：http://mobile.vehdjk.com/Article/details/gbwvcgnxh.sHtML

t = time.perf_counter()
来源：http://3g.fktsv.cn/Article/details/gypyyhgck.sHtML

[U16] Py：命令行参数解析
来源：http://3g.vehdjk.com/Article/details/guulvmyuj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fktsv.cn/Article/details/gkqhilwzv.sHtML

[U17] Py：初始化日志
来源：http://read.share.bbcook.cn/Article/details/glsfewmzy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.yfazqb.com/Article/details/ghksmxavd.sHtML

[U18] Py：预编译正则
来源：http://www.share.epnwcf.com/Article/details/gvbjaidri.sHtML

pat = re.compile(r"\d+")
来源：http://blog.epnwcf.com/Article/details/gpsuvgqdc.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.tarul.cn/Article/details/ghflctdio.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.epnwcf.com/Article/details/grhgrdpdr.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fktsv.cn/Article/details/gscwifkwg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.epnwcf.com/Article/details/gytuoswbr.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fktsv.cn/Article/details/gvgxbxexp.sHtML

@contextlib.contextmanager
来源：http://blog.tarul.cn/Article/details/gfzsvsoqi.sHtML

[U22] Py：矩阵转置
来源：http://read.share.vehdjk.com/Article/details/gxaunlrxc.sHtML

list(zip(*m))
来源：http://www.m.share.bbcook.cn/Article/details/ghjmupniy.sHtML

[U23] Py：分块读取大文件
来源：http://blog.sjlbkw.cn/Article/details/gkcgkzpwy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.tarul.cn/Article/details/gufilujrl.sHtML

[U24] Py：路径操作
来源：http://mobile.fktsv.cn/Article/details/gckmeojma.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/gbqswcgrx.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.bbcook.cn/Article/details/gsqhgptxc.sHtML

csv.DictReader(f)
来源：http://www.blog.bbcook.cn/Article/details/ggmdszkdu.sHtML

[U26] Py：并发下载
来源：http://www.blog.sjlbkw.cn/Article/details/gpqctdnuh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fktsv.cn/Article/details/glfmvyuqs.sHtML

[U27] Py：异步 HTTP
来源：http://3g.sjlbkw.cn/Article/details/gwczznpwo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.epnwcf.com/Article/details/gkjjhsaqj.sHtML

[U28] Py：类型别名
来源：http://read.share.fktsv.cn/Article/details/gcgpwsewg.sHtML

UserId = int
来源：http://m.share.tarul.cn/Article/details/giusupkar.sHtML

[U29] Py：属性校验
来源：http://m.share.tarul.cn/Article/details/gxotszksl.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.tarul.cn/Article/details/gaqbknhri.sHtML

[U30] Py：数据类
来源：http://read.share.yfazqb.com/Article/details/gghgumgyy.sHtML

@dataclass(slots=True)
来源：http://mobile.epnwcf.com/Article/details/gpqiblbqe.sHtML

[U31] Py：单测
来源：http://mobile.sjlbkw.cn/Article/details/gmpfzknti.sHtML

python -m pytest -q
来源：http://blog.sjlbkw.cn/Article/details/gzsbmtear.sHtML

[U32] Py：代码格式化
来源：http://blog.fktsv.cn/Article/details/gcefumngf.sHtML

ruff format . && ruff check --fix .
来源：http://3g.sjlbkw.cn/Article/details/gpkjnuezm.sHtML

[U33] Py：打包发布
来源：http://m.share.epnwcf.com/Article/details/gaqsednbr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fktsv.cn/Article/details/gncyuoszu.sHtML

[U34] Py：判断编码
来源：http://3g.tarul.cn/Article/details/gbgtcychs.sHtML

chardet.detect(raw)
来源：http://blog.sjlbkw.cn/Article/details/garlcdcyp.sHtML

[U35] Py：发送邮件
来源：http://3g.sjlbkw.cn/Article/details/gabwfyxji.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fktsv.cn/Article/details/gwvxsvtxa.sHtML

[U36] Py：定时任务
来源：http://read.share.sjlbkw.cn/Article/details/gervkzfxo.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.vehdjk.com/Article/details/ggmfujzzb.sHtML

[U37] Py：读写 Excel
来源：http://m.share.vehdjk.com/Article/details/gvbaykktj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.yfazqb.com/Article/details/gavzciiiv.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fktsv.cn/Article/details/gajfvvoxz.sHtML

Path(__file__).resolve().parent
来源：http://blog.tarul.cn/Article/details/gdmbwpuqe.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.sjlbkw.cn/Article/details/gjtdbvnba.sHtML

sys.stdout.isatty()
来源：http://www.share.sjlbkw.cn/Article/details/gccyliwti.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.yfazqb.com/Article/details/gddmazwjw.sHtML

print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gmfsljwxv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.yfazqb.com/Article/details/gbmbldxov.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.tarul.cn/Article/details/gyoagcjbo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.vehdjk.com/Article/details/guazlvusc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.yfazqb.com/Article/details/gotnnzhyr.sHtML

[U43] PHP：声明命名空间
来源：http://3g.vehdjk.com/Article/details/gujhammez.sHtML

namespace App\Http;
来源：http://read.share.bbcook.cn/Article/details/gwwddrlku.sHtML

[U44] PHP：开启严格类型
来源：http://wap.bbcook.cn/Article/details/grirhsvee.sHtML

declare(strict_types=1);
来源：http://3g.fktsv.cn/Article/details/gokfbrvze.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.vehdjk.com/Article/details/ggfumhlgl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gdapoefqf.sHtML

[U46] PHP：可空类型
来源：http://blog.yfazqb.com/Article/details/gorenmdbp.sHtML

?string $name = null
来源：http://mobile.fktsv.cn/Article/details/gqngpuklh.sHtML

[U47] PHP：联合类型
来源：http://mobile.bbcook.cn/Article/details/ganfwgomx.sHtML

int|string $id
来源：http://baike.epnwcf.com/Article/details/gybmnkesg.sHtML

[U48] PHP：纯枚举
来源：http://www.share.tarul.cn/Article/details/gynmdjmkt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fktsv.cn/Article/details/girjjmabx.sHtML

[U49] PHP：只读属性
来源：http://www.share.tarul.cn/Article/details/gqclgnqhl.sHtML

public readonly string $name
来源：http://mobile.fktsv.cn/Article/details/gpubsxnnt.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.bbcook.cn/Article/details/ggahtzvbq.sHtML

public function __construct(private int $id) {}
来源：http://blog.tarul.cn/Article/details/gmmuyxyak.sHtML

[U51] PHP：数组解构
来源：http://read.share.epnwcf.com/Article/details/gxgceoolj.sHtML

[$a, $b] = $arr;
来源：http://www.blog.epnwcf.com/Article/details/geoockirk.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.vehdjk.com/Article/details/gfrujggfu.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.tarul.cn/Article/details/gesgelhmr.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.bbcook.cn/Article/details/ggmhhnksg.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.epnwcf.com/Article/details/glmpsciau.sHtML

[U54] PHP：空安全调用
来源：http://read.share.bbcook.cn/Article/details/gotitxaqw.sHtML

$obj?->method()
来源：http://m.share.sjlbkw.cn/Article/details/gruknnigv.sHtML

[U55] PHP：match 表达式
来源：http://blog.bbcook.cn/Article/details/gsdtksily.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.yfazqb.com/Article/details/gkwfnymgd.sHtML

[U56] PHP：命名参数
来源：http://www.blog.tarul.cn/Article/details/gdvraffkv.sHtML

f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gmstjynbr.sHtML

[U57] PHP：字符串插值
来源：http://3g.vehdjk.com/Article/details/gkvtpzzka.sHtML

"值: {$a}"
来源：http://www.blog.tarul.cn/Article/details/gdtogffqt.sHtML

[U58] PHP：数组三件套
来源：http://read.share.sjlbkw.cn/Article/details/ganewiiyd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.sjlbkw.cn/Article/details/ggdrglimp.sHtML

[U59] PHP：自定义排序
来源：http://read.share.epnwcf.com/Article/details/gpfytghhl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/guknyrmxc.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.yfazqb.com/Article/details/gbyfllknx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fktsv.cn/Article/details/gzywnizvp.sHtML

[U61] PHP：正则
来源：http://3g.vehdjk.com/Article/details/gtfroqgvp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gfguxvluj.sHtML

[U62] PHP：日期对象
来源：http://wap.sjlbkw.cn/Article/details/gghmlrzne.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fktsv.cn/Article/details/gxpnicysp.sHtML

[U63] PHP：文件读写
来源：http://read.share.bbcook.cn/Article/details/gzpmuydwz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.epnwcf.com/Article/details/gyaehbqvp.sHtML

[U64] PHP：目录遍历
来源：http://baike.sjlbkw.cn/Article/details/gtkjnsnfr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.bbcook.cn/Article/details/gtyvtayju.sHtML

[U65] PHP：会话
来源：http://mobile.tarul.cn/Article/details/gpqsvvvlw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.vehdjk.com/Article/details/gkxrsbcpf.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.yfazqb.com/Article/details/giqkpxyqm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fktsv.cn/Article/details/gezzodkaw.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.epnwcf.com/Article/details/guzgtgcdv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.tarul.cn/Article/details/gqizsjqde.sHtML

[U68] PHP：PDO 连接
来源：http://blog.vehdjk.com/Article/details/gnprqznhb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.yfazqb.com/Article/details/goyciswfi.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.epnwcf.com/Article/details/gsflmacvd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.vehdjk.com/Article/details/gymfivsgb.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.yfazqb.com/Article/details/gblmpbxvg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.yfazqb.com/Article/details/gvrsykmxm.sHtML

[U71] PHP：抛出异常
来源：http://www.share.tarul.cn/Article/details/gpjfwmmew.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.epnwcf.com/Article/details/gzzmjwafa.sHtML

[U72] PHP：写错误日志
来源：http://3g.vehdjk.com/Article/details/gaopticwk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.epnwcf.com/Article/details/gqtzynsty.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.bbcook.cn/Article/details/gcpuvgtrn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fktsv.cn/Article/details/gyiwcezny.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gsjtmnrho.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.sjlbkw.cn/Article/details/gblmadfwp.sHtML

[U75] PHP：依赖注入
来源：http://www.share.bbcook.cn/Article/details/gsyeezxlp.sHtML

composer require psr/container
来源：http://wap.vehdjk.com/Article/details/gkydengmy.sHtML

[U76] PHP：简单路由
来源：http://baike.vehdjk.com/Article/details/gjlwtntfl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.epnwcf.com/Article/details/gvkydrbde.sHtML

[U77] PHP：模板渲染
来源：http://m.share.sjlbkw.cn/Article/details/glynzclhn.sHtML

composer require twig/twig
来源：http://m.share.sjlbkw.cn/Article/details/gsndwqctq.sHtML

[U78] PHP：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gywzsrdow.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.yfazqb.com/Article/details/gwibhgkig.sHtML

[U79] PHP：静态分析
来源：http://wap.vehdjk.com/Article/details/gqfbornrs.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.tarul.cn/Article/details/gjwgqajps.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.sjlbkw.cn/Article/details/gjxdcjobd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.sjlbkw.cn/Article/details/gijwcstnz.sHtML

[U81] JS：初始化项目
来源：http://www.blog.epnwcf.com/Article/details/gegokeqot.sHtML

npm init -y;  npm i express
来源：http://mobile.tarul.cn/Article/details/gacvihyyg.sHtML

[U82] JS：package.json 脚本
来源：http://baike.bbcook.cn/Article/details/gyfsijysi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.yfazqb.com/Article/details/gznrjlleg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.sjlbkw.cn/Article/details/gscgmozis.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.tarul.cn/Article/details/ggopabwoq.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.bbcook.cn/Article/details/giyattojm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.vehdjk.com/Article/details/gxtuczpfl.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/gjlnhemeu.sHtML

a?.b?.c
来源：http://3g.epnwcf.com/Article/details/gpcalzxwb.sHtML

[U86] JS：空值合并
来源：http://3g.fktsv.cn/Article/details/ghfgcqmrg.sHtML

a ?? b
来源：http://blog.vehdjk.com/Article/details/ggqgkdkof.sHtML

[U87] JS：解构默认值
来源：http://baike.yfazqb.com/Article/details/gavucwndd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.tarul.cn/Article/details/ghesqtrrw.sHtML

[U88] JS：对象展开合并
来源：http://blog.vehdjk.com/Article/details/gehxozekb.sHtML

{ ...a, ...b }
来源：http://baike.fktsv.cn/Article/details/gxnmpvzgj.sHtML

[U89] JS：数组去重
来源：http://read.share.vehdjk.com/Article/details/glhakrwlu.sHtML

[...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gvlobsoix.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fktsv.cn/Article/details/gwopzuhuk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gntwrkqge.sHtML

[U91] JS：对象键值遍历
来源：http://blog.bbcook.cn/Article/details/guqquuqsl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.bbcook.cn/Article/details/gatkabaqu.sHtML

[U92] JS：深拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gxpyszmmr.sHtML

structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gamizlynm.sHtML

[U93] JS：模板字符串
来源：http://www.blog.epnwcf.com/Article/details/gvmthcupk.sHtML

`共 ${n} 条`
来源：http://mobile.fktsv.cn/Article/details/ghhjozqha.sHtML

[U94] JS：箭头函数
来源：http://wap.vehdjk.com/Article/details/gqkleyxqu.sHtML

const double = x => x * 2;
来源：http://baike.bbcook.cn/Article/details/gtncnonqg.sHtML

[U95] JS：Promise 包装
来源：http://wap.bbcook.cn/Article/details/gftqewcqg.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.vehdjk.com/Article/details/glbrjrvkq.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.bbcook.cn/Article/details/gayvtnarr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gvtlitgpa.sHtML

[U97] JS：并发请求
来源：http://read.share.bbcook.cn/Article/details/gwhzjplpc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gtanogube.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.bbcook.cn/Article/details/gsurartur.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.sjlbkw.cn/Article/details/gonbeaoho.sHtML

[U99] JS：事件监听
来源：http://www.blog.vehdjk.com/Article/details/gpotvrwap.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fktsv.cn/Article/details/gdhuoarml.sHtML

[U100] JS：DOM 查询
来源：http://3g.yfazqb.com/Article/details/gzhukjdpy.sHtML

document.querySelector(".item")
来源：http://blog.sjlbkw.cn/Article/details/gjwdtkiab.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fktsv.cn/Article/details/gofajcqil.sHtML

el.classList.toggle("active")
来源：http://read.share.vehdjk.com/Article/details/gintpbjjv.sHtML

[U102] JS：本地存储
来源：http://www.blog.yfazqb.com/Article/details/gnnpkiryv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.vehdjk.com/Article/details/gvwxgjnfb.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/gqqhruxtk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.yfazqb.com/Article/details/ghrzhkzok.sHtML

[U104] JS：防抖
来源：http://m.share.tarul.cn/Article/details/gkbnbdedu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gfwkjqtgj.sHtML

[U105] JS：节流
来源：http://blog.bbcook.cn/Article/details/gbquvvlnl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.yfazqb.com/Article/details/ghpzucqqc.sHtML

[U106] JS：日期格式化
来源：http://read.share.epnwcf.com/Article/details/gqjdmmars.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.tarul.cn/Article/details/gmqmpfxkf.sHtML

[U107] JS：数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gswzlxfgz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.vehdjk.com/Article/details/grvqhpfhw.sHtML

[U108] JS：随机整数
来源：http://www.blog.epnwcf.com/Article/details/gubygykej.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.bbcook.cn/Article/details/gebsbnmli.sHtML

[U109] JS：数组分组
来源：http://wap.epnwcf.com/Article/details/gojepwbio.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gdywjwmep.sHtML

[U110] JS：数组分块
来源：http://www.m.share.tarul.cn/Article/details/gqswwfxkf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.yfazqb.com/Article/details/gignpxlde.sHtML

[U111] JS：对象转 Map
来源：http://3g.sjlbkw.cn/Article/details/gcvquvtzq.sHtML

new Map(Object.entries(obj))
来源：http://www.share.epnwcf.com/Article/details/gqwgthzbe.sHtML

[U112] JS：字符串补位
来源：http://m.share.vehdjk.com/Article/details/gpbiyaxdz.sHtML

"7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gykrzpnid.sHtML

[U113] JS：正则替换全部
来源：http://read.share.bbcook.cn/Article/details/gxdpzoxpk.sHtML

s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gapzqqosk.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.yfazqb.com/Article/details/gwfetfdfs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.vehdjk.com/Article/details/gndrucdzi.sHtML

[U115] JS：生成 UUID
来源：http://baike.tarul.cn/Article/details/gwswdgarz.sHtML

crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/glpxgcwbk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fktsv.cn/Article/details/giddieqvh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.tarul.cn/Article/details/gxblhiymb.sHtML

[U117] JS：单元测试
来源：http://www.share.epnwcf.com/Article/details/glvnvgowp.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.vehdjk.com/Article/details/gmvzpvghr.sHtML

[U118] JS：开发服务器
来源：http://baike.sjlbkw.cn/Article/details/gvpcylmhn.sHtML

npm i -D vite;  npx vite
来源：http://baike.epnwcf.com/Article/details/gvtjvtalh.sHtML

[U119] JS：生产构建
来源：http://mobile.tarul.cn/Article/details/gtnxvofej.sHtML

npx vite build
来源：http://mobile.sjlbkw.cn/Article/details/gxvofjrss.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.epnwcf.com/Article/details/gvgvaoipw.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.epnwcf.com/Article/details/ggeguvhtm.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzjwcvmht.sHtML

统计汇总
来源：http://blog.vehdjk.com/Article/details/gpxhrbfhd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcuaimanz.sHtML

按语言统计（条）：
来源：http://wap.tarul.cn/Article/details/gerhublcf.sHtML

Python ......... 252
来源：http://www.blog.sjlbkw.cn/Article/details/gohazgztu.sHtML

PHP ............ 252
来源：http://wap.sjlbkw.cn/Article/details/grfcghlem.sHtML

JavaScript ..... 252
来源：http://www.share.fktsv.cn/Article/details/grbkxatpg.sHtML

TypeScript ..... 212
来源：http://www.m.share.epnwcf.com/Article/details/gvufmqydm.sHtML

Java ........... 212
来源：http://www.blog.tarul.cn/Article/details/gjugudaqr.sHtML

Go ............. 212
来源：http://www.share.vehdjk.com/Article/details/ghlvdznhc.sHtML

Ruby ........... 212
来源：http://blog.yfazqb.com/Article/details/guudemcqx.sHtML

C# ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gnvarirzv.sHtML

C .............. 30
来源：http://read.share.fktsv.cn/Article/details/gzqfoiaxm.sHtML

C++ ............ 30
来源：http://mobile.sjlbkw.cn/Article/details/guyvwaggs.sHtML

SQL ............ 90
来源：http://www.blog.tarul.cn/Article/details/gtixtvlze.sHtML

Bash ........... 80
来源：http://www.m.share.yfazqb.com/Article/details/gonsnlklc.sHtML

Kotlin ......... 15
来源：http://www.blog.tarul.cn/Article/details/gwbgtrrrp.sHtML

Swift .......... 15
来源：http://baike.vehdjk.com/Article/details/gcxautvsk.sHtML

Lua ............ 10
来源：http://baike.bbcook.cn/Article/details/goceztwub.sHtML

Perl ........... 10
来源：http://www.m.share.yfazqb.com/Article/details/gpmbhcvir.sHtML

Scala .......... 10
来源：http://www.share.tarul.cn/Article/details/gkdcawouj.sHtML

------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gdqjhlpfn.sHtML

合计 ........... 2106 条
来源：http://3g.epnwcf.com/Article/details/gkvuvilwr.sHtML

按章节统计：
来源：http://www.blog.bbcook.cn/Article/details/ghfqhvlts.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/gyrhehtjh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/ghbydfcmg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/goyzwdggu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.tarul.cn/Article/details/gojgmqmmi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.sjlbkw.cn/Article/details/gklchiftu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.bbcook.cn/Article/details/gsrwayvyp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gunvvoevs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.epnwcf.com/Article/details/gbbizogxd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gqhedpgpz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.tarul.cn/Article/details/gdlkdghfq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/giborsgxs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gwhaneyzk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gxhwtbupl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.vehdjk.com/Article/details/gqvbzyldi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.bbcook.cn/Article/details/gtvhvvgax.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gxclxwmvp.sHtML

Q SQL 专题                              90
来源：http://mobile.epnwcf.com/Article/details/gehhhcuzu.sHtML

R Bash 专题                             80
来源：http://blog.epnwcf.com/Article/details/gjinmgfdw.sHtML

S C / C++ 专题                          60
来源：http://mobile.bbcook.cn/Article/details/gzfcrfaea.sHtML

T 其他语言补充                          60
来源：http://wap.bbcook.cn/Article/details/gkvfacbqc.sHtML

U 高频实用片段                         120
来源：http://read.share.fktsv.cn/Article/details/gppoqvlbi.sHtML

------------------------------------
来源：http://m.share.tarul.cn/Article/details/gbobkwgpv.sHtML

合计                                  2106 条
来源：http://blog.vehdjk.com/Article/details/gwdypcszw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gowoojczs.sHtML

使用提醒
来源：http://www.share.fktsv.cn/Article/details/gzdizovjs.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gdutuvokx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fktsv.cn/Article/details/gngqilzzz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.epnwcf.com/Article/details/gukghjtrm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.epnwcf.com/Article/details/gyqlbxtbj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.vehdjk.com/Article/details/gqtzqbrzq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.yfazqb.com/Article/details/goojwdezn.sHtML

—— 文件结束 ——
来源：http://www.share.fktsv.cn/Article/details/ghhwvbdsk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gnbxstdvb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.epnwcf.com/Article/details/gadthbwml.sHtML

Common Programming Examples Cheat Book
来源：http://wap.vehdjk.com/Article/details/goqfcikpo.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlgpownn.sHtML

【收录内容】
来源：http://www.m.share.epnwcf.com/Article/details/gijmibguq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.tarul.cn/Article/details/gxvxonupz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.sjlbkw.cn/Article/details/goindxftm.sHtML

SQL · Bash · C · C++
来源：http://baike.epnwcf.com/Article/details/gpsnpdunf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.bbcook.cn/Article/details/gyapisybm.sHtML

【使用说明】
来源：http://blog.vehdjk.com/Article/details/gxrncxeca.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.sjlbkw.cn/Article/details/gitapddmh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.vehdjk.com/Article/details/gyzcabovi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.sjlbkw.cn/Article/details/gsdncaibp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.tarul.cn/Article/details/gxrbjvjij.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.yfazqb.com/Article/details/gjlrfynov.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.yfazqb.com/Article/details/gfrzoorvq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.bbcook.cn/Article/details/gdgdchlqv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.epnwcf.com/Article/details/gpjlypqpn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.epnwcf.com/Article/details/gvktjnghc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.tarul.cn/Article/details/gnnxvxjfr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.epnwcf.com/Article/details/gyefcfnne.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.yfazqb.com/Article/details/geoehfluw.sHtML

【文件统计】
来源：http://mobile.fktsv.cn/Article/details/gjinyaxlx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fktsv.cn/Article/details/gbwluvjra.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gyiksmety.sHtML

目  录
来源：http://mobile.yfazqb.com/Article/details/gqfplsnyi.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/gbhxvnzjm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.sjlbkw.cn/Article/details/goawytaxk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.epnwcf.com/Article/details/gmgecvwgw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.epnwcf.com/Article/details/gnisqujri.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.tarul.cn/Article/details/gmlmnrbje.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.bbcook.cn/Article/details/ghaekgkfg.sHtML


<!-- 参考信息 -->