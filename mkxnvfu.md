代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gpftghewm.sHtML

[T55] Scala：集合过滤
来源：http://wap.epnwcf.com/Article/details/gzsojplkt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.bbcook.cn/Article/details/gnohsylvh.sHtML

[T56] Scala：样例类
来源：http://blog.vehdjk.com/Article/details/gjbuoqqjm.sHtML

case class User(name: String, age: Int)
来源：http://www.share.bbcook.cn/Article/details/gtsripvez.sHtML

[T57] Scala：模式匹配
来源：http://wap.tarul.cn/Article/details/gsvwvfcdt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fktsv.cn/Article/details/gebmsegel.sHtML

[T58] Scala：函数定义
来源：http://www.share.yfazqb.com/Article/details/gumigxmhe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.vehdjk.com/Article/details/gwatkpnao.sHtML

[T59] Scala：循环
来源：http://baike.epnwcf.com/Article/details/ggmkkdjrk.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.tarul.cn/Article/details/gfqmczhpo.sHtML

[T60] Scala：折叠
来源：http://www.m.share.bbcook.cn/Article/details/gigcrhzpr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.bbcook.cn/Article/details/gbgaytglg.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfbjjohvh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.epnwcf.com/Article/details/gjqobtdkv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/guwwhtdef.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.vehdjk.com/Article/details/gvlgmcqrd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.epnwcf.com/Article/details/gcsyanufu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.epnwcf.com/Article/details/goyezaczv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.vehdjk.com/Article/details/gsuauxeky.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.epnwcf.com/Article/details/glqvwcvje.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.epnwcf.com/Article/details/gekzateju.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.epnwcf.com/Article/details/gyxdilvva.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/guuqzmggl.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.tarul.cn/Article/details/gwsotqlkg.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gamxfztiu.sHtML

[U06] Py：合并两个字典
来源：http://3g.tarul.cn/Article/details/gzlaldhkf.sHtML

{**a, **b}
来源：http://www.m.share.yfazqb.com/Article/details/gurgjvviy.sHtML

[U07] Py：反转字典键值
来源：http://wap.epnwcf.com/Article/details/gwruzhtja.sHtML

{v: k for k, v in d.items()}
来源：http://blog.epnwcf.com/Article/details/grcsoobyd.sHtML

[U08] Py：展平二维列表
来源：http://mobile.yfazqb.com/Article/details/govyyvilj.sHtML

[y for x in nested for y in x]
来源：http://read.share.fktsv.cn/Article/details/gurgrrrpe.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fktsv.cn/Article/details/grjlqsdzu.sHtML

max(d, key=d.get)
来源：http://baike.fktsv.cn/Article/details/guhvmhmzx.sHtML

[U10] Py：按值排序字典
来源：http://baike.tarul.cn/Article/details/gfygxcqtb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.bbcook.cn/Article/details/gckfuszam.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.epnwcf.com/Article/details/ggbkonmdu.sHtML

(x * 2 for x in arr)
来源：http://www.share.bbcook.cn/Article/details/gfwxjmprw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.sjlbkw.cn/Article/details/glrdaqozg.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fktsv.cn/Article/details/gbentcmqw.sHtML

[U13] Py：固定长度队列
来源：http://blog.sjlbkw.cn/Article/details/gnloeanop.sHtML

deque(maxlen=10)
来源：http://www.share.fktsv.cn/Article/details/gznqruyro.sHtML

[U14] Py：分组收集到列表
来源：http://wap.tarul.cn/Article/details/gwtigwlwg.sHtML

defaultdict(list)
来源：http://baike.yfazqb.com/Article/details/gavlriaxt.sHtML

[U15] Py：高精度计时
来源：http://read.share.bbcook.cn/Article/details/gopgwdsxb.sHtML

t = time.perf_counter()
来源：http://wap.bbcook.cn/Article/details/gmcxeixiz.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.vehdjk.com/Article/details/ggkkjvkde.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.yfazqb.com/Article/details/gyjqmguwq.sHtML

[U17] Py：初始化日志
来源：http://www.blog.bbcook.cn/Article/details/gmhhzqnwk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.yfazqb.com/Article/details/gqnpdmsxd.sHtML

[U18] Py：预编译正则
来源：http://www.share.sjlbkw.cn/Article/details/gtarhguzz.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/glcmnbhli.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fktsv.cn/Article/details/gtbwbsiuz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.vehdjk.com/Article/details/gzyqojkhk.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.vehdjk.com/Article/details/gifzafstp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.vehdjk.com/Article/details/gifcthvor.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.sjlbkw.cn/Article/details/gyonnnwhg.sHtML

@contextlib.contextmanager
来源：http://blog.yfazqb.com/Article/details/giyojnqhb.sHtML

[U22] Py：矩阵转置
来源：http://www.share.tarul.cn/Article/details/gghtpetyj.sHtML

list(zip(*m))
来源：http://m.share.yfazqb.com/Article/details/glbkbvdjw.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gekbvxjzo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fktsv.cn/Article/details/gdcymjkaf.sHtML

[U24] Py：路径操作
来源：http://m.share.sjlbkw.cn/Article/details/gyeocdpsy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gnlkofiqg.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/grthukefi.sHtML

csv.DictReader(f)
来源：http://m.share.bbcook.cn/Article/details/gdbdzhrpw.sHtML

[U26] Py：并发下载
来源：http://baike.fktsv.cn/Article/details/geicnwuhf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.tarul.cn/Article/details/gcstnhnzq.sHtML

[U27] Py：异步 HTTP
来源：http://3g.epnwcf.com/Article/details/ggiajnzmh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.epnwcf.com/Article/details/gijanejrb.sHtML

[U28] Py：类型别名
来源：http://www.m.share.epnwcf.com/Article/details/ggqiwmhwx.sHtML

UserId = int
来源：http://mobile.fktsv.cn/Article/details/gunnsvypt.sHtML

[U29] Py：属性校验
来源：http://baike.yfazqb.com/Article/details/giwrmxyjj.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fktsv.cn/Article/details/gchqnakhi.sHtML

[U30] Py：数据类
来源：http://www.share.epnwcf.com/Article/details/gsyifruqj.sHtML

@dataclass(slots=True)
来源：http://www.m.share.vehdjk.com/Article/details/gkuhzoewu.sHtML

[U31] Py：单测
来源：http://read.share.fktsv.cn/Article/details/gjrnmcxzj.sHtML

python -m pytest -q
来源：http://mobile.bbcook.cn/Article/details/gfplqupbi.sHtML

[U32] Py：代码格式化
来源：http://m.share.tarul.cn/Article/details/gyrttfkdh.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.bbcook.cn/Article/details/gjxybnfgf.sHtML

[U33] Py：打包发布
来源：http://blog.epnwcf.com/Article/details/gjighamlq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.tarul.cn/Article/details/gpaohremv.sHtML

[U34] Py：判断编码
来源：http://blog.fktsv.cn/Article/details/gdbrvpqmu.sHtML

chardet.detect(raw)
来源：http://baike.bbcook.cn/Article/details/gwboveqhe.sHtML

[U35] Py：发送邮件
来源：http://read.share.epnwcf.com/Article/details/gwbgfppbw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.sjlbkw.cn/Article/details/gukwjhcsl.sHtML

[U36] Py：定时任务
来源：http://3g.fktsv.cn/Article/details/gxvxitgqf.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.epnwcf.com/Article/details/gvkyjfxzu.sHtML

[U37] Py：读写 Excel
来源：http://mobile.tarul.cn/Article/details/guiaxztjb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.epnwcf.com/Article/details/gpvetemfu.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.bbcook.cn/Article/details/gxqigxuce.sHtML

Path(__file__).resolve().parent
来源：http://wap.sjlbkw.cn/Article/details/gqwmjkrwc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.vehdjk.com/Article/details/gwtdahwbm.sHtML

sys.stdout.isatty()
来源：http://wap.fktsv.cn/Article/details/gushyaygr.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.vehdjk.com/Article/details/gsluidtzd.sHtML

print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/geakgblhw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.vehdjk.com/Article/details/gndpijdbc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.vehdjk.com/Article/details/gehsxuzbj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fktsv.cn/Article/details/ggshzedhw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.sjlbkw.cn/Article/details/gybmvwgmb.sHtML

[U43] PHP：声明命名空间
来源：http://baike.sjlbkw.cn/Article/details/ganrdocho.sHtML

namespace App\Http;
来源：http://wap.fktsv.cn/Article/details/gegwrdked.sHtML

[U44] PHP：开启严格类型
来源：http://3g.yfazqb.com/Article/details/gwdiqogse.sHtML

declare(strict_types=1);
来源：http://read.share.tarul.cn/Article/details/gavtqmhnc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fktsv.cn/Article/details/gxljcdjwk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gnvpsuqrl.sHtML

[U46] PHP：可空类型
来源：http://www.blog.yfazqb.com/Article/details/gotswgwkm.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/ggbbyxosa.sHtML

[U47] PHP：联合类型
来源：http://wap.bbcook.cn/Article/details/gwsyanxot.sHtML

int|string $id
来源：http://3g.sjlbkw.cn/Article/details/ggzgceetf.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.yfazqb.com/Article/details/gaqthfprs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.epnwcf.com/Article/details/glskachbn.sHtML

[U49] PHP：只读属性
来源：http://wap.vehdjk.com/Article/details/gnaeuqoyb.sHtML

public readonly string $name
来源：http://mobile.epnwcf.com/Article/details/genlkbird.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fktsv.cn/Article/details/glabecydq.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.yfazqb.com/Article/details/gxzksahwo.sHtML

[U51] PHP：数组解构
来源：http://mobile.sjlbkw.cn/Article/details/gpktiaify.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/ghscedrml.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.yfazqb.com/Article/details/guhsrimwa.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.sjlbkw.cn/Article/details/gkgrlagnc.sHtML

[U53] PHP：空合并运算符
来源：http://baike.tarul.cn/Article/details/glehijull.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.vehdjk.com/Article/details/gyokjxlfd.sHtML

[U54] PHP：空安全调用
来源：http://baike.sjlbkw.cn/Article/details/gxshprbqq.sHtML

$obj?->method()
来源：http://3g.bbcook.cn/Article/details/gnptyawvl.sHtML

[U55] PHP：match 表达式
来源：http://3g.sjlbkw.cn/Article/details/gdqtyecsz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.yfazqb.com/Article/details/gdyqfymme.sHtML

[U56] PHP：命名参数
来源：http://wap.tarul.cn/Article/details/grwezjqvy.sHtML

f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gttvqpsrf.sHtML

[U57] PHP：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gkxrwxyoz.sHtML

"值: {$a}"
来源：http://m.share.bbcook.cn/Article/details/gjqwqijxe.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.epnwcf.com/Article/details/gynwjlkuh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gsydtqrij.sHtML

[U59] PHP：自定义排序
来源：http://wap.tarul.cn/Article/details/gikxjtdsd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gmtmijpus.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.yfazqb.com/Article/details/gvfacqoyj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fktsv.cn/Article/details/gsdnhhgpt.sHtML

[U61] PHP：正则
来源：http://m.share.tarul.cn/Article/details/givhxhcyq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.yfazqb.com/Article/details/gbcaxcgzo.sHtML

[U62] PHP：日期对象
来源：http://3g.fktsv.cn/Article/details/gwtxgyenm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fktsv.cn/Article/details/gyjpxhpub.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fktsv.cn/Article/details/gdzexstvo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fktsv.cn/Article/details/gccuvdpfl.sHtML

[U64] PHP：目录遍历
来源：http://blog.sjlbkw.cn/Article/details/gyngwvjoh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.bbcook.cn/Article/details/gzalldoav.sHtML

[U65] PHP：会话
来源：http://baike.bbcook.cn/Article/details/gohyusjba.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.epnwcf.com/Article/details/ghanlztrd.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.bbcook.cn/Article/details/ghacijish.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.yfazqb.com/Article/details/gmalhpwfb.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.epnwcf.com/Article/details/gobxbiymj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.yfazqb.com/Article/details/greesapws.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.tarul.cn/Article/details/gjzqkeasr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fktsv.cn/Article/details/gfxqwxysc.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.sjlbkw.cn/Article/details/gihtwuduo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fktsv.cn/Article/details/gsvdxkyfd.sHtML

[U70] PHP：PDO 事务
来源：http://3g.bbcook.cn/Article/details/gyhvzrhzs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fktsv.cn/Article/details/gxfhqnfnr.sHtML

[U71] PHP：抛出异常
来源：http://baike.tarul.cn/Article/details/ggehawhiy.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.yfazqb.com/Article/details/ggadetabx.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.yfazqb.com/Article/details/geojgfydv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.tarul.cn/Article/details/gxerkqaci.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.vehdjk.com/Article/details/groypfoge.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.yfazqb.com/Article/details/ghguidbtb.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gbvvwrdev.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.epnwcf.com/Article/details/gnsogtztt.sHtML

[U75] PHP：依赖注入
来源：http://wap.yfazqb.com/Article/details/gxknxghig.sHtML

composer require psr/container
来源：http://blog.epnwcf.com/Article/details/gxnhdxkyl.sHtML

[U76] PHP：简单路由
来源：http://www.blog.epnwcf.com/Article/details/gycxqzrlk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.epnwcf.com/Article/details/gwrlexdlv.sHtML

[U77] PHP：模板渲染
来源：http://mobile.vehdjk.com/Article/details/gilslfhhv.sHtML

composer require twig/twig
来源：http://www.blog.fktsv.cn/Article/details/gotbxatdh.sHtML

[U78] PHP：单元测试
来源：http://baike.vehdjk.com/Article/details/gygpturym.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.tarul.cn/Article/details/gacqxxpxo.sHtML

[U79] PHP：静态分析
来源：http://3g.tarul.cn/Article/details/ggbeesaqz.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.vehdjk.com/Article/details/ggbefuiuo.sHtML

[U80] PHP：代码规范修复
来源：http://blog.tarul.cn/Article/details/gdctnkhfp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fktsv.cn/Article/details/gnrwyuaaj.sHtML

[U81] JS：初始化项目
来源：http://blog.epnwcf.com/Article/details/gyspjupfm.sHtML

npm init -y;  npm i express
来源：http://read.share.yfazqb.com/Article/details/gwofxefok.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.bbcook.cn/Article/details/gqcxjkiem.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fktsv.cn/Article/details/gfvqoojua.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fktsv.cn/Article/details/gnmkexafx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gaxnoxrzh.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.yfazqb.com/Article/details/gfwafgeia.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.yfazqb.com/Article/details/gyyakslxm.sHtML

[U85] JS：可选链
来源：http://m.share.vehdjk.com/Article/details/gnwvrkbad.sHtML

a?.b?.c
来源：http://www.blog.fktsv.cn/Article/details/gxoopepqc.sHtML

[U86] JS：空值合并
来源：http://3g.epnwcf.com/Article/details/gmqvantsq.sHtML

a ?? b
来源：http://www.m.share.epnwcf.com/Article/details/gdbbjcnrl.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.bbcook.cn/Article/details/gxwqixzxt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.tarul.cn/Article/details/gdagyjufp.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.yfazqb.com/Article/details/gmjipvcqv.sHtML

{ ...a, ...b }
来源：http://mobile.bbcook.cn/Article/details/givgvhiyj.sHtML

[U89] JS：数组去重
来源：http://wap.yfazqb.com/Article/details/grskgbviu.sHtML

[...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gfztvbzyu.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.vehdjk.com/Article/details/gsyudhruq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gobhpxrva.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.sjlbkw.cn/Article/details/gzatafplg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.bbcook.cn/Article/details/gvomicndt.sHtML

[U92] JS：深拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gcngmlzyg.sHtML

structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gplmtvjsk.sHtML

[U93] JS：模板字符串
来源：http://mobile.vehdjk.com/Article/details/gllzzbixf.sHtML

`共 ${n} 条`
来源：http://mobile.tarul.cn/Article/details/gzmohrfoc.sHtML

[U94] JS：箭头函数
来源：http://read.share.yfazqb.com/Article/details/gornjdbzt.sHtML

const double = x => x * 2;
来源：http://wap.epnwcf.com/Article/details/gkfwxkgna.sHtML

[U95] JS：Promise 包装
来源：http://3g.yfazqb.com/Article/details/gkbhcuvbi.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.bbcook.cn/Article/details/gzbbhrivs.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fktsv.cn/Article/details/gmnyjkqyu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gmhxpvotx.sHtML

[U97] JS：并发请求
来源：http://wap.yfazqb.com/Article/details/gvyqswpbb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gjuumpjly.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.yfazqb.com/Article/details/gjgrtvvgk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.bbcook.cn/Article/details/gpzhyixzv.sHtML

[U99] JS：事件监听
来源：http://wap.fktsv.cn/Article/details/gsevgctxe.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fktsv.cn/Article/details/geztddcve.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.vehdjk.com/Article/details/grhagwgpm.sHtML

document.querySelector(".item")
来源：http://3g.vehdjk.com/Article/details/gxskhprdq.sHtML

[U101] JS：classList 操作
来源：http://mobile.fktsv.cn/Article/details/glfewhilq.sHtML

el.classList.toggle("active")
来源：http://www.blog.epnwcf.com/Article/details/gfilhrein.sHtML

[U102] JS：本地存储
来源：http://www.share.vehdjk.com/Article/details/gavkekkgj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.tarul.cn/Article/details/gzmbulszm.sHtML

[U103] JS：定时器
来源：http://wap.fktsv.cn/Article/details/gikeytypp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.bbcook.cn/Article/details/gpjodkniy.sHtML

[U104] JS：防抖
来源：http://baike.sjlbkw.cn/Article/details/gfcjiiegr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gppkgmbbh.sHtML

[U105] JS：节流
来源：http://wap.bbcook.cn/Article/details/gddmenccf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fktsv.cn/Article/details/gpusdttrl.sHtML

[U106] JS：日期格式化
来源：http://baike.yfazqb.com/Article/details/glxtqmwaj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.epnwcf.com/Article/details/grqiiwlia.sHtML

[U107] JS：数字千分位
来源：http://www.share.yfazqb.com/Article/details/gbjkujphl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.tarul.cn/Article/details/gibtkfbfe.sHtML

[U108] JS：随机整数
来源：http://m.share.bbcook.cn/Article/details/geoffvwjp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.sjlbkw.cn/Article/details/gpdzfjzet.sHtML

[U109] JS：数组分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmwtkxby.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.epnwcf.com/Article/details/gllpszyuh.sHtML

[U110] JS：数组分块
来源：http://3g.epnwcf.com/Article/details/gptdwkcmh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.epnwcf.com/Article/details/gtjorelxd.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.yfazqb.com/Article/details/gllabgmrl.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.epnwcf.com/Article/details/gczkkohrn.sHtML

[U112] JS：字符串补位
来源：http://mobile.yfazqb.com/Article/details/gdcayarvd.sHtML

"7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gpqemkpfq.sHtML

[U113] JS：正则替换全部
来源：http://m.share.epnwcf.com/Article/details/gkshujkrr.sHtML

s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gmqknrsmf.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.tarul.cn/Article/details/grcfqpynh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.bbcook.cn/Article/details/gvjqfuate.sHtML

[U115] JS：生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gleghngyj.sHtML

crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gqdocryce.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbobjbkqi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.yfazqb.com/Article/details/gtfymmxct.sHtML

[U117] JS：单元测试
来源：http://baike.vehdjk.com/Article/details/gpbbpxvfx.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.yfazqb.com/Article/details/gckzbkoik.sHtML

[U118] JS：开发服务器
来源：http://mobile.epnwcf.com/Article/details/gezeulmqk.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.yfazqb.com/Article/details/gefictibm.sHtML

[U119] JS：生产构建
来源：http://baike.sjlbkw.cn/Article/details/gzikukxgz.sHtML

npx vite build
来源：http://www.share.tarul.cn/Article/details/gmekbkdnm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.epnwcf.com/Article/details/gqiydvzre.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.vehdjk.com/Article/details/gyycafjsw.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glnmlozzz.sHtML

统计汇总
来源：http://www.blog.sjlbkw.cn/Article/details/guwgbifyl.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gxdauqvkr.sHtML

按语言统计（条）：
来源：http://www.m.share.tarul.cn/Article/details/guiwcygny.sHtML

Python ......... 252
来源：http://www.m.share.yfazqb.com/Article/details/gnzagtxow.sHtML

PHP ............ 252
来源：http://www.share.sjlbkw.cn/Article/details/ghordcixv.sHtML

JavaScript ..... 252
来源：http://www.m.share.tarul.cn/Article/details/grfjalceo.sHtML

TypeScript ..... 212
来源：http://3g.tarul.cn/Article/details/gszhwjpml.sHtML

Java ........... 212
来源：http://www.m.share.yfazqb.com/Article/details/gkheuygvj.sHtML

Go ............. 212
来源：http://read.share.vehdjk.com/Article/details/ggwrzoozw.sHtML

Ruby ........... 212
来源：http://mobile.bbcook.cn/Article/details/ggnginari.sHtML

C# ............. 212
来源：http://www.blog.vehdjk.com/Article/details/gpsrzhiqj.sHtML

C .............. 30
来源：http://www.blog.sjlbkw.cn/Article/details/guzmkpque.sHtML

C++ ............ 30
来源：http://mobile.yfazqb.com/Article/details/ghtefuuqe.sHtML

SQL ............ 90
来源：http://m.share.fktsv.cn/Article/details/gvcvknzpa.sHtML

Bash ........... 80
来源：http://m.share.fktsv.cn/Article/details/gkvfruqqi.sHtML

Kotlin ......... 15
来源：http://mobile.epnwcf.com/Article/details/gnohehqed.sHtML

Swift .......... 15
来源：http://mobile.sjlbkw.cn/Article/details/gmuiobehh.sHtML

Lua ............ 10
来源：http://wap.sjlbkw.cn/Article/details/gzgddaxia.sHtML

Perl ........... 10
来源：http://wap.fktsv.cn/Article/details/gvrorftfq.sHtML

Scala .......... 10
来源：http://www.blog.sjlbkw.cn/Article/details/gmuworktz.sHtML

------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gmavqblah.sHtML

合计 ........... 2106 条
来源：http://wap.bbcook.cn/Article/details/gnhlxthjf.sHtML

按章节统计：
来源：http://www.share.tarul.cn/Article/details/gtwqfnplm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.vehdjk.com/Article/details/gievgtzhb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gjtlpvxpe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.epnwcf.com/Article/details/ggqiksfkw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.tarul.cn/Article/details/gpquiflhz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.epnwcf.com/Article/details/gqlelnydy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.yfazqb.com/Article/details/guffdrkyt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gmvktfszk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.vehdjk.com/Article/details/gpbkrsqrr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gyfcxpzuu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.sjlbkw.cn/Article/details/gyzvopfqc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gxftnvotp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/grkglyahj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gusgdnmok.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.vehdjk.com/Article/details/giizrwpmc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.bbcook.cn/Article/details/gdbxkphty.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gtimhfgoi.sHtML

Q SQL 专题                              90
来源：http://baike.vehdjk.com/Article/details/giibdvfdb.sHtML

R Bash 专题                             80
来源：http://mobile.bbcook.cn/Article/details/gqftxfqgf.sHtML

S C / C++ 专题                          60
来源：http://3g.bbcook.cn/Article/details/ghulqmtsh.sHtML

T 其他语言补充                          60
来源：http://baike.fktsv.cn/Article/details/gpmpbccqk.sHtML


<!-- 参考信息 -->