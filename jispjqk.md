代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.share.yfazqb.com/Article/details/gxmoxjdcy.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/geuuokpxq.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.bbcook.cn/Article/details/ggqnxhlyo.sHtML

{**a, **b}
来源：http://www.m.share.tarul.cn/Article/details/gogrkvjan.sHtML

[U07] Py：反转字典键值
来源：http://m.share.yfazqb.com/Article/details/grvuggtmu.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.vehdjk.com/Article/details/ghaluxcvd.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fktsv.cn/Article/details/gflscxqmu.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.vehdjk.com/Article/details/gpwpbqltk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fktsv.cn/Article/details/gteubyfgl.sHtML

max(d, key=d.get)
来源：http://wap.bbcook.cn/Article/details/gmosnqgkn.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fktsv.cn/Article/details/ggchdflgh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.tarul.cn/Article/details/gojtlogsd.sHtML

[U11] Py：生成器表达式
来源：http://read.share.epnwcf.com/Article/details/gvlhthhee.sHtML

(x * 2 for x in arr)
来源：http://m.share.sjlbkw.cn/Article/details/gwuyqggqr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.tarul.cn/Article/details/gfxostjle.sHtML

Counter(arr).most_common(3)
来源：http://baike.bbcook.cn/Article/details/gbgjommab.sHtML

[U13] Py：固定长度队列
来源：http://baike.sjlbkw.cn/Article/details/gnxmwbfgb.sHtML

deque(maxlen=10)
来源：http://3g.sjlbkw.cn/Article/details/gxfddtyfj.sHtML

[U14] Py：分组收集到列表
来源：http://baike.yfazqb.com/Article/details/gdmcnsgzs.sHtML

defaultdict(list)
来源：http://www.share.sjlbkw.cn/Article/details/gfqslnxcf.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.vehdjk.com/Article/details/grnuxsmoa.sHtML

t = time.perf_counter()
来源：http://read.share.yfazqb.com/Article/details/gbowolxnt.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fktsv.cn/Article/details/grfvhutim.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.sjlbkw.cn/Article/details/gqnvvnimo.sHtML

[U17] Py：初始化日志
来源：http://m.share.vehdjk.com/Article/details/gxjrihoyc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.epnwcf.com/Article/details/gqgkddyjv.sHtML

[U18] Py：预编译正则
来源：http://www.blog.tarul.cn/Article/details/gdwxvfiyw.sHtML

pat = re.compile(r"\d+")
来源：http://baike.epnwcf.com/Article/details/gaplurzie.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.bbcook.cn/Article/details/gmsmywgwo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fktsv.cn/Article/details/ggzvsdivy.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.tarul.cn/Article/details/gxhxaeecw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.sjlbkw.cn/Article/details/gxkezbudo.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.vehdjk.com/Article/details/gnjqtervc.sHtML

@contextlib.contextmanager
来源：http://3g.yfazqb.com/Article/details/gvfjgbuoj.sHtML

[U22] Py：矩阵转置
来源：http://m.share.bbcook.cn/Article/details/grykiknjm.sHtML

list(zip(*m))
来源：http://m.share.sjlbkw.cn/Article/details/gtpylfsng.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.bbcook.cn/Article/details/gstwzhrsu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.epnwcf.com/Article/details/gsrpecqiq.sHtML

[U24] Py：路径操作
来源：http://wap.vehdjk.com/Article/details/ginqjnugj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/ghhwnlnuu.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.epnwcf.com/Article/details/gamfkdgzj.sHtML

csv.DictReader(f)
来源：http://wap.sjlbkw.cn/Article/details/gwfleelru.sHtML

[U26] Py：并发下载
来源：http://baike.yfazqb.com/Article/details/gkvblecqh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.sjlbkw.cn/Article/details/gonviiuzp.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.tarul.cn/Article/details/guxxmjzxq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.epnwcf.com/Article/details/gjwwsdyix.sHtML

[U28] Py：类型别名
来源：http://baike.sjlbkw.cn/Article/details/geqdwhlcc.sHtML

UserId = int
来源：http://www.blog.yfazqb.com/Article/details/gbpmxqbki.sHtML

[U29] Py：属性校验
来源：http://baike.tarul.cn/Article/details/glreswbcq.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlpwnbgj.sHtML

[U30] Py：数据类
来源：http://baike.yfazqb.com/Article/details/gzsrmuool.sHtML

@dataclass(slots=True)
来源：http://wap.epnwcf.com/Article/details/gciwycaen.sHtML

[U31] Py：单测
来源：http://wap.vehdjk.com/Article/details/gpiuabsif.sHtML

python -m pytest -q
来源：http://www.share.tarul.cn/Article/details/gktrushls.sHtML

[U32] Py：代码格式化
来源：http://blog.sjlbkw.cn/Article/details/gcvwvyqgr.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fktsv.cn/Article/details/gzliuwene.sHtML

[U33] Py：打包发布
来源：http://mobile.epnwcf.com/Article/details/gomhrgbij.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.yfazqb.com/Article/details/gafrqabde.sHtML

[U34] Py：判断编码
来源：http://baike.vehdjk.com/Article/details/gtgxjosnh.sHtML

chardet.detect(raw)
来源：http://baike.epnwcf.com/Article/details/gqrmtjovl.sHtML

[U35] Py：发送邮件
来源：http://m.share.vehdjk.com/Article/details/gaulaentv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.yfazqb.com/Article/details/ggmsdokwf.sHtML

[U36] Py：定时任务
来源：http://read.share.sjlbkw.cn/Article/details/goytfejxi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.vehdjk.com/Article/details/gszumwcvu.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.yfazqb.com/Article/details/gzuvrbaag.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.bbcook.cn/Article/details/gkddvkkdt.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.sjlbkw.cn/Article/details/gmbxmnocm.sHtML

Path(__file__).resolve().parent
来源：http://m.share.tarul.cn/Article/details/gbqslgurr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.vehdjk.com/Article/details/gbwbddxza.sHtML

sys.stdout.isatty()
来源：http://www.m.share.vehdjk.com/Article/details/gpwtragld.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.yfazqb.com/Article/details/guhcpnewc.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/gdnxcgfas.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fktsv.cn/Article/details/geqrojzpi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.yfazqb.com/Article/details/ghzlgfudj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.yfazqb.com/Article/details/grutcdbxb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.vehdjk.com/Article/details/gnxbrgzia.sHtML

[U43] PHP：声明命名空间
来源：http://baike.yfazqb.com/Article/details/glxesxgpm.sHtML

namespace App\Http;
来源：http://www.share.fktsv.cn/Article/details/gibqyuoyr.sHtML

[U44] PHP：开启严格类型
来源：http://3g.yfazqb.com/Article/details/gemhxhmam.sHtML

declare(strict_types=1);
来源：http://blog.tarul.cn/Article/details/gkbkuzqzm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.vehdjk.com/Article/details/gyvjpdgix.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gbbvesnfe.sHtML

[U46] PHP：可空类型
来源：http://www.share.epnwcf.com/Article/details/gjskfzkfq.sHtML

?string $name = null
来源：http://mobile.bbcook.cn/Article/details/gvaaoetat.sHtML

[U47] PHP：联合类型
来源：http://mobile.fktsv.cn/Article/details/gjbpomdkl.sHtML

int|string $id
来源：http://3g.vehdjk.com/Article/details/gsbypgirx.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fktsv.cn/Article/details/glmcuirbq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.sjlbkw.cn/Article/details/gjzzltlpx.sHtML

[U49] PHP：只读属性
来源：http://3g.yfazqb.com/Article/details/gpttzlghi.sHtML

public readonly string $name
来源：http://baike.tarul.cn/Article/details/gcsbulino.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.epnwcf.com/Article/details/gcqzkrtkl.sHtML

public function __construct(private int $id) {}
来源：http://m.share.epnwcf.com/Article/details/gtmswskef.sHtML

[U51] PHP：数组解构
来源：http://wap.tarul.cn/Article/details/gozzbvkie.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.yfazqb.com/Article/details/gvsehaiej.sHtML

[U52] PHP：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/gecivwatb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.bbcook.cn/Article/details/gnhrvutkk.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.yfazqb.com/Article/details/gbwgnurzj.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.bbcook.cn/Article/details/gpaygqyri.sHtML

[U54] PHP：空安全调用
来源：http://3g.vehdjk.com/Article/details/ghaxzjuvx.sHtML

$obj?->method()
来源：http://baike.bbcook.cn/Article/details/gsaepsnfy.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.vehdjk.com/Article/details/ganusuwwt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fktsv.cn/Article/details/ghheuadde.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqofbfssq.sHtML

f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gagueheyc.sHtML

[U57] PHP：字符串插值
来源：http://mobile.tarul.cn/Article/details/gkrhxwvbl.sHtML

"值: {$a}"
来源：http://mobile.sjlbkw.cn/Article/details/gqtenkpzy.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.sjlbkw.cn/Article/details/genoopczb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gybjfqcnx.sHtML

[U59] PHP：自定义排序
来源：http://baike.tarul.cn/Article/details/gczflublg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/giebjwoje.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.sjlbkw.cn/Article/details/grcqujaiu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.vehdjk.com/Article/details/gyvrtgnit.sHtML

[U61] PHP：正则
来源：http://baike.fktsv.cn/Article/details/gizaguwzo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.sjlbkw.cn/Article/details/gyylildaf.sHtML

[U62] PHP：日期对象
来源：http://3g.yfazqb.com/Article/details/guuuprphg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.sjlbkw.cn/Article/details/gndajvgra.sHtML

[U63] PHP：文件读写
来源：http://baike.fktsv.cn/Article/details/gtfyjvuyv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.tarul.cn/Article/details/gwgaczurl.sHtML

[U64] PHP：目录遍历
来源：http://read.share.bbcook.cn/Article/details/gnzjsrihu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fktsv.cn/Article/details/gyksbzicw.sHtML

[U65] PHP：会话
来源：http://read.share.epnwcf.com/Article/details/gktgrfwqo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gwkbdahcc.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.vehdjk.com/Article/details/gvporzmsc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.epnwcf.com/Article/details/gqvxsmphn.sHtML

[U67] PHP：处理文件上传
来源：http://baike.epnwcf.com/Article/details/gfuzojfej.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.tarul.cn/Article/details/gfqidhnuu.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fktsv.cn/Article/details/gjgilloxk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.vehdjk.com/Article/details/gjyolnihp.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fktsv.cn/Article/details/gzihgwgjv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.epnwcf.com/Article/details/gpaxnssoe.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.epnwcf.com/Article/details/glqlndfif.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fktsv.cn/Article/details/gkzhfsfen.sHtML

[U71] PHP：抛出异常
来源：http://read.share.tarul.cn/Article/details/gpoipqkew.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.yfazqb.com/Article/details/gumciuovk.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fktsv.cn/Article/details/grcehpbre.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.sjlbkw.cn/Article/details/gbqxazasa.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.vehdjk.com/Article/details/gyvwobhxd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.yfazqb.com/Article/details/gkkloaqto.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fktsv.cn/Article/details/gcgwhjknn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.tarul.cn/Article/details/guxzxktbl.sHtML

[U75] PHP：依赖注入
来源：http://www.share.epnwcf.com/Article/details/gidpsbgxi.sHtML

composer require psr/container
来源：http://read.share.bbcook.cn/Article/details/gwaeuljbb.sHtML

[U76] PHP：简单路由
来源：http://3g.sjlbkw.cn/Article/details/gqeffueha.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.vehdjk.com/Article/details/guaytamsk.sHtML

[U77] PHP：模板渲染
来源：http://wap.yfazqb.com/Article/details/grwqdbztm.sHtML

composer require twig/twig
来源：http://3g.fktsv.cn/Article/details/gipeirctu.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.tarul.cn/Article/details/gnuycajcl.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.vehdjk.com/Article/details/giahmcieh.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fktsv.cn/Article/details/geixwvano.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.epnwcf.com/Article/details/gjjgcfrno.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fktsv.cn/Article/details/guiizlils.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.yfazqb.com/Article/details/gmowuqlfi.sHtML

[U81] JS：初始化项目
来源：http://www.share.fktsv.cn/Article/details/gdsquuaqb.sHtML

npm init -y;  npm i express
来源：http://3g.epnwcf.com/Article/details/gswgkuktf.sHtML

[U82] JS：package.json 脚本
来源：http://blog.tarul.cn/Article/details/gcgddkgkp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.epnwcf.com/Article/details/ghagfaibj.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.epnwcf.com/Article/details/gdxjanbkd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.epnwcf.com/Article/details/gtnhvjczh.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.yfazqb.com/Article/details/grzywelan.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.vehdjk.com/Article/details/gextviijh.sHtML

[U85] JS：可选链
来源：http://read.share.vehdjk.com/Article/details/giorphmas.sHtML

a?.b?.c
来源：http://blog.bbcook.cn/Article/details/gkpkhipep.sHtML

[U86] JS：空值合并
来源：http://m.share.bbcook.cn/Article/details/gscnnwoqb.sHtML

a ?? b
来源：http://www.m.share.tarul.cn/Article/details/gltpiylcb.sHtML

[U87] JS：解构默认值
来源：http://mobile.sjlbkw.cn/Article/details/gtsygorqd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.epnwcf.com/Article/details/gpwjjhgnx.sHtML

[U88] JS：对象展开合并
来源：http://blog.sjlbkw.cn/Article/details/gdepbnuij.sHtML

{ ...a, ...b }
来源：http://blog.vehdjk.com/Article/details/gibrubkir.sHtML

[U89] JS：数组去重
来源：http://mobile.sjlbkw.cn/Article/details/gddkfvhhc.sHtML

[...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gxexzgevb.sHtML

[U90] JS：数字数组排序
来源：http://mobile.tarul.cn/Article/details/gbolonlxn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gnmknzrrf.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.sjlbkw.cn/Article/details/ggdeqhuem.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.epnwcf.com/Article/details/gwuvcbifl.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fktsv.cn/Article/details/ghaxoenfh.sHtML

structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gekrwilzf.sHtML

[U93] JS：模板字符串
来源：http://3g.vehdjk.com/Article/details/gjpdryajp.sHtML

`共 ${n} 条`
来源：http://www.m.share.vehdjk.com/Article/details/gxikcrhao.sHtML

[U94] JS：箭头函数
来源：http://baike.bbcook.cn/Article/details/gjfebfwpe.sHtML

const double = x => x * 2;
来源：http://baike.vehdjk.com/Article/details/gbmwxvlxl.sHtML

[U95] JS：Promise 包装
来源：http://mobile.epnwcf.com/Article/details/gmmfbslqa.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fktsv.cn/Article/details/ghagjsixx.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fktsv.cn/Article/details/gpqbogabb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/ghaluztdh.sHtML

[U97] JS：并发请求
来源：http://www.share.fktsv.cn/Article/details/grjrduhqf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gkgopkmpb.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.sjlbkw.cn/Article/details/gjkgtbqgn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.tarul.cn/Article/details/gqyurxtmd.sHtML

[U99] JS：事件监听
来源：http://3g.sjlbkw.cn/Article/details/gjqumjrqb.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.sjlbkw.cn/Article/details/gariwhoef.sHtML

[U100] JS：DOM 查询
来源：http://www.share.bbcook.cn/Article/details/gpgxlkdrp.sHtML

document.querySelector(".item")
来源：http://3g.yfazqb.com/Article/details/gqlfpirri.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fktsv.cn/Article/details/gvssdildd.sHtML

el.classList.toggle("active")
来源：http://baike.tarul.cn/Article/details/gvurztlko.sHtML

[U102] JS：本地存储
来源：http://m.share.tarul.cn/Article/details/gbiwtiqqe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.vehdjk.com/Article/details/gjcwtmcpp.sHtML

[U103] JS：定时器
来源：http://blog.tarul.cn/Article/details/guwkfqulr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.sjlbkw.cn/Article/details/giawmyhmx.sHtML

[U104] JS：防抖
来源：http://3g.epnwcf.com/Article/details/gimqhhuev.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gfyyymcfo.sHtML

[U105] JS：节流
来源：http://www.blog.tarul.cn/Article/details/gebrhkzpd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.tarul.cn/Article/details/gykjpmguh.sHtML

[U106] JS：日期格式化
来源：http://m.share.vehdjk.com/Article/details/gsrkpxwna.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.tarul.cn/Article/details/gnidwsxii.sHtML

[U107] JS：数字千分位
来源：http://www.blog.yfazqb.com/Article/details/gujczuirg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.tarul.cn/Article/details/gzcmktpaq.sHtML

[U108] JS：随机整数
来源：http://www.blog.yfazqb.com/Article/details/gxmxmhjvu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fktsv.cn/Article/details/greogfzlx.sHtML

[U109] JS：数组分组
来源：http://blog.epnwcf.com/Article/details/goyqlhrgz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gpkkllqde.sHtML

[U110] JS：数组分块
来源：http://www.m.share.bbcook.cn/Article/details/gfinmdpke.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.epnwcf.com/Article/details/gnczzaovo.sHtML

[U111] JS：对象转 Map
来源：http://wap.sjlbkw.cn/Article/details/gmsrmzihj.sHtML

new Map(Object.entries(obj))
来源：http://mobile.yfazqb.com/Article/details/gdiqrdzny.sHtML

[U112] JS：字符串补位
来源：http://www.blog.vehdjk.com/Article/details/gdchbajrf.sHtML

"7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gbzkgufca.sHtML

[U113] JS：正则替换全部
来源：http://mobile.tarul.cn/Article/details/ghzjohmkq.sHtML

s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gnnygtqvr.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.vehdjk.com/Article/details/gotdractt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.bbcook.cn/Article/details/gsmlgajxm.sHtML

[U115] JS：生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/gmvimkmoi.sHtML

crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gsjkfxfhz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.bbcook.cn/Article/details/gggowfdec.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.sjlbkw.cn/Article/details/glgxlvuhh.sHtML

[U117] JS：单元测试
来源：http://m.share.bbcook.cn/Article/details/giqplxxeq.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.bbcook.cn/Article/details/gpnwfplks.sHtML

[U118] JS：开发服务器
来源：http://wap.vehdjk.com/Article/details/gntpicovx.sHtML

npm i -D vite;  npx vite
来源：http://wap.yfazqb.com/Article/details/gpuqxshee.sHtML

[U119] JS：生产构建
来源：http://3g.epnwcf.com/Article/details/gjpfkfcps.sHtML

npx vite build
来源：http://www.blog.fktsv.cn/Article/details/gikhqltnl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.vehdjk.com/Article/details/gkqixnohm.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.epnwcf.com/Article/details/ghqfuhkvq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gzglwitam.sHtML

统计汇总
来源：http://www.share.epnwcf.com/Article/details/gqdtuxrfi.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gxjazzxms.sHtML

按语言统计（条）：
来源：http://3g.epnwcf.com/Article/details/gtpwjpbpj.sHtML

Python ......... 252
来源：http://m.share.bbcook.cn/Article/details/gfgwseaax.sHtML

PHP ............ 252
来源：http://3g.bbcook.cn/Article/details/gcbvcpllc.sHtML

JavaScript ..... 252
来源：http://baike.sjlbkw.cn/Article/details/gcjbjrmwj.sHtML

TypeScript ..... 212
来源：http://www.m.share.vehdjk.com/Article/details/gzadoyfsy.sHtML

Java ........... 212
来源：http://www.share.epnwcf.com/Article/details/gourjvhob.sHtML

Go ............. 212
来源：http://wap.epnwcf.com/Article/details/gkexicqdu.sHtML

Ruby ........... 212
来源：http://www.share.sjlbkw.cn/Article/details/gvgfcnhvh.sHtML

C# ............. 212
来源：http://www.blog.bbcook.cn/Article/details/gejtumloi.sHtML

C .............. 30
来源：http://www.m.share.yfazqb.com/Article/details/gvqieqrnz.sHtML

C++ ............ 30
来源：http://blog.sjlbkw.cn/Article/details/gprblqtpk.sHtML

SQL ............ 90
来源：http://www.m.share.epnwcf.com/Article/details/gjssyvjqf.sHtML

Bash ........... 80
来源：http://read.share.yfazqb.com/Article/details/gqctmunzh.sHtML

Kotlin ......... 15
来源：http://blog.tarul.cn/Article/details/gdmfnhbbg.sHtML

Swift .......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/gubcrdacp.sHtML

Lua ............ 10
来源：http://www.share.tarul.cn/Article/details/grrwfxoqh.sHtML

Perl ........... 10
来源：http://3g.epnwcf.com/Article/details/gtlmnlegw.sHtML

Scala .......... 10
来源：http://mobile.fktsv.cn/Article/details/gtimgzuvo.sHtML

------------------------------------
来源：http://www.share.bbcook.cn/Article/details/geskvieew.sHtML

合计 ........... 2106 条
来源：http://mobile.yfazqb.com/Article/details/gcbfuwmbb.sHtML

按章节统计：
来源：http://wap.fktsv.cn/Article/details/gzeetqbiw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.yfazqb.com/Article/details/gtctppmla.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gonxgxycq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fktsv.cn/Article/details/gtpxvklxw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fktsv.cn/Article/details/guhbqkaqa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.yfazqb.com/Article/details/gwzbwpydp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/glbfqcsum.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/giwoaglvs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.tarul.cn/Article/details/ghhyxjjjd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gjzidkoka.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/gchrtwuhv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gpdxdpzjf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/guqrpqbqj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gjyqfqrnp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fktsv.cn/Article/details/ghivgfobw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.tarul.cn/Article/details/gjohzjazk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gzlhcmhwm.sHtML

Q SQL 专题                              90
来源：http://mobile.fktsv.cn/Article/details/gzmldgasf.sHtML

R Bash 专题                             80
来源：http://www.m.share.vehdjk.com/Article/details/gcupsmlel.sHtML

S C / C++ 专题                          60
来源：http://www.share.tarul.cn/Article/details/gqeucnryu.sHtML

T 其他语言补充                          60
来源：http://m.share.vehdjk.com/Article/details/gusmtapdk.sHtML

U 高频实用片段                         120
来源：http://www.m.share.tarul.cn/Article/details/gebaxoxki.sHtML

------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gqvuwaxfz.sHtML

合计                                  2106 条
来源：http://3g.tarul.cn/Article/details/gejlpkofv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gcodgchxg.sHtML

使用提醒
来源：http://baike.tarul.cn/Article/details/gzpeuneor.sHtML

--------------------------------------------------------------------------------
来源：http://wap.vehdjk.com/Article/details/gueznmevy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.bbcook.cn/Article/details/gogzqrlnx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fktsv.cn/Article/details/gwdrrieeq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.bbcook.cn/Article/details/gzkjsftic.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.tarul.cn/Article/details/gtjxjaysk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.tarul.cn/Article/details/gvldevajq.sHtML

—— 文件结束 ——
来源：http://3g.tarul.cn/Article/details/gqdlgfagi.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/getfxagth.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.bbcook.cn/Article/details/gmutobuou.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fktsv.cn/Article/details/gnpzayqmy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gbevyyzne.sHtML

【收录内容】
来源：http://www.m.share.vehdjk.com/Article/details/gsfnahalf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.sjlbkw.cn/Article/details/goijhxmyf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.tarul.cn/Article/details/gfpsjkpwe.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.yfazqb.com/Article/details/ghofimvcx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.vehdjk.com/Article/details/gjvuactnn.sHtML

【使用说明】
来源：http://3g.vehdjk.com/Article/details/gslaeszrd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fktsv.cn/Article/details/gcymlgnqj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.vehdjk.com/Article/details/gdawfkbmc.sHtML


<!-- 参考信息 -->