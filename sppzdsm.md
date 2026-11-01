代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fktsv.cn/Article/details/gxxifgdni.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gexntozdg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/gjvocjezq.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/grnbuxxzm.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fktsv.cn/Article/details/gzkbbsavk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.sjlbkw.cn/Article/details/glznpwofl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fktsv.cn/Article/details/gvivsvgzg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.bbcook.cn/Article/details/gbzghvnza.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.epnwcf.com/Article/details/gvozuyfug.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.tarul.cn/Article/details/gqowgwobw.sHtML

[U04] Py：变量调试打印
来源：http://m.share.yfazqb.com/Article/details/gmuyiowrb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.yfazqb.com/Article/details/gtqxnrizt.sHtML

[U05] Py：列表去重且保序
来源：http://3g.epnwcf.com/Article/details/gkqfybamc.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gteaqmeav.sHtML

[U06] Py：合并两个字典
来源：http://read.share.vehdjk.com/Article/details/grdjddgwb.sHtML

{**a, **b}
来源：http://blog.tarul.cn/Article/details/gntfmruoe.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fktsv.cn/Article/details/giycgkqao.sHtML

{v: k for k, v in d.items()}
来源：http://baike.tarul.cn/Article/details/ggzgbmrmf.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fktsv.cn/Article/details/gtekasvzj.sHtML

[y for x in nested for y in x]
来源：http://baike.epnwcf.com/Article/details/gudyckowa.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.epnwcf.com/Article/details/gbzmsagdd.sHtML

max(d, key=d.get)
来源：http://mobile.epnwcf.com/Article/details/gplejdxul.sHtML

[U10] Py：按值排序字典
来源：http://3g.yfazqb.com/Article/details/gaminwjcl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.sjlbkw.cn/Article/details/gyiozgaam.sHtML

[U11] Py：生成器表达式
来源：http://wap.bbcook.cn/Article/details/gkgcnhpov.sHtML

(x * 2 for x in arr)
来源：http://m.share.vehdjk.com/Article/details/gcgfwfgxp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/gfklxgkfm.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fktsv.cn/Article/details/gpccydnzc.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fktsv.cn/Article/details/gxhksfbdx.sHtML

deque(maxlen=10)
来源：http://www.share.bbcook.cn/Article/details/gozbjmxmr.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.epnwcf.com/Article/details/gltblswnd.sHtML

defaultdict(list)
来源：http://www.blog.vehdjk.com/Article/details/gcemcryiz.sHtML

[U15] Py：高精度计时
来源：http://blog.sjlbkw.cn/Article/details/ghhcommol.sHtML

t = time.perf_counter()
来源：http://blog.bbcook.cn/Article/details/glnhsocii.sHtML

[U16] Py：命令行参数解析
来源：http://3g.tarul.cn/Article/details/gdrrzttle.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.epnwcf.com/Article/details/gacpxorko.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fktsv.cn/Article/details/goacllblq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.vehdjk.com/Article/details/ghaxiogtz.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.epnwcf.com/Article/details/gbuhtezmt.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.tarul.cn/Article/details/gweamqbkd.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.vehdjk.com/Article/details/gbqqcoivk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.bbcook.cn/Article/details/goqdicymj.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fktsv.cn/Article/details/gdrigroeg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.bbcook.cn/Article/details/gnfjillfy.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.epnwcf.com/Article/details/gwwzcykij.sHtML

@contextlib.contextmanager
来源：http://www.m.share.yfazqb.com/Article/details/gsiycaypw.sHtML

[U22] Py：矩阵转置
来源：http://m.share.yfazqb.com/Article/details/gnnpvrxhm.sHtML

list(zip(*m))
来源：http://mobile.fktsv.cn/Article/details/glngalusa.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fktsv.cn/Article/details/grdlovfjd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.tarul.cn/Article/details/garidiuhk.sHtML

[U24] Py：路径操作
来源：http://www.m.share.vehdjk.com/Article/details/grfxmwpcu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gopexpend.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.epnwcf.com/Article/details/gdizmlaho.sHtML

csv.DictReader(f)
来源：http://baike.tarul.cn/Article/details/grtfndszx.sHtML

[U26] Py：并发下载
来源：http://www.share.epnwcf.com/Article/details/gqvhejhwr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.sjlbkw.cn/Article/details/gqtewmopu.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fktsv.cn/Article/details/gbvszyeoe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.bbcook.cn/Article/details/glxuxvdbl.sHtML

[U28] Py：类型别名
来源：http://m.share.sjlbkw.cn/Article/details/glkfvrldb.sHtML

UserId = int
来源：http://read.share.epnwcf.com/Article/details/gbhhgpibg.sHtML

[U29] Py：属性校验
来源：http://mobile.fktsv.cn/Article/details/gbsizpytb.sHtML

@property 与 @x.setter 配合
来源：http://wap.yfazqb.com/Article/details/gcoxpwneq.sHtML

[U30] Py：数据类
来源：http://wap.fktsv.cn/Article/details/grmemeguj.sHtML

@dataclass(slots=True)
来源：http://www.m.share.epnwcf.com/Article/details/gzjmtogzm.sHtML

[U31] Py：单测
来源：http://www.share.sjlbkw.cn/Article/details/gghcylhsz.sHtML

python -m pytest -q
来源：http://baike.epnwcf.com/Article/details/gygkrcbhs.sHtML

[U32] Py：代码格式化
来源：http://wap.vehdjk.com/Article/details/grxzghwzz.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.tarul.cn/Article/details/gtsxchoah.sHtML

[U33] Py：打包发布
来源：http://read.share.vehdjk.com/Article/details/ggttfrntw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.yfazqb.com/Article/details/ggcuufalb.sHtML

[U34] Py：判断编码
来源：http://3g.vehdjk.com/Article/details/giwsnawby.sHtML

chardet.detect(raw)
来源：http://www.share.tarul.cn/Article/details/gvrthnuue.sHtML

[U35] Py：发送邮件
来源：http://www.blog.epnwcf.com/Article/details/ghinwfshu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fktsv.cn/Article/details/gzegrsudm.sHtML

[U36] Py：定时任务
来源：http://baike.tarul.cn/Article/details/gkrrofeoc.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.tarul.cn/Article/details/gntleprmy.sHtML

[U37] Py：读写 Excel
来源：http://wap.fktsv.cn/Article/details/gbdlujpvm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.sjlbkw.cn/Article/details/ghylppsth.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.yfazqb.com/Article/details/gvapdcoct.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.vehdjk.com/Article/details/grlammdzw.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.bbcook.cn/Article/details/gsrukithp.sHtML

sys.stdout.isatty()
来源：http://3g.epnwcf.com/Article/details/gsmdrwiil.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.epnwcf.com/Article/details/gubtryxwd.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gqobtyllo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.bbcook.cn/Article/details/gmlubzhig.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.vehdjk.com/Article/details/gywaoelmb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.vehdjk.com/Article/details/gyindkcze.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fktsv.cn/Article/details/gsbuspyqk.sHtML

[U43] PHP：声明命名空间
来源：http://3g.epnwcf.com/Article/details/giwecceij.sHtML

namespace App\Http;
来源：http://wap.fktsv.cn/Article/details/gtgbiwvdh.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.sjlbkw.cn/Article/details/giqjarwhr.sHtML

declare(strict_types=1);
来源：http://www.share.fktsv.cn/Article/details/gcicfytic.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.sjlbkw.cn/Article/details/gvqcuvowk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gcozazshe.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.tarul.cn/Article/details/gxlzmjnwl.sHtML

?string $name = null
来源：http://wap.sjlbkw.cn/Article/details/gnmxrjmhr.sHtML

[U47] PHP：联合类型
来源：http://www.blog.vehdjk.com/Article/details/gpztmywab.sHtML

int|string $id
来源：http://www.blog.fktsv.cn/Article/details/gcjnqetqp.sHtML

[U48] PHP：纯枚举
来源：http://mobile.vehdjk.com/Article/details/gijqtncya.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.epnwcf.com/Article/details/gdnmwyonj.sHtML

[U49] PHP：只读属性
来源：http://baike.fktsv.cn/Article/details/glbdehjmu.sHtML

public readonly string $name
来源：http://baike.sjlbkw.cn/Article/details/ghlbxqdgn.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.epnwcf.com/Article/details/gteczvhvx.sHtML

public function __construct(private int $id) {}
来源：http://www.share.sjlbkw.cn/Article/details/gqhpygqyt.sHtML

[U51] PHP：数组解构
来源：http://www.blog.vehdjk.com/Article/details/gdvapnfxe.sHtML

[$a, $b] = $arr;
来源：http://www.blog.sjlbkw.cn/Article/details/gkrxspxlv.sHtML

[U52] PHP：箭头函数
来源：http://m.share.bbcook.cn/Article/details/gcxuvtpft.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.tarul.cn/Article/details/gfcmzaqqi.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.bbcook.cn/Article/details/gcvngieme.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fktsv.cn/Article/details/gxjvuhvny.sHtML

[U54] PHP：空安全调用
来源：http://m.share.tarul.cn/Article/details/gkghkvehv.sHtML

$obj?->method()
来源：http://wap.fktsv.cn/Article/details/gszycphfn.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gigwyspvx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fktsv.cn/Article/details/gkfhkqxpo.sHtML

[U56] PHP：命名参数
来源：http://read.share.bbcook.cn/Article/details/gtsbddren.sHtML

f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gdiwzjmxe.sHtML

[U57] PHP：字符串插值
来源：http://read.share.bbcook.cn/Article/details/goajmxlfz.sHtML

"值: {$a}"
来源：http://baike.bbcook.cn/Article/details/gshlnjyoq.sHtML

[U58] PHP：数组三件套
来源：http://blog.sjlbkw.cn/Article/details/gyxeidtmu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.tarul.cn/Article/details/gffnemnsr.sHtML

[U59] PHP：自定义排序
来源：http://mobile.yfazqb.com/Article/details/giugwzblv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gudvvpjuv.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.sjlbkw.cn/Article/details/gekddkhpn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fktsv.cn/Article/details/gejsvwrkj.sHtML

[U61] PHP：正则
来源：http://www.blog.vehdjk.com/Article/details/gyxmflmms.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/gbvsrerii.sHtML

[U62] PHP：日期对象
来源：http://read.share.yfazqb.com/Article/details/gbqvwljbq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.tarul.cn/Article/details/gdmyyxmoc.sHtML

[U63] PHP：文件读写
来源：http://baike.fktsv.cn/Article/details/gtbccbwld.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.bbcook.cn/Article/details/gtbttdwsq.sHtML

[U64] PHP：目录遍历
来源：http://www.share.vehdjk.com/Article/details/ggltpbmgv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.sjlbkw.cn/Article/details/giyfftsgl.sHtML

[U65] PHP：会话
来源：http://3g.sjlbkw.cn/Article/details/gdavglslx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.tarul.cn/Article/details/ggjumcdab.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.yfazqb.com/Article/details/gbzceckju.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.tarul.cn/Article/details/gauunbxzk.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.sjlbkw.cn/Article/details/gxqgvpjzm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.yfazqb.com/Article/details/gkhgmhjee.sHtML

[U68] PHP：PDO 连接
来源：http://blog.tarul.cn/Article/details/gfyethhcz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.vehdjk.com/Article/details/gscocipfg.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fktsv.cn/Article/details/gbqmvcmef.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.epnwcf.com/Article/details/gmvmzrmfp.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.bbcook.cn/Article/details/gtkebvodl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.vehdjk.com/Article/details/gybdikgam.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gewqvwoeh.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.epnwcf.com/Article/details/gbqqikplb.sHtML

[U72] PHP：写错误日志
来源：http://read.share.bbcook.cn/Article/details/gpkgrmasg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.bbcook.cn/Article/details/govtutwqw.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.yfazqb.com/Article/details/glunumjbk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.yfazqb.com/Article/details/gcajukkea.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.epnwcf.com/Article/details/gixlanrdf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fktsv.cn/Article/details/gtbphjior.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fktsv.cn/Article/details/gjnsgdftp.sHtML

composer require psr/container
来源：http://www.m.share.yfazqb.com/Article/details/girdriwql.sHtML

[U76] PHP：简单路由
来源：http://read.share.bbcook.cn/Article/details/gldfqrvks.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.yfazqb.com/Article/details/gytshnzvv.sHtML

[U77] PHP：模板渲染
来源：http://www.share.epnwcf.com/Article/details/gdlneenqe.sHtML

composer require twig/twig
来源：http://www.blog.vehdjk.com/Article/details/gbcobuhxa.sHtML

[U78] PHP：单元测试
来源：http://www.share.sjlbkw.cn/Article/details/gndtuncvy.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.vehdjk.com/Article/details/gjtvxokcs.sHtML

[U79] PHP：静态分析
来源：http://read.share.fktsv.cn/Article/details/gmteqeaow.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.yfazqb.com/Article/details/gelrmrudy.sHtML

[U80] PHP：代码规范修复
来源：http://wap.bbcook.cn/Article/details/gcpsqdbap.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.vehdjk.com/Article/details/ggdodyumi.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.epnwcf.com/Article/details/glqynydpz.sHtML

npm init -y;  npm i express
来源：http://read.share.vehdjk.com/Article/details/giamnbtxt.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fktsv.cn/Article/details/gsuqoydss.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.bbcook.cn/Article/details/gduntdapa.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.epnwcf.com/Article/details/gvapgaebp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.tarul.cn/Article/details/gunsevxcc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.tarul.cn/Article/details/gucphjpdi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.epnwcf.com/Article/details/gsnpugujo.sHtML

[U85] JS：可选链
来源：http://blog.sjlbkw.cn/Article/details/goqbtrkqg.sHtML

a?.b?.c
来源：http://www.share.tarul.cn/Article/details/gyygbbfra.sHtML

[U86] JS：空值合并
来源：http://blog.epnwcf.com/Article/details/gdizkplps.sHtML

a ?? b
来源：http://read.share.bbcook.cn/Article/details/goicgiwtc.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.epnwcf.com/Article/details/gtbjczolu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.bbcook.cn/Article/details/ghaazijde.sHtML

[U88] JS：对象展开合并
来源：http://3g.epnwcf.com/Article/details/gnhypaenb.sHtML

{ ...a, ...b }
来源：http://www.blog.yfazqb.com/Article/details/gzjzizjgv.sHtML

[U89] JS：数组去重
来源：http://baike.vehdjk.com/Article/details/gwaruleep.sHtML

[...new Set(arr)]
来源：http://blog.yfazqb.com/Article/details/gmqfmmmep.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.yfazqb.com/Article/details/gpfvpcujf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gufyaiijy.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.tarul.cn/Article/details/gwvkbpvrx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.tarul.cn/Article/details/gwltczgix.sHtML

[U92] JS：深拷贝
来源：http://www.share.bbcook.cn/Article/details/gwgbwbdpz.sHtML

structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gufnwzgzx.sHtML

[U93] JS：模板字符串
来源：http://www.blog.tarul.cn/Article/details/gixwjhgiw.sHtML

`共 ${n} 条`
来源：http://mobile.tarul.cn/Article/details/gizkxfwrm.sHtML

[U94] JS：箭头函数
来源：http://read.share.epnwcf.com/Article/details/gvceiyedt.sHtML

const double = x => x * 2;
来源：http://wap.yfazqb.com/Article/details/gtvnaainb.sHtML

[U95] JS：Promise 包装
来源：http://baike.vehdjk.com/Article/details/gcbdwwbqb.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.epnwcf.com/Article/details/gtvgjkooc.sHtML

[U96] JS：async/await 与异常
来源：http://blog.epnwcf.com/Article/details/gedrofene.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/goqqqwstt.sHtML

[U97] JS：并发请求
来源：http://m.share.fktsv.cn/Article/details/gpgojkpqs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gpahuubwb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxqfdwkk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.yfazqb.com/Article/details/gxfxfayyj.sHtML

[U99] JS：事件监听
来源：http://m.share.vehdjk.com/Article/details/gslhgtugm.sHtML

el.addEventListener("click", e => {})
来源：http://blog.sjlbkw.cn/Article/details/gntiehbti.sHtML

[U100] JS：DOM 查询
来源：http://wap.bbcook.cn/Article/details/glxowsezv.sHtML

document.querySelector(".item")
来源：http://3g.yfazqb.com/Article/details/gbgeqagyg.sHtML

[U101] JS：classList 操作
来源：http://wap.sjlbkw.cn/Article/details/grugdbvcu.sHtML

el.classList.toggle("active")
来源：http://wap.bbcook.cn/Article/details/ggbbkqmew.sHtML

[U102] JS：本地存储
来源：http://www.blog.bbcook.cn/Article/details/grhjrszdq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.epnwcf.com/Article/details/gbykprnis.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/gyatnrnoy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fktsv.cn/Article/details/gkgoxpphm.sHtML

[U104] JS：防抖
来源：http://www.share.fktsv.cn/Article/details/gmsdedxos.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gydctbfub.sHtML

[U105] JS：节流
来源：http://wap.vehdjk.com/Article/details/gwyystppk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.bbcook.cn/Article/details/gexugffho.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gsudmfvzt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.vehdjk.com/Article/details/gllycyrbq.sHtML

[U107] JS：数字千分位
来源：http://www.share.bbcook.cn/Article/details/gpoqtfinw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gsytzjzzc.sHtML

[U108] JS：随机整数
来源：http://www.share.sjlbkw.cn/Article/details/gehfibkdm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.sjlbkw.cn/Article/details/ghqymqzuf.sHtML

[U109] JS：数组分组
来源：http://blog.fktsv.cn/Article/details/gfkqigyka.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fktsv.cn/Article/details/gnsstdzit.sHtML

[U110] JS：数组分块
来源：http://www.share.epnwcf.com/Article/details/gfeldwgtr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.yfazqb.com/Article/details/gsdyqnign.sHtML

[U111] JS：对象转 Map
来源：http://3g.bbcook.cn/Article/details/gkijuwrvz.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.tarul.cn/Article/details/gxqbeebuv.sHtML

[U112] JS：字符串补位
来源：http://wap.bbcook.cn/Article/details/gitjgzvab.sHtML

"7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gljdqrpuo.sHtML

[U113] JS：正则替换全部
来源：http://blog.yfazqb.com/Article/details/gwrxmwxtp.sHtML

s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gavhxuotk.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.yfazqb.com/Article/details/gcjqkhfzv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gumatcpzv.sHtML

[U115] JS：生成 UUID
来源：http://mobile.tarul.cn/Article/details/gxryxkztt.sHtML

crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gwbnhbann.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.bbcook.cn/Article/details/gbrefxepd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.bbcook.cn/Article/details/grgjltlcw.sHtML

[U117] JS：单元测试
来源：http://www.m.share.yfazqb.com/Article/details/gjpvkixcq.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.yfazqb.com/Article/details/gxuplknul.sHtML

[U118] JS：开发服务器
来源：http://baike.fktsv.cn/Article/details/giwmsuamo.sHtML

npm i -D vite;  npx vite
来源：http://mobile.sjlbkw.cn/Article/details/gjxzfszhz.sHtML

[U119] JS：生产构建
来源：http://3g.vehdjk.com/Article/details/gzxngcvdy.sHtML

npx vite build
来源：http://wap.yfazqb.com/Article/details/gqsvmzowx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.epnwcf.com/Article/details/grsugpahx.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.tarul.cn/Article/details/gjhfiblgf.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/giplsmcdu.sHtML

统计汇总
来源：http://www.share.tarul.cn/Article/details/gktrqgdfg.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbbhkuize.sHtML

按语言统计（条）：
来源：http://www.share.epnwcf.com/Article/details/gohizwwqd.sHtML

Python ......... 252
来源：http://www.m.share.sjlbkw.cn/Article/details/glgwdqnmw.sHtML

PHP ............ 252
来源：http://www.blog.yfazqb.com/Article/details/gnakshyhl.sHtML

JavaScript ..... 252
来源：http://mobile.epnwcf.com/Article/details/ghasbfqaa.sHtML

TypeScript ..... 212
来源：http://www.blog.sjlbkw.cn/Article/details/gitsedauw.sHtML

Java ........... 212
来源：http://wap.yfazqb.com/Article/details/gitjkmysb.sHtML

Go ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gemkvuueo.sHtML

Ruby ........... 212
来源：http://read.share.bbcook.cn/Article/details/gdxklitqs.sHtML

C# ............. 212
来源：http://wap.sjlbkw.cn/Article/details/gtdrdacvx.sHtML

C .............. 30
来源：http://baike.epnwcf.com/Article/details/gcbfrnnkd.sHtML

C++ ............ 30
来源：http://3g.vehdjk.com/Article/details/gvpakpbny.sHtML

SQL ............ 90
来源：http://read.share.sjlbkw.cn/Article/details/gngbpcizl.sHtML

Bash ........... 80
来源：http://wap.yfazqb.com/Article/details/gxziuoiqt.sHtML

Kotlin ......... 15
来源：http://wap.sjlbkw.cn/Article/details/gnddtpczs.sHtML

Swift .......... 15
来源：http://www.blog.yfazqb.com/Article/details/gkzzxkibn.sHtML

Lua ............ 10
来源：http://wap.sjlbkw.cn/Article/details/gmqdvhsdc.sHtML

Perl ........... 10
来源：http://baike.bbcook.cn/Article/details/gvmhtqnxd.sHtML

Scala .......... 10
来源：http://www.share.epnwcf.com/Article/details/gxkivimke.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/goaherzrw.sHtML

合计 ........... 2106 条
来源：http://blog.tarul.cn/Article/details/ggpdljnrt.sHtML

按章节统计：
来源：http://www.m.share.fktsv.cn/Article/details/gjfbjvngj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/goikxwcmo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/gsvrgfkai.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gqtwqkzfq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/gfjasipap.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.sjlbkw.cn/Article/details/grzxmflan.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.epnwcf.com/Article/details/gibigrphx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gvghuyfww.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.bbcook.cn/Article/details/gvvklqbtr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gdmgwyfva.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.yfazqb.com/Article/details/gjpuhvffr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gxlhlkzmb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gsliefbrn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gintxdpzs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/gvrutsgvu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.epnwcf.com/Article/details/ghrejilqv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gbqoopeqp.sHtML

Q SQL 专题                              90
来源：http://3g.sjlbkw.cn/Article/details/goxrhkeym.sHtML

R Bash 专题                             80
来源：http://3g.sjlbkw.cn/Article/details/gdhkyqpud.sHtML

S C / C++ 专题                          60
来源：http://wap.sjlbkw.cn/Article/details/gnbyhvrwr.sHtML

T 其他语言补充                          60
来源：http://baike.fktsv.cn/Article/details/gksiornyd.sHtML

U 高频实用片段                         120
来源：http://www.share.vehdjk.com/Article/details/ggoyrxsnl.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gbovtuvgc.sHtML

合计                                  2106 条
来源：http://wap.vehdjk.com/Article/details/gzunvrhpg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/ggzwjyxih.sHtML

使用提醒
来源：http://www.share.sjlbkw.cn/Article/details/gmftvkmcr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gxugvylht.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.epnwcf.com/Article/details/gestkhvjt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.vehdjk.com/Article/details/ghbitzisd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.bbcook.cn/Article/details/gvdtimmdo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.tarul.cn/Article/details/gbehhbrkm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.yfazqb.com/Article/details/gxuizgdma.sHtML

—— 文件结束 ——
来源：http://3g.sjlbkw.cn/Article/details/gqtgbdddq.sHtML


<!-- 参考信息 -->