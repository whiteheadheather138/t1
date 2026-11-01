代发 wailian999

[T45] Perl：数组遍历
来源：http://3g.tarul.cn/Article/details/giagosduc.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.epnwcf.com/Article/details/gmeyyzvfn.sHtML

[T46] Perl：哈希操作
来源：http://m.share.epnwcf.com/Article/details/gayegixta.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.vehdjk.com/Article/details/gcjaxhamj.sHtML

[T47] Perl：正则捕获
来源：http://baike.vehdjk.com/Article/details/gdklulese.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.epnwcf.com/Article/details/geilqlzgv.sHtML

[T48] Perl：正则替换
来源：http://wap.vehdjk.com/Article/details/gwvrrgjwr.sHtML

$s =~ s/old/new/g;
来源：http://wap.vehdjk.com/Article/details/gdsirqici.sHtML

[T49] Perl：函数
来源：http://wap.vehdjk.com/Article/details/gjpuxqlfq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gesdxslos.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fktsv.cn/Article/details/glyvenqlr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.sjlbkw.cn/Article/details/ggrwmwtno.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.bbcook.cn/Article/details/gfckvzrux.sHtML

[T51] Scala：Hello World
来源：http://blog.bbcook.cn/Article/details/gqmgirgsu.sHtML

println("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gafqndsdt.sHtML

[T52] Scala：变量
来源：http://www.blog.tarul.cn/Article/details/grejqcfwx.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.tarul.cn/Article/details/gpsdyzqrl.sHtML

[T53] Scala：字符串插值
来源：http://baike.yfazqb.com/Article/details/gjmmilqzq.sHtML

s"值: $b"
来源：http://wap.fktsv.cn/Article/details/gkrbdktqm.sHtML

[T54] Scala：集合映射
来源：http://m.share.bbcook.cn/Article/details/gzumcjtfc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.bbcook.cn/Article/details/glstggeib.sHtML

[T55] Scala：集合过滤
来源：http://baike.bbcook.cn/Article/details/grpfpqkpm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.yfazqb.com/Article/details/gqbrqkzcr.sHtML

[T56] Scala：样例类
来源：http://3g.vehdjk.com/Article/details/gffapmgtc.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gqufgypxj.sHtML

[T57] Scala：模式匹配
来源：http://blog.fktsv.cn/Article/details/gvctzhufw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.bbcook.cn/Article/details/guujxzidd.sHtML

[T58] Scala：函数定义
来源：http://baike.vehdjk.com/Article/details/guumwrqdu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fktsv.cn/Article/details/gtgutoioj.sHtML

[T59] Scala：循环
来源：http://baike.epnwcf.com/Article/details/gayvbkwbe.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.tarul.cn/Article/details/gkfjyshyf.sHtML

[T60] Scala：折叠
来源：http://mobile.sjlbkw.cn/Article/details/gpnjmijed.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.epnwcf.com/Article/details/ghkbnsupt.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghjmzbgyw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.tarul.cn/Article/details/grywdbece.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gzemkrjkn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.epnwcf.com/Article/details/gqjmghvwa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fktsv.cn/Article/details/gylodlxfc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.bbcook.cn/Article/details/gxwrbexbz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.epnwcf.com/Article/details/gwcitafyu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fktsv.cn/Article/details/gmvhlfgvr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.epnwcf.com/Article/details/gwnwcrwko.sHtML

[U04] Py：变量调试打印
来源：http://blog.sjlbkw.cn/Article/details/gbfnqoilp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.yfazqb.com/Article/details/gpmcwqstp.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.epnwcf.com/Article/details/gfktctgzg.sHtML

list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/gedztaumu.sHtML

[U06] Py：合并两个字典
来源：http://www.share.sjlbkw.cn/Article/details/gvvepcpvr.sHtML

{**a, **b}
来源：http://m.share.fktsv.cn/Article/details/gajbjksnk.sHtML

[U07] Py：反转字典键值
来源：http://wap.bbcook.cn/Article/details/gqbvfwmcb.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.tarul.cn/Article/details/ghjfjopuh.sHtML

[U08] Py：展平二维列表
来源：http://wap.yfazqb.com/Article/details/guwnodijr.sHtML

[y for x in nested for y in x]
来源：http://blog.yfazqb.com/Article/details/gqydfbfht.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fktsv.cn/Article/details/gjfdpiuud.sHtML

max(d, key=d.get)
来源：http://m.share.tarul.cn/Article/details/grtsgobcp.sHtML

[U10] Py：按值排序字典
来源：http://baike.fktsv.cn/Article/details/gskmmbnzh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.sjlbkw.cn/Article/details/gjrvgbrqf.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.vehdjk.com/Article/details/gdmohsagq.sHtML

(x * 2 for x in arr)
来源：http://mobile.sjlbkw.cn/Article/details/geqcbmqrb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.sjlbkw.cn/Article/details/gmaghldrn.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.sjlbkw.cn/Article/details/ggthweduz.sHtML

[U13] Py：固定长度队列
来源：http://blog.vehdjk.com/Article/details/gzoqvkonz.sHtML

deque(maxlen=10)
来源：http://www.m.share.epnwcf.com/Article/details/gegphudnu.sHtML

[U14] Py：分组收集到列表
来源：http://3g.tarul.cn/Article/details/gnuxlbpgm.sHtML

defaultdict(list)
来源：http://www.m.share.vehdjk.com/Article/details/gopxbgsij.sHtML

[U15] Py：高精度计时
来源：http://www.share.tarul.cn/Article/details/gxfvvxzbj.sHtML

t = time.perf_counter()
来源：http://3g.vehdjk.com/Article/details/ggdofqvdh.sHtML

[U16] Py：命令行参数解析
来源：http://wap.sjlbkw.cn/Article/details/gnrfpftmc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.sjlbkw.cn/Article/details/gsdhfcvst.sHtML

[U17] Py：初始化日志
来源：http://baike.tarul.cn/Article/details/gfdkaaitt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmvpvwnh.sHtML

[U18] Py：预编译正则
来源：http://wap.sjlbkw.cn/Article/details/grtrilfpj.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.yfazqb.com/Article/details/gpkfwvsdy.sHtML

[U19] Py：正则替换带回调
来源：http://baike.sjlbkw.cn/Article/details/geehamzjm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.epnwcf.com/Article/details/gnkkfacjg.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.vehdjk.com/Article/details/gckbpzfbg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.sjlbkw.cn/Article/details/gyhrhglou.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.sjlbkw.cn/Article/details/gqyhnugoj.sHtML

@contextlib.contextmanager
来源：http://m.share.fktsv.cn/Article/details/gsbzmycac.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.yfazqb.com/Article/details/ghrvlhmqu.sHtML

list(zip(*m))
来源：http://mobile.bbcook.cn/Article/details/gcpjkctpk.sHtML

[U23] Py：分块读取大文件
来源：http://blog.vehdjk.com/Article/details/gtvoecvrh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.bbcook.cn/Article/details/gjwoxfkjh.sHtML

[U24] Py：路径操作
来源：http://m.share.sjlbkw.cn/Article/details/gxhgckqyo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.yfazqb.com/Article/details/gjhsbzsdz.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.vehdjk.com/Article/details/gujfavvsm.sHtML

csv.DictReader(f)
来源：http://m.share.tarul.cn/Article/details/gdoxvuspi.sHtML

[U26] Py：并发下载
来源：http://wap.bbcook.cn/Article/details/gztlgiftq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.vehdjk.com/Article/details/gfteqjvry.sHtML

[U27] Py：异步 HTTP
来源：http://3g.epnwcf.com/Article/details/gjtptcpkq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.tarul.cn/Article/details/gqgfrledy.sHtML

[U28] Py：类型别名
来源：http://www.m.share.epnwcf.com/Article/details/gxvovtpgq.sHtML

UserId = int
来源：http://www.m.share.bbcook.cn/Article/details/gcnqtuolj.sHtML

[U29] Py：属性校验
来源：http://mobile.fktsv.cn/Article/details/gmtfaoedk.sHtML

@property 与 @x.setter 配合
来源：http://3g.fktsv.cn/Article/details/gipfnmcbx.sHtML

[U30] Py：数据类
来源：http://baike.epnwcf.com/Article/details/gnnfmrqul.sHtML

@dataclass(slots=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/grgrinrxc.sHtML

[U31] Py：单测
来源：http://www.m.share.yfazqb.com/Article/details/gjenvbtwl.sHtML

python -m pytest -q
来源：http://wap.tarul.cn/Article/details/gfofffbxh.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.vehdjk.com/Article/details/gqnnjqxog.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.sjlbkw.cn/Article/details/gjudfaoqe.sHtML

[U33] Py：打包发布
来源：http://wap.sjlbkw.cn/Article/details/grhxkrvjp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.epnwcf.com/Article/details/gstklkdlh.sHtML

[U34] Py：判断编码
来源：http://www.share.bbcook.cn/Article/details/gvwiztvhd.sHtML

chardet.detect(raw)
来源：http://baike.bbcook.cn/Article/details/gcvvnjefn.sHtML

[U35] Py：发送邮件
来源：http://mobile.sjlbkw.cn/Article/details/gjyqeplzo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.vehdjk.com/Article/details/grbgtthij.sHtML

[U36] Py：定时任务
来源：http://read.share.fktsv.cn/Article/details/gwfsmxluf.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.sjlbkw.cn/Article/details/gweijkxpp.sHtML

[U37] Py：读写 Excel
来源：http://3g.yfazqb.com/Article/details/ghueoiwur.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.bbcook.cn/Article/details/ggaglqowg.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fktsv.cn/Article/details/guoajwehe.sHtML

Path(__file__).resolve().parent
来源：http://www.share.yfazqb.com/Article/details/gsywtjpbd.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fktsv.cn/Article/details/gehtteaud.sHtML

sys.stdout.isatty()
来源：http://3g.epnwcf.com/Article/details/glfotwqwn.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fktsv.cn/Article/details/gcrkwbyhe.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gonqyjqze.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.epnwcf.com/Article/details/gmpvvhory.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.yfazqb.com/Article/details/glcwkpbpr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.tarul.cn/Article/details/gcrsukpwl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.sjlbkw.cn/Article/details/gmkdhglee.sHtML

[U43] PHP：声明命名空间
来源：http://3g.vehdjk.com/Article/details/gsbtmjgei.sHtML

namespace App\Http;
来源：http://3g.tarul.cn/Article/details/gtcjmpxyv.sHtML

[U44] PHP：开启严格类型
来源：http://3g.bbcook.cn/Article/details/giqqramzo.sHtML

declare(strict_types=1);
来源：http://baike.tarul.cn/Article/details/gplsugkro.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.tarul.cn/Article/details/gooucnlww.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gzzedgson.sHtML

[U46] PHP：可空类型
来源：http://www.share.epnwcf.com/Article/details/ghwbcdbte.sHtML

?string $name = null
来源：http://3g.tarul.cn/Article/details/gjqqiyhif.sHtML

[U47] PHP：联合类型
来源：http://wap.epnwcf.com/Article/details/gucveswgb.sHtML

int|string $id
来源：http://3g.fktsv.cn/Article/details/gpbytxirj.sHtML

[U48] PHP：纯枚举
来源：http://blog.bbcook.cn/Article/details/gegpeeswb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.sjlbkw.cn/Article/details/grthktfbm.sHtML

[U49] PHP：只读属性
来源：http://blog.bbcook.cn/Article/details/gcaequnak.sHtML

public readonly string $name
来源：http://www.m.share.vehdjk.com/Article/details/gkobahptd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.vehdjk.com/Article/details/gbsnsaqnq.sHtML

public function __construct(private int $id) {}
来源：http://3g.fktsv.cn/Article/details/gdcezbiuk.sHtML

[U51] PHP：数组解构
来源：http://www.blog.epnwcf.com/Article/details/gdsqgaldg.sHtML

[$a, $b] = $arr;
来源：http://wap.epnwcf.com/Article/details/grpimwvob.sHtML

[U52] PHP：箭头函数
来源：http://m.share.epnwcf.com/Article/details/gsgwzkrcs.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.sjlbkw.cn/Article/details/gbwrfaukf.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.yfazqb.com/Article/details/gcsvdpemk.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.tarul.cn/Article/details/gjvsxfbzi.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fktsv.cn/Article/details/gndlmgetp.sHtML

$obj?->method()
来源：http://baike.yfazqb.com/Article/details/gvtxrhvcs.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fktsv.cn/Article/details/gnasufyzb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fktsv.cn/Article/details/gfppjnqlz.sHtML

[U56] PHP：命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gratggkxr.sHtML

f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gipjugwcw.sHtML

[U57] PHP：字符串插值
来源：http://m.share.tarul.cn/Article/details/gmkcijgkd.sHtML

"值: {$a}"
来源：http://m.share.sjlbkw.cn/Article/details/gjamxdcxx.sHtML

[U58] PHP：数组三件套
来源：http://mobile.bbcook.cn/Article/details/gghvzbkyk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.tarul.cn/Article/details/gezozhwwu.sHtML

[U59] PHP：自定义排序
来源：http://baike.yfazqb.com/Article/details/gwtgzjgqk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/gmlmxllpp.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.bbcook.cn/Article/details/gwthatgss.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.vehdjk.com/Article/details/gqaxmgspf.sHtML

[U61] PHP：正则
来源：http://www.share.fktsv.cn/Article/details/gzzmhmrso.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.epnwcf.com/Article/details/gscgdkyxh.sHtML

[U62] PHP：日期对象
来源：http://www.blog.vehdjk.com/Article/details/gnazzrpij.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.bbcook.cn/Article/details/gkjdavofk.sHtML

[U63] PHP：文件读写
来源：http://baike.sjlbkw.cn/Article/details/gjmlsnsax.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.vehdjk.com/Article/details/gosnetvfd.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.yfazqb.com/Article/details/gvngtssss.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.yfazqb.com/Article/details/ghtorycsk.sHtML

[U65] PHP：会话
来源：http://blog.fktsv.cn/Article/details/gwyottnaj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/guvdgvfom.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.yfazqb.com/Article/details/giylqlehh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.sjlbkw.cn/Article/details/goauurqwq.sHtML

[U67] PHP：处理文件上传
来源：http://wap.sjlbkw.cn/Article/details/gvisdrcde.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.sjlbkw.cn/Article/details/gczvfjkgd.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.tarul.cn/Article/details/gaetahnne.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fktsv.cn/Article/details/gnqhtuqtc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.epnwcf.com/Article/details/gqxaewzzu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.tarul.cn/Article/details/gypkqhrct.sHtML

[U70] PHP：PDO 事务
来源：http://baike.vehdjk.com/Article/details/gxkodoeec.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.vehdjk.com/Article/details/gfmfzwnpt.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.vehdjk.com/Article/details/goqjgntyd.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.tarul.cn/Article/details/gryubmlhb.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.tarul.cn/Article/details/gostxdymy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fktsv.cn/Article/details/glonrbmvw.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.vehdjk.com/Article/details/gpkticbdr.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.yfazqb.com/Article/details/gncruexpz.sHtML

[U74] PHP：读取环境变量
来源：http://3g.sjlbkw.cn/Article/details/glvbqfegt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.bbcook.cn/Article/details/gubyqwbnn.sHtML

[U75] PHP：依赖注入
来源：http://www.share.yfazqb.com/Article/details/gznfvbpnc.sHtML

composer require psr/container
来源：http://www.share.epnwcf.com/Article/details/gntawucbz.sHtML

[U76] PHP：简单路由
来源：http://wap.vehdjk.com/Article/details/gfhnjlkog.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.yfazqb.com/Article/details/giipauokq.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fktsv.cn/Article/details/gjevtbuge.sHtML

composer require twig/twig
来源：http://baike.fktsv.cn/Article/details/gyhhlhuzo.sHtML

[U78] PHP：单元测试
来源：http://m.share.yfazqb.com/Article/details/gguzpfkrg.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fktsv.cn/Article/details/gsmokttke.sHtML

[U79] PHP：静态分析
来源：http://www.blog.yfazqb.com/Article/details/ggnkohsms.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.sjlbkw.cn/Article/details/gjtiiabge.sHtML

[U80] PHP：代码规范修复
来源：http://wap.bbcook.cn/Article/details/glvxrlueu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.epnwcf.com/Article/details/gfwsahqaw.sHtML

[U81] JS：初始化项目
来源：http://mobile.fktsv.cn/Article/details/geassidfg.sHtML

npm init -y;  npm i express
来源：http://3g.vehdjk.com/Article/details/gelskcwdz.sHtML

[U82] JS：package.json 脚本
来源：http://blog.vehdjk.com/Article/details/gabkfjbhf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.yfazqb.com/Article/details/gjasnptoz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.tarul.cn/Article/details/guyviknog.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.yfazqb.com/Article/details/gkqqrmzrm.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.sjlbkw.cn/Article/details/gmojrocik.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.bbcook.cn/Article/details/glcvrwodr.sHtML

[U85] JS：可选链
来源：http://www.share.fktsv.cn/Article/details/ggjxoaprb.sHtML

a?.b?.c
来源：http://3g.epnwcf.com/Article/details/gxzwieono.sHtML

[U86] JS：空值合并
来源：http://www.share.fktsv.cn/Article/details/gosaqsaoi.sHtML

a ?? b
来源：http://www.m.share.bbcook.cn/Article/details/gatninebk.sHtML

[U87] JS：解构默认值
来源：http://www.share.fktsv.cn/Article/details/gxtxcimci.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.yfazqb.com/Article/details/gsjacacwl.sHtML

[U88] JS：对象展开合并
来源：http://wap.fktsv.cn/Article/details/gaidvdjwb.sHtML

{ ...a, ...b }
来源：http://wap.fktsv.cn/Article/details/gsbsotvtb.sHtML

[U89] JS：数组去重
来源：http://baike.vehdjk.com/Article/details/gcdhgkzwt.sHtML

[...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/gpdozncrr.sHtML

[U90] JS：数字数组排序
来源：http://blog.epnwcf.com/Article/details/ghcbndeqx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gbpcpqmnk.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.bbcook.cn/Article/details/gjekoezed.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fktsv.cn/Article/details/gnkcafeof.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gmpyboipn.sHtML

structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/guyqrunav.sHtML

[U93] JS：模板字符串
来源：http://www.blog.vehdjk.com/Article/details/gqikxgnkf.sHtML

`共 ${n} 条`
来源：http://www.share.bbcook.cn/Article/details/gbgriyucc.sHtML

[U94] JS：箭头函数
来源：http://blog.epnwcf.com/Article/details/gbqiiscrt.sHtML

const double = x => x * 2;
来源：http://mobile.sjlbkw.cn/Article/details/glfkkjbqx.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.bbcook.cn/Article/details/getubjthq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.yfazqb.com/Article/details/gzsyfodel.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.yfazqb.com/Article/details/gwatqtkai.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gsbxmbket.sHtML

[U97] JS：并发请求
来源：http://www.share.tarul.cn/Article/details/gsvfnaaox.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/glrkvfqlx.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.sjlbkw.cn/Article/details/gstgqqopd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.sjlbkw.cn/Article/details/ggpflvexc.sHtML

[U99] JS：事件监听
来源：http://mobile.vehdjk.com/Article/details/guzrryjcj.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzvoyyhj.sHtML

[U100] JS：DOM 查询
来源：http://baike.vehdjk.com/Article/details/gtwyuhnhc.sHtML

document.querySelector(".item")
来源：http://3g.epnwcf.com/Article/details/gqgvcpfsh.sHtML

[U101] JS：classList 操作
来源：http://blog.tarul.cn/Article/details/gmhfaaycw.sHtML

el.classList.toggle("active")
来源：http://mobile.yfazqb.com/Article/details/gychzyiej.sHtML

[U102] JS：本地存储
来源：http://mobile.sjlbkw.cn/Article/details/gpvgpbbth.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.sjlbkw.cn/Article/details/gfdpuqerz.sHtML

[U103] JS：定时器
来源：http://3g.vehdjk.com/Article/details/gdfrrdqfv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fktsv.cn/Article/details/grcdibqpd.sHtML

[U104] JS：防抖
来源：http://www.blog.bbcook.cn/Article/details/gponcfnbj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gciookyqp.sHtML

[U105] JS：节流
来源：http://3g.sjlbkw.cn/Article/details/gewcwaavk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.epnwcf.com/Article/details/gydhamhkg.sHtML

[U106] JS：日期格式化
来源：http://wap.bbcook.cn/Article/details/gklkiddyz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.epnwcf.com/Article/details/gxezjqahi.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gvjjyclat.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/gopzaqcin.sHtML

[U108] JS：随机整数
来源：http://www.blog.tarul.cn/Article/details/gfmtqqgvq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.vehdjk.com/Article/details/gxlfwaezq.sHtML

[U109] JS：数组分组
来源：http://mobile.yfazqb.com/Article/details/gtwlqhfnl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/ghfmrfyiy.sHtML

[U110] JS：数组分块
来源：http://www.share.fktsv.cn/Article/details/grokslbeg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.sjlbkw.cn/Article/details/gjoggzlwg.sHtML

[U111] JS：对象转 Map
来源：http://read.share.bbcook.cn/Article/details/gdhgspqpz.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fktsv.cn/Article/details/gptuabnra.sHtML

[U112] JS：字符串补位
来源：http://www.share.epnwcf.com/Article/details/gcjypkzmz.sHtML

"7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gmciaappa.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fktsv.cn/Article/details/gpkxmyvmr.sHtML

s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gigjdakzv.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fktsv.cn/Article/details/glpxwqczf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fktsv.cn/Article/details/gjrkzsaak.sHtML

[U115] JS：生成 UUID
来源：http://mobile.yfazqb.com/Article/details/gmyzthrzp.sHtML

crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gwekfnogc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.vehdjk.com/Article/details/gdxbvawfe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.bbcook.cn/Article/details/gthnyeagb.sHtML

[U117] JS：单元测试
来源：http://mobile.epnwcf.com/Article/details/gaznmmdfz.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.sjlbkw.cn/Article/details/gwejuouct.sHtML

[U118] JS：开发服务器
来源：http://baike.fktsv.cn/Article/details/gqntupybm.sHtML

npm i -D vite;  npx vite
来源：http://wap.vehdjk.com/Article/details/getlacdzl.sHtML

[U119] JS：生产构建
来源：http://www.blog.vehdjk.com/Article/details/gevlrhvdq.sHtML

npx vite build
来源：http://wap.bbcook.cn/Article/details/glnbjstzz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.epnwcf.com/Article/details/gdbzeusky.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.bbcook.cn/Article/details/gypxbrfnc.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdlsznxvl.sHtML

统计汇总
来源：http://3g.epnwcf.com/Article/details/gamdoxvbm.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gvkawacrz.sHtML

按语言统计（条）：
来源：http://blog.vehdjk.com/Article/details/gkydtttkf.sHtML

Python ......... 252
来源：http://www.share.yfazqb.com/Article/details/gdvfgbkwt.sHtML

PHP ............ 252
来源：http://www.blog.yfazqb.com/Article/details/gydshevfq.sHtML

JavaScript ..... 252
来源：http://www.m.share.bbcook.cn/Article/details/gsoogckwd.sHtML

TypeScript ..... 212
来源：http://wap.yfazqb.com/Article/details/gamfdzwfg.sHtML

Java ........... 212
来源：http://mobile.epnwcf.com/Article/details/gfgfdplkq.sHtML

Go ............. 212
来源：http://wap.fktsv.cn/Article/details/gjizwtxco.sHtML

Ruby ........... 212
来源：http://m.share.epnwcf.com/Article/details/geyqldzud.sHtML

C# ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/gtaxpflnc.sHtML

C .............. 30
来源：http://blog.sjlbkw.cn/Article/details/guwqfyitx.sHtML

C++ ............ 30
来源：http://m.share.epnwcf.com/Article/details/gzqxavpzy.sHtML

SQL ............ 90
来源：http://www.blog.sjlbkw.cn/Article/details/gqadhlpla.sHtML

Bash ........... 80
来源：http://www.m.share.bbcook.cn/Article/details/gyiekjcpz.sHtML

Kotlin ......... 15
来源：http://www.blog.tarul.cn/Article/details/gqgujwwtu.sHtML

Swift .......... 15
来源：http://3g.epnwcf.com/Article/details/gytipdbhg.sHtML

Lua ............ 10
来源：http://blog.tarul.cn/Article/details/givjfnbwz.sHtML

Perl ........... 10
来源：http://www.blog.vehdjk.com/Article/details/gfbjveutu.sHtML

Scala .......... 10
来源：http://wap.tarul.cn/Article/details/gadbxpdtv.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gbpbmdrzy.sHtML

合计 ........... 2106 条
来源：http://blog.sjlbkw.cn/Article/details/guyhanwvc.sHtML

按章节统计：
来源：http://read.share.tarul.cn/Article/details/gksfrdtfp.sHtML


<!-- 参考信息 -->