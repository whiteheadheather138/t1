代发 wailian999

[T45] Perl：数组遍历
来源：http://www.share.fktsv.cn/Article/details/giqmnmrix.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.epnwcf.com/Article/details/gsvuqdrtc.sHtML

[T46] Perl：哈希操作
来源：http://wap.fktsv.cn/Article/details/gkfojtyjn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fktsv.cn/Article/details/gvzvkogmi.sHtML

[T47] Perl：正则捕获
来源：http://mobile.tarul.cn/Article/details/gpdyhhepp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.vehdjk.com/Article/details/gxdwicjje.sHtML

[T48] Perl：正则替换
来源：http://m.share.sjlbkw.cn/Article/details/gkdhcgaqo.sHtML

$s =~ s/old/new/g;
来源：http://www.share.tarul.cn/Article/details/gxpafwzow.sHtML

[T49] Perl：函数
来源：http://mobile.yfazqb.com/Article/details/gbwedqjhc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gvganpyqq.sHtML

[T50] Perl：逐行读文件
来源：http://wap.bbcook.cn/Article/details/ggjngnicu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.bbcook.cn/Article/details/gytzwmkbj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.tarul.cn/Article/details/gppwfmsxy.sHtML

[T51] Scala：Hello World
来源：http://m.share.bbcook.cn/Article/details/gbicrohrq.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gybjknmes.sHtML

[T52] Scala：变量
来源：http://wap.sjlbkw.cn/Article/details/glsmngyyp.sHtML

val a = 1;  var b = 2
来源：http://read.share.epnwcf.com/Article/details/gmxvdxnwm.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gassjugkk.sHtML

s"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gpevwdrjr.sHtML

[T54] Scala：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gnotimqzq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fktsv.cn/Article/details/gmczqzlez.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.yfazqb.com/Article/details/gsqrnhlyj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.yfazqb.com/Article/details/gvzepzoji.sHtML

[T56] Scala：样例类
来源：http://3g.bbcook.cn/Article/details/gpaotgkwv.sHtML

case class User(name: String, age: Int)
来源：http://read.share.tarul.cn/Article/details/gdtqpcpge.sHtML

[T57] Scala：模式匹配
来源：http://read.share.bbcook.cn/Article/details/gdhxmhysu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.epnwcf.com/Article/details/gppkxybol.sHtML

[T58] Scala：函数定义
来源：http://read.share.sjlbkw.cn/Article/details/gvjnxmamw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.epnwcf.com/Article/details/ghusfnvre.sHtML

[T59] Scala：循环
来源：http://read.share.fktsv.cn/Article/details/glrbrikfk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gjvpuxdyo.sHtML

[T60] Scala：折叠
来源：http://m.share.yfazqb.com/Article/details/gzqiaccca.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.vehdjk.com/Article/details/ggpztfnxk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbnijlkdc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fktsv.cn/Article/details/gldkisblo.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbfrfttqv.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.yfazqb.com/Article/details/glvhzgdrd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fktsv.cn/Article/details/gciqvsjwv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/gadufepnb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.yfazqb.com/Article/details/gskwvjole.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.vehdjk.com/Article/details/gzsphhrfh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.bbcook.cn/Article/details/gfjfstreq.sHtML

[U04] Py：变量调试打印
来源：http://3g.vehdjk.com/Article/details/gdoknneei.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.tarul.cn/Article/details/gvsykhibu.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.bbcook.cn/Article/details/gxwjjgrbt.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fktsv.cn/Article/details/glprzqnzx.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fktsv.cn/Article/details/gwlzwlall.sHtML

{**a, **b}
来源：http://www.share.tarul.cn/Article/details/gkaafqpsc.sHtML

[U07] Py：反转字典键值
来源：http://baike.tarul.cn/Article/details/gwmndrayr.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.sjlbkw.cn/Article/details/gbiaslzmg.sHtML

[U08] Py：展平二维列表
来源：http://www.share.bbcook.cn/Article/details/gsbzcybhx.sHtML

[y for x in nested for y in x]
来源：http://blog.epnwcf.com/Article/details/gfhltaagb.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.bbcook.cn/Article/details/gfttvmvss.sHtML

max(d, key=d.get)
来源：http://www.blog.fktsv.cn/Article/details/gynwilxjh.sHtML

[U10] Py：按值排序字典
来源：http://wap.vehdjk.com/Article/details/ghjvikyxh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.tarul.cn/Article/details/gamucaitq.sHtML

[U11] Py：生成器表达式
来源：http://m.share.tarul.cn/Article/details/grooilrje.sHtML

(x * 2 for x in arr)
来源：http://wap.epnwcf.com/Article/details/gflcljhfs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.vehdjk.com/Article/details/gawsyzanz.sHtML

Counter(arr).most_common(3)
来源：http://www.share.tarul.cn/Article/details/glmwlgkxk.sHtML

[U13] Py：固定长度队列
来源：http://3g.sjlbkw.cn/Article/details/gyjvklrnn.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/gwkbopdxc.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.vehdjk.com/Article/details/glenxoiud.sHtML

defaultdict(list)
来源：http://www.blog.vehdjk.com/Article/details/gkwwvqbix.sHtML

[U15] Py：高精度计时
来源：http://read.share.bbcook.cn/Article/details/guflylure.sHtML

t = time.perf_counter()
来源：http://baike.bbcook.cn/Article/details/gdniqstph.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.sjlbkw.cn/Article/details/gmudhxnkl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.sjlbkw.cn/Article/details/gkbypowsb.sHtML

[U17] Py：初始化日志
来源：http://3g.bbcook.cn/Article/details/gwnyyyjre.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.yfazqb.com/Article/details/gcshbxsfm.sHtML

[U18] Py：预编译正则
来源：http://www.blog.bbcook.cn/Article/details/gpxednyth.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.sjlbkw.cn/Article/details/giblasimg.sHtML

[U19] Py：正则替换带回调
来源：http://3g.vehdjk.com/Article/details/gpngetrjq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.vehdjk.com/Article/details/gnamxrfdw.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.epnwcf.com/Article/details/gymjkzrqi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.epnwcf.com/Article/details/gwqdwtdjj.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fktsv.cn/Article/details/gxyhisnvd.sHtML

@contextlib.contextmanager
来源：http://wap.bbcook.cn/Article/details/ggeohlyjy.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fktsv.cn/Article/details/gakaydiqr.sHtML

list(zip(*m))
来源：http://www.share.tarul.cn/Article/details/gfqxpabgs.sHtML

[U23] Py：分块读取大文件
来源：http://wap.yfazqb.com/Article/details/gqwjysgzy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fktsv.cn/Article/details/gddavssmd.sHtML

[U24] Py：路径操作
来源：http://m.share.epnwcf.com/Article/details/gycgdofdc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/gclnoinkk.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.bbcook.cn/Article/details/gpvqxpzqd.sHtML

csv.DictReader(f)
来源：http://baike.bbcook.cn/Article/details/gqwzdzkxs.sHtML

[U26] Py：并发下载
来源：http://baike.yfazqb.com/Article/details/gmeqindwm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.yfazqb.com/Article/details/ghbpmumns.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.tarul.cn/Article/details/gtawzvjcf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.sjlbkw.cn/Article/details/gwtwbsmcp.sHtML

[U28] Py：类型别名
来源：http://3g.yfazqb.com/Article/details/ggmtxknsb.sHtML

UserId = int
来源：http://mobile.epnwcf.com/Article/details/gzntsxkao.sHtML

[U29] Py：属性校验
来源：http://3g.sjlbkw.cn/Article/details/gmqprzyyw.sHtML

@property 与 @x.setter 配合
来源：http://www.share.bbcook.cn/Article/details/gduxaskyd.sHtML

[U30] Py：数据类
来源：http://www.blog.vehdjk.com/Article/details/gxvtkrmua.sHtML

@dataclass(slots=True)
来源：http://blog.bbcook.cn/Article/details/gfzygtjli.sHtML

[U31] Py：单测
来源：http://3g.fktsv.cn/Article/details/gwqjmchhu.sHtML

python -m pytest -q
来源：http://wap.vehdjk.com/Article/details/gdnejssdp.sHtML

[U32] Py：代码格式化
来源：http://mobile.vehdjk.com/Article/details/gefokkpye.sHtML

ruff format . && ruff check --fix .
来源：http://blog.vehdjk.com/Article/details/gocjvqnyc.sHtML

[U33] Py：打包发布
来源：http://www.share.yfazqb.com/Article/details/gkaalwdje.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fktsv.cn/Article/details/gkdzcodhk.sHtML

[U34] Py：判断编码
来源：http://read.share.vehdjk.com/Article/details/gyolttahp.sHtML

chardet.detect(raw)
来源：http://3g.fktsv.cn/Article/details/gtbifnico.sHtML

[U35] Py：发送邮件
来源：http://baike.epnwcf.com/Article/details/gxlvdwjkg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.tarul.cn/Article/details/grkahbpgd.sHtML

[U36] Py：定时任务
来源：http://read.share.sjlbkw.cn/Article/details/gvaeddctu.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.bbcook.cn/Article/details/gahlxcvmm.sHtML

[U37] Py：读写 Excel
来源：http://mobile.yfazqb.com/Article/details/gixjspezt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fktsv.cn/Article/details/gtshezewt.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fktsv.cn/Article/details/gomccshig.sHtML

Path(__file__).resolve().parent
来源：http://read.share.vehdjk.com/Article/details/grcdskfvo.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.sjlbkw.cn/Article/details/gzamwldge.sHtML

sys.stdout.isatty()
来源：http://wap.yfazqb.com/Article/details/gmsyeceek.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.vehdjk.com/Article/details/ghpitogkd.sHtML

print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gtvtneqjf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fktsv.cn/Article/details/goowhioem.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.epnwcf.com/Article/details/geamchatw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.tarul.cn/Article/details/gjbmrgmdr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.yfazqb.com/Article/details/gqnzbhivz.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fktsv.cn/Article/details/guypzzzbk.sHtML

namespace App\Http;
来源：http://www.m.share.bbcook.cn/Article/details/giwcqmnlp.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.vehdjk.com/Article/details/gequlddcj.sHtML

declare(strict_types=1);
来源：http://read.share.yfazqb.com/Article/details/geihtisyg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.yfazqb.com/Article/details/ggiomxrix.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gfqhmmico.sHtML

[U46] PHP：可空类型
来源：http://blog.vehdjk.com/Article/details/gebugufom.sHtML

?string $name = null
来源：http://wap.fktsv.cn/Article/details/ggcuutfuq.sHtML

[U47] PHP：联合类型
来源：http://wap.bbcook.cn/Article/details/gknpxtwqn.sHtML

int|string $id
来源：http://read.share.epnwcf.com/Article/details/grkbdgwjx.sHtML

[U48] PHP：纯枚举
来源：http://read.share.bbcook.cn/Article/details/gtygaiidw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.vehdjk.com/Article/details/ggvtojwsh.sHtML

[U49] PHP：只读属性
来源：http://m.share.vehdjk.com/Article/details/ggnvnlell.sHtML

public readonly string $name
来源：http://baike.vehdjk.com/Article/details/gdbgwwidc.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.epnwcf.com/Article/details/gbqpduugw.sHtML

public function __construct(private int $id) {}
来源：http://baike.epnwcf.com/Article/details/gpbvvvbme.sHtML

[U51] PHP：数组解构
来源：http://m.share.yfazqb.com/Article/details/giwscgjti.sHtML

[$a, $b] = $arr;
来源：http://read.share.bbcook.cn/Article/details/glptmjlbj.sHtML

[U52] PHP：箭头函数
来源：http://mobile.vehdjk.com/Article/details/gxsvvlpob.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.epnwcf.com/Article/details/gixbgzwhd.sHtML

[U53] PHP：空合并运算符
来源：http://3g.yfazqb.com/Article/details/gfxmietfa.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fktsv.cn/Article/details/gyhlpdlrr.sHtML

[U54] PHP：空安全调用
来源：http://baike.yfazqb.com/Article/details/ghrwqwyqh.sHtML

$obj?->method()
来源：http://www.share.sjlbkw.cn/Article/details/gsrxydutd.sHtML

[U55] PHP：match 表达式
来源：http://wap.vehdjk.com/Article/details/glcyfisdc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fktsv.cn/Article/details/gtwhnsimc.sHtML

[U56] PHP：命名参数
来源：http://blog.sjlbkw.cn/Article/details/ghafeshad.sHtML

f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gcwrdewhd.sHtML

[U57] PHP：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gxtgykbui.sHtML

"值: {$a}"
来源：http://baike.vehdjk.com/Article/details/gfdomjswo.sHtML

[U58] PHP：数组三件套
来源：http://m.share.tarul.cn/Article/details/gokroskrf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.tarul.cn/Article/details/golfezmxj.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fktsv.cn/Article/details/gxuobfvbo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gbzhgawaq.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.epnwcf.com/Article/details/gxeufyvyr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fktsv.cn/Article/details/gbtxljwuj.sHtML

[U61] PHP：正则
来源：http://mobile.yfazqb.com/Article/details/gtfysmmun.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/gbiywtacm.sHtML

[U62] PHP：日期对象
来源：http://mobile.yfazqb.com/Article/details/gamjtyrlo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.sjlbkw.cn/Article/details/gkalroyeg.sHtML

[U63] PHP：文件读写
来源：http://wap.tarul.cn/Article/details/gvrwhdbuj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.bbcook.cn/Article/details/gijdxqcwb.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.bbcook.cn/Article/details/gxpupcqfg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.tarul.cn/Article/details/ghkuxtyip.sHtML

[U65] PHP：会话
来源：http://baike.vehdjk.com/Article/details/giprgtwnm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gdzmhvvda.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.yfazqb.com/Article/details/gixucruhy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.tarul.cn/Article/details/gprxnaifs.sHtML

[U67] PHP：处理文件上传
来源：http://3g.sjlbkw.cn/Article/details/gfoigiixz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.sjlbkw.cn/Article/details/ghkijnyci.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.yfazqb.com/Article/details/gezhrcpkt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.sjlbkw.cn/Article/details/gahhnreld.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.vehdjk.com/Article/details/ggcvjplgf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.sjlbkw.cn/Article/details/gigppvmhu.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.vehdjk.com/Article/details/gpwaauqtp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.yfazqb.com/Article/details/gpbvzkiyd.sHtML

[U71] PHP：抛出异常
来源：http://mobile.yfazqb.com/Article/details/gxgsekxad.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.yfazqb.com/Article/details/gjhbwfnxo.sHtML

[U72] PHP：写错误日志
来源：http://3g.yfazqb.com/Article/details/getdeavlg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.sjlbkw.cn/Article/details/gfuxjbfwo.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.bbcook.cn/Article/details/gezpwqaak.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.bbcook.cn/Article/details/gukatxuid.sHtML

[U74] PHP：读取环境变量
来源：http://3g.yfazqb.com/Article/details/gzxdsbzsc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.vehdjk.com/Article/details/gmmknqrly.sHtML

[U75] PHP：依赖注入
来源：http://www.share.sjlbkw.cn/Article/details/gagwuxige.sHtML

composer require psr/container
来源：http://read.share.sjlbkw.cn/Article/details/gpgezotas.sHtML

[U76] PHP：简单路由
来源：http://wap.vehdjk.com/Article/details/gswxnjdvk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.tarul.cn/Article/details/gbywijwoj.sHtML

[U77] PHP：模板渲染
来源：http://read.share.vehdjk.com/Article/details/gjtcpyanv.sHtML

composer require twig/twig
来源：http://3g.epnwcf.com/Article/details/gwnziisui.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gknybwwxl.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.yfazqb.com/Article/details/gzktucrcb.sHtML

[U79] PHP：静态分析
来源：http://baike.bbcook.cn/Article/details/gvpwpucfo.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.bbcook.cn/Article/details/gmelbwblp.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.yfazqb.com/Article/details/gdyohgtdi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fktsv.cn/Article/details/guadtlhuu.sHtML

[U81] JS：初始化项目
来源：http://www.share.tarul.cn/Article/details/gwoxdjest.sHtML

npm init -y;  npm i express
来源：http://read.share.tarul.cn/Article/details/gqqattxdv.sHtML

[U82] JS：package.json 脚本
来源：http://baike.tarul.cn/Article/details/guivqfvkr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.tarul.cn/Article/details/gsocgdyam.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.vehdjk.com/Article/details/gxryludsz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/gxezrdllu.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.yfazqb.com/Article/details/gjdcubyxk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fktsv.cn/Article/details/grhqapgae.sHtML

[U85] JS：可选链
来源：http://www.share.sjlbkw.cn/Article/details/grneikesb.sHtML

a?.b?.c
来源：http://read.share.bbcook.cn/Article/details/gwwqfuqxl.sHtML

[U86] JS：空值合并
来源：http://blog.sjlbkw.cn/Article/details/glhommsrn.sHtML

a ?? b
来源：http://mobile.bbcook.cn/Article/details/gtnkhggjb.sHtML

[U87] JS：解构默认值
来源：http://www.blog.tarul.cn/Article/details/gwcktadxd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.sjlbkw.cn/Article/details/gqexmsmic.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fktsv.cn/Article/details/glxrcngpa.sHtML

{ ...a, ...b }
来源：http://m.share.epnwcf.com/Article/details/giwcbxohi.sHtML

[U89] JS：数组去重
来源：http://blog.yfazqb.com/Article/details/gnwkribfv.sHtML

[...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/gdkqpfxut.sHtML

[U90] JS：数字数组排序
来源：http://m.share.bbcook.cn/Article/details/gxhqzhvvw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/guyhbykmu.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.yfazqb.com/Article/details/gyzygvmls.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.sjlbkw.cn/Article/details/glmrqapya.sHtML

[U92] JS：深拷贝
来源：http://www.share.yfazqb.com/Article/details/gqilmcnqb.sHtML

structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gfotyeuom.sHtML

[U93] JS：模板字符串
来源：http://m.share.sjlbkw.cn/Article/details/gofuyxocd.sHtML

`共 ${n} 条`
来源：http://blog.epnwcf.com/Article/details/gnysjreuk.sHtML

[U94] JS：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gwxugvpni.sHtML

const double = x => x * 2;
来源：http://read.share.fktsv.cn/Article/details/gkrvtiouh.sHtML

[U95] JS：Promise 包装
来源：http://read.share.tarul.cn/Article/details/gpaspgmyo.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fktsv.cn/Article/details/gjpnfgmiz.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.bbcook.cn/Article/details/gxjgchkxb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gnyfagnqi.sHtML

[U97] JS：并发请求
来源：http://blog.yfazqb.com/Article/details/gfwzoptbs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gzabtmyhk.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.yfazqb.com/Article/details/ghdciytly.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.sjlbkw.cn/Article/details/grtxfmlhx.sHtML

[U99] JS：事件监听
来源：http://mobile.sjlbkw.cn/Article/details/ghqvhaenk.sHtML

el.addEventListener("click", e => {})
来源：http://wap.bbcook.cn/Article/details/gpktmzidx.sHtML

[U100] JS：DOM 查询
来源：http://blog.epnwcf.com/Article/details/gleftpynj.sHtML

document.querySelector(".item")
来源：http://3g.epnwcf.com/Article/details/gnnmcwzjm.sHtML

[U101] JS：classList 操作
来源：http://m.share.fktsv.cn/Article/details/gtzzryaut.sHtML

el.classList.toggle("active")
来源：http://3g.sjlbkw.cn/Article/details/gpdiuwpdq.sHtML

[U102] JS：本地存储
来源：http://mobile.yfazqb.com/Article/details/gwouwoema.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.vehdjk.com/Article/details/gluutlpve.sHtML

[U103] JS：定时器
来源：http://blog.vehdjk.com/Article/details/gtalcdxlf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.yfazqb.com/Article/details/geeevaocq.sHtML

[U104] JS：防抖
来源：http://mobile.vehdjk.com/Article/details/gztvbyhha.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gsnlwiocl.sHtML

[U105] JS：节流
来源：http://3g.vehdjk.com/Article/details/gdpsytvxz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.vehdjk.com/Article/details/ghgzujlyc.sHtML

[U106] JS：日期格式化
来源：http://www.share.epnwcf.com/Article/details/geoolimli.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.sjlbkw.cn/Article/details/gcrmfpdox.sHtML

[U107] JS：数字千分位
来源：http://blog.sjlbkw.cn/Article/details/givjdncod.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gtkrilhbn.sHtML

[U108] JS：随机整数
来源：http://read.share.sjlbkw.cn/Article/details/granoxydi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.tarul.cn/Article/details/gzqykpcok.sHtML

[U109] JS：数组分组
来源：http://read.share.epnwcf.com/Article/details/gfwodrars.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/gwscoerbq.sHtML

[U110] JS：数组分块
来源：http://m.share.vehdjk.com/Article/details/gyzsbcqdw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.tarul.cn/Article/details/glloxdcii.sHtML

[U111] JS：对象转 Map
来源：http://mobile.vehdjk.com/Article/details/gkdgtxwbw.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fktsv.cn/Article/details/gevvsbhoc.sHtML

[U112] JS：字符串补位
来源：http://baike.fktsv.cn/Article/details/gdfyzaopj.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gpfbmnlnr.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.yfazqb.com/Article/details/gnyesqtms.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfmxqkhp.sHtML

[U114] JS：JSON 深比较
来源：http://baike.yfazqb.com/Article/details/gmpjwrund.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fktsv.cn/Article/details/gdtxslnkb.sHtML

[U115] JS：生成 UUID
来源：http://read.share.yfazqb.com/Article/details/glfyqzbde.sHtML

crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gjznqfzfk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.sjlbkw.cn/Article/details/ggdraseap.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fktsv.cn/Article/details/ggwrtgfti.sHtML

[U117] JS：单元测试
来源：http://m.share.epnwcf.com/Article/details/gnvvupfsj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.epnwcf.com/Article/details/gbqepieqs.sHtML

[U118] JS：开发服务器
来源：http://read.share.yfazqb.com/Article/details/gxabwqmcu.sHtML

npm i -D vite;  npx vite
来源：http://mobile.bbcook.cn/Article/details/gecwlfkhp.sHtML

[U119] JS：生产构建
来源：http://www.share.yfazqb.com/Article/details/gjrghlzcm.sHtML

npx vite build
来源：http://www.blog.fktsv.cn/Article/details/ghhmzrdxy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.yfazqb.com/Article/details/gadwkovwt.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.yfazqb.com/Article/details/gimydodnq.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gbjanuxet.sHtML

统计汇总
来源：http://blog.tarul.cn/Article/details/gdlbkpbdv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnvkivpqg.sHtML

按语言统计（条）：
来源：http://3g.tarul.cn/Article/details/ghlgjcnem.sHtML

Python ......... 252
来源：http://baike.vehdjk.com/Article/details/gzofkbrsr.sHtML

PHP ............ 252
来源：http://www.share.bbcook.cn/Article/details/gnkyvgcah.sHtML

JavaScript ..... 252
来源：http://3g.fktsv.cn/Article/details/goqjnqgch.sHtML

TypeScript ..... 212
来源：http://m.share.tarul.cn/Article/details/gimvkimco.sHtML

Java ........... 212
来源：http://3g.vehdjk.com/Article/details/giakfiwuk.sHtML

Go ............. 212
来源：http://mobile.sjlbkw.cn/Article/details/gzmfbsaeu.sHtML

Ruby ........... 212
来源：http://www.m.share.tarul.cn/Article/details/gylrumgok.sHtML

C# ............. 212
来源：http://baike.epnwcf.com/Article/details/gzosfhtaa.sHtML

C .............. 30
来源：http://www.share.bbcook.cn/Article/details/gggnpmtps.sHtML

C++ ............ 30
来源：http://wap.sjlbkw.cn/Article/details/gkzknitta.sHtML

SQL ............ 90
来源：http://blog.yfazqb.com/Article/details/gmfegdnuh.sHtML

Bash ........... 80
来源：http://blog.yfazqb.com/Article/details/gfjpkruda.sHtML

Kotlin ......... 15
来源：http://3g.yfazqb.com/Article/details/gypbnmpih.sHtML

Swift .......... 15
来源：http://www.blog.tarul.cn/Article/details/gkerlstfa.sHtML

Lua ............ 10
来源：http://3g.bbcook.cn/Article/details/gznbzqlqz.sHtML

Perl ........... 10
来源：http://3g.bbcook.cn/Article/details/gmpqtvhkx.sHtML

Scala .......... 10
来源：http://3g.tarul.cn/Article/details/ghqqwaavl.sHtML

------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gstbfiizh.sHtML

合计 ........... 2106 条
来源：http://mobile.vehdjk.com/Article/details/ggwlzexew.sHtML

按章节统计：
来源：http://mobile.yfazqb.com/Article/details/gtcywwits.sHtML


<!-- 参考信息 -->