代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.epnwcf.com/Article/details/gftmjyain.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fktsv.cn/Article/details/gztpznspc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.epnwcf.com/Article/details/gjbtosrxw.sHtML

[T56] Scala：样例类
来源：http://baike.tarul.cn/Article/details/gjpwdwbio.sHtML

case class User(name: String, age: Int)
来源：http://www.share.yfazqb.com/Article/details/gwqyctjyt.sHtML

[T57] Scala：模式匹配
来源：http://m.share.epnwcf.com/Article/details/gwetxlqpl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.tarul.cn/Article/details/gxjvilhds.sHtML

[T58] Scala：函数定义
来源：http://www.share.fktsv.cn/Article/details/gwikjewby.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.sjlbkw.cn/Article/details/gwtdqboof.sHtML

[T59] Scala：循环
来源：http://m.share.fktsv.cn/Article/details/gvtuyytrh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gjxrfjxfq.sHtML

[T60] Scala：折叠
来源：http://www.share.vehdjk.com/Article/details/gfmxirtbg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.tarul.cn/Article/details/ggosngabq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbwbwhyeb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/gbuqythys.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gptohaazf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.epnwcf.com/Article/details/gerxbtpqx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.bbcook.cn/Article/details/grlzekmnc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.tarul.cn/Article/details/grrnowata.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.yfazqb.com/Article/details/gebvilekz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.yfazqb.com/Article/details/gcrvqhqnz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.epnwcf.com/Article/details/gcepuavja.sHtML

[U04] Py：变量调试打印
来源：http://blog.epnwcf.com/Article/details/gzisdesda.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.epnwcf.com/Article/details/grdhmsxwt.sHtML

[U05] Py：列表去重且保序
来源：http://wap.vehdjk.com/Article/details/gavxtcqlo.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gdzpmrlgk.sHtML

[U06] Py：合并两个字典
来源：http://baike.bbcook.cn/Article/details/gryqcsyss.sHtML

{**a, **b}
来源：http://baike.yfazqb.com/Article/details/gneublaqa.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.bbcook.cn/Article/details/gnazuoilk.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fktsv.cn/Article/details/gvcmtdkfp.sHtML

[U08] Py：展平二维列表
来源：http://m.share.tarul.cn/Article/details/guajmpnta.sHtML

[y for x in nested for y in x]
来源：http://read.share.epnwcf.com/Article/details/gkibvbwxl.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.vehdjk.com/Article/details/gyivuhdej.sHtML

max(d, key=d.get)
来源：http://3g.vehdjk.com/Article/details/gbidiqwbz.sHtML

[U10] Py：按值排序字典
来源：http://wap.vehdjk.com/Article/details/gzzxtixvp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.vehdjk.com/Article/details/gtaljozks.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.yfazqb.com/Article/details/gkgvvtchj.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.vehdjk.com/Article/details/gfnxnzbac.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.yfazqb.com/Article/details/gnlmemyox.sHtML

Counter(arr).most_common(3)
来源：http://read.share.tarul.cn/Article/details/gfxuailte.sHtML

[U13] Py：固定长度队列
来源：http://mobile.bbcook.cn/Article/details/gzbopbdeb.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/gxzctbexo.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.epnwcf.com/Article/details/gbmatnfrb.sHtML

defaultdict(list)
来源：http://read.share.bbcook.cn/Article/details/gyfufncxj.sHtML

[U15] Py：高精度计时
来源：http://mobile.sjlbkw.cn/Article/details/ghsmymmuo.sHtML

t = time.perf_counter()
来源：http://3g.fktsv.cn/Article/details/gaqprsrhr.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.tarul.cn/Article/details/gsrcjdhml.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.bbcook.cn/Article/details/gatraubgd.sHtML

[U17] Py：初始化日志
来源：http://read.share.bbcook.cn/Article/details/gexnglhyh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fktsv.cn/Article/details/gdcnivsur.sHtML

[U18] Py：预编译正则
来源：http://m.share.fktsv.cn/Article/details/ghwsameak.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.epnwcf.com/Article/details/gqnlxoxqw.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fktsv.cn/Article/details/gtsmscibt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.epnwcf.com/Article/details/gzoirwwyg.sHtML

[U20] Py：缓存函数结果
来源：http://blog.sjlbkw.cn/Article/details/ghgmmoofb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.bbcook.cn/Article/details/gybsqvzgq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.tarul.cn/Article/details/grbzqlxqt.sHtML

@contextlib.contextmanager
来源：http://wap.fktsv.cn/Article/details/galwjdhff.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.sjlbkw.cn/Article/details/ggsmbcdff.sHtML

list(zip(*m))
来源：http://read.share.bbcook.cn/Article/details/gxufbnrba.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.tarul.cn/Article/details/gjotbwweb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.tarul.cn/Article/details/gnlkkuysi.sHtML

[U24] Py：路径操作
来源：http://blog.epnwcf.com/Article/details/gvzweqkcg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.vehdjk.com/Article/details/gycjvqrfq.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.vehdjk.com/Article/details/gciwfsqfn.sHtML

csv.DictReader(f)
来源：http://blog.epnwcf.com/Article/details/gyzlcvace.sHtML

[U26] Py：并发下载
来源：http://www.m.share.yfazqb.com/Article/details/gxvczcjlu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.sjlbkw.cn/Article/details/gewiirmrc.sHtML

[U27] Py：异步 HTTP
来源：http://blog.tarul.cn/Article/details/gemenwthz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.yfazqb.com/Article/details/gtimymjii.sHtML

[U28] Py：类型别名
来源：http://mobile.fktsv.cn/Article/details/gmlswhpou.sHtML

UserId = int
来源：http://www.share.yfazqb.com/Article/details/gowyvdjpj.sHtML

[U29] Py：属性校验
来源：http://mobile.sjlbkw.cn/Article/details/gpozylgim.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gwjuualyf.sHtML

[U30] Py：数据类
来源：http://3g.fktsv.cn/Article/details/geuddiizw.sHtML

@dataclass(slots=True)
来源：http://3g.tarul.cn/Article/details/glzeicfyo.sHtML

[U31] Py：单测
来源：http://wap.bbcook.cn/Article/details/gcujzzyif.sHtML

python -m pytest -q
来源：http://www.share.yfazqb.com/Article/details/gdberjrex.sHtML

[U32] Py：代码格式化
来源：http://mobile.bbcook.cn/Article/details/gdfszqbpn.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.sjlbkw.cn/Article/details/glmjxzmrb.sHtML

[U33] Py：打包发布
来源：http://mobile.epnwcf.com/Article/details/gdooryosj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fktsv.cn/Article/details/geeqnmfhb.sHtML

[U34] Py：判断编码
来源：http://www.m.share.yfazqb.com/Article/details/gkifjpkan.sHtML

chardet.detect(raw)
来源：http://mobile.tarul.cn/Article/details/girxqgpjq.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fktsv.cn/Article/details/gzkbufmir.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.vehdjk.com/Article/details/gphobbqeu.sHtML

[U36] Py：定时任务
来源：http://m.share.yfazqb.com/Article/details/gogadijlm.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.vehdjk.com/Article/details/glwfhxkem.sHtML

[U37] Py：读写 Excel
来源：http://wap.epnwcf.com/Article/details/geypxnsfa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.epnwcf.com/Article/details/gmucznysl.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fktsv.cn/Article/details/gsxrflcwa.sHtML

Path(__file__).resolve().parent
来源：http://wap.fktsv.cn/Article/details/gmiiqfqwf.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.vehdjk.com/Article/details/gwindgrmt.sHtML

sys.stdout.isatty()
来源：http://baike.bbcook.cn/Article/details/gzmubytre.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fktsv.cn/Article/details/gfkofjkcs.sHtML

print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gwedptufx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.sjlbkw.cn/Article/details/guwehwgir.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.vehdjk.com/Article/details/ggplradek.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.bbcook.cn/Article/details/gisktauwg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.sjlbkw.cn/Article/details/gvosyikhf.sHtML

[U43] PHP：声明命名空间
来源：http://blog.sjlbkw.cn/Article/details/gcbhartzp.sHtML

namespace App\Http;
来源：http://www.blog.bbcook.cn/Article/details/gsuvgqutj.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.tarul.cn/Article/details/gapdoidbg.sHtML

declare(strict_types=1);
来源：http://wap.tarul.cn/Article/details/gympnwsco.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.epnwcf.com/Article/details/gkclfkswu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gmgkcmyju.sHtML

[U46] PHP：可空类型
来源：http://3g.sjlbkw.cn/Article/details/gaqkzgecl.sHtML

?string $name = null
来源：http://www.share.epnwcf.com/Article/details/gwwpqbocv.sHtML

[U47] PHP：联合类型
来源：http://wap.epnwcf.com/Article/details/gvskawksu.sHtML

int|string $id
来源：http://www.m.share.yfazqb.com/Article/details/gpknzfaci.sHtML

[U48] PHP：纯枚举
来源：http://baike.bbcook.cn/Article/details/gtsmpzvzc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.epnwcf.com/Article/details/getaateqm.sHtML

[U49] PHP：只读属性
来源：http://wap.tarul.cn/Article/details/goyfivbyq.sHtML

public readonly string $name
来源：http://blog.tarul.cn/Article/details/gebihsbsj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.vehdjk.com/Article/details/gonxlepem.sHtML

public function __construct(private int $id) {}
来源：http://3g.epnwcf.com/Article/details/gcxayclic.sHtML

[U51] PHP：数组解构
来源：http://read.share.bbcook.cn/Article/details/gwmfpmcon.sHtML

[$a, $b] = $arr;
来源：http://mobile.fktsv.cn/Article/details/gmikkixri.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.epnwcf.com/Article/details/giahdhkec.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.yfazqb.com/Article/details/gndbnjppb.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.yfazqb.com/Article/details/gcnykfcva.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.tarul.cn/Article/details/gakiafxvz.sHtML

[U54] PHP：空安全调用
来源：http://blog.tarul.cn/Article/details/gvghzpwki.sHtML

$obj?->method()
来源：http://mobile.epnwcf.com/Article/details/gyrrpcccs.sHtML

[U55] PHP：match 表达式
来源：http://read.share.yfazqb.com/Article/details/gjfnmeugh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/gufcldtbg.sHtML

[U56] PHP：命名参数
来源：http://www.share.epnwcf.com/Article/details/gfiqshwxp.sHtML

f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gmnqjmjzx.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gnozenoly.sHtML

"值: {$a}"
来源：http://baike.bbcook.cn/Article/details/gpgcndorx.sHtML

[U58] PHP：数组三件套
来源：http://mobile.epnwcf.com/Article/details/gminfpcct.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.tarul.cn/Article/details/grgmgqqpq.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fktsv.cn/Article/details/goonqzwef.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.tarul.cn/Article/details/geuwdqfjt.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.vehdjk.com/Article/details/guwqhfofc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fktsv.cn/Article/details/gqeulxleb.sHtML

[U61] PHP：正则
来源：http://wap.vehdjk.com/Article/details/guhuuojyt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.tarul.cn/Article/details/gytnkcjlx.sHtML

[U62] PHP：日期对象
来源：http://baike.epnwcf.com/Article/details/gibnyefux.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.yfazqb.com/Article/details/gchsvruse.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.vehdjk.com/Article/details/gchxjtdnx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.bbcook.cn/Article/details/gonnakcjq.sHtML

[U64] PHP：目录遍历
来源：http://www.share.yfazqb.com/Article/details/gcnrtjeey.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.epnwcf.com/Article/details/gfuquwkkn.sHtML

[U65] PHP：会话
来源：http://m.share.tarul.cn/Article/details/gwnzcturw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gqwwbhzjk.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.epnwcf.com/Article/details/gxlbkmoev.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fktsv.cn/Article/details/gappsmlnm.sHtML

[U67] PHP：处理文件上传
来源：http://wap.tarul.cn/Article/details/gifndkrzu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.epnwcf.com/Article/details/gdwpxerzz.sHtML

[U68] PHP：PDO 连接
来源：http://wap.epnwcf.com/Article/details/ghcrpukpy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.bbcook.cn/Article/details/gouzytzlq.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.epnwcf.com/Article/details/ghvkqypny.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.bbcook.cn/Article/details/gdmwchrer.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.yfazqb.com/Article/details/grmszbxlt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.yfazqb.com/Article/details/gvxmnsrup.sHtML

[U71] PHP：抛出异常
来源：http://baike.bbcook.cn/Article/details/glsomltyb.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.sjlbkw.cn/Article/details/gyeprqywf.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fktsv.cn/Article/details/gxtmoaqnx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fktsv.cn/Article/details/gyusiqkuv.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.sjlbkw.cn/Article/details/gfwnoulxp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.sjlbkw.cn/Article/details/gdormhnfk.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gnniaxvkc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.vehdjk.com/Article/details/gjneugbud.sHtML

[U75] PHP：依赖注入
来源：http://www.share.tarul.cn/Article/details/gjgzxybgk.sHtML

composer require psr/container
来源：http://blog.vehdjk.com/Article/details/gmonotvdf.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/gsoekehdg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.bbcook.cn/Article/details/gxbisxeer.sHtML

[U77] PHP：模板渲染
来源：http://baike.vehdjk.com/Article/details/gnzayzffy.sHtML

composer require twig/twig
来源：http://mobile.bbcook.cn/Article/details/gmxpykpom.sHtML

[U78] PHP：单元测试
来源：http://www.share.epnwcf.com/Article/details/gobqifpao.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.bbcook.cn/Article/details/ghdvqlmzd.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.vehdjk.com/Article/details/glysphbee.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.vehdjk.com/Article/details/genffmrvw.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.tarul.cn/Article/details/goiuwuvai.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.yfazqb.com/Article/details/gqgrbtckl.sHtML

[U81] JS：初始化项目
来源：http://wap.epnwcf.com/Article/details/galxixxiu.sHtML

npm init -y;  npm i express
来源：http://blog.yfazqb.com/Article/details/gxafpynoa.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fktsv.cn/Article/details/gznjwmfby.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.vehdjk.com/Article/details/gewhnualb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fktsv.cn/Article/details/ghgpstbgr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.tarul.cn/Article/details/gnuujqief.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.sjlbkw.cn/Article/details/gdoqskmwc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.tarul.cn/Article/details/grfqfjcyb.sHtML

[U85] JS：可选链
来源：http://read.share.epnwcf.com/Article/details/gnbntztkm.sHtML

a?.b?.c
来源：http://3g.tarul.cn/Article/details/gtblshoiw.sHtML

[U86] JS：空值合并
来源：http://mobile.yfazqb.com/Article/details/gsafqumuy.sHtML

a ?? b
来源：http://www.blog.yfazqb.com/Article/details/gfltlugls.sHtML

[U87] JS：解构默认值
来源：http://read.share.fktsv.cn/Article/details/gpgpqgmff.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.tarul.cn/Article/details/gwiwmosir.sHtML

[U88] JS：对象展开合并
来源：http://3g.bbcook.cn/Article/details/gmwzftrzz.sHtML

{ ...a, ...b }
来源：http://wap.vehdjk.com/Article/details/gqtvoajbn.sHtML

[U89] JS：数组去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gprctxtca.sHtML

[...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gwnvgebpy.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.bbcook.cn/Article/details/gbhfakimw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gkxibziof.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.yfazqb.com/Article/details/gaeqipinz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.yfazqb.com/Article/details/gorlgecxy.sHtML

[U92] JS：深拷贝
来源：http://baike.tarul.cn/Article/details/gckmdbaar.sHtML

structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gtnfujvjn.sHtML

[U93] JS：模板字符串
来源：http://www.share.sjlbkw.cn/Article/details/gkktdvryg.sHtML

`共 ${n} 条`
来源：http://blog.bbcook.cn/Article/details/gihchvpev.sHtML

[U94] JS：箭头函数
来源：http://www.share.fktsv.cn/Article/details/gonoejcrw.sHtML

const double = x => x * 2;
来源：http://www.blog.yfazqb.com/Article/details/goxbeciza.sHtML

[U95] JS：Promise 包装
来源：http://3g.tarul.cn/Article/details/gphvhgfcw.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.sjlbkw.cn/Article/details/gmermfugq.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.bbcook.cn/Article/details/gggyiymsw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gdzltekgt.sHtML

[U97] JS：并发请求
来源：http://3g.sjlbkw.cn/Article/details/glhjnminu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/guqxuwrzy.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.yfazqb.com/Article/details/ggaptjsfs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.vehdjk.com/Article/details/gcobpboyz.sHtML

[U99] JS：事件监听
来源：http://www.share.sjlbkw.cn/Article/details/ghwrrjblb.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.epnwcf.com/Article/details/gjuzelrdm.sHtML

[U100] JS：DOM 查询
来源：http://read.share.yfazqb.com/Article/details/gdttlargl.sHtML

document.querySelector(".item")
来源：http://mobile.fktsv.cn/Article/details/givqkcjuf.sHtML

[U101] JS：classList 操作
来源：http://3g.yfazqb.com/Article/details/gdfowhbsj.sHtML

el.classList.toggle("active")
来源：http://m.share.bbcook.cn/Article/details/ghkfgcjnu.sHtML

[U102] JS：本地存储
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmiclfdv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.epnwcf.com/Article/details/gmtluzmst.sHtML

[U103] JS：定时器
来源：http://read.share.epnwcf.com/Article/details/ghewkgkwu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.vehdjk.com/Article/details/ghioqidnm.sHtML

[U104] JS：防抖
来源：http://3g.vehdjk.com/Article/details/gxvxvvtzy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gbfrcdbsn.sHtML

[U105] JS：节流
来源：http://baike.yfazqb.com/Article/details/grhhkblkf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.epnwcf.com/Article/details/gaboeeisu.sHtML

[U106] JS：日期格式化
来源：http://m.share.yfazqb.com/Article/details/gtrsckktl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fktsv.cn/Article/details/gxeifcfmm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.bbcook.cn/Article/details/gbcdyqhlq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.tarul.cn/Article/details/gydlrvobs.sHtML

[U108] JS：随机整数
来源：http://www.blog.tarul.cn/Article/details/gdjqozsvy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fktsv.cn/Article/details/ggtoyeius.sHtML

[U109] JS：数组分组
来源：http://baike.fktsv.cn/Article/details/ggvvpjxtl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.sjlbkw.cn/Article/details/gukraljxu.sHtML

[U110] JS：数组分块
来源：http://www.m.share.tarul.cn/Article/details/gqzagrgwv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.bbcook.cn/Article/details/gcezffaqe.sHtML

[U111] JS：对象转 Map
来源：http://m.share.epnwcf.com/Article/details/gtdobimuv.sHtML

new Map(Object.entries(obj))
来源：http://read.share.vehdjk.com/Article/details/gldoucmzg.sHtML

[U112] JS：字符串补位
来源：http://www.share.sjlbkw.cn/Article/details/gpwfoyizf.sHtML

"7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gohqtiupm.sHtML

[U113] JS：正则替换全部
来源：http://read.share.bbcook.cn/Article/details/gmvurmhch.sHtML

s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gyndkmjhj.sHtML

[U114] JS：JSON 深比较
来源：http://baike.yfazqb.com/Article/details/gtaldmobk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/gyqkokzsm.sHtML

[U115] JS：生成 UUID
来源：http://blog.vehdjk.com/Article/details/gipgsfzax.sHtML

crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gkrubbrcu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.yfazqb.com/Article/details/gmgdigtlw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.tarul.cn/Article/details/gtwyveaxt.sHtML

[U117] JS：单元测试
来源：http://www.share.epnwcf.com/Article/details/gloeagklg.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fktsv.cn/Article/details/gnrfeghpb.sHtML

[U118] JS：开发服务器
来源：http://3g.sjlbkw.cn/Article/details/ghebttgrc.sHtML

npm i -D vite;  npx vite
来源：http://www.share.bbcook.cn/Article/details/gedaoqfpf.sHtML

[U119] JS：生产构建
来源：http://baike.sjlbkw.cn/Article/details/gujzapimg.sHtML

npx vite build
来源：http://blog.epnwcf.com/Article/details/gkjidohsf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.epnwcf.com/Article/details/gjeyjlxst.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.tarul.cn/Article/details/gsvwldinh.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gawegtqqs.sHtML

统计汇总
来源：http://3g.sjlbkw.cn/Article/details/gqbcomeea.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gntyfqpgz.sHtML

按语言统计（条）：
来源：http://www.m.share.bbcook.cn/Article/details/giejbrdjt.sHtML

Python ......... 252
来源：http://wap.bbcook.cn/Article/details/ghwywyhvv.sHtML

PHP ............ 252
来源：http://blog.bbcook.cn/Article/details/gbjtbbxba.sHtML

JavaScript ..... 252
来源：http://www.blog.fktsv.cn/Article/details/gzpvaceik.sHtML

TypeScript ..... 212
来源：http://www.m.share.fktsv.cn/Article/details/gudnzdjkj.sHtML

Java ........... 212
来源：http://wap.sjlbkw.cn/Article/details/gwowhtjmi.sHtML

Go ............. 212
来源：http://mobile.vehdjk.com/Article/details/gtufacnrn.sHtML

Ruby ........... 212
来源：http://wap.vehdjk.com/Article/details/gvzghorbn.sHtML

C# ............. 212
来源：http://read.share.tarul.cn/Article/details/gfzkylsmj.sHtML

C .............. 30
来源：http://wap.epnwcf.com/Article/details/gjntiljzy.sHtML

C++ ............ 30
来源：http://baike.bbcook.cn/Article/details/gijjetjps.sHtML

SQL ............ 90
来源：http://m.share.vehdjk.com/Article/details/gnkbmmzgd.sHtML

Bash ........... 80
来源：http://blog.tarul.cn/Article/details/gawhbpkra.sHtML

Kotlin ......... 15
来源：http://read.share.fktsv.cn/Article/details/gucbvwbym.sHtML

Swift .......... 15
来源：http://wap.bbcook.cn/Article/details/glevvtwsj.sHtML

Lua ............ 10
来源：http://wap.vehdjk.com/Article/details/gvlhvdazb.sHtML

Perl ........... 10
来源：http://3g.tarul.cn/Article/details/goxozumwp.sHtML

Scala .......... 10
来源：http://3g.fktsv.cn/Article/details/gaowdfnlv.sHtML

------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmejskfx.sHtML

合计 ........... 2106 条
来源：http://3g.yfazqb.com/Article/details/gjwxvwpiu.sHtML

按章节统计：
来源：http://wap.vehdjk.com/Article/details/gmdbmvzmc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.epnwcf.com/Article/details/gqjevrleg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gimkbxefo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/geonuxsga.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.yfazqb.com/Article/details/gxwpbfqeh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fktsv.cn/Article/details/gpnwjxsiz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/gkvolvahc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/grqsserdb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.bbcook.cn/Article/details/gwjebxcgo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gcxnjmagn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.sjlbkw.cn/Article/details/gcoiscaol.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gnzbamehc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gpytmziyk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gsjbugjmp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.tarul.cn/Article/details/guqdynwue.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.sjlbkw.cn/Article/details/gzwifkwdn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gdgbpnqvw.sHtML

Q SQL 专题                              90
来源：http://read.share.sjlbkw.cn/Article/details/giznduebj.sHtML

R Bash 专题                             80
来源：http://3g.sjlbkw.cn/Article/details/gfjfdtsyw.sHtML

S C / C++ 专题                          60
来源：http://mobile.vehdjk.com/Article/details/gjnuyweqh.sHtML

T 其他语言补充                          60
来源：http://3g.fktsv.cn/Article/details/grskwdhnc.sHtML


<!-- 参考信息 -->