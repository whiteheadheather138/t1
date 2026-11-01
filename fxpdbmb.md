代发 wailian999

[T49] Perl：函数
来源：http://m.share.tarul.cn/Article/details/gtiaadzsq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gljbxbczj.sHtML

[T50] Perl：逐行读文件
来源：http://3g.bbcook.cn/Article/details/glxjcuyom.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fktsv.cn/Article/details/gqsfdkkvi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.tarul.cn/Article/details/gtkxoxiyl.sHtML

[T51] Scala：Hello World
来源：http://read.share.fktsv.cn/Article/details/grpwbsewi.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gmezvqcjz.sHtML

[T52] Scala：变量
来源：http://baike.yfazqb.com/Article/details/ginftqusa.sHtML

val a = 1;  var b = 2
来源：http://m.share.vehdjk.com/Article/details/gzoemegvm.sHtML

[T53] Scala：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gteamxyvx.sHtML

s"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gcijdmixs.sHtML

[T54] Scala：集合映射
来源：http://read.share.vehdjk.com/Article/details/gbrsnxpjr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.vehdjk.com/Article/details/grwbfsifb.sHtML

[T55] Scala：集合过滤
来源：http://m.share.vehdjk.com/Article/details/ggqdwtgoa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fktsv.cn/Article/details/gkcbtdruo.sHtML

[T56] Scala：样例类
来源：http://wap.epnwcf.com/Article/details/guvkukjor.sHtML

case class User(name: String, age: Int)
来源：http://blog.epnwcf.com/Article/details/gmahtyiyf.sHtML

[T57] Scala：模式匹配
来源：http://3g.fktsv.cn/Article/details/gxzjqxorj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.yfazqb.com/Article/details/gkcjldjka.sHtML

[T58] Scala：函数定义
来源：http://wap.tarul.cn/Article/details/gfpopoewk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.tarul.cn/Article/details/gkisgbkaa.sHtML

[T59] Scala：循环
来源：http://3g.bbcook.cn/Article/details/grtzisuio.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.vehdjk.com/Article/details/glxlbcpdi.sHtML

[T60] Scala：折叠
来源：http://blog.vehdjk.com/Article/details/gfnkmbglz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.tarul.cn/Article/details/ggwifpper.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gounbnnik.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.epnwcf.com/Article/details/gvqaqwuvy.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gpgahreet.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.epnwcf.com/Article/details/gqffrtvut.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.yfazqb.com/Article/details/gebpbkkzh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.yfazqb.com/Article/details/guygvsxol.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.tarul.cn/Article/details/gnakoxmtn.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.tarul.cn/Article/details/gdstqdrhu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.yfazqb.com/Article/details/gufhoakav.sHtML

[U04] Py：变量调试打印
来源：http://m.share.epnwcf.com/Article/details/gtvcrbzvx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.vehdjk.com/Article/details/gavzwcxdl.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.bbcook.cn/Article/details/gqmaqblyj.sHtML

list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/gefukstey.sHtML

[U06] Py：合并两个字典
来源：http://baike.sjlbkw.cn/Article/details/gknqwclnl.sHtML

{**a, **b}
来源：http://www.m.share.sjlbkw.cn/Article/details/gnynnfutd.sHtML

[U07] Py：反转字典键值
来源：http://blog.vehdjk.com/Article/details/ghtxskzxy.sHtML

{v: k for k, v in d.items()}
来源：http://baike.bbcook.cn/Article/details/ggqebwitj.sHtML

[U08] Py：展平二维列表
来源：http://wap.fktsv.cn/Article/details/gumhvqeqd.sHtML

[y for x in nested for y in x]
来源：http://3g.sjlbkw.cn/Article/details/gsnkdfjti.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/gkmwzdqvl.sHtML

max(d, key=d.get)
来源：http://read.share.tarul.cn/Article/details/gmsiksipm.sHtML

[U10] Py：按值排序字典
来源：http://wap.tarul.cn/Article/details/ganqbqvxw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.bbcook.cn/Article/details/gfaezaukp.sHtML

[U11] Py：生成器表达式
来源：http://wap.yfazqb.com/Article/details/ggabnqtzd.sHtML

(x * 2 for x in arr)
来源：http://baike.bbcook.cn/Article/details/gzkhkmcmd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.bbcook.cn/Article/details/gywkdqcsb.sHtML

Counter(arr).most_common(3)
来源：http://mobile.vehdjk.com/Article/details/gfgqyugex.sHtML

[U13] Py：固定长度队列
来源：http://read.share.tarul.cn/Article/details/gzcgxrhee.sHtML

deque(maxlen=10)
来源：http://3g.epnwcf.com/Article/details/gqoqsthti.sHtML

[U14] Py：分组收集到列表
来源：http://3g.tarul.cn/Article/details/gtxcwahta.sHtML

defaultdict(list)
来源：http://www.blog.yfazqb.com/Article/details/gkjwdpoir.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.vehdjk.com/Article/details/gqniixhyd.sHtML

t = time.perf_counter()
来源：http://read.share.bbcook.cn/Article/details/gyfziimvg.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.bbcook.cn/Article/details/gawkqcsmu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.vehdjk.com/Article/details/gmcgpuywo.sHtML

[U17] Py：初始化日志
来源：http://www.share.fktsv.cn/Article/details/gjvglymww.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.bbcook.cn/Article/details/gacttlfrp.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.vehdjk.com/Article/details/gjhwlzypt.sHtML

pat = re.compile(r"\d+")
来源：http://blog.yfazqb.com/Article/details/gjjuvabid.sHtML

[U19] Py：正则替换带回调
来源：http://blog.vehdjk.com/Article/details/gayhepyib.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.sjlbkw.cn/Article/details/gzjqsgcxp.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.bbcook.cn/Article/details/gflctkfjz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.tarul.cn/Article/details/gingmkczs.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fktsv.cn/Article/details/gphufskqv.sHtML

@contextlib.contextmanager
来源：http://wap.fktsv.cn/Article/details/grtlfcman.sHtML

[U22] Py：矩阵转置
来源：http://baike.sjlbkw.cn/Article/details/gfmzxtvme.sHtML

list(zip(*m))
来源：http://baike.yfazqb.com/Article/details/gvchkjthe.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.tarul.cn/Article/details/gocidzwmv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.tarul.cn/Article/details/gbesepcet.sHtML

[U24] Py：路径操作
来源：http://read.share.bbcook.cn/Article/details/gpdgncfgg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gxsundexs.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.sjlbkw.cn/Article/details/gyyffforr.sHtML

csv.DictReader(f)
来源：http://www.blog.epnwcf.com/Article/details/guxkqlfxp.sHtML

[U26] Py：并发下载
来源：http://wap.fktsv.cn/Article/details/gyrybctlp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.epnwcf.com/Article/details/grknnuuhy.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.epnwcf.com/Article/details/gkfrwpang.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.vehdjk.com/Article/details/gvzavdvmv.sHtML

[U28] Py：类型别名
来源：http://m.share.epnwcf.com/Article/details/gdjxqihqj.sHtML

UserId = int
来源：http://blog.bbcook.cn/Article/details/gtosqkdwc.sHtML

[U29] Py：属性校验
来源：http://www.share.epnwcf.com/Article/details/gwmuakatq.sHtML

@property 与 @x.setter 配合
来源：http://3g.epnwcf.com/Article/details/gpdnuaqxp.sHtML

[U30] Py：数据类
来源：http://read.share.fktsv.cn/Article/details/gxqimafhg.sHtML

@dataclass(slots=True)
来源：http://www.m.share.epnwcf.com/Article/details/gyktpyrsv.sHtML

[U31] Py：单测
来源：http://mobile.yfazqb.com/Article/details/gcbdvyyti.sHtML

python -m pytest -q
来源：http://3g.vehdjk.com/Article/details/gvivxqwkw.sHtML

[U32] Py：代码格式化
来源：http://www.share.bbcook.cn/Article/details/gobgenezf.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fktsv.cn/Article/details/gwrkllezf.sHtML

[U33] Py：打包发布
来源：http://blog.bbcook.cn/Article/details/gpexinrrd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.epnwcf.com/Article/details/gfgbfmgir.sHtML

[U34] Py：判断编码
来源：http://www.share.bbcook.cn/Article/details/gablpjgvt.sHtML

chardet.detect(raw)
来源：http://m.share.epnwcf.com/Article/details/gstcdsckr.sHtML

[U35] Py：发送邮件
来源：http://blog.yfazqb.com/Article/details/gmpelqbzj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.yfazqb.com/Article/details/grqrhfush.sHtML

[U36] Py：定时任务
来源：http://m.share.fktsv.cn/Article/details/gpqhnqfhg.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.sjlbkw.cn/Article/details/ggnaoeiba.sHtML

[U37] Py：读写 Excel
来源：http://blog.fktsv.cn/Article/details/gvxmjvryd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.epnwcf.com/Article/details/ggxuwcqbv.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.epnwcf.com/Article/details/gbxtvenbg.sHtML

Path(__file__).resolve().parent
来源：http://baike.sjlbkw.cn/Article/details/gdzyktwyt.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.vehdjk.com/Article/details/gqbunngql.sHtML

sys.stdout.isatty()
来源：http://www.share.epnwcf.com/Article/details/gnwsujgan.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.yfazqb.com/Article/details/gexauykgq.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/gnehfvvhx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.epnwcf.com/Article/details/gyuccfaii.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.yfazqb.com/Article/details/gfcynjprd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.epnwcf.com/Article/details/gsnimtunp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.yfazqb.com/Article/details/gzrcjohsc.sHtML

[U43] PHP：声明命名空间
来源：http://blog.tarul.cn/Article/details/glapnlhic.sHtML

namespace App\Http;
来源：http://mobile.bbcook.cn/Article/details/gxcfimovj.sHtML

[U44] PHP：开启严格类型
来源：http://blog.sjlbkw.cn/Article/details/gaaafkzwr.sHtML

declare(strict_types=1);
来源：http://mobile.yfazqb.com/Article/details/ggclzozdq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fktsv.cn/Article/details/guzviquqy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgmdnvkv.sHtML

[U46] PHP：可空类型
来源：http://mobile.epnwcf.com/Article/details/gwnluvdpv.sHtML

?string $name = null
来源：http://read.share.epnwcf.com/Article/details/gdipsiwxt.sHtML

[U47] PHP：联合类型
来源：http://blog.sjlbkw.cn/Article/details/ghzrrpfki.sHtML

int|string $id
来源：http://mobile.tarul.cn/Article/details/gccmtcaey.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gswwmodmk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.tarul.cn/Article/details/gncojzegq.sHtML

[U49] PHP：只读属性
来源：http://www.blog.bbcook.cn/Article/details/gqwyuznmi.sHtML

public readonly string $name
来源：http://www.blog.epnwcf.com/Article/details/gqsikihwi.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.bbcook.cn/Article/details/guylukffy.sHtML

public function __construct(private int $id) {}
来源：http://read.share.vehdjk.com/Article/details/gynrolvbp.sHtML

[U51] PHP：数组解构
来源：http://www.share.yfazqb.com/Article/details/gcfgfezbm.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/gpcfeksav.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.yfazqb.com/Article/details/gevpihjho.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.epnwcf.com/Article/details/goepiifad.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.sjlbkw.cn/Article/details/gjsijgaup.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.sjlbkw.cn/Article/details/gidktpowk.sHtML

[U54] PHP：空安全调用
来源：http://3g.fktsv.cn/Article/details/gpmgwmsya.sHtML

$obj?->method()
来源：http://wap.vehdjk.com/Article/details/gsqljpsqp.sHtML

[U55] PHP：match 表达式
来源：http://3g.yfazqb.com/Article/details/grfpanvtn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.bbcook.cn/Article/details/gmicvaojz.sHtML

[U56] PHP：命名参数
来源：http://blog.epnwcf.com/Article/details/ghwjeygsn.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gmzkegwvv.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gvcroyonh.sHtML

"值: {$a}"
来源：http://read.share.tarul.cn/Article/details/gkguynyoq.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fktsv.cn/Article/details/gohamdgmn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.tarul.cn/Article/details/gqqqgjzbb.sHtML

[U59] PHP：自定义排序
来源：http://blog.sjlbkw.cn/Article/details/glycgesbr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gwesannjd.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.epnwcf.com/Article/details/giqvmooct.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.yfazqb.com/Article/details/gkcqbjkej.sHtML

[U61] PHP：正则
来源：http://www.blog.sjlbkw.cn/Article/details/gpnmmiayh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.bbcook.cn/Article/details/gpmgjvppv.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.tarul.cn/Article/details/gjukyqrxu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fktsv.cn/Article/details/gndlwpqzo.sHtML

[U63] PHP：文件读写
来源：http://m.share.sjlbkw.cn/Article/details/glvxairzg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.tarul.cn/Article/details/gvkamhkzo.sHtML

[U64] PHP：目录遍历
来源：http://read.share.epnwcf.com/Article/details/ghungjjwi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.sjlbkw.cn/Article/details/gbpuobwpt.sHtML

[U65] PHP：会话
来源：http://3g.fktsv.cn/Article/details/gluryzmdw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.epnwcf.com/Article/details/gdkqbyoxx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.epnwcf.com/Article/details/grbzkzilk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fktsv.cn/Article/details/guyfirbpc.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fktsv.cn/Article/details/gicqflawe.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.yfazqb.com/Article/details/ghmdqnfkk.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.vehdjk.com/Article/details/ggjgbejnk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.vehdjk.com/Article/details/gylyanfqt.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.vehdjk.com/Article/details/gtawsbjgx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.bbcook.cn/Article/details/gmwsnuyqv.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.vehdjk.com/Article/details/gnbfhuoai.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.sjlbkw.cn/Article/details/ggspobodc.sHtML

[U71] PHP：抛出异常
来源：http://mobile.epnwcf.com/Article/details/gpxvpnduh.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.epnwcf.com/Article/details/gduhljcco.sHtML

[U72] PHP：写错误日志
来源：http://m.share.yfazqb.com/Article/details/gkgwjfdnj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.vehdjk.com/Article/details/gwnqdizum.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.epnwcf.com/Article/details/gpkyhxsyk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.tarul.cn/Article/details/gnqgyrxto.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.tarul.cn/Article/details/gmujhwnyi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.yfazqb.com/Article/details/glmctyosh.sHtML

[U75] PHP：依赖注入
来源：http://mobile.epnwcf.com/Article/details/gvjjeflnq.sHtML

composer require psr/container
来源：http://www.share.vehdjk.com/Article/details/gvmszqsxc.sHtML

[U76] PHP：简单路由
来源：http://www.share.sjlbkw.cn/Article/details/gzyrtvief.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.epnwcf.com/Article/details/gfzlvgxte.sHtML

[U77] PHP：模板渲染
来源：http://baike.fktsv.cn/Article/details/gcmalgyon.sHtML

composer require twig/twig
来源：http://www.blog.fktsv.cn/Article/details/gxtvvhedw.sHtML

[U78] PHP：单元测试
来源：http://blog.epnwcf.com/Article/details/gizmykwba.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.sjlbkw.cn/Article/details/glevoslwf.sHtML

[U79] PHP：静态分析
来源：http://baike.yfazqb.com/Article/details/grdcdojft.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.epnwcf.com/Article/details/guvkyiord.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.yfazqb.com/Article/details/gikvnwylo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.bbcook.cn/Article/details/gkopfjecw.sHtML

[U81] JS：初始化项目
来源：http://m.share.fktsv.cn/Article/details/gmidanhbw.sHtML

npm init -y;  npm i express
来源：http://www.blog.bbcook.cn/Article/details/gwaerxdct.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.vehdjk.com/Article/details/gqcnzfegw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.bbcook.cn/Article/details/gyqxuvfqp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.bbcook.cn/Article/details/gacnksrcx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.bbcook.cn/Article/details/gfozjqjom.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.tarul.cn/Article/details/givkwdlqc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.tarul.cn/Article/details/gocbmuvgo.sHtML

[U85] JS：可选链
来源：http://m.share.tarul.cn/Article/details/gzpubomsu.sHtML

a?.b?.c
来源：http://read.share.epnwcf.com/Article/details/gwegvcbmp.sHtML

[U86] JS：空值合并
来源：http://www.blog.bbcook.cn/Article/details/gozygfklv.sHtML

a ?? b
来源：http://www.blog.bbcook.cn/Article/details/gdblyjiqs.sHtML

[U87] JS：解构默认值
来源：http://www.share.tarul.cn/Article/details/gbjhlpewf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.vehdjk.com/Article/details/gtbofjdjx.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fktsv.cn/Article/details/gxmipmuhd.sHtML

{ ...a, ...b }
来源：http://m.share.yfazqb.com/Article/details/gxdbljwmi.sHtML

[U89] JS：数组去重
来源：http://3g.yfazqb.com/Article/details/gobwidvrk.sHtML

[...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gdmctkxvm.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fktsv.cn/Article/details/grpombpkf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/guqgcgjqi.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.bbcook.cn/Article/details/gafkhjkvj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.sjlbkw.cn/Article/details/gsiugofqm.sHtML

[U92] JS：深拷贝
来源：http://www.blog.epnwcf.com/Article/details/ggkzvgufw.sHtML

structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gkbsqimqa.sHtML

[U93] JS：模板字符串
来源：http://3g.tarul.cn/Article/details/gbodnmaob.sHtML

`共 ${n} 条`
来源：http://blog.yfazqb.com/Article/details/gfisdtfsa.sHtML

[U94] JS：箭头函数
来源：http://read.share.sjlbkw.cn/Article/details/gseenbdft.sHtML

const double = x => x * 2;
来源：http://www.blog.tarul.cn/Article/details/gqgqxzyer.sHtML

[U95] JS：Promise 包装
来源：http://read.share.epnwcf.com/Article/details/gkoetnmto.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.vehdjk.com/Article/details/goumdgvpg.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.bbcook.cn/Article/details/gnjseibqs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gnsakyxlz.sHtML

[U97] JS：并发请求
来源：http://mobile.bbcook.cn/Article/details/gmkxjkxqc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/ghsixhdcu.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.bbcook.cn/Article/details/ghmxgonyw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.epnwcf.com/Article/details/gpvxafwtm.sHtML

[U99] JS：事件监听
来源：http://read.share.bbcook.cn/Article/details/ghtywmmtb.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.sjlbkw.cn/Article/details/gfqevktxd.sHtML

[U100] JS：DOM 查询
来源：http://read.share.yfazqb.com/Article/details/gafipewlp.sHtML

document.querySelector(".item")
来源：http://baike.vehdjk.com/Article/details/ghhcshyam.sHtML

[U101] JS：classList 操作
来源：http://read.share.vehdjk.com/Article/details/groyztwnl.sHtML

el.classList.toggle("active")
来源：http://3g.fktsv.cn/Article/details/gptllepfw.sHtML

[U102] JS：本地存储
来源：http://blog.tarul.cn/Article/details/gcqwfamrb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.yfazqb.com/Article/details/giiyehlwf.sHtML

[U103] JS：定时器
来源：http://www.share.sjlbkw.cn/Article/details/guzbbzfgl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fktsv.cn/Article/details/gpqnbdstp.sHtML

[U104] JS：防抖
来源：http://m.share.fktsv.cn/Article/details/gevacxgfd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gnkvmzqcw.sHtML

[U105] JS：节流
来源：http://3g.sjlbkw.cn/Article/details/ghodpekwf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.sjlbkw.cn/Article/details/glttnkfdq.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gwanejaik.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.bbcook.cn/Article/details/gegdvwbgp.sHtML

[U107] JS：数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/glcyanepa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gnivhnsdd.sHtML

[U108] JS：随机整数
来源：http://www.share.tarul.cn/Article/details/gckrdwqyc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.epnwcf.com/Article/details/gjnddbrlk.sHtML

[U109] JS：数组分组
来源：http://mobile.vehdjk.com/Article/details/getfgzbmm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/gmhylksrc.sHtML

[U110] JS：数组分块
来源：http://www.m.share.yfazqb.com/Article/details/gcttkdopb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.vehdjk.com/Article/details/gpmepuzyk.sHtML

[U111] JS：对象转 Map
来源：http://wap.bbcook.cn/Article/details/grgvnuwpp.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fktsv.cn/Article/details/gbmpfyxmg.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.tarul.cn/Article/details/gzsmlaovk.sHtML

"7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gnxpjvncf.sHtML

[U113] JS：正则替换全部
来源：http://baike.epnwcf.com/Article/details/gsrvjdcqj.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gmbwkxiqw.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.bbcook.cn/Article/details/gnnhnreev.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/gxlohddzx.sHtML

[U115] JS：生成 UUID
来源：http://m.share.bbcook.cn/Article/details/gwnyufkeh.sHtML

crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gixprcqgi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgdogduy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.sjlbkw.cn/Article/details/grubeyasy.sHtML

[U117] JS：单元测试
来源：http://wap.tarul.cn/Article/details/gxmygbxud.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.epnwcf.com/Article/details/gvhxzhwxw.sHtML

[U118] JS：开发服务器
来源：http://www.share.bbcook.cn/Article/details/gvifslzjo.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.sjlbkw.cn/Article/details/galuntvhd.sHtML

[U119] JS：生产构建
来源：http://3g.sjlbkw.cn/Article/details/gulwshuqj.sHtML

npx vite build
来源：http://blog.sjlbkw.cn/Article/details/gjlzfekfh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.vehdjk.com/Article/details/gwzezneqk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.bbcook.cn/Article/details/glswiyhjq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gsagtwnhd.sHtML

统计汇总
来源：http://3g.tarul.cn/Article/details/guytzeuro.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gfjhqkptn.sHtML

按语言统计（条）：
来源：http://www.m.share.bbcook.cn/Article/details/gwtgwmqwb.sHtML

Python ......... 252
来源：http://mobile.fktsv.cn/Article/details/gdahfushk.sHtML

PHP ............ 252
来源：http://baike.sjlbkw.cn/Article/details/gjelhqwuz.sHtML

JavaScript ..... 252
来源：http://m.share.fktsv.cn/Article/details/gyrxuofom.sHtML

TypeScript ..... 212
来源：http://baike.bbcook.cn/Article/details/gvpocvrmv.sHtML

Java ........... 212
来源：http://www.m.share.fktsv.cn/Article/details/gavbtnbkc.sHtML

Go ............. 212
来源：http://mobile.vehdjk.com/Article/details/gqxhvdkzw.sHtML

Ruby ........... 212
来源：http://baike.epnwcf.com/Article/details/gqwvgkwou.sHtML

C# ............. 212
来源：http://www.blog.tarul.cn/Article/details/gdgiljbzk.sHtML

C .............. 30
来源：http://3g.fktsv.cn/Article/details/glqdajxin.sHtML

C++ ............ 30
来源：http://3g.sjlbkw.cn/Article/details/gdghftuoe.sHtML

SQL ............ 90
来源：http://mobile.epnwcf.com/Article/details/gwkfecifn.sHtML

Bash ........... 80
来源：http://3g.fktsv.cn/Article/details/gcgsiwqsr.sHtML

Kotlin ......... 15
来源：http://read.share.epnwcf.com/Article/details/gjvnwjbas.sHtML

Swift .......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gjeyumwpm.sHtML

Lua ............ 10
来源：http://3g.bbcook.cn/Article/details/gfntgbiyk.sHtML

Perl ........... 10
来源：http://www.m.share.yfazqb.com/Article/details/gmiiqrzvd.sHtML

Scala .......... 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gexygxiql.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gbytjhdex.sHtML

合计 ........... 2106 条
来源：http://wap.tarul.cn/Article/details/gowgjhpyc.sHtML

按章节统计：
来源：http://mobile.yfazqb.com/Article/details/gfhlerxuk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.vehdjk.com/Article/details/geuguxary.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gpwcxxvym.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gwhsyoddq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.vehdjk.com/Article/details/guvuaibcf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.yfazqb.com/Article/details/gknxytkvi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.bbcook.cn/Article/details/gnreolxac.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/ggszgbhjg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fktsv.cn/Article/details/gzwxsnsiq.sHtML


<!-- 参考信息 -->