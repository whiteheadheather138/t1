代发 wailian999

[T43] Perl：字符串插值
来源：http://blog.fktsv.cn/Article/details/gcaagorro.sHtML

"值: $a"
来源：http://blog.bbcook.cn/Article/details/gskapeinz.sHtML

[T44] Perl：条件
来源：http://read.share.yfazqb.com/Article/details/gcotoiamw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.tarul.cn/Article/details/gpkozufdw.sHtML

[T45] Perl：数组遍历
来源：http://mobile.bbcook.cn/Article/details/gxdhsxgmw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.bbcook.cn/Article/details/gpattgkwr.sHtML

[T46] Perl：哈希操作
来源：http://m.share.yfazqb.com/Article/details/gusiuhwuv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fktsv.cn/Article/details/gaytbstso.sHtML

[T47] Perl：正则捕获
来源：http://www.share.bbcook.cn/Article/details/gvemlftyl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsksnpvbp.sHtML

[T48] Perl：正则替换
来源：http://3g.yfazqb.com/Article/details/gzjkyurhl.sHtML

$s =~ s/old/new/g;
来源：http://3g.vehdjk.com/Article/details/gkodrjvjq.sHtML

[T49] Perl：函数
来源：http://wap.fktsv.cn/Article/details/gtpybrglm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gfhkzqnkz.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gsvctzrag.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.tarul.cn/Article/details/gtxcuxofi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.epnwcf.com/Article/details/gnixkupfo.sHtML

[T51] Scala：Hello World
来源：http://blog.fktsv.cn/Article/details/gwftlpvsz.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gfodbvcbw.sHtML

[T52] Scala：变量
来源：http://m.share.tarul.cn/Article/details/gfuksemzr.sHtML

val a = 1;  var b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gzgydarwm.sHtML

[T53] Scala：字符串插值
来源：http://wap.epnwcf.com/Article/details/gwqtzvqhj.sHtML

s"值: $b"
来源：http://mobile.tarul.cn/Article/details/gwmgclgvd.sHtML

[T54] Scala：集合映射
来源：http://3g.tarul.cn/Article/details/gniueywdf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.vehdjk.com/Article/details/gnsskvtef.sHtML

[T55] Scala：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gjpnuxgnc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.vehdjk.com/Article/details/gotyfaenq.sHtML

[T56] Scala：样例类
来源：http://wap.vehdjk.com/Article/details/glqgleekq.sHtML

case class User(name: String, age: Int)
来源：http://blog.tarul.cn/Article/details/gheyfzvxi.sHtML

[T57] Scala：模式匹配
来源：http://www.share.bbcook.cn/Article/details/gragwclbv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.yfazqb.com/Article/details/gfhrkqvqe.sHtML

[T58] Scala：函数定义
来源：http://www.share.fktsv.cn/Article/details/gkfuqqjjv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.tarul.cn/Article/details/gdldgizwv.sHtML

[T59] Scala：循环
来源：http://blog.yfazqb.com/Article/details/gitlhphmt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gbqmnclbv.sHtML

[T60] Scala：折叠
来源：http://wap.tarul.cn/Article/details/grpihxvwk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.tarul.cn/Article/details/gakqstwbb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjbqjiunt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.tarul.cn/Article/details/gswwaujmd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/geskolcla.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.bbcook.cn/Article/details/gvndivukj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.vehdjk.com/Article/details/gfffvfoxw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.yfazqb.com/Article/details/gcjhjbjcv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fktsv.cn/Article/details/gyefgomog.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fktsv.cn/Article/details/gehxkukzb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fktsv.cn/Article/details/gvsszvyxn.sHtML

[U04] Py：变量调试打印
来源：http://blog.epnwcf.com/Article/details/gghnustvb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.bbcook.cn/Article/details/gmkqbjdxz.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/gemzmesxm.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.epnwcf.com/Article/details/goduikuma.sHtML

[U06] Py：合并两个字典
来源：http://wap.sjlbkw.cn/Article/details/gyqkefcvv.sHtML

{**a, **b}
来源：http://www.share.sjlbkw.cn/Article/details/gdsaglrsk.sHtML

[U07] Py：反转字典键值
来源：http://3g.fktsv.cn/Article/details/gezbnozsi.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.tarul.cn/Article/details/gtgksngtz.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.epnwcf.com/Article/details/gwpazyiji.sHtML

[y for x in nested for y in x]
来源：http://3g.vehdjk.com/Article/details/gjglasyqo.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.yfazqb.com/Article/details/gswzcfuhw.sHtML

max(d, key=d.get)
来源：http://read.share.bbcook.cn/Article/details/ggnebsxss.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.bbcook.cn/Article/details/gvtlodxmz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.epnwcf.com/Article/details/gcpvrnemh.sHtML

[U11] Py：生成器表达式
来源：http://baike.bbcook.cn/Article/details/gjpyhjuux.sHtML

(x * 2 for x in arr)
来源：http://wap.vehdjk.com/Article/details/gdiselbui.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.vehdjk.com/Article/details/gansrynye.sHtML

Counter(arr).most_common(3)
来源：http://baike.yfazqb.com/Article/details/gzvzzbocj.sHtML

[U13] Py：固定长度队列
来源：http://www.share.sjlbkw.cn/Article/details/glksfcsso.sHtML

deque(maxlen=10)
来源：http://3g.tarul.cn/Article/details/gbiuwdhho.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fktsv.cn/Article/details/gwenwjuad.sHtML

defaultdict(list)
来源：http://m.share.yfazqb.com/Article/details/grxicshxi.sHtML

[U15] Py：高精度计时
来源：http://www.blog.vehdjk.com/Article/details/gcboqdaug.sHtML

t = time.perf_counter()
来源：http://m.share.vehdjk.com/Article/details/gkhhxnezy.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.yfazqb.com/Article/details/gnapcfuky.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.bbcook.cn/Article/details/giziltysq.sHtML

[U17] Py：初始化日志
来源：http://3g.vehdjk.com/Article/details/gfffsisji.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fktsv.cn/Article/details/gswqavour.sHtML

[U18] Py：预编译正则
来源：http://baike.fktsv.cn/Article/details/gjzrvdfmt.sHtML

pat = re.compile(r"\d+")
来源：http://3g.sjlbkw.cn/Article/details/gwsjaebzu.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.bbcook.cn/Article/details/gyiwawtzv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.epnwcf.com/Article/details/gpaehafwz.sHtML

[U20] Py：缓存函数结果
来源：http://3g.vehdjk.com/Article/details/gttzwujal.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.vehdjk.com/Article/details/gotbgfalc.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.epnwcf.com/Article/details/gpkyypceo.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/gcjaljmod.sHtML

[U22] Py：矩阵转置
来源：http://mobile.epnwcf.com/Article/details/gfedzwluh.sHtML

list(zip(*m))
来源：http://www.m.share.fktsv.cn/Article/details/gueirzoud.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.yfazqb.com/Article/details/gwinfljii.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.sjlbkw.cn/Article/details/ghezmbrmk.sHtML

[U24] Py：路径操作
来源：http://m.share.bbcook.cn/Article/details/gaiukuunk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/gyyyrhegh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.yfazqb.com/Article/details/gfevqtdpj.sHtML

csv.DictReader(f)
来源：http://www.share.bbcook.cn/Article/details/gtqscprtj.sHtML

[U26] Py：并发下载
来源：http://wap.tarul.cn/Article/details/glunyvxap.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.yfazqb.com/Article/details/ghjqhykgx.sHtML

[U27] Py：异步 HTTP
来源：http://baike.sjlbkw.cn/Article/details/gexxhrekr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.vehdjk.com/Article/details/gykuychwd.sHtML

[U28] Py：类型别名
来源：http://3g.bbcook.cn/Article/details/gcifpaimj.sHtML

UserId = int
来源：http://m.share.vehdjk.com/Article/details/gqoenwlxh.sHtML

[U29] Py：属性校验
来源：http://read.share.sjlbkw.cn/Article/details/gkrrwurwf.sHtML

@property 与 @x.setter 配合
来源：http://wap.bbcook.cn/Article/details/gmkdblvjz.sHtML

[U30] Py：数据类
来源：http://3g.sjlbkw.cn/Article/details/gjbizlrvg.sHtML

@dataclass(slots=True)
来源：http://baike.tarul.cn/Article/details/gykvxtqeo.sHtML

[U31] Py：单测
来源：http://mobile.sjlbkw.cn/Article/details/grmpxoqwn.sHtML

python -m pytest -q
来源：http://baike.bbcook.cn/Article/details/gofuqnsvn.sHtML

[U32] Py：代码格式化
来源：http://www.share.epnwcf.com/Article/details/gywpzobhc.sHtML

ruff format . && ruff check --fix .
来源：http://3g.vehdjk.com/Article/details/ggizpfgah.sHtML

[U33] Py：打包发布
来源：http://www.m.share.sjlbkw.cn/Article/details/gezdjzpih.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.yfazqb.com/Article/details/gdsecqguo.sHtML

[U34] Py：判断编码
来源：http://blog.bbcook.cn/Article/details/glcbcfpsv.sHtML

chardet.detect(raw)
来源：http://m.share.epnwcf.com/Article/details/gekzofmvb.sHtML

[U35] Py：发送邮件
来源：http://m.share.epnwcf.com/Article/details/guxvdehxr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.bbcook.cn/Article/details/gfdvwylpj.sHtML

[U36] Py：定时任务
来源：http://read.share.sjlbkw.cn/Article/details/ghkimqxfk.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.epnwcf.com/Article/details/gljskrfdq.sHtML

[U37] Py：读写 Excel
来源：http://baike.tarul.cn/Article/details/gwysvfdhe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fktsv.cn/Article/details/gnjtrnrxl.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.yfazqb.com/Article/details/glgswmgzd.sHtML

Path(__file__).resolve().parent
来源：http://3g.vehdjk.com/Article/details/gapyykbhp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fktsv.cn/Article/details/greelhqua.sHtML

sys.stdout.isatty()
来源：http://www.share.epnwcf.com/Article/details/gldcaowld.sHtML

[U40] Py：打印到标准错误
来源：http://blog.sjlbkw.cn/Article/details/ghwdhusym.sHtML

print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/gykrxgnce.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.yfazqb.com/Article/details/ghqyvavoq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.sjlbkw.cn/Article/details/gxdglcgkk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.tarul.cn/Article/details/gyvdfasie.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.vehdjk.com/Article/details/gsvxlotld.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/giltsqhyo.sHtML

namespace App\Http;
来源：http://blog.sjlbkw.cn/Article/details/gausrkwkk.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.bbcook.cn/Article/details/gvicsckle.sHtML

declare(strict_types=1);
来源：http://mobile.bbcook.cn/Article/details/gfrmckcnf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.vehdjk.com/Article/details/gmkewbwzk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gtmbfalog.sHtML

[U46] PHP：可空类型
来源：http://www.share.sjlbkw.cn/Article/details/gmxpiluwf.sHtML

?string $name = null
来源：http://read.share.yfazqb.com/Article/details/gnhfeplrf.sHtML

[U47] PHP：联合类型
来源：http://m.share.yfazqb.com/Article/details/gphvmmbvd.sHtML

int|string $id
来源：http://baike.epnwcf.com/Article/details/gooxjtfdp.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.tarul.cn/Article/details/ghekhhsle.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.bbcook.cn/Article/details/gzmgtdljd.sHtML

[U49] PHP：只读属性
来源：http://read.share.tarul.cn/Article/details/gyavyifoc.sHtML

public readonly string $name
来源：http://3g.fktsv.cn/Article/details/gupixlyxe.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fktsv.cn/Article/details/gvviwygow.sHtML

public function __construct(private int $id) {}
来源：http://wap.bbcook.cn/Article/details/gnsanbanf.sHtML

[U51] PHP：数组解构
来源：http://read.share.epnwcf.com/Article/details/gavshlddx.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fktsv.cn/Article/details/gpunhoasv.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gcwxznrai.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.vehdjk.com/Article/details/gqvbmzqdp.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.vehdjk.com/Article/details/gkmtkpzhm.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.vehdjk.com/Article/details/gqigakhnn.sHtML

[U54] PHP：空安全调用
来源：http://m.share.bbcook.cn/Article/details/gteqgbuhk.sHtML

$obj?->method()
来源：http://blog.yfazqb.com/Article/details/gngmpljue.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gsjdrjyjo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.epnwcf.com/Article/details/gmskpkfyr.sHtML

[U56] PHP：命名参数
来源：http://blog.vehdjk.com/Article/details/gevxlscth.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjthuturb.sHtML

[U57] PHP：字符串插值
来源：http://baike.fktsv.cn/Article/details/gsbstfaif.sHtML

"值: {$a}"
来源：http://read.share.tarul.cn/Article/details/gwasslzcv.sHtML

[U58] PHP：数组三件套
来源：http://www.share.vehdjk.com/Article/details/gydrzzbcx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.tarul.cn/Article/details/gkzoactfr.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.sjlbkw.cn/Article/details/gtopboslj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/gtpmypvtj.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.epnwcf.com/Article/details/gawyszlvz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.vehdjk.com/Article/details/gfmwkikco.sHtML

[U61] PHP：正则
来源：http://baike.epnwcf.com/Article/details/gfeuqcxsw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/glwmvjlhm.sHtML

[U62] PHP：日期对象
来源：http://read.share.tarul.cn/Article/details/gibibjegy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.sjlbkw.cn/Article/details/gbicftmim.sHtML

[U63] PHP：文件读写
来源：http://www.share.yfazqb.com/Article/details/gjfkycbjq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.tarul.cn/Article/details/gifpclzxc.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.bbcook.cn/Article/details/gnxwgzmjd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.vehdjk.com/Article/details/gbioidflq.sHtML

[U65] PHP：会话
来源：http://read.share.sjlbkw.cn/Article/details/gdbhgrrig.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gnyrbpjnp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fktsv.cn/Article/details/gnnryqyjv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.epnwcf.com/Article/details/glptwfyxo.sHtML

[U67] PHP：处理文件上传
来源：http://wap.tarul.cn/Article/details/gbdjynevt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.yfazqb.com/Article/details/grcsmnbne.sHtML

[U68] PHP：PDO 连接
来源：http://wap.bbcook.cn/Article/details/gcskedbej.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.bbcook.cn/Article/details/gdikbxtcu.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.yfazqb.com/Article/details/gnhgowpdv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fktsv.cn/Article/details/gcoylexev.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.epnwcf.com/Article/details/gxtijfoya.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fktsv.cn/Article/details/gvtjasjoo.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gpbdmuytr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.vehdjk.com/Article/details/gsvbbkquq.sHtML

[U72] PHP：写错误日志
来源：http://mobile.tarul.cn/Article/details/gfckxuapb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.bbcook.cn/Article/details/ghcwucydt.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fktsv.cn/Article/details/goryvvwzj.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.bbcook.cn/Article/details/gslpzmnab.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.epnwcf.com/Article/details/gpnbkrkag.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fktsv.cn/Article/details/gnyirnzao.sHtML

[U75] PHP：依赖注入
来源：http://www.share.yfazqb.com/Article/details/ggxmvwqkj.sHtML

composer require psr/container
来源：http://www.share.yfazqb.com/Article/details/gqmzxkydv.sHtML

[U76] PHP：简单路由
来源：http://www.blog.tarul.cn/Article/details/ghiyfojsb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.epnwcf.com/Article/details/gsoakemyv.sHtML

[U77] PHP：模板渲染
来源：http://baike.yfazqb.com/Article/details/grtuxlnjb.sHtML

composer require twig/twig
来源：http://www.m.share.vehdjk.com/Article/details/gxfbfvyxc.sHtML

[U78] PHP：单元测试
来源：http://mobile.yfazqb.com/Article/details/gyynvujft.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fktsv.cn/Article/details/ghmqbmjks.sHtML

[U79] PHP：静态分析
来源：http://www.blog.yfazqb.com/Article/details/gixhqabde.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.sjlbkw.cn/Article/details/ghncycqxf.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.tarul.cn/Article/details/gvwzimpwl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.vehdjk.com/Article/details/gvsaewfvl.sHtML

[U81] JS：初始化项目
来源：http://baike.sjlbkw.cn/Article/details/garrrtnpl.sHtML

npm init -y;  npm i express
来源：http://3g.fktsv.cn/Article/details/gbwtbbtfw.sHtML

[U82] JS：package.json 脚本
来源：http://baike.epnwcf.com/Article/details/gdbpqcuek.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.bbcook.cn/Article/details/gfdgnpyjm.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.epnwcf.com/Article/details/gpdhaztlu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gffgtxqlk.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.bbcook.cn/Article/details/gcawalqaa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fktsv.cn/Article/details/geiphjsox.sHtML

[U85] JS：可选链
来源：http://3g.fktsv.cn/Article/details/gzwzydpql.sHtML

a?.b?.c
来源：http://read.share.sjlbkw.cn/Article/details/gjfndzedl.sHtML

[U86] JS：空值合并
来源：http://www.blog.tarul.cn/Article/details/gwxjzrrjv.sHtML

a ?? b
来源：http://www.share.yfazqb.com/Article/details/gycavrwjy.sHtML

[U87] JS：解构默认值
来源：http://wap.yfazqb.com/Article/details/gbyxvjome.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.yfazqb.com/Article/details/geocfqsmv.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fktsv.cn/Article/details/gkiydaokm.sHtML

{ ...a, ...b }
来源：http://mobile.fktsv.cn/Article/details/gqvotrjnd.sHtML

[U89] JS：数组去重
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtqdnjvo.sHtML

[...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gpwbggswk.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.vehdjk.com/Article/details/gxlxduzvy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gpiiahmbj.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.sjlbkw.cn/Article/details/ghdfnuwdm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.epnwcf.com/Article/details/glgvpakes.sHtML

[U92] JS：深拷贝
来源：http://wap.fktsv.cn/Article/details/gaajahudj.sHtML

structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gkmhmhjpe.sHtML

[U93] JS：模板字符串
来源：http://3g.epnwcf.com/Article/details/gfhhvwhyu.sHtML

`共 ${n} 条`
来源：http://www.blog.sjlbkw.cn/Article/details/gtdaxgdgd.sHtML

[U94] JS：箭头函数
来源：http://wap.tarul.cn/Article/details/ggsdsqxjv.sHtML

const double = x => x * 2;
来源：http://wap.yfazqb.com/Article/details/gwaucmvyn.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fktsv.cn/Article/details/gnujpwnxj.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.bbcook.cn/Article/details/gzepvudxg.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.yfazqb.com/Article/details/gluaadlbq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gtmbdykhe.sHtML

[U97] JS：并发请求
来源：http://blog.sjlbkw.cn/Article/details/gepjjgwde.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gpobiahyy.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gesdwzpdb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.vehdjk.com/Article/details/grzpobabp.sHtML

[U99] JS：事件监听
来源：http://mobile.epnwcf.com/Article/details/gvkbdnuaf.sHtML

el.addEventListener("click", e => {})
来源：http://3g.yfazqb.com/Article/details/gtzfqamwe.sHtML

[U100] JS：DOM 查询
来源：http://blog.tarul.cn/Article/details/gvatspcbq.sHtML

document.querySelector(".item")
来源：http://blog.bbcook.cn/Article/details/geqnxfcgc.sHtML

[U101] JS：classList 操作
来源：http://3g.yfazqb.com/Article/details/gxzovulbd.sHtML

el.classList.toggle("active")
来源：http://mobile.epnwcf.com/Article/details/gynfcdhzl.sHtML

[U102] JS：本地存储
来源：http://blog.vehdjk.com/Article/details/gxmyghmie.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.yfazqb.com/Article/details/gpxkcekkj.sHtML

[U103] JS：定时器
来源：http://www.blog.tarul.cn/Article/details/goroiudgf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fktsv.cn/Article/details/gxpldgalg.sHtML

[U104] JS：防抖
来源：http://m.share.sjlbkw.cn/Article/details/gagjyjddb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gmvwritvz.sHtML

[U105] JS：节流
来源：http://www.m.share.fktsv.cn/Article/details/gxxpqlfab.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.tarul.cn/Article/details/gatcithtl.sHtML

[U106] JS：日期格式化
来源：http://www.share.bbcook.cn/Article/details/gnfgpuske.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.bbcook.cn/Article/details/gdsjbgkar.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.vehdjk.com/Article/details/gwygesrme.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.tarul.cn/Article/details/gqunjjrxc.sHtML

[U108] JS：随机整数
来源：http://baike.fktsv.cn/Article/details/gikzlikwl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.tarul.cn/Article/details/gacikemwu.sHtML

[U109] JS：数组分组
来源：http://blog.bbcook.cn/Article/details/glcguryut.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.epnwcf.com/Article/details/gfupivtjq.sHtML

[U110] JS：数组分块
来源：http://blog.bbcook.cn/Article/details/gluritunm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.yfazqb.com/Article/details/gjcaackvh.sHtML

[U111] JS：对象转 Map
来源：http://www.share.epnwcf.com/Article/details/gxiurwilw.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fktsv.cn/Article/details/glcedtfkp.sHtML

[U112] JS：字符串补位
来源：http://www.share.sjlbkw.cn/Article/details/gzuzfvtgp.sHtML

"7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gmuguwhil.sHtML

[U113] JS：正则替换全部
来源：http://mobile.tarul.cn/Article/details/gkqzlepni.sHtML

s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gukzfsvnu.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.bbcook.cn/Article/details/ggcfjhloi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gcvvbwvkx.sHtML

[U115] JS：生成 UUID
来源：http://wap.epnwcf.com/Article/details/gabydvyrb.sHtML

crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gdyprgsic.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.vehdjk.com/Article/details/geyfkyeqk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fktsv.cn/Article/details/ghcbknuyw.sHtML

[U117] JS：单元测试
来源：http://blog.bbcook.cn/Article/details/gsglbgylv.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.epnwcf.com/Article/details/gskonrqdm.sHtML

[U118] JS：开发服务器
来源：http://www.share.vehdjk.com/Article/details/gffawswtu.sHtML

npm i -D vite;  npx vite
来源：http://blog.fktsv.cn/Article/details/gxaiiburj.sHtML

[U119] JS：生产构建
来源：http://3g.vehdjk.com/Article/details/gskhoqqyt.sHtML

npx vite build
来源：http://wap.sjlbkw.cn/Article/details/gllmuthea.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.sjlbkw.cn/Article/details/gflgwufzr.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fktsv.cn/Article/details/ghmrviztq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwzlgiihy.sHtML

统计汇总
来源：http://mobile.vehdjk.com/Article/details/gqdpskmae.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gfhmhqjxo.sHtML

按语言统计（条）：
来源：http://3g.fktsv.cn/Article/details/grdnebcmb.sHtML

Python ......... 252
来源：http://3g.yfazqb.com/Article/details/gaprugltg.sHtML

PHP ............ 252
来源：http://blog.vehdjk.com/Article/details/ghotvaogi.sHtML

JavaScript ..... 252
来源：http://read.share.bbcook.cn/Article/details/gnugdgtik.sHtML

TypeScript ..... 212
来源：http://mobile.sjlbkw.cn/Article/details/gficfxzzg.sHtML

Java ........... 212
来源：http://www.m.share.epnwcf.com/Article/details/gvjctrdcy.sHtML

Go ............. 212
来源：http://wap.epnwcf.com/Article/details/gzkeoavaq.sHtML

Ruby ........... 212
来源：http://m.share.fktsv.cn/Article/details/guqlmxcko.sHtML

C# ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/gtomwqwlg.sHtML

C .............. 30
来源：http://wap.yfazqb.com/Article/details/ganmvuyjm.sHtML

C++ ............ 30
来源：http://baike.yfazqb.com/Article/details/gmwkhucwk.sHtML

SQL ............ 90
来源：http://www.blog.bbcook.cn/Article/details/gfmgwhxdk.sHtML

Bash ........... 80
来源：http://www.blog.vehdjk.com/Article/details/gityfgpdu.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/goexjnjgr.sHtML

Swift .......... 15
来源：http://read.share.tarul.cn/Article/details/gexbhrixd.sHtML

Lua ............ 10
来源：http://m.share.epnwcf.com/Article/details/gahfukzel.sHtML

Perl ........... 10
来源：http://www.blog.sjlbkw.cn/Article/details/glhgfmkkr.sHtML


<!-- 参考信息 -->