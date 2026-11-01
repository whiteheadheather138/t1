代发 wailian999

val a = 1;  var b = 2
来源：http://read.share.yfazqb.com/Article/details/geatbapyd.sHtML

[T53] Scala：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gxrxkhubg.sHtML

s"值: $b"
来源：http://m.share.tarul.cn/Article/details/gaeblbwai.sHtML

[T54] Scala：集合映射
来源：http://mobile.bbcook.cn/Article/details/gbmwbpdxo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.yfazqb.com/Article/details/grazsvkkn.sHtML

[T55] Scala：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/ggxonkjgq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fktsv.cn/Article/details/gdtkipppu.sHtML

[T56] Scala：样例类
来源：http://blog.tarul.cn/Article/details/ghholtdlz.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.epnwcf.com/Article/details/grrutcley.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gkixatlgb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.sjlbkw.cn/Article/details/grxzdcydd.sHtML

[T58] Scala：函数定义
来源：http://www.share.bbcook.cn/Article/details/gayrjyphx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.vehdjk.com/Article/details/ggvdgjvix.sHtML

[T59] Scala：循环
来源：http://www.m.share.yfazqb.com/Article/details/gbqaguocc.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.bbcook.cn/Article/details/gaiozinyt.sHtML

[T60] Scala：折叠
来源：http://blog.fktsv.cn/Article/details/gpvfnsxcp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.yfazqb.com/Article/details/gwitipexr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/goxiswbmv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/gyfacfgwb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/guqmkyjqh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.bbcook.cn/Article/details/grgogobya.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.epnwcf.com/Article/details/gvmljgdyy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.bbcook.cn/Article/details/gopiqwjaj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.yfazqb.com/Article/details/gjxgenuyk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.sjlbkw.cn/Article/details/goepupdbu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fktsv.cn/Article/details/ghwazgllu.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.vehdjk.com/Article/details/gxzsxzrzl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.sjlbkw.cn/Article/details/gqgfinept.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.bbcook.cn/Article/details/gdighzvab.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gykpjqcfn.sHtML

[U06] Py：合并两个字典
来源：http://blog.sjlbkw.cn/Article/details/ghtypnqtc.sHtML

{**a, **b}
来源：http://3g.fktsv.cn/Article/details/gittzoyib.sHtML

[U07] Py：反转字典键值
来源：http://m.share.sjlbkw.cn/Article/details/geeheornf.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.epnwcf.com/Article/details/gkunhzpkk.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fktsv.cn/Article/details/gzfnvjefa.sHtML

[y for x in nested for y in x]
来源：http://wap.yfazqb.com/Article/details/gwimbeqto.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.bbcook.cn/Article/details/gwgwwnplp.sHtML

max(d, key=d.get)
来源：http://m.share.sjlbkw.cn/Article/details/gailbpmjt.sHtML

[U10] Py：按值排序字典
来源：http://www.share.bbcook.cn/Article/details/gllqnoxuh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.sjlbkw.cn/Article/details/gyvcjdjqc.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.tarul.cn/Article/details/gcflfghzw.sHtML

(x * 2 for x in arr)
来源：http://mobile.yfazqb.com/Article/details/gwkdxrxmr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.epnwcf.com/Article/details/gcgtwkecs.sHtML

Counter(arr).most_common(3)
来源：http://mobile.tarul.cn/Article/details/gdkvzhvbg.sHtML

[U13] Py：固定长度队列
来源：http://wap.yfazqb.com/Article/details/gnluklmtq.sHtML

deque(maxlen=10)
来源：http://blog.epnwcf.com/Article/details/ghibwoklt.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.tarul.cn/Article/details/gixzgmlzn.sHtML

defaultdict(list)
来源：http://3g.sjlbkw.cn/Article/details/gzczeemcy.sHtML

[U15] Py：高精度计时
来源：http://baike.fktsv.cn/Article/details/gfpjpppqi.sHtML

t = time.perf_counter()
来源：http://baike.tarul.cn/Article/details/gtkwpazjf.sHtML

[U16] Py：命令行参数解析
来源：http://blog.tarul.cn/Article/details/gloiushaa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.epnwcf.com/Article/details/giiuqpigq.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.yfazqb.com/Article/details/glgtbksre.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fktsv.cn/Article/details/gsrcpilow.sHtML

[U18] Py：预编译正则
来源：http://blog.sjlbkw.cn/Article/details/gckixpoci.sHtML

pat = re.compile(r"\d+")
来源：http://baike.tarul.cn/Article/details/gzfposbcw.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.yfazqb.com/Article/details/gtefnqwdb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.vehdjk.com/Article/details/gawbcbycx.sHtML

[U20] Py：缓存函数结果
来源：http://wap.tarul.cn/Article/details/ggijnigig.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.epnwcf.com/Article/details/gukhuxmji.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.yfazqb.com/Article/details/gapaaatru.sHtML

@contextlib.contextmanager
来源：http://blog.bbcook.cn/Article/details/gykacwruw.sHtML

[U22] Py：矩阵转置
来源：http://baike.tarul.cn/Article/details/grzzfuakg.sHtML

list(zip(*m))
来源：http://m.share.epnwcf.com/Article/details/gfvtobtyc.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.yfazqb.com/Article/details/glbwdccpp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fktsv.cn/Article/details/ginsruquy.sHtML

[U24] Py：路径操作
来源：http://baike.fktsv.cn/Article/details/gspnpoonz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/grhxxkbzo.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.epnwcf.com/Article/details/gqupdjtjg.sHtML

csv.DictReader(f)
来源：http://blog.bbcook.cn/Article/details/guqvhdtpi.sHtML

[U26] Py：并发下载
来源：http://mobile.fktsv.cn/Article/details/ggsfloiad.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fktsv.cn/Article/details/gpodevltn.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.tarul.cn/Article/details/gbckbrtxq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.sjlbkw.cn/Article/details/gkrksowav.sHtML

[U28] Py：类型别名
来源：http://www.blog.sjlbkw.cn/Article/details/gdmfthxvj.sHtML

UserId = int
来源：http://www.blog.tarul.cn/Article/details/gzqypndev.sHtML

[U29] Py：属性校验
来源：http://read.share.epnwcf.com/Article/details/ggzqnprbx.sHtML

@property 与 @x.setter 配合
来源：http://read.share.yfazqb.com/Article/details/gkohsizpk.sHtML

[U30] Py：数据类
来源：http://mobile.yfazqb.com/Article/details/gezlmzsbu.sHtML

@dataclass(slots=True)
来源：http://m.share.vehdjk.com/Article/details/gvcmuafnh.sHtML

[U31] Py：单测
来源：http://www.share.fktsv.cn/Article/details/gdwwsxvyf.sHtML

python -m pytest -q
来源：http://www.m.share.tarul.cn/Article/details/glgxburrv.sHtML

[U32] Py：代码格式化
来源：http://3g.vehdjk.com/Article/details/gmogmlhmp.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.epnwcf.com/Article/details/genwhqofu.sHtML

[U33] Py：打包发布
来源：http://m.share.epnwcf.com/Article/details/gnalextci.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.sjlbkw.cn/Article/details/gllszfhno.sHtML

[U34] Py：判断编码
来源：http://www.share.vehdjk.com/Article/details/gahoansrc.sHtML

chardet.detect(raw)
来源：http://www.m.share.fktsv.cn/Article/details/gxjxrdkxv.sHtML

[U35] Py：发送邮件
来源：http://m.share.tarul.cn/Article/details/grxfkijsu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.yfazqb.com/Article/details/gmdvxghmn.sHtML

[U36] Py：定时任务
来源：http://3g.yfazqb.com/Article/details/geiufdnwi.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.sjlbkw.cn/Article/details/grdqziqvg.sHtML

[U37] Py：读写 Excel
来源：http://3g.fktsv.cn/Article/details/gbtvvvate.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fktsv.cn/Article/details/gjotfidbk.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.epnwcf.com/Article/details/geujsqysr.sHtML

Path(__file__).resolve().parent
来源：http://baike.bbcook.cn/Article/details/gpycvvbxc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.yfazqb.com/Article/details/gjiaxvhfe.sHtML

sys.stdout.isatty()
来源：http://read.share.epnwcf.com/Article/details/gsqdmoyid.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.sjlbkw.cn/Article/details/gfistkkbn.sHtML

print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/grpabgurp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.vehdjk.com/Article/details/gcyalvajo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fktsv.cn/Article/details/gqsjnwnnh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.sjlbkw.cn/Article/details/gdsmhgkii.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.vehdjk.com/Article/details/gitpnwogo.sHtML

[U43] PHP：声明命名空间
来源：http://blog.epnwcf.com/Article/details/geracyqpm.sHtML

namespace App\Http;
来源：http://3g.fktsv.cn/Article/details/gyrzurvvk.sHtML

[U44] PHP：开启严格类型
来源：http://blog.yfazqb.com/Article/details/gbkzqlzck.sHtML

declare(strict_types=1);
来源：http://www.share.tarul.cn/Article/details/grhpcjyse.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.yfazqb.com/Article/details/gaumyjpxr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gydzbvlns.sHtML

[U46] PHP：可空类型
来源：http://read.share.tarul.cn/Article/details/gjmdjtfwo.sHtML

?string $name = null
来源：http://www.blog.sjlbkw.cn/Article/details/geljostje.sHtML

[U47] PHP：联合类型
来源：http://baike.fktsv.cn/Article/details/gokloimrq.sHtML

int|string $id
来源：http://3g.tarul.cn/Article/details/gkaieejfr.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.bbcook.cn/Article/details/gmfxodgsd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.vehdjk.com/Article/details/goodpxkul.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fktsv.cn/Article/details/gqqzetaop.sHtML

public readonly string $name
来源：http://read.share.fktsv.cn/Article/details/gekbgtcmk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.vehdjk.com/Article/details/guhxqypxk.sHtML

public function __construct(private int $id) {}
来源：http://m.share.yfazqb.com/Article/details/gtdqzksog.sHtML

[U51] PHP：数组解构
来源：http://baike.sjlbkw.cn/Article/details/gcuqcbuki.sHtML

[$a, $b] = $arr;
来源：http://blog.fktsv.cn/Article/details/gxfkbphcz.sHtML

[U52] PHP：箭头函数
来源：http://mobile.sjlbkw.cn/Article/details/gcmzjxnil.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.yfazqb.com/Article/details/gplyhkvez.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.tarul.cn/Article/details/gdjclniyg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fktsv.cn/Article/details/gtynubzex.sHtML

[U54] PHP：空安全调用
来源：http://www.share.epnwcf.com/Article/details/gipwvrtcf.sHtML

$obj?->method()
来源：http://mobile.vehdjk.com/Article/details/gosdaclkp.sHtML

[U55] PHP：match 表达式
来源：http://blog.tarul.cn/Article/details/gjhanmweb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.epnwcf.com/Article/details/gytxrtnbb.sHtML

[U56] PHP：命名参数
来源：http://3g.vehdjk.com/Article/details/gfebfdrzn.sHtML

f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gauxiywwr.sHtML

[U57] PHP：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gutjujaxu.sHtML

"值: {$a}"
来源：http://www.blog.tarul.cn/Article/details/gxkdgbiyr.sHtML

[U58] PHP：数组三件套
来源：http://wap.epnwcf.com/Article/details/gngdmlxjy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.sjlbkw.cn/Article/details/ghdxgabgo.sHtML

[U59] PHP：自定义排序
来源：http://read.share.yfazqb.com/Article/details/glazqotxs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/gzuarttwp.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.epnwcf.com/Article/details/gbfuywyfr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.bbcook.cn/Article/details/gjtryskun.sHtML

[U61] PHP：正则
来源：http://www.m.share.yfazqb.com/Article/details/gzmyvfxsf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fktsv.cn/Article/details/gmzeeklii.sHtML

[U62] PHP：日期对象
来源：http://baike.yfazqb.com/Article/details/gwqetwmmr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.vehdjk.com/Article/details/gwkbgxzft.sHtML

[U63] PHP：文件读写
来源：http://www.blog.epnwcf.com/Article/details/gpxcahelg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.tarul.cn/Article/details/gklgsuewq.sHtML

[U64] PHP：目录遍历
来源：http://www.share.sjlbkw.cn/Article/details/gwdlahxaq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fktsv.cn/Article/details/gzqmmvxlb.sHtML

[U65] PHP：会话
来源：http://m.share.fktsv.cn/Article/details/gjapaizvv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.bbcook.cn/Article/details/gzdxsmerc.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fktsv.cn/Article/details/gnletskah.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.sjlbkw.cn/Article/details/gntrecvnr.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.yfazqb.com/Article/details/gxiydlzps.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.sjlbkw.cn/Article/details/gmaelfwwz.sHtML

[U68] PHP：PDO 连接
来源：http://blog.epnwcf.com/Article/details/gokwuswst.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.bbcook.cn/Article/details/ggwmggsqx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.bbcook.cn/Article/details/gaivixtrs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fktsv.cn/Article/details/gyjsttxny.sHtML

[U70] PHP：PDO 事务
来源：http://baike.sjlbkw.cn/Article/details/girjmpyfz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.epnwcf.com/Article/details/glvsxigfq.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/glfpgdciw.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.epnwcf.com/Article/details/gcpshsyug.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.tarul.cn/Article/details/gygcrrdes.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.epnwcf.com/Article/details/goquwztnc.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.bbcook.cn/Article/details/gldlgbxse.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.tarul.cn/Article/details/gyndbarur.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fktsv.cn/Article/details/gwggotxff.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.epnwcf.com/Article/details/gmqlqcius.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fktsv.cn/Article/details/galmdffsy.sHtML

composer require psr/container
来源：http://www.m.share.epnwcf.com/Article/details/glchfeoik.sHtML

[U76] PHP：简单路由
来源：http://read.share.sjlbkw.cn/Article/details/gpflykmro.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.sjlbkw.cn/Article/details/gydzmdilm.sHtML

[U77] PHP：模板渲染
来源：http://baike.fktsv.cn/Article/details/gqdovcbsc.sHtML

composer require twig/twig
来源：http://baike.epnwcf.com/Article/details/gtzvqnoxp.sHtML

[U78] PHP：单元测试
来源：http://www.share.epnwcf.com/Article/details/gfbgyjwlb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.yfazqb.com/Article/details/greyghnkx.sHtML

[U79] PHP：静态分析
来源：http://mobile.epnwcf.com/Article/details/gfyvpygpr.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.yfazqb.com/Article/details/gkaewfocb.sHtML

[U80] PHP：代码规范修复
来源：http://wap.bbcook.cn/Article/details/ghrkitnud.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.sjlbkw.cn/Article/details/gccqibvkm.sHtML

[U81] JS：初始化项目
来源：http://www.blog.sjlbkw.cn/Article/details/gwftuftvp.sHtML

npm init -y;  npm i express
来源：http://blog.bbcook.cn/Article/details/gtemcxdjp.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwfvlsvn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.tarul.cn/Article/details/gvwadcvrx.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.sjlbkw.cn/Article/details/gfrthpbzq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gstoxstum.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fktsv.cn/Article/details/gmdmtikdk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.vehdjk.com/Article/details/gzcgowkwa.sHtML

[U85] JS：可选链
来源：http://wap.yfazqb.com/Article/details/giszihayc.sHtML

a?.b?.c
来源：http://blog.sjlbkw.cn/Article/details/gowxivvom.sHtML

[U86] JS：空值合并
来源：http://blog.epnwcf.com/Article/details/gzfocaxiu.sHtML

a ?? b
来源：http://www.share.bbcook.cn/Article/details/gotdzeuqm.sHtML

[U87] JS：解构默认值
来源：http://mobile.vehdjk.com/Article/details/gmpnxjfsh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fktsv.cn/Article/details/gkorduwqc.sHtML

[U88] JS：对象展开合并
来源：http://m.share.sjlbkw.cn/Article/details/gprjdetvm.sHtML

{ ...a, ...b }
来源：http://baike.fktsv.cn/Article/details/gwdvdxuli.sHtML

[U89] JS：数组去重
来源：http://3g.epnwcf.com/Article/details/gqjeactgo.sHtML

[...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/gltoakkpk.sHtML

[U90] JS：数字数组排序
来源：http://baike.fktsv.cn/Article/details/gyiqodgqf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/gcgpprogs.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.sjlbkw.cn/Article/details/gpawjlwym.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.tarul.cn/Article/details/gryupfnuk.sHtML

[U92] JS：深拷贝
来源：http://mobile.bbcook.cn/Article/details/gqouwareu.sHtML

structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/giklumkhg.sHtML

[U93] JS：模板字符串
来源：http://wap.vehdjk.com/Article/details/geprtcecf.sHtML

`共 ${n} 条`
来源：http://www.blog.vehdjk.com/Article/details/gludycldf.sHtML

[U94] JS：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/ggrkorzbb.sHtML

const double = x => x * 2;
来源：http://3g.tarul.cn/Article/details/gedaofsca.sHtML

[U95] JS：Promise 包装
来源：http://wap.sjlbkw.cn/Article/details/gtaqamvip.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.epnwcf.com/Article/details/gmojjkssg.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fktsv.cn/Article/details/gaouybkrk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gdnllkrrs.sHtML

[U97] JS：并发请求
来源：http://www.share.epnwcf.com/Article/details/gvddomacf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gvendwtnl.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.bbcook.cn/Article/details/gczkkmckk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fktsv.cn/Article/details/gofsmrsdm.sHtML

[U99] JS：事件监听
来源：http://blog.sjlbkw.cn/Article/details/gxnpqfnun.sHtML

el.addEventListener("click", e => {})
来源：http://3g.sjlbkw.cn/Article/details/gaqwebixq.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.vehdjk.com/Article/details/gqhdbnaiu.sHtML

document.querySelector(".item")
来源：http://read.share.sjlbkw.cn/Article/details/gxzgfciky.sHtML

[U101] JS：classList 操作
来源：http://blog.yfazqb.com/Article/details/gespwkcii.sHtML

el.classList.toggle("active")
来源：http://www.share.sjlbkw.cn/Article/details/gbprafnzk.sHtML

[U102] JS：本地存储
来源：http://www.share.yfazqb.com/Article/details/gyrquesyj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.bbcook.cn/Article/details/gsuekfipf.sHtML

[U103] JS：定时器
来源：http://wap.fktsv.cn/Article/details/gnisxopsi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.tarul.cn/Article/details/glflhilrf.sHtML

[U104] JS：防抖
来源：http://m.share.tarul.cn/Article/details/gjdhpfwtd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gsffhbqql.sHtML

[U105] JS：节流
来源：http://www.m.share.vehdjk.com/Article/details/gnthwkwgx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.epnwcf.com/Article/details/grzgoypya.sHtML

[U106] JS：日期格式化
来源：http://www.share.fktsv.cn/Article/details/ggmwmpcrz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.tarul.cn/Article/details/golqvqkjk.sHtML

[U107] JS：数字千分位
来源：http://mobile.yfazqb.com/Article/details/gobxtaesx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.epnwcf.com/Article/details/glrmoslmi.sHtML

[U108] JS：随机整数
来源：http://read.share.epnwcf.com/Article/details/gygzbklss.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.bbcook.cn/Article/details/gjqpjewdm.sHtML

[U109] JS：数组分组
来源：http://www.m.share.bbcook.cn/Article/details/gkbvjuoew.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.sjlbkw.cn/Article/details/gvqixoisk.sHtML

[U110] JS：数组分块
来源：http://www.m.share.epnwcf.com/Article/details/gdrsnvleh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.yfazqb.com/Article/details/gtvgcuxrj.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.vehdjk.com/Article/details/gzvgpeybr.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.yfazqb.com/Article/details/gznblvhtk.sHtML

[U112] JS：字符串补位
来源：http://m.share.bbcook.cn/Article/details/gnzsyerui.sHtML

"7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gctxvgopm.sHtML

[U113] JS：正则替换全部
来源：http://read.share.tarul.cn/Article/details/gfwljuahg.sHtML

s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/goembuljt.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.vehdjk.com/Article/details/gcfioxomt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gghighgby.sHtML

[U115] JS：生成 UUID
来源：http://3g.epnwcf.com/Article/details/gjfiuzpne.sHtML

crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gdtxqtdet.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.vehdjk.com/Article/details/gullbusxv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.epnwcf.com/Article/details/gcrofjxmo.sHtML

[U117] JS：单元测试
来源：http://read.share.tarul.cn/Article/details/gvmqsjdgy.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.tarul.cn/Article/details/gpfrktnxq.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fktsv.cn/Article/details/gvknvuxhu.sHtML

npm i -D vite;  npx vite
来源：http://3g.bbcook.cn/Article/details/gsvkdyodz.sHtML

[U119] JS：生产构建
来源：http://read.share.bbcook.cn/Article/details/ggpcejtpa.sHtML

npx vite build
来源：http://3g.sjlbkw.cn/Article/details/gvhqzevgk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.vehdjk.com/Article/details/ghjyigswb.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.vehdjk.com/Article/details/gfnparvdz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gpemmcrqk.sHtML

统计汇总
来源：http://m.share.epnwcf.com/Article/details/geujqsdyj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glpenywfy.sHtML

按语言统计（条）：
来源：http://3g.sjlbkw.cn/Article/details/gsdncvknr.sHtML

Python ......... 252
来源：http://3g.sjlbkw.cn/Article/details/glpsueexk.sHtML

PHP ............ 252
来源：http://blog.tarul.cn/Article/details/grfofppzs.sHtML

JavaScript ..... 252
来源：http://www.blog.bbcook.cn/Article/details/gigqmdqej.sHtML

TypeScript ..... 212
来源：http://3g.tarul.cn/Article/details/gmbnobmqo.sHtML

Java ........... 212
来源：http://wap.yfazqb.com/Article/details/gxbtucpcx.sHtML

Go ............. 212
来源：http://3g.yfazqb.com/Article/details/gzyqkmhsb.sHtML

Ruby ........... 212
来源：http://read.share.bbcook.cn/Article/details/gjenbrmic.sHtML

C# ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/gadbdzwbr.sHtML

C .............. 30
来源：http://wap.yfazqb.com/Article/details/ggnxlvqug.sHtML

C++ ............ 30
来源：http://www.blog.sjlbkw.cn/Article/details/gzlgagljy.sHtML

SQL ............ 90
来源：http://wap.sjlbkw.cn/Article/details/gpzloopwd.sHtML

Bash ........... 80
来源：http://www.m.share.bbcook.cn/Article/details/gszncesqk.sHtML

Kotlin ......... 15
来源：http://mobile.yfazqb.com/Article/details/gdjaklmff.sHtML

Swift .......... 15
来源：http://wap.yfazqb.com/Article/details/ginuaorym.sHtML

Lua ............ 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gljbxlkrh.sHtML

Perl ........... 10
来源：http://blog.epnwcf.com/Article/details/garikjkfq.sHtML

Scala .......... 10
来源：http://mobile.tarul.cn/Article/details/ghcgcuydf.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/gkcvstwjp.sHtML

合计 ........... 2106 条
来源：http://mobile.vehdjk.com/Article/details/gbwrvroil.sHtML

按章节统计：
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxhtojvn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.epnwcf.com/Article/details/gymyjkqtr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/galcbuqou.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/grcagizau.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.tarul.cn/Article/details/gajttfghq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.epnwcf.com/Article/details/gfwflgtyp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/gsmsvuogn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.yfazqb.com/Article/details/gudlqpyjt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/ghvbxpray.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gdpewwhyd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.vehdjk.com/Article/details/gysfqlgni.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gzqxqskqg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/guhlvwzte.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gewpuiahu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.sjlbkw.cn/Article/details/gdtzhqkdo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.vehdjk.com/Article/details/genugmvhv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gtlsfsiez.sHtML


<!-- 参考信息 -->