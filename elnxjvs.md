代发 wailian999

[T49] Perl：函数
来源：http://www.share.yfazqb.com/Article/details/gniaajrra.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/geehxfrdd.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gtwxdybgk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.epnwcf.com/Article/details/geezkxngh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.vehdjk.com/Article/details/gfdxfmpfp.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/gjsiacnta.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gmharabgu.sHtML

[T52] Scala：变量
来源：http://blog.tarul.cn/Article/details/gsnelfeez.sHtML

val a = 1;  var b = 2
来源：http://baike.vehdjk.com/Article/details/gkigeufdz.sHtML

[T53] Scala：字符串插值
来源：http://wap.tarul.cn/Article/details/guttwlwvh.sHtML

s"值: $b"
来源：http://wap.tarul.cn/Article/details/gjmuxsiuc.sHtML

[T54] Scala：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gexgyushf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fktsv.cn/Article/details/ghniqgful.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gtrkzrghs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.sjlbkw.cn/Article/details/gvxyhcjpj.sHtML

[T56] Scala：样例类
来源：http://blog.tarul.cn/Article/details/glplpfsln.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gnpzxqyxl.sHtML

[T57] Scala：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gabvwuhyv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gspnldoui.sHtML

[T58] Scala：函数定义
来源：http://mobile.epnwcf.com/Article/details/gmihmwkfh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.sjlbkw.cn/Article/details/glhbpmpgg.sHtML

[T59] Scala：循环
来源：http://www.m.share.epnwcf.com/Article/details/gbolqipvk.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.tarul.cn/Article/details/gqnngrytw.sHtML

[T60] Scala：折叠
来源：http://www.blog.sjlbkw.cn/Article/details/gubnzuydj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.bbcook.cn/Article/details/gubhndyko.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gfvyfhegq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fktsv.cn/Article/details/guotxrigj.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gcxhoztii.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.epnwcf.com/Article/details/gslvlpbyw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fktsv.cn/Article/details/gafslwejb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.tarul.cn/Article/details/gthvzuxcx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.vehdjk.com/Article/details/gapmmiepn.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.vehdjk.com/Article/details/gyjjwwcur.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gyozvvrca.sHtML

[U04] Py：变量调试打印
来源：http://3g.bbcook.cn/Article/details/gidzxykla.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.bbcook.cn/Article/details/gciienuxo.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.vehdjk.com/Article/details/gqsuvscrl.sHtML

list(dict.fromkeys(arr))
来源：http://3g.vehdjk.com/Article/details/gtcxetjkt.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.yfazqb.com/Article/details/gbmmgyfeg.sHtML

{**a, **b}
来源：http://www.m.share.epnwcf.com/Article/details/govzppfva.sHtML

[U07] Py：反转字典键值
来源：http://3g.bbcook.cn/Article/details/guuxoqfar.sHtML

{v: k for k, v in d.items()}
来源：http://blog.epnwcf.com/Article/details/gxmansuvd.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.yfazqb.com/Article/details/gmalqhzew.sHtML

[y for x in nested for y in x]
来源：http://www.share.sjlbkw.cn/Article/details/gqouwwatf.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.bbcook.cn/Article/details/gbteuzvgr.sHtML

max(d, key=d.get)
来源：http://baike.sjlbkw.cn/Article/details/gpxfpoxvt.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/grvbfuoio.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fktsv.cn/Article/details/ghjzkffvi.sHtML

[U11] Py：生成器表达式
来源：http://baike.tarul.cn/Article/details/gvsinbgoi.sHtML

(x * 2 for x in arr)
来源：http://3g.fktsv.cn/Article/details/gjpmgssxr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.vehdjk.com/Article/details/ghoyoycjd.sHtML

Counter(arr).most_common(3)
来源：http://m.share.vehdjk.com/Article/details/glfbijwvp.sHtML

[U13] Py：固定长度队列
来源：http://blog.fktsv.cn/Article/details/gvtmmcjgl.sHtML

deque(maxlen=10)
来源：http://www.blog.yfazqb.com/Article/details/ggxbtfbyt.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.vehdjk.com/Article/details/gmnawtvpl.sHtML

defaultdict(list)
来源：http://blog.yfazqb.com/Article/details/gtayrbqud.sHtML

[U15] Py：高精度计时
来源：http://wap.tarul.cn/Article/details/gvefxwstu.sHtML

t = time.perf_counter()
来源：http://baike.fktsv.cn/Article/details/geiaaohuw.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.tarul.cn/Article/details/gfgoqmmpe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.bbcook.cn/Article/details/gtrtaddfs.sHtML

[U17] Py：初始化日志
来源：http://baike.bbcook.cn/Article/details/ggxezetqg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.vehdjk.com/Article/details/grskvytkp.sHtML

[U18] Py：预编译正则
来源：http://3g.vehdjk.com/Article/details/ghhgkyvnj.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/gghttcdim.sHtML

[U19] Py：正则替换带回调
来源：http://3g.yfazqb.com/Article/details/gldismxkx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fktsv.cn/Article/details/gbtcrasqw.sHtML

[U20] Py：缓存函数结果
来源：http://3g.bbcook.cn/Article/details/grnvtwdjo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.epnwcf.com/Article/details/gzjuriciu.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.vehdjk.com/Article/details/gvppsoelz.sHtML

@contextlib.contextmanager
来源：http://wap.bbcook.cn/Article/details/ghzyjmzig.sHtML

[U22] Py：矩阵转置
来源：http://read.share.vehdjk.com/Article/details/gkhewsntn.sHtML

list(zip(*m))
来源：http://m.share.bbcook.cn/Article/details/gqsdcdupe.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.vehdjk.com/Article/details/glssdmxqq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.vehdjk.com/Article/details/gulkhbpjd.sHtML

[U24] Py：路径操作
来源：http://3g.yfazqb.com/Article/details/gsncccuoi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gzwzazatm.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fktsv.cn/Article/details/gdzfcwuig.sHtML

csv.DictReader(f)
来源：http://m.share.sjlbkw.cn/Article/details/ghsqnxptl.sHtML

[U26] Py：并发下载
来源：http://m.share.epnwcf.com/Article/details/gcagperqi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.vehdjk.com/Article/details/ghmhrnxfr.sHtML

[U27] Py：异步 HTTP
来源：http://3g.vehdjk.com/Article/details/gxghkacjk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.vehdjk.com/Article/details/gkhxrovex.sHtML

[U28] Py：类型别名
来源：http://wap.yfazqb.com/Article/details/gizrjmjcy.sHtML

UserId = int
来源：http://blog.vehdjk.com/Article/details/gsslqslag.sHtML

[U29] Py：属性校验
来源：http://mobile.vehdjk.com/Article/details/gtepnudoo.sHtML

@property 与 @x.setter 配合
来源：http://blog.yfazqb.com/Article/details/ghgalodfl.sHtML

[U30] Py：数据类
来源：http://3g.tarul.cn/Article/details/gqwxbveqq.sHtML

@dataclass(slots=True)
来源：http://read.share.bbcook.cn/Article/details/gojijqqnp.sHtML

[U31] Py：单测
来源：http://www.blog.epnwcf.com/Article/details/geoptaofd.sHtML

python -m pytest -q
来源：http://blog.sjlbkw.cn/Article/details/gsfcvwzsh.sHtML

[U32] Py：代码格式化
来源：http://blog.bbcook.cn/Article/details/giawaupwb.sHtML

ruff format . && ruff check --fix .
来源：http://baike.sjlbkw.cn/Article/details/gupofjbnm.sHtML

[U33] Py：打包发布
来源：http://mobile.fktsv.cn/Article/details/gsxitkcer.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fktsv.cn/Article/details/grzhnzkck.sHtML

[U34] Py：判断编码
来源：http://m.share.tarul.cn/Article/details/gxtmowdkn.sHtML

chardet.detect(raw)
来源：http://wap.yfazqb.com/Article/details/gcfzedkod.sHtML

[U35] Py：发送邮件
来源：http://m.share.bbcook.cn/Article/details/gfcnrxrua.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fktsv.cn/Article/details/genybhpbc.sHtML

[U36] Py：定时任务
来源：http://wap.tarul.cn/Article/details/glssvcxyc.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.tarul.cn/Article/details/gihjcmccf.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fktsv.cn/Article/details/gxaeoqyac.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.epnwcf.com/Article/details/ggynijfoh.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fktsv.cn/Article/details/ggcfiudms.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.tarul.cn/Article/details/gwktwdrkk.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.yfazqb.com/Article/details/gfmbmbenr.sHtML

sys.stdout.isatty()
来源：http://3g.fktsv.cn/Article/details/gybgxsyxf.sHtML

[U40] Py：打印到标准错误
来源：http://blog.yfazqb.com/Article/details/gdkmrwcfq.sHtML

print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/gwcdqbvkq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.epnwcf.com/Article/details/gbcrqdxaw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.sjlbkw.cn/Article/details/gmgwthsxj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.epnwcf.com/Article/details/ghelonsvw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.vehdjk.com/Article/details/gbplufytb.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.sjlbkw.cn/Article/details/glaymentc.sHtML

namespace App\Http;
来源：http://3g.sjlbkw.cn/Article/details/gkzgxwzmh.sHtML

[U44] PHP：开启严格类型
来源：http://wap.yfazqb.com/Article/details/grjsvicgn.sHtML

declare(strict_types=1);
来源：http://mobile.yfazqb.com/Article/details/gdlzjzzqz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.sjlbkw.cn/Article/details/gafxhbtnc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gbfjxnmyi.sHtML

[U46] PHP：可空类型
来源：http://3g.vehdjk.com/Article/details/ggobhvmcw.sHtML

?string $name = null
来源：http://blog.epnwcf.com/Article/details/gftddfxvd.sHtML

[U47] PHP：联合类型
来源：http://3g.yfazqb.com/Article/details/gnkmbwcoz.sHtML

int|string $id
来源：http://m.share.bbcook.cn/Article/details/gjicyveuc.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fktsv.cn/Article/details/gcfrhtufm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.vehdjk.com/Article/details/gakvyrcmm.sHtML

[U49] PHP：只读属性
来源：http://m.share.tarul.cn/Article/details/grewmzrgm.sHtML

public readonly string $name
来源：http://mobile.yfazqb.com/Article/details/gpuyzwxvm.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.bbcook.cn/Article/details/gwqazswua.sHtML

public function __construct(private int $id) {}
来源：http://blog.yfazqb.com/Article/details/gsyzbbegm.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gblvasuop.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.tarul.cn/Article/details/ghpwjcheh.sHtML

[U52] PHP：箭头函数
来源：http://blog.epnwcf.com/Article/details/gsxbncbzq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fktsv.cn/Article/details/gtcduqoqi.sHtML

[U53] PHP：空合并运算符
来源：http://wap.vehdjk.com/Article/details/gbdurcamj.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.tarul.cn/Article/details/glcqfdxzh.sHtML

[U54] PHP：空安全调用
来源：http://www.share.tarul.cn/Article/details/gdmgvdzxv.sHtML

$obj?->method()
来源：http://www.blog.sjlbkw.cn/Article/details/gounfeqaj.sHtML

[U55] PHP：match 表达式
来源：http://3g.epnwcf.com/Article/details/gyhvbqyda.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fktsv.cn/Article/details/gubnirzxt.sHtML

[U56] PHP：命名参数
来源：http://3g.bbcook.cn/Article/details/gzcheeqol.sHtML

f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/ggmgrmhrk.sHtML

[U57] PHP：字符串插值
来源：http://mobile.yfazqb.com/Article/details/girljvptv.sHtML

"值: {$a}"
来源：http://www.share.tarul.cn/Article/details/gfldlmqpb.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fktsv.cn/Article/details/gurgkgswi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.bbcook.cn/Article/details/gmbyeauzs.sHtML

[U59] PHP：自定义排序
来源：http://wap.vehdjk.com/Article/details/glfbmbmtr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.tarul.cn/Article/details/gbrrqybji.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.vehdjk.com/Article/details/gexzrlheb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fktsv.cn/Article/details/gathvfisr.sHtML

[U61] PHP：正则
来源：http://wap.sjlbkw.cn/Article/details/gcqnzmybr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/gxzfatuvb.sHtML

[U62] PHP：日期对象
来源：http://blog.tarul.cn/Article/details/gqmlgzvnc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.vehdjk.com/Article/details/gyqauvzxm.sHtML

[U63] PHP：文件读写
来源：http://3g.sjlbkw.cn/Article/details/gdonfhqwl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.sjlbkw.cn/Article/details/gkmbtwaqg.sHtML

[U64] PHP：目录遍历
来源：http://m.share.yfazqb.com/Article/details/givnrmvih.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.vehdjk.com/Article/details/gjqfozqnj.sHtML

[U65] PHP：会话
来源：http://wap.vehdjk.com/Article/details/gyphnzcss.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.yfazqb.com/Article/details/gbciqivxh.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.sjlbkw.cn/Article/details/ggacbkajb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.bbcook.cn/Article/details/gncpkwdph.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.epnwcf.com/Article/details/grnzmpkqb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.tarul.cn/Article/details/glqnpjxvz.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.vehdjk.com/Article/details/gvkpwlogt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.epnwcf.com/Article/details/gvcxvveiw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.tarul.cn/Article/details/gsxcyvpuf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.sjlbkw.cn/Article/details/gvroiyufx.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.sjlbkw.cn/Article/details/gqdfllvzk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fktsv.cn/Article/details/grnnfrmeu.sHtML

[U71] PHP：抛出异常
来源：http://wap.yfazqb.com/Article/details/gnxchltix.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.sjlbkw.cn/Article/details/guosdhecr.sHtML

[U72] PHP：写错误日志
来源：http://mobile.vehdjk.com/Article/details/gmciwplgg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.epnwcf.com/Article/details/ghrkkuizd.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.tarul.cn/Article/details/gwmhlveyr.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.epnwcf.com/Article/details/gpppcranx.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fktsv.cn/Article/details/gtfmzkmly.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.yfazqb.com/Article/details/gulqlnmpl.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fktsv.cn/Article/details/gfgyicyst.sHtML

composer require psr/container
来源：http://mobile.sjlbkw.cn/Article/details/gidlypwgn.sHtML

[U76] PHP：简单路由
来源：http://blog.fktsv.cn/Article/details/grozylxth.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.vehdjk.com/Article/details/gmfaskmdk.sHtML

[U77] PHP：模板渲染
来源：http://mobile.bbcook.cn/Article/details/goypphjzc.sHtML

composer require twig/twig
来源：http://www.m.share.bbcook.cn/Article/details/gxcknrkgi.sHtML

[U78] PHP：单元测试
来源：http://blog.yfazqb.com/Article/details/ghsdsdzwz.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.yfazqb.com/Article/details/grljzhnkm.sHtML

[U79] PHP：静态分析
来源：http://read.share.yfazqb.com/Article/details/geuhnjtla.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.tarul.cn/Article/details/ghjkjqlej.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fktsv.cn/Article/details/geceqxmzt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.bbcook.cn/Article/details/gsydaqlco.sHtML

[U81] JS：初始化项目
来源：http://wap.fktsv.cn/Article/details/gksusqfzy.sHtML

npm init -y;  npm i express
来源：http://www.share.sjlbkw.cn/Article/details/gijaaukol.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fktsv.cn/Article/details/gswvsmnth.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.epnwcf.com/Article/details/gejnywxjl.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.vehdjk.com/Article/details/gtflgyoix.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gmamvnevo.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.tarul.cn/Article/details/gpxprbuky.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.epnwcf.com/Article/details/gzczymscc.sHtML

[U85] JS：可选链
来源：http://m.share.fktsv.cn/Article/details/giippqaik.sHtML

a?.b?.c
来源：http://read.share.sjlbkw.cn/Article/details/gmihdprbg.sHtML

[U86] JS：空值合并
来源：http://www.share.fktsv.cn/Article/details/gshbsosrg.sHtML

a ?? b
来源：http://www.share.bbcook.cn/Article/details/gdmxjvlgz.sHtML

[U87] JS：解构默认值
来源：http://m.share.sjlbkw.cn/Article/details/gviduyegx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.vehdjk.com/Article/details/gcmctyrho.sHtML

[U88] JS：对象展开合并
来源：http://read.share.bbcook.cn/Article/details/gwdjvegsx.sHtML

{ ...a, ...b }
来源：http://3g.sjlbkw.cn/Article/details/gmpcqngau.sHtML

[U89] JS：数组去重
来源：http://3g.fktsv.cn/Article/details/gewwhqzsv.sHtML

[...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gdojyhora.sHtML

[U90] JS：数字数组排序
来源：http://blog.bbcook.cn/Article/details/gfctnocxp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gseyemmfl.sHtML

[U91] JS：对象键值遍历
来源：http://blog.tarul.cn/Article/details/gtuglqknl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.tarul.cn/Article/details/gjnoxgfur.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxltlnnt.sHtML

structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/getmtcwnw.sHtML

[U93] JS：模板字符串
来源：http://www.blog.tarul.cn/Article/details/gxtgpjczc.sHtML

`共 ${n} 条`
来源：http://mobile.vehdjk.com/Article/details/gmppcblio.sHtML

[U94] JS：箭头函数
来源：http://baike.bbcook.cn/Article/details/ghtwqahmr.sHtML

const double = x => x * 2;
来源：http://www.m.share.fktsv.cn/Article/details/gkckfkuaz.sHtML

[U95] JS：Promise 包装
来源：http://read.share.sjlbkw.cn/Article/details/ggcxmcpwo.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.tarul.cn/Article/details/gavqqbret.sHtML

[U96] JS：async/await 与异常
来源：http://baike.sjlbkw.cn/Article/details/gyeinovxu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gkuetylzi.sHtML

[U97] JS：并发请求
来源：http://www.blog.tarul.cn/Article/details/gvkkkavhm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gthuxrwjh.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fktsv.cn/Article/details/gmjzwcqav.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.tarul.cn/Article/details/gvpucfetc.sHtML

[U99] JS：事件监听
来源：http://3g.tarul.cn/Article/details/gifoldsho.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fktsv.cn/Article/details/gybyrkkjj.sHtML

[U100] JS：DOM 查询
来源：http://read.share.epnwcf.com/Article/details/ggugtfspq.sHtML

document.querySelector(".item")
来源：http://mobile.fktsv.cn/Article/details/gvlewiqtt.sHtML

[U101] JS：classList 操作
来源：http://baike.fktsv.cn/Article/details/gtnuklcyk.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fktsv.cn/Article/details/gjtkxwdff.sHtML

[U102] JS：本地存储
来源：http://www.blog.sjlbkw.cn/Article/details/gxwqmcfxp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.vehdjk.com/Article/details/gyvajntdm.sHtML

[U103] JS：定时器
来源：http://baike.sjlbkw.cn/Article/details/gtkbzyjbk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.bbcook.cn/Article/details/goihovgzp.sHtML

[U104] JS：防抖
来源：http://blog.vehdjk.com/Article/details/gydvjmzke.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/gnwhinyqt.sHtML

[U105] JS：节流
来源：http://read.share.epnwcf.com/Article/details/gbbmbzknp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.vehdjk.com/Article/details/ghitetkan.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gnzvixxnk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.sjlbkw.cn/Article/details/galjnpqte.sHtML

[U107] JS：数字千分位
来源：http://www.share.yfazqb.com/Article/details/gvntmbdwm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.sjlbkw.cn/Article/details/gyhxvdfhp.sHtML

[U108] JS：随机整数
来源：http://www.m.share.bbcook.cn/Article/details/gjxlzaeqh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.bbcook.cn/Article/details/gofdogfgp.sHtML

[U109] JS：数组分组
来源：http://mobile.vehdjk.com/Article/details/goldrfixm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gsznlozql.sHtML

[U110] JS：数组分块
来源：http://mobile.epnwcf.com/Article/details/ghxinasdc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.tarul.cn/Article/details/gdufieuyg.sHtML

[U111] JS：对象转 Map
来源：http://read.share.yfazqb.com/Article/details/geprfztzl.sHtML

new Map(Object.entries(obj))
来源：http://baike.fktsv.cn/Article/details/gxavekhze.sHtML

[U112] JS：字符串补位
来源：http://3g.vehdjk.com/Article/details/gmvfothot.sHtML

"7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/geoqthyvx.sHtML

[U113] JS：正则替换全部
来源：http://m.share.sjlbkw.cn/Article/details/gfktyzjbd.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/ghgsrnrdt.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.epnwcf.com/Article/details/gxyhtawhz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.sjlbkw.cn/Article/details/gyjrefeja.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gaeoegped.sHtML

crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gnlxgbbpm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.yfazqb.com/Article/details/gfczyrmhf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fktsv.cn/Article/details/gknrhzhzv.sHtML

[U117] JS：单元测试
来源：http://www.m.share.yfazqb.com/Article/details/gvkprxgoi.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpvbphvt.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fktsv.cn/Article/details/gtictfpwz.sHtML

npm i -D vite;  npx vite
来源：http://read.share.vehdjk.com/Article/details/gjdeifair.sHtML

[U119] JS：生产构建
来源：http://www.blog.epnwcf.com/Article/details/gpumigrpa.sHtML

npx vite build
来源：http://read.share.sjlbkw.cn/Article/details/gdxehakjl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.epnwcf.com/Article/details/gxexmfchk.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.bbcook.cn/Article/details/gbrcsrlhh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghjmwjiaz.sHtML

统计汇总
来源：http://www.blog.tarul.cn/Article/details/gmdstdrre.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmopsongq.sHtML

按语言统计（条）：
来源：http://m.share.sjlbkw.cn/Article/details/gnnbrogoj.sHtML

Python ......... 252
来源：http://3g.yfazqb.com/Article/details/guahtczol.sHtML

PHP ............ 252
来源：http://mobile.fktsv.cn/Article/details/gditcubku.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/gnzsnlmlf.sHtML

TypeScript ..... 212
来源：http://baike.vehdjk.com/Article/details/gstscqxkh.sHtML

Java ........... 212
来源：http://read.share.sjlbkw.cn/Article/details/gihhynraj.sHtML

Go ............. 212
来源：http://baike.bbcook.cn/Article/details/gwlarvyix.sHtML

Ruby ........... 212
来源：http://wap.sjlbkw.cn/Article/details/gjjoqnlbw.sHtML

C# ............. 212
来源：http://baike.bbcook.cn/Article/details/gewdoqsgi.sHtML

C .............. 30
来源：http://3g.vehdjk.com/Article/details/gnyowofik.sHtML

C++ ............ 30
来源：http://m.share.yfazqb.com/Article/details/gslthftuf.sHtML

SQL ............ 90
来源：http://baike.sjlbkw.cn/Article/details/ggnbtfirl.sHtML

Bash ........... 80
来源：http://baike.vehdjk.com/Article/details/gubgmrvye.sHtML

Kotlin ......... 15
来源：http://www.blog.fktsv.cn/Article/details/gpjzobjfl.sHtML

Swift .......... 15
来源：http://m.share.vehdjk.com/Article/details/gnuozigza.sHtML

Lua ............ 10
来源：http://www.share.sjlbkw.cn/Article/details/gitpkvrkd.sHtML

Perl ........... 10
来源：http://www.blog.sjlbkw.cn/Article/details/gjyvpaxur.sHtML

Scala .......... 10
来源：http://blog.bbcook.cn/Article/details/gndvyoycj.sHtML

------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gantkutbh.sHtML

合计 ........... 2106 条
来源：http://www.share.epnwcf.com/Article/details/gplmjhepd.sHtML

按章节统计：
来源：http://3g.yfazqb.com/Article/details/gxmmnfonj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.yfazqb.com/Article/details/gviqgnzlw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/garnitkjm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gvlaudrde.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.yfazqb.com/Article/details/genaatszr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.bbcook.cn/Article/details/gxfkotlhj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/gmpydiakt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/gtrlopxio.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.sjlbkw.cn/Article/details/gvawxmkxc.sHtML


<!-- 参考信息 -->