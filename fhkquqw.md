代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://baike.epnwcf.com/Article/details/gxrfhyrds.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gkoqdrqst.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.epnwcf.com/Article/details/ginuykojr.sHtML

[T56] Scala：样例类
来源：http://www.share.vehdjk.com/Article/details/ghocrlooi.sHtML

case class User(name: String, age: Int)
来源：http://blog.tarul.cn/Article/details/gcycvhcdm.sHtML

[T57] Scala：模式匹配
来源：http://3g.fktsv.cn/Article/details/gokovzzbg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.yfazqb.com/Article/details/gjwqsajyo.sHtML

[T58] Scala：函数定义
来源：http://www.blog.vehdjk.com/Article/details/grsleotgp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.sjlbkw.cn/Article/details/gjyafytxk.sHtML

[T59] Scala：循环
来源：http://baike.epnwcf.com/Article/details/gursspgui.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.vehdjk.com/Article/details/gtdlybfgd.sHtML

[T60] Scala：折叠
来源：http://wap.bbcook.cn/Article/details/gmbfaxfck.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.tarul.cn/Article/details/gxxraquvs.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gsrxwcbzo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.yfazqb.com/Article/details/gtngxionk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gldbkhbcs.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.yfazqb.com/Article/details/gmzmwweoo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.yfazqb.com/Article/details/gzbthbjyy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.yfazqb.com/Article/details/grexizhdn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gpbzpzifd.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.yfazqb.com/Article/details/gzwatqzrs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.epnwcf.com/Article/details/gztyxqfov.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.tarul.cn/Article/details/gfflxvppy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.tarul.cn/Article/details/gvmblksam.sHtML

[U05] Py：列表去重且保序
来源：http://baike.vehdjk.com/Article/details/gtwmxapir.sHtML

list(dict.fromkeys(arr))
来源：http://3g.vehdjk.com/Article/details/gzckktzjg.sHtML

[U06] Py：合并两个字典
来源：http://m.share.sjlbkw.cn/Article/details/goazonoux.sHtML

{**a, **b}
来源：http://blog.yfazqb.com/Article/details/gjatykbit.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/glvqwdmpi.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.bbcook.cn/Article/details/gxgjgzorf.sHtML

[U08] Py：展平二维列表
来源：http://mobile.epnwcf.com/Article/details/ghcsdmmgt.sHtML

[y for x in nested for y in x]
来源：http://m.share.yfazqb.com/Article/details/gswskwuqw.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fktsv.cn/Article/details/gsgdipqnb.sHtML

max(d, key=d.get)
来源：http://baike.vehdjk.com/Article/details/gbgscifct.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/gdfjvlqgc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fktsv.cn/Article/details/gguzopazz.sHtML

[U11] Py：生成器表达式
来源：http://blog.tarul.cn/Article/details/gyfgymojb.sHtML

(x * 2 for x in arr)
来源：http://mobile.tarul.cn/Article/details/gnakqncag.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.tarul.cn/Article/details/gnlobkcio.sHtML

Counter(arr).most_common(3)
来源：http://blog.fktsv.cn/Article/details/gnkcexhar.sHtML

[U13] Py：固定长度队列
来源：http://mobile.sjlbkw.cn/Article/details/gczthxmzp.sHtML

deque(maxlen=10)
来源：http://blog.sjlbkw.cn/Article/details/gfpaeotnr.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.tarul.cn/Article/details/gkdxcvezq.sHtML

defaultdict(list)
来源：http://read.share.epnwcf.com/Article/details/gxoeqxthv.sHtML

[U15] Py：高精度计时
来源：http://m.share.sjlbkw.cn/Article/details/gpboqnmlz.sHtML

t = time.perf_counter()
来源：http://www.m.share.epnwcf.com/Article/details/gxovewqqv.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.epnwcf.com/Article/details/gbaameato.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.yfazqb.com/Article/details/gcpuvibmb.sHtML

[U17] Py：初始化日志
来源：http://wap.tarul.cn/Article/details/gveiwwbng.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.yfazqb.com/Article/details/gdgxobpgn.sHtML

[U18] Py：预编译正则
来源：http://wap.sjlbkw.cn/Article/details/gbcqvnlgk.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/grrhojpgv.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.bbcook.cn/Article/details/gnautqsft.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.epnwcf.com/Article/details/gaeausjcy.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.vehdjk.com/Article/details/gjcczkhvb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.sjlbkw.cn/Article/details/gimisrtcq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.tarul.cn/Article/details/gggtgqxvz.sHtML

@contextlib.contextmanager
来源：http://www.m.share.tarul.cn/Article/details/gxqekwhno.sHtML

[U22] Py：矩阵转置
来源：http://mobile.bbcook.cn/Article/details/gfqdrykkp.sHtML

list(zip(*m))
来源：http://baike.fktsv.cn/Article/details/gtamthpsj.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.vehdjk.com/Article/details/gouvsegbk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.vehdjk.com/Article/details/guqexqusl.sHtML

[U24] Py：路径操作
来源：http://read.share.vehdjk.com/Article/details/giismispi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gqebpfsbo.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.vehdjk.com/Article/details/gpjipnlke.sHtML

csv.DictReader(f)
来源：http://www.m.share.yfazqb.com/Article/details/gxpkfusmi.sHtML

[U26] Py：并发下载
来源：http://www.blog.epnwcf.com/Article/details/ghldcqpma.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.tarul.cn/Article/details/gyigclita.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.vehdjk.com/Article/details/gnlpvogml.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.epnwcf.com/Article/details/gmdinsziz.sHtML

[U28] Py：类型别名
来源：http://m.share.sjlbkw.cn/Article/details/gdwgtakoo.sHtML

UserId = int
来源：http://m.share.bbcook.cn/Article/details/gxllyxvmy.sHtML

[U29] Py：属性校验
来源：http://mobile.sjlbkw.cn/Article/details/gqooibvcd.sHtML

@property 与 @x.setter 配合
来源：http://wap.sjlbkw.cn/Article/details/gaorpkmdp.sHtML

[U30] Py：数据类
来源：http://www.share.vehdjk.com/Article/details/gfjeklcef.sHtML

@dataclass(slots=True)
来源：http://m.share.bbcook.cn/Article/details/gbuioauzf.sHtML

[U31] Py：单测
来源：http://read.share.epnwcf.com/Article/details/guibwjvzt.sHtML

python -m pytest -q
来源：http://www.blog.epnwcf.com/Article/details/gllpjqozh.sHtML

[U32] Py：代码格式化
来源：http://blog.bbcook.cn/Article/details/gjrmkdkud.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.epnwcf.com/Article/details/gttatujuy.sHtML

[U33] Py：打包发布
来源：http://www.m.share.bbcook.cn/Article/details/gubtuhump.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.vehdjk.com/Article/details/gpdysaktc.sHtML

[U34] Py：判断编码
来源：http://blog.yfazqb.com/Article/details/ggymbnlqj.sHtML

chardet.detect(raw)
来源：http://blog.sjlbkw.cn/Article/details/giycgjlqc.sHtML

[U35] Py：发送邮件
来源：http://www.blog.vehdjk.com/Article/details/gtetpibaw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.tarul.cn/Article/details/gqezyxdng.sHtML

[U36] Py：定时任务
来源：http://wap.yfazqb.com/Article/details/gypggzakq.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.bbcook.cn/Article/details/grtifszek.sHtML

[U37] Py：读写 Excel
来源：http://m.share.bbcook.cn/Article/details/gausapael.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.tarul.cn/Article/details/gxplkcjhv.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.bbcook.cn/Article/details/gpxzoahfu.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fktsv.cn/Article/details/gwqbbycxq.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.bbcook.cn/Article/details/gdxbdqmkx.sHtML

sys.stdout.isatty()
来源：http://3g.tarul.cn/Article/details/gcgraxjgr.sHtML

[U40] Py：打印到标准错误
来源：http://wap.vehdjk.com/Article/details/guxojxqmk.sHtML

print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/gtgbzrhwn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.epnwcf.com/Article/details/gmomcjgkq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.yfazqb.com/Article/details/gjiwzfelu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.sjlbkw.cn/Article/details/gvbzidghz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.tarul.cn/Article/details/gygehdzbw.sHtML

[U43] PHP：声明命名空间
来源：http://blog.vehdjk.com/Article/details/gdvmqoxxj.sHtML

namespace App\Http;
来源：http://blog.epnwcf.com/Article/details/gucyvoaws.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.sjlbkw.cn/Article/details/gmsayznyn.sHtML

declare(strict_types=1);
来源：http://www.m.share.epnwcf.com/Article/details/gkmcftntt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.yfazqb.com/Article/details/gfqwtlwbx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gsbbunuqf.sHtML

[U46] PHP：可空类型
来源：http://mobile.vehdjk.com/Article/details/gqmcfjsoe.sHtML

?string $name = null
来源：http://www.share.tarul.cn/Article/details/gjwlmxebw.sHtML

[U47] PHP：联合类型
来源：http://m.share.fktsv.cn/Article/details/gpgtmgwed.sHtML

int|string $id
来源：http://mobile.sjlbkw.cn/Article/details/gbaoltzcv.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.epnwcf.com/Article/details/gcezzkomi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.tarul.cn/Article/details/gdxnsweyv.sHtML

[U49] PHP：只读属性
来源：http://read.share.bbcook.cn/Article/details/ghxzmppmc.sHtML

public readonly string $name
来源：http://baike.bbcook.cn/Article/details/gpketmopp.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.tarul.cn/Article/details/gtbszzluz.sHtML

public function __construct(private int $id) {}
来源：http://3g.bbcook.cn/Article/details/glxkfuxxr.sHtML

[U51] PHP：数组解构
来源：http://mobile.epnwcf.com/Article/details/gvgkhisvz.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fktsv.cn/Article/details/gyfqcstyb.sHtML

[U52] PHP：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/gfwcqrklo.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.bbcook.cn/Article/details/gubpuumwy.sHtML

[U53] PHP：空合并运算符
来源：http://baike.tarul.cn/Article/details/gjojwhduc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.yfazqb.com/Article/details/grznmjsum.sHtML

[U54] PHP：空安全调用
来源：http://read.share.sjlbkw.cn/Article/details/ggpeciclk.sHtML

$obj?->method()
来源：http://mobile.epnwcf.com/Article/details/gddldowyl.sHtML

[U55] PHP：match 表达式
来源：http://3g.epnwcf.com/Article/details/gambkgnhl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoqtieny.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.epnwcf.com/Article/details/guukdknks.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnztpctdn.sHtML

[U57] PHP：字符串插值
来源：http://mobile.tarul.cn/Article/details/gvmzswsui.sHtML

"值: {$a}"
来源：http://3g.tarul.cn/Article/details/gkiwajdnb.sHtML

[U58] PHP：数组三件套
来源：http://www.share.vehdjk.com/Article/details/guriepfvf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.bbcook.cn/Article/details/gooyrobkl.sHtML

[U59] PHP：自定义排序
来源：http://m.share.tarul.cn/Article/details/gszesljjc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/gtophsxhs.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.bbcook.cn/Article/details/gxnhevrpk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.sjlbkw.cn/Article/details/gruiomlkf.sHtML

[U61] PHP：正则
来源：http://m.share.epnwcf.com/Article/details/geptudlue.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/gngsserpx.sHtML

[U62] PHP：日期对象
来源：http://www.share.tarul.cn/Article/details/gsgdwdtef.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.sjlbkw.cn/Article/details/gjlosaubd.sHtML

[U63] PHP：文件读写
来源：http://blog.bbcook.cn/Article/details/gbhgybcux.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fktsv.cn/Article/details/gxregnhmt.sHtML

[U64] PHP：目录遍历
来源：http://blog.sjlbkw.cn/Article/details/guduonfif.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.vehdjk.com/Article/details/gwvgycfln.sHtML

[U65] PHP：会话
来源：http://www.share.vehdjk.com/Article/details/gnxewovbg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/givmdefnq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.tarul.cn/Article/details/gfickvwrc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.vehdjk.com/Article/details/ggqlcgsjj.sHtML

[U67] PHP：处理文件上传
来源：http://blog.vehdjk.com/Article/details/gstwyqxmr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.bbcook.cn/Article/details/grbwrlerq.sHtML

[U68] PHP：PDO 连接
来源：http://wap.bbcook.cn/Article/details/gzdttqjcw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.sjlbkw.cn/Article/details/ghmmhawqd.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.sjlbkw.cn/Article/details/gkhedqzyx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.vehdjk.com/Article/details/gssvpvcld.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.epnwcf.com/Article/details/gcancyigh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.yfazqb.com/Article/details/gnafvaltt.sHtML

[U71] PHP：抛出异常
来源：http://mobile.tarul.cn/Article/details/gcmtyvpni.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.tarul.cn/Article/details/gziejvoja.sHtML

[U72] PHP：写错误日志
来源：http://m.share.yfazqb.com/Article/details/grjhbtkqv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.tarul.cn/Article/details/gpjltuszr.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.tarul.cn/Article/details/gymdpqant.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.tarul.cn/Article/details/glvzkmdbe.sHtML

[U74] PHP：读取环境变量
来源：http://wap.epnwcf.com/Article/details/gkbbysevy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.tarul.cn/Article/details/gnbrdeort.sHtML

[U75] PHP：依赖注入
来源：http://3g.yfazqb.com/Article/details/ghwrmynyo.sHtML

composer require psr/container
来源：http://wap.vehdjk.com/Article/details/golqyeuin.sHtML

[U76] PHP：简单路由
来源：http://3g.fktsv.cn/Article/details/gkzvoxgmu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnqtobdl.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fktsv.cn/Article/details/gifpudvfh.sHtML

composer require twig/twig
来源：http://read.share.tarul.cn/Article/details/gvhwngxtp.sHtML

[U78] PHP：单元测试
来源：http://blog.sjlbkw.cn/Article/details/gcigdvuhm.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.bbcook.cn/Article/details/gusfnqwwm.sHtML

[U79] PHP：静态分析
来源：http://mobile.yfazqb.com/Article/details/ggxaefvwk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.yfazqb.com/Article/details/gxtvglmlx.sHtML

[U80] PHP：代码规范修复
来源：http://blog.tarul.cn/Article/details/geojeonte.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.sjlbkw.cn/Article/details/gjjluzgbj.sHtML

[U81] JS：初始化项目
来源：http://wap.fktsv.cn/Article/details/gnfjujthd.sHtML

npm init -y;  npm i express
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmhcdrsq.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.yfazqb.com/Article/details/gjhkpkfuw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.epnwcf.com/Article/details/ggiqizdsr.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.epnwcf.com/Article/details/gdhilhqtr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlrfivcy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.vehdjk.com/Article/details/gdpafxifo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.tarul.cn/Article/details/geujrqwxr.sHtML

[U85] JS：可选链
来源：http://blog.tarul.cn/Article/details/gsqqvyhrs.sHtML

a?.b?.c
来源：http://baike.tarul.cn/Article/details/gcehgnkwg.sHtML

[U86] JS：空值合并
来源：http://m.share.bbcook.cn/Article/details/gljuuixij.sHtML

a ?? b
来源：http://blog.bbcook.cn/Article/details/gthzxhcch.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fktsv.cn/Article/details/gphfkqhkg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.bbcook.cn/Article/details/gxhixjhvg.sHtML

[U88] JS：对象展开合并
来源：http://mobile.bbcook.cn/Article/details/goprgovqv.sHtML

{ ...a, ...b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvpuffsn.sHtML

[U89] JS：数组去重
来源：http://www.share.tarul.cn/Article/details/gjkswwlsj.sHtML

[...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/guovtnvhp.sHtML

[U90] JS：数字数组排序
来源：http://mobile.yfazqb.com/Article/details/gbvnlvppt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/ggtfaxmxz.sHtML

[U91] JS：对象键值遍历
来源：http://3g.vehdjk.com/Article/details/gewygaylj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.yfazqb.com/Article/details/gdrhmalvd.sHtML

[U92] JS：深拷贝
来源：http://baike.fktsv.cn/Article/details/gnpztxvkt.sHtML

structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gtgrlplbe.sHtML

[U93] JS：模板字符串
来源：http://m.share.tarul.cn/Article/details/gyncawljz.sHtML

`共 ${n} 条`
来源：http://baike.vehdjk.com/Article/details/gyteegxvy.sHtML

[U94] JS：箭头函数
来源：http://baike.vehdjk.com/Article/details/gidufypbp.sHtML

const double = x => x * 2;
来源：http://www.share.yfazqb.com/Article/details/gwgdmnfbv.sHtML

[U95] JS：Promise 包装
来源：http://blog.sjlbkw.cn/Article/details/gxiwgyfcn.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.vehdjk.com/Article/details/gwnskrarx.sHtML

[U96] JS：async/await 与异常
来源：http://3g.tarul.cn/Article/details/ghjpephae.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/guwuararr.sHtML

[U97] JS：并发请求
来源：http://m.share.tarul.cn/Article/details/gwjosspqk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gzetbszet.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.vehdjk.com/Article/details/gsulcsazo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.tarul.cn/Article/details/gtkrkaruv.sHtML

[U99] JS：事件监听
来源：http://www.m.share.tarul.cn/Article/details/gwsygdwur.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.bbcook.cn/Article/details/grhqsazyp.sHtML

[U100] JS：DOM 查询
来源：http://wap.vehdjk.com/Article/details/glsripngs.sHtML

document.querySelector(".item")
来源：http://3g.yfazqb.com/Article/details/grwpsfyks.sHtML

[U101] JS：classList 操作
来源：http://m.share.fktsv.cn/Article/details/gitfhxwmo.sHtML

el.classList.toggle("active")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkslmbkz.sHtML

[U102] JS：本地存储
来源：http://www.share.epnwcf.com/Article/details/ggtprnhop.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.sjlbkw.cn/Article/details/ghnxeievs.sHtML

[U103] JS：定时器
来源：http://www.m.share.bbcook.cn/Article/details/gpmbcutrb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.tarul.cn/Article/details/ghydhefzo.sHtML

[U104] JS：防抖
来源：http://read.share.fktsv.cn/Article/details/gbalbvnut.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gkgrmlemq.sHtML

[U105] JS：节流
来源：http://blog.yfazqb.com/Article/details/glnwmddvs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.yfazqb.com/Article/details/gkiovelro.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gwftyuxsd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.sjlbkw.cn/Article/details/gfribprzf.sHtML

[U107] JS：数字千分位
来源：http://3g.tarul.cn/Article/details/gtlxxorkt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/gpwocnjhl.sHtML

[U108] JS：随机整数
来源：http://m.share.epnwcf.com/Article/details/gisayweoj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.tarul.cn/Article/details/gpedaqwfy.sHtML

[U109] JS：数组分组
来源：http://www.share.fktsv.cn/Article/details/gsfcdrdbw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.tarul.cn/Article/details/gvbqatbce.sHtML

[U110] JS：数组分块
来源：http://mobile.sjlbkw.cn/Article/details/gupytplmu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.vehdjk.com/Article/details/grbyfzkor.sHtML

[U111] JS：对象转 Map
来源：http://blog.bbcook.cn/Article/details/gmcbojwel.sHtML

new Map(Object.entries(obj))
来源：http://www.share.yfazqb.com/Article/details/gvzqydnne.sHtML

[U112] JS：字符串补位
来源：http://read.share.tarul.cn/Article/details/gzixewzvx.sHtML

"7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gxxfsrlqn.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.yfazqb.com/Article/details/gnigfgsjn.sHtML

s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/ghmzembhs.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.bbcook.cn/Article/details/gwvhtguks.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/gwqsjzoje.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.sjlbkw.cn/Article/details/gusfmltgq.sHtML

crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gresoyjuk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.vehdjk.com/Article/details/ghzpofnwv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.tarul.cn/Article/details/guxfklgdp.sHtML

[U117] JS：单元测试
来源：http://mobile.sjlbkw.cn/Article/details/guzlmsbkd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fktsv.cn/Article/details/gguokdvrc.sHtML

[U118] JS：开发服务器
来源：http://baike.yfazqb.com/Article/details/gywyscmvd.sHtML

npm i -D vite;  npx vite
来源：http://m.share.vehdjk.com/Article/details/gemezvtlf.sHtML

[U119] JS：生产构建
来源：http://blog.vehdjk.com/Article/details/gxsdnfahm.sHtML

npx vite build
来源：http://www.m.share.fktsv.cn/Article/details/gywggxtln.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fktsv.cn/Article/details/ggwqrwpil.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fktsv.cn/Article/details/gztsswxkn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gucshslrb.sHtML

统计汇总
来源：http://wap.tarul.cn/Article/details/ghjwuugax.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gsqkoqxft.sHtML

按语言统计（条）：
来源：http://www.m.share.yfazqb.com/Article/details/giznnehkk.sHtML

Python ......... 252
来源：http://www.blog.yfazqb.com/Article/details/gcvrskedw.sHtML

PHP ............ 252
来源：http://mobile.vehdjk.com/Article/details/gqqjpktfc.sHtML

JavaScript ..... 252
来源：http://www.blog.yfazqb.com/Article/details/gokrfunya.sHtML

TypeScript ..... 212
来源：http://blog.fktsv.cn/Article/details/ghlajylqx.sHtML

Java ........... 212
来源：http://www.blog.fktsv.cn/Article/details/gnfbsltik.sHtML

Go ............. 212
来源：http://wap.fktsv.cn/Article/details/gkcjegjun.sHtML

Ruby ........... 212
来源：http://baike.yfazqb.com/Article/details/gvtnqjopb.sHtML

C# ............. 212
来源：http://3g.sjlbkw.cn/Article/details/gedmchevk.sHtML

C .............. 30
来源：http://baike.yfazqb.com/Article/details/gqquhzdlz.sHtML

C++ ............ 30
来源：http://3g.bbcook.cn/Article/details/gdihmulgq.sHtML

SQL ............ 90
来源：http://wap.fktsv.cn/Article/details/gydyloyah.sHtML

Bash ........... 80
来源：http://www.share.sjlbkw.cn/Article/details/gysiougrp.sHtML

Kotlin ......... 15
来源：http://blog.vehdjk.com/Article/details/gokztrkot.sHtML

Swift .......... 15
来源：http://3g.tarul.cn/Article/details/gtaxizxyi.sHtML

Lua ............ 10
来源：http://baike.tarul.cn/Article/details/gpvjzwqrz.sHtML

Perl ........... 10
来源：http://baike.vehdjk.com/Article/details/gnenilnzt.sHtML

Scala .......... 10
来源：http://read.share.sjlbkw.cn/Article/details/ghutbdswu.sHtML

------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gsytnulmm.sHtML

合计 ........... 2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/grnnmttrt.sHtML

按章节统计：
来源：http://www.blog.vehdjk.com/Article/details/glyafdfyk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fktsv.cn/Article/details/gswebddyr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/gcywcbfsv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/gpizyabxw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.sjlbkw.cn/Article/details/gbytlgqdx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.tarul.cn/Article/details/gjmrqyrch.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/gtjtqmwwx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.epnwcf.com/Article/details/gxypzwciw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.tarul.cn/Article/details/gqdxoxypt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gfimaasgq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.epnwcf.com/Article/details/gubbcqmpx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gresqjuzr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gqxezqjek.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gzwkalhkl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.bbcook.cn/Article/details/gveunrmgc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.bbcook.cn/Article/details/gtiirgoas.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gvqhgwtbj.sHtML

Q SQL 专题                              90
来源：http://baike.sjlbkw.cn/Article/details/gsihxecme.sHtML

R Bash 专题                             80
来源：http://3g.vehdjk.com/Article/details/gqogaoaow.sHtML

S C / C++ 专题                          60
来源：http://www.share.yfazqb.com/Article/details/gfvxtcuty.sHtML

T 其他语言补充                          60
来源：http://wap.tarul.cn/Article/details/gnpgiymbx.sHtML


<!-- 参考信息 -->