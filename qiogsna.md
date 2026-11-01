代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://baike.vehdjk.com/Article/details/ghmculdgj.sHtML

[T59] Scala：循环
来源：http://www.blog.tarul.cn/Article/details/gvpruuwnv.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fktsv.cn/Article/details/gwcrsaplr.sHtML

[T60] Scala：折叠
来源：http://wap.sjlbkw.cn/Article/details/geaoxgrdu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.sjlbkw.cn/Article/details/gmfqrwebu.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmzvivfae.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.epnwcf.com/Article/details/gohpulaxv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gioirnqbw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.vehdjk.com/Article/details/gkyadybzg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.sjlbkw.cn/Article/details/gweshglth.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.vehdjk.com/Article/details/geefjqjsd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.epnwcf.com/Article/details/gdxnikzgu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.vehdjk.com/Article/details/gsiokwxtg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.tarul.cn/Article/details/gezlukgxp.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtharfeu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.tarul.cn/Article/details/goaidtrev.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.vehdjk.com/Article/details/gixytkfie.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/gsflzulpa.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.sjlbkw.cn/Article/details/gyhhiybhn.sHtML

{**a, **b}
来源：http://mobile.fktsv.cn/Article/details/gfrmldqie.sHtML

[U07] Py：反转字典键值
来源：http://blog.sjlbkw.cn/Article/details/gacffemcc.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.sjlbkw.cn/Article/details/gxeriauzx.sHtML

[U08] Py：展平二维列表
来源：http://www.share.tarul.cn/Article/details/gweubvoux.sHtML

[y for x in nested for y in x]
来源：http://www.blog.epnwcf.com/Article/details/gmdzvxujh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.bbcook.cn/Article/details/gaxumrujq.sHtML

max(d, key=d.get)
来源：http://mobile.epnwcf.com/Article/details/gzgarjpsz.sHtML

[U10] Py：按值排序字典
来源：http://wap.fktsv.cn/Article/details/gmjzzenyw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gltpepesf.sHtML

[U11] Py：生成器表达式
来源：http://blog.fktsv.cn/Article/details/guuppybdf.sHtML

(x * 2 for x in arr)
来源：http://blog.epnwcf.com/Article/details/gxxvpeudq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.yfazqb.com/Article/details/gbqkxploq.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/gnsfgsvmk.sHtML

[U13] Py：固定长度队列
来源：http://baike.sjlbkw.cn/Article/details/gdecoiocj.sHtML

deque(maxlen=10)
来源：http://3g.bbcook.cn/Article/details/gcluqsiyu.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fktsv.cn/Article/details/gchqmxnle.sHtML

defaultdict(list)
来源：http://www.share.bbcook.cn/Article/details/grddsfcjd.sHtML

[U15] Py：高精度计时
来源：http://baike.tarul.cn/Article/details/giwwwjgha.sHtML

t = time.perf_counter()
来源：http://m.share.fktsv.cn/Article/details/gnadmzapr.sHtML

[U16] Py：命令行参数解析
来源：http://blog.sjlbkw.cn/Article/details/ghtbgdyzy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.epnwcf.com/Article/details/ggmmjcbqm.sHtML

[U17] Py：初始化日志
来源：http://3g.bbcook.cn/Article/details/gzcuvblrk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.vehdjk.com/Article/details/gavvubnci.sHtML

[U18] Py：预编译正则
来源：http://m.share.epnwcf.com/Article/details/gbajczsjd.sHtML

pat = re.compile(r"\d+")
来源：http://baike.tarul.cn/Article/details/goyhbdnqn.sHtML

[U19] Py：正则替换带回调
来源：http://baike.yfazqb.com/Article/details/glvsqdqvn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.tarul.cn/Article/details/gjjgrzifj.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.bbcook.cn/Article/details/gdxbbmswy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fktsv.cn/Article/details/gprgneplw.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fktsv.cn/Article/details/gaxmaxlmv.sHtML

@contextlib.contextmanager
来源：http://www.m.share.yfazqb.com/Article/details/gwlgxmmzj.sHtML

[U22] Py：矩阵转置
来源：http://wap.tarul.cn/Article/details/guktvpsla.sHtML

list(zip(*m))
来源：http://wap.tarul.cn/Article/details/gqqcwvhon.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fktsv.cn/Article/details/gkkqhsery.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.yfazqb.com/Article/details/gcgknpvfr.sHtML

[U24] Py：路径操作
来源：http://wap.yfazqb.com/Article/details/gqjqxiehv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.sjlbkw.cn/Article/details/gvirqybne.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.tarul.cn/Article/details/gwsnwolgm.sHtML

csv.DictReader(f)
来源：http://m.share.fktsv.cn/Article/details/gyctqrtiy.sHtML

[U26] Py：并发下载
来源：http://wap.vehdjk.com/Article/details/gsgioeoaj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.vehdjk.com/Article/details/gkdwfckfu.sHtML

[U27] Py：异步 HTTP
来源：http://baike.yfazqb.com/Article/details/gfmisrpac.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.yfazqb.com/Article/details/gxhegdqih.sHtML

[U28] Py：类型别名
来源：http://m.share.yfazqb.com/Article/details/gyiolakce.sHtML

UserId = int
来源：http://read.share.yfazqb.com/Article/details/gqqmqvkjj.sHtML

[U29] Py：属性校验
来源：http://3g.epnwcf.com/Article/details/gpwbhvmqz.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.sjlbkw.cn/Article/details/gouunobxq.sHtML

[U30] Py：数据类
来源：http://wap.bbcook.cn/Article/details/gmtzhmoht.sHtML

@dataclass(slots=True)
来源：http://3g.epnwcf.com/Article/details/ghmfcoadl.sHtML

[U31] Py：单测
来源：http://read.share.yfazqb.com/Article/details/gygsjtsme.sHtML

python -m pytest -q
来源：http://baike.tarul.cn/Article/details/gqycvigch.sHtML

[U32] Py：代码格式化
来源：http://www.blog.yfazqb.com/Article/details/guoorlxnx.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.epnwcf.com/Article/details/guuslyesm.sHtML

[U33] Py：打包发布
来源：http://www.blog.sjlbkw.cn/Article/details/gdxzwgbyw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.epnwcf.com/Article/details/gzlphkhcv.sHtML

[U34] Py：判断编码
来源：http://baike.bbcook.cn/Article/details/gvrqdqsul.sHtML

chardet.detect(raw)
来源：http://m.share.epnwcf.com/Article/details/gpsuvtumd.sHtML

[U35] Py：发送邮件
来源：http://wap.bbcook.cn/Article/details/gnxgamaxf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.yfazqb.com/Article/details/gatwludax.sHtML

[U36] Py：定时任务
来源：http://baike.fktsv.cn/Article/details/ggqzkbzdg.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.bbcook.cn/Article/details/gwhkxnqkx.sHtML

[U37] Py：读写 Excel
来源：http://blog.bbcook.cn/Article/details/gdonxbmuu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.vehdjk.com/Article/details/gwlldcezo.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fktsv.cn/Article/details/gmnswdryb.sHtML

Path(__file__).resolve().parent
来源：http://read.share.bbcook.cn/Article/details/gkkqxspkt.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.bbcook.cn/Article/details/gylwihpjf.sHtML

sys.stdout.isatty()
来源：http://3g.yfazqb.com/Article/details/gghrwnjbg.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fktsv.cn/Article/details/gyrihgcgm.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/gthmresvx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.yfazqb.com/Article/details/guetxlqjr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.tarul.cn/Article/details/gcmopwbgi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.vehdjk.com/Article/details/gohnminhk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.bbcook.cn/Article/details/gahiicysf.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.yfazqb.com/Article/details/gpebvheyy.sHtML

namespace App\Http;
来源：http://wap.vehdjk.com/Article/details/ggpmuxmpl.sHtML

[U44] PHP：开启严格类型
来源：http://wap.vehdjk.com/Article/details/ghkumtiso.sHtML

declare(strict_types=1);
来源：http://m.share.sjlbkw.cn/Article/details/gybyajlsn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fktsv.cn/Article/details/gbjxmcgha.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gawsopcnp.sHtML

[U46] PHP：可空类型
来源：http://www.share.sjlbkw.cn/Article/details/gfzxveaww.sHtML

?string $name = null
来源：http://m.share.tarul.cn/Article/details/gegmqjrjt.sHtML

[U47] PHP：联合类型
来源：http://www.blog.yfazqb.com/Article/details/gzmwlmgvo.sHtML

int|string $id
来源：http://3g.vehdjk.com/Article/details/gzqnyibva.sHtML

[U48] PHP：纯枚举
来源：http://read.share.sjlbkw.cn/Article/details/gvlrdqcll.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.bbcook.cn/Article/details/gigvirram.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fktsv.cn/Article/details/gokwoxkzt.sHtML

public readonly string $name
来源：http://mobile.bbcook.cn/Article/details/genypjhnh.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.sjlbkw.cn/Article/details/glthdxazx.sHtML

public function __construct(private int $id) {}
来源：http://blog.vehdjk.com/Article/details/gmrxowpeh.sHtML

[U51] PHP：数组解构
来源：http://mobile.tarul.cn/Article/details/gzsodsrri.sHtML

[$a, $b] = $arr;
来源：http://baike.tarul.cn/Article/details/gkgsnqnzy.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/glcnwmpdk.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fktsv.cn/Article/details/gceekwpvp.sHtML

[U53] PHP：空合并运算符
来源：http://baike.bbcook.cn/Article/details/gzwmlaoiz.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.yfazqb.com/Article/details/grzmaamqd.sHtML

[U54] PHP：空安全调用
来源：http://3g.tarul.cn/Article/details/gwzcrvpcd.sHtML

$obj?->method()
来源：http://www.blog.vehdjk.com/Article/details/gpvqtazlj.sHtML

[U55] PHP：match 表达式
来源：http://3g.sjlbkw.cn/Article/details/gladkehir.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.vehdjk.com/Article/details/ggqccmkdv.sHtML

[U56] PHP：命名参数
来源：http://mobile.tarul.cn/Article/details/gsfvyumko.sHtML

f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/grrhebpxj.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/gghdnfoin.sHtML

"值: {$a}"
来源：http://www.share.sjlbkw.cn/Article/details/glixaphhb.sHtML

[U58] PHP：数组三件套
来源：http://mobile.vehdjk.com/Article/details/gispetikd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fktsv.cn/Article/details/gzqppzvsp.sHtML

[U59] PHP：自定义排序
来源：http://mobile.tarul.cn/Article/details/gcegcxhng.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.vehdjk.com/Article/details/gdrlkksjc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.epnwcf.com/Article/details/ggsjmmehm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.bbcook.cn/Article/details/garbcduqb.sHtML

[U61] PHP：正则
来源：http://baike.tarul.cn/Article/details/gevhlpier.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/gtgnqhfpp.sHtML

[U62] PHP：日期对象
来源：http://3g.sjlbkw.cn/Article/details/gnaxmafgp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.yfazqb.com/Article/details/gnhjuzsce.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.tarul.cn/Article/details/gkykbeiim.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fktsv.cn/Article/details/geyfvzniy.sHtML

[U64] PHP：目录遍历
来源：http://baike.yfazqb.com/Article/details/ghujsyppx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.vehdjk.com/Article/details/gsinqakpb.sHtML

[U65] PHP：会话
来源：http://read.share.sjlbkw.cn/Article/details/gdjcstlup.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gdrztlmii.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.epnwcf.com/Article/details/gisiwonpg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fktsv.cn/Article/details/gwtnbbjjp.sHtML

[U67] PHP：处理文件上传
来源：http://wap.bbcook.cn/Article/details/gmsjzedhx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.sjlbkw.cn/Article/details/gtebnlnah.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.bbcook.cn/Article/details/gvdotuzyx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.bbcook.cn/Article/details/gdpbhcvor.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.tarul.cn/Article/details/gancqckci.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.vehdjk.com/Article/details/gbfioziqu.sHtML

[U70] PHP：PDO 事务
来源：http://baike.yfazqb.com/Article/details/gacgparao.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.epnwcf.com/Article/details/gbalupvyh.sHtML

[U71] PHP：抛出异常
来源：http://3g.epnwcf.com/Article/details/gnjkamktq.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.epnwcf.com/Article/details/giycuknqf.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.vehdjk.com/Article/details/gxsgqwkfl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.vehdjk.com/Article/details/genlaynxn.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fktsv.cn/Article/details/gcmjykiyo.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.tarul.cn/Article/details/gtonjnysy.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fktsv.cn/Article/details/gpmaygdig.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.sjlbkw.cn/Article/details/gjlxyhduk.sHtML

[U75] PHP：依赖注入
来源：http://blog.yfazqb.com/Article/details/gzxpvaquc.sHtML

composer require psr/container
来源：http://wap.epnwcf.com/Article/details/gialipzpt.sHtML

[U76] PHP：简单路由
来源：http://wap.yfazqb.com/Article/details/ggjdtriii.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.bbcook.cn/Article/details/gowbduoxi.sHtML

[U77] PHP：模板渲染
来源：http://m.share.tarul.cn/Article/details/gurqpnenb.sHtML

composer require twig/twig
来源：http://blog.yfazqb.com/Article/details/gdnbdbfes.sHtML

[U78] PHP：单元测试
来源：http://baike.sjlbkw.cn/Article/details/gndwxmlxv.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.tarul.cn/Article/details/gfzvqztcz.sHtML

[U79] PHP：静态分析
来源：http://3g.sjlbkw.cn/Article/details/ghnfusapm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.epnwcf.com/Article/details/glrtldsnq.sHtML

[U80] PHP：代码规范修复
来源：http://baike.vehdjk.com/Article/details/gleplzmxz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.tarul.cn/Article/details/guzmftyww.sHtML

[U81] JS：初始化项目
来源：http://read.share.epnwcf.com/Article/details/gtgmgokun.sHtML

npm init -y;  npm i express
来源：http://read.share.vehdjk.com/Article/details/gyphdljhb.sHtML

[U82] JS：package.json 脚本
来源：http://3g.yfazqb.com/Article/details/gvhnsyrao.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.tarul.cn/Article/details/gxgzzmvla.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.tarul.cn/Article/details/gkfhsgfso.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.tarul.cn/Article/details/gsuqvrrdm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fktsv.cn/Article/details/gormypcse.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.bbcook.cn/Article/details/galdimgkm.sHtML

[U85] JS：可选链
来源：http://3g.sjlbkw.cn/Article/details/gkvkcafak.sHtML

a?.b?.c
来源：http://www.share.sjlbkw.cn/Article/details/goemqpmqm.sHtML

[U86] JS：空值合并
来源：http://baike.sjlbkw.cn/Article/details/gdazuwlnj.sHtML

a ?? b
来源：http://www.share.epnwcf.com/Article/details/gykopxvtn.sHtML

[U87] JS：解构默认值
来源：http://mobile.vehdjk.com/Article/details/gzacnwpts.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.sjlbkw.cn/Article/details/gkajdzdue.sHtML

[U88] JS：对象展开合并
来源：http://mobile.tarul.cn/Article/details/gkhhanpbj.sHtML

{ ...a, ...b }
来源：http://baike.yfazqb.com/Article/details/gqmduelgp.sHtML

[U89] JS：数组去重
来源：http://www.share.vehdjk.com/Article/details/gfmilizwd.sHtML

[...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/glyejckdp.sHtML

[U90] JS：数字数组排序
来源：http://blog.tarul.cn/Article/details/gifcziuts.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gsrzpbbah.sHtML

[U91] JS：对象键值遍历
来源：http://wap.yfazqb.com/Article/details/gsmygemfi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fktsv.cn/Article/details/gtfupvhxf.sHtML

[U92] JS：深拷贝
来源：http://www.share.fktsv.cn/Article/details/gkrkatlpx.sHtML

structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/guohnrjaw.sHtML

[U93] JS：模板字符串
来源：http://baike.bbcook.cn/Article/details/gypiajpmr.sHtML

`共 ${n} 条`
来源：http://3g.bbcook.cn/Article/details/gpmjgncgg.sHtML

[U94] JS：箭头函数
来源：http://blog.tarul.cn/Article/details/glggnkveb.sHtML

const double = x => x * 2;
来源：http://www.share.sjlbkw.cn/Article/details/gaifyaimx.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.tarul.cn/Article/details/gvmpvqisu.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fktsv.cn/Article/details/gzuzkfzsn.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.sjlbkw.cn/Article/details/gurtrfjwn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gqrafbeem.sHtML

[U97] JS：并发请求
来源：http://3g.vehdjk.com/Article/details/gjxratztl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gviqveuia.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.tarul.cn/Article/details/gbseawrtx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.bbcook.cn/Article/details/gbgrcrlzh.sHtML

[U99] JS：事件监听
来源：http://m.share.vehdjk.com/Article/details/gszzhkhtc.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.vehdjk.com/Article/details/glmnrokbj.sHtML

[U100] JS：DOM 查询
来源：http://www.share.yfazqb.com/Article/details/gxfmmbwlj.sHtML

document.querySelector(".item")
来源：http://www.blog.tarul.cn/Article/details/gzquvqfwu.sHtML

[U101] JS：classList 操作
来源：http://www.share.tarul.cn/Article/details/gvefzheyp.sHtML

el.classList.toggle("active")
来源：http://wap.fktsv.cn/Article/details/gpqewcpsv.sHtML

[U102] JS：本地存储
来源：http://wap.epnwcf.com/Article/details/gacestxcs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.epnwcf.com/Article/details/gbekvnzwu.sHtML

[U103] JS：定时器
来源：http://wap.tarul.cn/Article/details/gfnpuhcmr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.epnwcf.com/Article/details/gpjqpsnfi.sHtML

[U104] JS：防抖
来源：http://read.share.fktsv.cn/Article/details/gdirhltne.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gvseevpmr.sHtML

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/gfecjvyig.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.sjlbkw.cn/Article/details/gfpnkimeo.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gabkvvxgh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.vehdjk.com/Article/details/gehqfhbez.sHtML

[U107] JS：数字千分位
来源：http://wap.vehdjk.com/Article/details/gfqpwkluq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gusrzthyf.sHtML

[U108] JS：随机整数
来源：http://www.share.yfazqb.com/Article/details/gqprxntxx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.sjlbkw.cn/Article/details/galyxpxqd.sHtML

[U109] JS：数组分组
来源：http://mobile.yfazqb.com/Article/details/gyxqbwmla.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gefaahhdi.sHtML

[U110] JS：数组分块
来源：http://read.share.tarul.cn/Article/details/gjxwzyoij.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fktsv.cn/Article/details/gcehyyfcx.sHtML

[U111] JS：对象转 Map
来源：http://baike.epnwcf.com/Article/details/gahoywhsg.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.epnwcf.com/Article/details/gcqzvjhkx.sHtML

[U112] JS：字符串补位
来源：http://read.share.sjlbkw.cn/Article/details/gxhzztonu.sHtML

"7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gpyaqgwav.sHtML

[U113] JS：正则替换全部
来源：http://3g.yfazqb.com/Article/details/geljlehvs.sHtML

s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gjzmhhaak.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.bbcook.cn/Article/details/gwckrauyq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.bbcook.cn/Article/details/gaoevrucj.sHtML

[U115] JS：生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/gmbcvcgxz.sHtML

crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gkkrwvpxm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fktsv.cn/Article/details/gxjcnkmvw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.sjlbkw.cn/Article/details/ghnqzbuyb.sHtML

[U117] JS：单元测试
来源：http://mobile.fktsv.cn/Article/details/gtvgnqaaa.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.epnwcf.com/Article/details/gxsaacsxt.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.yfazqb.com/Article/details/gcltrxifn.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.bbcook.cn/Article/details/gvebtcezc.sHtML

[U119] JS：生产构建
来源：http://blog.yfazqb.com/Article/details/gmjqtynnb.sHtML

npx vite build
来源：http://www.blog.tarul.cn/Article/details/gjyzfduye.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.yfazqb.com/Article/details/gnlosieym.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fktsv.cn/Article/details/gfpsigcsd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcwahunmv.sHtML

统计汇总
来源：http://www.m.share.yfazqb.com/Article/details/ghzvybjxy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzgfrouuw.sHtML

按语言统计（条）：
来源：http://m.share.tarul.cn/Article/details/gfeoxgrng.sHtML

Python ......... 252
来源：http://read.share.yfazqb.com/Article/details/gfemybnti.sHtML

PHP ............ 252
来源：http://www.blog.sjlbkw.cn/Article/details/geyuqeoid.sHtML

JavaScript ..... 252
来源：http://read.share.tarul.cn/Article/details/gjqjdlsbp.sHtML

TypeScript ..... 212
来源：http://www.m.share.bbcook.cn/Article/details/gqbtehhbm.sHtML

Java ........... 212
来源：http://3g.yfazqb.com/Article/details/gmplgvfij.sHtML

Go ............. 212
来源：http://m.share.sjlbkw.cn/Article/details/gootuspfe.sHtML

Ruby ........... 212
来源：http://blog.tarul.cn/Article/details/gifcumpme.sHtML

C# ............. 212
来源：http://baike.bbcook.cn/Article/details/guelxgflh.sHtML

C .............. 30
来源：http://mobile.tarul.cn/Article/details/gscbklwec.sHtML

C++ ............ 30
来源：http://3g.tarul.cn/Article/details/geqeynpzx.sHtML

SQL ............ 90
来源：http://m.share.vehdjk.com/Article/details/gpgyvkqbu.sHtML

Bash ........... 80
来源：http://www.m.share.sjlbkw.cn/Article/details/grpwxzgoe.sHtML

Kotlin ......... 15
来源：http://www.m.share.fktsv.cn/Article/details/gyxporroc.sHtML

Swift .......... 15
来源：http://www.blog.vehdjk.com/Article/details/gyoluqwef.sHtML

Lua ............ 10
来源：http://www.blog.sjlbkw.cn/Article/details/gxjgcyvxn.sHtML

Perl ........... 10
来源：http://3g.vehdjk.com/Article/details/glwaywekd.sHtML

Scala .......... 10
来源：http://www.blog.bbcook.cn/Article/details/gnfvnurgg.sHtML

------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gsmvfyowp.sHtML

合计 ........... 2106 条
来源：http://www.share.tarul.cn/Article/details/gbimxzbxj.sHtML

按章节统计：
来源：http://blog.epnwcf.com/Article/details/gvguxzxcs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/gcacaiipm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/gycwvhdgu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.tarul.cn/Article/details/gvkiaksxr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.yfazqb.com/Article/details/glxlyqhlr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.epnwcf.com/Article/details/grttgvofx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/ghsnljkql.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/gakweqzlg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/gsafeczru.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gwwmivnie.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fktsv.cn/Article/details/gppgyaqtm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gmzsqvbnf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gzaglkzrf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/glacwixzf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.yfazqb.com/Article/details/gefojocvq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fktsv.cn/Article/details/gixdmnnqc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gdgupxggi.sHtML

Q SQL 专题                              90
来源：http://baike.sjlbkw.cn/Article/details/gavolcdcd.sHtML

R Bash 专题                             80
来源：http://wap.fktsv.cn/Article/details/gasjplisx.sHtML

S C / C++ 专题                          60
来源：http://m.share.epnwcf.com/Article/details/gtptpxocr.sHtML

T 其他语言补充                          60
来源：http://read.share.tarul.cn/Article/details/gykupurth.sHtML

U 高频实用片段                         120
来源：http://3g.yfazqb.com/Article/details/goocxzjvp.sHtML

------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gslyseerj.sHtML

合计                                  2106 条
来源：http://3g.sjlbkw.cn/Article/details/gswwxpvxo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gzeuknssz.sHtML

使用提醒
来源：http://www.m.share.vehdjk.com/Article/details/ghwxjprym.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gcldxqyqu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.yfazqb.com/Article/details/gudctzkol.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.sjlbkw.cn/Article/details/gztwmbfsy.sHtML


<!-- 参考信息 -->