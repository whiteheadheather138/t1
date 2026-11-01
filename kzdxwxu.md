代发 wailian999

[T49] Perl：函数
来源：http://m.share.bbcook.cn/Article/details/gafcephpx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gxboaxfqa.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gyberiyiu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.tarul.cn/Article/details/gsykcxyld.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.tarul.cn/Article/details/gnohhpihz.sHtML

[T51] Scala：Hello World
来源：http://wap.fktsv.cn/Article/details/govdhhzvv.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gyexvymrx.sHtML

[T52] Scala：变量
来源：http://wap.fktsv.cn/Article/details/grphoxfvp.sHtML

val a = 1;  var b = 2
来源：http://3g.epnwcf.com/Article/details/glvvbvklb.sHtML

[T53] Scala：字符串插值
来源：http://blog.yfazqb.com/Article/details/gbpqprrif.sHtML

s"值: $b"
来源：http://m.share.tarul.cn/Article/details/gipczzvqg.sHtML

[T54] Scala：集合映射
来源：http://wap.epnwcf.com/Article/details/gynjaxawh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gsmidrytc.sHtML

[T55] Scala：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gltwfwiin.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.tarul.cn/Article/details/gspoophhk.sHtML

[T56] Scala：样例类
来源：http://blog.epnwcf.com/Article/details/gtpobyyqe.sHtML

case class User(name: String, age: Int)
来源：http://blog.fktsv.cn/Article/details/gcyuhojqp.sHtML

[T57] Scala：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gmafracsz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.tarul.cn/Article/details/gjfjnksme.sHtML

[T58] Scala：函数定义
来源：http://wap.bbcook.cn/Article/details/gghoatazz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.yfazqb.com/Article/details/gdnosmsqw.sHtML

[T59] Scala：循环
来源：http://3g.tarul.cn/Article/details/gkdktshug.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.tarul.cn/Article/details/ggpbqplnz.sHtML

[T60] Scala：折叠
来源：http://baike.vehdjk.com/Article/details/gjgmcibwb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.vehdjk.com/Article/details/gydmxdpcg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gmedmnqyu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gvzbddrok.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtnbxvgpz.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.vehdjk.com/Article/details/gwlestlkx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.yfazqb.com/Article/details/gygretfuo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fktsv.cn/Article/details/gxtutkswe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.sjlbkw.cn/Article/details/gsybgtcdu.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.epnwcf.com/Article/details/gzqpsnpcw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.sjlbkw.cn/Article/details/ghfwcpauz.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.bbcook.cn/Article/details/gwlarhdjp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.yfazqb.com/Article/details/grgjqfgyw.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fktsv.cn/Article/details/gtpagtlac.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gofqtozxg.sHtML

[U06] Py：合并两个字典
来源：http://wap.fktsv.cn/Article/details/ggvvecxdy.sHtML

{**a, **b}
来源：http://3g.vehdjk.com/Article/details/gwdmqiyvk.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.tarul.cn/Article/details/gkectdztb.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.bbcook.cn/Article/details/gyjqcafoq.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.yfazqb.com/Article/details/gjfxtwgzw.sHtML

[y for x in nested for y in x]
来源：http://3g.vehdjk.com/Article/details/gbdpksyzk.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.epnwcf.com/Article/details/gdkrxlizc.sHtML

max(d, key=d.get)
来源：http://www.m.share.fktsv.cn/Article/details/gwdnnjiht.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fktsv.cn/Article/details/ghhtwwfye.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.sjlbkw.cn/Article/details/godghtcer.sHtML

[U11] Py：生成器表达式
来源：http://read.share.yfazqb.com/Article/details/ggvraodsy.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fktsv.cn/Article/details/gsqukuiks.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.epnwcf.com/Article/details/guqilgyiw.sHtML

Counter(arr).most_common(3)
来源：http://m.share.epnwcf.com/Article/details/gveiuucbo.sHtML

[U13] Py：固定长度队列
来源：http://blog.yfazqb.com/Article/details/gulkzjthi.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/gueggsiej.sHtML

[U14] Py：分组收集到列表
来源：http://blog.epnwcf.com/Article/details/gnifkhkjs.sHtML

defaultdict(list)
来源：http://www.blog.vehdjk.com/Article/details/ghazwfqok.sHtML

[U15] Py：高精度计时
来源：http://wap.tarul.cn/Article/details/gwxfagrtk.sHtML

t = time.perf_counter()
来源：http://mobile.bbcook.cn/Article/details/gfvtljzxu.sHtML

[U16] Py：命令行参数解析
来源：http://wap.epnwcf.com/Article/details/gzbinnjbz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.bbcook.cn/Article/details/gpvlgeyvx.sHtML

[U17] Py：初始化日志
来源：http://wap.yfazqb.com/Article/details/gsfrvaolk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.sjlbkw.cn/Article/details/gyzlgdffd.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/gsepucxhq.sHtML

pat = re.compile(r"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gqosyrctb.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.bbcook.cn/Article/details/gipnilbsw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.vehdjk.com/Article/details/gcwslljbh.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.tarul.cn/Article/details/grvboefvc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.bbcook.cn/Article/details/gdpqrgpii.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.sjlbkw.cn/Article/details/gfynaxxoe.sHtML

@contextlib.contextmanager
来源：http://blog.tarul.cn/Article/details/grjuiuhpj.sHtML

[U22] Py：矩阵转置
来源：http://3g.bbcook.cn/Article/details/goiizeklo.sHtML

list(zip(*m))
来源：http://m.share.epnwcf.com/Article/details/gzjwdylrs.sHtML

[U23] Py：分块读取大文件
来源：http://baike.vehdjk.com/Article/details/gwphexnix.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.epnwcf.com/Article/details/gmaxbeefq.sHtML

[U24] Py：路径操作
来源：http://www.blog.vehdjk.com/Article/details/gpessexgn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/ghqppdyaj.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.bbcook.cn/Article/details/glhpyfwsg.sHtML

csv.DictReader(f)
来源：http://mobile.epnwcf.com/Article/details/gguymidde.sHtML

[U26] Py：并发下载
来源：http://m.share.yfazqb.com/Article/details/gbghyxvaf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.epnwcf.com/Article/details/gcbybapce.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.sjlbkw.cn/Article/details/gyevgfryi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.tarul.cn/Article/details/gabxuhnxa.sHtML

[U28] Py：类型别名
来源：http://baike.fktsv.cn/Article/details/gfvabxfza.sHtML

UserId = int
来源：http://baike.epnwcf.com/Article/details/gmnqnwatw.sHtML

[U29] Py：属性校验
来源：http://www.m.share.sjlbkw.cn/Article/details/gubxubshx.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.tarul.cn/Article/details/gadfxwnlm.sHtML

[U30] Py：数据类
来源：http://www.share.sjlbkw.cn/Article/details/globiavxj.sHtML

@dataclass(slots=True)
来源：http://blog.tarul.cn/Article/details/ggjobehgh.sHtML

[U31] Py：单测
来源：http://www.blog.vehdjk.com/Article/details/glufnejhg.sHtML

python -m pytest -q
来源：http://3g.tarul.cn/Article/details/gwodxkgtt.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fktsv.cn/Article/details/gquseufxo.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.epnwcf.com/Article/details/ggsfsokot.sHtML

[U33] Py：打包发布
来源：http://read.share.bbcook.cn/Article/details/ghsskyfoj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.bbcook.cn/Article/details/gfvndzgqf.sHtML

[U34] Py：判断编码
来源：http://blog.tarul.cn/Article/details/gpvomaazl.sHtML

chardet.detect(raw)
来源：http://baike.bbcook.cn/Article/details/gzqdlnhrj.sHtML

[U35] Py：发送邮件
来源：http://3g.vehdjk.com/Article/details/gnwwwrncd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.epnwcf.com/Article/details/gfjbkjrwo.sHtML

[U36] Py：定时任务
来源：http://3g.tarul.cn/Article/details/geobujcdx.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.epnwcf.com/Article/details/gfgrnybdp.sHtML

[U37] Py：读写 Excel
来源：http://blog.fktsv.cn/Article/details/gjyewvwvd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.epnwcf.com/Article/details/gwphygmov.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.sjlbkw.cn/Article/details/gzzxesaln.sHtML

Path(__file__).resolve().parent
来源：http://mobile.bbcook.cn/Article/details/giwbmwymm.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.epnwcf.com/Article/details/gqvokolmg.sHtML

sys.stdout.isatty()
来源：http://m.share.epnwcf.com/Article/details/gliabcabg.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.vehdjk.com/Article/details/gfzywhpbm.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gbefrtjhv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.epnwcf.com/Article/details/gldhsdrlm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.bbcook.cn/Article/details/gmidszalo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.epnwcf.com/Article/details/gvkzztlum.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fktsv.cn/Article/details/gujszoole.sHtML

[U43] PHP：声明命名空间
来源：http://wap.vehdjk.com/Article/details/gdlcjalwd.sHtML

namespace App\Http;
来源：http://www.blog.yfazqb.com/Article/details/gryueajef.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fktsv.cn/Article/details/gyexhxygc.sHtML

declare(strict_types=1);
来源：http://read.share.epnwcf.com/Article/details/ghqvydoqv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.yfazqb.com/Article/details/gghttdtei.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gevsctjrz.sHtML

[U46] PHP：可空类型
来源：http://baike.yfazqb.com/Article/details/gzofcfgvm.sHtML

?string $name = null
来源：http://baike.bbcook.cn/Article/details/glhsegznk.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fktsv.cn/Article/details/giybndwul.sHtML

int|string $id
来源：http://3g.yfazqb.com/Article/details/gnhweqihf.sHtML

[U48] PHP：纯枚举
来源：http://www.share.epnwcf.com/Article/details/gqlxmjxog.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.yfazqb.com/Article/details/gnfyefcug.sHtML

[U49] PHP：只读属性
来源：http://www.share.tarul.cn/Article/details/gdckrfjyn.sHtML

public readonly string $name
来源：http://baike.vehdjk.com/Article/details/gybkorlrn.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.vehdjk.com/Article/details/giuqdmsua.sHtML

public function __construct(private int $id) {}
来源：http://m.share.tarul.cn/Article/details/ghfornahl.sHtML

[U51] PHP：数组解构
来源：http://read.share.vehdjk.com/Article/details/gsxulurqi.sHtML

[$a, $b] = $arr;
来源：http://m.share.tarul.cn/Article/details/guroiazul.sHtML

[U52] PHP：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gkmendbls.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.yfazqb.com/Article/details/gakpciwjz.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.sjlbkw.cn/Article/details/giqchqiwc.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fktsv.cn/Article/details/gdhhelqrg.sHtML

[U54] PHP：空安全调用
来源：http://wap.vehdjk.com/Article/details/ghcwhroao.sHtML

$obj?->method()
来源：http://www.blog.tarul.cn/Article/details/gjnzgfwwv.sHtML

[U55] PHP：match 表达式
来源：http://wap.yfazqb.com/Article/details/golqkqwhk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.epnwcf.com/Article/details/gopzguaaa.sHtML

[U56] PHP：命名参数
来源：http://mobile.fktsv.cn/Article/details/gxllagtkj.sHtML

f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gwjkibwmi.sHtML

[U57] PHP：字符串插值
来源：http://3g.yfazqb.com/Article/details/goyclqvzu.sHtML

"值: {$a}"
来源：http://wap.epnwcf.com/Article/details/gmocdzdwr.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.vehdjk.com/Article/details/gbxcrgtkh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.tarul.cn/Article/details/goduwbhji.sHtML

[U59] PHP：自定义排序
来源：http://blog.vehdjk.com/Article/details/ghpkladzr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.tarul.cn/Article/details/gnwfyqsee.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.bbcook.cn/Article/details/gwuckrynv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.yfazqb.com/Article/details/gepitirld.sHtML

[U61] PHP：正则
来源：http://baike.yfazqb.com/Article/details/ghdyymvdm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/gxekfmomq.sHtML

[U62] PHP：日期对象
来源：http://baike.tarul.cn/Article/details/gzldmysvh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.tarul.cn/Article/details/gaguwfzjk.sHtML

[U63] PHP：文件读写
来源：http://3g.epnwcf.com/Article/details/gruvzmfmb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.tarul.cn/Article/details/gbfkhelzj.sHtML

[U64] PHP：目录遍历
来源：http://mobile.sjlbkw.cn/Article/details/gvegqatht.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.tarul.cn/Article/details/gspbwkhlk.sHtML

[U65] PHP：会话
来源：http://wap.yfazqb.com/Article/details/gxvufqpvi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.yfazqb.com/Article/details/glcohmtqt.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.yfazqb.com/Article/details/gcidjbkxu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fktsv.cn/Article/details/gjfxjcwpo.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.bbcook.cn/Article/details/gqsezrvph.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.epnwcf.com/Article/details/gwxkibnpq.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fktsv.cn/Article/details/gvwwkyise.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fktsv.cn/Article/details/gkckcikkx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.tarul.cn/Article/details/givmeirah.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.yfazqb.com/Article/details/ggpopfvec.sHtML

[U70] PHP：PDO 事务
来源：http://3g.yfazqb.com/Article/details/gjqzarbyl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.tarul.cn/Article/details/grjzxotyg.sHtML

[U71] PHP：抛出异常
来源：http://www.share.vehdjk.com/Article/details/gwdsjwvhb.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.yfazqb.com/Article/details/gumfjlwtc.sHtML

[U72] PHP：写错误日志
来源：http://mobile.epnwcf.com/Article/details/glxhemnpz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.vehdjk.com/Article/details/gmgkgmvit.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.yfazqb.com/Article/details/gryhtcfbo.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fktsv.cn/Article/details/gcdtsxjnw.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/grlytcpab.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fktsv.cn/Article/details/gyvanznwl.sHtML

[U75] PHP：依赖注入
来源：http://wap.tarul.cn/Article/details/gcatwital.sHtML

composer require psr/container
来源：http://wap.tarul.cn/Article/details/gwihgfekm.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.tarul.cn/Article/details/gjultfmzi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.yfazqb.com/Article/details/goakqetvf.sHtML

[U77] PHP：模板渲染
来源：http://read.share.bbcook.cn/Article/details/gxadsatkl.sHtML

composer require twig/twig
来源：http://mobile.fktsv.cn/Article/details/gejqhapmi.sHtML

[U78] PHP：单元测试
来源：http://www.blog.vehdjk.com/Article/details/gqwtyxunq.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.vehdjk.com/Article/details/gnyvwrhfd.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.yfazqb.com/Article/details/gdhvxvmah.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.vehdjk.com/Article/details/gbdrfsikf.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.yfazqb.com/Article/details/giwahrtda.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.yfazqb.com/Article/details/gnepbheoc.sHtML

[U81] JS：初始化项目
来源：http://mobile.bbcook.cn/Article/details/gcohwjcqq.sHtML

npm init -y;  npm i express
来源：http://baike.sjlbkw.cn/Article/details/gwlblponc.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.bbcook.cn/Article/details/geilxuvdl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.bbcook.cn/Article/details/gvbyqgszf.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.vehdjk.com/Article/details/gigsycwxp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.tarul.cn/Article/details/gtgeydcjx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.bbcook.cn/Article/details/gvoydozxk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.yfazqb.com/Article/details/guwxmzwpp.sHtML

[U85] JS：可选链
来源：http://3g.vehdjk.com/Article/details/gqgeeuton.sHtML

a?.b?.c
来源：http://3g.sjlbkw.cn/Article/details/gsoxmcbzn.sHtML

[U86] JS：空值合并
来源：http://mobile.yfazqb.com/Article/details/gwbaikckn.sHtML

a ?? b
来源：http://blog.epnwcf.com/Article/details/ghlxqyruq.sHtML

[U87] JS：解构默认值
来源：http://baike.sjlbkw.cn/Article/details/gdahjowdj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.epnwcf.com/Article/details/gafntcmfg.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fktsv.cn/Article/details/ghjfdnkac.sHtML

{ ...a, ...b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaydiwjzb.sHtML

[U89] JS：数组去重
来源：http://read.share.yfazqb.com/Article/details/giibcdskt.sHtML

[...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gfqvnmulp.sHtML

[U90] JS：数字数组排序
来源：http://read.share.bbcook.cn/Article/details/gedjlqzgk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gfkuzpjbi.sHtML

[U91] JS：对象键值遍历
来源：http://wap.epnwcf.com/Article/details/gfpjqdqls.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.epnwcf.com/Article/details/ghojcurfp.sHtML

[U92] JS：深拷贝
来源：http://mobile.vehdjk.com/Article/details/glunygxeu.sHtML

structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gsthutoym.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.yfazqb.com/Article/details/gvbyspyvh.sHtML

`共 ${n} 条`
来源：http://m.share.sjlbkw.cn/Article/details/gyibpcuhn.sHtML

[U94] JS：箭头函数
来源：http://www.blog.vehdjk.com/Article/details/gtorpwfdp.sHtML

const double = x => x * 2;
来源：http://blog.epnwcf.com/Article/details/grupqgodu.sHtML

[U95] JS：Promise 包装
来源：http://3g.sjlbkw.cn/Article/details/ggkncjuex.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.yfazqb.com/Article/details/gfiqprpgi.sHtML

[U96] JS：async/await 与异常
来源：http://wap.bbcook.cn/Article/details/gpwtrfaqq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gdpvznlmc.sHtML

[U97] JS：并发请求
来源：http://baike.vehdjk.com/Article/details/gvjlveivx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/grceiwqyd.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.tarul.cn/Article/details/gsgloflvj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.vehdjk.com/Article/details/gvrxbmyry.sHtML

[U99] JS：事件监听
来源：http://blog.bbcook.cn/Article/details/gehzsfiex.sHtML

el.addEventListener("click", e => {})
来源：http://3g.epnwcf.com/Article/details/glpnesvak.sHtML

[U100] JS：DOM 查询
来源：http://m.share.epnwcf.com/Article/details/gfnucypev.sHtML

document.querySelector(".item")
来源：http://blog.sjlbkw.cn/Article/details/ghjitgoqp.sHtML

[U101] JS：classList 操作
来源：http://www.share.bbcook.cn/Article/details/ggbowpfsx.sHtML

el.classList.toggle("active")
来源：http://m.share.fktsv.cn/Article/details/gvzimwvzq.sHtML

[U102] JS：本地存储
来源：http://m.share.epnwcf.com/Article/details/gefekhtzk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fktsv.cn/Article/details/gdaqohzmd.sHtML

[U103] JS：定时器
来源：http://read.share.sjlbkw.cn/Article/details/gffqhlmsa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.sjlbkw.cn/Article/details/gxqdhkijd.sHtML

[U104] JS：防抖
来源：http://www.blog.yfazqb.com/Article/details/ggjrpyfec.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gyikmqged.sHtML

[U105] JS：节流
来源：http://www.share.vehdjk.com/Article/details/gncrxyyxu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.sjlbkw.cn/Article/details/gcspgqxru.sHtML

[U106] JS：日期格式化
来源：http://blog.yfazqb.com/Article/details/gnmsqazve.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.bbcook.cn/Article/details/gvnovbgoz.sHtML

[U107] JS：数字千分位
来源：http://3g.fktsv.cn/Article/details/gyajxmhhc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.tarul.cn/Article/details/gdjziozep.sHtML

[U108] JS：随机整数
来源：http://3g.tarul.cn/Article/details/glfkibrqr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.tarul.cn/Article/details/ggakcsqjl.sHtML

[U109] JS：数组分组
来源：http://blog.sjlbkw.cn/Article/details/gtzlieoap.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/gidguonhd.sHtML

[U110] JS：数组分块
来源：http://3g.fktsv.cn/Article/details/glckzzhus.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fktsv.cn/Article/details/ggiecnchc.sHtML

[U111] JS：对象转 Map
来源：http://baike.vehdjk.com/Article/details/gjiewcadj.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gkwjjhqpr.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxrmghkz.sHtML

"7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gxltawqeo.sHtML

[U113] JS：正则替换全部
来源：http://wap.sjlbkw.cn/Article/details/ggbjeybxk.sHtML

s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/glzyfekgn.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.yfazqb.com/Article/details/gqrvqulvr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/gxaawoshw.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.bbcook.cn/Article/details/ggwwrqgdx.sHtML

crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/geceqgtmk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.sjlbkw.cn/Article/details/gvhjpfgjx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fktsv.cn/Article/details/gkesuhjxy.sHtML

[U117] JS：单元测试
来源：http://baike.yfazqb.com/Article/details/gputoljit.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fktsv.cn/Article/details/ghltaqpes.sHtML

[U118] JS：开发服务器
来源：http://baike.bbcook.cn/Article/details/gsvbuhlbz.sHtML

npm i -D vite;  npx vite
来源：http://wap.vehdjk.com/Article/details/gyuttuirm.sHtML

[U119] JS：生产构建
来源：http://blog.tarul.cn/Article/details/gewffxttb.sHtML

npx vite build
来源：http://mobile.tarul.cn/Article/details/gfkoabiqr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.bbcook.cn/Article/details/gxkoyenav.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.bbcook.cn/Article/details/gmnkemfjm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtbtfkvxv.sHtML

统计汇总
来源：http://www.m.share.yfazqb.com/Article/details/gdbywgvkz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqioderqc.sHtML

按语言统计（条）：
来源：http://3g.epnwcf.com/Article/details/gjreovfxo.sHtML

Python ......... 252
来源：http://3g.bbcook.cn/Article/details/gobtpqqin.sHtML

PHP ............ 252
来源：http://www.m.share.epnwcf.com/Article/details/gdwbayqjb.sHtML

JavaScript ..... 252
来源：http://read.share.sjlbkw.cn/Article/details/gfnqnirze.sHtML

TypeScript ..... 212
来源：http://blog.bbcook.cn/Article/details/gjuqqupmk.sHtML

Java ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gvfwxhzvc.sHtML

Go ............. 212
来源：http://mobile.bbcook.cn/Article/details/gghnxlgnr.sHtML

Ruby ........... 212
来源：http://blog.fktsv.cn/Article/details/gpketcvuh.sHtML

C# ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/gknuibkyc.sHtML

C .............. 30
来源：http://blog.vehdjk.com/Article/details/ghwbnjnan.sHtML

C++ ............ 30
来源：http://www.m.share.fktsv.cn/Article/details/guafjhumu.sHtML

SQL ............ 90
来源：http://read.share.epnwcf.com/Article/details/gnvwyzvbk.sHtML

Bash ........... 80
来源：http://m.share.vehdjk.com/Article/details/gzouppama.sHtML

Kotlin ......... 15
来源：http://baike.epnwcf.com/Article/details/gqtxlkmce.sHtML

Swift .......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gzwkvybff.sHtML

Lua ............ 10
来源：http://wap.fktsv.cn/Article/details/gogeyvujb.sHtML

Perl ........... 10
来源：http://3g.sjlbkw.cn/Article/details/gncjoblhk.sHtML

Scala .......... 10
来源：http://www.share.sjlbkw.cn/Article/details/gihvwiqpx.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gyoqgmtie.sHtML

合计 ........... 2106 条
来源：http://blog.yfazqb.com/Article/details/ggjwkewgd.sHtML

按章节统计：
来源：http://3g.fktsv.cn/Article/details/gynnhkocg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.yfazqb.com/Article/details/gfhwpjwdn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gouysuwki.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gvgywihhh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/gzlazufke.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fktsv.cn/Article/details/gemtdtegs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.bbcook.cn/Article/details/gxeelqeen.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gafamabyp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.yfazqb.com/Article/details/gnjdlfiue.sHtML


<!-- 参考信息 -->