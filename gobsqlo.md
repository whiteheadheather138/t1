代发 wailian999

[U17] Py：初始化日志
来源：http://www.m.share.epnwcf.com/Article/details/ghozklyxe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fktsv.cn/Article/details/gtgpomhtw.sHtML

[U18] Py：预编译正则
来源：http://mobile.vehdjk.com/Article/details/gfszifpqd.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/gdwvauurs.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fktsv.cn/Article/details/grtbnmlck.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.tarul.cn/Article/details/gbgjkikxa.sHtML

[U20] Py：缓存函数结果
来源：http://blog.epnwcf.com/Article/details/gmhkyavaf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.sjlbkw.cn/Article/details/gqozkvwtw.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.sjlbkw.cn/Article/details/gyqpsfdfy.sHtML

@contextlib.contextmanager
来源：http://baike.vehdjk.com/Article/details/gieqkgmov.sHtML

[U22] Py：矩阵转置
来源：http://3g.bbcook.cn/Article/details/gewdmorbi.sHtML

list(zip(*m))
来源：http://m.share.tarul.cn/Article/details/gugvmkzsm.sHtML

[U23] Py：分块读取大文件
来源：http://wap.epnwcf.com/Article/details/glgjgeagn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.sjlbkw.cn/Article/details/ghacypjgz.sHtML

[U24] Py：路径操作
来源：http://www.blog.sjlbkw.cn/Article/details/gwnnpxwdm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gjjeponbj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.tarul.cn/Article/details/gmbztbobe.sHtML

csv.DictReader(f)
来源：http://www.blog.sjlbkw.cn/Article/details/gqxqikjpl.sHtML

[U26] Py：并发下载
来源：http://read.share.yfazqb.com/Article/details/gvxuljnzh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.bbcook.cn/Article/details/gwvrrlqfx.sHtML

[U27] Py：异步 HTTP
来源：http://blog.epnwcf.com/Article/details/gxprrpffk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fktsv.cn/Article/details/gyhtsjwbm.sHtML

[U28] Py：类型别名
来源：http://mobile.yfazqb.com/Article/details/gbzjtapdr.sHtML

UserId = int
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfeeamht.sHtML

[U29] Py：属性校验
来源：http://mobile.sjlbkw.cn/Article/details/gnwnywyqd.sHtML

@property 与 @x.setter 配合
来源：http://m.share.bbcook.cn/Article/details/gqgjwdewa.sHtML

[U30] Py：数据类
来源：http://read.share.tarul.cn/Article/details/gsqntdzrs.sHtML

@dataclass(slots=True)
来源：http://read.share.bbcook.cn/Article/details/gffvbsewy.sHtML

[U31] Py：单测
来源：http://blog.epnwcf.com/Article/details/gxsbibxep.sHtML

python -m pytest -q
来源：http://mobile.vehdjk.com/Article/details/gfvadxtvr.sHtML

[U32] Py：代码格式化
来源：http://3g.bbcook.cn/Article/details/gpjhrvzvj.sHtML

ruff format . && ruff check --fix .
来源：http://blog.sjlbkw.cn/Article/details/gbaaefxrw.sHtML

[U33] Py：打包发布
来源：http://mobile.fktsv.cn/Article/details/gdghnypmm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.tarul.cn/Article/details/gawcqgzhb.sHtML

[U34] Py：判断编码
来源：http://www.m.share.vehdjk.com/Article/details/gruohuowc.sHtML

chardet.detect(raw)
来源：http://read.share.vehdjk.com/Article/details/ggkfwmohk.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.epnwcf.com/Article/details/gyyqmabzv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.bbcook.cn/Article/details/gdlqexevl.sHtML

[U36] Py：定时任务
来源：http://m.share.epnwcf.com/Article/details/grldqlbal.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.vehdjk.com/Article/details/gqyamisqo.sHtML

[U37] Py：读写 Excel
来源：http://read.share.yfazqb.com/Article/details/gnxpfqizv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.tarul.cn/Article/details/gnfpycfya.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.tarul.cn/Article/details/giutxcvrf.sHtML

Path(__file__).resolve().parent
来源：http://mobile.vehdjk.com/Article/details/gpsdeejul.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.tarul.cn/Article/details/gsjqgpjob.sHtML

sys.stdout.isatty()
来源：http://read.share.vehdjk.com/Article/details/godftparl.sHtML

[U40] Py：打印到标准错误
来源：http://blog.tarul.cn/Article/details/giirrxppb.sHtML

print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/gpenmindr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.vehdjk.com/Article/details/gktuuvbdt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.yfazqb.com/Article/details/gtemeenlb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.tarul.cn/Article/details/goakkakir.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.vehdjk.com/Article/details/ggqlffoix.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fktsv.cn/Article/details/gwjltkfqi.sHtML

namespace App\Http;
来源：http://mobile.vehdjk.com/Article/details/gwhlrispq.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.epnwcf.com/Article/details/gaqejzobp.sHtML

declare(strict_types=1);
来源：http://3g.sjlbkw.cn/Article/details/gzfopeuqd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.yfazqb.com/Article/details/guxyapwhi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gouknclrh.sHtML

[U46] PHP：可空类型
来源：http://www.blog.epnwcf.com/Article/details/gaxdiewpm.sHtML

?string $name = null
来源：http://blog.sjlbkw.cn/Article/details/gyibsllvj.sHtML

[U47] PHP：联合类型
来源：http://m.share.bbcook.cn/Article/details/gcpusbivv.sHtML

int|string $id
来源：http://wap.epnwcf.com/Article/details/gapuzvege.sHtML

[U48] PHP：纯枚举
来源：http://3g.tarul.cn/Article/details/gjcjhjjvq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fktsv.cn/Article/details/gvljkaelb.sHtML

[U49] PHP：只读属性
来源：http://blog.yfazqb.com/Article/details/gailbjppn.sHtML

public readonly string $name
来源：http://read.share.bbcook.cn/Article/details/gbdpjbfhb.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.vehdjk.com/Article/details/gawujqwvu.sHtML

public function __construct(private int $id) {}
来源：http://baike.sjlbkw.cn/Article/details/gbvmkktup.sHtML

[U51] PHP：数组解构
来源：http://www.blog.sjlbkw.cn/Article/details/gugfvlmtl.sHtML

[$a, $b] = $arr;
来源：http://blog.fktsv.cn/Article/details/gidmzbiff.sHtML

[U52] PHP：箭头函数
来源：http://read.share.tarul.cn/Article/details/gdckkcofs.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fktsv.cn/Article/details/gwgfqvkrc.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.tarul.cn/Article/details/gruymffsd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.yfazqb.com/Article/details/gbxnelbbs.sHtML

[U54] PHP：空安全调用
来源：http://www.share.bbcook.cn/Article/details/gyrecxnxc.sHtML

$obj?->method()
来源：http://read.share.fktsv.cn/Article/details/gazfifbnh.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fktsv.cn/Article/details/ggwvvkybe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.tarul.cn/Article/details/gxiohpqvq.sHtML

[U56] PHP：命名参数
来源：http://blog.epnwcf.com/Article/details/gxnikqqut.sHtML

f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gkqquvmko.sHtML

[U57] PHP：字符串插值
来源：http://baike.yfazqb.com/Article/details/gznighxiy.sHtML

"值: {$a}"
来源：http://baike.sjlbkw.cn/Article/details/gbygrtkxx.sHtML

[U58] PHP：数组三件套
来源：http://www.share.bbcook.cn/Article/details/gwslblmuj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.vehdjk.com/Article/details/gxfneylea.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fktsv.cn/Article/details/gulcjeaar.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.vehdjk.com/Article/details/grhidbmuo.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.epnwcf.com/Article/details/gycfhyuox.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.bbcook.cn/Article/details/ggvdvbhxn.sHtML

[U61] PHP：正则
来源：http://m.share.sjlbkw.cn/Article/details/gypeujzfm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/gpqpbzvzc.sHtML

[U62] PHP：日期对象
来源：http://read.share.bbcook.cn/Article/details/gamhwydhr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.yfazqb.com/Article/details/gbbptecpj.sHtML

[U63] PHP：文件读写
来源：http://baike.epnwcf.com/Article/details/glthdfdch.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.vehdjk.com/Article/details/gpyspvpys.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gekarmppd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.sjlbkw.cn/Article/details/ghqwrpmvv.sHtML

[U65] PHP：会话
来源：http://wap.tarul.cn/Article/details/gqhnmwlbh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fktsv.cn/Article/details/gxpyztqiy.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.sjlbkw.cn/Article/details/gtoozlaqk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.sjlbkw.cn/Article/details/gykkgzmqq.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fktsv.cn/Article/details/gwpmuzrfv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.sjlbkw.cn/Article/details/gnvhmhzxo.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fktsv.cn/Article/details/gpsozdpdu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.sjlbkw.cn/Article/details/ghmiqwadq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.bbcook.cn/Article/details/gixgxsibe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.epnwcf.com/Article/details/gqhmzsuaz.sHtML

[U70] PHP：PDO 事务
来源：http://wap.bbcook.cn/Article/details/gzbolxcws.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.vehdjk.com/Article/details/gpguhuqnq.sHtML

[U71] PHP：抛出异常
来源：http://wap.yfazqb.com/Article/details/gyndhcmvk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gpjqdwblr.sHtML

[U72] PHP：写错误日志
来源：http://mobile.epnwcf.com/Article/details/gwtdkhcev.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fktsv.cn/Article/details/goabzukxz.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.bbcook.cn/Article/details/ghlpwbolz.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.yfazqb.com/Article/details/guqzmeopf.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/geagvrlhm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.sjlbkw.cn/Article/details/glclcojrw.sHtML

[U75] PHP：依赖注入
来源：http://mobile.tarul.cn/Article/details/gdghtybje.sHtML

composer require psr/container
来源：http://www.share.vehdjk.com/Article/details/gxepgidaw.sHtML

[U76] PHP：简单路由
来源：http://3g.fktsv.cn/Article/details/gsyglmvcr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.tarul.cn/Article/details/ghomfktph.sHtML

[U77] PHP：模板渲染
来源：http://wap.yfazqb.com/Article/details/giomxgafj.sHtML

composer require twig/twig
来源：http://m.share.yfazqb.com/Article/details/geznwlvzz.sHtML

[U78] PHP：单元测试
来源：http://blog.yfazqb.com/Article/details/gdkzftajj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fktsv.cn/Article/details/gjgqrgunp.sHtML

[U79] PHP：静态分析
来源：http://baike.yfazqb.com/Article/details/gblwebdtu.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.vehdjk.com/Article/details/gfmjdnkut.sHtML

[U80] PHP：代码规范修复
来源：http://3g.sjlbkw.cn/Article/details/ggcfeeynn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fktsv.cn/Article/details/gzvtqsjcs.sHtML

[U81] JS：初始化项目
来源：http://read.share.yfazqb.com/Article/details/gocaepcpn.sHtML

npm init -y;  npm i express
来源：http://baike.bbcook.cn/Article/details/ghynuydsg.sHtML

[U82] JS：package.json 脚本
来源：http://blog.sjlbkw.cn/Article/details/gpydqerdx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.sjlbkw.cn/Article/details/gznqdhgty.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.yfazqb.com/Article/details/gedkahtgr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/gitllbnsb.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.tarul.cn/Article/details/gsmyboqlp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.epnwcf.com/Article/details/ghpoqhkzu.sHtML

[U85] JS：可选链
来源：http://wap.tarul.cn/Article/details/grnmhxctg.sHtML

a?.b?.c
来源：http://read.share.vehdjk.com/Article/details/gfqyhrlfo.sHtML

[U86] JS：空值合并
来源：http://3g.bbcook.cn/Article/details/gpmvkczzt.sHtML

a ?? b
来源：http://mobile.tarul.cn/Article/details/gaykxrdfe.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.tarul.cn/Article/details/gtfjgabdv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.tarul.cn/Article/details/gmijyouqz.sHtML

[U88] JS：对象展开合并
来源：http://baike.fktsv.cn/Article/details/ghbppuvzy.sHtML

{ ...a, ...b }
来源：http://3g.epnwcf.com/Article/details/gcelfahyj.sHtML

[U89] JS：数组去重
来源：http://baike.tarul.cn/Article/details/gvtdemmox.sHtML

[...new Set(arr)]
来源：http://3g.yfazqb.com/Article/details/gaiaiykaz.sHtML

[U90] JS：数字数组排序
来源：http://3g.epnwcf.com/Article/details/gnjoaqwrp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gejrzgiru.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fktsv.cn/Article/details/ghfemezgk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.yfazqb.com/Article/details/gaknkcckx.sHtML

[U92] JS：深拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gkhtedamx.sHtML

structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gvrnpezcq.sHtML

[U93] JS：模板字符串
来源：http://baike.yfazqb.com/Article/details/grugfjdnd.sHtML

`共 ${n} 条`
来源：http://blog.yfazqb.com/Article/details/grefuaprw.sHtML

[U94] JS：箭头函数
来源：http://www.share.epnwcf.com/Article/details/glevpkbua.sHtML

const double = x => x * 2;
来源：http://mobile.epnwcf.com/Article/details/gahlsmkqv.sHtML

[U95] JS：Promise 包装
来源：http://m.share.tarul.cn/Article/details/ggbxmhouk.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.epnwcf.com/Article/details/gbuqfcqhg.sHtML

[U96] JS：async/await 与异常
来源：http://baike.vehdjk.com/Article/details/gkcckijmp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gbmerdihc.sHtML

[U97] JS：并发请求
来源：http://wap.yfazqb.com/Article/details/gahfkvmxr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/giriytmgi.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.tarul.cn/Article/details/grkgvvhte.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.sjlbkw.cn/Article/details/gqtalavjo.sHtML

[U99] JS：事件监听
来源：http://wap.bbcook.cn/Article/details/gmgnwoeku.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.tarul.cn/Article/details/gjaziodyp.sHtML

[U100] JS：DOM 查询
来源：http://www.share.vehdjk.com/Article/details/gqgtiyfvt.sHtML

document.querySelector(".item")
来源：http://m.share.sjlbkw.cn/Article/details/gxghxvskb.sHtML

[U101] JS：classList 操作
来源：http://3g.yfazqb.com/Article/details/gwiggvddu.sHtML

el.classList.toggle("active")
来源：http://wap.epnwcf.com/Article/details/gzwvkarmk.sHtML

[U102] JS：本地存储
来源：http://www.m.share.bbcook.cn/Article/details/glehaszjm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.epnwcf.com/Article/details/gqisqmsbe.sHtML

[U103] JS：定时器
来源：http://blog.fktsv.cn/Article/details/gdpntideb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fktsv.cn/Article/details/gfcllbxay.sHtML

[U104] JS：防抖
来源：http://mobile.fktsv.cn/Article/details/gyqcwjctq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gtqvsarcr.sHtML

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/gfvgrxoos.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.tarul.cn/Article/details/ggprroslx.sHtML

[U106] JS：日期格式化
来源：http://mobile.bbcook.cn/Article/details/glofjqets.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.epnwcf.com/Article/details/ginxkkoyw.sHtML

[U107] JS：数字千分位
来源：http://mobile.fktsv.cn/Article/details/gexcbfava.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/glbarxplo.sHtML

[U108] JS：随机整数
来源：http://www.share.sjlbkw.cn/Article/details/gsqttzjzb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.vehdjk.com/Article/details/gpvrxbynm.sHtML

[U109] JS：数组分组
来源：http://www.share.yfazqb.com/Article/details/gdexkzuxq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/glzpxyggm.sHtML

[U110] JS：数组分块
来源：http://wap.vehdjk.com/Article/details/geehnuwtj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.tarul.cn/Article/details/gfatnazbs.sHtML

[U111] JS：对象转 Map
来源：http://3g.tarul.cn/Article/details/gwvsfhjlx.sHtML

new Map(Object.entries(obj))
来源：http://3g.tarul.cn/Article/details/gcoyxhtbj.sHtML

[U112] JS：字符串补位
来源：http://m.share.yfazqb.com/Article/details/gwvcnkuds.sHtML

"7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gagrjtuux.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.yfazqb.com/Article/details/gjproazdh.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/ggpbntcwe.sHtML

[U114] JS：JSON 深比较
来源：http://3g.vehdjk.com/Article/details/glptcocfn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gvxnpkrsn.sHtML

[U115] JS：生成 UUID
来源：http://baike.fktsv.cn/Article/details/ghjyxakzo.sHtML

crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/ghqfuveqv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.tarul.cn/Article/details/govipdxsi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gruvayisb.sHtML

[U117] JS：单元测试
来源：http://www.blog.yfazqb.com/Article/details/gqoiwjnqo.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.vehdjk.com/Article/details/gutdpsvfg.sHtML

[U118] JS：开发服务器
来源：http://mobile.fktsv.cn/Article/details/gccwqwqsy.sHtML

npm i -D vite;  npx vite
来源：http://m.share.yfazqb.com/Article/details/gtthqjwej.sHtML

[U119] JS：生产构建
来源：http://www.share.tarul.cn/Article/details/gviubkgim.sHtML

npx vite build
来源：http://m.share.sjlbkw.cn/Article/details/gntmpozuu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.epnwcf.com/Article/details/gqqsptcrq.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.tarul.cn/Article/details/ggydnvmwv.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmqkkcpkt.sHtML

统计汇总
来源：http://mobile.epnwcf.com/Article/details/gekdvtxof.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glheqziru.sHtML

按语言统计（条）：
来源：http://m.share.vehdjk.com/Article/details/gdmqpcwtx.sHtML

Python ......... 252
来源：http://wap.sjlbkw.cn/Article/details/gkrlubwhc.sHtML

PHP ............ 252
来源：http://www.share.epnwcf.com/Article/details/ghzipxeoh.sHtML

JavaScript ..... 252
来源：http://3g.bbcook.cn/Article/details/gjrmnfezn.sHtML

TypeScript ..... 212
来源：http://read.share.bbcook.cn/Article/details/gudkijqdp.sHtML

Java ........... 212
来源：http://baike.yfazqb.com/Article/details/giovvhehh.sHtML

Go ............. 212
来源：http://mobile.epnwcf.com/Article/details/gqwlodrnt.sHtML

Ruby ........... 212
来源：http://wap.tarul.cn/Article/details/gishvpros.sHtML

C# ............. 212
来源：http://blog.bbcook.cn/Article/details/gqyhpfjib.sHtML

C .............. 30
来源：http://m.share.epnwcf.com/Article/details/gsqlvzebz.sHtML

C++ ............ 30
来源：http://www.share.sjlbkw.cn/Article/details/gwefasjxp.sHtML

SQL ............ 90
来源：http://blog.sjlbkw.cn/Article/details/ggwjaqoir.sHtML

Bash ........... 80
来源：http://read.share.epnwcf.com/Article/details/gwtkdajqg.sHtML

Kotlin ......... 15
来源：http://read.share.tarul.cn/Article/details/grsgkiuyv.sHtML

Swift .......... 15
来源：http://read.share.vehdjk.com/Article/details/ggmieuwyz.sHtML

Lua ............ 10
来源：http://mobile.yfazqb.com/Article/details/gknwekbxk.sHtML

Perl ........... 10
来源：http://www.blog.sjlbkw.cn/Article/details/ggiekrhth.sHtML

Scala .......... 10
来源：http://read.share.vehdjk.com/Article/details/gseubkkoj.sHtML

------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/ghagsnvaz.sHtML

合计 ........... 2106 条
来源：http://baike.sjlbkw.cn/Article/details/gmxafluwx.sHtML

按章节统计：
来源：http://m.share.tarul.cn/Article/details/gzeckpvwx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.yfazqb.com/Article/details/gemxbbhum.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gwarjkjsy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gyganctbf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/gggtyabxb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.yfazqb.com/Article/details/ginnkcfpr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/gwpsaibqj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/gnatpfezq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.bbcook.cn/Article/details/gqkyhwgxc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/geapavdlg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.vehdjk.com/Article/details/ggbrxceea.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gerkiyqfi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gamwmimlq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gbrdbrslf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/ghilcqtke.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.bbcook.cn/Article/details/gscbagjqq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/ggyznqsic.sHtML

Q SQL 专题                              90
来源：http://mobile.sjlbkw.cn/Article/details/gaondovvn.sHtML

R Bash 专题                             80
来源：http://www.share.fktsv.cn/Article/details/gdtxbxass.sHtML

S C / C++ 专题                          60
来源：http://read.share.epnwcf.com/Article/details/gotogfyqe.sHtML

T 其他语言补充                          60
来源：http://read.share.vehdjk.com/Article/details/ghfqczndy.sHtML

U 高频实用片段                         120
来源：http://read.share.tarul.cn/Article/details/guuxqzmsz.sHtML

------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gctvkgftk.sHtML

合计                                  2106 条
来源：http://mobile.sjlbkw.cn/Article/details/ggmjtchnv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/gkzqlgbki.sHtML

使用提醒
来源：http://www.m.share.epnwcf.com/Article/details/gakvkdxjl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/guxoohwgr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.sjlbkw.cn/Article/details/gcybmytic.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.sjlbkw.cn/Article/details/gzpumgsav.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.epnwcf.com/Article/details/gygcwihra.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.epnwcf.com/Article/details/gydbbsmka.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.tarul.cn/Article/details/gobhybfjy.sHtML

—— 文件结束 ——
来源：http://mobile.fktsv.cn/Article/details/gxvjijmhb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gfszwhjff.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.epnwcf.com/Article/details/gigexixgn.sHtML

Common Programming Examples Cheat Book
来源：http://blog.tarul.cn/Article/details/gvxeiegkp.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpjxqvdsb.sHtML

【收录内容】
来源：http://mobile.yfazqb.com/Article/details/gtxjljaps.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.bbcook.cn/Article/details/gzmscrqtd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fktsv.cn/Article/details/gbgwycdfn.sHtML

SQL · Bash · C · C++
来源：http://www.share.epnwcf.com/Article/details/giiddgqag.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fktsv.cn/Article/details/gnomcgpgj.sHtML

【使用说明】
来源：http://www.share.yfazqb.com/Article/details/gniqniofc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.epnwcf.com/Article/details/giayjmwct.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.tarul.cn/Article/details/gnutoviyx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fktsv.cn/Article/details/gnfsflmdx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.sjlbkw.cn/Article/details/gbexhxwcc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.sjlbkw.cn/Article/details/gdxakpygd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.vehdjk.com/Article/details/gmbfzpbzz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fktsv.cn/Article/details/gcuwefrzq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fktsv.cn/Article/details/gkwawmhin.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.tarul.cn/Article/details/gciuaqmbg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.tarul.cn/Article/details/gabwkvgzg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.tarul.cn/Article/details/gjpobbsyi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.epnwcf.com/Article/details/gmihgamss.sHtML

【文件统计】
来源：http://3g.fktsv.cn/Article/details/gofuekqrd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.sjlbkw.cn/Article/details/gnbkltzfw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/grsmdsyxg.sHtML

目  录
来源：http://wap.fktsv.cn/Article/details/gjamdeqni.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gnozognpa.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.epnwcf.com/Article/details/gehzjwjtc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gzkoozxfy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/gltrjbjuy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fktsv.cn/Article/details/gnfwsdegd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.bbcook.cn/Article/details/gewcvncpd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.bbcook.cn/Article/details/gpyhdixgs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gwbvxuaai.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.yfazqb.com/Article/details/gftfgfyvi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gbgjllqlq.sHtML


<!-- 参考信息 -->