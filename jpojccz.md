代发 wailian999

val a = 1;  var b = 2
来源：http://m.share.epnwcf.com/Article/details/ghdgoymrv.sHtML

[T53] Scala：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gaowmnuvr.sHtML

s"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/gqakezqss.sHtML

[T54] Scala：集合映射
来源：http://m.share.vehdjk.com/Article/details/gnqaykogh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gbqropsxn.sHtML

[T55] Scala：集合过滤
来源：http://baike.bbcook.cn/Article/details/gmqmiqrye.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.bbcook.cn/Article/details/gponzmbab.sHtML

[T56] Scala：样例类
来源：http://read.share.bbcook.cn/Article/details/gyjnwumbq.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/grrzmnvam.sHtML

[T57] Scala：模式匹配
来源：http://wap.fktsv.cn/Article/details/gtnoboxyl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fktsv.cn/Article/details/gzfrvpjzp.sHtML

[T58] Scala：函数定义
来源：http://m.share.tarul.cn/Article/details/gqduxqacf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.sjlbkw.cn/Article/details/gyovdnohx.sHtML

[T59] Scala：循环
来源：http://3g.vehdjk.com/Article/details/guhjwplhb.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gxsulrzbe.sHtML

[T60] Scala：折叠
来源：http://m.share.tarul.cn/Article/details/gvgaebtfs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.bbcook.cn/Article/details/gvdtapyhb.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gvybxcume.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.bbcook.cn/Article/details/gsyhjstvs.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpjlptlsz.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.tarul.cn/Article/details/gcoqlxpsg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.sjlbkw.cn/Article/details/guqpgvtpr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.epnwcf.com/Article/details/gvelpqypg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.yfazqb.com/Article/details/gegnludml.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fktsv.cn/Article/details/gnqxqhjlo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.sjlbkw.cn/Article/details/garffwnac.sHtML

[U04] Py：变量调试打印
来源：http://baike.epnwcf.com/Article/details/gvxsrzzeb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.yfazqb.com/Article/details/gokslewyo.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fktsv.cn/Article/details/gnfholeji.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gkvfhcfgt.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.bbcook.cn/Article/details/gdmxywvlt.sHtML

{**a, **b}
来源：http://baike.sjlbkw.cn/Article/details/gqkxmgjih.sHtML

[U07] Py：反转字典键值
来源：http://baike.bbcook.cn/Article/details/gywxkxspi.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fktsv.cn/Article/details/gixwoubdm.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.tarul.cn/Article/details/goxptvcrb.sHtML

[y for x in nested for y in x]
来源：http://m.share.yfazqb.com/Article/details/gxtyypazi.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fktsv.cn/Article/details/gajozwyqv.sHtML

max(d, key=d.get)
来源：http://www.blog.fktsv.cn/Article/details/gsiorkzmu.sHtML

[U10] Py：按值排序字典
来源：http://blog.epnwcf.com/Article/details/ghbttpqzl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.vehdjk.com/Article/details/gzvkfbuvl.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.yfazqb.com/Article/details/geysxhspz.sHtML

(x * 2 for x in arr)
来源：http://wap.yfazqb.com/Article/details/gproyxeum.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fktsv.cn/Article/details/grarpofqx.sHtML

Counter(arr).most_common(3)
来源：http://3g.tarul.cn/Article/details/gwkfefavj.sHtML

[U13] Py：固定长度队列
来源：http://www.share.yfazqb.com/Article/details/gwhjbogro.sHtML

deque(maxlen=10)
来源：http://read.share.bbcook.cn/Article/details/gkzlzknji.sHtML

[U14] Py：分组收集到列表
来源：http://blog.epnwcf.com/Article/details/gvnpyclwy.sHtML

defaultdict(list)
来源：http://www.blog.tarul.cn/Article/details/gjxetjsga.sHtML

[U15] Py：高精度计时
来源：http://3g.vehdjk.com/Article/details/gmflgpisu.sHtML

t = time.perf_counter()
来源：http://read.share.vehdjk.com/Article/details/guepuzhiu.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.vehdjk.com/Article/details/gwxmpvuku.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fktsv.cn/Article/details/gbhmvutlt.sHtML

[U17] Py：初始化日志
来源：http://wap.bbcook.cn/Article/details/gthkhgpvu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fktsv.cn/Article/details/grrqurbcc.sHtML

[U18] Py：预编译正则
来源：http://blog.sjlbkw.cn/Article/details/gpebtwvgi.sHtML

pat = re.compile(r"\d+")
来源：http://blog.sjlbkw.cn/Article/details/gkmouvppb.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.yfazqb.com/Article/details/gtmgpblds.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.sjlbkw.cn/Article/details/gyrxwsxti.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.yfazqb.com/Article/details/gcdlvlbuy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fktsv.cn/Article/details/gaqoipfkp.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fktsv.cn/Article/details/gwpjsvtlv.sHtML

@contextlib.contextmanager
来源：http://baike.tarul.cn/Article/details/gkifmjsnl.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.bbcook.cn/Article/details/gjwqduyky.sHtML

list(zip(*m))
来源：http://www.blog.sjlbkw.cn/Article/details/grqqkmvod.sHtML

[U23] Py：分块读取大文件
来源：http://blog.tarul.cn/Article/details/gexsqtdpd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.sjlbkw.cn/Article/details/gxpueubxb.sHtML

[U24] Py：路径操作
来源：http://www.blog.vehdjk.com/Article/details/gdscllczh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/ghbwuofbb.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.tarul.cn/Article/details/grtpeucsi.sHtML

csv.DictReader(f)
来源：http://www.share.yfazqb.com/Article/details/gkwzwmttq.sHtML

[U26] Py：并发下载
来源：http://blog.bbcook.cn/Article/details/gjqilatgy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.tarul.cn/Article/details/giflkwlvc.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.sjlbkw.cn/Article/details/gzxkeeaut.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fktsv.cn/Article/details/ghncnfzid.sHtML

[U28] Py：类型别名
来源：http://www.share.sjlbkw.cn/Article/details/gblksrkua.sHtML

UserId = int
来源：http://read.share.yfazqb.com/Article/details/gyxxvtpmx.sHtML

[U29] Py：属性校验
来源：http://wap.tarul.cn/Article/details/gziviskjk.sHtML

@property 与 @x.setter 配合
来源：http://mobile.tarul.cn/Article/details/glbakqkcn.sHtML

[U30] Py：数据类
来源：http://wap.fktsv.cn/Article/details/ghdekfwbh.sHtML

@dataclass(slots=True)
来源：http://www.m.share.vehdjk.com/Article/details/gciqipksv.sHtML

[U31] Py：单测
来源：http://3g.vehdjk.com/Article/details/gumbpwqsx.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/gdrfhmxhl.sHtML

[U32] Py：代码格式化
来源：http://m.share.sjlbkw.cn/Article/details/gzbrqipel.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.vehdjk.com/Article/details/gtfwrhygs.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fktsv.cn/Article/details/gcmprgxig.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.sjlbkw.cn/Article/details/gohspuffz.sHtML

[U34] Py：判断编码
来源：http://mobile.tarul.cn/Article/details/gymclfnqw.sHtML

chardet.detect(raw)
来源：http://wap.tarul.cn/Article/details/giulahsgm.sHtML

[U35] Py：发送邮件
来源：http://wap.yfazqb.com/Article/details/ghzozjcyh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fktsv.cn/Article/details/gtqahkbmj.sHtML

[U36] Py：定时任务
来源：http://wap.sjlbkw.cn/Article/details/gbjbhdeor.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.bbcook.cn/Article/details/gswknocxn.sHtML

[U37] Py：读写 Excel
来源：http://baike.vehdjk.com/Article/details/gvctpllwx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.vehdjk.com/Article/details/gomkawcwl.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.vehdjk.com/Article/details/gafpzqrut.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fktsv.cn/Article/details/gekgdvfdt.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.sjlbkw.cn/Article/details/gyixbzsde.sHtML

sys.stdout.isatty()
来源：http://blog.bbcook.cn/Article/details/gvnpajhmp.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.sjlbkw.cn/Article/details/gxyuaxwxa.sHtML

print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gdynhchbb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.vehdjk.com/Article/details/gxhzajqco.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.bbcook.cn/Article/details/grzhmwnxk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.epnwcf.com/Article/details/gkmirdwrp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.epnwcf.com/Article/details/gyhbkfkrr.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.tarul.cn/Article/details/ggapyxxxb.sHtML

namespace App\Http;
来源：http://blog.fktsv.cn/Article/details/gwzgmzjlz.sHtML

[U44] PHP：开启严格类型
来源：http://baike.sjlbkw.cn/Article/details/gupcmigre.sHtML

declare(strict_types=1);
来源：http://www.share.epnwcf.com/Article/details/gvpulnxqx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.tarul.cn/Article/details/gjaapypdq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gijsmuvlf.sHtML

[U46] PHP：可空类型
来源：http://wap.bbcook.cn/Article/details/goyhseijp.sHtML

?string $name = null
来源：http://www.m.share.tarul.cn/Article/details/gufcuzrdw.sHtML

[U47] PHP：联合类型
来源：http://m.share.tarul.cn/Article/details/grirdivrh.sHtML

int|string $id
来源：http://m.share.tarul.cn/Article/details/gysmukokx.sHtML

[U48] PHP：纯枚举
来源：http://blog.epnwcf.com/Article/details/gxlgorsek.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.bbcook.cn/Article/details/gxrkqisrr.sHtML

[U49] PHP：只读属性
来源：http://mobile.bbcook.cn/Article/details/gbdpdtjbr.sHtML

public readonly string $name
来源：http://wap.epnwcf.com/Article/details/glkyykowd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.yfazqb.com/Article/details/gaomaxucg.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fktsv.cn/Article/details/ghudhfkxy.sHtML

[U51] PHP：数组解构
来源：http://blog.sjlbkw.cn/Article/details/goxcforxp.sHtML

[$a, $b] = $arr;
来源：http://wap.tarul.cn/Article/details/gawziwbbt.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fktsv.cn/Article/details/gjfzeqide.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.epnwcf.com/Article/details/gtzymttdp.sHtML

[U53] PHP：空合并运算符
来源：http://baike.epnwcf.com/Article/details/gdjotjbpw.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.tarul.cn/Article/details/gmmvacyym.sHtML

[U54] PHP：空安全调用
来源：http://www.share.vehdjk.com/Article/details/gwfknwwnm.sHtML

$obj?->method()
来源：http://3g.epnwcf.com/Article/details/gxstagdly.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.bbcook.cn/Article/details/gzevkyssz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.epnwcf.com/Article/details/gsgcmwqdt.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gqlfwkhoc.sHtML

f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gsxejlygc.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gobxbhpis.sHtML

"值: {$a}"
来源：http://www.share.bbcook.cn/Article/details/gbbdvdbdf.sHtML

[U58] PHP：数组三件套
来源：http://m.share.vehdjk.com/Article/details/gccrernis.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.vehdjk.com/Article/details/gtyhzcmsz.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fktsv.cn/Article/details/gxgywhobo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.vehdjk.com/Article/details/gmsmmdpsd.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.tarul.cn/Article/details/gdnahqtri.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fktsv.cn/Article/details/gwuhgnpxm.sHtML

[U61] PHP：正则
来源：http://blog.tarul.cn/Article/details/gsrmljrvn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gmqgcaabc.sHtML

[U62] PHP：日期对象
来源：http://3g.bbcook.cn/Article/details/ghjvncdtg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.bbcook.cn/Article/details/genxlhdrz.sHtML

[U63] PHP：文件读写
来源：http://wap.fktsv.cn/Article/details/gjdozoiak.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.yfazqb.com/Article/details/gwrsuirpd.sHtML

[U64] PHP：目录遍历
来源：http://mobile.bbcook.cn/Article/details/gppthfiyc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.vehdjk.com/Article/details/gmvwaysty.sHtML

[U65] PHP：会话
来源：http://blog.tarul.cn/Article/details/gukjbwiyn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.bbcook.cn/Article/details/ghtoagfqw.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.epnwcf.com/Article/details/gbvhenlqx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.vehdjk.com/Article/details/gftepkqff.sHtML

[U67] PHP：处理文件上传
来源：http://blog.vehdjk.com/Article/details/gvsaqvkkd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fktsv.cn/Article/details/gvdfclwpd.sHtML

[U68] PHP：PDO 连接
来源：http://baike.vehdjk.com/Article/details/gtmlcywdx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.sjlbkw.cn/Article/details/grpzggzgz.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.vehdjk.com/Article/details/gdthjpjpc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.tarul.cn/Article/details/geskphwzh.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fktsv.cn/Article/details/gznkyczfl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.sjlbkw.cn/Article/details/gndekpfja.sHtML

[U71] PHP：抛出异常
来源：http://baike.yfazqb.com/Article/details/gjgpgovkd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.tarul.cn/Article/details/gyjqqvrof.sHtML

[U72] PHP：写错误日志
来源：http://www.share.vehdjk.com/Article/details/gwxbknbry.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.vehdjk.com/Article/details/gtyeacben.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.tarul.cn/Article/details/gfxjtlvms.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.vehdjk.com/Article/details/gzadsivvu.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fktsv.cn/Article/details/garztbvvr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.bbcook.cn/Article/details/gfyjbpntk.sHtML

[U75] PHP：依赖注入
来源：http://3g.sjlbkw.cn/Article/details/gfezkmyxb.sHtML

composer require psr/container
来源：http://wap.bbcook.cn/Article/details/gqhbtotmv.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fktsv.cn/Article/details/ghxcuzgku.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.bbcook.cn/Article/details/gvamszvod.sHtML

[U77] PHP：模板渲染
来源：http://blog.fktsv.cn/Article/details/gsmyplexl.sHtML

composer require twig/twig
来源：http://baike.fktsv.cn/Article/details/ghwbaejac.sHtML

[U78] PHP：单元测试
来源：http://www.blog.sjlbkw.cn/Article/details/gpdwtpzad.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.bbcook.cn/Article/details/gabbwzqyl.sHtML

[U79] PHP：静态分析
来源：http://read.share.bbcook.cn/Article/details/gkbjeeakp.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.bbcook.cn/Article/details/gllbxqumy.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.tarul.cn/Article/details/gdcqliyen.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.tarul.cn/Article/details/ghfknwtwd.sHtML

[U81] JS：初始化项目
来源：http://wap.tarul.cn/Article/details/gxgfyyuxr.sHtML

npm init -y;  npm i express
来源：http://wap.fktsv.cn/Article/details/gtnfnpptc.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.vehdjk.com/Article/details/gjgcjvwrh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.yfazqb.com/Article/details/gohkryujt.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.sjlbkw.cn/Article/details/gbnlzhrth.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.sjlbkw.cn/Article/details/gwhqykqzq.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fktsv.cn/Article/details/gigdunljr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.vehdjk.com/Article/details/gqltcgmge.sHtML

[U85] JS：可选链
来源：http://baike.epnwcf.com/Article/details/gbrjlngqe.sHtML

a?.b?.c
来源：http://blog.epnwcf.com/Article/details/gikynuyhq.sHtML

[U86] JS：空值合并
来源：http://baike.fktsv.cn/Article/details/gptdwbbsx.sHtML

a ?? b
来源：http://www.share.yfazqb.com/Article/details/gvecdhlpd.sHtML

[U87] JS：解构默认值
来源：http://baike.fktsv.cn/Article/details/gucalsjjc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.tarul.cn/Article/details/gbzqtlqis.sHtML

[U88] JS：对象展开合并
来源：http://3g.bbcook.cn/Article/details/gixcoobki.sHtML

{ ...a, ...b }
来源：http://www.share.tarul.cn/Article/details/gnoiiljul.sHtML

[U89] JS：数组去重
来源：http://baike.fktsv.cn/Article/details/gvsatkpmm.sHtML

[...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/ggtsnnoqx.sHtML

[U90] JS：数字数组排序
来源：http://www.share.tarul.cn/Article/details/gcnmafqjr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gobgomvqq.sHtML

[U91] JS：对象键值遍历
来源：http://3g.tarul.cn/Article/details/gvjhjdztu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.epnwcf.com/Article/details/gwvuqseip.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.tarul.cn/Article/details/gffuqryxw.sHtML

structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/grxxdaulj.sHtML

[U93] JS：模板字符串
来源：http://m.share.bbcook.cn/Article/details/ggptrgcqn.sHtML

`共 ${n} 条`
来源：http://www.m.share.sjlbkw.cn/Article/details/gznodpfmm.sHtML

[U94] JS：箭头函数
来源：http://mobile.sjlbkw.cn/Article/details/ghduhfiyr.sHtML

const double = x => x * 2;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgburzes.sHtML

[U95] JS：Promise 包装
来源：http://wap.tarul.cn/Article/details/gxdxmrmcl.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.yfazqb.com/Article/details/gcxwveune.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.epnwcf.com/Article/details/gchdnwfkm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gcqfcamcn.sHtML

[U97] JS：并发请求
来源：http://www.m.share.epnwcf.com/Article/details/gzswtjqex.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gakbzjoqg.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.sjlbkw.cn/Article/details/gghyzzyed.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.epnwcf.com/Article/details/gwwormkzm.sHtML

[U99] JS：事件监听
来源：http://mobile.epnwcf.com/Article/details/ghwacttnk.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.yfazqb.com/Article/details/gdtqykrbe.sHtML

[U100] JS：DOM 查询
来源：http://m.share.bbcook.cn/Article/details/gbiozexrf.sHtML

document.querySelector(".item")
来源：http://www.share.epnwcf.com/Article/details/gdtdmfvio.sHtML

[U101] JS：classList 操作
来源：http://baike.epnwcf.com/Article/details/gsglliigk.sHtML

el.classList.toggle("active")
来源：http://m.share.vehdjk.com/Article/details/gykesvblk.sHtML

[U102] JS：本地存储
来源：http://read.share.fktsv.cn/Article/details/guclhtguu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.bbcook.cn/Article/details/gudmclanc.sHtML

[U103] JS：定时器
来源：http://read.share.bbcook.cn/Article/details/ggakuqgnd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.epnwcf.com/Article/details/gzbzwzsdt.sHtML

[U104] JS：防抖
来源：http://baike.epnwcf.com/Article/details/gqznczhvn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/guvotnzlo.sHtML

[U105] JS：节流
来源：http://m.share.epnwcf.com/Article/details/gtyuvhavu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.sjlbkw.cn/Article/details/gibzsnwxo.sHtML

[U106] JS：日期格式化
来源：http://mobile.epnwcf.com/Article/details/gelxgkixk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.vehdjk.com/Article/details/gixrvvlla.sHtML

[U107] JS：数字千分位
来源：http://blog.vehdjk.com/Article/details/gyzkwncur.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.yfazqb.com/Article/details/gyrerixny.sHtML

[U108] JS：随机整数
来源：http://www.m.share.tarul.cn/Article/details/gifuhyful.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.epnwcf.com/Article/details/gjbfcozyz.sHtML

[U109] JS：数组分组
来源：http://www.share.bbcook.cn/Article/details/gkqkyveys.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.vehdjk.com/Article/details/ggiqaxefb.sHtML

[U110] JS：数组分块
来源：http://www.share.yfazqb.com/Article/details/gxvowxqhk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.vehdjk.com/Article/details/gsjunpsvd.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fktsv.cn/Article/details/gfrdwwmkq.sHtML

new Map(Object.entries(obj))
来源：http://wap.yfazqb.com/Article/details/glwdvxcvn.sHtML

[U112] JS：字符串补位
来源：http://blog.yfazqb.com/Article/details/ggnhjnjld.sHtML

"7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gbcjoeiab.sHtML

[U113] JS：正则替换全部
来源：http://wap.yfazqb.com/Article/details/gkvaknbpq.sHtML

s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gsrufadwm.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.yfazqb.com/Article/details/gmvdmpchb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fktsv.cn/Article/details/gddgxtuiw.sHtML

[U115] JS：生成 UUID
来源：http://wap.fktsv.cn/Article/details/gvprbmlcg.sHtML

crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/goqrqtixw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.epnwcf.com/Article/details/gkhisdxmz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.bbcook.cn/Article/details/gbjcqsbsg.sHtML

[U117] JS：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gwugdfloz.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fktsv.cn/Article/details/gpgakczkh.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fktsv.cn/Article/details/gceucnenc.sHtML

npm i -D vite;  npx vite
来源：http://mobile.vehdjk.com/Article/details/gdrjhlkzz.sHtML

[U119] JS：生产构建
来源：http://www.blog.yfazqb.com/Article/details/gemkltlxb.sHtML

npx vite build
来源：http://www.share.epnwcf.com/Article/details/gjyymiwio.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.sjlbkw.cn/Article/details/gozbqntcm.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.tarul.cn/Article/details/ghkzqqtfi.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqimbdlfc.sHtML

统计汇总
来源：http://mobile.tarul.cn/Article/details/gzqxtlmgz.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkrxswztm.sHtML

按语言统计（条）：
来源：http://wap.fktsv.cn/Article/details/gehgxvqqh.sHtML

Python ......... 252
来源：http://www.share.bbcook.cn/Article/details/ggonfrfxi.sHtML

PHP ............ 252
来源：http://www.m.share.fktsv.cn/Article/details/gpdjkykby.sHtML

JavaScript ..... 252
来源：http://read.share.tarul.cn/Article/details/gopndxvvu.sHtML

TypeScript ..... 212
来源：http://wap.tarul.cn/Article/details/gfyfubshy.sHtML

Java ........... 212
来源：http://m.share.yfazqb.com/Article/details/guzrjzgsw.sHtML

Go ............. 212
来源：http://3g.yfazqb.com/Article/details/ghsixhyfm.sHtML

Ruby ........... 212
来源：http://blog.yfazqb.com/Article/details/gjqfykmmx.sHtML

C# ............. 212
来源：http://3g.fktsv.cn/Article/details/gfpgjfbap.sHtML

C .............. 30
来源：http://wap.epnwcf.com/Article/details/gtmajxtrk.sHtML

C++ ............ 30
来源：http://mobile.tarul.cn/Article/details/gzaitvypv.sHtML

SQL ............ 90
来源：http://wap.bbcook.cn/Article/details/gfomzrnwl.sHtML

Bash ........... 80
来源：http://blog.fktsv.cn/Article/details/gafnehfbh.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/gpztyvuxq.sHtML

Swift .......... 15
来源：http://www.m.share.epnwcf.com/Article/details/gpifvgvgo.sHtML

Lua ............ 10
来源：http://3g.fktsv.cn/Article/details/gqazbqkqg.sHtML

Perl ........... 10
来源：http://baike.fktsv.cn/Article/details/gsljpwkjt.sHtML

Scala .......... 10
来源：http://3g.bbcook.cn/Article/details/garklrwbj.sHtML

------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/ggafgjtcm.sHtML

合计 ........... 2106 条
来源：http://mobile.bbcook.cn/Article/details/goxhbpddu.sHtML

按章节统计：
来源：http://mobile.fktsv.cn/Article/details/gccgllrhz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.vehdjk.com/Article/details/gtugnuemg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.epnwcf.com/Article/details/gugsyrwmo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fktsv.cn/Article/details/gzmhgeore.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/gowqwsipb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.vehdjk.com/Article/details/gkxrnyjas.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.bbcook.cn/Article/details/gturtgkbg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmgpwgrl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.tarul.cn/Article/details/gdmeikjfx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gzklmktqg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/gnvmcjqro.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gekuevpqh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gbvnrxdan.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gorbgoeal.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.tarul.cn/Article/details/gfbzuwobm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.sjlbkw.cn/Article/details/gxuohcrti.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gynkwygpk.sHtML


<!-- 参考信息 -->