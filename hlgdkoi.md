代发 wailian999

val a = 1;  var b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gratlkzer.sHtML

[T53] Scala：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gpxvxmqzr.sHtML

s"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/gvdcspsij.sHtML

[T54] Scala：集合映射
来源：http://m.share.bbcook.cn/Article/details/gpzidpcle.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fktsv.cn/Article/details/garhxtkne.sHtML

[T55] Scala：集合过滤
来源：http://baike.fktsv.cn/Article/details/gjcxxeems.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.epnwcf.com/Article/details/gfgwzjghb.sHtML

[T56] Scala：样例类
来源：http://baike.epnwcf.com/Article/details/gaeorfnat.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/gcvaqljod.sHtML

[T57] Scala：模式匹配
来源：http://baike.yfazqb.com/Article/details/gqludnjzg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.yfazqb.com/Article/details/gmmozmkia.sHtML

[T58] Scala：函数定义
来源：http://3g.fktsv.cn/Article/details/gnxzmsjok.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.tarul.cn/Article/details/gnerglawr.sHtML

[T59] Scala：循环
来源：http://mobile.tarul.cn/Article/details/gvyozfsyn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gidazblrx.sHtML

[T60] Scala：折叠
来源：http://www.share.fktsv.cn/Article/details/gqjsozwuv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.epnwcf.com/Article/details/gnkzuovoh.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwvuqzgom.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/geoeebshv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gthpmwsia.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.vehdjk.com/Article/details/gsyaiynqc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.bbcook.cn/Article/details/gvtentdvc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.epnwcf.com/Article/details/gweksdemd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gfeqomitp.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.epnwcf.com/Article/details/ggnxptdfz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.tarul.cn/Article/details/gszsqkvhn.sHtML

[U04] Py：变量调试打印
来源：http://www.share.yfazqb.com/Article/details/gwhoaajgr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.sjlbkw.cn/Article/details/ggzrfnewb.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.sjlbkw.cn/Article/details/grajpztfz.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gyythipjj.sHtML

[U06] Py：合并两个字典
来源：http://m.share.epnwcf.com/Article/details/gjwpardhm.sHtML

{**a, **b}
来源：http://www.share.tarul.cn/Article/details/gqxhxrulp.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fktsv.cn/Article/details/ggdtoyefh.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.epnwcf.com/Article/details/gbpiofqif.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fktsv.cn/Article/details/gdwwnriua.sHtML

[y for x in nested for y in x]
来源：http://www.blog.vehdjk.com/Article/details/galtjnnbu.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fktsv.cn/Article/details/gxqrbrpyd.sHtML

max(d, key=d.get)
来源：http://3g.yfazqb.com/Article/details/gzosrzjvz.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.bbcook.cn/Article/details/gposyoute.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.tarul.cn/Article/details/gfqqquwbe.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fktsv.cn/Article/details/gawpwzptk.sHtML

(x * 2 for x in arr)
来源：http://mobile.tarul.cn/Article/details/gfiiyboiy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/gxjnxxrxj.sHtML

Counter(arr).most_common(3)
来源：http://3g.epnwcf.com/Article/details/gaqexlymq.sHtML

[U13] Py：固定长度队列
来源：http://wap.yfazqb.com/Article/details/giizpykun.sHtML

deque(maxlen=10)
来源：http://read.share.tarul.cn/Article/details/goazayfyo.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.vehdjk.com/Article/details/gmpnogeyj.sHtML

defaultdict(list)
来源：http://read.share.yfazqb.com/Article/details/gzzfivdsp.sHtML

[U15] Py：高精度计时
来源：http://read.share.yfazqb.com/Article/details/gnvjtglwx.sHtML

t = time.perf_counter()
来源：http://www.share.vehdjk.com/Article/details/gxjkbhsth.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.epnwcf.com/Article/details/gclmukcxk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.sjlbkw.cn/Article/details/gxkiexatr.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.vehdjk.com/Article/details/gumhjpiha.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.epnwcf.com/Article/details/gjtblgztf.sHtML

[U18] Py：预编译正则
来源：http://www.blog.bbcook.cn/Article/details/gbfbtwhyf.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.tarul.cn/Article/details/gnpejbhsg.sHtML

[U19] Py：正则替换带回调
来源：http://baike.tarul.cn/Article/details/gfrbezmsz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.bbcook.cn/Article/details/gjscbyajm.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.bbcook.cn/Article/details/gykcetmxd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.epnwcf.com/Article/details/gqcshivbb.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.epnwcf.com/Article/details/gosmmcgmt.sHtML

@contextlib.contextmanager
来源：http://blog.bbcook.cn/Article/details/gpultmlpb.sHtML

[U22] Py：矩阵转置
来源：http://www.share.epnwcf.com/Article/details/gkcpxursg.sHtML

list(zip(*m))
来源：http://3g.tarul.cn/Article/details/gnoxaipqk.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fktsv.cn/Article/details/guzptanjk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.tarul.cn/Article/details/gkwcciqnp.sHtML

[U24] Py：路径操作
来源：http://mobile.vehdjk.com/Article/details/grirlybes.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.yfazqb.com/Article/details/gtiwqshuy.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.yfazqb.com/Article/details/gxwjvelzo.sHtML

csv.DictReader(f)
来源：http://baike.bbcook.cn/Article/details/gdhgtxxph.sHtML

[U26] Py：并发下载
来源：http://read.share.vehdjk.com/Article/details/gpgtrpcao.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.bbcook.cn/Article/details/gnpzmidzn.sHtML

[U27] Py：异步 HTTP
来源：http://wap.tarul.cn/Article/details/gxbkuiyga.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fktsv.cn/Article/details/gbnzndsii.sHtML

[U28] Py：类型别名
来源：http://mobile.sjlbkw.cn/Article/details/gfgpggbvi.sHtML

UserId = int
来源：http://blog.fktsv.cn/Article/details/goouymayp.sHtML

[U29] Py：属性校验
来源：http://blog.yfazqb.com/Article/details/gldpdjwmd.sHtML

@property 与 @x.setter 配合
来源：http://m.share.vehdjk.com/Article/details/golpefgnt.sHtML

[U30] Py：数据类
来源：http://www.m.share.tarul.cn/Article/details/gmxdyqbiy.sHtML

@dataclass(slots=True)
来源：http://m.share.tarul.cn/Article/details/gkifrgwte.sHtML

[U31] Py：单测
来源：http://read.share.tarul.cn/Article/details/gfddyybmr.sHtML

python -m pytest -q
来源：http://m.share.epnwcf.com/Article/details/gqffwqfuc.sHtML

[U32] Py：代码格式化
来源：http://blog.yfazqb.com/Article/details/gletvxnmm.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.epnwcf.com/Article/details/gnhumlkto.sHtML

[U33] Py：打包发布
来源：http://www.share.yfazqb.com/Article/details/gnewjuqmm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.vehdjk.com/Article/details/gnlinnhoa.sHtML

[U34] Py：判断编码
来源：http://www.blog.yfazqb.com/Article/details/gpdrlcibu.sHtML

chardet.detect(raw)
来源：http://www.share.sjlbkw.cn/Article/details/gwsyelpmu.sHtML

[U35] Py：发送邮件
来源：http://wap.tarul.cn/Article/details/gvoslisrq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.bbcook.cn/Article/details/gosqpfipi.sHtML

[U36] Py：定时任务
来源：http://m.share.yfazqb.com/Article/details/grqqxpivy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.yfazqb.com/Article/details/gmotiedfu.sHtML

[U37] Py：读写 Excel
来源：http://blog.yfazqb.com/Article/details/grtztuevt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.sjlbkw.cn/Article/details/gyqcndflk.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.tarul.cn/Article/details/gkvtxvvwo.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fktsv.cn/Article/details/gbcktyunj.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.vehdjk.com/Article/details/gcdkcixhp.sHtML

sys.stdout.isatty()
来源：http://blog.vehdjk.com/Article/details/geumwdmwo.sHtML

[U40] Py：打印到标准错误
来源：http://blog.tarul.cn/Article/details/gtmvytswi.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fktsv.cn/Article/details/gvgtlpley.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fktsv.cn/Article/details/geljxzlpc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.tarul.cn/Article/details/gpbyurxge.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.epnwcf.com/Article/details/grtwgxirl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.yfazqb.com/Article/details/gvokzfljs.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fktsv.cn/Article/details/gznwmhylq.sHtML

namespace App\Http;
来源：http://mobile.tarul.cn/Article/details/gokrcrxht.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.vehdjk.com/Article/details/grbmfuvkb.sHtML

declare(strict_types=1);
来源：http://baike.yfazqb.com/Article/details/gmijwjpiz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fktsv.cn/Article/details/gskcchtcp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gwjacbdbw.sHtML

[U46] PHP：可空类型
来源：http://wap.vehdjk.com/Article/details/gpawzjkkz.sHtML

?string $name = null
来源：http://www.blog.bbcook.cn/Article/details/gynhzufto.sHtML

[U47] PHP：联合类型
来源：http://blog.yfazqb.com/Article/details/gtwmtmjhu.sHtML

int|string $id
来源：http://www.m.share.yfazqb.com/Article/details/gezfvfctt.sHtML

[U48] PHP：纯枚举
来源：http://www.share.tarul.cn/Article/details/gxoifeqbk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.yfazqb.com/Article/details/gdaxmmkgv.sHtML

[U49] PHP：只读属性
来源：http://www.blog.tarul.cn/Article/details/gjocgmbsr.sHtML

public readonly string $name
来源：http://m.share.bbcook.cn/Article/details/gxrujinzw.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.epnwcf.com/Article/details/ggdpgxsos.sHtML

public function __construct(private int $id) {}
来源：http://www.share.vehdjk.com/Article/details/gcyyhnxwe.sHtML

[U51] PHP：数组解构
来源：http://mobile.epnwcf.com/Article/details/gkgufufab.sHtML

[$a, $b] = $arr;
来源：http://www.blog.bbcook.cn/Article/details/gswzmqqtv.sHtML

[U52] PHP：箭头函数
来源：http://3g.yfazqb.com/Article/details/glywgqnft.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.sjlbkw.cn/Article/details/gelhbynrd.sHtML

[U53] PHP：空合并运算符
来源：http://baike.tarul.cn/Article/details/gtwqxkccb.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.vehdjk.com/Article/details/glayvbjqk.sHtML

[U54] PHP：空安全调用
来源：http://blog.vehdjk.com/Article/details/grisxotby.sHtML

$obj?->method()
来源：http://www.share.sjlbkw.cn/Article/details/gzzpxfmsz.sHtML

[U55] PHP：match 表达式
来源：http://m.share.vehdjk.com/Article/details/gsyuskyub.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.vehdjk.com/Article/details/gcqypjznc.sHtML

[U56] PHP：命名参数
来源：http://m.share.yfazqb.com/Article/details/godlovtho.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gwtgkugle.sHtML

[U57] PHP：字符串插值
来源：http://blog.fktsv.cn/Article/details/gouixeozq.sHtML

"值: {$a}"
来源：http://blog.tarul.cn/Article/details/gtahvarqf.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.tarul.cn/Article/details/gonsbspov.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.epnwcf.com/Article/details/gstjivxwf.sHtML

[U59] PHP：自定义排序
来源：http://3g.epnwcf.com/Article/details/glipmuxen.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.bbcook.cn/Article/details/ghbwtqgmh.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.epnwcf.com/Article/details/gbqvlwjgn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gytaspgfz.sHtML

[U61] PHP：正则
来源：http://www.blog.tarul.cn/Article/details/gqpaiofsn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gspdzrvbg.sHtML

[U62] PHP：日期对象
来源：http://m.share.fktsv.cn/Article/details/gmrhzttvf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.bbcook.cn/Article/details/gxhjrttnu.sHtML

[U63] PHP：文件读写
来源：http://read.share.sjlbkw.cn/Article/details/gutpmkppn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.sjlbkw.cn/Article/details/gkgmsfkcf.sHtML

[U64] PHP：目录遍历
来源：http://baike.vehdjk.com/Article/details/ghsxqrhwe.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.tarul.cn/Article/details/gcxtghahb.sHtML

[U65] PHP：会话
来源：http://mobile.yfazqb.com/Article/details/gvylhjxga.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.yfazqb.com/Article/details/gmqscuvkg.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.vehdjk.com/Article/details/geeagduzc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.yfazqb.com/Article/details/glpivxmwn.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.epnwcf.com/Article/details/gxajlzaiq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.vehdjk.com/Article/details/gbsnffhks.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fktsv.cn/Article/details/gfbszyrrx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.tarul.cn/Article/details/gldrkpity.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.sjlbkw.cn/Article/details/ggcmxaiyu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.vehdjk.com/Article/details/gephrkboz.sHtML

[U70] PHP：PDO 事务
来源：http://blog.yfazqb.com/Article/details/gliqvbtyw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.bbcook.cn/Article/details/geufqvuac.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/grdybosfe.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.vehdjk.com/Article/details/gevhygozg.sHtML

[U72] PHP：写错误日志
来源：http://read.share.yfazqb.com/Article/details/ghahiztdt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.tarul.cn/Article/details/gwgkgepbb.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.yfazqb.com/Article/details/gafdgldro.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.tarul.cn/Article/details/gslkwaaom.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gauiceldf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.bbcook.cn/Article/details/gfkvdqctm.sHtML

[U75] PHP：依赖注入
来源：http://3g.epnwcf.com/Article/details/gxpguanjt.sHtML

composer require psr/container
来源：http://www.blog.epnwcf.com/Article/details/guztkrvgf.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.bbcook.cn/Article/details/gxnveexeb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.sjlbkw.cn/Article/details/gaasrizpi.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fktsv.cn/Article/details/gkzoklypf.sHtML

composer require twig/twig
来源：http://3g.epnwcf.com/Article/details/gmnqutdjs.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.epnwcf.com/Article/details/gapgidggr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.tarul.cn/Article/details/ggibarwnu.sHtML

[U79] PHP：静态分析
来源：http://read.share.vehdjk.com/Article/details/glmxjdtcg.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.yfazqb.com/Article/details/gecltvozw.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.yfazqb.com/Article/details/gxftmwqcx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.vehdjk.com/Article/details/gvclofbdu.sHtML

[U81] JS：初始化项目
来源：http://mobile.epnwcf.com/Article/details/glkqgfvnd.sHtML

npm init -y;  npm i express
来源：http://blog.vehdjk.com/Article/details/gkaqglmxf.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fktsv.cn/Article/details/gpgpnqdas.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.bbcook.cn/Article/details/gljclpepd.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.epnwcf.com/Article/details/gmrnuvfve.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.yfazqb.com/Article/details/gnixtmlir.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.vehdjk.com/Article/details/grwalctrq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fktsv.cn/Article/details/glpczdepi.sHtML

[U85] JS：可选链
来源：http://m.share.bbcook.cn/Article/details/gkstafaui.sHtML

a?.b?.c
来源：http://mobile.bbcook.cn/Article/details/gmrbbshwt.sHtML

[U86] JS：空值合并
来源：http://mobile.bbcook.cn/Article/details/gtlafcfif.sHtML

a ?? b
来源：http://blog.sjlbkw.cn/Article/details/gulirxhse.sHtML

[U87] JS：解构默认值
来源：http://blog.tarul.cn/Article/details/grttqpqfu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.sjlbkw.cn/Article/details/gmreefgyh.sHtML

[U88] JS：对象展开合并
来源：http://baike.bbcook.cn/Article/details/gpshnadgd.sHtML

{ ...a, ...b }
来源：http://m.share.epnwcf.com/Article/details/gpxclgevc.sHtML

[U89] JS：数组去重
来源：http://www.blog.yfazqb.com/Article/details/gwtceaoto.sHtML

[...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/ganfiwtro.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.tarul.cn/Article/details/gvwuhilhu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gxbybvjdl.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fktsv.cn/Article/details/ggongwygw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.bbcook.cn/Article/details/gitrpfjex.sHtML

[U92] JS：深拷贝
来源：http://blog.fktsv.cn/Article/details/gyrljnuki.sHtML

structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gdvhlvorn.sHtML

[U93] JS：模板字符串
来源：http://read.share.yfazqb.com/Article/details/grfacfiqk.sHtML

`共 ${n} 条`
来源：http://www.blog.epnwcf.com/Article/details/gdhtafuei.sHtML

[U94] JS：箭头函数
来源：http://3g.vehdjk.com/Article/details/geyqwjuea.sHtML

const double = x => x * 2;
来源：http://blog.tarul.cn/Article/details/grkmgrkkr.sHtML

[U95] JS：Promise 包装
来源：http://baike.sjlbkw.cn/Article/details/gyxtwsyvx.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.tarul.cn/Article/details/gcxbmrgid.sHtML

[U96] JS：async/await 与异常
来源：http://baike.bbcook.cn/Article/details/gmcbdvfml.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/ghuhvpuvg.sHtML

[U97] JS：并发请求
来源：http://mobile.tarul.cn/Article/details/gcjfastsc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/ghgaypaft.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.sjlbkw.cn/Article/details/gelctwzdz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.bbcook.cn/Article/details/gllyrnrqb.sHtML

[U99] JS：事件监听
来源：http://wap.fktsv.cn/Article/details/gdbnrirwq.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gegswfkrg.sHtML

[U100] JS：DOM 查询
来源：http://3g.tarul.cn/Article/details/gcaaemqkh.sHtML

document.querySelector(".item")
来源：http://www.blog.fktsv.cn/Article/details/gkcxbvuak.sHtML

[U101] JS：classList 操作
来源：http://baike.yfazqb.com/Article/details/ggtpfhbxx.sHtML

el.classList.toggle("active")
来源：http://3g.sjlbkw.cn/Article/details/gtdymppjz.sHtML

[U102] JS：本地存储
来源：http://m.share.yfazqb.com/Article/details/gdukodexh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.sjlbkw.cn/Article/details/gqajcazrb.sHtML

[U103] JS：定时器
来源：http://www.share.fktsv.cn/Article/details/gwdabjfly.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.yfazqb.com/Article/details/glmbwmphd.sHtML

[U104] JS：防抖
来源：http://www.share.vehdjk.com/Article/details/gfelqitor.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gfkdvbrrd.sHtML

[U105] JS：节流
来源：http://wap.bbcook.cn/Article/details/gkuxrzich.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.epnwcf.com/Article/details/gmaiwsgdo.sHtML

[U106] JS：日期格式化
来源：http://m.share.epnwcf.com/Article/details/gzxziickf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.epnwcf.com/Article/details/gjynydarf.sHtML

[U107] JS：数字千分位
来源：http://3g.bbcook.cn/Article/details/gjljaugim.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gqcqisdjd.sHtML

[U108] JS：随机整数
来源：http://3g.tarul.cn/Article/details/gicwuulcb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.tarul.cn/Article/details/gqgonavvg.sHtML

[U109] JS：数组分组
来源：http://blog.fktsv.cn/Article/details/gssqfszbe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/ggxbnagih.sHtML

[U110] JS：数组分块
来源：http://3g.fktsv.cn/Article/details/glyfsgomb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.tarul.cn/Article/details/gqjyzdoqe.sHtML

[U111] JS：对象转 Map
来源：http://mobile.tarul.cn/Article/details/gfxiklern.sHtML

new Map(Object.entries(obj))
来源：http://mobile.sjlbkw.cn/Article/details/gcyroixab.sHtML

[U112] JS：字符串补位
来源：http://blog.fktsv.cn/Article/details/gbhbpzxsm.sHtML

"7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gqahdsiag.sHtML

[U113] JS：正则替换全部
来源：http://mobile.yfazqb.com/Article/details/gfzoxsvwf.sHtML

s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gmqkzrntt.sHtML

[U114] JS：JSON 深比较
来源：http://3g.yfazqb.com/Article/details/gmvksabek.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.epnwcf.com/Article/details/gxpsfzqmc.sHtML

[U115] JS：生成 UUID
来源：http://blog.bbcook.cn/Article/details/gzfewohgs.sHtML

crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gvnangjij.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fktsv.cn/Article/details/gupelrvrz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.yfazqb.com/Article/details/gtzlosqfe.sHtML

[U117] JS：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gfjfosfsn.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.bbcook.cn/Article/details/gubeoixay.sHtML

[U118] JS：开发服务器
来源：http://m.share.vehdjk.com/Article/details/gxiktfhrz.sHtML

npm i -D vite;  npx vite
来源：http://www.share.epnwcf.com/Article/details/gkgrrmuuk.sHtML

[U119] JS：生产构建
来源：http://read.share.bbcook.cn/Article/details/gxsjdhxuf.sHtML

npx vite build
来源：http://read.share.epnwcf.com/Article/details/gkhirmwbp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.epnwcf.com/Article/details/gzrqnzkqv.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fktsv.cn/Article/details/gkkuvigfq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gbetsyoiz.sHtML

统计汇总
来源：http://3g.bbcook.cn/Article/details/gwczcfpeo.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gyefubans.sHtML

按语言统计（条）：
来源：http://www.m.share.vehdjk.com/Article/details/gqzdnjtrt.sHtML

Python ......... 252
来源：http://m.share.vehdjk.com/Article/details/gjtzmhpix.sHtML

PHP ............ 252
来源：http://www.share.vehdjk.com/Article/details/glqfpwgpr.sHtML

JavaScript ..... 252
来源：http://mobile.tarul.cn/Article/details/gdufuzsyz.sHtML

TypeScript ..... 212
来源：http://wap.bbcook.cn/Article/details/gwgdeeuiv.sHtML

Java ........... 212
来源：http://read.share.yfazqb.com/Article/details/gbuuuegxj.sHtML

Go ............. 212
来源：http://blog.vehdjk.com/Article/details/gowrjnjte.sHtML

Ruby ........... 212
来源：http://baike.yfazqb.com/Article/details/gayyvmvds.sHtML

C# ............. 212
来源：http://www.share.tarul.cn/Article/details/gxzdwzdno.sHtML

C .............. 30
来源：http://www.share.bbcook.cn/Article/details/gkpkmoaei.sHtML

C++ ............ 30
来源：http://www.blog.bbcook.cn/Article/details/gpzbouexm.sHtML

SQL ............ 90
来源：http://www.blog.vehdjk.com/Article/details/gvyppjbjz.sHtML

Bash ........... 80
来源：http://3g.fktsv.cn/Article/details/gcfmzbfvx.sHtML

Kotlin ......... 15
来源：http://mobile.epnwcf.com/Article/details/gdjndkeiu.sHtML

Swift .......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/geqhlgsgf.sHtML

Lua ............ 10
来源：http://blog.epnwcf.com/Article/details/gubpptnol.sHtML

Perl ........... 10
来源：http://mobile.sjlbkw.cn/Article/details/gczlyeuyl.sHtML

Scala .......... 10
来源：http://www.blog.bbcook.cn/Article/details/gqngxenjn.sHtML

------------------------------------
来源：http://mobile.bbcook.cn/Article/details/glhckstyw.sHtML

合计 ........... 2106 条
来源：http://3g.sjlbkw.cn/Article/details/gxurdpmvx.sHtML

按章节统计：
来源：http://read.share.yfazqb.com/Article/details/gmkjphofd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fktsv.cn/Article/details/gpipanfwz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/gcvhmnfly.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/ghyufasad.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fktsv.cn/Article/details/gwpvndeej.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.bbcook.cn/Article/details/gsmlxzsaw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.sjlbkw.cn/Article/details/gwdxdafnl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/glfbehnxl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.tarul.cn/Article/details/ghevaeljy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/godyfbtlf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.bbcook.cn/Article/details/glbawmuts.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/golmdiztc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gydnyydjs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/gnztigeib.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.yfazqb.com/Article/details/gclyhqmeh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fktsv.cn/Article/details/grpizfetj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gzefjhlyz.sHtML


<!-- 参考信息 -->