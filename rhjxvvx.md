代发 wailian999

[U01] Py：创建虚拟环境
来源：http://baike.yfazqb.com/Article/details/gegczqpcc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.bbcook.cn/Article/details/gxoztuzzu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fktsv.cn/Article/details/gqdigeumn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.tarul.cn/Article/details/guopgdxic.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.bbcook.cn/Article/details/gremujvti.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.tarul.cn/Article/details/gzuxpxdpj.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.tarul.cn/Article/details/geavarbrh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.yfazqb.com/Article/details/ganublita.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.tarul.cn/Article/details/gviyhvuno.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/ghbnlgjfn.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.bbcook.cn/Article/details/gvmsejnng.sHtML

{**a, **b}
来源：http://m.share.tarul.cn/Article/details/goamylgkj.sHtML

[U07] Py：反转字典键值
来源：http://m.share.bbcook.cn/Article/details/geftdhumx.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.tarul.cn/Article/details/gctyddjjq.sHtML

[U08] Py：展平二维列表
来源：http://m.share.yfazqb.com/Article/details/ghmwksgxj.sHtML

[y for x in nested for y in x]
来源：http://baike.bbcook.cn/Article/details/gcgdqbkba.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.epnwcf.com/Article/details/ggovbuuhv.sHtML

max(d, key=d.get)
来源：http://wap.sjlbkw.cn/Article/details/gayrokoyi.sHtML

[U10] Py：按值排序字典
来源：http://wap.bbcook.cn/Article/details/ghbigkbhf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.epnwcf.com/Article/details/ghtcrgndu.sHtML

[U11] Py：生成器表达式
来源：http://blog.bbcook.cn/Article/details/gzjbtjrnw.sHtML

(x * 2 for x in arr)
来源：http://baike.fktsv.cn/Article/details/gabiczkzd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fktsv.cn/Article/details/gvxebvbdl.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/gplvecphm.sHtML

[U13] Py：固定长度队列
来源：http://m.share.sjlbkw.cn/Article/details/gnzdkielb.sHtML

deque(maxlen=10)
来源：http://read.share.yfazqb.com/Article/details/gteqfthdo.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fktsv.cn/Article/details/gbffpfwuo.sHtML

defaultdict(list)
来源：http://m.share.yfazqb.com/Article/details/gamojysol.sHtML

[U15] Py：高精度计时
来源：http://m.share.fktsv.cn/Article/details/gethftsgl.sHtML

t = time.perf_counter()
来源：http://www.blog.bbcook.cn/Article/details/gjialrnfl.sHtML

[U16] Py：命令行参数解析
来源：http://3g.vehdjk.com/Article/details/gokbrzzfn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.epnwcf.com/Article/details/glanuqnsg.sHtML

[U17] Py：初始化日志
来源：http://m.share.vehdjk.com/Article/details/giutvjmdg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fktsv.cn/Article/details/gsouymxig.sHtML

[U18] Py：预编译正则
来源：http://wap.bbcook.cn/Article/details/glwnzmypj.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.epnwcf.com/Article/details/gmwbkzoia.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fktsv.cn/Article/details/gomzqwmwm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.bbcook.cn/Article/details/gsyrbpvks.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.tarul.cn/Article/details/gnjjhibje.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.vehdjk.com/Article/details/gelgwvyjs.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.vehdjk.com/Article/details/gkjrpzpnn.sHtML

@contextlib.contextmanager
来源：http://mobile.fktsv.cn/Article/details/grxtedocx.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fktsv.cn/Article/details/gfzblidns.sHtML

list(zip(*m))
来源：http://wap.bbcook.cn/Article/details/gjtwsfral.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fktsv.cn/Article/details/gvdtdentp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.bbcook.cn/Article/details/gvuwpsoeo.sHtML

[U24] Py：路径操作
来源：http://www.share.epnwcf.com/Article/details/gaxmdqjko.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/gulljbnvi.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fktsv.cn/Article/details/gfdvwkjkh.sHtML

csv.DictReader(f)
来源：http://baike.epnwcf.com/Article/details/gspvalxkx.sHtML

[U26] Py：并发下载
来源：http://baike.bbcook.cn/Article/details/guhdndiia.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.yfazqb.com/Article/details/gjmnqqtwh.sHtML

[U27] Py：异步 HTTP
来源：http://3g.tarul.cn/Article/details/glrspzdkc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.epnwcf.com/Article/details/gkceaexvl.sHtML

[U28] Py：类型别名
来源：http://blog.yfazqb.com/Article/details/gxiemqilw.sHtML

UserId = int
来源：http://www.blog.bbcook.cn/Article/details/gqfurpqvl.sHtML

[U29] Py：属性校验
来源：http://baike.yfazqb.com/Article/details/gzzxzufob.sHtML

@property 与 @x.setter 配合
来源：http://3g.bbcook.cn/Article/details/gdxzwokxm.sHtML

[U30] Py：数据类
来源：http://www.share.epnwcf.com/Article/details/gpzspdviu.sHtML

@dataclass(slots=True)
来源：http://mobile.vehdjk.com/Article/details/gptqqgysy.sHtML

[U31] Py：单测
来源：http://wap.yfazqb.com/Article/details/gvpxesbpk.sHtML

python -m pytest -q
来源：http://read.share.epnwcf.com/Article/details/grrxsjhnq.sHtML

[U32] Py：代码格式化
来源：http://read.share.epnwcf.com/Article/details/gnvleomgb.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.bbcook.cn/Article/details/gtfdhhqnp.sHtML

[U33] Py：打包发布
来源：http://mobile.sjlbkw.cn/Article/details/gucdehlbm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.epnwcf.com/Article/details/gzjnznbqs.sHtML

[U34] Py：判断编码
来源：http://www.m.share.bbcook.cn/Article/details/gsvxaplrq.sHtML

chardet.detect(raw)
来源：http://m.share.sjlbkw.cn/Article/details/gprzsozzt.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fktsv.cn/Article/details/gqntkslev.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.tarul.cn/Article/details/gbpsmrvry.sHtML

[U36] Py：定时任务
来源：http://wap.vehdjk.com/Article/details/ghzdrwyui.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fktsv.cn/Article/details/gabpaajcs.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fktsv.cn/Article/details/grvpsdojq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.yfazqb.com/Article/details/ghpvjeucm.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.sjlbkw.cn/Article/details/gefuuwjrg.sHtML

Path(__file__).resolve().parent
来源：http://www.share.vehdjk.com/Article/details/giizfzchf.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fktsv.cn/Article/details/ggcixqpcb.sHtML

sys.stdout.isatty()
来源：http://www.share.fktsv.cn/Article/details/gwtlirtne.sHtML

[U40] Py：打印到标准错误
来源：http://blog.sjlbkw.cn/Article/details/govcxeuft.sHtML

print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/googfrptw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.epnwcf.com/Article/details/gcshuuzsm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.yfazqb.com/Article/details/gbzprlpis.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.tarul.cn/Article/details/gdatanfrp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.tarul.cn/Article/details/gbpmtkkqi.sHtML

[U43] PHP：声明命名空间
来源：http://3g.bbcook.cn/Article/details/gsykqgdwy.sHtML

namespace App\Http;
来源：http://m.share.sjlbkw.cn/Article/details/gngcgvspo.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.tarul.cn/Article/details/gmlxmtqlf.sHtML

declare(strict_types=1);
来源：http://mobile.bbcook.cn/Article/details/gniergbxy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.vehdjk.com/Article/details/gfmfcluyv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gwsszjmkb.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.yfazqb.com/Article/details/gzthhsuni.sHtML

?string $name = null
来源：http://baike.epnwcf.com/Article/details/gahuxisyb.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.epnwcf.com/Article/details/gewpewvtu.sHtML

int|string $id
来源：http://3g.tarul.cn/Article/details/gyoieyumg.sHtML

[U48] PHP：纯枚举
来源：http://blog.tarul.cn/Article/details/gdluvvqgo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.sjlbkw.cn/Article/details/gklhoukwc.sHtML

[U49] PHP：只读属性
来源：http://mobile.yfazqb.com/Article/details/gxdxkplcv.sHtML

public readonly string $name
来源：http://www.share.vehdjk.com/Article/details/gneicsfyh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fktsv.cn/Article/details/gvbzywddl.sHtML

public function __construct(private int $id) {}
来源：http://3g.yfazqb.com/Article/details/gwlwrpbdn.sHtML

[U51] PHP：数组解构
来源：http://wap.fktsv.cn/Article/details/glbzoekpe.sHtML

[$a, $b] = $arr;
来源：http://wap.tarul.cn/Article/details/gtizrgpml.sHtML

[U52] PHP：箭头函数
来源：http://wap.bbcook.cn/Article/details/guhknwvzx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.yfazqb.com/Article/details/gyhcbgasp.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.bbcook.cn/Article/details/ghnyjnlbm.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.vehdjk.com/Article/details/gzbcilats.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.bbcook.cn/Article/details/gujoxjbhp.sHtML

$obj?->method()
来源：http://www.blog.yfazqb.com/Article/details/grtbudymu.sHtML

[U55] PHP：match 表达式
来源：http://wap.epnwcf.com/Article/details/ggkgxoqvq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.sjlbkw.cn/Article/details/gfldoqhvm.sHtML

[U56] PHP：命名参数
来源：http://wap.vehdjk.com/Article/details/gdwwasozq.sHtML

f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gwmpmxqxt.sHtML

[U57] PHP：字符串插值
来源：http://mobile.bbcook.cn/Article/details/ghoqjbrfl.sHtML

"值: {$a}"
来源：http://mobile.tarul.cn/Article/details/gjcyegqkl.sHtML

[U58] PHP：数组三件套
来源：http://www.share.vehdjk.com/Article/details/gezcithnj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.epnwcf.com/Article/details/gkkelkdsd.sHtML

[U59] PHP：自定义排序
来源：http://m.share.bbcook.cn/Article/details/gvtjxbfer.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/gahaftcdh.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fktsv.cn/Article/details/gcwplcpfi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fktsv.cn/Article/details/gcpilwklc.sHtML

[U61] PHP：正则
来源：http://m.share.yfazqb.com/Article/details/gyrpvnfqm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.yfazqb.com/Article/details/giuskdvxk.sHtML

[U62] PHP：日期对象
来源：http://baike.fktsv.cn/Article/details/ggegphxdk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.bbcook.cn/Article/details/giyvrszea.sHtML

[U63] PHP：文件读写
来源：http://www.share.tarul.cn/Article/details/gqvvltbuj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.sjlbkw.cn/Article/details/grvngtcow.sHtML

[U64] PHP：目录遍历
来源：http://baike.vehdjk.com/Article/details/giwhbozhn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fktsv.cn/Article/details/grwaosuev.sHtML

[U65] PHP：会话
来源：http://www.blog.tarul.cn/Article/details/gzrhgwwzb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.bbcook.cn/Article/details/gvepjbdee.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.yfazqb.com/Article/details/gyzdywirp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.tarul.cn/Article/details/gnbuchrhe.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.tarul.cn/Article/details/gpaockwdn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.epnwcf.com/Article/details/gnvznzldx.sHtML

[U68] PHP：PDO 连接
来源：http://blog.vehdjk.com/Article/details/gevaygtmi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.yfazqb.com/Article/details/gwunhkzjx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.yfazqb.com/Article/details/ghahevodl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.bbcook.cn/Article/details/gyfhebmji.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.vehdjk.com/Article/details/gkmemsdyy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.epnwcf.com/Article/details/glojfcssm.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/gzpteiics.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.epnwcf.com/Article/details/gpxpvobdj.sHtML

[U72] PHP：写错误日志
来源：http://read.share.sjlbkw.cn/Article/details/gojuevcpe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.bbcook.cn/Article/details/grlefjmgr.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.vehdjk.com/Article/details/gbbcceixz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fktsv.cn/Article/details/gckdjjvyv.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gqfomjefy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.sjlbkw.cn/Article/details/ggoyhskbr.sHtML

[U75] PHP：依赖注入
来源：http://wap.tarul.cn/Article/details/geqvtojzb.sHtML

composer require psr/container
来源：http://wap.bbcook.cn/Article/details/gzwemtxab.sHtML

[U76] PHP：简单路由
来源：http://blog.fktsv.cn/Article/details/gfmiqavqa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.yfazqb.com/Article/details/geeuoewjk.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.yfazqb.com/Article/details/gybwajrys.sHtML

composer require twig/twig
来源：http://wap.tarul.cn/Article/details/goqyjhxrt.sHtML

[U78] PHP：单元测试
来源：http://mobile.tarul.cn/Article/details/gypxzgcgj.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.bbcook.cn/Article/details/gnekxkpea.sHtML

[U79] PHP：静态分析
来源：http://baike.sjlbkw.cn/Article/details/gzjfptlpa.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.vehdjk.com/Article/details/gblyfbnpt.sHtML

[U80] PHP：代码规范修复
来源：http://3g.vehdjk.com/Article/details/gupzmmmps.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.bbcook.cn/Article/details/gjqatqlbw.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.bbcook.cn/Article/details/gzqyqsvhx.sHtML

npm init -y;  npm i express
来源：http://mobile.epnwcf.com/Article/details/gdgnfekex.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fktsv.cn/Article/details/gaktbiznx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fktsv.cn/Article/details/gqrkfibmp.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.vehdjk.com/Article/details/ggmtsohpj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.tarul.cn/Article/details/gwjzohkfn.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fktsv.cn/Article/details/gbpybnezv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.bbcook.cn/Article/details/gtqzzsksn.sHtML

[U85] JS：可选链
来源：http://m.share.bbcook.cn/Article/details/gnoqqjzps.sHtML

a?.b?.c
来源：http://3g.epnwcf.com/Article/details/gxsbkfaff.sHtML

[U86] JS：空值合并
来源：http://3g.vehdjk.com/Article/details/gcnhoftqn.sHtML

a ?? b
来源：http://mobile.tarul.cn/Article/details/gobiwvfmc.sHtML

[U87] JS：解构默认值
来源：http://3g.bbcook.cn/Article/details/gkdyylnra.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.yfazqb.com/Article/details/gjyjjovch.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.yfazqb.com/Article/details/gazwqgpjk.sHtML

{ ...a, ...b }
来源：http://baike.vehdjk.com/Article/details/gfxuawvfr.sHtML

[U89] JS：数组去重
来源：http://www.blog.tarul.cn/Article/details/gauquewcu.sHtML

[...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gdmdonfgy.sHtML

[U90] JS：数字数组排序
来源：http://read.share.vehdjk.com/Article/details/gohxelvwy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gjbzmdewy.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.yfazqb.com/Article/details/gpjeyoumn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fktsv.cn/Article/details/gwtrxuwfn.sHtML

[U92] JS：深拷贝
来源：http://www.share.fktsv.cn/Article/details/gbizlbknp.sHtML

structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/ghsnrvfkl.sHtML

[U93] JS：模板字符串
来源：http://3g.sjlbkw.cn/Article/details/gjeyyeabg.sHtML

`共 ${n} 条`
来源：http://read.share.yfazqb.com/Article/details/gupwxttoj.sHtML

[U94] JS：箭头函数
来源：http://m.share.yfazqb.com/Article/details/gsfzqvfxt.sHtML

const double = x => x * 2;
来源：http://baike.vehdjk.com/Article/details/ggkbqkzid.sHtML

[U95] JS：Promise 包装
来源：http://wap.fktsv.cn/Article/details/grkmdqcgj.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.tarul.cn/Article/details/gknwswstx.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.sjlbkw.cn/Article/details/gvyipisuq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gnrzezxyo.sHtML

[U97] JS：并发请求
来源：http://baike.fktsv.cn/Article/details/gzrhfqffh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gqtzkdcoq.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.epnwcf.com/Article/details/gzdflznxo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fktsv.cn/Article/details/gjojqtblt.sHtML

[U99] JS：事件监听
来源：http://mobile.sjlbkw.cn/Article/details/gxdmvqcey.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fktsv.cn/Article/details/gcayryklw.sHtML

[U100] JS：DOM 查询
来源：http://blog.fktsv.cn/Article/details/gppgdknoa.sHtML

document.querySelector(".item")
来源：http://read.share.sjlbkw.cn/Article/details/gntfksspx.sHtML

[U101] JS：classList 操作
来源：http://blog.tarul.cn/Article/details/gcnumcwor.sHtML

el.classList.toggle("active")
来源：http://3g.epnwcf.com/Article/details/guaebpxae.sHtML

[U102] JS：本地存储
来源：http://www.blog.tarul.cn/Article/details/grqueggwc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.bbcook.cn/Article/details/gvqebxwjd.sHtML

[U103] JS：定时器
来源：http://www.share.yfazqb.com/Article/details/gaigezdje.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.tarul.cn/Article/details/gjicisjfz.sHtML

[U104] JS：防抖
来源：http://www.m.share.yfazqb.com/Article/details/gelrwyblj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gevntvbnb.sHtML

[U105] JS：节流
来源：http://3g.vehdjk.com/Article/details/gyqmrkvjg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.sjlbkw.cn/Article/details/gplbhdzks.sHtML

[U106] JS：日期格式化
来源：http://3g.bbcook.cn/Article/details/gvyjjhpmh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.sjlbkw.cn/Article/details/glgunfvte.sHtML

[U107] JS：数字千分位
来源：http://mobile.fktsv.cn/Article/details/gjucbvidc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gckljhicl.sHtML

[U108] JS：随机整数
来源：http://3g.bbcook.cn/Article/details/gearcbbvj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.tarul.cn/Article/details/glxeoqzww.sHtML

[U109] JS：数组分组
来源：http://mobile.yfazqb.com/Article/details/gvxnxoqzu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.tarul.cn/Article/details/gbfcsawgn.sHtML

[U110] JS：数组分块
来源：http://baike.bbcook.cn/Article/details/gffdkjsbk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.yfazqb.com/Article/details/gpggftlxa.sHtML

[U111] JS：对象转 Map
来源：http://wap.sjlbkw.cn/Article/details/gpdcylzxg.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.tarul.cn/Article/details/gvqheemdk.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.epnwcf.com/Article/details/gruqikpux.sHtML

"7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gvrradzns.sHtML

[U113] JS：正则替换全部
来源：http://read.share.epnwcf.com/Article/details/glqkwfijq.sHtML

s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gwlgvsxpn.sHtML

[U114] JS：JSON 深比较
来源：http://baike.yfazqb.com/Article/details/ghqfdesme.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.bbcook.cn/Article/details/gtgodmnsu.sHtML

[U115] JS：生成 UUID
来源：http://read.share.tarul.cn/Article/details/gahlwylwo.sHtML

crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gtslomdhz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fktsv.cn/Article/details/gwsgyhrhk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.tarul.cn/Article/details/gbrlhdkwy.sHtML

[U117] JS：单元测试
来源：http://wap.tarul.cn/Article/details/gvtmuidzp.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.vehdjk.com/Article/details/gdrokjask.sHtML

[U118] JS：开发服务器
来源：http://m.share.yfazqb.com/Article/details/genolsviw.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.vehdjk.com/Article/details/gaxdtxoff.sHtML

[U119] JS：生产构建
来源：http://www.m.share.bbcook.cn/Article/details/gtkmwbdgm.sHtML

npx vite build
来源：http://www.blog.epnwcf.com/Article/details/gtmpigtvb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.yfazqb.com/Article/details/grxnakili.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.epnwcf.com/Article/details/gtxuoytev.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdwplskvw.sHtML

统计汇总
来源：http://baike.bbcook.cn/Article/details/guzqltlrr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkgrbqsru.sHtML

按语言统计（条）：
来源：http://www.m.share.vehdjk.com/Article/details/gfblmefzb.sHtML

Python ......... 252
来源：http://read.share.fktsv.cn/Article/details/gfxozivnr.sHtML

PHP ............ 252
来源：http://www.blog.epnwcf.com/Article/details/gxmvfgivf.sHtML

JavaScript ..... 252
来源：http://baike.vehdjk.com/Article/details/gighdicpo.sHtML

TypeScript ..... 212
来源：http://wap.epnwcf.com/Article/details/gdgehlwow.sHtML

Java ........... 212
来源：http://3g.sjlbkw.cn/Article/details/gviwtckkx.sHtML

Go ............. 212
来源：http://baike.epnwcf.com/Article/details/gqsvqbpaz.sHtML

Ruby ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gtptixuwt.sHtML

C# ............. 212
来源：http://baike.yfazqb.com/Article/details/gtahanbqh.sHtML

C .............. 30
来源：http://read.share.fktsv.cn/Article/details/gnmghhsxd.sHtML

C++ ............ 30
来源：http://read.share.tarul.cn/Article/details/gsefxzrkt.sHtML

SQL ............ 90
来源：http://baike.epnwcf.com/Article/details/gktjipbhe.sHtML

Bash ........... 80
来源：http://3g.vehdjk.com/Article/details/gglmyefee.sHtML

Kotlin ......... 15
来源：http://read.share.epnwcf.com/Article/details/gltsiwmwb.sHtML

Swift .......... 15
来源：http://baike.bbcook.cn/Article/details/gzvigxamh.sHtML

Lua ............ 10
来源：http://mobile.fktsv.cn/Article/details/gidjjvtma.sHtML

Perl ........... 10
来源：http://wap.epnwcf.com/Article/details/gqwtzqhjy.sHtML

Scala .......... 10
来源：http://www.m.share.epnwcf.com/Article/details/giifqigqv.sHtML

------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gzcosyoei.sHtML

合计 ........... 2106 条
来源：http://blog.epnwcf.com/Article/details/gpxvzbdux.sHtML

按章节统计：
来源：http://www.m.share.epnwcf.com/Article/details/gxrwlvdaw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.bbcook.cn/Article/details/gahebslkk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gqoweyiui.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/grorfifqa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/grfnngrto.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fktsv.cn/Article/details/gclazraus.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gmlzxtptx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gqeabxfbx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.vehdjk.com/Article/details/gzehcxkvv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gkgnbkgoc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fktsv.cn/Article/details/gzrahoycz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gsovhkbfh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gxpqmdiqm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gwtvsfrbw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.tarul.cn/Article/details/gvikuzvkw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.tarul.cn/Article/details/gulchacav.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gxcluqbhs.sHtML

Q SQL 专题                              90
来源：http://www.m.share.tarul.cn/Article/details/gzjasdxzn.sHtML

R Bash 专题                             80
来源：http://3g.tarul.cn/Article/details/gdjttifmy.sHtML

S C / C++ 专题                          60
来源：http://www.blog.sjlbkw.cn/Article/details/gnbawslqo.sHtML

T 其他语言补充                          60
来源：http://www.blog.sjlbkw.cn/Article/details/gufbnjrib.sHtML

U 高频实用片段                         120
来源：http://baike.sjlbkw.cn/Article/details/gwkefujbv.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gpliumpvh.sHtML

合计                                  2106 条
来源：http://m.share.tarul.cn/Article/details/gywesvxxq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gtwdoiyna.sHtML

使用提醒
来源：http://www.blog.yfazqb.com/Article/details/gotazrbgq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gptgnfwpf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.yfazqb.com/Article/details/gbairjxze.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.vehdjk.com/Article/details/gvbfjunsj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fktsv.cn/Article/details/gnqqwoliy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.sjlbkw.cn/Article/details/giospupsx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.yfazqb.com/Article/details/gcqivdvna.sHtML

—— 文件结束 ——
来源：http://m.share.yfazqb.com/Article/details/gzgcjsthb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gurytmsnw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.vehdjk.com/Article/details/ghiqcrftb.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.sjlbkw.cn/Article/details/grbdbhniy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfxmazlue.sHtML


<!-- 参考信息 -->