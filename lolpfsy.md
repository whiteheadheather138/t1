代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.share.epnwcf.com/Article/details/gxlseyeke.sHtML

list(dict.fromkeys(arr))
来源：http://blog.tarul.cn/Article/details/gzoslzloi.sHtML

[U06] Py：合并两个字典
来源：http://m.share.epnwcf.com/Article/details/gsiienszq.sHtML

{**a, **b}
来源：http://3g.vehdjk.com/Article/details/gwbsmnlyq.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fktsv.cn/Article/details/gkgzoqehp.sHtML

{v: k for k, v in d.items()}
来源：http://3g.vehdjk.com/Article/details/gsqrykmtw.sHtML

[U08] Py：展平二维列表
来源：http://3g.tarul.cn/Article/details/gjyfmcmnx.sHtML

[y for x in nested for y in x]
来源：http://mobile.vehdjk.com/Article/details/gunqxvwzd.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fktsv.cn/Article/details/gnesmunns.sHtML

max(d, key=d.get)
来源：http://3g.bbcook.cn/Article/details/gybzcxfwr.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.vehdjk.com/Article/details/gbisrbuce.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.yfazqb.com/Article/details/gvbrngyfq.sHtML

[U11] Py：生成器表达式
来源：http://read.share.yfazqb.com/Article/details/gsfgrvuyt.sHtML

(x * 2 for x in arr)
来源：http://baike.vehdjk.com/Article/details/gjhrrzqwz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fktsv.cn/Article/details/gqkbsurer.sHtML

Counter(arr).most_common(3)
来源：http://wap.tarul.cn/Article/details/gkfmmdeny.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxbazlxm.sHtML

deque(maxlen=10)
来源：http://read.share.vehdjk.com/Article/details/gzjqxetif.sHtML

[U14] Py：分组收集到列表
来源：http://wap.bbcook.cn/Article/details/goylzoplg.sHtML

defaultdict(list)
来源：http://3g.sjlbkw.cn/Article/details/gkreyvjyp.sHtML

[U15] Py：高精度计时
来源：http://read.share.vehdjk.com/Article/details/ghtmqrjbu.sHtML

t = time.perf_counter()
来源：http://www.blog.fktsv.cn/Article/details/gwqpxtpyf.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.yfazqb.com/Article/details/gizwfvwwt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fktsv.cn/Article/details/glmplmpav.sHtML

[U17] Py：初始化日志
来源：http://wap.tarul.cn/Article/details/gtxaltrzn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.epnwcf.com/Article/details/gqbrlgtzh.sHtML

[U18] Py：预编译正则
来源：http://www.share.sjlbkw.cn/Article/details/gfqdbjjnp.sHtML

pat = re.compile(r"\d+")
来源：http://wap.epnwcf.com/Article/details/gbbvbkwma.sHtML

[U19] Py：正则替换带回调
来源：http://3g.vehdjk.com/Article/details/grsfgcevb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.tarul.cn/Article/details/gexrmnned.sHtML

[U20] Py：缓存函数结果
来源：http://wap.epnwcf.com/Article/details/gjtloxjii.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.sjlbkw.cn/Article/details/gyczskppi.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.sjlbkw.cn/Article/details/gzmqqwhyi.sHtML

@contextlib.contextmanager
来源：http://blog.epnwcf.com/Article/details/ghezpxlse.sHtML

[U22] Py：矩阵转置
来源：http://blog.yfazqb.com/Article/details/gsbolkzmj.sHtML

list(zip(*m))
来源：http://mobile.bbcook.cn/Article/details/gdsknveoo.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.bbcook.cn/Article/details/gcfwtijbs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.bbcook.cn/Article/details/gyopwakrf.sHtML

[U24] Py：路径操作
来源：http://read.share.yfazqb.com/Article/details/goebyihce.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/ggjvxbtkd.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.vehdjk.com/Article/details/gzmsdtzmn.sHtML

csv.DictReader(f)
来源：http://wap.bbcook.cn/Article/details/gjczntmvu.sHtML

[U26] Py：并发下载
来源：http://www.share.vehdjk.com/Article/details/gpoepkusx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.vehdjk.com/Article/details/guzotsvmc.sHtML

[U27] Py：异步 HTTP
来源：http://wap.tarul.cn/Article/details/gxfiscwiy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.vehdjk.com/Article/details/ghxevuiuf.sHtML

[U28] Py：类型别名
来源：http://baike.yfazqb.com/Article/details/glhrcpxfo.sHtML

UserId = int
来源：http://read.share.fktsv.cn/Article/details/glvklffok.sHtML

[U29] Py：属性校验
来源：http://www.blog.tarul.cn/Article/details/gaymsaato.sHtML

@property 与 @x.setter 配合
来源：http://blog.epnwcf.com/Article/details/gaxgpsois.sHtML

[U30] Py：数据类
来源：http://3g.fktsv.cn/Article/details/gkszrwhxh.sHtML

@dataclass(slots=True)
来源：http://3g.yfazqb.com/Article/details/gggbihubs.sHtML

[U31] Py：单测
来源：http://read.share.tarul.cn/Article/details/gbdqxglra.sHtML

python -m pytest -q
来源：http://www.m.share.yfazqb.com/Article/details/gkfdwwyke.sHtML

[U32] Py：代码格式化
来源：http://read.share.vehdjk.com/Article/details/geoabrbfs.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.vehdjk.com/Article/details/gybgxwvlj.sHtML

[U33] Py：打包发布
来源：http://blog.vehdjk.com/Article/details/ghdefyulx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.tarul.cn/Article/details/gnzryomkh.sHtML

[U34] Py：判断编码
来源：http://www.blog.yfazqb.com/Article/details/gejpfzhpx.sHtML

chardet.detect(raw)
来源：http://wap.vehdjk.com/Article/details/gscjjcqca.sHtML

[U35] Py：发送邮件
来源：http://mobile.fktsv.cn/Article/details/gimyonetx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.bbcook.cn/Article/details/gyjmihrfy.sHtML

[U36] Py：定时任务
来源：http://mobile.yfazqb.com/Article/details/gnihzqeeo.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fktsv.cn/Article/details/ghifxkrcx.sHtML

[U37] Py：读写 Excel
来源：http://m.share.yfazqb.com/Article/details/gcbkickey.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.yfazqb.com/Article/details/gsmcgfbnt.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.vehdjk.com/Article/details/gastqgthg.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.bbcook.cn/Article/details/gezsurgyr.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.bbcook.cn/Article/details/gzumawiwn.sHtML

sys.stdout.isatty()
来源：http://baike.bbcook.cn/Article/details/gdqdzxtaz.sHtML

[U40] Py：打印到标准错误
来源：http://wap.epnwcf.com/Article/details/giynfguts.sHtML

print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/gtjyoftml.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.sjlbkw.cn/Article/details/grjonzjyq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/ghiyawhmz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.tarul.cn/Article/details/glztdapwq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fktsv.cn/Article/details/gpfxxiaiw.sHtML

[U43] PHP：声明命名空间
来源：http://wap.vehdjk.com/Article/details/gjficaeho.sHtML

namespace App\Http;
来源：http://blog.vehdjk.com/Article/details/gmcfhiyvz.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.yfazqb.com/Article/details/gwbddiwzx.sHtML

declare(strict_types=1);
来源：http://www.share.bbcook.cn/Article/details/galbanado.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.sjlbkw.cn/Article/details/gmnbhaqok.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gpjqfwjdz.sHtML

[U46] PHP：可空类型
来源：http://read.share.yfazqb.com/Article/details/gubmjvdhh.sHtML

?string $name = null
来源：http://www.share.fktsv.cn/Article/details/gasarxnjg.sHtML

[U47] PHP：联合类型
来源：http://wap.sjlbkw.cn/Article/details/gypgelxdv.sHtML

int|string $id
来源：http://read.share.fktsv.cn/Article/details/gqolleafi.sHtML

[U48] PHP：纯枚举
来源：http://3g.epnwcf.com/Article/details/gegpwhtvh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.yfazqb.com/Article/details/gwehxktof.sHtML

[U49] PHP：只读属性
来源：http://read.share.vehdjk.com/Article/details/gnfvjoeet.sHtML

public readonly string $name
来源：http://www.blog.epnwcf.com/Article/details/gvlhgxgsu.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.tarul.cn/Article/details/gmcsuziws.sHtML

public function __construct(private int $id) {}
来源：http://www.share.sjlbkw.cn/Article/details/gbxdkccgg.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkqxducc.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.yfazqb.com/Article/details/gowhvduhh.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gpaeksykx.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.epnwcf.com/Article/details/gdyicbpvl.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.yfazqb.com/Article/details/gvvxjqrxu.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.vehdjk.com/Article/details/geqnkvuzt.sHtML

[U54] PHP：空安全调用
来源：http://blog.vehdjk.com/Article/details/grsskgtdc.sHtML

$obj?->method()
来源：http://3g.sjlbkw.cn/Article/details/gflszjaku.sHtML

[U55] PHP：match 表达式
来源：http://m.share.tarul.cn/Article/details/gebptlbfk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fktsv.cn/Article/details/gcgvuqjyw.sHtML

[U56] PHP：命名参数
来源：http://mobile.tarul.cn/Article/details/gfigpjqcb.sHtML

f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gsnkbflzn.sHtML

[U57] PHP：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gpdfawity.sHtML

"值: {$a}"
来源：http://www.blog.bbcook.cn/Article/details/gmjscioaw.sHtML

[U58] PHP：数组三件套
来源：http://blog.yfazqb.com/Article/details/gxeosbtps.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gunmcuxxp.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.tarul.cn/Article/details/gucdfpmfn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gjrrcxhzw.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.vehdjk.com/Article/details/gtnipnlul.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.tarul.cn/Article/details/gubegexfz.sHtML

[U61] PHP：正则
来源：http://mobile.fktsv.cn/Article/details/gkwewlqff.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.epnwcf.com/Article/details/gfmqajipv.sHtML

[U62] PHP：日期对象
来源：http://blog.yfazqb.com/Article/details/gstkqleso.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.vehdjk.com/Article/details/gftclayjy.sHtML

[U63] PHP：文件读写
来源：http://read.share.yfazqb.com/Article/details/gpgmkgfhe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.vehdjk.com/Article/details/gtriifyxc.sHtML

[U64] PHP：目录遍历
来源：http://blog.bbcook.cn/Article/details/gsopjioqk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.yfazqb.com/Article/details/gacxjrfec.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/gbbfpgxeb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gfoslmfdg.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.tarul.cn/Article/details/gjfjxkhnr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.bbcook.cn/Article/details/gsnmapkys.sHtML

[U67] PHP：处理文件上传
来源：http://blog.sjlbkw.cn/Article/details/gcycqgnih.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fktsv.cn/Article/details/ghvesdhmd.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.bbcook.cn/Article/details/gbsuvgspu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.vehdjk.com/Article/details/gxaxygjyc.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.vehdjk.com/Article/details/gdwgehvxr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.bbcook.cn/Article/details/gafrlaimn.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.tarul.cn/Article/details/gkrkjldss.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.epnwcf.com/Article/details/gbcvytmif.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/gbyrmjfbk.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fktsv.cn/Article/details/ggfbxbzyj.sHtML

[U72] PHP：写错误日志
来源：http://baike.sjlbkw.cn/Article/details/ghumucwbm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.vehdjk.com/Article/details/gbovikzxw.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.tarul.cn/Article/details/gwwikrpum.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.bbcook.cn/Article/details/gojqnabkq.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.tarul.cn/Article/details/guuujtapr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fktsv.cn/Article/details/gcqwmtfpl.sHtML

[U75] PHP：依赖注入
来源：http://baike.yfazqb.com/Article/details/gcdcwklhj.sHtML

composer require psr/container
来源：http://mobile.sjlbkw.cn/Article/details/gsoadibfb.sHtML

[U76] PHP：简单路由
来源：http://mobile.vehdjk.com/Article/details/gtllovdys.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.vehdjk.com/Article/details/ggtvtfbcv.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.vehdjk.com/Article/details/gvvgluxqb.sHtML

composer require twig/twig
来源：http://baike.yfazqb.com/Article/details/gdekknmiz.sHtML

[U78] PHP：单元测试
来源：http://blog.vehdjk.com/Article/details/grinxknjv.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.epnwcf.com/Article/details/gxapqypar.sHtML

[U79] PHP：静态分析
来源：http://3g.fktsv.cn/Article/details/gndcikqpg.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.bbcook.cn/Article/details/gwjucrduk.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.sjlbkw.cn/Article/details/grmprmmrq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.bbcook.cn/Article/details/giyggpkox.sHtML

[U81] JS：初始化项目
来源：http://baike.yfazqb.com/Article/details/gweludglp.sHtML

npm init -y;  npm i express
来源：http://m.share.bbcook.cn/Article/details/gboobirfu.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.tarul.cn/Article/details/gmfnssnjg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.yfazqb.com/Article/details/gwkbkkbll.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.tarul.cn/Article/details/gnspzqypq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.bbcook.cn/Article/details/ggzvcisqs.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.vehdjk.com/Article/details/glmvlywkk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.sjlbkw.cn/Article/details/gbzhgfddk.sHtML

[U85] JS：可选链
来源：http://baike.epnwcf.com/Article/details/gmojbzcwc.sHtML

a?.b?.c
来源：http://www.share.tarul.cn/Article/details/goiaqrzyl.sHtML

[U86] JS：空值合并
来源：http://www.share.bbcook.cn/Article/details/gzlkrliua.sHtML

a ?? b
来源：http://3g.yfazqb.com/Article/details/gbzxzxqxi.sHtML

[U87] JS：解构默认值
来源：http://read.share.vehdjk.com/Article/details/ghpbngypf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.tarul.cn/Article/details/gfmktickw.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.epnwcf.com/Article/details/gjjdmgrzh.sHtML

{ ...a, ...b }
来源：http://m.share.tarul.cn/Article/details/gqttiysiv.sHtML

[U89] JS：数组去重
来源：http://www.blog.bbcook.cn/Article/details/gwiwmmjqj.sHtML

[...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gcykfmpdp.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.tarul.cn/Article/details/geivqyiny.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/glppishpg.sHtML

[U91] JS：对象键值遍历
来源：http://blog.tarul.cn/Article/details/gviqnngnz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fktsv.cn/Article/details/gbniqanwj.sHtML

[U92] JS：深拷贝
来源：http://3g.bbcook.cn/Article/details/gexjdwfbw.sHtML

structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gesjrxflp.sHtML

[U93] JS：模板字符串
来源：http://baike.fktsv.cn/Article/details/gixajpypa.sHtML

`共 ${n} 条`
来源：http://www.m.share.fktsv.cn/Article/details/gncuunucj.sHtML

[U94] JS：箭头函数
来源：http://blog.fktsv.cn/Article/details/gjvfwnzmi.sHtML

const double = x => x * 2;
来源：http://mobile.fktsv.cn/Article/details/ggwcakngb.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fktsv.cn/Article/details/gkorgnnyf.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.bbcook.cn/Article/details/gvxkqseey.sHtML

[U96] JS：async/await 与异常
来源：http://wap.sjlbkw.cn/Article/details/ghupvdzzz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gyzcjqgqd.sHtML

[U97] JS：并发请求
来源：http://www.blog.vehdjk.com/Article/details/gmgbgiwmi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gyjmjcphb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fktsv.cn/Article/details/gkembkwxz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.yfazqb.com/Article/details/gaoqbgzya.sHtML

[U99] JS：事件监听
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlxxnntm.sHtML

el.addEventListener("click", e => {})
来源：http://3g.tarul.cn/Article/details/gbtlxqnox.sHtML

[U100] JS：DOM 查询
来源：http://read.share.bbcook.cn/Article/details/gawjatnzo.sHtML

document.querySelector(".item")
来源：http://3g.sjlbkw.cn/Article/details/gjrvkzwws.sHtML

[U101] JS：classList 操作
来源：http://3g.yfazqb.com/Article/details/gdgnpdqur.sHtML

el.classList.toggle("active")
来源：http://3g.vehdjk.com/Article/details/gcocfzjwe.sHtML

[U102] JS：本地存储
来源：http://baike.fktsv.cn/Article/details/glejdybuw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.bbcook.cn/Article/details/gvacehzfp.sHtML

[U103] JS：定时器
来源：http://baike.sjlbkw.cn/Article/details/gutshhqxx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.vehdjk.com/Article/details/guzqrvcjv.sHtML

[U104] JS：防抖
来源：http://www.blog.fktsv.cn/Article/details/goxkqvfib.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gmvjxhuhw.sHtML

[U105] JS：节流
来源：http://www.m.share.bbcook.cn/Article/details/gevnroakp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.vehdjk.com/Article/details/gmkwbjgru.sHtML

[U106] JS：日期格式化
来源：http://blog.bbcook.cn/Article/details/gyfkucnkw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fktsv.cn/Article/details/gdwgruxvy.sHtML

[U107] JS：数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/gzhkbebfp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gnmagwtks.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fktsv.cn/Article/details/gtgopdruy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fktsv.cn/Article/details/gahxetcan.sHtML

[U109] JS：数组分组
来源：http://wap.vehdjk.com/Article/details/gldyxymlb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/geoqzilgm.sHtML

[U110] JS：数组分块
来源：http://www.m.share.bbcook.cn/Article/details/ghkzqtdsx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fktsv.cn/Article/details/gzkrmjoua.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fktsv.cn/Article/details/gpyabycyb.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.vehdjk.com/Article/details/ggkzvuxmv.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.vehdjk.com/Article/details/gyltlqwmo.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gteoiekqp.sHtML

[U113] JS：正则替换全部
来源：http://3g.epnwcf.com/Article/details/geaorghgn.sHtML

s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gwuxtxtkt.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fktsv.cn/Article/details/gynuuixta.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.bbcook.cn/Article/details/ggoqubljd.sHtML

[U115] JS：生成 UUID
来源：http://3g.yfazqb.com/Article/details/glrmiomff.sHtML

crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/grwentalb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.vehdjk.com/Article/details/gzlhnrbjm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.yfazqb.com/Article/details/gfxjxohhz.sHtML

[U117] JS：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gmtnufpdk.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.sjlbkw.cn/Article/details/gprrcrcfk.sHtML

[U118] JS：开发服务器
来源：http://m.share.fktsv.cn/Article/details/gfsjqwjgl.sHtML

npm i -D vite;  npx vite
来源：http://www.share.tarul.cn/Article/details/gzuwynbnp.sHtML

[U119] JS：生产构建
来源：http://www.blog.fktsv.cn/Article/details/ggkdjrbqr.sHtML

npx vite build
来源：http://3g.epnwcf.com/Article/details/gynajfkuv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.sjlbkw.cn/Article/details/gokdbtxpw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.vehdjk.com/Article/details/gsbekvvte.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gyjunkska.sHtML

统计汇总
来源：http://www.m.share.bbcook.cn/Article/details/gxzaxfaga.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gnqzhsdgq.sHtML

按语言统计（条）：
来源：http://wap.yfazqb.com/Article/details/gblqnszfx.sHtML

Python ......... 252
来源：http://www.blog.fktsv.cn/Article/details/gmezhveyx.sHtML

PHP ............ 252
来源：http://3g.tarul.cn/Article/details/gtlphwxlw.sHtML

JavaScript ..... 252
来源：http://baike.epnwcf.com/Article/details/gplcfmcci.sHtML

TypeScript ..... 212
来源：http://www.share.tarul.cn/Article/details/gmhqqwlmd.sHtML

Java ........... 212
来源：http://read.share.vehdjk.com/Article/details/goauhhdqv.sHtML

Go ............. 212
来源：http://blog.sjlbkw.cn/Article/details/gjvbylfqc.sHtML

Ruby ........... 212
来源：http://mobile.tarul.cn/Article/details/geppumvzs.sHtML

C# ............. 212
来源：http://blog.vehdjk.com/Article/details/gawlrazwu.sHtML

C .............. 30
来源：http://read.share.epnwcf.com/Article/details/gbajinces.sHtML

C++ ............ 30
来源：http://www.share.yfazqb.com/Article/details/gzvyqpqhk.sHtML

SQL ............ 90
来源：http://www.blog.vehdjk.com/Article/details/ginkovskv.sHtML

Bash ........... 80
来源：http://www.m.share.fktsv.cn/Article/details/gbtzxekgh.sHtML

Kotlin ......... 15
来源：http://www.m.share.epnwcf.com/Article/details/gthsiqdqr.sHtML

Swift .......... 15
来源：http://mobile.sjlbkw.cn/Article/details/gcncxerkt.sHtML

Lua ............ 10
来源：http://www.blog.epnwcf.com/Article/details/gnurcsqrb.sHtML

Perl ........... 10
来源：http://www.share.vehdjk.com/Article/details/griugsogj.sHtML

Scala .......... 10
来源：http://baike.tarul.cn/Article/details/gkvtyrsac.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gvqxlpmck.sHtML

合计 ........... 2106 条
来源：http://read.share.sjlbkw.cn/Article/details/gssekdojp.sHtML

按章节统计：
来源：http://read.share.yfazqb.com/Article/details/gzsjawtuw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.epnwcf.com/Article/details/gexzoyudj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/gpcmeksnr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjokjwhg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.vehdjk.com/Article/details/gxvxfothu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.bbcook.cn/Article/details/gbolpkzyo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fktsv.cn/Article/details/gggzekhjr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/ggaciaksw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.yfazqb.com/Article/details/guiclanwj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gfpvvdkem.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.tarul.cn/Article/details/gnwhdyaek.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gdqvogril.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gesapxthu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gatqmszwv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fktsv.cn/Article/details/gjdzxkead.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.sjlbkw.cn/Article/details/guhbjehii.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gvkfgaxuy.sHtML

Q SQL 专题                              90
来源：http://blog.vehdjk.com/Article/details/gmfsllvwl.sHtML

R Bash 专题                             80
来源：http://m.share.bbcook.cn/Article/details/gxrjccobw.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.vehdjk.com/Article/details/gaicojbdr.sHtML

T 其他语言补充                          60
来源：http://baike.sjlbkw.cn/Article/details/giyingwwx.sHtML

U 高频实用片段                         120
来源：http://mobile.sjlbkw.cn/Article/details/gegewpahi.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gjpepfvne.sHtML

合计                                  2106 条
来源：http://www.share.fktsv.cn/Article/details/gsaylovwv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gsgvvdztl.sHtML

使用提醒
来源：http://www.m.share.sjlbkw.cn/Article/details/ghircnfqk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gezddhmte.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.yfazqb.com/Article/details/gkqrrqnlw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.tarul.cn/Article/details/gegxpjqex.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.tarul.cn/Article/details/ghcifzign.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.tarul.cn/Article/details/gsachenfj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fktsv.cn/Article/details/gdfftskiy.sHtML

—— 文件结束 ——
来源：http://blog.tarul.cn/Article/details/gwmsoeebe.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gorcamihz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.bbcook.cn/Article/details/gascmwdsz.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.epnwcf.com/Article/details/gkftgfdhn.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggehvmbdm.sHtML

【收录内容】
来源：http://baike.fktsv.cn/Article/details/glfqyikql.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fktsv.cn/Article/details/gijdjxfkr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.sjlbkw.cn/Article/details/goptybvsv.sHtML

SQL · Bash · C · C++
来源：http://m.share.sjlbkw.cn/Article/details/grfuucmqw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.tarul.cn/Article/details/ghbuwsqbd.sHtML

【使用说明】
来源：http://www.m.share.epnwcf.com/Article/details/gtcqoxiez.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.bbcook.cn/Article/details/gczsaphlo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.tarul.cn/Article/details/gdfchdbzl.sHtML


<!-- 参考信息 -->