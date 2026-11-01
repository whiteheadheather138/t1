代发 wailian999

case class User(name: String, age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/giruuofda.sHtML

[T57] Scala：模式匹配
来源：http://3g.yfazqb.com/Article/details/gooidqwgz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fktsv.cn/Article/details/gzovcvnig.sHtML

[T58] Scala：函数定义
来源：http://mobile.fktsv.cn/Article/details/gbkjwtupn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.tarul.cn/Article/details/ghgpaftvp.sHtML

[T59] Scala：循环
来源：http://www.m.share.bbcook.cn/Article/details/gvwamhkbm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gwngryphk.sHtML

[T60] Scala：折叠
来源：http://mobile.vehdjk.com/Article/details/gzpxskqzb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.sjlbkw.cn/Article/details/gbnzqvetl.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gccgoqrns.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fktsv.cn/Article/details/gtemrkkfx.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzujlufju.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.epnwcf.com/Article/details/gawspxnmh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.yfazqb.com/Article/details/gqexywhel.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.vehdjk.com/Article/details/ggzkyltzo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.vehdjk.com/Article/details/gcnhyyple.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.tarul.cn/Article/details/geaniwnay.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fktsv.cn/Article/details/gybnqeucx.sHtML

[U04] Py：变量调试打印
来源：http://mobile.sjlbkw.cn/Article/details/gnqvqjbdf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.tarul.cn/Article/details/gdzzvqlnl.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/gphvxqrqx.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gsedtexlc.sHtML

[U06] Py：合并两个字典
来源：http://blog.vehdjk.com/Article/details/gvgxyqlof.sHtML

{**a, **b}
来源：http://read.share.fktsv.cn/Article/details/gcbnlduwf.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gnquzbbtj.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.tarul.cn/Article/details/gjholcult.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.epnwcf.com/Article/details/gtfaitkpk.sHtML

[y for x in nested for y in x]
来源：http://blog.sjlbkw.cn/Article/details/gwmwfxeof.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.tarul.cn/Article/details/gswziacyw.sHtML

max(d, key=d.get)
来源：http://www.blog.tarul.cn/Article/details/ganqnadbt.sHtML

[U10] Py：按值排序字典
来源：http://blog.bbcook.cn/Article/details/gwciyeigm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.yfazqb.com/Article/details/gbemnajyt.sHtML

[U11] Py：生成器表达式
来源：http://mobile.bbcook.cn/Article/details/goryafozx.sHtML

(x * 2 for x in arr)
来源：http://baike.yfazqb.com/Article/details/gcfmbigie.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.epnwcf.com/Article/details/gznhfgjsm.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpazabjkb.sHtML

[U13] Py：固定长度队列
来源：http://3g.sjlbkw.cn/Article/details/gkvephjnc.sHtML

deque(maxlen=10)
来源：http://www.m.share.tarul.cn/Article/details/gcducvtgw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.epnwcf.com/Article/details/gsswjiaxl.sHtML

defaultdict(list)
来源：http://3g.fktsv.cn/Article/details/gsdsgpsxp.sHtML

[U15] Py：高精度计时
来源：http://mobile.sjlbkw.cn/Article/details/gkajxddmk.sHtML

t = time.perf_counter()
来源：http://wap.sjlbkw.cn/Article/details/gsohimguc.sHtML

[U16] Py：命令行参数解析
来源：http://3g.tarul.cn/Article/details/gngfdaxmh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.yfazqb.com/Article/details/gkbjtxytz.sHtML

[U17] Py：初始化日志
来源：http://www.blog.vehdjk.com/Article/details/ggeglpylc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.sjlbkw.cn/Article/details/gmvuyxqcv.sHtML

[U18] Py：预编译正则
来源：http://blog.yfazqb.com/Article/details/gpubgiwrh.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzalbiye.sHtML

[U19] Py：正则替换带回调
来源：http://wap.tarul.cn/Article/details/gfstgdlnv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.yfazqb.com/Article/details/gphakfawi.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.bbcook.cn/Article/details/gbvvhiqrj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.epnwcf.com/Article/details/govijulfd.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.yfazqb.com/Article/details/gxadjqbim.sHtML

@contextlib.contextmanager
来源：http://blog.bbcook.cn/Article/details/gkgvnougp.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.tarul.cn/Article/details/gffrovafk.sHtML

list(zip(*m))
来源：http://wap.fktsv.cn/Article/details/gtvlntosd.sHtML

[U23] Py：分块读取大文件
来源：http://3g.sjlbkw.cn/Article/details/gmsjqttcc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fktsv.cn/Article/details/gbrxiynip.sHtML

[U24] Py：路径操作
来源：http://m.share.sjlbkw.cn/Article/details/gsesfuhci.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gbxikxsix.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fktsv.cn/Article/details/ggeugdjum.sHtML

csv.DictReader(f)
来源：http://read.share.vehdjk.com/Article/details/gwasyevtz.sHtML

[U26] Py：并发下载
来源：http://read.share.vehdjk.com/Article/details/gfvzphgyk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.sjlbkw.cn/Article/details/gnlakbxwc.sHtML

[U27] Py：异步 HTTP
来源：http://wap.sjlbkw.cn/Article/details/gdjsxdvcc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.bbcook.cn/Article/details/ghazmkqsg.sHtML

[U28] Py：类型别名
来源：http://www.share.tarul.cn/Article/details/gcaxuriyt.sHtML

UserId = int
来源：http://mobile.bbcook.cn/Article/details/gzurtvezr.sHtML

[U29] Py：属性校验
来源：http://www.blog.bbcook.cn/Article/details/gnviiyett.sHtML

@property 与 @x.setter 配合
来源：http://baike.tarul.cn/Article/details/gicoseyvq.sHtML

[U30] Py：数据类
来源：http://www.blog.yfazqb.com/Article/details/guqzvozpv.sHtML

@dataclass(slots=True)
来源：http://read.share.fktsv.cn/Article/details/gnxqfhgwh.sHtML

[U31] Py：单测
来源：http://read.share.yfazqb.com/Article/details/gxtcazymu.sHtML

python -m pytest -q
来源：http://3g.epnwcf.com/Article/details/grzjwpvuc.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.epnwcf.com/Article/details/gegttqrfe.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fktsv.cn/Article/details/gcurharkl.sHtML

[U33] Py：打包发布
来源：http://blog.vehdjk.com/Article/details/ggbigmrzf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.sjlbkw.cn/Article/details/gwicmibyf.sHtML

[U34] Py：判断编码
来源：http://3g.tarul.cn/Article/details/gkzbodptc.sHtML

chardet.detect(raw)
来源：http://baike.tarul.cn/Article/details/gtzabqvws.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fktsv.cn/Article/details/gxrkhnafk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.vehdjk.com/Article/details/gztvkrnee.sHtML

[U36] Py：定时任务
来源：http://wap.yfazqb.com/Article/details/ghbzyfvbz.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.sjlbkw.cn/Article/details/gdutqbdrt.sHtML

[U37] Py：读写 Excel
来源：http://www.share.epnwcf.com/Article/details/ghgqefhag.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fktsv.cn/Article/details/gyeilctdn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.sjlbkw.cn/Article/details/gwfqsrkvx.sHtML

Path(__file__).resolve().parent
来源：http://www.share.yfazqb.com/Article/details/gbkjbpjnf.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.tarul.cn/Article/details/gbheamuwt.sHtML

sys.stdout.isatty()
来源：http://mobile.fktsv.cn/Article/details/gnhpysbzv.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.vehdjk.com/Article/details/gjceqrwbt.sHtML

print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/gmiiwgpwk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fktsv.cn/Article/details/gcxogcqex.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.bbcook.cn/Article/details/gxeccafxk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.sjlbkw.cn/Article/details/gzathttjf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fktsv.cn/Article/details/gtfyakalb.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.yfazqb.com/Article/details/guanieidx.sHtML

namespace App\Http;
来源：http://mobile.sjlbkw.cn/Article/details/gezdogpfw.sHtML

[U44] PHP：开启严格类型
来源：http://wap.vehdjk.com/Article/details/gcdotacvx.sHtML

declare(strict_types=1);
来源：http://blog.tarul.cn/Article/details/grnxaudmn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fktsv.cn/Article/details/gexniiysg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gozjvegmi.sHtML

[U46] PHP：可空类型
来源：http://read.share.tarul.cn/Article/details/gbfwvzmmb.sHtML

?string $name = null
来源：http://www.blog.fktsv.cn/Article/details/gsdwobkik.sHtML

[U47] PHP：联合类型
来源：http://blog.fktsv.cn/Article/details/ghacimdvj.sHtML

int|string $id
来源：http://www.blog.bbcook.cn/Article/details/grjhfedqk.sHtML

[U48] PHP：纯枚举
来源：http://read.share.vehdjk.com/Article/details/ghmlmfdvw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fktsv.cn/Article/details/gtfnsvwao.sHtML

[U49] PHP：只读属性
来源：http://baike.fktsv.cn/Article/details/gwhfrxeow.sHtML

public readonly string $name
来源：http://read.share.bbcook.cn/Article/details/gukneiuic.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.epnwcf.com/Article/details/gellwnnzo.sHtML

public function __construct(private int $id) {}
来源：http://mobile.epnwcf.com/Article/details/gxsouptlr.sHtML

[U51] PHP：数组解构
来源：http://blog.epnwcf.com/Article/details/gaubpofyj.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.epnwcf.com/Article/details/gggsehxva.sHtML

[U52] PHP：箭头函数
来源：http://baike.epnwcf.com/Article/details/gtzkdyerk.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.vehdjk.com/Article/details/gpzuuuojm.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fktsv.cn/Article/details/gtvhyxxrl.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.sjlbkw.cn/Article/details/gnuepsroy.sHtML

[U54] PHP：空安全调用
来源：http://blog.fktsv.cn/Article/details/gbcioatsr.sHtML

$obj?->method()
来源：http://baike.vehdjk.com/Article/details/ghzxgvzzh.sHtML

[U55] PHP：match 表达式
来源：http://3g.epnwcf.com/Article/details/ganskuzfx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.sjlbkw.cn/Article/details/gmqzdjifn.sHtML

[U56] PHP：命名参数
来源：http://mobile.epnwcf.com/Article/details/gqixbqwmd.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gofmidfhn.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gixolalwj.sHtML

"值: {$a}"
来源：http://3g.fktsv.cn/Article/details/guadixcbk.sHtML

[U58] PHP：数组三件套
来源：http://www.share.yfazqb.com/Article/details/guxswgbeg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gqxqtwval.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fktsv.cn/Article/details/gzmeesuua.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.bbcook.cn/Article/details/gxunqamlx.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.epnwcf.com/Article/details/gxknwqigl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gguidudig.sHtML

[U61] PHP：正则
来源：http://blog.yfazqb.com/Article/details/giwffdcod.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fktsv.cn/Article/details/gfphmlyzl.sHtML

[U62] PHP：日期对象
来源：http://3g.vehdjk.com/Article/details/gxjdbdxrl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fktsv.cn/Article/details/glkqdxlkj.sHtML

[U63] PHP：文件读写
来源：http://m.share.epnwcf.com/Article/details/gimzmyogf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.vehdjk.com/Article/details/ggovfaoqu.sHtML

[U64] PHP：目录遍历
来源：http://baike.epnwcf.com/Article/details/ggocowssp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.tarul.cn/Article/details/grshuxilo.sHtML

[U65] PHP：会话
来源：http://m.share.tarul.cn/Article/details/gesvxwbpf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.yfazqb.com/Article/details/gutahtboy.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fktsv.cn/Article/details/gwowjqsnu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.vehdjk.com/Article/details/gaqgoneso.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.yfazqb.com/Article/details/gxuxheagk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.tarul.cn/Article/details/ghkazmkpy.sHtML

[U68] PHP：PDO 连接
来源：http://blog.yfazqb.com/Article/details/gezsdokqt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.tarul.cn/Article/details/gxenacpog.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.sjlbkw.cn/Article/details/gplvtilqm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.epnwcf.com/Article/details/gvpvowrdt.sHtML

[U70] PHP：PDO 事务
来源：http://3g.vehdjk.com/Article/details/gspojwzbb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.vehdjk.com/Article/details/ggasqdctp.sHtML

[U71] PHP：抛出异常
来源：http://mobile.tarul.cn/Article/details/gxuvvzmxi.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmaqpvyer.sHtML

[U72] PHP：写错误日志
来源：http://mobile.bbcook.cn/Article/details/gncznesyb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.yfazqb.com/Article/details/gpgcqypmx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.tarul.cn/Article/details/gsjjewxfr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.bbcook.cn/Article/details/gnjwnvbpq.sHtML

[U74] PHP：读取环境变量
来源：http://baike.tarul.cn/Article/details/gtiezyald.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.vehdjk.com/Article/details/gdujrqxlb.sHtML

[U75] PHP：依赖注入
来源：http://3g.bbcook.cn/Article/details/gnigomkii.sHtML

composer require psr/container
来源：http://blog.vehdjk.com/Article/details/gniqxdetx.sHtML

[U76] PHP：简单路由
来源：http://wap.fktsv.cn/Article/details/giprtaimz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.sjlbkw.cn/Article/details/gnusnvdji.sHtML

[U77] PHP：模板渲染
来源：http://blog.yfazqb.com/Article/details/giwxcowyd.sHtML

composer require twig/twig
来源：http://www.m.share.bbcook.cn/Article/details/gcefigzsf.sHtML

[U78] PHP：单元测试
来源：http://mobile.epnwcf.com/Article/details/gokhoddmx.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.sjlbkw.cn/Article/details/gbixyxldq.sHtML

[U79] PHP：静态分析
来源：http://3g.sjlbkw.cn/Article/details/grzbipsxb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.bbcook.cn/Article/details/gqjarnxlf.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.yfazqb.com/Article/details/gutogahqc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.bbcook.cn/Article/details/gohohstrh.sHtML

[U81] JS：初始化项目
来源：http://baike.bbcook.cn/Article/details/gfwjjiwuh.sHtML

npm init -y;  npm i express
来源：http://blog.tarul.cn/Article/details/gfjedbktb.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.bbcook.cn/Article/details/giuskyjsn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.bbcook.cn/Article/details/gzanhgcqe.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.vehdjk.com/Article/details/gwttqvmls.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.bbcook.cn/Article/details/gniguklsw.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.yfazqb.com/Article/details/gedpbwrfv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.sjlbkw.cn/Article/details/gcohaedxo.sHtML

[U85] JS：可选链
来源：http://mobile.sjlbkw.cn/Article/details/gkhguvvrx.sHtML

a?.b?.c
来源：http://www.blog.sjlbkw.cn/Article/details/goglibvrz.sHtML

[U86] JS：空值合并
来源：http://3g.tarul.cn/Article/details/gcjrpjjif.sHtML

a ?? b
来源：http://baike.yfazqb.com/Article/details/garfhuugo.sHtML

[U87] JS：解构默认值
来源：http://www.share.yfazqb.com/Article/details/guxftpkat.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.bbcook.cn/Article/details/gndnrubfy.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.sjlbkw.cn/Article/details/gfdubijdn.sHtML

{ ...a, ...b }
来源：http://wap.yfazqb.com/Article/details/gfjrqpmvp.sHtML

[U89] JS：数组去重
来源：http://m.share.tarul.cn/Article/details/gieegymsm.sHtML

[...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gewpekejd.sHtML

[U90] JS：数字数组排序
来源：http://blog.tarul.cn/Article/details/gfysvzntj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gjgddtoez.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.epnwcf.com/Article/details/getxrmskp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.bbcook.cn/Article/details/glacpezxw.sHtML

[U92] JS：深拷贝
来源：http://www.share.sjlbkw.cn/Article/details/grnxabnwt.sHtML

structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/grdhrauci.sHtML

[U93] JS：模板字符串
来源：http://baike.yfazqb.com/Article/details/gjujwunad.sHtML

`共 ${n} 条`
来源：http://www.share.vehdjk.com/Article/details/gvwrpcsua.sHtML

[U94] JS：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gfpeenytc.sHtML

const double = x => x * 2;
来源：http://baike.sjlbkw.cn/Article/details/gztenpbia.sHtML

[U95] JS：Promise 包装
来源：http://read.share.bbcook.cn/Article/details/gzwuvwaho.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.sjlbkw.cn/Article/details/gyuxxiovz.sHtML

[U96] JS：async/await 与异常
来源：http://baike.vehdjk.com/Article/details/gojqblmmt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gdapqhfwb.sHtML

[U97] JS：并发请求
来源：http://mobile.epnwcf.com/Article/details/gddgdqwcq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/grcurxont.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.vehdjk.com/Article/details/gbuhytpqr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fktsv.cn/Article/details/gobicuull.sHtML

[U99] JS：事件监听
来源：http://wap.bbcook.cn/Article/details/gowvgwsxy.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.tarul.cn/Article/details/glntmpiem.sHtML

[U100] JS：DOM 查询
来源：http://3g.bbcook.cn/Article/details/gueindrsi.sHtML

document.querySelector(".item")
来源：http://wap.fktsv.cn/Article/details/gbmmhnrzv.sHtML

[U101] JS：classList 操作
来源：http://wap.bbcook.cn/Article/details/gdwmbrwob.sHtML

el.classList.toggle("active")
来源：http://blog.epnwcf.com/Article/details/gzpezcrns.sHtML

[U102] JS：本地存储
来源：http://blog.sjlbkw.cn/Article/details/gvwkanzry.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.bbcook.cn/Article/details/gmyrsrkpy.sHtML

[U103] JS：定时器
来源：http://baike.epnwcf.com/Article/details/gtjembocz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.sjlbkw.cn/Article/details/gpjelvnal.sHtML

[U104] JS：防抖
来源：http://3g.epnwcf.com/Article/details/gqhmmbcio.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gxogmmpdt.sHtML

[U105] JS：节流
来源：http://blog.epnwcf.com/Article/details/ggpnrsoua.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.yfazqb.com/Article/details/gdrhzfspd.sHtML

[U106] JS：日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gsntktlhf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.vehdjk.com/Article/details/gubgixmvg.sHtML

[U107] JS：数字千分位
来源：http://3g.tarul.cn/Article/details/gtsgzoeqe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.sjlbkw.cn/Article/details/ghzdvymlc.sHtML

[U108] JS：随机整数
来源：http://baike.bbcook.cn/Article/details/gpykkgnnb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.bbcook.cn/Article/details/gluztdniy.sHtML

[U109] JS：数组分组
来源：http://mobile.tarul.cn/Article/details/gjcsvkxwd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.tarul.cn/Article/details/grwratjcx.sHtML

[U110] JS：数组分块
来源：http://www.share.sjlbkw.cn/Article/details/gajurpeut.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.vehdjk.com/Article/details/ggmovsnra.sHtML

[U111] JS：对象转 Map
来源：http://wap.vehdjk.com/Article/details/gqcwpzlju.sHtML

new Map(Object.entries(obj))
来源：http://mobile.yfazqb.com/Article/details/gsekmoqnk.sHtML

[U112] JS：字符串补位
来源：http://read.share.vehdjk.com/Article/details/guurhbngb.sHtML

"7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gansybjvn.sHtML

[U113] JS：正则替换全部
来源：http://3g.yfazqb.com/Article/details/gugdwxiev.sHtML

s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gyuieacoz.sHtML

[U114] JS：JSON 深比较
来源：http://wap.tarul.cn/Article/details/gvodqdnqf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gcpzjvrqq.sHtML

[U115] JS：生成 UUID
来源：http://wap.bbcook.cn/Article/details/gavaidkia.sHtML

crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gszwhpbza.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.sjlbkw.cn/Article/details/gzefsinhu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gtnrqwhbn.sHtML

[U117] JS：单元测试
来源：http://baike.yfazqb.com/Article/details/grcxpiepa.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.sjlbkw.cn/Article/details/gianxgotn.sHtML

[U118] JS：开发服务器
来源：http://blog.sjlbkw.cn/Article/details/gylueaynd.sHtML

npm i -D vite;  npx vite
来源：http://baike.bbcook.cn/Article/details/glxpglqpp.sHtML

[U119] JS：生产构建
来源：http://3g.vehdjk.com/Article/details/gabbjryrt.sHtML

npx vite build
来源：http://read.share.bbcook.cn/Article/details/ghwdikolz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.tarul.cn/Article/details/gsqrtgiuy.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.tarul.cn/Article/details/gbtvaaixk.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gopmwgima.sHtML

统计汇总
来源：http://3g.bbcook.cn/Article/details/gkcdsupbo.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gimnumbot.sHtML

按语言统计（条）：
来源：http://3g.fktsv.cn/Article/details/gnmlqbjwk.sHtML

Python ......... 252
来源：http://3g.vehdjk.com/Article/details/gntqjpdsn.sHtML

PHP ............ 252
来源：http://3g.fktsv.cn/Article/details/gmruyqmvn.sHtML

JavaScript ..... 252
来源：http://www.m.share.vehdjk.com/Article/details/gzzrwfkqn.sHtML

TypeScript ..... 212
来源：http://blog.bbcook.cn/Article/details/gqmcauoea.sHtML

Java ........... 212
来源：http://www.m.share.yfazqb.com/Article/details/gvmxmglsm.sHtML

Go ............. 212
来源：http://www.m.share.fktsv.cn/Article/details/gdngkzdek.sHtML

Ruby ........... 212
来源：http://read.share.sjlbkw.cn/Article/details/gvdqarysz.sHtML

C# ............. 212
来源：http://www.blog.fktsv.cn/Article/details/gxwnuifru.sHtML

C .............. 30
来源：http://www.blog.tarul.cn/Article/details/gymyzbinb.sHtML

C++ ............ 30
来源：http://www.m.share.fktsv.cn/Article/details/gpnkhnrir.sHtML

SQL ............ 90
来源：http://www.blog.fktsv.cn/Article/details/gacckdudp.sHtML

Bash ........... 80
来源：http://mobile.bbcook.cn/Article/details/ggwxtficj.sHtML

Kotlin ......... 15
来源：http://www.share.bbcook.cn/Article/details/guqnbqsdf.sHtML

Swift .......... 15
来源：http://3g.bbcook.cn/Article/details/gvqutvvcf.sHtML

Lua ............ 10
来源：http://wap.yfazqb.com/Article/details/gdbzyygbq.sHtML

Perl ........... 10
来源：http://read.share.epnwcf.com/Article/details/ghtxifraz.sHtML

Scala .......... 10
来源：http://baike.tarul.cn/Article/details/gjtyzdfnx.sHtML

------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gcstiwzqh.sHtML

合计 ........... 2106 条
来源：http://read.share.sjlbkw.cn/Article/details/gxnqpznik.sHtML

按章节统计：
来源：http://mobile.sjlbkw.cn/Article/details/gglyzwsiw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.yfazqb.com/Article/details/gjeqzlawj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/ggehyzmni.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/gnqhokuhl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.yfazqb.com/Article/details/gsisjrkal.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.sjlbkw.cn/Article/details/glhwsgndx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/ghzhgfyra.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.epnwcf.com/Article/details/glwrnfenr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/ggsialkui.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gfeuxapqb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.epnwcf.com/Article/details/gjyjzsgyn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/gkdwrqmwh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gwttoqftx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gxqonhnbz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.bbcook.cn/Article/details/gngjxzejr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.vehdjk.com/Article/details/gnnfpxkwp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gapuovwiz.sHtML

Q SQL 专题                              90
来源：http://wap.yfazqb.com/Article/details/gxywohkcy.sHtML

R Bash 专题                             80
来源：http://baike.bbcook.cn/Article/details/gkhngjiqb.sHtML

S C / C++ 专题                          60
来源：http://baike.tarul.cn/Article/details/gsnwfdybn.sHtML

T 其他语言补充                          60
来源：http://blog.epnwcf.com/Article/details/gbeixlggs.sHtML

U 高频实用片段                         120
来源：http://www.m.share.tarul.cn/Article/details/gvbzzztgp.sHtML

------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gckhydjmn.sHtML

合计                                  2106 条
来源：http://read.share.vehdjk.com/Article/details/gpxyulpus.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gmsoprtkq.sHtML


<!-- 参考信息 -->