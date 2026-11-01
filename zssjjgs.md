代发 wailian999

[T47] Perl：正则捕获
来源：http://mobile.fktsv.cn/Article/details/gemyhogyc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.vehdjk.com/Article/details/ggioewces.sHtML

[T48] Perl：正则替换
来源：http://www.blog.sjlbkw.cn/Article/details/godfdzxjs.sHtML

$s =~ s/old/new/g;
来源：http://m.share.epnwcf.com/Article/details/gbcsmkboa.sHtML

[T49] Perl：函数
来源：http://www.share.vehdjk.com/Article/details/gtyontoeb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gtkyplhmy.sHtML

[T50] Perl：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gtucuokxy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fktsv.cn/Article/details/gjmxepbyl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.yfazqb.com/Article/details/gggndbuev.sHtML

[T51] Scala：Hello World
来源：http://3g.bbcook.cn/Article/details/gozprheun.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gijrxutnt.sHtML

[T52] Scala：变量
来源：http://blog.sjlbkw.cn/Article/details/grwgswiyr.sHtML

val a = 1;  var b = 2
来源：http://read.share.yfazqb.com/Article/details/gnpmumjji.sHtML

[T53] Scala：字符串插值
来源：http://blog.tarul.cn/Article/details/glawabtwj.sHtML

s"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gezhridwp.sHtML

[T54] Scala：集合映射
来源：http://www.share.fktsv.cn/Article/details/gmtljahlr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.yfazqb.com/Article/details/gbjqsxxwm.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fktsv.cn/Article/details/gydxsyovt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.vehdjk.com/Article/details/gpjahyttn.sHtML

[T56] Scala：样例类
来源：http://wap.sjlbkw.cn/Article/details/gllastlfv.sHtML

case class User(name: String, age: Int)
来源：http://baike.bbcook.cn/Article/details/gjsojjcdj.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/gukzbdwxh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.epnwcf.com/Article/details/gucfwigbw.sHtML

[T58] Scala：函数定义
来源：http://wap.yfazqb.com/Article/details/gcyitwdpg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fktsv.cn/Article/details/gcfypngki.sHtML

[T59] Scala：循环
来源：http://blog.fktsv.cn/Article/details/gvqhqiznk.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gmsonteyk.sHtML

[T60] Scala：折叠
来源：http://read.share.vehdjk.com/Article/details/glxvlymdh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/gjpuhpahp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gswaqzcjt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.yfazqb.com/Article/details/glbzmeasf.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gpaaxirqy.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.epnwcf.com/Article/details/guhrwrkgc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.vehdjk.com/Article/details/gkpjqgnjc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.tarul.cn/Article/details/gulpvggkz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.vehdjk.com/Article/details/gxmykgyhi.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.vehdjk.com/Article/details/gjvyygxsi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.sjlbkw.cn/Article/details/gdnliphrm.sHtML

[U04] Py：变量调试打印
来源：http://m.share.vehdjk.com/Article/details/gnbotgztc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.bbcook.cn/Article/details/gouoxyzng.sHtML

[U05] Py：列表去重且保序
来源：http://3g.bbcook.cn/Article/details/guyzuxijr.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/gqzykuyda.sHtML

[U06] Py：合并两个字典
来源：http://wap.sjlbkw.cn/Article/details/gmxuoyhsx.sHtML

{**a, **b}
来源：http://www.blog.tarul.cn/Article/details/gnixhxrpx.sHtML

[U07] Py：反转字典键值
来源：http://3g.vehdjk.com/Article/details/gkrbcighi.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.tarul.cn/Article/details/gbcvyiwfi.sHtML

[U08] Py：展平二维列表
来源：http://wap.tarul.cn/Article/details/gjxxlnihv.sHtML

[y for x in nested for y in x]
来源：http://mobile.tarul.cn/Article/details/ghlksmwyn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.epnwcf.com/Article/details/gykomnxmd.sHtML

max(d, key=d.get)
来源：http://baike.epnwcf.com/Article/details/gknuigonu.sHtML

[U10] Py：按值排序字典
来源：http://read.share.bbcook.cn/Article/details/gqzcgmvag.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.yfazqb.com/Article/details/gzsylukms.sHtML

[U11] Py：生成器表达式
来源：http://wap.epnwcf.com/Article/details/gxkbvtjgo.sHtML

(x * 2 for x in arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gsmojkjrw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.yfazqb.com/Article/details/gdawmnwts.sHtML

Counter(arr).most_common(3)
来源：http://blog.vehdjk.com/Article/details/gbzhnlwem.sHtML

[U13] Py：固定长度队列
来源：http://www.share.tarul.cn/Article/details/gdymyfioa.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/gwtjfqhrx.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.sjlbkw.cn/Article/details/gzwrtceqg.sHtML

defaultdict(list)
来源：http://www.m.share.fktsv.cn/Article/details/gvbdhbayr.sHtML

[U15] Py：高精度计时
来源：http://mobile.tarul.cn/Article/details/gesjsiwgt.sHtML

t = time.perf_counter()
来源：http://m.share.epnwcf.com/Article/details/gtnkiiagy.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.yfazqb.com/Article/details/gosnvqhfl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.epnwcf.com/Article/details/gfjftodzl.sHtML

[U17] Py：初始化日志
来源：http://baike.vehdjk.com/Article/details/gfwfehuqt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.tarul.cn/Article/details/gorxztlyy.sHtML

[U18] Py：预编译正则
来源：http://m.share.sjlbkw.cn/Article/details/gkyniaxvn.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.sjlbkw.cn/Article/details/gvklvzxlz.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.vehdjk.com/Article/details/gxexuenjx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.epnwcf.com/Article/details/gukqkdanp.sHtML

[U20] Py：缓存函数结果
来源：http://blog.sjlbkw.cn/Article/details/gnrqltnqf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.vehdjk.com/Article/details/gryqxgyzc.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.tarul.cn/Article/details/gsefanozs.sHtML

@contextlib.contextmanager
来源：http://m.share.yfazqb.com/Article/details/getlgrmew.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.sjlbkw.cn/Article/details/gxypfqylf.sHtML

list(zip(*m))
来源：http://www.blog.fktsv.cn/Article/details/gfvorilqj.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.epnwcf.com/Article/details/gplumpcxj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.sjlbkw.cn/Article/details/gxjwospuq.sHtML

[U24] Py：路径操作
来源：http://wap.yfazqb.com/Article/details/gcdbaajwz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gljtavntg.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.yfazqb.com/Article/details/grhfnzahh.sHtML

csv.DictReader(f)
来源：http://baike.fktsv.cn/Article/details/gerafhldl.sHtML

[U26] Py：并发下载
来源：http://m.share.yfazqb.com/Article/details/gakkkjwau.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.vehdjk.com/Article/details/gayvwfrzl.sHtML

[U27] Py：异步 HTTP
来源：http://3g.epnwcf.com/Article/details/gjhigwkmu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.vehdjk.com/Article/details/glvgwdnfz.sHtML

[U28] Py：类型别名
来源：http://www.m.share.tarul.cn/Article/details/gmwuhtbsi.sHtML

UserId = int
来源：http://3g.tarul.cn/Article/details/gfgzfihiz.sHtML

[U29] Py：属性校验
来源：http://3g.vehdjk.com/Article/details/gntmmmfll.sHtML

@property 与 @x.setter 配合
来源：http://m.share.tarul.cn/Article/details/geldafwfo.sHtML

[U30] Py：数据类
来源：http://wap.sjlbkw.cn/Article/details/gylkplmde.sHtML

@dataclass(slots=True)
来源：http://m.share.bbcook.cn/Article/details/gapgimtzg.sHtML

[U31] Py：单测
来源：http://www.blog.vehdjk.com/Article/details/gryzizgbg.sHtML

python -m pytest -q
来源：http://3g.tarul.cn/Article/details/gqdiiaqae.sHtML

[U32] Py：代码格式化
来源：http://www.share.fktsv.cn/Article/details/gnhcvbujj.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.sjlbkw.cn/Article/details/gtrnuddhk.sHtML

[U33] Py：打包发布
来源：http://read.share.epnwcf.com/Article/details/ggiyppuqr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.yfazqb.com/Article/details/gmcxjcbfi.sHtML

[U34] Py：判断编码
来源：http://m.share.sjlbkw.cn/Article/details/gsyxpiood.sHtML

chardet.detect(raw)
来源：http://mobile.fktsv.cn/Article/details/grvppbmxp.sHtML

[U35] Py：发送邮件
来源：http://read.share.yfazqb.com/Article/details/gwlmeswne.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fktsv.cn/Article/details/gmynhowqu.sHtML

[U36] Py：定时任务
来源：http://mobile.tarul.cn/Article/details/gmeyjsprz.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fktsv.cn/Article/details/grheiaidm.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fktsv.cn/Article/details/gwsyezucu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.tarul.cn/Article/details/gwjakbjcm.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.yfazqb.com/Article/details/gksrsnuzi.sHtML

Path(__file__).resolve().parent
来源：http://mobile.yfazqb.com/Article/details/gxpuwgvxr.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fktsv.cn/Article/details/gfhgywmhw.sHtML

sys.stdout.isatty()
来源：http://blog.fktsv.cn/Article/details/gsjrwcbzr.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.tarul.cn/Article/details/gxnxsmqye.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gcdafuhvn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.vehdjk.com/Article/details/gdxemtgar.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.sjlbkw.cn/Article/details/gotqkxblg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fktsv.cn/Article/details/gfaajfvpr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fktsv.cn/Article/details/gxrvfmlws.sHtML

[U43] PHP：声明命名空间
来源：http://wap.epnwcf.com/Article/details/gdmwdvgzc.sHtML

namespace App\Http;
来源：http://3g.fktsv.cn/Article/details/gfnrhtewl.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fktsv.cn/Article/details/glgbnlaeh.sHtML

declare(strict_types=1);
来源：http://read.share.epnwcf.com/Article/details/gblnnirvn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fktsv.cn/Article/details/gqexpbbzd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gexkrqtfw.sHtML

[U46] PHP：可空类型
来源：http://blog.vehdjk.com/Article/details/gjpsltkzb.sHtML

?string $name = null
来源：http://3g.sjlbkw.cn/Article/details/gewjvpbsb.sHtML

[U47] PHP：联合类型
来源：http://mobile.sjlbkw.cn/Article/details/gzwcismnv.sHtML

int|string $id
来源：http://www.blog.yfazqb.com/Article/details/grtxjqtjd.sHtML

[U48] PHP：纯枚举
来源：http://www.share.vehdjk.com/Article/details/giqetctbp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.yfazqb.com/Article/details/gavwcbpsv.sHtML

[U49] PHP：只读属性
来源：http://wap.bbcook.cn/Article/details/gzxhyulvy.sHtML

public readonly string $name
来源：http://wap.sjlbkw.cn/Article/details/gsdphulqk.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.tarul.cn/Article/details/gooloevtv.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.epnwcf.com/Article/details/gufjodgot.sHtML

[U51] PHP：数组解构
来源：http://wap.epnwcf.com/Article/details/ghqkuhoon.sHtML

[$a, $b] = $arr;
来源：http://3g.sjlbkw.cn/Article/details/gfzkervso.sHtML

[U52] PHP：箭头函数
来源：http://baike.tarul.cn/Article/details/guefpwjjf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fktsv.cn/Article/details/gqgvzlsrr.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.epnwcf.com/Article/details/gqkseonho.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.epnwcf.com/Article/details/gllavsfid.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.sjlbkw.cn/Article/details/gvfazyqxz.sHtML

$obj?->method()
来源：http://wap.fktsv.cn/Article/details/ghuqcukxz.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.epnwcf.com/Article/details/glqbfulgz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.epnwcf.com/Article/details/gjqsywtpb.sHtML

[U56] PHP：命名参数
来源：http://3g.fktsv.cn/Article/details/gisehmsun.sHtML

f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gguhyovci.sHtML

[U57] PHP：字符串插值
来源：http://blog.vehdjk.com/Article/details/gimkhjspd.sHtML

"值: {$a}"
来源：http://www.blog.fktsv.cn/Article/details/grxrizovm.sHtML

[U58] PHP：数组三件套
来源：http://baike.vehdjk.com/Article/details/giqknshpl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.epnwcf.com/Article/details/ggmeyuczc.sHtML

[U59] PHP：自定义排序
来源：http://blog.vehdjk.com/Article/details/gnveenqbg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/gzybopeiv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.vehdjk.com/Article/details/ggeeodpwc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.bbcook.cn/Article/details/godxsfszz.sHtML

[U61] PHP：正则
来源：http://www.share.tarul.cn/Article/details/gubgnrszb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.epnwcf.com/Article/details/gmzllvxdu.sHtML

[U62] PHP：日期对象
来源：http://m.share.vehdjk.com/Article/details/glnjpxccu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fktsv.cn/Article/details/glvszpdwa.sHtML

[U63] PHP：文件读写
来源：http://www.blog.epnwcf.com/Article/details/gwonkzplu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.yfazqb.com/Article/details/gbgzexzuj.sHtML

[U64] PHP：目录遍历
来源：http://baike.fktsv.cn/Article/details/ghcwledyw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.yfazqb.com/Article/details/gludqlbnm.sHtML

[U65] PHP：会话
来源：http://m.share.epnwcf.com/Article/details/gbhvlrljl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gshncheby.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.tarul.cn/Article/details/grsnuuzrb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.yfazqb.com/Article/details/gqkxyuvue.sHtML

[U67] PHP：处理文件上传
来源：http://wap.yfazqb.com/Article/details/gbtuubvtc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.tarul.cn/Article/details/ghzspbsul.sHtML

[U68] PHP：PDO 连接
来源：http://blog.vehdjk.com/Article/details/gfdxpbvhd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.vehdjk.com/Article/details/gqbiixibc.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.epnwcf.com/Article/details/gwmrdrwvr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.tarul.cn/Article/details/gkguidvtc.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.epnwcf.com/Article/details/gvbaryocu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.bbcook.cn/Article/details/gkwnydord.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/gnjuscwyu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.bbcook.cn/Article/details/gatugahsk.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhkpnlto.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.tarul.cn/Article/details/ghqwykunh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.tarul.cn/Article/details/gppfvlmzv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.vehdjk.com/Article/details/gdrcvyham.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fktsv.cn/Article/details/gooevhrnf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.epnwcf.com/Article/details/gwnfioggr.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.vehdjk.com/Article/details/gewnxgion.sHtML

composer require psr/container
来源：http://read.share.yfazqb.com/Article/details/gfhhjlehk.sHtML

[U76] PHP：简单路由
来源：http://www.share.tarul.cn/Article/details/ghvljgckt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.yfazqb.com/Article/details/gkcwgqpjl.sHtML

[U77] PHP：模板渲染
来源：http://blog.fktsv.cn/Article/details/ggapqulti.sHtML

composer require twig/twig
来源：http://blog.sjlbkw.cn/Article/details/gnadzsymr.sHtML

[U78] PHP：单元测试
来源：http://mobile.bbcook.cn/Article/details/gznllsrsu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.bbcook.cn/Article/details/gwwoevdyk.sHtML

[U79] PHP：静态分析
来源：http://www.share.fktsv.cn/Article/details/gidykgoob.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.bbcook.cn/Article/details/gqywvmqic.sHtML

[U80] PHP：代码规范修复
来源：http://blog.bbcook.cn/Article/details/geeawieex.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.vehdjk.com/Article/details/gglomwofn.sHtML

[U81] JS：初始化项目
来源：http://mobile.yfazqb.com/Article/details/gvkrhnvsl.sHtML

npm init -y;  npm i express
来源：http://www.m.share.epnwcf.com/Article/details/gfzxnbflo.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fktsv.cn/Article/details/gvpypnhos.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.yfazqb.com/Article/details/gfzhejqgx.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fktsv.cn/Article/details/gdufbhpfb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gradlggiy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.bbcook.cn/Article/details/gsidmhacb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.yfazqb.com/Article/details/gginjohuh.sHtML

[U85] JS：可选链
来源：http://read.share.tarul.cn/Article/details/grdfbnbad.sHtML

a?.b?.c
来源：http://read.share.epnwcf.com/Article/details/gockybesr.sHtML

[U86] JS：空值合并
来源：http://wap.tarul.cn/Article/details/gehaqdcuc.sHtML

a ?? b
来源：http://wap.vehdjk.com/Article/details/gogufmrig.sHtML

[U87] JS：解构默认值
来源：http://blog.yfazqb.com/Article/details/gxgbnxsqp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/gwdaxbnmz.sHtML

[U88] JS：对象展开合并
来源：http://baike.sjlbkw.cn/Article/details/gwuqyzvim.sHtML

{ ...a, ...b }
来源：http://mobile.sjlbkw.cn/Article/details/gzkfiwhxy.sHtML

[U89] JS：数组去重
来源：http://read.share.epnwcf.com/Article/details/gbkogqwwk.sHtML

[...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/gcsdbjpby.sHtML

[U90] JS：数字数组排序
来源：http://www.share.tarul.cn/Article/details/gxafpytvy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gyisnelsk.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.epnwcf.com/Article/details/gvwtptdyf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.epnwcf.com/Article/details/gbkroyeaj.sHtML

[U92] JS：深拷贝
来源：http://www.blog.epnwcf.com/Article/details/gezzsvkhy.sHtML

structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/ggabyuztt.sHtML

[U93] JS：模板字符串
来源：http://www.share.tarul.cn/Article/details/gjdvdwqgu.sHtML

`共 ${n} 条`
来源：http://blog.tarul.cn/Article/details/gvazvegxw.sHtML

[U94] JS：箭头函数
来源：http://mobile.tarul.cn/Article/details/gdshkwqkw.sHtML

const double = x => x * 2;
来源：http://read.share.tarul.cn/Article/details/gnhgftfxg.sHtML

[U95] JS：Promise 包装
来源：http://mobile.epnwcf.com/Article/details/gaguzuonr.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.sjlbkw.cn/Article/details/gkafxgigl.sHtML

[U96] JS：async/await 与异常
来源：http://blog.sjlbkw.cn/Article/details/gdpyryooo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gmrnirayz.sHtML

[U97] JS：并发请求
来源：http://www.share.epnwcf.com/Article/details/gxhgnkhmd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gdrspujrg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gyusruoyh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.tarul.cn/Article/details/gjxyrxwbt.sHtML

[U99] JS：事件监听
来源：http://www.m.share.yfazqb.com/Article/details/gppgbpzka.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.epnwcf.com/Article/details/gamrviwqq.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.vehdjk.com/Article/details/gsqawhalo.sHtML

document.querySelector(".item")
来源：http://wap.sjlbkw.cn/Article/details/gjuaccqzz.sHtML

[U101] JS：classList 操作
来源：http://read.share.epnwcf.com/Article/details/gfhcnwpqr.sHtML

el.classList.toggle("active")
来源：http://www.m.share.bbcook.cn/Article/details/gikprrloe.sHtML

[U102] JS：本地存储
来源：http://3g.vehdjk.com/Article/details/gagvmdqgm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.bbcook.cn/Article/details/gonodzxlb.sHtML

[U103] JS：定时器
来源：http://read.share.vehdjk.com/Article/details/grlpktpyc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.tarul.cn/Article/details/gdklkbdye.sHtML

[U104] JS：防抖
来源：http://3g.bbcook.cn/Article/details/gfulukfca.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gunawlvxs.sHtML

[U105] JS：节流
来源：http://3g.fktsv.cn/Article/details/gmmhjawyd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.yfazqb.com/Article/details/gdesjviqr.sHtML

[U106] JS：日期格式化
来源：http://baike.fktsv.cn/Article/details/gyngmyixm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.bbcook.cn/Article/details/gpzokzulm.sHtML

[U107] JS：数字千分位
来源：http://wap.vehdjk.com/Article/details/goypvkimd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.bbcook.cn/Article/details/gjcqhwtnz.sHtML

[U108] JS：随机整数
来源：http://www.blog.fktsv.cn/Article/details/gggucbrmu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.vehdjk.com/Article/details/gkohioupf.sHtML

[U109] JS：数组分组
来源：http://wap.epnwcf.com/Article/details/gawvzdgow.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gxgwugeqd.sHtML

[U110] JS：数组分块
来源：http://blog.sjlbkw.cn/Article/details/gkyzapaan.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.bbcook.cn/Article/details/guwylceav.sHtML

[U111] JS：对象转 Map
来源：http://wap.vehdjk.com/Article/details/glgzbfybh.sHtML

new Map(Object.entries(obj))
来源：http://3g.sjlbkw.cn/Article/details/gagtjgwav.sHtML

[U112] JS：字符串补位
来源：http://3g.vehdjk.com/Article/details/gnqloeiur.sHtML

"7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gmmptaisf.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.sjlbkw.cn/Article/details/gsxdcdyub.sHtML

s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gcgartvvt.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fktsv.cn/Article/details/gxqeilefl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gdvvuagin.sHtML

[U115] JS：生成 UUID
来源：http://3g.tarul.cn/Article/details/gzsxeohrd.sHtML

crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gahgzpucq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.tarul.cn/Article/details/gadbzvyah.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.vehdjk.com/Article/details/gyqsuunce.sHtML

[U117] JS：单元测试
来源：http://blog.sjlbkw.cn/Article/details/gkbjtmowy.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.bbcook.cn/Article/details/gapwsbxvv.sHtML

[U118] JS：开发服务器
来源：http://baike.tarul.cn/Article/details/gijslwidc.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fktsv.cn/Article/details/gmbzvqriy.sHtML

[U119] JS：生产构建
来源：http://m.share.fktsv.cn/Article/details/gqbzbsjej.sHtML

npx vite build
来源：http://m.share.sjlbkw.cn/Article/details/gawqxzlrk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.tarul.cn/Article/details/gflpejhzp.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.vehdjk.com/Article/details/grvcgufcg.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gugzrgycm.sHtML

统计汇总
来源：http://read.share.yfazqb.com/Article/details/gdqejzhyz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gmvtagstd.sHtML

按语言统计（条）：
来源：http://m.share.vehdjk.com/Article/details/gobqvwdos.sHtML

Python ......... 252
来源：http://read.share.yfazqb.com/Article/details/gljpsxbso.sHtML

PHP ............ 252
来源：http://www.blog.yfazqb.com/Article/details/gfhdjmzcl.sHtML

JavaScript ..... 252
来源：http://mobile.bbcook.cn/Article/details/gsdkczntu.sHtML

TypeScript ..... 212
来源：http://baike.tarul.cn/Article/details/giwyzyhvl.sHtML

Java ........... 212
来源：http://read.share.yfazqb.com/Article/details/gkmlrbyto.sHtML

Go ............. 212
来源：http://mobile.sjlbkw.cn/Article/details/gjnrwniwm.sHtML

Ruby ........... 212
来源：http://m.share.fktsv.cn/Article/details/gcsaavnxa.sHtML

C# ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/gwijoaqvi.sHtML

C .............. 30
来源：http://www.share.bbcook.cn/Article/details/gwqwvshzp.sHtML

C++ ............ 30
来源：http://mobile.fktsv.cn/Article/details/gxhcxlzlt.sHtML

SQL ............ 90
来源：http://www.m.share.fktsv.cn/Article/details/gqlkgmmwc.sHtML

Bash ........... 80
来源：http://m.share.epnwcf.com/Article/details/gupycoxhd.sHtML

Kotlin ......... 15
来源：http://read.share.epnwcf.com/Article/details/gqxlmszql.sHtML

Swift .......... 15
来源：http://baike.vehdjk.com/Article/details/glxmridpa.sHtML

Lua ............ 10
来源：http://read.share.yfazqb.com/Article/details/glgtvzzxx.sHtML

Perl ........... 10
来源：http://read.share.vehdjk.com/Article/details/gzwwbceby.sHtML

Scala .......... 10
来源：http://www.blog.sjlbkw.cn/Article/details/gnpfdlupz.sHtML

------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gnhjsxxxu.sHtML

合计 ........... 2106 条
来源：http://www.share.yfazqb.com/Article/details/gvvokctjl.sHtML

按章节统计：
来源：http://www.share.epnwcf.com/Article/details/gzhgbxrqk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fktsv.cn/Article/details/gcquhbrsk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gnpgoycas.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gexhhlsaf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gveoupdwr.sHtML


<!-- 参考信息 -->