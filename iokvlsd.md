代发 wailian999

[T47] Perl：正则捕获
来源：http://m.share.sjlbkw.cn/Article/details/gtkqgnzpz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fktsv.cn/Article/details/ghftwmaga.sHtML

[T48] Perl：正则替换
来源：http://3g.fktsv.cn/Article/details/gqxsnlpsx.sHtML

$s =~ s/old/new/g;
来源：http://read.share.sjlbkw.cn/Article/details/gxxlhugdj.sHtML

[T49] Perl：函数
来源：http://baike.vehdjk.com/Article/details/gxacthjib.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gcdfckbee.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gkniibpjk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/gxptnckpo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.tarul.cn/Article/details/gukboblgu.sHtML

[T51] Scala：Hello World
来源：http://mobile.fktsv.cn/Article/details/gwhzpouku.sHtML

println("Hello")
来源：http://m.share.bbcook.cn/Article/details/gbmtekiug.sHtML

[T52] Scala：变量
来源：http://3g.fktsv.cn/Article/details/gvqksqbrb.sHtML

val a = 1;  var b = 2
来源：http://wap.vehdjk.com/Article/details/gyjwysgmh.sHtML

[T53] Scala：字符串插值
来源：http://www.share.tarul.cn/Article/details/gjlngfixq.sHtML

s"值: $b"
来源：http://wap.sjlbkw.cn/Article/details/gevdntuxi.sHtML

[T54] Scala：集合映射
来源：http://www.share.fktsv.cn/Article/details/gubxwqtvw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.epnwcf.com/Article/details/gfjbwrcwu.sHtML

[T55] Scala：集合过滤
来源：http://3g.bbcook.cn/Article/details/gvohsksjb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.bbcook.cn/Article/details/gpdccpgpr.sHtML

[T56] Scala：样例类
来源：http://mobile.tarul.cn/Article/details/gawxaqogx.sHtML

case class User(name: String, age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gwxxggqyh.sHtML

[T57] Scala：模式匹配
来源：http://mobile.tarul.cn/Article/details/gqpjfvvmm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.tarul.cn/Article/details/gitybeinm.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.vehdjk.com/Article/details/gthwehvhp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/gphlgptmt.sHtML

[T59] Scala：循环
来源：http://m.share.vehdjk.com/Article/details/gbqwsalhf.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fktsv.cn/Article/details/gcgopoehu.sHtML

[T60] Scala：折叠
来源：http://www.share.epnwcf.com/Article/details/gvbsusmxq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.vehdjk.com/Article/details/gomyrmkoz.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gtkyjnmjf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.bbcook.cn/Article/details/gesrsaodg.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gukthdvds.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fktsv.cn/Article/details/gwjnzhbwf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.yfazqb.com/Article/details/gwxltsxpt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.bbcook.cn/Article/details/gfxaunpze.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.tarul.cn/Article/details/gyzxxstnc.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.vehdjk.com/Article/details/gghmotbgu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.epnwcf.com/Article/details/gybodoeoq.sHtML

[U04] Py：变量调试打印
来源：http://www.share.bbcook.cn/Article/details/gvobtbpdu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.yfazqb.com/Article/details/gzdbgvaqv.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.epnwcf.com/Article/details/grmlytefg.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/glnuwklxj.sHtML

[U06] Py：合并两个字典
来源：http://www.share.tarul.cn/Article/details/gnjsmlrxu.sHtML

{**a, **b}
来源：http://3g.tarul.cn/Article/details/gmbqajber.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/gbupkznfm.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.sjlbkw.cn/Article/details/gdfqghbsk.sHtML

[U08] Py：展平二维列表
来源：http://wap.vehdjk.com/Article/details/ghcxbogxk.sHtML

[y for x in nested for y in x]
来源：http://mobile.epnwcf.com/Article/details/gkbnnqmcz.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.sjlbkw.cn/Article/details/ggjiomttf.sHtML

max(d, key=d.get)
来源：http://www.blog.vehdjk.com/Article/details/gljeyzviv.sHtML

[U10] Py：按值排序字典
来源：http://baike.sjlbkw.cn/Article/details/gkzdtftmk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.vehdjk.com/Article/details/gtrzpripe.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.tarul.cn/Article/details/gopwsvedv.sHtML

(x * 2 for x in arr)
来源：http://3g.epnwcf.com/Article/details/gpvytfydb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.sjlbkw.cn/Article/details/gxkhjvlcq.sHtML

Counter(arr).most_common(3)
来源：http://wap.vehdjk.com/Article/details/gzouuujer.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fktsv.cn/Article/details/gbpxpgjzc.sHtML

deque(maxlen=10)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrybumcs.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.tarul.cn/Article/details/gpwtqugop.sHtML

defaultdict(list)
来源：http://baike.epnwcf.com/Article/details/gfrieatgt.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.yfazqb.com/Article/details/geqkcxbzy.sHtML

t = time.perf_counter()
来源：http://blog.yfazqb.com/Article/details/gvgrpaqhh.sHtML

[U16] Py：命令行参数解析
来源：http://blog.bbcook.cn/Article/details/gcloximpw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.sjlbkw.cn/Article/details/gtsknljqz.sHtML

[U17] Py：初始化日志
来源：http://m.share.bbcook.cn/Article/details/giffllelp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.yfazqb.com/Article/details/gemsavdeh.sHtML

[U18] Py：预编译正则
来源：http://wap.bbcook.cn/Article/details/giihsindz.sHtML

pat = re.compile(r"\d+")
来源：http://blog.vehdjk.com/Article/details/gecpdxhzt.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fktsv.cn/Article/details/gidyyydsk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fktsv.cn/Article/details/gtfpgilaf.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.epnwcf.com/Article/details/gpdtddnna.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.bbcook.cn/Article/details/gcmglutle.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.bbcook.cn/Article/details/gvgbtfkgp.sHtML

@contextlib.contextmanager
来源：http://read.share.sjlbkw.cn/Article/details/gnqilutpo.sHtML

[U22] Py：矩阵转置
来源：http://www.share.vehdjk.com/Article/details/gbmbmbncl.sHtML

list(zip(*m))
来源：http://read.share.fktsv.cn/Article/details/gzalsvonh.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.tarul.cn/Article/details/givhmqnpn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fktsv.cn/Article/details/gifirsscf.sHtML

[U24] Py：路径操作
来源：http://wap.sjlbkw.cn/Article/details/gdeepzzxr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.bbcook.cn/Article/details/gwlxkzsmj.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.sjlbkw.cn/Article/details/gqvdsdqke.sHtML

csv.DictReader(f)
来源：http://mobile.tarul.cn/Article/details/gmbwrtslk.sHtML

[U26] Py：并发下载
来源：http://3g.fktsv.cn/Article/details/gqxzgxxqo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.tarul.cn/Article/details/gfkpyrfxs.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.vehdjk.com/Article/details/gpucgsonw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/gdftmmoyp.sHtML

[U28] Py：类型别名
来源：http://www.share.tarul.cn/Article/details/ggjgahqvj.sHtML

UserId = int
来源：http://wap.tarul.cn/Article/details/gpookohvi.sHtML

[U29] Py：属性校验
来源：http://www.blog.epnwcf.com/Article/details/gnumzoppj.sHtML

@property 与 @x.setter 配合
来源：http://3g.yfazqb.com/Article/details/gxhmzagdr.sHtML

[U30] Py：数据类
来源：http://baike.tarul.cn/Article/details/gjzwzqanx.sHtML

@dataclass(slots=True)
来源：http://3g.bbcook.cn/Article/details/guhbojrtn.sHtML

[U31] Py：单测
来源：http://m.share.epnwcf.com/Article/details/gkmutoung.sHtML

python -m pytest -q
来源：http://m.share.vehdjk.com/Article/details/gqxpfqmew.sHtML

[U32] Py：代码格式化
来源：http://www.blog.vehdjk.com/Article/details/goupzkhhr.sHtML

ruff format . && ruff check --fix .
来源：http://wap.bbcook.cn/Article/details/gvemdtgbk.sHtML

[U33] Py：打包发布
来源：http://www.blog.sjlbkw.cn/Article/details/gaisgvmdp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.epnwcf.com/Article/details/guzasikja.sHtML

[U34] Py：判断编码
来源：http://3g.bbcook.cn/Article/details/gbiovzbtp.sHtML

chardet.detect(raw)
来源：http://blog.epnwcf.com/Article/details/gugfswins.sHtML

[U35] Py：发送邮件
来源：http://m.share.vehdjk.com/Article/details/grwvksjlc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.vehdjk.com/Article/details/gvlvqgpdp.sHtML

[U36] Py：定时任务
来源：http://baike.tarul.cn/Article/details/gdjcudsnh.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.bbcook.cn/Article/details/gjeejytif.sHtML

[U37] Py：读写 Excel
来源：http://blog.bbcook.cn/Article/details/gmemddutv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.tarul.cn/Article/details/gvqshgkpi.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.sjlbkw.cn/Article/details/gkdrkvvbe.sHtML

Path(__file__).resolve().parent
来源：http://wap.vehdjk.com/Article/details/gfcwwgevk.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.epnwcf.com/Article/details/geordowzm.sHtML

sys.stdout.isatty()
来源：http://blog.sjlbkw.cn/Article/details/gurizlzhn.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.tarul.cn/Article/details/gdiimsvfp.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fktsv.cn/Article/details/ggyvuisoq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.sjlbkw.cn/Article/details/gsyzkvylf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.bbcook.cn/Article/details/givgsdsol.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.sjlbkw.cn/Article/details/gatqjulyu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fktsv.cn/Article/details/gypxflquj.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fktsv.cn/Article/details/ggnasbjoj.sHtML

namespace App\Http;
来源：http://mobile.vehdjk.com/Article/details/grlvuvreq.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fktsv.cn/Article/details/ggvyyaeup.sHtML

declare(strict_types=1);
来源：http://mobile.fktsv.cn/Article/details/gksvrimxf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fktsv.cn/Article/details/gqahywpme.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gnsqtfyzr.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fktsv.cn/Article/details/goiajzwpt.sHtML

?string $name = null
来源：http://www.share.sjlbkw.cn/Article/details/ghsdesewz.sHtML

[U47] PHP：联合类型
来源：http://read.share.epnwcf.com/Article/details/gcchhofyt.sHtML

int|string $id
来源：http://3g.yfazqb.com/Article/details/gkyxthujr.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gydugqxmm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fktsv.cn/Article/details/gwphktume.sHtML

[U49] PHP：只读属性
来源：http://read.share.epnwcf.com/Article/details/gdxbtuoes.sHtML

public readonly string $name
来源：http://wap.tarul.cn/Article/details/ghlcsqzlg.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fktsv.cn/Article/details/gzuwnoiow.sHtML

public function __construct(private int $id) {}
来源：http://3g.epnwcf.com/Article/details/gfdgzshcw.sHtML

[U51] PHP：数组解构
来源：http://read.share.yfazqb.com/Article/details/gotvzlwll.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.yfazqb.com/Article/details/gznnjffbh.sHtML

[U52] PHP：箭头函数
来源：http://blog.epnwcf.com/Article/details/gsuxzheig.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.epnwcf.com/Article/details/gardvrabk.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.yfazqb.com/Article/details/ggrikosxv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.sjlbkw.cn/Article/details/gcgnsfoiv.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fktsv.cn/Article/details/gchesdboe.sHtML

$obj?->method()
来源：http://blog.tarul.cn/Article/details/ghuvskdlt.sHtML

[U55] PHP：match 表达式
来源：http://wap.epnwcf.com/Article/details/gexfkqmny.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.vehdjk.com/Article/details/gzvfkbfso.sHtML

[U56] PHP：命名参数
来源：http://wap.epnwcf.com/Article/details/gbugosclf.sHtML

f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gkrxbfrtf.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gsebisyhq.sHtML

"值: {$a}"
来源：http://mobile.fktsv.cn/Article/details/gnnlvimeh.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fktsv.cn/Article/details/gkxfrxgbg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gxgrgcoci.sHtML

[U59] PHP：自定义排序
来源：http://blog.tarul.cn/Article/details/glylhghsq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/gaziinzpk.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.epnwcf.com/Article/details/ggxcujrut.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.bbcook.cn/Article/details/gcqpgfjap.sHtML

[U61] PHP：正则
来源：http://www.share.yfazqb.com/Article/details/gxftykhtd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gjaqzyumx.sHtML

[U62] PHP：日期对象
来源：http://read.share.vehdjk.com/Article/details/gwmrirdvs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fktsv.cn/Article/details/gqfavxdeg.sHtML

[U63] PHP：文件读写
来源：http://www.blog.yfazqb.com/Article/details/gdmudgsdf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.vehdjk.com/Article/details/gvzjrkzkc.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.yfazqb.com/Article/details/ghzylnezt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.yfazqb.com/Article/details/gsvsbhgua.sHtML

[U65] PHP：会话
来源：http://wap.bbcook.cn/Article/details/gxxmlxuom.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.tarul.cn/Article/details/gskhbchwu.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.epnwcf.com/Article/details/ghoesuwzt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.vehdjk.com/Article/details/gfgvzyndr.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.yfazqb.com/Article/details/gornbvvdz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.epnwcf.com/Article/details/gitbaifzb.sHtML

[U68] PHP：PDO 连接
来源：http://baike.sjlbkw.cn/Article/details/gbjdgofoa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.sjlbkw.cn/Article/details/gasjcjgij.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.sjlbkw.cn/Article/details/gjdmpoqmp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.tarul.cn/Article/details/gppxrgqiz.sHtML

[U70] PHP：PDO 事务
来源：http://3g.yfazqb.com/Article/details/gsqvptacr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fktsv.cn/Article/details/gesekzdze.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fktsv.cn/Article/details/gnhshpriy.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.epnwcf.com/Article/details/gepmdcjvq.sHtML

[U72] PHP：写错误日志
来源：http://baike.epnwcf.com/Article/details/gfnzmxtif.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.tarul.cn/Article/details/gokrasjur.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.vehdjk.com/Article/details/gmugsajem.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.vehdjk.com/Article/details/gopycjubx.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.bbcook.cn/Article/details/grivhcskf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.vehdjk.com/Article/details/gankxgstf.sHtML

[U75] PHP：依赖注入
来源：http://blog.bbcook.cn/Article/details/gmifuiujr.sHtML

composer require psr/container
来源：http://3g.tarul.cn/Article/details/gmmjjhsgk.sHtML

[U76] PHP：简单路由
来源：http://wap.tarul.cn/Article/details/gxbvnjanf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.yfazqb.com/Article/details/gmmdbcphx.sHtML

[U77] PHP：模板渲染
来源：http://3g.fktsv.cn/Article/details/grvoldour.sHtML

composer require twig/twig
来源：http://read.share.sjlbkw.cn/Article/details/gqutyhfeg.sHtML

[U78] PHP：单元测试
来源：http://baike.bbcook.cn/Article/details/gfopkcjhd.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.epnwcf.com/Article/details/gxrrvqvgl.sHtML

[U79] PHP：静态分析
来源：http://blog.yfazqb.com/Article/details/gehdiqyho.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fktsv.cn/Article/details/giyzmcmbc.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.bbcook.cn/Article/details/gavvpizqr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.tarul.cn/Article/details/gxmqowykz.sHtML

[U81] JS：初始化项目
来源：http://m.share.bbcook.cn/Article/details/gutddpcst.sHtML

npm init -y;  npm i express
来源：http://m.share.bbcook.cn/Article/details/glavzelfx.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.yfazqb.com/Article/details/ghxzdypvr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.bbcook.cn/Article/details/ghefobwsw.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fktsv.cn/Article/details/gevggpyab.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.tarul.cn/Article/details/gprcussyk.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.tarul.cn/Article/details/gkojbyyah.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.sjlbkw.cn/Article/details/geyodkohu.sHtML

[U85] JS：可选链
来源：http://read.share.sjlbkw.cn/Article/details/gdpoqkzoe.sHtML

a?.b?.c
来源：http://mobile.sjlbkw.cn/Article/details/gaqcfwypl.sHtML

[U86] JS：空值合并
来源：http://3g.epnwcf.com/Article/details/gmfleqekt.sHtML

a ?? b
来源：http://www.blog.yfazqb.com/Article/details/gkarmzlqt.sHtML

[U87] JS：解构默认值
来源：http://blog.tarul.cn/Article/details/gvasqqijc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fktsv.cn/Article/details/gkwzekelz.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.bbcook.cn/Article/details/gbpkbtkui.sHtML

{ ...a, ...b }
来源：http://www.blog.epnwcf.com/Article/details/gsoipwifg.sHtML

[U89] JS：数组去重
来源：http://3g.fktsv.cn/Article/details/gsfaquqic.sHtML

[...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/ghyieyscb.sHtML

[U90] JS：数字数组排序
来源：http://mobile.bbcook.cn/Article/details/gqcvorwxa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gqkkmvqkp.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.epnwcf.com/Article/details/gzkrctveu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.yfazqb.com/Article/details/gusbpgyyr.sHtML

[U92] JS：深拷贝
来源：http://mobile.bbcook.cn/Article/details/gwurknwhp.sHtML

structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gjizxanvr.sHtML

[U93] JS：模板字符串
来源：http://m.share.vehdjk.com/Article/details/guhrrjcmw.sHtML

`共 ${n} 条`
来源：http://www.blog.vehdjk.com/Article/details/gtotmmmti.sHtML

[U94] JS：箭头函数
来源：http://3g.epnwcf.com/Article/details/gstwewxuv.sHtML

const double = x => x * 2;
来源：http://3g.yfazqb.com/Article/details/gzdbzphdn.sHtML

[U95] JS：Promise 包装
来源：http://wap.fktsv.cn/Article/details/gplrnvyob.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.vehdjk.com/Article/details/gzwehummy.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fktsv.cn/Article/details/gnnajhilb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gwfpnujmu.sHtML

[U97] JS：并发请求
来源：http://www.share.fktsv.cn/Article/details/giytlgywp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gxpuzfsfp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fktsv.cn/Article/details/gigseqeoq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.bbcook.cn/Article/details/grtcpainh.sHtML

[U99] JS：事件监听
来源：http://read.share.epnwcf.com/Article/details/gdroexzsp.sHtML

el.addEventListener("click", e => {})
来源：http://3g.epnwcf.com/Article/details/gtadscgaf.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.bbcook.cn/Article/details/ggjshhwei.sHtML

document.querySelector(".item")
来源：http://m.share.yfazqb.com/Article/details/gxksofxzh.sHtML

[U101] JS：classList 操作
来源：http://www.blog.tarul.cn/Article/details/gocafgfyn.sHtML

el.classList.toggle("active")
来源：http://www.m.share.epnwcf.com/Article/details/gkagzuvvw.sHtML

[U102] JS：本地存储
来源：http://www.blog.fktsv.cn/Article/details/grhlxpyeb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fktsv.cn/Article/details/gmxcndxve.sHtML

[U103] JS：定时器
来源：http://m.share.bbcook.cn/Article/details/gmvxndlfl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.yfazqb.com/Article/details/gohxygaam.sHtML

[U104] JS：防抖
来源：http://read.share.epnwcf.com/Article/details/gvhazmawt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gvzyexfnk.sHtML

[U105] JS：节流
来源：http://www.share.yfazqb.com/Article/details/gsmwpqwka.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fktsv.cn/Article/details/gbhidnwba.sHtML

[U106] JS：日期格式化
来源：http://3g.fktsv.cn/Article/details/glmpjjjiw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fktsv.cn/Article/details/gptbbpuqg.sHtML

[U107] JS：数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gcdnwjaqi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.epnwcf.com/Article/details/gpvbqvcad.sHtML

[U108] JS：随机整数
来源：http://m.share.bbcook.cn/Article/details/gmsigupaj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.vehdjk.com/Article/details/glwyuxbec.sHtML

[U109] JS：数组分组
来源：http://mobile.tarul.cn/Article/details/gxjfxkqvp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gsnzynhwq.sHtML

[U110] JS：数组分块
来源：http://m.share.bbcook.cn/Article/details/gzjcwfxsw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.tarul.cn/Article/details/gfzmjiexf.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fktsv.cn/Article/details/geotozqar.sHtML

new Map(Object.entries(obj))
来源：http://m.share.sjlbkw.cn/Article/details/gtsfijixa.sHtML

[U112] JS：字符串补位
来源：http://www.blog.vehdjk.com/Article/details/ghxfelcqh.sHtML

"7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gdpxqajvg.sHtML

[U113] JS：正则替换全部
来源：http://m.share.sjlbkw.cn/Article/details/gvdprorxc.sHtML

s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gccfbgjkf.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fktsv.cn/Article/details/gtlhyupym.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gizlgmvou.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/gvhqivhec.sHtML

crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/grudbruce.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.bbcook.cn/Article/details/gbopjyjio.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.vehdjk.com/Article/details/grotoxnvq.sHtML

[U117] JS：单元测试
来源：http://www.blog.tarul.cn/Article/details/goywctfik.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.epnwcf.com/Article/details/gxpsmkzwr.sHtML

[U118] JS：开发服务器
来源：http://m.share.yfazqb.com/Article/details/gamkxojfl.sHtML

npm i -D vite;  npx vite
来源：http://www.share.bbcook.cn/Article/details/ghgbmvhwf.sHtML

[U119] JS：生产构建
来源：http://3g.sjlbkw.cn/Article/details/ghgftmrax.sHtML

npx vite build
来源：http://m.share.sjlbkw.cn/Article/details/gqbnfmzoc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.vehdjk.com/Article/details/ghrhyxnrs.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.bbcook.cn/Article/details/gypmfuvwr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grfvlojmd.sHtML

统计汇总
来源：http://www.m.share.bbcook.cn/Article/details/gnkoitahd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gxhlwttor.sHtML

按语言统计（条）：
来源：http://mobile.yfazqb.com/Article/details/gxyleveoh.sHtML

Python ......... 252
来源：http://www.blog.bbcook.cn/Article/details/gdbdtuqsd.sHtML

PHP ............ 252
来源：http://baike.vehdjk.com/Article/details/grwgsbvnk.sHtML

JavaScript ..... 252
来源：http://baike.epnwcf.com/Article/details/gahdfridq.sHtML

TypeScript ..... 212
来源：http://www.blog.vehdjk.com/Article/details/gldhqxdim.sHtML

Java ........... 212
来源：http://blog.tarul.cn/Article/details/gkmjxvyqn.sHtML

Go ............. 212
来源：http://3g.yfazqb.com/Article/details/gosezgpby.sHtML

Ruby ........... 212
来源：http://www.blog.fktsv.cn/Article/details/gxgusddff.sHtML

C# ............. 212
来源：http://www.blog.sjlbkw.cn/Article/details/gkkeskozv.sHtML

C .............. 30
来源：http://baike.fktsv.cn/Article/details/gtxkwffsy.sHtML

C++ ............ 30
来源：http://www.m.share.bbcook.cn/Article/details/gvddgkshu.sHtML

SQL ............ 90
来源：http://www.blog.sjlbkw.cn/Article/details/gsjbxetyw.sHtML

Bash ........... 80
来源：http://www.m.share.fktsv.cn/Article/details/grxvdezls.sHtML

Kotlin ......... 15
来源：http://wap.fktsv.cn/Article/details/gufbijcov.sHtML

Swift .......... 15
来源：http://blog.tarul.cn/Article/details/gzywjtsbv.sHtML

Lua ............ 10
来源：http://blog.epnwcf.com/Article/details/gmgfqlfig.sHtML

Perl ........... 10
来源：http://m.share.yfazqb.com/Article/details/goamxamnq.sHtML

Scala .......... 10
来源：http://www.share.bbcook.cn/Article/details/gzayimhxr.sHtML

------------------------------------
来源：http://wap.yfazqb.com/Article/details/gtepqavyi.sHtML

合计 ........... 2106 条
来源：http://wap.yfazqb.com/Article/details/gjpumvtpq.sHtML

按章节统计：
来源：http://www.m.share.tarul.cn/Article/details/gdrzgrmla.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.bbcook.cn/Article/details/gyacfsedb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gcgechtzf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/geyzznsel.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/gfevvknzu.sHtML


<!-- 参考信息 -->