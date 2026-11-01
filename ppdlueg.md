代发 wailian999

val a = 1;  var b = 2
来源：http://3g.epnwcf.com/Article/details/gvxpgzqoy.sHtML

[T53] Scala：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/ghsttlwqg.sHtML

s"值: $b"
来源：http://wap.fktsv.cn/Article/details/gqtfusypb.sHtML

[T54] Scala：集合映射
来源：http://read.share.tarul.cn/Article/details/gkktnuicd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtunqtda.sHtML

[T55] Scala：集合过滤
来源：http://mobile.epnwcf.com/Article/details/gyekfxggo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fktsv.cn/Article/details/gslmnyyrv.sHtML

[T56] Scala：样例类
来源：http://baike.tarul.cn/Article/details/gpqdelqwv.sHtML

case class User(name: String, age: Int)
来源：http://www.share.epnwcf.com/Article/details/gpgxutpht.sHtML

[T57] Scala：模式匹配
来源：http://blog.vehdjk.com/Article/details/gkchdrqww.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.vehdjk.com/Article/details/giwieixzi.sHtML

[T58] Scala：函数定义
来源：http://www.share.tarul.cn/Article/details/glcblpihp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.vehdjk.com/Article/details/grlcvkjvv.sHtML

[T59] Scala：循环
来源：http://wap.bbcook.cn/Article/details/gukbebvlt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gdlmlzlnj.sHtML

[T60] Scala：折叠
来源：http://3g.fktsv.cn/Article/details/giqunwknq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.vehdjk.com/Article/details/gpbhgaaag.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gamaccovv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/gyxujuvsq.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/geuplovec.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.tarul.cn/Article/details/gybbzhprc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.tarul.cn/Article/details/gqxvawumt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.yfazqb.com/Article/details/glnmwmdwq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/grwclxjur.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.epnwcf.com/Article/details/gzbvekwjo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.bbcook.cn/Article/details/ghdthziby.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.tarul.cn/Article/details/gucnbyrsn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.tarul.cn/Article/details/gnbtdgoqh.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.tarul.cn/Article/details/gpxvwusct.sHtML

list(dict.fromkeys(arr))
来源：http://3g.vehdjk.com/Article/details/gqbplixdk.sHtML

[U06] Py：合并两个字典
来源：http://3g.bbcook.cn/Article/details/gfvapjtfg.sHtML

{**a, **b}
来源：http://m.share.sjlbkw.cn/Article/details/gngzelyqu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fktsv.cn/Article/details/gkgnrlggu.sHtML

{v: k for k, v in d.items()}
来源：http://wap.sjlbkw.cn/Article/details/golxdetmm.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gcvynjnnm.sHtML

[y for x in nested for y in x]
来源：http://mobile.tarul.cn/Article/details/gwkahtpsp.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.vehdjk.com/Article/details/ghslsyygo.sHtML

max(d, key=d.get)
来源：http://m.share.sjlbkw.cn/Article/details/gouqjdkgm.sHtML

[U10] Py：按值排序字典
来源：http://blog.fktsv.cn/Article/details/ggtsxddvd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.tarul.cn/Article/details/gnvqmehkb.sHtML

[U11] Py：生成器表达式
来源：http://blog.vehdjk.com/Article/details/gpftqcoib.sHtML

(x * 2 for x in arr)
来源：http://www.share.tarul.cn/Article/details/ghqpxygrl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.sjlbkw.cn/Article/details/gpunpfibs.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fktsv.cn/Article/details/gbxorsszu.sHtML

[U13] Py：固定长度队列
来源：http://blog.yfazqb.com/Article/details/govyhmbfd.sHtML

deque(maxlen=10)
来源：http://www.blog.bbcook.cn/Article/details/gsqhopvep.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fktsv.cn/Article/details/glwwupehj.sHtML

defaultdict(list)
来源：http://blog.vehdjk.com/Article/details/gbuwcttol.sHtML

[U15] Py：高精度计时
来源：http://read.share.tarul.cn/Article/details/gnupkkdwk.sHtML

t = time.perf_counter()
来源：http://blog.bbcook.cn/Article/details/gyfknzyea.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.tarul.cn/Article/details/gbdtjmphu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.tarul.cn/Article/details/gfunlikvw.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fktsv.cn/Article/details/ghxzjpgvq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.tarul.cn/Article/details/gzofpbniy.sHtML

[U18] Py：预编译正则
来源：http://blog.fktsv.cn/Article/details/gimvyskxm.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpemdmgi.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.sjlbkw.cn/Article/details/gesbsyacd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fktsv.cn/Article/details/gpewgqwbv.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/gmtsrjzew.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.epnwcf.com/Article/details/ghmbhnike.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.vehdjk.com/Article/details/gcmiyvfsi.sHtML

@contextlib.contextmanager
来源：http://read.share.tarul.cn/Article/details/grscgzrqx.sHtML

[U22] Py：矩阵转置
来源：http://blog.yfazqb.com/Article/details/gdlishbhh.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/gjhuamxmv.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.yfazqb.com/Article/details/gpmghwmes.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.vehdjk.com/Article/details/grgwrbcal.sHtML

[U24] Py：路径操作
来源：http://www.m.share.tarul.cn/Article/details/gfoaxtdmz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.yfazqb.com/Article/details/ghrmfbgwc.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fktsv.cn/Article/details/gjydxixpm.sHtML

csv.DictReader(f)
来源：http://www.blog.bbcook.cn/Article/details/gzasurmsb.sHtML

[U26] Py：并发下载
来源：http://m.share.yfazqb.com/Article/details/gywrccfri.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.bbcook.cn/Article/details/gledsxxqn.sHtML

[U27] Py：异步 HTTP
来源：http://blog.sjlbkw.cn/Article/details/gmhuvzyfw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.yfazqb.com/Article/details/gttocbhun.sHtML

[U28] Py：类型别名
来源：http://m.share.vehdjk.com/Article/details/gnopkqkot.sHtML

UserId = int
来源：http://read.share.vehdjk.com/Article/details/gvbdrgxcg.sHtML

[U29] Py：属性校验
来源：http://wap.sjlbkw.cn/Article/details/gooindkgi.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fktsv.cn/Article/details/gtvysdggx.sHtML

[U30] Py：数据类
来源：http://m.share.vehdjk.com/Article/details/gjhmrzchi.sHtML

@dataclass(slots=True)
来源：http://wap.sjlbkw.cn/Article/details/gqxlpbotr.sHtML

[U31] Py：单测
来源：http://m.share.tarul.cn/Article/details/gylidxmlo.sHtML

python -m pytest -q
来源：http://www.share.epnwcf.com/Article/details/grnrntqps.sHtML

[U32] Py：代码格式化
来源：http://wap.bbcook.cn/Article/details/gjhsxhuew.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fktsv.cn/Article/details/gusqqryct.sHtML

[U33] Py：打包发布
来源：http://www.m.share.vehdjk.com/Article/details/gnkvtprmn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.epnwcf.com/Article/details/gqxuywwrg.sHtML

[U34] Py：判断编码
来源：http://www.share.bbcook.cn/Article/details/gwyxepkss.sHtML

chardet.detect(raw)
来源：http://www.share.bbcook.cn/Article/details/gxbdmjbsq.sHtML

[U35] Py：发送邮件
来源：http://www.share.fktsv.cn/Article/details/gbpaemvwq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.yfazqb.com/Article/details/gksmfqqwd.sHtML

[U36] Py：定时任务
来源：http://baike.epnwcf.com/Article/details/gctguuncg.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.vehdjk.com/Article/details/gzwttjzrt.sHtML

[U37] Py：读写 Excel
来源：http://m.share.sjlbkw.cn/Article/details/gbaiibpwr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.sjlbkw.cn/Article/details/gkcmsjflx.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.vehdjk.com/Article/details/gfvoiwpyl.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.epnwcf.com/Article/details/glfmrinei.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.epnwcf.com/Article/details/gxwixywgt.sHtML

sys.stdout.isatty()
来源：http://wap.epnwcf.com/Article/details/gzgxncyiv.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.yfazqb.com/Article/details/gonkxyjdj.sHtML

print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gwzzsonla.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.bbcook.cn/Article/details/gfmmhrljg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.bbcook.cn/Article/details/grzziwlsg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.yfazqb.com/Article/details/gnigcxkcm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fktsv.cn/Article/details/gbvdtzkzd.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.yfazqb.com/Article/details/ghysbljhu.sHtML

namespace App\Http;
来源：http://mobile.bbcook.cn/Article/details/gwvpynxko.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.vehdjk.com/Article/details/gfwsltagh.sHtML

declare(strict_types=1);
来源：http://m.share.fktsv.cn/Article/details/gqiswjjar.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.vehdjk.com/Article/details/gntinhvjp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gvzkqvwks.sHtML

[U46] PHP：可空类型
来源：http://www.share.bbcook.cn/Article/details/gpaiybdma.sHtML

?string $name = null
来源：http://www.m.share.sjlbkw.cn/Article/details/grbaucsdr.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.yfazqb.com/Article/details/gdduukcvh.sHtML

int|string $id
来源：http://baike.yfazqb.com/Article/details/gnojyytxn.sHtML

[U48] PHP：纯枚举
来源：http://m.share.yfazqb.com/Article/details/goijaswfy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.sjlbkw.cn/Article/details/gzxjisafd.sHtML

[U49] PHP：只读属性
来源：http://3g.vehdjk.com/Article/details/gmnjavcbl.sHtML

public readonly string $name
来源：http://3g.bbcook.cn/Article/details/gelorozeo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.epnwcf.com/Article/details/gubplsxlj.sHtML

public function __construct(private int $id) {}
来源：http://www.share.tarul.cn/Article/details/glfzkpmtx.sHtML

[U51] PHP：数组解构
来源：http://baike.vehdjk.com/Article/details/gqafmvhlj.sHtML

[$a, $b] = $arr;
来源：http://read.share.epnwcf.com/Article/details/guygpmxkv.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/guapkgnso.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.tarul.cn/Article/details/gzlqjmdde.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.tarul.cn/Article/details/gidwgjiil.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.bbcook.cn/Article/details/gvmeawzkm.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fktsv.cn/Article/details/grgfbmkvy.sHtML

$obj?->method()
来源：http://m.share.epnwcf.com/Article/details/gyrejgecz.sHtML

[U55] PHP：match 表达式
来源：http://www.share.yfazqb.com/Article/details/gjksmqnyj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.sjlbkw.cn/Article/details/ghcuxxbfu.sHtML

[U56] PHP：命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gxrvqehet.sHtML

f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gyolsjngz.sHtML

[U57] PHP：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gkfvkswje.sHtML

"值: {$a}"
来源：http://mobile.epnwcf.com/Article/details/gvitczpzy.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.sjlbkw.cn/Article/details/ggeonnvjw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.tarul.cn/Article/details/gjghfbnay.sHtML

[U59] PHP：自定义排序
来源：http://mobile.bbcook.cn/Article/details/gngfzubpu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/glkaffctk.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fktsv.cn/Article/details/gsrkeldub.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.epnwcf.com/Article/details/ggetaqvye.sHtML

[U61] PHP：正则
来源：http://m.share.epnwcf.com/Article/details/guqaqqhuc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gekaiilkx.sHtML

[U62] PHP：日期对象
来源：http://www.blog.bbcook.cn/Article/details/gtfgcevgm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.epnwcf.com/Article/details/gsvzlltmu.sHtML

[U63] PHP：文件读写
来源：http://m.share.epnwcf.com/Article/details/gejcuspgx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.epnwcf.com/Article/details/gxzopnert.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fktsv.cn/Article/details/guwspjzhx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.tarul.cn/Article/details/gopmzowwk.sHtML

[U65] PHP：会话
来源：http://wap.yfazqb.com/Article/details/gpkjrpwot.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.epnwcf.com/Article/details/grsdtzzqx.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.epnwcf.com/Article/details/gkmqzsudk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gmcrukwat.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.epnwcf.com/Article/details/glqbxtupy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.bbcook.cn/Article/details/gdlhzieye.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.yfazqb.com/Article/details/gkborkwzo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.tarul.cn/Article/details/gfinrbuyn.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fktsv.cn/Article/details/gmfpjrvra.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.epnwcf.com/Article/details/gwjvpiqwv.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fktsv.cn/Article/details/greddedht.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fktsv.cn/Article/details/gqxfwoqke.sHtML

[U71] PHP：抛出异常
来源：http://mobile.yfazqb.com/Article/details/gzfepwcdn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.yfazqb.com/Article/details/gmpewnoke.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.epnwcf.com/Article/details/ghczrcnpm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.epnwcf.com/Article/details/gmbadluks.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.bbcook.cn/Article/details/gzfdvefbi.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.yfazqb.com/Article/details/gzsecbzuv.sHtML

[U74] PHP：读取环境变量
来源：http://3g.epnwcf.com/Article/details/gwraortdn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.sjlbkw.cn/Article/details/grvzdarng.sHtML

[U75] PHP：依赖注入
来源：http://3g.tarul.cn/Article/details/gmlamjjkr.sHtML

composer require psr/container
来源：http://wap.tarul.cn/Article/details/gxnpftmwa.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/gfdmkozvy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.tarul.cn/Article/details/gbhafxhze.sHtML

[U77] PHP：模板渲染
来源：http://www.share.epnwcf.com/Article/details/gscpqnqpa.sHtML

composer require twig/twig
来源：http://mobile.tarul.cn/Article/details/gwvihlmrk.sHtML

[U78] PHP：单元测试
来源：http://wap.yfazqb.com/Article/details/gmhwqswfg.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.sjlbkw.cn/Article/details/glrgknomf.sHtML

[U79] PHP：静态分析
来源：http://m.share.fktsv.cn/Article/details/gxvfxfigx.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.epnwcf.com/Article/details/grcszoehw.sHtML

[U80] PHP：代码规范修复
来源：http://baike.yfazqb.com/Article/details/gocpuwlad.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.vehdjk.com/Article/details/gsajifpzc.sHtML

[U81] JS：初始化项目
来源：http://baike.tarul.cn/Article/details/gjzzuovkf.sHtML

npm init -y;  npm i express
来源：http://read.share.vehdjk.com/Article/details/gngyggfof.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.vehdjk.com/Article/details/gocujelyn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.tarul.cn/Article/details/gmllgtarz.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fktsv.cn/Article/details/ggihzcdke.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.tarul.cn/Article/details/gminqmbuo.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.yfazqb.com/Article/details/gqzozgcet.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.bbcook.cn/Article/details/gtogsilek.sHtML

[U85] JS：可选链
来源：http://read.share.vehdjk.com/Article/details/godmwxdvq.sHtML

a?.b?.c
来源：http://wap.yfazqb.com/Article/details/ggiltxmfn.sHtML

[U86] JS：空值合并
来源：http://blog.epnwcf.com/Article/details/gigihxwxn.sHtML

a ?? b
来源：http://read.share.tarul.cn/Article/details/gwnjfbgna.sHtML

[U87] JS：解构默认值
来源：http://wap.sjlbkw.cn/Article/details/gfsopvsii.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.bbcook.cn/Article/details/gxvvuupzz.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.bbcook.cn/Article/details/gplnblmct.sHtML

{ ...a, ...b }
来源：http://wap.yfazqb.com/Article/details/gevblmpec.sHtML

[U89] JS：数组去重
来源：http://read.share.sjlbkw.cn/Article/details/gypareisk.sHtML

[...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gyztjzeam.sHtML

[U90] JS：数字数组排序
来源：http://baike.fktsv.cn/Article/details/gifzugvaj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/grsyakqqe.sHtML

[U91] JS：对象键值遍历
来源：http://wap.vehdjk.com/Article/details/gmyyeccnc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.yfazqb.com/Article/details/ghukxafyn.sHtML

[U92] JS：深拷贝
来源：http://www.share.bbcook.cn/Article/details/grginjcjq.sHtML

structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gusrkzixy.sHtML

[U93] JS：模板字符串
来源：http://3g.tarul.cn/Article/details/gosmedcbg.sHtML

`共 ${n} 条`
来源：http://3g.sjlbkw.cn/Article/details/gtvkoljuv.sHtML

[U94] JS：箭头函数
来源：http://m.share.epnwcf.com/Article/details/gzirncbxt.sHtML

const double = x => x * 2;
来源：http://blog.tarul.cn/Article/details/gcrjiqzug.sHtML

[U95] JS：Promise 包装
来源：http://3g.tarul.cn/Article/details/ggyxqbrmb.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.bbcook.cn/Article/details/gmgonsziv.sHtML

[U96] JS：async/await 与异常
来源：http://wap.sjlbkw.cn/Article/details/gpftotyme.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gcfqfvgjv.sHtML

[U97] JS：并发请求
来源：http://wap.yfazqb.com/Article/details/gjyrxwdur.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/grmqupihu.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.tarul.cn/Article/details/gmsxhcxmo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.tarul.cn/Article/details/grtspainw.sHtML

[U99] JS：事件监听
来源：http://www.blog.yfazqb.com/Article/details/gcbubmbhh.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fktsv.cn/Article/details/gpgvpzmlp.sHtML

[U100] JS：DOM 查询
来源：http://baike.bbcook.cn/Article/details/ggcekvgnw.sHtML

document.querySelector(".item")
来源：http://blog.epnwcf.com/Article/details/ggxcxjitv.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.epnwcf.com/Article/details/gtytnxmuv.sHtML

el.classList.toggle("active")
来源：http://www.share.epnwcf.com/Article/details/geldxmdxt.sHtML

[U102] JS：本地存储
来源：http://3g.tarul.cn/Article/details/gxihnlydv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.vehdjk.com/Article/details/gojgpapvi.sHtML

[U103] JS：定时器
来源：http://m.share.bbcook.cn/Article/details/gjbnefrta.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.vehdjk.com/Article/details/gctybjrye.sHtML

[U104] JS：防抖
来源：http://wap.bbcook.cn/Article/details/grhmhhevv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gndqqivan.sHtML

[U105] JS：节流
来源：http://baike.yfazqb.com/Article/details/gyexiqwgw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.yfazqb.com/Article/details/gpfnmgexg.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gkgifymue.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.epnwcf.com/Article/details/gmhdicgnk.sHtML

[U107] JS：数字千分位
来源：http://wap.epnwcf.com/Article/details/gideaxqmu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gevqytkqn.sHtML

[U108] JS：随机整数
来源：http://blog.bbcook.cn/Article/details/ghrldtbxw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fktsv.cn/Article/details/gflzmhefb.sHtML

[U109] JS：数组分组
来源：http://wap.sjlbkw.cn/Article/details/gyntrlrhd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gwtxloonw.sHtML

[U110] JS：数组分块
来源：http://blog.fktsv.cn/Article/details/gjduonpvm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.epnwcf.com/Article/details/gnvfyyuww.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fktsv.cn/Article/details/gbsnhilos.sHtML

new Map(Object.entries(obj))
来源：http://wap.vehdjk.com/Article/details/ggaozqnwn.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.tarul.cn/Article/details/goemzupjy.sHtML

"7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gsuroksun.sHtML

[U113] JS：正则替换全部
来源：http://3g.fktsv.cn/Article/details/guznfloty.sHtML

s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gutfoimgc.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.epnwcf.com/Article/details/gyuyullcs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gqkigocbz.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gqfnabxvy.sHtML

crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gddlkttoo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.sjlbkw.cn/Article/details/giweaenpl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.vehdjk.com/Article/details/gozaczsqb.sHtML

[U117] JS：单元测试
来源：http://www.m.share.epnwcf.com/Article/details/gdnrksueb.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.yfazqb.com/Article/details/grewaaann.sHtML

[U118] JS：开发服务器
来源：http://3g.vehdjk.com/Article/details/gavhwmcoh.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fktsv.cn/Article/details/gewmynpze.sHtML

[U119] JS：生产构建
来源：http://baike.bbcook.cn/Article/details/gyzcdcmhe.sHtML

npx vite build
来源：http://3g.epnwcf.com/Article/details/geexvswsl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.sjlbkw.cn/Article/details/gfrfkoyms.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.tarul.cn/Article/details/gazslnifp.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gilseimts.sHtML

统计汇总
来源：http://baike.sjlbkw.cn/Article/details/gbuxiwxew.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbdqdmqjq.sHtML

按语言统计（条）：
来源：http://read.share.yfazqb.com/Article/details/gfrwdxdzs.sHtML

Python ......... 252
来源：http://www.share.epnwcf.com/Article/details/gdbvxzqkg.sHtML

PHP ............ 252
来源：http://wap.tarul.cn/Article/details/ggaaxaohh.sHtML

JavaScript ..... 252
来源：http://m.share.yfazqb.com/Article/details/gvdpwnynz.sHtML

TypeScript ..... 212
来源：http://read.share.epnwcf.com/Article/details/glordqvfp.sHtML

Java ........... 212
来源：http://3g.vehdjk.com/Article/details/gacwesfcg.sHtML

Go ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/ghlgwjhav.sHtML

Ruby ........... 212
来源：http://m.share.epnwcf.com/Article/details/gzrecigsr.sHtML

C# ............. 212
来源：http://m.share.epnwcf.com/Article/details/gpqntwpvb.sHtML

C .............. 30
来源：http://baike.epnwcf.com/Article/details/gttlhqaiy.sHtML

C++ ............ 30
来源：http://blog.sjlbkw.cn/Article/details/geevgcgpq.sHtML

SQL ............ 90
来源：http://read.share.epnwcf.com/Article/details/gibdoaaqa.sHtML

Bash ........... 80
来源：http://baike.fktsv.cn/Article/details/gqbothrzd.sHtML

Kotlin ......... 15
来源：http://baike.tarul.cn/Article/details/gfwgsazkz.sHtML

Swift .......... 15
来源：http://m.share.bbcook.cn/Article/details/gvzyrdmtu.sHtML

Lua ............ 10
来源：http://wap.vehdjk.com/Article/details/gdfwgwycl.sHtML

Perl ........... 10
来源：http://www.m.share.epnwcf.com/Article/details/gpuhyvnzj.sHtML

Scala .......... 10
来源：http://3g.vehdjk.com/Article/details/gztcxwsft.sHtML

------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gxxtqppqe.sHtML

合计 ........... 2106 条
来源：http://baike.bbcook.cn/Article/details/geklqohsl.sHtML

按章节统计：
来源：http://baike.tarul.cn/Article/details/glozluefa.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/glahrlgkh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/gpjjsmnxh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gkarjumme.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.yfazqb.com/Article/details/gxcjqsmrl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhbpqrnr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.vehdjk.com/Article/details/gnpgoimrx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/ghajawqxp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/gtjcjtawg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/ggwzpjjmp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.vehdjk.com/Article/details/gswjifxhu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gombfuvfb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gizabjrdf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gzqitlzon.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/gazzleuaz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fktsv.cn/Article/details/gaomyepia.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gkixvfmfc.sHtML


<!-- 参考信息 -->