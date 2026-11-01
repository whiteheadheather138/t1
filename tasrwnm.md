代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://blog.bbcook.cn/Article/details/goavohuhn.sHtML

[T51] Scala：Hello World
来源：http://3g.vehdjk.com/Article/details/gfzafgsda.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gslbmqqsd.sHtML

[T52] Scala：变量
来源：http://read.share.sjlbkw.cn/Article/details/gaoldrqxf.sHtML

val a = 1;  var b = 2
来源：http://baike.bbcook.cn/Article/details/glqxrjvqd.sHtML

[T53] Scala：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gsftoomqo.sHtML

s"值: $b"
来源：http://wap.vehdjk.com/Article/details/gnepoewpn.sHtML

[T54] Scala：集合映射
来源：http://www.share.yfazqb.com/Article/details/gpqpjhuxl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.vehdjk.com/Article/details/gaohxrwxh.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gzquirabf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.sjlbkw.cn/Article/details/gfqpokkwi.sHtML

[T56] Scala：样例类
来源：http://baike.bbcook.cn/Article/details/gfhcvxjgp.sHtML

case class User(name: String, age: Int)
来源：http://3g.tarul.cn/Article/details/gsqgrsofe.sHtML

[T57] Scala：模式匹配
来源：http://wap.bbcook.cn/Article/details/gqtsxqagy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.bbcook.cn/Article/details/gdqucikor.sHtML

[T58] Scala：函数定义
来源：http://3g.tarul.cn/Article/details/guqnftzly.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.tarul.cn/Article/details/ggjgfwndy.sHtML

[T59] Scala：循环
来源：http://m.share.sjlbkw.cn/Article/details/gbwyummid.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gzrogcvfo.sHtML

[T60] Scala：折叠
来源：http://www.blog.sjlbkw.cn/Article/details/gcmfwyxmg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.bbcook.cn/Article/details/gwbethadp.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gjuspgkbo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/ghekldezv.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gmuwplnob.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.vehdjk.com/Article/details/gowhpxhmp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.sjlbkw.cn/Article/details/grmkyuckj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fktsv.cn/Article/details/gzazflioi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.sjlbkw.cn/Article/details/getmugjqh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.epnwcf.com/Article/details/gvnekenjq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.tarul.cn/Article/details/grdqezbay.sHtML

[U04] Py：变量调试打印
来源：http://www.share.yfazqb.com/Article/details/gnywqdnhv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.tarul.cn/Article/details/gsfgcgfkk.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.sjlbkw.cn/Article/details/gvwfxhwci.sHtML

list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/glyyhvlnc.sHtML

[U06] Py：合并两个字典
来源：http://baike.tarul.cn/Article/details/gtaapbnco.sHtML

{**a, **b}
来源：http://mobile.sjlbkw.cn/Article/details/ghytajnez.sHtML

[U07] Py：反转字典键值
来源：http://www.share.yfazqb.com/Article/details/gyrywpvrl.sHtML

{v: k for k, v in d.items()}
来源：http://wap.yfazqb.com/Article/details/gwysqpufz.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fktsv.cn/Article/details/gkryekakc.sHtML

[y for x in nested for y in x]
来源：http://blog.tarul.cn/Article/details/glvusbgnd.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.sjlbkw.cn/Article/details/gxxtfqihc.sHtML

max(d, key=d.get)
来源：http://3g.epnwcf.com/Article/details/gktqqyjnq.sHtML

[U10] Py：按值排序字典
来源：http://m.share.yfazqb.com/Article/details/gsnmdvrik.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.vehdjk.com/Article/details/gmzesqrld.sHtML

[U11] Py：生成器表达式
来源：http://wap.fktsv.cn/Article/details/gogylkfym.sHtML

(x * 2 for x in arr)
来源：http://baike.sjlbkw.cn/Article/details/gutyhvnkm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.epnwcf.com/Article/details/gxlpwakps.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/gsryfacwi.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.bbcook.cn/Article/details/gtzjkgumx.sHtML

deque(maxlen=10)
来源：http://www.m.share.yfazqb.com/Article/details/griomzlfn.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.yfazqb.com/Article/details/gkkxkqhrg.sHtML

defaultdict(list)
来源：http://mobile.yfazqb.com/Article/details/gkxrxwbmy.sHtML

[U15] Py：高精度计时
来源：http://baike.sjlbkw.cn/Article/details/grpmvnseu.sHtML

t = time.perf_counter()
来源：http://baike.vehdjk.com/Article/details/gvgisorpi.sHtML

[U16] Py：命令行参数解析
来源：http://baike.sjlbkw.cn/Article/details/gqzspdjzc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.bbcook.cn/Article/details/gwqxostpu.sHtML

[U17] Py：初始化日志
来源：http://www.share.fktsv.cn/Article/details/gsjfbqwxy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fktsv.cn/Article/details/gdpgxrvio.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fktsv.cn/Article/details/gihmobkuf.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/gbdskoirf.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.epnwcf.com/Article/details/gehjcxqqc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.epnwcf.com/Article/details/gaworzitt.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.sjlbkw.cn/Article/details/gmbjewnqy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.tarul.cn/Article/details/gxlpfjjqb.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.vehdjk.com/Article/details/grdcrfyxs.sHtML

@contextlib.contextmanager
来源：http://www.share.vehdjk.com/Article/details/gtnptdjxr.sHtML

[U22] Py：矩阵转置
来源：http://3g.tarul.cn/Article/details/gmwtpbuxl.sHtML

list(zip(*m))
来源：http://baike.yfazqb.com/Article/details/gyfropaul.sHtML

[U23] Py：分块读取大文件
来源：http://baike.bbcook.cn/Article/details/gwsoacprv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.vehdjk.com/Article/details/glwgstjdl.sHtML

[U24] Py：路径操作
来源：http://m.share.tarul.cn/Article/details/ghzodryoh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/guanfxwmo.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.tarul.cn/Article/details/geyqdktsg.sHtML

csv.DictReader(f)
来源：http://m.share.yfazqb.com/Article/details/gzphxrihj.sHtML

[U26] Py：并发下载
来源：http://www.blog.vehdjk.com/Article/details/gmbyjalmo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fktsv.cn/Article/details/gmnevejsd.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.epnwcf.com/Article/details/gkcnewivx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.tarul.cn/Article/details/guvgbtlgr.sHtML

[U28] Py：类型别名
来源：http://read.share.tarul.cn/Article/details/gequgtefq.sHtML

UserId = int
来源：http://3g.fktsv.cn/Article/details/gaixuueht.sHtML

[U29] Py：属性校验
来源：http://wap.yfazqb.com/Article/details/gfmgjuyvj.sHtML

@property 与 @x.setter 配合
来源：http://blog.epnwcf.com/Article/details/gpgbpcmkn.sHtML

[U30] Py：数据类
来源：http://www.share.epnwcf.com/Article/details/gdvpqgfbq.sHtML

@dataclass(slots=True)
来源：http://www.blog.vehdjk.com/Article/details/gejkcytvp.sHtML

[U31] Py：单测
来源：http://read.share.bbcook.cn/Article/details/gjveddwda.sHtML

python -m pytest -q
来源：http://mobile.epnwcf.com/Article/details/gfieksvib.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.bbcook.cn/Article/details/geqqyfvbx.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.epnwcf.com/Article/details/ghjaldubj.sHtML

[U33] Py：打包发布
来源：http://wap.vehdjk.com/Article/details/gksfpgwse.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.sjlbkw.cn/Article/details/gbndvqmpm.sHtML

[U34] Py：判断编码
来源：http://3g.bbcook.cn/Article/details/gmarinwnh.sHtML

chardet.detect(raw)
来源：http://baike.bbcook.cn/Article/details/gcytpsgwv.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.vehdjk.com/Article/details/gckgzmlav.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.tarul.cn/Article/details/geqrfssci.sHtML

[U36] Py：定时任务
来源：http://read.share.vehdjk.com/Article/details/gqblvggew.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fktsv.cn/Article/details/gtclxibft.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.vehdjk.com/Article/details/glfxkdiad.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.tarul.cn/Article/details/ghffatbiq.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.epnwcf.com/Article/details/gdqqtkxcb.sHtML

Path(__file__).resolve().parent
来源：http://m.share.yfazqb.com/Article/details/goctlwnll.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.epnwcf.com/Article/details/glwqvdrog.sHtML

sys.stdout.isatty()
来源：http://3g.fktsv.cn/Article/details/gzdqeieab.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.epnwcf.com/Article/details/gwgfociqo.sHtML

print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gecejmyed.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.vehdjk.com/Article/details/gzorxntbj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fktsv.cn/Article/details/gtlbirymc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.sjlbkw.cn/Article/details/gxfzinxpg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.sjlbkw.cn/Article/details/gzjvmobpw.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gwfuuekaj.sHtML

namespace App\Http;
来源：http://www.share.epnwcf.com/Article/details/gjhaaketo.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.vehdjk.com/Article/details/gqgtpaniw.sHtML

declare(strict_types=1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gihjavyru.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.tarul.cn/Article/details/gjbtszkqw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/ghhdjxnje.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.yfazqb.com/Article/details/gzpgqaenf.sHtML

?string $name = null
来源：http://blog.tarul.cn/Article/details/grxcojzfw.sHtML

[U47] PHP：联合类型
来源：http://m.share.epnwcf.com/Article/details/gulscdpra.sHtML

int|string $id
来源：http://m.share.sjlbkw.cn/Article/details/gzpjjimbm.sHtML

[U48] PHP：纯枚举
来源：http://wap.sjlbkw.cn/Article/details/genbhxitk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fktsv.cn/Article/details/gsnqssjne.sHtML

[U49] PHP：只读属性
来源：http://www.blog.tarul.cn/Article/details/gpwhxasfi.sHtML

public readonly string $name
来源：http://www.share.yfazqb.com/Article/details/gjgluhbvm.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.tarul.cn/Article/details/gmwbisnmu.sHtML

public function __construct(private int $id) {}
来源：http://www.share.yfazqb.com/Article/details/ggdvrkyxw.sHtML

[U51] PHP：数组解构
来源：http://www.blog.epnwcf.com/Article/details/gabwwgerp.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fktsv.cn/Article/details/gmcrwetux.sHtML

[U52] PHP：箭头函数
来源：http://mobile.vehdjk.com/Article/details/gkvajgsto.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.vehdjk.com/Article/details/galuykwmc.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fktsv.cn/Article/details/gcnzerjrh.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.epnwcf.com/Article/details/gvesorrmk.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fktsv.cn/Article/details/ghekxrwyi.sHtML

$obj?->method()
来源：http://www.blog.bbcook.cn/Article/details/gxlfrvgnw.sHtML

[U55] PHP：match 表达式
来源：http://3g.epnwcf.com/Article/details/ggqxmfkii.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.sjlbkw.cn/Article/details/giaejspqz.sHtML

[U56] PHP：命名参数
来源：http://read.share.yfazqb.com/Article/details/gzyemkszh.sHtML

f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/glhtstapz.sHtML

[U57] PHP：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gnjtlasdm.sHtML

"值: {$a}"
来源：http://www.share.sjlbkw.cn/Article/details/gcamkcddh.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fktsv.cn/Article/details/grjnqtrqf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.yfazqb.com/Article/details/glyewiuqi.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.bbcook.cn/Article/details/gftxnlrht.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.yfazqb.com/Article/details/gbnyhnhoa.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.sjlbkw.cn/Article/details/gctfrczvq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.vehdjk.com/Article/details/gihilydka.sHtML

[U61] PHP：正则
来源：http://www.share.vehdjk.com/Article/details/ggeftjprm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/gyfhstipw.sHtML

[U62] PHP：日期对象
来源：http://m.share.epnwcf.com/Article/details/gkwakewro.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.tarul.cn/Article/details/gmtyzdopo.sHtML

[U63] PHP：文件读写
来源：http://www.blog.tarul.cn/Article/details/gwvebftsh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.yfazqb.com/Article/details/gxrhmpyhk.sHtML

[U64] PHP：目录遍历
来源：http://mobile.epnwcf.com/Article/details/gwxvhbviv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.tarul.cn/Article/details/gndqckjko.sHtML

[U65] PHP：会话
来源：http://baike.bbcook.cn/Article/details/gissotpjn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.bbcook.cn/Article/details/gqrybqddv.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.vehdjk.com/Article/details/gfpsxeoof.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.vehdjk.com/Article/details/gtxyjvqex.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fktsv.cn/Article/details/glctwwxej.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fktsv.cn/Article/details/gioosemup.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.yfazqb.com/Article/details/gkjcgqatn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.epnwcf.com/Article/details/gvwfdshcr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.vehdjk.com/Article/details/gynxwytoj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.vehdjk.com/Article/details/gminjeilc.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.vehdjk.com/Article/details/gbpujkfur.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.vehdjk.com/Article/details/guyxykchb.sHtML

[U71] PHP：抛出异常
来源：http://baike.vehdjk.com/Article/details/glfqzkrqu.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.vehdjk.com/Article/details/gvszeewht.sHtML

[U72] PHP：写错误日志
来源：http://m.share.bbcook.cn/Article/details/gfmmlqten.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fktsv.cn/Article/details/ggnggrhle.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.yfazqb.com/Article/details/gnodkarks.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.epnwcf.com/Article/details/gacvwsyxe.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gzhmjsept.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.bbcook.cn/Article/details/gavxbsdyp.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fktsv.cn/Article/details/gnvsmvlvb.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/giwmyykxp.sHtML

[U76] PHP：简单路由
来源：http://blog.epnwcf.com/Article/details/gndqctmme.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.vehdjk.com/Article/details/ggheoinwm.sHtML

[U77] PHP：模板渲染
来源：http://www.share.tarul.cn/Article/details/gphxzdkwq.sHtML

composer require twig/twig
来源：http://wap.yfazqb.com/Article/details/gworajecn.sHtML

[U78] PHP：单元测试
来源：http://read.share.yfazqb.com/Article/details/gzsmanhqx.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.sjlbkw.cn/Article/details/gioifgqzq.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.vehdjk.com/Article/details/gmhuuwrvz.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.vehdjk.com/Article/details/gsltzyfth.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.tarul.cn/Article/details/gurabcvyz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.epnwcf.com/Article/details/gyywljnhw.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fktsv.cn/Article/details/gqkazankw.sHtML

npm init -y;  npm i express
来源：http://www.share.epnwcf.com/Article/details/ghzgpwkvp.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.sjlbkw.cn/Article/details/gyiosmqpj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fktsv.cn/Article/details/gacjmcfzx.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.vehdjk.com/Article/details/gnmusepob.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.yfazqb.com/Article/details/gfayeilmi.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.vehdjk.com/Article/details/gxofpoxew.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fktsv.cn/Article/details/gtjeizvtc.sHtML

[U85] JS：可选链
来源：http://blog.yfazqb.com/Article/details/ghguuwoqe.sHtML

a?.b?.c
来源：http://www.m.share.epnwcf.com/Article/details/gwsueihog.sHtML

[U86] JS：空值合并
来源：http://m.share.sjlbkw.cn/Article/details/giuxkqvjb.sHtML

a ?? b
来源：http://read.share.fktsv.cn/Article/details/gvszaoomb.sHtML

[U87] JS：解构默认值
来源：http://www.share.tarul.cn/Article/details/gmnpcoiut.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fktsv.cn/Article/details/gloytxyme.sHtML

[U88] JS：对象展开合并
来源：http://wap.tarul.cn/Article/details/gfvolwzwg.sHtML

{ ...a, ...b }
来源：http://wap.sjlbkw.cn/Article/details/gornciqux.sHtML

[U89] JS：数组去重
来源：http://www.m.share.epnwcf.com/Article/details/guttqxvkx.sHtML

[...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/ghkkyoymv.sHtML

[U90] JS：数字数组排序
来源：http://www.share.tarul.cn/Article/details/gsultimfz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gbyjothii.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fktsv.cn/Article/details/gcknhuxwh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.bbcook.cn/Article/details/gvfcmrctm.sHtML

[U92] JS：深拷贝
来源：http://www.blog.tarul.cn/Article/details/guemdktzw.sHtML

structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gzvqxgutb.sHtML

[U93] JS：模板字符串
来源：http://read.share.yfazqb.com/Article/details/gykoaxwff.sHtML

`共 ${n} 条`
来源：http://www.share.vehdjk.com/Article/details/gpcyrmqyd.sHtML

[U94] JS：箭头函数
来源：http://baike.epnwcf.com/Article/details/gxbfetrly.sHtML

const double = x => x * 2;
来源：http://www.m.share.bbcook.cn/Article/details/goegiwrfn.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.bbcook.cn/Article/details/gkriwrgby.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.tarul.cn/Article/details/gdhtrttcp.sHtML

[U96] JS：async/await 与异常
来源：http://baike.vehdjk.com/Article/details/gtkngsink.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gvpueijwt.sHtML

[U97] JS：并发请求
来源：http://baike.yfazqb.com/Article/details/gmgivrbaa.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gnrcckorj.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.epnwcf.com/Article/details/gjtkhapki.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.sjlbkw.cn/Article/details/ghxbjalpo.sHtML

[U99] JS：事件监听
来源：http://www.share.epnwcf.com/Article/details/gsmuoxfad.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.yfazqb.com/Article/details/gxtmroxmx.sHtML

[U100] JS：DOM 查询
来源：http://3g.vehdjk.com/Article/details/gynuurcdz.sHtML

document.querySelector(".item")
来源：http://wap.bbcook.cn/Article/details/ghomahvyl.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.epnwcf.com/Article/details/galevyrnm.sHtML

el.classList.toggle("active")
来源：http://m.share.fktsv.cn/Article/details/germsmyrl.sHtML

[U102] JS：本地存储
来源：http://wap.tarul.cn/Article/details/gwptuyivm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.vehdjk.com/Article/details/gyynejkpd.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/gprdtiooc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fktsv.cn/Article/details/gsharbhsy.sHtML

[U104] JS：防抖
来源：http://www.share.bbcook.cn/Article/details/gpnrukmzi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gdamrzird.sHtML

[U105] JS：节流
来源：http://www.blog.bbcook.cn/Article/details/giiqriigq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.bbcook.cn/Article/details/gshkkvlul.sHtML

[U106] JS：日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gaqfhrvpp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.bbcook.cn/Article/details/gkuczhwyn.sHtML

[U107] JS：数字千分位
来源：http://wap.sjlbkw.cn/Article/details/gofjlpsgr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.tarul.cn/Article/details/gpysnwkvj.sHtML

[U108] JS：随机整数
来源：http://blog.yfazqb.com/Article/details/gvxowgvem.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.vehdjk.com/Article/details/geotozcnz.sHtML

[U109] JS：数组分组
来源：http://m.share.tarul.cn/Article/details/ghtalxdof.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/gzeuukbws.sHtML

[U110] JS：数组分块
来源：http://mobile.sjlbkw.cn/Article/details/gwimvtvst.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.epnwcf.com/Article/details/gjgkuzliv.sHtML

[U111] JS：对象转 Map
来源：http://3g.yfazqb.com/Article/details/gvluwlhxu.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fktsv.cn/Article/details/ghahyntbx.sHtML

[U112] JS：字符串补位
来源：http://blog.fktsv.cn/Article/details/gvvqxjpre.sHtML

"7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gmpezevvf.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.sjlbkw.cn/Article/details/gvnnpuzxy.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gjiptezkq.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.tarul.cn/Article/details/gctiofesq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbajjxub.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/grduzkxvu.sHtML

crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gjgkuoflw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fktsv.cn/Article/details/gfsmfwbnn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.vehdjk.com/Article/details/gojtvuxba.sHtML

[U117] JS：单元测试
来源：http://www.blog.bbcook.cn/Article/details/gqnoaqhju.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.yfazqb.com/Article/details/gbokhsexx.sHtML

[U118] JS：开发服务器
来源：http://m.share.epnwcf.com/Article/details/ghrmmvblg.sHtML

npm i -D vite;  npx vite
来源：http://blog.tarul.cn/Article/details/gcodwuvvt.sHtML

[U119] JS：生产构建
来源：http://mobile.epnwcf.com/Article/details/getvvmzjl.sHtML

npx vite build
来源：http://www.share.yfazqb.com/Article/details/gjodjshlu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fktsv.cn/Article/details/gxghoizfe.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.bbcook.cn/Article/details/gmybqjjpn.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwdyvachk.sHtML

统计汇总
来源：http://3g.epnwcf.com/Article/details/gvtvkethz.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gsmeideot.sHtML

按语言统计（条）：
来源：http://m.share.sjlbkw.cn/Article/details/gdgilxvaq.sHtML

Python ......... 252
来源：http://www.blog.yfazqb.com/Article/details/gmitpfbar.sHtML

PHP ............ 252
来源：http://m.share.epnwcf.com/Article/details/giowjttxq.sHtML

JavaScript ..... 252
来源：http://read.share.vehdjk.com/Article/details/gdlcfordu.sHtML

TypeScript ..... 212
来源：http://www.blog.tarul.cn/Article/details/gsmkizhue.sHtML

Java ........... 212
来源：http://www.blog.fktsv.cn/Article/details/grmcwppfi.sHtML

Go ............. 212
来源：http://www.m.share.bbcook.cn/Article/details/gierxpetm.sHtML

Ruby ........... 212
来源：http://baike.tarul.cn/Article/details/gdojjbbxg.sHtML

C# ............. 212
来源：http://blog.fktsv.cn/Article/details/gqjzddagh.sHtML

C .............. 30
来源：http://www.blog.vehdjk.com/Article/details/gylwplnsl.sHtML

C++ ............ 30
来源：http://www.m.share.vehdjk.com/Article/details/gaealkvva.sHtML

SQL ............ 90
来源：http://www.blog.fktsv.cn/Article/details/govexzzpj.sHtML

Bash ........... 80
来源：http://www.m.share.sjlbkw.cn/Article/details/gphrblcai.sHtML

Kotlin ......... 15
来源：http://www.m.share.vehdjk.com/Article/details/glitibfef.sHtML

Swift .......... 15
来源：http://3g.tarul.cn/Article/details/gowpjpqce.sHtML

Lua ............ 10
来源：http://read.share.yfazqb.com/Article/details/gxqbrsrhr.sHtML

Perl ........... 10
来源：http://3g.vehdjk.com/Article/details/gqpahchiv.sHtML

Scala .......... 10
来源：http://www.blog.fktsv.cn/Article/details/gzrnidthc.sHtML

------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gxescdnpg.sHtML

合计 ........... 2106 条
来源：http://blog.bbcook.cn/Article/details/ggfohoqfj.sHtML

按章节统计：
来源：http://blog.sjlbkw.cn/Article/details/glmnsvnzb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/grywrukcb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/gzidgxfdp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gugikcjso.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.bbcook.cn/Article/details/ghkgkkdqy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.bbcook.cn/Article/details/gdeurtynx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.yfazqb.com/Article/details/gblcxihnz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gpfoouagn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/gwurppitd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/gjvghyjgz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.yfazqb.com/Article/details/gvrqhsnfc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gndvevrpo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gakxssimn.sHtML


<!-- 参考信息 -->