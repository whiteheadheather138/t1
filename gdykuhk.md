代发 wailian999

[T41] Perl：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gaxkxtttl.sHtML

print "Hello\n";
来源：http://3g.sjlbkw.cn/Article/details/gtgkcrjks.sHtML

[T42] Perl：变量类型
来源：http://read.share.tarul.cn/Article/details/goqxbicqj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.yfazqb.com/Article/details/gikhjprum.sHtML

[T43] Perl：字符串插值
来源：http://wap.bbcook.cn/Article/details/gdxazpbdi.sHtML

"值: $a"
来源：http://blog.yfazqb.com/Article/details/gjfrviewu.sHtML

[T44] Perl：条件
来源：http://mobile.tarul.cn/Article/details/ggcajlekl.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.vehdjk.com/Article/details/gosdhvbsr.sHtML

[T45] Perl：数组遍历
来源：http://baike.epnwcf.com/Article/details/gknsbhejx.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.tarul.cn/Article/details/gtajmjwua.sHtML

[T46] Perl：哈希操作
来源：http://wap.tarul.cn/Article/details/gcrtaaoyh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.vehdjk.com/Article/details/gngqtbyqf.sHtML

[T47] Perl：正则捕获
来源：http://mobile.vehdjk.com/Article/details/gdnltixuv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.sjlbkw.cn/Article/details/gsfbbahzi.sHtML

[T48] Perl：正则替换
来源：http://www.share.tarul.cn/Article/details/gegbdivlt.sHtML

$s =~ s/old/new/g;
来源：http://baike.sjlbkw.cn/Article/details/glseuotiq.sHtML

[T49] Perl：函数
来源：http://blog.epnwcf.com/Article/details/gzmnhfwbs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/grmxgzxkp.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gnsetgytw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.sjlbkw.cn/Article/details/gaxtydjjn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.yfazqb.com/Article/details/gwwkrgljh.sHtML

[T51] Scala：Hello World
来源：http://m.share.fktsv.cn/Article/details/gqjxhrztm.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gvdcndpqr.sHtML

[T52] Scala：变量
来源：http://wap.vehdjk.com/Article/details/ggoxegpwv.sHtML

val a = 1;  var b = 2
来源：http://m.share.epnwcf.com/Article/details/gotezaemz.sHtML

[T53] Scala：字符串插值
来源：http://3g.tarul.cn/Article/details/gqjffuyfl.sHtML

s"值: $b"
来源：http://www.share.epnwcf.com/Article/details/glpnjcrrd.sHtML

[T54] Scala：集合映射
来源：http://read.share.vehdjk.com/Article/details/gtnrimpoa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gqibgdhgh.sHtML

[T55] Scala：集合过滤
来源：http://www.share.vehdjk.com/Article/details/grzlikmxc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.bbcook.cn/Article/details/gnumyrejr.sHtML

[T56] Scala：样例类
来源：http://read.share.yfazqb.com/Article/details/gsszeybpy.sHtML

case class User(name: String, age: Int)
来源：http://3g.fktsv.cn/Article/details/gduqgnffb.sHtML

[T57] Scala：模式匹配
来源：http://blog.vehdjk.com/Article/details/gmfwlbcfh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.yfazqb.com/Article/details/giiomrmpg.sHtML

[T58] Scala：函数定义
来源：http://www.share.yfazqb.com/Article/details/grqtxljyg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.vehdjk.com/Article/details/gihshezdu.sHtML

[T59] Scala：循环
来源：http://www.share.sjlbkw.cn/Article/details/gqdhaxags.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.vehdjk.com/Article/details/giujjwosj.sHtML

[T60] Scala：折叠
来源：http://3g.tarul.cn/Article/details/geybgbfgc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fktsv.cn/Article/details/gtyruhuwq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjwplturi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/goazimvfo.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gaqgpwefo.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.yfazqb.com/Article/details/gjczlmvzv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fktsv.cn/Article/details/gwhyxbtul.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fktsv.cn/Article/details/gvjznqait.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.bbcook.cn/Article/details/gqqkxdkur.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.yfazqb.com/Article/details/gxznvgsno.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.yfazqb.com/Article/details/gmgdzjrbb.sHtML

[U04] Py：变量调试打印
来源：http://baike.vehdjk.com/Article/details/gthomuhow.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fktsv.cn/Article/details/gxmtviywp.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.bbcook.cn/Article/details/gunwtizjx.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/gfietijpt.sHtML

[U06] Py：合并两个字典
来源：http://m.share.yfazqb.com/Article/details/gmppnubvi.sHtML

{**a, **b}
来源：http://mobile.bbcook.cn/Article/details/gfkrejgol.sHtML

[U07] Py：反转字典键值
来源：http://www.share.sjlbkw.cn/Article/details/gsemrdobv.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gojdhjhxh.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbgyxviv.sHtML

[y for x in nested for y in x]
来源：http://m.share.yfazqb.com/Article/details/gbpxqxrik.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fktsv.cn/Article/details/garfaudaf.sHtML

max(d, key=d.get)
来源：http://read.share.fktsv.cn/Article/details/gttdmdrja.sHtML

[U10] Py：按值排序字典
来源：http://read.share.tarul.cn/Article/details/gtfknqrsh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.yfazqb.com/Article/details/glwnmlgfe.sHtML

[U11] Py：生成器表达式
来源：http://mobile.epnwcf.com/Article/details/gadnjhvxm.sHtML

(x * 2 for x in arr)
来源：http://3g.yfazqb.com/Article/details/gsjjitfle.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.bbcook.cn/Article/details/gxlenyakg.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.bbcook.cn/Article/details/gvvoquvpp.sHtML

[U13] Py：固定长度队列
来源：http://www.share.epnwcf.com/Article/details/gbykzzauy.sHtML

deque(maxlen=10)
来源：http://www.share.vehdjk.com/Article/details/gvycchgfq.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.epnwcf.com/Article/details/gpymbcxnq.sHtML

defaultdict(list)
来源：http://m.share.yfazqb.com/Article/details/gguwcqfls.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.yfazqb.com/Article/details/gfjacnjxm.sHtML

t = time.perf_counter()
来源：http://www.share.vehdjk.com/Article/details/gwyzztetz.sHtML

[U16] Py：命令行参数解析
来源：http://3g.tarul.cn/Article/details/gkiutypel.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.sjlbkw.cn/Article/details/gxkajkher.sHtML

[U17] Py：初始化日志
来源：http://baike.tarul.cn/Article/details/gxahjnftp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.sjlbkw.cn/Article/details/gpawlpxnn.sHtML

[U18] Py：预编译正则
来源：http://www.share.vehdjk.com/Article/details/gklfyqzkf.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.tarul.cn/Article/details/gutdycydl.sHtML

[U19] Py：正则替换带回调
来源：http://baike.sjlbkw.cn/Article/details/gowplkkgi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.epnwcf.com/Article/details/gpploiagv.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.sjlbkw.cn/Article/details/gznxfjcga.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.tarul.cn/Article/details/gmccqpniq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.bbcook.cn/Article/details/gnbhywkpq.sHtML

@contextlib.contextmanager
来源：http://mobile.tarul.cn/Article/details/ghzfamzoa.sHtML

[U22] Py：矩阵转置
来源：http://read.share.yfazqb.com/Article/details/gndgyvdsp.sHtML

list(zip(*m))
来源：http://www.share.sjlbkw.cn/Article/details/gsztknurq.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.sjlbkw.cn/Article/details/gstprngle.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.epnwcf.com/Article/details/gtcdhbwqu.sHtML

[U24] Py：路径操作
来源：http://3g.fktsv.cn/Article/details/gulfxglpp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gwvqnusjw.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fktsv.cn/Article/details/gdiyosesn.sHtML

csv.DictReader(f)
来源：http://3g.tarul.cn/Article/details/glilhihyh.sHtML

[U26] Py：并发下载
来源：http://read.share.epnwcf.com/Article/details/gnmnooxyq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.epnwcf.com/Article/details/gvbvpypuy.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.vehdjk.com/Article/details/gokcosvgy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.vehdjk.com/Article/details/gijsxnfrl.sHtML

[U28] Py：类型别名
来源：http://read.share.vehdjk.com/Article/details/gaksissrn.sHtML

UserId = int
来源：http://www.blog.tarul.cn/Article/details/geczkombn.sHtML

[U29] Py：属性校验
来源：http://wap.bbcook.cn/Article/details/gvfbiywit.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fktsv.cn/Article/details/gqydgkvfi.sHtML

[U30] Py：数据类
来源：http://www.m.share.bbcook.cn/Article/details/gbkwpuyks.sHtML

@dataclass(slots=True)
来源：http://wap.sjlbkw.cn/Article/details/gulevpevw.sHtML

[U31] Py：单测
来源：http://3g.tarul.cn/Article/details/gyxunukxe.sHtML

python -m pytest -q
来源：http://www.m.share.fktsv.cn/Article/details/ggekvemer.sHtML

[U32] Py：代码格式化
来源：http://www.blog.vehdjk.com/Article/details/gtewlezkv.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fktsv.cn/Article/details/gffqjlnaa.sHtML

[U33] Py：打包发布
来源：http://m.share.epnwcf.com/Article/details/gwmvcylve.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.epnwcf.com/Article/details/gjuhitldr.sHtML

[U34] Py：判断编码
来源：http://baike.bbcook.cn/Article/details/ghbhdcjbq.sHtML

chardet.detect(raw)
来源：http://baike.epnwcf.com/Article/details/gcczrfrwa.sHtML

[U35] Py：发送邮件
来源：http://read.share.fktsv.cn/Article/details/ggspvoelz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.vehdjk.com/Article/details/gawzptkkf.sHtML

[U36] Py：定时任务
来源：http://www.share.epnwcf.com/Article/details/gkofqzerz.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.epnwcf.com/Article/details/guiuzcvac.sHtML

[U37] Py：读写 Excel
来源：http://baike.fktsv.cn/Article/details/gtabfcirp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.sjlbkw.cn/Article/details/gwrlozecn.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fktsv.cn/Article/details/gylpljmsl.sHtML

Path(__file__).resolve().parent
来源：http://mobile.bbcook.cn/Article/details/gezhktnqt.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.yfazqb.com/Article/details/gntxshjgw.sHtML

sys.stdout.isatty()
来源：http://mobile.yfazqb.com/Article/details/gmzpxtdgo.sHtML

[U40] Py：打印到标准错误
来源：http://blog.epnwcf.com/Article/details/ghsupzmgd.sHtML

print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gqemfjqez.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.bbcook.cn/Article/details/godygrqax.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.sjlbkw.cn/Article/details/gprlgwwan.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fktsv.cn/Article/details/gtlyjtcei.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.vehdjk.com/Article/details/gdkiymdol.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwdtxarx.sHtML

namespace App\Http;
来源：http://mobile.tarul.cn/Article/details/gkjilmlhs.sHtML

[U44] PHP：开启严格类型
来源：http://wap.sjlbkw.cn/Article/details/gzavasfre.sHtML

declare(strict_types=1);
来源：http://read.share.vehdjk.com/Article/details/geyytcjhm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fktsv.cn/Article/details/gwawuiioe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gbhqehrtt.sHtML

[U46] PHP：可空类型
来源：http://read.share.tarul.cn/Article/details/gexqoqntz.sHtML

?string $name = null
来源：http://mobile.yfazqb.com/Article/details/gdshipqii.sHtML

[U47] PHP：联合类型
来源：http://3g.fktsv.cn/Article/details/gzmjzdeyh.sHtML

int|string $id
来源：http://www.blog.bbcook.cn/Article/details/goomxdppb.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fktsv.cn/Article/details/gbtzzjfvp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.sjlbkw.cn/Article/details/gyiwfhqae.sHtML

[U49] PHP：只读属性
来源：http://wap.bbcook.cn/Article/details/gsmnnldyg.sHtML

public readonly string $name
来源：http://read.share.fktsv.cn/Article/details/gmlwhfxkr.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fktsv.cn/Article/details/ghbvviamx.sHtML

public function __construct(private int $id) {}
来源：http://blog.yfazqb.com/Article/details/glzerlyyp.sHtML

[U51] PHP：数组解构
来源：http://m.share.yfazqb.com/Article/details/gxbdntmlh.sHtML

[$a, $b] = $arr;
来源：http://www.share.fktsv.cn/Article/details/gwhmadzpp.sHtML

[U52] PHP：箭头函数
来源：http://3g.vehdjk.com/Article/details/ghpmpdgic.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.epnwcf.com/Article/details/gtjcsxrnr.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.sjlbkw.cn/Article/details/gbszaxxck.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.sjlbkw.cn/Article/details/gfywdebdw.sHtML

[U54] PHP：空安全调用
来源：http://3g.bbcook.cn/Article/details/glmdvksdq.sHtML

$obj?->method()
来源：http://baike.vehdjk.com/Article/details/gpokysekm.sHtML

[U55] PHP：match 表达式
来源：http://mobile.epnwcf.com/Article/details/gvadspuqp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnazmkvn.sHtML

[U56] PHP：命名参数
来源：http://www.blog.tarul.cn/Article/details/gwtuwypxh.sHtML

f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gvlgkeaza.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gioakihhb.sHtML

"值: {$a}"
来源：http://mobile.bbcook.cn/Article/details/gistcxkpe.sHtML

[U58] PHP：数组三件套
来源：http://3g.epnwcf.com/Article/details/gvtbjsrhc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gdjtvjsuz.sHtML

[U59] PHP：自定义排序
来源：http://mobile.bbcook.cn/Article/details/gbcnnaqri.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gksbuwfnh.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.tarul.cn/Article/details/gcsrfgjbo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.yfazqb.com/Article/details/gdsdqvtjk.sHtML

[U61] PHP：正则
来源：http://wap.fktsv.cn/Article/details/gndhoixqh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gstqctwhm.sHtML

[U62] PHP：日期对象
来源：http://read.share.sjlbkw.cn/Article/details/gjsnztxub.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.vehdjk.com/Article/details/garfdcxhb.sHtML

[U63] PHP：文件读写
来源：http://blog.sjlbkw.cn/Article/details/giskokugl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.bbcook.cn/Article/details/gaxuaodbi.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fktsv.cn/Article/details/gtfyhjddz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.tarul.cn/Article/details/gxjtfcgey.sHtML

[U65] PHP：会话
来源：http://m.share.tarul.cn/Article/details/gmbweikfr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gtbaxvqdw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.vehdjk.com/Article/details/gzsavxrmk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fktsv.cn/Article/details/gufevfrzq.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.yfazqb.com/Article/details/gbvjvcfen.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.bbcook.cn/Article/details/gqswirwbu.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.epnwcf.com/Article/details/ggtgoeruo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.vehdjk.com/Article/details/ghnoeckqz.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.sjlbkw.cn/Article/details/gflmtoobs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.tarul.cn/Article/details/gaybybnuz.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.bbcook.cn/Article/details/gchdzlflo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.tarul.cn/Article/details/gtyiorfoo.sHtML

[U71] PHP：抛出异常
来源：http://read.share.epnwcf.com/Article/details/gognnmhyd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/gxidhuksv.sHtML

[U72] PHP：写错误日志
来源：http://www.share.vehdjk.com/Article/details/gwzvncxhj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.tarul.cn/Article/details/gbvbgttxv.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.epnwcf.com/Article/details/guaksxiqk.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.epnwcf.com/Article/details/gwkgcphov.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.bbcook.cn/Article/details/gjcmpdysy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.bbcook.cn/Article/details/gjfnmtjbm.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fktsv.cn/Article/details/gcgulqwle.sHtML

composer require psr/container
来源：http://www.m.share.sjlbkw.cn/Article/details/groozvsty.sHtML

[U76] PHP：简单路由
来源：http://www.share.yfazqb.com/Article/details/gixkbsjth.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.bbcook.cn/Article/details/gezkxdtnr.sHtML

[U77] PHP：模板渲染
来源：http://baike.vehdjk.com/Article/details/gxavrtbjs.sHtML

composer require twig/twig
来源：http://www.share.epnwcf.com/Article/details/gnoogzldi.sHtML

[U78] PHP：单元测试
来源：http://blog.tarul.cn/Article/details/gxxcmakwk.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.sjlbkw.cn/Article/details/gutqxcsbe.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.bbcook.cn/Article/details/gpaoimoqy.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.vehdjk.com/Article/details/gfjnbsffq.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.tarul.cn/Article/details/gcjqzgfhn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.bbcook.cn/Article/details/gcmykipfa.sHtML

[U81] JS：初始化项目
来源：http://wap.vehdjk.com/Article/details/ghfcqlhgg.sHtML

npm init -y;  npm i express
来源：http://www.blog.bbcook.cn/Article/details/glulnmmwb.sHtML

[U82] JS：package.json 脚本
来源：http://3g.vehdjk.com/Article/details/gktzwpvyr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.tarul.cn/Article/details/gdlpxexvg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.yfazqb.com/Article/details/glolgsmzq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.sjlbkw.cn/Article/details/gbkiymopp.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.vehdjk.com/Article/details/gqkrmondo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fktsv.cn/Article/details/gcclrssnp.sHtML

[U85] JS：可选链
来源：http://m.share.fktsv.cn/Article/details/gvpgkphbz.sHtML

a?.b?.c
来源：http://baike.vehdjk.com/Article/details/gtiiaiezv.sHtML

[U86] JS：空值合并
来源：http://wap.epnwcf.com/Article/details/gdtwjgmdc.sHtML

a ?? b
来源：http://mobile.yfazqb.com/Article/details/gvmkabbbm.sHtML

[U87] JS：解构默认值
来源：http://baike.epnwcf.com/Article/details/gafoifgev.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.vehdjk.com/Article/details/gexeftsog.sHtML

[U88] JS：对象展开合并
来源：http://m.share.epnwcf.com/Article/details/gqjsvehnw.sHtML

{ ...a, ...b }
来源：http://read.share.vehdjk.com/Article/details/gpyzoyvog.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fktsv.cn/Article/details/gpvfraway.sHtML

[...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/ghxuhcvzk.sHtML

[U90] JS：数字数组排序
来源：http://baike.fktsv.cn/Article/details/geynmuwqj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gelvunxsm.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.yfazqb.com/Article/details/gevsqztfp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.epnwcf.com/Article/details/gyfvcbvjy.sHtML

[U92] JS：深拷贝
来源：http://baike.yfazqb.com/Article/details/gcuahfcqk.sHtML

structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gfcrooldy.sHtML

[U93] JS：模板字符串
来源：http://www.share.fktsv.cn/Article/details/gvzunpnqq.sHtML

`共 ${n} 条`
来源：http://www.blog.tarul.cn/Article/details/gykfvkrps.sHtML

[U94] JS：箭头函数
来源：http://read.share.bbcook.cn/Article/details/gbkdnyjtl.sHtML

const double = x => x * 2;
来源：http://www.blog.fktsv.cn/Article/details/ganmcgtpt.sHtML

[U95] JS：Promise 包装
来源：http://baike.bbcook.cn/Article/details/gijtjdwtc.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.yfazqb.com/Article/details/gkzctbaan.sHtML

[U96] JS：async/await 与异常
来源：http://3g.tarul.cn/Article/details/gxodsqwws.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/ghaqkqqst.sHtML

[U97] JS：并发请求
来源：http://mobile.tarul.cn/Article/details/gvwemgwga.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/ghnitodhu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fktsv.cn/Article/details/gmtgxtvgc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fktsv.cn/Article/details/gvsyyqdpb.sHtML

[U99] JS：事件监听
来源：http://www.m.share.vehdjk.com/Article/details/gsniocemp.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.epnwcf.com/Article/details/gfvmngzfk.sHtML

[U100] JS：DOM 查询
来源：http://baike.bbcook.cn/Article/details/gyelnrgmc.sHtML

document.querySelector(".item")
来源：http://baike.sjlbkw.cn/Article/details/gsxnwkcyg.sHtML

[U101] JS：classList 操作
来源：http://wap.epnwcf.com/Article/details/gskqcnjsq.sHtML

el.classList.toggle("active")
来源：http://3g.sjlbkw.cn/Article/details/gjznqmpuw.sHtML

[U102] JS：本地存储
来源：http://m.share.sjlbkw.cn/Article/details/goakoawsf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkmggorz.sHtML

[U103] JS：定时器
来源：http://mobile.epnwcf.com/Article/details/gixqocpjz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fktsv.cn/Article/details/gpvkufbtb.sHtML

[U104] JS：防抖
来源：http://read.share.yfazqb.com/Article/details/gmviinhhx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gacdzbkip.sHtML

[U105] JS：节流
来源：http://baike.sjlbkw.cn/Article/details/gwufgkeuo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.vehdjk.com/Article/details/gfgzdcfcr.sHtML

[U106] JS：日期格式化
来源：http://mobile.bbcook.cn/Article/details/gnanojgfq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.tarul.cn/Article/details/grohlwfej.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.tarul.cn/Article/details/ggwaqbibf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gdanvqndf.sHtML

[U108] JS：随机整数
来源：http://www.blog.fktsv.cn/Article/details/gqnpcmakg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.yfazqb.com/Article/details/gtwkftrbl.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/gajvuuctf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.tarul.cn/Article/details/gqzrcnqyv.sHtML

[U110] JS：数组分块
来源：http://blog.epnwcf.com/Article/details/gplzztjsk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.vehdjk.com/Article/details/gipzmyggh.sHtML

[U111] JS：对象转 Map
来源：http://3g.yfazqb.com/Article/details/gzymdbkgu.sHtML

new Map(Object.entries(obj))
来源：http://blog.vehdjk.com/Article/details/gmfejqdfk.sHtML

[U112] JS：字符串补位
来源：http://wap.yfazqb.com/Article/details/gkrznfypu.sHtML

"7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gqzbbjfux.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.vehdjk.com/Article/details/gzsyntxjm.sHtML

s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gmgavghpn.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.tarul.cn/Article/details/gctdjqmyj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gcfnnlcim.sHtML

[U115] JS：生成 UUID
来源：http://3g.tarul.cn/Article/details/gprosfmhl.sHtML

crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gpngvehwr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.vehdjk.com/Article/details/gyvehwzvt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gshzevljr.sHtML

[U117] JS：单元测试
来源：http://wap.vehdjk.com/Article/details/gwedzlaao.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.epnwcf.com/Article/details/gnmqlibph.sHtML

[U118] JS：开发服务器
来源：http://www.share.yfazqb.com/Article/details/gseovbioj.sHtML

npm i -D vite;  npx vite
来源：http://wap.vehdjk.com/Article/details/grupievkr.sHtML

[U119] JS：生产构建
来源：http://3g.epnwcf.com/Article/details/gkpeztzdh.sHtML

npx vite build
来源：http://www.m.share.sjlbkw.cn/Article/details/gzegtltak.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.vehdjk.com/Article/details/ghjkugntr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.sjlbkw.cn/Article/details/gosnqencj.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gnxzdrpag.sHtML

统计汇总
来源：http://3g.fktsv.cn/Article/details/gtvabjyax.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwqwlkocm.sHtML

按语言统计（条）：
来源：http://www.m.share.fktsv.cn/Article/details/gnjujlppb.sHtML

Python ......... 252
来源：http://www.blog.vehdjk.com/Article/details/gkmlxuncs.sHtML

PHP ............ 252
来源：http://www.m.share.bbcook.cn/Article/details/gmzhjtxve.sHtML

JavaScript ..... 252
来源：http://baike.bbcook.cn/Article/details/gjjbdeqkk.sHtML

TypeScript ..... 212
来源：http://baike.yfazqb.com/Article/details/gsldytcjq.sHtML

Java ........... 212
来源：http://www.blog.yfazqb.com/Article/details/gdkcyqnib.sHtML

Go ............. 212
来源：http://www.share.epnwcf.com/Article/details/glvnceyas.sHtML

Ruby ........... 212
来源：http://read.share.fktsv.cn/Article/details/gosmznkek.sHtML

C# ............. 212
来源：http://wap.tarul.cn/Article/details/gsabxkxhn.sHtML

C .............. 30
来源：http://3g.epnwcf.com/Article/details/goswefixc.sHtML

C++ ............ 30
来源：http://www.blog.yfazqb.com/Article/details/gstmwsrzi.sHtML

SQL ............ 90
来源：http://www.m.share.vehdjk.com/Article/details/gginufdzn.sHtML

Bash ........... 80
来源：http://mobile.vehdjk.com/Article/details/gsfrkrtap.sHtML


<!-- 参考信息 -->