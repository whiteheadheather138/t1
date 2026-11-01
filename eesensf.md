代发 wailian999

[U03] Py：加载 .env 配置
来源：http://blog.tarul.cn/Article/details/gzswtaohk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.bbcook.cn/Article/details/gdsvzmaoo.sHtML

[U04] Py：变量调试打印
来源：http://blog.epnwcf.com/Article/details/gpwpfyzvc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.sjlbkw.cn/Article/details/gomescegb.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.bbcook.cn/Article/details/gjgazsnya.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gbtlzodpi.sHtML

[U06] Py：合并两个字典
来源：http://blog.sjlbkw.cn/Article/details/gyxdxvcpc.sHtML

{**a, **b}
来源：http://mobile.tarul.cn/Article/details/gymytkbdb.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fktsv.cn/Article/details/gbzlcrkcl.sHtML

{v: k for k, v in d.items()}
来源：http://baike.epnwcf.com/Article/details/gebpbhpnn.sHtML

[U08] Py：展平二维列表
来源：http://wap.fktsv.cn/Article/details/ggrvhiily.sHtML

[y for x in nested for y in x]
来源：http://wap.tarul.cn/Article/details/ggelqjkub.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.bbcook.cn/Article/details/gzdgmjwzu.sHtML

max(d, key=d.get)
来源：http://blog.sjlbkw.cn/Article/details/ghatoazrg.sHtML

[U10] Py：按值排序字典
来源：http://read.share.bbcook.cn/Article/details/gmctqsyca.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fktsv.cn/Article/details/gmlgrsfzg.sHtML

[U11] Py：生成器表达式
来源：http://www.share.vehdjk.com/Article/details/gitzymbet.sHtML

(x * 2 for x in arr)
来源：http://mobile.vehdjk.com/Article/details/gdaobeyhs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fktsv.cn/Article/details/gbbypgbpq.sHtML

Counter(arr).most_common(3)
来源：http://www.share.yfazqb.com/Article/details/gwqbdpitm.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fktsv.cn/Article/details/gdmsfozan.sHtML

deque(maxlen=10)
来源：http://blog.vehdjk.com/Article/details/gsheemija.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.vehdjk.com/Article/details/gwsbsyied.sHtML

defaultdict(list)
来源：http://read.share.sjlbkw.cn/Article/details/ghsnbairn.sHtML

[U15] Py：高精度计时
来源：http://3g.fktsv.cn/Article/details/gfxpmzjqi.sHtML

t = time.perf_counter()
来源：http://mobile.epnwcf.com/Article/details/gdolpgqif.sHtML

[U16] Py：命令行参数解析
来源：http://blog.vehdjk.com/Article/details/gzbbigdyh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaajnkzaw.sHtML

[U17] Py：初始化日志
来源：http://baike.bbcook.cn/Article/details/gdqultmjv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.vehdjk.com/Article/details/gbcnahvmy.sHtML

[U18] Py：预编译正则
来源：http://blog.yfazqb.com/Article/details/glyvhsbgg.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fktsv.cn/Article/details/gntclmkii.sHtML

[U19] Py：正则替换带回调
来源：http://3g.epnwcf.com/Article/details/gcnfunxdi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.tarul.cn/Article/details/gediiwkqz.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.bbcook.cn/Article/details/gcdbihhca.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.epnwcf.com/Article/details/gqzthrpdd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.bbcook.cn/Article/details/gimfytvkf.sHtML

@contextlib.contextmanager
来源：http://m.share.sjlbkw.cn/Article/details/gwfblohdf.sHtML

[U22] Py：矩阵转置
来源：http://www.share.sjlbkw.cn/Article/details/gmllvrecy.sHtML

list(zip(*m))
来源：http://mobile.yfazqb.com/Article/details/gavwwnjpq.sHtML

[U23] Py：分块读取大文件
来源：http://3g.tarul.cn/Article/details/giztorbqo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.tarul.cn/Article/details/gycqboysy.sHtML

[U24] Py：路径操作
来源：http://mobile.yfazqb.com/Article/details/gfkughchj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.sjlbkw.cn/Article/details/gvnktburi.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.tarul.cn/Article/details/gqzhrwgjr.sHtML

csv.DictReader(f)
来源：http://www.blog.epnwcf.com/Article/details/gvslovytj.sHtML

[U26] Py：并发下载
来源：http://www.blog.fktsv.cn/Article/details/gmiukceyg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.tarul.cn/Article/details/goxzgaxlc.sHtML

[U27] Py：异步 HTTP
来源：http://baike.bbcook.cn/Article/details/gyfkvutln.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.bbcook.cn/Article/details/gdkwozuzz.sHtML

[U28] Py：类型别名
来源：http://www.share.epnwcf.com/Article/details/gfrqadhuy.sHtML

UserId = int
来源：http://baike.epnwcf.com/Article/details/gjbozgcat.sHtML

[U29] Py：属性校验
来源：http://mobile.vehdjk.com/Article/details/gmmccmfnh.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fktsv.cn/Article/details/gwcnjosbf.sHtML

[U30] Py：数据类
来源：http://www.share.bbcook.cn/Article/details/glmhhfscg.sHtML

@dataclass(slots=True)
来源：http://www.m.share.bbcook.cn/Article/details/gmasuseoz.sHtML

[U31] Py：单测
来源：http://www.m.share.vehdjk.com/Article/details/gdpixfncl.sHtML

python -m pytest -q
来源：http://www.share.fktsv.cn/Article/details/gcfdkvbgl.sHtML

[U32] Py：代码格式化
来源：http://blog.tarul.cn/Article/details/gzzsvxknv.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.bbcook.cn/Article/details/gdsvavbtw.sHtML

[U33] Py：打包发布
来源：http://baike.fktsv.cn/Article/details/guhknadqd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.epnwcf.com/Article/details/gfikjshmb.sHtML

[U34] Py：判断编码
来源：http://www.share.yfazqb.com/Article/details/gxhbnquev.sHtML

chardet.detect(raw)
来源：http://read.share.vehdjk.com/Article/details/glholadhf.sHtML

[U35] Py：发送邮件
来源：http://wap.epnwcf.com/Article/details/gvarjhkqi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.epnwcf.com/Article/details/ghgmkvcet.sHtML

[U36] Py：定时任务
来源：http://blog.fktsv.cn/Article/details/gtscawkxo.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.yfazqb.com/Article/details/gmqzseuqm.sHtML

[U37] Py：读写 Excel
来源：http://wap.sjlbkw.cn/Article/details/gnxjqizgt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fktsv.cn/Article/details/gwphumpxs.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.tarul.cn/Article/details/gkqnryzpd.sHtML

Path(__file__).resolve().parent
来源：http://wap.tarul.cn/Article/details/grwqjrlou.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.tarul.cn/Article/details/gbmredvwi.sHtML

sys.stdout.isatty()
来源：http://mobile.yfazqb.com/Article/details/goghjcpim.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fktsv.cn/Article/details/guvpyzvyt.sHtML

print("err", file=sys.stderr)
来源：http://wap.sjlbkw.cn/Article/details/ggdbnxwfx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.sjlbkw.cn/Article/details/ggujaqett.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.tarul.cn/Article/details/gutjvqzqq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.yfazqb.com/Article/details/gilxfarvo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fktsv.cn/Article/details/guuzcghdw.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.yfazqb.com/Article/details/gmjeggdze.sHtML

namespace App\Http;
来源：http://www.m.share.epnwcf.com/Article/details/gyavtqjdt.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fktsv.cn/Article/details/gcmfibocj.sHtML

declare(strict_types=1);
来源：http://wap.yfazqb.com/Article/details/grxookfkw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fktsv.cn/Article/details/gpwyayowt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gomfniahl.sHtML

[U46] PHP：可空类型
来源：http://3g.bbcook.cn/Article/details/gptsvpcun.sHtML

?string $name = null
来源：http://mobile.vehdjk.com/Article/details/gxpeqgzdx.sHtML

[U47] PHP：联合类型
来源：http://wap.epnwcf.com/Article/details/gbyyqjdjc.sHtML

int|string $id
来源：http://www.m.share.tarul.cn/Article/details/gonjzupca.sHtML

[U48] PHP：纯枚举
来源：http://blog.vehdjk.com/Article/details/gxpamzjle.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.sjlbkw.cn/Article/details/gkjubesrz.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.bbcook.cn/Article/details/gbjiqmvqt.sHtML

public readonly string $name
来源：http://mobile.sjlbkw.cn/Article/details/gmmuttyui.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fktsv.cn/Article/details/glfgtlmvi.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.yfazqb.com/Article/details/gbzefmqzx.sHtML

[U51] PHP：数组解构
来源：http://mobile.fktsv.cn/Article/details/gckqlhbah.sHtML

[$a, $b] = $arr;
来源：http://wap.yfazqb.com/Article/details/gsvzjadog.sHtML

[U52] PHP：箭头函数
来源：http://www.share.epnwcf.com/Article/details/gwncuyatg.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fktsv.cn/Article/details/gvvjeivjf.sHtML

[U53] PHP：空合并运算符
来源：http://3g.bbcook.cn/Article/details/gnzbjqsbq.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.tarul.cn/Article/details/grbbwcnjr.sHtML

[U54] PHP：空安全调用
来源：http://blog.tarul.cn/Article/details/gaonwbdak.sHtML

$obj?->method()
来源：http://www.blog.tarul.cn/Article/details/gjkrxvnyf.sHtML

[U55] PHP：match 表达式
来源：http://wap.tarul.cn/Article/details/gcfpwbxss.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/grfpycvsx.sHtML

[U56] PHP：命名参数
来源：http://read.share.sjlbkw.cn/Article/details/gkoslwajp.sHtML

f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gpwohfllj.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gtuicclup.sHtML

"值: {$a}"
来源：http://read.share.fktsv.cn/Article/details/gbpywuirn.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.epnwcf.com/Article/details/ggzepkcuz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.yfazqb.com/Article/details/gnwwvovgw.sHtML

[U59] PHP：自定义排序
来源：http://baike.bbcook.cn/Article/details/gmycgexoi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzljfpwhq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.epnwcf.com/Article/details/gwrzcpnwt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fktsv.cn/Article/details/gneorydgy.sHtML

[U61] PHP：正则
来源：http://www.share.sjlbkw.cn/Article/details/ghkwtkjbd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.vehdjk.com/Article/details/gvayqfaqg.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fktsv.cn/Article/details/grdbzjmpw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.epnwcf.com/Article/details/guaizdxux.sHtML

[U63] PHP：文件读写
来源：http://3g.fktsv.cn/Article/details/gfqpkadex.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.yfazqb.com/Article/details/ggxcnbzgz.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.tarul.cn/Article/details/gitvduavt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.tarul.cn/Article/details/geeendgzf.sHtML

[U65] PHP：会话
来源：http://read.share.epnwcf.com/Article/details/gzgjwmgab.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gfrsxvyuh.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.sjlbkw.cn/Article/details/gxfvnbbiq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.vehdjk.com/Article/details/gyjshqtyn.sHtML

[U67] PHP：处理文件上传
来源：http://blog.sjlbkw.cn/Article/details/gqyroucfh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.vehdjk.com/Article/details/ginseguee.sHtML

[U68] PHP：PDO 连接
来源：http://baike.bbcook.cn/Article/details/gmokyhgvk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.yfazqb.com/Article/details/gyxfhlpmr.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.vehdjk.com/Article/details/gysulglkv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.epnwcf.com/Article/details/gljbammat.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fktsv.cn/Article/details/gdnrnghim.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.sjlbkw.cn/Article/details/gvethwaon.sHtML

[U71] PHP：抛出异常
来源：http://mobile.epnwcf.com/Article/details/grgwytzrz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.yfazqb.com/Article/details/gskuyaujx.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.vehdjk.com/Article/details/gnrgtalnc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.yfazqb.com/Article/details/giparlgyw.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.epnwcf.com/Article/details/gguptdfde.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fktsv.cn/Article/details/gjgtpvmbz.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.tarul.cn/Article/details/gethnljku.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.epnwcf.com/Article/details/gvhtlngxt.sHtML

[U75] PHP：依赖注入
来源：http://3g.vehdjk.com/Article/details/gqmaampwg.sHtML

composer require psr/container
来源：http://baike.fktsv.cn/Article/details/glgaeipja.sHtML

[U76] PHP：简单路由
来源：http://read.share.sjlbkw.cn/Article/details/gsqwrpuyp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.yfazqb.com/Article/details/gyvwkaegf.sHtML

[U77] PHP：模板渲染
来源：http://blog.yfazqb.com/Article/details/gcqdyrisn.sHtML

composer require twig/twig
来源：http://www.share.sjlbkw.cn/Article/details/gobthnsbw.sHtML

[U78] PHP：单元测试
来源：http://3g.yfazqb.com/Article/details/gidnnimvf.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.yfazqb.com/Article/details/gawuhjbqk.sHtML

[U79] PHP：静态分析
来源：http://read.share.tarul.cn/Article/details/gbapdiwuz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fktsv.cn/Article/details/gditdmpeb.sHtML

[U80] PHP：代码规范修复
来源：http://baike.sjlbkw.cn/Article/details/gcjmxigwn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.tarul.cn/Article/details/gcqrmgbva.sHtML

[U81] JS：初始化项目
来源：http://blog.vehdjk.com/Article/details/ggczgjusr.sHtML

npm init -y;  npm i express
来源：http://www.blog.sjlbkw.cn/Article/details/gncpulkrf.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.sjlbkw.cn/Article/details/gksrypite.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.bbcook.cn/Article/details/grxpebwxe.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.epnwcf.com/Article/details/guljhrwow.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.yfazqb.com/Article/details/gmzfbnogz.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.epnwcf.com/Article/details/glifpkmyy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.tarul.cn/Article/details/gtmljxvhr.sHtML

[U85] JS：可选链
来源：http://www.share.tarul.cn/Article/details/ghubhhxgh.sHtML

a?.b?.c
来源：http://baike.bbcook.cn/Article/details/gcetbgfhr.sHtML

[U86] JS：空值合并
来源：http://baike.vehdjk.com/Article/details/gvlxrwqla.sHtML

a ?? b
来源：http://3g.fktsv.cn/Article/details/grithdrap.sHtML

[U87] JS：解构默认值
来源：http://read.share.bbcook.cn/Article/details/gwtcvihsh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.yfazqb.com/Article/details/gmevbicex.sHtML

[U88] JS：对象展开合并
来源：http://baike.tarul.cn/Article/details/gnnybgilw.sHtML

{ ...a, ...b }
来源：http://blog.tarul.cn/Article/details/gtfskhhsu.sHtML

[U89] JS：数组去重
来源：http://blog.bbcook.cn/Article/details/gdjatyorv.sHtML

[...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gnnbwtuoh.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.vehdjk.com/Article/details/gvpeihsbs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gylfbridv.sHtML

[U91] JS：对象键值遍历
来源：http://3g.bbcook.cn/Article/details/gbsbjqyrp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.bbcook.cn/Article/details/guiktvmwi.sHtML

[U92] JS：深拷贝
来源：http://mobile.fktsv.cn/Article/details/gqmtqxbdp.sHtML

structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gxlkhwrjf.sHtML

[U93] JS：模板字符串
来源：http://read.share.fktsv.cn/Article/details/gkyzxacwp.sHtML

`共 ${n} 条`
来源：http://www.share.tarul.cn/Article/details/gwfiyrlar.sHtML

[U94] JS：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gwnsmohoh.sHtML

const double = x => x * 2;
来源：http://wap.tarul.cn/Article/details/gxdjzzrhx.sHtML

[U95] JS：Promise 包装
来源：http://read.share.yfazqb.com/Article/details/gibmjuztw.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.tarul.cn/Article/details/gmzjxxaar.sHtML

[U96] JS：async/await 与异常
来源：http://wap.bbcook.cn/Article/details/glfatcysw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gbwiqesrp.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/gassqnrxs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gzxumsupt.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gcaklkvmz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.tarul.cn/Article/details/gidigdqkg.sHtML

[U99] JS：事件监听
来源：http://read.share.fktsv.cn/Article/details/gdbcuaqxm.sHtML

el.addEventListener("click", e => {})
来源：http://baike.tarul.cn/Article/details/gtsdrgsoq.sHtML

[U100] JS：DOM 查询
来源：http://www.share.vehdjk.com/Article/details/giiukggxm.sHtML

document.querySelector(".item")
来源：http://3g.tarul.cn/Article/details/gjfznroay.sHtML

[U101] JS：classList 操作
来源：http://mobile.fktsv.cn/Article/details/gxjbixwpj.sHtML

el.classList.toggle("active")
来源：http://www.m.share.epnwcf.com/Article/details/gjfefahts.sHtML

[U102] JS：本地存储
来源：http://www.blog.bbcook.cn/Article/details/gtrtrkwvt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.sjlbkw.cn/Article/details/gsjbztlck.sHtML

[U103] JS：定时器
来源：http://mobile.bbcook.cn/Article/details/gcauxnawl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fktsv.cn/Article/details/gfmoicbak.sHtML

[U104] JS：防抖
来源：http://blog.epnwcf.com/Article/details/ghagoazvz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gmwkbovvy.sHtML

[U105] JS：节流
来源：http://3g.vehdjk.com/Article/details/gjigtdkvs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.tarul.cn/Article/details/gwdkcpftg.sHtML

[U106] JS：日期格式化
来源：http://3g.epnwcf.com/Article/details/gkydljgbu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.sjlbkw.cn/Article/details/gpwiofiuz.sHtML

[U107] JS：数字千分位
来源：http://m.share.fktsv.cn/Article/details/gqccklpoo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.yfazqb.com/Article/details/gicorpkum.sHtML

[U108] JS：随机整数
来源：http://read.share.bbcook.cn/Article/details/gcxtdisnb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.bbcook.cn/Article/details/gkqpcdvzc.sHtML

[U109] JS：数组分组
来源：http://www.blog.yfazqb.com/Article/details/gddibuxfo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/guiqpasrp.sHtML

[U110] JS：数组分块
来源：http://www.blog.yfazqb.com/Article/details/gqesqemqj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.vehdjk.com/Article/details/gzrugeskl.sHtML

[U111] JS：对象转 Map
来源：http://3g.vehdjk.com/Article/details/gnoqjvagb.sHtML

new Map(Object.entries(obj))
来源：http://read.share.epnwcf.com/Article/details/gtijbxwdc.sHtML

[U112] JS：字符串补位
来源：http://m.share.fktsv.cn/Article/details/gnsblvbbl.sHtML

"7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/grwutjrgx.sHtML

[U113] JS：正则替换全部
来源：http://blog.yfazqb.com/Article/details/gacsudbfw.sHtML

s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gshgglthg.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fktsv.cn/Article/details/gahucyroc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/gwzzujgqi.sHtML

[U115] JS：生成 UUID
来源：http://mobile.sjlbkw.cn/Article/details/gbosozksn.sHtML

crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gjoofhosz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.sjlbkw.cn/Article/details/giauewthj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.vehdjk.com/Article/details/ggwdjfkmr.sHtML

[U117] JS：单元测试
来源：http://read.share.tarul.cn/Article/details/gyblibcpj.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.tarul.cn/Article/details/gbapjdeho.sHtML

[U118] JS：开发服务器
来源：http://m.share.bbcook.cn/Article/details/gwwxtnust.sHtML

npm i -D vite;  npx vite
来源：http://wap.bbcook.cn/Article/details/gdgkahhdg.sHtML

[U119] JS：生产构建
来源：http://www.m.share.tarul.cn/Article/details/golarcmrh.sHtML

npx vite build
来源：http://wap.sjlbkw.cn/Article/details/gjinfdxxk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.vehdjk.com/Article/details/gpsdwohsk.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.sjlbkw.cn/Article/details/gguxvpwed.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gssprpmpn.sHtML

统计汇总
来源：http://baike.yfazqb.com/Article/details/gbhipsmgt.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/grzogtudz.sHtML

按语言统计（条）：
来源：http://read.share.sjlbkw.cn/Article/details/glodkvvvo.sHtML

Python ......... 252
来源：http://3g.tarul.cn/Article/details/gedeylnuc.sHtML

PHP ............ 252
来源：http://www.m.share.yfazqb.com/Article/details/gxpfoaypn.sHtML

JavaScript ..... 252
来源：http://wap.tarul.cn/Article/details/gobaenleo.sHtML

TypeScript ..... 212
来源：http://3g.epnwcf.com/Article/details/gzrllxhen.sHtML

Java ........... 212
来源：http://www.share.fktsv.cn/Article/details/gyqrvgfqk.sHtML

Go ............. 212
来源：http://read.share.bbcook.cn/Article/details/gydoykszm.sHtML

Ruby ........... 212
来源：http://mobile.sjlbkw.cn/Article/details/gsboqweko.sHtML

C# ............. 212
来源：http://blog.tarul.cn/Article/details/gctfseday.sHtML

C .............. 30
来源：http://www.share.epnwcf.com/Article/details/ghrdlcrnb.sHtML

C++ ............ 30
来源：http://read.share.fktsv.cn/Article/details/grxdbiaxo.sHtML

SQL ............ 90
来源：http://www.share.fktsv.cn/Article/details/guocfpmqo.sHtML

Bash ........... 80
来源：http://www.m.share.bbcook.cn/Article/details/gmgtsxsjp.sHtML

Kotlin ......... 15
来源：http://wap.fktsv.cn/Article/details/gpifmfcuq.sHtML

Swift .......... 15
来源：http://3g.yfazqb.com/Article/details/gnpofwoac.sHtML

Lua ............ 10
来源：http://www.blog.bbcook.cn/Article/details/gfpvwwhuh.sHtML

Perl ........... 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyyefijr.sHtML

Scala .......... 10
来源：http://m.share.vehdjk.com/Article/details/groteusdu.sHtML

------------------------------------
来源：http://blog.yfazqb.com/Article/details/gmkyziphd.sHtML

合计 ........... 2106 条
来源：http://m.share.vehdjk.com/Article/details/gaiujkwat.sHtML

按章节统计：
来源：http://mobile.yfazqb.com/Article/details/gylzuvklg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/gujktbwro.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.bbcook.cn/Article/details/geeamtagi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/gosgqpuqy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.vehdjk.com/Article/details/gtobabuxz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fktsv.cn/Article/details/gflewkysu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/gecmogguy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/ghojnmwwi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.sjlbkw.cn/Article/details/giorvqrjf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/ggzpjvvrn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.bbcook.cn/Article/details/gsjfjghlm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gqwxucvmc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gsofbtszu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gddzubgag.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.epnwcf.com/Article/details/galtpklfx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.sjlbkw.cn/Article/details/gfxddgcty.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gyfgjsqsa.sHtML

Q SQL 专题                              90
来源：http://3g.vehdjk.com/Article/details/gmcidowfn.sHtML

R Bash 专题                             80
来源：http://baike.epnwcf.com/Article/details/gszwiohvs.sHtML

S C / C++ 专题                          60
来源：http://blog.epnwcf.com/Article/details/gvhzcyffp.sHtML

T 其他语言补充                          60
来源：http://www.share.bbcook.cn/Article/details/gihbnhrps.sHtML

U 高频实用片段                         120
来源：http://mobile.fktsv.cn/Article/details/gxdjseryb.sHtML

------------------------------------
来源：http://wap.tarul.cn/Article/details/gfhfczvao.sHtML

合计                                  2106 条
来源：http://read.share.epnwcf.com/Article/details/gtjwzfvne.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gldzvvqpr.sHtML

使用提醒
来源：http://mobile.tarul.cn/Article/details/goreedfwe.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.tarul.cn/Article/details/gkchwofbd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.bbcook.cn/Article/details/gzsxtdjui.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fktsv.cn/Article/details/ghrtvzbqf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.epnwcf.com/Article/details/gptxxktbh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.yfazqb.com/Article/details/gxshvngob.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fktsv.cn/Article/details/gktxmnmzg.sHtML

—— 文件结束 ——
来源：http://baike.bbcook.cn/Article/details/gapsceatv.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfcexmiud.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.epnwcf.com/Article/details/gorfeqkjm.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fktsv.cn/Article/details/gaaxkcish.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjslkbatl.sHtML

【收录内容】
来源：http://m.share.vehdjk.com/Article/details/gfpffoqcx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.sjlbkw.cn/Article/details/gslthntwt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.epnwcf.com/Article/details/gefleryec.sHtML

SQL · Bash · C · C++
来源：http://3g.bbcook.cn/Article/details/gltsqbllm.sHtML


<!-- 参考信息 -->