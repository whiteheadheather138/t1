代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.m.share.bbcook.cn/Article/details/gwtvcadml.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.yfazqb.com/Article/details/gkecwgpsp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/goxkwzjgr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.sjlbkw.cn/Article/details/gjjisjveo.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.epnwcf.com/Article/details/gwefcbtmq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.bbcook.cn/Article/details/gixovkgcc.sHtML

[U04] Py：变量调试打印
来源：http://3g.yfazqb.com/Article/details/gvqsalhpq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.epnwcf.com/Article/details/gvuqhgplv.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.epnwcf.com/Article/details/giuoghpjf.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gpcltlawo.sHtML

[U06] Py：合并两个字典
来源：http://blog.epnwcf.com/Article/details/gxglgyozv.sHtML

{**a, **b}
来源：http://m.share.epnwcf.com/Article/details/gabcmmhpf.sHtML

[U07] Py：反转字典键值
来源：http://www.share.bbcook.cn/Article/details/gqcvpskfp.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.yfazqb.com/Article/details/gqwxphnwi.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.vehdjk.com/Article/details/gnwyamdrr.sHtML

[y for x in nested for y in x]
来源：http://mobile.vehdjk.com/Article/details/gwhgxkxvg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.tarul.cn/Article/details/gwsfsnzkc.sHtML

max(d, key=d.get)
来源：http://m.share.fktsv.cn/Article/details/gklmrqezb.sHtML

[U10] Py：按值排序字典
来源：http://baike.sjlbkw.cn/Article/details/gtlegerrn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.yfazqb.com/Article/details/gfesittmx.sHtML

[U11] Py：生成器表达式
来源：http://3g.yfazqb.com/Article/details/ggpvvibaa.sHtML

(x * 2 for x in arr)
来源：http://m.share.bbcook.cn/Article/details/ggixsgoxm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.tarul.cn/Article/details/gqozxuwmd.sHtML

Counter(arr).most_common(3)
来源：http://3g.bbcook.cn/Article/details/gohlkhlhk.sHtML

[U13] Py：固定长度队列
来源：http://m.share.vehdjk.com/Article/details/gbbbjibwp.sHtML

deque(maxlen=10)
来源：http://wap.bbcook.cn/Article/details/gqmgcuiyg.sHtML

[U14] Py：分组收集到列表
来源：http://3g.epnwcf.com/Article/details/gogilkdcu.sHtML

defaultdict(list)
来源：http://read.share.tarul.cn/Article/details/guzoonkcz.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.yfazqb.com/Article/details/gheuniyvo.sHtML

t = time.perf_counter()
来源：http://www.blog.yfazqb.com/Article/details/geroygckh.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fktsv.cn/Article/details/gvxkjvnqf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.vehdjk.com/Article/details/gxuridjib.sHtML

[U17] Py：初始化日志
来源：http://wap.vehdjk.com/Article/details/gklpklhcc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.sjlbkw.cn/Article/details/gdppaqlhg.sHtML

[U18] Py：预编译正则
来源：http://www.share.sjlbkw.cn/Article/details/gmaerltcm.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fktsv.cn/Article/details/gwfpywugt.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.sjlbkw.cn/Article/details/gywaacdia.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.yfazqb.com/Article/details/gxojygrcr.sHtML

[U20] Py：缓存函数结果
来源：http://wap.bbcook.cn/Article/details/guhtartrk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.sjlbkw.cn/Article/details/gvmmodphv.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fktsv.cn/Article/details/gzwfbxgmy.sHtML

@contextlib.contextmanager
来源：http://www.blog.fktsv.cn/Article/details/gqhamubsl.sHtML

[U22] Py：矩阵转置
来源：http://read.share.sjlbkw.cn/Article/details/gipfwliim.sHtML

list(zip(*m))
来源：http://read.share.sjlbkw.cn/Article/details/geusgfjcd.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.bbcook.cn/Article/details/gnyysizmz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.vehdjk.com/Article/details/gxztxtwwj.sHtML

[U24] Py：路径操作
来源：http://3g.yfazqb.com/Article/details/gicrfozej.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gkkuslasp.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.sjlbkw.cn/Article/details/gbzysbfmq.sHtML

csv.DictReader(f)
来源：http://www.blog.yfazqb.com/Article/details/gmnozehmw.sHtML

[U26] Py：并发下载
来源：http://m.share.epnwcf.com/Article/details/gezmgglsc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.epnwcf.com/Article/details/gdysoxhuh.sHtML

[U27] Py：异步 HTTP
来源：http://baike.sjlbkw.cn/Article/details/giyjjmrxd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fktsv.cn/Article/details/gvwghktui.sHtML

[U28] Py：类型别名
来源：http://baike.vehdjk.com/Article/details/grjbdtshh.sHtML

UserId = int
来源：http://3g.vehdjk.com/Article/details/gmtdpbwym.sHtML

[U29] Py：属性校验
来源：http://mobile.epnwcf.com/Article/details/gkilibojz.sHtML

@property 与 @x.setter 配合
来源：http://read.share.bbcook.cn/Article/details/ggcsjwmwu.sHtML

[U30] Py：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/gqcmxasrt.sHtML

@dataclass(slots=True)
来源：http://3g.vehdjk.com/Article/details/gathpamty.sHtML

[U31] Py：单测
来源：http://www.m.share.yfazqb.com/Article/details/gelhsnlbx.sHtML

python -m pytest -q
来源：http://baike.vehdjk.com/Article/details/gjhuhhoal.sHtML

[U32] Py：代码格式化
来源：http://3g.yfazqb.com/Article/details/gsdhuskid.sHtML

ruff format . && ruff check --fix .
来源：http://wap.vehdjk.com/Article/details/gbjpkxrmt.sHtML

[U33] Py：打包发布
来源：http://www.share.fktsv.cn/Article/details/glhjseris.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fktsv.cn/Article/details/grmkbbztu.sHtML

[U34] Py：判断编码
来源：http://www.blog.tarul.cn/Article/details/gzyaqeday.sHtML

chardet.detect(raw)
来源：http://m.share.epnwcf.com/Article/details/gprrwxpzz.sHtML

[U35] Py：发送邮件
来源：http://www.share.vehdjk.com/Article/details/gmjjntbfj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.tarul.cn/Article/details/gyinoadxz.sHtML

[U36] Py：定时任务
来源：http://3g.yfazqb.com/Article/details/grwyvrffi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.epnwcf.com/Article/details/gbagekzlu.sHtML

[U37] Py：读写 Excel
来源：http://mobile.vehdjk.com/Article/details/gpvlfvhcz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.epnwcf.com/Article/details/gabomblwy.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.sjlbkw.cn/Article/details/gvchgxfvt.sHtML

Path(__file__).resolve().parent
来源：http://mobile.tarul.cn/Article/details/ginvmdmle.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.epnwcf.com/Article/details/gpszbopbv.sHtML

sys.stdout.isatty()
来源：http://read.share.fktsv.cn/Article/details/gmnnwhiai.sHtML

[U40] Py：打印到标准错误
来源：http://3g.vehdjk.com/Article/details/gtaoynqak.sHtML

print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gklqjkzhl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.yfazqb.com/Article/details/gxnxbeaem.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.bbcook.cn/Article/details/gevhsemfy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.bbcook.cn/Article/details/gbtmljodw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.tarul.cn/Article/details/gxhudvtvs.sHtML

[U43] PHP：声明命名空间
来源：http://blog.bbcook.cn/Article/details/ggxrhhspa.sHtML

namespace App\Http;
来源：http://baike.sjlbkw.cn/Article/details/gzdmqaahj.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fktsv.cn/Article/details/gvuzoqrso.sHtML

declare(strict_types=1);
来源：http://baike.bbcook.cn/Article/details/gobyuaavd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.yfazqb.com/Article/details/grlpzbzce.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/grcjjhyoq.sHtML

[U46] PHP：可空类型
来源：http://baike.sjlbkw.cn/Article/details/gbdmyoqiq.sHtML

?string $name = null
来源：http://www.blog.epnwcf.com/Article/details/glrcorbeh.sHtML

[U47] PHP：联合类型
来源：http://3g.tarul.cn/Article/details/gigezzqyy.sHtML

int|string $id
来源：http://mobile.vehdjk.com/Article/details/ggytwueiz.sHtML

[U48] PHP：纯枚举
来源：http://3g.bbcook.cn/Article/details/gnacxntlu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.bbcook.cn/Article/details/gqfkjpmwb.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fktsv.cn/Article/details/grfafdsvr.sHtML

public readonly string $name
来源：http://m.share.epnwcf.com/Article/details/gdqwiogql.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.epnwcf.com/Article/details/gyhluddsv.sHtML

public function __construct(private int $id) {}
来源：http://blog.epnwcf.com/Article/details/gfdmieybc.sHtML

[U51] PHP：数组解构
来源：http://3g.vehdjk.com/Article/details/gieqjctyp.sHtML

[$a, $b] = $arr;
来源：http://www.blog.tarul.cn/Article/details/gaecajevv.sHtML

[U52] PHP：箭头函数
来源：http://www.share.vehdjk.com/Article/details/grhgyuicg.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.tarul.cn/Article/details/gdagdrifl.sHtML

[U53] PHP：空合并运算符
来源：http://baike.vehdjk.com/Article/details/gqlblrmnr.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.yfazqb.com/Article/details/grbbknmuj.sHtML

[U54] PHP：空安全调用
来源：http://wap.sjlbkw.cn/Article/details/gukbdfwct.sHtML

$obj?->method()
来源：http://wap.vehdjk.com/Article/details/gftnfsvuc.sHtML

[U55] PHP：match 表达式
来源：http://mobile.bbcook.cn/Article/details/gfvuotlig.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/gzzxsstsq.sHtML

[U56] PHP：命名参数
来源：http://3g.epnwcf.com/Article/details/gqgvltajh.sHtML

f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gpysusnrs.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gtvcbypag.sHtML

"值: {$a}"
来源：http://m.share.epnwcf.com/Article/details/gqmsebgze.sHtML

[U58] PHP：数组三件套
来源：http://wap.epnwcf.com/Article/details/gunbwgdha.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gnrdjlopr.sHtML

[U59] PHP：自定义排序
来源：http://wap.tarul.cn/Article/details/giybmvsie.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.sjlbkw.cn/Article/details/gdcuvucqy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.bbcook.cn/Article/details/gscrwjxja.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.yfazqb.com/Article/details/girnvbtoi.sHtML

[U61] PHP：正则
来源：http://read.share.fktsv.cn/Article/details/gcrvlhpzp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/ghhftwcza.sHtML

[U62] PHP：日期对象
来源：http://m.share.fktsv.cn/Article/details/gvbvdbukl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.tarul.cn/Article/details/gropjxdct.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.vehdjk.com/Article/details/gsmicuwxz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.epnwcf.com/Article/details/gqlwnbcgf.sHtML

[U64] PHP：目录遍历
来源：http://m.share.sjlbkw.cn/Article/details/gghpdfurm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.epnwcf.com/Article/details/gkeltaxhu.sHtML

[U65] PHP：会话
来源：http://www.m.share.yfazqb.com/Article/details/gplgyfygn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/ghrmjgvwj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fktsv.cn/Article/details/glmcokxal.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.bbcook.cn/Article/details/gqadtucec.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.sjlbkw.cn/Article/details/gklowebzm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.tarul.cn/Article/details/gpxywedmc.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.tarul.cn/Article/details/grnrlzsmt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.vehdjk.com/Article/details/gsvtyceqd.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.tarul.cn/Article/details/gcdgfwnmh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.sjlbkw.cn/Article/details/gkgvkwzmp.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.vehdjk.com/Article/details/gjeolcoff.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fktsv.cn/Article/details/grywrchxc.sHtML

[U71] PHP：抛出异常
来源：http://read.share.tarul.cn/Article/details/giyyrmswo.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fktsv.cn/Article/details/grphvybig.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.sjlbkw.cn/Article/details/gerzsbhba.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.yfazqb.com/Article/details/ggjdsdhsy.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.epnwcf.com/Article/details/gqldghecp.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.tarul.cn/Article/details/gldutwoce.sHtML

[U74] PHP：读取环境变量
来源：http://wap.bbcook.cn/Article/details/gajfvskgw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.epnwcf.com/Article/details/gbncqghjh.sHtML

[U75] PHP：依赖注入
来源：http://wap.yfazqb.com/Article/details/gqynbguvd.sHtML

composer require psr/container
来源：http://mobile.yfazqb.com/Article/details/graiejifv.sHtML

[U76] PHP：简单路由
来源：http://www.share.yfazqb.com/Article/details/gwasdqlhm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.bbcook.cn/Article/details/gfdiplwut.sHtML

[U77] PHP：模板渲染
来源：http://3g.yfazqb.com/Article/details/grcgjbuyq.sHtML

composer require twig/twig
来源：http://www.share.tarul.cn/Article/details/gcmeqibml.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.tarul.cn/Article/details/gpafotios.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.sjlbkw.cn/Article/details/gqgbhdqjs.sHtML

[U79] PHP：静态分析
来源：http://m.share.yfazqb.com/Article/details/gehdwkxzr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.epnwcf.com/Article/details/ggqrvzvbv.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.tarul.cn/Article/details/giwsqulde.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.tarul.cn/Article/details/gnyafinfo.sHtML

[U81] JS：初始化项目
来源：http://www.blog.tarul.cn/Article/details/gswkniwdo.sHtML

npm init -y;  npm i express
来源：http://www.share.yfazqb.com/Article/details/ggsznhmsz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.vehdjk.com/Article/details/gipiwblwn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.yfazqb.com/Article/details/gjllihlvc.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.yfazqb.com/Article/details/gxijvlsgv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/glovuhsmt.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fktsv.cn/Article/details/grwponzsi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.vehdjk.com/Article/details/glofiatxb.sHtML

[U85] JS：可选链
来源：http://m.share.fktsv.cn/Article/details/gjcdibjef.sHtML

a?.b?.c
来源：http://baike.yfazqb.com/Article/details/grzocawth.sHtML

[U86] JS：空值合并
来源：http://wap.tarul.cn/Article/details/grlippuej.sHtML

a ?? b
来源：http://wap.sjlbkw.cn/Article/details/gpnpdcged.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fktsv.cn/Article/details/grzlhhirr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.yfazqb.com/Article/details/gmftvgyah.sHtML

[U88] JS：对象展开合并
来源：http://3g.yfazqb.com/Article/details/gynxcyakw.sHtML

{ ...a, ...b }
来源：http://read.share.bbcook.cn/Article/details/guygszqie.sHtML

[U89] JS：数组去重
来源：http://3g.epnwcf.com/Article/details/gsolevnps.sHtML

[...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gdjakpycg.sHtML

[U90] JS：数字数组排序
来源：http://baike.vehdjk.com/Article/details/gzzgfkuix.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gaahzbfte.sHtML

[U91] JS：对象键值遍历
来源：http://wap.sjlbkw.cn/Article/details/grzhohzcs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fktsv.cn/Article/details/gksdwokuc.sHtML

[U92] JS：深拷贝
来源：http://3g.sjlbkw.cn/Article/details/gbbizeeem.sHtML

structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gejmfwyed.sHtML

[U93] JS：模板字符串
来源：http://baike.epnwcf.com/Article/details/gzexbqfkh.sHtML

`共 ${n} 条`
来源：http://blog.vehdjk.com/Article/details/guqhhfeeb.sHtML

[U94] JS：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/geuwqhkez.sHtML

const double = x => x * 2;
来源：http://www.m.share.epnwcf.com/Article/details/gxzpzhsaz.sHtML

[U95] JS：Promise 包装
来源：http://3g.vehdjk.com/Article/details/gmbxtbwjl.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.sjlbkw.cn/Article/details/ghforpudm.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.yfazqb.com/Article/details/gejjadojo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gsnegviqw.sHtML

[U97] JS：并发请求
来源：http://www.blog.yfazqb.com/Article/details/gkrlczvtd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gqbahrjeh.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.tarul.cn/Article/details/ghpfjhaea.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.yfazqb.com/Article/details/gvgeafldd.sHtML

[U99] JS：事件监听
来源：http://wap.yfazqb.com/Article/details/gyxaufram.sHtML

el.addEventListener("click", e => {})
来源：http://3g.sjlbkw.cn/Article/details/gyxqvgxdj.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.bbcook.cn/Article/details/ghixinvjj.sHtML

document.querySelector(".item")
来源：http://baike.yfazqb.com/Article/details/gfoctnkdc.sHtML

[U101] JS：classList 操作
来源：http://mobile.bbcook.cn/Article/details/gydfprjpl.sHtML

el.classList.toggle("active")
来源：http://wap.yfazqb.com/Article/details/glnjyedaq.sHtML

[U102] JS：本地存储
来源：http://read.share.fktsv.cn/Article/details/gtfybtwbh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.bbcook.cn/Article/details/gngkvokig.sHtML

[U103] JS：定时器
来源：http://wap.yfazqb.com/Article/details/gwsvlubld.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.vehdjk.com/Article/details/gzoguoqqu.sHtML

[U104] JS：防抖
来源：http://baike.yfazqb.com/Article/details/gqyxvuini.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gdagfguxz.sHtML

[U105] JS：节流
来源：http://www.share.sjlbkw.cn/Article/details/gznessqbs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.epnwcf.com/Article/details/giqtjmrac.sHtML

[U106] JS：日期格式化
来源：http://mobile.bbcook.cn/Article/details/gzpgvpvxd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.tarul.cn/Article/details/gvmzalssi.sHtML

[U107] JS：数字千分位
来源：http://blog.yfazqb.com/Article/details/gletefvlz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.bbcook.cn/Article/details/gxmcygdcv.sHtML

[U108] JS：随机整数
来源：http://blog.sjlbkw.cn/Article/details/gmnjkhsve.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.vehdjk.com/Article/details/gllkkqnsn.sHtML

[U109] JS：数组分组
来源：http://mobile.bbcook.cn/Article/details/gtvdsgivm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gfnfuqzjt.sHtML

[U110] JS：数组分块
来源：http://mobile.sjlbkw.cn/Article/details/gfjbetzzb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.sjlbkw.cn/Article/details/getjrkzyy.sHtML

[U111] JS：对象转 Map
来源：http://www.share.yfazqb.com/Article/details/gajqlyscv.sHtML

new Map(Object.entries(obj))
来源：http://wap.fktsv.cn/Article/details/gqilpedvo.sHtML

[U112] JS：字符串补位
来源：http://m.share.bbcook.cn/Article/details/gbbhlcwca.sHtML

"7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/ghhtefxuc.sHtML

[U113] JS：正则替换全部
来源：http://www.share.tarul.cn/Article/details/ghpfqzzjx.sHtML

s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/grodnglsm.sHtML

[U114] JS：JSON 深比较
来源：http://wap.sjlbkw.cn/Article/details/gtnppkkob.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/gtturhdol.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/gvyfoctli.sHtML

crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gyphitlpu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.bbcook.cn/Article/details/gloqjhplb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.bbcook.cn/Article/details/gbchztila.sHtML

[U117] JS：单元测试
来源：http://3g.tarul.cn/Article/details/gqowdglvh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.vehdjk.com/Article/details/gnesmgmyu.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.sjlbkw.cn/Article/details/grnziqrii.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.sjlbkw.cn/Article/details/gqcragmmx.sHtML

[U119] JS：生产构建
来源：http://wap.tarul.cn/Article/details/girutcadb.sHtML

npx vite build
来源：http://www.share.vehdjk.com/Article/details/giwzsknyr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fktsv.cn/Article/details/gxhfwvaap.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.bbcook.cn/Article/details/gunzdqabg.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gomtvubqc.sHtML

统计汇总
来源：http://blog.yfazqb.com/Article/details/gbbvltrka.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwgjntujo.sHtML

按语言统计（条）：
来源：http://baike.epnwcf.com/Article/details/guagyboix.sHtML

Python ......... 252
来源：http://blog.tarul.cn/Article/details/gxntzczyu.sHtML

PHP ............ 252
来源：http://read.share.sjlbkw.cn/Article/details/gvrurekcz.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/gfjxswyui.sHtML

TypeScript ..... 212
来源：http://wap.bbcook.cn/Article/details/gmoeuejzi.sHtML

Java ........... 212
来源：http://3g.sjlbkw.cn/Article/details/gttqxzmgs.sHtML

Go ............. 212
来源：http://www.m.share.tarul.cn/Article/details/ginmqfaxe.sHtML

Ruby ........... 212
来源：http://www.m.share.vehdjk.com/Article/details/gnqsrypbo.sHtML

C# ............. 212
来源：http://www.m.share.fktsv.cn/Article/details/gmgaizujn.sHtML

C .............. 30
来源：http://3g.bbcook.cn/Article/details/gpuetzcjb.sHtML

C++ ............ 30
来源：http://wap.epnwcf.com/Article/details/gmobfcdmy.sHtML

SQL ............ 90
来源：http://baike.vehdjk.com/Article/details/gcyvkxoco.sHtML

Bash ........... 80
来源：http://www.share.epnwcf.com/Article/details/gujxxtsku.sHtML

Kotlin ......... 15
来源：http://baike.bbcook.cn/Article/details/guvsisjel.sHtML

Swift .......... 15
来源：http://www.blog.bbcook.cn/Article/details/gtewqzhwl.sHtML

Lua ............ 10
来源：http://www.share.sjlbkw.cn/Article/details/grkidglsd.sHtML

Perl ........... 10
来源：http://baike.fktsv.cn/Article/details/gsxryiuww.sHtML

Scala .......... 10
来源：http://blog.epnwcf.com/Article/details/gnloqqjvk.sHtML

------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gvipjliyt.sHtML

合计 ........... 2106 条
来源：http://mobile.yfazqb.com/Article/details/gadmkysye.sHtML

按章节统计：
来源：http://blog.vehdjk.com/Article/details/gbfhybuhj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/gkxotrylh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gkutboofk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gtjjdxgnm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/gnuyxpqzr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.epnwcf.com/Article/details/gcbwwshrv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.yfazqb.com/Article/details/ghhvabczp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/gfwedlkhu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/gcdcruhqo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gvjndaevt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.vehdjk.com/Article/details/gmitnreiy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gigdwxoor.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gahqzljlj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gjelwisgy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fktsv.cn/Article/details/gubdnsags.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.epnwcf.com/Article/details/gldkgcjqk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/ggunthjvb.sHtML

Q SQL 专题                              90
来源：http://mobile.vehdjk.com/Article/details/gjdtemfcn.sHtML

R Bash 专题                             80
来源：http://m.share.sjlbkw.cn/Article/details/gacpobqri.sHtML

S C / C++ 专题                          60
来源：http://m.share.bbcook.cn/Article/details/givaznkrp.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fktsv.cn/Article/details/gajwkevbe.sHtML

U 高频实用片段                         120
来源：http://baike.sjlbkw.cn/Article/details/ggkltuaxc.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gigltzfdc.sHtML

合计                                  2106 条
来源：http://blog.bbcook.cn/Article/details/gryhgbwya.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gnqcagjlw.sHtML

使用提醒
来源：http://www.m.share.tarul.cn/Article/details/gdqjqmhim.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gplgbzdmp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fktsv.cn/Article/details/gjoylafap.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.sjlbkw.cn/Article/details/gcsaimgcn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fktsv.cn/Article/details/gtwifqqqp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.vehdjk.com/Article/details/ggmetxhco.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.vehdjk.com/Article/details/gkrlqhppt.sHtML

—— 文件结束 ——
来源：http://3g.bbcook.cn/Article/details/gvhfqkhcw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxckuflbd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fktsv.cn/Article/details/grrfibgyw.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnwpbuxw.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/giuipdaga.sHtML


<!-- 参考信息 -->