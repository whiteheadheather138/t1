代发 wailian999

[U15] Py：高精度计时
来源：http://www.m.share.fktsv.cn/Article/details/gdwxwftqn.sHtML

t = time.perf_counter()
来源：http://mobile.bbcook.cn/Article/details/ghuuvldoe.sHtML

[U16] Py：命令行参数解析
来源：http://3g.bbcook.cn/Article/details/ghyiboiuq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.epnwcf.com/Article/details/grnuqypxf.sHtML

[U17] Py：初始化日志
来源：http://www.share.sjlbkw.cn/Article/details/goocxgxua.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.tarul.cn/Article/details/gmdirownw.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.tarul.cn/Article/details/gxnmsfxsn.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.bbcook.cn/Article/details/gfcodijta.sHtML

[U19] Py：正则替换带回调
来源：http://blog.bbcook.cn/Article/details/ghqfffscj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.bbcook.cn/Article/details/gwexqkeql.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.yfazqb.com/Article/details/gpnmrzula.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.yfazqb.com/Article/details/gmsdgmzos.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fktsv.cn/Article/details/gtrzblsid.sHtML

@contextlib.contextmanager
来源：http://baike.vehdjk.com/Article/details/gyirhdmqw.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fktsv.cn/Article/details/gjppaulrd.sHtML

list(zip(*m))
来源：http://read.share.yfazqb.com/Article/details/ggogzwoeb.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.yfazqb.com/Article/details/gxndvwmvm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.bbcook.cn/Article/details/gyszslyyl.sHtML

[U24] Py：路径操作
来源：http://read.share.vehdjk.com/Article/details/ggbvfcelt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gsroitfbj.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.tarul.cn/Article/details/golodqrly.sHtML

csv.DictReader(f)
来源：http://m.share.yfazqb.com/Article/details/gpoknqbjb.sHtML

[U26] Py：并发下载
来源：http://www.share.fktsv.cn/Article/details/gotzqfbev.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.vehdjk.com/Article/details/gfaujdqnp.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.yfazqb.com/Article/details/gojntbkrz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fktsv.cn/Article/details/gaqzssfhl.sHtML

[U28] Py：类型别名
来源：http://3g.fktsv.cn/Article/details/gdziszozv.sHtML

UserId = int
来源：http://www.m.share.tarul.cn/Article/details/gdkbdymna.sHtML

[U29] Py：属性校验
来源：http://www.m.share.sjlbkw.cn/Article/details/gltmbpwva.sHtML

@property 与 @x.setter 配合
来源：http://m.share.tarul.cn/Article/details/gkmksblit.sHtML

[U30] Py：数据类
来源：http://blog.fktsv.cn/Article/details/guoorxjds.sHtML

@dataclass(slots=True)
来源：http://blog.vehdjk.com/Article/details/gxjzxjqwy.sHtML

[U31] Py：单测
来源：http://baike.fktsv.cn/Article/details/gbywhmjsj.sHtML

python -m pytest -q
来源：http://www.share.bbcook.cn/Article/details/ggynlycse.sHtML

[U32] Py：代码格式化
来源：http://www.share.sjlbkw.cn/Article/details/ggjavvyxk.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.tarul.cn/Article/details/goypspfjf.sHtML

[U33] Py：打包发布
来源：http://baike.epnwcf.com/Article/details/gwvpnsgyp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.sjlbkw.cn/Article/details/gqcukelws.sHtML

[U34] Py：判断编码
来源：http://mobile.sjlbkw.cn/Article/details/gpahugcwl.sHtML

chardet.detect(raw)
来源：http://read.share.yfazqb.com/Article/details/gmkcnopsn.sHtML

[U35] Py：发送邮件
来源：http://m.share.sjlbkw.cn/Article/details/ggfpwivwr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fktsv.cn/Article/details/gknhganoo.sHtML

[U36] Py：定时任务
来源：http://www.share.tarul.cn/Article/details/gzxyjvpkg.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.tarul.cn/Article/details/ggobsnjtx.sHtML

[U37] Py：读写 Excel
来源：http://read.share.epnwcf.com/Article/details/gokxgtpfg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fktsv.cn/Article/details/ggmnwxtzk.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.yfazqb.com/Article/details/gesgijldm.sHtML

Path(__file__).resolve().parent
来源：http://read.share.tarul.cn/Article/details/gljipakfv.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fktsv.cn/Article/details/gpatcgsox.sHtML

sys.stdout.isatty()
来源：http://baike.yfazqb.com/Article/details/gmvmcjkhe.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.yfazqb.com/Article/details/gqimqjlpv.sHtML

print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gcdyhbaom.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.bbcook.cn/Article/details/gjvpjnpan.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fktsv.cn/Article/details/gjjfxnkio.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.sjlbkw.cn/Article/details/ggkuwsafc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fktsv.cn/Article/details/gzdcrjedl.sHtML

[U43] PHP：声明命名空间
来源：http://blog.bbcook.cn/Article/details/gxxpcunhy.sHtML

namespace App\Http;
来源：http://www.blog.tarul.cn/Article/details/gkduascht.sHtML

[U44] PHP：开启严格类型
来源：http://baike.bbcook.cn/Article/details/gxupwiqxz.sHtML

declare(strict_types=1);
来源：http://3g.vehdjk.com/Article/details/gvhjjxexm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fktsv.cn/Article/details/gmxzoedls.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gqyavmyxm.sHtML

[U46] PHP：可空类型
来源：http://baike.fktsv.cn/Article/details/gibemqtvu.sHtML

?string $name = null
来源：http://blog.fktsv.cn/Article/details/gcgifpyii.sHtML

[U47] PHP：联合类型
来源：http://www.blog.vehdjk.com/Article/details/gmchohgbk.sHtML

int|string $id
来源：http://mobile.sjlbkw.cn/Article/details/gjylxmcwo.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.bbcook.cn/Article/details/ghiulgxhr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.bbcook.cn/Article/details/guogiqexi.sHtML

[U49] PHP：只读属性
来源：http://blog.tarul.cn/Article/details/gszmrjcjq.sHtML

public readonly string $name
来源：http://m.share.bbcook.cn/Article/details/gylawsnzs.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.vehdjk.com/Article/details/ggxcqvjzl.sHtML

public function __construct(private int $id) {}
来源：http://baike.tarul.cn/Article/details/gtythvwgy.sHtML

[U51] PHP：数组解构
来源：http://m.share.yfazqb.com/Article/details/gjnhcibpr.sHtML

[$a, $b] = $arr;
来源：http://read.share.fktsv.cn/Article/details/gaznisluk.sHtML

[U52] PHP：箭头函数
来源：http://baike.epnwcf.com/Article/details/gngazwsfp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.vehdjk.com/Article/details/gmniwjyxt.sHtML

[U53] PHP：空合并运算符
来源：http://wap.bbcook.cn/Article/details/ghkcazxmu.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.tarul.cn/Article/details/gsejsuulr.sHtML

[U54] PHP：空安全调用
来源：http://mobile.bbcook.cn/Article/details/gsitajznr.sHtML

$obj?->method()
来源：http://m.share.sjlbkw.cn/Article/details/gmlgciqal.sHtML

[U55] PHP：match 表达式
来源：http://read.share.vehdjk.com/Article/details/gyhktwtzm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.vehdjk.com/Article/details/gogfkcgdb.sHtML

[U56] PHP：命名参数
来源：http://3g.sjlbkw.cn/Article/details/gqvkpliwv.sHtML

f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gyoamyxpt.sHtML

[U57] PHP：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gtzrsqyay.sHtML

"值: {$a}"
来源：http://3g.yfazqb.com/Article/details/gaqrveoek.sHtML

[U58] PHP：数组三件套
来源：http://wap.yfazqb.com/Article/details/gjuzjurwo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.bbcook.cn/Article/details/goncjzpzy.sHtML

[U59] PHP：自定义排序
来源：http://wap.epnwcf.com/Article/details/guuufsmwj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gzwcmynoc.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.bbcook.cn/Article/details/ghglwekas.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fktsv.cn/Article/details/gcrjwotqz.sHtML

[U61] PHP：正则
来源：http://3g.epnwcf.com/Article/details/gcqbmejhu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/grozkondr.sHtML

[U62] PHP：日期对象
来源：http://read.share.sjlbkw.cn/Article/details/guhirleih.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.sjlbkw.cn/Article/details/graihfmoo.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.tarul.cn/Article/details/gbcexcplv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.yfazqb.com/Article/details/ggwnyyxlr.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.bbcook.cn/Article/details/gatumaqwc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fktsv.cn/Article/details/gicbujtgq.sHtML

[U65] PHP：会话
来源：http://www.blog.tarul.cn/Article/details/gbgwjgzzd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gqgtpefeu.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.yfazqb.com/Article/details/gcchsqeru.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.bbcook.cn/Article/details/gaztjzjkk.sHtML

[U67] PHP：处理文件上传
来源：http://wap.epnwcf.com/Article/details/gxwtxshdc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.yfazqb.com/Article/details/gcocnqmts.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.tarul.cn/Article/details/gtopvbgnl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fktsv.cn/Article/details/gdpaxzpyq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.yfazqb.com/Article/details/grobrgcqa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.epnwcf.com/Article/details/gngiymcmp.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fktsv.cn/Article/details/gqsmzsrko.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.vehdjk.com/Article/details/gaitxxdvi.sHtML

[U71] PHP：抛出异常
来源：http://blog.fktsv.cn/Article/details/gsrxgggzc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fktsv.cn/Article/details/gkjxlsmoi.sHtML

[U72] PHP：写错误日志
来源：http://baike.bbcook.cn/Article/details/gpjrqxptm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.vehdjk.com/Article/details/gqntrfqce.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.sjlbkw.cn/Article/details/gqwotndhp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fktsv.cn/Article/details/gyjofemxr.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gkfzupwri.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.yfazqb.com/Article/details/gfsyftgvm.sHtML

[U75] PHP：依赖注入
来源：http://wap.sjlbkw.cn/Article/details/goaqmolkf.sHtML

composer require psr/container
来源：http://baike.tarul.cn/Article/details/gattnastl.sHtML

[U76] PHP：简单路由
来源：http://m.share.epnwcf.com/Article/details/gxyyjgkyu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.epnwcf.com/Article/details/grjtsfdrr.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgvlrhft.sHtML

composer require twig/twig
来源：http://blog.yfazqb.com/Article/details/grrvvyeav.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.sjlbkw.cn/Article/details/gouygoxdn.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.bbcook.cn/Article/details/gomszrozm.sHtML

[U79] PHP：静态分析
来源：http://read.share.sjlbkw.cn/Article/details/glrldqotb.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fktsv.cn/Article/details/gwreekrlj.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.bbcook.cn/Article/details/gicqyejto.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.yfazqb.com/Article/details/gufsvspjj.sHtML

[U81] JS：初始化项目
来源：http://m.share.bbcook.cn/Article/details/gdumpeexl.sHtML

npm init -y;  npm i express
来源：http://m.share.epnwcf.com/Article/details/gqktmlapt.sHtML

[U82] JS：package.json 脚本
来源：http://wap.epnwcf.com/Article/details/gdulbgwxd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.yfazqb.com/Article/details/gwruanwmp.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.sjlbkw.cn/Article/details/gfgmlacqb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.tarul.cn/Article/details/gkwwzufwp.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.yfazqb.com/Article/details/gjfcqgwkx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.bbcook.cn/Article/details/gxximbeop.sHtML

[U85] JS：可选链
来源：http://baike.fktsv.cn/Article/details/gazicgiki.sHtML

a?.b?.c
来源：http://www.share.vehdjk.com/Article/details/gusujegnx.sHtML

[U86] JS：空值合并
来源：http://www.share.tarul.cn/Article/details/gzjkgcfmx.sHtML

a ?? b
来源：http://www.m.share.fktsv.cn/Article/details/gghppqdmm.sHtML

[U87] JS：解构默认值
来源：http://mobile.epnwcf.com/Article/details/gsubinkmn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fktsv.cn/Article/details/gvuigcwme.sHtML

[U88] JS：对象展开合并
来源：http://mobile.yfazqb.com/Article/details/gyzpkxnem.sHtML

{ ...a, ...b }
来源：http://baike.yfazqb.com/Article/details/gbzioyjyq.sHtML

[U89] JS：数组去重
来源：http://www.share.tarul.cn/Article/details/glcpgbipy.sHtML

[...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gclfdeuoe.sHtML

[U90] JS：数字数组排序
来源：http://baike.yfazqb.com/Article/details/gzhrpyycx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/glcnosdpw.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.yfazqb.com/Article/details/gqcuyrerl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.epnwcf.com/Article/details/gfczvdujb.sHtML

[U92] JS：深拷贝
来源：http://3g.yfazqb.com/Article/details/gtdyxjwki.sHtML

structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gwwnycltp.sHtML

[U93] JS：模板字符串
来源：http://read.share.bbcook.cn/Article/details/gcxqtsvdf.sHtML

`共 ${n} 条`
来源：http://blog.vehdjk.com/Article/details/godowfqio.sHtML

[U94] JS：箭头函数
来源：http://baike.bbcook.cn/Article/details/gldwlpage.sHtML

const double = x => x * 2;
来源：http://m.share.bbcook.cn/Article/details/guxdiiako.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.sjlbkw.cn/Article/details/gsnxobjjn.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.yfazqb.com/Article/details/ggmfhhavn.sHtML

[U96] JS：async/await 与异常
来源：http://wap.bbcook.cn/Article/details/gmmcpoven.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gyspxcgjg.sHtML

[U97] JS：并发请求
来源：http://mobile.sjlbkw.cn/Article/details/ggljheoid.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gvikhmumc.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.tarul.cn/Article/details/gjpzfqjpb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.vehdjk.com/Article/details/gbzivgboe.sHtML

[U99] JS：事件监听
来源：http://read.share.tarul.cn/Article/details/gorswqsob.sHtML

el.addEventListener("click", e => {})
来源：http://3g.tarul.cn/Article/details/gotdnjjud.sHtML

[U100] JS：DOM 查询
来源：http://blog.bbcook.cn/Article/details/gngfvgeqi.sHtML

document.querySelector(".item")
来源：http://3g.fktsv.cn/Article/details/gvkybzywm.sHtML

[U101] JS：classList 操作
来源：http://www.share.vehdjk.com/Article/details/gckclzofc.sHtML

el.classList.toggle("active")
来源：http://m.share.yfazqb.com/Article/details/giguaywbd.sHtML

[U102] JS：本地存储
来源：http://blog.tarul.cn/Article/details/gstzjwpsl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.tarul.cn/Article/details/glxmkwwnh.sHtML

[U103] JS：定时器
来源：http://baike.fktsv.cn/Article/details/gctchcqbe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.epnwcf.com/Article/details/gypjfqmsu.sHtML

[U104] JS：防抖
来源：http://www.blog.epnwcf.com/Article/details/gzmfqmmwh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/ggrpvhjkp.sHtML

[U105] JS：节流
来源：http://read.share.fktsv.cn/Article/details/gagstqqap.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmcozmae.sHtML

[U106] JS：日期格式化
来源：http://mobile.yfazqb.com/Article/details/gdyxtfnxx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.vehdjk.com/Article/details/grmvexdor.sHtML

[U107] JS：数字千分位
来源：http://3g.vehdjk.com/Article/details/gdimhbqvc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gsmfiropf.sHtML

[U108] JS：随机整数
来源：http://blog.yfazqb.com/Article/details/gvxpftfnc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fktsv.cn/Article/details/gpypnilch.sHtML

[U109] JS：数组分组
来源：http://mobile.yfazqb.com/Article/details/gqndskwmd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.epnwcf.com/Article/details/glfgnoldc.sHtML

[U110] JS：数组分块
来源：http://read.share.sjlbkw.cn/Article/details/gfdlvwbvc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.yfazqb.com/Article/details/ghbxeazhi.sHtML

[U111] JS：对象转 Map
来源：http://baike.sjlbkw.cn/Article/details/gbtfiuvei.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.yfazqb.com/Article/details/gxzatdhuq.sHtML

[U112] JS：字符串补位
来源：http://wap.tarul.cn/Article/details/grdwazbjq.sHtML

"7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/grtilslhh.sHtML

[U113] JS：正则替换全部
来源：http://wap.bbcook.cn/Article/details/gxesncsfx.sHtML

s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/glmmhghvz.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fktsv.cn/Article/details/gwklsscva.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/goavynbok.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gqqbnadpn.sHtML

crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gepwdkjhk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.epnwcf.com/Article/details/gywewghee.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.sjlbkw.cn/Article/details/grqdrwzak.sHtML

[U117] JS：单元测试
来源：http://www.blog.tarul.cn/Article/details/gqgoiisqw.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.epnwcf.com/Article/details/gvjhksfmh.sHtML

[U118] JS：开发服务器
来源：http://www.share.tarul.cn/Article/details/gaymxjxhj.sHtML

npm i -D vite;  npx vite
来源：http://3g.epnwcf.com/Article/details/gnsjphvut.sHtML

[U119] JS：生产构建
来源：http://3g.fktsv.cn/Article/details/gzoelgnzh.sHtML

npx vite build
来源：http://mobile.bbcook.cn/Article/details/gouafxtmr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.epnwcf.com/Article/details/gcoxgjwhj.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.bbcook.cn/Article/details/gfaerfpwr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmybfbfuq.sHtML

统计汇总
来源：http://www.blog.fktsv.cn/Article/details/glaiejeub.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjrzlqcvi.sHtML

按语言统计（条）：
来源：http://read.share.tarul.cn/Article/details/gxebhjcmd.sHtML

Python ......... 252
来源：http://www.blog.vehdjk.com/Article/details/gquijapcz.sHtML

PHP ............ 252
来源：http://www.m.share.bbcook.cn/Article/details/glhrwuhhx.sHtML

JavaScript ..... 252
来源：http://m.share.vehdjk.com/Article/details/gelfgnpnk.sHtML

TypeScript ..... 212
来源：http://3g.yfazqb.com/Article/details/gslpmdjzv.sHtML

Java ........... 212
来源：http://mobile.bbcook.cn/Article/details/gqmvmictw.sHtML

Go ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gunfhscpj.sHtML

Ruby ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gjsacpcwg.sHtML

C# ............. 212
来源：http://www.blog.vehdjk.com/Article/details/gmsytrhvm.sHtML

C .............. 30
来源：http://www.share.vehdjk.com/Article/details/gzhrritpo.sHtML

C++ ............ 30
来源：http://www.blog.epnwcf.com/Article/details/gdxgikmwh.sHtML

SQL ............ 90
来源：http://m.share.tarul.cn/Article/details/gdyirgllq.sHtML

Bash ........... 80
来源：http://www.share.tarul.cn/Article/details/glamhpzji.sHtML

Kotlin ......... 15
来源：http://www.blog.vehdjk.com/Article/details/ghfgizqiw.sHtML

Swift .......... 15
来源：http://www.share.fktsv.cn/Article/details/gamvdmgnd.sHtML

Lua ............ 10
来源：http://blog.vehdjk.com/Article/details/gopbxjilz.sHtML

Perl ........... 10
来源：http://read.share.bbcook.cn/Article/details/gjgrihemq.sHtML

Scala .......... 10
来源：http://wap.tarul.cn/Article/details/gzgwwzqrs.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/gqzwhbeae.sHtML

合计 ........... 2106 条
来源：http://www.blog.yfazqb.com/Article/details/gxudmwpjr.sHtML

按章节统计：
来源：http://mobile.fktsv.cn/Article/details/gnbzahign.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.bbcook.cn/Article/details/gmmxxmgkt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/grmopnclz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gmxszcrrm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.bbcook.cn/Article/details/guwplkell.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.vehdjk.com/Article/details/gcbzdlhsg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.tarul.cn/Article/details/gtwbhirio.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/gevhcniwt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.tarul.cn/Article/details/gqndnzrfb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gbuhliemu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.bbcook.cn/Article/details/gfrtmtqgp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gcmqafwvx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gqkhkypqd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gnhstdpcb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.sjlbkw.cn/Article/details/gekxuamwl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.sjlbkw.cn/Article/details/gxppnzkzb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/ggpniyueh.sHtML

Q SQL 专题                              90
来源：http://baike.tarul.cn/Article/details/gfjjprnff.sHtML

R Bash 专题                             80
来源：http://www.blog.vehdjk.com/Article/details/gesqwmjqf.sHtML

S C / C++ 专题                          60
来源：http://www.blog.vehdjk.com/Article/details/gkcdosnox.sHtML

T 其他语言补充                          60
来源：http://www.share.epnwcf.com/Article/details/gaacyacvw.sHtML

U 高频实用片段                         120
来源：http://www.share.vehdjk.com/Article/details/gsmvmwqew.sHtML

------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gdczcuhht.sHtML

合计                                  2106 条
来源：http://baike.epnwcf.com/Article/details/gxtouiuum.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gbwkxdygg.sHtML

使用提醒
来源：http://m.share.sjlbkw.cn/Article/details/goyjprgjg.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gwfqtmtxl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.vehdjk.com/Article/details/gzmocgguf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.vehdjk.com/Article/details/geyzxuhho.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.epnwcf.com/Article/details/gceumhgih.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.vehdjk.com/Article/details/gtoasioig.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.sjlbkw.cn/Article/details/ggktbnrle.sHtML

—— 文件结束 ——
来源：http://blog.tarul.cn/Article/details/gilaupmqo.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxutwutpu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.vehdjk.com/Article/details/gunfhwvop.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.vehdjk.com/Article/details/gzwbnlxdz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfhdhploc.sHtML

【收录内容】
来源：http://www.share.vehdjk.com/Article/details/ggvsxgfle.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.tarul.cn/Article/details/gjuzjazri.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.bbcook.cn/Article/details/gqylszorb.sHtML

SQL · Bash · C · C++
来源：http://www.share.sjlbkw.cn/Article/details/grhqpvkgg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.bbcook.cn/Article/details/gzxdnabwe.sHtML

【使用说明】
来源：http://www.blog.fktsv.cn/Article/details/gfsbmdqvf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fktsv.cn/Article/details/gctvthqrx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.sjlbkw.cn/Article/details/gssvqbcse.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.epnwcf.com/Article/details/gqkdaihyd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fktsv.cn/Article/details/gtstddlra.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.yfazqb.com/Article/details/gbmvrcyom.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.tarul.cn/Article/details/grobhxugk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.tarul.cn/Article/details/gpnsudlwo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.epnwcf.com/Article/details/gsbziktvh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.tarul.cn/Article/details/gbdbjtsij.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.sjlbkw.cn/Article/details/giahfmome.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fktsv.cn/Article/details/gcaflwgez.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fktsv.cn/Article/details/gifrurxzr.sHtML

【文件统计】
来源：http://www.blog.tarul.cn/Article/details/grhtwkvrt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.epnwcf.com/Article/details/geonfrocm.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gnzsziqjl.sHtML

目  录
来源：http://www.blog.tarul.cn/Article/details/gpocnhptm.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gclzroyrp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.yfazqb.com/Article/details/gdrxfjjet.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gxyehsjke.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.tarul.cn/Article/details/gintwfwsj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.tarul.cn/Article/details/gxkrhfxyh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.bbcook.cn/Article/details/gqwssnvga.sHtML


<!-- 参考信息 -->