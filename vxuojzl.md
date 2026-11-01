代发 wailian999

[T45] Perl：数组遍历
来源：http://wap.vehdjk.com/Article/details/gkqhpxiyn.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fktsv.cn/Article/details/gpcvnkvfw.sHtML

[T46] Perl：哈希操作
来源：http://3g.bbcook.cn/Article/details/gyxvzfwgo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fktsv.cn/Article/details/gxoggkuic.sHtML

[T47] Perl：正则捕获
来源：http://wap.sjlbkw.cn/Article/details/grksjsqiz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.sjlbkw.cn/Article/details/ghbjedgga.sHtML

[T48] Perl：正则替换
来源：http://3g.sjlbkw.cn/Article/details/gwznaqyje.sHtML

$s =~ s/old/new/g;
来源：http://baike.vehdjk.com/Article/details/gviwgjmcy.sHtML

[T49] Perl：函数
来源：http://mobile.epnwcf.com/Article/details/gsjzqgmmh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gigqtfnij.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/geqmggktr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.tarul.cn/Article/details/gdwgpfhco.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fktsv.cn/Article/details/gyhgudshz.sHtML

[T51] Scala：Hello World
来源：http://3g.vehdjk.com/Article/details/gqnqcdfpa.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gsfzhsvqd.sHtML

[T52] Scala：变量
来源：http://mobile.fktsv.cn/Article/details/gphvvives.sHtML

val a = 1;  var b = 2
来源：http://3g.vehdjk.com/Article/details/gyqkebuuc.sHtML

[T53] Scala：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gtyriuwuq.sHtML

s"值: $b"
来源：http://blog.yfazqb.com/Article/details/glrqvslxp.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/gmhwwswai.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/grjsnutlq.sHtML

[T55] Scala：集合过滤
来源：http://wap.fktsv.cn/Article/details/gewfdtrtl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.sjlbkw.cn/Article/details/gbofwmbfb.sHtML

[T56] Scala：样例类
来源：http://wap.fktsv.cn/Article/details/gigcpjkvh.sHtML

case class User(name: String, age: Int)
来源：http://baike.fktsv.cn/Article/details/gzawjyvjr.sHtML

[T57] Scala：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/gxlwoonwm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.yfazqb.com/Article/details/gvihxajwv.sHtML

[T58] Scala：函数定义
来源：http://www.share.epnwcf.com/Article/details/glsvixagf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.yfazqb.com/Article/details/gidjokwek.sHtML

[T59] Scala：循环
来源：http://www.share.vehdjk.com/Article/details/gcfdtlauc.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fktsv.cn/Article/details/ggdiibepu.sHtML

[T60] Scala：折叠
来源：http://3g.vehdjk.com/Article/details/gbphxqyfc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fktsv.cn/Article/details/gtiwsgxaz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghjtkwzyj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gqwlwlbok.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvfvjuvkk.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.yfazqb.com/Article/details/gclaycklq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.epnwcf.com/Article/details/gjkztehwh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fktsv.cn/Article/details/gbsyuceqa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.tarul.cn/Article/details/gnocguwyc.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.bbcook.cn/Article/details/gjnpuvukx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fktsv.cn/Article/details/glszapalx.sHtML

[U04] Py：变量调试打印
来源：http://wap.bbcook.cn/Article/details/gvxupppgn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.vehdjk.com/Article/details/gfypkbrgh.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.tarul.cn/Article/details/gzcbnmoto.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gpfvdgmnv.sHtML

[U06] Py：合并两个字典
来源：http://baike.yfazqb.com/Article/details/gmyilqbya.sHtML

{**a, **b}
来源：http://m.share.bbcook.cn/Article/details/gqwlvzgdl.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fktsv.cn/Article/details/gozzgtufr.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fktsv.cn/Article/details/gyqjvmmlg.sHtML

[U08] Py：展平二维列表
来源：http://wap.bbcook.cn/Article/details/gmcbgjfty.sHtML

[y for x in nested for y in x]
来源：http://mobile.fktsv.cn/Article/details/gxulmydnb.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.sjlbkw.cn/Article/details/grsrphrjv.sHtML

max(d, key=d.get)
来源：http://read.share.yfazqb.com/Article/details/gitcsfbyz.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fktsv.cn/Article/details/gwvplqsss.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fktsv.cn/Article/details/grjglnscv.sHtML

[U11] Py：生成器表达式
来源：http://mobile.bbcook.cn/Article/details/glguduzcg.sHtML

(x * 2 for x in arr)
来源：http://read.share.epnwcf.com/Article/details/gnsdmlccu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/gqzzxanwq.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.epnwcf.com/Article/details/gzlujxkgv.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fktsv.cn/Article/details/gdpsbvoez.sHtML

deque(maxlen=10)
来源：http://3g.yfazqb.com/Article/details/gsxqkgeur.sHtML

[U14] Py：分组收集到列表
来源：http://3g.sjlbkw.cn/Article/details/gmkmptcip.sHtML

defaultdict(list)
来源：http://mobile.bbcook.cn/Article/details/gydpyikll.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.tarul.cn/Article/details/gfqcptiwz.sHtML

t = time.perf_counter()
来源：http://www.m.share.sjlbkw.cn/Article/details/grhqmxwgi.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.sjlbkw.cn/Article/details/gpiqctrcx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.tarul.cn/Article/details/gegxckknx.sHtML

[U17] Py：初始化日志
来源：http://blog.fktsv.cn/Article/details/guacclmbo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.yfazqb.com/Article/details/gxmkubbsy.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.bbcook.cn/Article/details/gzwnxpynj.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fktsv.cn/Article/details/gkdyanthp.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fktsv.cn/Article/details/gbphtpbkx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.bbcook.cn/Article/details/gwompzwul.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.tarul.cn/Article/details/gzceiswxe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.yfazqb.com/Article/details/gvsaihstx.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.sjlbkw.cn/Article/details/gprivprpx.sHtML

@contextlib.contextmanager
来源：http://read.share.sjlbkw.cn/Article/details/gpbmjudzs.sHtML

[U22] Py：矩阵转置
来源：http://www.share.yfazqb.com/Article/details/gsamrttvm.sHtML

list(zip(*m))
来源：http://blog.tarul.cn/Article/details/guciptyef.sHtML

[U23] Py：分块读取大文件
来源：http://baike.yfazqb.com/Article/details/giqceoytn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.tarul.cn/Article/details/gstavjyiz.sHtML

[U24] Py：路径操作
来源：http://m.share.bbcook.cn/Article/details/gjcjobrtj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gvmvotcjn.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.tarul.cn/Article/details/gjcgxeyld.sHtML

csv.DictReader(f)
来源：http://blog.fktsv.cn/Article/details/gelvnfwjc.sHtML

[U26] Py：并发下载
来源：http://3g.tarul.cn/Article/details/gembyziso.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.sjlbkw.cn/Article/details/ghffkuqcg.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.vehdjk.com/Article/details/ggrranzah.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.yfazqb.com/Article/details/gbvoeyazn.sHtML

[U28] Py：类型别名
来源：http://wap.epnwcf.com/Article/details/gcungswzx.sHtML

UserId = int
来源：http://mobile.vehdjk.com/Article/details/gejfuvvod.sHtML

[U29] Py：属性校验
来源：http://3g.epnwcf.com/Article/details/goxlwimxb.sHtML

@property 与 @x.setter 配合
来源：http://blog.epnwcf.com/Article/details/glmehusii.sHtML

[U30] Py：数据类
来源：http://www.m.share.yfazqb.com/Article/details/gvjbijwvf.sHtML

@dataclass(slots=True)
来源：http://baike.tarul.cn/Article/details/goirsgcdx.sHtML

[U31] Py：单测
来源：http://read.share.vehdjk.com/Article/details/gzvawvnlp.sHtML

python -m pytest -q
来源：http://wap.yfazqb.com/Article/details/gglyrywia.sHtML

[U32] Py：代码格式化
来源：http://www.blog.vehdjk.com/Article/details/gczaxmvjh.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.sjlbkw.cn/Article/details/gofedviuq.sHtML

[U33] Py：打包发布
来源：http://www.m.share.bbcook.cn/Article/details/gpkijwfbg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.epnwcf.com/Article/details/gobzbvyup.sHtML

[U34] Py：判断编码
来源：http://3g.sjlbkw.cn/Article/details/gjwgxbynd.sHtML

chardet.detect(raw)
来源：http://www.m.share.sjlbkw.cn/Article/details/giongqrmu.sHtML

[U35] Py：发送邮件
来源：http://www.share.tarul.cn/Article/details/gyagcjubr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.bbcook.cn/Article/details/gzmjyqjpb.sHtML

[U36] Py：定时任务
来源：http://blog.vehdjk.com/Article/details/gxyvijmqw.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.tarul.cn/Article/details/gdnhyfkmn.sHtML

[U37] Py：读写 Excel
来源：http://blog.tarul.cn/Article/details/glyimuqjp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.yfazqb.com/Article/details/gjgweceeq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fktsv.cn/Article/details/gjoyesysz.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fktsv.cn/Article/details/gzfstfgql.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.epnwcf.com/Article/details/gvyjuhsvk.sHtML

sys.stdout.isatty()
来源：http://3g.sjlbkw.cn/Article/details/gpqhqqglk.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.vehdjk.com/Article/details/gnltsgmom.sHtML

print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/gbkzufjhr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.tarul.cn/Article/details/geivjdlmi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/gekqfihir.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fktsv.cn/Article/details/gzdhqivyn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.sjlbkw.cn/Article/details/gllagtjvi.sHtML

[U43] PHP：声明命名空间
来源：http://blog.tarul.cn/Article/details/ghkdyijwo.sHtML

namespace App\Http;
来源：http://m.share.tarul.cn/Article/details/gjkvudqvt.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.sjlbkw.cn/Article/details/glohcneyh.sHtML

declare(strict_types=1);
来源：http://www.share.vehdjk.com/Article/details/gkicjtevq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.bbcook.cn/Article/details/gklzxzrjt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/ghcvaptfo.sHtML

[U46] PHP：可空类型
来源：http://wap.epnwcf.com/Article/details/gedvgvjga.sHtML

?string $name = null
来源：http://wap.yfazqb.com/Article/details/gplmctvlk.sHtML

[U47] PHP：联合类型
来源：http://m.share.sjlbkw.cn/Article/details/gudaiickp.sHtML

int|string $id
来源：http://baike.vehdjk.com/Article/details/gfetwyozq.sHtML

[U48] PHP：纯枚举
来源：http://mobile.bbcook.cn/Article/details/gzypmqzer.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grxppphfk.sHtML

[U49] PHP：只读属性
来源：http://baike.sjlbkw.cn/Article/details/gdcvjswel.sHtML

public readonly string $name
来源：http://www.share.epnwcf.com/Article/details/gtvvniglu.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.bbcook.cn/Article/details/ghngeedcd.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.yfazqb.com/Article/details/gwvipffhq.sHtML

[U51] PHP：数组解构
来源：http://www.share.epnwcf.com/Article/details/gfiwppcmm.sHtML

[$a, $b] = $arr;
来源：http://blog.sjlbkw.cn/Article/details/ggvelbuqd.sHtML

[U52] PHP：箭头函数
来源：http://mobile.yfazqb.com/Article/details/gcslcdmab.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.epnwcf.com/Article/details/gvkwejmys.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.tarul.cn/Article/details/gfrccbelm.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.yfazqb.com/Article/details/glwlbexso.sHtML

[U54] PHP：空安全调用
来源：http://www.share.bbcook.cn/Article/details/ggsqeojbp.sHtML

$obj?->method()
来源：http://3g.tarul.cn/Article/details/gtwhsmrod.sHtML

[U55] PHP：match 表达式
来源：http://wap.yfazqb.com/Article/details/gpofqdmno.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/gkitldnqk.sHtML

[U56] PHP：命名参数
来源：http://baike.vehdjk.com/Article/details/gjtqsqsoq.sHtML

f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gxzkvewwm.sHtML

[U57] PHP：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gogyukmai.sHtML

"值: {$a}"
来源：http://mobile.tarul.cn/Article/details/gplsjvrbi.sHtML

[U58] PHP：数组三件套
来源：http://baike.vehdjk.com/Article/details/gxdplznxo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gmxahneud.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.yfazqb.com/Article/details/gcdpnartw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.yfazqb.com/Article/details/gvrutqdmb.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.tarul.cn/Article/details/gyomvntax.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.tarul.cn/Article/details/ghbnzlwsw.sHtML

[U61] PHP：正则
来源：http://3g.sjlbkw.cn/Article/details/goitjylbo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/gqvsxssed.sHtML

[U62] PHP：日期对象
来源：http://read.share.yfazqb.com/Article/details/gcpgxdydb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.sjlbkw.cn/Article/details/gazfqvzlg.sHtML

[U63] PHP：文件读写
来源：http://m.share.epnwcf.com/Article/details/gxntvfzow.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.epnwcf.com/Article/details/ggodulimq.sHtML

[U64] PHP：目录遍历
来源：http://3g.sjlbkw.cn/Article/details/gyqkfwbjg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.vehdjk.com/Article/details/gmshdfgtu.sHtML

[U65] PHP：会话
来源：http://3g.fktsv.cn/Article/details/gdinnojyb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gflhfqtca.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fktsv.cn/Article/details/gcadsytmj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.tarul.cn/Article/details/gjaiwwwyq.sHtML

[U67] PHP：处理文件上传
来源：http://blog.epnwcf.com/Article/details/gijiskqag.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.yfazqb.com/Article/details/gbwdukdog.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.tarul.cn/Article/details/gfptfzstq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.bbcook.cn/Article/details/ghqdrtzfb.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.bbcook.cn/Article/details/gtjhpdpre.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.sjlbkw.cn/Article/details/gnrmeudyb.sHtML

[U70] PHP：PDO 事务
来源：http://baike.vehdjk.com/Article/details/gvnqhrvvs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.bbcook.cn/Article/details/gaqkovxrm.sHtML

[U71] PHP：抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/goxrnwycs.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.bbcook.cn/Article/details/gnaqudktm.sHtML

[U72] PHP：写错误日志
来源：http://mobile.epnwcf.com/Article/details/gpcpqcscb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fktsv.cn/Article/details/ghfftxflv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.yfazqb.com/Article/details/gnuqbnmtb.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fktsv.cn/Article/details/grokmibcu.sHtML

[U74] PHP：读取环境变量
来源：http://baike.yfazqb.com/Article/details/gajgbcqra.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.bbcook.cn/Article/details/gmchyqmxc.sHtML

[U75] PHP：依赖注入
来源：http://3g.epnwcf.com/Article/details/geqxqmtvk.sHtML

composer require psr/container
来源：http://read.share.fktsv.cn/Article/details/ghxscjbnr.sHtML

[U76] PHP：简单路由
来源：http://mobile.fktsv.cn/Article/details/gxxaxmdga.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.sjlbkw.cn/Article/details/gnojlmzte.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fktsv.cn/Article/details/grrgozqwx.sHtML

composer require twig/twig
来源：http://mobile.yfazqb.com/Article/details/gnntiaccu.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.bbcook.cn/Article/details/glvskepfn.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.vehdjk.com/Article/details/gpqaxlqmj.sHtML

[U79] PHP：静态分析
来源：http://m.share.fktsv.cn/Article/details/gwtzoxegg.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.vehdjk.com/Article/details/gfbwexxyj.sHtML

[U80] PHP：代码规范修复
来源：http://wap.vehdjk.com/Article/details/gudfaayzd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.tarul.cn/Article/details/gfzgidyvc.sHtML

[U81] JS：初始化项目
来源：http://blog.epnwcf.com/Article/details/gkvxdczuc.sHtML

npm init -y;  npm i express
来源：http://3g.fktsv.cn/Article/details/gklajngnu.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fktsv.cn/Article/details/gbbsdodsp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.sjlbkw.cn/Article/details/gblizaloo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.sjlbkw.cn/Article/details/ggverxamq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gfctojlxw.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.bbcook.cn/Article/details/gkywvkftr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.bbcook.cn/Article/details/gskeyaoyl.sHtML

[U85] JS：可选链
来源：http://3g.epnwcf.com/Article/details/gtqpujdtu.sHtML

a?.b?.c
来源：http://m.share.fktsv.cn/Article/details/gsjctjdxf.sHtML

[U86] JS：空值合并
来源：http://m.share.yfazqb.com/Article/details/gtlxlcvak.sHtML

a ?? b
来源：http://wap.sjlbkw.cn/Article/details/gpzkwzhhl.sHtML

[U87] JS：解构默认值
来源：http://www.share.fktsv.cn/Article/details/gznqnqvut.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.vehdjk.com/Article/details/gyowuusdn.sHtML

[U88] JS：对象展开合并
来源：http://blog.bbcook.cn/Article/details/glidctqqf.sHtML

{ ...a, ...b }
来源：http://baike.fktsv.cn/Article/details/gynimgbrs.sHtML

[U89] JS：数组去重
来源：http://mobile.tarul.cn/Article/details/ghiyyczhd.sHtML

[...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gexlslszs.sHtML

[U90] JS：数字数组排序
来源：http://www.share.sjlbkw.cn/Article/details/gwxbjcjlx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gytmpkwpu.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.bbcook.cn/Article/details/gzjfeawee.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.vehdjk.com/Article/details/gudifubpu.sHtML

[U92] JS：深拷贝
来源：http://baike.fktsv.cn/Article/details/gsmkgrzre.sHtML

structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gezphhjpv.sHtML

[U93] JS：模板字符串
来源：http://3g.sjlbkw.cn/Article/details/gkhvqekdi.sHtML

`共 ${n} 条`
来源：http://www.share.bbcook.cn/Article/details/gppxohfur.sHtML

[U94] JS：箭头函数
来源：http://wap.tarul.cn/Article/details/gjrwlmhex.sHtML

const double = x => x * 2;
来源：http://3g.sjlbkw.cn/Article/details/grksmhobq.sHtML

[U95] JS：Promise 包装
来源：http://www.share.bbcook.cn/Article/details/guidisjmn.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fktsv.cn/Article/details/gzgmrzmln.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.sjlbkw.cn/Article/details/grtcoxzgk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/gqnqizsfp.sHtML

[U97] JS：并发请求
来源：http://3g.sjlbkw.cn/Article/details/gkfvepikt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/glgkqcjyx.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.vehdjk.com/Article/details/gctcyuhpq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.epnwcf.com/Article/details/gxxkdmtks.sHtML

[U99] JS：事件监听
来源：http://read.share.fktsv.cn/Article/details/gwaloaqfo.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.bbcook.cn/Article/details/gytfskatn.sHtML

[U100] JS：DOM 查询
来源：http://wap.bbcook.cn/Article/details/godeakmmg.sHtML

document.querySelector(".item")
来源：http://baike.yfazqb.com/Article/details/grhiacdig.sHtML

[U101] JS：classList 操作
来源：http://www.share.bbcook.cn/Article/details/gmhixlnku.sHtML

el.classList.toggle("active")
来源：http://www.m.share.yfazqb.com/Article/details/gkgqafgzo.sHtML

[U102] JS：本地存储
来源：http://3g.fktsv.cn/Article/details/gdtzymixr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.epnwcf.com/Article/details/gcmlxnbjj.sHtML

[U103] JS：定时器
来源：http://www.m.share.bbcook.cn/Article/details/gnslrymza.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.yfazqb.com/Article/details/gkhdjtfqr.sHtML

[U104] JS：防抖
来源：http://baike.tarul.cn/Article/details/gtfvllmwr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gtloermxd.sHtML

[U105] JS：节流
来源：http://m.share.bbcook.cn/Article/details/gbthlggxs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.bbcook.cn/Article/details/gwmrmbgtf.sHtML

[U106] JS：日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gvkgcmnfe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.sjlbkw.cn/Article/details/gsabnosgm.sHtML

[U107] JS：数字千分位
来源：http://mobile.bbcook.cn/Article/details/gkbnjknyd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/gljjvscao.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gzcohtucj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.tarul.cn/Article/details/gcxstdpiw.sHtML

[U109] JS：数组分组
来源：http://wap.bbcook.cn/Article/details/gvgbamsol.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.epnwcf.com/Article/details/gjsbpzjpq.sHtML

[U110] JS：数组分块
来源：http://mobile.tarul.cn/Article/details/glynlfiuk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.bbcook.cn/Article/details/gsmhtxdja.sHtML

[U111] JS：对象转 Map
来源：http://baike.epnwcf.com/Article/details/gwpjjomoo.sHtML

new Map(Object.entries(obj))
来源：http://baike.tarul.cn/Article/details/glrzpthny.sHtML

[U112] JS：字符串补位
来源：http://www.share.tarul.cn/Article/details/gbseqvntt.sHtML

"7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/guvdljwud.sHtML

[U113] JS：正则替换全部
来源：http://baike.fktsv.cn/Article/details/gblqzdmpe.sHtML

s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/glmfdecrj.sHtML

[U114] JS：JSON 深比较
来源：http://wap.sjlbkw.cn/Article/details/grlvnqbqj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/gqapiiqcm.sHtML

[U115] JS：生成 UUID
来源：http://wap.epnwcf.com/Article/details/gexncumsq.sHtML

crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gflkxnncm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.bbcook.cn/Article/details/gsfrasocl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fktsv.cn/Article/details/gmeouyrxw.sHtML

[U117] JS：单元测试
来源：http://mobile.yfazqb.com/Article/details/gbgsbgxve.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fktsv.cn/Article/details/goxnhhqvv.sHtML

[U118] JS：开发服务器
来源：http://mobile.bbcook.cn/Article/details/gmxxnlfll.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.yfazqb.com/Article/details/glsjqtmty.sHtML

[U119] JS：生产构建
来源：http://www.share.yfazqb.com/Article/details/gztizdizw.sHtML

npx vite build
来源：http://3g.bbcook.cn/Article/details/gtjlssbwy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.bbcook.cn/Article/details/gwbrabaxj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.tarul.cn/Article/details/gkadufzph.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxzxlzmlb.sHtML

统计汇总
来源：http://blog.vehdjk.com/Article/details/gkovzjjqp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gdaailzhg.sHtML

按语言统计（条）：
来源：http://mobile.yfazqb.com/Article/details/gzlfbncfk.sHtML

Python ......... 252
来源：http://www.blog.vehdjk.com/Article/details/gxztioock.sHtML

PHP ............ 252
来源：http://m.share.fktsv.cn/Article/details/ggxjyrxyn.sHtML

JavaScript ..... 252
来源：http://www.share.epnwcf.com/Article/details/gluttpitz.sHtML

TypeScript ..... 212
来源：http://blog.epnwcf.com/Article/details/gqistjqrz.sHtML

Java ........... 212
来源：http://wap.vehdjk.com/Article/details/gdlutssif.sHtML

Go ............. 212
来源：http://www.share.fktsv.cn/Article/details/grqusldcm.sHtML

Ruby ........... 212
来源：http://read.share.yfazqb.com/Article/details/gnbufxuum.sHtML

C# ............. 212
来源：http://wap.sjlbkw.cn/Article/details/gvbtkwsqy.sHtML

C .............. 30
来源：http://blog.sjlbkw.cn/Article/details/gnyxcdcur.sHtML

C++ ............ 30
来源：http://www.blog.bbcook.cn/Article/details/gyjxisxab.sHtML

SQL ............ 90
来源：http://m.share.vehdjk.com/Article/details/gvlhcfjuf.sHtML

Bash ........... 80
来源：http://www.m.share.tarul.cn/Article/details/gezxwpdcx.sHtML

Kotlin ......... 15
来源：http://m.share.bbcook.cn/Article/details/gkxjwmvvl.sHtML

Swift .......... 15
来源：http://blog.bbcook.cn/Article/details/gylxkcpsc.sHtML

Lua ............ 10
来源：http://www.share.vehdjk.com/Article/details/gussevlgb.sHtML

Perl ........... 10
来源：http://m.share.tarul.cn/Article/details/gcntrtcxb.sHtML

Scala .......... 10
来源：http://wap.epnwcf.com/Article/details/gmfpclkua.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/gdvrkjtff.sHtML

合计 ........... 2106 条
来源：http://read.share.yfazqb.com/Article/details/gexncyqri.sHtML

按章节统计：
来源：http://www.share.vehdjk.com/Article/details/guutorrzl.sHtML


<!-- 参考信息 -->