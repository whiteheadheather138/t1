代发 wailian999

case class User(name: String, age: Int)
来源：http://m.share.tarul.cn/Article/details/gfdhgctqa.sHtML

[T57] Scala：模式匹配
来源：http://baike.epnwcf.com/Article/details/gceujkdtx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fktsv.cn/Article/details/gqjeuqfcy.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fktsv.cn/Article/details/gahvqvavx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fktsv.cn/Article/details/guhmpqkzs.sHtML

[T59] Scala：循环
来源：http://www.m.share.fktsv.cn/Article/details/gheffcfqq.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fktsv.cn/Article/details/gdzuixygg.sHtML

[T60] Scala：折叠
来源：http://mobile.vehdjk.com/Article/details/guecjbskw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.epnwcf.com/Article/details/ggednxnvh.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gntqqoiea.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/ghvkxpcgx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzsgiuujq.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.vehdjk.com/Article/details/ghfdymcog.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.sjlbkw.cn/Article/details/ggooaqext.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fktsv.cn/Article/details/grorotjbq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.bbcook.cn/Article/details/gqofalsbl.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.bbcook.cn/Article/details/gxnlandqu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.epnwcf.com/Article/details/gxeigexvy.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.yfazqb.com/Article/details/gsvxasugr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.vehdjk.com/Article/details/gbwuncgrk.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.bbcook.cn/Article/details/gwxmidcvn.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gmjhbmesj.sHtML

[U06] Py：合并两个字典
来源：http://blog.fktsv.cn/Article/details/gvjmtxjzh.sHtML

{**a, **b}
来源：http://wap.tarul.cn/Article/details/gemziymfu.sHtML

[U07] Py：反转字典键值
来源：http://baike.tarul.cn/Article/details/gcfwsyema.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fktsv.cn/Article/details/gkrloualj.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gpekadpge.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/gbulcadrv.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fktsv.cn/Article/details/gtiubqpvb.sHtML

max(d, key=d.get)
来源：http://www.share.epnwcf.com/Article/details/gxmuemvos.sHtML

[U10] Py：按值排序字典
来源：http://wap.yfazqb.com/Article/details/gfsxajmxm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.tarul.cn/Article/details/gwkqobfhj.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.bbcook.cn/Article/details/gfzzexqhq.sHtML

(x * 2 for x in arr)
来源：http://baike.yfazqb.com/Article/details/ghhibapad.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fktsv.cn/Article/details/gqyidchxk.sHtML

Counter(arr).most_common(3)
来源：http://3g.fktsv.cn/Article/details/gfktxgjdz.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fktsv.cn/Article/details/gjkrwkial.sHtML

deque(maxlen=10)
来源：http://blog.fktsv.cn/Article/details/gtvcwvaum.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fktsv.cn/Article/details/gamynmjvp.sHtML

defaultdict(list)
来源：http://m.share.yfazqb.com/Article/details/gfagjciyg.sHtML

[U15] Py：高精度计时
来源：http://read.share.vehdjk.com/Article/details/gjnyomgod.sHtML

t = time.perf_counter()
来源：http://wap.bbcook.cn/Article/details/gxcofjyln.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.bbcook.cn/Article/details/gcctwjukb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.bbcook.cn/Article/details/gcizburvd.sHtML

[U17] Py：初始化日志
来源：http://www.blog.yfazqb.com/Article/details/gzkodxchh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.vehdjk.com/Article/details/gcptbeppr.sHtML

[U18] Py：预编译正则
来源：http://m.share.yfazqb.com/Article/details/gtwkxvhhb.sHtML

pat = re.compile(r"\d+")
来源：http://wap.yfazqb.com/Article/details/gumhbqjpb.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.bbcook.cn/Article/details/gczjozeqj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.bbcook.cn/Article/details/gsamzbfvv.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/gbkqtptst.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.vehdjk.com/Article/details/gdwzlwner.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fktsv.cn/Article/details/gxizfirri.sHtML

@contextlib.contextmanager
来源：http://baike.vehdjk.com/Article/details/gummwiwor.sHtML

[U22] Py：矩阵转置
来源：http://www.share.bbcook.cn/Article/details/gdfganhwz.sHtML

list(zip(*m))
来源：http://mobile.yfazqb.com/Article/details/gfybkbzni.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.bbcook.cn/Article/details/geerjpjrr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.vehdjk.com/Article/details/gfennqpbk.sHtML

[U24] Py：路径操作
来源：http://read.share.vehdjk.com/Article/details/ghkepadbd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gsakxqvxy.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.vehdjk.com/Article/details/gcidhzatn.sHtML

csv.DictReader(f)
来源：http://3g.fktsv.cn/Article/details/gorgipenx.sHtML

[U26] Py：并发下载
来源：http://wap.tarul.cn/Article/details/gpgtpyrtv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.tarul.cn/Article/details/gcysgyskc.sHtML

[U27] Py：异步 HTTP
来源：http://baike.yfazqb.com/Article/details/gyuwqokaj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.sjlbkw.cn/Article/details/gabbdqsvu.sHtML

[U28] Py：类型别名
来源：http://3g.bbcook.cn/Article/details/gushmubzf.sHtML

UserId = int
来源：http://3g.fktsv.cn/Article/details/gyxrsxifu.sHtML

[U29] Py：属性校验
来源：http://m.share.vehdjk.com/Article/details/gpvqcklvw.sHtML

@property 与 @x.setter 配合
来源：http://baike.yfazqb.com/Article/details/gvbwoouei.sHtML

[U30] Py：数据类
来源：http://blog.yfazqb.com/Article/details/gakybsdpm.sHtML

@dataclass(slots=True)
来源：http://www.m.share.bbcook.cn/Article/details/gmtautyqy.sHtML

[U31] Py：单测
来源：http://baike.sjlbkw.cn/Article/details/ghmdrdbgl.sHtML

python -m pytest -q
来源：http://blog.bbcook.cn/Article/details/grrjoowqf.sHtML

[U32] Py：代码格式化
来源：http://www.share.bbcook.cn/Article/details/gdddworcr.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.sjlbkw.cn/Article/details/ghkokpewc.sHtML

[U33] Py：打包发布
来源：http://www.m.share.vehdjk.com/Article/details/gaauiyekh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fktsv.cn/Article/details/gydofqowb.sHtML

[U34] Py：判断编码
来源：http://3g.sjlbkw.cn/Article/details/gclgqgdbl.sHtML

chardet.detect(raw)
来源：http://www.m.share.fktsv.cn/Article/details/gsksasapz.sHtML

[U35] Py：发送邮件
来源：http://www.blog.sjlbkw.cn/Article/details/gfpfeqnrs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.bbcook.cn/Article/details/gojnfmddc.sHtML

[U36] Py：定时任务
来源：http://blog.sjlbkw.cn/Article/details/gwbpwurub.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.sjlbkw.cn/Article/details/glhpngxjb.sHtML

[U37] Py：读写 Excel
来源：http://wap.fktsv.cn/Article/details/gvkhrvbym.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.bbcook.cn/Article/details/gvkbtngza.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.vehdjk.com/Article/details/gkvqrvycb.sHtML

Path(__file__).resolve().parent
来源：http://wap.yfazqb.com/Article/details/gilsgnnbt.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.yfazqb.com/Article/details/gflksibyi.sHtML

sys.stdout.isatty()
来源：http://3g.epnwcf.com/Article/details/gceiohzoa.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.bbcook.cn/Article/details/gikutbupc.sHtML

print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gejkdznsg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.epnwcf.com/Article/details/ghivmxyeu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.bbcook.cn/Article/details/ggusnzoen.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.yfazqb.com/Article/details/gidnuiicl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fktsv.cn/Article/details/ggczalxbw.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.vehdjk.com/Article/details/glxpnidoh.sHtML

namespace App\Http;
来源：http://www.m.share.yfazqb.com/Article/details/grrqvajvs.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fktsv.cn/Article/details/gkjzsljcx.sHtML

declare(strict_types=1);
来源：http://www.m.share.sjlbkw.cn/Article/details/geaxqzqml.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fktsv.cn/Article/details/gibrkstbv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gxlfulpkq.sHtML

[U46] PHP：可空类型
来源：http://blog.tarul.cn/Article/details/gpfrivdsl.sHtML

?string $name = null
来源：http://blog.sjlbkw.cn/Article/details/gycvugbdy.sHtML

[U47] PHP：联合类型
来源：http://www.share.vehdjk.com/Article/details/gcdrugesn.sHtML

int|string $id
来源：http://baike.yfazqb.com/Article/details/gggyffwel.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fktsv.cn/Article/details/ggtyfgmxn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.vehdjk.com/Article/details/gdulaoapk.sHtML

[U49] PHP：只读属性
来源：http://blog.sjlbkw.cn/Article/details/gfhfqwran.sHtML

public readonly string $name
来源：http://www.blog.tarul.cn/Article/details/gvvqyioez.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.yfazqb.com/Article/details/gfkunfnnl.sHtML

public function __construct(private int $id) {}
来源：http://www.share.vehdjk.com/Article/details/gqqoanvmy.sHtML

[U51] PHP：数组解构
来源：http://3g.sjlbkw.cn/Article/details/gwiqiirmm.sHtML

[$a, $b] = $arr;
来源：http://blog.bbcook.cn/Article/details/gpuqkmxkv.sHtML

[U52] PHP：箭头函数
来源：http://wap.epnwcf.com/Article/details/gzenzrfdo.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fktsv.cn/Article/details/gkmlxlqez.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.epnwcf.com/Article/details/gtynyfond.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.epnwcf.com/Article/details/geeohrduo.sHtML

[U54] PHP：空安全调用
来源：http://read.share.epnwcf.com/Article/details/gnwrthkpm.sHtML

$obj?->method()
来源：http://read.share.sjlbkw.cn/Article/details/gyynwljjv.sHtML

[U55] PHP：match 表达式
来源：http://www.share.yfazqb.com/Article/details/gtllfuqvv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.epnwcf.com/Article/details/grkfbnvnr.sHtML

[U56] PHP：命名参数
来源：http://m.share.vehdjk.com/Article/details/gjrpziuly.sHtML

f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gkdchgnig.sHtML

[U57] PHP：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gbgrdiiti.sHtML

"值: {$a}"
来源：http://www.m.share.yfazqb.com/Article/details/gkfsxfnnd.sHtML

[U58] PHP：数组三件套
来源：http://www.share.vehdjk.com/Article/details/gssxqxsja.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.bbcook.cn/Article/details/gwlwuivqu.sHtML

[U59] PHP：自定义排序
来源：http://wap.yfazqb.com/Article/details/gxtihsyux.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fktsv.cn/Article/details/gazusdzcx.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/gphjdlmnu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.yfazqb.com/Article/details/gdcziuupw.sHtML

[U61] PHP：正则
来源：http://read.share.epnwcf.com/Article/details/gljcwbtrn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/ghlslehtq.sHtML

[U62] PHP：日期对象
来源：http://www.share.tarul.cn/Article/details/gdhnyufys.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.bbcook.cn/Article/details/ggsopyvar.sHtML

[U63] PHP：文件读写
来源：http://baike.bbcook.cn/Article/details/giebjojwz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.bbcook.cn/Article/details/gpqympsbe.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.epnwcf.com/Article/details/gydashnvu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.bbcook.cn/Article/details/gbofvppxc.sHtML

[U65] PHP：会话
来源：http://blog.bbcook.cn/Article/details/gwsbqbxno.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gttzimybs.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.bbcook.cn/Article/details/gjoapzhlw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.bbcook.cn/Article/details/gdtsnftqf.sHtML

[U67] PHP：处理文件上传
来源：http://3g.sjlbkw.cn/Article/details/gfuyswnkd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.epnwcf.com/Article/details/grwnhytrr.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.yfazqb.com/Article/details/gyijogjbw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.tarul.cn/Article/details/gbljhamho.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.tarul.cn/Article/details/gmyvrblck.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.bbcook.cn/Article/details/glkxyakpo.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.sjlbkw.cn/Article/details/gpvbwijdv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.yfazqb.com/Article/details/grmwrmwmz.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gouwvfcvq.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.vehdjk.com/Article/details/gmlrbomfg.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gqluammoy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.bbcook.cn/Article/details/genetpgnt.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fktsv.cn/Article/details/ggvwixvng.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.sjlbkw.cn/Article/details/gmvpskmsi.sHtML

[U74] PHP：读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/gdmyglsuv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.bbcook.cn/Article/details/gpewvmsfd.sHtML

[U75] PHP：依赖注入
来源：http://mobile.vehdjk.com/Article/details/gajmsvcqj.sHtML

composer require psr/container
来源：http://www.blog.fktsv.cn/Article/details/gcrldmcdp.sHtML

[U76] PHP：简单路由
来源：http://blog.bbcook.cn/Article/details/gytbgbefu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.tarul.cn/Article/details/gnyikaiik.sHtML

[U77] PHP：模板渲染
来源：http://baike.tarul.cn/Article/details/gaxdalyyn.sHtML

composer require twig/twig
来源：http://3g.vehdjk.com/Article/details/gdfomocql.sHtML

[U78] PHP：单元测试
来源：http://3g.vehdjk.com/Article/details/gacupcmyg.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.epnwcf.com/Article/details/gesoeufmw.sHtML

[U79] PHP：静态分析
来源：http://www.blog.sjlbkw.cn/Article/details/grwjbdwtw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fktsv.cn/Article/details/glrkplrif.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fktsv.cn/Article/details/gshhgazne.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.bbcook.cn/Article/details/gilhalghd.sHtML

[U81] JS：初始化项目
来源：http://m.share.fktsv.cn/Article/details/govaarpze.sHtML

npm init -y;  npm i express
来源：http://www.m.share.yfazqb.com/Article/details/gypbfgulq.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.bbcook.cn/Article/details/gonevvtnt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.bbcook.cn/Article/details/gnkjhpuxd.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fktsv.cn/Article/details/ghbyfczeq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fktsv.cn/Article/details/gdgrlshqa.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.vehdjk.com/Article/details/ggafqevsu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.yfazqb.com/Article/details/gqkeagrgx.sHtML

[U85] JS：可选链
来源：http://www.share.sjlbkw.cn/Article/details/gussbwpoe.sHtML

a?.b?.c
来源：http://www.share.fktsv.cn/Article/details/gducqevcr.sHtML

[U86] JS：空值合并
来源：http://mobile.tarul.cn/Article/details/gzsszzrze.sHtML

a ?? b
来源：http://blog.fktsv.cn/Article/details/gzpllnxsd.sHtML

[U87] JS：解构默认值
来源：http://read.share.bbcook.cn/Article/details/gqfnixmka.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.yfazqb.com/Article/details/gxrphdzet.sHtML

[U88] JS：对象展开合并
来源：http://www.share.yfazqb.com/Article/details/grlanryxv.sHtML

{ ...a, ...b }
来源：http://3g.vehdjk.com/Article/details/gwkonkagr.sHtML

[U89] JS：数组去重
来源：http://wap.vehdjk.com/Article/details/gteddoasf.sHtML

[...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gboetgoue.sHtML

[U90] JS：数字数组排序
来源：http://3g.bbcook.cn/Article/details/gnriamlgu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gftbdqwwl.sHtML

[U91] JS：对象键值遍历
来源：http://baike.yfazqb.com/Article/details/gpyrtrdww.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.sjlbkw.cn/Article/details/gzydmhpye.sHtML

[U92] JS：深拷贝
来源：http://baike.sjlbkw.cn/Article/details/gkrbsfefs.sHtML

structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gcokionrt.sHtML

[U93] JS：模板字符串
来源：http://mobile.epnwcf.com/Article/details/gflqpfzwr.sHtML

`共 ${n} 条`
来源：http://wap.yfazqb.com/Article/details/gysmvfhhd.sHtML

[U94] JS：箭头函数
来源：http://www.share.tarul.cn/Article/details/grxtwfxgm.sHtML

const double = x => x * 2;
来源：http://blog.epnwcf.com/Article/details/gcthwlxuh.sHtML

[U95] JS：Promise 包装
来源：http://mobile.vehdjk.com/Article/details/gfnhbedbg.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.tarul.cn/Article/details/gdcvcklji.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.yfazqb.com/Article/details/gaczzdtpm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gmcjrugdx.sHtML

[U97] JS：并发请求
来源：http://blog.vehdjk.com/Article/details/gsciokznu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/ggrjzeozx.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.tarul.cn/Article/details/gvvkmefwo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.yfazqb.com/Article/details/gwffdhcvc.sHtML

[U99] JS：事件监听
来源：http://read.share.yfazqb.com/Article/details/gxwhzduym.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.vehdjk.com/Article/details/ggmpnbwtm.sHtML

[U100] JS：DOM 查询
来源：http://baike.yfazqb.com/Article/details/grkfudyzg.sHtML

document.querySelector(".item")
来源：http://www.share.bbcook.cn/Article/details/gkajyzygz.sHtML

[U101] JS：classList 操作
来源：http://read.share.sjlbkw.cn/Article/details/geqagwybn.sHtML

el.classList.toggle("active")
来源：http://www.m.share.vehdjk.com/Article/details/gcrfpiyeu.sHtML

[U102] JS：本地存储
来源：http://read.share.fktsv.cn/Article/details/gvbuqhslg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.vehdjk.com/Article/details/gpclumxvc.sHtML

[U103] JS：定时器
来源：http://mobile.bbcook.cn/Article/details/gpmzsqpmn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.tarul.cn/Article/details/gmapxzlww.sHtML

[U104] JS：防抖
来源：http://www.blog.sjlbkw.cn/Article/details/gmfiamypg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gsuvadcsb.sHtML

[U105] JS：节流
来源：http://www.m.share.epnwcf.com/Article/details/ggxficllv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.sjlbkw.cn/Article/details/gzrthywgt.sHtML

[U106] JS：日期格式化
来源：http://m.share.fktsv.cn/Article/details/grzwvopsf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fktsv.cn/Article/details/gwpjtelsk.sHtML

[U107] JS：数字千分位
来源：http://mobile.epnwcf.com/Article/details/gavsqcyhv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbonpixn.sHtML

[U108] JS：随机整数
来源：http://baike.sjlbkw.cn/Article/details/ggjpngspx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.yfazqb.com/Article/details/gswqgeqmn.sHtML

[U109] JS：数组分组
来源：http://blog.tarul.cn/Article/details/gsgjtltre.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.epnwcf.com/Article/details/gtisxstvx.sHtML

[U110] JS：数组分块
来源：http://baike.vehdjk.com/Article/details/gddzirjbb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.vehdjk.com/Article/details/godbknjmd.sHtML

[U111] JS：对象转 Map
来源：http://3g.bbcook.cn/Article/details/gdhjbnpwm.sHtML

new Map(Object.entries(obj))
来源：http://m.share.yfazqb.com/Article/details/ghvfyveot.sHtML

[U112] JS：字符串补位
来源：http://3g.epnwcf.com/Article/details/grlihjsfv.sHtML

"7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gurqmlvhv.sHtML

[U113] JS：正则替换全部
来源：http://3g.epnwcf.com/Article/details/gnrcxtrqc.sHtML

s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gkzadrqic.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fktsv.cn/Article/details/gpmwefusc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.bbcook.cn/Article/details/gwwavrdlv.sHtML

[U115] JS：生成 UUID
来源：http://3g.fktsv.cn/Article/details/gnozoynjr.sHtML

crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gnvendlfh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.vehdjk.com/Article/details/gfgqanpvr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.sjlbkw.cn/Article/details/gmcjxgjtk.sHtML

[U117] JS：单元测试
来源：http://www.blog.yfazqb.com/Article/details/gugcmaucz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.bbcook.cn/Article/details/gxlybdcpb.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.bbcook.cn/Article/details/gsfrpettr.sHtML

npm i -D vite;  npx vite
来源：http://www.share.sjlbkw.cn/Article/details/gvnoaqdzg.sHtML

[U119] JS：生产构建
来源：http://mobile.sjlbkw.cn/Article/details/gcbqeyiuq.sHtML

npx vite build
来源：http://baike.epnwcf.com/Article/details/gsujzzmpm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.vehdjk.com/Article/details/gshivmnjf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.yfazqb.com/Article/details/gelbpwnwz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gebhbjziq.sHtML

统计汇总
来源：http://3g.sjlbkw.cn/Article/details/gcjlznjmy.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/grkojhiym.sHtML

按语言统计（条）：
来源：http://www.share.sjlbkw.cn/Article/details/gniiewaob.sHtML

Python ......... 252
来源：http://m.share.fktsv.cn/Article/details/gzebpmxwt.sHtML

PHP ............ 252
来源：http://m.share.sjlbkw.cn/Article/details/gmrpjddlw.sHtML

JavaScript ..... 252
来源：http://www.blog.epnwcf.com/Article/details/gbsjwrkdw.sHtML

TypeScript ..... 212
来源：http://www.m.share.epnwcf.com/Article/details/gpkbegcnm.sHtML

Java ........... 212
来源：http://www.share.bbcook.cn/Article/details/gckmwbysj.sHtML

Go ............. 212
来源：http://read.share.vehdjk.com/Article/details/gkwjrslcl.sHtML

Ruby ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gahsrabzp.sHtML

C# ............. 212
来源：http://m.share.tarul.cn/Article/details/gtlwjtojb.sHtML

C .............. 30
来源：http://wap.epnwcf.com/Article/details/gwqdcscwg.sHtML

C++ ............ 30
来源：http://mobile.vehdjk.com/Article/details/gjpfzkmmb.sHtML

SQL ............ 90
来源：http://www.share.bbcook.cn/Article/details/gybtfdmzh.sHtML

Bash ........... 80
来源：http://read.share.vehdjk.com/Article/details/gpxwzazez.sHtML

Kotlin ......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gntwhzcrl.sHtML

Swift .......... 15
来源：http://m.share.sjlbkw.cn/Article/details/gtwwvhkxr.sHtML

Lua ............ 10
来源：http://blog.sjlbkw.cn/Article/details/gfpqtdvpf.sHtML

Perl ........... 10
来源：http://wap.epnwcf.com/Article/details/ghreddutj.sHtML

Scala .......... 10
来源：http://www.m.share.tarul.cn/Article/details/gkioqymxd.sHtML

------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gsjbgyseo.sHtML

合计 ........... 2106 条
来源：http://wap.yfazqb.com/Article/details/glcscgfaf.sHtML

按章节统计：
来源：http://m.share.epnwcf.com/Article/details/gncrtstjx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.tarul.cn/Article/details/gasyyavil.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gkeyizquz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gptjxqhkn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.epnwcf.com/Article/details/gvvinichr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fktsv.cn/Article/details/gdhdzfupp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.sjlbkw.cn/Article/details/gjgxixrby.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/gkufoucyu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.bbcook.cn/Article/details/gtnutoiwr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/ggyzipgnt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gbltzglpm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/ggzkbzjpr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gigtoetzl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gjjqzdyyd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.yfazqb.com/Article/details/gyrknjzyr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fktsv.cn/Article/details/girpsfzmd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gwybevcfc.sHtML

Q SQL 专题                              90
来源：http://m.share.tarul.cn/Article/details/ggxjullew.sHtML

R Bash 专题                             80
来源：http://wap.yfazqb.com/Article/details/gitspwpel.sHtML

S C / C++ 专题                          60
来源：http://read.share.sjlbkw.cn/Article/details/gmpnkbfdy.sHtML

T 其他语言补充                          60
来源：http://blog.yfazqb.com/Article/details/gpnrkaqgc.sHtML

U 高频实用片段                         120
来源：http://blog.vehdjk.com/Article/details/gzwfsppgc.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gbupzpvnp.sHtML

合计                                  2106 条
来源：http://baike.sjlbkw.cn/Article/details/gnaptygtv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gfjrvwbif.sHtML


<!-- 参考信息 -->