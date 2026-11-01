代发 wailian999

[T47] Perl：正则捕获
来源：http://blog.sjlbkw.cn/Article/details/ghhtoovos.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.yfazqb.com/Article/details/ghnxximmu.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gwooutnfi.sHtML

$s =~ s/old/new/g;
来源：http://read.share.yfazqb.com/Article/details/gbbzmzajg.sHtML

[T49] Perl：函数
来源：http://3g.tarul.cn/Article/details/gdxggggyb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/guguyxgqe.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/ghseulroi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.tarul.cn/Article/details/gyymupige.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fktsv.cn/Article/details/grsmkqlmo.sHtML

[T51] Scala：Hello World
来源：http://www.share.vehdjk.com/Article/details/gyemiwsqr.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gixinzzhp.sHtML

[T52] Scala：变量
来源：http://read.share.fktsv.cn/Article/details/gdgbzxbpu.sHtML

val a = 1;  var b = 2
来源：http://mobile.epnwcf.com/Article/details/ggfypghga.sHtML

[T53] Scala：字符串插值
来源：http://wap.tarul.cn/Article/details/gfujednle.sHtML

s"值: $b"
来源：http://read.share.vehdjk.com/Article/details/grzvjqvgl.sHtML

[T54] Scala：集合映射
来源：http://wap.tarul.cn/Article/details/gzymixasn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.epnwcf.com/Article/details/gagqylexx.sHtML

[T55] Scala：集合过滤
来源：http://www.share.tarul.cn/Article/details/ggvaxcngv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.bbcook.cn/Article/details/gcfksaenh.sHtML

[T56] Scala：样例类
来源：http://www.share.vehdjk.com/Article/details/giftrnsis.sHtML

case class User(name: String, age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/ghwpvzlph.sHtML

[T57] Scala：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gbkwyiffs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.vehdjk.com/Article/details/gdgfnhflf.sHtML

[T58] Scala：函数定义
来源：http://baike.tarul.cn/Article/details/glxxwpcpg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fktsv.cn/Article/details/gluxhjccm.sHtML

[T59] Scala：循环
来源：http://m.share.bbcook.cn/Article/details/gzngpboxw.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fktsv.cn/Article/details/gsjbhgnuk.sHtML

[T60] Scala：折叠
来源：http://baike.yfazqb.com/Article/details/gsoziduzk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.tarul.cn/Article/details/ggtdiqfza.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gnxpdfhlh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/gjydxqusm.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gedtotcxs.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fktsv.cn/Article/details/glvpoynzs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.vehdjk.com/Article/details/gplpzlgkg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fktsv.cn/Article/details/gakfukpjs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.vehdjk.com/Article/details/gxlleqkqd.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.sjlbkw.cn/Article/details/gjjfzvzwl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.epnwcf.com/Article/details/gcrixbuns.sHtML

[U04] Py：变量调试打印
来源：http://www.share.bbcook.cn/Article/details/ghggsqtsk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.sjlbkw.cn/Article/details/gfraexbqy.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/gmtsuqqni.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gqpsyxisn.sHtML

[U06] Py：合并两个字典
来源：http://www.share.epnwcf.com/Article/details/ghvyrbbjn.sHtML

{**a, **b}
来源：http://read.share.yfazqb.com/Article/details/glysybxxr.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fktsv.cn/Article/details/gfcllzofe.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.yfazqb.com/Article/details/gspagazyd.sHtML

[U08] Py：展平二维列表
来源：http://baike.epnwcf.com/Article/details/gtvcadxbv.sHtML

[y for x in nested for y in x]
来源：http://www.share.bbcook.cn/Article/details/giuyhxydt.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.yfazqb.com/Article/details/giqfxnqqt.sHtML

max(d, key=d.get)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyqzhyns.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.epnwcf.com/Article/details/gyklipxnk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.vehdjk.com/Article/details/gcsmmhdns.sHtML

[U11] Py：生成器表达式
来源：http://m.share.tarul.cn/Article/details/gjcrfbipo.sHtML

(x * 2 for x in arr)
来源：http://3g.sjlbkw.cn/Article/details/ghbdmzijp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.tarul.cn/Article/details/gseehtnfb.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.bbcook.cn/Article/details/gmrzpbkvj.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.vehdjk.com/Article/details/grcormtzh.sHtML

deque(maxlen=10)
来源：http://wap.sjlbkw.cn/Article/details/gyhmilybz.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fktsv.cn/Article/details/gqhoplias.sHtML

defaultdict(list)
来源：http://3g.fktsv.cn/Article/details/ggmkqznhz.sHtML

[U15] Py：高精度计时
来源：http://www.blog.epnwcf.com/Article/details/gxldkgkmf.sHtML

t = time.perf_counter()
来源：http://www.blog.fktsv.cn/Article/details/ggqgcwppv.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.yfazqb.com/Article/details/gvlqkdnju.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.sjlbkw.cn/Article/details/guissazxv.sHtML

[U17] Py：初始化日志
来源：http://blog.sjlbkw.cn/Article/details/gcqfmsacg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.tarul.cn/Article/details/gjcmgtnjt.sHtML

[U18] Py：预编译正则
来源：http://www.share.epnwcf.com/Article/details/gjqdtxdnc.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/gwdtqomwh.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.epnwcf.com/Article/details/grlixzqtk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fktsv.cn/Article/details/gtzmfllsw.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.epnwcf.com/Article/details/gzihvaklt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.yfazqb.com/Article/details/gmhafaqzd.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.epnwcf.com/Article/details/geqyrlqlz.sHtML

@contextlib.contextmanager
来源：http://3g.fktsv.cn/Article/details/gcuxyxbfa.sHtML

[U22] Py：矩阵转置
来源：http://wap.epnwcf.com/Article/details/gnzuvsnnu.sHtML

list(zip(*m))
来源：http://read.share.epnwcf.com/Article/details/gizddthye.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.yfazqb.com/Article/details/gjwovwlki.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.epnwcf.com/Article/details/gbdgmkgyt.sHtML

[U24] Py：路径操作
来源：http://read.share.fktsv.cn/Article/details/gkvxjxomu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gohsqlxcn.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.sjlbkw.cn/Article/details/gjnwhcmtv.sHtML

csv.DictReader(f)
来源：http://3g.bbcook.cn/Article/details/gnjgyyeit.sHtML

[U26] Py：并发下载
来源：http://www.share.yfazqb.com/Article/details/gcetohqud.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.tarul.cn/Article/details/gnmdrrahl.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.epnwcf.com/Article/details/gippfzhna.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.sjlbkw.cn/Article/details/gfdjqwvyp.sHtML

[U28] Py：类型别名
来源：http://mobile.fktsv.cn/Article/details/gibgfoceg.sHtML

UserId = int
来源：http://m.share.epnwcf.com/Article/details/gjliufixr.sHtML

[U29] Py：属性校验
来源：http://3g.yfazqb.com/Article/details/gqjnvkhog.sHtML

@property 与 @x.setter 配合
来源：http://m.share.tarul.cn/Article/details/gzxdszgkn.sHtML

[U30] Py：数据类
来源：http://baike.sjlbkw.cn/Article/details/gqcddhdat.sHtML

@dataclass(slots=True)
来源：http://m.share.epnwcf.com/Article/details/gxysjuglo.sHtML

[U31] Py：单测
来源：http://m.share.sjlbkw.cn/Article/details/gfbviizcy.sHtML

python -m pytest -q
来源：http://blog.tarul.cn/Article/details/gydrrquzt.sHtML

[U32] Py：代码格式化
来源：http://m.share.epnwcf.com/Article/details/goxyjnhkt.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.bbcook.cn/Article/details/gtikjdxka.sHtML

[U33] Py：打包发布
来源：http://blog.tarul.cn/Article/details/gfwwtyhif.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.bbcook.cn/Article/details/gaccsprou.sHtML

[U34] Py：判断编码
来源：http://mobile.vehdjk.com/Article/details/gehqlsebh.sHtML

chardet.detect(raw)
来源：http://read.share.bbcook.cn/Article/details/gfogdfece.sHtML

[U35] Py：发送邮件
来源：http://mobile.yfazqb.com/Article/details/gsigpzkpk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fktsv.cn/Article/details/gxevlvvpj.sHtML

[U36] Py：定时任务
来源：http://read.share.yfazqb.com/Article/details/gcfqxorza.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.vehdjk.com/Article/details/gsgxmsdsn.sHtML

[U37] Py：读写 Excel
来源：http://read.share.sjlbkw.cn/Article/details/ghcoscrmw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.sjlbkw.cn/Article/details/gbftbloxv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.yfazqb.com/Article/details/gsqtrwigy.sHtML

Path(__file__).resolve().parent
来源：http://m.share.sjlbkw.cn/Article/details/gelyxqqcp.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.epnwcf.com/Article/details/gofdzqljv.sHtML

sys.stdout.isatty()
来源：http://www.blog.vehdjk.com/Article/details/gppgfjhzp.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fktsv.cn/Article/details/gzvweydhy.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/gsoawhhbf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.yfazqb.com/Article/details/gwoaqeorn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.bbcook.cn/Article/details/gjnqulzcm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.bbcook.cn/Article/details/gpotglqei.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.tarul.cn/Article/details/ghuucfvmn.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.yfazqb.com/Article/details/gdpzewgnp.sHtML

namespace App\Http;
来源：http://baike.epnwcf.com/Article/details/gguckupey.sHtML

[U44] PHP：开启严格类型
来源：http://3g.tarul.cn/Article/details/gjfdynelt.sHtML

declare(strict_types=1);
来源：http://www.blog.yfazqb.com/Article/details/gqybxwdkp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.sjlbkw.cn/Article/details/gzonlkfwk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gbuzdgiot.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fktsv.cn/Article/details/galcflacm.sHtML

?string $name = null
来源：http://www.m.share.epnwcf.com/Article/details/gtlpgmcqc.sHtML

[U47] PHP：联合类型
来源：http://3g.bbcook.cn/Article/details/gjvwlpdia.sHtML

int|string $id
来源：http://m.share.bbcook.cn/Article/details/gvnvgzwke.sHtML

[U48] PHP：纯枚举
来源：http://m.share.sjlbkw.cn/Article/details/gdsownngz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.bbcook.cn/Article/details/gilprukcx.sHtML

[U49] PHP：只读属性
来源：http://blog.sjlbkw.cn/Article/details/goypumuev.sHtML

public readonly string $name
来源：http://wap.epnwcf.com/Article/details/ghnufwlnc.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.yfazqb.com/Article/details/gmfadztzz.sHtML

public function __construct(private int $id) {}
来源：http://read.share.epnwcf.com/Article/details/gehiidona.sHtML

[U51] PHP：数组解构
来源：http://www.share.yfazqb.com/Article/details/gvjlsxqaz.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/geaewxhwj.sHtML

[U52] PHP：箭头函数
来源：http://m.share.yfazqb.com/Article/details/gdgqtxkkq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.sjlbkw.cn/Article/details/geqrilbcm.sHtML

[U53] PHP：空合并运算符
来源：http://3g.yfazqb.com/Article/details/gjguelmzd.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.epnwcf.com/Article/details/gnznvewzp.sHtML

[U54] PHP：空安全调用
来源：http://read.share.vehdjk.com/Article/details/gtvvqlgje.sHtML

$obj?->method()
来源：http://blog.bbcook.cn/Article/details/giaeetgum.sHtML

[U55] PHP：match 表达式
来源：http://www.share.yfazqb.com/Article/details/gijgslssp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fktsv.cn/Article/details/gbbfnlgrv.sHtML

[U56] PHP：命名参数
来源：http://www.blog.tarul.cn/Article/details/gugxrjajq.sHtML

f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gtnqgyhkd.sHtML

[U57] PHP：字符串插值
来源：http://www.share.tarul.cn/Article/details/gdjlyjuxl.sHtML

"值: {$a}"
来源：http://baike.bbcook.cn/Article/details/guxovjtkq.sHtML

[U58] PHP：数组三件套
来源：http://3g.epnwcf.com/Article/details/gvgnriepo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gfiusoetu.sHtML

[U59] PHP：自定义排序
来源：http://www.share.yfazqb.com/Article/details/gzvswthzq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fktsv.cn/Article/details/gsqlvlgpr.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fktsv.cn/Article/details/gmpddbzyp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.epnwcf.com/Article/details/gdtkqidop.sHtML

[U61] PHP：正则
来源：http://www.share.sjlbkw.cn/Article/details/gflcgxwka.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fktsv.cn/Article/details/gzivohvto.sHtML

[U62] PHP：日期对象
来源：http://blog.bbcook.cn/Article/details/gqcdolmrk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fktsv.cn/Article/details/gubwrhbqg.sHtML

[U63] PHP：文件读写
来源：http://blog.vehdjk.com/Article/details/gwnsvyzod.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fktsv.cn/Article/details/gtqiomdwi.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.tarul.cn/Article/details/gyqsbyiij.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fktsv.cn/Article/details/gpbrihaye.sHtML

[U65] PHP：会话
来源：http://www.blog.yfazqb.com/Article/details/gzcnwzvrk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.tarul.cn/Article/details/ghlzacemf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.vehdjk.com/Article/details/gpwjhyklz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.vehdjk.com/Article/details/garzwqjyj.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.epnwcf.com/Article/details/gmefpfrqh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.tarul.cn/Article/details/gzxjpmytb.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.vehdjk.com/Article/details/gyfydxujn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.sjlbkw.cn/Article/details/ghuvvpoat.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fktsv.cn/Article/details/gtwoptknv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.bbcook.cn/Article/details/gvwigcpts.sHtML

[U70] PHP：PDO 事务
来源：http://3g.epnwcf.com/Article/details/gnbxthumc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.yfazqb.com/Article/details/golxqrmta.sHtML

[U71] PHP：抛出异常
来源：http://wap.fktsv.cn/Article/details/glvlcjnhx.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.sjlbkw.cn/Article/details/gplqkocjr.sHtML

[U72] PHP：写错误日志
来源：http://www.share.bbcook.cn/Article/details/geashfaml.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.epnwcf.com/Article/details/gouchppzx.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fktsv.cn/Article/details/ggkmcsfub.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.bbcook.cn/Article/details/gtbeiclhw.sHtML

[U74] PHP：读取环境变量
来源：http://3g.tarul.cn/Article/details/gsealbzkp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.vehdjk.com/Article/details/gnqigfunu.sHtML

[U75] PHP：依赖注入
来源：http://wap.vehdjk.com/Article/details/gibihbsex.sHtML

composer require psr/container
来源：http://read.share.bbcook.cn/Article/details/ghledrykq.sHtML

[U76] PHP：简单路由
来源：http://blog.sjlbkw.cn/Article/details/ghslmclpy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.vehdjk.com/Article/details/gebddlpqk.sHtML

[U77] PHP：模板渲染
来源：http://blog.epnwcf.com/Article/details/ginalokbe.sHtML

composer require twig/twig
来源：http://m.share.fktsv.cn/Article/details/gqymrsjyp.sHtML

[U78] PHP：单元测试
来源：http://m.share.yfazqb.com/Article/details/gaugyozsx.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.epnwcf.com/Article/details/gllbwspja.sHtML

[U79] PHP：静态分析
来源：http://blog.epnwcf.com/Article/details/gftrnrsxt.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.vehdjk.com/Article/details/gxohzmtgw.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.bbcook.cn/Article/details/gusjjkctf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.bbcook.cn/Article/details/gfctlumgf.sHtML

[U81] JS：初始化项目
来源：http://m.share.bbcook.cn/Article/details/gjuruorcn.sHtML

npm init -y;  npm i express
来源：http://www.share.epnwcf.com/Article/details/ghrgpzjgr.sHtML

[U82] JS：package.json 脚本
来源：http://3g.tarul.cn/Article/details/gechbcidx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.vehdjk.com/Article/details/gdpxfblvv.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fktsv.cn/Article/details/gkjbgpfmx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/gnguwqclk.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.vehdjk.com/Article/details/gcevbxdyi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.bbcook.cn/Article/details/gehsnvgfi.sHtML

[U85] JS：可选链
来源：http://m.share.epnwcf.com/Article/details/gclkyxddk.sHtML

a?.b?.c
来源：http://blog.fktsv.cn/Article/details/ghbkaksxf.sHtML

[U86] JS：空值合并
来源：http://www.blog.tarul.cn/Article/details/gslqynmfh.sHtML

a ?? b
来源：http://baike.bbcook.cn/Article/details/gdsmqmlfs.sHtML

[U87] JS：解构默认值
来源：http://blog.yfazqb.com/Article/details/gczdojbrg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.bbcook.cn/Article/details/ggbyftllh.sHtML

[U88] JS：对象展开合并
来源：http://wap.epnwcf.com/Article/details/gsgsxwgyk.sHtML

{ ...a, ...b }
来源：http://m.share.vehdjk.com/Article/details/gqrmlswnj.sHtML

[U89] JS：数组去重
来源：http://baike.fktsv.cn/Article/details/gejrvwuko.sHtML

[...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gtmpgpvsh.sHtML

[U90] JS：数字数组排序
来源：http://wap.sjlbkw.cn/Article/details/gmjudkkga.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/grhnztbwq.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.vehdjk.com/Article/details/gdlccfurb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.sjlbkw.cn/Article/details/gfhoyvrai.sHtML

[U92] JS：深拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gstjpxocd.sHtML

structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/glylqbcus.sHtML

[U93] JS：模板字符串
来源：http://blog.sjlbkw.cn/Article/details/gchipfcwt.sHtML

`共 ${n} 条`
来源：http://wap.tarul.cn/Article/details/gagmvrcpt.sHtML

[U94] JS：箭头函数
来源：http://read.share.tarul.cn/Article/details/gtmfcgacd.sHtML

const double = x => x * 2;
来源：http://www.blog.epnwcf.com/Article/details/gpqyzzgka.sHtML

[U95] JS：Promise 包装
来源：http://mobile.epnwcf.com/Article/details/gvccotofr.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.yfazqb.com/Article/details/gmlkdxcwd.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.vehdjk.com/Article/details/giijlttyz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gayvdeitp.sHtML

[U97] JS：并发请求
来源：http://www.share.yfazqb.com/Article/details/gyvjpvadc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gdnrervyw.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.vehdjk.com/Article/details/gogczxzrg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.epnwcf.com/Article/details/gjdbfkcsb.sHtML

[U99] JS：事件监听
来源：http://www.m.share.tarul.cn/Article/details/gmmalljxr.sHtML

el.addEventListener("click", e => {})
来源：http://3g.vehdjk.com/Article/details/gykkqbwwt.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.bbcook.cn/Article/details/gecuzdrev.sHtML

document.querySelector(".item")
来源：http://m.share.epnwcf.com/Article/details/gbgcdujmw.sHtML

[U101] JS：classList 操作
来源：http://www.share.epnwcf.com/Article/details/gucergdqo.sHtML

el.classList.toggle("active")
来源：http://www.share.vehdjk.com/Article/details/gprrkqqgi.sHtML

[U102] JS：本地存储
来源：http://m.share.bbcook.cn/Article/details/gizywdmib.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.sjlbkw.cn/Article/details/gxyyzwbqx.sHtML

[U103] JS：定时器
来源：http://3g.tarul.cn/Article/details/gjibjgtix.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.yfazqb.com/Article/details/gpqqcqfst.sHtML

[U104] JS：防抖
来源：http://www.share.sjlbkw.cn/Article/details/gtlcgdqiq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/ghwrsfsqf.sHtML

[U105] JS：节流
来源：http://blog.tarul.cn/Article/details/gchbdoiqz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.bbcook.cn/Article/details/gxcdqjhmp.sHtML

[U106] JS：日期格式化
来源：http://blog.tarul.cn/Article/details/gokigtjpz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.sjlbkw.cn/Article/details/gjixbless.sHtML

[U107] JS：数字千分位
来源：http://m.share.yfazqb.com/Article/details/gpyrzbgwm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/goclfldqj.sHtML

[U108] JS：随机整数
来源：http://blog.fktsv.cn/Article/details/gtuhdvoxy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.sjlbkw.cn/Article/details/gnoiikeza.sHtML

[U109] JS：数组分组
来源：http://baike.fktsv.cn/Article/details/gzrdlskwp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/gpuasrtvj.sHtML

[U110] JS：数组分块
来源：http://www.blog.bbcook.cn/Article/details/gjqvydggg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fktsv.cn/Article/details/gkdtlzene.sHtML

[U111] JS：对象转 Map
来源：http://m.share.yfazqb.com/Article/details/guxswoorq.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.tarul.cn/Article/details/gdrmlmseq.sHtML

[U112] JS：字符串补位
来源：http://read.share.tarul.cn/Article/details/grvhgcadp.sHtML

"7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/genqjywzg.sHtML

[U113] JS：正则替换全部
来源：http://m.share.epnwcf.com/Article/details/gdnybakhf.sHtML

s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gjvzbayxg.sHtML

[U114] JS：JSON 深比较
来源：http://3g.sjlbkw.cn/Article/details/gwzxubtmg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.sjlbkw.cn/Article/details/gvoofedxf.sHtML

[U115] JS：生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/gpagucgeh.sHtML

crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/ggsytygex.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.sjlbkw.cn/Article/details/gzmqgwykk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.tarul.cn/Article/details/gwsfufeft.sHtML

[U117] JS：单元测试
来源：http://www.m.share.bbcook.cn/Article/details/gfzduwuoe.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.vehdjk.com/Article/details/grrvddtsl.sHtML

[U118] JS：开发服务器
来源：http://read.share.epnwcf.com/Article/details/gdrqzevew.sHtML

npm i -D vite;  npx vite
来源：http://wap.fktsv.cn/Article/details/gmvwiwfjj.sHtML

[U119] JS：生产构建
来源：http://baike.fktsv.cn/Article/details/gyechfjbl.sHtML

npx vite build
来源：http://3g.yfazqb.com/Article/details/gvbztflxl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.sjlbkw.cn/Article/details/gspxzuvsg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.epnwcf.com/Article/details/gwhtxjmvy.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ginrejcpz.sHtML

统计汇总
来源：http://www.share.vehdjk.com/Article/details/giyxtdqee.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/guvpajmdm.sHtML

按语言统计（条）：
来源：http://baike.yfazqb.com/Article/details/gitxcfjad.sHtML

Python ......... 252
来源：http://www.m.share.sjlbkw.cn/Article/details/guqofqkjc.sHtML

PHP ............ 252
来源：http://blog.bbcook.cn/Article/details/gmjtcumlh.sHtML

JavaScript ..... 252
来源：http://www.blog.tarul.cn/Article/details/gtdzuawuo.sHtML

TypeScript ..... 212
来源：http://www.m.share.tarul.cn/Article/details/gmzwlhlag.sHtML

Java ........... 212
来源：http://read.share.tarul.cn/Article/details/gfqaiiiuv.sHtML

Go ............. 212
来源：http://wap.vehdjk.com/Article/details/gguumoxds.sHtML

Ruby ........... 212
来源：http://3g.epnwcf.com/Article/details/gplgxmato.sHtML

C# ............. 212
来源：http://baike.bbcook.cn/Article/details/gugqpdmav.sHtML

C .............. 30
来源：http://3g.vehdjk.com/Article/details/gtkriswsu.sHtML

C++ ............ 30
来源：http://www.share.vehdjk.com/Article/details/gpsioyijv.sHtML

SQL ............ 90
来源：http://www.share.vehdjk.com/Article/details/gbrswlrfn.sHtML

Bash ........... 80
来源：http://3g.yfazqb.com/Article/details/ggqvsmjud.sHtML

Kotlin ......... 15
来源：http://mobile.fktsv.cn/Article/details/guvtcmlrg.sHtML

Swift .......... 15
来源：http://www.m.share.tarul.cn/Article/details/gmhwykais.sHtML

Lua ............ 10
来源：http://baike.vehdjk.com/Article/details/gqeejpqxw.sHtML

Perl ........... 10
来源：http://baike.tarul.cn/Article/details/gcndwlzpj.sHtML

Scala .......... 10
来源：http://www.blog.bbcook.cn/Article/details/grfqeqbnm.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gctzuupdp.sHtML

合计 ........... 2106 条
来源：http://blog.fktsv.cn/Article/details/gvtpazpyp.sHtML

按章节统计：
来源：http://www.share.fktsv.cn/Article/details/gkhkxizim.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.sjlbkw.cn/Article/details/gcvgwevgv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/glvshnvez.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gfdgxskbc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.bbcook.cn/Article/details/gfklzmmwv.sHtML


<!-- 参考信息 -->