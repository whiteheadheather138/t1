代发 wailian999

[U01] Py：创建虚拟环境
来源：http://baike.fktsv.cn/Article/details/gorkyewui.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.tarul.cn/Article/details/gfzibpcei.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.vehdjk.com/Article/details/gydlrvhpf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.bbcook.cn/Article/details/grczamqxb.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.bbcook.cn/Article/details/gnbwwavaz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.vehdjk.com/Article/details/gycymlmwz.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fktsv.cn/Article/details/gedqggfyy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.yfazqb.com/Article/details/geyzxddsk.sHtML

[U05] Py：列表去重且保序
来源：http://3g.bbcook.cn/Article/details/gwfsbrijn.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/gkmmhkdil.sHtML

[U06] Py：合并两个字典
来源：http://mobile.epnwcf.com/Article/details/gtunogypr.sHtML

{**a, **b}
来源：http://3g.epnwcf.com/Article/details/gwfksrmpl.sHtML

[U07] Py：反转字典键值
来源：http://m.share.vehdjk.com/Article/details/gynmsodzf.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.sjlbkw.cn/Article/details/gfubhdqpr.sHtML

[U08] Py：展平二维列表
来源：http://mobile.epnwcf.com/Article/details/gschfbekp.sHtML

[y for x in nested for y in x]
来源：http://blog.sjlbkw.cn/Article/details/gffyegtal.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fktsv.cn/Article/details/gwdjhqiul.sHtML

max(d, key=d.get)
来源：http://m.share.bbcook.cn/Article/details/gxihenqvb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fktsv.cn/Article/details/gmmylkkbj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.epnwcf.com/Article/details/gdidrrdnx.sHtML

[U11] Py：生成器表达式
来源：http://blog.yfazqb.com/Article/details/glzwuxlmp.sHtML

(x * 2 for x in arr)
来源：http://mobile.epnwcf.com/Article/details/gslcxypsm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.yfazqb.com/Article/details/gpmrwgyyl.sHtML

Counter(arr).most_common(3)
来源：http://3g.sjlbkw.cn/Article/details/gclqfryuo.sHtML

[U13] Py：固定长度队列
来源：http://wap.tarul.cn/Article/details/ggwbdforc.sHtML

deque(maxlen=10)
来源：http://read.share.sjlbkw.cn/Article/details/gpvkybhmg.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.vehdjk.com/Article/details/glthtcgjs.sHtML

defaultdict(list)
来源：http://m.share.epnwcf.com/Article/details/gvpktpctn.sHtML

[U15] Py：高精度计时
来源：http://www.blog.vehdjk.com/Article/details/gtjqgqtox.sHtML

t = time.perf_counter()
来源：http://baike.yfazqb.com/Article/details/gaqnyosvd.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.yfazqb.com/Article/details/gfdyjztla.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.yfazqb.com/Article/details/gfaysmqkn.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gdejcqrpc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fktsv.cn/Article/details/gloiizczl.sHtML

[U18] Py：预编译正则
来源：http://baike.bbcook.cn/Article/details/gyervqmok.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fktsv.cn/Article/details/gftynmjrl.sHtML

[U19] Py：正则替换带回调
来源：http://wap.vehdjk.com/Article/details/gxbiakalm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.sjlbkw.cn/Article/details/gxvbyhtyo.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.epnwcf.com/Article/details/gmtgffbcs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.tarul.cn/Article/details/gnnomzvqw.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fktsv.cn/Article/details/gghxigibs.sHtML

@contextlib.contextmanager
来源：http://mobile.sjlbkw.cn/Article/details/gsbtvbpcf.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fktsv.cn/Article/details/gaxyokuxk.sHtML

list(zip(*m))
来源：http://wap.fktsv.cn/Article/details/gmyaixeow.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.yfazqb.com/Article/details/gdcvehcee.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.vehdjk.com/Article/details/gyyjnutoa.sHtML

[U24] Py：路径操作
来源：http://m.share.tarul.cn/Article/details/gvfqbunxq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.yfazqb.com/Article/details/gctyloxkg.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fktsv.cn/Article/details/gfbhwkmnz.sHtML

csv.DictReader(f)
来源：http://mobile.sjlbkw.cn/Article/details/gyzwawupw.sHtML

[U26] Py：并发下载
来源：http://wap.yfazqb.com/Article/details/gjelwoilo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fktsv.cn/Article/details/gfexjkeos.sHtML

[U27] Py：异步 HTTP
来源：http://baike.bbcook.cn/Article/details/gyaauxmbt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fktsv.cn/Article/details/gbmhuwmga.sHtML

[U28] Py：类型别名
来源：http://mobile.tarul.cn/Article/details/glfmpqkuz.sHtML

UserId = int
来源：http://www.blog.vehdjk.com/Article/details/glmkmrcfr.sHtML

[U29] Py：属性校验
来源：http://blog.vehdjk.com/Article/details/guhutssul.sHtML

@property 与 @x.setter 配合
来源：http://www.share.sjlbkw.cn/Article/details/gwloewlgw.sHtML

[U30] Py：数据类
来源：http://m.share.tarul.cn/Article/details/gylfdoaqx.sHtML

@dataclass(slots=True)
来源：http://wap.epnwcf.com/Article/details/ghqbslihu.sHtML

[U31] Py：单测
来源：http://www.share.bbcook.cn/Article/details/gltilfgkx.sHtML

python -m pytest -q
来源：http://blog.sjlbkw.cn/Article/details/gmztwirmh.sHtML

[U32] Py：代码格式化
来源：http://wap.fktsv.cn/Article/details/grcqfoczb.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.vehdjk.com/Article/details/gdrcmixnh.sHtML

[U33] Py：打包发布
来源：http://www.blog.sjlbkw.cn/Article/details/gmnxnsutv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.sjlbkw.cn/Article/details/gygkhgorn.sHtML

[U34] Py：判断编码
来源：http://mobile.vehdjk.com/Article/details/gjysrqgnr.sHtML

chardet.detect(raw)
来源：http://wap.sjlbkw.cn/Article/details/ggfjhlrql.sHtML

[U35] Py：发送邮件
来源：http://mobile.tarul.cn/Article/details/gydbhgetd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.tarul.cn/Article/details/gfodqfdlb.sHtML

[U36] Py：定时任务
来源：http://www.blog.epnwcf.com/Article/details/gzembyyfy.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.epnwcf.com/Article/details/gtlmedcng.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.tarul.cn/Article/details/giyodgqzz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.bbcook.cn/Article/details/ggtzrkrju.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.epnwcf.com/Article/details/gtlhyopsm.sHtML

Path(__file__).resolve().parent
来源：http://read.share.epnwcf.com/Article/details/ghxlrodxs.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.vehdjk.com/Article/details/glqwjeanm.sHtML

sys.stdout.isatty()
来源：http://www.share.sjlbkw.cn/Article/details/gbrmohcor.sHtML

[U40] Py：打印到标准错误
来源：http://baike.bbcook.cn/Article/details/gibrwyeph.sHtML

print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/gymutkfkv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.yfazqb.com/Article/details/gprcdxaqp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.epnwcf.com/Article/details/gnlewagsv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.sjlbkw.cn/Article/details/gqvwfqfzp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.tarul.cn/Article/details/gtauiexvh.sHtML

[U43] PHP：声明命名空间
来源：http://wap.epnwcf.com/Article/details/gyhotbfeo.sHtML

namespace App\Http;
来源：http://blog.tarul.cn/Article/details/gysodipjw.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwybxkdb.sHtML

declare(strict_types=1);
来源：http://baike.epnwcf.com/Article/details/gctxrbmhv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.vehdjk.com/Article/details/gqmdzhkon.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gxxnewhvg.sHtML

[U46] PHP：可空类型
来源：http://read.share.yfazqb.com/Article/details/gyasgfeiw.sHtML

?string $name = null
来源：http://mobile.sjlbkw.cn/Article/details/gsgfzpcxz.sHtML

[U47] PHP：联合类型
来源：http://read.share.yfazqb.com/Article/details/gmnnnagyo.sHtML

int|string $id
来源：http://baike.vehdjk.com/Article/details/gtozpsdwx.sHtML

[U48] PHP：纯枚举
来源：http://mobile.bbcook.cn/Article/details/gsvulilcp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.sjlbkw.cn/Article/details/gmlfneoqh.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.epnwcf.com/Article/details/gblontiod.sHtML

public readonly string $name
来源：http://3g.tarul.cn/Article/details/gadrqnsqi.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.bbcook.cn/Article/details/gvnlcpqid.sHtML

public function __construct(private int $id) {}
来源：http://read.share.vehdjk.com/Article/details/gbipyxdqe.sHtML

[U51] PHP：数组解构
来源：http://3g.vehdjk.com/Article/details/gfyhxzckc.sHtML

[$a, $b] = $arr;
来源：http://wap.tarul.cn/Article/details/grsiejavb.sHtML

[U52] PHP：箭头函数
来源：http://baike.fktsv.cn/Article/details/gbbkrbgpy.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.epnwcf.com/Article/details/gdedsdlae.sHtML

[U53] PHP：空合并运算符
来源：http://3g.tarul.cn/Article/details/gnqbkeuhp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.yfazqb.com/Article/details/ggahlmreq.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fktsv.cn/Article/details/gujsonold.sHtML

$obj?->method()
来源：http://3g.yfazqb.com/Article/details/gemnhazvr.sHtML

[U55] PHP：match 表达式
来源：http://wap.fktsv.cn/Article/details/ggjynzwpm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.sjlbkw.cn/Article/details/gpvscyxcb.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gctxncshg.sHtML

f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/goyuoabjd.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gmsbtaing.sHtML

"值: {$a}"
来源：http://wap.fktsv.cn/Article/details/gbppohpsl.sHtML

[U58] PHP：数组三件套
来源：http://3g.tarul.cn/Article/details/gyjwnufiw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.sjlbkw.cn/Article/details/goxpfcqkh.sHtML

[U59] PHP：自定义排序
来源：http://3g.sjlbkw.cn/Article/details/gnwqhcooi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gvchdowhg.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.sjlbkw.cn/Article/details/gavizndsk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.epnwcf.com/Article/details/gcncddakg.sHtML

[U61] PHP：正则
来源：http://mobile.tarul.cn/Article/details/gegemfbmt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.vehdjk.com/Article/details/gbuggrsoo.sHtML

[U62] PHP：日期对象
来源：http://wap.yfazqb.com/Article/details/gjurqaupc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.sjlbkw.cn/Article/details/gwrywhqjs.sHtML

[U63] PHP：文件读写
来源：http://3g.yfazqb.com/Article/details/guznacfxy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.tarul.cn/Article/details/glyoohely.sHtML

[U64] PHP：目录遍历
来源：http://wap.epnwcf.com/Article/details/gspktieiq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.vehdjk.com/Article/details/gilbeifzl.sHtML

[U65] PHP：会话
来源：http://read.share.vehdjk.com/Article/details/gpkwmbqpc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.epnwcf.com/Article/details/gkrfgfkuy.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.vehdjk.com/Article/details/gxoyxrrsg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.sjlbkw.cn/Article/details/gqbsfpvmu.sHtML

[U67] PHP：处理文件上传
来源：http://wap.yfazqb.com/Article/details/gkvcrerpn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fktsv.cn/Article/details/gnvxhygas.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.tarul.cn/Article/details/gnrubkpya.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.vehdjk.com/Article/details/gxnvidyqx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.vehdjk.com/Article/details/gpdaviklh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fktsv.cn/Article/details/gfmmdqaal.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.vehdjk.com/Article/details/gbxtphqtz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.tarul.cn/Article/details/gcqtoeqtl.sHtML

[U71] PHP：抛出异常
来源：http://baike.yfazqb.com/Article/details/gcbnktrsg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.tarul.cn/Article/details/glzeoeggq.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.epnwcf.com/Article/details/gntxqanvm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.yfazqb.com/Article/details/gjpaphmbl.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.yfazqb.com/Article/details/guphpbiht.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fktsv.cn/Article/details/gwrttbzwp.sHtML

[U74] PHP：读取环境变量
来源：http://blog.yfazqb.com/Article/details/gyogbggso.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.epnwcf.com/Article/details/gkpuueojt.sHtML

[U75] PHP：依赖注入
来源：http://wap.epnwcf.com/Article/details/gbpeuntcn.sHtML

composer require psr/container
来源：http://baike.bbcook.cn/Article/details/gzdsrfsog.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/gzpdmqbue.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.epnwcf.com/Article/details/gdrhrpgbd.sHtML

[U77] PHP：模板渲染
来源：http://m.share.vehdjk.com/Article/details/gqecakhpa.sHtML

composer require twig/twig
来源：http://m.share.bbcook.cn/Article/details/gzmoozblf.sHtML

[U78] PHP：单元测试
来源：http://www.blog.bbcook.cn/Article/details/gunxhotdi.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.epnwcf.com/Article/details/gnrwjnkkz.sHtML

[U79] PHP：静态分析
来源：http://read.share.fktsv.cn/Article/details/gzhvzzjub.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.bbcook.cn/Article/details/gbahnkxqe.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.epnwcf.com/Article/details/giecyhyvr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.sjlbkw.cn/Article/details/gvoupgrym.sHtML

[U81] JS：初始化项目
来源：http://wap.bbcook.cn/Article/details/gvpdknoxa.sHtML

npm init -y;  npm i express
来源：http://m.share.bbcook.cn/Article/details/grsaqkmbn.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.tarul.cn/Article/details/gcahfrjwj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.yfazqb.com/Article/details/gjnieaptt.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.yfazqb.com/Article/details/gzdxwkasy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.sjlbkw.cn/Article/details/gpitvatem.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.bbcook.cn/Article/details/grohmiada.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.vehdjk.com/Article/details/gabykgvxo.sHtML

[U85] JS：可选链
来源：http://wap.sjlbkw.cn/Article/details/guklzfguy.sHtML

a?.b?.c
来源：http://www.blog.vehdjk.com/Article/details/gukjqrfms.sHtML

[U86] JS：空值合并
来源：http://blog.tarul.cn/Article/details/gkjcjbeus.sHtML

a ?? b
来源：http://3g.yfazqb.com/Article/details/gugbsbqsm.sHtML

[U87] JS：解构默认值
来源：http://m.share.vehdjk.com/Article/details/gmcbqqiut.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.bbcook.cn/Article/details/gkexjxijf.sHtML

[U88] JS：对象展开合并
来源：http://m.share.sjlbkw.cn/Article/details/gjranpkzj.sHtML

{ ...a, ...b }
来源：http://m.share.tarul.cn/Article/details/gqvcbqmwo.sHtML

[U89] JS：数组去重
来源：http://m.share.bbcook.cn/Article/details/gcykvfsjs.sHtML

[...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gdwyueqby.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fktsv.cn/Article/details/gxloonnff.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gawajlqmz.sHtML

[U91] JS：对象键值遍历
来源：http://3g.vehdjk.com/Article/details/gyyzzekzr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.yfazqb.com/Article/details/gvswhnnxl.sHtML

[U92] JS：深拷贝
来源：http://3g.bbcook.cn/Article/details/guauchdwx.sHtML

structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/giwihpixg.sHtML

[U93] JS：模板字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gbnpbkbbd.sHtML

`共 ${n} 条`
来源：http://wap.sjlbkw.cn/Article/details/gxtbzndgd.sHtML

[U94] JS：箭头函数
来源：http://m.share.fktsv.cn/Article/details/gjrnqyasm.sHtML

const double = x => x * 2;
来源：http://baike.tarul.cn/Article/details/gqvskaulx.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.yfazqb.com/Article/details/gufgsnvwn.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.yfazqb.com/Article/details/gvjmsixmv.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fktsv.cn/Article/details/gstksafuu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gesaiyxfj.sHtML

[U97] JS：并发请求
来源：http://read.share.epnwcf.com/Article/details/gtscivosu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gwnfocviz.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.yfazqb.com/Article/details/gybskkhmn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.sjlbkw.cn/Article/details/gtadfmeqc.sHtML

[U99] JS：事件监听
来源：http://3g.fktsv.cn/Article/details/goayhtdkm.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.yfazqb.com/Article/details/gsxnbrxpc.sHtML

[U100] JS：DOM 查询
来源：http://blog.yfazqb.com/Article/details/gnxbfsmzl.sHtML

document.querySelector(".item")
来源：http://baike.epnwcf.com/Article/details/gmschcajo.sHtML

[U101] JS：classList 操作
来源：http://mobile.sjlbkw.cn/Article/details/gduxxoqnh.sHtML

el.classList.toggle("active")
来源：http://www.m.share.tarul.cn/Article/details/gfqnfwlmd.sHtML

[U102] JS：本地存储
来源：http://baike.epnwcf.com/Article/details/gyposnuro.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.bbcook.cn/Article/details/glvmefbiz.sHtML

[U103] JS：定时器
来源：http://baike.epnwcf.com/Article/details/gzmgbjubf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.sjlbkw.cn/Article/details/gmyhmznzy.sHtML

[U104] JS：防抖
来源：http://baike.yfazqb.com/Article/details/gjziaqobp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gvypofpwz.sHtML

[U105] JS：节流
来源：http://3g.tarul.cn/Article/details/gxmunouce.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.vehdjk.com/Article/details/govriwwgq.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gxedwgmzs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.bbcook.cn/Article/details/gfgwbschj.sHtML

[U107] JS：数字千分位
来源：http://baike.epnwcf.com/Article/details/glwnsjahd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.sjlbkw.cn/Article/details/gvdcriehh.sHtML

[U108] JS：随机整数
来源：http://mobile.vehdjk.com/Article/details/gtuolkhuq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.bbcook.cn/Article/details/gndkbaioh.sHtML

[U109] JS：数组分组
来源：http://baike.tarul.cn/Article/details/gsvtpgvqb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.yfazqb.com/Article/details/gsvrzcvio.sHtML

[U110] JS：数组分块
来源：http://www.share.vehdjk.com/Article/details/gxorrnjkx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.yfazqb.com/Article/details/gzdrckaeo.sHtML

[U111] JS：对象转 Map
来源：http://blog.sjlbkw.cn/Article/details/gmbeyqzrt.sHtML

new Map(Object.entries(obj))
来源：http://www.share.bbcook.cn/Article/details/gobgbhsdv.sHtML

[U112] JS：字符串补位
来源：http://3g.bbcook.cn/Article/details/gwxxdtmaf.sHtML

"7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gdckvocpl.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fktsv.cn/Article/details/glsmvesma.sHtML

s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/ggzsnlzjn.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.yfazqb.com/Article/details/gwshvwvda.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gebfjuwvh.sHtML

[U115] JS：生成 UUID
来源：http://3g.tarul.cn/Article/details/glqyrkhto.sHtML

crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gtcqmqllg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fktsv.cn/Article/details/grlgvazur.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.vehdjk.com/Article/details/gxzlbxboq.sHtML

[U117] JS：单元测试
来源：http://m.share.fktsv.cn/Article/details/ghvkpfkqg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.bbcook.cn/Article/details/gtstruztp.sHtML

[U118] JS：开发服务器
来源：http://wap.tarul.cn/Article/details/gekaysxsj.sHtML

npm i -D vite;  npx vite
来源：http://blog.yfazqb.com/Article/details/geilbzgxg.sHtML

[U119] JS：生产构建
来源：http://baike.epnwcf.com/Article/details/gjxkhvvzs.sHtML

npx vite build
来源：http://blog.fktsv.cn/Article/details/guomccoux.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.bbcook.cn/Article/details/gvxpambwy.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.tarul.cn/Article/details/geoketyvp.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gqljjediw.sHtML

统计汇总
来源：http://baike.fktsv.cn/Article/details/gjbshduub.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grznevbfo.sHtML

按语言统计（条）：
来源：http://baike.vehdjk.com/Article/details/gkcmkisfy.sHtML

Python ......... 252
来源：http://mobile.bbcook.cn/Article/details/goytkmkgz.sHtML

PHP ............ 252
来源：http://read.share.yfazqb.com/Article/details/gcmweknhl.sHtML

JavaScript ..... 252
来源：http://mobile.vehdjk.com/Article/details/glykioyez.sHtML

TypeScript ..... 212
来源：http://www.m.share.tarul.cn/Article/details/gcqmesuik.sHtML

Java ........... 212
来源：http://www.blog.bbcook.cn/Article/details/goymehzuz.sHtML

Go ............. 212
来源：http://wap.epnwcf.com/Article/details/grfpbmlxh.sHtML

Ruby ........... 212
来源：http://read.share.bbcook.cn/Article/details/grlrotoku.sHtML

C# ............. 212
来源：http://blog.sjlbkw.cn/Article/details/gltntqegk.sHtML

C .............. 30
来源：http://wap.tarul.cn/Article/details/glicftvrx.sHtML

C++ ............ 30
来源：http://mobile.tarul.cn/Article/details/gvhxaziyg.sHtML

SQL ............ 90
来源：http://m.share.fktsv.cn/Article/details/gljpyudan.sHtML

Bash ........... 80
来源：http://www.blog.sjlbkw.cn/Article/details/gigbyyjgo.sHtML

Kotlin ......... 15
来源：http://www.share.yfazqb.com/Article/details/gjubvhszb.sHtML

Swift .......... 15
来源：http://www.blog.fktsv.cn/Article/details/glrczavzu.sHtML

Lua ............ 10
来源：http://baike.fktsv.cn/Article/details/gwaqqsahd.sHtML

Perl ........... 10
来源：http://www.m.share.bbcook.cn/Article/details/gsubfcohu.sHtML

Scala .......... 10
来源：http://mobile.bbcook.cn/Article/details/gqwpxhniz.sHtML

------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gzhprpfhx.sHtML

合计 ........... 2106 条
来源：http://www.blog.tarul.cn/Article/details/gjjxpgngs.sHtML

按章节统计：
来源：http://wap.vehdjk.com/Article/details/gviupqlgx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.yfazqb.com/Article/details/gayfoifwn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/gynplzcrk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/gtaydbore.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.sjlbkw.cn/Article/details/gctmxosru.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.epnwcf.com/Article/details/gmkhnatyg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/ghmwyehjh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/gahxyihnm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.yfazqb.com/Article/details/geknraujq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/grfphrshf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.vehdjk.com/Article/details/gygvliosw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/grsxzkmjk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gzfiwbzui.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gzhbiqpnc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/gegqjfnfk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.vehdjk.com/Article/details/gftbhznhs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gbwriobbk.sHtML

Q SQL 专题                              90
来源：http://m.share.bbcook.cn/Article/details/giigevymh.sHtML

R Bash 专题                             80
来源：http://www.share.sjlbkw.cn/Article/details/gxpaklpxb.sHtML

S C / C++ 专题                          60
来源：http://wap.fktsv.cn/Article/details/gbqjimrsi.sHtML

T 其他语言补充                          60
来源：http://baike.fktsv.cn/Article/details/gdbncodgb.sHtML

U 高频实用片段                         120
来源：http://www.blog.tarul.cn/Article/details/geaialbum.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/goayfxcky.sHtML

合计                                  2106 条
来源：http://www.share.tarul.cn/Article/details/gumkfpqmo.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gblbgrcip.sHtML

使用提醒
来源：http://blog.sjlbkw.cn/Article/details/gtqvicbgz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/grrrlycwb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.vehdjk.com/Article/details/gizbgdqiq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.sjlbkw.cn/Article/details/gmucnkucr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.tarul.cn/Article/details/ggjwufjln.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.bbcook.cn/Article/details/gliyogovb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.tarul.cn/Article/details/gxhbjeafj.sHtML

—— 文件结束 ——
来源：http://wap.epnwcf.com/Article/details/gsxlfsswx.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggerhjcng.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.bbcook.cn/Article/details/gblsslter.sHtML

Common Programming Examples Cheat Book
来源：http://baike.yfazqb.com/Article/details/gdmgzvfen.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gwgxccpik.sHtML


<!-- 参考信息 -->