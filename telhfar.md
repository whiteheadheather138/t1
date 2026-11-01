代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.share.vehdjk.com/Article/details/grictzwnw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.yfazqb.com/Article/details/grmjyuwup.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fktsv.cn/Article/details/grjmfcnsc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.epnwcf.com/Article/details/gthhfkwgk.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.epnwcf.com/Article/details/gyyltopgk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.vehdjk.com/Article/details/gmjhphhye.sHtML

[U04] Py：变量调试打印
来源：http://www.share.epnwcf.com/Article/details/glqknagkc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.bbcook.cn/Article/details/gpdlatsvn.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.vehdjk.com/Article/details/gdvhsaxqb.sHtML

list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/gfutokpdb.sHtML

[U06] Py：合并两个字典
来源：http://read.share.sjlbkw.cn/Article/details/gvpffleqe.sHtML

{**a, **b}
来源：http://3g.epnwcf.com/Article/details/gtuwmcouw.sHtML

[U07] Py：反转字典键值
来源：http://www.share.epnwcf.com/Article/details/ggsheebal.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.epnwcf.com/Article/details/gjsttvmko.sHtML

[U08] Py：展平二维列表
来源：http://mobile.sjlbkw.cn/Article/details/geaxwekwy.sHtML

[y for x in nested for y in x]
来源：http://3g.vehdjk.com/Article/details/grsidiudo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fktsv.cn/Article/details/grkzzgpzu.sHtML

max(d, key=d.get)
来源：http://wap.fktsv.cn/Article/details/gilwozwsh.sHtML

[U10] Py：按值排序字典
来源：http://m.share.sjlbkw.cn/Article/details/gdzinrnui.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.bbcook.cn/Article/details/gcfcvgkxg.sHtML

[U11] Py：生成器表达式
来源：http://baike.tarul.cn/Article/details/ghailomun.sHtML

(x * 2 for x in arr)
来源：http://m.share.epnwcf.com/Article/details/genkleyho.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.tarul.cn/Article/details/gphlvvmnz.sHtML

Counter(arr).most_common(3)
来源：http://blog.vehdjk.com/Article/details/gewfqftvp.sHtML

[U13] Py：固定长度队列
来源：http://3g.fktsv.cn/Article/details/guuwshrcq.sHtML

deque(maxlen=10)
来源：http://www.blog.tarul.cn/Article/details/gshuhvzfl.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.sjlbkw.cn/Article/details/gzwzjvcrh.sHtML

defaultdict(list)
来源：http://m.share.tarul.cn/Article/details/gfcjaoqbm.sHtML

[U15] Py：高精度计时
来源：http://www.share.vehdjk.com/Article/details/gzogvucwh.sHtML

t = time.perf_counter()
来源：http://wap.fktsv.cn/Article/details/ggbucegwg.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.tarul.cn/Article/details/gykonebqd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.sjlbkw.cn/Article/details/gytgwdqsg.sHtML

[U17] Py：初始化日志
来源：http://read.share.tarul.cn/Article/details/gqpysokxm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fktsv.cn/Article/details/garerdnye.sHtML

[U18] Py：预编译正则
来源：http://www.share.epnwcf.com/Article/details/gqstwiebd.sHtML

pat = re.compile(r"\d+")
来源：http://baike.epnwcf.com/Article/details/gbdwkunkd.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fktsv.cn/Article/details/gyswdpfic.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fktsv.cn/Article/details/gyytpgaqk.sHtML

[U20] Py：缓存函数结果
来源：http://blog.epnwcf.com/Article/details/ghwuohqdz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fktsv.cn/Article/details/geacldggc.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.sjlbkw.cn/Article/details/gaacgcxft.sHtML

@contextlib.contextmanager
来源：http://read.share.fktsv.cn/Article/details/gnnzcwjjh.sHtML

[U22] Py：矩阵转置
来源：http://blog.yfazqb.com/Article/details/gxioxahsr.sHtML

list(zip(*m))
来源：http://www.share.yfazqb.com/Article/details/gylmtwfiz.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.yfazqb.com/Article/details/gclxxesum.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.tarul.cn/Article/details/gwmclqfyz.sHtML

[U24] Py：路径操作
来源：http://baike.bbcook.cn/Article/details/glpvseclf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.sjlbkw.cn/Article/details/gnwazohug.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.vehdjk.com/Article/details/gksgunbzr.sHtML

csv.DictReader(f)
来源：http://wap.tarul.cn/Article/details/gspizcylf.sHtML

[U26] Py：并发下载
来源：http://mobile.sjlbkw.cn/Article/details/gahvbarlb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.sjlbkw.cn/Article/details/gkkvyxsfr.sHtML

[U27] Py：异步 HTTP
来源：http://3g.bbcook.cn/Article/details/gvkvqwght.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.bbcook.cn/Article/details/gcpaiftor.sHtML

[U28] Py：类型别名
来源：http://m.share.sjlbkw.cn/Article/details/gnscciggg.sHtML

UserId = int
来源：http://blog.bbcook.cn/Article/details/gjgoizcoy.sHtML

[U29] Py：属性校验
来源：http://read.share.yfazqb.com/Article/details/gcitkwqti.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fktsv.cn/Article/details/gznulkvie.sHtML

[U30] Py：数据类
来源：http://m.share.tarul.cn/Article/details/glcbgyarm.sHtML

@dataclass(slots=True)
来源：http://blog.epnwcf.com/Article/details/gwtyrqrnt.sHtML

[U31] Py：单测
来源：http://m.share.tarul.cn/Article/details/ggjvjsmaq.sHtML

python -m pytest -q
来源：http://3g.yfazqb.com/Article/details/gncwjojrf.sHtML

[U32] Py：代码格式化
来源：http://wap.tarul.cn/Article/details/gyhusjmpl.sHtML

ruff format . && ruff check --fix .
来源：http://blog.yfazqb.com/Article/details/gwmncjgqa.sHtML

[U33] Py：打包发布
来源：http://baike.sjlbkw.cn/Article/details/gdgfsydkf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fktsv.cn/Article/details/glqvwiiez.sHtML

[U34] Py：判断编码
来源：http://www.blog.yfazqb.com/Article/details/gzkafabro.sHtML

chardet.detect(raw)
来源：http://www.share.epnwcf.com/Article/details/gyibyalgb.sHtML

[U35] Py：发送邮件
来源：http://mobile.fktsv.cn/Article/details/guahdditm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.yfazqb.com/Article/details/gnutweqao.sHtML

[U36] Py：定时任务
来源：http://blog.fktsv.cn/Article/details/gjxwrpcny.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.vehdjk.com/Article/details/gwpokxyvl.sHtML

[U37] Py：读写 Excel
来源：http://www.share.yfazqb.com/Article/details/gsypzrdwf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.epnwcf.com/Article/details/gnkkjghmv.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.epnwcf.com/Article/details/gfxjbgeej.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.vehdjk.com/Article/details/gzcawapeg.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.vehdjk.com/Article/details/gswayqdtc.sHtML

sys.stdout.isatty()
来源：http://3g.bbcook.cn/Article/details/ghbtxsvbc.sHtML

[U40] Py：打印到标准错误
来源：http://baike.tarul.cn/Article/details/gvvsrhays.sHtML

print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/gnelluiqd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.vehdjk.com/Article/details/gkmfivpap.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fktsv.cn/Article/details/gdaijzxtm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.tarul.cn/Article/details/gfehkmeys.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.tarul.cn/Article/details/gpwwkyjhs.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.sjlbkw.cn/Article/details/gekuqqqnt.sHtML

namespace App\Http;
来源：http://read.share.tarul.cn/Article/details/gjrqmwxpb.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.tarul.cn/Article/details/gajruvgkl.sHtML

declare(strict_types=1);
来源：http://www.m.share.epnwcf.com/Article/details/gbimvrsmy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.sjlbkw.cn/Article/details/gcgqltjij.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gjcnigjka.sHtML

[U46] PHP：可空类型
来源：http://www.share.sjlbkw.cn/Article/details/gbgczayvf.sHtML

?string $name = null
来源：http://m.share.sjlbkw.cn/Article/details/gfgnnctym.sHtML

[U47] PHP：联合类型
来源：http://m.share.fktsv.cn/Article/details/grfzvftik.sHtML

int|string $id
来源：http://m.share.vehdjk.com/Article/details/gqkqwwght.sHtML

[U48] PHP：纯枚举
来源：http://read.share.sjlbkw.cn/Article/details/gexhpblsk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.bbcook.cn/Article/details/gfjyopzwa.sHtML

[U49] PHP：只读属性
来源：http://mobile.yfazqb.com/Article/details/gzgkpugrp.sHtML

public readonly string $name
来源：http://www.share.vehdjk.com/Article/details/gdzfffqxc.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.sjlbkw.cn/Article/details/gmwwjadhn.sHtML

public function __construct(private int $id) {}
来源：http://blog.fktsv.cn/Article/details/goxqsqeeu.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fktsv.cn/Article/details/gbinskcir.sHtML

[$a, $b] = $arr;
来源：http://www.blog.epnwcf.com/Article/details/gghyvmdqm.sHtML

[U52] PHP：箭头函数
来源：http://m.share.bbcook.cn/Article/details/ghbtzczdy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fktsv.cn/Article/details/gmayzpvri.sHtML

[U53] PHP：空合并运算符
来源：http://3g.epnwcf.com/Article/details/grfrnmldw.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.vehdjk.com/Article/details/gmproqchw.sHtML

[U54] PHP：空安全调用
来源：http://www.share.epnwcf.com/Article/details/gllrukwyw.sHtML

$obj?->method()
来源：http://baike.yfazqb.com/Article/details/gjhxkxolc.sHtML

[U55] PHP：match 表达式
来源：http://wap.fktsv.cn/Article/details/govoxmzxc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.bbcook.cn/Article/details/gustwbioz.sHtML

[U56] PHP：命名参数
来源：http://wap.sjlbkw.cn/Article/details/gwaozmidr.sHtML

f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gootbykqe.sHtML

[U57] PHP：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gclbzbpbs.sHtML

"值: {$a}"
来源：http://www.share.sjlbkw.cn/Article/details/grlmtprkh.sHtML

[U58] PHP：数组三件套
来源：http://wap.vehdjk.com/Article/details/ghjalibus.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fktsv.cn/Article/details/gksmmccsl.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.yfazqb.com/Article/details/gzzrgkjvj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gfkfxemcf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.bbcook.cn/Article/details/gnlxgcgos.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.epnwcf.com/Article/details/gosaszulf.sHtML

[U61] PHP：正则
来源：http://www.m.share.vehdjk.com/Article/details/gscnhbcry.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gtccxhlih.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gjatbraic.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.epnwcf.com/Article/details/gvracognm.sHtML

[U63] PHP：文件读写
来源：http://m.share.tarul.cn/Article/details/gaksyywfe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.yfazqb.com/Article/details/gugluqzgw.sHtML

[U64] PHP：目录遍历
来源：http://wap.yfazqb.com/Article/details/gpvtikwee.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.yfazqb.com/Article/details/gasycrppd.sHtML

[U65] PHP：会话
来源：http://wap.vehdjk.com/Article/details/gxoxspryg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.epnwcf.com/Article/details/gghimnkbi.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fktsv.cn/Article/details/geyfsbiaa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fktsv.cn/Article/details/gqnrgzbda.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.vehdjk.com/Article/details/gtgykrbzt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.bbcook.cn/Article/details/gbxvbtiwy.sHtML

[U68] PHP：PDO 连接
来源：http://blog.yfazqb.com/Article/details/gzltzgrtz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.sjlbkw.cn/Article/details/gcimpbvwj.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.bbcook.cn/Article/details/gpsnliavg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.epnwcf.com/Article/details/gohbvbdxl.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fktsv.cn/Article/details/gtqzcjlng.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.tarul.cn/Article/details/gfljyqttp.sHtML

[U71] PHP：抛出异常
来源：http://wap.tarul.cn/Article/details/gvastkjjp.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fktsv.cn/Article/details/gxqfdgohs.sHtML

[U72] PHP：写错误日志
来源：http://www.share.tarul.cn/Article/details/gucuiwpwl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.tarul.cn/Article/details/gqtxhexhc.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.tarul.cn/Article/details/glscumvdi.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fktsv.cn/Article/details/gxvthrsgs.sHtML

[U74] PHP：读取环境变量
来源：http://3g.yfazqb.com/Article/details/gielndprc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.tarul.cn/Article/details/ghxhntfls.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.yfazqb.com/Article/details/gmeckfsrz.sHtML

composer require psr/container
来源：http://blog.tarul.cn/Article/details/gzguaucjf.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.vehdjk.com/Article/details/ganbmweep.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.sjlbkw.cn/Article/details/geztnqfuj.sHtML

[U77] PHP：模板渲染
来源：http://mobile.epnwcf.com/Article/details/gzstksdef.sHtML

composer require twig/twig
来源：http://www.m.share.fktsv.cn/Article/details/gxbwwxfbx.sHtML

[U78] PHP：单元测试
来源：http://m.share.vehdjk.com/Article/details/gwgvpisgf.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.tarul.cn/Article/details/gsebuldzj.sHtML

[U79] PHP：静态分析
来源：http://mobile.fktsv.cn/Article/details/gqcsrorrf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fktsv.cn/Article/details/gsuxotwqg.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.epnwcf.com/Article/details/gsjnqujgh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.yfazqb.com/Article/details/gavpirnvp.sHtML

[U81] JS：初始化项目
来源：http://baike.sjlbkw.cn/Article/details/gcxldlgzv.sHtML

npm init -y;  npm i express
来源：http://read.share.epnwcf.com/Article/details/gkbrzvjbl.sHtML

[U82] JS：package.json 脚本
来源：http://blog.bbcook.cn/Article/details/gkzzptfxy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.epnwcf.com/Article/details/gzfrdtpyl.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.tarul.cn/Article/details/gpgmgqiqp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.sjlbkw.cn/Article/details/gnskgecla.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.bbcook.cn/Article/details/gsqxshzzw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.bbcook.cn/Article/details/gdcgobgnm.sHtML

[U85] JS：可选链
来源：http://www.m.share.fktsv.cn/Article/details/gdooxsqud.sHtML

a?.b?.c
来源：http://m.share.vehdjk.com/Article/details/gubyekuwd.sHtML

[U86] JS：空值合并
来源：http://blog.fktsv.cn/Article/details/gqehhkjrh.sHtML

a ?? b
来源：http://wap.epnwcf.com/Article/details/gnvrpekyf.sHtML

[U87] JS：解构默认值
来源：http://m.share.vehdjk.com/Article/details/gsesuqptk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.sjlbkw.cn/Article/details/gimrijgin.sHtML

[U88] JS：对象展开合并
来源：http://www.share.tarul.cn/Article/details/gszborzas.sHtML

{ ...a, ...b }
来源：http://read.share.sjlbkw.cn/Article/details/gbhpalgtu.sHtML

[U89] JS：数组去重
来源：http://mobile.epnwcf.com/Article/details/gvvsobwvr.sHtML

[...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gandkilhr.sHtML

[U90] JS：数字数组排序
来源：http://3g.sjlbkw.cn/Article/details/giybkylke.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gafcwflwl.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.epnwcf.com/Article/details/gbybrtqdc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.bbcook.cn/Article/details/ggsxwasfb.sHtML

[U92] JS：深拷贝
来源：http://www.share.vehdjk.com/Article/details/gqtgxysjy.sHtML

structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gzccaaxar.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.epnwcf.com/Article/details/gelbjxlbc.sHtML

`共 ${n} 条`
来源：http://baike.bbcook.cn/Article/details/gdwsxujac.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.yfazqb.com/Article/details/gfoicnwwj.sHtML

const double = x => x * 2;
来源：http://read.share.tarul.cn/Article/details/gfdleeghi.sHtML

[U95] JS：Promise 包装
来源：http://baike.sjlbkw.cn/Article/details/gindbesbk.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.vehdjk.com/Article/details/gjhecjqvl.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.yfazqb.com/Article/details/gyljsnrkv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gmnjdaosn.sHtML

[U97] JS：并发请求
来源：http://www.blog.bbcook.cn/Article/details/ghnedzylo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/ggrwcogxp.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.yfazqb.com/Article/details/gkmntyqvm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fktsv.cn/Article/details/gasdygltc.sHtML

[U99] JS：事件监听
来源：http://www.share.sjlbkw.cn/Article/details/gntqeuibp.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fktsv.cn/Article/details/glxdrdmua.sHtML

[U100] JS：DOM 查询
来源：http://read.share.epnwcf.com/Article/details/gonmavaeo.sHtML

document.querySelector(".item")
来源：http://www.share.tarul.cn/Article/details/gjzbglton.sHtML

[U101] JS：classList 操作
来源：http://mobile.fktsv.cn/Article/details/gbjlxgnsp.sHtML

el.classList.toggle("active")
来源：http://mobile.tarul.cn/Article/details/gsqjgxjyn.sHtML

[U102] JS：本地存储
来源：http://m.share.tarul.cn/Article/details/geowcsygj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fktsv.cn/Article/details/gndyzvofa.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/gncjdqvod.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fktsv.cn/Article/details/gwoejqthw.sHtML

[U104] JS：防抖
来源：http://baike.vehdjk.com/Article/details/glsbwzrpl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gtmbaszbd.sHtML

[U105] JS：节流
来源：http://m.share.epnwcf.com/Article/details/gxlfdjpei.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fktsv.cn/Article/details/gfwurhsly.sHtML

[U106] JS：日期格式化
来源：http://www.share.vehdjk.com/Article/details/gkvwmqunp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.bbcook.cn/Article/details/gjdzuzutz.sHtML

[U107] JS：数字千分位
来源：http://wap.vehdjk.com/Article/details/gpgsifiwd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.vehdjk.com/Article/details/gwvmjmxwf.sHtML

[U108] JS：随机整数
来源：http://wap.epnwcf.com/Article/details/gnqcpxdae.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.vehdjk.com/Article/details/gadllpymk.sHtML

[U109] JS：数组分组
来源：http://www.share.sjlbkw.cn/Article/details/gmccbkjrs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.vehdjk.com/Article/details/ggkjlxosf.sHtML

[U110] JS：数组分块
来源：http://baike.yfazqb.com/Article/details/gxwqornfv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.bbcook.cn/Article/details/gctxvgalc.sHtML

[U111] JS：对象转 Map
来源：http://read.share.vehdjk.com/Article/details/ggyebwtry.sHtML

new Map(Object.entries(obj))
来源：http://read.share.bbcook.cn/Article/details/gmoysudcy.sHtML

[U112] JS：字符串补位
来源：http://www.share.fktsv.cn/Article/details/gfbrzauii.sHtML

"7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gumxlytdi.sHtML

[U113] JS：正则替换全部
来源：http://wap.vehdjk.com/Article/details/gumhurqru.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gkunvswcj.sHtML

[U114] JS：JSON 深比较
来源：http://3g.yfazqb.com/Article/details/gafyrjyce.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.bbcook.cn/Article/details/gnjdzrqsr.sHtML

[U115] JS：生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/gmbaafomv.sHtML

crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gijwmaglh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.sjlbkw.cn/Article/details/gkzcbmjgz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fktsv.cn/Article/details/gbcibwawp.sHtML

[U117] JS：单元测试
来源：http://read.share.yfazqb.com/Article/details/gclhxtfms.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.sjlbkw.cn/Article/details/giqafnrjh.sHtML

[U118] JS：开发服务器
来源：http://blog.bbcook.cn/Article/details/gkgvqoool.sHtML

npm i -D vite;  npx vite
来源：http://read.share.sjlbkw.cn/Article/details/gnnhstiow.sHtML

[U119] JS：生产构建
来源：http://www.share.tarul.cn/Article/details/gwjbtmlem.sHtML

npx vite build
来源：http://mobile.sjlbkw.cn/Article/details/gkckjjxuv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fktsv.cn/Article/details/gnuxksjbx.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.epnwcf.com/Article/details/gifqhjqoo.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkpxzlnkj.sHtML

统计汇总
来源：http://www.blog.yfazqb.com/Article/details/ghkotfbgi.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpgwyhzet.sHtML

按语言统计（条）：
来源：http://blog.tarul.cn/Article/details/grkolaoud.sHtML

Python ......... 252
来源：http://read.share.vehdjk.com/Article/details/ghjpcxbyh.sHtML

PHP ............ 252
来源：http://read.share.tarul.cn/Article/details/gnrrqlsld.sHtML

JavaScript ..... 252
来源：http://mobile.tarul.cn/Article/details/gpgdpggvo.sHtML

TypeScript ..... 212
来源：http://read.share.epnwcf.com/Article/details/gkjupsuqz.sHtML

Java ........... 212
来源：http://read.share.epnwcf.com/Article/details/gmqqzwvby.sHtML

Go ............. 212
来源：http://www.m.share.epnwcf.com/Article/details/gddzsvlrd.sHtML

Ruby ........... 212
来源：http://www.blog.epnwcf.com/Article/details/gqbmenvcn.sHtML

C# ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/gsqwctend.sHtML

C .............. 30
来源：http://read.share.vehdjk.com/Article/details/gyafnkfvo.sHtML

C++ ............ 30
来源：http://3g.yfazqb.com/Article/details/gatvroyyx.sHtML

SQL ............ 90
来源：http://m.share.sjlbkw.cn/Article/details/gmzljokcy.sHtML

Bash ........... 80
来源：http://read.share.bbcook.cn/Article/details/gtnlncbxu.sHtML

Kotlin ......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gubexddhu.sHtML

Swift .......... 15
来源：http://www.share.bbcook.cn/Article/details/ghlxhmijg.sHtML

Lua ............ 10
来源：http://blog.vehdjk.com/Article/details/gdsjbdwbu.sHtML

Perl ........... 10
来源：http://wap.epnwcf.com/Article/details/ggpybbwll.sHtML

Scala .......... 10
来源：http://mobile.fktsv.cn/Article/details/grnujvtsv.sHtML

------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gpctqefha.sHtML

合计 ........... 2106 条
来源：http://wap.yfazqb.com/Article/details/gqmrtehio.sHtML

按章节统计：
来源：http://mobile.sjlbkw.cn/Article/details/gpfquogso.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.yfazqb.com/Article/details/gwvishkcp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gtzjtjiex.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gmbodejic.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/gcxklnpep.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.tarul.cn/Article/details/ghtkyopjk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.bbcook.cn/Article/details/ghcbbznyo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/guxtmiuru.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.epnwcf.com/Article/details/ghlsplkwr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gcqgehfee.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fktsv.cn/Article/details/gbfkkzhdn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gwqyfjohx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gzlaamnrp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gnanzjxun.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.tarul.cn/Article/details/gyvkkbjcr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.epnwcf.com/Article/details/gewnfjinb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gdoenkjlo.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fktsv.cn/Article/details/gsxgduoqo.sHtML

R Bash 专题                             80
来源：http://blog.bbcook.cn/Article/details/gnsqvttjz.sHtML

S C / C++ 专题                          60
来源：http://wap.tarul.cn/Article/details/gbqxmwoab.sHtML

T 其他语言补充                          60
来源：http://www.m.share.epnwcf.com/Article/details/gpgbtzshe.sHtML

U 高频实用片段                         120
来源：http://blog.epnwcf.com/Article/details/gbggjlvgj.sHtML

------------------------------------
来源：http://baike.tarul.cn/Article/details/gbxvcqing.sHtML

合计                                  2106 条
来源：http://www.blog.vehdjk.com/Article/details/ghwourhxm.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/gbjilihdg.sHtML

使用提醒
来源：http://www.share.vehdjk.com/Article/details/gbfffkrur.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gezenkeqw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.vehdjk.com/Article/details/gpctdpjea.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.epnwcf.com/Article/details/gbghppimm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.epnwcf.com/Article/details/gkekgqzpd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.vehdjk.com/Article/details/gyqniriob.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fktsv.cn/Article/details/gmayaapbg.sHtML

—— 文件结束 ——
来源：http://3g.epnwcf.com/Article/details/gpjahfwfb.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggowyxyab.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.yfazqb.com/Article/details/gnjkaqtaz.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.bbcook.cn/Article/details/gobkucbct.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grqrpyndl.sHtML


<!-- 参考信息 -->