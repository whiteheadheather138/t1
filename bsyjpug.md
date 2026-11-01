代发 wailian999

[T47] Perl：正则捕获
来源：http://blog.tarul.cn/Article/details/gljefprfs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fktsv.cn/Article/details/gyqiuclch.sHtML

[T48] Perl：正则替换
来源：http://wap.bbcook.cn/Article/details/ggdtxegrw.sHtML

$s =~ s/old/new/g;
来源：http://wap.yfazqb.com/Article/details/goqxymbua.sHtML

[T49] Perl：函数
来源：http://wap.sjlbkw.cn/Article/details/guxqaujbl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/goyyybwfv.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gklmmozuu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/ggwcqleqn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.epnwcf.com/Article/details/gxyogbaqn.sHtML

[T51] Scala：Hello World
来源：http://blog.vehdjk.com/Article/details/guqtkyglk.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gckqjrptu.sHtML

[T52] Scala：变量
来源：http://www.m.share.tarul.cn/Article/details/gxwmgqywn.sHtML

val a = 1;  var b = 2
来源：http://wap.tarul.cn/Article/details/gviplshiq.sHtML

[T53] Scala：字符串插值
来源：http://www.share.epnwcf.com/Article/details/ggfciyqvh.sHtML

s"值: $b"
来源：http://blog.epnwcf.com/Article/details/gggivgihe.sHtML

[T54] Scala：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gvrtrtbza.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.epnwcf.com/Article/details/gsxyrswzp.sHtML

[T55] Scala：集合过滤
来源：http://m.share.tarul.cn/Article/details/glzntyahr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.bbcook.cn/Article/details/gqojmobfi.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fktsv.cn/Article/details/grjcvovny.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.vehdjk.com/Article/details/gyhkncnrg.sHtML

[T57] Scala：模式匹配
来源：http://baike.yfazqb.com/Article/details/gigtbcofu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.yfazqb.com/Article/details/ggargksxr.sHtML

[T58] Scala：函数定义
来源：http://www.share.fktsv.cn/Article/details/gyyeypfhy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.vehdjk.com/Article/details/gqkdyptbu.sHtML

[T59] Scala：循环
来源：http://3g.vehdjk.com/Article/details/gcglcbcfm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gaijbvovz.sHtML

[T60] Scala：折叠
来源：http://mobile.bbcook.cn/Article/details/gromttxdq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.sjlbkw.cn/Article/details/ghczrdwcq.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grlqqkcpv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/gvfmypdsa.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gltyyuvwb.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.epnwcf.com/Article/details/gqjalonvu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.tarul.cn/Article/details/gpyeespet.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.tarul.cn/Article/details/ghpmswdsw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.tarul.cn/Article/details/gocofvpdm.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.epnwcf.com/Article/details/ghhznqsao.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.epnwcf.com/Article/details/gixczmrwa.sHtML

[U04] Py：变量调试打印
来源：http://wap.vehdjk.com/Article/details/ggaxsdvcc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fktsv.cn/Article/details/gwuvbtmin.sHtML

[U05] Py：列表去重且保序
来源：http://wap.epnwcf.com/Article/details/gozincnla.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gsbrgohjy.sHtML

[U06] Py：合并两个字典
来源：http://wap.epnwcf.com/Article/details/gievhijdk.sHtML

{**a, **b}
来源：http://mobile.fktsv.cn/Article/details/grfcdfegd.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fktsv.cn/Article/details/gluyzohmi.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.vehdjk.com/Article/details/gmqxpjgwz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.epnwcf.com/Article/details/gjoqkexwc.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fktsv.cn/Article/details/gfpypvlho.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fktsv.cn/Article/details/gloqjyyha.sHtML

max(d, key=d.get)
来源：http://www.share.tarul.cn/Article/details/glnklugde.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.vehdjk.com/Article/details/gxhpvenmd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.bbcook.cn/Article/details/grmxdrrds.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.bbcook.cn/Article/details/gqyrzbqhi.sHtML

(x * 2 for x in arr)
来源：http://www.share.bbcook.cn/Article/details/gsfkeolia.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fktsv.cn/Article/details/gsnimbelq.sHtML

Counter(arr).most_common(3)
来源：http://3g.bbcook.cn/Article/details/geatrumwx.sHtML

[U13] Py：固定长度队列
来源：http://wap.vehdjk.com/Article/details/gqtlkhfvp.sHtML

deque(maxlen=10)
来源：http://www.share.epnwcf.com/Article/details/gndtsepwd.sHtML

[U14] Py：分组收集到列表
来源：http://blog.bbcook.cn/Article/details/geyicbmsl.sHtML

defaultdict(list)
来源：http://wap.fktsv.cn/Article/details/gqlyutxmr.sHtML

[U15] Py：高精度计时
来源：http://3g.vehdjk.com/Article/details/gdhpsimpm.sHtML

t = time.perf_counter()
来源：http://www.m.share.fktsv.cn/Article/details/gjiahweqb.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.yfazqb.com/Article/details/gwuovbuzj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.tarul.cn/Article/details/guluegixs.sHtML

[U17] Py：初始化日志
来源：http://mobile.tarul.cn/Article/details/guzldnkwy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fktsv.cn/Article/details/gdjxmwjhj.sHtML

[U18] Py：预编译正则
来源：http://3g.sjlbkw.cn/Article/details/gylpbdpns.sHtML

pat = re.compile(r"\d+")
来源：http://3g.yfazqb.com/Article/details/gwplfwute.sHtML

[U19] Py：正则替换带回调
来源：http://3g.sjlbkw.cn/Article/details/gspipoqil.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.bbcook.cn/Article/details/gvbpinpei.sHtML

[U20] Py：缓存函数结果
来源：http://blog.sjlbkw.cn/Article/details/grlrsscyc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.vehdjk.com/Article/details/ggzxmsbbm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.yfazqb.com/Article/details/gohwnencf.sHtML

@contextlib.contextmanager
来源：http://www.blog.bbcook.cn/Article/details/gmagedgnn.sHtML

[U22] Py：矩阵转置
来源：http://www.share.yfazqb.com/Article/details/gkkztpmyu.sHtML

list(zip(*m))
来源：http://www.blog.epnwcf.com/Article/details/gsguhmlqf.sHtML

[U23] Py：分块读取大文件
来源：http://blog.tarul.cn/Article/details/gslsazwjy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.sjlbkw.cn/Article/details/grktsiqfa.sHtML

[U24] Py：路径操作
来源：http://blog.tarul.cn/Article/details/ghyxhhqkn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/geqbavdkv.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fktsv.cn/Article/details/ghtnqkerx.sHtML

csv.DictReader(f)
来源：http://blog.yfazqb.com/Article/details/gvgzodhrk.sHtML

[U26] Py：并发下载
来源：http://blog.epnwcf.com/Article/details/gniiaqiwe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.tarul.cn/Article/details/gcfsuwici.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.bbcook.cn/Article/details/getwdaaep.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.epnwcf.com/Article/details/gnkbcgwov.sHtML

[U28] Py：类型别名
来源：http://3g.fktsv.cn/Article/details/gevqpkrzm.sHtML

UserId = int
来源：http://read.share.sjlbkw.cn/Article/details/gfskgwvdr.sHtML

[U29] Py：属性校验
来源：http://mobile.tarul.cn/Article/details/gxxsglrbf.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.sjlbkw.cn/Article/details/gealvrhsq.sHtML

[U30] Py：数据类
来源：http://wap.fktsv.cn/Article/details/ghugtmsoo.sHtML

@dataclass(slots=True)
来源：http://m.share.bbcook.cn/Article/details/goduxuyaj.sHtML

[U31] Py：单测
来源：http://3g.sjlbkw.cn/Article/details/gyuaiucgb.sHtML

python -m pytest -q
来源：http://www.m.share.fktsv.cn/Article/details/gjfyqcbtm.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.epnwcf.com/Article/details/ggrbzawch.sHtML

ruff format . && ruff check --fix .
来源：http://baike.vehdjk.com/Article/details/grrkkmnnp.sHtML

[U33] Py：打包发布
来源：http://blog.epnwcf.com/Article/details/gjosjdgdw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.yfazqb.com/Article/details/gkisoetco.sHtML

[U34] Py：判断编码
来源：http://mobile.tarul.cn/Article/details/giuqikuld.sHtML

chardet.detect(raw)
来源：http://wap.yfazqb.com/Article/details/gbsqigjth.sHtML

[U35] Py：发送邮件
来源：http://mobile.fktsv.cn/Article/details/glrvtqmkv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.tarul.cn/Article/details/gvnonprdc.sHtML

[U36] Py：定时任务
来源：http://m.share.fktsv.cn/Article/details/gqcwcuoux.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.yfazqb.com/Article/details/gyclevydl.sHtML

[U37] Py：读写 Excel
来源：http://mobile.yfazqb.com/Article/details/grtvrilve.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.yfazqb.com/Article/details/ghwgvzdxf.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.bbcook.cn/Article/details/gqyvwvseg.sHtML

Path(__file__).resolve().parent
来源：http://m.share.epnwcf.com/Article/details/gjykyvlzz.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.tarul.cn/Article/details/gfvrxrkuu.sHtML

sys.stdout.isatty()
来源：http://read.share.epnwcf.com/Article/details/gajoefnsu.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.yfazqb.com/Article/details/gtslplggd.sHtML

print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gunahqpdp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.vehdjk.com/Article/details/gfncshcno.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.bbcook.cn/Article/details/gnfxwrauu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.epnwcf.com/Article/details/gjbtiattj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.tarul.cn/Article/details/gnkojqqrs.sHtML

[U43] PHP：声明命名空间
来源：http://wap.bbcook.cn/Article/details/gfwmorngi.sHtML

namespace App\Http;
来源：http://www.blog.yfazqb.com/Article/details/gqwhufsvu.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.sjlbkw.cn/Article/details/glolrppky.sHtML

declare(strict_types=1);
来源：http://www.share.epnwcf.com/Article/details/gyjlaslhj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.bbcook.cn/Article/details/ghjefjszc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gtsfoakqx.sHtML

[U46] PHP：可空类型
来源：http://m.share.fktsv.cn/Article/details/gtaquyiky.sHtML

?string $name = null
来源：http://www.blog.epnwcf.com/Article/details/gopbfxkht.sHtML

[U47] PHP：联合类型
来源：http://wap.tarul.cn/Article/details/gtnzmtads.sHtML

int|string $id
来源：http://m.share.tarul.cn/Article/details/gxwcmitcr.sHtML

[U48] PHP：纯枚举
来源：http://read.share.sjlbkw.cn/Article/details/gutqxkyjd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.epnwcf.com/Article/details/gbjbivmmb.sHtML

[U49] PHP：只读属性
来源：http://www.share.bbcook.cn/Article/details/gdfwmeybi.sHtML

public readonly string $name
来源：http://baike.epnwcf.com/Article/details/gludhtuws.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.vehdjk.com/Article/details/gmhkvpdzu.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fktsv.cn/Article/details/gejktbrqp.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.tarul.cn/Article/details/gpoubxujx.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.vehdjk.com/Article/details/gvocdfxaj.sHtML

[U52] PHP：箭头函数
来源：http://3g.fktsv.cn/Article/details/gyncukdqp.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fktsv.cn/Article/details/geetxetdc.sHtML

[U53] PHP：空合并运算符
来源：http://blog.sjlbkw.cn/Article/details/gqtpdshjl.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.sjlbkw.cn/Article/details/galchjyqa.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fktsv.cn/Article/details/gbeacawmt.sHtML

$obj?->method()
来源：http://www.m.share.tarul.cn/Article/details/gaopcggsz.sHtML

[U55] PHP：match 表达式
来源：http://mobile.bbcook.cn/Article/details/gdqfneiep.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fktsv.cn/Article/details/geketgwfd.sHtML

[U56] PHP：命名参数
来源：http://read.share.vehdjk.com/Article/details/gjgijyldj.sHtML

f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gtjrhkhmz.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gusttwjak.sHtML

"值: {$a}"
来源：http://www.share.vehdjk.com/Article/details/gysqetvmm.sHtML

[U58] PHP：数组三件套
来源：http://m.share.bbcook.cn/Article/details/gjhaiojfu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.vehdjk.com/Article/details/gwhfhylbc.sHtML

[U59] PHP：自定义排序
来源：http://3g.vehdjk.com/Article/details/gacnsxbcn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.bbcook.cn/Article/details/gqccktlvt.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fktsv.cn/Article/details/grbwisbqs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.sjlbkw.cn/Article/details/gawsnubkl.sHtML

[U61] PHP：正则
来源：http://3g.yfazqb.com/Article/details/ggfneopuk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gadhhtuqa.sHtML

[U62] PHP：日期对象
来源：http://www.share.vehdjk.com/Article/details/gnqqpmodr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.yfazqb.com/Article/details/gwuzmgrgj.sHtML

[U63] PHP：文件读写
来源：http://m.share.tarul.cn/Article/details/gybrgamvr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.tarul.cn/Article/details/grmgrrhek.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.bbcook.cn/Article/details/gkedepasz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.bbcook.cn/Article/details/gxhzgjiyg.sHtML

[U65] PHP：会话
来源：http://baike.epnwcf.com/Article/details/ggeinzskm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/ghzygwjai.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fktsv.cn/Article/details/gukvivuxs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gzimfcxtb.sHtML

[U67] PHP：处理文件上传
来源：http://baike.vehdjk.com/Article/details/gxspawpnv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.sjlbkw.cn/Article/details/gpcjynxip.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.epnwcf.com/Article/details/gjvcwngxg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.tarul.cn/Article/details/gwkgnrwpx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.tarul.cn/Article/details/gmsrqlwvq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.bbcook.cn/Article/details/gtcrpnzex.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.bbcook.cn/Article/details/gygjlsyvd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.epnwcf.com/Article/details/gbzplkhdn.sHtML

[U71] PHP：抛出异常
来源：http://www.share.tarul.cn/Article/details/gygjgmlwk.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.bbcook.cn/Article/details/gsbfoacgj.sHtML

[U72] PHP：写错误日志
来源：http://wap.sjlbkw.cn/Article/details/gepipojao.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.sjlbkw.cn/Article/details/gjdytwdze.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fktsv.cn/Article/details/gdwvuomcj.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.bbcook.cn/Article/details/ggzufxwky.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gmpgezrdp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fktsv.cn/Article/details/geugjchzm.sHtML

[U75] PHP：依赖注入
来源：http://mobile.vehdjk.com/Article/details/gtrkrazgk.sHtML

composer require psr/container
来源：http://3g.vehdjk.com/Article/details/gwxrgadds.sHtML

[U76] PHP：简单路由
来源：http://read.share.yfazqb.com/Article/details/glckpotjm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.sjlbkw.cn/Article/details/gnwhnnqic.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.yfazqb.com/Article/details/grcrvpigi.sHtML

composer require twig/twig
来源：http://www.m.share.sjlbkw.cn/Article/details/gegaljydk.sHtML

[U78] PHP：单元测试
来源：http://m.share.fktsv.cn/Article/details/gayujjdwx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.yfazqb.com/Article/details/givjphxos.sHtML

[U79] PHP：静态分析
来源：http://www.share.epnwcf.com/Article/details/gszhuabbj.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.tarul.cn/Article/details/gitlelwdv.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fktsv.cn/Article/details/gkampeayt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.vehdjk.com/Article/details/gcxdnzzmp.sHtML

[U81] JS：初始化项目
来源：http://blog.epnwcf.com/Article/details/gdnbdoriz.sHtML

npm init -y;  npm i express
来源：http://blog.tarul.cn/Article/details/gnsrvigzi.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fktsv.cn/Article/details/ggcqifpgn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.vehdjk.com/Article/details/glweqgljk.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fktsv.cn/Article/details/gyvpolbfx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gdzenihlc.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.yfazqb.com/Article/details/gopyobtmq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fktsv.cn/Article/details/ggrmpalfw.sHtML

[U85] JS：可选链
来源：http://blog.tarul.cn/Article/details/gnbmdhniu.sHtML

a?.b?.c
来源：http://www.share.sjlbkw.cn/Article/details/gtexxofgp.sHtML

[U86] JS：空值合并
来源：http://www.m.share.yfazqb.com/Article/details/gakaecmxf.sHtML

a ?? b
来源：http://wap.vehdjk.com/Article/details/gzbwjhgka.sHtML

[U87] JS：解构默认值
来源：http://baike.vehdjk.com/Article/details/gicasicjm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fktsv.cn/Article/details/gbdpgwjbn.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fktsv.cn/Article/details/glwcvlsjy.sHtML

{ ...a, ...b }
来源：http://m.share.vehdjk.com/Article/details/gyyxdiboh.sHtML

[U89] JS：数组去重
来源：http://www.m.share.bbcook.cn/Article/details/ghahqygaw.sHtML

[...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/glntkbhfa.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.epnwcf.com/Article/details/gssiezwxp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gwoglolkf.sHtML

[U91] JS：对象键值遍历
来源：http://baike.yfazqb.com/Article/details/gzelcidyr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.yfazqb.com/Article/details/gbijulsdu.sHtML

[U92] JS：深拷贝
来源：http://www.blog.bbcook.cn/Article/details/gfhpspgyw.sHtML

structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gzuubdogb.sHtML

[U93] JS：模板字符串
来源：http://wap.yfazqb.com/Article/details/gkstfgcwj.sHtML

`共 ${n} 条`
来源：http://blog.fktsv.cn/Article/details/gwsmsemjn.sHtML

[U94] JS：箭头函数
来源：http://wap.epnwcf.com/Article/details/ggnorcidz.sHtML

const double = x => x * 2;
来源：http://mobile.yfazqb.com/Article/details/ghphortnf.sHtML

[U95] JS：Promise 包装
来源：http://3g.fktsv.cn/Article/details/gseliwmib.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.bbcook.cn/Article/details/gszkfzrxv.sHtML

[U96] JS：async/await 与异常
来源：http://blog.yfazqb.com/Article/details/gtlojtoqc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gzuwlktoq.sHtML

[U97] JS：并发请求
来源：http://m.share.yfazqb.com/Article/details/gyrbhyxoo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gogeganir.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.tarul.cn/Article/details/gdzvjacpp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.bbcook.cn/Article/details/gguhwmyzk.sHtML

[U99] JS：事件监听
来源：http://wap.tarul.cn/Article/details/ggvyjwubq.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.yfazqb.com/Article/details/gbrqkushn.sHtML

[U100] JS：DOM 查询
来源：http://read.share.yfazqb.com/Article/details/gzpsoereo.sHtML

document.querySelector(".item")
来源：http://wap.bbcook.cn/Article/details/gahvxzdne.sHtML

[U101] JS：classList 操作
来源：http://read.share.vehdjk.com/Article/details/ggtvfeauf.sHtML

el.classList.toggle("active")
来源：http://mobile.vehdjk.com/Article/details/gukprnbmq.sHtML

[U102] JS：本地存储
来源：http://m.share.yfazqb.com/Article/details/gafssimyw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.yfazqb.com/Article/details/gpjvcfrwo.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/gcklixmby.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.epnwcf.com/Article/details/gvkufuzhb.sHtML

[U104] JS：防抖
来源：http://baike.bbcook.cn/Article/details/gprfdaqtb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gnaiuvezh.sHtML

[U105] JS：节流
来源：http://www.share.yfazqb.com/Article/details/gveunwxkn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.tarul.cn/Article/details/ggmeoatrf.sHtML

[U106] JS：日期格式化
来源：http://m.share.epnwcf.com/Article/details/gozwyimyi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.tarul.cn/Article/details/gvvsqxmtz.sHtML

[U107] JS：数字千分位
来源：http://read.share.yfazqb.com/Article/details/ghctqresq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.tarul.cn/Article/details/gydlcijtg.sHtML

[U108] JS：随机整数
来源：http://www.share.yfazqb.com/Article/details/gppjbzbrk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.tarul.cn/Article/details/gntafqavf.sHtML

[U109] JS：数组分组
来源：http://3g.sjlbkw.cn/Article/details/grrottsgm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/gssrlteev.sHtML

[U110] JS：数组分块
来源：http://www.share.tarul.cn/Article/details/gpziukily.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.vehdjk.com/Article/details/ggathaglf.sHtML

[U111] JS：对象转 Map
来源：http://read.share.vehdjk.com/Article/details/gekxouzfo.sHtML

new Map(Object.entries(obj))
来源：http://m.share.bbcook.cn/Article/details/gqcyocega.sHtML

[U112] JS：字符串补位
来源：http://www.share.epnwcf.com/Article/details/gfuvfnapg.sHtML

"7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gunvolngj.sHtML

[U113] JS：正则替换全部
来源：http://blog.epnwcf.com/Article/details/gmrkzvvoi.sHtML

s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gmsqkhjip.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.epnwcf.com/Article/details/gffusjcnl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/garuevacd.sHtML

[U115] JS：生成 UUID
来源：http://3g.tarul.cn/Article/details/gfpgkapog.sHtML

crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gznralgmz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.bbcook.cn/Article/details/gnomrwzsd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fktsv.cn/Article/details/gyhxcjvrd.sHtML

[U117] JS：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gfbeccgqx.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.tarul.cn/Article/details/gzbhdmpcz.sHtML

[U118] JS：开发服务器
来源：http://m.share.yfazqb.com/Article/details/gnpzloljv.sHtML

npm i -D vite;  npx vite
来源：http://mobile.epnwcf.com/Article/details/genukcbtp.sHtML

[U119] JS：生产构建
来源：http://blog.tarul.cn/Article/details/gjpzhmbjg.sHtML

npx vite build
来源：http://read.share.bbcook.cn/Article/details/gifviqwgf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.epnwcf.com/Article/details/giakpcsdf.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.tarul.cn/Article/details/gbwbbykiv.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gszfpczcb.sHtML

统计汇总
来源：http://www.share.bbcook.cn/Article/details/gndajvwia.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvvggngqq.sHtML

按语言统计（条）：
来源：http://blog.fktsv.cn/Article/details/gjykajhbd.sHtML

Python ......... 252
来源：http://read.share.bbcook.cn/Article/details/gjpfgryqk.sHtML

PHP ............ 252
来源：http://blog.yfazqb.com/Article/details/gxkvpufvr.sHtML

JavaScript ..... 252
来源：http://read.share.vehdjk.com/Article/details/giwjxabdg.sHtML

TypeScript ..... 212
来源：http://www.m.share.epnwcf.com/Article/details/gfijuidfv.sHtML

Java ........... 212
来源：http://www.blog.fktsv.cn/Article/details/gajtuwgrs.sHtML

Go ............. 212
来源：http://www.m.share.tarul.cn/Article/details/godnzolhn.sHtML

Ruby ........... 212
来源：http://wap.tarul.cn/Article/details/ghdwqttax.sHtML

C# ............. 212
来源：http://www.blog.fktsv.cn/Article/details/gfmnqoeqg.sHtML

C .............. 30
来源：http://baike.sjlbkw.cn/Article/details/gwxyhgsvy.sHtML

C++ ............ 30
来源：http://3g.bbcook.cn/Article/details/gdrlauwqh.sHtML

SQL ............ 90
来源：http://www.m.share.epnwcf.com/Article/details/gxvnhdoqv.sHtML

Bash ........... 80
来源：http://3g.fktsv.cn/Article/details/gqpcrmyme.sHtML

Kotlin ......... 15
来源：http://blog.epnwcf.com/Article/details/gkmszmqjk.sHtML

Swift .......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gvqthbxno.sHtML

Lua ............ 10
来源：http://m.share.epnwcf.com/Article/details/gshhxhkxt.sHtML

Perl ........... 10
来源：http://mobile.epnwcf.com/Article/details/grvtvnfif.sHtML

Scala .......... 10
来源：http://read.share.sjlbkw.cn/Article/details/gyhquqjxu.sHtML

------------------------------------
来源：http://mobile.tarul.cn/Article/details/gikhlquls.sHtML

合计 ........... 2106 条
来源：http://wap.vehdjk.com/Article/details/gzkgiawrl.sHtML

按章节统计：
来源：http://wap.tarul.cn/Article/details/gtildsmng.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.epnwcf.com/Article/details/gwesdzvlo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/gddvwmwzi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/ggkvqvtpe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.bbcook.cn/Article/details/gqaqrqevj.sHtML


<!-- 参考信息 -->