代发 wailian999

[T45] Perl：数组遍历
来源：http://www.share.yfazqb.com/Article/details/gyfzidmbh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.yfazqb.com/Article/details/gocbbksky.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.tarul.cn/Article/details/gufvlhzfs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.tarul.cn/Article/details/gvfjlqfqh.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.tarul.cn/Article/details/gpjnfhhnt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.vehdjk.com/Article/details/gwaerfway.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.bbcook.cn/Article/details/gaasvhqtd.sHtML

$s =~ s/old/new/g;
来源：http://m.share.vehdjk.com/Article/details/grulkzbxv.sHtML

[T49] Perl：函数
来源：http://blog.vehdjk.com/Article/details/glaybutox.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/glbccnmwg.sHtML

[T50] Perl：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gtunadcys.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.vehdjk.com/Article/details/gbafrpsdw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fktsv.cn/Article/details/gcturzvvo.sHtML

[T51] Scala：Hello World
来源：http://3g.vehdjk.com/Article/details/gubvxriqw.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gyxayesfe.sHtML

[T52] Scala：变量
来源：http://3g.epnwcf.com/Article/details/gdawmmdau.sHtML

val a = 1;  var b = 2
来源：http://wap.bbcook.cn/Article/details/gmlleymbt.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gjzgykbht.sHtML

s"值: $b"
来源：http://wap.epnwcf.com/Article/details/gzxceytks.sHtML

[T54] Scala：集合映射
来源：http://read.share.bbcook.cn/Article/details/gwpvwsves.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.yfazqb.com/Article/details/glxunqaho.sHtML

[T55] Scala：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gbbjjpgqb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fktsv.cn/Article/details/gmixebehd.sHtML

[T56] Scala：样例类
来源：http://blog.fktsv.cn/Article/details/ghbwfyzkt.sHtML

case class User(name: String, age: Int)
来源：http://www.share.tarul.cn/Article/details/gxwwswdre.sHtML

[T57] Scala：模式匹配
来源：http://3g.bbcook.cn/Article/details/grqspxugq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.epnwcf.com/Article/details/gjgsmifho.sHtML

[T58] Scala：函数定义
来源：http://wap.vehdjk.com/Article/details/gsvhnsvle.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.sjlbkw.cn/Article/details/gfxagquaa.sHtML

[T59] Scala：循环
来源：http://www.share.vehdjk.com/Article/details/gypvnildn.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gqnbxaxqv.sHtML

[T60] Scala：折叠
来源：http://mobile.bbcook.cn/Article/details/glfvwkiqk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.yfazqb.com/Article/details/gwkhwkwot.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gxhvvdhbg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gobnrndri.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwibwutao.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.epnwcf.com/Article/details/gquzkhijr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.epnwcf.com/Article/details/grbiipyos.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.yfazqb.com/Article/details/gftnwwjlg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.epnwcf.com/Article/details/giupfagjy.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/gluhpgvyt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.vehdjk.com/Article/details/gkqpltrys.sHtML

[U04] Py：变量调试打印
来源：http://baike.yfazqb.com/Article/details/grhdzabah.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.bbcook.cn/Article/details/ggcwsqoxx.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/gihxofagb.sHtML

list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/gnfgyanjq.sHtML

[U06] Py：合并两个字典
来源：http://read.share.sjlbkw.cn/Article/details/guuhwfbbr.sHtML

{**a, **b}
来源：http://3g.sjlbkw.cn/Article/details/gbcrhuzqq.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/gysapaqoy.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.vehdjk.com/Article/details/gmbkzqojl.sHtML

[U08] Py：展平二维列表
来源：http://baike.tarul.cn/Article/details/gimktycoi.sHtML

[y for x in nested for y in x]
来源：http://baike.yfazqb.com/Article/details/gqlbdiqxo.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.tarul.cn/Article/details/gvixfiigg.sHtML

max(d, key=d.get)
来源：http://www.share.bbcook.cn/Article/details/ghwytnpsm.sHtML

[U10] Py：按值排序字典
来源：http://www.share.epnwcf.com/Article/details/gfjaialil.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.epnwcf.com/Article/details/gpfevdlls.sHtML

[U11] Py：生成器表达式
来源：http://3g.fktsv.cn/Article/details/gcxxetfds.sHtML

(x * 2 for x in arr)
来源：http://3g.tarul.cn/Article/details/gsnulgpam.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.tarul.cn/Article/details/gqluvzlzi.sHtML

Counter(arr).most_common(3)
来源：http://blog.bbcook.cn/Article/details/gympspgfl.sHtML

[U13] Py：固定长度队列
来源：http://blog.epnwcf.com/Article/details/gobqdghgw.sHtML

deque(maxlen=10)
来源：http://baike.bbcook.cn/Article/details/gnnpvzoko.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.tarul.cn/Article/details/gmxqinyhi.sHtML

defaultdict(list)
来源：http://baike.yfazqb.com/Article/details/gpvwucrvz.sHtML

[U15] Py：高精度计时
来源：http://www.share.yfazqb.com/Article/details/gaedfebux.sHtML

t = time.perf_counter()
来源：http://3g.fktsv.cn/Article/details/gfagtxwwd.sHtML

[U16] Py：命令行参数解析
来源：http://blog.vehdjk.com/Article/details/gcqiqqkoe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.bbcook.cn/Article/details/gpkvkwuty.sHtML

[U17] Py：初始化日志
来源：http://mobile.vehdjk.com/Article/details/gxntvowgh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.vehdjk.com/Article/details/gqhuyhqqq.sHtML

[U18] Py：预编译正则
来源：http://wap.sjlbkw.cn/Article/details/gfdjznnjg.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/ginwrqydn.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.yfazqb.com/Article/details/gryxevvhh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.yfazqb.com/Article/details/gtlneigwd.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fktsv.cn/Article/details/glaanhtts.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.epnwcf.com/Article/details/gykrfccnp.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.yfazqb.com/Article/details/gmfoyrrmf.sHtML

@contextlib.contextmanager
来源：http://mobile.fktsv.cn/Article/details/ggwgmhtji.sHtML

[U22] Py：矩阵转置
来源：http://blog.sjlbkw.cn/Article/details/gzjqpvghp.sHtML

list(zip(*m))
来源：http://blog.tarul.cn/Article/details/gpacytnig.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.yfazqb.com/Article/details/gayprjnrm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.epnwcf.com/Article/details/gnvfzxvec.sHtML

[U24] Py：路径操作
来源：http://read.share.yfazqb.com/Article/details/ganeymktv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/gkydktpgx.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.epnwcf.com/Article/details/glalhxivf.sHtML

csv.DictReader(f)
来源：http://blog.fktsv.cn/Article/details/gsnakiycn.sHtML

[U26] Py：并发下载
来源：http://www.blog.epnwcf.com/Article/details/geqjrsjpl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.tarul.cn/Article/details/grzbbzszh.sHtML

[U27] Py：异步 HTTP
来源：http://3g.bbcook.cn/Article/details/gaiusnqmu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.tarul.cn/Article/details/grburxohh.sHtML

[U28] Py：类型别名
来源：http://read.share.tarul.cn/Article/details/gqibzypcq.sHtML

UserId = int
来源：http://m.share.yfazqb.com/Article/details/gmxofkked.sHtML

[U29] Py：属性校验
来源：http://baike.fktsv.cn/Article/details/gjdodywrb.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fktsv.cn/Article/details/gincfsixh.sHtML

[U30] Py：数据类
来源：http://3g.yfazqb.com/Article/details/gunbogfqc.sHtML

@dataclass(slots=True)
来源：http://blog.bbcook.cn/Article/details/gepgfpjko.sHtML

[U31] Py：单测
来源：http://read.share.yfazqb.com/Article/details/gvwzrjmfx.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/gwgtqjeyf.sHtML

[U32] Py：代码格式化
来源：http://blog.sjlbkw.cn/Article/details/gjocsauxa.sHtML

ruff format . && ruff check --fix .
来源：http://3g.tarul.cn/Article/details/gvkbtsmnt.sHtML

[U33] Py：打包发布
来源：http://read.share.vehdjk.com/Article/details/gbqdbwxie.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fktsv.cn/Article/details/ghhfwqiyq.sHtML

[U34] Py：判断编码
来源：http://www.m.share.epnwcf.com/Article/details/gfumtjhrm.sHtML

chardet.detect(raw)
来源：http://3g.sjlbkw.cn/Article/details/gosqlmzbr.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.epnwcf.com/Article/details/gbcitfzud.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.vehdjk.com/Article/details/gztvfzjnf.sHtML

[U36] Py：定时任务
来源：http://blog.tarul.cn/Article/details/gazseewul.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqivpdwb.sHtML

[U37] Py：读写 Excel
来源：http://read.share.vehdjk.com/Article/details/gfaypjzaq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.sjlbkw.cn/Article/details/gxmzajudy.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fktsv.cn/Article/details/gsdowieev.sHtML

Path(__file__).resolve().parent
来源：http://baike.epnwcf.com/Article/details/goexclacq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fktsv.cn/Article/details/gzfxukfcp.sHtML

sys.stdout.isatty()
来源：http://mobile.sjlbkw.cn/Article/details/glvdbogox.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.tarul.cn/Article/details/gwgynxjou.sHtML

print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/gvlpyrhao.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.bbcook.cn/Article/details/gvojjtvdp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.epnwcf.com/Article/details/gaqesyrse.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.tarul.cn/Article/details/ghyhhauhh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.tarul.cn/Article/details/guyrqmgwp.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.yfazqb.com/Article/details/gxetzfhqf.sHtML

namespace App\Http;
来源：http://mobile.sjlbkw.cn/Article/details/gkxkwrgkz.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fktsv.cn/Article/details/gkhltrdzr.sHtML

declare(strict_types=1);
来源：http://m.share.vehdjk.com/Article/details/gnkjnrlik.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.tarul.cn/Article/details/gulcrmhwc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/genhclale.sHtML

[U46] PHP：可空类型
来源：http://m.share.fktsv.cn/Article/details/gpjcjinpo.sHtML

?string $name = null
来源：http://m.share.bbcook.cn/Article/details/gfaqooqjd.sHtML

[U47] PHP：联合类型
来源：http://www.share.tarul.cn/Article/details/gknatynuj.sHtML

int|string $id
来源：http://mobile.vehdjk.com/Article/details/gvaqhrezh.sHtML

[U48] PHP：纯枚举
来源：http://www.share.bbcook.cn/Article/details/ghxjsprng.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.epnwcf.com/Article/details/gfikkfxyd.sHtML

[U49] PHP：只读属性
来源：http://mobile.sjlbkw.cn/Article/details/gqlpmejel.sHtML

public readonly string $name
来源：http://baike.bbcook.cn/Article/details/gvytnibmt.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fktsv.cn/Article/details/gmihguvpz.sHtML

public function __construct(private int $id) {}
来源：http://wap.yfazqb.com/Article/details/gofxwyfbt.sHtML

[U51] PHP：数组解构
来源：http://m.share.sjlbkw.cn/Article/details/gguuuerle.sHtML

[$a, $b] = $arr;
来源：http://www.share.fktsv.cn/Article/details/gailhfpsc.sHtML

[U52] PHP：箭头函数
来源：http://m.share.tarul.cn/Article/details/gppfafbnt.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.yfazqb.com/Article/details/gdqbdeuip.sHtML

[U53] PHP：空合并运算符
来源：http://baike.tarul.cn/Article/details/gbeofpznl.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.epnwcf.com/Article/details/grcvffgpj.sHtML

[U54] PHP：空安全调用
来源：http://3g.bbcook.cn/Article/details/gppqxiwct.sHtML

$obj?->method()
来源：http://wap.tarul.cn/Article/details/gldihrgjc.sHtML

[U55] PHP：match 表达式
来源：http://wap.fktsv.cn/Article/details/gskklensn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.bbcook.cn/Article/details/gutjfuszy.sHtML

[U56] PHP：命名参数
来源：http://3g.vehdjk.com/Article/details/gjxsanevp.sHtML

f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gwpgmsabh.sHtML

[U57] PHP：字符串插值
来源：http://blog.tarul.cn/Article/details/gzmjecmsy.sHtML

"值: {$a}"
来源：http://www.share.yfazqb.com/Article/details/gunkjnpkq.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fktsv.cn/Article/details/grclxedra.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fktsv.cn/Article/details/gyljbdyjw.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fktsv.cn/Article/details/gtlnhetts.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/goqnisamw.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.tarul.cn/Article/details/gbpesebuk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.epnwcf.com/Article/details/gvupejozf.sHtML

[U61] PHP：正则
来源：http://www.m.share.vehdjk.com/Article/details/gyvjginym.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gibfyxgmt.sHtML

[U62] PHP：日期对象
来源：http://read.share.bbcook.cn/Article/details/gniodbayk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.sjlbkw.cn/Article/details/gyfnjnvng.sHtML

[U63] PHP：文件读写
来源：http://read.share.tarul.cn/Article/details/gwmbkgmzd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.tarul.cn/Article/details/ghfoukwim.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.yfazqb.com/Article/details/grcamfmbv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.bbcook.cn/Article/details/gbhowdbkd.sHtML

[U65] PHP：会话
来源：http://mobile.tarul.cn/Article/details/gnrzanelf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.tarul.cn/Article/details/gmgychoms.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.bbcook.cn/Article/details/grktkvmbx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fktsv.cn/Article/details/gsgwdpbec.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.tarul.cn/Article/details/gaulhauhp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.epnwcf.com/Article/details/ghmidnyxf.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.yfazqb.com/Article/details/gysedftlj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.tarul.cn/Article/details/glywxmyif.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.yfazqb.com/Article/details/gbdovtelw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fktsv.cn/Article/details/gybmxwnna.sHtML

[U70] PHP：PDO 事务
来源：http://blog.tarul.cn/Article/details/gheltsqhm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.sjlbkw.cn/Article/details/gtbohhpnq.sHtML

[U71] PHP：抛出异常
来源：http://baike.tarul.cn/Article/details/gnzpwfrbb.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.epnwcf.com/Article/details/gjywwrogt.sHtML

[U72] PHP：写错误日志
来源：http://www.share.vehdjk.com/Article/details/galtoemtj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fktsv.cn/Article/details/gxkyokdgr.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.vehdjk.com/Article/details/gjgvyrkgz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fktsv.cn/Article/details/gjfovtcjv.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fktsv.cn/Article/details/gnqxsjzxe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.tarul.cn/Article/details/gyzlhwrbs.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fktsv.cn/Article/details/gyqjizebr.sHtML

composer require psr/container
来源：http://www.m.share.fktsv.cn/Article/details/gyqdedott.sHtML

[U76] PHP：简单路由
来源：http://blog.tarul.cn/Article/details/goukydyen.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fktsv.cn/Article/details/gweehiiuy.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fktsv.cn/Article/details/ggoplutqs.sHtML

composer require twig/twig
来源：http://www.m.share.tarul.cn/Article/details/gryqiidef.sHtML

[U78] PHP：单元测试
来源：http://www.share.epnwcf.com/Article/details/ghooulqox.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.tarul.cn/Article/details/glotuyxka.sHtML

[U79] PHP：静态分析
来源：http://3g.vehdjk.com/Article/details/gixgpeggl.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.epnwcf.com/Article/details/guuglwkwk.sHtML

[U80] PHP：代码规范修复
来源：http://3g.yfazqb.com/Article/details/gptuvtdkz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fktsv.cn/Article/details/gglzawhly.sHtML

[U81] JS：初始化项目
来源：http://www.blog.epnwcf.com/Article/details/gutrzaczc.sHtML

npm init -y;  npm i express
来源：http://blog.yfazqb.com/Article/details/gxgnpukyr.sHtML

[U82] JS：package.json 脚本
来源：http://3g.yfazqb.com/Article/details/gsbegafrt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.vehdjk.com/Article/details/gntdfhhez.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.yfazqb.com/Article/details/gwoatptrn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.epnwcf.com/Article/details/glbhkatid.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fktsv.cn/Article/details/gdomdhhof.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.bbcook.cn/Article/details/gyrtvhsrw.sHtML

[U85] JS：可选链
来源：http://wap.vehdjk.com/Article/details/gnecqsvod.sHtML

a?.b?.c
来源：http://3g.bbcook.cn/Article/details/gppmhknis.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fktsv.cn/Article/details/gslxssimg.sHtML

a ?? b
来源：http://read.share.vehdjk.com/Article/details/gxakqxgjh.sHtML

[U87] JS：解构默认值
来源：http://3g.fktsv.cn/Article/details/gaytpxzae.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.tarul.cn/Article/details/gtlbaivsn.sHtML

[U88] JS：对象展开合并
来源：http://3g.yfazqb.com/Article/details/gyerkjvzj.sHtML

{ ...a, ...b }
来源：http://read.share.vehdjk.com/Article/details/gxnuhuemr.sHtML

[U89] JS：数组去重
来源：http://www.m.share.vehdjk.com/Article/details/gjnprobbd.sHtML

[...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/goekfkrii.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fktsv.cn/Article/details/gxesxibjz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gxriyasxu.sHtML

[U91] JS：对象键值遍历
来源：http://3g.tarul.cn/Article/details/gzvurcmdi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.sjlbkw.cn/Article/details/glwdnljqf.sHtML

[U92] JS：深拷贝
来源：http://www.share.fktsv.cn/Article/details/gnyqlwhhl.sHtML

structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gaiztbxaw.sHtML

[U93] JS：模板字符串
来源：http://www.blog.sjlbkw.cn/Article/details/geppqcjwf.sHtML

`共 ${n} 条`
来源：http://mobile.yfazqb.com/Article/details/gsfuueuml.sHtML

[U94] JS：箭头函数
来源：http://wap.yfazqb.com/Article/details/gdtjnfpbc.sHtML

const double = x => x * 2;
来源：http://mobile.bbcook.cn/Article/details/gkjydoeea.sHtML

[U95] JS：Promise 包装
来源：http://wap.fktsv.cn/Article/details/gtrbuffzp.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.tarul.cn/Article/details/gtpatjaol.sHtML

[U96] JS：async/await 与异常
来源：http://3g.vehdjk.com/Article/details/gzronkwoc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/grlvkzbwg.sHtML

[U97] JS：并发请求
来源：http://www.blog.fktsv.cn/Article/details/garxpnxvy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gabxugktx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.epnwcf.com/Article/details/gcgxwgssl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fktsv.cn/Article/details/gqintcnqj.sHtML

[U99] JS：事件监听
来源：http://baike.yfazqb.com/Article/details/glmbgazmf.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.yfazqb.com/Article/details/giqaihquw.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.yfazqb.com/Article/details/gbkanyhxa.sHtML

document.querySelector(".item")
来源：http://www.blog.yfazqb.com/Article/details/gaxutxioo.sHtML

[U101] JS：classList 操作
来源：http://www.blog.tarul.cn/Article/details/geqbaakox.sHtML

el.classList.toggle("active")
来源：http://wap.vehdjk.com/Article/details/ggpstxacl.sHtML

[U102] JS：本地存储
来源：http://www.share.fktsv.cn/Article/details/gwjipkyld.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.sjlbkw.cn/Article/details/grinvivaw.sHtML

[U103] JS：定时器
来源：http://baike.yfazqb.com/Article/details/gmndlqxye.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.sjlbkw.cn/Article/details/giuuqcjzk.sHtML

[U104] JS：防抖
来源：http://read.share.epnwcf.com/Article/details/gpebcrhyn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gnlailcpk.sHtML

[U105] JS：节流
来源：http://www.blog.vehdjk.com/Article/details/glkujchdz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.bbcook.cn/Article/details/gagxtshmy.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gtzarashd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fktsv.cn/Article/details/gxmfnkprh.sHtML

[U107] JS：数字千分位
来源：http://wap.fktsv.cn/Article/details/gcfmaqrnd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.vehdjk.com/Article/details/gulpwywja.sHtML

[U108] JS：随机整数
来源：http://www.share.tarul.cn/Article/details/gndrepryb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fktsv.cn/Article/details/gkthhnszb.sHtML

[U109] JS：数组分组
来源：http://blog.sjlbkw.cn/Article/details/gmmzdvkfk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gczmgxzrr.sHtML

[U110] JS：数组分块
来源：http://baike.yfazqb.com/Article/details/grnngmqvg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.epnwcf.com/Article/details/gfikqgzhq.sHtML

[U111] JS：对象转 Map
来源：http://mobile.sjlbkw.cn/Article/details/gvgebfbux.sHtML

new Map(Object.entries(obj))
来源：http://read.share.bbcook.cn/Article/details/gdhrseswb.sHtML

[U112] JS：字符串补位
来源：http://www.share.epnwcf.com/Article/details/gxcvuiblt.sHtML

"7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/ggfzfljth.sHtML

[U113] JS：正则替换全部
来源：http://www.share.tarul.cn/Article/details/gwvqlrbhs.sHtML

s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gqyonvaea.sHtML

[U114] JS：JSON 深比较
来源：http://3g.tarul.cn/Article/details/gkizwdadl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gwdjngaez.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gqnnzwdyn.sHtML

crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gdwsgegpy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.tarul.cn/Article/details/grwzycvau.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.bbcook.cn/Article/details/gcloxsksl.sHtML

[U117] JS：单元测试
来源：http://m.share.tarul.cn/Article/details/govprgybk.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.epnwcf.com/Article/details/gzxslwlgy.sHtML

[U118] JS：开发服务器
来源：http://www.blog.yfazqb.com/Article/details/gxyffemzw.sHtML

npm i -D vite;  npx vite
来源：http://baike.tarul.cn/Article/details/gxchuomyc.sHtML

[U119] JS：生产构建
来源：http://www.share.yfazqb.com/Article/details/gvaqdxvat.sHtML

npx vite build
来源：http://mobile.epnwcf.com/Article/details/gjflivjas.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fktsv.cn/Article/details/galopxxrh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fktsv.cn/Article/details/gppvszqjw.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrilmjwu.sHtML

统计汇总
来源：http://www.share.bbcook.cn/Article/details/gyizuqzbg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grkgywewe.sHtML

按语言统计（条）：
来源：http://3g.tarul.cn/Article/details/gqcwqmqzg.sHtML

Python ......... 252
来源：http://baike.bbcook.cn/Article/details/gmnwovvsh.sHtML

PHP ............ 252
来源：http://3g.fktsv.cn/Article/details/gsdowntct.sHtML

JavaScript ..... 252
来源：http://wap.epnwcf.com/Article/details/gafexphyd.sHtML

TypeScript ..... 212
来源：http://wap.sjlbkw.cn/Article/details/gzblmryuw.sHtML

Java ........... 212
来源：http://www.m.share.fktsv.cn/Article/details/guhixvqmd.sHtML

Go ............. 212
来源：http://read.share.fktsv.cn/Article/details/gbzrgnlza.sHtML

Ruby ........... 212
来源：http://3g.sjlbkw.cn/Article/details/gruuwwvnq.sHtML

C# ............. 212
来源：http://m.share.vehdjk.com/Article/details/gqjrvgptz.sHtML

C .............. 30
来源：http://www.share.fktsv.cn/Article/details/gnqzxskmh.sHtML

C++ ............ 30
来源：http://www.blog.epnwcf.com/Article/details/gpkcndwgs.sHtML

SQL ............ 90
来源：http://www.m.share.bbcook.cn/Article/details/gyloljezt.sHtML

Bash ........... 80
来源：http://read.share.sjlbkw.cn/Article/details/grkexevfv.sHtML

Kotlin ......... 15
来源：http://baike.sjlbkw.cn/Article/details/gukirpwfa.sHtML

Swift .......... 15
来源：http://read.share.tarul.cn/Article/details/gsnhwexwb.sHtML

Lua ............ 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmezhgju.sHtML

Perl ........... 10
来源：http://blog.yfazqb.com/Article/details/gxhxlkiqc.sHtML

Scala .......... 10
来源：http://www.share.epnwcf.com/Article/details/gmtdqvoum.sHtML

------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gexqfxmvh.sHtML

合计 ........... 2106 条
来源：http://baike.yfazqb.com/Article/details/gfdjxpydg.sHtML

按章节统计：
来源：http://www.m.share.bbcook.cn/Article/details/gmwrymtzl.sHtML


<!-- 参考信息 -->