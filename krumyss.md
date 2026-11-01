代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://blog.vehdjk.com/Article/details/gwqsxygls.sHtML

[T59] Scala：循环
来源：http://blog.yfazqb.com/Article/details/gmmdhttxj.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.bbcook.cn/Article/details/gsrpftjrt.sHtML

[T60] Scala：折叠
来源：http://baike.tarul.cn/Article/details/gmtagcbti.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.tarul.cn/Article/details/gdvwzqten.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gajhsrmcd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/gkoiwefmw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gijcefeoq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.epnwcf.com/Article/details/gpofvukjz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fktsv.cn/Article/details/ggwscceua.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.sjlbkw.cn/Article/details/ghutddktg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.sjlbkw.cn/Article/details/ghrhqyrdw.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.vehdjk.com/Article/details/gmlenxwbu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fktsv.cn/Article/details/gvyvzlmob.sHtML

[U04] Py：变量调试打印
来源：http://wap.fktsv.cn/Article/details/gxntyhiqi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.tarul.cn/Article/details/gzakfokkx.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.yfazqb.com/Article/details/gfwkpykkp.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gxjnkynuw.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fktsv.cn/Article/details/gmcytqvcz.sHtML

{**a, **b}
来源：http://wap.bbcook.cn/Article/details/gscfddaez.sHtML

[U07] Py：反转字典键值
来源：http://3g.fktsv.cn/Article/details/glzluormu.sHtML

{v: k for k, v in d.items()}
来源：http://blog.vehdjk.com/Article/details/gehytswuc.sHtML

[U08] Py：展平二维列表
来源：http://www.share.tarul.cn/Article/details/grercbtel.sHtML

[y for x in nested for y in x]
来源：http://mobile.sjlbkw.cn/Article/details/gckjtxlqp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.yfazqb.com/Article/details/gvbqkvqra.sHtML

max(d, key=d.get)
来源：http://mobile.epnwcf.com/Article/details/gyfijdyth.sHtML

[U10] Py：按值排序字典
来源：http://blog.bbcook.cn/Article/details/gnhgcebpl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.yfazqb.com/Article/details/gjxhdkjtf.sHtML

[U11] Py：生成器表达式
来源：http://3g.fktsv.cn/Article/details/ggpcnohpx.sHtML

(x * 2 for x in arr)
来源：http://wap.tarul.cn/Article/details/gjoqsdypc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fktsv.cn/Article/details/gulhdmxwx.sHtML

Counter(arr).most_common(3)
来源：http://wap.tarul.cn/Article/details/gcvbkehrz.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.yfazqb.com/Article/details/gdxkpkuml.sHtML

deque(maxlen=10)
来源：http://m.share.yfazqb.com/Article/details/gdvoqjxom.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.vehdjk.com/Article/details/gadnuwbuz.sHtML

defaultdict(list)
来源：http://baike.sjlbkw.cn/Article/details/gkpyfhpje.sHtML

[U15] Py：高精度计时
来源：http://m.share.sjlbkw.cn/Article/details/gdmtdhkmw.sHtML

t = time.perf_counter()
来源：http://baike.tarul.cn/Article/details/gsmyklrtx.sHtML

[U16] Py：命令行参数解析
来源：http://3g.sjlbkw.cn/Article/details/gqgmoydpo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.epnwcf.com/Article/details/gzdabfbln.sHtML

[U17] Py：初始化日志
来源：http://read.share.yfazqb.com/Article/details/gnqglnuuu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.vehdjk.com/Article/details/gzplqbnxm.sHtML

[U18] Py：预编译正则
来源：http://3g.epnwcf.com/Article/details/gpdwtaiuz.sHtML

pat = re.compile(r"\d+")
来源：http://baike.vehdjk.com/Article/details/gtmiafrmq.sHtML

[U19] Py：正则替换带回调
来源：http://3g.epnwcf.com/Article/details/gbwjghaaz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.yfazqb.com/Article/details/gnsdpwvon.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.bbcook.cn/Article/details/gvtbwapoq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.yfazqb.com/Article/details/gqnmgglnt.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.tarul.cn/Article/details/gtgrhqndc.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/gcslksraq.sHtML

[U22] Py：矩阵转置
来源：http://read.share.bbcook.cn/Article/details/gzbjkvdol.sHtML

list(zip(*m))
来源：http://m.share.tarul.cn/Article/details/gzzwddwxj.sHtML

[U23] Py：分块读取大文件
来源：http://wap.tarul.cn/Article/details/gxikgtsks.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.epnwcf.com/Article/details/gflojoicj.sHtML

[U24] Py：路径操作
来源：http://www.m.share.vehdjk.com/Article/details/gjuoktdmh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gjzllaegl.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.bbcook.cn/Article/details/gqgxiefup.sHtML

csv.DictReader(f)
来源：http://blog.fktsv.cn/Article/details/grygybpyd.sHtML

[U26] Py：并发下载
来源：http://mobile.sjlbkw.cn/Article/details/gfgkoqfev.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.epnwcf.com/Article/details/gdunupwig.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.yfazqb.com/Article/details/gbtmnnzgs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.epnwcf.com/Article/details/glenmvohg.sHtML

[U28] Py：类型别名
来源：http://wap.sjlbkw.cn/Article/details/gjaxmpaib.sHtML

UserId = int
来源：http://blog.epnwcf.com/Article/details/gwmsqmomn.sHtML

[U29] Py：属性校验
来源：http://mobile.yfazqb.com/Article/details/gbrihmhfa.sHtML

@property 与 @x.setter 配合
来源：http://baike.tarul.cn/Article/details/gxktxqfbi.sHtML

[U30] Py：数据类
来源：http://www.m.share.yfazqb.com/Article/details/gdyqcpljy.sHtML

@dataclass(slots=True)
来源：http://3g.vehdjk.com/Article/details/gxtbluvli.sHtML

[U31] Py：单测
来源：http://www.m.share.vehdjk.com/Article/details/gzyaepsyf.sHtML

python -m pytest -q
来源：http://read.share.yfazqb.com/Article/details/gtnfrjeoh.sHtML

[U32] Py：代码格式化
来源：http://m.share.fktsv.cn/Article/details/gbjjksrdc.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.sjlbkw.cn/Article/details/gbvmmgyau.sHtML

[U33] Py：打包发布
来源：http://mobile.yfazqb.com/Article/details/gvzmbyrht.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.tarul.cn/Article/details/gqjkhpkaf.sHtML

[U34] Py：判断编码
来源：http://blog.bbcook.cn/Article/details/gsadvdghj.sHtML

chardet.detect(raw)
来源：http://www.m.share.yfazqb.com/Article/details/gnrchakqt.sHtML

[U35] Py：发送邮件
来源：http://read.share.tarul.cn/Article/details/grjtguhvs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.yfazqb.com/Article/details/gdjlqolnw.sHtML

[U36] Py：定时任务
来源：http://read.share.bbcook.cn/Article/details/gmzzeorij.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fktsv.cn/Article/details/gqebhddyd.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.sjlbkw.cn/Article/details/glihspjjp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.yfazqb.com/Article/details/gkvdladex.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.bbcook.cn/Article/details/gohgxuqtb.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.tarul.cn/Article/details/gapjnerjb.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.bbcook.cn/Article/details/gzjcqbtnt.sHtML

sys.stdout.isatty()
来源：http://3g.sjlbkw.cn/Article/details/gezhtoyiu.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fktsv.cn/Article/details/giozbvcya.sHtML

print("err", file=sys.stderr)
来源：http://wap.epnwcf.com/Article/details/gjjyxagnc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.epnwcf.com/Article/details/gyagocytm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.epnwcf.com/Article/details/gskdrppsv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.vehdjk.com/Article/details/gmkuekaag.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.vehdjk.com/Article/details/gtdnztbka.sHtML

[U43] PHP：声明命名空间
来源：http://3g.sjlbkw.cn/Article/details/gvitgaubj.sHtML

namespace App\Http;
来源：http://www.blog.vehdjk.com/Article/details/ghqbdlhjm.sHtML

[U44] PHP：开启严格类型
来源：http://blog.epnwcf.com/Article/details/gpbywfaqz.sHtML

declare(strict_types=1);
来源：http://blog.yfazqb.com/Article/details/gytxwmdgt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.tarul.cn/Article/details/gyoypeeni.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gnxcohtem.sHtML

[U46] PHP：可空类型
来源：http://www.blog.yfazqb.com/Article/details/gymayhlhg.sHtML

?string $name = null
来源：http://baike.tarul.cn/Article/details/gcathdvst.sHtML

[U47] PHP：联合类型
来源：http://blog.bbcook.cn/Article/details/guleuxlmi.sHtML

int|string $id
来源：http://wap.sjlbkw.cn/Article/details/gckkstspw.sHtML

[U48] PHP：纯枚举
来源：http://baike.sjlbkw.cn/Article/details/gdgebpksd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.sjlbkw.cn/Article/details/gfkaqrzbu.sHtML

[U49] PHP：只读属性
来源：http://blog.yfazqb.com/Article/details/gikhueiic.sHtML

public readonly string $name
来源：http://www.m.share.fktsv.cn/Article/details/gxzjijuit.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.tarul.cn/Article/details/gxvyufpno.sHtML

public function __construct(private int $id) {}
来源：http://mobile.yfazqb.com/Article/details/gszaucjyz.sHtML

[U51] PHP：数组解构
来源：http://baike.sjlbkw.cn/Article/details/grmtptekw.sHtML

[$a, $b] = $arr;
来源：http://baike.epnwcf.com/Article/details/guyqarpeq.sHtML

[U52] PHP：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gwprvkmws.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.vehdjk.com/Article/details/gaiivacik.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.vehdjk.com/Article/details/gikdvdyjg.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.tarul.cn/Article/details/gfdwatpte.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fktsv.cn/Article/details/gmchjxccs.sHtML

$obj?->method()
来源：http://3g.vehdjk.com/Article/details/gjkyxfebg.sHtML

[U55] PHP：match 表达式
来源：http://www.share.yfazqb.com/Article/details/gcipkdwpg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.tarul.cn/Article/details/gelvbjqti.sHtML

[U56] PHP：命名参数
来源：http://wap.vehdjk.com/Article/details/glsubxznx.sHtML

f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gwhrehaoz.sHtML

[U57] PHP：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gapsohpch.sHtML

"值: {$a}"
来源：http://www.share.yfazqb.com/Article/details/gqipnezvm.sHtML

[U58] PHP：数组三件套
来源：http://blog.fktsv.cn/Article/details/gzvqqjoug.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.bbcook.cn/Article/details/ghjkrfoqq.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.yfazqb.com/Article/details/gpraqxzsk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/gruyhkqbf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.tarul.cn/Article/details/glipdolsf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.bbcook.cn/Article/details/gejyjtzex.sHtML

[U61] PHP：正则
来源：http://www.share.epnwcf.com/Article/details/gwelvhvij.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gpvrqdinb.sHtML

[U62] PHP：日期对象
来源：http://read.share.sjlbkw.cn/Article/details/gzxbnkuse.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.epnwcf.com/Article/details/gujkifewh.sHtML

[U63] PHP：文件读写
来源：http://wap.epnwcf.com/Article/details/gclfrerqe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.epnwcf.com/Article/details/gccpodcty.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.epnwcf.com/Article/details/guqclyntq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.epnwcf.com/Article/details/gtugxbbnk.sHtML

[U65] PHP：会话
来源：http://m.share.yfazqb.com/Article/details/ggbbjmsbq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gpfzrgnrt.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.bbcook.cn/Article/details/gawitnfjf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.sjlbkw.cn/Article/details/gbpohpnyb.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.sjlbkw.cn/Article/details/gjmaktlyp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.epnwcf.com/Article/details/gqcvpmhco.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.bbcook.cn/Article/details/gcevhapbv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.vehdjk.com/Article/details/gcqckihmg.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.tarul.cn/Article/details/gqettvsvp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.vehdjk.com/Article/details/gcipztihh.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fktsv.cn/Article/details/glpwkgxbx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.yfazqb.com/Article/details/gxrxpfwby.sHtML

[U71] PHP：抛出异常
来源：http://mobile.bbcook.cn/Article/details/guyrgbzex.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.tarul.cn/Article/details/gefujpqtr.sHtML

[U72] PHP：写错误日志
来源：http://mobile.epnwcf.com/Article/details/gwpzftekr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.vehdjk.com/Article/details/gtejqypil.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.tarul.cn/Article/details/gbbvstdfn.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fktsv.cn/Article/details/gsrrghkgo.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/ghrqstkes.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.yfazqb.com/Article/details/glkvxjplx.sHtML

[U75] PHP：依赖注入
来源：http://mobile.tarul.cn/Article/details/gxrbgjoin.sHtML

composer require psr/container
来源：http://baike.yfazqb.com/Article/details/ghtmhnbsi.sHtML

[U76] PHP：简单路由
来源：http://www.share.yfazqb.com/Article/details/gpmososay.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.tarul.cn/Article/details/ghizywwyb.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.tarul.cn/Article/details/ggchxiuqe.sHtML

composer require twig/twig
来源：http://www.m.share.tarul.cn/Article/details/gkioezlvm.sHtML

[U78] PHP：单元测试
来源：http://www.blog.epnwcf.com/Article/details/ggmmneysj.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.bbcook.cn/Article/details/gzjudulwp.sHtML

[U79] PHP：静态分析
来源：http://blog.sjlbkw.cn/Article/details/gmcqxdyqv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.yfazqb.com/Article/details/ggyewzbfh.sHtML

[U80] PHP：代码规范修复
来源：http://blog.bbcook.cn/Article/details/gjrdrfxbz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.epnwcf.com/Article/details/glozwefyf.sHtML

[U81] JS：初始化项目
来源：http://www.blog.sjlbkw.cn/Article/details/gfupenzgj.sHtML

npm init -y;  npm i express
来源：http://m.share.epnwcf.com/Article/details/gxdenrcwx.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.sjlbkw.cn/Article/details/gdrsgyodp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.epnwcf.com/Article/details/gyjhybvfe.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.bbcook.cn/Article/details/glnkapmko.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fktsv.cn/Article/details/gqbdedqok.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.vehdjk.com/Article/details/gapnviyjf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.vehdjk.com/Article/details/gxtraudac.sHtML

[U85] JS：可选链
来源：http://m.share.bbcook.cn/Article/details/gmuchhrzs.sHtML

a?.b?.c
来源：http://www.share.epnwcf.com/Article/details/gsengpskb.sHtML

[U86] JS：空值合并
来源：http://3g.tarul.cn/Article/details/gnxgzpdqj.sHtML

a ?? b
来源：http://blog.vehdjk.com/Article/details/gpzfmqwuk.sHtML

[U87] JS：解构默认值
来源：http://www.blog.sjlbkw.cn/Article/details/gijhndptr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.epnwcf.com/Article/details/gqstnxgqe.sHtML

[U88] JS：对象展开合并
来源：http://3g.fktsv.cn/Article/details/ggqlmxlat.sHtML

{ ...a, ...b }
来源：http://mobile.vehdjk.com/Article/details/gqikhyekl.sHtML

[U89] JS：数组去重
来源：http://wap.vehdjk.com/Article/details/gkhuifvdx.sHtML

[...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gdjgvanjk.sHtML

[U90] JS：数字数组排序
来源：http://baike.bbcook.cn/Article/details/gtzytkiss.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gxgiegvxc.sHtML

[U91] JS：对象键值遍历
来源：http://3g.yfazqb.com/Article/details/gideqhbjz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.epnwcf.com/Article/details/gpexqwhdt.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.vehdjk.com/Article/details/goxscfiur.sHtML

structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gxzhctajp.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.epnwcf.com/Article/details/gpnsrvisn.sHtML

`共 ${n} 条`
来源：http://baike.tarul.cn/Article/details/gfeplnqak.sHtML

[U94] JS：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/giivpwomg.sHtML

const double = x => x * 2;
来源：http://www.blog.sjlbkw.cn/Article/details/gdauphmej.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fktsv.cn/Article/details/gmyibqykp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.bbcook.cn/Article/details/gzpckxrhc.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.tarul.cn/Article/details/gehylcbea.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/gzwhlwcnb.sHtML

[U97] JS：并发请求
来源：http://3g.sjlbkw.cn/Article/details/glwsqzszq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/ggwsoeisi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fktsv.cn/Article/details/gpfxexxff.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.vehdjk.com/Article/details/gbmjmhard.sHtML

[U99] JS：事件监听
来源：http://www.share.yfazqb.com/Article/details/gpfxoharp.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fktsv.cn/Article/details/gbvzpcpiv.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.vehdjk.com/Article/details/gxvhpdhpj.sHtML

document.querySelector(".item")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpovgluko.sHtML

[U101] JS：classList 操作
来源：http://wap.epnwcf.com/Article/details/gxavozmhj.sHtML

el.classList.toggle("active")
来源：http://mobile.bbcook.cn/Article/details/gyumaroso.sHtML

[U102] JS：本地存储
来源：http://www.blog.vehdjk.com/Article/details/gafvvsogb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.sjlbkw.cn/Article/details/gtrmlaztk.sHtML

[U103] JS：定时器
来源：http://mobile.yfazqb.com/Article/details/gjvvyasra.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.yfazqb.com/Article/details/gwozqyppg.sHtML

[U104] JS：防抖
来源：http://baike.sjlbkw.cn/Article/details/geovobssd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/glsbazdbr.sHtML

[U105] JS：节流
来源：http://m.share.bbcook.cn/Article/details/goxatreqk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.sjlbkw.cn/Article/details/gijmxadyl.sHtML

[U106] JS：日期格式化
来源：http://wap.epnwcf.com/Article/details/gezjwrlht.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.sjlbkw.cn/Article/details/gnnrinnlj.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fktsv.cn/Article/details/gjuinidkp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.bbcook.cn/Article/details/gfmyrbifz.sHtML

[U108] JS：随机整数
来源：http://m.share.bbcook.cn/Article/details/gmfjkwkee.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.sjlbkw.cn/Article/details/ggxjuifam.sHtML

[U109] JS：数组分组
来源：http://3g.tarul.cn/Article/details/gbyhbfsql.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fktsv.cn/Article/details/gxeooseed.sHtML

[U110] JS：数组分块
来源：http://www.blog.vehdjk.com/Article/details/gifeigffi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.vehdjk.com/Article/details/geggoofvy.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.bbcook.cn/Article/details/gadqshrtk.sHtML

new Map(Object.entries(obj))
来源：http://blog.tarul.cn/Article/details/geaxwzcse.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.tarul.cn/Article/details/gqcljyuvg.sHtML

"7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gkfgwndbq.sHtML

[U113] JS：正则替换全部
来源：http://read.share.yfazqb.com/Article/details/gtsawtksy.sHtML

s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gbmezbawl.sHtML

[U114] JS：JSON 深比较
来源：http://baike.epnwcf.com/Article/details/gpcdfiutd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.tarul.cn/Article/details/ggipicaja.sHtML

[U115] JS：生成 UUID
来源：http://blog.bbcook.cn/Article/details/goebovfbh.sHtML

crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gatjwbykq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.yfazqb.com/Article/details/gmtacmsfz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.bbcook.cn/Article/details/gknkmfroc.sHtML

[U117] JS：单元测试
来源：http://baike.fktsv.cn/Article/details/ghqcaixhl.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.tarul.cn/Article/details/gvdvhzmgw.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.yfazqb.com/Article/details/gmpjltbfz.sHtML

npm i -D vite;  npx vite
来源：http://read.share.tarul.cn/Article/details/gwtxrbrgv.sHtML

[U119] JS：生产构建
来源：http://mobile.bbcook.cn/Article/details/geiissgnb.sHtML

npx vite build
来源：http://www.share.epnwcf.com/Article/details/gufcrdpov.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.epnwcf.com/Article/details/ghffcjbkr.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.sjlbkw.cn/Article/details/gjlaeyhrk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gznlhgdbt.sHtML

统计汇总
来源：http://wap.bbcook.cn/Article/details/gnvepkfkp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdsxmzosl.sHtML

按语言统计（条）：
来源：http://mobile.yfazqb.com/Article/details/gmvezdwzv.sHtML

Python ......... 252
来源：http://read.share.vehdjk.com/Article/details/gfkkdbken.sHtML

PHP ............ 252
来源：http://3g.vehdjk.com/Article/details/gcpnambmh.sHtML

JavaScript ..... 252
来源：http://m.share.vehdjk.com/Article/details/ghowqaghi.sHtML

TypeScript ..... 212
来源：http://baike.yfazqb.com/Article/details/gdwnjjtse.sHtML

Java ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gduohgmgr.sHtML

Go ............. 212
来源：http://read.share.vehdjk.com/Article/details/gdpbanwlt.sHtML

Ruby ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gkkmwizwl.sHtML

C# ............. 212
来源：http://mobile.epnwcf.com/Article/details/gckwjntbt.sHtML

C .............. 30
来源：http://read.share.epnwcf.com/Article/details/ghslunfcp.sHtML

C++ ............ 30
来源：http://baike.sjlbkw.cn/Article/details/grjqzuqaz.sHtML

SQL ............ 90
来源：http://www.share.yfazqb.com/Article/details/gskchkbjn.sHtML

Bash ........... 80
来源：http://www.m.share.bbcook.cn/Article/details/gotqfmjzw.sHtML

Kotlin ......... 15
来源：http://3g.vehdjk.com/Article/details/grdmdgico.sHtML

Swift .......... 15
来源：http://www.share.bbcook.cn/Article/details/grczgqpny.sHtML

Lua ............ 10
来源：http://www.blog.bbcook.cn/Article/details/gjehwbraz.sHtML

Perl ........... 10
来源：http://blog.bbcook.cn/Article/details/gzxfukfvl.sHtML

Scala .......... 10
来源：http://www.blog.bbcook.cn/Article/details/gbcahmdcl.sHtML

------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gavthmnjv.sHtML

合计 ........... 2106 条
来源：http://baike.bbcook.cn/Article/details/grspswodm.sHtML

按章节统计：
来源：http://3g.tarul.cn/Article/details/geukgqcpo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.sjlbkw.cn/Article/details/ggzepodoz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/gjkhclbdz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/ghtjapgbc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/grmlpblll.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.epnwcf.com/Article/details/gndptasip.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.epnwcf.com/Article/details/glkvpbxcz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/gxylvkzah.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.yfazqb.com/Article/details/grhizxtib.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvdwqeyx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/gvbixqzfz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/grsvicnti.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/ggntlaapu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gsefpjmvp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fktsv.cn/Article/details/gnobsshlg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.bbcook.cn/Article/details/ghmtfjjem.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gsytzttzd.sHtML

Q SQL 专题                              90
来源：http://mobile.yfazqb.com/Article/details/gqzuoudpq.sHtML

R Bash 专题                             80
来源：http://www.m.share.tarul.cn/Article/details/ghzbotvuu.sHtML

S C / C++ 专题                          60
来源：http://www.share.bbcook.cn/Article/details/giiojnklc.sHtML

T 其他语言补充                          60
来源：http://www.m.share.vehdjk.com/Article/details/gxblwiptj.sHtML

U 高频实用片段                         120
来源：http://www.m.share.vehdjk.com/Article/details/gqjenkfeh.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gmlivrwjr.sHtML

合计                                  2106 条
来源：http://www.share.yfazqb.com/Article/details/ghtjlzgxe.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gcmsaobcy.sHtML

使用提醒
来源：http://read.share.sjlbkw.cn/Article/details/gdhpimexc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gaxldzhbg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.vehdjk.com/Article/details/gbusawpsj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.yfazqb.com/Article/details/gamflrydn.sHtML


<!-- 参考信息 -->