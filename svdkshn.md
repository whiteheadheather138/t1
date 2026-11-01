代发 wailian999

val a = 1;  var b = 2
来源：http://read.share.yfazqb.com/Article/details/gvvpesxuv.sHtML

[T53] Scala：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gujxouvqz.sHtML

s"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gmdyjobsc.sHtML

[T54] Scala：集合映射
来源：http://m.share.vehdjk.com/Article/details/gzvongyyj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.sjlbkw.cn/Article/details/gxfkompng.sHtML

[T55] Scala：集合过滤
来源：http://baike.yfazqb.com/Article/details/gioazxcbj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.vehdjk.com/Article/details/gsnosiojw.sHtML

[T56] Scala：样例类
来源：http://blog.yfazqb.com/Article/details/gqgawrfis.sHtML

case class User(name: String, age: Int)
来源：http://m.share.bbcook.cn/Article/details/gydrjvqfy.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gaayktgkk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.yfazqb.com/Article/details/gxtbnizkd.sHtML

[T58] Scala：函数定义
来源：http://3g.bbcook.cn/Article/details/grizhadah.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.epnwcf.com/Article/details/gcttmhsjn.sHtML

[T59] Scala：循环
来源：http://www.blog.epnwcf.com/Article/details/gvudgrsaa.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gkdqepyyu.sHtML

[T60] Scala：折叠
来源：http://baike.fktsv.cn/Article/details/gwfivisus.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fktsv.cn/Article/details/gkvytmkji.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gupgssdpt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.bbcook.cn/Article/details/gkdtznfds.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzheopgdh.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.yfazqb.com/Article/details/gyoarxmjb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/gkyhturvy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.tarul.cn/Article/details/guidddehf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fktsv.cn/Article/details/gztqbdrax.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.yfazqb.com/Article/details/gbpjgywou.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.yfazqb.com/Article/details/gdfpqbsql.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.tarul.cn/Article/details/gbwmpfyny.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.bbcook.cn/Article/details/gfukxpnxp.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fktsv.cn/Article/details/ghefixvju.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/ggrjvezwn.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fktsv.cn/Article/details/gcydrtdmi.sHtML

{**a, **b}
来源：http://wap.yfazqb.com/Article/details/gmgirrmwa.sHtML

[U07] Py：反转字典键值
来源：http://mobile.sjlbkw.cn/Article/details/gcnpnonwj.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.epnwcf.com/Article/details/gdrpwkiue.sHtML

[U08] Py：展平二维列表
来源：http://www.share.bbcook.cn/Article/details/glcxjuxgm.sHtML

[y for x in nested for y in x]
来源：http://www.share.epnwcf.com/Article/details/gkxxnxluj.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.tarul.cn/Article/details/gstdqlutq.sHtML

max(d, key=d.get)
来源：http://baike.bbcook.cn/Article/details/gvjxjonuc.sHtML

[U10] Py：按值排序字典
来源：http://wap.bbcook.cn/Article/details/gmgtrvuzw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.tarul.cn/Article/details/gbtpsmpda.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.vehdjk.com/Article/details/gjhybpfao.sHtML

(x * 2 for x in arr)
来源：http://blog.yfazqb.com/Article/details/gnvuzvjwa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.sjlbkw.cn/Article/details/gxchnwdkx.sHtML

Counter(arr).most_common(3)
来源：http://www.share.epnwcf.com/Article/details/gupftbbji.sHtML

[U13] Py：固定长度队列
来源：http://m.share.yfazqb.com/Article/details/gtpwwwtta.sHtML

deque(maxlen=10)
来源：http://read.share.bbcook.cn/Article/details/gmekzfndz.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfpwysfn.sHtML

defaultdict(list)
来源：http://www.share.epnwcf.com/Article/details/grbdecrzo.sHtML

[U15] Py：高精度计时
来源：http://wap.yfazqb.com/Article/details/ggspsjilp.sHtML

t = time.perf_counter()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdptgfkue.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.yfazqb.com/Article/details/gwumjtkmh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.yfazqb.com/Article/details/gyfzfybgl.sHtML

[U17] Py：初始化日志
来源：http://baike.vehdjk.com/Article/details/gsvlzyvfj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.epnwcf.com/Article/details/gjnawsrki.sHtML

[U18] Py：预编译正则
来源：http://wap.tarul.cn/Article/details/gpatbkdgb.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fktsv.cn/Article/details/gudlztcte.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.sjlbkw.cn/Article/details/gjihsvnbz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.vehdjk.com/Article/details/gkepqesip.sHtML

[U20] Py：缓存函数结果
来源：http://wap.vehdjk.com/Article/details/gejyqlaub.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.epnwcf.com/Article/details/gpwttpipr.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.epnwcf.com/Article/details/gewoeopuc.sHtML

@contextlib.contextmanager
来源：http://mobile.yfazqb.com/Article/details/gqmbfvkwg.sHtML

[U22] Py：矩阵转置
来源：http://wap.fktsv.cn/Article/details/gycnlbcgs.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/giezgnotr.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gknzvtwwl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.sjlbkw.cn/Article/details/glesbstmz.sHtML

[U24] Py：路径操作
来源：http://wap.vehdjk.com/Article/details/gsznpkzbx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/gywnxlcqh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.vehdjk.com/Article/details/gjybrtcxh.sHtML

csv.DictReader(f)
来源：http://read.share.tarul.cn/Article/details/gagptrvhe.sHtML

[U26] Py：并发下载
来源：http://baike.vehdjk.com/Article/details/gurkwsqzj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.tarul.cn/Article/details/guwijqpmd.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fktsv.cn/Article/details/gcsnzoytl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.vehdjk.com/Article/details/gpkookecz.sHtML

[U28] Py：类型别名
来源：http://www.blog.tarul.cn/Article/details/gchwpnlzt.sHtML

UserId = int
来源：http://mobile.vehdjk.com/Article/details/gxxuhexbd.sHtML

[U29] Py：属性校验
来源：http://www.share.tarul.cn/Article/details/ghrvxsttt.sHtML

@property 与 @x.setter 配合
来源：http://blog.bbcook.cn/Article/details/glmiakmyt.sHtML

[U30] Py：数据类
来源：http://m.share.bbcook.cn/Article/details/gapyxzurz.sHtML

@dataclass(slots=True)
来源：http://3g.yfazqb.com/Article/details/gctgyfqcq.sHtML

[U31] Py：单测
来源：http://mobile.vehdjk.com/Article/details/gzinukead.sHtML

python -m pytest -q
来源：http://read.share.tarul.cn/Article/details/gqlynynmx.sHtML

[U32] Py：代码格式化
来源：http://www.blog.yfazqb.com/Article/details/gnpaaytda.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.sjlbkw.cn/Article/details/gfchjiixv.sHtML

[U33] Py：打包发布
来源：http://baike.bbcook.cn/Article/details/gagwseeoh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.vehdjk.com/Article/details/gaozlkoiy.sHtML

[U34] Py：判断编码
来源：http://wap.fktsv.cn/Article/details/gijsnjyom.sHtML

chardet.detect(raw)
来源：http://wap.epnwcf.com/Article/details/ghpxnwcdd.sHtML

[U35] Py：发送邮件
来源：http://m.share.tarul.cn/Article/details/gmkkpnndb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.sjlbkw.cn/Article/details/gwdomotxh.sHtML

[U36] Py：定时任务
来源：http://www.share.epnwcf.com/Article/details/gvtcftyvx.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.epnwcf.com/Article/details/giebgjdyj.sHtML

[U37] Py：读写 Excel
来源：http://3g.vehdjk.com/Article/details/gedlfczcg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.bbcook.cn/Article/details/gczwnsisg.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.tarul.cn/Article/details/gpokqazey.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.tarul.cn/Article/details/gopmjemee.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.sjlbkw.cn/Article/details/gjxcvkprv.sHtML

sys.stdout.isatty()
来源：http://baike.bbcook.cn/Article/details/gnvfirvbe.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fktsv.cn/Article/details/gnkwvgsro.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/ggkntmklu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.sjlbkw.cn/Article/details/ggcjwucoj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.epnwcf.com/Article/details/gptuyvhyv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.yfazqb.com/Article/details/gtomxnkoq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.bbcook.cn/Article/details/gnmjgwuhb.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fktsv.cn/Article/details/gzvdkbgxy.sHtML

namespace App\Http;
来源：http://wap.tarul.cn/Article/details/gagbhrilc.sHtML

[U44] PHP：开启严格类型
来源：http://wap.epnwcf.com/Article/details/gacdauvoy.sHtML

declare(strict_types=1);
来源：http://www.m.share.epnwcf.com/Article/details/gjnwqsljt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.vehdjk.com/Article/details/ggvghnvxu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gnevalfph.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.vehdjk.com/Article/details/gctttzznb.sHtML

?string $name = null
来源：http://www.blog.epnwcf.com/Article/details/gqwvshgpc.sHtML

[U47] PHP：联合类型
来源：http://wap.sjlbkw.cn/Article/details/ginyvmajx.sHtML

int|string $id
来源：http://read.share.epnwcf.com/Article/details/gvewiiwqj.sHtML

[U48] PHP：纯枚举
来源：http://read.share.vehdjk.com/Article/details/gbafdfzpz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.tarul.cn/Article/details/gfstivggd.sHtML

[U49] PHP：只读属性
来源：http://wap.sjlbkw.cn/Article/details/gzagupeje.sHtML

public readonly string $name
来源：http://mobile.yfazqb.com/Article/details/gmhcagngs.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.vehdjk.com/Article/details/glkrsnavu.sHtML

public function __construct(private int $id) {}
来源：http://m.share.bbcook.cn/Article/details/guyeeingd.sHtML

[U51] PHP：数组解构
来源：http://www.blog.epnwcf.com/Article/details/gyuklcpue.sHtML

[$a, $b] = $arr;
来源：http://read.share.yfazqb.com/Article/details/gxghegqrj.sHtML

[U52] PHP：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gaahrmymf.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.tarul.cn/Article/details/gnfrmbylj.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fktsv.cn/Article/details/gwnhwsjkk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.bbcook.cn/Article/details/gahltewll.sHtML

[U54] PHP：空安全调用
来源：http://www.share.tarul.cn/Article/details/getgzvvtj.sHtML

$obj?->method()
来源：http://mobile.bbcook.cn/Article/details/ggbsjvggr.sHtML

[U55] PHP：match 表达式
来源：http://blog.epnwcf.com/Article/details/gnetaqsid.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/gdxhwtdux.sHtML

[U56] PHP：命名参数
来源：http://wap.fktsv.cn/Article/details/gtwwtjjzb.sHtML

f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gipxtible.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gfhqbyklf.sHtML

"值: {$a}"
来源：http://mobile.yfazqb.com/Article/details/gpowlumpu.sHtML

[U58] PHP：数组三件套
来源：http://wap.fktsv.cn/Article/details/gspejevbb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.tarul.cn/Article/details/grikxwuex.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fktsv.cn/Article/details/gsocqxiqo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/gyvmryxuq.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.vehdjk.com/Article/details/gdoltqdwe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.epnwcf.com/Article/details/gyinxooyv.sHtML

[U61] PHP：正则
来源：http://m.share.bbcook.cn/Article/details/glvvhjdgy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fktsv.cn/Article/details/gvdccwazv.sHtML

[U62] PHP：日期对象
来源：http://blog.fktsv.cn/Article/details/gteqefley.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.bbcook.cn/Article/details/gplzqjjfi.sHtML

[U63] PHP：文件读写
来源：http://mobile.sjlbkw.cn/Article/details/gyzprhcix.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.sjlbkw.cn/Article/details/gemclrmyq.sHtML

[U64] PHP：目录遍历
来源：http://wap.vehdjk.com/Article/details/gdbhngijs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fktsv.cn/Article/details/geyoxptmg.sHtML

[U65] PHP：会话
来源：http://blog.bbcook.cn/Article/details/gzwfwpemj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.yfazqb.com/Article/details/gsrfyaxii.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.epnwcf.com/Article/details/gaavybiao.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.bbcook.cn/Article/details/gybouqumv.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.vehdjk.com/Article/details/grwnspluw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.epnwcf.com/Article/details/gmhysfoft.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.vehdjk.com/Article/details/gleaenudy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.tarul.cn/Article/details/ghwoxzvyo.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.tarul.cn/Article/details/gjnzzcqrx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.tarul.cn/Article/details/gkprwqolg.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.epnwcf.com/Article/details/gilosnrfh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.vehdjk.com/Article/details/gfayplffd.sHtML

[U71] PHP：抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gmdmcwzou.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.vehdjk.com/Article/details/gaagempdo.sHtML

[U72] PHP：写错误日志
来源：http://m.share.tarul.cn/Article/details/gvsbcvfcz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.tarul.cn/Article/details/goylzuhws.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.vehdjk.com/Article/details/gjnjcdbmn.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fktsv.cn/Article/details/gkgpootng.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gclwtlwuv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.tarul.cn/Article/details/gafslzptd.sHtML

[U75] PHP：依赖注入
来源：http://blog.vehdjk.com/Article/details/gkdnxeouw.sHtML

composer require psr/container
来源：http://read.share.vehdjk.com/Article/details/gsvvsujjp.sHtML

[U76] PHP：简单路由
来源：http://blog.bbcook.cn/Article/details/gfebdhnym.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.tarul.cn/Article/details/gonqdrzol.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.tarul.cn/Article/details/gsbzukxoc.sHtML

composer require twig/twig
来源：http://www.blog.epnwcf.com/Article/details/gzuoiaklw.sHtML

[U78] PHP：单元测试
来源：http://3g.epnwcf.com/Article/details/gonmzuuyn.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.sjlbkw.cn/Article/details/gwdgkyxll.sHtML

[U79] PHP：静态分析
来源：http://www.share.tarul.cn/Article/details/gpvrstkff.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.tarul.cn/Article/details/gidvqimsa.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fktsv.cn/Article/details/grlsfczhj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.bbcook.cn/Article/details/gddbyiisr.sHtML

[U81] JS：初始化项目
来源：http://www.blog.vehdjk.com/Article/details/gsbbsjurt.sHtML

npm init -y;  npm i express
来源：http://www.m.share.tarul.cn/Article/details/guubbvddn.sHtML

[U82] JS：package.json 脚本
来源：http://wap.epnwcf.com/Article/details/garqajuxv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.yfazqb.com/Article/details/gdbcxulpm.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.epnwcf.com/Article/details/gscnfyffd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/ggxdyuhnu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.yfazqb.com/Article/details/gnmfkoaza.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.tarul.cn/Article/details/gypjagcov.sHtML

[U85] JS：可选链
来源：http://www.blog.vehdjk.com/Article/details/gprtlzaar.sHtML

a?.b?.c
来源：http://3g.vehdjk.com/Article/details/gwpwcmnsv.sHtML

[U86] JS：空值合并
来源：http://read.share.yfazqb.com/Article/details/gsrooegkt.sHtML

a ?? b
来源：http://3g.vehdjk.com/Article/details/gqxdvnhce.sHtML

[U87] JS：解构默认值
来源：http://blog.yfazqb.com/Article/details/gdxcqtjlq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fktsv.cn/Article/details/gpfxabdjq.sHtML

[U88] JS：对象展开合并
来源：http://mobile.vehdjk.com/Article/details/gbfsyoxrx.sHtML

{ ...a, ...b }
来源：http://www.blog.sjlbkw.cn/Article/details/ggbitcndl.sHtML

[U89] JS：数组去重
来源：http://read.share.epnwcf.com/Article/details/geqjhxvro.sHtML

[...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/ggxgxoxll.sHtML

[U90] JS：数字数组排序
来源：http://baike.yfazqb.com/Article/details/gbkuusgmx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/grtbyctar.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.vehdjk.com/Article/details/gdomgjqdf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.sjlbkw.cn/Article/details/gfksiiipd.sHtML

[U92] JS：深拷贝
来源：http://blog.vehdjk.com/Article/details/giqdqvnhx.sHtML

structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gdievzxws.sHtML

[U93] JS：模板字符串
来源：http://baike.epnwcf.com/Article/details/gvezwnzns.sHtML

`共 ${n} 条`
来源：http://3g.epnwcf.com/Article/details/ghnnbdkej.sHtML

[U94] JS：箭头函数
来源：http://www.blog.yfazqb.com/Article/details/gvmqwynjt.sHtML

const double = x => x * 2;
来源：http://m.share.epnwcf.com/Article/details/giirxqfyy.sHtML

[U95] JS：Promise 包装
来源：http://www.share.bbcook.cn/Article/details/guaxkfuhe.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.sjlbkw.cn/Article/details/gldngyfsl.sHtML

[U96] JS：async/await 与异常
来源：http://wap.tarul.cn/Article/details/gxrduskbv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/geacrnplj.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/gjdcezdvv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gdghtlsuj.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.tarul.cn/Article/details/gcghgywsg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.sjlbkw.cn/Article/details/glzoftgkj.sHtML

[U99] JS：事件监听
来源：http://wap.bbcook.cn/Article/details/ghbkoypqc.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.yfazqb.com/Article/details/gudnjxzyi.sHtML

[U100] JS：DOM 查询
来源：http://baike.tarul.cn/Article/details/gtavopwie.sHtML

document.querySelector(".item")
来源：http://read.share.yfazqb.com/Article/details/gggbsrynh.sHtML

[U101] JS：classList 操作
来源：http://www.blog.tarul.cn/Article/details/gtrscqonj.sHtML

el.classList.toggle("active")
来源：http://blog.vehdjk.com/Article/details/ghnqcfizi.sHtML

[U102] JS：本地存储
来源：http://blog.epnwcf.com/Article/details/gekqfwydp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.yfazqb.com/Article/details/gjtiiekmq.sHtML

[U103] JS：定时器
来源：http://baike.vehdjk.com/Article/details/gqayeluel.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.epnwcf.com/Article/details/gggkzuedt.sHtML

[U104] JS：防抖
来源：http://www.m.share.yfazqb.com/Article/details/gaovogkvo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gfapfsres.sHtML

[U105] JS：节流
来源：http://www.m.share.tarul.cn/Article/details/gegoungvu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.epnwcf.com/Article/details/guoweyxzq.sHtML

[U106] JS：日期格式化
来源：http://blog.fktsv.cn/Article/details/gokgjydjp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.bbcook.cn/Article/details/gcygpvawn.sHtML

[U107] JS：数字千分位
来源：http://baike.tarul.cn/Article/details/gbyuabpes.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gywqimcyw.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gwmkztvag.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fktsv.cn/Article/details/gktqrobvn.sHtML

[U109] JS：数组分组
来源：http://baike.fktsv.cn/Article/details/gwtwsivjp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gjacxhqgm.sHtML

[U110] JS：数组分块
来源：http://www.share.yfazqb.com/Article/details/gmbgnlbrt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.bbcook.cn/Article/details/gtvceuebt.sHtML

[U111] JS：对象转 Map
来源：http://read.share.bbcook.cn/Article/details/gprvmjplf.sHtML

new Map(Object.entries(obj))
来源：http://m.share.sjlbkw.cn/Article/details/gapaiirmx.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fktsv.cn/Article/details/gswpyihtj.sHtML

"7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gvjvdwjtr.sHtML

[U113] JS：正则替换全部
来源：http://m.share.bbcook.cn/Article/details/gyzoljftx.sHtML

s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/giktkxdlh.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.yfazqb.com/Article/details/gasssesyp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gaeuywzfh.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gotkokacv.sHtML

crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gzvxpebbu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.epnwcf.com/Article/details/gczrqjnmh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fktsv.cn/Article/details/ggycbafbx.sHtML

[U117] JS：单元测试
来源：http://wap.vehdjk.com/Article/details/gcjyzzrjb.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.tarul.cn/Article/details/gdnshrdfp.sHtML

[U118] JS：开发服务器
来源：http://blog.bbcook.cn/Article/details/gtsabgvyc.sHtML

npm i -D vite;  npx vite
来源：http://mobile.vehdjk.com/Article/details/guqdmugtt.sHtML

[U119] JS：生产构建
来源：http://www.share.bbcook.cn/Article/details/geechcikw.sHtML

npx vite build
来源：http://wap.fktsv.cn/Article/details/gkazvrued.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.epnwcf.com/Article/details/giivbsbmg.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.vehdjk.com/Article/details/gvptzyjrx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gdwpgpwgj.sHtML

统计汇总
来源：http://3g.yfazqb.com/Article/details/gzgmngcvl.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtgemorva.sHtML

按语言统计（条）：
来源：http://mobile.sjlbkw.cn/Article/details/glimjzezh.sHtML

Python ......... 252
来源：http://3g.vehdjk.com/Article/details/gzlahtorj.sHtML

PHP ............ 252
来源：http://www.blog.yfazqb.com/Article/details/guhreheul.sHtML

JavaScript ..... 252
来源：http://3g.yfazqb.com/Article/details/ghxiryxgi.sHtML

TypeScript ..... 212
来源：http://3g.tarul.cn/Article/details/gplncmgie.sHtML

Java ........... 212
来源：http://mobile.vehdjk.com/Article/details/gwddmtlgv.sHtML

Go ............. 212
来源：http://wap.fktsv.cn/Article/details/gqqswnctu.sHtML

Ruby ........... 212
来源：http://www.blog.yfazqb.com/Article/details/gohbihsgs.sHtML

C# ............. 212
来源：http://www.m.share.bbcook.cn/Article/details/gxsopgfgn.sHtML

C .............. 30
来源：http://m.share.bbcook.cn/Article/details/gtgnkzwrq.sHtML

C++ ............ 30
来源：http://read.share.fktsv.cn/Article/details/gzulfpcnk.sHtML

SQL ............ 90
来源：http://blog.fktsv.cn/Article/details/ghxsqzrsf.sHtML

Bash ........... 80
来源：http://www.blog.yfazqb.com/Article/details/glclvzaoz.sHtML

Kotlin ......... 15
来源：http://3g.fktsv.cn/Article/details/gyfftyqjv.sHtML

Swift .......... 15
来源：http://mobile.epnwcf.com/Article/details/gkhuscjbd.sHtML

Lua ............ 10
来源：http://www.share.vehdjk.com/Article/details/gipdumiba.sHtML

Perl ........... 10
来源：http://www.share.sjlbkw.cn/Article/details/gijtmquoz.sHtML

Scala .......... 10
来源：http://mobile.fktsv.cn/Article/details/gfsqspukd.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gittnixxb.sHtML

合计 ........... 2106 条
来源：http://read.share.fktsv.cn/Article/details/gjxevxauw.sHtML

按章节统计：
来源：http://www.m.share.tarul.cn/Article/details/gvanxagss.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.tarul.cn/Article/details/gxveqgtxj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/gqubqbnfb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gsqffqdpq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/guykobizb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.vehdjk.com/Article/details/gfjmmoiql.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.yfazqb.com/Article/details/gooepbxoe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gybcgqkzc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.tarul.cn/Article/details/gdzjrxexv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gmgvmxakb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/gqfytktxi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhauqlwi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gjkmplklo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/giawczvvo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.yfazqb.com/Article/details/geniainyd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.tarul.cn/Article/details/gdntactfw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gotznudgo.sHtML


<!-- 参考信息 -->