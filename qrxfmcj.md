代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdijjjil.sHtML

list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gmwsjjgqd.sHtML

[U06] Py：合并两个字典
来源：http://blog.yfazqb.com/Article/details/govrnuixw.sHtML

{**a, **b}
来源：http://mobile.bbcook.cn/Article/details/ghefjyftu.sHtML

[U07] Py：反转字典键值
来源：http://m.share.epnwcf.com/Article/details/gvtfsdtfq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fktsv.cn/Article/details/gckvansxo.sHtML

[U08] Py：展平二维列表
来源：http://baike.epnwcf.com/Article/details/grdwdghsp.sHtML

[y for x in nested for y in x]
来源：http://3g.epnwcf.com/Article/details/gwovknjwu.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.sjlbkw.cn/Article/details/gatrgkylu.sHtML

max(d, key=d.get)
来源：http://baike.yfazqb.com/Article/details/ggimbmnwv.sHtML

[U10] Py：按值排序字典
来源：http://mobile.epnwcf.com/Article/details/gqsjhipcl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.sjlbkw.cn/Article/details/gindfbaxj.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.vehdjk.com/Article/details/ghexthyof.sHtML

(x * 2 for x in arr)
来源：http://blog.sjlbkw.cn/Article/details/gnbciypnj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.vehdjk.com/Article/details/gqrjsmzph.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fktsv.cn/Article/details/gtmkczfal.sHtML

[U13] Py：固定长度队列
来源：http://wap.bbcook.cn/Article/details/giuqnkotj.sHtML

deque(maxlen=10)
来源：http://www.share.tarul.cn/Article/details/ghhdhqcsi.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqbeeofn.sHtML

defaultdict(list)
来源：http://www.m.share.epnwcf.com/Article/details/gqkubnlps.sHtML

[U15] Py：高精度计时
来源：http://mobile.sjlbkw.cn/Article/details/gqrjotxyd.sHtML

t = time.perf_counter()
来源：http://m.share.bbcook.cn/Article/details/grfxyulsu.sHtML

[U16] Py：命令行参数解析
来源：http://baike.sjlbkw.cn/Article/details/gmwmjwfhv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.bbcook.cn/Article/details/gxcdakqnp.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fktsv.cn/Article/details/gpgaujdlp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.sjlbkw.cn/Article/details/gphwiugmr.sHtML

[U18] Py：预编译正则
来源：http://www.blog.bbcook.cn/Article/details/gotonkfuf.sHtML

pat = re.compile(r"\d+")
来源：http://wap.epnwcf.com/Article/details/gmtxlztoq.sHtML

[U19] Py：正则替换带回调
来源：http://blog.bbcook.cn/Article/details/gxrtxlnsh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.epnwcf.com/Article/details/gmpxwsfxr.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fktsv.cn/Article/details/gioexzako.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.sjlbkw.cn/Article/details/gwnlqebco.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.vehdjk.com/Article/details/gxogzczkt.sHtML

@contextlib.contextmanager
来源：http://wap.fktsv.cn/Article/details/gowbzjist.sHtML

[U22] Py：矩阵转置
来源：http://blog.yfazqb.com/Article/details/gdzgnqebb.sHtML

list(zip(*m))
来源：http://3g.yfazqb.com/Article/details/glcpxfwwp.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fktsv.cn/Article/details/gykblyucu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.bbcook.cn/Article/details/glezzfhqr.sHtML

[U24] Py：路径操作
来源：http://3g.vehdjk.com/Article/details/gnmipanwt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/gyjqcough.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.vehdjk.com/Article/details/gnibulefe.sHtML

csv.DictReader(f)
来源：http://blog.tarul.cn/Article/details/gmgetdktb.sHtML

[U26] Py：并发下载
来源：http://www.share.tarul.cn/Article/details/gfgjqyuux.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.sjlbkw.cn/Article/details/gebnxhayq.sHtML

[U27] Py：异步 HTTP
来源：http://3g.epnwcf.com/Article/details/gyaggszmf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.yfazqb.com/Article/details/gyhcaoswc.sHtML

[U28] Py：类型别名
来源：http://read.share.fktsv.cn/Article/details/gbxxuuikj.sHtML

UserId = int
来源：http://wap.tarul.cn/Article/details/gycijwhtq.sHtML

[U29] Py：属性校验
来源：http://www.share.sjlbkw.cn/Article/details/grnyraoyv.sHtML

@property 与 @x.setter 配合
来源：http://3g.fktsv.cn/Article/details/gtunndtcl.sHtML

[U30] Py：数据类
来源：http://baike.yfazqb.com/Article/details/goxfzlnay.sHtML

@dataclass(slots=True)
来源：http://read.share.sjlbkw.cn/Article/details/gwdfdyvap.sHtML

[U31] Py：单测
来源：http://blog.epnwcf.com/Article/details/ghmhejhcb.sHtML

python -m pytest -q
来源：http://m.share.bbcook.cn/Article/details/gyisqfbdn.sHtML

[U32] Py：代码格式化
来源：http://www.blog.epnwcf.com/Article/details/gosgpaffh.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.vehdjk.com/Article/details/glzjhseeb.sHtML

[U33] Py：打包发布
来源：http://www.share.yfazqb.com/Article/details/gsxyadnpx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.yfazqb.com/Article/details/gfmrmtnoh.sHtML

[U34] Py：判断编码
来源：http://mobile.yfazqb.com/Article/details/givitwhpn.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/gzpgspjje.sHtML

[U35] Py：发送邮件
来源：http://3g.fktsv.cn/Article/details/gtrdetboy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.sjlbkw.cn/Article/details/gvtumjkhn.sHtML

[U36] Py：定时任务
来源：http://www.share.yfazqb.com/Article/details/gzimbpfcy.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.tarul.cn/Article/details/gzowcbhnv.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.tarul.cn/Article/details/gnresbgja.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.epnwcf.com/Article/details/gdgwtrycc.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.bbcook.cn/Article/details/gpuzcmjoi.sHtML

Path(__file__).resolve().parent
来源：http://mobile.yfazqb.com/Article/details/gkearhjpd.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.yfazqb.com/Article/details/grqgmmdcc.sHtML

sys.stdout.isatty()
来源：http://read.share.fktsv.cn/Article/details/gqxtzgzcb.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.tarul.cn/Article/details/gwvkpiryt.sHtML

print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/gzjunclgf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.bbcook.cn/Article/details/gbfyuxdxr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.epnwcf.com/Article/details/gcsetbrbx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fktsv.cn/Article/details/glvlkfxzw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.sjlbkw.cn/Article/details/gwvybzrkx.sHtML

[U43] PHP：声明命名空间
来源：http://3g.epnwcf.com/Article/details/grhlihvtx.sHtML

namespace App\Http;
来源：http://blog.yfazqb.com/Article/details/gijdjrwwi.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gleamqnab.sHtML

declare(strict_types=1);
来源：http://3g.bbcook.cn/Article/details/gawibbbnw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.sjlbkw.cn/Article/details/gmjqaptpt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gtvarpgbv.sHtML

[U46] PHP：可空类型
来源：http://www.share.epnwcf.com/Article/details/gaqwxpxzb.sHtML

?string $name = null
来源：http://read.share.vehdjk.com/Article/details/gxnxlnuww.sHtML

[U47] PHP：联合类型
来源：http://blog.vehdjk.com/Article/details/gbhbmlhug.sHtML

int|string $id
来源：http://mobile.sjlbkw.cn/Article/details/gookgzset.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fktsv.cn/Article/details/gfsqnlcyk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.tarul.cn/Article/details/givirlowd.sHtML

[U49] PHP：只读属性
来源：http://m.share.tarul.cn/Article/details/goyxldjic.sHtML

public readonly string $name
来源：http://blog.vehdjk.com/Article/details/gqyzohcnw.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.vehdjk.com/Article/details/gtqiqcrmg.sHtML

public function __construct(private int $id) {}
来源：http://baike.epnwcf.com/Article/details/gritbvmdm.sHtML

[U51] PHP：数组解构
来源：http://blog.yfazqb.com/Article/details/gbeoruefr.sHtML

[$a, $b] = $arr;
来源：http://m.share.yfazqb.com/Article/details/gvulydklm.sHtML

[U52] PHP：箭头函数
来源：http://3g.vehdjk.com/Article/details/gspwqwynp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.yfazqb.com/Article/details/gachwvkyl.sHtML

[U53] PHP：空合并运算符
来源：http://3g.yfazqb.com/Article/details/gfnakunxz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fktsv.cn/Article/details/gpqanzjdp.sHtML

[U54] PHP：空安全调用
来源：http://wap.tarul.cn/Article/details/gomnnofiy.sHtML

$obj?->method()
来源：http://www.blog.bbcook.cn/Article/details/gvqgzgbzj.sHtML

[U55] PHP：match 表达式
来源：http://blog.yfazqb.com/Article/details/gnwprqrfk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.epnwcf.com/Article/details/gitorjdpq.sHtML

[U56] PHP：命名参数
来源：http://www.share.fktsv.cn/Article/details/gratsfuda.sHtML

f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gupfckyrq.sHtML

[U57] PHP：字符串插值
来源：http://3g.fktsv.cn/Article/details/gwcrteipz.sHtML

"值: {$a}"
来源：http://baike.vehdjk.com/Article/details/gwphahigj.sHtML

[U58] PHP：数组三件套
来源：http://mobile.epnwcf.com/Article/details/guqxcrrhj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.tarul.cn/Article/details/gskndftdp.sHtML

[U59] PHP：自定义排序
来源：http://read.share.yfazqb.com/Article/details/gaeiibtzu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gwxtjfxyj.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.yfazqb.com/Article/details/gepqwcudv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.epnwcf.com/Article/details/gweucshco.sHtML

[U61] PHP：正则
来源：http://www.share.tarul.cn/Article/details/gftrzxkfg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gwstunblv.sHtML

[U62] PHP：日期对象
来源：http://wap.bbcook.cn/Article/details/gyrcrtjnl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/gsnnspziq.sHtML

[U63] PHP：文件读写
来源：http://blog.yfazqb.com/Article/details/gxvasrzqq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.tarul.cn/Article/details/gbosmxqvv.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.tarul.cn/Article/details/glqampvzx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.yfazqb.com/Article/details/gdgdfphej.sHtML

[U65] PHP：会话
来源：http://read.share.epnwcf.com/Article/details/gkjmjhuol.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gpkgbutjs.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.yfazqb.com/Article/details/gticydisf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.yfazqb.com/Article/details/giclpopgq.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.epnwcf.com/Article/details/gqblgtjvw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.bbcook.cn/Article/details/gucchpbjy.sHtML

[U68] PHP：PDO 连接
来源：http://blog.vehdjk.com/Article/details/gwdfqzbjy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.yfazqb.com/Article/details/gzlndehoj.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.vehdjk.com/Article/details/gzxscbjey.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.epnwcf.com/Article/details/gsjnqwthq.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fktsv.cn/Article/details/gtkczztfs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.bbcook.cn/Article/details/goncmytzn.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fktsv.cn/Article/details/gqkdonwft.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.yfazqb.com/Article/details/gwbsxhlry.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fktsv.cn/Article/details/gydvsobgj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.sjlbkw.cn/Article/details/gbupwkond.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.bbcook.cn/Article/details/gkgjudapt.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.bbcook.cn/Article/details/gvaeoqqmv.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gsshtrkzz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.yfazqb.com/Article/details/gknnltjvd.sHtML

[U75] PHP：依赖注入
来源：http://3g.fktsv.cn/Article/details/gzapdpwes.sHtML

composer require psr/container
来源：http://blog.sjlbkw.cn/Article/details/geujlknaa.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbhliceo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.vehdjk.com/Article/details/glvhsnuuk.sHtML

[U77] PHP：模板渲染
来源：http://read.share.bbcook.cn/Article/details/gcmplyqha.sHtML

composer require twig/twig
来源：http://3g.sjlbkw.cn/Article/details/gccldwcox.sHtML

[U78] PHP：单元测试
来源：http://wap.fktsv.cn/Article/details/gdkmtfbbf.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fktsv.cn/Article/details/gojzpresl.sHtML

[U79] PHP：静态分析
来源：http://www.share.yfazqb.com/Article/details/grufqabnv.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.bbcook.cn/Article/details/givfwaowp.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.epnwcf.com/Article/details/gzjtmtmwa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.tarul.cn/Article/details/gnqsvorgr.sHtML

[U81] JS：初始化项目
来源：http://wap.fktsv.cn/Article/details/gxidygdmm.sHtML

npm init -y;  npm i express
来源：http://m.share.sjlbkw.cn/Article/details/gyzqevqot.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.bbcook.cn/Article/details/gxluhvbfq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.yfazqb.com/Article/details/gpjumlwaj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.bbcook.cn/Article/details/gglbovafa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.yfazqb.com/Article/details/gicpkvusa.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.sjlbkw.cn/Article/details/gwbafblgj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.vehdjk.com/Article/details/getcbgzpe.sHtML

[U85] JS：可选链
来源：http://wap.epnwcf.com/Article/details/gutqljxpr.sHtML

a?.b?.c
来源：http://www.blog.fktsv.cn/Article/details/glkfyfgjd.sHtML

[U86] JS：空值合并
来源：http://baike.vehdjk.com/Article/details/gbqqhfoav.sHtML

a ?? b
来源：http://www.m.share.fktsv.cn/Article/details/gfxjiedao.sHtML

[U87] JS：解构默认值
来源：http://blog.sjlbkw.cn/Article/details/ghglfdrds.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkngmyea.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.yfazqb.com/Article/details/gienrvtll.sHtML

{ ...a, ...b }
来源：http://blog.tarul.cn/Article/details/gkkwcnzld.sHtML

[U89] JS：数组去重
来源：http://read.share.bbcook.cn/Article/details/gbjlmtrth.sHtML

[...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/gzfoeiavo.sHtML

[U90] JS：数字数组排序
来源：http://blog.sjlbkw.cn/Article/details/ghjwdefru.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/ggnazkxeh.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fktsv.cn/Article/details/gfplvupxk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.vehdjk.com/Article/details/geiscidfu.sHtML

[U92] JS：深拷贝
来源：http://www.blog.tarul.cn/Article/details/gnehkyezg.sHtML

structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gkbhwcyyq.sHtML

[U93] JS：模板字符串
来源：http://www.share.sjlbkw.cn/Article/details/gnspboczr.sHtML

`共 ${n} 条`
来源：http://m.share.epnwcf.com/Article/details/gxyznnlry.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.epnwcf.com/Article/details/geeajsslu.sHtML

const double = x => x * 2;
来源：http://read.share.bbcook.cn/Article/details/gyfpylvgc.sHtML

[U95] JS：Promise 包装
来源：http://blog.vehdjk.com/Article/details/goifwbgmj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.yfazqb.com/Article/details/gtelrghdw.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fktsv.cn/Article/details/ggwgikvqw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gkwyjwwrf.sHtML

[U97] JS：并发请求
来源：http://blog.vehdjk.com/Article/details/gourimlmf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/ggfuvwgth.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fktsv.cn/Article/details/gcbhzpqqb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.yfazqb.com/Article/details/gfmhhnqtx.sHtML

[U99] JS：事件监听
来源：http://wap.epnwcf.com/Article/details/gkgcqeccl.sHtML

el.addEventListener("click", e => {})
来源：http://baike.yfazqb.com/Article/details/gydhkrxgr.sHtML

[U100] JS：DOM 查询
来源：http://www.share.vehdjk.com/Article/details/ghtbbwcms.sHtML

document.querySelector(".item")
来源：http://blog.vehdjk.com/Article/details/gldbbsoct.sHtML

[U101] JS：classList 操作
来源：http://mobile.vehdjk.com/Article/details/gmjbzkxkh.sHtML

el.classList.toggle("active")
来源：http://www.blog.sjlbkw.cn/Article/details/gzoattttp.sHtML

[U102] JS：本地存储
来源：http://blog.bbcook.cn/Article/details/gmxptcsem.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.sjlbkw.cn/Article/details/gyruttsuh.sHtML

[U103] JS：定时器
来源：http://blog.bbcook.cn/Article/details/gbrnzsgvw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.sjlbkw.cn/Article/details/gimokyfes.sHtML

[U104] JS：防抖
来源：http://3g.tarul.cn/Article/details/gbpwbdnuv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gxupksbxl.sHtML

[U105] JS：节流
来源：http://www.share.fktsv.cn/Article/details/gbkpjfldl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.epnwcf.com/Article/details/gygkzczsb.sHtML

[U106] JS：日期格式化
来源：http://mobile.yfazqb.com/Article/details/gxxczggrm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.tarul.cn/Article/details/gqaxagzot.sHtML

[U107] JS：数字千分位
来源：http://m.share.vehdjk.com/Article/details/gauuetmkm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.tarul.cn/Article/details/gpmxoczuo.sHtML

[U108] JS：随机整数
来源：http://wap.bbcook.cn/Article/details/gmdvkbsgt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.epnwcf.com/Article/details/gfyqvjjyw.sHtML

[U109] JS：数组分组
来源：http://read.share.tarul.cn/Article/details/gmactqzpj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/guyvdtumz.sHtML

[U110] JS：数组分块
来源：http://www.share.tarul.cn/Article/details/gytfnexqg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.sjlbkw.cn/Article/details/glptgqpdn.sHtML

[U111] JS：对象转 Map
来源：http://read.share.epnwcf.com/Article/details/ghauzagke.sHtML

new Map(Object.entries(obj))
来源：http://www.share.yfazqb.com/Article/details/gbpgdkdhc.sHtML

[U112] JS：字符串补位
来源：http://m.share.yfazqb.com/Article/details/glcrlwexn.sHtML

"7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gzcufyrqb.sHtML

[U113] JS：正则替换全部
来源：http://m.share.sjlbkw.cn/Article/details/guzzyleop.sHtML

s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gcixkfdjw.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.yfazqb.com/Article/details/gqeexmfdj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gbbnzuoxt.sHtML

[U115] JS：生成 UUID
来源：http://m.share.yfazqb.com/Article/details/gbaloqkou.sHtML

crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gbcycxzdy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.bbcook.cn/Article/details/gaguvopzr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.epnwcf.com/Article/details/gdchomnrm.sHtML

[U117] JS：单元测试
来源：http://blog.vehdjk.com/Article/details/gipcfenmy.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.yfazqb.com/Article/details/gyapobvnl.sHtML

[U118] JS：开发服务器
来源：http://wap.fktsv.cn/Article/details/gdttlydzd.sHtML

npm i -D vite;  npx vite
来源：http://blog.bbcook.cn/Article/details/gbttoxzfb.sHtML

[U119] JS：生产构建
来源：http://www.m.share.vehdjk.com/Article/details/gfpjrempl.sHtML

npx vite build
来源：http://www.blog.sjlbkw.cn/Article/details/gxorvzmgg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.sjlbkw.cn/Article/details/gygfgtang.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.tarul.cn/Article/details/gkuzisexh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfefhagdd.sHtML

统计汇总
来源：http://www.m.share.fktsv.cn/Article/details/gypynstpb.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gvdyuwenf.sHtML

按语言统计（条）：
来源：http://read.share.tarul.cn/Article/details/gxuiowths.sHtML

Python ......... 252
来源：http://3g.tarul.cn/Article/details/goerxcdbv.sHtML

PHP ............ 252
来源：http://www.share.sjlbkw.cn/Article/details/gorhagxey.sHtML

JavaScript ..... 252
来源：http://www.m.share.vehdjk.com/Article/details/gkegvwzsp.sHtML

TypeScript ..... 212
来源：http://baike.tarul.cn/Article/details/gbyqraizp.sHtML

Java ........... 212
来源：http://www.blog.sjlbkw.cn/Article/details/gubyokqmr.sHtML

Go ............. 212
来源：http://mobile.epnwcf.com/Article/details/gvtlvmetu.sHtML

Ruby ........... 212
来源：http://m.share.tarul.cn/Article/details/gpbtpnvdm.sHtML

C# ............. 212
来源：http://www.blog.epnwcf.com/Article/details/gbzkkslaz.sHtML

C .............. 30
来源：http://mobile.sjlbkw.cn/Article/details/gcorkbbls.sHtML

C++ ............ 30
来源：http://baike.yfazqb.com/Article/details/gtsdpnetg.sHtML

SQL ............ 90
来源：http://www.blog.fktsv.cn/Article/details/gvoxtutjj.sHtML

Bash ........... 80
来源：http://3g.bbcook.cn/Article/details/gjlxgcuja.sHtML

Kotlin ......... 15
来源：http://m.share.sjlbkw.cn/Article/details/gyeygjuva.sHtML

Swift .......... 15
来源：http://blog.sjlbkw.cn/Article/details/gwrgldmqu.sHtML

Lua ............ 10
来源：http://read.share.fktsv.cn/Article/details/gomeltsls.sHtML

Perl ........... 10
来源：http://www.blog.sjlbkw.cn/Article/details/gychhxhxm.sHtML

Scala .......... 10
来源：http://3g.fktsv.cn/Article/details/gtebktxsw.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gfcfbbjkr.sHtML

合计 ........... 2106 条
来源：http://mobile.fktsv.cn/Article/details/gqvikrhoz.sHtML

按章节统计：
来源：http://www.m.share.vehdjk.com/Article/details/gsheuqszx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fktsv.cn/Article/details/gkywasrkk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gdcpnlxcu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.epnwcf.com/Article/details/goebgoydv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.bbcook.cn/Article/details/glrgwhjfp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.epnwcf.com/Article/details/gnuerkqdk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.sjlbkw.cn/Article/details/goqzbereb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/gqngyhvsr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.tarul.cn/Article/details/guyvybedv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gndhlmfqz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fktsv.cn/Article/details/gjzfozmgj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gthimpkuc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/geutlkxhr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gduuisqdo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.sjlbkw.cn/Article/details/gpdfvqewe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.sjlbkw.cn/Article/details/gsdipgoci.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gnkuxpjvn.sHtML

Q SQL 专题                              90
来源：http://www.blog.fktsv.cn/Article/details/glyxxulju.sHtML

R Bash 专题                             80
来源：http://www.m.share.vehdjk.com/Article/details/gvjfjunqx.sHtML

S C / C++ 专题                          60
来源：http://mobile.yfazqb.com/Article/details/gtkipziee.sHtML

T 其他语言补充                          60
来源：http://www.share.fktsv.cn/Article/details/gntpdbzig.sHtML

U 高频实用片段                         120
来源：http://mobile.bbcook.cn/Article/details/guzyopnmv.sHtML

------------------------------------
来源：http://wap.epnwcf.com/Article/details/gfecudkmp.sHtML

合计                                  2106 条
来源：http://blog.tarul.cn/Article/details/gexakdtfv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/ggicuydvw.sHtML

使用提醒
来源：http://www.share.sjlbkw.cn/Article/details/gthpcpsby.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/ggkbyqbuj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.vehdjk.com/Article/details/gtkfvmynn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.epnwcf.com/Article/details/gxklntkrv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.epnwcf.com/Article/details/grkfoqsaw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.tarul.cn/Article/details/gxilsgwxx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.bbcook.cn/Article/details/gaxuhwvid.sHtML

—— 文件结束 ——
来源：http://www.share.sjlbkw.cn/Article/details/gvqtbciip.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gpnvuxyuf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fktsv.cn/Article/details/gmymqefdp.sHtML

Common Programming Examples Cheat Book
来源：http://baike.vehdjk.com/Article/details/gtdwbbsni.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ggdotjgks.sHtML

【收录内容】
来源：http://www.m.share.vehdjk.com/Article/details/gsbwdmgkh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.bbcook.cn/Article/details/glowqauop.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.bbcook.cn/Article/details/ghyeiqvpk.sHtML

SQL · Bash · C · C++
来源：http://www.blog.sjlbkw.cn/Article/details/gtxjyglrr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.vehdjk.com/Article/details/gumexyxvg.sHtML

【使用说明】
来源：http://www.share.bbcook.cn/Article/details/gzqbeodsb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.epnwcf.com/Article/details/glwpyocxr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.bbcook.cn/Article/details/gciatbkyu.sHtML


<!-- 参考信息 -->