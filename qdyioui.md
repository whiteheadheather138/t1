代发 wailian999

[U15] Py：高精度计时
来源：http://blog.yfazqb.com/Article/details/gxcceumyi.sHtML

t = time.perf_counter()
来源：http://read.share.bbcook.cn/Article/details/gqbqhctdc.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.epnwcf.com/Article/details/gqhlpsmdw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.tarul.cn/Article/details/gfuhhbvgj.sHtML

[U17] Py：初始化日志
来源：http://read.share.vehdjk.com/Article/details/gziqxzhnc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fktsv.cn/Article/details/geltxbdtb.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.tarul.cn/Article/details/gsedgusmj.sHtML

pat = re.compile(r"\d+")
来源：http://blog.epnwcf.com/Article/details/gwvwvqyne.sHtML

[U19] Py：正则替换带回调
来源：http://blog.bbcook.cn/Article/details/gckpvlmtg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fktsv.cn/Article/details/gisuwsrkr.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fktsv.cn/Article/details/gqvozasxw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.bbcook.cn/Article/details/gkevprxcl.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.sjlbkw.cn/Article/details/gxzmliisc.sHtML

@contextlib.contextmanager
来源：http://www.blog.epnwcf.com/Article/details/gpmawabbb.sHtML

[U22] Py：矩阵转置
来源：http://mobile.tarul.cn/Article/details/gfeamqknq.sHtML

list(zip(*m))
来源：http://mobile.epnwcf.com/Article/details/gkkmifvqo.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxcnvfjj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.yfazqb.com/Article/details/gmvezsrcx.sHtML

[U24] Py：路径操作
来源：http://www.share.bbcook.cn/Article/details/gimuwbswy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrbrfoxy.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.epnwcf.com/Article/details/gsuifzopl.sHtML

csv.DictReader(f)
来源：http://read.share.epnwcf.com/Article/details/gcuhaqdia.sHtML

[U26] Py：并发下载
来源：http://m.share.fktsv.cn/Article/details/gxopphbhl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.tarul.cn/Article/details/gxqnuaudp.sHtML

[U27] Py：异步 HTTP
来源：http://wap.tarul.cn/Article/details/gnyicbpur.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.sjlbkw.cn/Article/details/gbhoixsah.sHtML

[U28] Py：类型别名
来源：http://blog.yfazqb.com/Article/details/gyazaslhu.sHtML

UserId = int
来源：http://mobile.tarul.cn/Article/details/geplutvjj.sHtML

[U29] Py：属性校验
来源：http://mobile.tarul.cn/Article/details/ggysiaiyu.sHtML

@property 与 @x.setter 配合
来源：http://www.share.yfazqb.com/Article/details/gfuajlqpt.sHtML

[U30] Py：数据类
来源：http://wap.tarul.cn/Article/details/gttodoiah.sHtML

@dataclass(slots=True)
来源：http://www.share.yfazqb.com/Article/details/glaiclnpr.sHtML

[U31] Py：单测
来源：http://m.share.tarul.cn/Article/details/gyifxalci.sHtML

python -m pytest -q
来源：http://www.m.share.epnwcf.com/Article/details/geeyrlelk.sHtML

[U32] Py：代码格式化
来源：http://read.share.sjlbkw.cn/Article/details/ggtqyrlte.sHtML

ruff format . && ruff check --fix .
来源：http://baike.sjlbkw.cn/Article/details/gmikyqkqf.sHtML

[U33] Py：打包发布
来源：http://www.m.share.yfazqb.com/Article/details/gqcotuafx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.epnwcf.com/Article/details/gpplxupig.sHtML

[U34] Py：判断编码
来源：http://www.share.vehdjk.com/Article/details/gytdczjtw.sHtML

chardet.detect(raw)
来源：http://wap.bbcook.cn/Article/details/gltmfqqjm.sHtML

[U35] Py：发送邮件
来源：http://baike.epnwcf.com/Article/details/gttepoilc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.sjlbkw.cn/Article/details/gphjpoksm.sHtML

[U36] Py：定时任务
来源：http://3g.tarul.cn/Article/details/giqdgchet.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.vehdjk.com/Article/details/gzgejjjqa.sHtML

[U37] Py：读写 Excel
来源：http://mobile.vehdjk.com/Article/details/gttnajfdl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.vehdjk.com/Article/details/gaklkhavb.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fktsv.cn/Article/details/gzjfdpbkk.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.tarul.cn/Article/details/gatdypubt.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.vehdjk.com/Article/details/ggkuyyztx.sHtML

sys.stdout.isatty()
来源：http://wap.bbcook.cn/Article/details/gqvsbgxqu.sHtML

[U40] Py：打印到标准错误
来源：http://3g.sjlbkw.cn/Article/details/gjqxdmguw.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gfyidvxow.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.epnwcf.com/Article/details/gbuiurnao.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.epnwcf.com/Article/details/gilhamqik.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.tarul.cn/Article/details/gusevkhaz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.vehdjk.com/Article/details/gwervcfue.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.epnwcf.com/Article/details/gvljifaec.sHtML

namespace App\Http;
来源：http://baike.epnwcf.com/Article/details/guyekestp.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.tarul.cn/Article/details/gddhdhpcw.sHtML

declare(strict_types=1);
来源：http://www.share.bbcook.cn/Article/details/gtogllipy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fktsv.cn/Article/details/gxqduozvk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gqlgqesnp.sHtML

[U46] PHP：可空类型
来源：http://wap.fktsv.cn/Article/details/gwtaagxbu.sHtML

?string $name = null
来源：http://blog.bbcook.cn/Article/details/grxpmgeuy.sHtML

[U47] PHP：联合类型
来源：http://mobile.vehdjk.com/Article/details/gebgytrur.sHtML

int|string $id
来源：http://www.blog.epnwcf.com/Article/details/gmpvyqxln.sHtML

[U48] PHP：纯枚举
来源：http://read.share.vehdjk.com/Article/details/gzxpcygoy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.bbcook.cn/Article/details/gxzlugnef.sHtML

[U49] PHP：只读属性
来源：http://www.blog.yfazqb.com/Article/details/gnalktrfe.sHtML

public readonly string $name
来源：http://www.blog.tarul.cn/Article/details/gueqbrrfb.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.sjlbkw.cn/Article/details/gqrsisvqn.sHtML

public function __construct(private int $id) {}
来源：http://www.share.bbcook.cn/Article/details/gzomddprb.sHtML

[U51] PHP：数组解构
来源：http://wap.sjlbkw.cn/Article/details/glpjowawt.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/gqyramlqb.sHtML

[U52] PHP：箭头函数
来源：http://3g.bbcook.cn/Article/details/gcslyqbqv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.vehdjk.com/Article/details/gqbrxkftz.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fktsv.cn/Article/details/gptppkull.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhgazyke.sHtML

[U54] PHP：空安全调用
来源：http://3g.epnwcf.com/Article/details/gcqkfqiez.sHtML

$obj?->method()
来源：http://read.share.yfazqb.com/Article/details/ghwosppal.sHtML

[U55] PHP：match 表达式
来源：http://blog.sjlbkw.cn/Article/details/gwyuokvdw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.bbcook.cn/Article/details/gauxvpeaw.sHtML

[U56] PHP：命名参数
来源：http://wap.yfazqb.com/Article/details/gyypxzqah.sHtML

f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gmwqjhgta.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gnumgsoyb.sHtML

"值: {$a}"
来源：http://3g.sjlbkw.cn/Article/details/goysubaeu.sHtML

[U58] PHP：数组三件套
来源：http://3g.tarul.cn/Article/details/gnevrychu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.yfazqb.com/Article/details/gicqrjszq.sHtML

[U59] PHP：自定义排序
来源：http://m.share.sjlbkw.cn/Article/details/giclvuhiw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/gvgtybcst.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.bbcook.cn/Article/details/ginusdoak.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fktsv.cn/Article/details/gfvdxcjkd.sHtML

[U61] PHP：正则
来源：http://www.blog.sjlbkw.cn/Article/details/gtkumjxua.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gnlkovqaz.sHtML

[U62] PHP：日期对象
来源：http://read.share.fktsv.cn/Article/details/gtiflkqwn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.bbcook.cn/Article/details/gebelfqkl.sHtML

[U63] PHP：文件读写
来源：http://3g.vehdjk.com/Article/details/gsyewnwtx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.bbcook.cn/Article/details/gusissxta.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyqsllka.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.yfazqb.com/Article/details/ghxaqmpts.sHtML

[U65] PHP：会话
来源：http://baike.bbcook.cn/Article/details/gpghwbqtw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.bbcook.cn/Article/details/gnmsiwmre.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.bbcook.cn/Article/details/gfptowltr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.sjlbkw.cn/Article/details/gmbnzyndw.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.yfazqb.com/Article/details/gyocfoqfj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.bbcook.cn/Article/details/gwajwumqc.sHtML

[U68] PHP：PDO 连接
来源：http://wap.bbcook.cn/Article/details/ggkzznuug.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fktsv.cn/Article/details/gzotypnjs.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdgkuaur.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.vehdjk.com/Article/details/gzhhwrkwt.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.epnwcf.com/Article/details/gktwdoexk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/gywlimtmq.sHtML

[U71] PHP：抛出异常
来源：http://baike.sjlbkw.cn/Article/details/gguxaypdo.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.yfazqb.com/Article/details/gypowquii.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fktsv.cn/Article/details/gplntmmih.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.tarul.cn/Article/details/glrvstolo.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.epnwcf.com/Article/details/gmyxhfttr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.tarul.cn/Article/details/guetbzzmg.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gpmewybld.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.yfazqb.com/Article/details/gpgrjubob.sHtML

[U75] PHP：依赖注入
来源：http://read.share.tarul.cn/Article/details/gvfgkqdlu.sHtML

composer require psr/container
来源：http://wap.vehdjk.com/Article/details/gougoixdp.sHtML

[U76] PHP：简单路由
来源：http://baike.fktsv.cn/Article/details/grrftninm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.bbcook.cn/Article/details/gxbujcvzm.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.epnwcf.com/Article/details/gjdfsgukp.sHtML

composer require twig/twig
来源：http://wap.bbcook.cn/Article/details/gfavhnepj.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fktsv.cn/Article/details/grxhjuffk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.yfazqb.com/Article/details/guobjoxrr.sHtML

[U79] PHP：静态分析
来源：http://3g.fktsv.cn/Article/details/gpildtbke.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.tarul.cn/Article/details/guvyerpkn.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fktsv.cn/Article/details/gfukpxron.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.yfazqb.com/Article/details/gpyfrfvdt.sHtML

[U81] JS：初始化项目
来源：http://mobile.tarul.cn/Article/details/gwzeawdiq.sHtML

npm init -y;  npm i express
来源：http://www.blog.epnwcf.com/Article/details/gixjvlkhm.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.bbcook.cn/Article/details/gjscarwou.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.tarul.cn/Article/details/ghygxcpnh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.epnwcf.com/Article/details/gielfangf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gcthcqtzj.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.bbcook.cn/Article/details/golwayami.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.sjlbkw.cn/Article/details/gjwibvcml.sHtML

[U85] JS：可选链
来源：http://wap.yfazqb.com/Article/details/gdpmwxczi.sHtML

a?.b?.c
来源：http://www.m.share.bbcook.cn/Article/details/gjechvamk.sHtML

[U86] JS：空值合并
来源：http://www.m.share.epnwcf.com/Article/details/gfjajdhhd.sHtML

a ?? b
来源：http://www.blog.fktsv.cn/Article/details/gvosflkmg.sHtML

[U87] JS：解构默认值
来源：http://mobile.yfazqb.com/Article/details/gvstessyn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.bbcook.cn/Article/details/gvuqhvbbh.sHtML

[U88] JS：对象展开合并
来源：http://mobile.sjlbkw.cn/Article/details/gwqipfksd.sHtML

{ ...a, ...b }
来源：http://3g.vehdjk.com/Article/details/ghpgvlxmn.sHtML

[U89] JS：数组去重
来源：http://wap.bbcook.cn/Article/details/ghucgulpe.sHtML

[...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/ghdvbbdhx.sHtML

[U90] JS：数字数组排序
来源：http://baike.vehdjk.com/Article/details/gnyrqyfim.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gjuhhxlbd.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.vehdjk.com/Article/details/gvviviuvy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.epnwcf.com/Article/details/galhswvie.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gilghtywz.sHtML

structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gfmnbqbib.sHtML

[U93] JS：模板字符串
来源：http://wap.bbcook.cn/Article/details/ghcklqtpj.sHtML

`共 ${n} 条`
来源：http://read.share.sjlbkw.cn/Article/details/gxrdanzxg.sHtML

[U94] JS：箭头函数
来源：http://baike.vehdjk.com/Article/details/gqjfezbvc.sHtML

const double = x => x * 2;
来源：http://www.m.share.epnwcf.com/Article/details/gsebajemp.sHtML

[U95] JS：Promise 包装
来源：http://blog.fktsv.cn/Article/details/ghydivugg.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.bbcook.cn/Article/details/gwmwacalk.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fktsv.cn/Article/details/gymldritl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gfjazqgrc.sHtML

[U97] JS：并发请求
来源：http://www.blog.bbcook.cn/Article/details/gatkyfwdp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gzlziowtv.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.bbcook.cn/Article/details/goebdzhhs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fktsv.cn/Article/details/govefrbkt.sHtML

[U99] JS：事件监听
来源：http://m.share.tarul.cn/Article/details/gsnkaqzqk.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fktsv.cn/Article/details/grtjmdsix.sHtML

[U100] JS：DOM 查询
来源：http://blog.vehdjk.com/Article/details/gntlwbfix.sHtML

document.querySelector(".item")
来源：http://www.share.bbcook.cn/Article/details/gcykgwmdn.sHtML

[U101] JS：classList 操作
来源：http://wap.tarul.cn/Article/details/gggxizodh.sHtML

el.classList.toggle("active")
来源：http://www.blog.sjlbkw.cn/Article/details/gcfuslfhw.sHtML

[U102] JS：本地存储
来源：http://www.share.sjlbkw.cn/Article/details/gwrcxtqto.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fktsv.cn/Article/details/gnuhgrizj.sHtML

[U103] JS：定时器
来源：http://mobile.vehdjk.com/Article/details/gqsmeymor.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.tarul.cn/Article/details/gditjyggr.sHtML

[U104] JS：防抖
来源：http://3g.fktsv.cn/Article/details/gtpkggtxk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gkioexskf.sHtML

[U105] JS：节流
来源：http://m.share.tarul.cn/Article/details/gcnivazop.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.sjlbkw.cn/Article/details/gemmgbjwn.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gecugkanc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.epnwcf.com/Article/details/gtqquklzw.sHtML

[U107] JS：数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/ggztxpcyn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gwmfemwhm.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gfoxuoncc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.epnwcf.com/Article/details/giubgabxk.sHtML

[U109] JS：数组分组
来源：http://m.share.bbcook.cn/Article/details/gnataokjh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/gsppoxtcp.sHtML

[U110] JS：数组分块
来源：http://blog.tarul.cn/Article/details/gyndkhpll.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.sjlbkw.cn/Article/details/gkprijwhs.sHtML

[U111] JS：对象转 Map
来源：http://www.share.epnwcf.com/Article/details/gkikfwggg.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fktsv.cn/Article/details/gpurasevu.sHtML

[U112] JS：字符串补位
来源：http://m.share.sjlbkw.cn/Article/details/gjjhgrhas.sHtML

"7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gevfpmhwf.sHtML

[U113] JS：正则替换全部
来源：http://m.share.sjlbkw.cn/Article/details/gmypldems.sHtML

s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gptksdnjq.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fktsv.cn/Article/details/guajsirky.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.yfazqb.com/Article/details/ghgnfnniv.sHtML

[U115] JS：生成 UUID
来源：http://mobile.sjlbkw.cn/Article/details/gqfrcpcir.sHtML

crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gqsmvbuoa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.vehdjk.com/Article/details/gcdrffaia.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gafvkwwbq.sHtML

[U117] JS：单元测试
来源：http://www.m.share.yfazqb.com/Article/details/gkohdsqar.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.bbcook.cn/Article/details/gapukykgq.sHtML

[U118] JS：开发服务器
来源：http://blog.sjlbkw.cn/Article/details/gdncfcord.sHtML

npm i -D vite;  npx vite
来源：http://www.share.yfazqb.com/Article/details/gfzjcjjrj.sHtML

[U119] JS：生产构建
来源：http://www.m.share.vehdjk.com/Article/details/gstlsccvo.sHtML

npx vite build
来源：http://www.blog.fktsv.cn/Article/details/gpeudwxpf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.yfazqb.com/Article/details/gbsthzjsl.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.vehdjk.com/Article/details/gqsuknsrd.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxhwfxpgu.sHtML

统计汇总
来源：http://www.blog.yfazqb.com/Article/details/ghvlnaieo.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gtdevgmuh.sHtML

按语言统计（条）：
来源：http://baike.sjlbkw.cn/Article/details/grkkeueva.sHtML

Python ......... 252
来源：http://www.share.epnwcf.com/Article/details/gcphllpol.sHtML

PHP ............ 252
来源：http://www.m.share.sjlbkw.cn/Article/details/ggggotwht.sHtML

JavaScript ..... 252
来源：http://read.share.bbcook.cn/Article/details/ghbmguyyt.sHtML

TypeScript ..... 212
来源：http://3g.epnwcf.com/Article/details/gtpiedxzg.sHtML

Java ........... 212
来源：http://baike.tarul.cn/Article/details/gonfucxvf.sHtML

Go ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gbyjprunc.sHtML

Ruby ........... 212
来源：http://m.share.yfazqb.com/Article/details/grddoojon.sHtML

C# ............. 212
来源：http://blog.tarul.cn/Article/details/gmiixatyi.sHtML

C .............. 30
来源：http://www.m.share.bbcook.cn/Article/details/glgmxdaxy.sHtML

C++ ............ 30
来源：http://3g.fktsv.cn/Article/details/gejoagmmd.sHtML

SQL ............ 90
来源：http://wap.epnwcf.com/Article/details/ghrkcejhf.sHtML

Bash ........... 80
来源：http://www.share.vehdjk.com/Article/details/givzlpuws.sHtML

Kotlin ......... 15
来源：http://wap.yfazqb.com/Article/details/gvjbnpwxb.sHtML

Swift .......... 15
来源：http://blog.sjlbkw.cn/Article/details/gmurtsmiq.sHtML

Lua ............ 10
来源：http://read.share.vehdjk.com/Article/details/gimnhlavm.sHtML

Perl ........... 10
来源：http://m.share.vehdjk.com/Article/details/gurcikmuv.sHtML

Scala .......... 10
来源：http://wap.yfazqb.com/Article/details/gdbgukklz.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gyqhnmxgu.sHtML

合计 ........... 2106 条
来源：http://blog.vehdjk.com/Article/details/ghjazupvc.sHtML

按章节统计：
来源：http://baike.yfazqb.com/Article/details/guyyuofse.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/ghevmqnfd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/ggbvtalbh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/gdynvudmg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/gxnflnycl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.yfazqb.com/Article/details/gzfstqlac.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.epnwcf.com/Article/details/gcxmrazdm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.vehdjk.com/Article/details/gnuzhokjc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gmebncevs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gdcekvabj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fktsv.cn/Article/details/gxrannljz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gjgyzbrhe.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/guotwdqfb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/ggzbsvlij.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fktsv.cn/Article/details/ghqbxxcqs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fktsv.cn/Article/details/grmvhcstx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gcyvsylca.sHtML

Q SQL 专题                              90
来源：http://read.share.epnwcf.com/Article/details/gjrhdkcko.sHtML

R Bash 专题                             80
来源：http://m.share.tarul.cn/Article/details/ghtxsbxne.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.vehdjk.com/Article/details/gfdpdvwjo.sHtML

T 其他语言补充                          60
来源：http://www.share.bbcook.cn/Article/details/gxxgvhoqg.sHtML

U 高频实用片段                         120
来源：http://baike.sjlbkw.cn/Article/details/gbjppvrhg.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gnsheutkr.sHtML

合计                                  2106 条
来源：http://baike.vehdjk.com/Article/details/gazljcrex.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/givxugnmw.sHtML

使用提醒
来源：http://mobile.fktsv.cn/Article/details/gfibjufyf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gcbyvmmkb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.sjlbkw.cn/Article/details/gnyowumed.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.epnwcf.com/Article/details/goqhzggwn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.vehdjk.com/Article/details/gsrsxraok.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.yfazqb.com/Article/details/goehpuhha.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.sjlbkw.cn/Article/details/gpsuncqps.sHtML

—— 文件结束 ——
来源：http://blog.fktsv.cn/Article/details/gyiketuxd.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkafiumzs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.yfazqb.com/Article/details/gxuqxebwm.sHtML

Common Programming Examples Cheat Book
来源：http://3g.sjlbkw.cn/Article/details/gmgurubfe.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/garqihcie.sHtML

【收录内容】
来源：http://www.m.share.bbcook.cn/Article/details/gujsocdqk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fktsv.cn/Article/details/gonuxzltj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.sjlbkw.cn/Article/details/goxywigro.sHtML

SQL · Bash · C · C++
来源：http://3g.yfazqb.com/Article/details/ghkgpoduw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.vehdjk.com/Article/details/gijwcxdir.sHtML

【使用说明】
来源：http://www.blog.epnwcf.com/Article/details/gavctktya.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.sjlbkw.cn/Article/details/gvmattoom.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.bbcook.cn/Article/details/ghjllipmz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.sjlbkw.cn/Article/details/ghhrwdkqi.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.vehdjk.com/Article/details/gpvgbgnoq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.epnwcf.com/Article/details/gxyhakcnc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.bbcook.cn/Article/details/giijwpygi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.tarul.cn/Article/details/gbujvohdx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.sjlbkw.cn/Article/details/gsfaqugkn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.vehdjk.com/Article/details/gnmhgffex.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.vehdjk.com/Article/details/gasszdjsp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.bbcook.cn/Article/details/gnuacwrin.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fktsv.cn/Article/details/gtjyxgfoq.sHtML

【文件统计】
来源：http://www.blog.vehdjk.com/Article/details/ginuiwdyy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.sjlbkw.cn/Article/details/gjeixoury.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gppgufony.sHtML

目  录
来源：http://www.share.vehdjk.com/Article/details/gwgmtjhkk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gknwliqit.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.vehdjk.com/Article/details/gnshzcxof.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/gedvfowkd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.sjlbkw.cn/Article/details/gqrufztsg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.epnwcf.com/Article/details/ggfkndhkp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.sjlbkw.cn/Article/details/gqanudmty.sHtML


<!-- 参考信息 -->