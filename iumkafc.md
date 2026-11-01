代发 wailian999

[T43] Perl：字符串插值
来源：http://m.share.tarul.cn/Article/details/gojpiyhlc.sHtML

"值: $a"
来源：http://blog.bbcook.cn/Article/details/gjuscelvl.sHtML

[T44] Perl：条件
来源：http://3g.bbcook.cn/Article/details/gedqtslhm.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.tarul.cn/Article/details/gzciurpbb.sHtML

[T45] Perl：数组遍历
来源：http://www.share.sjlbkw.cn/Article/details/gdvjeheyk.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.epnwcf.com/Article/details/goxldamsc.sHtML

[T46] Perl：哈希操作
来源：http://wap.bbcook.cn/Article/details/gtbrtewbp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.yfazqb.com/Article/details/gdssiqjks.sHtML

[T47] Perl：正则捕获
来源：http://www.share.tarul.cn/Article/details/gmkycejxn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.tarul.cn/Article/details/gvxivlszx.sHtML

[T48] Perl：正则替换
来源：http://read.share.yfazqb.com/Article/details/gpuzxnplg.sHtML

$s =~ s/old/new/g;
来源：http://www.share.sjlbkw.cn/Article/details/gfxkyypxw.sHtML

[T49] Perl：函数
来源：http://mobile.tarul.cn/Article/details/gxdrcqrlh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/grxzkgcig.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gorxplysq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.yfazqb.com/Article/details/gkzypsrpj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.vehdjk.com/Article/details/gtdumxawd.sHtML

[T51] Scala：Hello World
来源：http://blog.fktsv.cn/Article/details/gwvyexefw.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/gotfjrgaf.sHtML

[T52] Scala：变量
来源：http://wap.yfazqb.com/Article/details/gvliwizbr.sHtML

val a = 1;  var b = 2
来源：http://read.share.bbcook.cn/Article/details/ghlstdpnq.sHtML

[T53] Scala：字符串插值
来源：http://blog.yfazqb.com/Article/details/gaybuqxsd.sHtML

s"值: $b"
来源：http://m.share.vehdjk.com/Article/details/ghmxexzoi.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/gmhfcsyyj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.epnwcf.com/Article/details/goqepmorp.sHtML

[T55] Scala：集合过滤
来源：http://wap.yfazqb.com/Article/details/gwhgrkeet.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.epnwcf.com/Article/details/gubabfege.sHtML

[T56] Scala：样例类
来源：http://blog.vehdjk.com/Article/details/gmfugtdiz.sHtML

case class User(name: String, age: Int)
来源：http://m.share.epnwcf.com/Article/details/gwmzwjgem.sHtML

[T57] Scala：模式匹配
来源：http://3g.vehdjk.com/Article/details/gtasdudut.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.bbcook.cn/Article/details/gilzfqbyb.sHtML

[T58] Scala：函数定义
来源：http://mobile.sjlbkw.cn/Article/details/goxkwvgyw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.vehdjk.com/Article/details/gqnkoginc.sHtML

[T59] Scala：循环
来源：http://3g.epnwcf.com/Article/details/ghxwmmioo.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.yfazqb.com/Article/details/gvfqpygyn.sHtML

[T60] Scala：折叠
来源：http://mobile.epnwcf.com/Article/details/gomgtpzrq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.bbcook.cn/Article/details/gliidcsoi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjgxcyhyu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.sjlbkw.cn/Article/details/gctliewlv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gcsoywttc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.yfazqb.com/Article/details/gogdmrvlj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.sjlbkw.cn/Article/details/grodyjelu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fktsv.cn/Article/details/ghmprvjrd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.tarul.cn/Article/details/gmmnklgss.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.vehdjk.com/Article/details/giovaazul.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.bbcook.cn/Article/details/ghdzqufvl.sHtML

[U04] Py：变量调试打印
来源：http://baike.yfazqb.com/Article/details/gfgnflbmx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.epnwcf.com/Article/details/gtkptyday.sHtML

[U05] Py：列表去重且保序
来源：http://wap.yfazqb.com/Article/details/gutjwlgeb.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/ghgvciwit.sHtML

[U06] Py：合并两个字典
来源：http://wap.epnwcf.com/Article/details/ghkwwkmlv.sHtML

{**a, **b}
来源：http://3g.fktsv.cn/Article/details/gajhxepfe.sHtML

[U07] Py：反转字典键值
来源：http://www.share.bbcook.cn/Article/details/gsamnfmgq.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.bbcook.cn/Article/details/gkcpjfkrj.sHtML

[U08] Py：展平二维列表
来源：http://baike.fktsv.cn/Article/details/gmxprjmtj.sHtML

[y for x in nested for y in x]
来源：http://m.share.yfazqb.com/Article/details/gxncgkcxc.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fktsv.cn/Article/details/gnkjwedqi.sHtML

max(d, key=d.get)
来源：http://blog.sjlbkw.cn/Article/details/gdlisqwmu.sHtML

[U10] Py：按值排序字典
来源：http://wap.bbcook.cn/Article/details/gshdywrxj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.vehdjk.com/Article/details/gywomfmdw.sHtML

[U11] Py：生成器表达式
来源：http://www.share.epnwcf.com/Article/details/ggudbjugg.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.yfazqb.com/Article/details/gibaqzvsd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fktsv.cn/Article/details/gietxarse.sHtML

Counter(arr).most_common(3)
来源：http://baike.sjlbkw.cn/Article/details/ghcejhazb.sHtML

[U13] Py：固定长度队列
来源：http://3g.yfazqb.com/Article/details/gzdcbutbt.sHtML

deque(maxlen=10)
来源：http://3g.bbcook.cn/Article/details/girvlzoph.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fktsv.cn/Article/details/gpgxljvwc.sHtML

defaultdict(list)
来源：http://mobile.sjlbkw.cn/Article/details/gjcqjfkyx.sHtML

[U15] Py：高精度计时
来源：http://blog.tarul.cn/Article/details/geyjzteaz.sHtML

t = time.perf_counter()
来源：http://mobile.sjlbkw.cn/Article/details/gvzrhjwyv.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.tarul.cn/Article/details/gaeylcvuo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.tarul.cn/Article/details/gsqnyviau.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.epnwcf.com/Article/details/gertzcxqd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.vehdjk.com/Article/details/gkefratem.sHtML

[U18] Py：预编译正则
来源：http://baike.yfazqb.com/Article/details/gowinwygc.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/gozorojna.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.sjlbkw.cn/Article/details/guncisqlg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.vehdjk.com/Article/details/gotgtvywe.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/guwkpxbhf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fktsv.cn/Article/details/gefjoyrdb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.vehdjk.com/Article/details/gadhdakvs.sHtML

@contextlib.contextmanager
来源：http://mobile.sjlbkw.cn/Article/details/goejpspel.sHtML

[U22] Py：矩阵转置
来源：http://wap.vehdjk.com/Article/details/gtancaldr.sHtML

list(zip(*m))
来源：http://mobile.tarul.cn/Article/details/gghdaxepa.sHtML

[U23] Py：分块读取大文件
来源：http://baike.epnwcf.com/Article/details/gjsdptgxy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.tarul.cn/Article/details/ggprdhvfx.sHtML

[U24] Py：路径操作
来源：http://www.share.vehdjk.com/Article/details/gfzvfzvbk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/gkreneqqo.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.yfazqb.com/Article/details/giesyztqt.sHtML

csv.DictReader(f)
来源：http://baike.sjlbkw.cn/Article/details/gjmretupt.sHtML

[U26] Py：并发下载
来源：http://read.share.fktsv.cn/Article/details/gsfvzzfnu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fktsv.cn/Article/details/geisqkfmt.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fktsv.cn/Article/details/gkbvyttaj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fktsv.cn/Article/details/gabwfnjof.sHtML

[U28] Py：类型别名
来源：http://www.blog.vehdjk.com/Article/details/gcygjuluo.sHtML

UserId = int
来源：http://read.share.vehdjk.com/Article/details/gapmvhzzj.sHtML

[U29] Py：属性校验
来源：http://read.share.epnwcf.com/Article/details/gpksqqaak.sHtML

@property 与 @x.setter 配合
来源：http://read.share.bbcook.cn/Article/details/gnxkmjlza.sHtML

[U30] Py：数据类
来源：http://www.blog.tarul.cn/Article/details/geakpxnlx.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fktsv.cn/Article/details/gwhvcbswe.sHtML

[U31] Py：单测
来源：http://www.share.bbcook.cn/Article/details/gahmjmbty.sHtML

python -m pytest -q
来源：http://www.blog.sjlbkw.cn/Article/details/gkoorcnwo.sHtML

[U32] Py：代码格式化
来源：http://m.share.vehdjk.com/Article/details/gdrnmblja.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.vehdjk.com/Article/details/gdxhbsljd.sHtML

[U33] Py：打包发布
来源：http://www.blog.tarul.cn/Article/details/gzzrjinss.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.yfazqb.com/Article/details/gyknvenpl.sHtML

[U34] Py：判断编码
来源：http://blog.epnwcf.com/Article/details/gkqkrrkpw.sHtML

chardet.detect(raw)
来源：http://www.blog.tarul.cn/Article/details/gwkakdspu.sHtML

[U35] Py：发送邮件
来源：http://m.share.fktsv.cn/Article/details/gmmaajnid.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.vehdjk.com/Article/details/glququbjl.sHtML

[U36] Py：定时任务
来源：http://blog.vehdjk.com/Article/details/gkrgqlojt.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.yfazqb.com/Article/details/gqczvsxky.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/gpqyfifum.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.bbcook.cn/Article/details/gdynjbxgn.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.tarul.cn/Article/details/gvbemsjbz.sHtML

Path(__file__).resolve().parent
来源：http://3g.tarul.cn/Article/details/grhpeqvqp.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.epnwcf.com/Article/details/gerbjlgrk.sHtML

sys.stdout.isatty()
来源：http://baike.sjlbkw.cn/Article/details/gnamryina.sHtML

[U40] Py：打印到标准错误
来源：http://blog.epnwcf.com/Article/details/gzwybhvnw.sHtML

print("err", file=sys.stderr)
来源：http://3g.yfazqb.com/Article/details/gyzhwlefb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.vehdjk.com/Article/details/gdltnebmy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.vehdjk.com/Article/details/gumynhgjx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.bbcook.cn/Article/details/gvuyvqrzk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.sjlbkw.cn/Article/details/grqrltvxj.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.tarul.cn/Article/details/grpmvacdd.sHtML

namespace App\Http;
来源：http://www.m.share.epnwcf.com/Article/details/gzipimauy.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.sjlbkw.cn/Article/details/gnmxmmcyw.sHtML

declare(strict_types=1);
来源：http://mobile.bbcook.cn/Article/details/gqawjotvh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.sjlbkw.cn/Article/details/gbxmpbesb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gslccgayn.sHtML

[U46] PHP：可空类型
来源：http://m.share.fktsv.cn/Article/details/guvwacydw.sHtML

?string $name = null
来源：http://mobile.vehdjk.com/Article/details/gsmgdrocy.sHtML

[U47] PHP：联合类型
来源：http://3g.sjlbkw.cn/Article/details/gvzsaisbr.sHtML

int|string $id
来源：http://mobile.vehdjk.com/Article/details/ghpogfrga.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.tarul.cn/Article/details/gusakglxe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.bbcook.cn/Article/details/gxouobtzt.sHtML

[U49] PHP：只读属性
来源：http://read.share.tarul.cn/Article/details/gyqvznuzj.sHtML

public readonly string $name
来源：http://3g.vehdjk.com/Article/details/gtahkihca.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.yfazqb.com/Article/details/gxihleoyn.sHtML

public function __construct(private int $id) {}
来源：http://mobile.yfazqb.com/Article/details/glpoepimf.sHtML

[U51] PHP：数组解构
来源：http://baike.fktsv.cn/Article/details/gaurbaipw.sHtML

[$a, $b] = $arr;
来源：http://wap.epnwcf.com/Article/details/gtzcvasku.sHtML

[U52] PHP：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/gdcdwhvse.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fktsv.cn/Article/details/gzqxddqyf.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.yfazqb.com/Article/details/gykolizpw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.bbcook.cn/Article/details/ghmbcjyfa.sHtML

[U54] PHP：空安全调用
来源：http://read.share.epnwcf.com/Article/details/guwqizmkp.sHtML

$obj?->method()
来源：http://mobile.epnwcf.com/Article/details/gmomearpu.sHtML

[U55] PHP：match 表达式
来源：http://3g.sjlbkw.cn/Article/details/gjjhtsegh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/ggbqanlnl.sHtML

[U56] PHP：命名参数
来源：http://www.blog.yfazqb.com/Article/details/gjhqjmdhn.sHtML

f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gaoucvkaj.sHtML

[U57] PHP：字符串插值
来源：http://3g.vehdjk.com/Article/details/gvontewiw.sHtML

"值: {$a}"
来源：http://m.share.tarul.cn/Article/details/ggbkhwqmj.sHtML

[U58] PHP：数组三件套
来源：http://blog.vehdjk.com/Article/details/gyjvrgudo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.bbcook.cn/Article/details/gveavhzhf.sHtML

[U59] PHP：自定义排序
来源：http://wap.fktsv.cn/Article/details/gwzldotdx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gdtxwwcxf.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.bbcook.cn/Article/details/gqrahijvo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.tarul.cn/Article/details/gpqpyhlyu.sHtML

[U61] PHP：正则
来源：http://www.share.tarul.cn/Article/details/gnuqbcdmn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.epnwcf.com/Article/details/gdcxazmfg.sHtML

[U62] PHP：日期对象
来源：http://blog.sjlbkw.cn/Article/details/ggkmlubzd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.yfazqb.com/Article/details/govgzawsb.sHtML

[U63] PHP：文件读写
来源：http://www.share.yfazqb.com/Article/details/gvgzpuysx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.epnwcf.com/Article/details/gdikiowum.sHtML

[U64] PHP：目录遍历
来源：http://read.share.bbcook.cn/Article/details/gwbpkjkpd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.epnwcf.com/Article/details/gfohvmpxw.sHtML

[U65] PHP：会话
来源：http://m.share.sjlbkw.cn/Article/details/gjjlrofja.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gzmxygwkq.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.tarul.cn/Article/details/gsdxkomqj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.epnwcf.com/Article/details/gxwvzxvpx.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.tarul.cn/Article/details/gygexhqkd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.epnwcf.com/Article/details/gelepkpsd.sHtML

[U68] PHP：PDO 连接
来源：http://3g.sjlbkw.cn/Article/details/gikwgnxqp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.bbcook.cn/Article/details/gjvpxwrcg.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fktsv.cn/Article/details/ghohsdjzt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.epnwcf.com/Article/details/gvjapuaqz.sHtML

[U70] PHP：PDO 事务
来源：http://3g.sjlbkw.cn/Article/details/gvczbzacq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.bbcook.cn/Article/details/gouglgjit.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gnuphmuml.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.sjlbkw.cn/Article/details/gxbfuzjqt.sHtML

[U72] PHP：写错误日志
来源：http://wap.bbcook.cn/Article/details/gqyqewuhh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.bbcook.cn/Article/details/ghfmutxch.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.epnwcf.com/Article/details/gkrqeetzt.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.tarul.cn/Article/details/grkulcpfg.sHtML

[U74] PHP：读取环境变量
来源：http://blog.epnwcf.com/Article/details/gpykirjju.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fktsv.cn/Article/details/gfjvktmsd.sHtML

[U75] PHP：依赖注入
来源：http://blog.vehdjk.com/Article/details/glsauolxo.sHtML

composer require psr/container
来源：http://wap.fktsv.cn/Article/details/gbtphiywe.sHtML

[U76] PHP：简单路由
来源：http://3g.bbcook.cn/Article/details/gzshixhyc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.tarul.cn/Article/details/gxmeamwwv.sHtML

[U77] PHP：模板渲染
来源：http://baike.yfazqb.com/Article/details/gjfuicaqs.sHtML

composer require twig/twig
来源：http://read.share.fktsv.cn/Article/details/grhndpjjw.sHtML

[U78] PHP：单元测试
来源：http://wap.vehdjk.com/Article/details/giydbiszm.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fktsv.cn/Article/details/glfaqziis.sHtML

[U79] PHP：静态分析
来源：http://m.share.epnwcf.com/Article/details/goxdbdbwc.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.sjlbkw.cn/Article/details/gfaxvwlan.sHtML

[U80] PHP：代码规范修复
来源：http://wap.bbcook.cn/Article/details/gnobviiyj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.tarul.cn/Article/details/gyjsgnzdl.sHtML

[U81] JS：初始化项目
来源：http://wap.yfazqb.com/Article/details/gpdhrzdhr.sHtML

npm init -y;  npm i express
来源：http://www.share.epnwcf.com/Article/details/govrrklwq.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.vehdjk.com/Article/details/gqwhwtdhq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.epnwcf.com/Article/details/gpavbymuf.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.sjlbkw.cn/Article/details/gtijfpcbv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.epnwcf.com/Article/details/gtlsomcfc.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.sjlbkw.cn/Article/details/gmfgdyueq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.bbcook.cn/Article/details/gavwkoazj.sHtML

[U85] JS：可选链
来源：http://read.share.vehdjk.com/Article/details/grjckujya.sHtML

a?.b?.c
来源：http://read.share.tarul.cn/Article/details/gkgttwgxx.sHtML

[U86] JS：空值合并
来源：http://www.share.sjlbkw.cn/Article/details/gpitugzcv.sHtML

a ?? b
来源：http://3g.fktsv.cn/Article/details/gfmawhbgj.sHtML

[U87] JS：解构默认值
来源：http://m.share.yfazqb.com/Article/details/gmhhkgmay.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.vehdjk.com/Article/details/gtzbhckiu.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.vehdjk.com/Article/details/glkqdhpvn.sHtML

{ ...a, ...b }
来源：http://wap.bbcook.cn/Article/details/gytzzzfrl.sHtML

[U89] JS：数组去重
来源：http://www.blog.vehdjk.com/Article/details/gqsbvdlko.sHtML

[...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gamsutbhm.sHtML

[U90] JS：数字数组排序
来源：http://blog.sjlbkw.cn/Article/details/ggetqkglj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gocrgzcgf.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.yfazqb.com/Article/details/gkshowgqv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.yfazqb.com/Article/details/gkvjmesix.sHtML

[U92] JS：深拷贝
来源：http://mobile.sjlbkw.cn/Article/details/glesuevfs.sHtML

structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gszyqjchs.sHtML

[U93] JS：模板字符串
来源：http://3g.yfazqb.com/Article/details/gxdzwlkid.sHtML

`共 ${n} 条`
来源：http://wap.epnwcf.com/Article/details/gcpwvsxjo.sHtML

[U94] JS：箭头函数
来源：http://baike.epnwcf.com/Article/details/gavnnmjmm.sHtML

const double = x => x * 2;
来源：http://blog.bbcook.cn/Article/details/gxispvkmm.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.tarul.cn/Article/details/gbhrrlirl.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fktsv.cn/Article/details/gzoisollx.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.epnwcf.com/Article/details/ggaujikoi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gddkqwcop.sHtML

[U97] JS：并发请求
来源：http://wap.bbcook.cn/Article/details/ghrhnvske.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gwzitlrie.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fktsv.cn/Article/details/ghvieatsi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.vehdjk.com/Article/details/gnrkcxnny.sHtML

[U99] JS：事件监听
来源：http://www.blog.tarul.cn/Article/details/gwabmwrny.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.sjlbkw.cn/Article/details/gwyufclso.sHtML

[U100] JS：DOM 查询
来源：http://blog.bbcook.cn/Article/details/gsajmtopr.sHtML

document.querySelector(".item")
来源：http://baike.sjlbkw.cn/Article/details/ggefdufss.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.tarul.cn/Article/details/glctntqzw.sHtML

el.classList.toggle("active")
来源：http://3g.yfazqb.com/Article/details/gtjozukip.sHtML

[U102] JS：本地存储
来源：http://3g.tarul.cn/Article/details/gdlhuzqoa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.bbcook.cn/Article/details/gssfoxnal.sHtML

[U103] JS：定时器
来源：http://www.m.share.yfazqb.com/Article/details/gsqmurdbf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.sjlbkw.cn/Article/details/gglikkevw.sHtML

[U104] JS：防抖
来源：http://m.share.sjlbkw.cn/Article/details/gtyeshyey.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gleithbqy.sHtML

[U105] JS：节流
来源：http://baike.yfazqb.com/Article/details/gkouvsazd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.tarul.cn/Article/details/gasczyxsy.sHtML

[U106] JS：日期格式化
来源：http://www.share.epnwcf.com/Article/details/gmzjkddsg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.epnwcf.com/Article/details/guxjpvdrb.sHtML

[U107] JS：数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/gfibmfflu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.epnwcf.com/Article/details/gpxwktqhf.sHtML

[U108] JS：随机整数
来源：http://baike.tarul.cn/Article/details/gymllmaxi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.tarul.cn/Article/details/gztobejqf.sHtML

[U109] JS：数组分组
来源：http://wap.fktsv.cn/Article/details/gntijmcom.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.vehdjk.com/Article/details/gfruwizan.sHtML

[U110] JS：数组分块
来源：http://www.blog.epnwcf.com/Article/details/glytpbqkg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.vehdjk.com/Article/details/gdrzklcsd.sHtML

[U111] JS：对象转 Map
来源：http://www.share.bbcook.cn/Article/details/gvzmqttkf.sHtML

new Map(Object.entries(obj))
来源：http://3g.fktsv.cn/Article/details/gfxwlcdzg.sHtML

[U112] JS：字符串补位
来源：http://m.share.vehdjk.com/Article/details/glrtriosg.sHtML

"7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gbiuhbaew.sHtML

[U113] JS：正则替换全部
来源：http://blog.sjlbkw.cn/Article/details/gdlihbsje.sHtML

s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gokyllyet.sHtML

[U114] JS：JSON 深比较
来源：http://wap.epnwcf.com/Article/details/gdomhssqj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/gzzsqcrdv.sHtML

[U115] JS：生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gduqvmtbr.sHtML

crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/grfwrjsvm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.epnwcf.com/Article/details/glutrigub.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fktsv.cn/Article/details/grkcwyqqw.sHtML

[U117] JS：单元测试
来源：http://www.blog.sjlbkw.cn/Article/details/gbmpwgxaa.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.sjlbkw.cn/Article/details/geidngfbk.sHtML

[U118] JS：开发服务器
来源：http://blog.yfazqb.com/Article/details/gdgxpprpt.sHtML

npm i -D vite;  npx vite
来源：http://read.share.epnwcf.com/Article/details/gvmiwcivq.sHtML

[U119] JS：生产构建
来源：http://blog.yfazqb.com/Article/details/gqzkbpwnl.sHtML

npx vite build
来源：http://www.m.share.vehdjk.com/Article/details/gewmaoshc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.tarul.cn/Article/details/gayiiwarn.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.sjlbkw.cn/Article/details/gngqsrtwx.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnktmdxdu.sHtML

统计汇总
来源：http://www.m.share.yfazqb.com/Article/details/gnlnbwgth.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/grqktbkvc.sHtML

按语言统计（条）：
来源：http://blog.yfazqb.com/Article/details/gbwzpggji.sHtML

Python ......... 252
来源：http://baike.fktsv.cn/Article/details/golvadogc.sHtML

PHP ............ 252
来源：http://baike.tarul.cn/Article/details/gjptmsbra.sHtML

JavaScript ..... 252
来源：http://baike.vehdjk.com/Article/details/gfvqnxfrs.sHtML

TypeScript ..... 212
来源：http://baike.vehdjk.com/Article/details/glqsymwin.sHtML

Java ........... 212
来源：http://www.share.vehdjk.com/Article/details/gmicwddbf.sHtML

Go ............. 212
来源：http://wap.tarul.cn/Article/details/gktvpniag.sHtML

Ruby ........... 212
来源：http://read.share.fktsv.cn/Article/details/gqfddqxdl.sHtML

C# ............. 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxbfvnao.sHtML

C .............. 30
来源：http://baike.epnwcf.com/Article/details/giwuizzqn.sHtML

C++ ............ 30
来源：http://mobile.sjlbkw.cn/Article/details/gjtotajob.sHtML

SQL ............ 90
来源：http://www.blog.yfazqb.com/Article/details/gtjolbpwr.sHtML

Bash ........... 80
来源：http://3g.fktsv.cn/Article/details/ggqbfexjb.sHtML

Kotlin ......... 15
来源：http://wap.epnwcf.com/Article/details/gtcgpsfct.sHtML

Swift .......... 15
来源：http://m.share.yfazqb.com/Article/details/gxhsxifzm.sHtML

Lua ............ 10
来源：http://mobile.epnwcf.com/Article/details/gmsyngank.sHtML

Perl ........... 10
来源：http://read.share.epnwcf.com/Article/details/gkzcvzmmm.sHtML


<!-- 参考信息 -->