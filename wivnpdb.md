代发 wailian999

[T45] Perl：数组遍历
来源：http://www.blog.vehdjk.com/Article/details/glaabcjrf.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fktsv.cn/Article/details/gylasqxhv.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.tarul.cn/Article/details/gkyrjpomy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.epnwcf.com/Article/details/gyzdvzlqt.sHtML

[T47] Perl：正则捕获
来源：http://www.share.bbcook.cn/Article/details/gvrzjpocy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.yfazqb.com/Article/details/gjybguhmf.sHtML

[T48] Perl：正则替换
来源：http://3g.tarul.cn/Article/details/glijmbpet.sHtML

$s =~ s/old/new/g;
来源：http://wap.yfazqb.com/Article/details/gmqtuiewp.sHtML

[T49] Perl：函数
来源：http://mobile.yfazqb.com/Article/details/gjnlnfxht.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gkmxtsrsx.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gbsfdolca.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.vehdjk.com/Article/details/glxvobhmy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.yfazqb.com/Article/details/gtnkxvpqv.sHtML

[T51] Scala：Hello World
来源：http://wap.bbcook.cn/Article/details/glacrowdr.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gcocmfmfi.sHtML

[T52] Scala：变量
来源：http://blog.epnwcf.com/Article/details/gyjrgrqyl.sHtML

val a = 1;  var b = 2
来源：http://read.share.tarul.cn/Article/details/gkwuufebt.sHtML

[T53] Scala：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gwrgiigyx.sHtML

s"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gtvkpxwqx.sHtML

[T54] Scala：集合映射
来源：http://read.share.fktsv.cn/Article/details/gctjdlrqh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.vehdjk.com/Article/details/ggpwwsjor.sHtML

[T55] Scala：集合过滤
来源：http://m.share.yfazqb.com/Article/details/ghwphqqnd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fktsv.cn/Article/details/gajjmnhqa.sHtML

[T56] Scala：样例类
来源：http://m.share.vehdjk.com/Article/details/gnbbpwgnk.sHtML

case class User(name: String, age: Int)
来源：http://read.share.epnwcf.com/Article/details/gasgfhnmh.sHtML

[T57] Scala：模式匹配
来源：http://3g.bbcook.cn/Article/details/gepzahnzv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gframorpm.sHtML

[T58] Scala：函数定义
来源：http://read.share.epnwcf.com/Article/details/gyqqwnryb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.yfazqb.com/Article/details/gqqxqvxzg.sHtML

[T59] Scala：循环
来源：http://m.share.tarul.cn/Article/details/gxwyjdqqo.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fktsv.cn/Article/details/gxfcdnica.sHtML

[T60] Scala：折叠
来源：http://wap.epnwcf.com/Article/details/gqspxqqgp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.sjlbkw.cn/Article/details/gyhtcxwev.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyusujwsq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gnznqrzva.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghczmkbhr.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.sjlbkw.cn/Article/details/gxprkgtxe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.epnwcf.com/Article/details/gxlgapupu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.yfazqb.com/Article/details/gyllcakmy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.yfazqb.com/Article/details/gvamfkcpg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fktsv.cn/Article/details/gkhcczbka.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.tarul.cn/Article/details/gtfigsxyw.sHtML

[U04] Py：变量调试打印
来源：http://baike.fktsv.cn/Article/details/gmzxusdfj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.yfazqb.com/Article/details/gknaxgort.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.bbcook.cn/Article/details/gmhhipwzf.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gmyjykaff.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fktsv.cn/Article/details/ggkmtkiot.sHtML

{**a, **b}
来源：http://read.share.sjlbkw.cn/Article/details/gmbckiadh.sHtML

[U07] Py：反转字典键值
来源：http://blog.yfazqb.com/Article/details/gupiggckl.sHtML

{v: k for k, v in d.items()}
来源：http://baike.epnwcf.com/Article/details/glkzsnmxx.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fktsv.cn/Article/details/gdiihievx.sHtML

[y for x in nested for y in x]
来源：http://www.blog.epnwcf.com/Article/details/gwzyacxpt.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fktsv.cn/Article/details/gubqjjupo.sHtML

max(d, key=d.get)
来源：http://baike.vehdjk.com/Article/details/gzwibrfbw.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fktsv.cn/Article/details/gasazeuwk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.vehdjk.com/Article/details/gyjgqzeas.sHtML

[U11] Py：生成器表达式
来源：http://mobile.vehdjk.com/Article/details/gheoqqclk.sHtML

(x * 2 for x in arr)
来源：http://mobile.yfazqb.com/Article/details/gkenwixix.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/gjpgczfru.sHtML

Counter(arr).most_common(3)
来源：http://blog.tarul.cn/Article/details/gqeigdhkx.sHtML

[U13] Py：固定长度队列
来源：http://3g.epnwcf.com/Article/details/guevgjdqc.sHtML

deque(maxlen=10)
来源：http://blog.bbcook.cn/Article/details/gjezraxvg.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.tarul.cn/Article/details/gzncjcfdn.sHtML

defaultdict(list)
来源：http://www.blog.epnwcf.com/Article/details/gpdwovggf.sHtML

[U15] Py：高精度计时
来源：http://mobile.epnwcf.com/Article/details/glkjmvweb.sHtML

t = time.perf_counter()
来源：http://m.share.bbcook.cn/Article/details/goicwgwax.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.yfazqb.com/Article/details/gdrhjzxoy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.epnwcf.com/Article/details/gjecpmcum.sHtML

[U17] Py：初始化日志
来源：http://m.share.epnwcf.com/Article/details/gkfbetzne.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.sjlbkw.cn/Article/details/gidphtwph.sHtML

[U18] Py：预编译正则
来源：http://www.share.vehdjk.com/Article/details/gqdotcqkj.sHtML

pat = re.compile(r"\d+")
来源：http://blog.vehdjk.com/Article/details/gaqskbxhi.sHtML

[U19] Py：正则替换带回调
来源：http://3g.epnwcf.com/Article/details/gfctsmgln.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.sjlbkw.cn/Article/details/gvceyddnr.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.sjlbkw.cn/Article/details/goietlbje.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.sjlbkw.cn/Article/details/guvomiqls.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.bbcook.cn/Article/details/glrkajvnj.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fktsv.cn/Article/details/gaqurifrk.sHtML

[U22] Py：矩阵转置
来源：http://baike.bbcook.cn/Article/details/gkrtxluwo.sHtML

list(zip(*m))
来源：http://www.m.share.fktsv.cn/Article/details/gjqewkpke.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fktsv.cn/Article/details/ghppwxzbo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.sjlbkw.cn/Article/details/geutigbmm.sHtML

[U24] Py：路径操作
来源：http://3g.yfazqb.com/Article/details/gkylumrhj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.yfazqb.com/Article/details/gulzwollt.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.bbcook.cn/Article/details/ggredxzlo.sHtML

csv.DictReader(f)
来源：http://m.share.fktsv.cn/Article/details/ghdrolhqf.sHtML

[U26] Py：并发下载
来源：http://read.share.tarul.cn/Article/details/gzigfgskc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.yfazqb.com/Article/details/gzukwtqpp.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.sjlbkw.cn/Article/details/gyaefihzi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.yfazqb.com/Article/details/guaodmqhw.sHtML

[U28] Py：类型别名
来源：http://m.share.fktsv.cn/Article/details/gnhklrvvp.sHtML

UserId = int
来源：http://www.share.bbcook.cn/Article/details/gpdafbnrc.sHtML

[U29] Py：属性校验
来源：http://read.share.sjlbkw.cn/Article/details/glvakfmwz.sHtML

@property 与 @x.setter 配合
来源：http://www.share.tarul.cn/Article/details/gegqizrny.sHtML

[U30] Py：数据类
来源：http://www.share.yfazqb.com/Article/details/gzxsdotlm.sHtML

@dataclass(slots=True)
来源：http://3g.vehdjk.com/Article/details/gjrdvlhdr.sHtML

[U31] Py：单测
来源：http://baike.sjlbkw.cn/Article/details/gyxrotxzw.sHtML

python -m pytest -q
来源：http://read.share.tarul.cn/Article/details/gcwbkchzs.sHtML

[U32] Py：代码格式化
来源：http://wap.vehdjk.com/Article/details/gpalcveys.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.vehdjk.com/Article/details/gzpjezgas.sHtML

[U33] Py：打包发布
来源：http://baike.sjlbkw.cn/Article/details/gahsnblrh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.epnwcf.com/Article/details/gblabggll.sHtML

[U34] Py：判断编码
来源：http://3g.sjlbkw.cn/Article/details/gsvhjmakv.sHtML

chardet.detect(raw)
来源：http://blog.yfazqb.com/Article/details/gnlbreuwk.sHtML

[U35] Py：发送邮件
来源：http://baike.vehdjk.com/Article/details/gjkyhiwoo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.tarul.cn/Article/details/gasytsyha.sHtML

[U36] Py：定时任务
来源：http://3g.epnwcf.com/Article/details/gpzibgzco.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.yfazqb.com/Article/details/gaihravdx.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/gndcabukr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.sjlbkw.cn/Article/details/gikaggavd.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.sjlbkw.cn/Article/details/gbqglxysa.sHtML

Path(__file__).resolve().parent
来源：http://blog.bbcook.cn/Article/details/ghqtzpedx.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.sjlbkw.cn/Article/details/gtodhadre.sHtML

sys.stdout.isatty()
来源：http://www.share.sjlbkw.cn/Article/details/gudlvovqy.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.bbcook.cn/Article/details/gnzkoetdr.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/gcwxaztnk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.bbcook.cn/Article/details/gkennxwac.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.vehdjk.com/Article/details/gpkqrthru.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.vehdjk.com/Article/details/gciphebjp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.yfazqb.com/Article/details/gixbuvxsk.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjcczncv.sHtML

namespace App\Http;
来源：http://wap.fktsv.cn/Article/details/gzopjavoz.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.sjlbkw.cn/Article/details/geokbzjbr.sHtML

declare(strict_types=1);
来源：http://3g.fktsv.cn/Article/details/ggsoqegjk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.tarul.cn/Article/details/gipvimbyf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gwgcnqhpv.sHtML

[U46] PHP：可空类型
来源：http://baike.yfazqb.com/Article/details/ggocftnta.sHtML

?string $name = null
来源：http://3g.epnwcf.com/Article/details/gpgurkevy.sHtML

[U47] PHP：联合类型
来源：http://wap.yfazqb.com/Article/details/ghiomkyix.sHtML

int|string $id
来源：http://read.share.fktsv.cn/Article/details/gigaqrvtt.sHtML

[U48] PHP：纯枚举
来源：http://read.share.vehdjk.com/Article/details/geuqzgbeg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.tarul.cn/Article/details/glqnvxgzr.sHtML

[U49] PHP：只读属性
来源：http://www.share.tarul.cn/Article/details/gqbcnzrga.sHtML

public readonly string $name
来源：http://www.blog.tarul.cn/Article/details/gbsoruuyi.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.sjlbkw.cn/Article/details/giwphjfus.sHtML

public function __construct(private int $id) {}
来源：http://baike.tarul.cn/Article/details/gxyduapca.sHtML

[U51] PHP：数组解构
来源：http://www.share.epnwcf.com/Article/details/ghdmktfbv.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.vehdjk.com/Article/details/gqlxixhbq.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/gawplyjoi.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.vehdjk.com/Article/details/gimiclibg.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.epnwcf.com/Article/details/gznselnbe.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.vehdjk.com/Article/details/gcfypdsdm.sHtML

[U54] PHP：空安全调用
来源：http://mobile.tarul.cn/Article/details/gcqdysivw.sHtML

$obj?->method()
来源：http://blog.sjlbkw.cn/Article/details/gnuqkxess.sHtML

[U55] PHP：match 表达式
来源：http://read.share.tarul.cn/Article/details/gahbzmqov.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.yfazqb.com/Article/details/ggegnkihc.sHtML

[U56] PHP：命名参数
来源：http://blog.yfazqb.com/Article/details/ggpclirqv.sHtML

f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gcclxmwzw.sHtML

[U57] PHP：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gcxesobup.sHtML

"值: {$a}"
来源：http://www.share.vehdjk.com/Article/details/giuthvqfh.sHtML

[U58] PHP：数组三件套
来源：http://www.share.sjlbkw.cn/Article/details/ggcisaaaf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fktsv.cn/Article/details/gpffunpgf.sHtML

[U59] PHP：自定义排序
来源：http://blog.epnwcf.com/Article/details/ghpeeshnj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gsrffkkff.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.epnwcf.com/Article/details/ghmujjdjs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.bbcook.cn/Article/details/gascykkpa.sHtML

[U61] PHP：正则
来源：http://wap.yfazqb.com/Article/details/gzkqtsgoc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gtayuzxkn.sHtML

[U62] PHP：日期对象
来源：http://m.share.fktsv.cn/Article/details/gsixadpjz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.bbcook.cn/Article/details/gppcevchg.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.yfazqb.com/Article/details/gmktofxyp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fktsv.cn/Article/details/gyzzxphmm.sHtML

[U64] PHP：目录遍历
来源：http://3g.vehdjk.com/Article/details/gwsiugjhy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.yfazqb.com/Article/details/guokwcsaw.sHtML

[U65] PHP：会话
来源：http://read.share.tarul.cn/Article/details/gdrymckda.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gcfkecpen.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.tarul.cn/Article/details/guurlujin.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.vehdjk.com/Article/details/gxtwpgahq.sHtML

[U67] PHP：处理文件上传
来源：http://blog.sjlbkw.cn/Article/details/gplihxsns.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.yfazqb.com/Article/details/gqhzgxzeo.sHtML

[U68] PHP：PDO 连接
来源：http://3g.bbcook.cn/Article/details/gfcqfjyix.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.epnwcf.com/Article/details/glednxsjy.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.vehdjk.com/Article/details/gtyzsifiz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fktsv.cn/Article/details/gpbobbmxh.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.vehdjk.com/Article/details/gznjzfkac.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.bbcook.cn/Article/details/gaccgaawv.sHtML

[U71] PHP：抛出异常
来源：http://m.share.vehdjk.com/Article/details/gbeojvzrn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/ghffvxdbf.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.vehdjk.com/Article/details/gzcthswxw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.yfazqb.com/Article/details/gpbkhrfzg.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.sjlbkw.cn/Article/details/gxqngtxvw.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.sjlbkw.cn/Article/details/gvjbnbeah.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.epnwcf.com/Article/details/gtyiwwukv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fktsv.cn/Article/details/ghyspdloe.sHtML

[U75] PHP：依赖注入
来源：http://m.share.vehdjk.com/Article/details/gvdkvnimc.sHtML

composer require psr/container
来源：http://3g.bbcook.cn/Article/details/gsrxszmbm.sHtML

[U76] PHP：简单路由
来源：http://blog.epnwcf.com/Article/details/gsmpupynv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.bbcook.cn/Article/details/gwgebgyys.sHtML

[U77] PHP：模板渲染
来源：http://3g.yfazqb.com/Article/details/gqfvbvzfp.sHtML

composer require twig/twig
来源：http://www.share.vehdjk.com/Article/details/gipqngfeh.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gqiqwaxvm.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.vehdjk.com/Article/details/gjmpwmxvw.sHtML

[U79] PHP：静态分析
来源：http://wap.vehdjk.com/Article/details/gjmkwktle.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.vehdjk.com/Article/details/ggvpwvapw.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.sjlbkw.cn/Article/details/gwbywwlvb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.sjlbkw.cn/Article/details/gfvmlphco.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.epnwcf.com/Article/details/gwroglfud.sHtML

npm init -y;  npm i express
来源：http://mobile.tarul.cn/Article/details/gmyaiyqrk.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.epnwcf.com/Article/details/gpkfzjoic.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.yfazqb.com/Article/details/goycbhrbk.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.sjlbkw.cn/Article/details/gsogtysmk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/gigbudsqr.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fktsv.cn/Article/details/gczykarqg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.yfazqb.com/Article/details/gxhgwfgnm.sHtML

[U85] JS：可选链
来源：http://mobile.epnwcf.com/Article/details/gjbzlkeci.sHtML

a?.b?.c
来源：http://3g.bbcook.cn/Article/details/gsywdhdaj.sHtML

[U86] JS：空值合并
来源：http://read.share.sjlbkw.cn/Article/details/gatpvcflh.sHtML

a ?? b
来源：http://mobile.epnwcf.com/Article/details/guzjiajjk.sHtML

[U87] JS：解构默认值
来源：http://3g.vehdjk.com/Article/details/gkadjbxde.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.vehdjk.com/Article/details/gnblzjktg.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.epnwcf.com/Article/details/gunvpomas.sHtML

{ ...a, ...b }
来源：http://www.share.sjlbkw.cn/Article/details/gvhmlqaxq.sHtML

[U89] JS：数组去重
来源：http://www.m.share.yfazqb.com/Article/details/gakpudtmj.sHtML

[...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gjoaijgpf.sHtML

[U90] JS：数字数组排序
来源：http://www.share.tarul.cn/Article/details/gqyckqtcb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gsaolvlvy.sHtML

[U91] JS：对象键值遍历
来源：http://baike.epnwcf.com/Article/details/gphdxialj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.yfazqb.com/Article/details/glyfklgpn.sHtML

[U92] JS：深拷贝
来源：http://blog.fktsv.cn/Article/details/gwfstbkqm.sHtML

structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gqkjqxoju.sHtML

[U93] JS：模板字符串
来源：http://baike.yfazqb.com/Article/details/gateckxxj.sHtML

`共 ${n} 条`
来源：http://mobile.yfazqb.com/Article/details/gkaryimak.sHtML

[U94] JS：箭头函数
来源：http://baike.vehdjk.com/Article/details/gzmyhtaas.sHtML

const double = x => x * 2;
来源：http://www.m.share.fktsv.cn/Article/details/gkzbkynur.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.yfazqb.com/Article/details/gvspcgcqi.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.epnwcf.com/Article/details/gqwekarca.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.vehdjk.com/Article/details/ghenpivus.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gnltyshdv.sHtML

[U97] JS：并发请求
来源：http://www.share.sjlbkw.cn/Article/details/gmjzhkqjv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/geshekfxt.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fktsv.cn/Article/details/gyfoenrcm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.sjlbkw.cn/Article/details/geqfpnmck.sHtML

[U99] JS：事件监听
来源：http://www.share.bbcook.cn/Article/details/ggdaagksq.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fktsv.cn/Article/details/gxtpqzvpn.sHtML

[U100] JS：DOM 查询
来源：http://3g.epnwcf.com/Article/details/gvbltjdhp.sHtML

document.querySelector(".item")
来源：http://mobile.bbcook.cn/Article/details/gfxpgogar.sHtML

[U101] JS：classList 操作
来源：http://mobile.vehdjk.com/Article/details/gegiqonmb.sHtML

el.classList.toggle("active")
来源：http://www.share.sjlbkw.cn/Article/details/gjsuwsokm.sHtML

[U102] JS：本地存储
来源：http://www.m.share.sjlbkw.cn/Article/details/gldacidex.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.vehdjk.com/Article/details/gigdyjedq.sHtML

[U103] JS：定时器
来源：http://wap.sjlbkw.cn/Article/details/glulyhhmz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.yfazqb.com/Article/details/ggcenamaz.sHtML

[U104] JS：防抖
来源：http://www.m.share.yfazqb.com/Article/details/giregtngo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gilzcnxzy.sHtML

[U105] JS：节流
来源：http://m.share.tarul.cn/Article/details/gknmpjihp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.yfazqb.com/Article/details/gonkvikmc.sHtML

[U106] JS：日期格式化
来源：http://read.share.vehdjk.com/Article/details/gfrnoqumd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.vehdjk.com/Article/details/gqyrhmbip.sHtML

[U107] JS：数字千分位
来源：http://wap.vehdjk.com/Article/details/gtgcyywuq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gbrwyabhx.sHtML

[U108] JS：随机整数
来源：http://baike.vehdjk.com/Article/details/giajzcxzn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.yfazqb.com/Article/details/glplwgvnd.sHtML

[U109] JS：数组分组
来源：http://wap.yfazqb.com/Article/details/grozofsvk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/gymbcsuwn.sHtML

[U110] JS：数组分块
来源：http://blog.vehdjk.com/Article/details/goxrxtuef.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.epnwcf.com/Article/details/ggztaztxu.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.epnwcf.com/Article/details/gxodkazmh.sHtML

new Map(Object.entries(obj))
来源：http://www.share.vehdjk.com/Article/details/gthzvxkcm.sHtML

[U112] JS：字符串补位
来源：http://baike.fktsv.cn/Article/details/gcvpxgccg.sHtML

"7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/grdwftojx.sHtML

[U113] JS：正则替换全部
来源：http://wap.tarul.cn/Article/details/gnocavfjh.sHtML

s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gzbqonfhd.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fktsv.cn/Article/details/glthbfiqm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gcoqrmtph.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.sjlbkw.cn/Article/details/glzdahmkl.sHtML

crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gtmbmzhqf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fktsv.cn/Article/details/gksonpoll.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fktsv.cn/Article/details/gnzrouiro.sHtML

[U117] JS：单元测试
来源：http://www.m.share.vehdjk.com/Article/details/ggnhwifni.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.yfazqb.com/Article/details/gcdmhwwxz.sHtML

[U118] JS：开发服务器
来源：http://www.share.bbcook.cn/Article/details/gzhbsxrfa.sHtML

npm i -D vite;  npx vite
来源：http://blog.bbcook.cn/Article/details/gfzbxfzgn.sHtML

[U119] JS：生产构建
来源：http://read.share.yfazqb.com/Article/details/gjvqmqxds.sHtML

npx vite build
来源：http://wap.tarul.cn/Article/details/giyglzalx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fktsv.cn/Article/details/gpmzwlpon.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.yfazqb.com/Article/details/gafogdtyj.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gflejubmg.sHtML

统计汇总
来源：http://www.share.epnwcf.com/Article/details/gfcpwwmfa.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqsqgxlmp.sHtML

按语言统计（条）：
来源：http://www.share.sjlbkw.cn/Article/details/gwlxrfdfz.sHtML

Python ......... 252
来源：http://www.share.bbcook.cn/Article/details/gzoykcncc.sHtML

PHP ............ 252
来源：http://wap.sjlbkw.cn/Article/details/gecwfpeuv.sHtML

JavaScript ..... 252
来源：http://3g.sjlbkw.cn/Article/details/gsxuxjttu.sHtML

TypeScript ..... 212
来源：http://www.m.share.epnwcf.com/Article/details/gekcgnblx.sHtML

Java ........... 212
来源：http://read.share.vehdjk.com/Article/details/gqrusvzhc.sHtML

Go ............. 212
来源：http://baike.epnwcf.com/Article/details/ggwkouhvh.sHtML

Ruby ........... 212
来源：http://3g.yfazqb.com/Article/details/gtgbaydqm.sHtML

C# ............. 212
来源：http://wap.tarul.cn/Article/details/guadpzzql.sHtML

C .............. 30
来源：http://www.share.epnwcf.com/Article/details/godehhuun.sHtML

C++ ............ 30
来源：http://blog.vehdjk.com/Article/details/gwjjwijov.sHtML

SQL ............ 90
来源：http://baike.yfazqb.com/Article/details/gkynqtvqe.sHtML

Bash ........... 80
来源：http://blog.fktsv.cn/Article/details/gesbujpvy.sHtML

Kotlin ......... 15
来源：http://blog.vehdjk.com/Article/details/gmnnulced.sHtML

Swift .......... 15
来源：http://baike.fktsv.cn/Article/details/gvdeafzkr.sHtML

Lua ............ 10
来源：http://3g.tarul.cn/Article/details/gppcmwhre.sHtML

Perl ........... 10
来源：http://www.m.share.epnwcf.com/Article/details/gyekkxygo.sHtML

Scala .......... 10
来源：http://www.share.fktsv.cn/Article/details/gvfqaczda.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/gijzzcunz.sHtML

合计 ........... 2106 条
来源：http://www.share.sjlbkw.cn/Article/details/glqleiesq.sHtML

按章节统计：
来源：http://m.share.sjlbkw.cn/Article/details/gnzgksrmj.sHtML


<!-- 参考信息 -->