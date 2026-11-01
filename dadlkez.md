代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://blog.epnwcf.com/Article/details/gezsnjdxa.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gtpvbjhph.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gdenbsusd.sHtML

[T52] Scala：变量
来源：http://www.blog.fktsv.cn/Article/details/glhdkpnoz.sHtML

val a = 1;  var b = 2
来源：http://mobile.bbcook.cn/Article/details/ghfbnncvx.sHtML

[T53] Scala：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gmarsuvic.sHtML

s"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gstxrzkra.sHtML

[T54] Scala：集合映射
来源：http://www.share.vehdjk.com/Article/details/gawzuxsts.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.vehdjk.com/Article/details/gajahwgjn.sHtML

[T55] Scala：集合过滤
来源：http://www.share.tarul.cn/Article/details/gkjcmunld.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.bbcook.cn/Article/details/gtnikhyee.sHtML

[T56] Scala：样例类
来源：http://blog.sjlbkw.cn/Article/details/ghefjqiko.sHtML

case class User(name: String, age: Int)
来源：http://mobile.tarul.cn/Article/details/gvoizzkpd.sHtML

[T57] Scala：模式匹配
来源：http://blog.yfazqb.com/Article/details/gpjzwimup.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/ghzeqveaa.sHtML

[T58] Scala：函数定义
来源：http://read.share.bbcook.cn/Article/details/gjyjcoall.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.vehdjk.com/Article/details/gpufkbcqi.sHtML

[T59] Scala：循环
来源：http://www.blog.vehdjk.com/Article/details/godaritld.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/guhnjfzab.sHtML

[T60] Scala：折叠
来源：http://m.share.vehdjk.com/Article/details/gmztboinl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.tarul.cn/Article/details/gddrsezqq.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gqjbyfydx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.vehdjk.com/Article/details/gznkczqvm.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gxtydhxuq.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/gbmuhucss.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.yfazqb.com/Article/details/gbyustdpb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.bbcook.cn/Article/details/gqeaduulr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.vehdjk.com/Article/details/gqtmrdbda.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.sjlbkw.cn/Article/details/gmkhbkuvq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fktsv.cn/Article/details/gzcrqczdw.sHtML

[U04] Py：变量调试打印
来源：http://www.share.epnwcf.com/Article/details/goljekjmk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.tarul.cn/Article/details/gbmtkduiz.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.bbcook.cn/Article/details/glpfokptl.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.bbcook.cn/Article/details/guyghxzmq.sHtML

[U06] Py：合并两个字典
来源：http://m.share.bbcook.cn/Article/details/gyxgewxmi.sHtML

{**a, **b}
来源：http://read.share.sjlbkw.cn/Article/details/gwrwmrkea.sHtML

[U07] Py：反转字典键值
来源：http://mobile.epnwcf.com/Article/details/gbddqbeuw.sHtML

{v: k for k, v in d.items()}
来源：http://baike.sjlbkw.cn/Article/details/gkaurwakw.sHtML

[U08] Py：展平二维列表
来源：http://wap.tarul.cn/Article/details/gfkhbbmfc.sHtML

[y for x in nested for y in x]
来源：http://www.blog.tarul.cn/Article/details/gtfmtwdhi.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.yfazqb.com/Article/details/goqrnikfg.sHtML

max(d, key=d.get)
来源：http://wap.vehdjk.com/Article/details/ghvalcraj.sHtML

[U10] Py：按值排序字典
来源：http://wap.sjlbkw.cn/Article/details/glnbyfjwb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.bbcook.cn/Article/details/gpovdjvgi.sHtML

[U11] Py：生成器表达式
来源：http://baike.bbcook.cn/Article/details/gzdzewzjt.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fktsv.cn/Article/details/gmsbanjgb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.tarul.cn/Article/details/gstepxwed.sHtML

Counter(arr).most_common(3)
来源：http://wap.tarul.cn/Article/details/gphrtxdro.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.bbcook.cn/Article/details/gxptqngnu.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/goxlmjouj.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.epnwcf.com/Article/details/gtcgcmbyb.sHtML

defaultdict(list)
来源：http://www.share.tarul.cn/Article/details/glsauyqvj.sHtML

[U15] Py：高精度计时
来源：http://www.share.bbcook.cn/Article/details/gjcokvuac.sHtML

t = time.perf_counter()
来源：http://www.share.vehdjk.com/Article/details/gwqwlpmcc.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.tarul.cn/Article/details/gnqmuhtxn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.tarul.cn/Article/details/gphhawqtu.sHtML

[U17] Py：初始化日志
来源：http://mobile.epnwcf.com/Article/details/glqwhowgm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.epnwcf.com/Article/details/gtqxukjai.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/gaocvxwal.sHtML

pat = re.compile(r"\d+")
来源：http://3g.vehdjk.com/Article/details/gumnemmaw.sHtML

[U19] Py：正则替换带回调
来源：http://blog.sjlbkw.cn/Article/details/gprrjvttd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.bbcook.cn/Article/details/grttyunmj.sHtML

[U20] Py：缓存函数结果
来源：http://blog.epnwcf.com/Article/details/ggnanykfm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.epnwcf.com/Article/details/ghxhdhxcb.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.yfazqb.com/Article/details/gmosqlxoe.sHtML

@contextlib.contextmanager
来源：http://www.share.fktsv.cn/Article/details/gxwfqgafm.sHtML

[U22] Py：矩阵转置
来源：http://baike.tarul.cn/Article/details/gztgeihph.sHtML

list(zip(*m))
来源：http://www.m.share.yfazqb.com/Article/details/gxtqlxrfm.sHtML

[U23] Py：分块读取大文件
来源：http://baike.tarul.cn/Article/details/gkzedommz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.sjlbkw.cn/Article/details/gjplhlwvr.sHtML

[U24] Py：路径操作
来源：http://mobile.fktsv.cn/Article/details/gkoxtaphd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gkmitgqvy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.tarul.cn/Article/details/gifddjccb.sHtML

csv.DictReader(f)
来源：http://3g.epnwcf.com/Article/details/gmhoqkayd.sHtML

[U26] Py：并发下载
来源：http://m.share.yfazqb.com/Article/details/gdjbuthsk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.sjlbkw.cn/Article/details/gezylflbx.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.bbcook.cn/Article/details/grrqwoxjf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.yfazqb.com/Article/details/gpiijvnkm.sHtML

[U28] Py：类型别名
来源：http://3g.epnwcf.com/Article/details/gvbgowisk.sHtML

UserId = int
来源：http://wap.vehdjk.com/Article/details/gsfwmcjoj.sHtML

[U29] Py：属性校验
来源：http://wap.tarul.cn/Article/details/gerfkursg.sHtML

@property 与 @x.setter 配合
来源：http://3g.epnwcf.com/Article/details/gikauohuq.sHtML

[U30] Py：数据类
来源：http://baike.fktsv.cn/Article/details/gscxhmflv.sHtML

@dataclass(slots=True)
来源：http://baike.vehdjk.com/Article/details/geuizktmt.sHtML

[U31] Py：单测
来源：http://www.m.share.tarul.cn/Article/details/gybgaxjxg.sHtML

python -m pytest -q
来源：http://read.share.yfazqb.com/Article/details/gcoabyjym.sHtML

[U32] Py：代码格式化
来源：http://mobile.sjlbkw.cn/Article/details/gurgihfur.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.tarul.cn/Article/details/gvnftbytj.sHtML

[U33] Py：打包发布
来源：http://www.m.share.yfazqb.com/Article/details/gbasqgvpv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fktsv.cn/Article/details/gdqjapwuk.sHtML

[U34] Py：判断编码
来源：http://www.share.sjlbkw.cn/Article/details/gqqzvqxas.sHtML

chardet.detect(raw)
来源：http://wap.epnwcf.com/Article/details/gzsznmpem.sHtML

[U35] Py：发送邮件
来源：http://3g.fktsv.cn/Article/details/gbvhdeggu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.tarul.cn/Article/details/gtjtvqszo.sHtML

[U36] Py：定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gstfhfxrt.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fktsv.cn/Article/details/glapvrrhw.sHtML

[U37] Py：读写 Excel
来源：http://mobile.tarul.cn/Article/details/ghvagylnu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.bbcook.cn/Article/details/gaogdrlol.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.sjlbkw.cn/Article/details/gtlplsumx.sHtML

Path(__file__).resolve().parent
来源：http://blog.bbcook.cn/Article/details/gtuhbmcgy.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.sjlbkw.cn/Article/details/gpszfqlxz.sHtML

sys.stdout.isatty()
来源：http://3g.epnwcf.com/Article/details/gksrjkggh.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.sjlbkw.cn/Article/details/gpvdspgau.sHtML

print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gijewunly.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.epnwcf.com/Article/details/ghnvvwpoo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fktsv.cn/Article/details/gxwfcucsj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.tarul.cn/Article/details/gjshrqbuc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.vehdjk.com/Article/details/gzfywcpwp.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.vehdjk.com/Article/details/gcxkkbtzz.sHtML

namespace App\Http;
来源：http://baike.yfazqb.com/Article/details/gmbwrkqkl.sHtML

[U44] PHP：开启严格类型
来源：http://baike.vehdjk.com/Article/details/gbocufwtc.sHtML

declare(strict_types=1);
来源：http://baike.bbcook.cn/Article/details/gveoktwfp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.sjlbkw.cn/Article/details/gkzpbnair.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gpagufegf.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fktsv.cn/Article/details/gcvumgoac.sHtML

?string $name = null
来源：http://wap.epnwcf.com/Article/details/gchfcjvmq.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fktsv.cn/Article/details/goqdylldd.sHtML

int|string $id
来源：http://www.m.share.epnwcf.com/Article/details/gzidqhdoy.sHtML

[U48] PHP：纯枚举
来源：http://m.share.yfazqb.com/Article/details/gjuuvssrh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.vehdjk.com/Article/details/gcrihgwii.sHtML

[U49] PHP：只读属性
来源：http://m.share.vehdjk.com/Article/details/gczvncxkm.sHtML

public readonly string $name
来源：http://baike.tarul.cn/Article/details/glnndcjmc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.yfazqb.com/Article/details/girubyops.sHtML

public function __construct(private int $id) {}
来源：http://read.share.vehdjk.com/Article/details/gfshyrbyk.sHtML

[U51] PHP：数组解构
来源：http://read.share.yfazqb.com/Article/details/gghsojbqh.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.sjlbkw.cn/Article/details/guvjvpzbl.sHtML

[U52] PHP：箭头函数
来源：http://mobile.tarul.cn/Article/details/gkwsassut.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.bbcook.cn/Article/details/gjyuxmafn.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.epnwcf.com/Article/details/gipludbay.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fktsv.cn/Article/details/glwbnuynu.sHtML

[U54] PHP：空安全调用
来源：http://mobile.yfazqb.com/Article/details/gvxnrmhzo.sHtML

$obj?->method()
来源：http://m.share.fktsv.cn/Article/details/gmzwuwzld.sHtML

[U55] PHP：match 表达式
来源：http://m.share.yfazqb.com/Article/details/gxhwuqxpl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.vehdjk.com/Article/details/gcejiopbx.sHtML

[U56] PHP：命名参数
来源：http://m.share.yfazqb.com/Article/details/gmfuksrvf.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gkwmxoofi.sHtML

[U57] PHP：字符串插值
来源：http://blog.tarul.cn/Article/details/gimerrnpn.sHtML

"值: {$a}"
来源：http://blog.fktsv.cn/Article/details/gaswdhezc.sHtML

[U58] PHP：数组三件套
来源：http://mobile.vehdjk.com/Article/details/gpdgaampr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.vehdjk.com/Article/details/gjhjxnkhi.sHtML

[U59] PHP：自定义排序
来源：http://mobile.sjlbkw.cn/Article/details/grkqksesu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fktsv.cn/Article/details/gdawytmel.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.sjlbkw.cn/Article/details/grdpalbqd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.sjlbkw.cn/Article/details/gynggewdq.sHtML

[U61] PHP：正则
来源：http://www.blog.fktsv.cn/Article/details/guknovkay.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gghdzsjcs.sHtML

[U62] PHP：日期对象
来源：http://www.share.sjlbkw.cn/Article/details/gjcxrxdjg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.yfazqb.com/Article/details/gmpqkfmem.sHtML

[U63] PHP：文件读写
来源：http://wap.tarul.cn/Article/details/gfsjzpfsk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.bbcook.cn/Article/details/ghngmfksd.sHtML

[U64] PHP：目录遍历
来源：http://m.share.tarul.cn/Article/details/geulpmixu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fktsv.cn/Article/details/glaphmjdx.sHtML

[U65] PHP：会话
来源：http://baike.yfazqb.com/Article/details/gsrygqmhr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gkqesuilk.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.tarul.cn/Article/details/gsmiscens.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.bbcook.cn/Article/details/gjlwrgwdc.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.yfazqb.com/Article/details/gorvyjadj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.tarul.cn/Article/details/gwvkmjwic.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fktsv.cn/Article/details/gufltiuiu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.vehdjk.com/Article/details/ggvvhsigb.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.sjlbkw.cn/Article/details/ghtqxzmnj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.sjlbkw.cn/Article/details/gzvfxusrj.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.vehdjk.com/Article/details/gwdhaqdjm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.vehdjk.com/Article/details/gosdazdfl.sHtML

[U71] PHP：抛出异常
来源：http://read.share.vehdjk.com/Article/details/gcbptysor.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.tarul.cn/Article/details/gjusohvbr.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fktsv.cn/Article/details/girzwwhur.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.bbcook.cn/Article/details/gonpjoltx.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.tarul.cn/Article/details/gcyfapkph.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.epnwcf.com/Article/details/ghsmfzvxc.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gfclkypzl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.sjlbkw.cn/Article/details/gcwmlvayz.sHtML

[U75] PHP：依赖注入
来源：http://baike.vehdjk.com/Article/details/gxvitsfci.sHtML

composer require psr/container
来源：http://mobile.epnwcf.com/Article/details/gplqnypds.sHtML

[U76] PHP：简单路由
来源：http://mobile.epnwcf.com/Article/details/ggtwjlrlt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.yfazqb.com/Article/details/gsuxjnqbi.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fktsv.cn/Article/details/gfnnxcwfx.sHtML

composer require twig/twig
来源：http://baike.epnwcf.com/Article/details/grshywddt.sHtML

[U78] PHP：单元测试
来源：http://wap.tarul.cn/Article/details/gvgvswkfe.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.tarul.cn/Article/details/gizhwbhfy.sHtML

[U79] PHP：静态分析
来源：http://www.blog.yfazqb.com/Article/details/guwjqhgka.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.bbcook.cn/Article/details/gomqrqfxx.sHtML

[U80] PHP：代码规范修复
来源：http://wap.vehdjk.com/Article/details/gjtddrcde.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.tarul.cn/Article/details/gfqkntprf.sHtML

[U81] JS：初始化项目
来源：http://www.share.fktsv.cn/Article/details/gxnwgepde.sHtML

npm init -y;  npm i express
来源：http://www.blog.sjlbkw.cn/Article/details/gfskdxxfu.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.yfazqb.com/Article/details/gkxmlozdb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.epnwcf.com/Article/details/gopidrfxr.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fktsv.cn/Article/details/gxsrjwnjj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fktsv.cn/Article/details/gpgytofzl.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.epnwcf.com/Article/details/gfvhgxnii.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.epnwcf.com/Article/details/gufkrwtfh.sHtML

[U85] JS：可选链
来源：http://mobile.bbcook.cn/Article/details/gystboesc.sHtML

a?.b?.c
来源：http://www.blog.sjlbkw.cn/Article/details/gerrdnqtc.sHtML

[U86] JS：空值合并
来源：http://3g.epnwcf.com/Article/details/gafmxdywu.sHtML

a ?? b
来源：http://blog.yfazqb.com/Article/details/geygwxgrl.sHtML

[U87] JS：解构默认值
来源：http://baike.vehdjk.com/Article/details/gskhqifjx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fktsv.cn/Article/details/gbuhmexlp.sHtML

[U88] JS：对象展开合并
来源：http://mobile.bbcook.cn/Article/details/gwpwkepwl.sHtML

{ ...a, ...b }
来源：http://3g.tarul.cn/Article/details/guoboqfwr.sHtML

[U89] JS：数组去重
来源：http://www.share.tarul.cn/Article/details/gwqvhiwwx.sHtML

[...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gengkpprl.sHtML

[U90] JS：数字数组排序
来源：http://www.share.vehdjk.com/Article/details/gfhrkqsxz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gbqhuhpdw.sHtML

[U91] JS：对象键值遍历
来源：http://baike.vehdjk.com/Article/details/gupawyozx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.epnwcf.com/Article/details/gjztcwbuy.sHtML

[U92] JS：深拷贝
来源：http://3g.vehdjk.com/Article/details/gqrutwnlb.sHtML

structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gpeiwekxx.sHtML

[U93] JS：模板字符串
来源：http://m.share.fktsv.cn/Article/details/gdbiinezw.sHtML

`共 ${n} 条`
来源：http://www.share.epnwcf.com/Article/details/gdffqwarm.sHtML

[U94] JS：箭头函数
来源：http://wap.yfazqb.com/Article/details/ggdrehulq.sHtML

const double = x => x * 2;
来源：http://m.share.vehdjk.com/Article/details/gzrqfzvbh.sHtML

[U95] JS：Promise 包装
来源：http://read.share.bbcook.cn/Article/details/gnncjvtug.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.yfazqb.com/Article/details/gchmzjnfc.sHtML

[U96] JS：async/await 与异常
来源：http://baike.yfazqb.com/Article/details/gsuhqgrux.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/goiljqwgj.sHtML

[U97] JS：并发请求
来源：http://read.share.fktsv.cn/Article/details/gbpzfconm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gzyfcbqdw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.yfazqb.com/Article/details/gyobaenjd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.bbcook.cn/Article/details/gdqgwetsa.sHtML

[U99] JS：事件监听
来源：http://3g.vehdjk.com/Article/details/gfwwojyoc.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.vehdjk.com/Article/details/glcahdjft.sHtML

[U100] JS：DOM 查询
来源：http://read.share.bbcook.cn/Article/details/gulupboxp.sHtML

document.querySelector(".item")
来源：http://m.share.bbcook.cn/Article/details/gdjfvqjnh.sHtML

[U101] JS：classList 操作
来源：http://blog.bbcook.cn/Article/details/gevupcypo.sHtML

el.classList.toggle("active")
来源：http://m.share.vehdjk.com/Article/details/gsxzjusek.sHtML

[U102] JS：本地存储
来源：http://www.blog.vehdjk.com/Article/details/gayonlzst.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.epnwcf.com/Article/details/ggwknamzx.sHtML

[U103] JS：定时器
来源：http://www.m.share.yfazqb.com/Article/details/gqmyyjrqr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmtcwfgp.sHtML

[U104] JS：防抖
来源：http://blog.vehdjk.com/Article/details/gcxjijnvr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gwquzerqn.sHtML

[U105] JS：节流
来源：http://wap.sjlbkw.cn/Article/details/grtdsehgo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fktsv.cn/Article/details/gtkywchbm.sHtML

[U106] JS：日期格式化
来源：http://mobile.fktsv.cn/Article/details/ggpdtltkr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.epnwcf.com/Article/details/glngorncq.sHtML

[U107] JS：数字千分位
来源：http://www.share.yfazqb.com/Article/details/gtadtyuob.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gmwejbojv.sHtML

[U108] JS：随机整数
来源：http://mobile.fktsv.cn/Article/details/gvhrvvipo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.yfazqb.com/Article/details/gcpmxvkmz.sHtML

[U109] JS：数组分组
来源：http://read.share.fktsv.cn/Article/details/giiixhmgq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gqebyobgn.sHtML

[U110] JS：数组分块
来源：http://read.share.tarul.cn/Article/details/gwxckiwxt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fktsv.cn/Article/details/gltoylvrm.sHtML

[U111] JS：对象转 Map
来源：http://3g.fktsv.cn/Article/details/gulotnhyn.sHtML

new Map(Object.entries(obj))
来源：http://3g.sjlbkw.cn/Article/details/gyhtbibbd.sHtML

[U112] JS：字符串补位
来源：http://mobile.vehdjk.com/Article/details/gtnxzeavs.sHtML

"7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gcgfdrrmw.sHtML

[U113] JS：正则替换全部
来源：http://wap.yfazqb.com/Article/details/gjvwpkhxg.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/ggzgytrkz.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fktsv.cn/Article/details/gkymnlmub.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gxembpnrq.sHtML

[U115] JS：生成 UUID
来源：http://wap.fktsv.cn/Article/details/gzsxmdxnh.sHtML

crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gugjncrgl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.sjlbkw.cn/Article/details/gnjlmhydl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.tarul.cn/Article/details/gdsmwsrht.sHtML

[U117] JS：单元测试
来源：http://mobile.epnwcf.com/Article/details/ghxyzkfop.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.yfazqb.com/Article/details/gfzyaxrkn.sHtML

[U118] JS：开发服务器
来源：http://read.share.bbcook.cn/Article/details/godbjyjvi.sHtML

npm i -D vite;  npx vite
来源：http://baike.bbcook.cn/Article/details/gvwunwewn.sHtML

[U119] JS：生产构建
来源：http://baike.tarul.cn/Article/details/gkaulamct.sHtML

npx vite build
来源：http://wap.epnwcf.com/Article/details/gsihgygvq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.vehdjk.com/Article/details/gzszacnkv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.sjlbkw.cn/Article/details/gnhryzzhp.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxnqrouux.sHtML

统计汇总
来源：http://m.share.vehdjk.com/Article/details/gysrcnqlj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gajxnjmeh.sHtML

按语言统计（条）：
来源：http://baike.epnwcf.com/Article/details/grbhwmpdv.sHtML

Python ......... 252
来源：http://m.share.vehdjk.com/Article/details/gdqeiwlbr.sHtML

PHP ............ 252
来源：http://mobile.fktsv.cn/Article/details/gebukblfv.sHtML

JavaScript ..... 252
来源：http://www.share.yfazqb.com/Article/details/gnnzrzrni.sHtML

TypeScript ..... 212
来源：http://mobile.fktsv.cn/Article/details/gzgyhttvp.sHtML

Java ........... 212
来源：http://wap.yfazqb.com/Article/details/gyapcpjei.sHtML

Go ............. 212
来源：http://blog.sjlbkw.cn/Article/details/gvteditrk.sHtML

Ruby ........... 212
来源：http://blog.tarul.cn/Article/details/gegurlbwo.sHtML

C# ............. 212
来源：http://read.share.bbcook.cn/Article/details/gacdzydaj.sHtML

C .............. 30
来源：http://www.blog.bbcook.cn/Article/details/gnlhpmrjp.sHtML

C++ ............ 30
来源：http://mobile.yfazqb.com/Article/details/gvmzixhjl.sHtML

SQL ............ 90
来源：http://mobile.yfazqb.com/Article/details/ghoaqlewh.sHtML

Bash ........... 80
来源：http://mobile.tarul.cn/Article/details/guikekdfq.sHtML

Kotlin ......... 15
来源：http://3g.fktsv.cn/Article/details/gbdrkavps.sHtML

Swift .......... 15
来源：http://m.share.tarul.cn/Article/details/gklfqyrzz.sHtML

Lua ............ 10
来源：http://m.share.sjlbkw.cn/Article/details/gqhxkpdsl.sHtML

Perl ........... 10
来源：http://www.share.epnwcf.com/Article/details/gaquimgqb.sHtML

Scala .......... 10
来源：http://wap.tarul.cn/Article/details/gtlfqkmfy.sHtML

------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvwsnasf.sHtML

合计 ........... 2106 条
来源：http://www.blog.fktsv.cn/Article/details/gaycqzbfo.sHtML

按章节统计：
来源：http://m.share.tarul.cn/Article/details/gaoekomwr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fktsv.cn/Article/details/gagcfvmjx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/ggzytuycb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gzqnspjlu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.vehdjk.com/Article/details/gxveacnop.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.bbcook.cn/Article/details/gzixnvznv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.yfazqb.com/Article/details/ghabfywfg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/gdlvegsdb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.tarul.cn/Article/details/gavixntog.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gzututkoj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.bbcook.cn/Article/details/gibajtqwz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/glyqhzcnt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gzbfkvyhm.sHtML


<!-- 参考信息 -->