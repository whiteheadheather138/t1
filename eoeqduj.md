代发 wailian999

[T45] Perl：数组遍历
来源：http://baike.bbcook.cn/Article/details/gwbazviwo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.tarul.cn/Article/details/gdawylcls.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fktsv.cn/Article/details/gdhntabxb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.sjlbkw.cn/Article/details/gtnkopzqc.sHtML

[T47] Perl：正则捕获
来源：http://baike.tarul.cn/Article/details/ghcluiwtb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.tarul.cn/Article/details/gpzvxkpij.sHtML

[T48] Perl：正则替换
来源：http://read.share.yfazqb.com/Article/details/glmhdilkb.sHtML

$s =~ s/old/new/g;
来源：http://www.share.bbcook.cn/Article/details/ghbnvdgna.sHtML

[T49] Perl：函数
来源：http://baike.tarul.cn/Article/details/gfxpsymqx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/glyboqens.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gmvmhlmkn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.tarul.cn/Article/details/gtyutrzsr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.vehdjk.com/Article/details/gxsflmoar.sHtML

[T51] Scala：Hello World
来源：http://baike.epnwcf.com/Article/details/gslgdkmoc.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/gjkpulmew.sHtML

[T52] Scala：变量
来源：http://3g.fktsv.cn/Article/details/glazubglv.sHtML

val a = 1;  var b = 2
来源：http://read.share.vehdjk.com/Article/details/gshiiqybz.sHtML

[T53] Scala：字符串插值
来源：http://wap.epnwcf.com/Article/details/gvoecwtiw.sHtML

s"值: $b"
来源：http://blog.fktsv.cn/Article/details/gmvifazgl.sHtML

[T54] Scala：集合映射
来源：http://m.share.epnwcf.com/Article/details/giovbwoxk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.tarul.cn/Article/details/gmdbvntgp.sHtML

[T55] Scala：集合过滤
来源：http://mobile.tarul.cn/Article/details/goxmphjiw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.tarul.cn/Article/details/gwtjixkfx.sHtML

[T56] Scala：样例类
来源：http://www.share.epnwcf.com/Article/details/gmvexayrb.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.bbcook.cn/Article/details/gauunvzrh.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gnlzdkzyc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.sjlbkw.cn/Article/details/gurkwpfqv.sHtML

[T58] Scala：函数定义
来源：http://baike.fktsv.cn/Article/details/gvwnvdxvb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.yfazqb.com/Article/details/gibjkyxmu.sHtML

[T59] Scala：循环
来源：http://mobile.sjlbkw.cn/Article/details/gentkccnn.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gzbqzzteq.sHtML

[T60] Scala：折叠
来源：http://www.m.share.tarul.cn/Article/details/gxaoptvax.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/gbzfobcrg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gohiazdvd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.bbcook.cn/Article/details/gkyuaiihl.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gclapdhah.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.epnwcf.com/Article/details/guvrlawst.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.tarul.cn/Article/details/gxxzmkwak.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.bbcook.cn/Article/details/gfegpiwvx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.vehdjk.com/Article/details/gtxiunbcx.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.vehdjk.com/Article/details/gxiksfpnf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.vehdjk.com/Article/details/geybjevss.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fktsv.cn/Article/details/gdysmlomn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.epnwcf.com/Article/details/gvxezacon.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.epnwcf.com/Article/details/gxduhnasq.sHtML

list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gagbmqepp.sHtML

[U06] Py：合并两个字典
来源：http://baike.sjlbkw.cn/Article/details/goppwlcbw.sHtML

{**a, **b}
来源：http://blog.vehdjk.com/Article/details/gheebcosq.sHtML

[U07] Py：反转字典键值
来源：http://www.share.yfazqb.com/Article/details/gciykvbdh.sHtML

{v: k for k, v in d.items()}
来源：http://wap.bbcook.cn/Article/details/gkwmafcdb.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gfdjjkgnm.sHtML

[y for x in nested for y in x]
来源：http://www.share.sjlbkw.cn/Article/details/grcicgezx.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.epnwcf.com/Article/details/ggjehjues.sHtML

max(d, key=d.get)
来源：http://mobile.sjlbkw.cn/Article/details/geslmovpt.sHtML

[U10] Py：按值排序字典
来源：http://m.share.epnwcf.com/Article/details/gfllesetm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.vehdjk.com/Article/details/gkmfokabe.sHtML

[U11] Py：生成器表达式
来源：http://mobile.vehdjk.com/Article/details/gotmjbbmv.sHtML

(x * 2 for x in arr)
来源：http://blog.tarul.cn/Article/details/getyvndys.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.sjlbkw.cn/Article/details/grumvkfgo.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gculygwre.sHtML

[U13] Py：固定长度队列
来源：http://wap.fktsv.cn/Article/details/gudscunmd.sHtML

deque(maxlen=10)
来源：http://3g.vehdjk.com/Article/details/gikcvmmba.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.sjlbkw.cn/Article/details/glzbstqwm.sHtML

defaultdict(list)
来源：http://baike.fktsv.cn/Article/details/gkztwcjoh.sHtML

[U15] Py：高精度计时
来源：http://www.share.epnwcf.com/Article/details/givzcjcbf.sHtML

t = time.perf_counter()
来源：http://baike.tarul.cn/Article/details/gbzezbsgy.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.tarul.cn/Article/details/gdeprbwzh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.epnwcf.com/Article/details/gerbxluqy.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.yfazqb.com/Article/details/gpfoijiom.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.sjlbkw.cn/Article/details/gpmwhvvhe.sHtML

[U18] Py：预编译正则
来源：http://mobile.vehdjk.com/Article/details/gtxtbfofy.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.sjlbkw.cn/Article/details/gqssgcwbq.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.tarul.cn/Article/details/gykmdynkb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.yfazqb.com/Article/details/gffzxrlqo.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.vehdjk.com/Article/details/gkxredyqu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.epnwcf.com/Article/details/glwsonncd.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.sjlbkw.cn/Article/details/gjprwucub.sHtML

@contextlib.contextmanager
来源：http://mobile.fktsv.cn/Article/details/gxaljgwhn.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.yfazqb.com/Article/details/gokxurfke.sHtML

list(zip(*m))
来源：http://3g.vehdjk.com/Article/details/gbuodswjb.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gijsjkvkz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.bbcook.cn/Article/details/glvzhqwdw.sHtML

[U24] Py：路径操作
来源：http://wap.yfazqb.com/Article/details/gjvatljrh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.yfazqb.com/Article/details/gqlsusgfq.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.vehdjk.com/Article/details/gwlaawiut.sHtML

csv.DictReader(f)
来源：http://mobile.vehdjk.com/Article/details/guwvwecxi.sHtML

[U26] Py：并发下载
来源：http://www.share.tarul.cn/Article/details/gxgdqngve.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.bbcook.cn/Article/details/gvcxpvghe.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fktsv.cn/Article/details/gxtfievqc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.sjlbkw.cn/Article/details/glaeyimww.sHtML

[U28] Py：类型别名
来源：http://blog.yfazqb.com/Article/details/gjxtrzgts.sHtML

UserId = int
来源：http://www.blog.tarul.cn/Article/details/gensljgym.sHtML

[U29] Py：属性校验
来源：http://blog.yfazqb.com/Article/details/gjmszjihb.sHtML

@property 与 @x.setter 配合
来源：http://baike.yfazqb.com/Article/details/gwfhcidvd.sHtML

[U30] Py：数据类
来源：http://m.share.vehdjk.com/Article/details/gvpmrrtst.sHtML

@dataclass(slots=True)
来源：http://read.share.bbcook.cn/Article/details/gheiectng.sHtML

[U31] Py：单测
来源：http://www.m.share.tarul.cn/Article/details/gbjsiuleb.sHtML

python -m pytest -q
来源：http://www.blog.yfazqb.com/Article/details/glzaplmzd.sHtML

[U32] Py：代码格式化
来源：http://3g.yfazqb.com/Article/details/gsevbnggj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.epnwcf.com/Article/details/gxfiodhbo.sHtML

[U33] Py：打包发布
来源：http://baike.sjlbkw.cn/Article/details/glsfnqwky.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.sjlbkw.cn/Article/details/gkalozarh.sHtML

[U34] Py：判断编码
来源：http://baike.epnwcf.com/Article/details/gpspgumxu.sHtML

chardet.detect(raw)
来源：http://www.m.share.fktsv.cn/Article/details/gyzvnjmee.sHtML

[U35] Py：发送邮件
来源：http://wap.vehdjk.com/Article/details/ghmiwejqi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.epnwcf.com/Article/details/gtgibtbkz.sHtML

[U36] Py：定时任务
来源：http://www.share.fktsv.cn/Article/details/ghlgmzzbg.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.sjlbkw.cn/Article/details/gwpgbcfwr.sHtML

[U37] Py：读写 Excel
来源：http://m.share.yfazqb.com/Article/details/gtfuatnnd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fktsv.cn/Article/details/gtertdibr.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.epnwcf.com/Article/details/guyoixhgx.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.sjlbkw.cn/Article/details/gizlccqzy.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.epnwcf.com/Article/details/gnkkygfri.sHtML

sys.stdout.isatty()
来源：http://www.blog.epnwcf.com/Article/details/gozrwnjhc.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.epnwcf.com/Article/details/grnqnajxd.sHtML

print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/glkkfxais.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.yfazqb.com/Article/details/gcymlhoha.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.epnwcf.com/Article/details/gfzmjtgun.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.yfazqb.com/Article/details/ggaohqzut.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.bbcook.cn/Article/details/glkubrneb.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gldevalnx.sHtML

namespace App\Http;
来源：http://mobile.sjlbkw.cn/Article/details/gkfpjaqfg.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.tarul.cn/Article/details/gfdouzala.sHtML

declare(strict_types=1);
来源：http://read.share.tarul.cn/Article/details/ghqbbtetm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.tarul.cn/Article/details/gtfijnfvd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gpqxookmq.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gdysruqux.sHtML

?string $name = null
来源：http://www.blog.epnwcf.com/Article/details/gibeuatvv.sHtML

[U47] PHP：联合类型
来源：http://wap.fktsv.cn/Article/details/gknkvlsdc.sHtML

int|string $id
来源：http://baike.epnwcf.com/Article/details/gquqmxrpb.sHtML

[U48] PHP：纯枚举
来源：http://read.share.bbcook.cn/Article/details/glmeqzoml.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.yfazqb.com/Article/details/gqipcxtsg.sHtML

[U49] PHP：只读属性
来源：http://blog.fktsv.cn/Article/details/gjrmjtjfn.sHtML

public readonly string $name
来源：http://wap.sjlbkw.cn/Article/details/gfxigqgqb.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.sjlbkw.cn/Article/details/gfsdlcquo.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.epnwcf.com/Article/details/gqcqupsms.sHtML

[U51] PHP：数组解构
来源：http://wap.epnwcf.com/Article/details/govmmooob.sHtML

[$a, $b] = $arr;
来源：http://m.share.fktsv.cn/Article/details/gfhfcrfyi.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/gdyhzeoou.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fktsv.cn/Article/details/gixgderth.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.yfazqb.com/Article/details/gegapfdcq.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.epnwcf.com/Article/details/gboutducn.sHtML

[U54] PHP：空安全调用
来源：http://www.share.yfazqb.com/Article/details/gliticxrn.sHtML

$obj?->method()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjidacmzy.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fktsv.cn/Article/details/ghafswwhg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.epnwcf.com/Article/details/gzjbrogqn.sHtML

[U56] PHP：命名参数
来源：http://read.share.bbcook.cn/Article/details/gljsjatoy.sHtML

f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/ggnjojbim.sHtML

[U57] PHP：字符串插值
来源：http://3g.vehdjk.com/Article/details/gvgbjdjep.sHtML

"值: {$a}"
来源：http://mobile.epnwcf.com/Article/details/gszphgynu.sHtML

[U58] PHP：数组三件套
来源：http://3g.tarul.cn/Article/details/gjuqjgbte.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.bbcook.cn/Article/details/gflkeojfe.sHtML

[U59] PHP：自定义排序
来源：http://mobile.sjlbkw.cn/Article/details/gsttncrzv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.bbcook.cn/Article/details/gdgtozvsy.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.sjlbkw.cn/Article/details/giuokovnz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.epnwcf.com/Article/details/gixcsvkgt.sHtML

[U61] PHP：正则
来源：http://3g.yfazqb.com/Article/details/gjktdlkhg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gzzsxppho.sHtML

[U62] PHP：日期对象
来源：http://wap.tarul.cn/Article/details/grkdzkqkz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.yfazqb.com/Article/details/gtnrlciyn.sHtML

[U63] PHP：文件读写
来源：http://read.share.fktsv.cn/Article/details/gqylqmsov.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.bbcook.cn/Article/details/gsqvxdvre.sHtML

[U64] PHP：目录遍历
来源：http://blog.vehdjk.com/Article/details/gzpdngjub.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.yfazqb.com/Article/details/goopexumw.sHtML

[U65] PHP：会话
来源：http://mobile.tarul.cn/Article/details/gcmtlygyp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gxlfyxujc.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.sjlbkw.cn/Article/details/gkmfyonic.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.bbcook.cn/Article/details/gygujqsqe.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fktsv.cn/Article/details/gbozektlq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fktsv.cn/Article/details/ggnpjyvhb.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fktsv.cn/Article/details/gionyywgo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.tarul.cn/Article/details/gzpfwzlsk.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fktsv.cn/Article/details/gpvsbluev.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.epnwcf.com/Article/details/gwnbwyery.sHtML

[U70] PHP：PDO 事务
来源：http://wap.vehdjk.com/Article/details/gzrkfpqjv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.epnwcf.com/Article/details/gfycfmaxh.sHtML

[U71] PHP：抛出异常
来源：http://blog.yfazqb.com/Article/details/gblusdvdg.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.bbcook.cn/Article/details/gyxwbdgjy.sHtML

[U72] PHP：写错误日志
来源：http://read.share.tarul.cn/Article/details/gsytxvixa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.bbcook.cn/Article/details/ggzwzxfai.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.yfazqb.com/Article/details/gzuqsdicn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.sjlbkw.cn/Article/details/gnqxdknfk.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.tarul.cn/Article/details/gjsqqhftx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.sjlbkw.cn/Article/details/gxtbjqwqh.sHtML

[U75] PHP：依赖注入
来源：http://www.share.bbcook.cn/Article/details/gmjqdjnyt.sHtML

composer require psr/container
来源：http://www.blog.vehdjk.com/Article/details/gakdniieb.sHtML

[U76] PHP：简单路由
来源：http://www.share.epnwcf.com/Article/details/gnllaqvwk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.yfazqb.com/Article/details/gpgahlrdo.sHtML

[U77] PHP：模板渲染
来源：http://m.share.tarul.cn/Article/details/gmtcmdjop.sHtML

composer require twig/twig
来源：http://www.m.share.bbcook.cn/Article/details/gsqzzpvnj.sHtML

[U78] PHP：单元测试
来源：http://www.share.yfazqb.com/Article/details/giofohlkk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.bbcook.cn/Article/details/gpdikvvku.sHtML

[U79] PHP：静态分析
来源：http://wap.epnwcf.com/Article/details/gauwmvdhu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.bbcook.cn/Article/details/gllgstyjk.sHtML

[U80] PHP：代码规范修复
来源：http://3g.tarul.cn/Article/details/gktxmdwyi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.sjlbkw.cn/Article/details/gitojnlvs.sHtML

[U81] JS：初始化项目
来源：http://www.blog.vehdjk.com/Article/details/gjuoqvyqo.sHtML

npm init -y;  npm i express
来源：http://baike.sjlbkw.cn/Article/details/glptzoxti.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.sjlbkw.cn/Article/details/gjspfxkdm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.epnwcf.com/Article/details/gpzymqfgb.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.tarul.cn/Article/details/guqjcdwbv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gckglbous.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.bbcook.cn/Article/details/godeqmjzv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.yfazqb.com/Article/details/gtabqrwfx.sHtML

[U85] JS：可选链
来源：http://m.share.yfazqb.com/Article/details/gykvfvgrf.sHtML

a?.b?.c
来源：http://www.share.sjlbkw.cn/Article/details/gzlwwhhpu.sHtML

[U86] JS：空值合并
来源：http://read.share.yfazqb.com/Article/details/gdbootwgd.sHtML

a ?? b
来源：http://www.share.vehdjk.com/Article/details/geqzzgdrf.sHtML

[U87] JS：解构默认值
来源：http://m.share.bbcook.cn/Article/details/gnfuwedfd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.vehdjk.com/Article/details/ghggulncp.sHtML

[U88] JS：对象展开合并
来源：http://m.share.epnwcf.com/Article/details/gwboepdmn.sHtML

{ ...a, ...b }
来源：http://wap.tarul.cn/Article/details/glfcopune.sHtML

[U89] JS：数组去重
来源：http://www.m.share.bbcook.cn/Article/details/ggcstnmjq.sHtML

[...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gprgsmcqx.sHtML

[U90] JS：数字数组排序
来源：http://baike.fktsv.cn/Article/details/gymtulelr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gvrcmoshy.sHtML

[U91] JS：对象键值遍历
来源：http://blog.yfazqb.com/Article/details/gsxwgxbva.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.yfazqb.com/Article/details/gcwifxpec.sHtML

[U92] JS：深拷贝
来源：http://3g.epnwcf.com/Article/details/gpkissuge.sHtML

structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ggeqkphle.sHtML

[U93] JS：模板字符串
来源：http://mobile.yfazqb.com/Article/details/gzpdyazlh.sHtML

`共 ${n} 条`
来源：http://3g.yfazqb.com/Article/details/gfahblvrc.sHtML

[U94] JS：箭头函数
来源：http://mobile.sjlbkw.cn/Article/details/gksqxheqh.sHtML

const double = x => x * 2;
来源：http://www.m.share.vehdjk.com/Article/details/glhfukkvw.sHtML

[U95] JS：Promise 包装
来源：http://wap.tarul.cn/Article/details/gyrfurwoo.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.yfazqb.com/Article/details/gsidtyyka.sHtML

[U96] JS：async/await 与异常
来源：http://3g.vehdjk.com/Article/details/glihjjbcd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gymfwtjpt.sHtML

[U97] JS：并发请求
来源：http://www.blog.yfazqb.com/Article/details/gmgcdrcei.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gxpvgrhvq.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.epnwcf.com/Article/details/gazidvwgv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.epnwcf.com/Article/details/gdhxgorjh.sHtML

[U99] JS：事件监听
来源：http://www.share.tarul.cn/Article/details/gvnxfhqzw.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.tarul.cn/Article/details/gsxifrrja.sHtML

[U100] JS：DOM 查询
来源：http://blog.sjlbkw.cn/Article/details/gwaxjaugi.sHtML

document.querySelector(".item")
来源：http://www.share.bbcook.cn/Article/details/gccvglnki.sHtML

[U101] JS：classList 操作
来源：http://mobile.epnwcf.com/Article/details/grjewfeiz.sHtML

el.classList.toggle("active")
来源：http://blog.epnwcf.com/Article/details/goddunpcp.sHtML

[U102] JS：本地存储
来源：http://wap.epnwcf.com/Article/details/gufhwothv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.tarul.cn/Article/details/gjolcwpzj.sHtML

[U103] JS：定时器
来源：http://wap.bbcook.cn/Article/details/grxcjnxeb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.sjlbkw.cn/Article/details/gbiwhwapr.sHtML

[U104] JS：防抖
来源：http://www.m.share.bbcook.cn/Article/details/gfannggba.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/ghxkpwopd.sHtML

[U105] JS：节流
来源：http://read.share.bbcook.cn/Article/details/gjwqhodbb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.sjlbkw.cn/Article/details/gyaoyhdpm.sHtML

[U106] JS：日期格式化
来源：http://www.share.fktsv.cn/Article/details/ggthlohwr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.tarul.cn/Article/details/gpuhihpex.sHtML

[U107] JS：数字千分位
来源：http://read.share.vehdjk.com/Article/details/gixdlvgnf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fktsv.cn/Article/details/gnkcjjeor.sHtML

[U108] JS：随机整数
来源：http://read.share.tarul.cn/Article/details/gbyiucxrh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.vehdjk.com/Article/details/ghtlfomzm.sHtML

[U109] JS：数组分组
来源：http://baike.sjlbkw.cn/Article/details/gyigzuokz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gsoqllpto.sHtML

[U110] JS：数组分块
来源：http://wap.epnwcf.com/Article/details/gnvemzvvd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.yfazqb.com/Article/details/gwkahrtit.sHtML

[U111] JS：对象转 Map
来源：http://m.share.yfazqb.com/Article/details/gezhsdlwj.sHtML

new Map(Object.entries(obj))
来源：http://blog.vehdjk.com/Article/details/gynsfkwha.sHtML

[U112] JS：字符串补位
来源：http://read.share.vehdjk.com/Article/details/gvltsukil.sHtML

"7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/govvaztib.sHtML

[U113] JS：正则替换全部
来源：http://3g.yfazqb.com/Article/details/gnpqbfckl.sHtML

s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gchsiuwhp.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fktsv.cn/Article/details/gaknszoss.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gflfnodnc.sHtML

[U115] JS：生成 UUID
来源：http://baike.bbcook.cn/Article/details/gkrvxfvlj.sHtML

crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gkhyjftms.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.tarul.cn/Article/details/gioyyajjn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fktsv.cn/Article/details/gfwvwxllc.sHtML

[U117] JS：单元测试
来源：http://blog.epnwcf.com/Article/details/gleuhnjuj.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.vehdjk.com/Article/details/gqhpkkvbz.sHtML

[U118] JS：开发服务器
来源：http://www.blog.vehdjk.com/Article/details/goxxycopv.sHtML

npm i -D vite;  npx vite
来源：http://m.share.sjlbkw.cn/Article/details/gkmutmhoc.sHtML

[U119] JS：生产构建
来源：http://read.share.tarul.cn/Article/details/ggphbieeb.sHtML

npx vite build
来源：http://wap.sjlbkw.cn/Article/details/grqrcjoka.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.epnwcf.com/Article/details/gwnnhltcu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.epnwcf.com/Article/details/golewfvpj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gztzuzrns.sHtML

统计汇总
来源：http://www.share.epnwcf.com/Article/details/gnmjcbmny.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glpdulcry.sHtML

按语言统计（条）：
来源：http://wap.tarul.cn/Article/details/gzklzlafi.sHtML

Python ......... 252
来源：http://3g.bbcook.cn/Article/details/gmhhwwwjf.sHtML

PHP ............ 252
来源：http://read.share.sjlbkw.cn/Article/details/gujfhizej.sHtML

JavaScript ..... 252
来源：http://m.share.yfazqb.com/Article/details/glwgpdfdf.sHtML

TypeScript ..... 212
来源：http://read.share.tarul.cn/Article/details/gdinvrqyn.sHtML

Java ........... 212
来源：http://3g.tarul.cn/Article/details/gkorhjhxn.sHtML

Go ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/ggohazlbx.sHtML

Ruby ........... 212
来源：http://baike.yfazqb.com/Article/details/gqdhuwoqp.sHtML

C# ............. 212
来源：http://3g.vehdjk.com/Article/details/gwkdjhvby.sHtML

C .............. 30
来源：http://www.m.share.fktsv.cn/Article/details/gulbpnmbe.sHtML

C++ ............ 30
来源：http://mobile.tarul.cn/Article/details/gvafxtynf.sHtML

SQL ............ 90
来源：http://m.share.fktsv.cn/Article/details/gualianxy.sHtML

Bash ........... 80
来源：http://3g.fktsv.cn/Article/details/gbsaomipu.sHtML

Kotlin ......... 15
来源：http://www.blog.tarul.cn/Article/details/gkcnmklyt.sHtML

Swift .......... 15
来源：http://m.share.tarul.cn/Article/details/gniwwyuym.sHtML

Lua ............ 10
来源：http://www.blog.vehdjk.com/Article/details/gloziyack.sHtML

Perl ........... 10
来源：http://wap.sjlbkw.cn/Article/details/gqdcpuiji.sHtML

Scala .......... 10
来源：http://www.share.sjlbkw.cn/Article/details/gtlrxgpwz.sHtML

------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/geagzzxhb.sHtML

合计 ........... 2106 条
来源：http://www.share.epnwcf.com/Article/details/ggmjcboox.sHtML

按章节统计：
来源：http://blog.sjlbkw.cn/Article/details/gdjqgmlhv.sHtML


<!-- 参考信息 -->