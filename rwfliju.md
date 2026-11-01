代发 wailian999

[T45] Perl：数组遍历
来源：http://baike.fktsv.cn/Article/details/gdwqagfjy.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.bbcook.cn/Article/details/gtvwmgrpj.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gicnjubwo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.yfazqb.com/Article/details/gfhwfxbni.sHtML

[T47] Perl：正则捕获
来源：http://baike.vehdjk.com/Article/details/gxkjbkfau.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.yfazqb.com/Article/details/gawonesnq.sHtML

[T48] Perl：正则替换
来源：http://wap.fktsv.cn/Article/details/gyodprusr.sHtML

$s =~ s/old/new/g;
来源：http://www.share.bbcook.cn/Article/details/grcvknfbq.sHtML

[T49] Perl：函数
来源：http://blog.epnwcf.com/Article/details/gngzpzhgu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqzmtijg.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gnwxtvaid.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.tarul.cn/Article/details/gomcwqgns.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.tarul.cn/Article/details/gcmjcywhz.sHtML

[T51] Scala：Hello World
来源：http://3g.fktsv.cn/Article/details/gybbwfdrz.sHtML

println("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gpgmorujd.sHtML

[T52] Scala：变量
来源：http://www.m.share.vehdjk.com/Article/details/goresxfyv.sHtML

val a = 1;  var b = 2
来源：http://www.share.sjlbkw.cn/Article/details/glscsdsyd.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gmyamqqza.sHtML

s"值: $b"
来源：http://wap.tarul.cn/Article/details/gtkyuiioo.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/gbesrwvsf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fktsv.cn/Article/details/gcdsmlrng.sHtML

[T55] Scala：集合过滤
来源：http://3g.bbcook.cn/Article/details/gmnpzancv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.vehdjk.com/Article/details/gcoufleqi.sHtML

[T56] Scala：样例类
来源：http://3g.bbcook.cn/Article/details/gxxzcdtgc.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjiwhtgxl.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbifbawy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.bbcook.cn/Article/details/gozwiqzzg.sHtML

[T58] Scala：函数定义
来源：http://www.blog.yfazqb.com/Article/details/gjxfxlyyi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/gqiiyzamv.sHtML

[T59] Scala：循环
来源：http://m.share.sjlbkw.cn/Article/details/gyhcfsuss.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.bbcook.cn/Article/details/gfbkzpqal.sHtML

[T60] Scala：折叠
来源：http://www.blog.epnwcf.com/Article/details/gponupiqw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.tarul.cn/Article/details/gmdpoguln.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkihnrbgu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.epnwcf.com/Article/details/gsztmeuds.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbgpjpghf.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.vehdjk.com/Article/details/gnjnhmfdr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.yfazqb.com/Article/details/gebqeulow.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.vehdjk.com/Article/details/gffsmxxno.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.sjlbkw.cn/Article/details/ggjrarrwv.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.sjlbkw.cn/Article/details/grqedovvl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fktsv.cn/Article/details/gujdoufir.sHtML

[U04] Py：变量调试打印
来源：http://mobile.epnwcf.com/Article/details/ginqytrrj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.vehdjk.com/Article/details/gmepprtco.sHtML

[U05] Py：列表去重且保序
来源：http://wap.bbcook.cn/Article/details/gudsuldqx.sHtML

list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/gnoquryqq.sHtML

[U06] Py：合并两个字典
来源：http://www.share.sjlbkw.cn/Article/details/gjwiwepyq.sHtML

{**a, **b}
来源：http://www.share.tarul.cn/Article/details/gxlvtwpyi.sHtML

[U07] Py：反转字典键值
来源：http://mobile.sjlbkw.cn/Article/details/gfgqwvqck.sHtML

{v: k for k, v in d.items()}
来源：http://baike.yfazqb.com/Article/details/gvswlllod.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.tarul.cn/Article/details/grcjmmozl.sHtML

[y for x in nested for y in x]
来源：http://baike.bbcook.cn/Article/details/gkxtfbgxn.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.yfazqb.com/Article/details/gnuxidkbw.sHtML

max(d, key=d.get)
来源：http://www.m.share.tarul.cn/Article/details/grwhabkvj.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fktsv.cn/Article/details/gbhzonptj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyrcbmsz.sHtML

[U11] Py：生成器表达式
来源：http://wap.epnwcf.com/Article/details/gbiseechw.sHtML

(x * 2 for x in arr)
来源：http://3g.tarul.cn/Article/details/ghwaerxjs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.vehdjk.com/Article/details/gfwuomrzo.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.bbcook.cn/Article/details/ggwyjxihu.sHtML

[U13] Py：固定长度队列
来源：http://baike.bbcook.cn/Article/details/ggzadcqej.sHtML

deque(maxlen=10)
来源：http://baike.vehdjk.com/Article/details/glwbloisa.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.yfazqb.com/Article/details/gqniimoiv.sHtML

defaultdict(list)
来源：http://mobile.yfazqb.com/Article/details/gyzjqueve.sHtML

[U15] Py：高精度计时
来源：http://mobile.bbcook.cn/Article/details/gblydkafp.sHtML

t = time.perf_counter()
来源：http://www.m.share.epnwcf.com/Article/details/gcpwzpbda.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.epnwcf.com/Article/details/gvmjniftv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.sjlbkw.cn/Article/details/grqoembsc.sHtML

[U17] Py：初始化日志
来源：http://www.blog.tarul.cn/Article/details/glosyoask.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/gcrhdnsjm.sHtML

[U18] Py：预编译正则
来源：http://wap.bbcook.cn/Article/details/gplbxfpjm.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/gcxczdbnw.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.epnwcf.com/Article/details/gqxpgubxm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.vehdjk.com/Article/details/gdqnyeyqh.sHtML

[U20] Py：缓存函数结果
来源：http://blog.epnwcf.com/Article/details/gjapzllqj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.yfazqb.com/Article/details/gytlwcswc.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.sjlbkw.cn/Article/details/gvxdcxrbe.sHtML

@contextlib.contextmanager
来源：http://www.share.epnwcf.com/Article/details/ghbtpuzjo.sHtML

[U22] Py：矩阵转置
来源：http://baike.yfazqb.com/Article/details/gzwdtnsdm.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/gdroanprk.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.vehdjk.com/Article/details/ghyluayze.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.vehdjk.com/Article/details/ghhijmkch.sHtML

[U24] Py：路径操作
来源：http://www.m.share.yfazqb.com/Article/details/gpzkjfsjm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.tarul.cn/Article/details/ggqyudacn.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.tarul.cn/Article/details/gipukumus.sHtML

csv.DictReader(f)
来源：http://m.share.tarul.cn/Article/details/guyqewjhi.sHtML

[U26] Py：并发下载
来源：http://www.blog.bbcook.cn/Article/details/grblxxpuq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.sjlbkw.cn/Article/details/gpypjgmbm.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.vehdjk.com/Article/details/gmmfiehxz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.vehdjk.com/Article/details/gdkmlvobw.sHtML

[U28] Py：类型别名
来源：http://blog.vehdjk.com/Article/details/gunfpxqmr.sHtML

UserId = int
来源：http://www.m.share.vehdjk.com/Article/details/gzsydeqdi.sHtML

[U29] Py：属性校验
来源：http://read.share.yfazqb.com/Article/details/gzoztarkr.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.bbcook.cn/Article/details/gjtwhtity.sHtML

[U30] Py：数据类
来源：http://www.blog.vehdjk.com/Article/details/gankxosvm.sHtML

@dataclass(slots=True)
来源：http://www.blog.fktsv.cn/Article/details/ggkvjvnms.sHtML

[U31] Py：单测
来源：http://mobile.vehdjk.com/Article/details/gddqvtzop.sHtML

python -m pytest -q
来源：http://blog.vehdjk.com/Article/details/gmmpwppjh.sHtML

[U32] Py：代码格式化
来源：http://www.share.sjlbkw.cn/Article/details/gsmktmikv.sHtML

ruff format . && ruff check --fix .
来源：http://3g.tarul.cn/Article/details/gpnqumrko.sHtML

[U33] Py：打包发布
来源：http://www.m.share.tarul.cn/Article/details/gcavcnrea.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.epnwcf.com/Article/details/grymamdwx.sHtML

[U34] Py：判断编码
来源：http://www.share.epnwcf.com/Article/details/gsrtkroqn.sHtML

chardet.detect(raw)
来源：http://www.blog.sjlbkw.cn/Article/details/goaetfvwf.sHtML

[U35] Py：发送邮件
来源：http://blog.fktsv.cn/Article/details/gujpqinfy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.sjlbkw.cn/Article/details/giuzmkfsr.sHtML

[U36] Py：定时任务
来源：http://blog.tarul.cn/Article/details/gtcwootka.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.yfazqb.com/Article/details/gdcqvlixj.sHtML

[U37] Py：读写 Excel
来源：http://mobile.epnwcf.com/Article/details/gfyhyovoq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.vehdjk.com/Article/details/ggsoppuko.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.sjlbkw.cn/Article/details/gdsaksvhg.sHtML

Path(__file__).resolve().parent
来源：http://mobile.bbcook.cn/Article/details/gvdyairjl.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.yfazqb.com/Article/details/gblliewqv.sHtML

sys.stdout.isatty()
来源：http://wap.fktsv.cn/Article/details/gzrzecxby.sHtML

[U40] Py：打印到标准错误
来源：http://blog.sjlbkw.cn/Article/details/guyryfnzt.sHtML

print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/gsqxuhicz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.vehdjk.com/Article/details/gjmjwjstr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.epnwcf.com/Article/details/gahorpwyq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.yfazqb.com/Article/details/gexvlckxq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.vehdjk.com/Article/details/glesvjtjs.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.vehdjk.com/Article/details/grgbexipp.sHtML

namespace App\Http;
来源：http://read.share.epnwcf.com/Article/details/gvblyzoyz.sHtML

[U44] PHP：开启严格类型
来源：http://wap.sjlbkw.cn/Article/details/gdjzdauzy.sHtML

declare(strict_types=1);
来源：http://mobile.tarul.cn/Article/details/gbqjnwmfv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.sjlbkw.cn/Article/details/grtnebtek.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/ggtigdoqf.sHtML

[U46] PHP：可空类型
来源：http://3g.tarul.cn/Article/details/gznkbcawf.sHtML

?string $name = null
来源：http://3g.yfazqb.com/Article/details/gzdxszhgo.sHtML

[U47] PHP：联合类型
来源：http://www.blog.tarul.cn/Article/details/gmatwiklb.sHtML

int|string $id
来源：http://m.share.tarul.cn/Article/details/gtmxtmttg.sHtML

[U48] PHP：纯枚举
来源：http://m.share.yfazqb.com/Article/details/gsbbifvzk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fktsv.cn/Article/details/gufmirdam.sHtML

[U49] PHP：只读属性
来源：http://www.blog.bbcook.cn/Article/details/gxnvxemoj.sHtML

public readonly string $name
来源：http://wap.epnwcf.com/Article/details/giibmkhdo.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.sjlbkw.cn/Article/details/gqlcejmaj.sHtML

public function __construct(private int $id) {}
来源：http://3g.tarul.cn/Article/details/gkrmuyync.sHtML

[U51] PHP：数组解构
来源：http://3g.bbcook.cn/Article/details/goytjrewd.sHtML

[$a, $b] = $arr;
来源：http://3g.bbcook.cn/Article/details/ghcxedvdh.sHtML

[U52] PHP：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/gxdecrnzi.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.vehdjk.com/Article/details/gqedhgreg.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fktsv.cn/Article/details/gpgxvrwta.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.bbcook.cn/Article/details/ghcggsyjb.sHtML

[U54] PHP：空安全调用
来源：http://m.share.tarul.cn/Article/details/glwxwroty.sHtML

$obj?->method()
来源：http://www.m.share.sjlbkw.cn/Article/details/giqxdakdp.sHtML

[U55] PHP：match 表达式
来源：http://m.share.epnwcf.com/Article/details/geryecxcy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.vehdjk.com/Article/details/gdeijaghy.sHtML

[U56] PHP：命名参数
来源：http://3g.tarul.cn/Article/details/gqemllowx.sHtML

f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/grgmzskvo.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gdlwcnjzz.sHtML

"值: {$a}"
来源：http://3g.epnwcf.com/Article/details/gzsenzmmi.sHtML

[U58] PHP：数组三件套
来源：http://www.share.vehdjk.com/Article/details/gsgxzyupp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.yfazqb.com/Article/details/gstrezqyl.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.epnwcf.com/Article/details/gkmktqfrw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fktsv.cn/Article/details/gfqspydod.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.sjlbkw.cn/Article/details/gqeuubedj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fktsv.cn/Article/details/gxmhagnko.sHtML

[U61] PHP：正则
来源：http://www.m.share.fktsv.cn/Article/details/gwlmenbkp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gklurmmwk.sHtML

[U62] PHP：日期对象
来源：http://read.share.tarul.cn/Article/details/gdentpirh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.bbcook.cn/Article/details/grumaiugu.sHtML

[U63] PHP：文件读写
来源：http://m.share.epnwcf.com/Article/details/gdwbynjcv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.yfazqb.com/Article/details/ggdxbchza.sHtML

[U64] PHP：目录遍历
来源：http://3g.yfazqb.com/Article/details/ghqbxakbo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.tarul.cn/Article/details/grtoyhajm.sHtML

[U65] PHP：会话
来源：http://wap.yfazqb.com/Article/details/gyewfppwu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.vehdjk.com/Article/details/gmuobkelh.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fktsv.cn/Article/details/gzepgnvei.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.bbcook.cn/Article/details/gfflyhfll.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.sjlbkw.cn/Article/details/gnmydnoqr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.yfazqb.com/Article/details/geiavbhbh.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.epnwcf.com/Article/details/gydzvoyfo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fktsv.cn/Article/details/gtxicaocd.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.epnwcf.com/Article/details/gmafpxfbp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.epnwcf.com/Article/details/gmsrmgejs.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.sjlbkw.cn/Article/details/gwoqeitka.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.vehdjk.com/Article/details/geywlggeu.sHtML

[U71] PHP：抛出异常
来源：http://baike.bbcook.cn/Article/details/grjqgqmmn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.bbcook.cn/Article/details/gtfcwixaz.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fktsv.cn/Article/details/gbjbazkht.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.bbcook.cn/Article/details/gjxavgyso.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.tarul.cn/Article/details/glmwasgty.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.vehdjk.com/Article/details/goepsjfpu.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.tarul.cn/Article/details/gsxajakle.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fktsv.cn/Article/details/gkmhowazt.sHtML

[U75] PHP：依赖注入
来源：http://wap.fktsv.cn/Article/details/gfcmaihyq.sHtML

composer require psr/container
来源：http://m.share.bbcook.cn/Article/details/gghqjbrox.sHtML

[U76] PHP：简单路由
来源：http://3g.bbcook.cn/Article/details/gzgazayor.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.yfazqb.com/Article/details/gsgovzzwq.sHtML

[U77] PHP：模板渲染
来源：http://baike.yfazqb.com/Article/details/gfebteeus.sHtML

composer require twig/twig
来源：http://baike.vehdjk.com/Article/details/genyqnkwi.sHtML

[U78] PHP：单元测试
来源：http://mobile.sjlbkw.cn/Article/details/gnvkzragt.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.tarul.cn/Article/details/gawoucrpx.sHtML

[U79] PHP：静态分析
来源：http://read.share.sjlbkw.cn/Article/details/gggkunato.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.sjlbkw.cn/Article/details/grdmrgzdg.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.epnwcf.com/Article/details/glvfvmfii.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fktsv.cn/Article/details/gvyucgnmq.sHtML

[U81] JS：初始化项目
来源：http://baike.tarul.cn/Article/details/gavtrnrfs.sHtML

npm init -y;  npm i express
来源：http://read.share.fktsv.cn/Article/details/grqiknnme.sHtML

[U82] JS：package.json 脚本
来源：http://3g.sjlbkw.cn/Article/details/givrrbxez.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.yfazqb.com/Article/details/gjlxcqakj.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.bbcook.cn/Article/details/gbjnvkxys.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.yfazqb.com/Article/details/gflwkfydw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fktsv.cn/Article/details/gzztwfvqg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.vehdjk.com/Article/details/gfzojadqb.sHtML

[U85] JS：可选链
来源：http://blog.bbcook.cn/Article/details/gxnpnmhhx.sHtML

a?.b?.c
来源：http://www.blog.yfazqb.com/Article/details/gxmazflyo.sHtML

[U86] JS：空值合并
来源：http://m.share.bbcook.cn/Article/details/gytyergrp.sHtML

a ?? b
来源：http://3g.epnwcf.com/Article/details/guvakkpof.sHtML

[U87] JS：解构默认值
来源：http://baike.yfazqb.com/Article/details/gmeasbqbv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.yfazqb.com/Article/details/gcjunrjrj.sHtML

[U88] JS：对象展开合并
来源：http://read.share.yfazqb.com/Article/details/gcjqqwfcl.sHtML

{ ...a, ...b }
来源：http://wap.tarul.cn/Article/details/gkhrsgonj.sHtML

[U89] JS：数组去重
来源：http://www.blog.sjlbkw.cn/Article/details/gkbhqtnnl.sHtML

[...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gfbhqokeq.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fktsv.cn/Article/details/gysknssta.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gbhpbjszw.sHtML

[U91] JS：对象键值遍历
来源：http://baike.tarul.cn/Article/details/gjuzunsga.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.yfazqb.com/Article/details/gmslxvlre.sHtML

[U92] JS：深拷贝
来源：http://blog.bbcook.cn/Article/details/gsjdivvng.sHtML

structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gzaiykqsy.sHtML

[U93] JS：模板字符串
来源：http://mobile.bbcook.cn/Article/details/gzaikhbqh.sHtML

`共 ${n} 条`
来源：http://www.blog.sjlbkw.cn/Article/details/gcdzcdxzc.sHtML

[U94] JS：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gkxszinos.sHtML

const double = x => x * 2;
来源：http://www.m.share.yfazqb.com/Article/details/ghsizitlt.sHtML

[U95] JS：Promise 包装
来源：http://read.share.tarul.cn/Article/details/gyofupfkf.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.vehdjk.com/Article/details/gdqlaqkpw.sHtML

[U96] JS：async/await 与异常
来源：http://3g.vehdjk.com/Article/details/gwkljeeet.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gsrbqgvjm.sHtML

[U97] JS：并发请求
来源：http://m.share.fktsv.cn/Article/details/gibolwmkb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/galnoiopw.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.tarul.cn/Article/details/ggoqmrztz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fktsv.cn/Article/details/gkkqzhoxz.sHtML

[U99] JS：事件监听
来源：http://wap.epnwcf.com/Article/details/gueinuqit.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fktsv.cn/Article/details/gpijmlzpe.sHtML

[U100] JS：DOM 查询
来源：http://blog.yfazqb.com/Article/details/gqcnsplzh.sHtML

document.querySelector(".item")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjjeujpj.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gjukqugxd.sHtML

el.classList.toggle("active")
来源：http://m.share.vehdjk.com/Article/details/gtghvazsj.sHtML

[U102] JS：本地存储
来源：http://read.share.yfazqb.com/Article/details/gtdhwaiak.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fktsv.cn/Article/details/gdmgsaxiu.sHtML

[U103] JS：定时器
来源：http://www.m.share.epnwcf.com/Article/details/gxkwkvull.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.yfazqb.com/Article/details/gzxhzqqit.sHtML

[U104] JS：防抖
来源：http://mobile.sjlbkw.cn/Article/details/gvvjfoswt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gmhgzawet.sHtML

[U105] JS：节流
来源：http://www.blog.bbcook.cn/Article/details/gyanlrmxd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.yfazqb.com/Article/details/giydsfibx.sHtML

[U106] JS：日期格式化
来源：http://www.share.yfazqb.com/Article/details/gokkelpqt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.tarul.cn/Article/details/gzysghoqw.sHtML

[U107] JS：数字千分位
来源：http://www.blog.bbcook.cn/Article/details/gulllcskb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gpyhevwoa.sHtML

[U108] JS：随机整数
来源：http://3g.yfazqb.com/Article/details/gksqmmmmi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.sjlbkw.cn/Article/details/gfpndkybi.sHtML

[U109] JS：数组分组
来源：http://blog.bbcook.cn/Article/details/gsyopaqgo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/gromuktfu.sHtML

[U110] JS：数组分块
来源：http://www.share.bbcook.cn/Article/details/gulomrffx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.vehdjk.com/Article/details/gqwrjeyzs.sHtML

[U111] JS：对象转 Map
来源：http://baike.tarul.cn/Article/details/gutqusepa.sHtML

new Map(Object.entries(obj))
来源：http://baike.vehdjk.com/Article/details/grcgudjio.sHtML

[U112] JS：字符串补位
来源：http://m.share.bbcook.cn/Article/details/gpqrybkpp.sHtML

"7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gvcrjkpwf.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.bbcook.cn/Article/details/gatpomrqw.sHtML

s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gzfnnuhla.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.tarul.cn/Article/details/gkcvpxmhx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/glhzalnfy.sHtML

[U115] JS：生成 UUID
来源：http://baike.bbcook.cn/Article/details/gsxhzdmyy.sHtML

crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gmmmcwurr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.tarul.cn/Article/details/gyjcrgwny.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdxinnjef.sHtML

[U117] JS：单元测试
来源：http://baike.bbcook.cn/Article/details/gwyviusfw.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.tarul.cn/Article/details/glsuyhhgf.sHtML

[U118] JS：开发服务器
来源：http://mobile.vehdjk.com/Article/details/gthowxsgn.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fktsv.cn/Article/details/gjzllnuwo.sHtML

[U119] JS：生产构建
来源：http://mobile.epnwcf.com/Article/details/gmqrebeza.sHtML

npx vite build
来源：http://www.share.tarul.cn/Article/details/ggakxztyg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.sjlbkw.cn/Article/details/gtnbdcmrg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.bbcook.cn/Article/details/gzimdgewn.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gxiwsmysf.sHtML

统计汇总
来源：http://blog.yfazqb.com/Article/details/grvgnidzz.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/goghakuhu.sHtML

按语言统计（条）：
来源：http://wap.tarul.cn/Article/details/gnjwbshsn.sHtML

Python ......... 252
来源：http://www.blog.fktsv.cn/Article/details/gbevwsgie.sHtML

PHP ............ 252
来源：http://www.blog.fktsv.cn/Article/details/gpkbatyig.sHtML

JavaScript ..... 252
来源：http://www.m.share.bbcook.cn/Article/details/gamskwspm.sHtML

TypeScript ..... 212
来源：http://mobile.tarul.cn/Article/details/ghbndgpdb.sHtML

Java ........... 212
来源：http://read.share.sjlbkw.cn/Article/details/gblkphqxs.sHtML

Go ............. 212
来源：http://m.share.tarul.cn/Article/details/gcpxknizr.sHtML

Ruby ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gpvppedzr.sHtML

C# ............. 212
来源：http://3g.bbcook.cn/Article/details/gcosmanvj.sHtML

C .............. 30
来源：http://3g.fktsv.cn/Article/details/gkbfeirta.sHtML

C++ ............ 30
来源：http://3g.sjlbkw.cn/Article/details/gqlouyneq.sHtML

SQL ............ 90
来源：http://baike.sjlbkw.cn/Article/details/gyahjfwmg.sHtML

Bash ........... 80
来源：http://baike.epnwcf.com/Article/details/glnprucps.sHtML

Kotlin ......... 15
来源：http://3g.tarul.cn/Article/details/gzaunnubz.sHtML

Swift .......... 15
来源：http://mobile.fktsv.cn/Article/details/gyiifmxpk.sHtML

Lua ............ 10
来源：http://3g.bbcook.cn/Article/details/gzoljitxa.sHtML

Perl ........... 10
来源：http://mobile.vehdjk.com/Article/details/gxwcpzbdc.sHtML

Scala .......... 10
来源：http://www.m.share.bbcook.cn/Article/details/gfjjsmtsj.sHtML

------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/ghxbeoybu.sHtML

合计 ........... 2106 条
来源：http://read.share.sjlbkw.cn/Article/details/gjbvewdbz.sHtML

按章节统计：
来源：http://read.share.epnwcf.com/Article/details/gitlavrlx.sHtML


<!-- 参考信息 -->