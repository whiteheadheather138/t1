代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.yfazqb.com/Article/details/ghfpridmg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gtrevejuy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/gsmznnpcv.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfdxdkvmw.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fktsv.cn/Article/details/gmfkpqptd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.sjlbkw.cn/Article/details/gwzxosmbj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.yfazqb.com/Article/details/gvbvjpmzk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.sjlbkw.cn/Article/details/gbedfuuqo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.vehdjk.com/Article/details/ggcvygozw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.tarul.cn/Article/details/gmkldzqzc.sHtML

[U04] Py：变量调试打印
来源：http://blog.tarul.cn/Article/details/gmvhjgrvz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.sjlbkw.cn/Article/details/gvyzcvrzw.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.yfazqb.com/Article/details/gnkwscscu.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gmzgwhzrl.sHtML

[U06] Py：合并两个字典
来源：http://baike.yfazqb.com/Article/details/gkicfdmbu.sHtML

{**a, **b}
来源：http://read.share.sjlbkw.cn/Article/details/gujkmtxyo.sHtML

[U07] Py：反转字典键值
来源：http://m.share.yfazqb.com/Article/details/gpbiugqfj.sHtML

{v: k for k, v in d.items()}
来源：http://blog.bbcook.cn/Article/details/ggmhlklfl.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.yfazqb.com/Article/details/gtemyhtbg.sHtML

[y for x in nested for y in x]
来源：http://www.share.sjlbkw.cn/Article/details/gwlsowjxq.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.tarul.cn/Article/details/gbdixgkan.sHtML

max(d, key=d.get)
来源：http://m.share.yfazqb.com/Article/details/gxzmazxws.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.epnwcf.com/Article/details/goepocqfy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.yfazqb.com/Article/details/gvycolonv.sHtML

[U11] Py：生成器表达式
来源：http://read.share.bbcook.cn/Article/details/geepfijxb.sHtML

(x * 2 for x in arr)
来源：http://blog.yfazqb.com/Article/details/gfomfrdle.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.sjlbkw.cn/Article/details/ginrnqsss.sHtML

Counter(arr).most_common(3)
来源：http://blog.epnwcf.com/Article/details/grjcqggwu.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.tarul.cn/Article/details/gfzrofmuw.sHtML

deque(maxlen=10)
来源：http://wap.vehdjk.com/Article/details/gvczaxkpp.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/gkrezmflc.sHtML

defaultdict(list)
来源：http://m.share.bbcook.cn/Article/details/gguosvgzw.sHtML

[U15] Py：高精度计时
来源：http://mobile.sjlbkw.cn/Article/details/gryfgwesm.sHtML

t = time.perf_counter()
来源：http://wap.vehdjk.com/Article/details/gzayalked.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fktsv.cn/Article/details/gfykgrfka.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.yfazqb.com/Article/details/gotmwhdeq.sHtML

[U17] Py：初始化日志
来源：http://www.share.sjlbkw.cn/Article/details/gzolkfqys.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.yfazqb.com/Article/details/gwvqfcqto.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/govsoafpn.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fktsv.cn/Article/details/gjnezuptb.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.tarul.cn/Article/details/gctpmmivq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.epnwcf.com/Article/details/gsgpuonmj.sHtML

[U20] Py：缓存函数结果
来源：http://wap.yfazqb.com/Article/details/grnluihot.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.yfazqb.com/Article/details/gomxfhiws.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.bbcook.cn/Article/details/ghrggqrcp.sHtML

@contextlib.contextmanager
来源：http://www.share.vehdjk.com/Article/details/glahsolnz.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.vehdjk.com/Article/details/grlbpvhuw.sHtML

list(zip(*m))
来源：http://3g.yfazqb.com/Article/details/gkrugzdqv.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.yfazqb.com/Article/details/gcfuipxxk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.epnwcf.com/Article/details/gjaxhnfey.sHtML

[U24] Py：路径操作
来源：http://wap.bbcook.cn/Article/details/gswnduued.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/gsybzgbby.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.epnwcf.com/Article/details/gpgtljcen.sHtML

csv.DictReader(f)
来源：http://read.share.yfazqb.com/Article/details/gczmndjwm.sHtML

[U26] Py：并发下载
来源：http://mobile.yfazqb.com/Article/details/gwqtcnyvp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.vehdjk.com/Article/details/gnbacajyi.sHtML

[U27] Py：异步 HTTP
来源：http://blog.sjlbkw.cn/Article/details/gcesqmwov.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.epnwcf.com/Article/details/ghdsrublk.sHtML

[U28] Py：类型别名
来源：http://mobile.vehdjk.com/Article/details/gotfejsdw.sHtML

UserId = int
来源：http://read.share.tarul.cn/Article/details/gmotieivp.sHtML

[U29] Py：属性校验
来源：http://www.blog.tarul.cn/Article/details/gzazonujf.sHtML

@property 与 @x.setter 配合
来源：http://www.share.bbcook.cn/Article/details/gagtmlzrx.sHtML

[U30] Py：数据类
来源：http://blog.tarul.cn/Article/details/gomweayrw.sHtML

@dataclass(slots=True)
来源：http://mobile.yfazqb.com/Article/details/gajuotuqr.sHtML

[U31] Py：单测
来源：http://www.share.epnwcf.com/Article/details/gyncoflpr.sHtML

python -m pytest -q
来源：http://3g.sjlbkw.cn/Article/details/gsgtbvufb.sHtML

[U32] Py：代码格式化
来源：http://www.share.fktsv.cn/Article/details/gpqyrvjaj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.bbcook.cn/Article/details/gemognvzg.sHtML

[U33] Py：打包发布
来源：http://baike.tarul.cn/Article/details/gjojaxawq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.tarul.cn/Article/details/gqevecaie.sHtML

[U34] Py：判断编码
来源：http://wap.bbcook.cn/Article/details/gwglbayol.sHtML

chardet.detect(raw)
来源：http://wap.fktsv.cn/Article/details/gquskkxgr.sHtML

[U35] Py：发送邮件
来源：http://wap.yfazqb.com/Article/details/guqwfkcdw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fktsv.cn/Article/details/galilpwpn.sHtML

[U36] Py：定时任务
来源：http://m.share.yfazqb.com/Article/details/gqclblmnn.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.epnwcf.com/Article/details/gtpjydwid.sHtML

[U37] Py：读写 Excel
来源：http://3g.bbcook.cn/Article/details/grtrvghdl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.yfazqb.com/Article/details/gjznbyxux.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.vehdjk.com/Article/details/gbtxlksed.sHtML

Path(__file__).resolve().parent
来源：http://mobile.yfazqb.com/Article/details/gvkdxioof.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.bbcook.cn/Article/details/gpanddomq.sHtML

sys.stdout.isatty()
来源：http://blog.vehdjk.com/Article/details/gzlevpmxc.sHtML

[U40] Py：打印到标准错误
来源：http://blog.epnwcf.com/Article/details/gltfzxfta.sHtML

print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/gnosbzqab.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.tarul.cn/Article/details/gjhmzcypi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.epnwcf.com/Article/details/gkoieandp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.yfazqb.com/Article/details/gcgkzcgbg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.sjlbkw.cn/Article/details/gbjhpociq.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.epnwcf.com/Article/details/gwitixvbe.sHtML

namespace App\Http;
来源：http://3g.sjlbkw.cn/Article/details/gzfylnrpw.sHtML

[U44] PHP：开启严格类型
来源：http://baike.tarul.cn/Article/details/gydwcjjiz.sHtML

declare(strict_types=1);
来源：http://www.share.fktsv.cn/Article/details/gbmbegzli.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.bbcook.cn/Article/details/giwrknjkp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gvbmwzihd.sHtML

[U46] PHP：可空类型
来源：http://3g.sjlbkw.cn/Article/details/gsdhsalex.sHtML

?string $name = null
来源：http://3g.vehdjk.com/Article/details/gwalhyfzb.sHtML

[U47] PHP：联合类型
来源：http://read.share.yfazqb.com/Article/details/grcxwgrbo.sHtML

int|string $id
来源：http://m.share.epnwcf.com/Article/details/ggeznlnzt.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fktsv.cn/Article/details/gazxsbhvx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.tarul.cn/Article/details/gobxoqgkv.sHtML

[U49] PHP：只读属性
来源：http://baike.tarul.cn/Article/details/gsnyttzlw.sHtML

public readonly string $name
来源：http://www.m.share.bbcook.cn/Article/details/gqkeczysk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.sjlbkw.cn/Article/details/gowvrhayh.sHtML

public function __construct(private int $id) {}
来源：http://blog.yfazqb.com/Article/details/gvdgduomo.sHtML

[U51] PHP：数组解构
来源：http://m.share.tarul.cn/Article/details/gpfjtwzad.sHtML

[$a, $b] = $arr;
来源：http://wap.fktsv.cn/Article/details/gsavpugax.sHtML

[U52] PHP：箭头函数
来源：http://www.share.bbcook.cn/Article/details/gvqpypbin.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.sjlbkw.cn/Article/details/goalcnihg.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.vehdjk.com/Article/details/gzcvfusbh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.yfazqb.com/Article/details/gayylrewq.sHtML

[U54] PHP：空安全调用
来源：http://www.share.yfazqb.com/Article/details/gabnrmbtp.sHtML

$obj?->method()
来源：http://blog.fktsv.cn/Article/details/gassvuwte.sHtML

[U55] PHP：match 表达式
来源：http://www.share.sjlbkw.cn/Article/details/goqfelype.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqeofxwb.sHtML

[U56] PHP：命名参数
来源：http://m.share.yfazqb.com/Article/details/gjcsbubji.sHtML

f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gbfhzlwyj.sHtML

[U57] PHP：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gbizipaqq.sHtML

"值: {$a}"
来源：http://baike.tarul.cn/Article/details/goudapirw.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.yfazqb.com/Article/details/gvozitcyk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.tarul.cn/Article/details/gfcxbmsmj.sHtML

[U59] PHP：自定义排序
来源：http://baike.sjlbkw.cn/Article/details/ghmzjjgia.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/gouhvgrwv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fktsv.cn/Article/details/gdfbytqnw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fktsv.cn/Article/details/gltubkntu.sHtML

[U61] PHP：正则
来源：http://www.blog.vehdjk.com/Article/details/gfpwcfpaz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/glwhlyngp.sHtML

[U62] PHP：日期对象
来源：http://m.share.tarul.cn/Article/details/gwqeubqgj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.bbcook.cn/Article/details/glacmiswr.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fktsv.cn/Article/details/gyuwlvmmo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.yfazqb.com/Article/details/gezxftqbz.sHtML

[U64] PHP：目录遍历
来源：http://m.share.tarul.cn/Article/details/gwfwhrigo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.sjlbkw.cn/Article/details/gnpbaajux.sHtML

[U65] PHP：会话
来源：http://m.share.vehdjk.com/Article/details/gemwpynpt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.yfazqb.com/Article/details/givpofvfc.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.sjlbkw.cn/Article/details/glgnowaep.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.bbcook.cn/Article/details/gotpeqvfc.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fktsv.cn/Article/details/gzegudgez.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.tarul.cn/Article/details/glqljkyxl.sHtML

[U68] PHP：PDO 连接
来源：http://blog.sjlbkw.cn/Article/details/gxitjgkdj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.epnwcf.com/Article/details/gnietdwoy.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.yfazqb.com/Article/details/gsqkooyvb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.epnwcf.com/Article/details/gkcqaqeos.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.yfazqb.com/Article/details/gmoraopfh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.epnwcf.com/Article/details/gzgpdvjlm.sHtML

[U71] PHP：抛出异常
来源：http://m.share.vehdjk.com/Article/details/gmlzlbtam.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fktsv.cn/Article/details/gualjhdpp.sHtML

[U72] PHP：写错误日志
来源：http://m.share.epnwcf.com/Article/details/golukedvf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fktsv.cn/Article/details/gpdyvdwpv.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.yfazqb.com/Article/details/gydhsvidc.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.sjlbkw.cn/Article/details/gyonsmeup.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fktsv.cn/Article/details/gghmvqjgg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.yfazqb.com/Article/details/gtldpmvcs.sHtML

[U75] PHP：依赖注入
来源：http://m.share.bbcook.cn/Article/details/guibgtyac.sHtML

composer require psr/container
来源：http://mobile.tarul.cn/Article/details/gxagqqyro.sHtML

[U76] PHP：简单路由
来源：http://3g.fktsv.cn/Article/details/gjxkcbpzg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.epnwcf.com/Article/details/gftvxmajn.sHtML

[U77] PHP：模板渲染
来源：http://www.share.epnwcf.com/Article/details/guimvciky.sHtML

composer require twig/twig
来源：http://m.share.tarul.cn/Article/details/goqhfhvlj.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gmsjcofis.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.tarul.cn/Article/details/gvrwrdyrf.sHtML

[U79] PHP：静态分析
来源：http://baike.epnwcf.com/Article/details/gwcqztjbi.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.epnwcf.com/Article/details/gtgimdmvl.sHtML

[U80] PHP：代码规范修复
来源：http://baike.bbcook.cn/Article/details/grrboqvjp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.vehdjk.com/Article/details/gmfpqykxr.sHtML

[U81] JS：初始化项目
来源：http://baike.vehdjk.com/Article/details/gkydkhlln.sHtML

npm init -y;  npm i express
来源：http://mobile.vehdjk.com/Article/details/gespxvgag.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fktsv.cn/Article/details/gpjsgndlu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.vehdjk.com/Article/details/ghdbcwgaa.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.sjlbkw.cn/Article/details/gphmizjxe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/gmkehgifj.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.tarul.cn/Article/details/gozkvqkpw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.tarul.cn/Article/details/gifwfggpg.sHtML

[U85] JS：可选链
来源：http://m.share.fktsv.cn/Article/details/gghazdkhl.sHtML

a?.b?.c
来源：http://blog.epnwcf.com/Article/details/gbkbcrzvq.sHtML

[U86] JS：空值合并
来源：http://m.share.vehdjk.com/Article/details/gepbxdwhz.sHtML

a ?? b
来源：http://m.share.yfazqb.com/Article/details/gtttovshj.sHtML

[U87] JS：解构默认值
来源：http://m.share.bbcook.cn/Article/details/ghorwxmrn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnegcmsnp.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.vehdjk.com/Article/details/gmggugwlv.sHtML

{ ...a, ...b }
来源：http://m.share.sjlbkw.cn/Article/details/gpdpwedns.sHtML

[U89] JS：数组去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gomyvemqa.sHtML

[...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gsxoerbxx.sHtML

[U90] JS：数字数组排序
来源：http://baike.epnwcf.com/Article/details/gjgpxmdrv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gxvnhhioz.sHtML

[U91] JS：对象键值遍历
来源：http://blog.sjlbkw.cn/Article/details/gsrwvdivx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.sjlbkw.cn/Article/details/gzaqohzzu.sHtML

[U92] JS：深拷贝
来源：http://baike.vehdjk.com/Article/details/gjvxskyjv.sHtML

structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gdqogxwfu.sHtML

[U93] JS：模板字符串
来源：http://baike.tarul.cn/Article/details/gganxxdkn.sHtML

`共 ${n} 条`
来源：http://3g.tarul.cn/Article/details/gmtrgnngw.sHtML

[U94] JS：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gwawhsezu.sHtML

const double = x => x * 2;
来源：http://mobile.vehdjk.com/Article/details/gaegskeyn.sHtML

[U95] JS：Promise 包装
来源：http://read.share.epnwcf.com/Article/details/gubzskabf.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.yfazqb.com/Article/details/gnizkclqm.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkbnwasl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gpslelwnp.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/gmsxsgvtc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gjiuyrvdb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.bbcook.cn/Article/details/gkeafafpe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fktsv.cn/Article/details/gtxjjozut.sHtML

[U99] JS：事件监听
来源：http://wap.fktsv.cn/Article/details/gyxhqiikd.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.epnwcf.com/Article/details/gpefnboiy.sHtML

[U100] JS：DOM 查询
来源：http://www.share.sjlbkw.cn/Article/details/gbsfbphnr.sHtML

document.querySelector(".item")
来源：http://wap.fktsv.cn/Article/details/gbkhclhbe.sHtML

[U101] JS：classList 操作
来源：http://www.share.sjlbkw.cn/Article/details/gdpflwmtj.sHtML

el.classList.toggle("active")
来源：http://3g.fktsv.cn/Article/details/gudqspamp.sHtML

[U102] JS：本地存储
来源：http://read.share.fktsv.cn/Article/details/gwdriafhu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.yfazqb.com/Article/details/gzbvrhoey.sHtML

[U103] JS：定时器
来源：http://baike.bbcook.cn/Article/details/gpkgtsspn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fktsv.cn/Article/details/gqdhkxuqk.sHtML

[U104] JS：防抖
来源：http://read.share.yfazqb.com/Article/details/ghcbrmzms.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/gqtiyfrom.sHtML

[U105] JS：节流
来源：http://www.m.share.epnwcf.com/Article/details/gpnbsxgxs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fktsv.cn/Article/details/gfmdpqpqc.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gdzqfhcul.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.vehdjk.com/Article/details/gsvhofwtf.sHtML

[U107] JS：数字千分位
来源：http://wap.vehdjk.com/Article/details/gmwdbbatb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/gifjuyjbf.sHtML

[U108] JS：随机整数
来源：http://3g.sjlbkw.cn/Article/details/glsvjsfbz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.vehdjk.com/Article/details/gkuwlewgx.sHtML

[U109] JS：数组分组
来源：http://baike.yfazqb.com/Article/details/gfxnwnvzu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.sjlbkw.cn/Article/details/ggtjnpqmy.sHtML

[U110] JS：数组分块
来源：http://wap.yfazqb.com/Article/details/gjnfqmlvt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.tarul.cn/Article/details/gkfcpvevj.sHtML

[U111] JS：对象转 Map
来源：http://wap.epnwcf.com/Article/details/gahqlrhsp.sHtML

new Map(Object.entries(obj))
来源：http://wap.sjlbkw.cn/Article/details/gxeicokmo.sHtML

[U112] JS：字符串补位
来源：http://blog.fktsv.cn/Article/details/gddopmyok.sHtML

"7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gdgffzmle.sHtML

[U113] JS：正则替换全部
来源：http://wap.epnwcf.com/Article/details/gmhnjxbjo.sHtML

s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gjmfjuerz.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.sjlbkw.cn/Article/details/guhahrvgl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/gytmbyrjq.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gofmxdzxa.sHtML

crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gavqkaqpe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.vehdjk.com/Article/details/gfkifoblc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.sjlbkw.cn/Article/details/gennoolyf.sHtML

[U117] JS：单元测试
来源：http://mobile.tarul.cn/Article/details/gwohwytgu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fktsv.cn/Article/details/gnvqjvatx.sHtML

[U118] JS：开发服务器
来源：http://blog.fktsv.cn/Article/details/gegkgojko.sHtML

npm i -D vite;  npx vite
来源：http://m.share.epnwcf.com/Article/details/glnodvlob.sHtML

[U119] JS：生产构建
来源：http://blog.bbcook.cn/Article/details/gfyfkixub.sHtML

npx vite build
来源：http://wap.yfazqb.com/Article/details/gmfqyynqa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.yfazqb.com/Article/details/giynacqib.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.bbcook.cn/Article/details/gbodmrjmx.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gulmiydjx.sHtML

统计汇总
来源：http://www.share.tarul.cn/Article/details/glnuwaqhf.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gksnrprpr.sHtML

按语言统计（条）：
来源：http://wap.epnwcf.com/Article/details/gddbvtijp.sHtML

Python ......... 252
来源：http://blog.vehdjk.com/Article/details/gxtuyhkje.sHtML

PHP ............ 252
来源：http://www.share.vehdjk.com/Article/details/glbbiritn.sHtML

JavaScript ..... 252
来源：http://3g.tarul.cn/Article/details/gritsauqf.sHtML

TypeScript ..... 212
来源：http://3g.tarul.cn/Article/details/gcucmxofg.sHtML

Java ........... 212
来源：http://blog.epnwcf.com/Article/details/gkufkhqez.sHtML

Go ............. 212
来源：http://blog.bbcook.cn/Article/details/gvwgoexld.sHtML

Ruby ........... 212
来源：http://3g.sjlbkw.cn/Article/details/gguezqmvr.sHtML

C# ............. 212
来源：http://wap.epnwcf.com/Article/details/gcrafmquc.sHtML

C .............. 30
来源：http://baike.epnwcf.com/Article/details/gdwprizxj.sHtML

C++ ............ 30
来源：http://baike.yfazqb.com/Article/details/gzftjvrio.sHtML

SQL ............ 90
来源：http://www.m.share.fktsv.cn/Article/details/gygwglolb.sHtML

Bash ........... 80
来源：http://www.m.share.epnwcf.com/Article/details/gdjcnmlnt.sHtML

Kotlin ......... 15
来源：http://www.blog.vehdjk.com/Article/details/gaxovovwb.sHtML

Swift .......... 15
来源：http://www.share.bbcook.cn/Article/details/gmehlqlwg.sHtML

Lua ............ 10
来源：http://mobile.yfazqb.com/Article/details/gnqgehvpb.sHtML

Perl ........... 10
来源：http://www.share.yfazqb.com/Article/details/gpdbualnr.sHtML

Scala .......... 10
来源：http://blog.tarul.cn/Article/details/gbhqjzvwi.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gbrxnfpyj.sHtML

合计 ........... 2106 条
来源：http://m.share.bbcook.cn/Article/details/gvvqluyfw.sHtML

按章节统计：
来源：http://wap.yfazqb.com/Article/details/gvwyvteku.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.yfazqb.com/Article/details/gagyxagsn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gwoqvocys.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gmxynfoim.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/gtzkwrljc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvbjrmsb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/gcftqjqym.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gqthnlimc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/gbnewcqwb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gsvkbpzfo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.vehdjk.com/Article/details/gmzghdilv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gpyfmyuxt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/ghqwjjxku.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gdhhsrudo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gvqukkgdk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.vehdjk.com/Article/details/gkzegexol.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gohmefrzz.sHtML

Q SQL 专题                              90
来源：http://read.share.epnwcf.com/Article/details/gjgcjdfkb.sHtML

R Bash 专题                             80
来源：http://3g.yfazqb.com/Article/details/gfioymquv.sHtML

S C / C++ 专题                          60
来源：http://baike.vehdjk.com/Article/details/grldwoajg.sHtML

T 其他语言补充                          60
来源：http://mobile.sjlbkw.cn/Article/details/ggitldsee.sHtML

U 高频实用片段                         120
来源：http://blog.yfazqb.com/Article/details/govzdytaj.sHtML

------------------------------------
来源：http://3g.vehdjk.com/Article/details/gsyrwhksa.sHtML

合计                                  2106 条
来源：http://read.share.epnwcf.com/Article/details/gmpsvwtqb.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gyqiqijlb.sHtML

使用提醒
来源：http://www.share.yfazqb.com/Article/details/gkdjeokmx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gbuyzcysy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fktsv.cn/Article/details/glxgmcpfw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.yfazqb.com/Article/details/gpqiirljy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.sjlbkw.cn/Article/details/gcjkqjjzv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.tarul.cn/Article/details/gytejwpgf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.tarul.cn/Article/details/gemifvfdz.sHtML

—— 文件结束 ——
来源：http://blog.sjlbkw.cn/Article/details/gmulkcihp.sHtML


<!-- 参考信息 -->