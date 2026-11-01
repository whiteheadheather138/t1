代发 wailian999

[U15] Py：高精度计时
来源：http://www.share.sjlbkw.cn/Article/details/ggexoiluv.sHtML

t = time.perf_counter()
来源：http://mobile.epnwcf.com/Article/details/gwylbslhd.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.epnwcf.com/Article/details/gfdtrycrm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.epnwcf.com/Article/details/gclxatsnh.sHtML

[U17] Py：初始化日志
来源：http://3g.vehdjk.com/Article/details/girlhldgw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.yfazqb.com/Article/details/gsdjudaoz.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.epnwcf.com/Article/details/gvnswdjqj.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fktsv.cn/Article/details/gqibotcuu.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrvnfbfz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.tarul.cn/Article/details/gquucrdgc.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.epnwcf.com/Article/details/gijozgxwf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.sjlbkw.cn/Article/details/gwwebxkmg.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.epnwcf.com/Article/details/gdowcccil.sHtML

@contextlib.contextmanager
来源：http://www.share.fktsv.cn/Article/details/gogsjtldn.sHtML

[U22] Py：矩阵转置
来源：http://mobile.epnwcf.com/Article/details/gxdulngze.sHtML

list(zip(*m))
来源：http://www.blog.epnwcf.com/Article/details/gmixsbpaw.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.sjlbkw.cn/Article/details/gxwvklczy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.tarul.cn/Article/details/gfqcftlnr.sHtML

[U24] Py：路径操作
来源：http://blog.vehdjk.com/Article/details/glmmzgvao.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/giphtrabx.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fktsv.cn/Article/details/gkmgsxxsu.sHtML

csv.DictReader(f)
来源：http://3g.sjlbkw.cn/Article/details/gvkehiaxv.sHtML

[U26] Py：并发下载
来源：http://m.share.bbcook.cn/Article/details/ghiwktaea.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.bbcook.cn/Article/details/gfwwedqjl.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.yfazqb.com/Article/details/gtcglygbx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.bbcook.cn/Article/details/gvkpdtslm.sHtML

[U28] Py：类型别名
来源：http://blog.yfazqb.com/Article/details/garxreadd.sHtML

UserId = int
来源：http://m.share.fktsv.cn/Article/details/gckgpflts.sHtML

[U29] Py：属性校验
来源：http://www.blog.bbcook.cn/Article/details/gzyiuqoor.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.yfazqb.com/Article/details/gzhcuiolj.sHtML

[U30] Py：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlytpayi.sHtML

@dataclass(slots=True)
来源：http://3g.bbcook.cn/Article/details/gjtpznigu.sHtML

[U31] Py：单测
来源：http://www.blog.fktsv.cn/Article/details/gnuajeucw.sHtML

python -m pytest -q
来源：http://baike.vehdjk.com/Article/details/gjyoaxcwr.sHtML

[U32] Py：代码格式化
来源：http://3g.tarul.cn/Article/details/gpwimlvmj.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.tarul.cn/Article/details/gnfzsgwlr.sHtML

[U33] Py：打包发布
来源：http://www.blog.vehdjk.com/Article/details/ggardylbh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.yfazqb.com/Article/details/gvakfereh.sHtML

[U34] Py：判断编码
来源：http://read.share.vehdjk.com/Article/details/gonggbaxc.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/geqdhvuni.sHtML

[U35] Py：发送邮件
来源：http://blog.sjlbkw.cn/Article/details/gbthpxuur.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.epnwcf.com/Article/details/gnwlmprss.sHtML

[U36] Py：定时任务
来源：http://blog.bbcook.cn/Article/details/gsgdsswbh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.sjlbkw.cn/Article/details/gfpstkrml.sHtML

[U37] Py：读写 Excel
来源：http://wap.fktsv.cn/Article/details/gkklwcmwu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fktsv.cn/Article/details/grcuiwrgu.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.yfazqb.com/Article/details/gfwvottep.sHtML

Path(__file__).resolve().parent
来源：http://read.share.epnwcf.com/Article/details/gnwoegdpc.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.yfazqb.com/Article/details/gxutfpoua.sHtML

sys.stdout.isatty()
来源：http://m.share.bbcook.cn/Article/details/gcdfpulbj.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.yfazqb.com/Article/details/ghtybnnsf.sHtML

print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/ghmhlqmaq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.bbcook.cn/Article/details/gptevyjhi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.yfazqb.com/Article/details/ggbcbmcoq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.vehdjk.com/Article/details/gzbuubbku.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.yfazqb.com/Article/details/grvczvhfo.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.tarul.cn/Article/details/gsskwsfqr.sHtML

namespace App\Http;
来源：http://baike.sjlbkw.cn/Article/details/gdfenqlzn.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.tarul.cn/Article/details/geuotzlaw.sHtML

declare(strict_types=1);
来源：http://3g.vehdjk.com/Article/details/ghbtmmnan.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.vehdjk.com/Article/details/gjqvjovzb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gosbbiptu.sHtML

[U46] PHP：可空类型
来源：http://read.share.fktsv.cn/Article/details/gshfyoutw.sHtML

?string $name = null
来源：http://read.share.bbcook.cn/Article/details/gjeloyjwe.sHtML

[U47] PHP：联合类型
来源：http://m.share.tarul.cn/Article/details/gumeubujo.sHtML

int|string $id
来源：http://read.share.bbcook.cn/Article/details/gvkcjjekq.sHtML

[U48] PHP：纯枚举
来源：http://blog.vehdjk.com/Article/details/gspobljqd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.yfazqb.com/Article/details/gfoebgppo.sHtML

[U49] PHP：只读属性
来源：http://blog.vehdjk.com/Article/details/gnycocjwv.sHtML

public readonly string $name
来源：http://blog.epnwcf.com/Article/details/gwisiuqzl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.vehdjk.com/Article/details/glptrmbkx.sHtML

public function __construct(private int $id) {}
来源：http://mobile.epnwcf.com/Article/details/gghtffcau.sHtML

[U51] PHP：数组解构
来源：http://www.blog.sjlbkw.cn/Article/details/gsnqfbdhq.sHtML

[$a, $b] = $arr;
来源：http://m.share.tarul.cn/Article/details/gczgysnmg.sHtML

[U52] PHP：箭头函数
来源：http://blog.yfazqb.com/Article/details/gczuiufyk.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.vehdjk.com/Article/details/gsuzsgrtl.sHtML

[U53] PHP：空合并运算符
来源：http://blog.sjlbkw.cn/Article/details/gutbfmnqp.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.sjlbkw.cn/Article/details/ggdxsbpft.sHtML

[U54] PHP：空安全调用
来源：http://m.share.epnwcf.com/Article/details/gnkvofayx.sHtML

$obj?->method()
来源：http://mobile.epnwcf.com/Article/details/gghunfgop.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fktsv.cn/Article/details/gbnisruqn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.epnwcf.com/Article/details/gzhltwgta.sHtML

[U56] PHP：命名参数
来源：http://wap.vehdjk.com/Article/details/gvgotikut.sHtML

f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gbattejug.sHtML

[U57] PHP：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gmheziwvv.sHtML

"值: {$a}"
来源：http://baike.fktsv.cn/Article/details/gdkilhgbk.sHtML

[U58] PHP：数组三件套
来源：http://mobile.vehdjk.com/Article/details/gstygcboo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.sjlbkw.cn/Article/details/ghwpkfhie.sHtML

[U59] PHP：自定义排序
来源：http://m.share.epnwcf.com/Article/details/gylzgkywj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gfhbvskeb.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.vehdjk.com/Article/details/gkymamdnc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fktsv.cn/Article/details/gxbgccoon.sHtML

[U61] PHP：正则
来源：http://www.share.yfazqb.com/Article/details/gecoijypy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/gqycfnbnz.sHtML

[U62] PHP：日期对象
来源：http://read.share.yfazqb.com/Article/details/gxeqnjdoi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.vehdjk.com/Article/details/gawarxntu.sHtML

[U63] PHP：文件读写
来源：http://wap.tarul.cn/Article/details/gygkjbmke.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.yfazqb.com/Article/details/ghqluzdhg.sHtML

[U64] PHP：目录遍历
来源：http://wap.epnwcf.com/Article/details/glzwsepwv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.epnwcf.com/Article/details/gookxujar.sHtML

[U65] PHP：会话
来源：http://blog.epnwcf.com/Article/details/gemqppvnt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gsmvtjxlh.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.bbcook.cn/Article/details/gfdiiszdi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.bbcook.cn/Article/details/ggncdsksz.sHtML

[U67] PHP：处理文件上传
来源：http://blog.yfazqb.com/Article/details/gojjswhwu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fktsv.cn/Article/details/globofvyv.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.vehdjk.com/Article/details/gmzsnsawr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.yfazqb.com/Article/details/gljsczkob.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fktsv.cn/Article/details/gtlaxslrh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.bbcook.cn/Article/details/giedjyvpi.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.tarul.cn/Article/details/gapavicyw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/gspeqpewg.sHtML

[U71] PHP：抛出异常
来源：http://wap.epnwcf.com/Article/details/gzqrpjtam.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.sjlbkw.cn/Article/details/gabksukpt.sHtML

[U72] PHP：写错误日志
来源：http://m.share.sjlbkw.cn/Article/details/gnmdegygz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.yfazqb.com/Article/details/gvslxmejb.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.sjlbkw.cn/Article/details/gtsiqwjwg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.vehdjk.com/Article/details/gmgpkkpbp.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.epnwcf.com/Article/details/ggotfhcww.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fktsv.cn/Article/details/gbzmmmhic.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fktsv.cn/Article/details/gbnrsadlm.sHtML

composer require psr/container
来源：http://3g.yfazqb.com/Article/details/ghatckylp.sHtML

[U76] PHP：简单路由
来源：http://www.share.fktsv.cn/Article/details/gwoxikmsn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fktsv.cn/Article/details/gdvzaadrm.sHtML

[U77] PHP：模板渲染
来源：http://baike.bbcook.cn/Article/details/gskdmmokp.sHtML

composer require twig/twig
来源：http://blog.bbcook.cn/Article/details/ggofwkjkx.sHtML

[U78] PHP：单元测试
来源：http://wap.vehdjk.com/Article/details/gnrvhzhcr.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fktsv.cn/Article/details/ghreevpjm.sHtML

[U79] PHP：静态分析
来源：http://baike.bbcook.cn/Article/details/gctzrmszb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.sjlbkw.cn/Article/details/ghdcemhme.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.sjlbkw.cn/Article/details/gdyadjhxt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.vehdjk.com/Article/details/gvdzhrcrj.sHtML

[U81] JS：初始化项目
来源：http://3g.yfazqb.com/Article/details/gfomcxmft.sHtML

npm init -y;  npm i express
来源：http://m.share.yfazqb.com/Article/details/gqxczguba.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fktsv.cn/Article/details/gdwyifkco.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.sjlbkw.cn/Article/details/gsgnduxqq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.tarul.cn/Article/details/goilxdmwd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.bbcook.cn/Article/details/gaubvbncz.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.epnwcf.com/Article/details/gyudygohd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.epnwcf.com/Article/details/gzwhuaqjl.sHtML

[U85] JS：可选链
来源：http://m.share.fktsv.cn/Article/details/gfxlfkpap.sHtML

a?.b?.c
来源：http://www.blog.vehdjk.com/Article/details/gtgyqflyi.sHtML

[U86] JS：空值合并
来源：http://mobile.sjlbkw.cn/Article/details/gtfcpablm.sHtML

a ?? b
来源：http://www.blog.fktsv.cn/Article/details/gtequqtfm.sHtML

[U87] JS：解构默认值
来源：http://www.share.yfazqb.com/Article/details/gihihcwxy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.vehdjk.com/Article/details/gxcjvnrfb.sHtML

[U88] JS：对象展开合并
来源：http://3g.yfazqb.com/Article/details/gfbqlxotu.sHtML

{ ...a, ...b }
来源：http://www.m.share.vehdjk.com/Article/details/grstoyred.sHtML

[U89] JS：数组去重
来源：http://baike.yfazqb.com/Article/details/gkxjarooa.sHtML

[...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gjnsblgps.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.tarul.cn/Article/details/gqvqsnhbn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/geaafpeol.sHtML

[U91] JS：对象键值遍历
来源：http://baike.tarul.cn/Article/details/gyvogcykv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.tarul.cn/Article/details/grwmkasph.sHtML

[U92] JS：深拷贝
来源：http://www.share.tarul.cn/Article/details/gbhqrgbty.sHtML

structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gnfmtakbf.sHtML

[U93] JS：模板字符串
来源：http://blog.fktsv.cn/Article/details/gudvzqyhv.sHtML

`共 ${n} 条`
来源：http://blog.fktsv.cn/Article/details/gyxjtabog.sHtML

[U94] JS：箭头函数
来源：http://baike.tarul.cn/Article/details/gkdqndeho.sHtML

const double = x => x * 2;
来源：http://wap.fktsv.cn/Article/details/gukjaxlmw.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.vehdjk.com/Article/details/gefkazxku.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fktsv.cn/Article/details/gcrudeoex.sHtML

[U96] JS：async/await 与异常
来源：http://baike.yfazqb.com/Article/details/gybyirgeo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gphpdycez.sHtML

[U97] JS：并发请求
来源：http://www.blog.bbcook.cn/Article/details/gizhkyned.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gmzrznfkc.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.epnwcf.com/Article/details/gkjfbbwyc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.bbcook.cn/Article/details/gybpztziz.sHtML

[U99] JS：事件监听
来源：http://m.share.sjlbkw.cn/Article/details/gnemiqnve.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.vehdjk.com/Article/details/gldktjalj.sHtML

[U100] JS：DOM 查询
来源：http://m.share.bbcook.cn/Article/details/gdownfymx.sHtML

document.querySelector(".item")
来源：http://read.share.fktsv.cn/Article/details/ggwabxbjb.sHtML

[U101] JS：classList 操作
来源：http://www.blog.vehdjk.com/Article/details/gjvrjnnhj.sHtML

el.classList.toggle("active")
来源：http://www.m.share.bbcook.cn/Article/details/gppajasjy.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fktsv.cn/Article/details/gkucofrdf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.bbcook.cn/Article/details/gfofbqqbq.sHtML

[U103] JS：定时器
来源：http://baike.sjlbkw.cn/Article/details/gyvgsjeqh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.tarul.cn/Article/details/ggetdemfo.sHtML

[U104] JS：防抖
来源：http://3g.vehdjk.com/Article/details/gpardtwup.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gyylqvmtc.sHtML

[U105] JS：节流
来源：http://mobile.vehdjk.com/Article/details/gkgfivgyb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.tarul.cn/Article/details/gzmwqhofs.sHtML

[U106] JS：日期格式化
来源：http://mobile.yfazqb.com/Article/details/gcubzngnl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.epnwcf.com/Article/details/gxpfkskih.sHtML

[U107] JS：数字千分位
来源：http://mobile.bbcook.cn/Article/details/gazmefiei.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fktsv.cn/Article/details/gbapswjnb.sHtML

[U108] JS：随机整数
来源：http://blog.vehdjk.com/Article/details/gdgjmagtl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.vehdjk.com/Article/details/gdhnrifld.sHtML

[U109] JS：数组分组
来源：http://wap.yfazqb.com/Article/details/gkepujfgz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.bbcook.cn/Article/details/goqcistkq.sHtML

[U110] JS：数组分块
来源：http://www.share.sjlbkw.cn/Article/details/gnldqzeus.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.sjlbkw.cn/Article/details/gchnlwqis.sHtML

[U111] JS：对象转 Map
来源：http://m.share.sjlbkw.cn/Article/details/gxlzbzitc.sHtML

new Map(Object.entries(obj))
来源：http://m.share.yfazqb.com/Article/details/gximcyalu.sHtML

[U112] JS：字符串补位
来源：http://read.share.sjlbkw.cn/Article/details/gnhtcdtsb.sHtML

"7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gyiyoxguj.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.yfazqb.com/Article/details/gmtgeiolt.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gvnsbcavq.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.tarul.cn/Article/details/gaiufmqki.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvtcimxn.sHtML

[U115] JS：生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gdeufiavs.sHtML

crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gyqjwetpz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fktsv.cn/Article/details/gtfkgsvbq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.vehdjk.com/Article/details/ghecqunek.sHtML

[U117] JS：单元测试
来源：http://baike.yfazqb.com/Article/details/gkbaemmsm.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.tarul.cn/Article/details/gytgnbmmc.sHtML

[U118] JS：开发服务器
来源：http://www.share.fktsv.cn/Article/details/gfbmjvxoq.sHtML

npm i -D vite;  npx vite
来源：http://www.share.yfazqb.com/Article/details/gwnoauwdq.sHtML

[U119] JS：生产构建
来源：http://blog.tarul.cn/Article/details/ggmxtuvey.sHtML

npx vite build
来源：http://baike.yfazqb.com/Article/details/gnhcugawd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.sjlbkw.cn/Article/details/gnucecohw.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fktsv.cn/Article/details/gwwcjptpv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gnyxycyci.sHtML

统计汇总
来源：http://read.share.epnwcf.com/Article/details/gdixeppqg.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ghemrfywn.sHtML

按语言统计（条）：
来源：http://m.share.vehdjk.com/Article/details/gbnrqayep.sHtML

Python ......... 252
来源：http://www.share.yfazqb.com/Article/details/gdcsckxux.sHtML

PHP ............ 252
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcywfjmn.sHtML

JavaScript ..... 252
来源：http://3g.epnwcf.com/Article/details/gcrolyfot.sHtML

TypeScript ..... 212
来源：http://www.m.share.epnwcf.com/Article/details/gnmbtqbvf.sHtML

Java ........... 212
来源：http://mobile.sjlbkw.cn/Article/details/gnsitbtza.sHtML

Go ............. 212
来源：http://read.share.bbcook.cn/Article/details/gnpyejslr.sHtML

Ruby ........... 212
来源：http://read.share.bbcook.cn/Article/details/gizhswpki.sHtML

C# ............. 212
来源：http://3g.epnwcf.com/Article/details/gjeazhbif.sHtML

C .............. 30
来源：http://baike.epnwcf.com/Article/details/gskiyxplt.sHtML

C++ ............ 30
来源：http://www.share.bbcook.cn/Article/details/gkmgodnbn.sHtML

SQL ............ 90
来源：http://3g.yfazqb.com/Article/details/gnhwglrbk.sHtML

Bash ........... 80
来源：http://3g.fktsv.cn/Article/details/gkhezmiax.sHtML

Kotlin ......... 15
来源：http://read.share.sjlbkw.cn/Article/details/gmwfirzzd.sHtML

Swift .......... 15
来源：http://read.share.epnwcf.com/Article/details/ghvdqsfek.sHtML

Lua ............ 10
来源：http://baike.sjlbkw.cn/Article/details/gasndkqzf.sHtML

Perl ........... 10
来源：http://blog.fktsv.cn/Article/details/gerilsati.sHtML

Scala .......... 10
来源：http://m.share.vehdjk.com/Article/details/gqtsangxb.sHtML

------------------------------------
来源：http://3g.bbcook.cn/Article/details/gcdapapid.sHtML

合计 ........... 2106 条
来源：http://3g.epnwcf.com/Article/details/gmrabqsuh.sHtML

按章节统计：
来源：http://mobile.yfazqb.com/Article/details/gzmesbwns.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.vehdjk.com/Article/details/gqbzhqlwl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/grigztolx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/gtuuupavj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/gplydnlhl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.tarul.cn/Article/details/gghfjtvbe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/giocuhtfg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gqvnozbko.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/ghvgjwlib.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gxmoaczwx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fktsv.cn/Article/details/gexeuipia.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gbacfewgk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/glhjsdhto.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gyuptholg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.bbcook.cn/Article/details/gealiwkse.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.yfazqb.com/Article/details/groahmnxf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gnvszshqi.sHtML

Q SQL 专题                              90
来源：http://read.share.fktsv.cn/Article/details/gqedjilry.sHtML

R Bash 专题                             80
来源：http://mobile.yfazqb.com/Article/details/gereyozop.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.vehdjk.com/Article/details/gdokcygxp.sHtML

T 其他语言补充                          60
来源：http://read.share.epnwcf.com/Article/details/gohrpghnu.sHtML

U 高频实用片段                         120
来源：http://read.share.yfazqb.com/Article/details/gaqccybsv.sHtML

------------------------------------
来源：http://www.share.tarul.cn/Article/details/gmlalqwoj.sHtML

合计                                  2106 条
来源：http://www.m.share.epnwcf.com/Article/details/gkxorxjfa.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/grlpauiva.sHtML

使用提醒
来源：http://blog.fktsv.cn/Article/details/godewagyh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gqfdwyckc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.epnwcf.com/Article/details/gdirydtqi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.bbcook.cn/Article/details/grupcbtpn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.vehdjk.com/Article/details/gpiymtzig.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.sjlbkw.cn/Article/details/gqwqhffyn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.epnwcf.com/Article/details/gsxjddqri.sHtML

—— 文件结束 ——
来源：http://read.share.fktsv.cn/Article/details/gfzupnjjl.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/guinnfyui.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.sjlbkw.cn/Article/details/gwmmeckto.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.tarul.cn/Article/details/gzuyefsee.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gctxboost.sHtML

【收录内容】
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdlgwqae.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.yfazqb.com/Article/details/gsufybbxi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.vehdjk.com/Article/details/gnlhpeput.sHtML

SQL · Bash · C · C++
来源：http://read.share.tarul.cn/Article/details/gxjkdefgt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.yfazqb.com/Article/details/gsucqftvb.sHtML

【使用说明】
来源：http://read.share.tarul.cn/Article/details/gtzgtmhwu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.bbcook.cn/Article/details/gnyfbiaym.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.bbcook.cn/Article/details/gahuequuu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.epnwcf.com/Article/details/gguopkllv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.tarul.cn/Article/details/gmobmmxlf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.vehdjk.com/Article/details/gtfpwxwzf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.yfazqb.com/Article/details/gzvcowjvw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fktsv.cn/Article/details/gisbrqxqc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.vehdjk.com/Article/details/ghqohijvt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fktsv.cn/Article/details/gyskglztw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fktsv.cn/Article/details/gprhvfxny.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.bbcook.cn/Article/details/godzjhijz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.epnwcf.com/Article/details/gnnujqvsx.sHtML

【文件统计】
来源：http://www.blog.yfazqb.com/Article/details/gnnbsqclw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fktsv.cn/Article/details/gtkpkmnaw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gxoleieze.sHtML

目  录
来源：http://read.share.epnwcf.com/Article/details/gbhhdzkkq.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/grndlatqv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.yfazqb.com/Article/details/gfqgbqszt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.epnwcf.com/Article/details/gewsbfjzp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fktsv.cn/Article/details/gnbnxdngy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.bbcook.cn/Article/details/gzwrykatc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.vehdjk.com/Article/details/grterdxqi.sHtML


<!-- 参考信息 -->