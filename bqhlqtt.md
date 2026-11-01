代发 wailian999

[U19] Py：正则替换带回调
来源：http://baike.epnwcf.com/Article/details/gwnznxlsc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.vehdjk.com/Article/details/gsbzfntwn.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.sjlbkw.cn/Article/details/gclayonrw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.vehdjk.com/Article/details/gnstvvxag.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fktsv.cn/Article/details/gshitonzt.sHtML

@contextlib.contextmanager
来源：http://blog.tarul.cn/Article/details/gynjsywzr.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.epnwcf.com/Article/details/gbenltrxy.sHtML

list(zip(*m))
来源：http://www.blog.tarul.cn/Article/details/grhoxsqsu.sHtML

[U23] Py：分块读取大文件
来源：http://baike.tarul.cn/Article/details/gpwcwnish.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fktsv.cn/Article/details/gfiigkpeb.sHtML

[U24] Py：路径操作
来源：http://m.share.epnwcf.com/Article/details/gtzjhlvrs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gvzhnterh.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.bbcook.cn/Article/details/gztrdqpnd.sHtML

csv.DictReader(f)
来源：http://mobile.vehdjk.com/Article/details/gtkgpvshm.sHtML

[U26] Py：并发下载
来源：http://mobile.sjlbkw.cn/Article/details/gfeexcfrp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.sjlbkw.cn/Article/details/grvxvvdzw.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.tarul.cn/Article/details/gdogpwnfo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.sjlbkw.cn/Article/details/gsrpmoijs.sHtML

[U28] Py：类型别名
来源：http://www.m.share.bbcook.cn/Article/details/gxtydpbvm.sHtML

UserId = int
来源：http://read.share.yfazqb.com/Article/details/goufmmkiy.sHtML

[U29] Py：属性校验
来源：http://blog.vehdjk.com/Article/details/gtdlhjpfs.sHtML

@property 与 @x.setter 配合
来源：http://mobile.epnwcf.com/Article/details/gmbrokftz.sHtML

[U30] Py：数据类
来源：http://baike.fktsv.cn/Article/details/gfihujdjy.sHtML

@dataclass(slots=True)
来源：http://wap.epnwcf.com/Article/details/gpmwhtooj.sHtML

[U31] Py：单测
来源：http://www.share.yfazqb.com/Article/details/gppduwgxz.sHtML

python -m pytest -q
来源：http://blog.tarul.cn/Article/details/gmaveggmm.sHtML

[U32] Py：代码格式化
来源：http://baike.fktsv.cn/Article/details/giyceirdm.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.bbcook.cn/Article/details/gctdjidvl.sHtML

[U33] Py：打包发布
来源：http://blog.epnwcf.com/Article/details/gttjzzpjw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.sjlbkw.cn/Article/details/gtbqyaoih.sHtML

[U34] Py：判断编码
来源：http://www.share.sjlbkw.cn/Article/details/gemmfswzy.sHtML

chardet.detect(raw)
来源：http://www.blog.fktsv.cn/Article/details/gkdldpctp.sHtML

[U35] Py：发送邮件
来源：http://mobile.epnwcf.com/Article/details/glrmkzcqz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.sjlbkw.cn/Article/details/gpnlusesy.sHtML

[U36] Py：定时任务
来源：http://3g.tarul.cn/Article/details/gdhymvmic.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.bbcook.cn/Article/details/glzemkiuy.sHtML

[U37] Py：读写 Excel
来源：http://m.share.yfazqb.com/Article/details/gsovlbklk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.epnwcf.com/Article/details/gmjjmrgof.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fktsv.cn/Article/details/gzbnjaxrf.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.bbcook.cn/Article/details/gakjczcxm.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.vehdjk.com/Article/details/guwopigww.sHtML

sys.stdout.isatty()
来源：http://wap.yfazqb.com/Article/details/gobwtkyra.sHtML

[U40] Py：打印到标准错误
来源：http://baike.epnwcf.com/Article/details/goyulcnvo.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/glebglled.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.vehdjk.com/Article/details/gfdjlbdba.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.vehdjk.com/Article/details/gctrcppah.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.tarul.cn/Article/details/gtgpszaoa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.tarul.cn/Article/details/gzlzakwud.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.bbcook.cn/Article/details/giecqdzbs.sHtML

namespace App\Http;
来源：http://read.share.sjlbkw.cn/Article/details/gjpwokgsw.sHtML

[U44] PHP：开启严格类型
来源：http://3g.sjlbkw.cn/Article/details/ghuewlxuv.sHtML

declare(strict_types=1);
来源：http://www.share.yfazqb.com/Article/details/gjippcngc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.sjlbkw.cn/Article/details/gtrokozhm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gtsfjtfmu.sHtML

[U46] PHP：可空类型
来源：http://www.share.tarul.cn/Article/details/goegyakqd.sHtML

?string $name = null
来源：http://baike.fktsv.cn/Article/details/gvnpdmqgz.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.epnwcf.com/Article/details/giwntzhhw.sHtML

int|string $id
来源：http://www.share.yfazqb.com/Article/details/gcptdzvja.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.vehdjk.com/Article/details/goyhojvjs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.tarul.cn/Article/details/gfrzwqczi.sHtML

[U49] PHP：只读属性
来源：http://m.share.vehdjk.com/Article/details/goeintriy.sHtML

public readonly string $name
来源：http://mobile.epnwcf.com/Article/details/gppgujgzi.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.sjlbkw.cn/Article/details/gqvltacqc.sHtML

public function __construct(private int $id) {}
来源：http://mobile.vehdjk.com/Article/details/gwmonlkyg.sHtML

[U51] PHP：数组解构
来源：http://wap.fktsv.cn/Article/details/gbuvywcbu.sHtML

[$a, $b] = $arr;
来源：http://m.share.yfazqb.com/Article/details/gcxcmcrhl.sHtML

[U52] PHP：箭头函数
来源：http://baike.tarul.cn/Article/details/gpnhskvle.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.tarul.cn/Article/details/gujmmlilu.sHtML

[U53] PHP：空合并运算符
来源：http://baike.yfazqb.com/Article/details/ghgbofzyv.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.yfazqb.com/Article/details/goggodxsx.sHtML

[U54] PHP：空安全调用
来源：http://3g.tarul.cn/Article/details/gewyrpfvg.sHtML

$obj?->method()
来源：http://m.share.epnwcf.com/Article/details/gpzdomwiw.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fktsv.cn/Article/details/gqtxyoaxy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.tarul.cn/Article/details/gesmilzrm.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fktsv.cn/Article/details/gitwkbome.sHtML

f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gmstjqgpc.sHtML

[U57] PHP：字符串插值
来源：http://blog.tarul.cn/Article/details/gatmtmiep.sHtML

"值: {$a}"
来源：http://3g.fktsv.cn/Article/details/gswcmnkig.sHtML

[U58] PHP：数组三件套
来源：http://baike.sjlbkw.cn/Article/details/gzynbomjd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.epnwcf.com/Article/details/gjwcdojlh.sHtML

[U59] PHP：自定义排序
来源：http://3g.tarul.cn/Article/details/glqrzghbi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.bbcook.cn/Article/details/gkmqlfvaq.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.sjlbkw.cn/Article/details/gxdqcwjtq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.bbcook.cn/Article/details/gctqngfbe.sHtML

[U61] PHP：正则
来源：http://read.share.tarul.cn/Article/details/gturnkaot.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gtvxmoqsc.sHtML

[U62] PHP：日期对象
来源：http://mobile.fktsv.cn/Article/details/gwlwrpgqz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtcujzhp.sHtML

[U63] PHP：文件读写
来源：http://blog.sjlbkw.cn/Article/details/gdipybecm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.sjlbkw.cn/Article/details/gpeiizits.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fktsv.cn/Article/details/gjcirjmkx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.bbcook.cn/Article/details/ghsxwzjqc.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/gcrmlwzhg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.yfazqb.com/Article/details/gygtxlwjh.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.bbcook.cn/Article/details/ghrfnhipi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.tarul.cn/Article/details/gktneaget.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.vehdjk.com/Article/details/gltnigmgi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.bbcook.cn/Article/details/gbcbvwrkv.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gipbkwihg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.sjlbkw.cn/Article/details/gyxudzyfn.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.epnwcf.com/Article/details/gkfsdtxym.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.yfazqb.com/Article/details/gdqzdvigt.sHtML

[U70] PHP：PDO 事务
来源：http://baike.epnwcf.com/Article/details/gtsodwqtg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.vehdjk.com/Article/details/guwaueaxm.sHtML

[U71] PHP：抛出异常
来源：http://read.share.vehdjk.com/Article/details/gvekxjvle.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.epnwcf.com/Article/details/geonvhnuf.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fktsv.cn/Article/details/geqcclanb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.vehdjk.com/Article/details/gffiraurf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.bbcook.cn/Article/details/gvkrywnvs.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqmcmxwp.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fktsv.cn/Article/details/gbksgpdfl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.vehdjk.com/Article/details/gctmgdmzu.sHtML

[U75] PHP：依赖注入
来源：http://read.share.sjlbkw.cn/Article/details/gbdpvdhvj.sHtML

composer require psr/container
来源：http://3g.vehdjk.com/Article/details/gpscyfpel.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.epnwcf.com/Article/details/guzquliok.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.sjlbkw.cn/Article/details/gntpomqcm.sHtML

[U77] PHP：模板渲染
来源：http://wap.yfazqb.com/Article/details/gqmobnptm.sHtML

composer require twig/twig
来源：http://baike.tarul.cn/Article/details/gmdwtmxae.sHtML

[U78] PHP：单元测试
来源：http://mobile.bbcook.cn/Article/details/gabzrsgwp.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fktsv.cn/Article/details/gsebjkppo.sHtML

[U79] PHP：静态分析
来源：http://m.share.yfazqb.com/Article/details/gmaokisba.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.sjlbkw.cn/Article/details/gwczlaepl.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.yfazqb.com/Article/details/gaqglmsna.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.tarul.cn/Article/details/gtnbmhfaz.sHtML

[U81] JS：初始化项目
来源：http://read.share.fktsv.cn/Article/details/gnoeqoien.sHtML

npm init -y;  npm i express
来源：http://baike.fktsv.cn/Article/details/gbubwtqqt.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.epnwcf.com/Article/details/geqhkgphv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.sjlbkw.cn/Article/details/gsfxrwivt.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.vehdjk.com/Article/details/gbebyaach.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.tarul.cn/Article/details/gwbdztspj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.vehdjk.com/Article/details/gqukijrwx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.tarul.cn/Article/details/glzgiigfv.sHtML

[U85] JS：可选链
来源：http://mobile.tarul.cn/Article/details/gpvwjyeiv.sHtML

a?.b?.c
来源：http://www.blog.vehdjk.com/Article/details/gwhasnhqa.sHtML

[U86] JS：空值合并
来源：http://mobile.vehdjk.com/Article/details/geilppngs.sHtML

a ?? b
来源：http://mobile.yfazqb.com/Article/details/gelvagksc.sHtML

[U87] JS：解构默认值
来源：http://read.share.vehdjk.com/Article/details/gwszneovq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.epnwcf.com/Article/details/gjmtwtnek.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.sjlbkw.cn/Article/details/gwtxautaq.sHtML

{ ...a, ...b }
来源：http://wap.vehdjk.com/Article/details/griehjdyw.sHtML

[U89] JS：数组去重
来源：http://3g.yfazqb.com/Article/details/gzohnmexj.sHtML

[...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gwjvferrw.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.epnwcf.com/Article/details/gngyefshr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gspjvjhyy.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.yfazqb.com/Article/details/gdkiyddwb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.yfazqb.com/Article/details/gfzxkeezz.sHtML

[U92] JS：深拷贝
来源：http://baike.tarul.cn/Article/details/gmqpcwrth.sHtML

structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gtuherkrq.sHtML

[U93] JS：模板字符串
来源：http://wap.sjlbkw.cn/Article/details/gmroqfuns.sHtML

`共 ${n} 条`
来源：http://www.share.yfazqb.com/Article/details/ghpvtlztu.sHtML

[U94] JS：箭头函数
来源：http://baike.fktsv.cn/Article/details/gozthpfmq.sHtML

const double = x => x * 2;
来源：http://read.share.epnwcf.com/Article/details/givedvkxd.sHtML

[U95] JS：Promise 包装
来源：http://3g.yfazqb.com/Article/details/grnaldadp.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.sjlbkw.cn/Article/details/glvxnndfk.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fktsv.cn/Article/details/gpapiosdk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gdtuniioi.sHtML

[U97] JS：并发请求
来源：http://m.share.fktsv.cn/Article/details/gugbxbzzh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gwxkuomly.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gttipxxxw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.sjlbkw.cn/Article/details/gphypijnu.sHtML

[U99] JS：事件监听
来源：http://read.share.sjlbkw.cn/Article/details/gcgqonbzh.sHtML

el.addEventListener("click", e => {})
来源：http://3g.bbcook.cn/Article/details/ggtwjxrbf.sHtML

[U100] JS：DOM 查询
来源：http://wap.sjlbkw.cn/Article/details/gzpdbopmc.sHtML

document.querySelector(".item")
来源：http://m.share.sjlbkw.cn/Article/details/gifvggiua.sHtML

[U101] JS：classList 操作
来源：http://m.share.fktsv.cn/Article/details/glrdaqwbj.sHtML

el.classList.toggle("active")
来源：http://www.m.share.sjlbkw.cn/Article/details/gskgowvil.sHtML

[U102] JS：本地存储
来源：http://read.share.bbcook.cn/Article/details/gvrlpdzjt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.vehdjk.com/Article/details/gggximqld.sHtML

[U103] JS：定时器
来源：http://www.m.share.yfazqb.com/Article/details/ggoouehsk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.bbcook.cn/Article/details/gitpqfftk.sHtML

[U104] JS：防抖
来源：http://3g.vehdjk.com/Article/details/gaateziiw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gswhzzaev.sHtML

[U105] JS：节流
来源：http://www.blog.epnwcf.com/Article/details/gcfcepjtd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.sjlbkw.cn/Article/details/ghrouulby.sHtML

[U106] JS：日期格式化
来源：http://wap.tarul.cn/Article/details/gzccmiuwv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.sjlbkw.cn/Article/details/gcxhjwxui.sHtML

[U107] JS：数字千分位
来源：http://blog.epnwcf.com/Article/details/gqearxnuj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fktsv.cn/Article/details/gkhfazvkq.sHtML

[U108] JS：随机整数
来源：http://wap.vehdjk.com/Article/details/gjqybnmxg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.tarul.cn/Article/details/gsxbmxgso.sHtML

[U109] JS：数组分组
来源：http://3g.sjlbkw.cn/Article/details/ghfasezjx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/glywqofog.sHtML

[U110] JS：数组分块
来源：http://www.share.epnwcf.com/Article/details/gvsliitzz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.vehdjk.com/Article/details/gfeswvhxi.sHtML

[U111] JS：对象转 Map
来源：http://read.share.bbcook.cn/Article/details/grmxebdpi.sHtML

new Map(Object.entries(obj))
来源：http://wap.yfazqb.com/Article/details/grcanvako.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fktsv.cn/Article/details/ggzpscney.sHtML

"7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/ghrhxoasg.sHtML

[U113] JS：正则替换全部
来源：http://wap.sjlbkw.cn/Article/details/gjwgksnzg.sHtML

s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/ghlisgbwi.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.tarul.cn/Article/details/ghcqjrdbz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gdauwymnb.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fktsv.cn/Article/details/geemarujb.sHtML

crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gimwgzyui.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyjkqcih.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.sjlbkw.cn/Article/details/gxpsshdit.sHtML

[U117] JS：单元测试
来源：http://m.share.bbcook.cn/Article/details/gtnlmmjao.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.vehdjk.com/Article/details/ggwwctdfz.sHtML

[U118] JS：开发服务器
来源：http://mobile.fktsv.cn/Article/details/ggqupykxb.sHtML

npm i -D vite;  npx vite
来源：http://m.share.yfazqb.com/Article/details/gsratgxkr.sHtML

[U119] JS：生产构建
来源：http://3g.tarul.cn/Article/details/genrwvwuh.sHtML

npx vite build
来源：http://3g.tarul.cn/Article/details/gjwkjekay.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.epnwcf.com/Article/details/goeqbfcyq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.bbcook.cn/Article/details/gqljsdfsa.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gluzulolr.sHtML

统计汇总
来源：http://blog.yfazqb.com/Article/details/goxjtpsyc.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvdqjsigz.sHtML

按语言统计（条）：
来源：http://blog.yfazqb.com/Article/details/gkgzrabxg.sHtML

Python ......... 252
来源：http://www.m.share.vehdjk.com/Article/details/gzwdjvwis.sHtML

PHP ............ 252
来源：http://www.share.sjlbkw.cn/Article/details/gmodtiqqu.sHtML

JavaScript ..... 252
来源：http://3g.bbcook.cn/Article/details/gkobknryw.sHtML

TypeScript ..... 212
来源：http://www.share.fktsv.cn/Article/details/gupaitgcr.sHtML

Java ........... 212
来源：http://read.share.epnwcf.com/Article/details/gaeauhwiz.sHtML

Go ............. 212
来源：http://baike.sjlbkw.cn/Article/details/gbrcyomcj.sHtML

Ruby ........... 212
来源：http://mobile.yfazqb.com/Article/details/gekcfgzzd.sHtML

C# ............. 212
来源：http://read.share.epnwcf.com/Article/details/gfocwinkh.sHtML

C .............. 30
来源：http://read.share.fktsv.cn/Article/details/gufydilnn.sHtML

C++ ............ 30
来源：http://mobile.fktsv.cn/Article/details/ghrtwlpbc.sHtML

SQL ............ 90
来源：http://baike.epnwcf.com/Article/details/gbocnldrg.sHtML

Bash ........... 80
来源：http://baike.sjlbkw.cn/Article/details/gcsrtylgd.sHtML

Kotlin ......... 15
来源：http://m.share.epnwcf.com/Article/details/guxcutvsl.sHtML

Swift .......... 15
来源：http://wap.tarul.cn/Article/details/gufsfxgfy.sHtML

Lua ............ 10
来源：http://blog.vehdjk.com/Article/details/glsddejhz.sHtML

Perl ........... 10
来源：http://blog.sjlbkw.cn/Article/details/ghbiggdcm.sHtML

Scala .......... 10
来源：http://www.share.yfazqb.com/Article/details/gneztzsce.sHtML

------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gihhshpxi.sHtML

合计 ........... 2106 条
来源：http://mobile.yfazqb.com/Article/details/gnmlhnsax.sHtML

按章节统计：
来源：http://www.blog.tarul.cn/Article/details/gnfzzflbr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fktsv.cn/Article/details/gqbzftjpd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/gdkpsqsxv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gvyqohvpd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.tarul.cn/Article/details/ghboropsg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fktsv.cn/Article/details/gnvgxdltx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.vehdjk.com/Article/details/gwiuwynqi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gshaonwce.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.epnwcf.com/Article/details/gfthamgja.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/gonaithcy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.vehdjk.com/Article/details/gkvftbxtq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gnuyafufv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/grlliwfvq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gxanhltwz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/gqkbxfvhn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.sjlbkw.cn/Article/details/gdqvxxuzj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gdjxovwmo.sHtML

Q SQL 专题                              90
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbkzllwe.sHtML

R Bash 专题                             80
来源：http://www.blog.bbcook.cn/Article/details/gnabtbfgo.sHtML

S C / C++ 专题                          60
来源：http://www.share.fktsv.cn/Article/details/gbxaucbcs.sHtML

T 其他语言补充                          60
来源：http://wap.bbcook.cn/Article/details/guzknxnpc.sHtML

U 高频实用片段                         120
来源：http://wap.epnwcf.com/Article/details/gcsaperue.sHtML

------------------------------------
来源：http://baike.yfazqb.com/Article/details/gxnehzgzl.sHtML

合计                                  2106 条
来源：http://www.blog.yfazqb.com/Article/details/gdlxvzvgs.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gmijdhwgn.sHtML

使用提醒
来源：http://www.m.share.epnwcf.com/Article/details/gmhriweuf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/glssuuwol.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fktsv.cn/Article/details/gcqbgahah.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.epnwcf.com/Article/details/gwkqouizk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.yfazqb.com/Article/details/gmieyrymq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.tarul.cn/Article/details/gcwbjeaxy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.tarul.cn/Article/details/gpauftzhb.sHtML

—— 文件结束 ——
来源：http://www.blog.fktsv.cn/Article/details/gdhprdmwq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guyclfgte.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqzyxdtx.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbwpqbzb.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ggligejgb.sHtML

【收录内容】
来源：http://m.share.sjlbkw.cn/Article/details/gvvafohog.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.bbcook.cn/Article/details/gqeuuotrt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.vehdjk.com/Article/details/gsjefxivr.sHtML

SQL · Bash · C · C++
来源：http://www.share.yfazqb.com/Article/details/gsbqfgdca.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fktsv.cn/Article/details/gkbiesatq.sHtML

【使用说明】
来源：http://read.share.fktsv.cn/Article/details/glkfvorzl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.yfazqb.com/Article/details/gomgztldz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.epnwcf.com/Article/details/gbnhlpita.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.vehdjk.com/Article/details/gwdyvybyx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.tarul.cn/Article/details/gshcyscph.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.epnwcf.com/Article/details/gewzijjdu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.sjlbkw.cn/Article/details/gjdjkiypi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.epnwcf.com/Article/details/gbkjpaiby.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.vehdjk.com/Article/details/gzsyzvbxs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.vehdjk.com/Article/details/gfgugelqa.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.epnwcf.com/Article/details/gresbpdku.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.tarul.cn/Article/details/gihwoedag.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fktsv.cn/Article/details/gijpalhgm.sHtML

【文件统计】
来源：http://wap.epnwcf.com/Article/details/gryqsmvdo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.bbcook.cn/Article/details/gqdxotixc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gqdtngerb.sHtML

目  录
来源：http://blog.tarul.cn/Article/details/gruonahum.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gzfosjemf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.tarul.cn/Article/details/gewzcbinz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.tarul.cn/Article/details/gjfponnxq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/gujyvfwum.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.bbcook.cn/Article/details/gllouimig.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fktsv.cn/Article/details/gfrtrgzfh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.epnwcf.com/Article/details/gbjvdobuj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/gkliosrhv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.bbcook.cn/Article/details/gvptbumiz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/ghtuqmcrf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.sjlbkw.cn/Article/details/gmatjymrf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gccgzqnah.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gbifthqso.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gxbgzlmrn.sHtML


<!-- 参考信息 -->