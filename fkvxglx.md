代发 wailian999

[U01] Py：创建虚拟环境
来源：http://blog.vehdjk.com/Article/details/gpxogaozb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.sjlbkw.cn/Article/details/gctnrjpaa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.tarul.cn/Article/details/ggazsomzp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.sjlbkw.cn/Article/details/gkutlphyn.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.epnwcf.com/Article/details/gjgetajsa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.bbcook.cn/Article/details/gwbyyshsa.sHtML

[U04] Py：变量调试打印
来源：http://baike.bbcook.cn/Article/details/gvrcxfzrq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.bbcook.cn/Article/details/gkhkyhqfd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fktsv.cn/Article/details/gqvgfjaij.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gegdzxqfa.sHtML

[U06] Py：合并两个字典
来源：http://m.share.bbcook.cn/Article/details/grzjvfian.sHtML

{**a, **b}
来源：http://www.m.share.fktsv.cn/Article/details/gyidjoisd.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.tarul.cn/Article/details/gyfekqwpe.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fktsv.cn/Article/details/gnpvgrcld.sHtML

[U08] Py：展平二维列表
来源：http://m.share.sjlbkw.cn/Article/details/gduupbame.sHtML

[y for x in nested for y in x]
来源：http://baike.sjlbkw.cn/Article/details/gzajhzpta.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.vehdjk.com/Article/details/ghqooquch.sHtML

max(d, key=d.get)
来源：http://mobile.bbcook.cn/Article/details/gtmxdnumy.sHtML

[U10] Py：按值排序字典
来源：http://m.share.yfazqb.com/Article/details/gvawbhsuw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.vehdjk.com/Article/details/gevmkuecb.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fktsv.cn/Article/details/gtpnkzyxg.sHtML

(x * 2 for x in arr)
来源：http://mobile.sjlbkw.cn/Article/details/goglvopxr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.vehdjk.com/Article/details/ghkxtobkv.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gdpjvaurg.sHtML

[U13] Py：固定长度队列
来源：http://3g.yfazqb.com/Article/details/ghdyzclhl.sHtML

deque(maxlen=10)
来源：http://wap.yfazqb.com/Article/details/galssmvlp.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.yfazqb.com/Article/details/gvtneyvhw.sHtML

defaultdict(list)
来源：http://blog.fktsv.cn/Article/details/gfhxjsoyf.sHtML

[U15] Py：高精度计时
来源：http://baike.vehdjk.com/Article/details/gjholjaix.sHtML

t = time.perf_counter()
来源：http://mobile.fktsv.cn/Article/details/gzqgcbxlr.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.tarul.cn/Article/details/givdftmgr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.yfazqb.com/Article/details/gpwtqwwts.sHtML

[U17] Py：初始化日志
来源：http://baike.bbcook.cn/Article/details/gyokqzsgy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.bbcook.cn/Article/details/gjsvybjes.sHtML

[U18] Py：预编译正则
来源：http://www.blog.tarul.cn/Article/details/ginknqtps.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.epnwcf.com/Article/details/gxynykzhy.sHtML

[U19] Py：正则替换带回调
来源：http://wap.epnwcf.com/Article/details/gzhhaqllt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.tarul.cn/Article/details/gdpxsondv.sHtML

[U20] Py：缓存函数结果
来源：http://wap.sjlbkw.cn/Article/details/gxlnacroq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fktsv.cn/Article/details/gzwibmlnz.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.sjlbkw.cn/Article/details/gykqmdgdq.sHtML

@contextlib.contextmanager
来源：http://www.share.yfazqb.com/Article/details/ghuleghax.sHtML

[U22] Py：矩阵转置
来源：http://baike.tarul.cn/Article/details/gryccqolg.sHtML

list(zip(*m))
来源：http://www.blog.sjlbkw.cn/Article/details/gtaewoggq.sHtML

[U23] Py：分块读取大文件
来源：http://blog.sjlbkw.cn/Article/details/gkphfdqpu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fktsv.cn/Article/details/gaxpdszau.sHtML

[U24] Py：路径操作
来源：http://blog.bbcook.cn/Article/details/gnqzqvmsi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gjtyvwtla.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.tarul.cn/Article/details/gswdumxzs.sHtML

csv.DictReader(f)
来源：http://baike.fktsv.cn/Article/details/gtbmecwlu.sHtML

[U26] Py：并发下载
来源：http://m.share.bbcook.cn/Article/details/gmkisfsof.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.yfazqb.com/Article/details/gvqcbcqzc.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.yfazqb.com/Article/details/gmfrroyra.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.yfazqb.com/Article/details/gynqzzihn.sHtML

[U28] Py：类型别名
来源：http://www.blog.vehdjk.com/Article/details/grucdrajp.sHtML

UserId = int
来源：http://www.blog.vehdjk.com/Article/details/gwunkpijp.sHtML

[U29] Py：属性校验
来源：http://wap.tarul.cn/Article/details/ghiftgefi.sHtML

@property 与 @x.setter 配合
来源：http://blog.tarul.cn/Article/details/gtejwyicz.sHtML

[U30] Py：数据类
来源：http://mobile.tarul.cn/Article/details/gaougqeul.sHtML

@dataclass(slots=True)
来源：http://www.share.vehdjk.com/Article/details/gafwalfbl.sHtML

[U31] Py：单测
来源：http://m.share.sjlbkw.cn/Article/details/gsjynwrqe.sHtML

python -m pytest -q
来源：http://mobile.sjlbkw.cn/Article/details/gejaeheqc.sHtML

[U32] Py：代码格式化
来源：http://read.share.yfazqb.com/Article/details/gxdqscdsy.sHtML

ruff format . && ruff check --fix .
来源：http://3g.tarul.cn/Article/details/gyxwawtob.sHtML

[U33] Py：打包发布
来源：http://www.share.bbcook.cn/Article/details/gdzyynwjt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.yfazqb.com/Article/details/gfwlqdoyj.sHtML

[U34] Py：判断编码
来源：http://www.m.share.vehdjk.com/Article/details/gmkulgfof.sHtML

chardet.detect(raw)
来源：http://www.share.bbcook.cn/Article/details/gapgpuizb.sHtML

[U35] Py：发送邮件
来源：http://baike.bbcook.cn/Article/details/gegsecltt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fktsv.cn/Article/details/gluziakhj.sHtML

[U36] Py：定时任务
来源：http://www.m.share.vehdjk.com/Article/details/glrgwzyqk.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.tarul.cn/Article/details/godfssrwd.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/gydidzdfl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.bbcook.cn/Article/details/gypytrhiu.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fktsv.cn/Article/details/gmvplgyhi.sHtML

Path(__file__).resolve().parent
来源：http://www.share.bbcook.cn/Article/details/gkeckzryf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.sjlbkw.cn/Article/details/glbgmxjnr.sHtML

sys.stdout.isatty()
来源：http://blog.yfazqb.com/Article/details/godkzaqxd.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.bbcook.cn/Article/details/gxipqakch.sHtML

print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/gjavnjtjg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.sjlbkw.cn/Article/details/guqmcbsce.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.vehdjk.com/Article/details/gvpzpvdhm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.bbcook.cn/Article/details/gvjtwxkhc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fktsv.cn/Article/details/gkaazjpac.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.bbcook.cn/Article/details/gzuorzdin.sHtML

namespace App\Http;
来源：http://blog.fktsv.cn/Article/details/gpdqiivub.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.tarul.cn/Article/details/gwvozbjio.sHtML

declare(strict_types=1);
来源：http://mobile.tarul.cn/Article/details/gcxnutxpj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.epnwcf.com/Article/details/gxdtkzpya.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gswurozdw.sHtML

[U46] PHP：可空类型
来源：http://www.blog.yfazqb.com/Article/details/gijbsvzmt.sHtML

?string $name = null
来源：http://wap.fktsv.cn/Article/details/gftceouwk.sHtML

[U47] PHP：联合类型
来源：http://3g.yfazqb.com/Article/details/gcwhofmhx.sHtML

int|string $id
来源：http://m.share.tarul.cn/Article/details/gpmcbuywc.sHtML

[U48] PHP：纯枚举
来源：http://mobile.tarul.cn/Article/details/gkscixvfa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.vehdjk.com/Article/details/gbamtxtyx.sHtML

[U49] PHP：只读属性
来源：http://wap.fktsv.cn/Article/details/gkoquqzbj.sHtML

public readonly string $name
来源：http://www.m.share.tarul.cn/Article/details/guertvufh.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.yfazqb.com/Article/details/giititgup.sHtML

public function __construct(private int $id) {}
来源：http://m.share.yfazqb.com/Article/details/gsvvzsogr.sHtML

[U51] PHP：数组解构
来源：http://www.share.epnwcf.com/Article/details/gwcyeoiwj.sHtML

[$a, $b] = $arr;
来源：http://baike.fktsv.cn/Article/details/gfphexxjm.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fktsv.cn/Article/details/gmikurqdk.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/gddvwykpk.sHtML

[U53] PHP：空合并运算符
来源：http://baike.bbcook.cn/Article/details/gtdbmziig.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.epnwcf.com/Article/details/gwdyfegal.sHtML

[U54] PHP：空安全调用
来源：http://wap.epnwcf.com/Article/details/gglqsplpc.sHtML

$obj?->method()
来源：http://mobile.fktsv.cn/Article/details/gwdmsnnua.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.epnwcf.com/Article/details/gghhhdajj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.yfazqb.com/Article/details/gxplbvjjf.sHtML

[U56] PHP：命名参数
来源：http://baike.fktsv.cn/Article/details/gjisssfcf.sHtML

f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gaozspgvw.sHtML

[U57] PHP：字符串插值
来源：http://blog.tarul.cn/Article/details/gtkrbuzeg.sHtML

"值: {$a}"
来源：http://3g.yfazqb.com/Article/details/gfarhkklw.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fktsv.cn/Article/details/gckogeqwk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.yfazqb.com/Article/details/goenxmjik.sHtML

[U59] PHP：自定义排序
来源：http://wap.vehdjk.com/Article/details/gljvvzyki.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.tarul.cn/Article/details/gbhsnzkqs.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.sjlbkw.cn/Article/details/gsuggzxuz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.yfazqb.com/Article/details/grvhrynke.sHtML

[U61] PHP：正则
来源：http://www.blog.fktsv.cn/Article/details/goloxvcfh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/gwnfivdam.sHtML

[U62] PHP：日期对象
来源：http://m.share.epnwcf.com/Article/details/gondxitmu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.tarul.cn/Article/details/gvhfnaolw.sHtML

[U63] PHP：文件读写
来源：http://read.share.vehdjk.com/Article/details/gxgglmlrv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.sjlbkw.cn/Article/details/gsweykxcb.sHtML

[U64] PHP：目录遍历
来源：http://www.share.epnwcf.com/Article/details/gxwihveyx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.bbcook.cn/Article/details/gxdlalxuu.sHtML

[U65] PHP：会话
来源：http://mobile.bbcook.cn/Article/details/giucnjspz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gzzxhghri.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.epnwcf.com/Article/details/gisoiaarq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.yfazqb.com/Article/details/gopolpxat.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fktsv.cn/Article/details/geonbzbwc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.epnwcf.com/Article/details/gtskohxqv.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.bbcook.cn/Article/details/gustbkyri.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.sjlbkw.cn/Article/details/ghnpuyblg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.bbcook.cn/Article/details/gnbfwefou.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.sjlbkw.cn/Article/details/gfxfohtzo.sHtML

[U70] PHP：PDO 事务
来源：http://wap.epnwcf.com/Article/details/gjfwvvppw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.yfazqb.com/Article/details/gpuujrtis.sHtML

[U71] PHP：抛出异常
来源：http://www.share.yfazqb.com/Article/details/gggbziwuu.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.vehdjk.com/Article/details/goidrhysz.sHtML

[U72] PHP：写错误日志
来源：http://3g.sjlbkw.cn/Article/details/gajrvnzzo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.yfazqb.com/Article/details/geqkuqlgj.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fktsv.cn/Article/details/gdlejqpxu.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fktsv.cn/Article/details/glmatfcpc.sHtML

[U74] PHP：读取环境变量
来源：http://baike.tarul.cn/Article/details/ghenojggz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.bbcook.cn/Article/details/girppoktw.sHtML

[U75] PHP：依赖注入
来源：http://3g.yfazqb.com/Article/details/ggsyuekbj.sHtML

composer require psr/container
来源：http://mobile.epnwcf.com/Article/details/gojkmmaxv.sHtML

[U76] PHP：简单路由
来源：http://wap.vehdjk.com/Article/details/gprvhuasr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fktsv.cn/Article/details/glskoarfo.sHtML

[U77] PHP：模板渲染
来源：http://3g.sjlbkw.cn/Article/details/ghesmddgy.sHtML

composer require twig/twig
来源：http://www.m.share.sjlbkw.cn/Article/details/gtufrcbeo.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gmcryrtzb.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fktsv.cn/Article/details/gtfsshxyx.sHtML

[U79] PHP：静态分析
来源：http://m.share.epnwcf.com/Article/details/gehyrauda.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fktsv.cn/Article/details/gcfwwxtpd.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.bbcook.cn/Article/details/gicuzcykd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.vehdjk.com/Article/details/gujpobvtm.sHtML

[U81] JS：初始化项目
来源：http://m.share.sjlbkw.cn/Article/details/gissubauk.sHtML

npm init -y;  npm i express
来源：http://www.blog.bbcook.cn/Article/details/ghgpcoexx.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.epnwcf.com/Article/details/gnsmyyhbc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.yfazqb.com/Article/details/golkhxdnb.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fktsv.cn/Article/details/gjsrerjzu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.tarul.cn/Article/details/gpyncacje.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.yfazqb.com/Article/details/gentgcrdp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.yfazqb.com/Article/details/gupycwaln.sHtML

[U85] JS：可选链
来源：http://wap.epnwcf.com/Article/details/gqkrdltmd.sHtML

a?.b?.c
来源：http://www.blog.tarul.cn/Article/details/ggvoyxkvp.sHtML

[U86] JS：空值合并
来源：http://read.share.bbcook.cn/Article/details/gvtetfrug.sHtML

a ?? b
来源：http://www.m.share.vehdjk.com/Article/details/gzzwwlbpb.sHtML

[U87] JS：解构默认值
来源：http://m.share.yfazqb.com/Article/details/grbvdstxn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.tarul.cn/Article/details/gpdzesxom.sHtML

[U88] JS：对象展开合并
来源：http://3g.sjlbkw.cn/Article/details/gruwbgivo.sHtML

{ ...a, ...b }
来源：http://m.share.sjlbkw.cn/Article/details/gewlzuuef.sHtML

[U89] JS：数组去重
来源：http://www.share.yfazqb.com/Article/details/gmvxxkepe.sHtML

[...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gxnpmhlzi.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fktsv.cn/Article/details/ghdjtgvcj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/ggztdcmvw.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.yfazqb.com/Article/details/goxaumveg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.yfazqb.com/Article/details/guofnorws.sHtML

[U92] JS：深拷贝
来源：http://mobile.tarul.cn/Article/details/gmwitxlyk.sHtML

structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gxgtljhhk.sHtML

[U93] JS：模板字符串
来源：http://baike.yfazqb.com/Article/details/gphyhiany.sHtML

`共 ${n} 条`
来源：http://www.m.share.vehdjk.com/Article/details/gugmmgdfi.sHtML

[U94] JS：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/gqexldbzc.sHtML

const double = x => x * 2;
来源：http://mobile.vehdjk.com/Article/details/gdghvncjr.sHtML

[U95] JS：Promise 包装
来源：http://3g.tarul.cn/Article/details/gdhmrryov.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.epnwcf.com/Article/details/glrsvaxsg.sHtML

[U96] JS：async/await 与异常
来源：http://wap.sjlbkw.cn/Article/details/ggdmfiayy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gssacnwur.sHtML

[U97] JS：并发请求
来源：http://www.share.epnwcf.com/Article/details/gctjocplt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gbxpugnnd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.yfazqb.com/Article/details/gvcjsherf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gjklcidvw.sHtML

[U99] JS：事件监听
来源：http://baike.sjlbkw.cn/Article/details/gfukfpwqc.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.tarul.cn/Article/details/ghinbubgv.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.yfazqb.com/Article/details/gghcodjax.sHtML

document.querySelector(".item")
来源：http://blog.fktsv.cn/Article/details/gqdlpnbjj.sHtML

[U101] JS：classList 操作
来源：http://3g.bbcook.cn/Article/details/gvmyaoajh.sHtML

el.classList.toggle("active")
来源：http://read.share.epnwcf.com/Article/details/gqzyqbiid.sHtML

[U102] JS：本地存储
来源：http://3g.sjlbkw.cn/Article/details/guxeqivnk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.epnwcf.com/Article/details/gevrqzoro.sHtML

[U103] JS：定时器
来源：http://baike.tarul.cn/Article/details/gcyrbglya.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fktsv.cn/Article/details/gufyatput.sHtML

[U104] JS：防抖
来源：http://blog.sjlbkw.cn/Article/details/grdmfdpgp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/ggvkcqhqi.sHtML

[U105] JS：节流
来源：http://www.m.share.tarul.cn/Article/details/gaavfpcey.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.epnwcf.com/Article/details/gnxxkynyy.sHtML

[U106] JS：日期格式化
来源：http://mobile.yfazqb.com/Article/details/gmvayktwg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.vehdjk.com/Article/details/gfkmskhrh.sHtML

[U107] JS：数字千分位
来源：http://3g.sjlbkw.cn/Article/details/gksayycgj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/gxmnovoin.sHtML

[U108] JS：随机整数
来源：http://3g.epnwcf.com/Article/details/gwaeohtav.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.sjlbkw.cn/Article/details/gkowzqdrl.sHtML

[U109] JS：数组分组
来源：http://blog.yfazqb.com/Article/details/gwzwbmknd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.yfazqb.com/Article/details/gtennbhtc.sHtML

[U110] JS：数组分块
来源：http://baike.sjlbkw.cn/Article/details/gvrohpdou.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fktsv.cn/Article/details/gcrxfdxxh.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.yfazqb.com/Article/details/gdgcisucj.sHtML

new Map(Object.entries(obj))
来源：http://baike.yfazqb.com/Article/details/gpmifdyas.sHtML

[U112] JS：字符串补位
来源：http://blog.sjlbkw.cn/Article/details/ggfcialvj.sHtML

"7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gsgllkudj.sHtML

[U113] JS：正则替换全部
来源：http://m.share.bbcook.cn/Article/details/gpxfgqlop.sHtML

s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gtrdfyede.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.tarul.cn/Article/details/gukqdclul.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gdzauhaqb.sHtML

[U115] JS：生成 UUID
来源：http://blog.vehdjk.com/Article/details/gpzvhajrd.sHtML

crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/gwebnxrzu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgmphzor.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.sjlbkw.cn/Article/details/glmzaoopj.sHtML

[U117] JS：单元测试
来源：http://mobile.epnwcf.com/Article/details/gwddlqgel.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.yfazqb.com/Article/details/gsbpqrnve.sHtML

[U118] JS：开发服务器
来源：http://3g.sjlbkw.cn/Article/details/gmtmczfje.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fktsv.cn/Article/details/gtfksuswx.sHtML

[U119] JS：生产构建
来源：http://mobile.sjlbkw.cn/Article/details/ghzgfjzou.sHtML

npx vite build
来源：http://www.blog.tarul.cn/Article/details/gjaxdrzje.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.yfazqb.com/Article/details/gouqiidlh.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.yfazqb.com/Article/details/gkqfngrmo.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gxacedpol.sHtML

统计汇总
来源：http://mobile.epnwcf.com/Article/details/gsefihbzk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzwxjstsx.sHtML

按语言统计（条）：
来源：http://m.share.fktsv.cn/Article/details/gpyzjaxhr.sHtML

Python ......... 252
来源：http://baike.epnwcf.com/Article/details/gnyimajeq.sHtML

PHP ............ 252
来源：http://blog.sjlbkw.cn/Article/details/gnbjhzzzf.sHtML

JavaScript ..... 252
来源：http://www.blog.tarul.cn/Article/details/gtfzoqcmr.sHtML

TypeScript ..... 212
来源：http://mobile.bbcook.cn/Article/details/glcnizqal.sHtML

Java ........... 212
来源：http://baike.epnwcf.com/Article/details/gwfzlpncm.sHtML

Go ............. 212
来源：http://mobile.yfazqb.com/Article/details/gzwbbnyqq.sHtML

Ruby ........... 212
来源：http://www.m.share.epnwcf.com/Article/details/gfrlsynxb.sHtML

C# ............. 212
来源：http://www.share.epnwcf.com/Article/details/ggjyernkw.sHtML

C .............. 30
来源：http://blog.tarul.cn/Article/details/gkjduejts.sHtML

C++ ............ 30
来源：http://mobile.yfazqb.com/Article/details/ghricthth.sHtML

SQL ............ 90
来源：http://wap.bbcook.cn/Article/details/gxsjidsba.sHtML

Bash ........... 80
来源：http://m.share.vehdjk.com/Article/details/gjclelghr.sHtML

Kotlin ......... 15
来源：http://www.share.fktsv.cn/Article/details/gfirsftjo.sHtML

Swift .......... 15
来源：http://blog.fktsv.cn/Article/details/gppwixivv.sHtML

Lua ............ 10
来源：http://blog.tarul.cn/Article/details/gybngfhao.sHtML

Perl ........... 10
来源：http://blog.bbcook.cn/Article/details/grvzwcqgg.sHtML

Scala .......... 10
来源：http://www.m.share.yfazqb.com/Article/details/gdoirljaq.sHtML

------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gpirkxyur.sHtML

合计 ........... 2106 条
来源：http://www.m.share.yfazqb.com/Article/details/ghplhszov.sHtML

按章节统计：
来源：http://read.share.fktsv.cn/Article/details/grwlrnlep.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.bbcook.cn/Article/details/gbyhcmmhi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/gdfxqwiat.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/geelrdrct.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.vehdjk.com/Article/details/gmqaxgznv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.epnwcf.com/Article/details/glpowbmme.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.sjlbkw.cn/Article/details/grnfvqriq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gntiajukk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwhlzbot.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gxoyzpckl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.epnwcf.com/Article/details/gqmkbrtdy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gqmfbrzrx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gpxlbnedk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gzvjkisvq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.yfazqb.com/Article/details/gtowbsqvs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.epnwcf.com/Article/details/ghosxlpva.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/ghiagbzka.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fktsv.cn/Article/details/gontpprap.sHtML

R Bash 专题                             80
来源：http://www.blog.epnwcf.com/Article/details/gmbsgsyxd.sHtML

S C / C++ 专题                          60
来源：http://read.share.bbcook.cn/Article/details/gnajqlaig.sHtML

T 其他语言补充                          60
来源：http://3g.vehdjk.com/Article/details/gixgzgvse.sHtML

U 高频实用片段                         120
来源：http://baike.fktsv.cn/Article/details/gpsjkpdal.sHtML

------------------------------------
来源：http://m.share.vehdjk.com/Article/details/ggjbalont.sHtML

合计                                  2106 条
来源：http://www.blog.vehdjk.com/Article/details/ggavuahdw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/ggidkitjj.sHtML

使用提醒
来源：http://m.share.tarul.cn/Article/details/gdoetdtgk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/ghapugkoi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.vehdjk.com/Article/details/gajqmrskh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.sjlbkw.cn/Article/details/gpvwtslxk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.vehdjk.com/Article/details/gzbfzuvyg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.yfazqb.com/Article/details/gtvjhpblp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.sjlbkw.cn/Article/details/gdzcrywfm.sHtML

—— 文件结束 ——
来源：http://baike.epnwcf.com/Article/details/gqmfmablp.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gowwpgjww.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.epnwcf.com/Article/details/gxlqgpaoj.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.sjlbkw.cn/Article/details/gbcdlkdhe.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ggvtzofff.sHtML


<!-- 参考信息 -->