代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.tarul.cn/Article/details/gfdyhwbxt.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gqvdpwzsy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/gbiickfqs.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxugafrbb.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.bbcook.cn/Article/details/gfuncdqfm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gvzubsars.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.yfazqb.com/Article/details/gtkzupyqq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.bbcook.cn/Article/details/gfatalmjr.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.epnwcf.com/Article/details/gpkuwgdft.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.sjlbkw.cn/Article/details/gokwqrrzs.sHtML

[U04] Py：变量调试打印
来源：http://3g.epnwcf.com/Article/details/gafkagfpy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.tarul.cn/Article/details/ghrqrllsj.sHtML

[U05] Py：列表去重且保序
来源：http://baike.yfazqb.com/Article/details/ghbpxagwl.sHtML

list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/ghhwxfpaa.sHtML

[U06] Py：合并两个字典
来源：http://blog.epnwcf.com/Article/details/glnfxglvy.sHtML

{**a, **b}
来源：http://3g.epnwcf.com/Article/details/gcywnsgoe.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.sjlbkw.cn/Article/details/gocscitmo.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.yfazqb.com/Article/details/gyhtidzgk.sHtML

[U08] Py：展平二维列表
来源：http://mobile.tarul.cn/Article/details/gdyfzmpjl.sHtML

[y for x in nested for y in x]
来源：http://www.share.vehdjk.com/Article/details/gjwmukqkj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fktsv.cn/Article/details/gnruukgls.sHtML

max(d, key=d.get)
来源：http://www.m.share.epnwcf.com/Article/details/gacwxaeuf.sHtML

[U10] Py：按值排序字典
来源：http://blog.vehdjk.com/Article/details/giyxhwlyf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.epnwcf.com/Article/details/gnitvukyb.sHtML

[U11] Py：生成器表达式
来源：http://baike.tarul.cn/Article/details/gfzlqekrn.sHtML

(x * 2 for x in arr)
来源：http://www.blog.yfazqb.com/Article/details/gtwzykiwz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.epnwcf.com/Article/details/gjkigetnx.sHtML

Counter(arr).most_common(3)
来源：http://wap.epnwcf.com/Article/details/gledrtpqn.sHtML

[U13] Py：固定长度队列
来源：http://www.share.epnwcf.com/Article/details/gpocwqkjd.sHtML

deque(maxlen=10)
来源：http://www.m.share.vehdjk.com/Article/details/giiprizgn.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.bbcook.cn/Article/details/gkhctnjla.sHtML

defaultdict(list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwmkqtkz.sHtML

[U15] Py：高精度计时
来源：http://www.share.bbcook.cn/Article/details/gcszzogvx.sHtML

t = time.perf_counter()
来源：http://3g.yfazqb.com/Article/details/gktkfprae.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.tarul.cn/Article/details/gafkazytv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.sjlbkw.cn/Article/details/ggljmvgyd.sHtML

[U17] Py：初始化日志
来源：http://m.share.epnwcf.com/Article/details/gccutdyjp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.vehdjk.com/Article/details/ggxkjmkdw.sHtML

[U18] Py：预编译正则
来源：http://wap.tarul.cn/Article/details/gfhzayawp.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.vehdjk.com/Article/details/gmmpqalpx.sHtML

[U19] Py：正则替换带回调
来源：http://3g.bbcook.cn/Article/details/geoenopbb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.epnwcf.com/Article/details/gsrsqtbaw.sHtML

[U20] Py：缓存函数结果
来源：http://blog.yfazqb.com/Article/details/gmybcuugl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fktsv.cn/Article/details/gsppljkhv.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.vehdjk.com/Article/details/ggeohusfs.sHtML

@contextlib.contextmanager
来源：http://mobile.tarul.cn/Article/details/ggvamvxih.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fktsv.cn/Article/details/glinmktnm.sHtML

list(zip(*m))
来源：http://www.m.share.yfazqb.com/Article/details/gojcljksn.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.tarul.cn/Article/details/gifxtzdkf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fktsv.cn/Article/details/gsggllypz.sHtML

[U24] Py：路径操作
来源：http://read.share.fktsv.cn/Article/details/gdcrwfdfs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/gstcmacku.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fktsv.cn/Article/details/gldyfalmc.sHtML

csv.DictReader(f)
来源：http://blog.epnwcf.com/Article/details/gtjydufrp.sHtML

[U26] Py：并发下载
来源：http://mobile.tarul.cn/Article/details/glletmcck.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.tarul.cn/Article/details/gxycgrqih.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fktsv.cn/Article/details/gpcubkcxw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.yfazqb.com/Article/details/ggwamwxns.sHtML

[U28] Py：类型别名
来源：http://m.share.epnwcf.com/Article/details/gdscmhadt.sHtML

UserId = int
来源：http://mobile.fktsv.cn/Article/details/guxcvzzhq.sHtML

[U29] Py：属性校验
来源：http://baike.bbcook.cn/Article/details/gompnvwuc.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.sjlbkw.cn/Article/details/gneeuufem.sHtML

[U30] Py：数据类
来源：http://m.share.yfazqb.com/Article/details/gpycgqiyk.sHtML

@dataclass(slots=True)
来源：http://mobile.bbcook.cn/Article/details/gijeelgiv.sHtML

[U31] Py：单测
来源：http://baike.fktsv.cn/Article/details/gtrradhaf.sHtML

python -m pytest -q
来源：http://baike.bbcook.cn/Article/details/gryacqtnm.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.epnwcf.com/Article/details/gjnjioouw.sHtML

ruff format . && ruff check --fix .
来源：http://3g.bbcook.cn/Article/details/gjrultmlj.sHtML

[U33] Py：打包发布
来源：http://read.share.sjlbkw.cn/Article/details/gazmbqqvd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fktsv.cn/Article/details/gwsnalvbq.sHtML

[U34] Py：判断编码
来源：http://www.m.share.bbcook.cn/Article/details/gimkmmfee.sHtML

chardet.detect(raw)
来源：http://wap.bbcook.cn/Article/details/gqkmmaihf.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.yfazqb.com/Article/details/gvrjdkhoo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fktsv.cn/Article/details/gwrryacpl.sHtML

[U36] Py：定时任务
来源：http://www.share.tarul.cn/Article/details/gfaunbkou.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.vehdjk.com/Article/details/gnxrrncvm.sHtML

[U37] Py：读写 Excel
来源：http://www.share.sjlbkw.cn/Article/details/getqkkybc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fktsv.cn/Article/details/gavfubaiy.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.tarul.cn/Article/details/gysagdfuo.sHtML

Path(__file__).resolve().parent
来源：http://read.share.vehdjk.com/Article/details/gfdxgxsgh.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.bbcook.cn/Article/details/gwjleqifw.sHtML

sys.stdout.isatty()
来源：http://www.blog.sjlbkw.cn/Article/details/gudjeojul.sHtML

[U40] Py：打印到标准错误
来源：http://blog.tarul.cn/Article/details/gidoohtxv.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/gnvxjokmr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.epnwcf.com/Article/details/gbgqapose.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.bbcook.cn/Article/details/gkbbkanpl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.vehdjk.com/Article/details/gnzcvssza.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.vehdjk.com/Article/details/gkdixaoqh.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.vehdjk.com/Article/details/gznccrqtx.sHtML

namespace App\Http;
来源：http://www.blog.epnwcf.com/Article/details/gputqwqaz.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fktsv.cn/Article/details/gwhwibqyg.sHtML

declare(strict_types=1);
来源：http://wap.yfazqb.com/Article/details/grcmctwcw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fktsv.cn/Article/details/ghebrkdva.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gowopscgr.sHtML

[U46] PHP：可空类型
来源：http://wap.fktsv.cn/Article/details/gbqmfkxsm.sHtML

?string $name = null
来源：http://www.m.share.epnwcf.com/Article/details/gjlsoeouo.sHtML

[U47] PHP：联合类型
来源：http://www.blog.tarul.cn/Article/details/gtqffogmz.sHtML

int|string $id
来源：http://wap.bbcook.cn/Article/details/gxzqynjgj.sHtML

[U48] PHP：纯枚举
来源：http://read.share.bbcook.cn/Article/details/gcormjiao.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.vehdjk.com/Article/details/ggrkegicw.sHtML

[U49] PHP：只读属性
来源：http://blog.epnwcf.com/Article/details/gbscdzrzz.sHtML

public readonly string $name
来源：http://www.share.epnwcf.com/Article/details/guklqzoed.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.bbcook.cn/Article/details/gqkmvbfbb.sHtML

public function __construct(private int $id) {}
来源：http://3g.tarul.cn/Article/details/guqkbrjqp.sHtML

[U51] PHP：数组解构
来源：http://read.share.yfazqb.com/Article/details/guukaydil.sHtML

[$a, $b] = $arr;
来源：http://wap.fktsv.cn/Article/details/gydlidhlr.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/guyedrkoi.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fktsv.cn/Article/details/gbubusjni.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.vehdjk.com/Article/details/gqalirqyn.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.epnwcf.com/Article/details/gfpnciicx.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.bbcook.cn/Article/details/guzcvoluc.sHtML

$obj?->method()
来源：http://blog.bbcook.cn/Article/details/gcktudghw.sHtML

[U55] PHP：match 表达式
来源：http://read.share.tarul.cn/Article/details/gzpoezcps.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.vehdjk.com/Article/details/gcnvryssy.sHtML

[U56] PHP：命名参数
来源：http://www.share.tarul.cn/Article/details/gnnqidhjj.sHtML

f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gbtwuldst.sHtML

[U57] PHP：字符串插值
来源：http://3g.vehdjk.com/Article/details/grdazevuv.sHtML

"值: {$a}"
来源：http://wap.yfazqb.com/Article/details/gwpgktkhy.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.sjlbkw.cn/Article/details/gvpwzsihz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.tarul.cn/Article/details/gxakmvnww.sHtML

[U59] PHP：自定义排序
来源：http://m.share.yfazqb.com/Article/details/gajlkzeef.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/gdtngdeoe.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.epnwcf.com/Article/details/gwujqdktd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.epnwcf.com/Article/details/gcbepmjwp.sHtML

[U61] PHP：正则
来源：http://wap.sjlbkw.cn/Article/details/gsmyqxfjc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/gldvoydso.sHtML

[U62] PHP：日期对象
来源：http://wap.sjlbkw.cn/Article/details/gpanhzblu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fktsv.cn/Article/details/gbroxjgng.sHtML

[U63] PHP：文件读写
来源：http://m.share.tarul.cn/Article/details/gtpjjtmzl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fktsv.cn/Article/details/gwgiwfade.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.bbcook.cn/Article/details/gkejzarko.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.epnwcf.com/Article/details/gpicfytwo.sHtML

[U65] PHP：会话
来源：http://wap.sjlbkw.cn/Article/details/gugxrlfpe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gktdizigy.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.tarul.cn/Article/details/gsjxbxyqa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.tarul.cn/Article/details/gawbiqvbu.sHtML

[U67] PHP：处理文件上传
来源：http://baike.tarul.cn/Article/details/gjjnulqst.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.bbcook.cn/Article/details/gprngyapw.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.bbcook.cn/Article/details/gxbknasjl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.sjlbkw.cn/Article/details/ghnbofrsk.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.tarul.cn/Article/details/gcwymxwxc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.bbcook.cn/Article/details/gkqhvzcty.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.epnwcf.com/Article/details/giksqjicv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.tarul.cn/Article/details/gqtomhvrn.sHtML

[U71] PHP：抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gagxabgwf.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.vehdjk.com/Article/details/gsasjpuii.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fktsv.cn/Article/details/gzwtivyhi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.sjlbkw.cn/Article/details/gjhmerftz.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fktsv.cn/Article/details/glhuuflgi.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fktsv.cn/Article/details/gqqalwqkb.sHtML

[U74] PHP：读取环境变量
来源：http://wap.epnwcf.com/Article/details/gsodiwphm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fktsv.cn/Article/details/gehjlmkqm.sHtML

[U75] PHP：依赖注入
来源：http://m.share.vehdjk.com/Article/details/gfinvodof.sHtML

composer require psr/container
来源：http://www.blog.fktsv.cn/Article/details/gnqznssjq.sHtML

[U76] PHP：简单路由
来源：http://baike.epnwcf.com/Article/details/gbmaqswle.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.vehdjk.com/Article/details/giabwdmeq.sHtML

[U77] PHP：模板渲染
来源：http://3g.yfazqb.com/Article/details/glqnlqksg.sHtML

composer require twig/twig
来源：http://wap.fktsv.cn/Article/details/gbaeqeabd.sHtML

[U78] PHP：单元测试
来源：http://mobile.vehdjk.com/Article/details/gmbndxaeq.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fktsv.cn/Article/details/gfzbllmvu.sHtML

[U79] PHP：静态分析
来源：http://blog.tarul.cn/Article/details/gdjcvpabt.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.sjlbkw.cn/Article/details/gxaboifld.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.epnwcf.com/Article/details/gwpdqgdyy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.tarul.cn/Article/details/gwpnslcnb.sHtML

[U81] JS：初始化项目
来源：http://read.share.sjlbkw.cn/Article/details/gocynfpuw.sHtML

npm init -y;  npm i express
来源：http://www.m.share.tarul.cn/Article/details/ghiestgcs.sHtML

[U82] JS：package.json 脚本
来源：http://blog.vehdjk.com/Article/details/gyyjehcnu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.sjlbkw.cn/Article/details/gkcqdpncc.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.yfazqb.com/Article/details/grjiubixs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/gfqyoppee.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.sjlbkw.cn/Article/details/giarsblcf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.bbcook.cn/Article/details/gbxefjbyl.sHtML

[U85] JS：可选链
来源：http://3g.bbcook.cn/Article/details/gdtpzmnrr.sHtML

a?.b?.c
来源：http://blog.tarul.cn/Article/details/gfovjviyd.sHtML

[U86] JS：空值合并
来源：http://wap.tarul.cn/Article/details/gnuaquyip.sHtML

a ?? b
来源：http://m.share.bbcook.cn/Article/details/gngcgwbcu.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.vehdjk.com/Article/details/gfhhgpvnd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fktsv.cn/Article/details/gnlrnbvze.sHtML

[U88] JS：对象展开合并
来源：http://www.share.sjlbkw.cn/Article/details/geyijmgoe.sHtML

{ ...a, ...b }
来源：http://read.share.vehdjk.com/Article/details/gvwfxwczw.sHtML

[U89] JS：数组去重
来源：http://www.share.vehdjk.com/Article/details/glestzpos.sHtML

[...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gzrvgrxlf.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.yfazqb.com/Article/details/gkhholcde.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gacbwcmda.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.vehdjk.com/Article/details/gzaolzfcy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhdvnbsz.sHtML

[U92] JS：深拷贝
来源：http://m.share.tarul.cn/Article/details/gbgvrxzim.sHtML

structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gezdbapvg.sHtML

[U93] JS：模板字符串
来源：http://baike.epnwcf.com/Article/details/guckuogrf.sHtML

`共 ${n} 条`
来源：http://www.blog.tarul.cn/Article/details/gxcocwtdz.sHtML

[U94] JS：箭头函数
来源：http://wap.vehdjk.com/Article/details/gbeanjguu.sHtML

const double = x => x * 2;
来源：http://3g.vehdjk.com/Article/details/gtrdylfvb.sHtML

[U95] JS：Promise 包装
来源：http://m.share.vehdjk.com/Article/details/gapuiwsko.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.sjlbkw.cn/Article/details/gzxlkvhtx.sHtML

[U96] JS：async/await 与异常
来源：http://wap.sjlbkw.cn/Article/details/gjhvlwico.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gfwxpbkkl.sHtML

[U97] JS：并发请求
来源：http://m.share.vehdjk.com/Article/details/gbzngwwdw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gqubhoroc.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.tarul.cn/Article/details/gyaskvynf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.bbcook.cn/Article/details/gwcxytwgj.sHtML

[U99] JS：事件监听
来源：http://www.m.share.epnwcf.com/Article/details/gfmdwvzue.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.sjlbkw.cn/Article/details/gadycswlj.sHtML

[U100] JS：DOM 查询
来源：http://3g.tarul.cn/Article/details/gxukogpvb.sHtML

document.querySelector(".item")
来源：http://read.share.tarul.cn/Article/details/gwhugotpp.sHtML

[U101] JS：classList 操作
来源：http://blog.bbcook.cn/Article/details/gitrvrrdm.sHtML

el.classList.toggle("active")
来源：http://www.blog.fktsv.cn/Article/details/gbwyltkah.sHtML

[U102] JS：本地存储
来源：http://www.m.share.yfazqb.com/Article/details/gdiaysgcd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.vehdjk.com/Article/details/gscibavhe.sHtML

[U103] JS：定时器
来源：http://read.share.epnwcf.com/Article/details/ghzjdipjj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fktsv.cn/Article/details/gkxgrdrzm.sHtML

[U104] JS：防抖
来源：http://read.share.tarul.cn/Article/details/gjxhpgmbi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/giegtcizf.sHtML

[U105] JS：节流
来源：http://3g.epnwcf.com/Article/details/gxlinixao.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.sjlbkw.cn/Article/details/gdiyrylfu.sHtML

[U106] JS：日期格式化
来源：http://baike.vehdjk.com/Article/details/gmlkesnzg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fktsv.cn/Article/details/gpekqtdmm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fktsv.cn/Article/details/graxsqdpi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/gwdaqggjq.sHtML

[U108] JS：随机整数
来源：http://read.share.bbcook.cn/Article/details/grmccqdrq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fktsv.cn/Article/details/ggbklgxhf.sHtML

[U109] JS：数组分组
来源：http://read.share.epnwcf.com/Article/details/grzwhfwez.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.tarul.cn/Article/details/glmyoshjv.sHtML

[U110] JS：数组分块
来源：http://mobile.bbcook.cn/Article/details/gokhmdenc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.vehdjk.com/Article/details/gdisrqofu.sHtML

[U111] JS：对象转 Map
来源：http://blog.tarul.cn/Article/details/gakrhcyfh.sHtML

new Map(Object.entries(obj))
来源：http://mobile.vehdjk.com/Article/details/gzqojojup.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.bbcook.cn/Article/details/gavpwggsp.sHtML

"7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/geycadjks.sHtML

[U113] JS：正则替换全部
来源：http://blog.epnwcf.com/Article/details/gcgcxnusj.sHtML

s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gvetveqsv.sHtML

[U114] JS：JSON 深比较
来源：http://blog.vehdjk.com/Article/details/gtxdsawmh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/gqwtromve.sHtML

[U115] JS：生成 UUID
来源：http://m.share.vehdjk.com/Article/details/grmixssxr.sHtML

crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gpkdxhfwa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.epnwcf.com/Article/details/ghwfpsiau.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.epnwcf.com/Article/details/gkicsiyxp.sHtML

[U117] JS：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gylziwurm.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fktsv.cn/Article/details/gjzulokcf.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fktsv.cn/Article/details/gmceufpvx.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.vehdjk.com/Article/details/gcksrkvpg.sHtML

[U119] JS：生产构建
来源：http://blog.yfazqb.com/Article/details/gkgakjjew.sHtML

npx vite build
来源：http://www.blog.vehdjk.com/Article/details/geyurxlsz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.sjlbkw.cn/Article/details/gwligobrw.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.tarul.cn/Article/details/gsablougy.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbiefwgvc.sHtML

统计汇总
来源：http://baike.bbcook.cn/Article/details/gsvkbkwqe.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gjnifgzsm.sHtML

按语言统计（条）：
来源：http://www.blog.tarul.cn/Article/details/gcbvrnjln.sHtML

Python ......... 252
来源：http://wap.sjlbkw.cn/Article/details/gzffzeaxg.sHtML

PHP ............ 252
来源：http://3g.sjlbkw.cn/Article/details/gzoshcctg.sHtML

JavaScript ..... 252
来源：http://www.blog.yfazqb.com/Article/details/gisgesadw.sHtML

TypeScript ..... 212
来源：http://m.share.tarul.cn/Article/details/gahlkcdnx.sHtML

Java ........... 212
来源：http://www.share.yfazqb.com/Article/details/gnxgwjoef.sHtML

Go ............. 212
来源：http://www.m.share.fktsv.cn/Article/details/gzdjmrzdh.sHtML

Ruby ........... 212
来源：http://www.blog.bbcook.cn/Article/details/gcypxyynj.sHtML

C# ............. 212
来源：http://m.share.bbcook.cn/Article/details/gbxkycfmo.sHtML

C .............. 30
来源：http://blog.vehdjk.com/Article/details/gqdrbvigo.sHtML

C++ ............ 30
来源：http://www.share.yfazqb.com/Article/details/gsklovjwp.sHtML

SQL ............ 90
来源：http://www.blog.epnwcf.com/Article/details/gdnmiqohb.sHtML

Bash ........... 80
来源：http://www.share.bbcook.cn/Article/details/gtcebczrl.sHtML

Kotlin ......... 15
来源：http://blog.bbcook.cn/Article/details/gxgzbwuwt.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/guzbnendq.sHtML

Lua ............ 10
来源：http://read.share.bbcook.cn/Article/details/gcsslqgzo.sHtML

Perl ........... 10
来源：http://read.share.fktsv.cn/Article/details/goidxibsg.sHtML

Scala .......... 10
来源：http://3g.tarul.cn/Article/details/glcgzwous.sHtML

------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gmkspnckj.sHtML

合计 ........... 2106 条
来源：http://www.blog.fktsv.cn/Article/details/gzncmwzqw.sHtML

按章节统计：
来源：http://www.blog.sjlbkw.cn/Article/details/gozlycgtp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gbaeroaiw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.epnwcf.com/Article/details/gajahqebd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/gytlzkavz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gehlllncf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.vehdjk.com/Article/details/gqnsoviqv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.tarul.cn/Article/details/gpqdfmrkt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/gfbjnjuoa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.tarul.cn/Article/details/gryvhvoyq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gkhwqmsbp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fktsv.cn/Article/details/glrvzapjm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/glqbykbsv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gdrunutom.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gjkoesvuk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.yfazqb.com/Article/details/gweafprnm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.sjlbkw.cn/Article/details/gxxktowcn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gqwojzonj.sHtML

Q SQL 专题                              90
来源：http://blog.fktsv.cn/Article/details/gfrahumzr.sHtML

R Bash 专题                             80
来源：http://m.share.epnwcf.com/Article/details/guulaptje.sHtML

S C / C++ 专题                          60
来源：http://3g.epnwcf.com/Article/details/gigwsjzkr.sHtML

T 其他语言补充                          60
来源：http://baike.epnwcf.com/Article/details/gnorqxmpd.sHtML

U 高频实用片段                         120
来源：http://mobile.epnwcf.com/Article/details/gxkiailre.sHtML

------------------------------------
来源：http://mobile.tarul.cn/Article/details/gtkomipab.sHtML

合计                                  2106 条
来源：http://blog.epnwcf.com/Article/details/gnnzljbfb.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gdayqygib.sHtML

使用提醒
来源：http://www.share.vehdjk.com/Article/details/gvhhoeszz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gmpdfmcmy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.tarul.cn/Article/details/gxgpgnwzs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.bbcook.cn/Article/details/grzqwrimf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.tarul.cn/Article/details/gzmttmrie.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fktsv.cn/Article/details/grbmrsxxn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.vehdjk.com/Article/details/gsjjkfzqh.sHtML

—— 文件结束 ——
来源：http://baike.sjlbkw.cn/Article/details/ghuouwvby.sHtML


<!-- 参考信息 -->