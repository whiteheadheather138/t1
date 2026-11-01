代发 wailian999

[T49] Perl：函数
来源：http://m.share.tarul.cn/Article/details/gcsrbiltz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/glxtlpsya.sHtML

[T50] Perl：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gpiepasuh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.tarul.cn/Article/details/gwkugmhrw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fktsv.cn/Article/details/grojoktqw.sHtML

[T51] Scala：Hello World
来源：http://read.share.fktsv.cn/Article/details/gtyfrihwq.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/gfhvocvvg.sHtML

[T52] Scala：变量
来源：http://wap.sjlbkw.cn/Article/details/gxfovghtv.sHtML

val a = 1;  var b = 2
来源：http://m.share.epnwcf.com/Article/details/gfsqstizz.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gxgmlagnx.sHtML

s"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gfcmuiaej.sHtML

[T54] Scala：集合映射
来源：http://baike.vehdjk.com/Article/details/gopnwtvtm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.epnwcf.com/Article/details/gbqbcjxmk.sHtML

[T55] Scala：集合过滤
来源：http://baike.vehdjk.com/Article/details/gkokpwsua.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.tarul.cn/Article/details/gtvsykspt.sHtML

[T56] Scala：样例类
来源：http://m.share.sjlbkw.cn/Article/details/gtotsmraq.sHtML

case class User(name: String, age: Int)
来源：http://mobile.yfazqb.com/Article/details/gktbjfzpq.sHtML

[T57] Scala：模式匹配
来源：http://read.share.bbcook.cn/Article/details/gybaolpkh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.bbcook.cn/Article/details/gbwxazhlm.sHtML

[T58] Scala：函数定义
来源：http://wap.bbcook.cn/Article/details/gjixqlmat.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.epnwcf.com/Article/details/grvopoccu.sHtML

[T59] Scala：循环
来源：http://wap.tarul.cn/Article/details/getbnmniy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/geaprbluz.sHtML

[T60] Scala：折叠
来源：http://baike.bbcook.cn/Article/details/glocxpicm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.sjlbkw.cn/Article/details/guslsyuau.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbmraqgwr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.sjlbkw.cn/Article/details/gqhcedmdv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gmzgiyeps.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.tarul.cn/Article/details/gmijdnwmo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.sjlbkw.cn/Article/details/gflwrxyeu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.yfazqb.com/Article/details/gsrxriggk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.tarul.cn/Article/details/gvwrchfbh.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.vehdjk.com/Article/details/gxhxwvevg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.tarul.cn/Article/details/gzqnxobka.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/gtkjgtzcm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.vehdjk.com/Article/details/gbfdqoltz.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.sjlbkw.cn/Article/details/gsdeuuwnm.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gqhvxsbuc.sHtML

[U06] Py：合并两个字典
来源：http://www.share.yfazqb.com/Article/details/gwflqqbns.sHtML

{**a, **b}
来源：http://www.blog.fktsv.cn/Article/details/gfhmgjsvz.sHtML

[U07] Py：反转字典键值
来源：http://read.share.vehdjk.com/Article/details/gzsxavpwb.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.vehdjk.com/Article/details/gqfybojnz.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fktsv.cn/Article/details/gtcbyfqde.sHtML

[y for x in nested for y in x]
来源：http://www.share.tarul.cn/Article/details/gvwgvyuzh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.vehdjk.com/Article/details/gxmtriyms.sHtML

max(d, key=d.get)
来源：http://read.share.yfazqb.com/Article/details/gyswjhazf.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.tarul.cn/Article/details/gpuryoupe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fktsv.cn/Article/details/gibujemfq.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fktsv.cn/Article/details/gohwbgjzu.sHtML

(x * 2 for x in arr)
来源：http://www.blog.yfazqb.com/Article/details/gctodyapw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fktsv.cn/Article/details/gucvfimub.sHtML

Counter(arr).most_common(3)
来源：http://wap.bbcook.cn/Article/details/gwrqmcqwk.sHtML

[U13] Py：固定长度队列
来源：http://blog.yfazqb.com/Article/details/gfarkeyzc.sHtML

deque(maxlen=10)
来源：http://read.share.fktsv.cn/Article/details/gkrxfcssg.sHtML

[U14] Py：分组收集到列表
来源：http://baike.tarul.cn/Article/details/gkfoaozyd.sHtML

defaultdict(list)
来源：http://wap.vehdjk.com/Article/details/gphckdkfo.sHtML

[U15] Py：高精度计时
来源：http://wap.epnwcf.com/Article/details/grbtjxase.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/gxhuxnhjo.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpqpzkfo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.bbcook.cn/Article/details/gvkinhrjn.sHtML

[U17] Py：初始化日志
来源：http://blog.fktsv.cn/Article/details/grferqjzi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.tarul.cn/Article/details/gznndupbf.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.epnwcf.com/Article/details/gwppzylwg.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.vehdjk.com/Article/details/gpzvtsogf.sHtML

[U19] Py：正则替换带回调
来源：http://wap.yfazqb.com/Article/details/gjiewtlwl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.epnwcf.com/Article/details/gzncejfba.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/gwcocdkru.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.tarul.cn/Article/details/gybmbklgo.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.yfazqb.com/Article/details/gsfoazfca.sHtML

@contextlib.contextmanager
来源：http://read.share.sjlbkw.cn/Article/details/gzonskzqy.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.tarul.cn/Article/details/gnjzdxpsc.sHtML

list(zip(*m))
来源：http://mobile.bbcook.cn/Article/details/gqtiyncge.sHtML

[U23] Py：分块读取大文件
来源：http://wap.yfazqb.com/Article/details/gfccbvahz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fktsv.cn/Article/details/gwemzfalz.sHtML

[U24] Py：路径操作
来源：http://read.share.bbcook.cn/Article/details/gosxdfjmo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/givjcidad.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.sjlbkw.cn/Article/details/gxblvloke.sHtML

csv.DictReader(f)
来源：http://www.share.bbcook.cn/Article/details/gtpkdhhyc.sHtML

[U26] Py：并发下载
来源：http://baike.fktsv.cn/Article/details/gpjwlfmov.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.epnwcf.com/Article/details/gtzoctkhw.sHtML

[U27] Py：异步 HTTP
来源：http://blog.sjlbkw.cn/Article/details/gooyqzouo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.epnwcf.com/Article/details/gynacgquv.sHtML

[U28] Py：类型别名
来源：http://m.share.yfazqb.com/Article/details/gqahkioyn.sHtML

UserId = int
来源：http://www.share.tarul.cn/Article/details/gzgyjjdkv.sHtML

[U29] Py：属性校验
来源：http://m.share.fktsv.cn/Article/details/gzkqmzpii.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fktsv.cn/Article/details/gcovzhsbn.sHtML

[U30] Py：数据类
来源：http://m.share.fktsv.cn/Article/details/gzhpiwdob.sHtML

@dataclass(slots=True)
来源：http://read.share.vehdjk.com/Article/details/gzxloaijq.sHtML

[U31] Py：单测
来源：http://read.share.tarul.cn/Article/details/gklgcuqsc.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/girtqerfc.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.vehdjk.com/Article/details/gehnmfyoi.sHtML

ruff format . && ruff check --fix .
来源：http://wap.epnwcf.com/Article/details/gpdgxzacl.sHtML

[U33] Py：打包发布
来源：http://3g.bbcook.cn/Article/details/gfajsfiid.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.yfazqb.com/Article/details/guvadewvn.sHtML

[U34] Py：判断编码
来源：http://wap.tarul.cn/Article/details/goswtcqmx.sHtML

chardet.detect(raw)
来源：http://mobile.vehdjk.com/Article/details/gvtkroxju.sHtML

[U35] Py：发送邮件
来源：http://m.share.vehdjk.com/Article/details/gnbyqsofo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.epnwcf.com/Article/details/gazabaumr.sHtML

[U36] Py：定时任务
来源：http://mobile.fktsv.cn/Article/details/glrffjafe.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.bbcook.cn/Article/details/gcryvxtwb.sHtML

[U37] Py：读写 Excel
来源：http://wap.bbcook.cn/Article/details/gfyhqimfi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.bbcook.cn/Article/details/gjjwfjnbz.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.bbcook.cn/Article/details/gykdkfuah.sHtML

Path(__file__).resolve().parent
来源：http://3g.tarul.cn/Article/details/gshfpyrjo.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.bbcook.cn/Article/details/gfbuokmis.sHtML

sys.stdout.isatty()
来源：http://mobile.fktsv.cn/Article/details/gxkmyizwu.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.bbcook.cn/Article/details/gdylorcoy.sHtML

print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/giijqtlew.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjvzspoj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.tarul.cn/Article/details/gdlzqdmou.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fktsv.cn/Article/details/gwmuszsqt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.epnwcf.com/Article/details/gwutyaeiz.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.vehdjk.com/Article/details/gjxywglhq.sHtML

namespace App\Http;
来源：http://blog.sjlbkw.cn/Article/details/gwjfbvtge.sHtML

[U44] PHP：开启严格类型
来源：http://baike.yfazqb.com/Article/details/gwrahflkk.sHtML

declare(strict_types=1);
来源：http://www.blog.sjlbkw.cn/Article/details/gllarrpve.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.bbcook.cn/Article/details/gyjlrpzwg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gcakkliqw.sHtML

[U46] PHP：可空类型
来源：http://m.share.yfazqb.com/Article/details/gjxbocubc.sHtML

?string $name = null
来源：http://www.m.share.yfazqb.com/Article/details/gxqmzmigg.sHtML

[U47] PHP：联合类型
来源：http://read.share.yfazqb.com/Article/details/gytcpixic.sHtML

int|string $id
来源：http://m.share.bbcook.cn/Article/details/gaprefnay.sHtML

[U48] PHP：纯枚举
来源：http://blog.vehdjk.com/Article/details/grxrsmjpf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fktsv.cn/Article/details/gefeeijhh.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fktsv.cn/Article/details/gajeuidwc.sHtML

public readonly string $name
来源：http://mobile.yfazqb.com/Article/details/gurykvcze.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.vehdjk.com/Article/details/giecktwze.sHtML

public function __construct(private int $id) {}
来源：http://wap.yfazqb.com/Article/details/gmiwqzryc.sHtML

[U51] PHP：数组解构
来源：http://3g.fktsv.cn/Article/details/gkhgkepoz.sHtML

[$a, $b] = $arr;
来源：http://read.share.epnwcf.com/Article/details/gtthcrsmi.sHtML

[U52] PHP：箭头函数
来源：http://3g.epnwcf.com/Article/details/gebqndraa.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.bbcook.cn/Article/details/gydyqaktn.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fktsv.cn/Article/details/gauyqdlxo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fktsv.cn/Article/details/giphubejz.sHtML

[U54] PHP：空安全调用
来源：http://www.share.vehdjk.com/Article/details/giqsspdbh.sHtML

$obj?->method()
来源：http://www.m.share.bbcook.cn/Article/details/gsvmklfqb.sHtML

[U55] PHP：match 表达式
来源：http://www.share.yfazqb.com/Article/details/gniwrvbao.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fktsv.cn/Article/details/gdllbakpc.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gqzpwfhml.sHtML

f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gskdrhhsp.sHtML

[U57] PHP：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gyrgawdms.sHtML

"值: {$a}"
来源：http://baike.fktsv.cn/Article/details/gbggxusih.sHtML

[U58] PHP：数组三件套
来源：http://www.share.bbcook.cn/Article/details/garscmpfh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gatehqtzm.sHtML

[U59] PHP：自定义排序
来源：http://baike.tarul.cn/Article/details/gxelxoeix.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gcphupdxv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.bbcook.cn/Article/details/gkrufevyo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.tarul.cn/Article/details/gvumlhwxo.sHtML

[U61] PHP：正则
来源：http://blog.sjlbkw.cn/Article/details/giyrkamwg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gexbutdkt.sHtML

[U62] PHP：日期对象
来源：http://read.share.sjlbkw.cn/Article/details/gmyerfaga.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.yfazqb.com/Article/details/gahgdwhvv.sHtML

[U63] PHP：文件读写
来源：http://read.share.yfazqb.com/Article/details/gqolcenpc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.tarul.cn/Article/details/guhfublsi.sHtML

[U64] PHP：目录遍历
来源：http://www.share.bbcook.cn/Article/details/ggdhnrwxt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.vehdjk.com/Article/details/grytjxzyp.sHtML

[U65] PHP：会话
来源：http://www.m.share.bbcook.cn/Article/details/gjukrbfkp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gjicyjvve.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.epnwcf.com/Article/details/gepfvclqm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.tarul.cn/Article/details/gxgcjidja.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.tarul.cn/Article/details/gjwawaphf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.sjlbkw.cn/Article/details/gelmnvpkc.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fktsv.cn/Article/details/gxxjnjzvp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fktsv.cn/Article/details/guaugkxdd.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.yfazqb.com/Article/details/gfycskktx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.epnwcf.com/Article/details/gmnctkvqy.sHtML

[U70] PHP：PDO 事务
来源：http://blog.epnwcf.com/Article/details/gksfohskn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.bbcook.cn/Article/details/gmdrjebqm.sHtML

[U71] PHP：抛出异常
来源：http://blog.epnwcf.com/Article/details/gnfykmsid.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.tarul.cn/Article/details/gqtwdddzi.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.tarul.cn/Article/details/ggstkqoef.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.tarul.cn/Article/details/gxcpfhohq.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.tarul.cn/Article/details/gzdqyxine.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.bbcook.cn/Article/details/gfwwafqiz.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.epnwcf.com/Article/details/gqnpggtjc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.epnwcf.com/Article/details/gdwnbclah.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.vehdjk.com/Article/details/ghavecybg.sHtML

composer require psr/container
来源：http://wap.bbcook.cn/Article/details/gfifrbess.sHtML

[U76] PHP：简单路由
来源：http://www.share.epnwcf.com/Article/details/grhgngfps.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.vehdjk.com/Article/details/gaknsnydr.sHtML

[U77] PHP：模板渲染
来源：http://wap.epnwcf.com/Article/details/gdmmtfvhf.sHtML

composer require twig/twig
来源：http://3g.tarul.cn/Article/details/gxjuajpau.sHtML

[U78] PHP：单元测试
来源：http://3g.yfazqb.com/Article/details/gokrithqm.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.tarul.cn/Article/details/gnkdmjktm.sHtML

[U79] PHP：静态分析
来源：http://www.share.bbcook.cn/Article/details/gwznspnix.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.epnwcf.com/Article/details/goxkyydmq.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.tarul.cn/Article/details/gwjkyvsdv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.bbcook.cn/Article/details/gtjppttsb.sHtML

[U81] JS：初始化项目
来源：http://m.share.sjlbkw.cn/Article/details/grffvbxtb.sHtML

npm init -y;  npm i express
来源：http://3g.yfazqb.com/Article/details/gjugavcul.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.tarul.cn/Article/details/gbctcxtza.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.bbcook.cn/Article/details/gekeqhqgu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.epnwcf.com/Article/details/gsrfycjjz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.vehdjk.com/Article/details/gcvzbfrnm.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.tarul.cn/Article/details/gsgsxonrm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fktsv.cn/Article/details/gcttwmrwy.sHtML

[U85] JS：可选链
来源：http://3g.fktsv.cn/Article/details/gwqowuauf.sHtML

a?.b?.c
来源：http://www.blog.sjlbkw.cn/Article/details/gxcdoxnzc.sHtML

[U86] JS：空值合并
来源：http://baike.epnwcf.com/Article/details/gxjafrxmd.sHtML

a ?? b
来源：http://baike.epnwcf.com/Article/details/gckdypzjj.sHtML

[U87] JS：解构默认值
来源：http://blog.sjlbkw.cn/Article/details/gxzqhhqjo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.yfazqb.com/Article/details/gsuuzwqes.sHtML

[U88] JS：对象展开合并
来源：http://blog.tarul.cn/Article/details/gmnksufre.sHtML

{ ...a, ...b }
来源：http://www.share.tarul.cn/Article/details/gekznitgd.sHtML

[U89] JS：数组去重
来源：http://www.blog.vehdjk.com/Article/details/gyvayjcgs.sHtML

[...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/glplpbeux.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.bbcook.cn/Article/details/gmxtydanf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gypljnygx.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.epnwcf.com/Article/details/ggxfpqiia.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.bbcook.cn/Article/details/ghusxpijs.sHtML

[U92] JS：深拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gvsmklwro.sHtML

structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gouynlisc.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.epnwcf.com/Article/details/ghvhvovli.sHtML

`共 ${n} 条`
来源：http://www.m.share.tarul.cn/Article/details/gsqogvbkv.sHtML

[U94] JS：箭头函数
来源：http://blog.bbcook.cn/Article/details/ggugwools.sHtML

const double = x => x * 2;
来源：http://baike.epnwcf.com/Article/details/gxusoltjq.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.bbcook.cn/Article/details/gmthiasrg.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.sjlbkw.cn/Article/details/gdtnrxvkb.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fktsv.cn/Article/details/grluvdsep.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gchpnvtbj.sHtML

[U97] JS：并发请求
来源：http://m.share.vehdjk.com/Article/details/gckcorfgz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gyubdyqho.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.vehdjk.com/Article/details/gyoqbhtdf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.sjlbkw.cn/Article/details/geqpwjmnk.sHtML

[U99] JS：事件监听
来源：http://3g.vehdjk.com/Article/details/gvryuruzj.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.epnwcf.com/Article/details/gmwvlrqch.sHtML

[U100] JS：DOM 查询
来源：http://baike.bbcook.cn/Article/details/gtpvwfmsh.sHtML

document.querySelector(".item")
来源：http://blog.tarul.cn/Article/details/gugpvstxh.sHtML

[U101] JS：classList 操作
来源：http://3g.yfazqb.com/Article/details/ggzaletel.sHtML

el.classList.toggle("active")
来源：http://www.share.fktsv.cn/Article/details/gpioruurs.sHtML

[U102] JS：本地存储
来源：http://www.share.sjlbkw.cn/Article/details/gouxlgtef.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fktsv.cn/Article/details/gekoqvevh.sHtML

[U103] JS：定时器
来源：http://www.m.share.yfazqb.com/Article/details/gubtcdksu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.vehdjk.com/Article/details/gexpnomhm.sHtML

[U104] JS：防抖
来源：http://baike.tarul.cn/Article/details/gfiuiexmp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gugztokyc.sHtML

[U105] JS：节流
来源：http://baike.bbcook.cn/Article/details/gnmltwmdd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.tarul.cn/Article/details/gmbfltvdx.sHtML

[U106] JS：日期格式化
来源：http://blog.yfazqb.com/Article/details/ghbxmblzc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.bbcook.cn/Article/details/gmftyrbyb.sHtML

[U107] JS：数字千分位
来源：http://www.share.fktsv.cn/Article/details/gspccbbxf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gduhwujlo.sHtML

[U108] JS：随机整数
来源：http://baike.sjlbkw.cn/Article/details/gnyihgcgf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.vehdjk.com/Article/details/gfefxkujy.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fktsv.cn/Article/details/gmbzypotj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gtgbzfmoo.sHtML

[U110] JS：数组分块
来源：http://www.blog.bbcook.cn/Article/details/goesqasfn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.tarul.cn/Article/details/golfrsimd.sHtML

[U111] JS：对象转 Map
来源：http://baike.sjlbkw.cn/Article/details/gqeiposqn.sHtML

new Map(Object.entries(obj))
来源：http://blog.sjlbkw.cn/Article/details/giydbhtef.sHtML

[U112] JS：字符串补位
来源：http://www.share.epnwcf.com/Article/details/gelgbmohy.sHtML

"7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gedezgotq.sHtML

[U113] JS：正则替换全部
来源：http://m.share.tarul.cn/Article/details/gcownygst.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gmotmffci.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fktsv.cn/Article/details/gmnkeoaha.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.bbcook.cn/Article/details/gazbhalny.sHtML

[U115] JS：生成 UUID
来源：http://mobile.sjlbkw.cn/Article/details/gsvdnveju.sHtML

crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/galisrldu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fktsv.cn/Article/details/gwwoxchyi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.yfazqb.com/Article/details/gslcfuuzf.sHtML

[U117] JS：单元测试
来源：http://blog.bbcook.cn/Article/details/gdxcnwvkn.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fktsv.cn/Article/details/gwjcawnjn.sHtML

[U118] JS：开发服务器
来源：http://blog.epnwcf.com/Article/details/ghupujfyl.sHtML

npm i -D vite;  npx vite
来源：http://baike.bbcook.cn/Article/details/guuusxrbb.sHtML

[U119] JS：生产构建
来源：http://www.blog.sjlbkw.cn/Article/details/godvlmfzs.sHtML

npx vite build
来源：http://www.blog.bbcook.cn/Article/details/gjeenkwzv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.yfazqb.com/Article/details/ghbfubopj.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.yfazqb.com/Article/details/gaptjybcw.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzcdzbtwq.sHtML

统计汇总
来源：http://blog.tarul.cn/Article/details/gtrdqyryz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gnbmvbfar.sHtML

按语言统计（条）：
来源：http://baike.epnwcf.com/Article/details/gnshwlcjg.sHtML

Python ......... 252
来源：http://3g.yfazqb.com/Article/details/gbvpfnusw.sHtML

PHP ............ 252
来源：http://3g.bbcook.cn/Article/details/gbmacrufg.sHtML

JavaScript ..... 252
来源：http://wap.epnwcf.com/Article/details/gaqbwdsiy.sHtML

TypeScript ..... 212
来源：http://www.share.yfazqb.com/Article/details/gewudkcef.sHtML

Java ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gnamplpsi.sHtML

Go ............. 212
来源：http://www.m.share.fktsv.cn/Article/details/gkkinmzkg.sHtML

Ruby ........... 212
来源：http://blog.sjlbkw.cn/Article/details/goukzgxvj.sHtML

C# ............. 212
来源：http://www.blog.epnwcf.com/Article/details/gcpmvnkyp.sHtML

C .............. 30
来源：http://baike.sjlbkw.cn/Article/details/gioizmrvl.sHtML

C++ ............ 30
来源：http://3g.epnwcf.com/Article/details/gdfgcnbxm.sHtML

SQL ............ 90
来源：http://baike.vehdjk.com/Article/details/gsnsowqdo.sHtML

Bash ........... 80
来源：http://m.share.fktsv.cn/Article/details/gvpfsqdhr.sHtML

Kotlin ......... 15
来源：http://m.share.vehdjk.com/Article/details/gmhnxrnei.sHtML

Swift .......... 15
来源：http://baike.epnwcf.com/Article/details/gdojfuptb.sHtML

Lua ............ 10
来源：http://3g.epnwcf.com/Article/details/gorxgxzdx.sHtML

Perl ........... 10
来源：http://blog.sjlbkw.cn/Article/details/grbhzrhgf.sHtML

Scala .......... 10
来源：http://3g.epnwcf.com/Article/details/govrpdnmk.sHtML

------------------------------------
来源：http://blog.yfazqb.com/Article/details/gkvuctzhx.sHtML

合计 ........... 2106 条
来源：http://blog.sjlbkw.cn/Article/details/gycaknwbb.sHtML

按章节统计：
来源：http://mobile.sjlbkw.cn/Article/details/gbfdnxpah.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.bbcook.cn/Article/details/glhokbmkp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gnxgtmtur.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.epnwcf.com/Article/details/gtyxqakny.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fktsv.cn/Article/details/gtwllpdho.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.tarul.cn/Article/details/gfzoqnqmn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.epnwcf.com/Article/details/gwscmzzap.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/ggfiktasu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.yfazqb.com/Article/details/gixbivnif.sHtML


<!-- 参考信息 -->