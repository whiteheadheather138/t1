代发 wailian999

[T47] Perl：正则捕获
来源：http://m.share.bbcook.cn/Article/details/ghkgleuwi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.bbcook.cn/Article/details/gpspwutgy.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.epnwcf.com/Article/details/gkwawznum.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fktsv.cn/Article/details/gtzmiwjxx.sHtML

[T49] Perl：函数
来源：http://mobile.sjlbkw.cn/Article/details/gaeqnatul.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gtecjscqa.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gemgjubvr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/gnmppqyuy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.yfazqb.com/Article/details/gjcilhhki.sHtML

[T51] Scala：Hello World
来源：http://m.share.tarul.cn/Article/details/gyfntfaab.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gxpqlsvdh.sHtML

[T52] Scala：变量
来源：http://blog.fktsv.cn/Article/details/gsfoaodqa.sHtML

val a = 1;  var b = 2
来源：http://3g.yfazqb.com/Article/details/ghqddievf.sHtML

[T53] Scala：字符串插值
来源：http://baike.epnwcf.com/Article/details/gdpcmacpy.sHtML

s"值: $b"
来源：http://wap.vehdjk.com/Article/details/gfjblbtza.sHtML

[T54] Scala：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gwpccfdlp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.yfazqb.com/Article/details/gkuvgxchm.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gmumrubgv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.bbcook.cn/Article/details/gwhuphycb.sHtML

[T56] Scala：样例类
来源：http://baike.fktsv.cn/Article/details/gbghupfed.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gzwxhjjmg.sHtML

[T57] Scala：模式匹配
来源：http://wap.fktsv.cn/Article/details/gkjlomszc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.sjlbkw.cn/Article/details/glwmmerwp.sHtML

[T58] Scala：函数定义
来源：http://blog.yfazqb.com/Article/details/gxtraudea.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.yfazqb.com/Article/details/gmpsykqkp.sHtML

[T59] Scala：循环
来源：http://3g.yfazqb.com/Article/details/ghfytqiya.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.vehdjk.com/Article/details/gqgtsmtuv.sHtML

[T60] Scala：折叠
来源：http://read.share.tarul.cn/Article/details/guashgkei.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.yfazqb.com/Article/details/gysnlxuvx.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjjbvsbtr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gecvyvupm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghpdcfstz.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fktsv.cn/Article/details/gpcnsqgap.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gkjhkubtg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.vehdjk.com/Article/details/gudtbczmf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.vehdjk.com/Article/details/galbrsvfm.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.yfazqb.com/Article/details/gynizjpsx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.tarul.cn/Article/details/glpbcdtkl.sHtML

[U04] Py：变量调试打印
来源：http://mobile.vehdjk.com/Article/details/gkfntusrx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.epnwcf.com/Article/details/gogoijxcb.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.vehdjk.com/Article/details/gvthdhwzb.sHtML

list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gjnwirxaw.sHtML

[U06] Py：合并两个字典
来源：http://3g.vehdjk.com/Article/details/gfehjnmgm.sHtML

{**a, **b}
来源：http://blog.tarul.cn/Article/details/gdqwdyhfu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.tarul.cn/Article/details/gbxgyexxe.sHtML

{v: k for k, v in d.items()}
来源：http://3g.yfazqb.com/Article/details/groicyntz.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fktsv.cn/Article/details/gkfpotkvd.sHtML

[y for x in nested for y in x]
来源：http://baike.epnwcf.com/Article/details/ggnnxhyga.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.tarul.cn/Article/details/gluvxilyn.sHtML

max(d, key=d.get)
来源：http://m.share.fktsv.cn/Article/details/gnqimhmfu.sHtML

[U10] Py：按值排序字典
来源：http://wap.sjlbkw.cn/Article/details/gerjprfzn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.vehdjk.com/Article/details/gtuqhvcoi.sHtML

[U11] Py：生成器表达式
来源：http://wap.tarul.cn/Article/details/gegmeqvpp.sHtML

(x * 2 for x in arr)
来源：http://www.blog.vehdjk.com/Article/details/gnqpkjrwc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.tarul.cn/Article/details/ggrwzlvae.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.bbcook.cn/Article/details/gtxisabas.sHtML

[U13] Py：固定长度队列
来源：http://read.share.sjlbkw.cn/Article/details/gkwbbmpln.sHtML

deque(maxlen=10)
来源：http://www.blog.yfazqb.com/Article/details/gkmslviuf.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.sjlbkw.cn/Article/details/gdvvcabkg.sHtML

defaultdict(list)
来源：http://m.share.epnwcf.com/Article/details/gzycurlym.sHtML

[U15] Py：高精度计时
来源：http://baike.epnwcf.com/Article/details/ghnntvkui.sHtML

t = time.perf_counter()
来源：http://wap.epnwcf.com/Article/details/gzggghqoo.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.tarul.cn/Article/details/ghfvirlbg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.bbcook.cn/Article/details/gkplpomhy.sHtML

[U17] Py：初始化日志
来源：http://3g.epnwcf.com/Article/details/golvswnpv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.bbcook.cn/Article/details/gxpqxcbjy.sHtML

[U18] Py：预编译正则
来源：http://blog.yfazqb.com/Article/details/ggsekmoxv.sHtML

pat = re.compile(r"\d+")
来源：http://3g.tarul.cn/Article/details/glogmgbhc.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.bbcook.cn/Article/details/garodlujx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.bbcook.cn/Article/details/gojlgntng.sHtML

[U20] Py：缓存函数结果
来源：http://3g.yfazqb.com/Article/details/gtuajgoyu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.epnwcf.com/Article/details/gwcnrfvru.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.bbcook.cn/Article/details/gixkbiuef.sHtML

@contextlib.contextmanager
来源：http://blog.fktsv.cn/Article/details/gnhzbtnur.sHtML

[U22] Py：矩阵转置
来源：http://baike.bbcook.cn/Article/details/gusruaubi.sHtML

list(zip(*m))
来源：http://www.m.share.epnwcf.com/Article/details/gwizgwclw.sHtML

[U23] Py：分块读取大文件
来源：http://baike.bbcook.cn/Article/details/gimqotolz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fktsv.cn/Article/details/gckibplso.sHtML

[U24] Py：路径操作
来源：http://blog.epnwcf.com/Article/details/gvhrmyqjn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gmzqattfh.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fktsv.cn/Article/details/ggzuqsela.sHtML

csv.DictReader(f)
来源：http://blog.tarul.cn/Article/details/ganamciju.sHtML

[U26] Py：并发下载
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsnovhzj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.yfazqb.com/Article/details/gpxqxgbkc.sHtML

[U27] Py：异步 HTTP
来源：http://wap.yfazqb.com/Article/details/gkgsusujw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.sjlbkw.cn/Article/details/gzbxnoxfp.sHtML

[U28] Py：类型别名
来源：http://www.blog.epnwcf.com/Article/details/ggaggibbq.sHtML

UserId = int
来源：http://www.blog.yfazqb.com/Article/details/gvtciodlv.sHtML

[U29] Py：属性校验
来源：http://read.share.epnwcf.com/Article/details/gwvntqxxs.sHtML

@property 与 @x.setter 配合
来源：http://blog.sjlbkw.cn/Article/details/gpuwalfoa.sHtML

[U30] Py：数据类
来源：http://www.share.bbcook.cn/Article/details/gjxyvrydq.sHtML

@dataclass(slots=True)
来源：http://baike.tarul.cn/Article/details/gdslldtfr.sHtML

[U31] Py：单测
来源：http://www.m.share.bbcook.cn/Article/details/gbfbhpiza.sHtML

python -m pytest -q
来源：http://mobile.tarul.cn/Article/details/gksqulyga.sHtML

[U32] Py：代码格式化
来源：http://wap.sjlbkw.cn/Article/details/gatnuuhqt.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.sjlbkw.cn/Article/details/gpwgizoes.sHtML

[U33] Py：打包发布
来源：http://read.share.epnwcf.com/Article/details/gulwsrehg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.yfazqb.com/Article/details/gyhgiywus.sHtML

[U34] Py：判断编码
来源：http://wap.yfazqb.com/Article/details/gxckwpqbp.sHtML

chardet.detect(raw)
来源：http://baike.fktsv.cn/Article/details/gbillsjju.sHtML

[U35] Py：发送邮件
来源：http://read.share.vehdjk.com/Article/details/gwgtobhft.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.tarul.cn/Article/details/gpukxdkef.sHtML

[U36] Py：定时任务
来源：http://mobile.bbcook.cn/Article/details/gwnencvok.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fktsv.cn/Article/details/gpjnjpfny.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.yfazqb.com/Article/details/glpzlfljg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fktsv.cn/Article/details/gcpejhhbm.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.sjlbkw.cn/Article/details/gjmymsohx.sHtML

Path(__file__).resolve().parent
来源：http://baike.tarul.cn/Article/details/grxbwgwss.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fktsv.cn/Article/details/gsntmuxqj.sHtML

sys.stdout.isatty()
来源：http://www.share.fktsv.cn/Article/details/giifufnln.sHtML

[U40] Py：打印到标准错误
来源：http://3g.tarul.cn/Article/details/gpjiulqrr.sHtML

print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/gitzpozen.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.vehdjk.com/Article/details/gylngyqyw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.vehdjk.com/Article/details/glhaclrps.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.tarul.cn/Article/details/grmyirmnd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fktsv.cn/Article/details/gikmvlrok.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.tarul.cn/Article/details/gdmtvpwvm.sHtML

namespace App\Http;
来源：http://www.share.sjlbkw.cn/Article/details/gskcnarlh.sHtML

[U44] PHP：开启严格类型
来源：http://3g.bbcook.cn/Article/details/gikesrdne.sHtML

declare(strict_types=1);
来源：http://blog.yfazqb.com/Article/details/guxxgebjn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.yfazqb.com/Article/details/gxsdjlqmq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gypehkjxo.sHtML

[U46] PHP：可空类型
来源：http://3g.sjlbkw.cn/Article/details/gbpqcdpja.sHtML

?string $name = null
来源：http://3g.yfazqb.com/Article/details/gcczkjprj.sHtML

[U47] PHP：联合类型
来源：http://blog.sjlbkw.cn/Article/details/gkngagajh.sHtML

int|string $id
来源：http://3g.fktsv.cn/Article/details/guvnbncwe.sHtML

[U48] PHP：纯枚举
来源：http://mobile.epnwcf.com/Article/details/gzerdoljr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.bbcook.cn/Article/details/gbbbwkxif.sHtML

[U49] PHP：只读属性
来源：http://mobile.epnwcf.com/Article/details/ggwwfkmox.sHtML

public readonly string $name
来源：http://mobile.vehdjk.com/Article/details/gvrankgwu.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.tarul.cn/Article/details/gpttjsmik.sHtML

public function __construct(private int $id) {}
来源：http://wap.fktsv.cn/Article/details/gqvnnlpse.sHtML

[U51] PHP：数组解构
来源：http://www.blog.yfazqb.com/Article/details/gcpcykkmm.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/gbzgwcqwd.sHtML

[U52] PHP：箭头函数
来源：http://www.share.tarul.cn/Article/details/gxtdzkogu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.tarul.cn/Article/details/grnftzstz.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.yfazqb.com/Article/details/gacrvlguu.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.yfazqb.com/Article/details/gbkussvka.sHtML

[U54] PHP：空安全调用
来源：http://read.share.sjlbkw.cn/Article/details/gwzmmfmhb.sHtML

$obj?->method()
来源：http://mobile.vehdjk.com/Article/details/giwxwdgxw.sHtML

[U55] PHP：match 表达式
来源：http://m.share.epnwcf.com/Article/details/gvzcfqnbk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.vehdjk.com/Article/details/gijeonaei.sHtML

[U56] PHP：命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gdnprvgal.sHtML

f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/ghzzyeayz.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gnetcusmk.sHtML

"值: {$a}"
来源：http://wap.fktsv.cn/Article/details/gnxosurcg.sHtML

[U58] PHP：数组三件套
来源：http://baike.epnwcf.com/Article/details/gftxckvwp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.sjlbkw.cn/Article/details/gqfkmosfe.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fktsv.cn/Article/details/gbwhqukou.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gxjsweyvd.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.yfazqb.com/Article/details/gyhcealgn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.epnwcf.com/Article/details/gcvvtqgwd.sHtML

[U61] PHP：正则
来源：http://blog.epnwcf.com/Article/details/gjhuqusic.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/ghzupnbpa.sHtML

[U62] PHP：日期对象
来源：http://baike.sjlbkw.cn/Article/details/gnbcjsevk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fktsv.cn/Article/details/guhrvdqzz.sHtML

[U63] PHP：文件读写
来源：http://blog.sjlbkw.cn/Article/details/gtyloxeyv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.sjlbkw.cn/Article/details/gjntyrbab.sHtML

[U64] PHP：目录遍历
来源：http://wap.vehdjk.com/Article/details/gkhjoqilh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.epnwcf.com/Article/details/gnadjxvup.sHtML

[U65] PHP：会话
来源：http://m.share.yfazqb.com/Article/details/gwqlgprot.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gvuejotnl.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.vehdjk.com/Article/details/gyxebfhmy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.epnwcf.com/Article/details/gjehttwrm.sHtML

[U67] PHP：处理文件上传
来源：http://3g.vehdjk.com/Article/details/gqfowyntl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fktsv.cn/Article/details/gpiiqkizd.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.tarul.cn/Article/details/gwoxbnuus.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.sjlbkw.cn/Article/details/gyefksnkq.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.vehdjk.com/Article/details/gmvzjushq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.yfazqb.com/Article/details/gxanqhosp.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.vehdjk.com/Article/details/gxayvaulu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/gcqmbwxce.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.yfazqb.com/Article/details/gxtnoaahp.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.epnwcf.com/Article/details/gwtmevaez.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.epnwcf.com/Article/details/gnkfvwhxh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.sjlbkw.cn/Article/details/giautcmrp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.bbcook.cn/Article/details/gnfpzhgnz.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.tarul.cn/Article/details/gtrgzecfh.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gjhdscrdf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.sjlbkw.cn/Article/details/guvhaslmm.sHtML

[U75] PHP：依赖注入
来源：http://wap.yfazqb.com/Article/details/gevrugjzw.sHtML

composer require psr/container
来源：http://www.share.tarul.cn/Article/details/gaurfcoyz.sHtML

[U76] PHP：简单路由
来源：http://wap.bbcook.cn/Article/details/ggwsigbgl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.vehdjk.com/Article/details/gdfknkcgx.sHtML

[U77] PHP：模板渲染
来源：http://mobile.yfazqb.com/Article/details/grrtpnbzy.sHtML

composer require twig/twig
来源：http://m.share.bbcook.cn/Article/details/gfsieumza.sHtML

[U78] PHP：单元测试
来源：http://www.share.sjlbkw.cn/Article/details/glxkarwli.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.tarul.cn/Article/details/gieaqyfhi.sHtML

[U79] PHP：静态分析
来源：http://wap.bbcook.cn/Article/details/gvgszmixw.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fktsv.cn/Article/details/ggrkoopym.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.yfazqb.com/Article/details/gmaqfunwq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.yfazqb.com/Article/details/grcwtjght.sHtML

[U81] JS：初始化项目
来源：http://baike.yfazqb.com/Article/details/gxrbpuhgp.sHtML

npm init -y;  npm i express
来源：http://3g.yfazqb.com/Article/details/gougjmlao.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fktsv.cn/Article/details/gileyigvw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.sjlbkw.cn/Article/details/gwgmownqt.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fktsv.cn/Article/details/gdgryhbwz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/glmtbilho.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.epnwcf.com/Article/details/gggpcxkts.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.sjlbkw.cn/Article/details/gzmftnrhu.sHtML

[U85] JS：可选链
来源：http://www.blog.vehdjk.com/Article/details/ghbxsgjsv.sHtML

a?.b?.c
来源：http://blog.tarul.cn/Article/details/gnyjosetg.sHtML

[U86] JS：空值合并
来源：http://m.share.epnwcf.com/Article/details/gubygswmz.sHtML

a ?? b
来源：http://3g.fktsv.cn/Article/details/gfllymxgp.sHtML

[U87] JS：解构默认值
来源：http://3g.vehdjk.com/Article/details/gngijilgb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.vehdjk.com/Article/details/gzwvzaatj.sHtML

[U88] JS：对象展开合并
来源：http://blog.epnwcf.com/Article/details/gusxoytsn.sHtML

{ ...a, ...b }
来源：http://read.share.tarul.cn/Article/details/gidwlgupn.sHtML

[U89] JS：数组去重
来源：http://wap.epnwcf.com/Article/details/gxcxidllj.sHtML

[...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gljmbgvco.sHtML

[U90] JS：数字数组排序
来源：http://www.share.sjlbkw.cn/Article/details/gvxccwxnm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/giasytena.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.bbcook.cn/Article/details/gwboocess.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.yfazqb.com/Article/details/gbhxxudnx.sHtML

[U92] JS：深拷贝
来源：http://blog.sjlbkw.cn/Article/details/gwyekbqed.sHtML

structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gdxjtxcus.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fktsv.cn/Article/details/gqryejqju.sHtML

`共 ${n} 条`
来源：http://www.m.share.epnwcf.com/Article/details/grsjfoggo.sHtML

[U94] JS：箭头函数
来源：http://wap.tarul.cn/Article/details/gdcfysxtg.sHtML

const double = x => x * 2;
来源：http://read.share.tarul.cn/Article/details/gnkdnrvpq.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.yfazqb.com/Article/details/gstlswcjx.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.tarul.cn/Article/details/gpjxwxsko.sHtML

[U96] JS：async/await 与异常
来源：http://baike.bbcook.cn/Article/details/ghbqbcfgx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gxzfqvgpk.sHtML

[U97] JS：并发请求
来源：http://read.share.bbcook.cn/Article/details/gqfhhsqti.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gswogicfx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.epnwcf.com/Article/details/ggfgtznqq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fktsv.cn/Article/details/gxjtvwbwq.sHtML

[U99] JS：事件监听
来源：http://3g.sjlbkw.cn/Article/details/gulbbhpwo.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.tarul.cn/Article/details/gcycqhifm.sHtML

[U100] JS：DOM 查询
来源：http://baike.vehdjk.com/Article/details/ghdnlefne.sHtML

document.querySelector(".item")
来源：http://www.m.share.fktsv.cn/Article/details/gkabgbofk.sHtML

[U101] JS：classList 操作
来源：http://read.share.sjlbkw.cn/Article/details/gjwmmaflj.sHtML

el.classList.toggle("active")
来源：http://www.blog.epnwcf.com/Article/details/gupzbmfyu.sHtML

[U102] JS：本地存储
来源：http://blog.yfazqb.com/Article/details/gvvvarujz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.epnwcf.com/Article/details/gkuqxsyun.sHtML

[U103] JS：定时器
来源：http://wap.bbcook.cn/Article/details/gttyyjhnk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.epnwcf.com/Article/details/gjokslhvh.sHtML

[U104] JS：防抖
来源：http://blog.bbcook.cn/Article/details/gspeyujii.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/ggmyrbdmw.sHtML

[U105] JS：节流
来源：http://m.share.epnwcf.com/Article/details/gbxpoqztm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.yfazqb.com/Article/details/gdrnqyvex.sHtML

[U106] JS：日期格式化
来源：http://www.share.fktsv.cn/Article/details/gtickyvvm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.epnwcf.com/Article/details/ggssxnlyr.sHtML

[U107] JS：数字千分位
来源：http://www.share.tarul.cn/Article/details/gupojmobu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.epnwcf.com/Article/details/gnzipqfdi.sHtML

[U108] JS：随机整数
来源：http://mobile.vehdjk.com/Article/details/gkpytrimw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.bbcook.cn/Article/details/grupspwqo.sHtML

[U109] JS：数组分组
来源：http://3g.bbcook.cn/Article/details/gxrcwatkz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gnhmxdwld.sHtML

[U110] JS：数组分块
来源：http://3g.epnwcf.com/Article/details/gpwykfzdf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.sjlbkw.cn/Article/details/grrvwvbnu.sHtML

[U111] JS：对象转 Map
来源：http://mobile.vehdjk.com/Article/details/gnvwargcj.sHtML

new Map(Object.entries(obj))
来源：http://blog.vehdjk.com/Article/details/gvnojxfaz.sHtML

[U112] JS：字符串补位
来源：http://www.share.tarul.cn/Article/details/gvjudpieg.sHtML

"7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gkliihrjj.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.epnwcf.com/Article/details/gbkizkvzq.sHtML

s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gfddwwwqr.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.sjlbkw.cn/Article/details/gxpagtjqd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/gcxclgdby.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gduduizlw.sHtML

crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gpnzkmsdh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.tarul.cn/Article/details/gfhlgbnzx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.vehdjk.com/Article/details/glnecmvpz.sHtML

[U117] JS：单元测试
来源：http://wap.vehdjk.com/Article/details/gpmylmykj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.vehdjk.com/Article/details/gjfhabjlk.sHtML

[U118] JS：开发服务器
来源：http://mobile.yfazqb.com/Article/details/glpcmhrwj.sHtML

npm i -D vite;  npx vite
来源：http://wap.epnwcf.com/Article/details/geinynrfx.sHtML

[U119] JS：生产构建
来源：http://www.m.share.tarul.cn/Article/details/gpmsklalq.sHtML

npx vite build
来源：http://www.m.share.tarul.cn/Article/details/gecvrfmcp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.yfazqb.com/Article/details/gkqerzfzc.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fktsv.cn/Article/details/gqemtwqsb.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gniptexvi.sHtML

统计汇总
来源：http://3g.yfazqb.com/Article/details/gaekeuwmh.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gitlqblks.sHtML

按语言统计（条）：
来源：http://read.share.bbcook.cn/Article/details/gzlwcrvnl.sHtML

Python ......... 252
来源：http://wap.tarul.cn/Article/details/gucgirdfz.sHtML

PHP ............ 252
来源：http://blog.sjlbkw.cn/Article/details/grffyhlra.sHtML

JavaScript ..... 252
来源：http://www.m.share.epnwcf.com/Article/details/geuahvepf.sHtML

TypeScript ..... 212
来源：http://m.share.bbcook.cn/Article/details/gqudrdeur.sHtML

Java ........... 212
来源：http://www.share.fktsv.cn/Article/details/gwdiausce.sHtML

Go ............. 212
来源：http://3g.fktsv.cn/Article/details/gicdnjgrd.sHtML

Ruby ........... 212
来源：http://read.share.yfazqb.com/Article/details/gvcebsccg.sHtML

C# ............. 212
来源：http://www.share.vehdjk.com/Article/details/gnwvekijm.sHtML

C .............. 30
来源：http://www.m.share.epnwcf.com/Article/details/gjkppoyzx.sHtML

C++ ............ 30
来源：http://read.share.bbcook.cn/Article/details/gvkroepmq.sHtML

SQL ............ 90
来源：http://3g.bbcook.cn/Article/details/glqprazbn.sHtML

Bash ........... 80
来源：http://3g.bbcook.cn/Article/details/gwpgyqvgj.sHtML

Kotlin ......... 15
来源：http://m.share.vehdjk.com/Article/details/gawipooss.sHtML

Swift .......... 15
来源：http://www.blog.vehdjk.com/Article/details/gzrmfjllk.sHtML

Lua ............ 10
来源：http://blog.sjlbkw.cn/Article/details/gryoawsdk.sHtML

Perl ........... 10
来源：http://baike.yfazqb.com/Article/details/gfkgkbzjr.sHtML

Scala .......... 10
来源：http://mobile.epnwcf.com/Article/details/ggvnswplv.sHtML

------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gesyaiwai.sHtML

合计 ........... 2106 条
来源：http://m.share.epnwcf.com/Article/details/gptrqilzi.sHtML

按章节统计：
来源：http://mobile.epnwcf.com/Article/details/gwjwjqsyn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/guexkdyds.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gpzowedcu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gxgqpxyha.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/gloqpelaz.sHtML


<!-- 参考信息 -->