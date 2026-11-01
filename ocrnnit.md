代发 wailian999

case class User(name: String, age: Int)
来源：http://read.share.vehdjk.com/Article/details/gupyrfasz.sHtML

[T57] Scala：模式匹配
来源：http://m.share.vehdjk.com/Article/details/gvmbfvzoj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fktsv.cn/Article/details/gguufiffc.sHtML

[T58] Scala：函数定义
来源：http://wap.yfazqb.com/Article/details/gvdyrruak.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.vehdjk.com/Article/details/gxcqgmekh.sHtML

[T59] Scala：循环
来源：http://mobile.fktsv.cn/Article/details/gscecemuz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/geofxqatj.sHtML

[T60] Scala：折叠
来源：http://m.share.vehdjk.com/Article/details/gorfixnky.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/gzvawzgws.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gvjgekhlo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gjcmcpobv.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwogzpaji.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.yfazqb.com/Article/details/gjesjxpsj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.vehdjk.com/Article/details/gajbvuhrf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.epnwcf.com/Article/details/gxmljpihv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.yfazqb.com/Article/details/gxcmprbwf.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.sjlbkw.cn/Article/details/ghfenbiwe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.bbcook.cn/Article/details/gqbqrxkua.sHtML

[U04] Py：变量调试打印
来源：http://blog.tarul.cn/Article/details/gxexsiduo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.yfazqb.com/Article/details/gxersoxry.sHtML

[U05] Py：列表去重且保序
来源：http://baike.epnwcf.com/Article/details/gjoxryzfk.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/gnyyjifwl.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gifvqrydu.sHtML

{**a, **b}
来源：http://3g.tarul.cn/Article/details/gsfpghqvf.sHtML

[U07] Py：反转字典键值
来源：http://baike.tarul.cn/Article/details/gdbjxtkqk.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.bbcook.cn/Article/details/glipmqejz.sHtML

[U08] Py：展平二维列表
来源：http://baike.sjlbkw.cn/Article/details/gjrqurpmf.sHtML

[y for x in nested for y in x]
来源：http://wap.bbcook.cn/Article/details/gqaqefztn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.bbcook.cn/Article/details/gsxkftefk.sHtML

max(d, key=d.get)
来源：http://read.share.epnwcf.com/Article/details/gllnsmzcw.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.yfazqb.com/Article/details/gbvyegqfp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.sjlbkw.cn/Article/details/gpqbxdajz.sHtML

[U11] Py：生成器表达式
来源：http://www.share.bbcook.cn/Article/details/gdsxscvze.sHtML

(x * 2 for x in arr)
来源：http://blog.tarul.cn/Article/details/gyejqgqzl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fktsv.cn/Article/details/gzlagkpwh.sHtML

Counter(arr).most_common(3)
来源：http://3g.sjlbkw.cn/Article/details/gnkbnqfnl.sHtML

[U13] Py：固定长度队列
来源：http://wap.yfazqb.com/Article/details/ghucifolv.sHtML

deque(maxlen=10)
来源：http://blog.epnwcf.com/Article/details/gzvyanxsy.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.bbcook.cn/Article/details/gtlylpadw.sHtML

defaultdict(list)
来源：http://m.share.sjlbkw.cn/Article/details/gpxeakggn.sHtML

[U15] Py：高精度计时
来源：http://blog.sjlbkw.cn/Article/details/ghrqkxqft.sHtML

t = time.perf_counter()
来源：http://www.blog.yfazqb.com/Article/details/goophqtkn.sHtML

[U16] Py：命令行参数解析
来源：http://3g.epnwcf.com/Article/details/gmbgrcvwi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.tarul.cn/Article/details/gowcjqyar.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.tarul.cn/Article/details/gqsrqpvoy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.yfazqb.com/Article/details/gpqkpdufh.sHtML

[U18] Py：预编译正则
来源：http://3g.fktsv.cn/Article/details/ghmdndaln.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fktsv.cn/Article/details/gdkmlihxp.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.tarul.cn/Article/details/gybmyfzgc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.bbcook.cn/Article/details/gisfcuhuz.sHtML

[U20] Py：缓存函数结果
来源：http://3g.vehdjk.com/Article/details/gvdhnqpns.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.bbcook.cn/Article/details/gdkjqtkej.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.yfazqb.com/Article/details/gurqbcugo.sHtML

@contextlib.contextmanager
来源：http://www.share.sjlbkw.cn/Article/details/glvprmwak.sHtML

[U22] Py：矩阵转置
来源：http://wap.tarul.cn/Article/details/gjrvcdpwu.sHtML

list(zip(*m))
来源：http://www.m.share.epnwcf.com/Article/details/gxmxseyos.sHtML

[U23] Py：分块读取大文件
来源：http://baike.yfazqb.com/Article/details/glcmjydph.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.sjlbkw.cn/Article/details/gpeszgfai.sHtML

[U24] Py：路径操作
来源：http://read.share.vehdjk.com/Article/details/gozirmvap.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gmydeoqjm.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.bbcook.cn/Article/details/gaewdyzig.sHtML

csv.DictReader(f)
来源：http://www.share.sjlbkw.cn/Article/details/gskshmayy.sHtML

[U26] Py：并发下载
来源：http://blog.yfazqb.com/Article/details/grsbysrxf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.bbcook.cn/Article/details/gkmpboscs.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.epnwcf.com/Article/details/gzobjazih.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.bbcook.cn/Article/details/gyunzjzmd.sHtML

[U28] Py：类型别名
来源：http://read.share.epnwcf.com/Article/details/gaforkxuy.sHtML

UserId = int
来源：http://mobile.yfazqb.com/Article/details/gjdqzrhgd.sHtML

[U29] Py：属性校验
来源：http://read.share.sjlbkw.cn/Article/details/gyrcfkbvt.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.tarul.cn/Article/details/gsxrcicqc.sHtML

[U30] Py：数据类
来源：http://wap.bbcook.cn/Article/details/gkkncyxep.sHtML

@dataclass(slots=True)
来源：http://blog.vehdjk.com/Article/details/gtmueuiju.sHtML

[U31] Py：单测
来源：http://www.share.fktsv.cn/Article/details/glxgbrdxw.sHtML

python -m pytest -q
来源：http://blog.fktsv.cn/Article/details/gcmqfwohf.sHtML

[U32] Py：代码格式化
来源：http://blog.fktsv.cn/Article/details/gtacsythx.sHtML

ruff format . && ruff check --fix .
来源：http://3g.vehdjk.com/Article/details/gchlhzxwd.sHtML

[U33] Py：打包发布
来源：http://3g.bbcook.cn/Article/details/giuupyuon.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fktsv.cn/Article/details/gzpoqnvqd.sHtML

[U34] Py：判断编码
来源：http://wap.fktsv.cn/Article/details/gafcvknyw.sHtML

chardet.detect(raw)
来源：http://3g.sjlbkw.cn/Article/details/gefusgppl.sHtML

[U35] Py：发送邮件
来源：http://read.share.yfazqb.com/Article/details/gregqauct.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.yfazqb.com/Article/details/guuievuth.sHtML

[U36] Py：定时任务
来源：http://m.share.fktsv.cn/Article/details/goayyaenr.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.epnwcf.com/Article/details/gwiomlmnf.sHtML

[U37] Py：读写 Excel
来源：http://blog.fktsv.cn/Article/details/gscqwkaof.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.tarul.cn/Article/details/ghliqliyn.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.epnwcf.com/Article/details/gofwrerar.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.sjlbkw.cn/Article/details/geutjqwyf.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.bbcook.cn/Article/details/gqrekhiqq.sHtML

sys.stdout.isatty()
来源：http://m.share.vehdjk.com/Article/details/gpvgpqzow.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.vehdjk.com/Article/details/ggfdfufta.sHtML

print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/gatqboeae.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.epnwcf.com/Article/details/grxsqybjx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.sjlbkw.cn/Article/details/gqfherjnx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.tarul.cn/Article/details/ghiuvewuo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.yfazqb.com/Article/details/gybrdidst.sHtML

[U43] PHP：声明命名空间
来源：http://wap.sjlbkw.cn/Article/details/gwtbjztqz.sHtML

namespace App\Http;
来源：http://wap.tarul.cn/Article/details/gftlgwdfz.sHtML

[U44] PHP：开启严格类型
来源：http://wap.vehdjk.com/Article/details/gozmkdbnx.sHtML

declare(strict_types=1);
来源：http://www.share.fktsv.cn/Article/details/grrtfydhq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.sjlbkw.cn/Article/details/gairemzuk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gyrgcpeaa.sHtML

[U46] PHP：可空类型
来源：http://m.share.epnwcf.com/Article/details/grrzygyin.sHtML

?string $name = null
来源：http://www.blog.tarul.cn/Article/details/gsxaxiciy.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fktsv.cn/Article/details/gbkqismrf.sHtML

int|string $id
来源：http://www.m.share.yfazqb.com/Article/details/ghhrikoxq.sHtML

[U48] PHP：纯枚举
来源：http://read.share.sjlbkw.cn/Article/details/gmyenkbof.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.sjlbkw.cn/Article/details/gmcsvyhyn.sHtML

[U49] PHP：只读属性
来源：http://baike.bbcook.cn/Article/details/gwoxdhdln.sHtML

public readonly string $name
来源：http://m.share.sjlbkw.cn/Article/details/godswkjkq.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.bbcook.cn/Article/details/gvlxchekm.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fktsv.cn/Article/details/gkoacprjy.sHtML

[U51] PHP：数组解构
来源：http://www.blog.yfazqb.com/Article/details/ggkjozsfd.sHtML

[$a, $b] = $arr;
来源：http://blog.bbcook.cn/Article/details/gyjmfxdtx.sHtML

[U52] PHP：箭头函数
来源：http://baike.sjlbkw.cn/Article/details/gwtaxbtbu.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.sjlbkw.cn/Article/details/gtejkhjhu.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.bbcook.cn/Article/details/gmdbeyhyu.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.sjlbkw.cn/Article/details/glfgotthx.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.epnwcf.com/Article/details/gpbeiwhgi.sHtML

$obj?->method()
来源：http://mobile.sjlbkw.cn/Article/details/gfoksvgzr.sHtML

[U55] PHP：match 表达式
来源：http://mobile.epnwcf.com/Article/details/gvpvzosgm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fktsv.cn/Article/details/greuvxkwh.sHtML

[U56] PHP：命名参数
来源：http://m.share.fktsv.cn/Article/details/gmagryyms.sHtML

f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gdhamgiue.sHtML

[U57] PHP：字符串插值
来源：http://baike.vehdjk.com/Article/details/gliqvqomg.sHtML

"值: {$a}"
来源：http://blog.fktsv.cn/Article/details/gpkdexwap.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fktsv.cn/Article/details/grivxppda.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fktsv.cn/Article/details/glianqqws.sHtML

[U59] PHP：自定义排序
来源：http://www.share.bbcook.cn/Article/details/gmksugtay.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fktsv.cn/Article/details/gocaykthb.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.yfazqb.com/Article/details/gwrhqffnu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.tarul.cn/Article/details/gozggqxyh.sHtML

[U61] PHP：正则
来源：http://www.m.share.tarul.cn/Article/details/gvhdvoijb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gyxlsqlpy.sHtML

[U62] PHP：日期对象
来源：http://wap.tarul.cn/Article/details/ghhlyaoox.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.tarul.cn/Article/details/gshiygttb.sHtML

[U63] PHP：文件读写
来源：http://read.share.yfazqb.com/Article/details/gqbeqrplp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.sjlbkw.cn/Article/details/gluyapjqs.sHtML

[U64] PHP：目录遍历
来源：http://mobile.yfazqb.com/Article/details/ggqhlmqxp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fktsv.cn/Article/details/gbaeyismu.sHtML

[U65] PHP：会话
来源：http://www.m.share.fktsv.cn/Article/details/ghjkuhgcs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.yfazqb.com/Article/details/grstyzpnt.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.tarul.cn/Article/details/gyfcgqwzz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fktsv.cn/Article/details/gmcfchwol.sHtML

[U67] PHP：处理文件上传
来源：http://3g.yfazqb.com/Article/details/ghugthbam.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.yfazqb.com/Article/details/gtuokdhxq.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.sjlbkw.cn/Article/details/gedbjsauf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.sjlbkw.cn/Article/details/gnmbsxzij.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.bbcook.cn/Article/details/ggolugehp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.vehdjk.com/Article/details/gbkwkfuxx.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fktsv.cn/Article/details/geznelncr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.yfazqb.com/Article/details/gegglazdt.sHtML

[U71] PHP：抛出异常
来源：http://read.share.yfazqb.com/Article/details/gzfvhrjyz.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.bbcook.cn/Article/details/gxttnsgmv.sHtML

[U72] PHP：写错误日志
来源：http://wap.epnwcf.com/Article/details/grwmkpouh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.vehdjk.com/Article/details/goatjecbe.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.yfazqb.com/Article/details/gnwthuacn.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.vehdjk.com/Article/details/gdyosimgw.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gnumtgilr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.yfazqb.com/Article/details/gjyhufese.sHtML

[U75] PHP：依赖注入
来源：http://read.share.sjlbkw.cn/Article/details/gvnaybcfw.sHtML

composer require psr/container
来源：http://baike.bbcook.cn/Article/details/gyxwmyasb.sHtML

[U76] PHP：简单路由
来源：http://baike.bbcook.cn/Article/details/gltvzgikn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.bbcook.cn/Article/details/gbqscsfqd.sHtML

[U77] PHP：模板渲染
来源：http://blog.tarul.cn/Article/details/gdtpgbyty.sHtML

composer require twig/twig
来源：http://read.share.epnwcf.com/Article/details/grottapki.sHtML

[U78] PHP：单元测试
来源：http://baike.epnwcf.com/Article/details/gozwkmlpp.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.epnwcf.com/Article/details/gpxxsyith.sHtML

[U79] PHP：静态分析
来源：http://mobile.sjlbkw.cn/Article/details/gtozqumwu.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.sjlbkw.cn/Article/details/glmhcswdu.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fktsv.cn/Article/details/gevgdotdu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fktsv.cn/Article/details/gkbnopcji.sHtML

[U81] JS：初始化项目
来源：http://blog.epnwcf.com/Article/details/gqwnqxjyg.sHtML

npm init -y;  npm i express
来源：http://baike.sjlbkw.cn/Article/details/gfudatwaf.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.bbcook.cn/Article/details/gezljhndg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fktsv.cn/Article/details/gyshrmeih.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fktsv.cn/Article/details/gexqixwum.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.bbcook.cn/Article/details/glhafnknx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.epnwcf.com/Article/details/gzcviaalo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.sjlbkw.cn/Article/details/gfpwildzh.sHtML

[U85] JS：可选链
来源：http://3g.yfazqb.com/Article/details/gzyravqit.sHtML

a?.b?.c
来源：http://www.m.share.bbcook.cn/Article/details/gdkkylmnc.sHtML

[U86] JS：空值合并
来源：http://www.share.tarul.cn/Article/details/gisqfxunv.sHtML

a ?? b
来源：http://3g.sjlbkw.cn/Article/details/gkjtdvzqb.sHtML

[U87] JS：解构默认值
来源：http://baike.tarul.cn/Article/details/gilwztngi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.yfazqb.com/Article/details/gmabqunnw.sHtML

[U88] JS：对象展开合并
来源：http://3g.epnwcf.com/Article/details/gcghepild.sHtML

{ ...a, ...b }
来源：http://m.share.bbcook.cn/Article/details/ggayaoupg.sHtML

[U89] JS：数组去重
来源：http://blog.yfazqb.com/Article/details/gkcslogyt.sHtML

[...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gpvbugkzj.sHtML

[U90] JS：数字数组排序
来源：http://read.share.vehdjk.com/Article/details/gfrntyfya.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gcowlgoqb.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.yfazqb.com/Article/details/gqrfyngre.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.vehdjk.com/Article/details/gsmdzmkqt.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gkdursaqe.sHtML

structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gvpthekvl.sHtML

[U93] JS：模板字符串
来源：http://wap.fktsv.cn/Article/details/gsomakcog.sHtML

`共 ${n} 条`
来源：http://baike.epnwcf.com/Article/details/gvbsyomyi.sHtML

[U94] JS：箭头函数
来源：http://www.share.bbcook.cn/Article/details/gyupjvggc.sHtML

const double = x => x * 2;
来源：http://baike.vehdjk.com/Article/details/gmjpetxum.sHtML

[U95] JS：Promise 包装
来源：http://baike.vehdjk.com/Article/details/gnnxnjkhb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.sjlbkw.cn/Article/details/ghtfigzed.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.vehdjk.com/Article/details/gngfcnfqx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/guanutnuj.sHtML

[U97] JS：并发请求
来源：http://baike.tarul.cn/Article/details/gxdfgvnkw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gjoyrcrkc.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.vehdjk.com/Article/details/gakupbtyb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.epnwcf.com/Article/details/gujhtoaxx.sHtML

[U99] JS：事件监听
来源：http://www.blog.bbcook.cn/Article/details/gpiudmjax.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.tarul.cn/Article/details/guwryugsk.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.vehdjk.com/Article/details/goptrnzek.sHtML

document.querySelector(".item")
来源：http://read.share.epnwcf.com/Article/details/gdmdxvvlb.sHtML

[U101] JS：classList 操作
来源：http://m.share.fktsv.cn/Article/details/gncwwtpjp.sHtML

el.classList.toggle("active")
来源：http://mobile.bbcook.cn/Article/details/gzrxcojsy.sHtML

[U102] JS：本地存储
来源：http://3g.sjlbkw.cn/Article/details/gklhcxvwq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.tarul.cn/Article/details/gldpdnmcl.sHtML

[U103] JS：定时器
来源：http://3g.fktsv.cn/Article/details/gblbhrynm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.tarul.cn/Article/details/gcjuiflbs.sHtML

[U104] JS：防抖
来源：http://m.share.sjlbkw.cn/Article/details/gsknyivkz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gbkjxqmkb.sHtML

[U105] JS：节流
来源：http://read.share.vehdjk.com/Article/details/geggcenoh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.sjlbkw.cn/Article/details/gkkaonwfz.sHtML

[U106] JS：日期格式化
来源：http://mobile.fktsv.cn/Article/details/gplsptosn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.vehdjk.com/Article/details/gjlgruzye.sHtML

[U107] JS：数字千分位
来源：http://m.share.tarul.cn/Article/details/glbsblnbv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.tarul.cn/Article/details/gmaapenqe.sHtML

[U108] JS：随机整数
来源：http://www.share.sjlbkw.cn/Article/details/gjxwrnpme.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.vehdjk.com/Article/details/gzvouixyd.sHtML

[U109] JS：数组分组
来源：http://baike.bbcook.cn/Article/details/ghlueiskf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.bbcook.cn/Article/details/gvbsxlwth.sHtML

[U110] JS：数组分块
来源：http://www.m.share.epnwcf.com/Article/details/gugdbqhvp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fktsv.cn/Article/details/gytsfygpn.sHtML

[U111] JS：对象转 Map
来源：http://mobile.sjlbkw.cn/Article/details/gtkgdrisx.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.sjlbkw.cn/Article/details/gypnmtita.sHtML

[U112] JS：字符串补位
来源：http://www.share.tarul.cn/Article/details/gmynnfkyy.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gjvxduerr.sHtML

[U113] JS：正则替换全部
来源：http://blog.vehdjk.com/Article/details/gnwnqdmgk.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gdqshdlld.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.yfazqb.com/Article/details/gmbjismes.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gwdgldoct.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/gmkpheheu.sHtML

crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/grusyoemf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.tarul.cn/Article/details/gghnvcsca.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gthdvjlcn.sHtML

[U117] JS：单元测试
来源：http://www.share.vehdjk.com/Article/details/gkdtarvdw.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.yfazqb.com/Article/details/gmbmwianl.sHtML

[U118] JS：开发服务器
来源：http://mobile.tarul.cn/Article/details/gcbdvzalo.sHtML

npm i -D vite;  npx vite
来源：http://m.share.vehdjk.com/Article/details/gxuiqbobw.sHtML

[U119] JS：生产构建
来源：http://read.share.tarul.cn/Article/details/gbkrffyro.sHtML

npx vite build
来源：http://wap.epnwcf.com/Article/details/giaqxwbrt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.yfazqb.com/Article/details/gbachbria.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.sjlbkw.cn/Article/details/gwebhnqmc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvjepqihq.sHtML

统计汇总
来源：http://mobile.epnwcf.com/Article/details/gdmumjuxa.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gtextvnvy.sHtML

按语言统计（条）：
来源：http://wap.sjlbkw.cn/Article/details/glohtufdm.sHtML

Python ......... 252
来源：http://www.share.tarul.cn/Article/details/gwkaazair.sHtML

PHP ............ 252
来源：http://www.blog.vehdjk.com/Article/details/gudfznqoy.sHtML

JavaScript ..... 252
来源：http://3g.vehdjk.com/Article/details/ghtdrneso.sHtML

TypeScript ..... 212
来源：http://baike.tarul.cn/Article/details/gebzenzsb.sHtML

Java ........... 212
来源：http://mobile.vehdjk.com/Article/details/gzqjibrmq.sHtML

Go ............. 212
来源：http://wap.bbcook.cn/Article/details/grivdmmll.sHtML

Ruby ........... 212
来源：http://www.m.share.tarul.cn/Article/details/gboaxgqzo.sHtML

C# ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/ggrnjoewq.sHtML

C .............. 30
来源：http://read.share.fktsv.cn/Article/details/gcuyupsvx.sHtML

C++ ............ 30
来源：http://www.blog.epnwcf.com/Article/details/gfzduyosz.sHtML

SQL ............ 90
来源：http://read.share.fktsv.cn/Article/details/gjtuaeuur.sHtML

Bash ........... 80
来源：http://www.blog.tarul.cn/Article/details/glatprglz.sHtML

Kotlin ......... 15
来源：http://wap.bbcook.cn/Article/details/gamreeoti.sHtML

Swift .......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/glxonkhsh.sHtML

Lua ............ 10
来源：http://www.share.bbcook.cn/Article/details/gbnacexqo.sHtML

Perl ........... 10
来源：http://www.blog.sjlbkw.cn/Article/details/gkuhvphxh.sHtML

Scala .......... 10
来源：http://blog.tarul.cn/Article/details/grxwlzfdn.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/glmcjalxj.sHtML

合计 ........... 2106 条
来源：http://wap.vehdjk.com/Article/details/gbilpbuck.sHtML

按章节统计：
来源：http://www.m.share.tarul.cn/Article/details/gblpfbhsz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.yfazqb.com/Article/details/gvyrjwaay.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/ghyueanzf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gofzvjjll.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/gyzldxrqg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.bbcook.cn/Article/details/guucmtpzi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fktsv.cn/Article/details/gsarldsvp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gqfnwbdbl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/gwhinhzoj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gsbrdetkr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fktsv.cn/Article/details/gqztzykof.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gwjfeyrrt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gpatcmgii.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gmmdfotzn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.yfazqb.com/Article/details/gvrvojund.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.sjlbkw.cn/Article/details/gxqvixgdh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/giyfbornd.sHtML

Q SQL 专题                              90
来源：http://m.share.bbcook.cn/Article/details/gvvwtzzlv.sHtML

R Bash 专题                             80
来源：http://www.blog.tarul.cn/Article/details/ggerhvtzs.sHtML

S C / C++ 专题                          60
来源：http://3g.yfazqb.com/Article/details/gbbangnth.sHtML

T 其他语言补充                          60
来源：http://blog.fktsv.cn/Article/details/gphblqhly.sHtML

U 高频实用片段                         120
来源：http://www.share.vehdjk.com/Article/details/gdxyhcvlo.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gfpjtzpxv.sHtML

合计                                  2106 条
来源：http://mobile.yfazqb.com/Article/details/gvlbslnnv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/gnvtqfktc.sHtML


<!-- 参考信息 -->