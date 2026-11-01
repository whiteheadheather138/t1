代发 wailian999

case class User(name: String, age: Int)
来源：http://m.share.epnwcf.com/Article/details/grjrqjksb.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.bbcook.cn/Article/details/giqbioqcl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fktsv.cn/Article/details/goacsbtwm.sHtML

[T58] Scala：函数定义
来源：http://3g.epnwcf.com/Article/details/gbzalkpzv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.sjlbkw.cn/Article/details/gkogzmzys.sHtML

[T59] Scala：循环
来源：http://www.share.bbcook.cn/Article/details/gedidnmql.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.yfazqb.com/Article/details/gjeouommz.sHtML

[T60] Scala：折叠
来源：http://mobile.epnwcf.com/Article/details/gcpozfukc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.yfazqb.com/Article/details/gccpltdnl.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfkylunpt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.sjlbkw.cn/Article/details/gxabvgmvg.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtzqapvbh.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.yfazqb.com/Article/details/ggcfahprh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.vehdjk.com/Article/details/gfkchnniu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.vehdjk.com/Article/details/gkoeohmuo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.epnwcf.com/Article/details/giaithbju.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.bbcook.cn/Article/details/grggkmuid.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fktsv.cn/Article/details/gtxqqxphd.sHtML

[U04] Py：变量调试打印
来源：http://mobile.bbcook.cn/Article/details/glskoirjz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fktsv.cn/Article/details/glguoqfpq.sHtML

[U05] Py：列表去重且保序
来源：http://wap.vehdjk.com/Article/details/gtymuriys.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gofqkuyoc.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fktsv.cn/Article/details/gzminfsid.sHtML

{**a, **b}
来源：http://wap.fktsv.cn/Article/details/glmckjetq.sHtML

[U07] Py：反转字典键值
来源：http://www.share.epnwcf.com/Article/details/gxgnbodok.sHtML

{v: k for k, v in d.items()}
来源：http://baike.epnwcf.com/Article/details/gidsfkllh.sHtML

[U08] Py：展平二维列表
来源：http://mobile.epnwcf.com/Article/details/gptedzeky.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.yfazqb.com/Article/details/gtiqknjmh.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.bbcook.cn/Article/details/gkqhyggmd.sHtML

max(d, key=d.get)
来源：http://www.share.fktsv.cn/Article/details/goocgobut.sHtML

[U10] Py：按值排序字典
来源：http://mobile.vehdjk.com/Article/details/gfbdmgrai.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.vehdjk.com/Article/details/gykhjjhvj.sHtML

[U11] Py：生成器表达式
来源：http://blog.epnwcf.com/Article/details/gbyrjeadb.sHtML

(x * 2 for x in arr)
来源：http://blog.yfazqb.com/Article/details/glqtnkbpm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.tarul.cn/Article/details/gliwmxsuy.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fktsv.cn/Article/details/ggvywtrlg.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fktsv.cn/Article/details/grlndgyhb.sHtML

deque(maxlen=10)
来源：http://read.share.sjlbkw.cn/Article/details/gvvxupfeh.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.epnwcf.com/Article/details/gnlnpamnj.sHtML

defaultdict(list)
来源：http://baike.vehdjk.com/Article/details/gpkxsbimb.sHtML

[U15] Py：高精度计时
来源：http://www.share.sjlbkw.cn/Article/details/gzwwvhayk.sHtML

t = time.perf_counter()
来源：http://www.m.share.fktsv.cn/Article/details/gqdwiohew.sHtML

[U16] Py：命令行参数解析
来源：http://wap.epnwcf.com/Article/details/gcdhcdpuo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.sjlbkw.cn/Article/details/gvkxcdufk.sHtML

[U17] Py：初始化日志
来源：http://m.share.sjlbkw.cn/Article/details/gfwgtcles.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.sjlbkw.cn/Article/details/gyabizoxh.sHtML

[U18] Py：预编译正则
来源：http://mobile.sjlbkw.cn/Article/details/gizglircy.sHtML

pat = re.compile(r"\d+")
来源：http://3g.vehdjk.com/Article/details/goxrzilju.sHtML

[U19] Py：正则替换带回调
来源：http://blog.yfazqb.com/Article/details/gtpjortue.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.bbcook.cn/Article/details/gtpeceyyu.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.epnwcf.com/Article/details/ghwqzribs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.epnwcf.com/Article/details/gdxxcadiw.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.vehdjk.com/Article/details/gelhllbmp.sHtML

@contextlib.contextmanager
来源：http://www.blog.tarul.cn/Article/details/gjgdyfhoi.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fktsv.cn/Article/details/grqqpursj.sHtML

list(zip(*m))
来源：http://www.share.fktsv.cn/Article/details/gvujzmtji.sHtML

[U23] Py：分块读取大文件
来源：http://blog.vehdjk.com/Article/details/gvuaqfdmc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.epnwcf.com/Article/details/grcgwuyik.sHtML

[U24] Py：路径操作
来源：http://m.share.sjlbkw.cn/Article/details/gfvugkeoe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gydvmfnpo.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.tarul.cn/Article/details/goixqutpv.sHtML

csv.DictReader(f)
来源：http://www.blog.vehdjk.com/Article/details/gxosgqysw.sHtML

[U26] Py：并发下载
来源：http://www.blog.bbcook.cn/Article/details/guujqddnf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fktsv.cn/Article/details/gkjohbyzk.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.tarul.cn/Article/details/gzfgszvlg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.bbcook.cn/Article/details/ghztsivub.sHtML

[U28] Py：类型别名
来源：http://3g.yfazqb.com/Article/details/gxizzgzjq.sHtML

UserId = int
来源：http://3g.yfazqb.com/Article/details/gmueqnbdc.sHtML

[U29] Py：属性校验
来源：http://www.blog.sjlbkw.cn/Article/details/gqcgzixsg.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.bbcook.cn/Article/details/gfljzlgdb.sHtML

[U30] Py：数据类
来源：http://baike.tarul.cn/Article/details/gbcqynyvq.sHtML

@dataclass(slots=True)
来源：http://3g.tarul.cn/Article/details/gbuktsodq.sHtML

[U31] Py：单测
来源：http://blog.bbcook.cn/Article/details/gzaawuoib.sHtML

python -m pytest -q
来源：http://mobile.tarul.cn/Article/details/gwesxcfll.sHtML

[U32] Py：代码格式化
来源：http://blog.vehdjk.com/Article/details/gmqizelga.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.bbcook.cn/Article/details/gtwjqmjqb.sHtML

[U33] Py：打包发布
来源：http://mobile.fktsv.cn/Article/details/gwifhwlyr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.sjlbkw.cn/Article/details/gfogluerx.sHtML

[U34] Py：判断编码
来源：http://3g.epnwcf.com/Article/details/gjbxlytbc.sHtML

chardet.detect(raw)
来源：http://3g.fktsv.cn/Article/details/goxlfmlxx.sHtML

[U35] Py：发送邮件
来源：http://wap.yfazqb.com/Article/details/grfbaydnj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.tarul.cn/Article/details/gntenoedn.sHtML

[U36] Py：定时任务
来源：http://read.share.bbcook.cn/Article/details/gjarwpbcy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.tarul.cn/Article/details/giinqzggv.sHtML

[U37] Py：读写 Excel
来源：http://blog.yfazqb.com/Article/details/gjzedzcsk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fktsv.cn/Article/details/getjtvjpc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.epnwcf.com/Article/details/gtehjlzbe.sHtML

Path(__file__).resolve().parent
来源：http://blog.fktsv.cn/Article/details/goizigpfd.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.tarul.cn/Article/details/gtxoxicrx.sHtML

sys.stdout.isatty()
来源：http://baike.fktsv.cn/Article/details/grdqykeyv.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fktsv.cn/Article/details/gdiyivcco.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gthikzvqe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.yfazqb.com/Article/details/gyherbbau.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.vehdjk.com/Article/details/gscnjffgr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.bbcook.cn/Article/details/gznktevst.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.tarul.cn/Article/details/gtplaeiph.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.sjlbkw.cn/Article/details/grgtndppx.sHtML

namespace App\Http;
来源：http://wap.yfazqb.com/Article/details/gfjuszxgq.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.epnwcf.com/Article/details/gvsqprjuf.sHtML

declare(strict_types=1);
来源：http://www.share.bbcook.cn/Article/details/gwogtctxe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.bbcook.cn/Article/details/ggsjiaoba.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gkkoqwsqd.sHtML

[U46] PHP：可空类型
来源：http://www.blog.tarul.cn/Article/details/gbiypkwjr.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gthjckmzi.sHtML

[U47] PHP：联合类型
来源：http://baike.sjlbkw.cn/Article/details/gspfzrrbp.sHtML

int|string $id
来源：http://read.share.fktsv.cn/Article/details/guanyytrk.sHtML

[U48] PHP：纯枚举
来源：http://mobile.epnwcf.com/Article/details/grkfquhgj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.tarul.cn/Article/details/gyuxsqqtx.sHtML

[U49] PHP：只读属性
来源：http://baike.epnwcf.com/Article/details/gnhstdgeu.sHtML

public readonly string $name
来源：http://wap.bbcook.cn/Article/details/gvowqjftl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.tarul.cn/Article/details/glbuujcyc.sHtML

public function __construct(private int $id) {}
来源：http://3g.vehdjk.com/Article/details/gzjvlpzam.sHtML

[U51] PHP：数组解构
来源：http://baike.sjlbkw.cn/Article/details/gfbbkfmrn.sHtML

[$a, $b] = $arr;
来源：http://3g.tarul.cn/Article/details/ggunkodqn.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.vehdjk.com/Article/details/gwhzkqcuv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.bbcook.cn/Article/details/gwphfnpcs.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fktsv.cn/Article/details/goqbzerli.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.yfazqb.com/Article/details/gmfdfmnfd.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fktsv.cn/Article/details/gdtjihwko.sHtML

$obj?->method()
来源：http://mobile.vehdjk.com/Article/details/gjcwhkrxn.sHtML

[U55] PHP：match 表达式
来源：http://wap.epnwcf.com/Article/details/guffyijai.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fktsv.cn/Article/details/gmeutjmvj.sHtML

[U56] PHP：命名参数
来源：http://wap.vehdjk.com/Article/details/gdqbyjnsn.sHtML

f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gwirshovw.sHtML

[U57] PHP：字符串插值
来源：http://baike.tarul.cn/Article/details/ggztjbkqi.sHtML

"值: {$a}"
来源：http://www.m.share.epnwcf.com/Article/details/geikwlvda.sHtML

[U58] PHP：数组三件套
来源：http://www.share.tarul.cn/Article/details/gvmjjltqy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fktsv.cn/Article/details/gexelwgfq.sHtML

[U59] PHP：自定义排序
来源：http://m.share.epnwcf.com/Article/details/gvdxgcfzd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.tarul.cn/Article/details/gizutkvot.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.epnwcf.com/Article/details/gxhwuksvf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.vehdjk.com/Article/details/gyubawtlm.sHtML

[U61] PHP：正则
来源：http://www.share.fktsv.cn/Article/details/gnvldxejk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/gzmphglsa.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.yfazqb.com/Article/details/gtaslbero.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.epnwcf.com/Article/details/gitxsyktk.sHtML

[U63] PHP：文件读写
来源：http://read.share.sjlbkw.cn/Article/details/ggxsidhds.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.sjlbkw.cn/Article/details/gwvrwzeiz.sHtML

[U64] PHP：目录遍历
来源：http://read.share.tarul.cn/Article/details/gatqmnuun.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.sjlbkw.cn/Article/details/grrahhbxi.sHtML

[U65] PHP：会话
来源：http://baike.fktsv.cn/Article/details/glbzipzqu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/glltnytou.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.tarul.cn/Article/details/gbdosxhok.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.yfazqb.com/Article/details/gakxkdaxw.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.sjlbkw.cn/Article/details/gqmxjdqac.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.sjlbkw.cn/Article/details/gyozjgcax.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.bbcook.cn/Article/details/gaufjxjio.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.epnwcf.com/Article/details/gunadzlse.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.vehdjk.com/Article/details/gqohdwhne.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.vehdjk.com/Article/details/gsovzsqwd.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.bbcook.cn/Article/details/ghyjuctpk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.bbcook.cn/Article/details/gmsghzuky.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.yfazqb.com/Article/details/gqqnuvbfh.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.sjlbkw.cn/Article/details/ggqomjtek.sHtML

[U72] PHP：写错误日志
来源：http://mobile.bbcook.cn/Article/details/gxnjajxnu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.sjlbkw.cn/Article/details/gyfhhfebd.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fktsv.cn/Article/details/gmhzrzfrq.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.vehdjk.com/Article/details/gnqgftcua.sHtML

[U74] PHP：读取环境变量
来源：http://wap.yfazqb.com/Article/details/gzdvpueif.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.vehdjk.com/Article/details/gtaxiugej.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fktsv.cn/Article/details/gzfugmjdi.sHtML

composer require psr/container
来源：http://3g.vehdjk.com/Article/details/gzwhtmdjo.sHtML

[U76] PHP：简单路由
来源：http://www.blog.tarul.cn/Article/details/gksqikoro.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.bbcook.cn/Article/details/gzapixufs.sHtML

[U77] PHP：模板渲染
来源：http://mobile.bbcook.cn/Article/details/gqzhdtggg.sHtML

composer require twig/twig
来源：http://read.share.vehdjk.com/Article/details/gfnjqdlpc.sHtML

[U78] PHP：单元测试
来源：http://mobile.yfazqb.com/Article/details/gohaevjpw.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.vehdjk.com/Article/details/gnvubazzp.sHtML

[U79] PHP：静态分析
来源：http://www.share.tarul.cn/Article/details/gjplqbadq.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.bbcook.cn/Article/details/guyyyjfxj.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fktsv.cn/Article/details/gjxdtcubu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fktsv.cn/Article/details/gmvyfmppr.sHtML

[U81] JS：初始化项目
来源：http://www.blog.yfazqb.com/Article/details/glugvplvy.sHtML

npm init -y;  npm i express
来源：http://www.m.share.bbcook.cn/Article/details/grpvlbqhs.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.yfazqb.com/Article/details/gtrekjour.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.sjlbkw.cn/Article/details/gjspboxyr.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.tarul.cn/Article/details/gviccuqhf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/gzllzkbib.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.vehdjk.com/Article/details/glgaarepg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.sjlbkw.cn/Article/details/gpjbbldva.sHtML

[U85] JS：可选链
来源：http://mobile.sjlbkw.cn/Article/details/gaqadnrjc.sHtML

a?.b?.c
来源：http://3g.sjlbkw.cn/Article/details/ggzgvnbvw.sHtML

[U86] JS：空值合并
来源：http://www.m.share.bbcook.cn/Article/details/gylfuxgrq.sHtML

a ?? b
来源：http://www.share.fktsv.cn/Article/details/gohyjbgol.sHtML

[U87] JS：解构默认值
来源：http://read.share.vehdjk.com/Article/details/gpqxyzube.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.tarul.cn/Article/details/gujgnxetr.sHtML

[U88] JS：对象展开合并
来源：http://blog.tarul.cn/Article/details/gsxnaxokp.sHtML

{ ...a, ...b }
来源：http://m.share.tarul.cn/Article/details/gwxlqwdid.sHtML

[U89] JS：数组去重
来源：http://m.share.vehdjk.com/Article/details/guizdxgkc.sHtML

[...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/giqtclyvi.sHtML

[U90] JS：数字数组排序
来源：http://mobile.epnwcf.com/Article/details/gohccesfx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gwfobbyzf.sHtML

[U91] JS：对象键值遍历
来源：http://wap.yfazqb.com/Article/details/gobrglppi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.bbcook.cn/Article/details/gjxufszfb.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjqvrtex.sHtML

structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/ggkdbhckq.sHtML

[U93] JS：模板字符串
来源：http://m.share.tarul.cn/Article/details/gkfdamped.sHtML

`共 ${n} 条`
来源：http://www.share.tarul.cn/Article/details/gbrcgerwy.sHtML

[U94] JS：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/gkblpixln.sHtML

const double = x => x * 2;
来源：http://read.share.fktsv.cn/Article/details/gepthnfzt.sHtML

[U95] JS：Promise 包装
来源：http://www.share.epnwcf.com/Article/details/guzkiadzj.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.epnwcf.com/Article/details/gsobekopa.sHtML

[U96] JS：async/await 与异常
来源：http://3g.yfazqb.com/Article/details/greedeyuq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gziukstvd.sHtML

[U97] JS：并发请求
来源：http://blog.bbcook.cn/Article/details/gbnswblzm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gttzncnkg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gkgiifjxx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.vehdjk.com/Article/details/gohaxiunu.sHtML

[U99] JS：事件监听
来源：http://m.share.yfazqb.com/Article/details/gzpctmang.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.yfazqb.com/Article/details/gagnxcqos.sHtML

[U100] JS：DOM 查询
来源：http://wap.fktsv.cn/Article/details/guhfijjtw.sHtML

document.querySelector(".item")
来源：http://www.share.epnwcf.com/Article/details/gomxybpsl.sHtML

[U101] JS：classList 操作
来源：http://read.share.sjlbkw.cn/Article/details/gdrzizptf.sHtML

el.classList.toggle("active")
来源：http://wap.epnwcf.com/Article/details/gzxwxjhor.sHtML

[U102] JS：本地存储
来源：http://www.m.share.yfazqb.com/Article/details/gmiuaipxy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.tarul.cn/Article/details/geixzmasv.sHtML

[U103] JS：定时器
来源：http://baike.yfazqb.com/Article/details/ghrahuixa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.yfazqb.com/Article/details/gorqscaro.sHtML

[U104] JS：防抖
来源：http://www.share.epnwcf.com/Article/details/gbqotfwdq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gbbizfchr.sHtML

[U105] JS：节流
来源：http://read.share.fktsv.cn/Article/details/gchxmmmaw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.bbcook.cn/Article/details/gnhltpxnt.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gghpmttaw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fktsv.cn/Article/details/gpgignbip.sHtML

[U107] JS：数字千分位
来源：http://www.share.vehdjk.com/Article/details/gwlxgtkig.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.tarul.cn/Article/details/gkkdweilp.sHtML

[U108] JS：随机整数
来源：http://www.blog.fktsv.cn/Article/details/givgunhyc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.yfazqb.com/Article/details/guujzyqos.sHtML

[U109] JS：数组分组
来源：http://mobile.yfazqb.com/Article/details/gosvkpelm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.epnwcf.com/Article/details/gseleissk.sHtML

[U110] JS：数组分块
来源：http://www.blog.epnwcf.com/Article/details/gvktlylcr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.bbcook.cn/Article/details/gmcgjgqpn.sHtML

[U111] JS：对象转 Map
来源：http://wap.epnwcf.com/Article/details/gxmshedem.sHtML

new Map(Object.entries(obj))
来源：http://mobile.tarul.cn/Article/details/gdpeollws.sHtML

[U112] JS：字符串补位
来源：http://mobile.yfazqb.com/Article/details/gaqjpckdi.sHtML

"7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gqslvjgnx.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fktsv.cn/Article/details/gypjlyvvx.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gyrydgmvh.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.yfazqb.com/Article/details/gfqpphovb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/gtfrorqyz.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fktsv.cn/Article/details/gmkcieewz.sHtML

crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/golympbqo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.yfazqb.com/Article/details/gnotzbofm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.bbcook.cn/Article/details/gpowpexes.sHtML

[U117] JS：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/gkiofgnjt.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.yfazqb.com/Article/details/gkfwiubzu.sHtML

[U118] JS：开发服务器
来源：http://read.share.sjlbkw.cn/Article/details/grozwqsph.sHtML

npm i -D vite;  npx vite
来源：http://wap.bbcook.cn/Article/details/gopgxgexq.sHtML

[U119] JS：生产构建
来源：http://www.m.share.sjlbkw.cn/Article/details/gudjytrlx.sHtML

npx vite build
来源：http://www.m.share.vehdjk.com/Article/details/glmfrxdcq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.bbcook.cn/Article/details/gqnqqedkg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.vehdjk.com/Article/details/gziobuixt.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gjonzcfns.sHtML

统计汇总
来源：http://wap.yfazqb.com/Article/details/goejdcogr.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/giijaimxb.sHtML

按语言统计（条）：
来源：http://3g.vehdjk.com/Article/details/gtetxeucy.sHtML

Python ......... 252
来源：http://blog.sjlbkw.cn/Article/details/grgdmwcin.sHtML

PHP ............ 252
来源：http://mobile.epnwcf.com/Article/details/gtyykzzyy.sHtML

JavaScript ..... 252
来源：http://blog.bbcook.cn/Article/details/gyuycmstx.sHtML

TypeScript ..... 212
来源：http://mobile.bbcook.cn/Article/details/gjvhbbjgg.sHtML

Java ........... 212
来源：http://m.share.yfazqb.com/Article/details/gykhcykvg.sHtML

Go ............. 212
来源：http://www.m.share.bbcook.cn/Article/details/gjmsueoop.sHtML

Ruby ........... 212
来源：http://mobile.fktsv.cn/Article/details/ghxrebhvd.sHtML

C# ............. 212
来源：http://www.blog.tarul.cn/Article/details/gqrbrkacd.sHtML

C .............. 30
来源：http://3g.tarul.cn/Article/details/gvwhtcstt.sHtML

C++ ............ 30
来源：http://read.share.epnwcf.com/Article/details/gcznqkhsr.sHtML

SQL ............ 90
来源：http://baike.epnwcf.com/Article/details/gnuqcfhaq.sHtML

Bash ........... 80
来源：http://baike.vehdjk.com/Article/details/gzromzezi.sHtML

Kotlin ......... 15
来源：http://www.blog.yfazqb.com/Article/details/ghrhfbneo.sHtML

Swift .......... 15
来源：http://mobile.sjlbkw.cn/Article/details/ghfygmflq.sHtML

Lua ............ 10
来源：http://blog.bbcook.cn/Article/details/gfecnyypb.sHtML

Perl ........... 10
来源：http://wap.sjlbkw.cn/Article/details/gprquaxjk.sHtML

Scala .......... 10
来源：http://www.blog.vehdjk.com/Article/details/gbjhkhqsv.sHtML

------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gfqxwdgvn.sHtML

合计 ........... 2106 条
来源：http://3g.epnwcf.com/Article/details/gorjrmecf.sHtML

按章节统计：
来源：http://baike.yfazqb.com/Article/details/gltkexnky.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/gzjvamupb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gonqboqbe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/gpezlsozb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gblprxtlj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.sjlbkw.cn/Article/details/gyjzgjlhb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/glnujckag.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/gvjrpkrbf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.yfazqb.com/Article/details/gjmrzclkm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gdwvhiqmd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.tarul.cn/Article/details/gypgdbubr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gawguwhgg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gssqnrdnl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gbbaawpqu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.vehdjk.com/Article/details/gtthjlgbx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.tarul.cn/Article/details/ghmqdfuui.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/giwwcdats.sHtML

Q SQL 专题                              90
来源：http://blog.sjlbkw.cn/Article/details/gjkckittz.sHtML

R Bash 专题                             80
来源：http://3g.sjlbkw.cn/Article/details/gyzdpfxsb.sHtML

S C / C++ 专题                          60
来源：http://m.share.yfazqb.com/Article/details/gpmixcrvj.sHtML

T 其他语言补充                          60
来源：http://baike.vehdjk.com/Article/details/gxybvgwoc.sHtML

U 高频实用片段                         120
来源：http://www.m.share.yfazqb.com/Article/details/ggzghvbbq.sHtML

------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gcodjwzha.sHtML

合计                                  2106 条
来源：http://read.share.vehdjk.com/Article/details/gxysqcxav.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gugnnlnfa.sHtML


<!-- 参考信息 -->