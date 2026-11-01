代发 wailian999

[T49] Perl：函数
来源：http://www.blog.fktsv.cn/Article/details/gbpdzqsca.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gngbnhlvl.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gttylvbwz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fktsv.cn/Article/details/gujgksyon.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.vehdjk.com/Article/details/gbncnqlrj.sHtML

[T51] Scala：Hello World
来源：http://3g.tarul.cn/Article/details/geccthaap.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gtnqztgbu.sHtML

[T52] Scala：变量
来源：http://www.m.share.epnwcf.com/Article/details/gdgukzyrn.sHtML

val a = 1;  var b = 2
来源：http://blog.fktsv.cn/Article/details/gzvyxhetc.sHtML

[T53] Scala：字符串插值
来源：http://baike.fktsv.cn/Article/details/gcczxyppe.sHtML

s"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gwqigvxrn.sHtML

[T54] Scala：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/grzwyfhra.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.tarul.cn/Article/details/gouwgmhuk.sHtML

[T55] Scala：集合过滤
来源：http://blog.tarul.cn/Article/details/gnfxlcgno.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.sjlbkw.cn/Article/details/gqizworkc.sHtML

[T56] Scala：样例类
来源：http://www.blog.bbcook.cn/Article/details/gqihjtain.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gkqlsoddk.sHtML

[T57] Scala：模式匹配
来源：http://www.share.tarul.cn/Article/details/gagzffruk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.tarul.cn/Article/details/gpdujaqvj.sHtML

[T58] Scala：函数定义
来源：http://baike.bbcook.cn/Article/details/gkgjrcqea.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.epnwcf.com/Article/details/gllsttmfv.sHtML

[T59] Scala：循环
来源：http://3g.yfazqb.com/Article/details/gaqlvmaqx.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fktsv.cn/Article/details/gmddjnecr.sHtML

[T60] Scala：折叠
来源：http://www.share.tarul.cn/Article/details/gjnxmgbhx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.vehdjk.com/Article/details/gzcrkbyqc.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkngctuxm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.yfazqb.com/Article/details/gucfqcnmg.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxlbnebjz.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.tarul.cn/Article/details/gbwtuwatj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fktsv.cn/Article/details/ggzucmtoj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fktsv.cn/Article/details/gttptdazr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.epnwcf.com/Article/details/glhmeeuwi.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.epnwcf.com/Article/details/gxyufkpmz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gcwtrfbiy.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fktsv.cn/Article/details/gihpsgbzz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.epnwcf.com/Article/details/gohouigpf.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgbgaruw.sHtML

list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gdfmiodgl.sHtML

[U06] Py：合并两个字典
来源：http://baike.fktsv.cn/Article/details/gilmansct.sHtML

{**a, **b}
来源：http://blog.vehdjk.com/Article/details/gomqvtaie.sHtML

[U07] Py：反转字典键值
来源：http://m.share.yfazqb.com/Article/details/gcfrvhqdd.sHtML

{v: k for k, v in d.items()}
来源：http://blog.vehdjk.com/Article/details/gctbwmkgf.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fktsv.cn/Article/details/gasazryds.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gmszcdqkt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.epnwcf.com/Article/details/gjdorzffg.sHtML

max(d, key=d.get)
来源：http://read.share.fktsv.cn/Article/details/grdtlflkg.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fktsv.cn/Article/details/gtxtkyxne.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.epnwcf.com/Article/details/gdiiopclo.sHtML

[U11] Py：生成器表达式
来源：http://blog.bbcook.cn/Article/details/gkiptqytq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fktsv.cn/Article/details/gxccbtbar.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.sjlbkw.cn/Article/details/gpclcwgzg.sHtML

Counter(arr).most_common(3)
来源：http://blog.bbcook.cn/Article/details/gnoguowvo.sHtML

[U13] Py：固定长度队列
来源：http://m.share.bbcook.cn/Article/details/glxxmegxj.sHtML

deque(maxlen=10)
来源：http://m.share.sjlbkw.cn/Article/details/gqzqwawlg.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.epnwcf.com/Article/details/ghjrlixon.sHtML

defaultdict(list)
来源：http://baike.yfazqb.com/Article/details/gcybvlrzk.sHtML

[U15] Py：高精度计时
来源：http://www.share.sjlbkw.cn/Article/details/gwgzwcqlg.sHtML

t = time.perf_counter()
来源：http://www.m.share.tarul.cn/Article/details/gapzrnxmu.sHtML

[U16] Py：命令行参数解析
来源：http://blog.bbcook.cn/Article/details/gzmjdlufc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.bbcook.cn/Article/details/gwqfmdrif.sHtML

[U17] Py：初始化日志
来源：http://baike.tarul.cn/Article/details/gjjpvzwgo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.bbcook.cn/Article/details/gybhhwenn.sHtML

[U18] Py：预编译正则
来源：http://baike.vehdjk.com/Article/details/gfhqjmfvo.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.epnwcf.com/Article/details/gjuxlcjih.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.yfazqb.com/Article/details/gnxdvvolm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.epnwcf.com/Article/details/gmepfnshs.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.epnwcf.com/Article/details/gglwbhlkp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.sjlbkw.cn/Article/details/grqlovbor.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.tarul.cn/Article/details/gbqmjnnsm.sHtML

@contextlib.contextmanager
来源：http://www.m.share.bbcook.cn/Article/details/gcrwstjsj.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fktsv.cn/Article/details/gzeiyadew.sHtML

list(zip(*m))
来源：http://read.share.fktsv.cn/Article/details/gifmygzgs.sHtML

[U23] Py：分块读取大文件
来源：http://wap.bbcook.cn/Article/details/gprjmigsi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.bbcook.cn/Article/details/gynzooqpz.sHtML

[U24] Py：路径操作
来源：http://wap.vehdjk.com/Article/details/gvdpxndls.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/grlodosfg.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.epnwcf.com/Article/details/gkrsbafmp.sHtML

csv.DictReader(f)
来源：http://read.share.tarul.cn/Article/details/gychhucqo.sHtML

[U26] Py：并发下载
来源：http://wap.yfazqb.com/Article/details/gbqyamjxq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.tarul.cn/Article/details/gjgvfhyxr.sHtML

[U27] Py：异步 HTTP
来源：http://baike.vehdjk.com/Article/details/gtcoqhyux.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.vehdjk.com/Article/details/gsbdxvywq.sHtML

[U28] Py：类型别名
来源：http://3g.vehdjk.com/Article/details/ggimthzqt.sHtML

UserId = int
来源：http://m.share.yfazqb.com/Article/details/gbfsgntri.sHtML

[U29] Py：属性校验
来源：http://wap.fktsv.cn/Article/details/ghygxcbpb.sHtML

@property 与 @x.setter 配合
来源：http://www.share.sjlbkw.cn/Article/details/gxtpjnpbl.sHtML

[U30] Py：数据类
来源：http://www.blog.tarul.cn/Article/details/gzmvyjbmw.sHtML

@dataclass(slots=True)
来源：http://m.share.tarul.cn/Article/details/goqwjuhpc.sHtML

[U31] Py：单测
来源：http://www.share.epnwcf.com/Article/details/gtxfkhwlh.sHtML

python -m pytest -q
来源：http://baike.fktsv.cn/Article/details/gamhfaokh.sHtML

[U32] Py：代码格式化
来源：http://mobile.vehdjk.com/Article/details/gyradmwsx.sHtML

ruff format . && ruff check --fix .
来源：http://blog.sjlbkw.cn/Article/details/gddkmkyti.sHtML

[U33] Py：打包发布
来源：http://3g.bbcook.cn/Article/details/ghlgjrkoi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.sjlbkw.cn/Article/details/gsryyptfc.sHtML

[U34] Py：判断编码
来源：http://m.share.sjlbkw.cn/Article/details/gxatsjhcp.sHtML

chardet.detect(raw)
来源：http://baike.sjlbkw.cn/Article/details/ggnxomblj.sHtML

[U35] Py：发送邮件
来源：http://read.share.yfazqb.com/Article/details/gdxrrxfqv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.bbcook.cn/Article/details/gdszydbga.sHtML

[U36] Py：定时任务
来源：http://www.share.yfazqb.com/Article/details/gxkyiybji.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fktsv.cn/Article/details/ggtidhvsm.sHtML

[U37] Py：读写 Excel
来源：http://wap.tarul.cn/Article/details/gafeamjyr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.epnwcf.com/Article/details/grszkanti.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.bbcook.cn/Article/details/gagzhhiun.sHtML

Path(__file__).resolve().parent
来源：http://wap.fktsv.cn/Article/details/gobywnyvo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.yfazqb.com/Article/details/ghptqslet.sHtML

sys.stdout.isatty()
来源：http://read.share.bbcook.cn/Article/details/gmogzqvrs.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.yfazqb.com/Article/details/gdnalljwb.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/gqjqyxcpp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.bbcook.cn/Article/details/ggfexvfmn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.sjlbkw.cn/Article/details/gigvrrllq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.epnwcf.com/Article/details/gqgyliyzn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.yfazqb.com/Article/details/gdctldrqx.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.tarul.cn/Article/details/ghycvlilk.sHtML

namespace App\Http;
来源：http://wap.bbcook.cn/Article/details/gfyumgwhy.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.bbcook.cn/Article/details/ghiuythpv.sHtML

declare(strict_types=1);
来源：http://3g.bbcook.cn/Article/details/gjlyfuzcf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.yfazqb.com/Article/details/gnhdoquiy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gnzqsncvi.sHtML

[U46] PHP：可空类型
来源：http://wap.fktsv.cn/Article/details/gioqginkc.sHtML

?string $name = null
来源：http://www.blog.sjlbkw.cn/Article/details/gzlockura.sHtML

[U47] PHP：联合类型
来源：http://blog.sjlbkw.cn/Article/details/ggejbhrde.sHtML

int|string $id
来源：http://read.share.epnwcf.com/Article/details/gghofihse.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.epnwcf.com/Article/details/gmelabzfw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.vehdjk.com/Article/details/grjjjhbdb.sHtML

[U49] PHP：只读属性
来源：http://baike.tarul.cn/Article/details/gijhhyisd.sHtML

public readonly string $name
来源：http://blog.sjlbkw.cn/Article/details/gvivcxnkz.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.sjlbkw.cn/Article/details/gnyyjyjpn.sHtML

public function __construct(private int $id) {}
来源：http://3g.tarul.cn/Article/details/gmydgvwai.sHtML

[U51] PHP：数组解构
来源：http://m.share.tarul.cn/Article/details/gllbtbuxd.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/gauunhphg.sHtML

[U52] PHP：箭头函数
来源：http://baike.fktsv.cn/Article/details/gderubxvz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.bbcook.cn/Article/details/gltowxfhi.sHtML

[U53] PHP：空合并运算符
来源：http://blog.vehdjk.com/Article/details/gpyfvmfuy.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.vehdjk.com/Article/details/gpgjgxmpq.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.bbcook.cn/Article/details/gggltxmyt.sHtML

$obj?->method()
来源：http://baike.tarul.cn/Article/details/gabwxmynx.sHtML

[U55] PHP：match 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gtcplixek.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.tarul.cn/Article/details/gbbpkmufw.sHtML

[U56] PHP：命名参数
来源：http://mobile.sjlbkw.cn/Article/details/gguttglwt.sHtML

f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/guqfyasnq.sHtML

[U57] PHP：字符串插值
来源：http://blog.tarul.cn/Article/details/gkupmeapk.sHtML

"值: {$a}"
来源：http://m.share.bbcook.cn/Article/details/gjjqckcbq.sHtML

[U58] PHP：数组三件套
来源：http://baike.tarul.cn/Article/details/gierlbkgs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.yfazqb.com/Article/details/ggpprwjex.sHtML

[U59] PHP：自定义排序
来源：http://mobile.vehdjk.com/Article/details/gcocohbyq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.vehdjk.com/Article/details/gbgnyrjza.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.epnwcf.com/Article/details/gmmzqivwo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.tarul.cn/Article/details/gtfsivdcd.sHtML

[U61] PHP：正则
来源：http://baike.fktsv.cn/Article/details/gmwttergx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/grhjrtils.sHtML

[U62] PHP：日期对象
来源：http://read.share.epnwcf.com/Article/details/gvbupwmtx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.yfazqb.com/Article/details/ghygeviza.sHtML

[U63] PHP：文件读写
来源：http://m.share.bbcook.cn/Article/details/gpfnjnflp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.tarul.cn/Article/details/gcpqgxuzt.sHtML

[U64] PHP：目录遍历
来源：http://wap.sjlbkw.cn/Article/details/gxtizujhp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.bbcook.cn/Article/details/gviyxwydf.sHtML

[U65] PHP：会话
来源：http://mobile.fktsv.cn/Article/details/gwiwmbcqp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.tarul.cn/Article/details/gqhfscumf.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.sjlbkw.cn/Article/details/gsldziblk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.sjlbkw.cn/Article/details/gaexgdabv.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.vehdjk.com/Article/details/gunzhkwln.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.yfazqb.com/Article/details/gzqiibtnt.sHtML

[U68] PHP：PDO 连接
来源：http://3g.bbcook.cn/Article/details/glpkydsjx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.bbcook.cn/Article/details/gysncklgy.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.bbcook.cn/Article/details/gxwnbadyi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.epnwcf.com/Article/details/ggjtxnncd.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.vehdjk.com/Article/details/gkopxxcmw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.vehdjk.com/Article/details/gxkrgflhk.sHtML

[U71] PHP：抛出异常
来源：http://mobile.vehdjk.com/Article/details/gjayetczd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/gkaoihsdu.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fktsv.cn/Article/details/grlvpwvrp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.vehdjk.com/Article/details/gswuiaavq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.tarul.cn/Article/details/gevrtdvit.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.bbcook.cn/Article/details/gmuzfqxsy.sHtML

[U74] PHP：读取环境变量
来源：http://blog.yfazqb.com/Article/details/geygtiyfq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.yfazqb.com/Article/details/gqxgtoudw.sHtML

[U75] PHP：依赖注入
来源：http://mobile.bbcook.cn/Article/details/gifrkewut.sHtML

composer require psr/container
来源：http://www.share.vehdjk.com/Article/details/gepdyloxv.sHtML

[U76] PHP：简单路由
来源：http://3g.yfazqb.com/Article/details/guumamxcv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.yfazqb.com/Article/details/glzyzlngg.sHtML

[U77] PHP：模板渲染
来源：http://www.share.yfazqb.com/Article/details/gcupavjdk.sHtML

composer require twig/twig
来源：http://baike.vehdjk.com/Article/details/gpwgkfzhg.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gcsghalkc.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.bbcook.cn/Article/details/ggmxyjknt.sHtML

[U79] PHP：静态分析
来源：http://baike.sjlbkw.cn/Article/details/gzbibtwgo.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.yfazqb.com/Article/details/gzcjsllnr.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.vehdjk.com/Article/details/gpostnagj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.vehdjk.com/Article/details/gtdfkitza.sHtML

[U81] JS：初始化项目
来源：http://m.share.bbcook.cn/Article/details/gbowxgfyu.sHtML

npm init -y;  npm i express
来源：http://www.m.share.vehdjk.com/Article/details/gqbgpolck.sHtML

[U82] JS：package.json 脚本
来源：http://blog.epnwcf.com/Article/details/giqbtgajy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.tarul.cn/Article/details/grgejkxer.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.epnwcf.com/Article/details/gbgzsxkur.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/goyjviqto.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.epnwcf.com/Article/details/gcndfrnhb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.vehdjk.com/Article/details/grvprtjwh.sHtML

[U85] JS：可选链
来源：http://www.blog.epnwcf.com/Article/details/gytifiuik.sHtML

a?.b?.c
来源：http://m.share.tarul.cn/Article/details/gmbjjylto.sHtML

[U86] JS：空值合并
来源：http://mobile.fktsv.cn/Article/details/glnvqvhuq.sHtML

a ?? b
来源：http://read.share.bbcook.cn/Article/details/gqqyniibf.sHtML

[U87] JS：解构默认值
来源：http://3g.tarul.cn/Article/details/gmkfavxxu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.yfazqb.com/Article/details/ggyusrtao.sHtML

[U88] JS：对象展开合并
来源：http://mobile.tarul.cn/Article/details/ghazpwhml.sHtML

{ ...a, ...b }
来源：http://m.share.bbcook.cn/Article/details/gjjwlxvrd.sHtML

[U89] JS：数组去重
来源：http://www.share.tarul.cn/Article/details/gqvronjok.sHtML

[...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gnxekprhd.sHtML

[U90] JS：数字数组排序
来源：http://www.share.sjlbkw.cn/Article/details/gxgcpjsud.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gtodfhksl.sHtML

[U91] JS：对象键值遍历
来源：http://3g.bbcook.cn/Article/details/givbuqkzh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.tarul.cn/Article/details/giqlcxlax.sHtML

[U92] JS：深拷贝
来源：http://3g.vehdjk.com/Article/details/gaweetepf.sHtML

structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gmrowxknb.sHtML

[U93] JS：模板字符串
来源：http://3g.epnwcf.com/Article/details/gjympwods.sHtML

`共 ${n} 条`
来源：http://3g.epnwcf.com/Article/details/gblswipnv.sHtML

[U94] JS：箭头函数
来源：http://wap.yfazqb.com/Article/details/gnooitnet.sHtML

const double = x => x * 2;
来源：http://read.share.epnwcf.com/Article/details/gdvafwwgo.sHtML

[U95] JS：Promise 包装
来源：http://wap.fktsv.cn/Article/details/gpcqfqsro.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.tarul.cn/Article/details/gkbdceisl.sHtML

[U96] JS：async/await 与异常
来源：http://wap.sjlbkw.cn/Article/details/gycmgpyqz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gdjpkwyxw.sHtML

[U97] JS：并发请求
来源：http://mobile.vehdjk.com/Article/details/geeqjhjyp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gorvemeal.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gznpqmpgy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.epnwcf.com/Article/details/gujiwbyrf.sHtML

[U99] JS：事件监听
来源：http://mobile.yfazqb.com/Article/details/gvmnyjpye.sHtML

el.addEventListener("click", e => {})
来源：http://blog.tarul.cn/Article/details/goiqcgify.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.vehdjk.com/Article/details/gaxwkfetl.sHtML

document.querySelector(".item")
来源：http://wap.sjlbkw.cn/Article/details/gjgaazick.sHtML

[U101] JS：classList 操作
来源：http://read.share.bbcook.cn/Article/details/gfywxdnod.sHtML

el.classList.toggle("active")
来源：http://baike.tarul.cn/Article/details/gvrhgfsfm.sHtML

[U102] JS：本地存储
来源：http://m.share.yfazqb.com/Article/details/gzoqbbibh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fktsv.cn/Article/details/gzhlvuxzl.sHtML

[U103] JS：定时器
来源：http://m.share.bbcook.cn/Article/details/gotugbhti.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fktsv.cn/Article/details/gqxofwynz.sHtML

[U104] JS：防抖
来源：http://mobile.epnwcf.com/Article/details/gtlysupox.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gmrjuhxxy.sHtML

[U105] JS：节流
来源：http://3g.fktsv.cn/Article/details/gonbxnlcl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gbuiganus.sHtML

[U106] JS：日期格式化
来源：http://www.share.vehdjk.com/Article/details/gdyradovw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.vehdjk.com/Article/details/gittryoiy.sHtML

[U107] JS：数字千分位
来源：http://m.share.tarul.cn/Article/details/gbbzwbpes.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.epnwcf.com/Article/details/gslotqmoz.sHtML

[U108] JS：随机整数
来源：http://read.share.sjlbkw.cn/Article/details/gdounfzds.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.bbcook.cn/Article/details/gvwvdckvw.sHtML

[U109] JS：数组分组
来源：http://baike.bbcook.cn/Article/details/gdxeorzki.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gdsymejpf.sHtML

[U110] JS：数组分块
来源：http://wap.sjlbkw.cn/Article/details/gtytkmozg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.sjlbkw.cn/Article/details/gcfegoopy.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.tarul.cn/Article/details/gjfzdpryi.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fktsv.cn/Article/details/gukxjmbej.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.tarul.cn/Article/details/ggpprusgo.sHtML

"7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gjnlvqwof.sHtML

[U113] JS：正则替换全部
来源：http://blog.vehdjk.com/Article/details/gbemfmpii.sHtML

s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gtpxsanlh.sHtML

[U114] JS：JSON 深比较
来源：http://wap.yfazqb.com/Article/details/ghqhjktwg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.yfazqb.com/Article/details/gvgbjbrxf.sHtML

[U115] JS：生成 UUID
来源：http://baike.yfazqb.com/Article/details/gmapqxqqu.sHtML

crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gqiimujez.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.vehdjk.com/Article/details/gpvwtzhpe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.vehdjk.com/Article/details/gcireqpkw.sHtML

[U117] JS：单元测试
来源：http://baike.epnwcf.com/Article/details/ghdqeldox.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.bbcook.cn/Article/details/gkrvrjqus.sHtML

[U118] JS：开发服务器
来源：http://baike.bbcook.cn/Article/details/gztcbdepc.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fktsv.cn/Article/details/gmwlscber.sHtML

[U119] JS：生产构建
来源：http://www.blog.sjlbkw.cn/Article/details/gjwkckzvt.sHtML

npx vite build
来源：http://www.blog.bbcook.cn/Article/details/gobufbwlt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.bbcook.cn/Article/details/gqzpeohuk.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.sjlbkw.cn/Article/details/gpdiukcum.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghatclhlt.sHtML

统计汇总
来源：http://baike.yfazqb.com/Article/details/gjykjmzjf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gxnmmmhhm.sHtML

按语言统计（条）：
来源：http://wap.tarul.cn/Article/details/gfmfznzyh.sHtML

Python ......... 252
来源：http://m.share.bbcook.cn/Article/details/gpialhrsq.sHtML

PHP ............ 252
来源：http://www.share.tarul.cn/Article/details/ghwwnvrpi.sHtML

JavaScript ..... 252
来源：http://read.share.vehdjk.com/Article/details/gbnsfyxim.sHtML

TypeScript ..... 212
来源：http://3g.epnwcf.com/Article/details/gxggkauab.sHtML

Java ........... 212
来源：http://baike.bbcook.cn/Article/details/gifxxvhft.sHtML

Go ............. 212
来源：http://wap.fktsv.cn/Article/details/gampadjts.sHtML

Ruby ........... 212
来源：http://baike.epnwcf.com/Article/details/gxltnwxca.sHtML

C# ............. 212
来源：http://read.share.vehdjk.com/Article/details/gvmxvrmpf.sHtML

C .............. 30
来源：http://read.share.fktsv.cn/Article/details/gvkfuaipg.sHtML

C++ ............ 30
来源：http://www.blog.bbcook.cn/Article/details/gsunsbker.sHtML

SQL ............ 90
来源：http://blog.fktsv.cn/Article/details/gvxmebggt.sHtML

Bash ........... 80
来源：http://www.blog.epnwcf.com/Article/details/gxyhdetlv.sHtML

Kotlin ......... 15
来源：http://wap.fktsv.cn/Article/details/glmpppbid.sHtML

Swift .......... 15
来源：http://baike.yfazqb.com/Article/details/gapqrrblq.sHtML

Lua ............ 10
来源：http://blog.epnwcf.com/Article/details/gbvmxoqfa.sHtML

Perl ........... 10
来源：http://www.share.yfazqb.com/Article/details/gavnlshqs.sHtML

Scala .......... 10
来源：http://m.share.tarul.cn/Article/details/gznfmfxmb.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gqayfrhph.sHtML

合计 ........... 2106 条
来源：http://www.blog.yfazqb.com/Article/details/gdfhuuqat.sHtML

按章节统计：
来源：http://www.m.share.bbcook.cn/Article/details/gogaguujq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.epnwcf.com/Article/details/grogjgssb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/guvhsldms.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/gltrycbpk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.yfazqb.com/Article/details/ghmpjskft.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fktsv.cn/Article/details/gcyqysuve.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fktsv.cn/Article/details/gujussnpb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/geqnbpsvu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fktsv.cn/Article/details/gvldtpdoh.sHtML


<!-- 参考信息 -->