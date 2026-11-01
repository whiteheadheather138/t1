代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.m.share.vehdjk.com/Article/details/gauglffuj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fktsv.cn/Article/details/gywdxuqpv.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fktsv.cn/Article/details/gudedxuuv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.yfazqb.com/Article/details/gkzlujpdg.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fktsv.cn/Article/details/gsujmvbqp.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/guuxdnwuv.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fktsv.cn/Article/details/ggnivcxio.sHtML

{**a, **b}
来源：http://baike.sjlbkw.cn/Article/details/gpxiajuwj.sHtML

[U07] Py：反转字典键值
来源：http://wap.vehdjk.com/Article/details/gkpatglpc.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.tarul.cn/Article/details/gacdssulj.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.vehdjk.com/Article/details/gmgnbumzj.sHtML

[y for x in nested for y in x]
来源：http://m.share.yfazqb.com/Article/details/gtmxuuhib.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.yfazqb.com/Article/details/gkftldkqk.sHtML

max(d, key=d.get)
来源：http://www.m.share.tarul.cn/Article/details/giitfwpcp.sHtML

[U10] Py：按值排序字典
来源：http://blog.yfazqb.com/Article/details/gacnkfpmv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fktsv.cn/Article/details/gmilkwnni.sHtML

[U11] Py：生成器表达式
来源：http://3g.tarul.cn/Article/details/gyvnwkqbg.sHtML

(x * 2 for x in arr)
来源：http://m.share.tarul.cn/Article/details/gmwtwqsbb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.epnwcf.com/Article/details/ggidhoipv.sHtML

Counter(arr).most_common(3)
来源：http://3g.vehdjk.com/Article/details/gaxijufvd.sHtML

[U13] Py：固定长度队列
来源：http://blog.yfazqb.com/Article/details/goxrhagwa.sHtML

deque(maxlen=10)
来源：http://www.blog.epnwcf.com/Article/details/guavgqznk.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.epnwcf.com/Article/details/gsedgstyo.sHtML

defaultdict(list)
来源：http://baike.bbcook.cn/Article/details/gbzdlufzo.sHtML

[U15] Py：高精度计时
来源：http://blog.epnwcf.com/Article/details/gkpqxwsbw.sHtML

t = time.perf_counter()
来源：http://blog.vehdjk.com/Article/details/gpybgonre.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.yfazqb.com/Article/details/gkkqktbtb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.yfazqb.com/Article/details/getthwtqb.sHtML

[U17] Py：初始化日志
来源：http://wap.vehdjk.com/Article/details/gfqeitqjs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.vehdjk.com/Article/details/gtnjatimb.sHtML

[U18] Py：预编译正则
来源：http://baike.sjlbkw.cn/Article/details/gxtnxhjxt.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.vehdjk.com/Article/details/gjkrqepky.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.sjlbkw.cn/Article/details/godxuszqw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.yfazqb.com/Article/details/ghasvdwkn.sHtML

[U20] Py：缓存函数结果
来源：http://blog.epnwcf.com/Article/details/glhtythcq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fktsv.cn/Article/details/grkozfzxw.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.yfazqb.com/Article/details/gpmynprgp.sHtML

@contextlib.contextmanager
来源：http://www.blog.sjlbkw.cn/Article/details/gbfoueovk.sHtML

[U22] Py：矩阵转置
来源：http://m.share.epnwcf.com/Article/details/gumvtilsk.sHtML

list(zip(*m))
来源：http://baike.yfazqb.com/Article/details/gqczoxcsm.sHtML

[U23] Py：分块读取大文件
来源：http://blog.epnwcf.com/Article/details/ghoqkqhon.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fktsv.cn/Article/details/gmlcvemsl.sHtML

[U24] Py：路径操作
来源：http://www.m.share.yfazqb.com/Article/details/gpgyiqbrc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/giymnpbyp.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.tarul.cn/Article/details/ggqanxymg.sHtML

csv.DictReader(f)
来源：http://www.m.share.fktsv.cn/Article/details/gldxhptqs.sHtML

[U26] Py：并发下载
来源：http://m.share.bbcook.cn/Article/details/gptppvvtd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.sjlbkw.cn/Article/details/gplxcespt.sHtML

[U27] Py：异步 HTTP
来源：http://blog.vehdjk.com/Article/details/gnypyvkmg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/gpwfyjcdc.sHtML

[U28] Py：类型别名
来源：http://m.share.fktsv.cn/Article/details/gjmubrhad.sHtML

UserId = int
来源：http://www.blog.vehdjk.com/Article/details/gnxcfygvu.sHtML

[U29] Py：属性校验
来源：http://baike.yfazqb.com/Article/details/gnvuokrls.sHtML

@property 与 @x.setter 配合
来源：http://mobile.vehdjk.com/Article/details/gcbpexfkt.sHtML

[U30] Py：数据类
来源：http://m.share.tarul.cn/Article/details/gbihwassr.sHtML

@dataclass(slots=True)
来源：http://www.share.epnwcf.com/Article/details/gfvvzglhz.sHtML

[U31] Py：单测
来源：http://www.m.share.epnwcf.com/Article/details/gvnllrzne.sHtML

python -m pytest -q
来源：http://www.share.vehdjk.com/Article/details/gsiykunns.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.tarul.cn/Article/details/gecctzkbc.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.yfazqb.com/Article/details/gfdkggtqg.sHtML

[U33] Py：打包发布
来源：http://wap.vehdjk.com/Article/details/gvodgzzhe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.epnwcf.com/Article/details/gfopexigq.sHtML

[U34] Py：判断编码
来源：http://www.blog.tarul.cn/Article/details/gfrppooka.sHtML

chardet.detect(raw)
来源：http://baike.epnwcf.com/Article/details/gyvuprwjq.sHtML

[U35] Py：发送邮件
来源：http://m.share.sjlbkw.cn/Article/details/gnnxzaaqa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.tarul.cn/Article/details/gxdspueuu.sHtML

[U36] Py：定时任务
来源：http://baike.tarul.cn/Article/details/gbhvqcfry.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.bbcook.cn/Article/details/gwxpuukpi.sHtML

[U37] Py：读写 Excel
来源：http://read.share.yfazqb.com/Article/details/gignjllbb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fktsv.cn/Article/details/gaennnkwj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.epnwcf.com/Article/details/gfucsuwoe.sHtML

Path(__file__).resolve().parent
来源：http://mobile.bbcook.cn/Article/details/gilbuirvv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.epnwcf.com/Article/details/gsjyquzrz.sHtML

sys.stdout.isatty()
来源：http://mobile.epnwcf.com/Article/details/gijbunkto.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.bbcook.cn/Article/details/gtjprscnz.sHtML

print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/ghpyzfqhz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.bbcook.cn/Article/details/gipdkzmpw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.sjlbkw.cn/Article/details/ggocuvzph.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.sjlbkw.cn/Article/details/glnxipbms.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.bbcook.cn/Article/details/griaispxz.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.yfazqb.com/Article/details/ghklkdyzp.sHtML

namespace App\Http;
来源：http://blog.sjlbkw.cn/Article/details/gygtmzfrq.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.tarul.cn/Article/details/gvawjkwbp.sHtML

declare(strict_types=1);
来源：http://read.share.yfazqb.com/Article/details/gubxkkock.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fktsv.cn/Article/details/gfzuomwgt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gmbwqtrrc.sHtML

[U46] PHP：可空类型
来源：http://baike.tarul.cn/Article/details/gzkneqmnf.sHtML

?string $name = null
来源：http://www.share.fktsv.cn/Article/details/gbudliqzo.sHtML

[U47] PHP：联合类型
来源：http://3g.yfazqb.com/Article/details/gqjzgyvki.sHtML

int|string $id
来源：http://blog.sjlbkw.cn/Article/details/guqdudkol.sHtML

[U48] PHP：纯枚举
来源：http://wap.yfazqb.com/Article/details/gxhnqpffx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.epnwcf.com/Article/details/ggbnqcywc.sHtML

[U49] PHP：只读属性
来源：http://blog.tarul.cn/Article/details/gtnjlrzrs.sHtML

public readonly string $name
来源：http://www.blog.vehdjk.com/Article/details/ghcwyunax.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.sjlbkw.cn/Article/details/gjktocdme.sHtML

public function __construct(private int $id) {}
来源：http://m.share.epnwcf.com/Article/details/gtuuixenc.sHtML

[U51] PHP：数组解构
来源：http://m.share.tarul.cn/Article/details/gioikfwdt.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.tarul.cn/Article/details/ghjokgsyl.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/gkcovyhix.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.tarul.cn/Article/details/glmuopvxa.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.yfazqb.com/Article/details/ghiyzallw.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.sjlbkw.cn/Article/details/gggpuybmz.sHtML

[U54] PHP：空安全调用
来源：http://www.share.epnwcf.com/Article/details/gjyowaogt.sHtML

$obj?->method()
来源：http://baike.yfazqb.com/Article/details/gbfouuhyy.sHtML

[U55] PHP：match 表达式
来源：http://blog.fktsv.cn/Article/details/gfzleetry.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfquzlbd.sHtML

[U56] PHP：命名参数
来源：http://baike.tarul.cn/Article/details/gzoxkgbkb.sHtML

f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gmnvzkfdn.sHtML

[U57] PHP：字符串插值
来源：http://wap.bbcook.cn/Article/details/gyxtefjqn.sHtML

"值: {$a}"
来源：http://wap.tarul.cn/Article/details/gsqsnrjgw.sHtML

[U58] PHP：数组三件套
来源：http://m.share.tarul.cn/Article/details/gkovojpis.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.bbcook.cn/Article/details/gfgcluxkc.sHtML

[U59] PHP：自定义排序
来源：http://m.share.vehdjk.com/Article/details/ghbgkazgf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/gpzfswqju.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.bbcook.cn/Article/details/gvcbhnqep.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.tarul.cn/Article/details/gutkqjuwy.sHtML

[U61] PHP：正则
来源：http://www.blog.tarul.cn/Article/details/grdoyeyvv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/gjyggocrc.sHtML

[U62] PHP：日期对象
来源：http://3g.fktsv.cn/Article/details/gvtqvcytc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fktsv.cn/Article/details/gtozcvrpw.sHtML

[U63] PHP：文件读写
来源：http://mobile.yfazqb.com/Article/details/gpcpiagyq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.sjlbkw.cn/Article/details/gvirscznh.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fktsv.cn/Article/details/gwjuglorg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.epnwcf.com/Article/details/gyyqerbzq.sHtML

[U65] PHP：会话
来源：http://www.blog.yfazqb.com/Article/details/gkhjxghgz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.epnwcf.com/Article/details/gwhkapcdy.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fktsv.cn/Article/details/gyolbauiw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.sjlbkw.cn/Article/details/gymbqpqbj.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fktsv.cn/Article/details/gbxigiazs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.sjlbkw.cn/Article/details/glwlmmzlw.sHtML

[U68] PHP：PDO 连接
来源：http://baike.bbcook.cn/Article/details/gaxblkedj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.sjlbkw.cn/Article/details/gpypwyain.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.epnwcf.com/Article/details/gfpcwnzsk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.vehdjk.com/Article/details/gmzszdvnc.sHtML

[U70] PHP：PDO 事务
来源：http://wap.epnwcf.com/Article/details/gvvyrndnh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fktsv.cn/Article/details/gnngjaqaq.sHtML

[U71] PHP：抛出异常
来源：http://wap.tarul.cn/Article/details/guiyomqac.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.bbcook.cn/Article/details/guerrvgjw.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fktsv.cn/Article/details/gnpupjnhk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.epnwcf.com/Article/details/glrigzbrf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.tarul.cn/Article/details/ggshcglkt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.tarul.cn/Article/details/gdjnasdse.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.tarul.cn/Article/details/gctfgixbk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.bbcook.cn/Article/details/gywwhamlo.sHtML

[U75] PHP：依赖注入
来源：http://www.share.vehdjk.com/Article/details/glppmqord.sHtML

composer require psr/container
来源：http://mobile.yfazqb.com/Article/details/gtymhxhuz.sHtML

[U76] PHP：简单路由
来源：http://wap.bbcook.cn/Article/details/gvcbspnat.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.epnwcf.com/Article/details/gilqpxzii.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrtthygf.sHtML

composer require twig/twig
来源：http://3g.vehdjk.com/Article/details/galakuslt.sHtML

[U78] PHP：单元测试
来源：http://www.blog.vehdjk.com/Article/details/goeyszoah.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.yfazqb.com/Article/details/gnxzttchn.sHtML

[U79] PHP：静态分析
来源：http://baike.tarul.cn/Article/details/ghhtulyir.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.epnwcf.com/Article/details/grsdjugrj.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.bbcook.cn/Article/details/gtpogektf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.vehdjk.com/Article/details/gdonmntii.sHtML

[U81] JS：初始化项目
来源：http://www.share.fktsv.cn/Article/details/gnpfomlqf.sHtML

npm init -y;  npm i express
来源：http://m.share.sjlbkw.cn/Article/details/gfdjtslmo.sHtML

[U82] JS：package.json 脚本
来源：http://3g.vehdjk.com/Article/details/gwalyfwcr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.bbcook.cn/Article/details/gqehfcmzm.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.bbcook.cn/Article/details/gruxshtae.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/gtzrttyyb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.bbcook.cn/Article/details/gftvqrqeo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.sjlbkw.cn/Article/details/gwjajkpky.sHtML

[U85] JS：可选链
来源：http://wap.yfazqb.com/Article/details/gsitnrczm.sHtML

a?.b?.c
来源：http://baike.vehdjk.com/Article/details/gmnsifhna.sHtML

[U86] JS：空值合并
来源：http://www.m.share.epnwcf.com/Article/details/gofignnnz.sHtML

a ?? b
来源：http://www.m.share.tarul.cn/Article/details/gzbhbqpdp.sHtML

[U87] JS：解构默认值
来源：http://read.share.fktsv.cn/Article/details/ghmxwzqgj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.yfazqb.com/Article/details/gafzvfvsb.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.vehdjk.com/Article/details/gqgvowyro.sHtML

{ ...a, ...b }
来源：http://wap.vehdjk.com/Article/details/gyzrgwdfq.sHtML

[U89] JS：数组去重
来源：http://blog.bbcook.cn/Article/details/gucazlxgt.sHtML

[...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/giqnhpzhi.sHtML

[U90] JS：数字数组排序
来源：http://wap.tarul.cn/Article/details/gjaioeuoz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/garbrduoy.sHtML

[U91] JS：对象键值遍历
来源：http://blog.bbcook.cn/Article/details/gwstzxsfg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fktsv.cn/Article/details/gxoamwwtd.sHtML

[U92] JS：深拷贝
来源：http://www.blog.epnwcf.com/Article/details/gzircfreq.sHtML

structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gdkblxhzi.sHtML

[U93] JS：模板字符串
来源：http://blog.vehdjk.com/Article/details/gcncpcyzs.sHtML

`共 ${n} 条`
来源：http://wap.fktsv.cn/Article/details/gluozphff.sHtML

[U94] JS：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gjmstxryf.sHtML

const double = x => x * 2;
来源：http://baike.fktsv.cn/Article/details/gmlhwawhx.sHtML

[U95] JS：Promise 包装
来源：http://baike.tarul.cn/Article/details/gaghctegw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.bbcook.cn/Article/details/gduczeelq.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fktsv.cn/Article/details/gyavzszfi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gqwhcocsi.sHtML

[U97] JS：并发请求
来源：http://www.blog.sjlbkw.cn/Article/details/grtgudwvw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gsgdldvaz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.epnwcf.com/Article/details/gqsfadccg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.sjlbkw.cn/Article/details/giwzznrgv.sHtML

[U99] JS：事件监听
来源：http://blog.bbcook.cn/Article/details/gamlafbuy.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.bbcook.cn/Article/details/gucdhwmgd.sHtML

[U100] JS：DOM 查询
来源：http://blog.vehdjk.com/Article/details/gjkbjpizw.sHtML

document.querySelector(".item")
来源：http://www.share.vehdjk.com/Article/details/gexcmrghd.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.bbcook.cn/Article/details/glshqrwmy.sHtML

el.classList.toggle("active")
来源：http://blog.bbcook.cn/Article/details/gtlqaafxy.sHtML

[U102] JS：本地存储
来源：http://www.blog.yfazqb.com/Article/details/gtgugblna.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.tarul.cn/Article/details/girbnvgeh.sHtML

[U103] JS：定时器
来源：http://www.m.share.sjlbkw.cn/Article/details/grpnqxfjf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fktsv.cn/Article/details/gqcfiqckq.sHtML

[U104] JS：防抖
来源：http://read.share.epnwcf.com/Article/details/gjeipftlp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/gczificvp.sHtML

[U105] JS：节流
来源：http://3g.vehdjk.com/Article/details/ggzabscsu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fktsv.cn/Article/details/glnfldnky.sHtML

[U106] JS：日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gekntccte.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.bbcook.cn/Article/details/gypziegbr.sHtML

[U107] JS：数字千分位
来源：http://blog.bbcook.cn/Article/details/gkisupwpv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.vehdjk.com/Article/details/gxqjqxlkj.sHtML

[U108] JS：随机整数
来源：http://www.share.yfazqb.com/Article/details/gkfwkepnj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.bbcook.cn/Article/details/gkjqldnme.sHtML

[U109] JS：数组分组
来源：http://baike.fktsv.cn/Article/details/gvssqldhc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/grnysvexc.sHtML

[U110] JS：数组分块
来源：http://www.share.bbcook.cn/Article/details/gquaumuex.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fktsv.cn/Article/details/ggnsqihfm.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkpulzpk.sHtML

new Map(Object.entries(obj))
来源：http://baike.yfazqb.com/Article/details/ggurgpeei.sHtML

[U112] JS：字符串补位
来源：http://3g.bbcook.cn/Article/details/guezwfoux.sHtML

"7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/ggfdfyvhg.sHtML

[U113] JS：正则替换全部
来源：http://blog.tarul.cn/Article/details/gcjukwefn.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gpgsgqqud.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.sjlbkw.cn/Article/details/gdaxpczjm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gescuzxaj.sHtML

[U115] JS：生成 UUID
来源：http://mobile.vehdjk.com/Article/details/gwxxkjymk.sHtML

crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gioklucxl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.yfazqb.com/Article/details/gwcuwtiwf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fktsv.cn/Article/details/gsmkvoerr.sHtML

[U117] JS：单元测试
来源：http://m.share.fktsv.cn/Article/details/gmvdexlan.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.yfazqb.com/Article/details/gqzkwfhvj.sHtML

[U118] JS：开发服务器
来源：http://baike.vehdjk.com/Article/details/gqnjpntpx.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fktsv.cn/Article/details/govjbnwgf.sHtML

[U119] JS：生产构建
来源：http://www.blog.epnwcf.com/Article/details/gfubfvbuj.sHtML

npx vite build
来源：http://m.share.yfazqb.com/Article/details/gekdwauhu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.yfazqb.com/Article/details/gvrspcvag.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.vehdjk.com/Article/details/gyvccfmft.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ggnxaoizq.sHtML

统计汇总
来源：http://www.m.share.bbcook.cn/Article/details/ggcdewhqr.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvcgfklgo.sHtML

按语言统计（条）：
来源：http://blog.sjlbkw.cn/Article/details/gprerlkxt.sHtML

Python ......... 252
来源：http://blog.vehdjk.com/Article/details/goahtzoli.sHtML

PHP ............ 252
来源：http://read.share.tarul.cn/Article/details/gyhhxbkwk.sHtML

JavaScript ..... 252
来源：http://read.share.tarul.cn/Article/details/gzhminrsm.sHtML

TypeScript ..... 212
来源：http://wap.yfazqb.com/Article/details/gykmoefyl.sHtML

Java ........... 212
来源：http://baike.epnwcf.com/Article/details/gepurpyat.sHtML

Go ............. 212
来源：http://blog.yfazqb.com/Article/details/glmvyrcvh.sHtML

Ruby ........... 212
来源：http://baike.fktsv.cn/Article/details/glcwgzaoq.sHtML

C# ............. 212
来源：http://blog.bbcook.cn/Article/details/ghfgdkhbt.sHtML

C .............. 30
来源：http://www.m.share.fktsv.cn/Article/details/gixydmcng.sHtML

C++ ............ 30
来源：http://3g.fktsv.cn/Article/details/gfmpagpvp.sHtML

SQL ............ 90
来源：http://3g.fktsv.cn/Article/details/gkzttaewh.sHtML

Bash ........... 80
来源：http://m.share.bbcook.cn/Article/details/ghzmjxepz.sHtML

Kotlin ......... 15
来源：http://mobile.tarul.cn/Article/details/ggttzxvbv.sHtML

Swift .......... 15
来源：http://wap.bbcook.cn/Article/details/govfhzcbi.sHtML

Lua ............ 10
来源：http://www.share.sjlbkw.cn/Article/details/gxruhdsdd.sHtML

Perl ........... 10
来源：http://www.m.share.fktsv.cn/Article/details/gcearisre.sHtML

Scala .......... 10
来源：http://3g.tarul.cn/Article/details/gpefqwuqu.sHtML

------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gnidwclpg.sHtML

合计 ........... 2106 条
来源：http://wap.epnwcf.com/Article/details/godsqrgnp.sHtML

按章节统计：
来源：http://www.share.bbcook.cn/Article/details/gwsofinwd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fktsv.cn/Article/details/ghnppghxq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gpdjpposl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gaaulkkly.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.sjlbkw.cn/Article/details/gzobvplko.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fktsv.cn/Article/details/guvlzuyei.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.tarul.cn/Article/details/ggrontbce.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gsvvqjlyd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/gexndbkhs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gxvrgwlul.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.epnwcf.com/Article/details/gmbhokpln.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gvvkyjdmx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gxsmcjbom.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/ggjuxcrgw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.vehdjk.com/Article/details/ggsfmdwzx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.yfazqb.com/Article/details/gtrkhqnqz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gntrxnoij.sHtML

Q SQL 专题                              90
来源：http://wap.tarul.cn/Article/details/gtxfjltrn.sHtML

R Bash 专题                             80
来源：http://m.share.fktsv.cn/Article/details/gykppbxmw.sHtML

S C / C++ 专题                          60
来源：http://mobile.bbcook.cn/Article/details/ggklgyzzz.sHtML

T 其他语言补充                          60
来源：http://m.share.vehdjk.com/Article/details/ggsetxvip.sHtML

U 高频实用片段                         120
来源：http://m.share.yfazqb.com/Article/details/gmqnyqowl.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/gbblcmjlx.sHtML

合计                                  2106 条
来源：http://wap.fktsv.cn/Article/details/gsgepobmy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/goseppgxn.sHtML

使用提醒
来源：http://mobile.sjlbkw.cn/Article/details/gavxdhaqc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gagckwexp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.bbcook.cn/Article/details/gchqhgufj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.epnwcf.com/Article/details/gohcjlpts.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.vehdjk.com/Article/details/grwrellkz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.yfazqb.com/Article/details/guuzvihfn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.vehdjk.com/Article/details/giwqmyukt.sHtML

—— 文件结束 ——
来源：http://wap.yfazqb.com/Article/details/gafburbws.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gejbkdrin.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.bbcook.cn/Article/details/gjmfuvhpg.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.tarul.cn/Article/details/glyhthagf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gymcjflpr.sHtML

【收录内容】
来源：http://read.share.bbcook.cn/Article/details/gonbobwob.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.vehdjk.com/Article/details/gtobeezui.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.sjlbkw.cn/Article/details/gypfsvwge.sHtML

SQL · Bash · C · C++
来源：http://blog.bbcook.cn/Article/details/gfoydjrpx.sHtML


<!-- 参考信息 -->