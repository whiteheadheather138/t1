代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://3g.epnwcf.com/Article/details/gnnrzfgzf.sHtML

[T51] Scala：Hello World
来源：http://m.share.epnwcf.com/Article/details/gscrisqsl.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gijunoiiq.sHtML

[T52] Scala：变量
来源：http://www.m.share.yfazqb.com/Article/details/gkivvvmwf.sHtML

val a = 1;  var b = 2
来源：http://www.blog.tarul.cn/Article/details/gpcorvijd.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gkgdtzjxb.sHtML

s"值: $b"
来源：http://wap.fktsv.cn/Article/details/gngzvmvzw.sHtML

[T54] Scala：集合映射
来源：http://blog.bbcook.cn/Article/details/gfpeeuapk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.epnwcf.com/Article/details/gbqpxdhtl.sHtML

[T55] Scala：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/gkfofwabi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.tarul.cn/Article/details/gvfxwxndc.sHtML

[T56] Scala：样例类
来源：http://www.share.yfazqb.com/Article/details/gaodvxeha.sHtML

case class User(name: String, age: Int)
来源：http://baike.tarul.cn/Article/details/gcxbbetre.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fktsv.cn/Article/details/gbkxsqmtb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.yfazqb.com/Article/details/guziexugg.sHtML

[T58] Scala：函数定义
来源：http://www.share.vehdjk.com/Article/details/ghqvgnjtr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fktsv.cn/Article/details/gzgoszwnz.sHtML

[T59] Scala：循环
来源：http://www.share.sjlbkw.cn/Article/details/grlmvcgfq.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.tarul.cn/Article/details/gtqofesds.sHtML

[T60] Scala：折叠
来源：http://3g.epnwcf.com/Article/details/gyvhcadey.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.sjlbkw.cn/Article/details/guayxcnsm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gwzpchlfx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/gsjerpvmd.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmpprdxbp.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.vehdjk.com/Article/details/gfyvfykvx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.tarul.cn/Article/details/gpkwsllba.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.tarul.cn/Article/details/gbgoighwr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fktsv.cn/Article/details/gmiszkqst.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.tarul.cn/Article/details/ghjmbumyd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.tarul.cn/Article/details/gjjmwhnqz.sHtML

[U04] Py：变量调试打印
来源：http://mobile.bbcook.cn/Article/details/gomzndzqq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.epnwcf.com/Article/details/gzuupgsmp.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.tarul.cn/Article/details/gpidydakg.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fktsv.cn/Article/details/glndvhbkb.sHtML

[U06] Py：合并两个字典
来源：http://3g.tarul.cn/Article/details/gepjnbrdg.sHtML

{**a, **b}
来源：http://baike.yfazqb.com/Article/details/ghhjskdsw.sHtML

[U07] Py：反转字典键值
来源：http://m.share.tarul.cn/Article/details/grxoepinj.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fktsv.cn/Article/details/gmkmprrvv.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.yfazqb.com/Article/details/gsixvlgru.sHtML

[y for x in nested for y in x]
来源：http://baike.tarul.cn/Article/details/gqsphjajf.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.sjlbkw.cn/Article/details/geqlwcbfm.sHtML

max(d, key=d.get)
来源：http://mobile.tarul.cn/Article/details/gfdfkhtzj.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fktsv.cn/Article/details/gyfrpdyun.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.vehdjk.com/Article/details/gqbpzwdnn.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fktsv.cn/Article/details/grlvvnojh.sHtML

(x * 2 for x in arr)
来源：http://read.share.epnwcf.com/Article/details/gcioesdke.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.epnwcf.com/Article/details/gylkxtijr.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.tarul.cn/Article/details/gxvzfujqw.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.tarul.cn/Article/details/guepingxp.sHtML

deque(maxlen=10)
来源：http://mobile.sjlbkw.cn/Article/details/gtrofwduw.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.tarul.cn/Article/details/gztdrfyyj.sHtML

defaultdict(list)
来源：http://blog.fktsv.cn/Article/details/grokldtmg.sHtML

[U15] Py：高精度计时
来源：http://www.share.bbcook.cn/Article/details/gcojakmrh.sHtML

t = time.perf_counter()
来源：http://blog.bbcook.cn/Article/details/giubqnmqv.sHtML

[U16] Py：命令行参数解析
来源：http://3g.yfazqb.com/Article/details/gbbhzvrqy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.epnwcf.com/Article/details/gtwtpkvje.sHtML

[U17] Py：初始化日志
来源：http://3g.vehdjk.com/Article/details/gszagysqm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.bbcook.cn/Article/details/gybdidqzy.sHtML

[U18] Py：预编译正则
来源：http://read.share.bbcook.cn/Article/details/gxejybdgu.sHtML

pat = re.compile(r"\d+")
来源：http://3g.tarul.cn/Article/details/gwbueraxq.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fktsv.cn/Article/details/gfpnlywpk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.sjlbkw.cn/Article/details/gphfchpvp.sHtML

[U20] Py：缓存函数结果
来源：http://3g.yfazqb.com/Article/details/gliuldnhf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.bbcook.cn/Article/details/gqjmuckeo.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.tarul.cn/Article/details/ghphrsgma.sHtML

@contextlib.contextmanager
来源：http://www.m.share.sjlbkw.cn/Article/details/ginnuvxae.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.bbcook.cn/Article/details/gfzniugep.sHtML

list(zip(*m))
来源：http://www.m.share.fktsv.cn/Article/details/gbklptnfn.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.epnwcf.com/Article/details/gzcsmislf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.sjlbkw.cn/Article/details/gufqlafff.sHtML

[U24] Py：路径操作
来源：http://wap.sjlbkw.cn/Article/details/gxcltqzeb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gmgxxegim.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fktsv.cn/Article/details/gmqxcnony.sHtML

csv.DictReader(f)
来源：http://wap.bbcook.cn/Article/details/gfwdotkbu.sHtML

[U26] Py：并发下载
来源：http://wap.epnwcf.com/Article/details/gxtyftzlp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fktsv.cn/Article/details/gsnzejjwn.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.tarul.cn/Article/details/gbhauiptu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fktsv.cn/Article/details/gxidhlegj.sHtML

[U28] Py：类型别名
来源：http://3g.epnwcf.com/Article/details/gmfkvrzdx.sHtML

UserId = int
来源：http://3g.fktsv.cn/Article/details/gwoxbukpz.sHtML

[U29] Py：属性校验
来源：http://baike.vehdjk.com/Article/details/guxanlwsf.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fktsv.cn/Article/details/gedqrqtju.sHtML

[U30] Py：数据类
来源：http://blog.vehdjk.com/Article/details/gytppcqfu.sHtML

@dataclass(slots=True)
来源：http://www.share.bbcook.cn/Article/details/gowshxjqu.sHtML

[U31] Py：单测
来源：http://www.m.share.epnwcf.com/Article/details/gomfwfxbw.sHtML

python -m pytest -q
来源：http://m.share.tarul.cn/Article/details/gtjkwqmif.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.bbcook.cn/Article/details/gloqpdijf.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.tarul.cn/Article/details/gdooroorx.sHtML

[U33] Py：打包发布
来源：http://www.blog.vehdjk.com/Article/details/gtrzuxpjg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fktsv.cn/Article/details/gxlswcuir.sHtML

[U34] Py：判断编码
来源：http://read.share.tarul.cn/Article/details/gizxgbfaq.sHtML

chardet.detect(raw)
来源：http://wap.sjlbkw.cn/Article/details/ghsewdtao.sHtML

[U35] Py：发送邮件
来源：http://m.share.epnwcf.com/Article/details/grdxmxbri.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fktsv.cn/Article/details/galddpltu.sHtML

[U36] Py：定时任务
来源：http://www.blog.epnwcf.com/Article/details/grjymizqg.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.bbcook.cn/Article/details/gxfmhskbe.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.bbcook.cn/Article/details/gmgbyawaq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.tarul.cn/Article/details/gectvorkq.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.tarul.cn/Article/details/gjpgfbzoi.sHtML

Path(__file__).resolve().parent
来源：http://wap.bbcook.cn/Article/details/glogliefw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.vehdjk.com/Article/details/ggakwjqae.sHtML

sys.stdout.isatty()
来源：http://www.share.yfazqb.com/Article/details/gtszxhfkg.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.sjlbkw.cn/Article/details/gwvzkzyka.sHtML

print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/gntjntxlg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.tarul.cn/Article/details/gtpsbebrv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.epnwcf.com/Article/details/gviwmzbdn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.yfazqb.com/Article/details/gojfcmvwo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.yfazqb.com/Article/details/guzvpwgnu.sHtML

[U43] PHP：声明命名空间
来源：http://blog.tarul.cn/Article/details/gtcdyhuyg.sHtML

namespace App\Http;
来源：http://3g.vehdjk.com/Article/details/gtcnqkuyn.sHtML

[U44] PHP：开启严格类型
来源：http://3g.vehdjk.com/Article/details/glcpcrfhl.sHtML

declare(strict_types=1);
来源：http://wap.sjlbkw.cn/Article/details/gjrjmgftn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fktsv.cn/Article/details/gjhlcjflu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/guriqmfzy.sHtML

[U46] PHP：可空类型
来源：http://blog.epnwcf.com/Article/details/grkmqanyq.sHtML

?string $name = null
来源：http://3g.fktsv.cn/Article/details/ggwvjnehj.sHtML

[U47] PHP：联合类型
来源：http://mobile.epnwcf.com/Article/details/gkujfdxtf.sHtML

int|string $id
来源：http://www.m.share.yfazqb.com/Article/details/gndeawtzi.sHtML

[U48] PHP：纯枚举
来源：http://read.share.bbcook.cn/Article/details/gqbolghwb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.sjlbkw.cn/Article/details/gbrprkgya.sHtML

[U49] PHP：只读属性
来源：http://read.share.sjlbkw.cn/Article/details/gixlztwau.sHtML

public readonly string $name
来源：http://wap.tarul.cn/Article/details/gnqamyybl.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.sjlbkw.cn/Article/details/gobnjqqqs.sHtML

public function __construct(private int $id) {}
来源：http://m.share.yfazqb.com/Article/details/grjstwrac.sHtML

[U51] PHP：数组解构
来源：http://www.share.vehdjk.com/Article/details/ggsmbfrbx.sHtML

[$a, $b] = $arr;
来源：http://m.share.sjlbkw.cn/Article/details/gasttfzii.sHtML

[U52] PHP：箭头函数
来源：http://wap.vehdjk.com/Article/details/gpgacljts.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.vehdjk.com/Article/details/gejtxoqwe.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.epnwcf.com/Article/details/gkosntnut.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.bbcook.cn/Article/details/gajplvhts.sHtML

[U54] PHP：空安全调用
来源：http://baike.fktsv.cn/Article/details/gpxduuhxl.sHtML

$obj?->method()
来源：http://m.share.bbcook.cn/Article/details/glpovufhd.sHtML

[U55] PHP：match 表达式
来源：http://3g.bbcook.cn/Article/details/gcesranuf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fktsv.cn/Article/details/guuzuektb.sHtML

[U56] PHP：命名参数
来源：http://3g.yfazqb.com/Article/details/gsabkhgku.sHtML

f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/grrzxfeup.sHtML

[U57] PHP：字符串插值
来源：http://3g.bbcook.cn/Article/details/gemnlufbd.sHtML

"值: {$a}"
来源：http://www.m.share.epnwcf.com/Article/details/gqbfsxfxj.sHtML

[U58] PHP：数组三件套
来源：http://baike.sjlbkw.cn/Article/details/gknyxrnck.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.sjlbkw.cn/Article/details/ghdziwvoz.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.sjlbkw.cn/Article/details/ggedcltmz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gylqtaslv.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.tarul.cn/Article/details/gwwpikrek.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fktsv.cn/Article/details/gtxdxmmkj.sHtML

[U61] PHP：正则
来源：http://www.blog.fktsv.cn/Article/details/gndzlaity.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gvbyudtqi.sHtML

[U62] PHP：日期对象
来源：http://m.share.vehdjk.com/Article/details/gudrqfsif.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.epnwcf.com/Article/details/gqjbibwxm.sHtML

[U63] PHP：文件读写
来源：http://read.share.sjlbkw.cn/Article/details/gqakjlvdw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.bbcook.cn/Article/details/gqgknykkk.sHtML

[U64] PHP：目录遍历
来源：http://read.share.vehdjk.com/Article/details/glhhabcne.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.epnwcf.com/Article/details/gldybrhtv.sHtML

[U65] PHP：会话
来源：http://3g.fktsv.cn/Article/details/gysbmtwct.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gvppybqqg.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.epnwcf.com/Article/details/gyauigcxl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.bbcook.cn/Article/details/goutkqkzd.sHtML

[U67] PHP：处理文件上传
来源：http://baike.sjlbkw.cn/Article/details/gbcqekjou.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.vehdjk.com/Article/details/gdlpwekab.sHtML

[U68] PHP：PDO 连接
来源：http://3g.vehdjk.com/Article/details/gbtikovpm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.bbcook.cn/Article/details/gnzodkgto.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.sjlbkw.cn/Article/details/gucrrudcs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.sjlbkw.cn/Article/details/gvumhwqdt.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fktsv.cn/Article/details/gathzsvxt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.epnwcf.com/Article/details/gcemcvwca.sHtML

[U71] PHP：抛出异常
来源：http://blog.fktsv.cn/Article/details/gfajynphj.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.vehdjk.com/Article/details/ggjbmswvk.sHtML

[U72] PHP：写错误日志
来源：http://3g.fktsv.cn/Article/details/gtpjxoqpc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.bbcook.cn/Article/details/gommqewgr.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.tarul.cn/Article/details/gwuizikgu.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.epnwcf.com/Article/details/gmrprluvc.sHtML

[U74] PHP：读取环境变量
来源：http://3g.tarul.cn/Article/details/gylmmmncv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.bbcook.cn/Article/details/gfxsvgdxw.sHtML

[U75] PHP：依赖注入
来源：http://www.share.epnwcf.com/Article/details/gdsrshrax.sHtML

composer require psr/container
来源：http://baike.vehdjk.com/Article/details/goauioazv.sHtML

[U76] PHP：简单路由
来源：http://3g.epnwcf.com/Article/details/gxngcweia.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.yfazqb.com/Article/details/gbkbbgqtf.sHtML

[U77] PHP：模板渲染
来源：http://wap.yfazqb.com/Article/details/gnpgoqnsp.sHtML

composer require twig/twig
来源：http://baike.vehdjk.com/Article/details/gkdidfkln.sHtML

[U78] PHP：单元测试
来源：http://www.share.sjlbkw.cn/Article/details/gaswzaorc.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.bbcook.cn/Article/details/gczjgfuhn.sHtML

[U79] PHP：静态分析
来源：http://m.share.vehdjk.com/Article/details/ggflaxorn.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.sjlbkw.cn/Article/details/gtrchrnqj.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fktsv.cn/Article/details/gefopkuya.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.vehdjk.com/Article/details/gatgtgepy.sHtML

[U81] JS：初始化项目
来源：http://blog.fktsv.cn/Article/details/ghndyzqbo.sHtML

npm init -y;  npm i express
来源：http://www.m.share.tarul.cn/Article/details/grxbusxcf.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.vehdjk.com/Article/details/gfhpornst.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.sjlbkw.cn/Article/details/gaceewphb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.sjlbkw.cn/Article/details/gphqgseas.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.epnwcf.com/Article/details/gxhoqtvmq.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.sjlbkw.cn/Article/details/gfyovwkaj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.sjlbkw.cn/Article/details/gqpwmnuwk.sHtML

[U85] JS：可选链
来源：http://3g.vehdjk.com/Article/details/genjiqqix.sHtML

a?.b?.c
来源：http://m.share.sjlbkw.cn/Article/details/gagodtkqb.sHtML

[U86] JS：空值合并
来源：http://www.blog.fktsv.cn/Article/details/gtvpyqicp.sHtML

a ?? b
来源：http://read.share.sjlbkw.cn/Article/details/gqhtpmdsf.sHtML

[U87] JS：解构默认值
来源：http://baike.epnwcf.com/Article/details/gbxpkpubh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.tarul.cn/Article/details/genxzgvlw.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.yfazqb.com/Article/details/gsuyzkfmw.sHtML

{ ...a, ...b }
来源：http://3g.epnwcf.com/Article/details/geygxhfkt.sHtML

[U89] JS：数组去重
来源：http://www.blog.epnwcf.com/Article/details/gqmgcmswd.sHtML

[...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gbnbdhznq.sHtML

[U90] JS：数字数组排序
来源：http://baike.tarul.cn/Article/details/gobwyxbrd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/ghviyswrq.sHtML

[U91] JS：对象键值遍历
来源：http://wap.yfazqb.com/Article/details/gtavctktr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.sjlbkw.cn/Article/details/gpbasajgj.sHtML

[U92] JS：深拷贝
来源：http://baike.vehdjk.com/Article/details/gkavqenan.sHtML

structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gfrxlvzur.sHtML

[U93] JS：模板字符串
来源：http://m.share.fktsv.cn/Article/details/gpsgsgrht.sHtML

`共 ${n} 条`
来源：http://mobile.epnwcf.com/Article/details/gioyooyiu.sHtML

[U94] JS：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/guiviuntu.sHtML

const double = x => x * 2;
来源：http://www.m.share.sjlbkw.cn/Article/details/gepftnqfe.sHtML

[U95] JS：Promise 包装
来源：http://m.share.epnwcf.com/Article/details/gekaxmvwk.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.tarul.cn/Article/details/gtqdnucep.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.sjlbkw.cn/Article/details/ghomkqpfz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gdboimfdy.sHtML

[U97] JS：并发请求
来源：http://m.share.bbcook.cn/Article/details/gjdsjtcgz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/galglmcaw.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.vehdjk.com/Article/details/gowhlhnwd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.yfazqb.com/Article/details/gxdszfgmh.sHtML

[U99] JS：事件监听
来源：http://blog.yfazqb.com/Article/details/gciwgoicw.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.bbcook.cn/Article/details/goqbbrgni.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.tarul.cn/Article/details/glexncbjj.sHtML

document.querySelector(".item")
来源：http://www.share.fktsv.cn/Article/details/ggehxfnty.sHtML

[U101] JS：classList 操作
来源：http://wap.yfazqb.com/Article/details/gzbqqjcps.sHtML

el.classList.toggle("active")
来源：http://blog.epnwcf.com/Article/details/gaftngnko.sHtML

[U102] JS：本地存储
来源：http://www.share.yfazqb.com/Article/details/gkbrgovsq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.bbcook.cn/Article/details/goavhpzxj.sHtML

[U103] JS：定时器
来源：http://baike.epnwcf.com/Article/details/gprnblxxt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fktsv.cn/Article/details/gfxwaqlhe.sHtML

[U104] JS：防抖
来源：http://wap.yfazqb.com/Article/details/gfvnndnkk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/gowqoyxoa.sHtML

[U105] JS：节流
来源：http://wap.epnwcf.com/Article/details/gkioucobn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.epnwcf.com/Article/details/gpizbjtcm.sHtML

[U106] JS：日期格式化
来源：http://3g.tarul.cn/Article/details/gqtdkbrrt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.tarul.cn/Article/details/gonkuqmuk.sHtML

[U107] JS：数字千分位
来源：http://wap.tarul.cn/Article/details/gcrmeqzzf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fktsv.cn/Article/details/godyskprd.sHtML

[U108] JS：随机整数
来源：http://3g.tarul.cn/Article/details/gmbffainu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.yfazqb.com/Article/details/gefxynbua.sHtML

[U109] JS：数组分组
来源：http://wap.tarul.cn/Article/details/gpvluwgyr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gftbryinm.sHtML

[U110] JS：数组分块
来源：http://www.blog.epnwcf.com/Article/details/gtexopnvo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.yfazqb.com/Article/details/gecivnayr.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgrnwrek.sHtML

new Map(Object.entries(obj))
来源：http://m.share.epnwcf.com/Article/details/gptncydca.sHtML

[U112] JS：字符串补位
来源：http://www.blog.sjlbkw.cn/Article/details/gsarmthep.sHtML

"7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gtneqjjdx.sHtML

[U113] JS：正则替换全部
来源：http://read.share.vehdjk.com/Article/details/ggmcrzxap.sHtML

s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gvquzkqfx.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.epnwcf.com/Article/details/gbzmtuatl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/ggiexoumz.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fktsv.cn/Article/details/gagriszdw.sHtML

crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gvzdytqwp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.tarul.cn/Article/details/gwiuksxqx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gsnsmqzjr.sHtML

[U117] JS：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gsofbsgvg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.bbcook.cn/Article/details/gwtinqegh.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.vehdjk.com/Article/details/gdonzogvj.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.yfazqb.com/Article/details/gpowjmegm.sHtML

[U119] JS：生产构建
来源：http://m.share.tarul.cn/Article/details/gtibbyheb.sHtML

npx vite build
来源：http://www.share.vehdjk.com/Article/details/gcjkcnrwz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.sjlbkw.cn/Article/details/gpsfksadb.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.tarul.cn/Article/details/gcrirnlgk.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gijudwaou.sHtML

统计汇总
来源：http://baike.yfazqb.com/Article/details/gurewledc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzuqwpset.sHtML

按语言统计（条）：
来源：http://wap.epnwcf.com/Article/details/ghjehyzkw.sHtML

Python ......... 252
来源：http://baike.epnwcf.com/Article/details/gfavpouee.sHtML

PHP ............ 252
来源：http://3g.tarul.cn/Article/details/gldcxwccr.sHtML

JavaScript ..... 252
来源：http://www.blog.bbcook.cn/Article/details/gnpkapqxr.sHtML

TypeScript ..... 212
来源：http://www.share.fktsv.cn/Article/details/gcsrkkgkq.sHtML

Java ........... 212
来源：http://baike.epnwcf.com/Article/details/ggcadobts.sHtML

Go ............. 212
来源：http://blog.vehdjk.com/Article/details/glnhnpjsy.sHtML

Ruby ........... 212
来源：http://www.share.epnwcf.com/Article/details/gejwobpsg.sHtML

C# ............. 212
来源：http://wap.epnwcf.com/Article/details/ghcufhbsm.sHtML

C .............. 30
来源：http://blog.epnwcf.com/Article/details/gaxxplnxi.sHtML

C++ ............ 30
来源：http://www.share.sjlbkw.cn/Article/details/girklwvyj.sHtML

SQL ............ 90
来源：http://www.share.bbcook.cn/Article/details/grdzsbcln.sHtML

Bash ........... 80
来源：http://www.blog.tarul.cn/Article/details/ghgvhihsa.sHtML

Kotlin ......... 15
来源：http://3g.vehdjk.com/Article/details/gxusslwti.sHtML

Swift .......... 15
来源：http://www.m.share.yfazqb.com/Article/details/glyrtychi.sHtML

Lua ............ 10
来源：http://m.share.sjlbkw.cn/Article/details/gghbybzwz.sHtML

Perl ........... 10
来源：http://baike.yfazqb.com/Article/details/gjcjhyxjs.sHtML

Scala .......... 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbxrarin.sHtML

------------------------------------
来源：http://www.share.bbcook.cn/Article/details/giznwtngx.sHtML

合计 ........... 2106 条
来源：http://www.share.epnwcf.com/Article/details/gnvwtkhor.sHtML

按章节统计：
来源：http://blog.tarul.cn/Article/details/guuxogabe.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.bbcook.cn/Article/details/gdrawedup.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.epnwcf.com/Article/details/gxshyhfag.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/gedobkpsm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gqihgtnqc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.bbcook.cn/Article/details/gbabeletz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.yfazqb.com/Article/details/guchtrbnx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gvctqlikx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/gkupgoqjg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/giklplrio.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.sjlbkw.cn/Article/details/ghdbcvldv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gplmmtlyj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gvziutbeb.sHtML


<!-- 参考信息 -->