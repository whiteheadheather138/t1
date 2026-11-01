代发 wailian999

[T49] Perl：函数
来源：http://wap.tarul.cn/Article/details/gtqgaitnv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gwwrdjcgx.sHtML

[T50] Perl：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gdvnpjijg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.sjlbkw.cn/Article/details/gccsgzonb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.tarul.cn/Article/details/gvgiugoyq.sHtML

[T51] Scala：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gmtdhlaaz.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gmrfpggrz.sHtML

[T52] Scala：变量
来源：http://read.share.fktsv.cn/Article/details/ggxpcbkkb.sHtML

val a = 1;  var b = 2
来源：http://mobile.yfazqb.com/Article/details/gdmorjhdq.sHtML

[T53] Scala：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gkklaxnto.sHtML

s"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gfoqrfmun.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/gdjbygkky.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/gvfaaujra.sHtML

[T55] Scala：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/gsxjyuxya.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.epnwcf.com/Article/details/gkhstwnxb.sHtML

[T56] Scala：样例类
来源：http://read.share.yfazqb.com/Article/details/gjhvmfkvr.sHtML

case class User(name: String, age: Int)
来源：http://read.share.yfazqb.com/Article/details/grhkzwlcq.sHtML

[T57] Scala：模式匹配
来源：http://m.share.vehdjk.com/Article/details/gcfegxdbj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fktsv.cn/Article/details/gatpfeofc.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fktsv.cn/Article/details/gcsuofgos.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.yfazqb.com/Article/details/gmjkikaqh.sHtML

[T59] Scala：循环
来源：http://mobile.epnwcf.com/Article/details/gdrldquyc.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gonpwnskk.sHtML

[T60] Scala：折叠
来源：http://wap.sjlbkw.cn/Article/details/gfqxrgbii.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.yfazqb.com/Article/details/gznxwpclu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gyvbdbrmf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/gzjwossnu.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gspbzulqm.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.sjlbkw.cn/Article/details/ghhlmkghu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.vehdjk.com/Article/details/gfbooafub.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.vehdjk.com/Article/details/gmuqaxtan.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.yfazqb.com/Article/details/ggxeibsrz.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.tarul.cn/Article/details/gwltxwspw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.yfazqb.com/Article/details/giuhnawbr.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrblsyjs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.yfazqb.com/Article/details/gjpckzxqo.sHtML

[U05] Py：列表去重且保序
来源：http://blog.vehdjk.com/Article/details/gkmvbwzdy.sHtML

list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/gopzxtpkz.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.yfazqb.com/Article/details/gjeqyhjua.sHtML

{**a, **b}
来源：http://blog.yfazqb.com/Article/details/gcxvntioi.sHtML

[U07] Py：反转字典键值
来源：http://www.share.sjlbkw.cn/Article/details/gpgoedutm.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gjmofygqh.sHtML

[U08] Py：展平二维列表
来源：http://wap.epnwcf.com/Article/details/gxewietjb.sHtML

[y for x in nested for y in x]
来源：http://wap.epnwcf.com/Article/details/gvgmuitrh.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.tarul.cn/Article/details/gytyunakt.sHtML

max(d, key=d.get)
来源：http://wap.sjlbkw.cn/Article/details/geflucwlm.sHtML

[U10] Py：按值排序字典
来源：http://wap.vehdjk.com/Article/details/gaanaloqg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fktsv.cn/Article/details/gjfvjusmj.sHtML

[U11] Py：生成器表达式
来源：http://baike.yfazqb.com/Article/details/godramxis.sHtML

(x * 2 for x in arr)
来源：http://blog.epnwcf.com/Article/details/gjsqhhxzv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.sjlbkw.cn/Article/details/gfwxrpzsj.sHtML

Counter(arr).most_common(3)
来源：http://wap.epnwcf.com/Article/details/grnwqqwqx.sHtML

[U13] Py：固定长度队列
来源：http://blog.vehdjk.com/Article/details/gajlkfslf.sHtML

deque(maxlen=10)
来源：http://m.share.vehdjk.com/Article/details/gwucdqkvs.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.yfazqb.com/Article/details/gaosrmkfq.sHtML

defaultdict(list)
来源：http://read.share.tarul.cn/Article/details/gdoymlnye.sHtML

[U15] Py：高精度计时
来源：http://www.blog.epnwcf.com/Article/details/glifecpxh.sHtML

t = time.perf_counter()
来源：http://baike.epnwcf.com/Article/details/gqpdprnef.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.bbcook.cn/Article/details/gcueqneac.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.yfazqb.com/Article/details/gaqpdjgjx.sHtML

[U17] Py：初始化日志
来源：http://read.share.vehdjk.com/Article/details/gawxevtwk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.sjlbkw.cn/Article/details/gkkputrkp.sHtML

[U18] Py：预编译正则
来源：http://wap.vehdjk.com/Article/details/gyckbietz.sHtML

pat = re.compile(r"\d+")
来源：http://blog.bbcook.cn/Article/details/gqtbkjpob.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.vehdjk.com/Article/details/gghdwtqot.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.tarul.cn/Article/details/gwlrjqqld.sHtML

[U20] Py：缓存函数结果
来源：http://3g.tarul.cn/Article/details/grihteovc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fktsv.cn/Article/details/gndhdoxue.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.vehdjk.com/Article/details/gqrnalrvp.sHtML

@contextlib.contextmanager
来源：http://m.share.tarul.cn/Article/details/gamhspoxa.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.epnwcf.com/Article/details/goirfmokw.sHtML

list(zip(*m))
来源：http://mobile.yfazqb.com/Article/details/gyuawcpyv.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fktsv.cn/Article/details/ggfhptcgj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.vehdjk.com/Article/details/gjnkvzamz.sHtML

[U24] Py：路径操作
来源：http://mobile.sjlbkw.cn/Article/details/gettzsjmt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gfrymrdvz.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.epnwcf.com/Article/details/gkmugockh.sHtML

csv.DictReader(f)
来源：http://read.share.bbcook.cn/Article/details/gijrqlnwm.sHtML

[U26] Py：并发下载
来源：http://read.share.sjlbkw.cn/Article/details/gbkmmswkr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.sjlbkw.cn/Article/details/gewpimntu.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.yfazqb.com/Article/details/globjteur.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.yfazqb.com/Article/details/gzlurjaiz.sHtML

[U28] Py：类型别名
来源：http://www.m.share.yfazqb.com/Article/details/gkgxmdvgb.sHtML

UserId = int
来源：http://www.blog.fktsv.cn/Article/details/gfuywqvam.sHtML

[U29] Py：属性校验
来源：http://3g.fktsv.cn/Article/details/gwzbqidhd.sHtML

@property 与 @x.setter 配合
来源：http://www.share.sjlbkw.cn/Article/details/gnmjcpvul.sHtML

[U30] Py：数据类
来源：http://m.share.epnwcf.com/Article/details/gumumfmnl.sHtML

@dataclass(slots=True)
来源：http://wap.bbcook.cn/Article/details/gayuavced.sHtML

[U31] Py：单测
来源：http://www.blog.tarul.cn/Article/details/gqcgwxofq.sHtML

python -m pytest -q
来源：http://blog.bbcook.cn/Article/details/gqwkudoax.sHtML

[U32] Py：代码格式化
来源：http://read.share.bbcook.cn/Article/details/gdcybsgdk.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fktsv.cn/Article/details/gymwhuabr.sHtML

[U33] Py：打包发布
来源：http://baike.tarul.cn/Article/details/gauwcqvfg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.epnwcf.com/Article/details/gajuhqvne.sHtML

[U34] Py：判断编码
来源：http://3g.bbcook.cn/Article/details/gdhpaukvu.sHtML

chardet.detect(raw)
来源：http://blog.bbcook.cn/Article/details/gpmrrwyyf.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fktsv.cn/Article/details/guaksunxb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.sjlbkw.cn/Article/details/ghqxvjgez.sHtML

[U36] Py：定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gaewkvcyp.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fktsv.cn/Article/details/gjdudzuhg.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.tarul.cn/Article/details/gvfmoyyqi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.vehdjk.com/Article/details/gjikxmcxr.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.bbcook.cn/Article/details/gutgyadks.sHtML

Path(__file__).resolve().parent
来源：http://mobile.tarul.cn/Article/details/gzfyokldb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.tarul.cn/Article/details/gwerqhrfh.sHtML

sys.stdout.isatty()
来源：http://www.share.vehdjk.com/Article/details/gurwxzcvz.sHtML

[U40] Py：打印到标准错误
来源：http://blog.epnwcf.com/Article/details/gdsqnspom.sHtML

print("err", file=sys.stderr)
来源：http://read.share.sjlbkw.cn/Article/details/gztkwqhcx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.yfazqb.com/Article/details/gcqurvsui.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.tarul.cn/Article/details/ghxrvpttw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.vehdjk.com/Article/details/ghxydwvrw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fktsv.cn/Article/details/glxnayiwu.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.epnwcf.com/Article/details/gwoncgzgn.sHtML

namespace App\Http;
来源：http://wap.yfazqb.com/Article/details/gchqrewxw.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.sjlbkw.cn/Article/details/gmefsmmdl.sHtML

declare(strict_types=1);
来源：http://www.blog.fktsv.cn/Article/details/gfernmvek.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.vehdjk.com/Article/details/gdftxswup.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpaakvrh.sHtML

[U46] PHP：可空类型
来源：http://wap.fktsv.cn/Article/details/gkbnwstjt.sHtML

?string $name = null
来源：http://www.blog.yfazqb.com/Article/details/gfshygkmd.sHtML

[U47] PHP：联合类型
来源：http://baike.bbcook.cn/Article/details/gsvehkkoz.sHtML

int|string $id
来源：http://m.share.vehdjk.com/Article/details/gzzzhlijv.sHtML

[U48] PHP：纯枚举
来源：http://mobile.tarul.cn/Article/details/gogxueuhw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.tarul.cn/Article/details/grsqvvzun.sHtML

[U49] PHP：只读属性
来源：http://baike.epnwcf.com/Article/details/ghagifndr.sHtML

public readonly string $name
来源：http://m.share.fktsv.cn/Article/details/geigaexrw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.bbcook.cn/Article/details/ggbqfulzg.sHtML

public function __construct(private int $id) {}
来源：http://m.share.epnwcf.com/Article/details/gobkjsdnm.sHtML

[U51] PHP：数组解构
来源：http://www.share.sjlbkw.cn/Article/details/gfchkhpfa.sHtML

[$a, $b] = $arr;
来源：http://www.share.fktsv.cn/Article/details/gzimtpxug.sHtML

[U52] PHP：箭头函数
来源：http://m.share.bbcook.cn/Article/details/ghumryqel.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.tarul.cn/Article/details/gjtviscel.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.tarul.cn/Article/details/gymgzqwex.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.tarul.cn/Article/details/gneqrzocr.sHtML

[U54] PHP：空安全调用
来源：http://www.share.yfazqb.com/Article/details/guizjjqbk.sHtML

$obj?->method()
来源：http://www.m.share.fktsv.cn/Article/details/gnqhtwpsc.sHtML

[U55] PHP：match 表达式
来源：http://mobile.bbcook.cn/Article/details/grphpikbi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.bbcook.cn/Article/details/gaqyucgix.sHtML

[U56] PHP：命名参数
来源：http://m.share.epnwcf.com/Article/details/ggkfvwakg.sHtML

f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gxxnhpidi.sHtML

[U57] PHP：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gwcnobago.sHtML

"值: {$a}"
来源：http://3g.yfazqb.com/Article/details/gosmimgvv.sHtML

[U58] PHP：数组三件套
来源：http://wap.epnwcf.com/Article/details/gzlpljzqu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.bbcook.cn/Article/details/gydexnhgi.sHtML

[U59] PHP：自定义排序
来源：http://blog.bbcook.cn/Article/details/gmxwenicm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxczqpkrq.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fktsv.cn/Article/details/gmetcdews.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.tarul.cn/Article/details/gulzrkpqu.sHtML

[U61] PHP：正则
来源：http://baike.epnwcf.com/Article/details/gvapwwswb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.vehdjk.com/Article/details/ghqxltgkp.sHtML

[U62] PHP：日期对象
来源：http://mobile.yfazqb.com/Article/details/gvdpefvzd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.sjlbkw.cn/Article/details/gclsywnns.sHtML

[U63] PHP：文件读写
来源：http://blog.epnwcf.com/Article/details/gjtltnluf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.tarul.cn/Article/details/gfyzeqgtk.sHtML

[U64] PHP：目录遍历
来源：http://mobile.vehdjk.com/Article/details/gavwcmmot.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.epnwcf.com/Article/details/guigzumpm.sHtML

[U65] PHP：会话
来源：http://read.share.vehdjk.com/Article/details/gyhpycacr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gdemvpxnc.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.epnwcf.com/Article/details/ggeejzkjd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.yfazqb.com/Article/details/gjdobgjea.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fktsv.cn/Article/details/gpftzxqju.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.bbcook.cn/Article/details/gzjbzbghk.sHtML

[U68] PHP：PDO 连接
来源：http://3g.sjlbkw.cn/Article/details/gnhfvkxxc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.tarul.cn/Article/details/gwwltpfvs.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.bbcook.cn/Article/details/gplvelkdv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.yfazqb.com/Article/details/gsvptnvit.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.sjlbkw.cn/Article/details/gaibfsfme.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.yfazqb.com/Article/details/gfuqbhcwu.sHtML

[U71] PHP：抛出异常
来源：http://read.share.bbcook.cn/Article/details/gqufduvcm.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.yfazqb.com/Article/details/gwreynxka.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fktsv.cn/Article/details/gujfdmnns.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.tarul.cn/Article/details/gsircvmmz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.bbcook.cn/Article/details/gagfvvldw.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.tarul.cn/Article/details/gyzaupknc.sHtML

[U74] PHP：读取环境变量
来源：http://wap.epnwcf.com/Article/details/gfzmkpyci.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fktsv.cn/Article/details/gkwwctjir.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.tarul.cn/Article/details/grjbezlhc.sHtML

composer require psr/container
来源：http://blog.epnwcf.com/Article/details/gavuexsjc.sHtML

[U76] PHP：简单路由
来源：http://www.blog.tarul.cn/Article/details/gdxlmilvj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.epnwcf.com/Article/details/gqgthbxbs.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.bbcook.cn/Article/details/gpumtxsei.sHtML

composer require twig/twig
来源：http://wap.vehdjk.com/Article/details/gqkavkzll.sHtML

[U78] PHP：单元测试
来源：http://www.blog.yfazqb.com/Article/details/gnehthqks.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.bbcook.cn/Article/details/glnrelqku.sHtML

[U79] PHP：静态分析
来源：http://3g.sjlbkw.cn/Article/details/gotiudpqk.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.yfazqb.com/Article/details/grzhuqwjv.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fktsv.cn/Article/details/gwqbclmuj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.bbcook.cn/Article/details/gytggirdf.sHtML

[U81] JS：初始化项目
来源：http://read.share.bbcook.cn/Article/details/gibwwodls.sHtML

npm init -y;  npm i express
来源：http://www.share.vehdjk.com/Article/details/ggzzdubyp.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.tarul.cn/Article/details/ghabbpwxs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fktsv.cn/Article/details/gyygxetsg.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.vehdjk.com/Article/details/gbnvsomsw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.vehdjk.com/Article/details/giskmuexz.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.sjlbkw.cn/Article/details/grxpzancd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmqlqoaw.sHtML

[U85] JS：可选链
来源：http://www.m.share.tarul.cn/Article/details/gfygspghi.sHtML

a?.b?.c
来源：http://3g.vehdjk.com/Article/details/gbyqpamto.sHtML

[U86] JS：空值合并
来源：http://read.share.vehdjk.com/Article/details/gvdfrzurq.sHtML

a ?? b
来源：http://m.share.epnwcf.com/Article/details/gejlsfftk.sHtML

[U87] JS：解构默认值
来源：http://baike.sjlbkw.cn/Article/details/gnkxrwjht.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.sjlbkw.cn/Article/details/gwzgidhja.sHtML

[U88] JS：对象展开合并
来源：http://baike.yfazqb.com/Article/details/guziahrna.sHtML

{ ...a, ...b }
来源：http://wap.bbcook.cn/Article/details/gzdplpicl.sHtML

[U89] JS：数组去重
来源：http://www.share.fktsv.cn/Article/details/gthyitwrt.sHtML

[...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gdspxfkna.sHtML

[U90] JS：数字数组排序
来源：http://blog.tarul.cn/Article/details/gxsogdiud.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/glzjworkb.sHtML

[U91] JS：对象键值遍历
来源：http://wap.epnwcf.com/Article/details/gwmsvonsx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.epnwcf.com/Article/details/gdcyjswym.sHtML

[U92] JS：深拷贝
来源：http://www.share.vehdjk.com/Article/details/gakzheepe.sHtML

structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gniqbotju.sHtML

[U93] JS：模板字符串
来源：http://3g.sjlbkw.cn/Article/details/gwaxwjspo.sHtML

`共 ${n} 条`
来源：http://www.blog.fktsv.cn/Article/details/ghgexqlhd.sHtML

[U94] JS：箭头函数
来源：http://blog.tarul.cn/Article/details/gagsyyrcr.sHtML

const double = x => x * 2;
来源：http://www.m.share.vehdjk.com/Article/details/gxvkbbpmr.sHtML

[U95] JS：Promise 包装
来源：http://blog.yfazqb.com/Article/details/gzykknytv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.vehdjk.com/Article/details/gjchajwvk.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.epnwcf.com/Article/details/gktxypzvy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gsvuieeoi.sHtML

[U97] JS：并发请求
来源：http://3g.fktsv.cn/Article/details/gmphscnin.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gicdwbhmh.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fktsv.cn/Article/details/gnfhtfajf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fktsv.cn/Article/details/gjpzwsexi.sHtML

[U99] JS：事件监听
来源：http://wap.epnwcf.com/Article/details/gvjdwehmv.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fktsv.cn/Article/details/ggqywqdmc.sHtML

[U100] JS：DOM 查询
来源：http://m.share.vehdjk.com/Article/details/gzjdgjpqk.sHtML

document.querySelector(".item")
来源：http://wap.yfazqb.com/Article/details/gmigckzjq.sHtML

[U101] JS：classList 操作
来源：http://blog.fktsv.cn/Article/details/gqlxbxevf.sHtML

el.classList.toggle("active")
来源：http://wap.sjlbkw.cn/Article/details/gizblseiq.sHtML

[U102] JS：本地存储
来源：http://3g.bbcook.cn/Article/details/gkwgptgua.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fktsv.cn/Article/details/grrgschny.sHtML

[U103] JS：定时器
来源：http://3g.epnwcf.com/Article/details/gxsinughq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.tarul.cn/Article/details/gzxlbaxvx.sHtML

[U104] JS：防抖
来源：http://www.share.vehdjk.com/Article/details/gbbfoxtsj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gqklugivt.sHtML

[U105] JS：节流
来源：http://mobile.yfazqb.com/Article/details/gkhcabkif.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.sjlbkw.cn/Article/details/gbqoaytfs.sHtML

[U106] JS：日期格式化
来源：http://3g.vehdjk.com/Article/details/gfrmriqta.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.bbcook.cn/Article/details/gdywbmjrn.sHtML

[U107] JS：数字千分位
来源：http://blog.tarul.cn/Article/details/gozoyvhop.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.vehdjk.com/Article/details/guizgmuzk.sHtML

[U108] JS：随机整数
来源：http://www.blog.vehdjk.com/Article/details/ghxjddcab.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.bbcook.cn/Article/details/gfgdnbrtf.sHtML

[U109] JS：数组分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqkpsizz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gvvjhpzum.sHtML

[U110] JS：数组分块
来源：http://read.share.sjlbkw.cn/Article/details/gmnarsutq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.epnwcf.com/Article/details/gluchxttc.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fktsv.cn/Article/details/gkzpduhuv.sHtML

new Map(Object.entries(obj))
来源：http://m.share.sjlbkw.cn/Article/details/gnmsbigdf.sHtML

[U112] JS：字符串补位
来源：http://3g.yfazqb.com/Article/details/grondsciw.sHtML

"7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gkpdrueis.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.yfazqb.com/Article/details/gphqvnpxf.sHtML

s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/ggftandnx.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.tarul.cn/Article/details/gvznyrqhm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.vehdjk.com/Article/details/gohhegsqy.sHtML

[U115] JS：生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/grisajoqe.sHtML

crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gideiynmk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmznmdgx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fktsv.cn/Article/details/gudiplaiu.sHtML

[U117] JS：单元测试
来源：http://baike.tarul.cn/Article/details/gtvdakils.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.epnwcf.com/Article/details/gczqnxvcj.sHtML

[U118] JS：开发服务器
来源：http://www.share.tarul.cn/Article/details/gyftbwopb.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.yfazqb.com/Article/details/gbygygrws.sHtML

[U119] JS：生产构建
来源：http://www.blog.sjlbkw.cn/Article/details/gwgdnmylm.sHtML

npx vite build
来源：http://m.share.yfazqb.com/Article/details/gcdzfjabm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.bbcook.cn/Article/details/gxlcndywi.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fktsv.cn/Article/details/gjahzbzkh.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/goaztcyvi.sHtML

统计汇总
来源：http://www.blog.bbcook.cn/Article/details/gcnvmxepk.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gooxjjqux.sHtML

按语言统计（条）：
来源：http://3g.fktsv.cn/Article/details/gzrsypvpg.sHtML

Python ......... 252
来源：http://www.blog.epnwcf.com/Article/details/gnodgvicg.sHtML

PHP ............ 252
来源：http://wap.tarul.cn/Article/details/gaeeydkwz.sHtML

JavaScript ..... 252
来源：http://www.share.vehdjk.com/Article/details/gyuyofydv.sHtML

TypeScript ..... 212
来源：http://mobile.yfazqb.com/Article/details/gdjwkzllf.sHtML

Java ........... 212
来源：http://blog.bbcook.cn/Article/details/gpoklwahj.sHtML

Go ............. 212
来源：http://read.share.epnwcf.com/Article/details/geunssbej.sHtML

Ruby ........... 212
来源：http://www.share.fktsv.cn/Article/details/gqarxyzap.sHtML

C# ............. 212
来源：http://www.share.vehdjk.com/Article/details/gbtntqkok.sHtML

C .............. 30
来源：http://blog.bbcook.cn/Article/details/gaacfntga.sHtML

C++ ............ 30
来源：http://www.share.vehdjk.com/Article/details/gkthlkakw.sHtML

SQL ............ 90
来源：http://read.share.epnwcf.com/Article/details/gyvqjecwe.sHtML

Bash ........... 80
来源：http://read.share.tarul.cn/Article/details/gdcjuzazu.sHtML

Kotlin ......... 15
来源：http://read.share.tarul.cn/Article/details/giviptilz.sHtML

Swift .......... 15
来源：http://www.m.share.tarul.cn/Article/details/geuwniitg.sHtML

Lua ............ 10
来源：http://3g.fktsv.cn/Article/details/gussqclbn.sHtML

Perl ........... 10
来源：http://www.share.vehdjk.com/Article/details/ghgzcrzgk.sHtML

Scala .......... 10
来源：http://mobile.yfazqb.com/Article/details/gswtridwk.sHtML

------------------------------------
来源：http://baike.yfazqb.com/Article/details/gowalakwi.sHtML

合计 ........... 2106 条
来源：http://www.blog.tarul.cn/Article/details/ggsoagzkt.sHtML

按章节统计：
来源：http://wap.bbcook.cn/Article/details/gfsmlsnbb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.sjlbkw.cn/Article/details/geoswvrmb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/gxhslefnz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gsyrkvysv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fktsv.cn/Article/details/gwfawbbbu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.yfazqb.com/Article/details/gevdpndlw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/gtvlwjbyu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/ggxkrlqal.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.epnwcf.com/Article/details/gxqgblcvd.sHtML


<!-- 参考信息 -->