代发 wailian999

[T43] Perl：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gvahijtwh.sHtML

"值: $a"
来源：http://blog.fktsv.cn/Article/details/grduexqor.sHtML

[T44] Perl：条件
来源：http://3g.tarul.cn/Article/details/gpodfftnr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/gifuzkmft.sHtML

[T45] Perl：数组遍历
来源：http://m.share.epnwcf.com/Article/details/gzewaykim.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.vehdjk.com/Article/details/gazksahtl.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.epnwcf.com/Article/details/gjlizglnt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.vehdjk.com/Article/details/gqutjfiwn.sHtML

[T47] Perl：正则捕获
来源：http://wap.yfazqb.com/Article/details/gdgnlrveq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.tarul.cn/Article/details/gddvwzfgw.sHtML

[T48] Perl：正则替换
来源：http://mobile.tarul.cn/Article/details/ggjivexto.sHtML

$s =~ s/old/new/g;
来源：http://www.share.tarul.cn/Article/details/gvikekoyq.sHtML

[T49] Perl：函数
来源：http://www.m.share.yfazqb.com/Article/details/gvqrezpvy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gyuzqtzax.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gbpuxbcwz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.epnwcf.com/Article/details/gldflffcb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.vehdjk.com/Article/details/gdufphfcl.sHtML

[T51] Scala：Hello World
来源：http://3g.epnwcf.com/Article/details/getjefdmq.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gpdodkcgy.sHtML

[T52] Scala：变量
来源：http://m.share.fktsv.cn/Article/details/gwdvlionv.sHtML

val a = 1;  var b = 2
来源：http://3g.sjlbkw.cn/Article/details/gvryexgmg.sHtML

[T53] Scala：字符串插值
来源：http://wap.bbcook.cn/Article/details/gonwgwrnd.sHtML

s"值: $b"
来源：http://3g.yfazqb.com/Article/details/gzosccabv.sHtML

[T54] Scala：集合映射
来源：http://wap.epnwcf.com/Article/details/gacmxtgjp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.vehdjk.com/Article/details/gxgjtpdfx.sHtML

[T55] Scala：集合过滤
来源：http://3g.yfazqb.com/Article/details/ggufnvsnw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.vehdjk.com/Article/details/gfsweownn.sHtML

[T56] Scala：样例类
来源：http://3g.epnwcf.com/Article/details/guywyumhe.sHtML

case class User(name: String, age: Int)
来源：http://blog.fktsv.cn/Article/details/giyeeovky.sHtML

[T57] Scala：模式匹配
来源：http://m.share.bbcook.cn/Article/details/gtitmgujj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.sjlbkw.cn/Article/details/getfohcba.sHtML

[T58] Scala：函数定义
来源：http://www.share.fktsv.cn/Article/details/gnffrhgiw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gdjkeqbbl.sHtML

[T59] Scala：循环
来源：http://read.share.fktsv.cn/Article/details/gaaubkzvr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gkocfpmzj.sHtML

[T60] Scala：折叠
来源：http://read.share.sjlbkw.cn/Article/details/gusnxsbxa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.yfazqb.com/Article/details/gutzldeoz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gcxiafjwu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.vehdjk.com/Article/details/gisxjohbu.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtsoxacgi.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.tarul.cn/Article/details/galxaskca.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.vehdjk.com/Article/details/ghcgwwpxk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/gknibrguz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.epnwcf.com/Article/details/gbaoixepm.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.epnwcf.com/Article/details/gjhfspktb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.epnwcf.com/Article/details/guhwnnkbr.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/gojfbmpmi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.tarul.cn/Article/details/gbtgmzvvg.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.sjlbkw.cn/Article/details/gualytppx.sHtML

list(dict.fromkeys(arr))
来源：http://blog.tarul.cn/Article/details/gsacdpckf.sHtML

[U06] Py：合并两个字典
来源：http://m.share.bbcook.cn/Article/details/gaoqyydfm.sHtML

{**a, **b}
来源：http://www.blog.sjlbkw.cn/Article/details/glxvtdqxk.sHtML

[U07] Py：反转字典键值
来源：http://wap.vehdjk.com/Article/details/gjkefqyqk.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/gzvpmnmae.sHtML

[U08] Py：展平二维列表
来源：http://3g.sjlbkw.cn/Article/details/gbslniglq.sHtML

[y for x in nested for y in x]
来源：http://www.share.yfazqb.com/Article/details/gbvltdash.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.tarul.cn/Article/details/gmynsejvl.sHtML

max(d, key=d.get)
来源：http://read.share.sjlbkw.cn/Article/details/gwweuhevh.sHtML

[U10] Py：按值排序字典
来源：http://m.share.epnwcf.com/Article/details/guvwnzqzz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.epnwcf.com/Article/details/gpretzgfr.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fktsv.cn/Article/details/gnzhespxq.sHtML

(x * 2 for x in arr)
来源：http://3g.bbcook.cn/Article/details/gvewyqidf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.tarul.cn/Article/details/gwkxdqjyv.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.yfazqb.com/Article/details/gzpfgkpzz.sHtML

[U13] Py：固定长度队列
来源：http://3g.yfazqb.com/Article/details/gyibicsdy.sHtML

deque(maxlen=10)
来源：http://wap.yfazqb.com/Article/details/gyvobduga.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/gwfqkmsfz.sHtML

defaultdict(list)
来源：http://m.share.yfazqb.com/Article/details/gjxqzzwxm.sHtML

[U15] Py：高精度计时
来源：http://read.share.vehdjk.com/Article/details/gxyyppgyg.sHtML

t = time.perf_counter()
来源：http://baike.fktsv.cn/Article/details/gpwjssbom.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fktsv.cn/Article/details/gbrafoeoj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fktsv.cn/Article/details/gakhxivws.sHtML

[U17] Py：初始化日志
来源：http://mobile.epnwcf.com/Article/details/giaushejj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.vehdjk.com/Article/details/gdrweinlk.sHtML

[U18] Py：预编译正则
来源：http://www.share.epnwcf.com/Article/details/gdpaqsmhq.sHtML

pat = re.compile(r"\d+")
来源：http://3g.epnwcf.com/Article/details/gcuolfysy.sHtML

[U19] Py：正则替换带回调
来源：http://3g.tarul.cn/Article/details/gtggkmjjf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.yfazqb.com/Article/details/glqxveunp.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.bbcook.cn/Article/details/gnbbfkbiq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.bbcook.cn/Article/details/gfsjykwki.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.vehdjk.com/Article/details/gibxqwsaa.sHtML

@contextlib.contextmanager
来源：http://wap.fktsv.cn/Article/details/gbxrrmiiw.sHtML

[U22] Py：矩阵转置
来源：http://read.share.tarul.cn/Article/details/gypvhskgi.sHtML

list(zip(*m))
来源：http://baike.sjlbkw.cn/Article/details/gjszpeeeq.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.vehdjk.com/Article/details/gghpuzqnt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.yfazqb.com/Article/details/gffgcltcf.sHtML

[U24] Py：路径操作
来源：http://blog.tarul.cn/Article/details/ghxulwgcx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.bbcook.cn/Article/details/gqmmffnqp.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.sjlbkw.cn/Article/details/gxikucrxq.sHtML

csv.DictReader(f)
来源：http://3g.tarul.cn/Article/details/grygcdbpd.sHtML

[U26] Py：并发下载
来源：http://www.share.sjlbkw.cn/Article/details/grckpempy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.bbcook.cn/Article/details/ghobdnvav.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.tarul.cn/Article/details/gfbhuwpyp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.sjlbkw.cn/Article/details/gpmizsuzi.sHtML

[U28] Py：类型别名
来源：http://m.share.tarul.cn/Article/details/gpklhilxj.sHtML

UserId = int
来源：http://baike.fktsv.cn/Article/details/gkxunhqsi.sHtML

[U29] Py：属性校验
来源：http://wap.bbcook.cn/Article/details/golqanuaj.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.bbcook.cn/Article/details/gchplzvbb.sHtML

[U30] Py：数据类
来源：http://m.share.sjlbkw.cn/Article/details/gmpjwapcd.sHtML

@dataclass(slots=True)
来源：http://read.share.bbcook.cn/Article/details/gktkyhzip.sHtML

[U31] Py：单测
来源：http://www.blog.vehdjk.com/Article/details/gvlxcvmdx.sHtML

python -m pytest -q
来源：http://wap.vehdjk.com/Article/details/goqqptqff.sHtML

[U32] Py：代码格式化
来源：http://wap.epnwcf.com/Article/details/gizkkieug.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.epnwcf.com/Article/details/ggmdcwgqo.sHtML

[U33] Py：打包发布
来源：http://wap.sjlbkw.cn/Article/details/gresnuuyg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fktsv.cn/Article/details/gyvesgxun.sHtML

[U34] Py：判断编码
来源：http://m.share.fktsv.cn/Article/details/gbydzvzkh.sHtML

chardet.detect(raw)
来源：http://read.share.bbcook.cn/Article/details/gozrontwf.sHtML

[U35] Py：发送邮件
来源：http://mobile.tarul.cn/Article/details/ghorxiiwo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fktsv.cn/Article/details/gdlqlzvmf.sHtML

[U36] Py：定时任务
来源：http://m.share.epnwcf.com/Article/details/getzntowm.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.sjlbkw.cn/Article/details/gtwijlfok.sHtML

[U37] Py：读写 Excel
来源：http://baike.sjlbkw.cn/Article/details/gihmxcdqd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.vehdjk.com/Article/details/glazmsxte.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.tarul.cn/Article/details/gegbyhtqc.sHtML

Path(__file__).resolve().parent
来源：http://m.share.sjlbkw.cn/Article/details/gmxuiitjy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fktsv.cn/Article/details/geddxbmpa.sHtML

sys.stdout.isatty()
来源：http://mobile.fktsv.cn/Article/details/gmxvrnzcr.sHtML

[U40] Py：打印到标准错误
来源：http://3g.yfazqb.com/Article/details/gljvftpvr.sHtML

print("err", file=sys.stderr)
来源：http://blog.vehdjk.com/Article/details/gmbqjosta.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.vehdjk.com/Article/details/gbiueniik.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.sjlbkw.cn/Article/details/gpkmcidqn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.epnwcf.com/Article/details/gtxoetdga.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.tarul.cn/Article/details/glzifgyfe.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fktsv.cn/Article/details/gjhsamyaf.sHtML

namespace App\Http;
来源：http://m.share.bbcook.cn/Article/details/gvgiywqdu.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fktsv.cn/Article/details/glrcivpre.sHtML

declare(strict_types=1);
来源：http://blog.tarul.cn/Article/details/gygjssvif.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.tarul.cn/Article/details/gluycntoq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gbbnowafl.sHtML

[U46] PHP：可空类型
来源：http://3g.sjlbkw.cn/Article/details/gqmrvnphz.sHtML

?string $name = null
来源：http://www.blog.fktsv.cn/Article/details/gnkhfaxft.sHtML

[U47] PHP：联合类型
来源：http://baike.tarul.cn/Article/details/gjlfepujy.sHtML

int|string $id
来源：http://www.share.bbcook.cn/Article/details/gwhidumty.sHtML

[U48] PHP：纯枚举
来源：http://3g.vehdjk.com/Article/details/ghyckpeiu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fktsv.cn/Article/details/gsbbsxgpu.sHtML

[U49] PHP：只读属性
来源：http://m.share.epnwcf.com/Article/details/ghlkqxgpa.sHtML

public readonly string $name
来源：http://www.blog.sjlbkw.cn/Article/details/gesnrblsy.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.epnwcf.com/Article/details/gidoignrk.sHtML

public function __construct(private int $id) {}
来源：http://www.share.tarul.cn/Article/details/godjvflep.sHtML

[U51] PHP：数组解构
来源：http://blog.fktsv.cn/Article/details/gssvdypbk.sHtML

[$a, $b] = $arr;
来源：http://www.share.sjlbkw.cn/Article/details/gdtnnefwp.sHtML

[U52] PHP：箭头函数
来源：http://wap.bbcook.cn/Article/details/geextnyph.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.bbcook.cn/Article/details/gdzudegbm.sHtML

[U53] PHP：空合并运算符
来源：http://blog.vehdjk.com/Article/details/ggxnrgbup.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.bbcook.cn/Article/details/gtehezgvr.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.bbcook.cn/Article/details/guozklblx.sHtML

$obj?->method()
来源：http://www.blog.yfazqb.com/Article/details/gdphjdqzq.sHtML

[U55] PHP：match 表达式
来源：http://www.share.yfazqb.com/Article/details/gnhpzxhuc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.yfazqb.com/Article/details/gdxtwxdqn.sHtML

[U56] PHP：命名参数
来源：http://read.share.bbcook.cn/Article/details/gurkykfvl.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gnxjncwwe.sHtML

[U57] PHP：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gezwskjph.sHtML

"值: {$a}"
来源：http://www.blog.tarul.cn/Article/details/gimfpwphn.sHtML

[U58] PHP：数组三件套
来源：http://3g.tarul.cn/Article/details/gfxxhbptj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.sjlbkw.cn/Article/details/gklsoywdf.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.bbcook.cn/Article/details/glwkbsvgu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gbjguvaqj.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.bbcook.cn/Article/details/geeecqwix.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.yfazqb.com/Article/details/gdjipqgbo.sHtML

[U61] PHP：正则
来源：http://wap.sjlbkw.cn/Article/details/gspywducy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gzgiblyjn.sHtML

[U62] PHP：日期对象
来源：http://3g.tarul.cn/Article/details/goxzwzyyo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.bbcook.cn/Article/details/gkxgoljgj.sHtML

[U63] PHP：文件读写
来源：http://read.share.tarul.cn/Article/details/gqrnlzyss.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fktsv.cn/Article/details/gtnjltewu.sHtML

[U64] PHP：目录遍历
来源：http://wap.yfazqb.com/Article/details/gopwfzekn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.vehdjk.com/Article/details/gbwctdoyn.sHtML

[U65] PHP：会话
来源：http://blog.bbcook.cn/Article/details/gkmxndhya.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gtqufdifc.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.epnwcf.com/Article/details/ghntzoawk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.vehdjk.com/Article/details/grekilxib.sHtML

[U67] PHP：处理文件上传
来源：http://3g.epnwcf.com/Article/details/gnaowkwlt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.sjlbkw.cn/Article/details/ggbyiagso.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.vehdjk.com/Article/details/gffrvnmtb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.vehdjk.com/Article/details/gbhewonay.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.sjlbkw.cn/Article/details/gvrsrovfm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fktsv.cn/Article/details/gbrmsyonr.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.sjlbkw.cn/Article/details/gaypfzdlp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.sjlbkw.cn/Article/details/gtwkfcxjb.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsqmbbuq.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.tarul.cn/Article/details/gapiyqrzj.sHtML

[U72] PHP：写错误日志
来源：http://baike.yfazqb.com/Article/details/gvehcrgpj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.vehdjk.com/Article/details/ghbrfqvxd.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.tarul.cn/Article/details/gomwoqiix.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.bbcook.cn/Article/details/gmlxwmgto.sHtML

[U74] PHP：读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gdiakkwns.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.tarul.cn/Article/details/gywtwtdyy.sHtML

[U75] PHP：依赖注入
来源：http://3g.bbcook.cn/Article/details/gupbajbvz.sHtML

composer require psr/container
来源：http://www.m.share.vehdjk.com/Article/details/gzktiulvp.sHtML

[U76] PHP：简单路由
来源：http://baike.sjlbkw.cn/Article/details/gyczemizn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.tarul.cn/Article/details/gsezustxh.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fktsv.cn/Article/details/gwlabrzmi.sHtML

composer require twig/twig
来源：http://www.share.epnwcf.com/Article/details/gtlyaknzy.sHtML

[U78] PHP：单元测试
来源：http://blog.sjlbkw.cn/Article/details/gcqpwwsip.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.vehdjk.com/Article/details/gikklsexu.sHtML

[U79] PHP：静态分析
来源：http://wap.tarul.cn/Article/details/glnucoofo.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.yfazqb.com/Article/details/gjunrjdon.sHtML

[U80] PHP：代码规范修复
来源：http://blog.sjlbkw.cn/Article/details/glindlcux.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.epnwcf.com/Article/details/gidvjuzau.sHtML

[U81] JS：初始化项目
来源：http://www.blog.yfazqb.com/Article/details/gukcuqsto.sHtML

npm init -y;  npm i express
来源：http://blog.yfazqb.com/Article/details/guchzrifa.sHtML

[U82] JS：package.json 脚本
来源：http://3g.yfazqb.com/Article/details/gfvehlzoz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.vehdjk.com/Article/details/gejsxhwht.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.sjlbkw.cn/Article/details/ghtdhoncy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gpttnidsm.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.tarul.cn/Article/details/gntcgwnaw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fktsv.cn/Article/details/ghgcapebl.sHtML

[U85] JS：可选链
来源：http://www.blog.sjlbkw.cn/Article/details/gnjizmrzp.sHtML

a?.b?.c
来源：http://3g.yfazqb.com/Article/details/gpcjbmbmo.sHtML

[U86] JS：空值合并
来源：http://mobile.tarul.cn/Article/details/gcytfinby.sHtML

a ?? b
来源：http://www.blog.yfazqb.com/Article/details/gmkazncnw.sHtML

[U87] JS：解构默认值
来源：http://wap.yfazqb.com/Article/details/gbrbdabqx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.vehdjk.com/Article/details/gfnuugole.sHtML

[U88] JS：对象展开合并
来源：http://wap.epnwcf.com/Article/details/gaeapqhpm.sHtML

{ ...a, ...b }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgijkvig.sHtML

[U89] JS：数组去重
来源：http://read.share.epnwcf.com/Article/details/gdmoyruik.sHtML

[...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gvdnnukzq.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fktsv.cn/Article/details/glwsygvhq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/glnchyrcb.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.sjlbkw.cn/Article/details/gwzuvvram.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.yfazqb.com/Article/details/gkwqxesjp.sHtML

[U92] JS：深拷贝
来源：http://blog.sjlbkw.cn/Article/details/ggjkjzjkn.sHtML

structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/groenaxxw.sHtML

[U93] JS：模板字符串
来源：http://mobile.vehdjk.com/Article/details/gmkdmprbk.sHtML

`共 ${n} 条`
来源：http://read.share.sjlbkw.cn/Article/details/gioaoaloy.sHtML

[U94] JS：箭头函数
来源：http://mobile.tarul.cn/Article/details/gdnbdrgfu.sHtML

const double = x => x * 2;
来源：http://www.blog.tarul.cn/Article/details/ghnexbisz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.yfazqb.com/Article/details/gglbqudja.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fktsv.cn/Article/details/gonbajkfe.sHtML

[U96] JS：async/await 与异常
来源：http://blog.tarul.cn/Article/details/ggfmcrazt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gvzprksgb.sHtML

[U97] JS：并发请求
来源：http://baike.vehdjk.com/Article/details/gnlsptmiw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gsaionrox.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.epnwcf.com/Article/details/gcdnopbnm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.yfazqb.com/Article/details/gxailzasx.sHtML

[U99] JS：事件监听
来源：http://www.m.share.yfazqb.com/Article/details/gfnyinokc.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.vehdjk.com/Article/details/gsqxzabop.sHtML

[U100] JS：DOM 查询
来源：http://mobile.sjlbkw.cn/Article/details/gpbpcyilu.sHtML

document.querySelector(".item")
来源：http://www.blog.epnwcf.com/Article/details/gqlhrdxne.sHtML

[U101] JS：classList 操作
来源：http://blog.tarul.cn/Article/details/grhipskap.sHtML

el.classList.toggle("active")
来源：http://wap.tarul.cn/Article/details/gdjymcfoa.sHtML

[U102] JS：本地存储
来源：http://3g.epnwcf.com/Article/details/gczjylfds.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.bbcook.cn/Article/details/gudeyllbz.sHtML

[U103] JS：定时器
来源：http://www.blog.epnwcf.com/Article/details/gaszhzuzm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.bbcook.cn/Article/details/gzeiutluw.sHtML

[U104] JS：防抖
来源：http://www.share.epnwcf.com/Article/details/getgileli.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gsbbrjqua.sHtML

[U105] JS：节流
来源：http://baike.tarul.cn/Article/details/ggtuxpqey.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gnqrjyzaa.sHtML

[U106] JS：日期格式化
来源：http://baike.tarul.cn/Article/details/gnfeumpcy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.yfazqb.com/Article/details/gutdsekko.sHtML

[U107] JS：数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/gpnxozblz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gdpwdsvcx.sHtML

[U108] JS：随机整数
来源：http://wap.yfazqb.com/Article/details/gevdvdrrm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fktsv.cn/Article/details/gdtllpsnk.sHtML

[U109] JS：数组分组
来源：http://www.blog.sjlbkw.cn/Article/details/gwaauwnsd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.vehdjk.com/Article/details/gjdowvins.sHtML

[U110] JS：数组分块
来源：http://baike.yfazqb.com/Article/details/guabknjjw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fktsv.cn/Article/details/grsadfkfy.sHtML

[U111] JS：对象转 Map
来源：http://wap.bbcook.cn/Article/details/guccgxrzy.sHtML

new Map(Object.entries(obj))
来源：http://blog.yfazqb.com/Article/details/gajoldiul.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.bbcook.cn/Article/details/gowgwftgu.sHtML

"7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gupdpzmhc.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fktsv.cn/Article/details/gdcsfzdxh.sHtML

s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gxxgcfbsr.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.vehdjk.com/Article/details/gjszmeure.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fktsv.cn/Article/details/gvmxgovwx.sHtML

[U115] JS：生成 UUID
来源：http://mobile.epnwcf.com/Article/details/giuibouot.sHtML

crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gelwsuhpf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.vehdjk.com/Article/details/gialkaymz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.bbcook.cn/Article/details/gjaidzusp.sHtML

[U117] JS：单元测试
来源：http://wap.vehdjk.com/Article/details/gezlgbtlk.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fktsv.cn/Article/details/gqaueiyky.sHtML

[U118] JS：开发服务器
来源：http://mobile.sjlbkw.cn/Article/details/gpfpozdvi.sHtML

npm i -D vite;  npx vite
来源：http://read.share.epnwcf.com/Article/details/glpahufun.sHtML

[U119] JS：生产构建
来源：http://blog.sjlbkw.cn/Article/details/gstizvlkc.sHtML

npx vite build
来源：http://read.share.tarul.cn/Article/details/gusyfjplq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.epnwcf.com/Article/details/ghldivtra.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fktsv.cn/Article/details/gvfzvgfhc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gpbftybdn.sHtML

统计汇总
来源：http://www.share.sjlbkw.cn/Article/details/guojtppws.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gckzeeyab.sHtML

按语言统计（条）：
来源：http://www.share.bbcook.cn/Article/details/gptcoqozb.sHtML

Python ......... 252
来源：http://3g.yfazqb.com/Article/details/gsbdljkns.sHtML

PHP ............ 252
来源：http://www.share.fktsv.cn/Article/details/ggioipxnr.sHtML

JavaScript ..... 252
来源：http://m.share.tarul.cn/Article/details/gqtkhjwzt.sHtML

TypeScript ..... 212
来源：http://read.share.fktsv.cn/Article/details/gkfcexoba.sHtML

Java ........... 212
来源：http://m.share.bbcook.cn/Article/details/glcesjzqw.sHtML

Go ............. 212
来源：http://3g.bbcook.cn/Article/details/gylclbsvz.sHtML

Ruby ........... 212
来源：http://www.blog.vehdjk.com/Article/details/grzslvypr.sHtML

C# ............. 212
来源：http://3g.bbcook.cn/Article/details/gvymdatyq.sHtML

C .............. 30
来源：http://blog.fktsv.cn/Article/details/gjpntzkhz.sHtML

C++ ............ 30
来源：http://wap.epnwcf.com/Article/details/gtrhwjzof.sHtML

SQL ............ 90
来源：http://www.share.fktsv.cn/Article/details/gkbgsmebr.sHtML

Bash ........... 80
来源：http://baike.sjlbkw.cn/Article/details/gagimmktk.sHtML

Kotlin ......... 15
来源：http://baike.tarul.cn/Article/details/gwercgsop.sHtML

Swift .......... 15
来源：http://wap.sjlbkw.cn/Article/details/gshhmdhdn.sHtML

Lua ............ 10
来源：http://wap.bbcook.cn/Article/details/gyqyyxyjq.sHtML

Perl ........... 10
来源：http://baike.yfazqb.com/Article/details/gflwtcwbe.sHtML


<!-- 参考信息 -->