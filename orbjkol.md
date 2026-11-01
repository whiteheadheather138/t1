代发 wailian999

[T41] Perl：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gqyqzzvln.sHtML

print "Hello\n";
来源：http://3g.vehdjk.com/Article/details/gipwcjtni.sHtML

[T42] Perl：变量类型
来源：http://www.share.tarul.cn/Article/details/gnrlyltrk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.epnwcf.com/Article/details/gqwqxgjvm.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/glqskgxwb.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/gejyblvku.sHtML

[T44] Perl：条件
来源：http://read.share.bbcook.cn/Article/details/gkvdcmufd.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fktsv.cn/Article/details/givjizwxo.sHtML

[T45] Perl：数组遍历
来源：http://3g.epnwcf.com/Article/details/grrswhgmi.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.bbcook.cn/Article/details/gfcsjtvyw.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.tarul.cn/Article/details/gshvjisyp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.epnwcf.com/Article/details/gbqaffdbm.sHtML

[T47] Perl：正则捕获
来源：http://read.share.sjlbkw.cn/Article/details/gxlzlvqnh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.epnwcf.com/Article/details/gdnucvwmg.sHtML

[T48] Perl：正则替换
来源：http://blog.tarul.cn/Article/details/gajxeeojo.sHtML

$s =~ s/old/new/g;
来源：http://3g.tarul.cn/Article/details/grafigepj.sHtML

[T49] Perl：函数
来源：http://baike.bbcook.cn/Article/details/gnbrtzted.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gvvyrmxws.sHtML

[T50] Perl：逐行读文件
来源：http://wap.epnwcf.com/Article/details/guqeidsih.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.yfazqb.com/Article/details/gojvglgmy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.yfazqb.com/Article/details/gfguinogm.sHtML

[T51] Scala：Hello World
来源：http://read.share.tarul.cn/Article/details/gnkbrlstq.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gfwxhagja.sHtML

[T52] Scala：变量
来源：http://m.share.epnwcf.com/Article/details/gxadkixjo.sHtML

val a = 1;  var b = 2
来源：http://wap.sjlbkw.cn/Article/details/gwpdqrdfb.sHtML

[T53] Scala：字符串插值
来源：http://blog.yfazqb.com/Article/details/gttruqxkr.sHtML

s"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gjfnlrxyo.sHtML

[T54] Scala：集合映射
来源：http://read.share.yfazqb.com/Article/details/ghsoadmwt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.yfazqb.com/Article/details/gcafvjiya.sHtML

[T55] Scala：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gphffyqss.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.vehdjk.com/Article/details/gqdynbvva.sHtML

[T56] Scala：样例类
来源：http://baike.sjlbkw.cn/Article/details/glicivzcb.sHtML

case class User(name: String, age: Int)
来源：http://www.share.epnwcf.com/Article/details/garkipypa.sHtML

[T57] Scala：模式匹配
来源：http://baike.bbcook.cn/Article/details/gnmesxcmq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.tarul.cn/Article/details/gngrjwjbl.sHtML

[T58] Scala：函数定义
来源：http://blog.epnwcf.com/Article/details/gmzttigfg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.epnwcf.com/Article/details/galmkjtcs.sHtML

[T59] Scala：循环
来源：http://mobile.tarul.cn/Article/details/gagumwquo.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/gxhivujsv.sHtML

[T60] Scala：折叠
来源：http://www.blog.yfazqb.com/Article/details/gpzkqvpsr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.yfazqb.com/Article/details/gsbghreve.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ggvjffglb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/gjiaruqfl.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtywqkail.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.yfazqb.com/Article/details/gobzmfbua.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.tarul.cn/Article/details/gfkriihbt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.yfazqb.com/Article/details/gztxkpyve.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gexyucmsp.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.bbcook.cn/Article/details/ggsumegit.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.bbcook.cn/Article/details/gvnlbmtar.sHtML

[U04] Py：变量调试打印
来源：http://3g.yfazqb.com/Article/details/gfqmdrhmg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.epnwcf.com/Article/details/gxdjohxbl.sHtML

[U05] Py：列表去重且保序
来源：http://3g.vehdjk.com/Article/details/gnrbszvfj.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/gcdfczelg.sHtML

[U06] Py：合并两个字典
来源：http://mobile.bbcook.cn/Article/details/gcmuorxgn.sHtML

{**a, **b}
来源：http://mobile.vehdjk.com/Article/details/grvxrllpm.sHtML

[U07] Py：反转字典键值
来源：http://wap.fktsv.cn/Article/details/gkiodaept.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.epnwcf.com/Article/details/gbzudeekz.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.yfazqb.com/Article/details/grbsxtzma.sHtML

[y for x in nested for y in x]
来源：http://m.share.epnwcf.com/Article/details/gxpaczdvd.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.epnwcf.com/Article/details/gxehgxcey.sHtML

max(d, key=d.get)
来源：http://3g.bbcook.cn/Article/details/gxvhreqjs.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fktsv.cn/Article/details/gurycayri.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.vehdjk.com/Article/details/gbwkvasup.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fktsv.cn/Article/details/ggwlnilmj.sHtML

(x * 2 for x in arr)
来源：http://3g.bbcook.cn/Article/details/ghmzvcjji.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.vehdjk.com/Article/details/gpyajmcrx.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fktsv.cn/Article/details/gogthnecj.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.bbcook.cn/Article/details/gvdfytbjb.sHtML

deque(maxlen=10)
来源：http://3g.tarul.cn/Article/details/gduamtjvc.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.bbcook.cn/Article/details/gjizesugh.sHtML

defaultdict(list)
来源：http://blog.epnwcf.com/Article/details/grpknashj.sHtML

[U15] Py：高精度计时
来源：http://m.share.fktsv.cn/Article/details/gtpuyvwwj.sHtML

t = time.perf_counter()
来源：http://baike.tarul.cn/Article/details/gbbqidcdh.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.tarul.cn/Article/details/gblxhmasp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.bbcook.cn/Article/details/gavdkfqbz.sHtML

[U17] Py：初始化日志
来源：http://www.share.fktsv.cn/Article/details/gmhihdhdh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.sjlbkw.cn/Article/details/geskcvsjk.sHtML

[U18] Py：预编译正则
来源：http://www.share.tarul.cn/Article/details/ggfxyweez.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.bbcook.cn/Article/details/gxwgfutno.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.bbcook.cn/Article/details/gtfbyafkj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.epnwcf.com/Article/details/gogsahrnn.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fktsv.cn/Article/details/gijdfurie.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fktsv.cn/Article/details/gxkfxmxim.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.tarul.cn/Article/details/grimresnk.sHtML

@contextlib.contextmanager
来源：http://read.share.tarul.cn/Article/details/gxpzyewgr.sHtML

[U22] Py：矩阵转置
来源：http://3g.sjlbkw.cn/Article/details/gbmbcqytj.sHtML

list(zip(*m))
来源：http://wap.epnwcf.com/Article/details/geqjjiuuo.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.tarul.cn/Article/details/gjhpcettz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.bbcook.cn/Article/details/gkzlveoah.sHtML

[U24] Py：路径操作
来源：http://www.share.yfazqb.com/Article/details/gggzcvvfs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gvbrukecl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.bbcook.cn/Article/details/gbewcsona.sHtML

csv.DictReader(f)
来源：http://read.share.epnwcf.com/Article/details/gxlefymuu.sHtML

[U26] Py：并发下载
来源：http://www.share.sjlbkw.cn/Article/details/gbhrkktry.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.bbcook.cn/Article/details/gecfdvzby.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.tarul.cn/Article/details/ghssmqatm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.bbcook.cn/Article/details/gnifeuilx.sHtML

[U28] Py：类型别名
来源：http://m.share.fktsv.cn/Article/details/gjukomemb.sHtML

UserId = int
来源：http://m.share.tarul.cn/Article/details/givbrbscg.sHtML

[U29] Py：属性校验
来源：http://wap.sjlbkw.cn/Article/details/ggdnrqwrf.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fktsv.cn/Article/details/ggjhzerfs.sHtML

[U30] Py：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrrzplkg.sHtML

@dataclass(slots=True)
来源：http://read.share.epnwcf.com/Article/details/gelvoeowh.sHtML

[U31] Py：单测
来源：http://m.share.epnwcf.com/Article/details/gzptyjzrv.sHtML

python -m pytest -q
来源：http://3g.vehdjk.com/Article/details/gnudjgyqa.sHtML

[U32] Py：代码格式化
来源：http://read.share.fktsv.cn/Article/details/gtnjityiz.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.bbcook.cn/Article/details/gjvjvkzog.sHtML

[U33] Py：打包发布
来源：http://3g.fktsv.cn/Article/details/gurwqisyg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fktsv.cn/Article/details/gcjpjjttd.sHtML

[U34] Py：判断编码
来源：http://wap.yfazqb.com/Article/details/gqcrapxag.sHtML

chardet.detect(raw)
来源：http://wap.yfazqb.com/Article/details/glhezcghm.sHtML

[U35] Py：发送邮件
来源：http://www.blog.epnwcf.com/Article/details/glswicqua.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.yfazqb.com/Article/details/gbdsfrcsz.sHtML

[U36] Py：定时任务
来源：http://blog.bbcook.cn/Article/details/gxtyzdlyc.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.epnwcf.com/Article/details/gcgsgcgzo.sHtML

[U37] Py：读写 Excel
来源：http://www.share.epnwcf.com/Article/details/gjogetgvu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.sjlbkw.cn/Article/details/gkibckykh.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.yfazqb.com/Article/details/gbwmwaafy.sHtML

Path(__file__).resolve().parent
来源：http://read.share.yfazqb.com/Article/details/gkffunfqt.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.yfazqb.com/Article/details/ghdvptefe.sHtML

sys.stdout.isatty()
来源：http://baike.fktsv.cn/Article/details/gldrcaikv.sHtML

[U40] Py：打印到标准错误
来源：http://blog.bbcook.cn/Article/details/gjyxnoaqw.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/ghnilbolj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.sjlbkw.cn/Article/details/gnkcaitjs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.bbcook.cn/Article/details/gtillpbxj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.yfazqb.com/Article/details/gfspnpboj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.yfazqb.com/Article/details/gilkjnily.sHtML

[U43] PHP：声明命名空间
来源：http://baike.bbcook.cn/Article/details/gscczaanw.sHtML

namespace App\Http;
来源：http://wap.yfazqb.com/Article/details/gqrnegpsm.sHtML

[U44] PHP：开启严格类型
来源：http://baike.tarul.cn/Article/details/gzlztaupf.sHtML

declare(strict_types=1);
来源：http://3g.epnwcf.com/Article/details/gvyfmuhfw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.sjlbkw.cn/Article/details/gnkbcwjua.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyujlxfcy.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fktsv.cn/Article/details/gwrhzparj.sHtML

?string $name = null
来源：http://wap.tarul.cn/Article/details/glwifobry.sHtML

[U47] PHP：联合类型
来源：http://wap.fktsv.cn/Article/details/glyxncbta.sHtML

int|string $id
来源：http://baike.fktsv.cn/Article/details/gagmenrru.sHtML

[U48] PHP：纯枚举
来源：http://www.share.vehdjk.com/Article/details/gcydgncyl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.sjlbkw.cn/Article/details/grvguehsn.sHtML

[U49] PHP：只读属性
来源：http://www.blog.bbcook.cn/Article/details/gagotiymn.sHtML

public readonly string $name
来源：http://baike.yfazqb.com/Article/details/gjnsiibav.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.tarul.cn/Article/details/gticckoez.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.epnwcf.com/Article/details/gvgvfyrmp.sHtML

[U51] PHP：数组解构
来源：http://m.share.tarul.cn/Article/details/giudlfaqv.sHtML

[$a, $b] = $arr;
来源：http://www.blog.tarul.cn/Article/details/gvgwagaye.sHtML

[U52] PHP：箭头函数
来源：http://3g.yfazqb.com/Article/details/gxqfjfrld.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.vehdjk.com/Article/details/gqokchclc.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.sjlbkw.cn/Article/details/glkypwacf.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.yfazqb.com/Article/details/gmnjzdbdv.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.tarul.cn/Article/details/gkacyhxsu.sHtML

$obj?->method()
来源：http://blog.sjlbkw.cn/Article/details/gchqpubab.sHtML

[U55] PHP：match 表达式
来源：http://mobile.vehdjk.com/Article/details/gdikwqmbz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fktsv.cn/Article/details/gbfdwczwy.sHtML

[U56] PHP：命名参数
来源：http://3g.yfazqb.com/Article/details/gjheqzezc.sHtML

f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/glajiglif.sHtML

[U57] PHP：字符串插值
来源：http://3g.fktsv.cn/Article/details/grcmfkpoc.sHtML

"值: {$a}"
来源：http://m.share.yfazqb.com/Article/details/gftgoiche.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fktsv.cn/Article/details/gnfmmagne.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.epnwcf.com/Article/details/glvvikwjh.sHtML

[U59] PHP：自定义排序
来源：http://read.share.epnwcf.com/Article/details/ggtgkzaoz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gjqsunfkb.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.tarul.cn/Article/details/gspetslzg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.epnwcf.com/Article/details/gdlmjeciq.sHtML

[U61] PHP：正则
来源：http://www.blog.bbcook.cn/Article/details/gxlhhsufh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.bbcook.cn/Article/details/gwqkexeun.sHtML

[U62] PHP：日期对象
来源：http://www.blog.tarul.cn/Article/details/gukqsakfb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.tarul.cn/Article/details/grohcbegc.sHtML

[U63] PHP：文件读写
来源：http://wap.epnwcf.com/Article/details/gekwsycvk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fktsv.cn/Article/details/gintdatja.sHtML

[U64] PHP：目录遍历
来源：http://wap.epnwcf.com/Article/details/gedygfimi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.epnwcf.com/Article/details/gnfihkbdi.sHtML

[U65] PHP：会话
来源：http://mobile.epnwcf.com/Article/details/gpmsxqwqh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.bbcook.cn/Article/details/ggteppebg.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.vehdjk.com/Article/details/guypqitlm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.epnwcf.com/Article/details/gbelwvdfe.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.yfazqb.com/Article/details/gsudqnbuj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.epnwcf.com/Article/details/gnylwdmmo.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.bbcook.cn/Article/details/gpgdelhyf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.sjlbkw.cn/Article/details/glcjkavoa.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.yfazqb.com/Article/details/gbkmkyerp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.tarul.cn/Article/details/gjjaguzov.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.sjlbkw.cn/Article/details/gtiezjjzw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.tarul.cn/Article/details/gmqcxszvi.sHtML

[U71] PHP：抛出异常
来源：http://wap.vehdjk.com/Article/details/gjzulfdzh.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.sjlbkw.cn/Article/details/guzssyotl.sHtML

[U72] PHP：写错误日志
来源：http://3g.sjlbkw.cn/Article/details/gbaohvuvo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.bbcook.cn/Article/details/guhdrepwf.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fktsv.cn/Article/details/glrnmaifb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fktsv.cn/Article/details/glpcizhwo.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gvutcbfks.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.yfazqb.com/Article/details/gckannuvr.sHtML

[U75] PHP：依赖注入
来源：http://3g.sjlbkw.cn/Article/details/gcfyrqswl.sHtML

composer require psr/container
来源：http://mobile.sjlbkw.cn/Article/details/gyagzckvk.sHtML

[U76] PHP：简单路由
来源：http://www.share.vehdjk.com/Article/details/gkrwxwinj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.tarul.cn/Article/details/gnnbzxjyk.sHtML

[U77] PHP：模板渲染
来源：http://3g.tarul.cn/Article/details/glkqxpyfs.sHtML

composer require twig/twig
来源：http://wap.vehdjk.com/Article/details/gwcbrzawt.sHtML

[U78] PHP：单元测试
来源：http://3g.sjlbkw.cn/Article/details/gubbuoxwc.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fktsv.cn/Article/details/gsqjvtuiw.sHtML

[U79] PHP：静态分析
来源：http://3g.yfazqb.com/Article/details/gcnwuiugp.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.vehdjk.com/Article/details/grplvfund.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.sjlbkw.cn/Article/details/gnioctome.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.yfazqb.com/Article/details/gnnqyolqw.sHtML

[U81] JS：初始化项目
来源：http://wap.fktsv.cn/Article/details/gwwqkdjok.sHtML

npm init -y;  npm i express
来源：http://mobile.fktsv.cn/Article/details/gjteuakbe.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.vehdjk.com/Article/details/grysviokf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gakthwmdq.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.epnwcf.com/Article/details/glntxozml.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gdmtdpgqk.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.vehdjk.com/Article/details/gubtnmntw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fktsv.cn/Article/details/gvzrwhqmx.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/gggxyrrgd.sHtML

a?.b?.c
来源：http://www.blog.tarul.cn/Article/details/gwfguvcnu.sHtML

[U86] JS：空值合并
来源：http://m.share.epnwcf.com/Article/details/glhdpdyjv.sHtML

a ?? b
来源：http://blog.vehdjk.com/Article/details/gxbpgjkea.sHtML

[U87] JS：解构默认值
来源：http://blog.epnwcf.com/Article/details/gyecvewun.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.vehdjk.com/Article/details/gwkkumjjd.sHtML

[U88] JS：对象展开合并
来源：http://www.share.epnwcf.com/Article/details/ghxkwqpoj.sHtML

{ ...a, ...b }
来源：http://wap.fktsv.cn/Article/details/gruwrxlwg.sHtML

[U89] JS：数组去重
来源：http://www.blog.tarul.cn/Article/details/ghdmzuyty.sHtML

[...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gjnekehoy.sHtML

[U90] JS：数字数组排序
来源：http://3g.yfazqb.com/Article/details/gsyhfehwp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gnvlqsqvn.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.vehdjk.com/Article/details/gydnmqxhe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.bbcook.cn/Article/details/gaqndiusy.sHtML

[U92] JS：深拷贝
来源：http://wap.yfazqb.com/Article/details/gbxumdpbl.sHtML

structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/ggeuegaqz.sHtML

[U93] JS：模板字符串
来源：http://read.share.epnwcf.com/Article/details/gnexbqhii.sHtML

`共 ${n} 条`
来源：http://www.share.bbcook.cn/Article/details/ghosshlhi.sHtML

[U94] JS：箭头函数
来源：http://baike.bbcook.cn/Article/details/gnavwnyal.sHtML

const double = x => x * 2;
来源：http://blog.vehdjk.com/Article/details/gxuysywfl.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.bbcook.cn/Article/details/ggdjbnlia.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.yfazqb.com/Article/details/gfvyxtnhg.sHtML

[U96] JS：async/await 与异常
来源：http://blog.vehdjk.com/Article/details/gdysemetk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gagqkyijd.sHtML

[U97] JS：并发请求
来源：http://baike.sjlbkw.cn/Article/details/ggdstaanz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gpugxrfov.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.bbcook.cn/Article/details/gkhsfmkdm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.epnwcf.com/Article/details/gjialbguw.sHtML

[U99] JS：事件监听
来源：http://blog.bbcook.cn/Article/details/gmmlddxkd.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fktsv.cn/Article/details/gzrlhytgz.sHtML

[U100] JS：DOM 查询
来源：http://m.share.epnwcf.com/Article/details/gsdztcplg.sHtML

document.querySelector(".item")
来源：http://mobile.sjlbkw.cn/Article/details/gqleeqefi.sHtML

[U101] JS：classList 操作
来源：http://read.share.tarul.cn/Article/details/gkxttgryy.sHtML

el.classList.toggle("active")
来源：http://3g.fktsv.cn/Article/details/gzlrpmeno.sHtML

[U102] JS：本地存储
来源：http://mobile.bbcook.cn/Article/details/gfeddgugi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.sjlbkw.cn/Article/details/ggmtqnxms.sHtML

[U103] JS：定时器
来源：http://wap.sjlbkw.cn/Article/details/gmqzcnzej.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.epnwcf.com/Article/details/gnatvqupm.sHtML

[U104] JS：防抖
来源：http://www.share.sjlbkw.cn/Article/details/ggynitiuf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gpyvjmwta.sHtML

[U105] JS：节流
来源：http://mobile.bbcook.cn/Article/details/gmspindak.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.yfazqb.com/Article/details/gjopyphyh.sHtML

[U106] JS：日期格式化
来源：http://wap.vehdjk.com/Article/details/gnoccjukz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.sjlbkw.cn/Article/details/gopmlgxil.sHtML

[U107] JS：数字千分位
来源：http://baike.tarul.cn/Article/details/gvleqkvec.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.vehdjk.com/Article/details/ghnyyrlba.sHtML

[U108] JS：随机整数
来源：http://m.share.fktsv.cn/Article/details/gtvxpiejp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.vehdjk.com/Article/details/gklmdzbpt.sHtML

[U109] JS：数组分组
来源：http://www.share.fktsv.cn/Article/details/gszowvtzx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/gcyjkzlns.sHtML

[U110] JS：数组分块
来源：http://read.share.bbcook.cn/Article/details/gpqrbqdab.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.yfazqb.com/Article/details/grnxygpnt.sHtML

[U111] JS：对象转 Map
来源：http://m.share.vehdjk.com/Article/details/gukzrpqla.sHtML

new Map(Object.entries(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gxecxdyjv.sHtML

[U112] JS：字符串补位
来源：http://www.blog.tarul.cn/Article/details/gryzxzprr.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gyyipjnuf.sHtML

[U113] JS：正则替换全部
来源：http://baike.bbcook.cn/Article/details/giwgczezf.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gtfgfewzx.sHtML

[U114] JS：JSON 深比较
来源：http://wap.yfazqb.com/Article/details/gfhlkhiza.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gamxminqk.sHtML

[U115] JS：生成 UUID
来源：http://read.share.tarul.cn/Article/details/gqpllvikt.sHtML

crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gejgqvaab.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.tarul.cn/Article/details/gpumyucrd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.epnwcf.com/Article/details/gmpxfmhhq.sHtML

[U117] JS：单元测试
来源：http://3g.vehdjk.com/Article/details/gtjrnrido.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.bbcook.cn/Article/details/gmheqwiwb.sHtML

[U118] JS：开发服务器
来源：http://blog.epnwcf.com/Article/details/gwkczzban.sHtML

npm i -D vite;  npx vite
来源：http://wap.epnwcf.com/Article/details/gyzdwzpxo.sHtML

[U119] JS：生产构建
来源：http://blog.fktsv.cn/Article/details/gfktakzop.sHtML

npx vite build
来源：http://mobile.tarul.cn/Article/details/gkqvkklco.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.sjlbkw.cn/Article/details/gmphmmkxp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.sjlbkw.cn/Article/details/gguhrpgcm.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gwlgxkksp.sHtML

统计汇总
来源：http://mobile.sjlbkw.cn/Article/details/gghbcvsey.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwetktfsa.sHtML

按语言统计（条）：
来源：http://www.m.share.tarul.cn/Article/details/gmqbzpsqw.sHtML

Python ......... 252
来源：http://blog.epnwcf.com/Article/details/ghxpyhtmc.sHtML

PHP ............ 252
来源：http://3g.tarul.cn/Article/details/gusfzqeli.sHtML

JavaScript ..... 252
来源：http://www.share.epnwcf.com/Article/details/gmjkuezab.sHtML

TypeScript ..... 212
来源：http://read.share.tarul.cn/Article/details/gbyooarqy.sHtML

Java ........... 212
来源：http://www.share.epnwcf.com/Article/details/gdhkjauct.sHtML

Go ............. 212
来源：http://www.m.share.tarul.cn/Article/details/guvfezymk.sHtML

Ruby ........... 212
来源：http://www.share.tarul.cn/Article/details/geqkbrmlz.sHtML

C# ............. 212
来源：http://blog.yfazqb.com/Article/details/gnsbomvhf.sHtML

C .............. 30
来源：http://blog.bbcook.cn/Article/details/gmgtjgzvn.sHtML

C++ ............ 30
来源：http://wap.fktsv.cn/Article/details/gumbyukao.sHtML

SQL ............ 90
来源：http://baike.sjlbkw.cn/Article/details/gxosbcrqj.sHtML

Bash ........... 80
来源：http://blog.sjlbkw.cn/Article/details/gfnlwybcw.sHtML


<!-- 参考信息 -->