代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://3g.yfazqb.com/Article/details/gkyfqodgl.sHtML

[T55] Scala：集合过滤
来源：http://blog.tarul.cn/Article/details/gohlvduoe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.bbcook.cn/Article/details/gqxkmfpab.sHtML

[T56] Scala：样例类
来源：http://m.share.epnwcf.com/Article/details/guvwaqpmz.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/gztgmvgkp.sHtML

[T57] Scala：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gdsqsmflx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gdmhtrvpi.sHtML

[T58] Scala：函数定义
来源：http://3g.vehdjk.com/Article/details/gkdtmvvly.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.yfazqb.com/Article/details/giyxredkg.sHtML

[T59] Scala：循环
来源：http://baike.epnwcf.com/Article/details/gpqhtpjze.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gaaaaahhl.sHtML

[T60] Scala：折叠
来源：http://baike.vehdjk.com/Article/details/glkollabn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.epnwcf.com/Article/details/glfogigag.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gtvfbfsdl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.bbcook.cn/Article/details/gnrqtqchn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbmhgotvl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.bbcook.cn/Article/details/gmqbnqpmm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.tarul.cn/Article/details/gankambpr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.yfazqb.com/Article/details/gyqqjaeon.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.sjlbkw.cn/Article/details/gjzwmlpwf.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.sjlbkw.cn/Article/details/gltimxawk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.yfazqb.com/Article/details/gsqbnwglw.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.tarul.cn/Article/details/guhkyozwq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.bbcook.cn/Article/details/gmdjcpquv.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.tarul.cn/Article/details/gnvsfhedx.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/gspyovjyy.sHtML

[U06] Py：合并两个字典
来源：http://wap.sjlbkw.cn/Article/details/grdwkzwwq.sHtML

{**a, **b}
来源：http://mobile.bbcook.cn/Article/details/gopkepvct.sHtML

[U07] Py：反转字典键值
来源：http://3g.yfazqb.com/Article/details/gcllrkppl.sHtML

{v: k for k, v in d.items()}
来源：http://wap.vehdjk.com/Article/details/gjaqigaox.sHtML

[U08] Py：展平二维列表
来源：http://m.share.epnwcf.com/Article/details/glcgnoqef.sHtML

[y for x in nested for y in x]
来源：http://wap.yfazqb.com/Article/details/gsoviiisc.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.bbcook.cn/Article/details/gnqlldlqk.sHtML

max(d, key=d.get)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyemcmdhm.sHtML

[U10] Py：按值排序字典
来源：http://read.share.epnwcf.com/Article/details/grvsmofcy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.sjlbkw.cn/Article/details/gjpquychz.sHtML

[U11] Py：生成器表达式
来源：http://www.share.tarul.cn/Article/details/gyfcqesxm.sHtML

(x * 2 for x in arr)
来源：http://blog.vehdjk.com/Article/details/ghaqqvyha.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fktsv.cn/Article/details/gobavhnyw.sHtML

Counter(arr).most_common(3)
来源：http://baike.bbcook.cn/Article/details/gzpiqcrns.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gxccrflpp.sHtML

deque(maxlen=10)
来源：http://www.m.share.yfazqb.com/Article/details/gjlikruuh.sHtML

[U14] Py：分组收集到列表
来源：http://baike.epnwcf.com/Article/details/gznqknjbc.sHtML

defaultdict(list)
来源：http://mobile.sjlbkw.cn/Article/details/govtfugjx.sHtML

[U15] Py：高精度计时
来源：http://3g.fktsv.cn/Article/details/gnusgvtcf.sHtML

t = time.perf_counter()
来源：http://www.m.share.yfazqb.com/Article/details/gjctdvftm.sHtML

[U16] Py：命令行参数解析
来源：http://3g.bbcook.cn/Article/details/gfgovrahx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.bbcook.cn/Article/details/gtrjebwwy.sHtML

[U17] Py：初始化日志
来源：http://m.share.sjlbkw.cn/Article/details/gywyijbvj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.epnwcf.com/Article/details/gbtohqdqp.sHtML

[U18] Py：预编译正则
来源：http://blog.yfazqb.com/Article/details/grbjgoows.sHtML

pat = re.compile(r"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gpaacritk.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.epnwcf.com/Article/details/gwwtvcrmh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.yfazqb.com/Article/details/gxrukvzty.sHtML

[U20] Py：缓存函数结果
来源：http://3g.tarul.cn/Article/details/gwqbvsnzl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.tarul.cn/Article/details/glmcssuai.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.sjlbkw.cn/Article/details/gpxxcrykr.sHtML

@contextlib.contextmanager
来源：http://wap.bbcook.cn/Article/details/gsaznkvok.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fktsv.cn/Article/details/gfigeajzm.sHtML

list(zip(*m))
来源：http://www.share.epnwcf.com/Article/details/grwkrndur.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.epnwcf.com/Article/details/gzzortmqu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.tarul.cn/Article/details/gwmirpjua.sHtML

[U24] Py：路径操作
来源：http://www.m.share.vehdjk.com/Article/details/gcagrmedk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gboahcvka.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/gmtwvkgpl.sHtML

csv.DictReader(f)
来源：http://blog.epnwcf.com/Article/details/gaywpcstn.sHtML

[U26] Py：并发下载
来源：http://baike.yfazqb.com/Article/details/gyaqvqwkp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.yfazqb.com/Article/details/gukuapmgb.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.vehdjk.com/Article/details/ggegalvjl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.vehdjk.com/Article/details/gldvgqwco.sHtML

[U28] Py：类型别名
来源：http://www.m.share.bbcook.cn/Article/details/gniqhangc.sHtML

UserId = int
来源：http://www.blog.bbcook.cn/Article/details/goxzgqqot.sHtML

[U29] Py：属性校验
来源：http://www.m.share.bbcook.cn/Article/details/gtnvvbxom.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fktsv.cn/Article/details/guyhhoqcp.sHtML

[U30] Py：数据类
来源：http://www.m.share.epnwcf.com/Article/details/gtqesafbj.sHtML

@dataclass(slots=True)
来源：http://www.m.share.tarul.cn/Article/details/gunggtijz.sHtML

[U31] Py：单测
来源：http://3g.fktsv.cn/Article/details/gdzaqkecn.sHtML

python -m pytest -q
来源：http://wap.bbcook.cn/Article/details/gvrfitevn.sHtML

[U32] Py：代码格式化
来源：http://mobile.vehdjk.com/Article/details/goltuinyh.sHtML

ruff format . && ruff check --fix .
来源：http://blog.yfazqb.com/Article/details/gtxninfcy.sHtML

[U33] Py：打包发布
来源：http://wap.epnwcf.com/Article/details/ghzxnicbn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.yfazqb.com/Article/details/gagoxkuma.sHtML

[U34] Py：判断编码
来源：http://www.share.sjlbkw.cn/Article/details/gkorbbpag.sHtML

chardet.detect(raw)
来源：http://m.share.yfazqb.com/Article/details/glbfijfal.sHtML

[U35] Py：发送邮件
来源：http://baike.bbcook.cn/Article/details/ghmowhdbc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.epnwcf.com/Article/details/ghnaqptfk.sHtML

[U36] Py：定时任务
来源：http://www.m.share.tarul.cn/Article/details/gnkdgguib.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fktsv.cn/Article/details/gzbqtadww.sHtML

[U37] Py：读写 Excel
来源：http://baike.tarul.cn/Article/details/gfspehick.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fktsv.cn/Article/details/gqatydqva.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.epnwcf.com/Article/details/gcnqauzyy.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.sjlbkw.cn/Article/details/gzhohjxmz.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.epnwcf.com/Article/details/gxvmehtwr.sHtML

sys.stdout.isatty()
来源：http://3g.bbcook.cn/Article/details/gggcqwagl.sHtML

[U40] Py：打印到标准错误
来源：http://baike.tarul.cn/Article/details/gxtzitcty.sHtML

print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gwkdakfhn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.tarul.cn/Article/details/ghibjecvj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.vehdjk.com/Article/details/gumofrawj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.epnwcf.com/Article/details/glmqjuldp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.epnwcf.com/Article/details/gtwetwres.sHtML

[U43] PHP：声明命名空间
来源：http://baike.bbcook.cn/Article/details/gtqgrhcib.sHtML

namespace App\Http;
来源：http://read.share.fktsv.cn/Article/details/ghjcolamm.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fktsv.cn/Article/details/gbhzjhsus.sHtML

declare(strict_types=1);
来源：http://mobile.sjlbkw.cn/Article/details/gurqkcaek.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.bbcook.cn/Article/details/gcjexckrf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/giipxtdba.sHtML

[U46] PHP：可空类型
来源：http://blog.vehdjk.com/Article/details/gdpltztge.sHtML

?string $name = null
来源：http://www.blog.bbcook.cn/Article/details/gaxjitjrt.sHtML

[U47] PHP：联合类型
来源：http://read.share.sjlbkw.cn/Article/details/gmpszzbjg.sHtML

int|string $id
来源：http://m.share.bbcook.cn/Article/details/gztjnjfyu.sHtML

[U48] PHP：纯枚举
来源：http://www.share.sjlbkw.cn/Article/details/gixuesxth.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.epnwcf.com/Article/details/gxmntbzeu.sHtML

[U49] PHP：只读属性
来源：http://www.share.bbcook.cn/Article/details/gzkeojnfg.sHtML

public readonly string $name
来源：http://read.share.yfazqb.com/Article/details/gssvyytcv.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.tarul.cn/Article/details/gijpwncdq.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.yfazqb.com/Article/details/gzziyjeul.sHtML

[U51] PHP：数组解构
来源：http://blog.bbcook.cn/Article/details/gcfsbfsox.sHtML

[$a, $b] = $arr;
来源：http://3g.sjlbkw.cn/Article/details/gnynwhdba.sHtML

[U52] PHP：箭头函数
来源：http://wap.fktsv.cn/Article/details/gifapwbaz.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.sjlbkw.cn/Article/details/gguupbkho.sHtML

[U53] PHP：空合并运算符
来源：http://baike.yfazqb.com/Article/details/gwjzbfita.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fktsv.cn/Article/details/gvynyzhvj.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fktsv.cn/Article/details/gnendqoyw.sHtML

$obj?->method()
来源：http://3g.vehdjk.com/Article/details/gesygatck.sHtML

[U55] PHP：match 表达式
来源：http://baike.tarul.cn/Article/details/gvfiatfru.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.tarul.cn/Article/details/gzityzzsh.sHtML

[U56] PHP：命名参数
来源：http://wap.yfazqb.com/Article/details/glczyhcma.sHtML

f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gytrcrepy.sHtML

[U57] PHP：字符串插值
来源：http://baike.bbcook.cn/Article/details/gqemrmlss.sHtML

"值: {$a}"
来源：http://m.share.yfazqb.com/Article/details/gyvtxsgez.sHtML

[U58] PHP：数组三件套
来源：http://3g.vehdjk.com/Article/details/gbxbendgd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.epnwcf.com/Article/details/gjwgepqnj.sHtML

[U59] PHP：自定义排序
来源：http://m.share.tarul.cn/Article/details/gpdukkkvc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwuzrxkn.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.vehdjk.com/Article/details/gwgyndpnw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.sjlbkw.cn/Article/details/ghpdoiare.sHtML

[U61] PHP：正则
来源：http://wap.epnwcf.com/Article/details/gszikxujo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.vehdjk.com/Article/details/gzkmskcqh.sHtML

[U62] PHP：日期对象
来源：http://blog.tarul.cn/Article/details/giwdtbbiy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fktsv.cn/Article/details/gurrhtryj.sHtML

[U63] PHP：文件读写
来源：http://m.share.tarul.cn/Article/details/gyedidsgu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.bbcook.cn/Article/details/gajlwhxvc.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fktsv.cn/Article/details/gdfcryckg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.sjlbkw.cn/Article/details/gbfwxbbjy.sHtML

[U65] PHP：会话
来源：http://baike.sjlbkw.cn/Article/details/geophrwvb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/ghasucglk.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.vehdjk.com/Article/details/gmhdzeqgd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fktsv.cn/Article/details/gbwktsuim.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.yfazqb.com/Article/details/gbfirawdo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.vehdjk.com/Article/details/gztsoohdb.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.bbcook.cn/Article/details/glqvzuwud.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.epnwcf.com/Article/details/gxafxlezz.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.tarul.cn/Article/details/gyukjfgpt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.epnwcf.com/Article/details/gkukzeumy.sHtML

[U70] PHP：PDO 事务
来源：http://blog.sjlbkw.cn/Article/details/glxhkhxem.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.vehdjk.com/Article/details/gyzcvzoxg.sHtML

[U71] PHP：抛出异常
来源：http://baike.tarul.cn/Article/details/gyayiphzm.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.yfazqb.com/Article/details/gknhotsyb.sHtML

[U72] PHP：写错误日志
来源：http://m.share.vehdjk.com/Article/details/gofyykxma.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fktsv.cn/Article/details/gwzaxiqxt.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fktsv.cn/Article/details/ggrluijsi.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.tarul.cn/Article/details/glatkqaww.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.tarul.cn/Article/details/gchwjsklj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.vehdjk.com/Article/details/gzmbuvpwx.sHtML

[U75] PHP：依赖注入
来源：http://mobile.bbcook.cn/Article/details/gclwyhkcm.sHtML

composer require psr/container
来源：http://baike.sjlbkw.cn/Article/details/gurklhdyp.sHtML

[U76] PHP：简单路由
来源：http://baike.epnwcf.com/Article/details/ggazhvnmw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcpvqaxa.sHtML

[U77] PHP：模板渲染
来源：http://m.share.vehdjk.com/Article/details/glqmqhhyl.sHtML

composer require twig/twig
来源：http://blog.vehdjk.com/Article/details/gpqaslsmu.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gkykoxwmg.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.yfazqb.com/Article/details/ggjzhfadn.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.bbcook.cn/Article/details/gnmsraojp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.sjlbkw.cn/Article/details/gzgbkepjp.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.epnwcf.com/Article/details/gneoxshqy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.sjlbkw.cn/Article/details/gmnwnlqsg.sHtML

[U81] JS：初始化项目
来源：http://read.share.fktsv.cn/Article/details/gjvwrifkj.sHtML

npm init -y;  npm i express
来源：http://m.share.tarul.cn/Article/details/gwvrtenhw.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.vehdjk.com/Article/details/gyklnpabd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fktsv.cn/Article/details/gjxoaoems.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.bbcook.cn/Article/details/gemiwxvss.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/gbzeuoidg.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.yfazqb.com/Article/details/gepuwlkqq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fktsv.cn/Article/details/gjpdazwrw.sHtML

[U85] JS：可选链
来源：http://baike.sjlbkw.cn/Article/details/ggdcmchlh.sHtML

a?.b?.c
来源：http://m.share.sjlbkw.cn/Article/details/gwmswicfd.sHtML

[U86] JS：空值合并
来源：http://www.share.yfazqb.com/Article/details/gqnpfwlfa.sHtML

a ?? b
来源：http://3g.yfazqb.com/Article/details/gwbocavpc.sHtML

[U87] JS：解构默认值
来源：http://mobile.tarul.cn/Article/details/gbiwshgbn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.epnwcf.com/Article/details/guzyqnnnq.sHtML

[U88] JS：对象展开合并
来源：http://blog.tarul.cn/Article/details/gfeyeamwl.sHtML

{ ...a, ...b }
来源：http://baike.vehdjk.com/Article/details/gajccatfj.sHtML

[U89] JS：数组去重
来源：http://3g.vehdjk.com/Article/details/gfpakxtfm.sHtML

[...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/gubhhhhju.sHtML

[U90] JS：数字数组排序
来源：http://blog.sjlbkw.cn/Article/details/gxayvmpcu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/glqwiazwg.sHtML

[U91] JS：对象键值遍历
来源：http://blog.sjlbkw.cn/Article/details/grcgfteib.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/griajegxc.sHtML

[U92] JS：深拷贝
来源：http://m.share.tarul.cn/Article/details/grwtejguc.sHtML

structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gchawtgqm.sHtML

[U93] JS：模板字符串
来源：http://www.share.fktsv.cn/Article/details/gjsxiilzv.sHtML

`共 ${n} 条`
来源：http://3g.tarul.cn/Article/details/gbzkginpk.sHtML

[U94] JS：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gwjmxpcrb.sHtML

const double = x => x * 2;
来源：http://www.blog.epnwcf.com/Article/details/govbjjxzx.sHtML

[U95] JS：Promise 包装
来源：http://wap.vehdjk.com/Article/details/ghkpkqpee.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.epnwcf.com/Article/details/ghyhoguvl.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.vehdjk.com/Article/details/gczqyubwg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gekgwicfe.sHtML

[U97] JS：并发请求
来源：http://baike.yfazqb.com/Article/details/givhanfzh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gltdbwpjb.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.epnwcf.com/Article/details/glbcgmkqu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.yfazqb.com/Article/details/ggrnaimwj.sHtML

[U99] JS：事件监听
来源：http://read.share.vehdjk.com/Article/details/golkcefoy.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.vehdjk.com/Article/details/gxlxvzeti.sHtML

[U100] JS：DOM 查询
来源：http://read.share.bbcook.cn/Article/details/gtnplhmaj.sHtML

document.querySelector(".item")
来源：http://baike.epnwcf.com/Article/details/ghdwdragw.sHtML

[U101] JS：classList 操作
来源：http://mobile.yfazqb.com/Article/details/gpbvdiacc.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fktsv.cn/Article/details/gxofpocbm.sHtML

[U102] JS：本地存储
来源：http://mobile.fktsv.cn/Article/details/gdhffzhgy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.vehdjk.com/Article/details/gectieeom.sHtML

[U103] JS：定时器
来源：http://www.blog.sjlbkw.cn/Article/details/geaksmkfh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fktsv.cn/Article/details/getomtxlt.sHtML

[U104] JS：防抖
来源：http://read.share.epnwcf.com/Article/details/gfnjdmdix.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gifbvimvu.sHtML

[U105] JS：节流
来源：http://blog.epnwcf.com/Article/details/gkpgvdvtz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.tarul.cn/Article/details/govbbqjtj.sHtML

[U106] JS：日期格式化
来源：http://baike.vehdjk.com/Article/details/gxkszzeht.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.sjlbkw.cn/Article/details/ggwuxaosg.sHtML

[U107] JS：数字千分位
来源：http://wap.sjlbkw.cn/Article/details/gumjsujte.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fktsv.cn/Article/details/gltxywzyp.sHtML

[U108] JS：随机整数
来源：http://read.share.sjlbkw.cn/Article/details/gnntwrzvn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.bbcook.cn/Article/details/grthvhufz.sHtML

[U109] JS：数组分组
来源：http://www.m.share.tarul.cn/Article/details/gttzwfubo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.vehdjk.com/Article/details/gugvnmwbd.sHtML

[U110] JS：数组分块
来源：http://www.share.bbcook.cn/Article/details/gtxndhmel.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.epnwcf.com/Article/details/gputxvtqg.sHtML

[U111] JS：对象转 Map
来源：http://blog.sjlbkw.cn/Article/details/gmvfdjhho.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.yfazqb.com/Article/details/gqkbkqvec.sHtML

[U112] JS：字符串补位
来源：http://www.share.bbcook.cn/Article/details/gqditcxmc.sHtML

"7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gtpupztol.sHtML

[U113] JS：正则替换全部
来源：http://blog.bbcook.cn/Article/details/gioysqdxz.sHtML

s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gyqefudfn.sHtML

[U114] JS：JSON 深比较
来源：http://3g.yfazqb.com/Article/details/gtsaamdwj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.vehdjk.com/Article/details/gmphecbjr.sHtML

[U115] JS：生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gavormitt.sHtML

crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gtjwudrcu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fktsv.cn/Article/details/gfalwwzhv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fktsv.cn/Article/details/getjstxow.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/ghoivtwev.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.vehdjk.com/Article/details/gjjgoyzdb.sHtML

[U118] JS：开发服务器
来源：http://baike.epnwcf.com/Article/details/gvbpfuoei.sHtML

npm i -D vite;  npx vite
来源：http://read.share.vehdjk.com/Article/details/gwibqgnvi.sHtML

[U119] JS：生产构建
来源：http://www.share.epnwcf.com/Article/details/gsreibpeh.sHtML

npx vite build
来源：http://wap.yfazqb.com/Article/details/gntewhxcl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.tarul.cn/Article/details/gadrewqjz.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.vehdjk.com/Article/details/gbgcckutu.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwoautzvc.sHtML

统计汇总
来源：http://wap.epnwcf.com/Article/details/goftrgoik.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghhgekmqi.sHtML

按语言统计（条）：
来源：http://m.share.tarul.cn/Article/details/gmujioohb.sHtML

Python ......... 252
来源：http://m.share.fktsv.cn/Article/details/gotdcrvsv.sHtML

PHP ............ 252
来源：http://3g.tarul.cn/Article/details/gczlsryei.sHtML

JavaScript ..... 252
来源：http://read.share.yfazqb.com/Article/details/gyvsygweq.sHtML

TypeScript ..... 212
来源：http://mobile.sjlbkw.cn/Article/details/gsesarkul.sHtML

Java ........... 212
来源：http://baike.bbcook.cn/Article/details/gbnrjvpml.sHtML

Go ............. 212
来源：http://blog.tarul.cn/Article/details/ghdjrkcva.sHtML

Ruby ........... 212
来源：http://m.share.sjlbkw.cn/Article/details/gynaniyuj.sHtML

C# ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/gdwhsomrz.sHtML

C .............. 30
来源：http://www.m.share.sjlbkw.cn/Article/details/gglwyalqb.sHtML

C++ ............ 30
来源：http://wap.tarul.cn/Article/details/gqbyfbxaf.sHtML

SQL ............ 90
来源：http://www.blog.bbcook.cn/Article/details/ghvypxxxv.sHtML

Bash ........... 80
来源：http://www.share.yfazqb.com/Article/details/gsactkrnu.sHtML

Kotlin ......... 15
来源：http://www.blog.epnwcf.com/Article/details/gcvqdefxt.sHtML

Swift .......... 15
来源：http://m.share.vehdjk.com/Article/details/gyayvlyaf.sHtML

Lua ............ 10
来源：http://www.share.yfazqb.com/Article/details/gvpafheok.sHtML

Perl ........... 10
来源：http://wap.fktsv.cn/Article/details/gwlndidrg.sHtML

Scala .......... 10
来源：http://www.m.share.fktsv.cn/Article/details/gjyvbviav.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gjowgmnbz.sHtML

合计 ........... 2106 条
来源：http://baike.epnwcf.com/Article/details/gmzfkkazs.sHtML

按章节统计：
来源：http://wap.epnwcf.com/Article/details/grbyrkmzk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.bbcook.cn/Article/details/gyblgxwyo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/gnocmoqjr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/guvbpwuzc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.yfazqb.com/Article/details/gsbppxzks.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.sjlbkw.cn/Article/details/gmlhjqwms.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/gwweuwbcj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/glpvcfktn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.yfazqb.com/Article/details/gdbtirkkg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gdrsbejwm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.tarul.cn/Article/details/gmkbptlwn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gftjeuzcj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/ggtlhpvdx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/ggzyzslet.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.tarul.cn/Article/details/gqskmvjpg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.epnwcf.com/Article/details/gllkcjkox.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gzgsekbmb.sHtML

Q SQL 专题                              90
来源：http://read.share.vehdjk.com/Article/details/gvgosgiep.sHtML

R Bash 专题                             80
来源：http://3g.tarul.cn/Article/details/gpnzfwvga.sHtML

S C / C++ 专题                          60
来源：http://blog.sjlbkw.cn/Article/details/gzwfgmvdr.sHtML

T 其他语言补充                          60
来源：http://baike.epnwcf.com/Article/details/gifuxrnar.sHtML


<!-- 参考信息 -->