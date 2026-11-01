代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.epnwcf.com/Article/details/gubwvhdse.sHtML

[T59] Scala：循环
来源：http://www.share.tarul.cn/Article/details/grqewjjmw.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.vehdjk.com/Article/details/gbnoclfrj.sHtML

[T60] Scala：折叠
来源：http://mobile.tarul.cn/Article/details/gjzqolltl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.vehdjk.com/Article/details/gkbbnbmrq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/glysxjnft.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fktsv.cn/Article/details/gcuziehlz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghmdgflig.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.yfazqb.com/Article/details/guufyodfb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.vehdjk.com/Article/details/glxfugrog.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.yfazqb.com/Article/details/gatpnsgml.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.epnwcf.com/Article/details/geibfqxgs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.bbcook.cn/Article/details/gxyvilfnq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.yfazqb.com/Article/details/geljrayfl.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqgfeqer.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.tarul.cn/Article/details/gmunfutfh.sHtML

[U05] Py：列表去重且保序
来源：http://3g.epnwcf.com/Article/details/gcaxtcpkt.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gwmklnyse.sHtML

[U06] Py：合并两个字典
来源：http://www.share.yfazqb.com/Article/details/gthfvmvut.sHtML

{**a, **b}
来源：http://m.share.fktsv.cn/Article/details/gcketanjg.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gllaeqfnv.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.sjlbkw.cn/Article/details/ghnifajro.sHtML

[U08] Py：展平二维列表
来源：http://wap.vehdjk.com/Article/details/gkhavkeup.sHtML

[y for x in nested for y in x]
来源：http://www.blog.vehdjk.com/Article/details/gblpaftla.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.yfazqb.com/Article/details/gvoxxpscj.sHtML

max(d, key=d.get)
来源：http://www.m.share.sjlbkw.cn/Article/details/glrcfqbgs.sHtML

[U10] Py：按值排序字典
来源：http://mobile.epnwcf.com/Article/details/grmslnbhk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.vehdjk.com/Article/details/gchzreqfq.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.yfazqb.com/Article/details/gqgjgutpx.sHtML

(x * 2 for x in arr)
来源：http://m.share.fktsv.cn/Article/details/glbnqkolg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.epnwcf.com/Article/details/gjuygflzx.sHtML

Counter(arr).most_common(3)
来源：http://3g.fktsv.cn/Article/details/gfegrcgjl.sHtML

[U13] Py：固定长度队列
来源：http://baike.fktsv.cn/Article/details/gwokwdwng.sHtML

deque(maxlen=10)
来源：http://www.blog.fktsv.cn/Article/details/guqqtnlwh.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.bbcook.cn/Article/details/gdnkrdboc.sHtML

defaultdict(list)
来源：http://baike.bbcook.cn/Article/details/gqtofpbcw.sHtML

[U15] Py：高精度计时
来源：http://mobile.tarul.cn/Article/details/gcscxdhma.sHtML

t = time.perf_counter()
来源：http://read.share.yfazqb.com/Article/details/gsmmpwwbi.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.vehdjk.com/Article/details/guucafndo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.vehdjk.com/Article/details/gvuqnhsrf.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.yfazqb.com/Article/details/glkrkevtf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.tarul.cn/Article/details/gjiokmjeb.sHtML

[U18] Py：预编译正则
来源：http://www.blog.tarul.cn/Article/details/gqopysxpw.sHtML

pat = re.compile(r"\d+")
来源：http://wap.yfazqb.com/Article/details/gaonppjly.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.vehdjk.com/Article/details/glakhwoni.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.sjlbkw.cn/Article/details/gsuiburlu.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fktsv.cn/Article/details/ghonibrpd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.vehdjk.com/Article/details/gxnmfymug.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.tarul.cn/Article/details/ggvzrtnjy.sHtML

@contextlib.contextmanager
来源：http://3g.epnwcf.com/Article/details/ghkxysgjo.sHtML

[U22] Py：矩阵转置
来源：http://blog.sjlbkw.cn/Article/details/gcgvttpho.sHtML

list(zip(*m))
来源：http://baike.epnwcf.com/Article/details/gpmapnnuj.sHtML

[U23] Py：分块读取大文件
来源：http://3g.bbcook.cn/Article/details/gltaglzax.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.tarul.cn/Article/details/gdfbmbvxn.sHtML

[U24] Py：路径操作
来源：http://blog.vehdjk.com/Article/details/gxrpitbjb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gtlzwluuo.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.epnwcf.com/Article/details/gaxfcmozo.sHtML

csv.DictReader(f)
来源：http://baike.sjlbkw.cn/Article/details/gfondrqpp.sHtML

[U26] Py：并发下载
来源：http://wap.yfazqb.com/Article/details/gkvlzbezt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fktsv.cn/Article/details/gmnvaterd.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fktsv.cn/Article/details/gawiznnou.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.tarul.cn/Article/details/ggaalcocv.sHtML

[U28] Py：类型别名
来源：http://baike.yfazqb.com/Article/details/gmnchojqa.sHtML

UserId = int
来源：http://www.blog.tarul.cn/Article/details/gdprvqrjw.sHtML

[U29] Py：属性校验
来源：http://m.share.epnwcf.com/Article/details/guhnjxkhw.sHtML

@property 与 @x.setter 配合
来源：http://blog.sjlbkw.cn/Article/details/gylogltwy.sHtML

[U30] Py：数据类
来源：http://3g.tarul.cn/Article/details/gfgpmlvxt.sHtML

@dataclass(slots=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gnfeggjjh.sHtML

[U31] Py：单测
来源：http://www.m.share.fktsv.cn/Article/details/gfeoiedoq.sHtML

python -m pytest -q
来源：http://baike.sjlbkw.cn/Article/details/gbhszjusx.sHtML

[U32] Py：代码格式化
来源：http://blog.bbcook.cn/Article/details/gqhzdbaea.sHtML

ruff format . && ruff check --fix .
来源：http://wap.sjlbkw.cn/Article/details/grtzmthuu.sHtML

[U33] Py：打包发布
来源：http://read.share.epnwcf.com/Article/details/gajkfywwt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.epnwcf.com/Article/details/gnvpvmswi.sHtML

[U34] Py：判断编码
来源：http://wap.tarul.cn/Article/details/gflxyusgu.sHtML

chardet.detect(raw)
来源：http://www.blog.fktsv.cn/Article/details/guywajmbn.sHtML

[U35] Py：发送邮件
来源：http://3g.sjlbkw.cn/Article/details/gflzyyzlz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.vehdjk.com/Article/details/gwymenfnp.sHtML

[U36] Py：定时任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gumkvxjqs.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.tarul.cn/Article/details/ggwyvvuzm.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fktsv.cn/Article/details/gwqxfbgqa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.bbcook.cn/Article/details/guaxwhaid.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.tarul.cn/Article/details/glodqusga.sHtML

Path(__file__).resolve().parent
来源：http://mobile.yfazqb.com/Article/details/gpdfajqkv.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.bbcook.cn/Article/details/gpcahincu.sHtML

sys.stdout.isatty()
来源：http://3g.tarul.cn/Article/details/gpwcwhyca.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fktsv.cn/Article/details/gayqxwcvk.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gzbmendfy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.bbcook.cn/Article/details/glmmwdtcp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.sjlbkw.cn/Article/details/gowrmbeuh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.yfazqb.com/Article/details/gnpaqddur.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.sjlbkw.cn/Article/details/gghzujwjn.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.epnwcf.com/Article/details/ggayqbadl.sHtML

namespace App\Http;
来源：http://read.share.yfazqb.com/Article/details/gcjskqxhb.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.epnwcf.com/Article/details/gnftdsbys.sHtML

declare(strict_types=1);
来源：http://baike.tarul.cn/Article/details/gtuvykxvs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.vehdjk.com/Article/details/gilyjigju.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gazjpfcgy.sHtML

[U46] PHP：可空类型
来源：http://www.share.tarul.cn/Article/details/gjvrskluf.sHtML

?string $name = null
来源：http://www.m.share.epnwcf.com/Article/details/gmihfggcy.sHtML

[U47] PHP：联合类型
来源：http://www.blog.vehdjk.com/Article/details/gmumsvgxt.sHtML

int|string $id
来源：http://baike.fktsv.cn/Article/details/gckryjxyb.sHtML

[U48] PHP：纯枚举
来源：http://www.share.epnwcf.com/Article/details/gngysioza.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.vehdjk.com/Article/details/gyxhdryxq.sHtML

[U49] PHP：只读属性
来源：http://www.share.bbcook.cn/Article/details/gcsfoqawc.sHtML

public readonly string $name
来源：http://wap.yfazqb.com/Article/details/gaqfnlher.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.epnwcf.com/Article/details/gxmayehbt.sHtML

public function __construct(private int $id) {}
来源：http://www.share.vehdjk.com/Article/details/gpkkfwcrm.sHtML

[U51] PHP：数组解构
来源：http://blog.fktsv.cn/Article/details/geyjwxpcy.sHtML

[$a, $b] = $arr;
来源：http://3g.yfazqb.com/Article/details/gightttdk.sHtML

[U52] PHP：箭头函数
来源：http://read.share.sjlbkw.cn/Article/details/gruavifyo.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fktsv.cn/Article/details/govxqfzbe.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.bbcook.cn/Article/details/grqounykg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fktsv.cn/Article/details/gmzpytqgi.sHtML

[U54] PHP：空安全调用
来源：http://3g.bbcook.cn/Article/details/gtlafmjdt.sHtML

$obj?->method()
来源：http://3g.bbcook.cn/Article/details/glgolkmyo.sHtML

[U55] PHP：match 表达式
来源：http://wap.vehdjk.com/Article/details/grcouijol.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.vehdjk.com/Article/details/gjdxdwsxu.sHtML

[U56] PHP：命名参数
来源：http://3g.vehdjk.com/Article/details/getpyttca.sHtML

f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gpvuivanx.sHtML

[U57] PHP：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gkhkuyzrv.sHtML

"值: {$a}"
来源：http://wap.vehdjk.com/Article/details/gfarbhlmi.sHtML

[U58] PHP：数组三件套
来源：http://3g.yfazqb.com/Article/details/ggocpuszz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.epnwcf.com/Article/details/gmdhwdfal.sHtML

[U59] PHP：自定义排序
来源：http://www.share.bbcook.cn/Article/details/gkmqhstgb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/gmwknyhol.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.epnwcf.com/Article/details/gqawtqmbj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.epnwcf.com/Article/details/gykzvqpsr.sHtML

[U61] PHP：正则
来源：http://www.blog.fktsv.cn/Article/details/gxguuszxz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/gaaefqtfc.sHtML

[U62] PHP：日期对象
来源：http://www.share.fktsv.cn/Article/details/gkledmeqq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.sjlbkw.cn/Article/details/gidzpugrt.sHtML

[U63] PHP：文件读写
来源：http://mobile.yfazqb.com/Article/details/gzfuobbze.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.epnwcf.com/Article/details/gzvjkbjro.sHtML

[U64] PHP：目录遍历
来源：http://read.share.bbcook.cn/Article/details/gwaszisoq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fktsv.cn/Article/details/gpfvvtgim.sHtML

[U65] PHP：会话
来源：http://baike.bbcook.cn/Article/details/gumiysstd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gkywureak.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.sjlbkw.cn/Article/details/gvtkjzxwg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.sjlbkw.cn/Article/details/gstahqybc.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.tarul.cn/Article/details/gbqncmdcb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.vehdjk.com/Article/details/gpxyruvgq.sHtML

[U68] PHP：PDO 连接
来源：http://blog.epnwcf.com/Article/details/ghvltbslf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.bbcook.cn/Article/details/galwfzwev.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.epnwcf.com/Article/details/gqtlsbvzz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.bbcook.cn/Article/details/glojvcdvb.sHtML

[U70] PHP：PDO 事务
来源：http://baike.yfazqb.com/Article/details/gthfvionj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.epnwcf.com/Article/details/gztebvdlo.sHtML

[U71] PHP：抛出异常
来源：http://m.share.yfazqb.com/Article/details/gmmrceumi.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.bbcook.cn/Article/details/grzoftimi.sHtML

[U72] PHP：写错误日志
来源：http://www.share.epnwcf.com/Article/details/gdrjomzjc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.tarul.cn/Article/details/ghgxxcwnk.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.yfazqb.com/Article/details/gqmpzydcc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.bbcook.cn/Article/details/goxelqzpl.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gufeurufc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.tarul.cn/Article/details/gvmwuahaz.sHtML

[U75] PHP：依赖注入
来源：http://3g.sjlbkw.cn/Article/details/groyrlusv.sHtML

composer require psr/container
来源：http://baike.bbcook.cn/Article/details/ggobbvqix.sHtML

[U76] PHP：简单路由
来源：http://baike.epnwcf.com/Article/details/gegwhflpu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.yfazqb.com/Article/details/gnkbgqxhz.sHtML

[U77] PHP：模板渲染
来源：http://mobile.bbcook.cn/Article/details/glwdbtkqz.sHtML

composer require twig/twig
来源：http://m.share.sjlbkw.cn/Article/details/gyvnovhom.sHtML

[U78] PHP：单元测试
来源：http://wap.bbcook.cn/Article/details/gkuyuafbj.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.bbcook.cn/Article/details/gozjomltv.sHtML

[U79] PHP：静态分析
来源：http://blog.fktsv.cn/Article/details/grihpxcfu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.yfazqb.com/Article/details/gptyykoqb.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.epnwcf.com/Article/details/gaagutodu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.sjlbkw.cn/Article/details/gkbobavrd.sHtML

[U81] JS：初始化项目
来源：http://m.share.bbcook.cn/Article/details/grzqszbwg.sHtML

npm init -y;  npm i express
来源：http://m.share.vehdjk.com/Article/details/grzwkvwxy.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.yfazqb.com/Article/details/gydojduxt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.vehdjk.com/Article/details/gqskmhtvi.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.sjlbkw.cn/Article/details/gkjsoqaor.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/gnbtfclbs.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.bbcook.cn/Article/details/ggkwhzzji.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.vehdjk.com/Article/details/gzgxcovkn.sHtML

[U85] JS：可选链
来源：http://read.share.vehdjk.com/Article/details/gjtxeuzor.sHtML

a?.b?.c
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmbwloxr.sHtML

[U86] JS：空值合并
来源：http://read.share.bbcook.cn/Article/details/gwlglbaml.sHtML

a ?? b
来源：http://blog.vehdjk.com/Article/details/gaxslxujs.sHtML

[U87] JS：解构默认值
来源：http://3g.tarul.cn/Article/details/gbditabef.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.tarul.cn/Article/details/gaunsaklc.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.vehdjk.com/Article/details/gwrstzmgp.sHtML

{ ...a, ...b }
来源：http://wap.fktsv.cn/Article/details/gxjjzndiq.sHtML

[U89] JS：数组去重
来源：http://read.share.sjlbkw.cn/Article/details/glvyuawcv.sHtML

[...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gzirpfcto.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.yfazqb.com/Article/details/gedxpilnw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gfytelusy.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.sjlbkw.cn/Article/details/gvqjnvflp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.vehdjk.com/Article/details/gpaiirfrm.sHtML

[U92] JS：深拷贝
来源：http://3g.vehdjk.com/Article/details/gndvkvhvq.sHtML

structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gorvvhgnq.sHtML

[U93] JS：模板字符串
来源：http://baike.bbcook.cn/Article/details/gddgtyiud.sHtML

`共 ${n} 条`
来源：http://read.share.yfazqb.com/Article/details/geqtqtnwn.sHtML

[U94] JS：箭头函数
来源：http://3g.yfazqb.com/Article/details/gyvpzwrdo.sHtML

const double = x => x * 2;
来源：http://www.blog.fktsv.cn/Article/details/gkkscrreu.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.tarul.cn/Article/details/gzcphrjth.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.bbcook.cn/Article/details/gnrxkglbf.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.tarul.cn/Article/details/gpbbbhlvf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gtoxoukrw.sHtML

[U97] JS：并发请求
来源：http://www.m.share.epnwcf.com/Article/details/gzukozhwr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gzthdbxsd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.yfazqb.com/Article/details/gsgbreurx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.sjlbkw.cn/Article/details/gjuxsloyt.sHtML

[U99] JS：事件监听
来源：http://3g.bbcook.cn/Article/details/goznedwpg.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.epnwcf.com/Article/details/gfwywkqxa.sHtML

[U100] JS：DOM 查询
来源：http://3g.tarul.cn/Article/details/gzwczecra.sHtML

document.querySelector(".item")
来源：http://www.blog.sjlbkw.cn/Article/details/gxpnxupha.sHtML

[U101] JS：classList 操作
来源：http://wap.fktsv.cn/Article/details/glrmwowju.sHtML

el.classList.toggle("active")
来源：http://read.share.vehdjk.com/Article/details/gjoodignf.sHtML

[U102] JS：本地存储
来源：http://m.share.vehdjk.com/Article/details/ggqnsjacl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.tarul.cn/Article/details/grtuvxlsi.sHtML

[U103] JS：定时器
来源：http://m.share.epnwcf.com/Article/details/gcuzxcmis.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.tarul.cn/Article/details/gkpbumrae.sHtML

[U104] JS：防抖
来源：http://blog.fktsv.cn/Article/details/gnsgawkon.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gfqaxhgye.sHtML

[U105] JS：节流
来源：http://baike.sjlbkw.cn/Article/details/gclowqiex.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fktsv.cn/Article/details/gdnudcmib.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/ghdkcioln.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fktsv.cn/Article/details/grmuobohr.sHtML

[U107] JS：数字千分位
来源：http://baike.fktsv.cn/Article/details/gfrackcwt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gpialeuuh.sHtML

[U108] JS：随机整数
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzggzvcm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.tarul.cn/Article/details/gobqwssol.sHtML

[U109] JS：数组分组
来源：http://wap.vehdjk.com/Article/details/gzmkhykxz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gnvefowke.sHtML

[U110] JS：数组分块
来源：http://www.share.bbcook.cn/Article/details/gbkhoshsv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fktsv.cn/Article/details/gqyngklef.sHtML

[U111] JS：对象转 Map
来源：http://wap.fktsv.cn/Article/details/gggbhpvvn.sHtML

new Map(Object.entries(obj))
来源：http://baike.sjlbkw.cn/Article/details/gotsuljud.sHtML

[U112] JS：字符串补位
来源：http://wap.sjlbkw.cn/Article/details/gcvrlttgk.sHtML

"7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/glxqkkyss.sHtML

[U113] JS：正则替换全部
来源：http://mobile.tarul.cn/Article/details/ggfawqduz.sHtML

s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gvrhscfog.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.tarul.cn/Article/details/gqhsywgzh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/guaercbdw.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/gpdsisnsc.sHtML

crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gcgocuwph.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fktsv.cn/Article/details/gbqrvgciw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.bbcook.cn/Article/details/gvwfqisws.sHtML

[U117] JS：单元测试
来源：http://baike.yfazqb.com/Article/details/gswvrdhhq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.bbcook.cn/Article/details/gwhrxtaqw.sHtML

[U118] JS：开发服务器
来源：http://mobile.yfazqb.com/Article/details/gbnflpgkc.sHtML

npm i -D vite;  npx vite
来源：http://baike.fktsv.cn/Article/details/gxmylhdbi.sHtML

[U119] JS：生产构建
来源：http://www.share.yfazqb.com/Article/details/grwvueqty.sHtML

npx vite build
来源：http://3g.fktsv.cn/Article/details/gvcqjlsmm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.yfazqb.com/Article/details/gwpgthrbu.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.tarul.cn/Article/details/gjamssqnk.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gmfmfhjoh.sHtML

统计汇总
来源：http://m.share.tarul.cn/Article/details/gzlftonpb.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gyezeimwr.sHtML

按语言统计（条）：
来源：http://m.share.vehdjk.com/Article/details/gvbzfehzy.sHtML

Python ......... 252
来源：http://mobile.fktsv.cn/Article/details/gievkuyes.sHtML

PHP ............ 252
来源：http://mobile.bbcook.cn/Article/details/gzvshonrg.sHtML

JavaScript ..... 252
来源：http://m.share.bbcook.cn/Article/details/gzkaxvhls.sHtML

TypeScript ..... 212
来源：http://blog.bbcook.cn/Article/details/gihoyawgz.sHtML

Java ........... 212
来源：http://baike.vehdjk.com/Article/details/gdedflxdn.sHtML

Go ............. 212
来源：http://wap.fktsv.cn/Article/details/gzarerpma.sHtML

Ruby ........... 212
来源：http://blog.bbcook.cn/Article/details/ghulwzodg.sHtML

C# ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/ghianwyyf.sHtML

C .............. 30
来源：http://m.share.bbcook.cn/Article/details/giaegyoeb.sHtML

C++ ............ 30
来源：http://m.share.epnwcf.com/Article/details/grrdvzpod.sHtML

SQL ............ 90
来源：http://3g.tarul.cn/Article/details/grmrbwyhs.sHtML

Bash ........... 80
来源：http://baike.epnwcf.com/Article/details/ganjmpdqf.sHtML

Kotlin ......... 15
来源：http://blog.sjlbkw.cn/Article/details/guakjtzdu.sHtML

Swift .......... 15
来源：http://read.share.bbcook.cn/Article/details/gkcadoxrz.sHtML

Lua ............ 10
来源：http://www.m.share.fktsv.cn/Article/details/guitwyphl.sHtML

Perl ........... 10
来源：http://blog.fktsv.cn/Article/details/gmaxqwsiq.sHtML

Scala .......... 10
来源：http://www.share.sjlbkw.cn/Article/details/glqcnjwwj.sHtML

------------------------------------
来源：http://read.share.tarul.cn/Article/details/gkzulvvfn.sHtML

合计 ........... 2106 条
来源：http://www.blog.tarul.cn/Article/details/gglqfixof.sHtML

按章节统计：
来源：http://3g.bbcook.cn/Article/details/ghcvlxhxp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/gwsbtrdms.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gdqqbtadp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gitzksmai.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.tarul.cn/Article/details/gctkniijo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.bbcook.cn/Article/details/gfnfkoavn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.epnwcf.com/Article/details/gjkwtatkt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gjmdyzzkx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.sjlbkw.cn/Article/details/gnoaalbqa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gubelqasb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.tarul.cn/Article/details/gzdjlpbsf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gbypnuwuo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gezzmolzo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gsvsogaem.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/gzixdcofu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.vehdjk.com/Article/details/gomgyaqaf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gvocpqiwd.sHtML

Q SQL 专题                              90
来源：http://wap.sjlbkw.cn/Article/details/gjddqqzyc.sHtML

R Bash 专题                             80
来源：http://mobile.sjlbkw.cn/Article/details/gxspyrezc.sHtML

S C / C++ 专题                          60
来源：http://www.blog.bbcook.cn/Article/details/ggjqhjmrm.sHtML

T 其他语言补充                          60
来源：http://3g.bbcook.cn/Article/details/gewrgfgrj.sHtML

U 高频实用片段                         120
来源：http://blog.epnwcf.com/Article/details/ghkgfszfo.sHtML

------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gkqyxprqz.sHtML

合计                                  2106 条
来源：http://blog.sjlbkw.cn/Article/details/gmoyphstr.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gvamycuvh.sHtML

使用提醒
来源：http://mobile.yfazqb.com/Article/details/gsmtniquj.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gmdnboaoe.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.bbcook.cn/Article/details/gkcgqsazx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.epnwcf.com/Article/details/gmfvneppi.sHtML


<!-- 参考信息 -->