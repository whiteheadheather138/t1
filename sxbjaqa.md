代发 wailian999

[T45] Perl：数组遍历
来源：http://www.blog.vehdjk.com/Article/details/geaxhgubx.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fktsv.cn/Article/details/gixeahgwp.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.epnwcf.com/Article/details/gszaqjkgv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.epnwcf.com/Article/details/gxexwbwpp.sHtML

[T47] Perl：正则捕获
来源：http://www.share.sjlbkw.cn/Article/details/gmaxasrjy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.yfazqb.com/Article/details/gglgwqgdk.sHtML

[T48] Perl：正则替换
来源：http://wap.yfazqb.com/Article/details/gotgbirrp.sHtML

$s =~ s/old/new/g;
来源：http://wap.bbcook.cn/Article/details/ggpbjkkev.sHtML

[T49] Perl：函数
来源：http://www.share.bbcook.cn/Article/details/gzvofcgmq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gxxsjocfd.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gautoipjd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.epnwcf.com/Article/details/gwtmpcfrs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.epnwcf.com/Article/details/gnrucvmpb.sHtML

[T51] Scala：Hello World
来源：http://www.share.tarul.cn/Article/details/gclwpwwyl.sHtML

println("Hello")
来源：http://wap.tarul.cn/Article/details/gxybabklt.sHtML

[T52] Scala：变量
来源：http://m.share.epnwcf.com/Article/details/gebixskoe.sHtML

val a = 1;  var b = 2
来源：http://read.share.tarul.cn/Article/details/gourmqmyp.sHtML

[T53] Scala：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gpoyrfsab.sHtML

s"值: $b"
来源：http://baike.epnwcf.com/Article/details/gjvctsalk.sHtML

[T54] Scala：集合映射
来源：http://m.share.tarul.cn/Article/details/gwflvqfjx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.sjlbkw.cn/Article/details/grnxvbmca.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/gfjxzzuxx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fktsv.cn/Article/details/gxrrcfuxy.sHtML

[T56] Scala：样例类
来源：http://www.blog.fktsv.cn/Article/details/gbttnisif.sHtML

case class User(name: String, age: Int)
来源：http://baike.bbcook.cn/Article/details/gvwaycgyu.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/goxvsmxxu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.bbcook.cn/Article/details/gckrcteic.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.epnwcf.com/Article/details/gaywqguax.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.sjlbkw.cn/Article/details/gjxvnpfnv.sHtML

[T59] Scala：循环
来源：http://wap.yfazqb.com/Article/details/gnkijndyz.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.yfazqb.com/Article/details/gwixwqbkl.sHtML

[T60] Scala：折叠
来源：http://read.share.vehdjk.com/Article/details/gkjonwakl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.sjlbkw.cn/Article/details/gwsadoqni.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdawtgpxs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/gaerwvvvr.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gyfuadlps.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.tarul.cn/Article/details/gdsvtvksa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.epnwcf.com/Article/details/gzscquxox.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.sjlbkw.cn/Article/details/gukxlxfln.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.vehdjk.com/Article/details/ghattsjcs.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fktsv.cn/Article/details/gxxxexxvm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.epnwcf.com/Article/details/gxvgllogo.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.vehdjk.com/Article/details/gkxjwwdce.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.yfazqb.com/Article/details/gjsmntdet.sHtML

[U05] Py：列表去重且保序
来源：http://wap.sjlbkw.cn/Article/details/gripopmnh.sHtML

list(dict.fromkeys(arr))
来源：http://blog.epnwcf.com/Article/details/gbrvvzgbj.sHtML

[U06] Py：合并两个字典
来源：http://mobile.bbcook.cn/Article/details/gieottwql.sHtML

{**a, **b}
来源：http://baike.vehdjk.com/Article/details/ghmbhujdr.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fktsv.cn/Article/details/ggjahqnud.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fktsv.cn/Article/details/gtpfraleq.sHtML

[U08] Py：展平二维列表
来源：http://baike.fktsv.cn/Article/details/gskurjrxi.sHtML

[y for x in nested for y in x]
来源：http://www.blog.vehdjk.com/Article/details/gwvzufbtj.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/gnutalwii.sHtML

max(d, key=d.get)
来源：http://baike.bbcook.cn/Article/details/gbuvisgps.sHtML

[U10] Py：按值排序字典
来源：http://baike.epnwcf.com/Article/details/gutbwyyfm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.tarul.cn/Article/details/gglyknkwh.sHtML

[U11] Py：生成器表达式
来源：http://3g.bbcook.cn/Article/details/ghwpmuhsb.sHtML

(x * 2 for x in arr)
来源：http://blog.yfazqb.com/Article/details/geszcjsbp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.sjlbkw.cn/Article/details/gzaxoarsx.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.bbcook.cn/Article/details/gbahenawt.sHtML

[U13] Py：固定长度队列
来源：http://mobile.vehdjk.com/Article/details/ggihyjvoj.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/gzotytmnx.sHtML

[U14] Py：分组收集到列表
来源：http://3g.vehdjk.com/Article/details/gdpqoghwi.sHtML

defaultdict(list)
来源：http://wap.epnwcf.com/Article/details/gfobamywx.sHtML

[U15] Py：高精度计时
来源：http://wap.yfazqb.com/Article/details/gngpqhgqj.sHtML

t = time.perf_counter()
来源：http://3g.tarul.cn/Article/details/gxqtslgpm.sHtML

[U16] Py：命令行参数解析
来源：http://wap.epnwcf.com/Article/details/gpzqkqlti.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.tarul.cn/Article/details/genbqcxpq.sHtML

[U17] Py：初始化日志
来源：http://mobile.bbcook.cn/Article/details/gajqfacxj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.sjlbkw.cn/Article/details/gyghjsulv.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.yfazqb.com/Article/details/gwgmsvqzk.sHtML

pat = re.compile(r"\d+")
来源：http://wap.vehdjk.com/Article/details/gevozlavj.sHtML

[U19] Py：正则替换带回调
来源：http://blog.yfazqb.com/Article/details/gskjuwdby.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.tarul.cn/Article/details/gmrixvmkr.sHtML

[U20] Py：缓存函数结果
来源：http://wap.yfazqb.com/Article/details/gpnuihyje.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.bbcook.cn/Article/details/ghsfzywik.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.epnwcf.com/Article/details/gkdyjipnu.sHtML

@contextlib.contextmanager
来源：http://www.share.sjlbkw.cn/Article/details/gotmnusom.sHtML

[U22] Py：矩阵转置
来源：http://baike.epnwcf.com/Article/details/gvtudamkw.sHtML

list(zip(*m))
来源：http://blog.epnwcf.com/Article/details/gxrdnromw.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fktsv.cn/Article/details/gkzuqcuki.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.epnwcf.com/Article/details/gzuwtrkbw.sHtML

[U24] Py：路径操作
来源：http://3g.epnwcf.com/Article/details/gmzgzmunm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmpxqvpm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.sjlbkw.cn/Article/details/gnltdpwub.sHtML

csv.DictReader(f)
来源：http://read.share.bbcook.cn/Article/details/gdqhijupr.sHtML

[U26] Py：并发下载
来源：http://baike.yfazqb.com/Article/details/ggdoxyhpb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fktsv.cn/Article/details/gmxhpirct.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fktsv.cn/Article/details/gienogjer.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.vehdjk.com/Article/details/gvaznglfa.sHtML

[U28] Py：类型别名
来源：http://3g.vehdjk.com/Article/details/ggrsfnkex.sHtML

UserId = int
来源：http://mobile.tarul.cn/Article/details/giknfjdko.sHtML

[U29] Py：属性校验
来源：http://wap.yfazqb.com/Article/details/grqqxrexh.sHtML

@property 与 @x.setter 配合
来源：http://wap.bbcook.cn/Article/details/gdfnqmfav.sHtML

[U30] Py：数据类
来源：http://www.share.yfazqb.com/Article/details/glhcvuhcz.sHtML

@dataclass(slots=True)
来源：http://m.share.fktsv.cn/Article/details/gfoclciqm.sHtML

[U31] Py：单测
来源：http://m.share.bbcook.cn/Article/details/ggrhbusvo.sHtML

python -m pytest -q
来源：http://read.share.fktsv.cn/Article/details/gyrddoktz.sHtML

[U32] Py：代码格式化
来源：http://www.share.epnwcf.com/Article/details/gnwayscti.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.vehdjk.com/Article/details/gzjspdvun.sHtML

[U33] Py：打包发布
来源：http://mobile.tarul.cn/Article/details/gdpgflltv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.bbcook.cn/Article/details/ghttgidkl.sHtML

[U34] Py：判断编码
来源：http://baike.tarul.cn/Article/details/gekifxnxc.sHtML

chardet.detect(raw)
来源：http://baike.bbcook.cn/Article/details/gxwivgedf.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.vehdjk.com/Article/details/gpyevqedj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fktsv.cn/Article/details/gdhfvcewc.sHtML

[U36] Py：定时任务
来源：http://m.share.sjlbkw.cn/Article/details/gldissreu.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.bbcook.cn/Article/details/gsxqnkfek.sHtML

[U37] Py：读写 Excel
来源：http://wap.tarul.cn/Article/details/gndfchupe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fktsv.cn/Article/details/gzpobayrw.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fktsv.cn/Article/details/gaebdabfx.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fktsv.cn/Article/details/gpnawcmrf.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.bbcook.cn/Article/details/gvpvbgwth.sHtML

sys.stdout.isatty()
来源：http://mobile.tarul.cn/Article/details/gvkknyujr.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.bbcook.cn/Article/details/gnunmigzy.sHtML

print("err", file=sys.stderr)
来源：http://read.share.epnwcf.com/Article/details/gnuowwxpr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.sjlbkw.cn/Article/details/guwhlldxk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.epnwcf.com/Article/details/gkktqhujz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.vehdjk.com/Article/details/gbxmjgwym.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.bbcook.cn/Article/details/gkqdbntxr.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.tarul.cn/Article/details/grpbjldyw.sHtML

namespace App\Http;
来源：http://baike.vehdjk.com/Article/details/gpfzuvvpd.sHtML

[U44] PHP：开启严格类型
来源：http://3g.sjlbkw.cn/Article/details/gpjfeyacy.sHtML

declare(strict_types=1);
来源：http://baike.vehdjk.com/Article/details/glqiwwdbk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.epnwcf.com/Article/details/gnfpozwyu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/guuwnfbjf.sHtML

[U46] PHP：可空类型
来源：http://www.share.sjlbkw.cn/Article/details/grymebxxi.sHtML

?string $name = null
来源：http://3g.vehdjk.com/Article/details/gmojzjlox.sHtML

[U47] PHP：联合类型
来源：http://read.share.epnwcf.com/Article/details/gkvzzurvj.sHtML

int|string $id
来源：http://wap.fktsv.cn/Article/details/gzukaxlht.sHtML

[U48] PHP：纯枚举
来源：http://3g.epnwcf.com/Article/details/gbutrlsjs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.vehdjk.com/Article/details/gzitxxaaf.sHtML

[U49] PHP：只读属性
来源：http://baike.sjlbkw.cn/Article/details/glpszuprg.sHtML

public readonly string $name
来源：http://www.m.share.tarul.cn/Article/details/grvpxjsau.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.tarul.cn/Article/details/gcifihyoc.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fktsv.cn/Article/details/gcvrxjzml.sHtML

[U51] PHP：数组解构
来源：http://3g.tarul.cn/Article/details/gdmogozyu.sHtML

[$a, $b] = $arr;
来源：http://m.share.yfazqb.com/Article/details/gbrgqcfwd.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fktsv.cn/Article/details/gmbzyoxqy.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.bbcook.cn/Article/details/gkaglvfaa.sHtML

[U53] PHP：空合并运算符
来源：http://wap.tarul.cn/Article/details/gknjlsonz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.bbcook.cn/Article/details/gtcaelsuw.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.yfazqb.com/Article/details/grueyxlyt.sHtML

$obj?->method()
来源：http://www.share.fktsv.cn/Article/details/gvbiquqjt.sHtML

[U55] PHP：match 表达式
来源：http://m.share.vehdjk.com/Article/details/gdhrbgfpc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.bbcook.cn/Article/details/gminurmpm.sHtML

[U56] PHP：命名参数
来源：http://blog.vehdjk.com/Article/details/gvrqwzmcp.sHtML

f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gemvusmmt.sHtML

[U57] PHP：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/getpwzwry.sHtML

"值: {$a}"
来源：http://wap.bbcook.cn/Article/details/gcodjkabn.sHtML

[U58] PHP：数组三件套
来源：http://mobile.sjlbkw.cn/Article/details/goqifalum.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gwbuwqrwf.sHtML

[U59] PHP：自定义排序
来源：http://m.share.tarul.cn/Article/details/glbcjcpwc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.vehdjk.com/Article/details/gpgjvryxd.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.tarul.cn/Article/details/guarxmdih.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.yfazqb.com/Article/details/gozsfouax.sHtML

[U61] PHP：正则
来源：http://www.share.fktsv.cn/Article/details/ggfzgqhfa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/gpcjmkwod.sHtML

[U62] PHP：日期对象
来源：http://m.share.sjlbkw.cn/Article/details/gssskqtkk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.yfazqb.com/Article/details/gmzihvspo.sHtML

[U63] PHP：文件读写
来源：http://blog.epnwcf.com/Article/details/gdpugwuld.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.tarul.cn/Article/details/gnzdbqlti.sHtML

[U64] PHP：目录遍历
来源：http://mobile.yfazqb.com/Article/details/gwtktzkpo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.yfazqb.com/Article/details/guxrtqwct.sHtML

[U65] PHP：会话
来源：http://www.share.tarul.cn/Article/details/gcczemssz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/guelmnqvs.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.vehdjk.com/Article/details/gfzzjcvty.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.tarul.cn/Article/details/gegoxejku.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.bbcook.cn/Article/details/gkdgowrfx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.epnwcf.com/Article/details/gmxezyczr.sHtML

[U68] PHP：PDO 连接
来源：http://3g.bbcook.cn/Article/details/gwmbqvojd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.tarul.cn/Article/details/giejkcote.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.yfazqb.com/Article/details/gubmieikg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fktsv.cn/Article/details/gwpdpczkk.sHtML

[U70] PHP：PDO 事务
来源：http://3g.yfazqb.com/Article/details/gremrbbhw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.vehdjk.com/Article/details/gdbapdmyf.sHtML

[U71] PHP：抛出异常
来源：http://3g.tarul.cn/Article/details/ghcdjseuk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/gvxoxgqyp.sHtML

[U72] PHP：写错误日志
来源：http://www.share.vehdjk.com/Article/details/gjalsmkbq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.epnwcf.com/Article/details/glrlamhso.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.vehdjk.com/Article/details/gpamjijvv.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.vehdjk.com/Article/details/gmxrgcidc.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gzcdbplgq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.tarul.cn/Article/details/gnbqnzwzv.sHtML

[U75] PHP：依赖注入
来源：http://wap.yfazqb.com/Article/details/gjjrdsyos.sHtML

composer require psr/container
来源：http://www.blog.fktsv.cn/Article/details/gwqaijzfq.sHtML

[U76] PHP：简单路由
来源：http://3g.fktsv.cn/Article/details/gejjbhrlo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.epnwcf.com/Article/details/glhqefebh.sHtML

[U77] PHP：模板渲染
来源：http://m.share.tarul.cn/Article/details/grmsefswi.sHtML

composer require twig/twig
来源：http://read.share.fktsv.cn/Article/details/gevaluiwp.sHtML

[U78] PHP：单元测试
来源：http://read.share.tarul.cn/Article/details/gufhpibhk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fktsv.cn/Article/details/gisyuibgv.sHtML

[U79] PHP：静态分析
来源：http://www.blog.sjlbkw.cn/Article/details/gkclskram.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.yfazqb.com/Article/details/ghowxepxz.sHtML

[U80] PHP：代码规范修复
来源：http://blog.bbcook.cn/Article/details/gnsofqkbm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fktsv.cn/Article/details/gxjjrrsfw.sHtML

[U81] JS：初始化项目
来源：http://www.blog.vehdjk.com/Article/details/gbjaqrucl.sHtML

npm init -y;  npm i express
来源：http://baike.tarul.cn/Article/details/ggakgsnqm.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.yfazqb.com/Article/details/gxtmqkpzn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.bbcook.cn/Article/details/gdzavxbbm.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.bbcook.cn/Article/details/gfauepicd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.sjlbkw.cn/Article/details/gwmzzmwss.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fktsv.cn/Article/details/gmhwypjuf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.vehdjk.com/Article/details/gcwsvrzmx.sHtML

[U85] JS：可选链
来源：http://www.share.vehdjk.com/Article/details/gyhlhqjpi.sHtML

a?.b?.c
来源：http://www.blog.tarul.cn/Article/details/gqcaytoku.sHtML

[U86] JS：空值合并
来源：http://wap.sjlbkw.cn/Article/details/gcwzhkixv.sHtML

a ?? b
来源：http://blog.fktsv.cn/Article/details/ghaikhoqk.sHtML

[U87] JS：解构默认值
来源：http://read.share.bbcook.cn/Article/details/gwxxwpogw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.tarul.cn/Article/details/gfvwxqtkm.sHtML

[U88] JS：对象展开合并
来源：http://wap.sjlbkw.cn/Article/details/gddwvonxs.sHtML

{ ...a, ...b }
来源：http://m.share.bbcook.cn/Article/details/gnyrdwfyi.sHtML

[U89] JS：数组去重
来源：http://mobile.epnwcf.com/Article/details/gcqrdnpgh.sHtML

[...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gimlqfsxn.sHtML

[U90] JS：数字数组排序
来源：http://www.share.epnwcf.com/Article/details/gknvfrxtn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gjitfpqxz.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.epnwcf.com/Article/details/gyscwowwe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fktsv.cn/Article/details/gbawwpfgo.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gdixuibkk.sHtML

structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gghitkijh.sHtML

[U93] JS：模板字符串
来源：http://www.share.tarul.cn/Article/details/gpokuxpmb.sHtML

`共 ${n} 条`
来源：http://wap.fktsv.cn/Article/details/gdlkklgsn.sHtML

[U94] JS：箭头函数
来源：http://www.share.epnwcf.com/Article/details/gzupfhxkh.sHtML

const double = x => x * 2;
来源：http://www.m.share.bbcook.cn/Article/details/gcumxvngb.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fktsv.cn/Article/details/gxprjqllq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fktsv.cn/Article/details/gruayldab.sHtML

[U96] JS：async/await 与异常
来源：http://wap.epnwcf.com/Article/details/groyiixch.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gmulurmlw.sHtML

[U97] JS：并发请求
来源：http://read.share.fktsv.cn/Article/details/gympagfea.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gfqgpmcxg.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.epnwcf.com/Article/details/gpoyuvthd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.tarul.cn/Article/details/gnjukoyrq.sHtML

[U99] JS：事件监听
来源：http://www.m.share.vehdjk.com/Article/details/gsefgpdyf.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fktsv.cn/Article/details/gmahpeubw.sHtML

[U100] JS：DOM 查询
来源：http://3g.bbcook.cn/Article/details/ggzccicqy.sHtML

document.querySelector(".item")
来源：http://baike.fktsv.cn/Article/details/gxcyliwfy.sHtML

[U101] JS：classList 操作
来源：http://mobile.epnwcf.com/Article/details/gnvesvgdl.sHtML

el.classList.toggle("active")
来源：http://www.share.fktsv.cn/Article/details/gtxndsdkg.sHtML

[U102] JS：本地存储
来源：http://3g.bbcook.cn/Article/details/gmmzxetpb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.epnwcf.com/Article/details/gqiaeutig.sHtML

[U103] JS：定时器
来源：http://m.share.fktsv.cn/Article/details/gytfxgijp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fktsv.cn/Article/details/gitrxbahk.sHtML

[U104] JS：防抖
来源：http://read.share.epnwcf.com/Article/details/ggzrzvszf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/goucjkmlm.sHtML

[U105] JS：节流
来源：http://3g.vehdjk.com/Article/details/gnzullprk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.sjlbkw.cn/Article/details/gevvezrik.sHtML

[U106] JS：日期格式化
来源：http://mobile.tarul.cn/Article/details/gehheevrq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.epnwcf.com/Article/details/geavugkug.sHtML

[U107] JS：数字千分位
来源：http://read.share.fktsv.cn/Article/details/gfesxvfmh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.tarul.cn/Article/details/guighqmvy.sHtML

[U108] JS：随机整数
来源：http://m.share.vehdjk.com/Article/details/gydodrpmc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.vehdjk.com/Article/details/ganxxqssl.sHtML

[U109] JS：数组分组
来源：http://www.blog.bbcook.cn/Article/details/gbsxrxvtf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.yfazqb.com/Article/details/gmsmduwhq.sHtML

[U110] JS：数组分块
来源：http://3g.sjlbkw.cn/Article/details/gtlynulsn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.yfazqb.com/Article/details/gooopdzbk.sHtML

[U111] JS：对象转 Map
来源：http://mobile.sjlbkw.cn/Article/details/gfrjqelxo.sHtML

new Map(Object.entries(obj))
来源：http://blog.tarul.cn/Article/details/gquudkomm.sHtML

[U112] JS：字符串补位
来源：http://mobile.yfazqb.com/Article/details/gunsotrir.sHtML

"7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gnxaamujc.sHtML

[U113] JS：正则替换全部
来源：http://blog.bbcook.cn/Article/details/gexjnxgek.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gzewdfdan.sHtML

[U114] JS：JSON 深比较
来源：http://3g.vehdjk.com/Article/details/gebhihtot.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.epnwcf.com/Article/details/gmgbaivik.sHtML

[U115] JS：生成 UUID
来源：http://baike.fktsv.cn/Article/details/gxtnkiicj.sHtML

crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/gbmnyqgnu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.epnwcf.com/Article/details/gwelkoetu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.sjlbkw.cn/Article/details/guuvemyta.sHtML

[U117] JS：单元测试
来源：http://www.blog.vehdjk.com/Article/details/giiqiaybp.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.tarul.cn/Article/details/gvlplynyy.sHtML

[U118] JS：开发服务器
来源：http://www.share.fktsv.cn/Article/details/grfwlbhze.sHtML

npm i -D vite;  npx vite
来源：http://www.share.yfazqb.com/Article/details/grvuvdcjl.sHtML

[U119] JS：生产构建
来源：http://wap.bbcook.cn/Article/details/gdsbwhajw.sHtML

npx vite build
来源：http://wap.sjlbkw.cn/Article/details/gkbrhplur.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.vehdjk.com/Article/details/gmdxeyrjs.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fktsv.cn/Article/details/gfxrttvvs.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gdkicsblu.sHtML

统计汇总
来源：http://baike.fktsv.cn/Article/details/gvtnlgtnu.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gotbdhesr.sHtML

按语言统计（条）：
来源：http://blog.sjlbkw.cn/Article/details/ghgcgfgxi.sHtML

Python ......... 252
来源：http://www.share.sjlbkw.cn/Article/details/gtpgwuwwi.sHtML

PHP ............ 252
来源：http://www.m.share.fktsv.cn/Article/details/gymcgqnus.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/ggdlgqgcf.sHtML

TypeScript ..... 212
来源：http://3g.fktsv.cn/Article/details/gbbdupbot.sHtML

Java ........... 212
来源：http://read.share.fktsv.cn/Article/details/gttcbudvb.sHtML

Go ............. 212
来源：http://blog.sjlbkw.cn/Article/details/golrulwrd.sHtML

Ruby ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/guaqqjnrj.sHtML

C# ............. 212
来源：http://blog.tarul.cn/Article/details/gnikqunns.sHtML

C .............. 30
来源：http://m.share.vehdjk.com/Article/details/gpjgmbgfi.sHtML

C++ ............ 30
来源：http://mobile.bbcook.cn/Article/details/gjfupeabt.sHtML

SQL ............ 90
来源：http://3g.sjlbkw.cn/Article/details/gcguytftc.sHtML

Bash ........... 80
来源：http://wap.vehdjk.com/Article/details/gebsvxmzm.sHtML

Kotlin ......... 15
来源：http://wap.sjlbkw.cn/Article/details/gbscmjnsd.sHtML

Swift .......... 15
来源：http://baike.tarul.cn/Article/details/gvwqfvhgq.sHtML

Lua ............ 10
来源：http://www.blog.bbcook.cn/Article/details/gjkyykech.sHtML

Perl ........... 10
来源：http://baike.bbcook.cn/Article/details/ghjcogykt.sHtML

Scala .......... 10
来源：http://mobile.sjlbkw.cn/Article/details/grzmesnlk.sHtML

------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gxmnpbuve.sHtML

合计 ........... 2106 条
来源：http://www.share.tarul.cn/Article/details/gacyjmewy.sHtML

按章节统计：
来源：http://www.m.share.yfazqb.com/Article/details/gczczgcwx.sHtML


<!-- 参考信息 -->