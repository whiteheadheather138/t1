代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://3g.sjlbkw.cn/Article/details/gpyyuxiij.sHtML

[T59] Scala：循环
来源：http://3g.sjlbkw.cn/Article/details/gnglpxxca.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.yfazqb.com/Article/details/gandwwigu.sHtML

[T60] Scala：折叠
来源：http://www.m.share.tarul.cn/Article/details/gzhzvbszk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/ggeljhzsd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwxalojvm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/gaveqpkei.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grdbzawas.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.bbcook.cn/Article/details/gthqduusn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.sjlbkw.cn/Article/details/gtgliqxow.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.tarul.cn/Article/details/gmgbnbwfg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fktsv.cn/Article/details/gzzidjpow.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.sjlbkw.cn/Article/details/gekdhbgti.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gozyzmlhm.sHtML

[U04] Py：变量调试打印
来源：http://baike.tarul.cn/Article/details/gejwymuqt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.yfazqb.com/Article/details/gpkieagjl.sHtML

[U05] Py：列表去重且保序
来源：http://baike.epnwcf.com/Article/details/gqiawjojy.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gsaqkriwu.sHtML

[U06] Py：合并两个字典
来源：http://wap.vehdjk.com/Article/details/gnfijgfeh.sHtML

{**a, **b}
来源：http://mobile.tarul.cn/Article/details/gjqqogdzy.sHtML

[U07] Py：反转字典键值
来源：http://read.share.vehdjk.com/Article/details/ghhtepzcm.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.yfazqb.com/Article/details/gwdrvywau.sHtML

[U08] Py：展平二维列表
来源：http://blog.bbcook.cn/Article/details/gflylbgzf.sHtML

[y for x in nested for y in x]
来源：http://wap.fktsv.cn/Article/details/ggjisbmjr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.bbcook.cn/Article/details/gxvswvvip.sHtML

max(d, key=d.get)
来源：http://3g.fktsv.cn/Article/details/gqnaydrlv.sHtML

[U10] Py：按值排序字典
来源：http://mobile.sjlbkw.cn/Article/details/gukspcfwj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.yfazqb.com/Article/details/gmmnfopuh.sHtML

[U11] Py：生成器表达式
来源：http://read.share.bbcook.cn/Article/details/ggmlrdtvk.sHtML

(x * 2 for x in arr)
来源：http://read.share.sjlbkw.cn/Article/details/gkydktbba.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.yfazqb.com/Article/details/gfyihgbnk.sHtML

Counter(arr).most_common(3)
来源：http://www.share.epnwcf.com/Article/details/gwjunygtf.sHtML

[U13] Py：固定长度队列
来源：http://wap.tarul.cn/Article/details/gtjshahvy.sHtML

deque(maxlen=10)
来源：http://wap.epnwcf.com/Article/details/gqmsvsuda.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.sjlbkw.cn/Article/details/godmyczpt.sHtML

defaultdict(list)
来源：http://read.share.sjlbkw.cn/Article/details/gnxaukjzo.sHtML

[U15] Py：高精度计时
来源：http://mobile.vehdjk.com/Article/details/geflhhurg.sHtML

t = time.perf_counter()
来源：http://mobile.vehdjk.com/Article/details/gvwptfyhu.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.yfazqb.com/Article/details/gvdmjzbim.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.yfazqb.com/Article/details/gaucfuwgg.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.vehdjk.com/Article/details/gsyhbqokf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.vehdjk.com/Article/details/gkrxldfow.sHtML

[U18] Py：预编译正则
来源：http://3g.vehdjk.com/Article/details/gicdjzhct.sHtML

pat = re.compile(r"\d+")
来源：http://baike.vehdjk.com/Article/details/gqzbswgbu.sHtML

[U19] Py：正则替换带回调
来源：http://blog.yfazqb.com/Article/details/gkudgmcxi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.epnwcf.com/Article/details/gokwercei.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fktsv.cn/Article/details/gabgazzau.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.epnwcf.com/Article/details/gtgsvyuuz.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.tarul.cn/Article/details/gbprvkllo.sHtML

@contextlib.contextmanager
来源：http://www.blog.sjlbkw.cn/Article/details/gwvpaizmp.sHtML

[U22] Py：矩阵转置
来源：http://3g.sjlbkw.cn/Article/details/gwnkeytbk.sHtML

list(zip(*m))
来源：http://wap.sjlbkw.cn/Article/details/gmnvldeur.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.sjlbkw.cn/Article/details/gjfkgcusb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.vehdjk.com/Article/details/gakfaabgr.sHtML

[U24] Py：路径操作
来源：http://mobile.epnwcf.com/Article/details/gyietbhmj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gtwvnaoou.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fktsv.cn/Article/details/guncvqtlx.sHtML

csv.DictReader(f)
来源：http://m.share.epnwcf.com/Article/details/ghecegtpj.sHtML

[U26] Py：并发下载
来源：http://3g.vehdjk.com/Article/details/ggxpatvgv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.vehdjk.com/Article/details/gmvemilor.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.epnwcf.com/Article/details/gsmkldqnd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fktsv.cn/Article/details/gicdxygkk.sHtML

[U28] Py：类型别名
来源：http://www.blog.fktsv.cn/Article/details/ggagvaoca.sHtML

UserId = int
来源：http://m.share.sjlbkw.cn/Article/details/gbdjsgerg.sHtML

[U29] Py：属性校验
来源：http://www.m.share.epnwcf.com/Article/details/glohhnynm.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.epnwcf.com/Article/details/ghbmhrytp.sHtML

[U30] Py：数据类
来源：http://blog.tarul.cn/Article/details/gfgckpgds.sHtML

@dataclass(slots=True)
来源：http://3g.epnwcf.com/Article/details/gcaegwbwz.sHtML

[U31] Py：单测
来源：http://www.share.vehdjk.com/Article/details/gcohnfjfv.sHtML

python -m pytest -q
来源：http://read.share.bbcook.cn/Article/details/gfcppnbhy.sHtML

[U32] Py：代码格式化
来源：http://mobile.sjlbkw.cn/Article/details/gxpcvzzof.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.bbcook.cn/Article/details/gbbnsyjho.sHtML

[U33] Py：打包发布
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfufpctl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fktsv.cn/Article/details/giaztdjip.sHtML

[U34] Py：判断编码
来源：http://3g.sjlbkw.cn/Article/details/gkkadtbfl.sHtML

chardet.detect(raw)
来源：http://www.m.share.epnwcf.com/Article/details/grjnutxvc.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.vehdjk.com/Article/details/gfeaxirkh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.tarul.cn/Article/details/gfssglyun.sHtML

[U36] Py：定时任务
来源：http://www.blog.tarul.cn/Article/details/gmxtqxzlf.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.bbcook.cn/Article/details/gjqxpjklr.sHtML

[U37] Py：读写 Excel
来源：http://3g.tarul.cn/Article/details/gvfeqdvzq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fktsv.cn/Article/details/gaaxzaekf.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.sjlbkw.cn/Article/details/ghuepvrsw.sHtML

Path(__file__).resolve().parent
来源：http://m.share.yfazqb.com/Article/details/guvntepnd.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.epnwcf.com/Article/details/gnmnqqegu.sHtML

sys.stdout.isatty()
来源：http://mobile.tarul.cn/Article/details/gqmobebqm.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.epnwcf.com/Article/details/gzrziobar.sHtML

print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/gfnjadqqs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fktsv.cn/Article/details/gedecpntg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.tarul.cn/Article/details/gpraiaouy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.vehdjk.com/Article/details/gzyrpnfxp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.yfazqb.com/Article/details/glpzhyyiz.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.yfazqb.com/Article/details/grxulvfok.sHtML

namespace App\Http;
来源：http://3g.bbcook.cn/Article/details/gshhdlxhd.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.bbcook.cn/Article/details/gdvrxtegj.sHtML

declare(strict_types=1);
来源：http://blog.vehdjk.com/Article/details/gimcetqgs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.tarul.cn/Article/details/gfmjntrab.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gzwekwddn.sHtML

[U46] PHP：可空类型
来源：http://blog.epnwcf.com/Article/details/gnogqznms.sHtML

?string $name = null
来源：http://wap.sjlbkw.cn/Article/details/gfaxjfzyy.sHtML

[U47] PHP：联合类型
来源：http://mobile.fktsv.cn/Article/details/ghuwrutov.sHtML

int|string $id
来源：http://www.share.tarul.cn/Article/details/gkhyfgiix.sHtML

[U48] PHP：纯枚举
来源：http://wap.tarul.cn/Article/details/gwoabodst.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.epnwcf.com/Article/details/guxjbbvhj.sHtML

[U49] PHP：只读属性
来源：http://read.share.epnwcf.com/Article/details/gtuqlnrbj.sHtML

public readonly string $name
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzqxkzrz.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.tarul.cn/Article/details/gdpnavold.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.vehdjk.com/Article/details/grdjuhmje.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fktsv.cn/Article/details/gpmcwvqrn.sHtML

[$a, $b] = $arr;
来源：http://read.share.yfazqb.com/Article/details/gvdfepicw.sHtML

[U52] PHP：箭头函数
来源：http://3g.vehdjk.com/Article/details/gknkpphzd.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.epnwcf.com/Article/details/ghnxfudbg.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fktsv.cn/Article/details/gkybedeal.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.sjlbkw.cn/Article/details/goqpqskxt.sHtML

[U54] PHP：空安全调用
来源：http://wap.fktsv.cn/Article/details/gdlilcuif.sHtML

$obj?->method()
来源：http://mobile.yfazqb.com/Article/details/gbcepegsi.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmhvwhej.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.vehdjk.com/Article/details/gdddpsaor.sHtML

[U56] PHP：命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gitupjdfn.sHtML

f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gmbiwusrk.sHtML

[U57] PHP：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/ghqvdmkbi.sHtML

"值: {$a}"
来源：http://3g.sjlbkw.cn/Article/details/gndquucjt.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fktsv.cn/Article/details/gbvwuhlag.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.yfazqb.com/Article/details/gvuzlizeu.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fktsv.cn/Article/details/grsnibpmo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.sjlbkw.cn/Article/details/guvzjzxum.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.yfazqb.com/Article/details/gknzxbaes.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fktsv.cn/Article/details/gcoldrpdl.sHtML

[U61] PHP：正则
来源：http://baike.sjlbkw.cn/Article/details/gezceypgn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gbavitlqe.sHtML

[U62] PHP：日期对象
来源：http://wap.sjlbkw.cn/Article/details/gydyeixic.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.bbcook.cn/Article/details/gczogpbtd.sHtML

[U63] PHP：文件读写
来源：http://baike.sjlbkw.cn/Article/details/gjupxdtjt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fktsv.cn/Article/details/gpomwijvh.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.tarul.cn/Article/details/glkdhuply.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.yfazqb.com/Article/details/gfmjqtrwn.sHtML

[U65] PHP：会话
来源：http://m.share.epnwcf.com/Article/details/guwbirvkh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gzyvmlsey.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.bbcook.cn/Article/details/gegxolbqg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.yfazqb.com/Article/details/gjvfxcmnr.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.yfazqb.com/Article/details/gcgraqddp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.vehdjk.com/Article/details/ggdqijumt.sHtML

[U68] PHP：PDO 连接
来源：http://wap.tarul.cn/Article/details/gubbogirh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.bbcook.cn/Article/details/gsmaumuxk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.vehdjk.com/Article/details/gvnnczohf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.yfazqb.com/Article/details/gqvxoplqs.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.bbcook.cn/Article/details/gqzmercgi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.epnwcf.com/Article/details/gxslywstj.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/gwzmztyvd.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.vehdjk.com/Article/details/gmwmklkzj.sHtML

[U72] PHP：写错误日志
来源：http://wap.vehdjk.com/Article/details/gtoacoaqw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fktsv.cn/Article/details/gjwimtsgj.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.vehdjk.com/Article/details/gkscclfwq.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fktsv.cn/Article/details/geitqflwi.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.yfazqb.com/Article/details/gausuxxed.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.bbcook.cn/Article/details/gmulwhucg.sHtML

[U75] PHP：依赖注入
来源：http://blog.epnwcf.com/Article/details/gbjocpzvy.sHtML

composer require psr/container
来源：http://wap.bbcook.cn/Article/details/gkhbwfxtf.sHtML

[U76] PHP：简单路由
来源：http://3g.vehdjk.com/Article/details/gvzxwykjf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fktsv.cn/Article/details/gkhdhhwdx.sHtML

[U77] PHP：模板渲染
来源：http://m.share.tarul.cn/Article/details/gbfdacmks.sHtML

composer require twig/twig
来源：http://wap.fktsv.cn/Article/details/gdmccskqk.sHtML

[U78] PHP：单元测试
来源：http://www.share.epnwcf.com/Article/details/gnnrlsigg.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.yfazqb.com/Article/details/gjwyatips.sHtML

[U79] PHP：静态分析
来源：http://3g.vehdjk.com/Article/details/gcliucmra.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.bbcook.cn/Article/details/gcwqvqhnd.sHtML

[U80] PHP：代码规范修复
来源：http://blog.tarul.cn/Article/details/guqouwgce.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fktsv.cn/Article/details/gpvdnqetf.sHtML

[U81] JS：初始化项目
来源：http://www.share.sjlbkw.cn/Article/details/gchtsknuh.sHtML

npm init -y;  npm i express
来源：http://baike.sjlbkw.cn/Article/details/gwtemqpiz.sHtML

[U82] JS：package.json 脚本
来源：http://wap.tarul.cn/Article/details/gvtuydnfl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.bbcook.cn/Article/details/gcuqyibvm.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.bbcook.cn/Article/details/gdenlufhp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.yfazqb.com/Article/details/guaikinbs.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.yfazqb.com/Article/details/gwtcekiac.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fktsv.cn/Article/details/guyvucovm.sHtML

[U85] JS：可选链
来源：http://www.share.sjlbkw.cn/Article/details/gspqnrkbz.sHtML

a?.b?.c
来源：http://wap.vehdjk.com/Article/details/gucgnqugf.sHtML

[U86] JS：空值合并
来源：http://blog.fktsv.cn/Article/details/gpnywfgkr.sHtML

a ?? b
来源：http://m.share.sjlbkw.cn/Article/details/ggxzjzwno.sHtML

[U87] JS：解构默认值
来源：http://3g.vehdjk.com/Article/details/gulilgehm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.yfazqb.com/Article/details/gockmghyq.sHtML

[U88] JS：对象展开合并
来源：http://read.share.tarul.cn/Article/details/gsnnghdrd.sHtML

{ ...a, ...b }
来源：http://wap.bbcook.cn/Article/details/gaxyxjbhp.sHtML

[U89] JS：数组去重
来源：http://wap.bbcook.cn/Article/details/gnajonayo.sHtML

[...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/grlarefot.sHtML

[U90] JS：数字数组排序
来源：http://wap.bbcook.cn/Article/details/glerzvexv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gmktdwdgd.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.yfazqb.com/Article/details/gvlrnpbfp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.tarul.cn/Article/details/gvcajokph.sHtML

[U92] JS：深拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gragdfwew.sHtML

structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gmkbrwzmp.sHtML

[U93] JS：模板字符串
来源：http://m.share.fktsv.cn/Article/details/gvfpskkxv.sHtML

`共 ${n} 条`
来源：http://3g.yfazqb.com/Article/details/guytlltcx.sHtML

[U94] JS：箭头函数
来源：http://baike.epnwcf.com/Article/details/gvpbbebxf.sHtML

const double = x => x * 2;
来源：http://www.share.epnwcf.com/Article/details/gdewywczw.sHtML

[U95] JS：Promise 包装
来源：http://baike.yfazqb.com/Article/details/ghnrcsjjt.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.epnwcf.com/Article/details/gmptzpkme.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.tarul.cn/Article/details/gxgumfleo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gwlwdkpkv.sHtML

[U97] JS：并发请求
来源：http://mobile.vehdjk.com/Article/details/gonhctdxr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/gyvxjzbgu.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.epnwcf.com/Article/details/gwndqmmbj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fktsv.cn/Article/details/gsycmtsef.sHtML

[U99] JS：事件监听
来源：http://www.blog.sjlbkw.cn/Article/details/ggukjibhn.sHtML

el.addEventListener("click", e => {})
来源：http://baike.tarul.cn/Article/details/guftrzouc.sHtML

[U100] JS：DOM 查询
来源：http://m.share.yfazqb.com/Article/details/gnhdctstj.sHtML

document.querySelector(".item")
来源：http://baike.fktsv.cn/Article/details/ghnydgwvw.sHtML

[U101] JS：classList 操作
来源：http://m.share.yfazqb.com/Article/details/geloryoqd.sHtML

el.classList.toggle("active")
来源：http://mobile.yfazqb.com/Article/details/gijzqsuoo.sHtML

[U102] JS：本地存储
来源：http://www.m.share.tarul.cn/Article/details/gqkpoatdj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.epnwcf.com/Article/details/giobodpoj.sHtML

[U103] JS：定时器
来源：http://m.share.epnwcf.com/Article/details/gtliwfvwk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.yfazqb.com/Article/details/ggvsknbmv.sHtML

[U104] JS：防抖
来源：http://baike.yfazqb.com/Article/details/gzntrmsmz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/gozkvvvgy.sHtML

[U105] JS：节流
来源：http://www.share.sjlbkw.cn/Article/details/glkjmoabi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.epnwcf.com/Article/details/gjbuyogxu.sHtML

[U106] JS：日期格式化
来源：http://blog.epnwcf.com/Article/details/ghkrufipv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.yfazqb.com/Article/details/gnduqmpdj.sHtML

[U107] JS：数字千分位
来源：http://wap.bbcook.cn/Article/details/gbscjllxn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.yfazqb.com/Article/details/gmjvytfcz.sHtML

[U108] JS：随机整数
来源：http://www.m.share.yfazqb.com/Article/details/gudmypjul.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fktsv.cn/Article/details/ghqcseapa.sHtML

[U109] JS：数组分组
来源：http://www.blog.tarul.cn/Article/details/gjolxxsut.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.tarul.cn/Article/details/gthzyxova.sHtML

[U110] JS：数组分块
来源：http://m.share.tarul.cn/Article/details/gbuggyeld.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.yfazqb.com/Article/details/ghyaeweaq.sHtML

[U111] JS：对象转 Map
来源：http://m.share.tarul.cn/Article/details/gpuhhdtni.sHtML

new Map(Object.entries(obj))
来源：http://baike.sjlbkw.cn/Article/details/gesljsfju.sHtML

[U112] JS：字符串补位
来源：http://wap.vehdjk.com/Article/details/gcwwyitnu.sHtML

"7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gkakfvfhk.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fktsv.cn/Article/details/gsfqlewtu.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gugwkyyyf.sHtML

[U114] JS：JSON 深比较
来源：http://3g.sjlbkw.cn/Article/details/gfohommfk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.epnwcf.com/Article/details/guehnlgcn.sHtML

[U115] JS：生成 UUID
来源：http://m.share.vehdjk.com/Article/details/gayeldalg.sHtML

crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gknhwzjmq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fktsv.cn/Article/details/gnicgrahg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.bbcook.cn/Article/details/guugndccn.sHtML

[U117] JS：单元测试
来源：http://m.share.bbcook.cn/Article/details/gotfecixc.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.yfazqb.com/Article/details/gpxwtmhxr.sHtML

[U118] JS：开发服务器
来源：http://3g.fktsv.cn/Article/details/gfcyiqdgn.sHtML

npm i -D vite;  npx vite
来源：http://wap.bbcook.cn/Article/details/gnqquzrzj.sHtML

[U119] JS：生产构建
来源：http://wap.yfazqb.com/Article/details/grcmdzgxg.sHtML

npx vite build
来源：http://www.m.share.yfazqb.com/Article/details/gnipvzrzf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.epnwcf.com/Article/details/gqpwzoyli.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fktsv.cn/Article/details/gewbrycpu.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/glqtiwmmp.sHtML

统计汇总
来源：http://wap.vehdjk.com/Article/details/gyqihbnrd.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gryzuillq.sHtML

按语言统计（条）：
来源：http://www.m.share.bbcook.cn/Article/details/gzmqryluw.sHtML

Python ......... 252
来源：http://baike.tarul.cn/Article/details/gokimmjgi.sHtML

PHP ............ 252
来源：http://read.share.tarul.cn/Article/details/gnsnqvhjm.sHtML

JavaScript ..... 252
来源：http://www.m.share.fktsv.cn/Article/details/gwmudldcx.sHtML

TypeScript ..... 212
来源：http://blog.fktsv.cn/Article/details/geefuacss.sHtML

Java ........... 212
来源：http://baike.bbcook.cn/Article/details/giclnxjgz.sHtML

Go ............. 212
来源：http://read.share.yfazqb.com/Article/details/gnjzmzoju.sHtML

Ruby ........... 212
来源：http://www.blog.bbcook.cn/Article/details/gjixpkbzl.sHtML

C# ............. 212
来源：http://www.m.share.bbcook.cn/Article/details/gghltnxjm.sHtML

C .............. 30
来源：http://read.share.epnwcf.com/Article/details/gjeopybhz.sHtML

C++ ............ 30
来源：http://3g.sjlbkw.cn/Article/details/gggceccyk.sHtML

SQL ............ 90
来源：http://baike.vehdjk.com/Article/details/gytvszgns.sHtML

Bash ........... 80
来源：http://3g.epnwcf.com/Article/details/gtntknxvu.sHtML

Kotlin ......... 15
来源：http://www.m.share.tarul.cn/Article/details/gtxhivdcu.sHtML

Swift .......... 15
来源：http://read.share.tarul.cn/Article/details/gzzuqdwrb.sHtML

Lua ............ 10
来源：http://m.share.epnwcf.com/Article/details/gcoojbptz.sHtML

Perl ........... 10
来源：http://baike.bbcook.cn/Article/details/gjfscscyq.sHtML

Scala .......... 10
来源：http://m.share.fktsv.cn/Article/details/gitgogwry.sHtML

------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gatzbplnz.sHtML

合计 ........... 2106 条
来源：http://www.blog.sjlbkw.cn/Article/details/gmjgjzcnl.sHtML

按章节统计：
来源：http://blog.yfazqb.com/Article/details/gzobflemv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fktsv.cn/Article/details/gagrlpvxn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.epnwcf.com/Article/details/gnzttaumv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gdzgbvsmn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.vehdjk.com/Article/details/gyigilnps.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fktsv.cn/Article/details/gkszmexnr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fktsv.cn/Article/details/gtunvqakv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gekvrydit.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.yfazqb.com/Article/details/gfqxkgwci.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gvyfutyew.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.vehdjk.com/Article/details/gzhyvzils.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gffgmhcjr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gsuzhdcot.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gxyyyrcug.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.tarul.cn/Article/details/gfovblszd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.sjlbkw.cn/Article/details/ggkqkluoz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gdsezlkoq.sHtML

Q SQL 专题                              90
来源：http://www.share.yfazqb.com/Article/details/gyjmrgzat.sHtML

R Bash 专题                             80
来源：http://wap.vehdjk.com/Article/details/gxruiqudt.sHtML

S C / C++ 专题                          60
来源：http://wap.bbcook.cn/Article/details/ghldzlrrl.sHtML

T 其他语言补充                          60
来源：http://www.share.tarul.cn/Article/details/giutdsnyc.sHtML

U 高频实用片段                         120
来源：http://baike.tarul.cn/Article/details/gvwpiwwuu.sHtML

------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/glxdbhlyz.sHtML

合计                                  2106 条
来源：http://www.m.share.epnwcf.com/Article/details/gxvsvrxvk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/gfiwhwpsm.sHtML

使用提醒
来源：http://m.share.fktsv.cn/Article/details/ghlexhlry.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gornqzmld.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.epnwcf.com/Article/details/gqkfgfvkz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.yfazqb.com/Article/details/gdeiaptwa.sHtML


<!-- 参考信息 -->