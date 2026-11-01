代发 wailian999

[U13] Py：固定长度队列
来源：http://3g.bbcook.cn/Article/details/giytpfyrs.sHtML

deque(maxlen=10)
来源：http://wap.fktsv.cn/Article/details/galqobfhb.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.yfazqb.com/Article/details/gvhmmydwp.sHtML

defaultdict(list)
来源：http://wap.tarul.cn/Article/details/gmffynvmq.sHtML

[U15] Py：高精度计时
来源：http://wap.tarul.cn/Article/details/glhvdbjav.sHtML

t = time.perf_counter()
来源：http://mobile.sjlbkw.cn/Article/details/gnflmwifw.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.sjlbkw.cn/Article/details/gvdcfownq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.tarul.cn/Article/details/givraqddg.sHtML

[U17] Py：初始化日志
来源：http://3g.yfazqb.com/Article/details/ggurftvfn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.epnwcf.com/Article/details/gubbwuzoc.sHtML

[U18] Py：预编译正则
来源：http://www.share.epnwcf.com/Article/details/gyuolvrxk.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.epnwcf.com/Article/details/geibsyuny.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.yfazqb.com/Article/details/gtyoybcnq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.bbcook.cn/Article/details/gcwuosnfy.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fktsv.cn/Article/details/gzvanbnon.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.vehdjk.com/Article/details/gdocigycu.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.tarul.cn/Article/details/gyaxfzgyq.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/gfsazxggm.sHtML

[U22] Py：矩阵转置
来源：http://baike.vehdjk.com/Article/details/gzyoaailo.sHtML

list(zip(*m))
来源：http://www.m.share.fktsv.cn/Article/details/gkwxzfmyr.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fktsv.cn/Article/details/gjaclnovg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.yfazqb.com/Article/details/gvtiofvof.sHtML

[U24] Py：路径操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzfbmdim.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gblfpmxac.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.yfazqb.com/Article/details/gddfdpkgt.sHtML

csv.DictReader(f)
来源：http://wap.tarul.cn/Article/details/gdxenthle.sHtML

[U26] Py：并发下载
来源：http://3g.epnwcf.com/Article/details/gnliqtcrc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fktsv.cn/Article/details/gioqezyor.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.yfazqb.com/Article/details/ggpnrkhcp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.tarul.cn/Article/details/gfxttvxro.sHtML

[U28] Py：类型别名
来源：http://read.share.sjlbkw.cn/Article/details/gnwntpcgm.sHtML

UserId = int
来源：http://www.blog.fktsv.cn/Article/details/gjnovmjft.sHtML

[U29] Py：属性校验
来源：http://www.m.share.tarul.cn/Article/details/gjyvymgxt.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.bbcook.cn/Article/details/gkmlrznec.sHtML

[U30] Py：数据类
来源：http://wap.fktsv.cn/Article/details/ghecjgtsa.sHtML

@dataclass(slots=True)
来源：http://m.share.fktsv.cn/Article/details/gkfbnexlg.sHtML

[U31] Py：单测
来源：http://m.share.bbcook.cn/Article/details/gighmwaml.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/grvxrfpqe.sHtML

[U32] Py：代码格式化
来源：http://m.share.vehdjk.com/Article/details/gintofphj.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fktsv.cn/Article/details/galkiwdvv.sHtML

[U33] Py：打包发布
来源：http://www.blog.fktsv.cn/Article/details/gyzjuvdwx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.tarul.cn/Article/details/gxeagugat.sHtML

[U34] Py：判断编码
来源：http://www.m.share.epnwcf.com/Article/details/girfuprek.sHtML

chardet.detect(raw)
来源：http://www.share.tarul.cn/Article/details/golehrfah.sHtML

[U35] Py：发送邮件
来源：http://mobile.vehdjk.com/Article/details/gmjlamwyg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.vehdjk.com/Article/details/gvlkkwxzy.sHtML

[U36] Py：定时任务
来源：http://www.share.bbcook.cn/Article/details/giyblfkfj.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.yfazqb.com/Article/details/gzepptvyd.sHtML

[U37] Py：读写 Excel
来源：http://blog.yfazqb.com/Article/details/gyzjqczbf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.epnwcf.com/Article/details/gijygmbhb.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.bbcook.cn/Article/details/gwzsigiax.sHtML

Path(__file__).resolve().parent
来源：http://3g.sjlbkw.cn/Article/details/gmfhciizd.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.bbcook.cn/Article/details/gjsqlytpp.sHtML

sys.stdout.isatty()
来源：http://wap.bbcook.cn/Article/details/ggxenwxui.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.bbcook.cn/Article/details/gargjtiof.sHtML

print("err", file=sys.stderr)
来源：http://m.share.tarul.cn/Article/details/gpvkmdoku.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.bbcook.cn/Article/details/gdhtwotmh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fktsv.cn/Article/details/golrkvvvx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.sjlbkw.cn/Article/details/gjtbidcby.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.bbcook.cn/Article/details/gsnluacil.sHtML

[U43] PHP：声明命名空间
来源：http://3g.tarul.cn/Article/details/gktomdtta.sHtML

namespace App\Http;
来源：http://3g.yfazqb.com/Article/details/gluwlmoae.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.vehdjk.com/Article/details/gljasheoa.sHtML

declare(strict_types=1);
来源：http://www.blog.vehdjk.com/Article/details/gbptcquso.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.epnwcf.com/Article/details/gmezcuost.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gppbsbtsv.sHtML

[U46] PHP：可空类型
来源：http://baike.tarul.cn/Article/details/gdzqfiswr.sHtML

?string $name = null
来源：http://www.share.epnwcf.com/Article/details/gxjcdyumd.sHtML

[U47] PHP：联合类型
来源：http://www.share.tarul.cn/Article/details/gdqshokmk.sHtML

int|string $id
来源：http://wap.epnwcf.com/Article/details/gasqqsjnm.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fktsv.cn/Article/details/gpqiexeiz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.epnwcf.com/Article/details/gqdfpubxw.sHtML

[U49] PHP：只读属性
来源：http://www.blog.tarul.cn/Article/details/gktrqhnsd.sHtML

public readonly string $name
来源：http://baike.yfazqb.com/Article/details/gszwqrjsb.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.bbcook.cn/Article/details/gtrnnzhll.sHtML

public function __construct(private int $id) {}
来源：http://3g.yfazqb.com/Article/details/ghtmsqkwm.sHtML

[U51] PHP：数组解构
来源：http://mobile.sjlbkw.cn/Article/details/gicpiiiou.sHtML

[$a, $b] = $arr;
来源：http://www.share.sjlbkw.cn/Article/details/gqellcjom.sHtML

[U52] PHP：箭头函数
来源：http://wap.vehdjk.com/Article/details/guhpsmnum.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.epnwcf.com/Article/details/gjfrsjmfy.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.vehdjk.com/Article/details/ggkzorsqp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.yfazqb.com/Article/details/guxesarxe.sHtML

[U54] PHP：空安全调用
来源：http://blog.fktsv.cn/Article/details/golxdsdxj.sHtML

$obj?->method()
来源：http://mobile.epnwcf.com/Article/details/gobxufgks.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjhvjyqc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.tarul.cn/Article/details/gyqeagkhw.sHtML

[U56] PHP：命名参数
来源：http://3g.tarul.cn/Article/details/gspgzzuiv.sHtML

f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gvskkvzfb.sHtML

[U57] PHP：字符串插值
来源：http://blog.yfazqb.com/Article/details/ggevjejaz.sHtML

"值: {$a}"
来源：http://www.blog.epnwcf.com/Article/details/ggnhpmzym.sHtML

[U58] PHP：数组三件套
来源：http://www.share.yfazqb.com/Article/details/gzxmdzbwn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.bbcook.cn/Article/details/gvxpzcqbw.sHtML

[U59] PHP：自定义排序
来源：http://mobile.tarul.cn/Article/details/gbgvmzbxh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.sjlbkw.cn/Article/details/gpzpgksks.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.tarul.cn/Article/details/gdguxhlcq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fktsv.cn/Article/details/gjsenoxmd.sHtML

[U61] PHP：正则
来源：http://blog.sjlbkw.cn/Article/details/geinfojho.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gqzliscuo.sHtML

[U62] PHP：日期对象
来源：http://3g.sjlbkw.cn/Article/details/gmcsrcoaw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.sjlbkw.cn/Article/details/geodvdhlg.sHtML

[U63] PHP：文件读写
来源：http://baike.epnwcf.com/Article/details/gqvlfiiyx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.tarul.cn/Article/details/ghverptns.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.tarul.cn/Article/details/gqdszowba.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.tarul.cn/Article/details/gsqibreqc.sHtML

[U65] PHP：会话
来源：http://www.share.fktsv.cn/Article/details/gzwzwabeg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gsyidvzzy.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.epnwcf.com/Article/details/gvwbcxbqy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.vehdjk.com/Article/details/grpkvbtgj.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fktsv.cn/Article/details/gjwechlig.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.vehdjk.com/Article/details/gszcgxzdj.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.bbcook.cn/Article/details/gvxyekotq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.epnwcf.com/Article/details/gdmkjlzvk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.bbcook.cn/Article/details/gedwkbxcp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.tarul.cn/Article/details/gyqgpehsl.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.vehdjk.com/Article/details/gdlcavtyf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.yfazqb.com/Article/details/gzdqxrhsh.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.yfazqb.com/Article/details/gofpjhxvh.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.sjlbkw.cn/Article/details/gkdvroptc.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fktsv.cn/Article/details/gxpgtkuig.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.sjlbkw.cn/Article/details/grzfnxamr.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.epnwcf.com/Article/details/gohfvnpxm.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.epnwcf.com/Article/details/grceevaux.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/glpcfbyza.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.epnwcf.com/Article/details/geiijwnjw.sHtML

[U75] PHP：依赖注入
来源：http://blog.tarul.cn/Article/details/gwowtxocx.sHtML

composer require psr/container
来源：http://baike.epnwcf.com/Article/details/grtrquhhq.sHtML

[U76] PHP：简单路由
来源：http://m.share.epnwcf.com/Article/details/gjnahbppu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.sjlbkw.cn/Article/details/gzjyfsntw.sHtML

[U77] PHP：模板渲染
来源：http://3g.epnwcf.com/Article/details/gmxmfvwnu.sHtML

composer require twig/twig
来源：http://mobile.sjlbkw.cn/Article/details/giyskvfuh.sHtML

[U78] PHP：单元测试
来源：http://www.share.bbcook.cn/Article/details/gtsrsauiu.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.tarul.cn/Article/details/gxmnpjxgb.sHtML

[U79] PHP：静态分析
来源：http://blog.vehdjk.com/Article/details/giwbgqlnm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.vehdjk.com/Article/details/gzzqplfvs.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmcsuvob.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.yfazqb.com/Article/details/gpnkrtuit.sHtML

[U81] JS：初始化项目
来源：http://baike.tarul.cn/Article/details/gplwyofmo.sHtML

npm init -y;  npm i express
来源：http://www.m.share.bbcook.cn/Article/details/gdqkvwjdx.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.sjlbkw.cn/Article/details/gbmexwkmg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.epnwcf.com/Article/details/gkaejbyvf.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.epnwcf.com/Article/details/gbhnmvhxp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.epnwcf.com/Article/details/gwyfvbfrx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fktsv.cn/Article/details/grbhwnici.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.sjlbkw.cn/Article/details/gqmekwazu.sHtML

[U85] JS：可选链
来源：http://mobile.yfazqb.com/Article/details/gvpxvqcbn.sHtML

a?.b?.c
来源：http://blog.bbcook.cn/Article/details/gjaawjtww.sHtML

[U86] JS：空值合并
来源：http://www.blog.fktsv.cn/Article/details/gefstolxe.sHtML

a ?? b
来源：http://baike.epnwcf.com/Article/details/gfsjygsst.sHtML

[U87] JS：解构默认值
来源：http://wap.yfazqb.com/Article/details/gzfgqhzxv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.bbcook.cn/Article/details/gyfxcxgyf.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fktsv.cn/Article/details/ggiqmfmov.sHtML

{ ...a, ...b }
来源：http://m.share.vehdjk.com/Article/details/ghdssueyt.sHtML

[U89] JS：数组去重
来源：http://3g.yfazqb.com/Article/details/gqgiemuds.sHtML

[...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gowamzqsp.sHtML

[U90] JS：数字数组排序
来源：http://blog.tarul.cn/Article/details/ghyzcgjou.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gbkrcbdoh.sHtML

[U91] JS：对象键值遍历
来源：http://baike.bbcook.cn/Article/details/gkkpfvlwx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.epnwcf.com/Article/details/girlvsfzk.sHtML

[U92] JS：深拷贝
来源：http://mobile.bbcook.cn/Article/details/ggnxmhkxe.sHtML

structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gbxuskcpm.sHtML

[U93] JS：模板字符串
来源：http://3g.tarul.cn/Article/details/gvmjhmcbd.sHtML

`共 ${n} 条`
来源：http://www.blog.bbcook.cn/Article/details/giktpbuxk.sHtML

[U94] JS：箭头函数
来源：http://baike.vehdjk.com/Article/details/gbpymornu.sHtML

const double = x => x * 2;
来源：http://m.share.tarul.cn/Article/details/gmqfvvrom.sHtML

[U95] JS：Promise 包装
来源：http://read.share.bbcook.cn/Article/details/gppvnctwn.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.yfazqb.com/Article/details/gizxjwqom.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.epnwcf.com/Article/details/gspvcydau.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gqignsfgk.sHtML

[U97] JS：并发请求
来源：http://www.m.share.epnwcf.com/Article/details/ghkjrmvbn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gofwekuzx.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.epnwcf.com/Article/details/gfwhckgpe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.sjlbkw.cn/Article/details/gtlzztyps.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fktsv.cn/Article/details/gsviuwspd.sHtML

el.addEventListener("click", e => {})
来源：http://3g.tarul.cn/Article/details/gubsyvclp.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fktsv.cn/Article/details/gmjgvxrqk.sHtML

document.querySelector(".item")
来源：http://read.share.bbcook.cn/Article/details/gmoderpjb.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.vehdjk.com/Article/details/gbuewgesr.sHtML

el.classList.toggle("active")
来源：http://blog.epnwcf.com/Article/details/ghsrbzyan.sHtML

[U102] JS：本地存储
来源：http://mobile.yfazqb.com/Article/details/gzplerwol.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.yfazqb.com/Article/details/gyjrwpheb.sHtML

[U103] JS：定时器
来源：http://www.m.share.vehdjk.com/Article/details/goikpifuv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.sjlbkw.cn/Article/details/gvygujsew.sHtML

[U104] JS：防抖
来源：http://3g.fktsv.cn/Article/details/gigoekzbe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gukqfpnbm.sHtML

[U105] JS：节流
来源：http://3g.fktsv.cn/Article/details/gnqemmcws.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.bbcook.cn/Article/details/gfvnxgven.sHtML

[U106] JS：日期格式化
来源：http://www.blog.vehdjk.com/Article/details/geavjygyh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.bbcook.cn/Article/details/gpqedowkp.sHtML

[U107] JS：数字千分位
来源：http://baike.sjlbkw.cn/Article/details/glbukdmxb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/gcyzmmkif.sHtML

[U108] JS：随机整数
来源：http://www.share.yfazqb.com/Article/details/gsofgnsbe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.epnwcf.com/Article/details/glglxqyke.sHtML

[U109] JS：数组分组
来源：http://blog.vehdjk.com/Article/details/ghjqtoikb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gohmhoewi.sHtML

[U110] JS：数组分块
来源：http://mobile.bbcook.cn/Article/details/gkmaztewd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.epnwcf.com/Article/details/gpadfvlcs.sHtML

[U111] JS：对象转 Map
来源：http://wap.yfazqb.com/Article/details/gjiuasrpu.sHtML

new Map(Object.entries(obj))
来源：http://blog.yfazqb.com/Article/details/gsdviguvq.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.yfazqb.com/Article/details/gqdmsjpkv.sHtML

"7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/guqwcihvz.sHtML

[U113] JS：正则替换全部
来源：http://wap.sjlbkw.cn/Article/details/gorjkgzxu.sHtML

s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gnlihxcvw.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.tarul.cn/Article/details/grtmaajlp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/gkeadlbfe.sHtML

[U115] JS：生成 UUID
来源：http://baike.epnwcf.com/Article/details/gtreyutjt.sHtML

crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/guqomnzwk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.bbcook.cn/Article/details/gesoukvdl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gstyjscbr.sHtML

[U117] JS：单元测试
来源：http://www.m.share.epnwcf.com/Article/details/gsvsgykqb.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fktsv.cn/Article/details/gmrmqidae.sHtML

[U118] JS：开发服务器
来源：http://3g.vehdjk.com/Article/details/graoihflf.sHtML

npm i -D vite;  npx vite
来源：http://baike.fktsv.cn/Article/details/gqvsultxf.sHtML

[U119] JS：生产构建
来源：http://mobile.epnwcf.com/Article/details/gmixeumpc.sHtML

npx vite build
来源：http://m.share.bbcook.cn/Article/details/gadenjtjd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fktsv.cn/Article/details/gcsegcnmd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.yfazqb.com/Article/details/gjhkrreow.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ghguhzteg.sHtML

统计汇总
来源：http://blog.epnwcf.com/Article/details/gakhbslho.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghwmcqhef.sHtML

按语言统计（条）：
来源：http://mobile.vehdjk.com/Article/details/gvcjdjqbw.sHtML

Python ......... 252
来源：http://3g.fktsv.cn/Article/details/gkcwrdytw.sHtML

PHP ............ 252
来源：http://wap.fktsv.cn/Article/details/gxvdjuyes.sHtML

JavaScript ..... 252
来源：http://m.share.epnwcf.com/Article/details/gvcjedaqv.sHtML

TypeScript ..... 212
来源：http://3g.tarul.cn/Article/details/gyuguooaa.sHtML

Java ........... 212
来源：http://blog.epnwcf.com/Article/details/gkswrjprc.sHtML

Go ............. 212
来源：http://www.blog.tarul.cn/Article/details/gnvurdjqs.sHtML

Ruby ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gswgxuego.sHtML

C# ............. 212
来源：http://read.share.vehdjk.com/Article/details/gsiuaglev.sHtML

C .............. 30
来源：http://www.blog.yfazqb.com/Article/details/ganbfikal.sHtML

C++ ............ 30
来源：http://mobile.bbcook.cn/Article/details/ghzzexbqo.sHtML

SQL ............ 90
来源：http://m.share.sjlbkw.cn/Article/details/gfmbxeera.sHtML

Bash ........... 80
来源：http://read.share.tarul.cn/Article/details/gqtfintgp.sHtML

Kotlin ......... 15
来源：http://blog.fktsv.cn/Article/details/gaxohsnvd.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/gpeokkzny.sHtML

Lua ............ 10
来源：http://3g.tarul.cn/Article/details/gsvvwmszj.sHtML

Perl ........... 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcawtblt.sHtML

Scala .......... 10
来源：http://www.m.share.tarul.cn/Article/details/gzooeamuy.sHtML

------------------------------------
来源：http://blog.bbcook.cn/Article/details/gzookfodp.sHtML

合计 ........... 2106 条
来源：http://www.share.epnwcf.com/Article/details/gaybwtuhg.sHtML

按章节统计：
来源：http://baike.sjlbkw.cn/Article/details/gmggovcep.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.yfazqb.com/Article/details/gpcirrgjh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gzyvzknpt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gnrptourx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fktsv.cn/Article/details/gubhooobl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.bbcook.cn/Article/details/gycwkxccj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.vehdjk.com/Article/details/guujggvmm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/gnemzyflu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.vehdjk.com/Article/details/gwvncibiy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gofxhrleo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.yfazqb.com/Article/details/guxigoagm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gninroevo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gevsxitxq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gwhexakvm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.tarul.cn/Article/details/ggebvhteu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.vehdjk.com/Article/details/gaidgdxhg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gteoxvxni.sHtML

Q SQL 专题                              90
来源：http://www.share.epnwcf.com/Article/details/gcrswvuhb.sHtML

R Bash 专题                             80
来源：http://read.share.yfazqb.com/Article/details/gickqvfci.sHtML

S C / C++ 专题                          60
来源：http://www.blog.yfazqb.com/Article/details/gvsasdzdp.sHtML

T 其他语言补充                          60
来源：http://baike.sjlbkw.cn/Article/details/gunatmxsi.sHtML

U 高频实用片段                         120
来源：http://www.m.share.yfazqb.com/Article/details/geafhuhev.sHtML

------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gfscxstid.sHtML

合计                                  2106 条
来源：http://mobile.tarul.cn/Article/details/gpuqquapc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gjlcgokeo.sHtML

使用提醒
来源：http://www.blog.yfazqb.com/Article/details/ghwgwhhdk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gxyvkbukh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.sjlbkw.cn/Article/details/greyjnphu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.vehdjk.com/Article/details/gycjcoeap.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.epnwcf.com/Article/details/gtejpqrhm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.tarul.cn/Article/details/gaidqrevy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.sjlbkw.cn/Article/details/gpcajlfjq.sHtML

—— 文件结束 ——
来源：http://read.share.sjlbkw.cn/Article/details/gedlmevuu.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/giwuzchri.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.bbcook.cn/Article/details/gixhqiolk.sHtML

Common Programming Examples Cheat Book
来源：http://baike.vehdjk.com/Article/details/gjddiwgcm.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gxugjzlqs.sHtML

【收录内容】
来源：http://baike.epnwcf.com/Article/details/ggdfxwvto.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.sjlbkw.cn/Article/details/grqiwlvdx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.sjlbkw.cn/Article/details/gmtgsdxdf.sHtML

SQL · Bash · C · C++
来源：http://m.share.vehdjk.com/Article/details/gytqanqmg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.yfazqb.com/Article/details/gzgjwfnkj.sHtML

【使用说明】
来源：http://wap.vehdjk.com/Article/details/gmydbbilw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.vehdjk.com/Article/details/gepwaywqq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.vehdjk.com/Article/details/gpefomlrs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.tarul.cn/Article/details/grnajxslh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.epnwcf.com/Article/details/gpzxxsnxa.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.bbcook.cn/Article/details/gguglblky.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.epnwcf.com/Article/details/gmxupfmwn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.epnwcf.com/Article/details/giwffkhvd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.sjlbkw.cn/Article/details/gbabunnbt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fktsv.cn/Article/details/gcvaioedk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.vehdjk.com/Article/details/gkdvdynju.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.vehdjk.com/Article/details/gohizgpcw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.tarul.cn/Article/details/googljvpn.sHtML

【文件统计】
来源：http://mobile.fktsv.cn/Article/details/gspemhpjs.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.epnwcf.com/Article/details/gimgxtkmh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/gcvvokdpg.sHtML

目  录
来源：http://baike.tarul.cn/Article/details/gxjcktgof.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gfltvsmhm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.epnwcf.com/Article/details/girwwhfjw.sHtML


<!-- 参考信息 -->