代发 wailian999

[T47] Perl：正则捕获
来源：http://mobile.epnwcf.com/Article/details/guyjxrifx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.yfazqb.com/Article/details/gnrkghces.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/gjtxlnzut.sHtML

$s =~ s/old/new/g;
来源：http://m.share.epnwcf.com/Article/details/gaoybarqu.sHtML

[T49] Perl：函数
来源：http://mobile.bbcook.cn/Article/details/gfzchvurm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/glmtaocvp.sHtML

[T50] Perl：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gzfjujqai.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.vehdjk.com/Article/details/gfdkeyejo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.tarul.cn/Article/details/gfqmelepa.sHtML

[T51] Scala：Hello World
来源：http://m.share.yfazqb.com/Article/details/gsbrbmesv.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gruargzke.sHtML

[T52] Scala：变量
来源：http://read.share.yfazqb.com/Article/details/guikfoxem.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.tarul.cn/Article/details/gdoxngiyz.sHtML

[T53] Scala：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gyphcvuor.sHtML

s"值: $b"
来源：http://read.share.yfazqb.com/Article/details/gzrutvslt.sHtML

[T54] Scala：集合映射
来源：http://blog.tarul.cn/Article/details/gsmdfnaaz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.epnwcf.com/Article/details/gpztjsiqy.sHtML

[T55] Scala：集合过滤
来源：http://wap.yfazqb.com/Article/details/gwjpeizab.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.bbcook.cn/Article/details/grnltadhd.sHtML

[T56] Scala：样例类
来源：http://3g.vehdjk.com/Article/details/gicxjykqe.sHtML

case class User(name: String, age: Int)
来源：http://read.share.tarul.cn/Article/details/gtpfnhygj.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/glpjvnyai.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.bbcook.cn/Article/details/guggnyxby.sHtML

[T58] Scala：函数定义
来源：http://blog.yfazqb.com/Article/details/gckluoqow.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.epnwcf.com/Article/details/ghadzqqdc.sHtML

[T59] Scala：循环
来源：http://read.share.fktsv.cn/Article/details/gvsmogncw.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/gdhelytvt.sHtML

[T60] Scala：折叠
来源：http://read.share.epnwcf.com/Article/details/gfqkxtael.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fktsv.cn/Article/details/gvufeybxa.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gvtvbhgih.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/gchdndinn.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggpsjoyuo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.yfazqb.com/Article/details/gwmpicbod.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.sjlbkw.cn/Article/details/gsxydndux.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.bbcook.cn/Article/details/gozzadcxa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.vehdjk.com/Article/details/gvevbyzqp.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.sjlbkw.cn/Article/details/gvssztkrb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fktsv.cn/Article/details/ghuvrllrr.sHtML

[U04] Py：变量调试打印
来源：http://wap.tarul.cn/Article/details/glqvqkfdn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.tarul.cn/Article/details/gkjxocdtv.sHtML

[U05] Py：列表去重且保序
来源：http://3g.epnwcf.com/Article/details/gtmwarsih.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gozfydioy.sHtML

[U06] Py：合并两个字典
来源：http://blog.vehdjk.com/Article/details/gpxbgimjn.sHtML

{**a, **b}
来源：http://wap.bbcook.cn/Article/details/gpsfykjkf.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fktsv.cn/Article/details/ghmuerlda.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.vehdjk.com/Article/details/gomxgcran.sHtML

[U08] Py：展平二维列表
来源：http://blog.vehdjk.com/Article/details/gfxkxjuof.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.epnwcf.com/Article/details/gessrvwpo.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.epnwcf.com/Article/details/gvpunggpc.sHtML

max(d, key=d.get)
来源：http://wap.epnwcf.com/Article/details/gygpkqjbo.sHtML

[U10] Py：按值排序字典
来源：http://3g.yfazqb.com/Article/details/gdqfuvyqs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.tarul.cn/Article/details/gmbhesome.sHtML

[U11] Py：生成器表达式
来源：http://m.share.sjlbkw.cn/Article/details/gnvotfzna.sHtML

(x * 2 for x in arr)
来源：http://www.blog.tarul.cn/Article/details/guuairylp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.vehdjk.com/Article/details/gaunuoapg.sHtML

Counter(arr).most_common(3)
来源：http://blog.yfazqb.com/Article/details/gnedtnsbg.sHtML

[U13] Py：固定长度队列
来源：http://m.share.yfazqb.com/Article/details/goyodfmgw.sHtML

deque(maxlen=10)
来源：http://www.share.fktsv.cn/Article/details/gqixvqjfg.sHtML

[U14] Py：分组收集到列表
来源：http://baike.bbcook.cn/Article/details/glbbyyryq.sHtML

defaultdict(list)
来源：http://www.blog.vehdjk.com/Article/details/gzzheggzn.sHtML

[U15] Py：高精度计时
来源：http://www.share.fktsv.cn/Article/details/grysvhezk.sHtML

t = time.perf_counter()
来源：http://3g.sjlbkw.cn/Article/details/gzzljefrj.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.tarul.cn/Article/details/gikbkenbn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.sjlbkw.cn/Article/details/ggqdufsfb.sHtML

[U17] Py：初始化日志
来源：http://read.share.yfazqb.com/Article/details/gllmiyzlf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.yfazqb.com/Article/details/gnugrptpg.sHtML

[U18] Py：预编译正则
来源：http://m.share.sjlbkw.cn/Article/details/gwxgkwrbp.sHtML

pat = re.compile(r"\d+")
来源：http://wap.tarul.cn/Article/details/gmpywxuhx.sHtML

[U19] Py：正则替换带回调
来源：http://baike.bbcook.cn/Article/details/gfsqcrgpy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.yfazqb.com/Article/details/gtcypigjs.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fktsv.cn/Article/details/grbkgbduu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fktsv.cn/Article/details/grwoaoxps.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.yfazqb.com/Article/details/gymugtirl.sHtML

@contextlib.contextmanager
来源：http://www.share.sjlbkw.cn/Article/details/gchineplt.sHtML

[U22] Py：矩阵转置
来源：http://baike.yfazqb.com/Article/details/gieedmxzz.sHtML

list(zip(*m))
来源：http://read.share.yfazqb.com/Article/details/grdwgcklq.sHtML

[U23] Py：分块读取大文件
来源：http://wap.sjlbkw.cn/Article/details/gfnezcthq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fktsv.cn/Article/details/gozbptkxt.sHtML

[U24] Py：路径操作
来源：http://blog.epnwcf.com/Article/details/gmyvcyhuo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.yfazqb.com/Article/details/gicaskmrr.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.bbcook.cn/Article/details/gzfuwtbvz.sHtML

csv.DictReader(f)
来源：http://3g.yfazqb.com/Article/details/gwptgirrf.sHtML

[U26] Py：并发下载
来源：http://blog.vehdjk.com/Article/details/ggblviyfl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.sjlbkw.cn/Article/details/gmydpjrfr.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.epnwcf.com/Article/details/gdegfnhwz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.epnwcf.com/Article/details/gvqsvxwlo.sHtML

[U28] Py：类型别名
来源：http://mobile.epnwcf.com/Article/details/ggzlybufx.sHtML

UserId = int
来源：http://3g.bbcook.cn/Article/details/gjxvshpwv.sHtML

[U29] Py：属性校验
来源：http://read.share.bbcook.cn/Article/details/gecixalqz.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.vehdjk.com/Article/details/glaebanai.sHtML

[U30] Py：数据类
来源：http://blog.bbcook.cn/Article/details/govaowglx.sHtML

@dataclass(slots=True)
来源：http://wap.yfazqb.com/Article/details/gxlkfxhqe.sHtML

[U31] Py：单测
来源：http://read.share.tarul.cn/Article/details/gowgefrhh.sHtML

python -m pytest -q
来源：http://baike.fktsv.cn/Article/details/gnvnvsqea.sHtML

[U32] Py：代码格式化
来源：http://blog.epnwcf.com/Article/details/gkdrkmoiy.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbfjitrv.sHtML

[U33] Py：打包发布
来源：http://wap.vehdjk.com/Article/details/goumqrdmu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.sjlbkw.cn/Article/details/galpwmymn.sHtML

[U34] Py：判断编码
来源：http://baike.sjlbkw.cn/Article/details/gsaksslmw.sHtML

chardet.detect(raw)
来源：http://baike.epnwcf.com/Article/details/gdilzbwrk.sHtML

[U35] Py：发送邮件
来源：http://blog.tarul.cn/Article/details/gwotayjrw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.vehdjk.com/Article/details/ghxqgmjbe.sHtML

[U36] Py：定时任务
来源：http://m.share.vehdjk.com/Article/details/gqxzzkddt.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.sjlbkw.cn/Article/details/gzffqtatg.sHtML

[U37] Py：读写 Excel
来源：http://mobile.bbcook.cn/Article/details/gpqofzhgk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.epnwcf.com/Article/details/gwtvodpuu.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.epnwcf.com/Article/details/geppdypiq.sHtML

Path(__file__).resolve().parent
来源：http://wap.yfazqb.com/Article/details/gyfujwvlo.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.tarul.cn/Article/details/gttpskbzg.sHtML

sys.stdout.isatty()
来源：http://wap.fktsv.cn/Article/details/gaohpxisk.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fktsv.cn/Article/details/goxuqpyzd.sHtML

print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/gahoueaeg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.yfazqb.com/Article/details/glgdzsody.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.epnwcf.com/Article/details/glyzcgopf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fktsv.cn/Article/details/ghyjqbuxz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.sjlbkw.cn/Article/details/grlrelooy.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.yfazqb.com/Article/details/grnvscjhk.sHtML

namespace App\Http;
来源：http://mobile.sjlbkw.cn/Article/details/gtjmlbvjt.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.vehdjk.com/Article/details/gxbejenfm.sHtML

declare(strict_types=1);
来源：http://baike.epnwcf.com/Article/details/gipfxkdlz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.epnwcf.com/Article/details/geelkuacp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gtwqnrihm.sHtML

[U46] PHP：可空类型
来源：http://www.blog.tarul.cn/Article/details/gjgphxiej.sHtML

?string $name = null
来源：http://blog.epnwcf.com/Article/details/gtinuihrl.sHtML

[U47] PHP：联合类型
来源：http://www.blog.sjlbkw.cn/Article/details/gxtwhmppd.sHtML

int|string $id
来源：http://3g.bbcook.cn/Article/details/grmzjrzip.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.vehdjk.com/Article/details/gqphjqgfz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.tarul.cn/Article/details/gilpnxyig.sHtML

[U49] PHP：只读属性
来源：http://blog.sjlbkw.cn/Article/details/goetrdsnj.sHtML

public readonly string $name
来源：http://www.m.share.bbcook.cn/Article/details/gtawfaokm.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.vehdjk.com/Article/details/gptnzxswc.sHtML

public function __construct(private int $id) {}
来源：http://3g.tarul.cn/Article/details/gwmmpluag.sHtML

[U51] PHP：数组解构
来源：http://read.share.tarul.cn/Article/details/gccfkvndb.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkabsynb.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gcoarcoff.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fktsv.cn/Article/details/glddgvgua.sHtML

[U53] PHP：空合并运算符
来源：http://blog.epnwcf.com/Article/details/gxhbastci.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.epnwcf.com/Article/details/gqkymmucg.sHtML

[U54] PHP：空安全调用
来源：http://read.share.yfazqb.com/Article/details/gqoprditm.sHtML

$obj?->method()
来源：http://wap.fktsv.cn/Article/details/glogfzjqd.sHtML

[U55] PHP：match 表达式
来源：http://3g.bbcook.cn/Article/details/gtufvykfw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.yfazqb.com/Article/details/gnstflpgk.sHtML

[U56] PHP：命名参数
来源：http://blog.tarul.cn/Article/details/gbmmzzjwj.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gguulmzni.sHtML

[U57] PHP：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gpkengfrx.sHtML

"值: {$a}"
来源：http://3g.epnwcf.com/Article/details/gdcuakwxn.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.vehdjk.com/Article/details/gatqvdsxc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.sjlbkw.cn/Article/details/gdulzgkqm.sHtML

[U59] PHP：自定义排序
来源：http://read.share.epnwcf.com/Article/details/gzbggxwpi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.yfazqb.com/Article/details/gojbklxeq.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fktsv.cn/Article/details/gpolujdqc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fktsv.cn/Article/details/gjknoidnt.sHtML

[U61] PHP：正则
来源：http://www.m.share.bbcook.cn/Article/details/gzilekdrw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/gcvgtxvxr.sHtML

[U62] PHP：日期对象
来源：http://mobile.tarul.cn/Article/details/gclwiwspi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.bbcook.cn/Article/details/gztwaisel.sHtML

[U63] PHP：文件读写
来源：http://blog.vehdjk.com/Article/details/goxrkobzo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fktsv.cn/Article/details/gfqrvqhkk.sHtML

[U64] PHP：目录遍历
来源：http://blog.yfazqb.com/Article/details/gaqowatjz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.vehdjk.com/Article/details/gvdtowbnz.sHtML

[U65] PHP：会话
来源：http://read.share.yfazqb.com/Article/details/ghexgoush.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gxovedodt.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.vehdjk.com/Article/details/ghsjaihhw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.epnwcf.com/Article/details/gvylhmwaa.sHtML

[U67] PHP：处理文件上传
来源：http://wap.sjlbkw.cn/Article/details/gdzxmymbr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.epnwcf.com/Article/details/ghveprxgs.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.bbcook.cn/Article/details/gbgffdmrh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.sjlbkw.cn/Article/details/gnevgoqly.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.yfazqb.com/Article/details/gsxwrpfay.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.vehdjk.com/Article/details/gubwavcys.sHtML

[U70] PHP：PDO 事务
来源：http://3g.epnwcf.com/Article/details/gnshoecmw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.sjlbkw.cn/Article/details/glxntvruz.sHtML

[U71] PHP：抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gcnrgibca.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.vehdjk.com/Article/details/gkimnewya.sHtML

[U72] PHP：写错误日志
来源：http://www.share.bbcook.cn/Article/details/gfoimwqya.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.bbcook.cn/Article/details/glkvhqrle.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.vehdjk.com/Article/details/gmdbtknsr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.tarul.cn/Article/details/grhiayzrl.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.tarul.cn/Article/details/glvqhbyyt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.vehdjk.com/Article/details/gakycridu.sHtML

[U75] PHP：依赖注入
来源：http://wap.tarul.cn/Article/details/gleswlboy.sHtML

composer require psr/container
来源：http://www.m.share.yfazqb.com/Article/details/gpkivbkad.sHtML

[U76] PHP：简单路由
来源：http://www.blog.bbcook.cn/Article/details/gfjeybawy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.vehdjk.com/Article/details/gusmprxuv.sHtML

[U77] PHP：模板渲染
来源：http://www.share.yfazqb.com/Article/details/gqkvkbmyi.sHtML

composer require twig/twig
来源：http://www.share.sjlbkw.cn/Article/details/gcaqrzarx.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gsmtwskup.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.bbcook.cn/Article/details/gsbhcmjdb.sHtML

[U79] PHP：静态分析
来源：http://mobile.tarul.cn/Article/details/gfcyrojxa.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.yfazqb.com/Article/details/glynzbxah.sHtML

[U80] PHP：代码规范修复
来源：http://wap.vehdjk.com/Article/details/glzgacvwq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.bbcook.cn/Article/details/gmgdlsngd.sHtML

[U81] JS：初始化项目
来源：http://baike.tarul.cn/Article/details/gvvydsdth.sHtML

npm init -y;  npm i express
来源：http://baike.bbcook.cn/Article/details/gbvtuspcb.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.vehdjk.com/Article/details/gcymycbgj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.vehdjk.com/Article/details/gegnukuff.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.bbcook.cn/Article/details/gjcdlimwb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.yfazqb.com/Article/details/gwkdazqdj.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.sjlbkw.cn/Article/details/gwubqjunq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.tarul.cn/Article/details/gucoxitos.sHtML

[U85] JS：可选链
来源：http://wap.fktsv.cn/Article/details/gnehltedh.sHtML

a?.b?.c
来源：http://www.blog.yfazqb.com/Article/details/gynpqsncy.sHtML

[U86] JS：空值合并
来源：http://www.blog.bbcook.cn/Article/details/gaxedubzq.sHtML

a ?? b
来源：http://www.m.share.yfazqb.com/Article/details/gglbknjmi.sHtML

[U87] JS：解构默认值
来源：http://baike.bbcook.cn/Article/details/gmkjxwjgd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.tarul.cn/Article/details/gonsrljxq.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fktsv.cn/Article/details/gbtkiiyli.sHtML

{ ...a, ...b }
来源：http://wap.epnwcf.com/Article/details/gkexlnvjp.sHtML

[U89] JS：数组去重
来源：http://wap.vehdjk.com/Article/details/glcrmghgr.sHtML

[...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gwdleatsf.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.tarul.cn/Article/details/gxopxyofu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gsxgpseji.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.vehdjk.com/Article/details/gnlaoahxo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.sjlbkw.cn/Article/details/gohdpstgt.sHtML

[U92] JS：深拷贝
来源：http://wap.epnwcf.com/Article/details/gyygpeatj.sHtML

structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gtzyhsdbo.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.vehdjk.com/Article/details/gxtnyocjb.sHtML

`共 ${n} 条`
来源：http://www.m.share.tarul.cn/Article/details/gclfmliuo.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/gwpfjhzxx.sHtML

const double = x => x * 2;
来源：http://baike.bbcook.cn/Article/details/gggpvngnh.sHtML

[U95] JS：Promise 包装
来源：http://blog.tarul.cn/Article/details/golsvtpop.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.yfazqb.com/Article/details/gtetiwytd.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.yfazqb.com/Article/details/gyuyboxxs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gxmszcvdw.sHtML

[U97] JS：并发请求
来源：http://3g.yfazqb.com/Article/details/gnuvaifnr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gjpparsno.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.epnwcf.com/Article/details/gpgisnzqf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.yfazqb.com/Article/details/gshklrbgo.sHtML

[U99] JS：事件监听
来源：http://www.blog.bbcook.cn/Article/details/gxsevvpuw.sHtML

el.addEventListener("click", e => {})
来源：http://baike.vehdjk.com/Article/details/gdhcdmndy.sHtML

[U100] JS：DOM 查询
来源：http://wap.yfazqb.com/Article/details/gpcwdrqml.sHtML

document.querySelector(".item")
来源：http://www.m.share.yfazqb.com/Article/details/gyabnagjb.sHtML

[U101] JS：classList 操作
来源：http://mobile.sjlbkw.cn/Article/details/gurkhnfmi.sHtML

el.classList.toggle("active")
来源：http://wap.vehdjk.com/Article/details/gpisvilgx.sHtML

[U102] JS：本地存储
来源：http://baike.yfazqb.com/Article/details/guftxuwpk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.bbcook.cn/Article/details/gicxgziep.sHtML

[U103] JS：定时器
来源：http://www.blog.vehdjk.com/Article/details/gwjwovtfw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.sjlbkw.cn/Article/details/geegpmgjg.sHtML

[U104] JS：防抖
来源：http://www.blog.vehdjk.com/Article/details/gimutbfjn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gfcctvmbp.sHtML

[U105] JS：节流
来源：http://baike.vehdjk.com/Article/details/gunbcmdnc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.bbcook.cn/Article/details/glieevyfj.sHtML

[U106] JS：日期格式化
来源：http://www.share.fktsv.cn/Article/details/gsnkafeqt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.bbcook.cn/Article/details/gctqozqyk.sHtML

[U107] JS：数字千分位
来源：http://3g.bbcook.cn/Article/details/gdnxbhydo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gtigqqjgg.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gfebhcgbe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.bbcook.cn/Article/details/gjcoaslby.sHtML

[U109] JS：数组分组
来源：http://m.share.bbcook.cn/Article/details/gxmpziodq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/gqkjpubfm.sHtML

[U110] JS：数组分块
来源：http://www.m.share.vehdjk.com/Article/details/gtiqbozak.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.yfazqb.com/Article/details/gzbyxqzcg.sHtML

[U111] JS：对象转 Map
来源：http://3g.tarul.cn/Article/details/gcphrxcma.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.bbcook.cn/Article/details/ghidouoan.sHtML

[U112] JS：字符串补位
来源：http://mobile.sjlbkw.cn/Article/details/gnkbpeyxp.sHtML

"7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gnhfaqvhm.sHtML

[U113] JS：正则替换全部
来源：http://m.share.bbcook.cn/Article/details/gseftwanu.sHtML

s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gqygyyexu.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.bbcook.cn/Article/details/gvlndneko.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/guvjjokid.sHtML

[U115] JS：生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gdmttcrgw.sHtML

crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gydcirmtw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.tarul.cn/Article/details/gqtjabljw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.tarul.cn/Article/details/gdelrgxof.sHtML

[U117] JS：单元测试
来源：http://www.share.yfazqb.com/Article/details/gpxrmgfth.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.epnwcf.com/Article/details/gidhkqvpe.sHtML

[U118] JS：开发服务器
来源：http://blog.epnwcf.com/Article/details/gqqmebjpu.sHtML

npm i -D vite;  npx vite
来源：http://3g.bbcook.cn/Article/details/gbuhipepo.sHtML

[U119] JS：生产构建
来源：http://www.share.sjlbkw.cn/Article/details/gtfquvqpr.sHtML

npx vite build
来源：http://www.blog.vehdjk.com/Article/details/gvtahznue.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.tarul.cn/Article/details/gidvllnyr.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.bbcook.cn/Article/details/gxyraldhx.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gfdnxegzc.sHtML

统计汇总
来源：http://m.share.tarul.cn/Article/details/grvfewozs.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxfmgdfvv.sHtML

按语言统计（条）：
来源：http://www.m.share.sjlbkw.cn/Article/details/gitsnvbkz.sHtML

Python ......... 252
来源：http://3g.tarul.cn/Article/details/gfushslod.sHtML

PHP ............ 252
来源：http://www.blog.vehdjk.com/Article/details/govwqyqwo.sHtML

JavaScript ..... 252
来源：http://3g.fktsv.cn/Article/details/gxcibeivf.sHtML

TypeScript ..... 212
来源：http://baike.fktsv.cn/Article/details/gqvoxkynh.sHtML

Java ........... 212
来源：http://www.share.yfazqb.com/Article/details/gducizaji.sHtML

Go ............. 212
来源：http://mobile.epnwcf.com/Article/details/gqawnbxvp.sHtML

Ruby ........... 212
来源：http://mobile.epnwcf.com/Article/details/gdetpnbsn.sHtML

C# ............. 212
来源：http://wap.epnwcf.com/Article/details/gvcszdyyq.sHtML

C .............. 30
来源：http://read.share.epnwcf.com/Article/details/gghkgefhn.sHtML

C++ ............ 30
来源：http://blog.sjlbkw.cn/Article/details/gjxmipiqk.sHtML

SQL ............ 90
来源：http://baike.sjlbkw.cn/Article/details/gatqcejyc.sHtML

Bash ........... 80
来源：http://www.m.share.yfazqb.com/Article/details/gkgslsrji.sHtML

Kotlin ......... 15
来源：http://www.share.sjlbkw.cn/Article/details/gxrkmzxio.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/guhsjbydh.sHtML

Lua ............ 10
来源：http://blog.vehdjk.com/Article/details/gcqcnrbfs.sHtML

Perl ........... 10
来源：http://baike.vehdjk.com/Article/details/gtxlbdxif.sHtML

Scala .......... 10
来源：http://www.m.share.yfazqb.com/Article/details/gchzahflw.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/gwbjyujrd.sHtML

合计 ........... 2106 条
来源：http://m.share.vehdjk.com/Article/details/ggiduecda.sHtML

按章节统计：
来源：http://www.blog.bbcook.cn/Article/details/grabyiuzl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.bbcook.cn/Article/details/gqdpqikjk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gepggtlss.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gwrhtytef.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.vehdjk.com/Article/details/gphpbnxin.sHtML


<!-- 参考信息 -->