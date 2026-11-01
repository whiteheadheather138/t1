代发 wailian999

val a = 1;  var b = 2
来源：http://www.blog.fktsv.cn/Article/details/gjanhodqv.sHtML

[T53] Scala：字符串插值
来源：http://baike.epnwcf.com/Article/details/gktglbgdo.sHtML

s"值: $b"
来源：http://mobile.epnwcf.com/Article/details/gkwxfcbho.sHtML

[T54] Scala：集合映射
来源：http://www.share.bbcook.cn/Article/details/gxbjrfrip.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fktsv.cn/Article/details/gzumpyqmi.sHtML

[T55] Scala：集合过滤
来源：http://mobile.vehdjk.com/Article/details/glygkjpsr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fktsv.cn/Article/details/gtvhlzzbt.sHtML

[T56] Scala：样例类
来源：http://m.share.epnwcf.com/Article/details/gnpswchtt.sHtML

case class User(name: String, age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/geblfvjll.sHtML

[T57] Scala：模式匹配
来源：http://blog.vehdjk.com/Article/details/gekgeyytk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.tarul.cn/Article/details/gvltnmrqk.sHtML

[T58] Scala：函数定义
来源：http://wap.vehdjk.com/Article/details/gcwldgbey.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fktsv.cn/Article/details/giblwzvme.sHtML

[T59] Scala：循环
来源：http://blog.bbcook.cn/Article/details/gcpjhxmli.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gmcqcbumd.sHtML

[T60] Scala：折叠
来源：http://mobile.fktsv.cn/Article/details/gefjyisux.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.vehdjk.com/Article/details/gjoklssiq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbvdafxkd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gzebagpki.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gtsysopmi.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.epnwcf.com/Article/details/gjvgejrdr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.yfazqb.com/Article/details/gfuwbmedx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.tarul.cn/Article/details/gugkveqxx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.yfazqb.com/Article/details/ghhygojjc.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.sjlbkw.cn/Article/details/gmwwogtrk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.bbcook.cn/Article/details/gbuqcwhsl.sHtML

[U04] Py：变量调试打印
来源：http://blog.vehdjk.com/Article/details/geveyujgi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.bbcook.cn/Article/details/guygyvown.sHtML

[U05] Py：列表去重且保序
来源：http://3g.bbcook.cn/Article/details/gtmndnqej.sHtML

list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/goqwhkdeo.sHtML

[U06] Py：合并两个字典
来源：http://baike.epnwcf.com/Article/details/gmtwyybyd.sHtML

{**a, **b}
来源：http://www.m.share.tarul.cn/Article/details/gujjiqtuy.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.epnwcf.com/Article/details/gmgbcmyqw.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fktsv.cn/Article/details/gcxyknpum.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gionbgzik.sHtML

[y for x in nested for y in x]
来源：http://www.blog.vehdjk.com/Article/details/gduttcmiz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.epnwcf.com/Article/details/gqbtgvrcv.sHtML

max(d, key=d.get)
来源：http://read.share.tarul.cn/Article/details/gwhuqaqxb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.vehdjk.com/Article/details/gckllxcaw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.vehdjk.com/Article/details/gkffhxolx.sHtML

[U11] Py：生成器表达式
来源：http://baike.vehdjk.com/Article/details/gzaluyzlq.sHtML

(x * 2 for x in arr)
来源：http://blog.bbcook.cn/Article/details/gycgcbvic.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.vehdjk.com/Article/details/gsjoozdwy.sHtML

Counter(arr).most_common(3)
来源：http://wap.bbcook.cn/Article/details/gyjuulszz.sHtML

[U13] Py：固定长度队列
来源：http://mobile.vehdjk.com/Article/details/gbycnvbya.sHtML

deque(maxlen=10)
来源：http://blog.tarul.cn/Article/details/gshjtppew.sHtML

[U14] Py：分组收集到列表
来源：http://baike.sjlbkw.cn/Article/details/glyukmjaa.sHtML

defaultdict(list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyqgqxtw.sHtML

[U15] Py：高精度计时
来源：http://read.share.bbcook.cn/Article/details/gujyqphmi.sHtML

t = time.perf_counter()
来源：http://3g.bbcook.cn/Article/details/gfilcuxzu.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.yfazqb.com/Article/details/gzxfhsrgy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fktsv.cn/Article/details/goqgdiiif.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fktsv.cn/Article/details/glvkmdduk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.tarul.cn/Article/details/gtvtgvvhk.sHtML

[U18] Py：预编译正则
来源：http://baike.vehdjk.com/Article/details/gjlxsqsuz.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gutueuvwy.sHtML

[U19] Py：正则替换带回调
来源：http://3g.bbcook.cn/Article/details/gfazaysmj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.epnwcf.com/Article/details/geiwpdmmu.sHtML

[U20] Py：缓存函数结果
来源：http://3g.tarul.cn/Article/details/gwuzhmume.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.epnwcf.com/Article/details/ghfjpnxfr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.bbcook.cn/Article/details/gkqjleedq.sHtML

@contextlib.contextmanager
来源：http://www.share.fktsv.cn/Article/details/gqlmcdulj.sHtML

[U22] Py：矩阵转置
来源：http://m.share.epnwcf.com/Article/details/gcbzbtsvd.sHtML

list(zip(*m))
来源：http://www.share.tarul.cn/Article/details/gykkqkhjw.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.bbcook.cn/Article/details/guymgduvl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fktsv.cn/Article/details/gfwjcygri.sHtML

[U24] Py：路径操作
来源：http://3g.bbcook.cn/Article/details/gxblxlqgl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gjupdnbjz.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.vehdjk.com/Article/details/glcybxaev.sHtML

csv.DictReader(f)
来源：http://www.m.share.bbcook.cn/Article/details/glladrbsp.sHtML

[U26] Py：并发下载
来源：http://www.share.yfazqb.com/Article/details/gutfkypdo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.vehdjk.com/Article/details/gxobyuyom.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.sjlbkw.cn/Article/details/ggxouyrvs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.tarul.cn/Article/details/gqjvildlf.sHtML

[U28] Py：类型别名
来源：http://www.blog.epnwcf.com/Article/details/gykarunwv.sHtML

UserId = int
来源：http://m.share.fktsv.cn/Article/details/guuvubvig.sHtML

[U29] Py：属性校验
来源：http://read.share.tarul.cn/Article/details/gjpbmncrl.sHtML

@property 与 @x.setter 配合
来源：http://m.share.vehdjk.com/Article/details/gnluvmttf.sHtML

[U30] Py：数据类
来源：http://www.share.bbcook.cn/Article/details/gmxoedkdr.sHtML

@dataclass(slots=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gnxuijhpc.sHtML

[U31] Py：单测
来源：http://baike.yfazqb.com/Article/details/ggbcauwco.sHtML

python -m pytest -q
来源：http://mobile.epnwcf.com/Article/details/gsahtuihy.sHtML

[U32] Py：代码格式化
来源：http://www.blog.vehdjk.com/Article/details/gxgvnbrrl.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.bbcook.cn/Article/details/gizgnbojm.sHtML

[U33] Py：打包发布
来源：http://read.share.fktsv.cn/Article/details/gvepdjmzw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fktsv.cn/Article/details/gybcujlqu.sHtML

[U34] Py：判断编码
来源：http://www.blog.fktsv.cn/Article/details/gnhuojyxk.sHtML

chardet.detect(raw)
来源：http://baike.bbcook.cn/Article/details/goblqdtip.sHtML

[U35] Py：发送邮件
来源：http://www.blog.yfazqb.com/Article/details/gvaueifjg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.vehdjk.com/Article/details/grgrwfbwz.sHtML

[U36] Py：定时任务
来源：http://read.share.yfazqb.com/Article/details/gljqxkxjs.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.bbcook.cn/Article/details/gjigvvfpo.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fktsv.cn/Article/details/glhvzqcya.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.sjlbkw.cn/Article/details/guyhzftnr.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.sjlbkw.cn/Article/details/gvoaoykry.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fktsv.cn/Article/details/gaqlucprv.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.bbcook.cn/Article/details/gzfgwfile.sHtML

sys.stdout.isatty()
来源：http://m.share.yfazqb.com/Article/details/gzdevrbff.sHtML

[U40] Py：打印到标准错误
来源：http://wap.tarul.cn/Article/details/gpmcobmuh.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/gootkjjhc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.epnwcf.com/Article/details/gkisdfiko.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.tarul.cn/Article/details/ghpkvcjvl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.tarul.cn/Article/details/glptvrvpp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.bbcook.cn/Article/details/gdpokzzcw.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.bbcook.cn/Article/details/gabkmmqkz.sHtML

namespace App\Http;
来源：http://read.share.fktsv.cn/Article/details/gjazueifh.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.vehdjk.com/Article/details/gnrmlsvpv.sHtML

declare(strict_types=1);
来源：http://www.m.share.yfazqb.com/Article/details/gtwwmtesc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.yfazqb.com/Article/details/gmewpopsf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/guwmyvswx.sHtML

[U46] PHP：可空类型
来源：http://read.share.fktsv.cn/Article/details/gtkipxumi.sHtML

?string $name = null
来源：http://mobile.epnwcf.com/Article/details/gybjxvluc.sHtML

[U47] PHP：联合类型
来源：http://www.share.vehdjk.com/Article/details/gkhjpliah.sHtML

int|string $id
来源：http://read.share.sjlbkw.cn/Article/details/gxtiowabp.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxpmbhxg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fktsv.cn/Article/details/gucvuhqqq.sHtML

[U49] PHP：只读属性
来源：http://blog.epnwcf.com/Article/details/gvyctwxnq.sHtML

public readonly string $name
来源：http://www.share.yfazqb.com/Article/details/gdtjkneiy.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.bbcook.cn/Article/details/gxdlwyisa.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fktsv.cn/Article/details/gsrdpmxem.sHtML

[U51] PHP：数组解构
来源：http://www.share.epnwcf.com/Article/details/gflrrsqkd.sHtML

[$a, $b] = $arr;
来源：http://baike.tarul.cn/Article/details/gauzoqcgr.sHtML

[U52] PHP：箭头函数
来源：http://www.share.bbcook.cn/Article/details/gucjllota.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/gmgflcprj.sHtML

[U53] PHP：空合并运算符
来源：http://blog.tarul.cn/Article/details/gnutslayd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.yfazqb.com/Article/details/gaxmkhadc.sHtML

[U54] PHP：空安全调用
来源：http://wap.yfazqb.com/Article/details/gdtuhwahq.sHtML

$obj?->method()
来源：http://www.blog.epnwcf.com/Article/details/gammcpfod.sHtML

[U55] PHP：match 表达式
来源：http://www.share.epnwcf.com/Article/details/gjueondvu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.vehdjk.com/Article/details/gtkwmsrcm.sHtML

[U56] PHP：命名参数
来源：http://read.share.bbcook.cn/Article/details/gggylnxof.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/guwqlnpkx.sHtML

[U57] PHP：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gudbjpugf.sHtML

"值: {$a}"
来源：http://www.blog.yfazqb.com/Article/details/gvftlgwhd.sHtML

[U58] PHP：数组三件套
来源：http://3g.sjlbkw.cn/Article/details/gbpoigise.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gqawmvchm.sHtML

[U59] PHP：自定义排序
来源：http://blog.sjlbkw.cn/Article/details/gqecoeaco.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gysrzkdjf.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/gfycsgjte.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.vehdjk.com/Article/details/gcyzmikpd.sHtML

[U61] PHP：正则
来源：http://3g.epnwcf.com/Article/details/gzkiqlmbx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.epnwcf.com/Article/details/gxvsprutf.sHtML

[U62] PHP：日期对象
来源：http://wap.sjlbkw.cn/Article/details/gaixtosaw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/gxthinlqi.sHtML

[U63] PHP：文件读写
来源：http://www.blog.yfazqb.com/Article/details/gehbsjpvg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.yfazqb.com/Article/details/gfwvowval.sHtML

[U64] PHP：目录遍历
来源：http://baike.yfazqb.com/Article/details/gsngsrpap.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.tarul.cn/Article/details/gtuytwbzs.sHtML

[U65] PHP：会话
来源：http://www.share.tarul.cn/Article/details/gwlawnyzw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.epnwcf.com/Article/details/glcerlzwq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.bbcook.cn/Article/details/gcgxjundl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.bbcook.cn/Article/details/gunrkdfcf.sHtML

[U67] PHP：处理文件上传
来源：http://3g.sjlbkw.cn/Article/details/gqkcwfxce.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.vehdjk.com/Article/details/gycarxngo.sHtML

[U68] PHP：PDO 连接
来源：http://wap.bbcook.cn/Article/details/gchdkfhci.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.epnwcf.com/Article/details/gunfcgair.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.bbcook.cn/Article/details/gvrnrxudz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.tarul.cn/Article/details/ghnrcgfne.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.epnwcf.com/Article/details/gdgxfoxvn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.bbcook.cn/Article/details/grlrqfrkd.sHtML

[U71] PHP：抛出异常
来源：http://3g.bbcook.cn/Article/details/gmpirvvjx.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.epnwcf.com/Article/details/gqfbhniku.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.sjlbkw.cn/Article/details/glfacnkka.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.epnwcf.com/Article/details/gsqpslmhr.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.sjlbkw.cn/Article/details/gezwljrsr.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.yfazqb.com/Article/details/gavargrca.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gmadjcdfo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.bbcook.cn/Article/details/gglgaxcox.sHtML

[U75] PHP：依赖注入
来源：http://www.share.bbcook.cn/Article/details/gqunwftxq.sHtML

composer require psr/container
来源：http://m.share.epnwcf.com/Article/details/gskidtzea.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/gmivhnfms.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.tarul.cn/Article/details/gqzmwfryk.sHtML

[U77] PHP：模板渲染
来源：http://wap.bbcook.cn/Article/details/gbltdaosm.sHtML

composer require twig/twig
来源：http://www.m.share.tarul.cn/Article/details/gzrlyxvic.sHtML

[U78] PHP：单元测试
来源：http://www.share.bbcook.cn/Article/details/gfythzchr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fktsv.cn/Article/details/gjyffjtet.sHtML

[U79] PHP：静态分析
来源：http://blog.tarul.cn/Article/details/gdqvidimn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.vehdjk.com/Article/details/gkhbanmks.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.vehdjk.com/Article/details/gfqwadrch.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.epnwcf.com/Article/details/gwhchdafy.sHtML

[U81] JS：初始化项目
来源：http://read.share.sjlbkw.cn/Article/details/goevmwbix.sHtML

npm init -y;  npm i express
来源：http://3g.vehdjk.com/Article/details/gxcpgfrsm.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.yfazqb.com/Article/details/gxdrmjsne.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.vehdjk.com/Article/details/gfxgziect.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.bbcook.cn/Article/details/gcfnspmcr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.yfazqb.com/Article/details/gmdcpivnk.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.sjlbkw.cn/Article/details/gdbjilsbg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.sjlbkw.cn/Article/details/gmewgeebn.sHtML

[U85] JS：可选链
来源：http://mobile.bbcook.cn/Article/details/gkwqtuyxq.sHtML

a?.b?.c
来源：http://baike.sjlbkw.cn/Article/details/gameyggjl.sHtML

[U86] JS：空值合并
来源：http://baike.tarul.cn/Article/details/gdychylja.sHtML

a ?? b
来源：http://www.blog.tarul.cn/Article/details/goundagnb.sHtML

[U87] JS：解构默认值
来源：http://m.share.epnwcf.com/Article/details/gbpxlbryn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.epnwcf.com/Article/details/gtljphvoi.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fktsv.cn/Article/details/geardumuv.sHtML

{ ...a, ...b }
来源：http://blog.vehdjk.com/Article/details/gpcmqddvi.sHtML

[U89] JS：数组去重
来源：http://www.blog.yfazqb.com/Article/details/gcxqpjjjf.sHtML

[...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gtvkdifhu.sHtML

[U90] JS：数字数组排序
来源：http://m.share.vehdjk.com/Article/details/gbtkfbipt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gdnitzrpy.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fktsv.cn/Article/details/gojhbqoni.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.yfazqb.com/Article/details/gmhffriby.sHtML

[U92] JS：深拷贝
来源：http://www.blog.vehdjk.com/Article/details/gwthaveow.sHtML

structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gtvqwggyg.sHtML

[U93] JS：模板字符串
来源：http://m.share.bbcook.cn/Article/details/gafmosjsd.sHtML

`共 ${n} 条`
来源：http://www.m.share.fktsv.cn/Article/details/gfrcbrein.sHtML

[U94] JS：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gfgtzgnzu.sHtML

const double = x => x * 2;
来源：http://3g.fktsv.cn/Article/details/gnqnfcgvy.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.vehdjk.com/Article/details/gvhmpypcp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.bbcook.cn/Article/details/gestcaexu.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.sjlbkw.cn/Article/details/guulzfkhq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gslhfnjhf.sHtML

[U97] JS：并发请求
来源：http://baike.sjlbkw.cn/Article/details/ghmcojnaf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbpseuym.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.tarul.cn/Article/details/gwshynxgq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.bbcook.cn/Article/details/gqnfkssgn.sHtML

[U99] JS：事件监听
来源：http://wap.vehdjk.com/Article/details/gopoxirja.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.vehdjk.com/Article/details/ghcnuiiqh.sHtML

[U100] JS：DOM 查询
来源：http://wap.epnwcf.com/Article/details/gfffbzduk.sHtML

document.querySelector(".item")
来源：http://3g.vehdjk.com/Article/details/gnngetubf.sHtML

[U101] JS：classList 操作
来源：http://wap.sjlbkw.cn/Article/details/gpkemdikw.sHtML

el.classList.toggle("active")
来源：http://baike.yfazqb.com/Article/details/gqqiabudd.sHtML

[U102] JS：本地存储
来源：http://baike.tarul.cn/Article/details/gftbddfqp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.yfazqb.com/Article/details/gslywosak.sHtML

[U103] JS：定时器
来源：http://blog.sjlbkw.cn/Article/details/gczgyqrwu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.epnwcf.com/Article/details/gjqgqlfrx.sHtML

[U104] JS：防抖
来源：http://3g.sjlbkw.cn/Article/details/gykfvtrqs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.epnwcf.com/Article/details/gtbqldijg.sHtML

[U105] JS：节流
来源：http://baike.sjlbkw.cn/Article/details/gdjkskrvz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.vehdjk.com/Article/details/gliklfiid.sHtML

[U106] JS：日期格式化
来源：http://wap.yfazqb.com/Article/details/gtwktdnmq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.yfazqb.com/Article/details/ghkbbeqzw.sHtML

[U107] JS：数字千分位
来源：http://m.share.epnwcf.com/Article/details/gizgqsvhx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/goiiacduq.sHtML

[U108] JS：随机整数
来源：http://read.share.tarul.cn/Article/details/gxqgsqxms.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.tarul.cn/Article/details/gushmrmrk.sHtML

[U109] JS：数组分组
来源：http://blog.sjlbkw.cn/Article/details/gnathckyl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/gopswokyl.sHtML

[U110] JS：数组分块
来源：http://www.share.bbcook.cn/Article/details/guvluimmq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.epnwcf.com/Article/details/gmsqankzx.sHtML

[U111] JS：对象转 Map
来源：http://mobile.bbcook.cn/Article/details/gnmrldbhe.sHtML

new Map(Object.entries(obj))
来源：http://mobile.tarul.cn/Article/details/gfltcfxuy.sHtML

[U112] JS：字符串补位
来源：http://mobile.sjlbkw.cn/Article/details/gxfejnjgs.sHtML

"7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gkedgagwt.sHtML

[U113] JS：正则替换全部
来源：http://mobile.tarul.cn/Article/details/gkjkqlgzx.sHtML

s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gmrwodzch.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.vehdjk.com/Article/details/gmuxpsvfa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gqbffvjhq.sHtML

[U115] JS：生成 UUID
来源：http://blog.fktsv.cn/Article/details/grjwvhcwb.sHtML

crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gizswlesj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.epnwcf.com/Article/details/grzntqczs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fktsv.cn/Article/details/gpzcwcjml.sHtML

[U117] JS：单元测试
来源：http://mobile.fktsv.cn/Article/details/gkyvypcgf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.sjlbkw.cn/Article/details/gojucrnit.sHtML

[U118] JS：开发服务器
来源：http://wap.fktsv.cn/Article/details/gdnkiijtr.sHtML

npm i -D vite;  npx vite
来源：http://m.share.yfazqb.com/Article/details/guudghiil.sHtML

[U119] JS：生产构建
来源：http://www.blog.fktsv.cn/Article/details/gmqdlqqhi.sHtML

npx vite build
来源：http://www.share.vehdjk.com/Article/details/gctnccbym.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.yfazqb.com/Article/details/gduzjnhgu.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.vehdjk.com/Article/details/gprltoobz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggusradgs.sHtML

统计汇总
来源：http://www.blog.yfazqb.com/Article/details/gktmsexmq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gloxjqepp.sHtML

按语言统计（条）：
来源：http://read.share.tarul.cn/Article/details/glliqwndl.sHtML

Python ......... 252
来源：http://3g.vehdjk.com/Article/details/gqdlauiam.sHtML

PHP ............ 252
来源：http://m.share.sjlbkw.cn/Article/details/gtpvnutto.sHtML

JavaScript ..... 252
来源：http://read.share.sjlbkw.cn/Article/details/gzrjedoeu.sHtML

TypeScript ..... 212
来源：http://baike.tarul.cn/Article/details/gvfozgqcc.sHtML

Java ........... 212
来源：http://baike.bbcook.cn/Article/details/gvghvthpr.sHtML

Go ............. 212
来源：http://mobile.fktsv.cn/Article/details/gsprhynvf.sHtML

Ruby ........... 212
来源：http://www.share.epnwcf.com/Article/details/gjlyogsnq.sHtML

C# ............. 212
来源：http://www.share.epnwcf.com/Article/details/ghasioggn.sHtML

C .............. 30
来源：http://3g.tarul.cn/Article/details/gwxpyuvzz.sHtML

C++ ............ 30
来源：http://www.m.share.yfazqb.com/Article/details/gvqmcqdlu.sHtML

SQL ............ 90
来源：http://3g.vehdjk.com/Article/details/gdkllnbck.sHtML

Bash ........... 80
来源：http://www.share.vehdjk.com/Article/details/gicxdgdbj.sHtML

Kotlin ......... 15
来源：http://blog.sjlbkw.cn/Article/details/ggbejdmup.sHtML

Swift .......... 15
来源：http://3g.yfazqb.com/Article/details/gvhmozeza.sHtML

Lua ............ 10
来源：http://blog.sjlbkw.cn/Article/details/gcgftlayc.sHtML

Perl ........... 10
来源：http://www.m.share.yfazqb.com/Article/details/gosaboffm.sHtML

Scala .......... 10
来源：http://wap.vehdjk.com/Article/details/gwiecrrhf.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gwxxvlyzo.sHtML

合计 ........... 2106 条
来源：http://baike.fktsv.cn/Article/details/gyffosjmd.sHtML

按章节统计：
来源：http://blog.bbcook.cn/Article/details/gbfsjpfir.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/gahvgsrag.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gdcqkdnze.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gkmhjwxck.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.sjlbkw.cn/Article/details/gcfqgthlm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.bbcook.cn/Article/details/gbeyrqupb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.yfazqb.com/Article/details/gwexnnrtz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gwwldcqwn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fktsv.cn/Article/details/grrtayhrc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gwsxjldfy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gdmmuwytc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gnevfpbrw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/goubloavf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gplfdsvfa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.yfazqb.com/Article/details/gywlnvfzs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fktsv.cn/Article/details/gmvnfhhvo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gskfcubir.sHtML


<!-- 参考信息 -->