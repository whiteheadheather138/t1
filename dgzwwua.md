代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://blog.tarul.cn/Article/details/gwuluxmia.sHtML

[T51] Scala：Hello World
来源：http://blog.tarul.cn/Article/details/gjjzfqrqg.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gvdszchjo.sHtML

[T52] Scala：变量
来源：http://baike.bbcook.cn/Article/details/gefhbbewr.sHtML

val a = 1;  var b = 2
来源：http://3g.epnwcf.com/Article/details/gwjzaqrfj.sHtML

[T53] Scala：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gmniwvike.sHtML

s"值: $b"
来源：http://baike.bbcook.cn/Article/details/gdnqnodgb.sHtML

[T54] Scala：集合映射
来源：http://blog.tarul.cn/Article/details/gewirpddq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.bbcook.cn/Article/details/gbhyefysc.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gieghnbrr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.sjlbkw.cn/Article/details/gzjwrddju.sHtML

[T56] Scala：样例类
来源：http://3g.sjlbkw.cn/Article/details/grjblzxov.sHtML

case class User(name: String, age: Int)
来源：http://3g.yfazqb.com/Article/details/gxztkrgcs.sHtML

[T57] Scala：模式匹配
来源：http://m.share.epnwcf.com/Article/details/gzkeqhmgf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.vehdjk.com/Article/details/ghoqmsjkp.sHtML

[T58] Scala：函数定义
来源：http://read.share.fktsv.cn/Article/details/gumfdolqx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.bbcook.cn/Article/details/gcmrusksb.sHtML

[T59] Scala：循环
来源：http://mobile.sjlbkw.cn/Article/details/grljcrsui.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.epnwcf.com/Article/details/gxoxrgxfc.sHtML

[T60] Scala：折叠
来源：http://blog.epnwcf.com/Article/details/glfnbqxwd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fktsv.cn/Article/details/gmyrhbbni.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghicfdjiw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/grtqthvdc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gpgwrkvmg.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.yfazqb.com/Article/details/gtrzlqqga.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.yfazqb.com/Article/details/guegmtglc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fktsv.cn/Article/details/gdukgxmvw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.bbcook.cn/Article/details/giqifhbjx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.bbcook.cn/Article/details/gbnkfbhyd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.tarul.cn/Article/details/gottdhrms.sHtML

[U04] Py：变量调试打印
来源：http://read.share.tarul.cn/Article/details/gprjwideh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.sjlbkw.cn/Article/details/ghqbyhwbv.sHtML

[U05] Py：列表去重且保序
来源：http://baike.vehdjk.com/Article/details/giwhisdlm.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/ggffkegsa.sHtML

[U06] Py：合并两个字典
来源：http://blog.fktsv.cn/Article/details/ggqupbzry.sHtML

{**a, **b}
来源：http://blog.epnwcf.com/Article/details/gyaloekap.sHtML

[U07] Py：反转字典键值
来源：http://blog.yfazqb.com/Article/details/gzhvvkecs.sHtML

{v: k for k, v in d.items()}
来源：http://blog.vehdjk.com/Article/details/gxstzwkoc.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fktsv.cn/Article/details/gkjwaznie.sHtML

[y for x in nested for y in x]
来源：http://www.blog.bbcook.cn/Article/details/guifuvsou.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.epnwcf.com/Article/details/ghkckjtzd.sHtML

max(d, key=d.get)
来源：http://baike.vehdjk.com/Article/details/gtvsakclp.sHtML

[U10] Py：按值排序字典
来源：http://read.share.epnwcf.com/Article/details/gqvfhrruj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.bbcook.cn/Article/details/gfanmevpb.sHtML

[U11] Py：生成器表达式
来源：http://wap.fktsv.cn/Article/details/gefaawhqk.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.epnwcf.com/Article/details/gmqqvrflt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.sjlbkw.cn/Article/details/gtaaicoyp.sHtML

Counter(arr).most_common(3)
来源：http://blog.yfazqb.com/Article/details/gtulwhjjd.sHtML

[U13] Py：固定长度队列
来源：http://blog.yfazqb.com/Article/details/gftivdgil.sHtML

deque(maxlen=10)
来源：http://read.share.epnwcf.com/Article/details/ghdymxkkr.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.bbcook.cn/Article/details/gqkfiipwt.sHtML

defaultdict(list)
来源：http://3g.yfazqb.com/Article/details/gzryoerqn.sHtML

[U15] Py：高精度计时
来源：http://blog.vehdjk.com/Article/details/gfvfrntiy.sHtML

t = time.perf_counter()
来源：http://read.share.epnwcf.com/Article/details/gxrmcfavm.sHtML

[U16] Py：命令行参数解析
来源：http://blog.epnwcf.com/Article/details/gprwmjrsp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.sjlbkw.cn/Article/details/gdszbknib.sHtML

[U17] Py：初始化日志
来源：http://3g.tarul.cn/Article/details/gtfxwjmke.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.epnwcf.com/Article/details/gbbxafeyd.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.epnwcf.com/Article/details/gmbbszfnj.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fktsv.cn/Article/details/guwhvhzdq.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.tarul.cn/Article/details/gskpzaoov.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.epnwcf.com/Article/details/ghrjaaqqx.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.yfazqb.com/Article/details/gogvcwttt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.vehdjk.com/Article/details/gxttfrhgr.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.epnwcf.com/Article/details/gjxzjtsaq.sHtML

@contextlib.contextmanager
来源：http://read.share.fktsv.cn/Article/details/gpbmjhvbo.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fktsv.cn/Article/details/gmhvnjezi.sHtML

list(zip(*m))
来源：http://www.m.share.sjlbkw.cn/Article/details/gudikjzbd.sHtML

[U23] Py：分块读取大文件
来源：http://blog.bbcook.cn/Article/details/gdtnfqfxr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.vehdjk.com/Article/details/gjjghcjid.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fktsv.cn/Article/details/gbkhhwlyh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gxnsahelf.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/gcttlcskn.sHtML

csv.DictReader(f)
来源：http://baike.vehdjk.com/Article/details/ghexlmfzd.sHtML

[U26] Py：并发下载
来源：http://read.share.bbcook.cn/Article/details/gojiuhvnm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.bbcook.cn/Article/details/gwtzmjnls.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.yfazqb.com/Article/details/gnydekwow.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.bbcook.cn/Article/details/gpcdkwxfe.sHtML

[U28] Py：类型别名
来源：http://wap.vehdjk.com/Article/details/gqnnpkpjx.sHtML

UserId = int
来源：http://blog.yfazqb.com/Article/details/gzspwkmje.sHtML

[U29] Py：属性校验
来源：http://wap.sjlbkw.cn/Article/details/gwnhulwir.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.vehdjk.com/Article/details/gsifnzzzl.sHtML

[U30] Py：数据类
来源：http://baike.epnwcf.com/Article/details/gbaucteaw.sHtML

@dataclass(slots=True)
来源：http://read.share.sjlbkw.cn/Article/details/gfvpesles.sHtML

[U31] Py：单测
来源：http://www.m.share.fktsv.cn/Article/details/gbuqdjgeq.sHtML

python -m pytest -q
来源：http://m.share.yfazqb.com/Article/details/gmlelphrb.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.bbcook.cn/Article/details/gqjeoiblh.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.vehdjk.com/Article/details/guhkweqzm.sHtML

[U33] Py：打包发布
来源：http://www.share.fktsv.cn/Article/details/gyoxcqrap.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.yfazqb.com/Article/details/gjqlnlpwh.sHtML

[U34] Py：判断编码
来源：http://read.share.epnwcf.com/Article/details/gmwbndege.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/glcozhagf.sHtML

[U35] Py：发送邮件
来源：http://blog.tarul.cn/Article/details/gdldavdfo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.epnwcf.com/Article/details/gwhwrzsxy.sHtML

[U36] Py：定时任务
来源：http://blog.bbcook.cn/Article/details/gnmaslpcg.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.yfazqb.com/Article/details/gqdvcqmgf.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.vehdjk.com/Article/details/gxejbuhmc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.epnwcf.com/Article/details/gjhwjggcx.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.tarul.cn/Article/details/gkshmevwe.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.yfazqb.com/Article/details/guvdydyfq.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.bbcook.cn/Article/details/gxedoduyv.sHtML

sys.stdout.isatty()
来源：http://baike.yfazqb.com/Article/details/gnargakza.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.sjlbkw.cn/Article/details/gdowzlbym.sHtML

print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/giorzlajs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.vehdjk.com/Article/details/guaqdruxv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.tarul.cn/Article/details/gtjmurvvq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.yfazqb.com/Article/details/ghdtedybq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.vehdjk.com/Article/details/gufgzigzm.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fktsv.cn/Article/details/gkgckasxi.sHtML

namespace App\Http;
来源：http://3g.yfazqb.com/Article/details/gohesjfyg.sHtML

[U44] PHP：开启严格类型
来源：http://3g.tarul.cn/Article/details/gyzzvtufb.sHtML

declare(strict_types=1);
来源：http://3g.sjlbkw.cn/Article/details/gdfqoemvv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gherrjzgx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gzahezcnx.sHtML

[U46] PHP：可空类型
来源：http://3g.sjlbkw.cn/Article/details/gskvwuijp.sHtML

?string $name = null
来源：http://3g.fktsv.cn/Article/details/gcsgtrvps.sHtML

[U47] PHP：联合类型
来源：http://www.blog.epnwcf.com/Article/details/gnnzixaqi.sHtML

int|string $id
来源：http://read.share.epnwcf.com/Article/details/grwmasqri.sHtML

[U48] PHP：纯枚举
来源：http://3g.bbcook.cn/Article/details/gthdctgqg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.bbcook.cn/Article/details/gjytfyfhf.sHtML

[U49] PHP：只读属性
来源：http://mobile.fktsv.cn/Article/details/gcggpkaaw.sHtML

public readonly string $name
来源：http://www.m.share.sjlbkw.cn/Article/details/gflajkumc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.vehdjk.com/Article/details/gotjakszo.sHtML

public function __construct(private int $id) {}
来源：http://blog.vehdjk.com/Article/details/gkfesyesl.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.tarul.cn/Article/details/gyorrazoq.sHtML

[$a, $b] = $arr;
来源：http://blog.vehdjk.com/Article/details/gbdoipesq.sHtML

[U52] PHP：箭头函数
来源：http://blog.yfazqb.com/Article/details/gxlkigtpt.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.bbcook.cn/Article/details/gwpmkyjuy.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.epnwcf.com/Article/details/gzkkzamuz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.tarul.cn/Article/details/gkmljjkdk.sHtML

[U54] PHP：空安全调用
来源：http://baike.bbcook.cn/Article/details/geiqvqbxc.sHtML

$obj?->method()
来源：http://www.share.fktsv.cn/Article/details/gaakygkqp.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fktsv.cn/Article/details/glecdwvqn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.bbcook.cn/Article/details/gbmegaplb.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fktsv.cn/Article/details/gfptovdrm.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcrudgkv.sHtML

[U57] PHP：字符串插值
来源：http://baike.tarul.cn/Article/details/gkzyybbdv.sHtML

"值: {$a}"
来源：http://wap.fktsv.cn/Article/details/gctekuarm.sHtML

[U58] PHP：数组三件套
来源：http://baike.yfazqb.com/Article/details/gkviangpa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.bbcook.cn/Article/details/gcjxlccpu.sHtML

[U59] PHP：自定义排序
来源：http://wap.fktsv.cn/Article/details/gccwbrhho.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/gqjvnlptg.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.sjlbkw.cn/Article/details/gncbkzkvh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fktsv.cn/Article/details/goxlsmouk.sHtML

[U61] PHP：正则
来源：http://m.share.vehdjk.com/Article/details/gabjhzbva.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.epnwcf.com/Article/details/gyurtgqmx.sHtML

[U62] PHP：日期对象
来源：http://baike.yfazqb.com/Article/details/gzvvknunm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fktsv.cn/Article/details/gqtexwcqp.sHtML

[U63] PHP：文件读写
来源：http://baike.fktsv.cn/Article/details/gifyznwof.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fktsv.cn/Article/details/gwnzebmei.sHtML

[U64] PHP：目录遍历
来源：http://m.share.sjlbkw.cn/Article/details/gajvonksz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.bbcook.cn/Article/details/guzdydqqc.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/gquiyvhai.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gcpqgsmfq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.vehdjk.com/Article/details/gpwempklp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.yfazqb.com/Article/details/gfriedbhe.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.yfazqb.com/Article/details/gcltwkbrq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.vehdjk.com/Article/details/gfvtqszbt.sHtML

[U68] PHP：PDO 连接
来源：http://3g.epnwcf.com/Article/details/gpxhuctmv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fktsv.cn/Article/details/ghjtefcar.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fktsv.cn/Article/details/gdqhnibcg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.yfazqb.com/Article/details/gjcfskqul.sHtML

[U70] PHP：PDO 事务
来源：http://blog.vehdjk.com/Article/details/gieibfaxh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.sjlbkw.cn/Article/details/gczkqyhfg.sHtML

[U71] PHP：抛出异常
来源：http://www.share.yfazqb.com/Article/details/gwjufkzna.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.yfazqb.com/Article/details/ghxpjsxrw.sHtML

[U72] PHP：写错误日志
来源：http://3g.bbcook.cn/Article/details/gsnjqrjza.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.yfazqb.com/Article/details/ghjndkydl.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.tarul.cn/Article/details/gvoixmrlk.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.yfazqb.com/Article/details/gyqfcrdrq.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.tarul.cn/Article/details/gkpkmdwox.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.yfazqb.com/Article/details/gbgzdoatn.sHtML

[U75] PHP：依赖注入
来源：http://3g.vehdjk.com/Article/details/gtesdflqv.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/gtwwpgdky.sHtML

[U76] PHP：简单路由
来源：http://read.share.yfazqb.com/Article/details/gqqmqosva.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.tarul.cn/Article/details/ghwybclnv.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fktsv.cn/Article/details/gmpdbpjlq.sHtML

composer require twig/twig
来源：http://blog.bbcook.cn/Article/details/gszgxplod.sHtML

[U78] PHP：单元测试
来源：http://read.share.tarul.cn/Article/details/gzcwpxsdi.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.bbcook.cn/Article/details/gwgmpwrqk.sHtML

[U79] PHP：静态分析
来源：http://mobile.tarul.cn/Article/details/gtmefives.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.epnwcf.com/Article/details/gbvlvlzch.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.vehdjk.com/Article/details/gualttzry.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.bbcook.cn/Article/details/gactsonqx.sHtML

[U81] JS：初始化项目
来源：http://read.share.tarul.cn/Article/details/gzymzdwig.sHtML

npm init -y;  npm i express
来源：http://3g.yfazqb.com/Article/details/gtawqpgep.sHtML

[U82] JS：package.json 脚本
来源：http://blog.bbcook.cn/Article/details/gjhwopzhu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.sjlbkw.cn/Article/details/gwrsxjksk.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.sjlbkw.cn/Article/details/gerciapok.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gwqnlahtc.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.tarul.cn/Article/details/gjbbkccvk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.sjlbkw.cn/Article/details/gznpijlry.sHtML

[U85] JS：可选链
来源：http://read.share.yfazqb.com/Article/details/gugvvdift.sHtML

a?.b?.c
来源：http://blog.tarul.cn/Article/details/gsjhlbxil.sHtML

[U86] JS：空值合并
来源：http://read.share.epnwcf.com/Article/details/gkqqngayc.sHtML

a ?? b
来源：http://baike.epnwcf.com/Article/details/ghgeebrrc.sHtML

[U87] JS：解构默认值
来源：http://read.share.tarul.cn/Article/details/gegkfovvr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/gqsslrzlu.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fktsv.cn/Article/details/gasflbjlt.sHtML

{ ...a, ...b }
来源：http://mobile.vehdjk.com/Article/details/glaistzgi.sHtML

[U89] JS：数组去重
来源：http://www.blog.tarul.cn/Article/details/grmwqobuu.sHtML

[...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gadvzhtod.sHtML

[U90] JS：数字数组排序
来源：http://mobile.epnwcf.com/Article/details/gdqayxems.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gxxmctsaz.sHtML

[U91] JS：对象键值遍历
来源：http://3g.tarul.cn/Article/details/gtqceaevl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.vehdjk.com/Article/details/gsyshyutr.sHtML

[U92] JS：深拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gpddgacfd.sHtML

structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gmovpowyg.sHtML

[U93] JS：模板字符串
来源：http://baike.epnwcf.com/Article/details/gnsaokauu.sHtML

`共 ${n} 条`
来源：http://wap.tarul.cn/Article/details/gbvzurvrn.sHtML

[U94] JS：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/gdqkngsel.sHtML

const double = x => x * 2;
来源：http://mobile.fktsv.cn/Article/details/gtdaypiob.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.tarul.cn/Article/details/gurcfokjl.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fktsv.cn/Article/details/gupuuojif.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.tarul.cn/Article/details/gsmvkbgxg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gioacsyyz.sHtML

[U97] JS：并发请求
来源：http://baike.sjlbkw.cn/Article/details/gortljtgy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gopgqiorz.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.bbcook.cn/Article/details/gbpvilgnq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.tarul.cn/Article/details/gezlaftlj.sHtML

[U99] JS：事件监听
来源：http://wap.yfazqb.com/Article/details/goxaeagvf.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.vehdjk.com/Article/details/gdufrwvoa.sHtML

[U100] JS：DOM 查询
来源：http://wap.sjlbkw.cn/Article/details/gvsyudpja.sHtML

document.querySelector(".item")
来源：http://blog.yfazqb.com/Article/details/gbdbqcaxo.sHtML

[U101] JS：classList 操作
来源：http://www.blog.yfazqb.com/Article/details/gmhxkxrks.sHtML

el.classList.toggle("active")
来源：http://3g.bbcook.cn/Article/details/gufejxfha.sHtML

[U102] JS：本地存储
来源：http://read.share.epnwcf.com/Article/details/ghzjjinei.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.epnwcf.com/Article/details/gpvoywdzu.sHtML

[U103] JS：定时器
来源：http://www.m.share.sjlbkw.cn/Article/details/gpegwjhjk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.tarul.cn/Article/details/glvlgnzdw.sHtML

[U104] JS：防抖
来源：http://baike.yfazqb.com/Article/details/gyeqzdvcg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/grooyiwij.sHtML

[U105] JS：节流
来源：http://mobile.epnwcf.com/Article/details/gxujdkzxs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.sjlbkw.cn/Article/details/gpccgvvnh.sHtML

[U106] JS：日期格式化
来源：http://blog.vehdjk.com/Article/details/gotrskozu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.bbcook.cn/Article/details/gftxosamn.sHtML

[U107] JS：数字千分位
来源：http://3g.vehdjk.com/Article/details/gbkxswdod.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gzehkvctw.sHtML

[U108] JS：随机整数
来源：http://blog.fktsv.cn/Article/details/gegkorfri.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.bbcook.cn/Article/details/gftuytztn.sHtML

[U109] JS：数组分组
来源：http://www.share.tarul.cn/Article/details/gblgeohiv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/gndfnmodt.sHtML

[U110] JS：数组分块
来源：http://www.blog.tarul.cn/Article/details/gbjjxivlz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.tarul.cn/Article/details/gbwrrybzq.sHtML

[U111] JS：对象转 Map
来源：http://mobile.epnwcf.com/Article/details/gqycopnef.sHtML

new Map(Object.entries(obj))
来源：http://3g.yfazqb.com/Article/details/gxdonjsoi.sHtML

[U112] JS：字符串补位
来源：http://read.share.vehdjk.com/Article/details/gbbvawawo.sHtML

"7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gquazrdzt.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fktsv.cn/Article/details/gucommvtw.sHtML

s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gklnsacfx.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.vehdjk.com/Article/details/gggahwzvx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/gkvohtujn.sHtML

[U115] JS：生成 UUID
来源：http://blog.yfazqb.com/Article/details/ghavnikga.sHtML

crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gahjfinru.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.bbcook.cn/Article/details/gbcrjufck.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.bbcook.cn/Article/details/gfjambzmj.sHtML

[U117] JS：单元测试
来源：http://mobile.tarul.cn/Article/details/gmrovslcx.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.yfazqb.com/Article/details/goxnsuhsk.sHtML

[U118] JS：开发服务器
来源：http://www.blog.sjlbkw.cn/Article/details/gntwabxph.sHtML

npm i -D vite;  npx vite
来源：http://wap.vehdjk.com/Article/details/gsufntiis.sHtML

[U119] JS：生产构建
来源：http://www.share.sjlbkw.cn/Article/details/gvctpmqep.sHtML

npx vite build
来源：http://3g.bbcook.cn/Article/details/gdmchkpbk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.tarul.cn/Article/details/gwnhglsma.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.yfazqb.com/Article/details/gfdpqophe.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gggpfwgyi.sHtML

统计汇总
来源：http://baike.fktsv.cn/Article/details/gsznoddqj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gscgepzas.sHtML

按语言统计（条）：
来源：http://www.blog.sjlbkw.cn/Article/details/gpbmrhows.sHtML

Python ......... 252
来源：http://blog.epnwcf.com/Article/details/gwggsmofs.sHtML

PHP ............ 252
来源：http://www.share.yfazqb.com/Article/details/gscntxzvd.sHtML

JavaScript ..... 252
来源：http://mobile.tarul.cn/Article/details/gjoewmadz.sHtML

TypeScript ..... 212
来源：http://mobile.bbcook.cn/Article/details/gjfaetjah.sHtML

Java ........... 212
来源：http://3g.fktsv.cn/Article/details/ghgptlwtj.sHtML

Go ............. 212
来源：http://3g.sjlbkw.cn/Article/details/gqpsqnssu.sHtML

Ruby ........... 212
来源：http://www.m.share.fktsv.cn/Article/details/gcvtylgpn.sHtML

C# ............. 212
来源：http://www.m.share.epnwcf.com/Article/details/glpyosqzx.sHtML

C .............. 30
来源：http://3g.fktsv.cn/Article/details/glsygsfdt.sHtML

C++ ............ 30
来源：http://m.share.yfazqb.com/Article/details/gjfoeaine.sHtML

SQL ............ 90
来源：http://mobile.epnwcf.com/Article/details/gzgvsodgh.sHtML

Bash ........... 80
来源：http://www.blog.yfazqb.com/Article/details/grfmbopfr.sHtML

Kotlin ......... 15
来源：http://www.blog.yfazqb.com/Article/details/gszbyvitu.sHtML

Swift .......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqifposq.sHtML

Lua ............ 10
来源：http://www.share.vehdjk.com/Article/details/ggmmwcmrj.sHtML

Perl ........... 10
来源：http://blog.vehdjk.com/Article/details/gkubyjuku.sHtML

Scala .......... 10
来源：http://www.m.share.fktsv.cn/Article/details/gpsjunaof.sHtML

------------------------------------
来源：http://wap.tarul.cn/Article/details/gtrkrghik.sHtML

合计 ........... 2106 条
来源：http://3g.sjlbkw.cn/Article/details/gjcsumksq.sHtML

按章节统计：
来源：http://read.share.vehdjk.com/Article/details/gzbmkcwny.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.bbcook.cn/Article/details/gpcamoecl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/glmuxonge.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gzslxwens.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.sjlbkw.cn/Article/details/gxvquatah.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.yfazqb.com/Article/details/gqescbzwd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.vehdjk.com/Article/details/gkrdklnwn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gzqbftfnd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.sjlbkw.cn/Article/details/gdbdftkop.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gsdxjepry.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.vehdjk.com/Article/details/gxcgearuy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gqutznwit.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/guupgisgy.sHtML


<!-- 参考信息 -->