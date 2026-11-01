代发 wailian999

[U01] Py：创建虚拟环境
来源：http://mobile.fktsv.cn/Article/details/gaznpvpgv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/gffqulvqg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.tarul.cn/Article/details/gpyvoimqa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.tarul.cn/Article/details/gvelrqqhg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.epnwcf.com/Article/details/ghszjblwz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fktsv.cn/Article/details/gqnahwabx.sHtML

[U04] Py：变量调试打印
来源：http://wap.tarul.cn/Article/details/gcmqihnkw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.tarul.cn/Article/details/grkughnem.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.yfazqb.com/Article/details/gpvelripl.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/ggnpetvnq.sHtML

[U06] Py：合并两个字典
来源：http://wap.bbcook.cn/Article/details/gmlfxydsi.sHtML

{**a, **b}
来源：http://mobile.vehdjk.com/Article/details/grktjzdar.sHtML

[U07] Py：反转字典键值
来源：http://mobile.tarul.cn/Article/details/giaolypev.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.yfazqb.com/Article/details/gtozclmuh.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fktsv.cn/Article/details/gpobtgefi.sHtML

[y for x in nested for y in x]
来源：http://read.share.yfazqb.com/Article/details/gdilkgsfu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.vehdjk.com/Article/details/gqrcgdjte.sHtML

max(d, key=d.get)
来源：http://wap.sjlbkw.cn/Article/details/gyfnghbna.sHtML

[U10] Py：按值排序字典
来源：http://wap.fktsv.cn/Article/details/gcgkltlmg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.bbcook.cn/Article/details/gkkrkvgzu.sHtML

[U11] Py：生成器表达式
来源：http://mobile.bbcook.cn/Article/details/gyqqfpoew.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.yfazqb.com/Article/details/gzbtzfipd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.yfazqb.com/Article/details/gccqcsddu.sHtML

Counter(arr).most_common(3)
来源：http://mobile.yfazqb.com/Article/details/gyxzckwav.sHtML

[U13] Py：固定长度队列
来源：http://baike.epnwcf.com/Article/details/gqrvbfnhx.sHtML

deque(maxlen=10)
来源：http://blog.vehdjk.com/Article/details/gbctxztvc.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.bbcook.cn/Article/details/ggcuytxlt.sHtML

defaultdict(list)
来源：http://m.share.tarul.cn/Article/details/gbxqypmwx.sHtML

[U15] Py：高精度计时
来源：http://wap.vehdjk.com/Article/details/gafngyjxu.sHtML

t = time.perf_counter()
来源：http://3g.tarul.cn/Article/details/gmhcbfbca.sHtML

[U16] Py：命令行参数解析
来源：http://baike.vehdjk.com/Article/details/gojloigey.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.bbcook.cn/Article/details/ghoysphlj.sHtML

[U17] Py：初始化日志
来源：http://m.share.fktsv.cn/Article/details/gyhxbnnbt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.tarul.cn/Article/details/gsmimbufp.sHtML

[U18] Py：预编译正则
来源：http://m.share.sjlbkw.cn/Article/details/gsdfqezei.sHtML

pat = re.compile(r"\d+")
来源：http://blog.yfazqb.com/Article/details/gmajjbzes.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.bbcook.cn/Article/details/glxxelowi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.epnwcf.com/Article/details/gsltddmku.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.vehdjk.com/Article/details/gsahqrwqg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.tarul.cn/Article/details/gzemxjufw.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.tarul.cn/Article/details/grsayaszn.sHtML

@contextlib.contextmanager
来源：http://www.share.vehdjk.com/Article/details/gpicyhdse.sHtML

[U22] Py：矩阵转置
来源：http://3g.tarul.cn/Article/details/gaivstude.sHtML

list(zip(*m))
来源：http://read.share.bbcook.cn/Article/details/gsvlirara.sHtML

[U23] Py：分块读取大文件
来源：http://3g.bbcook.cn/Article/details/gvbztqrpu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.epnwcf.com/Article/details/gmltywqjl.sHtML

[U24] Py：路径操作
来源：http://www.blog.tarul.cn/Article/details/ghnwtuhub.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/gkjtigejo.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.epnwcf.com/Article/details/gcwrhvhez.sHtML

csv.DictReader(f)
来源：http://3g.yfazqb.com/Article/details/gcxjkycqp.sHtML

[U26] Py：并发下载
来源：http://read.share.sjlbkw.cn/Article/details/glhtbqwpy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.tarul.cn/Article/details/gvrooakob.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.epnwcf.com/Article/details/gqrojaoul.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.sjlbkw.cn/Article/details/gsreimflz.sHtML

[U28] Py：类型别名
来源：http://blog.epnwcf.com/Article/details/gkdxbcwtq.sHtML

UserId = int
来源：http://www.share.epnwcf.com/Article/details/gromyyotx.sHtML

[U29] Py：属性校验
来源：http://www.share.sjlbkw.cn/Article/details/ghyhggdji.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.vehdjk.com/Article/details/gfnfsjvhr.sHtML

[U30] Py：数据类
来源：http://3g.epnwcf.com/Article/details/ggaqlkclq.sHtML

@dataclass(slots=True)
来源：http://blog.vehdjk.com/Article/details/gwyljkobh.sHtML

[U31] Py：单测
来源：http://www.blog.sjlbkw.cn/Article/details/gnovjyrxv.sHtML

python -m pytest -q
来源：http://m.share.vehdjk.com/Article/details/gxivygnzu.sHtML

[U32] Py：代码格式化
来源：http://mobile.tarul.cn/Article/details/gtzwsfycx.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fktsv.cn/Article/details/gwobkavad.sHtML

[U33] Py：打包发布
来源：http://blog.fktsv.cn/Article/details/gjdlzfkqd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.epnwcf.com/Article/details/gajisscmr.sHtML

[U34] Py：判断编码
来源：http://read.share.fktsv.cn/Article/details/gvltmfjqm.sHtML

chardet.detect(raw)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvodtjejz.sHtML

[U35] Py：发送邮件
来源：http://wap.vehdjk.com/Article/details/gelccvbgp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.vehdjk.com/Article/details/gjyitsejk.sHtML

[U36] Py：定时任务
来源：http://mobile.bbcook.cn/Article/details/gdnvplord.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.vehdjk.com/Article/details/gmgyvqawc.sHtML

[U37] Py：读写 Excel
来源：http://wap.yfazqb.com/Article/details/gzgsvgdlj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.bbcook.cn/Article/details/gborrenfu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fktsv.cn/Article/details/gaeugruga.sHtML

Path(__file__).resolve().parent
来源：http://baike.fktsv.cn/Article/details/gejtljjcw.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.epnwcf.com/Article/details/gzhdvroiz.sHtML

sys.stdout.isatty()
来源：http://www.m.share.vehdjk.com/Article/details/gscmmnsvm.sHtML

[U40] Py：打印到标准错误
来源：http://3g.epnwcf.com/Article/details/gstcahtqu.sHtML

print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/gnfvmsttg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.vehdjk.com/Article/details/ggtlydkle.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.bbcook.cn/Article/details/gkyjgwfwt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.bbcook.cn/Article/details/gpwwkuojz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.epnwcf.com/Article/details/ggfknknle.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.epnwcf.com/Article/details/gtrjfdczs.sHtML

namespace App\Http;
来源：http://mobile.sjlbkw.cn/Article/details/ggkwzxfnj.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.vehdjk.com/Article/details/gexjffotz.sHtML

declare(strict_types=1);
来源：http://www.blog.sjlbkw.cn/Article/details/gxsyvvngn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.epnwcf.com/Article/details/gcdurxftj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gskokaokp.sHtML

[U46] PHP：可空类型
来源：http://m.share.tarul.cn/Article/details/gahptfjyr.sHtML

?string $name = null
来源：http://baike.tarul.cn/Article/details/gufdysyrs.sHtML

[U47] PHP：联合类型
来源：http://www.blog.bbcook.cn/Article/details/gchjzegvj.sHtML

int|string $id
来源：http://wap.tarul.cn/Article/details/gunsfgfin.sHtML

[U48] PHP：纯枚举
来源：http://3g.bbcook.cn/Article/details/gwdgheqct.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.epnwcf.com/Article/details/gwjfwnbei.sHtML

[U49] PHP：只读属性
来源：http://mobile.tarul.cn/Article/details/gfhrndvjx.sHtML

public readonly string $name
来源：http://read.share.epnwcf.com/Article/details/gdqgxsnco.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.bbcook.cn/Article/details/gjolmwpiq.sHtML

public function __construct(private int $id) {}
来源：http://3g.bbcook.cn/Article/details/grypsevxw.sHtML

[U51] PHP：数组解构
来源：http://m.share.bbcook.cn/Article/details/gnchfvmwy.sHtML

[$a, $b] = $arr;
来源：http://mobile.tarul.cn/Article/details/gnemyszzs.sHtML

[U52] PHP：箭头函数
来源：http://www.share.vehdjk.com/Article/details/ghbphydqf.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.vehdjk.com/Article/details/gdbqkpjmm.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.sjlbkw.cn/Article/details/gfyjnjdfe.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.vehdjk.com/Article/details/geblhabdj.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.bbcook.cn/Article/details/gacrajnrm.sHtML

$obj?->method()
来源：http://m.share.fktsv.cn/Article/details/gihhaqfen.sHtML

[U55] PHP：match 表达式
来源：http://blog.vehdjk.com/Article/details/gjxiwknzy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fktsv.cn/Article/details/gwezjbinu.sHtML

[U56] PHP：命名参数
来源：http://www.blog.tarul.cn/Article/details/gfcbazokg.sHtML

f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gmmylnukv.sHtML

[U57] PHP：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gekjjjwoo.sHtML

"值: {$a}"
来源：http://blog.epnwcf.com/Article/details/gsfutyahf.sHtML

[U58] PHP：数组三件套
来源：http://baike.sjlbkw.cn/Article/details/gfdqxuale.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.sjlbkw.cn/Article/details/gmsmuwoqz.sHtML

[U59] PHP：自定义排序
来源：http://mobile.sjlbkw.cn/Article/details/gdmtuxsyq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/gcqthrkpe.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.yfazqb.com/Article/details/gofqgvqer.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.epnwcf.com/Article/details/gxilyuypd.sHtML

[U61] PHP：正则
来源：http://mobile.fktsv.cn/Article/details/gofrcaees.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/gyccimsby.sHtML

[U62] PHP：日期对象
来源：http://wap.fktsv.cn/Article/details/gsuwdwjfx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.vehdjk.com/Article/details/gcijfdxcj.sHtML

[U63] PHP：文件读写
来源：http://blog.sjlbkw.cn/Article/details/gkljelgfn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.sjlbkw.cn/Article/details/gvccxulbz.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fktsv.cn/Article/details/gcptdqtaf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.sjlbkw.cn/Article/details/gvqhflfgd.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/gcurkjtqp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gyizhvzxb.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.sjlbkw.cn/Article/details/gaotudxur.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.epnwcf.com/Article/details/gsrxsyanf.sHtML

[U67] PHP：处理文件上传
来源：http://baike.tarul.cn/Article/details/gbqmcvdfu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.yfazqb.com/Article/details/gfwdrlsvz.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.epnwcf.com/Article/details/ghtfunkmw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.sjlbkw.cn/Article/details/gfewltygn.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.yfazqb.com/Article/details/gwlnohekw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.tarul.cn/Article/details/goufnoslv.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.yfazqb.com/Article/details/gzqmckett.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.tarul.cn/Article/details/gyqbmrmaw.sHtML

[U71] PHP：抛出异常
来源：http://m.share.bbcook.cn/Article/details/ghyttovts.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.vehdjk.com/Article/details/gyzokmjbj.sHtML

[U72] PHP：写错误日志
来源：http://wap.sjlbkw.cn/Article/details/ghsgcgjji.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.epnwcf.com/Article/details/gxhwpnvvn.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.bbcook.cn/Article/details/gpyhscjiv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.yfazqb.com/Article/details/gopqkuouq.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.tarul.cn/Article/details/gcwufzzpa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fktsv.cn/Article/details/gozqstitf.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fktsv.cn/Article/details/gwwdntrnx.sHtML

composer require psr/container
来源：http://baike.bbcook.cn/Article/details/ggerchezh.sHtML

[U76] PHP：简单路由
来源：http://m.share.vehdjk.com/Article/details/giumfqqqw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.vehdjk.com/Article/details/gcwhxskyw.sHtML

[U77] PHP：模板渲染
来源：http://3g.vehdjk.com/Article/details/grpjnetzq.sHtML

composer require twig/twig
来源：http://blog.yfazqb.com/Article/details/gdqvrlbpw.sHtML

[U78] PHP：单元测试
来源：http://3g.bbcook.cn/Article/details/gscswxeip.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.tarul.cn/Article/details/gwgrkillg.sHtML

[U79] PHP：静态分析
来源：http://3g.epnwcf.com/Article/details/gsqujhghe.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fktsv.cn/Article/details/gjxhskoau.sHtML

[U80] PHP：代码规范修复
来源：http://3g.bbcook.cn/Article/details/gsrsdlvdc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.epnwcf.com/Article/details/gtmqhjhog.sHtML

[U81] JS：初始化项目
来源：http://www.share.tarul.cn/Article/details/gjiqnbvvx.sHtML

npm init -y;  npm i express
来源：http://mobile.sjlbkw.cn/Article/details/gjopwfwqt.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.sjlbkw.cn/Article/details/gziqmnasp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.tarul.cn/Article/details/gmiypywjv.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.epnwcf.com/Article/details/ghfvboruh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.yfazqb.com/Article/details/gpyjxbkqn.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.bbcook.cn/Article/details/gffttqett.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.yfazqb.com/Article/details/gpjxsjjyk.sHtML

[U85] JS：可选链
来源：http://read.share.tarul.cn/Article/details/gnvvjgvoi.sHtML

a?.b?.c
来源：http://www.share.sjlbkw.cn/Article/details/gbozspplo.sHtML

[U86] JS：空值合并
来源：http://m.share.tarul.cn/Article/details/gumioatgx.sHtML

a ?? b
来源：http://mobile.epnwcf.com/Article/details/gmvpxntip.sHtML

[U87] JS：解构默认值
来源：http://m.share.tarul.cn/Article/details/gklpykiul.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.bbcook.cn/Article/details/gecatqvye.sHtML

[U88] JS：对象展开合并
来源：http://baike.yfazqb.com/Article/details/gjwgqvtzu.sHtML

{ ...a, ...b }
来源：http://blog.bbcook.cn/Article/details/gomxmjttg.sHtML

[U89] JS：数组去重
来源：http://www.blog.vehdjk.com/Article/details/groxwuizv.sHtML

[...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gstnhqnxb.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.yfazqb.com/Article/details/glclliytp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gumkssduj.sHtML

[U91] JS：对象键值遍历
来源：http://blog.tarul.cn/Article/details/gatbbmjxb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fktsv.cn/Article/details/goehhebnw.sHtML

[U92] JS：深拷贝
来源：http://wap.tarul.cn/Article/details/gxqoblqfy.sHtML

structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/galskemih.sHtML

[U93] JS：模板字符串
来源：http://baike.fktsv.cn/Article/details/gyjvwbeqp.sHtML

`共 ${n} 条`
来源：http://www.m.share.sjlbkw.cn/Article/details/grcpljlxr.sHtML

[U94] JS：箭头函数
来源：http://blog.yfazqb.com/Article/details/gqgadstif.sHtML

const double = x => x * 2;
来源：http://wap.bbcook.cn/Article/details/gmvzcnvgx.sHtML

[U95] JS：Promise 包装
来源：http://baike.tarul.cn/Article/details/gmpgwkvve.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.sjlbkw.cn/Article/details/gmejzgjex.sHtML

[U96] JS：async/await 与异常
来源：http://wap.epnwcf.com/Article/details/gfbprdpbd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gmgdzjruh.sHtML

[U97] JS：并发请求
来源：http://read.share.fktsv.cn/Article/details/grdqenltu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/glhryhhwc.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.yfazqb.com/Article/details/gdncwbogg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.vehdjk.com/Article/details/gnalrphku.sHtML

[U99] JS：事件监听
来源：http://read.share.fktsv.cn/Article/details/grfzrkcua.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fktsv.cn/Article/details/ggsoqwalv.sHtML

[U100] JS：DOM 查询
来源：http://wap.fktsv.cn/Article/details/giawmgmjf.sHtML

document.querySelector(".item")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvttonqzh.sHtML

[U101] JS：classList 操作
来源：http://www.share.yfazqb.com/Article/details/gyirgkgxf.sHtML

el.classList.toggle("active")
来源：http://3g.tarul.cn/Article/details/gujedyjhv.sHtML

[U102] JS：本地存储
来源：http://m.share.fktsv.cn/Article/details/gzjjxnync.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.sjlbkw.cn/Article/details/gahuykhkg.sHtML

[U103] JS：定时器
来源：http://baike.yfazqb.com/Article/details/gqozwwozb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.bbcook.cn/Article/details/goeqgtggt.sHtML

[U104] JS：防抖
来源：http://www.m.share.fktsv.cn/Article/details/getikjrna.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/gxvvxgtgw.sHtML

[U105] JS：节流
来源：http://www.m.share.vehdjk.com/Article/details/gmszqsayi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.sjlbkw.cn/Article/details/gvjmxoqhg.sHtML

[U106] JS：日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gctuzjsmp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.bbcook.cn/Article/details/gghrcwtcn.sHtML

[U107] JS：数字千分位
来源：http://baike.tarul.cn/Article/details/gqbjznvye.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.yfazqb.com/Article/details/gkrnzozdg.sHtML

[U108] JS：随机整数
来源：http://www.m.share.bbcook.cn/Article/details/grbzprsxd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.yfazqb.com/Article/details/gcsdlbkji.sHtML

[U109] JS：数组分组
来源：http://www.blog.yfazqb.com/Article/details/grcscjito.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gzikpfhin.sHtML

[U110] JS：数组分块
来源：http://baike.tarul.cn/Article/details/glklpvmcl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.epnwcf.com/Article/details/guvohhhlw.sHtML

[U111] JS：对象转 Map
来源：http://baike.yfazqb.com/Article/details/gmyajhmkw.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fktsv.cn/Article/details/gfeoioaes.sHtML

[U112] JS：字符串补位
来源：http://m.share.tarul.cn/Article/details/ggryztvoy.sHtML

"7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gdfrccula.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.bbcook.cn/Article/details/gwruoojaz.sHtML

s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gemsfpnjg.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.bbcook.cn/Article/details/gchsbgncc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.tarul.cn/Article/details/gdkzawxbn.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/ghwitbvdd.sHtML

crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gdliwggvx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.vehdjk.com/Article/details/guihmrudc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.tarul.cn/Article/details/govzmqhxt.sHtML

[U117] JS：单元测试
来源：http://wap.bbcook.cn/Article/details/gvywyrdvj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.vehdjk.com/Article/details/gvzezyzka.sHtML

[U118] JS：开发服务器
来源：http://3g.tarul.cn/Article/details/gawklfejn.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.bbcook.cn/Article/details/ginsivyoa.sHtML

[U119] JS：生产构建
来源：http://read.share.epnwcf.com/Article/details/gtpyrrhiz.sHtML

npx vite build
来源：http://www.blog.tarul.cn/Article/details/gdxnisepm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.sjlbkw.cn/Article/details/gbsccyvkz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.tarul.cn/Article/details/goixqzqnp.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ggjuadytz.sHtML

统计汇总
来源：http://read.share.tarul.cn/Article/details/gsmzmyrze.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzsbfjimx.sHtML

按语言统计（条）：
来源：http://www.share.vehdjk.com/Article/details/gcurgxiem.sHtML

Python ......... 252
来源：http://3g.bbcook.cn/Article/details/gaicsqwmp.sHtML

PHP ............ 252
来源：http://www.m.share.vehdjk.com/Article/details/ghgjabiax.sHtML

JavaScript ..... 252
来源：http://www.m.share.tarul.cn/Article/details/gekfbjawe.sHtML

TypeScript ..... 212
来源：http://www.blog.fktsv.cn/Article/details/gbfosfjwb.sHtML

Java ........... 212
来源：http://www.blog.tarul.cn/Article/details/gawuimnya.sHtML

Go ............. 212
来源：http://blog.tarul.cn/Article/details/gfrkvfyew.sHtML

Ruby ........... 212
来源：http://blog.fktsv.cn/Article/details/gmntchibz.sHtML

C# ............. 212
来源：http://blog.vehdjk.com/Article/details/gicchvgrr.sHtML

C .............. 30
来源：http://blog.tarul.cn/Article/details/ggyvmknwr.sHtML

C++ ............ 30
来源：http://www.blog.epnwcf.com/Article/details/gvhfuthtf.sHtML

SQL ............ 90
来源：http://read.share.bbcook.cn/Article/details/ghhyrifrd.sHtML

Bash ........... 80
来源：http://www.share.vehdjk.com/Article/details/gsdgeusww.sHtML

Kotlin ......... 15
来源：http://3g.vehdjk.com/Article/details/gupxaeqac.sHtML

Swift .......... 15
来源：http://www.blog.yfazqb.com/Article/details/glmteoysx.sHtML

Lua ............ 10
来源：http://3g.vehdjk.com/Article/details/gbpuopdsp.sHtML

Perl ........... 10
来源：http://blog.sjlbkw.cn/Article/details/gklaclovl.sHtML

Scala .......... 10
来源：http://mobile.epnwcf.com/Article/details/ghjvvpnta.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gaxewluzr.sHtML

合计 ........... 2106 条
来源：http://www.blog.sjlbkw.cn/Article/details/gjzrskurj.sHtML

按章节统计：
来源：http://read.share.vehdjk.com/Article/details/gjzbdyqmu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/guotkckxc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gfdvfczds.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/gfnmtkiwo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fktsv.cn/Article/details/gpyzvpctp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.vehdjk.com/Article/details/gqbchgthb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.yfazqb.com/Article/details/ggxcggfqs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gfymrqukd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/ganlhwduo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gotmdbgqb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.sjlbkw.cn/Article/details/giyloxnyh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/glbaxznge.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gtswplaxb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gteommnla.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.yfazqb.com/Article/details/gqzzdnkbf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.sjlbkw.cn/Article/details/gwmtamscp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/goroilszv.sHtML

Q SQL 专题                              90
来源：http://www.blog.bbcook.cn/Article/details/gekqshhvq.sHtML

R Bash 专题                             80
来源：http://www.m.share.sjlbkw.cn/Article/details/gspvtflbs.sHtML

S C / C++ 专题                          60
来源：http://mobile.epnwcf.com/Article/details/gryecvckc.sHtML

T 其他语言补充                          60
来源：http://mobile.yfazqb.com/Article/details/gmhwsyctu.sHtML

U 高频实用片段                         120
来源：http://www.blog.bbcook.cn/Article/details/gkkkwrdbu.sHtML

------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/godsjzain.sHtML

合计                                  2106 条
来源：http://m.share.vehdjk.com/Article/details/gtvlyseil.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gyxjrevar.sHtML

使用提醒
来源：http://www.share.tarul.cn/Article/details/ghmsdgash.sHtML

--------------------------------------------------------------------------------
来源：http://wap.vehdjk.com/Article/details/gkzbkqzbn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.yfazqb.com/Article/details/gubylgyrd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.sjlbkw.cn/Article/details/gqhgmpznd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.sjlbkw.cn/Article/details/grnbpwzqy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.sjlbkw.cn/Article/details/gdoxevhod.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.yfazqb.com/Article/details/ghuiqivor.sHtML

—— 文件结束 ——
来源：http://3g.yfazqb.com/Article/details/gdsqzpprj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gpqfhowak.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.vehdjk.com/Article/details/gglbqcbbg.sHtML

Common Programming Examples Cheat Book
来源：http://baike.yfazqb.com/Article/details/glgwfszsp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/govubowcr.sHtML


<!-- 参考信息 -->