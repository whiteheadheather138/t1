代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.tarul.cn/Article/details/gwpeotpyg.sHtML

[T51] Scala：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gayufezlc.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/gwvauejyy.sHtML

[T52] Scala：变量
来源：http://baike.yfazqb.com/Article/details/gertzxhwm.sHtML

val a = 1;  var b = 2
来源：http://3g.bbcook.cn/Article/details/gjdlwjevi.sHtML

[T53] Scala：字符串插值
来源：http://3g.epnwcf.com/Article/details/gzeirwgkj.sHtML

s"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/gqtqpbnsg.sHtML

[T54] Scala：集合映射
来源：http://mobile.fktsv.cn/Article/details/goszlzjsr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.vehdjk.com/Article/details/grlawbdea.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/gstmtyops.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.epnwcf.com/Article/details/gjpmpglrb.sHtML

[T56] Scala：样例类
来源：http://read.share.yfazqb.com/Article/details/gmpoobnup.sHtML

case class User(name: String, age: Int)
来源：http://read.share.epnwcf.com/Article/details/gkotulwko.sHtML

[T57] Scala：模式匹配
来源：http://blog.vehdjk.com/Article/details/gsteugsrw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.yfazqb.com/Article/details/gtsmxdzrm.sHtML

[T58] Scala：函数定义
来源：http://m.share.epnwcf.com/Article/details/gmrheynra.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.vehdjk.com/Article/details/guxmoapun.sHtML

[T59] Scala：循环
来源：http://blog.vehdjk.com/Article/details/ghndpecog.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.yfazqb.com/Article/details/glxrwhhmb.sHtML

[T60] Scala：折叠
来源：http://www.share.yfazqb.com/Article/details/gjtbycfoj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.tarul.cn/Article/details/gwgrfavda.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gvrluzrxb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.bbcook.cn/Article/details/ghiapeuca.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwmgzrsoc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.epnwcf.com/Article/details/gfhbdqbne.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.tarul.cn/Article/details/giuwucbxg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.epnwcf.com/Article/details/ghpzvrxil.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.bbcook.cn/Article/details/gjvvwcfsr.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fktsv.cn/Article/details/gqyocmogq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gpjjogaba.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.tarul.cn/Article/details/gyqjnxyvv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.tarul.cn/Article/details/gujvoaooe.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.vehdjk.com/Article/details/gycjwjlia.sHtML

list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/gbcobweui.sHtML

[U06] Py：合并两个字典
来源：http://wap.bbcook.cn/Article/details/gursimdgj.sHtML

{**a, **b}
来源：http://m.share.sjlbkw.cn/Article/details/glmiigush.sHtML

[U07] Py：反转字典键值
来源：http://baike.vehdjk.com/Article/details/gvknykfkd.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.vehdjk.com/Article/details/gjbzjhgxm.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.tarul.cn/Article/details/gkxugmlhf.sHtML

[y for x in nested for y in x]
来源：http://m.share.tarul.cn/Article/details/gyfhvvbbs.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.bbcook.cn/Article/details/gpulxihqu.sHtML

max(d, key=d.get)
来源：http://m.share.vehdjk.com/Article/details/gcwfzszik.sHtML

[U10] Py：按值排序字典
来源：http://blog.yfazqb.com/Article/details/gzyjldjma.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.sjlbkw.cn/Article/details/gbzogyknt.sHtML

[U11] Py：生成器表达式
来源：http://www.share.tarul.cn/Article/details/gysnvwkca.sHtML

(x * 2 for x in arr)
来源：http://wap.sjlbkw.cn/Article/details/gqvxbybvz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.tarul.cn/Article/details/gomqyutti.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fktsv.cn/Article/details/gwtufqzav.sHtML

[U13] Py：固定长度队列
来源：http://read.share.vehdjk.com/Article/details/ghfixillq.sHtML

deque(maxlen=10)
来源：http://m.share.epnwcf.com/Article/details/gwmiqfhcc.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.yfazqb.com/Article/details/gozjzboic.sHtML

defaultdict(list)
来源：http://mobile.epnwcf.com/Article/details/gthoibfki.sHtML

[U15] Py：高精度计时
来源：http://read.share.yfazqb.com/Article/details/gznvspiku.sHtML

t = time.perf_counter()
来源：http://baike.vehdjk.com/Article/details/gfixskqsi.sHtML

[U16] Py：命令行参数解析
来源：http://3g.vehdjk.com/Article/details/gnkhvdpzi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.tarul.cn/Article/details/gertkrwjs.sHtML

[U17] Py：初始化日志
来源：http://wap.yfazqb.com/Article/details/ggclijecx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.tarul.cn/Article/details/gzivmkqra.sHtML

[U18] Py：预编译正则
来源：http://read.share.bbcook.cn/Article/details/gpoxjevrn.sHtML

pat = re.compile(r"\d+")
来源：http://3g.yfazqb.com/Article/details/gkrvnodxo.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.epnwcf.com/Article/details/gxygoyeve.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fktsv.cn/Article/details/gthoghgnv.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.tarul.cn/Article/details/glmhbyfho.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.sjlbkw.cn/Article/details/gvvowrqdw.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.vehdjk.com/Article/details/goyvbckcy.sHtML

@contextlib.contextmanager
来源：http://3g.fktsv.cn/Article/details/gndtanqmr.sHtML

[U22] Py：矩阵转置
来源：http://read.share.yfazqb.com/Article/details/gbwuiggbn.sHtML

list(zip(*m))
来源：http://baike.bbcook.cn/Article/details/gbyosecfi.sHtML

[U23] Py：分块读取大文件
来源：http://blog.vehdjk.com/Article/details/ginjzvrnw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.epnwcf.com/Article/details/gyzosnkqu.sHtML

[U24] Py：路径操作
来源：http://m.share.tarul.cn/Article/details/gvwkqlcxz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gjwzbjrns.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.epnwcf.com/Article/details/gpybvepys.sHtML

csv.DictReader(f)
来源：http://m.share.epnwcf.com/Article/details/gpfvicguu.sHtML

[U26] Py：并发下载
来源：http://baike.epnwcf.com/Article/details/gmxxteozh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.sjlbkw.cn/Article/details/gzkfhvbiq.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.epnwcf.com/Article/details/gzdrfpmqz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.tarul.cn/Article/details/gxbkknbud.sHtML

[U28] Py：类型别名
来源：http://m.share.vehdjk.com/Article/details/gpnvhmpjg.sHtML

UserId = int
来源：http://www.m.share.yfazqb.com/Article/details/gubkvrybb.sHtML

[U29] Py：属性校验
来源：http://wap.sjlbkw.cn/Article/details/gxbuvblyi.sHtML

@property 与 @x.setter 配合
来源：http://mobile.vehdjk.com/Article/details/ghjhrrkjc.sHtML

[U30] Py：数据类
来源：http://baike.bbcook.cn/Article/details/gftgyujxr.sHtML

@dataclass(slots=True)
来源：http://3g.tarul.cn/Article/details/gtlyjxbyr.sHtML

[U31] Py：单测
来源：http://www.m.share.fktsv.cn/Article/details/gssyzhkrr.sHtML

python -m pytest -q
来源：http://baike.fktsv.cn/Article/details/gvhrwzlrf.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.vehdjk.com/Article/details/gfeiskmfi.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fktsv.cn/Article/details/gybicbegu.sHtML

[U33] Py：打包发布
来源：http://baike.tarul.cn/Article/details/gwptbgltu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.epnwcf.com/Article/details/gefzydrec.sHtML

[U34] Py：判断编码
来源：http://3g.bbcook.cn/Article/details/gidwmddnf.sHtML

chardet.detect(raw)
来源：http://www.share.fktsv.cn/Article/details/galtkpyyc.sHtML

[U35] Py：发送邮件
来源：http://wap.fktsv.cn/Article/details/gdsamxcdb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.sjlbkw.cn/Article/details/gcadppejb.sHtML

[U36] Py：定时任务
来源：http://blog.yfazqb.com/Article/details/gsumlyedu.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.tarul.cn/Article/details/gichzwhhl.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.epnwcf.com/Article/details/gawpceksp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.sjlbkw.cn/Article/details/gezdeydxa.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.vehdjk.com/Article/details/gqtnkdwhz.sHtML

Path(__file__).resolve().parent
来源：http://3g.yfazqb.com/Article/details/gqgpwydvf.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.epnwcf.com/Article/details/gohfbltbx.sHtML

sys.stdout.isatty()
来源：http://baike.epnwcf.com/Article/details/gkbvpffbz.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.yfazqb.com/Article/details/gwhntrzcr.sHtML

print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/gmkhojius.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.sjlbkw.cn/Article/details/gmdxncsxf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxfeschb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.bbcook.cn/Article/details/gxyrhpcpy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.yfazqb.com/Article/details/gbofxpkle.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.vehdjk.com/Article/details/gerbjpycg.sHtML

namespace App\Http;
来源：http://www.blog.fktsv.cn/Article/details/gvnqqezxk.sHtML

[U44] PHP：开启严格类型
来源：http://wap.sjlbkw.cn/Article/details/gwarvizdx.sHtML

declare(strict_types=1);
来源：http://blog.vehdjk.com/Article/details/gxcfzgepx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.bbcook.cn/Article/details/gplkoanwf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gplitjixt.sHtML

[U46] PHP：可空类型
来源：http://mobile.sjlbkw.cn/Article/details/gmufztasr.sHtML

?string $name = null
来源：http://www.m.share.fktsv.cn/Article/details/gigzebmjc.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.bbcook.cn/Article/details/gtsoemflq.sHtML

int|string $id
来源：http://mobile.epnwcf.com/Article/details/grwfbejli.sHtML

[U48] PHP：纯枚举
来源：http://wap.yfazqb.com/Article/details/ghlychnxf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.sjlbkw.cn/Article/details/gqduunwir.sHtML

[U49] PHP：只读属性
来源：http://blog.sjlbkw.cn/Article/details/gnezdxxyy.sHtML

public readonly string $name
来源：http://www.m.share.vehdjk.com/Article/details/gcnemyefe.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.epnwcf.com/Article/details/grhifhjpk.sHtML

public function __construct(private int $id) {}
来源：http://blog.epnwcf.com/Article/details/gfldefhpz.sHtML

[U51] PHP：数组解构
来源：http://m.share.yfazqb.com/Article/details/gbqetifiu.sHtML

[$a, $b] = $arr;
来源：http://wap.bbcook.cn/Article/details/gloodrvdc.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.yfazqb.com/Article/details/gtiartoih.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.vehdjk.com/Article/details/gpogkmudc.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.sjlbkw.cn/Article/details/goluvyzum.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.yfazqb.com/Article/details/ganojcbva.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fktsv.cn/Article/details/gsvdmrziy.sHtML

$obj?->method()
来源：http://wap.tarul.cn/Article/details/gproidsrw.sHtML

[U55] PHP：match 表达式
来源：http://blog.fktsv.cn/Article/details/gsjvplarg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.epnwcf.com/Article/details/gvvtwxdxm.sHtML

[U56] PHP：命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gdwuccbnj.sHtML

f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gihatwozb.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gfecbzhnt.sHtML

"值: {$a}"
来源：http://mobile.yfazqb.com/Article/details/geoeaqbjb.sHtML

[U58] PHP：数组三件套
来源：http://read.share.yfazqb.com/Article/details/ghyoqaqqm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.vehdjk.com/Article/details/glzohllxd.sHtML

[U59] PHP：自定义排序
来源：http://wap.bbcook.cn/Article/details/gkbnrixap.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.tarul.cn/Article/details/gxhsukcef.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.sjlbkw.cn/Article/details/gztoxgcwz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fktsv.cn/Article/details/ggfvnvyxr.sHtML

[U61] PHP：正则
来源：http://3g.sjlbkw.cn/Article/details/gbtbcajjr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/geezrfbnv.sHtML

[U62] PHP：日期对象
来源：http://www.share.epnwcf.com/Article/details/gjcswjkkr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.bbcook.cn/Article/details/gupwzhesz.sHtML

[U63] PHP：文件读写
来源：http://www.share.tarul.cn/Article/details/gkjrfloko.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.epnwcf.com/Article/details/gkbdzzvom.sHtML

[U64] PHP：目录遍历
来源：http://read.share.epnwcf.com/Article/details/gdewtpkda.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.sjlbkw.cn/Article/details/gkhtwahtd.sHtML

[U65] PHP：会话
来源：http://mobile.vehdjk.com/Article/details/gxcjboaum.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gajnrslum.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.epnwcf.com/Article/details/gcmrxwkcd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.bbcook.cn/Article/details/gqucginsk.sHtML

[U67] PHP：处理文件上传
来源：http://wap.bbcook.cn/Article/details/gejgopqwc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.yfazqb.com/Article/details/gfycbbase.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fktsv.cn/Article/details/gkuialbyj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.bbcook.cn/Article/details/gauzzuwrs.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.sjlbkw.cn/Article/details/gvdjukvyp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.epnwcf.com/Article/details/ganqwqyde.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.vehdjk.com/Article/details/gnvsardja.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.bbcook.cn/Article/details/gnjrlkcwb.sHtML

[U71] PHP：抛出异常
来源：http://read.share.bbcook.cn/Article/details/gjgrbvhmj.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fktsv.cn/Article/details/gposksycg.sHtML

[U72] PHP：写错误日志
来源：http://m.share.sjlbkw.cn/Article/details/gwmrapxwf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.bbcook.cn/Article/details/gqiqkduuk.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.vehdjk.com/Article/details/ggaoclfdb.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.yfazqb.com/Article/details/gieqytiaj.sHtML

[U74] PHP：读取环境变量
来源：http://wap.tarul.cn/Article/details/gvwdqnrhq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.epnwcf.com/Article/details/gqcvezpqe.sHtML

[U75] PHP：依赖注入
来源：http://wap.tarul.cn/Article/details/gqjxctfmy.sHtML

composer require psr/container
来源：http://mobile.fktsv.cn/Article/details/gdzuoibfl.sHtML

[U76] PHP：简单路由
来源：http://3g.yfazqb.com/Article/details/gjnmswyir.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.bbcook.cn/Article/details/gwcgeuvgi.sHtML

[U77] PHP：模板渲染
来源：http://m.share.sjlbkw.cn/Article/details/guvawecys.sHtML

composer require twig/twig
来源：http://www.m.share.yfazqb.com/Article/details/gskavtsfb.sHtML

[U78] PHP：单元测试
来源：http://wap.epnwcf.com/Article/details/gzlsgsxip.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.epnwcf.com/Article/details/gnmvfemxe.sHtML

[U79] PHP：静态分析
来源：http://www.blog.yfazqb.com/Article/details/gkbacptsy.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.epnwcf.com/Article/details/gyfsvkfrx.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.tarul.cn/Article/details/geqgpoxpb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.tarul.cn/Article/details/gxlmfknct.sHtML

[U81] JS：初始化项目
来源：http://mobile.yfazqb.com/Article/details/gdxrbezpz.sHtML

npm init -y;  npm i express
来源：http://read.share.sjlbkw.cn/Article/details/gyoyrttnc.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.tarul.cn/Article/details/gwppmdnfb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.bbcook.cn/Article/details/gxdiziprq.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.tarul.cn/Article/details/ghivzdjsi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/gqgysqnzg.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.sjlbkw.cn/Article/details/gmwbhmcdo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fktsv.cn/Article/details/glcvzkwic.sHtML

[U85] JS：可选链
来源：http://www.blog.vehdjk.com/Article/details/gyrivfsxt.sHtML

a?.b?.c
来源：http://m.share.fktsv.cn/Article/details/gmhjsgvcd.sHtML

[U86] JS：空值合并
来源：http://www.blog.epnwcf.com/Article/details/ggpidinni.sHtML

a ?? b
来源：http://www.m.share.vehdjk.com/Article/details/gzvcecuur.sHtML

[U87] JS：解构默认值
来源：http://www.share.vehdjk.com/Article/details/ghkyyytme.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.epnwcf.com/Article/details/gctjtuoqs.sHtML

[U88] JS：对象展开合并
来源：http://wap.yfazqb.com/Article/details/gxhnsocln.sHtML

{ ...a, ...b }
来源：http://wap.epnwcf.com/Article/details/gvrxartyy.sHtML

[U89] JS：数组去重
来源：http://www.m.share.bbcook.cn/Article/details/gbqspwwqb.sHtML

[...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gqnsxyaeb.sHtML

[U90] JS：数字数组排序
来源：http://baike.sjlbkw.cn/Article/details/gmzovsufj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gzfboabev.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.epnwcf.com/Article/details/gtercxqhl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fktsv.cn/Article/details/gtqitexkz.sHtML

[U92] JS：深拷贝
来源：http://baike.sjlbkw.cn/Article/details/gsqoribvy.sHtML

structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gpmjinwog.sHtML

[U93] JS：模板字符串
来源：http://www.blog.tarul.cn/Article/details/gsusnwbly.sHtML

`共 ${n} 条`
来源：http://read.share.bbcook.cn/Article/details/gzlmqpquy.sHtML

[U94] JS：箭头函数
来源：http://read.share.sjlbkw.cn/Article/details/gstvbaglp.sHtML

const double = x => x * 2;
来源：http://www.blog.vehdjk.com/Article/details/gismpzwpy.sHtML

[U95] JS：Promise 包装
来源：http://www.share.tarul.cn/Article/details/gxzbydyiy.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.epnwcf.com/Article/details/gbzzyrjld.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.sjlbkw.cn/Article/details/gtdsttkzm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gtwdpmmav.sHtML

[U97] JS：并发请求
来源：http://www.blog.yfazqb.com/Article/details/gqmpbnbyc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gjqxrghyr.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.bbcook.cn/Article/details/gvfnpxvxd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fktsv.cn/Article/details/gmvzloaed.sHtML

[U99] JS：事件监听
来源：http://www.blog.epnwcf.com/Article/details/gpksgilnq.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fktsv.cn/Article/details/gvtihkupr.sHtML

[U100] JS：DOM 查询
来源：http://baike.vehdjk.com/Article/details/gxztmxjbp.sHtML

document.querySelector(".item")
来源：http://www.m.share.bbcook.cn/Article/details/gpvscwczh.sHtML

[U101] JS：classList 操作
来源：http://www.blog.vehdjk.com/Article/details/gfytrexdc.sHtML

el.classList.toggle("active")
来源：http://baike.fktsv.cn/Article/details/gnpikhjre.sHtML

[U102] JS：本地存储
来源：http://blog.fktsv.cn/Article/details/giulhhqkj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.tarul.cn/Article/details/gbzhmbokr.sHtML

[U103] JS：定时器
来源：http://www.m.share.tarul.cn/Article/details/gchlhqlqk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.bbcook.cn/Article/details/ggbgmcehq.sHtML

[U104] JS：防抖
来源：http://www.blog.yfazqb.com/Article/details/gzgcikenz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/ghosuthsd.sHtML

[U105] JS：节流
来源：http://3g.yfazqb.com/Article/details/gmfggelbq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.vehdjk.com/Article/details/gmvjpzwyz.sHtML

[U106] JS：日期格式化
来源：http://3g.fktsv.cn/Article/details/gvqgcqdzj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.yfazqb.com/Article/details/guoishpoy.sHtML

[U107] JS：数字千分位
来源：http://blog.fktsv.cn/Article/details/gelnmmxqt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.epnwcf.com/Article/details/gatrlflbp.sHtML

[U108] JS：随机整数
来源：http://m.share.bbcook.cn/Article/details/gdwbyhmvz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.yfazqb.com/Article/details/gvyyfrakg.sHtML

[U109] JS：数组分组
来源：http://www.blog.vehdjk.com/Article/details/gvgqcvtzk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/gbniyfuej.sHtML

[U110] JS：数组分块
来源：http://www.share.vehdjk.com/Article/details/gzswarapw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.yfazqb.com/Article/details/grbrtqztv.sHtML

[U111] JS：对象转 Map
来源：http://3g.fktsv.cn/Article/details/gnluddlap.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.yfazqb.com/Article/details/gwfyscqse.sHtML

[U112] JS：字符串补位
来源：http://3g.sjlbkw.cn/Article/details/gezaahhiv.sHtML

"7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gtoqbinky.sHtML

[U113] JS：正则替换全部
来源：http://3g.sjlbkw.cn/Article/details/gcpkqnhlv.sHtML

s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gzkahdwzt.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gluklfryt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gzrdnnioz.sHtML

[U115] JS：生成 UUID
来源：http://blog.epnwcf.com/Article/details/gktjpbvzi.sHtML

crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gufqgsrwl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.tarul.cn/Article/details/gpbgscvlw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gtovvhyol.sHtML

[U117] JS：单元测试
来源：http://wap.tarul.cn/Article/details/gsmotuqkb.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.tarul.cn/Article/details/gvcooavok.sHtML

[U118] JS：开发服务器
来源：http://3g.vehdjk.com/Article/details/grbeomiau.sHtML

npm i -D vite;  npx vite
来源：http://wap.fktsv.cn/Article/details/gnvfeouxb.sHtML

[U119] JS：生产构建
来源：http://read.share.epnwcf.com/Article/details/gmdtbanpw.sHtML

npx vite build
来源：http://read.share.yfazqb.com/Article/details/gdkqdihbl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.tarul.cn/Article/details/gdiowectc.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fktsv.cn/Article/details/gulqzmsmt.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gsrhniowi.sHtML

统计汇总
来源：http://m.share.sjlbkw.cn/Article/details/goyqdbibm.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gzqnfvpst.sHtML

按语言统计（条）：
来源：http://www.share.bbcook.cn/Article/details/gykgnbzww.sHtML

Python ......... 252
来源：http://www.m.share.yfazqb.com/Article/details/gtguqrodd.sHtML

PHP ............ 252
来源：http://www.blog.fktsv.cn/Article/details/giighgnzf.sHtML

JavaScript ..... 252
来源：http://www.m.share.epnwcf.com/Article/details/gpzkhtmcr.sHtML

TypeScript ..... 212
来源：http://blog.tarul.cn/Article/details/gkbhhiozr.sHtML

Java ........... 212
来源：http://wap.tarul.cn/Article/details/guauwkwzc.sHtML

Go ............. 212
来源：http://mobile.vehdjk.com/Article/details/gkuxmzxhh.sHtML

Ruby ........... 212
来源：http://m.share.vehdjk.com/Article/details/gekkszclo.sHtML

C# ............. 212
来源：http://m.share.sjlbkw.cn/Article/details/gjiuljtth.sHtML

C .............. 30
来源：http://www.m.share.vehdjk.com/Article/details/gxuouyjvb.sHtML

C++ ............ 30
来源：http://read.share.epnwcf.com/Article/details/gnliqykcd.sHtML

SQL ............ 90
来源：http://blog.sjlbkw.cn/Article/details/ggvyrurnd.sHtML

Bash ........... 80
来源：http://baike.sjlbkw.cn/Article/details/gfcylikef.sHtML

Kotlin ......... 15
来源：http://www.share.tarul.cn/Article/details/grailpnnn.sHtML

Swift .......... 15
来源：http://www.m.share.vehdjk.com/Article/details/geigxpvvj.sHtML

Lua ............ 10
来源：http://www.blog.sjlbkw.cn/Article/details/gmgprnxzv.sHtML

Perl ........... 10
来源：http://read.share.fktsv.cn/Article/details/ghmxeaqem.sHtML

Scala .......... 10
来源：http://www.share.bbcook.cn/Article/details/gcpmgqmvt.sHtML

------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gfbpvbedx.sHtML

合计 ........... 2106 条
来源：http://wap.sjlbkw.cn/Article/details/gakezgrsc.sHtML

按章节统计：
来源：http://www.share.yfazqb.com/Article/details/glntrbqwo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/ghqmgsqxw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/gmgokdwmz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/gcxnowogg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.epnwcf.com/Article/details/gyeigcuxr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fktsv.cn/Article/details/gmpdiqwoz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.epnwcf.com/Article/details/gquitxyli.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/ghumrrdbq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fktsv.cn/Article/details/gncwjiqhx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gojxkgthx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.vehdjk.com/Article/details/gmnywjgib.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gnedozdym.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmsdykjg.sHtML


<!-- 参考信息 -->