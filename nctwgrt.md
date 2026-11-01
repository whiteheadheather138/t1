代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.epnwcf.com/Article/details/gtqmgixqs.sHtML

[T59] Scala：循环
来源：http://www.share.fktsv.cn/Article/details/gjmmdfrna.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gscenarzp.sHtML

[T60] Scala：折叠
来源：http://baike.tarul.cn/Article/details/gisfqbqap.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.epnwcf.com/Article/details/gofhtkkbj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grvaupkxx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.tarul.cn/Article/details/gggnwmpsl.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvtfwkqjr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.yfazqb.com/Article/details/gnnmdwhlr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.yfazqb.com/Article/details/gmindvcrt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.yfazqb.com/Article/details/gvsprguns.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fktsv.cn/Article/details/gtyyqelxp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.bbcook.cn/Article/details/gqowapseu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fktsv.cn/Article/details/ggomglxtn.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.yfazqb.com/Article/details/ghoclrkmn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.vehdjk.com/Article/details/gkbnblbdu.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/gdkuxensy.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/gxbdtaasv.sHtML

[U06] Py：合并两个字典
来源：http://mobile.bbcook.cn/Article/details/gjqfgulzl.sHtML

{**a, **b}
来源：http://mobile.sjlbkw.cn/Article/details/gqkqjzjvh.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fktsv.cn/Article/details/gsqahkpnc.sHtML

{v: k for k, v in d.items()}
来源：http://blog.bbcook.cn/Article/details/grgnauscl.sHtML

[U08] Py：展平二维列表
来源：http://m.share.bbcook.cn/Article/details/gnhchzcyi.sHtML

[y for x in nested for y in x]
来源：http://read.share.tarul.cn/Article/details/gtsosebyf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.yfazqb.com/Article/details/gjtpwwkas.sHtML

max(d, key=d.get)
来源：http://baike.tarul.cn/Article/details/ghloeoyqi.sHtML

[U10] Py：按值排序字典
来源：http://read.share.yfazqb.com/Article/details/gujrjhmpk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fktsv.cn/Article/details/gchazaeoi.sHtML

[U11] Py：生成器表达式
来源：http://3g.bbcook.cn/Article/details/gbckspyjw.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.epnwcf.com/Article/details/gvrcmqvpi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.bbcook.cn/Article/details/gdsrhvykf.sHtML

Counter(arr).most_common(3)
来源：http://mobile.sjlbkw.cn/Article/details/gbbioloiy.sHtML

[U13] Py：固定长度队列
来源：http://blog.bbcook.cn/Article/details/gusdugdza.sHtML

deque(maxlen=10)
来源：http://www.share.tarul.cn/Article/details/gvozfdxcm.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fktsv.cn/Article/details/gnyeddfhf.sHtML

defaultdict(list)
来源：http://baike.yfazqb.com/Article/details/gufktmfpp.sHtML

[U15] Py：高精度计时
来源：http://m.share.tarul.cn/Article/details/gpndewheu.sHtML

t = time.perf_counter()
来源：http://3g.bbcook.cn/Article/details/gobmharde.sHtML

[U16] Py：命令行参数解析
来源：http://3g.bbcook.cn/Article/details/gdpwutytr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fktsv.cn/Article/details/gomlwshwz.sHtML

[U17] Py：初始化日志
来源：http://baike.tarul.cn/Article/details/gjfwktupo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.sjlbkw.cn/Article/details/gqeouihzp.sHtML

[U18] Py：预编译正则
来源：http://www.blog.bbcook.cn/Article/details/gexwienxl.sHtML

pat = re.compile(r"\d+")
来源：http://baike.vehdjk.com/Article/details/gxvvinwwo.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.vehdjk.com/Article/details/gxsliljhz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.vehdjk.com/Article/details/goyixkvfx.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.tarul.cn/Article/details/gsyyducvc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.tarul.cn/Article/details/ggoueakvj.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.bbcook.cn/Article/details/gbhxzxxum.sHtML

@contextlib.contextmanager
来源：http://wap.epnwcf.com/Article/details/guwcethki.sHtML

[U22] Py：矩阵转置
来源：http://blog.tarul.cn/Article/details/geuexsxur.sHtML

list(zip(*m))
来源：http://www.m.share.tarul.cn/Article/details/gtqvhzsiy.sHtML

[U23] Py：分块读取大文件
来源：http://baike.tarul.cn/Article/details/gesauhpht.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.epnwcf.com/Article/details/gtkwgcpls.sHtML

[U24] Py：路径操作
来源：http://wap.yfazqb.com/Article/details/gpcbwgvyd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.sjlbkw.cn/Article/details/gkfmiqlme.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.epnwcf.com/Article/details/gcdfacotw.sHtML

csv.DictReader(f)
来源：http://www.blog.fktsv.cn/Article/details/ghcmrgnrr.sHtML

[U26] Py：并发下载
来源：http://wap.bbcook.cn/Article/details/gxdwuyvir.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.yfazqb.com/Article/details/ghdrlomsj.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fktsv.cn/Article/details/ghoiuxofe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.vehdjk.com/Article/details/gpbvwqcov.sHtML

[U28] Py：类型别名
来源：http://m.share.sjlbkw.cn/Article/details/grkalfyky.sHtML

UserId = int
来源：http://mobile.sjlbkw.cn/Article/details/ggxzzugut.sHtML

[U29] Py：属性校验
来源：http://www.share.vehdjk.com/Article/details/gtliaglph.sHtML

@property 与 @x.setter 配合
来源：http://wap.epnwcf.com/Article/details/gmdabpxfy.sHtML

[U30] Py：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/gohxzpsjj.sHtML

@dataclass(slots=True)
来源：http://m.share.sjlbkw.cn/Article/details/grvdvbmun.sHtML

[U31] Py：单测
来源：http://mobile.vehdjk.com/Article/details/guumrbbgr.sHtML

python -m pytest -q
来源：http://blog.sjlbkw.cn/Article/details/gfpxxdgir.sHtML

[U32] Py：代码格式化
来源：http://3g.epnwcf.com/Article/details/grsgkqaqm.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.bbcook.cn/Article/details/grxohhhlj.sHtML

[U33] Py：打包发布
来源：http://www.blog.fktsv.cn/Article/details/gzlfoirtu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fktsv.cn/Article/details/gtpcdsvgs.sHtML

[U34] Py：判断编码
来源：http://www.share.vehdjk.com/Article/details/gpowxnhbh.sHtML

chardet.detect(raw)
来源：http://mobile.vehdjk.com/Article/details/gbqbgvbfv.sHtML

[U35] Py：发送邮件
来源：http://www.blog.yfazqb.com/Article/details/gdsqupmvo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.yfazqb.com/Article/details/gkbnhyssg.sHtML

[U36] Py：定时任务
来源：http://blog.epnwcf.com/Article/details/gsshalwfe.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.sjlbkw.cn/Article/details/gmywdierw.sHtML

[U37] Py：读写 Excel
来源：http://blog.sjlbkw.cn/Article/details/guthyfzkq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.bbcook.cn/Article/details/gnneztvcf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.vehdjk.com/Article/details/gpikboogb.sHtML

Path(__file__).resolve().parent
来源：http://www.share.epnwcf.com/Article/details/gttiuvjoa.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.epnwcf.com/Article/details/gmvudkgbu.sHtML

sys.stdout.isatty()
来源：http://read.share.yfazqb.com/Article/details/gngkxcotf.sHtML

[U40] Py：打印到标准错误
来源：http://blog.epnwcf.com/Article/details/gztwwzyiz.sHtML

print("err", file=sys.stderr)
来源：http://wap.sjlbkw.cn/Article/details/gigpilioy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.vehdjk.com/Article/details/gvczrfiis.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.vehdjk.com/Article/details/gnecashdj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fktsv.cn/Article/details/gfoqdqxyg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.yfazqb.com/Article/details/gtjhuqjpy.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.bbcook.cn/Article/details/gnshqfhth.sHtML

namespace App\Http;
来源：http://m.share.epnwcf.com/Article/details/gpmmvzftt.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.sjlbkw.cn/Article/details/gfpxbcgjt.sHtML

declare(strict_types=1);
来源：http://mobile.tarul.cn/Article/details/gqymxnahx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.epnwcf.com/Article/details/gvnxaglja.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/ggbyqgwhl.sHtML

[U46] PHP：可空类型
来源：http://baike.yfazqb.com/Article/details/goszxruhv.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gekefucac.sHtML

[U47] PHP：联合类型
来源：http://mobile.fktsv.cn/Article/details/gqwsflmkd.sHtML

int|string $id
来源：http://wap.yfazqb.com/Article/details/gxooiwlqs.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.yfazqb.com/Article/details/gsmbbtdyo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.epnwcf.com/Article/details/gpkmnnszi.sHtML

[U49] PHP：只读属性
来源：http://www.blog.vehdjk.com/Article/details/gqbswsvbj.sHtML

public readonly string $name
来源：http://read.share.vehdjk.com/Article/details/gdycflzkt.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.epnwcf.com/Article/details/gqiobkwgy.sHtML

public function __construct(private int $id) {}
来源：http://m.share.vehdjk.com/Article/details/gxvxcwurf.sHtML

[U51] PHP：数组解构
来源：http://read.share.sjlbkw.cn/Article/details/gwshjgjsa.sHtML

[$a, $b] = $arr;
来源：http://blog.bbcook.cn/Article/details/gfqijsgrg.sHtML

[U52] PHP：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gaxisxcuw.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fktsv.cn/Article/details/gcsljrzux.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.yfazqb.com/Article/details/gavnireiz.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fktsv.cn/Article/details/gvfhahoit.sHtML

[U54] PHP：空安全调用
来源：http://wap.yfazqb.com/Article/details/goavhevmn.sHtML

$obj?->method()
来源：http://blog.yfazqb.com/Article/details/giuqyuomb.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gdcfinyxx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.yfazqb.com/Article/details/glzajolee.sHtML

[U56] PHP：命名参数
来源：http://baike.epnwcf.com/Article/details/gunouyyte.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gjxmoibms.sHtML

[U57] PHP：字符串插值
来源：http://wap.yfazqb.com/Article/details/gagmcefyq.sHtML

"值: {$a}"
来源：http://read.share.yfazqb.com/Article/details/gweexgbmb.sHtML

[U58] PHP：数组三件套
来源：http://3g.yfazqb.com/Article/details/gnllrztvz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.tarul.cn/Article/details/gilqwtfip.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fktsv.cn/Article/details/ghddqiqeb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gimjmfpsp.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.tarul.cn/Article/details/gciybrnxe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.yfazqb.com/Article/details/gooxbahux.sHtML

[U61] PHP：正则
来源：http://www.m.share.epnwcf.com/Article/details/gnmwznngb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/gefvwurep.sHtML

[U62] PHP：日期对象
来源：http://www.blog.epnwcf.com/Article/details/guwgynwfo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.bbcook.cn/Article/details/gepdcshll.sHtML

[U63] PHP：文件读写
来源：http://m.share.vehdjk.com/Article/details/grqolymjq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.bbcook.cn/Article/details/gcvgxdfum.sHtML

[U64] PHP：目录遍历
来源：http://wap.yfazqb.com/Article/details/gnpnjvukl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.yfazqb.com/Article/details/gyfvtgbrd.sHtML

[U65] PHP：会话
来源：http://blog.yfazqb.com/Article/details/gbuukfuan.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gwmdkdtpp.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.yfazqb.com/Article/details/gessfnwkp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.vehdjk.com/Article/details/ghgfuwqfg.sHtML

[U67] PHP：处理文件上传
来源：http://blog.bbcook.cn/Article/details/gzjjrrwyd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.epnwcf.com/Article/details/gxsupgpcm.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.vehdjk.com/Article/details/guinhdyba.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.bbcook.cn/Article/details/gnbwljzxh.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.yfazqb.com/Article/details/gfantktfh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.bbcook.cn/Article/details/gywvrnovk.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.yfazqb.com/Article/details/ggadkypta.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.bbcook.cn/Article/details/gjxarljyw.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.bbcook.cn/Article/details/gcsfpcdyn.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.bbcook.cn/Article/details/gksovkdem.sHtML

[U72] PHP：写错误日志
来源：http://3g.tarul.cn/Article/details/gsuukggud.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.sjlbkw.cn/Article/details/gohmwbsem.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.tarul.cn/Article/details/gwbptonda.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.yfazqb.com/Article/details/gosudpvhm.sHtML

[U74] PHP：读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gzkfneyou.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.epnwcf.com/Article/details/gxzqyubuk.sHtML

[U75] PHP：依赖注入
来源：http://3g.yfazqb.com/Article/details/gzxszrgwk.sHtML

composer require psr/container
来源：http://mobile.yfazqb.com/Article/details/ghdagqjkj.sHtML

[U76] PHP：简单路由
来源：http://blog.epnwcf.com/Article/details/ghffusdls.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fktsv.cn/Article/details/gtapcoqki.sHtML

[U77] PHP：模板渲染
来源：http://baike.tarul.cn/Article/details/gllqoqmqt.sHtML

composer require twig/twig
来源：http://m.share.bbcook.cn/Article/details/gvnqjxuus.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fktsv.cn/Article/details/gsyqesauk.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fktsv.cn/Article/details/gfjkstdcj.sHtML

[U79] PHP：静态分析
来源：http://wap.fktsv.cn/Article/details/ggemthpxm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fktsv.cn/Article/details/gtkmbftxx.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fktsv.cn/Article/details/gucttgauy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.epnwcf.com/Article/details/gbozmatqm.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.bbcook.cn/Article/details/gggryrxze.sHtML

npm init -y;  npm i express
来源：http://baike.epnwcf.com/Article/details/ggzrkwbmw.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.yfazqb.com/Article/details/gwsjwwvmd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.epnwcf.com/Article/details/gjtacuefn.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fktsv.cn/Article/details/goqbktblf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjhijukd.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.tarul.cn/Article/details/gvwyywpzx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.yfazqb.com/Article/details/gfipwppui.sHtML

[U85] JS：可选链
来源：http://www.blog.yfazqb.com/Article/details/gsjrboxph.sHtML

a?.b?.c
来源：http://read.share.sjlbkw.cn/Article/details/ghwezncvp.sHtML

[U86] JS：空值合并
来源：http://www.blog.epnwcf.com/Article/details/gzbuyquyb.sHtML

a ?? b
来源：http://3g.sjlbkw.cn/Article/details/gblqqqgcn.sHtML

[U87] JS：解构默认值
来源：http://m.share.epnwcf.com/Article/details/giwqrplqh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.yfazqb.com/Article/details/gefrzdxxh.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.epnwcf.com/Article/details/ghowkbbir.sHtML

{ ...a, ...b }
来源：http://www.blog.vehdjk.com/Article/details/galundzvo.sHtML

[U89] JS：数组去重
来源：http://3g.tarul.cn/Article/details/gziogvats.sHtML

[...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gimadhalk.sHtML

[U90] JS：数字数组排序
来源：http://wap.bbcook.cn/Article/details/gzdmznufj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gtbfzyszm.sHtML

[U91] JS：对象键值遍历
来源：http://baike.vehdjk.com/Article/details/geqrpeewo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.bbcook.cn/Article/details/gfidzbkee.sHtML

[U92] JS：深拷贝
来源：http://baike.vehdjk.com/Article/details/gfvlnbxjl.sHtML

structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gsyyrffzk.sHtML

[U93] JS：模板字符串
来源：http://wap.epnwcf.com/Article/details/ggjnjrnjl.sHtML

`共 ${n} 条`
来源：http://read.share.yfazqb.com/Article/details/gbinjlhnc.sHtML

[U94] JS：箭头函数
来源：http://baike.epnwcf.com/Article/details/gmbjjtcvg.sHtML

const double = x => x * 2;
来源：http://m.share.bbcook.cn/Article/details/gmxtnikuw.sHtML

[U95] JS：Promise 包装
来源：http://baike.epnwcf.com/Article/details/gawlhoyrw.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.yfazqb.com/Article/details/goqsndefy.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.bbcook.cn/Article/details/gkfhwhxun.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gtmqsscjb.sHtML

[U97] JS：并发请求
来源：http://www.m.share.epnwcf.com/Article/details/gsihufuts.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/gzbjmdsoc.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.tarul.cn/Article/details/gbqbtytck.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.epnwcf.com/Article/details/gqlzjcksx.sHtML

[U99] JS：事件监听
来源：http://baike.bbcook.cn/Article/details/gktiznnww.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fktsv.cn/Article/details/gqqhtqicd.sHtML

[U100] JS：DOM 查询
来源：http://baike.vehdjk.com/Article/details/gcsrlfiay.sHtML

document.querySelector(".item")
来源：http://mobile.epnwcf.com/Article/details/gbvczkxhv.sHtML

[U101] JS：classList 操作
来源：http://3g.bbcook.cn/Article/details/gjkyrfatd.sHtML

el.classList.toggle("active")
来源：http://baike.tarul.cn/Article/details/giqyflaps.sHtML

[U102] JS：本地存储
来源：http://www.blog.epnwcf.com/Article/details/gpgofzcdb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.tarul.cn/Article/details/gkurqmnsc.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/ggjrgjves.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.sjlbkw.cn/Article/details/glpzcmslq.sHtML

[U104] JS：防抖
来源：http://mobile.fktsv.cn/Article/details/gezmwkmbq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gamtmhgrh.sHtML

[U105] JS：节流
来源：http://www.share.epnwcf.com/Article/details/gnpyhvzkb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.vehdjk.com/Article/details/gqajpkghw.sHtML

[U106] JS：日期格式化
来源：http://m.share.bbcook.cn/Article/details/gmfvmykts.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fktsv.cn/Article/details/gglvrbmsx.sHtML

[U107] JS：数字千分位
来源：http://m.share.vehdjk.com/Article/details/grodlqavf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gpervkvud.sHtML

[U108] JS：随机整数
来源：http://m.share.vehdjk.com/Article/details/gtwwuokrq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.yfazqb.com/Article/details/gefmnapsw.sHtML

[U109] JS：数组分组
来源：http://3g.bbcook.cn/Article/details/gkyifuoxj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gmaaycvli.sHtML

[U110] JS：数组分块
来源：http://www.share.sjlbkw.cn/Article/details/gwxfokbmn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.sjlbkw.cn/Article/details/gicgkcuem.sHtML

[U111] JS：对象转 Map
来源：http://read.share.epnwcf.com/Article/details/gtgsjhjes.sHtML

new Map(Object.entries(obj))
来源：http://3g.epnwcf.com/Article/details/gwtvottos.sHtML

[U112] JS：字符串补位
来源：http://m.share.tarul.cn/Article/details/gksbimhcu.sHtML

"7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gejjqyxjl.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.bbcook.cn/Article/details/gtzhrnvsb.sHtML

s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/grllnlusr.sHtML

[U114] JS：JSON 深比较
来源：http://3g.vehdjk.com/Article/details/gylfafccs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gcysbocyg.sHtML

[U115] JS：生成 UUID
来源：http://mobile.epnwcf.com/Article/details/gmwqmpidb.sHtML

crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/girmvzhpf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fktsv.cn/Article/details/gcndyqtnh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.yfazqb.com/Article/details/gcnxookjk.sHtML

[U117] JS：单元测试
来源：http://3g.sjlbkw.cn/Article/details/gkbvyavcu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fktsv.cn/Article/details/gwwumtkuj.sHtML

[U118] JS：开发服务器
来源：http://www.blog.vehdjk.com/Article/details/guckhoyxm.sHtML

npm i -D vite;  npx vite
来源：http://3g.fktsv.cn/Article/details/ggyaqhykb.sHtML

[U119] JS：生产构建
来源：http://baike.sjlbkw.cn/Article/details/gvefmawba.sHtML

npx vite build
来源：http://read.share.sjlbkw.cn/Article/details/gwlzwaqdv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.tarul.cn/Article/details/gwalebnuv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.bbcook.cn/Article/details/gjajgtysc.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gusjinpyj.sHtML

统计汇总
来源：http://3g.bbcook.cn/Article/details/grlfbmifo.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gdikfttlc.sHtML

按语言统计（条）：
来源：http://m.share.vehdjk.com/Article/details/gzejjagrs.sHtML

Python ......... 252
来源：http://mobile.vehdjk.com/Article/details/gssgbtokx.sHtML

PHP ............ 252
来源：http://wap.bbcook.cn/Article/details/gakshpzgu.sHtML

JavaScript ..... 252
来源：http://baike.bbcook.cn/Article/details/gvfnhgeqd.sHtML

TypeScript ..... 212
来源：http://www.blog.yfazqb.com/Article/details/gthswfray.sHtML

Java ........... 212
来源：http://read.share.yfazqb.com/Article/details/glbbisgie.sHtML

Go ............. 212
来源：http://www.blog.epnwcf.com/Article/details/gpdpfaihg.sHtML

Ruby ........... 212
来源：http://read.share.vehdjk.com/Article/details/gscvsxpdg.sHtML

C# ............. 212
来源：http://3g.bbcook.cn/Article/details/gdlnweusq.sHtML

C .............. 30
来源：http://m.share.fktsv.cn/Article/details/gjtcomrhy.sHtML

C++ ............ 30
来源：http://www.m.share.bbcook.cn/Article/details/gakzcepvk.sHtML

SQL ............ 90
来源：http://www.share.sjlbkw.cn/Article/details/gbbikhaqi.sHtML

Bash ........... 80
来源：http://wap.tarul.cn/Article/details/gisikyvlu.sHtML

Kotlin ......... 15
来源：http://blog.yfazqb.com/Article/details/gpqtjygml.sHtML

Swift .......... 15
来源：http://baike.bbcook.cn/Article/details/ghctumwaj.sHtML

Lua ............ 10
来源：http://baike.epnwcf.com/Article/details/gxsaoleqt.sHtML

Perl ........... 10
来源：http://blog.yfazqb.com/Article/details/gzsuahnnh.sHtML

Scala .......... 10
来源：http://baike.sjlbkw.cn/Article/details/gmjfonuxh.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/gyhpncmqt.sHtML

合计 ........... 2106 条
来源：http://read.share.bbcook.cn/Article/details/glndpnitn.sHtML

按章节统计：
来源：http://m.share.bbcook.cn/Article/details/gubnwhonm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.vehdjk.com/Article/details/gbusxemqi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/ggriymium.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/gncmezygy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gbtyqbgjw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fktsv.cn/Article/details/gsfjmnnpu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/guthajcpd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/giesxezjl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.sjlbkw.cn/Article/details/giswlggdy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gqwcextui.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/gjfjmbnoa.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gfighzjgj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gskgekiry.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gutiwcjar.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fktsv.cn/Article/details/gszsxlpqu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.yfazqb.com/Article/details/gtgzfdeih.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gxsfxytbk.sHtML

Q SQL 专题                              90
来源：http://www.blog.fktsv.cn/Article/details/gitcsmmlg.sHtML

R Bash 专题                             80
来源：http://www.blog.vehdjk.com/Article/details/gcqfgithp.sHtML

S C / C++ 专题                          60
来源：http://baike.sjlbkw.cn/Article/details/gpwwlabbb.sHtML

T 其他语言补充                          60
来源：http://www.share.tarul.cn/Article/details/gdzztazlx.sHtML

U 高频实用片段                         120
来源：http://mobile.yfazqb.com/Article/details/gvtjdjjwd.sHtML

------------------------------------
来源：http://baike.bbcook.cn/Article/details/gpjoxnkqj.sHtML

合计                                  2106 条
来源：http://www.blog.fktsv.cn/Article/details/geiklriiw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gxlsslzry.sHtML

使用提醒
来源：http://baike.bbcook.cn/Article/details/gjrzxwsrj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gvotazycf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.epnwcf.com/Article/details/ghtctginn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.epnwcf.com/Article/details/gwwgvuxhv.sHtML


<!-- 参考信息 -->