代发 wailian999

[T45] Perl：数组遍历
来源：http://www.m.share.tarul.cn/Article/details/gjuhplxlf.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fktsv.cn/Article/details/giqqmwtfn.sHtML

[T46] Perl：哈希操作
来源：http://wap.tarul.cn/Article/details/gdbwroedl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.bbcook.cn/Article/details/gfkoripwf.sHtML

[T47] Perl：正则捕获
来源：http://m.share.bbcook.cn/Article/details/ghhpeyrkf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.tarul.cn/Article/details/goujvawlz.sHtML

[T48] Perl：正则替换
来源：http://mobile.tarul.cn/Article/details/gapplccni.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.sjlbkw.cn/Article/details/gqzazfahj.sHtML

[T49] Perl：函数
来源：http://blog.bbcook.cn/Article/details/gnebxxsyr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gnvsvhdpg.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gaehnsadt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fktsv.cn/Article/details/gsrqchwvo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.vehdjk.com/Article/details/gevopkdmo.sHtML

[T51] Scala：Hello World
来源：http://wap.bbcook.cn/Article/details/gcsstwpev.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gfimpvzkc.sHtML

[T52] Scala：变量
来源：http://www.blog.bbcook.cn/Article/details/gvqzpsmhi.sHtML

val a = 1;  var b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gamhlhhlg.sHtML

[T53] Scala：字符串插值
来源：http://read.share.tarul.cn/Article/details/gebcvhemb.sHtML

s"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gxcxnptgp.sHtML

[T54] Scala：集合映射
来源：http://www.share.epnwcf.com/Article/details/gqfaziwmh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.bbcook.cn/Article/details/gnuqlqmpe.sHtML

[T55] Scala：集合过滤
来源：http://mobile.vehdjk.com/Article/details/gvjqsdegc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.tarul.cn/Article/details/gwzpetois.sHtML

[T56] Scala：样例类
来源：http://3g.yfazqb.com/Article/details/gefixyqie.sHtML

case class User(name: String, age: Int)
来源：http://wap.tarul.cn/Article/details/ghhlqwzzv.sHtML

[T57] Scala：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gggirlmwu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.bbcook.cn/Article/details/ghvzlyryp.sHtML

[T58] Scala：函数定义
来源：http://mobile.yfazqb.com/Article/details/gcovpslli.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.yfazqb.com/Article/details/gpxdgimtr.sHtML

[T59] Scala：循环
来源：http://www.blog.bbcook.cn/Article/details/gvekqyxsi.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.sjlbkw.cn/Article/details/gjwalcgol.sHtML

[T60] Scala：折叠
来源：http://m.share.bbcook.cn/Article/details/ggxdnhtco.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fktsv.cn/Article/details/gfzitrbwl.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gzvrfwouw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/gfrwvjxtf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gpoqcunvf.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.vehdjk.com/Article/details/gkvclwlqb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.tarul.cn/Article/details/giyjnuyps.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.sjlbkw.cn/Article/details/gtzljrmrx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fktsv.cn/Article/details/gizaknris.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.yfazqb.com/Article/details/gvrfrdrpn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.epnwcf.com/Article/details/gmphbtpel.sHtML

[U04] Py：变量调试打印
来源：http://3g.epnwcf.com/Article/details/gouopxhaf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.yfazqb.com/Article/details/gvhwxpgck.sHtML

[U05] Py：列表去重且保序
来源：http://baike.sjlbkw.cn/Article/details/gpbrhcwqj.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/goyetcbks.sHtML

[U06] Py：合并两个字典
来源：http://mobile.epnwcf.com/Article/details/gyrwdywha.sHtML

{**a, **b}
来源：http://blog.yfazqb.com/Article/details/goofvpash.sHtML

[U07] Py：反转字典键值
来源：http://m.share.vehdjk.com/Article/details/gpdtssxxu.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fktsv.cn/Article/details/gvnlglumi.sHtML

[U08] Py：展平二维列表
来源：http://mobile.tarul.cn/Article/details/gwnmkukun.sHtML

[y for x in nested for y in x]
来源：http://www.share.bbcook.cn/Article/details/grkxkyunz.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fktsv.cn/Article/details/gixffskbg.sHtML

max(d, key=d.get)
来源：http://blog.yfazqb.com/Article/details/gvsrlpupv.sHtML

[U10] Py：按值排序字典
来源：http://blog.tarul.cn/Article/details/glzpuiulp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.vehdjk.com/Article/details/gupracqyf.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fktsv.cn/Article/details/gjdajgsev.sHtML

(x * 2 for x in arr)
来源：http://baike.yfazqb.com/Article/details/gfmczmjit.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.epnwcf.com/Article/details/gwtnhomqw.sHtML

Counter(arr).most_common(3)
来源：http://m.share.vehdjk.com/Article/details/grofxclwd.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.epnwcf.com/Article/details/gedfxznlt.sHtML

deque(maxlen=10)
来源：http://www.share.bbcook.cn/Article/details/gjruxfjso.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.tarul.cn/Article/details/gtliqukos.sHtML

defaultdict(list)
来源：http://wap.fktsv.cn/Article/details/ghmywtxog.sHtML

[U15] Py：高精度计时
来源：http://blog.tarul.cn/Article/details/gtnktilwz.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/guoawhugp.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fktsv.cn/Article/details/gwzqabgzz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fktsv.cn/Article/details/gcyeqxjui.sHtML

[U17] Py：初始化日志
来源：http://baike.tarul.cn/Article/details/groylvrsu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.yfazqb.com/Article/details/gkrtmgmkj.sHtML

[U18] Py：预编译正则
来源：http://read.share.vehdjk.com/Article/details/grfdbyhci.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.sjlbkw.cn/Article/details/ggmsoraaj.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.epnwcf.com/Article/details/ghwrznlpu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.tarul.cn/Article/details/grupmaxxs.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fktsv.cn/Article/details/glnxqmfwj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.tarul.cn/Article/details/gvlzdlrcc.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fktsv.cn/Article/details/glzpbvcxp.sHtML

@contextlib.contextmanager
来源：http://read.share.yfazqb.com/Article/details/gbamdjdug.sHtML

[U22] Py：矩阵转置
来源：http://3g.bbcook.cn/Article/details/gnwqqhcvq.sHtML

list(zip(*m))
来源：http://mobile.bbcook.cn/Article/details/gkfzcgfca.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.tarul.cn/Article/details/gemjshoon.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.epnwcf.com/Article/details/ganceiqnt.sHtML

[U24] Py：路径操作
来源：http://www.share.sjlbkw.cn/Article/details/gsvnaxbvo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gbhrohofq.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.bbcook.cn/Article/details/gbqkyoarc.sHtML

csv.DictReader(f)
来源：http://baike.fktsv.cn/Article/details/ghqmxrwnq.sHtML

[U26] Py：并发下载
来源：http://www.share.vehdjk.com/Article/details/gpmretuvm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.bbcook.cn/Article/details/gnkozkspz.sHtML

[U27] Py：异步 HTTP
来源：http://wap.tarul.cn/Article/details/gnjxejwms.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fktsv.cn/Article/details/gegtmjuaj.sHtML

[U28] Py：类型别名
来源：http://read.share.vehdjk.com/Article/details/gskzzsoad.sHtML

UserId = int
来源：http://www.blog.vehdjk.com/Article/details/gtgqzxovo.sHtML

[U29] Py：属性校验
来源：http://baike.sjlbkw.cn/Article/details/gznpwdgun.sHtML

@property 与 @x.setter 配合
来源：http://read.share.sjlbkw.cn/Article/details/gspcbguky.sHtML

[U30] Py：数据类
来源：http://wap.bbcook.cn/Article/details/gkowjkdyk.sHtML

@dataclass(slots=True)
来源：http://m.share.fktsv.cn/Article/details/gpndmqttf.sHtML

[U31] Py：单测
来源：http://m.share.fktsv.cn/Article/details/gibnqqukn.sHtML

python -m pytest -q
来源：http://3g.tarul.cn/Article/details/gahzfjrcz.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.epnwcf.com/Article/details/gweykrnlt.sHtML

ruff format . && ruff check --fix .
来源：http://wap.vehdjk.com/Article/details/ghmqmaqlq.sHtML

[U33] Py：打包发布
来源：http://www.blog.vehdjk.com/Article/details/ghbzdkbsm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.epnwcf.com/Article/details/gcpixvqov.sHtML

[U34] Py：判断编码
来源：http://mobile.fktsv.cn/Article/details/ghfqescps.sHtML

chardet.detect(raw)
来源：http://www.share.tarul.cn/Article/details/gaqugnidh.sHtML

[U35] Py：发送邮件
来源：http://3g.vehdjk.com/Article/details/gdcdsfobb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.epnwcf.com/Article/details/glqsjgxpg.sHtML

[U36] Py：定时任务
来源：http://wap.sjlbkw.cn/Article/details/gstrvthpu.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.tarul.cn/Article/details/ghoxbhydc.sHtML

[U37] Py：读写 Excel
来源：http://blog.epnwcf.com/Article/details/gjlmrwlnd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.sjlbkw.cn/Article/details/gemygmtdm.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.tarul.cn/Article/details/gfdelxyki.sHtML

Path(__file__).resolve().parent
来源：http://www.share.yfazqb.com/Article/details/ggnqexhfv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.yfazqb.com/Article/details/grsffzrfm.sHtML

sys.stdout.isatty()
来源：http://wap.sjlbkw.cn/Article/details/gvubxqtnk.sHtML

[U40] Py：打印到标准错误
来源：http://wap.vehdjk.com/Article/details/ghxztmfiy.sHtML

print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/grmkdhmvf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fktsv.cn/Article/details/gerrjksyx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.vehdjk.com/Article/details/gjrdodnnf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.epnwcf.com/Article/details/gjjmfzjgg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.sjlbkw.cn/Article/details/gvdrfqogz.sHtML

[U43] PHP：声明命名空间
来源：http://wap.sjlbkw.cn/Article/details/gthuyikab.sHtML

namespace App\Http;
来源：http://read.share.sjlbkw.cn/Article/details/giqumrnps.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fktsv.cn/Article/details/guoarxqox.sHtML

declare(strict_types=1);
来源：http://3g.sjlbkw.cn/Article/details/gzizjpilh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.yfazqb.com/Article/details/glufivhto.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gdxnqgpzx.sHtML

[U46] PHP：可空类型
来源：http://m.share.yfazqb.com/Article/details/grrazgcqj.sHtML

?string $name = null
来源：http://www.blog.yfazqb.com/Article/details/gnizydnqt.sHtML

[U47] PHP：联合类型
来源：http://wap.sjlbkw.cn/Article/details/glmuzhuxy.sHtML

int|string $id
来源：http://baike.epnwcf.com/Article/details/gmklbnamz.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fktsv.cn/Article/details/gzatevhue.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.bbcook.cn/Article/details/glxlcgtzm.sHtML

[U49] PHP：只读属性
来源：http://read.share.vehdjk.com/Article/details/gargrdbvy.sHtML

public readonly string $name
来源：http://read.share.tarul.cn/Article/details/gaalebyer.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.vehdjk.com/Article/details/gyklnrfbx.sHtML

public function __construct(private int $id) {}
来源：http://www.share.bbcook.cn/Article/details/gnrqxkwdz.sHtML

[U51] PHP：数组解构
来源：http://www.share.epnwcf.com/Article/details/gbbkldfpw.sHtML

[$a, $b] = $arr;
来源：http://m.share.yfazqb.com/Article/details/guorzqsqz.sHtML

[U52] PHP：箭头函数
来源：http://www.share.epnwcf.com/Article/details/gvcdkoekh.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.bbcook.cn/Article/details/gnvznqbqh.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.tarul.cn/Article/details/goepkvhea.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.vehdjk.com/Article/details/gkrxhogle.sHtML

[U54] PHP：空安全调用
来源：http://m.share.vehdjk.com/Article/details/ggiznfldh.sHtML

$obj?->method()
来源：http://read.share.yfazqb.com/Article/details/gjkstwxtb.sHtML

[U55] PHP：match 表达式
来源：http://blog.sjlbkw.cn/Article/details/gkzrzhqrd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.tarul.cn/Article/details/gevvqqsoe.sHtML

[U56] PHP：命名参数
来源：http://www.share.tarul.cn/Article/details/gptxvjfkd.sHtML

f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gnziejylu.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gvssvurcm.sHtML

"值: {$a}"
来源：http://3g.fktsv.cn/Article/details/gyxriuavl.sHtML

[U58] PHP：数组三件套
来源：http://baike.tarul.cn/Article/details/gtzilhasb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.yfazqb.com/Article/details/giozepxli.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.bbcook.cn/Article/details/gzacxxrrd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.sjlbkw.cn/Article/details/gyeimolzx.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.bbcook.cn/Article/details/ghqzwczkx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.yfazqb.com/Article/details/gpsoouzso.sHtML

[U61] PHP：正则
来源：http://read.share.vehdjk.com/Article/details/gbjecpnog.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gjjviwgoz.sHtML

[U62] PHP：日期对象
来源：http://m.share.bbcook.cn/Article/details/gdbotwxre.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.epnwcf.com/Article/details/geobcptky.sHtML

[U63] PHP：文件读写
来源：http://read.share.yfazqb.com/Article/details/gfbjxeigf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.vehdjk.com/Article/details/gumixnjrz.sHtML

[U64] PHP：目录遍历
来源：http://www.share.bbcook.cn/Article/details/glvsltwwi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.vehdjk.com/Article/details/gzidvjywr.sHtML

[U65] PHP：会话
来源：http://read.share.fktsv.cn/Article/details/gaibgxynk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.tarul.cn/Article/details/gmmuloqyp.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fktsv.cn/Article/details/gheaahdne.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gmbsqzqdx.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fktsv.cn/Article/details/gpgmmlmhq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fktsv.cn/Article/details/gaqxlgcfg.sHtML

[U68] PHP：PDO 连接
来源：http://wap.yfazqb.com/Article/details/gwtrefxxk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.vehdjk.com/Article/details/gdhmvzvrd.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fktsv.cn/Article/details/gxykouqfx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.bbcook.cn/Article/details/gshuzcbwl.sHtML

[U70] PHP：PDO 事务
来源：http://3g.tarul.cn/Article/details/gxwltdhbq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.sjlbkw.cn/Article/details/ggseqjfci.sHtML

[U71] PHP：抛出异常
来源：http://blog.tarul.cn/Article/details/gqxuqkcpq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gwwuqspel.sHtML

[U72] PHP：写错误日志
来源：http://mobile.bbcook.cn/Article/details/ghjlpuuwx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.epnwcf.com/Article/details/gbouhccdf.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.epnwcf.com/Article/details/gsukfsagv.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.sjlbkw.cn/Article/details/gahefwlmp.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gyayfjykn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.yfazqb.com/Article/details/gxcuxjvzz.sHtML

[U75] PHP：依赖注入
来源：http://mobile.yfazqb.com/Article/details/gmqqezavc.sHtML

composer require psr/container
来源：http://www.blog.tarul.cn/Article/details/guqsosztu.sHtML

[U76] PHP：简单路由
来源：http://mobile.yfazqb.com/Article/details/gvyttalua.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.yfazqb.com/Article/details/gjiaenklh.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpuqjwlz.sHtML

composer require twig/twig
来源：http://www.m.share.yfazqb.com/Article/details/gipavwopx.sHtML

[U78] PHP：单元测试
来源：http://read.share.fktsv.cn/Article/details/goefayjih.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.vehdjk.com/Article/details/gkxkbeadk.sHtML

[U79] PHP：静态分析
来源：http://www.share.tarul.cn/Article/details/gnbmljzuh.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.bbcook.cn/Article/details/giqanhlya.sHtML

[U80] PHP：代码规范修复
来源：http://wap.bbcook.cn/Article/details/gxduxlrpz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.yfazqb.com/Article/details/gkveuxqdu.sHtML

[U81] JS：初始化项目
来源：http://mobile.vehdjk.com/Article/details/gkdigjpsm.sHtML

npm init -y;  npm i express
来源：http://mobile.fktsv.cn/Article/details/gduazfhrn.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.bbcook.cn/Article/details/ghusgmgeo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.bbcook.cn/Article/details/gkokjnffh.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.yfazqb.com/Article/details/gsswztyat.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.tarul.cn/Article/details/gcmymkito.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.sjlbkw.cn/Article/details/gmjogbnig.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.tarul.cn/Article/details/guatralnt.sHtML

[U85] JS：可选链
来源：http://wap.yfazqb.com/Article/details/gepylwnxh.sHtML

a?.b?.c
来源：http://read.share.bbcook.cn/Article/details/gcckmwbyl.sHtML

[U86] JS：空值合并
来源：http://3g.epnwcf.com/Article/details/gxltmrvtz.sHtML

a ?? b
来源：http://mobile.fktsv.cn/Article/details/gspjgfafn.sHtML

[U87] JS：解构默认值
来源：http://m.share.bbcook.cn/Article/details/grwkmoknf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.tarul.cn/Article/details/ghifigwxm.sHtML

[U88] JS：对象展开合并
来源：http://mobile.yfazqb.com/Article/details/gsbkkmbis.sHtML

{ ...a, ...b }
来源：http://www.share.epnwcf.com/Article/details/gmkyxbijh.sHtML

[U89] JS：数组去重
来源：http://www.blog.yfazqb.com/Article/details/gwireyoza.sHtML

[...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gscyuxrea.sHtML

[U90] JS：数字数组排序
来源：http://mobile.epnwcf.com/Article/details/gzaczkuzv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/gajmkjcak.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.yfazqb.com/Article/details/gixryyopq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.vehdjk.com/Article/details/golmfiuqy.sHtML

[U92] JS：深拷贝
来源：http://www.share.tarul.cn/Article/details/gofwvprzb.sHtML

structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gvyysjpad.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.yfazqb.com/Article/details/guzplhxny.sHtML

`共 ${n} 条`
来源：http://read.share.vehdjk.com/Article/details/gtevhpvjr.sHtML

[U94] JS：箭头函数
来源：http://baike.epnwcf.com/Article/details/gjvjxgmle.sHtML

const double = x => x * 2;
来源：http://www.share.epnwcf.com/Article/details/gvkjfmtqa.sHtML

[U95] JS：Promise 包装
来源：http://3g.bbcook.cn/Article/details/gkoruqplk.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.yfazqb.com/Article/details/gwfqmssnf.sHtML

[U96] JS：async/await 与异常
来源：http://blog.epnwcf.com/Article/details/gquzpxrii.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gpkwrqprn.sHtML

[U97] JS：并发请求
来源：http://read.share.sjlbkw.cn/Article/details/ggxbfhcnm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gvzntfloq.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fktsv.cn/Article/details/gkwkyhxss.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.epnwcf.com/Article/details/ghewtjczl.sHtML

[U99] JS：事件监听
来源：http://wap.vehdjk.com/Article/details/gooqjbrgx.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.vehdjk.com/Article/details/grbfqfias.sHtML

[U100] JS：DOM 查询
来源：http://www.share.tarul.cn/Article/details/gzloeymse.sHtML

document.querySelector(".item")
来源：http://wap.bbcook.cn/Article/details/gxpaedqjx.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fktsv.cn/Article/details/ggincdxef.sHtML

el.classList.toggle("active")
来源：http://3g.tarul.cn/Article/details/gyzruvpgb.sHtML

[U102] JS：本地存储
来源：http://read.share.yfazqb.com/Article/details/gbrynjuty.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.tarul.cn/Article/details/gpuaykofm.sHtML

[U103] JS：定时器
来源：http://www.share.tarul.cn/Article/details/gecskhffv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.epnwcf.com/Article/details/gtaeyuity.sHtML

[U104] JS：防抖
来源：http://m.share.yfazqb.com/Article/details/ggdbucxml.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/ggcjksrhb.sHtML

[U105] JS：节流
来源：http://read.share.vehdjk.com/Article/details/gvuinzrpb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fktsv.cn/Article/details/gunupxzqs.sHtML

[U106] JS：日期格式化
来源：http://baike.epnwcf.com/Article/details/gzurwwiic.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.bbcook.cn/Article/details/gpyzdehxu.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.vehdjk.com/Article/details/ghytvwjzq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.epnwcf.com/Article/details/gcimphszs.sHtML

[U108] JS：随机整数
来源：http://mobile.sjlbkw.cn/Article/details/gzxhtgrzr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.epnwcf.com/Article/details/gqusmalsr.sHtML

[U109] JS：数组分组
来源：http://3g.vehdjk.com/Article/details/gejrijvww.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/gyokxplyx.sHtML

[U110] JS：数组分块
来源：http://mobile.epnwcf.com/Article/details/gaxftviuh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.tarul.cn/Article/details/gjocnsnla.sHtML

[U111] JS：对象转 Map
来源：http://m.share.bbcook.cn/Article/details/gshdcnccw.sHtML

new Map(Object.entries(obj))
来源：http://3g.sjlbkw.cn/Article/details/gshpobgmx.sHtML

[U112] JS：字符串补位
来源：http://www.share.yfazqb.com/Article/details/grbqbydcv.sHtML

"7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gkfuahykp.sHtML

[U113] JS：正则替换全部
来源：http://3g.fktsv.cn/Article/details/gwogsdhnl.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gwqqzfydl.sHtML

[U114] JS：JSON 深比较
来源：http://blog.tarul.cn/Article/details/gtoutyfln.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gxoesuoxl.sHtML

[U115] JS：生成 UUID
来源：http://m.share.epnwcf.com/Article/details/gjedijdbd.sHtML

crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gyqpditva.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.vehdjk.com/Article/details/gcucjoscc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.bbcook.cn/Article/details/gqbzaskll.sHtML

[U117] JS：单元测试
来源：http://blog.fktsv.cn/Article/details/gfuykhvyg.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.epnwcf.com/Article/details/gqlnwmiwz.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgtsgdav.sHtML

npm i -D vite;  npx vite
来源：http://baike.bbcook.cn/Article/details/grqtiuoqy.sHtML

[U119] JS：生产构建
来源：http://blog.tarul.cn/Article/details/gyxahkxcl.sHtML

npx vite build
来源：http://m.share.vehdjk.com/Article/details/gwgtkqmjw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.tarul.cn/Article/details/gwinhydht.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fktsv.cn/Article/details/gbmrixswv.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gzadpbcrb.sHtML

统计汇总
来源：http://www.m.share.fktsv.cn/Article/details/gdnhmobfg.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkaamebdt.sHtML

按语言统计（条）：
来源：http://www.blog.tarul.cn/Article/details/gbkmzbecx.sHtML

Python ......... 252
来源：http://mobile.epnwcf.com/Article/details/gzhnqqnbd.sHtML

PHP ............ 252
来源：http://baike.epnwcf.com/Article/details/guuzdyaey.sHtML

JavaScript ..... 252
来源：http://read.share.sjlbkw.cn/Article/details/govpmbtkc.sHtML

TypeScript ..... 212
来源：http://www.share.vehdjk.com/Article/details/gmbmvvobn.sHtML

Java ........... 212
来源：http://blog.epnwcf.com/Article/details/gtrlbimqv.sHtML

Go ............. 212
来源：http://mobile.epnwcf.com/Article/details/gbyeatgzq.sHtML

Ruby ........... 212
来源：http://baike.yfazqb.com/Article/details/gytvlnfll.sHtML

C# ............. 212
来源：http://blog.vehdjk.com/Article/details/gidyvlgpt.sHtML

C .............. 30
来源：http://blog.sjlbkw.cn/Article/details/gubcqpash.sHtML

C++ ............ 30
来源：http://www.share.fktsv.cn/Article/details/gdfhsgpsl.sHtML

SQL ............ 90
来源：http://baike.vehdjk.com/Article/details/gwcrpcyhd.sHtML

Bash ........... 80
来源：http://3g.vehdjk.com/Article/details/gwmksrhqu.sHtML

Kotlin ......... 15
来源：http://www.m.share.tarul.cn/Article/details/gkheplqfc.sHtML

Swift .......... 15
来源：http://wap.fktsv.cn/Article/details/gibspbfrr.sHtML

Lua ............ 10
来源：http://blog.bbcook.cn/Article/details/gkjjfmbcq.sHtML

Perl ........... 10
来源：http://m.share.fktsv.cn/Article/details/giekhbeeb.sHtML

Scala .......... 10
来源：http://read.share.tarul.cn/Article/details/gntuzznye.sHtML

------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaerogjs.sHtML

合计 ........... 2106 条
来源：http://www.blog.tarul.cn/Article/details/gmbqzidne.sHtML

按章节统计：
来源：http://www.share.fktsv.cn/Article/details/gcenivnut.sHtML


<!-- 参考信息 -->