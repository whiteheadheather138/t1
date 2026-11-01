代发 wailian999

[T45] Perl：数组遍历
来源：http://wap.bbcook.cn/Article/details/gbofmrncr.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.tarul.cn/Article/details/ggawqutrd.sHtML

[T46] Perl：哈希操作
来源：http://3g.fktsv.cn/Article/details/guyycdrih.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.tarul.cn/Article/details/gkkedgyce.sHtML

[T47] Perl：正则捕获
来源：http://www.share.epnwcf.com/Article/details/gmsolgfft.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fktsv.cn/Article/details/gltnlvvvw.sHtML

[T48] Perl：正则替换
来源：http://read.share.bbcook.cn/Article/details/ginmffgqt.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/gxhvlimyc.sHtML

[T49] Perl：函数
来源：http://mobile.fktsv.cn/Article/details/gnmpqvqrl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gwclvubfy.sHtML

[T50] Perl：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gllinybjs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.bbcook.cn/Article/details/gwmmhgcoi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.tarul.cn/Article/details/gmmdzvxqy.sHtML

[T51] Scala：Hello World
来源：http://m.share.vehdjk.com/Article/details/gaxynkwwa.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/gbihqvpzs.sHtML

[T52] Scala：变量
来源：http://baike.sjlbkw.cn/Article/details/gtliqrvoc.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gydbkvssf.sHtML

[T53] Scala：字符串插值
来源：http://www.share.tarul.cn/Article/details/gcqnivwqq.sHtML

s"值: $b"
来源：http://blog.yfazqb.com/Article/details/gbkzumdse.sHtML

[T54] Scala：集合映射
来源：http://www.blog.tarul.cn/Article/details/gtekzcgmj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.yfazqb.com/Article/details/glfezdfbz.sHtML

[T55] Scala：集合过滤
来源：http://wap.bbcook.cn/Article/details/gmismzoxg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.yfazqb.com/Article/details/gbrdpxyfh.sHtML

[T56] Scala：样例类
来源：http://m.share.bbcook.cn/Article/details/grhtbwoih.sHtML

case class User(name: String, age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/ghwzpgran.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gvypyxnfl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.bbcook.cn/Article/details/gqqbpegco.sHtML

[T58] Scala：函数定义
来源：http://read.share.sjlbkw.cn/Article/details/ggcdxsqed.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gazevwgqc.sHtML

[T59] Scala：循环
来源：http://www.share.sjlbkw.cn/Article/details/gjsjrveoc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gvpobgwak.sHtML

[T60] Scala：折叠
来源：http://read.share.vehdjk.com/Article/details/gtchgvnbb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.bbcook.cn/Article/details/gqyglxgpe.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gfnmlxwtx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.bbcook.cn/Article/details/gdvloqesk.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpvjrcbud.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.tarul.cn/Article/details/gmgfzmrcz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.sjlbkw.cn/Article/details/gnhhlwfgv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.epnwcf.com/Article/details/gltjotdqj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.vehdjk.com/Article/details/gsghvodsz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.vehdjk.com/Article/details/gtzhcyasj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.yfazqb.com/Article/details/ginznwsqg.sHtML

[U04] Py：变量调试打印
来源：http://blog.sjlbkw.cn/Article/details/gmagninva.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.vehdjk.com/Article/details/gfbiycscy.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.yfazqb.com/Article/details/ghpmnjrdu.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/gjzgtfoas.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fktsv.cn/Article/details/gfcpekzbj.sHtML

{**a, **b}
来源：http://read.share.epnwcf.com/Article/details/gndqqymtq.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.vehdjk.com/Article/details/gpltmtbib.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fktsv.cn/Article/details/gjygodyit.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.tarul.cn/Article/details/gvnwdahlm.sHtML

[y for x in nested for y in x]
来源：http://read.share.yfazqb.com/Article/details/gehutyqpj.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.tarul.cn/Article/details/gzjgsstrz.sHtML

max(d, key=d.get)
来源：http://baike.epnwcf.com/Article/details/gzxkgtlvv.sHtML

[U10] Py：按值排序字典
来源：http://wap.epnwcf.com/Article/details/gruhtiogs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.epnwcf.com/Article/details/gnuqyatxj.sHtML

[U11] Py：生成器表达式
来源：http://m.share.vehdjk.com/Article/details/gqmrhmvun.sHtML

(x * 2 for x in arr)
来源：http://blog.fktsv.cn/Article/details/gejbzsmxv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.tarul.cn/Article/details/gyhljbztm.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.yfazqb.com/Article/details/gpibvbcmf.sHtML

[U13] Py：固定长度队列
来源：http://mobile.epnwcf.com/Article/details/gyolcrcds.sHtML

deque(maxlen=10)
来源：http://baike.bbcook.cn/Article/details/guykuhrow.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.bbcook.cn/Article/details/godypqksz.sHtML

defaultdict(list)
来源：http://wap.vehdjk.com/Article/details/gmaexzgcp.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fktsv.cn/Article/details/gwsgwmnel.sHtML

t = time.perf_counter()
来源：http://www.share.bbcook.cn/Article/details/gvspkumeq.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.yfazqb.com/Article/details/gkovijsdb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.yfazqb.com/Article/details/gnkcsawjf.sHtML

[U17] Py：初始化日志
来源：http://wap.tarul.cn/Article/details/grofpnlfx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.bbcook.cn/Article/details/gxublenpw.sHtML

[U18] Py：预编译正则
来源：http://blog.bbcook.cn/Article/details/gxwrwohrg.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.tarul.cn/Article/details/gxwbqjodz.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.epnwcf.com/Article/details/gygaafqhy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.tarul.cn/Article/details/gozpgdwnk.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.epnwcf.com/Article/details/gebdnjcbm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.bbcook.cn/Article/details/gcswpgyck.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.sjlbkw.cn/Article/details/gikzgyqqf.sHtML

@contextlib.contextmanager
来源：http://blog.vehdjk.com/Article/details/gtuqmkdrf.sHtML

[U22] Py：矩阵转置
来源：http://read.share.bbcook.cn/Article/details/gklvalfay.sHtML

list(zip(*m))
来源：http://blog.tarul.cn/Article/details/gikygnhsu.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fktsv.cn/Article/details/gxjtprdrj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.tarul.cn/Article/details/gxqjanosv.sHtML

[U24] Py：路径操作
来源：http://wap.yfazqb.com/Article/details/gubmlenky.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gkfgctisl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fktsv.cn/Article/details/gofrojars.sHtML

csv.DictReader(f)
来源：http://wap.bbcook.cn/Article/details/guwrzlzsm.sHtML

[U26] Py：并发下载
来源：http://blog.bbcook.cn/Article/details/gvqfhlzxw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.bbcook.cn/Article/details/gbqpwetsr.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.yfazqb.com/Article/details/ggbstepev.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.yfazqb.com/Article/details/gidthvpvr.sHtML

[U28] Py：类型别名
来源：http://baike.tarul.cn/Article/details/goasviaww.sHtML

UserId = int
来源：http://wap.sjlbkw.cn/Article/details/gzctisilv.sHtML

[U29] Py：属性校验
来源：http://m.share.bbcook.cn/Article/details/gujvvjmdj.sHtML

@property 与 @x.setter 配合
来源：http://baike.epnwcf.com/Article/details/gzmzjmamp.sHtML

[U30] Py：数据类
来源：http://blog.vehdjk.com/Article/details/gmxqxiwcy.sHtML

@dataclass(slots=True)
来源：http://m.share.yfazqb.com/Article/details/grresgrih.sHtML

[U31] Py：单测
来源：http://wap.fktsv.cn/Article/details/gycijzmst.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/gzgcfstmf.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fktsv.cn/Article/details/glfzgxfqk.sHtML

ruff format . && ruff check --fix .
来源：http://wap.vehdjk.com/Article/details/gxnikekxz.sHtML

[U33] Py：打包发布
来源：http://www.blog.vehdjk.com/Article/details/geyixjqlo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.tarul.cn/Article/details/ggoigfqwq.sHtML

[U34] Py：判断编码
来源：http://blog.epnwcf.com/Article/details/gqqsklano.sHtML

chardet.detect(raw)
来源：http://www.m.share.tarul.cn/Article/details/gssduthhj.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.bbcook.cn/Article/details/gqszaezcm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.epnwcf.com/Article/details/ginmkxenu.sHtML

[U36] Py：定时任务
来源：http://wap.tarul.cn/Article/details/gqrlbkwes.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.sjlbkw.cn/Article/details/gfzbeeuud.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fktsv.cn/Article/details/gvzazzirc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.tarul.cn/Article/details/gslsovyak.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.tarul.cn/Article/details/gngyfzvck.sHtML

Path(__file__).resolve().parent
来源：http://wap.fktsv.cn/Article/details/ggrqkypki.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.sjlbkw.cn/Article/details/gmzqtrwhm.sHtML

sys.stdout.isatty()
来源：http://mobile.vehdjk.com/Article/details/gwyvzwdxs.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.epnwcf.com/Article/details/gwcpkjlnz.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gcxhuyshd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.epnwcf.com/Article/details/gvataajri.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fktsv.cn/Article/details/grzhmvhsj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.tarul.cn/Article/details/gktemlgwp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.yfazqb.com/Article/details/ghyotpioq.sHtML

[U43] PHP：声明命名空间
来源：http://baike.sjlbkw.cn/Article/details/gkfbkpecd.sHtML

namespace App\Http;
来源：http://www.share.fktsv.cn/Article/details/grxzgitle.sHtML

[U44] PHP：开启严格类型
来源：http://baike.vehdjk.com/Article/details/gfcvnsbjf.sHtML

declare(strict_types=1);
来源：http://www.blog.fktsv.cn/Article/details/gxkadjvtn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.epnwcf.com/Article/details/gtwpxzcow.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/godfhaxke.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.epnwcf.com/Article/details/gcryzyamj.sHtML

?string $name = null
来源：http://wap.sjlbkw.cn/Article/details/gbxngpndu.sHtML

[U47] PHP：联合类型
来源：http://3g.vehdjk.com/Article/details/gpwqwziij.sHtML

int|string $id
来源：http://read.share.sjlbkw.cn/Article/details/gfurrmlxm.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/geutprphi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.epnwcf.com/Article/details/gzgoqwghq.sHtML

[U49] PHP：只读属性
来源：http://wap.sjlbkw.cn/Article/details/gbpnpeixy.sHtML

public readonly string $name
来源：http://blog.epnwcf.com/Article/details/gihjwsnex.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.epnwcf.com/Article/details/gzdpclddd.sHtML

public function __construct(private int $id) {}
来源：http://www.share.vehdjk.com/Article/details/gjagxljbq.sHtML

[U51] PHP：数组解构
来源：http://3g.tarul.cn/Article/details/gddezjrqa.sHtML

[$a, $b] = $arr;
来源：http://baike.epnwcf.com/Article/details/gffzfqrts.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/gmzcdnsff.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.bbcook.cn/Article/details/gvdkzgiwl.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.tarul.cn/Article/details/gecgmpuwc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.bbcook.cn/Article/details/gcaeftshg.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.epnwcf.com/Article/details/grqcapekd.sHtML

$obj?->method()
来源：http://read.share.fktsv.cn/Article/details/gevtkvrgo.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/ghmesjpjm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.bbcook.cn/Article/details/grkvqusif.sHtML

[U56] PHP：命名参数
来源：http://read.share.vehdjk.com/Article/details/gcqxyrovj.sHtML

f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gxeywrwdb.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gvzuxerfx.sHtML

"值: {$a}"
来源：http://3g.bbcook.cn/Article/details/gyroedhqt.sHtML

[U58] PHP：数组三件套
来源：http://www.share.bbcook.cn/Article/details/guiucydnk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.epnwcf.com/Article/details/gbmuqbeeh.sHtML

[U59] PHP：自定义排序
来源：http://mobile.tarul.cn/Article/details/gskboerte.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/gedyjlaqe.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.epnwcf.com/Article/details/gsivkpewr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.bbcook.cn/Article/details/gorfjzivd.sHtML

[U61] PHP：正则
来源：http://www.m.share.tarul.cn/Article/details/ggpjtktxk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/gjvyamwih.sHtML

[U62] PHP：日期对象
来源：http://blog.vehdjk.com/Article/details/gyetovgwl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fktsv.cn/Article/details/gcydvaxrg.sHtML

[U63] PHP：文件读写
来源：http://3g.epnwcf.com/Article/details/gbixmgynq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.sjlbkw.cn/Article/details/gmwokgimb.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.yfazqb.com/Article/details/gezlzwhna.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.sjlbkw.cn/Article/details/gdnmljlzw.sHtML

[U65] PHP：会话
来源：http://read.share.fktsv.cn/Article/details/ghbfdyvhq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.yfazqb.com/Article/details/getwfdxfh.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fktsv.cn/Article/details/guzusrfqr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.tarul.cn/Article/details/grtdcjfct.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.bbcook.cn/Article/details/gxurltxxq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.tarul.cn/Article/details/gzycysuzp.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.sjlbkw.cn/Article/details/gwcuesvxa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxhdtxkw.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.sjlbkw.cn/Article/details/gpafnvroa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.vehdjk.com/Article/details/gnvzbfsyl.sHtML

[U70] PHP：PDO 事务
来源：http://wap.tarul.cn/Article/details/gtttuedii.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.yfazqb.com/Article/details/gyfjofkgl.sHtML

[U71] PHP：抛出异常
来源：http://blog.epnwcf.com/Article/details/gmhekjzyw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.bbcook.cn/Article/details/goortopkr.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.epnwcf.com/Article/details/gmmilrogs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.epnwcf.com/Article/details/gwrgshaij.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fktsv.cn/Article/details/gjplzqcqw.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.yfazqb.com/Article/details/gwjvomgfb.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gywqgklie.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fktsv.cn/Article/details/gcknlbeqm.sHtML

[U75] PHP：依赖注入
来源：http://wap.vehdjk.com/Article/details/guybknqlc.sHtML

composer require psr/container
来源：http://www.m.share.epnwcf.com/Article/details/gpcjvtxcy.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fktsv.cn/Article/details/gdedjidhn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fktsv.cn/Article/details/gknilsyme.sHtML

[U77] PHP：模板渲染
来源：http://m.share.sjlbkw.cn/Article/details/gxyyxqzpr.sHtML

composer require twig/twig
来源：http://www.m.share.yfazqb.com/Article/details/genzptyjk.sHtML

[U78] PHP：单元测试
来源：http://3g.vehdjk.com/Article/details/ggbcfrnwg.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.vehdjk.com/Article/details/glubolvfv.sHtML

[U79] PHP：静态分析
来源：http://wap.epnwcf.com/Article/details/gnrtkxzpg.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fktsv.cn/Article/details/gcsertrnc.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.epnwcf.com/Article/details/gynrrwabv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.bbcook.cn/Article/details/gprrzvbks.sHtML

[U81] JS：初始化项目
来源：http://blog.epnwcf.com/Article/details/gkyivrovb.sHtML

npm init -y;  npm i express
来源：http://wap.bbcook.cn/Article/details/gzqlolbyb.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.tarul.cn/Article/details/gjyhkbevi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.epnwcf.com/Article/details/gdxniluzl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.yfazqb.com/Article/details/gilfsvtri.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fktsv.cn/Article/details/gkfbatjur.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.yfazqb.com/Article/details/gauuotyfj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fktsv.cn/Article/details/gcbhxxkpl.sHtML

[U85] JS：可选链
来源：http://www.blog.vehdjk.com/Article/details/gqmrjhczr.sHtML

a?.b?.c
来源：http://3g.yfazqb.com/Article/details/goxafvzzx.sHtML

[U86] JS：空值合并
来源：http://www.share.fktsv.cn/Article/details/gbwgwfydf.sHtML

a ?? b
来源：http://3g.vehdjk.com/Article/details/grrudajiw.sHtML

[U87] JS：解构默认值
来源：http://baike.vehdjk.com/Article/details/gtzyrxxon.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.bbcook.cn/Article/details/gwwxtcrsj.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.sjlbkw.cn/Article/details/gwgghkmbe.sHtML

{ ...a, ...b }
来源：http://mobile.fktsv.cn/Article/details/grewkvbrh.sHtML

[U89] JS：数组去重
来源：http://www.m.share.tarul.cn/Article/details/guekvxbvd.sHtML

[...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gkblvhtup.sHtML

[U90] JS：数字数组排序
来源：http://read.share.sjlbkw.cn/Article/details/ggiblpqbs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gjgmeakns.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.epnwcf.com/Article/details/gwmemojrl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/geoaenpmk.sHtML

[U92] JS：深拷贝
来源：http://wap.epnwcf.com/Article/details/gjqmcbxzu.sHtML

structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gaxczxlwy.sHtML

[U93] JS：模板字符串
来源：http://m.share.yfazqb.com/Article/details/gkxjcuudu.sHtML

`共 ${n} 条`
来源：http://baike.yfazqb.com/Article/details/ghyaoqksq.sHtML

[U94] JS：箭头函数
来源：http://mobile.vehdjk.com/Article/details/gzogcwopi.sHtML

const double = x => x * 2;
来源：http://baike.yfazqb.com/Article/details/gkdhietmt.sHtML

[U95] JS：Promise 包装
来源：http://mobile.epnwcf.com/Article/details/gbexereig.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.epnwcf.com/Article/details/gtgdxdzcl.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.bbcook.cn/Article/details/gramqkiwk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gxzgfprsn.sHtML

[U97] JS：并发请求
来源：http://www.m.share.vehdjk.com/Article/details/gznfyiycz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/ggshfzydp.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fktsv.cn/Article/details/galqsfesg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fktsv.cn/Article/details/gugnicndj.sHtML

[U99] JS：事件监听
来源：http://mobile.sjlbkw.cn/Article/details/gtbzpbkfk.sHtML

el.addEventListener("click", e => {})
来源：http://3g.yfazqb.com/Article/details/gqbqqrlch.sHtML

[U100] JS：DOM 查询
来源：http://wap.fktsv.cn/Article/details/gnkmjhadi.sHtML

document.querySelector(".item")
来源：http://m.share.sjlbkw.cn/Article/details/gpsnjbdlu.sHtML

[U101] JS：classList 操作
来源：http://baike.yfazqb.com/Article/details/goeyyuuci.sHtML

el.classList.toggle("active")
来源：http://baike.bbcook.cn/Article/details/grrinrhvr.sHtML

[U102] JS：本地存储
来源：http://www.m.share.epnwcf.com/Article/details/gnjpxqfyv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.epnwcf.com/Article/details/gxbohlrqk.sHtML

[U103] JS：定时器
来源：http://www.m.share.vehdjk.com/Article/details/gbwbnrbro.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.tarul.cn/Article/details/gqafxebou.sHtML

[U104] JS：防抖
来源：http://read.share.sjlbkw.cn/Article/details/ggmazxhqg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gzzengpez.sHtML

[U105] JS：节流
来源：http://read.share.fktsv.cn/Article/details/gdwrmsthc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.yfazqb.com/Article/details/gjfvmzywn.sHtML

[U106] JS：日期格式化
来源：http://m.share.epnwcf.com/Article/details/guzeincmg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.bbcook.cn/Article/details/gedwodiht.sHtML

[U107] JS：数字千分位
来源：http://mobile.vehdjk.com/Article/details/gshssougz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gcmhlbjqz.sHtML

[U108] JS：随机整数
来源：http://www.share.bbcook.cn/Article/details/ggjcsexwc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fktsv.cn/Article/details/gusveoomb.sHtML

[U109] JS：数组分组
来源：http://mobile.bbcook.cn/Article/details/gblmfwgbk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gcbqonscd.sHtML

[U110] JS：数组分块
来源：http://3g.tarul.cn/Article/details/gzpwaebbf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.epnwcf.com/Article/details/gczmstfhd.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fktsv.cn/Article/details/gkektouwl.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fktsv.cn/Article/details/ghwhozrcr.sHtML

[U112] JS：字符串补位
来源：http://wap.yfazqb.com/Article/details/ghkuvihij.sHtML

"7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/glxcvujfa.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fktsv.cn/Article/details/gdvwkvgqc.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gvmbdsbjf.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.bbcook.cn/Article/details/gmpjglxyd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gzpdmcrry.sHtML

[U115] JS：生成 UUID
来源：http://www.share.bbcook.cn/Article/details/gsgwtkcdo.sHtML

crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/glleumnno.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.yfazqb.com/Article/details/gcaneigrc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.sjlbkw.cn/Article/details/gkdjigpph.sHtML

[U117] JS：单元测试
来源：http://www.m.share.bbcook.cn/Article/details/gdwezljqu.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.sjlbkw.cn/Article/details/gdqfmwgny.sHtML

[U118] JS：开发服务器
来源：http://www.blog.bbcook.cn/Article/details/gjbxocpja.sHtML

npm i -D vite;  npx vite
来源：http://www.share.bbcook.cn/Article/details/gdtsttcst.sHtML

[U119] JS：生产构建
来源：http://mobile.vehdjk.com/Article/details/ghqehgiig.sHtML

npx vite build
来源：http://3g.sjlbkw.cn/Article/details/gmdppzypc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fktsv.cn/Article/details/gtodeerba.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.yfazqb.com/Article/details/gebveveql.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gajchzyiu.sHtML

统计汇总
来源：http://mobile.yfazqb.com/Article/details/gvdeukfjm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmelyxhvu.sHtML

按语言统计（条）：
来源：http://www.blog.vehdjk.com/Article/details/gbmmebbhy.sHtML

Python ......... 252
来源：http://m.share.sjlbkw.cn/Article/details/gpkhqieyy.sHtML

PHP ............ 252
来源：http://3g.sjlbkw.cn/Article/details/gojgykacb.sHtML

JavaScript ..... 252
来源：http://baike.yfazqb.com/Article/details/gkpackpoc.sHtML

TypeScript ..... 212
来源：http://mobile.yfazqb.com/Article/details/gzvmcsqer.sHtML

Java ........... 212
来源：http://baike.fktsv.cn/Article/details/gohvwiwsh.sHtML

Go ............. 212
来源：http://3g.fktsv.cn/Article/details/goaqcgqmq.sHtML

Ruby ........... 212
来源：http://www.blog.fktsv.cn/Article/details/glxupcdqn.sHtML

C# ............. 212
来源：http://www.share.bbcook.cn/Article/details/gohrfrmcf.sHtML

C .............. 30
来源：http://3g.vehdjk.com/Article/details/gmwuhkbqf.sHtML

C++ ............ 30
来源：http://www.share.bbcook.cn/Article/details/gpqjszqcn.sHtML

SQL ............ 90
来源：http://baike.sjlbkw.cn/Article/details/ginexqkut.sHtML

Bash ........... 80
来源：http://blog.tarul.cn/Article/details/gebmvvlov.sHtML

Kotlin ......... 15
来源：http://read.share.yfazqb.com/Article/details/gjsbpyvls.sHtML

Swift .......... 15
来源：http://blog.bbcook.cn/Article/details/gzbsafezb.sHtML

Lua ............ 10
来源：http://blog.bbcook.cn/Article/details/gkwmlasxq.sHtML

Perl ........... 10
来源：http://read.share.fktsv.cn/Article/details/gitlfwgif.sHtML

Scala .......... 10
来源：http://blog.bbcook.cn/Article/details/gmspvtfgy.sHtML

------------------------------------
来源：http://mobile.bbcook.cn/Article/details/ghkbxhaku.sHtML

合计 ........... 2106 条
来源：http://mobile.sjlbkw.cn/Article/details/gtejiaiws.sHtML

按章节统计：
来源：http://wap.tarul.cn/Article/details/gwrfghzfh.sHtML


<!-- 参考信息 -->