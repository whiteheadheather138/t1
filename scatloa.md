代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://baike.sjlbkw.cn/Article/details/gsqgnwzhr.sHtML

[T51] Scala：Hello World
来源：http://blog.vehdjk.com/Article/details/ggxgegdll.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gztjubcvv.sHtML

[T52] Scala：变量
来源：http://www.blog.fktsv.cn/Article/details/gokgroqkt.sHtML

val a = 1;  var b = 2
来源：http://mobile.epnwcf.com/Article/details/gidtgokmv.sHtML

[T53] Scala：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gspsanefy.sHtML

s"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gnrksjmyz.sHtML

[T54] Scala：集合映射
来源：http://wap.vehdjk.com/Article/details/ghovcuuov.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.bbcook.cn/Article/details/gnhxuqkvx.sHtML

[T55] Scala：集合过滤
来源：http://baike.fktsv.cn/Article/details/gcggjfqsb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.yfazqb.com/Article/details/gnlszbvcr.sHtML

[T56] Scala：样例类
来源：http://baike.bbcook.cn/Article/details/gtwxponik.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gkircpbyi.sHtML

[T57] Scala：模式匹配
来源：http://m.share.tarul.cn/Article/details/ggohoophz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.bbcook.cn/Article/details/gikzdhwwk.sHtML

[T58] Scala：函数定义
来源：http://wap.fktsv.cn/Article/details/gsmaiiwmz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gpywvysuk.sHtML

[T59] Scala：循环
来源：http://blog.epnwcf.com/Article/details/gixcatrcg.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.yfazqb.com/Article/details/gvbpyxpxy.sHtML

[T60] Scala：折叠
来源：http://mobile.tarul.cn/Article/details/gcajjhscs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.epnwcf.com/Article/details/ghuiaiaqd.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glmolcbvr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fktsv.cn/Article/details/gopoonzoo.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gjahigdsv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.tarul.cn/Article/details/graymaxam.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.vehdjk.com/Article/details/grqyyrmur.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.vehdjk.com/Article/details/gyypbledy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/gqouaziga.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.epnwcf.com/Article/details/grtimilga.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fktsv.cn/Article/details/genbmdzgz.sHtML

[U04] Py：变量调试打印
来源：http://www.share.tarul.cn/Article/details/gbocsoooa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.yfazqb.com/Article/details/gwkjpnfxz.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkxyblwf.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/gdmtuesyq.sHtML

[U06] Py：合并两个字典
来源：http://m.share.tarul.cn/Article/details/gqgkrdgjo.sHtML

{**a, **b}
来源：http://wap.yfazqb.com/Article/details/gfrwfxvyd.sHtML

[U07] Py：反转字典键值
来源：http://read.share.vehdjk.com/Article/details/gfcncjwju.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.sjlbkw.cn/Article/details/gsdmrptcu.sHtML

[U08] Py：展平二维列表
来源：http://www.share.yfazqb.com/Article/details/gwbdrxmtg.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.yfazqb.com/Article/details/gqpdykoec.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.epnwcf.com/Article/details/gywuidibd.sHtML

max(d, key=d.get)
来源：http://www.blog.fktsv.cn/Article/details/gzlsnkhfy.sHtML

[U10] Py：按值排序字典
来源：http://www.share.sjlbkw.cn/Article/details/gybxfytrd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.yfazqb.com/Article/details/gechelevh.sHtML

[U11] Py：生成器表达式
来源：http://baike.epnwcf.com/Article/details/gmactsuni.sHtML

(x * 2 for x in arr)
来源：http://3g.yfazqb.com/Article/details/gsxuygoij.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.vehdjk.com/Article/details/gkqjwcoug.sHtML

Counter(arr).most_common(3)
来源：http://www.share.epnwcf.com/Article/details/gzsmrvoua.sHtML

[U13] Py：固定长度队列
来源：http://3g.epnwcf.com/Article/details/gcjtjypuw.sHtML

deque(maxlen=10)
来源：http://www.share.sjlbkw.cn/Article/details/gqdnzyysr.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.yfazqb.com/Article/details/gzesfhpde.sHtML

defaultdict(list)
来源：http://www.m.share.yfazqb.com/Article/details/glhgdpffo.sHtML

[U15] Py：高精度计时
来源：http://baike.yfazqb.com/Article/details/gpavkmqdb.sHtML

t = time.perf_counter()
来源：http://blog.fktsv.cn/Article/details/gtnvdvrey.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fktsv.cn/Article/details/gnlfqgdbh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.sjlbkw.cn/Article/details/giezzhapo.sHtML

[U17] Py：初始化日志
来源：http://mobile.yfazqb.com/Article/details/gdorjjbug.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.sjlbkw.cn/Article/details/gutjdsfbe.sHtML

[U18] Py：预编译正则
来源：http://www.blog.yfazqb.com/Article/details/gjjcnfwem.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.yfazqb.com/Article/details/gofcoszho.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.epnwcf.com/Article/details/gcwtwzonp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.bbcook.cn/Article/details/gmlpkdtyq.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fktsv.cn/Article/details/geskqgshx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.bbcook.cn/Article/details/girjubcnr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.sjlbkw.cn/Article/details/gbilbmogo.sHtML

@contextlib.contextmanager
来源：http://www.m.share.bbcook.cn/Article/details/ggnqxmarh.sHtML

[U22] Py：矩阵转置
来源：http://blog.sjlbkw.cn/Article/details/giiewiwsz.sHtML

list(zip(*m))
来源：http://www.share.vehdjk.com/Article/details/gjdrfnwux.sHtML

[U23] Py：分块读取大文件
来源：http://baike.sjlbkw.cn/Article/details/gawzifvvo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.yfazqb.com/Article/details/goxaaqhkj.sHtML

[U24] Py：路径操作
来源：http://www.m.share.yfazqb.com/Article/details/gvtdwiljj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/geesbpzaj.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.bbcook.cn/Article/details/giiaagjmq.sHtML

csv.DictReader(f)
来源：http://m.share.sjlbkw.cn/Article/details/gqpfbxjsz.sHtML

[U26] Py：并发下载
来源：http://www.m.share.yfazqb.com/Article/details/gybtomcow.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.tarul.cn/Article/details/gmqrzoctv.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.vehdjk.com/Article/details/grtnklmvk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fktsv.cn/Article/details/ghyljmjfx.sHtML

[U28] Py：类型别名
来源：http://www.blog.fktsv.cn/Article/details/gkorwycle.sHtML

UserId = int
来源：http://wap.fktsv.cn/Article/details/gwgnwhbxg.sHtML

[U29] Py：属性校验
来源：http://m.share.bbcook.cn/Article/details/gwpxsekbu.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fktsv.cn/Article/details/gzfpqyxmv.sHtML

[U30] Py：数据类
来源：http://wap.vehdjk.com/Article/details/gmuodclyw.sHtML

@dataclass(slots=True)
来源：http://mobile.fktsv.cn/Article/details/gtgawvffv.sHtML

[U31] Py：单测
来源：http://m.share.bbcook.cn/Article/details/gxynfkqla.sHtML

python -m pytest -q
来源：http://mobile.yfazqb.com/Article/details/gcwjogyyn.sHtML

[U32] Py：代码格式化
来源：http://wap.yfazqb.com/Article/details/gfyztltix.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.tarul.cn/Article/details/ghqqldavm.sHtML

[U33] Py：打包发布
来源：http://read.share.bbcook.cn/Article/details/gkfvvlwei.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fktsv.cn/Article/details/gvwkigblh.sHtML

[U34] Py：判断编码
来源：http://www.m.share.vehdjk.com/Article/details/gkdlylzfi.sHtML

chardet.detect(raw)
来源：http://read.share.epnwcf.com/Article/details/gfndmybnh.sHtML

[U35] Py：发送邮件
来源：http://wap.bbcook.cn/Article/details/gshnndqcm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.tarul.cn/Article/details/gudjnsoqq.sHtML

[U36] Py：定时任务
来源：http://read.share.fktsv.cn/Article/details/gsduiquyh.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.epnwcf.com/Article/details/gnsgmbznh.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.sjlbkw.cn/Article/details/gqmtefgcj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.bbcook.cn/Article/details/gykwdktwc.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fktsv.cn/Article/details/gbxsssyjv.sHtML

Path(__file__).resolve().parent
来源：http://m.share.yfazqb.com/Article/details/gclqtztrd.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gytcpudtj.sHtML

sys.stdout.isatty()
来源：http://mobile.epnwcf.com/Article/details/gnxumoadq.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.vehdjk.com/Article/details/gcimaxcgv.sHtML

print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gvhgaqezb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.tarul.cn/Article/details/gngvhglfg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.vehdjk.com/Article/details/gqhsegwmd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.vehdjk.com/Article/details/guryavwwq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.tarul.cn/Article/details/gjrnhsugw.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.sjlbkw.cn/Article/details/gxjvdtiig.sHtML

namespace App\Http;
来源：http://www.blog.vehdjk.com/Article/details/ggcrxrapt.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fktsv.cn/Article/details/gshzyujub.sHtML

declare(strict_types=1);
来源：http://blog.bbcook.cn/Article/details/gisgyrzin.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.yfazqb.com/Article/details/gycatjwjm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gkyinmsbr.sHtML

[U46] PHP：可空类型
来源：http://read.share.tarul.cn/Article/details/ghhdasrqc.sHtML

?string $name = null
来源：http://mobile.vehdjk.com/Article/details/gjbnfxvwm.sHtML

[U47] PHP：联合类型
来源：http://wap.tarul.cn/Article/details/gyjoikgcg.sHtML

int|string $id
来源：http://baike.epnwcf.com/Article/details/gskeneggc.sHtML

[U48] PHP：纯枚举
来源：http://www.share.tarul.cn/Article/details/ggrkrybit.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.epnwcf.com/Article/details/gbnaodoni.sHtML

[U49] PHP：只读属性
来源：http://wap.fktsv.cn/Article/details/gsnsdpabu.sHtML

public readonly string $name
来源：http://www.blog.bbcook.cn/Article/details/gbdcqwioz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.epnwcf.com/Article/details/ghqyehxlw.sHtML

public function __construct(private int $id) {}
来源：http://3g.yfazqb.com/Article/details/gubscvtzl.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.tarul.cn/Article/details/gjhvqursh.sHtML

[$a, $b] = $arr;
来源：http://mobile.yfazqb.com/Article/details/gfuweiolb.sHtML

[U52] PHP：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gpwqbijcl.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fktsv.cn/Article/details/gjgmwvnww.sHtML

[U53] PHP：空合并运算符
来源：http://3g.epnwcf.com/Article/details/gyimbskpt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.bbcook.cn/Article/details/ghpaqsshf.sHtML

[U54] PHP：空安全调用
来源：http://baike.sjlbkw.cn/Article/details/goptktvmq.sHtML

$obj?->method()
来源：http://wap.yfazqb.com/Article/details/gbcescdns.sHtML

[U55] PHP：match 表达式
来源：http://3g.yfazqb.com/Article/details/gyyqjadhc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fktsv.cn/Article/details/grujwdepq.sHtML

[U56] PHP：命名参数
来源：http://mobile.fktsv.cn/Article/details/gtqdcwggd.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/ghwdvbptj.sHtML

[U57] PHP：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gzcadtycx.sHtML

"值: {$a}"
来源：http://www.share.sjlbkw.cn/Article/details/gciqqniic.sHtML

[U58] PHP：数组三件套
来源：http://baike.epnwcf.com/Article/details/gwazkqskl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.yfazqb.com/Article/details/gcsfophyu.sHtML

[U59] PHP：自定义排序
来源：http://www.share.bbcook.cn/Article/details/ggrpsfdhg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/gfaujktic.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.tarul.cn/Article/details/gokaverhr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.vehdjk.com/Article/details/gbrwhsbht.sHtML

[U61] PHP：正则
来源：http://www.share.sjlbkw.cn/Article/details/gcwpoalqx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/gqflgmako.sHtML

[U62] PHP：日期对象
来源：http://www.share.epnwcf.com/Article/details/ggmuttyea.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/golcnvttn.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.vehdjk.com/Article/details/glgdsinmw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.yfazqb.com/Article/details/gpkeasdqa.sHtML

[U64] PHP：目录遍历
来源：http://3g.yfazqb.com/Article/details/gkvdplqrb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.tarul.cn/Article/details/gadhzzjrs.sHtML

[U65] PHP：会话
来源：http://blog.yfazqb.com/Article/details/ggxnqgztf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhoyjazz.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.sjlbkw.cn/Article/details/grjkjlkfe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.epnwcf.com/Article/details/gpblzrkgp.sHtML

[U67] PHP：处理文件上传
来源：http://baike.sjlbkw.cn/Article/details/gouunagsp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.yfazqb.com/Article/details/gvjduefad.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.epnwcf.com/Article/details/gscbhfqbv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.bbcook.cn/Article/details/gfdxrhgdl.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.yfazqb.com/Article/details/guacsnrqb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.epnwcf.com/Article/details/grofoxwdx.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.yfazqb.com/Article/details/gvnwqymkr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpwgiark.sHtML

[U71] PHP：抛出异常
来源：http://baike.sjlbkw.cn/Article/details/gcjxqnfgi.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.vehdjk.com/Article/details/gpztxsydg.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.yfazqb.com/Article/details/gszqyrtwy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.bbcook.cn/Article/details/gvtzzulhz.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.vehdjk.com/Article/details/gpngmrgdp.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.yfazqb.com/Article/details/gmvepegcz.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.epnwcf.com/Article/details/grpxduvrb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.vehdjk.com/Article/details/gejzjtznr.sHtML

[U75] PHP：依赖注入
来源：http://m.share.sjlbkw.cn/Article/details/gfvbdprit.sHtML

composer require psr/container
来源：http://3g.bbcook.cn/Article/details/gfpkehvut.sHtML

[U76] PHP：简单路由
来源：http://mobile.sjlbkw.cn/Article/details/grxuyjoqt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.yfazqb.com/Article/details/gsjjqeipi.sHtML

[U77] PHP：模板渲染
来源：http://mobile.bbcook.cn/Article/details/gfmobftxe.sHtML

composer require twig/twig
来源：http://wap.yfazqb.com/Article/details/geuqiathf.sHtML

[U78] PHP：单元测试
来源：http://read.share.fktsv.cn/Article/details/gwlnfquas.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.tarul.cn/Article/details/gmxyeptfx.sHtML

[U79] PHP：静态分析
来源：http://mobile.sjlbkw.cn/Article/details/ginvpslxa.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fktsv.cn/Article/details/gdqjnwqgk.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.bbcook.cn/Article/details/gbcqevpfa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fktsv.cn/Article/details/gasnvucgj.sHtML

[U81] JS：初始化项目
来源：http://www.blog.bbcook.cn/Article/details/gvlzvxjvm.sHtML

npm init -y;  npm i express
来源：http://read.share.epnwcf.com/Article/details/gzgsriiqw.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fktsv.cn/Article/details/gplyqvfgj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fktsv.cn/Article/details/gyttmchla.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fktsv.cn/Article/details/gmjlzmjqa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.yfazqb.com/Article/details/ghdwmqmai.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.vehdjk.com/Article/details/gtfxyxdkc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.epnwcf.com/Article/details/gqvrssuqj.sHtML

[U85] JS：可选链
来源：http://read.share.epnwcf.com/Article/details/grfaflkgb.sHtML

a?.b?.c
来源：http://www.blog.bbcook.cn/Article/details/gxvvgqqqs.sHtML

[U86] JS：空值合并
来源：http://www.m.share.tarul.cn/Article/details/gaxpinkml.sHtML

a ?? b
来源：http://read.share.bbcook.cn/Article/details/gefgiyctd.sHtML

[U87] JS：解构默认值
来源：http://blog.yfazqb.com/Article/details/gklmireco.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.tarul.cn/Article/details/geshhbjup.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fktsv.cn/Article/details/gkirlpfih.sHtML

{ ...a, ...b }
来源：http://wap.yfazqb.com/Article/details/gfsufqzoo.sHtML

[U89] JS：数组去重
来源：http://www.share.epnwcf.com/Article/details/gptfanmbn.sHtML

[...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gmtjinjje.sHtML

[U90] JS：数字数组排序
来源：http://www.share.sjlbkw.cn/Article/details/gieelwahi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gxjdidfhm.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.bbcook.cn/Article/details/ghqyyygtw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.epnwcf.com/Article/details/guvhvyrty.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gpjsuegjs.sHtML

structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gequozkje.sHtML

[U93] JS：模板字符串
来源：http://read.share.epnwcf.com/Article/details/ggnwwhvyn.sHtML

`共 ${n} 条`
来源：http://mobile.bbcook.cn/Article/details/gjapmfkzi.sHtML

[U94] JS：箭头函数
来源：http://m.share.epnwcf.com/Article/details/grtzukxww.sHtML

const double = x => x * 2;
来源：http://3g.sjlbkw.cn/Article/details/giouvgfkr.sHtML

[U95] JS：Promise 包装
来源：http://baike.vehdjk.com/Article/details/gavazblpc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.epnwcf.com/Article/details/gjazavllp.sHtML

[U96] JS：async/await 与异常
来源：http://baike.yfazqb.com/Article/details/gwnovnsko.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gqgaivwpd.sHtML

[U97] JS：并发请求
来源：http://www.share.sjlbkw.cn/Article/details/gokgsfczx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gcmacehbw.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.epnwcf.com/Article/details/ggwsrufwr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.epnwcf.com/Article/details/gqroeomuv.sHtML

[U99] JS：事件监听
来源：http://3g.epnwcf.com/Article/details/gidanwjlc.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.sjlbkw.cn/Article/details/gwjtggsnx.sHtML

[U100] JS：DOM 查询
来源：http://mobile.epnwcf.com/Article/details/gqfewmmrt.sHtML

document.querySelector(".item")
来源：http://www.m.share.sjlbkw.cn/Article/details/genbhrcpb.sHtML

[U101] JS：classList 操作
来源：http://www.share.epnwcf.com/Article/details/gnmylnolp.sHtML

el.classList.toggle("active")
来源：http://www.share.tarul.cn/Article/details/gnksjyqip.sHtML

[U102] JS：本地存储
来源：http://read.share.bbcook.cn/Article/details/gxcsjokgg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.yfazqb.com/Article/details/gcyxkayyd.sHtML

[U103] JS：定时器
来源：http://m.share.bbcook.cn/Article/details/gnhjbcpqa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.vehdjk.com/Article/details/galljbtih.sHtML

[U104] JS：防抖
来源：http://www.blog.tarul.cn/Article/details/gwsgcfooz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gmvloqcsw.sHtML

[U105] JS：节流
来源：http://www.blog.epnwcf.com/Article/details/gxnbfznav.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.bbcook.cn/Article/details/gxfrpwacn.sHtML

[U106] JS：日期格式化
来源：http://read.share.yfazqb.com/Article/details/gdcrbznmw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.tarul.cn/Article/details/gxfmnueex.sHtML

[U107] JS：数字千分位
来源：http://wap.vehdjk.com/Article/details/grbekslkp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fktsv.cn/Article/details/gdnkeffli.sHtML

[U108] JS：随机整数
来源：http://mobile.tarul.cn/Article/details/genzqufcs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fktsv.cn/Article/details/gkgyfoluv.sHtML

[U109] JS：数组分组
来源：http://www.share.yfazqb.com/Article/details/grloarojm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gzcmqrkfd.sHtML

[U110] JS：数组分块
来源：http://www.share.tarul.cn/Article/details/gepczwvpl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.tarul.cn/Article/details/gsyxxtwgu.sHtML

[U111] JS：对象转 Map
来源：http://wap.epnwcf.com/Article/details/galrxdywz.sHtML

new Map(Object.entries(obj))
来源：http://blog.sjlbkw.cn/Article/details/goqapoysu.sHtML

[U112] JS：字符串补位
来源：http://www.blog.yfazqb.com/Article/details/gmjwqwsfa.sHtML

"7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/guhtqebfz.sHtML

[U113] JS：正则替换全部
来源：http://www.share.sjlbkw.cn/Article/details/gdugihbdj.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gailcsoig.sHtML

[U114] JS：JSON 深比较
来源：http://baike.epnwcf.com/Article/details/gshznjrfq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.bbcook.cn/Article/details/gyqupiwag.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/gcmndvjru.sHtML

crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gcyrhpmtm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.yfazqb.com/Article/details/gwyoxenvd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fktsv.cn/Article/details/gkzxovkdg.sHtML

[U117] JS：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gwtvfvedm.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fktsv.cn/Article/details/gsxvusgif.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.vehdjk.com/Article/details/gaccwkcew.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fktsv.cn/Article/details/gjhotxaws.sHtML

[U119] JS：生产构建
来源：http://m.share.tarul.cn/Article/details/gkkyfkvoi.sHtML

npx vite build
来源：http://www.blog.sjlbkw.cn/Article/details/grmedpmnw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fktsv.cn/Article/details/gfbdfhgct.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.epnwcf.com/Article/details/gvyqykoxd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjufuysnr.sHtML

统计汇总
来源：http://www.blog.epnwcf.com/Article/details/ghiniijdh.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmemnxbjq.sHtML

按语言统计（条）：
来源：http://www.share.yfazqb.com/Article/details/gbxdenimk.sHtML

Python ......... 252
来源：http://read.share.yfazqb.com/Article/details/ggxdovjrv.sHtML

PHP ............ 252
来源：http://www.blog.yfazqb.com/Article/details/grdfhwuig.sHtML

JavaScript ..... 252
来源：http://m.share.tarul.cn/Article/details/gnwpxufqw.sHtML

TypeScript ..... 212
来源：http://www.blog.vehdjk.com/Article/details/gxchhohth.sHtML

Java ........... 212
来源：http://m.share.epnwcf.com/Article/details/giedmkzlq.sHtML

Go ............. 212
来源：http://3g.tarul.cn/Article/details/ggyjkkdam.sHtML

Ruby ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gprirlkbi.sHtML

C# ............. 212
来源：http://m.share.fktsv.cn/Article/details/gxmwyrboj.sHtML

C .............. 30
来源：http://wap.epnwcf.com/Article/details/gumffelbj.sHtML

C++ ............ 30
来源：http://wap.fktsv.cn/Article/details/gwuwfikmc.sHtML

SQL ............ 90
来源：http://www.share.sjlbkw.cn/Article/details/gzuwzmvnm.sHtML

Bash ........... 80
来源：http://blog.vehdjk.com/Article/details/gmmxzpfqv.sHtML

Kotlin ......... 15
来源：http://read.share.yfazqb.com/Article/details/gbkbohzsi.sHtML

Swift .......... 15
来源：http://wap.yfazqb.com/Article/details/gsbintanc.sHtML

Lua ............ 10
来源：http://www.blog.yfazqb.com/Article/details/gwszxmwux.sHtML

Perl ........... 10
来源：http://m.share.vehdjk.com/Article/details/gtgxgetid.sHtML

Scala .......... 10
来源：http://www.share.tarul.cn/Article/details/gxlpvisjq.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/ggufatlvc.sHtML

合计 ........... 2106 条
来源：http://m.share.fktsv.cn/Article/details/grbsjgabg.sHtML

按章节统计：
来源：http://3g.epnwcf.com/Article/details/gyauqxgtu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.tarul.cn/Article/details/gyeivrdxq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gwojscxyv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/ggeyjhifg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.sjlbkw.cn/Article/details/gtmcinhhv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.bbcook.cn/Article/details/gspbrrwxg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fktsv.cn/Article/details/gqfnfutlb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gvboyhhnm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.vehdjk.com/Article/details/giqyzqbsq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gbpjghoan.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.vehdjk.com/Article/details/gywfnpofb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvxikcxj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gefqhswbb.sHtML


<!-- 参考信息 -->