代发 wailian999

[T43] Perl：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gwsbpnhdm.sHtML

"值: $a"
来源：http://3g.yfazqb.com/Article/details/goneupsqy.sHtML

[T44] Perl：条件
来源：http://www.blog.epnwcf.com/Article/details/gsmeewhki.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.vehdjk.com/Article/details/grraufane.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.yfazqb.com/Article/details/gqoqudkcg.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.yfazqb.com/Article/details/gkcjvavxv.sHtML

[T46] Perl：哈希操作
来源：http://baike.tarul.cn/Article/details/gczvsowuv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.epnwcf.com/Article/details/gdjgxuvmd.sHtML

[T47] Perl：正则捕获
来源：http://blog.bbcook.cn/Article/details/gsglxjrlz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fktsv.cn/Article/details/glprnylju.sHtML

[T48] Perl：正则替换
来源：http://www.blog.tarul.cn/Article/details/guptbzhbd.sHtML

$s =~ s/old/new/g;
来源：http://3g.sjlbkw.cn/Article/details/gqtyjmwph.sHtML

[T49] Perl：函数
来源：http://www.m.share.yfazqb.com/Article/details/gyyowytry.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gmuniumjr.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gdtxebgkx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.yfazqb.com/Article/details/galdfvrrm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fktsv.cn/Article/details/gmqlxxfov.sHtML

[T51] Scala：Hello World
来源：http://www.share.fktsv.cn/Article/details/gotslioig.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/gwpzzdstp.sHtML

[T52] Scala：变量
来源：http://www.share.tarul.cn/Article/details/graxrgixu.sHtML

val a = 1;  var b = 2
来源：http://www.blog.tarul.cn/Article/details/gnrrdslmi.sHtML

[T53] Scala：字符串插值
来源：http://m.share.bbcook.cn/Article/details/ggoqeovcx.sHtML

s"值: $b"
来源：http://baike.vehdjk.com/Article/details/gunantzwt.sHtML

[T54] Scala：集合映射
来源：http://blog.bbcook.cn/Article/details/gzolumatt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.bbcook.cn/Article/details/gjmmccdps.sHtML

[T55] Scala：集合过滤
来源：http://baike.fktsv.cn/Article/details/gductuslm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqaphcdk.sHtML

[T56] Scala：样例类
来源：http://www.share.epnwcf.com/Article/details/gemxsaabx.sHtML

case class User(name: String, age: Int)
来源：http://baike.vehdjk.com/Article/details/gdawvvese.sHtML

[T57] Scala：模式匹配
来源：http://m.share.bbcook.cn/Article/details/gsotvarsy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.bbcook.cn/Article/details/gmrspmhdn.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.yfazqb.com/Article/details/ggvrftjjh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fktsv.cn/Article/details/gluizaoed.sHtML

[T59] Scala：循环
来源：http://m.share.yfazqb.com/Article/details/gayrcbhdh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gasybmunk.sHtML

[T60] Scala：折叠
来源：http://www.m.share.vehdjk.com/Article/details/gkobtvjxy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.bbcook.cn/Article/details/ghnbtugdn.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gybgwnzaw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/ggbbhjpam.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/guzcyiqdj.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.bbcook.cn/Article/details/gtvroozgm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fktsv.cn/Article/details/gmtcrgthb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.vehdjk.com/Article/details/gqsviftam.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fktsv.cn/Article/details/gbdxciqio.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.sjlbkw.cn/Article/details/gvccizbat.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.sjlbkw.cn/Article/details/ghtgjethf.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.bbcook.cn/Article/details/glybdfbrj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.tarul.cn/Article/details/gutizkjcl.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fktsv.cn/Article/details/gefeurwqf.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.tarul.cn/Article/details/gviyphqaf.sHtML

[U06] Py：合并两个字典
来源：http://baike.fktsv.cn/Article/details/gcsxcdnhc.sHtML

{**a, **b}
来源：http://blog.tarul.cn/Article/details/gmxslcies.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/gqpvddlad.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.epnwcf.com/Article/details/gnkqcabbv.sHtML

[U08] Py：展平二维列表
来源：http://baike.sjlbkw.cn/Article/details/gsyykbqpo.sHtML

[y for x in nested for y in x]
来源：http://m.share.tarul.cn/Article/details/gvvoouytk.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.bbcook.cn/Article/details/gyqrhesba.sHtML

max(d, key=d.get)
来源：http://m.share.bbcook.cn/Article/details/gzfymxegx.sHtML

[U10] Py：按值排序字典
来源：http://wap.tarul.cn/Article/details/glkmbgfnj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.tarul.cn/Article/details/gfjbraeln.sHtML

[U11] Py：生成器表达式
来源：http://mobile.tarul.cn/Article/details/gqvdkyvim.sHtML

(x * 2 for x in arr)
来源：http://mobile.tarul.cn/Article/details/gffjtxaal.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.vehdjk.com/Article/details/ggfsnimxo.sHtML

Counter(arr).most_common(3)
来源：http://baike.epnwcf.com/Article/details/gndqjapft.sHtML

[U13] Py：固定长度队列
来源：http://read.share.vehdjk.com/Article/details/gmhsbdwtf.sHtML

deque(maxlen=10)
来源：http://blog.tarul.cn/Article/details/goqnbizip.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fktsv.cn/Article/details/gzenhacfr.sHtML

defaultdict(list)
来源：http://www.share.vehdjk.com/Article/details/garvfsakg.sHtML

[U15] Py：高精度计时
来源：http://wap.vehdjk.com/Article/details/gixdarhfq.sHtML

t = time.perf_counter()
来源：http://blog.sjlbkw.cn/Article/details/gxgarsqvt.sHtML

[U16] Py：命令行参数解析
来源：http://baike.bbcook.cn/Article/details/gcqyfccjn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fktsv.cn/Article/details/goekiytkn.sHtML

[U17] Py：初始化日志
来源：http://read.share.sjlbkw.cn/Article/details/gdgmveljr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.tarul.cn/Article/details/gyxmpfynr.sHtML

[U18] Py：预编译正则
来源：http://wap.tarul.cn/Article/details/gtfnregsb.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.tarul.cn/Article/details/guydqajpc.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.yfazqb.com/Article/details/gmhpggxhi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.sjlbkw.cn/Article/details/gskwkquzp.sHtML

[U20] Py：缓存函数结果
来源：http://wap.vehdjk.com/Article/details/gwbaeuqzp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.bbcook.cn/Article/details/gmjkjljxd.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.yfazqb.com/Article/details/gjfxjsjgn.sHtML

@contextlib.contextmanager
来源：http://baike.epnwcf.com/Article/details/gsfscgxjb.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.sjlbkw.cn/Article/details/glyiljzgx.sHtML

list(zip(*m))
来源：http://blog.fktsv.cn/Article/details/glkvkylbc.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.yfazqb.com/Article/details/gfttqmvqb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.sjlbkw.cn/Article/details/gapohoplo.sHtML

[U24] Py：路径操作
来源：http://read.share.epnwcf.com/Article/details/ghoyvwmur.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gzcpoawds.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.yfazqb.com/Article/details/gsogsdmry.sHtML

csv.DictReader(f)
来源：http://www.share.fktsv.cn/Article/details/gizmmkpzz.sHtML

[U26] Py：并发下载
来源：http://mobile.tarul.cn/Article/details/gvhuffoet.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.bbcook.cn/Article/details/goplbxfyv.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.tarul.cn/Article/details/gzzkywyre.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fktsv.cn/Article/details/gfgbtvdes.sHtML

[U28] Py：类型别名
来源：http://blog.epnwcf.com/Article/details/gbpafsahp.sHtML

UserId = int
来源：http://www.share.fktsv.cn/Article/details/gdbiourib.sHtML

[U29] Py：属性校验
来源：http://wap.fktsv.cn/Article/details/gifybbkqk.sHtML

@property 与 @x.setter 配合
来源：http://m.share.sjlbkw.cn/Article/details/gqyzlmtem.sHtML

[U30] Py：数据类
来源：http://mobile.tarul.cn/Article/details/gjjuqmchc.sHtML

@dataclass(slots=True)
来源：http://www.share.tarul.cn/Article/details/gdpttvzay.sHtML

[U31] Py：单测
来源：http://3g.bbcook.cn/Article/details/gwdoejgkm.sHtML

python -m pytest -q
来源：http://www.share.sjlbkw.cn/Article/details/gsubrzbcr.sHtML

[U32] Py：代码格式化
来源：http://blog.tarul.cn/Article/details/ghmofrnsg.sHtML

ruff format . && ruff check --fix .
来源：http://blog.sjlbkw.cn/Article/details/gozomuykj.sHtML

[U33] Py：打包发布
来源：http://wap.bbcook.cn/Article/details/gdwuljdxf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.epnwcf.com/Article/details/gqwrwejew.sHtML

[U34] Py：判断编码
来源：http://baike.vehdjk.com/Article/details/gprnalzpd.sHtML

chardet.detect(raw)
来源：http://3g.epnwcf.com/Article/details/gwvreewdg.sHtML

[U35] Py：发送邮件
来源：http://www.share.tarul.cn/Article/details/gormjdbtd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.tarul.cn/Article/details/gyecyoszn.sHtML

[U36] Py：定时任务
来源：http://m.share.bbcook.cn/Article/details/gafpabjyi.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.tarul.cn/Article/details/givdjwukx.sHtML

[U37] Py：读写 Excel
来源：http://read.share.sjlbkw.cn/Article/details/grgstauay.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.vehdjk.com/Article/details/ggauphozv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.yfazqb.com/Article/details/giaeraqdw.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.bbcook.cn/Article/details/gsayhsniz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.yfazqb.com/Article/details/gyvcpahna.sHtML

sys.stdout.isatty()
来源：http://www.share.bbcook.cn/Article/details/golbjioya.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.tarul.cn/Article/details/grdrolczr.sHtML

print("err", file=sys.stderr)
来源：http://m.share.sjlbkw.cn/Article/details/gpugolizx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.sjlbkw.cn/Article/details/gdkbiejay.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.epnwcf.com/Article/details/gjexcsjmm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.vehdjk.com/Article/details/gunrirsgu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.epnwcf.com/Article/details/ghwjchbbn.sHtML

[U43] PHP：声明命名空间
来源：http://blog.tarul.cn/Article/details/gesyjcwsi.sHtML

namespace App\Http;
来源：http://read.share.vehdjk.com/Article/details/gssswthrp.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fktsv.cn/Article/details/gtebvynge.sHtML

declare(strict_types=1);
来源：http://m.share.tarul.cn/Article/details/gmaxzthgr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fktsv.cn/Article/details/gigxwsepz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gycudqbzn.sHtML

[U46] PHP：可空类型
来源：http://3g.bbcook.cn/Article/details/gcsabcwcp.sHtML

?string $name = null
来源：http://www.share.yfazqb.com/Article/details/gsunkxwth.sHtML

[U47] PHP：联合类型
来源：http://3g.vehdjk.com/Article/details/ghsmwbplk.sHtML

int|string $id
来源：http://www.blog.bbcook.cn/Article/details/gtecsnyxa.sHtML

[U48] PHP：纯枚举
来源：http://3g.epnwcf.com/Article/details/gwbjethzg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.epnwcf.com/Article/details/gqbafrlqg.sHtML

[U49] PHP：只读属性
来源：http://3g.fktsv.cn/Article/details/gmyrvloav.sHtML

public readonly string $name
来源：http://3g.fktsv.cn/Article/details/gvwnrsnrc.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.vehdjk.com/Article/details/gwcdrqpjv.sHtML

public function __construct(private int $id) {}
来源：http://blog.bbcook.cn/Article/details/giqofzwby.sHtML

[U51] PHP：数组解构
来源：http://www.share.fktsv.cn/Article/details/gdujjjskq.sHtML

[$a, $b] = $arr;
来源：http://m.share.vehdjk.com/Article/details/grkhpreuu.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.bbcook.cn/Article/details/gwiaxtjnc.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.yfazqb.com/Article/details/gijjtvels.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.vehdjk.com/Article/details/gecvbaqkb.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.sjlbkw.cn/Article/details/gxgtsgndt.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.bbcook.cn/Article/details/gmaygkyki.sHtML

$obj?->method()
来源：http://blog.sjlbkw.cn/Article/details/grkpalwja.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.yfazqb.com/Article/details/gzfuykdce.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.bbcook.cn/Article/details/gvocsyrgl.sHtML

[U56] PHP：命名参数
来源：http://baike.sjlbkw.cn/Article/details/gdttbvxdh.sHtML

f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/guwxdtbvc.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gqwbqvplm.sHtML

"值: {$a}"
来源：http://baike.fktsv.cn/Article/details/gsbwyxzax.sHtML

[U58] PHP：数组三件套
来源：http://baike.yfazqb.com/Article/details/gbaevkioo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.tarul.cn/Article/details/gqpxsxhvt.sHtML

[U59] PHP：自定义排序
来源：http://blog.fktsv.cn/Article/details/gyfwmzohc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.bbcook.cn/Article/details/gvuzimkhh.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.bbcook.cn/Article/details/gooaucltq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.bbcook.cn/Article/details/gyjocbxca.sHtML

[U61] PHP：正则
来源：http://mobile.bbcook.cn/Article/details/gfvmtsqgb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/girsalndt.sHtML

[U62] PHP：日期对象
来源：http://baike.vehdjk.com/Article/details/gcpodrunu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.epnwcf.com/Article/details/gnxvtcofq.sHtML

[U63] PHP：文件读写
来源：http://blog.epnwcf.com/Article/details/gvwytyqms.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.sjlbkw.cn/Article/details/gxorpneuk.sHtML

[U64] PHP：目录遍历
来源：http://blog.sjlbkw.cn/Article/details/gwznwhmzi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.bbcook.cn/Article/details/gcmashihc.sHtML

[U65] PHP：会话
来源：http://3g.vehdjk.com/Article/details/geovqavps.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gpincbpni.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.vehdjk.com/Article/details/gcespagnb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.tarul.cn/Article/details/gpdwquvdh.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.sjlbkw.cn/Article/details/gjedkqlxu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fktsv.cn/Article/details/gyoptqzcr.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.yfazqb.com/Article/details/gibcqssoq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.tarul.cn/Article/details/gidqvawdx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fktsv.cn/Article/details/gzcqbjrmi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.sjlbkw.cn/Article/details/gzdqhqskm.sHtML

[U70] PHP：PDO 事务
来源：http://baike.tarul.cn/Article/details/grxcxcomk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.vehdjk.com/Article/details/gjpycjumb.sHtML

[U71] PHP：抛出异常
来源：http://wap.fktsv.cn/Article/details/gztkysrsa.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.epnwcf.com/Article/details/ggndjgkcq.sHtML

[U72] PHP：写错误日志
来源：http://www.share.tarul.cn/Article/details/ggemuidjc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fktsv.cn/Article/details/gvajnjyei.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.yfazqb.com/Article/details/grdkdjxwv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.tarul.cn/Article/details/gailpxyqc.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gdsdkzbxi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.yfazqb.com/Article/details/ggoylshhk.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.yfazqb.com/Article/details/gujhmpjic.sHtML

composer require psr/container
来源：http://read.share.epnwcf.com/Article/details/gmwyomixh.sHtML

[U76] PHP：简单路由
来源：http://www.blog.vehdjk.com/Article/details/goeunqmhd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.sjlbkw.cn/Article/details/gbknhyeqn.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.yfazqb.com/Article/details/gagcrtacx.sHtML

composer require twig/twig
来源：http://baike.bbcook.cn/Article/details/gjpuzviue.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gxqqzrdlq.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.bbcook.cn/Article/details/gqxtcmcsd.sHtML

[U79] PHP：静态分析
来源：http://www.blog.vehdjk.com/Article/details/ghbxcshke.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.sjlbkw.cn/Article/details/gdvnmzluq.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.vehdjk.com/Article/details/gtmctdhqp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.sjlbkw.cn/Article/details/ghbokzkoa.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fktsv.cn/Article/details/gdrbdzbbd.sHtML

npm init -y;  npm i express
来源：http://www.blog.fktsv.cn/Article/details/gjiixrfxe.sHtML

[U82] JS：package.json 脚本
来源：http://baike.sjlbkw.cn/Article/details/gfzwpulxu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.tarul.cn/Article/details/gfestwzeo.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.yfazqb.com/Article/details/gowhwozrf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/glhieszke.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.sjlbkw.cn/Article/details/groiycvpk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.sjlbkw.cn/Article/details/gruuzmqhm.sHtML

[U85] JS：可选链
来源：http://www.blog.fktsv.cn/Article/details/gnanwhihe.sHtML

a?.b?.c
来源：http://www.m.share.fktsv.cn/Article/details/guntebmrd.sHtML

[U86] JS：空值合并
来源：http://www.blog.bbcook.cn/Article/details/givuwtevx.sHtML

a ?? b
来源：http://www.blog.yfazqb.com/Article/details/gyfzeixls.sHtML

[U87] JS：解构默认值
来源：http://read.share.epnwcf.com/Article/details/gmhfctmix.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.tarul.cn/Article/details/gsxkjuuka.sHtML

[U88] JS：对象展开合并
来源：http://3g.fktsv.cn/Article/details/gfifohavu.sHtML

{ ...a, ...b }
来源：http://baike.bbcook.cn/Article/details/gbxiyutby.sHtML

[U89] JS：数组去重
来源：http://www.m.share.yfazqb.com/Article/details/gpondjxgv.sHtML

[...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gqcnmmmfg.sHtML

[U90] JS：数字数组排序
来源：http://wap.epnwcf.com/Article/details/gxwpljjlq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gicczdpub.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gwucjrlau.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.sjlbkw.cn/Article/details/gzsbkhoix.sHtML

[U92] JS：深拷贝
来源：http://blog.epnwcf.com/Article/details/gegsrawuc.sHtML

structuredClone(obj)
来源：http://m.share.fktsv.cn/Article/details/gjjwgsvsx.sHtML

[U93] JS：模板字符串
来源：http://mobile.epnwcf.com/Article/details/gvtqdxmlh.sHtML

`共 ${n} 条`
来源：http://www.blog.tarul.cn/Article/details/gbrkycmlg.sHtML

[U94] JS：箭头函数
来源：http://blog.yfazqb.com/Article/details/gxsmslgux.sHtML

const double = x => x * 2;
来源：http://read.share.sjlbkw.cn/Article/details/gdkchdfym.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fktsv.cn/Article/details/gistiufpg.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.epnwcf.com/Article/details/gutjbferc.sHtML

[U96] JS：async/await 与异常
来源：http://wap.vehdjk.com/Article/details/gjldjhwwn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gbhxrlcik.sHtML

[U97] JS：并发请求
来源：http://www.blog.sjlbkw.cn/Article/details/gbcxkdgpk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/ghgesenqz.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.yfazqb.com/Article/details/gwktyqlsz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.tarul.cn/Article/details/grcaqotrs.sHtML

[U99] JS：事件监听
来源：http://3g.fktsv.cn/Article/details/gacsfgxck.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.yfazqb.com/Article/details/gcjdrcisl.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.sjlbkw.cn/Article/details/gxigibfrf.sHtML

document.querySelector(".item")
来源：http://wap.tarul.cn/Article/details/gwmmnqkmy.sHtML

[U101] JS：classList 操作
来源：http://baike.bbcook.cn/Article/details/gcbtvjgtf.sHtML

el.classList.toggle("active")
来源：http://blog.tarul.cn/Article/details/glnqhbthi.sHtML

[U102] JS：本地存储
来源：http://m.share.fktsv.cn/Article/details/gzalgwqnl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.tarul.cn/Article/details/gzqcqwksc.sHtML

[U103] JS：定时器
来源：http://read.share.vehdjk.com/Article/details/gcjgsmcrx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.bbcook.cn/Article/details/gxblkzrpe.sHtML

[U104] JS：防抖
来源：http://www.m.share.epnwcf.com/Article/details/gshqnltfs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gcdfjwpmz.sHtML

[U105] JS：节流
来源：http://read.share.epnwcf.com/Article/details/gurebffvi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.bbcook.cn/Article/details/gfdkltsxg.sHtML

[U106] JS：日期格式化
来源：http://www.share.vehdjk.com/Article/details/gbhrwbxua.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.vehdjk.com/Article/details/ghlotargz.sHtML

[U107] JS：数字千分位
来源：http://www.blog.sjlbkw.cn/Article/details/gylzikmat.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.tarul.cn/Article/details/gaqguestj.sHtML

[U108] JS：随机整数
来源：http://www.blog.yfazqb.com/Article/details/gtssneych.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.vehdjk.com/Article/details/gwjkvhbkj.sHtML

[U109] JS：数组分组
来源：http://mobile.sjlbkw.cn/Article/details/gvztrmvnk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/gxjtptjwd.sHtML

[U110] JS：数组分块
来源：http://www.blog.bbcook.cn/Article/details/gmtklzpyu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.sjlbkw.cn/Article/details/gbegyomqm.sHtML

[U111] JS：对象转 Map
来源：http://mobile.yfazqb.com/Article/details/gaptuwojv.sHtML

new Map(Object.entries(obj))
来源：http://blog.tarul.cn/Article/details/gvefzldpy.sHtML

[U112] JS：字符串补位
来源：http://baike.bbcook.cn/Article/details/groxcjlah.sHtML

"7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gepohnyhj.sHtML

[U113] JS：正则替换全部
来源：http://wap.yfazqb.com/Article/details/gftmlyuuh.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gdmfrdhkq.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.tarul.cn/Article/details/gswdcewju.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/girstlbbv.sHtML

[U115] JS：生成 UUID
来源：http://m.share.vehdjk.com/Article/details/gortemjjs.sHtML

crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/ggslwigmq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fktsv.cn/Article/details/gjcplukic.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.bbcook.cn/Article/details/grefffxpy.sHtML

[U117] JS：单元测试
来源：http://www.share.tarul.cn/Article/details/ghnupeill.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.sjlbkw.cn/Article/details/gmafhwuli.sHtML

[U118] JS：开发服务器
来源：http://3g.bbcook.cn/Article/details/glkunysle.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fktsv.cn/Article/details/gdxifjoey.sHtML

[U119] JS：生产构建
来源：http://mobile.bbcook.cn/Article/details/glxnugnoc.sHtML

npx vite build
来源：http://m.share.yfazqb.com/Article/details/gqqimvfxy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fktsv.cn/Article/details/giecompyl.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.sjlbkw.cn/Article/details/ghjcbaede.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmouefnrp.sHtML

统计汇总
来源：http://blog.vehdjk.com/Article/details/gbrmxthnp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/grymthbvf.sHtML

按语言统计（条）：
来源：http://mobile.tarul.cn/Article/details/gkfwwjvba.sHtML

Python ......... 252
来源：http://www.blog.vehdjk.com/Article/details/gngwazbpv.sHtML

PHP ............ 252
来源：http://www.share.fktsv.cn/Article/details/gskpxizxf.sHtML

JavaScript ..... 252
来源：http://www.m.share.fktsv.cn/Article/details/gwfbwpwvh.sHtML

TypeScript ..... 212
来源：http://blog.epnwcf.com/Article/details/gbfqxpdlf.sHtML

Java ........... 212
来源：http://blog.bbcook.cn/Article/details/ggmrcdmwf.sHtML

Go ............. 212
来源：http://blog.vehdjk.com/Article/details/gdhkowuio.sHtML

Ruby ........... 212
来源：http://3g.epnwcf.com/Article/details/gqgglhqji.sHtML

C# ............. 212
来源：http://blog.fktsv.cn/Article/details/gjedmodxx.sHtML

C .............. 30
来源：http://mobile.epnwcf.com/Article/details/gzmuwxhae.sHtML

C++ ............ 30
来源：http://www.m.share.epnwcf.com/Article/details/guqopgjoq.sHtML

SQL ............ 90
来源：http://read.share.sjlbkw.cn/Article/details/gyysomblt.sHtML

Bash ........... 80
来源：http://3g.sjlbkw.cn/Article/details/gcdspssrb.sHtML

Kotlin ......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/ggllmjiik.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/gdfgmykon.sHtML

Lua ............ 10
来源：http://blog.epnwcf.com/Article/details/gxgrqvobi.sHtML

Perl ........... 10
来源：http://blog.fktsv.cn/Article/details/gzvbqvadk.sHtML


<!-- 参考信息 -->