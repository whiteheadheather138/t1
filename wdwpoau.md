代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.share.fktsv.cn/Article/details/gtydehhuy.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gxmzqqiwc.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.yfazqb.com/Article/details/ghwgetfec.sHtML

{**a, **b}
来源：http://www.blog.epnwcf.com/Article/details/gvdwnykam.sHtML

[U07] Py：反转字典键值
来源：http://wap.vehdjk.com/Article/details/gquvkuqvk.sHtML

{v: k for k, v in d.items()}
来源：http://blog.bbcook.cn/Article/details/giwpqyfnn.sHtML

[U08] Py：展平二维列表
来源：http://www.share.epnwcf.com/Article/details/gclxhymve.sHtML

[y for x in nested for y in x]
来源：http://mobile.yfazqb.com/Article/details/gxbczogpz.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/gluierouq.sHtML

max(d, key=d.get)
来源：http://www.blog.fktsv.cn/Article/details/glbyqjbfq.sHtML

[U10] Py：按值排序字典
来源：http://m.share.bbcook.cn/Article/details/gdhjvybea.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.yfazqb.com/Article/details/gixbfqpuh.sHtML

[U11] Py：生成器表达式
来源：http://www.share.bbcook.cn/Article/details/gpzgajmuy.sHtML

(x * 2 for x in arr)
来源：http://3g.vehdjk.com/Article/details/gqngdqggf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.tarul.cn/Article/details/gjsajptiw.sHtML

Counter(arr).most_common(3)
来源：http://www.share.sjlbkw.cn/Article/details/ghnzassbj.sHtML

[U13] Py：固定长度队列
来源：http://wap.tarul.cn/Article/details/gpfdqyuea.sHtML

deque(maxlen=10)
来源：http://m.share.yfazqb.com/Article/details/gkwiongiz.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.yfazqb.com/Article/details/gybctahzk.sHtML

defaultdict(list)
来源：http://www.share.epnwcf.com/Article/details/grreshltu.sHtML

[U15] Py：高精度计时
来源：http://www.share.epnwcf.com/Article/details/gqdewhzlz.sHtML

t = time.perf_counter()
来源：http://mobile.bbcook.cn/Article/details/gkkybexoi.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fktsv.cn/Article/details/gsdqictce.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.vehdjk.com/Article/details/gwbexfkjm.sHtML

[U17] Py：初始化日志
来源：http://baike.epnwcf.com/Article/details/gubbtiwht.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.yfazqb.com/Article/details/gmlagjlya.sHtML

[U18] Py：预编译正则
来源：http://baike.epnwcf.com/Article/details/gzavdyztv.sHtML

pat = re.compile(r"\d+")
来源：http://3g.epnwcf.com/Article/details/gfelthgma.sHtML

[U19] Py：正则替换带回调
来源：http://3g.vehdjk.com/Article/details/gjtjvsbvq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.yfazqb.com/Article/details/giryiwgdl.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuouwziy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.tarul.cn/Article/details/gcdfujhmq.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.yfazqb.com/Article/details/giymzepqm.sHtML

@contextlib.contextmanager
来源：http://blog.tarul.cn/Article/details/ginktxqew.sHtML

[U22] Py：矩阵转置
来源：http://mobile.vehdjk.com/Article/details/ghqvqnile.sHtML

list(zip(*m))
来源：http://read.share.epnwcf.com/Article/details/gtrcrprzw.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.bbcook.cn/Article/details/gxtcascdr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.tarul.cn/Article/details/gibazxogy.sHtML

[U24] Py：路径操作
来源：http://www.blog.fktsv.cn/Article/details/gxsafobxf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gxotypdrf.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.epnwcf.com/Article/details/guwxchpfl.sHtML

csv.DictReader(f)
来源：http://read.share.sjlbkw.cn/Article/details/gvxfrxaby.sHtML

[U26] Py：并发下载
来源：http://mobile.vehdjk.com/Article/details/gjdbxxqxk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.epnwcf.com/Article/details/ghftfwgkc.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.bbcook.cn/Article/details/gqtezhgkg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.yfazqb.com/Article/details/ggkkbbpjv.sHtML

[U28] Py：类型别名
来源：http://wap.epnwcf.com/Article/details/grivaviom.sHtML

UserId = int
来源：http://baike.bbcook.cn/Article/details/glbxnkwqi.sHtML

[U29] Py：属性校验
来源：http://www.share.tarul.cn/Article/details/gznodvxls.sHtML

@property 与 @x.setter 配合
来源：http://wap.fktsv.cn/Article/details/gioslgehm.sHtML

[U30] Py：数据类
来源：http://www.m.share.bbcook.cn/Article/details/gsqtjkccp.sHtML

@dataclass(slots=True)
来源：http://m.share.fktsv.cn/Article/details/grukhvmub.sHtML

[U31] Py：单测
来源：http://wap.vehdjk.com/Article/details/glfowcwea.sHtML

python -m pytest -q
来源：http://www.blog.tarul.cn/Article/details/ghwavwbdv.sHtML

[U32] Py：代码格式化
来源：http://read.share.sjlbkw.cn/Article/details/gxvnwuodk.sHtML

ruff format . && ruff check --fix .
来源：http://3g.epnwcf.com/Article/details/gfzhxuefu.sHtML

[U33] Py：打包发布
来源：http://www.blog.sjlbkw.cn/Article/details/gpnembqjt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.vehdjk.com/Article/details/gclbyfohe.sHtML

[U34] Py：判断编码
来源：http://www.share.bbcook.cn/Article/details/gyikvklze.sHtML

chardet.detect(raw)
来源：http://www.share.yfazqb.com/Article/details/ghsouzqie.sHtML

[U35] Py：发送邮件
来源：http://m.share.vehdjk.com/Article/details/gezesybzc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.sjlbkw.cn/Article/details/gdcsgdihy.sHtML

[U36] Py：定时任务
来源：http://mobile.sjlbkw.cn/Article/details/glwhizzer.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.vehdjk.com/Article/details/grirntfmd.sHtML

[U37] Py：读写 Excel
来源：http://read.share.sjlbkw.cn/Article/details/gjoxsngbs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.bbcook.cn/Article/details/gddyseigu.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.bbcook.cn/Article/details/goaidspsh.sHtML

Path(__file__).resolve().parent
来源：http://wap.vehdjk.com/Article/details/gswgysnug.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.tarul.cn/Article/details/ghfbxttsr.sHtML

sys.stdout.isatty()
来源：http://baike.tarul.cn/Article/details/gnaoeiwfz.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.vehdjk.com/Article/details/gsshapfoz.sHtML

print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/gdqlrgkri.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.vehdjk.com/Article/details/gdhthbgxb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fktsv.cn/Article/details/gvipzvssk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.sjlbkw.cn/Article/details/gwsvzjxhn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.sjlbkw.cn/Article/details/gkbsdhwgj.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.epnwcf.com/Article/details/gzxhurivk.sHtML

namespace App\Http;
来源：http://read.share.vehdjk.com/Article/details/gofysfghe.sHtML

[U44] PHP：开启严格类型
来源：http://baike.bbcook.cn/Article/details/gmuzxoqav.sHtML

declare(strict_types=1);
来源：http://www.blog.epnwcf.com/Article/details/gezjozytl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.bbcook.cn/Article/details/gfauzbnvd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gcvwqzmuz.sHtML

[U46] PHP：可空类型
来源：http://www.blog.sjlbkw.cn/Article/details/ggrjrhtlq.sHtML

?string $name = null
来源：http://mobile.sjlbkw.cn/Article/details/gjfhndlrc.sHtML

[U47] PHP：联合类型
来源：http://baike.tarul.cn/Article/details/gyqphxyls.sHtML

int|string $id
来源：http://www.share.sjlbkw.cn/Article/details/gziedbdji.sHtML

[U48] PHP：纯枚举
来源：http://blog.yfazqb.com/Article/details/gbahkwljk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.vehdjk.com/Article/details/gszxvfhzp.sHtML

[U49] PHP：只读属性
来源：http://www.blog.yfazqb.com/Article/details/gudqxfxit.sHtML

public readonly string $name
来源：http://3g.epnwcf.com/Article/details/gsjmpsnhf.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.tarul.cn/Article/details/gekpnguke.sHtML

public function __construct(private int $id) {}
来源：http://baike.sjlbkw.cn/Article/details/grofypjea.sHtML

[U51] PHP：数组解构
来源：http://blog.yfazqb.com/Article/details/gjfillmtm.sHtML

[$a, $b] = $arr;
来源：http://www.share.sjlbkw.cn/Article/details/gsdootxco.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.epnwcf.com/Article/details/gtuiwdkvv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.bbcook.cn/Article/details/gwimyssyb.sHtML

[U53] PHP：空合并运算符
来源：http://baike.epnwcf.com/Article/details/guqgvalqn.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fktsv.cn/Article/details/gipsjlndp.sHtML

[U54] PHP：空安全调用
来源：http://blog.yfazqb.com/Article/details/gwvdgsvjk.sHtML

$obj?->method()
来源：http://www.blog.sjlbkw.cn/Article/details/grnstmirc.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fktsv.cn/Article/details/grtulbgqr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.epnwcf.com/Article/details/gclwxhaip.sHtML

[U56] PHP：命名参数
来源：http://mobile.fktsv.cn/Article/details/gazpmjztw.sHtML

f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gdpgdrglt.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gxlzpetkl.sHtML

"值: {$a}"
来源：http://read.share.bbcook.cn/Article/details/gpkbqpatb.sHtML

[U58] PHP：数组三件套
来源：http://read.share.epnwcf.com/Article/details/glqyrbcck.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fktsv.cn/Article/details/gmvrcuosn.sHtML

[U59] PHP：自定义排序
来源：http://wap.epnwcf.com/Article/details/glqzctzhy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gdsqmkkxp.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtcgfgis.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.sjlbkw.cn/Article/details/glifmnmti.sHtML

[U61] PHP：正则
来源：http://www.m.share.vehdjk.com/Article/details/gmifulecb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.vehdjk.com/Article/details/gogwszbkk.sHtML

[U62] PHP：日期对象
来源：http://m.share.fktsv.cn/Article/details/gvzesyxvd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.vehdjk.com/Article/details/gqvtiwrvo.sHtML

[U63] PHP：文件读写
来源：http://mobile.vehdjk.com/Article/details/gvuobzvlc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.epnwcf.com/Article/details/ggbmwisuj.sHtML

[U64] PHP：目录遍历
来源：http://read.share.sjlbkw.cn/Article/details/groijbrbz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.tarul.cn/Article/details/glbygftrz.sHtML

[U65] PHP：会话
来源：http://wap.bbcook.cn/Article/details/gubgjzzig.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gbmsfyuon.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fktsv.cn/Article/details/gmndgaoth.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.yfazqb.com/Article/details/garuuofet.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.yfazqb.com/Article/details/gmldngqpd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.epnwcf.com/Article/details/gqefjnech.sHtML

[U68] PHP：PDO 连接
来源：http://baike.bbcook.cn/Article/details/grzfxvxmc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.epnwcf.com/Article/details/ghjmpfqkq.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.tarul.cn/Article/details/gyhwtkvrh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.epnwcf.com/Article/details/gdcugeiac.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.sjlbkw.cn/Article/details/gixqxzysf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fktsv.cn/Article/details/gebpiwnva.sHtML

[U71] PHP：抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gzpbusfra.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/gpsnalakw.sHtML

[U72] PHP：写错误日志
来源：http://wap.tarul.cn/Article/details/gtfhyoxjn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.tarul.cn/Article/details/gcpsdqbex.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.sjlbkw.cn/Article/details/glcmuynii.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.yfazqb.com/Article/details/gllpvfzbr.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gdwelyadc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.tarul.cn/Article/details/gyatlivfk.sHtML

[U75] PHP：依赖注入
来源：http://m.share.bbcook.cn/Article/details/ggedvzvdb.sHtML

composer require psr/container
来源：http://www.share.sjlbkw.cn/Article/details/ggodlqklh.sHtML

[U76] PHP：简单路由
来源：http://www.blog.epnwcf.com/Article/details/ggtcmbved.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fktsv.cn/Article/details/grgysfdth.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fktsv.cn/Article/details/gouvubmpk.sHtML

composer require twig/twig
来源：http://www.m.share.tarul.cn/Article/details/gvidlhyym.sHtML

[U78] PHP：单元测试
来源：http://3g.sjlbkw.cn/Article/details/ghwiououk.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.tarul.cn/Article/details/gwhskonnv.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.tarul.cn/Article/details/gtbdqefvz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.yfazqb.com/Article/details/gvwmnszoq.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.epnwcf.com/Article/details/gqqivtjlp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.yfazqb.com/Article/details/gklypsdnk.sHtML

[U81] JS：初始化项目
来源：http://m.share.vehdjk.com/Article/details/geozigsyj.sHtML

npm init -y;  npm i express
来源：http://wap.tarul.cn/Article/details/gwfhwsjhp.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fktsv.cn/Article/details/geursqedv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.epnwcf.com/Article/details/glvwagose.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.vehdjk.com/Article/details/gfvdcozsu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.epnwcf.com/Article/details/gczydlqmv.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.tarul.cn/Article/details/gtrhqkmfb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.vehdjk.com/Article/details/gekhyvney.sHtML

[U85] JS：可选链
来源：http://blog.fktsv.cn/Article/details/gbxxjpgek.sHtML

a?.b?.c
来源：http://read.share.vehdjk.com/Article/details/gyotqicve.sHtML

[U86] JS：空值合并
来源：http://3g.sjlbkw.cn/Article/details/gqvlljkxz.sHtML

a ?? b
来源：http://read.share.bbcook.cn/Article/details/gxdnmtuxc.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fktsv.cn/Article/details/gwjlhygrx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fktsv.cn/Article/details/gycnqtyvi.sHtML

[U88] JS：对象展开合并
来源：http://mobile.tarul.cn/Article/details/gbkikhkhq.sHtML

{ ...a, ...b }
来源：http://m.share.bbcook.cn/Article/details/gkdpnycyu.sHtML

[U89] JS：数组去重
来源：http://baike.bbcook.cn/Article/details/gpgkrzqgb.sHtML

[...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/gnhbdgaxs.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.vehdjk.com/Article/details/gpvcxfcls.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gnvervgzc.sHtML

[U91] JS：对象键值遍历
来源：http://wap.bbcook.cn/Article/details/gnkeguazo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.sjlbkw.cn/Article/details/gsjvwmjej.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fktsv.cn/Article/details/gwyoofvju.sHtML

structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gteklgxdm.sHtML

[U93] JS：模板字符串
来源：http://www.share.yfazqb.com/Article/details/gatdrhsmk.sHtML

`共 ${n} 条`
来源：http://www.m.share.fktsv.cn/Article/details/gtjuzefeb.sHtML

[U94] JS：箭头函数
来源：http://m.share.vehdjk.com/Article/details/gwmupqjno.sHtML

const double = x => x * 2;
来源：http://read.share.fktsv.cn/Article/details/gqkzhqvpt.sHtML

[U95] JS：Promise 包装
来源：http://baike.yfazqb.com/Article/details/gjgvjjgli.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.sjlbkw.cn/Article/details/gwhuzkias.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.tarul.cn/Article/details/gdnplgatl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gxyqxmyie.sHtML

[U97] JS：并发请求
来源：http://baike.fktsv.cn/Article/details/gflhxqnum.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gsrfylnje.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.bbcook.cn/Article/details/gpozlpugn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.yfazqb.com/Article/details/ggxbakpej.sHtML

[U99] JS：事件监听
来源：http://blog.tarul.cn/Article/details/gjnykiflb.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.vehdjk.com/Article/details/goctihsen.sHtML

[U100] JS：DOM 查询
来源：http://3g.tarul.cn/Article/details/gjxvpyfba.sHtML

document.querySelector(".item")
来源：http://www.m.share.vehdjk.com/Article/details/gadzbbdyb.sHtML

[U101] JS：classList 操作
来源：http://blog.fktsv.cn/Article/details/gqiabbgpw.sHtML

el.classList.toggle("active")
来源：http://www.share.fktsv.cn/Article/details/gmpdsoujm.sHtML

[U102] JS：本地存储
来源：http://www.blog.yfazqb.com/Article/details/gbzlezabf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.sjlbkw.cn/Article/details/ghrxccmik.sHtML

[U103] JS：定时器
来源：http://baike.epnwcf.com/Article/details/gtdwzjjld.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.tarul.cn/Article/details/ggvqxyxyj.sHtML

[U104] JS：防抖
来源：http://baike.vehdjk.com/Article/details/gvvxbbyyt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gjmkdjhui.sHtML

[U105] JS：节流
来源：http://mobile.yfazqb.com/Article/details/govuitkki.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fktsv.cn/Article/details/gktxcjcws.sHtML

[U106] JS：日期格式化
来源：http://baike.yfazqb.com/Article/details/golfxcdqd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.sjlbkw.cn/Article/details/gghgzcgwv.sHtML

[U107] JS：数字千分位
来源：http://m.share.fktsv.cn/Article/details/ghgthdeeq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.yfazqb.com/Article/details/gdsthbozr.sHtML

[U108] JS：随机整数
来源：http://wap.fktsv.cn/Article/details/givgkeosi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.vehdjk.com/Article/details/gnbjyrxhx.sHtML

[U109] JS：数组分组
来源：http://www.blog.bbcook.cn/Article/details/gqtcthhuw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.yfazqb.com/Article/details/gcvyqqbei.sHtML

[U110] JS：数组分块
来源：http://blog.tarul.cn/Article/details/gbecxqome.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.bbcook.cn/Article/details/gftxdzcrx.sHtML

[U111] JS：对象转 Map
来源：http://3g.tarul.cn/Article/details/gunpdsuer.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fktsv.cn/Article/details/gtphignvf.sHtML

[U112] JS：字符串补位
来源：http://baike.epnwcf.com/Article/details/gdftdclcw.sHtML

"7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/grnqrucyh.sHtML

[U113] JS：正则替换全部
来源：http://www.share.epnwcf.com/Article/details/gcmslncdp.sHtML

s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gndwlbqhi.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.bbcook.cn/Article/details/guoeonivh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.bbcook.cn/Article/details/gtyrukrte.sHtML

[U115] JS：生成 UUID
来源：http://wap.vehdjk.com/Article/details/gpkrcgpuh.sHtML

crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gjzlobcho.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.epnwcf.com/Article/details/gdwezuzja.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.epnwcf.com/Article/details/gxwzqnaet.sHtML

[U117] JS：单元测试
来源：http://mobile.epnwcf.com/Article/details/gmvqionmn.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.sjlbkw.cn/Article/details/gwvmuacfb.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fktsv.cn/Article/details/grrmigdfm.sHtML

npm i -D vite;  npx vite
来源：http://baike.fktsv.cn/Article/details/ggohukhjh.sHtML

[U119] JS：生产构建
来源：http://blog.yfazqb.com/Article/details/gzimzeaqo.sHtML

npx vite build
来源：http://3g.sjlbkw.cn/Article/details/ghdgbqrtg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.yfazqb.com/Article/details/geqytgfbi.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.vehdjk.com/Article/details/gufkxglhu.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvdrrmrvy.sHtML

统计汇总
来源：http://baike.fktsv.cn/Article/details/gxmtrcpko.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/getpdummx.sHtML

按语言统计（条）：
来源：http://m.share.epnwcf.com/Article/details/gapuzkomh.sHtML

Python ......... 252
来源：http://3g.tarul.cn/Article/details/gwtwtzkpz.sHtML

PHP ............ 252
来源：http://mobile.bbcook.cn/Article/details/gxmnjwmvj.sHtML

JavaScript ..... 252
来源：http://wap.vehdjk.com/Article/details/gxhgptzlb.sHtML

TypeScript ..... 212
来源：http://m.share.tarul.cn/Article/details/gfietwdkl.sHtML

Java ........... 212
来源：http://wap.sjlbkw.cn/Article/details/glihxoijg.sHtML

Go ............. 212
来源：http://mobile.bbcook.cn/Article/details/gvijasjhv.sHtML

Ruby ........... 212
来源：http://read.share.yfazqb.com/Article/details/gavtvwwki.sHtML

C# ............. 212
来源：http://www.blog.tarul.cn/Article/details/gdwbhocec.sHtML

C .............. 30
来源：http://m.share.tarul.cn/Article/details/gdwkfsrkr.sHtML

C++ ............ 30
来源：http://mobile.yfazqb.com/Article/details/gzvauxeqr.sHtML

SQL ............ 90
来源：http://blog.vehdjk.com/Article/details/gfiukmmnc.sHtML

Bash ........... 80
来源：http://m.share.yfazqb.com/Article/details/gcizcjfdb.sHtML

Kotlin ......... 15
来源：http://baike.bbcook.cn/Article/details/gfmdnzrou.sHtML

Swift .......... 15
来源：http://www.share.epnwcf.com/Article/details/gfdukkdjj.sHtML

Lua ............ 10
来源：http://www.share.vehdjk.com/Article/details/gpywxfhju.sHtML

Perl ........... 10
来源：http://www.blog.vehdjk.com/Article/details/gsfjnrqgg.sHtML

Scala .......... 10
来源：http://read.share.bbcook.cn/Article/details/guehjfbcq.sHtML

------------------------------------
来源：http://wap.fktsv.cn/Article/details/gbrrawptq.sHtML

合计 ........... 2106 条
来源：http://blog.fktsv.cn/Article/details/gchzkliil.sHtML

按章节统计：
来源：http://mobile.epnwcf.com/Article/details/gyadrbxqi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.tarul.cn/Article/details/gyjpdvayu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/gwizfjlyw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gmgfigfcq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.sjlbkw.cn/Article/details/gqqhhtlnp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.epnwcf.com/Article/details/gmvhgiumz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.epnwcf.com/Article/details/ggprgvhln.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/guaxjyjmy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.yfazqb.com/Article/details/gpberhloa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gqorxkdig.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.tarul.cn/Article/details/gpabxrxpy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gfdsukkrr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gumhtpstd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/glqpjofke.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.tarul.cn/Article/details/gfbhxizmd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.vehdjk.com/Article/details/gyuveyvcw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/graphywpq.sHtML

Q SQL 专题                              90
来源：http://blog.yfazqb.com/Article/details/gytemeenx.sHtML

R Bash 专题                             80
来源：http://blog.epnwcf.com/Article/details/gldvdqadg.sHtML

S C / C++ 专题                          60
来源：http://read.share.fktsv.cn/Article/details/glvkdezfc.sHtML

T 其他语言补充                          60
来源：http://blog.yfazqb.com/Article/details/gmpwhsrtx.sHtML

U 高频实用片段                         120
来源：http://www.blog.tarul.cn/Article/details/ghfmfytcm.sHtML

------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gdobccfba.sHtML

合计                                  2106 条
来源：http://blog.epnwcf.com/Article/details/gbfidlgit.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gqdgnrtpv.sHtML

使用提醒
来源：http://www.blog.yfazqb.com/Article/details/gxkykewka.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gyftqxpbf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fktsv.cn/Article/details/gmzsvndqx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.epnwcf.com/Article/details/gqzjtszvk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.sjlbkw.cn/Article/details/grkueorcy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.sjlbkw.cn/Article/details/gfswxeaui.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.vehdjk.com/Article/details/gesxuacao.sHtML

—— 文件结束 ——
来源：http://wap.yfazqb.com/Article/details/guopcizzu.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gipnsidqm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.tarul.cn/Article/details/gavrhcjzw.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.bbcook.cn/Article/details/gaovhtogs.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gyflrtvdq.sHtML

【收录内容】
来源：http://3g.sjlbkw.cn/Article/details/gldtzwcjz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.sjlbkw.cn/Article/details/gowulfreo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.yfazqb.com/Article/details/gyezmjwrs.sHtML

SQL · Bash · C · C++
来源：http://www.share.tarul.cn/Article/details/guwwqrvql.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.vehdjk.com/Article/details/gaysajivb.sHtML

【使用说明】
来源：http://blog.tarul.cn/Article/details/gumbbasws.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.tarul.cn/Article/details/godrqpzph.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.sjlbkw.cn/Article/details/geylbcnbm.sHtML


<!-- 参考信息 -->