代发 wailian999

[U15] Py：高精度计时
来源：http://www.blog.bbcook.cn/Article/details/gomkptade.sHtML

t = time.perf_counter()
来源：http://wap.epnwcf.com/Article/details/gxbjvqltz.sHtML

[U16] Py：命令行参数解析
来源：http://blog.vehdjk.com/Article/details/glxgcvpgb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.bbcook.cn/Article/details/gfuszubsn.sHtML

[U17] Py：初始化日志
来源：http://3g.vehdjk.com/Article/details/gbwhqqpdp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fktsv.cn/Article/details/galcwgwpb.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.sjlbkw.cn/Article/details/gopvxscjp.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.sjlbkw.cn/Article/details/grvybmqng.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.epnwcf.com/Article/details/gmjlkidjf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fktsv.cn/Article/details/gpdsjeudy.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fktsv.cn/Article/details/gnzwcubwj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.epnwcf.com/Article/details/gghxmmpwo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.epnwcf.com/Article/details/gbomuqlab.sHtML

@contextlib.contextmanager
来源：http://blog.sjlbkw.cn/Article/details/gybpfqiwh.sHtML

[U22] Py：矩阵转置
来源：http://mobile.bbcook.cn/Article/details/gytagzidz.sHtML

list(zip(*m))
来源：http://mobile.tarul.cn/Article/details/gqdwwwctl.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.epnwcf.com/Article/details/gezfqqfet.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.vehdjk.com/Article/details/gtnsefexa.sHtML

[U24] Py：路径操作
来源：http://blog.vehdjk.com/Article/details/gphxukaan.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/gtscddege.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.epnwcf.com/Article/details/gabqmxqtf.sHtML

csv.DictReader(f)
来源：http://blog.yfazqb.com/Article/details/gcabrujqy.sHtML

[U26] Py：并发下载
来源：http://www.m.share.vehdjk.com/Article/details/gxecriihi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.tarul.cn/Article/details/gergxmjwy.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.epnwcf.com/Article/details/gykdvuryr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.epnwcf.com/Article/details/gkwpcgfcs.sHtML

[U28] Py：类型别名
来源：http://blog.vehdjk.com/Article/details/gwdanqgkw.sHtML

UserId = int
来源：http://m.share.vehdjk.com/Article/details/gwwrgdnmv.sHtML

[U29] Py：属性校验
来源：http://3g.epnwcf.com/Article/details/gxujxmzem.sHtML

@property 与 @x.setter 配合
来源：http://3g.vehdjk.com/Article/details/ggswyolpi.sHtML

[U30] Py：数据类
来源：http://3g.bbcook.cn/Article/details/grqunusxw.sHtML

@dataclass(slots=True)
来源：http://3g.vehdjk.com/Article/details/gufbdtcwe.sHtML

[U31] Py：单测
来源：http://3g.sjlbkw.cn/Article/details/goequctki.sHtML

python -m pytest -q
来源：http://mobile.vehdjk.com/Article/details/gqyztvbuf.sHtML

[U32] Py：代码格式化
来源：http://mobile.bbcook.cn/Article/details/gnglpofyf.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.vehdjk.com/Article/details/gdsgctgui.sHtML

[U33] Py：打包发布
来源：http://wap.bbcook.cn/Article/details/gitrcrari.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.sjlbkw.cn/Article/details/gooywwzvq.sHtML

[U34] Py：判断编码
来源：http://3g.tarul.cn/Article/details/gsbvicjaw.sHtML

chardet.detect(raw)
来源：http://m.share.vehdjk.com/Article/details/gbclmkfwe.sHtML

[U35] Py：发送邮件
来源：http://mobile.bbcook.cn/Article/details/gpspcibkz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.bbcook.cn/Article/details/gxwyqximc.sHtML

[U36] Py：定时任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdoaixfx.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.sjlbkw.cn/Article/details/gntfbjdrx.sHtML

[U37] Py：读写 Excel
来源：http://read.share.vehdjk.com/Article/details/gwntgarel.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fktsv.cn/Article/details/gevtjavsf.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.sjlbkw.cn/Article/details/glwkiefjm.sHtML

Path(__file__).resolve().parent
来源：http://wap.vehdjk.com/Article/details/gpnebrndl.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.yfazqb.com/Article/details/gfpzasggq.sHtML

sys.stdout.isatty()
来源：http://m.share.sjlbkw.cn/Article/details/gzfwgpcqh.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.vehdjk.com/Article/details/guxccnxfh.sHtML

print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/gadhlobpe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.epnwcf.com/Article/details/gnmxfibwq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.bbcook.cn/Article/details/ghaqrkazh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.sjlbkw.cn/Article/details/gfgdysryd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.yfazqb.com/Article/details/ghikxquuv.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gbjcmtpyg.sHtML

namespace App\Http;
来源：http://www.share.fktsv.cn/Article/details/gmtsxspuh.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fktsv.cn/Article/details/gorufanwz.sHtML

declare(strict_types=1);
来源：http://read.share.sjlbkw.cn/Article/details/gplbwcdkz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.tarul.cn/Article/details/gmvhrwssw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gnwcltjcl.sHtML

[U46] PHP：可空类型
来源：http://blog.bbcook.cn/Article/details/gnokjjdoj.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gtwgcedce.sHtML

[U47] PHP：联合类型
来源：http://www.blog.sjlbkw.cn/Article/details/gjcnzlopn.sHtML

int|string $id
来源：http://www.share.tarul.cn/Article/details/gjejqtcbw.sHtML

[U48] PHP：纯枚举
来源：http://mobile.bbcook.cn/Article/details/gspsvkjdh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.tarul.cn/Article/details/geieixedw.sHtML

[U49] PHP：只读属性
来源：http://www.blog.yfazqb.com/Article/details/gppvyzlzt.sHtML

public readonly string $name
来源：http://m.share.tarul.cn/Article/details/gpvwfauwn.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.bbcook.cn/Article/details/gdmkkezcn.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fktsv.cn/Article/details/grnefhnck.sHtML

[U51] PHP：数组解构
来源：http://read.share.vehdjk.com/Article/details/gqpifddvb.sHtML

[$a, $b] = $arr;
来源：http://www.blog.bbcook.cn/Article/details/gadyxanxj.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fktsv.cn/Article/details/ghtqbmzwh.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.yfazqb.com/Article/details/gfivdbtuw.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fktsv.cn/Article/details/gepfgzuwd.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fktsv.cn/Article/details/gvcdlxoxg.sHtML

[U54] PHP：空安全调用
来源：http://3g.tarul.cn/Article/details/gbqdacywl.sHtML

$obj?->method()
来源：http://blog.bbcook.cn/Article/details/gyhxmvbxw.sHtML

[U55] PHP：match 表达式
来源：http://wap.bbcook.cn/Article/details/gbvjtbjbf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.sjlbkw.cn/Article/details/gdpouyghf.sHtML

[U56] PHP：命名参数
来源：http://wap.fktsv.cn/Article/details/glrhlqtho.sHtML

f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gumitqriy.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/giudivqnz.sHtML

"值: {$a}"
来源：http://mobile.yfazqb.com/Article/details/gesxuccyb.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.epnwcf.com/Article/details/gncgtjthh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fktsv.cn/Article/details/ghiqdsugr.sHtML

[U59] PHP：自定义排序
来源：http://blog.vehdjk.com/Article/details/gquwccaaa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gmygsfikh.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.epnwcf.com/Article/details/guycbegha.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.bbcook.cn/Article/details/gyltyrvjh.sHtML

[U61] PHP：正则
来源：http://m.share.sjlbkw.cn/Article/details/goqkarmqp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.epnwcf.com/Article/details/gbbjwlrcz.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.tarul.cn/Article/details/gnrcviuti.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fktsv.cn/Article/details/ghdrxirvn.sHtML

[U63] PHP：文件读写
来源：http://blog.sjlbkw.cn/Article/details/gjqrqnrlg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.vehdjk.com/Article/details/ghcskdkre.sHtML

[U64] PHP：目录遍历
来源：http://3g.tarul.cn/Article/details/gbdyckoll.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.tarul.cn/Article/details/guedauuen.sHtML

[U65] PHP：会话
来源：http://wap.fktsv.cn/Article/details/gkuyarsnm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.tarul.cn/Article/details/gdsdjdqfb.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.yfazqb.com/Article/details/ggyofvzst.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.yfazqb.com/Article/details/gcfrskgem.sHtML

[U67] PHP：处理文件上传
来源：http://baike.vehdjk.com/Article/details/gqiefvwve.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.yfazqb.com/Article/details/gmvuozydk.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.vehdjk.com/Article/details/gjdkmlpzs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.yfazqb.com/Article/details/gnzmiibtf.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.vehdjk.com/Article/details/gkhnxqcbr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.vehdjk.com/Article/details/gwbxnxlrb.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.sjlbkw.cn/Article/details/gwasfaboy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.vehdjk.com/Article/details/gkwwoucnd.sHtML

[U71] PHP：抛出异常
来源：http://wap.epnwcf.com/Article/details/gowwehfpd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fktsv.cn/Article/details/glaofofyo.sHtML

[U72] PHP：写错误日志
来源：http://read.share.yfazqb.com/Article/details/gklaskltl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.yfazqb.com/Article/details/gvqpllhvh.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.bbcook.cn/Article/details/gyehonzvn.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.tarul.cn/Article/details/gmakwxcfi.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.yfazqb.com/Article/details/gfzvsmtkt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.sjlbkw.cn/Article/details/garhjphsr.sHtML

[U75] PHP：依赖注入
来源：http://www.share.vehdjk.com/Article/details/gluflerib.sHtML

composer require psr/container
来源：http://mobile.yfazqb.com/Article/details/gykdcyycg.sHtML

[U76] PHP：简单路由
来源：http://www.blog.epnwcf.com/Article/details/gzntgcwns.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.epnwcf.com/Article/details/gwfeomqcx.sHtML

[U77] PHP：模板渲染
来源：http://read.share.vehdjk.com/Article/details/gfynynebg.sHtML

composer require twig/twig
来源：http://www.m.share.sjlbkw.cn/Article/details/gqydtiprb.sHtML

[U78] PHP：单元测试
来源：http://blog.yfazqb.com/Article/details/gqkrioued.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.tarul.cn/Article/details/gfqpmpklt.sHtML

[U79] PHP：静态分析
来源：http://read.share.sjlbkw.cn/Article/details/gjboanndn.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.yfazqb.com/Article/details/gaxjppnex.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.yfazqb.com/Article/details/gbmvpbsgd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.tarul.cn/Article/details/gqcwxilfj.sHtML

[U81] JS：初始化项目
来源：http://read.share.bbcook.cn/Article/details/gidzennfw.sHtML

npm init -y;  npm i express
来源：http://www.share.epnwcf.com/Article/details/gwipieioc.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fktsv.cn/Article/details/gpexxjbqu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.tarul.cn/Article/details/gbdgpnojn.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.sjlbkw.cn/Article/details/gdlttaylg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.tarul.cn/Article/details/gonpfdtcn.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.epnwcf.com/Article/details/gbgsgenrg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.sjlbkw.cn/Article/details/grwchsnbx.sHtML

[U85] JS：可选链
来源：http://www.m.share.vehdjk.com/Article/details/gbgbiajee.sHtML

a?.b?.c
来源：http://read.share.vehdjk.com/Article/details/glvcaqaif.sHtML

[U86] JS：空值合并
来源：http://m.share.epnwcf.com/Article/details/gjaaqrjgu.sHtML

a ?? b
来源：http://read.share.yfazqb.com/Article/details/gaoqjousu.sHtML

[U87] JS：解构默认值
来源：http://3g.sjlbkw.cn/Article/details/gclavzxtn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.yfazqb.com/Article/details/gicfqebuw.sHtML

[U88] JS：对象展开合并
来源：http://baike.yfazqb.com/Article/details/gfjwjhsik.sHtML

{ ...a, ...b }
来源：http://www.blog.tarul.cn/Article/details/gcgtivavq.sHtML

[U89] JS：数组去重
来源：http://wap.sjlbkw.cn/Article/details/glgjmswhb.sHtML

[...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gozjaxffo.sHtML

[U90] JS：数字数组排序
来源：http://blog.tarul.cn/Article/details/gczkrklcy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gohfsfctc.sHtML

[U91] JS：对象键值遍历
来源：http://baike.tarul.cn/Article/details/gqiiirwhj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.yfazqb.com/Article/details/gskkknuyz.sHtML

[U92] JS：深拷贝
来源：http://m.share.bbcook.cn/Article/details/gglobzwgc.sHtML

structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/ghovmmhjs.sHtML

[U93] JS：模板字符串
来源：http://read.share.yfazqb.com/Article/details/gcsyamesy.sHtML

`共 ${n} 条`
来源：http://3g.vehdjk.com/Article/details/ggmybcsgw.sHtML

[U94] JS：箭头函数
来源：http://3g.bbcook.cn/Article/details/guzcjemjg.sHtML

const double = x => x * 2;
来源：http://www.blog.epnwcf.com/Article/details/gppgnayvo.sHtML

[U95] JS：Promise 包装
来源：http://3g.fktsv.cn/Article/details/gdsyaqzsr.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.vehdjk.com/Article/details/gujmtpudd.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.vehdjk.com/Article/details/gtbedbzbc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gfuugusvt.sHtML

[U97] JS：并发请求
来源：http://read.share.sjlbkw.cn/Article/details/guraxtqfy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gpjpmlvsf.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.bbcook.cn/Article/details/gpbveavla.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.vehdjk.com/Article/details/gtkpgiolx.sHtML

[U99] JS：事件监听
来源：http://read.share.tarul.cn/Article/details/gfkaqokzw.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.yfazqb.com/Article/details/gtrqxdfwn.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fktsv.cn/Article/details/gbmtnrnrg.sHtML

document.querySelector(".item")
来源：http://baike.epnwcf.com/Article/details/gxzuguzir.sHtML

[U101] JS：classList 操作
来源：http://m.share.epnwcf.com/Article/details/gpubxosaf.sHtML

el.classList.toggle("active")
来源：http://www.share.sjlbkw.cn/Article/details/givwjuzna.sHtML

[U102] JS：本地存储
来源：http://wap.epnwcf.com/Article/details/gmsorbtzz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.vehdjk.com/Article/details/gczrhgmew.sHtML

[U103] JS：定时器
来源：http://blog.vehdjk.com/Article/details/gfyohozfa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.vehdjk.com/Article/details/grxzpisjf.sHtML

[U104] JS：防抖
来源：http://blog.fktsv.cn/Article/details/gqsdkzepr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gsoaawnbe.sHtML

[U105] JS：节流
来源：http://m.share.sjlbkw.cn/Article/details/gjmxuphki.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fktsv.cn/Article/details/gimombwoi.sHtML

[U106] JS：日期格式化
来源：http://baike.vehdjk.com/Article/details/grwunofpv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.bbcook.cn/Article/details/gsugnwsar.sHtML

[U107] JS：数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gyuobsfik.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gxvdujxcy.sHtML

[U108] JS：随机整数
来源：http://m.share.tarul.cn/Article/details/gsnpnwmwe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fktsv.cn/Article/details/gknlsjefr.sHtML

[U109] JS：数组分组
来源：http://baike.sjlbkw.cn/Article/details/gtmzeljvw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gszpcbxfs.sHtML

[U110] JS：数组分块
来源：http://mobile.bbcook.cn/Article/details/ggsyjhwxq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.vehdjk.com/Article/details/gstitebis.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fktsv.cn/Article/details/gvmrlhcjv.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.bbcook.cn/Article/details/gswoewnqb.sHtML

[U112] JS：字符串补位
来源：http://blog.sjlbkw.cn/Article/details/gcyvgimmd.sHtML

"7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/ghixnbdzw.sHtML

[U113] JS：正则替换全部
来源：http://blog.yfazqb.com/Article/details/glbmamlyd.sHtML

s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gxjzeanwr.sHtML

[U114] JS：JSON 深比较
来源：http://baike.vehdjk.com/Article/details/ghmwblwcb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrrsiqxt.sHtML

[U115] JS：生成 UUID
来源：http://baike.epnwcf.com/Article/details/gqprggeha.sHtML

crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gqbswheyt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.vehdjk.com/Article/details/gusdsgfct.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.epnwcf.com/Article/details/gygcoykdn.sHtML

[U117] JS：单元测试
来源：http://3g.sjlbkw.cn/Article/details/gvaqlknsq.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.vehdjk.com/Article/details/gkvvtvefe.sHtML

[U118] JS：开发服务器
来源：http://3g.sjlbkw.cn/Article/details/gigabspah.sHtML

npm i -D vite;  npx vite
来源：http://blog.fktsv.cn/Article/details/gqahezztd.sHtML

[U119] JS：生产构建
来源：http://baike.yfazqb.com/Article/details/gcqoxzqbj.sHtML

npx vite build
来源：http://read.share.epnwcf.com/Article/details/gitoielvt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.vehdjk.com/Article/details/gnqhmgktm.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.yfazqb.com/Article/details/gaoyotoes.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gggedvaom.sHtML

统计汇总
来源：http://www.share.epnwcf.com/Article/details/ggumigqjt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcpnkqtvh.sHtML

按语言统计（条）：
来源：http://www.blog.sjlbkw.cn/Article/details/gbsrrodpu.sHtML

Python ......... 252
来源：http://m.share.vehdjk.com/Article/details/gazsepssw.sHtML

PHP ............ 252
来源：http://baike.tarul.cn/Article/details/glxfcfmro.sHtML

JavaScript ..... 252
来源：http://baike.tarul.cn/Article/details/gxfejnfsc.sHtML

TypeScript ..... 212
来源：http://mobile.tarul.cn/Article/details/gdgenyekg.sHtML

Java ........... 212
来源：http://blog.sjlbkw.cn/Article/details/gmnssboku.sHtML

Go ............. 212
来源：http://www.m.share.yfazqb.com/Article/details/graynngvz.sHtML

Ruby ........... 212
来源：http://blog.vehdjk.com/Article/details/gogtsrmwf.sHtML

C# ............. 212
来源：http://blog.epnwcf.com/Article/details/gflmduyni.sHtML

C .............. 30
来源：http://baike.sjlbkw.cn/Article/details/gpqztlviv.sHtML

C++ ............ 30
来源：http://mobile.vehdjk.com/Article/details/gifbcvznb.sHtML

SQL ............ 90
来源：http://www.m.share.epnwcf.com/Article/details/gpkenxrtx.sHtML

Bash ........... 80
来源：http://m.share.yfazqb.com/Article/details/gutxkodmu.sHtML

Kotlin ......... 15
来源：http://m.share.yfazqb.com/Article/details/gaempkdvy.sHtML

Swift .......... 15
来源：http://www.share.yfazqb.com/Article/details/gujfewzgw.sHtML

Lua ............ 10
来源：http://www.m.share.vehdjk.com/Article/details/gvahudgul.sHtML

Perl ........... 10
来源：http://www.blog.sjlbkw.cn/Article/details/gvdfhetwi.sHtML

Scala .......... 10
来源：http://m.share.vehdjk.com/Article/details/goutkfoxu.sHtML

------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gvnydnkva.sHtML

合计 ........... 2106 条
来源：http://www.blog.sjlbkw.cn/Article/details/gvplfbltk.sHtML

按章节统计：
来源：http://www.blog.tarul.cn/Article/details/gulvatbdj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.yfazqb.com/Article/details/ghtgyehrh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/grduyxjsk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gijvafjug.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/gowbmgfci.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.tarul.cn/Article/details/gaicqokip.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fktsv.cn/Article/details/gexxnmngn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/guvwdbwqv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/gxiftzjov.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/ggqwhrjzw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/gzkcpzqpe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/geahrwbjn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gwyfjynhc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gcfowrzcc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/ggsvwbrgt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.sjlbkw.cn/Article/details/gzhymztxk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/grhpwspmz.sHtML

Q SQL 专题                              90
来源：http://mobile.yfazqb.com/Article/details/grrsvygrs.sHtML

R Bash 专题                             80
来源：http://wap.sjlbkw.cn/Article/details/glfagpjwe.sHtML

S C / C++ 专题                          60
来源：http://blog.epnwcf.com/Article/details/gpqjxniis.sHtML

T 其他语言补充                          60
来源：http://www.blog.bbcook.cn/Article/details/gquuuraul.sHtML

U 高频实用片段                         120
来源：http://www.blog.sjlbkw.cn/Article/details/gxbggpfgv.sHtML

------------------------------------
来源：http://baike.yfazqb.com/Article/details/gowuarsmp.sHtML

合计                                  2106 条
来源：http://m.share.sjlbkw.cn/Article/details/gdciugfox.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gdiocwtyy.sHtML

使用提醒
来源：http://baike.tarul.cn/Article/details/gcgrkwgzi.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gsjxeqepa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.tarul.cn/Article/details/gjzhxwlkv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.tarul.cn/Article/details/gcowpjnud.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.tarul.cn/Article/details/gfgktvaqf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.tarul.cn/Article/details/gcdhcnvey.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.tarul.cn/Article/details/gbhmsuzje.sHtML

—— 文件结束 ——
来源：http://3g.fktsv.cn/Article/details/gyotjsrjo.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gnqhurzrp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.epnwcf.com/Article/details/gqvmmpnpy.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.epnwcf.com/Article/details/gzismyxbf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gfvbdxuct.sHtML

【收录内容】
来源：http://wap.epnwcf.com/Article/details/gwqpcwyeq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.bbcook.cn/Article/details/gkmtfxqnp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.epnwcf.com/Article/details/gaqjqnott.sHtML

SQL · Bash · C · C++
来源：http://mobile.bbcook.cn/Article/details/gnovaguqp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.epnwcf.com/Article/details/gloaltsbv.sHtML

【使用说明】
来源：http://3g.bbcook.cn/Article/details/gpwjvskjz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.tarul.cn/Article/details/ghhhuaxjn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.sjlbkw.cn/Article/details/gczgxefww.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.yfazqb.com/Article/details/gsftefrbe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.vehdjk.com/Article/details/gfwmkscbu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fktsv.cn/Article/details/grggkpizw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.epnwcf.com/Article/details/gjkvbshut.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.sjlbkw.cn/Article/details/gyucfijav.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.yfazqb.com/Article/details/goiovkhtx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.yfazqb.com/Article/details/gisvyjnpl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.epnwcf.com/Article/details/gozfmsmmh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.epnwcf.com/Article/details/gkgkltssa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.sjlbkw.cn/Article/details/gpcmqdyjo.sHtML

【文件统计】
来源：http://read.share.bbcook.cn/Article/details/gibrtdewg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fktsv.cn/Article/details/gcehahhhy.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.tarul.cn/Article/details/gxgxpnrbb.sHtML

目  录
来源：http://blog.sjlbkw.cn/Article/details/gihtzebud.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/grrejjyst.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.sjlbkw.cn/Article/details/gwoxmycca.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/gsfdwlxrq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.yfazqb.com/Article/details/gfcsduupy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.epnwcf.com/Article/details/gtyofocsv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdeofgam.sHtML


<!-- 参考信息 -->