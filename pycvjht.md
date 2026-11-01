代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://blog.bbcook.cn/Article/details/gunxayjbo.sHtML

[T55] Scala：集合过滤
来源：http://blog.fktsv.cn/Article/details/glewmgwdo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.bbcook.cn/Article/details/gtqfwusxz.sHtML

[T56] Scala：样例类
来源：http://www.blog.yfazqb.com/Article/details/goyxtgkct.sHtML

case class User(name: String, age: Int)
来源：http://m.share.tarul.cn/Article/details/gduibkscx.sHtML

[T57] Scala：模式匹配
来源：http://wap.tarul.cn/Article/details/gedjatotd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.sjlbkw.cn/Article/details/gexakyfqo.sHtML

[T58] Scala：函数定义
来源：http://www.share.fktsv.cn/Article/details/gerlwuyeb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.tarul.cn/Article/details/glrouwxwz.sHtML

[T59] Scala：循环
来源：http://blog.epnwcf.com/Article/details/gqursdqqm.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fktsv.cn/Article/details/gblquoyvf.sHtML

[T60] Scala：折叠
来源：http://www.blog.yfazqb.com/Article/details/gtbesglbg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.yfazqb.com/Article/details/gjbmxzlxc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwnlayonb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.bbcook.cn/Article/details/gsiyirsoy.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjgirpmod.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.vehdjk.com/Article/details/gihqalveq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.yfazqb.com/Article/details/glvyabvsx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.sjlbkw.cn/Article/details/gtcdwpxul.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.yfazqb.com/Article/details/gixfbilne.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.sjlbkw.cn/Article/details/gzqvnefso.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.epnwcf.com/Article/details/gwalgbihj.sHtML

[U04] Py：变量调试打印
来源：http://mobile.tarul.cn/Article/details/gbqfbdfnq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.tarul.cn/Article/details/gomxffdvr.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.yfazqb.com/Article/details/gkhksrzcy.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/gnjrchphr.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.bbcook.cn/Article/details/grttucxps.sHtML

{**a, **b}
来源：http://www.blog.fktsv.cn/Article/details/gepbivhac.sHtML

[U07] Py：反转字典键值
来源：http://www.share.vehdjk.com/Article/details/gavwmqlab.sHtML

{v: k for k, v in d.items()}
来源：http://baike.epnwcf.com/Article/details/glkpumaof.sHtML

[U08] Py：展平二维列表
来源：http://baike.yfazqb.com/Article/details/gghtqdgng.sHtML

[y for x in nested for y in x]
来源：http://baike.epnwcf.com/Article/details/gimikkrwv.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.sjlbkw.cn/Article/details/gihmzrmrp.sHtML

max(d, key=d.get)
来源：http://blog.tarul.cn/Article/details/gscfqkkjo.sHtML

[U10] Py：按值排序字典
来源：http://baike.tarul.cn/Article/details/gxtqnttsm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.tarul.cn/Article/details/gisjykhvy.sHtML

[U11] Py：生成器表达式
来源：http://baike.vehdjk.com/Article/details/grqybdhws.sHtML

(x * 2 for x in arr)
来源：http://wap.fktsv.cn/Article/details/gicqmytzl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fktsv.cn/Article/details/gcxgmtesh.sHtML

Counter(arr).most_common(3)
来源：http://wap.sjlbkw.cn/Article/details/gyzwgkqqh.sHtML

[U13] Py：固定长度队列
来源：http://m.share.epnwcf.com/Article/details/ggswsllmg.sHtML

deque(maxlen=10)
来源：http://3g.vehdjk.com/Article/details/gcrzlqvwz.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.sjlbkw.cn/Article/details/gkyrvycai.sHtML

defaultdict(list)
来源：http://3g.sjlbkw.cn/Article/details/gerzneefg.sHtML

[U15] Py：高精度计时
来源：http://m.share.bbcook.cn/Article/details/gllttezna.sHtML

t = time.perf_counter()
来源：http://www.share.sjlbkw.cn/Article/details/gezyuxbqj.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fktsv.cn/Article/details/gkziugirj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fktsv.cn/Article/details/gaurviykx.sHtML

[U17] Py：初始化日志
来源：http://read.share.yfazqb.com/Article/details/gozwzsgvu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.epnwcf.com/Article/details/ghghhlqtb.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fktsv.cn/Article/details/gpmhyhivi.sHtML

pat = re.compile(r"\d+")
来源：http://blog.vehdjk.com/Article/details/goshskiim.sHtML

[U19] Py：正则替换带回调
来源：http://blog.vehdjk.com/Article/details/ggxpbwvnw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.yfazqb.com/Article/details/ggurgmwjs.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.vehdjk.com/Article/details/gergnlncx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.tarul.cn/Article/details/gbdcwtlsc.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.yfazqb.com/Article/details/gneifymjc.sHtML

@contextlib.contextmanager
来源：http://m.share.sjlbkw.cn/Article/details/gyetvecnt.sHtML

[U22] Py：矩阵转置
来源：http://read.share.sjlbkw.cn/Article/details/gleywkcng.sHtML

list(zip(*m))
来源：http://wap.tarul.cn/Article/details/gfhornxkx.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fktsv.cn/Article/details/gdrorssnk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.tarul.cn/Article/details/gtuhrqoey.sHtML

[U24] Py：路径操作
来源：http://www.blog.fktsv.cn/Article/details/gqtlbogqs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/glubkilzo.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/gvrzurgnu.sHtML

csv.DictReader(f)
来源：http://www.blog.epnwcf.com/Article/details/gaatakfhn.sHtML

[U26] Py：并发下载
来源：http://3g.tarul.cn/Article/details/gcglqkfub.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fktsv.cn/Article/details/gkgpbthez.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.epnwcf.com/Article/details/gphrswimv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.bbcook.cn/Article/details/gxecfoffz.sHtML

[U28] Py：类型别名
来源：http://wap.epnwcf.com/Article/details/getbuxoql.sHtML

UserId = int
来源：http://wap.epnwcf.com/Article/details/gmzoaoxea.sHtML

[U29] Py：属性校验
来源：http://read.share.yfazqb.com/Article/details/gdsrihgfc.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fktsv.cn/Article/details/gqemmdmjv.sHtML

[U30] Py：数据类
来源：http://blog.vehdjk.com/Article/details/gywvgjwvq.sHtML

@dataclass(slots=True)
来源：http://m.share.tarul.cn/Article/details/gtjsmxqvf.sHtML

[U31] Py：单测
来源：http://baike.bbcook.cn/Article/details/gqhubqmpz.sHtML

python -m pytest -q
来源：http://m.share.vehdjk.com/Article/details/gdjmagbmk.sHtML

[U32] Py：代码格式化
来源：http://3g.fktsv.cn/Article/details/gsmciesne.sHtML

ruff format . && ruff check --fix .
来源：http://3g.tarul.cn/Article/details/gtvlikmqc.sHtML

[U33] Py：打包发布
来源：http://blog.epnwcf.com/Article/details/gpvgwklmq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.tarul.cn/Article/details/gkpznlyzi.sHtML

[U34] Py：判断编码
来源：http://m.share.epnwcf.com/Article/details/gtezqxllz.sHtML

chardet.detect(raw)
来源：http://3g.bbcook.cn/Article/details/gjswqmtyf.sHtML

[U35] Py：发送邮件
来源：http://baike.sjlbkw.cn/Article/details/gitoxirsx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.epnwcf.com/Article/details/gaqustiqi.sHtML

[U36] Py：定时任务
来源：http://baike.tarul.cn/Article/details/gszhcybyd.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.sjlbkw.cn/Article/details/gstmzlnlu.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.epnwcf.com/Article/details/ggvckqlsf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.bbcook.cn/Article/details/gwleisshs.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.bbcook.cn/Article/details/gtdxitajq.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fktsv.cn/Article/details/gcmzscxnz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gilkawdgs.sHtML

sys.stdout.isatty()
来源：http://read.share.bbcook.cn/Article/details/gqetousvq.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.vehdjk.com/Article/details/gypmmjcon.sHtML

print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/grrssrypf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.tarul.cn/Article/details/gqocgekdt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.sjlbkw.cn/Article/details/ghsarhois.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.yfazqb.com/Article/details/gsjigcsrf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fktsv.cn/Article/details/gxuxupnog.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.sjlbkw.cn/Article/details/giyjuwdlo.sHtML

namespace App\Http;
来源：http://m.share.bbcook.cn/Article/details/gobfqkail.sHtML

[U44] PHP：开启严格类型
来源：http://3g.sjlbkw.cn/Article/details/gmdsljiun.sHtML

declare(strict_types=1);
来源：http://wap.fktsv.cn/Article/details/gteuufokc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.epnwcf.com/Article/details/gbnfhjzat.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gsybrnekt.sHtML

[U46] PHP：可空类型
来源：http://wap.yfazqb.com/Article/details/glhueghaz.sHtML

?string $name = null
来源：http://wap.tarul.cn/Article/details/gblgbmktj.sHtML

[U47] PHP：联合类型
来源：http://read.share.sjlbkw.cn/Article/details/gxlifhayt.sHtML

int|string $id
来源：http://wap.epnwcf.com/Article/details/gkfetzlgs.sHtML

[U48] PHP：纯枚举
来源：http://www.share.epnwcf.com/Article/details/gqpgkewzk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fktsv.cn/Article/details/gffzuddja.sHtML

[U49] PHP：只读属性
来源：http://mobile.fktsv.cn/Article/details/gchjmthrf.sHtML

public readonly string $name
来源：http://3g.bbcook.cn/Article/details/ghtmieqod.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.tarul.cn/Article/details/gludaikoz.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fktsv.cn/Article/details/gzkscilwc.sHtML

[U51] PHP：数组解构
来源：http://www.share.vehdjk.com/Article/details/gtuwnyptk.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.bbcook.cn/Article/details/gvuiusvzn.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gvouoaboi.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.yfazqb.com/Article/details/gfppxazoh.sHtML

[U53] PHP：空合并运算符
来源：http://baike.vehdjk.com/Article/details/gmbsbqhlm.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.tarul.cn/Article/details/gksmnvrbn.sHtML

[U54] PHP：空安全调用
来源：http://mobile.sjlbkw.cn/Article/details/gdmmierqn.sHtML

$obj?->method()
来源：http://wap.epnwcf.com/Article/details/gxqrverrx.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fktsv.cn/Article/details/gfmtudxyn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.vehdjk.com/Article/details/gtcsfzxbx.sHtML

[U56] PHP：命名参数
来源：http://baike.yfazqb.com/Article/details/gzryzvpfy.sHtML

f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gggsdstod.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/ghzciqhyr.sHtML

"值: {$a}"
来源：http://baike.tarul.cn/Article/details/gsuibqtkw.sHtML

[U58] PHP：数组三件套
来源：http://read.share.vehdjk.com/Article/details/ggcdazssd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.bbcook.cn/Article/details/gphyjocjb.sHtML

[U59] PHP：自定义排序
来源：http://mobile.bbcook.cn/Article/details/gurzhtrnu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/gzzkxinaz.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fktsv.cn/Article/details/gmiskbmiz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.tarul.cn/Article/details/gyclrjjeo.sHtML

[U61] PHP：正则
来源：http://mobile.tarul.cn/Article/details/goajbhrbp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/grdbbatza.sHtML

[U62] PHP：日期对象
来源：http://www.share.sjlbkw.cn/Article/details/gewszyxlo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.bbcook.cn/Article/details/gdpabeeyw.sHtML

[U63] PHP：文件读写
来源：http://3g.tarul.cn/Article/details/gkkbgfxpr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.bbcook.cn/Article/details/gsfeuzcxt.sHtML

[U64] PHP：目录遍历
来源：http://www.share.vehdjk.com/Article/details/gejfphpyn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.yfazqb.com/Article/details/gfjbnygmx.sHtML

[U65] PHP：会话
来源：http://www.share.bbcook.cn/Article/details/gsebulijp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.vehdjk.com/Article/details/grngghgsu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.vehdjk.com/Article/details/grtadmouc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.yfazqb.com/Article/details/gqdpvtsko.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fktsv.cn/Article/details/gbmwemnlz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.bbcook.cn/Article/details/gipfsolbo.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fktsv.cn/Article/details/gxowfirdb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.tarul.cn/Article/details/gwdmbefeb.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.bbcook.cn/Article/details/gxrurnsmz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.bbcook.cn/Article/details/gaeacdbhf.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.bbcook.cn/Article/details/gyyoyxpdx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.tarul.cn/Article/details/geieylnxb.sHtML

[U71] PHP：抛出异常
来源：http://3g.vehdjk.com/Article/details/gidnvbwci.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.sjlbkw.cn/Article/details/gnmbcpgkv.sHtML

[U72] PHP：写错误日志
来源：http://read.share.yfazqb.com/Article/details/glfkcafer.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.epnwcf.com/Article/details/gcealvuvh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.yfazqb.com/Article/details/gkeplllgn.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.yfazqb.com/Article/details/gqgehylfl.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gqpwhntdk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.tarul.cn/Article/details/gbxuqhcpi.sHtML

[U75] PHP：依赖注入
来源：http://www.share.bbcook.cn/Article/details/gaufjtekk.sHtML

composer require psr/container
来源：http://wap.epnwcf.com/Article/details/gicwncxpa.sHtML

[U76] PHP：简单路由
来源：http://mobile.fktsv.cn/Article/details/gblkfhbzv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.yfazqb.com/Article/details/gnabsnyyk.sHtML

[U77] PHP：模板渲染
来源：http://read.share.vehdjk.com/Article/details/gcademeyv.sHtML

composer require twig/twig
来源：http://wap.vehdjk.com/Article/details/gybmcmbrz.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.yfazqb.com/Article/details/gbzkjpoto.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.yfazqb.com/Article/details/glepkrypk.sHtML

[U79] PHP：静态分析
来源：http://baike.sjlbkw.cn/Article/details/gprjluivt.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.bbcook.cn/Article/details/gslmevwmt.sHtML

[U80] PHP：代码规范修复
来源：http://wap.yfazqb.com/Article/details/gzxsqucpk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.bbcook.cn/Article/details/gjqkkztpd.sHtML

[U81] JS：初始化项目
来源：http://www.share.vehdjk.com/Article/details/gnwryidps.sHtML

npm init -y;  npm i express
来源：http://baike.sjlbkw.cn/Article/details/gnykhgeuo.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.bbcook.cn/Article/details/gakolcjfj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.yfazqb.com/Article/details/gnozzzpux.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.bbcook.cn/Article/details/gzimtunqj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.bbcook.cn/Article/details/gaoiqptmg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fktsv.cn/Article/details/gupbnxkoo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.bbcook.cn/Article/details/gesbecegm.sHtML

[U85] JS：可选链
来源：http://read.share.epnwcf.com/Article/details/gzudueipm.sHtML

a?.b?.c
来源：http://m.share.bbcook.cn/Article/details/ggyomltov.sHtML

[U86] JS：空值合并
来源：http://wap.tarul.cn/Article/details/gctgoydzl.sHtML

a ?? b
来源：http://read.share.sjlbkw.cn/Article/details/gfmgkexpj.sHtML

[U87] JS：解构默认值
来源：http://read.share.epnwcf.com/Article/details/gvqyirgso.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.tarul.cn/Article/details/gwwfphdjw.sHtML

[U88] JS：对象展开合并
来源：http://mobile.bbcook.cn/Article/details/gfaouujdo.sHtML

{ ...a, ...b }
来源：http://baike.fktsv.cn/Article/details/gquncfczr.sHtML

[U89] JS：数组去重
来源：http://3g.bbcook.cn/Article/details/gxsqywizo.sHtML

[...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gulgolcgc.sHtML

[U90] JS：数字数组排序
来源：http://www.share.tarul.cn/Article/details/gabvidwsh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gkdswyqsr.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.yfazqb.com/Article/details/grdrgulph.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.epnwcf.com/Article/details/gaeewbziy.sHtML

[U92] JS：深拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gnhwroplb.sHtML

structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gfalpcgsv.sHtML

[U93] JS：模板字符串
来源：http://www.share.bbcook.cn/Article/details/gpldjapbp.sHtML

`共 ${n} 条`
来源：http://mobile.epnwcf.com/Article/details/gcompgyoo.sHtML

[U94] JS：箭头函数
来源：http://m.share.fktsv.cn/Article/details/gkrjldidv.sHtML

const double = x => x * 2;
来源：http://read.share.bbcook.cn/Article/details/gfrxfybwe.sHtML

[U95] JS：Promise 包装
来源：http://mobile.epnwcf.com/Article/details/gonijtbey.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.sjlbkw.cn/Article/details/geelsbaax.sHtML

[U96] JS：async/await 与异常
来源：http://wap.epnwcf.com/Article/details/gjpqutnwq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gxcrwcvka.sHtML

[U97] JS：并发请求
来源：http://baike.bbcook.cn/Article/details/gvrjmmsdk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gfargecja.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.vehdjk.com/Article/details/gyvfqhjkb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.yfazqb.com/Article/details/gabsylqof.sHtML

[U99] JS：事件监听
来源：http://www.share.fktsv.cn/Article/details/gammkggwz.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.epnwcf.com/Article/details/gqpmszkdw.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.epnwcf.com/Article/details/gzfxjkooh.sHtML

document.querySelector(".item")
来源：http://read.share.bbcook.cn/Article/details/gjlpfauig.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.vehdjk.com/Article/details/giatqrsbp.sHtML

el.classList.toggle("active")
来源：http://www.m.share.epnwcf.com/Article/details/gvzbcwsik.sHtML

[U102] JS：本地存储
来源：http://www.share.vehdjk.com/Article/details/gqhkdmycg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.bbcook.cn/Article/details/gnahansqc.sHtML

[U103] JS：定时器
来源：http://3g.tarul.cn/Article/details/guonxuojx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.vehdjk.com/Article/details/gtdmlxcua.sHtML

[U104] JS：防抖
来源：http://wap.bbcook.cn/Article/details/gbprvlpvj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/glkaafecl.sHtML

[U105] JS：节流
来源：http://m.share.bbcook.cn/Article/details/gxlkyxtij.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.tarul.cn/Article/details/guavisioh.sHtML

[U106] JS：日期格式化
来源：http://blog.bbcook.cn/Article/details/gykeegmxm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.yfazqb.com/Article/details/ghhygzzop.sHtML

[U107] JS：数字千分位
来源：http://m.share.fktsv.cn/Article/details/gehqoittc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fktsv.cn/Article/details/gapupawab.sHtML

[U108] JS：随机整数
来源：http://mobile.yfazqb.com/Article/details/gxvtkrfwk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmbzzejh.sHtML

[U109] JS：数组分组
来源：http://baike.epnwcf.com/Article/details/gyticpcln.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fktsv.cn/Article/details/gxczxkzrt.sHtML

[U110] JS：数组分块
来源：http://mobile.sjlbkw.cn/Article/details/gxperazny.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.tarul.cn/Article/details/gatoylqdv.sHtML

[U111] JS：对象转 Map
来源：http://wap.tarul.cn/Article/details/glshzkxsv.sHtML

new Map(Object.entries(obj))
来源：http://blog.yfazqb.com/Article/details/gxbzsmjhs.sHtML

[U112] JS：字符串补位
来源：http://mobile.vehdjk.com/Article/details/gkdxatnaw.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gnxtwkxly.sHtML

[U113] JS：正则替换全部
来源：http://read.share.vehdjk.com/Article/details/gprncgmgj.sHtML

s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gizxciwiu.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.yfazqb.com/Article/details/glmltiepf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpedelozp.sHtML

[U115] JS：生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gjzicfstb.sHtML

crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gonitekse.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.yfazqb.com/Article/details/gqzytjaaj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.vehdjk.com/Article/details/gnthcolwl.sHtML

[U117] JS：单元测试
来源：http://wap.tarul.cn/Article/details/gvehztbjj.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fktsv.cn/Article/details/gajyfawrp.sHtML

[U118] JS：开发服务器
来源：http://www.share.tarul.cn/Article/details/gpiarzxmy.sHtML

npm i -D vite;  npx vite
来源：http://baike.vehdjk.com/Article/details/gqbheerpl.sHtML

[U119] JS：生产构建
来源：http://www.blog.epnwcf.com/Article/details/gjyklbayc.sHtML

npx vite build
来源：http://m.share.yfazqb.com/Article/details/gklmmpwxg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.bbcook.cn/Article/details/gmrkoxjsx.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.sjlbkw.cn/Article/details/gfgajnomf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmtfvlzbf.sHtML

统计汇总
来源：http://www.m.share.yfazqb.com/Article/details/gkllbgbsu.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ghwpoxxrh.sHtML

按语言统计（条）：
来源：http://mobile.yfazqb.com/Article/details/gqhnefqsh.sHtML

Python ......... 252
来源：http://m.share.vehdjk.com/Article/details/ggdqxxfhn.sHtML

PHP ............ 252
来源：http://www.blog.epnwcf.com/Article/details/guceqysgp.sHtML

JavaScript ..... 252
来源：http://blog.bbcook.cn/Article/details/gkormbxmd.sHtML

TypeScript ..... 212
来源：http://www.blog.bbcook.cn/Article/details/gimznhbnn.sHtML

Java ........... 212
来源：http://www.blog.epnwcf.com/Article/details/gilkspgvo.sHtML

Go ............. 212
来源：http://baike.epnwcf.com/Article/details/gfdwaxfpz.sHtML

Ruby ........... 212
来源：http://wap.fktsv.cn/Article/details/gyzdszosg.sHtML

C# ............. 212
来源：http://blog.fktsv.cn/Article/details/gtsbiubwb.sHtML

C .............. 30
来源：http://read.share.sjlbkw.cn/Article/details/gnmmhmrjm.sHtML

C++ ............ 30
来源：http://www.m.share.tarul.cn/Article/details/gipnhgwfo.sHtML

SQL ............ 90
来源：http://blog.tarul.cn/Article/details/gronrzrkt.sHtML

Bash ........... 80
来源：http://blog.sjlbkw.cn/Article/details/gsjpsiaml.sHtML

Kotlin ......... 15
来源：http://m.share.tarul.cn/Article/details/ggkxkqkun.sHtML

Swift .......... 15
来源：http://www.m.share.yfazqb.com/Article/details/gzpjczxme.sHtML

Lua ............ 10
来源：http://www.share.vehdjk.com/Article/details/gbglzhmip.sHtML

Perl ........... 10
来源：http://mobile.tarul.cn/Article/details/gqqfyeqvq.sHtML

Scala .......... 10
来源：http://baike.yfazqb.com/Article/details/gzvivrofl.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gmhtjqejk.sHtML

合计 ........... 2106 条
来源：http://read.share.epnwcf.com/Article/details/gxoovlext.sHtML

按章节统计：
来源：http://mobile.epnwcf.com/Article/details/gzdhxxpsp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/gzjwtiakh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/glkghbbsg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gtmvzmobh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.vehdjk.com/Article/details/gnbffbfpx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.yfazqb.com/Article/details/ggrgcbfcf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.sjlbkw.cn/Article/details/grwagmmke.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/ggdkjyckx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.yfazqb.com/Article/details/gjbxglggk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gsjhtfxep.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/gctmwzgiu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gaxihjzeg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/ghdxqunxy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gqkyvkiaw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.yfazqb.com/Article/details/glhbailrp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkhbcmdx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gikhaxtzm.sHtML

Q SQL 专题                              90
来源：http://www.blog.epnwcf.com/Article/details/gzvvinokh.sHtML

R Bash 专题                             80
来源：http://m.share.tarul.cn/Article/details/gwycawtki.sHtML

S C / C++ 专题                          60
来源：http://read.share.tarul.cn/Article/details/gewcioofa.sHtML

T 其他语言补充                          60
来源：http://3g.bbcook.cn/Article/details/gcurxkgyt.sHtML


<!-- 参考信息 -->