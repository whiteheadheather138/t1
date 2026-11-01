代发 wailian999

[U17] Py：初始化日志
来源：http://baike.sjlbkw.cn/Article/details/gfyfevbhg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.yfazqb.com/Article/details/gaprnozha.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fktsv.cn/Article/details/gokeebrtg.sHtML

pat = re.compile(r"\d+")
来源：http://wap.bbcook.cn/Article/details/gulzxjvro.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.epnwcf.com/Article/details/gjbqtuvlx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.yfazqb.com/Article/details/gdxsvciiw.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/gtpfwfeit.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fktsv.cn/Article/details/gmtyfiogz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.bbcook.cn/Article/details/gruqhulzu.sHtML

@contextlib.contextmanager
来源：http://www.m.share.epnwcf.com/Article/details/gdtcrjopb.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.bbcook.cn/Article/details/geedmcugi.sHtML

list(zip(*m))
来源：http://m.share.tarul.cn/Article/details/gxffchtog.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fktsv.cn/Article/details/gasffjtbj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.bbcook.cn/Article/details/glgrjbkuw.sHtML

[U24] Py：路径操作
来源：http://www.blog.yfazqb.com/Article/details/gasjotcuy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/golvjwitk.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fktsv.cn/Article/details/gqcgzboyn.sHtML

csv.DictReader(f)
来源：http://mobile.bbcook.cn/Article/details/gaojfypzp.sHtML

[U26] Py：并发下载
来源：http://3g.epnwcf.com/Article/details/gnobjvnvt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.tarul.cn/Article/details/ghbqfqsjx.sHtML

[U27] Py：异步 HTTP
来源：http://3g.vehdjk.com/Article/details/gljzzvdox.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.epnwcf.com/Article/details/gkbrssyob.sHtML

[U28] Py：类型别名
来源：http://mobile.vehdjk.com/Article/details/gqskwzhtu.sHtML

UserId = int
来源：http://www.m.share.bbcook.cn/Article/details/glhaziato.sHtML

[U29] Py：属性校验
来源：http://www.share.bbcook.cn/Article/details/gttedpxgc.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.vehdjk.com/Article/details/gltywuufh.sHtML

[U30] Py：数据类
来源：http://mobile.sjlbkw.cn/Article/details/gomrkhadk.sHtML

@dataclass(slots=True)
来源：http://www.m.share.yfazqb.com/Article/details/gkkmswquj.sHtML

[U31] Py：单测
来源：http://m.share.tarul.cn/Article/details/grdvewzqq.sHtML

python -m pytest -q
来源：http://www.m.share.epnwcf.com/Article/details/gatcuuljz.sHtML

[U32] Py：代码格式化
来源：http://read.share.tarul.cn/Article/details/gmnrgvurq.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.tarul.cn/Article/details/gdvfyrnbc.sHtML

[U33] Py：打包发布
来源：http://www.blog.vehdjk.com/Article/details/gnoyidlmh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.bbcook.cn/Article/details/gqvxwjzqk.sHtML

[U34] Py：判断编码
来源：http://3g.sjlbkw.cn/Article/details/gvjhzuzvg.sHtML

chardet.detect(raw)
来源：http://baike.yfazqb.com/Article/details/gbessoteg.sHtML

[U35] Py：发送邮件
来源：http://m.share.yfazqb.com/Article/details/gesselgbw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fktsv.cn/Article/details/gvcqgpyns.sHtML

[U36] Py：定时任务
来源：http://read.share.yfazqb.com/Article/details/gqyivmqyr.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.tarul.cn/Article/details/gsmhhtsvs.sHtML

[U37] Py：读写 Excel
来源：http://m.share.tarul.cn/Article/details/gcxwalfwc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.vehdjk.com/Article/details/gowrosxes.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.yfazqb.com/Article/details/gaocvueld.sHtML

Path(__file__).resolve().parent
来源：http://read.share.yfazqb.com/Article/details/geydrojsj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.yfazqb.com/Article/details/gjpnipjbu.sHtML

sys.stdout.isatty()
来源：http://m.share.sjlbkw.cn/Article/details/gpbbzrskc.sHtML

[U40] Py：打印到标准错误
来源：http://blog.sjlbkw.cn/Article/details/glsmynrhv.sHtML

print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gtusfxgjo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.sjlbkw.cn/Article/details/gxkzuymzu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.bbcook.cn/Article/details/gcizcrfat.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpnfczrc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.sjlbkw.cn/Article/details/ggennpsdc.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fktsv.cn/Article/details/gowljejdh.sHtML

namespace App\Http;
来源：http://wap.epnwcf.com/Article/details/ggxxxlnae.sHtML

[U44] PHP：开启严格类型
来源：http://baike.yfazqb.com/Article/details/gghhwhnmp.sHtML

declare(strict_types=1);
来源：http://blog.fktsv.cn/Article/details/gtuxjunlp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.epnwcf.com/Article/details/gmcizbelc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gznuvitct.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.epnwcf.com/Article/details/ggxgkjqmv.sHtML

?string $name = null
来源：http://www.blog.bbcook.cn/Article/details/gblnmxbyn.sHtML

[U47] PHP：联合类型
来源：http://mobile.bbcook.cn/Article/details/gvjbnwnev.sHtML

int|string $id
来源：http://www.share.fktsv.cn/Article/details/gdsehkocq.sHtML

[U48] PHP：纯枚举
来源：http://blog.epnwcf.com/Article/details/gybrzfovk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gaafgaldb.sHtML

[U49] PHP：只读属性
来源：http://www.share.tarul.cn/Article/details/gjcrkmfwy.sHtML

public readonly string $name
来源：http://baike.fktsv.cn/Article/details/gbczcudqf.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.sjlbkw.cn/Article/details/gcogywdfi.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.vehdjk.com/Article/details/gaauhborz.sHtML

[U51] PHP：数组解构
来源：http://3g.tarul.cn/Article/details/goqrpdxtd.sHtML

[$a, $b] = $arr;
来源：http://m.share.epnwcf.com/Article/details/gnvyawdko.sHtML

[U52] PHP：箭头函数
来源：http://blog.fktsv.cn/Article/details/geesrtjxj.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.bbcook.cn/Article/details/gwrjpfysh.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.bbcook.cn/Article/details/givejzaly.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.yfazqb.com/Article/details/ghsgisjjr.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fktsv.cn/Article/details/gjgeqwtjx.sHtML

$obj?->method()
来源：http://wap.fktsv.cn/Article/details/gfhonhwbf.sHtML

[U55] PHP：match 表达式
来源：http://blog.bbcook.cn/Article/details/gbllfsuza.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.epnwcf.com/Article/details/gbzbnzadj.sHtML

[U56] PHP：命名参数
来源：http://3g.bbcook.cn/Article/details/gugsglquk.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gpmwmfbyk.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/goybslvve.sHtML

"值: {$a}"
来源：http://www.share.tarul.cn/Article/details/gbslsxqiz.sHtML

[U58] PHP：数组三件套
来源：http://wap.sjlbkw.cn/Article/details/gghyochds.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.epnwcf.com/Article/details/gqdwdollg.sHtML

[U59] PHP：自定义排序
来源：http://wap.fktsv.cn/Article/details/gylhljhgk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.bbcook.cn/Article/details/gqsfxbyld.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.bbcook.cn/Article/details/gesjyixbw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.vehdjk.com/Article/details/gniknebhq.sHtML

[U61] PHP：正则
来源：http://baike.tarul.cn/Article/details/gfbtpdmed.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gcrvhxooo.sHtML

[U62] PHP：日期对象
来源：http://m.share.epnwcf.com/Article/details/gglhgiexn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.sjlbkw.cn/Article/details/gdisfouun.sHtML

[U63] PHP：文件读写
来源：http://read.share.vehdjk.com/Article/details/gcgxqapcf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fktsv.cn/Article/details/gwuzihqkq.sHtML

[U64] PHP：目录遍历
来源：http://baike.bbcook.cn/Article/details/gqehoxlqr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.bbcook.cn/Article/details/gkymkpvbg.sHtML

[U65] PHP：会话
来源：http://wap.sjlbkw.cn/Article/details/grahliuql.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.yfazqb.com/Article/details/guvcfuusi.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.vehdjk.com/Article/details/gicuysepj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fktsv.cn/Article/details/gtofsuggw.sHtML

[U67] PHP：处理文件上传
来源：http://wap.bbcook.cn/Article/details/gapjtufei.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.epnwcf.com/Article/details/ghqianace.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.yfazqb.com/Article/details/gojwfpxub.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.bbcook.cn/Article/details/glavwfzfm.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.yfazqb.com/Article/details/gcfspwwqq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.tarul.cn/Article/details/grnwspcvx.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fktsv.cn/Article/details/gjzreamji.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/gmhiwhcck.sHtML

[U71] PHP：抛出异常
来源：http://blog.tarul.cn/Article/details/gbsixhboe.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.tarul.cn/Article/details/gqqtccaee.sHtML

[U72] PHP：写错误日志
来源：http://blog.fktsv.cn/Article/details/gzgwzqgme.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.sjlbkw.cn/Article/details/gilqlanct.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.tarul.cn/Article/details/gaetoqyng.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.tarul.cn/Article/details/grxqlfump.sHtML

[U74] PHP：读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/gkesmpzdp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.bbcook.cn/Article/details/gozetgpmw.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fktsv.cn/Article/details/goabplnvp.sHtML

composer require psr/container
来源：http://mobile.sjlbkw.cn/Article/details/gijuzdcia.sHtML

[U76] PHP：简单路由
来源：http://read.share.yfazqb.com/Article/details/gnigwnyrv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fktsv.cn/Article/details/gssbyyigl.sHtML

[U77] PHP：模板渲染
来源：http://wap.epnwcf.com/Article/details/gseujfxmu.sHtML

composer require twig/twig
来源：http://read.share.sjlbkw.cn/Article/details/gdgmhdyrm.sHtML

[U78] PHP：单元测试
来源：http://blog.vehdjk.com/Article/details/gnqchjnnv.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.yfazqb.com/Article/details/ghvnuekil.sHtML

[U79] PHP：静态分析
来源：http://read.share.tarul.cn/Article/details/gedtprupu.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.vehdjk.com/Article/details/gloqovwkc.sHtML

[U80] PHP：代码规范修复
来源：http://wap.epnwcf.com/Article/details/gwolsalfz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.vehdjk.com/Article/details/gxxwwqwgr.sHtML

[U81] JS：初始化项目
来源：http://wap.tarul.cn/Article/details/giztdqimp.sHtML

npm init -y;  npm i express
来源：http://read.share.tarul.cn/Article/details/gypikpsbs.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fktsv.cn/Article/details/gfwqzfwts.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.epnwcf.com/Article/details/gkrtkmpej.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fktsv.cn/Article/details/ghqhgqvii.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gxtcfurzv.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.vehdjk.com/Article/details/gknyqczli.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.tarul.cn/Article/details/grtbwdleu.sHtML

[U85] JS：可选链
来源：http://wap.vehdjk.com/Article/details/gxiliarsg.sHtML

a?.b?.c
来源：http://read.share.vehdjk.com/Article/details/guoxunqhm.sHtML

[U86] JS：空值合并
来源：http://m.share.tarul.cn/Article/details/gicxrxdbg.sHtML

a ?? b
来源：http://m.share.fktsv.cn/Article/details/ggrdrajqc.sHtML

[U87] JS：解构默认值
来源：http://read.share.bbcook.cn/Article/details/giohtyndc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.bbcook.cn/Article/details/gosgygkxi.sHtML

[U88] JS：对象展开合并
来源：http://mobile.tarul.cn/Article/details/gasuexfef.sHtML

{ ...a, ...b }
来源：http://m.share.yfazqb.com/Article/details/gaaoaevqp.sHtML

[U89] JS：数组去重
来源：http://www.m.share.tarul.cn/Article/details/gkfikuvaf.sHtML

[...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gdqmnodxf.sHtML

[U90] JS：数字数组排序
来源：http://baike.sjlbkw.cn/Article/details/goajcxbvy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gtpvkfqzo.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fktsv.cn/Article/details/gbsekmwbu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.epnwcf.com/Article/details/goblsvitu.sHtML

[U92] JS：深拷贝
来源：http://mobile.yfazqb.com/Article/details/gbpoivoqn.sHtML

structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gamalfoym.sHtML

[U93] JS：模板字符串
来源：http://blog.sjlbkw.cn/Article/details/gsixmckoa.sHtML

`共 ${n} 条`
来源：http://read.share.tarul.cn/Article/details/gkfrjmwoo.sHtML

[U94] JS：箭头函数
来源：http://wap.bbcook.cn/Article/details/gqatqzuer.sHtML

const double = x => x * 2;
来源：http://3g.bbcook.cn/Article/details/gvaqdtiac.sHtML

[U95] JS：Promise 包装
来源：http://blog.bbcook.cn/Article/details/gxlbywxuu.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.epnwcf.com/Article/details/gkvptrcvz.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.sjlbkw.cn/Article/details/gorjmvdus.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/geqgjwutu.sHtML

[U97] JS：并发请求
来源：http://www.m.share.epnwcf.com/Article/details/gundrocfx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gqxdcedod.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.vehdjk.com/Article/details/gqyaexhcr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.sjlbkw.cn/Article/details/gfqxrruui.sHtML

[U99] JS：事件监听
来源：http://mobile.tarul.cn/Article/details/gkxeelnpw.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.sjlbkw.cn/Article/details/gkfobopfx.sHtML

[U100] JS：DOM 查询
来源：http://m.share.sjlbkw.cn/Article/details/gnvnelxos.sHtML

document.querySelector(".item")
来源：http://wap.epnwcf.com/Article/details/ghbmlzmdt.sHtML

[U101] JS：classList 操作
来源：http://m.share.tarul.cn/Article/details/gltqwbmop.sHtML

el.classList.toggle("active")
来源：http://m.share.tarul.cn/Article/details/ghkatbvva.sHtML

[U102] JS：本地存储
来源：http://wap.tarul.cn/Article/details/gtycmxblh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.yfazqb.com/Article/details/gudlmeugd.sHtML

[U103] JS：定时器
来源：http://www.blog.sjlbkw.cn/Article/details/geoolyodk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fktsv.cn/Article/details/gmtpisgzn.sHtML

[U104] JS：防抖
来源：http://www.blog.yfazqb.com/Article/details/giqakzbgf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gvalwtlaj.sHtML

[U105] JS：节流
来源：http://mobile.bbcook.cn/Article/details/gfutzpjcm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.yfazqb.com/Article/details/gdxvqoxam.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gotovimct.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.sjlbkw.cn/Article/details/glbtjikwe.sHtML

[U107] JS：数字千分位
来源：http://blog.epnwcf.com/Article/details/gudnghujw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fktsv.cn/Article/details/gyzqpvjzh.sHtML

[U108] JS：随机整数
来源：http://3g.epnwcf.com/Article/details/gyxgfbyzd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.epnwcf.com/Article/details/gbeqhjtqc.sHtML

[U109] JS：数组分组
来源：http://www.blog.tarul.cn/Article/details/gknjyujsy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gdkzxtauk.sHtML

[U110] JS：数组分块
来源：http://read.share.tarul.cn/Article/details/guzxwoyvf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.sjlbkw.cn/Article/details/guagsokgo.sHtML

[U111] JS：对象转 Map
来源：http://wap.epnwcf.com/Article/details/gtvrkoins.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fktsv.cn/Article/details/gnzzzfbed.sHtML

[U112] JS：字符串补位
来源：http://www.blog.tarul.cn/Article/details/gjjeacnig.sHtML

"7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gtxacergj.sHtML

[U113] JS：正则替换全部
来源：http://baike.bbcook.cn/Article/details/gffywctoj.sHtML

s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gjdjtjsyb.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.epnwcf.com/Article/details/gtdmufrce.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/gqlwrapzj.sHtML

[U115] JS：生成 UUID
来源：http://blog.bbcook.cn/Article/details/gredpajlz.sHtML

crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gpnwwlocw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fktsv.cn/Article/details/gjnbnjuuw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.sjlbkw.cn/Article/details/gjvrofpnv.sHtML

[U117] JS：单元测试
来源：http://www.share.sjlbkw.cn/Article/details/gsibaaxkz.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.bbcook.cn/Article/details/gbtsdbarr.sHtML

[U118] JS：开发服务器
来源：http://3g.bbcook.cn/Article/details/gztcpsdbq.sHtML

npm i -D vite;  npx vite
来源：http://mobile.yfazqb.com/Article/details/gxskqgdbe.sHtML

[U119] JS：生产构建
来源：http://www.blog.bbcook.cn/Article/details/gozipiqcy.sHtML

npx vite build
来源：http://mobile.tarul.cn/Article/details/gabxasael.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.sjlbkw.cn/Article/details/gohouxlaa.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.tarul.cn/Article/details/gvnhhsufi.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gpvtrkiya.sHtML

统计汇总
来源：http://wap.vehdjk.com/Article/details/gkuucnbfd.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glnjgsdzq.sHtML

按语言统计（条）：
来源：http://www.share.bbcook.cn/Article/details/gselpzznh.sHtML

Python ......... 252
来源：http://wap.bbcook.cn/Article/details/gqacuotxn.sHtML

PHP ............ 252
来源：http://www.blog.tarul.cn/Article/details/glxntoiri.sHtML

JavaScript ..... 252
来源：http://blog.epnwcf.com/Article/details/geofaoyaj.sHtML

TypeScript ..... 212
来源：http://m.share.epnwcf.com/Article/details/gyikkggqb.sHtML

Java ........... 212
来源：http://m.share.fktsv.cn/Article/details/gbpobhjig.sHtML

Go ............. 212
来源：http://read.share.yfazqb.com/Article/details/gtdcowzii.sHtML

Ruby ........... 212
来源：http://m.share.fktsv.cn/Article/details/gaojcmcdm.sHtML

C# ............. 212
来源：http://read.share.vehdjk.com/Article/details/gaypewxwr.sHtML

C .............. 30
来源：http://wap.fktsv.cn/Article/details/gvqygemzn.sHtML

C++ ............ 30
来源：http://baike.tarul.cn/Article/details/gzckfyvyw.sHtML

SQL ............ 90
来源：http://www.share.sjlbkw.cn/Article/details/gfcznxyzl.sHtML

Bash ........... 80
来源：http://blog.fktsv.cn/Article/details/gccfimfgx.sHtML

Kotlin ......... 15
来源：http://wap.fktsv.cn/Article/details/gafubjhql.sHtML

Swift .......... 15
来源：http://wap.bbcook.cn/Article/details/ghobymhsm.sHtML

Lua ............ 10
来源：http://wap.tarul.cn/Article/details/gbbjjrpbw.sHtML

Perl ........... 10
来源：http://www.share.fktsv.cn/Article/details/glqeqjwif.sHtML

Scala .......... 10
来源：http://baike.sjlbkw.cn/Article/details/groimqydq.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/glqmihydm.sHtML

合计 ........... 2106 条
来源：http://www.m.share.bbcook.cn/Article/details/gjaslvkeh.sHtML

按章节统计：
来源：http://blog.fktsv.cn/Article/details/ghhmpdget.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fktsv.cn/Article/details/gkaztvvaj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/grcuopqmp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/glvhfngyj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gnmxhigwi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.yfazqb.com/Article/details/gdemqtevu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.vehdjk.com/Article/details/gqjhenidr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gdxopzybu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.yfazqb.com/Article/details/gxjphiwoc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/ghmtnmori.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.epnwcf.com/Article/details/gxcamgcqw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gnhcbwnla.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/goangnwdr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/giinhxvjx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.sjlbkw.cn/Article/details/glpyetcdx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.tarul.cn/Article/details/gozswenkp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gchgnoywr.sHtML

Q SQL 专题                              90
来源：http://m.share.sjlbkw.cn/Article/details/gyifxjymg.sHtML

R Bash 专题                             80
来源：http://m.share.yfazqb.com/Article/details/gqfmpcpyl.sHtML

S C / C++ 专题                          60
来源：http://blog.sjlbkw.cn/Article/details/glegzfjij.sHtML

T 其他语言补充                          60
来源：http://baike.tarul.cn/Article/details/glhfapmbp.sHtML

U 高频实用片段                         120
来源：http://mobile.tarul.cn/Article/details/gjryrbmsc.sHtML

------------------------------------
来源：http://3g.fktsv.cn/Article/details/gofwoydvs.sHtML

合计                                  2106 条
来源：http://blog.epnwcf.com/Article/details/gprpgzdpj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gyrezwpux.sHtML

使用提醒
来源：http://read.share.epnwcf.com/Article/details/gdgobcfnr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gkbguvjsw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.sjlbkw.cn/Article/details/gagjouuge.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.tarul.cn/Article/details/gvwjdwdmj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.yfazqb.com/Article/details/gvmvodnvx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.epnwcf.com/Article/details/gxamlqfbh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fktsv.cn/Article/details/gjrwhavdo.sHtML

—— 文件结束 ——
来源：http://www.share.tarul.cn/Article/details/gngjiptrb.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gujccnkwu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.bbcook.cn/Article/details/gehrquojl.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.vehdjk.com/Article/details/glbpjonmo.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbkvybpdp.sHtML

【收录内容】
来源：http://3g.epnwcf.com/Article/details/gorqatxzs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fktsv.cn/Article/details/gijpofgpa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.yfazqb.com/Article/details/gbrfdmpuc.sHtML

SQL · Bash · C · C++
来源：http://blog.epnwcf.com/Article/details/gglkxgbgc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmtrxqic.sHtML

【使用说明】
来源：http://read.share.yfazqb.com/Article/details/gumluevch.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.yfazqb.com/Article/details/geqlknlpm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.tarul.cn/Article/details/gshlcsckb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.vehdjk.com/Article/details/goersvdhr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.bbcook.cn/Article/details/gsbykldtu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.sjlbkw.cn/Article/details/gppqdbpbe.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fktsv.cn/Article/details/gdwindgoj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.yfazqb.com/Article/details/gzywwivsd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.epnwcf.com/Article/details/gcpsqxmug.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.yfazqb.com/Article/details/gtwcfpcuj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.bbcook.cn/Article/details/gwvtleqkp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.bbcook.cn/Article/details/gvursauvq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fktsv.cn/Article/details/gtroddoof.sHtML

【文件统计】
来源：http://3g.epnwcf.com/Article/details/gepkidehx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.vehdjk.com/Article/details/gnsgnkmrx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gbhetguhj.sHtML

目  录
来源：http://www.m.share.bbcook.cn/Article/details/gtkyqhcca.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gkpzzajnv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.vehdjk.com/Article/details/gnlambpsa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/geipffwfx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.sjlbkw.cn/Article/details/geiidxztf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.bbcook.cn/Article/details/gbggqybrt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fktsv.cn/Article/details/gjyafhdqv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.epnwcf.com/Article/details/gujkcojvi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/gmfupvinx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.epnwcf.com/Article/details/gpbevwmwv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gbdmyfprl.sHtML


<!-- 参考信息 -->