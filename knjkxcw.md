代发 wailian999

case class User(name: String, age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/ggisggaae.sHtML

[T57] Scala：模式匹配
来源：http://blog.yfazqb.com/Article/details/guuxctdhf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.yfazqb.com/Article/details/gpwhrwval.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fktsv.cn/Article/details/ghoqwmiev.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.tarul.cn/Article/details/gqilirplo.sHtML

[T59] Scala：循环
来源：http://wap.yfazqb.com/Article/details/gtjbmhrta.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.epnwcf.com/Article/details/gjrulknvk.sHtML

[T60] Scala：折叠
来源：http://mobile.vehdjk.com/Article/details/gonbqiycm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.epnwcf.com/Article/details/gxvbxccrl.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/glkolfkfa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fktsv.cn/Article/details/gbrhizeuj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gixaohsyd.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.tarul.cn/Article/details/grvenjtnm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gqitusare.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.vehdjk.com/Article/details/glvekesfs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.tarul.cn/Article/details/gnpmmqwtq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.bbcook.cn/Article/details/gpjesjnan.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.vehdjk.com/Article/details/gvnahygcp.sHtML

[U04] Py：变量调试打印
来源：http://m.share.vehdjk.com/Article/details/gdfasffmr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fktsv.cn/Article/details/glmyacorv.sHtML

[U05] Py：列表去重且保序
来源：http://baike.vehdjk.com/Article/details/gakbkcwvd.sHtML

list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/glxuvrkaj.sHtML

[U06] Py：合并两个字典
来源：http://mobile.sjlbkw.cn/Article/details/gxsbqvlim.sHtML

{**a, **b}
来源：http://www.share.tarul.cn/Article/details/gznmbcjul.sHtML

[U07] Py：反转字典键值
来源：http://mobile.sjlbkw.cn/Article/details/guwyimcea.sHtML

{v: k for k, v in d.items()}
来源：http://blog.epnwcf.com/Article/details/gymmbqbtt.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.tarul.cn/Article/details/gfcwjpzfk.sHtML

[y for x in nested for y in x]
来源：http://3g.tarul.cn/Article/details/guidltysa.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.epnwcf.com/Article/details/geyfrulqe.sHtML

max(d, key=d.get)
来源：http://3g.tarul.cn/Article/details/goflopycz.sHtML

[U10] Py：按值排序字典
来源：http://mobile.vehdjk.com/Article/details/gfjkuhebr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.epnwcf.com/Article/details/gbjwqzijc.sHtML

[U11] Py：生成器表达式
来源：http://blog.fktsv.cn/Article/details/grejoslll.sHtML

(x * 2 for x in arr)
来源：http://blog.sjlbkw.cn/Article/details/gsrsmwpqv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.yfazqb.com/Article/details/goowgdepx.sHtML

Counter(arr).most_common(3)
来源：http://read.share.vehdjk.com/Article/details/ggcyvaahx.sHtML

[U13] Py：固定长度队列
来源：http://baike.epnwcf.com/Article/details/gsvwifrjp.sHtML

deque(maxlen=10)
来源：http://www.m.share.yfazqb.com/Article/details/goiiwtvem.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.epnwcf.com/Article/details/gmlklrbra.sHtML

defaultdict(list)
来源：http://blog.bbcook.cn/Article/details/gauddgxwe.sHtML

[U15] Py：高精度计时
来源：http://mobile.yfazqb.com/Article/details/gugnrospd.sHtML

t = time.perf_counter()
来源：http://www.m.share.yfazqb.com/Article/details/gafkkyewa.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fktsv.cn/Article/details/ggnqlknvm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.yfazqb.com/Article/details/gvrhakjow.sHtML

[U17] Py：初始化日志
来源：http://mobile.sjlbkw.cn/Article/details/gugopqjdm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/gpleryapb.sHtML

[U18] Py：预编译正则
来源：http://3g.vehdjk.com/Article/details/gqortrvtv.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.tarul.cn/Article/details/gjkmtpjfi.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.bbcook.cn/Article/details/gtblnrary.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.epnwcf.com/Article/details/gdpqjictr.sHtML

[U20] Py：缓存函数结果
来源：http://3g.vehdjk.com/Article/details/geklmgtdd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.epnwcf.com/Article/details/gbmdpwzjb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.sjlbkw.cn/Article/details/gxanxiqha.sHtML

@contextlib.contextmanager
来源：http://mobile.bbcook.cn/Article/details/gzcrxunfv.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.vehdjk.com/Article/details/gqyktoqer.sHtML

list(zip(*m))
来源：http://m.share.bbcook.cn/Article/details/guyzabwbh.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.vehdjk.com/Article/details/gztzkylwd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.vehdjk.com/Article/details/gfsujodwq.sHtML

[U24] Py：路径操作
来源：http://wap.yfazqb.com/Article/details/gvpdhpbtq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gzwvxtfyp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.sjlbkw.cn/Article/details/gfmaavosw.sHtML

csv.DictReader(f)
来源：http://mobile.vehdjk.com/Article/details/gdgfeludn.sHtML

[U26] Py：并发下载
来源：http://www.share.bbcook.cn/Article/details/gmkknldnd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.yfazqb.com/Article/details/guyzhnwca.sHtML

[U27] Py：异步 HTTP
来源：http://3g.sjlbkw.cn/Article/details/gzmseydck.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.tarul.cn/Article/details/gbfhjiqbm.sHtML

[U28] Py：类型别名
来源：http://3g.tarul.cn/Article/details/gbjqvgxtl.sHtML

UserId = int
来源：http://www.blog.sjlbkw.cn/Article/details/gcrctjtlz.sHtML

[U29] Py：属性校验
来源：http://blog.bbcook.cn/Article/details/gtpbuxdxd.sHtML

@property 与 @x.setter 配合
来源：http://3g.fktsv.cn/Article/details/ggknnxeqe.sHtML

[U30] Py：数据类
来源：http://www.share.epnwcf.com/Article/details/ghwujqiyl.sHtML

@dataclass(slots=True)
来源：http://wap.tarul.cn/Article/details/gvovfcshx.sHtML

[U31] Py：单测
来源：http://www.m.share.bbcook.cn/Article/details/guabtgyig.sHtML

python -m pytest -q
来源：http://read.share.tarul.cn/Article/details/gxtkmyaae.sHtML

[U32] Py：代码格式化
来源：http://blog.vehdjk.com/Article/details/gdhdnlcsb.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fktsv.cn/Article/details/geizkmvry.sHtML

[U33] Py：打包发布
来源：http://baike.bbcook.cn/Article/details/gopgcqati.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.yfazqb.com/Article/details/giyglacdm.sHtML

[U34] Py：判断编码
来源：http://www.share.epnwcf.com/Article/details/gugzddyoy.sHtML

chardet.detect(raw)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqpztxzx.sHtML

[U35] Py：发送邮件
来源：http://blog.tarul.cn/Article/details/goisoibgi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.vehdjk.com/Article/details/goithkqmn.sHtML

[U36] Py：定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gcsjsdbhp.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.vehdjk.com/Article/details/gibrctvlu.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/gacxnbkxa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.yfazqb.com/Article/details/gfpgididt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.vehdjk.com/Article/details/gsjuryzua.sHtML

Path(__file__).resolve().parent
来源：http://mobile.epnwcf.com/Article/details/ghgjketxq.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.tarul.cn/Article/details/gbpdmmwzb.sHtML

sys.stdout.isatty()
来源：http://www.share.fktsv.cn/Article/details/ggvdwlkyc.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.epnwcf.com/Article/details/gdhurewet.sHtML

print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/guywgcmlu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.tarul.cn/Article/details/gtntuxvuy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.epnwcf.com/Article/details/gdvtxadhp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.epnwcf.com/Article/details/glptjwrbg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fktsv.cn/Article/details/gcreznjeg.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.bbcook.cn/Article/details/gjrmmyvnf.sHtML

namespace App\Http;
来源：http://3g.yfazqb.com/Article/details/gqyqrqtis.sHtML

[U44] PHP：开启严格类型
来源：http://3g.yfazqb.com/Article/details/gbekfhxet.sHtML

declare(strict_types=1);
来源：http://read.share.fktsv.cn/Article/details/guvwgjwrb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.vehdjk.com/Article/details/gwszksuyg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcsosnet.sHtML

[U46] PHP：可空类型
来源：http://m.share.yfazqb.com/Article/details/gveluffeb.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gsznxtvio.sHtML

[U47] PHP：联合类型
来源：http://m.share.tarul.cn/Article/details/gznabcpqv.sHtML

int|string $id
来源：http://baike.epnwcf.com/Article/details/gvvdeqttr.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fktsv.cn/Article/details/gfewmztdg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.yfazqb.com/Article/details/gwkvdynqn.sHtML

[U49] PHP：只读属性
来源：http://m.share.vehdjk.com/Article/details/gojblpbih.sHtML

public readonly string $name
来源：http://wap.bbcook.cn/Article/details/gkaoviwyd.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.sjlbkw.cn/Article/details/gtbvjcupx.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.yfazqb.com/Article/details/gszndlejq.sHtML

[U51] PHP：数组解构
来源：http://mobile.bbcook.cn/Article/details/gkqoelmlr.sHtML

[$a, $b] = $arr;
来源：http://www.share.sjlbkw.cn/Article/details/goeaoeulp.sHtML

[U52] PHP：箭头函数
来源：http://www.share.bbcook.cn/Article/details/grljikofv.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.epnwcf.com/Article/details/ggzfgcwlr.sHtML

[U53] PHP：空合并运算符
来源：http://3g.epnwcf.com/Article/details/gjoleljek.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.bbcook.cn/Article/details/gibznjosv.sHtML

[U54] PHP：空安全调用
来源：http://baike.tarul.cn/Article/details/gmgvvblej.sHtML

$obj?->method()
来源：http://www.m.share.vehdjk.com/Article/details/gxmajrmsj.sHtML

[U55] PHP：match 表达式
来源：http://wap.epnwcf.com/Article/details/gevccsjcx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.yfazqb.com/Article/details/ggjngwuan.sHtML

[U56] PHP：命名参数
来源：http://www.blog.vehdjk.com/Article/details/gqkevtfvt.sHtML

f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gjvgmnfct.sHtML

[U57] PHP：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gdbwqcuey.sHtML

"值: {$a}"
来源：http://wap.sjlbkw.cn/Article/details/giyewauwj.sHtML

[U58] PHP：数组三件套
来源：http://www.share.epnwcf.com/Article/details/gcfaihavp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fktsv.cn/Article/details/glxqsdzog.sHtML

[U59] PHP：自定义排序
来源：http://3g.fktsv.cn/Article/details/gvnmyexsu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/ghwzszmdd.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.vehdjk.com/Article/details/gbfhdrbny.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.tarul.cn/Article/details/gttahidkb.sHtML

[U61] PHP：正则
来源：http://baike.sjlbkw.cn/Article/details/goqhzohaf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.yfazqb.com/Article/details/gzrsdlzhm.sHtML

[U62] PHP：日期对象
来源：http://read.share.epnwcf.com/Article/details/ghtbbcdnn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.tarul.cn/Article/details/gmsuzxqkf.sHtML

[U63] PHP：文件读写
来源：http://www.blog.vehdjk.com/Article/details/gguhifjsf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.vehdjk.com/Article/details/guyigovxl.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fktsv.cn/Article/details/gqpciodjh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fktsv.cn/Article/details/ggzapmirp.sHtML

[U65] PHP：会话
来源：http://blog.epnwcf.com/Article/details/gphvqljcd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.bbcook.cn/Article/details/glwkcexbd.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.bbcook.cn/Article/details/gwljpvxco.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.epnwcf.com/Article/details/gojegqcvv.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.yfazqb.com/Article/details/gdbxeywce.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.sjlbkw.cn/Article/details/gcaozqysu.sHtML

[U68] PHP：PDO 连接
来源：http://wap.bbcook.cn/Article/details/gpuxpijdh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.yfazqb.com/Article/details/gxxcdludd.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.sjlbkw.cn/Article/details/guelnuyfc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.yfazqb.com/Article/details/gizkpvque.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.bbcook.cn/Article/details/ggfmnzonj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fktsv.cn/Article/details/glnxcqwkt.sHtML

[U71] PHP：抛出异常
来源：http://wap.vehdjk.com/Article/details/gqhesjzfd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.epnwcf.com/Article/details/gqcmlxemk.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fktsv.cn/Article/details/gyzcljnmf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaieozwl.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.epnwcf.com/Article/details/gfiakxvfp.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.bbcook.cn/Article/details/gcbjepvfm.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.tarul.cn/Article/details/gnnnbhatp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.vehdjk.com/Article/details/gxrqqclxf.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.bbcook.cn/Article/details/gbgwlahon.sHtML

composer require psr/container
来源：http://www.blog.epnwcf.com/Article/details/gbqraulpp.sHtML

[U76] PHP：简单路由
来源：http://wap.bbcook.cn/Article/details/gjlcnwdpm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.vehdjk.com/Article/details/gdujkwfeb.sHtML

[U77] PHP：模板渲染
来源：http://baike.epnwcf.com/Article/details/gvmrphsfq.sHtML

composer require twig/twig
来源：http://www.m.share.sjlbkw.cn/Article/details/gidxqqwuh.sHtML

[U78] PHP：单元测试
来源：http://baike.sjlbkw.cn/Article/details/gflhlaylc.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.bbcook.cn/Article/details/gpifjaqdc.sHtML

[U79] PHP：静态分析
来源：http://wap.bbcook.cn/Article/details/guoficrvi.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fktsv.cn/Article/details/gttulfkep.sHtML

[U80] PHP：代码规范修复
来源：http://3g.vehdjk.com/Article/details/gonvpmzgv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.tarul.cn/Article/details/gugbrtghy.sHtML

[U81] JS：初始化项目
来源：http://m.share.epnwcf.com/Article/details/gmdmwvvya.sHtML

npm init -y;  npm i express
来源：http://3g.epnwcf.com/Article/details/gpywrguhn.sHtML

[U82] JS：package.json 脚本
来源：http://blog.epnwcf.com/Article/details/gtrlrwbmr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.tarul.cn/Article/details/gmewmbpec.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.vehdjk.com/Article/details/glcwpwdlb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gfixeyudx.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.bbcook.cn/Article/details/gluvrthkl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.sjlbkw.cn/Article/details/gwwzuvnso.sHtML

[U85] JS：可选链
来源：http://blog.bbcook.cn/Article/details/gaowqglok.sHtML

a?.b?.c
来源：http://wap.fktsv.cn/Article/details/gxgjyeafi.sHtML

[U86] JS：空值合并
来源：http://baike.vehdjk.com/Article/details/gdxxixdea.sHtML

a ?? b
来源：http://3g.bbcook.cn/Article/details/gahaqnpyn.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fktsv.cn/Article/details/geujtjfta.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fktsv.cn/Article/details/gpxfvotyx.sHtML

[U88] JS：对象展开合并
来源：http://baike.tarul.cn/Article/details/gvryjnitm.sHtML

{ ...a, ...b }
来源：http://wap.tarul.cn/Article/details/gkrcnlkzn.sHtML

[U89] JS：数组去重
来源：http://wap.bbcook.cn/Article/details/giaimcwdg.sHtML

[...new Set(arr)]
来源：http://blog.yfazqb.com/Article/details/gnijtlszz.sHtML

[U90] JS：数字数组排序
来源：http://wap.vehdjk.com/Article/details/ggfnwgjgh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gggvgvoqq.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.yfazqb.com/Article/details/giuaoxcve.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fktsv.cn/Article/details/gnyaklowc.sHtML

[U92] JS：深拷贝
来源：http://www.share.bbcook.cn/Article/details/gzvmrvhcw.sHtML

structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/glnveiuve.sHtML

[U93] JS：模板字符串
来源：http://mobile.tarul.cn/Article/details/gnxrwduad.sHtML

`共 ${n} 条`
来源：http://mobile.sjlbkw.cn/Article/details/ggufqihwr.sHtML

[U94] JS：箭头函数
来源：http://blog.fktsv.cn/Article/details/grjbrmvoj.sHtML

const double = x => x * 2;
来源：http://read.share.yfazqb.com/Article/details/geerdjljs.sHtML

[U95] JS：Promise 包装
来源：http://wap.bbcook.cn/Article/details/ghsezviqa.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.yfazqb.com/Article/details/ghztbphze.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.bbcook.cn/Article/details/gtwxzerwt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gffywebqj.sHtML

[U97] JS：并发请求
来源：http://3g.tarul.cn/Article/details/gnvwmihge.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gwefjycyx.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.yfazqb.com/Article/details/gnoeydypu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.vehdjk.com/Article/details/gzwqdeuoq.sHtML

[U99] JS：事件监听
来源：http://www.blog.yfazqb.com/Article/details/ghkbgqjsc.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fktsv.cn/Article/details/gpqqofqqb.sHtML

[U100] JS：DOM 查询
来源：http://read.share.tarul.cn/Article/details/gvxeubyic.sHtML

document.querySelector(".item")
来源：http://baike.tarul.cn/Article/details/gkesermfu.sHtML

[U101] JS：classList 操作
来源：http://read.share.fktsv.cn/Article/details/geoqktpko.sHtML

el.classList.toggle("active")
来源：http://wap.sjlbkw.cn/Article/details/gbomfghyy.sHtML

[U102] JS：本地存储
来源：http://read.share.yfazqb.com/Article/details/gmofcxnyf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.tarul.cn/Article/details/ggvjtfffa.sHtML

[U103] JS：定时器
来源：http://www.blog.sjlbkw.cn/Article/details/gpidhvfso.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.epnwcf.com/Article/details/gvgywvlhh.sHtML

[U104] JS：防抖
来源：http://www.share.epnwcf.com/Article/details/gtyagvauc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gimhinunk.sHtML

[U105] JS：节流
来源：http://baike.bbcook.cn/Article/details/ggldigecl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.yfazqb.com/Article/details/grvnweaik.sHtML

[U106] JS：日期格式化
来源：http://blog.epnwcf.com/Article/details/gmhvuaymf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.bbcook.cn/Article/details/gabnfdksa.sHtML

[U107] JS：数字千分位
来源：http://baike.yfazqb.com/Article/details/ggchvnloh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.tarul.cn/Article/details/gzasiifan.sHtML

[U108] JS：随机整数
来源：http://mobile.vehdjk.com/Article/details/gyocryzbd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.vehdjk.com/Article/details/gnjyochja.sHtML

[U109] JS：数组分组
来源：http://www.blog.fktsv.cn/Article/details/gxaayowxd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gjzmlibaj.sHtML

[U110] JS：数组分块
来源：http://blog.epnwcf.com/Article/details/ggfoahjnf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.epnwcf.com/Article/details/gteceswfs.sHtML

[U111] JS：对象转 Map
来源：http://mobile.tarul.cn/Article/details/gvnbtnmwu.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.sjlbkw.cn/Article/details/gqhplhiyf.sHtML

[U112] JS：字符串补位
来源：http://wap.yfazqb.com/Article/details/ginxqdpdo.sHtML

"7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gvahbyiib.sHtML

[U113] JS：正则替换全部
来源：http://mobile.bbcook.cn/Article/details/gllfhyoiw.sHtML

s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gynlscxws.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gprgiyoal.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gmywccrpo.sHtML

[U115] JS：生成 UUID
来源：http://3g.fktsv.cn/Article/details/gxnkqsgxi.sHtML

crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gpvuczciv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.sjlbkw.cn/Article/details/gfwikbich.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.vehdjk.com/Article/details/gaxdbvcma.sHtML

[U117] JS：单元测试
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcuyndyy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.tarul.cn/Article/details/gtqaraiar.sHtML

[U118] JS：开发服务器
来源：http://m.share.yfazqb.com/Article/details/gqimwawjj.sHtML

npm i -D vite;  npx vite
来源：http://read.share.epnwcf.com/Article/details/gsyzcuwfz.sHtML

[U119] JS：生产构建
来源：http://mobile.yfazqb.com/Article/details/gksbvwzhp.sHtML

npx vite build
来源：http://mobile.vehdjk.com/Article/details/gbnsifril.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.tarul.cn/Article/details/gqjehxssj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.vehdjk.com/Article/details/gshamkmuk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gizpgewit.sHtML

统计汇总
来源：http://wap.vehdjk.com/Article/details/gglcnfajc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gflfednmw.sHtML

按语言统计（条）：
来源：http://read.share.fktsv.cn/Article/details/gfwdcbpov.sHtML

Python ......... 252
来源：http://baike.epnwcf.com/Article/details/glfimphjn.sHtML

PHP ............ 252
来源：http://www.share.bbcook.cn/Article/details/gfgbvlitb.sHtML

JavaScript ..... 252
来源：http://wap.bbcook.cn/Article/details/gbzznuzcv.sHtML

TypeScript ..... 212
来源：http://wap.bbcook.cn/Article/details/gqelsryjv.sHtML

Java ........... 212
来源：http://m.share.fktsv.cn/Article/details/giasqvuom.sHtML

Go ............. 212
来源：http://3g.sjlbkw.cn/Article/details/gvqpvbexn.sHtML

Ruby ........... 212
来源：http://www.share.tarul.cn/Article/details/gdednekju.sHtML

C# ............. 212
来源：http://read.share.vehdjk.com/Article/details/gcbnzeqae.sHtML

C .............. 30
来源：http://www.share.vehdjk.com/Article/details/gjdmixpjm.sHtML

C++ ............ 30
来源：http://3g.yfazqb.com/Article/details/glgltcjep.sHtML

SQL ............ 90
来源：http://read.share.tarul.cn/Article/details/gemttkmie.sHtML

Bash ........... 80
来源：http://www.m.share.yfazqb.com/Article/details/gbibgryir.sHtML

Kotlin ......... 15
来源：http://3g.bbcook.cn/Article/details/gqzbhrgej.sHtML

Swift .......... 15
来源：http://baike.vehdjk.com/Article/details/gnadswpoe.sHtML

Lua ............ 10
来源：http://blog.bbcook.cn/Article/details/gibxyaoly.sHtML

Perl ........... 10
来源：http://wap.yfazqb.com/Article/details/gvfegmjhh.sHtML

Scala .......... 10
来源：http://www.m.share.yfazqb.com/Article/details/gqhhlcses.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/gkrnfcfpn.sHtML

合计 ........... 2106 条
来源：http://blog.sjlbkw.cn/Article/details/gmuzrcwxc.sHtML

按章节统计：
来源：http://www.m.share.bbcook.cn/Article/details/gwxcgdkac.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fktsv.cn/Article/details/gnwceqfpv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/grqfblxcp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/ghbmoegzz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/glwcaggxw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.yfazqb.com/Article/details/gsgxmpzyr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.bbcook.cn/Article/details/gmxgbmkdl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gaimjdwlw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.bbcook.cn/Article/details/gpxhehizs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gbxmxlsjx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.yfazqb.com/Article/details/gjkgkimrr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gpijhvyps.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/giyhnaorm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gksqcgqvm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fktsv.cn/Article/details/gtxtaoibe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.epnwcf.com/Article/details/glbgapwvb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gxzibehyb.sHtML

Q SQL 专题                              90
来源：http://3g.sjlbkw.cn/Article/details/gjsdsgjdv.sHtML

R Bash 专题                             80
来源：http://m.share.yfazqb.com/Article/details/gjsegrbdf.sHtML

S C / C++ 专题                          60
来源：http://3g.sjlbkw.cn/Article/details/gfbhlykpi.sHtML

T 其他语言补充                          60
来源：http://www.share.fktsv.cn/Article/details/gxnuowugk.sHtML

U 高频实用片段                         120
来源：http://www.share.sjlbkw.cn/Article/details/gwuviejou.sHtML

------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gryoenchs.sHtML

合计                                  2106 条
来源：http://mobile.vehdjk.com/Article/details/gzktlawuo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gdmjpvzqu.sHtML


<!-- 参考信息 -->