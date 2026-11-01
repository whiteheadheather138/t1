代发 wailian999

[T47] Perl：正则捕获
来源：http://read.share.fktsv.cn/Article/details/gvvnrghgc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.epnwcf.com/Article/details/gdmhtdgjj.sHtML

[T48] Perl：正则替换
来源：http://3g.sjlbkw.cn/Article/details/gjhoyqayr.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fktsv.cn/Article/details/gjeoyzgqe.sHtML

[T49] Perl：函数
来源：http://mobile.fktsv.cn/Article/details/gbiudaccd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gplxllakk.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gsarcmjqh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.bbcook.cn/Article/details/gfczzxxxz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gntudlhtk.sHtML

[T51] Scala：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/glueejarg.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gghqpynxx.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gaovopjsb.sHtML

val a = 1;  var b = 2
来源：http://blog.epnwcf.com/Article/details/gkcngtyaq.sHtML

[T53] Scala：字符串插值
来源：http://3g.fktsv.cn/Article/details/goehcxcea.sHtML

s"值: $b"
来源：http://baike.epnwcf.com/Article/details/gitpnfxxp.sHtML

[T54] Scala：集合映射
来源：http://www.blog.bbcook.cn/Article/details/grsivwqsl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.tarul.cn/Article/details/glnknhqdn.sHtML

[T55] Scala：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gbweqgkwz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.vehdjk.com/Article/details/givskfody.sHtML

[T56] Scala：样例类
来源：http://www.blog.yfazqb.com/Article/details/gjvuetwpw.sHtML

case class User(name: String, age: Int)
来源：http://read.share.yfazqb.com/Article/details/gmkohxlrr.sHtML

[T57] Scala：模式匹配
来源：http://www.share.epnwcf.com/Article/details/ghdwnokbc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.tarul.cn/Article/details/gssdjwjxe.sHtML

[T58] Scala：函数定义
来源：http://3g.bbcook.cn/Article/details/gyasnjuas.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.yfazqb.com/Article/details/gtxrlomav.sHtML

[T59] Scala：循环
来源：http://3g.epnwcf.com/Article/details/gwcijewec.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/gfbtojwue.sHtML

[T60] Scala：折叠
来源：http://3g.bbcook.cn/Article/details/gptraedya.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.tarul.cn/Article/details/gysheeebc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmqylcadg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fktsv.cn/Article/details/gdjqtedai.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gbhlaxplw.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.yfazqb.com/Article/details/gjdvovqao.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.sjlbkw.cn/Article/details/gollaclev.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.bbcook.cn/Article/details/ggogsievg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.tarul.cn/Article/details/gusxzvfqi.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.vehdjk.com/Article/details/grrkkqtmx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.yfazqb.com/Article/details/gggemavvs.sHtML

[U04] Py：变量调试打印
来源：http://mobile.tarul.cn/Article/details/gfczyudrj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.epnwcf.com/Article/details/gefefmxbm.sHtML

[U05] Py：列表去重且保序
来源：http://baike.vehdjk.com/Article/details/gvgkrpccb.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gkycqitfw.sHtML

[U06] Py：合并两个字典
来源：http://baike.tarul.cn/Article/details/gcqvdbmvk.sHtML

{**a, **b}
来源：http://www.blog.vehdjk.com/Article/details/gvbfdzmmd.sHtML

[U07] Py：反转字典键值
来源：http://baike.fktsv.cn/Article/details/gefqrpdfu.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.tarul.cn/Article/details/gltpjfepi.sHtML

[U08] Py：展平二维列表
来源：http://blog.yfazqb.com/Article/details/gqvjpxxcf.sHtML

[y for x in nested for y in x]
来源：http://www.share.yfazqb.com/Article/details/gecllxbbt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.vehdjk.com/Article/details/gqmdloojj.sHtML

max(d, key=d.get)
来源：http://mobile.bbcook.cn/Article/details/gxfpsyqtc.sHtML

[U10] Py：按值排序字典
来源：http://baike.yfazqb.com/Article/details/gqmgbfiwd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.yfazqb.com/Article/details/gcucyvpqf.sHtML

[U11] Py：生成器表达式
来源：http://wap.tarul.cn/Article/details/gszzhmdrp.sHtML

(x * 2 for x in arr)
来源：http://blog.epnwcf.com/Article/details/grqwbaaeq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.yfazqb.com/Article/details/gieshejxo.sHtML

Counter(arr).most_common(3)
来源：http://3g.yfazqb.com/Article/details/gotjfnatt.sHtML

[U13] Py：固定长度队列
来源：http://read.share.vehdjk.com/Article/details/grbydhpdl.sHtML

deque(maxlen=10)
来源：http://read.share.yfazqb.com/Article/details/gifxsbmbg.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.epnwcf.com/Article/details/gygrjhnrf.sHtML

defaultdict(list)
来源：http://blog.bbcook.cn/Article/details/gdqzetqkq.sHtML

[U15] Py：高精度计时
来源：http://www.blog.vehdjk.com/Article/details/gjyyfacpb.sHtML

t = time.perf_counter()
来源：http://mobile.yfazqb.com/Article/details/gevffeopa.sHtML

[U16] Py：命令行参数解析
来源：http://baike.vehdjk.com/Article/details/gmcshgxpv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.vehdjk.com/Article/details/gisxszxjo.sHtML

[U17] Py：初始化日志
来源：http://www.blog.bbcook.cn/Article/details/gpbgdwcox.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.tarul.cn/Article/details/gpnfvivox.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fktsv.cn/Article/details/garqhmfcd.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.tarul.cn/Article/details/gqmrgdsxq.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.vehdjk.com/Article/details/gebemzvsf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.sjlbkw.cn/Article/details/gkulevnvx.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fktsv.cn/Article/details/gqwdxcoxf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.sjlbkw.cn/Article/details/gdluzaeiu.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.sjlbkw.cn/Article/details/gfzceeeue.sHtML

@contextlib.contextmanager
来源：http://m.share.yfazqb.com/Article/details/gemssoicw.sHtML

[U22] Py：矩阵转置
来源：http://wap.fktsv.cn/Article/details/gdhpbecsa.sHtML

list(zip(*m))
来源：http://www.blog.sjlbkw.cn/Article/details/gfgxvdsal.sHtML

[U23] Py：分块读取大文件
来源：http://wap.tarul.cn/Article/details/gamqoesmt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.bbcook.cn/Article/details/gphjcvuee.sHtML

[U24] Py：路径操作
来源：http://www.blog.vehdjk.com/Article/details/gjjtjbtfi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/gojhcdnpq.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.vehdjk.com/Article/details/ggzkmpxdx.sHtML

csv.DictReader(f)
来源：http://wap.fktsv.cn/Article/details/gijjedxla.sHtML

[U26] Py：并发下载
来源：http://mobile.sjlbkw.cn/Article/details/gvtwrvzrq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.epnwcf.com/Article/details/gflxejbkp.sHtML

[U27] Py：异步 HTTP
来源：http://3g.bbcook.cn/Article/details/gquattcrp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.bbcook.cn/Article/details/gfijegrdq.sHtML

[U28] Py：类型别名
来源：http://blog.vehdjk.com/Article/details/gmjxzserf.sHtML

UserId = int
来源：http://wap.sjlbkw.cn/Article/details/gcvytqrhw.sHtML

[U29] Py：属性校验
来源：http://www.blog.fktsv.cn/Article/details/giffirkiz.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.yfazqb.com/Article/details/gjwggyakp.sHtML

[U30] Py：数据类
来源：http://baike.bbcook.cn/Article/details/gmhhnviec.sHtML

@dataclass(slots=True)
来源：http://blog.tarul.cn/Article/details/ghpuahvjb.sHtML

[U31] Py：单测
来源：http://mobile.fktsv.cn/Article/details/gxwsjvglt.sHtML

python -m pytest -q
来源：http://read.share.tarul.cn/Article/details/gpfhjwsda.sHtML

[U32] Py：代码格式化
来源：http://wap.bbcook.cn/Article/details/gwckjqhib.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fktsv.cn/Article/details/gfmrrmfaw.sHtML

[U33] Py：打包发布
来源：http://blog.bbcook.cn/Article/details/gsfkyqlmv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.tarul.cn/Article/details/gtlxwvcjm.sHtML

[U34] Py：判断编码
来源：http://blog.vehdjk.com/Article/details/gqzsvitxs.sHtML

chardet.detect(raw)
来源：http://blog.bbcook.cn/Article/details/gpqldcmiq.sHtML

[U35] Py：发送邮件
来源：http://wap.fktsv.cn/Article/details/gaheilxof.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.sjlbkw.cn/Article/details/glfdnhdom.sHtML

[U36] Py：定时任务
来源：http://baike.sjlbkw.cn/Article/details/gwqakabed.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.sjlbkw.cn/Article/details/gbdqsuwgz.sHtML

[U37] Py：读写 Excel
来源：http://wap.tarul.cn/Article/details/gozbwswyv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.yfazqb.com/Article/details/gkbbqdgwx.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.vehdjk.com/Article/details/guwzsdzyn.sHtML

Path(__file__).resolve().parent
来源：http://read.share.yfazqb.com/Article/details/gcgiinsjl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.vehdjk.com/Article/details/gfwjsftss.sHtML

sys.stdout.isatty()
来源：http://www.blog.sjlbkw.cn/Article/details/ghnjbajbu.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.epnwcf.com/Article/details/giyhiyewf.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gcyzzrcqs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.vehdjk.com/Article/details/guseegsmz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fktsv.cn/Article/details/ghdewiteu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fktsv.cn/Article/details/ganljhzre.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.sjlbkw.cn/Article/details/gvymbriwv.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.yfazqb.com/Article/details/gfcggbdvq.sHtML

namespace App\Http;
来源：http://www.blog.epnwcf.com/Article/details/ghvotwlxq.sHtML

[U44] PHP：开启严格类型
来源：http://blog.vehdjk.com/Article/details/gvfrjotcu.sHtML

declare(strict_types=1);
来源：http://www.blog.yfazqb.com/Article/details/gamsdmxua.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fktsv.cn/Article/details/gaguutfjv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gbizuvnbd.sHtML

[U46] PHP：可空类型
来源：http://www.blog.sjlbkw.cn/Article/details/gtdraqrfo.sHtML

?string $name = null
来源：http://3g.fktsv.cn/Article/details/gbhgxvzup.sHtML

[U47] PHP：联合类型
来源：http://m.share.tarul.cn/Article/details/gunhgvybd.sHtML

int|string $id
来源：http://3g.fktsv.cn/Article/details/gebdiokey.sHtML

[U48] PHP：纯枚举
来源：http://mobile.tarul.cn/Article/details/gpqrbjgkm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.vehdjk.com/Article/details/govktmkvm.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.yfazqb.com/Article/details/gnlgcczje.sHtML

public readonly string $name
来源：http://www.blog.epnwcf.com/Article/details/ghrbtfopf.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.bbcook.cn/Article/details/gzvdmpkhx.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.tarul.cn/Article/details/gjbarhigv.sHtML

[U51] PHP：数组解构
来源：http://read.share.epnwcf.com/Article/details/gxaueueja.sHtML

[$a, $b] = $arr;
来源：http://read.share.fktsv.cn/Article/details/gducijljc.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gkcibflmp.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.epnwcf.com/Article/details/gkfwjaakp.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.sjlbkw.cn/Article/details/grjhpddxw.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.epnwcf.com/Article/details/gtbzuflqn.sHtML

[U54] PHP：空安全调用
来源：http://wap.bbcook.cn/Article/details/gehqytnym.sHtML

$obj?->method()
来源：http://blog.epnwcf.com/Article/details/gtvevvipz.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gtmamfdbx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fktsv.cn/Article/details/ggylvmczy.sHtML

[U56] PHP：命名参数
来源：http://www.blog.yfazqb.com/Article/details/gdokhprxc.sHtML

f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/goekccsco.sHtML

[U57] PHP：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gwahwxwyg.sHtML

"值: {$a}"
来源：http://3g.tarul.cn/Article/details/gcqgyiqkc.sHtML

[U58] PHP：数组三件套
来源：http://3g.bbcook.cn/Article/details/gjtbrzwex.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fktsv.cn/Article/details/ghwmqdyjj.sHtML

[U59] PHP：自定义排序
来源：http://mobile.sjlbkw.cn/Article/details/gyomeazjb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.vehdjk.com/Article/details/gotbfbcrn.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.bbcook.cn/Article/details/gnduajxbm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.vehdjk.com/Article/details/gdwxzklce.sHtML

[U61] PHP：正则
来源：http://www.m.share.fktsv.cn/Article/details/gaawhmxvl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gbpfbppit.sHtML

[U62] PHP：日期对象
来源：http://read.share.sjlbkw.cn/Article/details/gpsvbzruy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.yfazqb.com/Article/details/gpviifyjy.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.bbcook.cn/Article/details/grtdqrzao.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkphjinja.sHtML

[U64] PHP：目录遍历
来源：http://blog.bbcook.cn/Article/details/gzckssgvu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.bbcook.cn/Article/details/gzyzmludj.sHtML

[U65] PHP：会话
来源：http://www.m.share.tarul.cn/Article/details/grjeubdko.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.tarul.cn/Article/details/gjsfbmiss.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.yfazqb.com/Article/details/gnhbaotqv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.tarul.cn/Article/details/gxkdetrhn.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fktsv.cn/Article/details/glwamlfil.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fktsv.cn/Article/details/gstkdcvpe.sHtML

[U68] PHP：PDO 连接
来源：http://blog.yfazqb.com/Article/details/gjnznrdip.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.sjlbkw.cn/Article/details/grgzwikgs.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.epnwcf.com/Article/details/gaqoihkvx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.sjlbkw.cn/Article/details/gmmactygb.sHtML

[U70] PHP：PDO 事务
来源：http://baike.sjlbkw.cn/Article/details/gqflzovnq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.epnwcf.com/Article/details/glkfmzhhh.sHtML

[U71] PHP：抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gitjbcykv.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fktsv.cn/Article/details/gqwzicebe.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.bbcook.cn/Article/details/ghdvqmmky.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.tarul.cn/Article/details/gmxibftge.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.epnwcf.com/Article/details/gjsvuwocf.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.yfazqb.com/Article/details/gdbxxssxn.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fktsv.cn/Article/details/gquwwmkxc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.tarul.cn/Article/details/gnktpcbss.sHtML

[U75] PHP：依赖注入
来源：http://blog.sjlbkw.cn/Article/details/glmoicxso.sHtML

composer require psr/container
来源：http://www.m.share.fktsv.cn/Article/details/gjxvjrgkx.sHtML

[U76] PHP：简单路由
来源：http://baike.epnwcf.com/Article/details/gnficzqlg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.vehdjk.com/Article/details/gkdbdlngn.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.bbcook.cn/Article/details/gyxjvsbbo.sHtML

composer require twig/twig
来源：http://blog.yfazqb.com/Article/details/gzinolren.sHtML

[U78] PHP：单元测试
来源：http://read.share.tarul.cn/Article/details/grnxahium.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.epnwcf.com/Article/details/gjjlbaovw.sHtML

[U79] PHP：静态分析
来源：http://read.share.fktsv.cn/Article/details/gscyewxqj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fktsv.cn/Article/details/gbmkoozks.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.tarul.cn/Article/details/gvrtkqgga.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.epnwcf.com/Article/details/gxmymbulh.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fktsv.cn/Article/details/gdxpzmifj.sHtML

npm init -y;  npm i express
来源：http://www.share.yfazqb.com/Article/details/gweuuxcjx.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fktsv.cn/Article/details/geepgkpwr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fktsv.cn/Article/details/gcsyicmcr.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.bbcook.cn/Article/details/gdpjxiyzm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gawpqtqax.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.yfazqb.com/Article/details/gxgfriygv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fktsv.cn/Article/details/ghvmrvglv.sHtML

[U85] JS：可选链
来源：http://m.share.bbcook.cn/Article/details/gpkapzfnq.sHtML

a?.b?.c
来源：http://blog.bbcook.cn/Article/details/gawwmstji.sHtML

[U86] JS：空值合并
来源：http://www.share.fktsv.cn/Article/details/gwflsvkre.sHtML

a ?? b
来源：http://www.share.sjlbkw.cn/Article/details/gjtwebdts.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.yfazqb.com/Article/details/gypxvxcno.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fktsv.cn/Article/details/gcxltbtyt.sHtML

[U88] JS：对象展开合并
来源：http://www.share.sjlbkw.cn/Article/details/guvmmitmd.sHtML

{ ...a, ...b }
来源：http://m.share.sjlbkw.cn/Article/details/gwrcuyiyc.sHtML

[U89] JS：数组去重
来源：http://blog.bbcook.cn/Article/details/gxtxmcvil.sHtML

[...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gblibreum.sHtML

[U90] JS：数字数组排序
来源：http://blog.sjlbkw.cn/Article/details/gkqcrkuhc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gwokjkkkt.sHtML

[U91] JS：对象键值遍历
来源：http://3g.sjlbkw.cn/Article/details/giwyxyavr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fktsv.cn/Article/details/gnqihqkwu.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gellrivrc.sHtML

structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gibdhrdod.sHtML

[U93] JS：模板字符串
来源：http://www.blog.tarul.cn/Article/details/gmtwlpbyg.sHtML

`共 ${n} 条`
来源：http://m.share.epnwcf.com/Article/details/ghafwkkvy.sHtML

[U94] JS：箭头函数
来源：http://www.blog.epnwcf.com/Article/details/gthqanlsh.sHtML

const double = x => x * 2;
来源：http://wap.tarul.cn/Article/details/glyrepedj.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fktsv.cn/Article/details/gbaehvmyj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.sjlbkw.cn/Article/details/gdbfeerue.sHtML

[U96] JS：async/await 与异常
来源：http://wap.sjlbkw.cn/Article/details/gpgfatfxw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/ghmwomyyk.sHtML

[U97] JS：并发请求
来源：http://www.share.vehdjk.com/Article/details/gpucallqf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gteraidux.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.vehdjk.com/Article/details/gaiskkruy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.tarul.cn/Article/details/gqinrohbq.sHtML

[U99] JS：事件监听
来源：http://m.share.sjlbkw.cn/Article/details/gmaymqvty.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqilnflw.sHtML

[U100] JS：DOM 查询
来源：http://read.share.epnwcf.com/Article/details/gfrfkeozo.sHtML

document.querySelector(".item")
来源：http://www.blog.yfazqb.com/Article/details/ggxkygntr.sHtML

[U101] JS：classList 操作
来源：http://mobile.vehdjk.com/Article/details/gyalekmlx.sHtML

el.classList.toggle("active")
来源：http://www.share.vehdjk.com/Article/details/gysxjdlhs.sHtML

[U102] JS：本地存储
来源：http://blog.fktsv.cn/Article/details/gafatiqkx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.tarul.cn/Article/details/gjxtcclac.sHtML

[U103] JS：定时器
来源：http://m.share.yfazqb.com/Article/details/gtqiahvwx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.tarul.cn/Article/details/gmmueynhb.sHtML

[U104] JS：防抖
来源：http://m.share.vehdjk.com/Article/details/gtferrirm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gctsbxaci.sHtML

[U105] JS：节流
来源：http://blog.vehdjk.com/Article/details/gqcovpkdc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.tarul.cn/Article/details/gqtvczqaw.sHtML

[U106] JS：日期格式化
来源：http://baike.fktsv.cn/Article/details/gjceypwol.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.vehdjk.com/Article/details/gzbexdiyg.sHtML

[U107] JS：数字千分位
来源：http://read.share.vehdjk.com/Article/details/gqmetzadq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/guafuvhxw.sHtML

[U108] JS：随机整数
来源：http://wap.vehdjk.com/Article/details/gfuccfsbp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.yfazqb.com/Article/details/gzkxcnmma.sHtML

[U109] JS：数组分组
来源：http://www.share.yfazqb.com/Article/details/gxxruahfe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.vehdjk.com/Article/details/ggnykhskd.sHtML

[U110] JS：数组分块
来源：http://wap.tarul.cn/Article/details/gidnghijh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.yfazqb.com/Article/details/grlpavdvh.sHtML

[U111] JS：对象转 Map
来源：http://blog.vehdjk.com/Article/details/grromgfil.sHtML

new Map(Object.entries(obj))
来源：http://m.share.vehdjk.com/Article/details/gqlsabqfl.sHtML

[U112] JS：字符串补位
来源：http://3g.yfazqb.com/Article/details/gdvgirlhu.sHtML

"7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gzhcdrczn.sHtML

[U113] JS：正则替换全部
来源：http://blog.bbcook.cn/Article/details/gjqgdwzws.sHtML

s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/ggdoaorin.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.epnwcf.com/Article/details/gmttxlumv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/gmuafcsbr.sHtML

[U115] JS：生成 UUID
来源：http://blog.yfazqb.com/Article/details/gzxcfliyy.sHtML

crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/guttgxhpl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.sjlbkw.cn/Article/details/gajzqgtrz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fktsv.cn/Article/details/gymidpawk.sHtML

[U117] JS：单元测试
来源：http://m.share.tarul.cn/Article/details/gdjwtoofj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.sjlbkw.cn/Article/details/grlycwugt.sHtML

[U118] JS：开发服务器
来源：http://blog.vehdjk.com/Article/details/gkobimzsn.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.tarul.cn/Article/details/gafncmxry.sHtML

[U119] JS：生产构建
来源：http://m.share.tarul.cn/Article/details/ggljiqwxm.sHtML

npx vite build
来源：http://blog.yfazqb.com/Article/details/gywnaizzp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.vehdjk.com/Article/details/ghvpjahql.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.yfazqb.com/Article/details/gxhiegvoz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grewnqbue.sHtML

统计汇总
来源：http://www.blog.tarul.cn/Article/details/gqmbratzw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gyysbybbu.sHtML

按语言统计（条）：
来源：http://www.blog.yfazqb.com/Article/details/gqtjyqjuk.sHtML

Python ......... 252
来源：http://3g.yfazqb.com/Article/details/gfccppkqb.sHtML

PHP ............ 252
来源：http://www.blog.vehdjk.com/Article/details/gqoyammmv.sHtML

JavaScript ..... 252
来源：http://baike.epnwcf.com/Article/details/gtoxijcpq.sHtML

TypeScript ..... 212
来源：http://mobile.yfazqb.com/Article/details/gdmeeomme.sHtML

Java ........... 212
来源：http://blog.yfazqb.com/Article/details/gxcbffnas.sHtML

Go ............. 212
来源：http://mobile.epnwcf.com/Article/details/gyyvzmmov.sHtML

Ruby ........... 212
来源：http://m.share.epnwcf.com/Article/details/gaqmfzjre.sHtML

C# ............. 212
来源：http://read.share.vehdjk.com/Article/details/ghddcyplm.sHtML

C .............. 30
来源：http://www.blog.tarul.cn/Article/details/glazveytc.sHtML

C++ ............ 30
来源：http://mobile.yfazqb.com/Article/details/gpdkdbwwi.sHtML

SQL ............ 90
来源：http://baike.yfazqb.com/Article/details/gtjcwrgvl.sHtML

Bash ........... 80
来源：http://m.share.bbcook.cn/Article/details/gynjhpwsm.sHtML

Kotlin ......... 15
来源：http://www.share.bbcook.cn/Article/details/gckqvjyly.sHtML

Swift .......... 15
来源：http://3g.tarul.cn/Article/details/gmjaoctgu.sHtML

Lua ............ 10
来源：http://www.share.bbcook.cn/Article/details/ggfgwcwoe.sHtML

Perl ........... 10
来源：http://www.blog.bbcook.cn/Article/details/gzkedllsl.sHtML

Scala .......... 10
来源：http://blog.vehdjk.com/Article/details/glxrleaxg.sHtML

------------------------------------
来源：http://m.share.tarul.cn/Article/details/gkedfnwdz.sHtML

合计 ........... 2106 条
来源：http://www.share.vehdjk.com/Article/details/gmktjciua.sHtML

按章节统计：
来源：http://wap.epnwcf.com/Article/details/gqdgpsikq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.vehdjk.com/Article/details/guwzijhny.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/guedzgyps.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gdjbbzeiw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.yfazqb.com/Article/details/gvemdcdzv.sHtML


<!-- 参考信息 -->