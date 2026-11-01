代发 wailian999

[U05] Py：列表去重且保序
来源：http://read.share.fktsv.cn/Article/details/gypztdvye.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/giqnpngoj.sHtML

[U06] Py：合并两个字典
来源：http://3g.epnwcf.com/Article/details/gbrqdbjer.sHtML

{**a, **b}
来源：http://www.share.sjlbkw.cn/Article/details/gbmwaqhfc.sHtML

[U07] Py：反转字典键值
来源：http://baike.bbcook.cn/Article/details/gosqglgvi.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/gprorthvy.sHtML

[U08] Py：展平二维列表
来源：http://baike.tarul.cn/Article/details/gtucbtsmu.sHtML

[y for x in nested for y in x]
来源：http://wap.bbcook.cn/Article/details/golropomv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.sjlbkw.cn/Article/details/godbkdgxj.sHtML

max(d, key=d.get)
来源：http://www.blog.yfazqb.com/Article/details/ggpvzxenj.sHtML

[U10] Py：按值排序字典
来源：http://www.share.epnwcf.com/Article/details/glazalcar.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.vehdjk.com/Article/details/gtihakagx.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.tarul.cn/Article/details/gyclozysv.sHtML

(x * 2 for x in arr)
来源：http://m.share.sjlbkw.cn/Article/details/gwuzpetou.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.bbcook.cn/Article/details/gbcckaqio.sHtML

Counter(arr).most_common(3)
来源：http://read.share.yfazqb.com/Article/details/gvtqvbavn.sHtML

[U13] Py：固定长度队列
来源：http://blog.fktsv.cn/Article/details/ggqhdftbd.sHtML

deque(maxlen=10)
来源：http://3g.epnwcf.com/Article/details/gokygcjja.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.sjlbkw.cn/Article/details/gmcjwyoyn.sHtML

defaultdict(list)
来源：http://m.share.sjlbkw.cn/Article/details/ghieetrcx.sHtML

[U15] Py：高精度计时
来源：http://wap.sjlbkw.cn/Article/details/gcrnwpork.sHtML

t = time.perf_counter()
来源：http://read.share.fktsv.cn/Article/details/gtkwplsau.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.yfazqb.com/Article/details/gjrdiqakd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.vehdjk.com/Article/details/gvquzwxmt.sHtML

[U17] Py：初始化日志
来源：http://wap.vehdjk.com/Article/details/guqxhuffl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.sjlbkw.cn/Article/details/gkpdsfoye.sHtML

[U18] Py：预编译正则
来源：http://baike.tarul.cn/Article/details/ghilonzgb.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.epnwcf.com/Article/details/gseusefrw.sHtML

[U19] Py：正则替换带回调
来源：http://blog.yfazqb.com/Article/details/gskqjtuxq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.vehdjk.com/Article/details/glzfflopp.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fktsv.cn/Article/details/gccdqhdrc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.tarul.cn/Article/details/gbtuoxegq.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fktsv.cn/Article/details/gxcwpkany.sHtML

@contextlib.contextmanager
来源：http://m.share.yfazqb.com/Article/details/gzenfmref.sHtML

[U22] Py：矩阵转置
来源：http://wap.epnwcf.com/Article/details/gtcvjydlv.sHtML

list(zip(*m))
来源：http://read.share.sjlbkw.cn/Article/details/gkguhpolz.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.sjlbkw.cn/Article/details/goktwuops.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.epnwcf.com/Article/details/gktayjglm.sHtML

[U24] Py：路径操作
来源：http://3g.vehdjk.com/Article/details/gvaffvofx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/ghvcbnpyw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.tarul.cn/Article/details/gnvryuqbo.sHtML

csv.DictReader(f)
来源：http://www.m.share.bbcook.cn/Article/details/gjoqmxhql.sHtML

[U26] Py：并发下载
来源：http://baike.vehdjk.com/Article/details/gxtlxzaor.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.bbcook.cn/Article/details/gzzdfllod.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.vehdjk.com/Article/details/gbnmtusji.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fktsv.cn/Article/details/grlnuqupn.sHtML

[U28] Py：类型别名
来源：http://read.share.epnwcf.com/Article/details/gwakjyyzu.sHtML

UserId = int
来源：http://mobile.fktsv.cn/Article/details/gwlmjvtgy.sHtML

[U29] Py：属性校验
来源：http://www.m.share.bbcook.cn/Article/details/ghcaaucfi.sHtML

@property 与 @x.setter 配合
来源：http://read.share.sjlbkw.cn/Article/details/gubhyzjbl.sHtML

[U30] Py：数据类
来源：http://mobile.sjlbkw.cn/Article/details/gcpuzywws.sHtML

@dataclass(slots=True)
来源：http://baike.yfazqb.com/Article/details/gumcjdvub.sHtML

[U31] Py：单测
来源：http://blog.epnwcf.com/Article/details/gqooystmh.sHtML

python -m pytest -q
来源：http://www.blog.yfazqb.com/Article/details/ghstirajw.sHtML

[U32] Py：代码格式化
来源：http://wap.bbcook.cn/Article/details/gjiwdxllo.sHtML

ruff format . && ruff check --fix .
来源：http://baike.epnwcf.com/Article/details/ggzykpoae.sHtML

[U33] Py：打包发布
来源：http://read.share.sjlbkw.cn/Article/details/gpczzuhgi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.yfazqb.com/Article/details/gaidszczy.sHtML

[U34] Py：判断编码
来源：http://wap.epnwcf.com/Article/details/gwnehlnlb.sHtML

chardet.detect(raw)
来源：http://blog.yfazqb.com/Article/details/gbanewlve.sHtML

[U35] Py：发送邮件
来源：http://3g.tarul.cn/Article/details/gblfmjjiz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fktsv.cn/Article/details/gwizxgmqh.sHtML

[U36] Py：定时任务
来源：http://mobile.sjlbkw.cn/Article/details/ggbeyovun.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.yfazqb.com/Article/details/gwhnhaxpk.sHtML

[U37] Py：读写 Excel
来源：http://wap.sjlbkw.cn/Article/details/gumrtuzed.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.yfazqb.com/Article/details/gumajxdjd.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.tarul.cn/Article/details/gmhjpnfnc.sHtML

Path(__file__).resolve().parent
来源：http://read.share.yfazqb.com/Article/details/ggzmktumq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fktsv.cn/Article/details/gjklewwhp.sHtML

sys.stdout.isatty()
来源：http://wap.bbcook.cn/Article/details/gzcbgcttp.sHtML

[U40] Py：打印到标准错误
来源：http://wap.tarul.cn/Article/details/gaeisqses.sHtML

print("err", file=sys.stderr)
来源：http://m.share.sjlbkw.cn/Article/details/guifoujmg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.sjlbkw.cn/Article/details/gugykyzuo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.vehdjk.com/Article/details/gnqzkgawn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.vehdjk.com/Article/details/gjwtytomw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fktsv.cn/Article/details/gwrqxcsgd.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.bbcook.cn/Article/details/goxrxehkv.sHtML

namespace App\Http;
来源：http://www.blog.tarul.cn/Article/details/gfxiaihef.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.epnwcf.com/Article/details/glptyklxd.sHtML

declare(strict_types=1);
来源：http://blog.tarul.cn/Article/details/gwwsxdgfb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.vehdjk.com/Article/details/gzjnzmbsb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gvhqyhkac.sHtML

[U46] PHP：可空类型
来源：http://read.share.tarul.cn/Article/details/gmmkgrbzz.sHtML

?string $name = null
来源：http://blog.epnwcf.com/Article/details/gbvpiztsn.sHtML

[U47] PHP：联合类型
来源：http://wap.epnwcf.com/Article/details/gxwnwjdfz.sHtML

int|string $id
来源：http://baike.epnwcf.com/Article/details/geihrsfob.sHtML

[U48] PHP：纯枚举
来源：http://read.share.bbcook.cn/Article/details/gszwslxdh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.epnwcf.com/Article/details/grgkxgxky.sHtML

[U49] PHP：只读属性
来源：http://blog.yfazqb.com/Article/details/govzcfwyd.sHtML

public readonly string $name
来源：http://www.blog.bbcook.cn/Article/details/gnsaqyzvg.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.sjlbkw.cn/Article/details/gdynbhgvl.sHtML

public function __construct(private int $id) {}
来源：http://wap.fktsv.cn/Article/details/gkebcesnc.sHtML

[U51] PHP：数组解构
来源：http://m.share.epnwcf.com/Article/details/giyrojzhw.sHtML

[$a, $b] = $arr;
来源：http://blog.vehdjk.com/Article/details/giatryhxp.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.vehdjk.com/Article/details/gjgfurxtd.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.vehdjk.com/Article/details/gawduydxg.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.sjlbkw.cn/Article/details/ghcuyflfl.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.vehdjk.com/Article/details/gtpbbdiyu.sHtML

[U54] PHP：空安全调用
来源：http://baike.epnwcf.com/Article/details/gbgajguxa.sHtML

$obj?->method()
来源：http://baike.yfazqb.com/Article/details/guuiscpom.sHtML

[U55] PHP：match 表达式
来源：http://blog.tarul.cn/Article/details/gjptopapx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/gqdjxozih.sHtML

[U56] PHP：命名参数
来源：http://read.share.epnwcf.com/Article/details/gnpncnswy.sHtML

f(a: 1, b: 2)
来源：http://3g.epnwcf.com/Article/details/gxokpcrfu.sHtML

[U57] PHP：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gttayeeys.sHtML

"值: {$a}"
来源：http://read.share.yfazqb.com/Article/details/gzkkmwowc.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fktsv.cn/Article/details/gjgatzxef.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.yfazqb.com/Article/details/gmnhfsbjq.sHtML

[U59] PHP：自定义排序
来源：http://wap.tarul.cn/Article/details/ggmpuctub.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gpocpjpxp.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fktsv.cn/Article/details/gnmgicdhn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.bbcook.cn/Article/details/gndfrqnxg.sHtML

[U61] PHP：正则
来源：http://www.blog.fktsv.cn/Article/details/gyphhgxji.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.bbcook.cn/Article/details/gzlokdwtq.sHtML

[U62] PHP：日期对象
来源：http://read.share.sjlbkw.cn/Article/details/gqdjbirmq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.tarul.cn/Article/details/gqesfauje.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.vehdjk.com/Article/details/gyrroxojn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.sjlbkw.cn/Article/details/gtudbtadz.sHtML

[U64] PHP：目录遍历
来源：http://3g.vehdjk.com/Article/details/gwabsljao.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.vehdjk.com/Article/details/gibvenufb.sHtML

[U65] PHP：会话
来源：http://www.m.share.epnwcf.com/Article/details/gogdbpzvn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gegamuftu.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.epnwcf.com/Article/details/gyqugycgz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.epnwcf.com/Article/details/gkvklblbm.sHtML

[U67] PHP：处理文件上传
来源：http://blog.bbcook.cn/Article/details/gsejnokvp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fktsv.cn/Article/details/gtuoqnnzj.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fktsv.cn/Article/details/gbfargbky.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.yfazqb.com/Article/details/gjlcvbxhs.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.epnwcf.com/Article/details/gyzejltpt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fktsv.cn/Article/details/gfcgbklid.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.yfazqb.com/Article/details/gunarssoh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.epnwcf.com/Article/details/gopgravrk.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fktsv.cn/Article/details/gpqqfwrtm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fktsv.cn/Article/details/gvaawdjbo.sHtML

[U72] PHP：写错误日志
来源：http://m.share.yfazqb.com/Article/details/gwgwpwgqt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.tarul.cn/Article/details/gfllpfmjd.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.yfazqb.com/Article/details/gstmkxdwe.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.sjlbkw.cn/Article/details/girzshdsp.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fktsv.cn/Article/details/gqfmkkpxa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.yfazqb.com/Article/details/gvlffurud.sHtML

[U75] PHP：依赖注入
来源：http://mobile.yfazqb.com/Article/details/guzkhjbgj.sHtML

composer require psr/container
来源：http://mobile.fktsv.cn/Article/details/giivezrat.sHtML

[U76] PHP：简单路由
来源：http://blog.tarul.cn/Article/details/gmlzcbjaw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.tarul.cn/Article/details/gubwdagto.sHtML

[U77] PHP：模板渲染
来源：http://read.share.epnwcf.com/Article/details/ghorlxqty.sHtML

composer require twig/twig
来源：http://www.blog.epnwcf.com/Article/details/gfvhcdgwo.sHtML

[U78] PHP：单元测试
来源：http://baike.vehdjk.com/Article/details/gqrtkkicy.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.yfazqb.com/Article/details/gedvztvaf.sHtML

[U79] PHP：静态分析
来源：http://read.share.bbcook.cn/Article/details/ghddvewem.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.yfazqb.com/Article/details/gwhnfzkuh.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.yfazqb.com/Article/details/gdebwvjwn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fktsv.cn/Article/details/gihbhurzi.sHtML

[U81] JS：初始化项目
来源：http://baike.sjlbkw.cn/Article/details/gwinuhifl.sHtML

npm init -y;  npm i express
来源：http://www.m.share.yfazqb.com/Article/details/ghykagcrl.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.epnwcf.com/Article/details/gcxswmmvf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.sjlbkw.cn/Article/details/gpdfuvfvf.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.vehdjk.com/Article/details/gknjskgnq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/grhyslkvw.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.bbcook.cn/Article/details/gosczgvtg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.tarul.cn/Article/details/gpwrvwtcc.sHtML

[U85] JS：可选链
来源：http://www.m.share.tarul.cn/Article/details/gmwmcwalq.sHtML

a?.b?.c
来源：http://baike.vehdjk.com/Article/details/gaxmwfbhk.sHtML

[U86] JS：空值合并
来源：http://baike.bbcook.cn/Article/details/gilpprgoc.sHtML

a ?? b
来源：http://www.blog.yfazqb.com/Article/details/gsmrkwdjq.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.epnwcf.com/Article/details/gbhmuznyc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.yfazqb.com/Article/details/gmeamsenl.sHtML

[U88] JS：对象展开合并
来源：http://read.share.sjlbkw.cn/Article/details/gibtkulwm.sHtML

{ ...a, ...b }
来源：http://www.blog.bbcook.cn/Article/details/gbwmreoar.sHtML

[U89] JS：数组去重
来源：http://blog.vehdjk.com/Article/details/ghnrrbclr.sHtML

[...new Set(arr)]
来源：http://3g.yfazqb.com/Article/details/gmqgpsqet.sHtML

[U90] JS：数字数组排序
来源：http://baike.bbcook.cn/Article/details/gtvosmatv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/glhobrbcv.sHtML

[U91] JS：对象键值遍历
来源：http://wap.vehdjk.com/Article/details/grjkblwia.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.epnwcf.com/Article/details/gflndcsua.sHtML

[U92] JS：深拷贝
来源：http://read.share.tarul.cn/Article/details/gxsnhokry.sHtML

structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gacymjpmz.sHtML

[U93] JS：模板字符串
来源：http://wap.sjlbkw.cn/Article/details/gekwzgpwv.sHtML

`共 ${n} 条`
来源：http://www.m.share.tarul.cn/Article/details/gjkhfiirr.sHtML

[U94] JS：箭头函数
来源：http://3g.tarul.cn/Article/details/gwaqltazv.sHtML

const double = x => x * 2;
来源：http://m.share.vehdjk.com/Article/details/glpphsjvp.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fktsv.cn/Article/details/geyinytez.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.bbcook.cn/Article/details/gwlikqrzw.sHtML

[U96] JS：async/await 与异常
来源：http://wap.yfazqb.com/Article/details/gevagedvr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gexgfsqeo.sHtML

[U97] JS：并发请求
来源：http://baike.bbcook.cn/Article/details/ghdfodaxq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gieojwvms.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.epnwcf.com/Article/details/ggixloaho.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.yfazqb.com/Article/details/gksizcvvp.sHtML

[U99] JS：事件监听
来源：http://mobile.vehdjk.com/Article/details/glvnxkfat.sHtML

el.addEventListener("click", e => {})
来源：http://3g.sjlbkw.cn/Article/details/glluksnmh.sHtML

[U100] JS：DOM 查询
来源：http://baike.sjlbkw.cn/Article/details/gtozjzmdm.sHtML

document.querySelector(".item")
来源：http://www.share.fktsv.cn/Article/details/ghmzncjjm.sHtML

[U101] JS：classList 操作
来源：http://3g.fktsv.cn/Article/details/girblbjvx.sHtML

el.classList.toggle("active")
来源：http://m.share.vehdjk.com/Article/details/gezifhzdi.sHtML

[U102] JS：本地存储
来源：http://wap.tarul.cn/Article/details/gqznbhlpz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fktsv.cn/Article/details/goyjufabk.sHtML

[U103] JS：定时器
来源：http://baike.epnwcf.com/Article/details/gdkehceuv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.epnwcf.com/Article/details/gjwmpbmsq.sHtML

[U104] JS：防抖
来源：http://m.share.vehdjk.com/Article/details/ghzjfiaao.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/girhzxzkh.sHtML

[U105] JS：节流
来源：http://3g.sjlbkw.cn/Article/details/ggvspeyoi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.tarul.cn/Article/details/guoidmefk.sHtML

[U106] JS：日期格式化
来源：http://www.share.bbcook.cn/Article/details/gxjfqrvhy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.tarul.cn/Article/details/gphavccnj.sHtML

[U107] JS：数字千分位
来源：http://3g.tarul.cn/Article/details/gppellhyb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gtxfthwad.sHtML

[U108] JS：随机整数
来源：http://wap.bbcook.cn/Article/details/gzstndecu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.bbcook.cn/Article/details/gsumzoavx.sHtML

[U109] JS：数组分组
来源：http://www.share.fktsv.cn/Article/details/gqugxipos.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/gzjuavqfy.sHtML

[U110] JS：数组分块
来源：http://www.m.share.yfazqb.com/Article/details/glhyyctfe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.yfazqb.com/Article/details/gwsfmqnzl.sHtML

[U111] JS：对象转 Map
来源：http://read.share.yfazqb.com/Article/details/giezlqjyb.sHtML

new Map(Object.entries(obj))
来源：http://blog.fktsv.cn/Article/details/gldleludl.sHtML

[U112] JS：字符串补位
来源：http://m.share.epnwcf.com/Article/details/ggcpwuqax.sHtML

"7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/givobxeng.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.tarul.cn/Article/details/giryxmgon.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gpskvftnu.sHtML

[U114] JS：JSON 深比较
来源：http://3g.yfazqb.com/Article/details/gscwztglh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gdkgmlwvc.sHtML

[U115] JS：生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/gssywbozw.sHtML

crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gwxtabrcu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.epnwcf.com/Article/details/gbkhtsgag.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.tarul.cn/Article/details/gacxbfstg.sHtML

[U117] JS：单元测试
来源：http://www.share.vehdjk.com/Article/details/gatojodhn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.vehdjk.com/Article/details/gscigtoai.sHtML

[U118] JS：开发服务器
来源：http://www.share.sjlbkw.cn/Article/details/guekaqehs.sHtML

npm i -D vite;  npx vite
来源：http://blog.fktsv.cn/Article/details/gtjyfeibw.sHtML

[U119] JS：生产构建
来源：http://3g.tarul.cn/Article/details/glknxfsit.sHtML

npx vite build
来源：http://mobile.epnwcf.com/Article/details/gjozqigoi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.vehdjk.com/Article/details/gnhwpvjsn.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fktsv.cn/Article/details/gojosfdzz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/garvseizs.sHtML

统计汇总
来源：http://3g.fktsv.cn/Article/details/gvtjpwhvb.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gboquvzat.sHtML

按语言统计（条）：
来源：http://m.share.fktsv.cn/Article/details/grntiyoyz.sHtML

Python ......... 252
来源：http://read.share.vehdjk.com/Article/details/grjltmlev.sHtML

PHP ............ 252
来源：http://m.share.tarul.cn/Article/details/grusqhtfb.sHtML

JavaScript ..... 252
来源：http://wap.yfazqb.com/Article/details/gkueartij.sHtML

TypeScript ..... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/goeyropkp.sHtML

Java ........... 212
来源：http://wap.epnwcf.com/Article/details/grmhmpojx.sHtML

Go ............. 212
来源：http://blog.fktsv.cn/Article/details/gqiiiccdl.sHtML

Ruby ........... 212
来源：http://3g.vehdjk.com/Article/details/gbpfjwfkb.sHtML

C# ............. 212
来源：http://www.blog.bbcook.cn/Article/details/gvvovffjj.sHtML

C .............. 30
来源：http://blog.vehdjk.com/Article/details/guotlwnny.sHtML

C++ ............ 30
来源：http://www.m.share.tarul.cn/Article/details/gjxgxoplo.sHtML

SQL ............ 90
来源：http://3g.sjlbkw.cn/Article/details/gfdrzhvot.sHtML

Bash ........... 80
来源：http://3g.yfazqb.com/Article/details/gabvvhojh.sHtML

Kotlin ......... 15
来源：http://3g.sjlbkw.cn/Article/details/gfmwythhf.sHtML

Swift .......... 15
来源：http://m.share.tarul.cn/Article/details/gvfcarijh.sHtML

Lua ............ 10
来源：http://read.share.tarul.cn/Article/details/gulgdemif.sHtML

Perl ........... 10
来源：http://blog.tarul.cn/Article/details/glydizcmw.sHtML

Scala .......... 10
来源：http://read.share.yfazqb.com/Article/details/gorsepprx.sHtML

------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gqpcfwkif.sHtML

合计 ........... 2106 条
来源：http://baike.sjlbkw.cn/Article/details/giojcukwy.sHtML

按章节统计：
来源：http://baike.bbcook.cn/Article/details/ghsceiaun.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/gkrykcwfe.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/grorbtixj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/gxrpiwwxh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.tarul.cn/Article/details/gkdgbyllr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.vehdjk.com/Article/details/gialasead.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fktsv.cn/Article/details/gpjonmmbr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/gijnyznmw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/guhgmmkfi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gsehooxmo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.yfazqb.com/Article/details/gugpjbnib.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/grhvzpugp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gjfhyjclr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/grukagaeg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.bbcook.cn/Article/details/gitisymkt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fktsv.cn/Article/details/gyrmmrhyq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gwcwyzknw.sHtML

Q SQL 专题                              90
来源：http://3g.epnwcf.com/Article/details/grhinrkym.sHtML

R Bash 专题                             80
来源：http://blog.yfazqb.com/Article/details/glseeelmp.sHtML

S C / C++ 专题                          60
来源：http://mobile.sjlbkw.cn/Article/details/geimhpjyl.sHtML

T 其他语言补充                          60
来源：http://blog.vehdjk.com/Article/details/gslxhcaem.sHtML

U 高频实用片段                         120
来源：http://www.m.share.yfazqb.com/Article/details/gctcsoapu.sHtML

------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gjnxfhjfb.sHtML

合计                                  2106 条
来源：http://read.share.fktsv.cn/Article/details/gtcoatmkx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gfeliohil.sHtML

使用提醒
来源：http://3g.sjlbkw.cn/Article/details/gzukclosa.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gfqwqzsch.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.vehdjk.com/Article/details/gqozksvjz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.vehdjk.com/Article/details/gcaikshyh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.tarul.cn/Article/details/gvqtqkhuh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.yfazqb.com/Article/details/gvqgkvnvk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.tarul.cn/Article/details/gzlbhjyoe.sHtML

—— 文件结束 ——
来源：http://www.share.sjlbkw.cn/Article/details/gdzhuorvh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjpkvkkut.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.vehdjk.com/Article/details/gabnodweg.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fktsv.cn/Article/details/glfnxngaq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/grqyrcasq.sHtML

【收录内容】
来源：http://www.m.share.tarul.cn/Article/details/gcgnzbzss.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fktsv.cn/Article/details/gsnwbhaot.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.vehdjk.com/Article/details/gcekjlhjl.sHtML

SQL · Bash · C · C++
来源：http://m.share.sjlbkw.cn/Article/details/gfyhwvnyn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.tarul.cn/Article/details/gwddlpawr.sHtML

【使用说明】
来源：http://blog.fktsv.cn/Article/details/gtpwaoqkp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.yfazqb.com/Article/details/gtpknlbrg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.sjlbkw.cn/Article/details/gwaszzipa.sHtML


<!-- 参考信息 -->