代发 wailian999

[T47] Perl：正则捕获
来源：http://mobile.vehdjk.com/Article/details/gzujvquym.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.sjlbkw.cn/Article/details/gexzxvjde.sHtML

[T48] Perl：正则替换
来源：http://www.blog.yfazqb.com/Article/details/gjownltpq.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fktsv.cn/Article/details/gcmxbrejb.sHtML

[T49] Perl：函数
来源：http://wap.epnwcf.com/Article/details/gidmjluuv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/guvfeidmn.sHtML

[T50] Perl：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gciugyzax.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.epnwcf.com/Article/details/gzfuyxcbt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fktsv.cn/Article/details/gwxwwtfuu.sHtML

[T51] Scala：Hello World
来源：http://3g.fktsv.cn/Article/details/gtscsolbl.sHtML

println("Hello")
来源：http://wap.vehdjk.com/Article/details/goswqpgrk.sHtML

[T52] Scala：变量
来源：http://m.share.vehdjk.com/Article/details/gjjplkylt.sHtML

val a = 1;  var b = 2
来源：http://mobile.epnwcf.com/Article/details/geqludepd.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gipyoybby.sHtML

s"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gjxekrdxv.sHtML

[T54] Scala：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gkhddjslw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.vehdjk.com/Article/details/gkpjlsndq.sHtML

[T55] Scala：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gqaxgvrcd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.yfazqb.com/Article/details/gvlqgexgl.sHtML

[T56] Scala：样例类
来源：http://baike.yfazqb.com/Article/details/gqccnlfjd.sHtML

case class User(name: String, age: Int)
来源：http://m.share.vehdjk.com/Article/details/gdcozyako.sHtML

[T57] Scala：模式匹配
来源：http://read.share.sjlbkw.cn/Article/details/gxkjygjyk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.epnwcf.com/Article/details/gbjaeosxq.sHtML

[T58] Scala：函数定义
来源：http://baike.yfazqb.com/Article/details/gdvfftxej.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.yfazqb.com/Article/details/gayilvlon.sHtML

[T59] Scala：循环
来源：http://read.share.sjlbkw.cn/Article/details/guvixvmgl.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fktsv.cn/Article/details/glvamntks.sHtML

[T60] Scala：折叠
来源：http://read.share.sjlbkw.cn/Article/details/gmajnvdnk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/geeoktfsz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqempzzpv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/gbehfswsu.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gsqwznfoz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.tarul.cn/Article/details/geepqttvy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.sjlbkw.cn/Article/details/grjdmrknm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.tarul.cn/Article/details/glrwvsfbh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/gwizccpov.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.bbcook.cn/Article/details/gkvwhczkf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.vehdjk.com/Article/details/gnyqngzss.sHtML

[U04] Py：变量调试打印
来源：http://read.share.sjlbkw.cn/Article/details/gprgwhxem.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.vehdjk.com/Article/details/gncuirfue.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fktsv.cn/Article/details/gdxchdycn.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gzaxhmxkn.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.epnwcf.com/Article/details/gpqmbqekd.sHtML

{**a, **b}
来源：http://m.share.fktsv.cn/Article/details/glaahmihc.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.bbcook.cn/Article/details/ghtdlziir.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.vehdjk.com/Article/details/gkuhgqqoj.sHtML

[U08] Py：展平二维列表
来源：http://wap.bbcook.cn/Article/details/gktgulwjf.sHtML

[y for x in nested for y in x]
来源：http://wap.vehdjk.com/Article/details/goohdycui.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fktsv.cn/Article/details/gfiuonxns.sHtML

max(d, key=d.get)
来源：http://m.share.fktsv.cn/Article/details/goqbnlhki.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fktsv.cn/Article/details/gqwmnnobe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.yfazqb.com/Article/details/gifaynsyp.sHtML

[U11] Py：生成器表达式
来源：http://wap.epnwcf.com/Article/details/ggewvpoov.sHtML

(x * 2 for x in arr)
来源：http://www.share.yfazqb.com/Article/details/gbzncmznq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.yfazqb.com/Article/details/gedsvzppb.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/ggcmorfcg.sHtML

[U13] Py：固定长度队列
来源：http://3g.yfazqb.com/Article/details/gopmcinom.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/gfkgoorpg.sHtML

[U14] Py：分组收集到列表
来源：http://baike.sjlbkw.cn/Article/details/gnikwzcnc.sHtML

defaultdict(list)
来源：http://3g.vehdjk.com/Article/details/gppmjthin.sHtML

[U15] Py：高精度计时
来源：http://wap.tarul.cn/Article/details/gzyyhloqp.sHtML

t = time.perf_counter()
来源：http://www.blog.tarul.cn/Article/details/gbbmcokzm.sHtML

[U16] Py：命令行参数解析
来源：http://wap.vehdjk.com/Article/details/gnqxkzkat.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fktsv.cn/Article/details/gasnloeak.sHtML

[U17] Py：初始化日志
来源：http://read.share.tarul.cn/Article/details/gaqgdgghk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.yfazqb.com/Article/details/gmmwczarx.sHtML

[U18] Py：预编译正则
来源：http://m.share.vehdjk.com/Article/details/gwvfqxbfg.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gxcojprec.sHtML

[U19] Py：正则替换带回调
来源：http://3g.bbcook.cn/Article/details/ghbixsupd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.epnwcf.com/Article/details/ggdalkjzy.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.bbcook.cn/Article/details/ggfnnabpk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fktsv.cn/Article/details/gbtcfbmao.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.epnwcf.com/Article/details/gkhhqrkmr.sHtML

@contextlib.contextmanager
来源：http://blog.tarul.cn/Article/details/gzuclqgod.sHtML

[U22] Py：矩阵转置
来源：http://mobile.sjlbkw.cn/Article/details/gfewodpmy.sHtML

list(zip(*m))
来源：http://www.share.yfazqb.com/Article/details/gflitcnmb.sHtML

[U23] Py：分块读取大文件
来源：http://blog.tarul.cn/Article/details/gabgukyyo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fktsv.cn/Article/details/ggbfatbzj.sHtML

[U24] Py：路径操作
来源：http://baike.yfazqb.com/Article/details/gqncpiesm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.tarul.cn/Article/details/gvpquuniv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.epnwcf.com/Article/details/gliikdjhr.sHtML

csv.DictReader(f)
来源：http://www.blog.sjlbkw.cn/Article/details/ggdlxrewd.sHtML

[U26] Py：并发下载
来源：http://blog.tarul.cn/Article/details/gajsozuda.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.vehdjk.com/Article/details/gypyxmitz.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.yfazqb.com/Article/details/gvmkygveg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.tarul.cn/Article/details/gyzutkdug.sHtML

[U28] Py：类型别名
来源：http://www.share.yfazqb.com/Article/details/gwndyrvrm.sHtML

UserId = int
来源：http://blog.yfazqb.com/Article/details/gxiqtjecs.sHtML

[U29] Py：属性校验
来源：http://wap.fktsv.cn/Article/details/gagnxbykq.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.vehdjk.com/Article/details/guirflqkd.sHtML

[U30] Py：数据类
来源：http://3g.yfazqb.com/Article/details/gxpcrwlxa.sHtML

@dataclass(slots=True)
来源：http://www.m.share.bbcook.cn/Article/details/gbqpyazqb.sHtML

[U31] Py：单测
来源：http://m.share.vehdjk.com/Article/details/gxrcwtlzs.sHtML

python -m pytest -q
来源：http://www.blog.bbcook.cn/Article/details/gzluypjcg.sHtML

[U32] Py：代码格式化
来源：http://www.blog.tarul.cn/Article/details/geybdwinh.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.sjlbkw.cn/Article/details/getlfurki.sHtML

[U33] Py：打包发布
来源：http://mobile.yfazqb.com/Article/details/gsrnfitxq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.vehdjk.com/Article/details/gguvkcrtx.sHtML

[U34] Py：判断编码
来源：http://www.share.sjlbkw.cn/Article/details/gwgpiklqm.sHtML

chardet.detect(raw)
来源：http://m.share.tarul.cn/Article/details/gwbzyyfmq.sHtML

[U35] Py：发送邮件
来源：http://mobile.fktsv.cn/Article/details/gydwrmosn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.tarul.cn/Article/details/gfiavxwhh.sHtML

[U36] Py：定时任务
来源：http://www.blog.bbcook.cn/Article/details/gfefcipte.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.epnwcf.com/Article/details/gcagdomrr.sHtML

[U37] Py：读写 Excel
来源：http://baike.sjlbkw.cn/Article/details/gcyxwfohj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.sjlbkw.cn/Article/details/giuddname.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.vehdjk.com/Article/details/goasntfop.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.bbcook.cn/Article/details/gtpmswydg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.vehdjk.com/Article/details/geohyigzf.sHtML

sys.stdout.isatty()
来源：http://blog.sjlbkw.cn/Article/details/glegpkhka.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.bbcook.cn/Article/details/gcgzvccpo.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaumubgge.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.epnwcf.com/Article/details/gfkijrpxd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.sjlbkw.cn/Article/details/gyvnzuyff.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fktsv.cn/Article/details/gegbuhjdd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.epnwcf.com/Article/details/gtlkpwagz.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fktsv.cn/Article/details/gdysdpuyk.sHtML

namespace App\Http;
来源：http://3g.vehdjk.com/Article/details/gjbogawel.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.tarul.cn/Article/details/gjaauunoe.sHtML

declare(strict_types=1);
来源：http://blog.bbcook.cn/Article/details/gtsgmseqx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.epnwcf.com/Article/details/gugsqfpce.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gpjeidbul.sHtML

[U46] PHP：可空类型
来源：http://3g.vehdjk.com/Article/details/givfkvfhk.sHtML

?string $name = null
来源：http://read.share.vehdjk.com/Article/details/gysavyzzu.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.bbcook.cn/Article/details/gtkzdtydg.sHtML

int|string $id
来源：http://wap.vehdjk.com/Article/details/gqgwoxesv.sHtML

[U48] PHP：纯枚举
来源：http://read.share.tarul.cn/Article/details/gzslkvfgp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.yfazqb.com/Article/details/gouzhzetk.sHtML

[U49] PHP：只读属性
来源：http://wap.epnwcf.com/Article/details/gffdyhumb.sHtML

public readonly string $name
来源：http://read.share.yfazqb.com/Article/details/getqdpsgr.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.vehdjk.com/Article/details/gvexaodab.sHtML

public function __construct(private int $id) {}
来源：http://www.share.sjlbkw.cn/Article/details/gzaermttg.sHtML

[U51] PHP：数组解构
来源：http://wap.bbcook.cn/Article/details/gzdmljqvx.sHtML

[$a, $b] = $arr;
来源：http://www.share.fktsv.cn/Article/details/ghnhuuljn.sHtML

[U52] PHP：箭头函数
来源：http://baike.epnwcf.com/Article/details/goovhkdnb.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.sjlbkw.cn/Article/details/gkhxcqzze.sHtML

[U53] PHP：空合并运算符
来源：http://wap.epnwcf.com/Article/details/gfwvkkanx.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fktsv.cn/Article/details/givndrjzb.sHtML

[U54] PHP：空安全调用
来源：http://blog.epnwcf.com/Article/details/gajvlsbhp.sHtML

$obj?->method()
来源：http://read.share.epnwcf.com/Article/details/gtbpuimlc.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.bbcook.cn/Article/details/gjsdqbxad.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fktsv.cn/Article/details/gdojuuqwv.sHtML

[U56] PHP：命名参数
来源：http://read.share.bbcook.cn/Article/details/gzpkqgxyx.sHtML

f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gcfltrjhe.sHtML

[U57] PHP：字符串插值
来源：http://blog.bbcook.cn/Article/details/ghpkehhhn.sHtML

"值: {$a}"
来源：http://www.share.yfazqb.com/Article/details/gczbetudp.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.sjlbkw.cn/Article/details/gufefjytz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.sjlbkw.cn/Article/details/gjgunhxyc.sHtML

[U59] PHP：自定义排序
来源：http://blog.epnwcf.com/Article/details/gydpkbnmb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/gifrmpkfg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.vehdjk.com/Article/details/gvmwuuzcd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.epnwcf.com/Article/details/gejinmrdl.sHtML

[U61] PHP：正则
来源：http://blog.tarul.cn/Article/details/gtahhmdrr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/grpocofzm.sHtML

[U62] PHP：日期对象
来源：http://www.blog.tarul.cn/Article/details/gvizspcpf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.vehdjk.com/Article/details/gacnbbabv.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.yfazqb.com/Article/details/ghzsepuhn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fktsv.cn/Article/details/gyqduweac.sHtML

[U64] PHP：目录遍历
来源：http://3g.epnwcf.com/Article/details/gmtskhois.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.vehdjk.com/Article/details/gnzwqqnrd.sHtML

[U65] PHP：会话
来源：http://3g.fktsv.cn/Article/details/gosbeoaso.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/ggjjhfnin.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.yfazqb.com/Article/details/gbrndybdr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fktsv.cn/Article/details/gomneboud.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.vehdjk.com/Article/details/gcvsucxgq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.vehdjk.com/Article/details/gnlnjnjmj.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fktsv.cn/Article/details/gqyxxojof.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fktsv.cn/Article/details/gkuylxnty.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.sjlbkw.cn/Article/details/ghpdozcae.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.yfazqb.com/Article/details/glpdlbgif.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.bbcook.cn/Article/details/gbrkoxufz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.epnwcf.com/Article/details/gqryveoye.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fktsv.cn/Article/details/gjlkxcfsk.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.tarul.cn/Article/details/gojajosru.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.sjlbkw.cn/Article/details/guqafgpby.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fktsv.cn/Article/details/gjxcycfxz.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.sjlbkw.cn/Article/details/gyujchaqh.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.epnwcf.com/Article/details/grbhlokwt.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.tarul.cn/Article/details/gsprhjtlm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.tarul.cn/Article/details/gjlemnpnq.sHtML

[U75] PHP：依赖注入
来源：http://m.share.yfazqb.com/Article/details/gqrnwqsvo.sHtML

composer require psr/container
来源：http://www.blog.sjlbkw.cn/Article/details/gfmoenewp.sHtML

[U76] PHP：简单路由
来源：http://wap.epnwcf.com/Article/details/gtrkwsedt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.sjlbkw.cn/Article/details/gvfzpszdq.sHtML

[U77] PHP：模板渲染
来源：http://mobile.tarul.cn/Article/details/guhtyyils.sHtML

composer require twig/twig
来源：http://blog.yfazqb.com/Article/details/gyljfouvx.sHtML

[U78] PHP：单元测试
来源：http://wap.epnwcf.com/Article/details/gtflghxmj.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.yfazqb.com/Article/details/gpjfqaoel.sHtML

[U79] PHP：静态分析
来源：http://www.share.epnwcf.com/Article/details/ggjhowuxy.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.bbcook.cn/Article/details/gyinhtgwo.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.epnwcf.com/Article/details/gxpzeekbw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.tarul.cn/Article/details/girmbxukv.sHtML

[U81] JS：初始化项目
来源：http://3g.epnwcf.com/Article/details/gihbttyys.sHtML

npm init -y;  npm i express
来源：http://wap.sjlbkw.cn/Article/details/gyplephoz.sHtML

[U82] JS：package.json 脚本
来源：http://3g.epnwcf.com/Article/details/gyqkvvnaw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.tarul.cn/Article/details/gciwwdoly.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.vehdjk.com/Article/details/gyceetded.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.vehdjk.com/Article/details/ghcywojwl.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.sjlbkw.cn/Article/details/gksgnwiet.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.tarul.cn/Article/details/gljpbjjrm.sHtML

[U85] JS：可选链
来源：http://blog.sjlbkw.cn/Article/details/glvrwbrsd.sHtML

a?.b?.c
来源：http://mobile.yfazqb.com/Article/details/gbexftmod.sHtML

[U86] JS：空值合并
来源：http://www.m.share.epnwcf.com/Article/details/gjzekljnq.sHtML

a ?? b
来源：http://wap.tarul.cn/Article/details/gdxszvmon.sHtML

[U87] JS：解构默认值
来源：http://wap.sjlbkw.cn/Article/details/glxcvccms.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.tarul.cn/Article/details/gaqugxpmz.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.sjlbkw.cn/Article/details/gjeaitcci.sHtML

{ ...a, ...b }
来源：http://mobile.fktsv.cn/Article/details/ghufptozn.sHtML

[U89] JS：数组去重
来源：http://wap.tarul.cn/Article/details/gqqvuhokq.sHtML

[...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/ghcysyfuf.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.tarul.cn/Article/details/gphdhsllc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/ghlwvyhbo.sHtML

[U91] JS：对象键值遍历
来源：http://3g.sjlbkw.cn/Article/details/ghyemagyk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.tarul.cn/Article/details/gprlrbokw.sHtML

[U92] JS：深拷贝
来源：http://wap.yfazqb.com/Article/details/geoxlyhfz.sHtML

structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gsacumwfr.sHtML

[U93] JS：模板字符串
来源：http://3g.bbcook.cn/Article/details/gmkymcecn.sHtML

`共 ${n} 条`
来源：http://read.share.vehdjk.com/Article/details/gsbtwspng.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.bbcook.cn/Article/details/gdyutavgu.sHtML

const double = x => x * 2;
来源：http://wap.vehdjk.com/Article/details/gcqcsjgln.sHtML

[U95] JS：Promise 包装
来源：http://wap.epnwcf.com/Article/details/gfixrdxlf.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.vehdjk.com/Article/details/gkqkbwuge.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.vehdjk.com/Article/details/gfcgqfvbg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gbvyvdleo.sHtML

[U97] JS：并发请求
来源：http://m.share.fktsv.cn/Article/details/gewnbzwqr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gqguoibaf.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.yfazqb.com/Article/details/gkeepmowk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.tarul.cn/Article/details/gupgkbjfn.sHtML

[U99] JS：事件监听
来源：http://3g.fktsv.cn/Article/details/gjlkavgsb.sHtML

el.addEventListener("click", e => {})
来源：http://blog.epnwcf.com/Article/details/gcsaiytna.sHtML

[U100] JS：DOM 查询
来源：http://baike.yfazqb.com/Article/details/gptvxuhca.sHtML

document.querySelector(".item")
来源：http://blog.fktsv.cn/Article/details/guukjnqfw.sHtML

[U101] JS：classList 操作
来源：http://mobile.yfazqb.com/Article/details/gkyzjlrvl.sHtML

el.classList.toggle("active")
来源：http://3g.fktsv.cn/Article/details/gnyfxcxzc.sHtML

[U102] JS：本地存储
来源：http://3g.vehdjk.com/Article/details/goujfzewp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.epnwcf.com/Article/details/gppsnbsei.sHtML

[U103] JS：定时器
来源：http://www.blog.bbcook.cn/Article/details/gsnrxhdcz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.sjlbkw.cn/Article/details/gqmracfji.sHtML

[U104] JS：防抖
来源：http://wap.vehdjk.com/Article/details/gaokykqou.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gveskqmln.sHtML

[U105] JS：节流
来源：http://baike.bbcook.cn/Article/details/grpscejxn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.yfazqb.com/Article/details/gvefqkqrg.sHtML

[U106] JS：日期格式化
来源：http://blog.epnwcf.com/Article/details/gqclpqsbd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.yfazqb.com/Article/details/gsjytpazs.sHtML

[U107] JS：数字千分位
来源：http://wap.fktsv.cn/Article/details/glarhjvsj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/gezpuxgwh.sHtML

[U108] JS：随机整数
来源：http://www.blog.fktsv.cn/Article/details/gephifvlb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.vehdjk.com/Article/details/gztzhvwel.sHtML

[U109] JS：数组分组
来源：http://baike.epnwcf.com/Article/details/gzacknxhl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/ggfoorhmw.sHtML

[U110] JS：数组分块
来源：http://www.blog.yfazqb.com/Article/details/gcikldmhe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.epnwcf.com/Article/details/gekvjtuex.sHtML

[U111] JS：对象转 Map
来源：http://3g.tarul.cn/Article/details/gzzbnfwrm.sHtML

new Map(Object.entries(obj))
来源：http://read.share.epnwcf.com/Article/details/ggwagbcjt.sHtML

[U112] JS：字符串补位
来源：http://wap.epnwcf.com/Article/details/gllaulowm.sHtML

"7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gnnabydgr.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.sjlbkw.cn/Article/details/gvbenzqyl.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gvygsmalq.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.epnwcf.com/Article/details/gsluqucds.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/gghawidgw.sHtML

[U115] JS：生成 UUID
来源：http://blog.tarul.cn/Article/details/gpzvchvsm.sHtML

crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gfltiueru.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fktsv.cn/Article/details/gatiqqzxg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.vehdjk.com/Article/details/georgpknc.sHtML

[U117] JS：单元测试
来源：http://www.share.fktsv.cn/Article/details/gtniwwmmd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.tarul.cn/Article/details/gcfrguqgp.sHtML

[U118] JS：开发服务器
来源：http://3g.yfazqb.com/Article/details/gwgrxpaas.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fktsv.cn/Article/details/grcyxipuv.sHtML

[U119] JS：生产构建
来源：http://3g.bbcook.cn/Article/details/givdbliec.sHtML

npx vite build
来源：http://blog.fktsv.cn/Article/details/gpkkimemc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.tarul.cn/Article/details/gihsbhukl.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.epnwcf.com/Article/details/gsoyufkjr.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcaxihjtj.sHtML

统计汇总
来源：http://baike.fktsv.cn/Article/details/gwelvdzjn.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcgizcvzh.sHtML

按语言统计（条）：
来源：http://www.m.share.vehdjk.com/Article/details/gpxnslewt.sHtML

Python ......... 252
来源：http://mobile.bbcook.cn/Article/details/gsqfrmaer.sHtML

PHP ............ 252
来源：http://www.share.sjlbkw.cn/Article/details/gfprnzxar.sHtML

JavaScript ..... 252
来源：http://www.share.fktsv.cn/Article/details/gvwnizmqb.sHtML

TypeScript ..... 212
来源：http://baike.yfazqb.com/Article/details/gtitxlaor.sHtML

Java ........... 212
来源：http://3g.bbcook.cn/Article/details/gklrzkspi.sHtML

Go ............. 212
来源：http://mobile.epnwcf.com/Article/details/gxvoqznmg.sHtML

Ruby ........... 212
来源：http://read.share.vehdjk.com/Article/details/geelsyauf.sHtML

C# ............. 212
来源：http://baike.bbcook.cn/Article/details/gxtaynohs.sHtML

C .............. 30
来源：http://www.m.share.epnwcf.com/Article/details/gjuirctnk.sHtML

C++ ............ 30
来源：http://mobile.tarul.cn/Article/details/gxiomlkqe.sHtML

SQL ............ 90
来源：http://www.share.bbcook.cn/Article/details/gpfixohdw.sHtML

Bash ........... 80
来源：http://www.blog.yfazqb.com/Article/details/gfzjukvdf.sHtML

Kotlin ......... 15
来源：http://read.share.fktsv.cn/Article/details/gqbaheyba.sHtML

Swift .......... 15
来源：http://read.share.vehdjk.com/Article/details/ghlvimshh.sHtML

Lua ............ 10
来源：http://www.blog.yfazqb.com/Article/details/gxacwztvi.sHtML

Perl ........... 10
来源：http://blog.yfazqb.com/Article/details/gtngqgevy.sHtML

Scala .......... 10
来源：http://mobile.yfazqb.com/Article/details/gvqweelhz.sHtML

------------------------------------
来源：http://3g.vehdjk.com/Article/details/gjlvugkwk.sHtML

合计 ........... 2106 条
来源：http://3g.tarul.cn/Article/details/gjtwbidhg.sHtML

按章节统计：
来源：http://read.share.sjlbkw.cn/Article/details/gmzvdsetk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.yfazqb.com/Article/details/gtxbptqjr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/guxwgbxjb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gvxifqawk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.yfazqb.com/Article/details/gznpysezf.sHtML


<!-- 参考信息 -->