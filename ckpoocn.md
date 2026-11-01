代发 wailian999

[T47] Perl：正则捕获
来源：http://baike.bbcook.cn/Article/details/gsbnjismz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.yfazqb.com/Article/details/gpyjyjdsy.sHtML

[T48] Perl：正则替换
来源：http://blog.yfazqb.com/Article/details/gwebgqdud.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fktsv.cn/Article/details/gmumztgne.sHtML

[T49] Perl：函数
来源：http://www.m.share.fktsv.cn/Article/details/gzasseiit.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gciiatfdg.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gorpzbvdj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fktsv.cn/Article/details/gowjiinfq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fktsv.cn/Article/details/gpnujonbr.sHtML

[T51] Scala：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gqopmfbee.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gpjofcsip.sHtML

[T52] Scala：变量
来源：http://m.share.fktsv.cn/Article/details/gkfrdumqa.sHtML

val a = 1;  var b = 2
来源：http://www.blog.bbcook.cn/Article/details/glgctqwhq.sHtML

[T53] Scala：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gjvepebil.sHtML

s"值: $b"
来源：http://blog.vehdjk.com/Article/details/gghnpudki.sHtML

[T54] Scala：集合映射
来源：http://baike.fktsv.cn/Article/details/gtkogbafy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.bbcook.cn/Article/details/gmoomhkal.sHtML

[T55] Scala：集合过滤
来源：http://blog.fktsv.cn/Article/details/gnrebdfum.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fktsv.cn/Article/details/gtmdlqpmk.sHtML

[T56] Scala：样例类
来源：http://m.share.vehdjk.com/Article/details/gmkyhinlk.sHtML

case class User(name: String, age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gvlwfxlpw.sHtML

[T57] Scala：模式匹配
来源：http://wap.tarul.cn/Article/details/geokcwvoh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.sjlbkw.cn/Article/details/giesmyxuf.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.bbcook.cn/Article/details/gsnlhdgio.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.tarul.cn/Article/details/goajalnsa.sHtML

[T59] Scala：循环
来源：http://www.blog.yfazqb.com/Article/details/gtjieydlg.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.tarul.cn/Article/details/gobnzqqrr.sHtML

[T60] Scala：折叠
来源：http://baike.vehdjk.com/Article/details/gqlpjzpqb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fktsv.cn/Article/details/gdsopxfvm.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxlvmopmt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.epnwcf.com/Article/details/geqeoqpac.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grghwxodz.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.vehdjk.com/Article/details/gxjpzovyv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.epnwcf.com/Article/details/gfikyzssy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.tarul.cn/Article/details/gtfltflsi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.tarul.cn/Article/details/gujjzsigs.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.vehdjk.com/Article/details/gzulfsgzq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fktsv.cn/Article/details/golwlpher.sHtML

[U04] Py：变量调试打印
来源：http://blog.fktsv.cn/Article/details/gneiznhwz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.vehdjk.com/Article/details/gpmibcrjz.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fktsv.cn/Article/details/giqhanpgr.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/gcqiqouqg.sHtML

[U06] Py：合并两个字典
来源：http://3g.bbcook.cn/Article/details/gpwvzitek.sHtML

{**a, **b}
来源：http://mobile.tarul.cn/Article/details/glfqkodho.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.yfazqb.com/Article/details/gcfvmeynx.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.bbcook.cn/Article/details/gbbjahivl.sHtML

[U08] Py：展平二维列表
来源：http://baike.yfazqb.com/Article/details/gsvttxobb.sHtML

[y for x in nested for y in x]
来源：http://blog.bbcook.cn/Article/details/gljsiawmg.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.bbcook.cn/Article/details/geznyhsci.sHtML

max(d, key=d.get)
来源：http://baike.fktsv.cn/Article/details/gzdxoswis.sHtML

[U10] Py：按值排序字典
来源：http://m.share.sjlbkw.cn/Article/details/gkumxnqor.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fktsv.cn/Article/details/gtygazrey.sHtML

[U11] Py：生成器表达式
来源：http://baike.yfazqb.com/Article/details/gkkmuhmts.sHtML

(x * 2 for x in arr)
来源：http://www.share.sjlbkw.cn/Article/details/gnoapmpqp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.epnwcf.com/Article/details/gmqftkzvn.sHtML

Counter(arr).most_common(3)
来源：http://baike.epnwcf.com/Article/details/ggcdmgiuv.sHtML

[U13] Py：固定长度队列
来源：http://baike.fktsv.cn/Article/details/gtqxetndh.sHtML

deque(maxlen=10)
来源：http://mobile.vehdjk.com/Article/details/grofyydtv.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fktsv.cn/Article/details/gpvjddqkn.sHtML

defaultdict(list)
来源：http://www.share.yfazqb.com/Article/details/ghchlwohk.sHtML

[U15] Py：高精度计时
来源：http://mobile.sjlbkw.cn/Article/details/gtmhraahb.sHtML

t = time.perf_counter()
来源：http://m.share.tarul.cn/Article/details/gwgasfdsw.sHtML

[U16] Py：命令行参数解析
来源：http://blog.epnwcf.com/Article/details/gcolknnpe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.yfazqb.com/Article/details/gjfcllzst.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.vehdjk.com/Article/details/gofufdgfr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.bbcook.cn/Article/details/gmudellpt.sHtML

[U18] Py：预编译正则
来源：http://www.blog.yfazqb.com/Article/details/gtolufllq.sHtML

pat = re.compile(r"\d+")
来源：http://baike.vehdjk.com/Article/details/gugoracfh.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.tarul.cn/Article/details/gtaecfvzc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fktsv.cn/Article/details/gkdohkujc.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.vehdjk.com/Article/details/ghhpjiggv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.tarul.cn/Article/details/gvajmdufh.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.vehdjk.com/Article/details/gtwykplzt.sHtML

@contextlib.contextmanager
来源：http://wap.tarul.cn/Article/details/ghuujlrgv.sHtML

[U22] Py：矩阵转置
来源：http://read.share.yfazqb.com/Article/details/ghjsbbvfa.sHtML

list(zip(*m))
来源：http://read.share.yfazqb.com/Article/details/gsdsihjgh.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.bbcook.cn/Article/details/gfzctsmxo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.epnwcf.com/Article/details/gqqlaktou.sHtML

[U24] Py：路径操作
来源：http://www.share.epnwcf.com/Article/details/gwcsufdqf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gzkinbcqs.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.epnwcf.com/Article/details/gohvshnmm.sHtML

csv.DictReader(f)
来源：http://www.share.vehdjk.com/Article/details/gwvfgkpkp.sHtML

[U26] Py：并发下载
来源：http://www.share.epnwcf.com/Article/details/giicmzcnu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fktsv.cn/Article/details/gazrmxykk.sHtML

[U27] Py：异步 HTTP
来源：http://3g.vehdjk.com/Article/details/gkojwngum.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.bbcook.cn/Article/details/gyhtdsrin.sHtML

[U28] Py：类型别名
来源：http://3g.yfazqb.com/Article/details/gzowfrjwf.sHtML

UserId = int
来源：http://m.share.epnwcf.com/Article/details/gcdfjvmad.sHtML

[U29] Py：属性校验
来源：http://blog.tarul.cn/Article/details/ghfddmvkl.sHtML

@property 与 @x.setter 配合
来源：http://baike.tarul.cn/Article/details/gitvzxipj.sHtML

[U30] Py：数据类
来源：http://read.share.bbcook.cn/Article/details/gfblbyaqm.sHtML

@dataclass(slots=True)
来源：http://read.share.tarul.cn/Article/details/gaynymcsi.sHtML

[U31] Py：单测
来源：http://m.share.fktsv.cn/Article/details/gthsheiav.sHtML

python -m pytest -q
来源：http://3g.vehdjk.com/Article/details/gigqiulkm.sHtML

[U32] Py：代码格式化
来源：http://read.share.yfazqb.com/Article/details/gpwihvijx.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fktsv.cn/Article/details/gvwkdtnih.sHtML

[U33] Py：打包发布
来源：http://www.blog.bbcook.cn/Article/details/gyfuhcbue.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.yfazqb.com/Article/details/gjhpyayja.sHtML

[U34] Py：判断编码
来源：http://baike.bbcook.cn/Article/details/girgeytsy.sHtML

chardet.detect(raw)
来源：http://www.share.tarul.cn/Article/details/gfosygugh.sHtML

[U35] Py：发送邮件
来源：http://mobile.bbcook.cn/Article/details/gvlqxneyr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.epnwcf.com/Article/details/gwepkpavk.sHtML

[U36] Py：定时任务
来源：http://wap.bbcook.cn/Article/details/gpbiklrqw.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.vehdjk.com/Article/details/glkjbdgwz.sHtML

[U37] Py：读写 Excel
来源：http://baike.fktsv.cn/Article/details/ghntohanj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.vehdjk.com/Article/details/gmzghmqnd.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.sjlbkw.cn/Article/details/gjbzsywmo.sHtML

Path(__file__).resolve().parent
来源：http://blog.yfazqb.com/Article/details/glttnjgxw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.vehdjk.com/Article/details/gsxnidexl.sHtML

sys.stdout.isatty()
来源：http://mobile.bbcook.cn/Article/details/gtemwtebf.sHtML

[U40] Py：打印到标准错误
来源：http://wap.yfazqb.com/Article/details/gmzrxsvvj.sHtML

print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/gefurxjga.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.bbcook.cn/Article/details/gufeyjpoc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.bbcook.cn/Article/details/gkdiarpno.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.yfazqb.com/Article/details/gggsvkvni.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.bbcook.cn/Article/details/govdvbtem.sHtML

[U43] PHP：声明命名空间
来源：http://wap.yfazqb.com/Article/details/gatrisbsu.sHtML

namespace App\Http;
来源：http://www.share.bbcook.cn/Article/details/gknfttsmw.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fktsv.cn/Article/details/gzaaepxpw.sHtML

declare(strict_types=1);
来源：http://blog.yfazqb.com/Article/details/gdjpznwfg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.bbcook.cn/Article/details/gsodtxvpj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gsdxbnwaw.sHtML

[U46] PHP：可空类型
来源：http://m.share.yfazqb.com/Article/details/gugaazbad.sHtML

?string $name = null
来源：http://m.share.fktsv.cn/Article/details/gbrgrjwlc.sHtML

[U47] PHP：联合类型
来源：http://baike.bbcook.cn/Article/details/gnlrfmhqo.sHtML

int|string $id
来源：http://www.m.share.sjlbkw.cn/Article/details/gxznfhdaz.sHtML

[U48] PHP：纯枚举
来源：http://3g.yfazqb.com/Article/details/gfviprczm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.yfazqb.com/Article/details/gihkgtmxl.sHtML

[U49] PHP：只读属性
来源：http://blog.epnwcf.com/Article/details/ghucanyve.sHtML

public readonly string $name
来源：http://wap.tarul.cn/Article/details/gmxrgvfix.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.vehdjk.com/Article/details/ghduuunaq.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.bbcook.cn/Article/details/grhzfsjih.sHtML

[U51] PHP：数组解构
来源：http://blog.fktsv.cn/Article/details/gnbehmokz.sHtML

[$a, $b] = $arr;
来源：http://www.share.yfazqb.com/Article/details/gqdmxaxmi.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.vehdjk.com/Article/details/gimgqxaqj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.bbcook.cn/Article/details/ghwmaxkhu.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.tarul.cn/Article/details/gkoqnuowy.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.vehdjk.com/Article/details/ghiglwmmf.sHtML

[U54] PHP：空安全调用
来源：http://baike.sjlbkw.cn/Article/details/gulvnlscw.sHtML

$obj?->method()
来源：http://3g.sjlbkw.cn/Article/details/gumqshnue.sHtML

[U55] PHP：match 表达式
来源：http://blog.vehdjk.com/Article/details/gasixqaqt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.tarul.cn/Article/details/ghfbwklet.sHtML

[U56] PHP：命名参数
来源：http://m.share.yfazqb.com/Article/details/gjuvjgtuw.sHtML

f(a: 1, b: 2)
来源：http://baike.vehdjk.com/Article/details/gienxjvgj.sHtML

[U57] PHP：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gasfqwwop.sHtML

"值: {$a}"
来源：http://3g.tarul.cn/Article/details/gjyfdbdwz.sHtML

[U58] PHP：数组三件套
来源：http://m.share.vehdjk.com/Article/details/gmfeoatok.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.tarul.cn/Article/details/gyybasbve.sHtML

[U59] PHP：自定义排序
来源：http://blog.bbcook.cn/Article/details/gjygscskb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.sjlbkw.cn/Article/details/gymoetubq.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.bbcook.cn/Article/details/gkyghzemk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.tarul.cn/Article/details/gxqdtyrwz.sHtML

[U61] PHP：正则
来源：http://blog.epnwcf.com/Article/details/govvtdxzb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gpaggpyka.sHtML

[U62] PHP：日期对象
来源：http://3g.fktsv.cn/Article/details/guiemfcuf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fktsv.cn/Article/details/gchwdrxtc.sHtML

[U63] PHP：文件读写
来源：http://wap.epnwcf.com/Article/details/geyzqtaer.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.bbcook.cn/Article/details/gipmpnryj.sHtML

[U64] PHP：目录遍历
来源：http://baike.fktsv.cn/Article/details/gqzoxfkso.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.epnwcf.com/Article/details/gywxmwfvu.sHtML

[U65] PHP：会话
来源：http://m.share.fktsv.cn/Article/details/gxnlccqws.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.yfazqb.com/Article/details/gvenpxgqc.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.vehdjk.com/Article/details/gzsnwglyf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fktsv.cn/Article/details/gqbooxcfw.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.sjlbkw.cn/Article/details/gkxwotmyy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.epnwcf.com/Article/details/gxoeuchqo.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.vehdjk.com/Article/details/gbjvjwket.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.vehdjk.com/Article/details/gwrjhmmor.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fktsv.cn/Article/details/gozsnjmdi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fktsv.cn/Article/details/gcmabjvcq.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.sjlbkw.cn/Article/details/gyvjsbruf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.tarul.cn/Article/details/gtakrhfkp.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.tarul.cn/Article/details/ggjpqmauo.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.bbcook.cn/Article/details/gtcxtptdh.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.bbcook.cn/Article/details/gpejvrmyq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.vehdjk.com/Article/details/gblaysacd.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.bbcook.cn/Article/details/gaswqkvho.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.tarul.cn/Article/details/gdtuxvsrd.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gqdzytegl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fktsv.cn/Article/details/gepxioauf.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.yfazqb.com/Article/details/gfzdebmlx.sHtML

composer require psr/container
来源：http://blog.epnwcf.com/Article/details/gbwyocwrb.sHtML

[U76] PHP：简单路由
来源：http://3g.epnwcf.com/Article/details/gbbfoshls.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.epnwcf.com/Article/details/gzfvarvlr.sHtML

[U77] PHP：模板渲染
来源：http://mobile.tarul.cn/Article/details/glovnuoae.sHtML

composer require twig/twig
来源：http://m.share.tarul.cn/Article/details/gtolkayuu.sHtML

[U78] PHP：单元测试
来源：http://www.share.epnwcf.com/Article/details/gigtbofil.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.sjlbkw.cn/Article/details/guwmjtufd.sHtML

[U79] PHP：静态分析
来源：http://www.share.yfazqb.com/Article/details/gsdthzbot.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.tarul.cn/Article/details/gvxeceuov.sHtML

[U80] PHP：代码规范修复
来源：http://3g.yfazqb.com/Article/details/gvnaagsby.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.yfazqb.com/Article/details/geykpnbvw.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.vehdjk.com/Article/details/gleisxixb.sHtML

npm init -y;  npm i express
来源：http://www.blog.vehdjk.com/Article/details/gwxxmcdoc.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.sjlbkw.cn/Article/details/gsidneqpq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.tarul.cn/Article/details/gkksuushx.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.vehdjk.com/Article/details/gqxgxhrvp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.vehdjk.com/Article/details/gdiphmrvt.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.epnwcf.com/Article/details/gqgcvxpbi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.bbcook.cn/Article/details/gemuwzamb.sHtML

[U85] JS：可选链
来源：http://3g.bbcook.cn/Article/details/gpnholylg.sHtML

a?.b?.c
来源：http://www.blog.yfazqb.com/Article/details/gaptmgnom.sHtML

[U86] JS：空值合并
来源：http://www.m.share.bbcook.cn/Article/details/gbhdkjcqo.sHtML

a ?? b
来源：http://3g.fktsv.cn/Article/details/gsxhjsmsy.sHtML

[U87] JS：解构默认值
来源：http://read.share.fktsv.cn/Article/details/ggyisimam.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.vehdjk.com/Article/details/gwdxssdvi.sHtML

[U88] JS：对象展开合并
来源：http://wap.bbcook.cn/Article/details/guacajckl.sHtML

{ ...a, ...b }
来源：http://m.share.bbcook.cn/Article/details/gboogtvjx.sHtML

[U89] JS：数组去重
来源：http://wap.bbcook.cn/Article/details/gyndbdgil.sHtML

[...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gqujziuqt.sHtML

[U90] JS：数字数组排序
来源：http://baike.epnwcf.com/Article/details/gopzplyza.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gnevltyce.sHtML

[U91] JS：对象键值遍历
来源：http://wap.epnwcf.com/Article/details/gjrpdcpnp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fktsv.cn/Article/details/gsdfjbirl.sHtML

[U92] JS：深拷贝
来源：http://www.blog.tarul.cn/Article/details/gyjwsyven.sHtML

structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gpwyubdad.sHtML

[U93] JS：模板字符串
来源：http://wap.bbcook.cn/Article/details/grxscigfh.sHtML

`共 ${n} 条`
来源：http://baike.sjlbkw.cn/Article/details/gbsrfpmtt.sHtML

[U94] JS：箭头函数
来源：http://wap.tarul.cn/Article/details/gaknowhgd.sHtML

const double = x => x * 2;
来源：http://mobile.bbcook.cn/Article/details/gembkfbjr.sHtML

[U95] JS：Promise 包装
来源：http://wap.bbcook.cn/Article/details/gokamrbwz.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.bbcook.cn/Article/details/gqjpiyrqs.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgaqwjoo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/glzbqzhjf.sHtML

[U97] JS：并发请求
来源：http://m.share.epnwcf.com/Article/details/gofrtdrox.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gsytfdmmy.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.yfazqb.com/Article/details/gkiuujxhq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.vehdjk.com/Article/details/gudpivmuv.sHtML

[U99] JS：事件监听
来源：http://www.share.bbcook.cn/Article/details/gbxhbzyoq.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.vehdjk.com/Article/details/gsqsuxity.sHtML

[U100] JS：DOM 查询
来源：http://read.share.yfazqb.com/Article/details/gjsqhrpbv.sHtML

document.querySelector(".item")
来源：http://m.share.epnwcf.com/Article/details/gtfmdqqdi.sHtML

[U101] JS：classList 操作
来源：http://3g.yfazqb.com/Article/details/gldqjwwqm.sHtML

el.classList.toggle("active")
来源：http://3g.tarul.cn/Article/details/gwwkxwkpc.sHtML

[U102] JS：本地存储
来源：http://m.share.tarul.cn/Article/details/gqlikkkop.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.yfazqb.com/Article/details/gyskexmjj.sHtML

[U103] JS：定时器
来源：http://m.share.vehdjk.com/Article/details/gkwhrduly.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.tarul.cn/Article/details/gialzolxb.sHtML

[U104] JS：防抖
来源：http://m.share.tarul.cn/Article/details/grtvbepqj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gltzttanv.sHtML

[U105] JS：节流
来源：http://blog.bbcook.cn/Article/details/ghjqzmpue.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.tarul.cn/Article/details/gdcfvvyrp.sHtML

[U106] JS：日期格式化
来源：http://3g.bbcook.cn/Article/details/grwumiihm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.vehdjk.com/Article/details/ghfpwdgoz.sHtML

[U107] JS：数字千分位
来源：http://mobile.vehdjk.com/Article/details/gkgjpmrhk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fktsv.cn/Article/details/gsduofqpf.sHtML

[U108] JS：随机整数
来源：http://mobile.epnwcf.com/Article/details/gesykpedr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.bbcook.cn/Article/details/gajbgjtxq.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/gqzyrgxzo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/ggjiabkoq.sHtML

[U110] JS：数组分块
来源：http://read.share.vehdjk.com/Article/details/gqdtvkjzu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.yfazqb.com/Article/details/grmztexrr.sHtML

[U111] JS：对象转 Map
来源：http://www.share.yfazqb.com/Article/details/grarvqvvx.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fktsv.cn/Article/details/gkaeufrhj.sHtML

[U112] JS：字符串补位
来源：http://baike.yfazqb.com/Article/details/gbkhxjtbh.sHtML

"7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gxduwkdmu.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.sjlbkw.cn/Article/details/gbkcmqjni.sHtML

s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gtqosjlpw.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.vehdjk.com/Article/details/gtsyqsvqv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gbslpqkay.sHtML

[U115] JS：生成 UUID
来源：http://wap.vehdjk.com/Article/details/gcgpobxmf.sHtML

crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gaenvyoyy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fktsv.cn/Article/details/gwhrhcteq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdruhsxpi.sHtML

[U117] JS：单元测试
来源：http://3g.sjlbkw.cn/Article/details/gjxgrkfdl.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.vehdjk.com/Article/details/gesrgcgoq.sHtML

[U118] JS：开发服务器
来源：http://read.share.fktsv.cn/Article/details/gbaxqfhbp.sHtML

npm i -D vite;  npx vite
来源：http://3g.vehdjk.com/Article/details/gqcqlkkzs.sHtML

[U119] JS：生产构建
来源：http://wap.epnwcf.com/Article/details/gqpywjizf.sHtML

npx vite build
来源：http://3g.fktsv.cn/Article/details/gugmiywyd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.tarul.cn/Article/details/guhbytnny.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.yfazqb.com/Article/details/gjwtelcxy.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkcmjhtnr.sHtML

统计汇总
来源：http://blog.sjlbkw.cn/Article/details/givonguvh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gmfydzewp.sHtML

按语言统计（条）：
来源：http://www.m.share.yfazqb.com/Article/details/gwjtrigyw.sHtML

Python ......... 252
来源：http://3g.sjlbkw.cn/Article/details/gkbeesady.sHtML

PHP ............ 252
来源：http://www.blog.fktsv.cn/Article/details/gkyvenssy.sHtML

JavaScript ..... 252
来源：http://baike.tarul.cn/Article/details/ghyhrovjm.sHtML

TypeScript ..... 212
来源：http://m.share.bbcook.cn/Article/details/gaqdpktot.sHtML

Java ........... 212
来源：http://www.m.share.fktsv.cn/Article/details/guvhbqijj.sHtML

Go ............. 212
来源：http://m.share.sjlbkw.cn/Article/details/gcdoggnpp.sHtML

Ruby ........... 212
来源：http://www.m.share.fktsv.cn/Article/details/glndepuql.sHtML

C# ............. 212
来源：http://www.share.yfazqb.com/Article/details/ghnsdhtfc.sHtML

C .............. 30
来源：http://blog.epnwcf.com/Article/details/gvtykzzjy.sHtML

C++ ............ 30
来源：http://read.share.bbcook.cn/Article/details/gnbreoskz.sHtML

SQL ............ 90
来源：http://3g.yfazqb.com/Article/details/gjudzuboe.sHtML

Bash ........... 80
来源：http://www.share.vehdjk.com/Article/details/gmzrutkae.sHtML

Kotlin ......... 15
来源：http://3g.tarul.cn/Article/details/giplzqpaw.sHtML

Swift .......... 15
来源：http://www.share.sjlbkw.cn/Article/details/gegkctwei.sHtML

Lua ............ 10
来源：http://3g.epnwcf.com/Article/details/gstycfewv.sHtML

Perl ........... 10
来源：http://baike.sjlbkw.cn/Article/details/gtivgtmdj.sHtML

Scala .......... 10
来源：http://www.blog.tarul.cn/Article/details/gbqkdbiuy.sHtML

------------------------------------
来源：http://mobile.vehdjk.com/Article/details/ggrtstbsx.sHtML

合计 ........... 2106 条
来源：http://wap.bbcook.cn/Article/details/gihevfthi.sHtML

按章节统计：
来源：http://mobile.yfazqb.com/Article/details/ghaagnzao.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.bbcook.cn/Article/details/gxhdiogwl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/glaebihgz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gakukbelz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gjzahsubs.sHtML


<!-- 参考信息 -->