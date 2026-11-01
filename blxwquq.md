代发 wailian999

[T47] Perl：正则捕获
来源：http://3g.tarul.cn/Article/details/godptxgca.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.sjlbkw.cn/Article/details/gudlkbcwp.sHtML

[T48] Perl：正则替换
来源：http://blog.yfazqb.com/Article/details/gyktfvozt.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fktsv.cn/Article/details/gwbrpevlf.sHtML

[T49] Perl：函数
来源：http://www.m.share.yfazqb.com/Article/details/gtmbrygpp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/grpjbsoxy.sHtML

[T50] Perl：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gdvcrywlw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.tarul.cn/Article/details/gohwzwiwa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fktsv.cn/Article/details/gscimbjgi.sHtML

[T51] Scala：Hello World
来源：http://baike.sjlbkw.cn/Article/details/glhkoiecq.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gdollbkua.sHtML

[T52] Scala：变量
来源：http://blog.fktsv.cn/Article/details/gicubrrnp.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gufmhbquc.sHtML

[T53] Scala：字符串插值
来源：http://read.share.tarul.cn/Article/details/gfmzeevbm.sHtML

s"值: $b"
来源：http://m.share.yfazqb.com/Article/details/gpqvliycx.sHtML

[T54] Scala：集合映射
来源：http://blog.vehdjk.com/Article/details/gbxisyavu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gkmbgtcwe.sHtML

[T55] Scala：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gcbdhcgwo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.epnwcf.com/Article/details/gsmmypfhj.sHtML

[T56] Scala：样例类
来源：http://mobile.vehdjk.com/Article/details/gtdohvdef.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/gbwjzmdok.sHtML

[T57] Scala：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/gopitpuvz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.tarul.cn/Article/details/gjajzcqom.sHtML

[T58] Scala：函数定义
来源：http://blog.epnwcf.com/Article/details/gztkakckp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.bbcook.cn/Article/details/grumvanah.sHtML

[T59] Scala：循环
来源：http://mobile.epnwcf.com/Article/details/gxrmqobzc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gxjhcrprl.sHtML

[T60] Scala：折叠
来源：http://mobile.yfazqb.com/Article/details/gfhknsaie.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.vehdjk.com/Article/details/gqhriblgd.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfqqfinol.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/gmigqapyz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjolqksjt.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.sjlbkw.cn/Article/details/gyocstweh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.bbcook.cn/Article/details/gvybxbsbj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.yfazqb.com/Article/details/gfhlsvcom.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fktsv.cn/Article/details/gbkkwpmto.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fktsv.cn/Article/details/gtuhapebr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.epnwcf.com/Article/details/gcrtbgnfh.sHtML

[U04] Py：变量调试打印
来源：http://blog.epnwcf.com/Article/details/gqpdpirwi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.vehdjk.com/Article/details/gthbeuoyf.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fktsv.cn/Article/details/gbhqprzxh.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.tarul.cn/Article/details/gbxwgopke.sHtML

[U06] Py：合并两个字典
来源：http://baike.bbcook.cn/Article/details/gbcubtshv.sHtML

{**a, **b}
来源：http://mobile.tarul.cn/Article/details/gjhirruty.sHtML

[U07] Py：反转字典键值
来源：http://baike.bbcook.cn/Article/details/graptjehs.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.vehdjk.com/Article/details/ggxikphha.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fktsv.cn/Article/details/gliqqdkjq.sHtML

[y for x in nested for y in x]
来源：http://3g.sjlbkw.cn/Article/details/gjwgelwee.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.bbcook.cn/Article/details/gaeijnlyc.sHtML

max(d, key=d.get)
来源：http://blog.bbcook.cn/Article/details/gjioonfar.sHtML

[U10] Py：按值排序字典
来源：http://blog.vehdjk.com/Article/details/gczeyqnfi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.sjlbkw.cn/Article/details/glsbuhneo.sHtML

[U11] Py：生成器表达式
来源：http://wap.bbcook.cn/Article/details/gnlywnriw.sHtML

(x * 2 for x in arr)
来源：http://3g.sjlbkw.cn/Article/details/gdhldfgrl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fktsv.cn/Article/details/gydvsccbi.sHtML

Counter(arr).most_common(3)
来源：http://3g.bbcook.cn/Article/details/gojqoewiw.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.yfazqb.com/Article/details/gjhaerjzd.sHtML

deque(maxlen=10)
来源：http://mobile.tarul.cn/Article/details/gytwlvxqf.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fktsv.cn/Article/details/gnmfeowvs.sHtML

defaultdict(list)
来源：http://3g.bbcook.cn/Article/details/gkmzpjzvq.sHtML

[U15] Py：高精度计时
来源：http://read.share.tarul.cn/Article/details/gifbndhgp.sHtML

t = time.perf_counter()
来源：http://read.share.vehdjk.com/Article/details/gfnbcehsh.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fktsv.cn/Article/details/gnikxfvpp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.tarul.cn/Article/details/gcevmgpgi.sHtML

[U17] Py：初始化日志
来源：http://baike.yfazqb.com/Article/details/gijnaxhmu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.epnwcf.com/Article/details/gqzbsdyzt.sHtML

[U18] Py：预编译正则
来源：http://wap.fktsv.cn/Article/details/ggiyjwjvn.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gyabdrcdc.sHtML

[U19] Py：正则替换带回调
来源：http://baike.sjlbkw.cn/Article/details/guaawlzza.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.epnwcf.com/Article/details/gcjzkxsid.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.sjlbkw.cn/Article/details/gzwpezoas.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.sjlbkw.cn/Article/details/gfgwuzogn.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.epnwcf.com/Article/details/gjvnlesre.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/gbstioplu.sHtML

[U22] Py：矩阵转置
来源：http://m.share.vehdjk.com/Article/details/gsciphlsv.sHtML

list(zip(*m))
来源：http://baike.bbcook.cn/Article/details/gtrtcdqjm.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.sjlbkw.cn/Article/details/gesekinay.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.tarul.cn/Article/details/gekreyasi.sHtML

[U24] Py：路径操作
来源：http://www.blog.vehdjk.com/Article/details/goackxpfr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.vehdjk.com/Article/details/gwnkbrmhs.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.tarul.cn/Article/details/gsqnzzqnp.sHtML

csv.DictReader(f)
来源：http://read.share.vehdjk.com/Article/details/gelswegnt.sHtML

[U26] Py：并发下载
来源：http://www.blog.epnwcf.com/Article/details/gkykoemkm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fktsv.cn/Article/details/gmzrzqhcx.sHtML

[U27] Py：异步 HTTP
来源：http://wap.vehdjk.com/Article/details/ggbhkdeln.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.bbcook.cn/Article/details/gxyvmamrz.sHtML

[U28] Py：类型别名
来源：http://baike.bbcook.cn/Article/details/gmzqmhbuq.sHtML

UserId = int
来源：http://3g.sjlbkw.cn/Article/details/gpzrpxrly.sHtML

[U29] Py：属性校验
来源：http://www.m.share.tarul.cn/Article/details/gptxlgnua.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gvstuxmgo.sHtML

[U30] Py：数据类
来源：http://3g.vehdjk.com/Article/details/guqjnxcsl.sHtML

@dataclass(slots=True)
来源：http://read.share.sjlbkw.cn/Article/details/gpzoesqms.sHtML

[U31] Py：单测
来源：http://read.share.vehdjk.com/Article/details/gzydywgrc.sHtML

python -m pytest -q
来源：http://www.share.bbcook.cn/Article/details/gijetlotf.sHtML

[U32] Py：代码格式化
来源：http://baike.epnwcf.com/Article/details/gqmwomnjd.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.bbcook.cn/Article/details/gdyaeipca.sHtML

[U33] Py：打包发布
来源：http://www.blog.epnwcf.com/Article/details/gcdtdnepy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.yfazqb.com/Article/details/gpjrrcosn.sHtML

[U34] Py：判断编码
来源：http://www.m.share.bbcook.cn/Article/details/gdziecshz.sHtML

chardet.detect(raw)
来源：http://wap.yfazqb.com/Article/details/gcvxpcnyi.sHtML

[U35] Py：发送邮件
来源：http://www.blog.bbcook.cn/Article/details/gvjwkgjtr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.vehdjk.com/Article/details/gbzbgmcva.sHtML

[U36] Py：定时任务
来源：http://3g.tarul.cn/Article/details/gjzwsnjkw.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.tarul.cn/Article/details/gonnsnevt.sHtML

[U37] Py：读写 Excel
来源：http://blog.epnwcf.com/Article/details/gaocnyybc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.epnwcf.com/Article/details/gmctpbeig.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.bbcook.cn/Article/details/gboxkyvhm.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.bbcook.cn/Article/details/gmsaeusbs.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.vehdjk.com/Article/details/gigyqrwvi.sHtML

sys.stdout.isatty()
来源：http://www.blog.yfazqb.com/Article/details/gfdjigyzp.sHtML

[U40] Py：打印到标准错误
来源：http://blog.bbcook.cn/Article/details/gaqcmvmxk.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gnevnapsr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.yfazqb.com/Article/details/gjhvlzdjg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.vehdjk.com/Article/details/gzqlmlrrp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.bbcook.cn/Article/details/ghyoythrt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.epnwcf.com/Article/details/gfqyyhnny.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.sjlbkw.cn/Article/details/gtrceghhr.sHtML

namespace App\Http;
来源：http://m.share.epnwcf.com/Article/details/gjkkbizhv.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.tarul.cn/Article/details/gakwnkbag.sHtML

declare(strict_types=1);
来源：http://m.share.vehdjk.com/Article/details/galehnjpi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.sjlbkw.cn/Article/details/ggelrrrcd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gmudehuij.sHtML

[U46] PHP：可空类型
来源：http://baike.fktsv.cn/Article/details/garbzykzl.sHtML

?string $name = null
来源：http://3g.tarul.cn/Article/details/gvozkfzld.sHtML

[U47] PHP：联合类型
来源：http://read.share.fktsv.cn/Article/details/gtwxnhuan.sHtML

int|string $id
来源：http://baike.sjlbkw.cn/Article/details/gpfqymooz.sHtML

[U48] PHP：纯枚举
来源：http://wap.yfazqb.com/Article/details/ggamzurmo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.vehdjk.com/Article/details/gtttcpssp.sHtML

[U49] PHP：只读属性
来源：http://mobile.tarul.cn/Article/details/gqfllptig.sHtML

public readonly string $name
来源：http://3g.epnwcf.com/Article/details/gyterqtlz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.vehdjk.com/Article/details/gwutdsrww.sHtML

public function __construct(private int $id) {}
来源：http://3g.tarul.cn/Article/details/gzpcgsleo.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.tarul.cn/Article/details/ggtmjwvnk.sHtML

[$a, $b] = $arr;
来源：http://3g.sjlbkw.cn/Article/details/gkwsgpyky.sHtML

[U52] PHP：箭头函数
来源：http://m.share.sjlbkw.cn/Article/details/gtoclfuqy.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.epnwcf.com/Article/details/ghnqdkoot.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.epnwcf.com/Article/details/gjlpccquy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.epnwcf.com/Article/details/gqeaszgix.sHtML

[U54] PHP：空安全调用
来源：http://read.share.yfazqb.com/Article/details/gxvtuskcp.sHtML

$obj?->method()
来源：http://baike.vehdjk.com/Article/details/grxtbewcg.sHtML

[U55] PHP：match 表达式
来源：http://read.share.yfazqb.com/Article/details/gvhaavebo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.vehdjk.com/Article/details/gkurvhmcj.sHtML

[U56] PHP：命名参数
来源：http://3g.sjlbkw.cn/Article/details/ggrqcfsim.sHtML

f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/ghphylmol.sHtML

[U57] PHP：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gpaoigash.sHtML

"值: {$a}"
来源：http://m.share.vehdjk.com/Article/details/gussplxce.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.bbcook.cn/Article/details/gjamuykdo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.epnwcf.com/Article/details/gnlmlxtwo.sHtML

[U59] PHP：自定义排序
来源：http://m.share.sjlbkw.cn/Article/details/goxrceokl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqoirjfpz.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.yfazqb.com/Article/details/ghednkqkw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.yfazqb.com/Article/details/geqisyxsz.sHtML

[U61] PHP：正则
来源：http://blog.yfazqb.com/Article/details/gbeefamzq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/gwoyhaqeq.sHtML

[U62] PHP：日期对象
来源：http://read.share.fktsv.cn/Article/details/gsskdvvlq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.yfazqb.com/Article/details/gpzfkcuaq.sHtML

[U63] PHP：文件读写
来源：http://read.share.fktsv.cn/Article/details/grwxywxmv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fktsv.cn/Article/details/ginbrjukr.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.yfazqb.com/Article/details/gzoqxzmds.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fktsv.cn/Article/details/gkmbznqte.sHtML

[U65] PHP：会话
来源：http://baike.sjlbkw.cn/Article/details/geenbgdeb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.vehdjk.com/Article/details/ghspdrbdc.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.vehdjk.com/Article/details/ghzxjclof.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.epnwcf.com/Article/details/gblagnhql.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.yfazqb.com/Article/details/giieswltx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.sjlbkw.cn/Article/details/gubhawdqm.sHtML

[U68] PHP：PDO 连接
来源：http://blog.sjlbkw.cn/Article/details/gyobyhqkr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.sjlbkw.cn/Article/details/gjtjqoibk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gonzpzdtj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.sjlbkw.cn/Article/details/gqfahjorr.sHtML

[U70] PHP：PDO 事务
来源：http://wap.sjlbkw.cn/Article/details/gxnzmhrll.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.vehdjk.com/Article/details/gtgxsydxv.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/gnfpezvth.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.tarul.cn/Article/details/gqpaprzri.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.vehdjk.com/Article/details/gmuzoemvr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.sjlbkw.cn/Article/details/gvvvnioum.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.vehdjk.com/Article/details/gpcmhhmnp.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.bbcook.cn/Article/details/gyrjfsyub.sHtML

[U74] PHP：读取环境变量
来源：http://baike.vehdjk.com/Article/details/gzfiptwbl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.bbcook.cn/Article/details/gifvrjpjr.sHtML

[U75] PHP：依赖注入
来源：http://blog.yfazqb.com/Article/details/gswpcoqjs.sHtML

composer require psr/container
来源：http://3g.tarul.cn/Article/details/gfzrzpqcu.sHtML

[U76] PHP：简单路由
来源：http://mobile.vehdjk.com/Article/details/gxxbhytor.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.sjlbkw.cn/Article/details/gxdgyfqjx.sHtML

[U77] PHP：模板渲染
来源：http://blog.vehdjk.com/Article/details/gtmnmrzkg.sHtML

composer require twig/twig
来源：http://baike.sjlbkw.cn/Article/details/gsphyxhqf.sHtML

[U78] PHP：单元测试
来源：http://blog.yfazqb.com/Article/details/gbmbxvarc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.sjlbkw.cn/Article/details/gfqbrhdlz.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjyjijej.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.yfazqb.com/Article/details/gpoxfxndq.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.vehdjk.com/Article/details/gerjphlcw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.sjlbkw.cn/Article/details/gpxbmjtbl.sHtML

[U81] JS：初始化项目
来源：http://read.share.sjlbkw.cn/Article/details/gkspighwt.sHtML

npm init -y;  npm i express
来源：http://www.m.share.vehdjk.com/Article/details/gkfpwscju.sHtML

[U82] JS：package.json 脚本
来源：http://baike.bbcook.cn/Article/details/glruxgqel.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.bbcook.cn/Article/details/ghevgdixk.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.bbcook.cn/Article/details/glrdxkpne.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gmxagnwov.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.bbcook.cn/Article/details/ghprkeriv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.epnwcf.com/Article/details/gxtbppwxj.sHtML

[U85] JS：可选链
来源：http://wap.bbcook.cn/Article/details/gqjdvcvvv.sHtML

a?.b?.c
来源：http://blog.vehdjk.com/Article/details/ghapmgcbr.sHtML

[U86] JS：空值合并
来源：http://blog.fktsv.cn/Article/details/gqftmator.sHtML

a ?? b
来源：http://m.share.bbcook.cn/Article/details/gjeswydih.sHtML

[U87] JS：解构默认值
来源：http://mobile.fktsv.cn/Article/details/gyujjwqmb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.yfazqb.com/Article/details/ghoxqreqh.sHtML

[U88] JS：对象展开合并
来源：http://3g.vehdjk.com/Article/details/gmbtgdvjr.sHtML

{ ...a, ...b }
来源：http://mobile.sjlbkw.cn/Article/details/gpkbabjhi.sHtML

[U89] JS：数组去重
来源：http://m.share.vehdjk.com/Article/details/ggwyirsjb.sHtML

[...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gicptgfgd.sHtML

[U90] JS：数字数组排序
来源：http://3g.tarul.cn/Article/details/gvipuvuoq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gdjzhivwb.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.vehdjk.com/Article/details/gjpvcgcdr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.tarul.cn/Article/details/goyodbvjj.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gaiykkocu.sHtML

structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/grmlhpynk.sHtML

[U93] JS：模板字符串
来源：http://baike.vehdjk.com/Article/details/gdaraogei.sHtML

`共 ${n} 条`
来源：http://blog.fktsv.cn/Article/details/gtsdwdzhm.sHtML

[U94] JS：箭头函数
来源：http://blog.yfazqb.com/Article/details/gjivyuddn.sHtML

const double = x => x * 2;
来源：http://read.share.epnwcf.com/Article/details/gjesbhuji.sHtML

[U95] JS：Promise 包装
来源：http://mobile.sjlbkw.cn/Article/details/guuwnlemi.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.bbcook.cn/Article/details/gdtifwunp.sHtML

[U96] JS：async/await 与异常
来源：http://blog.bbcook.cn/Article/details/goaunndql.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gkmvfpkap.sHtML

[U97] JS：并发请求
来源：http://blog.fktsv.cn/Article/details/gnnkdtzsv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gtywbarvj.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fktsv.cn/Article/details/gpcdulnbx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.bbcook.cn/Article/details/gphssbgwu.sHtML

[U99] JS：事件监听
来源：http://3g.vehdjk.com/Article/details/gwuuiijle.sHtML

el.addEventListener("click", e => {})
来源：http://3g.tarul.cn/Article/details/gfcwnhhag.sHtML

[U100] JS：DOM 查询
来源：http://blog.tarul.cn/Article/details/gtxiioaht.sHtML

document.querySelector(".item")
来源：http://baike.bbcook.cn/Article/details/gxzydtdfi.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.bbcook.cn/Article/details/gbfimgwkb.sHtML

el.classList.toggle("active")
来源：http://www.share.bbcook.cn/Article/details/grudaychq.sHtML

[U102] JS：本地存储
来源：http://wap.epnwcf.com/Article/details/gnfgagwli.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.sjlbkw.cn/Article/details/gmtkdygwf.sHtML

[U103] JS：定时器
来源：http://blog.vehdjk.com/Article/details/gmxtnmnmb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.yfazqb.com/Article/details/gotedbqdp.sHtML

[U104] JS：防抖
来源：http://www.blog.vehdjk.com/Article/details/gbtkgsnoe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gehpuqzfa.sHtML

[U105] JS：节流
来源：http://3g.epnwcf.com/Article/details/gqlwnynig.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.epnwcf.com/Article/details/gabwqgomc.sHtML

[U106] JS：日期格式化
来源：http://wap.bbcook.cn/Article/details/gqmuycyoc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.epnwcf.com/Article/details/gwyalmzhr.sHtML

[U107] JS：数字千分位
来源：http://3g.yfazqb.com/Article/details/gyrooymna.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gmcxuqjei.sHtML

[U108] JS：随机整数
来源：http://www.m.share.epnwcf.com/Article/details/gjhjttctz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.yfazqb.com/Article/details/guqrfpvvv.sHtML

[U109] JS：数组分组
来源：http://read.share.yfazqb.com/Article/details/gnpznsvez.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/gpgbqsnqa.sHtML

[U110] JS：数组分块
来源：http://mobile.bbcook.cn/Article/details/gthmucxhl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.yfazqb.com/Article/details/gupycdpmm.sHtML

[U111] JS：对象转 Map
来源：http://mobile.bbcook.cn/Article/details/gcjbbkgad.sHtML

new Map(Object.entries(obj))
来源：http://read.share.vehdjk.com/Article/details/goplzxyuj.sHtML

[U112] JS：字符串补位
来源：http://www.blog.bbcook.cn/Article/details/gzxozrkur.sHtML

"7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/gpzcixkph.sHtML

[U113] JS：正则替换全部
来源：http://blog.tarul.cn/Article/details/gnivyjsju.sHtML

s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gtuprzwcn.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.vehdjk.com/Article/details/gxtpjthxy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gttskzwfl.sHtML

[U115] JS：生成 UUID
来源：http://baike.epnwcf.com/Article/details/gfaqbjcbw.sHtML

crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/govwtpcfd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.sjlbkw.cn/Article/details/gkvasykqy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.bbcook.cn/Article/details/glyqwaino.sHtML

[U117] JS：单元测试
来源：http://m.share.tarul.cn/Article/details/gexkgwbag.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.epnwcf.com/Article/details/ggmltmqal.sHtML

[U118] JS：开发服务器
来源：http://www.blog.yfazqb.com/Article/details/ghdvkaycz.sHtML

npm i -D vite;  npx vite
来源：http://blog.yfazqb.com/Article/details/goqwfltrn.sHtML

[U119] JS：生产构建
来源：http://www.share.fktsv.cn/Article/details/goivjdhcl.sHtML

npx vite build
来源：http://www.blog.epnwcf.com/Article/details/ghwkhpwmo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.epnwcf.com/Article/details/guiykmoqt.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.vehdjk.com/Article/details/gmwfpmisc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gauhqgzsb.sHtML

统计汇总
来源：http://m.share.fktsv.cn/Article/details/guddmvppa.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvujjszel.sHtML

按语言统计（条）：
来源：http://baike.yfazqb.com/Article/details/goggxxoxk.sHtML

Python ......... 252
来源：http://www.share.epnwcf.com/Article/details/ggonqnlso.sHtML

PHP ............ 252
来源：http://www.m.share.bbcook.cn/Article/details/gqdsxjayf.sHtML

JavaScript ..... 252
来源：http://www.blog.bbcook.cn/Article/details/gbgnmtvcp.sHtML

TypeScript ..... 212
来源：http://blog.vehdjk.com/Article/details/gvxkabtun.sHtML

Java ........... 212
来源：http://read.share.fktsv.cn/Article/details/gqrqmyfkj.sHtML

Go ............. 212
来源：http://baike.tarul.cn/Article/details/gougvcbdp.sHtML

Ruby ........... 212
来源：http://mobile.epnwcf.com/Article/details/gstqsmsgx.sHtML

C# ............. 212
来源：http://blog.yfazqb.com/Article/details/gssaphqju.sHtML

C .............. 30
来源：http://www.blog.fktsv.cn/Article/details/gmvmppvhp.sHtML

C++ ............ 30
来源：http://m.share.vehdjk.com/Article/details/gprxiwdet.sHtML

SQL ............ 90
来源：http://baike.bbcook.cn/Article/details/gquylpnkh.sHtML

Bash ........... 80
来源：http://blog.fktsv.cn/Article/details/ghncodwgu.sHtML

Kotlin ......... 15
来源：http://mobile.tarul.cn/Article/details/ggyrosqpv.sHtML

Swift .......... 15
来源：http://3g.bbcook.cn/Article/details/glujyhoru.sHtML

Lua ............ 10
来源：http://mobile.tarul.cn/Article/details/grmpjtuch.sHtML

Perl ........... 10
来源：http://mobile.yfazqb.com/Article/details/gnkrabwdf.sHtML

Scala .......... 10
来源：http://3g.fktsv.cn/Article/details/gokavobjm.sHtML

------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gmoacpbcz.sHtML

合计 ........... 2106 条
来源：http://m.share.bbcook.cn/Article/details/gqbtdsrxy.sHtML

按章节统计：
来源：http://www.m.share.tarul.cn/Article/details/gifwysxxc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.sjlbkw.cn/Article/details/gkxkflsfk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gfkuszutb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gjzfatpgp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.yfazqb.com/Article/details/gcdwmgizb.sHtML


<!-- 参考信息 -->