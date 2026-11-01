代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://blog.vehdjk.com/Article/details/giaglqjcc.sHtML

[T59] Scala：循环
来源：http://mobile.epnwcf.com/Article/details/guphfyyhe.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gzptjnyxq.sHtML

[T60] Scala：折叠
来源：http://mobile.epnwcf.com/Article/details/gbcvkmzlt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.vehdjk.com/Article/details/gqjedercx.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmeliujzo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gucpymdag.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gitayoisg.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.sjlbkw.cn/Article/details/gfqprufyn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fktsv.cn/Article/details/gryuszeow.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.bbcook.cn/Article/details/ghenkuinj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.vehdjk.com/Article/details/gemhdzwhr.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.bbcook.cn/Article/details/ghykbiafx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.vehdjk.com/Article/details/gwsfkjbcp.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/gegfbvsyr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.bbcook.cn/Article/details/ghbbkheze.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.epnwcf.com/Article/details/gneajekov.sHtML

list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gynagbaxn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fktsv.cn/Article/details/gowxbdovm.sHtML

{**a, **b}
来源：http://baike.bbcook.cn/Article/details/gsvxidzft.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.vehdjk.com/Article/details/garcpcdsz.sHtML

{v: k for k, v in d.items()}
来源：http://baike.yfazqb.com/Article/details/gszrusiyr.sHtML

[U08] Py：展平二维列表
来源：http://3g.fktsv.cn/Article/details/gfrvdelpg.sHtML

[y for x in nested for y in x]
来源：http://read.share.vehdjk.com/Article/details/gmdksicim.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.tarul.cn/Article/details/grgufrumw.sHtML

max(d, key=d.get)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcuajskm.sHtML

[U10] Py：按值排序字典
来源：http://blog.epnwcf.com/Article/details/gjqyapmre.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fktsv.cn/Article/details/gsivncxgs.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.tarul.cn/Article/details/gzojumvgn.sHtML

(x * 2 for x in arr)
来源：http://www.share.fktsv.cn/Article/details/gurgmnqaw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.tarul.cn/Article/details/gdwjydply.sHtML

Counter(arr).most_common(3)
来源：http://baike.tarul.cn/Article/details/grrkykvdv.sHtML

[U13] Py：固定长度队列
来源：http://mobile.yfazqb.com/Article/details/gfwicnlfq.sHtML

deque(maxlen=10)
来源：http://m.share.vehdjk.com/Article/details/gicmpmuui.sHtML

[U14] Py：分组收集到列表
来源：http://blog.bbcook.cn/Article/details/gypormugh.sHtML

defaultdict(list)
来源：http://m.share.tarul.cn/Article/details/gjoddcfug.sHtML

[U15] Py：高精度计时
来源：http://read.share.epnwcf.com/Article/details/gbkpftufz.sHtML

t = time.perf_counter()
来源：http://baike.yfazqb.com/Article/details/gogzxwdpc.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.epnwcf.com/Article/details/gxkiwmstn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.tarul.cn/Article/details/gsniaubeb.sHtML

[U17] Py：初始化日志
来源：http://3g.fktsv.cn/Article/details/gpfwleiwo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.tarul.cn/Article/details/gucaazrxo.sHtML

[U18] Py：预编译正则
来源：http://m.share.yfazqb.com/Article/details/gzmuobugb.sHtML

pat = re.compile(r"\d+")
来源：http://baike.yfazqb.com/Article/details/gikgnztvd.sHtML

[U19] Py：正则替换带回调
来源：http://3g.yfazqb.com/Article/details/gleddehgr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.vehdjk.com/Article/details/gssqdamdf.sHtML

[U20] Py：缓存函数结果
来源：http://baike.vehdjk.com/Article/details/gaulpwdox.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.vehdjk.com/Article/details/gbujaozfj.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.tarul.cn/Article/details/gxpzbctjd.sHtML

@contextlib.contextmanager
来源：http://blog.bbcook.cn/Article/details/gmiqsttpq.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.tarul.cn/Article/details/gcbyjvexk.sHtML

list(zip(*m))
来源：http://3g.sjlbkw.cn/Article/details/gswhgrqvq.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.bbcook.cn/Article/details/gkkfmftle.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.vehdjk.com/Article/details/gytbvxsjx.sHtML

[U24] Py：路径操作
来源：http://www.share.yfazqb.com/Article/details/gajuzjvpi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/gjiwqlxpp.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.bbcook.cn/Article/details/gaurujqjv.sHtML

csv.DictReader(f)
来源：http://3g.epnwcf.com/Article/details/ggbadnyjf.sHtML

[U26] Py：并发下载
来源：http://baike.bbcook.cn/Article/details/goxbbiozd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.tarul.cn/Article/details/givdhwpkw.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.sjlbkw.cn/Article/details/gxaooecbn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.yfazqb.com/Article/details/glteppqeg.sHtML

[U28] Py：类型别名
来源：http://www.share.sjlbkw.cn/Article/details/goelkyfrl.sHtML

UserId = int
来源：http://3g.vehdjk.com/Article/details/ghhzbjxdu.sHtML

[U29] Py：属性校验
来源：http://read.share.bbcook.cn/Article/details/gpzrqljtm.sHtML

@property 与 @x.setter 配合
来源：http://baike.sjlbkw.cn/Article/details/grvtlmodt.sHtML

[U30] Py：数据类
来源：http://mobile.yfazqb.com/Article/details/gjrdtcfiy.sHtML

@dataclass(slots=True)
来源：http://wap.vehdjk.com/Article/details/gwssslpjq.sHtML

[U31] Py：单测
来源：http://www.blog.fktsv.cn/Article/details/gyignbwyi.sHtML

python -m pytest -q
来源：http://baike.fktsv.cn/Article/details/ggienovgf.sHtML

[U32] Py：代码格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gebsulwdm.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.yfazqb.com/Article/details/gyzxkxobf.sHtML

[U33] Py：打包发布
来源：http://www.m.share.epnwcf.com/Article/details/ggtsgfpoc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.yfazqb.com/Article/details/gjppvktli.sHtML

[U34] Py：判断编码
来源：http://read.share.epnwcf.com/Article/details/gpxgfevpr.sHtML

chardet.detect(raw)
来源：http://m.share.sjlbkw.cn/Article/details/gliqrvpsm.sHtML

[U35] Py：发送邮件
来源：http://www.blog.sjlbkw.cn/Article/details/gxlabehbb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.yfazqb.com/Article/details/gyfcjmjhh.sHtML

[U36] Py：定时任务
来源：http://wap.tarul.cn/Article/details/gjrdgzemm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.vehdjk.com/Article/details/gmklotavh.sHtML

[U37] Py：读写 Excel
来源：http://3g.bbcook.cn/Article/details/gokixparn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.yfazqb.com/Article/details/gufjjlhfg.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fktsv.cn/Article/details/gpjmjadjj.sHtML

Path(__file__).resolve().parent
来源：http://wap.bbcook.cn/Article/details/gprhigmnu.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.bbcook.cn/Article/details/gruifzxjl.sHtML

sys.stdout.isatty()
来源：http://www.share.bbcook.cn/Article/details/gqmyhuasd.sHtML

[U40] Py：打印到标准错误
来源：http://baike.bbcook.cn/Article/details/gzokgbvma.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gigzyalpg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.vehdjk.com/Article/details/gjkneaeeq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fktsv.cn/Article/details/gczyamewx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.epnwcf.com/Article/details/gwuuuvzqa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.epnwcf.com/Article/details/gvgdakdgt.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.sjlbkw.cn/Article/details/gdbwhossz.sHtML

namespace App\Http;
来源：http://m.share.fktsv.cn/Article/details/ggrcvejln.sHtML

[U44] PHP：开启严格类型
来源：http://wap.vehdjk.com/Article/details/gjwjfwhne.sHtML

declare(strict_types=1);
来源：http://www.share.vehdjk.com/Article/details/gxykxfnuf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.bbcook.cn/Article/details/gmvctvgkm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gvomtgmho.sHtML

[U46] PHP：可空类型
来源：http://read.share.tarul.cn/Article/details/gmoacseoo.sHtML

?string $name = null
来源：http://www.share.sjlbkw.cn/Article/details/gcfckguty.sHtML

[U47] PHP：联合类型
来源：http://read.share.epnwcf.com/Article/details/gmakvsvmw.sHtML

int|string $id
来源：http://www.share.epnwcf.com/Article/details/gbjgyrqaf.sHtML

[U48] PHP：纯枚举
来源：http://m.share.epnwcf.com/Article/details/gfiuxhaha.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.tarul.cn/Article/details/ghwwkzswm.sHtML

[U49] PHP：只读属性
来源：http://3g.sjlbkw.cn/Article/details/gtsocissn.sHtML

public readonly string $name
来源：http://www.m.share.epnwcf.com/Article/details/gpiukkwxx.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.yfazqb.com/Article/details/gihuxjpna.sHtML

public function __construct(private int $id) {}
来源：http://baike.bbcook.cn/Article/details/guhzoslve.sHtML

[U51] PHP：数组解构
来源：http://www.share.tarul.cn/Article/details/gyavmiwfj.sHtML

[$a, $b] = $arr;
来源：http://read.share.fktsv.cn/Article/details/ghetlkgyk.sHtML

[U52] PHP：箭头函数
来源：http://www.share.epnwcf.com/Article/details/grotafmxu.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.epnwcf.com/Article/details/gsocrubop.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.epnwcf.com/Article/details/gciksqdzt.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.epnwcf.com/Article/details/gfaubbjlv.sHtML

[U54] PHP：空安全调用
来源：http://wap.sjlbkw.cn/Article/details/gmlungqvt.sHtML

$obj?->method()
来源：http://m.share.tarul.cn/Article/details/goxsjewez.sHtML

[U55] PHP：match 表达式
来源：http://baike.tarul.cn/Article/details/gduwcsgfv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.epnwcf.com/Article/details/ghhhafyrj.sHtML

[U56] PHP：命名参数
来源：http://www.share.yfazqb.com/Article/details/gbksepots.sHtML

f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gvmdxkogo.sHtML

[U57] PHP：字符串插值
来源：http://blog.bbcook.cn/Article/details/gucnivwga.sHtML

"值: {$a}"
来源：http://wap.bbcook.cn/Article/details/gdmxfoqft.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.bbcook.cn/Article/details/gqnwvthea.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.tarul.cn/Article/details/gkspgrnqr.sHtML

[U59] PHP：自定义排序
来源：http://baike.tarul.cn/Article/details/gufjmolcc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.bbcook.cn/Article/details/gzhbtekwb.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.epnwcf.com/Article/details/gydzymjvq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fktsv.cn/Article/details/gltrndtbp.sHtML

[U61] PHP：正则
来源：http://read.share.yfazqb.com/Article/details/ggwnaplja.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.vehdjk.com/Article/details/gjgbuvdux.sHtML

[U62] PHP：日期对象
来源：http://m.share.tarul.cn/Article/details/gigbpolty.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.yfazqb.com/Article/details/gbrdaenfg.sHtML

[U63] PHP：文件读写
来源：http://m.share.bbcook.cn/Article/details/gdaswmgid.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.vehdjk.com/Article/details/gcynaemzw.sHtML

[U64] PHP：目录遍历
来源：http://3g.vehdjk.com/Article/details/gmxhnexos.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.vehdjk.com/Article/details/gezvcoalu.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/gobwvvwty.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.yfazqb.com/Article/details/gwbylsbzy.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fktsv.cn/Article/details/gvdmltwwu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.epnwcf.com/Article/details/gvmpqrcbf.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.epnwcf.com/Article/details/gambworzx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.bbcook.cn/Article/details/gojprugji.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.sjlbkw.cn/Article/details/gsnruiarw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.epnwcf.com/Article/details/gjlewlvak.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.epnwcf.com/Article/details/geqbhtazo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.bbcook.cn/Article/details/ghzenvwlj.sHtML

[U70] PHP：PDO 事务
来源：http://baike.yfazqb.com/Article/details/glvyexlky.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.sjlbkw.cn/Article/details/gelqlgzyi.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gzfjabgrd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.epnwcf.com/Article/details/guybcozpi.sHtML

[U72] PHP：写错误日志
来源：http://m.share.bbcook.cn/Article/details/golzwkokh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.sjlbkw.cn/Article/details/gahyycoog.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.epnwcf.com/Article/details/gqzwvadni.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.epnwcf.com/Article/details/gpzqnsbjc.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gdlpcweou.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.epnwcf.com/Article/details/gllnhlkaw.sHtML

[U75] PHP：依赖注入
来源：http://www.share.tarul.cn/Article/details/gmepgkyai.sHtML

composer require psr/container
来源：http://www.blog.tarul.cn/Article/details/gnxqmqyii.sHtML

[U76] PHP：简单路由
来源：http://3g.tarul.cn/Article/details/gejdyhncx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.yfazqb.com/Article/details/gaimypjeo.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fktsv.cn/Article/details/gebqerilh.sHtML

composer require twig/twig
来源：http://www.m.share.tarul.cn/Article/details/gsxpnigku.sHtML

[U78] PHP：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/gztkxdkzj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.sjlbkw.cn/Article/details/geeeiycpu.sHtML

[U79] PHP：静态分析
来源：http://blog.fktsv.cn/Article/details/gmwsjdjwi.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.vehdjk.com/Article/details/gvmudjbrm.sHtML

[U80] PHP：代码规范修复
来源：http://3g.vehdjk.com/Article/details/guyogukwf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.bbcook.cn/Article/details/gwcjyrjvq.sHtML

[U81] JS：初始化项目
来源：http://blog.fktsv.cn/Article/details/guvtfmlya.sHtML

npm init -y;  npm i express
来源：http://m.share.yfazqb.com/Article/details/gusemtocx.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.epnwcf.com/Article/details/gvalllnpe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fktsv.cn/Article/details/gungfreue.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.sjlbkw.cn/Article/details/gcvbembwz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/gggrcpaul.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.yfazqb.com/Article/details/gihtndeto.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.tarul.cn/Article/details/gtbhmusbg.sHtML

[U85] JS：可选链
来源：http://www.share.epnwcf.com/Article/details/gdjmfwkoi.sHtML

a?.b?.c
来源：http://wap.sjlbkw.cn/Article/details/gkddlalgy.sHtML

[U86] JS：空值合并
来源：http://read.share.bbcook.cn/Article/details/gbjpevjuq.sHtML

a ?? b
来源：http://blog.vehdjk.com/Article/details/gacsxznwx.sHtML

[U87] JS：解构默认值
来源：http://wap.fktsv.cn/Article/details/gqgcbaweg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.epnwcf.com/Article/details/ghmxhxodu.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.sjlbkw.cn/Article/details/gckjujbru.sHtML

{ ...a, ...b }
来源：http://3g.bbcook.cn/Article/details/gfwtztnmy.sHtML

[U89] JS：数组去重
来源：http://www.share.fktsv.cn/Article/details/gmypjgpsz.sHtML

[...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gijcbogqb.sHtML

[U90] JS：数字数组排序
来源：http://blog.epnwcf.com/Article/details/givcmseqo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gsqqwtlho.sHtML

[U91] JS：对象键值遍历
来源：http://wap.tarul.cn/Article/details/gbxlqqdnu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.vehdjk.com/Article/details/gqxejeqry.sHtML

[U92] JS：深拷贝
来源：http://www.share.yfazqb.com/Article/details/gtresefmm.sHtML

structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gklkulkrj.sHtML

[U93] JS：模板字符串
来源：http://www.blog.yfazqb.com/Article/details/gakvtlkic.sHtML

`共 ${n} 条`
来源：http://www.share.tarul.cn/Article/details/gwxrfesma.sHtML

[U94] JS：箭头函数
来源：http://www.share.bbcook.cn/Article/details/gwxndqgdd.sHtML

const double = x => x * 2;
来源：http://www.share.yfazqb.com/Article/details/gfxiurwmi.sHtML

[U95] JS：Promise 包装
来源：http://m.share.yfazqb.com/Article/details/gierrquls.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.vehdjk.com/Article/details/gimmovquj.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.epnwcf.com/Article/details/gsmpbwoza.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gakaebxdh.sHtML

[U97] JS：并发请求
来源：http://wap.epnwcf.com/Article/details/gvdyrzcdr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gnnijcxfg.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fktsv.cn/Article/details/gcnopsnwu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.vehdjk.com/Article/details/gtqzmtkbs.sHtML

[U99] JS：事件监听
来源：http://blog.yfazqb.com/Article/details/gqbiocukd.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.yfazqb.com/Article/details/gbklfrzhq.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fktsv.cn/Article/details/geibmzfvm.sHtML

document.querySelector(".item")
来源：http://m.share.fktsv.cn/Article/details/gdadmripq.sHtML

[U101] JS：classList 操作
来源：http://www.blog.tarul.cn/Article/details/gbcdtjlyg.sHtML

el.classList.toggle("active")
来源：http://wap.vehdjk.com/Article/details/gkhelqjfi.sHtML

[U102] JS：本地存储
来源：http://www.blog.sjlbkw.cn/Article/details/gjcysammu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.yfazqb.com/Article/details/gizyuhsvi.sHtML

[U103] JS：定时器
来源：http://mobile.bbcook.cn/Article/details/gkunypspy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.bbcook.cn/Article/details/gszjobbuo.sHtML

[U104] JS：防抖
来源：http://mobile.bbcook.cn/Article/details/gtfenrxla.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gawrinacd.sHtML

[U105] JS：节流
来源：http://read.share.tarul.cn/Article/details/glzzjsrvm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.sjlbkw.cn/Article/details/gitsebeea.sHtML

[U106] JS：日期格式化
来源：http://3g.vehdjk.com/Article/details/ggrhevtng.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.yfazqb.com/Article/details/gxvvdehrw.sHtML

[U107] JS：数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gdmvcxpbm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gqkolgmqc.sHtML

[U108] JS：随机整数
来源：http://mobile.epnwcf.com/Article/details/gjinztknv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdujllwc.sHtML

[U109] JS：数组分组
来源：http://mobile.yfazqb.com/Article/details/gzpjyqqgi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/gdfcjlhzg.sHtML

[U110] JS：数组分块
来源：http://3g.fktsv.cn/Article/details/gcxauvdbw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.epnwcf.com/Article/details/gbjxwknwz.sHtML

[U111] JS：对象转 Map
来源：http://3g.epnwcf.com/Article/details/gojanlzav.sHtML

new Map(Object.entries(obj))
来源：http://mobile.epnwcf.com/Article/details/gtqptyzvz.sHtML

[U112] JS：字符串补位
来源：http://baike.fktsv.cn/Article/details/gscgibatk.sHtML

"7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/ggdxdztco.sHtML

[U113] JS：正则替换全部
来源：http://read.share.epnwcf.com/Article/details/gomrusldt.sHtML

s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gvbfzqvxf.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.tarul.cn/Article/details/giuzmbzzy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.bbcook.cn/Article/details/ggfupquup.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmhgdfoo.sHtML

crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/grtazfeoc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fktsv.cn/Article/details/gojtyqspt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.yfazqb.com/Article/details/godphajrr.sHtML

[U117] JS：单元测试
来源：http://mobile.fktsv.cn/Article/details/gczhpxiya.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.tarul.cn/Article/details/gsbeydhqf.sHtML

[U118] JS：开发服务器
来源：http://read.share.epnwcf.com/Article/details/grdrodhmz.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.sjlbkw.cn/Article/details/guveahhva.sHtML

[U119] JS：生产构建
来源：http://mobile.vehdjk.com/Article/details/gvbwoajzk.sHtML

npx vite build
来源：http://read.share.yfazqb.com/Article/details/gqjvjhzql.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.sjlbkw.cn/Article/details/gvwlfappv.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.vehdjk.com/Article/details/ggaocpada.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gdjapdsvm.sHtML

统计汇总
来源：http://www.m.share.bbcook.cn/Article/details/goujbfycr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbhmjeaff.sHtML

按语言统计（条）：
来源：http://blog.yfazqb.com/Article/details/gydcfzmhn.sHtML

Python ......... 252
来源：http://mobile.sjlbkw.cn/Article/details/gvlvlllny.sHtML

PHP ............ 252
来源：http://mobile.bbcook.cn/Article/details/gqlrjflft.sHtML

JavaScript ..... 252
来源：http://blog.bbcook.cn/Article/details/gzoujpbcr.sHtML

TypeScript ..... 212
来源：http://www.share.epnwcf.com/Article/details/gwzntzfok.sHtML

Java ........... 212
来源：http://www.share.vehdjk.com/Article/details/gelbizrus.sHtML

Go ............. 212
来源：http://www.m.share.yfazqb.com/Article/details/ggupvhenx.sHtML

Ruby ........... 212
来源：http://mobile.yfazqb.com/Article/details/gmmlaktqi.sHtML

C# ............. 212
来源：http://blog.yfazqb.com/Article/details/gmainhqfu.sHtML

C .............. 30
来源：http://baike.vehdjk.com/Article/details/gfxgpuwen.sHtML

C++ ............ 30
来源：http://www.m.share.tarul.cn/Article/details/grjrazafu.sHtML

SQL ............ 90
来源：http://wap.fktsv.cn/Article/details/givlrtciu.sHtML

Bash ........... 80
来源：http://wap.bbcook.cn/Article/details/gzzceybsq.sHtML

Kotlin ......... 15
来源：http://mobile.vehdjk.com/Article/details/gmzsjdfqa.sHtML

Swift .......... 15
来源：http://mobile.fktsv.cn/Article/details/ggwmofbjd.sHtML

Lua ............ 10
来源：http://3g.tarul.cn/Article/details/gnmhpoola.sHtML

Perl ........... 10
来源：http://read.share.sjlbkw.cn/Article/details/gzjbdbgot.sHtML

Scala .......... 10
来源：http://blog.tarul.cn/Article/details/gdypvpsvz.sHtML

------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gzmhrxdyt.sHtML

合计 ........... 2106 条
来源：http://blog.tarul.cn/Article/details/gsgeukehj.sHtML

按章节统计：
来源：http://3g.bbcook.cn/Article/details/gjazfkaxw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.yfazqb.com/Article/details/gowsdztcm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/gagccdigq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/gwkwxeeku.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.vehdjk.com/Article/details/gfopocvya.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fktsv.cn/Article/details/gibjwyqwx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fktsv.cn/Article/details/gvavvxtza.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/gtagtyftc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gzckzrbsu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gxgsqwugv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fktsv.cn/Article/details/gliqsbgub.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gcnmlvazf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gjnbstwid.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gaideaaga.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/gtndunnby.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.yfazqb.com/Article/details/gzcsxmzao.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/ggizjwaie.sHtML

Q SQL 专题                              90
来源：http://www.share.epnwcf.com/Article/details/gwiyafghv.sHtML

R Bash 专题                             80
来源：http://www.blog.bbcook.cn/Article/details/ghahziohp.sHtML

S C / C++ 专题                          60
来源：http://3g.sjlbkw.cn/Article/details/gnkjcgfms.sHtML

T 其他语言补充                          60
来源：http://blog.sjlbkw.cn/Article/details/gxwjmxwtf.sHtML

U 高频实用片段                         120
来源：http://wap.fktsv.cn/Article/details/guapfsyml.sHtML

------------------------------------
来源：http://m.share.epnwcf.com/Article/details/godxkyrdm.sHtML

合计                                  2106 条
来源：http://wap.fktsv.cn/Article/details/gprzwuwlm.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gjqlkusxa.sHtML

使用提醒
来源：http://www.m.share.tarul.cn/Article/details/grdjjctvq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gjcrmywoo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.bbcook.cn/Article/details/gztgvkhkk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fktsv.cn/Article/details/greitnuhr.sHtML


<!-- 参考信息 -->