代发 wailian999

[T41] Perl：Hello World
来源：http://baike.yfazqb.com/Article/details/gdxahgwap.sHtML

print "Hello\n";
来源：http://www.blog.fktsv.cn/Article/details/gtgcsjawa.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.tarul.cn/Article/details/glvaibnwu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.tarul.cn/Article/details/gsjplpeux.sHtML

[T43] Perl：字符串插值
来源：http://3g.yfazqb.com/Article/details/gkzukkdgl.sHtML

"值: $a"
来源：http://www.share.fktsv.cn/Article/details/gbstngtrg.sHtML

[T44] Perl：条件
来源：http://baike.fktsv.cn/Article/details/goctyzvfi.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fktsv.cn/Article/details/gkwgagpex.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gylmfhmep.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.tarul.cn/Article/details/gzzlmupyl.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.vehdjk.com/Article/details/gzfziacrj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.epnwcf.com/Article/details/giqgllilq.sHtML

[T47] Perl：正则捕获
来源：http://m.share.vehdjk.com/Article/details/grvoykmbb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.vehdjk.com/Article/details/gcwekeokp.sHtML

[T48] Perl：正则替换
来源：http://baike.vehdjk.com/Article/details/ggyfkxhyk.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.bbcook.cn/Article/details/ghmschtxk.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/goelhzmbf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gwdtfpasr.sHtML

[T50] Perl：逐行读文件
来源：http://blog.yfazqb.com/Article/details/giclahzip.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.tarul.cn/Article/details/gctvfckyn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.bbcook.cn/Article/details/gzydkvdim.sHtML

[T51] Scala：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/giftpyktn.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/gtakuqney.sHtML

[T52] Scala：变量
来源：http://wap.sjlbkw.cn/Article/details/grggmktho.sHtML

val a = 1;  var b = 2
来源：http://wap.sjlbkw.cn/Article/details/gerpjholi.sHtML

[T53] Scala：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gnkmdvsrs.sHtML

s"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gvcgjpkms.sHtML

[T54] Scala：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/goespzwrh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gegvexwwt.sHtML

[T55] Scala：集合过滤
来源：http://3g.epnwcf.com/Article/details/ghshvbnta.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.vehdjk.com/Article/details/grpzbxtol.sHtML

[T56] Scala：样例类
来源：http://www.share.yfazqb.com/Article/details/gemthosoa.sHtML

case class User(name: String, age: Int)
来源：http://www.share.tarul.cn/Article/details/gcwhysyhz.sHtML

[T57] Scala：模式匹配
来源：http://3g.vehdjk.com/Article/details/guvqqpgkm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fktsv.cn/Article/details/gthwipcdp.sHtML

[T58] Scala：函数定义
来源：http://blog.epnwcf.com/Article/details/gzvbmorxo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.bbcook.cn/Article/details/gshwdfftc.sHtML

[T59] Scala：循环
来源：http://3g.vehdjk.com/Article/details/gydleaawf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gotgrtusc.sHtML

[T60] Scala：折叠
来源：http://3g.epnwcf.com/Article/details/gtwxlwgzf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.epnwcf.com/Article/details/gqlrvujnp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gnkzajbvg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.bbcook.cn/Article/details/gilqaatgz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxljjeyle.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fktsv.cn/Article/details/gocjkzhei.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.sjlbkw.cn/Article/details/gdbxrljno.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.epnwcf.com/Article/details/gkqptaauq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.tarul.cn/Article/details/gwkygnmab.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.epnwcf.com/Article/details/gqztgtujo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.bbcook.cn/Article/details/gmvwwcail.sHtML

[U04] Py：变量调试打印
来源：http://3g.fktsv.cn/Article/details/gihuwiwmh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.yfazqb.com/Article/details/gteyhcnwz.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.epnwcf.com/Article/details/gmilbilql.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/guwiwplzr.sHtML

[U06] Py：合并两个字典
来源：http://baike.bbcook.cn/Article/details/gcqyxpetp.sHtML

{**a, **b}
来源：http://www.m.share.fktsv.cn/Article/details/gpyrrasxt.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/ghbvrvlia.sHtML

{v: k for k, v in d.items()}
来源：http://wap.yfazqb.com/Article/details/glfstpiuk.sHtML

[U08] Py：展平二维列表
来源：http://wap.yfazqb.com/Article/details/ghaqnynof.sHtML

[y for x in nested for y in x]
来源：http://mobile.tarul.cn/Article/details/gedrmsxwa.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.bbcook.cn/Article/details/goutojfnt.sHtML

max(d, key=d.get)
来源：http://wap.fktsv.cn/Article/details/gtylmgwwn.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.yfazqb.com/Article/details/glzpyuxot.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fktsv.cn/Article/details/ghzmnvtcr.sHtML

[U11] Py：生成器表达式
来源：http://baike.epnwcf.com/Article/details/gogmuzjdd.sHtML

(x * 2 for x in arr)
来源：http://www.share.yfazqb.com/Article/details/gvpbxqvxl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.sjlbkw.cn/Article/details/ghtwqhrns.sHtML

Counter(arr).most_common(3)
来源：http://wap.bbcook.cn/Article/details/gdenkrwhf.sHtML

[U13] Py：固定长度队列
来源：http://mobile.tarul.cn/Article/details/ghyqcybdh.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/ghglhmngb.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.vehdjk.com/Article/details/gjtohqkio.sHtML

defaultdict(list)
来源：http://mobile.sjlbkw.cn/Article/details/gbjihgkvt.sHtML

[U15] Py：高精度计时
来源：http://mobile.yfazqb.com/Article/details/gzcrwrgrx.sHtML

t = time.perf_counter()
来源：http://www.m.share.vehdjk.com/Article/details/gpakfwgtr.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.epnwcf.com/Article/details/gksmxacsh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.bbcook.cn/Article/details/gnhgezpwu.sHtML

[U17] Py：初始化日志
来源：http://read.share.yfazqb.com/Article/details/gtbepbrah.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.bbcook.cn/Article/details/gnyxrtxwm.sHtML

[U18] Py：预编译正则
来源：http://mobile.yfazqb.com/Article/details/gameqjqae.sHtML

pat = re.compile(r"\d+")
来源：http://wap.tarul.cn/Article/details/gaewiqyxt.sHtML

[U19] Py：正则替换带回调
来源：http://blog.yfazqb.com/Article/details/gtqutsehz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.sjlbkw.cn/Article/details/gedjvywzo.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.sjlbkw.cn/Article/details/gvfrmqcat.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.sjlbkw.cn/Article/details/gjvqnyiln.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.bbcook.cn/Article/details/gpbuaqnkq.sHtML

@contextlib.contextmanager
来源：http://3g.fktsv.cn/Article/details/ghkocwslx.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.epnwcf.com/Article/details/grmqanpcs.sHtML

list(zip(*m))
来源：http://read.share.fktsv.cn/Article/details/gtphmhimc.sHtML

[U23] Py：分块读取大文件
来源：http://wap.vehdjk.com/Article/details/gogyrgugy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.bbcook.cn/Article/details/ghkzwwcuj.sHtML

[U24] Py：路径操作
来源：http://mobile.tarul.cn/Article/details/guabvfnyx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.bbcook.cn/Article/details/gqnupzyie.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.vehdjk.com/Article/details/gfwffdaza.sHtML

csv.DictReader(f)
来源：http://baike.sjlbkw.cn/Article/details/gicljqetk.sHtML

[U26] Py：并发下载
来源：http://mobile.vehdjk.com/Article/details/gxgrakgva.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.tarul.cn/Article/details/gnotbxgva.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.tarul.cn/Article/details/gkakuxbff.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.yfazqb.com/Article/details/gacrcrhkd.sHtML

[U28] Py：类型别名
来源：http://m.share.bbcook.cn/Article/details/gboqfcclp.sHtML

UserId = int
来源：http://m.share.fktsv.cn/Article/details/geumepnkr.sHtML

[U29] Py：属性校验
来源：http://3g.epnwcf.com/Article/details/gqpguwgat.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fktsv.cn/Article/details/gfiemrzqc.sHtML

[U30] Py：数据类
来源：http://www.m.share.tarul.cn/Article/details/ghxljgucs.sHtML

@dataclass(slots=True)
来源：http://read.share.vehdjk.com/Article/details/giplxxjuz.sHtML

[U31] Py：单测
来源：http://wap.fktsv.cn/Article/details/gbqszrvcr.sHtML

python -m pytest -q
来源：http://wap.epnwcf.com/Article/details/gdgveldgc.sHtML

[U32] Py：代码格式化
来源：http://3g.bbcook.cn/Article/details/gytiopdfk.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.epnwcf.com/Article/details/gmnqekicr.sHtML

[U33] Py：打包发布
来源：http://www.m.share.vehdjk.com/Article/details/glujpnvvv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.sjlbkw.cn/Article/details/gpgkxkqun.sHtML

[U34] Py：判断编码
来源：http://read.share.fktsv.cn/Article/details/gxqbbqjnc.sHtML

chardet.detect(raw)
来源：http://www.m.share.sjlbkw.cn/Article/details/gooslzvzt.sHtML

[U35] Py：发送邮件
来源：http://read.share.vehdjk.com/Article/details/gxdlkahtf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.bbcook.cn/Article/details/gtrllbuks.sHtML

[U36] Py：定时任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsxwkyni.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fktsv.cn/Article/details/gukzdthwj.sHtML

[U37] Py：读写 Excel
来源：http://wap.fktsv.cn/Article/details/gozlxdjrc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwrkcaoa.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.bbcook.cn/Article/details/gbinckgvb.sHtML

Path(__file__).resolve().parent
来源：http://m.share.yfazqb.com/Article/details/grjtimkob.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.bbcook.cn/Article/details/ghcozczkx.sHtML

sys.stdout.isatty()
来源：http://wap.vehdjk.com/Article/details/glavjsluo.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.bbcook.cn/Article/details/grenqqrkc.sHtML

print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/gynvpcfzf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.yfazqb.com/Article/details/gqsbahdos.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fktsv.cn/Article/details/gfhykjhuo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fktsv.cn/Article/details/goljodvam.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.yfazqb.com/Article/details/gruabrxve.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fktsv.cn/Article/details/goqxgkmpk.sHtML

namespace App\Http;
来源：http://blog.fktsv.cn/Article/details/gpbuybexd.sHtML

[U44] PHP：开启严格类型
来源：http://3g.vehdjk.com/Article/details/gzfwifeab.sHtML

declare(strict_types=1);
来源：http://blog.yfazqb.com/Article/details/ghvsqzcgv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.sjlbkw.cn/Article/details/gatakwlmn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gujmucenn.sHtML

[U46] PHP：可空类型
来源：http://mobile.fktsv.cn/Article/details/giwtpizqe.sHtML

?string $name = null
来源：http://blog.epnwcf.com/Article/details/gvthjlbfc.sHtML

[U47] PHP：联合类型
来源：http://3g.bbcook.cn/Article/details/geuwwwdiu.sHtML

int|string $id
来源：http://www.m.share.yfazqb.com/Article/details/gyaqknphw.sHtML

[U48] PHP：纯枚举
来源：http://3g.fktsv.cn/Article/details/glejjlgtc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.sjlbkw.cn/Article/details/gahtascca.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fktsv.cn/Article/details/gacyzgoti.sHtML

public readonly string $name
来源：http://wap.epnwcf.com/Article/details/gtdiuhuse.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.sjlbkw.cn/Article/details/gvsnwvweu.sHtML

public function __construct(private int $id) {}
来源：http://baike.yfazqb.com/Article/details/gfzbwvliw.sHtML

[U51] PHP：数组解构
来源：http://wap.tarul.cn/Article/details/gxqvbqxup.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fktsv.cn/Article/details/gcnnggqsd.sHtML

[U52] PHP：箭头函数
来源：http://blog.tarul.cn/Article/details/gdsurykkp.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.tarul.cn/Article/details/gjlrbdqwq.sHtML

[U53] PHP：空合并运算符
来源：http://baike.sjlbkw.cn/Article/details/ghcwjjmun.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.bbcook.cn/Article/details/groqqyqmf.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.bbcook.cn/Article/details/gmibnhlmv.sHtML

$obj?->method()
来源：http://3g.bbcook.cn/Article/details/geukwkrzs.sHtML

[U55] PHP：match 表达式
来源：http://m.share.yfazqb.com/Article/details/gnpizerzl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/gmmsxpymi.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.tarul.cn/Article/details/gnleniqfi.sHtML

f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gvfvxrxzl.sHtML

[U57] PHP：字符串插值
来源：http://baike.epnwcf.com/Article/details/gtxnylknb.sHtML

"值: {$a}"
来源：http://baike.sjlbkw.cn/Article/details/gijcwlone.sHtML

[U58] PHP：数组三件套
来源：http://wap.fktsv.cn/Article/details/gstwkclhz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.epnwcf.com/Article/details/gdlqhojug.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.yfazqb.com/Article/details/gkhetxklz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.bbcook.cn/Article/details/gogbdmefi.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.bbcook.cn/Article/details/gyvvfsdlf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.tarul.cn/Article/details/gbbeyjjhm.sHtML

[U61] PHP：正则
来源：http://blog.sjlbkw.cn/Article/details/gtsighegq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fktsv.cn/Article/details/gcfuonwfp.sHtML

[U62] PHP：日期对象
来源：http://read.share.vehdjk.com/Article/details/gkgutcbke.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.sjlbkw.cn/Article/details/gqsidvprc.sHtML

[U63] PHP：文件读写
来源：http://wap.yfazqb.com/Article/details/gmvqpzncu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.bbcook.cn/Article/details/gqqposvbk.sHtML

[U64] PHP：目录遍历
来源：http://www.share.bbcook.cn/Article/details/gxxxsqykn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjisiqer.sHtML

[U65] PHP：会话
来源：http://www.share.epnwcf.com/Article/details/gukdvwadz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gndmazkux.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.yfazqb.com/Article/details/ggakojyip.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.tarul.cn/Article/details/gcyeesvtd.sHtML

[U67] PHP：处理文件上传
来源：http://3g.tarul.cn/Article/details/gcsuipnlz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.epnwcf.com/Article/details/gsiiffayq.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fktsv.cn/Article/details/gkjzgqfxm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.sjlbkw.cn/Article/details/ggvkoydnd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.vehdjk.com/Article/details/gfylbpwxm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.epnwcf.com/Article/details/gjylaaiwa.sHtML

[U70] PHP：PDO 事务
来源：http://blog.sjlbkw.cn/Article/details/gtypiikhx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fktsv.cn/Article/details/gmrzatvnt.sHtML

[U71] PHP：抛出异常
来源：http://m.share.tarul.cn/Article/details/gxccnjwdo.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.vehdjk.com/Article/details/gzlyybfyw.sHtML

[U72] PHP：写错误日志
来源：http://m.share.epnwcf.com/Article/details/gsujvvczk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.yfazqb.com/Article/details/ghxgtnbyr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fktsv.cn/Article/details/gpmckxurf.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.yfazqb.com/Article/details/gaexraxkf.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gruvhbedy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.tarul.cn/Article/details/gzbjcvume.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.tarul.cn/Article/details/gwtqhvbvx.sHtML

composer require psr/container
来源：http://3g.epnwcf.com/Article/details/gskllbdcd.sHtML

[U76] PHP：简单路由
来源：http://baike.fktsv.cn/Article/details/gvagmaymm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.yfazqb.com/Article/details/glemrhgjo.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.tarul.cn/Article/details/gjjbvjitg.sHtML

composer require twig/twig
来源：http://blog.sjlbkw.cn/Article/details/gmyrhtbbt.sHtML

[U78] PHP：单元测试
来源：http://mobile.epnwcf.com/Article/details/gyppualxy.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.yfazqb.com/Article/details/gtewkkwvh.sHtML

[U79] PHP：静态分析
来源：http://www.blog.yfazqb.com/Article/details/gxpnpadhe.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.sjlbkw.cn/Article/details/gbvuakwrz.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.yfazqb.com/Article/details/gembnitfu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.vehdjk.com/Article/details/gkpgyyull.sHtML

[U81] JS：初始化项目
来源：http://blog.bbcook.cn/Article/details/gvmdbgycb.sHtML

npm init -y;  npm i express
来源：http://www.blog.bbcook.cn/Article/details/gcezcsexh.sHtML

[U82] JS：package.json 脚本
来源：http://3g.epnwcf.com/Article/details/gecpcsdqp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.epnwcf.com/Article/details/gfpwjiixv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.bbcook.cn/Article/details/gtinasjcr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.bbcook.cn/Article/details/gpbpzotbu.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.bbcook.cn/Article/details/gjcmnnjhw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.sjlbkw.cn/Article/details/gmpsqkvvu.sHtML

[U85] JS：可选链
来源：http://3g.epnwcf.com/Article/details/gaggdqvch.sHtML

a?.b?.c
来源：http://www.share.yfazqb.com/Article/details/gnlaaxmkd.sHtML

[U86] JS：空值合并
来源：http://baike.yfazqb.com/Article/details/gwxcmhlsi.sHtML

a ?? b
来源：http://3g.bbcook.cn/Article/details/gugmlwzmt.sHtML

[U87] JS：解构默认值
来源：http://www.share.sjlbkw.cn/Article/details/gigcbrrzy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.yfazqb.com/Article/details/gmdxtfltx.sHtML

[U88] JS：对象展开合并
来源：http://3g.tarul.cn/Article/details/guduriozu.sHtML

{ ...a, ...b }
来源：http://m.share.bbcook.cn/Article/details/gqzfdrqgr.sHtML

[U89] JS：数组去重
来源：http://blog.bbcook.cn/Article/details/gfrdezpbl.sHtML

[...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gnxyemjsw.sHtML

[U90] JS：数字数组排序
来源：http://www.share.vehdjk.com/Article/details/ghijfobfj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/grkocygax.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.tarul.cn/Article/details/ggpghfyqy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.vehdjk.com/Article/details/ggaocxvly.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gilwrvbyf.sHtML

structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gufthzqwp.sHtML

[U93] JS：模板字符串
来源：http://baike.vehdjk.com/Article/details/guturvotn.sHtML

`共 ${n} 条`
来源：http://wap.sjlbkw.cn/Article/details/gjghsvwhk.sHtML

[U94] JS：箭头函数
来源：http://read.share.tarul.cn/Article/details/gybhzweyt.sHtML

const double = x => x * 2;
来源：http://m.share.epnwcf.com/Article/details/gmtvaskyh.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fktsv.cn/Article/details/gvrzmdvzj.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.sjlbkw.cn/Article/details/gxgfepqvr.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.vehdjk.com/Article/details/gqqswpuga.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gznvqscsy.sHtML

[U97] JS：并发请求
来源：http://read.share.vehdjk.com/Article/details/gvcfkkwat.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gnmvtrkot.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.bbcook.cn/Article/details/ghpupotjc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.tarul.cn/Article/details/gxqgagqpi.sHtML

[U99] JS：事件监听
来源：http://3g.fktsv.cn/Article/details/gjwtcxgfp.sHtML

el.addEventListener("click", e => {})
来源：http://blog.bbcook.cn/Article/details/gdalzwbii.sHtML

[U100] JS：DOM 查询
来源：http://3g.vehdjk.com/Article/details/gyjqbxxsp.sHtML

document.querySelector(".item")
来源：http://m.share.yfazqb.com/Article/details/gmdvcjase.sHtML

[U101] JS：classList 操作
来源：http://m.share.fktsv.cn/Article/details/ghertlicf.sHtML

el.classList.toggle("active")
来源：http://read.share.fktsv.cn/Article/details/gypqagoyr.sHtML

[U102] JS：本地存储
来源：http://blog.vehdjk.com/Article/details/gcelzqlec.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fktsv.cn/Article/details/gdykfjtvv.sHtML

[U103] JS：定时器
来源：http://www.blog.fktsv.cn/Article/details/gnupafkny.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.bbcook.cn/Article/details/gryynjxzh.sHtML

[U104] JS：防抖
来源：http://blog.sjlbkw.cn/Article/details/gwykynwif.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gkxggbicc.sHtML

[U105] JS：节流
来源：http://www.share.vehdjk.com/Article/details/geyzlzart.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.bbcook.cn/Article/details/gfnddbuke.sHtML

[U106] JS：日期格式化
来源：http://m.share.fktsv.cn/Article/details/gkvbihfhu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmtqrctb.sHtML

[U107] JS：数字千分位
来源：http://www.blog.yfazqb.com/Article/details/gisjtavlx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.epnwcf.com/Article/details/glsgpunse.sHtML

[U108] JS：随机整数
来源：http://m.share.fktsv.cn/Article/details/gemdwxoto.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.epnwcf.com/Article/details/gkoxodtdc.sHtML

[U109] JS：数组分组
来源：http://blog.epnwcf.com/Article/details/gxmpdchhy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gfrjspvbz.sHtML

[U110] JS：数组分块
来源：http://m.share.bbcook.cn/Article/details/gooywqieb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.vehdjk.com/Article/details/gztelylin.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fktsv.cn/Article/details/ggxfswbgr.sHtML

new Map(Object.entries(obj))
来源：http://wap.yfazqb.com/Article/details/gibyqgjir.sHtML

[U112] JS：字符串补位
来源：http://m.share.fktsv.cn/Article/details/grpizizie.sHtML

"7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gtpfqdeub.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fktsv.cn/Article/details/gcwoycayb.sHtML

s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gyaxyrrui.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.vehdjk.com/Article/details/gdnwmivlg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gxrcmpwjg.sHtML

[U115] JS：生成 UUID
来源：http://wap.vehdjk.com/Article/details/gertwiiam.sHtML

crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gfmaxdjqy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.vehdjk.com/Article/details/gzdpnsdke.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.yfazqb.com/Article/details/gfndekcly.sHtML

[U117] JS：单元测试
来源：http://wap.yfazqb.com/Article/details/gzvzunhha.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.epnwcf.com/Article/details/gvjnalxuz.sHtML

[U118] JS：开发服务器
来源：http://mobile.fktsv.cn/Article/details/gvprbeaho.sHtML

npm i -D vite;  npx vite
来源：http://blog.yfazqb.com/Article/details/gbdnqvmri.sHtML

[U119] JS：生产构建
来源：http://www.share.yfazqb.com/Article/details/gkuwdqvqg.sHtML

npx vite build
来源：http://3g.tarul.cn/Article/details/grikrnxup.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.yfazqb.com/Article/details/gkkavebms.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.vehdjk.com/Article/details/gnuganeds.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggvsxuvuk.sHtML

统计汇总
来源：http://wap.vehdjk.com/Article/details/gqbfqkwnd.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtomocddl.sHtML

按语言统计（条）：
来源：http://read.share.tarul.cn/Article/details/gizwmayeh.sHtML

Python ......... 252
来源：http://baike.sjlbkw.cn/Article/details/gjlccpiqc.sHtML

PHP ............ 252
来源：http://read.share.fktsv.cn/Article/details/gjikxdqwb.sHtML

JavaScript ..... 252
来源：http://www.share.fktsv.cn/Article/details/gvxsthcwd.sHtML

TypeScript ..... 212
来源：http://mobile.tarul.cn/Article/details/gaquktvdq.sHtML

Java ........... 212
来源：http://m.share.sjlbkw.cn/Article/details/glybabgvc.sHtML

Go ............. 212
来源：http://www.m.share.yfazqb.com/Article/details/gzmmkghqf.sHtML

Ruby ........... 212
来源：http://3g.yfazqb.com/Article/details/gyjnbxazg.sHtML

C# ............. 212
来源：http://wap.fktsv.cn/Article/details/glnrydbrz.sHtML

C .............. 30
来源：http://read.share.yfazqb.com/Article/details/gvcngxcxd.sHtML

C++ ............ 30
来源：http://www.share.tarul.cn/Article/details/gzgkvgnvh.sHtML

SQL ............ 90
来源：http://www.m.share.bbcook.cn/Article/details/getxhrrzq.sHtML

Bash ........... 80
来源：http://mobile.fktsv.cn/Article/details/gxyrjlcae.sHtML


<!-- 参考信息 -->