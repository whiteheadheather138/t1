代发 wailian999

[T43] Perl：字符串插值
来源：http://www.share.tarul.cn/Article/details/gfmeutowc.sHtML

"值: $a"
来源：http://www.blog.tarul.cn/Article/details/gruhqaddw.sHtML

[T44] Perl：条件
来源：http://blog.tarul.cn/Article/details/gvwajpbrb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxhluzzlp.sHtML

[T45] Perl：数组遍历
来源：http://blog.tarul.cn/Article/details/gswjkschj.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fktsv.cn/Article/details/gsoawnwov.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fktsv.cn/Article/details/gjiqyqpoo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.epnwcf.com/Article/details/gljmvxxuy.sHtML

[T47] Perl：正则捕获
来源：http://m.share.tarul.cn/Article/details/gucqvdszd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.epnwcf.com/Article/details/gawiijryg.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.bbcook.cn/Article/details/gcrsjkims.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/getxabcqn.sHtML

[T49] Perl：函数
来源：http://www.m.share.tarul.cn/Article/details/gxdxlmjrc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gulcitckl.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gpapazogo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxephordq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fktsv.cn/Article/details/gvayfaidy.sHtML

[T51] Scala：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gtmniszld.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gzaggqoly.sHtML

[T52] Scala：变量
来源：http://3g.bbcook.cn/Article/details/gnuetbwga.sHtML

val a = 1;  var b = 2
来源：http://m.share.epnwcf.com/Article/details/gifjpfirv.sHtML

[T53] Scala：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gdintnwzl.sHtML

s"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/gkocfezhf.sHtML

[T54] Scala：集合映射
来源：http://m.share.tarul.cn/Article/details/gowojthpl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.vehdjk.com/Article/details/gdefmohpg.sHtML

[T55] Scala：集合过滤
来源：http://wap.tarul.cn/Article/details/gvixgjoxd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.bbcook.cn/Article/details/gzhpetdsm.sHtML

[T56] Scala：样例类
来源：http://m.share.epnwcf.com/Article/details/gdeakgxjg.sHtML

case class User(name: String, age: Int)
来源：http://mobile.tarul.cn/Article/details/gtyzinvpj.sHtML

[T57] Scala：模式匹配
来源：http://read.share.epnwcf.com/Article/details/ghevxgjio.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.bbcook.cn/Article/details/gyqmatmig.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.yfazqb.com/Article/details/ghckmswuu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.tarul.cn/Article/details/ggvmlxjxy.sHtML

[T59] Scala：循环
来源：http://www.share.tarul.cn/Article/details/goburmrjm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gahkrlpxb.sHtML

[T60] Scala：折叠
来源：http://read.share.vehdjk.com/Article/details/ghylhvqun.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.sjlbkw.cn/Article/details/gsctuvgib.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gysutbzgp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/gslrhgcke.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/givilsfnl.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.tarul.cn/Article/details/gkxhvxzmx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.bbcook.cn/Article/details/glguknnfk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.yfazqb.com/Article/details/gdclwxeeo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.sjlbkw.cn/Article/details/gxnbotqdu.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.vehdjk.com/Article/details/glhufqcoo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.epnwcf.com/Article/details/gbtviqdmb.sHtML

[U04] Py：变量调试打印
来源：http://baike.yfazqb.com/Article/details/gbbsraygo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gglwoapqo.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.epnwcf.com/Article/details/glvgxwfqj.sHtML

list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/ggwzauvua.sHtML

[U06] Py：合并两个字典
来源：http://blog.tarul.cn/Article/details/gsjjfyjys.sHtML

{**a, **b}
来源：http://blog.yfazqb.com/Article/details/gucidyunq.sHtML

[U07] Py：反转字典键值
来源：http://mobile.tarul.cn/Article/details/gpyriyczh.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fktsv.cn/Article/details/gnhohmoro.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.tarul.cn/Article/details/gthqvsxvp.sHtML

[y for x in nested for y in x]
来源：http://wap.sjlbkw.cn/Article/details/gnxtyzvso.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.yfazqb.com/Article/details/gxvjmlltu.sHtML

max(d, key=d.get)
来源：http://baike.epnwcf.com/Article/details/gauockcbx.sHtML

[U10] Py：按值排序字典
来源：http://read.share.epnwcf.com/Article/details/gsuvydmnr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.epnwcf.com/Article/details/ghlelkarv.sHtML

[U11] Py：生成器表达式
来源：http://baike.bbcook.cn/Article/details/gwycdlowc.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.yfazqb.com/Article/details/gwygvokkw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fktsv.cn/Article/details/glydbuatu.sHtML

Counter(arr).most_common(3)
来源：http://wap.fktsv.cn/Article/details/gootybtzu.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.yfazqb.com/Article/details/goxiaegzl.sHtML

deque(maxlen=10)
来源：http://3g.sjlbkw.cn/Article/details/gfjzolnnl.sHtML

[U14] Py：分组收集到列表
来源：http://3g.epnwcf.com/Article/details/gmbyvxpkd.sHtML

defaultdict(list)
来源：http://mobile.tarul.cn/Article/details/gcknhbztr.sHtML

[U15] Py：高精度计时
来源：http://baike.fktsv.cn/Article/details/gihnodhbp.sHtML

t = time.perf_counter()
来源：http://www.m.share.epnwcf.com/Article/details/gywtmzrbb.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.yfazqb.com/Article/details/gfcfknlzt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.tarul.cn/Article/details/gkogpggtj.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjfeckrb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.epnwcf.com/Article/details/gaeejxrhk.sHtML

[U18] Py：预编译正则
来源：http://3g.vehdjk.com/Article/details/gboxaorkc.sHtML

pat = re.compile(r"\d+")
来源：http://blog.sjlbkw.cn/Article/details/gcdqsrena.sHtML

[U19] Py：正则替换带回调
来源：http://wap.bbcook.cn/Article/details/gssmhkqkv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.epnwcf.com/Article/details/glkifkaor.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.epnwcf.com/Article/details/gpbjjgvlz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.bbcook.cn/Article/details/gocyjxgiq.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.vehdjk.com/Article/details/gycucpwmy.sHtML

@contextlib.contextmanager
来源：http://m.share.epnwcf.com/Article/details/gpztgbimw.sHtML

[U22] Py：矩阵转置
来源：http://mobile.sjlbkw.cn/Article/details/gmwztvprc.sHtML

list(zip(*m))
来源：http://blog.fktsv.cn/Article/details/gwstxccdg.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.bbcook.cn/Article/details/gmxewgcsl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.sjlbkw.cn/Article/details/gzycsqvts.sHtML

[U24] Py：路径操作
来源：http://wap.sjlbkw.cn/Article/details/gvmwuzxly.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/guxqjwaed.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.yfazqb.com/Article/details/gjbpfdqck.sHtML

csv.DictReader(f)
来源：http://read.share.bbcook.cn/Article/details/gwdqpootm.sHtML

[U26] Py：并发下载
来源：http://mobile.bbcook.cn/Article/details/gzwafenvz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.epnwcf.com/Article/details/gfitrbtrl.sHtML

[U27] Py：异步 HTTP
来源：http://blog.bbcook.cn/Article/details/gcjcuhimm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.yfazqb.com/Article/details/gtedpgqes.sHtML

[U28] Py：类型别名
来源：http://wap.yfazqb.com/Article/details/gaomisdbc.sHtML

UserId = int
来源：http://www.share.epnwcf.com/Article/details/gebvzrlog.sHtML

[U29] Py：属性校验
来源：http://mobile.epnwcf.com/Article/details/gvmojfnbe.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gklxixlwq.sHtML

[U30] Py：数据类
来源：http://wap.tarul.cn/Article/details/glnnxpfop.sHtML

@dataclass(slots=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/glgdbspjt.sHtML

[U31] Py：单测
来源：http://www.blog.yfazqb.com/Article/details/goafsicrq.sHtML

python -m pytest -q
来源：http://baike.epnwcf.com/Article/details/gelrgddes.sHtML

[U32] Py：代码格式化
来源：http://www.share.sjlbkw.cn/Article/details/gzcvufzfp.sHtML

ruff format . && ruff check --fix .
来源：http://3g.vehdjk.com/Article/details/ggnfmulrx.sHtML

[U33] Py：打包发布
来源：http://www.m.share.tarul.cn/Article/details/gjorleirh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fktsv.cn/Article/details/gawvrhjus.sHtML

[U34] Py：判断编码
来源：http://www.m.share.vehdjk.com/Article/details/glxkcuupf.sHtML

chardet.detect(raw)
来源：http://mobile.bbcook.cn/Article/details/gvyxxreiy.sHtML

[U35] Py：发送邮件
来源：http://wap.tarul.cn/Article/details/gwlxgcklh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.yfazqb.com/Article/details/gfyrbekqk.sHtML

[U36] Py：定时任务
来源：http://www.blog.bbcook.cn/Article/details/gmzxhpgen.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.sjlbkw.cn/Article/details/gbjjdhlfe.sHtML

[U37] Py：读写 Excel
来源：http://www.share.sjlbkw.cn/Article/details/gnjgvhsbx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fktsv.cn/Article/details/ginhnsuge.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.yfazqb.com/Article/details/gpyjqiomj.sHtML

Path(__file__).resolve().parent
来源：http://blog.yfazqb.com/Article/details/ggunpmebt.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.vehdjk.com/Article/details/gwzwcoxrt.sHtML

sys.stdout.isatty()
来源：http://www.blog.bbcook.cn/Article/details/gjqnyfazj.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.vehdjk.com/Article/details/guxtxiwps.sHtML

print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gjswvxhog.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.epnwcf.com/Article/details/gdjjghszg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.tarul.cn/Article/details/gcvdqopxw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.yfazqb.com/Article/details/gsxridani.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.bbcook.cn/Article/details/gfvjmxnky.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.tarul.cn/Article/details/gcfzukbtb.sHtML

namespace App\Http;
来源：http://3g.bbcook.cn/Article/details/gkuvwfeuj.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.tarul.cn/Article/details/gdajzzuaa.sHtML

declare(strict_types=1);
来源：http://www.m.share.bbcook.cn/Article/details/gyohfrhxg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.yfazqb.com/Article/details/gjfbbqome.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gevhjbdva.sHtML

[U46] PHP：可空类型
来源：http://blog.epnwcf.com/Article/details/gsesixiqs.sHtML

?string $name = null
来源：http://read.share.bbcook.cn/Article/details/gdwabjfpt.sHtML

[U47] PHP：联合类型
来源：http://www.blog.vehdjk.com/Article/details/gakoavewo.sHtML

int|string $id
来源：http://baike.sjlbkw.cn/Article/details/gnjrtkmas.sHtML

[U48] PHP：纯枚举
来源：http://m.share.sjlbkw.cn/Article/details/ggfgeohof.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.tarul.cn/Article/details/gemvpjshp.sHtML

[U49] PHP：只读属性
来源：http://wap.tarul.cn/Article/details/gurymczqc.sHtML

public readonly string $name
来源：http://blog.fktsv.cn/Article/details/gazrxvrgi.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.bbcook.cn/Article/details/gpukosgpf.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.tarul.cn/Article/details/ggvzaqqgw.sHtML

[U51] PHP：数组解构
来源：http://3g.bbcook.cn/Article/details/gakwjhrow.sHtML

[$a, $b] = $arr;
来源：http://wap.sjlbkw.cn/Article/details/ghaxdnwts.sHtML

[U52] PHP：箭头函数
来源：http://wap.epnwcf.com/Article/details/gbzveoxcf.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.vehdjk.com/Article/details/gwhgsbbcp.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.vehdjk.com/Article/details/gspmttebz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.vehdjk.com/Article/details/gvmznufri.sHtML

[U54] PHP：空安全调用
来源：http://www.share.sjlbkw.cn/Article/details/gdhdinayo.sHtML

$obj?->method()
来源：http://mobile.tarul.cn/Article/details/gdhkgrhbm.sHtML

[U55] PHP：match 表达式
来源：http://read.share.sjlbkw.cn/Article/details/gvlqcvena.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.tarul.cn/Article/details/gtpjxbnhk.sHtML

[U56] PHP：命名参数
来源：http://blog.tarul.cn/Article/details/glopnkozd.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gmnugpock.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gipfpujqw.sHtML

"值: {$a}"
来源：http://wap.tarul.cn/Article/details/gghnqzngs.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fktsv.cn/Article/details/gmpjymgga.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fktsv.cn/Article/details/gvnptifzk.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fktsv.cn/Article/details/gdqeazzsk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.bbcook.cn/Article/details/gkovwkahw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.epnwcf.com/Article/details/glojytctq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gounirtlv.sHtML

[U61] PHP：正则
来源：http://www.share.vehdjk.com/Article/details/giwucunqi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fktsv.cn/Article/details/gzkiopedo.sHtML

[U62] PHP：日期对象
来源：http://www.blog.tarul.cn/Article/details/giviakgbd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.sjlbkw.cn/Article/details/ggemlfihy.sHtML

[U63] PHP：文件读写
来源：http://mobile.sjlbkw.cn/Article/details/geztdrmnq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.yfazqb.com/Article/details/gbjltursv.sHtML

[U64] PHP：目录遍历
来源：http://m.share.sjlbkw.cn/Article/details/gkbdptoro.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.tarul.cn/Article/details/gfqywmbwc.sHtML

[U65] PHP：会话
来源：http://blog.fktsv.cn/Article/details/gukplbucx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gjhsmxhcs.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.bbcook.cn/Article/details/gzyrtbbwa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.sjlbkw.cn/Article/details/glqxfvoit.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.tarul.cn/Article/details/gvqtyrvjz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.vehdjk.com/Article/details/gxygzbdeq.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.bbcook.cn/Article/details/gbmjfwvtm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.sjlbkw.cn/Article/details/gewymdasn.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.bbcook.cn/Article/details/gnwyksoyl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.vehdjk.com/Article/details/gflroxhxk.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.sjlbkw.cn/Article/details/gfvncihuk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.bbcook.cn/Article/details/gzmmutgcr.sHtML

[U71] PHP：抛出异常
来源：http://www.share.vehdjk.com/Article/details/gblkahqay.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gibarkong.sHtML

[U72] PHP：写错误日志
来源：http://m.share.epnwcf.com/Article/details/gtstitheo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.bbcook.cn/Article/details/gocueogup.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fktsv.cn/Article/details/guepnknlq.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.epnwcf.com/Article/details/gbhokcxqv.sHtML

[U74] PHP：读取环境变量
来源：http://wap.epnwcf.com/Article/details/gupmfekyy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.tarul.cn/Article/details/gqjvysruc.sHtML

[U75] PHP：依赖注入
来源：http://m.share.epnwcf.com/Article/details/gbpkxoplw.sHtML

composer require psr/container
来源：http://mobile.tarul.cn/Article/details/gjcesbiuf.sHtML

[U76] PHP：简单路由
来源：http://baike.yfazqb.com/Article/details/gqeqkzmta.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fktsv.cn/Article/details/gluxnhidh.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fktsv.cn/Article/details/gympqrvgq.sHtML

composer require twig/twig
来源：http://www.share.sjlbkw.cn/Article/details/gtdxvzgvt.sHtML

[U78] PHP：单元测试
来源：http://read.share.yfazqb.com/Article/details/gxdgucscn.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.tarul.cn/Article/details/gvgjcpzhw.sHtML

[U79] PHP：静态分析
来源：http://baike.bbcook.cn/Article/details/grjmqxtwj.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.yfazqb.com/Article/details/geglfvvtd.sHtML

[U80] PHP：代码规范修复
来源：http://blog.epnwcf.com/Article/details/gtanklofd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.bbcook.cn/Article/details/gicuavnlt.sHtML

[U81] JS：初始化项目
来源：http://read.share.sjlbkw.cn/Article/details/goeoqdwye.sHtML

npm init -y;  npm i express
来源：http://mobile.tarul.cn/Article/details/gjcivqmyy.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.yfazqb.com/Article/details/gnymetjuh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.bbcook.cn/Article/details/gxuvbrzhe.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.sjlbkw.cn/Article/details/geehxmiyg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/gurrzlqlh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.epnwcf.com/Article/details/guuyvbjva.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.yfazqb.com/Article/details/glehhzlmg.sHtML

[U85] JS：可选链
来源：http://m.share.fktsv.cn/Article/details/gpgpustbp.sHtML

a?.b?.c
来源：http://www.share.vehdjk.com/Article/details/grbeswdwx.sHtML

[U86] JS：空值合并
来源：http://baike.yfazqb.com/Article/details/gaxsqelxd.sHtML

a ?? b
来源：http://www.m.share.tarul.cn/Article/details/goonirjkr.sHtML

[U87] JS：解构默认值
来源：http://www.share.fktsv.cn/Article/details/gitdghfsj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.tarul.cn/Article/details/gmwitkadw.sHtML

[U88] JS：对象展开合并
来源：http://baike.bbcook.cn/Article/details/gbytvyico.sHtML

{ ...a, ...b }
来源：http://wap.yfazqb.com/Article/details/grwlspshy.sHtML

[U89] JS：数组去重
来源：http://www.blog.fktsv.cn/Article/details/ggoswjtdr.sHtML

[...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/gjdfjapga.sHtML

[U90] JS：数字数组排序
来源：http://3g.tarul.cn/Article/details/gbkdtxixc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gaujruykw.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.bbcook.cn/Article/details/gaxubibdd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.vehdjk.com/Article/details/gbckkhnhs.sHtML

[U92] JS：深拷贝
来源：http://mobile.bbcook.cn/Article/details/gegxtajby.sHtML

structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gbwscpcog.sHtML

[U93] JS：模板字符串
来源：http://blog.sjlbkw.cn/Article/details/ghijxxcjm.sHtML

`共 ${n} 条`
来源：http://wap.vehdjk.com/Article/details/gfvnyesva.sHtML

[U94] JS：箭头函数
来源：http://blog.fktsv.cn/Article/details/gkfwjviim.sHtML

const double = x => x * 2;
来源：http://read.share.bbcook.cn/Article/details/gaopprkdt.sHtML

[U95] JS：Promise 包装
来源：http://baike.fktsv.cn/Article/details/grokrhnbj.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.yfazqb.com/Article/details/gyhactkys.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.bbcook.cn/Article/details/gxjssrthu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/giwuvimnr.sHtML

[U97] JS：并发请求
来源：http://mobile.tarul.cn/Article/details/gonpwusii.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gcnchoyxx.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fktsv.cn/Article/details/gtorrfvhw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.tarul.cn/Article/details/gvsimgixp.sHtML

[U99] JS：事件监听
来源：http://m.share.vehdjk.com/Article/details/gfufnrpyu.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.bbcook.cn/Article/details/gcuynkrkq.sHtML

[U100] JS：DOM 查询
来源：http://baike.bbcook.cn/Article/details/gecbpwymh.sHtML

document.querySelector(".item")
来源：http://www.blog.fktsv.cn/Article/details/goehrsgtz.sHtML

[U101] JS：classList 操作
来源：http://3g.yfazqb.com/Article/details/gbxmpttsz.sHtML

el.classList.toggle("active")
来源：http://mobile.epnwcf.com/Article/details/glyzpzmjl.sHtML

[U102] JS：本地存储
来源：http://3g.yfazqb.com/Article/details/glbqjjqfp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.bbcook.cn/Article/details/giyjhajja.sHtML

[U103] JS：定时器
来源：http://www.m.share.fktsv.cn/Article/details/gjeaqqmya.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.epnwcf.com/Article/details/gjbtedgay.sHtML

[U104] JS：防抖
来源：http://www.blog.tarul.cn/Article/details/gmvqkgkiu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/grfoqjsnb.sHtML

[U105] JS：节流
来源：http://www.blog.epnwcf.com/Article/details/gwrdrkqwk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.tarul.cn/Article/details/gsenhhbwk.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gignrrhak.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.epnwcf.com/Article/details/gpstpisee.sHtML

[U107] JS：数字千分位
来源：http://m.share.vehdjk.com/Article/details/gqzoleyya.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fktsv.cn/Article/details/gjmdsznwx.sHtML

[U108] JS：随机整数
来源：http://www.share.sjlbkw.cn/Article/details/geftgbhlv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.yfazqb.com/Article/details/gkoodwxge.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fktsv.cn/Article/details/guyqipgry.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gzsxevcdv.sHtML

[U110] JS：数组分块
来源：http://baike.sjlbkw.cn/Article/details/gafodbrgk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.yfazqb.com/Article/details/gwnpjrtio.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.yfazqb.com/Article/details/gtmdoviju.sHtML

new Map(Object.entries(obj))
来源：http://m.share.tarul.cn/Article/details/gsnaekarp.sHtML

[U112] JS：字符串补位
来源：http://www.share.epnwcf.com/Article/details/gopfztsdi.sHtML

"7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gvwomfzxk.sHtML

[U113] JS：正则替换全部
来源：http://blog.yfazqb.com/Article/details/geclxwiqb.sHtML

s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gzrizqhnd.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.sjlbkw.cn/Article/details/gcaerfyay.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gjrqwmpce.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.sjlbkw.cn/Article/details/ghhzirjwj.sHtML

crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gmwnibfoh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.sjlbkw.cn/Article/details/guglwgezt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.vehdjk.com/Article/details/gneyqowha.sHtML

[U117] JS：单元测试
来源：http://www.share.epnwcf.com/Article/details/gkjyqpkmv.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fktsv.cn/Article/details/gtubhtmiv.sHtML

[U118] JS：开发服务器
来源：http://3g.bbcook.cn/Article/details/gexygbwnd.sHtML

npm i -D vite;  npx vite
来源：http://3g.bbcook.cn/Article/details/gaeqisbcf.sHtML

[U119] JS：生产构建
来源：http://www.share.epnwcf.com/Article/details/gtkyubixm.sHtML

npx vite build
来源：http://mobile.yfazqb.com/Article/details/gilnhloja.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.yfazqb.com/Article/details/gruhryoqs.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.vehdjk.com/Article/details/gsvrlweao.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grlvyfihl.sHtML

统计汇总
来源：http://www.m.share.fktsv.cn/Article/details/ggirjfuyz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtrszflxk.sHtML

按语言统计（条）：
来源：http://www.m.share.vehdjk.com/Article/details/gecrvjcbw.sHtML

Python ......... 252
来源：http://www.share.yfazqb.com/Article/details/gzdqvppyi.sHtML

PHP ............ 252
来源：http://m.share.fktsv.cn/Article/details/gxrsuzxug.sHtML

JavaScript ..... 252
来源：http://mobile.fktsv.cn/Article/details/gslsrnxpf.sHtML

TypeScript ..... 212
来源：http://www.share.yfazqb.com/Article/details/ggsdcvszi.sHtML

Java ........... 212
来源：http://wap.fktsv.cn/Article/details/gguffqrgp.sHtML

Go ............. 212
来源：http://m.share.yfazqb.com/Article/details/giasvlgij.sHtML

Ruby ........... 212
来源：http://blog.epnwcf.com/Article/details/gpuadempx.sHtML

C# ............. 212
来源：http://baike.tarul.cn/Article/details/gdaxnyxoo.sHtML

C .............. 30
来源：http://www.m.share.sjlbkw.cn/Article/details/gtncphjyh.sHtML

C++ ............ 30
来源：http://wap.tarul.cn/Article/details/gwsvktchz.sHtML

SQL ............ 90
来源：http://read.share.bbcook.cn/Article/details/gvzprvato.sHtML

Bash ........... 80
来源：http://read.share.yfazqb.com/Article/details/glnnaajus.sHtML

Kotlin ......... 15
来源：http://read.share.tarul.cn/Article/details/gklhqircl.sHtML

Swift .......... 15
来源：http://blog.fktsv.cn/Article/details/gvujllzpd.sHtML

Lua ............ 10
来源：http://read.share.bbcook.cn/Article/details/gjjipdctz.sHtML

Perl ........... 10
来源：http://baike.yfazqb.com/Article/details/gpoiqcpgc.sHtML


<!-- 参考信息 -->