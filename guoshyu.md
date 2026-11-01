代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://wap.tarul.cn/Article/details/gfnouxycg.sHtML

[T59] Scala：循环
来源：http://read.share.fktsv.cn/Article/details/gpfcolqbo.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gzfcbqgji.sHtML

[T60] Scala：折叠
来源：http://mobile.tarul.cn/Article/details/gzwqprzul.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/gmeivtfmr.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwxpfjhog.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.bbcook.cn/Article/details/ggkslkehc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghyhuhoww.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fktsv.cn/Article/details/gnkjlulnw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.vehdjk.com/Article/details/gzhbnvtsx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.epnwcf.com/Article/details/gwzitwber.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.tarul.cn/Article/details/gqbiuhkuw.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.tarul.cn/Article/details/gprajumkn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fktsv.cn/Article/details/gtkgynltw.sHtML

[U04] Py：变量调试打印
来源：http://baike.sjlbkw.cn/Article/details/gpjrgglye.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.yfazqb.com/Article/details/gdwqwugeu.sHtML

[U05] Py：列表去重且保序
来源：http://baike.bbcook.cn/Article/details/ghhpabiln.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gqkeoguoo.sHtML

[U06] Py：合并两个字典
来源：http://baike.tarul.cn/Article/details/gvizwjflb.sHtML

{**a, **b}
来源：http://baike.yfazqb.com/Article/details/gtvrbinfe.sHtML

[U07] Py：反转字典键值
来源：http://mobile.tarul.cn/Article/details/gdkgbrulp.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.tarul.cn/Article/details/gvaohxhoo.sHtML

[U08] Py：展平二维列表
来源：http://3g.vehdjk.com/Article/details/gkcljezvb.sHtML

[y for x in nested for y in x]
来源：http://3g.fktsv.cn/Article/details/glwuwjhkn.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.yfazqb.com/Article/details/gammqsoyn.sHtML

max(d, key=d.get)
来源：http://blog.sjlbkw.cn/Article/details/gozxypscb.sHtML

[U10] Py：按值排序字典
来源：http://mobile.yfazqb.com/Article/details/gevlunyws.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.yfazqb.com/Article/details/gmtyjduea.sHtML

[U11] Py：生成器表达式
来源：http://wap.bbcook.cn/Article/details/ghddsthmz.sHtML

(x * 2 for x in arr)
来源：http://m.share.bbcook.cn/Article/details/gqposarmn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.bbcook.cn/Article/details/gsobdqiwz.sHtML

Counter(arr).most_common(3)
来源：http://blog.tarul.cn/Article/details/gtkjctmoo.sHtML

[U13] Py：固定长度队列
来源：http://mobile.yfazqb.com/Article/details/geyqrrcgv.sHtML

deque(maxlen=10)
来源：http://read.share.epnwcf.com/Article/details/gwekajljp.sHtML

[U14] Py：分组收集到列表
来源：http://3g.tarul.cn/Article/details/gyizsaxyf.sHtML

defaultdict(list)
来源：http://3g.epnwcf.com/Article/details/guxrmbsrw.sHtML

[U15] Py：高精度计时
来源：http://3g.bbcook.cn/Article/details/gcwvbbybq.sHtML

t = time.perf_counter()
来源：http://blog.sjlbkw.cn/Article/details/gxovlximd.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fktsv.cn/Article/details/ginlnajwt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.tarul.cn/Article/details/ghaeestzo.sHtML

[U17] Py：初始化日志
来源：http://baike.tarul.cn/Article/details/gkimyhinx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.sjlbkw.cn/Article/details/gmpcwgvns.sHtML

[U18] Py：预编译正则
来源：http://m.share.vehdjk.com/Article/details/gptdabzqx.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.tarul.cn/Article/details/gguhahatm.sHtML

[U19] Py：正则替换带回调
来源：http://baike.tarul.cn/Article/details/gklqijzwq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.bbcook.cn/Article/details/gofcpcmhk.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.vehdjk.com/Article/details/grgnwapso.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.yfazqb.com/Article/details/ghlthhrsw.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fktsv.cn/Article/details/gjjodzzvj.sHtML

@contextlib.contextmanager
来源：http://www.m.share.bbcook.cn/Article/details/gmimwlumq.sHtML

[U22] Py：矩阵转置
来源：http://baike.fktsv.cn/Article/details/gymgekgqh.sHtML

list(zip(*m))
来源：http://read.share.yfazqb.com/Article/details/gbvromahn.sHtML

[U23] Py：分块读取大文件
来源：http://baike.vehdjk.com/Article/details/gfxradzkk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.sjlbkw.cn/Article/details/gonuctvsq.sHtML

[U24] Py：路径操作
来源：http://m.share.yfazqb.com/Article/details/gdadzlcgf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/gnydzuzva.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.tarul.cn/Article/details/gknqwwrpn.sHtML

csv.DictReader(f)
来源：http://www.blog.yfazqb.com/Article/details/ghgikfoks.sHtML

[U26] Py：并发下载
来源：http://3g.yfazqb.com/Article/details/ghbabpwfj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fktsv.cn/Article/details/gwetvsbkj.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fktsv.cn/Article/details/giqjskmzt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.tarul.cn/Article/details/gduyggimp.sHtML

[U28] Py：类型别名
来源：http://www.blog.tarul.cn/Article/details/gmmbkfxis.sHtML

UserId = int
来源：http://mobile.fktsv.cn/Article/details/glndugrmn.sHtML

[U29] Py：属性校验
来源：http://read.share.bbcook.cn/Article/details/gmbaufdwh.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.epnwcf.com/Article/details/gfkvrivrv.sHtML

[U30] Py：数据类
来源：http://m.share.epnwcf.com/Article/details/gjillljpp.sHtML

@dataclass(slots=True)
来源：http://3g.fktsv.cn/Article/details/gnbctpzvc.sHtML

[U31] Py：单测
来源：http://mobile.yfazqb.com/Article/details/grieixamq.sHtML

python -m pytest -q
来源：http://read.share.fktsv.cn/Article/details/guqgaqqez.sHtML

[U32] Py：代码格式化
来源：http://baike.sjlbkw.cn/Article/details/gpkolcwje.sHtML

ruff format . && ruff check --fix .
来源：http://blog.tarul.cn/Article/details/gyloyqqpu.sHtML

[U33] Py：打包发布
来源：http://www.share.fktsv.cn/Article/details/gnqdzukxc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.bbcook.cn/Article/details/gtzwywiha.sHtML

[U34] Py：判断编码
来源：http://wap.fktsv.cn/Article/details/gggylffof.sHtML

chardet.detect(raw)
来源：http://m.share.sjlbkw.cn/Article/details/gdvutbgan.sHtML

[U35] Py：发送邮件
来源：http://www.blog.yfazqb.com/Article/details/gqwoiiczy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.yfazqb.com/Article/details/gnfjlubrq.sHtML

[U36] Py：定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gbqskrfdf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.vehdjk.com/Article/details/gawtnsgge.sHtML

[U37] Py：读写 Excel
来源：http://www.share.sjlbkw.cn/Article/details/gnpvmlora.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.epnwcf.com/Article/details/gvyyojxtk.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.bbcook.cn/Article/details/gvsjjuwml.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fktsv.cn/Article/details/gmmpuprhk.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.bbcook.cn/Article/details/ggdkqbzuh.sHtML

sys.stdout.isatty()
来源：http://read.share.sjlbkw.cn/Article/details/gdhnudmkj.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.vehdjk.com/Article/details/goeanqzld.sHtML

print("err", file=sys.stderr)
来源：http://mobile.yfazqb.com/Article/details/gxvcmcppk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.bbcook.cn/Article/details/gijyzwfgf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.yfazqb.com/Article/details/gwrrmydpa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.bbcook.cn/Article/details/gxwrztoax.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.bbcook.cn/Article/details/gonzmyxag.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.tarul.cn/Article/details/gemeoqqlu.sHtML

namespace App\Http;
来源：http://read.share.vehdjk.com/Article/details/gdplieugv.sHtML

[U44] PHP：开启严格类型
来源：http://wap.tarul.cn/Article/details/gzbycenel.sHtML

declare(strict_types=1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxhmboua.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.vehdjk.com/Article/details/gxxlyuccs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/glbvrlrpg.sHtML

[U46] PHP：可空类型
来源：http://blog.sjlbkw.cn/Article/details/gsdybwyfp.sHtML

?string $name = null
来源：http://www.share.fktsv.cn/Article/details/gfolxztec.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.vehdjk.com/Article/details/gjlsaukve.sHtML

int|string $id
来源：http://read.share.bbcook.cn/Article/details/gcotgvqxz.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fktsv.cn/Article/details/ghellgmtu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fktsv.cn/Article/details/gtlfpdsip.sHtML

[U49] PHP：只读属性
来源：http://m.share.bbcook.cn/Article/details/gsdjrpsee.sHtML

public readonly string $name
来源：http://blog.vehdjk.com/Article/details/gjmlduqrj.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.bbcook.cn/Article/details/gsbbwicqd.sHtML

public function __construct(private int $id) {}
来源：http://read.share.bbcook.cn/Article/details/ghmujqdaf.sHtML

[U51] PHP：数组解构
来源：http://wap.epnwcf.com/Article/details/gdauxbbzt.sHtML

[$a, $b] = $arr;
来源：http://mobile.yfazqb.com/Article/details/ghxmcuhed.sHtML

[U52] PHP：箭头函数
来源：http://read.share.yfazqb.com/Article/details/gvsmzpfah.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.bbcook.cn/Article/details/ggbznfqyd.sHtML

[U53] PHP：空合并运算符
来源：http://blog.sjlbkw.cn/Article/details/ghkkwniex.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fktsv.cn/Article/details/geveaoviu.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.yfazqb.com/Article/details/gfjunwzvx.sHtML

$obj?->method()
来源：http://baike.yfazqb.com/Article/details/gjfnkcmne.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.epnwcf.com/Article/details/ggmkwewsi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fktsv.cn/Article/details/gfqopwgcx.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.tarul.cn/Article/details/gpnmguale.sHtML

f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gkrkjhiws.sHtML

[U57] PHP：字符串插值
来源：http://wap.fktsv.cn/Article/details/gtcbfaymo.sHtML

"值: {$a}"
来源：http://3g.tarul.cn/Article/details/gddeikiir.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fktsv.cn/Article/details/gdfesaqwj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.epnwcf.com/Article/details/gypktzygw.sHtML

[U59] PHP：自定义排序
来源：http://mobile.vehdjk.com/Article/details/gzlxgqvxh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/ggjypvgrl.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.bbcook.cn/Article/details/gonlsdfeo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.bbcook.cn/Article/details/gizrmdean.sHtML

[U61] PHP：正则
来源：http://www.blog.bbcook.cn/Article/details/gnixdczzu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fktsv.cn/Article/details/gnoshdtry.sHtML

[U62] PHP：日期对象
来源：http://3g.yfazqb.com/Article/details/gbejorurm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fktsv.cn/Article/details/gpifdjnnt.sHtML

[U63] PHP：文件读写
来源：http://3g.fktsv.cn/Article/details/gouwigngf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.epnwcf.com/Article/details/guxewuphm.sHtML

[U64] PHP：目录遍历
来源：http://blog.sjlbkw.cn/Article/details/gbyratzsx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.yfazqb.com/Article/details/gtqavpdaf.sHtML

[U65] PHP：会话
来源：http://wap.fktsv.cn/Article/details/gyifhbqcj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.epnwcf.com/Article/details/gfbjyhzdd.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.bbcook.cn/Article/details/gkuohfuyk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.vehdjk.com/Article/details/gruwuqydd.sHtML

[U67] PHP：处理文件上传
来源：http://3g.yfazqb.com/Article/details/gbfsofmjn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.yfazqb.com/Article/details/gkenhwjai.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.vehdjk.com/Article/details/goinbilui.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.sjlbkw.cn/Article/details/gbdpwwrqw.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.vehdjk.com/Article/details/gclmrxizs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.tarul.cn/Article/details/glqaqnqme.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.yfazqb.com/Article/details/gmgdhoqci.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.vehdjk.com/Article/details/gbfpettko.sHtML

[U71] PHP：抛出异常
来源：http://mobile.sjlbkw.cn/Article/details/gwycvzuew.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.sjlbkw.cn/Article/details/gkenihkga.sHtML

[U72] PHP：写错误日志
来源：http://mobile.epnwcf.com/Article/details/gpgjirllv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.bbcook.cn/Article/details/gblkqywig.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.yfazqb.com/Article/details/gmvcmlbkn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.tarul.cn/Article/details/glhoioysd.sHtML

[U74] PHP：读取环境变量
来源：http://baike.yfazqb.com/Article/details/giexhnxxd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.epnwcf.com/Article/details/ggrnooysw.sHtML

[U75] PHP：依赖注入
来源：http://wap.bbcook.cn/Article/details/gciofojlz.sHtML

composer require psr/container
来源：http://wap.bbcook.cn/Article/details/gcbwffobc.sHtML

[U76] PHP：简单路由
来源：http://mobile.fktsv.cn/Article/details/gayspbiga.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.vehdjk.com/Article/details/gdozoujsd.sHtML

[U77] PHP：模板渲染
来源：http://baike.fktsv.cn/Article/details/gheyrlvgp.sHtML

composer require twig/twig
来源：http://www.m.share.vehdjk.com/Article/details/gdkettjkb.sHtML

[U78] PHP：单元测试
来源：http://m.share.vehdjk.com/Article/details/gucnjlirg.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.bbcook.cn/Article/details/gratbewdx.sHtML

[U79] PHP：静态分析
来源：http://read.share.sjlbkw.cn/Article/details/gcyfmsyou.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.sjlbkw.cn/Article/details/gwkhfsegn.sHtML

[U80] PHP：代码规范修复
来源：http://3g.tarul.cn/Article/details/gskkkfaln.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.yfazqb.com/Article/details/gtxddifqd.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.yfazqb.com/Article/details/ggbimaojh.sHtML

npm init -y;  npm i express
来源：http://3g.sjlbkw.cn/Article/details/grdifsmby.sHtML

[U82] JS：package.json 脚本
来源：http://blog.vehdjk.com/Article/details/gqiheywuz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.tarul.cn/Article/details/glxfmydpx.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.sjlbkw.cn/Article/details/gqxshxvmf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.vehdjk.com/Article/details/gytykidhg.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.bbcook.cn/Article/details/gywzvmdgd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.sjlbkw.cn/Article/details/ghurkdnor.sHtML

[U85] JS：可选链
来源：http://3g.yfazqb.com/Article/details/gpnidfiwo.sHtML

a?.b?.c
来源：http://www.m.share.tarul.cn/Article/details/gymjjkano.sHtML

[U86] JS：空值合并
来源：http://mobile.sjlbkw.cn/Article/details/gvvutuzmz.sHtML

a ?? b
来源：http://read.share.fktsv.cn/Article/details/gkhcihxpf.sHtML

[U87] JS：解构默认值
来源：http://mobile.vehdjk.com/Article/details/gysppjijd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.vehdjk.com/Article/details/gpmrsinhd.sHtML

[U88] JS：对象展开合并
来源：http://m.share.tarul.cn/Article/details/gsuxghgdt.sHtML

{ ...a, ...b }
来源：http://www.m.share.yfazqb.com/Article/details/gfaqhapsx.sHtML

[U89] JS：数组去重
来源：http://m.share.vehdjk.com/Article/details/gjfvdhdvi.sHtML

[...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gdkpcegyf.sHtML

[U90] JS：数字数组排序
来源：http://mobile.tarul.cn/Article/details/guoelxefo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gykskicxn.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.bbcook.cn/Article/details/gdhntxidq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.vehdjk.com/Article/details/gplfgprav.sHtML

[U92] JS：深拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gydqrpnyb.sHtML

structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gybwfwqpx.sHtML

[U93] JS：模板字符串
来源：http://read.share.vehdjk.com/Article/details/gpzmgjhon.sHtML

`共 ${n} 条`
来源：http://www.share.epnwcf.com/Article/details/gtqvpfpfs.sHtML

[U94] JS：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/gqhfobwsm.sHtML

const double = x => x * 2;
来源：http://www.share.bbcook.cn/Article/details/gnfaskjrz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.yfazqb.com/Article/details/gaankcryd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.vehdjk.com/Article/details/gssejkqny.sHtML

[U96] JS：async/await 与异常
来源：http://3g.yfazqb.com/Article/details/gzyigjury.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gjaxbhluk.sHtML

[U97] JS：并发请求
来源：http://3g.yfazqb.com/Article/details/gkbflvqly.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gsrhawdnz.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.yfazqb.com/Article/details/gpljijnfx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fktsv.cn/Article/details/guztcjahx.sHtML

[U99] JS：事件监听
来源：http://www.m.share.yfazqb.com/Article/details/gwwhrpzrm.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.sjlbkw.cn/Article/details/gxcqgxzyu.sHtML

[U100] JS：DOM 查询
来源：http://mobile.vehdjk.com/Article/details/gaksilurk.sHtML

document.querySelector(".item")
来源：http://wap.vehdjk.com/Article/details/gezqxksob.sHtML

[U101] JS：classList 操作
来源：http://wap.sjlbkw.cn/Article/details/gaecbsdee.sHtML

el.classList.toggle("active")
来源：http://www.share.bbcook.cn/Article/details/gswuiuvai.sHtML

[U102] JS：本地存储
来源：http://m.share.bbcook.cn/Article/details/gqfvuggnr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.tarul.cn/Article/details/gekabdweo.sHtML

[U103] JS：定时器
来源：http://read.share.fktsv.cn/Article/details/gaumapfuy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.epnwcf.com/Article/details/glpgiikqb.sHtML

[U104] JS：防抖
来源：http://3g.yfazqb.com/Article/details/gidctbhzw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/grbslvzbu.sHtML

[U105] JS：节流
来源：http://mobile.bbcook.cn/Article/details/gyktdkdsm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.tarul.cn/Article/details/gyhlfeqjv.sHtML

[U106] JS：日期格式化
来源：http://www.share.bbcook.cn/Article/details/gzxkhsvyv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.tarul.cn/Article/details/gohxvxnag.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.bbcook.cn/Article/details/gxlkcxaiy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.tarul.cn/Article/details/gdsaoscxj.sHtML

[U108] JS：随机整数
来源：http://wap.yfazqb.com/Article/details/gnatyohpj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.bbcook.cn/Article/details/gidskfbow.sHtML

[U109] JS：数组分组
来源：http://wap.yfazqb.com/Article/details/gjgsufjhu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gnlseiyfy.sHtML

[U110] JS：数组分块
来源：http://read.share.yfazqb.com/Article/details/gywwmxgpv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.yfazqb.com/Article/details/gbcradaed.sHtML

[U111] JS：对象转 Map
来源：http://www.share.sjlbkw.cn/Article/details/gxymfodis.sHtML

new Map(Object.entries(obj))
来源：http://m.share.epnwcf.com/Article/details/gquhiityx.sHtML

[U112] JS：字符串补位
来源：http://baike.sjlbkw.cn/Article/details/grqkvoekh.sHtML

"7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gojklixka.sHtML

[U113] JS：正则替换全部
来源：http://wap.sjlbkw.cn/Article/details/gaslvvoat.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/grnqmahdc.sHtML

[U114] JS：JSON 深比较
来源：http://blog.tarul.cn/Article/details/gjthuflvf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.bbcook.cn/Article/details/gmajetigz.sHtML

[U115] JS：生成 UUID
来源：http://mobile.tarul.cn/Article/details/gzzbziakx.sHtML

crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gmyqvtprw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.vehdjk.com/Article/details/gkjxnopmo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.vehdjk.com/Article/details/gpstywplz.sHtML

[U117] JS：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gqiazqfdj.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fktsv.cn/Article/details/grorvifmc.sHtML

[U118] JS：开发服务器
来源：http://blog.tarul.cn/Article/details/grthtdvrt.sHtML

npm i -D vite;  npx vite
来源：http://blog.bbcook.cn/Article/details/gpewqgrsd.sHtML

[U119] JS：生产构建
来源：http://m.share.fktsv.cn/Article/details/gvvtggfwo.sHtML

npx vite build
来源：http://www.m.share.tarul.cn/Article/details/garfseqld.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.epnwcf.com/Article/details/gfimjalhk.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.sjlbkw.cn/Article/details/gjfxqcgdu.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfcfuqgfa.sHtML

统计汇总
来源：http://blog.fktsv.cn/Article/details/goalpqlqn.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gresangoy.sHtML

按语言统计（条）：
来源：http://read.share.fktsv.cn/Article/details/ggcmtgfgv.sHtML

Python ......... 252
来源：http://read.share.bbcook.cn/Article/details/gwlpxrtya.sHtML

PHP ............ 252
来源：http://baike.fktsv.cn/Article/details/gzfidvaks.sHtML

JavaScript ..... 252
来源：http://www.m.share.tarul.cn/Article/details/gapcpnsqx.sHtML

TypeScript ..... 212
来源：http://wap.yfazqb.com/Article/details/gxrxcthox.sHtML

Java ........... 212
来源：http://www.share.yfazqb.com/Article/details/gtkmmifju.sHtML

Go ............. 212
来源：http://www.blog.sjlbkw.cn/Article/details/gsscxekxs.sHtML

Ruby ........... 212
来源：http://3g.yfazqb.com/Article/details/goixbcijc.sHtML

C# ............. 212
来源：http://m.share.fktsv.cn/Article/details/ggybmrhkn.sHtML

C .............. 30
来源：http://mobile.vehdjk.com/Article/details/gkgpostin.sHtML

C++ ............ 30
来源：http://mobile.bbcook.cn/Article/details/gqswdadhu.sHtML

SQL ............ 90
来源：http://mobile.yfazqb.com/Article/details/ghyamfybl.sHtML

Bash ........... 80
来源：http://m.share.epnwcf.com/Article/details/ggsuwcgvg.sHtML

Kotlin ......... 15
来源：http://www.m.share.epnwcf.com/Article/details/gnfettdpg.sHtML

Swift .......... 15
来源：http://www.blog.fktsv.cn/Article/details/gsordykgp.sHtML

Lua ............ 10
来源：http://mobile.fktsv.cn/Article/details/gcpofvtig.sHtML

Perl ........... 10
来源：http://www.m.share.epnwcf.com/Article/details/gfrvdasxx.sHtML

Scala .......... 10
来源：http://baike.tarul.cn/Article/details/gcrnanqca.sHtML

------------------------------------
来源：http://wap.vehdjk.com/Article/details/gweszbnss.sHtML

合计 ........... 2106 条
来源：http://3g.bbcook.cn/Article/details/ggjafuuhh.sHtML

按章节统计：
来源：http://www.blog.bbcook.cn/Article/details/gzlhptbaq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.yfazqb.com/Article/details/graqgujbr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/golajcvuk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gxmifesxm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.sjlbkw.cn/Article/details/gacgrmdsb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.yfazqb.com/Article/details/gzgsznmip.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.tarul.cn/Article/details/grmvmdduy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/givmwzsqu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/glguwbymh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gifjqzvkh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.vehdjk.com/Article/details/gvjklryfw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/giitggsiu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gjavzxmso.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gcaxwdqcs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fktsv.cn/Article/details/gewlblbfw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.epnwcf.com/Article/details/godkskbyp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gmxhiqncz.sHtML

Q SQL 专题                              90
来源：http://m.share.bbcook.cn/Article/details/gsitmjsrm.sHtML

R Bash 专题                             80
来源：http://wap.epnwcf.com/Article/details/gwpuyazqb.sHtML

S C / C++ 专题                          60
来源：http://www.share.vehdjk.com/Article/details/gblihkqzs.sHtML

T 其他语言补充                          60
来源：http://www.m.share.yfazqb.com/Article/details/gvpppkpce.sHtML

U 高频实用片段                         120
来源：http://wap.bbcook.cn/Article/details/ggctkzkkp.sHtML

------------------------------------
来源：http://blog.bbcook.cn/Article/details/gjhtxnaen.sHtML

合计                                  2106 条
来源：http://baike.epnwcf.com/Article/details/gzdybtohe.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/ggjlposyg.sHtML

使用提醒
来源：http://read.share.vehdjk.com/Article/details/gocomaxpt.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gkucjyzmo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.sjlbkw.cn/Article/details/gsseomxpx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.yfazqb.com/Article/details/ganfsrfgl.sHtML


<!-- 参考信息 -->