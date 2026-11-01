代发 wailian999

[U13] Py：固定长度队列
来源：http://m.share.tarul.cn/Article/details/gtroijpas.sHtML

deque(maxlen=10)
来源：http://blog.epnwcf.com/Article/details/ggnurdiyb.sHtML

[U14] Py：分组收集到列表
来源：http://baike.tarul.cn/Article/details/ghguzyyhp.sHtML

defaultdict(list)
来源：http://3g.vehdjk.com/Article/details/gpgsfvdri.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fktsv.cn/Article/details/gohhigsgq.sHtML

t = time.perf_counter()
来源：http://m.share.fktsv.cn/Article/details/gprxmkexl.sHtML

[U16] Py：命令行参数解析
来源：http://baike.bbcook.cn/Article/details/gthpvhbfi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.bbcook.cn/Article/details/gcwmxdzxp.sHtML

[U17] Py：初始化日志
来源：http://blog.vehdjk.com/Article/details/gcfnserek.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fktsv.cn/Article/details/glpnukusv.sHtML

[U18] Py：预编译正则
来源：http://www.share.tarul.cn/Article/details/ghpxmgjis.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fktsv.cn/Article/details/gpntnqviw.sHtML

[U19] Py：正则替换带回调
来源：http://blog.yfazqb.com/Article/details/gjkaqxjme.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.epnwcf.com/Article/details/guvbjcwsk.sHtML

[U20] Py：缓存函数结果
来源：http://wap.sjlbkw.cn/Article/details/goehcwkco.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.epnwcf.com/Article/details/glbmcryec.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.epnwcf.com/Article/details/gnfmytanx.sHtML

@contextlib.contextmanager
来源：http://blog.epnwcf.com/Article/details/gjlmyyuaw.sHtML

[U22] Py：矩阵转置
来源：http://mobile.epnwcf.com/Article/details/goelkmkjx.sHtML

list(zip(*m))
来源：http://3g.bbcook.cn/Article/details/gbjtpwfkk.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/grzksexrb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.epnwcf.com/Article/details/gqqmxsihs.sHtML

[U24] Py：路径操作
来源：http://3g.vehdjk.com/Article/details/ggnqdmypk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gjrgmedvd.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.yfazqb.com/Article/details/gatsijeon.sHtML

csv.DictReader(f)
来源：http://www.share.yfazqb.com/Article/details/gejmjnjau.sHtML

[U26] Py：并发下载
来源：http://wap.tarul.cn/Article/details/gjyfnvmkr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.vehdjk.com/Article/details/gbeorycnb.sHtML

[U27] Py：异步 HTTP
来源：http://3g.epnwcf.com/Article/details/glhvajvrg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fktsv.cn/Article/details/gcemirqbh.sHtML

[U28] Py：类型别名
来源：http://m.share.epnwcf.com/Article/details/goifinxpc.sHtML

UserId = int
来源：http://m.share.tarul.cn/Article/details/gefjshjfl.sHtML

[U29] Py：属性校验
来源：http://baike.tarul.cn/Article/details/ghnmynozb.sHtML

@property 与 @x.setter 配合
来源：http://mobile.bbcook.cn/Article/details/gmtmizsqk.sHtML

[U30] Py：数据类
来源：http://3g.tarul.cn/Article/details/grchzcrod.sHtML

@dataclass(slots=True)
来源：http://www.share.vehdjk.com/Article/details/gdatxurok.sHtML

[U31] Py：单测
来源：http://blog.bbcook.cn/Article/details/gkrrxwqdp.sHtML

python -m pytest -q
来源：http://mobile.tarul.cn/Article/details/gpzkbvofq.sHtML

[U32] Py：代码格式化
来源：http://www.share.yfazqb.com/Article/details/gfmzfckcg.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.sjlbkw.cn/Article/details/gjaoyulfd.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fktsv.cn/Article/details/gbonrtqxd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.yfazqb.com/Article/details/glsbjjqaq.sHtML

[U34] Py：判断编码
来源：http://m.share.epnwcf.com/Article/details/gvomzifua.sHtML

chardet.detect(raw)
来源：http://m.share.yfazqb.com/Article/details/gjarjbjlg.sHtML

[U35] Py：发送邮件
来源：http://mobile.epnwcf.com/Article/details/gwyczdhul.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.yfazqb.com/Article/details/gzqeozukr.sHtML

[U36] Py：定时任务
来源：http://www.blog.bbcook.cn/Article/details/gqunznthg.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fktsv.cn/Article/details/gpzotqkqb.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.tarul.cn/Article/details/grdkphqcx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.bbcook.cn/Article/details/gutgrnyjz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fktsv.cn/Article/details/gfugcaueo.sHtML

Path(__file__).resolve().parent
来源：http://mobile.tarul.cn/Article/details/gkuxojneh.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.tarul.cn/Article/details/gklqyfzfi.sHtML

sys.stdout.isatty()
来源：http://mobile.sjlbkw.cn/Article/details/gvnbskjly.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.yfazqb.com/Article/details/gckpndwof.sHtML

print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/geqzjbkqv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.tarul.cn/Article/details/gxkesfmdz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.sjlbkw.cn/Article/details/guhcyiadc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.bbcook.cn/Article/details/gltiokepw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.sjlbkw.cn/Article/details/gkqrvbnan.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.yfazqb.com/Article/details/gdluqkgom.sHtML

namespace App\Http;
来源：http://blog.bbcook.cn/Article/details/glhrilawe.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.vehdjk.com/Article/details/gztrpzekj.sHtML

declare(strict_types=1);
来源：http://blog.fktsv.cn/Article/details/gpapwmlwb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.yfazqb.com/Article/details/gozoljcpm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gcijxiibv.sHtML

[U46] PHP：可空类型
来源：http://mobile.epnwcf.com/Article/details/gicplvqfk.sHtML

?string $name = null
来源：http://read.share.bbcook.cn/Article/details/gjxpmogqi.sHtML

[U47] PHP：联合类型
来源：http://blog.sjlbkw.cn/Article/details/gywiqdnbk.sHtML

int|string $id
来源：http://www.m.share.fktsv.cn/Article/details/gqnteituy.sHtML

[U48] PHP：纯枚举
来源：http://wap.yfazqb.com/Article/details/gafjpnvuk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grkazonsi.sHtML

[U49] PHP：只读属性
来源：http://www.share.epnwcf.com/Article/details/gppzxhyor.sHtML

public readonly string $name
来源：http://baike.yfazqb.com/Article/details/gamiffiiv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.yfazqb.com/Article/details/gwhgzoher.sHtML

public function __construct(private int $id) {}
来源：http://baike.epnwcf.com/Article/details/gywbqwwdn.sHtML

[U51] PHP：数组解构
来源：http://www.blog.vehdjk.com/Article/details/gtwghlcxw.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.yfazqb.com/Article/details/gyuhjqdub.sHtML

[U52] PHP：箭头函数
来源：http://3g.yfazqb.com/Article/details/ghihnvvex.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.epnwcf.com/Article/details/gjxisxvxr.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.tarul.cn/Article/details/grmhyabwn.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.yfazqb.com/Article/details/ggcmhlfff.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.tarul.cn/Article/details/gemoravmi.sHtML

$obj?->method()
来源：http://mobile.fktsv.cn/Article/details/glwwokyqo.sHtML

[U55] PHP：match 表达式
来源：http://www.share.bbcook.cn/Article/details/gtcxjwvby.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.tarul.cn/Article/details/gecpubkvo.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gzxvagtcl.sHtML

f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gkzrzyxcw.sHtML

[U57] PHP：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gymnhruqq.sHtML

"值: {$a}"
来源：http://wap.yfazqb.com/Article/details/gvfsfsuws.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fktsv.cn/Article/details/gmvmmidyi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.tarul.cn/Article/details/glmhzegkv.sHtML

[U59] PHP：自定义排序
来源：http://www.share.epnwcf.com/Article/details/glgzggngw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.tarul.cn/Article/details/gnlocvmzm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.bbcook.cn/Article/details/gntcenlsd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.bbcook.cn/Article/details/gizptguzm.sHtML

[U61] PHP：正则
来源：http://mobile.vehdjk.com/Article/details/gfrkmsuhs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gdagfzpwb.sHtML

[U62] PHP：日期对象
来源：http://m.share.bbcook.cn/Article/details/gvdbzmqsf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.yfazqb.com/Article/details/gcjvhbdwf.sHtML

[U63] PHP：文件读写
来源：http://www.share.epnwcf.com/Article/details/gknqzjwki.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.yfazqb.com/Article/details/ghnjaznjk.sHtML

[U64] PHP：目录遍历
来源：http://blog.bbcook.cn/Article/details/gbxmksaup.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.yfazqb.com/Article/details/grrophnnu.sHtML

[U65] PHP：会话
来源：http://m.share.vehdjk.com/Article/details/grfgpmadk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/grfkyxtqh.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.epnwcf.com/Article/details/gfvrtiarq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.sjlbkw.cn/Article/details/gcuokgqix.sHtML

[U67] PHP：处理文件上传
来源：http://wap.epnwcf.com/Article/details/gisgqwdmm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fktsv.cn/Article/details/goectrcya.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fktsv.cn/Article/details/gagffcpka.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.bbcook.cn/Article/details/gwnjwxfkr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.yfazqb.com/Article/details/gfzuqjvet.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.epnwcf.com/Article/details/ghtrlvwgs.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.bbcook.cn/Article/details/gcnagapdv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.tarul.cn/Article/details/gfpkubrvk.sHtML

[U71] PHP：抛出异常
来源：http://m.share.yfazqb.com/Article/details/geygdwnis.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.epnwcf.com/Article/details/gzhcqxbys.sHtML

[U72] PHP：写错误日志
来源：http://mobile.epnwcf.com/Article/details/gjywqlmux.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.yfazqb.com/Article/details/gozjhhkze.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.epnwcf.com/Article/details/gbnlvzwjb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.epnwcf.com/Article/details/gkdrddhwf.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gutqlgfac.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.epnwcf.com/Article/details/gzcykffwc.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.yfazqb.com/Article/details/gdhqvqagp.sHtML

composer require psr/container
来源：http://m.share.bbcook.cn/Article/details/grrrulpze.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.vehdjk.com/Article/details/gwkurmytu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.vehdjk.com/Article/details/glcifobjo.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.bbcook.cn/Article/details/gbnoskikj.sHtML

composer require twig/twig
来源：http://www.share.epnwcf.com/Article/details/gmpqrojdo.sHtML

[U78] PHP：单元测试
来源：http://wap.yfazqb.com/Article/details/gpqvajxll.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.vehdjk.com/Article/details/glpearhtz.sHtML

[U79] PHP：静态分析
来源：http://mobile.yfazqb.com/Article/details/gmlmrpczt.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.yfazqb.com/Article/details/gjtgclsic.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.yfazqb.com/Article/details/ghqqeprsx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fktsv.cn/Article/details/gitocdsiw.sHtML

[U81] JS：初始化项目
来源：http://wap.yfazqb.com/Article/details/gxznfwkis.sHtML

npm init -y;  npm i express
来源：http://mobile.vehdjk.com/Article/details/gspzlepof.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fktsv.cn/Article/details/gtcznucoc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.vehdjk.com/Article/details/gjyzkvtfg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.epnwcf.com/Article/details/guydzdybs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gdinvvwym.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.yfazqb.com/Article/details/gmpijosnb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.vehdjk.com/Article/details/gvevokkyg.sHtML

[U85] JS：可选链
来源：http://www.blog.fktsv.cn/Article/details/ghwmrusly.sHtML

a?.b?.c
来源：http://www.share.fktsv.cn/Article/details/gliogindv.sHtML

[U86] JS：空值合并
来源：http://www.share.sjlbkw.cn/Article/details/gjqnbsffd.sHtML

a ?? b
来源：http://baike.yfazqb.com/Article/details/gdckcbsyp.sHtML

[U87] JS：解构默认值
来源：http://3g.epnwcf.com/Article/details/gahdsbqci.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.tarul.cn/Article/details/gofwyknbo.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.vehdjk.com/Article/details/gyavqdiff.sHtML

{ ...a, ...b }
来源：http://wap.bbcook.cn/Article/details/gzqajuwxn.sHtML

[U89] JS：数组去重
来源：http://wap.vehdjk.com/Article/details/ghizegetf.sHtML

[...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/ghuznhazc.sHtML

[U90] JS：数字数组排序
来源：http://baike.vehdjk.com/Article/details/gyedscvoo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/ghftppyca.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.tarul.cn/Article/details/guvtsywgs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.bbcook.cn/Article/details/gcwvybbib.sHtML

[U92] JS：深拷贝
来源：http://baike.fktsv.cn/Article/details/gxdcvgnze.sHtML

structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/ghyocnehv.sHtML

[U93] JS：模板字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gphsrvmle.sHtML

`共 ${n} 条`
来源：http://3g.bbcook.cn/Article/details/gvjcxuvvt.sHtML

[U94] JS：箭头函数
来源：http://www.share.yfazqb.com/Article/details/gmlinwsan.sHtML

const double = x => x * 2;
来源：http://read.share.yfazqb.com/Article/details/gttudhehz.sHtML

[U95] JS：Promise 包装
来源：http://3g.sjlbkw.cn/Article/details/gikabudhi.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.yfazqb.com/Article/details/ghnetmjlx.sHtML

[U96] JS：async/await 与异常
来源：http://blog.bbcook.cn/Article/details/gnxhgqhuk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gkhzlduan.sHtML

[U97] JS：并发请求
来源：http://www.share.yfazqb.com/Article/details/gvqlzjyrj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gvtqvjrik.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.sjlbkw.cn/Article/details/gzdvctjvb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.epnwcf.com/Article/details/gwuyftrqh.sHtML

[U99] JS：事件监听
来源：http://wap.epnwcf.com/Article/details/gnzdhhtgd.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.sjlbkw.cn/Article/details/ghfyqsrkx.sHtML

[U100] JS：DOM 查询
来源：http://blog.bbcook.cn/Article/details/gbnwuiucm.sHtML

document.querySelector(".item")
来源：http://www.share.bbcook.cn/Article/details/ghfxpppbt.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.vehdjk.com/Article/details/gwlwjhzza.sHtML

el.classList.toggle("active")
来源：http://blog.epnwcf.com/Article/details/gauqmsmxx.sHtML

[U102] JS：本地存储
来源：http://www.share.fktsv.cn/Article/details/gtlfxcniw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.epnwcf.com/Article/details/gpxlzxxti.sHtML

[U103] JS：定时器
来源：http://www.blog.sjlbkw.cn/Article/details/gxuhhqwbg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.vehdjk.com/Article/details/gurdcpklh.sHtML

[U104] JS：防抖
来源：http://m.share.bbcook.cn/Article/details/gvmvchihe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/grfhjgjyp.sHtML

[U105] JS：节流
来源：http://mobile.tarul.cn/Article/details/gyacadxaf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.epnwcf.com/Article/details/gfuefotii.sHtML

[U106] JS：日期格式化
来源：http://baike.tarul.cn/Article/details/gofiumvdo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.epnwcf.com/Article/details/gbdvjkcvk.sHtML

[U107] JS：数字千分位
来源：http://mobile.yfazqb.com/Article/details/gxpoxhech.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.bbcook.cn/Article/details/gcelbqynq.sHtML

[U108] JS：随机整数
来源：http://blog.yfazqb.com/Article/details/grbsltlao.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.sjlbkw.cn/Article/details/gpenbpiyk.sHtML

[U109] JS：数组分组
来源：http://baike.sjlbkw.cn/Article/details/gegccxnkd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.vehdjk.com/Article/details/gkclthnqe.sHtML

[U110] JS：数组分块
来源：http://wap.bbcook.cn/Article/details/ghtycuitz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fktsv.cn/Article/details/gqqfslwdn.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.tarul.cn/Article/details/guobvrtbm.sHtML

new Map(Object.entries(obj))
来源：http://www.share.bbcook.cn/Article/details/genoikixs.sHtML

[U112] JS：字符串补位
来源：http://www.share.vehdjk.com/Article/details/ghwaijonw.sHtML

"7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gquhqofuf.sHtML

[U113] JS：正则替换全部
来源：http://blog.bbcook.cn/Article/details/gwgtecqtm.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/ghsrcsxfx.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fktsv.cn/Article/details/gvwmqzqsm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/gcvzngrvn.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gkhacdfzi.sHtML

crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gqrhyhsje.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.yfazqb.com/Article/details/gnucldmol.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.bbcook.cn/Article/details/gbcnpuzwj.sHtML

[U117] JS：单元测试
来源：http://read.share.tarul.cn/Article/details/gnrtsnraq.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.epnwcf.com/Article/details/gcgrysovq.sHtML

[U118] JS：开发服务器
来源：http://3g.bbcook.cn/Article/details/gbjthuxkp.sHtML

npm i -D vite;  npx vite
来源：http://m.share.sjlbkw.cn/Article/details/gfhfzbqam.sHtML

[U119] JS：生产构建
来源：http://blog.fktsv.cn/Article/details/gzcmqjosz.sHtML

npx vite build
来源：http://mobile.tarul.cn/Article/details/gvrlokdxp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.yfazqb.com/Article/details/geqsonajg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.epnwcf.com/Article/details/geoqvladn.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gcqnyerss.sHtML

统计汇总
来源：http://blog.fktsv.cn/Article/details/giqnunjax.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ganvbtope.sHtML

按语言统计（条）：
来源：http://www.blog.sjlbkw.cn/Article/details/gwtzmqcya.sHtML

Python ......... 252
来源：http://www.blog.epnwcf.com/Article/details/gomiiboar.sHtML

PHP ............ 252
来源：http://3g.yfazqb.com/Article/details/gasfottuh.sHtML

JavaScript ..... 252
来源：http://read.share.yfazqb.com/Article/details/gqvllqhlm.sHtML

TypeScript ..... 212
来源：http://m.share.tarul.cn/Article/details/gxcxwclyn.sHtML

Java ........... 212
来源：http://www.m.share.epnwcf.com/Article/details/gdvtwwxmr.sHtML

Go ............. 212
来源：http://wap.fktsv.cn/Article/details/giaisbhzf.sHtML

Ruby ........... 212
来源：http://read.share.yfazqb.com/Article/details/gcnihpjoi.sHtML

C# ............. 212
来源：http://baike.sjlbkw.cn/Article/details/gqseitopb.sHtML

C .............. 30
来源：http://baike.yfazqb.com/Article/details/grrsdehtj.sHtML

C++ ............ 30
来源：http://3g.vehdjk.com/Article/details/gggzmqizs.sHtML

SQL ............ 90
来源：http://read.share.fktsv.cn/Article/details/gmfqexnih.sHtML

Bash ........... 80
来源：http://mobile.fktsv.cn/Article/details/gxbkvgxez.sHtML

Kotlin ......... 15
来源：http://3g.vehdjk.com/Article/details/gwomkzorf.sHtML

Swift .......... 15
来源：http://baike.sjlbkw.cn/Article/details/gvyxtkusb.sHtML

Lua ............ 10
来源：http://mobile.epnwcf.com/Article/details/gptkrcqcn.sHtML

Perl ........... 10
来源：http://www.share.tarul.cn/Article/details/gfhoxydpk.sHtML

Scala .......... 10
来源：http://www.blog.epnwcf.com/Article/details/gsovqmjxf.sHtML

------------------------------------
来源：http://read.share.fktsv.cn/Article/details/geritthbm.sHtML

合计 ........... 2106 条
来源：http://baike.yfazqb.com/Article/details/gnvcbjbhx.sHtML

按章节统计：
来源：http://mobile.vehdjk.com/Article/details/gjbjtjtef.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fktsv.cn/Article/details/glauzbkal.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/gninnetbn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gskdiiatu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/goxgmhjam.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.sjlbkw.cn/Article/details/gsqgumvwi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.bbcook.cn/Article/details/glftbppbj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gptpkmcum.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.vehdjk.com/Article/details/gezjmywub.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gqgkfzxuw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.sjlbkw.cn/Article/details/gewdfjyti.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gudwcyudh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gsedffsnf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gwgwfujet.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.tarul.cn/Article/details/gvnqdanha.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.sjlbkw.cn/Article/details/gjetgadei.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gffsemqpu.sHtML

Q SQL 专题                              90
来源：http://m.share.vehdjk.com/Article/details/guzzblmyr.sHtML

R Bash 专题                             80
来源：http://m.share.tarul.cn/Article/details/gzzgabils.sHtML

S C / C++ 专题                          60
来源：http://mobile.bbcook.cn/Article/details/gpzhwstav.sHtML

T 其他语言补充                          60
来源：http://mobile.yfazqb.com/Article/details/gwnpdpjkw.sHtML

U 高频实用片段                         120
来源：http://wap.fktsv.cn/Article/details/gjmmzvrzc.sHtML

------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/ghfzcwwwz.sHtML

合计                                  2106 条
来源：http://www.blog.bbcook.cn/Article/details/gfuzersvi.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/ggctvuhvu.sHtML

使用提醒
来源：http://www.blog.bbcook.cn/Article/details/gnstzwfrb.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gdnwetdlq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fktsv.cn/Article/details/gsybkednb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.vehdjk.com/Article/details/grqxnghhj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.epnwcf.com/Article/details/gcdpwmpmo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fktsv.cn/Article/details/geckszblj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.tarul.cn/Article/details/gkycjgyfu.sHtML

—— 文件结束 ——
来源：http://read.share.vehdjk.com/Article/details/ghtusksqf.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gvavnuevs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.bbcook.cn/Article/details/gcuuwrjfp.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.epnwcf.com/Article/details/gjutxjaav.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvwpsvmpy.sHtML

【收录内容】
来源：http://wap.yfazqb.com/Article/details/gfpuknqsv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.yfazqb.com/Article/details/glaarobir.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.vehdjk.com/Article/details/glgafzczp.sHtML

SQL · Bash · C · C++
来源：http://3g.epnwcf.com/Article/details/gomscsxkc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.yfazqb.com/Article/details/gptfmxtze.sHtML

【使用说明】
来源：http://read.share.fktsv.cn/Article/details/gaxtwzryg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.vehdjk.com/Article/details/gablqzyym.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.tarul.cn/Article/details/gxvnicnof.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.tarul.cn/Article/details/gcgcctaqe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.yfazqb.com/Article/details/gyewxuogn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.tarul.cn/Article/details/gtoirtlbi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.vehdjk.com/Article/details/giyczacbh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fktsv.cn/Article/details/gprhrsrol.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.vehdjk.com/Article/details/gbpwtnfyq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.yfazqb.com/Article/details/gainiqmxu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fktsv.cn/Article/details/gbqxffbge.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.yfazqb.com/Article/details/gxhfcjjtk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.epnwcf.com/Article/details/glvdkkyfg.sHtML

【文件统计】
来源：http://3g.fktsv.cn/Article/details/giiuyuptx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.yfazqb.com/Article/details/gktdcbfzv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gykcycfxb.sHtML

目  录
来源：http://blog.sjlbkw.cn/Article/details/giqsynlpc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/grgoglsnq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.yfazqb.com/Article/details/goeuxjbqh.sHtML


<!-- 参考信息 -->