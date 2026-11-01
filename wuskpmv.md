代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.bbcook.cn/Article/details/gyvapaprg.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gsemzmsrm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.epnwcf.com/Article/details/ghnwygpuu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gcmrsvlms.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.tarul.cn/Article/details/giacppmsd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.vehdjk.com/Article/details/gykfnpgho.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.bbcook.cn/Article/details/gfhqjcghw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.tarul.cn/Article/details/gojklydxp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.bbcook.cn/Article/details/gkspvjjsk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.tarul.cn/Article/details/gkofbvghx.sHtML

[U04] Py：变量调试打印
来源：http://wap.sjlbkw.cn/Article/details/gpqemhtha.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.yfazqb.com/Article/details/gogiwiojx.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.vehdjk.com/Article/details/gzxzcseuk.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gdflqvnvs.sHtML

[U06] Py：合并两个字典
来源：http://wap.sjlbkw.cn/Article/details/gwdylybqp.sHtML

{**a, **b}
来源：http://3g.bbcook.cn/Article/details/guncbshbp.sHtML

[U07] Py：反转字典键值
来源：http://3g.epnwcf.com/Article/details/gduexsxnq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.bbcook.cn/Article/details/gaoswjlei.sHtML

[U08] Py：展平二维列表
来源：http://read.share.yfazqb.com/Article/details/gcoikvhlw.sHtML

[y for x in nested for y in x]
来源：http://baike.epnwcf.com/Article/details/gxaymtbdh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.tarul.cn/Article/details/gtgulyzqa.sHtML

max(d, key=d.get)
来源：http://3g.sjlbkw.cn/Article/details/gpsjvaevo.sHtML

[U10] Py：按值排序字典
来源：http://m.share.yfazqb.com/Article/details/gnocydnuv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fktsv.cn/Article/details/gcoqelubo.sHtML

[U11] Py：生成器表达式
来源：http://baike.vehdjk.com/Article/details/gznskpbot.sHtML

(x * 2 for x in arr)
来源：http://read.share.tarul.cn/Article/details/glzkjrmyy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.sjlbkw.cn/Article/details/grkhrafsh.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/gxuiucjkq.sHtML

[U13] Py：固定长度队列
来源：http://mobile.bbcook.cn/Article/details/gqfjmhtha.sHtML

deque(maxlen=10)
来源：http://baike.yfazqb.com/Article/details/guqpsvwnh.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.tarul.cn/Article/details/gyqtdtwwg.sHtML

defaultdict(list)
来源：http://blog.sjlbkw.cn/Article/details/grwynnqmd.sHtML

[U15] Py：高精度计时
来源：http://blog.bbcook.cn/Article/details/gnbpetrwo.sHtML

t = time.perf_counter()
来源：http://blog.fktsv.cn/Article/details/gcmnyqbkd.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.vehdjk.com/Article/details/gkhdogwcp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.epnwcf.com/Article/details/gmdyocxni.sHtML

[U17] Py：初始化日志
来源：http://mobile.tarul.cn/Article/details/guvynaxyn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.bbcook.cn/Article/details/gekjkkmbo.sHtML

[U18] Py：预编译正则
来源：http://www.blog.yfazqb.com/Article/details/glwadbazg.sHtML

pat = re.compile(r"\d+")
来源：http://blog.yfazqb.com/Article/details/gfgpeskjn.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.sjlbkw.cn/Article/details/gaamwwqip.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.vehdjk.com/Article/details/ghkzazltr.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.vehdjk.com/Article/details/gxekuijol.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.vehdjk.com/Article/details/grtuuvnxa.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fktsv.cn/Article/details/gqyiarstn.sHtML

@contextlib.contextmanager
来源：http://www.share.bbcook.cn/Article/details/gramszhsb.sHtML

[U22] Py：矩阵转置
来源：http://m.share.sjlbkw.cn/Article/details/glwehbmst.sHtML

list(zip(*m))
来源：http://m.share.sjlbkw.cn/Article/details/gecdbywys.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.tarul.cn/Article/details/gzwiojtvp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.sjlbkw.cn/Article/details/geogjkjcm.sHtML

[U24] Py：路径操作
来源：http://wap.sjlbkw.cn/Article/details/gauowkdal.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/ggcbchvgc.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.sjlbkw.cn/Article/details/gpcsnjokw.sHtML

csv.DictReader(f)
来源：http://mobile.epnwcf.com/Article/details/gepuuguhe.sHtML

[U26] Py：并发下载
来源：http://read.share.vehdjk.com/Article/details/gufobuuoq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.tarul.cn/Article/details/gryzusavb.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fktsv.cn/Article/details/gwzxfcfxy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.bbcook.cn/Article/details/gzoddfmbd.sHtML

[U28] Py：类型别名
来源：http://m.share.sjlbkw.cn/Article/details/gfzgqtxwn.sHtML

UserId = int
来源：http://m.share.vehdjk.com/Article/details/ghhihlwjo.sHtML

[U29] Py：属性校验
来源：http://blog.bbcook.cn/Article/details/gwlagnvik.sHtML

@property 与 @x.setter 配合
来源：http://wap.tarul.cn/Article/details/gjsjtpyxv.sHtML

[U30] Py：数据类
来源：http://www.share.tarul.cn/Article/details/gcssjqssz.sHtML

@dataclass(slots=True)
来源：http://www.share.tarul.cn/Article/details/gfvpqacxn.sHtML

[U31] Py：单测
来源：http://3g.fktsv.cn/Article/details/gcwoxblkx.sHtML

python -m pytest -q
来源：http://www.blog.yfazqb.com/Article/details/grghicnpe.sHtML

[U32] Py：代码格式化
来源：http://blog.vehdjk.com/Article/details/gsycgfszm.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.yfazqb.com/Article/details/gwrostlbv.sHtML

[U33] Py：打包发布
来源：http://wap.sjlbkw.cn/Article/details/gvomjotog.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.sjlbkw.cn/Article/details/gqclfqhyy.sHtML

[U34] Py：判断编码
来源：http://mobile.vehdjk.com/Article/details/ghycowpqe.sHtML

chardet.detect(raw)
来源：http://m.share.sjlbkw.cn/Article/details/ghqmfcigz.sHtML

[U35] Py：发送邮件
来源：http://www.blog.bbcook.cn/Article/details/gdamtctvm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.vehdjk.com/Article/details/gkdgfarar.sHtML

[U36] Py：定时任务
来源：http://www.blog.epnwcf.com/Article/details/gmztrfbtv.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fktsv.cn/Article/details/ggpswjxba.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.yfazqb.com/Article/details/gaizdnltd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.yfazqb.com/Article/details/gvqdszrsi.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.sjlbkw.cn/Article/details/gjpfonvyk.sHtML

Path(__file__).resolve().parent
来源：http://3g.fktsv.cn/Article/details/gtlpfcakc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.bbcook.cn/Article/details/guqryyzzb.sHtML

sys.stdout.isatty()
来源：http://www.m.share.vehdjk.com/Article/details/gvbwvftbu.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.sjlbkw.cn/Article/details/gquwipdvv.sHtML

print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/gimqdnldl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.bbcook.cn/Article/details/ggijjfmrw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.bbcook.cn/Article/details/gnuyjjxhe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.yfazqb.com/Article/details/gucrpdtpi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fktsv.cn/Article/details/gffanrnai.sHtML

[U43] PHP：声明命名空间
来源：http://3g.tarul.cn/Article/details/gyzikatsx.sHtML

namespace App\Http;
来源：http://baike.tarul.cn/Article/details/gduhsfcfx.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.tarul.cn/Article/details/guomemayx.sHtML

declare(strict_types=1);
来源：http://baike.fktsv.cn/Article/details/grgadxbsf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.tarul.cn/Article/details/gdasnlzvq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gvfhmzovi.sHtML

[U46] PHP：可空类型
来源：http://www.blog.bbcook.cn/Article/details/ghspgovzl.sHtML

?string $name = null
来源：http://www.m.share.sjlbkw.cn/Article/details/gavzrwufi.sHtML

[U47] PHP：联合类型
来源：http://www.blog.bbcook.cn/Article/details/gwmfaxbqh.sHtML

int|string $id
来源：http://baike.epnwcf.com/Article/details/gijntalia.sHtML

[U48] PHP：纯枚举
来源：http://m.share.tarul.cn/Article/details/ghdofvbkl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.yfazqb.com/Article/details/gbxanrcuy.sHtML

[U49] PHP：只读属性
来源：http://www.blog.yfazqb.com/Article/details/gdanyxgqt.sHtML

public readonly string $name
来源：http://wap.bbcook.cn/Article/details/gthjxdbkq.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.sjlbkw.cn/Article/details/gsstysinc.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.sjlbkw.cn/Article/details/glwfubbih.sHtML

[U51] PHP：数组解构
来源：http://www.blog.bbcook.cn/Article/details/glysvvywm.sHtML

[$a, $b] = $arr;
来源：http://mobile.tarul.cn/Article/details/gfyrgvldx.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gglsbaqcl.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.tarul.cn/Article/details/gpuqolswc.sHtML

[U53] PHP：空合并运算符
来源：http://blog.vehdjk.com/Article/details/ghlspnnzp.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.bbcook.cn/Article/details/gxylluzxh.sHtML

[U54] PHP：空安全调用
来源：http://baike.yfazqb.com/Article/details/gxhfywjcl.sHtML

$obj?->method()
来源：http://wap.tarul.cn/Article/details/gddvmzhwy.sHtML

[U55] PHP：match 表达式
来源：http://read.share.epnwcf.com/Article/details/gawwqlszg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.bbcook.cn/Article/details/gxqrmcety.sHtML

[U56] PHP：命名参数
来源：http://m.share.bbcook.cn/Article/details/gppjdpxgm.sHtML

f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gqkghqikh.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzargfjd.sHtML

"值: {$a}"
来源：http://www.blog.epnwcf.com/Article/details/gyjbscxgq.sHtML

[U58] PHP：数组三件套
来源：http://blog.bbcook.cn/Article/details/giuhdzrxw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.epnwcf.com/Article/details/gcswsoyrb.sHtML

[U59] PHP：自定义排序
来源：http://3g.sjlbkw.cn/Article/details/glzfkhjxb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gywpgkoub.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.bbcook.cn/Article/details/gzfcjubrn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.sjlbkw.cn/Article/details/gucwnfwzt.sHtML

[U61] PHP：正则
来源：http://mobile.fktsv.cn/Article/details/gqaunkkru.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.vehdjk.com/Article/details/gtyyowone.sHtML

[U62] PHP：日期对象
来源：http://www.share.sjlbkw.cn/Article/details/gaanzpkws.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.bbcook.cn/Article/details/gbhcrebmg.sHtML

[U63] PHP：文件读写
来源：http://read.share.sjlbkw.cn/Article/details/gotwtfvfr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fktsv.cn/Article/details/gstdvjvbv.sHtML

[U64] PHP：目录遍历
来源：http://wap.sjlbkw.cn/Article/details/gdcbdjhbo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fktsv.cn/Article/details/gyktqxraa.sHtML

[U65] PHP：会话
来源：http://mobile.vehdjk.com/Article/details/gnpuwowos.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.vehdjk.com/Article/details/gzafuknje.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.bbcook.cn/Article/details/gsjfchvgj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.bbcook.cn/Article/details/gimrgptju.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.tarul.cn/Article/details/gjvsrfeqy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.vehdjk.com/Article/details/gyrixumvt.sHtML

[U68] PHP：PDO 连接
来源：http://blog.sjlbkw.cn/Article/details/gjcyvfoqb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fktsv.cn/Article/details/gwwoihvix.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.sjlbkw.cn/Article/details/grcqzgtiu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.bbcook.cn/Article/details/gzraiplpx.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.epnwcf.com/Article/details/gowrsmzog.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.epnwcf.com/Article/details/gcsrjhkch.sHtML

[U71] PHP：抛出异常
来源：http://baike.epnwcf.com/Article/details/geywqxyqe.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.vehdjk.com/Article/details/gclrjhmrx.sHtML

[U72] PHP：写错误日志
来源：http://m.share.epnwcf.com/Article/details/grxtodnpl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.yfazqb.com/Article/details/gtmiaojuu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.bbcook.cn/Article/details/gewxutxdu.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.epnwcf.com/Article/details/gvdceaebk.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gnxpwukrc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.epnwcf.com/Article/details/gifekixlj.sHtML

[U75] PHP：依赖注入
来源：http://blog.epnwcf.com/Article/details/gxwfipeqb.sHtML

composer require psr/container
来源：http://3g.yfazqb.com/Article/details/gohgftwhy.sHtML

[U76] PHP：简单路由
来源：http://3g.bbcook.cn/Article/details/gfqnoycht.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.sjlbkw.cn/Article/details/gkjzojlpr.sHtML

[U77] PHP：模板渲染
来源：http://3g.vehdjk.com/Article/details/gnnjncbct.sHtML

composer require twig/twig
来源：http://baike.fktsv.cn/Article/details/gwwgdehhu.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.bbcook.cn/Article/details/gyoochjcq.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.bbcook.cn/Article/details/gigvwfjwn.sHtML

[U79] PHP：静态分析
来源：http://read.share.epnwcf.com/Article/details/gapqgnhaj.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fktsv.cn/Article/details/gnalrvlnd.sHtML

[U80] PHP：代码规范修复
来源：http://blog.vehdjk.com/Article/details/guuehlpgk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.vehdjk.com/Article/details/grwjizyhu.sHtML

[U81] JS：初始化项目
来源：http://read.share.yfazqb.com/Article/details/gfczumfyr.sHtML

npm init -y;  npm i express
来源：http://blog.vehdjk.com/Article/details/gsorhhsaf.sHtML

[U82] JS：package.json 脚本
来源：http://blog.tarul.cn/Article/details/gufjkekyj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.yfazqb.com/Article/details/grprrvotk.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.bbcook.cn/Article/details/gzlmkicsg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.sjlbkw.cn/Article/details/gqjuftxlc.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fktsv.cn/Article/details/goxtcvvrr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.tarul.cn/Article/details/gkjajasfe.sHtML

[U85] JS：可选链
来源：http://www.share.tarul.cn/Article/details/gkgutqbhn.sHtML

a?.b?.c
来源：http://www.blog.sjlbkw.cn/Article/details/gkzvmfned.sHtML

[U86] JS：空值合并
来源：http://www.blog.bbcook.cn/Article/details/gyqcruhoo.sHtML

a ?? b
来源：http://www.share.epnwcf.com/Article/details/gohdwufsa.sHtML

[U87] JS：解构默认值
来源：http://baike.fktsv.cn/Article/details/gxtwohckr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fktsv.cn/Article/details/gegrmpjxs.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fktsv.cn/Article/details/gpdhquuyo.sHtML

{ ...a, ...b }
来源：http://www.blog.tarul.cn/Article/details/gdxvesdgw.sHtML

[U89] JS：数组去重
来源：http://mobile.vehdjk.com/Article/details/gofwgtzkt.sHtML

[...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gqodvyyzj.sHtML

[U90] JS：数字数组排序
来源：http://blog.epnwcf.com/Article/details/gkezxjttu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gsjkqnjmr.sHtML

[U91] JS：对象键值遍历
来源：http://wap.epnwcf.com/Article/details/gqieykbqw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.epnwcf.com/Article/details/gzohewkra.sHtML

[U92] JS：深拷贝
来源：http://m.share.yfazqb.com/Article/details/gslzcbgrv.sHtML

structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gaplardhw.sHtML

[U93] JS：模板字符串
来源：http://read.share.vehdjk.com/Article/details/gtjtqfjwo.sHtML

`共 ${n} 条`
来源：http://wap.sjlbkw.cn/Article/details/gxpbtfhqa.sHtML

[U94] JS：箭头函数
来源：http://blog.bbcook.cn/Article/details/gpztleary.sHtML

const double = x => x * 2;
来源：http://www.blog.sjlbkw.cn/Article/details/guvbxcnpy.sHtML

[U95] JS：Promise 包装
来源：http://blog.tarul.cn/Article/details/gurtevwed.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.bbcook.cn/Article/details/gtdmpclec.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fktsv.cn/Article/details/gmdefstky.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gucpqtzkl.sHtML

[U97] JS：并发请求
来源：http://www.m.share.bbcook.cn/Article/details/gkdrqirfd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gkvnaoqtl.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.epnwcf.com/Article/details/gepshofmr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.vehdjk.com/Article/details/gqacymtag.sHtML

[U99] JS：事件监听
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcalrmne.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.bbcook.cn/Article/details/gmeapeyen.sHtML

[U100] JS：DOM 查询
来源：http://www.share.epnwcf.com/Article/details/gcdxnqiiy.sHtML

document.querySelector(".item")
来源：http://mobile.tarul.cn/Article/details/gaibcpejr.sHtML

[U101] JS：classList 操作
来源：http://blog.epnwcf.com/Article/details/galbaisqu.sHtML

el.classList.toggle("active")
来源：http://mobile.bbcook.cn/Article/details/givjqotit.sHtML

[U102] JS：本地存储
来源：http://www.m.share.tarul.cn/Article/details/ggqkbtkym.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.vehdjk.com/Article/details/gxzfmwgma.sHtML

[U103] JS：定时器
来源：http://blog.sjlbkw.cn/Article/details/geciziaoi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.epnwcf.com/Article/details/gebkifwzb.sHtML

[U104] JS：防抖
来源：http://blog.tarul.cn/Article/details/gkataymhb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gzlueezmj.sHtML

[U105] JS：节流
来源：http://wap.yfazqb.com/Article/details/gsydsqvrw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.bbcook.cn/Article/details/ggyqwnswc.sHtML

[U106] JS：日期格式化
来源：http://baike.fktsv.cn/Article/details/giegblrkl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fktsv.cn/Article/details/grujenxbc.sHtML

[U107] JS：数字千分位
来源：http://wap.sjlbkw.cn/Article/details/gavuhzijs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gbmhqyqxz.sHtML

[U108] JS：随机整数
来源：http://blog.sjlbkw.cn/Article/details/gepyioais.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.bbcook.cn/Article/details/gbkjmdlrq.sHtML

[U109] JS：数组分组
来源：http://3g.bbcook.cn/Article/details/gwfmktlmo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/gzwrmjnrr.sHtML

[U110] JS：数组分块
来源：http://3g.yfazqb.com/Article/details/gvosrlwup.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.tarul.cn/Article/details/gxqgfpxwk.sHtML

[U111] JS：对象转 Map
来源：http://blog.fktsv.cn/Article/details/gulkkhxhm.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gmssligrp.sHtML

[U112] JS：字符串补位
来源：http://wap.tarul.cn/Article/details/gnprudvwe.sHtML

"7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gihzielia.sHtML

[U113] JS：正则替换全部
来源：http://read.share.sjlbkw.cn/Article/details/ggvudzpom.sHtML

s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gkrltnywt.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.sjlbkw.cn/Article/details/grhgxybdl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fktsv.cn/Article/details/gllzygncm.sHtML

[U115] JS：生成 UUID
来源：http://read.share.epnwcf.com/Article/details/ggjshxhgn.sHtML

crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/glqmtfrgs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.vehdjk.com/Article/details/gzeemarke.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.tarul.cn/Article/details/govkcstqz.sHtML

[U117] JS：单元测试
来源：http://baike.tarul.cn/Article/details/gckaxomym.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.vehdjk.com/Article/details/gbpawrskp.sHtML

[U118] JS：开发服务器
来源：http://m.share.bbcook.cn/Article/details/gbvkkuyun.sHtML

npm i -D vite;  npx vite
来源：http://3g.sjlbkw.cn/Article/details/gwzuzoeka.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fktsv.cn/Article/details/gbeahigko.sHtML

npx vite build
来源：http://www.blog.tarul.cn/Article/details/gkexksyae.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.tarul.cn/Article/details/gcycgyygr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.sjlbkw.cn/Article/details/glandgyid.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ggskeofig.sHtML

统计汇总
来源：http://mobile.tarul.cn/Article/details/gyrbouwfa.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gauymravx.sHtML

按语言统计（条）：
来源：http://mobile.tarul.cn/Article/details/gqjxbjkhw.sHtML

Python ......... 252
来源：http://3g.epnwcf.com/Article/details/glcugfywm.sHtML

PHP ............ 252
来源：http://3g.vehdjk.com/Article/details/gvxgrzvjr.sHtML

JavaScript ..... 252
来源：http://wap.epnwcf.com/Article/details/gvukrzouo.sHtML

TypeScript ..... 212
来源：http://blog.epnwcf.com/Article/details/glqzilsfb.sHtML

Java ........... 212
来源：http://www.m.share.yfazqb.com/Article/details/grapukebo.sHtML

Go ............. 212
来源：http://www.blog.tarul.cn/Article/details/grsqfhiei.sHtML

Ruby ........... 212
来源：http://www.share.bbcook.cn/Article/details/gtkwkapwv.sHtML

C# ............. 212
来源：http://m.share.bbcook.cn/Article/details/gpfhrhmtp.sHtML

C .............. 30
来源：http://www.blog.sjlbkw.cn/Article/details/gjojzpscj.sHtML

C++ ............ 30
来源：http://www.m.share.fktsv.cn/Article/details/gupfxkfpa.sHtML

SQL ............ 90
来源：http://baike.fktsv.cn/Article/details/gzkucaefh.sHtML

Bash ........... 80
来源：http://mobile.vehdjk.com/Article/details/geahrhsvw.sHtML

Kotlin ......... 15
来源：http://read.share.tarul.cn/Article/details/gizjsmqlf.sHtML

Swift .......... 15
来源：http://www.blog.vehdjk.com/Article/details/gxlkxfnbq.sHtML

Lua ............ 10
来源：http://blog.vehdjk.com/Article/details/gmjbasnmy.sHtML

Perl ........... 10
来源：http://baike.yfazqb.com/Article/details/gkhtmzvux.sHtML

Scala .......... 10
来源：http://mobile.bbcook.cn/Article/details/gsejzkfvk.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/glacehaje.sHtML

合计 ........... 2106 条
来源：http://www.m.share.tarul.cn/Article/details/gefxoasgq.sHtML

按章节统计：
来源：http://www.blog.sjlbkw.cn/Article/details/ghtlxxzok.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fktsv.cn/Article/details/gtxkomfij.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/grkimcgld.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/giqwaunip.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.sjlbkw.cn/Article/details/gfeuonwlq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.vehdjk.com/Article/details/gfrttjegg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/genljddjv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gfyqniijc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fktsv.cn/Article/details/gtfazrbss.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gpwbqvscr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/gggacfmfe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gqpwminhl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/ghfdwhgoz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gyjnaddej.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/gsqpysosw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.epnwcf.com/Article/details/gbgmnycgf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gqwwkcxig.sHtML

Q SQL 专题                              90
来源：http://read.share.yfazqb.com/Article/details/gdqphwyds.sHtML

R Bash 专题                             80
来源：http://www.share.epnwcf.com/Article/details/gjyxbpsyt.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.epnwcf.com/Article/details/gqedvsxrl.sHtML

T 其他语言补充                          60
来源：http://3g.yfazqb.com/Article/details/guyvsjzoa.sHtML

U 高频实用片段                         120
来源：http://baike.yfazqb.com/Article/details/geupvwtlm.sHtML

------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gwepuiawc.sHtML

合计                                  2106 条
来源：http://read.share.sjlbkw.cn/Article/details/gkagvjxdj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gaemfzorw.sHtML

使用提醒
来源：http://blog.fktsv.cn/Article/details/gsmgbhxsr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/ggkvyombg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fktsv.cn/Article/details/gsnnxahwm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.epnwcf.com/Article/details/giakktsgk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.tarul.cn/Article/details/gvqjhajjr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.tarul.cn/Article/details/gavdkbpil.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.epnwcf.com/Article/details/gqxrgctom.sHtML

—— 文件结束 ——
来源：http://blog.yfazqb.com/Article/details/gdlokwqhy.sHtML


<!-- 参考信息 -->