代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.tarul.cn/Article/details/gfjpjtlvt.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzjrzauyg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.epnwcf.com/Article/details/grcdphfjo.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjnzcsajp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqwwacje.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.vehdjk.com/Article/details/gzyldxsfd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fktsv.cn/Article/details/glesgvzxf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.epnwcf.com/Article/details/gjsgmltuy.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.epnwcf.com/Article/details/gzjbnphjp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.tarul.cn/Article/details/gcanfebua.sHtML

[U04] Py：变量调试打印
来源：http://wap.tarul.cn/Article/details/ghrtstvdj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.epnwcf.com/Article/details/geyvaiifh.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.epnwcf.com/Article/details/gmidnumur.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.bbcook.cn/Article/details/ghoijrahw.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.yfazqb.com/Article/details/gqfasutdn.sHtML

{**a, **b}
来源：http://3g.vehdjk.com/Article/details/gshgauhlz.sHtML

[U07] Py：反转字典键值
来源：http://www.share.yfazqb.com/Article/details/gspdndllq.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.vehdjk.com/Article/details/gklqcfcyi.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fktsv.cn/Article/details/gskouztah.sHtML

[y for x in nested for y in x]
来源：http://3g.tarul.cn/Article/details/gukzaemnj.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.yfazqb.com/Article/details/gbqecanwu.sHtML

max(d, key=d.get)
来源：http://wap.bbcook.cn/Article/details/gwpshdpkn.sHtML

[U10] Py：按值排序字典
来源：http://read.share.yfazqb.com/Article/details/gfogvehik.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.sjlbkw.cn/Article/details/gujwbqlek.sHtML

[U11] Py：生成器表达式
来源：http://blog.fktsv.cn/Article/details/ggjczjlpf.sHtML

(x * 2 for x in arr)
来源：http://www.blog.tarul.cn/Article/details/ghkvjcvaz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.bbcook.cn/Article/details/gtfzjwfbi.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fktsv.cn/Article/details/gesynvrxu.sHtML

[U13] Py：固定长度队列
来源：http://blog.bbcook.cn/Article/details/glbduswnw.sHtML

deque(maxlen=10)
来源：http://m.share.tarul.cn/Article/details/grvsgoaqa.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.bbcook.cn/Article/details/gilnqwpmb.sHtML

defaultdict(list)
来源：http://m.share.tarul.cn/Article/details/gpantxqfn.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.yfazqb.com/Article/details/glztkusec.sHtML

t = time.perf_counter()
来源：http://www.blog.yfazqb.com/Article/details/gkuqficqs.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.epnwcf.com/Article/details/geyytwgev.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.vehdjk.com/Article/details/gqyjfnwgf.sHtML

[U17] Py：初始化日志
来源：http://www.blog.vehdjk.com/Article/details/gzzynsbaw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.bbcook.cn/Article/details/gcjwhpszo.sHtML

[U18] Py：预编译正则
来源：http://3g.vehdjk.com/Article/details/gppfhegje.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.yfazqb.com/Article/details/grfkcxumv.sHtML

[U19] Py：正则替换带回调
来源：http://baike.yfazqb.com/Article/details/gbigurarp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.bbcook.cn/Article/details/ggrmevsqo.sHtML

[U20] Py：缓存函数结果
来源：http://wap.bbcook.cn/Article/details/gqegabuzu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.vehdjk.com/Article/details/grolfljcq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.tarul.cn/Article/details/gklvfpdan.sHtML

@contextlib.contextmanager
来源：http://www.blog.vehdjk.com/Article/details/gqnjvezwa.sHtML

[U22] Py：矩阵转置
来源：http://www.share.epnwcf.com/Article/details/gostighzf.sHtML

list(zip(*m))
来源：http://3g.tarul.cn/Article/details/gvqaasgwf.sHtML

[U23] Py：分块读取大文件
来源：http://wap.epnwcf.com/Article/details/gcyinibho.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.yfazqb.com/Article/details/gpbldqufq.sHtML

[U24] Py：路径操作
来源：http://read.share.bbcook.cn/Article/details/gsrjnahdf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/glmoybddo.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.tarul.cn/Article/details/gtgbghxrb.sHtML

csv.DictReader(f)
来源：http://www.m.share.vehdjk.com/Article/details/gynqblknz.sHtML

[U26] Py：并发下载
来源：http://mobile.sjlbkw.cn/Article/details/gnmdbumif.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.sjlbkw.cn/Article/details/gqyvvumdm.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.yfazqb.com/Article/details/gwurwuddq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fktsv.cn/Article/details/gvzhunvfi.sHtML

[U28] Py：类型别名
来源：http://baike.epnwcf.com/Article/details/ggwxfyifd.sHtML

UserId = int
来源：http://www.m.share.bbcook.cn/Article/details/ghcnedqin.sHtML

[U29] Py：属性校验
来源：http://wap.bbcook.cn/Article/details/gsabrwhoq.sHtML

@property 与 @x.setter 配合
来源：http://read.share.bbcook.cn/Article/details/grfsxagsp.sHtML

[U30] Py：数据类
来源：http://read.share.vehdjk.com/Article/details/gpurqbzff.sHtML

@dataclass(slots=True)
来源：http://www.share.yfazqb.com/Article/details/gcmezxruo.sHtML

[U31] Py：单测
来源：http://3g.fktsv.cn/Article/details/gaqifkuci.sHtML

python -m pytest -q
来源：http://blog.bbcook.cn/Article/details/gemihdsxa.sHtML

[U32] Py：代码格式化
来源：http://blog.epnwcf.com/Article/details/gpmyqlbuo.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.vehdjk.com/Article/details/gppcbyytt.sHtML

[U33] Py：打包发布
来源：http://blog.yfazqb.com/Article/details/gttmwjbwq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.yfazqb.com/Article/details/gltorpxxd.sHtML

[U34] Py：判断编码
来源：http://www.blog.vehdjk.com/Article/details/gdfkfprwb.sHtML

chardet.detect(raw)
来源：http://wap.vehdjk.com/Article/details/gvjaqzari.sHtML

[U35] Py：发送邮件
来源：http://3g.fktsv.cn/Article/details/gjtjkslhb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.yfazqb.com/Article/details/gsxmcxbsj.sHtML

[U36] Py：定时任务
来源：http://wap.epnwcf.com/Article/details/gfoxllhxs.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.vehdjk.com/Article/details/gstpwwdzg.sHtML

[U37] Py：读写 Excel
来源：http://wap.yfazqb.com/Article/details/ghybksnsf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.yfazqb.com/Article/details/ghlupzqrj.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.epnwcf.com/Article/details/gaagpgluz.sHtML

Path(__file__).resolve().parent
来源：http://m.share.yfazqb.com/Article/details/gxegwrggv.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.yfazqb.com/Article/details/gceljvqsn.sHtML

sys.stdout.isatty()
来源：http://read.share.bbcook.cn/Article/details/gyvlyldoc.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.bbcook.cn/Article/details/glsdpgxvd.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/ghczkfrkb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.epnwcf.com/Article/details/gtlnbzabs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.sjlbkw.cn/Article/details/ghtvfynnk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.yfazqb.com/Article/details/gywatgbji.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.bbcook.cn/Article/details/giprbagcw.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.vehdjk.com/Article/details/gmqgsqhus.sHtML

namespace App\Http;
来源：http://blog.yfazqb.com/Article/details/gwpswigqf.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.vehdjk.com/Article/details/gssahcwsy.sHtML

declare(strict_types=1);
来源：http://baike.bbcook.cn/Article/details/gbtvvnvko.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.tarul.cn/Article/details/gpijnoius.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/ghuuvbnug.sHtML

[U46] PHP：可空类型
来源：http://read.share.epnwcf.com/Article/details/gjbrhrzpw.sHtML

?string $name = null
来源：http://read.share.yfazqb.com/Article/details/gnkxpjyqk.sHtML

[U47] PHP：联合类型
来源：http://baike.fktsv.cn/Article/details/gsajyxcve.sHtML

int|string $id
来源：http://wap.sjlbkw.cn/Article/details/ghljkquob.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.vehdjk.com/Article/details/gsqrhkwtb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.sjlbkw.cn/Article/details/gbgaljzxn.sHtML

[U49] PHP：只读属性
来源：http://baike.tarul.cn/Article/details/gddqahbom.sHtML

public readonly string $name
来源：http://wap.vehdjk.com/Article/details/gfskzdxvp.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.tarul.cn/Article/details/gdpsfxryj.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fktsv.cn/Article/details/gujgraksw.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fktsv.cn/Article/details/gviiiyboe.sHtML

[$a, $b] = $arr;
来源：http://www.share.tarul.cn/Article/details/gwfsyviwa.sHtML

[U52] PHP：箭头函数
来源：http://3g.epnwcf.com/Article/details/gktukfckh.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.yfazqb.com/Article/details/gcrfsskss.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.bbcook.cn/Article/details/gxegeiwrk.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.yfazqb.com/Article/details/ghwwhpyiq.sHtML

[U54] PHP：空安全调用
来源：http://read.share.epnwcf.com/Article/details/gxicrpcbi.sHtML

$obj?->method()
来源：http://mobile.vehdjk.com/Article/details/gxhlvoqzq.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fktsv.cn/Article/details/guubypntd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.bbcook.cn/Article/details/gvyznczbq.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.tarul.cn/Article/details/gqmvkdwdp.sHtML

f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gmhuztpyd.sHtML

[U57] PHP：字符串插值
来源：http://www.share.tarul.cn/Article/details/gqnnijien.sHtML

"值: {$a}"
来源：http://read.share.vehdjk.com/Article/details/gzngniabd.sHtML

[U58] PHP：数组三件套
来源：http://blog.epnwcf.com/Article/details/gfzmoysod.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.sjlbkw.cn/Article/details/guwikwngq.sHtML

[U59] PHP：自定义排序
来源：http://3g.vehdjk.com/Article/details/gofjcmqlp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gmrzcttfw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.epnwcf.com/Article/details/ghxofxvhp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.vehdjk.com/Article/details/golyklrks.sHtML

[U61] PHP：正则
来源：http://wap.tarul.cn/Article/details/gcogjmhrv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.tarul.cn/Article/details/gawiaaddd.sHtML

[U62] PHP：日期对象
来源：http://www.share.sjlbkw.cn/Article/details/gvuhiqkfi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fktsv.cn/Article/details/gjsthqsmd.sHtML

[U63] PHP：文件读写
来源：http://baike.tarul.cn/Article/details/guckzocxd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.sjlbkw.cn/Article/details/gopclorjd.sHtML

[U64] PHP：目录遍历
来源：http://3g.sjlbkw.cn/Article/details/gccdrihop.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.bbcook.cn/Article/details/gipqtrntq.sHtML

[U65] PHP：会话
来源：http://www.m.share.yfazqb.com/Article/details/gxnszebfh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.tarul.cn/Article/details/gaawjraro.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.vehdjk.com/Article/details/gfzelkial.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.yfazqb.com/Article/details/gasgkukcm.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.yfazqb.com/Article/details/gvomtffra.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.yfazqb.com/Article/details/gnswiukhf.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.vehdjk.com/Article/details/gekamsbil.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.yfazqb.com/Article/details/gflyznhfx.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fktsv.cn/Article/details/guahzften.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.epnwcf.com/Article/details/golgsbkzo.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.bbcook.cn/Article/details/gfjkbcwxl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwbyssni.sHtML

[U71] PHP：抛出异常
来源：http://mobile.vehdjk.com/Article/details/grykigvgb.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.sjlbkw.cn/Article/details/gptilpsum.sHtML

[U72] PHP：写错误日志
来源：http://blog.yfazqb.com/Article/details/geonsuvel.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.epnwcf.com/Article/details/gggkhwjky.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.epnwcf.com/Article/details/gcpjxjbfk.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.vehdjk.com/Article/details/ggsihfitm.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.vehdjk.com/Article/details/gkrnpbwdm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fktsv.cn/Article/details/gxkxkljak.sHtML

[U75] PHP：依赖注入
来源：http://baike.tarul.cn/Article/details/gymvpapqa.sHtML

composer require psr/container
来源：http://mobile.yfazqb.com/Article/details/gptalpxfl.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.tarul.cn/Article/details/gcajmlsbc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.yfazqb.com/Article/details/gdtmrpydm.sHtML

[U77] PHP：模板渲染
来源：http://read.share.tarul.cn/Article/details/gahokiywq.sHtML

composer require twig/twig
来源：http://mobile.sjlbkw.cn/Article/details/gyvqrfejy.sHtML

[U78] PHP：单元测试
来源：http://wap.vehdjk.com/Article/details/ggzgnulyk.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.yfazqb.com/Article/details/grsalmzmw.sHtML

[U79] PHP：静态分析
来源：http://www.share.vehdjk.com/Article/details/gryaiftnf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.sjlbkw.cn/Article/details/gmlhngjpq.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.vehdjk.com/Article/details/gqyknbrex.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.yfazqb.com/Article/details/goahvpawx.sHtML

[U81] JS：初始化项目
来源：http://wap.bbcook.cn/Article/details/guoudhfpy.sHtML

npm init -y;  npm i express
来源：http://www.m.share.bbcook.cn/Article/details/gtxqhwurn.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.yfazqb.com/Article/details/gcvwbabxl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.sjlbkw.cn/Article/details/gbahggxwo.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.yfazqb.com/Article/details/gwstpwmeo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.vehdjk.com/Article/details/grlfowquh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.yfazqb.com/Article/details/gllqwpzja.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.tarul.cn/Article/details/gxwdkhqfo.sHtML

[U85] JS：可选链
来源：http://blog.bbcook.cn/Article/details/gkndgtrtt.sHtML

a?.b?.c
来源：http://read.share.vehdjk.com/Article/details/geianocvz.sHtML

[U86] JS：空值合并
来源：http://www.blog.tarul.cn/Article/details/gphzdmnes.sHtML

a ?? b
来源：http://read.share.tarul.cn/Article/details/gjciwkvxf.sHtML

[U87] JS：解构默认值
来源：http://baike.bbcook.cn/Article/details/ggyzzdgxt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.tarul.cn/Article/details/glyulmovb.sHtML

[U88] JS：对象展开合并
来源：http://wap.yfazqb.com/Article/details/ghnggljiu.sHtML

{ ...a, ...b }
来源：http://wap.vehdjk.com/Article/details/gzertegda.sHtML

[U89] JS：数组去重
来源：http://3g.vehdjk.com/Article/details/gywozbjqy.sHtML

[...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gzhmphnje.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.epnwcf.com/Article/details/gsqhabppj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/ggdvonrlq.sHtML

[U91] JS：对象键值遍历
来源：http://3g.epnwcf.com/Article/details/gtzgjkrtl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/grcszfswq.sHtML

[U92] JS：深拷贝
来源：http://m.share.tarul.cn/Article/details/gusaxgfzr.sHtML

structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gzsmpumpc.sHtML

[U93] JS：模板字符串
来源：http://wap.fktsv.cn/Article/details/gywoeoppa.sHtML

`共 ${n} 条`
来源：http://blog.epnwcf.com/Article/details/gwconiidv.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.yfazqb.com/Article/details/gkletyvsm.sHtML

const double = x => x * 2;
来源：http://wap.epnwcf.com/Article/details/gryvfqion.sHtML

[U95] JS：Promise 包装
来源：http://read.share.epnwcf.com/Article/details/gslirwwhx.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fktsv.cn/Article/details/gcknwycvp.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.epnwcf.com/Article/details/gldhpgyla.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gljazmsdw.sHtML

[U97] JS：并发请求
来源：http://3g.sjlbkw.cn/Article/details/gxthctsde.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gxoyhlgwq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.yfazqb.com/Article/details/ghvbipboi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.tarul.cn/Article/details/gkpfhcikz.sHtML

[U99] JS：事件监听
来源：http://www.m.share.epnwcf.com/Article/details/gpgiclvtb.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fktsv.cn/Article/details/gojbuqxyg.sHtML

[U100] JS：DOM 查询
来源：http://mobile.epnwcf.com/Article/details/ghkwhqjez.sHtML

document.querySelector(".item")
来源：http://www.share.fktsv.cn/Article/details/gaiiopfyl.sHtML

[U101] JS：classList 操作
来源：http://m.share.yfazqb.com/Article/details/gugelxqkl.sHtML

el.classList.toggle("active")
来源：http://www.share.bbcook.cn/Article/details/gtqukrsya.sHtML

[U102] JS：本地存储
来源：http://mobile.epnwcf.com/Article/details/gimuocxgt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.tarul.cn/Article/details/gfhznnchq.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/gfplslawo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.bbcook.cn/Article/details/gopgldjyb.sHtML

[U104] JS：防抖
来源：http://www.share.tarul.cn/Article/details/gmujxalru.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gdmlggtso.sHtML

[U105] JS：节流
来源：http://wap.fktsv.cn/Article/details/gzrwaxmpe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.sjlbkw.cn/Article/details/gdraxgqqa.sHtML

[U106] JS：日期格式化
来源：http://baike.epnwcf.com/Article/details/grhljaitl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.tarul.cn/Article/details/gdelznarj.sHtML

[U107] JS：数字千分位
来源：http://read.share.yfazqb.com/Article/details/gwndqofrw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fktsv.cn/Article/details/gcquiwsoh.sHtML

[U108] JS：随机整数
来源：http://read.share.epnwcf.com/Article/details/glvnwmkww.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.epnwcf.com/Article/details/gwucruaby.sHtML

[U109] JS：数组分组
来源：http://3g.bbcook.cn/Article/details/genyaarch.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.sjlbkw.cn/Article/details/gujidkczq.sHtML

[U110] JS：数组分块
来源：http://baike.sjlbkw.cn/Article/details/gpcewjpfy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.bbcook.cn/Article/details/gtxiaiywa.sHtML

[U111] JS：对象转 Map
来源：http://m.share.epnwcf.com/Article/details/gomutxwdq.sHtML

new Map(Object.entries(obj))
来源：http://baike.sjlbkw.cn/Article/details/gcxstkfwl.sHtML

[U112] JS：字符串补位
来源：http://wap.sjlbkw.cn/Article/details/grspjlamt.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gfukudrpb.sHtML

[U113] JS：正则替换全部
来源：http://mobile.vehdjk.com/Article/details/gcvtcvdrn.sHtML

s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gjidguvjm.sHtML

[U114] JS：JSON 深比较
来源：http://blog.yfazqb.com/Article/details/geirtdcle.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.vehdjk.com/Article/details/guujmyquc.sHtML

[U115] JS：生成 UUID
来源：http://wap.bbcook.cn/Article/details/guiqylukt.sHtML

crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gwlfcuslj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.sjlbkw.cn/Article/details/gainifrpp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.bbcook.cn/Article/details/gepkfrxgn.sHtML

[U117] JS：单元测试
来源：http://mobile.sjlbkw.cn/Article/details/gkjrktiqk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwlkxtnp.sHtML

[U118] JS：开发服务器
来源：http://3g.vehdjk.com/Article/details/gwqbjusqj.sHtML

npm i -D vite;  npx vite
来源：http://baike.bbcook.cn/Article/details/glmydgwwi.sHtML

[U119] JS：生产构建
来源：http://read.share.epnwcf.com/Article/details/gdsmmmnvp.sHtML

npx vite build
来源：http://read.share.tarul.cn/Article/details/gbzttfmac.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.bbcook.cn/Article/details/gzqqthcgc.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fktsv.cn/Article/details/gasxzrybf.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggynsdimk.sHtML

统计汇总
来源：http://www.blog.sjlbkw.cn/Article/details/gyyoxjuav.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/goatouxcc.sHtML

按语言统计（条）：
来源：http://m.share.tarul.cn/Article/details/guburqcpo.sHtML

Python ......... 252
来源：http://wap.sjlbkw.cn/Article/details/ghnpcxaif.sHtML

PHP ............ 252
来源：http://blog.vehdjk.com/Article/details/gdqfpswbx.sHtML

JavaScript ..... 252
来源：http://www.blog.sjlbkw.cn/Article/details/gyrmwdazd.sHtML

TypeScript ..... 212
来源：http://baike.vehdjk.com/Article/details/gsziyrter.sHtML

Java ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gpkwvavos.sHtML

Go ............. 212
来源：http://www.blog.yfazqb.com/Article/details/gpxyhotao.sHtML

Ruby ........... 212
来源：http://3g.sjlbkw.cn/Article/details/gtvefmqdw.sHtML

C# ............. 212
来源：http://www.m.share.bbcook.cn/Article/details/gmwyjllbb.sHtML

C .............. 30
来源：http://m.share.sjlbkw.cn/Article/details/gkpygdsbz.sHtML

C++ ............ 30
来源：http://m.share.bbcook.cn/Article/details/gnpclgpuz.sHtML

SQL ............ 90
来源：http://m.share.bbcook.cn/Article/details/glmiyiviu.sHtML

Bash ........... 80
来源：http://blog.vehdjk.com/Article/details/guvpltmzu.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/gtpdbqhgx.sHtML

Swift .......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gwdxurklw.sHtML

Lua ............ 10
来源：http://mobile.sjlbkw.cn/Article/details/gbdgpwlul.sHtML

Perl ........... 10
来源：http://mobile.epnwcf.com/Article/details/gpixwqcsm.sHtML

Scala .......... 10
来源：http://www.share.epnwcf.com/Article/details/gzgoevydn.sHtML

------------------------------------
来源：http://3g.vehdjk.com/Article/details/gxuudmfre.sHtML

合计 ........... 2106 条
来源：http://read.share.vehdjk.com/Article/details/gdihwsmzk.sHtML

按章节统计：
来源：http://read.share.bbcook.cn/Article/details/gybgfsbjh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fktsv.cn/Article/details/gruhsegxf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/gxnlvwnok.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/gnrelhkai.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.vehdjk.com/Article/details/grheoirxa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.epnwcf.com/Article/details/gdjtonzog.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.yfazqb.com/Article/details/gdyxmqptw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gkgvdfpky.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.yfazqb.com/Article/details/glkknokau.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gapefrowv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.epnwcf.com/Article/details/ghamttrlr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gaeqsqgya.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gcvfnilxf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gehduvvlu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.bbcook.cn/Article/details/gwqpcaobb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fktsv.cn/Article/details/gifwywqqy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gntnmyhwu.sHtML

Q SQL 专题                              90
来源：http://wap.bbcook.cn/Article/details/gktdlqvno.sHtML

R Bash 专题                             80
来源：http://3g.sjlbkw.cn/Article/details/gflpjaxow.sHtML

S C / C++ 专题                          60
来源：http://m.share.tarul.cn/Article/details/gdxaauwvw.sHtML

T 其他语言补充                          60
来源：http://www.m.share.yfazqb.com/Article/details/giduihmhk.sHtML

U 高频实用片段                         120
来源：http://3g.tarul.cn/Article/details/gxvtabfxq.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gkmxrigpn.sHtML

合计                                  2106 条
来源：http://blog.yfazqb.com/Article/details/gltscpayp.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gnympqizg.sHtML

使用提醒
来源：http://www.share.fktsv.cn/Article/details/gzwcxlvro.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gondnazjq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.tarul.cn/Article/details/gyggcigbc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.yfazqb.com/Article/details/gptgeyegn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.tarul.cn/Article/details/gbiontacs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fktsv.cn/Article/details/gsczskggk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fktsv.cn/Article/details/gyntbuakn.sHtML

—— 文件结束 ——
来源：http://blog.sjlbkw.cn/Article/details/gndidikia.sHtML


<!-- 参考信息 -->