代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fktsv.cn/Article/details/gjrbvycgh.sHtML

[T59] Scala：循环
来源：http://wap.sjlbkw.cn/Article/details/gevnqjkci.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.vehdjk.com/Article/details/gjmukmlvc.sHtML

[T60] Scala：折叠
来源：http://baike.tarul.cn/Article/details/ggyyqwqey.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.vehdjk.com/Article/details/gogvssxnz.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gwohonufz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/ggykdxpzx.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjgrldxbw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.epnwcf.com/Article/details/gzkradzud.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.sjlbkw.cn/Article/details/gwmzuzamw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.bbcook.cn/Article/details/gqefypuvm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.bbcook.cn/Article/details/gogjuqtvj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.yfazqb.com/Article/details/gnggrbmie.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.yfazqb.com/Article/details/gpgjyyidj.sHtML

[U04] Py：变量调试打印
来源：http://www.share.bbcook.cn/Article/details/golnzuuxl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.tarul.cn/Article/details/gpuomvftq.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.yfazqb.com/Article/details/gkufbfvdp.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/glcmovmjs.sHtML

[U06] Py：合并两个字典
来源：http://m.share.sjlbkw.cn/Article/details/gptokhogd.sHtML

{**a, **b}
来源：http://read.share.fktsv.cn/Article/details/guoihawlp.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fktsv.cn/Article/details/gvyrkhemf.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.yfazqb.com/Article/details/gbivgryvd.sHtML

[U08] Py：展平二维列表
来源：http://baike.tarul.cn/Article/details/gepkodhyv.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fktsv.cn/Article/details/gjbzymvpz.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.tarul.cn/Article/details/gnyancsab.sHtML

max(d, key=d.get)
来源：http://blog.bbcook.cn/Article/details/gaadigufk.sHtML

[U10] Py：按值排序字典
来源：http://mobile.bbcook.cn/Article/details/gxuyrshtd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.yfazqb.com/Article/details/gyltbruzi.sHtML

[U11] Py：生成器表达式
来源：http://3g.epnwcf.com/Article/details/gztykvrib.sHtML

(x * 2 for x in arr)
来源：http://www.share.fktsv.cn/Article/details/gtqksrock.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.epnwcf.com/Article/details/ghrvdyucj.sHtML

Counter(arr).most_common(3)
来源：http://baike.bbcook.cn/Article/details/gezexggli.sHtML

[U13] Py：固定长度队列
来源：http://mobile.tarul.cn/Article/details/gbtysgitt.sHtML

deque(maxlen=10)
来源：http://www.share.bbcook.cn/Article/details/gdphefgjc.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fktsv.cn/Article/details/gmubfkgpb.sHtML

defaultdict(list)
来源：http://www.m.share.yfazqb.com/Article/details/garzybnhb.sHtML

[U15] Py：高精度计时
来源：http://blog.sjlbkw.cn/Article/details/gthyfxrlb.sHtML

t = time.perf_counter()
来源：http://baike.fktsv.cn/Article/details/giuptzpkl.sHtML

[U16] Py：命令行参数解析
来源：http://3g.bbcook.cn/Article/details/gtdzodgbi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.bbcook.cn/Article/details/gecozyupe.sHtML

[U17] Py：初始化日志
来源：http://mobile.yfazqb.com/Article/details/ghtywheql.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fktsv.cn/Article/details/gjzjxxhad.sHtML

[U18] Py：预编译正则
来源：http://wap.sjlbkw.cn/Article/details/ggpiqwxxh.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.epnwcf.com/Article/details/gqytglrrl.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.tarul.cn/Article/details/gfpxtqleu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.tarul.cn/Article/details/gndigtqkn.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.tarul.cn/Article/details/gtmidwark.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.sjlbkw.cn/Article/details/gmrgxbqwh.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.bbcook.cn/Article/details/gnhbvxida.sHtML

@contextlib.contextmanager
来源：http://www.share.sjlbkw.cn/Article/details/gamolcpbq.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fktsv.cn/Article/details/gnmrkcpxk.sHtML

list(zip(*m))
来源：http://www.share.sjlbkw.cn/Article/details/geyldlzhc.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.tarul.cn/Article/details/gnhzbeqnw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.sjlbkw.cn/Article/details/gmfmxznzo.sHtML

[U24] Py：路径操作
来源：http://baike.fktsv.cn/Article/details/guktmbpwh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gvuekrzvu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.bbcook.cn/Article/details/gqamiwufb.sHtML

csv.DictReader(f)
来源：http://baike.epnwcf.com/Article/details/gfzkcsbhq.sHtML

[U26] Py：并发下载
来源：http://blog.sjlbkw.cn/Article/details/gfztlljyr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.sjlbkw.cn/Article/details/gxcvmpqvx.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.tarul.cn/Article/details/gqdjjujsl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.tarul.cn/Article/details/gwxstuopn.sHtML

[U28] Py：类型别名
来源：http://www.blog.bbcook.cn/Article/details/gjjecgokq.sHtML

UserId = int
来源：http://wap.yfazqb.com/Article/details/ghwmqgbof.sHtML

[U29] Py：属性校验
来源：http://m.share.tarul.cn/Article/details/gwnlqudxq.sHtML

@property 与 @x.setter 配合
来源：http://m.share.sjlbkw.cn/Article/details/giqczvusr.sHtML

[U30] Py：数据类
来源：http://m.share.yfazqb.com/Article/details/gddzvflbu.sHtML

@dataclass(slots=True)
来源：http://m.share.tarul.cn/Article/details/gizuawyfy.sHtML

[U31] Py：单测
来源：http://mobile.sjlbkw.cn/Article/details/gzbpmkbnf.sHtML

python -m pytest -q
来源：http://3g.sjlbkw.cn/Article/details/gusudrbot.sHtML

[U32] Py：代码格式化
来源：http://3g.bbcook.cn/Article/details/gggsmrjwa.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.yfazqb.com/Article/details/glyvpazmh.sHtML

[U33] Py：打包发布
来源：http://www.share.fktsv.cn/Article/details/grbfubcvt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.vehdjk.com/Article/details/gbewsrzjm.sHtML

[U34] Py：判断编码
来源：http://3g.vehdjk.com/Article/details/gctzdzgsq.sHtML

chardet.detect(raw)
来源：http://read.share.tarul.cn/Article/details/gwomqchdc.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.epnwcf.com/Article/details/grqahfxny.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.vehdjk.com/Article/details/gqbkvrzxi.sHtML

[U36] Py：定时任务
来源：http://3g.vehdjk.com/Article/details/ghcnjtfew.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.vehdjk.com/Article/details/gnyarakzx.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fktsv.cn/Article/details/gfkecayeo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.epnwcf.com/Article/details/gyxqxbgol.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.sjlbkw.cn/Article/details/gjxlkhjen.sHtML

Path(__file__).resolve().parent
来源：http://read.share.yfazqb.com/Article/details/gzyqijadu.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fktsv.cn/Article/details/gsdyejilv.sHtML

sys.stdout.isatty()
来源：http://www.share.sjlbkw.cn/Article/details/gfttkfixo.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.vehdjk.com/Article/details/gkuyxtzzt.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gefmbjxxw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.sjlbkw.cn/Article/details/glkzvpqoc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.vehdjk.com/Article/details/gxwgnwjqn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.sjlbkw.cn/Article/details/gfglseaxj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.bbcook.cn/Article/details/gajmibrea.sHtML

[U43] PHP：声明命名空间
来源：http://baike.bbcook.cn/Article/details/gsqkffzfh.sHtML

namespace App\Http;
来源：http://www.m.share.yfazqb.com/Article/details/gxgvpqbcp.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.tarul.cn/Article/details/gmqunosqq.sHtML

declare(strict_types=1);
来源：http://wap.sjlbkw.cn/Article/details/grlpljwrt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.vehdjk.com/Article/details/ggjwlaxcf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gcwfdluoo.sHtML

[U46] PHP：可空类型
来源：http://mobile.sjlbkw.cn/Article/details/gntubhpeb.sHtML

?string $name = null
来源：http://m.share.vehdjk.com/Article/details/giymzwmeo.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbjcghun.sHtML

int|string $id
来源：http://mobile.sjlbkw.cn/Article/details/gvaykytkk.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.yfazqb.com/Article/details/gwixrlubu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fktsv.cn/Article/details/genczpkdj.sHtML

[U49] PHP：只读属性
来源：http://www.blog.tarul.cn/Article/details/gengcbdiw.sHtML

public readonly string $name
来源：http://3g.sjlbkw.cn/Article/details/gdysrswkg.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.sjlbkw.cn/Article/details/gfuxqoqyx.sHtML

public function __construct(private int $id) {}
来源：http://baike.epnwcf.com/Article/details/gplxkaepw.sHtML

[U51] PHP：数组解构
来源：http://blog.epnwcf.com/Article/details/gadumrlbp.sHtML

[$a, $b] = $arr;
来源：http://3g.epnwcf.com/Article/details/gnwyelmyw.sHtML

[U52] PHP：箭头函数
来源：http://3g.yfazqb.com/Article/details/gaptqemec.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.epnwcf.com/Article/details/gnralvzvh.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.epnwcf.com/Article/details/gtfjkcowd.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.epnwcf.com/Article/details/gjljqnfku.sHtML

[U54] PHP：空安全调用
来源：http://3g.yfazqb.com/Article/details/gxxvfcoog.sHtML

$obj?->method()
来源：http://www.blog.sjlbkw.cn/Article/details/gdlumcqqf.sHtML

[U55] PHP：match 表达式
来源：http://mobile.epnwcf.com/Article/details/guwfmfhzl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.epnwcf.com/Article/details/glvlypkbn.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gcsnjcssb.sHtML

f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gseyldbew.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gdpfotimp.sHtML

"值: {$a}"
来源：http://m.share.tarul.cn/Article/details/gvsdmcfis.sHtML

[U58] PHP：数组三件套
来源：http://baike.tarul.cn/Article/details/gekpufywj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.bbcook.cn/Article/details/grcszegck.sHtML

[U59] PHP：自定义排序
来源：http://mobile.sjlbkw.cn/Article/details/gbhcvjkyz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/goenahpfm.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.yfazqb.com/Article/details/gezkubngx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.vehdjk.com/Article/details/gmyrtdlzh.sHtML

[U61] PHP：正则
来源：http://m.share.sjlbkw.cn/Article/details/gmoqxfnnc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gmtdwqkze.sHtML

[U62] PHP：日期对象
来源：http://baike.epnwcf.com/Article/details/ghoqaipvi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.bbcook.cn/Article/details/gdevmjdks.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.epnwcf.com/Article/details/gxuvesvua.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.tarul.cn/Article/details/ghsyaivak.sHtML

[U64] PHP：目录遍历
来源：http://www.share.vehdjk.com/Article/details/gmtzoupnb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.bbcook.cn/Article/details/gnwjfstue.sHtML

[U65] PHP：会话
来源：http://www.share.sjlbkw.cn/Article/details/gbnogzbwk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.vehdjk.com/Article/details/gehbbvtay.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fktsv.cn/Article/details/gvptthmwb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.yfazqb.com/Article/details/gmgsvhpbc.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.vehdjk.com/Article/details/gbpdnxvuy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.yfazqb.com/Article/details/gxnvxjzwl.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fktsv.cn/Article/details/ghiwlzbza.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.epnwcf.com/Article/details/glptfkdds.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fktsv.cn/Article/details/gnectapdj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fktsv.cn/Article/details/gjidtlahf.sHtML

[U70] PHP：PDO 事务
来源：http://baike.vehdjk.com/Article/details/gcachmzgv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fktsv.cn/Article/details/gmbrwbopr.sHtML

[U71] PHP：抛出异常
来源：http://baike.epnwcf.com/Article/details/gqxjejsxh.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgomavdz.sHtML

[U72] PHP：写错误日志
来源：http://www.share.tarul.cn/Article/details/gqdznbzdp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.vehdjk.com/Article/details/gswwxzmlb.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.vehdjk.com/Article/details/gremphxmp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.sjlbkw.cn/Article/details/gnfmeuewb.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gfyyktfdj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.epnwcf.com/Article/details/gzkaxmphi.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.bbcook.cn/Article/details/gztqyuahb.sHtML

composer require psr/container
来源：http://baike.vehdjk.com/Article/details/gkgvoiiak.sHtML

[U76] PHP：简单路由
来源：http://mobile.sjlbkw.cn/Article/details/glzblrbop.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.bbcook.cn/Article/details/gowlkqkip.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fktsv.cn/Article/details/gtcdgcmmp.sHtML

composer require twig/twig
来源：http://3g.vehdjk.com/Article/details/gwyunojel.sHtML

[U78] PHP：单元测试
来源：http://baike.epnwcf.com/Article/details/glxgzzbpt.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.tarul.cn/Article/details/gkodwmfzd.sHtML

[U79] PHP：静态分析
来源：http://blog.yfazqb.com/Article/details/gsjdkbbyi.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.yfazqb.com/Article/details/ggzlmsetb.sHtML

[U80] PHP：代码规范修复
来源：http://blog.bbcook.cn/Article/details/gaemhkxcr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.epnwcf.com/Article/details/gzbihfzzh.sHtML

[U81] JS：初始化项目
来源：http://wap.bbcook.cn/Article/details/gohgzyzzj.sHtML

npm init -y;  npm i express
来源：http://3g.fktsv.cn/Article/details/gwbjfqmco.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.yfazqb.com/Article/details/gevwejsor.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.epnwcf.com/Article/details/gpfohevbc.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.yfazqb.com/Article/details/gxuhlrkei.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.bbcook.cn/Article/details/gtygmsfes.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.tarul.cn/Article/details/gyoyzekvh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.sjlbkw.cn/Article/details/gekdylcff.sHtML

[U85] JS：可选链
来源：http://baike.bbcook.cn/Article/details/gtybjodcv.sHtML

a?.b?.c
来源：http://blog.fktsv.cn/Article/details/gevatmbws.sHtML

[U86] JS：空值合并
来源：http://baike.epnwcf.com/Article/details/gfkguhwzl.sHtML

a ?? b
来源：http://blog.sjlbkw.cn/Article/details/getnvsqyu.sHtML

[U87] JS：解构默认值
来源：http://baike.fktsv.cn/Article/details/gyxlcfewz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.vehdjk.com/Article/details/gwpbdjbum.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fktsv.cn/Article/details/gddgxirfx.sHtML

{ ...a, ...b }
来源：http://wap.vehdjk.com/Article/details/gupyskbat.sHtML

[U89] JS：数组去重
来源：http://www.blog.epnwcf.com/Article/details/girpyjlpx.sHtML

[...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/guggfrbvm.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fktsv.cn/Article/details/gusihgbxx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gtjtlmikx.sHtML

[U91] JS：对象键值遍历
来源：http://3g.tarul.cn/Article/details/gbwcyhtkb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.yfazqb.com/Article/details/gbaoxtxmw.sHtML

[U92] JS：深拷贝
来源：http://read.share.yfazqb.com/Article/details/geblnsddj.sHtML

structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gycmhbmfw.sHtML

[U93] JS：模板字符串
来源：http://www.share.vehdjk.com/Article/details/ghmtjcgvk.sHtML

`共 ${n} 条`
来源：http://3g.tarul.cn/Article/details/gitrpedfm.sHtML

[U94] JS：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gqttuntwo.sHtML

const double = x => x * 2;
来源：http://read.share.sjlbkw.cn/Article/details/gbzreajyz.sHtML

[U95] JS：Promise 包装
来源：http://blog.sjlbkw.cn/Article/details/gagalokjb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.tarul.cn/Article/details/gmthsmbyj.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fktsv.cn/Article/details/gnxownfcp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gdwxtczdr.sHtML

[U97] JS：并发请求
来源：http://www.share.yfazqb.com/Article/details/gbwhyhzyy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gydcjwpsy.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fktsv.cn/Article/details/gbrjregxp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.tarul.cn/Article/details/gnbukkqok.sHtML

[U99] JS：事件监听
来源：http://www.m.share.vehdjk.com/Article/details/gsssizqlv.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.yfazqb.com/Article/details/gdgemqhqr.sHtML

[U100] JS：DOM 查询
来源：http://www.share.sjlbkw.cn/Article/details/gicygxkow.sHtML

document.querySelector(".item")
来源：http://www.share.yfazqb.com/Article/details/gbxxtifvm.sHtML

[U101] JS：classList 操作
来源：http://wap.fktsv.cn/Article/details/gwdeaaaux.sHtML

el.classList.toggle("active")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqtbcvwk.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fktsv.cn/Article/details/gjmaamggh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.epnwcf.com/Article/details/gvbfljuno.sHtML

[U103] JS：定时器
来源：http://mobile.yfazqb.com/Article/details/girjoooka.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.epnwcf.com/Article/details/guykxaqju.sHtML

[U104] JS：防抖
来源：http://www.share.sjlbkw.cn/Article/details/gjxdzwdoy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/gwghhwuas.sHtML

[U105] JS：节流
来源：http://baike.bbcook.cn/Article/details/gcdmyrogk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.bbcook.cn/Article/details/gmphucwtb.sHtML

[U106] JS：日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gmzduocac.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fktsv.cn/Article/details/grjktitoo.sHtML

[U107] JS：数字千分位
来源：http://blog.yfazqb.com/Article/details/gntfpethz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fktsv.cn/Article/details/gflbuanpc.sHtML

[U108] JS：随机整数
来源：http://read.share.tarul.cn/Article/details/gwspcdqsu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.vehdjk.com/Article/details/gbvdtpooj.sHtML

[U109] JS：数组分组
来源：http://read.share.epnwcf.com/Article/details/gabapezck.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fktsv.cn/Article/details/gwcktprff.sHtML

[U110] JS：数组分块
来源：http://www.blog.sjlbkw.cn/Article/details/gyakrxbjc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.epnwcf.com/Article/details/gsghgyqxw.sHtML

[U111] JS：对象转 Map
来源：http://www.share.tarul.cn/Article/details/gjuuznouf.sHtML

new Map(Object.entries(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gqksjbxhm.sHtML

[U112] JS：字符串补位
来源：http://read.share.sjlbkw.cn/Article/details/gegtjcxfp.sHtML

"7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gkwqwsqeg.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.yfazqb.com/Article/details/grnedfkdd.sHtML

s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gledzsnqj.sHtML

[U114] JS：JSON 深比较
来源：http://blog.tarul.cn/Article/details/gungrozgm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gfburoawp.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/grfpwxbri.sHtML

crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gfpvtndte.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.sjlbkw.cn/Article/details/gjyllbrap.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.tarul.cn/Article/details/gdzylgrhw.sHtML

[U117] JS：单元测试
来源：http://www.share.yfazqb.com/Article/details/ghcdnjidf.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.yfazqb.com/Article/details/gzhthojgu.sHtML

[U118] JS：开发服务器
来源：http://baike.tarul.cn/Article/details/gbrovcrkh.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fktsv.cn/Article/details/geoplzokn.sHtML

[U119] JS：生产构建
来源：http://m.share.tarul.cn/Article/details/glrwpcjwx.sHtML

npx vite build
来源：http://www.m.share.bbcook.cn/Article/details/gdzfjvgvo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.tarul.cn/Article/details/gfrqjerql.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.sjlbkw.cn/Article/details/gobcckyas.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gixoboihc.sHtML

统计汇总
来源：http://mobile.yfazqb.com/Article/details/gzmtujpqj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gscpbfubx.sHtML

按语言统计（条）：
来源：http://read.share.sjlbkw.cn/Article/details/ghuepzzwp.sHtML

Python ......... 252
来源：http://www.blog.sjlbkw.cn/Article/details/gyulyycll.sHtML

PHP ............ 252
来源：http://blog.vehdjk.com/Article/details/glofsmokg.sHtML

JavaScript ..... 252
来源：http://m.share.epnwcf.com/Article/details/gucwioxtf.sHtML

TypeScript ..... 212
来源：http://3g.bbcook.cn/Article/details/gdlleaqky.sHtML

Java ........... 212
来源：http://www.m.share.yfazqb.com/Article/details/gzgtxbkbr.sHtML

Go ............. 212
来源：http://blog.bbcook.cn/Article/details/gtelytyir.sHtML

Ruby ........... 212
来源：http://www.share.sjlbkw.cn/Article/details/grynypqkb.sHtML

C# ............. 212
来源：http://3g.sjlbkw.cn/Article/details/grwmzsrnq.sHtML

C .............. 30
来源：http://www.m.share.yfazqb.com/Article/details/gqqblxtev.sHtML

C++ ............ 30
来源：http://blog.epnwcf.com/Article/details/gtguicrly.sHtML

SQL ............ 90
来源：http://blog.yfazqb.com/Article/details/gctqlgmra.sHtML

Bash ........... 80
来源：http://www.share.fktsv.cn/Article/details/gtwhgqmtj.sHtML

Kotlin ......... 15
来源：http://mobile.yfazqb.com/Article/details/ghlbejlwa.sHtML

Swift .......... 15
来源：http://www.blog.tarul.cn/Article/details/gmupnwjbt.sHtML

Lua ............ 10
来源：http://3g.vehdjk.com/Article/details/gtlovrwba.sHtML

Perl ........... 10
来源：http://read.share.vehdjk.com/Article/details/ggnlfnlvj.sHtML

Scala .......... 10
来源：http://m.share.bbcook.cn/Article/details/gyxuseiml.sHtML

------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gnssxgohr.sHtML

合计 ........... 2106 条
来源：http://wap.bbcook.cn/Article/details/ghpsiracf.sHtML

按章节统计：
来源：http://mobile.yfazqb.com/Article/details/gjpuyxenk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/gtuwyxrfx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/gzcxemjat.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gtlfxpwsb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.sjlbkw.cn/Article/details/goatzeuer.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.bbcook.cn/Article/details/gpjbuicdg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.bbcook.cn/Article/details/gwitwffno.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gtcdyrohb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.bbcook.cn/Article/details/gjpazdlyf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gdvianlbv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.epnwcf.com/Article/details/gfnqfxdhn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/gqcuykztd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gngjqffum.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gvztovhby.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.vehdjk.com/Article/details/gbaflendh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.tarul.cn/Article/details/gannxpmse.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gfayuczgl.sHtML

Q SQL 专题                              90
来源：http://3g.yfazqb.com/Article/details/gpkozldpl.sHtML

R Bash 专题                             80
来源：http://www.share.tarul.cn/Article/details/gpzmezxjh.sHtML

S C / C++ 专题                          60
来源：http://read.share.epnwcf.com/Article/details/gsujkttuh.sHtML

T 其他语言补充                          60
来源：http://www.m.share.epnwcf.com/Article/details/gierzhdmf.sHtML

U 高频实用片段                         120
来源：http://www.blog.epnwcf.com/Article/details/gptdoiiuo.sHtML

------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gokqpbrnx.sHtML

合计                                  2106 条
来源：http://www.m.share.bbcook.cn/Article/details/gneeyitnr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/ggftkqkwy.sHtML

使用提醒
来源：http://www.m.share.yfazqb.com/Article/details/gphzlxytj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/glssjdijt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.yfazqb.com/Article/details/gozxdnmmf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.bbcook.cn/Article/details/grgcudpdj.sHtML


<!-- 参考信息 -->